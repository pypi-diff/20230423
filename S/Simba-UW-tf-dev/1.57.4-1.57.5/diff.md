# Comparing `tmp/Simba-UW-tf-dev-1.57.4.tar.gz` & `tmp/Simba-UW-tf-dev-1.57.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Simba-UW-tf-dev-1.57.4.tar", last modified: Sat Apr 22 17:32:08 2023, max compression
+gzip compressed data, was "dist/Simba-UW-tf-dev-1.57.5.tar", last modified: Sun Apr 23 12:52:10 2023, max compression
```

## Comparing `Simba-UW-tf-dev-1.57.4.tar` & `Simba-UW-tf-dev-1.57.5.tar`

### file list

```diff
@@ -1,395 +1,396 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:08.000000 Simba-UW-tf-dev-1.57.4/
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-22 17:32:08.000000 Simba-UW-tf-dev-1.57.4/PKG-INFO
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/simba/
--rw-r--r--   0 simon      (501) staff       (20)    38767 2023-04-15 18:44:14.000000 Simba-UW-tf-dev-1.57.4/simba/video_processing.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/simba/blob_storage/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-21 20:39:46.000000 Simba-UW-tf-dev-1.57.4/simba/blob_storage/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:08.000000 Simba-UW-tf-dev-1.57.4/simba/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)    11938 2023-04-20 14:29:24.000000 Simba-UW-tf-dev-1.57.4/simba/unsupervised/dbcv_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    10960 2023-04-19 14:59:03.000000 Simba-UW-tf-dev-1.57.4/simba/unsupervised/unsupervised_ui.py
--rw-r--r--   0 simon      (501) staff       (20)     3354 2023-04-20 14:05:40.000000 Simba-UW-tf-dev-1.57.4/simba/unsupervised/enums.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-20 13:38:50.000000 Simba-UW-tf-dev-1.57.4/simba/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7569 2023-04-20 15:20:31.000000 Simba-UW-tf-dev-1.57.4/simba/unsupervised/dataset_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     4812 2023-04-20 14:48:41.000000 Simba-UW-tf-dev-1.57.4/simba/unsupervised/grid_search_visualizers.py
--rw-r--r--   0 simon      (501) staff       (20)     6687 2023-04-20 15:04:13.000000 Simba-UW-tf-dev-1.57.4/simba/unsupervised/data_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)     9907 2023-04-20 12:55:14.000000 Simba-UW-tf-dev-1.57.4/simba/unsupervised/ui.py
--rw-r--r--   0 simon      (501) staff       (20)     8375 2023-04-19 18:35:33.000000 Simba-UW-tf-dev-1.57.4/simba/unsupervised/umap_embedder.py
--rw-r--r--   0 simon      (501) staff       (20)    41552 2023-04-20 14:49:52.000000 Simba-UW-tf-dev-1.57.4/simba/unsupervised/pop_up_classes.py
--rw-r--r--   0 simon      (501) staff       (20)     2331 2023-04-20 12:56:44.000000 Simba-UW-tf-dev-1.57.4/simba/unsupervised/bout_aggregator.py
--rw-r--r--   0 simon      (501) staff       (20)    18472 2023-04-19 23:04:27.000000 Simba-UW-tf-dev-1.57.4/simba/unsupervised/cluster_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.57.4/simba/unsupervised/data_map.yaml
--rw-r--r--   0 simon      (501) staff       (20)     8421 2023-04-20 13:33:19.000000 Simba-UW-tf-dev-1.57.4/simba/unsupervised/hdbscan_clusterer.py
--rw-r--r--   0 simon      (501) staff       (20)     3931 2023-04-19 18:21:47.000000 Simba-UW-tf-dev-1.57.4/simba/unsupervised/tsne.py
--rw-r--r--   0 simon      (501) staff       (20)     5895 2023-04-18 19:12:52.000000 Simba-UW-tf-dev-1.57.4/simba/unsupervised/cluster_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    19486 2023-04-18 14:10:55.000000 Simba-UW-tf-dev-1.57.4/simba/enums.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/simba/bounding_box_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/bounding_box_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7520 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.4/simba/bounding_box_tools/agg_boundary_stats.py
--rw-r--r--   0 simon      (501) staff       (20)     8596 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.4/simba/bounding_box_tools/find_bounderies.py
--rw-r--r--   0 simon      (501) staff       (20)    24561 2023-04-06 11:22:38.000000 Simba-UW-tf-dev-1.57.4/simba/bounding_box_tools/boundary_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     9536 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.4/simba/bounding_box_tools/boundary_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    12664 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.4/simba/bounding_box_tools/visualize_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    32772 2023-04-22 15:14:38.000000 Simba-UW-tf-dev-1.57.4/simba/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/
--rw-r--r--   0 simon      (501) staff       (20)    42823 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/feature_extractor_14bp.py
--rw-r--r--   0 simon      (501) staff       (20)    21575 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/feature_extractor_7bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/
--rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/doctests.py
--rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
--rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/read_in_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     1959 2023-04-20 20:07:38.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/peaks.py
--rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/fish_feature_extractor_2022.py
--rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
--rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/convex_hull_scratch_1.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
--rw-r--r--   0 simon      (501) staff       (20)     7127 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/egocentrical_aligner.py
--rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/count_values_in_range.py
--rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/graph_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/termite_rois.csv
--rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/mutual_exclusive.py
--rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/video_color.py
--rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/graph_3d_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/video_rotator.py
--rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/add_probability_cnt_features.py
--rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/make_splash.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/video_rotator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    26890 2023-04-20 18:25:40.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
--rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/convex_hull_scratch_2.py
--rw-r--r--   0 simon      (501) staff       (20)    28003 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/feature_extractor_8bps_2_animals.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-04-22 15:54:57.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     2293 2023-04-13 15:35:56.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/perimeter_jit.py
--rw-r--r--   0 simon      (501) staff       (20)    10774 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/feature_subsets.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)      905 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)   238196 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    69038 2023-04-04 11:32:25.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)   238298 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    69338 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     2179 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    36728 2023-04-17 19:25:13.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/extract_features_9bp.py
--rw-r--r--   0 simon      (501) staff       (20)     8483 2023-04-22 17:31:56.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/feature_extractor_user_defined.py
--rw-r--r--   0 simon      (501) staff       (20)     5380 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/unit_tests.py
--rw-r--r--   0 simon      (501) staff       (20)    46489 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/feature_extractor_16bp.py
--rw-r--r--   0 simon      (501) staff       (20)    24076 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/feature_extractor_8bp.py
--rw-r--r--   0 simon      (501) staff       (20)    16793 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/feature_extractor_4bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/.idea/features_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/.idea/.gitignore
--rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/.idea/.name
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)     6044 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/plotly_create_h5.py
--rw-r--r--   0 simon      (501) staff       (20)    15351 2023-04-06 14:48:36.000000 Simba-UW-tf-dev-1.57.4/simba/requirements.txt
--rw-r--r--   0 simon      (501) staff       (20)     5928 2023-04-10 15:43:18.000000 Simba-UW-tf-dev-1.57.4/simba/severity_processor.py
--rw-r--r--   0 simon      (501) staff       (20)     5900 2023-04-10 16:12:09.000000 Simba-UW-tf-dev-1.57.4/simba/user_pose_config_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/simba/mixins/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.57.4/simba/mixins/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    42063 2023-04-19 23:53:37.000000 Simba-UW-tf-dev-1.57.4/simba/mixins/pop_up_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     8351 2023-04-22 13:11:36.000000 Simba-UW-tf-dev-1.57.4/simba/mixins/config_reader.py
--rw-r--r--   0 simon      (501) staff       (20)     6781 2023-04-11 20:14:16.000000 Simba-UW-tf-dev-1.57.4/simba/mixins/feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     6092 2023-04-19 18:08:18.000000 Simba-UW-tf-dev-1.57.4/simba/mixins/unsupervised_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    34586 2023-04-15 19:04:12.000000 Simba-UW-tf-dev-1.57.4/simba/machine_model_settings_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5231 2023-04-10 15:22:21.000000 Simba-UW-tf-dev-1.57.4/simba/remove_keypoints_in_pose.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:08.000000 Simba-UW-tf-dev-1.57.4/simba/third_party_label_appenders/
--rw-r--r--   0 simon      (501) staff       (20)     6400 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.4/simba/third_party_label_appenders/deepethogram_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     9984 2023-04-10 18:32:39.000000 Simba-UW-tf-dev-1.57.4/simba/third_party_label_appenders/BORIS_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     9242 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.4/simba/third_party_label_appenders/observer_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    16922 2023-03-28 20:30:38.000000 Simba-UW-tf-dev-1.57.4/simba/third_party_label_appenders/tools.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.57.4/simba/third_party_label_appenders/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18322 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.4/simba/third_party_label_appenders/third_party_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8372 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.4/simba/third_party_label_appenders/ethovision_import.py
--rw-r--r--   0 simon      (501) staff       (20)     6964 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.4/simba/third_party_label_appenders/BENTO_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     5471 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.4/simba/third_party_label_appenders/solomon_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7286 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.4/simba/multi_cropper.py
--rw-r--r--   0 simon      (501) staff       (20)    12867 2023-04-18 20:27:02.000000 Simba-UW-tf-dev-1.57.4/simba/FSTTC_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    12575 2023-04-10 12:13:26.000000 Simba-UW-tf-dev-1.57.4/simba/create_project_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    13377 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.57.4/simba/video_info_table.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/simba/cue_light_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:25:58.000000 Simba-UW-tf-dev-1.57.4/simba/cue_light_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     8632 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.4/simba/cue_light_tools/cue_light_clf_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    13564 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.4/simba/cue_light_tools/cue_light_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    18253 2023-04-06 11:29:26.000000 Simba-UW-tf-dev-1.57.4/simba/cue_light_tools/cue_light_menues.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/cue_light_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1660 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/cue_light_tools/cue_light_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    16427 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.4/simba/cue_light_tools/cue_light_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    13265 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.4/simba/cue_light_tools/cue_light_movement_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2813 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/extract_frames_fast.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:08.000000 Simba-UW-tf-dev-1.57.4/simba/utils/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 20:15:03.000000 Simba-UW-tf-dev-1.57.4/simba/utils/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7335 2023-04-10 18:32:39.000000 Simba-UW-tf-dev-1.57.4/simba/utils/warnings.py
--rw-r--r--   0 simon      (501) staff       (20)     5345 2023-04-14 15:36:09.000000 Simba-UW-tf-dev-1.57.4/simba/utils/lookups.py
--rw-r--r--   0 simon      (501) staff       (20)    14631 2023-04-16 19:52:37.000000 Simba-UW-tf-dev-1.57.4/simba/utils/errors.py
--rw-r--r--   0 simon      (501) staff       (20)     1045 2023-04-12 13:34:48.000000 Simba-UW-tf-dev-1.57.4/simba/utils/printing.py
--rw-r--r--   0 simon      (501) staff       (20)    21641 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.4/simba/labelling_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     9980 2023-04-10 15:43:18.000000 Simba-UW-tf-dev-1.57.4/simba/timebins_movement_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    47395 2023-04-20 01:59:56.000000 Simba-UW-tf-dev-1.57.4/simba/train_model_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/SimBA_dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     7556 2023-04-10 15:43:18.000000 Simba-UW-tf-dev-1.57.4/simba/timebins_clf_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     8240 2023-03-17 16:23:58.000000 Simba-UW-tf-dev-1.57.4/simba/calculate_px_dist.py
--rw-r--r--   0 simon      (501) staff       (20)     6566 2023-04-10 15:22:21.000000 Simba-UW-tf-dev-1.57.4/simba/movement_processor.py
--rw-r--r--   0 simon      (501) staff       (20)     2904 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/pybursts.py
--rw-r--r--   0 simon      (501) staff       (20)     4047 2023-04-17 01:05:46.000000 Simba-UW-tf-dev-1.57.4/simba/rw_dfs.py
--rw-r--r--   0 simon      (501) staff       (20)     6536 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.4/simba/reverse_2_animal_tracking.py
--rw-r--r--   0 simon      (501) staff       (20)     9770 2023-04-10 14:38:06.000000 Simba-UW-tf-dev-1.57.4/simba/Directing_animals_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     3570 2023-04-10 23:04:08.000000 Simba-UW-tf-dev-1.57.4/simba/Validate_model_one_video_run_clf.py
--rw-r--r--   0 simon      (501) staff       (20)    10872 2023-04-21 16:14:46.000000 Simba-UW-tf-dev-1.57.4/simba/tkinter_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    13767 2023-03-24 12:49:19.000000 Simba-UW-tf-dev-1.57.4/simba/setting_menu.py
--rw-r--r--   0 simon      (501) staff       (20)     6614 2023-03-19 16:33:17.000000 Simba-UW-tf-dev-1.57.4/simba/interpolate_pose.py
--rw-r--r--   0 simon      (501) staff       (20)     4771 2023-04-10 19:17:14.000000 Simba-UW-tf-dev-1.57.4/simba/run_inference.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:08.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/
--rw-r--r--   0 simon      (501) staff       (20)     8634 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/gantt_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:08.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/tools/
--rw-r--r--   0 simon      (501) staff       (20)     5353 2023-03-30 15:38:37.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/tools/tkinter_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    18101 2023-04-10 17:14:05.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/ROI_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15262 2023-04-19 14:54:02.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/shap_agg_stats_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12985 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/gantt_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15811 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/heat_mapper_clf_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8839 2023-04-10 17:06:45.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/probability_plot_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    16036 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/misc_visualizations.py
--rw-r--r--   0 simon      (501) staff       (20)    13533 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/plot_clf_results.py
--rw-r--r--   0 simon      (501) staff       (20)    17734 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/plot_clf_results_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    16340 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/ROI_feature_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12691 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/heat_mapper_location.py
--rw-r--r--   0 simon      (501) staff       (20)    12646 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/probability_plot_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     5341 2023-03-30 15:46:49.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/interactive_probability_grapher.py
--rw-r--r--   0 simon      (501) staff       (20)     5896 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/plot_pose_in_dir.py
--rw-r--r--   0 simon      (501) staff       (20)    12256 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/single_run_model_validation_video.py
--rw-r--r--   0 simon      (501) staff       (20)    11246 2023-04-10 17:06:45.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/frame_mergerer_ffmpeg.py
--rw-r--r--   0 simon      (501) staff       (20)    12570 2023-04-10 16:40:38.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/Directing_animals_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     9979 2023-04-10 16:36:45.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/clf_validator.py
--rw-r--r--   0 simon      (501) staff       (20)    17891 2023-04-22 14:54:57.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/path_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    20037 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/ROI_feature_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    10219 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/data_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    12889 2023-04-22 14:51:45.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/path_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     8685 2023-04-10 17:02:33.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/ez_lineplot.py
--rw-r--r--   0 simon      (501) staff       (20)    13027 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/distance_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15890 2023-04-10 17:14:05.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/ROI_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13230 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/heat_mapper_clf.py
--rw-r--r--   0 simon      (501) staff       (20)     8951 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13625 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/single_run_model_validation_video_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    10005 2023-04-10 16:38:59.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/Directing_animals_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    16189 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/heat_mapper_location_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/run_dash_tkinter.py
--rw-r--r--   0 simon      (501) staff       (20)     7609 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.4/simba/interpolate_smooth_post_hoc.py
--rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     6350 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/reverse_tracking_order.py
--rw-r--r--   0 simon      (501) staff       (20)     5772 2023-03-20 13:55:20.000000 Simba-UW-tf-dev-1.57.4/simba/concatenator_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2863 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.4/simba/extract_annotation_frames.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:08.000000 Simba-UW-tf-dev-1.57.4/simba/roi_tools/
--rw-r--r--   0 simon      (501) staff       (20)     7437 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.4/simba/roi_tools/ROI_time_bin_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     2166 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.4/simba/roi_tools/ROI_movement_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.57.4/simba/roi_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    43921 2023-04-10 18:21:25.000000 Simba-UW-tf-dev-1.57.4/simba/roi_tools/ROI_define.py
--rw-r--r--   0 simon      (501) staff       (20)     3384 2023-03-20 12:41:16.000000 Simba-UW-tf-dev-1.57.4/simba/roi_tools/ROI_reset.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/roi_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    21277 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.57.4/simba/roi_tools/ROI_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    11934 2023-04-10 18:32:39.000000 Simba-UW-tf-dev-1.57.4/simba/roi_tools/ROI_feature_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     3537 2023-03-15 17:12:38.000000 Simba-UW-tf-dev-1.57.4/simba/roi_tools/ROI_multiply.py
--rw-r--r--   0 simon      (501) staff       (20)      961 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/roi_tools/ROI_size_calculations.py
--rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/roi_tools/ROI_zoom.py
--rw-r--r--   0 simon      (501) staff       (20)    11335 2023-04-05 11:07:42.000000 Simba-UW-tf-dev-1.57.4/simba/roi_tools/ROI_directing_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/roi_tools/ROI_move_shape.py
--rw-r--r--   0 simon      (501) staff       (20)     5097 2023-04-05 20:01:02.000000 Simba-UW-tf-dev-1.57.4/simba/roi_tools/ROI_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    15290 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.57.4/simba/roi_tools/ROI_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    22682 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/roi_tools/ROI_image.py
--rw-r--r--   0 simon      (501) staff       (20)    56353 2023-04-20 15:18:16.000000 Simba-UW-tf-dev-1.57.4/simba/misc_tools.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:08.000000 Simba-UW-tf-dev-1.57.4/simba/pose_importers/
--rw-r--r--   0 simon      (501) staff       (20)     2494 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/pose_importers/read_DANNCE_mat.py
--rw-r--r--   0 simon      (501) staff       (20)    25864 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.4/simba/pose_importers/sleap_importer_slp.py
--rw-r--r--   0 simon      (501) staff       (20)    24665 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.57.4/simba/pose_importers/sleap_importer_h5.py
--rw-r--r--   0 simon      (501) staff       (20)    26731 2023-04-10 17:34:37.000000 Simba-UW-tf-dev-1.57.4/simba/pose_importers/dlc_multi_animal_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    23776 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.57.4/simba/pose_importers/sleap_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)    16483 2023-04-14 16:41:29.000000 Simba-UW-tf-dev-1.57.4/simba/pose_importers/import_trk.py
--rw-r--r--   0 simon      (501) staff       (20)     7924 2023-04-10 17:34:37.000000 Simba-UW-tf-dev-1.57.4/simba/pose_importers/import_mars.py
--rw-r--r--   0 simon      (501) staff       (20)     8919 2023-04-10 17:29:32.000000 Simba-UW-tf-dev-1.57.4/simba/pose_importers/dlc_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)     7828 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.57.4/simba/pose_importers/trk_importer.py
--rw-r--r--   0 simon      (501) staff       (20)   236359 2023-04-22 15:26:04.000000 Simba-UW-tf-dev-1.57.4/simba/pop_up_classes.py
--rw-r--r--   0 simon      (501) staff       (20)     4692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/extract_seqframes.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:08.000000 Simba-UW-tf-dev-1.57.4/simba/pose_configurations/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.57.4/simba/pose_configurations/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:08.000000 Simba-UW-tf-dev-1.57.4/simba/pose_configurations/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.57.4/simba/pose_configurations/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-10 12:22:28.000000 Simba-UW-tf-dev-1.57.4/simba/pose_configurations/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:08.000000 Simba-UW-tf-dev-1.57.4/simba/pose_configurations/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       24 2023-03-20 15:55:45.000000 Simba-UW-tf-dev-1.57.4/simba/pose_configurations/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.57.4/simba/pose_configurations/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:08.000000 Simba-UW-tf-dev-1.57.4/simba/pose_configurations/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.57.4/simba/pose_configurations/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      267 2023-03-20 15:55:45.000000 Simba-UW-tf-dev-1.57.4/simba/pose_configurations/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:08.000000 Simba-UW-tf-dev-1.57.4/simba/pose_configurations/schematics/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.57.4/simba/pose_configurations/schematics/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/pose_configurations/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.57.4/simba/pose_configurations/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/pose_configurations/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.57.4/simba/pose_configurations/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.57.4/simba/pose_configurations/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/pose_configurations/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/pose_configurations/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/pose_configurations/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/pose_configurations/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/pose_configurations/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/pose_configurations/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/pose_configurations/schematics/1.png
--rw-r--r--   0 simon      (501) staff       (20)     7273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/get_coordinates_tools_v2.py
--rw-r--r--   0 simon      (501) staff       (20)    16252 2023-03-15 19:16:56.000000 Simba-UW-tf-dev-1.57.4/simba/pup_retrieval_protocol.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/simba/outlier_tools/
--rw-r--r--   0 simon      (501) staff       (20)     7822 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.57.4/simba/outlier_tools/outlier_corrector_movement.py
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-15 17:05:05.000000 Simba-UW-tf-dev-1.57.4/simba/outlier_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/outlier_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8304 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.4/simba/outlier_tools/outlier_corrector_location.py
--rw-r--r--   0 simon      (501) staff       (20)     4411 2023-04-10 16:33:31.000000 Simba-UW-tf-dev-1.57.4/simba/outlier_tools/skip_outlier_correction.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/simba/outlier_tools/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/outlier_tools/.idea/outlier_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/outlier_tools/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/simba/outlier_tools/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/simba/outlier_tools/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/outlier_tools/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/outlier_tools/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/outlier_tools/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/outlier_tools/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)     2610 2023-04-10 15:22:21.000000 Simba-UW-tf-dev-1.57.4/simba/pose_reset.py
--rw-r--r--   0 simon      (501) staff       (20)    19358 2023-04-21 19:25:08.000000 Simba-UW-tf-dev-1.57.4/simba/train_mutiple_models.py
--rw-r--r--   0 simon      (501) staff       (20)    64554 2023-04-22 15:14:52.000000 Simba-UW-tf-dev-1.57.4/simba/SimBA.py
--rw-r--r--   0 simon      (501) staff       (20)    27472 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.4/simba/labelling_advanced_interface.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/simba/assets/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/simba/assets/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/unsupervised/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/unsupervised/features.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/simba/assets/shap/
--rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/shap/down_arrow.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/shap/intruder_shape.jpg
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/simba/assets/shap/feature_categories/
--rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
--rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/shap/feature_categories/shap_feature_categories.csv
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.57.4/simba/assets/shap/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/shap/resident_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/shap/resident_intruder_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/shap/animal_distances.jpg
--rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/shap/baseline_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/shap/ubuntu.regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/shap/side_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/shap/UbuntuMono-Regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/shap/side_scale_5.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/shap/intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/shap/resident_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/shap/color_bar.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/shap/resident_intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)    16388 2023-04-22 15:52:42.000000 Simba-UW-tf-dev-1.57.4/simba/assets/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/simba/assets/lookups/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/lookups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/lookups/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)     2426 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/lookups/feature_extraction_headers.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/lookups/features.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/lookups/unsupervised_example_x.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/simba/assets/stl/
--rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/stl/operant_tray.stl
--rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/stl/operant_lever.stl
--rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/stl/operant_walls.stl
--rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/stl/grid_floor.stl
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/simba/assets/img/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.57.4/simba/assets/img/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/img/about_me.png
--rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.57.4/simba/assets/img/splash.mp4
--rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.57.4/simba/assets/img/bg_2.png
--rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/img/splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.57.4/simba/assets/img/bg.png
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/UbuntuMono-Regular.ttf
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/
--rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/factory.png
--rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/cluster.png
--rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/load.png
--rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/gif.png
--rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/pose.png
--rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/features.png
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/.DS_Store
--rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/settings.png
--rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/stopwatch.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/link.png
--rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/dash_simba.css
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/documentation.png
--rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/fps.png
--rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/dimensionality_reduction.png
--rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/roi.png
--rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/superimpose.png
--rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/label.png
--rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/change.png
--rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/crop.png
--rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/rotate.png
--rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/path.png
--rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/clip.png
--rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/restart.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/calipher.png
--rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/add_on.png
--rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/create.png
--rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/SimBA_logo.ico
--rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/print.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/clf.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/concat_icons/
--rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/concat_icons/mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/concat_icons/vertical.png
--rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/concat_icons/horizontal.png
--rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/concat_icons/mixed_mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/merge.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/clean.png
--rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/clf_2.png
--rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/visualize.png
--rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/concat.png
--rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/boris.png
--rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/frames.png
--rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/video.png
--rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/sample.png
--rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/metrics.png
--rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/grey.png
--rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/exit.png
--rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/outlier.png
--rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/clahe.png
--rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/trash.png
--rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/about.png
--rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/convert.png
--rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/SimBA_logo.icns
--rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/reorganize.png
--rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/browse.png
--rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/SimBA_logo.png
--rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/ethovision.png
--rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/close.png
--rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/dash_simba_base.css
--rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/TheGoldenLab.PNG
--rw-r--r--   0 simon      (501) staff       (20)    15545 2023-04-14 16:40:51.000000 Simba-UW-tf-dev-1.57.4/simba/drop_bp_cords.py
--rw-r--r--   0 simon      (501) staff       (20)     9460 2023-04-21 14:18:35.000000 Simba-UW-tf-dev-1.57.4/simba/read_config_unit_tests.py
--rw-r--r--   0 simon      (501) staff       (20)    11742 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.4/simba/project_config_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    27444 2023-03-15 15:58:40.000000 Simba-UW-tf-dev-1.57.4/simba/set_hyperparameters.py
--rw-r--r--   0 simon      (501) staff       (20)    20756 2023-04-19 14:41:07.000000 Simba-UW-tf-dev-1.57.4/simba/train_single_model.py
--rw-r--r--   0 simon      (501) staff       (20)     6467 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.4/simba/create_clf_log.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/simba/batch_process_videos/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-17 14:43:38.000000 Simba-UW-tf-dev-1.57.4/simba/batch_process_videos/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    24911 2023-04-17 19:39:19.000000 Simba-UW-tf-dev-1.57.4/simba/batch_process_videos/batch_process_menus.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/batch_process_videos/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    10930 2023-04-17 19:35:15.000000 Simba-UW-tf-dev-1.57.4/simba/batch_process_videos/batch_process_create_ffmpeg_commands.py
--rw-r--r--   0 simon      (501) staff       (20)     9585 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.4/simba/Kleinberg_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8349 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.4/simba/reorganize_keypoint_in_pose.py
--rw-r--r--   0 simon      (501) staff       (20)      165 2023-03-25 11:18:21.000000 Simba-UW-tf-dev-1.57.4/simba/~$features.pptx
--rw-r--r--   0 simon      (501) staff       (20)     6557 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/play_annotation_video.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/Simba_UW_tf_dev.egg-info/
--rw-rw-r--   0 simon      (501) staff       (20)      579 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/Simba_UW_tf_dev.egg-info/PKG-INFO
--rw-rw-r--   0 simon      (501) staff       (20)    13533 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/Simba_UW_tf_dev.egg-info/SOURCES.txt
--rw-rw-r--   0 simon      (501) staff       (20)       44 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/Simba_UW_tf_dev.egg-info/entry_points.txt
--rw-rw-r--   0 simon      (501) staff       (20)      639 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/Simba_UW_tf_dev.egg-info/requires.txt
--rw-rw-r--   0 simon      (501) staff       (20)        6 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/Simba_UW_tf_dev.egg-info/top_level.txt
--rw-rw-r--   0 simon      (501) staff       (20)        1 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/Simba_UW_tf_dev.egg-info/dependency_links.txt
--rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.57.4/LICENSE.md
--rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.57.4/MANIFEST.in
--rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.57.4/README.md
--rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-04-22 17:31:56.000000 Simba-UW-tf-dev-1.57.4/setup.py
--rw-r--r--   0 simon      (501) staff       (20)       38 2023-04-22 17:32:08.000000 Simba-UW-tf-dev-1.57.4/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-23 12:52:10.000000 Simba-UW-tf-dev-1.57.5/
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-23 12:52:10.000000 Simba-UW-tf-dev-1.57.5/PKG-INFO
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-23 12:52:10.000000 Simba-UW-tf-dev-1.57.5/simba/
+-rw-r--r--   0 simon      (501) staff       (20)    38767 2023-04-15 18:44:14.000000 Simba-UW-tf-dev-1.57.5/simba/video_processing.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-23 12:52:10.000000 Simba-UW-tf-dev-1.57.5/simba/blob_storage/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-21 20:39:46.000000 Simba-UW-tf-dev-1.57.5/simba/blob_storage/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-23 12:52:10.000000 Simba-UW-tf-dev-1.57.5/simba/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)    11938 2023-04-20 14:29:24.000000 Simba-UW-tf-dev-1.57.5/simba/unsupervised/dbcv_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    10960 2023-04-19 14:59:03.000000 Simba-UW-tf-dev-1.57.5/simba/unsupervised/unsupervised_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     3354 2023-04-20 14:05:40.000000 Simba-UW-tf-dev-1.57.5/simba/unsupervised/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-20 13:38:50.000000 Simba-UW-tf-dev-1.57.5/simba/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7569 2023-04-20 15:20:31.000000 Simba-UW-tf-dev-1.57.5/simba/unsupervised/dataset_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     4812 2023-04-20 14:48:41.000000 Simba-UW-tf-dev-1.57.5/simba/unsupervised/grid_search_visualizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     6687 2023-04-20 15:04:13.000000 Simba-UW-tf-dev-1.57.5/simba/unsupervised/data_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)     9907 2023-04-20 12:55:14.000000 Simba-UW-tf-dev-1.57.5/simba/unsupervised/ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     8375 2023-04-19 18:35:33.000000 Simba-UW-tf-dev-1.57.5/simba/unsupervised/umap_embedder.py
+-rw-r--r--   0 simon      (501) staff       (20)    41552 2023-04-20 14:49:52.000000 Simba-UW-tf-dev-1.57.5/simba/unsupervised/pop_up_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)     2331 2023-04-20 12:56:44.000000 Simba-UW-tf-dev-1.57.5/simba/unsupervised/bout_aggregator.py
+-rw-r--r--   0 simon      (501) staff       (20)    18472 2023-04-19 23:04:27.000000 Simba-UW-tf-dev-1.57.5/simba/unsupervised/cluster_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.57.5/simba/unsupervised/data_map.yaml
+-rw-r--r--   0 simon      (501) staff       (20)     8421 2023-04-20 13:33:19.000000 Simba-UW-tf-dev-1.57.5/simba/unsupervised/hdbscan_clusterer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3931 2023-04-19 18:21:47.000000 Simba-UW-tf-dev-1.57.5/simba/unsupervised/tsne.py
+-rw-r--r--   0 simon      (501) staff       (20)     5895 2023-04-18 19:12:52.000000 Simba-UW-tf-dev-1.57.5/simba/unsupervised/cluster_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    19486 2023-04-18 14:10:55.000000 Simba-UW-tf-dev-1.57.5/simba/enums.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-23 12:52:10.000000 Simba-UW-tf-dev-1.57.5/simba/bounding_box_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/bounding_box_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7520 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.5/simba/bounding_box_tools/agg_boundary_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)     8596 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.5/simba/bounding_box_tools/find_bounderies.py
+-rw-r--r--   0 simon      (501) staff       (20)    24561 2023-04-06 11:22:38.000000 Simba-UW-tf-dev-1.57.5/simba/bounding_box_tools/boundary_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     9536 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.5/simba/bounding_box_tools/boundary_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    12664 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.5/simba/bounding_box_tools/visualize_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    32772 2023-04-22 15:14:38.000000 Simba-UW-tf-dev-1.57.5/simba/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-23 12:52:10.000000 Simba-UW-tf-dev-1.57.5/simba/feature_extractors/
+-rw-r--r--   0 simon      (501) staff       (20)    42823 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.57.5/simba/feature_extractors/feature_extractor_14bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    21575 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.57.5/simba/feature_extractors/feature_extractor_7bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-23 12:52:10.000000 Simba-UW-tf-dev-1.57.5/simba/feature_extractors/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.57.5/simba/feature_extractors/misc/doctests.py
+-rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.57.5/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.57.5/simba/feature_extractors/misc/read_in_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.57.5/simba/feature_extractors/misc/peaks.py
+-rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.57.5/simba/feature_extractors/misc/fish_feature_extractor_2022.py
+-rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.57.5/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.57.5/simba/feature_extractors/misc/convex_hull_scratch_1.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.57.5/simba/feature_extractors/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.57.5/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     7127 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/feature_extractors/misc/egocentrical_aligner.py
+-rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.57.5/simba/feature_extractors/misc/count_values_in_range.py
+-rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/feature_extractors/misc/graph_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/feature_extractors/misc/termite_rois.csv
+-rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.57.5/simba/feature_extractors/misc/mutual_exclusive.py
+-rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.57.5/simba/feature_extractors/misc/video_color.py
+-rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/feature_extractors/misc/graph_3d_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.57.5/simba/feature_extractors/misc/video_rotator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/feature_extractors/misc/add_probability_cnt_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.57.5/simba/feature_extractors/misc/make_splash.py
+-rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.57.5/simba/feature_extractors/misc/time_stamp_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.57.5/simba/feature_extractors/misc/video_rotator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    30331 2023-04-23 12:30:57.000000 Simba-UW-tf-dev-1.57.5/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
+-rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.57.5/simba/feature_extractors/misc/convex_hull_scratch_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    28003 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.57.5/simba/feature_extractors/feature_extractor_8bps_2_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-04-22 19:19:45.000000 Simba-UW-tf-dev-1.57.5/simba/feature_extractors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     2293 2023-04-13 15:35:56.000000 Simba-UW-tf-dev-1.57.5/simba/feature_extractors/perimeter_jit.py
+-rw-r--r--   0 simon      (501) staff       (20)    10774 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.5/simba/feature_extractors/feature_subsets.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/feature_extractors/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-23 12:52:10.000000 Simba-UW-tf-dev-1.57.5/simba/feature_extractors/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)      905 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.57.5/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)   238196 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.57.5/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    69038 2023-04-04 11:32:25.000000 Simba-UW-tf-dev-1.57.5/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)   238298 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.57.5/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    69338 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.57.5/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.57.5/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     2179 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.57.5/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    36728 2023-04-17 19:25:13.000000 Simba-UW-tf-dev-1.57.5/simba/feature_extractors/extract_features_9bp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8483 2023-04-22 17:31:56.000000 Simba-UW-tf-dev-1.57.5/simba/feature_extractors/feature_extractor_user_defined.py
+-rw-r--r--   0 simon      (501) staff       (20)     5380 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.57.5/simba/feature_extractors/unit_tests.py
+-rw-r--r--   0 simon      (501) staff       (20)    46489 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.57.5/simba/feature_extractors/feature_extractor_16bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    24076 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.57.5/simba/feature_extractors/feature_extractor_8bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16793 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.57.5/simba/feature_extractors/feature_extractor_4bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-23 12:52:10.000000 Simba-UW-tf-dev-1.57.5/simba/feature_extractors/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/feature_extractors/.idea/features_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/feature_extractors/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-23 12:52:10.000000 Simba-UW-tf-dev-1.57.5/simba/feature_extractors/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-23 12:52:10.000000 Simba-UW-tf-dev-1.57.5/simba/feature_extractors/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/feature_extractors/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/feature_extractors/.idea/.gitignore
+-rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/feature_extractors/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/feature_extractors/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/feature_extractors/.idea/.name
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/feature_extractors/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)     6044 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/plotly_create_h5.py
+-rw-r--r--   0 simon      (501) staff       (20)    15351 2023-04-06 14:48:36.000000 Simba-UW-tf-dev-1.57.5/simba/requirements.txt
+-rw-r--r--   0 simon      (501) staff       (20)     5928 2023-04-10 15:43:18.000000 Simba-UW-tf-dev-1.57.5/simba/severity_processor.py
+-rw-r--r--   0 simon      (501) staff       (20)     5900 2023-04-10 16:12:09.000000 Simba-UW-tf-dev-1.57.5/simba/user_pose_config_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-23 12:52:10.000000 Simba-UW-tf-dev-1.57.5/simba/mixins/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.57.5/simba/mixins/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    42063 2023-04-19 23:53:37.000000 Simba-UW-tf-dev-1.57.5/simba/mixins/pop_up_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     8351 2023-04-22 13:11:36.000000 Simba-UW-tf-dev-1.57.5/simba/mixins/config_reader.py
+-rw-r--r--   0 simon      (501) staff       (20)     9048 2023-04-22 18:03:18.000000 Simba-UW-tf-dev-1.57.5/simba/mixins/feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     6092 2023-04-19 18:08:18.000000 Simba-UW-tf-dev-1.57.5/simba/mixins/unsupervised_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    34586 2023-04-15 19:04:12.000000 Simba-UW-tf-dev-1.57.5/simba/machine_model_settings_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5231 2023-04-10 15:22:21.000000 Simba-UW-tf-dev-1.57.5/simba/remove_keypoints_in_pose.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-23 12:52:10.000000 Simba-UW-tf-dev-1.57.5/simba/third_party_label_appenders/
+-rw-r--r--   0 simon      (501) staff       (20)     6400 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.5/simba/third_party_label_appenders/deepethogram_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     9984 2023-04-10 18:32:39.000000 Simba-UW-tf-dev-1.57.5/simba/third_party_label_appenders/BORIS_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     9242 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.5/simba/third_party_label_appenders/observer_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16922 2023-03-28 20:30:38.000000 Simba-UW-tf-dev-1.57.5/simba/third_party_label_appenders/tools.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.57.5/simba/third_party_label_appenders/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18322 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.5/simba/third_party_label_appenders/third_party_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8372 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.5/simba/third_party_label_appenders/ethovision_import.py
+-rw-r--r--   0 simon      (501) staff       (20)     6964 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.5/simba/third_party_label_appenders/BENTO_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     5471 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.5/simba/third_party_label_appenders/solomon_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7286 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.5/simba/multi_cropper.py
+-rw-r--r--   0 simon      (501) staff       (20)    12867 2023-04-18 20:27:02.000000 Simba-UW-tf-dev-1.57.5/simba/FSTTC_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12575 2023-04-10 12:13:26.000000 Simba-UW-tf-dev-1.57.5/simba/create_project_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    13377 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.57.5/simba/video_info_table.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-23 12:52:10.000000 Simba-UW-tf-dev-1.57.5/simba/cue_light_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:25:58.000000 Simba-UW-tf-dev-1.57.5/simba/cue_light_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     8632 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.5/simba/cue_light_tools/cue_light_clf_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    13564 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.5/simba/cue_light_tools/cue_light_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    18253 2023-04-06 11:29:26.000000 Simba-UW-tf-dev-1.57.5/simba/cue_light_tools/cue_light_menues.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/cue_light_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1660 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/cue_light_tools/cue_light_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    16427 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.5/simba/cue_light_tools/cue_light_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    13265 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.5/simba/cue_light_tools/cue_light_movement_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2813 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/extract_frames_fast.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-23 12:52:10.000000 Simba-UW-tf-dev-1.57.5/simba/utils/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 20:15:03.000000 Simba-UW-tf-dev-1.57.5/simba/utils/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7335 2023-04-10 18:32:39.000000 Simba-UW-tf-dev-1.57.5/simba/utils/warnings.py
+-rw-r--r--   0 simon      (501) staff       (20)     5345 2023-04-14 15:36:09.000000 Simba-UW-tf-dev-1.57.5/simba/utils/lookups.py
+-rw-r--r--   0 simon      (501) staff       (20)    14631 2023-04-16 19:52:37.000000 Simba-UW-tf-dev-1.57.5/simba/utils/errors.py
+-rw-r--r--   0 simon      (501) staff       (20)     1045 2023-04-12 13:34:48.000000 Simba-UW-tf-dev-1.57.5/simba/utils/printing.py
+-rw-r--r--   0 simon      (501) staff       (20)    21641 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.5/simba/labelling_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     9980 2023-04-10 15:43:18.000000 Simba-UW-tf-dev-1.57.5/simba/timebins_movement_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    47395 2023-04-20 01:59:56.000000 Simba-UW-tf-dev-1.57.5/simba/train_model_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/SimBA_dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     7556 2023-04-10 15:43:18.000000 Simba-UW-tf-dev-1.57.5/simba/timebins_clf_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     8240 2023-03-17 16:23:58.000000 Simba-UW-tf-dev-1.57.5/simba/calculate_px_dist.py
+-rw-r--r--   0 simon      (501) staff       (20)     6566 2023-04-10 15:22:21.000000 Simba-UW-tf-dev-1.57.5/simba/movement_processor.py
+-rw-r--r--   0 simon      (501) staff       (20)     2904 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/pybursts.py
+-rw-r--r--   0 simon      (501) staff       (20)     4154 2023-04-23 12:50:46.000000 Simba-UW-tf-dev-1.57.5/simba/rw_dfs.py
+-rw-r--r--   0 simon      (501) staff       (20)     6536 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.5/simba/reverse_2_animal_tracking.py
+-rw-r--r--   0 simon      (501) staff       (20)     9770 2023-04-10 14:38:06.000000 Simba-UW-tf-dev-1.57.5/simba/Directing_animals_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3570 2023-04-10 23:04:08.000000 Simba-UW-tf-dev-1.57.5/simba/Validate_model_one_video_run_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)    10872 2023-04-21 16:14:46.000000 Simba-UW-tf-dev-1.57.5/simba/tkinter_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    13767 2023-03-24 12:49:19.000000 Simba-UW-tf-dev-1.57.5/simba/setting_menu.py
+-rw-r--r--   0 simon      (501) staff       (20)     6614 2023-03-19 16:33:17.000000 Simba-UW-tf-dev-1.57.5/simba/interpolate_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)     4771 2023-04-10 19:17:14.000000 Simba-UW-tf-dev-1.57.5/simba/run_inference.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-23 12:52:10.000000 Simba-UW-tf-dev-1.57.5/simba/plotting/
+-rw-r--r--   0 simon      (501) staff       (20)     8634 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.5/simba/plotting/gantt_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-23 12:52:10.000000 Simba-UW-tf-dev-1.57.5/simba/plotting/tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5353 2023-03-30 15:38:37.000000 Simba-UW-tf-dev-1.57.5/simba/plotting/tools/tkinter_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    18101 2023-04-10 17:14:05.000000 Simba-UW-tf-dev-1.57.5/simba/plotting/ROI_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15262 2023-04-19 14:54:02.000000 Simba-UW-tf-dev-1.57.5/simba/plotting/shap_agg_stats_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12985 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.5/simba/plotting/gantt_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15811 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.5/simba/plotting/heat_mapper_clf_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8839 2023-04-10 17:06:45.000000 Simba-UW-tf-dev-1.57.5/simba/plotting/probability_plot_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16036 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.5/simba/plotting/misc_visualizations.py
+-rw-r--r--   0 simon      (501) staff       (20)    13533 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.5/simba/plotting/plot_clf_results.py
+-rw-r--r--   0 simon      (501) staff       (20)    17734 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.5/simba/plotting/plot_clf_results_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16340 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.5/simba/plotting/ROI_feature_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12691 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.5/simba/plotting/heat_mapper_location.py
+-rw-r--r--   0 simon      (501) staff       (20)    12646 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.5/simba/plotting/probability_plot_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     5341 2023-03-30 15:46:49.000000 Simba-UW-tf-dev-1.57.5/simba/plotting/interactive_probability_grapher.py
+-rw-r--r--   0 simon      (501) staff       (20)     5896 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.5/simba/plotting/plot_pose_in_dir.py
+-rw-r--r--   0 simon      (501) staff       (20)    12256 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.5/simba/plotting/single_run_model_validation_video.py
+-rw-r--r--   0 simon      (501) staff       (20)    11246 2023-04-10 17:06:45.000000 Simba-UW-tf-dev-1.57.5/simba/plotting/frame_mergerer_ffmpeg.py
+-rw-r--r--   0 simon      (501) staff       (20)    12570 2023-04-10 16:40:38.000000 Simba-UW-tf-dev-1.57.5/simba/plotting/Directing_animals_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     9979 2023-04-10 16:36:45.000000 Simba-UW-tf-dev-1.57.5/simba/plotting/clf_validator.py
+-rw-r--r--   0 simon      (501) staff       (20)    17891 2023-04-22 14:54:57.000000 Simba-UW-tf-dev-1.57.5/simba/plotting/path_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    20037 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.5/simba/plotting/ROI_feature_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    10219 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.5/simba/plotting/data_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    12889 2023-04-22 14:51:45.000000 Simba-UW-tf-dev-1.57.5/simba/plotting/path_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     8685 2023-04-10 17:02:33.000000 Simba-UW-tf-dev-1.57.5/simba/plotting/ez_lineplot.py
+-rw-r--r--   0 simon      (501) staff       (20)    13027 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.5/simba/plotting/distance_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15890 2023-04-10 17:14:05.000000 Simba-UW-tf-dev-1.57.5/simba/plotting/ROI_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13230 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.5/simba/plotting/heat_mapper_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)     8951 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.5/simba/plotting/distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13625 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.5/simba/plotting/single_run_model_validation_video_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    10005 2023-04-10 16:38:59.000000 Simba-UW-tf-dev-1.57.5/simba/plotting/Directing_animals_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16189 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.5/simba/plotting/heat_mapper_location_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/run_dash_tkinter.py
+-rw-r--r--   0 simon      (501) staff       (20)     7609 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.5/simba/interpolate_smooth_post_hoc.py
+-rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     6350 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/reverse_tracking_order.py
+-rw-r--r--   0 simon      (501) staff       (20)     5772 2023-03-20 13:55:20.000000 Simba-UW-tf-dev-1.57.5/simba/concatenator_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2863 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.5/simba/extract_annotation_frames.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-23 12:52:10.000000 Simba-UW-tf-dev-1.57.5/simba/roi_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     7437 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.5/simba/roi_tools/ROI_time_bin_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2166 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.5/simba/roi_tools/ROI_movement_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.57.5/simba/roi_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    43921 2023-04-10 18:21:25.000000 Simba-UW-tf-dev-1.57.5/simba/roi_tools/ROI_define.py
+-rw-r--r--   0 simon      (501) staff       (20)     3384 2023-03-20 12:41:16.000000 Simba-UW-tf-dev-1.57.5/simba/roi_tools/ROI_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/roi_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    21277 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.57.5/simba/roi_tools/ROI_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11934 2023-04-10 18:32:39.000000 Simba-UW-tf-dev-1.57.5/simba/roi_tools/ROI_feature_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3537 2023-03-15 17:12:38.000000 Simba-UW-tf-dev-1.57.5/simba/roi_tools/ROI_multiply.py
+-rw-r--r--   0 simon      (501) staff       (20)      961 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/roi_tools/ROI_size_calculations.py
+-rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/roi_tools/ROI_zoom.py
+-rw-r--r--   0 simon      (501) staff       (20)    11335 2023-04-05 11:07:42.000000 Simba-UW-tf-dev-1.57.5/simba/roi_tools/ROI_directing_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/roi_tools/ROI_move_shape.py
+-rw-r--r--   0 simon      (501) staff       (20)     5097 2023-04-05 20:01:02.000000 Simba-UW-tf-dev-1.57.5/simba/roi_tools/ROI_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    15290 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.57.5/simba/roi_tools/ROI_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    22682 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/roi_tools/ROI_image.py
+-rw-r--r--   0 simon      (501) staff       (20)    56353 2023-04-20 15:18:16.000000 Simba-UW-tf-dev-1.57.5/simba/misc_tools.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-23 12:52:10.000000 Simba-UW-tf-dev-1.57.5/simba/pose_importers/
+-rw-r--r--   0 simon      (501) staff       (20)     2494 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/pose_importers/read_DANNCE_mat.py
+-rw-r--r--   0 simon      (501) staff       (20)    25864 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.5/simba/pose_importers/sleap_importer_slp.py
+-rw-r--r--   0 simon      (501) staff       (20)    24665 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.57.5/simba/pose_importers/sleap_importer_h5.py
+-rw-r--r--   0 simon      (501) staff       (20)    26731 2023-04-10 17:34:37.000000 Simba-UW-tf-dev-1.57.5/simba/pose_importers/dlc_multi_animal_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    23776 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.57.5/simba/pose_importers/sleap_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)    16483 2023-04-14 16:41:29.000000 Simba-UW-tf-dev-1.57.5/simba/pose_importers/import_trk.py
+-rw-r--r--   0 simon      (501) staff       (20)     7924 2023-04-10 17:34:37.000000 Simba-UW-tf-dev-1.57.5/simba/pose_importers/import_mars.py
+-rw-r--r--   0 simon      (501) staff       (20)     8919 2023-04-10 17:29:32.000000 Simba-UW-tf-dev-1.57.5/simba/pose_importers/dlc_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)     7828 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.57.5/simba/pose_importers/trk_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)   236359 2023-04-22 15:26:04.000000 Simba-UW-tf-dev-1.57.5/simba/pop_up_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)     4692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/extract_seqframes.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-23 12:52:10.000000 Simba-UW-tf-dev-1.57.5/simba/pose_configurations/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.57.5/simba/pose_configurations/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-23 12:52:10.000000 Simba-UW-tf-dev-1.57.5/simba/pose_configurations/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.57.5/simba/pose_configurations/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-10 12:22:28.000000 Simba-UW-tf-dev-1.57.5/simba/pose_configurations/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-23 12:52:10.000000 Simba-UW-tf-dev-1.57.5/simba/pose_configurations/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       24 2023-03-20 15:55:45.000000 Simba-UW-tf-dev-1.57.5/simba/pose_configurations/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.57.5/simba/pose_configurations/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-23 12:52:10.000000 Simba-UW-tf-dev-1.57.5/simba/pose_configurations/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.57.5/simba/pose_configurations/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      267 2023-03-20 15:55:45.000000 Simba-UW-tf-dev-1.57.5/simba/pose_configurations/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-23 12:52:10.000000 Simba-UW-tf-dev-1.57.5/simba/pose_configurations/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.57.5/simba/pose_configurations/schematics/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/pose_configurations/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.57.5/simba/pose_configurations/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/pose_configurations/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.57.5/simba/pose_configurations/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.57.5/simba/pose_configurations/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/pose_configurations/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/pose_configurations/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/pose_configurations/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/pose_configurations/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/pose_configurations/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/pose_configurations/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/pose_configurations/schematics/1.png
+-rw-r--r--   0 simon      (501) staff       (20)     7273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/get_coordinates_tools_v2.py
+-rw-r--r--   0 simon      (501) staff       (20)    16252 2023-03-15 19:16:56.000000 Simba-UW-tf-dev-1.57.5/simba/pup_retrieval_protocol.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-23 12:52:10.000000 Simba-UW-tf-dev-1.57.5/simba/outlier_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     7822 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.57.5/simba/outlier_tools/outlier_corrector_movement.py
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-15 17:05:05.000000 Simba-UW-tf-dev-1.57.5/simba/outlier_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/outlier_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8304 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.5/simba/outlier_tools/outlier_corrector_location.py
+-rw-r--r--   0 simon      (501) staff       (20)     4584 2023-04-23 12:51:22.000000 Simba-UW-tf-dev-1.57.5/simba/outlier_tools/skip_outlier_correction.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-23 12:52:10.000000 Simba-UW-tf-dev-1.57.5/simba/outlier_tools/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/outlier_tools/.idea/outlier_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/outlier_tools/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-23 12:52:10.000000 Simba-UW-tf-dev-1.57.5/simba/outlier_tools/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-23 12:52:10.000000 Simba-UW-tf-dev-1.57.5/simba/outlier_tools/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/outlier_tools/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/outlier_tools/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/outlier_tools/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/outlier_tools/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)     2610 2023-04-10 15:22:21.000000 Simba-UW-tf-dev-1.57.5/simba/pose_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)    19358 2023-04-21 19:25:08.000000 Simba-UW-tf-dev-1.57.5/simba/train_mutiple_models.py
+-rw-r--r--   0 simon      (501) staff       (20)    64554 2023-04-22 15:14:52.000000 Simba-UW-tf-dev-1.57.5/simba/SimBA.py
+-rw-r--r--   0 simon      (501) staff       (20)    27472 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.5/simba/labelling_advanced_interface.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-23 12:52:10.000000 Simba-UW-tf-dev-1.57.5/simba/assets/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-23 12:52:10.000000 Simba-UW-tf-dev-1.57.5/simba/assets/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/assets/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/assets/unsupervised/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/assets/unsupervised/features.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-23 12:52:10.000000 Simba-UW-tf-dev-1.57.5/simba/assets/shap/
+-rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/assets/shap/down_arrow.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/assets/shap/intruder_shape.jpg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-23 12:52:10.000000 Simba-UW-tf-dev-1.57.5/simba/assets/shap/feature_categories/
+-rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
+-rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/assets/shap/feature_categories/shap_feature_categories.csv
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.57.5/simba/assets/shap/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/assets/shap/resident_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/assets/shap/resident_intruder_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/assets/shap/animal_distances.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/assets/shap/baseline_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/assets/shap/ubuntu.regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/assets/shap/side_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/assets/shap/UbuntuMono-Regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/assets/shap/side_scale_5.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/assets/shap/intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/assets/shap/resident_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/assets/shap/color_bar.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/assets/shap/resident_intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)    16388 2023-04-22 15:52:42.000000 Simba-UW-tf-dev-1.57.5/simba/assets/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-23 12:52:10.000000 Simba-UW-tf-dev-1.57.5/simba/assets/lookups/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/assets/lookups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/assets/lookups/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)     2426 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/assets/lookups/feature_extraction_headers.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/assets/lookups/features.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/assets/lookups/unsupervised_example_x.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-23 12:52:10.000000 Simba-UW-tf-dev-1.57.5/simba/assets/stl/
+-rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/assets/stl/operant_tray.stl
+-rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/assets/stl/operant_lever.stl
+-rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/assets/stl/operant_walls.stl
+-rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/assets/stl/grid_floor.stl
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-23 12:52:10.000000 Simba-UW-tf-dev-1.57.5/simba/assets/img/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.57.5/simba/assets/img/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/assets/img/about_me.png
+-rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.57.5/simba/assets/img/splash.mp4
+-rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.57.5/simba/assets/img/bg_2.png
+-rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/assets/img/splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.57.5/simba/assets/img/bg.png
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/assets/UbuntuMono-Regular.ttf
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-23 12:52:10.000000 Simba-UW-tf-dev-1.57.5/simba/assets/icons/
+-rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.57.5/simba/assets/icons/factory.png
+-rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.57.5/simba/assets/icons/cluster.png
+-rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.57.5/simba/assets/icons/load.png
+-rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.57.5/simba/assets/icons/gif.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.57.5/simba/assets/icons/pose.png
+-rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.57.5/simba/assets/icons/features.png
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.57.5/simba/assets/icons/.DS_Store
+-rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.57.5/simba/assets/icons/settings.png
+-rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.57.5/simba/assets/icons/stopwatch.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.57.5/simba/assets/icons/link.png
+-rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/assets/icons/dash_simba.css
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.57.5/simba/assets/icons/documentation.png
+-rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.57.5/simba/assets/icons/fps.png
+-rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.57.5/simba/assets/icons/dimensionality_reduction.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.57.5/simba/assets/icons/roi.png
+-rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.57.5/simba/assets/icons/superimpose.png
+-rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.57.5/simba/assets/icons/label.png
+-rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.57.5/simba/assets/icons/change.png
+-rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.57.5/simba/assets/icons/crop.png
+-rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.57.5/simba/assets/icons/rotate.png
+-rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.57.5/simba/assets/icons/path.png
+-rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.57.5/simba/assets/icons/clip.png
+-rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.57.5/simba/assets/icons/restart.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.57.5/simba/assets/icons/calipher.png
+-rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.57.5/simba/assets/icons/add_on.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.57.5/simba/assets/icons/create.png
+-rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.57.5/simba/assets/icons/SimBA_logo.ico
+-rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.57.5/simba/assets/icons/print.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.57.5/simba/assets/icons/clf.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-23 12:52:10.000000 Simba-UW-tf-dev-1.57.5/simba/assets/icons/concat_icons/
+-rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/assets/icons/concat_icons/mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/assets/icons/concat_icons/vertical.png
+-rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/assets/icons/concat_icons/horizontal.png
+-rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/assets/icons/concat_icons/mixed_mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.57.5/simba/assets/icons/merge.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.57.5/simba/assets/icons/clean.png
+-rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.57.5/simba/assets/icons/clf_2.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.57.5/simba/assets/icons/visualize.png
+-rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.57.5/simba/assets/icons/concat.png
+-rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.57.5/simba/assets/icons/boris.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.57.5/simba/assets/icons/frames.png
+-rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.57.5/simba/assets/icons/video.png
+-rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.57.5/simba/assets/icons/sample.png
+-rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.57.5/simba/assets/icons/metrics.png
+-rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.57.5/simba/assets/icons/grey.png
+-rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.57.5/simba/assets/icons/exit.png
+-rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.57.5/simba/assets/icons/outlier.png
+-rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.57.5/simba/assets/icons/clahe.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.57.5/simba/assets/icons/trash.png
+-rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.57.5/simba/assets/icons/about.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.57.5/simba/assets/icons/convert.png
+-rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.57.5/simba/assets/icons/SimBA_logo.icns
+-rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.57.5/simba/assets/icons/reorganize.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.57.5/simba/assets/icons/browse.png
+-rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.57.5/simba/assets/icons/SimBA_logo.png
+-rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.57.5/simba/assets/icons/ethovision.png
+-rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.57.5/simba/assets/icons/close.png
+-rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/assets/dash_simba_base.css
+-rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/assets/TheGoldenLab.PNG
+-rw-r--r--   0 simon      (501) staff       (20)    15545 2023-04-14 16:40:51.000000 Simba-UW-tf-dev-1.57.5/simba/drop_bp_cords.py
+-rw-r--r--   0 simon      (501) staff       (20)     9460 2023-04-21 14:18:35.000000 Simba-UW-tf-dev-1.57.5/simba/read_config_unit_tests.py
+-rw-r--r--   0 simon      (501) staff       (20)    11742 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.5/simba/project_config_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    27444 2023-03-15 15:58:40.000000 Simba-UW-tf-dev-1.57.5/simba/set_hyperparameters.py
+-rw-r--r--   0 simon      (501) staff       (20)    20756 2023-04-19 14:41:07.000000 Simba-UW-tf-dev-1.57.5/simba/train_single_model.py
+-rw-r--r--   0 simon      (501) staff       (20)     6467 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.5/simba/create_clf_log.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-23 12:52:10.000000 Simba-UW-tf-dev-1.57.5/simba/batch_process_videos/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-17 14:43:38.000000 Simba-UW-tf-dev-1.57.5/simba/batch_process_videos/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    24911 2023-04-17 19:39:19.000000 Simba-UW-tf-dev-1.57.5/simba/batch_process_videos/batch_process_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/batch_process_videos/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    10930 2023-04-17 19:35:15.000000 Simba-UW-tf-dev-1.57.5/simba/batch_process_videos/batch_process_create_ffmpeg_commands.py
+-rw-r--r--   0 simon      (501) staff       (20)     9585 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.5/simba/Kleinberg_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8349 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.5/simba/reorganize_keypoint_in_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)      165 2023-03-25 11:18:21.000000 Simba-UW-tf-dev-1.57.5/simba/~$features.pptx
+-rw-r--r--   0 simon      (501) staff       (20)     6557 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.5/simba/play_annotation_video.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-23 12:52:10.000000 Simba-UW-tf-dev-1.57.5/Simba_UW_tf_dev.egg-info/
+-rw-rw-r--   0 simon      (501) staff       (20)      579 2023-04-23 12:52:10.000000 Simba-UW-tf-dev-1.57.5/Simba_UW_tf_dev.egg-info/PKG-INFO
+-rw-rw-r--   0 simon      (501) staff       (20)    13588 2023-04-23 12:52:10.000000 Simba-UW-tf-dev-1.57.5/Simba_UW_tf_dev.egg-info/SOURCES.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       44 2023-04-23 12:52:10.000000 Simba-UW-tf-dev-1.57.5/Simba_UW_tf_dev.egg-info/entry_points.txt
+-rw-rw-r--   0 simon      (501) staff       (20)      639 2023-04-23 12:52:10.000000 Simba-UW-tf-dev-1.57.5/Simba_UW_tf_dev.egg-info/requires.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        6 2023-04-23 12:52:10.000000 Simba-UW-tf-dev-1.57.5/Simba_UW_tf_dev.egg-info/top_level.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        1 2023-04-23 12:52:10.000000 Simba-UW-tf-dev-1.57.5/Simba_UW_tf_dev.egg-info/dependency_links.txt
+-rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.57.5/LICENSE.md
+-rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.57.5/MANIFEST.in
+-rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.57.5/README.md
+-rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-04-23 12:51:22.000000 Simba-UW-tf-dev-1.57.5/setup.py
+-rw-r--r--   0 simon      (501) staff       (20)       38 2023-04-23 12:52:10.000000 Simba-UW-tf-dev-1.57.5/setup.cfg
```

### Comparing `Simba-UW-tf-dev-1.57.4/PKG-INFO` & `Simba-UW-tf-dev-1.57.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.57.4
+Version: 1.57.5
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.57.4/simba/video_processing.py` & `Simba-UW-tf-dev-1.57.5/simba/video_processing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/blob_storage/.DS_Store` & `Simba-UW-tf-dev-1.57.5/simba/blob_storage/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/unsupervised/dbcv_calculator.py` & `Simba-UW-tf-dev-1.57.5/simba/unsupervised/dbcv_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/unsupervised/unsupervised_ui.py` & `Simba-UW-tf-dev-1.57.5/simba/unsupervised/unsupervised_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/unsupervised/enums.py` & `Simba-UW-tf-dev-1.57.5/simba/unsupervised/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.57.5/simba/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/unsupervised/dataset_creator.py` & `Simba-UW-tf-dev-1.57.5/simba/unsupervised/dataset_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/unsupervised/grid_search_visualizers.py` & `Simba-UW-tf-dev-1.57.5/simba/unsupervised/grid_search_visualizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/unsupervised/data_extractor.py` & `Simba-UW-tf-dev-1.57.5/simba/unsupervised/data_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/unsupervised/ui.py` & `Simba-UW-tf-dev-1.57.5/simba/unsupervised/ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/unsupervised/umap_embedder.py` & `Simba-UW-tf-dev-1.57.5/simba/unsupervised/umap_embedder.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/unsupervised/pop_up_classes.py` & `Simba-UW-tf-dev-1.57.5/simba/unsupervised/pop_up_classes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/unsupervised/bout_aggregator.py` & `Simba-UW-tf-dev-1.57.5/simba/unsupervised/bout_aggregator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/unsupervised/cluster_statistics.py` & `Simba-UW-tf-dev-1.57.5/simba/unsupervised/cluster_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/unsupervised/data_map.yaml` & `Simba-UW-tf-dev-1.57.5/simba/unsupervised/data_map.yaml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/unsupervised/hdbscan_clusterer.py` & `Simba-UW-tf-dev-1.57.5/simba/unsupervised/hdbscan_clusterer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/unsupervised/tsne.py` & `Simba-UW-tf-dev-1.57.5/simba/unsupervised/tsne.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/unsupervised/cluster_visualizer.py` & `Simba-UW-tf-dev-1.57.5/simba/unsupervised/cluster_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/enums.py` & `Simba-UW-tf-dev-1.57.5/simba/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/bounding_box_tools/.DS_Store` & `Simba-UW-tf-dev-1.57.5/simba/bounding_box_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/bounding_box_tools/agg_boundary_stats.py` & `Simba-UW-tf-dev-1.57.5/simba/bounding_box_tools/agg_boundary_stats.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/bounding_box_tools/find_bounderies.py` & `Simba-UW-tf-dev-1.57.5/simba/bounding_box_tools/find_bounderies.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/bounding_box_tools/boundary_menus.py` & `Simba-UW-tf-dev-1.57.5/simba/bounding_box_tools/boundary_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/bounding_box_tools/boundary_statistics.py` & `Simba-UW-tf-dev-1.57.5/simba/bounding_box_tools/boundary_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/bounding_box_tools/visualize_boundaries.py` & `Simba-UW-tf-dev-1.57.5/simba/bounding_box_tools/visualize_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/.DS_Store` & `Simba-UW-tf-dev-1.57.5/simba/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/feature_extractor_14bp.py` & `Simba-UW-tf-dev-1.57.5/simba/feature_extractors/feature_extractor_14bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/feature_extractor_7bp.py` & `Simba-UW-tf-dev-1.57.5/simba/feature_extractors/feature_extractor_7bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/doctests.py` & `Simba-UW-tf-dev-1.57.5/simba/feature_extractors/misc/doctests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py` & `Simba-UW-tf-dev-1.57.5/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/read_in_mp.py` & `Simba-UW-tf-dev-1.57.5/simba/feature_extractors/misc/read_in_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/peaks.py` & `Simba-UW-tf-dev-1.57.5/simba/feature_extractors/misc/peaks.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,50 @@
 import pandas as pd
 import numpy as np
 from scipy import stats
 from statsmodels.stats.diagnostic import lilliefors
 from scipy.signal import find_peaks
 
 
