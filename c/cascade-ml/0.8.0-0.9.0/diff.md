# Comparing `tmp/cascade-ml-0.8.0.tar.gz` & `tmp/cascade-ml-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cascade-ml-0.8.0.tar", last modified: Tue Nov 15 22:01:14 2022, max compression
+gzip compressed data, was "cascade-ml-0.9.0.tar", last modified: Fri Dec 16 15:06:04 2022, max compression
```

## Comparing `cascade-ml-0.8.0.tar` & `cascade-ml-0.9.0.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2022-11-15 22:01:14.326391 cascade-ml-0.8.0/
--rw-rw-r--   0 ilia      (1000) ilia      (1000)    11328 2022-09-03 15:51:41.000000 cascade-ml-0.8.0/LICENSE
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     5021 2022-11-15 22:01:14.326391 cascade-ml-0.8.0/PKG-INFO
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     4560 2022-09-29 10:07:30.000000 cascade-ml-0.8.0/README.md
-drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2022-11-15 22:01:14.318391 cascade-ml-0.8.0/cascade/
--rw-rw-r--   0 ilia      (1000) ilia      (1000)      972 2022-11-15 22:00:08.000000 cascade-ml-0.8.0/cascade/__init__.py
-drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2022-11-15 22:01:14.318391 cascade-ml-0.8.0/cascade/base/
--rw-rw-r--   0 ilia      (1000) ilia      (1000)      150 2022-09-23 15:03:14.000000 cascade-ml-0.8.0/cascade/base/__init__.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     6257 2022-11-15 22:00:08.000000 cascade-ml-0.8.0/cascade/base/meta_handler.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     2273 2022-11-15 22:00:08.000000 cascade-ml-0.8.0/cascade/base/traceable.py
-drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2022-11-15 22:01:14.318391 cascade-ml-0.8.0/cascade/data/
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     1107 2022-11-15 22:00:08.000000 cascade-ml-0.8.0/cascade/data/__init__.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     1633 2022-11-15 22:00:08.000000 cascade-ml-0.8.0/cascade/data/apply_modifier.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     2325 2022-10-06 09:46:54.000000 cascade-ml-0.8.0/cascade/data/bruteforce_cacher.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     1646 2022-11-15 22:00:08.000000 cascade-ml-0.8.0/cascade/data/composer.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     2479 2022-10-06 09:46:54.000000 cascade-ml-0.8.0/cascade/data/concatenator.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     1067 2022-10-06 09:46:54.000000 cascade-ml-0.8.0/cascade/data/cyclic_sampler.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     5653 2022-11-15 22:00:08.000000 cascade-ml-0.8.0/cascade/data/dataset.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     1443 2022-11-15 22:00:08.000000 cascade-ml-0.8.0/cascade/data/folder_dataset.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     1909 2022-11-15 22:00:08.000000 cascade-ml-0.8.0/cascade/data/pickler.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     1793 2022-10-06 09:46:54.000000 cascade-ml-0.8.0/cascade/data/random_sampler.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     2045 2022-11-15 22:00:08.000000 cascade-ml-0.8.0/cascade/data/range_sampler.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     2183 2022-11-15 22:00:08.000000 cascade-ml-0.8.0/cascade/data/sequential_cacher.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     1182 2022-10-06 09:46:54.000000 cascade-ml-0.8.0/cascade/data/utils.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     5909 2022-11-15 22:00:08.000000 cascade-ml-0.8.0/cascade/data/version_assigner.py
-drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2022-11-15 22:01:14.322391 cascade-ml-0.8.0/cascade/meta/
--rw-rw-r--   0 ilia      (1000) ilia      (1000)      899 2022-11-15 22:00:08.000000 cascade-ml-0.8.0/cascade/meta/__init__.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     1768 2022-11-15 22:00:08.000000 cascade-ml-0.8.0/cascade/meta/dataleak_validator.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)      652 2022-11-15 22:00:08.000000 cascade-ml-0.8.0/cascade/meta/hashes.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     7846 2022-11-15 22:00:08.000000 cascade-ml-0.8.0/cascade/meta/history_viewer.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     3402 2022-10-06 09:46:54.000000 cascade-ml-0.8.0/cascade/meta/meta_validator.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     2869 2022-11-15 22:00:08.000000 cascade-ml-0.8.0/cascade/meta/meta_viewer.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     8872 2022-11-15 22:00:08.000000 cascade-ml-0.8.0/cascade/meta/metric_viewer.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     3666 2022-11-15 22:00:08.000000 cascade-ml-0.8.0/cascade/meta/validator.py
-drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2022-11-15 22:01:14.322391 cascade-ml-0.8.0/cascade/models/
--rw-rw-r--   0 ilia      (1000) ilia      (1000)      768 2022-09-23 15:03:14.000000 cascade-ml-0.8.0/cascade/models/__init__.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     2397 2022-10-06 09:46:54.000000 cascade-ml-0.8.0/cascade/models/basic_model.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     4035 2022-10-06 09:46:54.000000 cascade-ml-0.8.0/cascade/models/model.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     5833 2022-10-06 09:46:54.000000 cascade-ml-0.8.0/cascade/models/model_line.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)    10036 2022-11-15 22:00:08.000000 cascade-ml-0.8.0/cascade/models/model_repo.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     5992 2022-11-15 22:00:08.000000 cascade-ml-0.8.0/cascade/models/trainer.py
-drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2022-11-15 22:01:14.326391 cascade-ml-0.8.0/cascade/tests/
--rw-rw-r--   0 ilia      (1000) ilia      (1000)       44 2022-09-05 21:14:08.000000 cascade-ml-0.8.0/cascade/tests/__init__.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     3294 2022-09-23 15:03:14.000000 cascade-ml-0.8.0/cascade/tests/conftest.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     1102 2022-09-23 15:03:14.000000 cascade-ml-0.8.0/cascade/tests/test_apply_modifier.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     2088 2022-09-05 21:14:08.000000 cascade-ml-0.8.0/cascade/tests/test_basic_model.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     1201 2022-09-23 15:03:14.000000 cascade-ml-0.8.0/cascade/tests/test_bruteforce_cacher.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     1630 2022-11-15 22:00:08.000000 cascade-ml-0.8.0/cascade/tests/test_composer.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     1350 2022-11-15 22:00:08.000000 cascade-ml-0.8.0/cascade/tests/test_concatenator.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)      970 2022-09-23 15:03:14.000000 cascade-ml-0.8.0/cascade/tests/test_cyclic_sampler.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     1233 2022-09-23 15:03:14.000000 cascade-ml-0.8.0/cascade/tests/test_data_split.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     1780 2022-11-15 22:00:08.000000 cascade-ml-0.8.0/cascade/tests/test_dataleak_validator.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     2484 2022-09-23 15:03:14.000000 cascade-ml-0.8.0/cascade/tests/test_dataset.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     1143 2022-09-23 15:03:14.000000 cascade-ml-0.8.0/cascade/tests/test_folder_dataset.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     2172 2022-09-23 15:03:14.000000 cascade-ml-0.8.0/cascade/tests/test_history_viewer.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     2929 2022-09-23 15:03:14.000000 cascade-ml-0.8.0/cascade/tests/test_meta_handler.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     1214 2022-09-05 21:14:08.000000 cascade-ml-0.8.0/cascade/tests/test_meta_validator.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     2027 2022-11-15 22:00:08.000000 cascade-ml-0.8.0/cascade/tests/test_meta_viewer.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     2365 2022-11-15 22:00:08.000000 cascade-ml-0.8.0/cascade/tests/test_metric_viewer.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     1118 2022-09-23 15:03:14.000000 cascade-ml-0.8.0/cascade/tests/test_model_line.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     9379 2022-11-15 22:00:08.000000 cascade-ml-0.8.0/cascade/tests/test_model_repo.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     1028 2022-09-23 15:03:14.000000 cascade-ml-0.8.0/cascade/tests/test_modifier.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     1300 2022-11-15 22:00:08.000000 cascade-ml-0.8.0/cascade/tests/test_pickler.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     1459 2022-09-23 15:03:14.000000 cascade-ml-0.8.0/cascade/tests/test_random_sampler.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     1403 2022-09-23 15:03:14.000000 cascade-ml-0.8.0/cascade/tests/test_range_sampler.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)      923 2022-09-23 15:03:14.000000 cascade-ml-0.8.0/cascade/tests/test_sequential_cacher.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     1867 2022-09-23 15:03:14.000000 cascade-ml-0.8.0/cascade/tests/test_traceable.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     1538 2022-09-23 15:03:14.000000 cascade-ml-0.8.0/cascade/tests/test_trainer.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     2060 2022-09-23 15:03:14.000000 cascade-ml-0.8.0/cascade/tests/test_validator.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     1398 2022-11-15 22:00:08.000000 cascade-ml-0.8.0/cascade/tests/test_version_assigner.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     1900 2022-11-15 22:00:08.000000 cascade-ml-0.8.0/cascade/tests/test_weighed_sampler.py
-drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2022-11-15 22:01:14.326391 cascade-ml-0.8.0/cascade/utils/
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     1339 2022-11-15 22:00:08.000000 cascade-ml-0.8.0/cascade/utils/__init__.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     1566 2022-10-06 09:46:54.000000 cascade-ml-0.8.0/cascade/utils/baselines.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     1117 2022-09-23 15:03:14.000000 cascade-ml-0.8.0/cascade/utils/folder_image_dataset.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)      757 2022-09-23 15:03:14.000000 cascade-ml-0.8.0/cascade/utils/model_aggregate.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)      996 2022-10-06 09:46:54.000000 cascade-ml-0.8.0/cascade/utils/numpy_wrapper.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     2324 2022-11-15 22:00:08.000000 cascade-ml-0.8.0/cascade/utils/oversampler.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     1213 2022-11-15 22:00:08.000000 cascade-ml-0.8.0/cascade/utils/pa_schema_validator.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     3808 2022-11-15 22:00:08.000000 cascade-ml-0.8.0/cascade/utils/sk_model.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     6038 2022-11-15 22:00:08.000000 cascade-ml-0.8.0/cascade/utils/table_dataset.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     2490 2022-10-06 09:46:54.000000 cascade-ml-0.8.0/cascade/utils/text_classification_dataset.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     7346 2022-11-15 22:00:08.000000 cascade-ml-0.8.0/cascade/utils/time_series_dataset.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     1892 2022-10-06 09:46:54.000000 cascade-ml-0.8.0/cascade/utils/torch_model.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     2050 2022-11-15 22:00:08.000000 cascade-ml-0.8.0/cascade/utils/undersampler.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     3152 2022-11-15 22:00:08.000000 cascade-ml-0.8.0/cascade/utils/weighed_sampler.py
-drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2022-11-15 22:01:14.326391 cascade-ml-0.8.0/cascade_ml.egg-info/
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     5021 2022-11-15 22:01:14.000000 cascade-ml-0.8.0/cascade_ml.egg-info/PKG-INFO
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     2717 2022-11-15 22:01:14.000000 cascade-ml-0.8.0/cascade_ml.egg-info/SOURCES.txt
--rw-rw-r--   0 ilia      (1000) ilia      (1000)        1 2022-11-15 22:01:14.000000 cascade-ml-0.8.0/cascade_ml.egg-info/dependency_links.txt
--rw-rw-r--   0 ilia      (1000) ilia      (1000)      122 2022-11-15 22:01:14.000000 cascade-ml-0.8.0/cascade_ml.egg-info/requires.txt
--rw-rw-r--   0 ilia      (1000) ilia      (1000)        8 2022-11-15 22:01:14.000000 cascade-ml-0.8.0/cascade_ml.egg-info/top_level.txt
--rw-rw-r--   0 ilia      (1000) ilia      (1000)       87 2022-09-23 15:03:14.000000 cascade-ml-0.8.0/pyproject.toml
--rw-rw-r--   0 ilia      (1000) ilia      (1000)      318 2022-11-15 22:01:14.326391 cascade-ml-0.8.0/setup.cfg
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     1061 2022-11-15 22:00:08.000000 cascade-ml-0.8.0/setup.py
+drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2022-12-16 15:06:04.088738 cascade-ml-0.9.0/
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)    11328 2022-09-03 15:51:41.000000 cascade-ml-0.9.0/LICENSE
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     5021 2022-12-16 15:06:04.088738 cascade-ml-0.9.0/PKG-INFO
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     4560 2022-09-29 10:07:30.000000 cascade-ml-0.9.0/README.md
+drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2022-12-16 15:06:04.080738 cascade-ml-0.9.0/cascade/
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)      972 2022-12-16 15:04:52.000000 cascade-ml-0.9.0/cascade/__init__.py
+drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2022-12-16 15:06:04.080738 cascade-ml-0.9.0/cascade/base/
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)      782 2022-12-16 15:04:52.000000 cascade-ml-0.9.0/cascade/base/__init__.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     6721 2022-12-16 15:04:52.000000 cascade-ml-0.9.0/cascade/base/meta_handler.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     3164 2022-12-16 15:04:52.000000 cascade-ml-0.9.0/cascade/base/traceable.py
+drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2022-12-16 15:06:04.080738 cascade-ml-0.9.0/cascade/data/
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     1121 2022-12-16 15:04:52.000000 cascade-ml-0.9.0/cascade/data/__init__.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     1709 2022-12-16 15:04:52.000000 cascade-ml-0.9.0/cascade/data/apply_modifier.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     2426 2022-12-16 15:04:52.000000 cascade-ml-0.9.0/cascade/data/bruteforce_cacher.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     2280 2022-12-16 15:04:52.000000 cascade-ml-0.9.0/cascade/data/composer.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     2515 2022-12-16 15:04:52.000000 cascade-ml-0.9.0/cascade/data/concatenator.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     1072 2022-12-16 15:04:52.000000 cascade-ml-0.9.0/cascade/data/cyclic_sampler.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     6296 2022-12-16 15:04:52.000000 cascade-ml-0.9.0/cascade/data/dataset.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     2040 2022-12-16 15:04:52.000000 cascade-ml-0.9.0/cascade/data/folder_dataset.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     2033 2022-12-16 15:04:52.000000 cascade-ml-0.9.0/cascade/data/pickler.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     1888 2022-12-16 15:04:52.000000 cascade-ml-0.9.0/cascade/data/random_sampler.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     2788 2022-12-16 15:04:52.000000 cascade-ml-0.9.0/cascade/data/range_sampler.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     2191 2022-12-16 15:04:52.000000 cascade-ml-0.9.0/cascade/data/sequential_cacher.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     1963 2022-12-16 15:04:52.000000 cascade-ml-0.9.0/cascade/data/utils.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     6540 2022-12-16 15:04:52.000000 cascade-ml-0.9.0/cascade/data/version_assigner.py
+drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2022-12-16 15:06:04.080738 cascade-ml-0.9.0/cascade/meta/
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)      927 2022-12-16 15:04:52.000000 cascade-ml-0.9.0/cascade/meta/__init__.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     1970 2022-12-16 15:04:52.000000 cascade-ml-0.9.0/cascade/meta/dataleak_validator.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)      680 2022-12-16 15:04:52.000000 cascade-ml-0.9.0/cascade/meta/hashes.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     8234 2022-12-16 15:04:52.000000 cascade-ml-0.9.0/cascade/meta/history_viewer.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     4158 2022-12-16 15:04:52.000000 cascade-ml-0.9.0/cascade/meta/meta_validator.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     2964 2022-12-16 15:04:52.000000 cascade-ml-0.9.0/cascade/meta/meta_viewer.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     9469 2022-12-16 15:04:52.000000 cascade-ml-0.9.0/cascade/meta/metric_viewer.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     2072 2022-12-16 15:04:52.000000 cascade-ml-0.9.0/cascade/meta/utils.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     3729 2022-12-16 15:04:52.000000 cascade-ml-0.9.0/cascade/meta/validator.py
+drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2022-12-16 15:06:04.080738 cascade-ml-0.9.0/cascade/models/
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)      768 2022-09-23 15:03:14.000000 cascade-ml-0.9.0/cascade/models/__init__.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     2484 2022-12-16 15:04:52.000000 cascade-ml-0.9.0/cascade/models/basic_model.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     4237 2022-12-16 15:04:52.000000 cascade-ml-0.9.0/cascade/models/model.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     5768 2022-12-16 15:04:52.000000 cascade-ml-0.9.0/cascade/models/model_line.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)    10376 2022-12-16 15:04:52.000000 cascade-ml-0.9.0/cascade/models/model_repo.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     6829 2022-12-16 15:04:52.000000 cascade-ml-0.9.0/cascade/models/trainer.py
+drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2022-12-16 15:06:04.084738 cascade-ml-0.9.0/cascade/tests/
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)      605 2022-12-16 15:04:52.000000 cascade-ml-0.9.0/cascade/tests/__init__.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     4341 2022-12-16 15:04:52.000000 cascade-ml-0.9.0/cascade/tests/conftest.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     1102 2022-09-23 15:03:14.000000 cascade-ml-0.9.0/cascade/tests/test_apply_modifier.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     2088 2022-09-05 21:14:08.000000 cascade-ml-0.9.0/cascade/tests/test_basic_model.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     1201 2022-09-23 15:03:14.000000 cascade-ml-0.9.0/cascade/tests/test_bruteforce_cacher.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     1630 2022-11-15 22:00:08.000000 cascade-ml-0.9.0/cascade/tests/test_composer.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     1387 2022-12-16 15:04:52.000000 cascade-ml-0.9.0/cascade/tests/test_concatenator.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)      970 2022-09-23 15:03:14.000000 cascade-ml-0.9.0/cascade/tests/test_cyclic_sampler.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     1565 2022-12-16 15:04:52.000000 cascade-ml-0.9.0/cascade/tests/test_data_split.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     1780 2022-11-15 22:00:08.000000 cascade-ml-0.9.0/cascade/tests/test_dataleak_validator.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     2485 2022-12-16 15:04:52.000000 cascade-ml-0.9.0/cascade/tests/test_dataset.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     1143 2022-09-23 15:03:14.000000 cascade-ml-0.9.0/cascade/tests/test_folder_dataset.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     2172 2022-09-23 15:03:14.000000 cascade-ml-0.9.0/cascade/tests/test_history_viewer.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     3382 2022-12-16 15:04:52.000000 cascade-ml-0.9.0/cascade/tests/test_meta_handler.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     1215 2022-12-16 15:04:52.000000 cascade-ml-0.9.0/cascade/tests/test_meta_validator.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     2027 2022-11-15 22:00:08.000000 cascade-ml-0.9.0/cascade/tests/test_meta_viewer.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     3239 2022-12-16 15:04:52.000000 cascade-ml-0.9.0/cascade/tests/test_metric_viewer.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     1118 2022-09-23 15:03:14.000000 cascade-ml-0.9.0/cascade/tests/test_model_line.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     9379 2022-11-15 22:00:08.000000 cascade-ml-0.9.0/cascade/tests/test_model_repo.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     1028 2022-09-23 15:03:14.000000 cascade-ml-0.9.0/cascade/tests/test_modifier.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     1586 2022-12-16 15:04:52.000000 cascade-ml-0.9.0/cascade/tests/test_pickler.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     1459 2022-09-23 15:03:14.000000 cascade-ml-0.9.0/cascade/tests/test_random_sampler.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     1535 2022-12-16 15:04:52.000000 cascade-ml-0.9.0/cascade/tests/test_range_sampler.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     1267 2022-12-16 15:04:52.000000 cascade-ml-0.9.0/cascade/tests/test_sequential_cacher.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     1868 2022-12-16 15:04:52.000000 cascade-ml-0.9.0/cascade/tests/test_traceable.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     1539 2022-12-16 15:04:52.000000 cascade-ml-0.9.0/cascade/tests/test_trainer.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     2060 2022-09-23 15:03:14.000000 cascade-ml-0.9.0/cascade/tests/test_validator.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     2053 2022-12-16 15:04:52.000000 cascade-ml-0.9.0/cascade/tests/test_version_assigner.py
+drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2022-12-16 15:06:04.088738 cascade-ml-0.9.0/cascade/utils/
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     1339 2022-11-15 22:00:08.000000 cascade-ml-0.9.0/cascade/utils/__init__.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     1875 2022-12-16 15:04:52.000000 cascade-ml-0.9.0/cascade/utils/baselines.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     1133 2022-12-16 15:04:52.000000 cascade-ml-0.9.0/cascade/utils/folder_image_dataset.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)      757 2022-09-23 15:03:14.000000 cascade-ml-0.9.0/cascade/utils/model_aggregate.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     1049 2022-12-16 15:04:52.000000 cascade-ml-0.9.0/cascade/utils/numpy_wrapper.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     2403 2022-12-16 15:04:52.000000 cascade-ml-0.9.0/cascade/utils/oversampler.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     1864 2022-12-16 15:04:52.000000 cascade-ml-0.9.0/cascade/utils/pa_schema_validator.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     3950 2022-12-16 15:04:52.000000 cascade-ml-0.9.0/cascade/utils/sk_model.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     6348 2022-12-16 15:04:52.000000 cascade-ml-0.9.0/cascade/utils/table_dataset.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     2557 2022-12-16 15:04:52.000000 cascade-ml-0.9.0/cascade/utils/text_classification_dataset.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     8739 2022-12-16 15:04:52.000000 cascade-ml-0.9.0/cascade/utils/time_series_dataset.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     1965 2022-12-16 15:04:52.000000 cascade-ml-0.9.0/cascade/utils/torch_model.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     2194 2022-12-16 15:04:52.000000 cascade-ml-0.9.0/cascade/utils/undersampler.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     3726 2022-12-16 15:04:52.000000 cascade-ml-0.9.0/cascade/utils/weighed_sampler.py
+drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2022-12-16 15:06:04.088738 cascade-ml-0.9.0/cascade_ml.egg-info/
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     5021 2022-12-16 15:06:04.000000 cascade-ml-0.9.0/cascade_ml.egg-info/PKG-INFO
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     2701 2022-12-16 15:06:04.000000 cascade-ml-0.9.0/cascade_ml.egg-info/SOURCES.txt
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)        1 2022-12-16 15:06:04.000000 cascade-ml-0.9.0/cascade_ml.egg-info/dependency_links.txt
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)      122 2022-12-16 15:06:04.000000 cascade-ml-0.9.0/cascade_ml.egg-info/requires.txt
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)        8 2022-12-16 15:06:04.000000 cascade-ml-0.9.0/cascade_ml.egg-info/top_level.txt
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)       87 2022-09-23 15:03:14.000000 cascade-ml-0.9.0/pyproject.toml
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)      318 2022-12-16 15:06:04.088738 cascade-ml-0.9.0/setup.cfg
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     1061 2022-12-16 15:04:52.000000 cascade-ml-0.9.0/setup.py
```

### Comparing `cascade-ml-0.8.0/LICENSE` & `cascade-ml-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cascade-ml-0.8.0/PKG-INFO` & `cascade-ml-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cascade-ml
-Version: 0.8.0
+Version: 0.9.0
 Summary: ML-Engineering library
 Home-page: https://github.com/oxid15/cascade
 Author: Ilia Moiseev
 Author-email: ilia.moiseev.5@yandex.ru
 License: Apache License 2.0
 Project-URL: Documentation, https://oxid15.github.io/cascade
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cascade-ml-0.8.0/README.md` & `cascade-ml-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `cascade-ml-0.8.0/cascade/base/meta_handler.py` & `cascade-ml-0.9.0/cascade/base/meta_handler.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,26 +13,27 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import os
 import json
 import datetime
-from typing import Union, List, Dict
+from typing import NoReturn, Union, List, Dict, Any
 from json import JSONEncoder
 
 import yaml
 import numpy as np
 
+from . import Meta
 
 supported_meta_formats = ('.json', '.yml')
 
 
 class CustomEncoder(JSONEncoder):
-    def default(self, obj):
+    def default(self, obj: Any) -> Any:
         if isinstance(obj, type):
             return str(obj)
 
         if isinstance(obj, (datetime.datetime, datetime.date, datetime.time)):
             return obj.isoformat()
 
         elif isinstance(obj, datetime.timedelta):
@@ -56,69 +57,76 @@
             return bool(obj)
 
         elif isinstance(obj, np.void):
             return None
 
         return super(CustomEncoder, self).default(obj)
 
-    def obj_to_dict(self, obj) -> Dict:
+    def obj_to_dict(self, obj: Any) -> Dict:
         return json.loads(self.encode(obj))
 
 
 class BaseHandler:
-    def read(self, path: str) -> Union[Dict, List[Dict]]:
+    def read(self, path: str) -> Union[List[Any], Dict[Any, Any]]:
         raise NotImplementedError()
 
-    def write(self, path: str, obj, overwrite=True) -> None:
+    def write(self, path: str, obj: Any, overwrite: bool = True) -> None:
         raise NotImplementedError()
 
-    def _raise_io_error(self, path, exc):
+    def _raise_io_error(self, path: str, exc: Union[Exception, None] = None) -> NoReturn:
         # Any file decoding errors will be
         # prepended with filepath for user
         # to be able to identify broken file
-        raise IOError(f'Error while reading file `{path}`') from exc
+        if exc is not None:
+            raise IOError(f'Error while reading file `{path}`') from exc
+        else:
+            raise IOError(f'Error while reading file `{path}`')
 
 
 class JSONHandler(BaseHandler):
-    def read(self, path: str) -> Union[Dict, List[Dict]]:
+    def read(self, path: str) -> Union[List[Any], Dict[Any, Any]]:
         _, ext = os.path.splitext(path)
         if ext == '':
             path += '.json'
 
         with open(path, 'r') as meta_file:
             try:
                 meta = json.load(meta_file)
                 if isinstance(meta, str):
                     meta = json.loads(meta)
             except json.JSONDecodeError as e:
                 self._raise_io_error(path, e)
             return meta
 
-    def write(self, path: str, obj: List[Dict], overwrite=True) -> None:
+    def write(self, path: str, obj: List[Dict], overwrite: bool = True) -> None:
         if not overwrite and os.path.exists(path):
             return
 
         with open(path, 'w') as f:
             json.dump(obj, f, cls=CustomEncoder, indent=4)
 
 
 class YAMLHandler(BaseHandler):
-    def read(self, path: str) -> Union[Dict, List[Dict]]:
+    def read(self, path: str) -> Union[List[Any], Dict[Any, Any]]:
         _, ext = os.path.splitext(path)
         if ext == '':
             path += '.yml'
 
         with open(path, 'r') as meta_file:
             try:
                 meta = yaml.safe_load(meta_file)
+
+                # Safe load may return None if something wrong
+                if meta is None:
+                    self._raise_io_error(path)
             except yaml.YAMLError as e:
                 self._raise_io_error(path, e)
             return meta
 
-    def write(self, path: str, obj, overwrite=True) -> None:
+    def write(self, path: str, obj: Any, overwrite: bool = True) -> None:
         if not overwrite and os.path.exists(path):
             return
 
         obj = CustomEncoder().obj_to_dict(obj)
         with open(path, 'w') as f:
             yaml.safe_dump(obj, f)
 
@@ -135,15 +143,15 @@
             Path to the file
         """
 
         with open(path, 'r') as meta_file:
             meta = {path: ''.join(meta_file.readlines())}
             return meta
 
-    def write(self, path, obj, overwrite=True) -> None:
+    def write(self, path: str, obj: Any, overwrite: bool = True) -> NoReturn:
         raise NotImplementedError(
             'MetaHandler does not write text files, only reads')
 
 
 class MetaHandler:
     """
     Encapsulates the logic of reading and writing metadata to disk.
@@ -156,36 +164,36 @@
     >>> from cascade.base import MetaHandler
     >>> mh = MetaHandler()
     >>> mh.write('meta.json', {'hello': 'world'})
     >>> obj = mh.read('meta.json')
     >>> mh.write('meta.yml', {'hello': 'world'})
     >>> obj = mh.read('meta.yml')
     """
-    def read(self, path: str) -> Union[Dict, List[Dict]]:
+    def read(self, path: str) -> Union[List[Any], Dict[Any, Any]]:
         """
         Reads object from path.
 
         Parameters
         ----------
             path: str
                 Path to the object.
 
         Returns
         -------
-            obj: Union[Dict, List[Dict]]
+            obj: Union[List[Any], Dict[Any, Any]]
 
         Raises
         ------
         IOError
             when decoding errors occur
         """
         handler = self._get_handler(path)
         return handler.read(path)
 
-    def write(self, path: str, obj, overwrite: bool = True) -> None:
+    def write(self, path: str, obj: Any, overwrite: bool = True) -> None:
         """
         Writes object to path.
 
         Parameters
         ----------
             path: str
                 Path where to write object with name and extension
@@ -199,15 +207,15 @@
         ------
         IOError
             when encoding errors occur
         """
         handler = self._get_handler(path)
         return handler.write(path, obj, overwrite=overwrite)
 
-    def _get_handler(self, path) -> BaseHandler:
+    def _get_handler(self, path: str) -> BaseHandler:
         ext = os.path.splitext(path)[-1]
         if ext == '.json':
             return JSONHandler()
         elif ext == '.yml':
             return YAMLHandler()
         else:
             return TextHandler()
```

