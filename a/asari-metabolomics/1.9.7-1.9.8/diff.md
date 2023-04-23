# Comparing `tmp/asari-metabolomics-1.9.7.tar.gz` & `tmp/asari-metabolomics-1.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/shuzhao/li.github/asari/dist/.tmp-c97jb_5n/asari-metabolomics-1.9.7.tar", last modified: Mon Jan  9 18:07:21 2023, max compression
+gzip compressed data, was "/Users/shuzhao/li.github/asari/dist/.tmp-u763dpoq/asari-metabolomics-1.9.8.tar", last modified: Thu Jan 12 01:22:54 2023, max compression
```

## Comparing `asari-metabolomics-1.9.7.tar` & `asari-metabolomics-1.9.8.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 shuzhao    (501) staff       (20)        0 2023-01-09 18:07:21.000000 asari-metabolomics-1.9.7/
--rwxr-xr-x   0 shuzhao    (501) staff       (20)      360 2021-09-07 19:59:03.000000 asari-metabolomics-1.9.7/LICENSE
--rw-r--r--   0 shuzhao    (501) staff       (20)     9520 2023-01-09 18:07:21.000000 asari-metabolomics-1.9.7/PKG-INFO
--rwxr-xr-x   0 shuzhao    (501) staff       (20)     8673 2023-01-09 18:05:11.000000 asari-metabolomics-1.9.7/README.md
-drwxr-xr-x   0 shuzhao    (501) staff       (20)        0 2023-01-09 18:07:21.000000 asari-metabolomics-1.9.7/asari/
--rw-r--r--   0 shuzhao    (501) staff       (20)       22 2023-01-09 15:49:16.000000 asari-metabolomics-1.9.7/asari/__init__.py
--rw-r--r--   0 shuzhao    (501) staff       (20)     2197 2021-09-08 18:46:12.000000 asari-metabolomics-1.9.7/asari/_test.py
--rw-r--r--   0 shuzhao    (501) staff       (20)     8625 2022-12-31 20:57:07.000000 asari-metabolomics-1.9.7/asari/analyze.py
--rw-r--r--   0 shuzhao    (501) staff       (20)     2449 2023-01-01 22:50:59.000000 asari-metabolomics-1.9.7/asari/annotate_user_table.py
--rw-r--r--   0 shuzhao    (501) staff       (20)    15413 2022-05-23 17:18:00.000000 asari-metabolomics-1.9.7/asari/chromatograms.py
--rw-r--r--   0 shuzhao    (501) staff       (20)       24 2022-03-17 01:30:11.000000 asari-metabolomics-1.9.7/asari/command_line.py
--rw-r--r--   0 shuzhao    (501) staff       (20)    21089 2023-01-09 16:54:40.000000 asari-metabolomics-1.9.7/asari/constructors.py
--rw-r--r--   0 shuzhao    (501) staff       (20)    12469 2022-05-22 14:30:28.000000 asari-metabolomics-1.9.7/asari/dashboard.py
-drwxr-xr-x   0 shuzhao    (501) staff       (20)        0 2023-01-09 18:07:21.000000 asari-metabolomics-1.9.7/asari/db/
--rw-r--r--   0 shuzhao    (501) staff       (20)        0 2021-12-12 13:57:25.000000 asari-metabolomics-1.9.7/asari/db/__init__.py
--rw-r--r--   0 shuzhao    (501) staff       (20)     4732 2022-03-11 18:32:37.000000 asari-metabolomics-1.9.7/asari/db/calibration_dbs.py
--rw-r--r--   0 shuzhao    (501) staff       (20)  3215952 2022-02-15 01:41:57.000000 asari-metabolomics-1.9.7/asari/db/emp_cpds_trees.pickle
--rw-r--r--   0 shuzhao    (501) staff       (20) 30809306 2022-02-15 01:41:12.000000 asari-metabolomics-1.9.7/asari/db/mass_indexed_compounds.pickle
--rw-r--r--   0 shuzhao    (501) staff       (20)     3736 2023-01-09 18:05:11.000000 asari-metabolomics-1.9.7/asari/defaul_parameters.py
--rw-r--r--   0 shuzhao    (501) staff       (20)    18348 2023-01-09 16:54:40.000000 asari-metabolomics-1.9.7/asari/experiment.py
--rw-r--r--   0 shuzhao    (501) staff       (20)      513 2022-02-24 14:02:12.000000 asari-metabolomics-1.9.7/asari/json_encoder.py
--rw-r--r--   0 shuzhao    (501) staff       (20)     6103 2023-01-09 16:01:14.000000 asari-metabolomics-1.9.7/asari/main.py
--rw-r--r--   0 shuzhao    (501) staff       (20)    19548 2022-12-31 21:12:11.000000 asari-metabolomics-1.9.7/asari/mass_functions.py
--rw-r--r--   0 shuzhao    (501) staff       (20)     3879 2022-03-11 18:32:37.000000 asari-metabolomics-1.9.7/asari/mongo.py
--rw-r--r--   0 shuzhao    (501) staff       (20)    28999 2023-01-09 16:52:30.000000 asari-metabolomics-1.9.7/asari/peaks.py
--rw-r--r--   0 shuzhao    (501) staff       (20)     4052 2022-04-26 13:01:07.000000 asari-metabolomics-1.9.7/asari/samples.py
-drwxr-xr-x   0 shuzhao    (501) staff       (20)        0 2023-01-09 18:07:21.000000 asari-metabolomics-1.9.7/asari/tools/
--rw-r--r--   0 shuzhao    (501) staff       (20)        0 2022-04-11 22:02:28.000000 asari-metabolomics-1.9.7/asari/tools/__init__.py
--rw-r--r--   0 shuzhao    (501) staff       (20)     1972 2022-04-11 22:03:08.000000 asari-metabolomics-1.9.7/asari/tools/extract_masstracks.py
--rw-r--r--   0 shuzhao    (501) staff       (20)     7459 2021-09-28 12:26:36.000000 asari-metabolomics-1.9.7/asari/tools/merge.py
--rw-r--r--   0 shuzhao    (501) staff       (20)     7414 2022-05-03 01:39:21.000000 asari-metabolomics-1.9.7/asari/tools/plot.py
--rw-r--r--   0 shuzhao    (501) staff       (20)    10337 2022-12-31 21:38:58.000000 asari-metabolomics-1.9.7/asari/workflow.py
-drwxr-xr-x   0 shuzhao    (501) staff       (20)        0 2023-01-09 18:07:21.000000 asari-metabolomics-1.9.7/asari_metabolomics.egg-info/
--rw-r--r--   0 shuzhao    (501) staff       (20)     9520 2023-01-09 18:07:21.000000 asari-metabolomics-1.9.7/asari_metabolomics.egg-info/PKG-INFO
--rw-r--r--   0 shuzhao    (501) staff       (20)      872 2023-01-09 18:07:21.000000 asari-metabolomics-1.9.7/asari_metabolomics.egg-info/SOURCES.txt
--rw-r--r--   0 shuzhao    (501) staff       (20)        1 2023-01-09 18:07:21.000000 asari-metabolomics-1.9.7/asari_metabolomics.egg-info/dependency_links.txt
--rw-r--r--   0 shuzhao    (501) staff       (20)       50 2023-01-09 18:07:21.000000 asari-metabolomics-1.9.7/asari_metabolomics.egg-info/entry_points.txt
--rw-r--r--   0 shuzhao    (501) staff       (20)      114 2023-01-09 18:07:21.000000 asari-metabolomics-1.9.7/asari_metabolomics.egg-info/requires.txt
--rw-r--r--   0 shuzhao    (501) staff       (20)        6 2023-01-09 18:07:21.000000 asari-metabolomics-1.9.7/asari_metabolomics.egg-info/top_level.txt
--rw-r--r--   0 shuzhao    (501) staff       (20)        1 2023-01-09 18:07:21.000000 asari-metabolomics-1.9.7/asari_metabolomics.egg-info/zip-safe
--rw-r--r--   0 shuzhao    (501) staff       (20)       38 2023-01-09 18:07:21.000000 asari-metabolomics-1.9.7/setup.cfg
--rwxr-xr-x   0 shuzhao    (501) staff       (20)     1489 2022-03-15 15:04:18.000000 asari-metabolomics-1.9.7/setup.py
+drwxr-xr-x   0 shuzhao    (501) staff       (20)        0 2023-01-12 01:22:54.000000 asari-metabolomics-1.9.8/
+-rwxr-xr-x   0 shuzhao    (501) staff       (20)      360 2021-09-07 19:59:03.000000 asari-metabolomics-1.9.8/LICENSE
+-rw-r--r--   0 shuzhao    (501) staff       (20)     9520 2023-01-12 01:22:54.000000 asari-metabolomics-1.9.8/PKG-INFO
+-rwxr-xr-x   0 shuzhao    (501) staff       (20)     8673 2023-01-09 18:05:11.000000 asari-metabolomics-1.9.8/README.md
+drwxr-xr-x   0 shuzhao    (501) staff       (20)        0 2023-01-12 01:22:54.000000 asari-metabolomics-1.9.8/asari/
+-rw-r--r--   0 shuzhao    (501) staff       (20)       22 2023-01-12 01:21:48.000000 asari-metabolomics-1.9.8/asari/__init__.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)     2197 2021-09-08 18:46:12.000000 asari-metabolomics-1.9.8/asari/_test.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)     8625 2022-12-31 20:57:07.000000 asari-metabolomics-1.9.8/asari/analyze.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)     2449 2023-01-01 22:50:59.000000 asari-metabolomics-1.9.8/asari/annotate_user_table.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)    15413 2022-05-23 17:18:00.000000 asari-metabolomics-1.9.8/asari/chromatograms.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)       24 2022-03-17 01:30:11.000000 asari-metabolomics-1.9.8/asari/command_line.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)    21089 2023-01-09 16:54:40.000000 asari-metabolomics-1.9.8/asari/constructors.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)    12469 2022-05-22 14:30:28.000000 asari-metabolomics-1.9.8/asari/dashboard.py
+drwxr-xr-x   0 shuzhao    (501) staff       (20)        0 2023-01-12 01:22:54.000000 asari-metabolomics-1.9.8/asari/db/
+-rw-r--r--   0 shuzhao    (501) staff       (20)        0 2021-12-12 13:57:25.000000 asari-metabolomics-1.9.8/asari/db/__init__.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)     4732 2022-03-11 18:32:37.000000 asari-metabolomics-1.9.8/asari/db/calibration_dbs.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)  3215952 2022-02-15 01:41:57.000000 asari-metabolomics-1.9.8/asari/db/emp_cpds_trees.pickle
+-rw-r--r--   0 shuzhao    (501) staff       (20) 30809306 2022-02-15 01:41:12.000000 asari-metabolomics-1.9.8/asari/db/mass_indexed_compounds.pickle
+-rw-r--r--   0 shuzhao    (501) staff       (20)     3737 2023-01-12 01:21:48.000000 asari-metabolomics-1.9.8/asari/defaul_parameters.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)    18374 2023-01-12 01:21:48.000000 asari-metabolomics-1.9.8/asari/experiment.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)      513 2022-02-24 14:02:12.000000 asari-metabolomics-1.9.8/asari/json_encoder.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)     6103 2023-01-09 16:01:14.000000 asari-metabolomics-1.9.8/asari/main.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)    19548 2022-12-31 21:12:11.000000 asari-metabolomics-1.9.8/asari/mass_functions.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)     3879 2022-03-11 18:32:37.000000 asari-metabolomics-1.9.8/asari/mongo.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)    29059 2023-01-12 01:21:48.000000 asari-metabolomics-1.9.8/asari/peaks.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)     4052 2022-04-26 13:01:07.000000 asari-metabolomics-1.9.8/asari/samples.py
+drwxr-xr-x   0 shuzhao    (501) staff       (20)        0 2023-01-12 01:22:54.000000 asari-metabolomics-1.9.8/asari/tools/
+-rw-r--r--   0 shuzhao    (501) staff       (20)        0 2022-04-11 22:02:28.000000 asari-metabolomics-1.9.8/asari/tools/__init__.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)     1972 2022-04-11 22:03:08.000000 asari-metabolomics-1.9.8/asari/tools/extract_masstracks.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)     7459 2021-09-28 12:26:36.000000 asari-metabolomics-1.9.8/asari/tools/merge.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)     7414 2022-05-03 01:39:21.000000 asari-metabolomics-1.9.8/asari/tools/plot.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)    10337 2022-12-31 21:38:58.000000 asari-metabolomics-1.9.8/asari/workflow.py
+drwxr-xr-x   0 shuzhao    (501) staff       (20)        0 2023-01-12 01:22:54.000000 asari-metabolomics-1.9.8/asari_metabolomics.egg-info/
+-rw-r--r--   0 shuzhao    (501) staff       (20)     9520 2023-01-12 01:22:54.000000 asari-metabolomics-1.9.8/asari_metabolomics.egg-info/PKG-INFO
+-rw-r--r--   0 shuzhao    (501) staff       (20)      872 2023-01-12 01:22:54.000000 asari-metabolomics-1.9.8/asari_metabolomics.egg-info/SOURCES.txt
+-rw-r--r--   0 shuzhao    (501) staff       (20)        1 2023-01-12 01:22:54.000000 asari-metabolomics-1.9.8/asari_metabolomics.egg-info/dependency_links.txt
+-rw-r--r--   0 shuzhao    (501) staff       (20)       50 2023-01-12 01:22:54.000000 asari-metabolomics-1.9.8/asari_metabolomics.egg-info/entry_points.txt
+-rw-r--r--   0 shuzhao    (501) staff       (20)      133 2023-01-12 01:22:54.000000 asari-metabolomics-1.9.8/asari_metabolomics.egg-info/requires.txt
+-rw-r--r--   0 shuzhao    (501) staff       (20)        6 2023-01-12 01:22:54.000000 asari-metabolomics-1.9.8/asari_metabolomics.egg-info/top_level.txt
+-rw-r--r--   0 shuzhao    (501) staff       (20)        1 2023-01-12 01:22:53.000000 asari-metabolomics-1.9.8/asari_metabolomics.egg-info/zip-safe
+-rw-r--r--   0 shuzhao    (501) staff       (20)       38 2023-01-12 01:22:54.000000 asari-metabolomics-1.9.8/setup.cfg
+-rwxr-xr-x   0 shuzhao    (501) staff       (20)     1489 2022-03-15 15:04:18.000000 asari-metabolomics-1.9.8/setup.py
```

### Comparing `asari-metabolomics-1.9.7/PKG-INFO` & `asari-metabolomics-1.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asari-metabolomics
-Version: 1.9.7
+Version: 1.9.8
 Summary: LC-MS metabolomics data preprocessing
 Home-page: https://github.com/shuzhao-li/asari
 Author: Shuzhao Li
 Author-email: shuzhao.li@gmail.com
 License: BSD 3-Clause
 Keywords: metabolomics bioinformatics mass spectrometry
 Classifier: Intended Audience :: Developers
