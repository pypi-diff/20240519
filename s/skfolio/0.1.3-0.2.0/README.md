# Comparing `tmp/skfolio-0.1.3.tar.gz` & `tmp/skfolio-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skfolio-0.1.3.tar", last modified: Wed Mar 13 08:19:59 2024, max compression
+gzip compressed data, was "skfolio-0.2.0.tar", last modified: Sun May 19 21:47:56 2024, max compression
```

## Comparing `skfolio-0.1.3.tar` & `skfolio-0.2.0.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 08:19:59.914672 skfolio-0.1.3/
--rw-r--r--   0 root         (0) root         (0)     1526 2024-03-13 08:19:55.000000 skfolio-0.1.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       48 2024-03-13 08:19:55.000000 skfolio-0.1.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    19590 2024-03-13 08:19:59.914672 skfolio-0.1.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    15352 2024-03-13 08:19:55.000000 skfolio-0.1.3/README.rst
--rw-r--r--   0 root         (0) root         (0)     3470 2024-03-13 08:19:56.000000 skfolio-0.1.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-13 08:19:59.914672 skfolio-0.1.3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 08:19:59.886672 skfolio-0.1.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 08:19:59.894672 skfolio-0.1.3/src/skfolio/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 08:19:59.894672 skfolio-0.1.3/src/skfolio/cluster/
--rw-r--r--   0 root         (0) root         (0)      251 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/cluster/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12817 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/cluster/_hierarchical.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 08:19:59.894672 skfolio-0.1.3/src/skfolio/datasets/
--rw-r--r--   0 root         (0) root         (0)      407 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/datasets/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13952 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/datasets/_base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 08:19:59.894672 skfolio-0.1.3/src/skfolio/datasets/data/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/datasets/data/__init__.py
--rw-r--r--   0 root         (0) root         (0)    36146 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/datasets/data/factors_dataset.csv.gz
--rw-r--r--   0 root         (0) root         (0)   426065 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/datasets/data/sp500_dataset.csv.gz
--rw-r--r--   0 root         (0) root         (0)    41898 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/datasets/data/sp500_index.csv.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 08:19:59.898672 skfolio-0.1.3/src/skfolio/distance/
--rw-r--r--   0 root         (0) root         (0)      547 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/distance/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1326 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/distance/_base.py
--rw-r--r--   0 root         (0) root         (0)    18538 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/distance/_distance.py
--rw-r--r--   0 root         (0) root         (0)      662 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 08:19:59.898672 skfolio-0.1.3/src/skfolio/measures/
--rw-r--r--   0 root         (0) root         (0)     1631 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/measures/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8934 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/measures/_enums.py
--rw-r--r--   0 root         (0) root         (0)    16829 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/measures/_measures.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 08:19:59.898672 skfolio-0.1.3/src/skfolio/metrics/
--rw-r--r--   0 root         (0) root         (0)       75 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/metrics/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4306 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/metrics/_scorer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 08:19:59.898672 skfolio-0.1.3/src/skfolio/model_selection/
--rw-r--r--   0 root         (0) root         (0)      453 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/model_selection/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14782 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/model_selection/_combinatorial.py
--rw-r--r--   0 root         (0) root         (0)     7686 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/model_selection/_validation.py
--rw-r--r--   0 root         (0) root         (0)     7539 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/model_selection/_walk_forward.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 08:19:59.898672 skfolio-0.1.3/src/skfolio/moments/
--rw-r--r--   0 root         (0) root         (0)      746 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/moments/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 08:19:59.898672 skfolio-0.1.3/src/skfolio/moments/covariance/
--rw-r--r--   0 root         (0) root         (0)      563 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/moments/covariance/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3955 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/moments/covariance/_base.py
--rw-r--r--   0 root         (0) root         (0)    39003 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/moments/covariance/_covariance.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 08:19:59.898672 skfolio-0.1.3/src/skfolio/moments/expected_returns/
--rw-r--r--   0 root         (0) root         (0)      367 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/moments/expected_returns/__init__.py
--rw-r--r--   0 root         (0) root         (0)      871 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/moments/expected_returns/_base.py
--rw-r--r--   0 root         (0) root         (0)    13388 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/moments/expected_returns/_expected_returns.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 08:19:59.902672 skfolio-0.1.3/src/skfolio/optimization/
--rw-r--r--   0 root         (0) root         (0)     1021 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/optimization/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5668 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/optimization/_base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 08:19:59.902672 skfolio-0.1.3/src/skfolio/optimization/cluster/
--rw-r--r--   0 root         (0) root         (0)      388 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/optimization/cluster/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14834 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/optimization/cluster/_nco.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 08:19:59.902672 skfolio-0.1.3/src/skfolio/optimization/cluster/hierarchical/
--rw-r--r--   0 root         (0) root         (0)      405 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/optimization/cluster/hierarchical/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17255 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/optimization/cluster/hierarchical/_base.py
--rw-r--r--   0 root         (0) root         (0)    17235 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/optimization/cluster/hierarchical/_herc.py
--rw-r--r--   0 root         (0) root         (0)    16120 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/optimization/cluster/hierarchical/_hrp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 08:19:59.902672 skfolio-0.1.3/src/skfolio/optimization/convex/
--rw-r--r--   0 root         (0) root         (0)      570 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/optimization/convex/__init__.py
--rw-r--r--   0 root         (0) root         (0)    75413 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/optimization/convex/_base.py
--rw-r--r--   0 root         (0) root         (0)    17308 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/optimization/convex/_distributionally_robust.py
--rw-r--r--   0 root         (0) root         (0)    19137 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/optimization/convex/_maximum_diversification.py
--rw-r--r--   0 root         (0) root         (0)    43130 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/optimization/convex/_mean_risk.py
--rw-r--r--   0 root         (0) root         (0)    23618 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/optimization/convex/_risk_budgeting.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 08:19:59.902672 skfolio-0.1.3/src/skfolio/optimization/ensemble/
--rw-r--r--   0 root         (0) root         (0)      158 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/optimization/ensemble/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3399 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/optimization/ensemble/_base.py
--rw-r--r--   0 root         (0) root         (0)    13148 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/optimization/ensemble/_stacking.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 08:19:59.906672 skfolio-0.1.3/src/skfolio/optimization/naive/
--rw-r--r--   0 root         (0) root         (0)      147 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/optimization/naive/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5561 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/optimization/naive/_naive.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 08:19:59.906672 skfolio-0.1.3/src/skfolio/population/
--rw-r--r--   0 root         (0) root         (0)       80 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/population/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29411 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/population/_population.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 08:19:59.906672 skfolio-0.1.3/src/skfolio/portfolio/
--rw-r--r--   0 root         (0) root         (0)      586 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/portfolio/__init__.py
--rw-r--r--   0 root         (0) root         (0)    38313 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/portfolio/_base.py
--rw-r--r--   0 root         (0) root         (0)    22759 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/portfolio/_multi_period_portfolio.py
--rw-r--r--   0 root         (0) root         (0)    31649 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/portfolio/_portfolio.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 08:19:59.906672 skfolio-0.1.3/src/skfolio/pre_selection/
--rw-r--r--   0 root         (0) root         (0)      189 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/pre_selection/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12163 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/pre_selection/_pre_selection.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 08:19:59.906672 skfolio-0.1.3/src/skfolio/preprocessing/
--rw-r--r--   0 root         (0) root         (0)       94 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/preprocessing/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3826 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/preprocessing/_returns.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 08:19:59.906672 skfolio-0.1.3/src/skfolio/prior/
--rw-r--r--   0 root         (0) root         (0)      446 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/prior/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1927 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/prior/_base.py
--rw-r--r--   0 root         (0) root         (0)     9397 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/prior/_black_litterman.py
--rw-r--r--   0 root         (0) root         (0)     5740 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/prior/_empirical.py
--rw-r--r--   0 root         (0) root         (0)     9642 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/prior/_factor_model.py
--rw-r--r--   0 root         (0) root         (0)     1378 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/typing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 08:19:59.910672 skfolio-0.1.3/src/skfolio/uncertainty_set/
--rw-r--r--   0 root         (0) root         (0)      617 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/uncertainty_set/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3301 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/uncertainty_set/_base.py
--rw-r--r--   0 root         (0) root         (0)    10301 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/uncertainty_set/_bootstrap.py
--rw-r--r--   0 root         (0) root         (0)     8429 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/uncertainty_set/_empirical.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 08:19:59.910672 skfolio-0.1.3/src/skfolio/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3550 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/utils/bootstrap.py
--rw-r--r--   0 root         (0) root         (0)    11047 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/utils/equations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 08:19:59.910672 skfolio-0.1.3/src/skfolio/utils/fixes/
--rw-r--r--   0 root         (0) root         (0)       95 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/utils/fixes/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13551 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/utils/fixes/_dendrogram.py
--rw-r--r--   0 root         (0) root         (0)     3504 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/utils/sorting.py
--rw-r--r--   0 root         (0) root         (0)    13132 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/utils/stats.py
--rw-r--r--   0 root         (0) root         (0)    15351 2024-03-13 08:19:55.000000 skfolio-0.1.3/src/skfolio/utils/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 08:19:59.910672 skfolio-0.1.3/src/skfolio.egg-info/
--rw-r--r--   0 root         (0) root         (0)    19590 2024-03-13 08:19:59.000000 skfolio-0.1.3/src/skfolio.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3203 2024-03-13 08:19:59.000000 skfolio-0.1.3/src/skfolio.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-13 08:19:59.000000 skfolio-0.1.3/src/skfolio.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      337 2024-03-13 08:19:59.000000 skfolio-0.1.3/src/skfolio.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-03-13 08:19:59.000000 skfolio-0.1.3/src/skfolio.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:47:56.238159 skfolio-0.2.0/
+-rw-r--r--   0 root         (0) root         (0)     1526 2024-05-19 21:47:51.000000 skfolio-0.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       48 2024-05-19 21:47:51.000000 skfolio-0.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    19630 2024-05-19 21:47:56.238159 skfolio-0.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    15392 2024-05-19 21:47:51.000000 skfolio-0.2.0/README.rst
+-rw-r--r--   0 root         (0) root         (0)     3470 2024-05-19 21:47:52.000000 skfolio-0.2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-19 21:47:56.238159 skfolio-0.2.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:47:56.214159 skfolio-0.2.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:47:56.218159 skfolio-0.2.0/src/skfolio/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:47:56.218159 skfolio-0.2.0/src/skfolio/cluster/
+-rw-r--r--   0 root         (0) root         (0)      251 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/cluster/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12817 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/cluster/_hierarchical.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:47:56.222159 skfolio-0.2.0/src/skfolio/datasets/
+-rw-r--r--   0 root         (0) root         (0)      407 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/datasets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13952 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/datasets/_base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:47:56.222159 skfolio-0.2.0/src/skfolio/datasets/data/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/datasets/data/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    36146 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/datasets/data/factors_dataset.csv.gz
+-rw-r--r--   0 root         (0) root         (0)   426065 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/datasets/data/sp500_dataset.csv.gz
+-rw-r--r--   0 root         (0) root         (0)    41898 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/datasets/data/sp500_index.csv.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:47:56.222159 skfolio-0.2.0/src/skfolio/distance/
+-rw-r--r--   0 root         (0) root         (0)      547 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/distance/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1326 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/distance/_base.py
+-rw-r--r--   0 root         (0) root         (0)    18538 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/distance/_distance.py
+-rw-r--r--   0 root         (0) root         (0)      662 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:47:56.222159 skfolio-0.2.0/src/skfolio/measures/
+-rw-r--r--   0 root         (0) root         (0)     1631 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/measures/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8934 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/measures/_enums.py
+-rw-r--r--   0 root         (0) root         (0)    16829 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/measures/_measures.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:47:56.222159 skfolio-0.2.0/src/skfolio/metrics/
+-rw-r--r--   0 root         (0) root         (0)       75 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/metrics/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4306 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/metrics/_scorer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:47:56.226159 skfolio-0.2.0/src/skfolio/model_selection/
+-rw-r--r--   0 root         (0) root         (0)      507 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/model_selection/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19045 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/model_selection/_combinatorial.py
+-rw-r--r--   0 root         (0) root         (0)     7686 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/model_selection/_validation.py
+-rw-r--r--   0 root         (0) root         (0)     7539 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/model_selection/_walk_forward.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:47:56.226159 skfolio-0.2.0/src/skfolio/moments/
+-rw-r--r--   0 root         (0) root         (0)      746 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/moments/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:47:56.226159 skfolio-0.2.0/src/skfolio/moments/covariance/
+-rw-r--r--   0 root         (0) root         (0)      563 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/moments/covariance/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3955 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/moments/covariance/_base.py
+-rw-r--r--   0 root         (0) root         (0)    39003 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/moments/covariance/_covariance.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:47:56.226159 skfolio-0.2.0/src/skfolio/moments/expected_returns/
+-rw-r--r--   0 root         (0) root         (0)      367 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/moments/expected_returns/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      871 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/moments/expected_returns/_base.py
+-rw-r--r--   0 root         (0) root         (0)    13388 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/moments/expected_returns/_expected_returns.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:47:56.226159 skfolio-0.2.0/src/skfolio/optimization/
+-rw-r--r--   0 root         (0) root         (0)     1021 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/optimization/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5748 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/optimization/_base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:47:56.226159 skfolio-0.2.0/src/skfolio/optimization/cluster/
+-rw-r--r--   0 root         (0) root         (0)      388 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/optimization/cluster/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14834 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/optimization/cluster/_nco.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:47:56.226159 skfolio-0.2.0/src/skfolio/optimization/cluster/hierarchical/
+-rw-r--r--   0 root         (0) root         (0)      405 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/optimization/cluster/hierarchical/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17281 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/optimization/cluster/hierarchical/_base.py
+-rw-r--r--   0 root         (0) root         (0)    17238 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/optimization/cluster/hierarchical/_herc.py
+-rw-r--r--   0 root         (0) root         (0)    16123 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/optimization/cluster/hierarchical/_hrp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:47:56.230159 skfolio-0.2.0/src/skfolio/optimization/convex/
+-rw-r--r--   0 root         (0) root         (0)      570 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/optimization/convex/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    75439 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/optimization/convex/_base.py
+-rw-r--r--   0 root         (0) root         (0)    17311 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/optimization/convex/_distributionally_robust.py
+-rw-r--r--   0 root         (0) root         (0)    19140 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/optimization/convex/_maximum_diversification.py
+-rw-r--r--   0 root         (0) root         (0)    43134 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/optimization/convex/_mean_risk.py
+-rw-r--r--   0 root         (0) root         (0)    23622 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/optimization/convex/_risk_budgeting.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:47:56.230159 skfolio-0.2.0/src/skfolio/optimization/ensemble/
+-rw-r--r--   0 root         (0) root         (0)      158 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/optimization/ensemble/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3399 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/optimization/ensemble/_base.py
+-rw-r--r--   0 root         (0) root         (0)    13148 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/optimization/ensemble/_stacking.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:47:56.230159 skfolio-0.2.0/src/skfolio/optimization/naive/
+-rw-r--r--   0 root         (0) root         (0)      147 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/optimization/naive/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5570 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/optimization/naive/_naive.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:47:56.230159 skfolio-0.2.0/src/skfolio/population/
+-rw-r--r--   0 root         (0) root         (0)       80 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/population/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29148 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/population/_population.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:47:56.230159 skfolio-0.2.0/src/skfolio/portfolio/
+-rw-r--r--   0 root         (0) root         (0)      586 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/portfolio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    38313 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/portfolio/_base.py
+-rw-r--r--   0 root         (0) root         (0)    22759 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/portfolio/_multi_period_portfolio.py
+-rw-r--r--   0 root         (0) root         (0)    31649 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/portfolio/_portfolio.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:47:56.234159 skfolio-0.2.0/src/skfolio/pre_selection/
+-rw-r--r--   0 root         (0) root         (0)      189 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/pre_selection/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12163 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/pre_selection/_pre_selection.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:47:56.234159 skfolio-0.2.0/src/skfolio/preprocessing/
+-rw-r--r--   0 root         (0) root         (0)       94 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/preprocessing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3826 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/preprocessing/_returns.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:47:56.234159 skfolio-0.2.0/src/skfolio/prior/
+-rw-r--r--   0 root         (0) root         (0)      446 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/prior/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1927 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/prior/_base.py
+-rw-r--r--   0 root         (0) root         (0)     9397 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/prior/_black_litterman.py
+-rw-r--r--   0 root         (0) root         (0)     5740 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/prior/_empirical.py
+-rw-r--r--   0 root         (0) root         (0)     9665 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/prior/_factor_model.py
+-rw-r--r--   0 root         (0) root         (0)     1378 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/typing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:47:56.234159 skfolio-0.2.0/src/skfolio/uncertainty_set/
+-rw-r--r--   0 root         (0) root         (0)      617 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/uncertainty_set/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3301 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/uncertainty_set/_base.py
+-rw-r--r--   0 root         (0) root         (0)    10301 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/uncertainty_set/_bootstrap.py
+-rw-r--r--   0 root         (0) root         (0)     8429 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/uncertainty_set/_empirical.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:47:56.238159 skfolio-0.2.0/src/skfolio/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3550 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/utils/bootstrap.py
+-rw-r--r--   0 root         (0) root         (0)    11047 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/utils/equations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:47:56.238159 skfolio-0.2.0/src/skfolio/utils/fixes/
+-rw-r--r--   0 root         (0) root         (0)       95 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/utils/fixes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13551 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/utils/fixes/_dendrogram.py
+-rw-r--r--   0 root         (0) root         (0)     3504 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/utils/sorting.py
+-rw-r--r--   0 root         (0) root         (0)    13132 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/utils/stats.py
+-rw-r--r--   0 root         (0) root         (0)    15374 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/utils/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:47:56.238159 skfolio-0.2.0/src/skfolio.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    19630 2024-05-19 21:47:56.000000 skfolio-0.2.0/src/skfolio.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3203 2024-05-19 21:47:56.000000 skfolio-0.2.0/src/skfolio.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-19 21:47:56.000000 skfolio-0.2.0/src/skfolio.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      337 2024-05-19 21:47:56.000000 skfolio-0.2.0/src/skfolio.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-19 21:47:56.000000 skfolio-0.2.0/src/skfolio.egg-info/top_level.txt
```

### Comparing `skfolio-0.1.3/LICENSE` & `skfolio-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `skfolio-0.1.3/PKG-INFO` & `skfolio-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skfolio
-Version: 0.1.3
+Version: 0.2.0
 Summary: Portfolio optimization built on top of scikit-learn
 Author-email: Hugo Delatte <delatte.hugo@gmail.com>
 Maintainer-email: Hugo Delatte <delatte.hugo@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2007-2023 The skfolio developers.
         All rights reserved.
@@ -81,45 +81,45 @@
 Requires-Dist: sphinx-prompt; extra == "docs"
 Requires-Dist: sphinxext.opengraph; extra == "docs"
 Requires-Dist: sphinx-sitemap; extra == "docs"
 Requires-Dist: sphinx-favicon; extra == "docs"
 
 .. -*- mode: rst -*-
 
-|Licence|_ |Codecov|_ |Black|_ |PythonVersion|_ |PyPi|_ |CI/CD|_ |Downloads|_ |Ruff|_ |Contribution|_ |Website|_
+|Licence| |Codecov| |Black| |PythonVersion| |PyPi| |CI/CD| |Downloads| |Ruff| |Contribution| |Website|
 
 .. |Licence| image:: https://img.shields.io/badge/License-BSD%203--Clause-blue.svg
-.. _Licence: https://github.com/skfolio/skfolio/blob/main/LICENSE
+   :target: https://github.com/skfolio/skfolio/blob/main/LICENSE
 
 .. |Codecov| image:: https://codecov.io/gh/skfolio/skfolio/graph/badge.svg?token=KJ0SE4LHPV
-.. _Codecov: https://codecov.io/gh/skfolio/skfolio
+   :target: https://codecov.io/gh/skfolio/skfolio
 
-.. |PythonVersion| image:: https://img.shields.io/badge/python-3.10%20%7C%203.11%20%7C%203.12-blue
-.. _PythonVersion: https://pypi.org/project/skfolio/
+.. |PythonVersion| image:: https://img.shields.io/badge/python-3.10%20%7C%203.11%20%7C%203.12-blue.svg
+   :target: https://pypi.org/project/skfolio/
 
 .. |PyPi| image:: https://img.shields.io/pypi/v/skfolio
-.. _PyPi: https://pypi.org/project/skfolio
+   :target: https://pypi.org/project/skfolio
 
 .. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
-.. _Black: https://github.com/psf/black
+   :target: https://github.com/psf/black
 
-.. |CI/CD| image:: https://img.shields.io/github/actions/workflow/status/skfolio/skfolio/release.yml?logo=github
-.. _CI/CD: https://github.com/skfolio/skfolio/raw/main/LICENSE
+.. |CI/CD| image:: https://img.shields.io/github/actions/workflow/status/skfolio/skfolio/release.yml.svg?logo=github
+   :target: https://github.com/skfolio/skfolio/raw/main/LICENSE
 
 .. |Downloads| image:: https://static.pepy.tech/badge/skfolio
-.. _Downloads: https://pepy.tech/project/skfolio
+   :target: https://pepy.tech/project/skfolio
 
 .. |Ruff| image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json
-.. _Ruff: https://github.com/astral-sh/ruff
+   :target: https://github.com/astral-sh/ruff
 
 .. |Contribution| image:: https://img.shields.io/badge/Contributions-Welcome-blue
-.. _Contribution: https://github.com/skfolio/skfolio/blob/main/CONTRIBUTING.md
+   :target: https://github.com/skfolio/skfolio/blob/main/CONTRIBUTING.md
 
-.. |Website| image:: https://img.shields.io/website-up-down-53cc0d-red/http/skfolio.org
-.. _Website: https://skfolio.org
+.. |Website| image:: https://img.shields.io/website.svg?down_color=red&down_message=down&up_color=53cc0d&up_message=up&url=https://skfolio.org
+   :target: https://skfolio.org
 
 .. |PythonMinVersion| replace:: 3.10
 .. |NumpyMinVersion| replace:: 1.23.4
 .. |ScipyMinVersion| replace:: 1.8.0
 .. |PandasMinVersion| replace:: 1.4.1
 .. |CvxpyMinVersion| replace:: 1.4.1
 .. |SklearnMinVersion| replace:: 1.3.2
```