### Comparing `cascade-ml-0.8.0/cascade/data/__init__.py` & `cascade-ml-0.9.0/cascade/data/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from .dataset import Dataset, Modifier, Sampler, T, Wrapper, Iterator
+from .dataset import Dataset, Modifier, Sampler, T, Wrapper, Iterator, SizedDataset
 
 from .apply_modifier import ApplyModifier
 from .bruteforce_cacher import BruteforceCacher
 from .sequential_cacher import SequentialCacher
 from .composer import Composer
 from .concatenator import Concatenator
 from .cyclic_sampler import CyclicSampler
```

### Comparing `cascade-ml-0.8.0/cascade/data/apply_modifier.py` & `cascade-ml-0.9.0/cascade/data/apply_modifier.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,23 +10,24 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from typing import Callable
+from typing import Callable, Any, List, Dict
 from . import Dataset, Modifier, T
 
 
 class ApplyModifier(Modifier):
     """
     Modifier that maps a function to given dataset's items in a lazy way.
     """
-    def __init__(self, dataset: Dataset, func: Callable, *args, **kwargs) -> None:
+    def __init__(self, dataset: Dataset[T], func: Callable[[T], Any],
+                 *args: List[Any], **kwargs: Dict[Any, Any]) -> None:
         """
         Parameters
         ----------
         dataset: Dataset
             A dataset to modify
         func: Callable
             A function to be applied to every item of a dataset -
@@ -41,10 +42,10 @@
         Now function will only be applied when items are retrieved
 
         >>> assert [item for item in ds] == [0, 1, 4, 9, 16]
         """
         super().__init__(dataset, *args, **kwargs)
         self._func = func
 
-    def __getitem__(self, index: int) -> T:
+    def __getitem__(self, index: int) -> Any:
         item = self._dataset[index]
         return self._func(item)
```

### Comparing `cascade-ml-0.8.0/cascade/data/bruteforce_cacher.py` & `cascade-ml-0.9.0/cascade/data/bruteforce_cacher.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
+from typing import Any
 from tqdm import tqdm, trange
 from . import Dataset, Modifier, T
 
 
 class BruteforceCacher(Modifier):
     """
     Identity modifier that calls all previous pipeline in __init__ loading everything
@@ -47,25 +48,28 @@
     >>> ds = cdd.RandomSampler(ds, 1000)
 
     See also
     --------
     cascade.data.SequentialCacher
     cascade.data.Pickler
     """
-    def __init__(self, dataset: Dataset, *args, **kwargs) -> None:
+    def __init__(self, dataset: Dataset[T],
+                 *args: Any, **kwargs: Any) -> None:
         """
         Loads every item in dataset in internal list.
         """
         super().__init__(dataset, *args, **kwargs)
         # forcibly calling all previous datasets in the init
         if hasattr(self._dataset, '__len__') and hasattr(self._dataset, '__getitem__'):
             self._data = [self._dataset[i] for i in trange(len(self._dataset))]
         elif hasattr(self._dataset, '__iter__'):
             self._data = [item for item in tqdm(self._dataset)]
         else:
-            raise AttributeError('Input dataset must provide Mapping or Iterable interface')
+            raise AttributeError(
+                'Input dataset must provide __len__ and __getitem__ or __iter__'
+            )
 
-    def __getitem__(self, index) -> T:
+    def __getitem__(self, index: int) -> T:
         return self._data[index]
 
-    def __len__(self):
+    def __len__(self) -> int:
         return len(self._data)
```

### Comparing `cascade-ml-0.8.0/cascade/data/concatenator.py` & `cascade-ml-0.9.0/cascade/data/concatenator.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,47 +10,48 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from typing import List, Dict, Iterable
+from typing import List, Any
 
 import numpy as np
-from .dataset import Dataset, T
+from .dataset import SizedDataset, T
+from ..base import Meta
 
 
-class Concatenator(Dataset):
+class Concatenator(SizedDataset):
     """
     Unifies several Datasets under one, calling them sequentially in the provided order.
 
     Examples
     --------
     >>> from cascade.data import Wrapper, Concatenator
     >>> ds_1 = Wrapper([0, 1, 2])
     >>> ds_2 = Wrapper([2, 1, 0])
     >>> ds = Concatenator((ds_1, ds_2))
     >>> assert [item for item in ds] == [0, 1, 2, 2, 1, 0]
     """
-    def __init__(self, datasets: Iterable[Dataset], *args, **kwargs) -> None:
+    def __init__(self, datasets: List[SizedDataset[T]], *args: Any, **kwargs: Any) -> None:
         """
         Creates concatenated dataset from the list of datasets provided
 
         Parameters
         ----------
         datasets: Union[Iterable[Dataset], Mapping[Dataset]]
             A list or tuple of datasets to concatenate
         """
         self._datasets = datasets
         lengths = [len(ds) for ds in self._datasets]
         self._shifts = np.cumsum([0] + lengths)
         super().__init__(*args, **kwargs)
 
-    def __getitem__(self, index) -> T:
+    def __getitem__(self, index: int) -> T:
         ds_index = 0
         for sh in self._shifts[1:]:
             if index >= sh:
                 ds_index += 1
         return self._datasets[ds_index][index - self._shifts[ds_index]]
 
     def __len__(self) -> int:
@@ -66,14 +67,14 @@
         Dataset1
         Dataset2
         ...
         """
         rp = super().__repr__()
         return f'{rp} of\n' + '\n'.join(repr(ds) for ds in self._datasets)
 
-    def get_meta(self) -> List[Dict]:
+    def get_meta(self) -> Meta:
         """
         Concatenator calls `get_meta()` of all its datasets
         """
         meta = super().get_meta()
         meta[0]['data'] = [ds.get_meta() for ds in self._datasets]
         return meta
```

### Comparing `cascade-ml-0.8.0/cascade/data/cyclic_sampler.py` & `cascade-ml-0.9.0/cascade/data/cyclic_sampler.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,10 +24,10 @@
     Example
     -------
     >>> from cascade.data import CyclicSampler, Wrapper
     >>> ds = Wrapper([1,2,3])
     >>> ds = CyclicSampler(ds, 7)
     >>> assert [item for item in ds] == [1, 2, 3, 1, 2, 3, 1]
     """
-    def __getitem__(self, index) -> T:
+    def __getitem__(self, index: int) -> T:
         internal_index = index % len(self._dataset)
         return self._dataset[internal_index]
```

### Comparing `cascade-ml-0.8.0/cascade/data/dataset.py` & `cascade-ml-0.9.0/cascade/data/dataset.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from typing import Dict, Generic, Iterable, List, Mapping, TypeVar
-from ..base import Traceable
+from typing import Dict, Generic, Iterable, List, TypeVar, Any, Sized, Sequence
+from ..base import Traceable, Meta
 
 T = TypeVar('T')
 
 
 class Dataset(Generic[T], Traceable):
     """
     Base class of any module that constitutes a data-pipeline.
@@ -24,28 +24,28 @@
     It does not define `__len__` for similar reasons.
     See `pytorch/torch/utils/data/sampler.py` note on this topic.
 
     See also
     --------
     cascade.base.Traceable
     """
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
         super().__init__(**kwargs)
 