-def rolling_frequentist_distribution_tests(data: np.array, name: str):
-    rolling_idx = np.arange(50)[None, :] + 1*np.arange(data.shape[0])[:, None]
-    ks_results, ttest_results = np.full((data.shape[0]), -1.0), np.full((data.shape[0]), -1.0)
-    lillefors_results, shapiro_results = np.full((data.shape[0]), -1.0),  np.full((data.shape[0]), -1.0)
+def rolling_frequentist_distribution_tests(data: np.array,
+                                           feature_name: str,
+                                           fps: int):
+    """
+    Helper to compare feature value distributions in 1s sequential time-bins: Kolmogorov-Smirnov and T-tests
+    Compares the feature values against a normal distribution: Lillefors, Shapiro.
+    Find the number of peaks in *rolling* 1s long feature window.
+    """
+    ks_results, = np.full((data.shape[0]), -1.0),
+    t_test_results = np.full((data.shape[0]), -1.0)
+    lillefors_results = np.full((data.shape[0]), -1.0)
+    shapiro_results = np.full((data.shape[0]), -1.0)
     peak_cnt_results = np.full((data.shape[0]), -1.0)
-    for i in range(50, data.shape[0] - 50, 50):
-        bin_1_idx, bin_2_idx = [i-50, i], [i, i+50]
+
+    for i in range(fps, data.shape[0] - fps, fps):
+        bin_1_idx, bin_2_idx = [i-fps, i], [i, i+fps]
         bin_1_data, bin_2_data = data[bin_1_idx[0]:bin_1_idx[1]], data[bin_2_idx[0]:bin_2_idx[1]]