### Comparing `skfolio-0.1.3/README.rst` & `skfolio-0.2.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 .. -*- mode: rst -*-
 
-|Licence|_ |Codecov|_ |Black|_ |PythonVersion|_ |PyPi|_ |CI/CD|_ |Downloads|_ |Ruff|_ |Contribution|_ |Website|_
+|Licence| |Codecov| |Black| |PythonVersion| |PyPi| |CI/CD| |Downloads| |Ruff| |Contribution| |Website|
 
 .. |Licence| image:: https://img.shields.io/badge/License-BSD%203--Clause-blue.svg
-.. _Licence: https://github.com/skfolio/skfolio/blob/main/LICENSE
+   :target: https://github.com/skfolio/skfolio/blob/main/LICENSE
 
 .. |Codecov| image:: https://codecov.io/gh/skfolio/skfolio/graph/badge.svg?token=KJ0SE4LHPV
-.. _Codecov: https://codecov.io/gh/skfolio/skfolio
+   :target: https://codecov.io/gh/skfolio/skfolio
 
-.. |PythonVersion| image:: https://img.shields.io/badge/python-3.10%20%7C%203.11%20%7C%203.12-blue
-.. _PythonVersion: https://pypi.org/project/skfolio/
+.. |PythonVersion| image:: https://img.shields.io/badge/python-3.10%20%7C%203.11%20%7C%203.12-blue.svg
+   :target: https://pypi.org/project/skfolio/
 
 .. |PyPi| image:: https://img.shields.io/pypi/v/skfolio