-    def __getitem__(self, index) -> T:
+    def __getitem__(self, index: int) -> T:
         """
         Abstract method - should be defined in every successor
         """
         raise NotImplementedError()
 
-    def get_meta(self) -> List[Dict]:
+    def get_meta(self) -> Meta:
         """
         Returns
         -------
-        meta: List[Dict]
+        meta: Meta
             A list where last element is this dataset's metadata.
             Meta can be anything that is worth to document about the dataset and its data.
             This is done in form of list to enable cascade-like calls in Modifiers and Samplers.
         """
         meta = super().get_meta()
         meta[0]['type'] = 'dataset'
         return meta
@@ -58,114 +58,134 @@
             Representation of a Dataset. This repr used as a name for get_meta() method
             by default gives the name of class from basic repr
 
         See also
         --------
         cascade.data.Dataset.get_meta()
         """
-        return super().__repr__().split()[0]
+        # Removes adress part of basic object repr and leading < symbol
+        return super().__repr__().split()[0][1:]
+
+
+class SizedDataset(Dataset[T], Sized):
+    """
+    An abstract class to represent a dataset
+    with __len__ method present. Inheritance of
+    this class should mean the presence of length.
+
+    If your dataset does not have length defined, please
+    use Dataset.
+
+    See also
+    --------
+    cascade.data.Dataset
+    """
+    def len(self) -> int:
+        raise NotImplementedError()
 
 
 class Iterator(Dataset):
     """
     Wraps Dataset around any Iterable. Does not have map-like interface.
     """
-    def __init__(self, data: Iterable, *args, **kwargs):
+    def __init__(self, data: Iterable[T], *args: Any, **kwargs: Any) -> None:
         super().__init__(*args, **kwargs)
         self._data = data
 
-    def __getitem__(self, item):
+    def __getitem__(self, item: int) -> T:
         raise NotImplementedError()
 
-    def __iter__(self):
+    def __iter__(self) -> Iterable[T]:
         for item in self._data:
             yield item
 
-    def get_meta(self):
+    def get_meta(self) -> Meta:
         meta = super().get_meta()
         meta[0]['obj_type'] = str(type(self._data))
         return meta
 
 
-class Wrapper(Dataset):
+class Wrapper(SizedDataset):
     """
     Wraps Dataset around any list-like object.
     """
-    def __init__(self, obj: Mapping, *args, **kwargs) -> None:
+    def __init__(self, obj: Sequence[T], *args: Any, **kwargs: Any) -> None:
         self._data = obj
         super().__init__(*args, **kwargs)
 
-    def __getitem__(self, index) -> T:
+    def __getitem__(self, index: int) -> T:
         return self._data[index]
 
     def __len__(self) -> int:
         return len(self._data)
 
-    def get_meta(self):
+    def get_meta(self) -> Meta:
         meta = super().get_meta()
         meta[0]['len'] = len(self)
         meta[0]['obj_type'] = str(type(self._data))
         return meta
 
 
-class Modifier(Dataset):
+class Modifier(SizedDataset):
     """
-    Basic pipeline building block in Cascade. Every block which is not a data source should be a successor
-    of Sampler or Modifier.
+    Basic pipeline building block in Cascade. Every block which is not a data source should be
+    a successor of Sampler or Modifier.
     This structure enables a workflow, when we have a data pipeline which consists of uniform blocks
-    each of them has a reference to the previous one in its `_dataset` field. See get_meta method for example.
+    each of them has a reference to the previous one in its `_dataset` field. See get_meta method
+    for example.
     Basically Modifier defines an arbitrary transformation on every dataset's item that is applied
     in a lazy manner on each `__getitem__` call.
     Applies no transformation if `__getitem__` is not overridden.
     """
-    def __init__(self, dataset: Dataset, *args, **kwargs) -> None:
+    def __init__(self, dataset: SizedDataset[T], *args: Any, **kwargs: Any) -> None:
         """
         Constructs a Modifier. Makes no transformations in initialization.
         Parameters
         ----------
         dataset: Dataset
             A dataset to modify
         """
         self._dataset = dataset
         super().__init__(*args, **kwargs)
 
-    def __getitem__(self, index) -> T:
+    def __getitem__(self, index: int) -> T:
         return self._dataset[index]
 
     def __iter__(self) -> T:
         for i in range(len(self)):
             yield self.__getitem__(i)
 
     def __len__(self) -> int:
         return len(self._dataset)
 
-    def get_meta(self) -> List[Dict]:
+    def get_meta(self) -> Meta:
         """
         Overrides base method enabling cascade-like calls to previous datasets.
         The metadata of a pipeline that consist of several modifiers can be easily
         obtained with `get_meta` of the last block.
         """
         self_meta = super().get_meta()
         self_meta[0]['len'] = len(self)
         self_meta += self._dataset.get_meta()
         return self_meta
 
 
 class Sampler(Modifier):
     """
-    Defines certain sampling over a Dataset. Its distinctive feature is that it changes the number of
-    items in dataset. It can be used to build a batch sampler, random sampler, etc.
+    Defines certain sampling over a Dataset. Its distinctive feature is that it changes the number
+    of items in dataset. It can be used to build a batch sampler, random sampler, etc.
 
     See also
     --------
     cascade.data.CyclicSampler
     cascade.data.RandomSampler
     cascade.data.RangeSampler
     """
-    def __init__(self, dataset: Dataset, num_samples: int, *args, **kwargs) -> None:
+    def __init__(self, dataset: SizedDataset[T], num_samples: int,
+                 *args: Any, **kwargs: Any) -> None:
         """
         Constructs a Sampler.
 
         Parameters
         ----------
             dataset: Dataset
                 A dataset to sample from
```

### Comparing `cascade-ml-0.8.0/cascade/data/pickler.py` & `cascade-ml-0.9.0/cascade/data/pickler.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,23 +11,27 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import os
+from typing import Union, Any
 import pickle
-from . import Dataset, Modifier
+from . import Dataset, Modifier, T
 
 
 class Pickler(Modifier):
     """
     Pickles input dataset or unpickles one
     """
-    def __init__(self, path: str, dataset: Dataset = None, *args, **kwargs) -> None:
+    def __init__(self,
+                 path: str,
+                 dataset: Union[Dataset[T], None] = None,
+                 *args: Any, **kwargs: Any) -> None:
         """
         Loads pickled dataset or dumps one depending on parameters passed:
 
         1. If only path is passed - loads dataset from path provided if path exists
         2. if path provided with a dataset dumps dataset to the path
 
         Parameters
@@ -56,12 +60,12 @@
         with open(self._path, 'wb') as f:
             pickle.dump(self._dataset, f)
 
     def _load(self) -> None:
         with open(self._path, 'rb') as f:
             self._dataset = pickle.load(f)
 
-    def ds(self):
+    def ds(self) -> Dataset[T]:
         """
         Returns pickled dataset
         """
         return self._dataset
```

### Comparing `cascade-ml-0.8.0/cascade/data/random_sampler.py` & `cascade-ml-0.9.0/cascade/data/random_sampler.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,24 +10,26 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
+from typing import Any, Union
 from numpy.random import random_integers, shuffle
-from . import Dataset, Sampler, T
+from . import SizedDataset, Sampler, T
 
 
 class RandomSampler(Sampler):
     """
     Shuffles dataset. Can randomly sample from dataset
     if num_samples is not None and less than length of dataset.
     """
-    def __init__(self, dataset: Dataset, num_samples: int = None, **kwargs) -> None:
+    def __init__(self, dataset: SizedDataset[T], num_samples: Union[int, None] = None,
+                 *args: Any, **kwargs: Any) -> None:
         """
         Parameters
         ----------
         dataset: Dataset
             Input dataset to sample from
         num_samples: int, optional
             If less or equal than len(dataset) samples without repetitions (shuffles indices).
@@ -40,9 +42,9 @@
             self._indices = [i for i in range(len(dataset))]
             shuffle(self._indices)
             self._indices = self._indices[:num_samples]
         else:
             self._indices = random_integers(0, len(dataset) - 1, num_samples)
         super().__init__(dataset, num_samples, **kwargs)
 
-    def __getitem__(self, index) -> T:
+    def __getitem__(self, index: int) -> T:
         return super().__getitem__(self._indices[index])
```

### Comparing `cascade-ml-0.8.0/cascade/data/range_sampler.py` & `cascade-ml-0.9.0/cascade/data/range_sampler.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-
-from . import T, Dataset, Sampler
+from typing import Any, Union
+from . import T, SizedDataset, Sampler
 
 
 class RangeSampler(Sampler):
     """
     Implements an interface of standard range in a dataset.
 
     Example
@@ -40,34 +40,54 @@
     ...
     1
     2
     3
     """
     def __init__(
             self,
-            dataset: Dataset,
-            start: int = None,
-            stop: int = None,
-            step: int = 1,
-            *args, **kwargs) -> None:
+            dataset: SizedDataset[T],
+            start: Union[int, None] = None,
+            stop: Union[int, None] = None,
+            step: Union[int, None] = 1,
+            *args: Any, **kwargs: Any) -> None:
         """
         Parameters
         ----------
-            dataset: Dataset
-                A dataset to sampler from
+            dataset: SizedDataset
+                A dataset to sample from
             start: int
                 Start index in range - included
             stop: int
                 Stop index in range - excluded
             step: int, optional
                 Step of range
+        Raises
+        ------
+        ValueError: when no start or stop present or
+        when parameters given produce empty dataset
         """
+
+        # Check if can build range
+        if start is None and stop is None:
+            raise ValueError(
+                f"Either start or stop must be present\
+                Got start = {start}, stop = {stop}"
+            )
+
+        # Check if only stop was passed
         if start is not None and stop is None:
             stop = start
             start = 0
 
         self._indices = [i for i in range(start, stop, step)]
+
+        if len(self._indices) == 0:
+            raise ValueError(
+                f'Given combination of start, stop and step'
+                f'produced empty dataset. Got start = {start}, stop = {stop}, step = {step}'
+            )
+
         super().__init__(dataset, len(self._indices), *args, **kwargs)
 
-    def __getitem__(self, index) -> T:
+    def __getitem__(self, index: int) -> T:
         internal_index = self._indices[index]
         return super().__getitem__(internal_index)
```

### Comparing `cascade-ml-0.8.0/cascade/data/sequential_cacher.py` & `cascade-ml-0.9.0/cascade/data/sequential_cacher.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,63 +10,66 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from . import Dataset, Modifier, T
+from typing import Any
+
+from . import SizedDataset, Modifier, T
 from numpy import ceil
 
 
 class SequentialCacher(Modifier):
     """
     A batched version of BruteforceCacher class.
 
-    On first `__getitem__` call loads a batch of length `batch_size` and until indices are in the same batch doesn't
+    On first `__getitem__` call loads a batch of length `batch_size` and until
+    indices are in the same batch doesn't
     load anything. When index misses a cached batch, then a new one is loaded.
 
     See also
     --------
     BruteforceCacher
     """
     def __init__(
             self,
-            dataset: Dataset,
+            dataset: SizedDataset[T],
             batch_size: int = 2,
-            *args, **kwargs) -> None:
+            *args: Any, **kwargs: Any) -> None:
         """
         Parameters
         ----------
         dataset: Dataset
             Dataset to cache sequentially
         batch_size: int, optional
             A number of items to load and keep in each moment
         """
-        # TODO: make something to release this assert
+
         assert hasattr(dataset, '__len__'), 'Dataset should have __len__'
         super().__init__(dataset, *args, **kwargs)
         self._bs = batch_size
         self._num_batches = int(ceil(len(self._dataset) / self._bs))
         self._index = -1
         self._batch = None
 
-    def _load(self, index) -> None:
+    def _load(self, index: int) -> None:
         del self._batch
         self._batch = []
 
         start = index * self._bs
         end = min(start + self._bs, len(self._dataset))
 
         for i in range(start, end):
             self._batch.append(self._dataset[i])
 
         self._index += 1
 
-    def __getitem__(self, index) -> T:
+    def __getitem__(self, index: int) -> T:
         batch_index = index // self._bs
         in_batch_idx = index % self._bs
 
         if batch_index != self._index:
             self._load(batch_index)
 
         return self._batch[in_batch_idx]
```

### Comparing `cascade-ml-0.8.0/cascade/data/version_assigner.py` & `cascade-ml-0.9.0/cascade/data/version_assigner.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,29 @@
+"""
+Copyright 2022 Ilia Moiseev
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+   http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+"""
+
 import os
 from hashlib import md5
-from typing import Dict, List
-from . import Dataset, Modifier
+from typing import Dict, List, Any, Tuple
+from . import Dataset, Modifier, T
 from ..base import MetaHandler, supported_meta_formats
+from ..meta import skeleton
 
 
 class VersionAssigner(Modifier):
     """
     Class for automatic data versioning using metadata.
     `VersionAssigner` is a simple `Modifier` that tracks changes in metadata and assigns
     dataset a version considering changes in meta.
@@ -55,15 +72,16 @@
     ---------
     In current implementation counts only highest-level pipeline changes.
     For example if final part of a pipeline is Concatenator will only
     count it and not the structure of a pipelines before.
     It is only applied to the major version changes and may be fixed in
     following versions.
     """
-    def __init__(self, dataset: Dataset, path: str, verbose=False, *args, **kwargs) -> None:
+    def __init__(self, dataset: Dataset[T], path: str, verbose: bool = False,
+                 *args: Any, **kwargs: Any) -> None:
         """
         Parameters
         ----------
             dataset: Dataset
                 a dataset to infer version to
             path: str
                 a path to a version log file of this dataset can be of any supported
@@ -72,23 +90,22 @@
         super().__init__(dataset, *args, **kwargs)
         self._mh = MetaHandler()
         self._assign_path(path)
         self._versions = {}
 
         # get meta for info about pipeline
         meta = self._dataset.get_meta()
+        pipeline = skeleton(meta)
 
-        # TODO: extract all names
-        # use whole meta and pipeline which is only first-level names
         meta_str = str(meta)
-        pipeline = ' '.join([m['name'] for m in meta])
+        pipeline_str = str(pipeline)
 
         # identify pipeline
         meta_hash = md5(str.encode(meta_str, 'utf-8')).hexdigest()
-        pipe_hash = md5(str.encode(pipeline, 'utf-8')).hexdigest()
+        pipe_hash = md5(str.encode(pipeline_str, 'utf-8')).hexdigest()
 
         if os.path.exists(self._root):
             self._versions = self._mh.read(self._root)
 
             if pipe_hash in self._versions:
                 if meta_hash in self._versions[pipe_hash]:
                     self.version = self._versions[pipe_hash][meta_hash]['version']
@@ -124,35 +141,35 @@
                 'pipeline': pipeline
             }
             self._mh.write(self._root, self._versions)
 
         if verbose:
             print('Dataset version:', self.version)
 
-    def _assign_path(self, path):
+    def _assign_path(self, path: str) -> None:
         _, ext = os.path.splitext(path)
         if ext == '':
             raise ValueError(f'Provided path {path} has no extension')
 
         assert ext in supported_meta_formats, f'Only {supported_meta_formats} are supported formats'
         self._root = path
 
-    def _split_ver(self, ver):
+    def _split_ver(self, ver: str) -> Tuple[int, int]:
         major, minor = ver.split('.')
         return int(major), int(minor)
 
-    def _join_ver(self, major, minor):
+    def _join_ver(self, major: int, minor: int) -> str:
         return f'{major}.{minor}'
 
-    def _get_last_version_from_pipe(self, pipe_hash):
+    def _get_last_version_from_pipe(self, pipe_hash: str) -> str:
         versions = [item['version'] for item in self._versions[pipe_hash].values()]
         versions = sorted(versions)
         return versions[-1]
 
-    def _get_last_version(self):
+    def _get_last_version(self) -> str:
         versions_flat = []
         for pipe_hash in self._versions:
             versions_flat += [item['version'] for item in self._versions[pipe_hash].values()]
         versions = sorted(versions_flat)
         return versions[-1]
 
     def get_meta(self) -> List[Dict]:
```

### Comparing `cascade-ml-0.8.0/cascade/meta/__init__.py` & `cascade-ml-0.9.0/cascade/meta/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,7 +17,8 @@
 from .meta_viewer import MetaViewer
 from .metric_viewer import MetricViewer
 from .validator import DataValidationException, Validator, AggregateValidator, PredicateValidator
 from .meta_validator import MetaValidator
 from .history_viewer import HistoryViewer
 from .dataleak_validator import DataleakValidator
 from .hashes import numpy_md5
+from .utils import skeleton
```

### Comparing `cascade-ml-0.8.0/cascade/meta/dataleak_validator.py` & `cascade-ml-0.9.0/cascade/meta/dataleak_validator.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,22 +10,30 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
+from typing import Callable, Union, Any
 from tqdm import tqdm
 
 from . import Validator, DataValidationException
 from .validator import prettify_items
+from ..data import Dataset, T
 
 
 class DataleakValidator(Validator):
-    def __init__(self, train_ds, test_ds, hash_fn=None, **kwargs) -> None:
+    def __init__(
+            self,
+            train_ds: Dataset[T],
+            test_ds: Dataset[T],
+            hash_fn: Union[Callable[[Any], str], None] = None,
+            **kwargs: Any
+    ) -> None:
         if hash_fn is None:
             hash_fn = hash
 
         train_hashes = [hash_fn(item) for item in tqdm(train_ds, desc='Retrieve train data')]
         test_hashes = [hash_fn(item) for item in tqdm(test_ds, desc='Retrieve test data')]
 
         train_repeating_idx = []
```

### Comparing `cascade-ml-0.8.0/cascade/meta/hashes.py` & `cascade-ml-0.9.0/cascade/meta/hashes.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,12 +10,13 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
+from typing import Any
 from hashlib import md5
 
 
-def numpy_md5(x) -> str:
+def numpy_md5(x: Any) -> str:
     return md5(x.tobytes()).hexdigest()
```

### Comparing `cascade-ml-0.8.0/cascade/meta/history_viewer.py` & `cascade-ml-0.9.0/cascade/meta/history_viewer.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,37 +10,39 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from typing import List
+from typing import List, Union, Dict, Any
+
 import pendulum
 import pandas as pd
 from flatten_json import flatten
 from deepdiff import DeepDiff
 import plotly
 from plotly import express as px
 from plotly import graph_objects as go
 
+from ..models import ModelRepo
 from . import MetaViewer
 
 
 class HistoryViewer:
     """
     The tool which allows user to visualize training history of model versions.
     Uses shows how metrics of models changed over time and how
     models with different hyperparameters depend on each other.
     """
     def __init__(
             self,
-            repo,
-            last_lines: int = None,
-            last_models: int = None) -> None:
+            repo: ModelRepo,
+            last_lines: Union[int, None] = None,
+            last_models: Union[int, None] = None) -> None:
         """
         Parameters
         ----------
         repo: cascade.models.ModelRepo
             Repo to be viewed
         last_lines: int, optional
             Constraints the number of lines back from the last one to view
