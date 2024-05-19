# Comparing `tmp/aq_geometric-2024.5.1.2.tar.gz` & `tmp/aq_geometric-2024.5.19.1.tar.gz`

## Comparing `aq_geometric-2024.5.1.2.tar` & `aq_geometric-2024.5.19.1.tar`

### file list

```diff
@@ -1,70 +1,70 @@
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/requirements.txt
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/aq_geometric/__init__.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/aq_geometric/data/__init__.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/aq_geometric/data/file/__init__.py
--rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/aq_geometric/data/file/local.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/aq_geometric/data/filter/__init__.py
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/aq_geometric/data/filter/node_features.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/aq_geometric/data/graph/__init__.py
--rw-r--r--   0        0        0     5172 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/aq_geometric/data/graph/compute_graph.py
--rw-r--r--   0        0        0    17055 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/aq_geometric/data/graph/graphs_builder.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/aq_geometric/data/graph/edges/__init__.py
--rw-r--r--   0        0        0     7337 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/aq_geometric/data/graph/edges/compute_edges.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/aq_geometric/data/graph/nodes/__init__.py
--rw-r--r--   0        0        0    14503 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/aq_geometric/data/graph/nodes/compute_node_features.py
--rw-r--r--   0        0        0    10409 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/aq_geometric/data/graph/nodes/compute_nodes.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/aq_geometric/data/reindex/__init__.py
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/aq_geometric/data/reindex/features.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/aq_geometric/data/remote/__init__.py
--rw-r--r--   0        0        0     6877 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/aq_geometric/data/remote/psql.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/aq_geometric/datasets/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/aq_geometric/datasets/in_memory/__init__.py
--rw-r--r--   0        0        0    11724 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/aq_geometric/datasets/in_memory/aq_geometric_dataset.py
--rw-r--r--   0        0        0    26866 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/aq_geometric/datasets/on_disk/aq_geometric_dataset.py
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/aq_geometric/models/__init__.py
--rw-r--r--   0        0        0     9747 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/aq_geometric/models/base_model.py
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/aq_geometric/models/test_base_model.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/aq_geometric/models/edge_conv/__init__.py
--rw-r--r--   0        0        0     6322 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/aq_geometric/models/edge_conv/edge_conv.py
--rw-r--r--   0        0        0     3584 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/aq_geometric/models/edge_conv/test_edge_conv.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/aq_geometric/models/gcn/__init__.py
--rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/aq_geometric/models/gcn/gcn.py
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/aq_geometric/models/gcn/test_gcn.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/aq_geometric/models/hierarchical_edge_conv/__init__.py
--rw-r--r--   0        0        0    18524 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/aq_geometric/models/hierarchical_edge_conv/heirarchical_edge_conv.py
--rw-r--r--   0        0        0     3368 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/aq_geometric/models/hierarchical_edge_conv/test_heirarchical_edge_conv.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/aq_geometric/models/hierarchical_xgb/__init__.py
--rw-r--r--   0        0        0    31182 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/aq_geometric/models/hierarchical_xgb/base_hierarchical_xgb.py
--rw-r--r--   0        0        0     8125 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/aq_geometric/models/hierarchical_xgb/hierarchical_xgb_direct.py
--rw-r--r--   0        0        0    10666 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/aq_geometric/models/hierarchical_xgb/hierarchical_xgb_iterative.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/aq_geometric/models/message_passing/__init__.py
--rw-r--r--   0        0        0    14655 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/aq_geometric/models/message_passing/message_passing.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/aq_geometric/models/message_passing/test_message_passing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/aq_geometric/models/statistical_baselines/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/aq_geometric/models/statistical_baselines/climatology/__init__.py
--rw-r--r--   0        0        0     8464 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/aq_geometric/models/statistical_baselines/climatology/climatology.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/aq_geometric/models/statistical_baselines/linear/__init__.py
--rw-r--r--   0        0        0     7812 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/aq_geometric/models/statistical_baselines/linear/linear.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/aq_geometric/models/statistical_baselines/persistance/__init__.py
--rw-r--r--   0        0        0     8381 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/aq_geometric/models/statistical_baselines/persistance/persistance.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/aq_geometric/models/statistical_baselines/temporal/__init__.py
--rw-r--r--   0        0        0     9011 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/aq_geometric/models/statistical_baselines/temporal/temporal.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/aq_geometric/transforms/__init__.py
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/aq_geometric/transforms/change.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/aq_geometric/utils/__init__.py
--rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/aq_geometric/utils/evaluation.py
--rw-r--r--   0        0        0     6336 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/aq_geometric/utils/forecasts.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/aq_geometric/utils/station_filters.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/aq_geometric/utils/test_evaluation.py
--rw-r--r--   0        0        0     5440 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/aq_geometric/utils/test_forecasts.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/aq_geometric/utils/test_station_filters.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/tests/config/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/tests/data/__init__.py
--rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/tests/data/test_aq.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/tests/datasets/__init__.py
--rw-r--r--   0        0        0    10356 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/tests/datasets/test_aq.py
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/LICENSE.md
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/README.md
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/pyproject.toml
--rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.2/PKG-INFO
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/requirements.txt
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/aq_geometric/__init__.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/aq_geometric/data/__init__.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/aq_geometric/data/file/__init__.py
+-rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/aq_geometric/data/file/local.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/aq_geometric/data/filter/__init__.py
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/aq_geometric/data/filter/node_features.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/aq_geometric/data/graph/__init__.py
+-rw-r--r--   0        0        0     5172 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/aq_geometric/data/graph/compute_graph.py
+-rw-r--r--   0        0        0    17055 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/aq_geometric/data/graph/graphs_builder.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/aq_geometric/data/graph/edges/__init__.py
+-rw-r--r--   0        0        0     7337 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/aq_geometric/data/graph/edges/compute_edges.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/aq_geometric/data/graph/nodes/__init__.py
+-rw-r--r--   0        0        0    14503 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/aq_geometric/data/graph/nodes/compute_node_features.py
+-rw-r--r--   0        0        0    10409 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/aq_geometric/data/graph/nodes/compute_nodes.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/aq_geometric/data/reindex/__init__.py
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/aq_geometric/data/reindex/features.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/aq_geometric/data/remote/__init__.py
+-rw-r--r--   0        0        0     6877 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/aq_geometric/data/remote/psql.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/aq_geometric/datasets/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/aq_geometric/datasets/in_memory/__init__.py
+-rw-r--r--   0        0        0    11724 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/aq_geometric/datasets/in_memory/aq_geometric_dataset.py
+-rw-r--r--   0        0        0    26866 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/aq_geometric/datasets/on_disk/aq_geometric_dataset.py
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/aq_geometric/models/__init__.py
+-rw-r--r--   0        0        0     9747 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/aq_geometric/models/base_model.py
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/aq_geometric/models/test_base_model.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/aq_geometric/models/edge_conv/__init__.py
+-rw-r--r--   0        0        0     6322 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/aq_geometric/models/edge_conv/edge_conv.py
+-rw-r--r--   0        0        0     3584 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/aq_geometric/models/edge_conv/test_edge_conv.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/aq_geometric/models/gcn/__init__.py
+-rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/aq_geometric/models/gcn/gcn.py
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/aq_geometric/models/gcn/test_gcn.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/aq_geometric/models/hierarchical_edge_conv/__init__.py
+-rw-r--r--   0        0        0    18524 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/aq_geometric/models/hierarchical_edge_conv/heirarchical_edge_conv.py
+-rw-r--r--   0        0        0     3368 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/aq_geometric/models/hierarchical_edge_conv/test_heirarchical_edge_conv.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/aq_geometric/models/hierarchical_xgb/__init__.py
+-rw-r--r--   0        0        0    31182 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/aq_geometric/models/hierarchical_xgb/base_hierarchical_xgb.py
+-rw-r--r--   0        0        0     8125 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/aq_geometric/models/hierarchical_xgb/hierarchical_xgb_direct.py
+-rw-r--r--   0        0        0    10666 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/aq_geometric/models/hierarchical_xgb/hierarchical_xgb_iterative.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/aq_geometric/models/message_passing/__init__.py
+-rw-r--r--   0        0        0    15259 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/aq_geometric/models/message_passing/message_passing.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/aq_geometric/models/message_passing/test_message_passing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/aq_geometric/models/statistical_baselines/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/aq_geometric/models/statistical_baselines/climatology/__init__.py
+-rw-r--r--   0        0        0     8464 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/aq_geometric/models/statistical_baselines/climatology/climatology.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/aq_geometric/models/statistical_baselines/linear/__init__.py
+-rw-r--r--   0        0        0     7812 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/aq_geometric/models/statistical_baselines/linear/linear.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/aq_geometric/models/statistical_baselines/persistance/__init__.py
+-rw-r--r--   0        0        0     8381 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/aq_geometric/models/statistical_baselines/persistance/persistance.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/aq_geometric/models/statistical_baselines/temporal/__init__.py
+-rw-r--r--   0        0        0     9011 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/aq_geometric/models/statistical_baselines/temporal/temporal.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/aq_geometric/transforms/__init__.py
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/aq_geometric/transforms/change.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/aq_geometric/utils/__init__.py
+-rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/aq_geometric/utils/evaluation.py
+-rw-r--r--   0        0        0     6336 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/aq_geometric/utils/forecasts.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/aq_geometric/utils/station_filters.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/aq_geometric/utils/test_evaluation.py
+-rw-r--r--   0        0        0     5440 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/aq_geometric/utils/test_forecasts.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/aq_geometric/utils/test_station_filters.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/tests/config/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/tests/data/__init__.py
+-rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/tests/data/test_aq.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/tests/datasets/__init__.py
+-rw-r--r--   0        0        0    10356 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/tests/datasets/test_aq.py
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/LICENSE.md
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/README.md
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/pyproject.toml
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 aq_geometric-2024.5.19.1/PKG-INFO
```