-.. _PyPi: https://pypi.org/project/skfolio
+   :target: https://pypi.org/project/skfolio
 
 .. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
-.. _Black: https://github.com/psf/black
+   :target: https://github.com/psf/black
 
-.. |CI/CD| image:: https://img.shields.io/github/actions/workflow/status/skfolio/skfolio/release.yml?logo=github
-.. _CI/CD: https://github.com/skfolio/skfolio/raw/main/LICENSE
+.. |CI/CD| image:: https://img.shields.io/github/actions/workflow/status/skfolio/skfolio/release.yml.svg?logo=github
+   :target: https://github.com/skfolio/skfolio/raw/main/LICENSE
 
 .. |Downloads| image:: https://static.pepy.tech/badge/skfolio
-.. _Downloads: https://pepy.tech/project/skfolio
+   :target: https://pepy.tech/project/skfolio
 
 .. |Ruff| image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json
-.. _Ruff: https://github.com/astral-sh/ruff
+   :target: https://github.com/astral-sh/ruff
 
 .. |Contribution| image:: https://img.shields.io/badge/Contributions-Welcome-blue
-.. _Contribution: https://github.com/skfolio/skfolio/blob/main/CONTRIBUTING.md
+   :target: https://github.com/skfolio/skfolio/blob/main/CONTRIBUTING.md
 
-.. |Website| image:: https://img.shields.io/website-up-down-53cc0d-red/http/skfolio.org
-.. _Website: https://skfolio.org
+.. |Website| image:: https://img.shields.io/website.svg?down_color=red&down_message=down&up_color=53cc0d&up_message=up&url=https://skfolio.org
+   :target: https://skfolio.org
 
 .. |PythonMinVersion| replace:: 3.10
 .. |NumpyMinVersion| replace:: 1.23.4
 .. |ScipyMinVersion| replace:: 1.8.0
 .. |PandasMinVersion| replace:: 1.4.1
 .. |CvxpyMinVersion| replace:: 1.4.1
 .. |SklearnMinVersion| replace:: 1.3.2
```

### Comparing `skfolio-0.1.3/pyproject.toml` & `skfolio-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "skfolio"
-version = "0.1.3"
+version = "0.2.0"
 maintainers = [
     { name = "Hugo Delatte", email = "delatte.hugo@gmail.com" },
 ]
 authors = [
     { name = "Hugo Delatte", email = "delatte.hugo@gmail.com" },
 ]
 description = "Portfolio optimization built on top of scikit-learn"
```

### Comparing `skfolio-0.1.3/src/skfolio/__init__.py` & `skfolio-0.2.0/src/skfolio/__init__.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.1.3/src/skfolio/cluster/_hierarchical.py` & `skfolio-0.2.0/src/skfolio/cluster/_hierarchical.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.1.3/src/skfolio/datasets/_base.py` & `skfolio-0.2.0/src/skfolio/datasets/_base.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.1.3/src/skfolio/datasets/data/factors_dataset.csv.gz` & `skfolio-0.2.0/src/skfolio/datasets/data/factors_dataset.csv.gz`

 * *Files identical despite different names*

### Comparing `skfolio-0.1.3/src/skfolio/datasets/data/sp500_dataset.csv.gz` & `skfolio-0.2.0/src/skfolio/datasets/data/sp500_dataset.csv.gz`

 * *Files identical despite different names*

### Comparing `skfolio-0.1.3/src/skfolio/datasets/data/sp500_index.csv.gz` & `skfolio-0.2.0/src/skfolio/datasets/data/sp500_index.csv.gz`

 * *Files identical despite different names*

### Comparing `skfolio-0.1.3/src/skfolio/distance/__init__.py` & `skfolio-0.2.0/src/skfolio/distance/__init__.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.1.3/src/skfolio/distance/_base.py` & `skfolio-0.2.0/src/skfolio/distance/_base.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.1.3/src/skfolio/distance/_distance.py` & `skfolio-0.2.0/src/skfolio/distance/_distance.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.1.3/src/skfolio/exceptions.py` & `skfolio-0.2.0/src/skfolio/exceptions.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.1.3/src/skfolio/measures/__init__.py` & `skfolio-0.2.0/src/skfolio/measures/__init__.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.1.3/src/skfolio/measures/_enums.py` & `skfolio-0.2.0/src/skfolio/measures/_enums.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.1.3/src/skfolio/measures/_measures.py` & `skfolio-0.2.0/src/skfolio/measures/_measures.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.1.3/src/skfolio/metrics/_scorer.py` & `skfolio-0.2.0/src/skfolio/metrics/_scorer.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.1.3/src/skfolio/model_selection/_combinatorial.py` & `skfolio-0.2.0/src/skfolio/utils/tools.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,412 +1,572 @@
-"""Combinatorial module"""
+"""Tools module"""
 
 # Copyright (c) 2023
 # Author: Hugo Delatte <delatte.hugo@gmail.com>
 # License: BSD 3 clause
 # Implementation derived from:
-# scikit-portfolio, Copyright (c) 2022, Carlo Nicolini, Licensed under MIT Licence.
 # scikit-learn, Copyright (c) 2007-2010 David Cournapeau, Fabian Pedregosa, Olivier
 # Grisel Licensed under BSD 3 clause.
 
-import itertools
-import math
-import numbers
-from abc import ABC, abstractmethod
-from collections.abc import Iterator
+from collections.abc import Callable, Iterator
+from enum import Enum
+from functools import wraps
+from typing import Any
 
 import numpy as np
 import numpy.typing as npt
 import pandas as pd
-import plotly.graph_objects as go
-import sklearn.model_selection as skm
-import sklearn.utils as sku
-
-import skfolio.typing as skt
-
-
-class BaseCombinatorialCV(ABC):
-    """Base class for all combinatorial cross-validators.
-
-    Implementations must define `split` or `get_path_ids`.
-    """
-
-    @abstractmethod
-    def split(self, X: npt.ArrayLike, y=None) -> tuple[np.ndarray, list[np.ndarray]]:
-        pass
-
-    @abstractmethod
-    def get_path_ids(self) -> np.ndarray:
-        """Return the path id of each test sets in each split"""
-        pass
-
-    __repr__ = skm.BaseCrossValidator.__repr__
-
-
-# TODO: review params and function naming
-class CombinatorialPurgedCV(BaseCombinatorialCV):
-    """Combinatorial Purged Cross-Validation.
-
-    Provides train/test indices to split time series data samples based on
-    Combinatorial Purged Cross-Validation [1]_.
-
-    Compared to `KFold`, which splits the data into `k` folds with `1` fold for the test
-    set and `k - 1` folds for the training set, `CombinatorialPurgedCV` uses `k - p`
-    folds for the training set with `p > 1` being the number of test folds.
-
-    `KFold` can recombine one single testing path while `CombinatorialPurgedCV` can
-    recombine multiple testing paths from the combinations of the train/test sets.
-
-    To avoid data leakage, purging and embargoing can be performed.
-
-    Purging consist of removing from the training set all observations whose labels
-    overlapped in time with those labels included in the testing set.
-
-    Embargoing consist of removing from the training set all observations that
-    immediately follow an observation in the testing set, since financial features
-    often incorporate series that exhibit serial correlation (like ARMA processes).
-
-    Parameters
-    ----------
-    n_folds : int, default=10
-        Number of folds. Must be at least 3.
-
-    n_test_folds : int, default=8
-        Number of test folds. Must be at least 2.
-        For only one test fold, use `sklearn.model_validation.KFold`.
-
-    purged_size : int, default=0
-        Number of observations to exclude from the start of each train set that are
-        after a test set **and** the number of observations to exclude from the end of
-        each training set that are before a test set.
-
-    embargo_size : int, default=0
-        Number of observations to exclude from the start of each training set that are
-        after a test set.
-
-    Attributes
-    ----------
-    index_train_test_ : ndarray of shape (n_observations, n_splits)
-
-    Examples
-    --------
-    >>> import numpy as np
-    >>> from skfolio.model_selection import CombinatorialPurgedCV
-    >>> X = np.random.randn(12, 2)
-    >>> cv = CombinatorialPurgedCV(n_folds=3, n_test_folds=2)
-    >>> for i, (train_index, tests) in enumerate(cv.split(X)):
-    ...     print(f"Split {i}:")
-    ...     print(f"  Train: index={train_index}")
-    ...     for j, test_index in enumerate(tests):
-    ...         print(f"  Test {j}:  index={test_index}")
-    Split 0:
-      Train: index=[ 8  9 10 11]
-      Test 0:  index=[0 1 2 3]
-      Test 1:  index=[4 5 6 7]
-    Split 1:
-      Train: index=[4 5 6 7]
-      Test 0:  index=[0 1 2 3]
-      Test 1:  index=[ 8  9 10 11]
-    Split 2:
-      Train: index=[0 1 2 3]
-      Test 0:  index=[4 5 6 7]
-      Test 1:  index=[ 8  9 10 11]
-    >>> cv = CombinatorialPurgedCV(n_folds=3, n_test_folds=2, purged_size=1)
-    >>> for i, (train_index, tests) in enumerate(cv.split(X)):
-    ...     print(f"Split {i}:")
-    ...     print(f"  Train: index={train_index}")
-    ...     for j, test_index in enumerate(tests):
-    ...         print(f"  Test {j}:  index={test_index}")
-    Split 0:
-      Train: index=[ 9 10 11]
-      Test 0:  index=[0 1 2 3]
-      Test 1:  index=[4 5 6 7]
-    Split 1:
-      Train: index=[5 6]
-      Test 0:  index=[0 1 2 3]
-      Test 1:  index=[ 8  9 10 11]
-    Split 2:
-      Train: index=[0 1 2]
-      Test 0:  index=[4 5 6 7]
-      Test 1:  index=[ 8  9 10 11]
-    >>> cv = CombinatorialPurgedCV(n_folds=3, n_test_folds=2, embargo_size=1)
-    >>> for i, (train_index, tests) in enumerate(cv.split(X)):
-    ...     print(f"Split {i}:")
-    ...     print(f"  Train: index={train_index}")
-    ...     for j, test_index in enumerate(tests):
-    ...         print(f"  Test {j}:  index={test_index}")
-    Split 0:
-      Train: index=[ 9 10 11]
-      Test 0:  index=[0 1 2 3]
-      Test 1:  index=[4 5 6 7]
-    Split 1:
-      Train: index=[5 6 7]
-      Test 0:  index=[0 1 2 3]
-      Test 1:  index=[ 8  9 10 11]
-    Split 2:
-      Train: index=[0 1 2 3]
-      Test 0:  index=[4 5 6 7]
-      Test 1:  index=[ 8  9 10 11]
-
-    References
-    ----------
-    .. [1]  "Advances in Financial Machine Learning",
-        Marcos López de Prado (2018)
-    """
-
-    index_train_test_: np.ndarray
-
-    def __init__(
-        self,
-        n_folds: int = 10,
-        n_test_folds: int = 8,
-        purged_size: int = 0,
-        embargo_size: int = 0,
-    ):
-        if not isinstance(n_folds, numbers.Integral):
-            raise ValueError(
-                "The number of folds must be of Integral type. "
-                f"{n_folds} of type {type(n_folds)} was passed."
-            )
-        n_folds = int(n_folds)
+import sklearn as sk
+import sklearn.base as skb
 