-        ks_results[i:i+51] = stats.ks_2samp(data1=bin_1_data, data2=bin_2_data).statistic
-        ttest_results[i:i+51] = stats.ttest_ind(bin_1_data, bin_2_data).statistic
-    for i in range(0, data.shape[0]-50, 50):
-        lillefors_results[i:i+51] = lilliefors(data[i:i+50])[0]
-        shapiro_results[i:i+51] = stats.shapiro(data[i:i+50])[0]
+        ks_results[i:i+fps+1] = stats.ks_2samp(data1=bin_1_data, data2=bin_2_data).statistic
+        t_test_results[i:i+fps+1] = stats.ttest_ind(bin_1_data, bin_2_data).statistic
+
+    for i in range(0, data.shape[0]-fps, fps):
+        lillefors_results[i:i+fps+1] = lilliefors(data[i:i+fps])[0]
+        shapiro_results[i:i+fps+1] = stats.shapiro(data[i:i+fps])[0]
+
+    rolling_idx = np.arange(fps)[None, :] + 1*np.arange(data.shape[0])[:, None]
     for i in range(rolling_idx.shape[0]):
         bin_start_idx, bin_end_idx = rolling_idx[i][0], rolling_idx[i][-1]
         peaks, _ = find_peaks(data[bin_start_idx:bin_end_idx], height=0)
         peak_cnt_results[i] = len(peaks)
 