@@ -48,24 +50,31 @@
             For each line constraints the number of models back from the last one to view
         """
         self._repo = repo
         self._last_lines = last_lines
         self._last_models = last_models
         self._make_table()
 
-    def _make_table(self):
+    def _make_table(self) -> None:
         metas = []
         params = []
-        # TODO: refactor this
-        for line in [*self._repo][::-1][:self._last_lines]:
+
+        line_names = self._repo.get_line_names()
+        if self._last_lines is not None:
+            # Takes last N lines in correct order
+            line_names = line_names[-self._last_lines:]
+
+        for line_name in line_names:
+            line = self._repo[line_name]
             view = MetaViewer(line.root, filt={'type': 'model'})
 
             for i in range(len(line))[:self._last_models]:
                 new_meta = {'line': line.root, 'num': i}
                 try:
+                    # TODO: to take only first is not good...
                     meta = view[i][0]
                 except IndexError:
                     meta = {}
 
                 new_meta.update(flatten(meta))
                 metas.append(new_meta)
 
@@ -79,15 +88,15 @@
 
         self._table = pd.DataFrame(metas)
         self._params = params
         if 'saved_at' in self._table:
             self._table = self._table.sort_values('saved_at')
 
     @staticmethod
-    def _diff(p1, params) -> List:
+    def _diff(p1: Dict[Any, Any], params: Dict[Any, Any]) -> List:
         diff = [DeepDiff(p1, p2) for p2 in params]
         changed = [0 for _ in range(len(params))]
         for i in range(len(changed)):
             if 'values_changed' in diff[i]:
                 changed[i] += len(diff[i]['values_changed'])
             if 'dictionary_item_added' in diff[i]:
                 changed[i] += len(diff[i]['dictionary_item_added'])
@@ -186,15 +195,15 @@
                 ticktext=time_text
             ))
         if show:
             fig.show()
 
         return fig
 
-    def serve(self, metric: str, **kwargs):
+    def serve(self, metric: str, **kwargs: Any) -> None:
         """
         Run dash-based server with HistoryViewer, updating plots in real-time.
 
         Note
         ----
         This feature needs `dash` to be installed.
         """
```

### Comparing `cascade-ml-0.8.0/cascade/meta/meta_viewer.py` & `cascade-ml-0.9.0/cascade/meta/meta_viewer.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,30 +12,30 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import os
 import warnings
-from typing import List, Dict
+from typing import Dict, Union, Any
 
-from ..base import MetaHandler, supported_meta_formats
+from ..base import MetaHandler, supported_meta_formats, Meta
 
 
 class MetaViewer:
     """
     The class to view all metadata in folders and subfolders.
     """
-    def __init__(self, root: str, filt: Dict = None) -> None:
+    def __init__(self, root: str, filt: Union[Dict[str, Any], None] = None) -> None:
         """
         Parameters
         ----------
         root: str
             path to the folder containing metadata files
-        filt Dict, optional:
+        filt: Dict, optional
             dictionary that specifies which values that should be present in meta
             for example to find all models use `filt={'type': 'model'}`
 
         See also
         --------
         cascade.meta.MetaHandler
         """
@@ -45,47 +45,50 @@
         self._root = root
         self._filt = filt
         self._mh = MetaHandler()
 
         self.names = []
         for root, _, files in os.walk(self._root):
             self.names += [os.path.join(root, name)
-                           for name in files if os.path.splitext(name)[-1] in supported_meta_formats]
+                           for name in files
+                           if os.path.splitext(name)[-1] in supported_meta_formats]
         self.names = sorted(self.names)
 
         if filt is not None:
             self.names = list(filter(self._filter, self.names))
 
-    def __getitem__(self, index: int) -> List[Dict]:
+    def __getitem__(self, index: int) -> Meta:
         """
         Returns
         -------
         meta: List[Dict]
             Meta object
         """
         return self._mh.read(self.names[index])
 
     def __len__(self) -> int:
         return len(self.names)
 
-    def write(self, path, obj: List[Dict]) -> None:
+    def write(self, path: str, obj: Meta) -> None:
         """
         Dumps obj to path
         """
-        warnings.warn('This method will be deprecated in future versions. Consider using MetaHandler instead.')
+        warnings.warn('This method will be deprecated in future versions. \
+            Consider using MetaHandler instead.')
         self._mh.write(path, obj)
 
-    def read(self, path) -> List[Dict]:
+    def read(self, path: str) -> Meta:
         """
         Loads object from path
         """
-        warnings.warn('This method will be deprecated in future versions. Consider using MetaHandler instead.')
+        warnings.warn('This method will be deprecated in future versions. \
+            Consider using MetaHandler instead.')
         return self._mh.read(path)
 
-    def _filter(self, name):
+    def _filter(self, name: str) -> bool:
         meta = self._mh.read(name)
         meta = meta[0]  # Takes first meta which is last model's meta
         for key in self._filt:
             if key not in meta:
                 raise KeyError(f"'{key}' key is not in\n{meta}")
 
             if self._filt[key] != meta[key]:
```

### Comparing `cascade-ml-0.8.0/cascade/meta/metric_viewer.py` & `cascade-ml-0.9.0/cascade/meta/metric_viewer.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,32 +11,33 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import os
-from typing import Union, List
+from typing import Union, List, Any, NoReturn
 
 import pendulum
 from flatten_json import flatten
 from plotly import graph_objects as go
 import pandas as pd
 
 from . import MetaViewer
+from ..models import Model, ModelRepo
 
 
 class MetricViewer:
     """
     Interface for viewing metrics in model meta files
     uses ModelRepo to extract metrics of all models if any.
     As metrics it uses data from `metrics` field in models'
     meta and as parameters it uses `params` field.
     """
-    def __init__(self, repo, scope: Union[int, str, slice] = None) -> None:
+    def __init__(self, repo: ModelRepo, scope: Union[int, str, slice, None] = None) -> None:
         """
         Parameters
         ----------
         repo: ModelRepo
             ModelRepo object to extract metrics from
         scope: Union[int, str, slice]
             Index or a name of line to view. Can be set using `__getitem__`
@@ -49,15 +50,15 @@
     def __getitem__(self, key: Union[int, str, slice]):
         """
         Sets the scope of the viewer after creation.
         Basically creates new viewer with another scope.
         """
         return MetricViewer(self._repo, scope=key)
 
-    def reload_table(self):
+    def reload_table(self) -> None:
         self._metrics = []
         selected_names = self._repo.get_line_names()
 
         if self._scope is not None:
             selected_names = selected_names[self._scope]
             if not isinstance(selected_names, list):
                 selected_names = [selected_names]
@@ -113,66 +114,80 @@
                            align='left')
             )
         ])
         if show:
             fig.show()
         return fig
 
-    def get_best_by(self, metric: str, maximize=True):
+    def get_best_by(self, metric: str, maximize: bool = True) -> Model:
         """
         Loads the best model by the given metric
 
         Parameters
         ----------
-            metric: str
-                Name of the metric
-            maximize: bool
-                The direction of choosing the best model: `True` if best is better
-                and `False` if less is better
+        metric: str
+            Name of the metric
+        maximize: bool
+            The direction of choosing the best model: `True` if greater is better
+            and `False` if less is better
+
+        Raises
+        ------
+        TypeError if metric objects cannot be sorted. If only one model in repo, then
+        returns it without error since no sorting involved.
         """
         assert metric in self.table, f'{metric} is not in {self.table.columns}'
         t = self.table.loc[self.table[metric].notna()]
 
-        best_row = t.sort_values(metric, ascending=maximize).iloc[-1]
+        try:
+            t = t.sort_values(metric, ascending=maximize)
+        except TypeError as e:
+            raise TypeError(f'Metric {metric} objects cannot be sorted') from e
+
+        best_row = t.iloc[-1]
         name = os.path.split(best_row['line'])[-1]
         num = best_row['num']
         return self._repo[name][num]
 
     def serve(
             self,
             page_size: int = 50,
-            include: List[str] = None,
-            exclude: List[str] = None,
-            **kwargs) -> None:
+            include: Union[List[str], None] = None,
+            exclude: Union[List[str], None] = None,
+            **kwargs: Any) -> None:
         """
         Runs dash-based server with interactive table of metrics and parameters
 
         Parameters
         ----------
         page_size: int, optional
             Size of the table in rows on one page
         include: List[str], optional:
-            List of parameters or metrics to be added. Only them will be present along with some default
+            List of parameters or metrics to be added.
+            Only they will be present along with some default
         exclude: List[str], optional:
             List of parameters or metrics to be excluded from table
         **kwargs:
             Arguments of dash app. Can be ip or port for example
         """
         server = MetricServer(self, page_size=page_size, include=include, exclude=exclude)
         server.serve(**kwargs)
 
 
 class MetricServer:
-    def __init__(self, mv, page_size, include, exclude, **kwargs) -> None:
+    def __init__(self, mv: MetricViewer,
+                 page_size: int,
+                 include: Union[List[str], None],
+                 exclude: Union[List[str], None], **kwargs: Any) -> None:
         self._mv = mv
         self._page_size = page_size
         self._include = include
         self._exclude = exclude
 
-    def _update_graph_callback(self, _app):
+    def _update_graph_callback(self, _app) -> None:
         try:
             from dash import Output, Input
         except ModuleNotFoundError:
             self._raise_cannot_import()
 
         @_app.callback(
             Output(component_id='dependence-figure', component_property='figure'),
@@ -242,24 +257,24 @@
                 selected_rows=[],
                 page_action="native",
                 page_current=0,
                 page_size=self._page_size,
             )
         ])
 
-    def serve(self, **kwargs):
+    def serve(self, **kwargs: Any) -> None:
         # Conditional import
         try:
             import dash
         except ModuleNotFoundError:
             self._raise_cannot_import()
 
         app = dash.Dash()
         app.layout = self._layout
         self._update_graph_callback(app)
         app.run_server(use_reloader=False, **kwargs)
 
-    def _raise_cannot_import(self):
+    def _raise_cannot_import(self) -> NoReturn:
         raise ModuleNotFoundError('''
                     Cannot import dash. It is conditional
                     dependency you can install it
                     using the instructions from https://dash.plotly.com/installation''')
```

### Comparing `cascade-ml-0.8.0/cascade/meta/validator.py` & `cascade-ml-0.9.0/cascade/meta/validator.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from typing import Callable, Union, List
+from typing import Callable, Union, List, NoReturn, Dict, Any
 from tqdm import tqdm
 
 from ..data import Dataset, Modifier, T
 
 
 class DataValidationException(Exception):
     """
@@ -30,17 +30,17 @@
         return f'{", ".join(map(str, items[:5]))} ... {", ".join(map(str, items[-5:]))}'
 
 
 class Validator(Modifier):
     """
     Base class for validators. Defines basic `__init__` structure
     """
-    def __init__(self, dataset: Dataset,
+    def __init__(self, dataset: Dataset[T],
                  func: Union[Callable[[T], bool], List[Callable[[T], bool]]],
-                 **kwargs) -> None:
+                 **kwargs: Any) -> None:
         super().__init__(dataset, **kwargs)
         if isinstance(func, Callable):
             self._func = [func]
         else:
             self._func = func
 
 
@@ -51,15 +51,15 @@
 
     Example
     -------
     >>> from cascade.data import Wrapper
     >>> ds = Wrapper([1, 2, 3, 4, 5])
     >>> ds = AggregateValidator(ds, lambda x: len(x) == 5)
     """
-    def __init__(self, dataset: Dataset, func: Callable[[Dataset], bool], **kwargs) -> None:
+    def __init__(self, dataset: Dataset[T], func: Callable[[Dataset[T]], bool], **kwargs) -> None:
         super().__init__(dataset, func, **kwargs)
 
         bad_results = []
         for i, func in enumerate(self._func):
             if not func(self._dataset):
                 bad_results.append(i)
 
@@ -80,30 +80,30 @@
     >>> ds = Wrapper([1, 2, 3, 4, 5])
     >>> ds = PredicateValidator(ds, lambda x: x < 6)
     """
     def __init__(
             self,
             dataset: Dataset,
             func: Union[Callable[[T], bool], List[Callable[[T], bool]]],
-            **kwargs) -> None:
+            **kwargs: Any) -> None:
         super().__init__(dataset, func, **kwargs)
 
         bad_items = {j: [] for j in range(len(self._func))}
         for i, item in tqdm(enumerate(self._dataset), desc='Checking', leave=False):
             for j, func in enumerate(self._func):
                 if not func(item):
                     bad_items[j].append(i)
 
         bad_counts = [len(bad_items[i]) for i in range(len(self._func))]
         if any(bad_counts):
             self._raise(bad_items)
         else:
             print('OK!')
 
-    def _raise(self, items: List[int]):
+    def _raise(self, items: Dict[int, List[int]]) -> NoReturn:
         bad_counts = [len(items[i]) for i in range(len(self._func))]
 
         failed_checks = [i for i in range(len(bad_counts)) if bad_counts[i]]
         failed_items = '\n'.join([f'{i}: {prettify_items(items[i])}' for i in items])
         raise DataValidationException(
             f'Checks in positions {failed_checks} failed\n'
             f'Items failed by check:\n'
```

### Comparing `cascade-ml-0.8.0/cascade/models/__init__.py` & `cascade-ml-0.9.0/cascade/models/__init__.py`

 * *Files identical despite different names*

### Comparing `cascade-ml-0.8.0/cascade/models/basic_model.py` & `cascade-ml-0.9.0/cascade/models/basic_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,39 +11,40 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 
-from typing import Dict, Callable
+from typing import Dict, Callable, Any
 from .model import Model, ModelModifier
 
 
 class BasicModel(Model):
     """
     Basic model is a more concrete version of an abstract Model class.
     It provides common interface for all ML solutions. For more flexible interface
     refer to Model class.
 
     See also
     --------
     cascade.models.Model
     """
 
-    def load(self, filepath) -> None:
+    def load(self, filepath: str) -> None:
         raise NotImplementedError()
 
-    def save(self, filepath) -> None:
+    def save(self, filepath: str) -> None:
         raise NotImplementedError()
 
-    def predict(self, x, *args, **kwargs):
+    def predict(self, x: Any, *args: Any, **kwargs: Any):
         raise NotImplementedError()
 
-    def evaluate(self, x, y, metrics_dict: Dict[str, Callable], *args, **kwargs) -> None:
+    def evaluate(self, x: Any, y: Any,
+                 metrics_dict: Dict[str, Callable], *args: Any, **kwargs: Any) -> None:
         """
         Receives x and y validation sequences. Passes x to the model's predict
         method along with any args or kwargs needed.
         Then updates self.metrics with what functions in `metrics_dict` return.
         `metrics_dict` should contain names of the metrics and the functions with the interface:
         f(true, predicted) -> metric_value, where metric_value is not always scalar, can be
         array or dict. For example confusion matrix.
@@ -57,15 +58,15 @@
             metrics_dict: Dict[str, Callable]
                 Dictionary with functions that given ground-truth and
                 predicted values return metrics.
         """
         preds = self.predict(x, *args, **kwargs)
         self.metrics.update({key: metrics_dict[key](y, preds) for key in metrics_dict})
 
-    def fit(self, x, y, *args, **kwargs) -> None:
+    def fit(self, x: Any, y: Any, *args: Any, **kwargs: Any) -> None:
         raise NotImplementedError()
 
 
 class BasicModelModifier(ModelModifier, BasicModel):
     """
     Interface to unify BasicModel and ModelModifier.
     """
```

### Comparing `cascade-ml-0.8.0/cascade/models/model.py` & `cascade-ml-0.9.0/cascade/models/model.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,74 +11,75 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import warnings
-from typing import List, Dict
+from typing import List, Dict, Any, Union
 import pendulum
 
-from ..base import Traceable
+from ..base import Traceable, Meta
 
 
 class Model(Traceable):
     """
     Base class for any model.
     Used to provide unified interface to any model, store metadata including metrics.
     """
-    def __init__(self, *args, meta_prefix=None, **kwargs) -> None:
+    def __init__(self, *args: Any,
+                 meta_prefix: Union[Meta, str, None] = None, **kwargs: Any) -> None:
         """
         Should be called in any successor - initializes default meta needed.
         Arguments passed in it should be related to model's hyperparameters, architecture.
         All additional arguments should have defaults - to be able to create model and then load.
         Successors may pass all of their parameters to superclass for it to be able to