-        if n_folds <= 2:
-            raise ValueError(f"`n_folds` must be at least 3`, got `n_folds={n_folds}`.")
+__all__ = [
+    "AutoEnum",
+    "cached_property_slots",
+    "cache_method",
+    "input_to_array",
+    "args_names",
+    "format_measure",
+    "bisection",
+    "safe_split",
+    "fit_single_estimator",
+    "fit_and_predict",
+    "deduplicate_names",
+    "default_asset_names",
+    "check_estimator",
+]
+
+GenericAlias = type(list[int])
+
+
+class AutoEnum(str, Enum):
+    """Base Enum class used in `skfolio`"""
+
+    @staticmethod
+    def _generate_next_value_(
+        name: str, start: int, count: int, last_values: Any
+    ) -> str:
+        """Overriding `auto()`"""
+        return name.lower()
+
+    @classmethod
+    def has(cls, value: str) -> bool:
+        """Check if a value is in the Enum.
 
-        if n_test_folds <= 1:
-            raise ValueError(
-                f"`n_test_folds` must at least 2, got `n_test_folds={n_test_folds}`."
-            )
+        Parameters
+        ----------
+        value : str
+            Input value.
 
-        if n_test_folds >= n_folds:
-            raise ValueError(
-                "Combinatorial purged cross-validation requires `n_folds` "
-                "to be greater than `n_test_folds`."
+        Returns
+        -------
+        x : bool
+            True if the value is in the Enum, False otherwise.
+        """
+        return value in cls._value2member_map_
+
+    def __repr__(self) -> str:
+        """Representation of the Enum"""
+        return self.name
+
+
+# noinspection PyPep8Naming
+class cached_property_slots:
+    """Cached property decorator for slots"""
+
+    def __init__(self, func):
+        self.func = func
+        self.public_name = None
+        self.private_name = None
+        self.__doc__ = func.__doc__
+
+    def __set_name__(self, owner, name):
+        self.public_name = name
+        self.private_name = f"_{name}"
+
+    def __get__(self, instance, owner=None):
+        if instance is None:
+            return self
+        if self.private_name is None:
+            raise TypeError(
+                "Cannot use cached_property instance without calling __set_name__"
+                " on it."
             )
+        try:
+            value = getattr(instance, self.private_name)
+        except AttributeError:
+            value = self.func(instance)
+            setattr(instance, self.private_name, value)
+        return value
+
+    def __set__(self, instance, owner=None):
+        raise AttributeError(
+            f"'{type(instance).__name__}' object attribute '{self.public_name}' is"
+            " read-only"
+        )
 
-        if purged_size < 0:
-            raise ValueError("`purged_size` cannot be negative")
+    __class_getitem__ = classmethod(GenericAlias)
 
-        if embargo_size < 0:
-            raise ValueError("`embargo_size` cannot be negative")
 
-        self.n_folds = n_folds
-        self.n_test_folds = n_test_folds
-        self.purged_size = purged_size
-        self.embargo_size = embargo_size
-
-    @property
-    def n_splits(self) -> int:
-        """Number of splits"""
-        return int(
-            math.factorial(self.n_folds)
-            / (
-                math.factorial(self.n_test_folds)
-                * math.factorial(self.n_folds - self.n_test_folds)
-            )
-        )
+def _make_key(args, kwds) -> int:
+    """Make a cache key from optionally typed positional and keyword arguments"""
+    key = args
+    if kwds:
+        for item in kwds.items():
+            key += item
+    return hash(key)
 
-    @property
-    def n_test_paths(self) -> int:
-        """Number of test paths that can be reconstructed from the train/test
-        combinations"""
-        return self.n_splits * self.n_test_folds // self.n_folds
-
-    @property
-    def test_set_index(self) -> np.ndarray:
-        """Location of each test set"""
-        return np.array(
-            list(itertools.combinations(np.arange(self.n_folds), self.n_test_folds))
-        ).reshape(-1, self.n_test_folds)
-
-    @property
-    def binary_train_test_sets(self) -> np.ndarray:
-        """Identify training and test folds for each combinations by assigning `0` to
-        training folds and `1` to test folds"""
-        folds_train_test = np.zeros((self.n_folds, self.n_splits))
-        folds_train_test[
-            self.test_set_index, np.arange(self.n_splits)[:, np.newaxis]
-        ] = 1
-        return folds_train_test
-
-    @property
-    def recombined_paths(self) -> np.ndarray:
-        """Recombine each test path by returning the test set location in each split."""
-        return np.argwhere(self.binary_train_test_sets == 1)[:, 1].reshape(
-            self.n_folds, -1
-        )
 
-    def get_path_ids(self) -> np.ndarray:
-        """Return the path id of each test sets in each split"""
-        recombine_paths = self.recombined_paths
-        path_ids = np.zeros((self.n_splits, self.n_test_folds), dtype=int)
-        for i in range(self.n_splits):
-            for j in range(self.n_test_folds):
-                path_ids[i, j] = np.argwhere(recombine_paths == i)[j][1]
-        return path_ids
-
-    def split(
-        self, X: npt.ArrayLike, y=None, groups=None
-    ) -> Iterator[tuple[np.ndarray, list[np.ndarray]]]:
-        """Generate indices to split data into training and test set.
+def cache_method(cache_name: str) -> Callable:
+    """Decorator that caches class methods results into a class dictionary.
 
-        Parameters
-        ----------
-        X : array-like of shape (n_samples, n_features)
-            Training data, where `n_samples` is the number of samples
-            and `n_features` is the number of features.
-
-        y : array-like of shape (n_samples,), optional
-            The (multi-)target variable
-
-        groups : array-like of shape (n_samples,), optional
-            Group labels for the samples used while splitting the dataset into
-            train/test set.
-
-        Yields
-        ------
-        train : ndarray
-            The training set indices for that split.
+    Parameters
+    ----------
+    cache_name : str
+        Name of the dictionary class attribute.
 
-        test : ndarray
-            The testing set indices for that split.
-        """
-        test_set_index = self.test_set_index
-        recombine_paths = self.recombined_paths
+    Returns
+    -------
+    func : Callable
+        Decorating function that caches class methods.
+    """
+
+    # To avoid memory leakage and proper garbage collection, self should not be part of
+    # the cache key.
+    # This is a known issue when we use functools.lru_cache on class methods.
+    def decorating_function(method):
+        @wraps(method)
+        def wrapper(self, *args, **kwargs):
+            func_name = method.__name__
+            key = _make_key(args, kwargs)
+            try:
+                cache = getattr(self, cache_name)
+            except AttributeError:
+                raise AttributeError(
+                    "You first need to create a dictionary class attribute named "
+                    f"'{cache_name}'"
+                ) from None
+            if not isinstance(cache, dict):
+                raise AttributeError(
+                    f"'The cache named '{cache_name}' must be a "
+                    f"dictionary, got {type(cache)}"
+                )
+            if func_name not in cache:
+                cache[func_name] = {}
+            c = cache[func_name]
+            if key not in c:
+                c[key] = method(self, *args, **kwargs)
+            return c[key]
+
+        return wrapper
 
-        X, y = sku.indexable(X, y)
-        n_samples = X.shape[0]
-        min_fold_size = n_samples // self.n_folds
-        if self.purged_size + self.embargo_size >= min_fold_size - 1:
+    return decorating_function
+
+
+def args_names(func: object) -> list[str]:
+    """Returns the argument names of a function.
+
+    Parameters
+    ----------
+    func : object
+        Function.
+
+    Returns
+    -------
+    args : list[str]
+        The list of function arguments.
+    """
+    return [
+        v for v in func.__code__.co_varnames[: func.__code__.co_argcount] if v != "self"
+    ]
+
+
+def check_estimator(
+    estimator: skb.BaseEstimator | None, default: skb.BaseEstimator, check_type: Any
+):
+    """Check the estimator type and returns its cloned version it provided, otherwise
+     return the default estimator.
+
+    Parameters
+    ----------
+    estimator : BaseEstimator, optional
+        Estimator.
+
+    default : BaseEstimator
+        Default estimator to return when `estimator` is `None`.
+
+    check_type : Any
+        Expected type of the estimator to check against.
+
+    Returns
+    -------
+    estimator: Estimator
+        The checked estimator or the default.
+    """
+
+    if estimator is None:
+        return default
+    if not isinstance(estimator, check_type):
+        raise TypeError(f"Expected type {check_type}, got {type(estimator)}")
+    return sk.clone(estimator)
+
+
+def input_to_array(
+    items: dict | npt.ArrayLike,
+    n_assets: int,
+    fill_value: Any,
+    dim: int,
+    assets_names: np.ndarray | None,
+    name: str,
+) -> np.ndarray:
+    """Convert a collection of items (array-like or dictionary) into
+    a numpy array and verify its shape.
+
+    Parameters
+    ----------
+    items : np.ndarray | dict | list
+        Items to verify and convert to array.
+
+    n_assets : int
+        Expected number of assets.
+        Used to verify the shape of the converted array.
+
+    fill_value : Any
+        When `items` is a dictionary, elements that are not in `asset_names` are filled
+        with `fill_value` in the converted array.
+
+    dim : int
+        Dimension of the final array.
+        Possible values are `1` or `2`.
+
+    assets_names : ndarray, optional
+        Asset names used when `items` is a dictionary.
+
+    name : str
+        Name of the items used for error messages.
+
+    Returns
+    -------
+    values : ndarray of shape (n_assets) for dim=1 or (n_groups, n_assets) for dim=2
+        Converted array.
+    """
+    if dim not in [1, 2]:
+        raise ValueError(f"dim must be 1 or 2, got {dim}")
+    if isinstance(items, dict):
+        if assets_names is None:
             raise ValueError(
-                "The sum of `purged_size` and `embargo_size` must be smaller than the"
-                f" size of a train fold which is {min_fold_size}"
+                f"If `{name}` is provided as a dictionary, you must input `X` as a"
+                " DataFrame with assets names in columns"
+            )
+        if dim == 1:
+            arr = np.array([items.get(asset, fill_value) for asset in assets_names])
+        else:
+            # add assets and convert dict to ordered array
+            arr = {}
+            for asset in assets_names:
+                elem = items.get(asset)
+                if elem is None:
+                    elem = [asset]
+                elif np.isscalar(elem):
+                    elem = [asset, elem]
+                else:
+                    elem = [asset, *elem]
+                arr[asset] = elem
+            arr = (
+                pd.DataFrame.from_dict(arr, orient="index")
+                .loc[assets_names]
+                .to_numpy()
+                .T
             )
