# Comparing `tmp/Simba-UW-tf-dev-1.92.4.tar.gz` & `tmp/Simba-UW-tf-dev-1.92.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Simba-UW-tf-dev-1.92.4.tar", last modified: Sat May 18 15:52:47 2024, max compression
+gzip compressed data, was "dist/Simba-UW-tf-dev-1.92.5.tar", last modified: Sun May 19 17:55:13 2024, max compression
```

## Comparing `Simba-UW-tf-dev-1.92.4.tar` & `Simba-UW-tf-dev-1.92.5.tar`

### file list

```diff
@@ -1,685 +1,686 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-18 15:52:47.000000 Simba-UW-tf-dev-1.92.4/
--rw-r--r--   0 simon      (501) staff       (20)     2797 2024-05-18 15:52:47.000000 Simba-UW-tf-dev-1.92.4/PKG-INFO
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-18 15:52:47.000000 Simba-UW-tf-dev-1.92.4/simba/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-18 15:52:47.000000 Simba-UW-tf-dev-1.92.4/simba/ui/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-28 13:50:53.000000 Simba-UW-tf-dev-1.92.4/simba/ui/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-18 15:52:47.000000 Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/
--rw-r--r--   0 simon      (501) staff       (20)    11467 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/mutual_exclusivity_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4070 2024-03-29 20:30:28.000000 Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1676 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/csv_2_parquet_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5883 2024-04-22 13:59:07.000000 Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/quick_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2873 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/batch_preprocess_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8831 2024-05-02 13:40:02.000000 Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/heatmap_location_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9578 2024-04-26 18:13:38.000000 Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/clf_probability_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3456 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/movement_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4631 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    11362 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/clf_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    25598 2024-04-17 23:32:48.000000 Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1184 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/remove_roi_features_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6692 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/targeted_annotation_clips_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3340 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2174 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/roi_size_standardizer_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     6997 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4682 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/roi_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7898 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/outlier_settings_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9366 2024-04-29 16:29:26.000000 Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/gantt_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5830 2024-04-26 18:09:47.000000 Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/clf_validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8529 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/severity_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3221 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/fsttc_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4231 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/kleinberg_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8376 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9785 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/spontaneous_alternation_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6076 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/pose_reorganizer_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3437 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/animal_directing_other_animals_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3352 2024-04-26 15:18:54.000000 Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3468 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/clf_by_timebins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9154 2024-04-12 00:32:53.000000 Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/heatmap_clf_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9235 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/data_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    10787 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/roi_features_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9121 2024-04-25 13:46:55.000000 Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/pup_retrieval_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5577 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/boolean_conditional_slicer_pup_up.py
--rw-r--r--   0 simon      (501) staff       (20)      584 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/about_simba_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5451 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9419 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1821 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7312 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/directing_animal_to_bodypart_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6546 2024-02-16 01:12:37.000000 Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)   118245 2024-05-17 17:07:17.000000 Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/video_processing_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7800 2024-04-04 16:47:32.000000 Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6160 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/clf_by_roi_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4470 2024-04-22 13:59:07.000000 Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/make_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3622 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/direction_animal_to_bodypart_settings_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6166 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1072 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/archive_files_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4716 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/pose_bp_drop_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    12174 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/distance_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4673 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3651 2024-04-26 18:13:38.000000 Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4134 2024-03-31 17:07:13.000000 Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    16701 2024-02-08 00:53:55.000000 Simba-UW-tf-dev-1.92.4/simba/ui/video_info_ui.py
--rw-r--r--   0 simon      (501) staff       (20)     6573 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.92.4/simba/ui/user_defined_pose_creator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/ui/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    14374 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.92.4/simba/ui/create_project_ui.py
--rw-r--r--   0 simon      (501) staff       (20)    14487 2024-02-08 00:53:55.000000 Simba-UW-tf-dev-1.92.4/simba/ui/tkinter_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    38871 2024-04-16 13:37:42.000000 Simba-UW-tf-dev-1.92.4/simba/ui/machine_model_settings_ui.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-18 15:52:47.000000 Simba-UW-tf-dev-1.92.4/simba/labelling/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/labelling/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    24423 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/labelling/labelling_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     2362 2024-02-21 02:33:04.000000 Simba-UW-tf-dev-1.92.4/simba/labelling/targeted_annotations_clips.py
--rw-r--r--   0 simon      (501) staff       (20)     3974 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/labelling/extract_labelled_frames.py
--rw-r--r--   0 simon      (501) staff       (20)    31269 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/labelling/labelling_advanced_interface.py
--rw-r--r--   0 simon      (501) staff       (20)    10012 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/labelling/play_annotation_video.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-18 15:52:47.000000 Simba-UW-tf-dev-1.92.4/simba/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)    15004 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.92.4/simba/unsupervised/dbcv_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5077 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.92.4/simba/unsupervised/cluster_validation_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3645 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.92.4/simba/unsupervised/enums.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-03 14:33:55.000000 Simba-UW-tf-dev-1.92.4/simba/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     9036 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.92.4/simba/unsupervised/cluster_video_visualizer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-18 15:52:47.000000 Simba-UW-tf-dev-1.92.4/simba/unsupervised/pop_ups/
--rw-r--r--   0 simon      (501) staff       (20)     4642 2024-03-26 23:50:53.000000 Simba-UW-tf-dev-1.92.4/simba/unsupervised/pop_ups/cluster_videos_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     4027 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.92.4/simba/unsupervised/pop_ups/transform_cluster_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     5048 2024-02-15 23:45:22.000000 Simba-UW-tf-dev-1.92.4/simba/unsupervised/pop_ups/embedding_correlations_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-02 14:39:26.000000 Simba-UW-tf-dev-1.92.4/simba/unsupervised/pop_ups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     4070 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.92.4/simba/unsupervised/pop_ups/transform_dim_reduction_popup.py
--rw-r--r--   0 simon      (501) staff       (20)    11182 2024-02-15 23:45:22.000000 Simba-UW-tf-dev-1.92.4/simba/unsupervised/pop_ups/fit_dim_reduction_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     2546 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.92.4/simba/unsupervised/pop_ups/data_extractor_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     4536 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.92.4/simba/unsupervised/pop_ups/cluster_validation_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9305 2024-02-15 23:45:22.000000 Simba-UW-tf-dev-1.92.4/simba/unsupervised/pop_ups/fit_cluster_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     2574 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.92.4/simba/unsupervised/pop_ups/clusterer_comparison_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     6527 2024-03-26 23:50:53.000000 Simba-UW-tf-dev-1.92.4/simba/unsupervised/pop_ups/grid_search_visualizer_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     4332 2024-03-28 20:02:59.000000 Simba-UW-tf-dev-1.92.4/simba/unsupervised/pop_ups/cluster_xai_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     3820 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.92.4/simba/unsupervised/pop_ups/cluster_frequentist_stats_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     2355 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.92.4/simba/unsupervised/pop_ups/print_embedding_info_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     9946 2024-04-02 18:34:25.000000 Simba-UW-tf-dev-1.92.4/simba/unsupervised/dataset_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    12982 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.92.4/simba/unsupervised/unsupervised_main.py
--rw-r--r--   0 simon      (501) staff       (20)    10175 2024-03-27 12:56:51.000000 Simba-UW-tf-dev-1.92.4/simba/unsupervised/grid_search_visualizers.py
--rw-r--r--   0 simon      (501) staff       (20)    16005 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.92.4/simba/unsupervised/data_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)     5241 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.92.4/simba/unsupervised/outlier_detector.py
--rw-r--r--   0 simon      (501) staff       (20)    10397 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.92.4/simba/unsupervised/cluster_frequentist_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5798 2024-03-27 12:56:51.000000 Simba-UW-tf-dev-1.92.4/simba/unsupervised/embedding_correlation_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/unsupervised/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18194 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.92.4/simba/unsupervised/cluster_xai_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    15581 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.92.4/simba/unsupervised/umap_embedder.py
--rw-r--r--   0 simon      (501) staff       (20)     5582 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.92.4/simba/unsupervised/clusterer_comparison_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     4652 2024-03-26 19:09:58.000000 Simba-UW-tf-dev-1.92.4/simba/unsupervised/bout_aggregator.py
--rw-r--r--   0 simon      (501) staff       (20)     2188 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/unsupervised/data_map.yaml
--rw-r--r--   0 simon      (501) staff       (20)    14765 2024-03-26 19:09:58.000000 Simba-UW-tf-dev-1.92.4/simba/unsupervised/hdbscan_clusterer.py
--rw-r--r--   0 simon      (501) staff       (20)     3862 2024-02-15 21:37:53.000000 Simba-UW-tf-dev-1.92.4/simba/unsupervised/tsne.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-18 15:52:47.000000 Simba-UW-tf-dev-1.92.4/simba/bounding_box_tools/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/bounding_box_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8511 2024-02-08 00:53:55.000000 Simba-UW-tf-dev-1.92.4/simba/bounding_box_tools/agg_boundary_stats.py
--rw-r--r--   0 simon      (501) staff       (20)    27255 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/bounding_box_tools/boundary_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    10064 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/bounding_box_tools/boundary_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     7146 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/bounding_box_tools/find_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    12066 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/bounding_box_tools/visualize_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    18436 2024-05-15 23:38:06.000000 Simba-UW-tf-dev-1.92.4/simba/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-18 15:52:47.000000 Simba-UW-tf-dev-1.92.4/simba/feature_extractors/
--rw-r--r--   0 simon      (501) staff       (20)    57052 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/feature_extractors/feature_extractor_14bp.py
--rw-r--r--   0 simon      (501) staff       (20)    28094 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/feature_extractors/feature_extractor_7bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-18 15:52:47.000000 Simba-UW-tf-dev-1.92.4/simba/feature_extractors/misc/
--rw-r--r--   0 simon      (501) staff       (20)     1757 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.92.4/simba/feature_extractors/misc/doctests.py
--rw-r--r--   0 simon      (501) staff       (20)    29328 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.92.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
--rw-r--r--   0 simon      (501) staff       (20)     2705 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.92.4/simba/feature_extractors/misc/read_in_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2689 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.92.4/simba/feature_extractors/misc/peaks.py
--rw-r--r--   0 simon      (501) staff       (20)    16727 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.92.4/simba/feature_extractors/misc/fish_feature_extractor_2022.py
--rw-r--r--   0 simon      (501) staff       (20)     2144 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.92.4/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
--rw-r--r--   0 simon      (501) staff       (20)     5762 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.92.4/simba/feature_extractors/misc/convex_hull_scratch_1.py
--rw-r--r--   0 simon      (501) staff       (20)    26425 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.92.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
--rw-r--r--   0 simon      (501) staff       (20)     7535 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.92.4/simba/feature_extractors/misc/egocentrical_aligner.py
--rw-r--r--   0 simon      (501) staff       (20)     1274 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.92.4/simba/feature_extractors/misc/count_values_in_range.py
--rw-r--r--   0 simon      (501) staff       (20)     5011 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.92.4/simba/feature_extractors/misc/graph_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     3954 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.92.4/simba/feature_extractors/misc/termite_rois.csv
--rw-r--r--   0 simon      (501) staff       (20)      736 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.92.4/simba/feature_extractors/misc/mutual_exclusive.py
--rw-r--r--   0 simon      (501) staff       (20)     2883 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.92.4/simba/feature_extractors/misc/video_color.py
--rw-r--r--   0 simon      (501) staff       (20)     2055 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.92.4/simba/feature_extractors/misc/graph_3d_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.92.4/simba/feature_extractors/misc/video_rotator.py
--rw-r--r--   0 simon      (501) staff       (20)     2932 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.92.4/simba/feature_extractors/misc/add_probability_cnt_features.py
--rw-r--r--   0 simon      (501) staff       (20)     1619 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.92.4/simba/feature_extractors/misc/make_splash.py
--rw-r--r--   0 simon      (501) staff       (20)    37024 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.92.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py
--rw-r--r--   0 simon      (501) staff       (20)     1613 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.92.4/simba/feature_extractors/misc/time_stamp_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.92.4/simba/feature_extractors/misc/video_rotator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    37022 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.92.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
--rw-r--r--   0 simon      (501) staff       (20)     2068 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.92.4/simba/feature_extractors/misc/convex_hull_scratch_2.py
--rw-r--r--   0 simon      (501) staff       (20)    36307 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/feature_extractors/feature_extractor_8bps_2_animals.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-02-21 02:05:27.000000 Simba-UW-tf-dev-1.92.4/simba/feature_extractors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     4091 2024-02-16 21:14:07.000000 Simba-UW-tf-dev-1.92.4/simba/feature_extractors/perimeter_jit.py
--rw-r--r--   0 simon      (501) staff       (20)    26471 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/feature_extractors/feature_subsets.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/feature_extractors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    10043 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/feature_extractors/feature_extractor_user_defined.py
--rw-r--r--   0 simon      (501) staff       (20)    61607 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/feature_extractors/feature_extractor_16bp.py
--rw-r--r--   0 simon      (501) staff       (20)    37328 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/feature_extractors/feature_extractor_9bp.py
--rw-r--r--   0 simon      (501) staff       (20)    31163 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/feature_extractors/feature_extractor_8bp.py
--rw-r--r--   0 simon      (501) staff       (20)    21427 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/feature_extractors/feature_extractor_4bp.py
--rw-r--r--   0 simon      (501) staff       (20)    65534 2024-03-01 16:55:51.000000 Simba-UW-tf-dev-1.92.4/simba/feature_extractors/amber_feature_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)     1033 2024-04-11 12:52:35.000000 Simba-UW-tf-dev-1.92.4/simba/requirements.txt
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-18 15:52:47.000000 Simba-UW-tf-dev-1.92.4/simba/mixins/
--rw-r--r--   0 simon      (501) staff       (20)    40917 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/mixins/annotator_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    84123 2024-05-09 15:16:46.000000 Simba-UW-tf-dev-1.92.4/simba/mixins/timeseries_features_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-03 14:38:30.000000 Simba-UW-tf-dev-1.92.4/simba/mixins/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    53232 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.92.4/simba/mixins/pop_up_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    47980 2024-05-09 16:28:06.000000 Simba-UW-tf-dev-1.92.4/simba/mixins/config_reader.py
--rw-r--r--   0 simon      (501) staff       (20)    56304 2024-04-17 23:32:32.000000 Simba-UW-tf-dev-1.92.4/simba/mixins/circular_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    38682 2024-05-14 17:44:58.000000 Simba-UW-tf-dev-1.92.4/simba/mixins/network_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/mixins/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    24040 2024-04-18 18:35:47.000000 Simba-UW-tf-dev-1.92.4/simba/mixins/pose_importer_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     3020 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/mixins/video_processing_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    35785 2024-05-09 15:22:35.000000 Simba-UW-tf-dev-1.92.4/simba/mixins/feature_extraction_supplement_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)   181387 2024-05-17 20:42:23.000000 Simba-UW-tf-dev-1.92.4/simba/mixins/statistics_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    44711 2024-04-22 19:40:36.000000 Simba-UW-tf-dev-1.92.4/simba/mixins/feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    69908 2024-05-06 18:32:12.000000 Simba-UW-tf-dev-1.92.4/simba/mixins/plotting_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)      391 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/mixins/abstract_classes.py
--rw-r--r--   0 simon      (501) staff       (20)    62121 2024-05-02 14:32:34.000000 Simba-UW-tf-dev-1.92.4/simba/mixins/image_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)      880 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.92.4/simba/mixins/unsupervised_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)   133234 2024-05-08 23:47:18.000000 Simba-UW-tf-dev-1.92.4/simba/mixins/train_model_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)   167515 2024-05-09 16:36:03.000000 Simba-UW-tf-dev-1.92.4/simba/mixins/geometry_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    24978 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/mixins/feature_extraction_circular_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-18 15:52:47.000000 Simba-UW-tf-dev-1.92.4/simba/third_party_label_appenders/
--rw-r--r--   0 simon      (501) staff       (20)     6639 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/third_party_label_appenders/deepethogram_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    12306 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/third_party_label_appenders/BORIS_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     9739 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/third_party_label_appenders/observer_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-22 19:49:42.000000 Simba-UW-tf-dev-1.92.4/simba/third_party_label_appenders/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     5508 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/third_party_label_appenders/boris_source_cleaner.py
--rw-r--r--   0 simon      (501) staff       (20)    18963 2024-04-26 14:35:34.000000 Simba-UW-tf-dev-1.92.4/simba/third_party_label_appenders/tools.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/third_party_label_appenders/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    17344 2024-04-26 18:13:38.000000 Simba-UW-tf-dev-1.92.4/simba/third_party_label_appenders/third_party_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     9215 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/third_party_label_appenders/ethovision_import.py
--rw-r--r--   0 simon      (501) staff       (20)     7456 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/third_party_label_appenders/BENTO_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     5662 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/third_party_label_appenders/solomon_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-18 15:52:47.000000 Simba-UW-tf-dev-1.92.4/simba/cue_light_tools/
--rw-r--r--   0 simon      (501) staff       (20)     8841 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/cue_light_tools/cue_light_clf_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    14451 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/cue_light_tools/cue_light_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    18274 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/cue_light_tools/cue_light_menues.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/cue_light_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1921 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/cue_light_tools/cue_light_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    19237 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/cue_light_tools/cue_light_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    15281 2024-04-25 13:46:55.000000 Simba-UW-tf-dev-1.92.4/simba/cue_light_tools/cue_light_movement_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-18 15:52:47.000000 Simba-UW-tf-dev-1.92.4/simba/utils/
--rw-r--r--   0 simon      (501) staff       (20)    13211 2024-02-16 01:12:37.000000 Simba-UW-tf-dev-1.92.4/simba/utils/config_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    26136 2024-05-09 20:56:18.000000 Simba-UW-tf-dev-1.92.4/simba/utils/enums.py
--rw-r--r--   0 simon      (501) staff       (20)    10420 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.92.4/simba/utils/custom_feature_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-25 18:17:26.000000 Simba-UW-tf-dev-1.92.4/simba/utils/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7734 2024-05-08 13:50:22.000000 Simba-UW-tf-dev-1.92.4/simba/utils/warnings.py
--rw-r--r--   0 simon      (501) staff       (20)    56026 2024-05-14 14:03:50.000000 Simba-UW-tf-dev-1.92.4/simba/utils/checks.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/utils/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    79930 2024-05-16 13:13:35.000000 Simba-UW-tf-dev-1.92.4/simba/utils/read_write.py
--rw-r--r--   0 simon      (501) staff       (20)    17201 2024-05-14 11:12:57.000000 Simba-UW-tf-dev-1.92.4/simba/utils/lookups.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-18 15:52:47.000000 Simba-UW-tf-dev-1.92.4/simba/utils/cli/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/utils/cli/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     7129 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/utils/cli/cli_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    17086 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/utils/errors.py
--rw-r--r--   0 simon      (501) staff       (20)    46270 2024-04-26 16:10:44.000000 Simba-UW-tf-dev-1.92.4/simba/utils/data.py
--rw-r--r--   0 simon      (501) staff       (20)     4205 2024-02-21 03:51:46.000000 Simba-UW-tf-dev-1.92.4/simba/utils/printing.py
--rw-r--r--   0 simon      (501) staff       (20)   243998 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/SimBA_logo.ico
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-18 15:52:47.000000 Simba-UW-tf-dev-1.92.4/simba/pose_processors/
--rw-r--r--   0 simon      (501) staff       (20)     8626 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/pose_processors/reorganize_keypoint.py
--rw-r--r--   0 simon      (501) staff       (20)     5840 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/pose_processors/remove_keypoints.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/pose_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2872 2024-02-15 23:39:58.000000 Simba-UW-tf-dev-1.92.4/simba/pose_processors/pose_reset.py
--rw-r--r--   0 simon      (501) staff       (20)     6313 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/pose_processors/reverse_pose.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-18 15:52:47.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/
--rw-r--r--   0 simon      (501) staff       (20)      786 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/doctests.py
--rw-r--r--   0 simon      (501) staff       (20)    29328 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/fish_feature_extractor_2023_version_3.py
--rw-r--r--   0 simon      (501) staff       (20)     4080 2024-05-06 15:09:47.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/CLAHE.py
--rw-r--r--   0 simon      (501) staff       (20)     2387 2024-03-08 14:35:02.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/dprime.py
--rw-r--r--   0 simon      (501) staff       (20)     3869 2024-05-14 18:18:20.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/ffmpeg_progress_bar.py
--rw-r--r--   0 simon      (501) staff       (20)     2516 2024-03-18 17:01:43.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/linear_fretchet.py
--rw-r--r--   0 simon      (501) staff       (20)     2705 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/read_in_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2391 2024-03-14 12:45:59.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/piotr_120324 3.py.zip
--rw-r--r--   0 simon      (501) staff       (20)     2036 2024-03-28 18:29:59.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/dunn_index.py
--rw-r--r--   0 simon      (501) staff       (20)     3640 2024-04-08 13:30:56.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/hausdorff.py
--rw-r--r--   0 simon      (501) staff       (20)     2689 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/peaks.py
--rw-r--r--   0 simon      (501) staff       (20)    16727 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/fish_feature_extractor_2022.py
--rw-r--r--   0 simon      (501) staff       (20)     3494 2024-04-03 13:42:02.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/colinear_features.py
--rw-r--r--   0 simon      (501) staff       (20)     8921 2024-03-22 13:56:46.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/spontaneous_alternation_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    21658 2024-04-10 16:31:38.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/horizontal_videos_concat.py
--rw-r--r--   0 simon      (501) staff       (20)     2144 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/convex_hull_3_scratch_3.py
--rw-r--r--   0 simon      (501) staff       (20)     1103 2024-03-29 16:26:34.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/silhouette_score.py
--rw-r--r--   0 simon      (501) staff       (20)     3607 2024-04-09 14:21:58.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/two_fish_feature_extractor_040924.py.zip
--rw-r--r--   0 simon      (501) staff       (20)    33092 2024-02-22 15:57:45.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/cuda_jit.ipynb
--rw-r--r--   0 simon      (501) staff       (20)     5762 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/convex_hull_scratch_1.py
--rw-r--r--   0 simon      (501) staff       (20)     1867 2024-03-12 19:23:40.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/directed_hausdorff.py
--rw-r--r--   0 simon      (501) staff       (20)      963 2024-03-13 18:20:52.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/shannon_diversity_index.py
--rw-r--r--   0 simon      (501) staff       (20)     3726 2024-03-12 13:31:58.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/sequential_lag_analysis.py
--rw-r--r--   0 simon      (501) staff       (20)     1254 2024-03-13 16:09:50.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/wilcoxon.py
--rw-r--r--   0 simon      (501) staff       (20)    21599 2024-04-22 16:40:51.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/ROI_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-25 14:48:22.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      549 2024-05-14 19:00:13.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/detect_scene_changes.py
--rw-r--r--   0 simon      (501) staff       (20)     3328 2024-03-08 15:05:36.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/data.npy
--rw-r--r--   0 simon      (501) staff       (20)    12626 2024-03-25 20:59:27.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/distances.py
--rw-r--r--   0 simon      (501) staff       (20)    26425 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/fish_feature_extractor_2023_version_2.py
--rw-r--r--   0 simon      (501) staff       (20)     2623 2024-05-03 16:20:12.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/cohens_kappa.py
--rw-r--r--   0 simon      (501) staff       (20)     4950 2024-05-14 14:14:15.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/watermark.py
--rw-r--r--   0 simon      (501) staff       (20)     2465 2024-03-08 17:38:19.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/paths.py
--rw-r--r--   0 simon      (501) staff       (20)     1048 2024-03-13 14:41:23.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/outliers_tietjen.py
--rw-r--r--   0 simon      (501) staff       (20)     1424 2024-02-26 15:46:14.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/train_model.py
--rw-r--r--   0 simon      (501) staff       (20)     2346 2024-04-19 14:10:16.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/img_stack_to_bw.py
--rw-r--r--   0 simon      (501) staff       (20)     3171 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/amber_tests.py
--rw-r--r--   0 simon      (501) staff       (20)     3590 2024-03-11 17:05:31.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/line_locate_point.py
--rw-r--r--   0 simon      (501) staff       (20)     1841 2024-04-19 16:19:10.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/sorensen_dice_coefficient.py
--rw-r--r--   0 simon      (501) staff       (20)     3182 2024-02-24 20:57:19.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/multifrm_to_points.py
--rw-r--r--   0 simon      (501) staff       (20)      959 2024-05-16 13:12:21.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/clean_sleap_filename.py
--rw-r--r--   0 simon      (501) staff       (20)       69 2024-03-18 18:17:24.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/lcs.py
--rw-r--r--   0 simon      (501) staff       (20)    12448 2024-04-09 14:14:37.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/two_fish_feature_extractor_040924.py
--rw-r--r--   0 simon      (501) staff       (20)     6119 2024-04-20 17:58:22.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/ez_path_plot.py
--rw-r--r--   0 simon      (501) staff       (20)     7535 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/egocentrical_aligner.py
--rw-r--r--   0 simon      (501) staff       (20)     5109 2024-05-07 19:36:44.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/downsample_video_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     2350 2024-03-12 17:58:33.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/add_body_part.py
--rw-r--r--   0 simon      (501) staff       (20)     1008 2024-03-12 13:29:20.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/grubbs_test.py
--rw-r--r--   0 simon      (501) staff       (20)     3399 2024-02-16 01:12:37.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/slide_circ_mean.py
--rw-r--r--   0 simon      (501) staff       (20)     1835 2024-03-28 22:56:59.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/calinski_harabasz.py
--rw-r--r--   0 simon      (501) staff       (20)     1282 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/roi_feature_visualizer_example.py
--rw-r--r--   0 simon      (501) staff       (20)    10076 2024-03-22 16:51:40.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/spontaneuous_alternation_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)      895 2024-03-12 14:09:55.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/runs_test.py
--rw-r--r--   0 simon      (501) staff       (20)     2516 2024-04-06 11:33:24.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/pct_counts_in_top_N.py
--rw-r--r--   0 simon      (501) staff       (20)     1095 2024-04-19 18:37:50.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/concordance_ratio.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:46:33.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2287 2024-03-25 16:45:04.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/total_variation_distance.py
--rw-r--r--   0 simon      (501) staff       (20)     3056 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/crop_single_polygon.py
--rw-r--r--   0 simon      (501) staff       (20)    15977 2024-04-23 22:52:42.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/ROI_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     8010 2024-03-24 19:48:22.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/joint_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     1529 2024-04-19 15:08:24.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/segment_image_horizontal.py
--rw-r--r--   0 simon      (501) staff       (20)    11145 2024-04-15 15:02:56.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/clip_multiple_videos_by_frame_numbers.py
--rw-r--r--   0 simon      (501) staff       (20)     2552 2024-04-02 14:48:59.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/elliptic_envelope.py
--rw-r--r--   0 simon      (501) staff       (20)     1016 2024-03-14 14:57:29.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/roi_definition_csvs_to_h5.py.zip
--rw-r--r--   0 simon      (501) staff       (20)     1276 2024-03-12 17:58:38.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/add_body_part.py.zip
--rw-r--r--   0 simon      (501) staff       (20)      921 2024-02-26 15:46:14.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/roi_feature_visualizer_example.py.zip
--rw-r--r--   0 simon      (501) staff       (20)     2631 2024-04-05 16:23:07.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/sliding_crosscorrelation.py
--rw-r--r--   0 simon      (501) staff       (20)     1274 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/count_values_in_range.py
--rw-r--r--   0 simon      (501) staff       (20)     2174 2024-03-14 14:56:26.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/roi_definition_csvs_to_h5.py
--rw-r--r--   0 simon      (501) staff       (20)     1656 2024-03-30 18:32:44.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/distance_velocity.py
--rw-r--r--   0 simon      (501) staff       (20)     5011 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/graph_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     5666 2024-04-11 15:28:58.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/line_plot_plotly.py
--rw-r--r--   0 simon      (501) staff       (20)     3838 2024-05-14 11:30:22.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/crossfade.py
--rw-r--r--   0 simon      (501) staff       (20)     3043 2024-05-09 15:04:30.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/shift_geometries.py
--rw-r--r--   0 simon      (501) staff       (20)     3954 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/termite_rois.csv
--rw-r--r--   0 simon      (501) staff       (20)     1785 2024-05-15 19:11:53.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/convert_to_bw.py
--rw-r--r--   0 simon      (501) staff       (20)     5254 2024-05-07 19:55:25.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/downsample_multiple_videos_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     1351 2024-03-26 21:10:40.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/unsupervised_lof.py
--rw-r--r--   0 simon      (501) staff       (20)     2553 2024-03-11 15:09:38.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/siegel_tukey.py
--rw-r--r--   0 simon      (501) staff       (20)      958 2024-03-13 18:05:08.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/berger_parker.py
--rw-r--r--   0 simon      (501) staff       (20)     4177 2024-04-10 01:56:43.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/isolation_forest.py
--rw-r--r--   0 simon      (501) staff       (20)     2845 2024-03-28 19:23:54.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/davis_bouldin.py
--rw-r--r--   0 simon      (501) staff       (20)     4094 2024-04-10 14:09:54.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/vertical_video_concatenator.py
--rw-r--r--   0 simon      (501) staff       (20)     2770 2024-04-07 19:14:13.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/batch_video_to_greyscale.py
--rw-r--r--   0 simon      (501) staff       (20)     7215 2024-02-26 15:46:14.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/crop_circles_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1410 2024-03-19 12:49:24.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/heading.py
--rw-r--r--   0 simon      (501) staff       (20)     2243 2024-03-13 18:35:02.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/piotr_120324 2.py.zip
--rw-r--r--   0 simon      (501) staff       (20)      736 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/mutual_exclusive.py
--rw-r--r--   0 simon      (501) staff       (20)     2278 2024-05-04 19:11:33.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/mahalanobis.py
--rw-r--r--   0 simon      (501) staff       (20)     1626 2024-05-08 16:59:35.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/superpixels.py
--rw-r--r--   0 simon      (501) staff       (20)     2225 2024-05-09 20:57:38.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/img_conv.py
--rw-r--r--   0 simon      (501) staff       (20)     2907 2024-03-14 19:31:25.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/grangercausalitytests.py
--rw-r--r--   0 simon      (501) staff       (20)     2432 2024-03-19 20:48:43.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/multiframe_is_shape_covered.py
--rw-r--r--   0 simon      (501) staff       (20)      592 2024-02-27 21:31:33.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/redis.py
--rw-r--r--   0 simon      (501) staff       (20)     2893 2024-02-26 20:49:33.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/video_color.py
--rw-r--r--   0 simon      (501) staff       (20)     2055 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/graph_3d_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     3137 2024-05-15 15:22:04.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/blurbox.py
--rw-r--r--   0 simon      (501) staff       (20)     6186 2024-03-18 12:44:45.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/piotr_120324.py
--rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/video_rotator.py
--rw-r--r--   0 simon      (501) staff       (20)     4166 2024-05-06 21:09:36.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/superimpose_frame_count.py
--rw-r--r--   0 simon      (501) staff       (20)     5433 2024-05-14 15:38:59.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/inset_overlay_video.py
--rw-r--r--   0 simon      (501) staff       (20)     1004 2024-03-12 13:11:45.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/hartley_fmax.py
--rw-r--r--   0 simon      (501) staff       (20)       84 2024-04-03 17:05:23.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/calc_N_degree_direction_switches.py
--rw-r--r--   0 simon      (501) staff       (20)     2307 2024-02-27 21:31:33.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/fix_clahe.py
--rw-r--r--   0 simon      (501) staff       (20)     1836 2024-03-10 15:38:46.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/cochran_q.py
--rw-r--r--   0 simon      (501) staff       (20)      682 2024-03-13 19:19:43.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/menhinicks_index.py
--rw-r--r--   0 simon      (501) staff       (20)      493 2024-05-02 16:25:29.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/lbp.py
--rw-r--r--   0 simon      (501) staff       (20)     2932 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/add_probability_cnt_features.py
--rw-r--r--   0 simon      (501) staff       (20)     1559 2024-04-19 15:50:37.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/brillouins_index.py
--rw-r--r--   0 simon      (501) staff       (20)    13575 2024-03-20 11:47:11.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/spontanous_alternations.py
--rw-r--r--   0 simon      (501) staff       (20)     1951 2024-05-03 14:45:28.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/eta_squared.py
--rw-r--r--   0 simon      (501) staff       (20)     2268 2024-03-13 13:59:07.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/piotr_120324.py.zip
--rw-r--r--   0 simon      (501) staff       (20)    16301 2024-05-13 14:59:18.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/convert_to_mp4.py
--rw-r--r--   0 simon      (501) staff       (20)     4655 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/velocity_aggregator.py
--rw-r--r--   0 simon      (501) staff       (20)     1619 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/make_splash.py
--rw-r--r--   0 simon      (501) staff       (20)     6440 2024-05-09 20:10:17.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/change_img_file_format.py
--rw-r--r--   0 simon      (501) staff       (20)     4478 2024-04-08 20:43:42.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/abod.py
--rw-r--r--   0 simon      (501) staff       (20)    37024 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/fish_feature_extractor_2023_version_5.py
--rw-r--r--   0 simon      (501) staff       (20)     1374 2024-04-18 13:56:20.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/violin.py
--rw-r--r--   0 simon      (501) staff       (20)    16527 2024-05-17 20:38:47.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/bg_substraction.py
--rw-r--r--   0 simon      (501) staff       (20)     1073 2024-03-13 16:46:16.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/simpson_diversity_index.py
--rw-r--r--   0 simon      (501) staff       (20)     4485 2024-04-14 19:07:54.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/clip_videos_by_frm.py
--rw-r--r--   0 simon      (501) staff       (20)      770 2024-05-02 20:50:37.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/fleiss_kappa.py
--rw-r--r--   0 simon      (501) staff       (20)     2396 2024-03-17 16:55:38.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/piotr_120324 4.py.zip
--rw-r--r--   0 simon      (501) staff       (20)    12282 2024-05-12 17:13:08.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/convert_to_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     1106 2024-04-18 13:46:43.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/rotate image.py
--rw-r--r--   0 simon      (501) staff       (20)     1214 2024-05-03 17:07:43.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/jaccard_distance.py
--rw-r--r--   0 simon      (501) staff       (20)     5336 2024-02-10 20:28:08.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/geometry_ex.py
--rw-r--r--   0 simon      (501) staff       (20)     1613 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/time_stamp_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     1505 2024-03-28 14:36:24.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/line_plot.py
--rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/video_rotator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15996 2024-04-09 13:41:30.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/unsupervised_outliers.py
--rw-r--r--   0 simon      (501) staff       (20)      122 2024-05-15 13:58:53.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/profiler.py
--rw-r--r--   0 simon      (501) staff       (20)     1378 2024-05-03 20:13:55.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/manhattan_distance.py
--rw-r--r--   0 simon      (501) staff       (20)     5690 2024-02-10 20:28:08.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/statistics_ex.py
--rw-r--r--   0 simon      (501) staff       (20)    16646 2024-04-22 16:43:10.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/ROI_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     1391 2024-03-18 23:21:46.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/sliding_displacement.py
--rw-r--r--   0 simon      (501) staff       (20)     7819 2024-04-18 14:47:28.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/path_plots.py
--rw-r--r--   0 simon      (501) staff       (20)     2671 2024-05-08 14:43:03.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/seekable.py
--rw-r--r--   0 simon      (501) staff       (20)     6572 2024-05-15 13:42:29.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/superimpose_elapsed_time.py
--rw-r--r--   0 simon      (501) staff       (20)      925 2024-03-11 13:06:04.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/wald_wolfowitz.py
--rw-r--r--   0 simon      (501) staff       (20)     2425 2024-05-03 15:57:50.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/relative_risk.py
--rw-r--r--   0 simon      (501) staff       (20)     1814 2024-04-05 14:36:58.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/sliding_autoc.py
--rw-r--r--   0 simon      (501) staff       (20)     2369 2024-03-14 17:07:10.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/linestring_path.py
--rw-r--r--   0 simon      (501) staff       (20)     2233 2024-03-18 15:20:48.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/cronbach_alpha.py
--rw-r--r--   0 simon      (501) staff       (20)     2809 2024-03-08 21:15:58.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/mcnamar.py
--rw-r--r--   0 simon      (501) staff       (20)     6507 2024-05-06 12:58:30.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/contrast.py
--rw-r--r--   0 simon      (501) staff       (20)    37022 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/fish_feature_extractor_2023_version_4.py
--rw-r--r--   0 simon      (501) staff       (20)     6220 2024-02-24 20:57:19.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/AmberFeatureExtractor.py.zip
--rw-r--r--   0 simon      (501) staff       (20)     1157 2024-05-02 20:32:28.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/youden_j.py
--rw-r--r--   0 simon      (501) staff       (20)     1933 2024-04-10 15:09:25.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/mosaic.py
--rw-r--r--   0 simon      (501) staff       (20)      441 2024-04-12 17:03:24.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/bouts_df
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-05-06 15:36:55.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/color_filtering.py
--rw-r--r--   0 simon      (501) staff       (20)    69423 2024-02-20 14:30:23.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/amber_featurizer.py
--rw-r--r--   0 simon      (501) staff       (20)     6286 2024-04-17 19:28:51.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/make_path_plot.py
--rw-r--r--   0 simon      (501) staff       (20)      837 2024-03-13 18:56:21.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/margalef_diversification_index.py
--rw-r--r--   0 simon      (501) staff       (20)      997 2024-03-17 17:49:00.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/biweight_midcorrelation.py
--rw-r--r--   0 simon      (501) staff       (20)     2186 2024-03-18 15:31:23.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/madmedianrule.py
--rw-r--r--   0 simon      (501) staff       (20)     2915 2024-04-01 14:12:59.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/adjusted_rand_score.py
--rw-r--r--   0 simon      (501) staff       (20)     2068 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/convex_hull_scratch_2.py
--rw-r--r--   0 simon      (501) staff       (20)     1957 2024-04-12 14:55:03.000000 Simba-UW-tf-dev-1.92.4/simba/sandbox/plotly_gantt.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-18 15:52:47.000000 Simba-UW-tf-dev-1.92.4/simba/plotting/
--rw-r--r--   0 simon      (501) staff       (20)     8538 2024-02-23 18:25:51.000000 Simba-UW-tf-dev-1.92.4/simba/plotting/directing_animals_to_bodypart_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    10307 2024-05-06 15:39:18.000000 Simba-UW-tf-dev-1.92.4/simba/plotting/gantt_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-18 15:52:47.000000 Simba-UW-tf-dev-1.92.4/simba/plotting/tools/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:43:56.000000 Simba-UW-tf-dev-1.92.4/simba/plotting/tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     5946 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/plotting/tools/tkinter_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    23490 2024-04-29 16:23:41.000000 Simba-UW-tf-dev-1.92.4/simba/plotting/ROI_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-05-09 13:03:17.000000 Simba-UW-tf-dev-1.92.4/simba/plotting/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    19315 2024-05-08 18:11:04.000000 Simba-UW-tf-dev-1.92.4/simba/plotting/shap_agg_stats_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12956 2024-05-06 15:39:18.000000 Simba-UW-tf-dev-1.92.4/simba/plotting/gantt_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15819 2024-04-25 18:19:38.000000 Simba-UW-tf-dev-1.92.4/simba/plotting/heat_mapper_clf_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    10620 2024-04-26 18:13:38.000000 Simba-UW-tf-dev-1.92.4/simba/plotting/probability_plot_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     8987 2024-05-09 16:36:03.000000 Simba-UW-tf-dev-1.92.4/simba/plotting/circular_plotting.py
--rw-r--r--   0 simon      (501) staff       (20)    16960 2024-05-06 15:39:18.000000 Simba-UW-tf-dev-1.92.4/simba/plotting/plot_clf_results.py
--rw-r--r--   0 simon      (501) staff       (20)    10328 2024-04-25 15:48:10.000000 Simba-UW-tf-dev-1.92.4/simba/plotting/ez_path_plot.py
--rw-r--r--   0 simon      (501) staff       (20)    17432 2024-04-17 23:57:27.000000 Simba-UW-tf-dev-1.92.4/simba/plotting/plot_clf_results_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    21343 2024-04-29 18:50:27.000000 Simba-UW-tf-dev-1.92.4/simba/plotting/ROI_feature_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    14847 2024-05-06 15:39:18.000000 Simba-UW-tf-dev-1.92.4/simba/plotting/heat_mapper_location.py
--rw-r--r--   0 simon      (501) staff       (20)    13512 2024-04-26 18:13:38.000000 Simba-UW-tf-dev-1.92.4/simba/plotting/probability_plot_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/plotting/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     5253 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/plotting/interactive_probability_grapher.py
--rw-r--r--   0 simon      (501) staff       (20)     6517 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/plotting/plot_pose_in_dir.py
--rw-r--r--   0 simon      (501) staff       (20)    20950 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.92.4/simba/plotting/single_run_model_validation_video.py
--rw-r--r--   0 simon      (501) staff       (20)     8732 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.92.4/simba/plotting/frame_mergerer_ffmpeg.py
--rw-r--r--   0 simon      (501) staff       (20)    10667 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.92.4/simba/plotting/pose_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    16477 2024-04-25 18:30:53.000000 Simba-UW-tf-dev-1.92.4/simba/plotting/directing_animals_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11565 2024-04-28 20:02:42.000000 Simba-UW-tf-dev-1.92.4/simba/plotting/clf_validator.py
--rw-r--r--   0 simon      (501) staff       (20)    23459 2024-04-25 18:18:16.000000 Simba-UW-tf-dev-1.92.4/simba/plotting/path_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    24207 2024-05-07 12:24:30.000000 Simba-UW-tf-dev-1.92.4/simba/plotting/ROI_feature_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11824 2024-04-17 19:58:21.000000 Simba-UW-tf-dev-1.92.4/simba/plotting/data_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13091 2024-03-26 23:49:10.000000 Simba-UW-tf-dev-1.92.4/simba/plotting/spontaneous_alternation_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    21979 2024-04-25 18:18:16.000000 Simba-UW-tf-dev-1.92.4/simba/plotting/path_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    16926 2024-04-25 19:01:12.000000 Simba-UW-tf-dev-1.92.4/simba/plotting/distance_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    17511 2024-04-28 19:58:43.000000 Simba-UW-tf-dev-1.92.4/simba/plotting/ROI_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    10034 2024-03-19 12:54:07.000000 Simba-UW-tf-dev-1.92.4/simba/plotting/geometry_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    15989 2024-04-28 20:02:42.000000 Simba-UW-tf-dev-1.92.4/simba/plotting/clf_validator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    14224 2024-04-25 18:19:38.000000 Simba-UW-tf-dev-1.92.4/simba/plotting/heat_mapper_clf.py
--rw-r--r--   0 simon      (501) staff       (20)    11994 2024-04-11 22:38:54.000000 Simba-UW-tf-dev-1.92.4/simba/plotting/distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    19073 2024-04-11 20:26:33.000000 Simba-UW-tf-dev-1.92.4/simba/plotting/single_run_model_validation_video_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    12552 2024-04-25 18:30:28.000000 Simba-UW-tf-dev-1.92.4/simba/plotting/directing_animals_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)     9549 2024-05-09 16:36:03.000000 Simba-UW-tf-dev-1.92.4/simba/plotting/circular_feature_overlay_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    14663 2024-05-06 15:39:18.000000 Simba-UW-tf-dev-1.92.4/simba/plotting/heat_mapper_location_mp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-18 15:52:47.000000 Simba-UW-tf-dev-1.92.4/simba/dash_app/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:44:15.000000 Simba-UW-tf-dev-1.92.4/simba/dash_app/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    72715 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/dash_app/SimBA_dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     4965 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/dash_app/run_dash_tkinter.py
--rw-r--r--   0 simon      (501) staff       (20)    47546 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/dash_app/dash_app.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-18 15:52:47.000000 Simba-UW-tf-dev-1.92.4/simba/data_processors/
--rw-r--r--   0 simon      (501) staff       (20)    13060 2024-04-26 18:13:38.000000 Simba-UW-tf-dev-1.92.4/simba/data_processors/spontaneous_alternation_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    11813 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/data_processors/agg_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-21 11:48:06.000000 Simba-UW-tf-dev-1.92.4/simba/data_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    13224 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/data_processors/severity_bout_based_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    39110 2024-03-19 12:54:07.000000 Simba-UW-tf-dev-1.92.4/simba/data_processors/interpolation_smoothing.py
--rw-r--r--   0 simon      (501) staff       (20)    10968 2024-02-21 19:10:40.000000 Simba-UW-tf-dev-1.92.4/simba/data_processors/directing_animal_to_bodypart.py
--rw-r--r--   0 simon      (501) staff       (20)     9580 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/data_processors/timebins_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    20617 2024-04-18 21:13:37.000000 Simba-UW-tf-dev-1.92.4/simba/data_processors/fsttc_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/data_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     4872 2024-04-26 15:18:54.000000 Simba-UW-tf-dev-1.92.4/simba/data_processors/boolean_conditional_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     7117 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/data_processors/interpolate_pose.py
--rw-r--r--   0 simon      (501) staff       (20)    15989 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.92.4/simba/data_processors/directing_other_animals_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8957 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/data_processors/gibbs_sampler.py
--rw-r--r--   0 simon      (501) staff       (20)    10054 2024-04-04 16:23:22.000000 Simba-UW-tf-dev-1.92.4/simba/data_processors/timebins_movement_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5255 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/data_processors/severity_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    18517 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/data_processors/pup_retrieval_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3118 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/data_processors/pybursts_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    13660 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/data_processors/severity_frame_based_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8738 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/data_processors/mutual_exclusivity_corrector.py
--rw-r--r--   0 simon      (501) staff       (20)    12919 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/data_processors/kleinberg_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    10196 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/data_processors/movement_calculator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-18 15:52:47.000000 Simba-UW-tf-dev-1.92.4/simba/model/
--rw-r--r--   0 simon      (501) staff       (20)    21997 2024-05-08 23:53:08.000000 Simba-UW-tf-dev-1.92.4/simba/model/train_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     4969 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/model/inference_batch.py
--rw-r--r--   0 simon      (501) staff       (20)    14036 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/model/train_multiclass_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     3937 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/model/inference_multiclass_batch.py
--rw-r--r--   0 simon      (501) staff       (20)    15931 2024-02-20 14:30:06.000000 Simba-UW-tf-dev-1.92.4/simba/model/grid_search_multiclass_rf.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:41:19.000000 Simba-UW-tf-dev-1.92.4/simba/model/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    14317 2024-05-08 23:47:18.000000 Simba-UW-tf-dev-1.92.4/simba/model/grid_search_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     3768 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/model/inference_validation.py
--rw-r--r--   0 simon      (501) staff       (20)     6872 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/model/train_multilabel_rf.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-18 15:52:47.000000 Simba-UW-tf-dev-1.92.4/simba/roi_tools/
--rw-r--r--   0 simon      (501) staff       (20)    11039 2024-05-09 16:32:28.000000 Simba-UW-tf-dev-1.92.4/simba/roi_tools/ROI_time_bin_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-25 18:17:26.000000 Simba-UW-tf-dev-1.92.4/simba/roi_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    50014 2024-05-17 13:19:01.000000 Simba-UW-tf-dev-1.92.4/simba/roi_tools/ROI_define.py
--rw-r--r--   0 simon      (501) staff       (20)     3616 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/roi_tools/ROI_reset.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/roi_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     9876 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/roi_tools/ROI_size_standardizer.py
--rw-r--r--   0 simon      (501) staff       (20)    18552 2024-05-09 16:13:09.000000 Simba-UW-tf-dev-1.92.4/simba/roi_tools/ROI_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    15406 2024-05-07 01:16:15.000000 Simba-UW-tf-dev-1.92.4/simba/roi_tools/ROI_feature_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     4386 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/roi_tools/ROI_multiply.py
--rw-r--r--   0 simon      (501) staff       (20)     2313 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/roi_tools/ROI_size_calculations.py
--rw-r--r--   0 simon      (501) staff       (20)     3716 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/roi_tools/ROI_zoom.py
--rw-r--r--   0 simon      (501) staff       (20)    12313 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.92.4/simba/roi_tools/ROI_directing_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    11974 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/roi_tools/ROI_move_shape.py
--rw-r--r--   0 simon      (501) staff       (20)     5470 2024-02-21 03:51:46.000000 Simba-UW-tf-dev-1.92.4/simba/roi_tools/ROI_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    16129 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/roi_tools/ROI_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    29746 2024-05-17 13:17:50.000000 Simba-UW-tf-dev-1.92.4/simba/roi_tools/ROI_image.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-18 15:52:47.000000 Simba-UW-tf-dev-1.92.4/simba/pose_importers/
--rw-r--r--   0 simon      (501) staff       (20)    10711 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.92.4/simba/pose_importers/sleap_csv_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-18 15:52:47.000000 Simba-UW-tf-dev-1.92.4/simba/pose_importers/misc/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:31.000000 Simba-UW-tf-dev-1.92.4/simba/pose_importers/misc/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8084 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/pose_importers/misc/apt_trk_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     2577 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/pose_importers/read_DANNCE_mat.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-22 19:49:42.000000 Simba-UW-tf-dev-1.92.4/simba/pose_importers/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    13867 2024-05-16 18:24:39.000000 Simba-UW-tf-dev-1.92.4/simba/pose_importers/sleap_h5_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     8161 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/pose_importers/madlc_importer.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/pose_importers/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    13672 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.92.4/simba/pose_importers/sleap_slp_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     8645 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/pose_importers/import_mars.py
--rw-r--r--   0 simon      (501) staff       (20)     7464 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/pose_importers/dlc_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)     8417 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/pose_importers/trk_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-18 15:52:47.000000 Simba-UW-tf-dev-1.92.4/simba/pose_configurations/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2024-03-19 18:18:43.000000 Simba-UW-tf-dev-1.92.4/simba/pose_configurations/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-18 15:52:47.000000 Simba-UW-tf-dev-1.92.4/simba/pose_configurations/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:10.000000 Simba-UW-tf-dev-1.92.4/simba/pose_configurations/bp_names/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     4485 2024-03-04 19:10:54.000000 Simba-UW-tf-dev-1.92.4/simba/pose_configurations/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-18 15:52:47.000000 Simba-UW-tf-dev-1.92.4/simba/pose_configurations/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       27 2024-03-04 19:10:54.000000 Simba-UW-tf-dev-1.92.4/simba/pose_configurations/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:18.000000 Simba-UW-tf-dev-1.92.4/simba/pose_configurations/no_animals/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:05.000000 Simba-UW-tf-dev-1.92.4/simba/pose_configurations/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-18 15:52:47.000000 Simba-UW-tf-dev-1.92.4/simba/pose_configurations/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:14.000000 Simba-UW-tf-dev-1.92.4/simba/pose_configurations/configuration_names/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)      273 2024-03-04 19:10:54.000000 Simba-UW-tf-dev-1.92.4/simba/pose_configurations/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-18 15:52:47.000000 Simba-UW-tf-dev-1.92.4/simba/pose_configurations/schematics/
--rw-r--r--   0 simon      (501) staff       (20)    39805 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/pose_configurations/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/pose_configurations/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/pose_configurations/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    34231 2024-02-20 18:50:39.000000 Simba-UW-tf-dev-1.92.4/simba/pose_configurations/schematics/13.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/pose_configurations/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/pose_configurations/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/pose_configurations/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/pose_configurations/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/pose_configurations/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/pose_configurations/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/pose_configurations/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/pose_configurations/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/pose_configurations/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-18 15:52:47.000000 Simba-UW-tf-dev-1.92.4/simba/video_processors/
--rw-r--r--   0 simon      (501) staff       (20)   190333 2024-05-17 21:09:49.000000 Simba-UW-tf-dev-1.92.4/simba/video_processors/video_processing.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-05-15 15:29:21.000000 Simba-UW-tf-dev-1.92.4/simba/video_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     5577 2024-04-08 11:29:52.000000 Simba-UW-tf-dev-1.92.4/simba/video_processors/roi_selector_circle.py
--rw-r--r--   0 simon      (501) staff       (20)     9073 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/video_processors/px_to_mm.py
--rw-r--r--   0 simon      (501) staff       (20)    35053 2024-02-26 15:42:07.000000 Simba-UW-tf-dev-1.92.4/simba/video_processors/batch_process_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    11439 2024-05-14 20:38:00.000000 Simba-UW-tf-dev-1.92.4/simba/video_processors/multi_cropper.py
--rw-r--r--   0 simon      (501) staff       (20)     3066 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/video_processors/extract_frames.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/video_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     6598 2024-02-26 21:50:01.000000 Simba-UW-tf-dev-1.92.4/simba/video_processors/roi_selector.py
--rw-r--r--   0 simon      (501) staff       (20)    10007 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/video_processors/calculate_px_dist.py
--rw-r--r--   0 simon      (501) staff       (20)     3674 2024-05-06 19:29:28.000000 Simba-UW-tf-dev-1.92.4/simba/video_processors/brightness_contrast_ui.py
--rw-r--r--   0 simon      (501) staff       (20)     5963 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.92.4/simba/video_processors/roi_selector_polygon.py
--rw-r--r--   0 simon      (501) staff       (20)     4926 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/video_processors/extract_seqframes.py
--rw-r--r--   0 simon      (501) staff       (20)    15117 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.92.4/simba/video_processors/batch_process_create_ffmpeg_commands.py
--rw-r--r--   0 simon      (501) staff       (20)     3595 2024-05-06 15:51:58.000000 Simba-UW-tf-dev-1.92.4/simba/video_processors/clahe_ui.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-18 15:52:47.000000 Simba-UW-tf-dev-1.92.4/simba/outlier_tools/
--rw-r--r--   0 simon      (501) staff       (20)     7837 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/outlier_tools/outlier_corrector_movement.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/outlier_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    14462 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/outlier_tools/outlier_corrector_location_advanced.py
--rw-r--r--   0 simon      (501) staff       (20)    13117 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/outlier_tools/outlier_corrector_movement_advanced.py
--rw-r--r--   0 simon      (501) staff       (20)    10396 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/outlier_tools/outlier_corrector_location.py
--rw-r--r--   0 simon      (501) staff       (20)     2751 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/outlier_tools/skip_outlier_correction.py
--rw-r--r--   0 simon      (501) staff       (20)    83331 2024-05-13 18:56:03.000000 Simba-UW-tf-dev-1.92.4/simba/SimBA.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-18 15:52:47.000000 Simba-UW-tf-dev-1.92.4/simba/assets/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-18 15:52:47.000000 Simba-UW-tf-dev-1.92.4/simba/assets/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)   109483 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/unsupervised/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:36.000000 Simba-UW-tf-dev-1.92.4/simba/assets/unsupervised/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    14175 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/unsupervised/features.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-18 15:52:47.000000 Simba-UW-tf-dev-1.92.4/simba/assets/shap/
--rw-r--r--   0 simon      (501) staff       (20)     1177 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/shap/down_arrow.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1733 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/shap/intruder_shape.jpg
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-18 15:52:47.000000 Simba-UW-tf-dev-1.92.4/simba/assets/shap/feature_categories/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:25.000000 Simba-UW-tf-dev-1.92.4/simba/assets/shap/feature_categories/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    17420 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/shap/feature_categories/shap_feature_categories.csv
--rw-r--r--   0 simon      (501) staff       (20)     1665 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/shap/resident_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2415 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/shap/resident_intruder_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2012 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/shap/animal_distances.jpg
--rw-r--r--   0 simon      (501) staff       (20)     4422 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/shap/baseline_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:21.000000 Simba-UW-tf-dev-1.92.4/simba/assets/shap/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)   353824 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/shap/ubuntu.regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     6672 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/shap/side_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   189004 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/shap/UbuntuMono-Regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     2737 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/shap/side_scale_5.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1785 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/shap/intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1435 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/shap/resident_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     3134 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/shap/color_bar.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2120 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/shap/resident_intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)    10244 2024-05-14 12:52:17.000000 Simba-UW-tf-dev-1.92.4/simba/assets/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-18 15:52:47.000000 Simba-UW-tf-dev-1.92.4/simba/assets/lookups/
--rw-r--r--   0 simon      (501) staff       (20)   270783 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/lookups/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)     2987 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/lookups/feature_extraction_headers.csv
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:11.000000 Simba-UW-tf-dev-1.92.4/simba/assets/lookups/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    26256 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/lookups/critical_values_05.pickle
--rw-r--r--   0 simon      (501) staff       (20)    14175 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/lookups/features.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/lookups/unsupervised_example_x.csv
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:41:54.000000 Simba-UW-tf-dev-1.92.4/simba/assets/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-18 15:52:47.000000 Simba-UW-tf-dev-1.92.4/simba/assets/stl/
--rw-r--r--   0 simon      (501) staff       (20)   551576 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/stl/operant_tray.stl
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:31.000000 Simba-UW-tf-dev-1.92.4/simba/assets/stl/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    67647 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/stl/operant_lever.stl
--rw-r--r--   0 simon      (501) staff       (20)    92896 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/stl/operant_walls.stl
--rw-r--r--   0 simon      (501) staff       (20)  4759984 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/stl/grid_floor.stl
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-18 15:52:47.000000 Simba-UW-tf-dev-1.92.4/simba/assets/img/
--rw-r--r--   0 simon      (501) staff       (20)   489479 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/img/splash_2024.mp4
--rw-r--r--   0 simon      (501) staff       (20)    79863 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/img/bg_2024.png
--rw-r--r--   0 simon      (501) staff       (20)   399272 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/img/about_me.png
--rw-r--r--   0 simon      (501) staff       (20)   117108 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/img/splash.mp4
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:02.000000 Simba-UW-tf-dev-1.92.4/simba/assets/img/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)   322242 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/img/bg_2.png
--rw-r--r--   0 simon      (501) staff       (20)      165 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/img/~$splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)    69267 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/img/splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)   204362 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/img/bg.png
--rw-r--r--   0 simon      (501) staff       (20)   189004 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/UbuntuMono-Regular.ttf
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-18 15:52:47.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/
--rw-r--r--   0 simon      (501) staff       (20)     1350 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/factory.png
--rw-r--r--   0 simon      (501) staff       (20)     1413 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/cluster.png
--rw-r--r--   0 simon      (501) staff       (20)     1340 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/load.png
--rw-r--r--   0 simon      (501) staff       (20)     4507 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/gif.png
--rw-r--r--   0 simon      (501) staff       (20)     4566 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/pose.png
--rw-r--r--   0 simon      (501) staff       (20)     1943 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/features.png
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-09 15:42:22.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     4896 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/settings.png
--rw-r--r--   0 simon      (501) staff       (20)     2090 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/stopwatch.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/link.png
--rw-r--r--   0 simon      (501) staff       (20)    14250 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/dash_simba.css
--rw-r--r--   0 simon      (501) staff       (20)      917 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/documentation.png
--rw-r--r--   0 simon      (501) staff       (20)     4503 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/fps.png
--rw-r--r--   0 simon      (501) staff       (20)     1299 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/dimensionality_reduction.png
--rw-r--r--   0 simon      (501) staff       (20)     4823 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/roi.png
--rw-r--r--   0 simon      (501) staff       (20)   171446 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/simba_logo_2.png
--rw-r--r--   0 simon      (501) staff       (20)      920 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/superimpose.png
--rw-r--r--   0 simon      (501) staff       (20)     1136 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/label.png
--rw-r--r--   0 simon      (501) staff       (20)     1016 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/change.png
--rw-r--r--   0 simon      (501) staff       (20)    59896 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/readthedocs_logo.png
--rw-r--r--   0 simon      (501) staff       (20)     1124 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/crop.png
--rw-r--r--   0 simon      (501) staff       (20)     2146 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/rotate.png
--rw-r--r--   0 simon      (501) staff       (20)     1921 2024-02-26 14:29:54.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/circle.png
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:44:37.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1057 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/path.png
--rw-r--r--   0 simon      (501) staff       (20)     1148 2024-02-26 20:39:14.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/polygon.png
--rw-r--r--   0 simon      (501) staff       (20)      950 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/clip.png
--rw-r--r--   0 simon      (501) staff       (20)     2121 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/restart.png
--rw-r--r--   0 simon      (501) staff       (20)     4653 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/calipher.png
--rw-r--r--   0 simon      (501) staff       (20)     1291 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/add_on.png
--rw-r--r--   0 simon      (501) staff       (20)     4695 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/create.png
--rw-r--r--   0 simon      (501) staff       (20)    78182 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/SimBA_logo.ico
--rw-r--r--   0 simon      (501) staff       (20)     1067 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/print.png
--rw-r--r--   0 simon      (501) staff       (20)     4653 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/clf.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-18 15:52:47.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/concat_icons/
--rw-r--r--   0 simon      (501) staff       (20)     6027 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/concat_icons/mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     5654 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/concat_icons/vertical.png
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:44:45.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/concat_icons/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     5542 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/concat_icons/horizontal.png
--rw-r--r--   0 simon      (501) staff       (20)     5939 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/concat_icons/mixed_mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     4256 2024-05-06 13:20:42.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/brightness.png
--rw-r--r--   0 simon      (501) staff       (20)     2060 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/merge.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/clean.png
--rw-r--r--   0 simon      (501) staff       (20)     4725 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/clf_2.png
--rw-r--r--   0 simon      (501) staff       (20)     4795 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/visualize.png
--rw-r--r--   0 simon      (501) staff       (20)     2142 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/concat.png
--rw-r--r--   0 simon      (501) staff       (20)     1474 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/boris.png
--rw-r--r--   0 simon      (501) staff       (20)     4804 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/frames.png
--rw-r--r--   0 simon      (501) staff       (20)     2425 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/video.png
--rw-r--r--   0 simon      (501) staff       (20)     2089 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/sample.png
--rw-r--r--   0 simon      (501) staff       (20)     1471 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/metrics.png
--rw-r--r--   0 simon      (501) staff       (20)     4555 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/grey.png
--rw-r--r--   0 simon      (501) staff       (20)      930 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/exit.png
--rw-r--r--   0 simon      (501) staff       (20)     4751 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/outlier.png
--rw-r--r--   0 simon      (501) staff       (20)     4392 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/clahe.png
--rw-r--r--   0 simon      (501) staff       (20)     4637 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/trash.png
--rw-r--r--   0 simon      (501) staff       (20)     1239 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/about.png
--rw-r--r--   0 simon      (501) staff       (20)     4666 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/convert.png
--rw-r--r--   0 simon      (501) staff       (20)    93229 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/SimBA_logo.icns
--rw-r--r--   0 simon      (501) staff       (20)      991 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/reorganize.png
--rw-r--r--   0 simon      (501) staff       (20)     4784 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/browse.png
--rw-r--r--   0 simon      (501) staff       (20)    30707 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/SimBA_logo.png
--rw-r--r--   0 simon      (501) staff       (20)     2293 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/ethovision.png
--rw-r--r--   0 simon      (501) staff       (20)     1018 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/icons/close.png
--rw-r--r--   0 simon      (501) staff       (20)    13672 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/dash_simba_base.css
--rw-r--r--   0 simon      (501) staff       (20)    31812 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.4/simba/assets/TheGoldenLab.PNG
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-18 15:52:47.000000 Simba-UW-tf-dev-1.92.4/Simba_UW_tf_dev.egg-info/
--rw-r--r--   0 simon      (501) staff       (20)     2797 2024-05-18 15:52:46.000000 Simba-UW-tf-dev-1.92.4/Simba_UW_tf_dev.egg-info/PKG-INFO
--rw-r--r--   0 simon      (501) staff       (20)    24600 2024-05-18 15:52:46.000000 Simba-UW-tf-dev-1.92.4/Simba_UW_tf_dev.egg-info/SOURCES.txt
--rw-r--r--   0 simon      (501) staff       (20)       44 2024-05-18 15:52:46.000000 Simba-UW-tf-dev-1.92.4/Simba_UW_tf_dev.egg-info/entry_points.txt
--rw-r--r--   0 simon      (501) staff       (20)      857 2024-05-18 15:52:46.000000 Simba-UW-tf-dev-1.92.4/Simba_UW_tf_dev.egg-info/requires.txt
--rw-r--r--   0 simon      (501) staff       (20)        6 2024-05-18 15:52:46.000000 Simba-UW-tf-dev-1.92.4/Simba_UW_tf_dev.egg-info/top_level.txt
--rw-r--r--   0 simon      (501) staff       (20)        1 2024-05-18 15:52:46.000000 Simba-UW-tf-dev-1.92.4/Simba_UW_tf_dev.egg-info/dependency_links.txt
--rw-r--r--   0 simon      (501) staff       (20)    35127 2024-02-07 18:56:10.000000 Simba-UW-tf-dev-1.92.4/LICENSE
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-18 15:52:47.000000 Simba-UW-tf-dev-1.92.4/tests/
--rw-r--r--   0 simon      (501) staff       (20)     4753 2024-04-11 20:40:04.000000 Simba-UW-tf-dev-1.92.4/tests/test_data_processors.py
--rw-r--r--   0 simon      (501) staff       (20)    13415 2024-03-01 16:43:04.000000 Simba-UW-tf-dev-1.92.4/tests/test_circlular_stats.py
--rw-r--r--   0 simon      (501) staff       (20)    13399 2024-04-11 20:36:51.000000 Simba-UW-tf-dev-1.92.4/tests/test_stats.py
--rw-r--r--   0 simon      (501) staff       (20)    11863 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.92.4/tests/test_train_model_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     6525 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.92.4/tests/test_feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     1739 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.92.4/tests/test_utils_data.py
--rw-r--r--   0 simon      (501) staff       (20)     8120 2024-03-01 19:06:25.000000 Simba-UW-tf-dev-1.92.4/tests/test_config_reader_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     1070 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.92.4/tests/test_outlier_correctors.py
--rw-r--r--   0 simon      (501) staff       (20)     1596 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.92.4/tests/test_featurizers.py
--rw-r--r--   0 simon      (501) staff       (20)     8582 2024-05-12 17:13:08.000000 Simba-UW-tf-dev-1.92.4/tests/test_video_processors.py
--rw-r--r--   0 simon      (501) staff       (20)     3554 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.92.4/tests/test_thirdparty_appenders.py
--rw-r--r--   0 simon      (501) staff       (20)     3021 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.92.4/tests/test_validation_clips.py
--rw-r--r--   0 simon      (501) staff       (20)     3921 2024-04-26 17:59:40.000000 Simba-UW-tf-dev-1.92.4/tests/test_roi_tools.py
--rw-r--r--   0 simon      (501) staff       (20)      318 2024-03-04 20:16:28.000000 Simba-UW-tf-dev-1.92.4/MANIFEST.in
--rw-r--r--   0 simon      (501) staff       (20)    18478 2024-04-17 19:58:21.000000 Simba-UW-tf-dev-1.92.4/README.md
--rw-r--r--   0 simon      (501) staff       (20)     1426 2024-05-18 15:52:42.000000 Simba-UW-tf-dev-1.92.4/setup.py
--rw-r--r--   0 simon      (501) staff       (20)       38 2024-05-18 15:52:47.000000 Simba-UW-tf-dev-1.92.4/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 17:55:13.000000 Simba-UW-tf-dev-1.92.5/
+-rw-r--r--   0 simon      (501) staff       (20)     2797 2024-05-19 17:55:13.000000 Simba-UW-tf-dev-1.92.5/PKG-INFO
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 17:55:12.000000 Simba-UW-tf-dev-1.92.5/simba/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 17:55:13.000000 Simba-UW-tf-dev-1.92.5/simba/ui/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-28 13:50:53.000000 Simba-UW-tf-dev-1.92.5/simba/ui/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 17:55:13.000000 Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/
+-rw-r--r--   0 simon      (501) staff       (20)    11467 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/mutual_exclusivity_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4070 2024-03-29 20:30:28.000000 Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1676 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/csv_2_parquet_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5883 2024-04-22 13:59:07.000000 Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/quick_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2873 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/batch_preprocess_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8831 2024-05-02 13:40:02.000000 Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/heatmap_location_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9578 2024-04-26 18:13:38.000000 Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/clf_probability_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3456 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/movement_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4631 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    11362 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/clf_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    25598 2024-04-17 23:32:48.000000 Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1184 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/remove_roi_features_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6692 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/targeted_annotation_clips_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3340 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2174 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/roi_size_standardizer_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     6997 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4682 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/roi_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7898 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/outlier_settings_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9366 2024-04-29 16:29:26.000000 Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/gantt_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5830 2024-04-26 18:09:47.000000 Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/clf_validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8529 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/severity_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3221 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/fsttc_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4231 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/kleinberg_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8376 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9785 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/spontaneous_alternation_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6076 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/pose_reorganizer_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3437 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/animal_directing_other_animals_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3352 2024-04-26 15:18:54.000000 Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3468 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/clf_by_timebins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9154 2024-04-12 00:32:53.000000 Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/heatmap_clf_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9235 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/data_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    10787 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/roi_features_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9121 2024-04-25 13:46:55.000000 Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/pup_retrieval_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5577 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/boolean_conditional_slicer_pup_up.py
+-rw-r--r--   0 simon      (501) staff       (20)      584 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/about_simba_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5451 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9419 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1821 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7312 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/directing_animal_to_bodypart_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6546 2024-02-16 01:12:37.000000 Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)   130051 2024-05-19 17:50:50.000000 Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/video_processing_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7800 2024-04-04 16:47:32.000000 Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6160 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/clf_by_roi_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4470 2024-04-22 13:59:07.000000 Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/make_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3622 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/direction_animal_to_bodypart_settings_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6166 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1072 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/archive_files_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4716 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/pose_bp_drop_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    12174 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/distance_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4673 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3651 2024-04-26 18:13:38.000000 Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4134 2024-03-31 17:07:13.000000 Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    16701 2024-02-08 00:53:55.000000 Simba-UW-tf-dev-1.92.5/simba/ui/video_info_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     6573 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.92.5/simba/ui/user_defined_pose_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/ui/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    14374 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.92.5/simba/ui/create_project_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)    14487 2024-02-08 00:53:55.000000 Simba-UW-tf-dev-1.92.5/simba/ui/tkinter_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    38871 2024-04-16 13:37:42.000000 Simba-UW-tf-dev-1.92.5/simba/ui/machine_model_settings_ui.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 17:55:12.000000 Simba-UW-tf-dev-1.92.5/simba/labelling/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/labelling/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    24423 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/labelling/labelling_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     2362 2024-02-21 02:33:04.000000 Simba-UW-tf-dev-1.92.5/simba/labelling/targeted_annotations_clips.py
+-rw-r--r--   0 simon      (501) staff       (20)     3974 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/labelling/extract_labelled_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)    31269 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/labelling/labelling_advanced_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)    10012 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/labelling/play_annotation_video.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 17:55:13.000000 Simba-UW-tf-dev-1.92.5/simba/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)    15004 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.92.5/simba/unsupervised/dbcv_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5077 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.92.5/simba/unsupervised/cluster_validation_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3645 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.92.5/simba/unsupervised/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-03 14:33:55.000000 Simba-UW-tf-dev-1.92.5/simba/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     9036 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.92.5/simba/unsupervised/cluster_video_visualizer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 17:55:13.000000 Simba-UW-tf-dev-1.92.5/simba/unsupervised/pop_ups/
+-rw-r--r--   0 simon      (501) staff       (20)     4642 2024-03-26 23:50:53.000000 Simba-UW-tf-dev-1.92.5/simba/unsupervised/pop_ups/cluster_videos_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     4027 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.92.5/simba/unsupervised/pop_ups/transform_cluster_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     5048 2024-02-15 23:45:22.000000 Simba-UW-tf-dev-1.92.5/simba/unsupervised/pop_ups/embedding_correlations_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-02 14:39:26.000000 Simba-UW-tf-dev-1.92.5/simba/unsupervised/pop_ups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     4070 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.92.5/simba/unsupervised/pop_ups/transform_dim_reduction_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)    11182 2024-02-15 23:45:22.000000 Simba-UW-tf-dev-1.92.5/simba/unsupervised/pop_ups/fit_dim_reduction_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     2546 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.92.5/simba/unsupervised/pop_ups/data_extractor_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     4536 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.92.5/simba/unsupervised/pop_ups/cluster_validation_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9305 2024-02-15 23:45:22.000000 Simba-UW-tf-dev-1.92.5/simba/unsupervised/pop_ups/fit_cluster_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     2574 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.92.5/simba/unsupervised/pop_ups/clusterer_comparison_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     6527 2024-03-26 23:50:53.000000 Simba-UW-tf-dev-1.92.5/simba/unsupervised/pop_ups/grid_search_visualizer_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     4332 2024-03-28 20:02:59.000000 Simba-UW-tf-dev-1.92.5/simba/unsupervised/pop_ups/cluster_xai_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     3820 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.92.5/simba/unsupervised/pop_ups/cluster_frequentist_stats_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     2355 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.92.5/simba/unsupervised/pop_ups/print_embedding_info_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     9946 2024-04-02 18:34:25.000000 Simba-UW-tf-dev-1.92.5/simba/unsupervised/dataset_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12982 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.92.5/simba/unsupervised/unsupervised_main.py
+-rw-r--r--   0 simon      (501) staff       (20)    10175 2024-03-27 12:56:51.000000 Simba-UW-tf-dev-1.92.5/simba/unsupervised/grid_search_visualizers.py
+-rw-r--r--   0 simon      (501) staff       (20)    16005 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.92.5/simba/unsupervised/data_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)     5241 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.92.5/simba/unsupervised/outlier_detector.py
+-rw-r--r--   0 simon      (501) staff       (20)    10397 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.92.5/simba/unsupervised/cluster_frequentist_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5798 2024-03-27 12:56:51.000000 Simba-UW-tf-dev-1.92.5/simba/unsupervised/embedding_correlation_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/unsupervised/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18194 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.92.5/simba/unsupervised/cluster_xai_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    15581 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.92.5/simba/unsupervised/umap_embedder.py
+-rw-r--r--   0 simon      (501) staff       (20)     5582 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.92.5/simba/unsupervised/clusterer_comparison_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     4652 2024-03-26 19:09:58.000000 Simba-UW-tf-dev-1.92.5/simba/unsupervised/bout_aggregator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2188 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/unsupervised/data_map.yaml
+-rw-r--r--   0 simon      (501) staff       (20)    14765 2024-03-26 19:09:58.000000 Simba-UW-tf-dev-1.92.5/simba/unsupervised/hdbscan_clusterer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3862 2024-02-15 21:37:53.000000 Simba-UW-tf-dev-1.92.5/simba/unsupervised/tsne.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 17:55:12.000000 Simba-UW-tf-dev-1.92.5/simba/bounding_box_tools/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/bounding_box_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8511 2024-02-08 00:53:55.000000 Simba-UW-tf-dev-1.92.5/simba/bounding_box_tools/agg_boundary_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)    27255 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/bounding_box_tools/boundary_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    10064 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/bounding_box_tools/boundary_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     7146 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/bounding_box_tools/find_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    12066 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/bounding_box_tools/visualize_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    18436 2024-05-19 17:46:48.000000 Simba-UW-tf-dev-1.92.5/simba/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 17:55:12.000000 Simba-UW-tf-dev-1.92.5/simba/feature_extractors/
+-rw-r--r--   0 simon      (501) staff       (20)    57052 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/feature_extractors/feature_extractor_14bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    28094 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/feature_extractors/feature_extractor_7bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 17:55:12.000000 Simba-UW-tf-dev-1.92.5/simba/feature_extractors/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     1757 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.92.5/simba/feature_extractors/misc/doctests.py
+-rw-r--r--   0 simon      (501) staff       (20)    29328 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.92.5/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     2705 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.92.5/simba/feature_extractors/misc/read_in_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2689 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.92.5/simba/feature_extractors/misc/peaks.py
+-rw-r--r--   0 simon      (501) staff       (20)    16727 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.92.5/simba/feature_extractors/misc/fish_feature_extractor_2022.py
+-rw-r--r--   0 simon      (501) staff       (20)     2144 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.92.5/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     5762 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.92.5/simba/feature_extractors/misc/convex_hull_scratch_1.py
+-rw-r--r--   0 simon      (501) staff       (20)    26425 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.92.5/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     7535 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.92.5/simba/feature_extractors/misc/egocentrical_aligner.py
+-rw-r--r--   0 simon      (501) staff       (20)     1274 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.92.5/simba/feature_extractors/misc/count_values_in_range.py
+-rw-r--r--   0 simon      (501) staff       (20)     5011 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.92.5/simba/feature_extractors/misc/graph_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3954 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.92.5/simba/feature_extractors/misc/termite_rois.csv
+-rw-r--r--   0 simon      (501) staff       (20)      736 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.92.5/simba/feature_extractors/misc/mutual_exclusive.py
+-rw-r--r--   0 simon      (501) staff       (20)     2883 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.92.5/simba/feature_extractors/misc/video_color.py
+-rw-r--r--   0 simon      (501) staff       (20)     2055 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.92.5/simba/feature_extractors/misc/graph_3d_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.92.5/simba/feature_extractors/misc/video_rotator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2932 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.92.5/simba/feature_extractors/misc/add_probability_cnt_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     1619 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.92.5/simba/feature_extractors/misc/make_splash.py
+-rw-r--r--   0 simon      (501) staff       (20)    37024 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.92.5/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py
+-rw-r--r--   0 simon      (501) staff       (20)     1613 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.92.5/simba/feature_extractors/misc/time_stamp_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.92.5/simba/feature_extractors/misc/video_rotator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    37022 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.92.5/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
+-rw-r--r--   0 simon      (501) staff       (20)     2068 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.92.5/simba/feature_extractors/misc/convex_hull_scratch_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    36307 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/feature_extractors/feature_extractor_8bps_2_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-02-21 02:05:27.000000 Simba-UW-tf-dev-1.92.5/simba/feature_extractors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     4091 2024-02-16 21:14:07.000000 Simba-UW-tf-dev-1.92.5/simba/feature_extractors/perimeter_jit.py
+-rw-r--r--   0 simon      (501) staff       (20)    26471 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/feature_extractors/feature_subsets.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/feature_extractors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    10043 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/feature_extractors/feature_extractor_user_defined.py
+-rw-r--r--   0 simon      (501) staff       (20)    61607 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/feature_extractors/feature_extractor_16bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    37328 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/feature_extractors/feature_extractor_9bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    31163 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/feature_extractors/feature_extractor_8bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    21427 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/feature_extractors/feature_extractor_4bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    65534 2024-03-01 16:55:51.000000 Simba-UW-tf-dev-1.92.5/simba/feature_extractors/amber_feature_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)     1173 2024-05-19 16:18:01.000000 Simba-UW-tf-dev-1.92.5/simba/requirements.txt
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 17:55:12.000000 Simba-UW-tf-dev-1.92.5/simba/mixins/
+-rw-r--r--   0 simon      (501) staff       (20)    40917 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/mixins/annotator_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    84123 2024-05-09 15:16:46.000000 Simba-UW-tf-dev-1.92.5/simba/mixins/timeseries_features_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-03 14:38:30.000000 Simba-UW-tf-dev-1.92.5/simba/mixins/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    53232 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.92.5/simba/mixins/pop_up_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    47980 2024-05-09 16:28:06.000000 Simba-UW-tf-dev-1.92.5/simba/mixins/config_reader.py
+-rw-r--r--   0 simon      (501) staff       (20)    56304 2024-04-17 23:32:32.000000 Simba-UW-tf-dev-1.92.5/simba/mixins/circular_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    38682 2024-05-14 17:44:58.000000 Simba-UW-tf-dev-1.92.5/simba/mixins/network_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/mixins/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    24040 2024-04-18 18:35:47.000000 Simba-UW-tf-dev-1.92.5/simba/mixins/pose_importer_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     3020 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/mixins/video_processing_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    35785 2024-05-09 15:22:35.000000 Simba-UW-tf-dev-1.92.5/simba/mixins/feature_extraction_supplement_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)   181387 2024-05-17 20:42:23.000000 Simba-UW-tf-dev-1.92.5/simba/mixins/statistics_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    44711 2024-04-22 19:40:36.000000 Simba-UW-tf-dev-1.92.5/simba/mixins/feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    69908 2024-05-06 18:32:12.000000 Simba-UW-tf-dev-1.92.5/simba/mixins/plotting_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)      391 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/mixins/abstract_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)    62121 2024-05-02 14:32:34.000000 Simba-UW-tf-dev-1.92.5/simba/mixins/image_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)      880 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.92.5/simba/mixins/unsupervised_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)   133234 2024-05-08 23:47:18.000000 Simba-UW-tf-dev-1.92.5/simba/mixins/train_model_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)   167515 2024-05-09 16:36:03.000000 Simba-UW-tf-dev-1.92.5/simba/mixins/geometry_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    24978 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/mixins/feature_extraction_circular_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 17:55:13.000000 Simba-UW-tf-dev-1.92.5/simba/third_party_label_appenders/
+-rw-r--r--   0 simon      (501) staff       (20)     6639 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/third_party_label_appenders/deepethogram_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12306 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/third_party_label_appenders/BORIS_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     9739 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/third_party_label_appenders/observer_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-22 19:49:42.000000 Simba-UW-tf-dev-1.92.5/simba/third_party_label_appenders/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     5508 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/third_party_label_appenders/boris_source_cleaner.py
+-rw-r--r--   0 simon      (501) staff       (20)    18963 2024-04-26 14:35:34.000000 Simba-UW-tf-dev-1.92.5/simba/third_party_label_appenders/tools.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/third_party_label_appenders/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    17344 2024-04-26 18:13:38.000000 Simba-UW-tf-dev-1.92.5/simba/third_party_label_appenders/third_party_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     9215 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/third_party_label_appenders/ethovision_import.py
+-rw-r--r--   0 simon      (501) staff       (20)     7456 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/third_party_label_appenders/BENTO_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     5662 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/third_party_label_appenders/solomon_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 17:55:12.000000 Simba-UW-tf-dev-1.92.5/simba/cue_light_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     8841 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/cue_light_tools/cue_light_clf_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    14451 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/cue_light_tools/cue_light_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    18274 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/cue_light_tools/cue_light_menues.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/cue_light_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1921 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/cue_light_tools/cue_light_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    19237 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/cue_light_tools/cue_light_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    15281 2024-04-25 13:46:55.000000 Simba-UW-tf-dev-1.92.5/simba/cue_light_tools/cue_light_movement_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 17:55:13.000000 Simba-UW-tf-dev-1.92.5/simba/utils/
+-rw-r--r--   0 simon      (501) staff       (20)    13211 2024-02-16 01:12:37.000000 Simba-UW-tf-dev-1.92.5/simba/utils/config_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    26136 2024-05-09 20:56:18.000000 Simba-UW-tf-dev-1.92.5/simba/utils/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)    10420 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.92.5/simba/utils/custom_feature_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-25 18:17:26.000000 Simba-UW-tf-dev-1.92.5/simba/utils/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7734 2024-05-08 13:50:22.000000 Simba-UW-tf-dev-1.92.5/simba/utils/warnings.py
+-rw-r--r--   0 simon      (501) staff       (20)    56026 2024-05-14 14:03:50.000000 Simba-UW-tf-dev-1.92.5/simba/utils/checks.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/utils/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    79930 2024-05-16 13:13:35.000000 Simba-UW-tf-dev-1.92.5/simba/utils/read_write.py
+-rw-r--r--   0 simon      (501) staff       (20)    17201 2024-05-14 11:12:57.000000 Simba-UW-tf-dev-1.92.5/simba/utils/lookups.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 17:55:13.000000 Simba-UW-tf-dev-1.92.5/simba/utils/cli/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/utils/cli/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7129 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/utils/cli/cli_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    17086 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/utils/errors.py
+-rw-r--r--   0 simon      (501) staff       (20)    46270 2024-04-26 16:10:44.000000 Simba-UW-tf-dev-1.92.5/simba/utils/data.py
+-rw-r--r--   0 simon      (501) staff       (20)     4205 2024-02-21 03:51:46.000000 Simba-UW-tf-dev-1.92.5/simba/utils/printing.py
+-rw-r--r--   0 simon      (501) staff       (20)   243998 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/SimBA_logo.ico
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 17:55:13.000000 Simba-UW-tf-dev-1.92.5/simba/pose_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     8626 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/pose_processors/reorganize_keypoint.py
+-rw-r--r--   0 simon      (501) staff       (20)     5840 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/pose_processors/remove_keypoints.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/pose_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2872 2024-02-15 23:39:58.000000 Simba-UW-tf-dev-1.92.5/simba/pose_processors/pose_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)     6313 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/pose_processors/reverse_pose.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 17:55:13.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/
+-rw-r--r--   0 simon      (501) staff       (20)      786 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/doctests.py
+-rw-r--r--   0 simon      (501) staff       (20)    29328 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/fish_feature_extractor_2023_version_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     4080 2024-05-06 15:09:47.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/CLAHE.py
+-rw-r--r--   0 simon      (501) staff       (20)     2387 2024-03-08 14:35:02.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/dprime.py
+-rw-r--r--   0 simon      (501) staff       (20)     3869 2024-05-14 18:18:20.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/ffmpeg_progress_bar.py
+-rw-r--r--   0 simon      (501) staff       (20)     2516 2024-03-18 17:01:43.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/linear_fretchet.py
+-rw-r--r--   0 simon      (501) staff       (20)     2705 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/read_in_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2391 2024-03-14 12:45:59.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/piotr_120324 3.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)     2036 2024-03-28 18:29:59.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/dunn_index.py
+-rw-r--r--   0 simon      (501) staff       (20)     3640 2024-04-08 13:30:56.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/hausdorff.py
+-rw-r--r--   0 simon      (501) staff       (20)     2689 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/peaks.py
+-rw-r--r--   0 simon      (501) staff       (20)    16727 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/fish_feature_extractor_2022.py
+-rw-r--r--   0 simon      (501) staff       (20)     3494 2024-04-03 13:42:02.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/colinear_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     8921 2024-03-22 13:56:46.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/spontaneous_alternation_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    21658 2024-04-10 16:31:38.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/horizontal_videos_concat.py
+-rw-r--r--   0 simon      (501) staff       (20)     2144 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/convex_hull_3_scratch_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     1103 2024-03-29 16:26:34.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/silhouette_score.py
+-rw-r--r--   0 simon      (501) staff       (20)     3607 2024-04-09 14:21:58.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/two_fish_feature_extractor_040924.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)    33092 2024-02-22 15:57:45.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/cuda_jit.ipynb
+-rw-r--r--   0 simon      (501) staff       (20)     5762 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/convex_hull_scratch_1.py
+-rw-r--r--   0 simon      (501) staff       (20)     1867 2024-03-12 19:23:40.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/directed_hausdorff.py
+-rw-r--r--   0 simon      (501) staff       (20)      963 2024-03-13 18:20:52.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/shannon_diversity_index.py
+-rw-r--r--   0 simon      (501) staff       (20)     3726 2024-03-12 13:31:58.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/sequential_lag_analysis.py
+-rw-r--r--   0 simon      (501) staff       (20)     1254 2024-03-13 16:09:50.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/wilcoxon.py
+-rw-r--r--   0 simon      (501) staff       (20)    21599 2024-04-22 16:40:51.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/ROI_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-25 14:48:22.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      549 2024-05-14 19:00:13.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/detect_scene_changes.py
+-rw-r--r--   0 simon      (501) staff       (20)     3328 2024-03-08 15:05:36.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/data.npy
+-rw-r--r--   0 simon      (501) staff       (20)    12626 2024-03-25 20:59:27.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/distances.py
+-rw-r--r--   0 simon      (501) staff       (20)    26425 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/fish_feature_extractor_2023_version_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     2623 2024-05-03 16:20:12.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/cohens_kappa.py
+-rw-r--r--   0 simon      (501) staff       (20)     4950 2024-05-14 14:14:15.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/watermark.py
+-rw-r--r--   0 simon      (501) staff       (20)     2465 2024-03-08 17:38:19.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/paths.py
+-rw-r--r--   0 simon      (501) staff       (20)     1048 2024-03-13 14:41:23.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/outliers_tietjen.py
+-rw-r--r--   0 simon      (501) staff       (20)     1424 2024-02-26 15:46:14.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/train_model.py
+-rw-r--r--   0 simon      (501) staff       (20)     2346 2024-04-19 14:10:16.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/img_stack_to_bw.py
+-rw-r--r--   0 simon      (501) staff       (20)     3171 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/amber_tests.py
+-rw-r--r--   0 simon      (501) staff       (20)     3590 2024-03-11 17:05:31.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/line_locate_point.py
+-rw-r--r--   0 simon      (501) staff       (20)     1841 2024-04-19 16:19:10.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/sorensen_dice_coefficient.py
+-rw-r--r--   0 simon      (501) staff       (20)     3182 2024-02-24 20:57:19.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/multifrm_to_points.py
+-rw-r--r--   0 simon      (501) staff       (20)      959 2024-05-16 13:12:21.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/clean_sleap_filename.py
+-rw-r--r--   0 simon      (501) staff       (20)       69 2024-03-18 18:17:24.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/lcs.py
+-rw-r--r--   0 simon      (501) staff       (20)    12448 2024-04-09 14:14:37.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/two_fish_feature_extractor_040924.py
+-rw-r--r--   0 simon      (501) staff       (20)     6119 2024-04-20 17:58:22.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/ez_path_plot.py
+-rw-r--r--   0 simon      (501) staff       (20)     7535 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/egocentrical_aligner.py
+-rw-r--r--   0 simon      (501) staff       (20)     5109 2024-05-07 19:36:44.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/downsample_video_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     2350 2024-03-12 17:58:33.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/add_body_part.py
+-rw-r--r--   0 simon      (501) staff       (20)     1008 2024-03-12 13:29:20.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/grubbs_test.py
+-rw-r--r--   0 simon      (501) staff       (20)     3399 2024-02-16 01:12:37.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/slide_circ_mean.py
+-rw-r--r--   0 simon      (501) staff       (20)     1835 2024-03-28 22:56:59.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/calinski_harabasz.py
+-rw-r--r--   0 simon      (501) staff       (20)     1282 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/roi_feature_visualizer_example.py
+-rw-r--r--   0 simon      (501) staff       (20)    10076 2024-03-22 16:51:40.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/spontaneuous_alternation_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)      895 2024-03-12 14:09:55.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/runs_test.py
+-rw-r--r--   0 simon      (501) staff       (20)     2516 2024-04-06 11:33:24.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/pct_counts_in_top_N.py
+-rw-r--r--   0 simon      (501) staff       (20)     1095 2024-04-19 18:37:50.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/concordance_ratio.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:46:33.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2287 2024-03-25 16:45:04.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/total_variation_distance.py
+-rw-r--r--   0 simon      (501) staff       (20)     3056 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/crop_single_polygon.py
+-rw-r--r--   0 simon      (501) staff       (20)    15977 2024-04-23 22:52:42.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/ROI_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     8010 2024-03-24 19:48:22.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/joint_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     1529 2024-04-19 15:08:24.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/segment_image_horizontal.py
+-rw-r--r--   0 simon      (501) staff       (20)    11145 2024-04-15 15:02:56.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/clip_multiple_videos_by_frame_numbers.py
+-rw-r--r--   0 simon      (501) staff       (20)     2552 2024-04-02 14:48:59.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/elliptic_envelope.py
+-rw-r--r--   0 simon      (501) staff       (20)     1016 2024-03-14 14:57:29.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/roi_definition_csvs_to_h5.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)     1276 2024-03-12 17:58:38.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/add_body_part.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)      921 2024-02-26 15:46:14.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/roi_feature_visualizer_example.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)     2631 2024-04-05 16:23:07.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/sliding_crosscorrelation.py
+-rw-r--r--   0 simon      (501) staff       (20)     1274 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/count_values_in_range.py
+-rw-r--r--   0 simon      (501) staff       (20)     2174 2024-03-14 14:56:26.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/roi_definition_csvs_to_h5.py
+-rw-r--r--   0 simon      (501) staff       (20)     1656 2024-03-30 18:32:44.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/distance_velocity.py
+-rw-r--r--   0 simon      (501) staff       (20)     5011 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/graph_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5666 2024-04-11 15:28:58.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/line_plot_plotly.py
+-rw-r--r--   0 simon      (501) staff       (20)     3838 2024-05-14 11:30:22.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/crossfade.py
+-rw-r--r--   0 simon      (501) staff       (20)     3043 2024-05-09 15:04:30.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/shift_geometries.py
+-rw-r--r--   0 simon      (501) staff       (20)     3954 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/termite_rois.csv
+-rw-r--r--   0 simon      (501) staff       (20)     1785 2024-05-15 19:11:53.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/convert_to_bw.py
+-rw-r--r--   0 simon      (501) staff       (20)     5254 2024-05-07 19:55:25.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/downsample_multiple_videos_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     1351 2024-03-26 21:10:40.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/unsupervised_lof.py
+-rw-r--r--   0 simon      (501) staff       (20)     2553 2024-03-11 15:09:38.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/siegel_tukey.py
+-rw-r--r--   0 simon      (501) staff       (20)      958 2024-03-13 18:05:08.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/berger_parker.py
+-rw-r--r--   0 simon      (501) staff       (20)     4177 2024-04-10 01:56:43.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/isolation_forest.py
+-rw-r--r--   0 simon      (501) staff       (20)     2845 2024-03-28 19:23:54.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/davis_bouldin.py
+-rw-r--r--   0 simon      (501) staff       (20)     4094 2024-04-10 14:09:54.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/vertical_video_concatenator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2770 2024-04-07 19:14:13.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/batch_video_to_greyscale.py
+-rw-r--r--   0 simon      (501) staff       (20)     7215 2024-02-26 15:46:14.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/crop_circles_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1410 2024-03-19 12:49:24.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/heading.py
+-rw-r--r--   0 simon      (501) staff       (20)     2243 2024-03-13 18:35:02.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/piotr_120324 2.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)      736 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/mutual_exclusive.py
+-rw-r--r--   0 simon      (501) staff       (20)     2278 2024-05-04 19:11:33.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/mahalanobis.py
+-rw-r--r--   0 simon      (501) staff       (20)     1626 2024-05-08 16:59:35.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/superpixels.py
+-rw-r--r--   0 simon      (501) staff       (20)     2225 2024-05-09 20:57:38.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/img_conv.py
+-rw-r--r--   0 simon      (501) staff       (20)     2907 2024-03-14 19:31:25.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/grangercausalitytests.py
+-rw-r--r--   0 simon      (501) staff       (20)     2432 2024-03-19 20:48:43.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/multiframe_is_shape_covered.py
+-rw-r--r--   0 simon      (501) staff       (20)      592 2024-02-27 21:31:33.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/redis.py
+-rw-r--r--   0 simon      (501) staff       (20)     2893 2024-02-26 20:49:33.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/video_color.py
+-rw-r--r--   0 simon      (501) staff       (20)     2055 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/graph_3d_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     3137 2024-05-15 15:22:04.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/blurbox.py
+-rw-r--r--   0 simon      (501) staff       (20)     6186 2024-03-18 12:44:45.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/piotr_120324.py
+-rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/video_rotator.py
+-rw-r--r--   0 simon      (501) staff       (20)     4166 2024-05-06 21:09:36.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/superimpose_frame_count.py
+-rw-r--r--   0 simon      (501) staff       (20)     5433 2024-05-14 15:38:59.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/inset_overlay_video.py
+-rw-r--r--   0 simon      (501) staff       (20)     1004 2024-03-12 13:11:45.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/hartley_fmax.py
+-rw-r--r--   0 simon      (501) staff       (20)       84 2024-04-03 17:05:23.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/calc_N_degree_direction_switches.py
+-rw-r--r--   0 simon      (501) staff       (20)     2307 2024-02-27 21:31:33.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/fix_clahe.py
+-rw-r--r--   0 simon      (501) staff       (20)     1836 2024-03-10 15:38:46.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/cochran_q.py
+-rw-r--r--   0 simon      (501) staff       (20)      682 2024-03-13 19:19:43.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/menhinicks_index.py
+-rw-r--r--   0 simon      (501) staff       (20)      493 2024-05-02 16:25:29.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/lbp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2932 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/add_probability_cnt_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     1559 2024-04-19 15:50:37.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/brillouins_index.py
+-rw-r--r--   0 simon      (501) staff       (20)    13575 2024-03-20 11:47:11.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/spontanous_alternations.py
+-rw-r--r--   0 simon      (501) staff       (20)     1951 2024-05-03 14:45:28.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/eta_squared.py
+-rw-r--r--   0 simon      (501) staff       (20)     2268 2024-03-13 13:59:07.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/piotr_120324.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)    16301 2024-05-13 14:59:18.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/convert_to_mp4.py
+-rw-r--r--   0 simon      (501) staff       (20)     4655 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/velocity_aggregator.py
+-rw-r--r--   0 simon      (501) staff       (20)     1619 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/make_splash.py
+-rw-r--r--   0 simon      (501) staff       (20)     6440 2024-05-09 20:10:17.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/change_img_file_format.py
+-rw-r--r--   0 simon      (501) staff       (20)     4478 2024-04-08 20:43:42.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/abod.py
+-rw-r--r--   0 simon      (501) staff       (20)    37024 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/fish_feature_extractor_2023_version_5.py
+-rw-r--r--   0 simon      (501) staff       (20)     1374 2024-04-18 13:56:20.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/violin.py
+-rw-r--r--   0 simon      (501) staff       (20)    16527 2024-05-17 20:38:47.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/bg_substraction.py
+-rw-r--r--   0 simon      (501) staff       (20)     1073 2024-03-13 16:46:16.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/simpson_diversity_index.py
+-rw-r--r--   0 simon      (501) staff       (20)     4485 2024-04-14 19:07:54.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/clip_videos_by_frm.py
+-rw-r--r--   0 simon      (501) staff       (20)      770 2024-05-02 20:50:37.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/fleiss_kappa.py
+-rw-r--r--   0 simon      (501) staff       (20)     2396 2024-03-17 16:55:38.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/piotr_120324 4.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)    12282 2024-05-12 17:13:08.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/convert_to_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     1106 2024-04-18 13:46:43.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/rotate image.py
+-rw-r--r--   0 simon      (501) staff       (20)     1214 2024-05-03 17:07:43.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/jaccard_distance.py
+-rw-r--r--   0 simon      (501) staff       (20)     5336 2024-02-10 20:28:08.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/geometry_ex.py
+-rw-r--r--   0 simon      (501) staff       (20)     1613 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/time_stamp_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     1505 2024-03-28 14:36:24.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/line_plot.py
+-rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/video_rotator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15996 2024-04-09 13:41:30.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/unsupervised_outliers.py
+-rw-r--r--   0 simon      (501) staff       (20)      122 2024-05-15 13:58:53.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/profiler.py
+-rw-r--r--   0 simon      (501) staff       (20)     1378 2024-05-03 20:13:55.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/manhattan_distance.py
+-rw-r--r--   0 simon      (501) staff       (20)     5690 2024-02-10 20:28:08.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/statistics_ex.py
+-rw-r--r--   0 simon      (501) staff       (20)    16646 2024-04-22 16:43:10.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/ROI_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     1391 2024-03-18 23:21:46.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/sliding_displacement.py
+-rw-r--r--   0 simon      (501) staff       (20)     7819 2024-04-18 14:47:28.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/path_plots.py
+-rw-r--r--   0 simon      (501) staff       (20)     2671 2024-05-08 14:43:03.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/seekable.py
+-rw-r--r--   0 simon      (501) staff       (20)    12182 2024-05-19 17:38:25.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/superimpose_popups.py
+-rw-r--r--   0 simon      (501) staff       (20)     6572 2024-05-15 13:42:29.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/superimpose_elapsed_time.py
+-rw-r--r--   0 simon      (501) staff       (20)      925 2024-03-11 13:06:04.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/wald_wolfowitz.py
+-rw-r--r--   0 simon      (501) staff       (20)     2425 2024-05-03 15:57:50.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/relative_risk.py
+-rw-r--r--   0 simon      (501) staff       (20)     1814 2024-04-05 14:36:58.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/sliding_autoc.py
+-rw-r--r--   0 simon      (501) staff       (20)     2369 2024-03-14 17:07:10.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/linestring_path.py
+-rw-r--r--   0 simon      (501) staff       (20)     2233 2024-03-18 15:20:48.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/cronbach_alpha.py
+-rw-r--r--   0 simon      (501) staff       (20)     2809 2024-03-08 21:15:58.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/mcnamar.py
+-rw-r--r--   0 simon      (501) staff       (20)     6507 2024-05-06 12:58:30.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/contrast.py
+-rw-r--r--   0 simon      (501) staff       (20)    37022 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/fish_feature_extractor_2023_version_4.py
+-rw-r--r--   0 simon      (501) staff       (20)     6220 2024-02-24 20:57:19.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/AmberFeatureExtractor.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)     1157 2024-05-02 20:32:28.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/youden_j.py
+-rw-r--r--   0 simon      (501) staff       (20)     1933 2024-04-10 15:09:25.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/mosaic.py
+-rw-r--r--   0 simon      (501) staff       (20)      441 2024-04-12 17:03:24.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/bouts_df
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-05-06 15:36:55.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/color_filtering.py
+-rw-r--r--   0 simon      (501) staff       (20)    69423 2024-02-20 14:30:23.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/amber_featurizer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6286 2024-04-17 19:28:51.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/make_path_plot.py
+-rw-r--r--   0 simon      (501) staff       (20)      837 2024-03-13 18:56:21.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/margalef_diversification_index.py
+-rw-r--r--   0 simon      (501) staff       (20)      997 2024-03-17 17:49:00.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/biweight_midcorrelation.py
+-rw-r--r--   0 simon      (501) staff       (20)     2186 2024-03-18 15:31:23.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/madmedianrule.py
+-rw-r--r--   0 simon      (501) staff       (20)     2915 2024-04-01 14:12:59.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/adjusted_rand_score.py
+-rw-r--r--   0 simon      (501) staff       (20)     2068 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/convex_hull_scratch_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     1957 2024-04-12 14:55:03.000000 Simba-UW-tf-dev-1.92.5/simba/sandbox/plotly_gantt.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 17:55:12.000000 Simba-UW-tf-dev-1.92.5/simba/plotting/
+-rw-r--r--   0 simon      (501) staff       (20)     8538 2024-02-23 18:25:51.000000 Simba-UW-tf-dev-1.92.5/simba/plotting/directing_animals_to_bodypart_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10307 2024-05-06 15:39:18.000000 Simba-UW-tf-dev-1.92.5/simba/plotting/gantt_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 17:55:12.000000 Simba-UW-tf-dev-1.92.5/simba/plotting/tools/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:43:56.000000 Simba-UW-tf-dev-1.92.5/simba/plotting/tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     5946 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/plotting/tools/tkinter_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    23490 2024-04-29 16:23:41.000000 Simba-UW-tf-dev-1.92.5/simba/plotting/ROI_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-05-09 13:03:17.000000 Simba-UW-tf-dev-1.92.5/simba/plotting/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    19315 2024-05-08 18:11:04.000000 Simba-UW-tf-dev-1.92.5/simba/plotting/shap_agg_stats_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12956 2024-05-06 15:39:18.000000 Simba-UW-tf-dev-1.92.5/simba/plotting/gantt_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15819 2024-04-25 18:19:38.000000 Simba-UW-tf-dev-1.92.5/simba/plotting/heat_mapper_clf_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    10620 2024-04-26 18:13:38.000000 Simba-UW-tf-dev-1.92.5/simba/plotting/probability_plot_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8987 2024-05-09 16:36:03.000000 Simba-UW-tf-dev-1.92.5/simba/plotting/circular_plotting.py
+-rw-r--r--   0 simon      (501) staff       (20)    16960 2024-05-06 15:39:18.000000 Simba-UW-tf-dev-1.92.5/simba/plotting/plot_clf_results.py
+-rw-r--r--   0 simon      (501) staff       (20)    10328 2024-04-25 15:48:10.000000 Simba-UW-tf-dev-1.92.5/simba/plotting/ez_path_plot.py
+-rw-r--r--   0 simon      (501) staff       (20)    17432 2024-04-17 23:57:27.000000 Simba-UW-tf-dev-1.92.5/simba/plotting/plot_clf_results_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    21343 2024-04-29 18:50:27.000000 Simba-UW-tf-dev-1.92.5/simba/plotting/ROI_feature_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    14847 2024-05-06 15:39:18.000000 Simba-UW-tf-dev-1.92.5/simba/plotting/heat_mapper_location.py
+-rw-r--r--   0 simon      (501) staff       (20)    13512 2024-04-26 18:13:38.000000 Simba-UW-tf-dev-1.92.5/simba/plotting/probability_plot_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/plotting/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     5253 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/plotting/interactive_probability_grapher.py
+-rw-r--r--   0 simon      (501) staff       (20)     6517 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/plotting/plot_pose_in_dir.py
+-rw-r--r--   0 simon      (501) staff       (20)    20950 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.92.5/simba/plotting/single_run_model_validation_video.py
+-rw-r--r--   0 simon      (501) staff       (20)     8732 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.92.5/simba/plotting/frame_mergerer_ffmpeg.py
+-rw-r--r--   0 simon      (501) staff       (20)    10667 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.92.5/simba/plotting/pose_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16477 2024-04-25 18:30:53.000000 Simba-UW-tf-dev-1.92.5/simba/plotting/directing_animals_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11565 2024-04-28 20:02:42.000000 Simba-UW-tf-dev-1.92.5/simba/plotting/clf_validator.py
+-rw-r--r--   0 simon      (501) staff       (20)    23459 2024-04-25 18:18:16.000000 Simba-UW-tf-dev-1.92.5/simba/plotting/path_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    24207 2024-05-07 12:24:30.000000 Simba-UW-tf-dev-1.92.5/simba/plotting/ROI_feature_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11824 2024-04-17 19:58:21.000000 Simba-UW-tf-dev-1.92.5/simba/plotting/data_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13091 2024-03-26 23:49:10.000000 Simba-UW-tf-dev-1.92.5/simba/plotting/spontaneous_alternation_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    21979 2024-04-25 18:18:16.000000 Simba-UW-tf-dev-1.92.5/simba/plotting/path_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    16926 2024-04-25 19:01:12.000000 Simba-UW-tf-dev-1.92.5/simba/plotting/distance_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    17511 2024-04-28 19:58:43.000000 Simba-UW-tf-dev-1.92.5/simba/plotting/ROI_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    10034 2024-03-19 12:54:07.000000 Simba-UW-tf-dev-1.92.5/simba/plotting/geometry_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    15989 2024-04-28 20:02:42.000000 Simba-UW-tf-dev-1.92.5/simba/plotting/clf_validator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    14224 2024-04-25 18:19:38.000000 Simba-UW-tf-dev-1.92.5/simba/plotting/heat_mapper_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)    11994 2024-04-11 22:38:54.000000 Simba-UW-tf-dev-1.92.5/simba/plotting/distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    19073 2024-04-11 20:26:33.000000 Simba-UW-tf-dev-1.92.5/simba/plotting/single_run_model_validation_video_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    12552 2024-04-25 18:30:28.000000 Simba-UW-tf-dev-1.92.5/simba/plotting/directing_animals_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)     9549 2024-05-09 16:36:03.000000 Simba-UW-tf-dev-1.92.5/simba/plotting/circular_feature_overlay_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    14663 2024-05-06 15:39:18.000000 Simba-UW-tf-dev-1.92.5/simba/plotting/heat_mapper_location_mp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 17:55:12.000000 Simba-UW-tf-dev-1.92.5/simba/dash_app/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:44:15.000000 Simba-UW-tf-dev-1.92.5/simba/dash_app/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    72715 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/dash_app/SimBA_dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     4965 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/dash_app/run_dash_tkinter.py
+-rw-r--r--   0 simon      (501) staff       (20)    47546 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/dash_app/dash_app.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 17:55:12.000000 Simba-UW-tf-dev-1.92.5/simba/data_processors/
+-rw-r--r--   0 simon      (501) staff       (20)    13060 2024-04-26 18:13:38.000000 Simba-UW-tf-dev-1.92.5/simba/data_processors/spontaneous_alternation_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    11813 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/data_processors/agg_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-21 11:48:06.000000 Simba-UW-tf-dev-1.92.5/simba/data_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    13224 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/data_processors/severity_bout_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    39110 2024-03-19 12:54:07.000000 Simba-UW-tf-dev-1.92.5/simba/data_processors/interpolation_smoothing.py
+-rw-r--r--   0 simon      (501) staff       (20)    10968 2024-02-21 19:10:40.000000 Simba-UW-tf-dev-1.92.5/simba/data_processors/directing_animal_to_bodypart.py
+-rw-r--r--   0 simon      (501) staff       (20)     9580 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/data_processors/timebins_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    20617 2024-04-18 21:13:37.000000 Simba-UW-tf-dev-1.92.5/simba/data_processors/fsttc_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/data_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     4872 2024-04-26 15:18:54.000000 Simba-UW-tf-dev-1.92.5/simba/data_processors/boolean_conditional_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     7117 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/data_processors/interpolate_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)    15989 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.92.5/simba/data_processors/directing_other_animals_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8957 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/data_processors/gibbs_sampler.py
+-rw-r--r--   0 simon      (501) staff       (20)    10054 2024-04-04 16:23:22.000000 Simba-UW-tf-dev-1.92.5/simba/data_processors/timebins_movement_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5255 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/data_processors/severity_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    18517 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/data_processors/pup_retrieval_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3118 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/data_processors/pybursts_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    13660 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/data_processors/severity_frame_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8738 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/data_processors/mutual_exclusivity_corrector.py
+-rw-r--r--   0 simon      (501) staff       (20)    12919 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/data_processors/kleinberg_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    10196 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/data_processors/movement_calculator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 17:55:12.000000 Simba-UW-tf-dev-1.92.5/simba/model/
+-rw-r--r--   0 simon      (501) staff       (20)    21997 2024-05-08 23:53:08.000000 Simba-UW-tf-dev-1.92.5/simba/model/train_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     4969 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/model/inference_batch.py
+-rw-r--r--   0 simon      (501) staff       (20)    14036 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/model/train_multiclass_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     3937 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/model/inference_multiclass_batch.py
+-rw-r--r--   0 simon      (501) staff       (20)    15931 2024-02-20 14:30:06.000000 Simba-UW-tf-dev-1.92.5/simba/model/grid_search_multiclass_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:41:19.000000 Simba-UW-tf-dev-1.92.5/simba/model/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    14317 2024-05-08 23:47:18.000000 Simba-UW-tf-dev-1.92.5/simba/model/grid_search_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     3768 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/model/inference_validation.py
+-rw-r--r--   0 simon      (501) staff       (20)     6872 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/model/train_multilabel_rf.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 17:55:13.000000 Simba-UW-tf-dev-1.92.5/simba/roi_tools/
+-rw-r--r--   0 simon      (501) staff       (20)    11039 2024-05-09 16:32:28.000000 Simba-UW-tf-dev-1.92.5/simba/roi_tools/ROI_time_bin_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-25 18:17:26.000000 Simba-UW-tf-dev-1.92.5/simba/roi_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    50014 2024-05-17 13:19:01.000000 Simba-UW-tf-dev-1.92.5/simba/roi_tools/ROI_define.py
+-rw-r--r--   0 simon      (501) staff       (20)     3616 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/roi_tools/ROI_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/roi_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     9876 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/roi_tools/ROI_size_standardizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    18552 2024-05-09 16:13:09.000000 Simba-UW-tf-dev-1.92.5/simba/roi_tools/ROI_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    15406 2024-05-07 01:16:15.000000 Simba-UW-tf-dev-1.92.5/simba/roi_tools/ROI_feature_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     4386 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/roi_tools/ROI_multiply.py
+-rw-r--r--   0 simon      (501) staff       (20)     2313 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/roi_tools/ROI_size_calculations.py
+-rw-r--r--   0 simon      (501) staff       (20)     3716 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/roi_tools/ROI_zoom.py
+-rw-r--r--   0 simon      (501) staff       (20)    12313 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.92.5/simba/roi_tools/ROI_directing_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11974 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/roi_tools/ROI_move_shape.py
+-rw-r--r--   0 simon      (501) staff       (20)     5470 2024-02-21 03:51:46.000000 Simba-UW-tf-dev-1.92.5/simba/roi_tools/ROI_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    16129 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/roi_tools/ROI_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    29746 2024-05-17 13:17:50.000000 Simba-UW-tf-dev-1.92.5/simba/roi_tools/ROI_image.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 17:55:13.000000 Simba-UW-tf-dev-1.92.5/simba/pose_importers/
+-rw-r--r--   0 simon      (501) staff       (20)    10711 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.92.5/simba/pose_importers/sleap_csv_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 17:55:13.000000 Simba-UW-tf-dev-1.92.5/simba/pose_importers/misc/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:31.000000 Simba-UW-tf-dev-1.92.5/simba/pose_importers/misc/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8084 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/pose_importers/misc/apt_trk_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     2577 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/pose_importers/read_DANNCE_mat.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-22 19:49:42.000000 Simba-UW-tf-dev-1.92.5/simba/pose_importers/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    13867 2024-05-16 18:24:39.000000 Simba-UW-tf-dev-1.92.5/simba/pose_importers/sleap_h5_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     8161 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/pose_importers/madlc_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/pose_importers/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    13672 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.92.5/simba/pose_importers/sleap_slp_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     8645 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/pose_importers/import_mars.py
+-rw-r--r--   0 simon      (501) staff       (20)     7464 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/pose_importers/dlc_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)     8417 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/pose_importers/trk_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 17:55:12.000000 Simba-UW-tf-dev-1.92.5/simba/pose_configurations/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2024-03-19 18:18:43.000000 Simba-UW-tf-dev-1.92.5/simba/pose_configurations/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 17:55:12.000000 Simba-UW-tf-dev-1.92.5/simba/pose_configurations/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:10.000000 Simba-UW-tf-dev-1.92.5/simba/pose_configurations/bp_names/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     4485 2024-03-04 19:10:54.000000 Simba-UW-tf-dev-1.92.5/simba/pose_configurations/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 17:55:12.000000 Simba-UW-tf-dev-1.92.5/simba/pose_configurations/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       27 2024-03-04 19:10:54.000000 Simba-UW-tf-dev-1.92.5/simba/pose_configurations/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:18.000000 Simba-UW-tf-dev-1.92.5/simba/pose_configurations/no_animals/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:05.000000 Simba-UW-tf-dev-1.92.5/simba/pose_configurations/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 17:55:12.000000 Simba-UW-tf-dev-1.92.5/simba/pose_configurations/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:14.000000 Simba-UW-tf-dev-1.92.5/simba/pose_configurations/configuration_names/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)      273 2024-03-04 19:10:54.000000 Simba-UW-tf-dev-1.92.5/simba/pose_configurations/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 17:55:12.000000 Simba-UW-tf-dev-1.92.5/simba/pose_configurations/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/pose_configurations/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/pose_configurations/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/pose_configurations/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    34231 2024-02-20 18:50:39.000000 Simba-UW-tf-dev-1.92.5/simba/pose_configurations/schematics/13.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/pose_configurations/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/pose_configurations/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/pose_configurations/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/pose_configurations/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/pose_configurations/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/pose_configurations/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/pose_configurations/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/pose_configurations/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/pose_configurations/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 17:55:13.000000 Simba-UW-tf-dev-1.92.5/simba/video_processors/
+-rw-r--r--   0 simon      (501) staff       (20)   190387 2024-05-19 17:29:59.000000 Simba-UW-tf-dev-1.92.5/simba/video_processors/video_processing.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-05-15 15:29:21.000000 Simba-UW-tf-dev-1.92.5/simba/video_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     5577 2024-04-08 11:29:52.000000 Simba-UW-tf-dev-1.92.5/simba/video_processors/roi_selector_circle.py
+-rw-r--r--   0 simon      (501) staff       (20)     9073 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/video_processors/px_to_mm.py
+-rw-r--r--   0 simon      (501) staff       (20)    35053 2024-02-26 15:42:07.000000 Simba-UW-tf-dev-1.92.5/simba/video_processors/batch_process_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    11439 2024-05-14 20:38:00.000000 Simba-UW-tf-dev-1.92.5/simba/video_processors/multi_cropper.py
+-rw-r--r--   0 simon      (501) staff       (20)     3066 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/video_processors/extract_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/video_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6598 2024-02-26 21:50:01.000000 Simba-UW-tf-dev-1.92.5/simba/video_processors/roi_selector.py
+-rw-r--r--   0 simon      (501) staff       (20)    10007 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/video_processors/calculate_px_dist.py
+-rw-r--r--   0 simon      (501) staff       (20)     3674 2024-05-06 19:29:28.000000 Simba-UW-tf-dev-1.92.5/simba/video_processors/brightness_contrast_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     5963 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.92.5/simba/video_processors/roi_selector_polygon.py
+-rw-r--r--   0 simon      (501) staff       (20)     4926 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/video_processors/extract_seqframes.py
+-rw-r--r--   0 simon      (501) staff       (20)    15117 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.92.5/simba/video_processors/batch_process_create_ffmpeg_commands.py
+-rw-r--r--   0 simon      (501) staff       (20)     3595 2024-05-06 15:51:58.000000 Simba-UW-tf-dev-1.92.5/simba/video_processors/clahe_ui.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 17:55:12.000000 Simba-UW-tf-dev-1.92.5/simba/outlier_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     7837 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/outlier_tools/outlier_corrector_movement.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/outlier_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    14462 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/outlier_tools/outlier_corrector_location_advanced.py
+-rw-r--r--   0 simon      (501) staff       (20)    13117 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/outlier_tools/outlier_corrector_movement_advanced.py
+-rw-r--r--   0 simon      (501) staff       (20)    10396 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/outlier_tools/outlier_corrector_location.py
+-rw-r--r--   0 simon      (501) staff       (20)     2751 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/outlier_tools/skip_outlier_correction.py
+-rw-r--r--   0 simon      (501) staff       (20)    83726 2024-05-19 17:49:14.000000 Simba-UW-tf-dev-1.92.5/simba/SimBA.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 17:55:12.000000 Simba-UW-tf-dev-1.92.5/simba/assets/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 17:55:12.000000 Simba-UW-tf-dev-1.92.5/simba/assets/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)   109483 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/unsupervised/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:36.000000 Simba-UW-tf-dev-1.92.5/simba/assets/unsupervised/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/unsupervised/features.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 17:55:12.000000 Simba-UW-tf-dev-1.92.5/simba/assets/shap/
+-rw-r--r--   0 simon      (501) staff       (20)     1177 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/shap/down_arrow.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1733 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/shap/intruder_shape.jpg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 17:55:12.000000 Simba-UW-tf-dev-1.92.5/simba/assets/shap/feature_categories/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:25.000000 Simba-UW-tf-dev-1.92.5/simba/assets/shap/feature_categories/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    17420 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/shap/feature_categories/shap_feature_categories.csv
+-rw-r--r--   0 simon      (501) staff       (20)     1665 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/shap/resident_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2415 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/shap/resident_intruder_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2012 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/shap/animal_distances.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     4422 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/shap/baseline_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:21.000000 Simba-UW-tf-dev-1.92.5/simba/assets/shap/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)   353824 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/shap/ubuntu.regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     6672 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/shap/side_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/shap/UbuntuMono-Regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     2737 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/shap/side_scale_5.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1785 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/shap/intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1435 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/shap/resident_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     3134 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/shap/color_bar.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2120 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/shap/resident_intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2024-05-19 17:46:48.000000 Simba-UW-tf-dev-1.92.5/simba/assets/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 17:55:12.000000 Simba-UW-tf-dev-1.92.5/simba/assets/lookups/
+-rw-r--r--   0 simon      (501) staff       (20)   270783 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/lookups/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)     2987 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/lookups/feature_extraction_headers.csv
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:11.000000 Simba-UW-tf-dev-1.92.5/simba/assets/lookups/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    26256 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/lookups/critical_values_05.pickle
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/lookups/features.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/lookups/unsupervised_example_x.csv
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:41:54.000000 Simba-UW-tf-dev-1.92.5/simba/assets/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 17:55:12.000000 Simba-UW-tf-dev-1.92.5/simba/assets/stl/
+-rw-r--r--   0 simon      (501) staff       (20)   551576 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/stl/operant_tray.stl
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:31.000000 Simba-UW-tf-dev-1.92.5/simba/assets/stl/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    67647 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/stl/operant_lever.stl
+-rw-r--r--   0 simon      (501) staff       (20)    92896 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/stl/operant_walls.stl
+-rw-r--r--   0 simon      (501) staff       (20)  4759984 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/stl/grid_floor.stl
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 17:55:12.000000 Simba-UW-tf-dev-1.92.5/simba/assets/img/
+-rw-r--r--   0 simon      (501) staff       (20)   489479 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/img/splash_2024.mp4
+-rw-r--r--   0 simon      (501) staff       (20)    79863 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/img/bg_2024.png
+-rw-r--r--   0 simon      (501) staff       (20)   399272 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/img/about_me.png
+-rw-r--r--   0 simon      (501) staff       (20)   117108 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/img/splash.mp4
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:02.000000 Simba-UW-tf-dev-1.92.5/simba/assets/img/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)   322242 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/img/bg_2.png
+-rw-r--r--   0 simon      (501) staff       (20)      165 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/img/~$splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)    69267 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/img/splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)   204362 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/img/bg.png
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/UbuntuMono-Regular.ttf
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 17:55:12.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/
+-rw-r--r--   0 simon      (501) staff       (20)     1350 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/factory.png
+-rw-r--r--   0 simon      (501) staff       (20)     1413 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/cluster.png
+-rw-r--r--   0 simon      (501) staff       (20)     1340 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/load.png
+-rw-r--r--   0 simon      (501) staff       (20)     4507 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/gif.png
+-rw-r--r--   0 simon      (501) staff       (20)     4566 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/pose.png
+-rw-r--r--   0 simon      (501) staff       (20)     1943 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/features.png
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-09 15:42:22.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     4896 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/settings.png
+-rw-r--r--   0 simon      (501) staff       (20)     2090 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/stopwatch.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/link.png
+-rw-r--r--   0 simon      (501) staff       (20)    14250 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/dash_simba.css
+-rw-r--r--   0 simon      (501) staff       (20)      917 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/documentation.png
+-rw-r--r--   0 simon      (501) staff       (20)     4503 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/fps.png
+-rw-r--r--   0 simon      (501) staff       (20)     1299 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/dimensionality_reduction.png
+-rw-r--r--   0 simon      (501) staff       (20)     4823 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/roi.png
+-rw-r--r--   0 simon      (501) staff       (20)   171446 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/simba_logo_2.png
+-rw-r--r--   0 simon      (501) staff       (20)      920 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/superimpose.png
+-rw-r--r--   0 simon      (501) staff       (20)     1136 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/label.png
+-rw-r--r--   0 simon      (501) staff       (20)     1016 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/change.png
+-rw-r--r--   0 simon      (501) staff       (20)    59896 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/readthedocs_logo.png
+-rw-r--r--   0 simon      (501) staff       (20)     1124 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/crop.png
+-rw-r--r--   0 simon      (501) staff       (20)     2146 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/rotate.png
+-rw-r--r--   0 simon      (501) staff       (20)     1921 2024-02-26 14:29:54.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/circle.png
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:44:37.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1057 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/path.png
+-rw-r--r--   0 simon      (501) staff       (20)     1148 2024-02-26 20:39:14.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/polygon.png
+-rw-r--r--   0 simon      (501) staff       (20)      950 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/clip.png
+-rw-r--r--   0 simon      (501) staff       (20)     2121 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/restart.png
+-rw-r--r--   0 simon      (501) staff       (20)     4653 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/calipher.png
+-rw-r--r--   0 simon      (501) staff       (20)     1291 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/add_on.png
+-rw-r--r--   0 simon      (501) staff       (20)     4695 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/create.png
+-rw-r--r--   0 simon      (501) staff       (20)    78182 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/SimBA_logo.ico
+-rw-r--r--   0 simon      (501) staff       (20)     1067 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/print.png
+-rw-r--r--   0 simon      (501) staff       (20)     4653 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/clf.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 17:55:12.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/concat_icons/
+-rw-r--r--   0 simon      (501) staff       (20)     6027 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/concat_icons/mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     5654 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/concat_icons/vertical.png
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:44:45.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/concat_icons/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     5542 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/concat_icons/horizontal.png
+-rw-r--r--   0 simon      (501) staff       (20)     5939 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/concat_icons/mixed_mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     4256 2024-05-06 13:20:42.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/brightness.png
+-rw-r--r--   0 simon      (501) staff       (20)     2060 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/merge.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/clean.png
+-rw-r--r--   0 simon      (501) staff       (20)     4725 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/clf_2.png
+-rw-r--r--   0 simon      (501) staff       (20)     4795 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/visualize.png
+-rw-r--r--   0 simon      (501) staff       (20)     2142 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/concat.png
+-rw-r--r--   0 simon      (501) staff       (20)     1474 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/boris.png
+-rw-r--r--   0 simon      (501) staff       (20)     4804 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/frames.png
+-rw-r--r--   0 simon      (501) staff       (20)     2425 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/video.png
+-rw-r--r--   0 simon      (501) staff       (20)     2089 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/sample.png
+-rw-r--r--   0 simon      (501) staff       (20)     1471 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/metrics.png
+-rw-r--r--   0 simon      (501) staff       (20)     4555 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/grey.png
+-rw-r--r--   0 simon      (501) staff       (20)      930 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/exit.png
+-rw-r--r--   0 simon      (501) staff       (20)     4751 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/outlier.png
+-rw-r--r--   0 simon      (501) staff       (20)     4392 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/clahe.png
+-rw-r--r--   0 simon      (501) staff       (20)     4637 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/trash.png
+-rw-r--r--   0 simon      (501) staff       (20)     1239 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/about.png
+-rw-r--r--   0 simon      (501) staff       (20)     4666 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/convert.png
+-rw-r--r--   0 simon      (501) staff       (20)    93229 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/SimBA_logo.icns
+-rw-r--r--   0 simon      (501) staff       (20)      991 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/reorganize.png
+-rw-r--r--   0 simon      (501) staff       (20)     4784 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/browse.png
+-rw-r--r--   0 simon      (501) staff       (20)    30707 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/SimBA_logo.png
+-rw-r--r--   0 simon      (501) staff       (20)     2293 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/ethovision.png
+-rw-r--r--   0 simon      (501) staff       (20)     1018 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/icons/close.png
+-rw-r--r--   0 simon      (501) staff       (20)    13672 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/dash_simba_base.css
+-rw-r--r--   0 simon      (501) staff       (20)    31812 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.92.5/simba/assets/TheGoldenLab.PNG
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 17:55:12.000000 Simba-UW-tf-dev-1.92.5/Simba_UW_tf_dev.egg-info/
+-rw-r--r--   0 simon      (501) staff       (20)     2797 2024-05-19 17:55:12.000000 Simba-UW-tf-dev-1.92.5/Simba_UW_tf_dev.egg-info/PKG-INFO
+-rw-r--r--   0 simon      (501) staff       (20)    24636 2024-05-19 17:55:12.000000 Simba-UW-tf-dev-1.92.5/Simba_UW_tf_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 simon      (501) staff       (20)       44 2024-05-19 17:55:12.000000 Simba-UW-tf-dev-1.92.5/Simba_UW_tf_dev.egg-info/entry_points.txt
+-rw-r--r--   0 simon      (501) staff       (20)      857 2024-05-19 17:55:12.000000 Simba-UW-tf-dev-1.92.5/Simba_UW_tf_dev.egg-info/requires.txt
+-rw-r--r--   0 simon      (501) staff       (20)        6 2024-05-19 17:55:12.000000 Simba-UW-tf-dev-1.92.5/Simba_UW_tf_dev.egg-info/top_level.txt
+-rw-r--r--   0 simon      (501) staff       (20)        1 2024-05-19 17:55:12.000000 Simba-UW-tf-dev-1.92.5/Simba_UW_tf_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 simon      (501) staff       (20)    35127 2024-02-07 18:56:10.000000 Simba-UW-tf-dev-1.92.5/LICENSE
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 17:55:13.000000 Simba-UW-tf-dev-1.92.5/tests/
+-rw-r--r--   0 simon      (501) staff       (20)     4753 2024-04-11 20:40:04.000000 Simba-UW-tf-dev-1.92.5/tests/test_data_processors.py
+-rw-r--r--   0 simon      (501) staff       (20)    13415 2024-03-01 16:43:04.000000 Simba-UW-tf-dev-1.92.5/tests/test_circlular_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)    13399 2024-04-11 20:36:51.000000 Simba-UW-tf-dev-1.92.5/tests/test_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)    11863 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.92.5/tests/test_train_model_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     6525 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.92.5/tests/test_feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     1739 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.92.5/tests/test_utils_data.py
+-rw-r--r--   0 simon      (501) staff       (20)     8120 2024-03-01 19:06:25.000000 Simba-UW-tf-dev-1.92.5/tests/test_config_reader_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     1070 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.92.5/tests/test_outlier_correctors.py
+-rw-r--r--   0 simon      (501) staff       (20)     1596 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.92.5/tests/test_featurizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     8582 2024-05-12 17:13:08.000000 Simba-UW-tf-dev-1.92.5/tests/test_video_processors.py
+-rw-r--r--   0 simon      (501) staff       (20)     3554 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.92.5/tests/test_thirdparty_appenders.py
+-rw-r--r--   0 simon      (501) staff       (20)     3021 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.92.5/tests/test_validation_clips.py
+-rw-r--r--   0 simon      (501) staff       (20)     3921 2024-04-26 17:59:40.000000 Simba-UW-tf-dev-1.92.5/tests/test_roi_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)      318 2024-03-04 20:16:28.000000 Simba-UW-tf-dev-1.92.5/MANIFEST.in
+-rw-r--r--   0 simon      (501) staff       (20)    18478 2024-04-17 19:58:21.000000 Simba-UW-tf-dev-1.92.5/README.md
+-rw-r--r--   0 simon      (501) staff       (20)     1426 2024-05-19 17:55:09.000000 Simba-UW-tf-dev-1.92.5/setup.py
+-rw-r--r--   0 simon      (501) staff       (20)       38 2024-05-19 17:55:13.000000 Simba-UW-tf-dev-1.92.5/setup.cfg
```

### Comparing `Simba-UW-tf-dev-1.92.4/PKG-INFO` & `Simba-UW-tf-dev-1.92.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.92.4
+Version: 1.92.5
 Summary: Toolkit for computer classification of behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.92.4/simba/ui/.DS_Store` & `Simba-UW-tf-dev-1.92.5/simba/ui/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/mutual_exclusivity_pop_up.py` & `Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/mutual_exclusivity_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/csv_2_parquet_pop_up.py` & `Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/csv_2_parquet_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/quick_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/quick_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/batch_preprocess_pop_up.py` & `Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/batch_preprocess_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/heatmap_location_pop_up.py` & `Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/heatmap_location_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/clf_probability_plot_pop_up.py` & `Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/clf_probability_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/movement_analysis_pop_up.py` & `Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/movement_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py` & `Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/clf_plot_pop_up.py` & `Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/clf_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/path_plot_pop_up.py` & `Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/remove_roi_features_pop_up.py` & `Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/remove_roi_features_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/targeted_annotation_clips_pop_up.py` & `Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/targeted_annotation_clips_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/smoothing_interpolation_pop_up.py` & `Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/smoothing_interpolation_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/roi_size_standardizer_popup.py` & `Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/roi_size_standardizer_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py` & `Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/roi_analysis_pop_up.py` & `Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/roi_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/outlier_settings_pop_up.py` & `Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/outlier_settings_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/gantt_pop_up.py` & `Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/gantt_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/clf_validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/clf_validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/severity_analysis_pop_up.py` & `Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/severity_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/fsttc_pop_up.py` & `Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/fsttc_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/kleinberg_pop_up.py` & `Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/kleinberg_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py` & `Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/spontaneous_alternation_pop_up.py` & `Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/spontaneous_alternation_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/pose_reorganizer_pop_up.py` & `Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/pose_reorganizer_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/animal_directing_other_animals_pop_up.py` & `Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/animal_directing_other_animals_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/append_roi_features_animals_pop_up.py` & `Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/append_roi_features_animals_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/clf_by_timebins_pop_up.py` & `Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/clf_by_timebins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/heatmap_clf_pop_up.py` & `Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/heatmap_clf_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/data_plot_pop_up.py` & `Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/data_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/roi_features_plot_pop_up.py` & `Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/roi_features_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/pup_retrieval_pop_up.py` & `Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/pup_retrieval_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/boolean_conditional_slicer_pup_up.py` & `Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/boolean_conditional_slicer_pup_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/about_simba_pop_up.py` & `Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/about_simba_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py` & `Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/roi_tracking_plot_pop_up.py` & `Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/roi_tracking_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py` & `Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/directing_animal_to_bodypart_plot_pop_up.py` & `Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/directing_animal_to_bodypart_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/clf_add_remove_print_pop_up.py` & `Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/clf_add_remove_print_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/video_processing_pop_up.py` & `Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/video_processing_pop_up.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 __author__ = "Simon Nilsson"
 
 import glob
 import os
 import subprocess
 import sys
 import threading
+import numpy as np
 from datetime import datetime
 from tkinter import *
 from typing import Optional, Union
 
 from PIL import Image, ImageTk
 
 import simba
@@ -27,14 +28,15 @@
                                 check_int, check_nvidea_gpu_available,
                                 check_that_hhmmss_start_is_before_end)
 from simba.utils.data import convert_roi_definitions
 from simba.utils.enums import Dtypes, Formats, Keys, Links, Options, Paths
 from simba.utils.errors import (CountError, FrameRangeError, InvalidInputError,
                                 MixedMosaicError, NoChoosenClassifierError,
                                 NoFilesFoundError, NotDirectoryError)
+from simba.utils.lookups import get_color_dict
 from simba.utils.printing import SimbaTimer, stdout_success
 from simba.utils.read_write import (
     check_if_hhmmss_timestamp_is_valid_part_of_video,
     concatenate_videos_in_folder, find_all_videos_in_directory,
     find_files_of_filetypes_in_directory, get_fn_ext, get_video_meta_data,
     seconds_to_timestamp, str_2_bool)
 from simba.video_processors.brightness_contrast_ui import \
@@ -53,15 +55,15 @@
     convert_video_powerpoint_compatible_format, copy_img_folder,
     crop_multiple_videos, crop_multiple_videos_circles,
     crop_multiple_videos_polygons, crop_single_video, crop_single_video_circle,
     crop_single_video_polygon, downsample_video, extract_frame_range,
     extract_frames_single_video, frames_to_movie, gif_creator,
     multi_split_video, remove_beginning_of_video, resize_videos_by_height,
     resize_videos_by_width, superimpose_frame_count, video_concatenator,
-    video_to_greyscale)
+    video_to_greyscale, watermark_video, superimpose_video_progressbar, superimpose_elapsed_time)
 
 sys.setrecursionlimit(10**7)
 
 
 class CLAHEPopUp(PopUpMixin):
     def __init__(self):
         super().__init__(title="CLAHE VIDEO CONVERSION")
@@ -2563,11 +2565,191 @@
             check_if_dir_exists(in_dir=video_path, source=self.__class__.__name__)
         codec = self.MOV_CODEC_LK[self.codec_dropdown.getChoices()]
         quality = int(self.quality_dropdown.getChoices())
         threading.Thread(target=convert_to_mov(path=video_path, codec=codec, quality=quality))
 
 
 
+class SuperimposeWatermarkPopUp(PopUpMixin):
+    def __init__(self):
+        PopUpMixin.__init__(self, title="WATERMARK VIDEOS")
+        self.LOCATIONS = {'TOP LEFT': 'top_left', 'TOP RIGHT': 'top_right', 'BOTTOM LEFT': 'bottom_left', 'BOTTOM RIGHT': 'bottom_right', 'CENTER': 'center'}
+        settings_frm = CreateLabelFrameWithIcon(parent=self.main_frm, header="SETTINGS", icon_name=Keys.DOCUMENTATION.value, icon_link=Links.VIDEO_TOOLS.value)
+        opacities = [round(x, 1) for x in list(np.arange(0.1, 1.1, 0.1))]
+        self.selected_img = FileSelect(settings_frm, "WATERMARK IMAGE PATH:", title="Select an image file", file_types=[("VIDEO", Options.ALL_IMAGE_FORMAT_OPTIONS.value)], lblwidth=25)
+        self.location_dropdown = DropDownMenu(settings_frm, "WATERMARK LOCATION:", list(self.LOCATIONS.keys()), labelwidth=25)
+        self.opacity_dropdown = DropDownMenu(settings_frm, "WATERMARK OPACITY:", opacities, labelwidth=25)
+        self.size_dropdown = DropDownMenu(settings_frm, "WATERMARK SCALE %:", list(range(5, 100, 5)), labelwidth=25)
+
+        self.location_dropdown.setChoices('TOP LEFT')
+        self.opacity_dropdown.setChoices(50)
+        self.size_dropdown.setChoices(5)
+
+        settings_frm.grid(row=0, column=0, sticky=NW)
+        self.selected_img.grid(row=0, column=0, sticky=NW)
+        self.location_dropdown.grid(row=1, column=0, sticky=NW)
+        self.opacity_dropdown.grid(row=2, column=0, sticky=NW)
+        self.size_dropdown.grid(row=3, column=0, sticky=NW)
+
+        single_video_frm = CreateLabelFrameWithIcon(parent=self.main_frm, header="SINGLE VIDEO - SUPERIMPOSE WATERMARK", icon_name=Keys.DOCUMENTATION.value, icon_link=Links.VIDEO_TOOLS.value)
+        self.selected_video = FileSelect(single_video_frm, "VIDEO PATH:", title="Select a video file", lblwidth=25, file_types=[("VIDEO FILE", Options.ALL_VIDEO_FORMAT_STR_OPTIONS.value)])
+        single_video_run = Button(single_video_frm, text="RUN - SINGLE VIDEO", command=lambda: self.run(multiple=False))
+
+        single_video_frm.grid(row=1, column=0, sticky="NW")
+        self.selected_video.grid(row=0, column=0, sticky="NW")
+        single_video_run.grid(row=1, column=0, sticky="NW")
+
+        multiple_videos_frm = CreateLabelFrameWithIcon(parent=self.main_frm, header="MULTIPLE VIDEOS - SUPERIMPOSE WATERMARK", icon_name=Keys.DOCUMENTATION.value, icon_link=Links.VIDEO_TOOLS.value)
+        self.selected_video_dir = FolderSelect(multiple_videos_frm, "VIDEO DIRECTORY PATH:", title="Select a video directory", lblwidth=25)
+        multiple_videos_run = Button(multiple_videos_frm, text="RUN - MULTIPLE VIDEOS", command=lambda: self.run(multiple=True))
+
+        multiple_videos_frm.grid(row=2, column=0, sticky="NW")
+        self.selected_video_dir.grid(row=0, column=0, sticky="NW")
+        multiple_videos_run.grid(row=1, column=0, sticky="NW")
+        self.main_frm.mainloop()
+
+    def run(self, multiple: bool):
+        img_path = self.selected_img.file_path
+        loc = self.location_dropdown.getChoices()
+        loc = self.LOCATIONS[loc]
+        opacity = float(self.opacity_dropdown.getChoices())
+        size = float(int(self.size_dropdown.getChoices()) / 100)
+        if size == 1.0: size = size - 0.001
+        check_file_exist_and_readable(file_path=img_path)
+        if not multiple:
+            data_path = self.selected_video.file_path
+            check_file_exist_and_readable(file_path=data_path)
+        else:
+            data_path = self.selected_video_dir.folder_path
+            check_if_dir_exists(in_dir=data_path)
+
+        threading.Thread(target=watermark_video(video_path=data_path,
+                                                watermark_path=img_path, position=loc,
+                                                opacity=opacity,
+                                                scale=size)).start()
+#SuperimposeWatermarkPopUp()
+
+
+class SuperimposeTimerPopUp(PopUpMixin):
+    def __init__(self):
+        PopUpMixin.__init__(self, title="SUPER-IMPOSE TIME ON VIDEOS")
+        self.LOCATIONS = {'TOP LEFT': 'top_left', 'TOP RIGHT': 'top_right', 'TOP MIDDLE': 'top_middle', 'BOTTOM LEFT': 'bottom_left', 'BOTTOM RIGHT': 'bottom_right', 'BOTTOM MIDDLE': 'bottom_middle'}
+        settings_frm = CreateLabelFrameWithIcon(parent=self.main_frm, header="SETTINGS", icon_name=Keys.DOCUMENTATION.value, icon_link=Links.VIDEO_TOOLS.value)
+        self.color_dict = get_color_dict()
+
+        self.location_dropdown = DropDownMenu(settings_frm, "TIMER LOCATION:", list(self.LOCATIONS.keys()), labelwidth=25)
+        self.font_size_dropdown = DropDownMenu(settings_frm, "FONT SIZE:", list(range(20, 100, 5)), labelwidth=25)
+        self.font_color_dropdown = DropDownMenu(settings_frm, "FONT COLOR:", list(self.color_dict.keys()), labelwidth=25)
+        self.font_border_dropdown = DropDownMenu(settings_frm, "FONT BORDER COLOR:", list(self.color_dict.keys()), labelwidth=25)
+        self.font_border_width_dropdown = DropDownMenu(settings_frm, "FONT BORDER WIDTH:", list(range(2, 52, 2)), labelwidth=25)
+
+        self.location_dropdown.setChoices('TOP LEFT')
+        self.font_size_dropdown.setChoices(20)
+        self.font_color_dropdown.setChoices('White')
+        self.font_border_dropdown.setChoices('Black')
+        self.font_border_width_dropdown.setChoices(2)
+
+        settings_frm.grid(row=0, column=0, sticky=NW)
+        self.location_dropdown.grid(row=0, column=0, sticky=NW)
+        self.font_size_dropdown.grid(row=1, column=0, sticky=NW)
+        self.font_color_dropdown.grid(row=2, column=0, sticky=NW)
+        self.font_border_dropdown.grid(row=3, column=0, sticky=NW)
+        self.font_border_width_dropdown.grid(row=4, column=0, sticky=NW)
+
+        single_video_frm = CreateLabelFrameWithIcon(parent=self.main_frm, header="SINGLE VIDEO - SUPERIMPOSE TIMER", icon_name=Keys.DOCUMENTATION.value, icon_link=Links.VIDEO_TOOLS.value)
+        self.selected_video = FileSelect(single_video_frm, "VIDEO PATH:", title="Select a video file", lblwidth=25, file_types=[("VIDEO FILE", Options.ALL_VIDEO_FORMAT_STR_OPTIONS.value)])
+        single_video_run = Button(single_video_frm, text="RUN - SINGLE VIDEO", command=lambda: self.run(multiple=False))
+
+        single_video_frm.grid(row=1, column=0, sticky="NW")
+        self.selected_video.grid(row=0, column=0, sticky="NW")
+        single_video_run.grid(row=1, column=0, sticky="NW")
+
+        multiple_videos_frm = CreateLabelFrameWithIcon(parent=self.main_frm, header="MULTIPLE VIDEOS - SUPERIMPOSE TIMER", icon_name=Keys.DOCUMENTATION.value, icon_link=Links.VIDEO_TOOLS.value)
+        self.selected_video_dir = FolderSelect(multiple_videos_frm, "VIDEO DIRECTORY PATH:", title="Select a video directory", lblwidth=25)
+        multiple_videos_run = Button(multiple_videos_frm, text="RUN - MULTIPLE VIDEOS", command=lambda: self.run(multiple=True))
+
+        multiple_videos_frm.grid(row=2, column=0, sticky="NW")
+        self.selected_video_dir.grid(row=0, column=0, sticky="NW")
+        multiple_videos_run.grid(row=1, column=0, sticky="NW")
+        self.main_frm.mainloop()
+
+    def run(self, multiple: bool):
+        loc = self.location_dropdown.getChoices()
+        loc = self.LOCATIONS[loc]
+        font_size = int(self.font_size_dropdown.getChoices())
+        font_clr = self.font_color_dropdown.getChoices()
+        font_border_clr = self.font_border_dropdown.getChoices()
+        font_border_width = int(self.font_border_width_dropdown.getChoices())
+        if not multiple:
+            data_path = self.selected_video.file_path
+            check_file_exist_and_readable(file_path=data_path)
+        else:
+            data_path = self.selected_video_dir.folder_path
+            check_if_dir_exists(in_dir=data_path)
+
+        threading.Thread(target=superimpose_elapsed_time(video_path=data_path,
+                                                         font_size=font_size,
+                                                         font_color=font_clr,
+                                                         font_border_color=font_border_clr,
+                                                         font_border_width=font_border_width,
+                                                         position=loc)).start()
+
+
+class SuperimposeProgressBarPopUp(PopUpMixin):
+    def __init__(self):
+        PopUpMixin.__init__(self, title="SUPER-IMPOSE PROGRESS BAR ON VIDEOS")
+        self.LOCATIONS = {'TOP': 'top', 'BOTTOM': 'bottom'}
+        settings_frm = CreateLabelFrameWithIcon(parent=self.main_frm, header="SETTINGS", icon_name=Keys.DOCUMENTATION.value, icon_link=Links.VIDEO_TOOLS.value)
+        self.color_dict = get_color_dict()
+        size_lst = list(range(0, 110, 5))
+        size_lst[0] = 1
+        self.bar_loc_dropdown = DropDownMenu(settings_frm, "PROGRESS BAR LOCATION:", list(self.LOCATIONS.keys()), labelwidth=25)
+        self.bar_color_dropdown = DropDownMenu(settings_frm, "PROGRESS BAR COLOR:", list(self.color_dict.keys()), labelwidth=25)
+        self.bar_size_dropdown = DropDownMenu(settings_frm, "PROGRESS BAR HEIGHT (%):", size_lst, labelwidth=25)
+        self.bar_color_dropdown.setChoices('Red')
+        self.bar_size_dropdown.setChoices(10)
+        self.bar_loc_dropdown.setChoices('BOTTOM')
+
+        settings_frm.grid(row=0, column=0, sticky=NW)
+        self.bar_loc_dropdown.grid(row=0, column=0, sticky=NW)
+        self.bar_color_dropdown.grid(row=1, column=0, sticky=NW)
+        self.bar_size_dropdown.grid(row=2, column=0, sticky=NW)
+
+        single_video_frm = CreateLabelFrameWithIcon(parent=self.main_frm, header="SINGLE VIDEO - SUPERIMPOSE PROGRESS BAR", icon_name=Keys.DOCUMENTATION.value, icon_link=Links.VIDEO_TOOLS.value)
+        self.selected_video = FileSelect(single_video_frm, "VIDEO PATH:", title="Select a video file", lblwidth=25, file_types=[("VIDEO FILE", Options.ALL_VIDEO_FORMAT_STR_OPTIONS.value)])
+        single_video_run = Button(single_video_frm, text="RUN - SINGLE VIDEO", command=lambda: self.run(multiple=False))
+
+        single_video_frm.grid(row=1, column=0, sticky="NW")
+        self.selected_video.grid(row=0, column=0, sticky="NW")
+        single_video_run.grid(row=1, column=0, sticky="NW")
+
+        multiple_videos_frm = CreateLabelFrameWithIcon(parent=self.main_frm, header="MULTIPLE VIDEOS - SUPERIMPOSE PROGRESS BAR", icon_name=Keys.DOCUMENTATION.value, icon_link=Links.VIDEO_TOOLS.value)
+        self.selected_video_dir = FolderSelect(multiple_videos_frm, "VIDEO DIRECTORY PATH:", title="Select a video directory", lblwidth=25)
+        multiple_videos_run = Button(multiple_videos_frm, text="RUN - MULTIPLE VIDEOS", command=lambda: self.run(multiple=True))
+
+        multiple_videos_frm.grid(row=2, column=0, sticky="NW")
+        self.selected_video_dir.grid(row=0, column=0, sticky="NW")
+        multiple_videos_run.grid(row=1, column=0, sticky="NW")
+        self.main_frm.mainloop()
+
+    def run(self, multiple: bool):
+        loc = self.bar_loc_dropdown.getChoices()
+        loc = self.LOCATIONS[loc]
+        bar_clr = self.bar_color_dropdown.getChoices()
+        bar_size = int(self.bar_size_dropdown.getChoices())
+        if not multiple:
+            data_path = self.selected_video.file_path
+            check_file_exist_and_readable(file_path=data_path)
+        else:
+            data_path = self.selected_video_dir.folder_path
+            check_if_dir_exists(in_dir=data_path)
+
+        threading.Thread(target=superimpose_video_progressbar(video_path=data_path,
+                                                              bar_height=bar_size,
+                                                              color=bar_clr,
+                                                              position=loc)).start()
+
+
 
 
 # ClipMultipleVideosByFrameNumbers
 # ClipMultipleVideosByFrameNumbers(data_dir='/Users/simon/Desktop/envs/simba/troubleshooting/beepboop174/project_folder/videos/test', save_dir='/Users/simon/Desktop/envs/simba/troubleshooting/beepboop174/project_folder/videos/clipped')
```

### Comparing `Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/clf_by_roi_pop_up.py` & `Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/clf_by_roi_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/make_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/make_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/direction_animal_to_bodypart_settings_pop_up.py` & `Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/direction_animal_to_bodypart_settings_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py` & `Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/archive_files_pop_up.py` & `Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/archive_files_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/pose_bp_drop_pop_up.py` & `Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/pose_bp_drop_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/distance_plot_pop_up.py` & `Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/distance_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/subset_feature_extractor_pop_up.py` & `Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/subset_feature_extractor_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py` & `Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.92.5/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/ui/video_info_ui.py` & `Simba-UW-tf-dev-1.92.5/simba/ui/video_info_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/ui/user_defined_pose_creator.py` & `Simba-UW-tf-dev-1.92.5/simba/ui/user_defined_pose_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/ui/create_project_ui.py` & `Simba-UW-tf-dev-1.92.5/simba/ui/create_project_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/ui/tkinter_functions.py` & `Simba-UW-tf-dev-1.92.5/simba/ui/tkinter_functions.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/ui/machine_model_settings_ui.py` & `Simba-UW-tf-dev-1.92.5/simba/ui/machine_model_settings_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/labelling/labelling_interface.py` & `Simba-UW-tf-dev-1.92.5/simba/labelling/labelling_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/labelling/targeted_annotations_clips.py` & `Simba-UW-tf-dev-1.92.5/simba/labelling/targeted_annotations_clips.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/labelling/extract_labelled_frames.py` & `Simba-UW-tf-dev-1.92.5/simba/labelling/extract_labelled_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/labelling/labelling_advanced_interface.py` & `Simba-UW-tf-dev-1.92.5/simba/labelling/labelling_advanced_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/labelling/play_annotation_video.py` & `Simba-UW-tf-dev-1.92.5/simba/labelling/play_annotation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/unsupervised/dbcv_calculator.py` & `Simba-UW-tf-dev-1.92.5/simba/unsupervised/dbcv_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/unsupervised/cluster_validation_calculator.py` & `Simba-UW-tf-dev-1.92.5/simba/unsupervised/cluster_validation_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/unsupervised/enums.py` & `Simba-UW-tf-dev-1.92.5/simba/unsupervised/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.92.5/simba/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/unsupervised/cluster_video_visualizer.py` & `Simba-UW-tf-dev-1.92.5/simba/unsupervised/cluster_video_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/unsupervised/pop_ups/cluster_videos_popup.py` & `Simba-UW-tf-dev-1.92.5/simba/unsupervised/pop_ups/cluster_videos_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/unsupervised/pop_ups/transform_cluster_popup.py` & `Simba-UW-tf-dev-1.92.5/simba/unsupervised/pop_ups/transform_cluster_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/unsupervised/pop_ups/embedding_correlations_popup.py` & `Simba-UW-tf-dev-1.92.5/simba/unsupervised/pop_ups/embedding_correlations_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/unsupervised/pop_ups/.DS_Store` & `Simba-UW-tf-dev-1.92.5/simba/unsupervised/pop_ups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/unsupervised/pop_ups/transform_dim_reduction_popup.py` & `Simba-UW-tf-dev-1.92.5/simba/unsupervised/pop_ups/transform_dim_reduction_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/unsupervised/pop_ups/fit_dim_reduction_popup.py` & `Simba-UW-tf-dev-1.92.5/simba/unsupervised/pop_ups/fit_dim_reduction_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/unsupervised/pop_ups/data_extractor_popup.py` & `Simba-UW-tf-dev-1.92.5/simba/unsupervised/pop_ups/data_extractor_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/unsupervised/pop_ups/cluster_validation_pop_up.py` & `Simba-UW-tf-dev-1.92.5/simba/unsupervised/pop_ups/cluster_validation_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/unsupervised/pop_ups/fit_cluster_popup.py` & `Simba-UW-tf-dev-1.92.5/simba/unsupervised/pop_ups/fit_cluster_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/unsupervised/pop_ups/clusterer_comparison_popup.py` & `Simba-UW-tf-dev-1.92.5/simba/unsupervised/pop_ups/clusterer_comparison_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/unsupervised/pop_ups/grid_search_visualizer_popup.py` & `Simba-UW-tf-dev-1.92.5/simba/unsupervised/pop_ups/grid_search_visualizer_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/unsupervised/pop_ups/cluster_xai_popup.py` & `Simba-UW-tf-dev-1.92.5/simba/unsupervised/pop_ups/cluster_xai_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/unsupervised/pop_ups/cluster_frequentist_stats_popup.py` & `Simba-UW-tf-dev-1.92.5/simba/unsupervised/pop_ups/cluster_frequentist_stats_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/unsupervised/pop_ups/print_embedding_info_popup.py` & `Simba-UW-tf-dev-1.92.5/simba/unsupervised/pop_ups/print_embedding_info_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/unsupervised/dataset_creator.py` & `Simba-UW-tf-dev-1.92.5/simba/unsupervised/dataset_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/unsupervised/unsupervised_main.py` & `Simba-UW-tf-dev-1.92.5/simba/unsupervised/unsupervised_main.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/unsupervised/grid_search_visualizers.py` & `Simba-UW-tf-dev-1.92.5/simba/unsupervised/grid_search_visualizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/unsupervised/data_extractor.py` & `Simba-UW-tf-dev-1.92.5/simba/unsupervised/data_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/unsupervised/outlier_detector.py` & `Simba-UW-tf-dev-1.92.5/simba/unsupervised/outlier_detector.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/unsupervised/cluster_frequentist_calculator.py` & `Simba-UW-tf-dev-1.92.5/simba/unsupervised/cluster_frequentist_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/unsupervised/embedding_correlation_calculator.py` & `Simba-UW-tf-dev-1.92.5/simba/unsupervised/embedding_correlation_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/unsupervised/cluster_xai_calculator.py` & `Simba-UW-tf-dev-1.92.5/simba/unsupervised/cluster_xai_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/unsupervised/umap_embedder.py` & `Simba-UW-tf-dev-1.92.5/simba/unsupervised/umap_embedder.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/unsupervised/clusterer_comparison_calculator.py` & `Simba-UW-tf-dev-1.92.5/simba/unsupervised/clusterer_comparison_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/unsupervised/bout_aggregator.py` & `Simba-UW-tf-dev-1.92.5/simba/unsupervised/bout_aggregator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/unsupervised/data_map.yaml` & `Simba-UW-tf-dev-1.92.5/simba/unsupervised/data_map.yaml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/unsupervised/hdbscan_clusterer.py` & `Simba-UW-tf-dev-1.92.5/simba/unsupervised/hdbscan_clusterer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/unsupervised/tsne.py` & `Simba-UW-tf-dev-1.92.5/simba/unsupervised/tsne.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/bounding_box_tools/agg_boundary_stats.py` & `Simba-UW-tf-dev-1.92.5/simba/bounding_box_tools/agg_boundary_stats.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/bounding_box_tools/boundary_menus.py` & `Simba-UW-tf-dev-1.92.5/simba/bounding_box_tools/boundary_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/bounding_box_tools/boundary_statistics.py` & `Simba-UW-tf-dev-1.92.5/simba/bounding_box_tools/boundary_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/bounding_box_tools/find_boundaries.py` & `Simba-UW-tf-dev-1.92.5/simba/bounding_box_tools/find_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/bounding_box_tools/visualize_boundaries.py` & `Simba-UW-tf-dev-1.92.5/simba/bounding_box_tools/visualize_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/.DS_Store` & `Simba-UW-tf-dev-1.92.5/simba/.DS_Store`

 * *Files 0% similar despite different names*

```diff
@@ -519,249 +519,249 @@
 00002060: 57f9 c541 0000 000b 005f 005f 0070 0079  W..A....._._.p.y
 00002070: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
 00002080: 6444 626c 6f62 0000 0008 f19f 2831 57f9  dDblob......(1W.
 00002090: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 000020a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
 000020b0: 636f 6d70 0000 0000 0001 0000 0000 0006  comp............
 000020c0: 0061 0073 0073 0065 0074 0073 6277 7370  .a.s.s.e.t.sbwsp
-000020d0: 626c 6f62 0000 00b8 6270 6c69 7374 3030  blob....bplist00
+000020d0: 626c 6f62 0000 00b7 6270 6c69 7374 3030  blob....bplist00
 000020e0: d601 0203 0405 0607 0807 080b 085d 5368  .............]Sh
 000020f0: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
 00002100: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
 00002110: 6965 775f 1014 436f 6e74 6169 6e65 7253  iew_..ContainerS
 00002120: 686f 7753 6964 6562 6172 5c57 696e 646f  howSidebar\Windo
 00002130: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
-00002140: 6261 7208 0908 095f 1018 7b7b 3236 302c  bar...._..{{260,
-00002150: 2033 3239 7d2c 207b 3932 302c 2034 3336   329}, {920, 436
-00002160: 7d7d 0908 1523 2f3b 525f 6b6c 6d6e 6f8a  }}...#/;R_klmno.
-00002170: 0000 0000 0000 0101 0000 0000 0000 000d  ................
-00002180: 0000 0000 0000 0000 0000 0000 0000 008b  ................
-00002190: 0000 0006 0061 0073 0073 0065 0074 0073  .....a.s.s.e.t.s
-000021a0: 6c67 3153 636f 6d70 0000 0000 008a 1694  lg1Scomp........
-000021b0: 0000 0006 0061 0073 0073 0065 0074 0073  .....a.s.s.e.t.s
-000021c0: 6d6f 4444 626c 6f62 0000 0008 ee16 90c8  moDDblob........
-000021d0: abba c541 0000 0006 0061 0073 0073 0065  ...A.....a.s.s.e
-000021e0: 0074 0073 6d6f 6444 626c 6f62 0000 0008  .t.smodDblob....
-000021f0: ee16 90c8 abba c541 0000 0006 0061 0073  .......A.....a.s
-00002200: 0073 0065 0074 0073 7068 3153 636f 6d70  .s.e.t.sph1Scomp
-00002210: 0000 0000 008d f000 0000 0006 0061 0073  .............a.s
-00002220: 0073 0065 0074 0073 7653 726e 6c6f 6e67  .s.e.t.svSrnlong
-00002230: 0000 0001 0000 0012 0062 006f 0075 006e  .........b.o.u.n
-00002240: 0064 0069 006e 0067 005f 0062 006f 0078  .d.i.n.g._.b.o.x
-00002250: 005f 0074 006f 006f 006c 0073 6c67 3153  ._.t.o.o.l.slg1S
-00002260: 636f 6d70 0000 0000 0003 222b 0000 0012  comp......"+....
-00002270: 0062 006f 0075 006e 0064 0069 006e 0067  .b.o.u.n.d.i.n.g
-00002280: 005f 0062 006f 0078 005f 0074 006f 006f  ._.b.o.x._.t.o.o
-00002290: 006c 0073 6d6f 4444 626c 6f62 0000 0008  .l.smoDDblob....
-000022a0: ac91 fad1 2eba c541 0000 0012 0062 006f  .......A.....b.o
-000022b0: 0075 006e 0064 0069 006e 0067 005f 0062  .u.n.d.i.n.g._.b
-000022c0: 006f 0078 005f 0074 006f 006f 006c 0073  .o.x._.t.o.o.l.s
-000022d0: 6d6f 6444 626c 6f62 0000 0008 ac91 fad1  modDblob........
-000022e0: 2eba c541 0000 0012 0062 006f 0075 006e  ...A.....b.o.u.n
-000022f0: 0064 0069 006e 0067 005f 0062 006f 0078  .d.i.n.g._.b.o.x
-00002300: 005f 0074 006f 006f 006c 0073 7068 3153  ._.t.o.o.l.sph1S
-00002310: 636f 6d70 0000 0000 0003 d000 0000 000f  comp............
-00002320: 0063 0075 0065 005f 006c 0069 0067 0068  .c.u.e._.l.i.g.h
-00002330: 0074 005f 0074 006f 006f 006c 0073 6c67  .t._.t.o.o.l.slg
-00002340: 3153 636f 6d70 0000 0000 0002 b278 0000  1Scomp.......x..
-00002350: 000f 0063 0075 0065 005f 006c 0069 0067  ...c.u.e._.l.i.g
-00002360: 0068 0074 005f 0074 006f 006f 006c 0073  .h.t._.t.o.o.l.s
-00002370: 6d6f 4444 626c 6f62 0000 0008 e82a d127  moDDblob.....*.'
-00002380: 4bed c541 0000 000f 0063 0075 0065 005f  K..A.....c.u.e._
-00002390: 006c 0069 0067 0068 0074 005f 0074 006f  .l.i.g.h.t._.t.o
-000023a0: 006f 006c 0073 6d6f 6444 626c 6f62 0000  .o.l.smodDblob..
-000023b0: 0008 e82a d127 4bed c541 0000 000f 0063  ...*.'K..A.....c
-000023c0: 0075 0065 005f 006c 0069 0067 0068 0074  .u.e._.l.i.g.h.t
-000023d0: 005f 0074 006f 006f 006c 0073 7068 3153  ._.t.o.o.l.sph1S
-000023e0: 636f 6d70 0000 0000 0003 8000 0000 0008  comp............
-000023f0: 0064 0061 0073 0068 005f 0061 0070 0070  .d.a.s.h._.a.p.p
-00002400: 6c67 3153 636f 6d70 0000 0000 0001 e92a  lg1Scomp.......*
-00002410: 0000 0008 0064 0061 0073 0068 005f 0061  .....d.a.s.h._.a
-00002420: 0070 0070 6d6f 4444 626c 6f62 0000 0008  .p.pmoDDblob....
-00002430: de5f c487 0aba c541 0000 0008 0064 0061  ._.....A.....d.a
-00002440: 0073 0068 005f 0061 0070 0070 6d6f 6444  .s.h._.a.p.pmodD
-00002450: 626c 6f62 0000 0008 de5f c487 0aba c541  blob....._.....A
-00002460: 0000 0008 0064 0061 0073 0068 005f 0061  .....d.a.s.h._.a
-00002470: 0070 0070 7068 3153 636f 6d70 0000 0000  .p.pph1Scomp....
-00002480: 0002 0000 0000 000f 0064 0061 0074 0061  .........d.a.t.a
-00002490: 005f 0070 0072 006f 0063 0065 0073 0073  ._.p.r.o.c.e.s.s
-000024a0: 006f 0072 0073 6c67 3153 636f 6d70 0000  .o.r.slg1Scomp..
-000024b0: 0000 0007 3126 0000 000f 0064 0061 0074  ....1&.....d.a.t
-000024c0: 0061 005f 0070 0072 006f 0063 0065 0073  .a._.p.r.o.c.e.s
-000024d0: 0073 006f 0072 0073 6d6f 4444 626c 6f62  .s.o.r.smoDDblob
-000024e0: 0000 0008 16d0 7829 13ee c541 0000 000f  ......x)...A....
-000024f0: 0064 0061 0074 0061 005f 0070 0072 006f  .d.a.t.a._.p.r.o
-00002500: 0063 0065 0073 0073 006f 0072 0073 6d6f  .c.e.s.s.o.r.smo
-00002510: 6444 626c 6f62 0000 0008 16d0 7829 13ee  dDblob......x)..
-00002520: c541 0000 000f 0064 0061 0074 0061 005f  .A.....d.a.t.a._
-00002530: 0070 0072 006f 0063 0065 0073 0073 006f  .p.r.o.c.e.s.s.o
-00002540: 0072 0073 7068 3153 636f 6d70 0000 0000  .r.sph1Scomp....
-00002550: 0009 1000 0000 0012 0066 0065 0061 0074  .........f.e.a.t
-00002560: 0075 0072 0065 005f 0065 0078 0074 0072  .u.r.e._.e.x.t.r
-00002570: 0061 0063 0074 006f 0072 0073 6277 7370  .a.c.t.o.r.sbwsp
-00002580: 626c 6f62 0000 00b9 6270 6c69 7374 3030  blob....bplist00
-00002590: d601 0203 0405 0607 0807 080b 085d 5368  .............]Sh
-000025a0: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
-000025b0: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
-000025c0: 6965 775f 1014 436f 6e74 6169 6e65 7253  iew_..ContainerS
-000025d0: 686f 7753 6964 6562 6172 5c57 696e 646f  howSidebar\Windo
-000025e0: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
-000025f0: 6261 7208 0908 095f 1019 7b7b 3939 2c20  bar...._..{{99, 
-00002600: 2d31 3636 7d2c 207b 3132 3833 2c20 3638  -166}, {1283, 68
-00002610: 397d 7d09 0815 232f 3b52 5f6b 6c6d 6e6f  9}}...#/;R_klmno
-00002620: 8b00 0000 0000 0001 0100 0000 0000 0000  ................
-00002630: 0d00 0000 0000 0000 0000 0000 0000 0000  ................
-00002640: 8c00 0000 1200 6600 6500 6100 7400 7500  ......f.e.a.t.u.
-00002650: 7200 6500 5f00 6500 7800 7400 7200 6100  r.e._.e.x.t.r.a.
-00002660: 6300 7400 6f00 7200 736c 6731 5363 6f6d  c.t.o.r.slg1Scom
-00002670: 7000 0000 0000 0c9d 2000 0000 1200 6600  p....... .....f.
-00002680: 6500 6100 7400 7500 7200 6500 5f00 6500  e.a.t.u.r.e._.e.
-00002690: 7800 7400 7200 6100 6300 7400 6f00 7200  x.t.r.a.c.t.o.r.
-000026a0: 736d 6f44 4462 6c6f 6200 0000 08c5 75b6  smoDDblob.....u.
-000026b0: 0b20 c9c5 4100 0000 1200 6600 6500 6100  . ..A.....f.e.a.
-000026c0: 7400 7500 7200 6500 5f00 6500 7800 7400  t.u.r.e._.e.x.t.
-000026d0: 7200 6100 6300 7400 6f00 7200 736d 6f64  r.a.c.t.o.r.smod
-000026e0: 4462 6c6f 6200 0000 08c5 75b6 0b20 c9c5  Dblob.....u.. ..
-000026f0: 4100 0000 1200 6600 6500 6100 7400 7500  A.....f.e.a.t.u.
-00002700: 7200 6500 5f00 6500 7800 7400 7200 6100  r.e._.e.x.t.r.a.
-00002710: 6300 7400 6f00 7200 7370 6831 5363 6f6d  c.t.o.r.sph1Scom
-00002720: 7000 0000 0000 0e70 0000 0000 1200 6600  p......p......f.
-00002730: 6500 6100 7400 7500 7200 6500 5f00 6500  e.a.t.u.r.e._.e.
-00002740: 7800 7400 7200 6100 6300 7400 6f00 7200  x.t.r.a.c.t.o.r.
-00002750: 7376 5372 6e6c 6f6e 6700 0000 0100 0000  svSrnlong.......
-00002760: 0900 6c00 6100 6200 6500 6c00 6c00 6900  ..l.a.b.e.l.l.i.
-00002770: 6e00 676c 6731 5363 6f6d 7000 0000 0000  n.glg1Scomp.....
-00002780: 0272 f000 0000 0900 6c00 6100 6200 6500  .r......l.a.b.e.
-00002790: 6c00 6c00 6900 6e00 676d 6f44 4462 6c6f  l.l.i.n.gmoDDblo
-000027a0: 6200 0000 0822 8d49 30cc c2c5 4100 0000  b....".I0...A...
-000027b0: 0900 6c00 6100 6200 6500 6c00 6c00 6900  ..l.a.b.e.l.l.i.
-000027c0: 6e00 676d 6f64 4462 6c6f 6200 0000 0822  n.gmodDblob...."
-000027d0: 8d49 30cc c2c5 4100 0000 0900 6c00 6100  .I0...A.....l.a.
-000027e0: 6200 6500 6c00 6c00 6900 6e00 6770 6831  b.e.l.l.i.n.gph1
-000027f0: 5363 6f6d 7000 0000 0000 02d0 0000 0000  Scomp...........
-00002800: 0600 6d00 6900 7800 6900 6e00 7362 7773  ..m.i.x.i.n.sbws
-00002810: 7062 6c6f 6200 0000 b862 706c 6973 7430  pblob....bplist0
-00002820: 30d6 0102 0304 0506 0708 0708 0b08 5d53  0.............]S
-00002830: 686f 7753 7461 7475 7342 6172 5b53 686f  howStatusBar[Sho
-00002840: 7754 6f6f 6c62 6172 5b53 686f 7754 6162  wToolbar[ShowTab
-00002850: 5669 6577 5f10 1443 6f6e 7461 696e 6572  View_..Container
-00002860: 5368 6f77 5369 6465 6261 725c 5769 6e64  ShowSidebar\Wind
-00002870: 6f77 426f 756e 6473 5b53 686f 7753 6964  owBounds[ShowSid
-00002880: 6562 6172 0809 0809 5f10 187b 7b32 3839  ebar...._..{{289
-00002890: 2c20 3330 307d 2c20 7b39 3230 2c20 3433  , 300}, {920, 43
-000028a0: 367d 7d09 0815 232f 3b52 5f6b 6c6d 6e6f  6}}...#/;R_klmno
-000028b0: 8a00 0000 0000 0001 0100 0000 0000 0000  ................
-000028c0: 0d00 0000 0000 0000 0000 0000 0000 0000  ................
-000028d0: 8b00 0000 0600 6d00 6900 7800 6900 6e00  ......m.i.x.i.n.
-000028e0: 736c 6731 5363 6f6d 7000 0000 0001 cec5  slg1Scomp.......
-000028f0: 5900 0000 0600 6d00 6900 7800 6900 6e00  Y.....m.i.x.i.n.
-00002900: 736c 7376 4362 6c6f 6200 0003 0a62 706c  slsvCblob....bpl
-00002910: 6973 7430 30d8 0102 0304 0506 0708 090a  ist00...........
-00002920: 0b1b 5556 0a58 5869 636f 6e53 697a 655f  ..UV.XXiconSize_
-00002930: 100f 7368 6f77 4963 6f6e 5072 6576 6965  ..showIconPrevie
-00002940: 7757 636f 6c75 6d6e 735f 1011 6361 6c63  wWcolumns_..calc
-00002950: 756c 6174 6541 6c6c 5369 7a65 7358 7465  ulateAllSizesXte
-00002960: 7874 5369 7a65 5a73 6f72 7443 6f6c 756d  xtSizeZsortColum
-00002970: 6e5f 1010 7573 6552 656c 6174 6976 6544  n_..useRelativeD
-00002980: 6174 6573 5f10 1276 6965 774f 7074 696f  ates_..viewOptio
-00002990: 6e73 5665 7273 696f 6e23 4030 0000 0000  nsVersion#@0....
-000029a0: 0000 09ae 0c15 1d22 262b 3035 3a3e 4347  ......."&+05:>CG
-000029b0: 4c50 d40d 0e0f 100a 120a 1457 7669 7369  LP.........Wvisi
-000029c0: 626c 6555 7769 6474 6859 6173 6365 6e64  bleUwidthYascend
-000029d0: 696e 675a 6964 656e 7469 6669 6572 0911  ingZidentifier..
-000029e0: 012c 0954 6e61 6d65 d410 1617 1819 1a1b  .,.Tname........
-000029f0: 1b55 7769 6474 6859 6173 6365 6e64 696e  .UwidthYascendin
-00002a00: 6757 7669 7369 626c 6558 7562 6971 7569  gWvisibleXubiqui
-00002a10: 7479 1023 0808 d40d 0e0f 100a 1f1b 2109  ty.#..........!.
-00002a20: 10b5 085c 6461 7465 4d6f 6469 6669 6564  ...\dateModified
-00002a30: d40d 0e0f 101b 1f1b 2508 085b 6461 7465  ........%..[date
-00002a40: 4372 6561 7465 64d4 0d0e 0f10 0a28 1b2a  Created......(.*
-00002a50: 0910 6108 5473 697a 65d4 0d0e 0f10 0a2d  ..a.Tsize......-
-00002a60: 0a2f 0910 7309 546b 696e 64d4 0d0e 0f10  ./..s.Tkind.....
-00002a70: 1b32 0a34 0810 6409 556c 6162 656c d40d  .2.4..d.Ulabel..
-00002a80: 0e0f 101b 370a 3908 104b 0957 7665 7273  ....7.9..K.Wvers
-00002a90: 696f 6ed4 0d0e 0f10 1b12 0a3d 0809 5863  ion........=..Xc
-00002aa0: 6f6d 6d65 6e74 73d4 0d0e 0f10 1b40 1b42  omments......@.B
-00002ab0: 0810 c808 5e64 6174 654c 6173 744f 7065  ....^dateLastOpe
-00002ac0: 6e65 64d4 1016 1718 441f 1b1b 5964 6174  ned.....D...Ydat
-00002ad0: 6541 6464 6564 0808 d418 1617 101b 491b  eAdded........I.
-00002ae0: 4b08 10d2 085a 7368 6172 654f 776e 6572  K....ZshareOwner
-00002af0: d418 1617 101b 491b 4f08 085f 100f 7368  ......I.O.._..sh
-00002b00: 6172 654c 6173 7445 6469 746f 72d4 1816  areLastEditor...
-00002b10: 1710 1b49 1b53 0808 5f10 1069 6e76 6974  ...I.S.._..invit
-00002b20: 6174 696f 6e53 7461 7475 7308 2340 2800  ationStatus.#@(.
-00002b30: 0000 0000 005c 6461 7465 4d6f 6469 6669  .....\dateModifi
-00002b40: 6564 0910 0100 0800 1900 2200 3400 3c00  ed........".4.<.
-00002b50: 5000 5900 6400 7700 8c00 9500 9600 a500  P.Y.d.w.........
-00002b60: ae00 b600 bc00 c600 d100 d200 d500 d600  ................
-00002b70: db00 e400 ea00 f400 fc01 0501 0701 0801  ................
-00002b80: 0901 1201 1301 1501 1601 2301 2c01 2d01  ..........#.,.-.
-00002b90: 2e01 3a01 4301 4401 4601 4701 4c01 5501  ..:.C.D.F.G.L.U.
-00002ba0: 5601 5801 5901 5e01 6701 6801 6a01 6b01  V.X.Y.^.g.h.j.k.
-00002bb0: 7101 7a01 7b01 7d01 7e01 8601 8f01 9001  q.z.{.}.~.......
-00002bc0: 9101 9a01 a301 a401 a601 a701 b601 bf01  ................
-00002bd0: c901 ca01 cb01 d401 d501 d701 d801 e301  ................
-00002be0: ec01 ed01 ee02 0002 0902 0a02 0b02 1e02  ................
-00002bf0: 1f02 2802 3502 3600 0000 0000 0002 0100  ..(.5.6.........
-00002c00: 0000 0000 0000 5900 0000 0000 0000 0000  ......Y.........
-00002c10: 0000 0000 0002 3800 0000 0600 6d00 6900  ......8.....m.i.
-00002c20: 7800 6900 6e00 736c 7376 7062 6c6f 6200  x.i.n.slsvpblob.
-00002c30: 0002 6162 706c 6973 7430 30d8 0102 0304  ..abplist00.....
-00002c40: 0506 0708 090a 0b1d 4546 0a33 5869 636f  ........EF.3Xico
-00002c50: 6e53 697a 655f 100f 7368 6f77 4963 6f6e  nSize_..showIcon
-00002c60: 5072 6576 6965 7757 636f 6c75 6d6e 735f  PreviewWcolumns_
-00002c70: 1011 6361 6c63 756c 6174 6541 6c6c 5369  ..calculateAllSi
-00002c80: 7a65 7358 7465 7874 5369 7a65 5a73 6f72  zesXtextSizeZsor
-00002c90: 7443 6f6c 756d 6e5f 1010 7573 6552 656c  tColumn_..useRel
-00002ca0: 6174 6976 6544 6174 6573 5f10 1276 6965  ativeDates_..vie
-00002cb0: 774f 7074 696f 6e73 5665 7273 696f 6e23  wOptionsVersion#
-00002cc0: 4030 0000 0000 0000 09d9 0c0d 0e0f 1011  @0..............
-00002cd0: 1213 1415 1e23 282d 3236 3b3f 5863 6f6d  .....#(-26;?Xcom
-00002ce0: 6d65 6e74 7355 6c61 6265 6c57 7665 7273  mentsUlabelWvers
-00002cf0: 696f 6e5b 6461 7465 4372 6561 7465 6454  ion[dateCreatedT
-00002d00: 7369 7a65 5c64 6174 654d 6f64 6966 6965  size\dateModifie
-00002d10: 6454 6b69 6e64 546e 616d 655e 6461 7465  dTkindTname^date
-00002d20: 4c61 7374 4f70 656e 6564 d416 1718 191a  LastOpened......
-00002d30: 1b0a 1d55 696e 6465 7855 7769 6474 6859  ...UindexUwidthY
-00002d40: 6173 6365 6e64 696e 6757 7669 7369 626c  ascendingWvisibl
-00002d50: 6510 0711 012c 0908 d416 1718 191f 200a  e....,........ .
-00002d60: 1d10 0510 6409 08d4 1617 1819 2425 0a1d  ....d.......$%..
-00002d70: 1006 104b 0908 d416 1718 1929 2a1d 1d10  ...K.......)*...
-00002d80: 0210 b508 08d4 1617 1819 2e2f 1d0a 1003  .........../....
-00002d90: 1061 0809 d416 1718 1933 2a1d 0a10 0108  .a.......3*.....
-00002da0: 09d4 1617 1819 3738 0a0a 1004 1073 0909  ......78.....s..
-00002db0: d416 1718 193c 1b0a 0a10 0009 09d4 1617  .....<..........
-00002dc0: 1819 4041 1d1d 1008 10c8 0808 0823 4028  ..@A.........#@(
-00002dd0: 0000 0000 0000 5c64 6174 654d 6f64 6966  ......\dateModif
-00002de0: 6965 6409 0008 0019 0022 0034 003c 0050  ied......".4.<.P
-00002df0: 0059 0064 0077 008c 0095 0096 00a9 00b2  .Y.d.w..........
-00002e00: 00b8 00c0 00cc 00d1 00de 00e3 00e8 00f7  ................
-00002e10: 0100 0106 010c 0116 011e 0120 0123 0124  ........... .#.$
-00002e20: 0125 012e 0130 0132 0133 0134 013d 013f  .%...0.2.3.4.=.?
-00002e30: 0141 0142 0143 014c 014e 0150 0151 0152  .A.B.C.L.N.P.Q.R
-00002e40: 015b 015d 015f 0160 0161 016a 016c 016d  .[.]._.`.a.j.l.m
-00002e50: 016e 0177 0179 017b 017c 017d 0186 0188  .n.w.y.{.|.}....
-00002e60: 0189 018a 0193 0195 0197 0198 0199 019a  ................
-00002e70: 01a3 01b0 0000 0000 0000 0201 0000 0000  ................
-00002e80: 0000 0048 0000 0000 0000 0000 0000 0000  ...H............
-00002e90: 0000 01b1 0000 0006 006d 0069 0078 0069  .........m.i.x.i
-00002ea0: 006e 0073 6d6f 4444 626c 6f62 0000 0008  .n.smoDDblob....
-00002eb0: 21bf 0c4d edf9 c541 0000 0006 006d 0069  !..M...A.....m.i
-00002ec0: 0078 0069 006e 0073 6d6f 6444 626c 6f62  .x.i.n.smodDblob
-00002ed0: 0000 0008 f8f6 8e79 99f6 c541 0000 0006  .......y...A....
-00002ee0: 006d 0069 0078 0069 006e 0073 7068 3153  .m.i.x.i.n.sph1S
-00002ef0: 636f 6d70 0000 0000 01e1 e000 0000 0006  comp............
-00002f00: 006d 0069 0078 0069 006e 0073 7653 726e  .m.i.x.i.n.svSrn
-00002f10: 6c6f 6e67 0000 0001 0000 0005 006d 006f  long.........m.o
-00002f20: 0064 0065 006c 6c67 3153 636f 6d70 0000  .d.e.llg1Scomp..
-00002f30: 0000 0002 17c2 0000 0005 006d 006f 0064  ...........m.o.d
-00002f40: 0065 006c 6d6f 4444 626c 6f62 0000 0008  .e.lmoDDblob....
-00002f50: 998d 3af2 23f6 c541 0000 0005 006d 006f  ..:.#..A.....m.o
-00002f60: 0064 0065 006c 6d6f 6444 626c 6f62 0000  .d.e.lmodDblob..
-00002f70: 0008 998d 3af2 23f6 c541 0072 0073 7653  ....:.#..A.r.svS
+00002140: 6261 7208 0908 095f 1017 7b7b 302c 2031  bar...._..{{0, 1
+00002150: 3236 7d2c 207b 3134 3430 2c20 3633 357d  26}, {1440, 635}
+00002160: 7d09 0815 232f 3b52 5f6b 6c6d 6e6f 8900  }...#/;R_klmno..
+00002170: 0000 0000 0001 0100 0000 0000 0000 0d00  ................
+00002180: 0000 0000 0000 0000 0000 0000 0000 8a00  ................
+00002190: 0000 0600 6100 7300 7300 6500 7400 736c  ....a.s.s.e.t.sl
+000021a0: 6731 5363 6f6d 7000 0000 0000 8a16 9400  g1Scomp.........
+000021b0: 0000 0600 6100 7300 7300 6500 7400 736d  ....a.s.s.e.t.sm
+000021c0: 6f44 4462 6c6f 6200 0000 08ee 1690 c8ab  oDDblob.........
+000021d0: bac5 4100 0000 0600 6100 7300 7300 6500  ..A.....a.s.s.e.
+000021e0: 7400 736d 6f64 4462 6c6f 6200 0000 08ee  t.smodDblob.....
+000021f0: 1690 c8ab bac5 4100 0000 0600 6100 7300  ......A.....a.s.
+00002200: 7300 6500 7400 7370 6831 5363 6f6d 7000  s.e.t.sph1Scomp.
+00002210: 0000 0000 8df0 0000 0000 0600 6100 7300  ............a.s.
+00002220: 7300 6500 7400 7376 5372 6e6c 6f6e 6700  s.e.t.svSrnlong.
+00002230: 0000 0100 0000 1200 6200 6f00 7500 6e00  ........b.o.u.n.
+00002240: 6400 6900 6e00 6700 5f00 6200 6f00 7800  d.i.n.g._.b.o.x.
+00002250: 5f00 7400 6f00 6f00 6c00 736c 6731 5363  _.t.o.o.l.slg1Sc
+00002260: 6f6d 7000 0000 0000 0322 2b00 0000 1200  omp......"+.....
+00002270: 6200 6f00 7500 6e00 6400 6900 6e00 6700  b.o.u.n.d.i.n.g.
+00002280: 5f00 6200 6f00 7800 5f00 7400 6f00 6f00  _.b.o.x._.t.o.o.
+00002290: 6c00 736d 6f44 4462 6c6f 6200 0000 08ac  l.smoDDblob.....
+000022a0: 91fa d12e bac5 4100 0000 1200 6200 6f00  ......A.....b.o.
+000022b0: 7500 6e00 6400 6900 6e00 6700 5f00 6200  u.n.d.i.n.g._.b.
+000022c0: 6f00 7800 5f00 7400 6f00 6f00 6c00 736d  o.x._.t.o.o.l.sm
+000022d0: 6f64 4462 6c6f 6200 0000 08ac 91fa d12e  odDblob.........
+000022e0: bac5 4100 0000 1200 6200 6f00 7500 6e00  ..A.....b.o.u.n.
+000022f0: 6400 6900 6e00 6700 5f00 6200 6f00 7800  d.i.n.g._.b.o.x.
+00002300: 5f00 7400 6f00 6f00 6c00 7370 6831 5363  _.t.o.o.l.sph1Sc
+00002310: 6f6d 7000 0000 0000 03d0 0000 0000 0f00  omp.............
+00002320: 6300 7500 6500 5f00 6c00 6900 6700 6800  c.u.e._.l.i.g.h.
+00002330: 7400 5f00 7400 6f00 6f00 6c00 736c 6731  t._.t.o.o.l.slg1
+00002340: 5363 6f6d 7000 0000 0000 02b2 7800 0000  Scomp.......x...
+00002350: 0f00 6300 7500 6500 5f00 6c00 6900 6700  ..c.u.e._.l.i.g.
+00002360: 6800 7400 5f00 7400 6f00 6f00 6c00 736d  h.t._.t.o.o.l.sm
+00002370: 6f44 4462 6c6f 6200 0000 08e8 2ad1 274b  oDDblob.....*.'K
+00002380: edc5 4100 0000 0f00 6300 7500 6500 5f00  ..A.....c.u.e._.
+00002390: 6c00 6900 6700 6800 7400 5f00 7400 6f00  l.i.g.h.t._.t.o.
+000023a0: 6f00 6c00 736d 6f64 4462 6c6f 6200 0000  o.l.smodDblob...
+000023b0: 08e8 2ad1 274b edc5 4100 0000 0f00 6300  ..*.'K..A.....c.
+000023c0: 7500 6500 5f00 6c00 6900 6700 6800 7400  u.e._.l.i.g.h.t.
+000023d0: 5f00 7400 6f00 6f00 6c00 7370 6831 5363  _.t.o.o.l.sph1Sc
+000023e0: 6f6d 7000 0000 0000 0380 0000 0000 0800  omp.............
+000023f0: 6400 6100 7300 6800 5f00 6100 7000 706c  d.a.s.h._.a.p.pl
+00002400: 6731 5363 6f6d 7000 0000 0000 01e9 2a00  g1Scomp.......*.
+00002410: 0000 0800 6400 6100 7300 6800 5f00 6100  ....d.a.s.h._.a.
+00002420: 7000 706d 6f44 4462 6c6f 6200 0000 08de  p.pmoDDblob.....
+00002430: 5fc4 870a bac5 4100 0000 0800 6400 6100  _.....A.....d.a.
+00002440: 7300 6800 5f00 6100 7000 706d 6f64 4462  s.h._.a.p.pmodDb
+00002450: 6c6f 6200 0000 08de 5fc4 870a bac5 4100  lob....._.....A.
+00002460: 0000 0800 6400 6100 7300 6800 5f00 6100  ....d.a.s.h._.a.
+00002470: 7000 7070 6831 5363 6f6d 7000 0000 0000  p.pph1Scomp.....
+00002480: 0200 0000 0000 0f00 6400 6100 7400 6100  ........d.a.t.a.
+00002490: 5f00 7000 7200 6f00 6300 6500 7300 7300  _.p.r.o.c.e.s.s.
+000024a0: 6f00 7200 736c 6731 5363 6f6d 7000 0000  o.r.slg1Scomp...
+000024b0: 0000 0731 2600 0000 0f00 6400 6100 7400  ...1&.....d.a.t.
+000024c0: 6100 5f00 7000 7200 6f00 6300 6500 7300  a._.p.r.o.c.e.s.
+000024d0: 7300 6f00 7200 736d 6f44 4462 6c6f 6200  s.o.r.smoDDblob.
+000024e0: 0000 0816 d078 2913 eec5 4100 0000 0f00  .....x)...A.....
+000024f0: 6400 6100 7400 6100 5f00 7000 7200 6f00  d.a.t.a._.p.r.o.
+00002500: 6300 6500 7300 7300 6f00 7200 736d 6f64  c.e.s.s.o.r.smod
+00002510: 4462 6c6f 6200 0000 0816 d078 2913 eec5  Dblob......x)...
+00002520: 4100 0000 0f00 6400 6100 7400 6100 5f00  A.....d.a.t.a._.
+00002530: 7000 7200 6f00 6300 6500 7300 7300 6f00  p.r.o.c.e.s.s.o.
+00002540: 7200 7370 6831 5363 6f6d 7000 0000 0000  r.sph1Scomp.....
+00002550: 0910 0000 0000 1200 6600 6500 6100 7400  ........f.e.a.t.
+00002560: 7500 7200 6500 5f00 6500 7800 7400 7200  u.r.e._.e.x.t.r.
+00002570: 6100 6300 7400 6f00 7200 7362 7773 7062  a.c.t.o.r.sbwspb
+00002580: 6c6f 6200 0000 b962 706c 6973 7430 30d6  lob....bplist00.
+00002590: 0102 0304 0506 0708 0708 0b08 5d53 686f  ............]Sho
+000025a0: 7753 7461 7475 7342 6172 5b53 686f 7754  wStatusBar[ShowT
+000025b0: 6f6f 6c62 6172 5b53 686f 7754 6162 5669  oolbar[ShowTabVi
+000025c0: 6577 5f10 1443 6f6e 7461 696e 6572 5368  ew_..ContainerSh
+000025d0: 6f77 5369 6465 6261 725c 5769 6e64 6f77  owSidebar\Window
+000025e0: 426f 756e 6473 5b53 686f 7753 6964 6562  Bounds[ShowSideb
+000025f0: 6172 0809 0809 5f10 197b 7b39 392c 202d  ar...._..{{99, -
+00002600: 3136 367d 2c20 7b31 3238 332c 2036 3839  166}, {1283, 689
+00002610: 7d7d 0908 1523 2f3b 525f 6b6c 6d6e 6f8b  }}...#/;R_klmno.
+00002620: 0000 0000 0000 0101 0000 0000 0000 000d  ................
+00002630: 0000 0000 0000 0000 0000 0000 0000 008c  ................
+00002640: 0000 0012 0066 0065 0061 0074 0075 0072  .....f.e.a.t.u.r
+00002650: 0065 005f 0065 0078 0074 0072 0061 0063  .e._.e.x.t.r.a.c
+00002660: 0074 006f 0072 0073 6c67 3153 636f 6d70  .t.o.r.slg1Scomp
+00002670: 0000 0000 000c 9d20 0000 0012 0066 0065  ....... .....f.e
+00002680: 0061 0074 0075 0072 0065 005f 0065 0078  .a.t.u.r.e._.e.x
+00002690: 0074 0072 0061 0063 0074 006f 0072 0073  .t.r.a.c.t.o.r.s
+000026a0: 6d6f 4444 626c 6f62 0000 0008 c575 b60b  moDDblob.....u..
+000026b0: 20c9 c541 0000 0012 0066 0065 0061 0074   ..A.....f.e.a.t
+000026c0: 0075 0072 0065 005f 0065 0078 0074 0072  .u.r.e._.e.x.t.r
+000026d0: 0061 0063 0074 006f 0072 0073 6d6f 6444  .a.c.t.o.r.smodD
+000026e0: 626c 6f62 0000 0008 c575 b60b 20c9 c541  blob.....u.. ..A
+000026f0: 0000 0012 0066 0065 0061 0074 0075 0072  .....f.e.a.t.u.r
+00002700: 0065 005f 0065 0078 0074 0072 0061 0063  .e._.e.x.t.r.a.c
+00002710: 0074 006f 0072 0073 7068 3153 636f 6d70  .t.o.r.sph1Scomp
+00002720: 0000 0000 000e 7000 0000 0012 0066 0065  ......p......f.e
+00002730: 0061 0074 0075 0072 0065 005f 0065 0078  .a.t.u.r.e._.e.x
+00002740: 0074 0072 0061 0063 0074 006f 0072 0073  .t.r.a.c.t.o.r.s
+00002750: 7653 726e 6c6f 6e67 0000 0001 0000 0009  vSrnlong........
+00002760: 006c 0061 0062 0065 006c 006c 0069 006e  .l.a.b.e.l.l.i.n
+00002770: 0067 6c67 3153 636f 6d70 0000 0000 0002  .glg1Scomp......
+00002780: 72f0 0000 0009 006c 0061 0062 0065 006c  r......l.a.b.e.l
+00002790: 006c 0069 006e 0067 6d6f 4444 626c 6f62  .l.i.n.gmoDDblob
+000027a0: 0000 0008 228d 4930 ccc2 c541 0000 0009  ....".I0...A....
+000027b0: 006c 0061 0062 0065 006c 006c 0069 006e  .l.a.b.e.l.l.i.n
+000027c0: 0067 6d6f 6444 626c 6f62 0000 0008 228d  .gmodDblob....".
+000027d0: 4930 ccc2 c541 0000 0009 006c 0061 0062  I0...A.....l.a.b
+000027e0: 0065 006c 006c 0069 006e 0067 7068 3153  .e.l.l.i.n.gph1S
+000027f0: 636f 6d70 0000 0000 0002 d000 0000 0006  comp............
+00002800: 006d 0069 0078 0069 006e 0073 6277 7370  .m.i.x.i.n.sbwsp
+00002810: 626c 6f62 0000 00b8 6270 6c69 7374 3030  blob....bplist00
+00002820: d601 0203 0405 0607 0807 080b 085d 5368  .............]Sh
+00002830: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
+00002840: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
+00002850: 6965 775f 1014 436f 6e74 6169 6e65 7253  iew_..ContainerS
+00002860: 686f 7753 6964 6562 6172 5c57 696e 646f  howSidebar\Windo
+00002870: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
+00002880: 6261 7208 0908 095f 1018 7b7b 3238 392c  bar...._..{{289,
+00002890: 2033 3030 7d2c 207b 3932 302c 2034 3336   300}, {920, 436
+000028a0: 7d7d 0908 1523 2f3b 525f 6b6c 6d6e 6f8a  }}...#/;R_klmno.
+000028b0: 0000 0000 0000 0101 0000 0000 0000 000d  ................
+000028c0: 0000 0000 0000 0000 0000 0000 0000 008b  ................
+000028d0: 0000 0006 006d 0069 0078 0069 006e 0073  .....m.i.x.i.n.s
+000028e0: 6c67 3153 636f 6d70 0000 0000 01ce c559  lg1Scomp.......Y
+000028f0: 0000 0006 006d 0069 0078 0069 006e 0073  .....m.i.x.i.n.s
+00002900: 6c73 7643 626c 6f62 0000 030a 6270 6c69  lsvCblob....bpli
+00002910: 7374 3030 d801 0203 0405 0607 0809 0a0b  st00............
+00002920: 1b55 560a 5858 6963 6f6e 5369 7a65 5f10  .UV.XXiconSize_.
+00002930: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
+00002940: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
+00002950: 6c61 7465 416c 6c53 697a 6573 5874 6578  lateAllSizesXtex
+00002960: 7453 697a 655a 736f 7274 436f 6c75 6d6e  tSizeZsortColumn
+00002970: 5f10 1075 7365 5265 6c61 7469 7665 4461  _..useRelativeDa
+00002980: 7465 735f 1012 7669 6577 4f70 7469 6f6e  tes_..viewOption
+00002990: 7356 6572 7369 6f6e 2340 3000 0000 0000  sVersion#@0.....
+000029a0: 0009 ae0c 151d 2226 2b30 353a 3e43 474c  ......"&+05:>CGL
+000029b0: 50d4 0d0e 0f10 0a12 0a14 5776 6973 6962  P.........Wvisib
+000029c0: 6c65 5577 6964 7468 5961 7363 656e 6469  leUwidthYascendi
+000029d0: 6e67 5a69 6465 6e74 6966 6965 7209 1101  ngZidentifier...
+000029e0: 2c09 546e 616d 65d4 1016 1718 191a 1b1b  ,.Tname.........
+000029f0: 5577 6964 7468 5961 7363 656e 6469 6e67  UwidthYascending
+00002a00: 5776 6973 6962 6c65 5875 6269 7175 6974  WvisibleXubiquit
+00002a10: 7910 2308 08d4 0d0e 0f10 0a1f 1b21 0910  y.#..........!..
+00002a20: b508 5c64 6174 654d 6f64 6966 6965 64d4  ..\dateModified.
+00002a30: 0d0e 0f10 1b1f 1b25 0808 5b64 6174 6543  .......%..[dateC
+00002a40: 7265 6174 6564 d40d 0e0f 100a 281b 2a09  reated......(.*.
+00002a50: 1061 0854 7369 7a65 d40d 0e0f 100a 2d0a  .a.Tsize......-.
+00002a60: 2f09 1073 0954 6b69 6e64 d40d 0e0f 101b  /..s.Tkind......
+00002a70: 320a 3408 1064 0955 6c61 6265 6cd4 0d0e  2.4..d.Ulabel...
+00002a80: 0f10 1b37 0a39 0810 4b09 5776 6572 7369  ...7.9..K.Wversi
+00002a90: 6f6e d40d 0e0f 101b 120a 3d08 0958 636f  on........=..Xco
+00002aa0: 6d6d 656e 7473 d40d 0e0f 101b 401b 4208  mments......@.B.
+00002ab0: 10c8 085e 6461 7465 4c61 7374 4f70 656e  ...^dateLastOpen
+00002ac0: 6564 d410 1617 1844 1f1b 1b59 6461 7465  ed.....D...Ydate
+00002ad0: 4164 6465 6408 08d4 1816 1710 1b49 1b4b  Added........I.K
+00002ae0: 0810 d208 5a73 6861 7265 4f77 6e65 72d4  ....ZshareOwner.
+00002af0: 1816 1710 1b49 1b4f 0808 5f10 0f73 6861  .....I.O.._..sha
+00002b00: 7265 4c61 7374 4564 6974 6f72 d418 1617  reLastEditor....
+00002b10: 101b 491b 5308 085f 1010 696e 7669 7461  ..I.S.._..invita
+00002b20: 7469 6f6e 5374 6174 7573 0823 4028 0000  tionStatus.#@(..
+00002b30: 0000 0000 5c64 6174 654d 6f64 6966 6965  ....\dateModifie
+00002b40: 6409 1001 0008 0019 0022 0034 003c 0050  d........".4.<.P
+00002b50: 0059 0064 0077 008c 0095 0096 00a5 00ae  .Y.d.w..........
+00002b60: 00b6 00bc 00c6 00d1 00d2 00d5 00d6 00db  ................
+00002b70: 00e4 00ea 00f4 00fc 0105 0107 0108 0109  ................
+00002b80: 0112 0113 0115 0116 0123 012c 012d 012e  .........#.,.-..
+00002b90: 013a 0143 0144 0146 0147 014c 0155 0156  .:.C.D.F.G.L.U.V
+00002ba0: 0158 0159 015e 0167 0168 016a 016b 0171  .X.Y.^.g.h.j.k.q
+00002bb0: 017a 017b 017d 017e 0186 018f 0190 0191  .z.{.}.~........
+00002bc0: 019a 01a3 01a4 01a6 01a7 01b6 01bf 01c9  ................
+00002bd0: 01ca 01cb 01d4 01d5 01d7 01d8 01e3 01ec  ................
+00002be0: 01ed 01ee 0200 0209 020a 020b 021e 021f  ................
+00002bf0: 0228 0235 0236 0000 0000 0000 0201 0000  .(.5.6..........
+00002c00: 0000 0000 0059 0000 0000 0000 0000 0000  .....Y..........
+00002c10: 0000 0000 0238 0000 0006 006d 0069 0078  .....8.....m.i.x
+00002c20: 0069 006e 0073 6c73 7670 626c 6f62 0000  .i.n.slsvpblob..
+00002c30: 0261 6270 6c69 7374 3030 d801 0203 0405  .abplist00......
+00002c40: 0607 0809 0a0b 1d45 460a 3358 6963 6f6e  .......EF.3Xicon
+00002c50: 5369 7a65 5f10 0f73 686f 7749 636f 6e50  Size_..showIconP
+00002c60: 7265 7669 6577 5763 6f6c 756d 6e73 5f10  reviewWcolumns_.
+00002c70: 1163 616c 6375 6c61 7465 416c 6c53 697a  .calculateAllSiz
+00002c80: 6573 5874 6578 7453 697a 655a 736f 7274  esXtextSizeZsort
+00002c90: 436f 6c75 6d6e 5f10 1075 7365 5265 6c61  Column_..useRela
+00002ca0: 7469 7665 4461 7465 735f 1012 7669 6577  tiveDates_..view
+00002cb0: 4f70 7469 6f6e 7356 6572 7369 6f6e 2340  OptionsVersion#@
+00002cc0: 3000 0000 0000 0009 d90c 0d0e 0f10 1112  0...............
+00002cd0: 1314 151e 2328 2d32 363b 3f58 636f 6d6d  ....#(-26;?Xcomm
+00002ce0: 656e 7473 556c 6162 656c 5776 6572 7369  entsUlabelWversi
+00002cf0: 6f6e 5b64 6174 6543 7265 6174 6564 5473  on[dateCreatedTs
+00002d00: 697a 655c 6461 7465 4d6f 6469 6669 6564  ize\dateModified
+00002d10: 546b 696e 6454 6e61 6d65 5e64 6174 654c  TkindTname^dateL
+00002d20: 6173 744f 7065 6e65 64d4 1617 1819 1a1b  astOpened.......
+00002d30: 0a1d 5569 6e64 6578 5577 6964 7468 5961  ..UindexUwidthYa
+00002d40: 7363 656e 6469 6e67 5776 6973 6962 6c65  scendingWvisible
+00002d50: 1007 1101 2c09 08d4 1617 1819 1f20 0a1d  ....,........ ..
+00002d60: 1005 1064 0908 d416 1718 1924 250a 1d10  ...d.......$%...
+00002d70: 0610 4b09 08d4 1617 1819 292a 1d1d 1002  ..K.......)*....
+00002d80: 10b5 0808 d416 1718 192e 2f1d 0a10 0310  ........../.....
+00002d90: 6108 09d4 1617 1819 332a 1d0a 1001 0809  a.......3*......
+00002da0: d416 1718 1937 380a 0a10 0410 7309 09d4  .....78.....s...
+00002db0: 1617 1819 3c1b 0a0a 1000 0909 d416 1718  ....<...........
+00002dc0: 1940 411d 1d10 0810 c808 0808 2340 2800  .@A.........#@(.
+00002dd0: 0000 0000 005c 6461 7465 4d6f 6469 6669  .....\dateModifi
+00002de0: 6564 0900 0800 1900 2200 3400 3c00 5000  ed......".4.<.P.
+00002df0: 5900 6400 7700 8c00 9500 9600 a900 b200  Y.d.w...........
+00002e00: b800 c000 cc00 d100 de00 e300 e800 f701  ................
+00002e10: 0001 0601 0c01 1601 1e01 2001 2301 2401  .......... .#.$.
+00002e20: 2501 2e01 3001 3201 3301 3401 3d01 3f01  %...0.2.3.4.=.?.
+00002e30: 4101 4201 4301 4c01 4e01 5001 5101 5201  A.B.C.L.N.P.Q.R.
+00002e40: 5b01 5d01 5f01 6001 6101 6a01 6c01 6d01  [.]._.`.a.j.l.m.
+00002e50: 6e01 7701 7901 7b01 7c01 7d01 8601 8801  n.w.y.{.|.}.....
+00002e60: 8901 8a01 9301 9501 9701 9801 9901 9a01  ................
+00002e70: a301 b000 0000 0000 0002 0100 0000 0000  ................
+00002e80: 0000 4800 0000 0000 0000 0000 0000 0000  ..H.............
+00002e90: 0001 b100 0000 0600 6d00 6900 7800 6900  ........m.i.x.i.
+00002ea0: 6e00 736d 6f44 4462 6c6f 6200 0000 0821  n.smoDDblob....!
+00002eb0: bf0c 4ded f9c5 4100 0000 0600 6d00 6900  ..M...A.....m.i.
+00002ec0: 7800 6900 6e00 736d 6f64 4462 6c6f 6200  x.i.n.smodDblob.
+00002ed0: 0000 08f8 f68e 7999 f6c5 4100 0000 0600  ......y...A.....
+00002ee0: 6d00 6900 7800 6900 6e00 7370 6831 5363  m.i.x.i.n.sph1Sc
+00002ef0: 6f6d 7000 0000 0001 e1e0 0000 0000 0600  omp.............
+00002f00: 6d00 6900 7800 6900 6e00 7376 5372 6e6c  m.i.x.i.n.svSrnl
+00002f10: 6f6e 6700 0000 0100 0000 0500 6d00 6f00  ong.........m.o.
+00002f20: 6400 6500 6c6c 6731 5363 6f6d 7000 0000  d.e.llg1Scomp...
+00002f30: 0000 0217 c200 0000 0500 6d00 6f00 6400  ..........m.o.d.
+00002f40: 6500 6c6d 6f44 4462 6c6f 6200 0000 0899  e.lmoDDblob.....
+00002f50: 8d3a f223 f6c5 4100 0000 0500 6d00 6f00  .:.#..A.....m.o.
+00002f60: 6400 6500 6c6d 6f64 4462 6c6f 6200 0000  d.e.lmodDblob...
+00002f70: 0899 8d3a f223 f6c5 416f 0072 0073 7653  ...:.#..Ao.r.svS
 00002f80: 726e 6c6f 6e67 0000 0001 0000 0000 0000  rnlong..........
 00002f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `Simba-UW-tf-dev-1.92.4/simba/feature_extractors/feature_extractor_14bp.py` & `Simba-UW-tf-dev-1.92.5/simba/feature_extractors/feature_extractor_14bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/feature_extractors/feature_extractor_7bp.py` & `Simba-UW-tf-dev-1.92.5/simba/feature_extractors/feature_extractor_7bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/feature_extractors/misc/doctests.py` & `Simba-UW-tf-dev-1.92.5/simba/feature_extractors/misc/doctests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py` & `Simba-UW-tf-dev-1.92.5/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/feature_extractors/misc/read_in_mp.py` & `Simba-UW-tf-dev-1.92.5/simba/feature_extractors/misc/read_in_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/feature_extractors/misc/peaks.py` & `Simba-UW-tf-dev-1.92.5/simba/feature_extractors/misc/peaks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/feature_extractors/misc/fish_feature_extractor_2022.py` & `Simba-UW-tf-dev-1.92.5/simba/feature_extractors/misc/fish_feature_extractor_2022.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/feature_extractors/misc/convex_hull_3_scratch_3.py` & `Simba-UW-tf-dev-1.92.5/simba/feature_extractors/misc/convex_hull_3_scratch_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/feature_extractors/misc/convex_hull_scratch_1.py` & `Simba-UW-tf-dev-1.92.5/simba/feature_extractors/misc/convex_hull_scratch_1.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py` & `Simba-UW-tf-dev-1.92.5/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/feature_extractors/misc/egocentrical_aligner.py` & `Simba-UW-tf-dev-1.92.5/simba/feature_extractors/misc/egocentrical_aligner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/feature_extractors/misc/count_values_in_range.py` & `Simba-UW-tf-dev-1.92.5/simba/feature_extractors/misc/count_values_in_range.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/feature_extractors/misc/graph_creator.py` & `Simba-UW-tf-dev-1.92.5/simba/feature_extractors/misc/graph_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/feature_extractors/misc/termite_rois.csv` & `Simba-UW-tf-dev-1.92.5/simba/feature_extractors/misc/termite_rois.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/feature_extractors/misc/mutual_exclusive.py` & `Simba-UW-tf-dev-1.92.5/simba/feature_extractors/misc/mutual_exclusive.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/feature_extractors/misc/video_color.py` & `Simba-UW-tf-dev-1.92.5/simba/feature_extractors/misc/video_color.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/feature_extractors/misc/graph_3d_plotter.py` & `Simba-UW-tf-dev-1.92.5/simba/feature_extractors/misc/graph_3d_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/feature_extractors/misc/video_rotator.py` & `Simba-UW-tf-dev-1.92.5/simba/feature_extractors/misc/video_rotator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/feature_extractors/misc/add_probability_cnt_features.py` & `Simba-UW-tf-dev-1.92.5/simba/feature_extractors/misc/add_probability_cnt_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/feature_extractors/misc/make_splash.py` & `Simba-UW-tf-dev-1.92.5/simba/feature_extractors/misc/make_splash.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py` & `Simba-UW-tf-dev-1.92.5/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/feature_extractors/misc/time_stamp_calculator.py` & `Simba-UW-tf-dev-1.92.5/simba/feature_extractors/misc/time_stamp_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/feature_extractors/misc/video_rotator_mp.py` & `Simba-UW-tf-dev-1.92.5/simba/feature_extractors/misc/video_rotator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py` & `Simba-UW-tf-dev-1.92.5/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/feature_extractors/misc/convex_hull_scratch_2.py` & `Simba-UW-tf-dev-1.92.5/simba/feature_extractors/misc/convex_hull_scratch_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/feature_extractors/feature_extractor_8bps_2_animals.py` & `Simba-UW-tf-dev-1.92.5/simba/feature_extractors/feature_extractor_8bps_2_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/feature_extractors/.DS_Store` & `Simba-UW-tf-dev-1.92.5/simba/feature_extractors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/feature_extractors/perimeter_jit.py` & `Simba-UW-tf-dev-1.92.5/simba/feature_extractors/perimeter_jit.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/feature_extractors/feature_subsets.py` & `Simba-UW-tf-dev-1.92.5/simba/feature_extractors/feature_subsets.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/feature_extractors/feature_extractor_user_defined.py` & `Simba-UW-tf-dev-1.92.5/simba/feature_extractors/feature_extractor_user_defined.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/feature_extractors/feature_extractor_16bp.py` & `Simba-UW-tf-dev-1.92.5/simba/feature_extractors/feature_extractor_16bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/feature_extractors/feature_extractor_9bp.py` & `Simba-UW-tf-dev-1.92.5/simba/feature_extractors/feature_extractor_9bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/feature_extractors/feature_extractor_8bp.py` & `Simba-UW-tf-dev-1.92.5/simba/feature_extractors/feature_extractor_8bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/feature_extractors/feature_extractor_4bp.py` & `Simba-UW-tf-dev-1.92.5/simba/feature_extractors/feature_extractor_4bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/feature_extractors/amber_feature_extractor.py` & `Simba-UW-tf-dev-1.92.5/simba/feature_extractors/amber_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/requirements.txt` & `Simba-UW-tf-dev-1.92.5/simba/requirements.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,31 @@
+pip==21.2.2;python_version=="3.6"
+pip==24.0;python_version>="3.9"
+setuptools==58.0.4;python_version=="3.6"
+setuptools==69.5.1;python_version>="3.9"
 Pillow
 pyyaml == 5.3.1
-shapely == 1.7.1;python_version=="3.6"
+shapely == 1.8.0;python_version=="3.6"
 shapely;python_version>="3.9"
 dtreeviz == 0.8.1
 eli5 == 0.10.1
-graphviz == 0.11
 imblearn == 0.0
 imgaug == 0.4.0
 imutils == 0.5.2
-matplotlib >= 3.0.3
+matplotlib == 3.3.4
 numpy==1.18.1;python_version=="3.6"
-numpy;python_version>="3.9"
+numpy==1.26.4;python_version>="3.9"
 opencv-python == 3.4.5.20;python_version=="3.6"
 opencv-python;python_version>="3.9"
 pandas==0.25.3;python_version=="3.6"
 pandas;python_version>="3.9"
 scikit-image
 scipy
 kaleido
-seaborn == 0.9.0
+seaborn == 0.11.0
 scikit-learn
 tabulate == 0.8.3;python_version=="3.6"
 tabulate == 0.9.0;python_version>="3.9"
 tqdm == 4.30.0
 xgboost == 0.90
 yellowbrick
 dash == 1.14.0
```

### Comparing `Simba-UW-tf-dev-1.92.4/simba/mixins/annotator_mixin.py` & `Simba-UW-tf-dev-1.92.5/simba/mixins/annotator_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/mixins/timeseries_features_mixin.py` & `Simba-UW-tf-dev-1.92.5/simba/mixins/timeseries_features_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/mixins/.DS_Store` & `Simba-UW-tf-dev-1.92.5/simba/mixins/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/mixins/pop_up_mixin.py` & `Simba-UW-tf-dev-1.92.5/simba/mixins/pop_up_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/mixins/config_reader.py` & `Simba-UW-tf-dev-1.92.5/simba/mixins/config_reader.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/mixins/circular_statistics.py` & `Simba-UW-tf-dev-1.92.5/simba/mixins/circular_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/mixins/network_mixin.py` & `Simba-UW-tf-dev-1.92.5/simba/mixins/network_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/mixins/pose_importer_mixin.py` & `Simba-UW-tf-dev-1.92.5/simba/mixins/pose_importer_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/mixins/video_processing_mixin.py` & `Simba-UW-tf-dev-1.92.5/simba/mixins/video_processing_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/mixins/feature_extraction_supplement_mixin.py` & `Simba-UW-tf-dev-1.92.5/simba/mixins/feature_extraction_supplement_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/mixins/statistics_mixin.py` & `Simba-UW-tf-dev-1.92.5/simba/mixins/statistics_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/mixins/feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.92.5/simba/mixins/feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/mixins/plotting_mixin.py` & `Simba-UW-tf-dev-1.92.5/simba/mixins/plotting_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/mixins/image_mixin.py` & `Simba-UW-tf-dev-1.92.5/simba/mixins/image_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/mixins/unsupervised_mixin.py` & `Simba-UW-tf-dev-1.92.5/simba/mixins/unsupervised_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/mixins/train_model_mixin.py` & `Simba-UW-tf-dev-1.92.5/simba/mixins/train_model_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/mixins/geometry_mixin.py` & `Simba-UW-tf-dev-1.92.5/simba/mixins/geometry_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/mixins/feature_extraction_circular_mixin.py` & `Simba-UW-tf-dev-1.92.5/simba/mixins/feature_extraction_circular_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/third_party_label_appenders/deepethogram_importer.py` & `Simba-UW-tf-dev-1.92.5/simba/third_party_label_appenders/deepethogram_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/third_party_label_appenders/BORIS_appender.py` & `Simba-UW-tf-dev-1.92.5/simba/third_party_label_appenders/BORIS_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/third_party_label_appenders/observer_importer.py` & `Simba-UW-tf-dev-1.92.5/simba/third_party_label_appenders/observer_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/third_party_label_appenders/.DS_Store` & `Simba-UW-tf-dev-1.92.5/simba/third_party_label_appenders/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/third_party_label_appenders/boris_source_cleaner.py` & `Simba-UW-tf-dev-1.92.5/simba/third_party_label_appenders/boris_source_cleaner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/third_party_label_appenders/tools.py` & `Simba-UW-tf-dev-1.92.5/simba/third_party_label_appenders/tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/third_party_label_appenders/third_party_appender.py` & `Simba-UW-tf-dev-1.92.5/simba/third_party_label_appenders/third_party_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/third_party_label_appenders/ethovision_import.py` & `Simba-UW-tf-dev-1.92.5/simba/third_party_label_appenders/ethovision_import.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/third_party_label_appenders/BENTO_appender.py` & `Simba-UW-tf-dev-1.92.5/simba/third_party_label_appenders/BENTO_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/third_party_label_appenders/solomon_importer.py` & `Simba-UW-tf-dev-1.92.5/simba/third_party_label_appenders/solomon_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/cue_light_tools/cue_light_clf_statistics.py` & `Simba-UW-tf-dev-1.92.5/simba/cue_light_tools/cue_light_clf_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/cue_light_tools/cue_light_analyzer.py` & `Simba-UW-tf-dev-1.92.5/simba/cue_light_tools/cue_light_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/cue_light_tools/cue_light_menues.py` & `Simba-UW-tf-dev-1.92.5/simba/cue_light_tools/cue_light_menues.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/cue_light_tools/cue_light_tools.py` & `Simba-UW-tf-dev-1.92.5/simba/cue_light_tools/cue_light_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/cue_light_tools/cue_light_visualizer.py` & `Simba-UW-tf-dev-1.92.5/simba/cue_light_tools/cue_light_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/cue_light_tools/cue_light_movement_statistics.py` & `Simba-UW-tf-dev-1.92.5/simba/cue_light_tools/cue_light_movement_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/utils/config_creator.py` & `Simba-UW-tf-dev-1.92.5/simba/utils/config_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/utils/enums.py` & `Simba-UW-tf-dev-1.92.5/simba/utils/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/utils/custom_feature_extractor.py` & `Simba-UW-tf-dev-1.92.5/simba/utils/custom_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/utils/.DS_Store` & `Simba-UW-tf-dev-1.92.5/simba/utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/utils/warnings.py` & `Simba-UW-tf-dev-1.92.5/simba/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/utils/checks.py` & `Simba-UW-tf-dev-1.92.5/simba/utils/checks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/utils/read_write.py` & `Simba-UW-tf-dev-1.92.5/simba/utils/read_write.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/utils/lookups.py` & `Simba-UW-tf-dev-1.92.5/simba/utils/lookups.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/utils/cli/cli_tools.py` & `Simba-UW-tf-dev-1.92.5/simba/utils/cli/cli_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/utils/errors.py` & `Simba-UW-tf-dev-1.92.5/simba/utils/errors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/utils/data.py` & `Simba-UW-tf-dev-1.92.5/simba/utils/data.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/utils/printing.py` & `Simba-UW-tf-dev-1.92.5/simba/utils/printing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/SimBA_logo.ico` & `Simba-UW-tf-dev-1.92.5/simba/SimBA_logo.ico`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/pose_processors/reorganize_keypoint.py` & `Simba-UW-tf-dev-1.92.5/simba/pose_processors/reorganize_keypoint.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/pose_processors/remove_keypoints.py` & `Simba-UW-tf-dev-1.92.5/simba/pose_processors/remove_keypoints.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/pose_processors/pose_reset.py` & `Simba-UW-tf-dev-1.92.5/simba/pose_processors/pose_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/pose_processors/reverse_pose.py` & `Simba-UW-tf-dev-1.92.5/simba/pose_processors/reverse_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/doctests.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/doctests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/fish_feature_extractor_2023_version_3.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/fish_feature_extractor_2023_version_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/CLAHE.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/CLAHE.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/dprime.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/dprime.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/ffmpeg_progress_bar.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/ffmpeg_progress_bar.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/linear_fretchet.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/linear_fretchet.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/read_in_mp.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/read_in_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/piotr_120324 3.py.zip` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/piotr_120324 3.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/dunn_index.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/dunn_index.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/hausdorff.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/hausdorff.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/peaks.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/peaks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/fish_feature_extractor_2022.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/fish_feature_extractor_2022.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/colinear_features.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/colinear_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/spontaneous_alternation_calculator.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/spontaneous_alternation_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/horizontal_videos_concat.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/horizontal_videos_concat.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/convex_hull_3_scratch_3.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/convex_hull_3_scratch_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/silhouette_score.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/silhouette_score.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/two_fish_feature_extractor_040924.py.zip` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/two_fish_feature_extractor_040924.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/cuda_jit.ipynb` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/cuda_jit.ipynb`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/convex_hull_scratch_1.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/convex_hull_scratch_1.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/directed_hausdorff.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/directed_hausdorff.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/shannon_diversity_index.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/shannon_diversity_index.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/sequential_lag_analysis.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/sequential_lag_analysis.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/wilcoxon.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/wilcoxon.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/ROI_plotter_mp.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/ROI_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/.DS_Store` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/detect_scene_changes.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/detect_scene_changes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/data.npy` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/data.npy`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/distances.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/distances.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/fish_feature_extractor_2023_version_2.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/fish_feature_extractor_2023_version_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/cohens_kappa.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/cohens_kappa.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/watermark.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/watermark.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/paths.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/paths.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/outliers_tietjen.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/outliers_tietjen.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/train_model.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/train_model.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/img_stack_to_bw.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/img_stack_to_bw.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/amber_tests.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/amber_tests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/line_locate_point.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/line_locate_point.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/sorensen_dice_coefficient.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/sorensen_dice_coefficient.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/multifrm_to_points.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/multifrm_to_points.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/clean_sleap_filename.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/clean_sleap_filename.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/two_fish_feature_extractor_040924.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/two_fish_feature_extractor_040924.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/ez_path_plot.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/ez_path_plot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/egocentrical_aligner.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/egocentrical_aligner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/downsample_video_popup.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/downsample_video_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/add_body_part.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/add_body_part.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/grubbs_test.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/grubbs_test.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/slide_circ_mean.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/slide_circ_mean.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/calinski_harabasz.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/calinski_harabasz.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/roi_feature_visualizer_example.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/roi_feature_visualizer_example.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/spontaneuous_alternation_plotter.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/spontaneuous_alternation_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/runs_test.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/runs_test.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/pct_counts_in_top_N.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/pct_counts_in_top_N.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/concordance_ratio.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/concordance_ratio.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/total_variation_distance.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/total_variation_distance.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/crop_single_polygon.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/crop_single_polygon.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/ROI_analyzer.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/ROI_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/joint_plotter.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/joint_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/segment_image_horizontal.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/segment_image_horizontal.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/clip_multiple_videos_by_frame_numbers.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/clip_multiple_videos_by_frame_numbers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/elliptic_envelope.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/elliptic_envelope.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/roi_definition_csvs_to_h5.py.zip` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/roi_definition_csvs_to_h5.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/add_body_part.py.zip` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/add_body_part.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/roi_feature_visualizer_example.py.zip` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/roi_feature_visualizer_example.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/sliding_crosscorrelation.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/sliding_crosscorrelation.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/count_values_in_range.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/count_values_in_range.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/roi_definition_csvs_to_h5.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/roi_definition_csvs_to_h5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/distance_velocity.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/distance_velocity.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/graph_creator.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/graph_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/line_plot_plotly.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/line_plot_plotly.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/crossfade.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/crossfade.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/shift_geometries.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/shift_geometries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/termite_rois.csv` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/termite_rois.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/convert_to_bw.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/convert_to_bw.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/downsample_multiple_videos_popup.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/downsample_multiple_videos_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/unsupervised_lof.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/unsupervised_lof.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/siegel_tukey.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/siegel_tukey.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/berger_parker.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/berger_parker.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/isolation_forest.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/isolation_forest.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/davis_bouldin.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/davis_bouldin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/vertical_video_concatenator.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/vertical_video_concatenator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/batch_video_to_greyscale.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/batch_video_to_greyscale.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/crop_circles_pop_up.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/crop_circles_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/heading.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/heading.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/piotr_120324 2.py.zip` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/piotr_120324 2.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/mutual_exclusive.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/mutual_exclusive.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/mahalanobis.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/mahalanobis.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/superpixels.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/superpixels.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/img_conv.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/img_conv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/grangercausalitytests.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/grangercausalitytests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/multiframe_is_shape_covered.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/multiframe_is_shape_covered.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/redis.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/redis.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/video_color.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/video_color.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/graph_3d_plotter.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/graph_3d_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/blurbox.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/blurbox.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/piotr_120324.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/piotr_120324.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/video_rotator.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/video_rotator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/superimpose_frame_count.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/superimpose_frame_count.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/inset_overlay_video.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/inset_overlay_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/hartley_fmax.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/hartley_fmax.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/fix_clahe.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/fix_clahe.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/cochran_q.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/cochran_q.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/menhinicks_index.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/menhinicks_index.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/add_probability_cnt_features.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/add_probability_cnt_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/brillouins_index.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/brillouins_index.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/spontanous_alternations.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/spontanous_alternations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/eta_squared.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/eta_squared.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/piotr_120324.py.zip` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/piotr_120324.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/convert_to_mp4.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/convert_to_mp4.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/velocity_aggregator.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/velocity_aggregator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/make_splash.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/make_splash.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/change_img_file_format.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/change_img_file_format.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/abod.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/abod.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/fish_feature_extractor_2023_version_5.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/fish_feature_extractor_2023_version_5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/violin.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/violin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/bg_substraction.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/bg_substraction.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/simpson_diversity_index.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/simpson_diversity_index.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/clip_videos_by_frm.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/clip_videos_by_frm.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/fleiss_kappa.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/fleiss_kappa.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/piotr_120324 4.py.zip` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/piotr_120324 4.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/convert_to_popup.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/convert_to_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/rotate image.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/rotate image.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/jaccard_distance.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/jaccard_distance.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/geometry_ex.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/geometry_ex.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/time_stamp_calculator.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/time_stamp_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/line_plot.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/line_plot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/video_rotator_mp.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/video_rotator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/unsupervised_outliers.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/unsupervised_outliers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/manhattan_distance.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/manhattan_distance.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/statistics_ex.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/statistics_ex.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/ROI_plotter.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/ROI_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/sliding_displacement.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/sliding_displacement.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/path_plots.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/path_plots.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/seekable.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/seekable.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/superimpose_elapsed_time.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/superimpose_elapsed_time.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/wald_wolfowitz.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/wald_wolfowitz.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/relative_risk.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/relative_risk.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/sliding_autoc.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/sliding_autoc.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/linestring_path.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/linestring_path.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/cronbach_alpha.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/cronbach_alpha.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/mcnamar.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/mcnamar.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/contrast.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/contrast.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/fish_feature_extractor_2023_version_4.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/fish_feature_extractor_2023_version_4.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/AmberFeatureExtractor.py.zip` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/AmberFeatureExtractor.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/youden_j.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/youden_j.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/mosaic.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/mosaic.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/amber_featurizer.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/amber_featurizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/make_path_plot.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/make_path_plot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/margalef_diversification_index.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/margalef_diversification_index.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/biweight_midcorrelation.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/biweight_midcorrelation.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/madmedianrule.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/madmedianrule.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/adjusted_rand_score.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/adjusted_rand_score.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/convex_hull_scratch_2.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/convex_hull_scratch_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/sandbox/plotly_gantt.py` & `Simba-UW-tf-dev-1.92.5/simba/sandbox/plotly_gantt.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/plotting/directing_animals_to_bodypart_visualizer.py` & `Simba-UW-tf-dev-1.92.5/simba/plotting/directing_animals_to_bodypart_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/plotting/gantt_creator.py` & `Simba-UW-tf-dev-1.92.5/simba/plotting/gantt_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/plotting/tools/tkinter_tools.py` & `Simba-UW-tf-dev-1.92.5/simba/plotting/tools/tkinter_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/plotting/ROI_plotter_mp.py` & `Simba-UW-tf-dev-1.92.5/simba/plotting/ROI_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/plotting/.DS_Store` & `Simba-UW-tf-dev-1.92.5/simba/plotting/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/plotting/shap_agg_stats_visualizer.py` & `Simba-UW-tf-dev-1.92.5/simba/plotting/shap_agg_stats_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/plotting/gantt_creator_mp.py` & `Simba-UW-tf-dev-1.92.5/simba/plotting/gantt_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/plotting/heat_mapper_clf_mp.py` & `Simba-UW-tf-dev-1.92.5/simba/plotting/heat_mapper_clf_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/plotting/probability_plot_creator.py` & `Simba-UW-tf-dev-1.92.5/simba/plotting/probability_plot_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/plotting/circular_plotting.py` & `Simba-UW-tf-dev-1.92.5/simba/plotting/circular_plotting.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/plotting/plot_clf_results.py` & `Simba-UW-tf-dev-1.92.5/simba/plotting/plot_clf_results.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/plotting/ez_path_plot.py` & `Simba-UW-tf-dev-1.92.5/simba/plotting/ez_path_plot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/plotting/plot_clf_results_mp.py` & `Simba-UW-tf-dev-1.92.5/simba/plotting/plot_clf_results_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/plotting/ROI_feature_visualizer.py` & `Simba-UW-tf-dev-1.92.5/simba/plotting/ROI_feature_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/plotting/heat_mapper_location.py` & `Simba-UW-tf-dev-1.92.5/simba/plotting/heat_mapper_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/plotting/probability_plot_creator_mp.py` & `Simba-UW-tf-dev-1.92.5/simba/plotting/probability_plot_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/plotting/interactive_probability_grapher.py` & `Simba-UW-tf-dev-1.92.5/simba/plotting/interactive_probability_grapher.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/plotting/plot_pose_in_dir.py` & `Simba-UW-tf-dev-1.92.5/simba/plotting/plot_pose_in_dir.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/plotting/single_run_model_validation_video.py` & `Simba-UW-tf-dev-1.92.5/simba/plotting/single_run_model_validation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/plotting/frame_mergerer_ffmpeg.py` & `Simba-UW-tf-dev-1.92.5/simba/plotting/frame_mergerer_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/plotting/pose_plotter_mp.py` & `Simba-UW-tf-dev-1.92.5/simba/plotting/pose_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/plotting/directing_animals_visualizer_mp.py` & `Simba-UW-tf-dev-1.92.5/simba/plotting/directing_animals_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/plotting/clf_validator.py` & `Simba-UW-tf-dev-1.92.5/simba/plotting/clf_validator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/plotting/path_plotter_mp.py` & `Simba-UW-tf-dev-1.92.5/simba/plotting/path_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/plotting/ROI_feature_visualizer_mp.py` & `Simba-UW-tf-dev-1.92.5/simba/plotting/ROI_feature_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/plotting/data_plotter.py` & `Simba-UW-tf-dev-1.92.5/simba/plotting/data_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/plotting/spontaneous_alternation_plotter.py` & `Simba-UW-tf-dev-1.92.5/simba/plotting/spontaneous_alternation_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/plotting/path_plotter.py` & `Simba-UW-tf-dev-1.92.5/simba/plotting/path_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/plotting/distance_plotter_mp.py` & `Simba-UW-tf-dev-1.92.5/simba/plotting/distance_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/plotting/ROI_plotter.py` & `Simba-UW-tf-dev-1.92.5/simba/plotting/ROI_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/plotting/geometry_plotter.py` & `Simba-UW-tf-dev-1.92.5/simba/plotting/geometry_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/plotting/clf_validator_mp.py` & `Simba-UW-tf-dev-1.92.5/simba/plotting/clf_validator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/plotting/heat_mapper_clf.py` & `Simba-UW-tf-dev-1.92.5/simba/plotting/heat_mapper_clf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/plotting/distance_plotter.py` & `Simba-UW-tf-dev-1.92.5/simba/plotting/distance_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/plotting/single_run_model_validation_video_mp.py` & `Simba-UW-tf-dev-1.92.5/simba/plotting/single_run_model_validation_video_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/plotting/directing_animals_visualizer.py` & `Simba-UW-tf-dev-1.92.5/simba/plotting/directing_animals_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/plotting/circular_feature_overlay_plotter.py` & `Simba-UW-tf-dev-1.92.5/simba/plotting/circular_feature_overlay_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/plotting/heat_mapper_location_mp.py` & `Simba-UW-tf-dev-1.92.5/simba/plotting/heat_mapper_location_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/dash_app/SimBA_dash_app.py` & `Simba-UW-tf-dev-1.92.5/simba/dash_app/SimBA_dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/dash_app/run_dash_tkinter.py` & `Simba-UW-tf-dev-1.92.5/simba/dash_app/run_dash_tkinter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/dash_app/dash_app.py` & `Simba-UW-tf-dev-1.92.5/simba/dash_app/dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/data_processors/spontaneous_alternation_calculator.py` & `Simba-UW-tf-dev-1.92.5/simba/data_processors/spontaneous_alternation_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/data_processors/agg_clf_calculator.py` & `Simba-UW-tf-dev-1.92.5/simba/data_processors/agg_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/data_processors/.DS_Store` & `Simba-UW-tf-dev-1.92.5/simba/data_processors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/data_processors/severity_bout_based_calculator.py` & `Simba-UW-tf-dev-1.92.5/simba/data_processors/severity_bout_based_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/data_processors/interpolation_smoothing.py` & `Simba-UW-tf-dev-1.92.5/simba/data_processors/interpolation_smoothing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/data_processors/directing_animal_to_bodypart.py` & `Simba-UW-tf-dev-1.92.5/simba/data_processors/directing_animal_to_bodypart.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/data_processors/timebins_clf_calculator.py` & `Simba-UW-tf-dev-1.92.5/simba/data_processors/timebins_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/data_processors/fsttc_calculator.py` & `Simba-UW-tf-dev-1.92.5/simba/data_processors/fsttc_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/data_processors/boolean_conditional_calculator.py` & `Simba-UW-tf-dev-1.92.5/simba/data_processors/boolean_conditional_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/data_processors/interpolate_pose.py` & `Simba-UW-tf-dev-1.92.5/simba/data_processors/interpolate_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/data_processors/directing_other_animals_calculator.py` & `Simba-UW-tf-dev-1.92.5/simba/data_processors/directing_other_animals_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/data_processors/gibbs_sampler.py` & `Simba-UW-tf-dev-1.92.5/simba/data_processors/gibbs_sampler.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/data_processors/timebins_movement_calculator.py` & `Simba-UW-tf-dev-1.92.5/simba/data_processors/timebins_movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/data_processors/severity_calculator.py` & `Simba-UW-tf-dev-1.92.5/simba/data_processors/severity_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/data_processors/pup_retrieval_calculator.py` & `Simba-UW-tf-dev-1.92.5/simba/data_processors/pup_retrieval_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/data_processors/pybursts_calculator.py` & `Simba-UW-tf-dev-1.92.5/simba/data_processors/pybursts_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/data_processors/severity_frame_based_calculator.py` & `Simba-UW-tf-dev-1.92.5/simba/data_processors/severity_frame_based_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/data_processors/mutual_exclusivity_corrector.py` & `Simba-UW-tf-dev-1.92.5/simba/data_processors/mutual_exclusivity_corrector.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/data_processors/kleinberg_calculator.py` & `Simba-UW-tf-dev-1.92.5/simba/data_processors/kleinberg_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/data_processors/movement_calculator.py` & `Simba-UW-tf-dev-1.92.5/simba/data_processors/movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/model/train_rf.py` & `Simba-UW-tf-dev-1.92.5/simba/model/train_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/model/inference_batch.py` & `Simba-UW-tf-dev-1.92.5/simba/model/inference_batch.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/model/train_multiclass_rf.py` & `Simba-UW-tf-dev-1.92.5/simba/model/train_multiclass_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/model/inference_multiclass_batch.py` & `Simba-UW-tf-dev-1.92.5/simba/model/inference_multiclass_batch.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/model/grid_search_multiclass_rf.py` & `Simba-UW-tf-dev-1.92.5/simba/model/grid_search_multiclass_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/model/grid_search_rf.py` & `Simba-UW-tf-dev-1.92.5/simba/model/grid_search_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/model/inference_validation.py` & `Simba-UW-tf-dev-1.92.5/simba/model/inference_validation.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/model/train_multilabel_rf.py` & `Simba-UW-tf-dev-1.92.5/simba/model/train_multilabel_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/roi_tools/ROI_time_bin_calculator.py` & `Simba-UW-tf-dev-1.92.5/simba/roi_tools/ROI_time_bin_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/roi_tools/.DS_Store` & `Simba-UW-tf-dev-1.92.5/simba/roi_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/roi_tools/ROI_define.py` & `Simba-UW-tf-dev-1.92.5/simba/roi_tools/ROI_define.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/roi_tools/ROI_reset.py` & `Simba-UW-tf-dev-1.92.5/simba/roi_tools/ROI_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/roi_tools/ROI_size_standardizer.py` & `Simba-UW-tf-dev-1.92.5/simba/roi_tools/ROI_size_standardizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/roi_tools/ROI_analyzer.py` & `Simba-UW-tf-dev-1.92.5/simba/roi_tools/ROI_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/roi_tools/ROI_feature_analyzer.py` & `Simba-UW-tf-dev-1.92.5/simba/roi_tools/ROI_feature_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/roi_tools/ROI_multiply.py` & `Simba-UW-tf-dev-1.92.5/simba/roi_tools/ROI_multiply.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/roi_tools/ROI_size_calculations.py` & `Simba-UW-tf-dev-1.92.5/simba/roi_tools/ROI_size_calculations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/roi_tools/ROI_zoom.py` & `Simba-UW-tf-dev-1.92.5/simba/roi_tools/ROI_zoom.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/roi_tools/ROI_directing_analyzer.py` & `Simba-UW-tf-dev-1.92.5/simba/roi_tools/ROI_directing_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/roi_tools/ROI_move_shape.py` & `Simba-UW-tf-dev-1.92.5/simba/roi_tools/ROI_move_shape.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/roi_tools/ROI_menus.py` & `Simba-UW-tf-dev-1.92.5/simba/roi_tools/ROI_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/roi_tools/ROI_clf_calculator.py` & `Simba-UW-tf-dev-1.92.5/simba/roi_tools/ROI_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/roi_tools/ROI_image.py` & `Simba-UW-tf-dev-1.92.5/simba/roi_tools/ROI_image.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/pose_importers/sleap_csv_importer.py` & `Simba-UW-tf-dev-1.92.5/simba/pose_importers/sleap_csv_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/pose_importers/misc/apt_trk_importer.py` & `Simba-UW-tf-dev-1.92.5/simba/pose_importers/misc/apt_trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/pose_importers/read_DANNCE_mat.py` & `Simba-UW-tf-dev-1.92.5/simba/pose_importers/read_DANNCE_mat.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/pose_importers/.DS_Store` & `Simba-UW-tf-dev-1.92.5/simba/pose_importers/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/pose_importers/sleap_h5_importer.py` & `Simba-UW-tf-dev-1.92.5/simba/pose_importers/sleap_h5_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/pose_importers/madlc_importer.py` & `Simba-UW-tf-dev-1.92.5/simba/pose_importers/madlc_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/pose_importers/sleap_slp_importer.py` & `Simba-UW-tf-dev-1.92.5/simba/pose_importers/sleap_slp_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/pose_importers/import_mars.py` & `Simba-UW-tf-dev-1.92.5/simba/pose_importers/import_mars.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/pose_importers/dlc_importer_csv.py` & `Simba-UW-tf-dev-1.92.5/simba/pose_importers/dlc_importer_csv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/pose_importers/trk_importer.py` & `Simba-UW-tf-dev-1.92.5/simba/pose_importers/trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/pose_configurations/.DS_Store` & `Simba-UW-tf-dev-1.92.5/simba/pose_configurations/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/pose_configurations/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.92.5/simba/pose_configurations/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/pose_configurations/schematics/8.png` & `Simba-UW-tf-dev-1.92.5/simba/pose_configurations/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/pose_configurations/schematics/9.png` & `Simba-UW-tf-dev-1.92.5/simba/pose_configurations/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/pose_configurations/schematics/12.png` & `Simba-UW-tf-dev-1.92.5/simba/pose_configurations/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/pose_configurations/schematics/13.png` & `Simba-UW-tf-dev-1.92.5/simba/pose_configurations/schematics/13.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/pose_configurations/schematics/11.png` & `Simba-UW-tf-dev-1.92.5/simba/pose_configurations/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/pose_configurations/schematics/10.png` & `Simba-UW-tf-dev-1.92.5/simba/pose_configurations/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/pose_configurations/schematics/4.png` & `Simba-UW-tf-dev-1.92.5/simba/pose_configurations/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/pose_configurations/schematics/5.png` & `Simba-UW-tf-dev-1.92.5/simba/pose_configurations/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/pose_configurations/schematics/7.png` & `Simba-UW-tf-dev-1.92.5/simba/pose_configurations/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/pose_configurations/schematics/6.png` & `Simba-UW-tf-dev-1.92.5/simba/pose_configurations/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/pose_configurations/schematics/2.png` & `Simba-UW-tf-dev-1.92.5/simba/pose_configurations/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/pose_configurations/schematics/3.png` & `Simba-UW-tf-dev-1.92.5/simba/pose_configurations/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/pose_configurations/schematics/1.png` & `Simba-UW-tf-dev-1.92.5/simba/pose_configurations/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/video_processors/video_processing.py` & `Simba-UW-tf-dev-1.92.5/simba/video_processors/video_processing.py`

 * *Files 2% similar despite different names*

```diff
@@ -9038,2859 +9038,2863 @@
 000234d0: 6420 746f 204d 4f56 2061 6e64 2073 6176  d to MOV and sav
 000234e0: 6564 2069 6e20 7b73 6176 655f 6469 727d  ed in {save_dir}
 000234f0: 2064 6972 6563 746f 7279 2e22 2c20 656c   directory.", el
 00023500: 6170 7365 645f 7469 6d65 3d74 696d 6572  apsed_time=timer
 00023510: 2e65 6c61 7073 6564 5f74 696d 655f 7374  .elapsed_time_st
 00023520: 722c 2073 6f75 7263 653d 636f 6e76 6572  r, source=conver
 00023530: 745f 746f 5f6d 6f76 2e5f 5f6e 616d 655f  t_to_mov.__name_
-00023540: 5f2c 2029 0a0a 0a64 6566 206f 7665 726c  _, )...def overl
-00023550: 6179 5f76 6964 656f 5f70 726f 6772 6573  ay_video_progres
-00023560: 7362 6172 2876 6964 656f 5f70 6174 683a  sbar(video_path:
-00023570: 2055 6e69 6f6e 5b73 7472 2c20 6f73 2e50   Union[str, os.P
-00023580: 6174 684c 696b 655d 2c0a 2020 2020 2020  athLike],.      
+00023540: 5f2c 2029 0a0a 0a64 6566 2073 7570 6572  _, )...def super
+00023550: 696d 706f 7365 5f76 6964 656f 5f70 726f  impose_video_pro
+00023560: 6772 6573 7362 6172 2876 6964 656f 5f70  gressbar(video_p
+00023570: 6174 683a 2055 6e69 6f6e 5b73 7472 2c20  ath: Union[str, 
+00023580: 6f73 2e50 6174 684c 696b 655d 2c0a 2020  os.PathLike],.  
 00023590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000235a0: 2020 2020 2020 2020 6261 725f 6865 6967          bar_heig
-000235b0: 6874 3a20 4f70 7469 6f6e 616c 5b69 6e74  ht: Optional[int
-000235c0: 5d20 3d20 3130 2c0a 2020 2020 2020 2020  ] = 10,.        
+000235a0: 2020 2020 2020 2020 2020 2020 6261 725f              bar_
+000235b0: 6865 6967 6874 3a20 4f70 7469 6f6e 616c  height: Optional
+000235c0: 5b69 6e74 5d20 3d20 3130 2c0a 2020 2020  [int] = 10,.    
 000235d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000235e0: 2020 2020 2020 636f 6c6f 723a 204f 7074        color: Opt
-000235f0: 696f 6e61 6c5b 7374 725d 203d 2027 7265  ional[str] = 're
-00023600: 6427 2c0a 2020 2020 2020 2020 2020 2020  d',.            
+000235e0: 2020 2020 2020 2020 2020 636f 6c6f 723a            color:
+000235f0: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
+00023600: 2027 7265 6427 2c0a 2020 2020 2020 2020   'red',.        
 00023610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023620: 2020 706f 7369 7469 6f6e 3a20 4f70 7469    position: Opti
-00023630: 6f6e 616c 5b4c 6974 6572 616c 5b27 746f  onal[Literal['to
-00023640: 7027 2c20 2762 6f74 746f 6d27 5d5d 203d  p', 'bottom']] =
-00023650: 2027 626f 7474 6f6d 272c 0a20 2020 2020   'bottom',.     
+00023620: 2020 2020 2020 706f 7369 7469 6f6e 3a20        position: 
+00023630: 4f70 7469 6f6e 616c 5b4c 6974 6572 616c  Optional[Literal
+00023640: 5b27 746f 7027 2c20 2762 6f74 746f 6d27  ['top', 'bottom'
+00023650: 5d5d 203d 2027 626f 7474 6f6d 272c 0a20  ]] = 'bottom',. 
 00023660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023670: 2020 2020 2020 2020 2073 6176 655f 6469           save_di
-00023680: 723a 204f 7074 696f 6e61 6c5b 556e 696f  r: Optional[Unio
-00023690: 6e5b 7374 722c 206f 732e 5061 7468 4c69  n[str, os.PathLi
-000236a0: 6b65 5d5d 203d 204e 6f6e 6529 202d 3e20  ke]] = None) -> 
-000236b0: 4e6f 6e65 3a0a 0a20 2020 2022 2222 0a20  None:..    """. 
-000236c0: 2020 204f 7665 726c 6179 2061 2070 726f     Overlay a pro
-000236d0: 6772 6573 7320 6261 7220 6f6e 2061 2064  gress bar on a d
-000236e0: 6972 6563 746f 7279 206f 6620 7669 6465  irectory of vide
-000236f0: 6f73 206f 7220 6120 7369 6e67 6c65 2076  os or a single v
-00023700: 6964 656f 2e0a 0a20 2020 202e 2e20 7669  ideo...    .. vi
-00023710: 6465 6f3a 3a20 5f73 7461 7469 632f 696d  deo:: _static/im
-00023720: 672f 6f76 6572 6c61 795f 7669 6465 6f5f  g/overlay_video_
-00023730: 7072 6f67 7265 7373 6261 722e 7765 626d  progressbar.webm
-00023740: 0a20 2020 2020 2020 3a77 6964 7468 3a20  .       :width: 
-00023750: 3730 300a 2020 2020 2020 203a 6c6f 6f70  700.       :loop
-00023760: 3a0a 0a20 2020 203a 7061 7261 6d20 556e  :..    :param Un
-00023770: 696f 6e5b 7374 722c 206f 732e 5061 7468  ion[str, os.Path
-00023780: 4c69 6b65 5d20 7669 6465 6f5f 7061 7468  Like] video_path
-00023790: 3a20 4469 7265 6374 6f72 7920 636f 6e74  : Directory cont
-000237a0: 6169 6e69 6e67 2076 6964 656f 2066 696c  aining video fil
-000237b0: 6573 206f 7220 6120 7369 6e67 6c65 2076  es or a single v
-000237c0: 6964 656f 2066 696c 650a 2020 2020 3a70  ideo file.    :p
-000237d0: 6172 616d 204f 7074 696f 6e61 6c5b 696e  aram Optional[in
-000237e0: 745d 2062 6172 5f68 6569 6768 743a 2054  t] bar_height: T
-000237f0: 6865 2068 6569 6768 7420 6f66 2074 6865  he height of the
-00023800: 2070 726f 6772 6573 7362 6172 2069 6e20   progressbar in 
-00023810: 7065 7263 656e 7420 6f66 2074 6865 2076  percent of the v
-00023820: 6964 656f 2068 6569 6768 742e 0a20 2020  ideo height..   
-00023830: 203a 7061 7261 6d20 4f70 7469 6f6e 616c   :param Optional
-00023840: 5b73 7472 5d20 636f 6c6f 723a 2054 6865  [str] color: The
-00023850: 2063 6f6c 6f72 206f 6620 7468 6520 7072   color of the pr
-00023860: 6f67 7265 7373 2062 6172 2e20 5365 6520  ogress bar. See 
-00023870: 7369 6d62 612e 7574 696c 732e 6c6f 6f6b  simba.utils.look
-00023880: 7570 732e 6765 745f 636f 6c6f 725f 6469  ups.get_color_di
-00023890: 6374 206b 6579 7320 666f 7220 6163 6365  ct keys for acce
-000238a0: 7074 6564 206e 616d 6573 2e0a 2020 2020  pted names..    
-000238b0: 3a70 6172 616d 204f 7074 696f 6e61 6c5b  :param Optional[
-000238c0: 7374 725d 2070 6f73 6974 696f 6e3a 2054  str] position: T
-000238d0: 6865 2070 6f73 6974 696f 6e20 6f66 2074  he position of t
-000238e0: 6865 2070 726f 6772 6573 7362 6172 2e20  he progressbar. 
-000238f0: 4f70 7469 6f6e 733a 2027 746f 7027 2c20  Options: 'top', 
-00023900: 2762 6f74 746f 6d27 2e0a 2020 2020 3a70  'bottom'..    :p
-00023910: 6172 616d 204f 7074 696f 6e61 6c5b 556e  aram Optional[Un
-00023920: 696f 6e5b 7374 722c 206f 732e 5061 7468  ion[str, os.Path
-00023930: 4c69 6b65 5d5d 2073 6176 655f 6469 723a  Like]] save_dir:
-00023940: 2049 6620 6e6f 7420 4e6f 6e65 2c20 7468   If not None, th
-00023950: 656e 2073 6176 6573 2074 6865 2076 6964  en saves the vid
-00023960: 656f 7320 696e 2074 6865 2070 6173 7365  eos in the passe
-00023970: 6420 6469 7265 6374 6f72 792e 2045 6c73  d directory. Els
-00023980: 652c 2069 6e20 7468 6520 7361 6d65 2064  e, in the same d
-00023990: 6972 6563 7472 7920 7769 7468 2074 6865  irectry with the
-000239a0: 2060 605f 7072 6f67 7265 7373 5f62 6172   ``_progress_bar
-000239b0: 6060 2073 7566 6669 782e 0a20 2020 203a  `` suffix..    :
-000239c0: 7265 7475 726e 3a20 4e6f 6e65 2e0a 2020  return: None..  
-000239d0: 2020 2222 220a 0a20 2020 2063 6865 636b    """..    check
-000239e0: 5f66 666d 7065 675f 6176 6169 6c61 626c  _ffmpeg_availabl
-000239f0: 6528 7261 6973 655f 6572 726f 723d 5472  e(raise_error=Tr
-00023a00: 7565 290a 2020 2020 7469 6d65 7220 3d20  ue).    timer = 
-00023a10: 5369 6d62 6154 696d 6572 2873 7461 7274  SimbaTimer(start
-00023a20: 3d54 7275 6529 0a20 2020 2063 6f6c 6f72  =True).    color
-00023a30: 203d 2027 272e 6a6f 696e 2866 696c 7465   = ''.join(filte
-00023a40: 7228 7374 722e 6973 616c 6e75 6d2c 2063  r(str.isalnum, c
-00023a50: 6f6c 6f72 2929 2e6c 6f77 6572 2829 0a20  olor)).lower(). 
-00023a60: 2020 2069 6620 6f73 2e70 6174 682e 6973     if os.path.is
-00023a70: 6669 6c65 2876 6964 656f 5f70 6174 6829  file(video_path)
-00023a80: 3a0a 2020 2020 2020 2020 6368 6563 6b5f  :.        check_
-00023a90: 6669 6c65 5f65 7869 7374 5f61 6e64 5f72  file_exist_and_r
-00023aa0: 6561 6461 626c 6528 6669 6c65 5f70 6174  eadable(file_pat
-00023ab0: 683d 7669 6465 6f5f 7061 7468 290a 2020  h=video_path).  
-00023ac0: 2020 2020 2020 7669 6465 6f5f 7061 7468        video_path
-00023ad0: 7320 3d20 5b76 6964 656f 5f70 6174 685d  s = [video_path]
-00023ae0: 0a20 2020 2065 6c69 6620 6f73 2e70 6174  .    elif os.pat
-00023af0: 682e 6973 6469 7228 7669 6465 6f5f 7061  h.isdir(video_pa
-00023b00: 7468 293a 0a20 2020 2020 2020 2076 6964  th):.        vid
-00023b10: 656f 5f70 6174 6820 3d20 6669 6e64 5f61  eo_path = find_a
-00023b20: 6c6c 5f76 6964 656f 735f 696e 5f64 6972  ll_videos_in_dir
-00023b30: 6563 746f 7279 2864 6972 6563 746f 7279  ectory(directory
-00023b40: 3d76 6964 656f 5f70 6174 682c 2061 735f  =video_path, as_
-00023b50: 6469 6374 3d54 7275 652c 2072 6169 7365  dict=True, raise
-00023b60: 5f65 7272 6f72 3d54 7275 6529 0a20 2020  _error=True).   
-00023b70: 2020 2020 2076 6964 656f 5f70 6174 6873       video_paths
-00023b80: 203d 206c 6973 7428 7669 6465 6f5f 7061   = list(video_pa
-00023b90: 7468 2e76 616c 7565 7328 2929 0a20 2020  th.values()).   
-00023ba0: 2065 6c73 653a 0a20 2020 2020 2020 2072   else:.        r
-00023bb0: 6169 7365 2049 6e76 616c 6964 496e 7075  aise InvalidInpu
-00023bc0: 7445 7272 6f72 286d 7367 3d27 7b7d 2069  tError(msg='{} i
-00023bd0: 7320 6e6f 7420 6120 7661 6c69 6420 6669  s not a valid fi
-00023be0: 6c65 2070 6174 6820 6f72 2064 6972 6563  le path or direc
-00023bf0: 746f 7279 2070 6174 682e 272c 2073 6f75  tory path.', sou
-00023c00: 7263 653d 6f76 6572 6c61 795f 7669 6465  rce=overlay_vide
-00023c10: 6f5f 7072 6f67 7265 7373 6261 722e 5f5f  o_progressbar.__
-00023c20: 6e61 6d65 5f5f 290a 2020 2020 6966 2073  name__).    if s
-00023c30: 6176 655f 6469 7220 6973 206e 6f74 204e  ave_dir is not N
-00023c40: 6f6e 653a 0a20 2020 2020 2020 2063 6865  one:.        che
-00023c50: 636b 5f69 665f 6469 725f 6578 6973 7473  ck_if_dir_exists
-00023c60: 2869 6e5f 6469 723d 7361 7665 5f64 6972  (in_dir=save_dir
-00023c70: 290a 2020 2020 656c 7365 3a0a 2020 2020  ).    else:.    
-00023c80: 2020 2020 7361 7665 5f64 6972 2c20 5f2c      save_dir, _,
-00023c90: 205f 203d 2067 6574 5f66 6e5f 6578 7428   _ = get_fn_ext(
-00023ca0: 6669 6c65 7061 7468 3d76 6964 656f 5f70  filepath=video_p
-00023cb0: 6174 6873 5b30 5d29 0a20 2020 2066 6f72  aths[0]).    for
-00023cc0: 2063 6e74 2c20 7669 6465 6f5f 7061 7468   cnt, video_path
-00023cd0: 2069 6e20 656e 756d 6572 6174 6528 7669   in enumerate(vi
-00023ce0: 6465 6f5f 7061 7468 7329 3a0a 2020 2020  deo_paths):.    
-00023cf0: 2020 2020 7669 6465 6f5f 6d65 7461 5f64      video_meta_d
-00023d00: 6174 6120 3d20 6765 745f 7669 6465 6f5f  ata = get_video_
-00023d10: 6d65 7461 5f64 6174 6128 7669 6465 6f5f  meta_data(video_
-00023d20: 7061 7468 3d76 6964 656f 5f70 6174 6829  path=video_path)
-00023d30: 0a20 2020 2020 2020 2076 6964 656f 5f6c  .        video_l
-00023d40: 656e 6774 6820 3d20 7669 6465 6f5f 6d65  ength = video_me
-00023d50: 7461 5f64 6174 615b 2776 6964 656f 5f6c  ta_data['video_l
-00023d60: 656e 6774 685f 7327 5d0a 2020 2020 2020  ength_s'].      
-00023d70: 2020 7769 6474 682c 2068 6569 6768 7420    width, height 
-00023d80: 3d20 7669 6465 6f5f 6d65 7461 5f64 6174  = video_meta_dat
-00023d90: 615b 2777 6964 7468 275d 2c20 7669 6465  a['width'], vide
-00023da0: 6f5f 6d65 7461 5f64 6174 615b 2768 6569  o_meta_data['hei
-00023db0: 6768 7427 5d0a 2020 2020 2020 2020 6261  ght'].        ba
-00023dc0: 725f 6865 6967 6874 203d 2069 6e74 2868  r_height = int(h
-00023dd0: 6569 6768 7420 2a20 2862 6172 5f68 6569  eight * (bar_hei
-00023de0: 6768 742f 3130 3029 290a 2020 2020 2020  ght/100)).      
-00023df0: 2020 5f2c 2076 6964 656f 5f6e 616d 652c    _, video_name,
-00023e00: 2065 7874 203d 2067 6574 5f66 6e5f 6578   ext = get_fn_ex
-00023e10: 7428 6669 6c65 7061 7468 3d76 6964 656f  t(filepath=video
-00023e20: 5f70 6174 6829 0a20 2020 2020 2020 2070  _path).        p
-00023e30: 7269 6e74 2866 2749 6e73 6572 7469 6e67  rint(f'Inserting
-00023e40: 2070 726f 6772 6573 7320 6261 7220 6f6e   progress bar on
-00023e50: 2076 6964 656f 207b 7669 6465 6f5f 6e61   video {video_na
-00023e60: 6d65 7d2e 2e2e 2729 0a20 2020 2020 2020  me}...').       
-00023e70: 2073 6176 655f 7061 7468 203d 206f 732e   save_path = os.
-00023e80: 7061 7468 2e6a 6f69 6e28 7361 7665 5f64  path.join(save_d
-00023e90: 6972 2c20 6627 7b76 6964 656f 5f6e 616d  ir, f'{video_nam
-00023ea0: 657d 5f70 726f 6772 6573 735f 6261 727b  e}_progress_bar{
-00023eb0: 6578 747d 2729 0a20 2020 2020 2020 2063  ext}').        c
-00023ec0: 6865 636b 5f69 6e74 286e 616d 653d 6627  heck_int(name=f'
-00023ed0: 7b6f 7665 726c 6179 5f76 6964 656f 5f70  {overlay_video_p
-00023ee0: 726f 6772 6573 7362 6172 7d20 6865 6967  rogressbar} heig
-00023ef0: 6874 272c 2076 616c 7565 3d62 6172 5f68  ht', value=bar_h
-00023f00: 6569 6768 742c 206d 6178 5f76 616c 7565  eight, max_value
-00023f10: 3d68 6569 6768 742c 206d 696e 5f76 616c  =height, min_val
-00023f20: 7565 3d31 290a 2020 2020 2020 2020 6966  ue=1).        if
-00023f30: 2070 6f73 6974 696f 6e20 3d3d 2027 626f   position == 'bo
-00023f40: 7474 6f6d 273a 0a20 2020 2020 2020 2020  ttom':.         
-00023f50: 2020 2063 6d64 203d 2066 2766 666d 7065     cmd = f'ffmpe
-00023f60: 6720 2d69 2022 7b76 6964 656f 5f70 6174  g -i "{video_pat
-00023f70: 687d 2220 2d66 696c 7465 725f 636f 6d70  h}" -filter_comp
-00023f80: 6c65 7820 2263 6f6c 6f72 3d63 3d7b 636f  lex "color=c={co
-00023f90: 6c6f 727d 3a73 3d7b 7769 6474 687d 787b  lor}:s={width}x{
-00023fa0: 6261 725f 6865 6967 6874 7d5b 6261 725d  bar_height}[bar]
-00023fb0: 3b5b 305d 5b62 6172 5d6f 7665 726c 6179  ;[0][bar]overlay
-00023fc0: 3d2d 772b 2877 2f7b 7669 6465 6f5f 6c65  =-w+(w/{video_le
-00023fd0: 6e67 7468 7d29 2a74 3a48 2d68 3a73 686f  ngth})*t:H-h:sho
-00023fe0: 7274 6573 743d 3122 202d 633a 6120 636f  rtest=1" -c:a co
-00023ff0: 7079 2022 7b73 6176 655f 7061 7468 7d22  py "{save_path}"
-00024000: 202d 6c6f 676c 6576 656c 2065 7272 6f72   -loglevel error
-00024010: 202d 7374 6174 7320 2d68 6964 655f 6261   -stats -hide_ba
-00024020: 6e6e 6572 202d 7927 0a20 2020 2020 2020  nner -y'.       
-00024030: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00024040: 2020 2063 6d64 203d 2066 2766 666d 7065     cmd = f'ffmpe
-00024050: 6720 2d69 2022 7b76 6964 656f 5f70 6174  g -i "{video_pat
-00024060: 687d 2220 2d66 696c 7465 725f 636f 6d70  h}" -filter_comp
-00024070: 6c65 7820 2263 6f6c 6f72 3d63 3d7b 636f  lex "color=c={co
-00024080: 6c6f 727d 3a73 3d7b 7769 6474 687d 787b  lor}:s={width}x{
-00024090: 6261 725f 6865 6967 6874 7d5b 6261 725d  bar_height}[bar]
-000240a0: 3b5b 305d 5b62 6172 5d6f 7665 726c 6179  ;[0][bar]overlay
-000240b0: 3d2d 772b 2877 2f7b 7669 6465 6f5f 6c65  =-w+(w/{video_le
-000240c0: 6e67 7468 7d29 2a74 3a7b 6261 725f 6865  ngth})*t:{bar_he
-000240d0: 6967 6874 7d2d 683a 7368 6f72 7465 7374  ight}-h:shortest
-000240e0: 3d31 2220 2d63 3a61 2063 6f70 7920 227b  =1" -c:a copy "{
-000240f0: 7361 7665 5f70 6174 687d 2220 2d6c 6f67  save_path}" -log
-00024100: 6c65 7665 6c20 6572 726f 7220 2d73 7461  level error -sta
-00024110: 7473 202d 6869 6465 5f62 616e 6e65 7220  ts -hide_banner 
-00024120: 2d79 270a 2020 2020 2020 2020 7375 6270  -y'.        subp
-00024130: 726f 6365 7373 2e63 616c 6c28 636d 642c  rocess.call(cmd,
-00024140: 2073 6865 6c6c 3d54 7275 652c 2073 7464   shell=True, std
-00024150: 6f75 743d 7375 6270 726f 6365 7373 2e50  out=subprocess.P
-00024160: 4950 4529 0a20 2020 2074 696d 6572 2e73  IPE).    timer.s
-00024170: 746f 705f 7469 6d65 7228 290a 2020 2020  top_timer().    
-00024180: 7374 646f 7574 5f73 7563 6365 7373 286d  stdout_success(m
-00024190: 7367 3d66 227b 6c65 6e28 7669 6465 6f5f  sg=f"{len(video_
-000241a0: 7061 7468 7329 7d20 7669 6465 6f28 7329  paths)} video(s)
-000241b0: 2073 6176 6564 2077 6974 6820 7072 6f67   saved with prog
-000241c0: 7265 7373 6261 7220 696e 207b 7361 7665  ressbar in {save
-000241d0: 5f64 6972 7d20 6469 7265 6374 6f72 792e  _dir} directory.
-000241e0: 222c 2065 6c61 7073 6564 5f74 696d 653d  ", elapsed_time=
-000241f0: 7469 6d65 722e 656c 6170 7365 645f 7469  timer.elapsed_ti
-00024200: 6d65 5f73 7472 2c20 736f 7572 6365 3d6f  me_str, source=o
-00024210: 7665 726c 6179 5f76 6964 656f 5f70 726f  verlay_video_pro
-00024220: 6772 6573 7362 6172 2e5f 5f6e 616d 655f  gressbar.__name_
-00024230: 5f2c 2029 0a0a 6465 6620 6372 6f73 7366  _, )..def crossf
-00024240: 6164 655f 7477 6f5f 7669 6465 6f73 2876  ade_two_videos(v
-00024250: 6964 656f 5f70 6174 685f 313a 2055 6e69  ideo_path_1: Uni
-00024260: 6f6e 5b73 7472 2c20 6f73 2e50 6174 684c  on[str, os.PathL
-00024270: 696b 655d 2c0a 2020 2020 2020 2020 2020  ike],.          
-00024280: 2020 2020 2020 2020 2020 2020 2020 2076                 v
-00024290: 6964 656f 5f70 6174 685f 323a 2055 6e69  ideo_path_2: Uni
-000242a0: 6f6e 5b73 7472 2c20 6f73 2e50 6174 684c  on[str, os.PathL
-000242b0: 696b 655d 2c0a 2020 2020 2020 2020 2020  ike],.          
-000242c0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-000242d0: 726f 7373 6661 6465 5f64 7572 6174 696f  rossfade_duratio
-000242e0: 6e3a 204f 7074 696f 6e61 6c5b 696e 745d  n: Optional[int]
-000242f0: 203d 2032 2c0a 2020 2020 2020 2020 2020   = 2,.          
-00024300: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00024310: 726f 7373 6661 6465 5f6d 6574 686f 643a  rossfade_method:
-00024320: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
-00024330: 2027 6661 6465 272c 0a20 2020 2020 2020   'fade',.       
-00024340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024350: 2020 6372 6f73 7366 6164 655f 6f66 6673    crossfade_offs
-00024360: 6574 3a20 4f70 7469 6f6e 616c 5b69 6e74  et: Optional[int
-00024370: 5d20 3d20 322c 0a20 2020 2020 2020 2020  ] = 2,.         
-00024380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024390: 7361 7665 5f70 6174 683a 204f 7074 696f  save_path: Optio
-000243a0: 6e61 6c5b 556e 696f 6e5b 7374 722c 206f  nal[Union[str, o
-000243b0: 732e 5061 7468 4c69 6b65 5d5d 203d 204e  s.PathLike]] = N
-000243c0: 6f6e 6529 3a0a 2020 2020 2222 220a 2020  one):.    """.  
-000243d0: 2020 4372 6f73 732d 6661 6465 2074 776f    Cross-fade two
-000243e0: 2076 6964 656f 732e 0a0a 2020 2020 2e2e   videos...    ..
-000243f0: 2076 6964 656f 3a3a 205f 7374 6174 6963   video:: _static
-00024400: 2f69 6d67 2f63 726f 7373 6661 6465 5f74  /img/crossfade_t
-00024410: 776f 5f76 6964 656f 732e 7765 626d 0a20  wo_videos.webm. 
-00024420: 2020 2020 2020 3a6c 6f6f 703a 0a0a 2020        :loop:..  
-00024430: 2020 2e2e 206e 6f74 653a 3a0a 2020 2020    .. note::.    
-00024440: 2020 2053 6565 2060 6073 696d 6261 2e75     See ``simba.u
-00024450: 7469 6c73 2e6c 6f6f 6b75 7073 2e67 6574  tils.lookups.get
-00024460: 5f66 666d 7065 675f 6372 6f73 7366 6164  _ffmpeg_crossfad
-00024470: 655f 6d65 7468 6f64 7360 6020 666f 7220  e_methods`` for 
-00024480: 6e61 6d65 6420 6372 6f73 7366 6164 6520  named crossfade 
-00024490: 6d65 7468 6f64 732e 0a20 2020 2020 2020  methods..       
-000244a0: 5365 6520 6068 7474 7073 3a2f 2f74 7261  See `https://tra
-000244b0: 632e 6666 6d70 6567 2e6f 7267 2f77 696b  c.ffmpeg.org/wik
-000244c0: 692f 5866 6164 6520 3c68 7474 7073 3a2f  i/Xfade <https:/
-000244d0: 2f74 7261 632e 6666 6d70 6567 2e6f 7267  /trac.ffmpeg.org
-000244e0: 2f77 696b 692f 5866 6164 653e 605f 5f2e  /wiki/Xfade>`__.
-000244f0: 2066 6f72 2076 6973 7561 6c69 7a61 7469   for visualizati
-00024500: 6f6e 7320 6f66 206e 616d 6564 2063 726f  ons of named cro
-00024510: 7373 6661 6465 206d 6574 686f 6473 2c0a  ssfade methods,.
-00024520: 0a20 2020 203a 7061 7261 6d20 556e 696f  .    :param Unio
-00024530: 6e5b 7374 722c 206f 732e 5061 7468 4c69  n[str, os.PathLi
-00024540: 6b65 5d20 7669 6465 6f5f 7061 7468 5f31  ke] video_path_1
-00024550: 3a20 5061 7468 2074 6f20 7468 6520 6669  : Path to the fi
-00024560: 7273 7420 7669 6465 6f20 6f6e 2064 6973  rst video on dis
-00024570: 6b2e 0a20 2020 203a 7061 7261 6d20 556e  k..    :param Un
-00024580: 696f 6e5b 7374 722c 206f 732e 5061 7468  ion[str, os.Path
-00024590: 4c69 6b65 5d20 7669 6465 6f5f 7061 7468  Like] video_path
-000245a0: 5f32 3a20 5061 7468 2074 6f20 7468 6520  _2: Path to the 
-000245b0: 7365 636f 6e64 2076 6964 656f 206f 6e20  second video on 
-000245c0: 6469 736b 2e0a 2020 2020 3a70 6172 616d  disk..    :param
-000245d0: 204f 7074 696f 6e61 6c5b 696e 745d 2063   Optional[int] c
-000245e0: 726f 7373 6661 6465 5f64 7572 6174 696f  rossfade_duratio
-000245f0: 6e3a 2054 6865 2064 7572 6174 696f 6e20  n: The duration 
-00024600: 6f66 2074 6865 2063 726f 7373 6661 6465  of the crossfade
-00024610: 2e0a 2020 2020 3a70 6172 616d 204f 7074  ..    :param Opt
-00024620: 696f 6e61 6c5b 7374 725d 2063 726f 7373  ional[str] cross
-00024630: 6661 6465 5f6d 6574 686f 643a 2054 6865  fade_method: The
-00024640: 2063 726f 7373 6661 6465 206d 6574 686f   crossfade metho
-00024650: 642e 2046 6f72 2061 6363 6570 7465 6420  d. For accepted 
-00024660: 6d65 7468 6f64 732c 2073 6565 2060 6073  methods, see ``s
-00024670: 696d 6261 2e75 7469 6c73 2e6c 6f6f 6b75  imba.utils.looku
-00024680: 7073 2e67 6574 5f66 666d 7065 675f 6372  ps.get_ffmpeg_cr
-00024690: 6f73 7366 6164 655f 6d65 7468 6f64 7360  ossfade_methods`
-000246a0: 602e 0a20 2020 203a 7061 7261 6d20 4f70  `..    :param Op
-000246b0: 7469 6f6e 616c 5b69 6e74 5d20 6372 6f73  tional[int] cros
-000246c0: 7366 6164 655f 6f66 6673 6574 3a20 5468  sfade_offset: Th
-000246d0: 6520 7469 6d65 2069 6e20 7365 636f 6e64  e time in second
-000246e0: 7320 696e 746f 2074 6865 2066 6972 7374  s into the first
-000246f0: 2076 6964 656f 2062 6566 6f72 6520 7468   video before th
-00024700: 6520 6372 6f73 7366 6164 6520 6475 7261  e crossfade dura
-00024710: 7469 6f6e 2062 6567 696e 732e 0a20 2020  tion begins..   
-00024720: 203a 7061 7261 6d20 4f70 7469 6f6e 616c   :param Optional
-00024730: 5b55 6e69 6f6e 5b73 7472 2c20 6f73 2e50  [Union[str, os.P
-00024740: 6174 684c 696b 655d 5d20 7361 7665 5f70  athLike]] save_p
-00024750: 6174 683a 2054 6865 206c 6f63 6174 696f  ath: The locatio
-00024760: 6e20 7768 6572 6520 746f 2073 6176 6520  n where to save 
-00024770: 7468 6520 6372 6f73 7366 6164 6564 2076  the crossfaded v
-00024780: 6964 656f 2e20 4966 204e 6f6e 652c 2074  ideo. If None, t
-00024790: 6865 6e20 7361 7665 7320 7468 6520 7669  hen saves the vi
-000247a0: 6465 6f20 696e 2074 6865 2073 616d 6520  deo in the same 
-000247b0: 6469 7265 6374 6f72 7920 6173 2060 6076  directory as ``v
-000247c0: 6964 656f 5f70 6174 685f 3160 6020 7769  ideo_path_1`` wi
-000247d0: 7468 2060 605f 6372 6f73 7366 6164 6560  th ``_crossfade`
-000247e0: 6020 7375 6666 6978 2e0a 0a20 2020 203a  ` suffix...    :
-000247f0: 7265 7475 726e 3a20 4e6f 6e65 2e0a 0a20  return: None... 
-00024800: 2020 203a 6578 616d 706c 653a 0a20 2020     :example:.   
-00024810: 203e 3e3e 2063 726f 7373 6661 6465 5f74   >>> crossfade_t
-00024820: 776f 5f76 6964 656f 7328 7669 6465 6f5f  wo_videos(video_
-00024830: 7061 7468 5f31 3d27 2f55 7365 7273 2f73  path_1='/Users/s
-00024840: 696d 6f6e 2f44 6573 6b74 6f70 2f65 6e76  imon/Desktop/env
-00024850: 732f 7369 6d62 612f 7472 6f75 626c 6573  s/simba/troubles
-00024860: 686f 6f74 696e 672f 7265 7074 696c 652f  hooting/reptile/
-00024870: 312e 6d70 3427 2c20 7669 6465 6f5f 7061  1.mp4', video_pa
-00024880: 7468 5f32 3d27 2f55 7365 7273 2f73 696d  th_2='/Users/sim
-00024890: 6f6e 2f44 6573 6b74 6f70 2f65 6e76 732f  on/Desktop/envs/
-000248a0: 7369 6d62 612f 7472 6f75 626c 6573 686f  simba/troublesho
-000248b0: 6f74 696e 672f 7265 7074 696c 652f 312e  oting/reptile/1.
-000248c0: 6d70 3427 2c20 6372 6f73 7366 6164 655f  mp4', crossfade_
-000248d0: 6475 7261 7469 6f6e 3d35 2c20 6372 6f73  duration=5, cros
-000248e0: 7366 6164 655f 6d65 7468 6f64 3d27 7a6f  sfade_method='zo
-000248f0: 6f6d 696e 272c 2073 6176 655f 7061 7468  omin', save_path
-00024900: 3d27 2f55 7365 7273 2f73 696d 6f6e 2f44  ='/Users/simon/D
-00024910: 6573 6b74 6f70 2f63 726f 7373 5f74 6573  esktop/cross_tes
-00024920: 742e 6d70 3427 290a 2020 2020 2222 220a  t.mp4').    """.
-00024930: 0a20 2020 2063 6865 636b 5f66 666d 7065  .    check_ffmpe
-00024940: 675f 6176 6169 6c61 626c 6528 7261 6973  g_available(rais
-00024950: 655f 6572 726f 723d 5472 7565 290a 2020  e_error=True).  
-00024960: 2020 7469 6d65 7220 3d20 5369 6d62 6154    timer = SimbaT
-00024970: 696d 6572 2873 7461 7274 3d54 7275 6529  imer(start=True)
-00024980: 0a20 2020 2076 6964 656f 5f31 5f6d 6574  .    video_1_met
-00024990: 6120 3d20 6765 745f 7669 6465 6f5f 6d65  a = get_video_me
-000249a0: 7461 5f64 6174 6128 7669 6465 6f5f 7061  ta_data(video_pa
-000249b0: 7468 3d76 6964 656f 5f70 6174 685f 3129  th=video_path_1)
-000249c0: 0a20 2020 2076 6964 656f 5f32 5f6d 6574  .    video_2_met
-000249d0: 6120 3d20 6765 745f 7669 6465 6f5f 6d65  a = get_video_me
-000249e0: 7461 5f64 6174 6128 7669 6465 6f5f 7061  ta_data(video_pa
-000249f0: 7468 3d76 6964 656f 5f70 6174 685f 3229  th=video_path_2)
-00024a00: 0a20 2020 2069 6620 7669 6465 6f5f 315f  .    if video_1_
-00024a10: 6d65 7461 5b27 7265 736f 6c75 7469 6f6e  meta['resolution
-00024a20: 5f73 7472 275d 2021 3d20 7669 6465 6f5f  _str'] != video_
-00024a30: 315f 6d65 7461 5b27 7265 736f 6c75 7469  1_meta['resoluti
-00024a40: 6f6e 5f73 7472 275d 3a0a 2020 2020 2020  on_str']:.      
-00024a50: 2020 7261 6973 6520 496e 7661 6c69 6449    raise InvalidI
-00024a60: 6e70 7574 4572 726f 7228 6d73 673d 6627  nputError(msg=f'
-00024a70: 5669 6465 6f20 3120 616e 6420 5669 6465  Video 1 and Vide
-00024a80: 6f20 3220 6e65 6564 7320 746f 2062 6520  o 2 needs to be 
-00024a90: 7468 6520 7361 6d65 2072 6573 6f6c 7574  the same resolut
-00024aa0: 696f 6e2c 2067 6f74 207b 7669 6465 6f5f  ion, got {video_
-00024ab0: 325f 6d65 7461 5b22 7265 736f 6c75 7469  2_meta["resoluti
-00024ac0: 6f6e 5f73 7472 225d 7d20 616e 6420 7b76  on_str"]} and {v
-00024ad0: 6964 656f 5f31 5f6d 6574 615b 2272 6573  ideo_1_meta["res
-00024ae0: 6f6c 7574 696f 6e5f 7374 7222 5d7d 272c  olution_str"]}',
-00024af0: 2073 6f75 7263 653d 6372 6f73 7366 6164   source=crossfad
-00024b00: 655f 7477 6f5f 7669 6465 6f73 2e5f 5f6e  e_two_videos.__n
-00024b10: 616d 655f 5f29 0a20 2020 2063 726f 7373  ame__).    cross
-00024b20: 6661 6465 5f6f 6666 7365 745f 6d65 7468  fade_offset_meth
-00024b30: 6f64 7320 3d20 6765 745f 6666 6d70 6567  ods = get_ffmpeg
-00024b40: 5f63 726f 7373 6661 6465 5f6d 6574 686f  _crossfade_metho
-00024b50: 6473 2829 0a20 2020 2063 6865 636b 5f73  ds().    check_s
-00024b60: 7472 286e 616d 653d 6627 7b63 726f 7373  tr(name=f'{cross
-00024b70: 6661 6465 5f6d 6574 686f 647d 2063 726f  fade_method} cro
-00024b80: 7373 6661 6465 5f6d 6574 686f 6427 2c20  ssfade_method', 
-00024b90: 7661 6c75 653d 6372 6f73 7366 6164 655f  value=crossfade_
-00024ba0: 6d65 7468 6f64 2c20 6f70 7469 6f6e 733d  method, options=
-00024bb0: 6372 6f73 7366 6164 655f 6f66 6673 6574  crossfade_offset
-00024bc0: 5f6d 6574 686f 6473 290a 2020 2020 6368  _methods).    ch
-00024bd0: 6563 6b5f 696e 7428 6e61 6d65 3d66 277b  eck_int(name=f'{
-00024be0: 6372 6f73 7366 6164 655f 7477 6f5f 7669  crossfade_two_vi
-00024bf0: 6465 6f73 2e5f 5f6e 616d 655f 5f7d 2063  deos.__name__} c
-00024c00: 726f 7373 6661 6465 5f64 7572 6174 696f  rossfade_duratio
-00024c10: 6e27 2c20 7661 6c75 653d 6372 6f73 7366  n', value=crossf
-00024c20: 6164 655f 6475 7261 7469 6f6e 2c20 6d69  ade_duration, mi
-00024c30: 6e5f 7661 6c75 653d 312c 206d 6178 5f76  n_value=1, max_v
-00024c40: 616c 7565 3d76 6964 656f 5f32 5f6d 6574  alue=video_2_met
-00024c50: 615b 2776 6964 656f 5f6c 656e 6774 685f  a['video_length_
-00024c60: 7327 5d29 0a20 2020 2063 6865 636b 5f69  s']).    check_i
-00024c70: 6e74 286e 616d 653d 6627 7b63 726f 7373  nt(name=f'{cross
-00024c80: 6661 6465 5f74 776f 5f76 6964 656f 732e  fade_two_videos.
-00024c90: 5f5f 6e61 6d65 5f5f 7d20 6372 6f73 7366  __name__} crossf
-00024ca0: 6164 655f 6f66 6673 6574 272c 2076 616c  ade_offset', val
-00024cb0: 7565 3d63 726f 7373 6661 6465 5f6f 6666  ue=crossfade_off
-00024cc0: 7365 742c 206d 696e 5f76 616c 7565 3d30  set, min_value=0
-00024cd0: 2c20 6d61 785f 7661 6c75 653d 7669 6465  , max_value=vide
-00024ce0: 6f5f 315f 6d65 7461 5b27 7669 6465 6f5f  o_1_meta['video_
-00024cf0: 6c65 6e67 7468 5f73 275d 290a 2020 2020  length_s']).    
-00024d00: 6469 725f 312c 2076 6964 656f 5f6e 616d  dir_1, video_nam
-00024d10: 655f 312c 2065 7874 5f31 203d 2067 6574  e_1, ext_1 = get
-00024d20: 5f66 6e5f 6578 7428 6669 6c65 7061 7468  _fn_ext(filepath
-00024d30: 3d76 6964 656f 5f70 6174 685f 3129 0a20  =video_path_1). 
-00024d40: 2020 2064 6972 5f32 2c20 7669 6465 6f5f     dir_2, video_
-00024d50: 6e61 6d65 5f32 2c20 6578 745f 3220 3d20  name_2, ext_2 = 
-00024d60: 6765 745f 666e 5f65 7874 2866 696c 6570  get_fn_ext(filep
-00024d70: 6174 683d 7669 6465 6f5f 7061 7468 5f32  ath=video_path_2
-00024d80: 290a 2020 2020 6966 2073 6176 655f 7061  ).    if save_pa
-00024d90: 7468 2069 7320 6e6f 7420 4e6f 6e65 3a0a  th is not None:.
-00024da0: 2020 2020 2020 2020 6368 6563 6b5f 6966          check_if
-00024db0: 5f64 6972 5f65 7869 7374 7328 696e 5f64  _dir_exists(in_d
-00024dc0: 6972 3d6f 732e 7061 7468 2e64 6972 6e61  ir=os.path.dirna
-00024dd0: 6d65 2873 6176 655f 7061 7468 2929 0a20  me(save_path)). 
-00024de0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00024df0: 2073 6176 655f 7061 7468 203d 206f 732e   save_path = os.
-00024e00: 7061 7468 2e6a 6f69 6e28 6469 725f 312c  path.join(dir_1,
-00024e10: 2066 277b 7669 6465 6f5f 6e61 6d65 5f31   f'{video_name_1
-00024e20: 7d5f 7b76 6964 656f 5f6e 616d 655f 327d  }_{video_name_2}
-00024e30: 5f63 726f 7373 6661 6465 7b65 7874 5f31  _crossfade{ext_1
-00024e40: 7d27 290a 2020 2020 636d 6420 3d20 6627  }').    cmd = f'
-00024e50: 6666 6d70 6567 202d 6920 227b 7669 6465  ffmpeg -i "{vide
-00024e60: 6f5f 7061 7468 5f31 7d22 202d 6920 227b  o_path_1}" -i "{
-00024e70: 7669 6465 6f5f 7061 7468 5f32 7d22 202d  video_path_2}" -
-00024e80: 6669 6c74 6572 5f63 6f6d 706c 6578 2022  filter_complex "
-00024e90: 7866 6164 653d 7472 616e 7369 7469 6f6e  xfade=transition
-00024ea0: 3d7b 6372 6f73 7366 6164 655f 6d65 7468  ={crossfade_meth
-00024eb0: 6f64 7d3a 6f66 6673 6574 3d7b 6372 6f73  od}:offset={cros
-00024ec0: 7366 6164 655f 6f66 6673 6574 7d3a 6475  sfade_offset}:du
-00024ed0: 7261 7469 6f6e 3d7b 6372 6f73 7366 6164  ration={crossfad
-00024ee0: 655f 6475 7261 7469 6f6e 7d22 2022 7b73  e_duration}" "{s
-00024ef0: 6176 655f 7061 7468 7d22 202d 6c6f 676c  ave_path}" -logl
-00024f00: 6576 656c 2065 7272 6f72 202d 7374 6174  evel error -stat
-00024f10: 7320 2d68 6964 655f 6261 6e6e 6572 202d  s -hide_banner -
-00024f20: 7927 0a20 2020 2073 7562 7072 6f63 6573  y'.    subproces
-00024f30: 732e 6361 6c6c 2863 6d64 2c20 7368 656c  s.call(cmd, shel
-00024f40: 6c3d 5472 7565 2c20 7374 646f 7574 3d73  l=True, stdout=s
-00024f50: 7562 7072 6f63 6573 732e 5049 5045 290a  ubprocess.PIPE).
-00024f60: 2020 2020 7469 6d65 722e 7374 6f70 5f74      timer.stop_t
-00024f70: 696d 6572 2829 0a20 2020 2073 7464 6f75  imer().    stdou
-00024f80: 745f 7375 6363 6573 7328 6d73 673d 6627  t_success(msg=f'
-00024f90: 4372 6f73 732d 6661 6465 6420 7669 6465  Cross-faded vide
-00024fa0: 6f20 7361 7665 6420 6174 207b 7361 7665  o saved at {save
-00024fb0: 5f70 6174 687d 272c 2065 6c61 7073 6564  _path}', elapsed
-00024fc0: 5f74 696d 653d 7469 6d65 722e 656c 6170  _time=timer.elap
-00024fd0: 7365 645f 7469 6d65 5f73 7472 290a 0a64  sed_time_str)..d
-00024fe0: 6566 2077 6174 6572 6d61 726b 5f76 6964  ef watermark_vid
-00024ff0: 656f 2876 6964 656f 5f70 6174 683a 2055  eo(video_path: U
-00025000: 6e69 6f6e 5b73 7472 2c20 6f73 2e50 6174  nion[str, os.Pat
-00025010: 684c 696b 655d 2c0a 2020 2020 2020 2020  hLike],.        
-00025020: 2020 2020 2020 2020 2020 2020 7761 7465              wate
-00025030: 726d 6172 6b5f 7061 7468 3a20 556e 696f  rmark_path: Unio
-00025040: 6e5b 7374 722c 206f 732e 5061 7468 4c69  n[str, os.PathLi
-00025050: 6b65 5d2c 0a20 2020 2020 2020 2020 2020  ke],.           
-00025060: 2020 2020 2020 2020 2070 6f73 6974 696f           positio
-00025070: 6e3a 204f 7074 696f 6e61 6c5b 4c69 7465  n: Optional[Lite
-00025080: 7261 6c5b 2774 6f70 5f6c 6566 7427 2c20  ral['top_left', 
-00025090: 2762 6f74 746f 6d5f 7269 6768 7427 2c20  'bottom_right', 
-000250a0: 2774 6f70 5f72 6967 6874 272c 2027 626f  'top_right', 'bo
-000250b0: 7474 6f6d 5f6c 6566 7427 2c20 2763 656e  ttom_left', 'cen
-000250c0: 7465 7227 5d5d 203d 2027 746f 705f 6c65  ter']] = 'top_le
-000250d0: 6674 272c 0a20 2020 2020 2020 2020 2020  ft',.           
-000250e0: 2020 2020 2020 2020 206f 7061 6369 7479           opacity
-000250f0: 3a20 4f70 7469 6f6e 616c 5b66 6c6f 6174  : Optional[float
-00025100: 5d20 3d20 302e 352c 0a20 2020 2020 2020  ] = 0.5,.       
-00025110: 2020 2020 2020 2020 2020 2020 2073 6361               sca
-00025120: 6c65 3a20 4f70 7469 6f6e 616c 5b66 6c6f  le: Optional[flo
-00025130: 6174 5d20 3d20 302e 3035 2c0a 2020 2020  at] = 0.05,.    
-00025140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025150: 7361 7665 5f64 6972 3a20 4f70 7469 6f6e  save_dir: Option
-00025160: 616c 5b55 6e69 6f6e 5b73 7472 2c20 6f73  al[Union[str, os
-00025170: 2e50 6174 684c 696b 655d 5d20 3d20 4e6f  .PathLike]] = No
-00025180: 6e65 2920 2d3e 204e 6f6e 653a 0a20 2020  ne) -> None:.   
-00025190: 2022 2222 0a20 2020 2057 6174 6572 6d61   """.    Waterma
-000251a0: 726b 2061 2076 6964 656f 2066 696c 6520  rk a video file 
-000251b0: 6f72 2061 2064 6972 6563 746f 7279 206f  or a directory o
-000251c0: 6620 7669 6465 6f20 6669 6c65 7320 7769  f video files wi
-000251d0: 7468 2073 7065 6369 6669 6564 2077 6174  th specified wat
-000251e0: 6572 6d61 726b 2073 697a 652c 206f 7061  ermark size, opa
-000251f0: 6369 7479 2c20 616e 6420 6c6f 6361 7469  city, and locati
-00025200: 6f6e 2e0a 0a20 2020 202e 2e20 7669 6465  on...    .. vide
-00025210: 6f3a 3a20 5f73 7461 7469 632f 696d 672f  o:: _static/img/
-00025220: 7761 7465 726d 6172 6b5f 7669 6465 6f2e  watermark_video.
-00025230: 7765 626d 0a20 2020 2020 2020 3a77 6964  webm.       :wid
-00025240: 7468 3a20 3930 300a 2020 2020 2020 203a  th: 900.       :
-00025250: 6c6f 6f70 3a0a 0a20 2020 203a 7061 7261  loop:..    :para
-00025260: 6d20 556e 696f 6e5b 7374 722c 206f 732e  m Union[str, os.
-00025270: 5061 7468 4c69 6b65 5d20 7669 6465 6f5f  PathLike] video_
-00025280: 7061 7468 3a20 5468 6520 7061 7468 2074  path: The path t
-00025290: 6f20 7468 6520 7669 6465 6f20 6669 6c65  o the video file
-000252a0: 2e0a 2020 2020 3a70 6172 616d 2055 6e69  ..    :param Uni
-000252b0: 6f6e 5b73 7472 2c20 6f73 2e50 6174 684c  on[str, os.PathL
-000252c0: 696b 655d 2077 6174 6572 6d61 726b 5f70  ike] watermark_p
-000252d0: 6174 683a 2054 6865 2070 6174 6820 746f  ath: The path to
-000252e0: 2074 6865 2077 6174 6572 6d61 726b 202e   the watermark .
-000252f0: 706e 6720 6669 6c65 2e0a 2020 2020 3a70  png file..    :p
-00025300: 6172 616d 204f 7074 696f 6e61 6c5b 7374  aram Optional[st
-00025310: 725d 2070 6f73 6974 696f 6e3a 2054 6865  r] position: The
-00025320: 2070 6f73 6974 696f 6e20 6f66 2074 6865   position of the
-00025330: 2077 6174 6572 6d61 726b 2e20 4f70 7469   watermark. Opti
-00025340: 6f6e 733a 2027 746f 705f 6c65 6674 272c  ons: 'top_left',
-00025350: 2027 626f 7474 6f6d 5f72 6967 6874 272c   'bottom_right',
-00025360: 2027 746f 705f 7269 6768 7427 2c20 2762   'top_right', 'b
-00025370: 6f74 746f 6d5f 6c65 6674 272c 2027 6365  ottom_left', 'ce
-00025380: 6e74 6572 270a 2020 2020 3a70 6172 616d  nter'.    :param
-00025390: 204f 7074 696f 6e61 6c5b 666c 6f61 745d   Optional[float]
-000253a0: 206f 7061 6369 7479 3a20 5468 6520 6f70   opacity: The op
-000253b0: 6163 6974 7920 6f66 2074 6865 2077 6174  acity of the wat
-000253c0: 6572 6d61 726b 2061 7320 6120 7661 6c75  ermark as a valu
-000253d0: 6520 6265 7477 6565 6e20 302d 312e 302e  e between 0-1.0.
-000253e0: 2031 2e30 206d 6561 6e69 6e67 2074 6865   1.0 meaning the
-000253f0: 2073 616d 6520 6173 2069 6e70 7574 2069   same as input i
-00025400: 6d61 6765 2e20 4465 6661 756c 743a 2030  mage. Default: 0
-00025410: 2e35 2e0a 2020 2020 3a70 6172 616d 204f  .5..    :param O
-00025420: 7074 696f 6e61 6c5b 666c 6f61 745d 2073  ptional[float] s
-00025430: 6361 6c65 3a20 5468 6520 7363 616c 6520  cale: The scale 
-00025440: 6f66 2074 6865 2077 6174 6572 6d61 726b  of the watermark
-00025450: 2061 7320 6120 7261 7469 6f20 6f73 2074   as a ratio os t
-00025460: 6865 2069 6d61 6765 2073 697a 652e 2044  he image size. D
-00025470: 6566 6175 6c74 3a20 302e 3035 2e0a 2020  efault: 0.05..  
-00025480: 2020 3a70 6172 616d 204f 7074 696f 6e61    :param Optiona
-00025490: 6c5b 556e 696f 6e5b 7374 722c 206f 732e  l[Union[str, os.
-000254a0: 5061 7468 4c69 6b65 5d5d 2073 6176 655f  PathLike]] save_
-000254b0: 6469 723a 2054 6865 206c 6f63 6174 696f  dir: The locatio
-000254c0: 6e20 7768 6572 6520 746f 2073 6176 6520  n where to save 
-000254d0: 7468 6520 7761 7465 726d 6172 6b65 6420  the watermarked 
-000254e0: 7669 6465 6f2e 2049 6620 4e6f 6e65 2c20  video. If None, 
-000254f0: 7468 656e 2073 6176 6573 2074 6865 2076  then saves the v
-00025500: 6964 656f 2069 6e20 7468 6520 7361 6d65  ideo in the same
-00025510: 2064 6972 6563 746f 7279 2061 7320 7468   directory as th
-00025520: 6520 6669 7273 7420 7669 6465 6f2e 0a20  e first video.. 
-00025530: 2020 203a 7265 7475 726e 3a20 4e6f 6e65     :return: None
-00025540: 0a0a 2020 2020 3a65 7861 6d70 6c65 3a0a  ..    :example:.
-00025550: 2020 2020 3e3e 3e20 7761 7465 726d 6172      >>> watermar
-00025560: 6b5f 7669 6465 6f28 7669 6465 6f5f 7061  k_video(video_pa
-00025570: 7468 3d27 2f55 7365 7273 2f73 696d 6f6e  th='/Users/simon
-00025580: 2f44 6573 6b74 6f70 2f65 6e76 732f 7369  /Desktop/envs/si
-00025590: 6d62 612f 7472 6f75 626c 6573 686f 6f74  mba/troubleshoot
-000255a0: 696e 672f 6d75 6c74 695f 616e 696d 616c  ing/multi_animal
-000255b0: 5f64 6c63 5f74 776f 5f63 3537 2f70 726f  _dlc_two_c57/pro
-000255c0: 6a65 6374 5f66 6f6c 6465 722f 7669 6465  ject_folder/vide
-000255d0: 6f73 2f77 6174 6572 6d61 726b 2f54 6f67  os/watermark/Tog
-000255e0: 6574 6865 725f 315f 706f 7765 7270 6f69  ether_1_powerpoi
-000255f0: 6e74 7265 6164 792e 6d70 3427 2c20 7761  ntready.mp4', wa
-00025600: 7465 726d 6172 6b5f 7061 7468 3d27 2f55  termark_path='/U
-00025610: 7365 7273 2f73 696d 6f6e 2f44 6573 6b74  sers/simon/Deskt
-00025620: 6f70 2f73 706c 6173 682e 706e 6727 2c20  op/splash.png', 
-00025630: 706f 7369 7469 6f6e 3d27 746f 705f 6c65  position='top_le
-00025640: 6674 272c 206f 7061 6369 7479 3d31 2e30  ft', opacity=1.0
-00025650: 2c20 7363 616c 653d 302e 3229 0a20 2020  , scale=0.2).   
-00025660: 2022 2222 0a20 2020 2063 6865 636b 5f66   """.    check_f
-00025670: 666d 7065 675f 6176 6169 6c61 626c 6528  fmpeg_available(
-00025680: 7261 6973 655f 6572 726f 723d 5472 7565  raise_error=True
-00025690: 290a 2020 2020 7469 6d65 7220 3d20 5369  ).    timer = Si
-000256a0: 6d62 6154 696d 6572 2873 7461 7274 3d54  mbaTimer(start=T
-000256b0: 7275 6529 0a20 2020 2050 4f53 4954 494f  rue).    POSITIO
-000256c0: 4e53 203d 205b 2774 6f70 5f6c 6566 7427  NS = ['top_left'
-000256d0: 2c20 2762 6f74 746f 6d5f 7269 6768 7427  , 'bottom_right'
-000256e0: 2c20 2774 6f70 5f72 6967 6874 272c 2027  , 'top_right', '
-000256f0: 626f 7474 6f6d 5f6c 6566 7427 2c20 2763  bottom_left', 'c
-00025700: 656e 7465 7227 5d0a 2020 2020 6368 6563  enter'].    chec
-00025710: 6b5f 666c 6f61 7428 6e61 6d65 3d66 277b  k_float(name=f'{
-00025720: 7761 7465 726d 6172 6b5f 7669 6465 6f2e  watermark_video.
-00025730: 5f5f 6e61 6d65 5f5f 7d20 6f70 6163 6974  __name__} opacit
-00025740: 7927 2c20 7661 6c75 653d 6f70 6163 6974  y', value=opacit
-00025750: 792c 206d 696e 5f76 616c 7565 3d30 2e30  y, min_value=0.0
-00025760: 3031 2c20 6d61 785f 7661 6c75 653d 312e  01, max_value=1.
-00025770: 3029 0a20 2020 2063 6865 636b 5f66 6c6f  0).    check_flo
-00025780: 6174 286e 616d 653d 6627 7b77 6174 6572  at(name=f'{water
-00025790: 6d61 726b 5f76 6964 656f 2e5f 5f6e 616d  mark_video.__nam
-000257a0: 655f 5f7d 2073 6361 6c65 272c 2076 616c  e__} scale', val
-000257b0: 7565 3d73 6361 6c65 2c20 6d69 6e5f 7661  ue=scale, min_va
-000257c0: 6c75 653d 302e 3030 312c 206d 6178 5f76  lue=0.001, max_v
-000257d0: 616c 7565 3d30 2e39 3939 290a 2020 2020  alue=0.999).    
-000257e0: 6368 6563 6b5f 7374 7228 6e61 6d65 3d66  check_str(name=f
-000257f0: 277b 7761 7465 726d 6172 6b5f 7669 6465  '{watermark_vide
-00025800: 6f2e 5f5f 6e61 6d65 5f5f 7d20 706f 7369  o.__name__} posi
-00025810: 7469 6f6e 272c 2076 616c 7565 3d70 6f73  tion', value=pos
-00025820: 6974 696f 6e2c 206f 7074 696f 6e73 3d50  ition, options=P
-00025830: 4f53 4954 494f 4e53 290a 2020 2020 6368  OSITIONS).    ch
-00025840: 6563 6b5f 6669 6c65 5f65 7869 7374 5f61  eck_file_exist_a
-00025850: 6e64 5f72 6561 6461 626c 6528 6669 6c65  nd_readable(file
-00025860: 5f70 6174 683d 7761 7465 726d 6172 6b5f  _path=watermark_
-00025870: 7061 7468 290a 0a20 2020 2069 6620 6f73  path)..    if os
-00025880: 2e70 6174 682e 6973 6669 6c65 2876 6964  .path.isfile(vid
-00025890: 656f 5f70 6174 6829 3a0a 2020 2020 2020  eo_path):.      
-000258a0: 2020 7669 6465 6f5f 7061 7468 7320 3d20    video_paths = 
-000258b0: 5b76 6964 656f 5f70 6174 685d 0a20 2020  [video_path].   
-000258c0: 2065 6c69 6620 6f73 2e70 6174 682e 6973   elif os.path.is
-000258d0: 6469 7228 7669 6465 6f5f 7061 7468 293a  dir(video_path):
-000258e0: 0a20 2020 2020 2020 2076 6964 656f 5f70  .        video_p
-000258f0: 6174 6873 203d 206c 6973 7428 6669 6e64  aths = list(find
-00025900: 5f61 6c6c 5f76 6964 656f 735f 696e 5f64  _all_videos_in_d
-00025910: 6972 6563 746f 7279 2864 6972 6563 746f  irectory(directo
-00025920: 7279 3d76 6964 656f 5f70 6174 682c 2061  ry=video_path, a
-00025930: 735f 6469 6374 3d54 7275 652c 2072 6169  s_dict=True, rai
-00025940: 7365 5f65 7272 6f72 3d54 7275 6529 2e76  se_error=True).v
-00025950: 616c 7565 7328 2929 0a20 2020 2065 6c73  alues()).    els
-00025960: 653a 0a20 2020 2020 2020 2072 6169 7365  e:.        raise
-00025970: 2049 6e76 616c 6964 496e 7075 7445 7272   InvalidInputErr
-00025980: 6f72 286d 7367 3d66 277b 7669 6465 6f5f  or(msg=f'{video_
-00025990: 7061 7468 7d20 6973 206e 6f74 2061 2076  path} is not a v
-000259a0: 616c 6964 2066 696c 6520 7061 7468 206f  alid file path o
-000259b0: 7220 6120 7661 6c69 6420 6469 7265 6374  r a valid direct
-000259c0: 6f72 7920 7061 7468 272c 2073 6f75 7263  ory path', sourc
-000259d0: 653d 7761 7465 726d 6172 6b5f 7669 6465  e=watermark_vide
-000259e0: 6f2e 5f5f 6e61 6d65 5f5f 290a 2020 2020  o.__name__).    
-000259f0: 6966 2073 6176 655f 6469 7220 6973 206e  if save_dir is n
-00025a00: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00025a10: 2063 6865 636b 5f69 665f 6469 725f 6578   check_if_dir_ex
-00025a20: 6973 7473 2869 6e5f 6469 723d 7361 7665  ists(in_dir=save
-00025a30: 5f64 6972 290a 2020 2020 656c 7365 3a0a  _dir).    else:.
-00025a40: 2020 2020 2020 2020 7361 7665 5f64 6972          save_dir
-00025a50: 203d 206f 732e 7061 7468 2e64 6972 6e61   = os.path.dirna
-00025a60: 6d65 2876 6964 656f 5f70 6174 6873 5b30  me(video_paths[0
-00025a70: 5d29 0a20 2020 2066 6f72 2066 696c 655f  ]).    for file_
-00025a80: 636e 742c 2076 6964 656f 5f70 6174 6820  cnt, video_path 
-00025a90: 696e 2065 6e75 6d65 7261 7465 2876 6964  in enumerate(vid
-00025aa0: 656f 5f70 6174 6873 293a 0a20 2020 2020  eo_paths):.     
-00025ab0: 2020 205f 2c20 7669 6465 6f5f 6e61 6d65     _, video_name
-00025ac0: 2c20 7669 6465 6f5f 6578 7420 3d20 6765  , video_ext = ge
-00025ad0: 745f 666e 5f65 7874 2876 6964 656f 5f70  t_fn_ext(video_p
-00025ae0: 6174 6829 0a20 2020 2020 2020 205f 203d  ath).        _ =
-00025af0: 2067 6574 5f76 6964 656f 5f6d 6574 615f   get_video_meta_
-00025b00: 6461 7461 2876 6964 656f 5f70 6174 683d  data(video_path=
-00025b10: 7669 6465 6f5f 7061 7468 290a 2020 2020  video_path).    
-00025b20: 2020 2020 7072 696e 7428 6627 5761 7465      print(f'Wate
-00025b30: 726d 6172 6b69 6e67 207b 7669 6465 6f5f  rmarking {video_
-00025b40: 6e61 6d65 7d20 2856 6964 656f 207b 6669  name} (Video {fi
-00025b50: 6c65 5f63 6e74 2b31 7d2f 7b6c 656e 2876  le_cnt+1}/{len(v
-00025b60: 6964 656f 5f70 6174 6873 297d 292e 2e2e  ideo_paths)})...
-00025b70: 2729 0a20 2020 2020 2020 206f 7574 5f70  ').        out_p
-00025b80: 6174 6820 3d20 6f73 2e70 6174 682e 6a6f  ath = os.path.jo
-00025b90: 696e 2873 6176 655f 6469 722c 2066 277b  in(save_dir, f'{
-00025ba0: 7669 6465 6f5f 6e61 6d65 7d5f 7761 7465  video_name}_wate
-00025bb0: 726d 6172 6b65 647b 7669 6465 6f5f 6578  rmarked{video_ex
-00025bc0: 747d 2729 0a20 2020 2020 2020 2069 6620  t}').        if 
-00025bd0: 706f 7369 7469 6f6e 203d 3d20 504f 5349  position == POSI
-00025be0: 5449 4f4e 535b 305d 3a0a 2020 2020 2020  TIONS[0]:.      
-00025bf0: 2020 2020 2020 636d 6420 3d20 6627 6666        cmd = f'ff
-00025c00: 6d70 6567 202d 6920 227b 7669 6465 6f5f  mpeg -i "{video_
-00025c10: 7061 7468 7d22 202d 6920 227b 7761 7465  path}" -i "{wate
-00025c20: 726d 6172 6b5f 7061 7468 7d22 202d 6669  rmark_path}" -fi
-00025c30: 6c74 6572 5f63 6f6d 706c 6578 2022 5b31  lter_complex "[1
-00025c40: 3a76 5d73 6361 6c65 3d69 772a 7b73 6361  :v]scale=iw*{sca
-00025c50: 6c65 7d3a 2d31 2c66 6f72 6d61 743d 7267  le}:-1,format=rg
-00025c60: 6261 2c63 6f6c 6f72 6368 616e 6e65 6c6d  ba,colorchannelm
-00025c70: 6978 6572 3d61 613d 7b6f 7061 6369 7479  ixer=aa={opacity
-00025c80: 7d5b 776d 5d3b 5b30 3a76 5d5b 776d 5d6f  }[wm];[0:v][wm]o
-00025c90: 7665 726c 6179 3d30 3a30 2220 227b 6f75  verlay=0:0" "{ou
-00025ca0: 745f 7061 7468 7d22 202d 6c6f 676c 6576  t_path}" -loglev
-00025cb0: 656c 2065 7272 6f72 202d 7374 6174 7320  el error -stats 
-00025cc0: 2d68 6964 655f 6261 6e6e 6572 202d 7927  -hide_banner -y'
-00025cd0: 0a20 2020 2020 2020 2065 6c69 6620 706f  .        elif po
-00025ce0: 7369 7469 6f6e 203d 3d20 504f 5349 5449  sition == POSITI
-00025cf0: 4f4e 535b 315d 3a0a 2020 2020 2020 2020  ONS[1]:.        
-00025d00: 2020 2020 636d 6420 3d20 6627 6666 6d70      cmd = f'ffmp
-00025d10: 6567 202d 6920 227b 7669 6465 6f5f 7061  eg -i "{video_pa
-00025d20: 7468 7d22 202d 6920 227b 7761 7465 726d  th}" -i "{waterm
-00025d30: 6172 6b5f 7061 7468 7d22 202d 6669 6c74  ark_path}" -filt
-00025d40: 6572 5f63 6f6d 706c 6578 2022 5b31 3a76  er_complex "[1:v
-00025d50: 5d73 6361 6c65 3d69 772a 7b73 6361 6c65  ]scale=iw*{scale
-00025d60: 7d3a 2d31 2c66 6f72 6d61 743d 7267 6261  }:-1,format=rgba
-00025d70: 2c63 6f6c 6f72 6368 616e 6e65 6c6d 6978  ,colorchannelmix
-00025d80: 6572 3d61 613d 7b6f 7061 6369 7479 7d5b  er=aa={opacity}[
-00025d90: 776d 5d3b 5b30 3a76 5d5b 776d 5d6f 7665  wm];[0:v][wm]ove
-00025da0: 726c 6179 3d57 2d77 3a48 2d68 2220 227b  rlay=W-w:H-h" "{
-00025db0: 6f75 745f 7061 7468 7d22 202d 6c6f 676c  out_path}" -logl
-00025dc0: 6576 656c 2065 7272 6f72 202d 7374 6174  evel error -stat
-00025dd0: 7320 2d68 6964 655f 6261 6e6e 6572 202d  s -hide_banner -
-00025de0: 7927 0a20 2020 2020 2020 2065 6c69 6620  y'.        elif 
-00025df0: 706f 7369 7469 6f6e 203d 3d20 504f 5349  position == POSI
-00025e00: 5449 4f4e 535b 325d 3a0a 2020 2020 2020  TIONS[2]:.      
-00025e10: 2020 2020 2020 636d 6420 3d20 6627 6666        cmd = f'ff
-00025e20: 6d70 6567 202d 6920 227b 7669 6465 6f5f  mpeg -i "{video_
-00025e30: 7061 7468 7d22 202d 6920 227b 7761 7465  path}" -i "{wate
-00025e40: 726d 6172 6b5f 7061 7468 7d22 202d 6669  rmark_path}" -fi
-00025e50: 6c74 6572 5f63 6f6d 706c 6578 2022 5b31  lter_complex "[1
-00025e60: 3a76 5d73 6361 6c65 3d69 772a 7b73 6361  :v]scale=iw*{sca
-00025e70: 6c65 7d3a 2d31 2c66 6f72 6d61 743d 7267  le}:-1,format=rg
-00025e80: 6261 2c63 6f6c 6f72 6368 616e 6e65 6c6d  ba,colorchannelm
-00025e90: 6978 6572 3d61 613d 7b6f 7061 6369 7479  ixer=aa={opacity
-00025ea0: 7d5b 776d 5d3b 5b30 3a76 5d5b 776d 5d6f  }[wm];[0:v][wm]o
-00025eb0: 7665 726c 6179 3d57 2d77 2d30 3a30 2220  verlay=W-w-0:0" 
-00025ec0: 227b 6f75 745f 7061 7468 7d22 202d 6c6f  "{out_path}" -lo
-00025ed0: 676c 6576 656c 2065 7272 6f72 202d 7374  glevel error -st
-00025ee0: 6174 7320 2d68 6964 655f 6261 6e6e 6572  ats -hide_banner
-00025ef0: 202d 7927 0a20 2020 2020 2020 2065 6c69   -y'.        eli
-00025f00: 6620 706f 7369 7469 6f6e 203d 3d20 504f  f position == PO
-00025f10: 5349 5449 4f4e 535b 335d 3a0a 2020 2020  SITIONS[3]:.    
-00025f20: 2020 2020 2020 2020 636d 6420 3d20 6627          cmd = f'
-00025f30: 6666 6d70 6567 202d 6920 227b 7669 6465  ffmpeg -i "{vide
-00025f40: 6f5f 7061 7468 7d22 202d 6920 227b 7761  o_path}" -i "{wa
-00025f50: 7465 726d 6172 6b5f 7061 7468 7d22 202d  termark_path}" -
-00025f60: 6669 6c74 6572 5f63 6f6d 706c 6578 2022  filter_complex "
-00025f70: 5b31 3a76 5d73 6361 6c65 3d69 772a 7b73  [1:v]scale=iw*{s
-00025f80: 6361 6c65 7d3a 2d31 2c66 6f72 6d61 743d  cale}:-1,format=
-00025f90: 7267 6261 2c63 6f6c 6f72 6368 616e 6e65  rgba,colorchanne
-00025fa0: 6c6d 6978 6572 3d61 613d 7b6f 7061 6369  lmixer=aa={opaci
-00025fb0: 7479 7d5b 776d 5d3b 5b30 3a76 5d5b 776d  ty}[wm];[0:v][wm
-00025fc0: 5d6f 7665 726c 6179 3d30 3a48 2d68 2d30  ]overlay=0:H-h-0
-00025fd0: 2220 227b 6f75 745f 7061 7468 7d22 202d  " "{out_path}" -
-00025fe0: 6c6f 676c 6576 656c 2065 7272 6f72 202d  loglevel error -
-00025ff0: 7374 6174 7320 2d68 6964 655f 6261 6e6e  stats -hide_bann
-00026000: 6572 202d 7927 0a20 2020 2020 2020 2065  er -y'.        e
-00026010: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00026020: 2063 6d64 203d 2066 2766 666d 7065 6720   cmd = f'ffmpeg 
-00026030: 2d69 2022 7b76 6964 656f 5f70 6174 687d  -i "{video_path}
-00026040: 2220 2d69 2022 7b77 6174 6572 6d61 726b  " -i "{watermark
-00026050: 5f70 6174 687d 2220 2d66 696c 7465 725f  _path}" -filter_
-00026060: 636f 6d70 6c65 7820 225b 313a 765d 7363  complex "[1:v]sc
-00026070: 616c 653d 6977 2a7b 7363 616c 657d 3a2d  ale=iw*{scale}:-
-00026080: 312c 666f 726d 6174 3d72 6762 612c 636f  1,format=rgba,co
-00026090: 6c6f 7263 6861 6e6e 656c 6d69 7865 723d  lorchannelmixer=
-000260a0: 6161 3d7b 6f70 6163 6974 797d 5b77 6d5d  aa={opacity}[wm]
-000260b0: 3b5b 303a 765d 5b77 6d5d 6f76 6572 6c61  ;[0:v][wm]overla
-000260c0: 793d 2857 2d77 292f 323a 2848 2d68 292f  y=(W-w)/2:(H-h)/
-000260d0: 3222 2022 7b6f 7574 5f70 6174 687d 2220  2" "{out_path}" 
-000260e0: 2d6c 6f67 6c65 7665 6c20 6572 726f 7220  -loglevel error 
-000260f0: 2d73 7461 7473 202d 6869 6465 5f62 616e  -stats -hide_ban
-00026100: 6e65 7220 2d79 270a 2020 2020 2020 2020  ner -y'.        
-00026110: 7375 6270 726f 6365 7373 2e63 616c 6c28  subprocess.call(
-00026120: 636d 642c 2073 6865 6c6c 3d54 7275 652c  cmd, shell=True,
-00026130: 2073 7464 6f75 743d 7375 6270 726f 6365   stdout=subproce
-00026140: 7373 2e50 4950 4529 0a20 2020 2074 696d  ss.PIPE).    tim
-00026150: 6572 2e73 746f 705f 7469 6d65 7228 290a  er.stop_timer().
-00026160: 2020 2020 7374 646f 7574 5f73 7563 6365      stdout_succe
-00026170: 7373 286d 7367 3d66 277b 6c65 6e28 7669  ss(msg=f'{len(vi
-00026180: 6465 6f5f 7061 7468 7329 7d20 7761 7465  deo_paths)} wate
-00026190: 726d 6172 6b65 6420 7669 6465 6f28 7329  rmarked video(s)
-000261a0: 2073 6176 6564 2069 6e20 7b73 6176 655f   saved in {save_
-000261b0: 6469 727d 272c 2065 6c61 7073 6564 5f74  dir}', elapsed_t
-000261c0: 696d 653d 7469 6d65 722e 656c 6170 7365  ime=timer.elapse
-000261d0: 645f 7469 6d65 5f73 7472 290a 0a64 6566  d_time_str)..def
-000261e0: 2069 6e73 6574 5f6f 7665 726c 6179 5f76   inset_overlay_v
-000261f0: 6964 656f 2876 6964 656f 5f70 6174 683a  ideo(video_path:
-00026200: 2055 6e69 6f6e 5b73 7472 2c20 6f73 2e50   Union[str, os.P
-00026210: 6174 684c 696b 655d 2c0a 2020 2020 2020  athLike],.      
-00026220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026230: 2020 6f76 6572 6c61 795f 7669 6465 6f5f    overlay_video_
-00026240: 7061 7468 3a20 556e 696f 6e5b 7374 722c  path: Union[str,
-00026250: 206f 732e 5061 7468 4c69 6b65 5d2c 0a20   os.PathLike],. 
-00026260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026270: 2020 2020 2020 2070 6f73 6974 696f 6e3a         position:
-00026280: 204f 7074 696f 6e61 6c5b 4c69 7465 7261   Optional[Litera
-00026290: 6c5b 2774 6f70 5f6c 6566 7427 2c20 2762  l['top_left', 'b
-000262a0: 6f74 746f 6d5f 7269 6768 7427 2c20 2774  ottom_right', 't
-000262b0: 6f70 5f72 6967 6874 272c 2027 626f 7474  op_right', 'bott
-000262c0: 6f6d 5f6c 6566 7427 2c20 2763 656e 7465  om_left', 'cente
-000262d0: 7227 5d5d 203d 2027 746f 705f 6c65 6674  r']] = 'top_left
-000262e0: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
-000262f0: 2020 2020 2020 2020 2020 206f 7061 6369             opaci
-00026300: 7479 3a20 4f70 7469 6f6e 616c 5b66 6c6f  ty: Optional[flo
-00026310: 6174 5d20 3d20 302e 352c 0a20 2020 2020  at] = 0.5,.     
+00023670: 2020 2020 2020 2020 2020 2020 2073 6176               sav
+00023680: 655f 6469 723a 204f 7074 696f 6e61 6c5b  e_dir: Optional[
+00023690: 556e 696f 6e5b 7374 722c 206f 732e 5061  Union[str, os.Pa
+000236a0: 7468 4c69 6b65 5d5d 203d 204e 6f6e 6529  thLike]] = None)
+000236b0: 202d 3e20 4e6f 6e65 3a0a 0a20 2020 2022   -> None:..    "
+000236c0: 2222 0a20 2020 204f 7665 726c 6179 2061  "".    Overlay a
+000236d0: 2070 726f 6772 6573 7320 6261 7220 6f6e   progress bar on
+000236e0: 2061 2064 6972 6563 746f 7279 206f 6620   a directory of 
+000236f0: 7669 6465 6f73 206f 7220 6120 7369 6e67  videos or a sing
+00023700: 6c65 2076 6964 656f 2e0a 0a20 2020 202e  le video...    .
+00023710: 2e20 7669 6465 6f3a 3a20 5f73 7461 7469  . video:: _stati
+00023720: 632f 696d 672f 6f76 6572 6c61 795f 7669  c/img/overlay_vi
+00023730: 6465 6f5f 7072 6f67 7265 7373 6261 722e  deo_progressbar.
+00023740: 7765 626d 0a20 2020 2020 2020 3a77 6964  webm.       :wid
+00023750: 7468 3a20 3730 300a 2020 2020 2020 203a  th: 700.       :
+00023760: 6c6f 6f70 3a0a 0a20 2020 203a 7061 7261  loop:..    :para
+00023770: 6d20 556e 696f 6e5b 7374 722c 206f 732e  m Union[str, os.
+00023780: 5061 7468 4c69 6b65 5d20 7669 6465 6f5f  PathLike] video_
+00023790: 7061 7468 3a20 4469 7265 6374 6f72 7920  path: Directory 
+000237a0: 636f 6e74 6169 6e69 6e67 2076 6964 656f  containing video
+000237b0: 2066 696c 6573 206f 7220 6120 7369 6e67   files or a sing
+000237c0: 6c65 2076 6964 656f 2066 696c 650a 2020  le video file.  
+000237d0: 2020 3a70 6172 616d 204f 7074 696f 6e61    :param Optiona
+000237e0: 6c5b 696e 745d 2062 6172 5f68 6569 6768  l[int] bar_heigh
+000237f0: 743a 2054 6865 2068 6569 6768 7420 6f66  t: The height of
+00023800: 2074 6865 2070 726f 6772 6573 7362 6172   the progressbar
+00023810: 2069 6e20 7065 7263 656e 7420 6f66 2074   in percent of t
+00023820: 6865 2076 6964 656f 2068 6569 6768 742e  he video height.
+00023830: 0a20 2020 203a 7061 7261 6d20 4f70 7469  .    :param Opti
+00023840: 6f6e 616c 5b73 7472 5d20 636f 6c6f 723a  onal[str] color:
+00023850: 2054 6865 2063 6f6c 6f72 206f 6620 7468   The color of th
+00023860: 6520 7072 6f67 7265 7373 2062 6172 2e20  e progress bar. 
+00023870: 5365 6520 7369 6d62 612e 7574 696c 732e  See simba.utils.
+00023880: 6c6f 6f6b 7570 732e 6765 745f 636f 6c6f  lookups.get_colo
+00023890: 725f 6469 6374 206b 6579 7320 666f 7220  r_dict keys for 
+000238a0: 6163 6365 7074 6564 206e 616d 6573 2e0a  accepted names..
+000238b0: 2020 2020 3a70 6172 616d 204f 7074 696f      :param Optio
+000238c0: 6e61 6c5b 7374 725d 2070 6f73 6974 696f  nal[str] positio
+000238d0: 6e3a 2054 6865 2070 6f73 6974 696f 6e20  n: The position 
+000238e0: 6f66 2074 6865 2070 726f 6772 6573 7362  of the progressb
+000238f0: 6172 2e20 4f70 7469 6f6e 733a 2027 746f  ar. Options: 'to
+00023900: 7027 2c20 2762 6f74 746f 6d27 2e0a 2020  p', 'bottom'..  
+00023910: 2020 3a70 6172 616d 204f 7074 696f 6e61    :param Optiona
+00023920: 6c5b 556e 696f 6e5b 7374 722c 206f 732e  l[Union[str, os.
+00023930: 5061 7468 4c69 6b65 5d5d 2073 6176 655f  PathLike]] save_
+00023940: 6469 723a 2049 6620 6e6f 7420 4e6f 6e65  dir: If not None
+00023950: 2c20 7468 656e 2073 6176 6573 2074 6865  , then saves the
+00023960: 2076 6964 656f 7320 696e 2074 6865 2070   videos in the p
+00023970: 6173 7365 6420 6469 7265 6374 6f72 792e  assed directory.
+00023980: 2045 6c73 652c 2069 6e20 7468 6520 7361   Else, in the sa
+00023990: 6d65 2064 6972 6563 7472 7920 7769 7468  me directry with
+000239a0: 2074 6865 2060 605f 7072 6f67 7265 7373   the ``_progress
+000239b0: 5f62 6172 6060 2073 7566 6669 782e 0a20  _bar`` suffix.. 
+000239c0: 2020 203a 7265 7475 726e 3a20 4e6f 6e65     :return: None
+000239d0: 2e0a 2020 2020 2222 220a 0a20 2020 2063  ..    """..    c
+000239e0: 6865 636b 5f66 666d 7065 675f 6176 6169  heck_ffmpeg_avai
+000239f0: 6c61 626c 6528 7261 6973 655f 6572 726f  lable(raise_erro
+00023a00: 723d 5472 7565 290a 2020 2020 7469 6d65  r=True).    time
+00023a10: 7220 3d20 5369 6d62 6154 696d 6572 2873  r = SimbaTimer(s
+00023a20: 7461 7274 3d54 7275 6529 0a20 2020 2063  tart=True).    c
+00023a30: 6f6c 6f72 203d 2027 272e 6a6f 696e 2866  olor = ''.join(f
+00023a40: 696c 7465 7228 7374 722e 6973 616c 6e75  ilter(str.isalnu
+00023a50: 6d2c 2063 6f6c 6f72 2929 2e6c 6f77 6572  m, color)).lower
+00023a60: 2829 0a20 2020 2069 6620 6f73 2e70 6174  ().    if os.pat
+00023a70: 682e 6973 6669 6c65 2876 6964 656f 5f70  h.isfile(video_p
+00023a80: 6174 6829 3a0a 2020 2020 2020 2020 6368  ath):.        ch
+00023a90: 6563 6b5f 6669 6c65 5f65 7869 7374 5f61  eck_file_exist_a
+00023aa0: 6e64 5f72 6561 6461 626c 6528 6669 6c65  nd_readable(file
+00023ab0: 5f70 6174 683d 7669 6465 6f5f 7061 7468  _path=video_path
+00023ac0: 290a 2020 2020 2020 2020 7669 6465 6f5f  ).        video_
+00023ad0: 7061 7468 7320 3d20 5b76 6964 656f 5f70  paths = [video_p
+00023ae0: 6174 685d 0a20 2020 2065 6c69 6620 6f73  ath].    elif os
+00023af0: 2e70 6174 682e 6973 6469 7228 7669 6465  .path.isdir(vide
+00023b00: 6f5f 7061 7468 293a 0a20 2020 2020 2020  o_path):.       
+00023b10: 2076 6964 656f 5f70 6174 6820 3d20 6669   video_path = fi
+00023b20: 6e64 5f61 6c6c 5f76 6964 656f 735f 696e  nd_all_videos_in
+00023b30: 5f64 6972 6563 746f 7279 2864 6972 6563  _directory(direc
+00023b40: 746f 7279 3d76 6964 656f 5f70 6174 682c  tory=video_path,
+00023b50: 2061 735f 6469 6374 3d54 7275 652c 2072   as_dict=True, r
+00023b60: 6169 7365 5f65 7272 6f72 3d54 7275 6529  aise_error=True)
+00023b70: 0a20 2020 2020 2020 2076 6964 656f 5f70  .        video_p
+00023b80: 6174 6873 203d 206c 6973 7428 7669 6465  aths = list(vide
+00023b90: 6f5f 7061 7468 2e76 616c 7565 7328 2929  o_path.values())
+00023ba0: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
+00023bb0: 2020 2072 6169 7365 2049 6e76 616c 6964     raise Invalid
+00023bc0: 496e 7075 7445 7272 6f72 286d 7367 3d27  InputError(msg='
+00023bd0: 7b7d 2069 7320 6e6f 7420 6120 7661 6c69  {} is not a vali
+00023be0: 6420 6669 6c65 2070 6174 6820 6f72 2064  d file path or d
+00023bf0: 6972 6563 746f 7279 2070 6174 682e 272c  irectory path.',
+00023c00: 2073 6f75 7263 653d 7375 7065 7269 6d70   source=superimp
+00023c10: 6f73 655f 7669 6465 6f5f 7072 6f67 7265  ose_video_progre
+00023c20: 7373 6261 722e 5f5f 6e61 6d65 5f5f 290a  ssbar.__name__).
+00023c30: 2020 2020 6966 2073 6176 655f 6469 7220      if save_dir 
+00023c40: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00023c50: 2020 2020 2063 6865 636b 5f69 665f 6469       check_if_di
+00023c60: 725f 6578 6973 7473 2869 6e5f 6469 723d  r_exists(in_dir=
+00023c70: 7361 7665 5f64 6972 290a 2020 2020 656c  save_dir).    el
+00023c80: 7365 3a0a 2020 2020 2020 2020 7361 7665  se:.        save
+00023c90: 5f64 6972 2c20 5f2c 205f 203d 2067 6574  _dir, _, _ = get
+00023ca0: 5f66 6e5f 6578 7428 6669 6c65 7061 7468  _fn_ext(filepath
+00023cb0: 3d76 6964 656f 5f70 6174 6873 5b30 5d29  =video_paths[0])
+00023cc0: 0a20 2020 2066 6f72 2063 6e74 2c20 7669  .    for cnt, vi
+00023cd0: 6465 6f5f 7061 7468 2069 6e20 656e 756d  deo_path in enum
+00023ce0: 6572 6174 6528 7669 6465 6f5f 7061 7468  erate(video_path
+00023cf0: 7329 3a0a 2020 2020 2020 2020 7669 6465  s):.        vide
+00023d00: 6f5f 6d65 7461 5f64 6174 6120 3d20 6765  o_meta_data = ge
+00023d10: 745f 7669 6465 6f5f 6d65 7461 5f64 6174  t_video_meta_dat
+00023d20: 6128 7669 6465 6f5f 7061 7468 3d76 6964  a(video_path=vid
+00023d30: 656f 5f70 6174 6829 0a20 2020 2020 2020  eo_path).       
+00023d40: 2076 6964 656f 5f6c 656e 6774 6820 3d20   video_length = 
+00023d50: 7669 6465 6f5f 6d65 7461 5f64 6174 615b  video_meta_data[
+00023d60: 2776 6964 656f 5f6c 656e 6774 685f 7327  'video_length_s'
+00023d70: 5d0a 2020 2020 2020 2020 7769 6474 682c  ].        width,
+00023d80: 2068 6569 6768 7420 3d20 7669 6465 6f5f   height = video_
+00023d90: 6d65 7461 5f64 6174 615b 2777 6964 7468  meta_data['width
+00023da0: 275d 2c20 7669 6465 6f5f 6d65 7461 5f64  '], video_meta_d
+00023db0: 6174 615b 2768 6569 6768 7427 5d0a 2020  ata['height'].  
+00023dc0: 2020 2020 2020 6261 725f 6865 6967 6874        bar_height
+00023dd0: 203d 2069 6e74 2868 6569 6768 7420 2a20   = int(height * 
+00023de0: 2862 6172 5f68 6569 6768 742f 3130 3029  (bar_height/100)
+00023df0: 290a 2020 2020 2020 2020 5f2c 2076 6964  ).        _, vid
+00023e00: 656f 5f6e 616d 652c 2065 7874 203d 2067  eo_name, ext = g
+00023e10: 6574 5f66 6e5f 6578 7428 6669 6c65 7061  et_fn_ext(filepa
+00023e20: 7468 3d76 6964 656f 5f70 6174 6829 0a20  th=video_path). 
+00023e30: 2020 2020 2020 2070 7269 6e74 2866 2749         print(f'I
+00023e40: 6e73 6572 7469 6e67 2070 726f 6772 6573  nserting progres
+00023e50: 7320 6261 7220 6f6e 2076 6964 656f 207b  s bar on video {
+00023e60: 7669 6465 6f5f 6e61 6d65 7d2e 2e2e 2729  video_name}...')
+00023e70: 0a20 2020 2020 2020 2073 6176 655f 7061  .        save_pa
+00023e80: 7468 203d 206f 732e 7061 7468 2e6a 6f69  th = os.path.joi
+00023e90: 6e28 7361 7665 5f64 6972 2c20 6627 7b76  n(save_dir, f'{v
+00023ea0: 6964 656f 5f6e 616d 657d 5f70 726f 6772  ideo_name}_progr
+00023eb0: 6573 735f 6261 727b 6578 747d 2729 0a20  ess_bar{ext}'). 
+00023ec0: 2020 2020 2020 2063 6865 636b 5f69 6e74         check_int
+00023ed0: 286e 616d 653d 6627 7b73 7570 6572 696d  (name=f'{superim
+00023ee0: 706f 7365 5f76 6964 656f 5f70 726f 6772  pose_video_progr
+00023ef0: 6573 7362 6172 7d20 6865 6967 6874 272c  essbar} height',
+00023f00: 2076 616c 7565 3d62 6172 5f68 6569 6768   value=bar_heigh
+00023f10: 742c 206d 6178 5f76 616c 7565 3d68 6569  t, max_value=hei
+00023f20: 6768 742c 206d 696e 5f76 616c 7565 3d31  ght, min_value=1
+00023f30: 290a 2020 2020 2020 2020 6966 2070 6f73  ).        if pos
+00023f40: 6974 696f 6e20 3d3d 2027 626f 7474 6f6d  ition == 'bottom
+00023f50: 273a 0a20 2020 2020 2020 2020 2020 2063  ':.            c
+00023f60: 6d64 203d 2066 2766 666d 7065 6720 2d69  md = f'ffmpeg -i
+00023f70: 2022 7b76 6964 656f 5f70 6174 687d 2220   "{video_path}" 
+00023f80: 2d66 696c 7465 725f 636f 6d70 6c65 7820  -filter_complex 
+00023f90: 2263 6f6c 6f72 3d63 3d7b 636f 6c6f 727d  "color=c={color}
+00023fa0: 3a73 3d7b 7769 6474 687d 787b 6261 725f  :s={width}x{bar_
+00023fb0: 6865 6967 6874 7d5b 6261 725d 3b5b 305d  height}[bar];[0]
+00023fc0: 5b62 6172 5d6f 7665 726c 6179 3d2d 772b  [bar]overlay=-w+
+00023fd0: 2877 2f7b 7669 6465 6f5f 6c65 6e67 7468  (w/{video_length
+00023fe0: 7d29 2a74 3a48 2d68 3a73 686f 7274 6573  })*t:H-h:shortes
+00023ff0: 743d 3122 202d 633a 6120 636f 7079 2022  t=1" -c:a copy "
+00024000: 7b73 6176 655f 7061 7468 7d22 202d 6c6f  {save_path}" -lo
+00024010: 676c 6576 656c 2065 7272 6f72 202d 7374  glevel error -st
+00024020: 6174 7320 2d68 6964 655f 6261 6e6e 6572  ats -hide_banner
+00024030: 202d 7927 0a20 2020 2020 2020 2065 6c73   -y'.        els
+00024040: 653a 0a20 2020 2020 2020 2020 2020 2063  e:.            c
+00024050: 6d64 203d 2066 2766 666d 7065 6720 2d69  md = f'ffmpeg -i
+00024060: 2022 7b76 6964 656f 5f70 6174 687d 2220   "{video_path}" 
+00024070: 2d66 696c 7465 725f 636f 6d70 6c65 7820  -filter_complex 
+00024080: 2263 6f6c 6f72 3d63 3d7b 636f 6c6f 727d  "color=c={color}
+00024090: 3a73 3d7b 7769 6474 687d 787b 6261 725f  :s={width}x{bar_
+000240a0: 6865 6967 6874 7d5b 6261 725d 3b5b 305d  height}[bar];[0]
+000240b0: 5b62 6172 5d6f 7665 726c 6179 3d2d 772b  [bar]overlay=-w+
+000240c0: 2877 2f7b 7669 6465 6f5f 6c65 6e67 7468  (w/{video_length
+000240d0: 7d29 2a74 3a7b 6261 725f 6865 6967 6874  })*t:{bar_height
+000240e0: 7d2d 683a 7368 6f72 7465 7374 3d31 2220  }-h:shortest=1" 
+000240f0: 2d63 3a61 2063 6f70 7920 227b 7361 7665  -c:a copy "{save
+00024100: 5f70 6174 687d 2220 2d6c 6f67 6c65 7665  _path}" -logleve
+00024110: 6c20 6572 726f 7220 2d73 7461 7473 202d  l error -stats -
+00024120: 6869 6465 5f62 616e 6e65 7220 2d79 270a  hide_banner -y'.
+00024130: 2020 2020 2020 2020 7375 6270 726f 6365          subproce
+00024140: 7373 2e63 616c 6c28 636d 642c 2073 6865  ss.call(cmd, she
+00024150: 6c6c 3d54 7275 652c 2073 7464 6f75 743d  ll=True, stdout=
+00024160: 7375 6270 726f 6365 7373 2e50 4950 4529  subprocess.PIPE)
+00024170: 0a20 2020 2074 696d 6572 2e73 746f 705f  .    timer.stop_
+00024180: 7469 6d65 7228 290a 2020 2020 7374 646f  timer().    stdo
+00024190: 7574 5f73 7563 6365 7373 286d 7367 3d66  ut_success(msg=f
+000241a0: 227b 6c65 6e28 7669 6465 6f5f 7061 7468  "{len(video_path
+000241b0: 7329 7d20 7669 6465 6f28 7329 2073 6176  s)} video(s) sav
+000241c0: 6564 2077 6974 6820 7072 6f67 7265 7373  ed with progress
+000241d0: 6261 7220 696e 207b 7361 7665 5f64 6972  bar in {save_dir
+000241e0: 7d20 6469 7265 6374 6f72 792e 222c 2065  } directory.", e
+000241f0: 6c61 7073 6564 5f74 696d 653d 7469 6d65  lapsed_time=time
+00024200: 722e 656c 6170 7365 645f 7469 6d65 5f73  r.elapsed_time_s
+00024210: 7472 2c20 736f 7572 6365 3d73 7570 6572  tr, source=super
+00024220: 696d 706f 7365 5f76 6964 656f 5f70 726f  impose_video_pro
+00024230: 6772 6573 7362 6172 2e5f 5f6e 616d 655f  gressbar.__name_
+00024240: 5f2c 2029 0a0a 6465 6620 6372 6f73 7366  _, )..def crossf
+00024250: 6164 655f 7477 6f5f 7669 6465 6f73 2876  ade_two_videos(v
+00024260: 6964 656f 5f70 6174 685f 313a 2055 6e69  ideo_path_1: Uni
+00024270: 6f6e 5b73 7472 2c20 6f73 2e50 6174 684c  on[str, os.PathL
+00024280: 696b 655d 2c0a 2020 2020 2020 2020 2020  ike],.          
+00024290: 2020 2020 2020 2020 2020 2020 2020 2076                 v
+000242a0: 6964 656f 5f70 6174 685f 323a 2055 6e69  ideo_path_2: Uni
+000242b0: 6f6e 5b73 7472 2c20 6f73 2e50 6174 684c  on[str, os.PathL
+000242c0: 696b 655d 2c0a 2020 2020 2020 2020 2020  ike],.          
+000242d0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000242e0: 726f 7373 6661 6465 5f64 7572 6174 696f  rossfade_duratio
+000242f0: 6e3a 204f 7074 696f 6e61 6c5b 696e 745d  n: Optional[int]
+00024300: 203d 2032 2c0a 2020 2020 2020 2020 2020   = 2,.          
+00024310: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00024320: 726f 7373 6661 6465 5f6d 6574 686f 643a  rossfade_method:
+00024330: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
+00024340: 2027 6661 6465 272c 0a20 2020 2020 2020   'fade',.       
+00024350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024360: 2020 6372 6f73 7366 6164 655f 6f66 6673    crossfade_offs
+00024370: 6574 3a20 4f70 7469 6f6e 616c 5b69 6e74  et: Optional[int
+00024380: 5d20 3d20 322c 0a20 2020 2020 2020 2020  ] = 2,.         
+00024390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000243a0: 7361 7665 5f70 6174 683a 204f 7074 696f  save_path: Optio
+000243b0: 6e61 6c5b 556e 696f 6e5b 7374 722c 206f  nal[Union[str, o
+000243c0: 732e 5061 7468 4c69 6b65 5d5d 203d 204e  s.PathLike]] = N
+000243d0: 6f6e 6529 3a0a 2020 2020 2222 220a 2020  one):.    """.  
+000243e0: 2020 4372 6f73 732d 6661 6465 2074 776f    Cross-fade two
+000243f0: 2076 6964 656f 732e 0a0a 2020 2020 2e2e   videos...    ..
+00024400: 2076 6964 656f 3a3a 205f 7374 6174 6963   video:: _static
+00024410: 2f69 6d67 2f63 726f 7373 6661 6465 5f74  /img/crossfade_t
+00024420: 776f 5f76 6964 656f 732e 7765 626d 0a20  wo_videos.webm. 
+00024430: 2020 2020 2020 3a6c 6f6f 703a 0a0a 2020        :loop:..  
+00024440: 2020 2e2e 206e 6f74 653a 3a0a 2020 2020    .. note::.    
+00024450: 2020 2053 6565 2060 6073 696d 6261 2e75     See ``simba.u
+00024460: 7469 6c73 2e6c 6f6f 6b75 7073 2e67 6574  tils.lookups.get
+00024470: 5f66 666d 7065 675f 6372 6f73 7366 6164  _ffmpeg_crossfad
+00024480: 655f 6d65 7468 6f64 7360 6020 666f 7220  e_methods`` for 
+00024490: 6e61 6d65 6420 6372 6f73 7366 6164 6520  named crossfade 
+000244a0: 6d65 7468 6f64 732e 0a20 2020 2020 2020  methods..       
+000244b0: 5365 6520 6068 7474 7073 3a2f 2f74 7261  See `https://tra
+000244c0: 632e 6666 6d70 6567 2e6f 7267 2f77 696b  c.ffmpeg.org/wik
+000244d0: 692f 5866 6164 6520 3c68 7474 7073 3a2f  i/Xfade <https:/
+000244e0: 2f74 7261 632e 6666 6d70 6567 2e6f 7267  /trac.ffmpeg.org
+000244f0: 2f77 696b 692f 5866 6164 653e 605f 5f2e  /wiki/Xfade>`__.
+00024500: 2066 6f72 2076 6973 7561 6c69 7a61 7469   for visualizati
+00024510: 6f6e 7320 6f66 206e 616d 6564 2063 726f  ons of named cro
+00024520: 7373 6661 6465 206d 6574 686f 6473 2c0a  ssfade methods,.
+00024530: 0a20 2020 203a 7061 7261 6d20 556e 696f  .    :param Unio
+00024540: 6e5b 7374 722c 206f 732e 5061 7468 4c69  n[str, os.PathLi
+00024550: 6b65 5d20 7669 6465 6f5f 7061 7468 5f31  ke] video_path_1
+00024560: 3a20 5061 7468 2074 6f20 7468 6520 6669  : Path to the fi
+00024570: 7273 7420 7669 6465 6f20 6f6e 2064 6973  rst video on dis
+00024580: 6b2e 0a20 2020 203a 7061 7261 6d20 556e  k..    :param Un
+00024590: 696f 6e5b 7374 722c 206f 732e 5061 7468  ion[str, os.Path
+000245a0: 4c69 6b65 5d20 7669 6465 6f5f 7061 7468  Like] video_path
+000245b0: 5f32 3a20 5061 7468 2074 6f20 7468 6520  _2: Path to the 
+000245c0: 7365 636f 6e64 2076 6964 656f 206f 6e20  second video on 
+000245d0: 6469 736b 2e0a 2020 2020 3a70 6172 616d  disk..    :param
+000245e0: 204f 7074 696f 6e61 6c5b 696e 745d 2063   Optional[int] c
+000245f0: 726f 7373 6661 6465 5f64 7572 6174 696f  rossfade_duratio
+00024600: 6e3a 2054 6865 2064 7572 6174 696f 6e20  n: The duration 
+00024610: 6f66 2074 6865 2063 726f 7373 6661 6465  of the crossfade
+00024620: 2e0a 2020 2020 3a70 6172 616d 204f 7074  ..    :param Opt
+00024630: 696f 6e61 6c5b 7374 725d 2063 726f 7373  ional[str] cross
+00024640: 6661 6465 5f6d 6574 686f 643a 2054 6865  fade_method: The
+00024650: 2063 726f 7373 6661 6465 206d 6574 686f   crossfade metho
+00024660: 642e 2046 6f72 2061 6363 6570 7465 6420  d. For accepted 
+00024670: 6d65 7468 6f64 732c 2073 6565 2060 6073  methods, see ``s
+00024680: 696d 6261 2e75 7469 6c73 2e6c 6f6f 6b75  imba.utils.looku
+00024690: 7073 2e67 6574 5f66 666d 7065 675f 6372  ps.get_ffmpeg_cr
+000246a0: 6f73 7366 6164 655f 6d65 7468 6f64 7360  ossfade_methods`
+000246b0: 602e 0a20 2020 203a 7061 7261 6d20 4f70  `..    :param Op
+000246c0: 7469 6f6e 616c 5b69 6e74 5d20 6372 6f73  tional[int] cros
+000246d0: 7366 6164 655f 6f66 6673 6574 3a20 5468  sfade_offset: Th
+000246e0: 6520 7469 6d65 2069 6e20 7365 636f 6e64  e time in second
+000246f0: 7320 696e 746f 2074 6865 2066 6972 7374  s into the first
+00024700: 2076 6964 656f 2062 6566 6f72 6520 7468   video before th
+00024710: 6520 6372 6f73 7366 6164 6520 6475 7261  e crossfade dura
+00024720: 7469 6f6e 2062 6567 696e 732e 0a20 2020  tion begins..   
+00024730: 203a 7061 7261 6d20 4f70 7469 6f6e 616c   :param Optional
+00024740: 5b55 6e69 6f6e 5b73 7472 2c20 6f73 2e50  [Union[str, os.P
+00024750: 6174 684c 696b 655d 5d20 7361 7665 5f70  athLike]] save_p
+00024760: 6174 683a 2054 6865 206c 6f63 6174 696f  ath: The locatio
+00024770: 6e20 7768 6572 6520 746f 2073 6176 6520  n where to save 
+00024780: 7468 6520 6372 6f73 7366 6164 6564 2076  the crossfaded v
+00024790: 6964 656f 2e20 4966 204e 6f6e 652c 2074  ideo. If None, t
+000247a0: 6865 6e20 7361 7665 7320 7468 6520 7669  hen saves the vi
+000247b0: 6465 6f20 696e 2074 6865 2073 616d 6520  deo in the same 
+000247c0: 6469 7265 6374 6f72 7920 6173 2060 6076  directory as ``v
+000247d0: 6964 656f 5f70 6174 685f 3160 6020 7769  ideo_path_1`` wi
+000247e0: 7468 2060 605f 6372 6f73 7366 6164 6560  th ``_crossfade`
+000247f0: 6020 7375 6666 6978 2e0a 0a20 2020 203a  ` suffix...    :
+00024800: 7265 7475 726e 3a20 4e6f 6e65 2e0a 0a20  return: None... 
+00024810: 2020 203a 6578 616d 706c 653a 0a20 2020     :example:.   
+00024820: 203e 3e3e 2063 726f 7373 6661 6465 5f74   >>> crossfade_t
+00024830: 776f 5f76 6964 656f 7328 7669 6465 6f5f  wo_videos(video_
+00024840: 7061 7468 5f31 3d27 2f55 7365 7273 2f73  path_1='/Users/s
+00024850: 696d 6f6e 2f44 6573 6b74 6f70 2f65 6e76  imon/Desktop/env
+00024860: 732f 7369 6d62 612f 7472 6f75 626c 6573  s/simba/troubles
+00024870: 686f 6f74 696e 672f 7265 7074 696c 652f  hooting/reptile/
+00024880: 312e 6d70 3427 2c20 7669 6465 6f5f 7061  1.mp4', video_pa
+00024890: 7468 5f32 3d27 2f55 7365 7273 2f73 696d  th_2='/Users/sim
+000248a0: 6f6e 2f44 6573 6b74 6f70 2f65 6e76 732f  on/Desktop/envs/
+000248b0: 7369 6d62 612f 7472 6f75 626c 6573 686f  simba/troublesho
+000248c0: 6f74 696e 672f 7265 7074 696c 652f 312e  oting/reptile/1.
+000248d0: 6d70 3427 2c20 6372 6f73 7366 6164 655f  mp4', crossfade_
+000248e0: 6475 7261 7469 6f6e 3d35 2c20 6372 6f73  duration=5, cros
+000248f0: 7366 6164 655f 6d65 7468 6f64 3d27 7a6f  sfade_method='zo
+00024900: 6f6d 696e 272c 2073 6176 655f 7061 7468  omin', save_path
+00024910: 3d27 2f55 7365 7273 2f73 696d 6f6e 2f44  ='/Users/simon/D
+00024920: 6573 6b74 6f70 2f63 726f 7373 5f74 6573  esktop/cross_tes
+00024930: 742e 6d70 3427 290a 2020 2020 2222 220a  t.mp4').    """.
+00024940: 0a20 2020 2063 6865 636b 5f66 666d 7065  .    check_ffmpe
+00024950: 675f 6176 6169 6c61 626c 6528 7261 6973  g_available(rais
+00024960: 655f 6572 726f 723d 5472 7565 290a 2020  e_error=True).  
+00024970: 2020 7469 6d65 7220 3d20 5369 6d62 6154    timer = SimbaT
+00024980: 696d 6572 2873 7461 7274 3d54 7275 6529  imer(start=True)
+00024990: 0a20 2020 2076 6964 656f 5f31 5f6d 6574  .    video_1_met
+000249a0: 6120 3d20 6765 745f 7669 6465 6f5f 6d65  a = get_video_me
+000249b0: 7461 5f64 6174 6128 7669 6465 6f5f 7061  ta_data(video_pa
+000249c0: 7468 3d76 6964 656f 5f70 6174 685f 3129  th=video_path_1)
+000249d0: 0a20 2020 2076 6964 656f 5f32 5f6d 6574  .    video_2_met
+000249e0: 6120 3d20 6765 745f 7669 6465 6f5f 6d65  a = get_video_me
+000249f0: 7461 5f64 6174 6128 7669 6465 6f5f 7061  ta_data(video_pa
+00024a00: 7468 3d76 6964 656f 5f70 6174 685f 3229  th=video_path_2)
+00024a10: 0a20 2020 2069 6620 7669 6465 6f5f 315f  .    if video_1_
+00024a20: 6d65 7461 5b27 7265 736f 6c75 7469 6f6e  meta['resolution
+00024a30: 5f73 7472 275d 2021 3d20 7669 6465 6f5f  _str'] != video_
+00024a40: 315f 6d65 7461 5b27 7265 736f 6c75 7469  1_meta['resoluti
+00024a50: 6f6e 5f73 7472 275d 3a0a 2020 2020 2020  on_str']:.      
+00024a60: 2020 7261 6973 6520 496e 7661 6c69 6449    raise InvalidI
+00024a70: 6e70 7574 4572 726f 7228 6d73 673d 6627  nputError(msg=f'
+00024a80: 5669 6465 6f20 3120 616e 6420 5669 6465  Video 1 and Vide
+00024a90: 6f20 3220 6e65 6564 7320 746f 2062 6520  o 2 needs to be 
+00024aa0: 7468 6520 7361 6d65 2072 6573 6f6c 7574  the same resolut
+00024ab0: 696f 6e2c 2067 6f74 207b 7669 6465 6f5f  ion, got {video_
+00024ac0: 325f 6d65 7461 5b22 7265 736f 6c75 7469  2_meta["resoluti
+00024ad0: 6f6e 5f73 7472 225d 7d20 616e 6420 7b76  on_str"]} and {v
+00024ae0: 6964 656f 5f31 5f6d 6574 615b 2272 6573  ideo_1_meta["res
+00024af0: 6f6c 7574 696f 6e5f 7374 7222 5d7d 272c  olution_str"]}',
+00024b00: 2073 6f75 7263 653d 6372 6f73 7366 6164   source=crossfad
+00024b10: 655f 7477 6f5f 7669 6465 6f73 2e5f 5f6e  e_two_videos.__n
+00024b20: 616d 655f 5f29 0a20 2020 2063 726f 7373  ame__).    cross
+00024b30: 6661 6465 5f6f 6666 7365 745f 6d65 7468  fade_offset_meth
+00024b40: 6f64 7320 3d20 6765 745f 6666 6d70 6567  ods = get_ffmpeg
+00024b50: 5f63 726f 7373 6661 6465 5f6d 6574 686f  _crossfade_metho
+00024b60: 6473 2829 0a20 2020 2063 6865 636b 5f73  ds().    check_s
+00024b70: 7472 286e 616d 653d 6627 7b63 726f 7373  tr(name=f'{cross
+00024b80: 6661 6465 5f6d 6574 686f 647d 2063 726f  fade_method} cro
+00024b90: 7373 6661 6465 5f6d 6574 686f 6427 2c20  ssfade_method', 
+00024ba0: 7661 6c75 653d 6372 6f73 7366 6164 655f  value=crossfade_
+00024bb0: 6d65 7468 6f64 2c20 6f70 7469 6f6e 733d  method, options=
+00024bc0: 6372 6f73 7366 6164 655f 6f66 6673 6574  crossfade_offset
+00024bd0: 5f6d 6574 686f 6473 290a 2020 2020 6368  _methods).    ch
+00024be0: 6563 6b5f 696e 7428 6e61 6d65 3d66 277b  eck_int(name=f'{
+00024bf0: 6372 6f73 7366 6164 655f 7477 6f5f 7669  crossfade_two_vi
+00024c00: 6465 6f73 2e5f 5f6e 616d 655f 5f7d 2063  deos.__name__} c
+00024c10: 726f 7373 6661 6465 5f64 7572 6174 696f  rossfade_duratio
+00024c20: 6e27 2c20 7661 6c75 653d 6372 6f73 7366  n', value=crossf
+00024c30: 6164 655f 6475 7261 7469 6f6e 2c20 6d69  ade_duration, mi
+00024c40: 6e5f 7661 6c75 653d 312c 206d 6178 5f76  n_value=1, max_v
+00024c50: 616c 7565 3d76 6964 656f 5f32 5f6d 6574  alue=video_2_met
+00024c60: 615b 2776 6964 656f 5f6c 656e 6774 685f  a['video_length_
+00024c70: 7327 5d29 0a20 2020 2063 6865 636b 5f69  s']).    check_i
+00024c80: 6e74 286e 616d 653d 6627 7b63 726f 7373  nt(name=f'{cross
+00024c90: 6661 6465 5f74 776f 5f76 6964 656f 732e  fade_two_videos.
+00024ca0: 5f5f 6e61 6d65 5f5f 7d20 6372 6f73 7366  __name__} crossf
+00024cb0: 6164 655f 6f66 6673 6574 272c 2076 616c  ade_offset', val
+00024cc0: 7565 3d63 726f 7373 6661 6465 5f6f 6666  ue=crossfade_off
+00024cd0: 7365 742c 206d 696e 5f76 616c 7565 3d30  set, min_value=0
+00024ce0: 2c20 6d61 785f 7661 6c75 653d 7669 6465  , max_value=vide
+00024cf0: 6f5f 315f 6d65 7461 5b27 7669 6465 6f5f  o_1_meta['video_
+00024d00: 6c65 6e67 7468 5f73 275d 290a 2020 2020  length_s']).    
+00024d10: 6469 725f 312c 2076 6964 656f 5f6e 616d  dir_1, video_nam
+00024d20: 655f 312c 2065 7874 5f31 203d 2067 6574  e_1, ext_1 = get
+00024d30: 5f66 6e5f 6578 7428 6669 6c65 7061 7468  _fn_ext(filepath
+00024d40: 3d76 6964 656f 5f70 6174 685f 3129 0a20  =video_path_1). 
+00024d50: 2020 2064 6972 5f32 2c20 7669 6465 6f5f     dir_2, video_
+00024d60: 6e61 6d65 5f32 2c20 6578 745f 3220 3d20  name_2, ext_2 = 
+00024d70: 6765 745f 666e 5f65 7874 2866 696c 6570  get_fn_ext(filep
+00024d80: 6174 683d 7669 6465 6f5f 7061 7468 5f32  ath=video_path_2
+00024d90: 290a 2020 2020 6966 2073 6176 655f 7061  ).    if save_pa
+00024da0: 7468 2069 7320 6e6f 7420 4e6f 6e65 3a0a  th is not None:.
+00024db0: 2020 2020 2020 2020 6368 6563 6b5f 6966          check_if
+00024dc0: 5f64 6972 5f65 7869 7374 7328 696e 5f64  _dir_exists(in_d
+00024dd0: 6972 3d6f 732e 7061 7468 2e64 6972 6e61  ir=os.path.dirna
+00024de0: 6d65 2873 6176 655f 7061 7468 2929 0a20  me(save_path)). 
+00024df0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00024e00: 2073 6176 655f 7061 7468 203d 206f 732e   save_path = os.
+00024e10: 7061 7468 2e6a 6f69 6e28 6469 725f 312c  path.join(dir_1,
+00024e20: 2066 277b 7669 6465 6f5f 6e61 6d65 5f31   f'{video_name_1
+00024e30: 7d5f 7b76 6964 656f 5f6e 616d 655f 327d  }_{video_name_2}
+00024e40: 5f63 726f 7373 6661 6465 7b65 7874 5f31  _crossfade{ext_1
+00024e50: 7d27 290a 2020 2020 636d 6420 3d20 6627  }').    cmd = f'
+00024e60: 6666 6d70 6567 202d 6920 227b 7669 6465  ffmpeg -i "{vide
+00024e70: 6f5f 7061 7468 5f31 7d22 202d 6920 227b  o_path_1}" -i "{
+00024e80: 7669 6465 6f5f 7061 7468 5f32 7d22 202d  video_path_2}" -
+00024e90: 6669 6c74 6572 5f63 6f6d 706c 6578 2022  filter_complex "
+00024ea0: 7866 6164 653d 7472 616e 7369 7469 6f6e  xfade=transition
+00024eb0: 3d7b 6372 6f73 7366 6164 655f 6d65 7468  ={crossfade_meth
+00024ec0: 6f64 7d3a 6f66 6673 6574 3d7b 6372 6f73  od}:offset={cros
+00024ed0: 7366 6164 655f 6f66 6673 6574 7d3a 6475  sfade_offset}:du
+00024ee0: 7261 7469 6f6e 3d7b 6372 6f73 7366 6164  ration={crossfad
+00024ef0: 655f 6475 7261 7469 6f6e 7d22 2022 7b73  e_duration}" "{s
+00024f00: 6176 655f 7061 7468 7d22 202d 6c6f 676c  ave_path}" -logl
+00024f10: 6576 656c 2065 7272 6f72 202d 7374 6174  evel error -stat
+00024f20: 7320 2d68 6964 655f 6261 6e6e 6572 202d  s -hide_banner -
+00024f30: 7927 0a20 2020 2073 7562 7072 6f63 6573  y'.    subproces
+00024f40: 732e 6361 6c6c 2863 6d64 2c20 7368 656c  s.call(cmd, shel
+00024f50: 6c3d 5472 7565 2c20 7374 646f 7574 3d73  l=True, stdout=s
+00024f60: 7562 7072 6f63 6573 732e 5049 5045 290a  ubprocess.PIPE).
+00024f70: 2020 2020 7469 6d65 722e 7374 6f70 5f74      timer.stop_t
+00024f80: 696d 6572 2829 0a20 2020 2073 7464 6f75  imer().    stdou
+00024f90: 745f 7375 6363 6573 7328 6d73 673d 6627  t_success(msg=f'
+00024fa0: 4372 6f73 732d 6661 6465 6420 7669 6465  Cross-faded vide
+00024fb0: 6f20 7361 7665 6420 6174 207b 7361 7665  o saved at {save
+00024fc0: 5f70 6174 687d 272c 2065 6c61 7073 6564  _path}', elapsed
+00024fd0: 5f74 696d 653d 7469 6d65 722e 656c 6170  _time=timer.elap
+00024fe0: 7365 645f 7469 6d65 5f73 7472 290a 0a64  sed_time_str)..d
+00024ff0: 6566 2077 6174 6572 6d61 726b 5f76 6964  ef watermark_vid
+00025000: 656f 2876 6964 656f 5f70 6174 683a 2055  eo(video_path: U
+00025010: 6e69 6f6e 5b73 7472 2c20 6f73 2e50 6174  nion[str, os.Pat
+00025020: 684c 696b 655d 2c0a 2020 2020 2020 2020  hLike],.        
+00025030: 2020 2020 2020 2020 2020 2020 7761 7465              wate
+00025040: 726d 6172 6b5f 7061 7468 3a20 556e 696f  rmark_path: Unio
+00025050: 6e5b 7374 722c 206f 732e 5061 7468 4c69  n[str, os.PathLi
+00025060: 6b65 5d2c 0a20 2020 2020 2020 2020 2020  ke],.           
+00025070: 2020 2020 2020 2020 2070 6f73 6974 696f           positio
+00025080: 6e3a 204f 7074 696f 6e61 6c5b 4c69 7465  n: Optional[Lite
+00025090: 7261 6c5b 2774 6f70 5f6c 6566 7427 2c20  ral['top_left', 
+000250a0: 2762 6f74 746f 6d5f 7269 6768 7427 2c20  'bottom_right', 
+000250b0: 2774 6f70 5f72 6967 6874 272c 2027 626f  'top_right', 'bo
+000250c0: 7474 6f6d 5f6c 6566 7427 2c20 2763 656e  ttom_left', 'cen
+000250d0: 7465 7227 5d5d 203d 2027 746f 705f 6c65  ter']] = 'top_le
+000250e0: 6674 272c 0a20 2020 2020 2020 2020 2020  ft',.           
+000250f0: 2020 2020 2020 2020 206f 7061 6369 7479           opacity
+00025100: 3a20 4f70 7469 6f6e 616c 5b66 6c6f 6174  : Optional[float
+00025110: 5d20 3d20 302e 352c 0a20 2020 2020 2020  ] = 0.5,.       
+00025120: 2020 2020 2020 2020 2020 2020 2073 6361               sca
+00025130: 6c65 3a20 4f70 7469 6f6e 616c 5b66 6c6f  le: Optional[flo
+00025140: 6174 5d20 3d20 302e 3035 2c0a 2020 2020  at] = 0.05,.    
+00025150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025160: 7361 7665 5f64 6972 3a20 4f70 7469 6f6e  save_dir: Option
+00025170: 616c 5b55 6e69 6f6e 5b73 7472 2c20 6f73  al[Union[str, os
+00025180: 2e50 6174 684c 696b 655d 5d20 3d20 4e6f  .PathLike]] = No
+00025190: 6e65 2920 2d3e 204e 6f6e 653a 0a20 2020  ne) -> None:.   
+000251a0: 2022 2222 0a20 2020 2057 6174 6572 6d61   """.    Waterma
+000251b0: 726b 2061 2076 6964 656f 2066 696c 6520  rk a video file 
+000251c0: 6f72 2061 2064 6972 6563 746f 7279 206f  or a directory o
+000251d0: 6620 7669 6465 6f20 6669 6c65 7320 7769  f video files wi
+000251e0: 7468 2073 7065 6369 6669 6564 2077 6174  th specified wat
+000251f0: 6572 6d61 726b 2073 697a 652c 206f 7061  ermark size, opa
+00025200: 6369 7479 2c20 616e 6420 6c6f 6361 7469  city, and locati
+00025210: 6f6e 2e0a 0a20 2020 202e 2e20 7669 6465  on...    .. vide
+00025220: 6f3a 3a20 5f73 7461 7469 632f 696d 672f  o:: _static/img/
+00025230: 7761 7465 726d 6172 6b5f 7669 6465 6f2e  watermark_video.
+00025240: 7765 626d 0a20 2020 2020 2020 3a77 6964  webm.       :wid
+00025250: 7468 3a20 3930 300a 2020 2020 2020 203a  th: 900.       :
+00025260: 6c6f 6f70 3a0a 0a20 2020 203a 7061 7261  loop:..    :para
+00025270: 6d20 556e 696f 6e5b 7374 722c 206f 732e  m Union[str, os.
+00025280: 5061 7468 4c69 6b65 5d20 7669 6465 6f5f  PathLike] video_
+00025290: 7061 7468 3a20 5468 6520 7061 7468 2074  path: The path t
+000252a0: 6f20 7468 6520 7669 6465 6f20 6669 6c65  o the video file
+000252b0: 206f 7220 7061 7468 2074 6f20 6469 7265   or path to dire
+000252c0: 6374 6f72 7920 7769 7468 2076 6964 656f  ctory with video
+000252d0: 2066 696c 6573 2e0a 2020 2020 3a70 6172   files..    :par
+000252e0: 616d 2055 6e69 6f6e 5b73 7472 2c20 6f73  am Union[str, os
+000252f0: 2e50 6174 684c 696b 655d 2077 6174 6572  .PathLike] water
+00025300: 6d61 726b 5f70 6174 683a 2054 6865 2070  mark_path: The p
+00025310: 6174 6820 746f 2074 6865 2077 6174 6572  ath to the water
+00025320: 6d61 726b 202e 706e 6720 6669 6c65 2e0a  mark .png file..
+00025330: 2020 2020 3a70 6172 616d 204f 7074 696f      :param Optio
+00025340: 6e61 6c5b 7374 725d 2070 6f73 6974 696f  nal[str] positio
+00025350: 6e3a 2054 6865 2070 6f73 6974 696f 6e20  n: The position 
+00025360: 6f66 2074 6865 2077 6174 6572 6d61 726b  of the watermark
+00025370: 2e20 4f70 7469 6f6e 733a 2027 746f 705f  . Options: 'top_
+00025380: 6c65 6674 272c 2027 626f 7474 6f6d 5f72  left', 'bottom_r
+00025390: 6967 6874 272c 2027 746f 705f 7269 6768  ight', 'top_righ
+000253a0: 7427 2c20 2762 6f74 746f 6d5f 6c65 6674  t', 'bottom_left
+000253b0: 272c 2027 6365 6e74 6572 270a 2020 2020  ', 'center'.    
+000253c0: 3a70 6172 616d 204f 7074 696f 6e61 6c5b  :param Optional[
+000253d0: 666c 6f61 745d 206f 7061 6369 7479 3a20  float] opacity: 
+000253e0: 5468 6520 6f70 6163 6974 7920 6f66 2074  The opacity of t
+000253f0: 6865 2077 6174 6572 6d61 726b 2061 7320  he watermark as 
+00025400: 6120 7661 6c75 6520 6265 7477 6565 6e20  a value between 
+00025410: 302d 312e 302e 2031 2e30 206d 6561 6e69  0-1.0. 1.0 meani
+00025420: 6e67 2074 6865 2073 616d 6520 6173 2069  ng the same as i
+00025430: 6e70 7574 2069 6d61 6765 2e20 4465 6661  nput image. Defa
+00025440: 756c 743a 2030 2e35 2e0a 2020 2020 3a70  ult: 0.5..    :p
+00025450: 6172 616d 204f 7074 696f 6e61 6c5b 666c  aram Optional[fl
+00025460: 6f61 745d 2073 6361 6c65 3a20 5468 6520  oat] scale: The 
+00025470: 7363 616c 6520 6f66 2074 6865 2077 6174  scale of the wat
+00025480: 6572 6d61 726b 2061 7320 6120 7261 7469  ermark as a rati
+00025490: 6f20 6f73 2074 6865 2069 6d61 6765 2073  o os the image s
+000254a0: 697a 652e 2044 6566 6175 6c74 3a20 302e  ize. Default: 0.
+000254b0: 3035 2e0a 2020 2020 3a70 6172 616d 204f  05..    :param O
+000254c0: 7074 696f 6e61 6c5b 556e 696f 6e5b 7374  ptional[Union[st
+000254d0: 722c 206f 732e 5061 7468 4c69 6b65 5d5d  r, os.PathLike]]
+000254e0: 2073 6176 655f 6469 723a 2054 6865 206c   save_dir: The l
+000254f0: 6f63 6174 696f 6e20 7768 6572 6520 746f  ocation where to
+00025500: 2073 6176 6520 7468 6520 7761 7465 726d   save the waterm
+00025510: 6172 6b65 6420 7669 6465 6f2e 2049 6620  arked video. If 
+00025520: 4e6f 6e65 2c20 7468 656e 2073 6176 6573  None, then saves
+00025530: 2074 6865 2076 6964 656f 2069 6e20 7468   the video in th
+00025540: 6520 7361 6d65 2064 6972 6563 746f 7279  e same directory
+00025550: 2061 7320 7468 6520 6669 7273 7420 7669   as the first vi
+00025560: 6465 6f2e 0a20 2020 203a 7265 7475 726e  deo..    :return
+00025570: 3a20 4e6f 6e65 0a0a 2020 2020 3a65 7861  : None..    :exa
+00025580: 6d70 6c65 3a0a 2020 2020 3e3e 3e20 7761  mple:.    >>> wa
+00025590: 7465 726d 6172 6b5f 7669 6465 6f28 7669  termark_video(vi
+000255a0: 6465 6f5f 7061 7468 3d27 2f55 7365 7273  deo_path='/Users
+000255b0: 2f73 696d 6f6e 2f44 6573 6b74 6f70 2f65  /simon/Desktop/e
+000255c0: 6e76 732f 7369 6d62 612f 7472 6f75 626c  nvs/simba/troubl
+000255d0: 6573 686f 6f74 696e 672f 6d75 6c74 695f  eshooting/multi_
+000255e0: 616e 696d 616c 5f64 6c63 5f74 776f 5f63  animal_dlc_two_c
+000255f0: 3537 2f70 726f 6a65 6374 5f66 6f6c 6465  57/project_folde
+00025600: 722f 7669 6465 6f73 2f77 6174 6572 6d61  r/videos/waterma
+00025610: 726b 2f54 6f67 6574 6865 725f 315f 706f  rk/Together_1_po
+00025620: 7765 7270 6f69 6e74 7265 6164 792e 6d70  werpointready.mp
+00025630: 3427 2c20 7761 7465 726d 6172 6b5f 7061  4', watermark_pa
+00025640: 7468 3d27 2f55 7365 7273 2f73 696d 6f6e  th='/Users/simon
+00025650: 2f44 6573 6b74 6f70 2f73 706c 6173 682e  /Desktop/splash.
+00025660: 706e 6727 2c20 706f 7369 7469 6f6e 3d27  png', position='
+00025670: 746f 705f 6c65 6674 272c 206f 7061 6369  top_left', opaci
+00025680: 7479 3d31 2e30 2c20 7363 616c 653d 302e  ty=1.0, scale=0.
+00025690: 3229 0a20 2020 2022 2222 0a20 2020 2063  2).    """.    c
+000256a0: 6865 636b 5f66 666d 7065 675f 6176 6169  heck_ffmpeg_avai
+000256b0: 6c61 626c 6528 7261 6973 655f 6572 726f  lable(raise_erro
+000256c0: 723d 5472 7565 290a 2020 2020 7469 6d65  r=True).    time
+000256d0: 7220 3d20 5369 6d62 6154 696d 6572 2873  r = SimbaTimer(s
+000256e0: 7461 7274 3d54 7275 6529 0a20 2020 2050  tart=True).    P
+000256f0: 4f53 4954 494f 4e53 203d 205b 2774 6f70  OSITIONS = ['top
+00025700: 5f6c 6566 7427 2c20 2762 6f74 746f 6d5f  _left', 'bottom_
+00025710: 7269 6768 7427 2c20 2774 6f70 5f72 6967  right', 'top_rig
+00025720: 6874 272c 2027 626f 7474 6f6d 5f6c 6566  ht', 'bottom_lef
+00025730: 7427 2c20 2763 656e 7465 7227 5d0a 2020  t', 'center'].  
+00025740: 2020 6368 6563 6b5f 666c 6f61 7428 6e61    check_float(na
+00025750: 6d65 3d66 277b 7761 7465 726d 6172 6b5f  me=f'{watermark_
+00025760: 7669 6465 6f2e 5f5f 6e61 6d65 5f5f 7d20  video.__name__} 
+00025770: 6f70 6163 6974 7927 2c20 7661 6c75 653d  opacity', value=
+00025780: 6f70 6163 6974 792c 206d 696e 5f76 616c  opacity, min_val
+00025790: 7565 3d30 2e30 3031 2c20 6d61 785f 7661  ue=0.001, max_va
+000257a0: 6c75 653d 312e 3029 0a20 2020 2063 6865  lue=1.0).    che
+000257b0: 636b 5f66 6c6f 6174 286e 616d 653d 6627  ck_float(name=f'
+000257c0: 7b77 6174 6572 6d61 726b 5f76 6964 656f  {watermark_video
+000257d0: 2e5f 5f6e 616d 655f 5f7d 2073 6361 6c65  .__name__} scale
+000257e0: 272c 2076 616c 7565 3d73 6361 6c65 2c20  ', value=scale, 
+000257f0: 6d69 6e5f 7661 6c75 653d 302e 3030 312c  min_value=0.001,
+00025800: 206d 6178 5f76 616c 7565 3d30 2e39 3939   max_value=0.999
+00025810: 290a 2020 2020 6368 6563 6b5f 7374 7228  ).    check_str(
+00025820: 6e61 6d65 3d66 277b 7761 7465 726d 6172  name=f'{watermar
+00025830: 6b5f 7669 6465 6f2e 5f5f 6e61 6d65 5f5f  k_video.__name__
+00025840: 7d20 706f 7369 7469 6f6e 272c 2076 616c  } position', val
+00025850: 7565 3d70 6f73 6974 696f 6e2c 206f 7074  ue=position, opt
+00025860: 696f 6e73 3d50 4f53 4954 494f 4e53 290a  ions=POSITIONS).
+00025870: 2020 2020 6368 6563 6b5f 6669 6c65 5f65      check_file_e
+00025880: 7869 7374 5f61 6e64 5f72 6561 6461 626c  xist_and_readabl
+00025890: 6528 6669 6c65 5f70 6174 683d 7761 7465  e(file_path=wate
+000258a0: 726d 6172 6b5f 7061 7468 290a 0a20 2020  rmark_path)..   
+000258b0: 2069 6620 6f73 2e70 6174 682e 6973 6669   if os.path.isfi
+000258c0: 6c65 2876 6964 656f 5f70 6174 6829 3a0a  le(video_path):.
+000258d0: 2020 2020 2020 2020 7669 6465 6f5f 7061          video_pa
+000258e0: 7468 7320 3d20 5b76 6964 656f 5f70 6174  ths = [video_pat
+000258f0: 685d 0a20 2020 2065 6c69 6620 6f73 2e70  h].    elif os.p
+00025900: 6174 682e 6973 6469 7228 7669 6465 6f5f  ath.isdir(video_
+00025910: 7061 7468 293a 0a20 2020 2020 2020 2076  path):.        v
+00025920: 6964 656f 5f70 6174 6873 203d 206c 6973  ideo_paths = lis
+00025930: 7428 6669 6e64 5f61 6c6c 5f76 6964 656f  t(find_all_video
+00025940: 735f 696e 5f64 6972 6563 746f 7279 2864  s_in_directory(d
+00025950: 6972 6563 746f 7279 3d76 6964 656f 5f70  irectory=video_p
+00025960: 6174 682c 2061 735f 6469 6374 3d54 7275  ath, as_dict=Tru
+00025970: 652c 2072 6169 7365 5f65 7272 6f72 3d54  e, raise_error=T
+00025980: 7275 6529 2e76 616c 7565 7328 2929 0a20  rue).values()). 
+00025990: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+000259a0: 2072 6169 7365 2049 6e76 616c 6964 496e   raise InvalidIn
+000259b0: 7075 7445 7272 6f72 286d 7367 3d66 277b  putError(msg=f'{
+000259c0: 7669 6465 6f5f 7061 7468 7d20 6973 206e  video_path} is n
+000259d0: 6f74 2061 2076 616c 6964 2066 696c 6520  ot a valid file 
+000259e0: 7061 7468 206f 7220 6120 7661 6c69 6420  path or a valid 
+000259f0: 6469 7265 6374 6f72 7920 7061 7468 272c  directory path',
+00025a00: 2073 6f75 7263 653d 7761 7465 726d 6172   source=watermar
+00025a10: 6b5f 7669 6465 6f2e 5f5f 6e61 6d65 5f5f  k_video.__name__
+00025a20: 290a 2020 2020 6966 2073 6176 655f 6469  ).    if save_di
+00025a30: 7220 6973 206e 6f74 204e 6f6e 653a 0a20  r is not None:. 
+00025a40: 2020 2020 2020 2063 6865 636b 5f69 665f         check_if_
+00025a50: 6469 725f 6578 6973 7473 2869 6e5f 6469  dir_exists(in_di
+00025a60: 723d 7361 7665 5f64 6972 290a 2020 2020  r=save_dir).    
+00025a70: 656c 7365 3a0a 2020 2020 2020 2020 7361  else:.        sa
+00025a80: 7665 5f64 6972 203d 206f 732e 7061 7468  ve_dir = os.path
+00025a90: 2e64 6972 6e61 6d65 2876 6964 656f 5f70  .dirname(video_p
+00025aa0: 6174 6873 5b30 5d29 0a20 2020 2066 6f72  aths[0]).    for
+00025ab0: 2066 696c 655f 636e 742c 2076 6964 656f   file_cnt, video
+00025ac0: 5f70 6174 6820 696e 2065 6e75 6d65 7261  _path in enumera
+00025ad0: 7465 2876 6964 656f 5f70 6174 6873 293a  te(video_paths):
+00025ae0: 0a20 2020 2020 2020 205f 2c20 7669 6465  .        _, vide
+00025af0: 6f5f 6e61 6d65 2c20 7669 6465 6f5f 6578  o_name, video_ex
+00025b00: 7420 3d20 6765 745f 666e 5f65 7874 2876  t = get_fn_ext(v
+00025b10: 6964 656f 5f70 6174 6829 0a20 2020 2020  ideo_path).     
+00025b20: 2020 205f 203d 2067 6574 5f76 6964 656f     _ = get_video
+00025b30: 5f6d 6574 615f 6461 7461 2876 6964 656f  _meta_data(video
+00025b40: 5f70 6174 683d 7669 6465 6f5f 7061 7468  _path=video_path
+00025b50: 290a 2020 2020 2020 2020 7072 696e 7428  ).        print(
+00025b60: 6627 5761 7465 726d 6172 6b69 6e67 207b  f'Watermarking {
+00025b70: 7669 6465 6f5f 6e61 6d65 7d20 2856 6964  video_name} (Vid
+00025b80: 656f 207b 6669 6c65 5f63 6e74 2b31 7d2f  eo {file_cnt+1}/
+00025b90: 7b6c 656e 2876 6964 656f 5f70 6174 6873  {len(video_paths
+00025ba0: 297d 292e 2e2e 2729 0a20 2020 2020 2020  )})...').       
+00025bb0: 206f 7574 5f70 6174 6820 3d20 6f73 2e70   out_path = os.p
+00025bc0: 6174 682e 6a6f 696e 2873 6176 655f 6469  ath.join(save_di
+00025bd0: 722c 2066 277b 7669 6465 6f5f 6e61 6d65  r, f'{video_name
+00025be0: 7d5f 7761 7465 726d 6172 6b65 647b 7669  }_watermarked{vi
+00025bf0: 6465 6f5f 6578 747d 2729 0a20 2020 2020  deo_ext}').     
+00025c00: 2020 2069 6620 706f 7369 7469 6f6e 203d     if position =
+00025c10: 3d20 504f 5349 5449 4f4e 535b 305d 3a0a  = POSITIONS[0]:.
+00025c20: 2020 2020 2020 2020 2020 2020 636d 6420              cmd 
+00025c30: 3d20 6627 6666 6d70 6567 202d 6920 227b  = f'ffmpeg -i "{
+00025c40: 7669 6465 6f5f 7061 7468 7d22 202d 6920  video_path}" -i 
+00025c50: 227b 7761 7465 726d 6172 6b5f 7061 7468  "{watermark_path
+00025c60: 7d22 202d 6669 6c74 6572 5f63 6f6d 706c  }" -filter_compl
+00025c70: 6578 2022 5b31 3a76 5d73 6361 6c65 3d69  ex "[1:v]scale=i
+00025c80: 772a 7b73 6361 6c65 7d3a 2d31 2c66 6f72  w*{scale}:-1,for
+00025c90: 6d61 743d 7267 6261 2c63 6f6c 6f72 6368  mat=rgba,colorch
+00025ca0: 616e 6e65 6c6d 6978 6572 3d61 613d 7b6f  annelmixer=aa={o
+00025cb0: 7061 6369 7479 7d5b 776d 5d3b 5b30 3a76  pacity}[wm];[0:v
+00025cc0: 5d5b 776d 5d6f 7665 726c 6179 3d30 3a30  ][wm]overlay=0:0
+00025cd0: 2220 227b 6f75 745f 7061 7468 7d22 202d  " "{out_path}" -
+00025ce0: 6c6f 676c 6576 656c 2065 7272 6f72 202d  loglevel error -
+00025cf0: 7374 6174 7320 2d68 6964 655f 6261 6e6e  stats -hide_bann
+00025d00: 6572 202d 7927 0a20 2020 2020 2020 2065  er -y'.        e
+00025d10: 6c69 6620 706f 7369 7469 6f6e 203d 3d20  lif position == 
+00025d20: 504f 5349 5449 4f4e 535b 315d 3a0a 2020  POSITIONS[1]:.  
+00025d30: 2020 2020 2020 2020 2020 636d 6420 3d20            cmd = 
+00025d40: 6627 6666 6d70 6567 202d 6920 227b 7669  f'ffmpeg -i "{vi
+00025d50: 6465 6f5f 7061 7468 7d22 202d 6920 227b  deo_path}" -i "{
+00025d60: 7761 7465 726d 6172 6b5f 7061 7468 7d22  watermark_path}"
+00025d70: 202d 6669 6c74 6572 5f63 6f6d 706c 6578   -filter_complex
+00025d80: 2022 5b31 3a76 5d73 6361 6c65 3d69 772a   "[1:v]scale=iw*
+00025d90: 7b73 6361 6c65 7d3a 2d31 2c66 6f72 6d61  {scale}:-1,forma
+00025da0: 743d 7267 6261 2c63 6f6c 6f72 6368 616e  t=rgba,colorchan
+00025db0: 6e65 6c6d 6978 6572 3d61 613d 7b6f 7061  nelmixer=aa={opa
+00025dc0: 6369 7479 7d5b 776d 5d3b 5b30 3a76 5d5b  city}[wm];[0:v][
+00025dd0: 776d 5d6f 7665 726c 6179 3d57 2d77 3a48  wm]overlay=W-w:H
+00025de0: 2d68 2220 227b 6f75 745f 7061 7468 7d22  -h" "{out_path}"
+00025df0: 202d 6c6f 676c 6576 656c 2065 7272 6f72   -loglevel error
+00025e00: 202d 7374 6174 7320 2d68 6964 655f 6261   -stats -hide_ba
+00025e10: 6e6e 6572 202d 7927 0a20 2020 2020 2020  nner -y'.       
+00025e20: 2065 6c69 6620 706f 7369 7469 6f6e 203d   elif position =
+00025e30: 3d20 504f 5349 5449 4f4e 535b 325d 3a0a  = POSITIONS[2]:.
+00025e40: 2020 2020 2020 2020 2020 2020 636d 6420              cmd 
+00025e50: 3d20 6627 6666 6d70 6567 202d 6920 227b  = f'ffmpeg -i "{
+00025e60: 7669 6465 6f5f 7061 7468 7d22 202d 6920  video_path}" -i 
+00025e70: 227b 7761 7465 726d 6172 6b5f 7061 7468  "{watermark_path
+00025e80: 7d22 202d 6669 6c74 6572 5f63 6f6d 706c  }" -filter_compl
+00025e90: 6578 2022 5b31 3a76 5d73 6361 6c65 3d69  ex "[1:v]scale=i
+00025ea0: 772a 7b73 6361 6c65 7d3a 2d31 2c66 6f72  w*{scale}:-1,for
+00025eb0: 6d61 743d 7267 6261 2c63 6f6c 6f72 6368  mat=rgba,colorch
+00025ec0: 616e 6e65 6c6d 6978 6572 3d61 613d 7b6f  annelmixer=aa={o
+00025ed0: 7061 6369 7479 7d5b 776d 5d3b 5b30 3a76  pacity}[wm];[0:v
+00025ee0: 5d5b 776d 5d6f 7665 726c 6179 3d57 2d77  ][wm]overlay=W-w
+00025ef0: 2d30 3a30 2220 227b 6f75 745f 7061 7468  -0:0" "{out_path
+00025f00: 7d22 202d 6c6f 676c 6576 656c 2065 7272  }" -loglevel err
+00025f10: 6f72 202d 7374 6174 7320 2d68 6964 655f  or -stats -hide_
+00025f20: 6261 6e6e 6572 202d 7927 0a20 2020 2020  banner -y'.     
+00025f30: 2020 2065 6c69 6620 706f 7369 7469 6f6e     elif position
+00025f40: 203d 3d20 504f 5349 5449 4f4e 535b 335d   == POSITIONS[3]
+00025f50: 3a0a 2020 2020 2020 2020 2020 2020 636d  :.            cm
+00025f60: 6420 3d20 6627 6666 6d70 6567 202d 6920  d = f'ffmpeg -i 
+00025f70: 227b 7669 6465 6f5f 7061 7468 7d22 202d  "{video_path}" -
+00025f80: 6920 227b 7761 7465 726d 6172 6b5f 7061  i "{watermark_pa
+00025f90: 7468 7d22 202d 6669 6c74 6572 5f63 6f6d  th}" -filter_com
+00025fa0: 706c 6578 2022 5b31 3a76 5d73 6361 6c65  plex "[1:v]scale
+00025fb0: 3d69 772a 7b73 6361 6c65 7d3a 2d31 2c66  =iw*{scale}:-1,f
+00025fc0: 6f72 6d61 743d 7267 6261 2c63 6f6c 6f72  ormat=rgba,color
+00025fd0: 6368 616e 6e65 6c6d 6978 6572 3d61 613d  channelmixer=aa=
+00025fe0: 7b6f 7061 6369 7479 7d5b 776d 5d3b 5b30  {opacity}[wm];[0
+00025ff0: 3a76 5d5b 776d 5d6f 7665 726c 6179 3d30  :v][wm]overlay=0
+00026000: 3a48 2d68 2d30 2220 227b 6f75 745f 7061  :H-h-0" "{out_pa
+00026010: 7468 7d22 202d 6c6f 676c 6576 656c 2065  th}" -loglevel e
+00026020: 7272 6f72 202d 7374 6174 7320 2d68 6964  rror -stats -hid
+00026030: 655f 6261 6e6e 6572 202d 7927 0a20 2020  e_banner -y'.   
+00026040: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00026050: 2020 2020 2020 2063 6d64 203d 2066 2766         cmd = f'f
+00026060: 666d 7065 6720 2d69 2022 7b76 6964 656f  fmpeg -i "{video
+00026070: 5f70 6174 687d 2220 2d69 2022 7b77 6174  _path}" -i "{wat
+00026080: 6572 6d61 726b 5f70 6174 687d 2220 2d66  ermark_path}" -f
+00026090: 696c 7465 725f 636f 6d70 6c65 7820 225b  ilter_complex "[
+000260a0: 313a 765d 7363 616c 653d 6977 2a7b 7363  1:v]scale=iw*{sc
+000260b0: 616c 657d 3a2d 312c 666f 726d 6174 3d72  ale}:-1,format=r
+000260c0: 6762 612c 636f 6c6f 7263 6861 6e6e 656c  gba,colorchannel
+000260d0: 6d69 7865 723d 6161 3d7b 6f70 6163 6974  mixer=aa={opacit
+000260e0: 797d 5b77 6d5d 3b5b 303a 765d 5b77 6d5d  y}[wm];[0:v][wm]
+000260f0: 6f76 6572 6c61 793d 2857 2d77 292f 323a  overlay=(W-w)/2:
+00026100: 2848 2d68 292f 3222 2022 7b6f 7574 5f70  (H-h)/2" "{out_p
+00026110: 6174 687d 2220 2d6c 6f67 6c65 7665 6c20  ath}" -loglevel 
+00026120: 6572 726f 7220 2d73 7461 7473 202d 6869  error -stats -hi
+00026130: 6465 5f62 616e 6e65 7220 2d79 270a 2020  de_banner -y'.  
+00026140: 2020 2020 2020 7375 6270 726f 6365 7373        subprocess
+00026150: 2e63 616c 6c28 636d 642c 2073 6865 6c6c  .call(cmd, shell
+00026160: 3d54 7275 652c 2073 7464 6f75 743d 7375  =True, stdout=su
+00026170: 6270 726f 6365 7373 2e50 4950 4529 0a20  bprocess.PIPE). 
+00026180: 2020 2074 696d 6572 2e73 746f 705f 7469     timer.stop_ti
+00026190: 6d65 7228 290a 2020 2020 7374 646f 7574  mer().    stdout
+000261a0: 5f73 7563 6365 7373 286d 7367 3d66 277b  _success(msg=f'{
+000261b0: 6c65 6e28 7669 6465 6f5f 7061 7468 7329  len(video_paths)
+000261c0: 7d20 7761 7465 726d 6172 6b65 6420 7669  } watermarked vi
+000261d0: 6465 6f28 7329 2073 6176 6564 2069 6e20  deo(s) saved in 
+000261e0: 7b73 6176 655f 6469 727d 272c 2065 6c61  {save_dir}', ela
+000261f0: 7073 6564 5f74 696d 653d 7469 6d65 722e  psed_time=timer.
+00026200: 656c 6170 7365 645f 7469 6d65 5f73 7472  elapsed_time_str
+00026210: 290a 0a64 6566 2069 6e73 6574 5f6f 7665  )..def inset_ove
+00026220: 726c 6179 5f76 6964 656f 2876 6964 656f  rlay_video(video
+00026230: 5f70 6174 683a 2055 6e69 6f6e 5b73 7472  _path: Union[str
+00026240: 2c20 6f73 2e50 6174 684c 696b 655d 2c0a  , os.PathLike],.
+00026250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026260: 2020 2020 2020 2020 6f76 6572 6c61 795f          overlay_
+00026270: 7669 6465 6f5f 7061 7468 3a20 556e 696f  video_path: Unio
+00026280: 6e5b 7374 722c 206f 732e 5061 7468 4c69  n[str, os.PathLi
+00026290: 6b65 5d2c 0a20 2020 2020 2020 2020 2020  ke],.           
+000262a0: 2020 2020 2020 2020 2020 2020 2070 6f73               pos
+000262b0: 6974 696f 6e3a 204f 7074 696f 6e61 6c5b  ition: Optional[
+000262c0: 4c69 7465 7261 6c5b 2774 6f70 5f6c 6566  Literal['top_lef
+000262d0: 7427 2c20 2762 6f74 746f 6d5f 7269 6768  t', 'bottom_righ
+000262e0: 7427 2c20 2774 6f70 5f72 6967 6874 272c  t', 'top_right',
+000262f0: 2027 626f 7474 6f6d 5f6c 6566 7427 2c20   'bottom_left', 
+00026300: 2763 656e 7465 7227 5d5d 203d 2027 746f  'center']] = 'to
+00026310: 705f 6c65 6674 272c 0a20 2020 2020 2020  p_left',.       
 00026320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026330: 2020 2073 6361 6c65 3a20 4f70 7469 6f6e     scale: Option
-00026340: 616c 5b66 6c6f 6174 5d20 3d20 302e 3035  al[float] = 0.05
-00026350: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00026360: 2020 2020 2020 2020 2020 7361 7665 5f64            save_d
-00026370: 6972 3a20 4f70 7469 6f6e 616c 5b55 6e69  ir: Optional[Uni
-00026380: 6f6e 5b73 7472 2c20 6f73 2e50 6174 684c  on[str, os.PathL
-00026390: 696b 655d 5d20 3d20 4e6f 6e65 2920 2d3e  ike]] = None) ->
-000263a0: 204e 6f6e 653a 0a20 2020 2022 2222 0a20   None:.    """. 
-000263b0: 2020 2049 6e73 6574 2061 2076 6964 656f     Inset a video
-000263c0: 206f 7665 726c 6179 206f 6e20 6120 7365   overlay on a se
-000263d0: 636f 6e64 2076 6964 656f 2077 6974 6820  cond video with 
-000263e0: 7370 6563 6966 6965 6420 7369 7a65 2c20  specified size, 
-000263f0: 6f70 6163 6974 792c 2061 6e64 206c 6f63  opacity, and loc
-00026400: 6174 696f 6e2e 0a0a 2020 2020 2e2e 2076  ation...    .. v
-00026410: 6964 656f 3a3a 205f 7374 6174 6963 2f69  ideo:: _static/i
-00026420: 6d67 2f69 6e73 6574 5f6f 7665 726c 6179  mg/inset_overlay
-00026430: 5f76 6964 656f 2e77 6562 6d0a 2020 2020  _video.webm.    
-00026440: 2020 203a 7769 6474 683a 2037 3030 0a20     :width: 700. 
-00026450: 2020 2020 2020 3a6c 6f6f 703a 0a0a 2020        :loop:..  
-00026460: 2020 3a70 6172 616d 2055 6e69 6f6e 5b73    :param Union[s
-00026470: 7472 2c20 6f73 2e50 6174 684c 696b 655d  tr, os.PathLike]
-00026480: 2076 6964 656f 5f70 6174 683a 2054 6865   video_path: The
-00026490: 2070 6174 6820 746f 2074 6865 2076 6964   path to the vid
-000264a0: 656f 2066 696c 652e 0a20 2020 203a 7061  eo file..    :pa
-000264b0: 7261 6d20 556e 696f 6e5b 7374 722c 206f  ram Union[str, o
-000264c0: 732e 5061 7468 4c69 6b65 5d20 6f76 6572  s.PathLike] over
-000264d0: 6c61 795f 7669 6465 6f5f 7061 7468 3a20  lay_video_path: 
-000264e0: 5468 6520 7061 7468 2074 6f20 7669 6465  The path to vide
-000264f0: 6f20 746f 2062 6520 696e 7365 7274 6564  o to be inserted
-00026500: 2069 6e74 6f20 7468 6520 6060 7669 6465   into the ``vide
-00026510: 6f5f 7061 7468 6060 2076 6964 656f 2e0a  o_path`` video..
-00026520: 2020 2020 3a70 6172 616d 204f 7074 696f      :param Optio
-00026530: 6e61 6c5b 7374 725d 2070 6f73 6974 696f  nal[str] positio
-00026540: 6e3a 2054 6865 2070 6f73 6974 696f 6e20  n: The position 
-00026550: 6f66 2074 6865 2069 6e73 6574 206f 7665  of the inset ove
-00026560: 726c 6179 2076 6964 656f 2e20 4f70 7469  rlay video. Opti
-00026570: 6f6e 733a 2027 746f 705f 6c65 6674 272c  ons: 'top_left',
-00026580: 2027 626f 7474 6f6d 5f72 6967 6874 272c   'bottom_right',
-00026590: 2027 746f 705f 7269 6768 7427 2c20 2762   'top_right', 'b
-000265a0: 6f74 746f 6d5f 6c65 6674 272c 2027 6365  ottom_left', 'ce
-000265b0: 6e74 6572 270a 2020 2020 3a70 6172 616d  nter'.    :param
-000265c0: 204f 7074 696f 6e61 6c5b 666c 6f61 745d   Optional[float]
-000265d0: 206f 7061 6369 7479 3a20 5468 6520 6f70   opacity: The op
-000265e0: 6163 6974 7920 6f66 2074 6865 2069 6e73  acity of the ins
-000265f0: 6574 206f 7665 726c 6179 2076 6964 656f  et overlay video
-00026600: 2061 7320 6120 7661 6c75 6520 6265 7477   as a value betw
-00026610: 6565 6e20 302d 312e 302e 2031 2e30 206d  een 0-1.0. 1.0 m
-00026620: 6561 6e69 6e67 2074 6865 2073 616d 6520  eaning the same 
-00026630: 6173 2069 6e70 7574 2069 6d61 6765 2e20  as input image. 
-00026640: 4465 6661 756c 743a 2030 2e35 2e0a 2020  Default: 0.5..  
-00026650: 2020 3a70 6172 616d 204f 7074 696f 6e61    :param Optiona
-00026660: 6c5b 666c 6f61 745d 2073 6361 6c65 3a20  l[float] scale: 
-00026670: 5468 6520 7363 616c 6520 6f66 2074 6865  The scale of the
-00026680: 2069 6e73 6574 206f 7665 726c 6179 2076   inset overlay v
-00026690: 6964 656f 2061 7320 6120 7261 7469 6f20  ideo as a ratio 
-000266a0: 6f73 2074 6865 2069 6d61 6765 2073 697a  os the image siz
-000266b0: 652e 2044 6566 6175 6c74 3a20 302e 3035  e. Default: 0.05
-000266c0: 2e0a 2020 2020 3a70 6172 616d 204f 7074  ..    :param Opt
-000266d0: 696f 6e61 6c5b 556e 696f 6e5b 7374 722c  ional[Union[str,
-000266e0: 206f 732e 5061 7468 4c69 6b65 5d5d 2073   os.PathLike]] s
-000266f0: 6176 655f 6469 723a 2054 6865 206c 6f63  ave_dir: The loc
-00026700: 6174 696f 6e20 7768 6572 6520 746f 2073  ation where to s
-00026710: 6176 6520 7468 6520 6f75 7470 7574 2076  ave the output v
-00026720: 6964 656f 2e20 4966 204e 6f6e 652c 2074  ideo. If None, t
-00026730: 6865 6e20 7361 7665 7320 7468 6520 7669  hen saves the vi
-00026740: 6465 6f20 696e 2074 6865 2073 616d 6520  deo in the same 
-00026750: 6469 7265 6374 6f72 7920 6173 2074 6865  directory as the
-00026760: 2066 6972 7374 2076 6964 656f 2e0a 2020   first video..  
-00026770: 2020 3a72 6574 7572 6e3a 204e 6f6e 650a    :return: None.
-00026780: 0a20 2020 203a 6578 616d 706c 653a 0a20  .    :example:. 
-00026790: 2020 203e 3e3e 2069 6e73 6574 5f6f 7665     >>> inset_ove
-000267a0: 726c 6179 5f76 6964 656f 2876 6964 656f  rlay_video(video
-000267b0: 5f70 6174 683d 272f 5573 6572 732f 7369  _path='/Users/si
-000267c0: 6d6f 6e2f 4465 736b 746f 702f 656e 7673  mon/Desktop/envs
-000267d0: 2f73 696d 6261 2f74 726f 7562 6c65 7368  /simba/troublesh
-000267e0: 6f6f 7469 6e67 2f6d 756c 7469 5f61 6e69  ooting/multi_ani
-000267f0: 6d61 6c5f 646c 635f 7477 6f5f 6335 372f  mal_dlc_two_c57/
-00026800: 7072 6f6a 6563 745f 666f 6c64 6572 2f76  project_folder/v
-00026810: 6964 656f 732f 7761 7465 726d 6172 6b2f  ideos/watermark/
-00026820: 546f 6765 7468 6572 5f31 5f70 6f77 6572  Together_1_power
-00026830: 706f 696e 7472 6561 6479 2e6d 7034 272c  pointready.mp4',
-00026840: 206f 7665 726c 6179 5f76 6964 656f 5f70   overlay_video_p
-00026850: 6174 683d 272f 5573 6572 732f 7369 6d6f  ath='/Users/simo
-00026860: 6e2f 4465 736b 746f 702f 7370 6c61 7368  n/Desktop/splash
-00026870: 2e70 6e67 272c 2070 6f73 6974 696f 6e3d  .png', position=
-00026880: 2774 6f70 5f6c 6566 7427 2c20 6f70 6163  'top_left', opac
-00026890: 6974 793d 312e 302c 2073 6361 6c65 3d30  ity=1.0, scale=0
-000268a0: 2e32 290a 2020 2020 2222 220a 0a20 2020  .2).    """..   
-000268b0: 2074 696d 6572 203d 2053 696d 6261 5469   timer = SimbaTi
-000268c0: 6d65 7228 7374 6172 743d 5472 7565 290a  mer(start=True).
-000268d0: 2020 2020 504f 5349 5449 4f4e 5320 3d20      POSITIONS = 
-000268e0: 5b27 746f 705f 6c65 6674 272c 2027 626f  ['top_left', 'bo
-000268f0: 7474 6f6d 5f72 6967 6874 272c 2027 746f  ttom_right', 'to
-00026900: 705f 7269 6768 7427 2c20 2762 6f74 746f  p_right', 'botto
-00026910: 6d5f 6c65 6674 272c 2027 6365 6e74 6572  m_left', 'center
-00026920: 275d 0a20 2020 2063 6865 636b 5f66 6c6f  '].    check_flo
-00026930: 6174 286e 616d 653d 6627 7b69 6e73 6574  at(name=f'{inset
-00026940: 5f6f 7665 726c 6179 5f76 6964 656f 2e5f  _overlay_video._
-00026950: 5f6e 616d 655f 5f7d 206f 7061 6369 7479  _name__} opacity
-00026960: 272c 2076 616c 7565 3d6f 7061 6369 7479  ', value=opacity
-00026970: 2c20 6d69 6e5f 7661 6c75 653d 302e 3030  , min_value=0.00
-00026980: 312c 206d 6178 5f76 616c 7565 3d31 2e30  1, max_value=1.0
-00026990: 290a 2020 2020 6368 6563 6b5f 666c 6f61  ).    check_floa
-000269a0: 7428 6e61 6d65 3d66 277b 696e 7365 745f  t(name=f'{inset_
-000269b0: 6f76 6572 6c61 795f 7669 6465 6f2e 5f5f  overlay_video.__
-000269c0: 6e61 6d65 5f5f 7d20 7363 616c 6527 2c20  name__} scale', 
-000269d0: 7661 6c75 653d 7363 616c 652c 206d 696e  value=scale, min
-000269e0: 5f76 616c 7565 3d30 2e30 3031 2c20 6d61  _value=0.001, ma
-000269f0: 785f 7661 6c75 653d 302e 3939 3929 0a20  x_value=0.999). 
-00026a00: 2020 2063 6865 636b 5f73 7472 286e 616d     check_str(nam
-00026a10: 653d 6627 7b69 6e73 6574 5f6f 7665 726c  e=f'{inset_overl
-00026a20: 6179 5f76 6964 656f 2e5f 5f6e 616d 655f  ay_video.__name_
-00026a30: 5f7d 2070 6f73 6974 696f 6e27 2c20 7661  _} position', va
-00026a40: 6c75 653d 706f 7369 7469 6f6e 2c20 6f70  lue=position, op
-00026a50: 7469 6f6e 733d 504f 5349 5449 4f4e 5329  tions=POSITIONS)
-00026a60: 0a20 2020 2063 6865 636b 5f66 696c 655f  .    check_file_
-00026a70: 6578 6973 745f 616e 645f 7265 6164 6162  exist_and_readab
-00026a80: 6c65 2866 696c 655f 7061 7468 3d76 6964  le(file_path=vid
-00026a90: 656f 5f70 6174 6829 0a20 2020 2063 6865  eo_path).    che
-00026aa0: 636b 5f66 696c 655f 6578 6973 745f 616e  ck_file_exist_an
-00026ab0: 645f 7265 6164 6162 6c65 2866 696c 655f  d_readable(file_
-00026ac0: 7061 7468 3d6f 7665 726c 6179 5f76 6964  path=overlay_vid
-00026ad0: 656f 5f70 6174 6829 0a0a 2020 2020 6966  eo_path)..    if
-00026ae0: 206f 732e 7061 7468 2e69 7366 696c 6528   os.path.isfile(
-00026af0: 7669 6465 6f5f 7061 7468 293a 0a20 2020  video_path):.   
-00026b00: 2020 2020 2076 6964 656f 5f70 6174 6873       video_paths
-00026b10: 203d 205b 7669 6465 6f5f 7061 7468 5d0a   = [video_path].
-00026b20: 2020 2020 656c 6966 206f 732e 7061 7468      elif os.path
-00026b30: 2e69 7364 6972 2876 6964 656f 5f70 6174  .isdir(video_pat
-00026b40: 6829 3a0a 2020 2020 2020 2020 7669 6465  h):.        vide
-00026b50: 6f5f 7061 7468 7320 3d20 6c69 7374 2866  o_paths = list(f
-00026b60: 696e 645f 616c 6c5f 7669 6465 6f73 5f69  ind_all_videos_i
-00026b70: 6e5f 6469 7265 6374 6f72 7928 6469 7265  n_directory(dire
-00026b80: 6374 6f72 793d 7669 6465 6f5f 7061 7468  ctory=video_path
-00026b90: 2c20 6173 5f64 6963 743d 5472 7565 2c20  , as_dict=True, 
-00026ba0: 7261 6973 655f 6572 726f 723d 5472 7565  raise_error=True
-00026bb0: 292e 7661 6c75 6573 2829 290a 2020 2020  ).values()).    
-00026bc0: 656c 7365 3a0a 2020 2020 2020 2020 7261  else:.        ra
-00026bd0: 6973 6520 496e 7661 6c69 6449 6e70 7574  ise InvalidInput
-00026be0: 4572 726f 7228 6d73 673d 6627 7b76 6964  Error(msg=f'{vid
-00026bf0: 656f 5f70 6174 687d 2069 7320 6e6f 7420  eo_path} is not 
-00026c00: 6120 7661 6c69 6420 6669 6c65 2070 6174  a valid file pat
-00026c10: 6820 6f72 2061 2076 616c 6964 2064 6972  h or a valid dir
-00026c20: 6563 746f 7279 2070 6174 6827 2c0a 2020  ectory path',.  
-00026c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026c40: 2020 2020 2020 2020 2020 2020 2020 736f                so
-00026c50: 7572 6365 3d69 6e73 6574 5f6f 7665 726c  urce=inset_overl
-00026c60: 6179 5f76 6964 656f 2e5f 5f6e 616d 655f  ay_video.__name_
-00026c70: 5f29 0a20 2020 2069 6620 7361 7665 5f64  _).    if save_d
-00026c80: 6972 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ir is not None:.
-00026c90: 2020 2020 2020 2020 6368 6563 6b5f 6966          check_if
-00026ca0: 5f64 6972 5f65 7869 7374 7328 696e 5f64  _dir_exists(in_d
-00026cb0: 6972 3d73 6176 655f 6469 7229 0a20 2020  ir=save_dir).   
-00026cc0: 2065 6c73 653a 0a20 2020 2020 2020 2073   else:.        s
-00026cd0: 6176 655f 6469 7220 3d20 6f73 2e70 6174  ave_dir = os.pat
-00026ce0: 682e 6469 726e 616d 6528 7669 6465 6f5f  h.dirname(video_
-00026cf0: 7061 7468 735b 305d 290a 2020 2020 666f  paths[0]).    fo
-00026d00: 7220 6669 6c65 5f63 6e74 2c20 7669 6465  r file_cnt, vide
-00026d10: 6f5f 7061 7468 2069 6e20 656e 756d 6572  o_path in enumer
-00026d20: 6174 6528 7669 6465 6f5f 7061 7468 7329  ate(video_paths)
-00026d30: 3a0a 2020 2020 2020 2020 5f2c 2076 6964  :.        _, vid
-00026d40: 656f 5f6e 616d 652c 2076 6964 656f 5f65  eo_name, video_e
-00026d50: 7874 203d 2067 6574 5f66 6e5f 6578 7428  xt = get_fn_ext(
-00026d60: 7669 6465 6f5f 7061 7468 290a 2020 2020  video_path).    
-00026d70: 2020 2020 5f20 3d20 6765 745f 7669 6465      _ = get_vide
-00026d80: 6f5f 6d65 7461 5f64 6174 6128 7669 6465  o_meta_data(vide
-00026d90: 6f5f 7061 7468 3d76 6964 656f 5f70 6174  o_path=video_pat
-00026da0: 6829 0a20 2020 2020 2020 2070 7269 6e74  h).        print
-00026db0: 2866 2749 6e73 6572 7469 6e67 206f 7665  (f'Inserting ove
-00026dc0: 726c 6179 206f 6e74 6f20 7b76 6964 656f  rlay onto {video
-00026dd0: 5f6e 616d 657d 2028 5669 6465 6f20 7b66  _name} (Video {f
-00026de0: 696c 655f 636e 7420 2b20 317d 2f7b 6c65  ile_cnt + 1}/{le
-00026df0: 6e28 7669 6465 6f5f 7061 7468 7329 7d29  n(video_paths)})
-00026e00: 2e2e 2e27 290a 2020 2020 2020 2020 6f75  ...').        ou
-00026e10: 745f 7061 7468 203d 206f 732e 7061 7468  t_path = os.path
-00026e20: 2e6a 6f69 6e28 7361 7665 5f64 6972 2c20  .join(save_dir, 
-00026e30: 6627 7b76 6964 656f 5f6e 616d 657d 5f69  f'{video_name}_i
-00026e40: 6e73 6574 5f6f 7665 726c 6179 7b76 6964  nset_overlay{vid
-00026e50: 656f 5f65 7874 7d27 290a 2020 2020 2020  eo_ext}').      
-00026e60: 2020 7072 696e 7428 6f75 745f 7061 7468    print(out_path
-00026e70: 290a 2020 2020 2020 2020 6966 2070 6f73  ).        if pos
-00026e80: 6974 696f 6e20 3d3d 2050 4f53 4954 494f  ition == POSITIO
-00026e90: 4e53 5b30 5d3a 0a20 2020 2020 2020 2020  NS[0]:.         
-00026ea0: 2020 2063 6d64 203d 2066 2766 666d 7065     cmd = f'ffmpe
-00026eb0: 6720 2d69 2022 7b76 6964 656f 5f70 6174  g -i "{video_pat
-00026ec0: 687d 2220 2d69 2022 7b6f 7665 726c 6179  h}" -i "{overlay
-00026ed0: 5f76 6964 656f 5f70 6174 687d 2220 2d66  _video_path}" -f
-00026ee0: 696c 7465 725f 636f 6d70 6c65 7820 225b  ilter_complex "[
-00026ef0: 313a 765d 7363 616c 653d 6977 2a7b 7363  1:v]scale=iw*{sc
-00026f00: 616c 657d 3a2d 312c 666f 726d 6174 3d72  ale}:-1,format=r
-00026f10: 6762 612c 636f 6c6f 7263 6861 6e6e 656c  gba,colorchannel
-00026f20: 6d69 7865 723d 6161 3d7b 6f70 6163 6974  mixer=aa={opacit
-00026f30: 797d 5b69 6e73 6574 5d3b 5b30 3a76 5d5b  y}[inset];[0:v][
-00026f40: 696e 7365 745d 6f76 6572 6c61 793d 303a  inset]overlay=0:
-00026f50: 3022 2022 7b6f 7574 5f70 6174 687d 2220  0" "{out_path}" 
-00026f60: 2d79 270a 2020 2020 2020 2020 656c 6966  -y'.        elif
-00026f70: 2070 6f73 6974 696f 6e20 3d3d 2050 4f53   position == POS
-00026f80: 4954 494f 4e53 5b31 5d3a 0a20 2020 2020  ITIONS[1]:.     
-00026f90: 2020 2020 2020 2063 6d64 203d 2066 2766         cmd = f'f
-00026fa0: 666d 7065 6720 2d69 2022 7b76 6964 656f  fmpeg -i "{video
-00026fb0: 5f70 6174 687d 2220 2d69 2022 7b6f 7665  _path}" -i "{ove
-00026fc0: 726c 6179 5f76 6964 656f 5f70 6174 687d  rlay_video_path}
-00026fd0: 2220 2d66 696c 7465 725f 636f 6d70 6c65  " -filter_comple
-00026fe0: 7820 225b 313a 765d 7363 616c 653d 6977  x "[1:v]scale=iw
-00026ff0: 2a7b 7363 616c 657d 3a2d 312c 666f 726d  *{scale}:-1,form
-00027000: 6174 3d72 6762 612c 636f 6c6f 7263 6861  at=rgba,colorcha
-00027010: 6e6e 656c 6d69 7865 723d 6161 3d7b 6f70  nnelmixer=aa={op
-00027020: 6163 6974 797d 5b69 6e73 6574 5d3b 5b30  acity}[inset];[0
-00027030: 3a76 5d5b 696e 7365 745d 6f76 6572 6c61  :v][inset]overla
-00027040: 793d 572d 773a 482d 6822 2022 7b6f 7574  y=W-w:H-h" "{out
-00027050: 5f70 6174 687d 2220 2d79 270a 2020 2020  _path}" -y'.    
-00027060: 2020 2020 656c 6966 2070 6f73 6974 696f      elif positio
-00027070: 6e20 3d3d 2050 4f53 4954 494f 4e53 5b32  n == POSITIONS[2
-00027080: 5d3a 0a20 2020 2020 2020 2020 2020 2063  ]:.            c
-00027090: 6d64 203d 2066 2766 666d 7065 6720 2d69  md = f'ffmpeg -i
-000270a0: 2022 7b76 6964 656f 5f70 6174 687d 2220   "{video_path}" 
-000270b0: 2d69 2022 7b6f 7665 726c 6179 5f76 6964  -i "{overlay_vid
-000270c0: 656f 5f70 6174 687d 2220 2d66 696c 7465  eo_path}" -filte
-000270d0: 725f 636f 6d70 6c65 7820 225b 313a 765d  r_complex "[1:v]
-000270e0: 7363 616c 653d 6977 2a7b 7363 616c 657d  scale=iw*{scale}
-000270f0: 3a2d 312c 666f 726d 6174 3d72 6762 612c  :-1,format=rgba,
-00027100: 636f 6c6f 7263 6861 6e6e 656c 6d69 7865  colorchannelmixe
-00027110: 723d 6161 3d7b 6f70 6163 6974 797d 5b69  r=aa={opacity}[i
-00027120: 6e73 6574 5d3b 5b30 3a76 5d5b 696e 7365  nset];[0:v][inse
-00027130: 745d 6f76 6572 6c61 793d 572d 773a 3022  t]overlay=W-w:0"
-00027140: 2022 7b6f 7574 5f70 6174 687d 2220 2d79   "{out_path}" -y
-00027150: 270a 2020 2020 2020 2020 656c 6966 2070  '.        elif p
-00027160: 6f73 6974 696f 6e20 3d3d 2050 4f53 4954  osition == POSIT
-00027170: 494f 4e53 5b33 5d3a 0a20 2020 2020 2020  IONS[3]:.       
-00027180: 2020 2020 2063 6d64 203d 2066 2766 666d       cmd = f'ffm
-00027190: 7065 6720 2d69 2022 7b76 6964 656f 5f70  peg -i "{video_p
-000271a0: 6174 687d 2220 2d69 2022 7b6f 7665 726c  ath}" -i "{overl
-000271b0: 6179 5f76 6964 656f 5f70 6174 687d 2220  ay_video_path}" 
-000271c0: 2d66 696c 7465 725f 636f 6d70 6c65 7820  -filter_complex 
-000271d0: 225b 313a 765d 7363 616c 653d 6977 2a7b  "[1:v]scale=iw*{
-000271e0: 7363 616c 657d 3a2d 312c 666f 726d 6174  scale}:-1,format
-000271f0: 3d72 6762 612c 636f 6c6f 7263 6861 6e6e  =rgba,colorchann
-00027200: 656c 6d69 7865 723d 6161 3d7b 6f70 6163  elmixer=aa={opac
-00027210: 6974 797d 5b69 6e73 6574 5d3b 5b30 3a76  ity}[inset];[0:v
-00027220: 5d5b 696e 7365 745d 6f76 6572 6c61 793d  ][inset]overlay=
-00027230: 303a 482d 6822 2022 7b6f 7574 5f70 6174  0:H-h" "{out_pat
-00027240: 687d 2220 2d79 270a 2020 2020 2020 2020  h}" -y'.        
-00027250: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00027260: 2020 636d 6420 3d20 6627 6666 6d70 6567    cmd = f'ffmpeg
-00027270: 202d 6920 227b 7669 6465 6f5f 7061 7468   -i "{video_path
-00027280: 7d22 202d 6920 227b 6f76 6572 6c61 795f  }" -i "{overlay_
-00027290: 7669 6465 6f5f 7061 7468 7d22 202d 6669  video_path}" -fi
-000272a0: 6c74 6572 5f63 6f6d 706c 6578 2022 5b31  lter_complex "[1
-000272b0: 3a76 5d73 6361 6c65 3d69 772a 7b73 6361  :v]scale=iw*{sca
-000272c0: 6c65 7d3a 2d31 2c66 6f72 6d61 743d 7267  le}:-1,format=rg
-000272d0: 6261 2c63 6f6c 6f72 6368 616e 6e65 6c6d  ba,colorchannelm
-000272e0: 6978 6572 3d61 613d 7b6f 7061 6369 7479  ixer=aa={opacity
-000272f0: 7d5b 696e 7365 745d 3b5b 303a 765d 5b69  }[inset];[0:v][i
-00027300: 6e73 6574 5d6f 7665 726c 6179 3d28 572d  nset]overlay=(W-
-00027310: 7729 2f32 3a28 482d 6829 2f32 2220 227b  w)/2:(H-h)/2" "{
-00027320: 6f75 745f 7061 7468 7d22 202d 7927 0a20  out_path}" -y'. 
-00027330: 2020 2020 2020 2073 7562 7072 6f63 6573         subproces
-00027340: 732e 6361 6c6c 2863 6d64 2c20 7368 656c  s.call(cmd, shel
-00027350: 6c3d 5472 7565 2c20 7374 646f 7574 3d73  l=True, stdout=s
-00027360: 7562 7072 6f63 6573 732e 5049 5045 290a  ubprocess.PIPE).
-00027370: 2020 2020 7469 6d65 722e 7374 6f70 5f74      timer.stop_t
-00027380: 696d 6572 2829 0a20 2020 2073 7464 6f75  imer().    stdou
-00027390: 745f 7375 6363 6573 7328 6d73 673d 6627  t_success(msg=f'
-000273a0: 7b6c 656e 2876 6964 656f 5f70 6174 6873  {len(video_paths
-000273b0: 297d 206f 7665 726c 6179 2076 6964 656f  )} overlay video
-000273c0: 2873 2920 7361 7665 6420 696e 207b 7361  (s) saved in {sa
-000273d0: 7665 5f64 6972 7d27 2c20 656c 6170 7365  ve_dir}', elapse
-000273e0: 645f 7469 6d65 3d74 696d 6572 2e65 6c61  d_time=timer.ela
-000273f0: 7073 6564 5f74 696d 655f 7374 7229 0a0a  psed_time_str)..
-00027400: 6465 6620 726f 695f 626c 7572 626f 7828  def roi_blurbox(
-00027410: 7669 6465 6f5f 7061 7468 3a20 556e 696f  video_path: Unio
-00027420: 6e5b 7374 722c 206f 732e 5061 7468 4c69  n[str, os.PathLi
-00027430: 6b65 5d2c 0a20 2020 2020 2020 2020 2020  ke],.           
-00027440: 2020 2020 2062 6c75 725f 6c65 7665 6c3a       blur_level:
-00027450: 204f 7074 696f 6e61 6c5b 666c 6f61 745d   Optional[float]
-00027460: 203d 2030 2e30 322c 0a20 2020 2020 2020   = 0.02,.       
-00027470: 2020 2020 2020 2020 2069 6e76 6572 743a           invert:
-00027480: 204f 7074 696f 6e61 6c5b 626f 6f6c 5d20   Optional[bool] 
-00027490: 3d20 4661 6c73 652c 0a20 2020 2020 2020  = False,.       
-000274a0: 2020 2020 2020 2020 2073 6176 655f 7061           save_pa
-000274b0: 7468 3a20 4f70 7469 6f6e 616c 5b55 6e69  th: Optional[Uni
-000274c0: 6f6e 5b73 7472 2c20 6f73 2e50 6174 684c  on[str, os.PathL
-000274d0: 696b 655d 5d20 3d20 4e6f 6e65 2920 2d3e  ike]] = None) ->
-000274e0: 204e 6f6e 653a 0a0a 2020 2020 2222 220a   None:..    """.
-000274f0: 2020 2020 426c 7572 7320 6569 7468 6572      Blurs either
-00027500: 2074 6865 2073 656c 6563 7465 6420 6f72   the selected or
-00027510: 2075 6e73 656c 6563 7465 6420 706f 7274   unselected port
-00027520: 696f 6e20 6f66 2061 2075 7365 722d 7370  ion of a user-sp
-00027530: 6563 6966 6965 6420 7265 6769 6f6e 2d6f  ecified region-o
-00027540: 662d 696e 7465 7265 7374 2061 6363 6f72  f-interest accor
-00027550: 6469 6e67 2074 6f20 7468 6520 7061 7373  ding to the pass
-00027560: 6564 2062 6c75 7220 6c65 7665 6c2e 0a20  ed blur level.. 
-00027570: 2020 2048 6967 6865 7220 626c 7572 206c     Higher blur l
-00027580: 6576 656c 7320 7072 6f64 7563 6573 206d  evels produces m
-00027590: 6f72 6520 6f70 6171 7565 2072 6567 696f  ore opaque regio
-000275a0: 6e73 2e0a 0a20 2020 202e 2e20 7669 6465  ns...    .. vide
-000275b0: 6f3a 3a20 5f73 7461 7469 632f 696d 672f  o:: _static/img/
-000275c0: 726f 695f 626c 7572 626f 782e 7765 626d  roi_blurbox.webm
-000275d0: 0a20 2020 2020 2020 3a6c 6f6f 703a 0a0a  .       :loop:..
-000275e0: 2020 2020 3a70 6172 616d 2055 6e69 6f6e      :param Union
-000275f0: 5b73 7472 2c20 6f73 2e50 6174 684c 696b  [str, os.PathLik
-00027600: 655d 2076 6964 656f 5f70 6174 683a 2054  e] video_path: T
-00027610: 6865 2070 6174 6820 746f 2074 6865 2076  he path to the v
-00027620: 6964 656f 206f 6e20 6469 736b 0a20 2020  ideo on disk.   
-00027630: 203a 7061 7261 6d20 4f70 7469 6f6e 616c   :param Optional
-00027640: 5b66 6c6f 6174 5d20 626c 7572 5f6c 6576  [float] blur_lev
-00027650: 656c 3a20 5468 6520 6c65 7665 6c20 6f66  el: The level of
-00027660: 2074 6865 2062 6c75 7220 6173 2061 2072   the blur as a r
-00027670: 6174 696f 2030 2d31 2e30 2e0a 2020 2020  atio 0-1.0..    
-00027680: 3a70 6172 616d 204f 7074 696f 6e61 6c5b  :param Optional[
-00027690: 626f 6f6c 5d20 696e 7665 7274 3a20 4966  bool] invert: If
-000276a0: 2054 7275 652c 2062 6c75 7273 2074 6865   True, blurs the
-000276b0: 2075 6e73 656c 6563 7465 6420 7265 6769   unselected regi
-000276c0: 6f6e 2e20 4966 2046 616c 7365 2c20 626c  on. If False, bl
-000276d0: 7572 7320 7468 6520 7365 6c65 6374 6564  urs the selected
-000276e0: 2072 6567 696f 6e2e 0a20 2020 203a 7061   region..    :pa
-000276f0: 7261 6d20 4f70 7469 6f6e 616c 5b55 6e69  ram Optional[Uni
-00027700: 6f6e 5b73 7472 2c20 6f73 2e50 6174 684c  on[str, os.PathL
-00027710: 696b 655d 5d20 7361 7665 5f70 6174 683a  ike]] save_path:
-00027720: 2054 6865 206c 6f63 6174 696f 6e20 7768   The location wh
-00027730: 6572 6520 746f 2073 6176 6520 7468 6520  ere to save the 
-00027740: 626c 7572 7265 6420 7669 6465 6f2e 2049  blurred video. I
-00027750: 6620 4e6f 6e65 2c20 7468 656e 2073 6176  f None, then sav
-00027760: 6573 2074 6865 2062 6c75 7272 6564 2076  es the blurred v
-00027770: 6964 656f 2069 6e20 7468 6520 7361 6d65  ideo in the same
-00027780: 2064 6972 6563 746f 7279 2061 7320 7468   directory as th
-00027790: 6520 696e 7075 7420 7669 6465 6f20 7769  e input video wi
-000277a0: 7468 2074 6865 2060 605f 626c 7572 7265  th the ``_blurre
-000277b0: 6460 6020 7375 6666 6978 2e0a 2020 2020  d`` suffix..    
-000277c0: 3a72 6574 7572 6e3a 204e 6f6e 650a 0a20  :return: None.. 
-000277d0: 2020 203a 6578 616d 706c 653a 0a20 2020     :example:.   
-000277e0: 203e 3e3e 2072 6f69 5f62 6c75 7262 6f78   >>> roi_blurbox
-000277f0: 2876 6964 656f 5f70 6174 683d 272f 5573  (video_path='/Us
-00027800: 6572 732f 7369 6d6f 6e2f 446f 776e 6c6f  ers/simon/Downlo
-00027810: 6164 732f 315f 4c48 5f63 6c69 7070 6564  ads/1_LH_clipped
-00027820: 5f64 6f77 6e73 616d 706c 6564 2e6d 7034  _downsampled.mp4
-00027830: 272c 2062 6c75 725f 6c65 7665 6c3d 302e  ', blur_level=0.
-00027840: 322c 2069 6e76 6572 743d 5472 7565 290a  2, invert=True).
-00027850: 2020 2020 2222 220a 0a20 2020 2063 6865      """..    che
-00027860: 636b 5f66 666d 7065 675f 6176 6169 6c61  ck_ffmpeg_availa
-00027870: 626c 6528 7261 6973 655f 6572 726f 723d  ble(raise_error=
-00027880: 5472 7565 290a 2020 2020 7469 6d65 7220  True).    timer 
-00027890: 3d20 5369 6d62 6154 696d 6572 2873 7461  = SimbaTimer(sta
-000278a0: 7274 3d54 7275 6529 0a20 2020 2063 6865  rt=True).    che
-000278b0: 636b 5f66 6c6f 6174 286e 616d 653d 6627  ck_float(name=f'
-000278c0: 7b72 6f69 5f62 6c75 7262 6f78 2e5f 5f6e  {roi_blurbox.__n
-000278d0: 616d 655f 5f7d 2062 6c75 725f 6c65 7665  ame__} blur_leve
-000278e0: 6c27 2c20 7661 6c75 653d 626c 7572 5f6c  l', value=blur_l
-000278f0: 6576 656c 2c20 6d69 6e5f 7661 6c75 653d  evel, min_value=
-00027900: 302e 3030 312c 206d 6178 5f76 616c 7565  0.001, max_value
-00027910: 3d31 2e30 290a 2020 2020 6368 6563 6b5f  =1.0).    check_
-00027920: 6669 6c65 5f65 7869 7374 5f61 6e64 5f72  file_exist_and_r
-00027930: 6561 6461 626c 6528 6669 6c65 5f70 6174  eadable(file_pat
-00027940: 683d 7669 6465 6f5f 7061 7468 290a 2020  h=video_path).  
-00027950: 2020 6469 722c 2076 6964 656f 5f6e 616d    dir, video_nam
-00027960: 652c 2065 7874 203d 2067 6574 5f66 6e5f  e, ext = get_fn_
-00027970: 6578 7428 7669 6465 6f5f 7061 7468 290a  ext(video_path).
-00027980: 2020 2020 5f20 3d20 6765 745f 7669 6465      _ = get_vide
-00027990: 6f5f 6d65 7461 5f64 6174 6128 7669 6465  o_meta_data(vide
-000279a0: 6f5f 7061 7468 3d76 6964 656f 5f70 6174  o_path=video_pat
-000279b0: 6829 0a20 2020 2069 6620 7361 7665 5f70  h).    if save_p
-000279c0: 6174 6820 6973 206e 6f74 204e 6f6e 653a  ath is not None:
-000279d0: 0a20 2020 2020 2020 2063 6865 636b 5f69  .        check_i
-000279e0: 665f 6469 725f 6578 6973 7473 2869 6e5f  f_dir_exists(in_
-000279f0: 6469 723d 6f73 2e70 6174 682e 6469 726e  dir=os.path.dirn
-00027a00: 616d 6528 7361 7665 5f70 6174 6829 2c20  ame(save_path), 
-00027a10: 736f 7572 6365 3d72 6f69 5f62 6c75 7262  source=roi_blurb
-00027a20: 6f78 2e5f 5f6e 616d 655f 5f29 0a20 2020  ox.__name__).   
-00027a30: 2065 6c73 653a 0a20 2020 2020 2020 2073   else:.        s
-00027a40: 6176 655f 7061 7468 203d 206f 732e 7061  ave_path = os.pa
-00027a50: 7468 2e6a 6f69 6e28 6469 722c 2066 277b  th.join(dir, f'{
-00027a60: 7669 6465 6f5f 6e61 6d65 7d5f 626c 7572  video_name}_blur
-00027a70: 7265 647b 6578 747d 2729 0a20 2020 2072  red{ext}').    r
-00027a80: 6f69 5f73 656c 6563 746f 7220 3d20 524f  oi_selector = RO
-00027a90: 4953 656c 6563 746f 7228 7061 7468 3d76  ISelector(path=v
-00027aa0: 6964 656f 5f70 6174 6829 0a20 2020 2072  ideo_path).    r
-00027ab0: 6f69 5f73 656c 6563 746f 722e 7275 6e28  oi_selector.run(
-00027ac0: 290a 2020 2020 772c 2068 203d 2072 6f69  ).    w, h = roi
-00027ad0: 5f73 656c 6563 746f 722e 7769 6474 682c  _selector.width,
-00027ae0: 2072 6f69 5f73 656c 6563 746f 722e 6865   roi_selector.he
-00027af0: 6967 6874 0a20 2020 2074 6f70 5f6c 6566  ight.    top_lef
-00027b00: 745f 782c 2074 6f70 5f6c 6566 745f 7920  t_x, top_left_y 
-00027b10: 3d20 726f 695f 7365 6c65 6374 6f72 2e74  = roi_selector.t
-00027b20: 6f70 5f6c 6566 740a 2020 2020 6d61 785f  op_left.    max_
-00027b30: 626c 7572 5f76 616c 7565 203d 2069 6e74  blur_value = int
-00027b40: 286d 696e 2877 2c20 6829 202f 2032 2920  (min(w, h) / 2) 
-00027b50: 2f20 320a 2020 2020 626c 7572 5f6c 6576  / 2.    blur_lev
-00027b60: 656c 203d 2069 6e74 286d 6178 5f62 6c75  el = int(max_blu
-00027b70: 725f 7661 6c75 6520 2a20 626c 7572 5f6c  r_value * blur_l
-00027b80: 6576 656c 290a 2020 2020 6966 206e 6f74  evel).    if not
-00027b90: 2069 6e76 6572 743a 0a20 2020 2020 2020   invert:.       
-00027ba0: 2063 6d64 203d 2066 2766 666d 7065 6720   cmd = f'ffmpeg 
-00027bb0: 2d69 2022 7b76 6964 656f 5f70 6174 687d  -i "{video_path}
-00027bc0: 2220 2d66 696c 7465 725f 636f 6d70 6c65  " -filter_comple
-00027bd0: 7820 225b 303a 765d 6372 6f70 3d7b 777d  x "[0:v]crop={w}
-00027be0: 3a7b 687d 3a7b 746f 705f 6c65 6674 5f78  :{h}:{top_left_x
-00027bf0: 7d3a 7b74 6f70 5f6c 6566 745f 797d 2c62  }:{top_left_y},b
-00027c00: 6f78 626c 7572 3d7b 696e 7428 626c 7572  oxblur={int(blur
-00027c10: 5f6c 6576 656c 297d 3a31 305b 6667 5d3b  _level)}:10[fg];
-00027c20: 205b 303a 765d 5b66 675d 6f76 6572 6c61   [0:v][fg]overla
-00027c30: 793d 7b74 6f70 5f6c 6566 745f 787d 3a7b  y={top_left_x}:{
-00027c40: 746f 705f 6c65 6674 5f79 7d5b 765d 2220  top_left_y}[v]" 
-00027c50: 2d6d 6170 2022 5b76 5d22 2022 7b73 6176  -map "[v]" "{sav
-00027c60: 655f 7061 7468 7d22 202d 6c6f 676c 6576  e_path}" -loglev
-00027c70: 656c 2065 7272 6f72 202d 7374 6174 7320  el error -stats 
-00027c80: 2d68 6964 655f 6261 6e6e 6572 202d 7927  -hide_banner -y'
-00027c90: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
-00027ca0: 2020 2063 6d64 203d 2066 2766 666d 7065     cmd = f'ffmpe
-00027cb0: 6720 2d69 2022 7b76 6964 656f 5f70 6174  g -i "{video_pat
-00027cc0: 687d 2220 2d66 696c 7465 725f 636f 6d70  h}" -filter_comp
-00027cd0: 6c65 7820 225b 303a 765d 626f 7862 6c75  lex "[0:v]boxblu
-00027ce0: 723d 7b62 6c75 725f 6c65 7665 6c7d 5b62  r={blur_level}[b
-00027cf0: 675d 3b5b 303a 765d 6372 6f70 3d7b 777d  g];[0:v]crop={w}
-00027d00: 3a7b 687d 3a7b 746f 705f 6c65 6674 5f78  :{h}:{top_left_x
-00027d10: 7d3a 7b74 6f70 5f6c 6566 745f 797d 5b66  }:{top_left_y}[f
-00027d20: 675d 3b5b 6267 5d5b 6667 5d6f 7665 726c  g];[bg][fg]overl
-00027d30: 6179 3d7b 746f 705f 6c65 6674 5f78 7d3a  ay={top_left_x}:
-00027d40: 7b74 6f70 5f6c 6566 745f 797d 2220 2d63  {top_left_y}" -c
-00027d50: 3a61 2063 6f70 7920 227b 7361 7665 5f70  :a copy "{save_p
-00027d60: 6174 687d 2220 2d6c 6f67 6c65 7665 6c20  ath}" -loglevel 
-00027d70: 6572 726f 7220 2d73 7461 7473 202d 6869  error -stats -hi
-00027d80: 6465 5f62 616e 6e65 7220 2d79 270a 2020  de_banner -y'.  
-00027d90: 2020 7375 6270 726f 6365 7373 2e63 616c    subprocess.cal
-00027da0: 6c28 636d 642c 2073 6865 6c6c 3d54 7275  l(cmd, shell=Tru
-00027db0: 652c 2073 7464 6f75 743d 7375 6270 726f  e, stdout=subpro
-00027dc0: 6365 7373 2e50 4950 4529 0a20 2020 2074  cess.PIPE).    t
-00027dd0: 696d 6572 2e73 746f 705f 7469 6d65 7228  imer.stop_timer(
-00027de0: 290a 2020 2020 7374 646f 7574 5f73 7563  ).    stdout_suc
-00027df0: 6365 7373 286d 7367 3d66 2742 6c75 7272  cess(msg=f'Blurr
-00027e00: 6564 207b 7669 6465 6f5f 6e61 6d65 7d20  ed {video_name} 
-00027e10: 7669 6465 6f20 7361 7665 6420 696e 207b  video saved in {
-00027e20: 7361 7665 5f70 6174 687d 272c 2065 6c61  save_path}', ela
-00027e30: 7073 6564 5f74 696d 653d 7469 6d65 722e  psed_time=timer.
-00027e40: 656c 6170 7365 645f 7469 6d65 5f73 7472  elapsed_time_str
-00027e50: 290a 0a0a 6465 6620 7375 7065 7269 6d70  )...def superimp
-00027e60: 6f73 655f 656c 6170 7365 645f 7469 6d65  ose_elapsed_time
-00027e70: 2876 6964 656f 5f70 6174 683a 2055 6e69  (video_path: Uni
-00027e80: 6f6e 5b73 7472 2c20 6f73 2e50 6174 684c  on[str, os.PathL
-00027e90: 696b 655d 2c0a 2020 2020 2020 2020 2020  ike],.          
-00027ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027eb0: 2020 2066 6f6e 745f 7369 7a65 3a20 4f70     font_size: Op
-00027ec0: 7469 6f6e 616c 5b69 6e74 5d20 3d20 3330  tional[int] = 30
-00027ed0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00027ee0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00027ef0: 6f6e 745f 636f 6c6f 723a 204f 7074 696f  ont_color: Optio
-00027f00: 6e61 6c5b 7374 725d 203d 2027 7768 6974  nal[str] = 'whit
-00027f10: 6527 2c0a 2020 2020 2020 2020 2020 2020  e',.            
-00027f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027f30: 2066 6f6e 745f 626f 7264 6572 5f63 6f6c   font_border_col
-00027f40: 6f72 3a20 4f70 7469 6f6e 616c 5b73 7472  or: Optional[str
-00027f50: 5d20 3d20 2762 6c61 636b 272c 0a20 2020  ] = 'black',.   
-00027f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027f70: 2020 2020 2020 2020 2020 666f 6e74 5f62            font_b
-00027f80: 6f72 6465 725f 7769 6474 683a 204f 7074  order_width: Opt
-00027f90: 696f 6e61 6c5b 696e 745d 203d 2032 2c0a  ional[int] = 2,.
+00026330: 206f 7061 6369 7479 3a20 4f70 7469 6f6e   opacity: Option
+00026340: 616c 5b66 6c6f 6174 5d20 3d20 302e 352c  al[float] = 0.5,
+00026350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00026360: 2020 2020 2020 2020 2073 6361 6c65 3a20           scale: 
+00026370: 4f70 7469 6f6e 616c 5b66 6c6f 6174 5d20  Optional[float] 
+00026380: 3d20 302e 3035 2c0a 2020 2020 2020 2020  = 0.05,.        
+00026390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000263a0: 7361 7665 5f64 6972 3a20 4f70 7469 6f6e  save_dir: Option
+000263b0: 616c 5b55 6e69 6f6e 5b73 7472 2c20 6f73  al[Union[str, os
+000263c0: 2e50 6174 684c 696b 655d 5d20 3d20 4e6f  .PathLike]] = No
+000263d0: 6e65 2920 2d3e 204e 6f6e 653a 0a20 2020  ne) -> None:.   
+000263e0: 2022 2222 0a20 2020 2049 6e73 6574 2061   """.    Inset a
+000263f0: 2076 6964 656f 206f 7665 726c 6179 206f   video overlay o
+00026400: 6e20 6120 7365 636f 6e64 2076 6964 656f  n a second video
+00026410: 2077 6974 6820 7370 6563 6966 6965 6420   with specified 
+00026420: 7369 7a65 2c20 6f70 6163 6974 792c 2061  size, opacity, a
+00026430: 6e64 206c 6f63 6174 696f 6e2e 0a0a 2020  nd location...  
+00026440: 2020 2e2e 2076 6964 656f 3a3a 205f 7374    .. video:: _st
+00026450: 6174 6963 2f69 6d67 2f69 6e73 6574 5f6f  atic/img/inset_o
+00026460: 7665 726c 6179 5f76 6964 656f 2e77 6562  verlay_video.web
+00026470: 6d0a 2020 2020 2020 203a 7769 6474 683a  m.       :width:
+00026480: 2037 3030 0a20 2020 2020 2020 3a6c 6f6f   700.       :loo
+00026490: 703a 0a0a 2020 2020 3a70 6172 616d 2055  p:..    :param U
+000264a0: 6e69 6f6e 5b73 7472 2c20 6f73 2e50 6174  nion[str, os.Pat
+000264b0: 684c 696b 655d 2076 6964 656f 5f70 6174  hLike] video_pat
+000264c0: 683a 2054 6865 2070 6174 6820 746f 2074  h: The path to t
+000264d0: 6865 2076 6964 656f 2066 696c 652e 0a20  he video file.. 
+000264e0: 2020 203a 7061 7261 6d20 556e 696f 6e5b     :param Union[
+000264f0: 7374 722c 206f 732e 5061 7468 4c69 6b65  str, os.PathLike
+00026500: 5d20 6f76 6572 6c61 795f 7669 6465 6f5f  ] overlay_video_
+00026510: 7061 7468 3a20 5468 6520 7061 7468 2074  path: The path t
+00026520: 6f20 7669 6465 6f20 746f 2062 6520 696e  o video to be in
+00026530: 7365 7274 6564 2069 6e74 6f20 7468 6520  serted into the 
+00026540: 6060 7669 6465 6f5f 7061 7468 6060 2076  ``video_path`` v
+00026550: 6964 656f 2e0a 2020 2020 3a70 6172 616d  ideo..    :param
+00026560: 204f 7074 696f 6e61 6c5b 7374 725d 2070   Optional[str] p
+00026570: 6f73 6974 696f 6e3a 2054 6865 2070 6f73  osition: The pos
+00026580: 6974 696f 6e20 6f66 2074 6865 2069 6e73  ition of the ins
+00026590: 6574 206f 7665 726c 6179 2076 6964 656f  et overlay video
+000265a0: 2e20 4f70 7469 6f6e 733a 2027 746f 705f  . Options: 'top_
+000265b0: 6c65 6674 272c 2027 626f 7474 6f6d 5f72  left', 'bottom_r
+000265c0: 6967 6874 272c 2027 746f 705f 7269 6768  ight', 'top_righ
+000265d0: 7427 2c20 2762 6f74 746f 6d5f 6c65 6674  t', 'bottom_left
+000265e0: 272c 2027 6365 6e74 6572 270a 2020 2020  ', 'center'.    
+000265f0: 3a70 6172 616d 204f 7074 696f 6e61 6c5b  :param Optional[
+00026600: 666c 6f61 745d 206f 7061 6369 7479 3a20  float] opacity: 
+00026610: 5468 6520 6f70 6163 6974 7920 6f66 2074  The opacity of t
+00026620: 6865 2069 6e73 6574 206f 7665 726c 6179  he inset overlay
+00026630: 2076 6964 656f 2061 7320 6120 7661 6c75   video as a valu
+00026640: 6520 6265 7477 6565 6e20 302d 312e 302e  e between 0-1.0.
+00026650: 2031 2e30 206d 6561 6e69 6e67 2074 6865   1.0 meaning the
+00026660: 2073 616d 6520 6173 2069 6e70 7574 2069   same as input i
+00026670: 6d61 6765 2e20 4465 6661 756c 743a 2030  mage. Default: 0
+00026680: 2e35 2e0a 2020 2020 3a70 6172 616d 204f  .5..    :param O
+00026690: 7074 696f 6e61 6c5b 666c 6f61 745d 2073  ptional[float] s
+000266a0: 6361 6c65 3a20 5468 6520 7363 616c 6520  cale: The scale 
+000266b0: 6f66 2074 6865 2069 6e73 6574 206f 7665  of the inset ove
+000266c0: 726c 6179 2076 6964 656f 2061 7320 6120  rlay video as a 
+000266d0: 7261 7469 6f20 6f73 2074 6865 2069 6d61  ratio os the ima
+000266e0: 6765 2073 697a 652e 2044 6566 6175 6c74  ge size. Default
+000266f0: 3a20 302e 3035 2e0a 2020 2020 3a70 6172  : 0.05..    :par
+00026700: 616d 204f 7074 696f 6e61 6c5b 556e 696f  am Optional[Unio
+00026710: 6e5b 7374 722c 206f 732e 5061 7468 4c69  n[str, os.PathLi
+00026720: 6b65 5d5d 2073 6176 655f 6469 723a 2054  ke]] save_dir: T
+00026730: 6865 206c 6f63 6174 696f 6e20 7768 6572  he location wher
+00026740: 6520 746f 2073 6176 6520 7468 6520 6f75  e to save the ou
+00026750: 7470 7574 2076 6964 656f 2e20 4966 204e  tput video. If N
+00026760: 6f6e 652c 2074 6865 6e20 7361 7665 7320  one, then saves 
+00026770: 7468 6520 7669 6465 6f20 696e 2074 6865  the video in the
+00026780: 2073 616d 6520 6469 7265 6374 6f72 7920   same directory 
+00026790: 6173 2074 6865 2066 6972 7374 2076 6964  as the first vid
+000267a0: 656f 2e0a 2020 2020 3a72 6574 7572 6e3a  eo..    :return:
+000267b0: 204e 6f6e 650a 0a20 2020 203a 6578 616d   None..    :exam
+000267c0: 706c 653a 0a20 2020 203e 3e3e 2069 6e73  ple:.    >>> ins
+000267d0: 6574 5f6f 7665 726c 6179 5f76 6964 656f  et_overlay_video
+000267e0: 2876 6964 656f 5f70 6174 683d 272f 5573  (video_path='/Us
+000267f0: 6572 732f 7369 6d6f 6e2f 4465 736b 746f  ers/simon/Deskto
+00026800: 702f 656e 7673 2f73 696d 6261 2f74 726f  p/envs/simba/tro
+00026810: 7562 6c65 7368 6f6f 7469 6e67 2f6d 756c  ubleshooting/mul
+00026820: 7469 5f61 6e69 6d61 6c5f 646c 635f 7477  ti_animal_dlc_tw
+00026830: 6f5f 6335 372f 7072 6f6a 6563 745f 666f  o_c57/project_fo
+00026840: 6c64 6572 2f76 6964 656f 732f 7761 7465  lder/videos/wate
+00026850: 726d 6172 6b2f 546f 6765 7468 6572 5f31  rmark/Together_1
+00026860: 5f70 6f77 6572 706f 696e 7472 6561 6479  _powerpointready
+00026870: 2e6d 7034 272c 206f 7665 726c 6179 5f76  .mp4', overlay_v
+00026880: 6964 656f 5f70 6174 683d 272f 5573 6572  ideo_path='/User
+00026890: 732f 7369 6d6f 6e2f 4465 736b 746f 702f  s/simon/Desktop/
+000268a0: 7370 6c61 7368 2e70 6e67 272c 2070 6f73  splash.png', pos
+000268b0: 6974 696f 6e3d 2774 6f70 5f6c 6566 7427  ition='top_left'
+000268c0: 2c20 6f70 6163 6974 793d 312e 302c 2073  , opacity=1.0, s
+000268d0: 6361 6c65 3d30 2e32 290a 2020 2020 2222  cale=0.2).    ""
+000268e0: 220a 0a20 2020 2074 696d 6572 203d 2053  "..    timer = S
+000268f0: 696d 6261 5469 6d65 7228 7374 6172 743d  imbaTimer(start=
+00026900: 5472 7565 290a 2020 2020 504f 5349 5449  True).    POSITI
+00026910: 4f4e 5320 3d20 5b27 746f 705f 6c65 6674  ONS = ['top_left
+00026920: 272c 2027 626f 7474 6f6d 5f72 6967 6874  ', 'bottom_right
+00026930: 272c 2027 746f 705f 7269 6768 7427 2c20  ', 'top_right', 
+00026940: 2762 6f74 746f 6d5f 6c65 6674 272c 2027  'bottom_left', '
+00026950: 6365 6e74 6572 275d 0a20 2020 2063 6865  center'].    che
+00026960: 636b 5f66 6c6f 6174 286e 616d 653d 6627  ck_float(name=f'
+00026970: 7b69 6e73 6574 5f6f 7665 726c 6179 5f76  {inset_overlay_v
+00026980: 6964 656f 2e5f 5f6e 616d 655f 5f7d 206f  ideo.__name__} o
+00026990: 7061 6369 7479 272c 2076 616c 7565 3d6f  pacity', value=o
+000269a0: 7061 6369 7479 2c20 6d69 6e5f 7661 6c75  pacity, min_valu
+000269b0: 653d 302e 3030 312c 206d 6178 5f76 616c  e=0.001, max_val
+000269c0: 7565 3d31 2e30 290a 2020 2020 6368 6563  ue=1.0).    chec
+000269d0: 6b5f 666c 6f61 7428 6e61 6d65 3d66 277b  k_float(name=f'{
+000269e0: 696e 7365 745f 6f76 6572 6c61 795f 7669  inset_overlay_vi
+000269f0: 6465 6f2e 5f5f 6e61 6d65 5f5f 7d20 7363  deo.__name__} sc
+00026a00: 616c 6527 2c20 7661 6c75 653d 7363 616c  ale', value=scal
+00026a10: 652c 206d 696e 5f76 616c 7565 3d30 2e30  e, min_value=0.0
+00026a20: 3031 2c20 6d61 785f 7661 6c75 653d 302e  01, max_value=0.
+00026a30: 3939 3929 0a20 2020 2063 6865 636b 5f73  999).    check_s
+00026a40: 7472 286e 616d 653d 6627 7b69 6e73 6574  tr(name=f'{inset
+00026a50: 5f6f 7665 726c 6179 5f76 6964 656f 2e5f  _overlay_video._
+00026a60: 5f6e 616d 655f 5f7d 2070 6f73 6974 696f  _name__} positio
+00026a70: 6e27 2c20 7661 6c75 653d 706f 7369 7469  n', value=positi
+00026a80: 6f6e 2c20 6f70 7469 6f6e 733d 504f 5349  on, options=POSI
+00026a90: 5449 4f4e 5329 0a20 2020 2063 6865 636b  TIONS).    check
+00026aa0: 5f66 696c 655f 6578 6973 745f 616e 645f  _file_exist_and_
+00026ab0: 7265 6164 6162 6c65 2866 696c 655f 7061  readable(file_pa
+00026ac0: 7468 3d76 6964 656f 5f70 6174 6829 0a20  th=video_path). 
+00026ad0: 2020 2063 6865 636b 5f66 696c 655f 6578     check_file_ex
+00026ae0: 6973 745f 616e 645f 7265 6164 6162 6c65  ist_and_readable
+00026af0: 2866 696c 655f 7061 7468 3d6f 7665 726c  (file_path=overl
+00026b00: 6179 5f76 6964 656f 5f70 6174 6829 0a0a  ay_video_path)..
+00026b10: 2020 2020 6966 206f 732e 7061 7468 2e69      if os.path.i
+00026b20: 7366 696c 6528 7669 6465 6f5f 7061 7468  sfile(video_path
+00026b30: 293a 0a20 2020 2020 2020 2076 6964 656f  ):.        video
+00026b40: 5f70 6174 6873 203d 205b 7669 6465 6f5f  _paths = [video_
+00026b50: 7061 7468 5d0a 2020 2020 656c 6966 206f  path].    elif o
+00026b60: 732e 7061 7468 2e69 7364 6972 2876 6964  s.path.isdir(vid
+00026b70: 656f 5f70 6174 6829 3a0a 2020 2020 2020  eo_path):.      
+00026b80: 2020 7669 6465 6f5f 7061 7468 7320 3d20    video_paths = 
+00026b90: 6c69 7374 2866 696e 645f 616c 6c5f 7669  list(find_all_vi
+00026ba0: 6465 6f73 5f69 6e5f 6469 7265 6374 6f72  deos_in_director
+00026bb0: 7928 6469 7265 6374 6f72 793d 7669 6465  y(directory=vide
+00026bc0: 6f5f 7061 7468 2c20 6173 5f64 6963 743d  o_path, as_dict=
+00026bd0: 5472 7565 2c20 7261 6973 655f 6572 726f  True, raise_erro
+00026be0: 723d 5472 7565 292e 7661 6c75 6573 2829  r=True).values()
+00026bf0: 290a 2020 2020 656c 7365 3a0a 2020 2020  ).    else:.    
+00026c00: 2020 2020 7261 6973 6520 496e 7661 6c69      raise Invali
+00026c10: 6449 6e70 7574 4572 726f 7228 6d73 673d  dInputError(msg=
+00026c20: 6627 7b76 6964 656f 5f70 6174 687d 2069  f'{video_path} i
+00026c30: 7320 6e6f 7420 6120 7661 6c69 6420 6669  s not a valid fi
+00026c40: 6c65 2070 6174 6820 6f72 2061 2076 616c  le path or a val
+00026c50: 6964 2064 6972 6563 746f 7279 2070 6174  id directory pat
+00026c60: 6827 2c0a 2020 2020 2020 2020 2020 2020  h',.            
+00026c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026c80: 2020 2020 736f 7572 6365 3d69 6e73 6574      source=inset
+00026c90: 5f6f 7665 726c 6179 5f76 6964 656f 2e5f  _overlay_video._
+00026ca0: 5f6e 616d 655f 5f29 0a20 2020 2069 6620  _name__).    if 
+00026cb0: 7361 7665 5f64 6972 2069 7320 6e6f 7420  save_dir is not 
+00026cc0: 4e6f 6e65 3a0a 2020 2020 2020 2020 6368  None:.        ch
+00026cd0: 6563 6b5f 6966 5f64 6972 5f65 7869 7374  eck_if_dir_exist
+00026ce0: 7328 696e 5f64 6972 3d73 6176 655f 6469  s(in_dir=save_di
+00026cf0: 7229 0a20 2020 2065 6c73 653a 0a20 2020  r).    else:.   
+00026d00: 2020 2020 2073 6176 655f 6469 7220 3d20       save_dir = 
+00026d10: 6f73 2e70 6174 682e 6469 726e 616d 6528  os.path.dirname(
+00026d20: 7669 6465 6f5f 7061 7468 735b 305d 290a  video_paths[0]).
+00026d30: 2020 2020 666f 7220 6669 6c65 5f63 6e74      for file_cnt
+00026d40: 2c20 7669 6465 6f5f 7061 7468 2069 6e20  , video_path in 
+00026d50: 656e 756d 6572 6174 6528 7669 6465 6f5f  enumerate(video_
+00026d60: 7061 7468 7329 3a0a 2020 2020 2020 2020  paths):.        
+00026d70: 5f2c 2076 6964 656f 5f6e 616d 652c 2076  _, video_name, v
+00026d80: 6964 656f 5f65 7874 203d 2067 6574 5f66  ideo_ext = get_f
+00026d90: 6e5f 6578 7428 7669 6465 6f5f 7061 7468  n_ext(video_path
+00026da0: 290a 2020 2020 2020 2020 5f20 3d20 6765  ).        _ = ge
+00026db0: 745f 7669 6465 6f5f 6d65 7461 5f64 6174  t_video_meta_dat
+00026dc0: 6128 7669 6465 6f5f 7061 7468 3d76 6964  a(video_path=vid
+00026dd0: 656f 5f70 6174 6829 0a20 2020 2020 2020  eo_path).       
+00026de0: 2070 7269 6e74 2866 2749 6e73 6572 7469   print(f'Inserti
+00026df0: 6e67 206f 7665 726c 6179 206f 6e74 6f20  ng overlay onto 
+00026e00: 7b76 6964 656f 5f6e 616d 657d 2028 5669  {video_name} (Vi
+00026e10: 6465 6f20 7b66 696c 655f 636e 7420 2b20  deo {file_cnt + 
+00026e20: 317d 2f7b 6c65 6e28 7669 6465 6f5f 7061  1}/{len(video_pa
+00026e30: 7468 7329 7d29 2e2e 2e27 290a 2020 2020  ths)})...').    
+00026e40: 2020 2020 6f75 745f 7061 7468 203d 206f      out_path = o
+00026e50: 732e 7061 7468 2e6a 6f69 6e28 7361 7665  s.path.join(save
+00026e60: 5f64 6972 2c20 6627 7b76 6964 656f 5f6e  _dir, f'{video_n
+00026e70: 616d 657d 5f69 6e73 6574 5f6f 7665 726c  ame}_inset_overl
+00026e80: 6179 7b76 6964 656f 5f65 7874 7d27 290a  ay{video_ext}').
+00026e90: 2020 2020 2020 2020 7072 696e 7428 6f75          print(ou
+00026ea0: 745f 7061 7468 290a 2020 2020 2020 2020  t_path).        
+00026eb0: 6966 2070 6f73 6974 696f 6e20 3d3d 2050  if position == P
+00026ec0: 4f53 4954 494f 4e53 5b30 5d3a 0a20 2020  OSITIONS[0]:.   
+00026ed0: 2020 2020 2020 2020 2063 6d64 203d 2066           cmd = f
+00026ee0: 2766 666d 7065 6720 2d69 2022 7b76 6964  'ffmpeg -i "{vid
+00026ef0: 656f 5f70 6174 687d 2220 2d69 2022 7b6f  eo_path}" -i "{o
+00026f00: 7665 726c 6179 5f76 6964 656f 5f70 6174  verlay_video_pat
+00026f10: 687d 2220 2d66 696c 7465 725f 636f 6d70  h}" -filter_comp
+00026f20: 6c65 7820 225b 313a 765d 7363 616c 653d  lex "[1:v]scale=
+00026f30: 6977 2a7b 7363 616c 657d 3a2d 312c 666f  iw*{scale}:-1,fo
+00026f40: 726d 6174 3d72 6762 612c 636f 6c6f 7263  rmat=rgba,colorc
+00026f50: 6861 6e6e 656c 6d69 7865 723d 6161 3d7b  hannelmixer=aa={
+00026f60: 6f70 6163 6974 797d 5b69 6e73 6574 5d3b  opacity}[inset];
+00026f70: 5b30 3a76 5d5b 696e 7365 745d 6f76 6572  [0:v][inset]over
+00026f80: 6c61 793d 303a 3022 2022 7b6f 7574 5f70  lay=0:0" "{out_p
+00026f90: 6174 687d 2220 2d79 270a 2020 2020 2020  ath}" -y'.      
+00026fa0: 2020 656c 6966 2070 6f73 6974 696f 6e20    elif position 
+00026fb0: 3d3d 2050 4f53 4954 494f 4e53 5b31 5d3a  == POSITIONS[1]:
+00026fc0: 0a20 2020 2020 2020 2020 2020 2063 6d64  .            cmd
+00026fd0: 203d 2066 2766 666d 7065 6720 2d69 2022   = f'ffmpeg -i "
+00026fe0: 7b76 6964 656f 5f70 6174 687d 2220 2d69  {video_path}" -i
+00026ff0: 2022 7b6f 7665 726c 6179 5f76 6964 656f   "{overlay_video
+00027000: 5f70 6174 687d 2220 2d66 696c 7465 725f  _path}" -filter_
+00027010: 636f 6d70 6c65 7820 225b 313a 765d 7363  complex "[1:v]sc
+00027020: 616c 653d 6977 2a7b 7363 616c 657d 3a2d  ale=iw*{scale}:-
+00027030: 312c 666f 726d 6174 3d72 6762 612c 636f  1,format=rgba,co
+00027040: 6c6f 7263 6861 6e6e 656c 6d69 7865 723d  lorchannelmixer=
+00027050: 6161 3d7b 6f70 6163 6974 797d 5b69 6e73  aa={opacity}[ins
+00027060: 6574 5d3b 5b30 3a76 5d5b 696e 7365 745d  et];[0:v][inset]
+00027070: 6f76 6572 6c61 793d 572d 773a 482d 6822  overlay=W-w:H-h"
+00027080: 2022 7b6f 7574 5f70 6174 687d 2220 2d79   "{out_path}" -y
+00027090: 270a 2020 2020 2020 2020 656c 6966 2070  '.        elif p
+000270a0: 6f73 6974 696f 6e20 3d3d 2050 4f53 4954  osition == POSIT
+000270b0: 494f 4e53 5b32 5d3a 0a20 2020 2020 2020  IONS[2]:.       
+000270c0: 2020 2020 2063 6d64 203d 2066 2766 666d       cmd = f'ffm
+000270d0: 7065 6720 2d69 2022 7b76 6964 656f 5f70  peg -i "{video_p
+000270e0: 6174 687d 2220 2d69 2022 7b6f 7665 726c  ath}" -i "{overl
+000270f0: 6179 5f76 6964 656f 5f70 6174 687d 2220  ay_video_path}" 
+00027100: 2d66 696c 7465 725f 636f 6d70 6c65 7820  -filter_complex 
+00027110: 225b 313a 765d 7363 616c 653d 6977 2a7b  "[1:v]scale=iw*{
+00027120: 7363 616c 657d 3a2d 312c 666f 726d 6174  scale}:-1,format
+00027130: 3d72 6762 612c 636f 6c6f 7263 6861 6e6e  =rgba,colorchann
+00027140: 656c 6d69 7865 723d 6161 3d7b 6f70 6163  elmixer=aa={opac
+00027150: 6974 797d 5b69 6e73 6574 5d3b 5b30 3a76  ity}[inset];[0:v
+00027160: 5d5b 696e 7365 745d 6f76 6572 6c61 793d  ][inset]overlay=
+00027170: 572d 773a 3022 2022 7b6f 7574 5f70 6174  W-w:0" "{out_pat
+00027180: 687d 2220 2d79 270a 2020 2020 2020 2020  h}" -y'.        
+00027190: 656c 6966 2070 6f73 6974 696f 6e20 3d3d  elif position ==
+000271a0: 2050 4f53 4954 494f 4e53 5b33 5d3a 0a20   POSITIONS[3]:. 
+000271b0: 2020 2020 2020 2020 2020 2063 6d64 203d             cmd =
+000271c0: 2066 2766 666d 7065 6720 2d69 2022 7b76   f'ffmpeg -i "{v
+000271d0: 6964 656f 5f70 6174 687d 2220 2d69 2022  ideo_path}" -i "
+000271e0: 7b6f 7665 726c 6179 5f76 6964 656f 5f70  {overlay_video_p
+000271f0: 6174 687d 2220 2d66 696c 7465 725f 636f  ath}" -filter_co
+00027200: 6d70 6c65 7820 225b 313a 765d 7363 616c  mplex "[1:v]scal
+00027210: 653d 6977 2a7b 7363 616c 657d 3a2d 312c  e=iw*{scale}:-1,
+00027220: 666f 726d 6174 3d72 6762 612c 636f 6c6f  format=rgba,colo
+00027230: 7263 6861 6e6e 656c 6d69 7865 723d 6161  rchannelmixer=aa
+00027240: 3d7b 6f70 6163 6974 797d 5b69 6e73 6574  ={opacity}[inset
+00027250: 5d3b 5b30 3a76 5d5b 696e 7365 745d 6f76  ];[0:v][inset]ov
+00027260: 6572 6c61 793d 303a 482d 6822 2022 7b6f  erlay=0:H-h" "{o
+00027270: 7574 5f70 6174 687d 2220 2d79 270a 2020  ut_path}" -y'.  
+00027280: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00027290: 2020 2020 2020 2020 636d 6420 3d20 6627          cmd = f'
+000272a0: 6666 6d70 6567 202d 6920 227b 7669 6465  ffmpeg -i "{vide
+000272b0: 6f5f 7061 7468 7d22 202d 6920 227b 6f76  o_path}" -i "{ov
+000272c0: 6572 6c61 795f 7669 6465 6f5f 7061 7468  erlay_video_path
+000272d0: 7d22 202d 6669 6c74 6572 5f63 6f6d 706c  }" -filter_compl
+000272e0: 6578 2022 5b31 3a76 5d73 6361 6c65 3d69  ex "[1:v]scale=i
+000272f0: 772a 7b73 6361 6c65 7d3a 2d31 2c66 6f72  w*{scale}:-1,for
+00027300: 6d61 743d 7267 6261 2c63 6f6c 6f72 6368  mat=rgba,colorch
+00027310: 616e 6e65 6c6d 6978 6572 3d61 613d 7b6f  annelmixer=aa={o
+00027320: 7061 6369 7479 7d5b 696e 7365 745d 3b5b  pacity}[inset];[
+00027330: 303a 765d 5b69 6e73 6574 5d6f 7665 726c  0:v][inset]overl
+00027340: 6179 3d28 572d 7729 2f32 3a28 482d 6829  ay=(W-w)/2:(H-h)
+00027350: 2f32 2220 227b 6f75 745f 7061 7468 7d22  /2" "{out_path}"
+00027360: 202d 7927 0a20 2020 2020 2020 2073 7562   -y'.        sub
+00027370: 7072 6f63 6573 732e 6361 6c6c 2863 6d64  process.call(cmd
+00027380: 2c20 7368 656c 6c3d 5472 7565 2c20 7374  , shell=True, st
+00027390: 646f 7574 3d73 7562 7072 6f63 6573 732e  dout=subprocess.
+000273a0: 5049 5045 290a 2020 2020 7469 6d65 722e  PIPE).    timer.
+000273b0: 7374 6f70 5f74 696d 6572 2829 0a20 2020  stop_timer().   
+000273c0: 2073 7464 6f75 745f 7375 6363 6573 7328   stdout_success(
+000273d0: 6d73 673d 6627 7b6c 656e 2876 6964 656f  msg=f'{len(video
+000273e0: 5f70 6174 6873 297d 206f 7665 726c 6179  _paths)} overlay
+000273f0: 2076 6964 656f 2873 2920 7361 7665 6420   video(s) saved 
+00027400: 696e 207b 7361 7665 5f64 6972 7d27 2c20  in {save_dir}', 
+00027410: 656c 6170 7365 645f 7469 6d65 3d74 696d  elapsed_time=tim
+00027420: 6572 2e65 6c61 7073 6564 5f74 696d 655f  er.elapsed_time_
+00027430: 7374 7229 0a0a 6465 6620 726f 695f 626c  str)..def roi_bl
+00027440: 7572 626f 7828 7669 6465 6f5f 7061 7468  urbox(video_path
+00027450: 3a20 556e 696f 6e5b 7374 722c 206f 732e  : Union[str, os.
+00027460: 5061 7468 4c69 6b65 5d2c 0a20 2020 2020  PathLike],.     
+00027470: 2020 2020 2020 2020 2020 2062 6c75 725f             blur_
+00027480: 6c65 7665 6c3a 204f 7074 696f 6e61 6c5b  level: Optional[
+00027490: 666c 6f61 745d 203d 2030 2e30 322c 0a20  float] = 0.02,. 
+000274a0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000274b0: 6e76 6572 743a 204f 7074 696f 6e61 6c5b  nvert: Optional[
+000274c0: 626f 6f6c 5d20 3d20 4661 6c73 652c 0a20  bool] = False,. 
+000274d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000274e0: 6176 655f 7061 7468 3a20 4f70 7469 6f6e  ave_path: Option
+000274f0: 616c 5b55 6e69 6f6e 5b73 7472 2c20 6f73  al[Union[str, os
+00027500: 2e50 6174 684c 696b 655d 5d20 3d20 4e6f  .PathLike]] = No
+00027510: 6e65 2920 2d3e 204e 6f6e 653a 0a0a 2020  ne) -> None:..  
+00027520: 2020 2222 220a 2020 2020 426c 7572 7320    """.    Blurs 
+00027530: 6569 7468 6572 2074 6865 2073 656c 6563  either the selec
+00027540: 7465 6420 6f72 2075 6e73 656c 6563 7465  ted or unselecte
+00027550: 6420 706f 7274 696f 6e20 6f66 2061 2075  d portion of a u
+00027560: 7365 722d 7370 6563 6966 6965 6420 7265  ser-specified re
+00027570: 6769 6f6e 2d6f 662d 696e 7465 7265 7374  gion-of-interest
+00027580: 2061 6363 6f72 6469 6e67 2074 6f20 7468   according to th
+00027590: 6520 7061 7373 6564 2062 6c75 7220 6c65  e passed blur le
+000275a0: 7665 6c2e 0a20 2020 2048 6967 6865 7220  vel..    Higher 
+000275b0: 626c 7572 206c 6576 656c 7320 7072 6f64  blur levels prod
+000275c0: 7563 6573 206d 6f72 6520 6f70 6171 7565  uces more opaque
+000275d0: 2072 6567 696f 6e73 2e0a 0a20 2020 202e   regions...    .
+000275e0: 2e20 7669 6465 6f3a 3a20 5f73 7461 7469  . video:: _stati
+000275f0: 632f 696d 672f 726f 695f 626c 7572 626f  c/img/roi_blurbo
+00027600: 782e 7765 626d 0a20 2020 2020 2020 3a6c  x.webm.       :l
+00027610: 6f6f 703a 0a0a 2020 2020 3a70 6172 616d  oop:..    :param
+00027620: 2055 6e69 6f6e 5b73 7472 2c20 6f73 2e50   Union[str, os.P
+00027630: 6174 684c 696b 655d 2076 6964 656f 5f70  athLike] video_p
+00027640: 6174 683a 2054 6865 2070 6174 6820 746f  ath: The path to
+00027650: 2074 6865 2076 6964 656f 206f 6e20 6469   the video on di
+00027660: 736b 0a20 2020 203a 7061 7261 6d20 4f70  sk.    :param Op
+00027670: 7469 6f6e 616c 5b66 6c6f 6174 5d20 626c  tional[float] bl
+00027680: 7572 5f6c 6576 656c 3a20 5468 6520 6c65  ur_level: The le
+00027690: 7665 6c20 6f66 2074 6865 2062 6c75 7220  vel of the blur 
+000276a0: 6173 2061 2072 6174 696f 2030 2d31 2e30  as a ratio 0-1.0
+000276b0: 2e0a 2020 2020 3a70 6172 616d 204f 7074  ..    :param Opt
+000276c0: 696f 6e61 6c5b 626f 6f6c 5d20 696e 7665  ional[bool] inve
+000276d0: 7274 3a20 4966 2054 7275 652c 2062 6c75  rt: If True, blu
+000276e0: 7273 2074 6865 2075 6e73 656c 6563 7465  rs the unselecte
+000276f0: 6420 7265 6769 6f6e 2e20 4966 2046 616c  d region. If Fal
+00027700: 7365 2c20 626c 7572 7320 7468 6520 7365  se, blurs the se
+00027710: 6c65 6374 6564 2072 6567 696f 6e2e 0a20  lected region.. 
+00027720: 2020 203a 7061 7261 6d20 4f70 7469 6f6e     :param Option
+00027730: 616c 5b55 6e69 6f6e 5b73 7472 2c20 6f73  al[Union[str, os
+00027740: 2e50 6174 684c 696b 655d 5d20 7361 7665  .PathLike]] save
+00027750: 5f70 6174 683a 2054 6865 206c 6f63 6174  _path: The locat
+00027760: 696f 6e20 7768 6572 6520 746f 2073 6176  ion where to sav
+00027770: 6520 7468 6520 626c 7572 7265 6420 7669  e the blurred vi
+00027780: 6465 6f2e 2049 6620 4e6f 6e65 2c20 7468  deo. If None, th
+00027790: 656e 2073 6176 6573 2074 6865 2062 6c75  en saves the blu
+000277a0: 7272 6564 2076 6964 656f 2069 6e20 7468  rred video in th
+000277b0: 6520 7361 6d65 2064 6972 6563 746f 7279  e same directory
+000277c0: 2061 7320 7468 6520 696e 7075 7420 7669   as the input vi
+000277d0: 6465 6f20 7769 7468 2074 6865 2060 605f  deo with the ``_
+000277e0: 626c 7572 7265 6460 6020 7375 6666 6978  blurred`` suffix
+000277f0: 2e0a 2020 2020 3a72 6574 7572 6e3a 204e  ..    :return: N
+00027800: 6f6e 650a 0a20 2020 203a 6578 616d 706c  one..    :exampl
+00027810: 653a 0a20 2020 203e 3e3e 2072 6f69 5f62  e:.    >>> roi_b
+00027820: 6c75 7262 6f78 2876 6964 656f 5f70 6174  lurbox(video_pat
+00027830: 683d 272f 5573 6572 732f 7369 6d6f 6e2f  h='/Users/simon/
+00027840: 446f 776e 6c6f 6164 732f 315f 4c48 5f63  Downloads/1_LH_c
+00027850: 6c69 7070 6564 5f64 6f77 6e73 616d 706c  lipped_downsampl
+00027860: 6564 2e6d 7034 272c 2062 6c75 725f 6c65  ed.mp4', blur_le
+00027870: 7665 6c3d 302e 322c 2069 6e76 6572 743d  vel=0.2, invert=
+00027880: 5472 7565 290a 2020 2020 2222 220a 0a20  True).    """.. 
+00027890: 2020 2063 6865 636b 5f66 666d 7065 675f     check_ffmpeg_
+000278a0: 6176 6169 6c61 626c 6528 7261 6973 655f  available(raise_
+000278b0: 6572 726f 723d 5472 7565 290a 2020 2020  error=True).    
+000278c0: 7469 6d65 7220 3d20 5369 6d62 6154 696d  timer = SimbaTim
+000278d0: 6572 2873 7461 7274 3d54 7275 6529 0a20  er(start=True). 
+000278e0: 2020 2063 6865 636b 5f66 6c6f 6174 286e     check_float(n
+000278f0: 616d 653d 6627 7b72 6f69 5f62 6c75 7262  ame=f'{roi_blurb
+00027900: 6f78 2e5f 5f6e 616d 655f 5f7d 2062 6c75  ox.__name__} blu
+00027910: 725f 6c65 7665 6c27 2c20 7661 6c75 653d  r_level', value=
+00027920: 626c 7572 5f6c 6576 656c 2c20 6d69 6e5f  blur_level, min_
+00027930: 7661 6c75 653d 302e 3030 312c 206d 6178  value=0.001, max
+00027940: 5f76 616c 7565 3d31 2e30 290a 2020 2020  _value=1.0).    
+00027950: 6368 6563 6b5f 6669 6c65 5f65 7869 7374  check_file_exist
+00027960: 5f61 6e64 5f72 6561 6461 626c 6528 6669  _and_readable(fi
+00027970: 6c65 5f70 6174 683d 7669 6465 6f5f 7061  le_path=video_pa
+00027980: 7468 290a 2020 2020 6469 722c 2076 6964  th).    dir, vid
+00027990: 656f 5f6e 616d 652c 2065 7874 203d 2067  eo_name, ext = g
+000279a0: 6574 5f66 6e5f 6578 7428 7669 6465 6f5f  et_fn_ext(video_
+000279b0: 7061 7468 290a 2020 2020 5f20 3d20 6765  path).    _ = ge
+000279c0: 745f 7669 6465 6f5f 6d65 7461 5f64 6174  t_video_meta_dat
+000279d0: 6128 7669 6465 6f5f 7061 7468 3d76 6964  a(video_path=vid
+000279e0: 656f 5f70 6174 6829 0a20 2020 2069 6620  eo_path).    if 
+000279f0: 7361 7665 5f70 6174 6820 6973 206e 6f74  save_path is not
+00027a00: 204e 6f6e 653a 0a20 2020 2020 2020 2063   None:.        c
+00027a10: 6865 636b 5f69 665f 6469 725f 6578 6973  heck_if_dir_exis
+00027a20: 7473 2869 6e5f 6469 723d 6f73 2e70 6174  ts(in_dir=os.pat
+00027a30: 682e 6469 726e 616d 6528 7361 7665 5f70  h.dirname(save_p
+00027a40: 6174 6829 2c20 736f 7572 6365 3d72 6f69  ath), source=roi
+00027a50: 5f62 6c75 7262 6f78 2e5f 5f6e 616d 655f  _blurbox.__name_
+00027a60: 5f29 0a20 2020 2065 6c73 653a 0a20 2020  _).    else:.   
+00027a70: 2020 2020 2073 6176 655f 7061 7468 203d       save_path =
+00027a80: 206f 732e 7061 7468 2e6a 6f69 6e28 6469   os.path.join(di
+00027a90: 722c 2066 277b 7669 6465 6f5f 6e61 6d65  r, f'{video_name
+00027aa0: 7d5f 626c 7572 7265 647b 6578 747d 2729  }_blurred{ext}')
+00027ab0: 0a20 2020 2072 6f69 5f73 656c 6563 746f  .    roi_selecto
+00027ac0: 7220 3d20 524f 4953 656c 6563 746f 7228  r = ROISelector(
+00027ad0: 7061 7468 3d76 6964 656f 5f70 6174 6829  path=video_path)
+00027ae0: 0a20 2020 2072 6f69 5f73 656c 6563 746f  .    roi_selecto
+00027af0: 722e 7275 6e28 290a 2020 2020 772c 2068  r.run().    w, h
+00027b00: 203d 2072 6f69 5f73 656c 6563 746f 722e   = roi_selector.
+00027b10: 7769 6474 682c 2072 6f69 5f73 656c 6563  width, roi_selec
+00027b20: 746f 722e 6865 6967 6874 0a20 2020 2074  tor.height.    t
+00027b30: 6f70 5f6c 6566 745f 782c 2074 6f70 5f6c  op_left_x, top_l
+00027b40: 6566 745f 7920 3d20 726f 695f 7365 6c65  eft_y = roi_sele
+00027b50: 6374 6f72 2e74 6f70 5f6c 6566 740a 2020  ctor.top_left.  
+00027b60: 2020 6d61 785f 626c 7572 5f76 616c 7565    max_blur_value
+00027b70: 203d 2069 6e74 286d 696e 2877 2c20 6829   = int(min(w, h)
+00027b80: 202f 2032 2920 2f20 320a 2020 2020 626c   / 2) / 2.    bl
+00027b90: 7572 5f6c 6576 656c 203d 2069 6e74 286d  ur_level = int(m
+00027ba0: 6178 5f62 6c75 725f 7661 6c75 6520 2a20  ax_blur_value * 
+00027bb0: 626c 7572 5f6c 6576 656c 290a 2020 2020  blur_level).    
+00027bc0: 6966 206e 6f74 2069 6e76 6572 743a 0a20  if not invert:. 
+00027bd0: 2020 2020 2020 2063 6d64 203d 2066 2766         cmd = f'f
+00027be0: 666d 7065 6720 2d69 2022 7b76 6964 656f  fmpeg -i "{video
+00027bf0: 5f70 6174 687d 2220 2d66 696c 7465 725f  _path}" -filter_
+00027c00: 636f 6d70 6c65 7820 225b 303a 765d 6372  complex "[0:v]cr
+00027c10: 6f70 3d7b 777d 3a7b 687d 3a7b 746f 705f  op={w}:{h}:{top_
+00027c20: 6c65 6674 5f78 7d3a 7b74 6f70 5f6c 6566  left_x}:{top_lef
+00027c30: 745f 797d 2c62 6f78 626c 7572 3d7b 696e  t_y},boxblur={in
+00027c40: 7428 626c 7572 5f6c 6576 656c 297d 3a31  t(blur_level)}:1
+00027c50: 305b 6667 5d3b 205b 303a 765d 5b66 675d  0[fg]; [0:v][fg]
+00027c60: 6f76 6572 6c61 793d 7b74 6f70 5f6c 6566  overlay={top_lef
+00027c70: 745f 787d 3a7b 746f 705f 6c65 6674 5f79  t_x}:{top_left_y
+00027c80: 7d5b 765d 2220 2d6d 6170 2022 5b76 5d22  }[v]" -map "[v]"
+00027c90: 2022 7b73 6176 655f 7061 7468 7d22 202d   "{save_path}" -
+00027ca0: 6c6f 676c 6576 656c 2065 7272 6f72 202d  loglevel error -
+00027cb0: 7374 6174 7320 2d68 6964 655f 6261 6e6e  stats -hide_bann
+00027cc0: 6572 202d 7927 0a20 2020 2065 6c73 653a  er -y'.    else:
+00027cd0: 0a20 2020 2020 2020 2063 6d64 203d 2066  .        cmd = f
+00027ce0: 2766 666d 7065 6720 2d69 2022 7b76 6964  'ffmpeg -i "{vid
+00027cf0: 656f 5f70 6174 687d 2220 2d66 696c 7465  eo_path}" -filte
+00027d00: 725f 636f 6d70 6c65 7820 225b 303a 765d  r_complex "[0:v]
+00027d10: 626f 7862 6c75 723d 7b62 6c75 725f 6c65  boxblur={blur_le
+00027d20: 7665 6c7d 5b62 675d 3b5b 303a 765d 6372  vel}[bg];[0:v]cr
+00027d30: 6f70 3d7b 777d 3a7b 687d 3a7b 746f 705f  op={w}:{h}:{top_
+00027d40: 6c65 6674 5f78 7d3a 7b74 6f70 5f6c 6566  left_x}:{top_lef
+00027d50: 745f 797d 5b66 675d 3b5b 6267 5d5b 6667  t_y}[fg];[bg][fg
+00027d60: 5d6f 7665 726c 6179 3d7b 746f 705f 6c65  ]overlay={top_le
+00027d70: 6674 5f78 7d3a 7b74 6f70 5f6c 6566 745f  ft_x}:{top_left_
+00027d80: 797d 2220 2d63 3a61 2063 6f70 7920 227b  y}" -c:a copy "{
+00027d90: 7361 7665 5f70 6174 687d 2220 2d6c 6f67  save_path}" -log
+00027da0: 6c65 7665 6c20 6572 726f 7220 2d73 7461  level error -sta
+00027db0: 7473 202d 6869 6465 5f62 616e 6e65 7220  ts -hide_banner 
+00027dc0: 2d79 270a 2020 2020 7375 6270 726f 6365  -y'.    subproce
+00027dd0: 7373 2e63 616c 6c28 636d 642c 2073 6865  ss.call(cmd, she
+00027de0: 6c6c 3d54 7275 652c 2073 7464 6f75 743d  ll=True, stdout=
+00027df0: 7375 6270 726f 6365 7373 2e50 4950 4529  subprocess.PIPE)
+00027e00: 0a20 2020 2074 696d 6572 2e73 746f 705f  .    timer.stop_
+00027e10: 7469 6d65 7228 290a 2020 2020 7374 646f  timer().    stdo
+00027e20: 7574 5f73 7563 6365 7373 286d 7367 3d66  ut_success(msg=f
+00027e30: 2742 6c75 7272 6564 207b 7669 6465 6f5f  'Blurred {video_
+00027e40: 6e61 6d65 7d20 7669 6465 6f20 7361 7665  name} video save
+00027e50: 6420 696e 207b 7361 7665 5f70 6174 687d  d in {save_path}
+00027e60: 272c 2065 6c61 7073 6564 5f74 696d 653d  ', elapsed_time=
+00027e70: 7469 6d65 722e 656c 6170 7365 645f 7469  timer.elapsed_ti
+00027e80: 6d65 5f73 7472 290a 0a0a 6465 6620 7375  me_str)...def su
+00027e90: 7065 7269 6d70 6f73 655f 656c 6170 7365  perimpose_elapse
+00027ea0: 645f 7469 6d65 2876 6964 656f 5f70 6174  d_time(video_pat
+00027eb0: 683a 2055 6e69 6f6e 5b73 7472 2c20 6f73  h: Union[str, os
+00027ec0: 2e50 6174 684c 696b 655d 2c0a 2020 2020  .PathLike],.    
+00027ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027ee0: 2020 2020 2020 2020 2066 6f6e 745f 7369           font_si
+00027ef0: 7a65 3a20 4f70 7469 6f6e 616c 5b69 6e74  ze: Optional[int
+00027f00: 5d20 3d20 3330 2c0a 2020 2020 2020 2020  ] = 30,.        
+00027f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027f20: 2020 2020 2066 6f6e 745f 636f 6c6f 723a       font_color:
+00027f30: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
+00027f40: 2027 7768 6974 6527 2c0a 2020 2020 2020   'white',.      
+00027f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027f60: 2020 2020 2020 2066 6f6e 745f 626f 7264         font_bord
+00027f70: 6572 5f63 6f6c 6f72 3a20 4f70 7469 6f6e  er_color: Option
+00027f80: 616c 5b73 7472 5d20 3d20 2762 6c61 636b  al[str] = 'black
+00027f90: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
 00027fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027fb0: 2020 2020 2020 2020 2020 2020 2070 6f73               pos
-00027fc0: 6974 696f 6e3a 204f 7074 696f 6e61 6c5b  ition: Optional[
-00027fd0: 4c69 7465 7261 6c5b 2774 6f70 5f6c 6566  Literal['top_lef
-00027fe0: 7427 2c20 2774 6f70 5f72 6967 6874 272c  t', 'top_right',
-00027ff0: 2027 626f 7474 6f6d 5f6c 6566 7427 2c20   'bottom_left', 
-00028000: 2762 6f74 746f 6d5f 7269 6768 7427 2c20  'bottom_right', 
-00028010: 276d 6964 646c 655f 746f 7027 2c20 276d  'middle_top', 'm
-00028020: 6964 646c 655f 626f 7474 6f6d 275d 5d20  iddle_bottom']] 
-00028030: 3d20 2774 6f70 5f6c 6566 7427 2c0a 2020  = 'top_left',.  
-00028040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028050: 2020 2020 2020 2020 2020 2073 6176 655f             save_
-00028060: 6469 723a 204f 7074 696f 6e61 6c5b 556e  dir: Optional[Un
-00028070: 696f 6e5b 7374 722c 206f 732e 5061 7468  ion[str, os.Path
-00028080: 4c69 6b65 5d5d 203d 204e 6f6e 6529 202d  Like]] = None) -
-00028090: 3e20 4e6f 6e65 3a0a 2020 2020 2222 220a  > None:.    """.
-000280a0: 2020 2020 5375 7065 7269 6d70 6f73 6573      Superimposes
-000280b0: 2065 6c61 7073 6564 2074 696d 6520 6f6e   elapsed time on
-000280c0: 2074 6865 2067 6976 656e 2076 6964 656f   the given video
-000280d0: 2066 696c 6528 7329 2061 6e64 2073 6176   file(s) and sav
-000280e0: 6573 2074 6865 206d 6f64 6966 6965 6420  es the modified 
-000280f0: 7669 6465 6f28 7329 2e0a 0a20 2020 202e  video(s)...    .
-00028100: 2e20 7669 6465 6f3a 3a20 5f73 7461 7469  . video:: _stati
-00028110: 632f 696d 672f 7375 7065 7269 6d70 6f73  c/img/superimpos
-00028120: 655f 656c 6170 7365 645f 7469 6d65 2e77  e_elapsed_time.w
-00028130: 6562 6d0a 2020 2020 2020 203a 7769 6474  ebm.       :widt
-00028140: 683a 2039 3030 0a20 2020 2020 2020 3a6c  h: 900.       :l
-00028150: 6f6f 703a 0a0a 2020 2020 3a70 6172 616d  oop:..    :param
-00028160: 2055 6e69 6f6e 5b73 7472 2c20 6f73 2e50   Union[str, os.P
-00028170: 6174 684c 696b 655d 2076 6964 656f 5f70  athLike] video_p
-00028180: 6174 683a 2050 6174 6820 746f 2074 6865  ath: Path to the
-00028190: 2069 6e70 7574 2076 6964 656f 2066 696c   input video fil
-000281a0: 6520 6f72 2064 6972 6563 746f 7279 2063  e or directory c
-000281b0: 6f6e 7461 696e 696e 6720 7669 6465 6f20  ontaining video 
-000281c0: 6669 6c65 732e 0a20 2020 203a 7061 7261  files..    :para
-000281d0: 6d20 4f70 7469 6f6e 616c 5b69 6e74 5d20  m Optional[int] 
-000281e0: 666f 6e74 5f73 697a 653a 2046 6f6e 7420  font_size: Font 
-000281f0: 7369 7a65 2066 6f72 2074 6865 2065 6c61  size for the ela
-00028200: 7073 6564 2074 696d 6520 7465 7874 2e20  psed time text. 
-00028210: 4465 6661 756c 7420 3330 2e0a 2020 2020  Default 30..    
-00028220: 3a70 6172 616d 204f 7074 696f 6e61 6c5b  :param Optional[
-00028230: 7374 725d 2066 6f6e 745f 636f 6c6f 723a  str] font_color:
-00028240: 2020 466f 6e74 2063 6f6c 6f72 2066 6f72    Font color for
-00028250: 2074 6865 2065 6c61 7073 6564 2074 696d   the elapsed tim
-00028260: 6520 7465 7874 2e20 4465 6661 756c 7420  e text. Default 
-00028270: 7768 6974 650a 2020 2020 3a70 6172 616d  white.    :param
-00028280: 204f 7074 696f 6e61 6c5b 7374 725d 2066   Optional[str] f
-00028290: 6f6e 745f 626f 7264 6572 5f63 6f6c 6f72  ont_border_color
-000282a0: 3a20 466f 6e74 2062 6f72 6465 7220 636f  : Font border co
-000282b0: 6c6f 7220 666f 7220 7468 6520 656c 6170  lor for the elap
-000282c0: 7365 6420 7469 6d65 2074 6578 742e 2044  sed time text. D
-000282d0: 6566 6175 6c74 2062 6c61 636b 2e0a 2020  efault black..  
-000282e0: 2020 3a70 6172 616d 204f 7074 696f 6e61    :param Optiona
-000282f0: 6c5b 696e 745d 2066 6f6e 745f 626f 7264  l[int] font_bord
-00028300: 6572 5f77 6964 7468 3a20 466f 6e74 2062  er_width: Font b
-00028310: 6f72 6465 7220 7769 6474 6820 666f 7220  order width for 
-00028320: 7468 6520 656c 6170 7365 6420 7469 6d65  the elapsed time
-00028330: 2074 6578 7420 696e 2070 6978 656c 732e   text in pixels.
-00028340: 2044 6566 6175 6c74 2032 2e0a 2020 2020   Default 2..    
-00028350: 3a70 6172 616d 204f 7074 696f 6e61 6c5b  :param Optional[
-00028360: 4c69 7465 7261 6c5b 2774 6f70 5f6c 6566  Literal['top_lef
-00028370: 7427 2c20 2774 6f70 5f72 6967 6874 272c  t', 'top_right',
-00028380: 2027 626f 7474 6f6d 5f6c 6566 7427 2c20   'bottom_left', 
-00028390: 2762 6f74 746f 6d5f 7269 6768 7427 2c20  'bottom_right', 
-000283a0: 276d 6964 646c 655f 746f 7027 2c20 276d  'middle_top', 'm
-000283b0: 6964 646c 655f 626f 7474 6f6d 275d 5d20  iddle_bottom']] 
-000283c0: 706f 7369 7469 6f6e 3a20 506f 7369 7469  position: Positi
-000283d0: 6f6e 2077 6865 7265 2074 6865 2065 6c61  on where the ela
-000283e0: 7073 6564 2074 696d 6520 7465 7874 2077  psed time text w
-000283f0: 696c 6c20 6265 2073 7570 6572 696d 706f  ill be superimpo
-00028400: 7365 642e 2044 6566 6175 6c74 2060 6074  sed. Default ``t
-00028410: 6f70 5f6c 6566 7460 602e 0a20 2020 203a  op_left``..    :
-00028420: 7061 7261 6d20 4f70 7469 6f6e 616c 5b55  param Optional[U
-00028430: 6e69 6f6e 5b73 7472 2c20 6f73 2e50 6174  nion[str, os.Pat
-00028440: 684c 696b 655d 5d20 7361 7665 5f64 6972  hLike]] save_dir
-00028450: 3a20 4469 7265 6374 6f72 7920 7768 6572  : Directory wher
-00028460: 6520 7468 6520 6d6f 6469 6669 6564 2076  e the modified v
-00028470: 6964 656f 2873 2920 7769 6c6c 2062 6520  ideo(s) will be 
-00028480: 7361 7665 642e 2049 6620 6e6f 7420 7072  saved. If not pr
-00028490: 6f76 6964 6564 2c20 7468 6520 6469 7265  ovided, the dire
-000284a0: 6374 6f72 7920 6f66 2074 6865 2069 6e70  ctory of the inp
-000284b0: 7574 2076 6964 656f 2873 2920 7769 6c6c  ut video(s) will
-000284c0: 2062 6520 7573 6564 2e0a 2020 2020 3a72   be used..    :r
-000284d0: 6574 7572 6e3a 204e 6f6e 650a 0a20 2020  eturn: None..   
-000284e0: 203a 6578 616d 706c 653a 0a20 2020 203e   :example:.    >
-000284f0: 3e3e 2073 7570 6572 696d 706f 7365 5f65  >> superimpose_e
-00028500: 6c61 7073 6564 5f74 696d 6528 7669 6465  lapsed_time(vide
-00028510: 6f5f 7061 7468 3d27 2f55 7365 7273 2f73  o_path='/Users/s
-00028520: 696d 6f6e 2f44 6573 6b74 6f70 2f65 6e76  imon/Desktop/env
-00028530: 732f 7369 6d62 612f 7472 6f75 626c 6573  s/simba/troubles
-00028540: 686f 6f74 696e 672f 6d6f 7573 655f 6f70  hooting/mouse_op
-00028550: 656e 5f66 6965 6c64 2f70 726f 6a65 6374  en_field/project
-00028560: 5f66 6f6c 6465 722f 7669 6465 6f73 2f74  _folder/videos/t
-00028570: 6573 745f 342f 312e 6d70 3427 2c20 706f  est_4/1.mp4', po
-00028580: 7369 7469 6f6e 3d27 6d69 6464 6c65 5f74  sition='middle_t
-00028590: 6f70 272c 2066 6f6e 745f 636f 6c6f 723d  op', font_color=
-000285a0: 2762 6c61 636b 272c 2066 6f6e 745f 626f  'black', font_bo
-000285b0: 7264 6572 5f63 6f6c 6f72 3d27 7069 6e6b  rder_color='pink
-000285c0: 272c 2066 6f6e 745f 626f 7264 6572 5f77  ', font_border_w
-000285d0: 6964 7468 3d35 2c20 666f 6e74 5f73 697a  idth=5, font_siz
-000285e0: 653d 3330 290a 2020 2020 2222 220a 0a20  e=30).    """.. 
-000285f0: 2020 2063 6865 636b 5f66 666d 7065 675f     check_ffmpeg_
-00028600: 6176 6169 6c61 626c 6528 7261 6973 655f  available(raise_
-00028610: 6572 726f 723d 5472 7565 290a 2020 2020  error=True).    
-00028620: 7469 6d65 7220 3d20 5369 6d62 6154 696d  timer = SimbaTim
-00028630: 6572 2873 7461 7274 3d54 7275 6529 0a20  er(start=True). 
-00028640: 2020 2050 4f53 4954 494f 4e53 203d 205b     POSITIONS = [
-00028650: 2774 6f70 5f6c 6566 7427 2c20 2774 6f70  'top_left', 'top
-00028660: 5f72 6967 6874 272c 2027 626f 7474 6f6d  _right', 'bottom
-00028670: 5f6c 6566 7427 2c20 2762 6f74 746f 6d5f  _left', 'bottom_
-00028680: 7269 6768 7427 2c20 276d 6964 646c 655f  right', 'middle_
-00028690: 746f 7027 2c20 276d 6964 646c 655f 626f  top', 'middle_bo
-000286a0: 7474 6f6d 275d 0a20 2020 2063 6865 636b  ttom'].    check
-000286b0: 5f73 7472 286e 616d 653d 6627 7b73 7570  _str(name=f'{sup
-000286c0: 6572 696d 706f 7365 5f65 6c61 7073 6564  erimpose_elapsed
-000286d0: 5f74 696d 652e 5f5f 6e61 6d65 5f5f 7d20  _time.__name__} 
-000286e0: 706f 7369 7469 6f6e 272c 2076 616c 7565  position', value
-000286f0: 3d70 6f73 6974 696f 6e2c 206f 7074 696f  =position, optio
-00028700: 6e73 3d50 4f53 4954 494f 4e53 290a 2020  ns=POSITIONS).  
-00028710: 2020 6368 6563 6b5f 696e 7428 6e61 6d65    check_int(name
-00028720: 3d66 277b 7375 7065 7269 6d70 6f73 655f  =f'{superimpose_
-00028730: 656c 6170 7365 645f 7469 6d65 2e5f 5f6e  elapsed_time.__n
-00028740: 616d 655f 5f7d 2066 6f6e 745f 7369 7a65  ame__} font_size
-00028750: 272c 2076 616c 7565 3d66 6f6e 745f 7369  ', value=font_si
-00028760: 7a65 2c20 6d69 6e5f 7661 6c75 653d 3129  ze, min_value=1)
-00028770: 0a20 2020 2063 6865 636b 5f69 6e74 286e  .    check_int(n
-00028780: 616d 653d 6627 7b73 7570 6572 696d 706f  ame=f'{superimpo
-00028790: 7365 5f65 6c61 7073 6564 5f74 696d 652e  se_elapsed_time.
-000287a0: 5f5f 6e61 6d65 5f5f 7d20 666f 6e74 5f62  __name__} font_b
-000287b0: 6f72 6465 725f 7769 6474 6827 2c20 7661  order_width', va
-000287c0: 6c75 653d 666f 6e74 5f62 6f72 6465 725f  lue=font_border_
-000287d0: 7769 6474 682c 206d 696e 5f76 616c 7565  width, min_value
-000287e0: 3d31 290a 2020 2020 666f 6e74 5f63 6f6c  =1).    font_col
-000287f0: 6f72 203d 2027 272e 6a6f 696e 2866 696c  or = ''.join(fil
-00028800: 7465 7228 7374 722e 6973 616c 6e75 6d2c  ter(str.isalnum,
-00028810: 2066 6f6e 745f 636f 6c6f 7229 292e 6c6f   font_color)).lo
-00028820: 7765 7228 290a 2020 2020 666f 6e74 5f62  wer().    font_b
-00028830: 6f72 6465 725f 636f 6c6f 7220 3d20 2727  order_color = ''
-00028840: 2e6a 6f69 6e28 6669 6c74 6572 2873 7472  .join(filter(str
-00028850: 2e69 7361 6c6e 756d 2c20 666f 6e74 5f62  .isalnum, font_b
-00028860: 6f72 6465 725f 636f 6c6f 7229 292e 6c6f  order_color)).lo
-00028870: 7765 7228 290a 2020 2020 6966 206f 732e  wer().    if os.
-00028880: 7061 7468 2e69 7366 696c 6528 7669 6465  path.isfile(vide
-00028890: 6f5f 7061 7468 293a 0a20 2020 2020 2020  o_path):.       
-000288a0: 2076 6964 656f 5f70 6174 6873 203d 205b   video_paths = [
-000288b0: 7669 6465 6f5f 7061 7468 5d0a 2020 2020  video_path].    
-000288c0: 656c 6966 206f 732e 7061 7468 2e69 7364  elif os.path.isd
-000288d0: 6972 2876 6964 656f 5f70 6174 6829 3a0a  ir(video_path):.
-000288e0: 2020 2020 2020 2020 7669 6465 6f5f 7061          video_pa
-000288f0: 7468 7320 3d20 6c69 7374 2866 696e 645f  ths = list(find_
-00028900: 616c 6c5f 7669 6465 6f73 5f69 6e5f 6469  all_videos_in_di
-00028910: 7265 6374 6f72 7928 6469 7265 6374 6f72  rectory(director
-00028920: 793d 7669 6465 6f5f 7061 7468 2c20 6173  y=video_path, as
-00028930: 5f64 6963 743d 5472 7565 2c20 7261 6973  _dict=True, rais
-00028940: 655f 6572 726f 723d 5472 7565 292e 7661  e_error=True).va
-00028950: 6c75 6573 2829 290a 2020 2020 656c 7365  lues()).    else
-00028960: 3a0a 2020 2020 2020 2020 7261 6973 6520  :.        raise 
-00028970: 496e 7661 6c69 6449 6e70 7574 4572 726f  InvalidInputErro
-00028980: 7228 6d73 673d 6627 7b76 6964 656f 5f70  r(msg=f'{video_p
-00028990: 6174 687d 2069 7320 6e6f 7420 6120 7661  ath} is not a va
-000289a0: 6c69 6420 6669 6c65 2070 6174 6820 6f72  lid file path or
-000289b0: 2061 2076 616c 6964 2064 6972 6563 746f   a valid directo
-000289c0: 7279 2070 6174 6827 2c0a 2020 2020 2020  ry path',.      
-000289d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000289e0: 2020 2020 2020 2020 2020 736f 7572 6365            source
-000289f0: 3d73 7570 6572 696d 706f 7365 5f65 6c61  =superimpose_ela
-00028a00: 7073 6564 5f74 696d 652e 5f5f 6e61 6d65  psed_time.__name
-00028a10: 5f5f 290a 2020 2020 6966 2073 6176 655f  __).    if save_
-00028a20: 6469 7220 6973 206e 6f74 204e 6f6e 653a  dir is not None:
-00028a30: 0a20 2020 2020 2020 2063 6865 636b 5f69  .        check_i
-00028a40: 665f 6469 725f 6578 6973 7473 2869 6e5f  f_dir_exists(in_
-00028a50: 6469 723d 7361 7665 5f64 6972 290a 2020  dir=save_dir).  
-00028a60: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00028a70: 7361 7665 5f64 6972 203d 206f 732e 7061  save_dir = os.pa
-00028a80: 7468 2e64 6972 6e61 6d65 2876 6964 656f  th.dirname(video
-00028a90: 5f70 6174 6873 5b30 5d29 0a20 2020 2066  _paths[0]).    f
-00028aa0: 6f72 2066 696c 655f 636e 742c 2076 6964  or file_cnt, vid
-00028ab0: 656f 5f70 6174 6820 696e 2065 6e75 6d65  eo_path in enume
-00028ac0: 7261 7465 2876 6964 656f 5f70 6174 6873  rate(video_paths
-00028ad0: 293a 0a20 2020 2020 2020 205f 2c20 7669  ):.        _, vi
-00028ae0: 6465 6f5f 6e61 6d65 2c20 6578 7420 3d20  deo_name, ext = 
-00028af0: 6765 745f 666e 5f65 7874 2876 6964 656f  get_fn_ext(video
-00028b00: 5f70 6174 6829 0a20 2020 2020 2020 2070  _path).        p
-00028b10: 7269 6e74 2866 2753 7570 6572 696d 706f  rint(f'Superimpo
-00028b20: 7369 6e67 2074 696d 6520 7b76 6964 656f  sing time {video
-00028b30: 5f6e 616d 657d 2028 5669 6465 6f20 7b66  _name} (Video {f
-00028b40: 696c 655f 636e 7420 2b20 317d 2f7b 6c65  ile_cnt + 1}/{le
-00028b50: 6e28 7669 6465 6f5f 7061 7468 7329 7d29  n(video_paths)})
-00028b60: 2e2e 2e27 290a 2020 2020 2020 2020 7361  ...').        sa
-00028b70: 7665 5f70 6174 6820 3d20 6f73 2e70 6174  ve_path = os.pat
-00028b80: 682e 6a6f 696e 2873 6176 655f 6469 722c  h.join(save_dir,
-00028b90: 2066 277b 7669 6465 6f5f 6e61 6d65 7d5f   f'{video_name}_
-00028ba0: 7469 6d65 5f73 7570 6572 696d 706f 7365  time_superimpose
-00028bb0: 647b 6578 747d 2729 0a20 2020 2020 2020  d{ext}').       
-00028bc0: 2069 6620 706f 7369 7469 6f6e 203d 3d20   if position == 
-00028bd0: 504f 5349 5449 4f4e 535b 305d 3a0a 2020  POSITIONS[0]:.  
-00028be0: 2020 2020 2020 2020 2020 636d 6420 3d20            cmd = 
-00028bf0: 6622 6666 6d70 6567 202d 6920 277b 7669  f"ffmpeg -i '{vi
-00028c00: 6465 6f5f 7061 7468 7d27 202d 7666 205c  deo_path}' -vf \
-00028c10: 2264 7261 7774 6578 743d 666f 6e74 6669  "drawtext=fontfi
-00028c20: 6c65 3d41 7269 616c 2e74 7466 3a74 6578  le=Arial.ttf:tex
-00028c30: 743d 2725 7b7b 7074 735c 3a68 6d73 7d7d  t='%{{pts\:hms}}
-00028c40: 2e25 7b7b 6569 665c 3a6d 6f64 286e 5c5c  .%{{eif\:mod(n\\
-00028c50: 2c31 3030 3029 5c5c 3a64 5c5c 3a33 7d7d  ,1000)\\:d\\:3}}
-00028c60: 273a 783d 353a 793d 353a 666f 6e74 7369  ':x=5:y=5:fontsi
-00028c70: 7a65 3d7b 666f 6e74 5f73 697a 657d 3a66  ze={font_size}:f
-00028c80: 6f6e 7463 6f6c 6f72 3d7b 666f 6e74 5f63  ontcolor={font_c
-00028c90: 6f6c 6f72 7d3a 626f 7264 6572 773d 7b66  olor}:borderw={f
-00028ca0: 6f6e 745f 626f 7264 6572 5f77 6964 7468  ont_border_width
-00028cb0: 7d3a 626f 7264 6572 636f 6c6f 723d 7b66  }:bordercolor={f
-00028cc0: 6f6e 745f 626f 7264 6572 5f63 6f6c 6f72  ont_border_color
-00028cd0: 7d5c 2220 2d63 3a61 2063 6f70 7920 277b  }\" -c:a copy '{
-00028ce0: 7361 7665 5f70 6174 687d 2720 2d6c 6f67  save_path}' -log
-00028cf0: 6c65 7665 6c20 6572 726f 7220 2d73 7461  level error -sta
-00028d00: 7473 202d 6869 6465 5f62 616e 6e65 7220  ts -hide_banner 
-00028d10: 2d79 220a 2020 2020 2020 2020 656c 6966  -y".        elif
-00028d20: 2070 6f73 6974 696f 6e20 3d3d 2050 4f53   position == POS
-00028d30: 4954 494f 4e53 5b31 5d3a 0a20 2020 2020  ITIONS[1]:.     
-00028d40: 2020 2020 2020 2063 6d64 203d 2066 2266         cmd = f"f
-00028d50: 666d 7065 6720 2d69 2027 7b76 6964 656f  fmpeg -i '{video
-00028d60: 5f70 6174 687d 2720 2d76 6620 5c22 6472  _path}' -vf \"dr
-00028d70: 6177 7465 7874 3d66 6f6e 7466 696c 653d  awtext=fontfile=
-00028d80: 4172 6961 6c2e 7474 663a 7465 7874 3d27  Arial.ttf:text='
-00028d90: 257b 7b70 7473 5c3a 686d 737d 7d2e 257b  %{{pts\:hms}}.%{
-00028da0: 7b65 6966 5c3a 6d6f 6428 6e5c 5c2c 3130  {eif\:mod(n\\,10
-00028db0: 3030 295c 5c3a 645c 5c3a 337d 7d27 3a78  00)\\:d\\:3}}':x
-00028dc0: 3d28 772d 7477 2d35 293a 793d 353a 666f  =(w-tw-5):y=5:fo
-00028dd0: 6e74 7369 7a65 3d7b 666f 6e74 5f73 697a  ntsize={font_siz
-00028de0: 657d 3a66 6f6e 7463 6f6c 6f72 3d7b 666f  e}:fontcolor={fo
-00028df0: 6e74 5f63 6f6c 6f72 7d3a 626f 7264 6572  nt_color}:border
-00028e00: 773d 7b66 6f6e 745f 626f 7264 6572 5f77  w={font_border_w
-00028e10: 6964 7468 7d3a 626f 7264 6572 636f 6c6f  idth}:bordercolo
-00028e20: 723d 7b66 6f6e 745f 626f 7264 6572 5f63  r={font_border_c
-00028e30: 6f6c 6f72 7d5c 2220 2d63 3a61 2063 6f70  olor}\" -c:a cop
-00028e40: 7920 277b 7361 7665 5f70 6174 687d 2720  y '{save_path}' 
-00028e50: 2d6c 6f67 6c65 7665 6c20 6572 726f 7220  -loglevel error 
-00028e60: 2d73 7461 7473 202d 6869 6465 5f62 616e  -stats -hide_ban
-00028e70: 6e65 7220 2d79 220a 2020 2020 2020 2020  ner -y".        
-00028e80: 656c 6966 2070 6f73 6974 696f 6e20 3d3d  elif position ==
-00028e90: 2050 4f53 4954 494f 4e53 5b32 5d3a 0a20   POSITIONS[2]:. 
-00028ea0: 2020 2020 2020 2020 2020 2063 6d64 203d             cmd =
-00028eb0: 2066 2266 666d 7065 6720 2d69 2027 7b76   f"ffmpeg -i '{v
-00028ec0: 6964 656f 5f70 6174 687d 2720 2d76 6620  ideo_path}' -vf 
-00028ed0: 5c22 6472 6177 7465 7874 3d66 6f6e 7466  \"drawtext=fontf
-00028ee0: 696c 653d 4172 6961 6c2e 7474 663a 7465  ile=Arial.ttf:te
-00028ef0: 7874 3d27 257b 7b70 7473 5c3a 686d 737d  xt='%{{pts\:hms}
-00028f00: 7d2e 257b 7b65 6966 5c3a 6d6f 6428 6e5c  }.%{{eif\:mod(n\
-00028f10: 5c2c 3130 3030 295c 5c3a 645c 5c3a 337d  \,1000)\\:d\\:3}
-00028f20: 7d27 3a78 3d35 3a79 3d28 682d 7468 2d35  }':x=5:y=(h-th-5
-00028f30: 293a 666f 6e74 7369 7a65 3d7b 666f 6e74  ):fontsize={font
-00028f40: 5f73 697a 657d 3a66 6f6e 7463 6f6c 6f72  _size}:fontcolor
-00028f50: 3d7b 666f 6e74 5f63 6f6c 6f72 7d3a 626f  ={font_color}:bo
-00028f60: 7264 6572 773d 7b66 6f6e 745f 626f 7264  rderw={font_bord
-00028f70: 6572 5f77 6964 7468 7d3a 626f 7264 6572  er_width}:border
-00028f80: 636f 6c6f 723d 7b66 6f6e 745f 626f 7264  color={font_bord
-00028f90: 6572 5f63 6f6c 6f72 7d5c 2220 2d63 3a61  er_color}\" -c:a
-00028fa0: 2063 6f70 7920 277b 7361 7665 5f70 6174   copy '{save_pat
-00028fb0: 687d 2720 2d6c 6f67 6c65 7665 6c20 6572  h}' -loglevel er
-00028fc0: 726f 7220 2d73 7461 7473 202d 6869 6465  ror -stats -hide
-00028fd0: 5f62 616e 6e65 7220 2d79 220a 2020 2020  _banner -y".    
-00028fe0: 2020 2020 656c 6966 2070 6f73 6974 696f      elif positio
-00028ff0: 6e20 3d3d 2050 4f53 4954 494f 4e53 5b33  n == POSITIONS[3
-00029000: 5d3a 0a20 2020 2020 2020 2020 2020 2063  ]:.            c
-00029010: 6d64 203d 2066 2266 666d 7065 6720 2d69  md = f"ffmpeg -i
-00029020: 2027 7b76 6964 656f 5f70 6174 687d 2720   '{video_path}' 
-00029030: 2d76 6620 5c22 6472 6177 7465 7874 3d66  -vf \"drawtext=f
-00029040: 6f6e 7466 696c 653d 4172 6961 6c2e 7474  ontfile=Arial.tt
-00029050: 663a 7465 7874 3d27 257b 7b70 7473 5c3a  f:text='%{{pts\:
-00029060: 686d 737d 7d2e 257b 7b65 6966 5c3a 6d6f  hms}}.%{{eif\:mo
-00029070: 6428 6e5c 5c2c 3130 3030 295c 5c3a 645c  d(n\\,1000)\\:d\
-00029080: 5c3a 337d 7d27 3a78 3d28 772d 7477 2d35  \:3}}':x=(w-tw-5
-00029090: 293a 793d 2868 2d74 682d 3529 3a66 6f6e  ):y=(h-th-5):fon
-000290a0: 7473 697a 653d 7b66 6f6e 745f 7369 7a65  tsize={font_size
-000290b0: 7d3a 666f 6e74 636f 6c6f 723d 7b66 6f6e  }:fontcolor={fon
-000290c0: 745f 636f 6c6f 727d 3a62 6f72 6465 7277  t_color}:borderw
-000290d0: 3d7b 666f 6e74 5f62 6f72 6465 725f 7769  ={font_border_wi
-000290e0: 6474 687d 3a62 6f72 6465 7263 6f6c 6f72  dth}:bordercolor
-000290f0: 3d7b 666f 6e74 5f62 6f72 6465 725f 636f  ={font_border_co
-00029100: 6c6f 727d 5c22 202d 633a 6120 636f 7079  lor}\" -c:a copy
-00029110: 2027 7b73 6176 655f 7061 7468 7d27 202d   '{save_path}' -
-00029120: 6c6f 676c 6576 656c 2065 7272 6f72 202d  loglevel error -
-00029130: 7374 6174 7320 2d68 6964 655f 6261 6e6e  stats -hide_bann
-00029140: 6572 202d 7922 0a20 2020 2020 2020 2065  er -y".        e
-00029150: 6c69 6620 706f 7369 7469 6f6e 203d 3d20  lif position == 
-00029160: 504f 5349 5449 4f4e 535b 345d 3a0a 2020  POSITIONS[4]:.  
-00029170: 2020 2020 2020 2020 2020 636d 6420 3d20            cmd = 
-00029180: 6622 6666 6d70 6567 202d 6920 277b 7669  f"ffmpeg -i '{vi
-00029190: 6465 6f5f 7061 7468 7d27 202d 7666 205c  deo_path}' -vf \
-000291a0: 2264 7261 7774 6578 743d 666f 6e74 6669  "drawtext=fontfi
-000291b0: 6c65 3d41 7269 616c 2e74 7466 3a74 6578  le=Arial.ttf:tex
-000291c0: 743d 2725 7b7b 7074 735c 3a68 6d73 7d7d  t='%{{pts\:hms}}
-000291d0: 2e25 7b7b 6569 665c 3a6d 6f64 286e 5c5c  .%{{eif\:mod(n\\
-000291e0: 2c31 3030 3029 5c5c 3a64 5c5c 3a33 7d7d  ,1000)\\:d\\:3}}
-000291f0: 273a 783d 2877 2d74 7729 2f32 3a79 3d31  ':x=(w-tw)/2:y=1
-00029200: 303a 666f 6e74 7369 7a65 3d7b 666f 6e74  0:fontsize={font
-00029210: 5f73 697a 657d 3a66 6f6e 7463 6f6c 6f72  _size}:fontcolor
-00029220: 3d7b 666f 6e74 5f63 6f6c 6f72 7d3a 626f  ={font_color}:bo
-00029230: 7264 6572 773d 7b66 6f6e 745f 626f 7264  rderw={font_bord
-00029240: 6572 5f77 6964 7468 7d3a 626f 7264 6572  er_width}:border
-00029250: 636f 6c6f 723d 7b66 6f6e 745f 626f 7264  color={font_bord
-00029260: 6572 5f63 6f6c 6f72 7d5c 2220 2d63 3a61  er_color}\" -c:a
-00029270: 2063 6f70 7920 277b 7361 7665 5f70 6174   copy '{save_pat
-00029280: 687d 2720 2d6c 6f67 6c65 7665 6c20 6572  h}' -loglevel er
-00029290: 726f 7220 2d73 7461 7473 202d 6869 6465  ror -stats -hide
-000292a0: 5f62 616e 6e65 7220 2d79 220a 2020 2020  _banner -y".    
-000292b0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-000292c0: 2020 2020 2020 636d 6420 3d20 6622 6666        cmd = f"ff
-000292d0: 6d70 6567 202d 6920 277b 7669 6465 6f5f  mpeg -i '{video_
-000292e0: 7061 7468 7d27 202d 7666 205c 2264 7261  path}' -vf \"dra
-000292f0: 7774 6578 743d 666f 6e74 6669 6c65 3d41  wtext=fontfile=A
-00029300: 7269 616c 2e74 7466 3a74 6578 743d 2725  rial.ttf:text='%
-00029310: 7b7b 7074 735c 3a68 6d73 7d7d 2e25 7b7b  {{pts\:hms}}.%{{
-00029320: 6569 665c 3a6d 6f64 286e 5c5c 2c31 3030  eif\:mod(n\\,100
-00029330: 3029 5c5c 3a64 5c5c 3a33 7d7d 273a 783d  0)\\:d\\:3}}':x=
-00029340: 2877 2d74 7729 2f32 3a79 3d28 682d 7468  (w-tw)/2:y=(h-th
-00029350: 2d31 3029 3a66 6f6e 7473 697a 653d 7b66  -10):fontsize={f
-00029360: 6f6e 745f 7369 7a65 7d3a 666f 6e74 636f  ont_size}:fontco
-00029370: 6c6f 723d 7b66 6f6e 745f 636f 6c6f 727d  lor={font_color}
-00029380: 3a62 6f72 6465 7277 3d7b 666f 6e74 5f62  :borderw={font_b
-00029390: 6f72 6465 725f 7769 6474 687d 3a62 6f72  order_width}:bor
-000293a0: 6465 7263 6f6c 6f72 3d7b 666f 6e74 5f62  dercolor={font_b
-000293b0: 6f72 6465 725f 636f 6c6f 727d 5c22 202d  order_color}\" -
-000293c0: 633a 6120 636f 7079 2027 7b73 6176 655f  c:a copy '{save_
-000293d0: 7061 7468 7d27 202d 6c6f 676c 6576 656c  path}' -loglevel
-000293e0: 2065 7272 6f72 202d 7374 6174 7320 2d68   error -stats -h
-000293f0: 6964 655f 6261 6e6e 6572 202d 7922 0a20  ide_banner -y". 
-00029400: 2020 2020 2020 2073 7562 7072 6f63 6573         subproces
-00029410: 732e 6361 6c6c 2863 6d64 2c20 7368 656c  s.call(cmd, shel
-00029420: 6c3d 5472 7565 2c20 7374 646f 7574 3d73  l=True, stdout=s
-00029430: 7562 7072 6f63 6573 732e 5049 5045 290a  ubprocess.PIPE).
-00029440: 2020 2020 7469 6d65 722e 7374 6f70 5f74      timer.stop_t
-00029450: 696d 6572 2829 0a20 2020 2073 7464 6f75  imer().    stdou
-00029460: 745f 7375 6363 6573 7328 6d73 673d 6627  t_success(msg=f'
-00029470: 5375 7065 722d 696d 706f 7365 6420 7469  Super-imposed ti
-00029480: 6d65 206f 6e20 7b6c 656e 2876 6964 656f  me on {len(video
-00029490: 5f70 6174 6873 297d 2076 6964 656f 2873  _paths)} video(s
-000294a0: 292c 2073 6176 6564 2069 6e20 7b73 6176  ), saved in {sav
-000294b0: 655f 6469 727d 272c 2065 6c61 7073 6564  e_dir}', elapsed
-000294c0: 5f74 696d 653d 7469 6d65 722e 656c 6170  _time=timer.elap
-000294d0: 7365 645f 7469 6d65 5f73 7472 290a 0a0a  sed_time_str)...
-000294e0: 6465 6620 7669 6465 6f5f 746f 5f62 7728  def video_to_bw(
-000294f0: 7669 6465 6f5f 7061 7468 3a20 556e 696f  video_path: Unio
-00029500: 6e5b 7374 722c 206f 732e 5061 7468 4c69  n[str, os.PathLi
-00029510: 6b65 5d2c 0a20 2020 2020 2020 2020 2020  ke],.           
-00029520: 2020 2020 2074 6872 6573 686f 6c64 3a20       threshold: 
-00029530: 4f70 7469 6f6e 616c 5b66 6c6f 6174 5d20  Optional[float] 
-00029540: 3d20 302e 3529 202d 3e20 4e6f 6e65 3a0a  = 0.5) -> None:.
-00029550: 2020 2020 2222 220a 2020 2020 436f 6e76      """.    Conv
-00029560: 6572 7420 7669 6465 6f20 746f 2062 6c61  ert video to bla
-00029570: 636b 2061 6e64 2077 6869 7465 2075 7369  ck and white usi
-00029580: 6e67 2070 6173 7365 6420 7468 7265 7368  ng passed thresh
-00029590: 6f6c 642e 0a0a 2020 2020 2e2e 2076 6964  old...    .. vid
-000295a0: 656f 3a3a 205f 7374 6174 6963 2f69 6d67  eo:: _static/img
-000295b0: 2f76 6964 656f 5f74 6f5f 6277 2e77 6562  /video_to_bw.web
-000295c0: 6d0a 2020 2020 2020 203a 6c6f 6f70 3a0a  m.       :loop:.
-000295d0: 0a20 2020 203a 7061 7261 6d20 556e 696f  .    :param Unio
-000295e0: 6e5b 7374 722c 206f 732e 5061 7468 4c69  n[str, os.PathLi
-000295f0: 6b65 5d20 7669 6465 6f5f 7061 7468 3a20  ke] video_path: 
-00029600: 5061 7468 2074 6f20 7468 6520 7669 6465  Path to the vide
-00029610: 6f0a 2020 2020 3a70 6172 616d 204f 7074  o.    :param Opt
-00029620: 696f 6e61 6c5b 666c 6f61 745d 2074 6872  ional[float] thr
-00029630: 6573 686f 6c64 3a20 5661 6c75 6520 6265  eshold: Value be
-00029640: 7477 6565 6e20 3020 616e 6420 312e 204c  tween 0 and 1. L
-00029650: 6f77 6572 2076 616c 7565 7320 6769 7665  ower values give
-00029660: 7320 6d6f 7265 2077 6869 7465 2061 6e64  s more white and
-00029670: 2076 6963 6520 7665 7273 612e 0a20 2020   vice versa..   
-00029680: 203a 7265 7475 726e 3a20 4e6f 6e65 2e0a   :return: None..
-00029690: 0a20 2020 203a 6578 616d 706c 653a 0a20  .    :example:. 
-000296a0: 2020 203e 3e3e 2076 6964 656f 5f74 6f5f     >>> video_to_
-000296b0: 6277 2876 6964 656f 5f70 6174 683d 272f  bw(video_path='/
-000296c0: 5573 6572 732f 7369 6d6f 6e2f 446f 776e  Users/simon/Down
-000296d0: 6c6f 6164 732f 315f 4c48 5f63 6c69 7070  loads/1_LH_clipp
-000296e0: 6564 5f63 726f 7070 6564 5f65 715f 3230  ed_cropped_eq_20
-000296f0: 3234 3035 3135 3133 3539 3236 2e6d 7034  240515135926.mp4
-00029700: 272c 2074 6872 6573 686f 6c64 3d30 2e30  ', threshold=0.0
-00029710: 3229 0a20 2020 2022 2222 0a0a 2020 2020  2).    """..    
-00029720: 6368 6563 6b5f 666c 6f61 7428 6e61 6d65  check_float(name
-00029730: 3d66 277b 7669 6465 6f5f 746f 5f62 772e  =f'{video_to_bw.
-00029740: 5f5f 6e61 6d65 5f5f 7d20 7468 7265 7368  __name__} thresh
-00029750: 6f6c 6427 2c20 7661 6c75 653d 7468 7265  old', value=thre
-00029760: 7368 6f6c 642c 206d 696e 5f76 616c 7565  shold, min_value
-00029770: 3d30 2c20 6d61 785f 7661 6c75 653d 312e  =0, max_value=1.
-00029780: 3029 0a20 2020 2074 6872 6573 686f 6c64  0).    threshold
-00029790: 203d 2069 6e74 2832 3535 202a 2074 6872   = int(255 * thr
-000297a0: 6573 686f 6c64 290a 2020 2020 6368 6563  eshold).    chec
-000297b0: 6b5f 6666 6d70 6567 5f61 7661 696c 6162  k_ffmpeg_availab
-000297c0: 6c65 2872 6169 7365 5f65 7272 6f72 3d54  le(raise_error=T
-000297d0: 7275 6529 0a20 2020 2074 696d 6572 203d  rue).    timer =
-000297e0: 2053 696d 6261 5469 6d65 7228 7374 6172   SimbaTimer(star
-000297f0: 743d 5472 7565 290a 2020 2020 5f20 3d20  t=True).    _ = 
-00029800: 6765 745f 7669 6465 6f5f 6d65 7461 5f64  get_video_meta_d
-00029810: 6174 6128 7669 6465 6f5f 7061 7468 3d76  ata(video_path=v
-00029820: 6964 656f 5f70 6174 6829 0a20 2020 2064  ideo_path).    d
-00029830: 6972 2c20 7669 6465 6f5f 6e61 6d65 2c20  ir, video_name, 
-00029840: 6578 7420 3d20 6765 745f 666e 5f65 7874  ext = get_fn_ext
-00029850: 2876 6964 656f 5f70 6174 6829 0a20 2020  (video_path).   
-00029860: 2073 6176 655f 7061 7468 203d 206f 732e   save_path = os.
-00029870: 7061 7468 2e6a 6f69 6e28 6469 722c 2066  path.join(dir, f
-00029880: 277b 7669 6465 6f5f 6e61 6d65 7d5f 6277  '{video_name}_bw
-00029890: 7b65 7874 7d27 290a 2020 2020 636d 6420  {ext}').    cmd 
-000298a0: 3d20 6622 6666 6d70 6567 202d 6920 277b  = f"ffmpeg -i '{
-000298b0: 7669 6465 6f5f 7061 7468 7d27 202d 7666  video_path}' -vf
-000298c0: 205c 2266 6f72 6d61 743d 6772 6179 2c67   \"format=gray,g
-000298d0: 6571 3d6c 756d 5f65 7870 723d 2769 6628  eq=lum_expr='if(
-000298e0: 6c74 286c 756d 2858 2c59 292c 7b74 6872  lt(lum(X,Y),{thr
-000298f0: 6573 686f 6c64 7d29 2c30 2c32 3535 2927  eshold}),0,255)'
-00029900: 5c22 202d 7069 785f 666d 7420 7975 7634  \" -pix_fmt yuv4
-00029910: 3230 7020 277b 7361 7665 5f70 6174 687d  20p '{save_path}
-00029920: 2720 2d79 220a 2020 2020 7375 6270 726f  ' -y".    subpro
-00029930: 6365 7373 2e63 616c 6c28 636d 642c 2073  cess.call(cmd, s
-00029940: 6865 6c6c 3d54 7275 652c 2073 7464 6f75  hell=True, stdou
-00029950: 743d 7375 6270 726f 6365 7373 2e50 4950  t=subprocess.PIP
-00029960: 4529 0a20 2020 2074 696d 6572 2e73 746f  E).    timer.sto
-00029970: 705f 7469 6d65 7228 290a 2020 2020 7374  p_timer().    st
-00029980: 646f 7574 5f73 7563 6365 7373 286d 7367  dout_success(msg
-00029990: 3d66 2756 6964 656f 207b 7669 6465 6f5f  =f'Video {video_
-000299a0: 6e61 6d65 7d20 636f 6e76 6572 7465 642e  name} converted.
-000299b0: 272c 2065 6c61 7073 6564 5f74 696d 653d  ', elapsed_time=
-000299c0: 7469 6d65 722e 656c 6170 7365 645f 7469  timer.elapsed_ti
-000299d0: 6d65 5f73 7472 290a 0a0a 6465 6620 6372  me_str)...def cr
-000299e0: 6561 7465 5f61 7665 7261 6765 5f66 726d  eate_average_frm
-000299f0: 2876 6964 656f 5f70 6174 683a 2055 6e69  (video_path: Uni
-00029a00: 6f6e 5b73 7472 2c20 6f73 2e50 6174 684c  on[str, os.PathL
-00029a10: 696b 655d 2c0a 2020 2020 2020 2020 2020  ike],.          
-00029a20: 2020 2020 2020 2020 2020 2020 2073 7461               sta
-00029a30: 7274 5f66 726d 3a20 4f70 7469 6f6e 616c  rt_frm: Optional
-00029a40: 5b69 6e74 5d20 3d20 4e6f 6e65 2c0a 2020  [int] = None,.  
+00027fb0: 666f 6e74 5f62 6f72 6465 725f 7769 6474  font_border_widt
+00027fc0: 683a 204f 7074 696f 6e61 6c5b 696e 745d  h: Optional[int]
+00027fd0: 203d 2032 2c0a 2020 2020 2020 2020 2020   = 2,.          
+00027fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027ff0: 2020 2070 6f73 6974 696f 6e3a 204f 7074     position: Opt
+00028000: 696f 6e61 6c5b 4c69 7465 7261 6c5b 2774  ional[Literal['t
+00028010: 6f70 5f6c 6566 7427 2c20 2774 6f70 5f72  op_left', 'top_r
+00028020: 6967 6874 272c 2027 626f 7474 6f6d 5f6c  ight', 'bottom_l
+00028030: 6566 7427 2c20 2762 6f74 746f 6d5f 7269  eft', 'bottom_ri
+00028040: 6768 7427 2c20 276d 6964 646c 655f 746f  ght', 'middle_to
+00028050: 7027 2c20 276d 6964 646c 655f 626f 7474  p', 'middle_bott
+00028060: 6f6d 275d 5d20 3d20 2774 6f70 5f6c 6566  om']] = 'top_lef
+00028070: 7427 2c0a 2020 2020 2020 2020 2020 2020  t',.            
+00028080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028090: 2073 6176 655f 6469 723a 204f 7074 696f   save_dir: Optio
+000280a0: 6e61 6c5b 556e 696f 6e5b 7374 722c 206f  nal[Union[str, o
+000280b0: 732e 5061 7468 4c69 6b65 5d5d 203d 204e  s.PathLike]] = N
+000280c0: 6f6e 6529 202d 3e20 4e6f 6e65 3a0a 2020  one) -> None:.  
+000280d0: 2020 2222 220a 2020 2020 5375 7065 7269    """.    Superi
+000280e0: 6d70 6f73 6573 2065 6c61 7073 6564 2074  mposes elapsed t
+000280f0: 696d 6520 6f6e 2074 6865 2067 6976 656e  ime on the given
+00028100: 2076 6964 656f 2066 696c 6528 7329 2061   video file(s) a
+00028110: 6e64 2073 6176 6573 2074 6865 206d 6f64  nd saves the mod
+00028120: 6966 6965 6420 7669 6465 6f28 7329 2e0a  ified video(s)..
+00028130: 0a20 2020 202e 2e20 7669 6465 6f3a 3a20  .    .. video:: 
+00028140: 5f73 7461 7469 632f 696d 672f 7375 7065  _static/img/supe
+00028150: 7269 6d70 6f73 655f 656c 6170 7365 645f  rimpose_elapsed_
+00028160: 7469 6d65 2e77 6562 6d0a 2020 2020 2020  time.webm.      
+00028170: 203a 7769 6474 683a 2039 3030 0a20 2020   :width: 900.   
+00028180: 2020 2020 3a6c 6f6f 703a 0a0a 2020 2020      :loop:..    
+00028190: 3a70 6172 616d 2055 6e69 6f6e 5b73 7472  :param Union[str
+000281a0: 2c20 6f73 2e50 6174 684c 696b 655d 2076  , os.PathLike] v
+000281b0: 6964 656f 5f70 6174 683a 2050 6174 6820  ideo_path: Path 
+000281c0: 746f 2074 6865 2069 6e70 7574 2076 6964  to the input vid
+000281d0: 656f 2066 696c 6520 6f72 2064 6972 6563  eo file or direc
+000281e0: 746f 7279 2063 6f6e 7461 696e 696e 6720  tory containing 
+000281f0: 7669 6465 6f20 6669 6c65 732e 0a20 2020  video files..   
+00028200: 203a 7061 7261 6d20 4f70 7469 6f6e 616c   :param Optional
+00028210: 5b69 6e74 5d20 666f 6e74 5f73 697a 653a  [int] font_size:
+00028220: 2046 6f6e 7420 7369 7a65 2066 6f72 2074   Font size for t
+00028230: 6865 2065 6c61 7073 6564 2074 696d 6520  he elapsed time 
+00028240: 7465 7874 2e20 4465 6661 756c 7420 3330  text. Default 30
+00028250: 2e0a 2020 2020 3a70 6172 616d 204f 7074  ..    :param Opt
+00028260: 696f 6e61 6c5b 7374 725d 2066 6f6e 745f  ional[str] font_
+00028270: 636f 6c6f 723a 2020 466f 6e74 2063 6f6c  color:  Font col
+00028280: 6f72 2066 6f72 2074 6865 2065 6c61 7073  or for the elaps
+00028290: 6564 2074 696d 6520 7465 7874 2e20 4465  ed time text. De
+000282a0: 6661 756c 7420 7768 6974 650a 2020 2020  fault white.    
+000282b0: 3a70 6172 616d 204f 7074 696f 6e61 6c5b  :param Optional[
+000282c0: 7374 725d 2066 6f6e 745f 626f 7264 6572  str] font_border
+000282d0: 5f63 6f6c 6f72 3a20 466f 6e74 2062 6f72  _color: Font bor
+000282e0: 6465 7220 636f 6c6f 7220 666f 7220 7468  der color for th
+000282f0: 6520 656c 6170 7365 6420 7469 6d65 2074  e elapsed time t
+00028300: 6578 742e 2044 6566 6175 6c74 2062 6c61  ext. Default bla
+00028310: 636b 2e0a 2020 2020 3a70 6172 616d 204f  ck..    :param O
+00028320: 7074 696f 6e61 6c5b 696e 745d 2066 6f6e  ptional[int] fon
+00028330: 745f 626f 7264 6572 5f77 6964 7468 3a20  t_border_width: 
+00028340: 466f 6e74 2062 6f72 6465 7220 7769 6474  Font border widt
+00028350: 6820 666f 7220 7468 6520 656c 6170 7365  h for the elapse
+00028360: 6420 7469 6d65 2074 6578 7420 696e 2070  d time text in p
+00028370: 6978 656c 732e 2044 6566 6175 6c74 2032  ixels. Default 2
+00028380: 2e0a 2020 2020 3a70 6172 616d 204f 7074  ..    :param Opt
+00028390: 696f 6e61 6c5b 4c69 7465 7261 6c5b 2774  ional[Literal['t
+000283a0: 6f70 5f6c 6566 7427 2c20 2774 6f70 5f72  op_left', 'top_r
+000283b0: 6967 6874 272c 2027 626f 7474 6f6d 5f6c  ight', 'bottom_l
+000283c0: 6566 7427 2c20 2762 6f74 746f 6d5f 7269  eft', 'bottom_ri
+000283d0: 6768 7427 2c20 276d 6964 646c 655f 746f  ght', 'middle_to
+000283e0: 7027 2c20 276d 6964 646c 655f 626f 7474  p', 'middle_bott
+000283f0: 6f6d 275d 5d20 706f 7369 7469 6f6e 3a20  om']] position: 
+00028400: 506f 7369 7469 6f6e 2077 6865 7265 2074  Position where t
+00028410: 6865 2065 6c61 7073 6564 2074 696d 6520  he elapsed time 
+00028420: 7465 7874 2077 696c 6c20 6265 2073 7570  text will be sup
+00028430: 6572 696d 706f 7365 642e 2044 6566 6175  erimposed. Defau
+00028440: 6c74 2060 6074 6f70 5f6c 6566 7460 602e  lt ``top_left``.
+00028450: 0a20 2020 203a 7061 7261 6d20 4f70 7469  .    :param Opti
+00028460: 6f6e 616c 5b55 6e69 6f6e 5b73 7472 2c20  onal[Union[str, 
+00028470: 6f73 2e50 6174 684c 696b 655d 5d20 7361  os.PathLike]] sa
+00028480: 7665 5f64 6972 3a20 4469 7265 6374 6f72  ve_dir: Director
+00028490: 7920 7768 6572 6520 7468 6520 6d6f 6469  y where the modi
+000284a0: 6669 6564 2076 6964 656f 2873 2920 7769  fied video(s) wi
+000284b0: 6c6c 2062 6520 7361 7665 642e 2049 6620  ll be saved. If 
+000284c0: 6e6f 7420 7072 6f76 6964 6564 2c20 7468  not provided, th
+000284d0: 6520 6469 7265 6374 6f72 7920 6f66 2074  e directory of t
+000284e0: 6865 2069 6e70 7574 2076 6964 656f 2873  he input video(s
+000284f0: 2920 7769 6c6c 2062 6520 7573 6564 2e0a  ) will be used..
+00028500: 2020 2020 3a72 6574 7572 6e3a 204e 6f6e      :return: Non
+00028510: 650a 0a20 2020 203a 6578 616d 706c 653a  e..    :example:
+00028520: 0a20 2020 203e 3e3e 2073 7570 6572 696d  .    >>> superim
+00028530: 706f 7365 5f65 6c61 7073 6564 5f74 696d  pose_elapsed_tim
+00028540: 6528 7669 6465 6f5f 7061 7468 3d27 2f55  e(video_path='/U
+00028550: 7365 7273 2f73 696d 6f6e 2f44 6573 6b74  sers/simon/Deskt
+00028560: 6f70 2f65 6e76 732f 7369 6d62 612f 7472  op/envs/simba/tr
+00028570: 6f75 626c 6573 686f 6f74 696e 672f 6d6f  oubleshooting/mo
+00028580: 7573 655f 6f70 656e 5f66 6965 6c64 2f70  use_open_field/p
+00028590: 726f 6a65 6374 5f66 6f6c 6465 722f 7669  roject_folder/vi
+000285a0: 6465 6f73 2f74 6573 745f 342f 312e 6d70  deos/test_4/1.mp
+000285b0: 3427 2c20 706f 7369 7469 6f6e 3d27 6d69  4', position='mi
+000285c0: 6464 6c65 5f74 6f70 272c 2066 6f6e 745f  ddle_top', font_
+000285d0: 636f 6c6f 723d 2762 6c61 636b 272c 2066  color='black', f
+000285e0: 6f6e 745f 626f 7264 6572 5f63 6f6c 6f72  ont_border_color
+000285f0: 3d27 7069 6e6b 272c 2066 6f6e 745f 626f  ='pink', font_bo
+00028600: 7264 6572 5f77 6964 7468 3d35 2c20 666f  rder_width=5, fo
+00028610: 6e74 5f73 697a 653d 3330 290a 2020 2020  nt_size=30).    
+00028620: 2222 220a 0a20 2020 2063 6865 636b 5f66  """..    check_f
+00028630: 666d 7065 675f 6176 6169 6c61 626c 6528  fmpeg_available(
+00028640: 7261 6973 655f 6572 726f 723d 5472 7565  raise_error=True
+00028650: 290a 2020 2020 7469 6d65 7220 3d20 5369  ).    timer = Si
+00028660: 6d62 6154 696d 6572 2873 7461 7274 3d54  mbaTimer(start=T
+00028670: 7275 6529 0a20 2020 2050 4f53 4954 494f  rue).    POSITIO
+00028680: 4e53 203d 205b 2774 6f70 5f6c 6566 7427  NS = ['top_left'
+00028690: 2c20 2774 6f70 5f72 6967 6874 272c 2027  , 'top_right', '
+000286a0: 626f 7474 6f6d 5f6c 6566 7427 2c20 2762  bottom_left', 'b
+000286b0: 6f74 746f 6d5f 7269 6768 7427 2c20 2774  ottom_right', 't
+000286c0: 6f70 5f6d 6964 646c 6527 2c20 2762 6f74  op_middle', 'bot
+000286d0: 746f 6d5f 6d69 6464 6c65 275d 0a20 2020  tom_middle'].   
+000286e0: 2063 6865 636b 5f73 7472 286e 616d 653d   check_str(name=
+000286f0: 6627 7b73 7570 6572 696d 706f 7365 5f65  f'{superimpose_e
+00028700: 6c61 7073 6564 5f74 696d 652e 5f5f 6e61  lapsed_time.__na
+00028710: 6d65 5f5f 7d20 706f 7369 7469 6f6e 272c  me__} position',
+00028720: 2076 616c 7565 3d70 6f73 6974 696f 6e2c   value=position,
+00028730: 206f 7074 696f 6e73 3d50 4f53 4954 494f   options=POSITIO
+00028740: 4e53 290a 2020 2020 6368 6563 6b5f 696e  NS).    check_in
+00028750: 7428 6e61 6d65 3d66 277b 7375 7065 7269  t(name=f'{superi
+00028760: 6d70 6f73 655f 656c 6170 7365 645f 7469  mpose_elapsed_ti
+00028770: 6d65 2e5f 5f6e 616d 655f 5f7d 2066 6f6e  me.__name__} fon
+00028780: 745f 7369 7a65 272c 2076 616c 7565 3d66  t_size', value=f
+00028790: 6f6e 745f 7369 7a65 2c20 6d69 6e5f 7661  ont_size, min_va
+000287a0: 6c75 653d 3129 0a20 2020 2063 6865 636b  lue=1).    check
+000287b0: 5f69 6e74 286e 616d 653d 6627 7b73 7570  _int(name=f'{sup
+000287c0: 6572 696d 706f 7365 5f65 6c61 7073 6564  erimpose_elapsed
+000287d0: 5f74 696d 652e 5f5f 6e61 6d65 5f5f 7d20  _time.__name__} 
+000287e0: 666f 6e74 5f62 6f72 6465 725f 7769 6474  font_border_widt
+000287f0: 6827 2c20 7661 6c75 653d 666f 6e74 5f62  h', value=font_b
+00028800: 6f72 6465 725f 7769 6474 682c 206d 696e  order_width, min
+00028810: 5f76 616c 7565 3d31 290a 2020 2020 666f  _value=1).    fo
+00028820: 6e74 5f63 6f6c 6f72 203d 2027 272e 6a6f  nt_color = ''.jo
+00028830: 696e 2866 696c 7465 7228 7374 722e 6973  in(filter(str.is
+00028840: 616c 6e75 6d2c 2066 6f6e 745f 636f 6c6f  alnum, font_colo
+00028850: 7229 292e 6c6f 7765 7228 290a 2020 2020  r)).lower().    
+00028860: 666f 6e74 5f62 6f72 6465 725f 636f 6c6f  font_border_colo
+00028870: 7220 3d20 2727 2e6a 6f69 6e28 6669 6c74  r = ''.join(filt
+00028880: 6572 2873 7472 2e69 7361 6c6e 756d 2c20  er(str.isalnum, 
+00028890: 666f 6e74 5f62 6f72 6465 725f 636f 6c6f  font_border_colo
+000288a0: 7229 292e 6c6f 7765 7228 290a 2020 2020  r)).lower().    
+000288b0: 6966 206f 732e 7061 7468 2e69 7366 696c  if os.path.isfil
+000288c0: 6528 7669 6465 6f5f 7061 7468 293a 0a20  e(video_path):. 
+000288d0: 2020 2020 2020 2076 6964 656f 5f70 6174         video_pat
+000288e0: 6873 203d 205b 7669 6465 6f5f 7061 7468  hs = [video_path
+000288f0: 5d0a 2020 2020 656c 6966 206f 732e 7061  ].    elif os.pa
+00028900: 7468 2e69 7364 6972 2876 6964 656f 5f70  th.isdir(video_p
+00028910: 6174 6829 3a0a 2020 2020 2020 2020 7669  ath):.        vi
+00028920: 6465 6f5f 7061 7468 7320 3d20 6c69 7374  deo_paths = list
+00028930: 2866 696e 645f 616c 6c5f 7669 6465 6f73  (find_all_videos
+00028940: 5f69 6e5f 6469 7265 6374 6f72 7928 6469  _in_directory(di
+00028950: 7265 6374 6f72 793d 7669 6465 6f5f 7061  rectory=video_pa
+00028960: 7468 2c20 6173 5f64 6963 743d 5472 7565  th, as_dict=True
+00028970: 2c20 7261 6973 655f 6572 726f 723d 5472  , raise_error=Tr
+00028980: 7565 292e 7661 6c75 6573 2829 290a 2020  ue).values()).  
+00028990: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+000289a0: 7261 6973 6520 496e 7661 6c69 6449 6e70  raise InvalidInp
+000289b0: 7574 4572 726f 7228 6d73 673d 6627 7b76  utError(msg=f'{v
+000289c0: 6964 656f 5f70 6174 687d 2069 7320 6e6f  ideo_path} is no
+000289d0: 7420 6120 7661 6c69 6420 6669 6c65 2070  t a valid file p
+000289e0: 6174 6820 6f72 2061 2076 616c 6964 2064  ath or a valid d
+000289f0: 6972 6563 746f 7279 2070 6174 6827 2c0a  irectory path',.
+00028a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028a20: 736f 7572 6365 3d73 7570 6572 696d 706f  source=superimpo
+00028a30: 7365 5f65 6c61 7073 6564 5f74 696d 652e  se_elapsed_time.
+00028a40: 5f5f 6e61 6d65 5f5f 290a 2020 2020 6966  __name__).    if
+00028a50: 2073 6176 655f 6469 7220 6973 206e 6f74   save_dir is not
+00028a60: 204e 6f6e 653a 0a20 2020 2020 2020 2063   None:.        c
+00028a70: 6865 636b 5f69 665f 6469 725f 6578 6973  heck_if_dir_exis
+00028a80: 7473 2869 6e5f 6469 723d 7361 7665 5f64  ts(in_dir=save_d
+00028a90: 6972 290a 2020 2020 656c 7365 3a0a 2020  ir).    else:.  
+00028aa0: 2020 2020 2020 7361 7665 5f64 6972 203d        save_dir =
+00028ab0: 206f 732e 7061 7468 2e64 6972 6e61 6d65   os.path.dirname
+00028ac0: 2876 6964 656f 5f70 6174 6873 5b30 5d29  (video_paths[0])
+00028ad0: 0a20 2020 2066 6f72 2066 696c 655f 636e  .    for file_cn
+00028ae0: 742c 2076 6964 656f 5f70 6174 6820 696e  t, video_path in
+00028af0: 2065 6e75 6d65 7261 7465 2876 6964 656f   enumerate(video
+00028b00: 5f70 6174 6873 293a 0a20 2020 2020 2020  _paths):.       
+00028b10: 205f 2c20 7669 6465 6f5f 6e61 6d65 2c20   _, video_name, 
+00028b20: 6578 7420 3d20 6765 745f 666e 5f65 7874  ext = get_fn_ext
+00028b30: 2876 6964 656f 5f70 6174 6829 0a20 2020  (video_path).   
+00028b40: 2020 2020 2070 7269 6e74 2866 2753 7570       print(f'Sup
+00028b50: 6572 696d 706f 7369 6e67 2074 696d 6520  erimposing time 
+00028b60: 7b76 6964 656f 5f6e 616d 657d 2028 5669  {video_name} (Vi
+00028b70: 6465 6f20 7b66 696c 655f 636e 7420 2b20  deo {file_cnt + 
+00028b80: 317d 2f7b 6c65 6e28 7669 6465 6f5f 7061  1}/{len(video_pa
+00028b90: 7468 7329 7d29 2e2e 2e27 290a 2020 2020  ths)})...').    
+00028ba0: 2020 2020 7361 7665 5f70 6174 6820 3d20      save_path = 
+00028bb0: 6f73 2e70 6174 682e 6a6f 696e 2873 6176  os.path.join(sav
+00028bc0: 655f 6469 722c 2066 277b 7669 6465 6f5f  e_dir, f'{video_
+00028bd0: 6e61 6d65 7d5f 7469 6d65 5f73 7570 6572  name}_time_super
+00028be0: 696d 706f 7365 647b 6578 747d 2729 0a20  imposed{ext}'). 
+00028bf0: 2020 2020 2020 2069 6620 706f 7369 7469         if positi
+00028c00: 6f6e 203d 3d20 504f 5349 5449 4f4e 535b  on == POSITIONS[
+00028c10: 305d 3a0a 2020 2020 2020 2020 2020 2020  0]:.            
+00028c20: 636d 6420 3d20 6622 6666 6d70 6567 202d  cmd = f"ffmpeg -
+00028c30: 6920 277b 7669 6465 6f5f 7061 7468 7d27  i '{video_path}'
+00028c40: 202d 7666 205c 2264 7261 7774 6578 743d   -vf \"drawtext=
+00028c50: 666f 6e74 6669 6c65 3d41 7269 616c 2e74  fontfile=Arial.t
+00028c60: 7466 3a74 6578 743d 2725 7b7b 7074 735c  tf:text='%{{pts\
+00028c70: 3a68 6d73 7d7d 2e25 7b7b 6569 665c 3a6d  :hms}}.%{{eif\:m
+00028c80: 6f64 286e 5c5c 2c31 3030 3029 5c5c 3a64  od(n\\,1000)\\:d
+00028c90: 5c5c 3a33 7d7d 273a 783d 353a 793d 353a  \\:3}}':x=5:y=5:
+00028ca0: 666f 6e74 7369 7a65 3d7b 666f 6e74 5f73  fontsize={font_s
+00028cb0: 697a 657d 3a66 6f6e 7463 6f6c 6f72 3d7b  ize}:fontcolor={
+00028cc0: 666f 6e74 5f63 6f6c 6f72 7d3a 626f 7264  font_color}:bord
+00028cd0: 6572 773d 7b66 6f6e 745f 626f 7264 6572  erw={font_border
+00028ce0: 5f77 6964 7468 7d3a 626f 7264 6572 636f  _width}:borderco
+00028cf0: 6c6f 723d 7b66 6f6e 745f 626f 7264 6572  lor={font_border
+00028d00: 5f63 6f6c 6f72 7d5c 2220 2d63 3a61 2063  _color}\" -c:a c
+00028d10: 6f70 7920 277b 7361 7665 5f70 6174 687d  opy '{save_path}
+00028d20: 2720 2d6c 6f67 6c65 7665 6c20 6572 726f  ' -loglevel erro
+00028d30: 7220 2d73 7461 7473 202d 6869 6465 5f62  r -stats -hide_b
+00028d40: 616e 6e65 7220 2d79 220a 2020 2020 2020  anner -y".      
+00028d50: 2020 656c 6966 2070 6f73 6974 696f 6e20    elif position 
+00028d60: 3d3d 2050 4f53 4954 494f 4e53 5b31 5d3a  == POSITIONS[1]:
+00028d70: 0a20 2020 2020 2020 2020 2020 2063 6d64  .            cmd
+00028d80: 203d 2066 2266 666d 7065 6720 2d69 2027   = f"ffmpeg -i '
+00028d90: 7b76 6964 656f 5f70 6174 687d 2720 2d76  {video_path}' -v
+00028da0: 6620 5c22 6472 6177 7465 7874 3d66 6f6e  f \"drawtext=fon
+00028db0: 7466 696c 653d 4172 6961 6c2e 7474 663a  tfile=Arial.ttf:
+00028dc0: 7465 7874 3d27 257b 7b70 7473 5c3a 686d  text='%{{pts\:hm
+00028dd0: 737d 7d2e 257b 7b65 6966 5c3a 6d6f 6428  s}}.%{{eif\:mod(
+00028de0: 6e5c 5c2c 3130 3030 295c 5c3a 645c 5c3a  n\\,1000)\\:d\\:
+00028df0: 337d 7d27 3a78 3d28 772d 7477 2d35 293a  3}}':x=(w-tw-5):
+00028e00: 793d 353a 666f 6e74 7369 7a65 3d7b 666f  y=5:fontsize={fo
+00028e10: 6e74 5f73 697a 657d 3a66 6f6e 7463 6f6c  nt_size}:fontcol
+00028e20: 6f72 3d7b 666f 6e74 5f63 6f6c 6f72 7d3a  or={font_color}:
+00028e30: 626f 7264 6572 773d 7b66 6f6e 745f 626f  borderw={font_bo
+00028e40: 7264 6572 5f77 6964 7468 7d3a 626f 7264  rder_width}:bord
+00028e50: 6572 636f 6c6f 723d 7b66 6f6e 745f 626f  ercolor={font_bo
+00028e60: 7264 6572 5f63 6f6c 6f72 7d5c 2220 2d63  rder_color}\" -c
+00028e70: 3a61 2063 6f70 7920 277b 7361 7665 5f70  :a copy '{save_p
+00028e80: 6174 687d 2720 2d6c 6f67 6c65 7665 6c20  ath}' -loglevel 
+00028e90: 6572 726f 7220 2d73 7461 7473 202d 6869  error -stats -hi
+00028ea0: 6465 5f62 616e 6e65 7220 2d79 220a 2020  de_banner -y".  
+00028eb0: 2020 2020 2020 656c 6966 2070 6f73 6974        elif posit
+00028ec0: 696f 6e20 3d3d 2050 4f53 4954 494f 4e53  ion == POSITIONS
+00028ed0: 5b32 5d3a 0a20 2020 2020 2020 2020 2020  [2]:.           
+00028ee0: 2063 6d64 203d 2066 2266 666d 7065 6720   cmd = f"ffmpeg 
+00028ef0: 2d69 2027 7b76 6964 656f 5f70 6174 687d  -i '{video_path}
+00028f00: 2720 2d76 6620 5c22 6472 6177 7465 7874  ' -vf \"drawtext
+00028f10: 3d66 6f6e 7466 696c 653d 4172 6961 6c2e  =fontfile=Arial.
+00028f20: 7474 663a 7465 7874 3d27 257b 7b70 7473  ttf:text='%{{pts
+00028f30: 5c3a 686d 737d 7d2e 257b 7b65 6966 5c3a  \:hms}}.%{{eif\:
+00028f40: 6d6f 6428 6e5c 5c2c 3130 3030 295c 5c3a  mod(n\\,1000)\\:
+00028f50: 645c 5c3a 337d 7d27 3a78 3d35 3a79 3d28  d\\:3}}':x=5:y=(
+00028f60: 682d 7468 2d35 293a 666f 6e74 7369 7a65  h-th-5):fontsize
+00028f70: 3d7b 666f 6e74 5f73 697a 657d 3a66 6f6e  ={font_size}:fon
+00028f80: 7463 6f6c 6f72 3d7b 666f 6e74 5f63 6f6c  tcolor={font_col
+00028f90: 6f72 7d3a 626f 7264 6572 773d 7b66 6f6e  or}:borderw={fon
+00028fa0: 745f 626f 7264 6572 5f77 6964 7468 7d3a  t_border_width}:
+00028fb0: 626f 7264 6572 636f 6c6f 723d 7b66 6f6e  bordercolor={fon
+00028fc0: 745f 626f 7264 6572 5f63 6f6c 6f72 7d5c  t_border_color}\
+00028fd0: 2220 2d63 3a61 2063 6f70 7920 277b 7361  " -c:a copy '{sa
+00028fe0: 7665 5f70 6174 687d 2720 2d6c 6f67 6c65  ve_path}' -logle
+00028ff0: 7665 6c20 6572 726f 7220 2d73 7461 7473  vel error -stats
+00029000: 202d 6869 6465 5f62 616e 6e65 7220 2d79   -hide_banner -y
+00029010: 220a 2020 2020 2020 2020 656c 6966 2070  ".        elif p
+00029020: 6f73 6974 696f 6e20 3d3d 2050 4f53 4954  osition == POSIT
+00029030: 494f 4e53 5b33 5d3a 0a20 2020 2020 2020  IONS[3]:.       
+00029040: 2020 2020 2063 6d64 203d 2066 2266 666d       cmd = f"ffm
+00029050: 7065 6720 2d69 2027 7b76 6964 656f 5f70  peg -i '{video_p
+00029060: 6174 687d 2720 2d76 6620 5c22 6472 6177  ath}' -vf \"draw
+00029070: 7465 7874 3d66 6f6e 7466 696c 653d 4172  text=fontfile=Ar
+00029080: 6961 6c2e 7474 663a 7465 7874 3d27 257b  ial.ttf:text='%{
+00029090: 7b70 7473 5c3a 686d 737d 7d2e 257b 7b65  {pts\:hms}}.%{{e
+000290a0: 6966 5c3a 6d6f 6428 6e5c 5c2c 3130 3030  if\:mod(n\\,1000
+000290b0: 295c 5c3a 645c 5c3a 337d 7d27 3a78 3d28  )\\:d\\:3}}':x=(
+000290c0: 772d 7477 2d35 293a 793d 2868 2d74 682d  w-tw-5):y=(h-th-
+000290d0: 3529 3a66 6f6e 7473 697a 653d 7b66 6f6e  5):fontsize={fon
+000290e0: 745f 7369 7a65 7d3a 666f 6e74 636f 6c6f  t_size}:fontcolo
+000290f0: 723d 7b66 6f6e 745f 636f 6c6f 727d 3a62  r={font_color}:b
+00029100: 6f72 6465 7277 3d7b 666f 6e74 5f62 6f72  orderw={font_bor
+00029110: 6465 725f 7769 6474 687d 3a62 6f72 6465  der_width}:borde
+00029120: 7263 6f6c 6f72 3d7b 666f 6e74 5f62 6f72  rcolor={font_bor
+00029130: 6465 725f 636f 6c6f 727d 5c22 202d 633a  der_color}\" -c:
+00029140: 6120 636f 7079 2027 7b73 6176 655f 7061  a copy '{save_pa
+00029150: 7468 7d27 202d 6c6f 676c 6576 656c 2065  th}' -loglevel e
+00029160: 7272 6f72 202d 7374 6174 7320 2d68 6964  rror -stats -hid
+00029170: 655f 6261 6e6e 6572 202d 7922 0a20 2020  e_banner -y".   
+00029180: 2020 2020 2065 6c69 6620 706f 7369 7469       elif positi
+00029190: 6f6e 203d 3d20 504f 5349 5449 4f4e 535b  on == POSITIONS[
+000291a0: 345d 3a0a 2020 2020 2020 2020 2020 2020  4]:.            
+000291b0: 636d 6420 3d20 6622 6666 6d70 6567 202d  cmd = f"ffmpeg -
+000291c0: 6920 277b 7669 6465 6f5f 7061 7468 7d27  i '{video_path}'
+000291d0: 202d 7666 205c 2264 7261 7774 6578 743d   -vf \"drawtext=
+000291e0: 666f 6e74 6669 6c65 3d41 7269 616c 2e74  fontfile=Arial.t
+000291f0: 7466 3a74 6578 743d 2725 7b7b 7074 735c  tf:text='%{{pts\
+00029200: 3a68 6d73 7d7d 2e25 7b7b 6569 665c 3a6d  :hms}}.%{{eif\:m
+00029210: 6f64 286e 5c5c 2c31 3030 3029 5c5c 3a64  od(n\\,1000)\\:d
+00029220: 5c5c 3a33 7d7d 273a 783d 2877 2d74 7729  \\:3}}':x=(w-tw)
+00029230: 2f32 3a79 3d31 303a 666f 6e74 7369 7a65  /2:y=10:fontsize
+00029240: 3d7b 666f 6e74 5f73 697a 657d 3a66 6f6e  ={font_size}:fon
+00029250: 7463 6f6c 6f72 3d7b 666f 6e74 5f63 6f6c  tcolor={font_col
+00029260: 6f72 7d3a 626f 7264 6572 773d 7b66 6f6e  or}:borderw={fon
+00029270: 745f 626f 7264 6572 5f77 6964 7468 7d3a  t_border_width}:
+00029280: 626f 7264 6572 636f 6c6f 723d 7b66 6f6e  bordercolor={fon
+00029290: 745f 626f 7264 6572 5f63 6f6c 6f72 7d5c  t_border_color}\
+000292a0: 2220 2d63 3a61 2063 6f70 7920 277b 7361  " -c:a copy '{sa
+000292b0: 7665 5f70 6174 687d 2720 2d6c 6f67 6c65  ve_path}' -logle
+000292c0: 7665 6c20 6572 726f 7220 2d73 7461 7473  vel error -stats
+000292d0: 202d 6869 6465 5f62 616e 6e65 7220 2d79   -hide_banner -y
+000292e0: 220a 2020 2020 2020 2020 656c 7365 3a0a  ".        else:.
+000292f0: 2020 2020 2020 2020 2020 2020 636d 6420              cmd 
+00029300: 3d20 6622 6666 6d70 6567 202d 6920 277b  = f"ffmpeg -i '{
+00029310: 7669 6465 6f5f 7061 7468 7d27 202d 7666  video_path}' -vf
+00029320: 205c 2264 7261 7774 6578 743d 666f 6e74   \"drawtext=font
+00029330: 6669 6c65 3d41 7269 616c 2e74 7466 3a74  file=Arial.ttf:t
+00029340: 6578 743d 2725 7b7b 7074 735c 3a68 6d73  ext='%{{pts\:hms
+00029350: 7d7d 2e25 7b7b 6569 665c 3a6d 6f64 286e  }}.%{{eif\:mod(n
+00029360: 5c5c 2c31 3030 3029 5c5c 3a64 5c5c 3a33  \\,1000)\\:d\\:3
+00029370: 7d7d 273a 783d 2877 2d74 7729 2f32 3a79  }}':x=(w-tw)/2:y
+00029380: 3d28 682d 7468 2d31 3029 3a66 6f6e 7473  =(h-th-10):fonts
+00029390: 697a 653d 7b66 6f6e 745f 7369 7a65 7d3a  ize={font_size}:
+000293a0: 666f 6e74 636f 6c6f 723d 7b66 6f6e 745f  fontcolor={font_
+000293b0: 636f 6c6f 727d 3a62 6f72 6465 7277 3d7b  color}:borderw={
+000293c0: 666f 6e74 5f62 6f72 6465 725f 7769 6474  font_border_widt
+000293d0: 687d 3a62 6f72 6465 7263 6f6c 6f72 3d7b  h}:bordercolor={
+000293e0: 666f 6e74 5f62 6f72 6465 725f 636f 6c6f  font_border_colo
+000293f0: 727d 5c22 202d 633a 6120 636f 7079 2027  r}\" -c:a copy '
+00029400: 7b73 6176 655f 7061 7468 7d27 202d 6c6f  {save_path}' -lo
+00029410: 676c 6576 656c 2065 7272 6f72 202d 7374  glevel error -st
+00029420: 6174 7320 2d68 6964 655f 6261 6e6e 6572  ats -hide_banner
+00029430: 202d 7922 0a20 2020 2020 2020 2073 7562   -y".        sub
+00029440: 7072 6f63 6573 732e 6361 6c6c 2863 6d64  process.call(cmd
+00029450: 2c20 7368 656c 6c3d 5472 7565 2c20 7374  , shell=True, st
+00029460: 646f 7574 3d73 7562 7072 6f63 6573 732e  dout=subprocess.
+00029470: 5049 5045 290a 2020 2020 7469 6d65 722e  PIPE).    timer.
+00029480: 7374 6f70 5f74 696d 6572 2829 0a20 2020  stop_timer().   
+00029490: 2073 7464 6f75 745f 7375 6363 6573 7328   stdout_success(
+000294a0: 6d73 673d 6627 5375 7065 722d 696d 706f  msg=f'Super-impo
+000294b0: 7365 6420 7469 6d65 206f 6e20 7b6c 656e  sed time on {len
+000294c0: 2876 6964 656f 5f70 6174 6873 297d 2076  (video_paths)} v
+000294d0: 6964 656f 2873 292c 2073 6176 6564 2069  ideo(s), saved i
+000294e0: 6e20 7b73 6176 655f 6469 727d 272c 2065  n {save_dir}', e
+000294f0: 6c61 7073 6564 5f74 696d 653d 7469 6d65  lapsed_time=time
+00029500: 722e 656c 6170 7365 645f 7469 6d65 5f73  r.elapsed_time_s
+00029510: 7472 290a 0a0a 6465 6620 7669 6465 6f5f  tr)...def video_
+00029520: 746f 5f62 7728 7669 6465 6f5f 7061 7468  to_bw(video_path
+00029530: 3a20 556e 696f 6e5b 7374 722c 206f 732e  : Union[str, os.
+00029540: 5061 7468 4c69 6b65 5d2c 0a20 2020 2020  PathLike],.     
+00029550: 2020 2020 2020 2020 2020 2074 6872 6573             thres
+00029560: 686f 6c64 3a20 4f70 7469 6f6e 616c 5b66  hold: Optional[f
+00029570: 6c6f 6174 5d20 3d20 302e 3529 202d 3e20  loat] = 0.5) -> 
+00029580: 4e6f 6e65 3a0a 2020 2020 2222 220a 2020  None:.    """.  
+00029590: 2020 436f 6e76 6572 7420 7669 6465 6f20    Convert video 
+000295a0: 746f 2062 6c61 636b 2061 6e64 2077 6869  to black and whi
+000295b0: 7465 2075 7369 6e67 2070 6173 7365 6420  te using passed 
+000295c0: 7468 7265 7368 6f6c 642e 0a0a 2020 2020  threshold...    
+000295d0: 2e2e 2076 6964 656f 3a3a 205f 7374 6174  .. video:: _stat
+000295e0: 6963 2f69 6d67 2f76 6964 656f 5f74 6f5f  ic/img/video_to_
+000295f0: 6277 2e77 6562 6d0a 2020 2020 2020 203a  bw.webm.       :
+00029600: 6c6f 6f70 3a0a 0a20 2020 203a 7061 7261  loop:..    :para
+00029610: 6d20 556e 696f 6e5b 7374 722c 206f 732e  m Union[str, os.
+00029620: 5061 7468 4c69 6b65 5d20 7669 6465 6f5f  PathLike] video_
+00029630: 7061 7468 3a20 5061 7468 2074 6f20 7468  path: Path to th
+00029640: 6520 7669 6465 6f0a 2020 2020 3a70 6172  e video.    :par
+00029650: 616d 204f 7074 696f 6e61 6c5b 666c 6f61  am Optional[floa
+00029660: 745d 2074 6872 6573 686f 6c64 3a20 5661  t] threshold: Va
+00029670: 6c75 6520 6265 7477 6565 6e20 3020 616e  lue between 0 an
+00029680: 6420 312e 204c 6f77 6572 2076 616c 7565  d 1. Lower value
+00029690: 7320 6769 7665 7320 6d6f 7265 2077 6869  s gives more whi
+000296a0: 7465 2061 6e64 2076 6963 6520 7665 7273  te and vice vers
+000296b0: 612e 0a20 2020 203a 7265 7475 726e 3a20  a..    :return: 
+000296c0: 4e6f 6e65 2e0a 0a20 2020 203a 6578 616d  None...    :exam
+000296d0: 706c 653a 0a20 2020 203e 3e3e 2076 6964  ple:.    >>> vid
+000296e0: 656f 5f74 6f5f 6277 2876 6964 656f 5f70  eo_to_bw(video_p
+000296f0: 6174 683d 272f 5573 6572 732f 7369 6d6f  ath='/Users/simo
+00029700: 6e2f 446f 776e 6c6f 6164 732f 315f 4c48  n/Downloads/1_LH
+00029710: 5f63 6c69 7070 6564 5f63 726f 7070 6564  _clipped_cropped
+00029720: 5f65 715f 3230 3234 3035 3135 3133 3539  _eq_202405151359
+00029730: 3236 2e6d 7034 272c 2074 6872 6573 686f  26.mp4', thresho
+00029740: 6c64 3d30 2e30 3229 0a20 2020 2022 2222  ld=0.02).    """
+00029750: 0a0a 2020 2020 6368 6563 6b5f 666c 6f61  ..    check_floa
+00029760: 7428 6e61 6d65 3d66 277b 7669 6465 6f5f  t(name=f'{video_
+00029770: 746f 5f62 772e 5f5f 6e61 6d65 5f5f 7d20  to_bw.__name__} 
+00029780: 7468 7265 7368 6f6c 6427 2c20 7661 6c75  threshold', valu
+00029790: 653d 7468 7265 7368 6f6c 642c 206d 696e  e=threshold, min
+000297a0: 5f76 616c 7565 3d30 2c20 6d61 785f 7661  _value=0, max_va
+000297b0: 6c75 653d 312e 3029 0a20 2020 2074 6872  lue=1.0).    thr
+000297c0: 6573 686f 6c64 203d 2069 6e74 2832 3535  eshold = int(255
+000297d0: 202a 2074 6872 6573 686f 6c64 290a 2020   * threshold).  
+000297e0: 2020 6368 6563 6b5f 6666 6d70 6567 5f61    check_ffmpeg_a
+000297f0: 7661 696c 6162 6c65 2872 6169 7365 5f65  vailable(raise_e
+00029800: 7272 6f72 3d54 7275 6529 0a20 2020 2074  rror=True).    t
+00029810: 696d 6572 203d 2053 696d 6261 5469 6d65  imer = SimbaTime
+00029820: 7228 7374 6172 743d 5472 7565 290a 2020  r(start=True).  
+00029830: 2020 5f20 3d20 6765 745f 7669 6465 6f5f    _ = get_video_
+00029840: 6d65 7461 5f64 6174 6128 7669 6465 6f5f  meta_data(video_
+00029850: 7061 7468 3d76 6964 656f 5f70 6174 6829  path=video_path)
+00029860: 0a20 2020 2064 6972 2c20 7669 6465 6f5f  .    dir, video_
+00029870: 6e61 6d65 2c20 6578 7420 3d20 6765 745f  name, ext = get_
+00029880: 666e 5f65 7874 2876 6964 656f 5f70 6174  fn_ext(video_pat
+00029890: 6829 0a20 2020 2073 6176 655f 7061 7468  h).    save_path
+000298a0: 203d 206f 732e 7061 7468 2e6a 6f69 6e28   = os.path.join(
+000298b0: 6469 722c 2066 277b 7669 6465 6f5f 6e61  dir, f'{video_na
+000298c0: 6d65 7d5f 6277 7b65 7874 7d27 290a 2020  me}_bw{ext}').  
+000298d0: 2020 636d 6420 3d20 6622 6666 6d70 6567    cmd = f"ffmpeg
+000298e0: 202d 6920 277b 7669 6465 6f5f 7061 7468   -i '{video_path
+000298f0: 7d27 202d 7666 205c 2266 6f72 6d61 743d  }' -vf \"format=
+00029900: 6772 6179 2c67 6571 3d6c 756d 5f65 7870  gray,geq=lum_exp
+00029910: 723d 2769 6628 6c74 286c 756d 2858 2c59  r='if(lt(lum(X,Y
+00029920: 292c 7b74 6872 6573 686f 6c64 7d29 2c30  ),{threshold}),0
+00029930: 2c32 3535 2927 5c22 202d 7069 785f 666d  ,255)'\" -pix_fm
+00029940: 7420 7975 7634 3230 7020 277b 7361 7665  t yuv420p '{save
+00029950: 5f70 6174 687d 2720 2d79 220a 2020 2020  _path}' -y".    
+00029960: 7375 6270 726f 6365 7373 2e63 616c 6c28  subprocess.call(
+00029970: 636d 642c 2073 6865 6c6c 3d54 7275 652c  cmd, shell=True,
+00029980: 2073 7464 6f75 743d 7375 6270 726f 6365   stdout=subproce
+00029990: 7373 2e50 4950 4529 0a20 2020 2074 696d  ss.PIPE).    tim
+000299a0: 6572 2e73 746f 705f 7469 6d65 7228 290a  er.stop_timer().
+000299b0: 2020 2020 7374 646f 7574 5f73 7563 6365      stdout_succe
+000299c0: 7373 286d 7367 3d66 2756 6964 656f 207b  ss(msg=f'Video {
+000299d0: 7669 6465 6f5f 6e61 6d65 7d20 636f 6e76  video_name} conv
+000299e0: 6572 7465 642e 272c 2065 6c61 7073 6564  erted.', elapsed
+000299f0: 5f74 696d 653d 7469 6d65 722e 656c 6170  _time=timer.elap
+00029a00: 7365 645f 7469 6d65 5f73 7472 290a 0a0a  sed_time_str)...
+00029a10: 6465 6620 6372 6561 7465 5f61 7665 7261  def create_avera
+00029a20: 6765 5f66 726d 2876 6964 656f 5f70 6174  ge_frm(video_pat
+00029a30: 683a 2055 6e69 6f6e 5b73 7472 2c20 6f73  h: Union[str, os
+00029a40: 2e50 6174 684c 696b 655d 2c0a 2020 2020  .PathLike],.    
 00029a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029a60: 2020 2020 2065 6e64 5f66 726d 3a20 4f70       end_frm: Op
+00029a60: 2020 2073 7461 7274 5f66 726d 3a20 4f70     start_frm: Op
 00029a70: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
 00029a80: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
-00029a90: 2020 2020 2020 2020 2020 2073 7461 7274             start
-00029aa0: 5f74 696d 653a 204f 7074 696f 6e61 6c5b  _time: Optional[
-00029ab0: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
+00029a90: 2020 2020 2020 2020 2020 2065 6e64 5f66             end_f
+00029aa0: 726d 3a20 4f70 7469 6f6e 616c 5b69 6e74  rm: Optional[int
+00029ab0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
 00029ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029ad0: 2020 2020 656e 645f 7469 6d65 3a20 4f70      end_time: Op
-00029ae0: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
-00029af0: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
-00029b00: 2020 2020 2020 2020 2020 2073 6176 655f             save_
-00029b10: 7061 7468 3a20 4f70 7469 6f6e 616c 5b55  path: Optional[U
-00029b20: 6e69 6f6e 5b73 7472 2c20 6f73 2e50 6174  nion[str, os.Pat
-00029b30: 684c 696b 655d 5d20 3d20 4e6f 6e65 2920  hLike]] = None) 
-00029b40: 2d3e 2055 6e69 6f6e 5b4e 6f6e 652c 206e  -> Union[None, n
-00029b50: 702e 6e64 6172 7261 795d 3a0a 2020 2020  p.ndarray]:.    
-00029b60: 2222 220a 2020 2020 4372 6561 7465 2061  """.    Create a
-00029b70: 6e20 696d 6167 6520 7265 7072 6573 656e  n image represen
-00029b80: 7469 6e67 2074 6865 2061 7665 7261 6765  ting the average
-00029b90: 2066 7261 6d65 206f 6620 6120 7365 676d   frame of a segm
-00029ba0: 656e 7420 696e 2061 2076 6964 656f 206f  ent in a video o
-00029bb0: 7220 616e 2065 6e74 6972 6520 7669 6465  r an entire vide
-00029bc0: 6f2e 0a0a 2020 2020 2e2e 206e 6f74 653a  o...    .. note:
-00029bd0: 3a0a 2020 2020 2020 2055 7365 6675 6c20  :.       Useful 
-00029be0: 6865 6c70 6572 2066 6f72 2065 2e67 2e2c  helper for e.g.,
-00029bf0: 2076 6964 656f 2062 6163 6b67 726f 756e   video backgroun
-00029c00: 6420 7375 6274 7261 6374 696f 6e20 6060  d subtraction ``
-00029c10: 7369 6d62 612e 7669 6465 6f5f 7072 6f63  simba.video_proc
-00029c20: 6573 736f 7273 2e76 6964 656f 5f70 726f  essors.video_pro
-00029c30: 6365 7373 696e 672e 7669 6465 6f5f 6267  cessing.video_bg
-00029c40: 5f73 7562 7374 7261 6374 696f 6e28 2960  _substraction()`
-00029c50: 600a 2020 2020 2020 2045 6974 6865 7220  `.       Either 
-00029c60: 7061 7373 2060 6073 7461 7274 5f66 726d  pass ``start_frm
-00029c70: 6060 2061 6e64 2060 6065 6e64 5f66 726d  `` and ``end_frm
-00029c80: 6060 204f 5220 6060 7374 6172 745f 7469  `` OR ``start_ti
-00029c90: 6d65 6060 2061 6e64 2060 6065 6e64 5f74  me`` and ``end_t
-00029ca0: 696d 6560 6020 4f52 2070 6173 7320 616c  ime`` OR pass al
-00029cb0: 6c20 666f 7572 2061 7267 756d 656e 7473  l four arguments
-00029cc0: 2061 7320 4e6f 6e65 2e0a 2020 2020 2020   as None..      
-00029cd0: 2049 6620 616c 6c20 6172 6520 4e6f 6e65   If all are None
-00029ce0: 2c20 7468 656e 2074 6865 2065 6e74 6972  , then the entir
-00029cf0: 6520 7669 6465 6f20 7769 6c6c 2062 6520  e video will be 
-00029d00: 7573 6564 2074 6f20 6372 6561 7465 2074  used to create t
-00029d10: 6865 2061 7665 7261 6765 2066 7261 6d65  he average frame
-00029d20: 2e0a 0a20 2020 203a 7061 7261 6d20 556e  ...    :param Un
-00029d30: 696f 6e5b 7374 722c 206f 732e 5061 7468  ion[str, os.Path
-00029d40: 4c69 6b65 5d20 7669 6465 6f5f 7061 7468  Like] video_path
-00029d50: 3a20 5468 6520 7061 7468 2074 6f20 7468  : The path to th
-00029d60: 6520 7669 6465 6f20 746f 2063 7265 6174  e video to creat
-00029d70: 6520 7468 6520 6176 6572 6167 6520 6672  e the average fr
-00029d80: 616d 6520 6672 6f6d 2e20 4465 6661 756c  ame from. Defaul
-00029d90: 743a 204e 6f6e 652e 0a20 2020 203a 7061  t: None..    :pa
-00029da0: 7261 6d20 4f70 7469 6f6e 616c 5b69 6e74  ram Optional[int
-00029db0: 5d20 7374 6172 745f 6672 6d3a 2054 6865  ] start_frm: The
-00029dc0: 2066 6972 7374 2066 7261 6d65 2069 6e20   first frame in 
-00029dd0: 7468 6520 7365 676d 656e 7420 746f 2063  the segment to c
-00029de0: 7265 6174 6520 7468 6520 6176 6572 6167  reate the averag
-00029df0: 6520 6672 616d 6520 6672 6f6d 2e20 4465  e frame from. De
-00029e00: 6661 756c 743a 204e 6f6e 652e 0a20 2020  fault: None..   
-00029e10: 203a 7061 7261 6d20 4f70 7469 6f6e 616c   :param Optional
-00029e20: 5b69 6e74 5d20 656e 645f 6672 6d3a 2054  [int] end_frm: T
-00029e30: 6865 206c 6173 7420 6672 616d 6520 696e  he last frame in
-00029e40: 2074 6865 2073 6567 6d65 6e74 2074 6f20   the segment to 
-00029e50: 6372 6561 7465 2074 6865 2061 7665 7261  create the avera
-00029e60: 6765 2066 7261 6d65 2066 726f 6d2e 2044  ge frame from. D
-00029e70: 6566 6175 6c74 3a20 4e6f 6e65 2e0a 2020  efault: None..  
-00029e80: 2020 3a70 6172 616d 204f 7074 696f 6e61    :param Optiona
-00029e90: 6c5b 7374 725d 2073 7461 7274 5f74 696d  l[str] start_tim
-00029ea0: 653a 2054 6865 2073 7461 7274 2074 696d  e: The start tim
-00029eb0: 6573 7461 6d70 2069 6e20 6048 483a 4d4d  estamp in `HH:MM
-00029ec0: 3a53 5360 2066 6f72 6d61 7420 696e 2074  :SS` format in t
-00029ed0: 6865 2073 6567 6d65 6e74 2074 6f20 6372  he segment to cr
-00029ee0: 6561 7465 2074 6865 2061 7665 7261 6765  eate the average
-00029ef0: 2066 7261 6d65 2066 726f 6d2e 2044 6566   frame from. Def
-00029f00: 6175 6c74 3a20 4e6f 6e65 2e0a 2020 2020  ault: None..    
-00029f10: 3a70 6172 616d 204f 7074 696f 6e61 6c5b  :param Optional[
-00029f20: 7374 725d 2065 6e64 5f74 696d 653a 2054  str] end_time: T
-00029f30: 6865 2065 6e64 2074 696d 6573 7461 6d70  he end timestamp
-00029f40: 2069 6e20 6048 483a 4d4d 3a53 5360 2066   in `HH:MM:SS` f
-00029f50: 6f72 6d61 7420 696e 2074 6865 2073 6567  ormat in the seg
-00029f60: 6d65 6e74 2074 6f20 6372 6561 7465 2074  ment to create t
-00029f70: 6865 2061 7665 7261 6765 2066 7261 6d65  he average frame
-00029f80: 2066 726f 6d2e 2044 6566 6175 6c74 3a20   from. Default: 
-00029f90: 4e6f 6e65 2e0a 2020 2020 3a70 6172 616d  None..    :param
-00029fa0: 204f 7074 696f 6e61 6c5b 556e 696f 6e5b   Optional[Union[
-00029fb0: 7374 722c 206f 732e 5061 7468 4c69 6b65  str, os.PathLike
-00029fc0: 5d5d 2073 6176 655f 7061 7468 3a20 5468  ]] save_path: Th
-00029fd0: 6520 7061 7468 2074 6f20 7768 6572 6520  e path to where 
-00029fe0: 746f 2073 6176 6520 7468 6520 6176 6572  to save the aver
-00029ff0: 6167 6520 696d 6167 652e 2049 6620 4e6f  age image. If No
-0002a000: 6e65 2c20 7468 656e 2072 6561 7475 7265  ne, then reature
-0002a010: 6e73 2074 6865 2061 7665 7261 6765 2069  ns the average i
-0002a020: 6d61 6765 2069 6e20 6e70 2c6e 6461 7272  mage in np,ndarr
-0002a030: 6179 2066 6f72 6d61 742e 2044 6566 6175  ay format. Defau
-0002a040: 6c74 3a20 4e6f 6e65 2e0a 2020 2020 3a72  lt: None..    :r
-0002a050: 6574 7572 6e20 556e 696f 6e5b 4e6f 6e65  eturn Union[None
-0002a060: 2c20 6e70 2e6e 6461 7272 6179 5d3a 2054  , np.ndarray]: T
-0002a070: 6865 2061 7665 7261 6765 2069 6d61 6765  he average image
-0002a080: 2028 6966 2060 6073 6176 655f 7061 7468   (if ``save_path
-0002a090: 6060 2069 7320 6e6f 7420 4e6f 6e65 2920  `` is not None) 
-0002a0a0: 6f72 204e 6f6e 6520 6966 2020 6060 7361  or None if  ``sa
-0002a0b0: 7665 5f70 6174 6860 6020 6973 2070 6173  ve_path`` is pas
-0002a0c0: 7365 642e 0a20 2020 2022 2222 0a0a 2020  sed..    """..  
-0002a0d0: 2020 6966 2028 2873 7461 7274 5f66 726d    if ((start_frm
-0002a0e0: 2069 7320 6e6f 7420 4e6f 6e65 2920 6f72   is not None) or
-0002a0f0: 2028 656e 645f 6672 6d20 6973 206e 6f74   (end_frm is not
-0002a100: 204e 6f6e 6529 2920 616e 6420 2828 7374   None)) and ((st
-0002a110: 6172 745f 7469 6d65 2069 7320 6e6f 7420  art_time is not 
-0002a120: 4e6f 6e65 2920 6f72 2028 656e 645f 7469  None) or (end_ti
-0002a130: 6d65 2069 7320 6e6f 7420 4e6f 6e65 2929  me is not None))
-0002a140: 3a0a 2020 2020 2020 2020 7261 6973 6520  :.        raise 
-0002a150: 496e 7661 6c69 6449 6e70 7574 4572 726f  InvalidInputErro
-0002a160: 7228 6d73 673d 6627 5061 7373 2073 7461  r(msg=f'Pass sta
-0002a170: 7274 5f66 726d 2061 6e64 2065 6e64 5f66  rt_frm and end_f
-0002a180: 726d 204f 5220 7374 6172 745f 7469 6d65  rm OR start_time
-0002a190: 2061 6e64 2065 6e64 5f74 696d 6527 2c0a   and end_time',.
-0002a1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a1c0: 736f 7572 6365 3d63 7265 6174 655f 6176  source=create_av
-0002a1d0: 6572 6167 655f 6672 6d2e 5f5f 6e61 6d65  erage_frm.__name
-0002a1e0: 5f5f 290a 2020 2020 656c 6966 2074 7970  __).    elif typ
-0002a1f0: 6528 7374 6172 745f 6672 6d29 2021 3d20  e(start_frm) != 
-0002a200: 7479 7065 2865 6e64 5f66 726d 293a 0a20  type(end_frm):. 
-0002a210: 2020 2020 2020 2072 6169 7365 2049 6e76         raise Inv
-0002a220: 616c 6964 496e 7075 7445 7272 6f72 286d  alidInputError(m
-0002a230: 7367 3d66 2750 6173 7320 7374 6172 7420  sg=f'Pass start 
-0002a240: 6672 616d 6520 616e 6420 656e 6420 6672  frame and end fr
-0002a250: 616d 6527 2c20 736f 7572 6365 3d63 7265  ame', source=cre
-0002a260: 6174 655f 6176 6572 6167 655f 6672 6d2e  ate_average_frm.
-0002a270: 5f5f 6e61 6d65 5f5f 290a 2020 2020 656c  __name__).    el
-0002a280: 6966 2074 7970 6528 7374 6172 745f 7469  if type(start_ti
-0002a290: 6d65 2920 213d 2074 7970 6528 656e 645f  me) != type(end_
-0002a2a0: 7469 6d65 293a 0a20 2020 2020 2020 2072  time):.        r
-0002a2b0: 6169 7365 2049 6e76 616c 6964 496e 7075  aise InvalidInpu
-0002a2c0: 7445 7272 6f72 286d 7367 3d66 2750 6173  tError(msg=f'Pas
-0002a2d0: 7320 7374 6172 7420 7469 6d65 2061 6e64  s start time and
-0002a2e0: 2065 6e64 2074 696d 6527 2c20 736f 7572   end time', sour
-0002a2f0: 6365 3d63 7265 6174 655f 6176 6572 6167  ce=create_averag
-0002a300: 655f 6672 6d2e 5f5f 6e61 6d65 5f5f 290a  e_frm.__name__).
-0002a310: 2020 2020 6368 6563 6b5f 6669 6c65 5f65      check_file_e
-0002a320: 7869 7374 5f61 6e64 5f72 6561 6461 626c  xist_and_readabl
-0002a330: 6528 6669 6c65 5f70 6174 683d 7669 6465  e(file_path=vide
-0002a340: 6f5f 7061 7468 290a 2020 2020 7669 6465  o_path).    vide
-0002a350: 6f5f 6d65 7461 5f64 6174 6120 3d20 6765  o_meta_data = ge
-0002a360: 745f 7669 6465 6f5f 6d65 7461 5f64 6174  t_video_meta_dat
-0002a370: 6128 7669 6465 6f5f 7061 7468 3d76 6964  a(video_path=vid
-0002a380: 656f 5f70 6174 6829 0a20 2020 2063 6170  eo_path).    cap
-0002a390: 203d 2063 7632 2e56 6964 656f 4361 7074   = cv2.VideoCapt
-0002a3a0: 7572 6528 7669 6465 6f5f 7061 7468 290a  ure(video_path).
-0002a3b0: 2020 2020 6966 2028 7374 6172 745f 6672      if (start_fr
-0002a3c0: 6d20 6973 206e 6f74 204e 6f6e 6529 2061  m is not None) a
-0002a3d0: 6e64 2028 656e 645f 6672 6d20 6973 206e  nd (end_frm is n
-0002a3e0: 6f74 204e 6f6e 6529 3a0a 2020 2020 2020  ot None):.      
-0002a3f0: 2020 6368 6563 6b5f 696e 7428 6e61 6d65    check_int(name
-0002a400: 3d27 7374 6172 745f 6672 6d27 2c20 7661  ='start_frm', va
-0002a410: 6c75 653d 7374 6172 745f 6672 6d2c 206d  lue=start_frm, m
-0002a420: 696e 5f76 616c 7565 3d30 2c20 6d61 785f  in_value=0, max_
-0002a430: 7661 6c75 653d 7669 6465 6f5f 6d65 7461  value=video_meta
-0002a440: 5f64 6174 615b 2766 7261 6d65 5f63 6f75  _data['frame_cou
-0002a450: 6e74 275d 290a 2020 2020 2020 2020 6368  nt']).        ch
-0002a460: 6563 6b5f 696e 7428 6e61 6d65 3d27 656e  eck_int(name='en
-0002a470: 645f 6672 6d27 2c20 7661 6c75 653d 656e  d_frm', value=en
-0002a480: 645f 6672 6d2c 206d 696e 5f76 616c 7565  d_frm, min_value
-0002a490: 3d30 2c20 6d61 785f 7661 6c75 653d 7669  =0, max_value=vi
-0002a4a0: 6465 6f5f 6d65 7461 5f64 6174 615b 2766  deo_meta_data['f
-0002a4b0: 7261 6d65 5f63 6f75 6e74 275d 290a 2020  rame_count']).  
-0002a4c0: 2020 2020 2020 6966 2073 7461 7274 5f66        if start_f
-0002a4d0: 726d 203e 2065 6e64 5f66 726d 3a0a 2020  rm > end_frm:.  
-0002a4e0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-0002a4f0: 496e 7661 6c69 6449 6e70 7574 4572 726f  InvalidInputErro
-0002a500: 7228 6d73 673d 6627 5374 6172 7420 6672  r(msg=f'Start fr
-0002a510: 616d 6520 287b 7374 6172 745f 6672 6d7d  ame ({start_frm}
-0002a520: 2920 6861 7320 746f 2062 6520 6265 666f  ) has to be befo
-0002a530: 7265 2065 6e64 2066 7261 6d65 2028 7b65  re end frame ({e
-0002a540: 6e64 5f66 726d 7d29 2e27 2c0a 2020 2020  nd_frm}).',.    
-0002a550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a570: 736f 7572 6365 3d63 7265 6174 655f 6176  source=create_av
-0002a580: 6572 6167 655f 6672 6d2e 5f5f 6e61 6d65  erage_frm.__name
-0002a590: 5f5f 290a 2020 2020 2020 2020 6672 616d  __).        fram
-0002a5a0: 655f 6964 7320 3d20 6c69 7374 2872 616e  e_ids = list(ran
-0002a5b0: 6765 2873 7461 7274 5f66 726d 2c20 656e  ge(start_frm, en
-0002a5c0: 645f 6672 6d20 2b20 3129 290a 2020 2020  d_frm + 1)).    
-0002a5d0: 656c 6966 2028 7374 6172 745f 7469 6d65  elif (start_time
-0002a5e0: 2069 7320 6e6f 7420 4e6f 6e65 2920 616e   is not None) an
-0002a5f0: 6420 2865 6e64 5f74 696d 6520 6973 206e  d (end_time is n
-0002a600: 6f74 204e 6f6e 6529 3a0a 2020 2020 2020  ot None):.      
-0002a610: 2020 6368 6563 6b5f 6966 5f73 7472 696e    check_if_strin
-0002a620: 675f 7661 6c75 655f 6973 5f76 616c 6964  g_value_is_valid
-0002a630: 5f76 6964 656f 5f74 696d 6573 7461 6d70  _video_timestamp
-0002a640: 2876 616c 7565 3d73 7461 7274 5f74 696d  (value=start_tim
-0002a650: 652c 206e 616d 653d 6372 6561 7465 5f61  e, name=create_a
-0002a660: 7665 7261 6765 5f66 726d 2e5f 5f6e 616d  verage_frm.__nam
-0002a670: 655f 5f29 0a20 2020 2020 2020 2063 6865  e__).        che
-0002a680: 636b 5f69 665f 7374 7269 6e67 5f76 616c  ck_if_string_val
-0002a690: 7565 5f69 735f 7661 6c69 645f 7669 6465  ue_is_valid_vide
-0002a6a0: 6f5f 7469 6d65 7374 616d 7028 7661 6c75  o_timestamp(valu
-0002a6b0: 653d 656e 645f 7469 6d65 2c20 6e61 6d65  e=end_time, name
-0002a6c0: 3d63 7265 6174 655f 6176 6572 6167 655f  =create_average_
-0002a6d0: 6672 6d2e 5f5f 6e61 6d65 5f5f 290a 2020  frm.__name__).  
-0002a6e0: 2020 2020 2020 6368 6563 6b5f 7468 6174        check_that
-0002a6f0: 5f68 686d 6d73 735f 7374 6172 745f 6973  _hhmmss_start_is
-0002a700: 5f62 6566 6f72 655f 656e 6428 7374 6172  _before_end(star
-0002a710: 745f 7469 6d65 3d73 7461 7274 5f74 696d  t_time=start_tim
-0002a720: 652c 2065 6e64 5f74 696d 653d 656e 645f  e, end_time=end_
-0002a730: 7469 6d65 2c0a 2020 2020 2020 2020 2020  time,.          
-0002a740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a760: 2020 2020 6e61 6d65 3d63 7265 6174 655f      name=create_
-0002a770: 6176 6572 6167 655f 6672 6d2e 5f5f 6e61  average_frm.__na
-0002a780: 6d65 5f5f 290a 2020 2020 2020 2020 6368  me__).        ch
-0002a790: 6563 6b5f 6966 5f68 686d 6d73 735f 7469  eck_if_hhmmss_ti
-0002a7a0: 6d65 7374 616d 705f 6973 5f76 616c 6964  mestamp_is_valid
-0002a7b0: 5f70 6172 745f 6f66 5f76 6964 656f 2874  _part_of_video(t
-0002a7c0: 696d 6573 7461 6d70 3d73 7461 7274 5f74  imestamp=start_t
-0002a7d0: 696d 652c 2076 6964 656f 5f70 6174 683d  ime, video_path=
-0002a7e0: 7669 6465 6f5f 7061 7468 290a 2020 2020  video_path).    
-0002a7f0: 2020 2020 6672 616d 655f 6964 7320 3d20      frame_ids = 
-0002a800: 6669 6e64 5f66 7261 6d65 5f6e 756d 6265  find_frame_numbe
-0002a810: 7273 5f66 726f 6d5f 7469 6d65 5f73 7461  rs_from_time_sta
-0002a820: 6d70 2873 7461 7274 5f74 696d 653d 7374  mp(start_time=st
-0002a830: 6172 745f 7469 6d65 2c20 656e 645f 7469  art_time, end_ti
-0002a840: 6d65 3d65 6e64 5f74 696d 652c 0a20 2020  me=end_time,.   
-0002a850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a880: 2020 2020 6670 733d 7669 6465 6f5f 6d65      fps=video_me
-0002a890: 7461 5f64 6174 615b 2766 7073 275d 290a  ta_data['fps']).
-0002a8a0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0002a8b0: 2020 6672 616d 655f 6964 7320 3d20 6c69    frame_ids = li
-0002a8c0: 7374 2872 616e 6765 2830 2c20 7669 6465  st(range(0, vide
-0002a8d0: 6f5f 6d65 7461 5f64 6174 615b 2766 7261  o_meta_data['fra
-0002a8e0: 6d65 5f63 6f75 6e74 275d 2929 0a20 2020  me_count'])).   
-0002a8f0: 2063 6170 2e73 6574 2830 2c20 6672 616d   cap.set(0, fram
-0002a900: 655f 6964 735b 305d 290a 2020 2020 6267  e_ids[0]).    bg
-0002a910: 5f73 756d 2c20 6672 6d5f 636e 742c 2066  _sum, frm_cnt, f
-0002a920: 726d 5f6c 656e 203d 204e 6f6e 652c 2030  rm_len = None, 0
-0002a930: 2c20 6c65 6e28 6672 616d 655f 6964 7329  , len(frame_ids)
-0002a940: 0a20 2020 2077 6869 6c65 2066 726d 5f63  .    while frm_c
-0002a950: 6e74 203c 3d20 6672 6d5f 6c65 6e3a 0a20  nt <= frm_len:. 
-0002a960: 2020 2020 2020 2072 6574 2c20 6672 6d20         ret, frm 
-0002a970: 3d20 6361 702e 7265 6164 2829 0a20 2020  = cap.read().   
-0002a980: 2020 2020 2069 6620 6267 5f73 756d 2069       if bg_sum i
-0002a990: 7320 4e6f 6e65 3a20 6267 5f73 756d 203d  s None: bg_sum =
-0002a9a0: 206e 702e 666c 6f61 7433 3228 6672 6d29   np.float32(frm)
-0002a9b0: 0a20 2020 2020 2020 2065 6c73 653a 2063  .        else: c
-0002a9c0: 7632 2e61 6363 756d 756c 6174 6528 6672  v2.accumulate(fr
-0002a9d0: 6d2c 2062 675f 7375 6d29 0a20 2020 2020  m, bg_sum).     
-0002a9e0: 2020 2066 726d 5f63 6e74 202b 3d20 310a     frm_cnt += 1.
-0002a9f0: 2020 2020 696d 6720 3d20 6376 322e 636f      img = cv2.co
-0002aa00: 6e76 6572 7453 6361 6c65 4162 7328 6267  nvertScaleAbs(bg
-0002aa10: 5f73 756d 202f 2066 726d 5f6c 656e 290a  _sum / frm_len).
-0002aa20: 2020 2020 6361 702e 7265 6c65 6173 6528      cap.release(
-0002aa30: 290a 2020 2020 6966 2073 6176 655f 7061  ).    if save_pa
-0002aa40: 7468 2069 7320 6e6f 7420 4e6f 6e65 3a0a  th is not None:.
-0002aa50: 2020 2020 2020 2020 6368 6563 6b5f 6966          check_if
-0002aa60: 5f64 6972 5f65 7869 7374 7328 696e 5f64  _dir_exists(in_d
-0002aa70: 6972 3d6f 732e 7061 7468 2e64 6972 6e61  ir=os.path.dirna
-0002aa80: 6d65 2873 6176 655f 7061 7468 292c 2073  me(save_path), s
-0002aa90: 6f75 7263 653d 6372 6561 7465 5f61 7665  ource=create_ave
-0002aaa0: 7261 6765 5f66 726d 2e5f 5f6e 616d 655f  rage_frm.__name_
-0002aab0: 5f29 0a20 2020 2020 2020 2063 7632 2e69  _).        cv2.i
-0002aac0: 6d77 7269 7465 2873 6176 655f 7061 7468  mwrite(save_path
-0002aad0: 2c20 696d 6729 0a20 2020 2065 6c73 653a  , img).    else:
-0002aae0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0002aaf0: 696d 670a 0a0a 6465 6620 7669 6465 6f5f  img...def video_
-0002ab00: 6267 5f73 7562 7472 6163 7469 6f6e 2876  bg_subtraction(v
-0002ab10: 6964 656f 5f70 6174 683a 2055 6e69 6f6e  ideo_path: Union
-0002ab20: 5b73 7472 2c20 6f73 2e50 6174 684c 696b  [str, os.PathLik
-0002ab30: 655d 2c0a 2020 2020 2020 2020 2020 2020  e],.            
-0002ab40: 2020 2020 2020 2020 2020 2020 2020 6267                bg
-0002ab50: 5f76 6964 656f 5f70 6174 683a 204f 7074  _video_path: Opt
-0002ab60: 696f 6e61 6c5b 556e 696f 6e5b 7374 722c  ional[Union[str,
-0002ab70: 206f 732e 5061 7468 4c69 6b65 5d5d 203d   os.PathLike]] =
-0002ab80: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
-0002ab90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002aba0: 2062 675f 7374 6172 745f 6672 6d3a 204f   bg_start_frm: O
-0002abb0: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
-0002abc0: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
-0002abd0: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-0002abe0: 675f 656e 645f 6672 6d3a 204f 7074 696f  g_end_frm: Optio
-0002abf0: 6e61 6c5b 696e 745d 203d 204e 6f6e 652c  nal[int] = None,
-0002ac00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002ac10: 2020 2020 2020 2020 2020 2062 675f 7374             bg_st
-0002ac20: 6172 745f 7469 6d65 3a20 4f70 7469 6f6e  art_time: Option
-0002ac30: 616c 5b73 7472 5d20 3d20 4e6f 6e65 2c0a  al[str] = None,.
+00029ad0: 2073 7461 7274 5f74 696d 653a 204f 7074   start_time: Opt
+00029ae0: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+00029af0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00029b00: 2020 2020 2020 2020 2020 656e 645f 7469            end_ti
+00029b10: 6d65 3a20 4f70 7469 6f6e 616c 5b73 7472  me: Optional[str
+00029b20: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+00029b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029b40: 2073 6176 655f 7061 7468 3a20 4f70 7469   save_path: Opti
+00029b50: 6f6e 616c 5b55 6e69 6f6e 5b73 7472 2c20  onal[Union[str, 
+00029b60: 6f73 2e50 6174 684c 696b 655d 5d20 3d20  os.PathLike]] = 
+00029b70: 4e6f 6e65 2920 2d3e 2055 6e69 6f6e 5b4e  None) -> Union[N
+00029b80: 6f6e 652c 206e 702e 6e64 6172 7261 795d  one, np.ndarray]
+00029b90: 3a0a 2020 2020 2222 220a 2020 2020 4372  :.    """.    Cr
+00029ba0: 6561 7465 2061 6e20 696d 6167 6520 7265  eate an image re
+00029bb0: 7072 6573 656e 7469 6e67 2074 6865 2061  presenting the a
+00029bc0: 7665 7261 6765 2066 7261 6d65 206f 6620  verage frame of 
+00029bd0: 6120 7365 676d 656e 7420 696e 2061 2076  a segment in a v
+00029be0: 6964 656f 206f 7220 616e 2065 6e74 6972  ideo or an entir
+00029bf0: 6520 7669 6465 6f2e 0a0a 2020 2020 2e2e  e video...    ..
+00029c00: 206e 6f74 653a 3a0a 2020 2020 2020 2055   note::.       U
+00029c10: 7365 6675 6c20 6865 6c70 6572 2066 6f72  seful helper for
+00029c20: 2065 2e67 2e2c 2076 6964 656f 2062 6163   e.g., video bac
+00029c30: 6b67 726f 756e 6420 7375 6274 7261 6374  kground subtract
+00029c40: 696f 6e20 6060 7369 6d62 612e 7669 6465  ion ``simba.vide
+00029c50: 6f5f 7072 6f63 6573 736f 7273 2e76 6964  o_processors.vid
+00029c60: 656f 5f70 726f 6365 7373 696e 672e 7669  eo_processing.vi
+00029c70: 6465 6f5f 6267 5f73 7562 7374 7261 6374  deo_bg_substract
+00029c80: 696f 6e28 2960 600a 2020 2020 2020 2045  ion()``.       E
+00029c90: 6974 6865 7220 7061 7373 2060 6073 7461  ither pass ``sta
+00029ca0: 7274 5f66 726d 6060 2061 6e64 2060 6065  rt_frm`` and ``e
+00029cb0: 6e64 5f66 726d 6060 204f 5220 6060 7374  nd_frm`` OR ``st
+00029cc0: 6172 745f 7469 6d65 6060 2061 6e64 2060  art_time`` and `
+00029cd0: 6065 6e64 5f74 696d 6560 6020 4f52 2070  `end_time`` OR p
+00029ce0: 6173 7320 616c 6c20 666f 7572 2061 7267  ass all four arg
+00029cf0: 756d 656e 7473 2061 7320 4e6f 6e65 2e0a  uments as None..
+00029d00: 2020 2020 2020 2049 6620 616c 6c20 6172         If all ar
+00029d10: 6520 4e6f 6e65 2c20 7468 656e 2074 6865  e None, then the
+00029d20: 2065 6e74 6972 6520 7669 6465 6f20 7769   entire video wi
+00029d30: 6c6c 2062 6520 7573 6564 2074 6f20 6372  ll be used to cr
+00029d40: 6561 7465 2074 6865 2061 7665 7261 6765  eate the average
+00029d50: 2066 7261 6d65 2e0a 0a20 2020 203a 7061   frame...    :pa
+00029d60: 7261 6d20 556e 696f 6e5b 7374 722c 206f  ram Union[str, o
+00029d70: 732e 5061 7468 4c69 6b65 5d20 7669 6465  s.PathLike] vide
+00029d80: 6f5f 7061 7468 3a20 5468 6520 7061 7468  o_path: The path
+00029d90: 2074 6f20 7468 6520 7669 6465 6f20 746f   to the video to
+00029da0: 2063 7265 6174 6520 7468 6520 6176 6572   create the aver
+00029db0: 6167 6520 6672 616d 6520 6672 6f6d 2e20  age frame from. 
+00029dc0: 4465 6661 756c 743a 204e 6f6e 652e 0a20  Default: None.. 
+00029dd0: 2020 203a 7061 7261 6d20 4f70 7469 6f6e     :param Option
+00029de0: 616c 5b69 6e74 5d20 7374 6172 745f 6672  al[int] start_fr
+00029df0: 6d3a 2054 6865 2066 6972 7374 2066 7261  m: The first fra
+00029e00: 6d65 2069 6e20 7468 6520 7365 676d 656e  me in the segmen
+00029e10: 7420 746f 2063 7265 6174 6520 7468 6520  t to create the 
+00029e20: 6176 6572 6167 6520 6672 616d 6520 6672  average frame fr
+00029e30: 6f6d 2e20 4465 6661 756c 743a 204e 6f6e  om. Default: Non
+00029e40: 652e 0a20 2020 203a 7061 7261 6d20 4f70  e..    :param Op
+00029e50: 7469 6f6e 616c 5b69 6e74 5d20 656e 645f  tional[int] end_
+00029e60: 6672 6d3a 2054 6865 206c 6173 7420 6672  frm: The last fr
+00029e70: 616d 6520 696e 2074 6865 2073 6567 6d65  ame in the segme
+00029e80: 6e74 2074 6f20 6372 6561 7465 2074 6865  nt to create the
+00029e90: 2061 7665 7261 6765 2066 7261 6d65 2066   average frame f
+00029ea0: 726f 6d2e 2044 6566 6175 6c74 3a20 4e6f  rom. Default: No
+00029eb0: 6e65 2e0a 2020 2020 3a70 6172 616d 204f  ne..    :param O
+00029ec0: 7074 696f 6e61 6c5b 7374 725d 2073 7461  ptional[str] sta
+00029ed0: 7274 5f74 696d 653a 2054 6865 2073 7461  rt_time: The sta
+00029ee0: 7274 2074 696d 6573 7461 6d70 2069 6e20  rt timestamp in 
+00029ef0: 6048 483a 4d4d 3a53 5360 2066 6f72 6d61  `HH:MM:SS` forma
+00029f00: 7420 696e 2074 6865 2073 6567 6d65 6e74  t in the segment
+00029f10: 2074 6f20 6372 6561 7465 2074 6865 2061   to create the a
+00029f20: 7665 7261 6765 2066 7261 6d65 2066 726f  verage frame fro
+00029f30: 6d2e 2044 6566 6175 6c74 3a20 4e6f 6e65  m. Default: None
+00029f40: 2e0a 2020 2020 3a70 6172 616d 204f 7074  ..    :param Opt
+00029f50: 696f 6e61 6c5b 7374 725d 2065 6e64 5f74  ional[str] end_t
+00029f60: 696d 653a 2054 6865 2065 6e64 2074 696d  ime: The end tim
+00029f70: 6573 7461 6d70 2069 6e20 6048 483a 4d4d  estamp in `HH:MM
+00029f80: 3a53 5360 2066 6f72 6d61 7420 696e 2074  :SS` format in t
+00029f90: 6865 2073 6567 6d65 6e74 2074 6f20 6372  he segment to cr
+00029fa0: 6561 7465 2074 6865 2061 7665 7261 6765  eate the average
+00029fb0: 2066 7261 6d65 2066 726f 6d2e 2044 6566   frame from. Def
+00029fc0: 6175 6c74 3a20 4e6f 6e65 2e0a 2020 2020  ault: None..    
+00029fd0: 3a70 6172 616d 204f 7074 696f 6e61 6c5b  :param Optional[
+00029fe0: 556e 696f 6e5b 7374 722c 206f 732e 5061  Union[str, os.Pa
+00029ff0: 7468 4c69 6b65 5d5d 2073 6176 655f 7061  thLike]] save_pa
+0002a000: 7468 3a20 5468 6520 7061 7468 2074 6f20  th: The path to 
+0002a010: 7768 6572 6520 746f 2073 6176 6520 7468  where to save th
+0002a020: 6520 6176 6572 6167 6520 696d 6167 652e  e average image.
+0002a030: 2049 6620 4e6f 6e65 2c20 7468 656e 2072   If None, then r
+0002a040: 6561 7475 7265 6e73 2074 6865 2061 7665  eaturens the ave
+0002a050: 7261 6765 2069 6d61 6765 2069 6e20 6e70  rage image in np
+0002a060: 2c6e 6461 7272 6179 2066 6f72 6d61 742e  ,ndarray format.
+0002a070: 2044 6566 6175 6c74 3a20 4e6f 6e65 2e0a   Default: None..
+0002a080: 2020 2020 3a72 6574 7572 6e20 556e 696f      :return Unio
+0002a090: 6e5b 4e6f 6e65 2c20 6e70 2e6e 6461 7272  n[None, np.ndarr
+0002a0a0: 6179 5d3a 2054 6865 2061 7665 7261 6765  ay]: The average
+0002a0b0: 2069 6d61 6765 2028 6966 2060 6073 6176   image (if ``sav
+0002a0c0: 655f 7061 7468 6060 2069 7320 6e6f 7420  e_path`` is not 
+0002a0d0: 4e6f 6e65 2920 6f72 204e 6f6e 6520 6966  None) or None if
+0002a0e0: 2020 6060 7361 7665 5f70 6174 6860 6020    ``save_path`` 
+0002a0f0: 6973 2070 6173 7365 642e 0a20 2020 2022  is passed..    "
+0002a100: 2222 0a0a 2020 2020 6966 2028 2873 7461  ""..    if ((sta
+0002a110: 7274 5f66 726d 2069 7320 6e6f 7420 4e6f  rt_frm is not No
+0002a120: 6e65 2920 6f72 2028 656e 645f 6672 6d20  ne) or (end_frm 
+0002a130: 6973 206e 6f74 204e 6f6e 6529 2920 616e  is not None)) an
+0002a140: 6420 2828 7374 6172 745f 7469 6d65 2069  d ((start_time i
+0002a150: 7320 6e6f 7420 4e6f 6e65 2920 6f72 2028  s not None) or (
+0002a160: 656e 645f 7469 6d65 2069 7320 6e6f 7420  end_time is not 
+0002a170: 4e6f 6e65 2929 3a0a 2020 2020 2020 2020  None)):.        
+0002a180: 7261 6973 6520 496e 7661 6c69 6449 6e70  raise InvalidInp
+0002a190: 7574 4572 726f 7228 6d73 673d 6627 5061  utError(msg=f'Pa
+0002a1a0: 7373 2073 7461 7274 5f66 726d 2061 6e64  ss start_frm and
+0002a1b0: 2065 6e64 5f66 726d 204f 5220 7374 6172   end_frm OR star
+0002a1c0: 745f 7469 6d65 2061 6e64 2065 6e64 5f74  t_time and end_t
+0002a1d0: 696d 6527 2c0a 2020 2020 2020 2020 2020  ime',.          
+0002a1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a1f0: 2020 2020 2020 736f 7572 6365 3d63 7265        source=cre
+0002a200: 6174 655f 6176 6572 6167 655f 6672 6d2e  ate_average_frm.
+0002a210: 5f5f 6e61 6d65 5f5f 290a 2020 2020 656c  __name__).    el
+0002a220: 6966 2074 7970 6528 7374 6172 745f 6672  if type(start_fr
+0002a230: 6d29 2021 3d20 7479 7065 2865 6e64 5f66  m) != type(end_f
+0002a240: 726d 293a 0a20 2020 2020 2020 2072 6169  rm):.        rai
+0002a250: 7365 2049 6e76 616c 6964 496e 7075 7445  se InvalidInputE
+0002a260: 7272 6f72 286d 7367 3d66 2750 6173 7320  rror(msg=f'Pass 
+0002a270: 7374 6172 7420 6672 616d 6520 616e 6420  start frame and 
+0002a280: 656e 6420 6672 616d 6527 2c20 736f 7572  end frame', sour
+0002a290: 6365 3d63 7265 6174 655f 6176 6572 6167  ce=create_averag
+0002a2a0: 655f 6672 6d2e 5f5f 6e61 6d65 5f5f 290a  e_frm.__name__).
+0002a2b0: 2020 2020 656c 6966 2074 7970 6528 7374      elif type(st
+0002a2c0: 6172 745f 7469 6d65 2920 213d 2074 7970  art_time) != typ
+0002a2d0: 6528 656e 645f 7469 6d65 293a 0a20 2020  e(end_time):.   
+0002a2e0: 2020 2020 2072 6169 7365 2049 6e76 616c       raise Inval
+0002a2f0: 6964 496e 7075 7445 7272 6f72 286d 7367  idInputError(msg
+0002a300: 3d66 2750 6173 7320 7374 6172 7420 7469  =f'Pass start ti
+0002a310: 6d65 2061 6e64 2065 6e64 2074 696d 6527  me and end time'
+0002a320: 2c20 736f 7572 6365 3d63 7265 6174 655f  , source=create_
+0002a330: 6176 6572 6167 655f 6672 6d2e 5f5f 6e61  average_frm.__na
+0002a340: 6d65 5f5f 290a 2020 2020 6368 6563 6b5f  me__).    check_
+0002a350: 6669 6c65 5f65 7869 7374 5f61 6e64 5f72  file_exist_and_r
+0002a360: 6561 6461 626c 6528 6669 6c65 5f70 6174  eadable(file_pat
+0002a370: 683d 7669 6465 6f5f 7061 7468 290a 2020  h=video_path).  
+0002a380: 2020 7669 6465 6f5f 6d65 7461 5f64 6174    video_meta_dat
+0002a390: 6120 3d20 6765 745f 7669 6465 6f5f 6d65  a = get_video_me
+0002a3a0: 7461 5f64 6174 6128 7669 6465 6f5f 7061  ta_data(video_pa
+0002a3b0: 7468 3d76 6964 656f 5f70 6174 6829 0a20  th=video_path). 
+0002a3c0: 2020 2063 6170 203d 2063 7632 2e56 6964     cap = cv2.Vid
+0002a3d0: 656f 4361 7074 7572 6528 7669 6465 6f5f  eoCapture(video_
+0002a3e0: 7061 7468 290a 2020 2020 6966 2028 7374  path).    if (st
+0002a3f0: 6172 745f 6672 6d20 6973 206e 6f74 204e  art_frm is not N
+0002a400: 6f6e 6529 2061 6e64 2028 656e 645f 6672  one) and (end_fr
+0002a410: 6d20 6973 206e 6f74 204e 6f6e 6529 3a0a  m is not None):.
+0002a420: 2020 2020 2020 2020 6368 6563 6b5f 696e          check_in
+0002a430: 7428 6e61 6d65 3d27 7374 6172 745f 6672  t(name='start_fr
+0002a440: 6d27 2c20 7661 6c75 653d 7374 6172 745f  m', value=start_
+0002a450: 6672 6d2c 206d 696e 5f76 616c 7565 3d30  frm, min_value=0
+0002a460: 2c20 6d61 785f 7661 6c75 653d 7669 6465  , max_value=vide
+0002a470: 6f5f 6d65 7461 5f64 6174 615b 2766 7261  o_meta_data['fra
+0002a480: 6d65 5f63 6f75 6e74 275d 290a 2020 2020  me_count']).    
+0002a490: 2020 2020 6368 6563 6b5f 696e 7428 6e61      check_int(na
+0002a4a0: 6d65 3d27 656e 645f 6672 6d27 2c20 7661  me='end_frm', va
+0002a4b0: 6c75 653d 656e 645f 6672 6d2c 206d 696e  lue=end_frm, min
+0002a4c0: 5f76 616c 7565 3d30 2c20 6d61 785f 7661  _value=0, max_va
+0002a4d0: 6c75 653d 7669 6465 6f5f 6d65 7461 5f64  lue=video_meta_d
+0002a4e0: 6174 615b 2766 7261 6d65 5f63 6f75 6e74  ata['frame_count
+0002a4f0: 275d 290a 2020 2020 2020 2020 6966 2073  ']).        if s
+0002a500: 7461 7274 5f66 726d 203e 2065 6e64 5f66  tart_frm > end_f
+0002a510: 726d 3a0a 2020 2020 2020 2020 2020 2020  rm:.            
+0002a520: 7261 6973 6520 496e 7661 6c69 6449 6e70  raise InvalidInp
+0002a530: 7574 4572 726f 7228 6d73 673d 6627 5374  utError(msg=f'St
+0002a540: 6172 7420 6672 616d 6520 287b 7374 6172  art frame ({star
+0002a550: 745f 6672 6d7d 2920 6861 7320 746f 2062  t_frm}) has to b
+0002a560: 6520 6265 666f 7265 2065 6e64 2066 7261  e before end fra
+0002a570: 6d65 2028 7b65 6e64 5f66 726d 7d29 2e27  me ({end_frm}).'
+0002a580: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0002a590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a5a0: 2020 2020 2020 736f 7572 6365 3d63 7265        source=cre
+0002a5b0: 6174 655f 6176 6572 6167 655f 6672 6d2e  ate_average_frm.
+0002a5c0: 5f5f 6e61 6d65 5f5f 290a 2020 2020 2020  __name__).      
+0002a5d0: 2020 6672 616d 655f 6964 7320 3d20 6c69    frame_ids = li
+0002a5e0: 7374 2872 616e 6765 2873 7461 7274 5f66  st(range(start_f
+0002a5f0: 726d 2c20 656e 645f 6672 6d20 2b20 3129  rm, end_frm + 1)
+0002a600: 290a 2020 2020 656c 6966 2028 7374 6172  ).    elif (star
+0002a610: 745f 7469 6d65 2069 7320 6e6f 7420 4e6f  t_time is not No
+0002a620: 6e65 2920 616e 6420 2865 6e64 5f74 696d  ne) and (end_tim
+0002a630: 6520 6973 206e 6f74 204e 6f6e 6529 3a0a  e is not None):.
+0002a640: 2020 2020 2020 2020 6368 6563 6b5f 6966          check_if
+0002a650: 5f73 7472 696e 675f 7661 6c75 655f 6973  _string_value_is
+0002a660: 5f76 616c 6964 5f76 6964 656f 5f74 696d  _valid_video_tim
+0002a670: 6573 7461 6d70 2876 616c 7565 3d73 7461  estamp(value=sta
+0002a680: 7274 5f74 696d 652c 206e 616d 653d 6372  rt_time, name=cr
+0002a690: 6561 7465 5f61 7665 7261 6765 5f66 726d  eate_average_frm
+0002a6a0: 2e5f 5f6e 616d 655f 5f29 0a20 2020 2020  .__name__).     
+0002a6b0: 2020 2063 6865 636b 5f69 665f 7374 7269     check_if_stri
+0002a6c0: 6e67 5f76 616c 7565 5f69 735f 7661 6c69  ng_value_is_vali
+0002a6d0: 645f 7669 6465 6f5f 7469 6d65 7374 616d  d_video_timestam
+0002a6e0: 7028 7661 6c75 653d 656e 645f 7469 6d65  p(value=end_time
+0002a6f0: 2c20 6e61 6d65 3d63 7265 6174 655f 6176  , name=create_av
+0002a700: 6572 6167 655f 6672 6d2e 5f5f 6e61 6d65  erage_frm.__name
+0002a710: 5f5f 290a 2020 2020 2020 2020 6368 6563  __).        chec
+0002a720: 6b5f 7468 6174 5f68 686d 6d73 735f 7374  k_that_hhmmss_st
+0002a730: 6172 745f 6973 5f62 6566 6f72 655f 656e  art_is_before_en
+0002a740: 6428 7374 6172 745f 7469 6d65 3d73 7461  d(start_time=sta
+0002a750: 7274 5f74 696d 652c 2065 6e64 5f74 696d  rt_time, end_tim
+0002a760: 653d 656e 645f 7469 6d65 2c0a 2020 2020  e=end_time,.    
+0002a770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a790: 2020 2020 2020 2020 2020 6e61 6d65 3d63            name=c
+0002a7a0: 7265 6174 655f 6176 6572 6167 655f 6672  reate_average_fr
+0002a7b0: 6d2e 5f5f 6e61 6d65 5f5f 290a 2020 2020  m.__name__).    
+0002a7c0: 2020 2020 6368 6563 6b5f 6966 5f68 686d      check_if_hhm
+0002a7d0: 6d73 735f 7469 6d65 7374 616d 705f 6973  mss_timestamp_is
+0002a7e0: 5f76 616c 6964 5f70 6172 745f 6f66 5f76  _valid_part_of_v
+0002a7f0: 6964 656f 2874 696d 6573 7461 6d70 3d73  ideo(timestamp=s
+0002a800: 7461 7274 5f74 696d 652c 2076 6964 656f  tart_time, video
+0002a810: 5f70 6174 683d 7669 6465 6f5f 7061 7468  _path=video_path
+0002a820: 290a 2020 2020 2020 2020 6672 616d 655f  ).        frame_
+0002a830: 6964 7320 3d20 6669 6e64 5f66 7261 6d65  ids = find_frame
+0002a840: 5f6e 756d 6265 7273 5f66 726f 6d5f 7469  _numbers_from_ti
+0002a850: 6d65 5f73 7461 6d70 2873 7461 7274 5f74  me_stamp(start_t
+0002a860: 696d 653d 7374 6172 745f 7469 6d65 2c20  ime=start_time, 
+0002a870: 656e 645f 7469 6d65 3d65 6e64 5f74 696d  end_time=end_tim
+0002a880: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+0002a890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a8b0: 2020 2020 2020 2020 2020 6670 733d 7669            fps=vi
+0002a8c0: 6465 6f5f 6d65 7461 5f64 6174 615b 2766  deo_meta_data['f
+0002a8d0: 7073 275d 290a 2020 2020 656c 7365 3a0a  ps']).    else:.
+0002a8e0: 2020 2020 2020 2020 6672 616d 655f 6964          frame_id
+0002a8f0: 7320 3d20 6c69 7374 2872 616e 6765 2830  s = list(range(0
+0002a900: 2c20 7669 6465 6f5f 6d65 7461 5f64 6174  , video_meta_dat
+0002a910: 615b 2766 7261 6d65 5f63 6f75 6e74 275d  a['frame_count']
+0002a920: 2929 0a20 2020 2063 6170 2e73 6574 2830  )).    cap.set(0
+0002a930: 2c20 6672 616d 655f 6964 735b 305d 290a  , frame_ids[0]).
+0002a940: 2020 2020 6267 5f73 756d 2c20 6672 6d5f      bg_sum, frm_
+0002a950: 636e 742c 2066 726d 5f6c 656e 203d 204e  cnt, frm_len = N
+0002a960: 6f6e 652c 2030 2c20 6c65 6e28 6672 616d  one, 0, len(fram
+0002a970: 655f 6964 7329 0a20 2020 2077 6869 6c65  e_ids).    while
+0002a980: 2066 726d 5f63 6e74 203c 3d20 6672 6d5f   frm_cnt <= frm_
+0002a990: 6c65 6e3a 0a20 2020 2020 2020 2072 6574  len:.        ret
+0002a9a0: 2c20 6672 6d20 3d20 6361 702e 7265 6164  , frm = cap.read
+0002a9b0: 2829 0a20 2020 2020 2020 2069 6620 6267  ().        if bg
+0002a9c0: 5f73 756d 2069 7320 4e6f 6e65 3a20 6267  _sum is None: bg
+0002a9d0: 5f73 756d 203d 206e 702e 666c 6f61 7433  _sum = np.float3
+0002a9e0: 3228 6672 6d29 0a20 2020 2020 2020 2065  2(frm).        e
+0002a9f0: 6c73 653a 2063 7632 2e61 6363 756d 756c  lse: cv2.accumul
+0002aa00: 6174 6528 6672 6d2c 2062 675f 7375 6d29  ate(frm, bg_sum)
+0002aa10: 0a20 2020 2020 2020 2066 726d 5f63 6e74  .        frm_cnt
+0002aa20: 202b 3d20 310a 2020 2020 696d 6720 3d20   += 1.    img = 
+0002aa30: 6376 322e 636f 6e76 6572 7453 6361 6c65  cv2.convertScale
+0002aa40: 4162 7328 6267 5f73 756d 202f 2066 726d  Abs(bg_sum / frm
+0002aa50: 5f6c 656e 290a 2020 2020 6361 702e 7265  _len).    cap.re
+0002aa60: 6c65 6173 6528 290a 2020 2020 6966 2073  lease().    if s
+0002aa70: 6176 655f 7061 7468 2069 7320 6e6f 7420  ave_path is not 
+0002aa80: 4e6f 6e65 3a0a 2020 2020 2020 2020 6368  None:.        ch
+0002aa90: 6563 6b5f 6966 5f64 6972 5f65 7869 7374  eck_if_dir_exist
+0002aaa0: 7328 696e 5f64 6972 3d6f 732e 7061 7468  s(in_dir=os.path
+0002aab0: 2e64 6972 6e61 6d65 2873 6176 655f 7061  .dirname(save_pa
+0002aac0: 7468 292c 2073 6f75 7263 653d 6372 6561  th), source=crea
+0002aad0: 7465 5f61 7665 7261 6765 5f66 726d 2e5f  te_average_frm._
+0002aae0: 5f6e 616d 655f 5f29 0a20 2020 2020 2020  _name__).       
+0002aaf0: 2063 7632 2e69 6d77 7269 7465 2873 6176   cv2.imwrite(sav
+0002ab00: 655f 7061 7468 2c20 696d 6729 0a20 2020  e_path, img).   
+0002ab10: 2065 6c73 653a 0a20 2020 2020 2020 2072   else:.        r
+0002ab20: 6574 7572 6e20 696d 670a 0a0a 6465 6620  eturn img...def 
+0002ab30: 7669 6465 6f5f 6267 5f73 7562 7472 6163  video_bg_subtrac
+0002ab40: 7469 6f6e 2876 6964 656f 5f70 6174 683a  tion(video_path:
+0002ab50: 2055 6e69 6f6e 5b73 7472 2c20 6f73 2e50   Union[str, os.P
+0002ab60: 6174 684c 696b 655d 2c0a 2020 2020 2020  athLike],.      
+0002ab70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002ab80: 2020 2020 6267 5f76 6964 656f 5f70 6174      bg_video_pat
+0002ab90: 683a 204f 7074 696f 6e61 6c5b 556e 696f  h: Optional[Unio
+0002aba0: 6e5b 7374 722c 206f 732e 5061 7468 4c69  n[str, os.PathLi
+0002abb0: 6b65 5d5d 203d 204e 6f6e 652c 0a20 2020  ke]] = None,.   
+0002abc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002abd0: 2020 2020 2020 2062 675f 7374 6172 745f         bg_start_
+0002abe0: 6672 6d3a 204f 7074 696f 6e61 6c5b 696e  frm: Optional[in
+0002abf0: 745d 203d 204e 6f6e 652c 0a20 2020 2020  t] = None,.     
+0002ac00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002ac10: 2020 2020 2062 675f 656e 645f 6672 6d3a       bg_end_frm:
+0002ac20: 204f 7074 696f 6e61 6c5b 696e 745d 203d   Optional[int] =
+0002ac30: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
 0002ac40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002ac50: 2020 2020 2020 2020 2020 6267 5f65 6e64            bg_end
-0002ac60: 5f74 696d 653a 204f 7074 696f 6e61 6c5b  _time: Optional[
-0002ac70: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
+0002ac50: 2062 675f 7374 6172 745f 7469 6d65 3a20   bg_start_time: 
+0002ac60: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+0002ac70: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
 0002ac80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002ac90: 2020 2020 2020 2062 675f 636f 6c6f 723a         bg_color:
-0002aca0: 204f 7074 696f 6e61 6c5b 5475 706c 655b   Optional[Tuple[
-0002acb0: 696e 742c 2069 6e74 2c20 696e 745d 5d20  int, int, int]] 
-0002acc0: 3d20 2830 2c20 302c 2030 292c 0a20 2020  = (0, 0, 0),.   
-0002acd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002ace0: 2020 2020 2020 2066 675f 636f 6c6f 723a         fg_color:
-0002acf0: 204f 7074 696f 6e61 6c5b 5475 706c 655b   Optional[Tuple[
-0002ad00: 696e 742c 2069 6e74 2c20 696e 745d 5d20  int, int, int]] 
-0002ad10: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-0002ad20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002ad30: 2020 7361 7665 5f70 6174 683a 204f 7074    save_path: Opt
-0002ad40: 696f 6e61 6c5b 556e 696f 6e5b 7374 722c  ional[Union[str,
-0002ad50: 206f 732e 5061 7468 4c69 6b65 5d5d 203d   os.PathLike]] =
-0002ad60: 204e 6f6e 6529 202d 3e20 4e6f 6e65 3a0a   None) -> None:.
-0002ad70: 2020 2020 2222 220a 2020 2020 5375 6274      """.    Subt
-0002ad80: 7261 6374 2074 6865 2062 6163 6b67 726f  ract the backgro
-0002ad90: 756e 6420 6672 6f6d 2061 2076 6964 656f  und from a video
-0002ada0: 2e0a 0a20 2020 202e 2e20 7669 6465 6f3a  ...    .. video:
-0002adb0: 3a20 5f73 7461 7469 632f 696d 672f 7669  : _static/img/vi
-0002adc0: 6465 6f5f 6267 5f73 7562 7472 6163 7469  deo_bg_subtracti
-0002add0: 6f6e 2e77 6562 6d0a 2020 2020 2020 203a  on.webm.       :
-0002ade0: 6c6f 6f70 3a0a 0a20 2020 202e 2e20 6e6f  loop:..    .. no
-0002adf0: 7465 3a3a 0a20 2020 2020 2020 4966 2020  te::.       If  
-0002ae00: 6060 6267 5f76 6964 656f 5f70 6174 6860  ``bg_video_path`
-0002ae10: 6020 6973 2070 6173 7365 642c 2074 6861  ` is passed, tha
-0002ae20: 7420 7669 6465 6f20 7769 6c6c 2062 6520  t video will be 
-0002ae30: 7573 6564 2074 6f20 7061 7273 6520 7468  used to parse th
-0002ae40: 6520 6261 636b 6772 6f75 6e64 2e20 4966  e background. If
-0002ae50: 204e 6f6e 652c 2060 6076 6964 656f 5f70   None, ``video_p
-0002ae60: 6174 6860 6020 7769 6c6c 2062 6520 7573  ath`` will be us
-0002ae70: 6520 6474 6f20 7061 7273 6520 6261 636b  e dto parse back
-0002ae80: 6772 6f75 6e64 2e0a 2020 2020 2020 2045  ground..       E
-0002ae90: 6974 6865 7220 7061 7373 2060 6073 7461  ither pass ``sta
-0002aea0: 7274 5f66 726d 6060 2061 6e64 2060 6065  rt_frm`` and ``e
-0002aeb0: 6e64 5f66 726d 6060 204f 5220 6060 7374  nd_frm`` OR ``st
-0002aec0: 6172 745f 7469 6d65 6060 2061 6e64 2060  art_time`` and `
-0002aed0: 6065 6e64 5f74 696d 6560 6020 4f52 2070  `end_time`` OR p
-0002aee0: 6173 7320 616c 6c20 666f 7572 2061 7267  ass all four arg
-0002aef0: 756d 656e 7473 2061 7320 4e6f 6e65 2e0a  uments as None..
-0002af00: 2020 2020 2020 2054 686f 7365 2074 776f         Those two
-0002af10: 2061 7267 756d 656e 7473 2077 696c 6c20   arguments will 
-0002af20: 6265 2075 7365 6420 746f 2073 6c69 6365  be used to slice
-0002af30: 2074 6865 2062 6163 6b67 726f 756e 6420   the background 
-0002af40: 7669 6465 6f2c 2061 6e64 2074 6865 2073  video, and the s
-0002af50: 6c69 6365 6420 7061 7274 2069 7320 7573  liced part is us
-0002af60: 6564 2074 6f20 7061 7273 6520 7468 6520  ed to parse the 
-0002af70: 6261 636b 6772 6f75 6e64 2e0a 0a20 2020  background...   
-0002af80: 2020 2020 466f 7220 6578 616d 706c 652c      For example,
-0002af90: 2069 6e20 7468 6520 7363 656e 6172 696f   in the scenario
-0002afa0: 2077 6865 7265 2074 6865 7265 2069 7320   where there is 
-0002afb0: 2a2a 6e6f 2a2a 2061 6e69 6d61 6c20 696e  **no** animal in
-0002afc0: 2074 6865 2060 6076 6964 656f 5f70 6174   the ``video_pat
-0002afd0: 6860 6020 7669 6465 6f20 666f 7220 7468  h`` video for th
-0002afe0: 6520 6669 7273 7420 3230 732c 2074 6865  e first 20s, the
-0002aff0: 6e20 7468 6520 6669 7273 7420 3230 7320  n the first 20s 
-0002b000: 6361 6e20 6265 2075 7365 6420 746f 2070  can be used to p
-0002b010: 6172 7365 2074 6865 2062 6163 6b67 726f  arse the backgro
-0002b020: 756e 642e 0a20 2020 2020 2020 496e 2074  und..       In t
-0002b030: 6869 7320 7363 656e 6172 696f 2c20 6060  his scenario, ``
-0002b040: 6267 5f76 6964 656f 5f70 6174 6860 6020  bg_video_path`` 
-0002b050: 6361 6e20 6265 2070 6173 7365 6420 6173  can be passed as
-0002b060: 2060 604e 6f6e 6560 6020 616e 6420 6267   ``None`` and bg
-0002b070: 5f73 7461 7274 5f74 696d 6520 616e 6420  _start_time and 
-0002b080: 6267 5f65 6e64 5f74 696d 6520 6361 6e20  bg_end_time can 
-0002b090: 6265 2060 6030 303a 3030 3a30 3060 6020  be ``00:00:00`` 
-0002b0a0: 616e 6420 6060 3030 3a30 303a 3230 6060  and ``00:00:20``
-0002b0b0: 2c20 7265 7065 6374 6976 656c 792e 0a0a  , repectively...
-0002b0c0: 2020 2020 2020 2049 6e20 7468 6520 7363         In the sc
-0002b0d0: 656e 6172 696f 2077 6865 7265 2074 6865  enario where the
-0002b0e0: 7265 202a 2a69 732a 2a20 616e 696d 616c  re **is** animal
-0002b0f0: 2873 2920 696e 2074 6865 2065 6e74 6972  (s) in the entir
-0002b100: 6520 6060 7669 6465 6f5f 7061 7468 6060  e ``video_path``
-0002b110: 2076 6964 656f 2c20 7061 7373 2060 6062   video, pass ``b
-0002b120: 675f 7669 6465 6f5f 7061 7468 6060 2061  g_video_path`` a
-0002b130: 7320 6120 7061 7468 2074 6f20 6120 7669  s a path to a vi
-0002b140: 6465 6f20 7265 636f 7264 696e 6720 7468  deo recording th
-0002b150: 6520 6172 656e 6120 7769 7468 6f75 7420  e arena without 
-0002b160: 7468 6520 616e 696d 616c 732e 0a0a 2020  the animals...  
-0002b170: 2020 3a70 6172 616d 2055 6e69 6f6e 5b73    :param Union[s
-0002b180: 7472 2c20 6f73 2e50 6174 684c 696b 655d  tr, os.PathLike]
-0002b190: 2076 6964 656f 5f70 6174 683a 2054 6865   video_path: The
-0002b1a0: 2070 6174 6820 746f 2074 6865 2076 6964   path to the vid
-0002b1b0: 656f 2074 6f20 7265 6d6f 7665 2074 6865  eo to remove the
-0002b1c0: 2062 6163 6b67 726f 756e 6420 6672 6f6d   background from
-0002b1d0: 2e0a 2020 2020 3a70 6172 616d 204f 7074  ..    :param Opt
-0002b1e0: 696f 6e61 6c5b 556e 696f 6e5b 7374 722c  ional[Union[str,
-0002b1f0: 206f 732e 5061 7468 4c69 6b65 5d5d 2062   os.PathLike]] b
-0002b200: 675f 7669 6465 6f5f 7061 7468 3a20 5061  g_video_path: Pa
-0002b210: 7468 2074 6f20 7468 6520 7669 6465 6f20  th to the video 
-0002b220: 7768 6963 6820 636f 6e74 6169 6e73 2061  which contains a
-0002b230: 2073 6567 6d65 6e74 2077 6974 6820 7468   segment with th
-0002b240: 6520 6261 636b 6772 6f75 6e64 206f 6e6c  e background onl
-0002b250: 792e 2049 6620 4e6f 6e65 2c20 7468 656e  y. If None, then
-0002b260: 2060 6076 6964 656f 5f70 6174 6860 6020   ``video_path`` 
-0002b270: 7769 6c6c 2062 6520 7573 6564 2e0a 2020  will be used..  
-0002b280: 2020 3a70 6172 616d 204f 7074 696f 6e61    :param Optiona
-0002b290: 6c5b 696e 745d 2062 675f 7374 6172 745f  l[int] bg_start_
-0002b2a0: 6672 6d3a 2054 6865 2066 6972 7374 2066  frm: The first f
-0002b2b0: 7261 6d65 2069 6e20 7468 6520 6261 636b  rame in the back
-0002b2c0: 6772 6f75 6e64 2076 6964 656f 2074 6f20  ground video to 
-0002b2d0: 7573 6520 7768 656e 2063 7265 6174 696e  use when creatin
-0002b2e0: 6720 6120 7265 7072 6573 656e 7461 7469  g a representati
-0002b2f0: 7665 2062 6163 6b67 726f 756e 6420 696d  ve background im
-0002b300: 6167 652e 2044 6566 6175 6c74 3a20 4e6f  age. Default: No
-0002b310: 6e65 2e0a 2020 2020 3a70 6172 616d 204f  ne..    :param O
-0002b320: 7074 696f 6e61 6c5b 696e 745d 2062 675f  ptional[int] bg_
-0002b330: 656e 645f 6672 6d3a 2054 6865 206c 6173  end_frm: The las
-0002b340: 7420 6672 616d 6520 696e 2074 6865 2062  t frame in the b
-0002b350: 6163 6b67 726f 756e 6420 7669 6465 6f20  ackground video 
-0002b360: 746f 2075 7365 2077 6865 6e20 6372 6561  to use when crea
-0002b370: 7469 6e67 2061 2072 6570 7265 7365 6e74  ting a represent
-0002b380: 6174 6976 6520 6261 636b 6772 6f75 6e64  ative background
-0002b390: 2069 6d61 6765 2e20 4465 6661 756c 743a   image. Default:
-0002b3a0: 204e 6f6e 652e 0a20 2020 203a 7061 7261   None..    :para
-0002b3b0: 6d20 4f70 7469 6f6e 616c 5b73 7472 5d20  m Optional[str] 
-0002b3c0: 6267 5f73 7461 7274 5f74 696d 653a 2054  bg_start_time: T
-0002b3d0: 6865 2073 7461 7274 2074 696d 6573 7461  he start timesta
-0002b3e0: 6d70 2069 6e20 6048 483a 4d4d 3a53 5360  mp in `HH:MM:SS`
-0002b3f0: 2066 6f72 6d61 7420 696e 2074 6865 2062   format in the b
-0002b400: 6163 6b67 726f 756e 6420 7669 6465 6f20  ackground video 
-0002b410: 746f 2075 7365 2074 6f20 6372 6561 7465  to use to create
-0002b420: 2061 2072 6570 7265 7365 6e74 6174 6976   a representativ
-0002b430: 6520 6261 636b 6772 6f75 6e64 2069 6d61  e background ima
-0002b440: 6765 2e20 4465 6661 756c 743a 204e 6f6e  ge. Default: Non
-0002b450: 652e 0a20 2020 203a 7061 7261 6d20 4f70  e..    :param Op
-0002b460: 7469 6f6e 616c 5b73 7472 5d20 6267 5f65  tional[str] bg_e
-0002b470: 6e64 5f74 696d 653a 2054 6865 2065 6e64  nd_time: The end
-0002b480: 2074 696d 6573 7461 6d70 2069 6e20 6048   timestamp in `H
-0002b490: 483a 4d4d 3a53 5360 2066 6f72 6d61 7420  H:MM:SS` format 
-0002b4a0: 696e 2074 6865 2062 6163 6b67 726f 756e  in the backgroun
-0002b4b0: 6420 7669 6465 6f20 746f 2075 7365 2074  d video to use t
-0002b4c0: 6f20 6372 6561 7465 2061 2072 6570 7265  o create a repre
-0002b4d0: 7365 6e74 6174 6976 6520 6261 636b 6772  sentative backgr
-0002b4e0: 6f75 6e64 2069 6d61 6765 2e20 4465 6661  ound image. Defa
-0002b4f0: 756c 743a 204e 6f6e 652e 0a20 2020 203a  ult: None..    :
-0002b500: 7061 7261 6d20 4f70 7469 6f6e 616c 5b54  param Optional[T
-0002b510: 7570 6c65 5b69 6e74 2c20 696e 742c 2069  uple[int, int, i
-0002b520: 6e74 5d5d 2062 675f 636f 6c6f 723a 2054  nt]] bg_color: T
-0002b530: 6865 2052 4742 2063 6f6c 6f72 206f 6620  he RGB color of 
-0002b540: 7468 6520 6d6f 7669 6e67 206f 626a 6563  the moving objec
-0002b550: 7473 2069 6e20 7468 6520 6f75 7470 7574  ts in the output
-0002b560: 2076 6964 656f 2e20 4465 6661 756c 7473   video. Defaults
-0002b570: 2074 6f20 4e6f 6e65 2c20 7768 6963 6820   to None, which 
-0002b580: 7265 7072 6573 656e 7473 2074 6865 206f  represents the o
-0002b590: 7269 6769 6e61 6c20 636f 6c6f 7273 206f  riginal colors o
-0002b5a0: 6620 7468 6520 6d6f 7669 6e67 206f 626a  f the moving obj
-0002b5b0: 6563 7473 2e0a 2020 2020 3a70 6172 616d  ects..    :param
-0002b5c0: 204f 7074 696f 6e61 6c5b 5475 706c 655b   Optional[Tuple[
-0002b5d0: 696e 742c 2069 6e74 2c20 696e 745d 5d20  int, int, int]] 
-0002b5e0: 6667 5f63 6f6c 6f72 3a20 5468 6520 5247  fg_color: The RG
-0002b5f0: 4220 636f 6c6f 7220 6f66 2074 6865 2062  B color of the b
-0002b600: 6163 6b67 726f 756e 6420 6f75 7470 7574  ackground output
-0002b610: 2076 6964 656f 2e20 4465 6661 756c 7473   video. Defaults
-0002b620: 2074 6f20 626c 6163 6b20 2830 2c20 302c   to black (0, 0,
-0002b630: 2030 292e 0a20 2020 203a 7061 7261 6d20   0)..    :param 
-0002b640: 4f70 7469 6f6e 616c 5b55 6e69 6f6e 5b73  Optional[Union[s
-0002b650: 7472 2c20 6f73 2e50 6174 684c 696b 655d  tr, os.PathLike]
-0002b660: 5d20 7361 7665 5f70 6174 683a 2054 6865  ] save_path: The
-0002b670: 2070 6174 6368 2074 6f20 7768 6572 6520   patch to where 
-0002b680: 746f 2073 6176 6520 7468 6520 6f75 7470  to save the outp
-0002b690: 7574 2076 6964 656f 2077 6865 7265 2074  ut video where t
-0002b6a0: 6865 2062 6163 6b67 726f 756e 6420 6973  he background is
-0002b6b0: 2072 656d 6f76 6564 2e20 4966 204e 6f6e   removed. If Non
-0002b6c0: 652c 2073 6176 6573 2074 6865 206f 7574  e, saves the out
-0002b6d0: 7075 7420 7669 6465 6f20 696e 2074 6865  put video in the
-0002b6e0: 2073 616d 6520 6469 7265 6374 6f72 7920   same directory 
-0002b6f0: 6173 2074 6865 2069 6e70 7574 2076 6964  as the input vid
-0002b700: 656f 2077 6974 6820 7468 6520 6060 5f62  eo with the ``_b
-0002b710: 675f 7375 6274 7261 6374 6564 6060 2073  g_subtracted`` s
-0002b720: 7566 6669 782e 2044 6566 6175 6c74 3a20  uffix. Default: 
-0002b730: 4e6f 6e65 2e0a 2020 2020 3a72 6574 7572  None..    :retur
-0002b740: 6e3a 204e 6f6e 652e 0a0a 2020 2020 3a65  n: None...    :e
-0002b750: 7861 6d70 6c65 3a0a 2020 2020 3e3e 3e20  xample:.    >>> 
-0002b760: 7669 6465 6f5f 6267 5f73 7562 7472 6163  video_bg_subtrac
-0002b770: 7469 6f6e 2876 6964 656f 5f70 6174 683d  tion(video_path=
-0002b780: 272f 5573 6572 732f 7369 6d6f 6e2f 446f  '/Users/simon/Do
-0002b790: 776e 6c6f 6164 732f 315f 4c48 5f63 726f  wnloads/1_LH_cro
-0002b7a0: 7070 6564 2e6d 7034 272c 2062 675f 7374  pped.mp4', bg_st
-0002b7b0: 6172 745f 7469 6d65 3d27 3030 3a30 303a  art_time='00:00:
-0002b7c0: 3030 272c 2062 675f 656e 645f 7469 6d65  00', bg_end_time
-0002b7d0: 3d27 3030 3a30 303a 3130 272c 2062 675f  ='00:00:10', bg_
-0002b7e0: 636f 6c6f 723d 2830 2c20 3130 362c 2031  color=(0, 106, 1
-0002b7f0: 3637 292c 2066 675f 636f 6c6f 723d 2832  67), fg_color=(2
-0002b800: 3534 2c20 3230 342c 2032 2929 0a20 2020  54, 204, 2)).   
-0002b810: 2022 2222 0a0a 2020 2020 7469 6d65 7220   """..    timer 
-0002b820: 3d20 5369 6d62 6154 696d 6572 2873 7461  = SimbaTimer(sta
-0002b830: 7274 3d54 7275 6529 0a20 2020 2063 6865  rt=True).    che
-0002b840: 636b 5f66 696c 655f 6578 6973 745f 616e  ck_file_exist_an
-0002b850: 645f 7265 6164 6162 6c65 2866 696c 655f  d_readable(file_
-0002b860: 7061 7468 3d76 6964 656f 5f70 6174 6829  path=video_path)
-0002b870: 0a20 2020 2069 6620 6267 5f76 6964 656f  .    if bg_video
-0002b880: 5f70 6174 6820 6973 204e 6f6e 653a 0a20  _path is None:. 
-0002b890: 2020 2020 2020 2062 675f 7669 6465 6f5f         bg_video_
-0002b8a0: 7061 7468 203d 2064 6565 7063 6f70 7928  path = deepcopy(
-0002b8b0: 7669 6465 6f5f 7061 7468 290a 2020 2020  video_path).    
-0002b8c0: 7669 6465 6f5f 6d65 7461 5f64 6174 6120  video_meta_data 
-0002b8d0: 3d20 6765 745f 7669 6465 6f5f 6d65 7461  = get_video_meta
-0002b8e0: 5f64 6174 6128 7669 6465 6f5f 7061 7468  _data(video_path
-0002b8f0: 3d76 6964 656f 5f70 6174 6829 0a20 2020  =video_path).   
-0002b900: 2064 6972 2c20 7669 6465 6f5f 6e61 6d65   dir, video_name
-0002b910: 2c20 6578 7420 3d20 6765 745f 666e 5f65  , ext = get_fn_e
-0002b920: 7874 2866 696c 6570 6174 683d 7669 6465  xt(filepath=vide
-0002b930: 6f5f 7061 7468 290a 2020 2020 6966 2073  o_path).    if s
-0002b940: 6176 655f 7061 7468 2069 7320 4e6f 6e65  ave_path is None
-0002b950: 3a0a 2020 2020 2020 2020 7361 7665 5f70  :.        save_p
-0002b960: 6174 6820 3d20 6f73 2e70 6174 682e 6a6f  ath = os.path.jo
-0002b970: 696e 2864 6972 2c20 6627 7b76 6964 656f  in(dir, f'{video
-0002b980: 5f6e 616d 657d 5f62 675f 7375 6274 7261  _name}_bg_subtra
-0002b990: 6374 6564 7b65 7874 7d27 290a 2020 2020  cted{ext}').    
-0002b9a0: 666f 7572 6363 203d 2063 7632 2e56 6964  fourcc = cv2.Vid
-0002b9b0: 656f 5772 6974 6572 5f66 6f75 7263 6328  eoWriter_fourcc(
-0002b9c0: 2a46 6f72 6d61 7473 2e4d 5034 5f43 4f44  *Formats.MP4_COD
-0002b9d0: 4543 2e76 616c 7565 290a 2020 2020 7772  EC.value).    wr
-0002b9e0: 6974 6572 203d 2063 7632 2e56 6964 656f  iter = cv2.Video
-0002b9f0: 5772 6974 6572 2873 6176 655f 7061 7468  Writer(save_path
-0002ba00: 2c20 666f 7572 6363 2c20 7669 6465 6f5f  , fourcc, video_
-0002ba10: 6d65 7461 5f64 6174 615b 2766 7073 275d  meta_data['fps']
-0002ba20: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0002ba30: 2020 2020 2020 2020 2020 2020 2020 2028                 (
+0002ac90: 6267 5f65 6e64 5f74 696d 653a 204f 7074  bg_end_time: Opt
+0002aca0: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+0002acb0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+0002acc0: 2020 2020 2020 2020 2020 2020 2062 675f               bg_
+0002acd0: 636f 6c6f 723a 204f 7074 696f 6e61 6c5b  color: Optional[
+0002ace0: 5475 706c 655b 696e 742c 2069 6e74 2c20  Tuple[int, int, 
+0002acf0: 696e 745d 5d20 3d20 2830 2c20 302c 2030  int]] = (0, 0, 0
+0002ad00: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+0002ad10: 2020 2020 2020 2020 2020 2020 2066 675f               fg_
+0002ad20: 636f 6c6f 723a 204f 7074 696f 6e61 6c5b  color: Optional[
+0002ad30: 5475 706c 655b 696e 742c 2069 6e74 2c20  Tuple[int, int, 
+0002ad40: 696e 745d 5d20 3d20 4e6f 6e65 2c0a 2020  int]] = None,.  
+0002ad50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002ad60: 2020 2020 2020 2020 7361 7665 5f70 6174          save_pat
+0002ad70: 683a 204f 7074 696f 6e61 6c5b 556e 696f  h: Optional[Unio
+0002ad80: 6e5b 7374 722c 206f 732e 5061 7468 4c69  n[str, os.PathLi
+0002ad90: 6b65 5d5d 203d 204e 6f6e 6529 202d 3e20  ke]] = None) -> 
+0002ada0: 4e6f 6e65 3a0a 2020 2020 2222 220a 2020  None:.    """.  
+0002adb0: 2020 5375 6274 7261 6374 2074 6865 2062    Subtract the b
+0002adc0: 6163 6b67 726f 756e 6420 6672 6f6d 2061  ackground from a
+0002add0: 2076 6964 656f 2e0a 0a20 2020 202e 2e20   video...    .. 
+0002ade0: 7669 6465 6f3a 3a20 5f73 7461 7469 632f  video:: _static/
+0002adf0: 696d 672f 7669 6465 6f5f 6267 5f73 7562  img/video_bg_sub
+0002ae00: 7472 6163 7469 6f6e 2e77 6562 6d0a 2020  traction.webm.  
+0002ae10: 2020 2020 203a 6c6f 6f70 3a0a 0a20 2020       :loop:..   
+0002ae20: 202e 2e20 6e6f 7465 3a3a 0a20 2020 2020   .. note::.     
+0002ae30: 2020 4966 2020 6060 6267 5f76 6964 656f    If  ``bg_video
+0002ae40: 5f70 6174 6860 6020 6973 2070 6173 7365  _path`` is passe
+0002ae50: 642c 2074 6861 7420 7669 6465 6f20 7769  d, that video wi
+0002ae60: 6c6c 2062 6520 7573 6564 2074 6f20 7061  ll be used to pa
+0002ae70: 7273 6520 7468 6520 6261 636b 6772 6f75  rse the backgrou
+0002ae80: 6e64 2e20 4966 204e 6f6e 652c 2060 6076  nd. If None, ``v
+0002ae90: 6964 656f 5f70 6174 6860 6020 7769 6c6c  ideo_path`` will
+0002aea0: 2062 6520 7573 6520 6474 6f20 7061 7273   be use dto pars
+0002aeb0: 6520 6261 636b 6772 6f75 6e64 2e0a 2020  e background..  
+0002aec0: 2020 2020 2045 6974 6865 7220 7061 7373       Either pass
+0002aed0: 2060 6073 7461 7274 5f66 726d 6060 2061   ``start_frm`` a
+0002aee0: 6e64 2060 6065 6e64 5f66 726d 6060 204f  nd ``end_frm`` O
+0002aef0: 5220 6060 7374 6172 745f 7469 6d65 6060  R ``start_time``
+0002af00: 2061 6e64 2060 6065 6e64 5f74 696d 6560   and ``end_time`
+0002af10: 6020 4f52 2070 6173 7320 616c 6c20 666f  ` OR pass all fo
+0002af20: 7572 2061 7267 756d 656e 7473 2061 7320  ur arguments as 
+0002af30: 4e6f 6e65 2e0a 2020 2020 2020 2054 686f  None..       Tho
+0002af40: 7365 2074 776f 2061 7267 756d 656e 7473  se two arguments
+0002af50: 2077 696c 6c20 6265 2075 7365 6420 746f   will be used to
+0002af60: 2073 6c69 6365 2074 6865 2062 6163 6b67   slice the backg
+0002af70: 726f 756e 6420 7669 6465 6f2c 2061 6e64  round video, and
+0002af80: 2074 6865 2073 6c69 6365 6420 7061 7274   the sliced part
+0002af90: 2069 7320 7573 6564 2074 6f20 7061 7273   is used to pars
+0002afa0: 6520 7468 6520 6261 636b 6772 6f75 6e64  e the background
+0002afb0: 2e0a 0a20 2020 2020 2020 466f 7220 6578  ...       For ex
+0002afc0: 616d 706c 652c 2069 6e20 7468 6520 7363  ample, in the sc
+0002afd0: 656e 6172 696f 2077 6865 7265 2074 6865  enario where the
+0002afe0: 7265 2069 7320 2a2a 6e6f 2a2a 2061 6e69  re is **no** ani
+0002aff0: 6d61 6c20 696e 2074 6865 2060 6076 6964  mal in the ``vid
+0002b000: 656f 5f70 6174 6860 6020 7669 6465 6f20  eo_path`` video 
+0002b010: 666f 7220 7468 6520 6669 7273 7420 3230  for the first 20
+0002b020: 732c 2074 6865 6e20 7468 6520 6669 7273  s, then the firs
+0002b030: 7420 3230 7320 6361 6e20 6265 2075 7365  t 20s can be use
+0002b040: 6420 746f 2070 6172 7365 2074 6865 2062  d to parse the b
+0002b050: 6163 6b67 726f 756e 642e 0a20 2020 2020  ackground..     
+0002b060: 2020 496e 2074 6869 7320 7363 656e 6172    In this scenar
+0002b070: 696f 2c20 6060 6267 5f76 6964 656f 5f70  io, ``bg_video_p
+0002b080: 6174 6860 6020 6361 6e20 6265 2070 6173  ath`` can be pas
+0002b090: 7365 6420 6173 2060 604e 6f6e 6560 6020  sed as ``None`` 
+0002b0a0: 616e 6420 6267 5f73 7461 7274 5f74 696d  and bg_start_tim
+0002b0b0: 6520 616e 6420 6267 5f65 6e64 5f74 696d  e and bg_end_tim
+0002b0c0: 6520 6361 6e20 6265 2060 6030 303a 3030  e can be ``00:00
+0002b0d0: 3a30 3060 6020 616e 6420 6060 3030 3a30  :00`` and ``00:0
+0002b0e0: 303a 3230 6060 2c20 7265 7065 6374 6976  0:20``, repectiv
+0002b0f0: 656c 792e 0a0a 2020 2020 2020 2049 6e20  ely...       In 
+0002b100: 7468 6520 7363 656e 6172 696f 2077 6865  the scenario whe
+0002b110: 7265 2074 6865 7265 202a 2a69 732a 2a20  re there **is** 
+0002b120: 616e 696d 616c 2873 2920 696e 2074 6865  animal(s) in the
+0002b130: 2065 6e74 6972 6520 6060 7669 6465 6f5f   entire ``video_
+0002b140: 7061 7468 6060 2076 6964 656f 2c20 7061  path`` video, pa
+0002b150: 7373 2060 6062 675f 7669 6465 6f5f 7061  ss ``bg_video_pa
+0002b160: 7468 6060 2061 7320 6120 7061 7468 2074  th`` as a path t
+0002b170: 6f20 6120 7669 6465 6f20 7265 636f 7264  o a video record
+0002b180: 696e 6720 7468 6520 6172 656e 6120 7769  ing the arena wi
+0002b190: 7468 6f75 7420 7468 6520 616e 696d 616c  thout the animal
+0002b1a0: 732e 0a0a 2020 2020 3a70 6172 616d 2055  s...    :param U
+0002b1b0: 6e69 6f6e 5b73 7472 2c20 6f73 2e50 6174  nion[str, os.Pat
+0002b1c0: 684c 696b 655d 2076 6964 656f 5f70 6174  hLike] video_pat
+0002b1d0: 683a 2054 6865 2070 6174 6820 746f 2074  h: The path to t
+0002b1e0: 6865 2076 6964 656f 2074 6f20 7265 6d6f  he video to remo
+0002b1f0: 7665 2074 6865 2062 6163 6b67 726f 756e  ve the backgroun
+0002b200: 6420 6672 6f6d 2e0a 2020 2020 3a70 6172  d from..    :par
+0002b210: 616d 204f 7074 696f 6e61 6c5b 556e 696f  am Optional[Unio
+0002b220: 6e5b 7374 722c 206f 732e 5061 7468 4c69  n[str, os.PathLi
+0002b230: 6b65 5d5d 2062 675f 7669 6465 6f5f 7061  ke]] bg_video_pa
+0002b240: 7468 3a20 5061 7468 2074 6f20 7468 6520  th: Path to the 
+0002b250: 7669 6465 6f20 7768 6963 6820 636f 6e74  video which cont
+0002b260: 6169 6e73 2061 2073 6567 6d65 6e74 2077  ains a segment w
+0002b270: 6974 6820 7468 6520 6261 636b 6772 6f75  ith the backgrou
+0002b280: 6e64 206f 6e6c 792e 2049 6620 4e6f 6e65  nd only. If None
+0002b290: 2c20 7468 656e 2060 6076 6964 656f 5f70  , then ``video_p
+0002b2a0: 6174 6860 6020 7769 6c6c 2062 6520 7573  ath`` will be us
+0002b2b0: 6564 2e0a 2020 2020 3a70 6172 616d 204f  ed..    :param O
+0002b2c0: 7074 696f 6e61 6c5b 696e 745d 2062 675f  ptional[int] bg_
+0002b2d0: 7374 6172 745f 6672 6d3a 2054 6865 2066  start_frm: The f
+0002b2e0: 6972 7374 2066 7261 6d65 2069 6e20 7468  irst frame in th
+0002b2f0: 6520 6261 636b 6772 6f75 6e64 2076 6964  e background vid
+0002b300: 656f 2074 6f20 7573 6520 7768 656e 2063  eo to use when c
+0002b310: 7265 6174 696e 6720 6120 7265 7072 6573  reating a repres
+0002b320: 656e 7461 7469 7665 2062 6163 6b67 726f  entative backgro
+0002b330: 756e 6420 696d 6167 652e 2044 6566 6175  und image. Defau
+0002b340: 6c74 3a20 4e6f 6e65 2e0a 2020 2020 3a70  lt: None..    :p
+0002b350: 6172 616d 204f 7074 696f 6e61 6c5b 696e  aram Optional[in
+0002b360: 745d 2062 675f 656e 645f 6672 6d3a 2054  t] bg_end_frm: T
+0002b370: 6865 206c 6173 7420 6672 616d 6520 696e  he last frame in
+0002b380: 2074 6865 2062 6163 6b67 726f 756e 6420   the background 
+0002b390: 7669 6465 6f20 746f 2075 7365 2077 6865  video to use whe
+0002b3a0: 6e20 6372 6561 7469 6e67 2061 2072 6570  n creating a rep
+0002b3b0: 7265 7365 6e74 6174 6976 6520 6261 636b  resentative back
+0002b3c0: 6772 6f75 6e64 2069 6d61 6765 2e20 4465  ground image. De
+0002b3d0: 6661 756c 743a 204e 6f6e 652e 0a20 2020  fault: None..   
+0002b3e0: 203a 7061 7261 6d20 4f70 7469 6f6e 616c   :param Optional
+0002b3f0: 5b73 7472 5d20 6267 5f73 7461 7274 5f74  [str] bg_start_t
+0002b400: 696d 653a 2054 6865 2073 7461 7274 2074  ime: The start t
+0002b410: 696d 6573 7461 6d70 2069 6e20 6048 483a  imestamp in `HH:
+0002b420: 4d4d 3a53 5360 2066 6f72 6d61 7420 696e  MM:SS` format in
+0002b430: 2074 6865 2062 6163 6b67 726f 756e 6420   the background 
+0002b440: 7669 6465 6f20 746f 2075 7365 2074 6f20  video to use to 
+0002b450: 6372 6561 7465 2061 2072 6570 7265 7365  create a represe
+0002b460: 6e74 6174 6976 6520 6261 636b 6772 6f75  ntative backgrou
+0002b470: 6e64 2069 6d61 6765 2e20 4465 6661 756c  nd image. Defaul
+0002b480: 743a 204e 6f6e 652e 0a20 2020 203a 7061  t: None..    :pa
+0002b490: 7261 6d20 4f70 7469 6f6e 616c 5b73 7472  ram Optional[str
+0002b4a0: 5d20 6267 5f65 6e64 5f74 696d 653a 2054  ] bg_end_time: T
+0002b4b0: 6865 2065 6e64 2074 696d 6573 7461 6d70  he end timestamp
+0002b4c0: 2069 6e20 6048 483a 4d4d 3a53 5360 2066   in `HH:MM:SS` f
+0002b4d0: 6f72 6d61 7420 696e 2074 6865 2062 6163  ormat in the bac
+0002b4e0: 6b67 726f 756e 6420 7669 6465 6f20 746f  kground video to
+0002b4f0: 2075 7365 2074 6f20 6372 6561 7465 2061   use to create a
+0002b500: 2072 6570 7265 7365 6e74 6174 6976 6520   representative 
+0002b510: 6261 636b 6772 6f75 6e64 2069 6d61 6765  background image
+0002b520: 2e20 4465 6661 756c 743a 204e 6f6e 652e  . Default: None.
+0002b530: 0a20 2020 203a 7061 7261 6d20 4f70 7469  .    :param Opti
+0002b540: 6f6e 616c 5b54 7570 6c65 5b69 6e74 2c20  onal[Tuple[int, 
+0002b550: 696e 742c 2069 6e74 5d5d 2062 675f 636f  int, int]] bg_co
+0002b560: 6c6f 723a 2054 6865 2052 4742 2063 6f6c  lor: The RGB col
+0002b570: 6f72 206f 6620 7468 6520 6d6f 7669 6e67  or of the moving
+0002b580: 206f 626a 6563 7473 2069 6e20 7468 6520   objects in the 
+0002b590: 6f75 7470 7574 2076 6964 656f 2e20 4465  output video. De
+0002b5a0: 6661 756c 7473 2074 6f20 4e6f 6e65 2c20  faults to None, 
+0002b5b0: 7768 6963 6820 7265 7072 6573 656e 7473  which represents
+0002b5c0: 2074 6865 206f 7269 6769 6e61 6c20 636f   the original co
+0002b5d0: 6c6f 7273 206f 6620 7468 6520 6d6f 7669  lors of the movi
+0002b5e0: 6e67 206f 626a 6563 7473 2e0a 2020 2020  ng objects..    
+0002b5f0: 3a70 6172 616d 204f 7074 696f 6e61 6c5b  :param Optional[
+0002b600: 5475 706c 655b 696e 742c 2069 6e74 2c20  Tuple[int, int, 
+0002b610: 696e 745d 5d20 6667 5f63 6f6c 6f72 3a20  int]] fg_color: 
+0002b620: 5468 6520 5247 4220 636f 6c6f 7220 6f66  The RGB color of
+0002b630: 2074 6865 2062 6163 6b67 726f 756e 6420   the background 
+0002b640: 6f75 7470 7574 2076 6964 656f 2e20 4465  output video. De
+0002b650: 6661 756c 7473 2074 6f20 626c 6163 6b20  faults to black 
+0002b660: 2830 2c20 302c 2030 292e 0a20 2020 203a  (0, 0, 0)..    :
+0002b670: 7061 7261 6d20 4f70 7469 6f6e 616c 5b55  param Optional[U
+0002b680: 6e69 6f6e 5b73 7472 2c20 6f73 2e50 6174  nion[str, os.Pat
+0002b690: 684c 696b 655d 5d20 7361 7665 5f70 6174  hLike]] save_pat
+0002b6a0: 683a 2054 6865 2070 6174 6368 2074 6f20  h: The patch to 
+0002b6b0: 7768 6572 6520 746f 2073 6176 6520 7468  where to save th
+0002b6c0: 6520 6f75 7470 7574 2076 6964 656f 2077  e output video w
+0002b6d0: 6865 7265 2074 6865 2062 6163 6b67 726f  here the backgro
+0002b6e0: 756e 6420 6973 2072 656d 6f76 6564 2e20  und is removed. 
+0002b6f0: 4966 204e 6f6e 652c 2073 6176 6573 2074  If None, saves t
+0002b700: 6865 206f 7574 7075 7420 7669 6465 6f20  he output video 
+0002b710: 696e 2074 6865 2073 616d 6520 6469 7265  in the same dire
+0002b720: 6374 6f72 7920 6173 2074 6865 2069 6e70  ctory as the inp
+0002b730: 7574 2076 6964 656f 2077 6974 6820 7468  ut video with th
+0002b740: 6520 6060 5f62 675f 7375 6274 7261 6374  e ``_bg_subtract
+0002b750: 6564 6060 2073 7566 6669 782e 2044 6566  ed`` suffix. Def
+0002b760: 6175 6c74 3a20 4e6f 6e65 2e0a 2020 2020  ault: None..    
+0002b770: 3a72 6574 7572 6e3a 204e 6f6e 652e 0a0a  :return: None...
+0002b780: 2020 2020 3a65 7861 6d70 6c65 3a0a 2020      :example:.  
+0002b790: 2020 3e3e 3e20 7669 6465 6f5f 6267 5f73    >>> video_bg_s
+0002b7a0: 7562 7472 6163 7469 6f6e 2876 6964 656f  ubtraction(video
+0002b7b0: 5f70 6174 683d 272f 5573 6572 732f 7369  _path='/Users/si
+0002b7c0: 6d6f 6e2f 446f 776e 6c6f 6164 732f 315f  mon/Downloads/1_
+0002b7d0: 4c48 5f63 726f 7070 6564 2e6d 7034 272c  LH_cropped.mp4',
+0002b7e0: 2062 675f 7374 6172 745f 7469 6d65 3d27   bg_start_time='
+0002b7f0: 3030 3a30 303a 3030 272c 2062 675f 656e  00:00:00', bg_en
+0002b800: 645f 7469 6d65 3d27 3030 3a30 303a 3130  d_time='00:00:10
+0002b810: 272c 2062 675f 636f 6c6f 723d 2830 2c20  ', bg_color=(0, 
+0002b820: 3130 362c 2031 3637 292c 2066 675f 636f  106, 167), fg_co
+0002b830: 6c6f 723d 2832 3534 2c20 3230 342c 2032  lor=(254, 204, 2
+0002b840: 2929 0a20 2020 2022 2222 0a0a 2020 2020  )).    """..    
+0002b850: 7469 6d65 7220 3d20 5369 6d62 6154 696d  timer = SimbaTim
+0002b860: 6572 2873 7461 7274 3d54 7275 6529 0a20  er(start=True). 
+0002b870: 2020 2063 6865 636b 5f66 696c 655f 6578     check_file_ex
+0002b880: 6973 745f 616e 645f 7265 6164 6162 6c65  ist_and_readable
+0002b890: 2866 696c 655f 7061 7468 3d76 6964 656f  (file_path=video
+0002b8a0: 5f70 6174 6829 0a20 2020 2069 6620 6267  _path).    if bg
+0002b8b0: 5f76 6964 656f 5f70 6174 6820 6973 204e  _video_path is N
+0002b8c0: 6f6e 653a 0a20 2020 2020 2020 2062 675f  one:.        bg_
+0002b8d0: 7669 6465 6f5f 7061 7468 203d 2064 6565  video_path = dee
+0002b8e0: 7063 6f70 7928 7669 6465 6f5f 7061 7468  pcopy(video_path
+0002b8f0: 290a 2020 2020 7669 6465 6f5f 6d65 7461  ).    video_meta
+0002b900: 5f64 6174 6120 3d20 6765 745f 7669 6465  _data = get_vide
+0002b910: 6f5f 6d65 7461 5f64 6174 6128 7669 6465  o_meta_data(vide
+0002b920: 6f5f 7061 7468 3d76 6964 656f 5f70 6174  o_path=video_pat
+0002b930: 6829 0a20 2020 2064 6972 2c20 7669 6465  h).    dir, vide
+0002b940: 6f5f 6e61 6d65 2c20 6578 7420 3d20 6765  o_name, ext = ge
+0002b950: 745f 666e 5f65 7874 2866 696c 6570 6174  t_fn_ext(filepat
+0002b960: 683d 7669 6465 6f5f 7061 7468 290a 2020  h=video_path).  
+0002b970: 2020 6966 2073 6176 655f 7061 7468 2069    if save_path i
+0002b980: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+0002b990: 7361 7665 5f70 6174 6820 3d20 6f73 2e70  save_path = os.p
+0002b9a0: 6174 682e 6a6f 696e 2864 6972 2c20 6627  ath.join(dir, f'
+0002b9b0: 7b76 6964 656f 5f6e 616d 657d 5f62 675f  {video_name}_bg_
+0002b9c0: 7375 6274 7261 6374 6564 7b65 7874 7d27  subtracted{ext}'
+0002b9d0: 290a 2020 2020 666f 7572 6363 203d 2063  ).    fourcc = c
+0002b9e0: 7632 2e56 6964 656f 5772 6974 6572 5f66  v2.VideoWriter_f
+0002b9f0: 6f75 7263 6328 2a46 6f72 6d61 7473 2e4d  ourcc(*Formats.M
+0002ba00: 5034 5f43 4f44 4543 2e76 616c 7565 290a  P4_CODEC.value).
+0002ba10: 2020 2020 7772 6974 6572 203d 2063 7632      writer = cv2
+0002ba20: 2e56 6964 656f 5772 6974 6572 2873 6176  .VideoWriter(sav
+0002ba30: 655f 7061 7468 2c20 666f 7572 6363 2c20  e_path, fourcc, 
 0002ba40: 7669 6465 6f5f 6d65 7461 5f64 6174 615b  video_meta_data[
-0002ba50: 2777 6964 7468 275d 2c20 7669 6465 6f5f  'width'], video_
-0002ba60: 6d65 7461 5f64 6174 615b 2768 6569 6768  meta_data['heigh
-0002ba70: 7427 5d29 290a 2020 2020 6267 5f66 726d  t'])).    bg_frm
-0002ba80: 203d 2063 7265 6174 655f 6176 6572 6167   = create_averag
-0002ba90: 655f 6672 6d28 7669 6465 6f5f 7061 7468  e_frm(video_path
-0002baa0: 3d62 675f 7669 6465 6f5f 7061 7468 2c20  =bg_video_path, 
-0002bab0: 7374 6172 745f 6672 6d3d 6267 5f73 7461  start_frm=bg_sta
-0002bac0: 7274 5f66 726d 2c20 656e 645f 6672 6d3d  rt_frm, end_frm=
-0002bad0: 6267 5f65 6e64 5f66 726d 2c0a 2020 2020  bg_end_frm,.    
-0002bae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002baf0: 2020 2020 2020 2020 2020 2020 7374 6172              star
-0002bb00: 745f 7469 6d65 3d62 675f 7374 6172 745f  t_time=bg_start_
-0002bb10: 7469 6d65 2c20 656e 645f 7469 6d65 3d62  time, end_time=b
-0002bb20: 675f 656e 645f 7469 6d65 290a 2020 2020  g_end_time).    
-0002bb30: 6267 5f66 726d 203d 2063 7632 2e72 6573  bg_frm = cv2.res
-0002bb40: 697a 6528 6267 5f66 726d 2c20 2876 6964  ize(bg_frm, (vid
-0002bb50: 656f 5f6d 6574 615f 6461 7461 5b27 7769  eo_meta_data['wi
-0002bb60: 6474 6827 5d2c 2076 6964 656f 5f6d 6574  dth'], video_met
-0002bb70: 615f 6461 7461 5b27 6865 6967 6874 275d  a_data['height']
-0002bb80: 2929 0a20 2020 2062 6720 3d20 6376 322e  )).    bg = cv2.
-0002bb90: 6376 7443 6f6c 6f72 286e 702e 6675 6c6c  cvtColor(np.full
-0002bba0: 5f6c 696b 6528 6267 5f66 726d 2c20 6267  _like(bg_frm, bg
-0002bbb0: 5f63 6f6c 6f72 292c 2063 7632 2e43 4f4c  _color), cv2.COL
-0002bbc0: 4f52 5f42 4752 3252 4742 290a 2020 2020  OR_BGR2RGB).    
-0002bbd0: 6361 7020 3d20 6376 322e 5669 6465 6f43  cap = cv2.VideoC
-0002bbe0: 6170 7475 7265 2876 6964 656f 5f70 6174  apture(video_pat
-0002bbf0: 6829 0a20 2020 2066 726d 5f63 6e74 203d  h).    frm_cnt =
-0002bc00: 2030 0a20 2020 2077 6869 6c65 2054 7275   0.    while Tru
-0002bc10: 653a 0a20 2020 2020 2020 2072 6574 2c20  e:.        ret, 
-0002bc20: 6672 6d20 3d20 6361 702e 7265 6164 2829  frm = cap.read()
-0002bc30: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-0002bc40: 7265 743a 0a20 2020 2020 2020 2020 2020  ret:.           
-0002bc50: 2062 7265 616b 0a20 2020 2020 2020 2064   break.        d
-0002bc60: 6966 6620 3d20 6376 322e 6162 7364 6966  iff = cv2.absdif
-0002bc70: 6628 6672 6d2c 2062 675f 6672 6d29 0a20  f(frm, bg_frm). 
-0002bc80: 2020 2020 2020 2067 7261 795f 6469 6666         gray_diff
-0002bc90: 203d 2063 7632 2e63 7674 436f 6c6f 7228   = cv2.cvtColor(
-0002bca0: 6469 6666 2c20 6376 322e 434f 4c4f 525f  diff, cv2.COLOR_
-0002bcb0: 4247 5232 4752 4159 290a 2020 2020 2020  BGR2GRAY).      
-0002bcc0: 2020 5f2c 206d 6173 6b20 3d20 6376 322e    _, mask = cv2.
-0002bcd0: 7468 7265 7368 6f6c 6428 6772 6179 5f64  threshold(gray_d
-0002bce0: 6966 662c 2035 302c 2032 3535 2c20 6376  iff, 50, 255, cv
-0002bcf0: 322e 5448 5245 5348 5f42 494e 4152 5929  2.THRESH_BINARY)
-0002bd00: 0a20 2020 2020 2020 2069 6620 6667 5f63  .        if fg_c
-0002bd10: 6f6c 6f72 2069 7320 4e6f 6e65 3a0a 2020  olor is None:.  
-0002bd20: 2020 2020 2020 2020 2020 6667 203d 2063            fg = c
-0002bd30: 7632 2e62 6974 7769 7365 5f61 6e64 2866  v2.bitwise_and(f
-0002bd40: 726d 2c20 6672 6d2c 206d 6173 6b3d 6d61  rm, frm, mask=ma
-0002bd50: 736b 290a 2020 2020 2020 2020 2020 2020  sk).            
-0002bd60: 7265 7375 6c74 203d 2063 7632 2e61 6464  result = cv2.add
-0002bd70: 2862 672c 2066 6729 0a20 2020 2020 2020  (bg, fg).       
-0002bd80: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0002bd90: 2020 206d 6173 6b5f 696e 7620 3d20 6376     mask_inv = cv
-0002bda0: 322e 6269 7477 6973 655f 6e6f 7428 6d61  2.bitwise_not(ma
-0002bdb0: 736b 290a 2020 2020 2020 2020 2020 2020  sk).            
-0002bdc0: 6667 5f63 6c72 203d 2063 7632 2e63 7674  fg_clr = cv2.cvt
-0002bdd0: 436f 6c6f 7228 6e70 2e66 756c 6c5f 6c69  Color(np.full_li
-0002bde0: 6b65 2866 726d 2c20 6667 5f63 6f6c 6f72  ke(frm, fg_color
-0002bdf0: 292c 2063 7632 2e43 4f4c 4f52 5f42 4752  ), cv2.COLOR_BGR
-0002be00: 3252 4742 290a 2020 2020 2020 2020 2020  2RGB).          
-0002be10: 2020 6667 5f63 6c72 203d 2063 7632 2e62    fg_clr = cv2.b
-0002be20: 6974 7769 7365 5f61 6e64 2866 675f 636c  itwise_and(fg_cl
-0002be30: 722c 2066 675f 636c 722c 206d 6173 6b3d  r, fg_clr, mask=
-0002be40: 6d61 736b 290a 2020 2020 2020 2020 2020  mask).          
-0002be50: 2020 7265 7375 6c74 203d 2063 7632 2e62    result = cv2.b
-0002be60: 6974 7769 7365 5f61 6e64 2862 672c 2062  itwise_and(bg, b
-0002be70: 672c 206d 6173 6b3d 6d61 736b 5f69 6e76  g, mask=mask_inv
-0002be80: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
-0002be90: 7375 6c74 203d 2063 7632 2e61 6464 2872  sult = cv2.add(r
-0002bea0: 6573 756c 742c 2066 675f 636c 7229 0a20  esult, fg_clr). 
-0002beb0: 2020 2020 2020 2077 7269 7465 722e 7772         writer.wr
-0002bec0: 6974 6528 7265 7375 6c74 290a 2020 2020  ite(result).    
-0002bed0: 2020 2020 6672 6d5f 636e 7420 2b3d 2031      frm_cnt += 1
-0002bee0: 0a20 2020 2020 2020 2070 7269 6e74 2866  .        print(f
-0002bef0: 2742 6163 6b67 726f 756e 6420 7375 6274  'Background subt
-0002bf00: 7261 6374 696f 6e20 6672 616d 6520 7b66  raction frame {f
-0002bf10: 726d 5f63 6e74 7d2f 7b76 6964 656f 5f6d  rm_cnt}/{video_m
-0002bf20: 6574 615f 6461 7461 5b22 6672 616d 655f  eta_data["frame_
-0002bf30: 636f 756e 7422 5d7d 2028 5669 6465 6f3a  count"]} (Video:
-0002bf40: 207b 7669 6465 6f5f 6e61 6d65 7d29 2729   {video_name})')
-0002bf50: 0a0a 2020 2020 7772 6974 6572 2e72 656c  ..    writer.rel
-0002bf60: 6561 7365 2829 0a20 2020 2063 6170 2e72  ease().    cap.r
-0002bf70: 656c 6561 7365 2829 0a20 2020 2074 696d  elease().    tim
-0002bf80: 6572 2e73 746f 705f 7469 6d65 7228 290a  er.stop_timer().
-0002bf90: 2020 2020 7374 646f 7574 5f73 7563 6365      stdout_succe
-0002bfa0: 7373 286d 7367 3d66 2742 6163 6b67 726f  ss(msg=f'Backgro
-0002bfb0: 756e 6420 7375 6274 7261 6374 6564 2066  und subtracted f
-0002bfc0: 726f 6d20 7b76 6964 656f 5f6e 616d 657d  rom {video_name}
-0002bfd0: 2061 6e64 2073 6176 6564 2061 7420 7b73   and saved at {s
-0002bfe0: 6176 655f 7061 7468 7d27 2c20 656c 6170  ave_path}', elap
-0002bff0: 7365 645f 7469 6d65 3d74 696d 6572 2e65  sed_time=timer.e
-0002c000: 6c61 7073 6564 5f74 696d 6529 0a0a 6465  lapsed_time)..de
-0002c010: 6620 5f62 675f 7265 6d6f 7665 725f 6d70  f _bg_remover_mp
-0002c020: 2866 726d 5f72 616e 6765 3a20 5475 706c  (frm_range: Tupl
-0002c030: 655b 696e 742c 206e 702e 6e64 6172 7261  e[int, np.ndarra
-0002c040: 795d 2c0a 2020 2020 2020 2020 2020 2020  y],.            
-0002c050: 2020 2020 2020 2076 6964 656f 5f70 6174         video_pat
-0002c060: 683a 2055 6e69 6f6e 5b73 7472 2c20 6f73  h: Union[str, os
-0002c070: 2e50 6174 684c 696b 655d 2c0a 2020 2020  .PathLike],.    
-0002c080: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-0002c090: 675f 6672 6d3a 206e 702e 6e64 6172 7261  g_frm: np.ndarra
-0002c0a0: 792c 0a20 2020 2020 2020 2020 2020 2020  y,.             
-0002c0b0: 2020 2020 2020 6267 5f63 6c72 3a20 5475        bg_clr: Tu
-0002c0c0: 706c 655b 696e 742c 2069 6e74 2c20 696e  ple[int, int, in
-0002c0d0: 745d 2c0a 2020 2020 2020 2020 2020 2020  t],.            
-0002c0e0: 2020 2020 2020 2066 675f 636c 723a 2054         fg_clr: T
-0002c0f0: 7570 6c65 5b69 6e74 2c20 696e 742c 2069  uple[int, int, i
-0002c100: 6e74 5d2c 0a20 2020 2020 2020 2020 2020  nt],.           
-0002c110: 2020 2020 2020 2020 7669 6465 6f5f 6d65          video_me
-0002c120: 7461 5f64 6174 613a 2044 6963 745b 7374  ta_data: Dict[st
-0002c130: 722c 2041 6e79 5d2c 0a20 2020 2020 2020  r, Any],.       
-0002c140: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
-0002c150: 5f64 6972 3a20 556e 696f 6e5b 7374 722c  _dir: Union[str,
-0002c160: 206f 732e 5061 7468 4c69 6b65 5d29 3a0a   os.PathLike]):.
-0002c170: 0a20 2020 2062 6174 6368 2c20 6672 6d5f  .    batch, frm_
-0002c180: 7261 6e67 6520 3d20 6672 6d5f 7261 6e67  range = frm_rang
-0002c190: 655b 305d 2c20 6672 6d5f 7261 6e67 655b  e[0], frm_range[
-0002c1a0: 315d 0a20 2020 2073 7461 7274 5f66 726d  1].    start_frm
-0002c1b0: 2c20 6375 7272 656e 745f 6672 6d2c 2065  , current_frm, e
-0002c1c0: 6e64 5f66 726d 203d 2066 726d 5f72 616e  nd_frm = frm_ran
-0002c1d0: 6765 5b30 5d2c 2066 726d 5f72 616e 6765  ge[0], frm_range
-0002c1e0: 5b30 5d2c 2066 726d 5f72 616e 6765 5b2d  [0], frm_range[-
-0002c1f0: 315d 0a20 2020 2063 6170 203d 2063 7632  1].    cap = cv2
-0002c200: 2e56 6964 656f 4361 7074 7572 6528 7669  .VideoCapture(vi
-0002c210: 6465 6f5f 7061 7468 290a 2020 2020 666f  deo_path).    fo
-0002c220: 7572 6363 203d 2063 7632 2e56 6964 656f  urcc = cv2.Video
-0002c230: 5772 6974 6572 5f66 6f75 7263 6328 2a46  Writer_fourcc(*F
-0002c240: 6f72 6d61 7473 2e4d 5034 5f43 4f44 4543  ormats.MP4_CODEC
-0002c250: 2e76 616c 7565 290a 2020 2020 7361 7665  .value).    save
-0002c260: 5f70 6174 6820 3d20 6f73 2e70 6174 682e  _path = os.path.
-0002c270: 6a6f 696e 2874 656d 705f 6469 722c 2066  join(temp_dir, f
-0002c280: 227b 6261 7463 687d 2e6d 7034 2229 0a20  "{batch}.mp4"). 
-0002c290: 2020 2063 6170 2e73 6574 2831 2c20 7374     cap.set(1, st
-0002c2a0: 6172 745f 6672 6d29 0a20 2020 2077 7269  art_frm).    wri
-0002c2b0: 7465 7220 3d20 6376 322e 5669 6465 6f57  ter = cv2.VideoW
-0002c2c0: 7269 7465 7228 7361 7665 5f70 6174 682c  riter(save_path,
-0002c2d0: 2066 6f75 7263 632c 2076 6964 656f 5f6d   fourcc, video_m
-0002c2e0: 6574 615f 6461 7461 5b27 6670 7327 5d2c  eta_data['fps'],
-0002c2f0: 2028 7669 6465 6f5f 6d65 7461 5f64 6174   (video_meta_dat
-0002c300: 615b 2777 6964 7468 275d 2c20 7669 6465  a['width'], vide
-0002c310: 6f5f 6d65 7461 5f64 6174 615b 2768 6569  o_meta_data['hei
-0002c320: 6768 7427 5d29 290a 2020 2020 6267 203d  ght'])).    bg =
-0002c330: 206e 702e 6675 6c6c 5f6c 696b 6528 6267   np.full_like(bg
-0002c340: 5f66 726d 2c20 6267 5f63 6c72 290a 2020  _frm, bg_clr).  
-0002c350: 2020 6267 203d 2062 675b 3a2c 203a 2c20    bg = bg[:, :, 
-0002c360: 3a3a 2d31 5d0a 2020 2020 6469 722c 2076  ::-1].    dir, v
-0002c370: 6964 656f 5f6e 616d 652c 2065 7874 203d  ideo_name, ext =
-0002c380: 2067 6574 5f66 6e5f 6578 7428 6669 6c65   get_fn_ext(file
-0002c390: 7061 7468 3d76 6964 656f 5f70 6174 6829  path=video_path)
-0002c3a0: 0a20 2020 2077 6869 6c65 2063 7572 7265  .    while curre
-0002c3b0: 6e74 5f66 726d 203c 3d20 656e 645f 6672  nt_frm <= end_fr
-0002c3c0: 6d3a 0a20 2020 2020 2020 2072 6574 2c20  m:.        ret, 
-0002c3d0: 6672 6d20 3d20 6361 702e 7265 6164 2829  frm = cap.read()
-0002c3e0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-0002c3f0: 7265 743a 0a20 2020 2020 2020 2020 2020  ret:.           
-0002c400: 2062 7265 616b 0a20 2020 2020 2020 2064   break.        d
-0002c410: 6966 6620 3d20 6376 322e 6162 7364 6966  iff = cv2.absdif
-0002c420: 6628 6672 6d2c 2062 675f 6672 6d29 0a20  f(frm, bg_frm). 
-0002c430: 2020 2020 2020 2062 2c20 672c 2072 203d         b, g, r =
-0002c440: 2064 6966 665b 3a2c 203a 2c20 305d 2c20   diff[:, :, 0], 
-0002c450: 6469 6666 5b3a 2c20 3a2c 2031 5d2c 2064  diff[:, :, 1], d
-0002c460: 6966 665b 3a2c 203a 2c20 325d 0a20 2020  iff[:, :, 2].   
-0002c470: 2020 2020 2067 7261 795f 6469 6666 203d       gray_diff =
-0002c480: 2030 2e32 3938 3920 2a20 7220 2b20 302e   0.2989 * r + 0.
-0002c490: 3538 3730 202a 2067 202b 2030 2e31 3134  5870 * g + 0.114
-0002c4a0: 3020 2a20 620a 2020 2020 2020 2020 6772  0 * b.        gr
-0002c4b0: 6179 5f64 6966 6620 3d20 6772 6179 5f64  ay_diff = gray_d
-0002c4c0: 6966 662e 6173 7479 7065 286e 702e 7569  iff.astype(np.ui
-0002c4d0: 6e74 3829 2020 2320 456e 7375 7265 2074  nt8)  # Ensure t
-0002c4e0: 6865 2074 7970 6520 6973 2075 696e 7438  he type is uint8
-0002c4f0: 0a20 2020 2020 2020 206d 6173 6b20 3d20  .        mask = 
-0002c500: 6e70 2e77 6865 7265 2867 7261 795f 6469  np.where(gray_di
-0002c510: 6666 203e 2035 302c 2032 3535 2c20 3029  ff > 50, 255, 0)
-0002c520: 2e61 7374 7970 6528 6e70 2e75 696e 7438  .astype(np.uint8
-0002c530: 290a 2020 2020 2020 2020 6966 2066 675f  ).        if fg_
-0002c540: 636c 7220 6973 204e 6f6e 653a 0a20 2020  clr is None:.   
-0002c550: 2020 2020 2020 2020 2066 6720 3d20 6376           fg = cv
-0002c560: 322e 6269 7477 6973 655f 616e 6428 6672  2.bitwise_and(fr
-0002c570: 6d2c 2066 726d 2c20 6d61 736b 3d6d 6173  m, frm, mask=mas
-0002c580: 6b29 0a20 2020 2020 2020 2020 2020 2072  k).            r
-0002c590: 6573 756c 7420 3d20 6376 322e 6164 6428  esult = cv2.add(
-0002c5a0: 6267 2c20 6667 290a 2020 2020 2020 2020  bg, fg).        
-0002c5b0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0002c5c0: 2020 6d61 736b 5f69 6e76 203d 2063 7632    mask_inv = cv2
-0002c5d0: 2e62 6974 7769 7365 5f6e 6f74 286d 6173  .bitwise_not(mas
-0002c5e0: 6b29 0a20 2020 2020 2020 2020 2020 2066  k).            f
-0002c5f0: 675f 636c 725f 696d 6720 3d20 6e70 2e66  g_clr_img = np.f
-0002c600: 756c 6c5f 6c69 6b65 2866 726d 2c20 6667  ull_like(frm, fg
-0002c610: 5f63 6c72 290a 2020 2020 2020 2020 2020  _clr).          
-0002c620: 2020 6667 5f63 6c72 5f69 6d67 203d 2066    fg_clr_img = f
-0002c630: 675f 636c 725f 696d 675b 3a2c 203a 2c20  g_clr_img[:, :, 
-0002c640: 3a3a 2d31 5d0a 2020 2020 2020 2020 2020  ::-1].          
-0002c650: 2020 6667 5f63 6c72 5f69 6d67 203d 2063    fg_clr_img = c
-0002c660: 7632 2e62 6974 7769 7365 5f61 6e64 2866  v2.bitwise_and(f
-0002c670: 675f 636c 725f 696d 672c 2066 675f 636c  g_clr_img, fg_cl
-0002c680: 725f 696d 672c 206d 6173 6b3d 6d61 736b  r_img, mask=mask
-0002c690: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
-0002c6a0: 7375 6c74 203d 2063 7632 2e62 6974 7769  sult = cv2.bitwi
-0002c6b0: 7365 5f61 6e64 2862 672c 2062 672c 206d  se_and(bg, bg, m
-0002c6c0: 6173 6b3d 6d61 736b 5f69 6e76 290a 2020  ask=mask_inv).  
-0002c6d0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-0002c6e0: 203d 2063 7632 2e61 6464 2872 6573 756c   = cv2.add(resul
-0002c6f0: 742c 2066 675f 636c 725f 696d 6729 0a20  t, fg_clr_img). 
-0002c700: 2020 2020 2020 2077 7269 7465 722e 7772         writer.wr
-0002c710: 6974 6528 7265 7375 6c74 290a 2020 2020  ite(result).    
-0002c720: 2020 2020 6375 7272 656e 745f 6672 6d20      current_frm 
-0002c730: 2b3d 2031 0a20 2020 2020 2020 2070 7269  += 1.        pri
-0002c740: 6e74 2866 2742 6163 6b67 726f 756e 6420  nt(f'Background 
-0002c750: 7375 6274 7261 6374 696f 6e20 6672 616d  subtraction fram
-0002c760: 6520 7b63 7572 7265 6e74 5f66 726d 7d2f  e {current_frm}/
-0002c770: 7b76 6964 656f 5f6d 6574 615f 6461 7461  {video_meta_data
-0002c780: 5b22 6672 616d 655f 636f 756e 7422 5d7d  ["frame_count"]}
-0002c790: 2028 5669 6465 6f3a 207b 7669 6465 6f5f   (Video: {video_
-0002c7a0: 6e61 6d65 7d29 2729 0a20 2020 2077 7269  name})').    wri
-0002c7b0: 7465 722e 7265 6c65 6173 6528 290a 2020  ter.release().  
-0002c7c0: 2020 6361 702e 7265 6c65 6173 6528 290a    cap.release().
-0002c7d0: 2020 2020 7265 7475 726e 2062 6174 6368      return batch
-0002c7e0: 0a0a 6465 6620 7669 6465 6f5f 6267 5f73  ..def video_bg_s
-0002c7f0: 7562 7374 7261 6374 696f 6e5f 6d70 2876  ubstraction_mp(v
-0002c800: 6964 656f 5f70 6174 683a 2055 6e69 6f6e  ideo_path: Union
-0002c810: 5b73 7472 2c20 6f73 2e50 6174 684c 696b  [str, os.PathLik
-0002c820: 655d 2c0a 2020 2020 2020 2020 2020 2020  e],.            
-0002c830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c840: 2062 675f 7669 6465 6f5f 7061 7468 3a20   bg_video_path: 
-0002c850: 4f70 7469 6f6e 616c 5b55 6e69 6f6e 5b73  Optional[Union[s
-0002c860: 7472 2c20 6f73 2e50 6174 684c 696b 655d  tr, os.PathLike]
-0002c870: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-0002c880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c890: 2020 2020 2020 2062 675f 7374 6172 745f         bg_start_
-0002c8a0: 6672 6d3a 204f 7074 696f 6e61 6c5b 696e  frm: Optional[in
-0002c8b0: 745d 203d 204e 6f6e 652c 0a20 2020 2020  t] = None,.     
-0002c8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c8d0: 2020 2020 2020 2020 6267 5f65 6e64 5f66          bg_end_f
-0002c8e0: 726d 3a20 4f70 7469 6f6e 616c 5b69 6e74  rm: Optional[int
-0002c8f0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-0002c900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c910: 2020 2020 2020 2062 675f 7374 6172 745f         bg_start_
-0002c920: 7469 6d65 3a20 4f70 7469 6f6e 616c 5b73  time: Optional[s
-0002c930: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
-0002c940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c950: 2020 2020 2020 2020 2062 675f 656e 645f           bg_end_
-0002c960: 7469 6d65 3a20 4f70 7469 6f6e 616c 5b73  time: Optional[s
-0002c970: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
-0002c980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c990: 2020 2020 2020 2020 2062 675f 636f 6c6f           bg_colo
-0002c9a0: 723a 204f 7074 696f 6e61 6c5b 5475 706c  r: Optional[Tupl
-0002c9b0: 655b 696e 742c 2069 6e74 2c20 696e 745d  e[int, int, int]
-0002c9c0: 5d20 3d20 2830 2c20 302c 2030 292c 0a20  ] = (0, 0, 0),. 
-0002c9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c9e0: 2020 2020 2020 2020 2020 2020 6667 5f63              fg_c
-0002c9f0: 6f6c 6f72 3a20 4f70 7469 6f6e 616c 5b54  olor: Optional[T
-0002ca00: 7570 6c65 5b69 6e74 2c20 696e 742c 2069  uple[int, int, i
-0002ca10: 6e74 5d5d 203d 204e 6f6e 652c 0a20 2020  nt]] = None,.   
-0002ca20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002ca30: 2020 2020 2020 2020 2020 7361 7665 5f70            save_p
-0002ca40: 6174 683a 204f 7074 696f 6e61 6c5b 556e  ath: Optional[Un
-0002ca50: 696f 6e5b 7374 722c 206f 732e 5061 7468  ion[str, os.Path
-0002ca60: 4c69 6b65 5d5d 203d 204e 6f6e 652c 0a20  Like]] = None,. 
-0002ca70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002ca80: 2020 2020 2020 2020 2020 2020 636f 7265              core
-0002ca90: 5f63 6e74 3a20 4f70 7469 6f6e 616c 5b69  _cnt: Optional[i
-0002caa0: 6e74 5d20 3d20 2d31 2920 2d3e 204e 6f6e  nt] = -1) -> Non
-0002cab0: 653a 0a0a 2020 2020 2222 220a 2020 2020  e:..    """.    
-0002cac0: 5375 6274 7261 6374 2074 6865 2062 6163  Subtract the bac
-0002cad0: 6b67 726f 756e 6420 6672 6f6d 2061 2076  kground from a v
-0002cae0: 6964 656f 2075 7369 6e67 206d 756c 7469  ideo using multi
-0002caf0: 7072 6f63 6573 7369 6e67 2e0a 0a20 2020  processing...   
-0002cb00: 202e 2e20 7669 6465 6f3a 3a20 5f73 7461   .. video:: _sta
-0002cb10: 7469 632f 696d 672f 7669 6465 6f5f 6267  tic/img/video_bg
-0002cb20: 5f73 7562 7374 7261 6374 696f 6e5f 6d70  _substraction_mp
-0002cb30: 2e77 6562 6d0a 2020 2020 2020 203a 7769  .webm.       :wi
-0002cb40: 6474 683a 2039 3030 0a20 2020 2020 2020  dth: 900.       
-0002cb50: 3a61 7574 6f70 6c61 793a 0a20 2020 2020  :autoplay:.     
-0002cb60: 2020 3a6c 6f6f 703a 0a0a 2020 2020 2e2e    :loop:..    ..
-0002cb70: 206e 6f74 653a 3a0a 2020 2020 2020 2020   note::.        
-0002cb80: 466f 7220 7369 6e67 6c65 2063 6f72 6520  For single core 
-0002cb90: 616c 7465 726e 6174 6976 652c 2073 6565  alternative, see
-0002cba0: 2060 6073 696d 6261 2e76 6964 656f 5f70   ``simba.video_p
-0002cbb0: 726f 6365 7373 6f72 732e 7669 6465 6f5f  rocessors.video_
-0002cbc0: 7072 6f63 6573 7369 6e67 2e76 6964 656f  processing.video
-0002cbd0: 5f62 675f 7375 6274 7261 6374 696f 6e60  _bg_subtraction`
-0002cbe0: 600a 0a20 2020 2020 2020 4966 2020 6060  `..       If  ``
-0002cbf0: 6267 5f76 6964 656f 5f70 6174 6860 6020  bg_video_path`` 
-0002cc00: 6973 2070 6173 7365 642c 2074 6861 7420  is passed, that 
-0002cc10: 7669 6465 6f20 7769 6c6c 2062 6520 7573  video will be us
-0002cc20: 6564 2074 6f20 7061 7273 6520 7468 6520  ed to parse the 
-0002cc30: 6261 636b 6772 6f75 6e64 2e20 4966 204e  background. If N
-0002cc40: 6f6e 652c 2060 6076 6964 656f 5f70 6174  one, ``video_pat
-0002cc50: 6860 6020 7769 6c6c 2062 6520 7573 6520  h`` will be use 
-0002cc60: 6474 6f20 7061 7273 6520 6261 636b 6772  dto parse backgr
-0002cc70: 6f75 6e64 2e0a 2020 2020 2020 2045 6974  ound..       Eit
-0002cc80: 6865 7220 7061 7373 2060 6073 7461 7274  her pass ``start
-0002cc90: 5f66 726d 6060 2061 6e64 2060 6065 6e64  _frm`` and ``end
-0002cca0: 5f66 726d 6060 204f 5220 6060 7374 6172  _frm`` OR ``star
-0002ccb0: 745f 7469 6d65 6060 2061 6e64 2060 6065  t_time`` and ``e
-0002ccc0: 6e64 5f74 696d 6560 6020 4f52 2070 6173  nd_time`` OR pas
-0002ccd0: 7320 616c 6c20 666f 7572 2061 7267 756d  s all four argum
-0002cce0: 656e 7473 2061 7320 4e6f 6e65 2e0a 2020  ents as None..  
-0002ccf0: 2020 2020 2054 686f 7365 2074 776f 2061       Those two a
-0002cd00: 7267 756d 656e 7473 2077 696c 6c20 6265  rguments will be
-0002cd10: 2075 7365 6420 746f 2073 6c69 6365 2074   used to slice t
-0002cd20: 6865 2062 6163 6b67 726f 756e 6420 7669  he background vi
-0002cd30: 6465 6f2c 2061 6e64 2074 6865 2073 6c69  deo, and the sli
-0002cd40: 6365 6420 7061 7274 2069 7320 7573 6564  ced part is used
-0002cd50: 2074 6f20 7061 7273 6520 7468 6520 6261   to parse the ba
-0002cd60: 636b 6772 6f75 6e64 2e0a 0a20 2020 2020  ckground...     
-0002cd70: 2020 466f 7220 6578 616d 706c 652c 2069    For example, i
-0002cd80: 6e20 7468 6520 7363 656e 6172 696f 2077  n the scenario w
-0002cd90: 6865 7265 2074 6865 7265 2069 7320 2a2a  here there is **
-0002cda0: 6e6f 2a2a 2061 6e69 6d61 6c20 696e 2074  no** animal in t
-0002cdb0: 6865 2060 6076 6964 656f 5f70 6174 6860  he ``video_path`
-0002cdc0: 6020 7669 6465 6f20 666f 7220 7468 6520  ` video for the 
-0002cdd0: 6669 7273 7420 3230 732c 2074 6865 6e20  first 20s, then 
-0002cde0: 7468 6520 6669 7273 7420 3230 7320 6361  the first 20s ca
-0002cdf0: 6e20 6265 2075 7365 6420 746f 2070 6172  n be used to par
-0002ce00: 7365 2074 6865 2062 6163 6b67 726f 756e  se the backgroun
-0002ce10: 642e 0a20 2020 2020 2020 496e 2074 6869  d..       In thi
-0002ce20: 7320 7363 656e 6172 696f 2c20 6060 6267  s scenario, ``bg
-0002ce30: 5f76 6964 656f 5f70 6174 6860 6020 6361  _video_path`` ca
-0002ce40: 6e20 6265 2070 6173 7365 6420 6173 2060  n be passed as `
-0002ce50: 604e 6f6e 6560 6020 616e 6420 6267 5f73  `None`` and bg_s
-0002ce60: 7461 7274 5f74 696d 6520 616e 6420 6267  tart_time and bg
-0002ce70: 5f65 6e64 5f74 696d 6520 6361 6e20 6265  _end_time can be
-0002ce80: 2060 6030 303a 3030 3a30 3060 6020 616e   ``00:00:00`` an
-0002ce90: 6420 6060 3030 3a30 303a 3230 6060 2c20  d ``00:00:20``, 
-0002cea0: 7265 7065 6374 6976 656c 792e 0a0a 2020  repectively...  
-0002ceb0: 2020 2020 2049 6e20 7468 6520 7363 656e       In the scen
-0002cec0: 6172 696f 2077 6865 7265 2074 6865 7265  ario where there
-0002ced0: 202a 2a69 732a 2a20 616e 696d 616c 2873   **is** animal(s
-0002cee0: 2920 696e 2074 6865 2065 6e74 6972 6520  ) in the entire 
-0002cef0: 6060 7669 6465 6f5f 7061 7468 6060 2076  ``video_path`` v
-0002cf00: 6964 656f 2c20 7061 7373 2060 6062 675f  ideo, pass ``bg_
-0002cf10: 7669 6465 6f5f 7061 7468 6060 2061 7320  video_path`` as 
-0002cf20: 6120 7061 7468 2074 6f20 6120 7669 6465  a path to a vide
-0002cf30: 6f20 7265 636f 7264 696e 6720 7468 6520  o recording the 
-0002cf40: 6172 656e 6120 7769 7468 6f75 7420 7468  arena without th
-0002cf50: 6520 616e 696d 616c 732e 0a0a 2020 2020  e animals...    
-0002cf60: 3a70 6172 616d 2055 6e69 6f6e 5b73 7472  :param Union[str
-0002cf70: 2c20 6f73 2e50 6174 684c 696b 655d 2076  , os.PathLike] v
-0002cf80: 6964 656f 5f70 6174 683a 2054 6865 2070  ideo_path: The p
-0002cf90: 6174 6820 746f 2074 6865 2076 6964 656f  ath to the video
-0002cfa0: 2074 6f20 7265 6d6f 7665 2074 6865 2062   to remove the b
-0002cfb0: 6163 6b67 726f 756e 6420 6672 6f6d 2e0a  ackground from..
-0002cfc0: 2020 2020 3a70 6172 616d 204f 7074 696f      :param Optio
-0002cfd0: 6e61 6c5b 556e 696f 6e5b 7374 722c 206f  nal[Union[str, o
-0002cfe0: 732e 5061 7468 4c69 6b65 5d5d 2062 675f  s.PathLike]] bg_
-0002cff0: 7669 6465 6f5f 7061 7468 3a20 5061 7468  video_path: Path
-0002d000: 2074 6f20 7468 6520 7669 6465 6f20 7768   to the video wh
-0002d010: 6963 6820 636f 6e74 6169 6e73 2061 2073  ich contains a s
-0002d020: 6567 6d65 6e74 2077 6974 6820 7468 6520  egment with the 
-0002d030: 6261 636b 6772 6f75 6e64 206f 6e6c 792e  background only.
-0002d040: 2049 6620 4e6f 6e65 2c20 7468 656e 2060   If None, then `
-0002d050: 6076 6964 656f 5f70 6174 6860 6020 7769  `video_path`` wi
-0002d060: 6c6c 2062 6520 7573 6564 2e0a 2020 2020  ll be used..    
-0002d070: 3a70 6172 616d 204f 7074 696f 6e61 6c5b  :param Optional[
-0002d080: 696e 745d 2062 675f 7374 6172 745f 6672  int] bg_start_fr
-0002d090: 6d3a 2054 6865 2066 6972 7374 2066 7261  m: The first fra
-0002d0a0: 6d65 2069 6e20 7468 6520 6261 636b 6772  me in the backgr
-0002d0b0: 6f75 6e64 2076 6964 656f 2074 6f20 7573  ound video to us
-0002d0c0: 6520 7768 656e 2063 7265 6174 696e 6720  e when creating 
-0002d0d0: 6120 7265 7072 6573 656e 7461 7469 7665  a representative
-0002d0e0: 2062 6163 6b67 726f 756e 6420 696d 6167   background imag
-0002d0f0: 652e 2044 6566 6175 6c74 3a20 4e6f 6e65  e. Default: None
-0002d100: 2e0a 2020 2020 3a70 6172 616d 204f 7074  ..    :param Opt
-0002d110: 696f 6e61 6c5b 696e 745d 2062 675f 656e  ional[int] bg_en
-0002d120: 645f 6672 6d3a 2054 6865 206c 6173 7420  d_frm: The last 
-0002d130: 6672 616d 6520 696e 2074 6865 2062 6163  frame in the bac
-0002d140: 6b67 726f 756e 6420 7669 6465 6f20 746f  kground video to
-0002d150: 2075 7365 2077 6865 6e20 6372 6561 7469   use when creati
-0002d160: 6e67 2061 2072 6570 7265 7365 6e74 6174  ng a representat
-0002d170: 6976 6520 6261 636b 6772 6f75 6e64 2069  ive background i
-0002d180: 6d61 6765 2e20 4465 6661 756c 743a 204e  mage. Default: N
-0002d190: 6f6e 652e 0a20 2020 203a 7061 7261 6d20  one..    :param 
-0002d1a0: 4f70 7469 6f6e 616c 5b73 7472 5d20 6267  Optional[str] bg
-0002d1b0: 5f73 7461 7274 5f74 696d 653a 2054 6865  _start_time: The
-0002d1c0: 2073 7461 7274 2074 696d 6573 7461 6d70   start timestamp
-0002d1d0: 2069 6e20 6048 483a 4d4d 3a53 5360 2066   in `HH:MM:SS` f
-0002d1e0: 6f72 6d61 7420 696e 2074 6865 2062 6163  ormat in the bac
-0002d1f0: 6b67 726f 756e 6420 7669 6465 6f20 746f  kground video to
-0002d200: 2075 7365 2074 6f20 6372 6561 7465 2061   use to create a
-0002d210: 2072 6570 7265 7365 6e74 6174 6976 6520   representative 
-0002d220: 6261 636b 6772 6f75 6e64 2069 6d61 6765  background image
-0002d230: 2e20 4465 6661 756c 743a 204e 6f6e 652e  . Default: None.
-0002d240: 0a20 2020 203a 7061 7261 6d20 4f70 7469  .    :param Opti
-0002d250: 6f6e 616c 5b73 7472 5d20 6267 5f65 6e64  onal[str] bg_end
-0002d260: 5f74 696d 653a 2054 6865 2065 6e64 2074  _time: The end t
-0002d270: 696d 6573 7461 6d70 2069 6e20 6048 483a  imestamp in `HH:
-0002d280: 4d4d 3a53 5360 2066 6f72 6d61 7420 696e  MM:SS` format in
-0002d290: 2074 6865 2062 6163 6b67 726f 756e 6420   the background 
-0002d2a0: 7669 6465 6f20 746f 2075 7365 2074 6f20  video to use to 
-0002d2b0: 6372 6561 7465 2061 2072 6570 7265 7365  create a represe
-0002d2c0: 6e74 6174 6976 6520 6261 636b 6772 6f75  ntative backgrou
-0002d2d0: 6e64 2069 6d61 6765 2e20 4465 6661 756c  nd image. Defaul
-0002d2e0: 743a 204e 6f6e 652e 0a20 2020 203a 7061  t: None..    :pa
-0002d2f0: 7261 6d20 4f70 7469 6f6e 616c 5b54 7570  ram Optional[Tup
-0002d300: 6c65 5b69 6e74 2c20 696e 742c 2069 6e74  le[int, int, int
-0002d310: 5d5d 2062 675f 636f 6c6f 723a 2054 6865  ]] bg_color: The
-0002d320: 2052 4742 2063 6f6c 6f72 206f 6620 7468   RGB color of th
-0002d330: 6520 6d6f 7669 6e67 206f 626a 6563 7473  e moving objects
-0002d340: 2069 6e20 7468 6520 6f75 7470 7574 2076   in the output v
-0002d350: 6964 656f 2e20 4465 6661 756c 7473 2074  ideo. Defaults t
-0002d360: 6f20 4e6f 6e65 2c20 7768 6963 6820 7265  o None, which re
-0002d370: 7072 6573 656e 7473 2074 6865 206f 7269  presents the ori
-0002d380: 6769 6e61 6c20 636f 6c6f 7273 206f 6620  ginal colors of 
-0002d390: 7468 6520 6d6f 7669 6e67 206f 626a 6563  the moving objec
-0002d3a0: 7473 2e0a 2020 2020 3a70 6172 616d 204f  ts..    :param O
-0002d3b0: 7074 696f 6e61 6c5b 5475 706c 655b 696e  ptional[Tuple[in
-0002d3c0: 742c 2069 6e74 2c20 696e 745d 5d20 6667  t, int, int]] fg
-0002d3d0: 5f63 6f6c 6f72 3a20 5468 6520 5247 4220  _color: The RGB 
-0002d3e0: 636f 6c6f 7220 6f66 2074 6865 2062 6163  color of the bac
-0002d3f0: 6b67 726f 756e 6420 6f75 7470 7574 2076  kground output v
-0002d400: 6964 656f 2e20 4465 6661 756c 7473 2074  ideo. Defaults t
-0002d410: 6f20 626c 6163 6b20 2830 2c20 302c 2030  o black (0, 0, 0
-0002d420: 292e 0a20 2020 203a 7061 7261 6d20 4f70  )..    :param Op
-0002d430: 7469 6f6e 616c 5b55 6e69 6f6e 5b73 7472  tional[Union[str
-0002d440: 2c20 6f73 2e50 6174 684c 696b 655d 5d20  , os.PathLike]] 
-0002d450: 7361 7665 5f70 6174 683a 2054 6865 2070  save_path: The p
-0002d460: 6174 6368 2074 6f20 7768 6572 6520 746f  atch to where to
-0002d470: 2073 6176 6520 7468 6520 6f75 7470 7574   save the output
-0002d480: 2076 6964 656f 2077 6865 7265 2074 6865   video where the
-0002d490: 2062 6163 6b67 726f 756e 6420 6973 2072   background is r
-0002d4a0: 656d 6f76 6564 2e20 4966 204e 6f6e 652c  emoved. If None,
-0002d4b0: 2073 6176 6573 2074 6865 206f 7574 7075   saves the outpu
-0002d4c0: 7420 7669 6465 6f20 696e 2074 6865 2073  t video in the s
-0002d4d0: 616d 6520 6469 7265 6374 6f72 7920 6173  ame directory as
-0002d4e0: 2074 6865 2069 6e70 7574 2076 6964 656f   the input video
-0002d4f0: 2077 6974 6820 7468 6520 6060 5f62 675f   with the ``_bg_
-0002d500: 7375 6274 7261 6374 6564 6060 2073 7566  subtracted`` suf
-0002d510: 6669 782e 2044 6566 6175 6c74 3a20 4e6f  fix. Default: No
-0002d520: 6e65 2e0a 2020 2020 3a70 6172 616d 204f  ne..    :param O
-0002d530: 7074 696f 6e61 6c5b 696e 745d 2063 6f72  ptional[int] cor
-0002d540: 655f 636e 743a 2054 6865 206e 756d 6265  e_cnt: The numbe
-0002d550: 7220 6f66 2063 6f72 6573 2074 6f20 7573  r of cores to us
-0002d560: 652e 2044 6566 6175 6c74 7320 746f 202d  e. Defaults to -
-0002d570: 3120 7265 7072 6573 656e 7469 6e67 2061  1 representing a
-0002d580: 6c6c 2061 7661 696c 6162 6c65 2063 6f72  ll available cor
-0002d590: 6573 2e0a 2020 2020 3a72 6574 7572 6e3a  es..    :return:
-0002d5a0: 204e 6f6e 652e 0a0a 2020 2020 3a65 7861   None...    :exa
-0002d5b0: 6d70 6c65 3a0a 2020 2020 3e3e 3e20 7669  mple:.    >>> vi
-0002d5c0: 6465 6f5f 6267 5f73 7562 7374 7261 6374  deo_bg_substract
-0002d5d0: 696f 6e5f 6d70 2876 6964 656f 5f70 6174  ion_mp(video_pat
-0002d5e0: 683d 272f 5573 6572 732f 7369 6d6f 6e2f  h='/Users/simon/
-0002d5f0: 446f 776e 6c6f 6164 732f 315f 4c48 2e6d  Downloads/1_LH.m
-0002d600: 7034 272c 2062 675f 7374 6172 745f 7469  p4', bg_start_ti
-0002d610: 6d65 3d27 3030 3a30 303a 3030 272c 2062  me='00:00:00', b
-0002d620: 675f 656e 645f 7469 6d65 3d27 3030 3a30  g_end_time='00:0
-0002d630: 303a 3130 272c 2062 675f 636f 6c6f 723d  0:10', bg_color=
-0002d640: 2830 2c20 302c 2030 292c 2066 675f 636f  (0, 0, 0), fg_co
-0002d650: 6c6f 723d 2832 3535 2c20 3235 352c 2032  lor=(255, 255, 2
-0002d660: 3535 2929 0a20 2020 2022 2222 0a0a 2020  55)).    """..  
-0002d670: 2020 7469 6d65 7220 3d20 5369 6d62 6154    timer = SimbaT
-0002d680: 696d 6572 2873 7461 7274 3d54 7275 6529  imer(start=True)
-0002d690: 0a20 2020 2063 6865 636b 5f66 696c 655f  .    check_file_
-0002d6a0: 6578 6973 745f 616e 645f 7265 6164 6162  exist_and_readab
-0002d6b0: 6c65 2866 696c 655f 7061 7468 3d76 6964  le(file_path=vid
-0002d6c0: 656f 5f70 6174 6829 0a20 2020 2069 6620  eo_path).    if 
-0002d6d0: 6267 5f76 6964 656f 5f70 6174 6820 6973  bg_video_path is
-0002d6e0: 204e 6f6e 653a 0a20 2020 2020 2020 2062   None:.        b
-0002d6f0: 675f 7669 6465 6f5f 7061 7468 203d 2064  g_video_path = d
-0002d700: 6565 7063 6f70 7928 7669 6465 6f5f 7061  eepcopy(video_pa
-0002d710: 7468 290a 2020 2020 7669 6465 6f5f 6d65  th).    video_me
-0002d720: 7461 5f64 6174 6120 3d20 6765 745f 7669  ta_data = get_vi
-0002d730: 6465 6f5f 6d65 7461 5f64 6174 6128 7669  deo_meta_data(vi
-0002d740: 6465 6f5f 7061 7468 3d76 6964 656f 5f70  deo_path=video_p
-0002d750: 6174 6829 0a20 2020 2064 6972 2c20 7669  ath).    dir, vi
-0002d760: 6465 6f5f 6e61 6d65 2c20 6578 7420 3d20  deo_name, ext = 
-0002d770: 6765 745f 666e 5f65 7874 2866 696c 6570  get_fn_ext(filep
-0002d780: 6174 683d 7669 6465 6f5f 7061 7468 290a  ath=video_path).
-0002d790: 2020 2020 6966 2073 6176 655f 7061 7468      if save_path
-0002d7a0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-0002d7b0: 2020 7361 7665 5f70 6174 6820 3d20 6f73    save_path = os
-0002d7c0: 2e70 6174 682e 6a6f 696e 2864 6972 2c20  .path.join(dir, 
-0002d7d0: 6627 7b76 6964 656f 5f6e 616d 657d 5f62  f'{video_name}_b
-0002d7e0: 675f 7375 6274 7261 6374 6564 7b65 7874  g_subtracted{ext
-0002d7f0: 7d27 290a 2020 2020 6474 203d 2064 6174  }').    dt = dat
-0002d800: 6574 696d 652e 6e6f 7728 292e 7374 7266  etime.now().strf
-0002d810: 7469 6d65 2822 2559 256d 2564 2548 254d  time("%Y%m%d%H%M
-0002d820: 2553 2229 0a20 2020 2074 656d 705f 6469  %S").    temp_di
-0002d830: 7220 3d20 6f73 2e70 6174 682e 6a6f 696e  r = os.path.join
-0002d840: 2864 6972 2c20 6627 7465 6d70 5f7b 7669  (dir, f'temp_{vi
-0002d850: 6465 6f5f 6e61 6d65 7d5f 7b64 747d 2729  deo_name}_{dt}')
-0002d860: 0a20 2020 206f 732e 6d61 6b65 6469 7273  .    os.makedirs
-0002d870: 2874 656d 705f 6469 7229 0a20 2020 2063  (temp_dir).    c
-0002d880: 6865 636b 5f69 6e74 286e 616d 653d 6627  heck_int(name=f'
-0002d890: 7b76 6964 656f 5f62 675f 7375 6273 7472  {video_bg_substr
-0002d8a0: 6163 7469 6f6e 5f6d 702e 5f5f 6e61 6d65  action_mp.__name
-0002d8b0: 5f5f 7d20 636f 7265 5f63 6e74 272c 2076  __} core_cnt', v
-0002d8c0: 616c 7565 3d63 6f72 655f 636e 742c 206d  alue=core_cnt, m
-0002d8d0: 696e 5f76 616c 7565 3d2d 312c 206d 6178  in_value=-1, max
-0002d8e0: 5f76 616c 7565 3d66 696e 645f 636f 7265  _value=find_core
-0002d8f0: 5f63 6e74 2829 5b30 5d29 0a20 2020 2069  _cnt()[0]).    i
-0002d900: 6620 636f 7265 5f63 6e74 203d 3d20 2d31  f core_cnt == -1
-0002d910: 3a20 636f 7265 5f63 6e74 203d 2066 696e  : core_cnt = fin
-0002d920: 645f 636f 7265 5f63 6e74 2829 5b30 5d0a  d_core_cnt()[0].
-0002d930: 2020 2020 6267 5f66 726d 203d 2063 7265      bg_frm = cre
-0002d940: 6174 655f 6176 6572 6167 655f 6672 6d28  ate_average_frm(
-0002d950: 7669 6465 6f5f 7061 7468 3d62 675f 7669  video_path=bg_vi
-0002d960: 6465 6f5f 7061 7468 2c20 7374 6172 745f  deo_path, start_
-0002d970: 6672 6d3d 6267 5f73 7461 7274 5f66 726d  frm=bg_start_frm
-0002d980: 2c20 656e 645f 6672 6d3d 6267 5f65 6e64  , end_frm=bg_end
-0002d990: 5f66 726d 2c20 7374 6172 745f 7469 6d65  _frm, start_time
-0002d9a0: 3d62 675f 7374 6172 745f 7469 6d65 2c20  =bg_start_time, 
-0002d9b0: 656e 645f 7469 6d65 3d62 675f 656e 645f  end_time=bg_end_
-0002d9c0: 7469 6d65 290a 2020 2020 6267 5f66 726d  time).    bg_frm
-0002d9d0: 203d 2063 7632 2e72 6573 697a 6528 6267   = cv2.resize(bg
-0002d9e0: 5f66 726d 2c20 2876 6964 656f 5f6d 6574  _frm, (video_met
-0002d9f0: 615f 6461 7461 5b27 7769 6474 6827 5d2c  a_data['width'],
-0002da00: 2076 6964 656f 5f6d 6574 615f 6461 7461   video_meta_data
-0002da10: 5b27 6865 6967 6874 275d 2929 0a20 2020  ['height'])).   
-0002da20: 2062 675f 6672 6d20 3d20 6267 5f66 726d   bg_frm = bg_frm
-0002da30: 5b3a 2c20 3a2c 203a 3a2d 315d 0a20 2020  [:, :, ::-1].   
-0002da40: 2066 726d 5f6c 6973 7420 3d20 6e70 2e61   frm_list = np.a
-0002da50: 7272 6179 5f73 706c 6974 286c 6973 7428  rray_split(list(
-0002da60: 7261 6e67 6528 302c 2076 6964 656f 5f6d  range(0, video_m
-0002da70: 6574 615f 6461 7461 5b27 6672 616d 655f  eta_data['frame_
-0002da80: 636f 756e 7427 5d29 292c 2063 6f72 655f  count'])), core_
-0002da90: 636e 7429 0a20 2020 2066 726d 5f64 6174  cnt).    frm_dat
-0002daa0: 6120 3d20 5b5d 0a20 2020 2066 6f72 2063  a = [].    for c
-0002dab0: 2c20 6920 696e 2065 6e75 6d65 7261 7465  , i in enumerate
-0002dac0: 2866 726d 5f6c 6973 7429 3a0a 2020 2020  (frm_list):.    
-0002dad0: 2020 2020 6672 6d5f 6461 7461 2e61 7070      frm_data.app
-0002dae0: 656e 6428 2863 2c20 6929 290a 2020 2020  end((c, i)).    
-0002daf0: 7769 7468 206d 756c 7469 7072 6f63 6573  with multiproces
-0002db00: 7369 6e67 2e50 6f6f 6c28 636f 7265 5f63  sing.Pool(core_c
-0002db10: 6e74 2c20 6d61 7874 6173 6b73 7065 7263  nt, maxtasksperc
-0002db20: 6869 6c64 3d39 3030 3029 2061 7320 706f  hild=9000) as po
-0002db30: 6f6c 3a0a 2020 2020 2020 2020 636f 6e73  ol:.        cons
-0002db40: 7461 6e74 7320 3d20 6675 6e63 746f 6f6c  tants = functool
-0002db50: 732e 7061 7274 6961 6c28 5f62 675f 7265  s.partial(_bg_re
-0002db60: 6d6f 7665 725f 6d70 2c0a 2020 2020 2020  mover_mp,.      
-0002db70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002db80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002db90: 7669 6465 6f5f 7061 7468 3d76 6964 656f  video_path=video
-0002dba0: 5f70 6174 682c 0a20 2020 2020 2020 2020  _path,.         
+0002ba50: 2766 7073 275d 2c0a 2020 2020 2020 2020  'fps'],.        
+0002ba60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002ba70: 2020 2020 2028 7669 6465 6f5f 6d65 7461       (video_meta
+0002ba80: 5f64 6174 615b 2777 6964 7468 275d 2c20  _data['width'], 
+0002ba90: 7669 6465 6f5f 6d65 7461 5f64 6174 615b  video_meta_data[
+0002baa0: 2768 6569 6768 7427 5d29 290a 2020 2020  'height'])).    
+0002bab0: 6267 5f66 726d 203d 2063 7265 6174 655f  bg_frm = create_
+0002bac0: 6176 6572 6167 655f 6672 6d28 7669 6465  average_frm(vide
+0002bad0: 6f5f 7061 7468 3d62 675f 7669 6465 6f5f  o_path=bg_video_
+0002bae0: 7061 7468 2c20 7374 6172 745f 6672 6d3d  path, start_frm=
+0002baf0: 6267 5f73 7461 7274 5f66 726d 2c20 656e  bg_start_frm, en
+0002bb00: 645f 6672 6d3d 6267 5f65 6e64 5f66 726d  d_frm=bg_end_frm
+0002bb10: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0002bb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002bb30: 2020 7374 6172 745f 7469 6d65 3d62 675f    start_time=bg_
+0002bb40: 7374 6172 745f 7469 6d65 2c20 656e 645f  start_time, end_
+0002bb50: 7469 6d65 3d62 675f 656e 645f 7469 6d65  time=bg_end_time
+0002bb60: 290a 2020 2020 6267 5f66 726d 203d 2063  ).    bg_frm = c
+0002bb70: 7632 2e72 6573 697a 6528 6267 5f66 726d  v2.resize(bg_frm
+0002bb80: 2c20 2876 6964 656f 5f6d 6574 615f 6461  , (video_meta_da
+0002bb90: 7461 5b27 7769 6474 6827 5d2c 2076 6964  ta['width'], vid
+0002bba0: 656f 5f6d 6574 615f 6461 7461 5b27 6865  eo_meta_data['he
+0002bbb0: 6967 6874 275d 2929 0a20 2020 2062 6720  ight'])).    bg 
+0002bbc0: 3d20 6376 322e 6376 7443 6f6c 6f72 286e  = cv2.cvtColor(n
+0002bbd0: 702e 6675 6c6c 5f6c 696b 6528 6267 5f66  p.full_like(bg_f
+0002bbe0: 726d 2c20 6267 5f63 6f6c 6f72 292c 2063  rm, bg_color), c
+0002bbf0: 7632 2e43 4f4c 4f52 5f42 4752 3252 4742  v2.COLOR_BGR2RGB
+0002bc00: 290a 2020 2020 6361 7020 3d20 6376 322e  ).    cap = cv2.
+0002bc10: 5669 6465 6f43 6170 7475 7265 2876 6964  VideoCapture(vid
+0002bc20: 656f 5f70 6174 6829 0a20 2020 2066 726d  eo_path).    frm
+0002bc30: 5f63 6e74 203d 2030 0a20 2020 2077 6869  _cnt = 0.    whi
+0002bc40: 6c65 2054 7275 653a 0a20 2020 2020 2020  le True:.       
+0002bc50: 2072 6574 2c20 6672 6d20 3d20 6361 702e   ret, frm = cap.
+0002bc60: 7265 6164 2829 0a20 2020 2020 2020 2069  read().        i
+0002bc70: 6620 6e6f 7420 7265 743a 0a20 2020 2020  f not ret:.     
+0002bc80: 2020 2020 2020 2062 7265 616b 0a20 2020         break.   
+0002bc90: 2020 2020 2064 6966 6620 3d20 6376 322e       diff = cv2.
+0002bca0: 6162 7364 6966 6628 6672 6d2c 2062 675f  absdiff(frm, bg_
+0002bcb0: 6672 6d29 0a20 2020 2020 2020 2067 7261  frm).        gra
+0002bcc0: 795f 6469 6666 203d 2063 7632 2e63 7674  y_diff = cv2.cvt
+0002bcd0: 436f 6c6f 7228 6469 6666 2c20 6376 322e  Color(diff, cv2.
+0002bce0: 434f 4c4f 525f 4247 5232 4752 4159 290a  COLOR_BGR2GRAY).
+0002bcf0: 2020 2020 2020 2020 5f2c 206d 6173 6b20          _, mask 
+0002bd00: 3d20 6376 322e 7468 7265 7368 6f6c 6428  = cv2.threshold(
+0002bd10: 6772 6179 5f64 6966 662c 2035 302c 2032  gray_diff, 50, 2
+0002bd20: 3535 2c20 6376 322e 5448 5245 5348 5f42  55, cv2.THRESH_B
+0002bd30: 494e 4152 5929 0a20 2020 2020 2020 2069  INARY).        i
+0002bd40: 6620 6667 5f63 6f6c 6f72 2069 7320 4e6f  f fg_color is No
+0002bd50: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0002bd60: 6667 203d 2063 7632 2e62 6974 7769 7365  fg = cv2.bitwise
+0002bd70: 5f61 6e64 2866 726d 2c20 6672 6d2c 206d  _and(frm, frm, m
+0002bd80: 6173 6b3d 6d61 736b 290a 2020 2020 2020  ask=mask).      
+0002bd90: 2020 2020 2020 7265 7375 6c74 203d 2063        result = c
+0002bda0: 7632 2e61 6464 2862 672c 2066 6729 0a20  v2.add(bg, fg). 
+0002bdb0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0002bdc0: 2020 2020 2020 2020 206d 6173 6b5f 696e           mask_in
+0002bdd0: 7620 3d20 6376 322e 6269 7477 6973 655f  v = cv2.bitwise_
+0002bde0: 6e6f 7428 6d61 736b 290a 2020 2020 2020  not(mask).      
+0002bdf0: 2020 2020 2020 6667 5f63 6c72 203d 2063        fg_clr = c
+0002be00: 7632 2e63 7674 436f 6c6f 7228 6e70 2e66  v2.cvtColor(np.f
+0002be10: 756c 6c5f 6c69 6b65 2866 726d 2c20 6667  ull_like(frm, fg
+0002be20: 5f63 6f6c 6f72 292c 2063 7632 2e43 4f4c  _color), cv2.COL
+0002be30: 4f52 5f42 4752 3252 4742 290a 2020 2020  OR_BGR2RGB).    
+0002be40: 2020 2020 2020 2020 6667 5f63 6c72 203d          fg_clr =
+0002be50: 2063 7632 2e62 6974 7769 7365 5f61 6e64   cv2.bitwise_and
+0002be60: 2866 675f 636c 722c 2066 675f 636c 722c  (fg_clr, fg_clr,
+0002be70: 206d 6173 6b3d 6d61 736b 290a 2020 2020   mask=mask).    
+0002be80: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+0002be90: 2063 7632 2e62 6974 7769 7365 5f61 6e64   cv2.bitwise_and
+0002bea0: 2862 672c 2062 672c 206d 6173 6b3d 6d61  (bg, bg, mask=ma
+0002beb0: 736b 5f69 6e76 290a 2020 2020 2020 2020  sk_inv).        
+0002bec0: 2020 2020 7265 7375 6c74 203d 2063 7632      result = cv2
+0002bed0: 2e61 6464 2872 6573 756c 742c 2066 675f  .add(result, fg_
+0002bee0: 636c 7229 0a20 2020 2020 2020 2077 7269  clr).        wri
+0002bef0: 7465 722e 7772 6974 6528 7265 7375 6c74  ter.write(result
+0002bf00: 290a 2020 2020 2020 2020 6672 6d5f 636e  ).        frm_cn
+0002bf10: 7420 2b3d 2031 0a20 2020 2020 2020 2070  t += 1.        p
+0002bf20: 7269 6e74 2866 2742 6163 6b67 726f 756e  rint(f'Backgroun
+0002bf30: 6420 7375 6274 7261 6374 696f 6e20 6672  d subtraction fr
+0002bf40: 616d 6520 7b66 726d 5f63 6e74 7d2f 7b76  ame {frm_cnt}/{v
+0002bf50: 6964 656f 5f6d 6574 615f 6461 7461 5b22  ideo_meta_data["
+0002bf60: 6672 616d 655f 636f 756e 7422 5d7d 2028  frame_count"]} (
+0002bf70: 5669 6465 6f3a 207b 7669 6465 6f5f 6e61  Video: {video_na
+0002bf80: 6d65 7d29 2729 0a0a 2020 2020 7772 6974  me})')..    writ
+0002bf90: 6572 2e72 656c 6561 7365 2829 0a20 2020  er.release().   
+0002bfa0: 2063 6170 2e72 656c 6561 7365 2829 0a20   cap.release(). 
+0002bfb0: 2020 2074 696d 6572 2e73 746f 705f 7469     timer.stop_ti
+0002bfc0: 6d65 7228 290a 2020 2020 7374 646f 7574  mer().    stdout
+0002bfd0: 5f73 7563 6365 7373 286d 7367 3d66 2742  _success(msg=f'B
+0002bfe0: 6163 6b67 726f 756e 6420 7375 6274 7261  ackground subtra
+0002bff0: 6374 6564 2066 726f 6d20 7b76 6964 656f  cted from {video
+0002c000: 5f6e 616d 657d 2061 6e64 2073 6176 6564  _name} and saved
+0002c010: 2061 7420 7b73 6176 655f 7061 7468 7d27   at {save_path}'
+0002c020: 2c20 656c 6170 7365 645f 7469 6d65 3d74  , elapsed_time=t
+0002c030: 696d 6572 2e65 6c61 7073 6564 5f74 696d  imer.elapsed_tim
+0002c040: 6529 0a0a 6465 6620 5f62 675f 7265 6d6f  e)..def _bg_remo
+0002c050: 7665 725f 6d70 2866 726d 5f72 616e 6765  ver_mp(frm_range
+0002c060: 3a20 5475 706c 655b 696e 742c 206e 702e  : Tuple[int, np.
+0002c070: 6e64 6172 7261 795d 2c0a 2020 2020 2020  ndarray],.      
+0002c080: 2020 2020 2020 2020 2020 2020 2076 6964               vid
+0002c090: 656f 5f70 6174 683a 2055 6e69 6f6e 5b73  eo_path: Union[s
+0002c0a0: 7472 2c20 6f73 2e50 6174 684c 696b 655d  tr, os.PathLike]
+0002c0b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0002c0c0: 2020 2020 2062 675f 6672 6d3a 206e 702e       bg_frm: np.
+0002c0d0: 6e64 6172 7261 792c 0a20 2020 2020 2020  ndarray,.       
+0002c0e0: 2020 2020 2020 2020 2020 2020 6267 5f63              bg_c
+0002c0f0: 6c72 3a20 5475 706c 655b 696e 742c 2069  lr: Tuple[int, i
+0002c100: 6e74 2c20 696e 745d 2c0a 2020 2020 2020  nt, int],.      
+0002c110: 2020 2020 2020 2020 2020 2020 2066 675f               fg_
+0002c120: 636c 723a 2054 7570 6c65 5b69 6e74 2c20  clr: Tuple[int, 
+0002c130: 696e 742c 2069 6e74 5d2c 0a20 2020 2020  int, int],.     
+0002c140: 2020 2020 2020 2020 2020 2020 2020 7669                vi
+0002c150: 6465 6f5f 6d65 7461 5f64 6174 613a 2044  deo_meta_data: D
+0002c160: 6963 745b 7374 722c 2041 6e79 5d2c 0a20  ict[str, Any],. 
+0002c170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002c180: 2020 7465 6d70 5f64 6972 3a20 556e 696f    temp_dir: Unio
+0002c190: 6e5b 7374 722c 206f 732e 5061 7468 4c69  n[str, os.PathLi
+0002c1a0: 6b65 5d29 3a0a 0a20 2020 2062 6174 6368  ke]):..    batch
+0002c1b0: 2c20 6672 6d5f 7261 6e67 6520 3d20 6672  , frm_range = fr
+0002c1c0: 6d5f 7261 6e67 655b 305d 2c20 6672 6d5f  m_range[0], frm_
+0002c1d0: 7261 6e67 655b 315d 0a20 2020 2073 7461  range[1].    sta
+0002c1e0: 7274 5f66 726d 2c20 6375 7272 656e 745f  rt_frm, current_
+0002c1f0: 6672 6d2c 2065 6e64 5f66 726d 203d 2066  frm, end_frm = f
+0002c200: 726d 5f72 616e 6765 5b30 5d2c 2066 726d  rm_range[0], frm
+0002c210: 5f72 616e 6765 5b30 5d2c 2066 726d 5f72  _range[0], frm_r
+0002c220: 616e 6765 5b2d 315d 0a20 2020 2063 6170  ange[-1].    cap
+0002c230: 203d 2063 7632 2e56 6964 656f 4361 7074   = cv2.VideoCapt
+0002c240: 7572 6528 7669 6465 6f5f 7061 7468 290a  ure(video_path).
+0002c250: 2020 2020 666f 7572 6363 203d 2063 7632      fourcc = cv2
+0002c260: 2e56 6964 656f 5772 6974 6572 5f66 6f75  .VideoWriter_fou
+0002c270: 7263 6328 2a46 6f72 6d61 7473 2e4d 5034  rcc(*Formats.MP4
+0002c280: 5f43 4f44 4543 2e76 616c 7565 290a 2020  _CODEC.value).  
+0002c290: 2020 7361 7665 5f70 6174 6820 3d20 6f73    save_path = os
+0002c2a0: 2e70 6174 682e 6a6f 696e 2874 656d 705f  .path.join(temp_
+0002c2b0: 6469 722c 2066 227b 6261 7463 687d 2e6d  dir, f"{batch}.m
+0002c2c0: 7034 2229 0a20 2020 2063 6170 2e73 6574  p4").    cap.set
+0002c2d0: 2831 2c20 7374 6172 745f 6672 6d29 0a20  (1, start_frm). 
+0002c2e0: 2020 2077 7269 7465 7220 3d20 6376 322e     writer = cv2.
+0002c2f0: 5669 6465 6f57 7269 7465 7228 7361 7665  VideoWriter(save
+0002c300: 5f70 6174 682c 2066 6f75 7263 632c 2076  _path, fourcc, v
+0002c310: 6964 656f 5f6d 6574 615f 6461 7461 5b27  ideo_meta_data['
+0002c320: 6670 7327 5d2c 2028 7669 6465 6f5f 6d65  fps'], (video_me
+0002c330: 7461 5f64 6174 615b 2777 6964 7468 275d  ta_data['width']
+0002c340: 2c20 7669 6465 6f5f 6d65 7461 5f64 6174  , video_meta_dat
+0002c350: 615b 2768 6569 6768 7427 5d29 290a 2020  a['height'])).  
+0002c360: 2020 6267 203d 206e 702e 6675 6c6c 5f6c    bg = np.full_l
+0002c370: 696b 6528 6267 5f66 726d 2c20 6267 5f63  ike(bg_frm, bg_c
+0002c380: 6c72 290a 2020 2020 6267 203d 2062 675b  lr).    bg = bg[
+0002c390: 3a2c 203a 2c20 3a3a 2d31 5d0a 2020 2020  :, :, ::-1].    
+0002c3a0: 6469 722c 2076 6964 656f 5f6e 616d 652c  dir, video_name,
+0002c3b0: 2065 7874 203d 2067 6574 5f66 6e5f 6578   ext = get_fn_ex
+0002c3c0: 7428 6669 6c65 7061 7468 3d76 6964 656f  t(filepath=video
+0002c3d0: 5f70 6174 6829 0a20 2020 2077 6869 6c65  _path).    while
+0002c3e0: 2063 7572 7265 6e74 5f66 726d 203c 3d20   current_frm <= 
+0002c3f0: 656e 645f 6672 6d3a 0a20 2020 2020 2020  end_frm:.       
+0002c400: 2072 6574 2c20 6672 6d20 3d20 6361 702e   ret, frm = cap.
+0002c410: 7265 6164 2829 0a20 2020 2020 2020 2069  read().        i
+0002c420: 6620 6e6f 7420 7265 743a 0a20 2020 2020  f not ret:.     
+0002c430: 2020 2020 2020 2062 7265 616b 0a20 2020         break.   
+0002c440: 2020 2020 2064 6966 6620 3d20 6376 322e       diff = cv2.
+0002c450: 6162 7364 6966 6628 6672 6d2c 2062 675f  absdiff(frm, bg_
+0002c460: 6672 6d29 0a20 2020 2020 2020 2062 2c20  frm).        b, 
+0002c470: 672c 2072 203d 2064 6966 665b 3a2c 203a  g, r = diff[:, :
+0002c480: 2c20 305d 2c20 6469 6666 5b3a 2c20 3a2c  , 0], diff[:, :,
+0002c490: 2031 5d2c 2064 6966 665b 3a2c 203a 2c20   1], diff[:, :, 
+0002c4a0: 325d 0a20 2020 2020 2020 2067 7261 795f  2].        gray_
+0002c4b0: 6469 6666 203d 2030 2e32 3938 3920 2a20  diff = 0.2989 * 
+0002c4c0: 7220 2b20 302e 3538 3730 202a 2067 202b  r + 0.5870 * g +
+0002c4d0: 2030 2e31 3134 3020 2a20 620a 2020 2020   0.1140 * b.    
+0002c4e0: 2020 2020 6772 6179 5f64 6966 6620 3d20      gray_diff = 
+0002c4f0: 6772 6179 5f64 6966 662e 6173 7479 7065  gray_diff.astype
+0002c500: 286e 702e 7569 6e74 3829 2020 2320 456e  (np.uint8)  # En
+0002c510: 7375 7265 2074 6865 2074 7970 6520 6973  sure the type is
+0002c520: 2075 696e 7438 0a20 2020 2020 2020 206d   uint8.        m
+0002c530: 6173 6b20 3d20 6e70 2e77 6865 7265 2867  ask = np.where(g
+0002c540: 7261 795f 6469 6666 203e 2035 302c 2032  ray_diff > 50, 2
+0002c550: 3535 2c20 3029 2e61 7374 7970 6528 6e70  55, 0).astype(np
+0002c560: 2e75 696e 7438 290a 2020 2020 2020 2020  .uint8).        
+0002c570: 6966 2066 675f 636c 7220 6973 204e 6f6e  if fg_clr is Non
+0002c580: 653a 0a20 2020 2020 2020 2020 2020 2066  e:.            f
+0002c590: 6720 3d20 6376 322e 6269 7477 6973 655f  g = cv2.bitwise_
+0002c5a0: 616e 6428 6672 6d2c 2066 726d 2c20 6d61  and(frm, frm, ma
+0002c5b0: 736b 3d6d 6173 6b29 0a20 2020 2020 2020  sk=mask).       
+0002c5c0: 2020 2020 2072 6573 756c 7420 3d20 6376       result = cv
+0002c5d0: 322e 6164 6428 6267 2c20 6667 290a 2020  2.add(bg, fg).  
+0002c5e0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0002c5f0: 2020 2020 2020 2020 6d61 736b 5f69 6e76          mask_inv
+0002c600: 203d 2063 7632 2e62 6974 7769 7365 5f6e   = cv2.bitwise_n
+0002c610: 6f74 286d 6173 6b29 0a20 2020 2020 2020  ot(mask).       
+0002c620: 2020 2020 2066 675f 636c 725f 696d 6720       fg_clr_img 
+0002c630: 3d20 6e70 2e66 756c 6c5f 6c69 6b65 2866  = np.full_like(f
+0002c640: 726d 2c20 6667 5f63 6c72 290a 2020 2020  rm, fg_clr).    
+0002c650: 2020 2020 2020 2020 6667 5f63 6c72 5f69          fg_clr_i
+0002c660: 6d67 203d 2066 675f 636c 725f 696d 675b  mg = fg_clr_img[
+0002c670: 3a2c 203a 2c20 3a3a 2d31 5d0a 2020 2020  :, :, ::-1].    
+0002c680: 2020 2020 2020 2020 6667 5f63 6c72 5f69          fg_clr_i
+0002c690: 6d67 203d 2063 7632 2e62 6974 7769 7365  mg = cv2.bitwise
+0002c6a0: 5f61 6e64 2866 675f 636c 725f 696d 672c  _and(fg_clr_img,
+0002c6b0: 2066 675f 636c 725f 696d 672c 206d 6173   fg_clr_img, mas
+0002c6c0: 6b3d 6d61 736b 290a 2020 2020 2020 2020  k=mask).        
+0002c6d0: 2020 2020 7265 7375 6c74 203d 2063 7632      result = cv2
+0002c6e0: 2e62 6974 7769 7365 5f61 6e64 2862 672c  .bitwise_and(bg,
+0002c6f0: 2062 672c 206d 6173 6b3d 6d61 736b 5f69   bg, mask=mask_i
+0002c700: 6e76 290a 2020 2020 2020 2020 2020 2020  nv).            
+0002c710: 7265 7375 6c74 203d 2063 7632 2e61 6464  result = cv2.add
+0002c720: 2872 6573 756c 742c 2066 675f 636c 725f  (result, fg_clr_
+0002c730: 696d 6729 0a20 2020 2020 2020 2077 7269  img).        wri
+0002c740: 7465 722e 7772 6974 6528 7265 7375 6c74  ter.write(result
+0002c750: 290a 2020 2020 2020 2020 6375 7272 656e  ).        curren
+0002c760: 745f 6672 6d20 2b3d 2031 0a20 2020 2020  t_frm += 1.     
+0002c770: 2020 2070 7269 6e74 2866 2742 6163 6b67     print(f'Backg
+0002c780: 726f 756e 6420 7375 6274 7261 6374 696f  round subtractio
+0002c790: 6e20 6672 616d 6520 7b63 7572 7265 6e74  n frame {current
+0002c7a0: 5f66 726d 7d2f 7b76 6964 656f 5f6d 6574  _frm}/{video_met
+0002c7b0: 615f 6461 7461 5b22 6672 616d 655f 636f  a_data["frame_co
+0002c7c0: 756e 7422 5d7d 2028 5669 6465 6f3a 207b  unt"]} (Video: {
+0002c7d0: 7669 6465 6f5f 6e61 6d65 7d29 2729 0a20  video_name})'). 
+0002c7e0: 2020 2077 7269 7465 722e 7265 6c65 6173     writer.releas
+0002c7f0: 6528 290a 2020 2020 6361 702e 7265 6c65  e().    cap.rele
+0002c800: 6173 6528 290a 2020 2020 7265 7475 726e  ase().    return
+0002c810: 2062 6174 6368 0a0a 6465 6620 7669 6465   batch..def vide
+0002c820: 6f5f 6267 5f73 7562 7374 7261 6374 696f  o_bg_substractio
+0002c830: 6e5f 6d70 2876 6964 656f 5f70 6174 683a  n_mp(video_path:
+0002c840: 2055 6e69 6f6e 5b73 7472 2c20 6f73 2e50   Union[str, os.P
+0002c850: 6174 684c 696b 655d 2c0a 2020 2020 2020  athLike],.      
+0002c860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002c870: 2020 2020 2020 2062 675f 7669 6465 6f5f         bg_video_
+0002c880: 7061 7468 3a20 4f70 7469 6f6e 616c 5b55  path: Optional[U
+0002c890: 6e69 6f6e 5b73 7472 2c20 6f73 2e50 6174  nion[str, os.Pat
+0002c8a0: 684c 696b 655d 5d20 3d20 4e6f 6e65 2c0a  hLike]] = None,.
+0002c8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002c8c0: 2020 2020 2020 2020 2020 2020 2062 675f               bg_
+0002c8d0: 7374 6172 745f 6672 6d3a 204f 7074 696f  start_frm: Optio
+0002c8e0: 6e61 6c5b 696e 745d 203d 204e 6f6e 652c  nal[int] = None,
+0002c8f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002c900: 2020 2020 2020 2020 2020 2020 2020 6267                bg
+0002c910: 5f65 6e64 5f66 726d 3a20 4f70 7469 6f6e  _end_frm: Option
+0002c920: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 2c0a  al[int] = None,.
+0002c930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002c940: 2020 2020 2020 2020 2020 2020 2062 675f               bg_
+0002c950: 7374 6172 745f 7469 6d65 3a20 4f70 7469  start_time: Opti
+0002c960: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+0002c970: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0002c980: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+0002c990: 675f 656e 645f 7469 6d65 3a20 4f70 7469  g_end_time: Opti
+0002c9a0: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+0002c9b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0002c9c0: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+0002c9d0: 675f 636f 6c6f 723a 204f 7074 696f 6e61  g_color: Optiona
+0002c9e0: 6c5b 5475 706c 655b 696e 742c 2069 6e74  l[Tuple[int, int
+0002c9f0: 2c20 696e 745d 5d20 3d20 2830 2c20 302c  , int]] = (0, 0,
+0002ca00: 2030 292c 0a20 2020 2020 2020 2020 2020   0),.           
+0002ca10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002ca20: 2020 6667 5f63 6f6c 6f72 3a20 4f70 7469    fg_color: Opti
+0002ca30: 6f6e 616c 5b54 7570 6c65 5b69 6e74 2c20  onal[Tuple[int, 
+0002ca40: 696e 742c 2069 6e74 5d5d 203d 204e 6f6e  int, int]] = Non
+0002ca50: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+0002ca60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002ca70: 7361 7665 5f70 6174 683a 204f 7074 696f  save_path: Optio
+0002ca80: 6e61 6c5b 556e 696f 6e5b 7374 722c 206f  nal[Union[str, o
+0002ca90: 732e 5061 7468 4c69 6b65 5d5d 203d 204e  s.PathLike]] = N
+0002caa0: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
+0002cab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002cac0: 2020 636f 7265 5f63 6e74 3a20 4f70 7469    core_cnt: Opti
+0002cad0: 6f6e 616c 5b69 6e74 5d20 3d20 2d31 2920  onal[int] = -1) 
+0002cae0: 2d3e 204e 6f6e 653a 0a0a 2020 2020 2222  -> None:..    ""
+0002caf0: 220a 2020 2020 5375 6274 7261 6374 2074  ".    Subtract t
+0002cb00: 6865 2062 6163 6b67 726f 756e 6420 6672  he background fr
+0002cb10: 6f6d 2061 2076 6964 656f 2075 7369 6e67  om a video using
+0002cb20: 206d 756c 7469 7072 6f63 6573 7369 6e67   multiprocessing
+0002cb30: 2e0a 0a20 2020 202e 2e20 7669 6465 6f3a  ...    .. video:
+0002cb40: 3a20 5f73 7461 7469 632f 696d 672f 7669  : _static/img/vi
+0002cb50: 6465 6f5f 6267 5f73 7562 7374 7261 6374  deo_bg_substract
+0002cb60: 696f 6e5f 6d70 2e77 6562 6d0a 2020 2020  ion_mp.webm.    
+0002cb70: 2020 203a 7769 6474 683a 2039 3030 0a20     :width: 900. 
+0002cb80: 2020 2020 2020 3a61 7574 6f70 6c61 793a        :autoplay:
+0002cb90: 0a20 2020 2020 2020 3a6c 6f6f 703a 0a0a  .       :loop:..
+0002cba0: 2020 2020 2e2e 206e 6f74 653a 3a0a 2020      .. note::.  
+0002cbb0: 2020 2020 2020 466f 7220 7369 6e67 6c65        For single
+0002cbc0: 2063 6f72 6520 616c 7465 726e 6174 6976   core alternativ
+0002cbd0: 652c 2073 6565 2060 6073 696d 6261 2e76  e, see ``simba.v
+0002cbe0: 6964 656f 5f70 726f 6365 7373 6f72 732e  ideo_processors.
+0002cbf0: 7669 6465 6f5f 7072 6f63 6573 7369 6e67  video_processing
+0002cc00: 2e76 6964 656f 5f62 675f 7375 6274 7261  .video_bg_subtra
+0002cc10: 6374 696f 6e60 600a 0a20 2020 2020 2020  ction``..       
+0002cc20: 4966 2020 6060 6267 5f76 6964 656f 5f70  If  ``bg_video_p
+0002cc30: 6174 6860 6020 6973 2070 6173 7365 642c  ath`` is passed,
+0002cc40: 2074 6861 7420 7669 6465 6f20 7769 6c6c   that video will
+0002cc50: 2062 6520 7573 6564 2074 6f20 7061 7273   be used to pars
+0002cc60: 6520 7468 6520 6261 636b 6772 6f75 6e64  e the background
+0002cc70: 2e20 4966 204e 6f6e 652c 2060 6076 6964  . If None, ``vid
+0002cc80: 656f 5f70 6174 6860 6020 7769 6c6c 2062  eo_path`` will b
+0002cc90: 6520 7573 6520 6474 6f20 7061 7273 6520  e use dto parse 
+0002cca0: 6261 636b 6772 6f75 6e64 2e0a 2020 2020  background..    
+0002ccb0: 2020 2045 6974 6865 7220 7061 7373 2060     Either pass `
+0002ccc0: 6073 7461 7274 5f66 726d 6060 2061 6e64  `start_frm`` and
+0002ccd0: 2060 6065 6e64 5f66 726d 6060 204f 5220   ``end_frm`` OR 
+0002cce0: 6060 7374 6172 745f 7469 6d65 6060 2061  ``start_time`` a
+0002ccf0: 6e64 2060 6065 6e64 5f74 696d 6560 6020  nd ``end_time`` 
+0002cd00: 4f52 2070 6173 7320 616c 6c20 666f 7572  OR pass all four
+0002cd10: 2061 7267 756d 656e 7473 2061 7320 4e6f   arguments as No
+0002cd20: 6e65 2e0a 2020 2020 2020 2054 686f 7365  ne..       Those
+0002cd30: 2074 776f 2061 7267 756d 656e 7473 2077   two arguments w
+0002cd40: 696c 6c20 6265 2075 7365 6420 746f 2073  ill be used to s
+0002cd50: 6c69 6365 2074 6865 2062 6163 6b67 726f  lice the backgro
+0002cd60: 756e 6420 7669 6465 6f2c 2061 6e64 2074  und video, and t
+0002cd70: 6865 2073 6c69 6365 6420 7061 7274 2069  he sliced part i
+0002cd80: 7320 7573 6564 2074 6f20 7061 7273 6520  s used to parse 
+0002cd90: 7468 6520 6261 636b 6772 6f75 6e64 2e0a  the background..
+0002cda0: 0a20 2020 2020 2020 466f 7220 6578 616d  .       For exam
+0002cdb0: 706c 652c 2069 6e20 7468 6520 7363 656e  ple, in the scen
+0002cdc0: 6172 696f 2077 6865 7265 2074 6865 7265  ario where there
+0002cdd0: 2069 7320 2a2a 6e6f 2a2a 2061 6e69 6d61   is **no** anima
+0002cde0: 6c20 696e 2074 6865 2060 6076 6964 656f  l in the ``video
+0002cdf0: 5f70 6174 6860 6020 7669 6465 6f20 666f  _path`` video fo
+0002ce00: 7220 7468 6520 6669 7273 7420 3230 732c  r the first 20s,
+0002ce10: 2074 6865 6e20 7468 6520 6669 7273 7420   then the first 
+0002ce20: 3230 7320 6361 6e20 6265 2075 7365 6420  20s can be used 
+0002ce30: 746f 2070 6172 7365 2074 6865 2062 6163  to parse the bac
+0002ce40: 6b67 726f 756e 642e 0a20 2020 2020 2020  kground..       
+0002ce50: 496e 2074 6869 7320 7363 656e 6172 696f  In this scenario
+0002ce60: 2c20 6060 6267 5f76 6964 656f 5f70 6174  , ``bg_video_pat
+0002ce70: 6860 6020 6361 6e20 6265 2070 6173 7365  h`` can be passe
+0002ce80: 6420 6173 2060 604e 6f6e 6560 6020 616e  d as ``None`` an
+0002ce90: 6420 6267 5f73 7461 7274 5f74 696d 6520  d bg_start_time 
+0002cea0: 616e 6420 6267 5f65 6e64 5f74 696d 6520  and bg_end_time 
+0002ceb0: 6361 6e20 6265 2060 6030 303a 3030 3a30  can be ``00:00:0
+0002cec0: 3060 6020 616e 6420 6060 3030 3a30 303a  0`` and ``00:00:
+0002ced0: 3230 6060 2c20 7265 7065 6374 6976 656c  20``, repectivel
+0002cee0: 792e 0a0a 2020 2020 2020 2049 6e20 7468  y...       In th
+0002cef0: 6520 7363 656e 6172 696f 2077 6865 7265  e scenario where
+0002cf00: 2074 6865 7265 202a 2a69 732a 2a20 616e   there **is** an
+0002cf10: 696d 616c 2873 2920 696e 2074 6865 2065  imal(s) in the e
+0002cf20: 6e74 6972 6520 6060 7669 6465 6f5f 7061  ntire ``video_pa
+0002cf30: 7468 6060 2076 6964 656f 2c20 7061 7373  th`` video, pass
+0002cf40: 2060 6062 675f 7669 6465 6f5f 7061 7468   ``bg_video_path
+0002cf50: 6060 2061 7320 6120 7061 7468 2074 6f20  `` as a path to 
+0002cf60: 6120 7669 6465 6f20 7265 636f 7264 696e  a video recordin
+0002cf70: 6720 7468 6520 6172 656e 6120 7769 7468  g the arena with
+0002cf80: 6f75 7420 7468 6520 616e 696d 616c 732e  out the animals.
+0002cf90: 0a0a 2020 2020 3a70 6172 616d 2055 6e69  ..    :param Uni
+0002cfa0: 6f6e 5b73 7472 2c20 6f73 2e50 6174 684c  on[str, os.PathL
+0002cfb0: 696b 655d 2076 6964 656f 5f70 6174 683a  ike] video_path:
+0002cfc0: 2054 6865 2070 6174 6820 746f 2074 6865   The path to the
+0002cfd0: 2076 6964 656f 2074 6f20 7265 6d6f 7665   video to remove
+0002cfe0: 2074 6865 2062 6163 6b67 726f 756e 6420   the background 
+0002cff0: 6672 6f6d 2e0a 2020 2020 3a70 6172 616d  from..    :param
+0002d000: 204f 7074 696f 6e61 6c5b 556e 696f 6e5b   Optional[Union[
+0002d010: 7374 722c 206f 732e 5061 7468 4c69 6b65  str, os.PathLike
+0002d020: 5d5d 2062 675f 7669 6465 6f5f 7061 7468  ]] bg_video_path
+0002d030: 3a20 5061 7468 2074 6f20 7468 6520 7669  : Path to the vi
+0002d040: 6465 6f20 7768 6963 6820 636f 6e74 6169  deo which contai
+0002d050: 6e73 2061 2073 6567 6d65 6e74 2077 6974  ns a segment wit
+0002d060: 6820 7468 6520 6261 636b 6772 6f75 6e64  h the background
+0002d070: 206f 6e6c 792e 2049 6620 4e6f 6e65 2c20   only. If None, 
+0002d080: 7468 656e 2060 6076 6964 656f 5f70 6174  then ``video_pat
+0002d090: 6860 6020 7769 6c6c 2062 6520 7573 6564  h`` will be used
+0002d0a0: 2e0a 2020 2020 3a70 6172 616d 204f 7074  ..    :param Opt
+0002d0b0: 696f 6e61 6c5b 696e 745d 2062 675f 7374  ional[int] bg_st
+0002d0c0: 6172 745f 6672 6d3a 2054 6865 2066 6972  art_frm: The fir
+0002d0d0: 7374 2066 7261 6d65 2069 6e20 7468 6520  st frame in the 
+0002d0e0: 6261 636b 6772 6f75 6e64 2076 6964 656f  background video
+0002d0f0: 2074 6f20 7573 6520 7768 656e 2063 7265   to use when cre
+0002d100: 6174 696e 6720 6120 7265 7072 6573 656e  ating a represen
+0002d110: 7461 7469 7665 2062 6163 6b67 726f 756e  tative backgroun
+0002d120: 6420 696d 6167 652e 2044 6566 6175 6c74  d image. Default
+0002d130: 3a20 4e6f 6e65 2e0a 2020 2020 3a70 6172  : None..    :par
+0002d140: 616d 204f 7074 696f 6e61 6c5b 696e 745d  am Optional[int]
+0002d150: 2062 675f 656e 645f 6672 6d3a 2054 6865   bg_end_frm: The
+0002d160: 206c 6173 7420 6672 616d 6520 696e 2074   last frame in t
+0002d170: 6865 2062 6163 6b67 726f 756e 6420 7669  he background vi
+0002d180: 6465 6f20 746f 2075 7365 2077 6865 6e20  deo to use when 
+0002d190: 6372 6561 7469 6e67 2061 2072 6570 7265  creating a repre
+0002d1a0: 7365 6e74 6174 6976 6520 6261 636b 6772  sentative backgr
+0002d1b0: 6f75 6e64 2069 6d61 6765 2e20 4465 6661  ound image. Defa
+0002d1c0: 756c 743a 204e 6f6e 652e 0a20 2020 203a  ult: None..    :
+0002d1d0: 7061 7261 6d20 4f70 7469 6f6e 616c 5b73  param Optional[s
+0002d1e0: 7472 5d20 6267 5f73 7461 7274 5f74 696d  tr] bg_start_tim
+0002d1f0: 653a 2054 6865 2073 7461 7274 2074 696d  e: The start tim
+0002d200: 6573 7461 6d70 2069 6e20 6048 483a 4d4d  estamp in `HH:MM
+0002d210: 3a53 5360 2066 6f72 6d61 7420 696e 2074  :SS` format in t
+0002d220: 6865 2062 6163 6b67 726f 756e 6420 7669  he background vi
+0002d230: 6465 6f20 746f 2075 7365 2074 6f20 6372  deo to use to cr
+0002d240: 6561 7465 2061 2072 6570 7265 7365 6e74  eate a represent
+0002d250: 6174 6976 6520 6261 636b 6772 6f75 6e64  ative background
+0002d260: 2069 6d61 6765 2e20 4465 6661 756c 743a   image. Default:
+0002d270: 204e 6f6e 652e 0a20 2020 203a 7061 7261   None..    :para
+0002d280: 6d20 4f70 7469 6f6e 616c 5b73 7472 5d20  m Optional[str] 
+0002d290: 6267 5f65 6e64 5f74 696d 653a 2054 6865  bg_end_time: The
+0002d2a0: 2065 6e64 2074 696d 6573 7461 6d70 2069   end timestamp i
+0002d2b0: 6e20 6048 483a 4d4d 3a53 5360 2066 6f72  n `HH:MM:SS` for
+0002d2c0: 6d61 7420 696e 2074 6865 2062 6163 6b67  mat in the backg
+0002d2d0: 726f 756e 6420 7669 6465 6f20 746f 2075  round video to u
+0002d2e0: 7365 2074 6f20 6372 6561 7465 2061 2072  se to create a r
+0002d2f0: 6570 7265 7365 6e74 6174 6976 6520 6261  epresentative ba
+0002d300: 636b 6772 6f75 6e64 2069 6d61 6765 2e20  ckground image. 
+0002d310: 4465 6661 756c 743a 204e 6f6e 652e 0a20  Default: None.. 
+0002d320: 2020 203a 7061 7261 6d20 4f70 7469 6f6e     :param Option
+0002d330: 616c 5b54 7570 6c65 5b69 6e74 2c20 696e  al[Tuple[int, in
+0002d340: 742c 2069 6e74 5d5d 2062 675f 636f 6c6f  t, int]] bg_colo
+0002d350: 723a 2054 6865 2052 4742 2063 6f6c 6f72  r: The RGB color
+0002d360: 206f 6620 7468 6520 6d6f 7669 6e67 206f   of the moving o
+0002d370: 626a 6563 7473 2069 6e20 7468 6520 6f75  bjects in the ou
+0002d380: 7470 7574 2076 6964 656f 2e20 4465 6661  tput video. Defa
+0002d390: 756c 7473 2074 6f20 4e6f 6e65 2c20 7768  ults to None, wh
+0002d3a0: 6963 6820 7265 7072 6573 656e 7473 2074  ich represents t
+0002d3b0: 6865 206f 7269 6769 6e61 6c20 636f 6c6f  he original colo
+0002d3c0: 7273 206f 6620 7468 6520 6d6f 7669 6e67  rs of the moving
+0002d3d0: 206f 626a 6563 7473 2e0a 2020 2020 3a70   objects..    :p
+0002d3e0: 6172 616d 204f 7074 696f 6e61 6c5b 5475  aram Optional[Tu
+0002d3f0: 706c 655b 696e 742c 2069 6e74 2c20 696e  ple[int, int, in
+0002d400: 745d 5d20 6667 5f63 6f6c 6f72 3a20 5468  t]] fg_color: Th
+0002d410: 6520 5247 4220 636f 6c6f 7220 6f66 2074  e RGB color of t
+0002d420: 6865 2062 6163 6b67 726f 756e 6420 6f75  he background ou
+0002d430: 7470 7574 2076 6964 656f 2e20 4465 6661  tput video. Defa
+0002d440: 756c 7473 2074 6f20 626c 6163 6b20 2830  ults to black (0
+0002d450: 2c20 302c 2030 292e 0a20 2020 203a 7061  , 0, 0)..    :pa
+0002d460: 7261 6d20 4f70 7469 6f6e 616c 5b55 6e69  ram Optional[Uni
+0002d470: 6f6e 5b73 7472 2c20 6f73 2e50 6174 684c  on[str, os.PathL
+0002d480: 696b 655d 5d20 7361 7665 5f70 6174 683a  ike]] save_path:
+0002d490: 2054 6865 2070 6174 6368 2074 6f20 7768   The patch to wh
+0002d4a0: 6572 6520 746f 2073 6176 6520 7468 6520  ere to save the 
+0002d4b0: 6f75 7470 7574 2076 6964 656f 2077 6865  output video whe
+0002d4c0: 7265 2074 6865 2062 6163 6b67 726f 756e  re the backgroun
+0002d4d0: 6420 6973 2072 656d 6f76 6564 2e20 4966  d is removed. If
+0002d4e0: 204e 6f6e 652c 2073 6176 6573 2074 6865   None, saves the
+0002d4f0: 206f 7574 7075 7420 7669 6465 6f20 696e   output video in
+0002d500: 2074 6865 2073 616d 6520 6469 7265 6374   the same direct
+0002d510: 6f72 7920 6173 2074 6865 2069 6e70 7574  ory as the input
+0002d520: 2076 6964 656f 2077 6974 6820 7468 6520   video with the 
+0002d530: 6060 5f62 675f 7375 6274 7261 6374 6564  ``_bg_subtracted
+0002d540: 6060 2073 7566 6669 782e 2044 6566 6175  `` suffix. Defau
+0002d550: 6c74 3a20 4e6f 6e65 2e0a 2020 2020 3a70  lt: None..    :p
+0002d560: 6172 616d 204f 7074 696f 6e61 6c5b 696e  aram Optional[in
+0002d570: 745d 2063 6f72 655f 636e 743a 2054 6865  t] core_cnt: The
+0002d580: 206e 756d 6265 7220 6f66 2063 6f72 6573   number of cores
+0002d590: 2074 6f20 7573 652e 2044 6566 6175 6c74   to use. Default
+0002d5a0: 7320 746f 202d 3120 7265 7072 6573 656e  s to -1 represen
+0002d5b0: 7469 6e67 2061 6c6c 2061 7661 696c 6162  ting all availab
+0002d5c0: 6c65 2063 6f72 6573 2e0a 2020 2020 3a72  le cores..    :r
+0002d5d0: 6574 7572 6e3a 204e 6f6e 652e 0a0a 2020  eturn: None...  
+0002d5e0: 2020 3a65 7861 6d70 6c65 3a0a 2020 2020    :example:.    
+0002d5f0: 3e3e 3e20 7669 6465 6f5f 6267 5f73 7562  >>> video_bg_sub
+0002d600: 7374 7261 6374 696f 6e5f 6d70 2876 6964  straction_mp(vid
+0002d610: 656f 5f70 6174 683d 272f 5573 6572 732f  eo_path='/Users/
+0002d620: 7369 6d6f 6e2f 446f 776e 6c6f 6164 732f  simon/Downloads/
+0002d630: 315f 4c48 2e6d 7034 272c 2062 675f 7374  1_LH.mp4', bg_st
+0002d640: 6172 745f 7469 6d65 3d27 3030 3a30 303a  art_time='00:00:
+0002d650: 3030 272c 2062 675f 656e 645f 7469 6d65  00', bg_end_time
+0002d660: 3d27 3030 3a30 303a 3130 272c 2062 675f  ='00:00:10', bg_
+0002d670: 636f 6c6f 723d 2830 2c20 302c 2030 292c  color=(0, 0, 0),
+0002d680: 2066 675f 636f 6c6f 723d 2832 3535 2c20   fg_color=(255, 
+0002d690: 3235 352c 2032 3535 2929 0a20 2020 2022  255, 255)).    "
+0002d6a0: 2222 0a0a 2020 2020 7469 6d65 7220 3d20  ""..    timer = 
+0002d6b0: 5369 6d62 6154 696d 6572 2873 7461 7274  SimbaTimer(start
+0002d6c0: 3d54 7275 6529 0a20 2020 2063 6865 636b  =True).    check
+0002d6d0: 5f66 696c 655f 6578 6973 745f 616e 645f  _file_exist_and_
+0002d6e0: 7265 6164 6162 6c65 2866 696c 655f 7061  readable(file_pa
+0002d6f0: 7468 3d76 6964 656f 5f70 6174 6829 0a20  th=video_path). 
+0002d700: 2020 2069 6620 6267 5f76 6964 656f 5f70     if bg_video_p
+0002d710: 6174 6820 6973 204e 6f6e 653a 0a20 2020  ath is None:.   
+0002d720: 2020 2020 2062 675f 7669 6465 6f5f 7061       bg_video_pa
+0002d730: 7468 203d 2064 6565 7063 6f70 7928 7669  th = deepcopy(vi
+0002d740: 6465 6f5f 7061 7468 290a 2020 2020 7669  deo_path).    vi
+0002d750: 6465 6f5f 6d65 7461 5f64 6174 6120 3d20  deo_meta_data = 
+0002d760: 6765 745f 7669 6465 6f5f 6d65 7461 5f64  get_video_meta_d
+0002d770: 6174 6128 7669 6465 6f5f 7061 7468 3d76  ata(video_path=v
+0002d780: 6964 656f 5f70 6174 6829 0a20 2020 2064  ideo_path).    d
+0002d790: 6972 2c20 7669 6465 6f5f 6e61 6d65 2c20  ir, video_name, 
+0002d7a0: 6578 7420 3d20 6765 745f 666e 5f65 7874  ext = get_fn_ext
+0002d7b0: 2866 696c 6570 6174 683d 7669 6465 6f5f  (filepath=video_
+0002d7c0: 7061 7468 290a 2020 2020 6966 2073 6176  path).    if sav
+0002d7d0: 655f 7061 7468 2069 7320 4e6f 6e65 3a0a  e_path is None:.
+0002d7e0: 2020 2020 2020 2020 7361 7665 5f70 6174          save_pat
+0002d7f0: 6820 3d20 6f73 2e70 6174 682e 6a6f 696e  h = os.path.join
+0002d800: 2864 6972 2c20 6627 7b76 6964 656f 5f6e  (dir, f'{video_n
+0002d810: 616d 657d 5f62 675f 7375 6274 7261 6374  ame}_bg_subtract
+0002d820: 6564 7b65 7874 7d27 290a 2020 2020 6474  ed{ext}').    dt
+0002d830: 203d 2064 6174 6574 696d 652e 6e6f 7728   = datetime.now(
+0002d840: 292e 7374 7266 7469 6d65 2822 2559 256d  ).strftime("%Y%m
+0002d850: 2564 2548 254d 2553 2229 0a20 2020 2074  %d%H%M%S").    t
+0002d860: 656d 705f 6469 7220 3d20 6f73 2e70 6174  emp_dir = os.pat
+0002d870: 682e 6a6f 696e 2864 6972 2c20 6627 7465  h.join(dir, f'te
+0002d880: 6d70 5f7b 7669 6465 6f5f 6e61 6d65 7d5f  mp_{video_name}_
+0002d890: 7b64 747d 2729 0a20 2020 206f 732e 6d61  {dt}').    os.ma
+0002d8a0: 6b65 6469 7273 2874 656d 705f 6469 7229  kedirs(temp_dir)
+0002d8b0: 0a20 2020 2063 6865 636b 5f69 6e74 286e  .    check_int(n
+0002d8c0: 616d 653d 6627 7b76 6964 656f 5f62 675f  ame=f'{video_bg_
+0002d8d0: 7375 6273 7472 6163 7469 6f6e 5f6d 702e  substraction_mp.
+0002d8e0: 5f5f 6e61 6d65 5f5f 7d20 636f 7265 5f63  __name__} core_c
+0002d8f0: 6e74 272c 2076 616c 7565 3d63 6f72 655f  nt', value=core_
+0002d900: 636e 742c 206d 696e 5f76 616c 7565 3d2d  cnt, min_value=-
+0002d910: 312c 206d 6178 5f76 616c 7565 3d66 696e  1, max_value=fin
+0002d920: 645f 636f 7265 5f63 6e74 2829 5b30 5d29  d_core_cnt()[0])
+0002d930: 0a20 2020 2069 6620 636f 7265 5f63 6e74  .    if core_cnt
+0002d940: 203d 3d20 2d31 3a20 636f 7265 5f63 6e74   == -1: core_cnt
+0002d950: 203d 2066 696e 645f 636f 7265 5f63 6e74   = find_core_cnt
+0002d960: 2829 5b30 5d0a 2020 2020 6267 5f66 726d  ()[0].    bg_frm
+0002d970: 203d 2063 7265 6174 655f 6176 6572 6167   = create_averag
+0002d980: 655f 6672 6d28 7669 6465 6f5f 7061 7468  e_frm(video_path
+0002d990: 3d62 675f 7669 6465 6f5f 7061 7468 2c20  =bg_video_path, 
+0002d9a0: 7374 6172 745f 6672 6d3d 6267 5f73 7461  start_frm=bg_sta
+0002d9b0: 7274 5f66 726d 2c20 656e 645f 6672 6d3d  rt_frm, end_frm=
+0002d9c0: 6267 5f65 6e64 5f66 726d 2c20 7374 6172  bg_end_frm, star
+0002d9d0: 745f 7469 6d65 3d62 675f 7374 6172 745f  t_time=bg_start_
+0002d9e0: 7469 6d65 2c20 656e 645f 7469 6d65 3d62  time, end_time=b
+0002d9f0: 675f 656e 645f 7469 6d65 290a 2020 2020  g_end_time).    
+0002da00: 6267 5f66 726d 203d 2063 7632 2e72 6573  bg_frm = cv2.res
+0002da10: 697a 6528 6267 5f66 726d 2c20 2876 6964  ize(bg_frm, (vid
+0002da20: 656f 5f6d 6574 615f 6461 7461 5b27 7769  eo_meta_data['wi
+0002da30: 6474 6827 5d2c 2076 6964 656f 5f6d 6574  dth'], video_met
+0002da40: 615f 6461 7461 5b27 6865 6967 6874 275d  a_data['height']
+0002da50: 2929 0a20 2020 2062 675f 6672 6d20 3d20  )).    bg_frm = 
+0002da60: 6267 5f66 726d 5b3a 2c20 3a2c 203a 3a2d  bg_frm[:, :, ::-
+0002da70: 315d 0a20 2020 2066 726d 5f6c 6973 7420  1].    frm_list 
+0002da80: 3d20 6e70 2e61 7272 6179 5f73 706c 6974  = np.array_split
+0002da90: 286c 6973 7428 7261 6e67 6528 302c 2076  (list(range(0, v
+0002daa0: 6964 656f 5f6d 6574 615f 6461 7461 5b27  ideo_meta_data['
+0002dab0: 6672 616d 655f 636f 756e 7427 5d29 292c  frame_count'])),
+0002dac0: 2063 6f72 655f 636e 7429 0a20 2020 2066   core_cnt).    f
+0002dad0: 726d 5f64 6174 6120 3d20 5b5d 0a20 2020  rm_data = [].   
+0002dae0: 2066 6f72 2063 2c20 6920 696e 2065 6e75   for c, i in enu
+0002daf0: 6d65 7261 7465 2866 726d 5f6c 6973 7429  merate(frm_list)
+0002db00: 3a0a 2020 2020 2020 2020 6672 6d5f 6461  :.        frm_da
+0002db10: 7461 2e61 7070 656e 6428 2863 2c20 6929  ta.append((c, i)
+0002db20: 290a 2020 2020 7769 7468 206d 756c 7469  ).    with multi
+0002db30: 7072 6f63 6573 7369 6e67 2e50 6f6f 6c28  processing.Pool(
+0002db40: 636f 7265 5f63 6e74 2c20 6d61 7874 6173  core_cnt, maxtas
+0002db50: 6b73 7065 7263 6869 6c64 3d39 3030 3029  ksperchild=9000)
+0002db60: 2061 7320 706f 6f6c 3a0a 2020 2020 2020   as pool:.      
+0002db70: 2020 636f 6e73 7461 6e74 7320 3d20 6675    constants = fu
+0002db80: 6e63 746f 6f6c 732e 7061 7274 6961 6c28  nctools.partial(
+0002db90: 5f62 675f 7265 6d6f 7665 725f 6d70 2c0a  _bg_remover_mp,.
+0002dba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0002dbb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002dbc0: 2020 2020 2020 2020 2020 2020 2062 675f               bg_
-0002dbd0: 6672 6d3d 6267 5f66 726d 2c0a 2020 2020  frm=bg_frm,.    
+0002dbc0: 2020 2020 2020 7669 6465 6f5f 7061 7468        video_path
+0002dbd0: 3d76 6964 656f 5f70 6174 682c 0a20 2020  =video_path,.   
 0002dbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0002dbf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002dc00: 2020 6267 5f63 6c72 3d62 675f 636f 6c6f    bg_clr=bg_colo
-0002dc10: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
+0002dc00: 2020 2062 675f 6672 6d3d 6267 5f66 726d     bg_frm=bg_frm
+0002dc10: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
 0002dc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002dc30: 2020 2020 2020 2020 2066 675f 636c 723d           fg_clr=
-0002dc40: 6667 5f63 6f6c 6f72 2c0a 2020 2020 2020  fg_color,.      
+0002dc30: 2020 2020 2020 2020 6267 5f63 6c72 3d62          bg_clr=b
+0002dc40: 675f 636f 6c6f 722c 0a20 2020 2020 2020  g_color,.       
 0002dc50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002dc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002dc70: 7669 6465 6f5f 6d65 7461 5f64 6174 613d  video_meta_data=
-0002dc80: 7669 6465 6f5f 6d65 7461 5f64 6174 612c  video_meta_data,
-0002dc90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002dca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002dcb0: 2020 2020 2020 2074 656d 705f 6469 723d         temp_dir=
-0002dcc0: 7465 6d70 5f64 6972 290a 2020 2020 2020  temp_dir).      
-0002dcd0: 2020 666f 7220 636e 742c 2072 6573 756c    for cnt, resul
-0002dce0: 7420 696e 2065 6e75 6d65 7261 7465 2870  t in enumerate(p
-0002dcf0: 6f6f 6c2e 696d 6170 2863 6f6e 7374 616e  ool.imap(constan
-0002dd00: 7473 2c20 6672 6d5f 6461 7461 2c20 6368  ts, frm_data, ch
-0002dd10: 756e 6b73 697a 653d 3129 293a 0a20 2020  unksize=1)):.   
-0002dd20: 2020 2020 2020 2020 2070 7269 6e74 2866           print(f
-0002dd30: 2746 7261 6d65 2062 6174 6368 207b 7265  'Frame batch {re
-0002dd40: 7375 6c74 2b31 7d20 636f 6d70 6c65 7465  sult+1} complete
-0002dd50: 642e 2e2e 2729 0a20 2020 2020 2020 2070  d...').        p
-0002dd60: 6f6f 6c2e 7465 726d 696e 6174 6528 290a  ool.terminate().
-0002dd70: 2020 2020 2020 2020 706f 6f6c 2e6a 6f69          pool.joi
-0002dd80: 6e28 290a 0a20 2020 2070 7269 6e74 2866  n()..    print(f
-0002dd90: 224a 6f69 6e69 6e67 207b 7669 6465 6f5f  "Joining {video_
-0002dda0: 6e61 6d65 7d20 6d75 6c74 6970 726f 6365  name} multiproce
-0002ddb0: 7373 6564 2076 6964 656f 2e2e 2e22 290a  ssed video...").
-0002ddc0: 2020 2020 636f 6e63 6174 656e 6174 655f      concatenate_
-0002ddd0: 7669 6465 6f73 5f69 6e5f 666f 6c64 6572  videos_in_folder
-0002dde0: 2869 6e5f 666f 6c64 6572 3d74 656d 705f  (in_folder=temp_
-0002ddf0: 6469 722c 2073 6176 655f 7061 7468 3d73  dir, save_path=s
-0002de00: 6176 655f 7061 7468 2c20 7669 6465 6f5f  ave_path, video_
-0002de10: 666f 726d 6174 3d65 7874 5b31 3a5d 2c20  format=ext[1:], 
-0002de20: 7265 6d6f 7665 5f73 706c 6974 733d 5472  remove_splits=Tr
-0002de30: 7565 290a 2020 2020 7469 6d65 722e 7374  ue).    timer.st
-0002de40: 6f70 5f74 696d 6572 2829 0a20 2020 2073  op_timer().    s
-0002de50: 7464 6f75 745f 7375 6363 6573 7328 6d73  tdout_success(ms
-0002de60: 673d 6627 5669 6465 6f20 7361 7665 6420  g=f'Video saved 
-0002de70: 6174 207b 7361 7665 5f70 6174 687d 272c  at {save_path}',
-0002de80: 2065 6c61 7073 6564 5f74 696d 653d 7469   elapsed_time=ti
-0002de90: 6d65 722e 656c 6170 7365 645f 7469 6d65  mer.elapsed_time
-0002dea0: 5f73 7472 290a 0a0a 0a0a 2320 7669 6465  _str).....# vide
-0002deb0: 6f5f 7061 7468 7320 3d20 5b27 2f55 7365  o_paths = ['/Use
-0002dec0: 7273 2f73 696d 6f6e 2f44 6573 6b74 6f70  rs/simon/Desktop
-0002ded0: 2f65 6e76 732f 7369 6d62 612f 7472 6f75  /envs/simba/trou
-0002dee0: 626c 6573 686f 6f74 696e 672f 6265 6570  bleshooting/beep
-0002def0: 626f 6f70 3137 342f 7072 6f6a 6563 745f  boop174/project_
-0002df00: 666f 6c64 6572 2f6d 6572 6765 2f54 7269  folder/merge/Tri
-0002df10: 616c 2020 2020 3130 5f63 6c69 7070 6564  al    10_clipped
-0002df20: 5f67 616e 7474 2e6d 7034 272c 0a23 2020  _gantt.mp4',.#  
-0002df30: 2020 2020 2020 2020 2020 2020 2020 272f                '/
-0002df40: 5573 6572 732f 7369 6d6f 6e2f 4465 736b  Users/simon/Desk
-0002df50: 746f 702f 656e 7673 2f73 696d 6261 2f74  top/envs/simba/t
-0002df60: 726f 7562 6c65 7368 6f6f 7469 6e67 2f62  roubleshooting/b
-0002df70: 6565 7062 6f6f 7031 3734 2f70 726f 6a65  eepboop174/proje
-0002df80: 6374 5f66 6f6c 6465 722f 6d65 7267 652f  ct_folder/merge/
-0002df90: 5472 6961 6c20 2020 2031 305f 636c 6970  Trial    10_clip
-0002dfa0: 7065 642e 6d70 3427 2c0a 2320 2020 2020  ped.mp4',.#     
-0002dfb0: 2020 2020 2020 2020 2020 2027 2f55 7365             '/Use
-0002dfc0: 7273 2f73 696d 6f6e 2f44 6573 6b74 6f70  rs/simon/Desktop
-0002dfd0: 2f65 6e76 732f 7369 6d62 612f 7472 6f75  /envs/simba/trou
-0002dfe0: 626c 6573 686f 6f74 696e 672f 6265 6570  bleshooting/beep
-0002dff0: 626f 6f70 3137 342f 7072 6f6a 6563 745f  boop174/project_
-0002e000: 666f 6c64 6572 2f6d 6572 6765 2f54 7269  folder/merge/Tri
-0002e010: 616c 2020 2020 3130 5f63 6c69 7070 6564  al    10_clipped
-0002e020: 5f6c 696e 652e 6d70 3427 2c0a 2320 2020  _line.mp4',.#   
-0002e030: 2020 2020 2020 2020 2020 2020 2027 2f55               '/U
-0002e040: 7365 7273 2f73 696d 6f6e 2f44 6573 6b74  sers/simon/Deskt
-0002e050: 6f70 2f65 6e76 732f 7369 6d62 612f 7472  op/envs/simba/tr
-0002e060: 6f75 626c 6573 686f 6f74 696e 672f 6265  oubleshooting/be
-0002e070: 6570 626f 6f70 3137 342f 7072 6f6a 6563  epboop174/projec
-0002e080: 745f 666f 6c64 6572 2f6d 6572 6765 2f54  t_folder/merge/T
-0002e090: 7269 616c 2020 2020 2033 5f63 6c69 7070  rial     3_clipp
-0002e0a0: 6564 2e6d 7034 275d 0a23 0a23 2076 6964  ed.mp4'].#.# vid
-0002e0b0: 656f 5f70 6174 6873 203d 205b 272f 5573  eo_paths = ['/Us
-0002e0c0: 6572 732f 7369 6d6f 6e2f 4465 736b 746f  ers/simon/Deskto
-0002e0d0: 702f 656e 7673 2f73 696d 6261 2f74 726f  p/envs/simba/tro
-0002e0e0: 7562 6c65 7368 6f6f 7469 6e67 2f62 6565  ubleshooting/bee
-0002e0f0: 7062 6f6f 7031 3734 2f70 726f 6a65 6374  pboop174/project
-0002e100: 5f66 6f6c 6465 722f 7669 6465 6f73 2f54  _folder/videos/T
-0002e110: 7269 616c 2020 2020 3130 2e6d 7034 272c  rial    10.mp4',
-0002e120: 0a23 2020 2020 2020 2020 2020 2020 2020  .#              
-0002e130: 2020 272f 5573 6572 732f 7369 6d6f 6e2f    '/Users/simon/
-0002e140: 4465 736b 746f 702f 656e 7673 2f73 696d  Desktop/envs/sim
-0002e150: 6261 2f74 726f 7562 6c65 7368 6f6f 7469  ba/troubleshooti
-0002e160: 6e67 2f62 6565 7062 6f6f 7031 3734 2f70  ng/beepboop174/p
-0002e170: 726f 6a65 6374 5f66 6f6c 6465 722f 6d65  roject_folder/me
-0002e180: 7267 652f 5472 6961 6c20 2020 2031 305f  rge/Trial    10_
-0002e190: 636c 6970 7065 645f 6761 6e74 742e 6d70  clipped_gantt.mp
-0002e1a0: 3427 2c0a 2320 2020 2020 2020 2020 2020  4',.#           
-0002e1b0: 2020 2020 2027 2f55 7365 7273 2f73 696d       '/Users/sim
-0002e1c0: 6f6e 2f44 6573 6b74 6f70 2f65 6e76 732f  on/Desktop/envs/
-0002e1d0: 7369 6d62 612f 7472 6f75 626c 6573 686f  simba/troublesho
-0002e1e0: 6f74 696e 672f 6265 6570 626f 6f70 3137  oting/beepboop17
-0002e1f0: 342f 7072 6f6a 6563 745f 666f 6c64 6572  4/project_folder
-0002e200: 2f6d 6572 6765 2f54 7269 616c 2020 2020  /merge/Trial    
-0002e210: 3130 5f63 6c69 7070 6564 5f6c 696e 652e  10_clipped_line.
-0002e220: 6d70 3427 2c0a 2320 2020 2020 2020 2020  mp4',.#         
-0002e230: 2020 2020 2020 2027 2f55 7365 7273 2f73         '/Users/s
-0002e240: 696d 6f6e 2f44 6573 6b74 6f70 2f65 6e76  imon/Desktop/env
-0002e250: 732f 7369 6d62 612f 7472 6f75 626c 6573  s/simba/troubles
-0002e260: 686f 6f74 696e 672f 6265 6570 626f 6f70  hooting/beepboop
-0002e270: 3137 342f 7072 6f6a 6563 745f 666f 6c64  174/project_fold
-0002e280: 6572 2f6d 6572 6765 2f54 7269 616c 2020  er/merge/Trial  
-0002e290: 2020 2033 5f63 6c69 7070 6564 2e6d 7034     3_clipped.mp4
-0002e2a0: 275d 0a23 0a23 2073 6176 655f 7061 7468  '].#.# save_path
-0002e2b0: 203d 2027 2f55 7365 7273 2f73 696d 6f6e   = '/Users/simon
-0002e2c0: 2f44 6573 6b74 6f70 2f65 6e76 732f 7369  /Desktop/envs/si
-0002e2d0: 6d62 612f 7472 6f75 626c 6573 686f 6f74  mba/troubleshoot
-0002e2e0: 696e 672f 6265 6570 626f 6f70 3137 342f  ing/beepboop174/
-0002e2f0: 7072 6f6a 6563 745f 666f 6c64 6572 2f6d  project_folder/m
-0002e300: 6572 6765 2f6f 7574 2e6d 7034 270a 0a23  erge/out.mp4'..#
-0002e310: 0a23 2076 6964 656f 5f70 6174 6873 203d  .# video_paths =
-0002e320: 205b 272f 5573 6572 732f 7369 6d6f 6e2f   ['/Users/simon/
-0002e330: 4465 736b 746f 702f 656e 7673 2f73 696d  Desktop/envs/sim
-0002e340: 6261 2f74 726f 7562 6c65 7368 6f6f 7469  ba/troubleshooti
-0002e350: 6e67 2f62 6565 7062 6f6f 7031 3734 2f70  ng/beepboop174/p
-0002e360: 726f 6a65 6374 5f66 6f6c 6465 722f 6672  roject_folder/fr
-0002e370: 616d 6573 2f6f 7574 7075 742f 6761 6e74  ames/output/gant
-0002e380: 745f 706c 6f74 732f 5472 6961 6c20 2020  t_plots/Trial   
-0002e390: 2031 302e 6d70 3427 2c0a 2320 2020 2020   10.mp4',.#     
-0002e3a0: 2020 2020 2020 2020 2020 2027 2f55 7365             '/Use
-0002e3b0: 7273 2f73 696d 6f6e 2f44 6573 6b74 6f70  rs/simon/Desktop
-0002e3c0: 2f65 6e76 732f 7369 6d62 612f 7472 6f75  /envs/simba/trou
-0002e3d0: 626c 6573 686f 6f74 696e 672f 6265 6570  bleshooting/beep
-0002e3e0: 626f 6f70 3137 342f 7072 6f6a 6563 745f  boop174/project_
-0002e3f0: 666f 6c64 6572 2f76 6964 656f 732f 5472  folder/videos/Tr
-0002e400: 6961 6c20 2020 2031 302e 6d70 3427 2c0a  ial    10.mp4',.
-0002e410: 2320 2020 2020 2020 2020 2020 2020 2020  #               
-0002e420: 2027 2f55 7365 7273 2f73 696d 6f6e 2f44   '/Users/simon/D
-0002e430: 6573 6b74 6f70 2f65 6e76 732f 7369 6d62  esktop/envs/simb
-0002e440: 612f 7472 6f75 626c 6573 686f 6f74 696e  a/troubleshootin
-0002e450: 672f 6265 6570 626f 6f70 3137 342f 7072  g/beepboop174/pr
-0002e460: 6f6a 6563 745f 666f 6c64 6572 2f66 7261  oject_folder/fra
-0002e470: 6d65 732f 6f75 7470 7574 2f6c 696e 655f  mes/output/line_
-0002e480: 706c 6f74 2f54 7269 616c 2020 2020 3130  plot/Trial    10
-0002e490: 2e6d 7034 272c 0a23 2020 2020 2020 2020  .mp4',.#        
-0002e4a0: 2020 2020 2020 2020 272f 5573 6572 732f          '/Users/
-0002e4b0: 7369 6d6f 6e2f 4465 736b 746f 702f 656e  simon/Desktop/en
-0002e4c0: 7673 2f73 696d 6261 2f74 726f 7562 6c65  vs/simba/trouble
-0002e4d0: 7368 6f6f 7469 6e67 2f62 6565 7062 6f6f  shooting/beepboo
-0002e4e0: 7031 3734 2f70 726f 6a65 6374 5f66 6f6c  p174/project_fol
-0002e4f0: 6465 722f 6672 616d 6573 2f6f 7574 7075  der/frames/outpu
-0002e500: 742f 6c69 6e65 5f70 6c6f 742f 5472 6961  t/line_plot/Tria
-0002e510: 6c20 2020 2020 332e 6d70 3427 5d0a 2320  l     3.mp4'].# 
-0002e520: 7361 7665 5f70 6174 6820 3d20 272f 5573  save_path = '/Us
-0002e530: 6572 732f 7369 6d6f 6e2f 4465 736b 746f  ers/simon/Deskto
-0002e540: 702f 656e 7673 2f73 696d 6261 2f74 726f  p/envs/simba/tro
-0002e550: 7562 6c65 7368 6f6f 7469 6e67 2f52 4154  ubleshooting/RAT
-0002e560: 5f4e 4f52 2f70 726f 6a65 6374 5f66 6f6c  _NOR/project_fol
-0002e570: 6465 722f 7669 6465 6f73 2f74 6573 742f  der/videos/test/
-0002e580: 6e65 772f 626c 616e 6b5f 7465 7374 2e6d  new/blank_test.m
-0002e590: 7034 270a 0a23 2076 6964 656f 5f70 6174  p4'..# video_pat
-0002e5a0: 6873 203d 205b 272f 5573 6572 732f 7369  hs = ['/Users/si
-0002e5b0: 6d6f 6e2f 4465 736b 746f 702f 656e 7673  mon/Desktop/envs
-0002e5c0: 2f73 696d 6261 2f74 726f 7562 6c65 7368  /simba/troublesh
-0002e5d0: 6f6f 7469 6e67 2f62 6565 7062 6f6f 7031  ooting/beepboop1
-0002e5e0: 3734 2f70 726f 6a65 6374 5f66 6f6c 6465  74/project_folde
-0002e5f0: 722f 7669 6465 6f73 2f54 7269 616c 2020  r/videos/Trial  
-0002e600: 2020 3130 2e6d 7034 272c 0a23 2020 2020    10.mp4',.#    
-0002e610: 2020 2020 2020 2020 2020 2020 272f 5573              '/Us
-0002e620: 6572 732f 7369 6d6f 6e2f 4465 736b 746f  ers/simon/Deskto
-0002e630: 702f 656e 7673 2f73 696d 6261 2f74 726f  p/envs/simba/tro
-0002e640: 7562 6c65 7368 6f6f 7469 6e67 2f62 6565  ubleshooting/bee
-0002e650: 7062 6f6f 7031 3734 2f70 726f 6a65 6374  pboop174/project
-0002e660: 5f66 6f6c 6465 722f 6672 616d 6573 2f6f  _folder/frames/o
-0002e670: 7574 7075 742f 6c69 6e65 5f70 6c6f 742f  utput/line_plot/
-0002e680: 5472 6961 6c20 2020 2031 302e 6d70 3427  Trial    10.mp4'
-0002e690: 2c0a 2320 2020 2020 2020 2020 2020 2020  ,.#             
-0002e6a0: 2020 2027 2f55 7365 7273 2f73 696d 6f6e     '/Users/simon
-0002e6b0: 2f44 6573 6b74 6f70 2f65 6e76 732f 7369  /Desktop/envs/si
-0002e6c0: 6d62 612f 7472 6f75 626c 6573 686f 6f74  mba/troubleshoot
-0002e6d0: 696e 672f 6265 6570 626f 6f70 3137 342f  ing/beepboop174/
-0002e6e0: 7072 6f6a 6563 745f 666f 6c64 6572 2f66  project_folder/f
-0002e6f0: 7261 6d65 732f 6f75 7470 7574 2f6c 696e  rames/output/lin
-0002e700: 655f 706c 6f74 2f54 7269 616c 2020 2020  e_plot/Trial    
-0002e710: 2033 2e6d 7034 275d 0a0a 2320 6d69 7865   3.mp4']..# mixe
-0002e720: 645f 6d6f 7361 6963 5f63 6f6e 6361 7465  d_mosaic_concate
-0002e730: 6e61 746f 7228 7669 6465 6f5f 7061 7468  nator(video_path
-0002e740: 733d 7669 6465 6f5f 7061 7468 732c 2073  s=video_paths, s
-0002e750: 6176 655f 7061 7468 3d73 6176 655f 7061  ave_path=save_pa
-0002e760: 7468 2c20 6770 753d 4661 6c73 652c 2076  th, gpu=False, v
-0002e770: 6572 626f 7365 3d54 7275 6529 0a         erbose=True).
+0002dc60: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0002dc70: 675f 636c 723d 6667 5f63 6f6c 6f72 2c0a  g_clr=fg_color,.
+0002dc80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002dc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002dca0: 2020 2020 2020 7669 6465 6f5f 6d65 7461        video_meta
+0002dcb0: 5f64 6174 613d 7669 6465 6f5f 6d65 7461  _data=video_meta
+0002dcc0: 5f64 6174 612c 0a20 2020 2020 2020 2020  _data,.         
+0002dcd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002dce0: 2020 2020 2020 2020 2020 2020 2074 656d               tem
+0002dcf0: 705f 6469 723d 7465 6d70 5f64 6972 290a  p_dir=temp_dir).
+0002dd00: 2020 2020 2020 2020 666f 7220 636e 742c          for cnt,
+0002dd10: 2072 6573 756c 7420 696e 2065 6e75 6d65   result in enume
+0002dd20: 7261 7465 2870 6f6f 6c2e 696d 6170 2863  rate(pool.imap(c
+0002dd30: 6f6e 7374 616e 7473 2c20 6672 6d5f 6461  onstants, frm_da
+0002dd40: 7461 2c20 6368 756e 6b73 697a 653d 3129  ta, chunksize=1)
+0002dd50: 293a 0a20 2020 2020 2020 2020 2020 2070  ):.            p
+0002dd60: 7269 6e74 2866 2746 7261 6d65 2062 6174  rint(f'Frame bat
+0002dd70: 6368 207b 7265 7375 6c74 2b31 7d20 636f  ch {result+1} co
+0002dd80: 6d70 6c65 7465 642e 2e2e 2729 0a20 2020  mpleted...').   
+0002dd90: 2020 2020 2070 6f6f 6c2e 7465 726d 696e       pool.termin
+0002dda0: 6174 6528 290a 2020 2020 2020 2020 706f  ate().        po
+0002ddb0: 6f6c 2e6a 6f69 6e28 290a 0a20 2020 2070  ol.join()..    p
+0002ddc0: 7269 6e74 2866 224a 6f69 6e69 6e67 207b  rint(f"Joining {
+0002ddd0: 7669 6465 6f5f 6e61 6d65 7d20 6d75 6c74  video_name} mult
+0002dde0: 6970 726f 6365 7373 6564 2076 6964 656f  iprocessed video
+0002ddf0: 2e2e 2e22 290a 2020 2020 636f 6e63 6174  ...").    concat
+0002de00: 656e 6174 655f 7669 6465 6f73 5f69 6e5f  enate_videos_in_
+0002de10: 666f 6c64 6572 2869 6e5f 666f 6c64 6572  folder(in_folder
+0002de20: 3d74 656d 705f 6469 722c 2073 6176 655f  =temp_dir, save_
+0002de30: 7061 7468 3d73 6176 655f 7061 7468 2c20  path=save_path, 
+0002de40: 7669 6465 6f5f 666f 726d 6174 3d65 7874  video_format=ext
+0002de50: 5b31 3a5d 2c20 7265 6d6f 7665 5f73 706c  [1:], remove_spl
+0002de60: 6974 733d 5472 7565 290a 2020 2020 7469  its=True).    ti
+0002de70: 6d65 722e 7374 6f70 5f74 696d 6572 2829  mer.stop_timer()
+0002de80: 0a20 2020 2073 7464 6f75 745f 7375 6363  .    stdout_succ
+0002de90: 6573 7328 6d73 673d 6627 5669 6465 6f20  ess(msg=f'Video 
+0002dea0: 7361 7665 6420 6174 207b 7361 7665 5f70  saved at {save_p
+0002deb0: 6174 687d 272c 2065 6c61 7073 6564 5f74  ath}', elapsed_t
+0002dec0: 696d 653d 7469 6d65 722e 656c 6170 7365  ime=timer.elapse
+0002ded0: 645f 7469 6d65 5f73 7472 290a 0a0a 0a0a  d_time_str).....
+0002dee0: 2320 7669 6465 6f5f 7061 7468 7320 3d20  # video_paths = 
+0002def0: 5b27 2f55 7365 7273 2f73 696d 6f6e 2f44  ['/Users/simon/D
+0002df00: 6573 6b74 6f70 2f65 6e76 732f 7369 6d62  esktop/envs/simb
+0002df10: 612f 7472 6f75 626c 6573 686f 6f74 696e  a/troubleshootin
+0002df20: 672f 6265 6570 626f 6f70 3137 342f 7072  g/beepboop174/pr
+0002df30: 6f6a 6563 745f 666f 6c64 6572 2f6d 6572  oject_folder/mer
+0002df40: 6765 2f54 7269 616c 2020 2020 3130 5f63  ge/Trial    10_c
+0002df50: 6c69 7070 6564 5f67 616e 7474 2e6d 7034  lipped_gantt.mp4
+0002df60: 272c 0a23 2020 2020 2020 2020 2020 2020  ',.#            
+0002df70: 2020 2020 272f 5573 6572 732f 7369 6d6f      '/Users/simo
+0002df80: 6e2f 4465 736b 746f 702f 656e 7673 2f73  n/Desktop/envs/s
+0002df90: 696d 6261 2f74 726f 7562 6c65 7368 6f6f  imba/troubleshoo
+0002dfa0: 7469 6e67 2f62 6565 7062 6f6f 7031 3734  ting/beepboop174
+0002dfb0: 2f70 726f 6a65 6374 5f66 6f6c 6465 722f  /project_folder/
+0002dfc0: 6d65 7267 652f 5472 6961 6c20 2020 2031  merge/Trial    1
+0002dfd0: 305f 636c 6970 7065 642e 6d70 3427 2c0a  0_clipped.mp4',.
+0002dfe0: 2320 2020 2020 2020 2020 2020 2020 2020  #               
+0002dff0: 2027 2f55 7365 7273 2f73 696d 6f6e 2f44   '/Users/simon/D
+0002e000: 6573 6b74 6f70 2f65 6e76 732f 7369 6d62  esktop/envs/simb
+0002e010: 612f 7472 6f75 626c 6573 686f 6f74 696e  a/troubleshootin
+0002e020: 672f 6265 6570 626f 6f70 3137 342f 7072  g/beepboop174/pr
+0002e030: 6f6a 6563 745f 666f 6c64 6572 2f6d 6572  oject_folder/mer
+0002e040: 6765 2f54 7269 616c 2020 2020 3130 5f63  ge/Trial    10_c
+0002e050: 6c69 7070 6564 5f6c 696e 652e 6d70 3427  lipped_line.mp4'
+0002e060: 2c0a 2320 2020 2020 2020 2020 2020 2020  ,.#             
+0002e070: 2020 2027 2f55 7365 7273 2f73 696d 6f6e     '/Users/simon
+0002e080: 2f44 6573 6b74 6f70 2f65 6e76 732f 7369  /Desktop/envs/si
+0002e090: 6d62 612f 7472 6f75 626c 6573 686f 6f74  mba/troubleshoot
+0002e0a0: 696e 672f 6265 6570 626f 6f70 3137 342f  ing/beepboop174/
+0002e0b0: 7072 6f6a 6563 745f 666f 6c64 6572 2f6d  project_folder/m
+0002e0c0: 6572 6765 2f54 7269 616c 2020 2020 2033  erge/Trial     3
+0002e0d0: 5f63 6c69 7070 6564 2e6d 7034 275d 0a23  _clipped.mp4'].#
+0002e0e0: 0a23 2076 6964 656f 5f70 6174 6873 203d  .# video_paths =
+0002e0f0: 205b 272f 5573 6572 732f 7369 6d6f 6e2f   ['/Users/simon/
+0002e100: 4465 736b 746f 702f 656e 7673 2f73 696d  Desktop/envs/sim
+0002e110: 6261 2f74 726f 7562 6c65 7368 6f6f 7469  ba/troubleshooti
+0002e120: 6e67 2f62 6565 7062 6f6f 7031 3734 2f70  ng/beepboop174/p
+0002e130: 726f 6a65 6374 5f66 6f6c 6465 722f 7669  roject_folder/vi
+0002e140: 6465 6f73 2f54 7269 616c 2020 2020 3130  deos/Trial    10
+0002e150: 2e6d 7034 272c 0a23 2020 2020 2020 2020  .mp4',.#        
+0002e160: 2020 2020 2020 2020 272f 5573 6572 732f          '/Users/
+0002e170: 7369 6d6f 6e2f 4465 736b 746f 702f 656e  simon/Desktop/en
+0002e180: 7673 2f73 696d 6261 2f74 726f 7562 6c65  vs/simba/trouble
+0002e190: 7368 6f6f 7469 6e67 2f62 6565 7062 6f6f  shooting/beepboo
+0002e1a0: 7031 3734 2f70 726f 6a65 6374 5f66 6f6c  p174/project_fol
+0002e1b0: 6465 722f 6d65 7267 652f 5472 6961 6c20  der/merge/Trial 
+0002e1c0: 2020 2031 305f 636c 6970 7065 645f 6761     10_clipped_ga
+0002e1d0: 6e74 742e 6d70 3427 2c0a 2320 2020 2020  ntt.mp4',.#     
+0002e1e0: 2020 2020 2020 2020 2020 2027 2f55 7365             '/Use
+0002e1f0: 7273 2f73 696d 6f6e 2f44 6573 6b74 6f70  rs/simon/Desktop
+0002e200: 2f65 6e76 732f 7369 6d62 612f 7472 6f75  /envs/simba/trou
+0002e210: 626c 6573 686f 6f74 696e 672f 6265 6570  bleshooting/beep
+0002e220: 626f 6f70 3137 342f 7072 6f6a 6563 745f  boop174/project_
+0002e230: 666f 6c64 6572 2f6d 6572 6765 2f54 7269  folder/merge/Tri
+0002e240: 616c 2020 2020 3130 5f63 6c69 7070 6564  al    10_clipped
+0002e250: 5f6c 696e 652e 6d70 3427 2c0a 2320 2020  _line.mp4',.#   
+0002e260: 2020 2020 2020 2020 2020 2020 2027 2f55               '/U
+0002e270: 7365 7273 2f73 696d 6f6e 2f44 6573 6b74  sers/simon/Deskt
+0002e280: 6f70 2f65 6e76 732f 7369 6d62 612f 7472  op/envs/simba/tr
+0002e290: 6f75 626c 6573 686f 6f74 696e 672f 6265  oubleshooting/be
+0002e2a0: 6570 626f 6f70 3137 342f 7072 6f6a 6563  epboop174/projec
+0002e2b0: 745f 666f 6c64 6572 2f6d 6572 6765 2f54  t_folder/merge/T
+0002e2c0: 7269 616c 2020 2020 2033 5f63 6c69 7070  rial     3_clipp
+0002e2d0: 6564 2e6d 7034 275d 0a23 0a23 2073 6176  ed.mp4'].#.# sav
+0002e2e0: 655f 7061 7468 203d 2027 2f55 7365 7273  e_path = '/Users
+0002e2f0: 2f73 696d 6f6e 2f44 6573 6b74 6f70 2f65  /simon/Desktop/e
+0002e300: 6e76 732f 7369 6d62 612f 7472 6f75 626c  nvs/simba/troubl
+0002e310: 6573 686f 6f74 696e 672f 6265 6570 626f  eshooting/beepbo
+0002e320: 6f70 3137 342f 7072 6f6a 6563 745f 666f  op174/project_fo
+0002e330: 6c64 6572 2f6d 6572 6765 2f6f 7574 2e6d  lder/merge/out.m
+0002e340: 7034 270a 0a23 0a23 2076 6964 656f 5f70  p4'..#.# video_p
+0002e350: 6174 6873 203d 205b 272f 5573 6572 732f  aths = ['/Users/
+0002e360: 7369 6d6f 6e2f 4465 736b 746f 702f 656e  simon/Desktop/en
+0002e370: 7673 2f73 696d 6261 2f74 726f 7562 6c65  vs/simba/trouble
+0002e380: 7368 6f6f 7469 6e67 2f62 6565 7062 6f6f  shooting/beepboo
+0002e390: 7031 3734 2f70 726f 6a65 6374 5f66 6f6c  p174/project_fol
+0002e3a0: 6465 722f 6672 616d 6573 2f6f 7574 7075  der/frames/outpu
+0002e3b0: 742f 6761 6e74 745f 706c 6f74 732f 5472  t/gantt_plots/Tr
+0002e3c0: 6961 6c20 2020 2031 302e 6d70 3427 2c0a  ial    10.mp4',.
+0002e3d0: 2320 2020 2020 2020 2020 2020 2020 2020  #               
+0002e3e0: 2027 2f55 7365 7273 2f73 696d 6f6e 2f44   '/Users/simon/D
+0002e3f0: 6573 6b74 6f70 2f65 6e76 732f 7369 6d62  esktop/envs/simb
+0002e400: 612f 7472 6f75 626c 6573 686f 6f74 696e  a/troubleshootin
+0002e410: 672f 6265 6570 626f 6f70 3137 342f 7072  g/beepboop174/pr
+0002e420: 6f6a 6563 745f 666f 6c64 6572 2f76 6964  oject_folder/vid
+0002e430: 656f 732f 5472 6961 6c20 2020 2031 302e  eos/Trial    10.
+0002e440: 6d70 3427 2c0a 2320 2020 2020 2020 2020  mp4',.#         
+0002e450: 2020 2020 2020 2027 2f55 7365 7273 2f73         '/Users/s
+0002e460: 696d 6f6e 2f44 6573 6b74 6f70 2f65 6e76  imon/Desktop/env
+0002e470: 732f 7369 6d62 612f 7472 6f75 626c 6573  s/simba/troubles
+0002e480: 686f 6f74 696e 672f 6265 6570 626f 6f70  hooting/beepboop
+0002e490: 3137 342f 7072 6f6a 6563 745f 666f 6c64  174/project_fold
+0002e4a0: 6572 2f66 7261 6d65 732f 6f75 7470 7574  er/frames/output
+0002e4b0: 2f6c 696e 655f 706c 6f74 2f54 7269 616c  /line_plot/Trial
+0002e4c0: 2020 2020 3130 2e6d 7034 272c 0a23 2020      10.mp4',.#  
+0002e4d0: 2020 2020 2020 2020 2020 2020 2020 272f                '/
+0002e4e0: 5573 6572 732f 7369 6d6f 6e2f 4465 736b  Users/simon/Desk
+0002e4f0: 746f 702f 656e 7673 2f73 696d 6261 2f74  top/envs/simba/t
+0002e500: 726f 7562 6c65 7368 6f6f 7469 6e67 2f62  roubleshooting/b
+0002e510: 6565 7062 6f6f 7031 3734 2f70 726f 6a65  eepboop174/proje
+0002e520: 6374 5f66 6f6c 6465 722f 6672 616d 6573  ct_folder/frames
+0002e530: 2f6f 7574 7075 742f 6c69 6e65 5f70 6c6f  /output/line_plo
+0002e540: 742f 5472 6961 6c20 2020 2020 332e 6d70  t/Trial     3.mp
+0002e550: 3427 5d0a 2320 7361 7665 5f70 6174 6820  4'].# save_path 
+0002e560: 3d20 272f 5573 6572 732f 7369 6d6f 6e2f  = '/Users/simon/
+0002e570: 4465 736b 746f 702f 656e 7673 2f73 696d  Desktop/envs/sim
+0002e580: 6261 2f74 726f 7562 6c65 7368 6f6f 7469  ba/troubleshooti
+0002e590: 6e67 2f52 4154 5f4e 4f52 2f70 726f 6a65  ng/RAT_NOR/proje
+0002e5a0: 6374 5f66 6f6c 6465 722f 7669 6465 6f73  ct_folder/videos
+0002e5b0: 2f74 6573 742f 6e65 772f 626c 616e 6b5f  /test/new/blank_
+0002e5c0: 7465 7374 2e6d 7034 270a 0a23 2076 6964  test.mp4'..# vid
+0002e5d0: 656f 5f70 6174 6873 203d 205b 272f 5573  eo_paths = ['/Us
+0002e5e0: 6572 732f 7369 6d6f 6e2f 4465 736b 746f  ers/simon/Deskto
+0002e5f0: 702f 656e 7673 2f73 696d 6261 2f74 726f  p/envs/simba/tro
+0002e600: 7562 6c65 7368 6f6f 7469 6e67 2f62 6565  ubleshooting/bee
+0002e610: 7062 6f6f 7031 3734 2f70 726f 6a65 6374  pboop174/project
+0002e620: 5f66 6f6c 6465 722f 7669 6465 6f73 2f54  _folder/videos/T
+0002e630: 7269 616c 2020 2020 3130 2e6d 7034 272c  rial    10.mp4',
+0002e640: 0a23 2020 2020 2020 2020 2020 2020 2020  .#              
+0002e650: 2020 272f 5573 6572 732f 7369 6d6f 6e2f    '/Users/simon/
+0002e660: 4465 736b 746f 702f 656e 7673 2f73 696d  Desktop/envs/sim
+0002e670: 6261 2f74 726f 7562 6c65 7368 6f6f 7469  ba/troubleshooti
+0002e680: 6e67 2f62 6565 7062 6f6f 7031 3734 2f70  ng/beepboop174/p
+0002e690: 726f 6a65 6374 5f66 6f6c 6465 722f 6672  roject_folder/fr
+0002e6a0: 616d 6573 2f6f 7574 7075 742f 6c69 6e65  ames/output/line
+0002e6b0: 5f70 6c6f 742f 5472 6961 6c20 2020 2031  _plot/Trial    1
+0002e6c0: 302e 6d70 3427 2c0a 2320 2020 2020 2020  0.mp4',.#       
+0002e6d0: 2020 2020 2020 2020 2027 2f55 7365 7273           '/Users
+0002e6e0: 2f73 696d 6f6e 2f44 6573 6b74 6f70 2f65  /simon/Desktop/e
+0002e6f0: 6e76 732f 7369 6d62 612f 7472 6f75 626c  nvs/simba/troubl
+0002e700: 6573 686f 6f74 696e 672f 6265 6570 626f  eshooting/beepbo
+0002e710: 6f70 3137 342f 7072 6f6a 6563 745f 666f  op174/project_fo
+0002e720: 6c64 6572 2f66 7261 6d65 732f 6f75 7470  lder/frames/outp
+0002e730: 7574 2f6c 696e 655f 706c 6f74 2f54 7269  ut/line_plot/Tri
+0002e740: 616c 2020 2020 2033 2e6d 7034 275d 0a0a  al     3.mp4']..
+0002e750: 2320 6d69 7865 645f 6d6f 7361 6963 5f63  # mixed_mosaic_c
+0002e760: 6f6e 6361 7465 6e61 746f 7228 7669 6465  oncatenator(vide
+0002e770: 6f5f 7061 7468 733d 7669 6465 6f5f 7061  o_paths=video_pa
+0002e780: 7468 732c 2073 6176 655f 7061 7468 3d73  ths, save_path=s
+0002e790: 6176 655f 7061 7468 2c20 6770 753d 4661  ave_path, gpu=Fa
+0002e7a0: 6c73 652c 2076 6572 626f 7365 3d54 7275  lse, verbose=Tru
+0002e7b0: 6529 0a                                  e).
```

### Comparing `Simba-UW-tf-dev-1.92.4/simba/video_processors/.DS_Store` & `Simba-UW-tf-dev-1.92.5/simba/video_processors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/video_processors/roi_selector_circle.py` & `Simba-UW-tf-dev-1.92.5/simba/video_processors/roi_selector_circle.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/video_processors/px_to_mm.py` & `Simba-UW-tf-dev-1.92.5/simba/video_processors/px_to_mm.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/video_processors/batch_process_menus.py` & `Simba-UW-tf-dev-1.92.5/simba/video_processors/batch_process_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/video_processors/multi_cropper.py` & `Simba-UW-tf-dev-1.92.5/simba/video_processors/multi_cropper.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/video_processors/extract_frames.py` & `Simba-UW-tf-dev-1.92.5/simba/video_processors/extract_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/video_processors/roi_selector.py` & `Simba-UW-tf-dev-1.92.5/simba/video_processors/roi_selector.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/video_processors/calculate_px_dist.py` & `Simba-UW-tf-dev-1.92.5/simba/video_processors/calculate_px_dist.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/video_processors/brightness_contrast_ui.py` & `Simba-UW-tf-dev-1.92.5/simba/video_processors/brightness_contrast_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/video_processors/roi_selector_polygon.py` & `Simba-UW-tf-dev-1.92.5/simba/video_processors/roi_selector_polygon.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/video_processors/extract_seqframes.py` & `Simba-UW-tf-dev-1.92.5/simba/video_processors/extract_seqframes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/video_processors/batch_process_create_ffmpeg_commands.py` & `Simba-UW-tf-dev-1.92.5/simba/video_processors/batch_process_create_ffmpeg_commands.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/video_processors/clahe_ui.py` & `Simba-UW-tf-dev-1.92.5/simba/video_processors/clahe_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/outlier_tools/outlier_corrector_movement.py` & `Simba-UW-tf-dev-1.92.5/simba/outlier_tools/outlier_corrector_movement.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/outlier_tools/outlier_corrector_location_advanced.py` & `Simba-UW-tf-dev-1.92.5/simba/outlier_tools/outlier_corrector_location_advanced.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/outlier_tools/outlier_corrector_movement_advanced.py` & `Simba-UW-tf-dev-1.92.5/simba/outlier_tools/outlier_corrector_movement_advanced.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/outlier_tools/outlier_corrector_location.py` & `Simba-UW-tf-dev-1.92.5/simba/outlier_tools/outlier_corrector_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/outlier_tools/skip_outlier_correction.py` & `Simba-UW-tf-dev-1.92.5/simba/outlier_tools/skip_outlier_correction.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/SimBA.py` & `Simba-UW-tf-dev-1.92.5/simba/SimBA.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,16 @@
     CropVideoPopUp, DownsampleMultipleVideosPopUp, DownsampleSingleVideoPopUp,
     DownsampleVideoPopUp, ExtractAllFramesPopUp, ExtractAnnotationFramesPopUp,
     ExtractSEQFramesPopUp, ExtractSpecificFramesPopUp,
     GreyscaleSingleVideoPopUp, ImportFrameDirectoryPopUp,
     InitiateClipMultipleVideosByFrameNumbersPopUp,
     InitiateClipMultipleVideosByTimestampsPopUp, InteractiveClahePopUp,
     MergeFrames2VideoPopUp, MultiCropPopUp, MultiShortenPopUp,
-    SuperImposeFrameCountPopUp, VideoRotatorPopUp, VideoTemporalJoinPopUp)
+    SuperImposeFrameCountPopUp, VideoRotatorPopUp, VideoTemporalJoinPopUp,
+    SuperimposeTimerPopUp, SuperimposeWatermarkPopUp, SuperimposeProgressBarPopUp)
 from simba.ui.pop_ups.visualize_pose_in_dir_pop_up import \
     VisualizePoseInFolderPopUp
 from simba.ui.tkinter_functions import DropDownMenu, Entry_Box, FileSelect
 from simba.ui.video_info_ui import VideoInfoTable
 from simba.utils.checks import (check_ffmpeg_available,
                                 check_file_exist_and_readable, check_int)
 from simba.utils.custom_feature_extractor import CustomFeatureExtractor
@@ -1773,26 +1774,22 @@
         video_process_menu.add_command(
             label="Rotate videos",
             compound="left",
             image=self.menu_icons["rotate"]["img"],
             command=VideoRotatorPopUp,
         )
 
-        video_process_menu.add_command(
-            label="Superimpose frame numbers on video",
-            compound="left",
-            image=self.menu_icons["trash"]["img"],
-            command=lambda: SuperImposeFrameCountPopUp(),
-        )
-        video_process_menu.add_command(
-            label="Temporal join videos",
-            compound="left",
-            image=self.menu_icons["stopwatch"]["img"],
-            command=VideoTemporalJoinPopUp,
-        )
+        superimpose_menu = Menu(menu)
+        superimpose_menu.add_command(label="Superimpose frame numbers on videos", command=SuperImposeFrameCountPopUp)
+        superimpose_menu.add_command(label="Superimpose watermark on videos", command=SuperimposeWatermarkPopUp)
+        superimpose_menu.add_command(label="Superimpose timer on videos", command=SuperimposeTimerPopUp)
+        superimpose_menu.add_command(label="Superimpose progress-bar on videos", command=SuperimposeProgressBarPopUp)
+        video_process_menu.add_cascade(label="Superimpose on videos...", compound="left", image=self.menu_icons["superimpose"]["img"], menu=superimpose_menu)
+
+        video_process_menu.add_command(label="Temporal join videos", compound="left", image=self.menu_icons["stopwatch"]["img"], command=VideoTemporalJoinPopUp)
 
         video_process_menu.add_cascade(
             label="Visualize pose-estimation in folder...",
             compound="left",
             image=self.menu_icons["visualize"]["img"],
             command=VisualizePoseInFolderPopUp,
         )
@@ -1935,22 +1932,18 @@
             font=Formats.LABELFRAME_HEADER_FORMAT.value,
             command=lambda: self.clean_txt(),
         )
         clear_txt_btn.pack(side=BOTTOM, fill=X)
         sys.stdout = StdRedirector(self.txt)
 
         if OS.PYTHON_VER.value != "3.6":
-            PythonVersionWarning(
-                msg=f"SimBA is not extensively tested beyond python 3.6. You are using python {OS.PYTHON_VER.value}. If you encounter errors in python>3.6, please report them on GitHub or Gitter and we will fix! (links in the help toolbar)",
-                source=self.__class__.__name__,
-            )
+            PythonVersionWarning(msg=f"SimBA is not extensively tested beyond python 3.6. You are using python {OS.PYTHON_VER.value}. If you encounter errors in python>3.6, please report them on GitHub or Gitter (links in the help toolbar) and we will work together to fix the issues!", source=self.__class__.__name__)
 
         if not check_ffmpeg_available():
-            FFMpegNotFoundWarning(
-                msg='SimBA could not find a FFMPEG installation on computer (as evaluated by "ffmpeg" returning None). SimBA works best with FFMPEG and it is recommended to install it on your computer',
+            FFMpegNotFoundWarning(msg='SimBA could not find a FFMPEG installation on computer (as evaluated by "ffmpeg" returning None). SimBA works best with FFMPEG and it is recommended to install it on your computer',
                 source=self.__class__.__name__,
             )
 
     def restart(self):
         confirm_restart = askyesno(
             title="RESTART", message="Are you sure that you want restart SimBA?"
         )
```

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/unsupervised/model_names.parquet` & `Simba-UW-tf-dev-1.92.5/simba/assets/unsupervised/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/unsupervised/features.csv` & `Simba-UW-tf-dev-1.92.5/simba/assets/unsupervised/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/shap/down_arrow.jpg` & `Simba-UW-tf-dev-1.92.5/simba/assets/shap/down_arrow.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/shap/intruder_shape.jpg` & `Simba-UW-tf-dev-1.92.5/simba/assets/shap/intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/shap/feature_categories/shap_feature_categories.csv` & `Simba-UW-tf-dev-1.92.5/simba/assets/shap/feature_categories/shap_feature_categories.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/shap/resident_shape.jpg` & `Simba-UW-tf-dev-1.92.5/simba/assets/shap/resident_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/shap/resident_intruder_shape.jpg` & `Simba-UW-tf-dev-1.92.5/simba/assets/shap/resident_intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/shap/animal_distances.jpg` & `Simba-UW-tf-dev-1.92.5/simba/assets/shap/animal_distances.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/shap/baseline_scale.jpg` & `Simba-UW-tf-dev-1.92.5/simba/assets/shap/baseline_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/shap/ubuntu.regular.ttf` & `Simba-UW-tf-dev-1.92.5/simba/assets/shap/ubuntu.regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/shap/side_scale.jpg` & `Simba-UW-tf-dev-1.92.5/simba/assets/shap/side_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/shap/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.92.5/simba/assets/shap/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/shap/side_scale_5.jpg` & `Simba-UW-tf-dev-1.92.5/simba/assets/shap/side_scale_5.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/shap/intruder_movement.jpg` & `Simba-UW-tf-dev-1.92.5/simba/assets/shap/intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/shap/resident_movement.jpg` & `Simba-UW-tf-dev-1.92.5/simba/assets/shap/resident_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/shap/color_bar.jpg` & `Simba-UW-tf-dev-1.92.5/simba/assets/shap/color_bar.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/shap/resident_intruder_movement.jpg` & `Simba-UW-tf-dev-1.92.5/simba/assets/shap/resident_intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/.DS_Store` & `Simba-UW-tf-dev-1.92.5/simba/assets/.DS_Store`

 * *Files 2% similar despite different names*

```diff
@@ -252,219 +252,219 @@
 00000fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001000: 0000 0000 0000 0000 0000 0022 0000 0005  ..........."....
 00001010: 0069 0063 006f 006e 0073 6277 7370 626c  .i.c.o.n.sbwspbl
-00001020: 6f62 0000 00b8 6270 6c69 7374 3030 d601  ob....bplist00..
+00001020: 6f62 0000 00b7 6270 6c69 7374 3030 d601  ob....bplist00..
 00001030: 0203 0405 0607 0807 080b 085d 5368 6f77  ...........]Show
 00001040: 5374 6174 7573 4261 725b 5368 6f77 546f  StatusBar[ShowTo
 00001050: 6f6c 6261 725b 5368 6f77 5461 6256 6965  olbar[ShowTabVie
 00001060: 775f 1014 436f 6e74 6169 6e65 7253 686f  w_..ContainerSho
 00001070: 7753 6964 6562 6172 5c57 696e 646f 7742  wSidebar\WindowB
 00001080: 6f75 6e64 735b 5368 6f77 5369 6465 6261  ounds[ShowSideba
-00001090: 7208 0908 095f 1018 7b7b 3236 302c 2033  r...._..{{260, 3
-000010a0: 3239 7d2c 207b 3932 302c 2034 3336 7d7d  29}, {920, 436}}
-000010b0: 0908 1523 2f3b 525f 6b6c 6d6e 6f8a 0000  ...#/;R_klmno...
-000010c0: 0000 0000 0101 0000 0000 0000 000d 0000  ................
-000010d0: 0000 0000 0000 0000 0000 0000 008b 0000  ................
-000010e0: 0005 0069 0063 006f 006e 0073 6c67 3153  ...i.c.o.n.slg1S
-000010f0: 636f 6d70 0000 0000 0009 454e 0000 0005  comp......EN....
-00001100: 0069 0063 006f 006e 0073 6c73 7643 626c  .i.c.o.n.slsvCbl
-00001110: 6f62 0000 0323 6270 6c69 7374 3030 da01  ob...#bplist00..
-00001120: 0203 0405 0607 0809 0a0b 0c0d 1a54 5554  .............TUT
-00001130: 560c 5858 6963 6f6e 5369 7a65 5f10 0f73  V.XXiconSize_..s
-00001140: 686f 7749 636f 6e50 7265 7669 6577 5763  howIconPreviewWc
-00001150: 6f6c 756d 6e73 5f10 1163 616c 6375 6c61  olumns_..calcula
-00001160: 7465 416c 6c53 697a 6573 5f10 0f73 6372  teAllSizes_..scr
-00001170: 6f6c 6c50 6f73 6974 696f 6e59 5874 6578  ollPositionYXtex
-00001180: 7453 697a 655f 100f 7363 726f 6c6c 506f  tSize_..scrollPo
-00001190: 7369 7469 6f6e 585a 736f 7274 436f 6c75  sitionXZsortColu
-000011a0: 6d6e 5f10 1075 7365 5265 6c61 7469 7665  mn_..useRelative
-000011b0: 4461 7465 735f 1012 7669 6577 4f70 7469  Dates_..viewOpti
-000011c0: 6f6e 7356 6572 7369 6f6e 2340 3000 0000  onsVersion#@0...
-000011d0: 0000 0009 ae0e 171c 2125 2a2f 3439 3d42  ........!%*/49=B
-000011e0: 464b 4fd4 0f10 1112 1314 0c0c 5a69 6465  FKO.........Zide
-000011f0: 6e74 6966 6965 7255 7769 6474 6859 6173  ntifierUwidthYas
-00001200: 6365 6e64 696e 6757 7669 7369 626c 6554  cendingWvisibleT
-00001210: 6e61 6d65 1101 2c09 09d4 0f10 1112 1819  name..,.........
-00001220: 1a1a 5875 6269 7175 6974 7910 2308 08d4  ..Xubiquity.#...
-00001230: 0f10 1112 1d1e 1a0c 5c64 6174 654d 6f64  ........\dateMod
-00001240: 6966 6965 6410 b508 09d4 0f10 1112 221e  ified.........".
-00001250: 1a1a 5b64 6174 6543 7265 6174 6564 0808  ..[dateCreated..
-00001260: d40f 1011 1226 271a 0c54 7369 7a65 1061  .....&'..Tsize.a
-00001270: 0809 d40f 1011 122b 2c0c 0c54 6b69 6e64  .......+,..Tkind
-00001280: 1073 0909 d40f 1011 1230 310c 1a55 6c61  .s.......01..Ula
-00001290: 6265 6c10 6409 08d4 0f10 1112 3536 0c1a  bel.d.......56..
-000012a0: 5776 6572 7369 6f6e 104b 0908 d40f 1011  Wversion.K......
-000012b0: 123a 140c 1a58 636f 6d6d 656e 7473 0908  .:...Xcomments..
-000012c0: d40f 1011 123e 3f1a 1a5e 6461 7465 4c61  .....>?..^dateLa
-000012d0: 7374 4f70 656e 6564 10c8 0808 d40f 1011  stOpened........
-000012e0: 1243 1e1a 1a59 6461 7465 4164 6465 6408  .C...YdateAdded.
-000012f0: 08d4 1210 110f 1a48 1a4a 0810 d208 5a73  .......H.J....Zs
-00001300: 6861 7265 4f77 6e65 72d4 1210 110f 1a48  hareOwner......H
-00001310: 1a4e 0808 5f10 0f73 6861 7265 4c61 7374  .N.._..shareLast
-00001320: 4564 6974 6f72 d412 1011 0f1a 481a 5208  Editor......H.R.
-00001330: 085f 1010 696e 7669 7461 7469 6f6e 5374  ._..invitationSt
-00001340: 6174 7573 0823 0000 0000 0000 0000 2340  atus.#........#@
-00001350: 2800 0000 0000 005c 6461 7465 4d6f 6469  (......\dateModi
-00001360: 6669 6564 0910 0100 0800 1d00 2600 3800  fied........&.8.
-00001370: 4000 5400 6600 6f00 8100 8c00 9f00 b400  @.T.f.o.........
-00001380: bd00 be00 cd00 d600 e100 e700 f100 f900  ................
-00001390: fe01 0101 0201 0301 0c01 1501 1701 1801  ................
-000013a0: 1901 2201 2f01 3101 3201 3301 3c01 4801  .."./.1.2.3.<.H.
-000013b0: 4901 4a01 5301 5801 5a01 5b01 5c01 6501  I.J.S.X.Z.[.\.e.
-000013c0: 6a01 6c01 6d01 6e01 7701 7d01 7f01 8001  j.l.m.n.w.}.....
-000013d0: 8101 8a01 9201 9401 9501 9601 9f01 a801  ................
-000013e0: a901 aa01 b301 c201 c401 c501 c601 cf01  ................
-000013f0: d901 da01 db01 e401 e501 e701 e801 f301  ................
-00001400: fc01 fd01 fe02 1002 1902 1a02 1b02 2e02  ................
-00001410: 2f02 3802 4102 4e02 4f00 0000 0000 0002  /.8.A.N.O.......
-00001420: 0100 0000 0000 0000 5900 0000 0000 0000  ........Y.......
-00001430: 0000 0000 0000 0002 5100 0000 0500 6900  ........Q.....i.
-00001440: 6300 6f00 6e00 736c 7376 7062 6c6f 6200  c.o.n.slsvpblob.
-00001450: 0002 9862 706c 6973 7430 30da 0102 0304  ...bplist00.....
-00001460: 0506 0708 090a 0b0c 0d1c 4748 4749 0c37  ..........GHGI.7
-00001470: 5869 636f 6e53 697a 655f 100f 7368 6f77  XiconSize_..show
-00001480: 4963 6f6e 5072 6576 6965 7757 636f 6c75  IconPreviewWcolu
-00001490: 6d6e 735f 1011 6361 6c63 756c 6174 6541  mns_..calculateA
-000014a0: 6c6c 5369 7a65 735f 100f 7363 726f 6c6c  llSizes_..scroll
-000014b0: 506f 7369 7469 6f6e 5958 7465 7874 5369  PositionYXtextSi
-000014c0: 7a65 5f10 0f73 6372 6f6c 6c50 6f73 6974  ze_..scrollPosit
-000014d0: 696f 6e58 5a73 6f72 7443 6f6c 756d 6e5f  ionXZsortColumn_
-000014e0: 1010 7573 6552 656c 6174 6976 6544 6174  ..useRelativeDat
-000014f0: 6573 5f10 1276 6965 774f 7074 696f 6e73  es_..viewOptions
-00001500: 5665 7273 696f 6e23 4030 0000 0000 0000  Version#@0......
-00001510: 09d9 0e0f 1011 1213 1415 1617 2025 2a2f  ............ %*/
-00001520: 3438 3d41 5863 6f6d 6d65 6e74 7355 6c61  48=AXcommentsUla
-00001530: 6265 6c57 7665 7273 696f 6e5b 6461 7465  belWversion[date
-00001540: 4372 6561 7465 6454 7369 7a65 5c64 6174  CreatedTsize\dat
-00001550: 654d 6f64 6966 6965 6454 6b69 6e64 546e  eModifiedTkindTn
-00001560: 616d 655e 6461 7465 4c61 7374 4f70 656e  ame^dateLastOpen
-00001570: 6564 d418 191a 1b1c 1d0c 1f57 7669 7369  ed.........Wvisi
-00001580: 626c 6555 7769 6474 6859 6173 6365 6e64  bleUwidthYascend
-00001590: 696e 6755 696e 6465 7808 1101 2c09 1007  ingUindex...,...
-000015a0: d418 191a 1b1c 220c 2408 1064 0910 05d4  ......".$..d....
-000015b0: 1819 1a1b 1c27 0c29 0810 4b09 1006 d418  .....'.)..K.....
-000015c0: 191a 1b1c 2c1c 2e08 10b5 0810 02d4 1819  ....,...........
-000015d0: 1a1b 0c31 1c33 0910 6108 1003 d418 191a  ...1.3..a.......
-000015e0: 1b0c 2c1c 3709 0810 01d4 1819 1a1b 0c3a  ..,.7..........:
-000015f0: 0c3c 0910 7309 1004 d418 191a 1b0c 1d0c  .<..s...........
-00001600: 4009 0910 00d4 1819 1a1b 1c43 1c45 0810  @..........C.E..
-00001610: c808 1008 0823 0000 0000 0000 0000 2340  .....#........#@
-00001620: 2800 0000 0000 005c 6461 7465 4d6f 6469  (......\dateModi
-00001630: 6669 6564 0900 0800 1d00 2600 3800 4000  fied......&.8.@.
-00001640: 5400 6600 6f00 8100 8c00 9f00 b400 bd00  T.f.o...........
-00001650: be00 d100 da00 e000 e800 f400 f901 0601  ................
-00001660: 0b01 1001 1f01 2801 3001 3601 4001 4601  ......(.0.6.@.F.
-00001670: 4701 4a01 4b01 4d01 5601 5701 5901 5a01  G.J.K.M.V.W.Y.Z.
-00001680: 5c01 6501 6601 6801 6901 6b01 7401 7501  \.e.f.h.i.k.t.u.
-00001690: 7701 7801 7a01 8301 8401 8601 8701 8901  w.x.z...........
-000016a0: 9201 9301 9401 9601 9f01 a001 a201 a301  ................
-000016b0: a501 ae01 af01 b001 b201 bb01 bc01 be01  ................
-000016c0: bf01 c101 c201 cb01 d401 e100 0000 0000  ................
-000016d0: 0002 0100 0000 0000 0000 4b00 0000 0000  ..........K.....
-000016e0: 0000 0000 0000 0000 0001 e200 0000 0500  ................
-000016f0: 6900 6300 6f00 6e00 736d 6f44 4462 6c6f  i.c.o.n.smoDDblo
-00001700: 6200 0000 0838 25f7 6a88 f4c5 4100 0000  b....8%.j...A...
-00001710: 0500 6900 6300 6f00 6e00 736d 6f64 4462  ..i.c.o.n.smodDb
-00001720: 6c6f 6200 0000 0838 25f7 6a88 f4c5 4100  lob....8%.j...A.
-00001730: 0000 0500 6900 6300 6f00 6e00 7370 6831  ....i.c.o.n.sph1
-00001740: 5363 6f6d 7000 0000 0000 0be0 0000 0000  Scomp...........
-00001750: 0500 6900 6300 6f00 6e00 7376 5372 6e6c  ..i.c.o.n.svSrnl
-00001760: 6f6e 6700 0000 0100 0000 0300 6900 6d00  ong.........i.m.
-00001770: 6762 7773 7062 6c6f 6200 0000 b862 706c  gbwspblob....bpl
-00001780: 6973 7430 30d6 0102 0304 0506 0708 0708  ist00...........
-00001790: 0b08 5d53 686f 7753 7461 7475 7342 6172  ..]ShowStatusBar
-000017a0: 5b53 686f 7754 6f6f 6c62 6172 5b53 686f  [ShowToolbar[Sho
-000017b0: 7754 6162 5669 6577 5f10 1443 6f6e 7461  wTabView_..Conta
-000017c0: 696e 6572 5368 6f77 5369 6465 6261 725c  inerShowSidebar\
-000017d0: 5769 6e64 6f77 426f 756e 6473 5b53 686f  WindowBounds[Sho
-000017e0: 7753 6964 6562 6172 0809 0809 5f10 187b  wSidebar...._..{
-000017f0: 7b32 3630 2c20 3332 397d 2c20 7b39 3230  {260, 329}, {920
-00001800: 2c20 3433 367d 7d09 0815 232f 3b52 5f6b  , 436}}...#/;R_k
-00001810: 6c6d 6e6f 8a00 0000 0000 0001 0100 0000  lmno............
-00001820: 0000 0000 0d00 0000 0000 0000 0000 0000  ................
-00001830: 0000 0000 8b00 0000 0300 6900 6d00 676c  ..........i.m.gl
-00001840: 6731 5363 6f6d 7000 0000 0000 19a9 5e00  g1Scomp.......^.
-00001850: 0000 0300 6900 6d00 676d 6f44 4462 6c6f  ....i.m.gmoDDblo
-00001860: 6200 0000 0814 dc41 9f0a bac5 4100 0000  b......A....A...
-00001870: 0300 6900 6d00 676d 6f64 4462 6c6f 6200  ..i.m.gmodDblob.
-00001880: 0000 0814 dc41 9f0a bac5 4100 0000 0300  .....A....A.....
-00001890: 6900 6d00 6770 6831 5363 6f6d 7000 0000  i.m.gph1Scomp...
-000018a0: 0000 19e0 0000 0000 0300 6900 6d00 6776  ..........i.m.gv
-000018b0: 5372 6e6c 6f6e 6700 0000 0100 0000 0700  Srnlong.........
-000018c0: 6c00 6f00 6f00 6b00 7500 7000 7362 7773  l.o.o.k.u.p.sbws
-000018d0: 7062 6c6f 6200 0000 b862 706c 6973 7430  pblob....bplist0
-000018e0: 30d6 0102 0304 0506 0708 0708 0b08 5d53  0.............]S
-000018f0: 686f 7753 7461 7475 7342 6172 5b53 686f  howStatusBar[Sho
-00001900: 7754 6f6f 6c62 6172 5b53 686f 7754 6162  wToolbar[ShowTab
-00001910: 5669 6577 5f10 1443 6f6e 7461 696e 6572  View_..Container
-00001920: 5368 6f77 5369 6465 6261 725c 5769 6e64  ShowSidebar\Wind
-00001930: 6f77 426f 756e 6473 5b53 686f 7753 6964  owBounds[ShowSid
-00001940: 6562 6172 0809 0809 5f10 187b 7b32 3630  ebar...._..{{260
-00001950: 2c20 3332 397d 2c20 7b39 3230 2c20 3433  , 329}, {920, 43
-00001960: 367d 7d09 0815 232f 3b52 5f6b 6c6d 6e6f  6}}...#/;R_klmno
-00001970: 8a00 0000 0000 0001 0100 0000 0000 0000  ................
-00001980: 0d00 0000 0000 0000 0000 0000 0000 0000  ................
-00001990: 8b00 0000 0700 6c00 6f00 6f00 6b00 7500  ......l.o.o.k.u.
-000019a0: 7000 736c 6731 5363 6f6d 7000 0000 0000  p.slg1Scomp.....
-000019b0: 0502 b800 0000 0700 6c00 6f00 6f00 6b00  ........l.o.o.k.
-000019c0: 7500 7000 736d 6f44 4462 6c6f 6200 0000  u.p.smoDDblob...
-000019d0: 083e 3494 a30a bac5 4100 0000 0700 6c00  .>4.....A.....l.
-000019e0: 6f00 6f00 6b00 7500 7000 736d 6f64 4462  o.o.k.u.p.smodDb
-000019f0: 6c6f 6200 0000 083e 3494 a30a bac5 4100  lob....>4.....A.
-00001a00: 0000 0700 6c00 6f00 6f00 6b00 7500 7000  ....l.o.o.k.u.p.
-00001a10: 7370 6831 5363 6f6d 7000 0000 0000 0530  sph1Scomp......0
-00001a20: 0000 0000 0700 6c00 6f00 6f00 6b00 7500  ......l.o.o.k.u.
-00001a30: 7000 7376 5372 6e6c 6f6e 6700 0000 0100  p.svSrnlong.....
-00001a40: 0000 0400 7300 6800 6100 706c 6731 5363  ....s.h.a.plg1Sc
-00001a50: 6f6d 7000 0000 0000 0906 c300 0000 0400  omp.............
-00001a60: 7300 6800 6100 706d 6f44 4462 6c6f 6200  s.h.a.pmoDDblob.
-00001a70: 0000 0886 8aa4 a80a bac5 4100 0000 0400  ..........A.....
-00001a80: 7300 6800 6100 706d 6f64 4462 6c6f 6200  s.h.a.pmodDblob.
-00001a90: 0000 0886 8aa4 a80a bac5 4100 0000 0400  ..........A.....
-00001aa0: 7300 6800 6100 7070 6831 5363 6f6d 7000  s.h.a.pph1Scomp.
-00001ab0: 0000 0000 0990 0000 0000 0300 7300 7400  ............s.t.
-00001ac0: 6c6c 6731 5363 6f6d 7000 0000 0000 537f  llg1Scomp.....S.
-00001ad0: 6700 0000 0300 7300 7400 6c6d 6f44 4462  g.....s.t.lmoDDb
-00001ae0: 6c6f 6200 0000 0839 8bb9 ad0a bac5 4100  lob....9......A.
-00001af0: 0000 0300 7300 7400 6c6d 6f64 4462 6c6f  ....s.t.lmodDblo
-00001b00: 6200 0000 0839 8bb9 ad0a bac5 4100 0000  b....9......A...
-00001b10: 0300 7300 7400 6c70 6831 5363 6f6d 7000  ..s.t.lph1Scomp.
-00001b20: 0000 0000 53a0 0000 0000 0c00 7500 6e00  ....S.......u.n.
-00001b30: 7300 7500 7000 6500 7200 7600 6900 7300  s.u.p.e.r.v.i.s.
-00001b40: 6500 6462 7773 7062 6c6f 6200 0000 b962  e.dbwspblob....b
-00001b50: 706c 6973 7430 30d6 0102 0304 0506 0708  plist00.........
-00001b60: 0708 0b08 5d53 686f 7753 7461 7475 7342  ....]ShowStatusB
-00001b70: 6172 5b53 686f 7754 6f6f 6c62 6172 5b53  ar[ShowToolbar[S
-00001b80: 686f 7754 6162 5669 6577 5f10 1443 6f6e  howTabView_..Con
-00001b90: 7461 696e 6572 5368 6f77 5369 6465 6261  tainerShowSideba
-00001ba0: 725c 5769 6e64 6f77 426f 756e 6473 5b53  r\WindowBounds[S
-00001bb0: 686f 7753 6964 6562 6172 0809 0809 5f10  howSidebar...._.
-00001bc0: 197b 7b32 3630 2c20 3132 387d 2c20 7b31  .{{260, 128}, {1
-00001bd0: 3134 342c 2036 3338 7d7d 0908 1523 2f3b  144, 638}}...#/;
-00001be0: 525f 6b6c 6d6e 6f8b 0000 0000 0000 0101  R_klmno.........
-00001bf0: 0000 0000 0000 000d 0000 0000 0000 0000  ................
-00001c00: 0000 0000 0000 008c 0000 000c 0075 006e  .............u.n
-00001c10: 0073 0075 0070 0065 0072 0076 0069 0073  .s.u.p.e.r.v.i.s
-00001c20: 0065 0064 6c67 3153 636f 6d70 0000 0000  .e.dlg1Scomp....
-00001c30: 0001 e30a 0000 000c 0075 006e 0073 0075  .........u.n.s.u
-00001c40: 0070 0065 0072 0076 0069 0073 0065 0064  .p.e.r.v.i.s.e.d
-00001c50: 6d6f 4444 626c 6f62 0000 0008 b583 0bb0  moDDblob........
-00001c60: 0aba c541 0000 000c 0075 006e 0073 0075  ...A.....u.n.s.u
-00001c70: 0070 0065 0072 0076 0069 0073 0065 0064  .p.e.r.v.i.s.e.d
-00001c80: 6d6f 6444 626c 6f62 0000 0008 b583 0bb0  modDblob........
-00001c90: 0aba c541 0000 000c 0075 006e 0073 0075  ...A.....u.n.s.u
-00001ca0: 0070 0065 0072 0076 0069 0073 0065 0064  .p.e.r.v.i.s.e.d
-00001cb0: 7068 3153 636f 6d70 0000 0000 0001 f000  ph1Scomp........
-00001cc0: 0000 000c 0075 006e 0073 0075 0070 0065  .....u.n.s.u.p.e
-00001cd0: 0072 0076 0069 0073 0065 0064 7653 726e  .r.v.i.s.e.dvSrn
-00001ce0: 6c6f 6e67 0000 0001 0000 0000 0000 0000  long............
+00001090: 7208 0908 095f 1017 7b7b 302c 2031 3236  r...._..{{0, 126
+000010a0: 7d2c 207b 3134 3430 2c20 3633 357d 7d09  }, {1440, 635}}.
+000010b0: 0815 232f 3b52 5f6b 6c6d 6e6f 8900 0000  ..#/;R_klmno....
+000010c0: 0000 0001 0100 0000 0000 0000 0d00 0000  ................
+000010d0: 0000 0000 0000 0000 0000 0000 8a00 0000  ................
+000010e0: 0500 6900 6300 6f00 6e00 736c 6731 5363  ..i.c.o.n.slg1Sc
+000010f0: 6f6d 7000 0000 0000 0945 4e00 0000 0500  omp......EN.....
+00001100: 6900 6300 6f00 6e00 736c 7376 4362 6c6f  i.c.o.n.slsvCblo
+00001110: 6200 0003 2362 706c 6973 7430 30da 0102  b...#bplist00...
+00001120: 0304 0506 0708 090a 0b0c 0d1a 5455 5456  ............TUTV
+00001130: 0c58 5869 636f 6e53 697a 655f 100f 7368  .XXiconSize_..sh
+00001140: 6f77 4963 6f6e 5072 6576 6965 7757 636f  owIconPreviewWco
+00001150: 6c75 6d6e 735f 1011 6361 6c63 756c 6174  lumns_..calculat
+00001160: 6541 6c6c 5369 7a65 735f 100f 7363 726f  eAllSizes_..scro
+00001170: 6c6c 506f 7369 7469 6f6e 5958 7465 7874  llPositionYXtext
+00001180: 5369 7a65 5f10 0f73 6372 6f6c 6c50 6f73  Size_..scrollPos
+00001190: 6974 696f 6e58 5a73 6f72 7443 6f6c 756d  itionXZsortColum
+000011a0: 6e5f 1010 7573 6552 656c 6174 6976 6544  n_..useRelativeD
+000011b0: 6174 6573 5f10 1276 6965 774f 7074 696f  ates_..viewOptio
+000011c0: 6e73 5665 7273 696f 6e23 4030 0000 0000  nsVersion#@0....
+000011d0: 0000 09ae 0e17 1c21 252a 2f34 393d 4246  .......!%*/49=BF
+000011e0: 4b4f d40f 1011 1213 140c 0c5a 6964 656e  KO.........Ziden
+000011f0: 7469 6669 6572 5577 6964 7468 5961 7363  tifierUwidthYasc
+00001200: 656e 6469 6e67 5776 6973 6962 6c65 546e  endingWvisibleTn
+00001210: 616d 6511 012c 0909 d40f 1011 1218 191a  ame..,..........
+00001220: 1a58 7562 6971 7569 7479 1023 0808 d40f  .Xubiquity.#....
+00001230: 1011 121d 1e1a 0c5c 6461 7465 4d6f 6469  .......\dateModi
+00001240: 6669 6564 10b5 0809 d40f 1011 1222 1e1a  fied........."..
+00001250: 1a5b 6461 7465 4372 6561 7465 6408 08d4  .[dateCreated...
+00001260: 0f10 1112 2627 1a0c 5473 697a 6510 6108  ....&'..Tsize.a.
+00001270: 09d4 0f10 1112 2b2c 0c0c 546b 696e 6410  ......+,..Tkind.
+00001280: 7309 09d4 0f10 1112 3031 0c1a 556c 6162  s.......01..Ulab
+00001290: 656c 1064 0908 d40f 1011 1235 360c 1a57  el.d.......56..W
+000012a0: 7665 7273 696f 6e10 4b09 08d4 0f10 1112  version.K.......
+000012b0: 3a14 0c1a 5863 6f6d 6d65 6e74 7309 08d4  :...Xcomments...
+000012c0: 0f10 1112 3e3f 1a1a 5e64 6174 654c 6173  ....>?..^dateLas
+000012d0: 744f 7065 6e65 6410 c808 08d4 0f10 1112  tOpened.........
+000012e0: 431e 1a1a 5964 6174 6541 6464 6564 0808  C...YdateAdded..
+000012f0: d412 1011 0f1a 481a 4a08 10d2 085a 7368  ......H.J....Zsh
+00001300: 6172 654f 776e 6572 d412 1011 0f1a 481a  areOwner......H.
+00001310: 4e08 085f 100f 7368 6172 654c 6173 7445  N.._..shareLastE
+00001320: 6469 746f 72d4 1210 110f 1a48 1a52 0808  ditor......H.R..
+00001330: 5f10 1069 6e76 6974 6174 696f 6e53 7461  _..invitationSta
+00001340: 7475 7308 2300 0000 0000 0000 0023 4028  tus.#........#@(
+00001350: 0000 0000 0000 5c64 6174 654d 6f64 6966  ......\dateModif
+00001360: 6965 6409 1001 0008 001d 0026 0038 0040  ied........&.8.@
+00001370: 0054 0066 006f 0081 008c 009f 00b4 00bd  .T.f.o..........
+00001380: 00be 00cd 00d6 00e1 00e7 00f1 00f9 00fe  ................
+00001390: 0101 0102 0103 010c 0115 0117 0118 0119  ................
+000013a0: 0122 012f 0131 0132 0133 013c 0148 0149  ."./.1.2.3.<.H.I
+000013b0: 014a 0153 0158 015a 015b 015c 0165 016a  .J.S.X.Z.[.\.e.j
+000013c0: 016c 016d 016e 0177 017d 017f 0180 0181  .l.m.n.w.}......
+000013d0: 018a 0192 0194 0195 0196 019f 01a8 01a9  ................
+000013e0: 01aa 01b3 01c2 01c4 01c5 01c6 01cf 01d9  ................
+000013f0: 01da 01db 01e4 01e5 01e7 01e8 01f3 01fc  ................
+00001400: 01fd 01fe 0210 0219 021a 021b 022e 022f  .............../
+00001410: 0238 0241 024e 024f 0000 0000 0000 0201  .8.A.N.O........
+00001420: 0000 0000 0000 0059 0000 0000 0000 0000  .......Y........
+00001430: 0000 0000 0000 0251 0000 0005 0069 0063  .......Q.....i.c
+00001440: 006f 006e 0073 6c73 7670 626c 6f62 0000  .o.n.slsvpblob..
+00001450: 0298 6270 6c69 7374 3030 da01 0203 0405  ..bplist00......
+00001460: 0607 0809 0a0b 0c0d 1c47 4847 490c 3758  .........GHGI.7X
+00001470: 6963 6f6e 5369 7a65 5f10 0f73 686f 7749  iconSize_..showI
+00001480: 636f 6e50 7265 7669 6577 5763 6f6c 756d  conPreviewWcolum
+00001490: 6e73 5f10 1163 616c 6375 6c61 7465 416c  ns_..calculateAl
+000014a0: 6c53 697a 6573 5f10 0f73 6372 6f6c 6c50  lSizes_..scrollP
+000014b0: 6f73 6974 696f 6e59 5874 6578 7453 697a  ositionYXtextSiz
+000014c0: 655f 100f 7363 726f 6c6c 506f 7369 7469  e_..scrollPositi
+000014d0: 6f6e 585a 736f 7274 436f 6c75 6d6e 5f10  onXZsortColumn_.
+000014e0: 1075 7365 5265 6c61 7469 7665 4461 7465  .useRelativeDate
+000014f0: 735f 1012 7669 6577 4f70 7469 6f6e 7356  s_..viewOptionsV
+00001500: 6572 7369 6f6e 2340 3000 0000 0000 0009  ersion#@0.......
+00001510: d90e 0f10 1112 1314 1516 1720 252a 2f34  ........... %*/4
+00001520: 383d 4158 636f 6d6d 656e 7473 556c 6162  8=AXcommentsUlab
+00001530: 656c 5776 6572 7369 6f6e 5b64 6174 6543  elWversion[dateC
+00001540: 7265 6174 6564 5473 697a 655c 6461 7465  reatedTsize\date
+00001550: 4d6f 6469 6669 6564 546b 696e 6454 6e61  ModifiedTkindTna
+00001560: 6d65 5e64 6174 654c 6173 744f 7065 6e65  me^dateLastOpene
+00001570: 64d4 1819 1a1b 1c1d 0c1f 5776 6973 6962  d.........Wvisib
+00001580: 6c65 5577 6964 7468 5961 7363 656e 6469  leUwidthYascendi
+00001590: 6e67 5569 6e64 6578 0811 012c 0910 07d4  ngUindex...,....
+000015a0: 1819 1a1b 1c22 0c24 0810 6409 1005 d418  .....".$..d.....
+000015b0: 191a 1b1c 270c 2908 104b 0910 06d4 1819  ....'.)..K......
+000015c0: 1a1b 1c2c 1c2e 0810 b508 1002 d418 191a  ...,............
+000015d0: 1b0c 311c 3309 1061 0810 03d4 1819 1a1b  ..1.3..a........
+000015e0: 0c2c 1c37 0908 1001 d418 191a 1b0c 3a0c  .,.7..........:.
+000015f0: 3c09 1073 0910 04d4 1819 1a1b 0c1d 0c40  <..s...........@
+00001600: 0909 1000 d418 191a 1b1c 431c 4508 10c8  ..........C.E...
+00001610: 0810 0808 2300 0000 0000 0000 0023 4028  ....#........#@(
+00001620: 0000 0000 0000 5c64 6174 654d 6f64 6966  ......\dateModif
+00001630: 6965 6409 0008 001d 0026 0038 0040 0054  ied......&.8.@.T
+00001640: 0066 006f 0081 008c 009f 00b4 00bd 00be  .f.o............
+00001650: 00d1 00da 00e0 00e8 00f4 00f9 0106 010b  ................
+00001660: 0110 011f 0128 0130 0136 0140 0146 0147  .....(.0.6.@.F.G
+00001670: 014a 014b 014d 0156 0157 0159 015a 015c  .J.K.M.V.W.Y.Z.\
+00001680: 0165 0166 0168 0169 016b 0174 0175 0177  .e.f.h.i.k.t.u.w
+00001690: 0178 017a 0183 0184 0186 0187 0189 0192  .x.z............
+000016a0: 0193 0194 0196 019f 01a0 01a2 01a3 01a5  ................
+000016b0: 01ae 01af 01b0 01b2 01bb 01bc 01be 01bf  ................
+000016c0: 01c1 01c2 01cb 01d4 01e1 0000 0000 0000  ................
+000016d0: 0201 0000 0000 0000 004b 0000 0000 0000  .........K......
+000016e0: 0000 0000 0000 0000 01e2 0000 0005 0069  ...............i
+000016f0: 0063 006f 006e 0073 6d6f 4444 626c 6f62  .c.o.n.smoDDblob
+00001700: 0000 0008 3825 f76a 88f4 c541 0000 0005  ....8%.j...A....
+00001710: 0069 0063 006f 006e 0073 6d6f 6444 626c  .i.c.o.n.smodDbl
+00001720: 6f62 0000 0008 3825 f76a 88f4 c541 0000  ob....8%.j...A..
+00001730: 0005 0069 0063 006f 006e 0073 7068 3153  ...i.c.o.n.sph1S
+00001740: 636f 6d70 0000 0000 000b e000 0000 0005  comp............
+00001750: 0069 0063 006f 006e 0073 7653 726e 6c6f  .i.c.o.n.svSrnlo
+00001760: 6e67 0000 0001 0000 0003 0069 006d 0067  ng.........i.m.g
+00001770: 6277 7370 626c 6f62 0000 00b8 6270 6c69  bwspblob....bpli
+00001780: 7374 3030 d601 0203 0405 0607 0807 080b  st00............
+00001790: 085d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
+000017a0: 5368 6f77 546f 6f6c 6261 725b 5368 6f77  ShowToolbar[Show
+000017b0: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
+000017c0: 6e65 7253 686f 7753 6964 6562 6172 5c57  nerShowSidebar\W
+000017d0: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
+000017e0: 5369 6465 6261 7208 0908 095f 1018 7b7b  Sidebar...._..{{
+000017f0: 3236 302c 2033 3239 7d2c 207b 3932 302c  260, 329}, {920,
+00001800: 2034 3336 7d7d 0908 1523 2f3b 525f 6b6c   436}}...#/;R_kl
+00001810: 6d6e 6f8a 0000 0000 0000 0101 0000 0000  mno.............
+00001820: 0000 000d 0000 0000 0000 0000 0000 0000  ................
+00001830: 0000 008b 0000 0003 0069 006d 0067 6c67  .........i.m.glg
+00001840: 3153 636f 6d70 0000 0000 0019 a95e 0000  1Scomp.......^..
+00001850: 0003 0069 006d 0067 6d6f 4444 626c 6f62  ...i.m.gmoDDblob
+00001860: 0000 0008 14dc 419f 0aba c541 0000 0003  ......A....A....
+00001870: 0069 006d 0067 6d6f 6444 626c 6f62 0000  .i.m.gmodDblob..
+00001880: 0008 14dc 419f 0aba c541 0000 0003 0069  ....A....A.....i
+00001890: 006d 0067 7068 3153 636f 6d70 0000 0000  .m.gph1Scomp....
+000018a0: 0019 e000 0000 0003 0069 006d 0067 7653  .........i.m.gvS
+000018b0: 726e 6c6f 6e67 0000 0001 0000 0007 006c  rnlong.........l
+000018c0: 006f 006f 006b 0075 0070 0073 6277 7370  .o.o.k.u.p.sbwsp
+000018d0: 626c 6f62 0000 00b8 6270 6c69 7374 3030  blob....bplist00
+000018e0: d601 0203 0405 0607 0807 080b 085d 5368  .............]Sh
+000018f0: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
+00001900: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
+00001910: 6965 775f 1014 436f 6e74 6169 6e65 7253  iew_..ContainerS
+00001920: 686f 7753 6964 6562 6172 5c57 696e 646f  howSidebar\Windo
+00001930: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
+00001940: 6261 7208 0908 095f 1018 7b7b 3236 302c  bar...._..{{260,
+00001950: 2033 3239 7d2c 207b 3932 302c 2034 3336   329}, {920, 436
+00001960: 7d7d 0908 1523 2f3b 525f 6b6c 6d6e 6f8a  }}...#/;R_klmno.
+00001970: 0000 0000 0000 0101 0000 0000 0000 000d  ................
+00001980: 0000 0000 0000 0000 0000 0000 0000 008b  ................
+00001990: 0000 0007 006c 006f 006f 006b 0075 0070  .....l.o.o.k.u.p
+000019a0: 0073 6c67 3153 636f 6d70 0000 0000 0005  .slg1Scomp......
+000019b0: 02b8 0000 0007 006c 006f 006f 006b 0075  .......l.o.o.k.u
+000019c0: 0070 0073 6d6f 4444 626c 6f62 0000 0008  .p.smoDDblob....
+000019d0: 3e34 94a3 0aba c541 0000 0007 006c 006f  >4.....A.....l.o
+000019e0: 006f 006b 0075 0070 0073 6d6f 6444 626c  .o.k.u.p.smodDbl
+000019f0: 6f62 0000 0008 3e34 94a3 0aba c541 0000  ob....>4.....A..
+00001a00: 0007 006c 006f 006f 006b 0075 0070 0073  ...l.o.o.k.u.p.s
+00001a10: 7068 3153 636f 6d70 0000 0000 0005 3000  ph1Scomp......0.
+00001a20: 0000 0007 006c 006f 006f 006b 0075 0070  .....l.o.o.k.u.p
+00001a30: 0073 7653 726e 6c6f 6e67 0000 0001 0000  .svSrnlong......
+00001a40: 0004 0073 0068 0061 0070 6c67 3153 636f  ...s.h.a.plg1Sco
+00001a50: 6d70 0000 0000 0009 06c3 0000 0004 0073  mp.............s
+00001a60: 0068 0061 0070 6d6f 4444 626c 6f62 0000  .h.a.pmoDDblob..
+00001a70: 0008 868a a4a8 0aba c541 0000 0004 0073  .........A.....s
+00001a80: 0068 0061 0070 6d6f 6444 626c 6f62 0000  .h.a.pmodDblob..
+00001a90: 0008 868a a4a8 0aba c541 0000 0004 0073  .........A.....s
+00001aa0: 0068 0061 0070 7068 3153 636f 6d70 0000  .h.a.pph1Scomp..
+00001ab0: 0000 0009 9000 0000 0003 0073 0074 006c  ...........s.t.l
+00001ac0: 6c67 3153 636f 6d70 0000 0000 0053 7f67  lg1Scomp.....S.g
+00001ad0: 0000 0003 0073 0074 006c 6d6f 4444 626c  .....s.t.lmoDDbl
+00001ae0: 6f62 0000 0008 398b b9ad 0aba c541 0000  ob....9......A..
+00001af0: 0003 0073 0074 006c 6d6f 6444 626c 6f62  ...s.t.lmodDblob
+00001b00: 0000 0008 398b b9ad 0aba c541 0000 0003  ....9......A....
+00001b10: 0073 0074 006c 7068 3153 636f 6d70 0000  .s.t.lph1Scomp..
+00001b20: 0000 0053 a000 0000 000c 0075 006e 0073  ...S.......u.n.s
+00001b30: 0075 0070 0065 0072 0076 0069 0073 0065  .u.p.e.r.v.i.s.e
+00001b40: 0064 6277 7370 626c 6f62 0000 00b9 6270  .dbwspblob....bp
+00001b50: 6c69 7374 3030 d601 0203 0405 0607 0807  list00..........
+00001b60: 080b 085d 5368 6f77 5374 6174 7573 4261  ...]ShowStatusBa
+00001b70: 725b 5368 6f77 546f 6f6c 6261 725b 5368  r[ShowToolbar[Sh
+00001b80: 6f77 5461 6256 6965 775f 1014 436f 6e74  owTabView_..Cont
+00001b90: 6169 6e65 7253 686f 7753 6964 6562 6172  ainerShowSidebar
+00001ba0: 5c57 696e 646f 7742 6f75 6e64 735b 5368  \WindowBounds[Sh
+00001bb0: 6f77 5369 6465 6261 7208 0908 095f 1019  owSidebar...._..
+00001bc0: 7b7b 3236 302c 2031 3238 7d2c 207b 3131  {{260, 128}, {11
+00001bd0: 3434 2c20 3633 387d 7d09 0815 232f 3b52  44, 638}}...#/;R
+00001be0: 5f6b 6c6d 6e6f 8b00 0000 0000 0001 0100  _klmno..........
+00001bf0: 0000 0000 0000 0d00 0000 0000 0000 0000  ................
+00001c00: 0000 0000 0000 8c00 0000 0c00 7500 6e00  ............u.n.
+00001c10: 7300 7500 7000 6500 7200 7600 6900 7300  s.u.p.e.r.v.i.s.
+00001c20: 6500 646c 6731 5363 6f6d 7000 0000 0000  e.dlg1Scomp.....
+00001c30: 01e3 0a00 0000 0c00 7500 6e00 7300 7500  ........u.n.s.u.
+00001c40: 7000 6500 7200 7600 6900 7300 6500 646d  p.e.r.v.i.s.e.dm
+00001c50: 6f44 4462 6c6f 6200 0000 08b5 830b b00a  oDDblob.........
+00001c60: bac5 4100 0000 0c00 7500 6e00 7300 7500  ..A.....u.n.s.u.
+00001c70: 7000 6500 7200 7600 6900 7300 6500 646d  p.e.r.v.i.s.e.dm
+00001c80: 6f64 4462 6c6f 6200 0000 08b5 830b b00a  odDblob.........
+00001c90: bac5 4100 0000 0c00 7500 6e00 7300 7500  ..A.....u.n.s.u.
+00001ca0: 7000 6500 7200 7600 6900 7300 6500 6470  p.e.r.v.i.s.e.dp
+00001cb0: 6831 5363 6f6d 7000 0000 0000 01f0 0000  h1Scomp.........
+00001cc0: 0000 0c00 7500 6e00 7300 7500 7000 6500  ....u.n.s.u.p.e.
+00001cd0: 7200 7600 6900 7300 6500 6476 5372 6e6c  r.v.i.s.e.dvSrnl
+00001ce0: 6f6e 6700 0000 0100 0000 0000 0000 0000  ong.............
 00001cf0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001d00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001d10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001d20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001d30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001d40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001d50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -586,56 +586,56 @@
 00002490: 0100 0200 0000 0000 0100 0400 0000 0000  ................
 000024a0: 0100 0800 0000 0000 0100 1000 0000 0000  ................
 000024b0: 0100 2000 0000 0000 0100 4000 0000 0000  .. .......@.....
 000024c0: 0100 8000 0000 0000 0101 0000 0000 0000  ................
 000024d0: 0102 0000 0000 0000 0104 0000 0000 0000  ................
 000024e0: 0108 0000 0000 0000 0110 0000 0000 0000  ................
 000024f0: 0120 0000 0000 0000 0140 0000 0000 0000  . .......@......
-00002500: 0065 7273 696f 6e23 4030 0000 0000 0000  .ersion#@0......
-00002510: 09d9 0e0f 1011 1213 1415 1617 2025 2a2f  ............ %*/
-00002520: 3438 3d41 5863 6f6d 6d65 6e74 7355 6c61  48=AXcommentsUla
-00002530: 6265 6c57 7665 7273 696f 6e5b 6461 7465  belWversion[date
-00002540: 4372 6561 7465 6454 7369 7a65 5c64 6174  CreatedTsize\dat
-00002550: 654d 6f64 6966 6965 6454 6b69 6e64 546e  eModifiedTkindTn
-00002560: 616d 655e 6461 7465 4c61 7374 4f70 656e  ame^dateLastOpen
-00002570: 6564 d418 191a 1b1c 1d0c 1f57 7669 7369  ed.........Wvisi
-00002580: 626c 6555 7769 6474 6859 6173 6365 6e64  bleUwidthYascend
-00002590: 696e 6755 696e 6465 7808 1101 2c09 1007  ingUindex...,...
-000025a0: d418 191a 1b1c 220c 2408 1064 0910 05d4  ......".$..d....
-000025b0: 1819 1a1b 1c27 0c29 0810 4b09 1006 d418  .....'.)..K.....
-000025c0: 191a 1b1c 2c1c 2e08 10b5 0810 02d4 1819  ....,...........
-000025d0: 1a1b 0c31 1c33 0910 6108 1003 d418 191a  ...1.3..a.......
-000025e0: 1b0c 2c1c 3709 0810 01d4 1819 1a1b 0c3a  ..,.7..........:
-000025f0: 0c3c 0910 7309 1004 d418 191a 1b0c 1d0c  .<..s...........
-00002600: 4009 0910 00d4 1819 1a1b 1c43 1c45 0810  @..........C.E..
-00002610: c808 1008 0823 0000 0000 0000 0000 2340  .....#........#@
-00002620: 2800 0000 0000 005c 6461 7465 4d6f 6469  (......\dateModi
-00002630: 6669 6564 0900 0800 1d00 2600 3800 4000  fied......&.8.@.
-00002640: 5400 6600 6f00 8100 8c00 9f00 b400 bd00  T.f.o...........
-00002650: be00 d100 da00 e000 e800 f400 f901 0601  ................
-00002660: 0b01 1001 1f01 2801 3001 3601 4001 4601  ......(.0.6.@.F.
-00002670: 4701 4a01 4b01 4d01 5601 5701 5901 5a01  G.J.K.M.V.W.Y.Z.
-00002680: 5c01 6501 6601 6801 6901 6b01 7401 7501  \.e.f.h.i.k.t.u.
-00002690: 7701 7801 7a01 8301 8401 8601 8701 8901  w.x.z...........
-000026a0: 9201 9301 9401 9601 9f01 a001 a201 a301  ................
-000026b0: a501 ae01 af01 b001 b201 bb01 bc01 be01  ................
-000026c0: bf01 c101 c201 cb01 d401 e100 0000 0000  ................
-000026d0: 0002 0100 0000 0000 0000 4b00 0000 0000  ..........K.....
-000026e0: 0000 0000 0000 0000 0001 e200 0000 0500  ................
-000026f0: 6900 6300 6f00 6e00 736d 6f44 4462 6c6f  i.c.o.n.smoDDblo
-00002700: 6200 0000 0838 25f7 6a88 f4c5 4100 0000  b....8%.j...A...
-00002710: 0500 6900 6300 6f00 6e00 736d 6f64 4462  ..i.c.o.n.smodDb
-00002720: 6c6f 6200 0000 0838 25f7 6a88 f4c5 4100  lob....8%.j...A.
-00002730: 0000 0500 6900 6300 6f00 6e00 7370 6831  ....i.c.o.n.sph1
-00002740: 5363 6f6d 7000 0000 0000 0be0 0000 0000  Scomp...........
-00002750: 0500 6900 6300 6f00 6e00 7376 5372 6e6c  ..i.c.o.n.svSrnl
-00002760: 6f6e 6700 0000 0100 0000 0300 6900 6d00  ong.........i.m.
-00002770: 6762 7773 7062 6c6f 6200 0000 b862 706c  gbwspblob....bpl
-00002780: 6973 7430 30d6 0102 0304 0506 0708 0708  ist00...........
-00002790: 0b08 5d53 686f 7753 7461 7475 7342 6172  ..]ShowStatusBar
-000027a0: 5b53 686f 7754 6f6f 6c62 6172 5b53 686f  [ShowToolbar[Sho
-000027b0: 7754 6162 5669 6577 5f10 1443 6f6e 7461  wTabView_..Conta
-000027c0: 696e 6572 5368 6f77 5369 6465 6261 725c  inerShowSidebar\
-000027d0: 5769 6e64 6f77 426f 756e 6473 5b53 686f  WindowBounds[Sho
-000027e0: 7753 6964 6562 6172 0809 0809 5f10 187b  wSidebar...._..{
-000027f0: 7b32 3630 2c20 3332 397d 2c20 7b39 3230  {260, 329}, {920
-00002800: 2c20 3433                                , 43
+00002500: 0072 7369 6f6e 2340 3000 0000 0000 0009  .rsion#@0.......
+00002510: d90e 0f10 1112 1314 1516 1720 252a 2f34  ........... %*/4
+00002520: 383d 4158 636f 6d6d 656e 7473 556c 6162  8=AXcommentsUlab
+00002530: 656c 5776 6572 7369 6f6e 5b64 6174 6543  elWversion[dateC
+00002540: 7265 6174 6564 5473 697a 655c 6461 7465  reatedTsize\date
+00002550: 4d6f 6469 6669 6564 546b 696e 6454 6e61  ModifiedTkindTna
+00002560: 6d65 5e64 6174 654c 6173 744f 7065 6e65  me^dateLastOpene
+00002570: 64d4 1819 1a1b 1c1d 0c1f 5776 6973 6962  d.........Wvisib
+00002580: 6c65 5577 6964 7468 5961 7363 656e 6469  leUwidthYascendi
+00002590: 6e67 5569 6e64 6578 0811 012c 0910 07d4  ngUindex...,....
+000025a0: 1819 1a1b 1c22 0c24 0810 6409 1005 d418  .....".$..d.....
+000025b0: 191a 1b1c 270c 2908 104b 0910 06d4 1819  ....'.)..K......
+000025c0: 1a1b 1c2c 1c2e 0810 b508 1002 d418 191a  ...,............
+000025d0: 1b0c 311c 3309 1061 0810 03d4 1819 1a1b  ..1.3..a........
+000025e0: 0c2c 1c37 0908 1001 d418 191a 1b0c 3a0c  .,.7..........:.
+000025f0: 3c09 1073 0910 04d4 1819 1a1b 0c1d 0c40  <..s...........@
+00002600: 0909 1000 d418 191a 1b1c 431c 4508 10c8  ..........C.E...
+00002610: 0810 0808 2300 0000 0000 0000 0023 4028  ....#........#@(
+00002620: 0000 0000 0000 5c64 6174 654d 6f64 6966  ......\dateModif
+00002630: 6965 6409 0008 001d 0026 0038 0040 0054  ied......&.8.@.T
+00002640: 0066 006f 0081 008c 009f 00b4 00bd 00be  .f.o............
+00002650: 00d1 00da 00e0 00e8 00f4 00f9 0106 010b  ................
+00002660: 0110 011f 0128 0130 0136 0140 0146 0147  .....(.0.6.@.F.G
+00002670: 014a 014b 014d 0156 0157 0159 015a 015c  .J.K.M.V.W.Y.Z.\
+00002680: 0165 0166 0168 0169 016b 0174 0175 0177  .e.f.h.i.k.t.u.w
+00002690: 0178 017a 0183 0184 0186 0187 0189 0192  .x.z............
+000026a0: 0193 0194 0196 019f 01a0 01a2 01a3 01a5  ................
+000026b0: 01ae 01af 01b0 01b2 01bb 01bc 01be 01bf  ................
+000026c0: 01c1 01c2 01cb 01d4 01e1 0000 0000 0000  ................
+000026d0: 0201 0000 0000 0000 004b 0000 0000 0000  .........K......
+000026e0: 0000 0000 0000 0000 01e2 0000 0005 0069  ...............i
+000026f0: 0063 006f 006e 0073 6d6f 4444 626c 6f62  .c.o.n.smoDDblob
+00002700: 0000 0008 3825 f76a 88f4 c541 0000 0005  ....8%.j...A....
+00002710: 0069 0063 006f 006e 0073 6d6f 6444 626c  .i.c.o.n.smodDbl
+00002720: 6f62 0000 0008 3825 f76a 88f4 c541 0000  ob....8%.j...A..
+00002730: 0005 0069 0063 006f 006e 0073 7068 3153  ...i.c.o.n.sph1S
+00002740: 636f 6d70 0000 0000 000b e000 0000 0005  comp............
+00002750: 0069 0063 006f 006e 0073 7653 726e 6c6f  .i.c.o.n.svSrnlo
+00002760: 6e67 0000 0001 0000 0003 0069 006d 0067  ng.........i.m.g
+00002770: 6277 7370 626c 6f62 0000 00b8 6270 6c69  bwspblob....bpli
+00002780: 7374 3030 d601 0203 0405 0607 0807 080b  st00............
+00002790: 085d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
+000027a0: 5368 6f77 546f 6f6c 6261 725b 5368 6f77  ShowToolbar[Show
+000027b0: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
+000027c0: 6e65 7253 686f 7753 6964 6562 6172 5c57  nerShowSidebar\W
+000027d0: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
+000027e0: 5369 6465 6261 7208 0908 095f 1018 7b7b  Sidebar...._..{{
+000027f0: 3236 302c 2033 3239 7d2c 207b 3932 302c  260, 329}, {920,
+00002800: 2034 3336                                 436
```

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/lookups/model_names.parquet` & `Simba-UW-tf-dev-1.92.5/simba/assets/lookups/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/lookups/feature_extraction_headers.csv` & `Simba-UW-tf-dev-1.92.5/simba/assets/lookups/feature_extraction_headers.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/lookups/critical_values_05.pickle` & `Simba-UW-tf-dev-1.92.5/simba/assets/lookups/critical_values_05.pickle`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/lookups/features.csv` & `Simba-UW-tf-dev-1.92.5/simba/assets/lookups/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/lookups/unsupervised_example_x.csv` & `Simba-UW-tf-dev-1.92.5/simba/assets/lookups/unsupervised_example_x.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/stl/operant_tray.stl` & `Simba-UW-tf-dev-1.92.5/simba/assets/stl/operant_tray.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/stl/operant_lever.stl` & `Simba-UW-tf-dev-1.92.5/simba/assets/stl/operant_lever.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/stl/operant_walls.stl` & `Simba-UW-tf-dev-1.92.5/simba/assets/stl/operant_walls.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/stl/grid_floor.stl` & `Simba-UW-tf-dev-1.92.5/simba/assets/stl/grid_floor.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/img/splash_2024.mp4` & `Simba-UW-tf-dev-1.92.5/simba/assets/img/splash_2024.mp4`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/img/bg_2024.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/img/bg_2024.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/img/about_me.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/img/about_me.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/img/splash.mp4` & `Simba-UW-tf-dev-1.92.5/simba/assets/img/splash.mp4`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/img/bg_2.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/img/bg_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/img/splash.pptx` & `Simba-UW-tf-dev-1.92.5/simba/assets/img/splash.pptx`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/img/bg.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/img/bg.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.92.5/simba/assets/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/factory.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/factory.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/cluster.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/cluster.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/load.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/load.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/gif.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/gif.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/pose.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/pose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/features.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/features.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/.DS_Store` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/settings.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/settings.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/stopwatch.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/stopwatch.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/link.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/link.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/dash_simba.css` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/dash_simba.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/documentation.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/documentation.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/fps.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/fps.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/dimensionality_reduction.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/dimensionality_reduction.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/roi.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/roi.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/simba_logo_2.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/simba_logo_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/superimpose.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/superimpose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/label.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/label.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/change.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/change.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/readthedocs_logo.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/readthedocs_logo.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/crop.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/crop.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/rotate.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/rotate.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/circle.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/circle.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/path.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/path.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/polygon.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/polygon.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/clip.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/clip.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/restart.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/restart.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/calipher.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/calipher.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/add_on.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/add_on.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/create.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/create.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/SimBA_logo.ico` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/SimBA_logo.ico`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/print.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/print.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/clf.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/clf.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/concat_icons/mosaic.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/concat_icons/mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/concat_icons/vertical.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/concat_icons/vertical.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/concat_icons/horizontal.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/concat_icons/horizontal.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/concat_icons/mixed_mosaic.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/concat_icons/mixed_mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/brightness.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/brightness.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/merge.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/merge.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/clean.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/clean.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/clf_2.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/clf_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/visualize.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/visualize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/concat.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/concat.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/boris.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/boris.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/frames.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/frames.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/video.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/video.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/sample.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/sample.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/metrics.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/metrics.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/grey.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/grey.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/exit.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/exit.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/outlier.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/outlier.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/clahe.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/clahe.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/trash.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/trash.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/about.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/about.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/convert.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/convert.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/SimBA_logo.icns` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/SimBA_logo.icns`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/reorganize.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/reorganize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/browse.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/browse.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/SimBA_logo.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/SimBA_logo.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/ethovision.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/ethovision.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/icons/close.png` & `Simba-UW-tf-dev-1.92.5/simba/assets/icons/close.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/dash_simba_base.css` & `Simba-UW-tf-dev-1.92.5/simba/assets/dash_simba_base.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/simba/assets/TheGoldenLab.PNG` & `Simba-UW-tf-dev-1.92.5/simba/assets/TheGoldenLab.PNG`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/Simba_UW_tf_dev.egg-info/PKG-INFO` & `Simba-UW-tf-dev-1.92.5/Simba_UW_tf_dev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.92.4
+Version: 1.92.5
 Summary: Toolkit for computer classification of behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.92.4/Simba_UW_tf_dev.egg-info/SOURCES.txt` & `Simba-UW-tf-dev-1.92.5/Simba_UW_tf_dev.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -468,14 +468,15 @@
 simba/sandbox/sorensen_dice_coefficient.py
 simba/sandbox/spontaneous_alternation_calculator.py
 simba/sandbox/spontaneuous_alternation_plotter.py
 simba/sandbox/spontanous_alternations.py
 simba/sandbox/statistics_ex.py
 simba/sandbox/superimpose_elapsed_time.py
 simba/sandbox/superimpose_frame_count.py
+simba/sandbox/superimpose_popups.py
 simba/sandbox/superpixels.py
 simba/sandbox/termite_rois.csv
 simba/sandbox/time_stamp_calculator.py
 simba/sandbox/total_variation_distance.py
 simba/sandbox/train_model.py
 simba/sandbox/two_fish_feature_extractor_040924.py
 simba/sandbox/two_fish_feature_extractor_040924.py.zip
```

### Comparing `Simba-UW-tf-dev-1.92.4/Simba_UW_tf_dev.egg-info/requires.txt` & `Simba-UW-tf-dev-1.92.5/Simba_UW_tf_dev.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/LICENSE` & `Simba-UW-tf-dev-1.92.5/LICENSE`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/tests/test_data_processors.py` & `Simba-UW-tf-dev-1.92.5/tests/test_data_processors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/tests/test_circlular_stats.py` & `Simba-UW-tf-dev-1.92.5/tests/test_circlular_stats.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/tests/test_stats.py` & `Simba-UW-tf-dev-1.92.5/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/tests/test_train_model_mixin.py` & `Simba-UW-tf-dev-1.92.5/tests/test_train_model_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/tests/test_feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.92.5/tests/test_feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/tests/test_utils_data.py` & `Simba-UW-tf-dev-1.92.5/tests/test_utils_data.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/tests/test_config_reader_mixin.py` & `Simba-UW-tf-dev-1.92.5/tests/test_config_reader_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/tests/test_outlier_correctors.py` & `Simba-UW-tf-dev-1.92.5/tests/test_outlier_correctors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/tests/test_featurizers.py` & `Simba-UW-tf-dev-1.92.5/tests/test_featurizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/tests/test_video_processors.py` & `Simba-UW-tf-dev-1.92.5/tests/test_video_processors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/tests/test_thirdparty_appenders.py` & `Simba-UW-tf-dev-1.92.5/tests/test_thirdparty_appenders.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/tests/test_validation_clips.py` & `Simba-UW-tf-dev-1.92.5/tests/test_validation_clips.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/tests/test_roi_tools.py` & `Simba-UW-tf-dev-1.92.5/tests/test_roi_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/README.md` & `Simba-UW-tf-dev-1.92.5/README.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.92.4/setup.py` & `Simba-UW-tf-dev-1.92.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 with open("requirements.txt", "r") as f:
     requirements = f.read().splitlines()
 
 exclusion_patterns = ["pose_configurations_archive"]
 
 setuptools.setup(
     name="Simba-UW-tf-dev",
-    version="1.92.4",
+    version="1.92.5",
     author="Simon Nilsson, Jia Jie Choong, Sophia Hwang",
     author_email="sronilsson@gmail.com",
     description="Toolkit for computer classification of behaviors in experimental animals",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/sgoldenlab/simba",
     install_requires=requirements,
```