-        log them in meta. Everything that is worth to document about model and data it was trained on can be
-        either in params or meta_prefix.
+        log them in meta. Everything that is worth to document about model and data 
+        it was trained on can be either in params or meta_prefix.
         """
         # Model accepts meta_prefix explicitly to not to record it in 'params'
         self.metrics = {}
         self.params = kwargs
         self.created_at = pendulum.now(tz='UTC')
-        super().__init__(meta_prefix=meta_prefix, **kwargs)
+        super().__init__(*args, meta_prefix=meta_prefix, **kwargs)
 
-    def fit(self, *args, **kwargs) -> None:
+    def fit(self, *args: Any, **kwargs: Any) -> None:
         """
         Method to encapsulate training loops.
         May be provided with any training-related arguments.
         """
         raise NotImplementedError()
 
-    def predict(self, *args, **kwargs):
+    def predict(self, *args: Any, **kwargs: Any) -> Any:
         """
         Method to encapsulate inference.
         May include preprocessing steps to make model self-sufficient.
         """
         raise NotImplementedError()
 
-    def evaluate(self, *args, **kwargs) -> None:
+    def evaluate(self, *args: Any, **kwargs: Any) -> None:
         """
         Evaluates model against any metrics. Should not return any value, just populate self.metrics dict.
         """
         raise NotImplementedError()
 
-    def load(self, filepath, *args, **kwargs) -> None:
+    def load(self, filepath: str, *args: Any, **kwargs: Any) -> None:
         """
         Loads model from provided filepath. May be unpickling process or reading json configs.
         Does not return any model, just restores internal state.
         """
         raise NotImplementedError()
 
-    def save(self, filepath, *args, **kwargs) -> None:
+    def save(self, filepath: str, *args: Any, **kwargs: Any) -> None:
         """
         Saves model's state using provided filepath.
         """
         raise NotImplementedError()
 
-    def get_meta(self) -> List[Dict]:
+    def get_meta(self) -> Meta:
         # Successors may not call super().__init__
         # they may not have these default fields
 
         meta = super().get_meta()
 
         all_default_exist = True
         if hasattr(self, 'created_at'):
@@ -93,31 +94,33 @@
 
         if hasattr(self, 'params'):
             meta[0]['params'] = self.params
         else:
             all_default_exist = False
 
         if not all_default_exist:
-            warnings.warn('Model\'s meta is incomplete, maybe you haven\'t call super().__init__ in subclass?')
+            warnings.warn(
+                'Model\'s meta is incomplete, '
+                'maybe you haven\'t call super().__init__ in subclass?')
 
         meta[0]['type'] = 'model'
         return meta
 
 
 class ModelModifier(Model):
     """
     Analog of dataset's Modifier. Can be used to chain
     two models in one.
     """
-    def __init__(self, model: Model, **kwargs):
+    def __init__(self, model: Model, *args: Any, **kwargs: Any) -> None:
         """
         Parameters
         ----------
         model: Model
             A model to modify.
         """
         self._model = model
-        super().__init__(**kwargs)
+        super().__init__(*args, **kwargs)
 
-    def get_meta(self) -> List[Dict]:
+    def get_meta(self) -> Meta:
         prev_meta = self._model.get_meta()
         return super().get_meta() + prev_meta
```

### Comparing `cascade-ml-0.8.0/cascade/models/model_line.py` & `cascade-ml-0.9.0/cascade/models/model_line.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,30 +12,31 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import os
 import warnings
-from typing import List, Dict
+from typing import Type, Literal, Any
 import pendulum
 import glob
 from hashlib import md5
 
-from ..base import Traceable, MetaHandler, supported_meta_formats
+from ..base import Traceable, MetaHandler, supported_meta_formats, Meta
 from .model import Model
 
 
 class ModelLine(Traceable):
     """
     A manager for a line of models. Used by ModelRepo for access to models on disk.
     A line of models is typically a models with the same hyperparameters and architecture,
     but different epochs or using different data.
     """
-    def __init__(self, folder: str, model_cls=Model, meta_fmt='.json', **kwargs) -> None:
+    def __init__(self, folder: str, model_cls: Type = Model,
+                 meta_fmt: Literal['.json', '.yml'] ='.json', **kwargs: Any) -> None:
         """
         All models in line should be instances of the same class.
 
         Parameters
         ----------
         folder: str
             Path to a folder where ModelLine will be created or already was created.
@@ -46,38 +47,38 @@
             Format in which to store meta data.
         See also
         --------
         cascade.models.ModelRepo
         """
         super().__init__(**kwargs)
 
-        assert meta_fmt in supported_meta_formats, f'Only {supported_meta_formats} are supported formats'
+        assert meta_fmt in supported_meta_formats, \
+            f'Only {supported_meta_formats} are supported formats'
         self._meta_fmt = meta_fmt
         self._model_cls = model_cls
         self.root = folder
         self.model_names = []
         if os.path.exists(self.root):
             assert os.path.isdir(self.root), f'folder should be directory, got `{folder}`'
             self.model_names = sorted(
                 [os.path.join(model_folder, 'model')
                     for model_folder in os.listdir(self.root)
                     if os.path.isdir(os.path.join(self.root, model_folder))])
 
             if len(self.model_names) == 0:
-                # TODO: add root to the message
-                warnings.warn('Model folders were not found by the line. It may be that '
-                              'you are using new version of cascade with old repos '
-                              'created before version 0.2.0')
+                warnings.warn(
+                    f'Model folders were not found by the line in {self.root}'
+                )
 
         else:
             # No folder -> create
             os.mkdir(self.root)
         self._mh = MetaHandler()
 
-    def __getitem__(self, num) -> Model:
+    def __getitem__(self, num: int) -> Model:
         """
         Creates a model of `model_cls` and loads it using Model's `load` method.
 
         Returns
         -------
             model: Model
                 a loaded model
@@ -90,15 +91,15 @@
         """
         Returns
         -------
         A number of models in line
         """
         return len(self.model_names)
 
-    def save(self, model: Model, only_meta=False) -> None:
+    def save(self, model: Model, only_meta: bool = False) -> None:
         """
         Saves a model and its metadata to a line's folder.
         Model is automatically assigned a number and a model is saved
         using Model's method `save` in its own folder.
         Folder's name is assigned using f'{idx:0>5d}'. For example: 00001 or 00042.
         The name passed to model's save is just "model" without extension.
         It is Model's responsibility to correctly  assign extension and save its own state.
@@ -148,15 +149,15 @@
 
         # Save updated line's meta
         self._mh.write(os.path.join(self.root, 'meta' + self._meta_fmt), self.get_meta())
 
     def __repr__(self) -> str:
         return f'ModelLine of {len(self)} models of {self._model_cls}'
 
-    def get_meta(self) -> List[Dict]:
+    def get_meta(self) -> Meta:
         meta = super().get_meta()
         meta[0].update({
             'root': self.root,
             'model_cls': repr(self._model_cls),
             'len': len(self),
             'updated_at': pendulum.now(tz='UTC'),
             'type': 'line'
```

### Comparing `cascade-ml-0.8.0/cascade/models/model_repo.py` & `cascade-ml-0.9.0/cascade/models/model_repo.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,72 +11,78 @@
 limitations under the License.
 """
 
 import os
 import warnings
 import itertools
 import logging
-from typing import List, Dict, Iterable, Union
+from typing import List, Iterable, Union, Any, Literal, Type, Generator
 import shutil
 
 import pendulum
 from deepdiff.diff import DeepDiff
 
-from ..base import Traceable, MetaHandler, JSONEncoder, supported_meta_formats
+from ..base import Traceable, MetaHandler, JSONEncoder, supported_meta_formats, Meta
 from .model import Model
 from .model_line import ModelLine
 
 
 class Repo(Traceable):
     """
     Base interface for repos of models.
 
     See also
     --------
     cascade.models.ModelRepo
     """
     root = None
 
-    def reload(self):
+    def reload(self) -> None:
         raise NotImplementedError()
 
-    def __getitem__(self, key):
+    def __getitem__(self, key: str) -> ModelLine:
         raise NotImplementedError()
 
-    def __len__(self):
+    def __len__(self) -> int:
         raise NotImplementedError()
 
 
 class ModelRepo(Repo):
     """
     An interface to manage experiments with several lines of models.
     When created, initializes an empty folder constituting a repository of model lines.
 
     Stores its meta-data in its root folder. With every run if the repo was already
     created earlier, updates its meta and logs changes in human-readable format in file history.log
 
     Example
     -------
     >>> from cascade.models import ModelRepo
-    >>> from cascade.utils import ConstantBaseline
-    >>> repo = ModelRepo('repo', _meta_prefix={'description': 'This is a repo with one VGG16 line for the example.'})
-    >>> line = repo.add_line('model', ConstantBaseline)
-    >>> model = ConstantBaseline(1)
+    >>> from cascade import utils as cdu
+    >>> repo = ModelRepo('repo', meta_prefix={'description': 'This is a repo with one line for the example.'})
+    >>> line = repo.add_line('model', cdu.ConstantBaseline)
+    >>> model = cdu.ConstantBaseline(1)
     >>> model.fit()
     >>> line.save(model)
 
 
     >>> from cascade.models import ModelRepo
-    >>> from cascade.utils import ConstantBaseline
-    >>> repo = ModelRepo('repo', lines=[dict(name='constant', model_cls=ConstantBaseline)])
-    >>> model = ConstantBaseline()
+    >>> from cascade import utils as cdu
+    >>> repo = ModelRepo('repo', lines=[dict(name='constant', model_cls=cdu.ConstantBaseline)])
+    >>> model = cdu.ConstantBaseline()
     >>> model.fit()
     >>> repo['constant'].save(model)
     """
-    def __init__(self, folder, lines=None, overwrite=False, meta_fmt='.json', model_cls=Model, **kwargs):
+    def __init__(
+        self,
+        folder: str,
+        lines: Union[Iterable[ModelLine], None] = None,
+        overwrite: bool = False,
+        meta_fmt: Literal['.json', '.yml'] = '.json',
+        model_cls: Type = Model, **kwargs: Any) -> None:
         """
         Parameters
         ----------
         folder:
             Path to a folder where ModelRepo needs to be created or already was created
             if folder does not exist, creates it
         lines: List[Dict]
@@ -94,15 +100,16 @@
         cascade.models.ModelLine
         """
         super().__init__(**kwargs)
         self._model_cls = model_cls
         self._root = folder
         self._lines = dict()
 
-        assert meta_fmt in supported_meta_formats, f'Only {supported_meta_formats} are supported formats'
+        assert meta_fmt in supported_meta_formats, \
+            f'Only {supported_meta_formats} are supported formats'
         self._meta_fmt = meta_fmt
         if overwrite and os.path.exists(self._root):
             shutil.rmtree(self._root)
 
         os.makedirs(self._root, exist_ok=True)
 
         self._mh = MetaHandler()
@@ -111,24 +118,24 @@
 
         if lines is not None:
             for line in lines:
                 self.add_line(**line)
 
         self._update_meta()
 
-    def _load_lines(self):
+    def _load_lines(self) -> None:
         self._lines = {
             name: ModelLine(os.path.join(self._root, name),
                             model_cls=self._model_cls,
                             meta_prefix=self._meta_prefix,
                             meta_fmt=self._meta_fmt)
             for name in sorted(os.listdir(self._root))
             if os.path.isdir(os.path.join(self._root, name))}
 
-    def add_line(self, name: str = None, *args, meta_fmt=None, **kwargs):
+    def add_line(self, name: str = None, *args, meta_fmt=None, **kwargs) -> ModelLine:
         """
         Adds new line to repo if it doesn't exist and returns it.
         If line exists, defines it in repo with parameters provided.
 
         Supports all the parameters of ModelLine using args and kwargs.
 
         Parameters:
@@ -178,15 +185,15 @@
         if isinstance(key, str):
             return self._lines[key]
         elif isinstance(key, int):
             return self._lines[list(self._lines.keys())[key]]
         else:
             raise TypeError(f'{type(key)} is not supported as key')
 
-    def __iter__(self):
+    def __iter__(self) -> Generator[ModelLine, None, None]:
         for line in self._lines:
             yield self.__getitem__(line)
 
     def __len__(self) -> int:
         """
         Returns
         -------
@@ -194,22 +201,22 @@
             a number of lines
         """
         return len(self._lines)
 
     def __repr__(self) -> str:
         return f'ModelRepo in {self._root} of {len(self)} lines'
 
-    def _setup_logger(self):
+    def _setup_logger(self) -> None:
         self.logger = logging.getLogger(self._root)
         hdlr = logging.FileHandler(os.path.join(self._root, 'history.log'))
         hdlr.setFormatter(logging.Formatter('\n%(asctime)s\n%(message)s'))
         self.logger.addHandler(hdlr)
         self.logger.setLevel('DEBUG')
 
-    def _update_meta(self):
+    def _update_meta(self) -> None:
         # Reads meta if exists and updates it with new values
         # writes back to disk
         meta_path = os.path.join(self._root, 'meta' + self._meta_fmt)
 
         meta = {}
         if os.path.exists(meta_path):
             try:
@@ -223,15 +230,15 @@
 
         meta.update(self.get_meta()[0])
         try:
             self._mh.write(meta_path, [meta])
         except IOError as e:
             warnings.warn(f'File writing error ignored: {e}')
 
-    def get_meta(self) -> List[Dict]:
+    def get_meta(self) -> Meta:
         meta = super().get_meta()
         meta[0].update({
             'root': self._root,
             'len': len(self),
             'updated_at': pendulum.now(tz='UTC'),
             'type': 'repo'
         })
@@ -240,63 +247,62 @@
     def reload(self) -> None:
         """
         Updates internal state.
         """
         self._load_lines()
         self._update_meta()
 
-    def __del__(self):
+    def __del__(self) -> None:
         # Release all files on destruction
         if hasattr(self, 'logger'):
             for handler in self.logger.handlers:
                 handler.close()
                 self.logger.removeHandler(handler)
 
     def __add__(self, repo):
         return ModelRepoConcatenator([self, repo])
 
     def get_line_names(self) -> List[str]:
         """
         Returns list of line names.
         """
-        # TODO: write test covering this
         return list(self._lines.keys())
 
 
 class ModelRepoConcatenator(Repo):
     """
     The class to concatenate different Repos.
     For the ease of use please, don't use it directly.
     Just do `repo = repo_1 + repo_2` to unify two or more repos.
     """
-    def __init__(self, repos: Iterable[Repo], *args, **kwargs) -> None:
+    def __init__(self, repos: Iterable[Repo], *args: Any, **kwargs: Any) -> None:
         super().__init__(*args, **kwargs)
         self._repos = repos
 
-    def __getitem__(self, key):
+    def __getitem__(self, key) -> ModelLine:
         pair = key.split('_')
         if len(pair) <= 2:
             raise KeyError(f'Key {key} is not in required format \
             `<repo_idx>_..._<line_name>`. \
             Please, use the key in this format. For example `0_line_1`')
         idx, line_name = pair[0], '_'.join(pair[1:])
         idx = int(idx)
 
         return self._repos[idx][line_name]
 
-    def __len__(self):
+    def __len__(self) -> int:
         return sum([len(repo) for repo in self._repos])
 
-    def __iter__(self):
+    def __iter__(self) -> Generator[ModelLine, None, None]:
         # this flattens the list of lines
         for line in itertools.chain(*[[line for line in repo] for repo in self._repos]):
             yield line
 
-    def __add__(self, repo):
+    def __add__(self, repo: ModelRepo):
         return ModelRepoConcatenator([self, repo])
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f'ModelRepoConcatenator of {len(self._repos)} repos, {len(self)} lines total'
 
-    def reload(self):
+    def reload(self) -> None:
         for repo in self._repos:
             repo.reload()
```

### Comparing `cascade-ml-0.8.0/cascade/models/trainer.py` & `cascade-ml-0.9.0/cascade/models/trainer.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,40 @@
+"""
+Copyright 2022 Ilia Moiseev
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+   http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+"""
+
 import os
 import logging
-from typing import Iterable, List, Dict, Union
+from typing import Iterable, List, Dict, Union, Any
 
 import pendulum
 from ..base import Traceable
-from ..models import Model, ModelRepo
+from ..models import Model, ModelLine, ModelRepo
 
 
 logger = logging.getLogger(__name__)
 
 
 class Trainer(Traceable):
     """
     A class that encapsulates training, evaluation and saving of models.
     """
-    def __init__(self, repo: Union[ModelRepo, str], *args, **kwargs) -> None:
+    def __init__(self, repo: Union[ModelRepo, str], *args: Any, **kwargs: Any) -> None:
         """
         Parameters
         ----------
         repo: Union[ModelRepo, str]
             Either repo or path to it
         """
         if isinstance(repo, str):
@@ -27,15 +43,15 @@
             self._repo = repo
         else:
             raise TypeError(f'Repo should be either ModelRepo or path, got {type(repo)}')
 
         self.metrics = []
         super().__init__(*args, **kwargs)
 
-    def train(self, model, *args, **kwargs):
+    def train(self, model: Model, *args: Any, **kwargs: Any) -> None:
         raise NotImplementedError()
 
     def get_meta(self) -> List[Dict]:
         meta = super().get_meta()
         meta[0]['metrics'] = self.metrics
         meta[0]['repo'] = self._repo.get_meta()
         return meta
@@ -44,15 +60,15 @@
 class BasicTrainer(Trainer):
     """
     The most common of concrete Trainers.
     Trains a model for a certain amount of epochs.
     Can start from checkpoint if model file exists.
     """
     @staticmethod
-    def _find_last_model(model, line):
+    def _find_last_model(model: Model, line: ModelLine) -> None:
         model_num = len(line) - 1
         while True:
             path = os.path.join(line.root, line.model_names[model_num])
             try:
                 model.load(path)
                 break
             except FileNotFoundError as e:
@@ -60,24 +76,24 @@
                 model_num -= 1
 
                 if model_num == -1:
                     raise FileNotFoundError(f'No model files were found in line {line}')
 
     def train(self,
               model: Model,
-              *args,
-              train_data: Iterable = None,
-              test_data: Iterable = None,
-              train_kwargs: Dict = None,
-              test_kwargs: Dict = None,
+              *args: Any,
+              train_data: Union[Iterable[Any], None] = None,
+              test_data: Union[Iterable[Any], None] = None,
+              train_kwargs: Union[Dict[Any, Any], None] = None,
+              test_kwargs: Union[Dict[Any, Any], None] = None,
               epochs: int = 1,
-              start_from: str = None,
-              eval_strategy: int = None,
-              save_strategy: int = None,
-              **kwargs) -> None:
+              start_from: Union[str, None] = None,
+              eval_strategy: Union[int, None] = None,
+              save_strategy: Union[int, None] = None,
+              **kwargs: Any) -> None:
         """
         Trains, evaluates and saves given model. If specified, loads model from checkpoint.
 
         Parameters:
             model: Model
                 a model to be trained or which to load from line specified in `start_from`
             train_data: Iterable
