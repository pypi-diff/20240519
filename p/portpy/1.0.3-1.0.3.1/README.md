# Comparing `tmp/portpy-1.0.3.tar.gz` & `tmp/portpy-1.0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\portpy-1.0.3.tar", last modified: Thu Jan  4 19:21:35 2024, max compression
+gzip compressed data, was "dist\portpy-1.0.3.1.tar", last modified: Sun May 19 12:57:34 2024, max compression
```

## Comparing `portpy-1.0.3.tar` & `portpy-1.0.3.1.tar`

### file list

```diff
@@ -1,79 +1,81 @@
-drwxrwxrwx   0        0        0        0 2024-01-04 19:21:35.000000 portpy-1.0.3/
--rw-rw-rw-   0        0        0      142 2023-06-13 16:08:24.000000 portpy-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0    16490 2024-01-04 19:21:35.000000 portpy-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0    14348 2023-11-27 15:31:50.000000 portpy-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-01-04 19:21:29.000000 portpy-1.0.3/images/
--rw-rw-rw-   0        0        0   184526 2023-05-12 05:53:35.000000 portpy-1.0.3/images/PortPy_logo.jpg
--rw-rw-rw-   0        0        0   179242 2023-07-20 15:30:39.000000 portpy-1.0.3/images/dose_comp.JPG
--rw-rw-rw-   0        0        0   161858 2023-07-20 15:59:20.000000 portpy-1.0.3/images/planner_vs_portpy_dvh.JPG
-drwxrwxrwx   0        0        0        0 2024-01-04 19:21:29.000000 portpy-1.0.3/portpy/
--rw-rw-rw-   0        0        0       52 2024-01-04 19:15:57.000000 portpy-1.0.3/portpy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-04 19:21:29.000000 portpy-1.0.3/portpy/ai/
--rw-rw-rw-   0        0        0        2 2023-07-21 17:36:30.000000 portpy-1.0.3/portpy/ai/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-04 19:21:29.000000 portpy-1.0.3/portpy/ai/data/
--rw-rw-rw-   0        0        0     3724 2023-07-21 19:16:53.000000 portpy-1.0.3/portpy/ai/data/__init__.py
--rw-rw-rw-   0        0        0     9475 2023-07-21 19:16:53.000000 portpy-1.0.3/portpy/ai/data/base_dataset.py
--rw-rw-rw-   0        0        0     3675 2023-07-21 19:16:53.000000 portpy-1.0.3/portpy/ai/data/dosepred3d_dataset.py
--rw-rw-rw-   0        0        0     2005 2023-07-21 19:16:53.000000 portpy-1.0.3/portpy/ai/data/image_folder.py
--rw-rw-rw-   0        0        0     2353 2023-07-21 19:16:53.000000 portpy-1.0.3/portpy/ai/data/single_dataset.py
--rw-rw-rw-   0        0        0     3583 2023-07-21 19:16:53.000000 portpy-1.0.3/portpy/ai/data/template_dataset.py
--rw-rw-rw-   0        0        0     4811 2023-07-17 14:00:42.000000 portpy-1.0.3/portpy/ai/example.py
-drwxrwxrwx   0        0        0        0 2024-01-04 19:21:29.000000 portpy-1.0.3/portpy/ai/models/
--rw-rw-rw-   0        0        0     3139 2023-07-21 19:16:52.000000 portpy-1.0.3/portpy/ai/models/__init__.py
--rw-rw-rw-   0        0        0    11391 2023-07-21 19:16:52.000000 portpy-1.0.3/portpy/ai/models/base_model.py
--rw-rw-rw-   0        0        0     7125 2023-07-21 19:16:52.000000 portpy-1.0.3/portpy/ai/models/doseprediction3d_model.py
--rw-rw-rw-   0        0        0    22899 2023-07-21 19:16:52.000000 portpy-1.0.3/portpy/ai/models/networks3d.py
--rw-rw-rw-   0        0        0     3490 2023-07-21 19:16:52.000000 portpy-1.0.3/portpy/ai/models/test_model.py
-drwxrwxrwx   0        0        0        0 2024-01-04 19:21:29.000000 portpy-1.0.3/portpy/ai/options/
--rw-rw-rw-   0        0        0     1838 2023-07-21 19:16:51.000000 portpy-1.0.3/portpy/ai/options/PyesapiTutorial.py
--rw-rw-rw-   0        0        0      137 2023-07-21 19:16:51.000000 portpy-1.0.3/portpy/ai/options/__init__.py
--rw-rw-rw-   0        0        0     8196 2023-07-21 19:16:52.000000 portpy-1.0.3/portpy/ai/options/base_options.py
--rw-rw-rw-   0        0        0     1181 2023-07-21 19:16:51.000000 portpy-1.0.3/portpy/ai/options/test_options.py
--rw-rw-rw-   0        0        0     3489 2023-07-21 19:16:51.000000 portpy-1.0.3/portpy/ai/options/train_options.py
--rw-rw-rw-   0        0        0     5048 2023-07-21 15:27:18.000000 portpy-1.0.3/portpy/ai/predict.py
--rw-rw-rw-   0        0        0     2238 2023-07-07 04:18:05.000000 portpy-1.0.3/portpy/ai/runRandomTrain.py
--rw-rw-rw-   0        0        0     4596 2023-07-21 19:16:53.000000 portpy-1.0.3/portpy/ai/test.py
--rw-rw-rw-   0        0        0     9041 2023-07-21 19:16:53.000000 portpy-1.0.3/portpy/ai/train.py
-drwxrwxrwx   0        0        0        0 2024-01-04 19:21:29.000000 portpy-1.0.3/portpy/ai/util/
--rw-rw-rw-   0        0        0       84 2023-07-21 19:16:52.000000 portpy-1.0.3/portpy/ai/util/__init__.py
--rw-rw-rw-   0        0        0     3633 2023-07-21 19:16:52.000000 portpy-1.0.3/portpy/ai/util/html.py
--rw-rw-rw-   0        0        0     2280 2023-07-21 19:16:52.000000 portpy-1.0.3/portpy/ai/util/image_pool.py
--rw-rw-rw-   0        0        0     4683 2023-07-21 19:16:52.000000 portpy-1.0.3/portpy/ai/util/util.py
--rw-rw-rw-   0        0        0    10211 2023-07-21 19:16:52.000000 portpy-1.0.3/portpy/ai/util/visualizer.py
-drwxrwxrwx   0        0        0        0 2024-01-04 19:21:29.000000 portpy-1.0.3/portpy/config_files/
--rw-rw-rw-   0        0        0        0 2023-06-13 16:25:21.000000 portpy-1.0.3/portpy/config_files/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-04 19:21:29.000000 portpy-1.0.3/portpy/config_files/clinical_criteria/
-drwxrwxrwx   0        0        0        0 2024-01-04 19:21:29.000000 portpy-1.0.3/portpy/config_files/clinical_criteria/Default/
--rw-rw-rw-   0        0        0     3372 2023-11-21 14:43:11.000000 portpy-1.0.3/portpy/config_files/clinical_criteria/Default/Lung_2Gy_30Fx.json
-drwxrwxrwx   0        0        0        0 2024-01-04 19:21:29.000000 portpy-1.0.3/portpy/config_files/optimization_params/
--rw-rw-rw-   0        0        0     2815 2023-11-24 11:52:14.000000 portpy-1.0.3/portpy/config_files/optimization_params/optimization_params_Lung_2Gy_30Fx.json
-drwxrwxrwx   0        0        0        0 2024-01-04 19:21:29.000000 portpy-1.0.3/portpy/photon/
--rw-rw-rw-   0        0        0      395 2023-06-12 21:08:08.000000 portpy-1.0.3/portpy/photon/__init__.py
--rw-rw-rw-   0        0        0     8347 2023-06-13 17:33:26.000000 portpy-1.0.3/portpy/photon/beam.py
--rw-rw-rw-   0        0        0     5417 2023-11-24 14:56:31.000000 portpy-1.0.3/portpy/photon/clinical_criteria.py
--rw-rw-rw-   0        0        0      702 2023-06-13 15:15:28.000000 portpy-1.0.3/portpy/photon/ct.py
--rw-rw-rw-   0        0        0    25077 2023-07-20 03:11:35.000000 portpy-1.0.3/portpy/photon/data_explorer.py
--rw-rw-rw-   0        0        0    20413 2023-11-24 11:50:01.000000 portpy-1.0.3/portpy/photon/evaluation.py
--rw-rw-rw-   0        0        0    50522 2024-01-04 19:08:35.000000 portpy-1.0.3/portpy/photon/influence_matrix.py
--rw-rw-rw-   0        0        0    29430 2023-11-27 15:27:10.000000 portpy-1.0.3/portpy/photon/optimization.py
--rw-rw-rw-   0        0        0     5806 2023-06-13 15:50:40.000000 portpy-1.0.3/portpy/photon/plan.py
--rw-rw-rw-   0        0        0    22381 2023-11-27 15:34:35.000000 portpy-1.0.3/portpy/photon/structures.py
-drwxrwxrwx   0        0        0        0 2024-01-04 19:21:29.000000 portpy-1.0.3/portpy/photon/utils/
--rw-rw-rw-   0        0        0      454 2023-08-30 02:17:56.000000 portpy-1.0.3/portpy/photon/utils/__init__.py
--rw-rw-rw-   0        0        0     2926 2023-09-29 19:20:32.000000 portpy-1.0.3/portpy/photon/utils/convert_dose_rt_dicom_to_portpy.py
--rw-rw-rw-   0        0        0     2543 2023-07-20 00:45:55.000000 portpy-1.0.3/portpy/photon/utils/get_eclipse_fluence.py
--rw-rw-rw-   0        0        0     8852 2023-08-30 02:17:55.000000 portpy-1.0.3/portpy/photon/utils/leaf_sequencing_siochi.py
--rw-rw-rw-   0        0        0     2846 2023-05-15 12:19:37.000000 portpy-1.0.3/portpy/photon/utils/save_nrrd.py
--rw-rw-rw-   0        0        0     4887 2023-05-15 11:43:22.000000 portpy-1.0.3/portpy/photon/utils/save_or_load_pickle.py
--rw-rw-rw-   0        0        0     1387 2023-05-09 07:09:19.000000 portpy-1.0.3/portpy/photon/utils/slicer_script.py
--rw-rw-rw-   0        0        0     4188 2023-06-12 16:42:02.000000 portpy-1.0.3/portpy/photon/utils/view_in_slicer_jupyter.py
--rw-rw-rw-   0        0        0     3604 2023-08-30 02:17:55.000000 portpy-1.0.3/portpy/photon/utils/write_rt_plan_imrt.py
--rw-rw-rw-   0        0        0    24680 2023-11-24 11:51:19.000000 portpy-1.0.3/portpy/photon/visualization.py
-drwxrwxrwx   0        0        0        0 2024-01-04 19:21:29.000000 portpy-1.0.3/portpy.egg-info/
--rw-rw-rw-   0        0        0    16490 2024-01-04 19:21:22.000000 portpy-1.0.3/portpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1924 2024-01-04 19:21:22.000000 portpy-1.0.3/portpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-04 19:21:22.000000 portpy-1.0.3/portpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      367 2024-01-04 19:21:22.000000 portpy-1.0.3/portpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-01-04 19:21:22.000000 portpy-1.0.3/portpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-01-04 19:21:35.000000 portpy-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     2529 2023-06-30 17:21:11.000000 portpy-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 12:57:34.000000 portpy-1.0.3.1/
+-rw-rw-rw-   0        0        0      142 2023-06-13 16:08:24.000000 portpy-1.0.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    21230 2024-05-19 12:57:34.000000 portpy-1.0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0    18430 2024-02-28 22:15:21.000000 portpy-1.0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-19 12:57:27.000000 portpy-1.0.3.1/images/
+-rw-rw-rw-   0        0        0    94149 2024-02-28 21:30:18.000000 portpy-1.0.3.1/images/PortPy-full-pipeline.jpg
+-rw-rw-rw-   0        0        0   184526 2023-05-12 05:53:35.000000 portpy-1.0.3.1/images/PortPy_logo.jpg
+-rw-rw-rw-   0        0        0   179242 2023-07-20 15:30:39.000000 portpy-1.0.3.1/images/dose_comp.JPG
+-rw-rw-rw-   0        0        0   161858 2023-07-20 15:59:20.000000 portpy-1.0.3.1/images/planner_vs_portpy_dvh.JPG
+drwxrwxrwx   0        0        0        0 2024-05-19 12:57:27.000000 portpy-1.0.3.1/portpy/
+-rw-rw-rw-   0        0        0       54 2024-05-19 12:47:45.000000 portpy-1.0.3.1/portpy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 12:57:28.000000 portpy-1.0.3.1/portpy/ai/
+-rw-rw-rw-   0        0        0        2 2023-07-21 17:36:30.000000 portpy-1.0.3.1/portpy/ai/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 12:57:29.000000 portpy-1.0.3.1/portpy/ai/data/
+-rw-rw-rw-   0        0        0     3724 2023-07-21 19:16:53.000000 portpy-1.0.3.1/portpy/ai/data/__init__.py
+-rw-rw-rw-   0        0        0     9475 2023-07-21 19:16:53.000000 portpy-1.0.3.1/portpy/ai/data/base_dataset.py
+-rw-rw-rw-   0        0        0     3675 2023-07-21 19:16:53.000000 portpy-1.0.3.1/portpy/ai/data/dosepred3d_dataset.py
+-rw-rw-rw-   0        0        0     2005 2023-07-21 19:16:53.000000 portpy-1.0.3.1/portpy/ai/data/image_folder.py
+-rw-rw-rw-   0        0        0     2353 2023-07-21 19:16:53.000000 portpy-1.0.3.1/portpy/ai/data/single_dataset.py
+-rw-rw-rw-   0        0        0     3583 2023-07-21 19:16:53.000000 portpy-1.0.3.1/portpy/ai/data/template_dataset.py
+-rw-rw-rw-   0        0        0     4811 2023-07-17 14:00:42.000000 portpy-1.0.3.1/portpy/ai/example.py
+drwxrwxrwx   0        0        0        0 2024-05-19 12:57:29.000000 portpy-1.0.3.1/portpy/ai/models/
+-rw-rw-rw-   0        0        0     3139 2023-07-21 19:16:52.000000 portpy-1.0.3.1/portpy/ai/models/__init__.py
+-rw-rw-rw-   0        0        0    11391 2023-07-21 19:16:52.000000 portpy-1.0.3.1/portpy/ai/models/base_model.py
+-rw-rw-rw-   0        0        0     7125 2023-07-21 19:16:52.000000 portpy-1.0.3.1/portpy/ai/models/doseprediction3d_model.py
+-rw-rw-rw-   0        0        0    22899 2023-07-21 19:16:52.000000 portpy-1.0.3.1/portpy/ai/models/networks3d.py
+-rw-rw-rw-   0        0        0     3490 2023-07-21 19:16:52.000000 portpy-1.0.3.1/portpy/ai/models/test_model.py
+drwxrwxrwx   0        0        0        0 2024-05-19 12:57:30.000000 portpy-1.0.3.1/portpy/ai/options/
+-rw-rw-rw-   0        0        0     1838 2023-07-21 19:16:51.000000 portpy-1.0.3.1/portpy/ai/options/PyesapiTutorial.py
+-rw-rw-rw-   0        0        0      137 2023-07-21 19:16:51.000000 portpy-1.0.3.1/portpy/ai/options/__init__.py
+-rw-rw-rw-   0        0        0     8196 2023-07-21 19:16:52.000000 portpy-1.0.3.1/portpy/ai/options/base_options.py
+-rw-rw-rw-   0        0        0     1181 2023-07-21 19:16:51.000000 portpy-1.0.3.1/portpy/ai/options/test_options.py
+-rw-rw-rw-   0        0        0     3489 2023-07-21 19:16:51.000000 portpy-1.0.3.1/portpy/ai/options/train_options.py
+-rw-rw-rw-   0        0        0     5048 2023-07-21 15:27:18.000000 portpy-1.0.3.1/portpy/ai/predict.py
+-rw-rw-rw-   0        0        0     2238 2023-07-07 04:18:05.000000 portpy-1.0.3.1/portpy/ai/runRandomTrain.py
+-rw-rw-rw-   0        0        0     4596 2023-07-21 19:16:53.000000 portpy-1.0.3.1/portpy/ai/test.py
+-rw-rw-rw-   0        0        0     9041 2023-07-21 19:16:53.000000 portpy-1.0.3.1/portpy/ai/train.py
+drwxrwxrwx   0        0        0        0 2024-05-19 12:57:31.000000 portpy-1.0.3.1/portpy/ai/util/
+-rw-rw-rw-   0        0        0       84 2023-07-21 19:16:52.000000 portpy-1.0.3.1/portpy/ai/util/__init__.py
+-rw-rw-rw-   0        0        0     3633 2023-07-21 19:16:52.000000 portpy-1.0.3.1/portpy/ai/util/html.py
+-rw-rw-rw-   0        0        0     2280 2023-07-21 19:16:52.000000 portpy-1.0.3.1/portpy/ai/util/image_pool.py
+-rw-rw-rw-   0        0        0     4683 2023-07-21 19:16:52.000000 portpy-1.0.3.1/portpy/ai/util/util.py
+-rw-rw-rw-   0        0        0    10211 2023-07-21 19:16:52.000000 portpy-1.0.3.1/portpy/ai/util/visualizer.py
+drwxrwxrwx   0        0        0        0 2024-05-19 12:57:31.000000 portpy-1.0.3.1/portpy/config_files/
+-rw-rw-rw-   0        0        0        0 2023-06-13 16:25:21.000000 portpy-1.0.3.1/portpy/config_files/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 12:57:26.000000 portpy-1.0.3.1/portpy/config_files/clinical_criteria/
+drwxrwxrwx   0        0        0        0 2024-05-19 12:57:31.000000 portpy-1.0.3.1/portpy/config_files/clinical_criteria/Default/
+-rw-rw-rw-   0        0        0     3922 2024-05-19 12:27:55.000000 portpy-1.0.3.1/portpy/config_files/clinical_criteria/Default/HN_1Gy_1Fx.json
+-rw-rw-rw-   0        0        0     3372 2024-03-25 18:12:20.000000 portpy-1.0.3.1/portpy/config_files/clinical_criteria/Default/Lung_2Gy_30Fx.json
+drwxrwxrwx   0        0        0        0 2024-05-19 12:57:26.000000 portpy-1.0.3.1/portpy/config_files/optimization_params/
+-rw-rw-rw-   0        0        0     2815 2023-11-24 11:52:14.000000 portpy-1.0.3.1/portpy/config_files/optimization_params/optimization_params_Lung_2Gy_30Fx.json
+drwxrwxrwx   0        0        0        0 2024-05-19 12:57:33.000000 portpy-1.0.3.1/portpy/photon/
+-rw-rw-rw-   0        0        0      395 2024-05-19 12:18:24.000000 portpy-1.0.3.1/portpy/photon/__init__.py
+-rw-rw-rw-   0        0        0     8347 2024-05-19 12:18:24.000000 portpy-1.0.3.1/portpy/photon/beam.py
+-rw-rw-rw-   0        0        0     5417 2024-05-19 12:18:25.000000 portpy-1.0.3.1/portpy/photon/clinical_criteria.py
+-rw-rw-rw-   0        0        0      702 2023-06-13 15:15:28.000000 portpy-1.0.3.1/portpy/photon/ct.py
+-rw-rw-rw-   0        0        0    25077 2023-07-20 03:11:35.000000 portpy-1.0.3.1/portpy/photon/data_explorer.py
+-rw-rw-rw-   0        0        0    20413 2024-05-19 12:18:25.000000 portpy-1.0.3.1/portpy/photon/evaluation.py
+-rw-rw-rw-   0        0        0    50525 2024-05-19 12:23:26.000000 portpy-1.0.3.1/portpy/photon/influence_matrix.py
+-rw-rw-rw-   0        0        0    29430 2024-05-19 12:18:25.000000 portpy-1.0.3.1/portpy/photon/optimization.py
+-rw-rw-rw-   0        0        0     5806 2024-05-19 12:18:25.000000 portpy-1.0.3.1/portpy/photon/plan.py
+-rw-rw-rw-   0        0        0    23395 2024-05-19 12:36:34.000000 portpy-1.0.3.1/portpy/photon/structures.py
+drwxrwxrwx   0        0        0        0 2024-05-19 12:57:34.000000 portpy-1.0.3.1/portpy/photon/utils/
+-rw-rw-rw-   0        0        0      454 2023-08-30 02:17:56.000000 portpy-1.0.3.1/portpy/photon/utils/__init__.py
+-rw-rw-rw-   0        0        0     2926 2023-09-29 19:20:32.000000 portpy-1.0.3.1/portpy/photon/utils/convert_dose_rt_dicom_to_portpy.py
+-rw-rw-rw-   0        0        0     2543 2024-05-19 12:18:26.000000 portpy-1.0.3.1/portpy/photon/utils/get_eclipse_fluence.py
+-rw-rw-rw-   0        0        0     8852 2023-08-30 02:17:55.000000 portpy-1.0.3.1/portpy/photon/utils/leaf_sequencing_siochi.py
+-rw-rw-rw-   0        0        0     2846 2023-05-15 12:19:37.000000 portpy-1.0.3.1/portpy/photon/utils/save_nrrd.py
+-rw-rw-rw-   0        0        0     4887 2024-05-19 12:18:26.000000 portpy-1.0.3.1/portpy/photon/utils/save_or_load_pickle.py
+-rw-rw-rw-   0        0        0     1387 2023-05-09 07:09:19.000000 portpy-1.0.3.1/portpy/photon/utils/slicer_script.py
+-rw-rw-rw-   0        0        0     4188 2023-06-12 16:42:02.000000 portpy-1.0.3.1/portpy/photon/utils/view_in_slicer_jupyter.py
+-rw-rw-rw-   0        0        0     3604 2023-08-30 02:17:55.000000 portpy-1.0.3.1/portpy/photon/utils/write_rt_plan_imrt.py
+-rw-rw-rw-   0        0        0    24680 2023-11-24 11:51:19.000000 portpy-1.0.3.1/portpy/photon/visualization.py
+drwxrwxrwx   0        0        0        0 2024-05-19 12:57:27.000000 portpy-1.0.3.1/portpy.egg-info/
+-rw-rw-rw-   0        0        0    21230 2024-05-19 12:57:09.000000 portpy-1.0.3.1/portpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2018 2024-05-19 12:57:10.000000 portpy-1.0.3.1/portpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 12:57:09.000000 portpy-1.0.3.1/portpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      367 2024-05-19 12:57:10.000000 portpy-1.0.3.1/portpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-19 12:57:10.000000 portpy-1.0.3.1/portpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-19 12:57:34.000000 portpy-1.0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     2547 2024-05-19 12:54:10.000000 portpy-1.0.3.1/setup.py
```

### Comparing `portpy-1.0.3/PKG-INFO` & `portpy-1.0.3.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,156 +1,217 @@
-Metadata-Version: 2.1
-Name: portpy
-Version: 1.0.3
-Summary: First open-source radiation treatment planning system in Python
-Home-page: https://github.com/PortPy-Project/PortPy
-Author: Gourav Jhanwar, Mojtaba Tefagh, Vicki Taasti, Seppo Tuomaala, Saad Nadeem, Masoud Zarepisheh
-Author-email: jhanwarg@mskcc.struct, mtefagh@acm.struct, vicki.taasti@maastro.nl, tuomaals@mskcc.struct, nadeems@mskcc.struct, zarepism@mskcc.struct
-License: Apache License, Version 2.0
-Description: <p align="center">
-          <img src="./images/PortPy_logo.png" width="40%" height="40%">
-        </p>
-        
-        ![Version](https://img.shields.io/static/v1?label=latest&message=v1.0.2&color=darkgreen)
-        [![Total Downloads](https://static.pepy.tech/personalized-badge/portpy?period=total&units=international_system&left_color=grey&right_color=blue&left_text=total%20downloads)](https://pepy.tech/project/portpy?&left_text=totalusers)
-        
-        # What is PortPy?
-        
-        PortPy, short for **P**lanning and **O**ptimization for **R**adiation **T**herapy, represents a collective effort to establish an open-source Python library dedicated to advancing the development and clinical implementation of cancer radiotherapy treatment planning algorithms. This initiative encompasses planning methodologies for Intensity Modulated Radiation Therapy (IMRT), Volumetric Modulated Arc Therapy (VMAT), along with other emerging modalities. PortPy provides clinical-grade data and coding resources that foster *benchmarking*, *reproducibility*, and *community development*.
-        
-        
-        **Contents**
-        - [What can you do with PortPy?](#WhatDo)
-        - [Quick Start](#QuickStart)
-        - [How to contribute?](#limitations)
-        - [The limitations of current version](#limitations)
-        - [Data](#Data)
-        - [Installation](#Installation)
-        - [Team](#Team)
-        
-        
-        
-        
-        # What can you do with PortPy? <a name="WhatDo"></a>
-        PortPy facilitates the **design**, **testing**, and **clinical validation** of your treatment planning algorithms. This includes both cutting-edge AI-based models and traditional optimization techniques. PortPy provides:
-        1. **Benchmark Dataset**
-             * Access to data required for optimization, extracted directly from the FDA-approved Eclipse treatment planning system via its API 
-             * A current set of data from 50 lung patients, which will be expanded to 100 lung patients by the end of 2023
-             * A **benchmark IMRT plan** for each patient, created using our in-house automated planning system ([Edelman Award Finalist YouTube Video](https://youtu.be/895M6j5KjPs), [Paper](https://aapm.onlinelibrary.wiley.com/doi/epdf/10.1002/mp.13572))
-           
-        2. **Benchmark Algorithms:** Offering globally optimal solutions for:
-             * Dose Volume Histogram (DVH) constraints (see [dvh_constraint_optimization.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/benchmark_algorithms/dvh_constraint_optimization.ipynb))
-             * IMRT Beam Orientation Optimization (BOO) (see [beam_orientation_optimization.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/benchmark_algorithms/beam_orientation_optimization.ipynb))
-             * Volumetric Modulated Arc Therapy (VMAT) (see [vmat_optimization.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/benchmark_algorithms/vmat_optimization.ipynb))
-        4. **Visualization**
-             * Basic built-in visualization tools (e.g., DVH, dose distribution) are integrated into PortPy (see (see [basic_tutorial.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/1_basic_tutorial.ipynb)))
-             * Enhanced visualizations are available through the integration with the popular open-source [3DSlicer](https://www.slicer.org/) package (see [3d_slicer_integration.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/3d_slicer_integration.ipynb))
-        5. **Evaluation**  
-             * PortPy IMRT plans with optimal fluence can be imported into Eclipse for leaf sequencing and final clinical evaluations  (see [eclipse_integration.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/eclipse_integration.ipynb))
-             * PortPy IMRT/VMAT plans can be imported into FDA approved TPS( e.g. Eclipse, Raystation) using DICOM RT Plan file for final clinical evaluations  (see [TPS-integration.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/TPS-Integration.ipynb))
-             * Plans can also be evaluated within PortPy using well-established clinical protocols (e.g., Lung 2Gyx30, see  [basic_tutorial.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/1_basic_tutorial.ipynb))
-             * Future updates will include more standardized RTOG metrics and outcome models (TCP/NTCP)
-        6. **Optimization** 
-             * PortPy provides high-level optimization problem formulation and access to both free and commercial optimization engines through the integration with a popular open-source [CVXPy](https://www.cvxpy.org/) package (see [basic_tutorial.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/1_basic_tutorial.ipynb))
-             * Commercial engines (e.g., [MOSEK](https://www.mosek.com/), [CPLEX](https://www.ibm.com/products/ilog-cplex-optimization-studio/cplex-optimizer), [GUROBI](https://www.gurobi.com/)) are also free for academic and research use
-        7. **AI-Based Planning** 
-             * The PortPy.AI module provides a framework for exploring AI-driven treatment planning  (see [dose_prediction_pipeline.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/AI_tutorials/dose_prediction_pipeline.ipynb))
-             * The newly added PortPy.AI module includes a tutorial on predicting a 3D-dose distribution and converting the prediction into a deliverable plan
-        
-        # Quick Start <a name="QuickStart"></a>
-        
-        1. To grasp the primary features of PortPy, we highly recommend exploring the [basic_tutorial.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/1_basic_tutorial.ipynb) notebook
-        2. To understand how to import a PortPy plan into Eclipse for final evaluations, browse through the [eclipse_integration.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/eclipse_integration.ipynb) notebook
-        3. To create dicom RT Plan file from PortPy plan and import into FDA approved commercial TPS (e.g. Eclipse, Raystation), please browse through [TPS-integration.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/TPS-Integration.ipynb) notebook
-        4. To learn about enhanced visualization techniques using the 3D-Slicer package, refer to the  [3d_slicer_integration.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/3d_slicer_integration.ipynb) notebook
-        5. For algorithm benchmarking, the global optimal solutions are provided for non-convex optimization problems resulting from beam angle optimization [beam_orientation_optimization.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/benchmark_algorithms/beam_orientation_optimization.ipynb), incorporating DVH constraints [dvh_constraint_optimization.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/benchmark_algorithms/dvh_constraint_optimization.ipynb), and VMAT optimization [vmat_optimization.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/benchmark_algorithms/vmat_optimization.ipynb) using the mixed-integer programming on down-sampled data.
-        6. If you encounter computational challenges with large-scale optimization problems, you can opt for down-sampling the voxels/beamlets, as illustrated in the [down_sampling](https://github.com/PortPy-Project/PortPy/blob/master/examples/advanced_tutorials/down_sampling.ipynb) notebook, or further sparsify the influence matrix, as demonstrated in the [inf_matrix_sparsification](https://github.com/PortPy-Project/PortPy/blob/master/examples/advanced_tutorials/inf_matrix_sparsification.ipynb) notebook.
-        7. To learn about creating a final deliverable plan using AI based model, please refer to [dose_prediction_pipeline.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/AI_tutorials/dose_prediction_pipeline.ipynb) notebook.
-        
-        # How to contribute? <a name="HowContribute"></a>
-        To maintain the lightweight nature and user-friendliness of PortPy modules, our aim is to include only fundamental functionalities, along with benchmark data and algorithms. We will establish separate repositories within the [PortPy-Project orgainization](https://github.com/PortPy-Project) for projects developed by our team using PortPy as a platform. This is similar to what we've done for projects like [LowDimRT](https://github.com/PortPy-Project/LowDimRT) and [VMAT](https://github.com/PortPy-Project/ECHO-VMAT).
-        
-        If you're interested in contributing to existing PortPy modules or wish to create a new module, we encourage you to contact us first. This will help ensure that our objectives and priorities are aligned. If you use PortPy to build your own package, you're welcome to host your package within the [PortPy-Project orgainization](https://github.com/PortPy-Project). Alternatively, you can host your package on your own GitHub page. In this case, please inform us so that we can fork it and feature it under the PortPy-Project organization.
-        
-        
-        # The limitations of current version of PortPy <a name="limitations"></a>
-        Current version of PortPy has the following limitations which would be addressed in the future updates:
-        
-        1. You can only work with the benchmark dataset provided in this PortPy repo and cannot use your own dataset for now.
-        2. PortPy.Photon and PortPy.AI are the only modules available. You cannot do proton research with the current version. Please use [OpenTPS](http://opentps.org/) for proton research.
-        
-        # Data <a name="Data"></a>
-        
-        PortPy equips researchers with a robust benchmark patient dataset, sourced from the FDA-approved Eclipse commercial treatment planning system through its API. This dataset embodies all necessary elements for optimizing various machine configurations such as beam angles, aperture shapes, and leaf movements. It includes
-        
-        1. **Dose Influence Matrix:** The dose contribution of each beamlet to each voxel,
-        2. **Beamlets/Voxels Details:** Detailed information about the position and size of beamlets/voxels,
-        3. **Expert-Selected Benchmark Beams:** An expert clinical physicist has carefully selected benchmark beams, providing reference beams for comparison and benchmarking,
-        4. **Benchmark IMRT Plan:** A benchmark IMRT plan generated using our in-house automated treatment planning system called ECHO ([Edelman Award Finalist YouTube Video](https://youtu.be/895M6j5KjPs), [Paper](https://aapm.onlinelibrary.wiley.com/doi/epdf/10.1002/mp.13572)). This plan serves as a benchmark for evaluating new treatment planning algorithms.
-        
-        To access these resources, users are advised to download the latest version of the dataset, which can be found [here](https://drive.google.com/drive/folders/1nA1oHEhlmh2Hk8an9e0Oi0ye6LRPREit?usp=sharing). Subsequently, create a directory titled './data' in the current project directory and transfer the downloaded file into it. For example, ./data/Lung_Phantom_Patient_1.
-        
-        
-        
-        **Note:** Initially, we will utilize a lung dataset from [TCIA](https://wiki.cancerimagingarchive.net/display/Public/NSCLC-Radiomics). The original DICOM CT images and structure sets are not included in the PortPy dataset and need to be directly downloaded from the TCIA. Users can fetch the **TCIA collection ID** and the **TCIA subject ID** for each PortPy patient using the *get_tcia_metadata()* method in PortPy and subsequently download the data from TCIA (see [eclipse_integration.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/eclipse_integration.ipynb))
-        
-        
-        # Installation <a name="Installation"></a>
-        
-        1. Install using pip:
-           
-            * Run the command '**pip install portpy**'
-        
-        2. Install using conda:
-        
-            * Run the command '**conda install -c conda-forge portpy**'
-        
-        3. Install from source:
-           
-            * Clone this repository using '**git clone https://github.com/PortPy-Project/PortPy.git**'
-            * Navigate to the repository with '**cd portpy**'
-        
-            * Install the dependencies within a Python virtual environment or Anaconda environment. To set up in a Python virtual environment, install all the dependencies specified in requirements.txt as follows:
-                * Create the virtual environment with '**python3 -m venv venv**'
-                * Activate the environment with '**source venv/bin/activate**'
-                * Install the requirements using '**(venv) pip install -r requirements.txt**'
-        
-        
-        # Team <a name="Team"></a>
-        PortPy is a community project initiated at [Memorial Sloan Kettering Cancer Center](https://www.mskcc.org/). It is currently developed and maintained by:
-        
-        | Name                                                                         | Expertise                                        | Institution |
-        |------------------------------------------------------------------------------|--------------------------------------------------|-------------|
-        | [Masoud Zarepisheh](https://masoudzp.github.io/)                             | Treatment Planning and Optimization              | MSK         |
-        | [Saad Nadeem](https://nadeemlab.org/)                                        | Computer Vision and AI in Medical Imaging        | MSK         |
-        | [Gourav Jhanwar](https://github.com/gourav3017)                              | Algorithm Design and Development                 | MSK         |
-        | [Mojtaba Tefagh](https://github.com/mtefagh)                                 | Mathematical Modeling and Reinforcement Learning | SUT         |
-        | [Vicki Taasti](https://scholar.google.com/citations?user=PEPyvewAAAAJ&hl=en) | Physics and Planning of Proton Therapy           | MAASTRO     |
-        | [Sadegh Alam](https://scholar.google.com/citations?user=iy7TlU0AAAAJ&hl=en)  | Adaptive Treatment Planning and Imaging          | Cornell     |
-        | [Seppo Tuomaala](https://www.linkedin.com/in/seppo-tuomaala-5b57913/)        | Eclispe API Scripting                            | VARIAN      |
-        
-        # License <a name="License"></a>
-        PortPy code is distributed under **Apache 2.0 with Commons Clause** license, and is available for non-commercial academic purposes.
-        
-        # Reference <a name="Reference"></a>
-        If you find our work useful in your research or if you use parts of this code please cite our [AAPM'23 abstract](https://aapm.confex.com/aapm/2023am/meetingapp.cgi/Paper/4208) :
-        ```
-        @article{jhanwar2023portpy,
-          title={Portpy: An Open-Source Python Package for Planning and Optimization in Radiation Therapy Including Benchmark Data and Algorithms},
-          author={Jhanwar, Gourav and Tefagh, Mojtaba and Taasti, Vicki T and Alam, Sadegh R and Tuomaala, Seppo and Nadeem, Saad and Zarepisheh, Masoud},
-          journal={AAPM 65th Annual Meeting & Exhibition},
-          year={2023}
-        }
-        ```
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 1 - Planning
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
+<p align="center">
+  <img src="./images/PortPy_logo.png" width="40%" height="40%">
+</p>
+
+![Version](https://img.shields.io/static/v1?label=latest&message=v1.0.3&color=darkgreen)
+[![Total Downloads](https://static.pepy.tech/personalized-badge/portpy?period=total&units=international_system&left_color=grey&right_color=blue&left_text=total%20downloads)](https://pepy.tech/project/portpy?&left_text=totalusers)
+
+# What is PortPy?
+
+PortPy, short for **P**lanning and **O**ptimization for **R**adiation **T**herapy, represents a collective effort 
+to establish an open-source Python library dedicated to advancing the development and clinical implementation of 
+cancer radiotherapy treatment planning algorithms. This initiative encompasses planning methodologies for 
+Intensity Modulated Radiation Therapy (IMRT), Volumetric Modulated Arc Therapy (VMAT), along with other 
+emerging modalities. PortPy provides clinical-grade data and coding resources that foster *benchmarking*, 
+*reproducibility*, and *community development*.
+
+**Note:** In the near future, we plan to launch an educational YouTube channel to assist 
+researchers new to this field. Meanwhile, we suggest reviewing relevant literature review papers
+([Zarepisheh et al. 2021](https://pubsonline.informs.org/doi/abs/10.1287/inte.2021.1095), 
+[Breedveld et al. 2019](https://www.sciencedirect.com/science/article/abs/pii/S0377221718307148), 
+[Ehrgott et al. 2010](https://link.springer.com/article/10.1007/s10479-009-0659-4)) and watching YouTube videos 
+([Edelman competition](https://www.youtube.com/watch?v=895M6j5KjPs&t=1025s), [Varian IMRT](https://www.youtube.com/watch?v=eZS6DVGBx0k), [Elekta VMAT](https://www.youtube.com/watch?v=AE1SxvnFT3s)).
+  
+
+**Contents**
+- [Why we created PortPy?](#Why)
+- [What can you do with PortPy?](#WhatDo)
+- [Quick Start](#QuickStart)
+- [How to contribute?](#limitations)
+- [Data](#Data)
+- [Installation](#Installation)
+- [Team](#Team)
+
+# Why we created PortPy? <a name="Why"></a>
+
+<p align="center">
+  <img src="./images/PortPyIntegration.png" width="60%" height="40%">
+<p>
+
+
+A key limitation of existing open-source packages in radiotherapy treatment planning is their
+inability to objectively evaluate new treatment planning techniques against current clinical practices. 
+This limitation stems from the difficulty in fully replicating clinical environments, such as detailed 
+linear accelerator configurations and commercial dose calculation engines. Consequently,
+plans generated using novel techniques, such as AI-based automated treatment planning, cannot be objectively compared
+with clinical plans used in patient treatment. To address this limitation, we are integrating PortPy with 
+commercial treatment planning systems (TPSs). PortPy is already compatible with the [Varian Eclipse TPS](https://www.varian.com/), 
+and we plan to expand compatibility to additional TPSs in the future. It's crucial to note that PortPy can 
+be used independently of any TPS, but accessing a TPS is essential for final evaluation within the TPS (see above figure).
+<p align="center">
+  <img src="./images/AI_Pyramid.png" width="40%" height="40%">
+<p>
+
+Above figure highlights the inspiration for developing PortPy, drawing on successful open-source practices 
+from the AI and computer science communities. Tools like PyTorch and TensorFlow, along with benchmark datasets 
+such as ImageNet and algorithms like AlexNet, have transformed AI and data science. Our aim is to emulate 
+this success, providing researchers with comprehensive resources (PortPy integration with commercial TPS 
+and other renowned open-source tools such as [3DSlicer](https://www.slicer.org/) and [CVXPy](https://www.cvxpy.org/), a benchmark dataset 
+(featuring 50 curated lung patients with expertly selected beams, all necessary optimization data, 
+and benchmark IMRT plans created using our in-house automated planning system, ECHO), 
+and benchmark algorithms, including Mixed Integer Programming (MIP) algorithms for achieving globally optimal solutions.
+
+
+
+
+# What can you do with PortPy? <a name="WhatDo"></a>
+
+<p align="center">
+<img src="./images/PortPy-Workflow.png" width="90%" height="40%">
+<p>
+
+PortPy facilitates the **design**, **testing**, and **clinical validation** of new treatment planning algorithms. 
+This includes both cutting-edge AI-based models and traditional optimization techniques. 
+The above figure illustrates the PortPy design and its three main
+modules: “Data Management”, “Plan Generation”, and “Plan
+Evaluation”,  which are discussed below. We recommend reviewing our Jupyter Notebooks 
+examples for a more comprehensive understanding of these modules. 
+
+1. **Data Management**
+     * This module provides access to the curated benchmark PortPy dataset, which currently comprises data from 50 lung patients.
+It allows researchers to test and develop their algorithms using the same dataset (see [basic_tutorial.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/1_basic_tutorial.ipynb) notebook)
+     * The available data includes: 1) CT images and contours, 2) all necessary data for optimization extracted from 
+Eclipse using its API (version 16.1), 3)expert-selected beams for each patient, 4) an IMRT plan for each patient, 
+generated using our in-house automated planning system, 
+ECHO ([YouTube Video](https://youtu.be/895M6j5KjPs), [Paper](https://aapm.onlinelibrary.wiley.com/doi/epdf/10.1002/mp.13572)).
+More information about data can be found in [Data](#Data) section.
+     * In the current version, you can only work with the benchmark dataset provided in this PortPy repo and 
+   cannot use your own dataset for now. We will address this problem in the near future
+
+2. **Plan Generation**
+     * This module facilitates the generation of treatment plans using either classical optimization methods or 
+emerging AI-based techniques 
+     * For optimization tasks, PortPy has been integrated with [CVXPy](https://www.cvxpy.org/), a widely-used open-source package. 
+CVXPy enables the high-level formulation of optimization problems and offers out-of-the-box access to a range
+of free (e.g., [SCIP](https://www.scipopt.org/), [SCIPY](https://docs.scipy.org/doc/scipy/reference/optimize.html)) and commercial (e.g., [MOSEK](https://www.mosek.com/), [CPLEX](https://www.ibm.com/products/ilog-cplex-optimization-studio/cplex-optimizer), [GUROBI](https://www.gurobi.com/)) optimization engines (available for free for research
+purposes) (see [basic_tutorial.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/1_basic_tutorial.ipynb) notebook)
+     * PortPy.AI module is equipped with essential functionalities for AI-based planning. These include data access, 
+data pre-processing, model training and testing, and patient-specific 3D dose prediction 
+(see [dose_prediction_pipeline.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/AI_tutorials/dose_prediction_pipeline.ipynb) notebook)
+     * The availability of both optimization and AI-based planning modules within PortPy allows researchers 
+to not only compare these techniques but also explore their complementary aspects
+
+3. **Plan Visualization and Evaluation**
+     * Basic built-in visualization tools (e.g., DVH, dose distribution) are integrated into PortPy 
+     * Enhanced visualizations are available through the integration with the popular open-source [3DSlicer](https://www.slicer.org/) package (see [3d_slicer_integration.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/3d_slicer_integration.ipynb) notebook)
+     * PortPy IMRT plans with optimal fluence can be imported into Eclipse for leaf sequencing and final clinical evaluations  (see [eclipse_integration.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/eclipse_integration.ipynb))
+     * PortPy IMRT/VMAT plans with optimal control points can be imported into any FDA approved TPS ( e.g. Eclipse, Raystation) using DICOM RT Plan file for final clinical evaluations  (see [TPS-integration.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/TPS-Integration.ipynb)).
+It should be noted that some discrepancies are anticipated 
+with TPSs other than Eclipse, due to the fact that our current data are derived from Eclipse, and there 
+may exist variations in dose calculation methods between Eclipse and other TPSs. 
+     * Plans can also be evaluated within PortPy using well-established clinical protocols (e.g., Lung 2Gyx30, see  [basic_tutorial.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/1_basic_tutorial.ipynb))
+     * Future updates will include more standardized RTOG metrics and outcome models (TCP/NTCP)
+
+
+
+# Quick Start <a name="QuickStart"></a>
+
+1. To grasp the primary features of PortPy, we highly recommend exploring the [basic_tutorial.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/1_basic_tutorial.ipynb) notebook
+2. To understand how to import a PortPy plan into Eclipse for final evaluations, browse through the [eclipse_integration.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/eclipse_integration.ipynb) notebook
+3. To create dicom RT Plan file from PortPy plan and import into FDA approved commercial TPS (e.g. Eclipse, Raystation), please browse through [TPS-integration.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/TPS-Integration.ipynb) notebook
+4. To learn about enhanced visualization techniques using the 3D-Slicer package, refer to the  [3d_slicer_integration.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/3d_slicer_integration.ipynb) notebook
+5. For algorithm benchmarking, the global optimal solutions are provided for non-convex optimization problems resulting from beam angle optimization [beam_orientation_optimization.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/benchmark_algorithms/beam_orientation_optimization.ipynb), incorporating DVH constraints [dvh_constraint_optimization.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/benchmark_algorithms/dvh_constraint_optimization.ipynb), and VMAT optimization [vmat_optimization.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/benchmark_algorithms/vmat_optimization.ipynb) using the mixed-integer programming on down-sampled data.
+6. If you encounter computational challenges with large-scale optimization problems, you can opt for down-sampling the voxels/beamlets, as illustrated in the [down_sampling](https://github.com/PortPy-Project/PortPy/blob/master/examples/advanced_tutorials/down_sampling.ipynb) notebook, or further sparsify the influence matrix, as demonstrated in the [inf_matrix_sparsification](https://github.com/PortPy-Project/PortPy/blob/master/examples/advanced_tutorials/inf_matrix_sparsification.ipynb) notebook.
+7. To learn about creating a final deliverable plan using AI based model, please refer to [dose_prediction_pipeline.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/AI_tutorials/dose_prediction_pipeline.ipynb) notebook.
+
+# How to contribute? <a name="HowContribute"></a>
+<p align="center">
+<img src="./images/PortPy_Organization.png" width="90%" height="40%">
+<p>
+
+As illustrated in the above figure, PortPy organization includes "PortPy", which is the current repository, 
+and PortPy extensions, which are the repositories developed using the PortPy as a platform. 
+To maintain the lightweight nature and user-friendliness of PortPy modules, our aim is to include only fundamental 
+functionalities, along with benchmark data and algorithms in the PortPy repo, and establish separate repositories 
+for other projects, similar to what we've done for projects like [LowDimRT](https://github.com/PortPy-Project/LowDimRT)
+and [ECHO VMAT](https://github.com/PortPy-Project/ECHO-VMAT).
+
+If you're interested in contributing to existing PortPy modules or wish to create a new module, 
+we encourage you to contact us first. This will help ensure that our objectives and priorities are aligned. 
+If you use PortPy to build your own package, you're welcome to host your package within the
+[PortPy-Project orgainization](https://github.com/PortPy-Project). 
+Alternatively, you can host your package on your own GitHub page. In this case, 
+please inform us so that we can fork it and feature it under the PortPy-Project organization. 
+For those keen on creating a logo for their repository, we offer the option to customize our [pre-designed logo](https://www.canva.com/design/DAFxivHC0Js/YqZREdr26pmEsIgCeuU-iA/view?utm_content=DAFxivHC0Js&utm_campaign=designshare&utm_medium=link&utm_source=publishsharelink&mode=preview).
+
+
+# Data <a name="Data"></a>
+<p align="center">
+<img src="./images/PortPy Data.png" width="90%" height="40%">
+<p>
+PortPy equips researchers with a robust benchmark patient dataset, sourced from the FDA-approved Eclipse commercial treatment planning system through its API. This dataset embodies all necessary elements for optimizing various machine configurations such as beam angles, aperture shapes, and leaf movements. It includes
+
+1. **Dose Influence Matrix (AKA dose deposition matrix, dij matrix):** The dose contribution of each beamlet to each voxel,
+2. **Beamlets/Voxels Details:** Detailed information about the position and size of beamlets/voxels,
+3. **Expert-Selected Benchmark Beams:** An expert clinical physicist has carefully selected benchmark beams, providing reference beams for comparison and benchmarking,
+4. **Benchmark IMRT Plan:** A benchmark IMRT plan generated using our in-house automated treatment planning system called ECHO ([YouTube Video](https://youtu.be/895M6j5KjPs), [Paper](https://aapm.onlinelibrary.wiley.com/doi/epdf/10.1002/mp.13572)). This plan serves as a benchmark for evaluating new treatment planning algorithms.
+5. **Benchmark Clinical Criteria:** A set of clinically relevant mean/max/DVH criteria for plan evaluation. 
+Currently, this set encompasses only the Lung 2Gy×30 protocol but will be expanded in the future to more protocols as well as TCP/NTCP evaluation functions.  
+
+To access these resources, users are advised to download the latest version of the dataset, 
+which can be found [here](https://drive.google.com/drive/folders/1nA1oHEhlmh2Hk8an9e0Oi0ye6LRPREit?usp=sharing). 
+Subsequently, create a directory titled './data' in the current project directory and transfer the downloaded 
+file into it. For example, ./data/Lung_Phantom_Patient_1. 
+We have adopted the widely-used JSON and HDF5 formats for data storage.
+[HDFViwer](https://www.hdfgroup.org/downloads/hdfview/) can be utilized to view the contents of the HDF5 files.  
+
+
+
+**Note:** Initially, we will utilize a lung dataset from [TCIA](https://wiki.cancerimagingarchive.net/display/Public/NSCLC-Radiomics). The original DICOM CT images and structure sets are not included in the PortPy dataset and need to be directly downloaded from the TCIA. Users can fetch the **TCIA collection ID** and the **TCIA subject ID** for each PortPy patient using the *get_tcia_metadata()* method in PortPy and subsequently download the data from TCIA (see [eclipse_integration.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/eclipse_integration.ipynb))
+
+
+# Installation <a name="Installation"></a>
+
+1. Install using pip:
+   
+    * Run the command '**pip install portpy**'
+
+2. Install using conda:
+
+    * Run the command '**conda install -c conda-forge portpy**'
+
+3. Install from source:
+   
+    * Clone this repository using '**git clone https://github.com/PortPy-Project/PortPy.git**'
+    * Navigate to the repository with '**cd portpy**'
+
+    * Install the dependencies within a Python virtual environment or Anaconda environment. To set up in a Python virtual environment, install all the dependencies specified in requirements.txt as follows:
+        * Create the virtual environment with '**python3 -m venv venv**'
+        * Activate the environment with '**source venv/bin/activate**'
+        * Install the requirements using '**(venv) pip install -r requirements.txt**'
+
+
+# Team <a name="Team"></a>
+PortPy is a community project initiated at [Memorial Sloan Kettering Cancer Center](https://www.mskcc.org/). It is currently developed and maintained by:
+
+| Name                                                                         | Expertise                                        | Institution |
+|------------------------------------------------------------------------------|--------------------------------------------------|-------------|
+| [Masoud Zarepisheh](https://masoudzp.github.io/)                             | Treatment Planning and Optimization              | MSK         |
+| [Saad Nadeem](https://nadeemlab.org/)                                        | Computer Vision and AI in Medical Imaging        | MSK         |
+| [Gourav Jhanwar](https://github.com/gourav3017)                              | Algorithm Design and Development                 | MSK         |
+| [Mojtaba Tefagh](https://github.com/mtefagh)                                 | Mathematical Modeling and Reinforcement Learning | SUT         |
+| [Vicki Taasti](https://scholar.google.com/citations?user=PEPyvewAAAAJ&hl=en) | Physics and Planning of Proton Therapy           | MAASTRO     |
+| [Seppo Tuomaala](https://www.linkedin.com/in/seppo-tuomaala-5b57913/)        | Eclispe API Scripting                            | VARIAN      |
+
+# License <a name="License"></a>
+PortPy code is distributed under **Apache 2.0 with Commons Clause** license, and is available for non-commercial academic purposes.
+
+# Reference <a name="Reference"></a>
+If you find our work useful in your research or if you use parts of this code please cite our [AAPM'23 abstract](https://aapm.confex.com/aapm/2023am/meetingapp.cgi/Paper/4208) :
+```
+@article{jhanwar2023portpy,
+  title={Portpy: An Open-Source Python Package for Planning and Optimization in Radiation Therapy Including Benchmark Data and Algorithms},
+  author={Jhanwar, Gourav and Tefagh, Mojtaba and Taasti, Vicki T and Alam, Sadegh R and Tuomaala, Seppo and Nadeem, Saad and Zarepisheh, Masoud},
+  journal={AAPM 65th Annual Meeting & Exhibition},
+  year={2023}
+}
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `portpy-1.0.3/images/PortPy_logo.jpg` & `portpy-1.0.3.1/images/PortPy_logo.jpg`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3/images/dose_comp.JPG` & `portpy-1.0.3.1/images/dose_comp.JPG`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3/images/planner_vs_portpy_dvh.JPG` & `portpy-1.0.3.1/images/planner_vs_portpy_dvh.JPG`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3/portpy/ai/data/__init__.py` & `portpy-1.0.3.1/portpy/ai/data/__init__.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3/portpy/ai/data/base_dataset.py` & `portpy-1.0.3.1/portpy/ai/data/base_dataset.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3/portpy/ai/data/dosepred3d_dataset.py` & `portpy-1.0.3.1/portpy/ai/data/dosepred3d_dataset.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3/portpy/ai/data/image_folder.py` & `portpy-1.0.3.1/portpy/ai/data/image_folder.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3/portpy/ai/data/single_dataset.py` & `portpy-1.0.3.1/portpy/ai/data/single_dataset.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3/portpy/ai/data/template_dataset.py` & `portpy-1.0.3.1/portpy/ai/data/template_dataset.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3/portpy/ai/example.py` & `portpy-1.0.3.1/portpy/ai/example.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3/portpy/ai/models/__init__.py` & `portpy-1.0.3.1/portpy/ai/models/__init__.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3/portpy/ai/models/base_model.py` & `portpy-1.0.3.1/portpy/ai/models/base_model.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3/portpy/ai/models/doseprediction3d_model.py` & `portpy-1.0.3.1/portpy/ai/models/doseprediction3d_model.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3/portpy/ai/models/networks3d.py` & `portpy-1.0.3.1/portpy/ai/models/networks3d.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3/portpy/ai/models/test_model.py` & `portpy-1.0.3.1/portpy/ai/models/test_model.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3/portpy/ai/options/PyesapiTutorial.py` & `portpy-1.0.3.1/portpy/ai/options/PyesapiTutorial.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3/portpy/ai/options/base_options.py` & `portpy-1.0.3.1/portpy/ai/options/base_options.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3/portpy/ai/options/test_options.py` & `portpy-1.0.3.1/portpy/ai/options/test_options.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3/portpy/ai/options/train_options.py` & `portpy-1.0.3.1/portpy/ai/options/train_options.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3/portpy/ai/predict.py` & `portpy-1.0.3.1/portpy/ai/predict.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3/portpy/ai/runRandomTrain.py` & `portpy-1.0.3.1/portpy/ai/runRandomTrain.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3/portpy/ai/test.py` & `portpy-1.0.3.1/portpy/ai/test.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3/portpy/ai/train.py` & `portpy-1.0.3.1/portpy/ai/train.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3/portpy/ai/util/html.py` & `portpy-1.0.3.1/portpy/ai/util/html.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3/portpy/ai/util/image_pool.py` & `portpy-1.0.3.1/portpy/ai/util/image_pool.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3/portpy/ai/util/util.py` & `portpy-1.0.3.1/portpy/ai/util/util.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3/portpy/ai/util/visualizer.py` & `portpy-1.0.3.1/portpy/ai/util/visualizer.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3/portpy/config_files/clinical_criteria/Default/Lung_2Gy_30Fx.json` & `portpy-1.0.3.1/portpy/config_files/clinical_criteria/Default/Lung_2Gy_30Fx.json`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3/portpy/config_files/optimization_params/optimization_params_Lung_2Gy_30Fx.json` & `portpy-1.0.3.1/portpy/config_files/optimization_params/optimization_params_Lung_2Gy_30Fx.json`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3/portpy/photon/beam.py` & `portpy-1.0.3.1/portpy/photon/beam.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3/portpy/photon/clinical_criteria.py` & `portpy-1.0.3.1/portpy/photon/clinical_criteria.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3/portpy/photon/ct.py` & `portpy-1.0.3.1/portpy/photon/ct.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3/portpy/photon/data_explorer.py` & `portpy-1.0.3.1/portpy/photon/data_explorer.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3/portpy/photon/evaluation.py` & `portpy-1.0.3.1/portpy/photon/evaluation.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3/portpy/photon/influence_matrix.py` & `portpy-1.0.3.1/portpy/photon/influence_matrix.py`

 * *Files 0% similar despite different names*

```diff
@@ -447,18 +447,18 @@
             x_and_y = [(a.x, a.y) for a in valid_points]
             XX, YY = np.meshgrid(x_min_max_sort, y_max_min_sort)
             w_all = np.column_stack((x_positions, y_positions))
             if count_num == 0:
                 mask = np.zeros_like(XX, dtype=bool)
             for row in range(XX.shape[0]):
                 for col in range(XX.shape[1]):
-                    ind = np.where((w_all[:, 0] == XX[row, col]) & (w_all[:, 1] == YY[row, col]))[0][0]
+                    ind1 = np.where((w_all[:, 0] == XX[row, col]) & (w_all[:, 1] == YY[row, col]))[0][0]
 
                     # if (beamlets[ind]['position_x_mm'], beamlets[ind]['position_y_mm']) in x_and_y:
-                    if (beamlets['position_x_mm'][0][ind], beamlets['position_y_mm'][0][ind]) in x_and_y:
+                    if (beamlets['position_x_mm'][0][ind1], beamlets['position_y_mm'][0][ind1]) in x_and_y:
                         # beam_map[row, col] = beamlets[ind]['id']
                         mask[row, col] = True
         return mask
 
     def preprocess_beams(self, structure='PTV', remove_corner_beamlets=False):
         """
         Preprocess beams to create beamlets dictionary based on beamlet resolution.
```

### Comparing `portpy-1.0.3/portpy/photon/optimization.py` & `portpy-1.0.3.1/portpy/photon/optimization.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3/portpy/photon/plan.py` & `portpy-1.0.3.1/portpy/photon/plan.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3/portpy/photon/structures.py` & `portpy-1.0.3.1/portpy/photon/structures.py`

 * *Files 2% similar despite different names*

```diff
@@ -264,27 +264,32 @@
 
         constraints = criteria + opt_params_constraints
         print('Creating optimization structures.. It may take some time due to dilation')
         for ind, obj in enumerate(obj_funcs):
             if 'structure_def' in obj:
                 if obj['structure_name'] not in self.get_structures():
                     structure_def = obj['structure_def']
-                    mask_3d = self.evaluate_expression(structure_def)
-                    result = mask_3d & self.get_structure_mask_3d('BODY')
-                    self.create_structure(new_struct_name=obj['structure_name'], mask_3d=result)
+                    try:
+                        mask_3d = self.evaluate_expression(structure_def)
+                        result = mask_3d & self.get_structure_mask_3d('BODY')
+                        self.create_structure(new_struct_name=obj['structure_name'], mask_3d=result)
+                    except:
+                        Warning('Cannot evaluate structure defintion'.format(structure_def))
 
         for ind, criterion in enumerate(constraints):
             if 'structure_def' in criterion['parameters']:
                 param = criterion['parameters']
                 structure_def = param['structure_def']
                 if param['structure_name'] not in self.get_structures():
-                    mask_3d = self.evaluate_expression(structure_def)
-                    result = mask_3d & self.get_structure_mask_3d('BODY')
-                    self.create_structure(new_struct_name=param['structure_name'], mask_3d=result)
-
+                    try:
+                        mask_3d = self.evaluate_expression(structure_def)
+                        result = mask_3d & self.get_structure_mask_3d('BODY')
+                        self.create_structure(new_struct_name=param['structure_name'], mask_3d=result)
+                    except:
+                        Warning('Cannot evaluate structure defintion'.format(structure_def))
         print('Optimization structures created!!')
         # for param in rind_params:
         #     self.set_opt_voxel_idx(struct_name=param['name'])
         self.preprocess_structures()
 
     def preprocess_structures(self):
         """
@@ -365,14 +370,17 @@
         :param structure: struct_name to be removed
         :return:
         """
         ind = self.structures_dict['name'].index(structure)
         for key in self.structures_dict.keys():
             del self.structures_dict[key][ind]
 
+    def get_ct_voxel_resolution_xyz_mm(self):
+        return self._ct_voxel_resolution_xyz_mm
+
     def set_opt_voxel_idx(self, struct_name):
         ind = self.structures_dict['name'].index(struct_name)
         vox_3d = self.structures_dict['structure_mask_3d'][ind] * \
                  self.opt_voxels_dict['ct_to_dose_voxel_map'][0]
         # my_plan.structures_dict['voxel_idx'][i] = np.unique(vox_3d[vox_3d > 0])
         vox, counts = np.unique(vox_3d[vox_3d > 0], return_counts=True)
         self.opt_voxels_dict['voxel_idx'].append(vox)
@@ -387,18 +395,24 @@
         if isinstance(right_operand, str):
             if right_operand == "inf":
                 right_operand = "500"
         left_operand = values_stack.pop()
 
         if isinstance(left_operand, str):
             if not left_operand.isnumeric():
-                left_operand = self.get_structure_mask_3d(left_operand)
+                if left_operand not in self.structures_dict['name']:
+                    raise Exception("Invalid structure {}".format(left_operand))
+                else:
+                    left_operand = self.get_structure_mask_3d(left_operand)
         if isinstance(right_operand, str):
             if not right_operand.isnumeric():
-                right_operand = self.get_structure_mask_3d(right_operand)
+                if right_operand not in self.structures_dict['name']:
+                    raise Exception("Invalid structure {}".format(right_operand))
+                else:
+                    right_operand = self.get_structure_mask_3d(right_operand)
 
         if operator == '+':
             if isinstance(right_operand, str):
                 result = self.expand(mask_3d=left_operand, margin_mm=float(right_operand), return_mask=True)
             else:
                 result = left_operand | right_operand
         elif operator == '-':
@@ -431,22 +445,28 @@
                 while j < len(expression) and (expression[j].isalpha() or expression[j] in '_.$^' or expression[j].isdigit()):
                     j += 1
                 struct = expression[i:j]
                 values_stack.append(struct)
                 i = j - 1
             elif expression[i] in '+-|&':
                 while operators_stack and operators_stack[-1] in '+-|&':
-                    self.apply_operator(operators_stack, values_stack)
+                    try:
+                        self.apply_operator(operators_stack, values_stack)
+                    except:
+                        raise Exception("Cannot evaluate expression")
                 operators_stack.append(expression[i])
             elif expression[i] == '(':
                 operators_stack.append(expression[i])
             elif expression[i] == ')':
                 while operators_stack[-1] != '(':
                     self.apply_operator(operators_stack, values_stack)
                 operators_stack.pop()
 
             i += 1
 
         while operators_stack:
-            self.apply_operator(operators_stack, values_stack)
+            try:
+                self.apply_operator(operators_stack, values_stack)
+            except:
+                raise Exception("Cannot evaluate expression")
 
         return values_stack[0]
```

### Comparing `portpy-1.0.3/portpy/photon/utils/convert_dose_rt_dicom_to_portpy.py` & `portpy-1.0.3.1/portpy/photon/utils/convert_dose_rt_dicom_to_portpy.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3/portpy/photon/utils/get_eclipse_fluence.py` & `portpy-1.0.3.1/portpy/photon/utils/get_eclipse_fluence.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3/portpy/photon/utils/leaf_sequencing_siochi.py` & `portpy-1.0.3.1/portpy/photon/utils/leaf_sequencing_siochi.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3/portpy/photon/utils/save_nrrd.py` & `portpy-1.0.3.1/portpy/photon/utils/save_nrrd.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3/portpy/photon/utils/save_or_load_pickle.py` & `portpy-1.0.3.1/portpy/photon/utils/save_or_load_pickle.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3/portpy/photon/utils/slicer_script.py` & `portpy-1.0.3.1/portpy/photon/utils/slicer_script.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3/portpy/photon/utils/view_in_slicer_jupyter.py` & `portpy-1.0.3.1/portpy/photon/utils/view_in_slicer_jupyter.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3/portpy/photon/utils/write_rt_plan_imrt.py` & `portpy-1.0.3.1/portpy/photon/utils/write_rt_plan_imrt.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3/portpy/photon/visualization.py` & `portpy-1.0.3.1/portpy/photon/visualization.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3/portpy.egg-info/PKG-INFO` & `portpy-1.0.3.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,97 +1,180 @@
 Metadata-Version: 2.1
 Name: portpy
-Version: 1.0.3
+Version: 1.0.3.1
 Summary: First open-source radiation treatment planning system in Python
 Home-page: https://github.com/PortPy-Project/PortPy
 Author: Gourav Jhanwar, Mojtaba Tefagh, Vicki Taasti, Seppo Tuomaala, Saad Nadeem, Masoud Zarepisheh
 Author-email: jhanwarg@mskcc.struct, mtefagh@acm.struct, vicki.taasti@maastro.nl, tuomaals@mskcc.struct, nadeems@mskcc.struct, zarepism@mskcc.struct
 License: Apache License, Version 2.0
 Description: <p align="center">
           <img src="./images/PortPy_logo.png" width="40%" height="40%">
         </p>
         
-        ![Version](https://img.shields.io/static/v1?label=latest&message=v1.0.2&color=darkgreen)
+        ![Version](https://img.shields.io/static/v1?label=latest&message=v1.0.3&color=darkgreen)
         [![Total Downloads](https://static.pepy.tech/personalized-badge/portpy?period=total&units=international_system&left_color=grey&right_color=blue&left_text=total%20downloads)](https://pepy.tech/project/portpy?&left_text=totalusers)
         
         # What is PortPy?
         
-        PortPy, short for **P**lanning and **O**ptimization for **R**adiation **T**herapy, represents a collective effort to establish an open-source Python library dedicated to advancing the development and clinical implementation of cancer radiotherapy treatment planning algorithms. This initiative encompasses planning methodologies for Intensity Modulated Radiation Therapy (IMRT), Volumetric Modulated Arc Therapy (VMAT), along with other emerging modalities. PortPy provides clinical-grade data and coding resources that foster *benchmarking*, *reproducibility*, and *community development*.
-        
+        PortPy, short for **P**lanning and **O**ptimization for **R**adiation **T**herapy, represents a collective effort 
+        to establish an open-source Python library dedicated to advancing the development and clinical implementation of 
+        cancer radiotherapy treatment planning algorithms. This initiative encompasses planning methodologies for 
+        Intensity Modulated Radiation Therapy (IMRT), Volumetric Modulated Arc Therapy (VMAT), along with other 
+        emerging modalities. PortPy provides clinical-grade data and coding resources that foster *benchmarking*, 
+        *reproducibility*, and *community development*.
+        
+        **Note:** In the near future, we plan to launch an educational YouTube channel to assist 
+        researchers new to this field. Meanwhile, we suggest reviewing relevant literature review papers
+        ([Zarepisheh et al. 2021](https://pubsonline.informs.org/doi/abs/10.1287/inte.2021.1095), 
+        [Breedveld et al. 2019](https://www.sciencedirect.com/science/article/abs/pii/S0377221718307148), 
+        [Ehrgott et al. 2010](https://link.springer.com/article/10.1007/s10479-009-0659-4)) and watching YouTube videos 
+        ([Edelman competition](https://www.youtube.com/watch?v=895M6j5KjPs&t=1025s), [Varian IMRT](https://www.youtube.com/watch?v=eZS6DVGBx0k), [Elekta VMAT](https://www.youtube.com/watch?v=AE1SxvnFT3s)).
+          
         
         **Contents**
+        - [Why we created PortPy?](#Why)
         - [What can you do with PortPy?](#WhatDo)
         - [Quick Start](#QuickStart)
         - [How to contribute?](#limitations)
-        - [The limitations of current version](#limitations)
         - [Data](#Data)
         - [Installation](#Installation)
         - [Team](#Team)
         
+        # Why we created PortPy? <a name="Why"></a>
+        
+        <p align="center">
+          <img src="./images/PortPyIntegration.png" width="60%" height="40%">
+        <p>
+        
+        
+        A key limitation of existing open-source packages in radiotherapy treatment planning is their
+        inability to objectively evaluate new treatment planning techniques against current clinical practices. 
+        This limitation stems from the difficulty in fully replicating clinical environments, such as detailed 
+        linear accelerator configurations and commercial dose calculation engines. Consequently,
+        plans generated using novel techniques, such as AI-based automated treatment planning, cannot be objectively compared
+        with clinical plans used in patient treatment. To address this limitation, we are integrating PortPy with 
+        commercial treatment planning systems (TPSs). PortPy is already compatible with the [Varian Eclipse TPS](https://www.varian.com/), 
+        and we plan to expand compatibility to additional TPSs in the future. It's crucial to note that PortPy can 
+        be used independently of any TPS, but accessing a TPS is essential for final evaluation within the TPS (see above figure).
+        <p align="center">
+          <img src="./images/AI_Pyramid.png" width="40%" height="40%">
+        <p>
+        
+        Above figure highlights the inspiration for developing PortPy, drawing on successful open-source practices 
+        from the AI and computer science communities. Tools like PyTorch and TensorFlow, along with benchmark datasets 
+        such as ImageNet and algorithms like AlexNet, have transformed AI and data science. Our aim is to emulate 
+        this success, providing researchers with comprehensive resources (PortPy integration with commercial TPS 
+        and other renowned open-source tools such as [3DSlicer](https://www.slicer.org/) and [CVXPy](https://www.cvxpy.org/), a benchmark dataset 
+        (featuring 50 curated lung patients with expertly selected beams, all necessary optimization data, 
+        and benchmark IMRT plans created using our in-house automated planning system, ECHO), 
+        and benchmark algorithms, including Mixed Integer Programming (MIP) algorithms for achieving globally optimal solutions.
+        
         
         
         
         # What can you do with PortPy? <a name="WhatDo"></a>
-        PortPy facilitates the **design**, **testing**, and **clinical validation** of your treatment planning algorithms. This includes both cutting-edge AI-based models and traditional optimization techniques. PortPy provides:
-        1. **Benchmark Dataset**
-             * Access to data required for optimization, extracted directly from the FDA-approved Eclipse treatment planning system via its API 
-             * A current set of data from 50 lung patients, which will be expanded to 100 lung patients by the end of 2023
-             * A **benchmark IMRT plan** for each patient, created using our in-house automated planning system ([Edelman Award Finalist YouTube Video](https://youtu.be/895M6j5KjPs), [Paper](https://aapm.onlinelibrary.wiley.com/doi/epdf/10.1002/mp.13572))
-           
-        2. **Benchmark Algorithms:** Offering globally optimal solutions for:
-             * Dose Volume Histogram (DVH) constraints (see [dvh_constraint_optimization.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/benchmark_algorithms/dvh_constraint_optimization.ipynb))
-             * IMRT Beam Orientation Optimization (BOO) (see [beam_orientation_optimization.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/benchmark_algorithms/beam_orientation_optimization.ipynb))
-             * Volumetric Modulated Arc Therapy (VMAT) (see [vmat_optimization.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/benchmark_algorithms/vmat_optimization.ipynb))
-        4. **Visualization**
-             * Basic built-in visualization tools (e.g., DVH, dose distribution) are integrated into PortPy (see (see [basic_tutorial.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/1_basic_tutorial.ipynb)))
-             * Enhanced visualizations are available through the integration with the popular open-source [3DSlicer](https://www.slicer.org/) package (see [3d_slicer_integration.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/3d_slicer_integration.ipynb))
-        5. **Evaluation**  
+        
+        <p align="center">
+        <img src="./images/PortPy-Workflow.png" width="90%" height="40%">
+        <p>
+        
+        PortPy facilitates the **design**, **testing**, and **clinical validation** of new treatment planning algorithms. 
+        This includes both cutting-edge AI-based models and traditional optimization techniques. 
+        The above figure illustrates the PortPy design and its three main
+        modules: “Data Management”, “Plan Generation”, and “Plan
+        Evaluation”,  which are discussed below. We recommend reviewing our Jupyter Notebooks 
+        examples for a more comprehensive understanding of these modules. 
+        
+        1. **Data Management**
+             * This module provides access to the curated benchmark PortPy dataset, which currently comprises data from 50 lung patients.
+        It allows researchers to test and develop their algorithms using the same dataset (see [basic_tutorial.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/1_basic_tutorial.ipynb) notebook)
+             * The available data includes: 1) CT images and contours, 2) all necessary data for optimization extracted from 
+        Eclipse using its API (version 16.1), 3)expert-selected beams for each patient, 4) an IMRT plan for each patient, 
+        generated using our in-house automated planning system, 
+        ECHO ([YouTube Video](https://youtu.be/895M6j5KjPs), [Paper](https://aapm.onlinelibrary.wiley.com/doi/epdf/10.1002/mp.13572)).
+        More information about data can be found in [Data](#Data) section.
+             * In the current version, you can only work with the benchmark dataset provided in this PortPy repo and 
+           cannot use your own dataset for now. We will address this problem in the near future
+        
+        2. **Plan Generation**
+             * This module facilitates the generation of treatment plans using either classical optimization methods or 
+        emerging AI-based techniques 
+             * For optimization tasks, PortPy has been integrated with [CVXPy](https://www.cvxpy.org/), a widely-used open-source package. 
+        CVXPy enables the high-level formulation of optimization problems and offers out-of-the-box access to a range
+        of free (e.g., [SCIP](https://www.scipopt.org/), [SCIPY](https://docs.scipy.org/doc/scipy/reference/optimize.html)) and commercial (e.g., [MOSEK](https://www.mosek.com/), [CPLEX](https://www.ibm.com/products/ilog-cplex-optimization-studio/cplex-optimizer), [GUROBI](https://www.gurobi.com/)) optimization engines (available for free for research
+        purposes) (see [basic_tutorial.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/1_basic_tutorial.ipynb) notebook)
+             * PortPy.AI module is equipped with essential functionalities for AI-based planning. These include data access, 
+        data pre-processing, model training and testing, and patient-specific 3D dose prediction 
+        (see [dose_prediction_pipeline.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/AI_tutorials/dose_prediction_pipeline.ipynb) notebook)
+             * The availability of both optimization and AI-based planning modules within PortPy allows researchers 
+        to not only compare these techniques but also explore their complementary aspects
+        
+        3. **Plan Visualization and Evaluation**
+             * Basic built-in visualization tools (e.g., DVH, dose distribution) are integrated into PortPy 
+             * Enhanced visualizations are available through the integration with the popular open-source [3DSlicer](https://www.slicer.org/) package (see [3d_slicer_integration.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/3d_slicer_integration.ipynb) notebook)
              * PortPy IMRT plans with optimal fluence can be imported into Eclipse for leaf sequencing and final clinical evaluations  (see [eclipse_integration.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/eclipse_integration.ipynb))
-             * PortPy IMRT/VMAT plans can be imported into FDA approved TPS( e.g. Eclipse, Raystation) using DICOM RT Plan file for final clinical evaluations  (see [TPS-integration.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/TPS-Integration.ipynb))
+             * PortPy IMRT/VMAT plans with optimal control points can be imported into any FDA approved TPS ( e.g. Eclipse, Raystation) using DICOM RT Plan file for final clinical evaluations  (see [TPS-integration.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/TPS-Integration.ipynb)).
+        It should be noted that some discrepancies are anticipated 
+        with TPSs other than Eclipse, due to the fact that our current data are derived from Eclipse, and there 
+        may exist variations in dose calculation methods between Eclipse and other TPSs. 
              * Plans can also be evaluated within PortPy using well-established clinical protocols (e.g., Lung 2Gyx30, see  [basic_tutorial.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/1_basic_tutorial.ipynb))
              * Future updates will include more standardized RTOG metrics and outcome models (TCP/NTCP)
-        6. **Optimization** 
-             * PortPy provides high-level optimization problem formulation and access to both free and commercial optimization engines through the integration with a popular open-source [CVXPy](https://www.cvxpy.org/) package (see [basic_tutorial.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/1_basic_tutorial.ipynb))
-             * Commercial engines (e.g., [MOSEK](https://www.mosek.com/), [CPLEX](https://www.ibm.com/products/ilog-cplex-optimization-studio/cplex-optimizer), [GUROBI](https://www.gurobi.com/)) are also free for academic and research use
-        7. **AI-Based Planning** 
-             * The PortPy.AI module provides a framework for exploring AI-driven treatment planning  (see [dose_prediction_pipeline.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/AI_tutorials/dose_prediction_pipeline.ipynb))
-             * The newly added PortPy.AI module includes a tutorial on predicting a 3D-dose distribution and converting the prediction into a deliverable plan
+        
+        
         
         # Quick Start <a name="QuickStart"></a>
         
         1. To grasp the primary features of PortPy, we highly recommend exploring the [basic_tutorial.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/1_basic_tutorial.ipynb) notebook
         2. To understand how to import a PortPy plan into Eclipse for final evaluations, browse through the [eclipse_integration.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/eclipse_integration.ipynb) notebook
         3. To create dicom RT Plan file from PortPy plan and import into FDA approved commercial TPS (e.g. Eclipse, Raystation), please browse through [TPS-integration.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/TPS-Integration.ipynb) notebook
         4. To learn about enhanced visualization techniques using the 3D-Slicer package, refer to the  [3d_slicer_integration.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/3d_slicer_integration.ipynb) notebook
         5. For algorithm benchmarking, the global optimal solutions are provided for non-convex optimization problems resulting from beam angle optimization [beam_orientation_optimization.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/benchmark_algorithms/beam_orientation_optimization.ipynb), incorporating DVH constraints [dvh_constraint_optimization.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/benchmark_algorithms/dvh_constraint_optimization.ipynb), and VMAT optimization [vmat_optimization.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/benchmark_algorithms/vmat_optimization.ipynb) using the mixed-integer programming on down-sampled data.
         6. If you encounter computational challenges with large-scale optimization problems, you can opt for down-sampling the voxels/beamlets, as illustrated in the [down_sampling](https://github.com/PortPy-Project/PortPy/blob/master/examples/advanced_tutorials/down_sampling.ipynb) notebook, or further sparsify the influence matrix, as demonstrated in the [inf_matrix_sparsification](https://github.com/PortPy-Project/PortPy/blob/master/examples/advanced_tutorials/inf_matrix_sparsification.ipynb) notebook.
         7. To learn about creating a final deliverable plan using AI based model, please refer to [dose_prediction_pipeline.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/AI_tutorials/dose_prediction_pipeline.ipynb) notebook.
         
         # How to contribute? <a name="HowContribute"></a>
-        To maintain the lightweight nature and user-friendliness of PortPy modules, our aim is to include only fundamental functionalities, along with benchmark data and algorithms. We will establish separate repositories within the [PortPy-Project orgainization](https://github.com/PortPy-Project) for projects developed by our team using PortPy as a platform. This is similar to what we've done for projects like [LowDimRT](https://github.com/PortPy-Project/LowDimRT) and [VMAT](https://github.com/PortPy-Project/ECHO-VMAT).
-        
-        If you're interested in contributing to existing PortPy modules or wish to create a new module, we encourage you to contact us first. This will help ensure that our objectives and priorities are aligned. If you use PortPy to build your own package, you're welcome to host your package within the [PortPy-Project orgainization](https://github.com/PortPy-Project). Alternatively, you can host your package on your own GitHub page. In this case, please inform us so that we can fork it and feature it under the PortPy-Project organization.
-        
+        <p align="center">
+        <img src="./images/PortPy_Organization.png" width="90%" height="40%">
+        <p>
+        
+        As illustrated in the above figure, PortPy organization includes "PortPy", which is the current repository, 
+        and PortPy extensions, which are the repositories developed using the PortPy as a platform. 
+        To maintain the lightweight nature and user-friendliness of PortPy modules, our aim is to include only fundamental 
+        functionalities, along with benchmark data and algorithms in the PortPy repo, and establish separate repositories 
+        for other projects, similar to what we've done for projects like [LowDimRT](https://github.com/PortPy-Project/LowDimRT)
+        and [ECHO VMAT](https://github.com/PortPy-Project/ECHO-VMAT).
+        
+        If you're interested in contributing to existing PortPy modules or wish to create a new module, 
+        we encourage you to contact us first. This will help ensure that our objectives and priorities are aligned. 
+        If you use PortPy to build your own package, you're welcome to host your package within the
+        [PortPy-Project orgainization](https://github.com/PortPy-Project). 
+        Alternatively, you can host your package on your own GitHub page. In this case, 
+        please inform us so that we can fork it and feature it under the PortPy-Project organization. 
+        For those keen on creating a logo for their repository, we offer the option to customize our [pre-designed logo](https://www.canva.com/design/DAFxivHC0Js/YqZREdr26pmEsIgCeuU-iA/view?utm_content=DAFxivHC0Js&utm_campaign=designshare&utm_medium=link&utm_source=publishsharelink&mode=preview).
         
-        # The limitations of current version of PortPy <a name="limitations"></a>
-        Current version of PortPy has the following limitations which would be addressed in the future updates:
-        
-        1. You can only work with the benchmark dataset provided in this PortPy repo and cannot use your own dataset for now.
-        2. PortPy.Photon and PortPy.AI are the only modules available. You cannot do proton research with the current version. Please use [OpenTPS](http://opentps.org/) for proton research.
         
         # Data <a name="Data"></a>
-        
+        <p align="center">
+        <img src="./images/PortPy Data.png" width="90%" height="40%">
+        <p>
         PortPy equips researchers with a robust benchmark patient dataset, sourced from the FDA-approved Eclipse commercial treatment planning system through its API. This dataset embodies all necessary elements for optimizing various machine configurations such as beam angles, aperture shapes, and leaf movements. It includes
         
-        1. **Dose Influence Matrix:** The dose contribution of each beamlet to each voxel,
+        1. **Dose Influence Matrix (AKA dose deposition matrix, dij matrix):** The dose contribution of each beamlet to each voxel,
         2. **Beamlets/Voxels Details:** Detailed information about the position and size of beamlets/voxels,
         3. **Expert-Selected Benchmark Beams:** An expert clinical physicist has carefully selected benchmark beams, providing reference beams for comparison and benchmarking,
-        4. **Benchmark IMRT Plan:** A benchmark IMRT plan generated using our in-house automated treatment planning system called ECHO ([Edelman Award Finalist YouTube Video](https://youtu.be/895M6j5KjPs), [Paper](https://aapm.onlinelibrary.wiley.com/doi/epdf/10.1002/mp.13572)). This plan serves as a benchmark for evaluating new treatment planning algorithms.
-        
-        To access these resources, users are advised to download the latest version of the dataset, which can be found [here](https://drive.google.com/drive/folders/1nA1oHEhlmh2Hk8an9e0Oi0ye6LRPREit?usp=sharing). Subsequently, create a directory titled './data' in the current project directory and transfer the downloaded file into it. For example, ./data/Lung_Phantom_Patient_1.
+        4. **Benchmark IMRT Plan:** A benchmark IMRT plan generated using our in-house automated treatment planning system called ECHO ([YouTube Video](https://youtu.be/895M6j5KjPs), [Paper](https://aapm.onlinelibrary.wiley.com/doi/epdf/10.1002/mp.13572)). This plan serves as a benchmark for evaluating new treatment planning algorithms.
+        5. **Benchmark Clinical Criteria:** A set of clinically relevant mean/max/DVH criteria for plan evaluation. 
+        Currently, this set encompasses only the Lung 2Gy×30 protocol but will be expanded in the future to more protocols as well as TCP/NTCP evaluation functions.  
+        
+        To access these resources, users are advised to download the latest version of the dataset, 
+        which can be found [here](https://drive.google.com/drive/folders/1nA1oHEhlmh2Hk8an9e0Oi0ye6LRPREit?usp=sharing). 
+        Subsequently, create a directory titled './data' in the current project directory and transfer the downloaded 
+        file into it. For example, ./data/Lung_Phantom_Patient_1. 
+        We have adopted the widely-used JSON and HDF5 formats for data storage.
+        [HDFViwer](https://www.hdfgroup.org/downloads/hdfview/) can be utilized to view the contents of the HDF5 files.  
         
         
         
         **Note:** Initially, we will utilize a lung dataset from [TCIA](https://wiki.cancerimagingarchive.net/display/Public/NSCLC-Radiomics). The original DICOM CT images and structure sets are not included in the PortPy dataset and need to be directly downloaded from the TCIA. Users can fetch the **TCIA collection ID** and the **TCIA subject ID** for each PortPy patient using the *get_tcia_metadata()* method in PortPy and subsequently download the data from TCIA (see [eclipse_integration.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/eclipse_integration.ipynb))
         
         
         # Installation <a name="Installation"></a>
@@ -121,15 +204,14 @@
         | Name                                                                         | Expertise                                        | Institution |
         |------------------------------------------------------------------------------|--------------------------------------------------|-------------|
         | [Masoud Zarepisheh](https://masoudzp.github.io/)                             | Treatment Planning and Optimization              | MSK         |
         | [Saad Nadeem](https://nadeemlab.org/)                                        | Computer Vision and AI in Medical Imaging        | MSK         |
         | [Gourav Jhanwar](https://github.com/gourav3017)                              | Algorithm Design and Development                 | MSK         |
         | [Mojtaba Tefagh](https://github.com/mtefagh)                                 | Mathematical Modeling and Reinforcement Learning | SUT         |
         | [Vicki Taasti](https://scholar.google.com/citations?user=PEPyvewAAAAJ&hl=en) | Physics and Planning of Proton Therapy           | MAASTRO     |
-        | [Sadegh Alam](https://scholar.google.com/citations?user=iy7TlU0AAAAJ&hl=en)  | Adaptive Treatment Planning and Imaging          | Cornell     |
         | [Seppo Tuomaala](https://www.linkedin.com/in/seppo-tuomaala-5b57913/)        | Eclispe API Scripting                            | VARIAN      |
         
         # License <a name="License"></a>
         PortPy code is distributed under **Apache 2.0 with Commons Clause** license, and is available for non-commercial academic purposes.
         
         # Reference <a name="Reference"></a>
         If you find our work useful in your research or if you use parts of this code please cite our [AAPM'23 abstract](https://aapm.confex.com/aapm/2023am/meetingapp.cgi/Paper/4208) :
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `portpy-1.0.3/portpy.egg-info/SOURCES.txt` & `portpy-1.0.3.1/portpy.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 MANIFEST.in
 README.md
 setup.py
+images/PortPy-full-pipeline.jpg
 images/PortPy_logo.jpg
 images/dose_comp.JPG
 images/planner_vs_portpy_dvh.JPG
 portpy/__init__.py
 portpy.egg-info/PKG-INFO
 portpy.egg-info/SOURCES.txt
 portpy.egg-info/dependency_links.txt
@@ -34,14 +35,15 @@
 portpy/ai/options/train_options.py
 portpy/ai/util/__init__.py
 portpy/ai/util/html.py
 portpy/ai/util/image_pool.py
 portpy/ai/util/util.py
 portpy/ai/util/visualizer.py
 portpy/config_files/__init__.py
+portpy/config_files/clinical_criteria/Default/HN_1Gy_1Fx.json
 portpy/config_files/clinical_criteria/Default/Lung_2Gy_30Fx.json
 portpy/config_files/optimization_params/optimization_params_Lung_2Gy_30Fx.json
 portpy/photon/__init__.py
 portpy/photon/beam.py
 portpy/photon/clinical_criteria.py
 portpy/photon/ct.py
 portpy/photon/data_explorer.py
```

### Comparing `portpy-1.0.3/setup.py` & `portpy-1.0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     version=_VERSION,
     url='https://github.com/PortPy-Project/PortPy',
     license='Apache License, Version 2.0',
     packages=find_packages(exclude=["examples*"]),
     author='Gourav Jhanwar, Mojtaba Tefagh, Vicki Taasti, Seppo Tuomaala, Saad Nadeem, Masoud Zarepisheh',
     author_email="jhanwarg@mskcc.struct, mtefagh@acm.struct, vicki.taasti@maastro.nl, tuomaals@mskcc.struct, nadeems@mskcc.struct, zarepism@mskcc.struct",
     description='First open-source radiation treatment planning system in Python',
-    long_description=open('README.md').read(),
+    long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     python_requires='>=3.7',
     include_package_data=True,
     classifiers=[
         'Development Status :: 1 - Planning',
         'Intended Audience :: Developers',
         'Intended Audience :: Education',
```

