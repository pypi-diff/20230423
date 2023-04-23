# Comparing `tmp/flarespy-0.9.0.tar.gz` & `tmp/flarespy-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flarespy-0.9.0.tar", max compression
+gzip compressed data, was "flarespy-0.9.1.tar", max compression
```

## Comparing `flarespy-0.9.0.tar` & `flarespy-0.9.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2022-09-03 06:20:05.854812 flarespy-0.9.0/LICENSE
--rw-r--r--   0        0        0      428 2023-04-23 16:46:40.327394 flarespy-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     3036 2023-02-03 08:53:00.981401 flarespy-0.9.0/src/flarespy/Flare_model.py
--rw-r--r--   0        0        0      118 2022-09-03 06:20:05.855706 flarespy-0.9.0/src/flarespy/__init__.py
--rw-r--r--   0        0        0   569289 2023-03-30 09:22:45.813451 flarespy-0.9.0/src/flarespy/data/model.dat
--rw-r--r--   0        0        0    31530 2023-04-23 16:44:16.842476 flarespy-0.9.0/src/flarespy/flarefinder.py
--rw-r--r--   0        0        0     7016 2023-04-23 16:22:07.776473 flarespy-0.9.0/src/flarespy/utils.py
--rw-r--r--   0        0        0       22 2023-04-23 16:46:40.330247 flarespy-0.9.0/src/flarespy/version.py
--rw-r--r--   0        0        0      726 1970-01-01 00:00:00.000000 flarespy-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-09-03 06:20:05.854812 flarespy-0.9.1/LICENSE
+-rw-r--r--   0        0        0      428 2023-04-23 17:08:09.188427 flarespy-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     3036 2023-02-03 08:53:00.981401 flarespy-0.9.1/src/flarespy/Flare_model.py
+-rw-r--r--   0        0        0      118 2022-09-03 06:20:05.855706 flarespy-0.9.1/src/flarespy/__init__.py
+-rw-r--r--   0        0        0   569289 2023-03-30 09:22:45.813451 flarespy-0.9.1/src/flarespy/data/model.dat
+-rw-r--r--   0        0        0    31636 2023-04-23 17:07:01.712469 flarespy-0.9.1/src/flarespy/flarefinder.py
+-rw-r--r--   0        0        0     7016 2023-04-23 16:22:07.776473 flarespy-0.9.1/src/flarespy/utils.py
+-rw-r--r--   0        0        0       22 2023-04-23 17:08:09.193086 flarespy-0.9.1/src/flarespy/version.py
+-rw-r--r--   0        0        0      726 1970-01-01 00:00:00.000000 flarespy-0.9.1/PKG-INFO
```

### Comparing `flarespy-0.9.0/LICENSE` & `flarespy-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flarespy-0.9.0/src/flarespy/Flare_model.py` & `flarespy-0.9.1/src/flarespy/Flare_model.py`

 * *Files identical despite different names*

### Comparing `flarespy-0.9.0/src/flarespy/data/model.dat` & `flarespy-0.9.1/src/flarespy/data/model.dat`

 * *Files identical despite different names*

### Comparing `flarespy-0.9.0/src/flarespy/flarefinder.py` & `flarespy-0.9.1/src/flarespy/flarefinder.py`

 * *Files 1% similar despite different names*

```diff
@@ -529,43 +529,45 @@
         flare probability, signal-to-noise ratio (SNR), amplitude, duration, equivalent duration
         (ED), and energy. The calculated parameters are added to the candidates DataFrame.
         """
 
         if self.candidate_parameters is not None:
             snr_array = np.zeros(len(self.candidate_parameters))
             for row in self.candidate_parameters.itertuples():
-                candidate = self[row.i_start: row.i_stop + 1].remove_nans("standardized_flux")
+                candidate = self[row.i_start : row.i_stop + 1].remove_nans("standardized_flux")
                 flux = candidate.standardized_flux.value
                 snr_array[row.Index] = round(np.max(flux), 2)
             self.candidate_parameters["snr"] = snr_array
 
             if validate:
                 self._calculate_prob()
 
-            if not self.meta["ZERO_CENTERED"]:
-                amp = np.zeros(len(self.candidate_parameters))
-                dur = np.zeros(len(self.candidate_parameters))
-                ed = np.zeros(len(self.candidate_parameters))
-
-                n_row = 0
-                for row in self.candidate_parameters.itertuples():
-                    time = self.time.value[row.i_start : row.i_stop + 1]
-                    flux = self.detrended_flux[row.i_start : row.i_stop + 1]
-                    amp[n_row] = np.nanmax(flux) - 1
-                    dur[n_row] = (time[-1] - time[0]) * 1440
-                    mask = np.isnan(flux)
-                    ed[n_row] = np.trapz(flux[~mask] - 1, x=time[~mask] * 86400)
-                    n_row += 1
+            amp = np.zeros(len(self.candidate_parameters))
+            dur = np.zeros(len(self.candidate_parameters))
+            ed = np.zeros(len(self.candidate_parameters))
+
+            for row in self.candidate_parameters.itertuples():
+                time = self.time.value[row.i_start : row.i_stop + 1]
+                flux = self.detrended_flux[row.i_start : row.i_stop + 1]
+                dur[row.Index] = (time[-1] - time[0]) * 1440
+                if not self.meta["ZERO_CENTERED"]:
+                    amp[row.Index] = np.nanmax(flux) - 1
+                    ed[row.Index] = np.trapz(flux[~np.isnan(flux)] - 1, x=time[~np.isnan(flux)] * 86400)
 
+            self.candidate_parameters["dur"] = np.round(dur, 1)
+
+            if not self.meta["ZERO_CENTERED"]:
                 self.candidate_parameters["amp"] = np.round(amp, 3)
-                self.candidate_parameters["dur"] = np.round(dur, 1)
                 self.candidate_parameters["ed"] = np.round(ed, 2)
-
                 if calculate_energy:
                     self._calculate_energy(ed)
+            else:
+                self.candidate_parameters["amp"] = np.nan
+                self.candidate_parameters["ed"] = np.nan
+                self.candidate_parameters["energy"] = np.nan
 
     def _calculate_prob(self):
         proba_array = np.zeros(len(self.candidate_parameters))
         for row in self.candidate_parameters.itertuples():
             candidate = self[row.i_start : row.i_stop + 1].remove_nans("standardized_flux")
             time = candidate.time.value
             flux = candidate.standardized_flux.value
@@ -581,15 +583,15 @@
         if self.stellar_parameters is None:
             self._query_gaia_dr3()
             self._query_tic()
 
         stellar_lum = calculate_stellar_luminosity(self.stellar_parameters.Tmag, self.stellar_parameters.Plx)
 
         if np.isnan(stellar_lum):
-            self.candidate_parameters["energy"] = np.full(len(self.candidate_parameters), np.nan)
+            self.candidate_parameters["energy"] = np.nan
         else:
             energy = ed * stellar_lum
             self.candidate_parameters["energy"] = [np.format_float_scientific(x, precision=2) for x in energy]
 
     # Main pipeline function -------------------------------------------------------------------------------------------
     def find_flares(self, exclude_cv=True, detect_sso=True, validate=True, calculate_energy=True):
         """
```

### Comparing `flarespy-0.9.0/src/flarespy/utils.py` & `flarespy-0.9.1/src/flarespy/utils.py`

 * *Files identical despite different names*

### Comparing `flarespy-0.9.0/PKG-INFO` & `flarespy-0.9.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flarespy
-Version: 0.9.0
+Version: 0.9.1
 Summary: Find flares in TESS light curves
 Home-page: https://github.com/keyuxing/flarespy
 License: MIT
 Author: Keyu Xing
 Author-email: kyxing@mail.bnu.edu.cn
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
```