@@ -96,21 +112,22 @@
             eval_strategy: int, optional
                 Evaluation will take place every `eval_strategy` epochs. If None - the strategy is 'no evaluation'.
             save_strategy: int, optional
                 Saving will take place every `save_strategy` epochs. Meta will be saved anyway.
                 If None - the strategy is 'save only meta'.
         """
 
-        # TODO: check if eval_strategy specified that test_data provided also
-
         if train_kwargs is None:
             train_kwargs = {}
         if test_kwargs is None:
             test_kwargs = {}
 
+        if eval_strategy is not None and test_data is None:
+            raise ValueError('Eval strategy is specified, but no test data provided')
+
         if start_from is not None:
             line_name = start_from
         else:
             line_name = f'{len(self._repo):0>5d}'
             if line_name in self._repo.get_line_names():
                 # Name can appear in the repo if the user manually
                 # removed the lines from the middle of the repo
```

### Comparing `cascade-ml-0.8.0/cascade/tests/conftest.py` & `cascade-ml-0.9.0/cascade/tests/conftest.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,20 +18,24 @@
 import os
 import sys
 import datetime
 import pendulum
 from dateutil import tz
 import numpy as np
 import pytest
+import pandas as pd
 
 MODULE_PATH = os.path.dirname(os.path.abspath(os.path.dirname(__file__)))
 sys.path.append(os.path.dirname(MODULE_PATH))
 
-from cascade.data import Wrapper, Iterator
+from cascade.data import Dataset, Wrapper, Iterator, ApplyModifier, \
+    BruteforceCacher, Composer, Concatenator, CyclicSampler, \
+    RandomSampler, RangeSampler, SequentialCacher
 from cascade.models import Model, ModelLine, ModelRepo, BasicModel
+from cascade import utils as cdu
 
 
 class DummyModel(Model):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.model = b'model'
 
@@ -72,14 +76,47 @@
     def save(self, filepath) -> None:
         pass
 
     def fit(self, x, y, *args, **kwargs) -> None:
         pass
 
 
+def f(x: int) -> int:
+    return 2 * x
+
+
+@pytest.fixture(
+    params=[
+        Iterator([0]),
+        Wrapper([0]),
+        ApplyModifier(Wrapper([0, 1, 2]), f),
+        BruteforceCacher(Wrapper([0, 2])),
+        Composer([Wrapper([0]), Wrapper([1])]),
+        Concatenator([Wrapper([0]), Wrapper([1])]),
+        CyclicSampler(Wrapper([0]), 1),
+        RandomSampler(Wrapper([1, 2, 3]), 2),
+        RangeSampler(Wrapper([0, 1, 2, 3]), 0, 3, 1),
+        SequentialCacher(Wrapper([0, 1, 2, 3]))
+    ]
+)
+def dataset(request) -> Dataset:
+    return request.param
+
+
+@pytest.fixture(
+    params=[
+        cdu.TableDataset(t=pd.DataFrame()),
+        cdu.TableFilter(cdu.TableDataset(t=pd.DataFrame()), []),
+        cdu.TimeSeriesDataset(time=[datetime.datetime(2022, 12, 2)], data=[24])
+    ]
+)
+def utils_dataset(request) -> Dataset:
+    return request.param
+
+
 @pytest.fixture(params=[
     [1, 2, 3, 4, 5],
     [0],
     [0, 0, 0, 0],
     [-i for i in range(0, 100)]
 ])
 def number_dataset(request):
```

### Comparing `cascade-ml-0.8.0/cascade/tests/test_apply_modifier.py` & `cascade-ml-0.9.0/cascade/tests/test_apply_modifier.py`

 * *Files identical despite different names*

### Comparing `cascade-ml-0.8.0/cascade/tests/test_basic_model.py` & `cascade-ml-0.9.0/cascade/tests/test_basic_model.py`

 * *Files identical despite different names*

### Comparing `cascade-ml-0.8.0/cascade/tests/test_bruteforce_cacher.py` & `cascade-ml-0.9.0/cascade/tests/test_bruteforce_cacher.py`

 * *Files identical despite different names*

### Comparing `cascade-ml-0.8.0/cascade/tests/test_composer.py` & `cascade-ml-0.9.0/cascade/tests/test_composer.py`

 * *Files identical despite different names*

### Comparing `cascade-ml-0.8.0/cascade/tests/test_cyclic_sampler.py` & `cascade-ml-0.9.0/cascade/tests/test_cyclic_sampler.py`

 * *Files identical despite different names*

### Comparing `cascade-ml-0.8.0/cascade/tests/test_data_split.py` & `cascade-ml-0.9.0/cascade/tests/test_data_split.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import os
 import sys
+import pytest
 
 MODULE_PATH = os.path.dirname(os.path.abspath(os.path.dirname(__file__)))
 sys.path.append(os.path.dirname(MODULE_PATH))
 
 import cascade.data as cdd
 
 
@@ -39,7 +40,24 @@
     ds1, ds2 = cdd.split(ds, num=4)
 
     assert [item for item in ds1] == [0, 1, 2, 3]
     assert [item for item in ds2] == [4]
 
     # This means pipeline was made
     assert len(ds1.get_meta()) == 2
+
+
+def test_wrong_usage():
+    ds = cdd.Wrapper([0, 1, 2, 3])
+
+    with pytest.raises(ValueError):
+        a, b = cdd.split(ds, None)
+
+
+def test_empty():
+    ds = cdd.Wrapper([])
+
+    with pytest.raises(ValueError):
+        a, b = cdd.split(ds, num=10)
+
+    with pytest.raises(ValueError):
+        a, b = cdd.split(ds)
```

### Comparing `cascade-ml-0.8.0/cascade/tests/test_dataleak_validator.py` & `cascade-ml-0.9.0/cascade/tests/test_dataleak_validator.py`

 * *Files identical despite different names*

### Comparing `cascade-ml-0.8.0/cascade/tests/test_dataset.py` & `cascade-ml-0.9.0/cascade/tests/test_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
+
 import datetime
 import os
 import json
 import sys
 import pytest
 
 MODULE_PATH = os.path.dirname(os.path.abspath(os.path.dirname(__file__)))
```

### Comparing `cascade-ml-0.8.0/cascade/tests/test_folder_dataset.py` & `cascade-ml-0.9.0/cascade/tests/test_folder_dataset.py`

 * *Files identical despite different names*

### Comparing `cascade-ml-0.8.0/cascade/tests/test_history_viewer.py` & `cascade-ml-0.9.0/cascade/tests/test_history_viewer.py`

 * *Files identical despite different names*

### Comparing `cascade-ml-0.8.0/cascade/tests/test_meta_handler.py` & `cascade-ml-0.9.0/cascade/tests/test_meta_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -124,7 +124,28 @@
     with open(filename, 'w') as f:
         f.write('\t{\t :this file is broken')
 
     # Test that file path is in error message
     with pytest.raises(IOError) as e:
         mh.read(filename)
     assert filename in e.value.args[0]
+
+
+@pytest.mark.parametrize(
+    'ext', [
+        '.json',
+        '.yml'
+    ]
+)
+def test_empty_file(tmp_path, ext):
+    tmp_path = str(tmp_path)
+    mh = MetaHandler()
+
+    # Simulate empty file
+    filename = os.path.join(tmp_path, 'meta' + ext)
+    with open(filename, 'w') as f:
+        f.write('')
+
+    # Test that file path is in error message
+    with pytest.raises(IOError) as e:
+        mh.read(filename)
+    assert filename in e.value.args[0]
```

### Comparing `cascade-ml-0.8.0/cascade/tests/test_meta_validator.py` & `cascade-ml-0.9.0/cascade/tests/test_meta_validator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
 Copyright 2022 Ilia Moiseev
+
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
    http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
```

### Comparing `cascade-ml-0.8.0/cascade/tests/test_meta_viewer.py` & `cascade-ml-0.9.0/cascade/tests/test_meta_viewer.py`

 * *Files identical despite different names*

### Comparing `cascade-ml-0.8.0/cascade/tests/test_metric_viewer.py` & `cascade-ml-0.9.0/cascade/tests/test_metric_viewer.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,20 +13,21 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import os
 import sys
 import pytest
+import numpy as np
 
 MODULE_PATH = os.path.dirname(os.path.abspath(os.path.dirname(__file__)))
 sys.path.append(os.path.dirname(MODULE_PATH))
 
 from cascade.tests.conftest import DummyModel
-from cascade.models import ModelRepo
+from cascade.models import ModelRepo, BasicModel
 from cascade.meta import MetricViewer
 
 
 def test(model_repo, dummy_model):
     m = dummy_model
     m.evaluate()
     model_repo['0'].save(m)
@@ -90,7 +91,38 @@
     line.save(model)
 
     model = DummyModel()
     line.save(model)
 
     mv = MetricViewer(repo)
     mv.get_best_by('acc')
+
+
+@pytest.mark.parametrize(
+    'ext', [
+        '.json',
+        '.yml'
+    ]
+)
+def test_get_best_by_non_sortable(tmp_path, ext):
+    class ModelComplexMetric(BasicModel):
+        def load(self, *args, **kwargs):
+            pass
+
+        def predict(self, *args, **kwargs):
+            return None
+
+    repo = ModelRepo(str(tmp_path),
+                     meta_fmt=ext,
+                     model_cls=ModelComplexMetric)
+    line = repo.add_line('00001', model_cls=ModelComplexMetric)
+
+    for _ in range(10):
+        model = ModelComplexMetric()
+        model.evaluate(None, None, {
+            'dict_metric':
+                lambda x, y: {np.random.choice(['a', 'b', 'c']): np.random.random()}})
+        line.save(model, only_meta=True)
+
+    mv = MetricViewer(repo)
+    with pytest.raises(TypeError):
+        mv.get_best_by('dict_metric')
```

### Comparing `cascade-ml-0.8.0/cascade/tests/test_model_line.py` & `cascade-ml-0.9.0/cascade/tests/test_model_line.py`

 * *Files identical despite different names*

### Comparing `cascade-ml-0.8.0/cascade/tests/test_model_repo.py` & `cascade-ml-0.9.0/cascade/tests/test_model_repo.py`

 * *Files identical despite different names*

### Comparing `cascade-ml-0.8.0/cascade/tests/test_modifier.py` & `cascade-ml-0.9.0/cascade/tests/test_modifier.py`

 * *Files identical despite different names*

### Comparing `cascade-ml-0.8.0/cascade/tests/test_pickler.py` & `cascade-ml-0.9.0/cascade/tests/test_pickler.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,39 +9,50 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import os
 import sys
+import datetime
 import pytest
+import pandas as pd
 
 MODULE_PATH = os.path.dirname(os.path.abspath(os.path.dirname(__file__)))
 sys.path.append(os.path.dirname(MODULE_PATH))
 
-from cascade.data import Pickler, Wrapper, Modifier, Sampler
+from cascade.data import *
+from cascade import utils as cdu
+
+
+def test_data_coverage(dataset, tmp_path):
+    Pickler(os.path.join(tmp_path, 'ds.pkl'), dataset)
+
+
+def test_utils_coverage(utils_dataset, tmp_path):
+    Pickler(os.path.join(tmp_path, 'ds.pkl'), utils_dataset)
 
 
 @pytest.mark.parametrize(
     'ds',
     [
         Wrapper([1, 2, 3, 4, 5]),
         Wrapper([1]),
         Sampler(Modifier(Wrapper([1])), 1)
     ]
 )
-def test(ds, tmp_path):
-    ds1 = Pickler(os.path.join(tmp_path, 'ds.pkl'), ds)
-    ds2 = Pickler(os.path.join(tmp_path, 'ds.pkl'))
+def test_integrity(ds, tmp_path):
+    _ = Pickler(os.path.join(tmp_path, 'ds.pkl'), ds)
+    loaded_ds = Pickler(os.path.join(tmp_path, 'ds.pkl'))
 
     true = []
     for i in range(len(ds)):
         true.append(ds[i])
 
     res = []
-    for i in range(len(ds2)):
-        res.append(ds2[i])
+    for i in range(len(loaded_ds)):
+        res.append(loaded_ds[i])
 
     assert res == true
 
-    assert type(ds2.ds()) == type(ds)
-    assert str(ds2.ds()) == str(ds)
+    assert type(loaded_ds.ds()) == type(ds)
+    assert str(loaded_ds.ds()) == str(ds)
```

### Comparing `cascade-ml-0.8.0/cascade/tests/test_random_sampler.py` & `cascade-ml-0.9.0/cascade/tests/test_random_sampler.py`

 * *Files identical despite different names*

### Comparing `cascade-ml-0.8.0/cascade/tests/test_range_sampler.py` & `cascade-ml-0.9.0/cascade/tests/test_range_sampler.py`

 * *Files 17% similar despite different names*

```diff
@@ -19,34 +19,45 @@
 import pytest
 
 MODULE_PATH = os.path.dirname(os.path.abspath(os.path.dirname(__file__)))
 sys.path.append(os.path.dirname(MODULE_PATH))
 
 from cascade.data import RangeSampler, Wrapper
 
+DATA = [0, 1, 2, 3, 4]
+
 
 def test():
-    data = [0, 1, 2, 3, 4]
-    ds = Wrapper(data)
+    ds = Wrapper(DATA)
     ds = RangeSampler(ds, 2)
 
     sampled = [item for item in ds]
 
-    assert sampled == [data[i] for i in range(2)]
+    assert sampled == [DATA[i] for i in range(2)]
+
 
-    ds = Wrapper(data)
+def test_start_stop():
+    ds = Wrapper(DATA)
     ds = RangeSampler(ds, 1, 3)
 
     sampled = [item for item in ds]
 
-    assert sampled == [data[i] for i in range(1, 3)]
+    assert sampled == [DATA[i] for i in range(1, 3)]
+
 
-    ds = Wrapper(data)
+def test_step():
+    ds = Wrapper(DATA)
     ds = RangeSampler(ds, 0, len(ds), 2)
 
     sampled = [item for item in ds]
 
-    assert sampled == [data[i] for i in range(0, len(data), 2)]
+    assert sampled == [DATA[i] for i in range(0, len(DATA), 2)]
+
+
+def test_wrong_usage():
+    with pytest.raises(ValueError):
+        ds = Wrapper(DATA)
+        ds = RangeSampler(ds, 10, 0)  # start > stop
 
-    with pytest.raises(AssertionError):
-        ds = Wrapper(data)
-        ds = RangeSampler(data, 10, 0)  # start > stop -> num_samples == 0
+    with pytest.raises(ValueError):
+        ds = Wrapper(DATA)
+        ds = RangeSampler(ds)
```

### Comparing `cascade-ml-0.8.0/cascade/tests/test_sequential_cacher.py` & `cascade-ml-0.9.0/cascade/utils/numpy_wrapper.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 """
 Copyright 2022 Ilia Moiseev
+
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
+
    http://www.apache.org/licenses/LICENSE-2.0
+
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-import os
-import sys
-
-MODULE_PATH = os.path.dirname(os.path.abspath(os.path.dirname(__file__)))
-sys.path.append(os.path.dirname(MODULE_PATH))
+from typing import Dict, List, Any
+import numpy as np
+from ..data import Wrapper
+from ..base import Meta
 
-from cascade.data import SequentialCacher
 
+class NumpyWrapper(Wrapper):
+    """
+    A wrapper around .npy files. Loads file in `__init__`.
+    """
+    def __init__(self, path: str, *args: Any, **kwargs: Any) -> None:
+        self._path = path
+        super().__init__(np.load(path), *args, **kwargs)
 
-def test(number_dataset):
-    ds = SequentialCacher(number_dataset, 2)
-    res = []
-    for i in range(len(ds)):
-        res.append(ds[i])
-    assert res == number_dataset._data
+    def get_meta(self) -> Meta:
+        meta = super().get_meta()
+        meta[0]['root'] = self._path
+        return meta
```

### Comparing `cascade-ml-0.8.0/cascade/tests/test_traceable.py` & `cascade-ml-0.9.0/cascade/tests/test_traceable.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
+
 import datetime
 import os
 import json
 import sys
 
 MODULE_PATH = os.path.dirname(os.path.abspath(os.path.dirname(__file__)))
 sys.path.append(os.path.dirname(MODULE_PATH))
```

### Comparing `cascade-ml-0.8.0/cascade/tests/test_trainer.py` & `cascade-ml-0.9.0/cascade/tests/test_trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
+
 import os
 import sys
 
 from cascade.models.trainer import BasicTrainer
 
 MODULE_PATH = os.path.dirname(os.path.abspath(os.path.dirname(__file__)))
 sys.path.append(os.path.dirname(MODULE_PATH))
```

### Comparing `cascade-ml-0.8.0/cascade/tests/test_validator.py` & `cascade-ml-0.9.0/cascade/tests/test_validator.py`

 * *Files identical despite different names*

### Comparing `cascade-ml-0.8.0/cascade/tests/test_version_assigner.py` & `cascade-ml-0.9.0/cascade/tests/test_version_assigner.py`

 * *Files 23% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import os
 import sys
 import pytest
 
 MODULE_PATH = os.path.dirname(os.path.abspath(os.path.dirname(__file__)))
 sys.path.append(os.path.dirname(MODULE_PATH))
 
-from cascade.data import Wrapper, ApplyModifier, VersionAssigner
+from cascade.data import Wrapper, ApplyModifier, VersionAssigner, Concatenator
 
 
 @pytest.mark.parametrize(
     'ext', [
         '.json',
         '.yml'
     ]
@@ -46,7 +46,34 @@
     assert ds.version == '1.0'
 
     ds = Wrapper([0, 1, 2, 3, 4, 5])
     ds = ApplyModifier(ds, lambda x: x ** 2)
     ds = VersionAssigner(ds, filepath)
 
     assert ds.version == '1.1'
+
+
+@pytest.mark.parametrize(
+    'ext', [
+        '.json',
+        '.yml'
+    ]
+)
+def test_deep_changes(tmp_path, ext):
+    filepath = os.path.join(tmp_path, 'ds' + ext)
+
+    ds = Wrapper([0, 1, 2, 3, 4])
+    ds = ApplyModifier(ds, lambda x: x * 2)
+    ds = Concatenator([ds, ds])
+    ds = Concatenator([ds, ds])
+    ds = VersionAssigner(ds, filepath)
+
+    assert ds.version == '0.0'
+
+    ds = Wrapper([0, 1, 2, 3, 4])
+    ds = ApplyModifier(ds, lambda x: x * 2)
+    ds = ApplyModifier(ds, lambda x: x * 2)
+    ds = Concatenator([ds, ds])
+    ds = Concatenator([ds, ds])
+    ds = VersionAssigner(ds, filepath)
+
+    assert ds.version == '1.0'
```