+    else:
+        arr = np.asarray(items)
 
-        fold_index_num = np.arange(n_samples) // (n_samples // self.n_folds)
-        fold_index_num[fold_index_num == self.n_folds] = self.n_folds - 1
+    if arr.ndim != dim:
+        raise ValueError(f"`{name}` must be a {dim}D array, got a {arr.ndim}D array")
 
-        index_train_test = np.zeros((n_samples, self.n_splits))
-        for i in range(self.n_splits):
-            index_train_test[
-                np.argwhere([fold_index_num == j for j in test_set_index[i]])[:, 1], i
-            ] = 1
-
-        diff = np.diff(index_train_test, axis=0)
-
-        # Purge before
-        before_index = np.argwhere(diff == 1)
-        for k in range(self.purged_size):
-            index_train_test[
-                np.maximum(0, before_index[:, 0] - k), before_index[:, 1]
-            ] = -1
-
-        # Purge after and Embargo
-        after_index = np.argwhere(diff == -1)
-        for k in range(self.purged_size + self.embargo_size):
-            index_train_test[
-                np.minimum(n_samples - 1, after_index[:, 0] + k + 1), after_index[:, 1]
-            ] = -1
-        self.index_train_test_ = index_train_test
-
-        fold_index = {
-            fold_id: np.argwhere(fold_index_num == fold_id).reshape(-1)
-            for fold_id in range(self.n_folds)
-        }
-        for i in range(self.n_splits):
-            train_index = np.argwhere(index_train_test[:, i] == 0).reshape(-1)
-            test_index_list = [
-                fold_index[fold_id] for fold_id, _ in np.argwhere(recombine_paths == i)
-            ]
-            yield train_index, test_index_list
-
-    def summary(self, X) -> pd.Series:
-        n_samples = X.shape[0]
-        return pd.Series(
-            {
-                "Number of Observations": n_samples,
-                "Total Number of Folds": self.n_folds,
-                "Number of Test Folds": self.n_test_folds,
-                "Purge Size": self.purged_size,
-                "Embargo Size": self.embargo_size,
-                "Average Training Size": int(
-                    n_samples / self.n_folds * (self.n_folds - self.n_test_folds)
-                ),
-                "Number of Test Paths": self.n_test_paths,
-                "Number of Training Combinations": self.n_splits,
-            }
-        )
+    if not isinstance(fill_value, str) and np.isnan(arr).any():
+        raise ValueError(f"`{name}` contains NaN")
 