### Comparing `aq_geometric-2024.5.1.2/aq_geometric/data/file/local.py` & `aq_geometric-2024.5.19.1/aq_geometric/data/file/local.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.5.1.2/aq_geometric/data/filter/node_features.py` & `aq_geometric-2024.5.19.1/aq_geometric/data/filter/node_features.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.5.1.2/aq_geometric/data/graph/compute_graph.py` & `aq_geometric-2024.5.19.1/aq_geometric/data/graph/compute_graph.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.5.1.2/aq_geometric/data/graph/graphs_builder.py` & `aq_geometric-2024.5.19.1/aq_geometric/data/graph/graphs_builder.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.5.1.2/aq_geometric/data/graph/edges/compute_edges.py` & `aq_geometric-2024.5.19.1/aq_geometric/data/graph/edges/compute_edges.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.5.1.2/aq_geometric/data/graph/nodes/compute_node_features.py` & `aq_geometric-2024.5.19.1/aq_geometric/data/graph/nodes/compute_node_features.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.5.1.2/aq_geometric/data/graph/nodes/compute_nodes.py` & `aq_geometric-2024.5.19.1/aq_geometric/data/graph/nodes/compute_nodes.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.5.1.2/aq_geometric/data/reindex/features.py` & `aq_geometric-2024.5.19.1/aq_geometric/data/reindex/features.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.5.1.2/aq_geometric/data/remote/psql.py` & `aq_geometric-2024.5.19.1/aq_geometric/data/remote/psql.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.5.1.2/aq_geometric/datasets/in_memory/aq_geometric_dataset.py` & `aq_geometric-2024.5.19.1/aq_geometric/datasets/in_memory/aq_geometric_dataset.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.5.1.2/aq_geometric/datasets/on_disk/aq_geometric_dataset.py` & `aq_geometric-2024.5.19.1/aq_geometric/datasets/on_disk/aq_geometric_dataset.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.5.1.2/aq_geometric/models/__init__.py` & `aq_geometric-2024.5.19.1/aq_geometric/models/__init__.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.5.1.2/aq_geometric/models/base_model.py` & `aq_geometric-2024.5.19.1/aq_geometric/models/base_model.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.5.1.2/aq_geometric/models/test_base_model.py` & `aq_geometric-2024.5.19.1/aq_geometric/models/test_base_model.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.5.1.2/aq_geometric/models/edge_conv/edge_conv.py` & `aq_geometric-2024.5.19.1/aq_geometric/models/edge_conv/edge_conv.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.5.1.2/aq_geometric/models/edge_conv/test_edge_conv.py` & `aq_geometric-2024.5.19.1/aq_geometric/models/edge_conv/test_edge_conv.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.5.1.2/aq_geometric/models/gcn/gcn.py` & `aq_geometric-2024.5.19.1/aq_geometric/models/gcn/gcn.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.5.1.2/aq_geometric/models/gcn/test_gcn.py` & `aq_geometric-2024.5.19.1/aq_geometric/models/gcn/test_gcn.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.5.1.2/aq_geometric/models/hierarchical_edge_conv/heirarchical_edge_conv.py` & `aq_geometric-2024.5.19.1/aq_geometric/models/hierarchical_edge_conv/heirarchical_edge_conv.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.5.1.2/aq_geometric/models/hierarchical_edge_conv/test_heirarchical_edge_conv.py` & `aq_geometric-2024.5.19.1/aq_geometric/models/hierarchical_edge_conv/test_heirarchical_edge_conv.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.5.1.2/aq_geometric/models/hierarchical_xgb/base_hierarchical_xgb.py` & `aq_geometric-2024.5.19.1/aq_geometric/models/hierarchical_xgb/base_hierarchical_xgb.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.5.1.2/aq_geometric/models/hierarchical_xgb/hierarchical_xgb_direct.py` & `aq_geometric-2024.5.19.1/aq_geometric/models/hierarchical_xgb/hierarchical_xgb_direct.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.5.1.2/aq_geometric/models/hierarchical_xgb/hierarchical_xgb_iterative.py` & `aq_geometric-2024.5.19.1/aq_geometric/models/hierarchical_xgb/hierarchical_xgb_iterative.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.5.1.2/aq_geometric/models/message_passing/message_passing.py` & `aq_geometric-2024.5.19.1/aq_geometric/models/message_passing/message_passing.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,15 +119,18 @@
         self.num_message_passing_steps = num_message_passing_steps
         self.embedding_dim = embedding_dim
         self.num_heads = num_heads
         self.verbose = verbose
        
         self.encoder = AqGeometricEncoder(self.num_samples_in_node_feature, self.num_features_in_node_feature, embedding_dim, num_heads)
         self.processor = AqGeometricProcessor(embedding_dim, num_message_passing_steps)