-    columns = [f'{name}_KS', f'{name}_TTEST', f'{name}_LILLEFORS', f'{name}_SHAPIRO', f'{name}_PEAK_CNT']
-    return pd.DataFrame(np.column_stack((ks_results, ttest_results,
-                                        lillefors_results, shapiro_results, peak_cnt_results)), columns=columns)
+    columns = [f'{feature_name}_KS', f'{feature_name}_TTEST', f'{feature_name}_LILLEFORS', f'{feature_name}_SHAPIRO', f'{feature_name}_PEAK_CNT']
+    return pd.DataFrame(np.column_stack((ks_results, t_test_results,lillefors_results, shapiro_results, peak_cnt_results)), columns=columns).round(4)
 
 
-features = [f'Convex_hull_mean_25_window']
-DATA_PATH = '/Users/simon/Desktop/envs/troubleshooting/naresh/project_folder/csv/features_extracted/SF2.csv'
-data = pd.read_csv(DATA_PATH, index_col=0)
-for feature in features:
-    df = rolling_frequentist_distribution_tests(data=data[feature].astype(int).values, name=feature)
-    print(df)
+# features = [f'Convex_hull_mean_25_window']
+# DATA_PATH = '/Users/simon/Desktop/envs/troubleshooting/naresh/project_folder/csv/features_extracted/SF2.csv'
+# data = pd.read_csv(DATA_PATH, index_col=0)
+# for feature in features:
+#     df = rolling_frequentist_distribution_tests(data=data[feature].values,
+#                                                 feature_name=feature, fps=25)
+#     df.to_csv('Test.csv')
```

### Comparing `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/fish_feature_extractor_2022.py` & `Simba-UW-tf-dev-1.57.5/simba/feature_extractors/misc/fish_feature_extractor_2022.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/convex_hull_3_scratch_3.py` & `Simba-UW-tf-dev-1.57.5/simba/feature_extractors/misc/convex_hull_3_scratch_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/convex_hull_scratch_1.py` & `Simba-UW-tf-dev-1.57.5/simba/feature_extractors/misc/convex_hull_scratch_1.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/.DS_Store` & `Simba-UW-tf-dev-1.57.5/simba/feature_extractors/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py` & `Simba-UW-tf-dev-1.57.5/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/egocentrical_aligner.py` & `Simba-UW-tf-dev-1.57.5/simba/feature_extractors/misc/egocentrical_aligner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/count_values_in_range.py` & `Simba-UW-tf-dev-1.57.5/simba/feature_extractors/misc/count_values_in_range.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/graph_creator.py` & `Simba-UW-tf-dev-1.57.5/simba/feature_extractors/misc/graph_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/termite_rois.csv` & `Simba-UW-tf-dev-1.57.5/simba/feature_extractors/misc/termite_rois.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/mutual_exclusive.py` & `Simba-UW-tf-dev-1.57.5/simba/feature_extractors/misc/mutual_exclusive.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/video_color.py` & `Simba-UW-tf-dev-1.57.5/simba/feature_extractors/misc/video_color.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/graph_3d_plotter.py` & `Simba-UW-tf-dev-1.57.5/simba/feature_extractors/misc/graph_3d_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/video_rotator.py` & `Simba-UW-tf-dev-1.57.5/simba/feature_extractors/misc/video_rotator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/add_probability_cnt_features.py` & `Simba-UW-tf-dev-1.57.5/simba/feature_extractors/misc/add_probability_cnt_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/make_splash.py` & `Simba-UW-tf-dev-1.57.5/simba/feature_extractors/misc/make_splash.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/video_rotator_mp.py` & `Simba-UW-tf-dev-1.57.5/simba/feature_extractors/misc/video_rotator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py` & `Simba-UW-tf-dev-1.57.5/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from __future__ import division
 import numpy as np
 import math
 import pandas as pd
 from simba.read_config_unit_tests import (read_project_path_and_file_type,
                                           check_if_filepath_list_is_empty)
+from scipy import stats
+from statsmodels.stats.diagnostic import lilliefors
+from scipy.signal import find_peaks
 from scipy.spatial import ConvexHull
 from scipy.spatial.qhull import QhullError
 from scipy.stats import zscore
 from numba import jit, prange
 from simba.drop_bp_cords import *
 from simba.feature_extractors.unit_tests import read_video_info, check_minimum_roll_windows
 from simba.drop_bp_cords import get_fn_ext, getBpNames, getBpHeaders
@@ -63,15 +66,20 @@
             video_info, self.px_per_mm, self.fps = read_video_info(self.video_info_df, file_name)
             self.video_width, self.video_height = video_info['Resolution_width'].values, video_info['Resolution_height'].values
             self.angular_dispersion_windows = []
             for i in range(len(ANGULAR_DISPERSION_S)):
                 self.angular_dispersion_windows.append(int(self.fps * ANGULAR_DISPERSION_S[i]))
 
             self.csv_df = read_df(file_path, self.file_type).fillna(0).apply(pd.to_numeric)
-            self.csv_df.columns = self.bp_header_list
+            try:
+                self.csv_df.columns = self.bp_header_list
+            except ValueError:
+                msg = f'ERROR: Data contains the following fields: {self.csv_df.columns}. \n SimBA wants to use the following field names {self.bp_header_list}'
+                print(msg)
+                raise ValueError(msg)
 
             csv_df_shifted = self.csv_df.shift(periods=1)
             csv_df_shifted.columns = self.col_headers_shifted
             self.csv_df_combined = pd.concat([self.csv_df, csv_df_shifted], axis=1, join='inner').fillna(0)
             self.calc_X_relative_to_Y_movement()
             self.calc_movement()
             self.calc_X_relative_to_Y_movement_rolling_windows()
@@ -84,15 +92,15 @@
             self.hot_end_encode_compass()
             self.calc_directional_switches_in_rolling_windows()
             self.calc_angular_dispersion()
             self.calc_border_distances()
             self.calc_distances_between_body_part()
             self.calc_convex_hulls()
             self.pose_confidence_probabilities()
-            #self.kernel_density_estimations()
+            self.distribution_tests()
             self.save_file()
             video_timer.stop_timer()
             print(f'Features extracted for video {file_name} (elapsed time {video_timer.elapsed_time_str}s)...')
 
         self.timer.stop_timer()
         print(f'Features extracted for all {str(len(self.files_found))} files, data saved in project_folder/csv/features_extracted directory (elapsed time {self.timer.elapsed_time_str}s)')
 
@@ -150,14 +158,55 @@
     def angular_dispersion(cumsum_cos_np, cumsum_sin_np):
         out_array = np.empty((cumsum_cos_np.shape))
         for index in range(cumsum_cos_np.shape[0]):
             X, Y = cumsum_cos_np[index] / (index + 1), cumsum_sin_np[index] / (index + 1)
             out_array[index] = math.sqrt(X ** 2 + Y ** 2)
         return out_array
 