```

### Comparing `asari-metabolomics-1.9.7/README.md` & `asari-metabolomics-1.9.8/README.md`

 * *Files identical despite different names*

### Comparing `asari-metabolomics-1.9.7/asari/_test.py` & `asari-metabolomics-1.9.8/asari/_test.py`

 * *Files identical despite different names*

### Comparing `asari-metabolomics-1.9.7/asari/analyze.py` & `asari-metabolomics-1.9.8/asari/analyze.py`

 * *Files identical despite different names*

### Comparing `asari-metabolomics-1.9.7/asari/annotate_user_table.py` & `asari-metabolomics-1.9.8/asari/annotate_user_table.py`

 * *Files identical despite different names*

### Comparing `asari-metabolomics-1.9.7/asari/chromatograms.py` & `asari-metabolomics-1.9.8/asari/chromatograms.py`

 * *Files identical despite different names*

### Comparing `asari-metabolomics-1.9.7/asari/constructors.py` & `asari-metabolomics-1.9.8/asari/constructors.py`

 * *Files identical despite different names*

### Comparing `asari-metabolomics-1.9.7/asari/dashboard.py` & `asari-metabolomics-1.9.8/asari/dashboard.py`

 * *Files identical despite different names*

### Comparing `asari-metabolomics-1.9.7/asari/db/calibration_dbs.py` & `asari-metabolomics-1.9.8/asari/db/calibration_dbs.py`

 * *Files identical despite different names*

### Comparing `asari-metabolomics-1.9.7/asari/db/emp_cpds_trees.pickle` & `asari-metabolomics-1.9.8/asari/db/emp_cpds_trees.pickle`

 * *Files identical despite different names*

### Comparing `asari-metabolomics-1.9.7/asari/db/mass_indexed_compounds.pickle` & `asari-metabolomics-1.9.8/asari/db/mass_indexed_compounds.pickle`

 * *Files identical despite different names*

### Comparing `asari-metabolomics-1.9.7/asari/defaul_parameters.py` & `asari-metabolomics-1.9.8/asari/defaul_parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     
     # default output names
     'output_feature_table': 'Feature_table.tsv',
     'mass_grid_mapping': "_mass_grid_mapping.csv",
     'annotation_filename': "Annotation_table.tsv",
     'json_empricalCompounds': "_empCpd_json.json",
     # for annotation