### Comparing `cascade-ml-0.8.0/cascade/utils/__init__.py` & `cascade-ml-0.9.0/cascade/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cascade-ml-0.8.0/cascade/utils/baselines.py` & `cascade-ml-0.9.0/cascade/utils/torch_model.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,41 +9,54 @@
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-import json
-import numpy as np
-from ..models import BasicModel
 
+from typing import Type, Any
+import torch
+from ..models import Model
+from ..base import Meta
 
-class ConstantBaseline(BasicModel):
+
+class TorchModel(Model):
     """
-    Constant function. This baseline can be used for
-    any classification task. It returns only one class
-    (for example it can be majority class)
+    The wrapper around `nn.Module`s.
     """
-    def __init__(self, constant=None, **kwargs) -> None:
-        super().__init__(**kwargs)
-        self._constant = constant
+    def __init__(self, model_class: Type, *args: Any, **kwargs: Any) -> None:
+        """
+        Parameters
+        ----------
+        model_class: type
+            The class created when new nn.Module was defined. Will be used
+            to construct model. If any arguments needed, please pass them
+            into `args` and `kwargs`.
+        """
+        self._model = model_class(*args, **kwargs)
+        super().__init__(*args, **kwargs)
 
-    def fit(self, x, y, *args, **kwargs) -> None:
-        pass
+    def predict(self, *args, **kwargs) -> Any:
+        """
+        Calls internal module with whatever arguments.
+        """
+        return self._model(*args, **kwargs)
 
-    def predict(self, x, *args, **kwargs) -> np.ndarray:
+    def save(self, path: str, *args: Any, **kwargs: Any) -> None:
         """
-        Returns the array of the same shape as input full of
-        given constant.
+        Saves the model using `torch.save`. Args and kwargs are passed into torch.save
         """
-        # TODO: make more universal when work with input shape
-        return np.full_like(x, self._constant)
+        with open(path, 'wb') as f:
+            torch.save(self._model, f, *args, **kwargs)
 
-    def save(self, path) -> None:
-        with open(path, 'w') as f:
-            json.dump({'constant': self._constant}, f)
+    def load(self, path: str, *args: Any, **kwargs: Any) -> None:
+        """
+        Loads the model using `torch.load`.
+        """
+        with open(path, 'rb') as f:
+            self._model = torch.load(f)
 
-    def load(self, path) -> None:
-        with open(path, 'r') as f:
-            obj = json.load(f)
-            self._constant = obj['constant']
+    def get_meta(self) -> Meta:
+        meta = super().get_meta()
+        meta[0]['module'] = repr(self._model)
+        return meta
```

### Comparing `cascade-ml-0.8.0/cascade/utils/folder_image_dataset.py` & `cascade-ml-0.9.0/cascade/utils/folder_image_dataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,14 +21,14 @@
 class FolderImageDataset(FolderDataset):
     """
     Simple dataset for image folder with lazy loading.
     Accepts the path to the folder with images. In each __getitem__ call
     invokes opencv imread on image and returns it if it exists.
     """
 
-    def __getitem__(self, index):
+    def __getitem__(self, index: int) -> cv2.Mat:
         name = self._names[index]
         img = cv2.imread(f'{name}')
         if img is not None:
             return cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
         else:
             raise RuntimeError(f'cv2 cannot read {name}')
```

### Comparing `cascade-ml-0.8.0/cascade/utils/model_aggregate.py` & `cascade-ml-0.9.0/cascade/utils/model_aggregate.py`

 * *Files identical despite different names*

### Comparing `cascade-ml-0.8.0/cascade/utils/numpy_wrapper.py` & `cascade-ml-0.9.0/cascade/tests/test_concatenator.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,23 +10,43 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from typing import Dict, List
-import numpy as np
-from ..data import Wrapper
-
-
-class NumpyWrapper(Wrapper):
-    """
-    A wrapper around .npy files. Loads file in `__init__`.
-    """
-    def __init__(self, path: str, *args, **kwargs) -> None:
-        self._path = path
-        super().__init__(np.load(path), *args, **kwargs)
-
-    def get_meta(self) -> List[Dict]:
-        meta = super().get_meta()
-        meta[0]['root'] = self._path
+import os
+import sys
+import pytest
+
+MODULE_PATH = os.path.dirname(os.path.abspath(os.path.dirname(__file__)))
+sys.path.append(os.path.dirname(MODULE_PATH))
+
+from cascade.data import Wrapper
+from cascade.data import Concatenator
+
+
+def test_meta():
+    n1 = Wrapper([0, 1])
+    n2 = Wrapper([2, 3, 4, 5])
+
+    c = Concatenator([n1, n2], meta_prefix={'num': 1})
+    assert c.get_meta()[0]['num'] == 1
+    assert len(c.get_meta()[0]['data']) == 2
+
+
+@pytest.mark.parametrize(
+    'arrs', [
+        (Wrapper([0]), Wrapper([0]), Wrapper([0])),
+        (Wrapper([1, 2, 3, 4]), Wrapper([11])),
+        (Wrapper([1]),),
+        (Wrapper([1, 2, 3, 4]), Wrapper([]))
+    ]
+)
+def test_concatenation(arrs):
+    c = Concatenator([*arrs])
+
+    res = []
+    for arr in arrs:
+        res += arr
+
+    assert [c[i] for i in range(len(c))] == res
```

### Comparing `cascade-ml-0.8.0/cascade/utils/oversampler.py` & `cascade-ml-0.9.0/cascade/utils/oversampler.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from ..data import T, Dataset, Sampler
+from typing import Tuple, Any
+
+from ..data import SizedDataset, Sampler
 from numpy import unique, max
 from tqdm import trange
 
 
 class OverSampler(Sampler):
     """
     Accepts datasets which return tuples of objects and labels in the respected order.
@@ -32,15 +34,15 @@
     Labels are considered to be in the second place of each item that a dataset returns.
 
     Important
     ---------
     Sampler orders the items in the dataset.
     Consider shuffling the dataset after sampling if label order is important.
     """
-    def __init__(self, dataset: Dataset, *args, **kwargs) -> None:
+    def __init__(self, dataset: SizedDataset[Tuple[Any, Any]], *args: Any, **kwargs: Any) -> None:
         labels = [int(dataset[i][1]) for i in trange(len(dataset))]
         ulabels, counts = unique(labels, return_counts=True)
         how_much_add = max(counts) - counts
 
         self._add_indices = []
         for label_idx, label in enumerate(ulabels):
             k = 0
@@ -50,15 +52,15 @@
                 self._add_indices.append(k)
 
         ln = len(dataset) + len(self._add_indices)
         print(f'Original length was {len(dataset)} and new is {ln}')
 
         super().__init__(dataset, num_samples=ln, *args, **kwargs)
 
-    def __getitem__(self, index: int) -> T:
+    def __getitem__(self, index: int) -> Tuple[Any, Any]:
         if index < len(self._dataset):
             return self._dataset[index]
         else:
             idx = self._add_indices[index - len(self._dataset)]
             return self._dataset[idx]
 
     def __len__(self) -> int:
```

### Comparing `cascade-ml-0.8.0/cascade/utils/sk_model.py` & `cascade-ml-0.9.0/cascade/utils/sk_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,64 +14,64 @@
 limitations under the License.
 """
 
 import os
 import glob
 from hashlib import md5
 import pickle
-from typing import Any, Dict, List
+from typing import Any, Dict, List, Union, Any
 from sklearn.pipeline import Pipeline
 
-from ..base import MetaHandler
+from ..base import MetaHandler, Meta
 from ..models import BasicModel
 
 
 class SkModel(BasicModel):
     """
     Wrapper for sklearn models.
     Accepts the name and block to form pipeline.
     Can fit, evaluate, predict save and load out of the box.
     """
-    def __init__(self, blocks=None, **kwargs) -> None:
+    def __init__(self, *args: Any, blocks: Union[List[Any], None]=None, **kwargs: Any) -> None:
         """
         Parameters
         ----------
         name: str, optional
             Name of the model
         blocks: list, optional
             List of sklearn transformers to make a pipeline from
         """
-        super().__init__(**kwargs)
+        super().__init__(*args, **kwargs)
 
         if blocks is not None:
             self._pipeline = self._construct_pipeline(blocks)
 
     @staticmethod
     def _construct_pipeline(blocks: List[Any]) -> Pipeline:
         return Pipeline([(str(i), block) for i, block in enumerate(blocks)])
 
-    def fit(self, x, y, *args, **kwargs) -> None:
+    def fit(self, x: Any, y: Any, *args: Any, **kwargs: Any) -> None:
         """
         Wrapper for pipeline.fit
         """
         self._pipeline.fit(x, y, *args, **kwargs)
 
-    def predict(self, x, *args, **kwargs):
+    def predict(self, x: Any, *args: Any, **kwargs: Any) -> Any:
         """
         Wrapper for pipeline.predict
         """
         return self._pipeline.predict(x, *args, **kwargs)
 
-    def predict_proba(self, x, *args, **kwargs):
+    def predict_proba(self, x: Any, *args: Any, **kwargs: Any) -> Any:
         """
         Wrapper for pipeline.predict_proba
         """
         return self._pipeline.predict_proba(x, *args, **kwargs)
 
-    def _check_model_hash(self, path) -> None:
+    def _check_model_hash(self, path: str) -> None:
         root = os.path.dirname(path)
         names = glob.glob(os.path.join(f'{root}', 'meta.*'))
         if len(names) == 1:
             meta = MetaHandler().read(names[0])
             # Uses first meta in list
             # Usually the list is of unit length
             meta = meta[0]
@@ -84,15 +84,15 @@
                         f'it may be that model\'s .pkl file was corrupted\n'
                         f'hash from {names[0]}: {meta["md5sum"]}\n'
                         f'hash of {path}: {file_hash}'
                     )
         elif len(names) > 1:
             raise RuntimeError(f'Multiple possible meta-files found: {names}')
 
-    def load(self, path, check_hash=True) -> None:
+    def load(self, path: str, check_hash: bool = True) -> None:
         """
         Loads the model from path provided. If no extension, .pkl is added.
         """
         if os.path.splitext(path)[-1] != '.pkl':
             path += '.pkl'
 
         if check_hash:
@@ -107,13 +107,13 @@
         If no extension, then .pkl is added.
         """
         if os.path.splitext(path)[-1] != '.pkl':
             path += '.pkl'
         with open(f'{path}', 'wb') as f:
             pickle.dump(self._pipeline, f)
 
-    def get_meta(self) -> List[Dict]:
+    def get_meta(self) -> Meta:
         meta = super().get_meta()
         meta[0].update({
             'pipeline': repr(self._pipeline)
         })
         return meta
```

### Comparing `cascade-ml-0.8.0/cascade/utils/table_dataset.py` & `cascade-ml-0.9.0/cascade/utils/table_dataset.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,28 +10,28 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from typing import List, Dict, Iterable
+from typing import List, Union, Any, Literal
 import pandas as pd
 from dask import dataframe as dd
 
 from ..meta import AggregateValidator, DataValidationException
 from ..data import Dataset, Modifier, Iterator, SequentialCacher
-
+from ..base import Meta
 
 class TableDataset(Dataset):
     """
     Wrapper for `pd.DataFrame`s which allows to manage metadata and perform
     validation.
     """
-    def __init__(self, *args, t=None, **kwargs):
+    def __init__(self, *args: Any, t: Union[pd.DataFrame, None] = None, **kwargs: Any) -> None:
         """
         Parameters
         ----------
         t: optional
             pd.DataFrame or TableDataset to be set as table
         """
         super().__init__(*args, **kwargs)
@@ -40,53 +40,53 @@
         elif isinstance(t, TableDataset):
             self._table = t._table
         elif t is None:
             self._table = pd.DataFrame()
         else:
             raise TypeError('Input table is not a pandas.DataFrame nor TableDataset')
 
-    def __getitem__(self, index):
+    def __getitem__(self, index: int) -> pd.Series:
         """
         Returns a row from table by index
         """
         return self._table.iloc[index]
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f'{super().__repr__()}\n {repr(self._table)}'
 
-    def __len__(self):
+    def __len__(self) -> int:
         """
         Returns length of the table
         """
         return len(self._table)
 
-    def get_meta(self) -> List[Dict]:
+    def get_meta(self) -> Meta:
         meta = super().get_meta()
         meta[0].update({
             'name': repr(self),
             'columns': list(self._table.columns),
             'len': len(self),
             'info': self._table.describe().to_dict()
         })
         return meta
 
-    def to_csv(self, path, **kwargs):
+    def to_csv(self, path: str, **kwargs: Any) -> None:
         """
         Saves the table to .csv file. Any kwargs are sent to
         `pd.DataFrame.to_csv`.
         """
         self._table.to_csv(path, **kwargs)
 
 
 class TableFilter(TableDataset, Modifier):
     """
     Filter for table values
     """
     def __init__(self, dataset: TableDataset,
-                 mask: Iterable[bool], *args, **kwargs):
+                 mask: List[bool], *args: Any, **kwargs: Any) -> None:
         """
         Parameters
         ----------
         dataset: TableDataset
             Dataset to be filtered.
         mask: Iterable[bool]
             Binary mask to select values from table.
@@ -98,15 +98,15 @@
         print(f'Length before filtering: {init_len}, length after: {len(self._table)}')
 
 
 class CSVDataset(TableDataset):
     """
     Wrapper for .csv files.
     """
-    def __init__(self, csv_file_path, *args, **kwargs):
+    def __init__(self, csv_file_path: str, *args: Any, **kwargs: Any) -> None:
         """
         Passes all args and kwargs to `pd.read_csv`
 
         Parameters
         ----------
         csv_file_path:
             path to the .csv file
@@ -120,36 +120,37 @@
     Works like CSVDataset, but uses dask to load tables
     and returns partitions on `__getitem__`.
 
     See also
     --------
     cascade.utils.CSVDataset
     """
-    def __init__(self, csv_file_path, *args, **kwargs):
+    def __init__(self, csv_file_path: str, *args: Any, **kwargs: Any) -> None:
         super().__init__(**kwargs)
         self._table = dd.read_csv(csv_file_path, *args, **kwargs)
 
-    def __getitem__(self, index):
+    def __getitem__(self, index: int):
         """
         Returns partition under the index.
         """
         return self._table.get_partition(index).compute()
 
-    def __len__(self):
+    def __len__(self) -> int:
         """
         Returns the number of partitions.
         """
         return self._table.npartitions
 
 
 class TableIterator(Iterator):
     """
     Iterates over the table from path by the chunks.
     """
-    def __init__(self, csv_file_path: str, *args, chunk_size: int = 1000, **kwargs):
+    def __init__(self, csv_file_path: str, *args: Any,
+                 chunk_size: int = 1000, **kwargs: Any) -> None:
         """
         Parameters
         ----------
         csv_file_path: str
             Path to the .csv file
         chunk_size: int, optional
             number of rows to return in one __next__
@@ -163,37 +164,37 @@
 
 
 class LargeCSVDataset(SequentialCacher):
     """
     SequentialCacher over large .csv file.
     Loads table by partitions.
     """
-    def __init__(self, csv_file_path, *args, **kwargs):
+    def __init__(self, csv_file_path: str, *args: Any, **kwargs: Any) -> None:
         dataset = PartedTableLoader(csv_file_path, *args, **kwargs)
-        self.len = len(dataset._table)
+        self._ln = len(dataset._table)
         self.num_batches = dataset._table.npartitions
-        self.bs = self.len // self.num_batches
+        self.bs = self._ln // self.num_batches
         super().__init__(dataset, self.bs)
 
-    def _load(self, index):
+    def _load(self, index: int) -> None:
         self._batch = TableDataset(t=self._dataset[index])
 
-    def __len__(self):
-        return self.len
+    def __len__(self) -> int:
+        return self._ln
 
 
 class NullValidator(TableDataset, AggregateValidator):
     """
     Checks that there are no null values in the table.
     """
-    def __init__(self, dataset: TableDataset, *args, **kwargs) -> None:
+    def __init__(self, dataset: TableDataset, *args: Any, **kwargs: Any) -> None:
         super().__init__(dataset, self._check_nulls,
                          *args, t=dataset._table, **kwargs)
 
-    def _check_nulls(self, x):
+    def _check_nulls(self, x: TableDataset) -> Literal[True]:
         mask = x._table.isnull().values
         if ~(mask.any()):
             return True
         else:
             total = mask.sum()
             by_columns = mask.sum(axis=0)
             missing = pd.DataFrame(by_columns.reshape(1, len(by_columns)), columns=x._table.columns)
```

### Comparing `cascade-ml-0.8.0/cascade/utils/text_classification_dataset.py` & `cascade-ml-0.9.0/cascade/utils/text_classification_dataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,26 +11,27 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import os
-from typing import List, Dict
+from typing import Any, Tuple
 
 import numpy as np
 from ..data import Dataset
+from ..base import Meta
 
 
 class TextClassificationDataset(Dataset):
     """
     Dataset to simplify loading of data for text classification.
     Texts of different classes should be placed in different folders.
     """