-    def plot_train_test_folds(self) -> skt.Figure:
-        """Plot the train/test fold locations"""
-        values = self.binary_train_test_sets
-        fill_color = np.where(values == 0, "blue", "red")
-        fill_color = fill_color.astype(object)
-        fill_color = np.insert(
-            fill_color, 0, np.array(["darkblue" for _ in range(self.n_splits)]), axis=0
+    if arr.shape[-1] != n_assets:
+        if dim == 1:
+            s = "(n_assets,)"
+        else:
+            s = "(n_groups, n_assets)"
+        raise ValueError(
+            f"`{name}` must be a of shape {s} with n_assets={n_assets}, "
+            f"got {arr.shape[0]}"
         )
-        values = np.insert(values, 0, np.arange(self.n_splits), axis=0)
-        fig = go.Figure(
-            data=[
-                go.Table(
-                    header=dict(
-                        values=["Train Combinations"]
-                        + [f"Fold {i}" for i in range(self.n_folds)],
-                        fill_color="darkblue",
-                        font=dict(color="white"),
-                        align="left",
-                    ),
-                    cells=dict(
-                        values=values,
-                        font=dict(color="white"),
-                        fill_color=fill_color,
-                        line_color="grey",
-                        align="left",
-                    ),
-                )
-            ]
-        )
-        fig.update_layout(title="Split Train (0) /Test (1) Folds per Combination")
-        return fig
+    return arr
 
-    def plot_train_test_index(self, X) -> skt.Figure:
-        """Plot the training and test indices for each combinations by assigning `0` to
-        training, `1` to test and `-1` to both purge and embargo indices."""
-        next(self.split(X))
-        n_samples = X.shape[0]
-        cond = [
-            self.index_train_test_ == -1,
-            self.index_train_test_ == 0,
-            self.index_train_test_ == 1,
-        ]
-        values = self.index_train_test_.T
-        values = np.insert(values, 0, np.arange(n_samples), axis=0)
-        fill_color = np.select(cond, ["green", "blue", "red"]).T
-        fill_color = fill_color.astype(object)
-        fill_color = np.insert(
-            fill_color, 0, np.array(["darkblue" for _ in range(n_samples)]), axis=0
-        )
-        fig = go.Figure(
-            data=[
-                go.Table(
-                    header=dict(
-                        values=["observations"]
-                        + [f"Split {i}" for i in range(self.n_splits)],
-                        fill_color="darkblue",
-                        font=dict(color="white"),
-                        align="left",
-                    ),
-                    cells=dict(
-                        values=values,
-                        font=dict(color="white"),
-                        fill_color=fill_color,
-                        line_color="grey",
-                        align="left",
-                    ),
-                )
-            ]
-        )
-        fig.update_layout(
-            title="Train (0), Test (1) and Purge/Embargo (-1) observations per splits"
-        )
 
-        return fig
+def format_measure(x: float, percent: bool = False) -> str:
+    """Format a measure number into a user-friendly string.
+
+    Parameters
+    ----------
+    x : float
+        Number to format.
+
+    percent : bool, default=False
+        If this is set to True, the number is formatted in percentage.
+
+    Returns
+    -------
+    formatted : str
+        Formatted string.
+    """
+    if np.isnan(x):
+        return str(x)
+    if percent:
+        xn = x * 100
+        f = "%"
+    else:
+        xn = x
+        f = "f"
+    if xn == 0:
+        n = 0
+    else:
+        n = min(6, max(int(-np.log10(abs(xn))) + 2, 2))
+    return "{value:{fmt}}".format(value=x, fmt=f".{n}{f}")
+
+
+def bisection(x: list[np.ndarray]) -> Iterator[list[np.ndarray, np.ndarray]]:
+    """Generator to bisect a list of array.
+
+    Parameters
+    ----------
+    x : list[ndarray]
+        A list of array.
+
+    Yields
+    ------
+    arr :  Iterator[list[ndarray, ndarray]]
+        Bisected array.
+    """
+    for e in x:
+        n = len(e)
+        if n > 1:
+            mid = n // 2
+            yield [e[0:mid], e[mid:n]]
+
+
+def safe_indexing(
+    X: npt.ArrayLike | pd.DataFrame, indices: npt.ArrayLike | None, axis: int = 0
+):
+    """
+    Return rows, items or columns of X using indices.
+
+    Parameters
+    ----------
+    X : array-like
+        Data from which to sample rows.
+
+    indices : array-like, optional
+        Indices of rows or columns.
+        The default (`None`) is to select the entire data.
+
+    axis : int, default=0
+        The axis along which `X` will be sub-sampled. `axis=0` will select
+        rows while `axis=1` will select columns.
+
+    Returns
+    -------
+    subset :
+        Subset of X on axis 0.
+    """
+    if indices is None:
+        return X
+    if hasattr(X, "iloc"):
+        return X.take(indices, axis=axis)
+    if axis == 0:
+        return X[indices]
+    return X[:, indices]
+
+
+def safe_split(
+    X: npt.ArrayLike,
+    y: npt.ArrayLike | None = None,
+    indices: np.ndarray | None = None,
+    axis: int = 0,
+):
+    """Create subset of dataset.
+
+    Slice X, y according to indices for cross-validation.
+
+    Parameters
+    ----------
+    X : array-like
+        Data to be indexed.
+
+    y : array-like
+        Data to be indexed.
+
+    indices : ndarray of int, optional
+        Rows or columns to select from X and y.
+        The default (`None`) is to select the entire data.
+
+    axis : int, default=0
+        The axis along which `X` will be sub-sampled. `axis=0` will select
+        rows while `axis=1` will select columns.
+
+    Returns
+    -------
+    X_subset : array-like
+        Indexed data.
+
+    y_subset : array-like
+        Indexed targets.
+    """
+
+    X_subset = safe_indexing(X, indices=indices, axis=axis)
+    if y is not None:
+        y_subset = safe_indexing(y, indices=indices, axis=axis)
+    else:
+        y_subset = None
+    return X_subset, y_subset
+
+
+def fit_single_estimator(
+    estimator: Any,
+    X: npt.ArrayLike,
+    y: npt.ArrayLike | None = None,
+    indices: np.ndarray | None = None,
+    axis: int = 0,
+):
+    """function used to fit an estimator within a job.
+
+    Parameters
+    ----------
+    estimator : estimator object implementing 'fit' and 'predict'
+        The object to use to fit the data.
+
+    X : array-like of shape (n_observations, n_assets)
+        The data to fit.
+
+    y : array-like of shape (n_observations, n_targets), optional
+        The target array if provided.
+
+    indices : ndarray of int, optional
+        Rows or columns to select from X and y.
+        The default (`None`) is to select the entire data.
+
+    axis : int, default=0
+        The axis along which `X` will be sub-sampled. `axis=0` will select
+        rows while `axis=1` will select columns.
+
+    Returns
+    -------
+    fitted_estimator : estimator
+        The fitted estimator.
+    """
+
+    X, y = safe_split(X, y, indices=indices, axis=axis)
+    estimator.fit(X, y)
+    return estimator
+
+
+def fit_and_predict(
+    estimator: Any,
+    X: npt.ArrayLike,
+    y: npt.ArrayLike | None,
+    train: np.ndarray,
+    test: np.ndarray | list[np.ndarray],
+    fit_params: dict,
+    method: str,
+    column_indices: np.ndarray | None = None,
+) -> npt.ArrayLike | list[npt.ArrayLike]:
+    """Fit the estimator and predict values for a given dataset split.
+
+    Parameters
+    ----------
+    estimator : estimator object implementing 'fit' and 'predict'
+        The object to use to fit the data.
+
+    X : array-like of shape (n_observations, n_assets)
+        The data to fit.
+
+    y : array-like of shape (n_observations, n_factors) or None
+        The factor array if provided
+
+    train : ndarray of int of shape (n_train_observations,)
+        Indices of training samples.
+
+    test : ndarray of int of shape (n_test_samples,) or list of ndarray
+        Indices of test samples or list of indices.
+
+    fit_params : dict
+        Parameters that will be passed to ``estimator.fit``.
+
+    method : str
+        Invokes the passed method name of the passed estimator.
+
+    column_indices : ndarray, optional
+        Indices of columns to select.
+        The default (`None`) is to select all columns.
+
+    Returns
+    -------
+    predictions : array-like or list of array-like
+        If `test` is an array, it returns the array-like result of calling
+        'estimator.method' on `test`.
+        Otherwise, if `test` is a list of arrays, it returns the list of array-like
+        results of calling 'estimator.method' on each test set in `test`.
+    """
+    fit_params = fit_params if fit_params is not None else {}
+    X, y = safe_split(X, y, indices=column_indices, axis=1)
+    X_train, y_train = safe_split(X, y, indices=train, axis=0)
+    if y_train is None:
+        estimator.fit(X_train, **fit_params)
+    else:
+        estimator.fit(X_train, y_train, **fit_params)
+    func = getattr(estimator, method)
+
+    if isinstance(test, list):
+        predictions = []
+        for t in test:
+            X_test, _ = safe_split(X, indices=t, axis=0)
+            predictions.append(func(X_test))
+    else:
+        X_test, _ = safe_split(X, indices=test, axis=0)
+        predictions = func(X_test)
+
+    return predictions
+
+
+def default_asset_names(n_assets: int) -> np.ndarray:
+    """Default asset names are `["x0", "x1", ..., "x(n_assets - 1)"]`
+
+    Parameters
+    ----------
+    n_assets : int
+        Number of assets.
+
+    Returns
+    -------
+    asset_names : ndarray of str
+        Default assets names.
+    """
+    return np.asarray([f"x{i}" for i in range(n_assets)], dtype=object)
+
+
+def deduplicate_names(names: npt.ArrayLike) -> list[str]:
+    """Rename duplicated names by appending "_{duplicate_nb}" at the end.
+
+    This function is inspired by the pandas function `_maybe_dedup_names`.
+
+    Parameters
+    ----------
+    names : array-like of shape (n_names,)
+        List of names.
+
+    Returns
+    -------
+    names : list[str]
+        Deduplicate names.
+    """
+    names = list(names)
+    counts = {}
+    for i, col in enumerate(names):
+        cur_count = counts.get(col, 0)
+        if cur_count > 0:
+            names[i] = f"{col}_{cur_count}"
+        counts[col] = cur_count + 1
+    return names
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `skfolio-0.1.3/src/skfolio/model_selection/_validation.py` & `skfolio-0.2.0/src/skfolio/model_selection/_validation.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.1.3/src/skfolio/model_selection/_walk_forward.py` & `skfolio-0.2.0/src/skfolio/model_selection/_walk_forward.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.1.3/src/skfolio/moments/__init__.py` & `skfolio-0.2.0/src/skfolio/moments/__init__.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.1.3/src/skfolio/moments/covariance/__init__.py` & `skfolio-0.2.0/src/skfolio/moments/covariance/__init__.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.1.3/src/skfolio/moments/covariance/_base.py` & `skfolio-0.2.0/src/skfolio/moments/covariance/_base.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.1.3/src/skfolio/moments/covariance/_covariance.py` & `skfolio-0.2.0/src/skfolio/moments/covariance/_covariance.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.1.3/src/skfolio/moments/expected_returns/_base.py` & `skfolio-0.2.0/src/skfolio/moments/expected_returns/_base.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.1.3/src/skfolio/moments/expected_returns/_expected_returns.py` & `skfolio-0.2.0/src/skfolio/moments/expected_returns/_expected_returns.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.1.3/src/skfolio/optimization/__init__.py` & `skfolio-0.2.0/src/skfolio/optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.1.3/src/skfolio/optimization/_base.py` & `skfolio-0.2.0/src/skfolio/optimization/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 
 class BaseOptimization(skb.BaseEstimator, ABC):
     """Base class for all portfolio optimizations in skfolio.
 
     portfolio_params :  dict, optional
         Portfolio parameters passed to the portfolio evaluated by the `predict` and
         `score` methods. If not provided, the `name`, `transaction_costs`,
-        `management_fees` and `previous_weights` are copied from the optimization
-        model and systematically passed to the portfolio.
+        `management_fees`, `previous_weights` and `risk_free_rate` are copied from the
+        optimization model and passed to the portfolio.
 
     Attributes
     ----------
     weights_ : ndarray of shape (n_assets,) or (n_optimizations, n_assets)
         Weights of the assets.
 
     Notes
@@ -80,15 +80,20 @@
 
         if self.portfolio_params is None:
             ptf_kwargs = {}
         else:
             ptf_kwargs = self.portfolio_params.copy()
 
         # Set the default portfolio parameters equal to the optimization parameters
-        for param in ["transaction_costs", "management_fees", "previous_weights"]:
+        for param in [
+            "transaction_costs",
+            "management_fees",
+            "previous_weights",
+            "risk_free_rate",
+        ]:
             if param not in ptf_kwargs and hasattr(self, param):
                 ptf_kwargs[param] = getattr(self, param)
 
         # If 'name' is not provided in the portfolio arguments, we use the first
         # 500 characters of the optimization estimator's name
         name = ptf_kwargs.pop("name", type(self).__name__)
```

### Comparing `skfolio-0.1.3/src/skfolio/optimization/cluster/_nco.py` & `skfolio-0.2.0/src/skfolio/optimization/cluster/_nco.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.1.3/src/skfolio/optimization/cluster/hierarchical/_base.py` & `skfolio-0.2.0/src/skfolio/optimization/cluster/hierarchical/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # Author: Hugo Delatte <delatte.hugo@gmail.com>
 # License: BSD 3 clause
 # Implementation derived from:
 # Riskfolio-Lib, Copyright (c) 2020-2023, Dany Cajas, Licensed under BSD 3 clause.
 # scikit-learn, Copyright (c) 2007-2010 David Cournapeau, Fabian Pedregosa, Olivier
 
 from abc import ABC, abstractmethod
+from typing import Any
 
 import numpy as np
 import numpy.typing as npt
 
 import skfolio.typing as skt
 from skfolio.cluster import HierarchicalClustering
 from skfolio.distance import BaseDistance
@@ -179,16 +180,16 @@
         (asset name/asset previous weight) and the input `X` of the `fit` method must
         be a DataFrame with the assets names in columns.
         The default (`None`) means no previous weights.
 
     portfolio_params :  dict, optional
         Portfolio parameters passed to the portfolio evaluated by the `predict` and
         `score` methods. If not provided, the `name`, `transaction_costs`,
-        `management_fees` and `previous_weights` are copied from the optimization
-        model and systematically passed to the portfolio.
+        `management_fees`, `previous_weights` and `risk_free_rate` are copied from the
+        optimization model and passed to the portfolio.
 
     Attributes
     ----------
     weights_ : ndarray of shape (n_assets,)
         Weights of the assets.
 
     prior_estimator_ : BasePrior
@@ -231,30 +232,30 @@
         self.previous_weights = previous_weights
         self._seriated = False
 
     def _clean_input(
         self,
         value: float | dict | np.ndarray | list,
         n_assets: int,
-        fill_value: any,
+        fill_value: Any,
         name: str,
     ) -> np.ndarray:
         """Convert input to cleaned 1D array
          value : float, dict, array-like or None.
             Input value to clean and convert.
 
         Parameters
         ----------
         value : float, dict or array-like.
             Input value to clean.
 
         n_assets : int
             Number of assets. Used to verify the shape of the converted array.
 
-        fill_value : any
+        fill_value : Any
             When `items` is a dictionary, elements that are not in `asset_names` are
             filled with `fill_value` in the converted array.
 
         name : str
             Name used for error messages.
 
         Returns
```

### Comparing `skfolio-0.1.3/src/skfolio/optimization/cluster/hierarchical/_herc.py` & `skfolio-0.2.0/src/skfolio/optimization/cluster/hierarchical/_herc.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,16 +200,16 @@
         (asset name/asset previous weight) and the input `X` of the `fit` method must
         be a DataFrame with the assets names in columns.
         The default (`None`) means no previous weights.
 
     portfolio_params :  dict, optional
         Portfolio parameters passed to the portfolio evaluated by the `predict` and
         `score` methods. If not provided, the `name`, `transaction_costs`,
-        `management_fees` and `previous_weights` are copied from the optimization
-        model and systematically passed to the portfolio.
+        `management_fees`, `previous_weights` and `risk_free_rate` are copied from the
+        optimization model and passed to the portfolio.
 
     Attributes
     ----------
     weights_ : ndarray of shape (n_assets,)
         Weights of the assets.
 
     distance_estimator_ : BaseDistance
```

### Comparing `skfolio-0.1.3/src/skfolio/optimization/cluster/hierarchical/_hrp.py` & `skfolio-0.2.0/src/skfolio/optimization/cluster/hierarchical/_hrp.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,16 +200,16 @@
         (asset name/asset previous weight) and the input `X` of the `fit` method must
         be a DataFrame with the assets names in columns.
         The default (`None`) means no previous weights.
 
     portfolio_params :  dict, optional
         Portfolio parameters passed to the portfolio evaluated by the `predict` and
         `score` methods. If not provided, the `name`, `transaction_costs`,
-        `management_fees` and `previous_weights` are copied from the optimization
-        model and systematically passed to the portfolio.
+        `management_fees`, `previous_weights` and `risk_free_rate` are copied from the
+        optimization model and passed to the portfolio.
 
     Attributes
     ----------
     weights_ : ndarray of shape (n_assets,)
         Weights of the assets.
 
     distance_estimator_ : BaseDistance
```

### Comparing `skfolio-0.1.3/src/skfolio/optimization/convex/__init__.py` & `skfolio-0.2.0/src/skfolio/optimization/convex/__init__.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.1.3/src/skfolio/optimization/convex/_base.py` & `skfolio-0.2.0/src/skfolio/optimization/convex/_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # License: BSD 3 clause
 # The optimization features are derived
 # from Riskfolio-Lib, Copyright (c) 2020-2023, Dany Cajas, Licensed under BSD 3 clause.
 
 import warnings
 from abc import ABC, abstractmethod
 from enum import auto
+from typing import Any
 
 import cvxpy as cp
 import cvxpy.constraints.constraint as cpc
 import numpy as np
 import numpy.typing as npt
 import scipy as sc
 import scipy.sparse.linalg as scl
@@ -399,16 +400,16 @@
     raise_on_failure : bool, default=True
         If this is set to True, an error is raised when the optimization fail otherwise
         it passes with a warning.
 
     portfolio_params :  dict, optional
         Portfolio parameters passed to the portfolio evaluated by the `predict` and
         `score` methods. If not provided, the `name`, `transaction_costs`,
-        `management_fees` and `previous_weights` are copied from the optimization
-        model and systematically passed to the portfolio.
+        `management_fees`, `previous_weights` and `risk_free_rate` are copied from the
+        optimization model and passed to the portfolio.
 
     Attributes
     ----------
     weights_ : ndarray of shape (n_assets,) or (n_optimizations, n_assets)
         Weights of the assets.
 
     problem_values_ :  dict[str, float] | list[dict[str, float]] of size n_optimizations
@@ -571,28 +572,28 @@
                 "the weight variable OR the weight variable and the estimator object."
             ) from err
 
     def _clean_input(
         self,
         value: float | dict | npt.ArrayLike | None,
         n_assets: int,
-        fill_value: any,
+        fill_value: Any,
         name: str,
     ) -> float | np.ndarray:
         """Convert input to cleaned float or ndarray.
 
         Parameters
         ----------
         value : float, dict, array-like or None.
             Input value to clean.
 
         n_assets : int
             Number of assets. Used to verify the shape of the converted array.
 
-        fill_value : any
+        fill_value : Any
             When `items` is a dictionary, elements that are not in `asset_names` are
             filled with `fill_value` in the converted array.
 
         name : str
             Name used for error messages.
 
         Returns
```

### Comparing `skfolio-0.1.3/src/skfolio/optimization/convex/_distributionally_robust.py` & `skfolio-0.2.0/src/skfolio/optimization/convex/_distributionally_robust.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,16 +204,16 @@
     raise_on_failure : bool, default=True
         If this is set to True, an error is raised when the optimization fail otherwise
         it passes with a warning.
 
     portfolio_params :  dict, optional
         Portfolio parameters passed to the portfolio evaluated by the `predict` and
         `score` methods. If not provided, the `name`, `transaction_costs`,
-        `management_fees` and `previous_weights` are copied from the optimization
-        model and systematically passed to the portfolio.
+        `management_fees`, `previous_weights` and `risk_free_rate` are copied from the
+        optimization model and passed to the portfolio.
 
     Attributes
     ----------
     weights_ : ndarray of shape (n_assets,) or (n_optimizations, n_assets)
         Weights of the assets.
 
     problem_values_ :  dict[str, float] | list[dict[str, float]] of size n_optimizations
```

### Comparing `skfolio-0.1.3/src/skfolio/optimization/convex/_maximum_diversification.py` & `skfolio-0.2.0/src/skfolio/optimization/convex/_maximum_diversification.py`

 * *Files 2% similar despite different names*

```diff
@@ -299,16 +299,16 @@
     raise_on_failure : bool, default=True
         If this is set to True, an error is raised when the optimization fail otherwise
         it passes with a warning.
 
     portfolio_params :  dict, optional
         Portfolio parameters passed to the portfolio evaluated by the `predict` and
         `score` methods. If not provided, the `name`, `transaction_costs`,
-        `management_fees` and `previous_weights` are copied from the optimization
-        model and systematically passed to the portfolio.
+        `management_fees`, `previous_weights` and `risk_free_rate` are copied from the
+        optimization model and passed to the portfolio.
 
     Attributes
     ----------
     weights_ : ndarray of shape (n_assets,) or (n_optimizations, n_assets)
         Weights of the assets.
 
     problem_values_ :  dict[str, float] | list[dict[str, float]] of size n_optimizations
```

### Comparing `skfolio-0.1.3/src/skfolio/optimization/convex/_mean_risk.py` & `skfolio-0.2.0/src/skfolio/optimization/convex/_mean_risk.py`

 * *Files 0% similar despite different names*

```diff
@@ -506,16 +506,16 @@
     raise_on_failure : bool, default=True
         If this is set to True, an error is raised when the optimization fail otherwise
         it passes with a warning.
 
     portfolio_params :  dict, optional
         Portfolio parameters passed to the portfolio evaluated by the `predict` and
         `score` methods. If not provided, the `name`, `transaction_costs`,
-        `management_fees` and `previous_weights` are copied from the optimization
-        model and systematically passed to the portfolio.
+        `management_fees`, `previous_weights` and `risk_free_rate` are copied from the 
+        optimization model and passed to the portfolio.
 
     Attributes
     ----------
     weights_ : ndarray of shape (n_assets,) or (n_optimizations, n_assets)
         Weights of the assets.
 
     problem_values_ :  dict[str, float] | list[dict[str, float]] of size n_optimizations
```

### Comparing `skfolio-0.1.3/src/skfolio/optimization/convex/_risk_budgeting.py` & `skfolio-0.2.0/src/skfolio/optimization/convex/_risk_budgeting.py`

 * *Files 0% similar despite different names*

```diff
@@ -336,16 +336,16 @@
     raise_on_failure : bool, default=True
         If this is set to True, an error is raised when the optimization fail otherwise
         it passes with a warning.
 
     portfolio_params :  dict, optional
         Portfolio parameters passed to the portfolio evaluated by the `predict` and
         `score` methods. If not provided, the `name`, `transaction_costs`,
-        `management_fees` and `previous_weights` are copied from the optimization
-        model and systematically passed to the portfolio.
+        `management_fees`, `previous_weights` and `risk_free_rate` are copied from the 
+        optimization model and passed to the portfolio.
 
     Attributes
     ----------
     weights_ : ndarray of shape (n_assets,) or (n_optimizations, n_assets)
         Weights of the assets.
 
     problem_values_ :  dict[str, float] | list[dict[str, float]] of size n_optimizations
```

### Comparing `skfolio-0.1.3/src/skfolio/optimization/ensemble/_base.py` & `skfolio-0.2.0/src/skfolio/optimization/ensemble/_base.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.1.3/src/skfolio/optimization/ensemble/_stacking.py` & `skfolio-0.2.0/src/skfolio/optimization/ensemble/_stacking.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.1.3/src/skfolio/optimization/naive/_naive.py` & `skfolio-0.2.0/src/skfolio/optimization/naive/_naive.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,16 +27,16 @@
         containing the estimation of assets expected returns, covariance matrix,
         returns and Cholesky decomposition of the covariance.
         The default (`None`) is to use :class:`~skfolio.prior.EmpiricalPrior`.
 
     portfolio_params :  dict, optional
         Portfolio parameters passed to the portfolio evaluated by the `predict` and
         `score` methods. If not provided, the `name`, `transaction_costs`,
-        `management_fees` and `previous_weights` are copied from the optimization
-        model and systematically passed to the portfolio.
+        `management_fees`, `previous_weights` and `risk_free_rate` are copied from the
+        optimization model and passed to the portfolio.
 
     Attributes
     ----------
     weights_ : ndarray of shape (n_assets,) or (n_optimizations, n_assets)
         Weights of the assets.
 
     prior_estimator_ : BasePrior
@@ -91,16 +91,16 @@
     Each asset weight is equal to `1/n_assets`.
 
     Parameters
     ----------
     portfolio_params :  dict, optional
         Portfolio parameters passed to the portfolio evaluated by the `predict` and
         `score` methods. If not provided, the `name`, `transaction_costs`,
-        `management_fees` and `previous_weights` are copied from the optimization
-        model and systematically passed to the portfolio.
+        `management_fees`, `previous_weights` and `risk_free_rate` are copied from the
+        optimization model and passed to the portfolio.
 
     Attributes
     ----------
     weights_ : ndarray of shape (n_assets,) or (n_optimizations, n_assets)
         Weights of the assets.
     """
 
@@ -135,16 +135,16 @@
     The assets weight are drawn from a Dirichlet distribution and sum to one.
 
     Parameters
     ----------
     portfolio_params :  dict, optional
         Portfolio parameters passed to the portfolio evaluated by the `predict` and
         `score` methods. If not provided, the `name`, `transaction_costs`,
-        `management_fees` and `previous_weights` are copied from the optimization
-        model and systematically passed to the portfolio.
+        `management_fees`, `previous_weights` and `risk_free_rate` are copied from the
+        optimization model and passed to the portfolio.
 
     Attributes
     ----------
     weights_ : ndarray of shape (n_assets,) or (n_optimizations, n_assets)
         Weights of the assets.
     """
```

### Comparing `skfolio-0.1.3/src/skfolio/population/_population.py` & `skfolio-0.2.0/src/skfolio/population/_population.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,89 +3,90 @@
 """
 
 # Copyright (c) 2023
 # Author: Hugo Delatte <delatte.hugo@gmail.com>
 # License: BSD 3 clause
 
 import inspect
+from typing import Any
 
 import numpy as np
 import pandas as pd
 import plotly.express as px
 import plotly.graph_objects as go
 import scipy.interpolate as sci
 
 import skfolio.typing as skt
-from skfolio.portfolio import BasePortfolio, MultiPeriodPortfolio, Portfolio
+from skfolio.portfolio import BasePortfolio, MultiPeriodPortfolio
 from skfolio.utils.sorting import non_denominated_sort
 from skfolio.utils.tools import deduplicate_names
 
 pd.options.plotting.backend = "plotly"
 
 
 class Population(list):
     """Population Class.
 
     A `Population` is a list of :class:`~skfolio.portfolio.Portfolio` or
     :class:`~skfolio.portfolio.MultiPeriodPortfolio` or both.
 
     Parameters
     ----------
-    iterable : list[Portfolio | MultiPeriodPortfolio]
+    iterable : list[BasePortfolio]
         The list of portfolios. Each item can be of type
         :class:`~skfolio.portfolio.Portfolio` and/or
         :class:`~skfolio.portfolio.MultiPeriodPortfolio`.
         Empty list are accepted.
     """
 
-    def __init__(self, iterable: list[Portfolio | MultiPeriodPortfolio]) -> None:
+    def __init__(self, iterable: list[BasePortfolio]) -> None:
         super().__init__(self._validate_item(item) for item in iterable)
 
     def __repr__(self) -> str:
         return "<Population(" + super().__repr__() + ")>"
 
     def __getitem__(
         self, indices: int | list[int] | slice
-    ) -> "Portfolio | MultiPeriodPortfolio|Population":
+    ) -> "BasePortfolio | Population":
         item = super().__getitem__(indices)
         if isinstance(item, list):
             return self.__class__(item)
         return item
 
-    def __setitem__(self, index: int, item: Portfolio | MultiPeriodPortfolio) -> None:
+    def __setitem__(self, index: int, item: BasePortfolio) -> None:
         super().__setitem__(index, self._validate_item(item))
 
-    def __add__(self, other: Portfolio | MultiPeriodPortfolio) -> "Population":
+    def __add__(self, other: BasePortfolio) -> "Population":
         if not isinstance(other, Population):
             raise TypeError(
                 f"Cannot add a Population with an object of type {type(other)}"
             )
         return self.__class__(super().__add__(other))
 
-    def insert(self, index, item: Portfolio | MultiPeriodPortfolio) -> None:
+    def insert(self, index, item: BasePortfolio) -> None:
         """Insert portfolio before index."""
         super().insert(index, self._validate_item(item))
 
-    def append(self, item: Portfolio | MultiPeriodPortfolio) -> None:
+    def append(self, item: BasePortfolio) -> None:
         """Append portfolio to the end of the population list."""
         super().append(self._validate_item(item))
 
-    def extend(self, other: Portfolio | MultiPeriodPortfolio) -> None:
+    def extend(self, other: BasePortfolio) -> None:
         """Extend population list by appending elements from the iterable."""
         if isinstance(other, type(self)):
             super().extend(other)
         else:
             super().extend(self._validate_item(item) for item in other)
 
-    def set_portfolio_params(self, **params: any) -> "Population":
+    def set_portfolio_params(self, **params: Any) -> "Population":
         """Set the parameters of all the portfolios.
 
         Parameters
         ----------
-        **params : any
+        **params : Any
             Portfolio parameters.
 
         Returns
         -------
         self : Population
             The Population instance.
         """
@@ -107,21 +108,22 @@
 
         for portfolio in self:
             for key, value in params.items():
                 setattr(portfolio, key, value)
 
     @staticmethod
     def _validate_item(
-        item: Portfolio | MultiPeriodPortfolio,
-    ) -> Portfolio | MultiPeriodPortfolio:
+        item: BasePortfolio,
+    ) -> BasePortfolio:
         """Validate that items are of type Portfolio or MultiPeriodPortfolio."""
-        if isinstance(item, Portfolio | MultiPeriodPortfolio):
+        if isinstance(item, BasePortfolio):
             return item
         raise TypeError(
-            "Population only accept items of type Portfolio and MultiPeriodPortfolio"
+            "Population only accept items that inherit from BasePortfolio such as "
+            "Portfolio or MultiPeriodPortfolio"
             f", got {type(item).__name__}"
         )
 
     def non_denominated_sort(self, first_front_only: bool = False) -> list[list[int]]:
         """Fast non-dominated sorting.
         Sort the portfolios into different non-domination levels.
         Complexity O(MN^2) where M is the number of objectives and N the number of
@@ -320,15 +322,15 @@
 
     def quantile(
         self,
         measure: skt.Measure,
         q: float,
         names: skt.Names | None = None,
         tags: skt.Tags | None = None,
-    ) -> Portfolio | MultiPeriodPortfolio:
+    ) -> BasePortfolio:
         """Returns the portfolio corresponding to the `q` quantile for a given portfolio
         measure.
 
         Parameters
         ----------
         measure : Measure
             The portfolio measure.
@@ -340,15 +342,15 @@
             If provided, the population is filtered by portfolio names.
 
         tags : str | list[str], optional
             If provided, the population is filtered by portfolio tags.
 
         Returns
         -------
-        values : Portfolio | MultiPeriodPortfolio
+        values : BasePortfolio
            Portfolio corresponding to the `q` quantile for the measure.
         """
         if not 0 <= q <= 1:
             raise ValueError("The quantile`q` must be between 0 and 1")
         sorted_portfolios = self.sort_measure(
             measure=measure, reverse=False, names=names, tags=tags
         )