+
+    def windowed_frequentist_distribution_tests(self,
+                                                data: np.array,
+                                                feature_name: str,
+                                                fps: int):
+        """
+        Helper to compare feature value distributions in 1s sequential time-bins: Kolmogorov-Smirnov and T-tests
+        Compares the feature values against a normal distribution: Lillefors, Shapiro.
+        Find the number of peaks in *rolling* 1s long feature window.
+        """
+
+        ks_results, = np.full((data.shape[0]), -1.0),
+        t_test_results = np.full((data.shape[0]), -1.0)
+        lillefors_results = np.full((data.shape[0]), -1.0)
+        shapiro_results = np.full((data.shape[0]), -1.0)
+        peak_cnt_results = np.full((data.shape[0]), -1.0)
+
+        for i in range(fps, data.shape[0] - fps, fps):
+            bin_1_idx, bin_2_idx = [i - fps, i], [i, i + fps]
+            bin_1_data, bin_2_data = data[bin_1_idx[0]:bin_1_idx[1]], data[bin_2_idx[0]:bin_2_idx[1]]
+            ks_results[i:i + fps + 1] = stats.ks_2samp(data1=bin_1_data, data2=bin_2_data).statistic
+            t_test_results[i:i + fps + 1] = stats.ttest_ind(bin_1_data, bin_2_data).statistic
+
+        for i in range(0, data.shape[0] - fps, fps):
+            lillefors_results[i:i + fps + 1] = lilliefors(data[i:i + fps])[0]
+            shapiro_results[i:i + fps + 1] = stats.shapiro(data[i:i + fps])[0]
+
+        rolling_idx = np.arange(fps)[None, :] + 1 * np.arange(data.shape[0])[:, None]
+        for i in range(rolling_idx.shape[0]):
+            bin_start_idx, bin_end_idx = rolling_idx[i][0], rolling_idx[i][-1]
+            peaks, _ = find_peaks(data[bin_start_idx:bin_end_idx], height=0)
+            peak_cnt_results[i] = len(peaks)
+
+        columns = [f'{feature_name}_KS', f'{feature_name}_TTEST', f'{feature_name}_LILLEFORS',
+                   f'{feature_name}_SHAPIRO', f'{feature_name}_PEAK_CNT']
+        return pd.DataFrame(
+            np.column_stack((ks_results, t_test_results, lillefors_results, shapiro_results, peak_cnt_results)),
+            columns=columns).round(4)
+
+
+
     @staticmethod
     @jit(nopython=True)
     def consecutive_frames_in_same_compass_direction(direction: np.array):
         results = np.full((direction.shape[0], 1), -1)
         cnt, results[0], last_direction = 0, 0, direction[0]
         for i in prange(1, direction.shape[0]):
             if direction[i] == last_direction:
@@ -376,17 +425,30 @@
             self.csv_df_combined[f'Absolute_diff_min_max_convex_hull_{window}_window'] = abs(self.csv_df_combined[f'Convex_hull_min_{window}_window'] - self.csv_df_combined[f'Convex_hull_max_{window}_window'])
             try:
                 self.csv_df_combined[f'Convex_hull_skew_{window}'] = self.csv_df_combined['Convex_hull'].rolling(window, min_periods=1).skew()
                 self.csv_df_combined[f'Convex_hull_kurtosis_{window}'] = self.csv_df_combined['Convex_hull'].rolling(window, min_periods=1).kurt()
             except:
                 pass
 
-    # def find_peaks(self):
-    #     pass
 
+    def distribution_tests(self):
+        distribution_features = ['Mean_bp_distance_to_left_border',
+                                 'Mean_bp_distance_to_right_border',
+                                 'Mean_bp_distance_to_top_border',
+                                 'Mean_bp_distance_to_bottom_border',
+                                 'Bp_velocity_mean',
+                                 'Bp_acceleration_mean_25_window',
+                                 'Clockwise_angle_degrees',
+                                 'Convex_hull',
+                                 'Sum_probabilities',
+                                 'Consecutive_ms_in_same_compass_direction']
+
+        for feature_name in distribution_features:
+            results = self.windowed_frequentist_distribution_tests(data=self.csv_df_combined[feature_name].values, feature_name=feature_name, fps=int(self.fps))
+            self.csv_df_combined = pd.concat([self.csv_df_combined, results], axis=1)
 
     def pose_confidence_probabilities(self):
         self.csv_df_combined['Sum_probabilities'] = self.csv_df_combined[self.p_cols].sum(axis=1)
         self.csv_df_combined['Sum_probabilities_deviation'] = (self.csv_df_combined['Sum_probabilities'].mean() - self.csv_df_combined['Sum_probabilities'])
         p_brackets_results = pd.DataFrame(self.count_values_in_range(data=self.csv_df_combined.filter(self.p_cols).values, ranges=np.array([[0.0, 0.1], [0.000000000, 0.5], [0.000000000, 0.75], [0.000000000, 0.95], [0.000000000, 0.99]])), columns=['Low_prob_detections_0.1', 'Low_prob_detections_0.5', 'Low_prob_detections_0.75', 'Low_prob_detections_0.95', 'Low_prob_detections_0.99'])
         self.csv_df_combined = pd.concat([self.csv_df_combined, p_brackets_results], axis=1).reset_index(drop=True).fillna(0)
```

### Comparing `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/convex_hull_scratch_2.py` & `Simba-UW-tf-dev-1.57.5/simba/feature_extractors/misc/convex_hull_scratch_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/feature_extractor_8bps_2_animals.py` & `Simba-UW-tf-dev-1.57.5/simba/feature_extractors/feature_extractor_8bps_2_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/.DS_Store` & `Simba-UW-tf-dev-1.57.5/simba/feature_extractors/.DS_Store`

 * *Files 25% similar despite different names*

```diff
@@ -288,125 +288,125 @@
 000011f0: 6444 626c 6f62 0000 0008 0a8c 6973 23f2  dDblob......is#.
 00001200: c441 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 00001210: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
 00001220: 636f 6d70 0000 0000 000c 9000 0000 000b  comp............
 00001230: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00001240: 0065 005f 005f 7653 726e 6c6f 6e67 0000  .e._._vSrnlong..
 00001250: 0001 0000 0004 006d 0069 0073 0063 6277  .......m.i.s.cbw