-    def __init__(self, path: str, encoding: str = 'utf-8', *args, **kwargs):
+    def __init__(self, path: str, encoding: str = 'utf-8', *args: Any, **kwargs: Any) -> None:
         """
         Parameters
         ----------
         path: str
             Path to the folder with folders of text files.
             In each folder should be only one class of texts.
         encoding: str, optional
@@ -48,27 +49,27 @@
             self._paths += [os.path.join(self._root, folder, f) for f in files]
             self._labels += [i for _ in range(len(files))]
 
         classes = [(folder, len(os.listdir(os.path.join(self._root, folder))))
                    for folder in folders]
         print(f'Found {len(folders)} classes: {classes}')
 
-    def __getitem__(self, index):
+    def __getitem__(self, index: int) -> Tuple[str, int]:
         with open(self._paths[index], 'r', encoding=self._encoding) as f:
             text = ' '.join(f.readlines())
             label = self._labels[index]
         return text, label
 
-    def __len__(self):
+    def __len__(self) -> int:
         """
         Total number of files.
         """
         return len(self._paths)
 
-    def get_meta(self) -> List[Dict]:
+    def get_meta(self) -> Meta:
         meta = super().get_meta()
         meta[0].update({
             'name': repr(self),
             'size': len(self),
             'root': self._root,
             'labels': np.unique(self._labels).tolist()
         })
```

### Comparing `cascade-ml-0.8.0/cascade/utils/time_series_dataset.py` & `cascade-ml-0.9.0/cascade/utils/time_series_dataset.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,32 +10,36 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from typing import Iterable
+from typing import Iterable, Any, Union, Tuple
 
 import pendulum
 from datetime import datetime
 import numpy as np
 import pandas as pd
 
+from ..base import Meta
 from ..data import Dataset, Modifier
 
 
 class TimeSeriesDataset(Dataset):
     """
     Dataset to simplify the work with time series.
     Manages the time and data. Reflects the list API
     and implements access by index and by datetime also.
     More than that, slices with indices and with datetimes can also be used.
     """
-    def __init__(self, *args, time=None, data=None, **kwargs):
+    def __init__(self, *args: Any,
+                 time: Union[Iterable[datetime], None] = None,
+                 data: Union[Iterable[Any], None] = None,
+                 **kwargs: Any) -> None:
         """
         Parameters
         ----------
         time: Iterable[datetime], optional
             The time dimension. Should be represented subclasses of datetime
         data: Iterable, optional
             The data dimension. Should be 1D array or list.
@@ -66,44 +70,44 @@
         self._time = time
         self._num_idx = [i for i in range(len(data))]
         index = pd.MultiIndex.from_frame(
             pd.DataFrame(self._time, self._num_idx))
         self._table = pd.DataFrame(data, index=index)
         super().__init__(*args, **kwargs)
 
-    def to_numpy(self):
+    def to_numpy(self) -> np.ndarray:
         """
         Returns only data without time in numpy array format.
 
         Returns
         -------
         data: np.ndarray
             np.array of data.
         """
         return self._table.to_numpy().T[0]
 
-    def to_pandas(self):
+    def to_pandas(self) -> pd.DataFrame:
         """
         Returns
         -------
         data: pd.DataFrame
             table with time as index
         """
         return pd.DataFrame(self.to_numpy(), index=self._time)
 
-    def get_data(self):
+    def get_data(self) -> Tuple[np.ndarray, np.ndarray]:
         """
         Returns
         -------
         data: tuple
             Time and data as np.array
         """
         return self._time, self.to_numpy()
 
-    def _get_slice(self, index):
+    def _get_slice(self, index: int):
         # If date slice
         if isinstance(index.start, datetime) or \
                 isinstance(index.stop, datetime):
 
             start = np.where(self._time == index.start)[0][0] \
                 if index.start is not None else None
             stop = np.where(self._time == index.stop)[0][0] \
@@ -116,29 +120,29 @@
         else:
             # If int slice
             time = self._time[index]
             data = self._table.iloc[index].to_numpy().T[0]
 
         return TimeSeriesDataset(time=time, data=data)
 
-    def _get_where(self, index):
+    def _get_where(self, index: Union[int, slice]):
         if isinstance(index[0], slice):
             raise NotImplementedError()
 
         if isinstance(index[0], datetime):
             new_time = np.array(index)
         else:
             new_time = self._time[[i for i in index]]
 
         new_data = np.zeros(len(index))
         for k, i in enumerate(index):
             new_data[k] = self[i]
         return TimeSeriesDataset(time=new_time, data=new_data)
 
-    def __getitem__(self, index):
+    def __getitem__(self, index: Union[int, slice, datetime, Iterable[int]]):
         if isinstance(index, slice):
             if index.step is not None:
                 raise NotImplementedError()
             return self._get_slice(index)
         elif isinstance(index, int):
             return self._table.iloc[index].item()
         elif isinstance(index, datetime):
@@ -146,25 +150,36 @@
         elif isinstance(index, Iterable):
             return self._get_where(index)
         else:
             raise NotImplementedError(
                 f'__getitem__ is not implemented for {type(index)}'
             )
 
-    def __len__(self):
+    def __len__(self) -> int:
         return len(self._num_idx)
 
+    def get_meta(self) -> Meta:
+        meta = super().get_meta()
+        meta[0].update(
+            {
+                'time_from': self._time[0],
+                'time_to': self._time[-1],
+                'info': self._table.describe().to_dict()
+            }
+        )
+        return meta
+
 
 class Average(TimeSeriesDataset, Modifier):
     """
     Averages values over some time step.
     """
     def __init__(self, dataset: TimeSeriesDataset,
                  unit: str = 'years',
-                 amount=1, *args, **kwargs):
+                 amount: int = 1, *args: Any, **kwargs: Any) -> None:
         """
         Parameters
         ----------
         dataset: TimeSeriesDataset,
             A dataset to average
         unit: str, optional
             Time unit over which to average - years, month, etc.
@@ -177,17 +192,30 @@
                     .period(time[0], time[-1])
                     .range(unit, amount=amount)]
 
         reg_data = self._avg(data, time, reg_time)
         assert len(reg_data) > 1, 'Please, provide unit that ' \
                                   'would get more than one period'
 
+        self._unit = unit
+        self._amount = amount
+
         super().__init__(dataset, time=reg_time,
                          data=reg_data, *args, **kwargs)
 
+    def get_meta(self) -> Meta:
+        meta = super().get_meta()
+        meta[0].update(
+            {
+                'unit': self._unit,
+                'amount': self._amount
+            }
+        )
+        return meta
+
     @staticmethod
     def _avg(arr, arr_dates, dates):
         new_p = np.zeros(len(dates))
         for i in range(len(dates) - 1):
             data = arr[(arr_dates >= dates[i]) & (arr_dates < dates[i + 1])]
             mean = np.nanmean(data)
             new_p[i] = mean
@@ -196,26 +224,42 @@
         return new_p
 
 
 class Interpolate(TimeSeriesDataset, Modifier):
     """
     The wrapper around pd.Series.interpolate.
     """
-    def __init__(self, dataset, method='linear',
-                 limit_direction='both', **kwargs):
+    def __init__(self, dataset: TimeSeriesDataset,
+                 method: str = 'linear',
+                 limit_direction: str = 'both',
+                 **kwargs: Any) -> None:
         t = dataset.to_pandas()
         time, _ = dataset.get_data()
         t.index = pd.Index(time)
         t = t[0].interpolate(method=method, limit_direction=limit_direction)
         super().__init__(dataset, time=time, data=t.to_numpy(), **kwargs)
 
+        self._method = method
+        self._limit_direction = limit_direction
+
+    def get_meta(self) -> Meta:
+        meta = super().get_meta()
+        meta[0].update(
+            {
+                'method': self._method,
+                'limit_direction': self._limit_direction
+            }
+        )
+        return meta
+
 
 class Align(TimeSeriesDataset, Modifier):
     """
     Given dataset and some time scale selects
     data from dataset using time scale. Works
     only if dataset has data in given points
     in time.
     """
-    def __init__(self, dataset, time, *args, **kwargs):
+    def __init__(self, dataset: TimeSeriesDataset,
+                 time: Iterable[datetime], *args: Any, **kwargs: Any) -> None:
         super().__init__(dataset, time=time,
                          data=dataset[time], *args, **kwargs)
```

### Comparing `cascade-ml-0.8.0/cascade/utils/torch_model.py` & `cascade-ml-0.9.0/cascade/utils/baselines.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,53 +10,47 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from typing import Dict, List
-import torch
-from ..models import Model
+import json
+from typing import Union, List, Any
+import numpy as np
+from ..models import BasicModel
 
+Number = Union[int, float, complex, np.number]
 
-class TorchModel(Model):
+
+class ConstantBaseline(BasicModel):
     """
-    The wrapper around `nn.Module`s.
+    Constant function. This baseline can be used for
+    any classification task. It returns only one class
+    (for example it can be majority class)
     """
-    def __init__(self, model_class: type, *args, **kwargs) -> None:
-        """
-        Parameters
-        ----------
-        model_class: type
-            The class created when new nn.Module was defined. Will be used
-            to construct model. If any arguments needed, please pass them
-            into `args` and `kwargs`.
-        """
-        self._model = model_class(*args, **kwargs)
-        super().__init__(*args, **kwargs)
-
-    def predict(self, *args, **kwargs):
-        """
-        Calls internal module with whatever arguments.
-        """
-        return self._model(*args, **kwargs)
-
-    def save(self, path: str, *args, **kwargs) -> None:
-        """
-        Saves the model using `torch.save`.
-        """
-        with open(path, 'wb') as f:
-            # TODO: pass args and kwargs
-            torch.save(self._model, f)
-
-    def load(self, path: str, *args, **kwargs) -> None:
-        """
-        Loads the model using `torch.load`.
-        """
-        with open(path, 'rb') as f:
-            self._model = torch.load(f)
-
-    def get_meta(self) -> List[Dict]:
-        meta = super().get_meta()
-        meta[0]['module'] = repr(self._model)
-        return meta
+    def __init__(self, constant: Union[List[Any], Number, None] = None, **kwargs: Any) -> None:
+        super().__init__(**kwargs)
+        self._constant = constant
+
+    def fit(self, x: Any, y: Any, *args: Any, **kwargs: Any) -> None:
+        pass
+
+    # Should be able to:
+    # give constant of desired shape
+    # give any number of given constant vectors as output
+    def predict(self, x: Any, *args: Any, **kwargs: Any) -> np.ndarray:
+        """
+        Returns the array of the same shape as input full of
+        given constant.
+        """
+        # TODO: make more universal when work with input shape
+        return np.asarray([self._constant for _ in range(len(x))])
+
+    def save(self, path: str) -> None:
+        with open(path, 'w') as f:
+            json.dump({'constant': self._constant}, f)
+
+    def load(self, path: str) -> None:
+        with open(path, 'r') as f:
+            obj = json.load(f)
+            self._constant = obj['constant']
```

### Comparing `cascade-ml-0.8.0/cascade/utils/undersampler.py` & `cascade-ml-0.9.0/cascade/utils/undersampler.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,18 +10,21 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from ..data import T, Dataset, Sampler
+from typing import Any, Tuple
+
 from numpy import unique, min
 from tqdm import trange
 
+from ..data import SizedDataset, Sampler
+
 
 class UnderSampler(Sampler):
     """
     Accepts datasets which return tuples of objects and labels.
     Isn't lazy - runs through all the items ones to determine key order.
     Doesn't store values in memory afterwards.
 
@@ -32,30 +35,31 @@
     Labels are considered to be in the second place of each item that a dataset returns.
 
     Important
     ---------
     Sampler orders the items in the dataset.
     Consider shuffling the dataset after sampling if label order is important.
     """
-    def __init__(self, dataset: Dataset) -> None:
+    def __init__(self, dataset: SizedDataset[Tuple[Any, Any]], *args: Any, **kwargs: Any) -> None:
         labels = [int(dataset[i][1]) for i in trange(len(dataset))]
         ulabels, counts = unique(labels, return_counts=True)
         min_count = min(counts)
 
         self._rem_indices = []
         for label in ulabels:
             k = 0
             for _ in range(min_count):
                 while labels[k] != label:
                     k += 1
                 self._rem_indices.append(k)
+                k += 1
 
         ln = len(self._rem_indices)
         print(f'Original length was {len(dataset)} and new is {ln}')
-        super().__init__(dataset, ln)
+        super().__init__(dataset, ln, *args, **kwargs)
 
-    def __getitem__(self, index: int) -> T:
+    def __getitem__(self, index: int) -> Tuple[Any, Any]:
         idx = self._rem_indices[index]
         return self._dataset[idx]
 
-    def __len__(self):
+    def __len__(self) -> int:
         return len(self._rem_indices)
```

### Comparing `cascade-ml-0.8.0/cascade/utils/weighed_sampler.py` & `cascade-ml-0.9.0/cascade/utils/weighed_sampler.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,20 +10,23 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from typing import Any, Dict
-from ..data import T, Dataset, Sampler
+from typing import Any, Dict, Union, Tuple
+
 from itertools import cycle
 import numpy as np
 from tqdm import trange
 
+from ..data import SizedDataset, Sampler
+from ..base import Meta
+
 
 class WeighedSampler(Sampler):
     """
     Samples each class certain amount of times.
 
     Important
     ---------
@@ -39,31 +42,34 @@
 
     See also
     --------
     cascade.utils.OverSampler
     cascade.utils.UnderSampler
     cascade.data.RandomSampler
     """
-    def __init__(self, dataset: Dataset, partitioning: Dict[Any, int] = None) -> None:
+    def __init__(self, dataset: SizedDataset[Tuple[Any, Any]],
+                 partitioning: Union[Dict[Any, int], None] = None) -> None:
         """
         Parameters
         ----------
             dataset: Dataset
                 A dataset to sample
             partitioning: Dict[Any, int], optional
                 A dictionary with labels as keys and the number of samples as values.
                 If some label omitted, assumes that it should be sampled the same number
                 of times it is actually appears in the dataset.
         """
+        labels = np.asarray([dataset[i][1] for i in trange(len(dataset))])
+        ulabels, counts = np.unique(labels, return_counts=True)
+
         if partitioning is None:
             partitioning = {}
 
+        self._check_partitioning(ulabels, partitioning)
         self._partitioning = partitioning
-        labels = np.asarray([int(dataset[i][1]) for i in trange(len(dataset))])
-        ulabels, counts = np.unique(labels, return_counts=True)
 
         # If label is omitted in partitioning, add it with true count
         for ulabel, count in zip(ulabels, counts):
             if ulabel not in self._partitioning:
                 self._partitioning[ulabel] = count
 
         self._indices = []
@@ -73,19 +79,29 @@
                 if count >= self._partitioning[label]:
                     break
 
                 self._indices.append(idx)
                 count += 1
 
         ln = len(self._indices)
-        assert ln == sum(partitioning.values()), 'The length should be equal to the sum of partitions'
+        assert ln == sum(partitioning.values()), \
+            'The length should be equal to the sum of partitions - something went wrong'
         print(f'Original length was {len(dataset)} and new is {ln}')
         super().__init__(dataset, ln)
 
-    def __getitem__(self, index: int) -> T:
+    def __getitem__(self, index: int) -> Tuple[Any, Any]:
         idx = self._indices[index]
         return self._dataset[idx]
 
-    def get_meta(self):
+    def get_meta(self) -> Meta:
         meta = super().get_meta()
         meta[0]['partitioning'] = self._partitioning
         return meta
+
+    def _check_partitioning(self, ulabels, partitioning) -> None:
+        '''
+        Checks if all labels that were passed in partitioning
+        are present in dataset's unique labels
+        '''
+        for label in partitioning:
+            if label not in ulabels:
+                raise ValueError(f'Label {label} was not found in dataset\'s labels: {ulabels}')
```

### Comparing `cascade-ml-0.8.0/cascade_ml.egg-info/PKG-INFO` & `cascade-ml-0.9.0/cascade_ml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cascade-ml
-Version: 0.8.0
+Version: 0.9.0
 Summary: ML-Engineering library
 Home-page: https://github.com/oxid15/cascade
 Author: Ilia Moiseev
 Author-email: ilia.moiseev.5@yandex.ru
 License: Apache License 2.0
 Project-URL: Documentation, https://oxid15.github.io/cascade
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cascade-ml-0.8.0/cascade_ml.egg-info/SOURCES.txt` & `cascade-ml-0.9.0/cascade_ml.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 ./cascade/meta/__init__.py
 ./cascade/meta/dataleak_validator.py
 ./cascade/meta/hashes.py
 ./cascade/meta/history_viewer.py
 ./cascade/meta/meta_validator.py
 ./cascade/meta/meta_viewer.py
 ./cascade/meta/metric_viewer.py
+./cascade/meta/utils.py
 ./cascade/meta/validator.py
 ./cascade/models/__init__.py
 ./cascade/models/basic_model.py
 ./cascade/models/model.py
 ./cascade/models/model_line.py
 ./cascade/models/model_repo.py
 ./cascade/models/trainer.py
@@ -59,15 +60,14 @@
 ./cascade/tests/test_random_sampler.py
 ./cascade/tests/test_range_sampler.py
 ./cascade/tests/test_sequential_cacher.py
 ./cascade/tests/test_traceable.py
 ./cascade/tests/test_trainer.py
 ./cascade/tests/test_validator.py
 ./cascade/tests/test_version_assigner.py
-./cascade/tests/test_weighed_sampler.py
 ./cascade/utils/__init__.py
 ./cascade/utils/baselines.py
 ./cascade/utils/folder_image_dataset.py
 ./cascade/utils/model_aggregate.py
 ./cascade/utils/numpy_wrapper.py
 ./cascade/utils/oversampler.py
 ./cascade/utils/pa_schema_validator.py
```

### Comparing `cascade-ml-0.8.0/setup.py` & `cascade-ml-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="cascade-ml",
-    version='0.8.0',
+    version='0.9.0',
     author='Ilia Moiseev',
     author_email='ilia.moiseev.5@yandex.ru',
     license='Apache License 2.0',
     description="ML-Engineering library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/oxid15/cascade",
```

