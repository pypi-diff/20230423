# Comparing `tmp/npyx-2.8.1.tar.gz` & `tmp/npyx-2.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "npyx-2.8.1.tar", last modified: Thu Apr 20 20:54:46 2023, max compression
+gzip compressed data, was "npyx-2.8.2.tar", last modified: Sun Apr 23 14:38:55 2023, max compression
```

## Comparing `npyx-2.8.1.tar` & `npyx-2.8.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-20 20:54:46.522986 npyx-2.8.1/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    35149 2022-11-30 14:14:46.000000 npyx-2.8.1/LICENSE.md
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    32083 2023-04-20 20:54:46.522986 npyx-2.8.1/PKG-INFO
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    31591 2023-03-28 09:45:46.000000 npyx-2.8.1/README.md
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-20 20:54:46.522986 npyx-2.8.1/npyx/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      789 2023-04-20 20:19:00.000000 npyx-2.8.1/npyx/__init__.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)   142298 2023-03-06 16:29:02.000000 npyx-2.8.1/npyx/behav.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    55561 2023-03-01 11:06:59.000000 npyx-2.8.1/npyx/circuitProphyler.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)   106738 2023-04-20 20:31:09.000000 npyx-2.8.1/npyx/corr.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    28838 2023-04-20 18:33:44.000000 npyx-2.8.1/npyx/datasets.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    56712 2023-04-20 20:40:50.000000 npyx-2.8.1/npyx/feat.py
--rwxrwxr-x   0 maxime    (1000) maxime    (1000)    17109 2023-04-20 18:33:44.000000 npyx-2.8.1/npyx/gl.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    38180 2023-04-20 19:53:38.000000 npyx-2.8.1/npyx/h5.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)        0 2022-11-30 14:14:47.000000 npyx-2.8.1/npyx/histo.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    16050 2022-11-30 14:14:47.000000 npyx-2.8.1/npyx/info.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    49232 2023-04-14 12:13:22.000000 npyx-2.8.1/npyx/inout.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    12770 2023-03-01 11:06:59.000000 npyx-2.8.1/npyx/merger.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    37349 2023-03-20 15:37:11.000000 npyx-2.8.1/npyx/metrics.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     4936 2023-04-20 18:33:44.000000 npyx-2.8.1/npyx/ml.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    16904 2023-03-01 11:06:59.000000 npyx-2.8.1/npyx/model.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)   149739 2023-04-20 20:19:11.000000 npyx-2.8.1/npyx/plot.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    38393 2023-03-01 11:06:59.000000 npyx-2.8.1/npyx/preprocess.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    40183 2023-04-20 20:36:25.000000 npyx-2.8.1/npyx/spk_t.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    47559 2023-04-20 18:33:44.000000 npyx-2.8.1/npyx/spk_wvf.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    14661 2023-03-01 11:06:59.000000 npyx-2.8.1/npyx/stats.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     3415 2023-03-01 11:06:59.000000 npyx-2.8.1/npyx/testing.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    65528 2023-03-24 11:24:27.000000 npyx-2.8.1/npyx/utils.py
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-20 20:54:46.522986 npyx-2.8.1/npyx.egg-info/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    32083 2023-04-20 20:54:46.000000 npyx-2.8.1/npyx.egg-info/PKG-INFO
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      492 2023-04-20 20:54:46.000000 npyx-2.8.1/npyx.egg-info/SOURCES.txt
--rw-rw-r--   0 maxime    (1000) maxime    (1000)        1 2023-04-20 20:54:46.000000 npyx-2.8.1/npyx.egg-info/dependency_links.txt
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      143 2023-04-20 20:54:46.000000 npyx-2.8.1/npyx.egg-info/requires.txt
--rw-rw-r--   0 maxime    (1000) maxime    (1000)        5 2023-04-20 20:54:46.000000 npyx-2.8.1/npyx.egg-info/top_level.txt
--rw-rw-r--   0 maxime    (1000) maxime    (1000)       38 2023-04-20 20:54:46.522986 npyx-2.8.1/setup.cfg
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     1491 2023-04-14 12:19:49.000000 npyx-2.8.1/setup.py
+drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-23 14:38:55.154370 npyx-2.8.2/
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    35149 2022-11-30 14:14:46.000000 npyx-2.8.2/LICENSE.md
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    32083 2023-04-23 14:38:55.154370 npyx-2.8.2/PKG-INFO
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    31591 2023-03-28 09:45:46.000000 npyx-2.8.2/README.md
+drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-23 14:38:55.154370 npyx-2.8.2/npyx/
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      789 2023-04-23 14:38:20.000000 npyx-2.8.2/npyx/__init__.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)   142298 2023-03-06 16:29:02.000000 npyx-2.8.2/npyx/behav.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    55561 2023-03-01 11:06:59.000000 npyx-2.8.2/npyx/circuitProphyler.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)   106738 2023-04-20 20:31:09.000000 npyx-2.8.2/npyx/corr.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    28838 2023-04-20 18:33:44.000000 npyx-2.8.2/npyx/datasets.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    56712 2023-04-20 20:40:50.000000 npyx-2.8.2/npyx/feat.py
+-rwxrwxr-x   0 maxime    (1000) maxime    (1000)    17109 2023-04-20 18:33:44.000000 npyx-2.8.2/npyx/gl.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    38180 2023-04-20 19:53:38.000000 npyx-2.8.2/npyx/h5.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)        0 2022-11-30 14:14:47.000000 npyx-2.8.2/npyx/histo.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    16050 2022-11-30 14:14:47.000000 npyx-2.8.2/npyx/info.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    49232 2023-04-14 12:13:22.000000 npyx-2.8.2/npyx/inout.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    12770 2023-03-01 11:06:59.000000 npyx-2.8.2/npyx/merger.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    37349 2023-03-20 15:37:11.000000 npyx-2.8.2/npyx/metrics.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     4936 2023-04-20 18:33:44.000000 npyx-2.8.2/npyx/ml.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    16904 2023-03-01 11:06:59.000000 npyx-2.8.2/npyx/model.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)   149739 2023-04-20 20:19:11.000000 npyx-2.8.2/npyx/plot.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    38393 2023-03-01 11:06:59.000000 npyx-2.8.2/npyx/preprocess.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    40231 2023-04-23 14:37:23.000000 npyx-2.8.2/npyx/spk_t.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    47559 2023-04-20 18:33:44.000000 npyx-2.8.2/npyx/spk_wvf.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    14661 2023-03-01 11:06:59.000000 npyx-2.8.2/npyx/stats.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     3415 2023-03-01 11:06:59.000000 npyx-2.8.2/npyx/testing.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    65528 2023-03-24 11:24:27.000000 npyx-2.8.2/npyx/utils.py
+drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-23 14:38:55.154370 npyx-2.8.2/npyx.egg-info/
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    32083 2023-04-23 14:38:55.000000 npyx-2.8.2/npyx.egg-info/PKG-INFO
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      492 2023-04-23 14:38:55.000000 npyx-2.8.2/npyx.egg-info/SOURCES.txt
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)        1 2023-04-23 14:38:55.000000 npyx-2.8.2/npyx.egg-info/dependency_links.txt
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      143 2023-04-23 14:38:55.000000 npyx-2.8.2/npyx.egg-info/requires.txt
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)        5 2023-04-23 14:38:55.000000 npyx-2.8.2/npyx.egg-info/top_level.txt
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)       38 2023-04-23 14:38:55.154370 npyx-2.8.2/setup.cfg
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     1491 2023-04-14 12:19:49.000000 npyx-2.8.2/setup.py
```

### Comparing `npyx-2.8.1/LICENSE.md` & `npyx-2.8.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `npyx-2.8.1/PKG-INFO` & `npyx-2.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npyx
-Version: 2.8.1
+Version: 2.8.2
 Summary: Python routines dealing with Neuropixels data.
 Home-page: https://github.com/Npix-routines/NeuroPyxels
 Author: Maxime Beau
 Author-email: maximebeaujeanroch047@gmail.com
 Keywords: neuropixels,kilosort,phy,data analysis,electrophysiology,neuroscience
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `npyx-2.8.1/README.md` & `npyx-2.8.2/README.md`

 * *Files identical despite different names*

### Comparing `npyx-2.8.1/npyx/__init__.py` & `npyx-2.8.2/npyx/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,10 +36,10 @@
  .behav
  .merger
  .circuitProphyler
  .feat
  .h5
 """
 
-__version__ = "2.8.1"
+__version__ = "2.8.2"
 
 print(f"npyx version {__version__} imported.")
```

### Comparing `npyx-2.8.1/npyx/behav.py` & `npyx-2.8.2/npyx/behav.py`

 * *Files identical despite different names*

### Comparing `npyx-2.8.1/npyx/circuitProphyler.py` & `npyx-2.8.2/npyx/circuitProphyler.py`

 * *Files identical despite different names*

### Comparing `npyx-2.8.1/npyx/corr.py` & `npyx-2.8.2/npyx/corr.py`

 * *Files identical despite different names*

### Comparing `npyx-2.8.1/npyx/datasets.py` & `npyx-2.8.2/npyx/datasets.py`

 * *Files identical despite different names*

### Comparing `npyx-2.8.1/npyx/feat.py` & `npyx-2.8.2/npyx/feat.py`

 * *Files identical despite different names*

### Comparing `npyx-2.8.1/npyx/gl.py` & `npyx-2.8.2/npyx/gl.py`

 * *Files identical despite different names*

### Comparing `npyx-2.8.1/npyx/h5.py` & `npyx-2.8.2/npyx/h5.py`

 * *Files identical despite different names*

### Comparing `npyx-2.8.1/npyx/info.py` & `npyx-2.8.2/npyx/info.py`

 * *Files identical despite different names*

### Comparing `npyx-2.8.1/npyx/inout.py` & `npyx-2.8.2/npyx/inout.py`

 * *Files identical despite different names*

### Comparing `npyx-2.8.1/npyx/merger.py` & `npyx-2.8.2/npyx/merger.py`

 * *Files identical despite different names*

### Comparing `npyx-2.8.1/npyx/metrics.py` & `npyx-2.8.2/npyx/metrics.py`

 * *Files identical despite different names*

### Comparing `npyx-2.8.1/npyx/ml.py` & `npyx-2.8.2/npyx/ml.py`

 * *Files identical despite different names*

### Comparing `npyx-2.8.1/npyx/model.py` & `npyx-2.8.2/npyx/model.py`

 * *Files identical despite different names*

### Comparing `npyx-2.8.1/npyx/plot.py` & `npyx-2.8.2/npyx/plot.py`

 * *Files identical despite different names*

### Comparing `npyx-2.8.1/npyx/preprocess.py` & `npyx-2.8.2/npyx/preprocess.py`

 * *Files identical despite different names*

### Comparing `npyx-2.8.1/npyx/spk_t.py` & `npyx-2.8.2/npyx/spk_t.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         indices = np.nonzero(spike_clusters==unit)[0].ravel()
 
         # Save it
         if sav:
             np.save(dpnm/fn, indices)
             
     # Optional selection of spies without duplicates
-    dp_source = get_source_dp_u(dp, unit)[0]
+    dp_source = npyx.merger.get_source_dp_u(dp, unit)[0]
     fs=read_metadata(dp_source)["highpass"]['sampling_rate']
     train = trn(dp, unit, again=again, enforced_rp=-1)
     duplicates_m = duplicates_mask(train, enforced_rp, fs)
     train = train[~duplicates_m]
     indices = indices[~duplicates_m]
 
     # Optional selection of a section of the recording.
@@ -124,15 +124,15 @@
     - again: boolean, if True recomputes data from source files without checking routines memory.
     - enforced_rp: float, enforced refractory period (ms)- if 2 spikes are separated by less than enforced_rp ms, the first one only is kept.
                    By default 0, only removed pure duplicates (they happen!).
     '''
 
     # Search if the variable is already saved in dp/routinesMemory
     dpnm = get_npyx_memory(dp)
-    dp_source = get_source_dp_u(dp, unit)[0]
+    dp_source = npyx.merger.get_source_dp_u(dp, unit)[0]
     fs=read_metadata(dp_source)['highpass']['sampling_rate']
 
     fn=f'trn{unit}_{enforced_rp}+.npy'
     if (dpnm/fn).exists() and not again:
         if verbose: print("File {} found in routines memory.".format(fn))
         try: train = np.load(dpnm/fn) # handling of weird allow_picke=True error
         except: pass
@@ -245,15 +245,15 @@
         assert train.ndim==1
         return mean_firing_rate(train, exclusion_quantile, fs)
 
     U=npa([U]).flatten()
     MFR=[]
     for u in U:
         t=trn(dp, u, periods=periods, again=again, enforced_rp=enforced_rp)
-        dp_source = get_source_dp_u(dp, u)[0]
+        dp_source = npyx.merger.get_source_dp_u(dp, u)[0]
         fs=read_metadata(dp_source)['highpass']['sampling_rate']
         MFR.append(mean_firing_rate(t, exclusion_quantile, fs))
 
     return MFR[0] if len(U)==1 else npa(MFR)
 
 def binarize(X, bin_size, fs, rec_len=None):
     '''Function to turn a spike train (array of time stamps)
@@ -290,15 +290,15 @@
     computes binarized spike train (1, Nspikes) - int64, in samples
     ********
 
     - dp (string): DataPath to the Neuropixels dataset.
     - u (int): unit index
     - bin_size: size of binarized spike train bins, in milliseconds.
     '''
-    dp_source = get_source_dp_u(dp, u)[0]
+    dp_source = npyx.merger.get_source_dp_u(dp, u)[0]
     fs=read_metadata(dp_source)['highpass']['sampling_rate']
     assert b>=1000/fs
     t = trn(dp, u, enforced_rp=1, periods=periods, again=again)
     t_end = np.load(Path(dp,'spike_times.npy'), mmap_mode='r').ravel()[-1]
     return binarize(t, b, fs, t_end)
 
 def get_firing_periods(dp, u, b=1, sd=1000, th=0.02, again=False, train=None, fs=None, t_end=None):
```

### Comparing `npyx-2.8.1/npyx/spk_wvf.py` & `npyx-2.8.2/npyx/spk_wvf.py`

 * *Files identical despite different names*

### Comparing `npyx-2.8.1/npyx/stats.py` & `npyx-2.8.2/npyx/stats.py`

 * *Files identical despite different names*

### Comparing `npyx-2.8.1/npyx/testing.py` & `npyx-2.8.2/npyx/testing.py`

 * *Files identical despite different names*

### Comparing `npyx-2.8.1/npyx/utils.py` & `npyx-2.8.2/npyx/utils.py`

 * *Files identical despite different names*

### Comparing `npyx-2.8.1/npyx.egg-info/PKG-INFO` & `npyx-2.8.2/npyx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npyx
-Version: 2.8.1
+Version: 2.8.2
 Summary: Python routines dealing with Neuropixels data.
 Home-page: https://github.com/Npix-routines/NeuroPyxels
 Author: Maxime Beau
 Author-email: maximebeaujeanroch047@gmail.com
 Keywords: neuropixels,kilosort,phy,data analysis,electrophysiology,neuroscience
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `npyx-2.8.1/setup.py` & `npyx-2.8.2/setup.py`

 * *Files identical despite different names*