-        self.decoder = AqGeometricDecoder(embedding_dim, 1, self.num_features_in_node_target, (1, self.num_features_in_node_target))
+        if self.is_iterative:
+            self.decoder = AqGeometricDecoder(embedding_dim, 1, self.num_features_in_node_target, (1, self.num_features_in_node_target))
+        else:
+            self.decoder = AqGeometricDecoder(embedding_dim, self.num_samples_in_node_target, self.num_features_in_node_target, (self.num_samples_in_node_target, self.num_features_in_node_target))
 
     def forward(self, x, edge_index, x_mask):
         x, _ = self.encoder(x, x_mask)
         x = self.processor(x, edge_index)
         x = self.decoder(x)
 
         return x
@@ -268,20 +271,28 @@
         targets: Union[List[str], None] = None,
         include_history: bool = False,
         verbose: Union[List[str], None] = None,
     ) -> Tuple[Dict[str, pd.DataFrame], np.ndarray, List[np.ndarray]]:
         """
         Generate forecasts using the model provided
         """
-        return self._generate_forecasts_iterative(
-            graph=graph,
-            targets=targets if targets is not None else self.targets,
-            include_history=include_history,
-            verbose=verbose if verbose is not None else self.verbose
-        )
+        if self.is_iterative:
+            return self._generate_forecasts_iterative(
+                graph=graph,
+                targets=targets if targets is not None else self.targets,
+                include_history=include_history,
+                verbose=verbose if verbose is not None else self.verbose
+            )
+        else:
+            return self._generate_forecasts_direct(
+                graph=graph,
+                targets=targets if targets is not None else self.targets,
+                include_history=include_history,
+                verbose=verbose if verbose is not None else self.verbose
+            )
 
     def _generate_forecasts_iterative(
         self,
         graph: "Data",
         targets: Union[List[str], None] = None,
         include_history: bool = False,
         verbose: Union[List[str], None] = None,
```

### Comparing `aq_geometric-2024.5.1.2/aq_geometric/models/statistical_baselines/climatology/climatology.py` & `aq_geometric-2024.5.19.1/aq_geometric/models/statistical_baselines/climatology/climatology.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.5.1.2/aq_geometric/models/statistical_baselines/linear/linear.py` & `aq_geometric-2024.5.19.1/aq_geometric/models/statistical_baselines/linear/linear.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.5.1.2/aq_geometric/models/statistical_baselines/persistance/persistance.py` & `aq_geometric-2024.5.19.1/aq_geometric/models/statistical_baselines/persistance/persistance.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.5.1.2/aq_geometric/models/statistical_baselines/temporal/temporal.py` & `aq_geometric-2024.5.19.1/aq_geometric/models/statistical_baselines/temporal/temporal.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.5.1.2/aq_geometric/transforms/change.py` & `aq_geometric-2024.5.19.1/aq_geometric/transforms/change.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.5.1.2/aq_geometric/utils/evaluation.py` & `aq_geometric-2024.5.19.1/aq_geometric/utils/evaluation.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.5.1.2/aq_geometric/utils/forecasts.py` & `aq_geometric-2024.5.19.1/aq_geometric/utils/forecasts.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.5.1.2/aq_geometric/utils/station_filters.py` & `aq_geometric-2024.5.19.1/aq_geometric/utils/station_filters.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.5.1.2/aq_geometric/utils/test_evaluation.py` & `aq_geometric-2024.5.19.1/aq_geometric/utils/test_evaluation.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.5.1.2/aq_geometric/utils/test_forecasts.py` & `aq_geometric-2024.5.19.1/aq_geometric/utils/test_forecasts.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.5.1.2/aq_geometric/utils/test_station_filters.py` & `aq_geometric-2024.5.19.1/aq_geometric/utils/test_station_filters.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.5.1.2/tests/data/test_aq.py` & `aq_geometric-2024.5.19.1/tests/data/test_aq.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.5.1.2/tests/datasets/test_aq.py` & `aq_geometric-2024.5.19.1/tests/datasets/test_aq.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.5.1.2/.gitignore` & `aq_geometric-2024.5.19.1/.gitignore`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.5.1.2/LICENSE.md` & `aq_geometric-2024.5.19.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.5.1.2/pyproject.toml` & `aq_geometric-2024.5.19.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name="aq-geometric"
-version="2024.05.01.2"
+version="2024.05.19.1"
 authors=[
     {name="Chris Jellen", email="cdjellen@gmail.com"},
 ]
 description="Geometric deep learning on air quality data."
 readme="README.md"
 requires-python=">=3.9"
 keywords=[
```

### Comparing `aq_geometric-2024.5.1.2/PKG-INFO` & `aq_geometric-2024.5.19.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: aq-geometric
-Version: 2024.5.1.2
+Version: 2024.5.19.1
 Summary: Geometric deep learning on air quality data.
 Project-URL: homepage, https://github.com/cdjellen/aq
 Project-URL: documentation, https://github.com/cdjellen/aq
 Author-email: Chris Jellen <cdjellen@gmail.com>
 License-File: LICENSE.md
 Keywords: deep-learning,earth-systems,geometric-deep-learning,pytorch
 Classifier: License :: OSI Approved :: MIT License
```