-00001260: 7370 626c 6f62 0000 00ca 6270 6c69 7374  spblob....bplist
+00001260: 7370 626c 6f62 0000 00c8 6270 6c69 7374  spblob....bplist
 00001270: 3030 d701 0203 0405 0607 0808 0a08 0a0d  00..............
 00001280: 0a5d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
 00001290: 5368 6f77 5061 7468 6261 725b 5368 6f77  ShowPathbar[Show
 000012a0: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
 000012b0: 6965 775f 1014 436f 6e74 6169 6e65 7253  iew_..ContainerS
 000012c0: 686f 7753 6964 6562 6172 5c57 696e 646f  howSidebar\Windo
 000012d0: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
-000012e0: 6261 7208 0809 0809 5f10 197b 7b35 3039  bar....._..{{509
-000012f0: 2c20 3130 347d 2c20 7b31 3031 352c 2037  , 104}, {1015, 7
-00001300: 3637 7d7d 0908 1725 313d 4960 6d79 7a7b  67}}...%1=I`myz{
-00001310: 7c7d 7e9a 0000 0000 0000 0101 0000 0000  |}~.............
-00001320: 0000 000f 0000 0000 0000 0000 0000 0000  ................
-00001330: 0000 009b 0000 0004 006d 0069 0073 0063  .........m.i.s.c
-00001340: 6c67 3153 636f 6d70 0000 0000 0002 ee9a  lg1Scomp........
-00001350: 0000 0004 006d 0069 0073 0063 6c73 7643  .....m.i.s.clsvC
-00001360: 626c 6f62 0000 02b0 6270 6c69 7374 3030  blob....bplist00
-00001370: da01 0203 0405 0607 0809 0a0b 0c0d 1848  ...............H
-00001380: 4948 4a4b 0c5f 1012 7669 6577 4f70 7469  IHJK._..viewOpti
-00001390: 6f6e 7356 6572 7369 6f6e 5f10 0f73 686f  onsVersion_..sho
-000013a0: 7749 636f 6e50 7265 7669 6577 5763 6f6c  wIconPreviewWcol
-000013b0: 756d 6e73 5f10 1163 616c 6375 6c61 7465  umns_..calculate
-000013c0: 416c 6c53 697a 6573 5f10 0f73 6372 6f6c  AllSizes_..scrol
-000013d0: 6c50 6f73 6974 696f 6e59 5874 6578 7453  lPositionYXtextS
-000013e0: 697a 655f 100f 7363 726f 6c6c 506f 7369  ize_..scrollPosi
-000013f0: 7469 6f6e 585a 736f 7274 436f 6c75 6d6e  tionXZsortColumn
-00001400: 5869 636f 6e53 697a 655f 1010 7573 6552  XiconSize_..useR
-00001410: 656c 6174 6976 6544 6174 6573 1001 09ab  elativeDates....
-00001420: 0e17 1c21 252a 2f34 393e 43d4 0f10 1112  ...!%*/49>C.....
-00001430: 1314 0c0c 5a69 6465 6e74 6966 6965 7255  ....ZidentifierU
-00001440: 7769 6474 6859 6173 6365 6e64 696e 6757  widthYascendingW
-00001450: 7669 7369 626c 6554 6e61 6d65 1101 a609  visibleTname....
-00001460: 09d4 1210 110f 1819 181b 0810 2308 5875  ............#.Xu
-00001470: 6269 7175 6974 79d4 1210 110f 0c1e 1820  biquity........ 
-00001480: 0910 b508 5c64 6174 654d 6f64 6966 6965  ....\dateModifie
-00001490: 64d4 1210 110f 181e 1824 0808 5b64 6174  d........$..[dat
-000014a0: 6543 7265 6174 6564 d412 1011 0f0c 2718  eCreated......'.
-000014b0: 2909 1061 0854 7369 7a65 d412 1011 0f0c  )..a.Tsize......
-000014c0: 2c0c 2e09 1073 0954 6b69 6e64 d412 1011  ,....s.Tkind....
-000014d0: 0f18 310c 3308 1064 0955 6c61 6265 6cd4  ..1.3..d.Ulabel.
-000014e0: 1210 110f 1836 0c38 0810 4b09 5776 6572  .....6.8..K.Wver
-000014f0: 7369 6f6e d412 1011 0f18 3b0c 3d08 1101  sion......;.=...
-00001500: 2c09 5863 6f6d 6d65 6e74 73d4 1210 110f  ,.Xcomments.....
-00001510: 1840 1842 0810 c808 5e64 6174 654c 6173  .@.B....^dateLas
-00001520: 744f 7065 6e65 64d4 1210 110f 181e 1846  tOpened........F
-00001530: 0808 5964 6174 6541 6464 6564 0823 0000  ..YdateAdded.#..
-00001540: 0000 0000 0000 2340 2800 0000 0000 0054  ......#@(......T
-00001550: 6e61 6d65 2340 3000 0000 0000 0009 0008  name#@0.........
-00001560: 001d 0032 0044 004c 0060 0072 007b 008d  ...2.D.L.`.r.{..
-00001570: 0098 00a1 00b4 00b6 00b7 00c3 00cc 00d7  ................
-00001580: 00dd 00e7 00ef 00f4 00f7 00f8 00f9 0102  ................
-00001590: 0103 0105 0106 010f 0118 0119 011b 011c  ................
-000015a0: 0129 0132 0133 0134 0140 0149 014a 014c  .).2.3.4.@.I.J.L
-000015b0: 014d 0152 015b 015c 015e 015f 0164 016d  .M.R.[.\.^._.d.m
-000015c0: 016e 0170 0171 0177 0180 0181 0183 0184  .n.p.q.w........
-000015d0: 018c 0195 0196 0199 019a 01a3 01ac 01ad  ................
-000015e0: 01af 01b0 01bf 01c8 01c9 01ca 01d4 01d5  ................
-000015f0: 01de 01e7 01ec 01f5 0000 0000 0000 0201  ................
-00001600: 0000 0000 0000 004d 0000 0000 0000 0000  .......M........
-00001610: 0000 0000 0000 01f6 0000 0004 006d 0069  .............m.i
-00001620: 0073 0063 6c73 7670 626c 6f62 0000 0295  .s.clsvpblob....
-00001630: 6270 6c69 7374 3030 da01 0203 0405 0607  bplist00........
-00001640: 0809 0a0b 0c0d 1f47 4847 494a 0c5f 1012  .......GHGIJ._..
-00001650: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
-00001660: 6f6e 5f10 0f73 686f 7749 636f 6e50 7265  on_..showIconPre
-00001670: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
-00001680: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
-00001690: 5f10 0f73 6372 6f6c 6c50 6f73 6974 696f  _..scrollPositio
-000016a0: 6e59 5874 6578 7453 697a 655f 100f 7363  nYXtextSize_..sc
-000016b0: 726f 6c6c 506f 7369 7469 6f6e 585a 736f  rollPositionXZso
-000016c0: 7274 436f 6c75 6d6e 5869 636f 6e53 697a  rtColumnXiconSiz
-000016d0: 655f 1010 7573 6552 656c 6174 6976 6544  e_..useRelativeD
-000016e0: 6174 6573 1001 09d9 0e0f 1011 1213 1415  ates............
-000016f0: 1617 2025 292d 3237 3c41 5863 6f6d 6d65  .. %)-27<AXcomme
-00001700: 6e74 735e 6461 7465 4c61 7374 4f70 656e  nts^dateLastOpen
-00001710: 6564 5c64 6174 654d 6f64 6966 6965 645b  ed\dateModified[
-00001720: 6461 7465 4372 6561 7465 6454 7369 7a65  dateCreatedTsize
-00001730: 556c 6162 656c 546b 696e 6457 7665 7273  UlabelTkindWvers
-00001740: 696f 6e54 6e61 6d65 d418 191a 1b1c 1d0c  ionTname........
-00001750: 1f55 696e 6465 7855 7769 6474 6859 6173  .UindexUwidthYas
-00001760: 6365 6e64 696e 6757 7669 7369 626c 6510  cendingWvisible.
-00001770: 0711 012c 0908 d418 191a 1b21 221f 1f10  ...,.......!"...
-00001780: 0810 c808 08d4 1819 1a1b 0b26 1f0c 10b5  ...........&....
-00001790: 0809 d418 191a 1b2a 261f 1f10 0208 08d4  .......*&.......
-000017a0: 1819 1a1b 2e2f 1f0c 1003 1061 0809 d418  ...../.....a....
-000017b0: 191a 1b33 340c 1f10 0510 6409 08d4 1819  ...34.....d.....
-000017c0: 1a1b 3839 0c0c 1004 1073 0909 d418 191a  ..89.....s......
-000017d0: 1b3d 3e0c 1f10 0610 4b09 08d4 1b19 1a18  .=>.....K.......
-000017e0: 0c43 0c45 0911 01a6 0910 0008 2300 0000  .C.E........#...
-000017f0: 0000 0000 0023 4028 0000 0000 0000 546e  .....#@(......Tn
-00001800: 616d 6523 4030 0000 0000 0000 0900 0800  ame#@0..........
-00001810: 1d00 3200 4400 4c00 6000 7200 7b00 8d00  ..2.D.L.`.r.{...
-00001820: 9800 a100 b400 b600 b700 ca00 d300 e200  ................
-00001830: ef00 fb01 0001 0601 0b01 1301 1801 2101  ..............!.
-00001840: 2701 2d01 3701 3f01 4101 4401 4501 4601  '.-.7.?.A.D.E.F.
-00001850: 4f01 5101 5301 5401 5501 5e01 6001 6101  O.Q.S.T.U.^.`.a.
-00001860: 6201 6b01 6d01 6e01 6f01 7801 7a01 7c01  b.k.m.n.o.x.z.|.
-00001870: 7d01 7e01 8701 8901 8b01 8c01 8d01 9601  }.~.............
-00001880: 9801 9a01 9b01 9c01 a501 a701 a901 aa01  ................
-00001890: ab01 b401 b501 b801 b901 bb01 bc01 c501  ................
-000018a0: ce01 d301 dc00 0000 0000 0002 0100 0000  ................
-000018b0: 0000 0000 4c00 0000 0000 0000 0000 0000  ....L...........
-000018c0: 0000 0001 dd00 0000 0400 6d00 6900 7300  ..........m.i.s.
-000018d0: 636d 6f44 4462 6c6f 6200 0000 0824 9c16  cmoDDblob....$..
-000018e0: 85e9 f8c4 4100 0000 0400 6d00 6900 7300  ....A.....m.i.s.
-000018f0: 636d 6f64 4462 6c6f 6200 0000 0824 9c16  cmodDblob....$..
-00001900: 85e9 f8c4 4100 0000 0400 6d00 6900 7300  ....A.....m.i.s.
-00001910: 6370 6831 5363 6f6d 7000 0000 0000 03e0  cph1Scomp.......
-00001920: 0000 0000 0400 6d00 6900 7300 6376 5372  ......m.i.s.cvSr
-00001930: 6e6c 6f6e 6700 0000 0100 0000 0000 0000  nlong...........
-00001940: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000012e0: 6261 7208 0809 0809 5f10 177b 7b33 342c  bar....._..{{34,
+000012f0: 2039 307d 2c20 7b31 3031 352c 2037 3637   90}, {1015, 767
+00001300: 7d7d 0908 1725 313d 4960 6d79 7a7b 7c7d  }}...%1=I`myz{|}
+00001310: 7e98 0000 0000 0000 0101 0000 0000 0000  ~...............
+00001320: 000f 0000 0000 0000 0000 0000 0000 0000  ................
+00001330: 0099 0000 0004 006d 0069 0073 0063 6c67  .......m.i.s.clg
+00001340: 3153 636f 6d70 0000 0000 0003 0365 0000  1Scomp.......e..
+00001350: 0004 006d 0069 0073 0063 6c73 7643 626c  ...m.i.s.clsvCbl
+00001360: 6f62 0000 02b8 6270 6c69 7374 3030 da01  ob....bplist00..
+00001370: 0203 0405 0607 0809 0a0b 0c0d 1848 4948  .............HIH
+00001380: 4a0c 4c58 6963 6f6e 5369 7a65 5f10 0f73  J.LXiconSize_..s
+00001390: 686f 7749 636f 6e50 7265 7669 6577 5763  howIconPreviewWc
+000013a0: 6f6c 756d 6e73 5f10 1163 616c 6375 6c61  olumns_..calcula
+000013b0: 7465 416c 6c53 697a 6573 5f10 0f73 6372  teAllSizes_..scr
+000013c0: 6f6c 6c50 6f73 6974 696f 6e59 5874 6578  ollPositionYXtex
+000013d0: 7453 697a 655f 100f 7363 726f 6c6c 506f  tSize_..scrollPo
+000013e0: 7369 7469 6f6e 585a 736f 7274 436f 6c75  sitionXZsortColu
+000013f0: 6d6e 5f10 1075 7365 5265 6c61 7469 7665  mn_..useRelative
+00001400: 4461 7465 735f 1012 7669 6577 4f70 7469  Dates_..viewOpti
+00001410: 6f6e 7356 6572 7369 6f6e 2340 3000 0000  onsVersion#@0...
+00001420: 0000 0009 ab0e 171c 2125 2a2f 3439 3e43  ........!%*/49>C
+00001430: d40f 1011 1213 140c 0c5a 6964 656e 7469  .........Zidenti
+00001440: 6669 6572 5577 6964 7468 5961 7363 656e  fierUwidthYascen
+00001450: 6469 6e67 5776 6973 6962 6c65 546e 616d  dingWvisibleTnam
+00001460: 6511 01a6 0909 d412 1011 0f18 1918 1b08  e...............
+00001470: 1023 0858 7562 6971 7569 7479 d412 1011  .#.Xubiquity....
+00001480: 0f0c 1e18 2009 10b5 085c 6461 7465 4d6f  .... ....\dateMo
+00001490: 6469 6669 6564 d412 1011 0f18 1e18 2408  dified........$.
+000014a0: 085b 6461 7465 4372 6561 7465 64d4 1210  .[dateCreated...
+000014b0: 110f 0c27 1829 0910 6108 5473 697a 65d4  ...'.)..a.Tsize.
+000014c0: 1210 110f 0c2c 0c2e 0910 7309 546b 696e  .....,....s.Tkin
+000014d0: 64d4 1210 110f 1831 0c33 0810 6409 556c  d......1.3..d.Ul
+000014e0: 6162 656c d412 1011 0f18 360c 3808 104b  abel......6.8..K
+000014f0: 0957 7665 7273 696f 6ed4 1210 110f 183b  .Wversion......;
+00001500: 0c3d 0811 012c 0958 636f 6d6d 656e 7473  .=...,.Xcomments
+00001510: d412 1011 0f18 4018 4208 10c8 085e 6461  ......@.B....^da
+00001520: 7465 4c61 7374 4f70 656e 6564 d412 1011  teLastOpened....
+00001530: 0f18 1e18 4608 0859 6461 7465 4164 6465  ....F..YdateAdde
+00001540: 6408 2300 0000 0000 0000 0023 4028 0000  d.#........#@(..
+00001550: 0000 0000 5c64 6174 654d 6f64 6966 6965  ....\dateModifie
+00001560: 6409 1001 0008 001d 0026 0038 0040 0054  d........&.8.@.T
+00001570: 0066 006f 0081 008c 009f 00b4 00bd 00be  .f.o............
+00001580: 00ca 00d3 00de 00e4 00ee 00f6 00fb 00fe  ................
+00001590: 00ff 0100 0109 010a 010c 010d 0116 011f  ................
+000015a0: 0120 0122 0123 0130 0139 013a 013b 0147  . .".#.0.9.:.;.G
+000015b0: 0150 0151 0153 0154 0159 0162 0163 0165  .P.Q.S.T.Y.b.c.e
+000015c0: 0166 016b 0174 0175 0177 0178 017e 0187  .f.k.t.u.w.x.~..
+000015d0: 0188 018a 018b 0193 019c 019d 01a0 01a1  ................
+000015e0: 01aa 01b3 01b4 01b6 01b7 01c6 01cf 01d0  ................
+000015f0: 01d1 01db 01dc 01e5 01ee 01fb 01fc 0000  ................
+00001600: 0000 0000 0201 0000 0000 0000 004d 0000  .............M..
+00001610: 0000 0000 0000 0000 0000 0000 01fe 0000  ................
+00001620: 0004 006d 0069 0073 0063 6c73 7670 626c  ...m.i.s.clsvpbl
+00001630: 6f62 0000 029d 6270 6c69 7374 3030 da01  ob....bplist00..
+00001640: 0203 0405 0607 0809 0a0b 0c0d 1f48 4948  .............HIH
+00001650: 4a0c 2658 6963 6f6e 5369 7a65 5f10 0f73  J.&XiconSize_..s
+00001660: 686f 7749 636f 6e50 7265 7669 6577 5763  howIconPreviewWc
+00001670: 6f6c 756d 6e73 5f10 1163 616c 6375 6c61  olumns_..calcula
+00001680: 7465 416c 6c53 697a 6573 5f10 0f73 6372  teAllSizes_..scr
+00001690: 6f6c 6c50 6f73 6974 696f 6e59 5874 6578  ollPositionYXtex
+000016a0: 7453 697a 655f 100f 7363 726f 6c6c 506f  tSize_..scrollPo
+000016b0: 7369 7469 6f6e 585a 736f 7274 436f 6c75  sitionXZsortColu
+000016c0: 6d6e 5f10 1075 7365 5265 6c61 7469 7665  mn_..useRelative
+000016d0: 4461 7465 735f 1012 7669 6577 4f70 7469  Dates_..viewOpti
+000016e0: 6f6e 7356 6572 7369 6f6e 2340 3000 0000  onsVersion#@0...
+000016f0: 0000 0009 d90e 0f10 1112 1314 1516 1720  ............... 
+00001700: 252a 2e33 383d 4258 636f 6d6d 656e 7473  %*.38=BXcomments
+00001710: 5e64 6174 654c 6173 744f 7065 6e65 645c  ^dateLastOpened\
+00001720: 6461 7465 4d6f 6469 6669 6564 5b64 6174  dateModified[dat
+00001730: 6543 7265 6174 6564 5473 697a 6555 6c61  eCreatedTsizeUla
+00001740: 6265 6c54 6b69 6e64 5776 6572 7369 6f6e  belTkindWversion
+00001750: 546e 616d 65d4 1819 1a1b 1c1d 0c1f 5569  Tname.........Ui
+00001760: 6e64 6578 5577 6964 7468 5961 7363 656e  ndexUwidthYascen
+00001770: 6469 6e67 5776 6973 6962 6c65 1007 1101  dingWvisible....
+00001780: 2c09 08d4 1819 1a1b 2122 1f1f 1008 10c8  ,.......!"......
+00001790: 0808 d418 191a 1b26 271f 0c10 0110 b508  .......&'.......
+000017a0: 09d4 1819 1a1b 2b27 1f1f 1002 0808 d418  ......+'........
+000017b0: 191a 1b2f 301f 0c10 0310 6108 09d4 1819  .../0.....a.....
+000017c0: 1a1b 3435 0c1f 1005 1064 0908 d418 191a  ..45.....d......
+000017d0: 1b39 3a0c 0c10 0410 7309 09d4 1819 1a1b  .9:.....s.......
+000017e0: 3e3f 0c1f 1006 104b 0908 d41b 191a 180c  >?.....K........
+000017f0: 440c 4609 1101 a609 1000 0823 0000 0000  D.F........#....
+00001800: 0000 0000 2340 2800 0000 0000 005c 6461  ....#@(......\da
+00001810: 7465 4d6f 6469 6669 6564 0900 0800 1d00  teModified......
+00001820: 2600 3800 4000 5400 6600 6f00 8100 8c00  &.8.@.T.f.o.....
+00001830: 9f00 b400 bd00 be00 d100 da00 e900 f601  ................
+00001840: 0201 0701 0d01 1201 1a01 1f01 2801 2e01  ............(...
+00001850: 3401 3e01 4601 4801 4b01 4c01 4d01 5601  4.>.F.H.K.L.M.V.
+00001860: 5801 5a01 5b01 5c01 6501 6701 6901 6a01  X.Z.[.\.e.g.i.j.
+00001870: 6b01 7401 7601 7701 7801 8101 8301 8501  k.t.v.w.x.......
+00001880: 8601 8701 9001 9201 9401 9501 9601 9f01  ................
+00001890: a101 a301 a401 a501 ae01 b001 b201 b301  ................
+000018a0: b401 bd01 be01 c101 c201 c401 c501 ce01  ................
+000018b0: d701 e400 0000 0000 0002 0100 0000 0000  ................
+000018c0: 0000 4c00 0000 0000 0000 0000 0000 0000  ..L.............
+000018d0: 0001 e500 0000 0400 6d00 6900 7300 636d  ........m.i.s.cm
+000018e0: 6f44 4462 6c6f 6200 0000 08e7 9910 0635  oDDblob........5
+000018f0: fac4 4100 0000 0400 6d00 6900 7300 636d  ..A.....m.i.s.cm
+00001900: 6f64 4462 6c6f 6200 0000 08e7 9910 0635  odDblob........5
+00001910: fac4 4100 0000 0400 6d00 6900 7300 6370  ..A.....m.i.s.cp
+00001920: 6831 5363 6f6d 7000 0000 0000 0400 0000  h1Scomp.........
+00001930: 0000 0400 6d00 6900 7300 6376 5372 6e6c  ....m.i.s.cvSrnl
+00001940: 6f6e 6700 0000 0100 0000 0000 0000 0000  ong.............
 00001950: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001960: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001970: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001980: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001990: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000019a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000019b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -586,56 +586,56 @@
 00002490: 0100 0200 0000 0000 0100 0400 0000 0000  ................
 000024a0: 0100 0800 0000 0000 0100 1000 0000 0000  ................
 000024b0: 0100 2000 0000 0000 0100 4000 0000 0000  .. .......@.....
 000024c0: 0100 8000 0000 0000 0101 0000 0000 0000  ................
 000024d0: 0102 0000 0000 0000 0104 0000 0000 0000  ................
 000024e0: 0108 0000 0000 0000 0110 0000 0000 0000  ................
 000024f0: 0120 0000 0000 0000 0140 0000 0000 0000  . .......@......
-00002500: 0009 5863 6f6d 6d65 6e74 73d4 1210 110f  ..Xcomments.....
-00002510: 1840 1842 0810 c808 5e64 6174 654c 6173  .@.B....^dateLas
-00002520: 744f 7065 6e65 64d4 1210 110f 181e 1846  tOpened........F
-00002530: 0808 5964 6174 6541 6464 6564 0823 0000  ..YdateAdded.#..
-00002540: 0000 0000 0000 2340 2800 0000 0000 0054  ......#@(......T
-00002550: 6e61 6d65 2340 3000 0000 0000 0009 0008  name#@0.........
-00002560: 001d 0032 0044 004c 0060 0072 007b 008d  ...2.D.L.`.r.{..
-00002570: 0098 00a1 00b4 00b6 00b7 00c3 00cc 00d7  ................
-00002580: 00dd 00e7 00ef 00f4 00f7 00f8 00f9 0102  ................
-00002590: 0103 0105 0106 010f 0118 0119 011b 011c  ................
-000025a0: 0129 0132 0133 0134 0140 0149 014a 014c  .).2.3.4.@.I.J.L
-000025b0: 014d 0152 015b 015c 015e 015f 0164 016d  .M.R.[.\.^._.d.m
-000025c0: 016e 0170 0171 0177 0180 0181 0183 0184  .n.p.q.w........
-000025d0: 018c 0195 0196 0199 019a 01a3 01ac 01ad  ................
-000025e0: 01af 01b0 01bf 01c8 01c9 01ca 01d4 01d5  ................
-000025f0: 01de 01e7 01ec 01f5 0000 0000 0000 0201  ................
-00002600: 0000 0000 0000 004d 0000 0000 0000 0000  .......M........
-00002610: 0000 0000 0000 01f6 0000 0004 006d 0069  .............m.i
-00002620: 0073 0063 6c73 7670 626c 6f62 0000 0295  .s.clsvpblob....
-00002630: 6270 6c69 7374 3030 da01 0203 0405 0607  bplist00........
-00002640: 0809 0a0b 0c0d 1f47 4847 494a 0c5f 1012  .......GHGIJ._..
-00002650: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
-00002660: 6f6e 5f10 0f73 686f 7749 636f 6e50 7265  on_..showIconPre
-00002670: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
-00002680: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
-00002690: 5f10 0f73 6372 6f6c 6c50 6f73 6974 696f  _..scrollPositio
-000026a0: 6e59 5874 6578 7453 697a 655f 100f 7363  nYXtextSize_..sc
-000026b0: 726f 6c6c 506f 7369 7469 6f6e 585a 736f  rollPositionXZso
-000026c0: 7274 436f 6c75 6d6e 5869 636f 6e53 697a  rtColumnXiconSiz
-000026d0: 655f 1010 7573 6552 656c 6174 6976 6544  e_..useRelativeD
-000026e0: 6174 6573 1001 09d9 0e0f 1011 1213 1415  ates............
-000026f0: 1617 2025 292d 3237 3c41 5863 6f6d 6d65  .. %)-27<AXcomme
-00002700: 6e74 735e 6461 7465 4c61 7374 4f70 656e  nts^dateLastOpen
-00002710: 6564 5c64 6174 654d 6f64 6966 6965 645b  ed\dateModified[
-00002720: 6461 7465 4372 6561 7465 6454 7369 7a65  dateCreatedTsize
-00002730: 556c 6162 656c 546b 696e 6457 7665 7273  UlabelTkindWvers
-00002740: 696f 6e54 6e61 6d65 d418 191a 1b1c 1d0c  ionTname........
-00002750: 1f55 696e 6465 7855 7769 6474 6859 6173  .UindexUwidthYas
-00002760: 6365 6e64 696e 6757 7669 7369 626c 6510  cendingWvisible.
-00002770: 0711 012c 0908 d418 191a 1b21 221f 1f10  ...,.......!"...
-00002780: 0810 c808 08d4 1819 1a1b 0b26 1f0c 10b5  ...........&....
-00002790: 0809 d418 191a 1b2a 261f 1f10 0208 08d4  .......*&.......
-000027a0: 1819 1a1b 2e2f 1f0c 1003 1061 0809 d418  ...../.....a....
-000027b0: 191a 1b33 340c 1f10 0510 6409 08d4 1819  ...34.....d.....
-000027c0: 1a1b 3839 0c0c 1004 1073 0909 d418 191a  ..89.....s......
-000027d0: 1b3d 3e0c 1f10 0610 4b09 08d4 1b19 1a18  .=>.....K.......
-000027e0: 0c43 0c45 0911 01a6 0910 0008 2300 0000  .C.E........#...
-000027f0: 0000 0000 0023 4028 0000 0000 0000 546e  .....#@(......Tn
-00002800: 616d 6523                                ame#
+00002500: 003d 0811 012c 0958 636f 6d6d 656e 7473  .=...,.Xcomments
+00002510: d412 1011 0f18 4018 4208 10c8 085e 6461  ......@.B....^da
+00002520: 7465 4c61 7374 4f70 656e 6564 d412 1011  teLastOpened....
+00002530: 0f18 1e18 4608 0859 6461 7465 4164 6465  ....F..YdateAdde
+00002540: 6408 2300 0000 0000 0000 0023 4028 0000  d.#........#@(..
+00002550: 0000 0000 5c64 6174 654d 6f64 6966 6965  ....\dateModifie
+00002560: 6409 1001 0008 001d 0026 0038 0040 0054  d........&.8.@.T
+00002570: 0066 006f 0081 008c 009f 00b4 00bd 00be  .f.o............
+00002580: 00ca 00d3 00de 00e4 00ee 00f6 00fb 00fe  ................
+00002590: 00ff 0100 0109 010a 010c 010d 0116 011f  ................
+000025a0: 0120 0122 0123 0130 0139 013a 013b 0147  . .".#.0.9.:.;.G
+000025b0: 0150 0151 0153 0154 0159 0162 0163 0165  .P.Q.S.T.Y.b.c.e
+000025c0: 0166 016b 0174 0175 0177 0178 017e 0187  .f.k.t.u.w.x.~..
+000025d0: 0188 018a 018b 0193 019c 019d 01a0 01a1  ................
+000025e0: 01aa 01b3 01b4 01b6 01b7 01c6 01cf 01d0  ................
+000025f0: 01d1 01db 01dc 01e5 01ee 01fb 01fc 0000  ................
+00002600: 0000 0000 0201 0000 0000 0000 004d 0000  .............M..
+00002610: 0000 0000 0000 0000 0000 0000 01fe 0000  ................
+00002620: 0004 006d 0069 0073 0063 6c73 7670 626c  ...m.i.s.clsvpbl
+00002630: 6f62 0000 029d 6270 6c69 7374 3030 da01  ob....bplist00..
+00002640: 0203 0405 0607 0809 0a0b 0c0d 1f48 4948  .............HIH
+00002650: 4a0c 2658 6963 6f6e 5369 7a65 5f10 0f73  J.&XiconSize_..s
+00002660: 686f 7749 636f 6e50 7265 7669 6577 5763  howIconPreviewWc
+00002670: 6f6c 756d 6e73 5f10 1163 616c 6375 6c61  olumns_..calcula
+00002680: 7465 416c 6c53 697a 6573 5f10 0f73 6372  teAllSizes_..scr
+00002690: 6f6c 6c50 6f73 6974 696f 6e59 5874 6578  ollPositionYXtex
+000026a0: 7453 697a 655f 100f 7363 726f 6c6c 506f  tSize_..scrollPo
+000026b0: 7369 7469 6f6e 585a 736f 7274 436f 6c75  sitionXZsortColu
+000026c0: 6d6e 5f10 1075 7365 5265 6c61 7469 7665  mn_..useRelative
+000026d0: 4461 7465 735f 1012 7669 6577 4f70 7469  Dates_..viewOpti
+000026e0: 6f6e 7356 6572 7369 6f6e 2340 3000 0000  onsVersion#@0...
+000026f0: 0000 0009 d90e 0f10 1112 1314 1516 1720  ............... 
+00002700: 252a 2e33 383d 4258 636f 6d6d 656e 7473  %*.38=BXcomments
+00002710: 5e64 6174 654c 6173 744f 7065 6e65 645c  ^dateLastOpened\
+00002720: 6461 7465 4d6f 6469 6669 6564 5b64 6174  dateModified[dat
+00002730: 6543 7265 6174 6564 5473 697a 6555 6c61  eCreatedTsizeUla
+00002740: 6265 6c54 6b69 6e64 5776 6572 7369 6f6e  belTkindWversion
+00002750: 546e 616d 65d4 1819 1a1b 1c1d 0c1f 5569  Tname.........Ui
+00002760: 6e64 6578 5577 6964 7468 5961 7363 656e  ndexUwidthYascen
+00002770: 6469 6e67 5776 6973 6962 6c65 1007 1101  dingWvisible....
+00002780: 2c09 08d4 1819 1a1b 2122 1f1f 1008 10c8  ,.......!"......
+00002790: 0808 d418 191a 1b26 271f 0c10 0110 b508  .......&'.......
+000027a0: 09d4 1819 1a1b 2b27 1f1f 1002 0808 d418  ......+'........
+000027b0: 191a 1b2f 301f 0c10 0310 6108 09d4 1819  .../0.....a.....
+000027c0: 1a1b 3435 0c1f 1005 1064 0908 d418 191a  ..45.....d......
+000027d0: 1b39 3a0c 0c10 0410 7309 09d4 1819 1a1b  .9:.....s.......
+000027e0: 3e3f 0c1f 1006 104b 0908 d41b 191a 180c  >?.....K........
+000027f0: 440c 4609 1101 a609 1000 0823 0000 0000  D.F........#....
+00002800: 0000 0000                                ....
```

### Comparing `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/perimeter_jit.py` & `Simba-UW-tf-dev-1.57.5/simba/feature_extractors/perimeter_jit.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/feature_subsets.py` & `Simba-UW-tf-dev-1.57.5/simba/feature_extractors/feature_subsets.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi` & `Simba-UW-tf-dev-1.57.5/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc` & `Simba-UW-tf-dev-1.57.5/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc` & `Simba-UW-tf-dev-1.57.5/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc` & `Simba-UW-tf-dev-1.57.5/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc` & `Simba-UW-tf-dev-1.57.5/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi` & `Simba-UW-tf-dev-1.57.5/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi` & `Simba-UW-tf-dev-1.57.5/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/extract_features_9bp.py` & `Simba-UW-tf-dev-1.57.5/simba/feature_extractors/extract_features_9bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/feature_extractor_user_defined.py` & `Simba-UW-tf-dev-1.57.5/simba/feature_extractors/feature_extractor_user_defined.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/unit_tests.py` & `Simba-UW-tf-dev-1.57.5/simba/feature_extractors/unit_tests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/feature_extractor_16bp.py` & `Simba-UW-tf-dev-1.57.5/simba/feature_extractors/feature_extractor_16bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/feature_extractor_8bp.py` & `Simba-UW-tf-dev-1.57.5/simba/feature_extractors/feature_extractor_8bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/feature_extractor_4bp.py` & `Simba-UW-tf-dev-1.57.5/simba/feature_extractors/feature_extractor_4bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/.idea/features_scripts.iml` & `Simba-UW-tf-dev-1.57.5/simba/feature_extractors/.idea/features_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.57.5/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/.idea/workspace.xml` & `Simba-UW-tf-dev-1.57.5/simba/feature_extractors/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/plotly_create_h5.py` & `Simba-UW-tf-dev-1.57.5/simba/plotly_create_h5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/requirements.txt` & `Simba-UW-tf-dev-1.57.5/simba/requirements.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/severity_processor.py` & `Simba-UW-tf-dev-1.57.5/simba/severity_processor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/user_pose_config_creator.py` & `Simba-UW-tf-dev-1.57.5/simba/user_pose_config_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/mixins/.DS_Store` & `Simba-UW-tf-dev-1.57.5/simba/mixins/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/mixins/pop_up_mixin.py` & `Simba-UW-tf-dev-1.57.5/simba/mixins/pop_up_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/mixins/config_reader.py` & `Simba-UW-tf-dev-1.57.5/simba/mixins/config_reader.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/mixins/feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.57.5/simba/mixins/feature_extraction_mixin.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 import numpy as np
 from numba import jit, prange
 from scipy.spatial import ConvexHull
 from scipy.spatial.qhull import QhullError
 import math
 import os, glob
+from scipy import stats
+from statsmodels.stats.diagnostic import lilliefors
+import pandas as pd
+from scipy.signal import find_peaks
 from simba.enums import Paths, Options, ReadConfig, Dtypes
 from simba.feature_extractors.unit_tests import (read_video_info_csv,
                                                check_minimum_roll_windows)
 from simba.read_config_unit_tests import (read_config_file,
                                           read_config_entry,
                                           read_project_path_and_file_type,
                                           check_if_filepath_list_is_empty)
@@ -135,8 +139,46 @@
                         xints = (y - p1y) * (p2x - p1x) / (p2y - p1y) + p1x
                     if p1x == p2x or x <= xints:
                         inside = not inside
                 p1x, p1y = p2x, p2y
             if inside:
                 results[i] = 1
 
-        return results
+        return results
+
+    def windowed_frequentist_distribution_tests(self,
+                                                data: np.array,
+                                                feature_name: str,
+                                                fps: int):
+        """
+        Helper to compare feature value distributions in 1s sequential time-bins: Kolmogorov-Smirnov and T-tests
+        Compares the feature values against a normal distribution: Lillefors, Shapiro.
+        Find the number of peaks in *rolling* 1s long feature window.
+        """
+
+        ks_results, = np.full((data.shape[0]), -1.0),
+        t_test_results = np.full((data.shape[0]), -1.0)
+        lillefors_results = np.full((data.shape[0]), -1.0)
+        shapiro_results = np.full((data.shape[0]), -1.0)
+        peak_cnt_results = np.full((data.shape[0]), -1.0)
+
+        for i in range(fps, data.shape[0] - fps, fps):
+            bin_1_idx, bin_2_idx = [i - fps, i], [i, i + fps]
+            bin_1_data, bin_2_data = data[bin_1_idx[0]:bin_1_idx[1]], data[bin_2_idx[0]:bin_2_idx[1]]
+            ks_results[i:i + fps + 1] = stats.ks_2samp(data1=bin_1_data, data2=bin_2_data).statistic
+            t_test_results[i:i + fps + 1] = stats.ttest_ind(bin_1_data, bin_2_data).statistic
+
+        for i in range(0, data.shape[0] - fps, fps):
+            lillefors_results[i:i + fps + 1] = lilliefors(data[i:i + fps])[0]
+            shapiro_results[i:i + fps + 1] = stats.shapiro(data[i:i + fps])[0]
+
+        rolling_idx = np.arange(fps)[None, :] + 1 * np.arange(data.shape[0])[:, None]
+        for i in range(rolling_idx.shape[0]):
+            bin_start_idx, bin_end_idx = rolling_idx[i][0], rolling_idx[i][-1]
+            peaks, _ = find_peaks(data[bin_start_idx:bin_end_idx], height=0)
+            peak_cnt_results[i] = len(peaks)
+
+        columns = [f'{feature_name}_KS', f'{feature_name}_TTEST', f'{feature_name}_LILLEFORS',
+                   f'{feature_name}_SHAPIRO', f'{feature_name}_PEAK_CNT']
+        return pd.DataFrame(
+            np.column_stack((ks_results, t_test_results, lillefors_results, shapiro_results, peak_cnt_results)),
+            columns=columns).round(4)
```

### Comparing `Simba-UW-tf-dev-1.57.4/simba/mixins/unsupervised_mixin.py` & `Simba-UW-tf-dev-1.57.5/simba/mixins/unsupervised_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/machine_model_settings_pop_up.py` & `Simba-UW-tf-dev-1.57.5/simba/machine_model_settings_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/remove_keypoints_in_pose.py` & `Simba-UW-tf-dev-1.57.5/simba/remove_keypoints_in_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/third_party_label_appenders/deepethogram_importer.py` & `Simba-UW-tf-dev-1.57.5/simba/third_party_label_appenders/deepethogram_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/third_party_label_appenders/BORIS_appender.py` & `Simba-UW-tf-dev-1.57.5/simba/third_party_label_appenders/BORIS_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/third_party_label_appenders/observer_importer.py` & `Simba-UW-tf-dev-1.57.5/simba/third_party_label_appenders/observer_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/third_party_label_appenders/tools.py` & `Simba-UW-tf-dev-1.57.5/simba/third_party_label_appenders/tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/third_party_label_appenders/third_party_appender.py` & `Simba-UW-tf-dev-1.57.5/simba/third_party_label_appenders/third_party_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/third_party_label_appenders/ethovision_import.py` & `Simba-UW-tf-dev-1.57.5/simba/third_party_label_appenders/ethovision_import.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/third_party_label_appenders/BENTO_appender.py` & `Simba-UW-tf-dev-1.57.5/simba/third_party_label_appenders/BENTO_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/third_party_label_appenders/solomon_importer.py` & `Simba-UW-tf-dev-1.57.5/simba/third_party_label_appenders/solomon_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/multi_cropper.py` & `Simba-UW-tf-dev-1.57.5/simba/multi_cropper.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/FSTTC_calculator.py` & `Simba-UW-tf-dev-1.57.5/simba/FSTTC_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/create_project_pop_up.py` & `Simba-UW-tf-dev-1.57.5/simba/create_project_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/video_info_table.py` & `Simba-UW-tf-dev-1.57.5/simba/video_info_table.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/cue_light_tools/.DS_Store` & `Simba-UW-tf-dev-1.57.5/simba/cue_light_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/cue_light_tools/cue_light_clf_statistics.py` & `Simba-UW-tf-dev-1.57.5/simba/cue_light_tools/cue_light_clf_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/cue_light_tools/cue_light_analyzer.py` & `Simba-UW-tf-dev-1.57.5/simba/cue_light_tools/cue_light_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/cue_light_tools/cue_light_menues.py` & `Simba-UW-tf-dev-1.57.5/simba/cue_light_tools/cue_light_menues.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/cue_light_tools/cue_light_tools.py` & `Simba-UW-tf-dev-1.57.5/simba/cue_light_tools/cue_light_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/cue_light_tools/cue_light_visualizer.py` & `Simba-UW-tf-dev-1.57.5/simba/cue_light_tools/cue_light_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/cue_light_tools/cue_light_movement_statistics.py` & `Simba-UW-tf-dev-1.57.5/simba/cue_light_tools/cue_light_movement_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/extract_frames_fast.py` & `Simba-UW-tf-dev-1.57.5/simba/extract_frames_fast.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/utils/.DS_Store` & `Simba-UW-tf-dev-1.57.5/simba/utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/utils/warnings.py` & `Simba-UW-tf-dev-1.57.5/simba/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/utils/lookups.py` & `Simba-UW-tf-dev-1.57.5/simba/utils/lookups.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/utils/errors.py` & `Simba-UW-tf-dev-1.57.5/simba/utils/errors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/utils/printing.py` & `Simba-UW-tf-dev-1.57.5/simba/utils/printing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/labelling_interface.py` & `Simba-UW-tf-dev-1.57.5/simba/labelling_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/timebins_movement_analyzer.py` & `Simba-UW-tf-dev-1.57.5/simba/timebins_movement_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/train_model_functions.py` & `Simba-UW-tf-dev-1.57.5/simba/train_model_functions.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/SimBA_dash_app.py` & `Simba-UW-tf-dev-1.57.5/simba/SimBA_dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/timebins_clf_analyzer.py` & `Simba-UW-tf-dev-1.57.5/simba/timebins_clf_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/calculate_px_dist.py` & `Simba-UW-tf-dev-1.57.5/simba/calculate_px_dist.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/movement_processor.py` & `Simba-UW-tf-dev-1.57.5/simba/movement_processor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/pybursts.py` & `Simba-UW-tf-dev-1.57.5/simba/pybursts.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/rw_dfs.py` & `Simba-UW-tf-dev-1.57.5/simba/rw_dfs.py`

 * *Files 5% similar despite different names*

```diff
@@ -81,14 +81,18 @@
     """
 
     if file_type == Formats.CSV.value:
         df = df.drop('scorer', axis=1, errors='ignore')
         idx = np.arange(len(df)).astype(str)
         df.insert(0, '', idx)
         df = pa.Table.from_pandas(df=df)
+        try:
+            df = df.drop(['__index_level_0__'])
+        except KeyError:
+            pass
         csv.write_csv(df, save_path)
     elif file_type == Formats.PARQUET.value:
         df.to_parquet(save_path)
     elif file_type == Formats.PICKLE.value:
         try:
             with open(save_path, 'wb') as f:
                 pickle.dump(df, f, protocol=pickle.HIGHEST_PROTOCOL)
```

### Comparing `Simba-UW-tf-dev-1.57.4/simba/reverse_2_animal_tracking.py` & `Simba-UW-tf-dev-1.57.5/simba/reverse_2_animal_tracking.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/Directing_animals_analyzer.py` & `Simba-UW-tf-dev-1.57.5/simba/Directing_animals_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/Validate_model_one_video_run_clf.py` & `Simba-UW-tf-dev-1.57.5/simba/Validate_model_one_video_run_clf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/tkinter_functions.py` & `Simba-UW-tf-dev-1.57.5/simba/tkinter_functions.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/setting_menu.py` & `Simba-UW-tf-dev-1.57.5/simba/setting_menu.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/interpolate_pose.py` & `Simba-UW-tf-dev-1.57.5/simba/interpolate_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/run_inference.py` & `Simba-UW-tf-dev-1.57.5/simba/run_inference.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/plotting/gantt_creator.py` & `Simba-UW-tf-dev-1.57.5/simba/plotting/gantt_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/plotting/tools/tkinter_tools.py` & `Simba-UW-tf-dev-1.57.5/simba/plotting/tools/tkinter_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/plotting/ROI_plotter_mp.py` & `Simba-UW-tf-dev-1.57.5/simba/plotting/ROI_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/plotting/shap_agg_stats_visualizer.py` & `Simba-UW-tf-dev-1.57.5/simba/plotting/shap_agg_stats_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/plotting/gantt_creator_mp.py` & `Simba-UW-tf-dev-1.57.5/simba/plotting/gantt_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/plotting/heat_mapper_clf_mp.py` & `Simba-UW-tf-dev-1.57.5/simba/plotting/heat_mapper_clf_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/plotting/probability_plot_creator.py` & `Simba-UW-tf-dev-1.57.5/simba/plotting/probability_plot_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/plotting/misc_visualizations.py` & `Simba-UW-tf-dev-1.57.5/simba/plotting/misc_visualizations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/plotting/plot_clf_results.py` & `Simba-UW-tf-dev-1.57.5/simba/plotting/plot_clf_results.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/plotting/plot_clf_results_mp.py` & `Simba-UW-tf-dev-1.57.5/simba/plotting/plot_clf_results_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/plotting/ROI_feature_visualizer.py` & `Simba-UW-tf-dev-1.57.5/simba/plotting/ROI_feature_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/plotting/heat_mapper_location.py` & `Simba-UW-tf-dev-1.57.5/simba/plotting/heat_mapper_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/plotting/probability_plot_creator_mp.py` & `Simba-UW-tf-dev-1.57.5/simba/plotting/probability_plot_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/plotting/interactive_probability_grapher.py` & `Simba-UW-tf-dev-1.57.5/simba/plotting/interactive_probability_grapher.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/plotting/plot_pose_in_dir.py` & `Simba-UW-tf-dev-1.57.5/simba/plotting/plot_pose_in_dir.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/plotting/single_run_model_validation_video.py` & `Simba-UW-tf-dev-1.57.5/simba/plotting/single_run_model_validation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/plotting/frame_mergerer_ffmpeg.py` & `Simba-UW-tf-dev-1.57.5/simba/plotting/frame_mergerer_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/plotting/Directing_animals_visualizer_mp.py` & `Simba-UW-tf-dev-1.57.5/simba/plotting/Directing_animals_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/plotting/clf_validator.py` & `Simba-UW-tf-dev-1.57.5/simba/plotting/clf_validator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/plotting/path_plotter_mp.py` & `Simba-UW-tf-dev-1.57.5/simba/plotting/path_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/plotting/ROI_feature_visualizer_mp.py` & `Simba-UW-tf-dev-1.57.5/simba/plotting/ROI_feature_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/plotting/data_plotter.py` & `Simba-UW-tf-dev-1.57.5/simba/plotting/data_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/plotting/path_plotter.py` & `Simba-UW-tf-dev-1.57.5/simba/plotting/path_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/plotting/ez_lineplot.py` & `Simba-UW-tf-dev-1.57.5/simba/plotting/ez_lineplot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/plotting/distance_plotter_mp.py` & `Simba-UW-tf-dev-1.57.5/simba/plotting/distance_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/plotting/ROI_plotter.py` & `Simba-UW-tf-dev-1.57.5/simba/plotting/ROI_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/plotting/heat_mapper_clf.py` & `Simba-UW-tf-dev-1.57.5/simba/plotting/heat_mapper_clf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/plotting/distance_plotter.py` & `Simba-UW-tf-dev-1.57.5/simba/plotting/distance_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/plotting/single_run_model_validation_video_mp.py` & `Simba-UW-tf-dev-1.57.5/simba/plotting/single_run_model_validation_video_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/plotting/Directing_animals_visualizer.py` & `Simba-UW-tf-dev-1.57.5/simba/plotting/Directing_animals_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/plotting/heat_mapper_location_mp.py` & `Simba-UW-tf-dev-1.57.5/simba/plotting/heat_mapper_location_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/run_dash_tkinter.py` & `Simba-UW-tf-dev-1.57.5/simba/run_dash_tkinter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/interpolate_smooth_post_hoc.py` & `Simba-UW-tf-dev-1.57.5/simba/interpolate_smooth_post_hoc.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/dash_app.py` & `Simba-UW-tf-dev-1.57.5/simba/dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/reverse_tracking_order.py` & `Simba-UW-tf-dev-1.57.5/simba/reverse_tracking_order.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/concatenator_pop_up.py` & `Simba-UW-tf-dev-1.57.5/simba/concatenator_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/extract_annotation_frames.py` & `Simba-UW-tf-dev-1.57.5/simba/extract_annotation_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/roi_tools/ROI_time_bin_calculator.py` & `Simba-UW-tf-dev-1.57.5/simba/roi_tools/ROI_time_bin_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/roi_tools/ROI_movement_analyzer.py` & `Simba-UW-tf-dev-1.57.5/simba/roi_tools/ROI_movement_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/roi_tools/.DS_Store` & `Simba-UW-tf-dev-1.57.5/simba/roi_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/roi_tools/ROI_define.py` & `Simba-UW-tf-dev-1.57.5/simba/roi_tools/ROI_define.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/roi_tools/ROI_reset.py` & `Simba-UW-tf-dev-1.57.5/simba/roi_tools/ROI_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/roi_tools/ROI_analyzer.py` & `Simba-UW-tf-dev-1.57.5/simba/roi_tools/ROI_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/roi_tools/ROI_feature_analyzer.py` & `Simba-UW-tf-dev-1.57.5/simba/roi_tools/ROI_feature_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/roi_tools/ROI_multiply.py` & `Simba-UW-tf-dev-1.57.5/simba/roi_tools/ROI_multiply.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/roi_tools/ROI_size_calculations.py` & `Simba-UW-tf-dev-1.57.5/simba/roi_tools/ROI_size_calculations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/roi_tools/ROI_zoom.py` & `Simba-UW-tf-dev-1.57.5/simba/roi_tools/ROI_zoom.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/roi_tools/ROI_directing_analyzer.py` & `Simba-UW-tf-dev-1.57.5/simba/roi_tools/ROI_directing_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/roi_tools/ROI_move_shape.py` & `Simba-UW-tf-dev-1.57.5/simba/roi_tools/ROI_move_shape.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/roi_tools/ROI_menus.py` & `Simba-UW-tf-dev-1.57.5/simba/roi_tools/ROI_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/roi_tools/ROI_clf_calculator.py` & `Simba-UW-tf-dev-1.57.5/simba/roi_tools/ROI_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/roi_tools/ROI_image.py` & `Simba-UW-tf-dev-1.57.5/simba/roi_tools/ROI_image.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/misc_tools.py` & `Simba-UW-tf-dev-1.57.5/simba/misc_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/pose_importers/read_DANNCE_mat.py` & `Simba-UW-tf-dev-1.57.5/simba/pose_importers/read_DANNCE_mat.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/pose_importers/sleap_importer_slp.py` & `Simba-UW-tf-dev-1.57.5/simba/pose_importers/sleap_importer_slp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/pose_importers/sleap_importer_h5.py` & `Simba-UW-tf-dev-1.57.5/simba/pose_importers/sleap_importer_h5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/pose_importers/dlc_multi_animal_importer.py` & `Simba-UW-tf-dev-1.57.5/simba/pose_importers/dlc_multi_animal_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/pose_importers/sleap_importer_csv.py` & `Simba-UW-tf-dev-1.57.5/simba/pose_importers/sleap_importer_csv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/pose_importers/import_trk.py` & `Simba-UW-tf-dev-1.57.5/simba/pose_importers/import_trk.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/pose_importers/import_mars.py` & `Simba-UW-tf-dev-1.57.5/simba/pose_importers/import_mars.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/pose_importers/dlc_importer_csv.py` & `Simba-UW-tf-dev-1.57.5/simba/pose_importers/dlc_importer_csv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/pose_importers/trk_importer.py` & `Simba-UW-tf-dev-1.57.5/simba/pose_importers/trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/pop_up_classes.py` & `Simba-UW-tf-dev-1.57.5/simba/pop_up_classes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/extract_seqframes.py` & `Simba-UW-tf-dev-1.57.5/simba/extract_seqframes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/pose_configurations/.DS_Store` & `Simba-UW-tf-dev-1.57.5/simba/pose_configurations/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/pose_configurations/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.57.5/simba/pose_configurations/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/pose_configurations/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.57.5/simba/pose_configurations/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/pose_configurations/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.57.5/simba/pose_configurations/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/pose_configurations/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.57.5/simba/pose_configurations/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/pose_configurations/schematics/.DS_Store` & `Simba-UW-tf-dev-1.57.5/simba/pose_configurations/schematics/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/pose_configurations/schematics/8.png` & `Simba-UW-tf-dev-1.57.5/simba/pose_configurations/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/pose_configurations/schematics/9.png` & `Simba-UW-tf-dev-1.57.5/simba/pose_configurations/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/pose_configurations/schematics/12.png` & `Simba-UW-tf-dev-1.57.5/simba/pose_configurations/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/pose_configurations/schematics/11.png` & `Simba-UW-tf-dev-1.57.5/simba/pose_configurations/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/pose_configurations/schematics/10.png` & `Simba-UW-tf-dev-1.57.5/simba/pose_configurations/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/pose_configurations/schematics/4.png` & `Simba-UW-tf-dev-1.57.5/simba/pose_configurations/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/pose_configurations/schematics/5.png` & `Simba-UW-tf-dev-1.57.5/simba/pose_configurations/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/pose_configurations/schematics/7.png` & `Simba-UW-tf-dev-1.57.5/simba/pose_configurations/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/pose_configurations/schematics/6.png` & `Simba-UW-tf-dev-1.57.5/simba/pose_configurations/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/pose_configurations/schematics/2.png` & `Simba-UW-tf-dev-1.57.5/simba/pose_configurations/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/pose_configurations/schematics/3.png` & `Simba-UW-tf-dev-1.57.5/simba/pose_configurations/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/pose_configurations/schematics/1.png` & `Simba-UW-tf-dev-1.57.5/simba/pose_configurations/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/get_coordinates_tools_v2.py` & `Simba-UW-tf-dev-1.57.5/simba/get_coordinates_tools_v2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/pup_retrieval_protocol.py` & `Simba-UW-tf-dev-1.57.5/simba/pup_retrieval_protocol.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/outlier_tools/outlier_corrector_movement.py` & `Simba-UW-tf-dev-1.57.5/simba/outlier_tools/outlier_corrector_movement.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/outlier_tools/.DS_Store` & `Simba-UW-tf-dev-1.57.5/simba/outlier_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/outlier_tools/outlier_corrector_location.py` & `Simba-UW-tf-dev-1.57.5/simba/outlier_tools/outlier_corrector_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/outlier_tools/skip_outlier_correction.py` & `Simba-UW-tf-dev-1.57.5/simba/outlier_tools/skip_outlier_correction.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,14 +69,19 @@
             data_df.index.name = None
             save_path = os.path.join(self.out_dir, video_name + '.' + self.file_type)
             save_df(data_df, self.file_type, save_path)
             self.file_cnt += 1
             print('Skipped outlier correction for video {} ...'.format(video_name))
         stdout_success(msg=f'Skipped outlier correction for {str(self.file_cnt)} files')
 
+# test = OutlierCorrectionSkipper(config_path='/Users/simon/Desktop/envs/troubleshooting/naresh/project_folder/project_config.ini')
+# test.skip_outlier_correction()
+
+
+
 # test = OutlierCorrectionSkipper(config_path='/Users/simon/Desktop/troubleshooting/Zebrafish/project_folder/project_config.ini')
 # test.skip_outlier_correction()
 
 # test = OutlierCorrectionSkipper(config_path=r"Z:\DeepLabCut\DLC_extract\Troubleshooting\Parquet_test2\project_folder\project_config.ini")
 # test.skip_outlier_correction()
 
 # test = OutlierCorrectionSkipper(config_path='/Users/simon/Desktop/troubleshooting/User_def_2/project_folder/project_config.ini')
```

### Comparing `Simba-UW-tf-dev-1.57.4/simba/outlier_tools/.idea/outlier_scripts.iml` & `Simba-UW-tf-dev-1.57.5/simba/outlier_tools/.idea/outlier_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.57.5/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/outlier_tools/.idea/workspace.xml` & `Simba-UW-tf-dev-1.57.5/simba/outlier_tools/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/pose_reset.py` & `Simba-UW-tf-dev-1.57.5/simba/pose_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/train_mutiple_models.py` & `Simba-UW-tf-dev-1.57.5/simba/train_mutiple_models.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/SimBA.py` & `Simba-UW-tf-dev-1.57.5/simba/SimBA.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/labelling_advanced_interface.py` & `Simba-UW-tf-dev-1.57.5/simba/labelling_advanced_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.57.5/simba/assets/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/unsupervised/model_names.parquet` & `Simba-UW-tf-dev-1.57.5/simba/assets/unsupervised/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/unsupervised/features.csv` & `Simba-UW-tf-dev-1.57.5/simba/assets/unsupervised/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/shap/down_arrow.jpg` & `Simba-UW-tf-dev-1.57.5/simba/assets/shap/down_arrow.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/shap/intruder_shape.jpg` & `Simba-UW-tf-dev-1.57.5/simba/assets/shap/intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/shap/feature_categories/shap_feature_categories.csv` & `Simba-UW-tf-dev-1.57.5/simba/assets/shap/feature_categories/shap_feature_categories.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/shap/.DS_Store` & `Simba-UW-tf-dev-1.57.5/simba/assets/shap/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/shap/resident_shape.jpg` & `Simba-UW-tf-dev-1.57.5/simba/assets/shap/resident_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/shap/resident_intruder_shape.jpg` & `Simba-UW-tf-dev-1.57.5/simba/assets/shap/resident_intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/shap/animal_distances.jpg` & `Simba-UW-tf-dev-1.57.5/simba/assets/shap/animal_distances.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/shap/baseline_scale.jpg` & `Simba-UW-tf-dev-1.57.5/simba/assets/shap/baseline_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/shap/ubuntu.regular.ttf` & `Simba-UW-tf-dev-1.57.5/simba/assets/shap/ubuntu.regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/shap/side_scale.jpg` & `Simba-UW-tf-dev-1.57.5/simba/assets/shap/side_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/shap/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.57.5/simba/assets/shap/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/shap/side_scale_5.jpg` & `Simba-UW-tf-dev-1.57.5/simba/assets/shap/side_scale_5.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/shap/intruder_movement.jpg` & `Simba-UW-tf-dev-1.57.5/simba/assets/shap/intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/shap/resident_movement.jpg` & `Simba-UW-tf-dev-1.57.5/simba/assets/shap/resident_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/shap/color_bar.jpg` & `Simba-UW-tf-dev-1.57.5/simba/assets/shap/color_bar.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/shap/resident_intruder_movement.jpg` & `Simba-UW-tf-dev-1.57.5/simba/assets/shap/resident_intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/.DS_Store` & `Simba-UW-tf-dev-1.57.5/simba/assets/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/lookups/.DS_Store` & `Simba-UW-tf-dev-1.57.5/simba/assets/lookups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/lookups/model_names.parquet` & `Simba-UW-tf-dev-1.57.5/simba/assets/lookups/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/lookups/feature_extraction_headers.csv` & `Simba-UW-tf-dev-1.57.5/simba/assets/lookups/feature_extraction_headers.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/lookups/features.csv` & `Simba-UW-tf-dev-1.57.5/simba/assets/lookups/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/lookups/unsupervised_example_x.csv` & `Simba-UW-tf-dev-1.57.5/simba/assets/lookups/unsupervised_example_x.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/stl/operant_tray.stl` & `Simba-UW-tf-dev-1.57.5/simba/assets/stl/operant_tray.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/stl/operant_lever.stl` & `Simba-UW-tf-dev-1.57.5/simba/assets/stl/operant_lever.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/stl/operant_walls.stl` & `Simba-UW-tf-dev-1.57.5/simba/assets/stl/operant_walls.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/stl/grid_floor.stl` & `Simba-UW-tf-dev-1.57.5/simba/assets/stl/grid_floor.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/img/.DS_Store` & `Simba-UW-tf-dev-1.57.5/simba/assets/img/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/img/about_me.png` & `Simba-UW-tf-dev-1.57.5/simba/assets/img/about_me.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/img/splash.mp4` & `Simba-UW-tf-dev-1.57.5/simba/assets/img/splash.mp4`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/img/bg_2.png` & `Simba-UW-tf-dev-1.57.5/simba/assets/img/bg_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/img/splash.pptx` & `Simba-UW-tf-dev-1.57.5/simba/assets/img/splash.pptx`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/img/bg.png` & `Simba-UW-tf-dev-1.57.5/simba/assets/img/bg.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.57.5/simba/assets/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/icons/factory.png` & `Simba-UW-tf-dev-1.57.5/simba/assets/icons/factory.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/icons/cluster.png` & `Simba-UW-tf-dev-1.57.5/simba/assets/icons/cluster.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/icons/load.png` & `Simba-UW-tf-dev-1.57.5/simba/assets/icons/load.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/icons/gif.png` & `Simba-UW-tf-dev-1.57.5/simba/assets/icons/gif.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/icons/pose.png` & `Simba-UW-tf-dev-1.57.5/simba/assets/icons/pose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/icons/features.png` & `Simba-UW-tf-dev-1.57.5/simba/assets/icons/features.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/icons/.DS_Store` & `Simba-UW-tf-dev-1.57.5/simba/assets/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/icons/settings.png` & `Simba-UW-tf-dev-1.57.5/simba/assets/icons/settings.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/icons/stopwatch.png` & `Simba-UW-tf-dev-1.57.5/simba/assets/icons/stopwatch.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/icons/link.png` & `Simba-UW-tf-dev-1.57.5/simba/assets/icons/link.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/icons/dash_simba.css` & `Simba-UW-tf-dev-1.57.5/simba/assets/icons/dash_simba.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/icons/documentation.png` & `Simba-UW-tf-dev-1.57.5/simba/assets/icons/documentation.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/icons/fps.png` & `Simba-UW-tf-dev-1.57.5/simba/assets/icons/fps.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/icons/dimensionality_reduction.png` & `Simba-UW-tf-dev-1.57.5/simba/assets/icons/dimensionality_reduction.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/icons/roi.png` & `Simba-UW-tf-dev-1.57.5/simba/assets/icons/roi.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/icons/superimpose.png` & `Simba-UW-tf-dev-1.57.5/simba/assets/icons/superimpose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/icons/label.png` & `Simba-UW-tf-dev-1.57.5/simba/assets/icons/label.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/icons/change.png` & `Simba-UW-tf-dev-1.57.5/simba/assets/icons/change.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/icons/crop.png` & `Simba-UW-tf-dev-1.57.5/simba/assets/icons/crop.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/icons/rotate.png` & `Simba-UW-tf-dev-1.57.5/simba/assets/icons/rotate.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/icons/path.png` & `Simba-UW-tf-dev-1.57.5/simba/assets/icons/path.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/icons/clip.png` & `Simba-UW-tf-dev-1.57.5/simba/assets/icons/clip.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/icons/restart.png` & `Simba-UW-tf-dev-1.57.5/simba/assets/icons/restart.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/icons/calipher.png` & `Simba-UW-tf-dev-1.57.5/simba/assets/icons/calipher.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/icons/add_on.png` & `Simba-UW-tf-dev-1.57.5/simba/assets/icons/add_on.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/icons/create.png` & `Simba-UW-tf-dev-1.57.5/simba/assets/icons/create.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/icons/SimBA_logo.ico` & `Simba-UW-tf-dev-1.57.5/simba/assets/icons/SimBA_logo.ico`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/icons/print.png` & `Simba-UW-tf-dev-1.57.5/simba/assets/icons/print.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/icons/clf.png` & `Simba-UW-tf-dev-1.57.5/simba/assets/icons/clf.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/icons/concat_icons/mosaic.png` & `Simba-UW-tf-dev-1.57.5/simba/assets/icons/concat_icons/mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/icons/concat_icons/vertical.png` & `Simba-UW-tf-dev-1.57.5/simba/assets/icons/concat_icons/vertical.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/icons/concat_icons/horizontal.png` & `Simba-UW-tf-dev-1.57.5/simba/assets/icons/concat_icons/horizontal.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/icons/concat_icons/mixed_mosaic.png` & `Simba-UW-tf-dev-1.57.5/simba/assets/icons/concat_icons/mixed_mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/icons/merge.png` & `Simba-UW-tf-dev-1.57.5/simba/assets/icons/merge.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/icons/clean.png` & `Simba-UW-tf-dev-1.57.5/simba/assets/icons/clean.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/icons/clf_2.png` & `Simba-UW-tf-dev-1.57.5/simba/assets/icons/clf_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/icons/visualize.png` & `Simba-UW-tf-dev-1.57.5/simba/assets/icons/visualize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/icons/concat.png` & `Simba-UW-tf-dev-1.57.5/simba/assets/icons/concat.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/icons/boris.png` & `Simba-UW-tf-dev-1.57.5/simba/assets/icons/boris.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/icons/frames.png` & `Simba-UW-tf-dev-1.57.5/simba/assets/icons/frames.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/icons/video.png` & `Simba-UW-tf-dev-1.57.5/simba/assets/icons/video.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/icons/sample.png` & `Simba-UW-tf-dev-1.57.5/simba/assets/icons/sample.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/icons/metrics.png` & `Simba-UW-tf-dev-1.57.5/simba/assets/icons/metrics.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/icons/grey.png` & `Simba-UW-tf-dev-1.57.5/simba/assets/icons/grey.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/icons/exit.png` & `Simba-UW-tf-dev-1.57.5/simba/assets/icons/exit.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/icons/outlier.png` & `Simba-UW-tf-dev-1.57.5/simba/assets/icons/outlier.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/icons/clahe.png` & `Simba-UW-tf-dev-1.57.5/simba/assets/icons/clahe.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/icons/trash.png` & `Simba-UW-tf-dev-1.57.5/simba/assets/icons/trash.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/icons/about.png` & `Simba-UW-tf-dev-1.57.5/simba/assets/icons/about.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/icons/convert.png` & `Simba-UW-tf-dev-1.57.5/simba/assets/icons/convert.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/icons/SimBA_logo.icns` & `Simba-UW-tf-dev-1.57.5/simba/assets/icons/SimBA_logo.icns`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/icons/reorganize.png` & `Simba-UW-tf-dev-1.57.5/simba/assets/icons/reorganize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/icons/browse.png` & `Simba-UW-tf-dev-1.57.5/simba/assets/icons/browse.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/icons/SimBA_logo.png` & `Simba-UW-tf-dev-1.57.5/simba/assets/icons/SimBA_logo.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/icons/ethovision.png` & `Simba-UW-tf-dev-1.57.5/simba/assets/icons/ethovision.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/icons/close.png` & `Simba-UW-tf-dev-1.57.5/simba/assets/icons/close.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/dash_simba_base.css` & `Simba-UW-tf-dev-1.57.5/simba/assets/dash_simba_base.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/assets/TheGoldenLab.PNG` & `Simba-UW-tf-dev-1.57.5/simba/assets/TheGoldenLab.PNG`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/drop_bp_cords.py` & `Simba-UW-tf-dev-1.57.5/simba/drop_bp_cords.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/read_config_unit_tests.py` & `Simba-UW-tf-dev-1.57.5/simba/read_config_unit_tests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/project_config_creator.py` & `Simba-UW-tf-dev-1.57.5/simba/project_config_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/set_hyperparameters.py` & `Simba-UW-tf-dev-1.57.5/simba/set_hyperparameters.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/train_single_model.py` & `Simba-UW-tf-dev-1.57.5/simba/train_single_model.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/create_clf_log.py` & `Simba-UW-tf-dev-1.57.5/simba/create_clf_log.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/batch_process_videos/.DS_Store` & `Simba-UW-tf-dev-1.57.5/simba/batch_process_videos/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/batch_process_videos/batch_process_menus.py` & `Simba-UW-tf-dev-1.57.5/simba/batch_process_videos/batch_process_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/batch_process_videos/batch_process_create_ffmpeg_commands.py` & `Simba-UW-tf-dev-1.57.5/simba/batch_process_videos/batch_process_create_ffmpeg_commands.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/Kleinberg_calculator.py` & `Simba-UW-tf-dev-1.57.5/simba/Kleinberg_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/reorganize_keypoint_in_pose.py` & `Simba-UW-tf-dev-1.57.5/simba/reorganize_keypoint_in_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/simba/play_annotation_video.py` & `Simba-UW-tf-dev-1.57.5/simba/play_annotation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/Simba_UW_tf_dev.egg-info/PKG-INFO` & `Simba-UW-tf-dev-1.57.5/Simba_UW_tf_dev.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.57.4
+Version: 1.57.5
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.57.4/Simba_UW_tf_dev.egg-info/SOURCES.txt` & `Simba-UW-tf-dev-1.57.5/Simba_UW_tf_dev.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -222,14 +222,15 @@
 simba/feature_extractors/misc/graph_3d_plotter.py
 simba/feature_extractors/misc/graph_creator.py
 simba/feature_extractors/misc/make_splash.py
 simba/feature_extractors/misc/mutual_exclusive.py
 simba/feature_extractors/misc/peaks.py
 simba/feature_extractors/misc/read_in_mp.py
 simba/feature_extractors/misc/termite_rois.csv
+simba/feature_extractors/misc/time_stamp_calculator.py
 simba/feature_extractors/misc/video_color.py
 simba/feature_extractors/misc/video_rotator.py
 simba/feature_extractors/misc/video_rotator_mp.py
 simba/mixins/.DS_Store
 simba/mixins/config_reader.py
 simba/mixins/feature_extraction_mixin.py
 simba/mixins/pop_up_mixin.py
```

### Comparing `Simba-UW-tf-dev-1.57.4/Simba_UW_tf_dev.egg-info/requires.txt` & `Simba-UW-tf-dev-1.57.5/Simba_UW_tf_dev.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/LICENSE.md` & `Simba-UW-tf-dev-1.57.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/README.md` & `Simba-UW-tf-dev-1.57.5/README.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.4/setup.py` & `Simba-UW-tf-dev-1.57.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Licensed under GNU Lesser General Public License v3.0
 """
 
 import setuptools
 
 setuptools.setup(
     name="Simba-UW-tf-dev",
-    version="1.57.4",
+    version="1.57.5",
     author="Simon Nilsson, Jia Jie Choong, Sophia Hwang",
     author_email="sronilsson@gmail.com",
     description="Toolkit for computer classification of complex social behaviors in experimental animals",
     url="https://github.com/sgoldenlab/simba",
     install_requires=['Pillow == 5.4.1', 'pyyaml == 5.3.1','shapely == 1.7','wxpython == 4.0.4',
               'dtreeviz == 0.8.1','eli5 == 0.10.1','graphviz == 0.11',
               'imblearn == 0.0','imgaug == 0.4.0','imutils == 0.5.2','matplotlib == 3.0.3', 'numpy == 1.18.1',
```