@@ -356,15 +358,15 @@
         return sorted_portfolios[k]
 
     def min_measure(
         self,
         measure: skt.Measure,
         names: skt.Names | None = None,
         tags: skt.Tags | None = None,
-    ) -> Portfolio | MultiPeriodPortfolio:
+    ) -> BasePortfolio:
         """Returns the portfolio with the minimum measure.
 
         Parameters
         ----------
         measure : Measure
             The portfolio measure.
 
@@ -372,25 +374,25 @@
             If provided, the population is filtered by portfolio names.
 
         tags : str | list[str], optional
             If provided, the population is filtered by portfolio tags.
 
         Returns
         -------
-        values : Portfolio | MultiPeriodPortfolio
+        values : BasePortfolio
             The portfolio with minimum measure.
         """
         return self.quantile(measure=measure, q=0, names=names, tags=tags)
 
     def max_measure(
         self,
         measure: skt.Measure,
         names: skt.Names | None = None,
         tags: skt.Tags | None = None,
-    ) -> Portfolio | MultiPeriodPortfolio:
+    ) -> BasePortfolio:
         """Returns the portfolio with the maximum measure.
 
         Parameters
         ----------
         measure: Measure
             The portfolio measure.
 
@@ -398,15 +400,15 @@
             If provided, the population is filtered by portfolio names.
 
         tags : str | list[str], optional
             If provided, the population is filtered by portfolio tags.
 
         Returns
         -------
-        values : Portfolio | MultiPeriodPortfolio
+        values : BasePortfolio
             The portfolio with maximum measure.
         """
         return self.quantile(measure=measure, q=1, names=names, tags=tags)
 
     def summary(
         self,
         formatted: bool = True,
```

### Comparing `skfolio-0.1.3/src/skfolio/portfolio/__init__.py` & `skfolio-0.2.0/src/skfolio/portfolio/__init__.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.1.3/src/skfolio/portfolio/_base.py` & `skfolio-0.2.0/src/skfolio/portfolio/_base.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.1.3/src/skfolio/portfolio/_multi_period_portfolio.py` & `skfolio-0.2.0/src/skfolio/portfolio/_multi_period_portfolio.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.1.3/src/skfolio/portfolio/_portfolio.py` & `skfolio-0.2.0/src/skfolio/portfolio/_portfolio.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.1.3/src/skfolio/pre_selection/_pre_selection.py` & `skfolio-0.2.0/src/skfolio/pre_selection/_pre_selection.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.1.3/src/skfolio/preprocessing/_returns.py` & `skfolio-0.2.0/src/skfolio/preprocessing/_returns.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.1.3/src/skfolio/prior/_base.py` & `skfolio-0.2.0/src/skfolio/prior/_base.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.1.3/src/skfolio/prior/_black_litterman.py` & `skfolio-0.2.0/src/skfolio/prior/_black_litterman.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.1.3/src/skfolio/prior/_empirical.py` & `skfolio-0.2.0/src/skfolio/prior/_empirical.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.1.3/src/skfolio/prior/_factor_model.py` & `skfolio-0.2.0/src/skfolio/prior/_factor_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # License: BSD 3 clause
 # Implementation derived from:
 # Riskfolio-Lib, Copyright (c) 2020-2023, Dany Cajas, Licensed under BSD 3 clause.
 # scikit-learn, Copyright (c) 2007-2010 David Cournapeau, Fabian Pedregosa, Olivier
 # Grisel Licensed under BSD 3 clause.
 
 from abc import ABC, abstractmethod
+from typing import Any
 
 import numpy as np
 import numpy.typing as npt
 import sklearn.base as skb
 import sklearn.linear_model as skl
 import sklearn.multioutput as skm
 
@@ -192,15 +193,15 @@
         self.loading_matrix_estimator = loading_matrix_estimator
         self.factor_prior_estimator = factor_prior_estimator
         self.residual_variance = residual_variance
         self.higham = higham
         self.max_iteration = max_iteration
 
     # noinspection PyMethodOverriding, PyPep8Naming
-    def fit(self, X: npt.ArrayLike, y: any):
+    def fit(self, X: npt.ArrayLike, y: Any):
         """Fit the Factor Model estimator.
 
         Parameters
         ----------
         X : array-like of shape (n_observations, n_assets)
             Price returns of the assets.
```

### Comparing `skfolio-0.1.3/src/skfolio/typing.py` & `skfolio-0.2.0/src/skfolio/typing.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.1.3/src/skfolio/uncertainty_set/__init__.py` & `skfolio-0.2.0/src/skfolio/uncertainty_set/__init__.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.1.3/src/skfolio/uncertainty_set/_base.py` & `skfolio-0.2.0/src/skfolio/uncertainty_set/_base.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.1.3/src/skfolio/uncertainty_set/_bootstrap.py` & `skfolio-0.2.0/src/skfolio/uncertainty_set/_bootstrap.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.1.3/src/skfolio/uncertainty_set/_empirical.py` & `skfolio-0.2.0/src/skfolio/uncertainty_set/_empirical.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.1.3/src/skfolio/utils/bootstrap.py` & `skfolio-0.2.0/src/skfolio/utils/bootstrap.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.1.3/src/skfolio/utils/equations.py` & `skfolio-0.2.0/src/skfolio/utils/equations.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.1.3/src/skfolio/utils/fixes/_dendrogram.py` & `skfolio-0.2.0/src/skfolio/utils/fixes/_dendrogram.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.1.3/src/skfolio/utils/sorting.py` & `skfolio-0.2.0/src/skfolio/utils/sorting.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.1.3/src/skfolio/utils/stats.py` & `skfolio-0.2.0/src/skfolio/utils/stats.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.1.3/src/skfolio.egg-info/PKG-INFO` & `skfolio-0.2.0/src/skfolio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skfolio
-Version: 0.1.3
+Version: 0.2.0
 Summary: Portfolio optimization built on top of scikit-learn
 Author-email: Hugo Delatte <delatte.hugo@gmail.com>
 Maintainer-email: Hugo Delatte <delatte.hugo@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2007-2023 The skfolio developers.
         All rights reserved.
@@ -81,45 +81,45 @@
 Requires-Dist: sphinx-prompt; extra == "docs"
 Requires-Dist: sphinxext.opengraph; extra == "docs"
 Requires-Dist: sphinx-sitemap; extra == "docs"
 Requires-Dist: sphinx-favicon; extra == "docs"
 
 .. -*- mode: rst -*-
 
-|Licence|_ |Codecov|_ |Black|_ |PythonVersion|_ |PyPi|_ |CI/CD|_ |Downloads|_ |Ruff|_ |Contribution|_ |Website|_
+|Licence| |Codecov| |Black| |PythonVersion| |PyPi| |CI/CD| |Downloads| |Ruff| |Contribution| |Website|
 
 .. |Licence| image:: https://img.shields.io/badge/License-BSD%203--Clause-blue.svg
-.. _Licence: https://github.com/skfolio/skfolio/blob/main/LICENSE
+   :target: https://github.com/skfolio/skfolio/blob/main/LICENSE
 
 .. |Codecov| image:: https://codecov.io/gh/skfolio/skfolio/graph/badge.svg?token=KJ0SE4LHPV
-.. _Codecov: https://codecov.io/gh/skfolio/skfolio
+   :target: https://codecov.io/gh/skfolio/skfolio
 
-.. |PythonVersion| image:: https://img.shields.io/badge/python-3.10%20%7C%203.11%20%7C%203.12-blue
-.. _PythonVersion: https://pypi.org/project/skfolio/
+.. |PythonVersion| image:: https://img.shields.io/badge/python-3.10%20%7C%203.11%20%7C%203.12-blue.svg
+   :target: https://pypi.org/project/skfolio/
 
 .. |PyPi| image:: https://img.shields.io/pypi/v/skfolio
-.. _PyPi: https://pypi.org/project/skfolio
+   :target: https://pypi.org/project/skfolio
 
 .. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
-.. _Black: https://github.com/psf/black
+   :target: https://github.com/psf/black
 
-.. |CI/CD| image:: https://img.shields.io/github/actions/workflow/status/skfolio/skfolio/release.yml?logo=github
-.. _CI/CD: https://github.com/skfolio/skfolio/raw/main/LICENSE
+.. |CI/CD| image:: https://img.shields.io/github/actions/workflow/status/skfolio/skfolio/release.yml.svg?logo=github
+   :target: https://github.com/skfolio/skfolio/raw/main/LICENSE
 
 .. |Downloads| image:: https://static.pepy.tech/badge/skfolio
-.. _Downloads: https://pepy.tech/project/skfolio
+   :target: https://pepy.tech/project/skfolio
 
 .. |Ruff| image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json
-.. _Ruff: https://github.com/astral-sh/ruff
+   :target: https://github.com/astral-sh/ruff
 
 .. |Contribution| image:: https://img.shields.io/badge/Contributions-Welcome-blue
-.. _Contribution: https://github.com/skfolio/skfolio/blob/main/CONTRIBUTING.md
+   :target: https://github.com/skfolio/skfolio/blob/main/CONTRIBUTING.md
 
-.. |Website| image:: https://img.shields.io/website-up-down-53cc0d-red/http/skfolio.org
-.. _Website: https://skfolio.org
+.. |Website| image:: https://img.shields.io/website.svg?down_color=red&down_message=down&up_color=53cc0d&up_message=up&url=https://skfolio.org
+   :target: https://skfolio.org
 
 .. |PythonMinVersion| replace:: 3.10
 .. |NumpyMinVersion| replace:: 1.23.4
 .. |ScipyMinVersion| replace:: 1.8.0
 .. |PandasMinVersion| replace:: 1.4.1
 .. |CvxpyMinVersion| replace:: 1.4.1
 .. |SklearnMinVersion| replace:: 1.3.2
```

### Comparing `skfolio-0.1.3/src/skfolio.egg-info/SOURCES.txt` & `skfolio-0.2.0/src/skfolio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