-    'check_isotope_ratio': True,
+    'check_isotope_ratio': False,
 
 
     # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
     # 'max_rtime': 300,                   # retention time range (chromatography) in seconds, to auto populate
     # 'prominence_window': 101,           # not used now; no need to modify  
     # 'cache_mass_traces': False,         # to save memory if not using DB; turn on if need to plot and diagnose
     # 'init_samples_number': 3,           # initiation samples,
```

### Comparing `asari-metabolomics-1.9.7/asari/experiment.py` & `asari-metabolomics-1.9.8/asari/experiment.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,17 @@
         Reference databases can be pre-loaded.
         With db_mass_calibrate to theoretical values, 
         '''
         self.load_annotation_db()
         self.db_mass_calibrate()
 
         EED = ExperimentalEcpdDatabase(mode=self.mode, mz_tolerance_ppm=self.mz_tolerance_ppm)
-        EED.build_from_list_peaks(self.CMAP.FeatureList, mz_tolerance_ppm=self.mz_tolerance_ppm, check_isotope_ratio=self.check_isotope_ratio)
+        EED.build_from_list_peaks(
+            self.CMAP.FeatureList, mz_tolerance_ppm=self.mz_tolerance_ppm, check_isotope_ratio=self.check_isotope_ratio
+            )
         EED.extend_empCpd_annotation(self.KCD)
         EED.annotate_singletons(self.KCD)       
         # EED.dict_empCpds misses some features 
         EED.dict_empCpds = self.append_orphans_to_epmCpds(EED.dict_empCpds)
 
         self.export_peak_annotation(EED.dict_empCpds, self.KCD, 'Feature_annotation')
```

### Comparing `asari-metabolomics-1.9.7/asari/json_encoder.py` & `asari-metabolomics-1.9.8/asari/json_encoder.py`

 * *Files identical despite different names*

### Comparing `asari-metabolomics-1.9.7/asari/main.py` & `asari-metabolomics-1.9.8/asari/main.py`

 * *Files identical despite different names*

### Comparing `asari-metabolomics-1.9.7/asari/mass_functions.py` & `asari-metabolomics-1.9.8/asari/mass_functions.py`

 * *Files identical despite different names*

### Comparing `asari-metabolomics-1.9.7/asari/mongo.py` & `asari-metabolomics-1.9.8/asari/mongo.py`

 * *Files identical despite different names*

### Comparing `asari-metabolomics-1.9.7/asari/peaks.py` & `asari-metabolomics-1.9.8/asari/peaks.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     min_peak_height = parameters['min_peak_height']
     min_prominence_threshold = parameters['min_prominence_threshold']
     min_fwhm = round( 0.5 * parameters['min_timepoints'] )
     snr = parameters['signal_noise_ratio']
     peakshape = parameters['gaussian_shape']
     reverse_detection = parameters['reverse_detection']
     wlen = 101                          # if used, this limits peak evaluation 50 scans to the left and 50 to right
-    min_prominence_ratio = 0.1
+    min_prominence_ratio = 0.05
     iteration = True                    # a 2nd round of peak detection if enough remaining datapoints
     for mass_track in list_mass_tracks:
         if mass_track['intensity'].max() > min_peak_height:
             iters.append(
                 (mass_track, number_of_scans, min_peak_height, min_fwhm, min_prominence_threshold,
                 wlen, snr, peakshape, min_prominence_ratio, iteration, reverse_detection, 
                 shared_list)
@@ -116,15 +116,17 @@
         else:
             ROIs.append(tmp)
             tmp = [ii]
 
     ROIs.append(tmp)
     ROIs = [r for r in ROIs if len(r) >= min_fwhm * 2]
     _do_smoothing = True                # noisy mass track
-    if list_intensity.max() > 100 * min_peak_height and len(__selected_scans__) < 0.5 * number_of_scans:
+    if __baseline__ < min_peak_height \
+        and list_intensity.max() > 100 * min_peak_height \
+            and len(__selected_scans__) < 0.5 * number_of_scans:
         _do_smoothing = False           # clean mass track 
 
     # min_prominence_ratio * list_intensity_roi.max() is not good because high noise will suppress peaks
     prominence = max(min_prominence_threshold, snr*__baseline__)
     for R in ROIs:
         if len(R) < 3 * min_fwhm:       # extend if too short - help narrow peaks
             R = extend_ROI(R, number_of_scans)
```

### Comparing `asari-metabolomics-1.9.7/asari/samples.py` & `asari-metabolomics-1.9.8/asari/samples.py`

 * *Files identical despite different names*

### Comparing `asari-metabolomics-1.9.7/asari/tools/extract_masstracks.py` & `asari-metabolomics-1.9.8/asari/tools/extract_masstracks.py`

 * *Files identical despite different names*

### Comparing `asari-metabolomics-1.9.7/asari/tools/merge.py` & `asari-metabolomics-1.9.8/asari/tools/merge.py`

 * *Files identical despite different names*

### Comparing `asari-metabolomics-1.9.7/asari/tools/plot.py` & `asari-metabolomics-1.9.8/asari/tools/plot.py`

 * *Files identical despite different names*

### Comparing `asari-metabolomics-1.9.7/asari/workflow.py` & `asari-metabolomics-1.9.8/asari/workflow.py`

 * *Files identical despite different names*

### Comparing `asari-metabolomics-1.9.7/asari_metabolomics.egg-info/PKG-INFO` & `asari-metabolomics-1.9.8/asari_metabolomics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asari-metabolomics
-Version: 1.9.7
+Version: 1.9.8
 Summary: LC-MS metabolomics data preprocessing
 Home-page: https://github.com/shuzhao-li/asari
 Author: Shuzhao Li
 Author-email: shuzhao.li@gmail.com
 License: BSD 3-Clause
 Keywords: metabolomics bioinformatics mass spectrometry
 Classifier: Intended Audience :: Developers
```

### Comparing `asari-metabolomics-1.9.7/asari_metabolomics.egg-info/SOURCES.txt` & `asari-metabolomics-1.9.8/asari_metabolomics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `asari-metabolomics-1.9.7/setup.py` & `asari-metabolomics-1.9.8/setup.py`

 * *Files identical despite different names*

