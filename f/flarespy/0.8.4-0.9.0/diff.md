# Comparing `tmp/flarespy-0.8.4.tar.gz` & `tmp/flarespy-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flarespy-0.8.4.tar", max compression
+gzip compressed data, was "flarespy-0.9.0.tar", max compression
```

## Comparing `flarespy-0.8.4.tar` & `flarespy-0.9.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2022-09-03 06:20:05.854812 flarespy-0.8.4/LICENSE
--rw-r--r--   0        0        0      428 2023-04-22 16:11:30.424936 flarespy-0.8.4/pyproject.toml
--rw-r--r--   0        0        0     3036 2023-02-03 08:53:00.981401 flarespy-0.8.4/src/flarespy/Flare_model.py
--rw-r--r--   0        0        0      118 2022-09-03 06:20:05.855706 flarespy-0.8.4/src/flarespy/__init__.py
--rw-r--r--   0        0        0   569289 2023-03-30 09:22:45.813451 flarespy-0.8.4/src/flarespy/data/model.dat
--rw-r--r--   0        0        0    29302 2023-04-22 16:09:52.872651 flarespy-0.8.4/src/flarespy/flarefinder.py
--rw-r--r--   0        0        0     7337 2023-04-22 03:01:00.209257 flarespy-0.8.4/src/flarespy/utils.py
--rw-r--r--   0        0        0       22 2023-04-22 16:11:30.422987 flarespy-0.8.4/src/flarespy/version.py
--rw-r--r--   0        0        0      726 1970-01-01 00:00:00.000000 flarespy-0.8.4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-09-03 06:20:05.854812 flarespy-0.9.0/LICENSE
+-rw-r--r--   0        0        0      428 2023-04-23 16:46:40.327394 flarespy-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     3036 2023-02-03 08:53:00.981401 flarespy-0.9.0/src/flarespy/Flare_model.py
+-rw-r--r--   0        0        0      118 2022-09-03 06:20:05.855706 flarespy-0.9.0/src/flarespy/__init__.py
+-rw-r--r--   0        0        0   569289 2023-03-30 09:22:45.813451 flarespy-0.9.0/src/flarespy/data/model.dat
+-rw-r--r--   0        0        0    31530 2023-04-23 16:44:16.842476 flarespy-0.9.0/src/flarespy/flarefinder.py
+-rw-r--r--   0        0        0     7016 2023-04-23 16:22:07.776473 flarespy-0.9.0/src/flarespy/utils.py
+-rw-r--r--   0        0        0       22 2023-04-23 16:46:40.330247 flarespy-0.9.0/src/flarespy/version.py
+-rw-r--r--   0        0        0      726 1970-01-01 00:00:00.000000 flarespy-0.9.0/PKG-INFO
```

### Comparing `flarespy-0.8.4/LICENSE` & `flarespy-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flarespy-0.8.4/src/flarespy/Flare_model.py` & `flarespy-0.9.0/src/flarespy/Flare_model.py`

 * *Files identical despite different names*

### Comparing `flarespy-0.8.4/src/flarespy/data/model.dat` & `flarespy-0.9.0/src/flarespy/data/model.dat`

 * *Files identical despite different names*

### Comparing `flarespy-0.8.4/src/flarespy/flarefinder.py` & `flarespy-0.9.0/src/flarespy/flarefinder.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,16 +13,14 @@
 from astroquery.simbad import Simbad
 from matplotlib import pyplot as plt
 from matplotlib.offsetbox import AnchoredText
 from matplotlib.ticker import MaxNLocator
 from wotan import flatten
 
 from .utils import (
-    CANDIDATES_COLUMNS,
-    STELLAR_PARAMETER_COLUMNS,
     calculate_stellar_luminosity,
     extend,
     fill_gaps,
     find_consecutive,
     get_flare_probability,
     query_gaia_dr3_id,
 )
@@ -61,119 +59,232 @@
     return flc
 
 
 class FlareLightCurve(lk.LightCurve):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.meta["stellar_parameters"] = None
-        self.meta["candidates"] = None
+        self.meta["candidate_parameters"] = None
 
-    def _generate_model(self):
+    # Data preprocessing -----------------------------------------------------------------------------------------------
+    def detrend(self, window_length=0.3, period_lower=0.05, period_upper=2):
         """
-        Generate a model for the light curve.
+        Detrend the light curve.
 
-        This method generates a model for the light curve by computing a percentile-based
-        representation of the flux values.
+        This method detrends the light curve by masking the eclipses, generating a model,
+        and applying a biweight filter to flatten the light curve. The detrended flux is
+        stored in a new column, and the standardized flux is calculated.
 
-        Returns
-        -------
-        model_flux : ndarray
-            The model flux values.
+        Parameters
+        ----------
+        window_length : float, optional
+            The window length (in days) for the detrending process. Default is 0.3.
+        """
+
+        self._calculate_period()
+        self._mask_eclipse()
+        if period_lower < self.period < period_upper:
+            model_flux = self._generate_model()
+        else:
+            model_flux = 0
+
+        masked_flux = self.flux.copy()
+        masked_flux[self.eclipse_mask] = np.nan
+        detrended_flux, trend_flux = flatten(
+            self.time.value,
+            masked_flux - model_flux,
+            method="biweight",
+            window_length=window_length,
+            return_trend=True,
+        )
+        trend_flux += model_flux
+        self.add_columns(
+            [detrended_flux * self.flux.unit, trend_flux * self.flux.unit],
+            names=["detrended_flux", "trend_flux"],
+        )
+        self._standardize()
+
+    def _calculate_period(self):
+        """
+        Calculate the period of the light curve.
+
+        This method calculates the period of the light curve by computing the periodogram
+        and finding the period with the highest power.
         """
 
         with warnings.catch_warnings():
             warnings.simplefilter("ignore", category=RuntimeWarning)
             pg = self.to_periodogram()
             period = pg.period_at_max_power.value
             snr = pg.max_power / np.nanmedian(pg.power)
 
             if period < 10 and snr > 5:
                 pg = self.to_periodogram(
                     minimum_period=max(period - 0.2, 0.01),
                     maximum_period=period + 0.2,
                     oversample_factor=1000,
                 )
-                period = pg.period_at_max_power.value
+                self.meta["PERIOD"] = pg.period_at_max_power.value
             else:
-                period = -999
-
-            self.meta["PERIOD"] = period
-
-        if 0.05 < period < 2:
-            period_array = np.array([1, 2, 4]) * period
-            std_array = np.zeros_like(period_array)
-            folded_lc_list = []
-            trend_folded_flux_list = []
-
-            for i, period in enumerate(period_array):
-                folded_lc = self.fold(period)
-                detrended_folded_flux, trend_folded_flux = flatten(
-                    folded_lc.time.value,
-                    folded_lc.flux,
-                    method="median",
-                    window_length=period / 50,
-                    return_trend=True,
-                )
-                std_array[i] = np.nanstd(detrended_folded_flux)
-                folded_lc_list.append(folded_lc)
-                trend_folded_flux_list.append(trend_folded_flux)
-
-            std_array *= 0.75 ** np.arange(len(period_array))[::-1]
-            index = std_array.argmin()
-            self.meta["PERIOD"] = period_array[index]
-            trend_folded_flux = trend_folded_flux_list[index]
-            folded_lc = folded_lc_list[index]
-
-            return trend_folded_flux[folded_lc.time_original.argsort()] - 1
-        return 0
+                self.meta["PERIOD"] = np.nan
 
     def _mask_eclipse(self):
         """
         Mask the eclipses in the light curve.
 
         This method masks the eclipses present in the light curve by setting the corresponding
         flux values to NaN (Not a Number).
         """
 
         with warnings.catch_warnings():
             warnings.simplefilter("ignore", category=AstropyUserWarning)
-
             sigma = mad_std(self.flux, ignore_nan=True)
-            eclipse_mask = self.flux < np.nanmedian(self.flux) - 3 * sigma
-            if hasattr(self.flux, "mask"):
-                eclipse_mask = np.logical_xor(eclipse_mask, self.flux.mask)
-
-            i_start_array, i_stop_array = find_consecutive(
-                np.nonzero(eclipse_mask)[0],
-                3,
-                gap=1.2 * self.meta["TIMEDEL"],
-                data=self.time.value,
+
+        mask = np.nonzero(self.flux < np.nanmedian(self.flux) - 3 * sigma)[0]
+        start_indexes, stop_indexes = find_consecutive(
+            indexes=mask,
+            n_consecutive=3,
+            gap=1.2 * self.meta["TIMEDEL"],
+            data=self.time.value,
+        )
+
+        eclipse_mask = np.zeros_like(self.time.value, dtype=bool)
+        if start_indexes.size > 3 and self.time.value[start_indexes[0]] < self.time.value[stop_indexes[-1]] - 10:
+            for i, (start_index, stop_index) in enumerate(zip(start_indexes, stop_indexes)):
+                t_start = self.time.value[start_index]
+                t_stop = self.time.value[stop_index]
+                t_start_ext, t_stop_ext = extend(
+                    self.time.value,
+                    (self.flux - 1) / sigma,
+                    t_start,
+                    t_stop,
+                    t_stop - t_start,
+                    n_sigma=0,
+                    mode=-1,
+                )
+                eclipse_mask[(self.time.value >= t_start_ext) & (self.time.value <= t_stop_ext)] = True
+
+        self.meta["eclipse_mask"] = eclipse_mask
+
+    def _generate_model(self):
+        """
+        Generate a model for the short-term periodic variations of the light curve.
+
+        Returns
+        -------
+        model_flux : ndarray
+            The model flux values.
+        """
+
+        period_array = np.array([1, 2, 4]) * self.period
+        std_array = np.zeros_like(period_array)
+        folded_lc_list = []
+        trend_folded_flux_list = []
+
+        for i, period in enumerate(period_array):
+            folded_lc = self.fold(period)
+            detrended_folded_flux, trend_folded_flux = flatten(
+                folded_lc.time.value,
+                folded_lc.flux,
+                method="median",
+                window_length=period / 50,
+                return_trend=True,
             )
+            std_array[i] = np.nanstd(detrended_folded_flux)
+            folded_lc_list.append(folded_lc)
+            trend_folded_flux_list.append(trend_folded_flux)
+
+        std_array *= 0.75 ** np.arange(len(period_array))[::-1]
+        index = std_array.argmin()
+        self.meta["PERIOD"] = period_array[index]
+        trend_folded_flux = trend_folded_flux_list[index]
+        folded_lc = folded_lc_list[index]
+
+        return trend_folded_flux[folded_lc.time_original.argsort()] - 1
+
+    def _standardize(self):
+        """
+        Standardize the detrended light curve.
+
+        This method standardizes the detrended light curve by dividing the difference between the
+        flux and 1 by the rolling standard deviation. It then adds the rolling standard deviation
+        and the standardized flux as new columns to the class.
+        """
+
+        flux_series = pd.Series(self.detrended_flux.value, index=pd.DatetimeIndex(self.time.datetime))
+
+        rolling_window = flux_series.rolling(pd.Timedelta(2, unit="d"), center=True)
+        rolling_std = rolling_window.apply(mad_std, kwargs={"ignore_nan": True})
+        rolling_std[np.isnan(self.detrended_flux.value)] = np.nan
 
-            lc = self.copy()
-            if i_start_array is not None:
-                if i_start_array.size > 3 and lc.time.value[i_start_array[0]] < lc.time.value[i_stop_array[-1]] - 10:
-                    for i in range(i_start_array.size):
-                        t_start = self.time.value[i_start_array[i]]
-                        t_stop = self.time.value[i_stop_array[i]]
-                        duration = t_stop - t_start
-                        t_start_ext, t_stop_ext = extend(
-                            lc.time.value,
-                            (lc.flux - 1) / sigma,
-                            t_start,
-                            t_stop,
-                            duration,
-                            n_sigma=0,
-                            mode=-1,
-                        )
-                        lc.flux[(self.time.value >= t_start_ext) & (self.time.value <= t_stop_ext)] = np.nan
+        standardized_flux = (self.detrended_flux.value - 1) / rolling_std
+
+        self.add_columns([rolling_std, standardized_flux], names=["rolling_std", "standardized_flux"])
+
+    # Candidate identification -----------------------------------------------------------------------------------------
+    def find_candidates(self, n_sigma: float = 3, n_consecutive: int = 2):
+        """
+        Find the candidates of flares.
+
+        This method identifies potential flare candidates in the detrended light curve.
+        It searches for outliers above a certain threshold and groups them into
+        consecutive events. The method then filters out candidates at the edge of the
+        light curve and stores the candidate information in a DataFrame.
+
+        Parameters
+        ----------
+        n_sigma : float, optional
+            The threshold for identifying flare candidates as a multiple of the standard deviation.
+            Default is 3.
+        n_consecutive : int, optional
+            The minimum number of consecutive data points above the threshold to be considered a
+            candidate. Default is 2.
 
-            self.meta["eclipse_mask"] = np.isnan(lc.flux)
+        This method identifies potential flare candidates in the standardized light curve using
+        the specified threshold and number of consecutive data points.
+        """
+
+        outlier_mask = np.nonzero(self.standardized_flux > n_sigma)[0]
+        start_indexes, stop_indexes = find_consecutive(
+            outlier_mask,
+            n_consecutive,
+            gap=1.2 * self.meta["TIMEDEL"],
+            data=self.time.value,
+        )
 
-        return lc
+        if start_indexes.size:
+            start_ext_indexes, stop_ext_indexes = self._extend_multiple_events(start_indexes, stop_indexes)
+
+            at_edge = np.zeros_like(start_ext_indexes, dtype=bool)
+            for i in range(at_edge.size):
+                at_edge[i] = self._is_at_edge(start_ext_indexes[i], stop_ext_indexes[i])
+
+            if not at_edge.all():
+                start_ext_indexes = start_ext_indexes[~at_edge]
+                stop_ext_indexes = stop_ext_indexes[~at_edge]
+
+                peak_indexes = np.copy(start_ext_indexes)
+                for i in range(start_ext_indexes.size):
+                    i_peak = self.standardized_flux[start_ext_indexes[i] : stop_ext_indexes[i] + 1].argmax()
+                    peak_indexes[i] += i_peak
+
+                self.candidate_parameters = pd.DataFrame(
+                    {
+                        "i_start": start_ext_indexes,
+                        "i_peak": peak_indexes,
+                        "i_stop": stop_ext_indexes,
+                        "t_start": np.round(self.time.value[start_ext_indexes], 7),
+                        "t_peak": np.round(self.time.value[peak_indexes], 7),
+                        "t_stop": np.round(self.time.value[stop_ext_indexes], 7),
+                    }
+                )
+        else:
+            self.candidate_parameters = pd.DataFrame(
+                columns=["i_start", "i_peak", "i_stop", "t_start", "t_peak", "t_stop"]
+            )
 
     def _extend_multiple_events(self, start_indexes, stop_indexes, max_extend_indexes=45):
         start_ext_indexes = np.zeros_like(start_indexes)
         stop_ext_indexes = np.zeros_like(stop_indexes)
 
         lc = self.copy()
         lc.flux[self.eclipse_mask] = np.nan
@@ -196,39 +307,65 @@
 
             start_ext_indexes[i] = np.nonzero(self.time.value == t_start_ext)[0][0]
             stop_ext_indexes[i] = np.nonzero(self.time.value == t_stop_ext)[0][0]
 
         overlap_indexes = np.nonzero(start_ext_indexes[1:] <= stop_ext_indexes[:-1])[0] + 1
         overlap_start, overlap_stop = find_consecutive(overlap_indexes, 1)
 
-        if overlap_start is not None:
+        if overlap_start.size:
             stop_ext_indexes[overlap_start - 1] = stop_ext_indexes[overlap_stop]
             start_ext_indexes = np.delete(start_ext_indexes, overlap_indexes)
             stop_ext_indexes = np.delete(stop_ext_indexes, overlap_indexes)
 
         return start_ext_indexes, stop_ext_indexes
 
-    def _standardize(self):
+    def _is_at_edge(self, i_start: int, i_stop: int, window: float = 0.1):
         """
-        Standardize the detrended light curve.
+        Check if a candidate is at the edge of a segment of the light curve.
 
-        This method standardizes the detrended light curve by dividing the difference between the
-        flux and 1 by the rolling standard deviation. It then adds the rolling standard deviation
-        and the standardized flux as new columns to the class.
+        Parameters
+        ----------
+        i_start : int
+            The start index of the candidate in the light curve.
+        i_stop : int
+            The stop index of the candidate in the light curve.
+        window : float, optional
+            The time window (in days) used to check if the candidate is at the edge. Default is 0.1.
+
+        Returns
+        -------
+        bool
+            False if the candidate is not at the edge of a segment of the light curve, True otherwise.
         """
 
-        flux_series = pd.Series(self.detrended_flux.value, index=pd.DatetimeIndex(self.time.datetime))
+        time = self.time[np.isfinite(self.standardized_flux)].value
+        t_start = self.time.value[i_start]
+        t_stop = self.time.value[i_stop]
 
-        rolling_window = flux_series.rolling(pd.Timedelta(2, unit="d"), center=True)
-        rolling_std = rolling_window.apply(mad_std, kwargs={"ignore_nan": True})
-        rolling_std[np.isnan(self.detrended_flux.value)] = np.nan
+        before = np.nonzero((time > t_start - window) & (time < t_start))[0]
+        after = np.nonzero((time > t_stop) & (time < t_stop + window))[0]
 
-        standardized_flux = (self.detrended_flux.value - 1) / rolling_std
+        return False if (before.size and after.size) else True
 
-        self.add_columns([rolling_std, standardized_flux], names=["rolling_std", "standardized_flux"])
+    # Solar System Objects (SSOs) checks -------------------------------------------------------------------------------
+    def detect_sso(self):
+        """
+        Detect if the candidates are caused by SSO encounters.
+
+        This method checks if the flare candidates identified in the light curve are caused by
+        encounters with Solar System Objects (SSOs). It adds a boolean array to the candidates
+        DataFrame indicating whether a candidate is caused by an SSO encounter or not.
+        """
+
+        if self.candidate_parameters is not None:
+            sso = np.zeros(len(self.candidate_parameters), dtype=bool)
+            for row in self.candidate_parameters.itertuples():
+                sso[row.Index] = self._is_sso(row.i_peak)
+
+            self.candidate_parameters["sso"] = sso
 
     def _is_sso(self, i_peak: int, radius: float = 8):
         """
         Check if a candidate is caused by a Solar System Object (SSO) encounter.
 
         Parameters
         ----------
@@ -280,299 +417,225 @@
                 except KeyError:
                     ap_mag[row.Index] = eph["Tmag"].value
             if (ap_mag < 19).any():
                 return True
 
         return False
 
-    def _is_at_edge(self, i_start: int, i_stop: int, window: float = 0.1):
-        """
-        Check if a candidate is at the edge of a segment of the light curve.
-
-        Parameters
-        ----------
-        i_start : int
-            The start index of the candidate in the light curve.
-        i_stop : int
-            The stop index of the candidate in the light curve.
-        window : float, optional
-            The time window (in days) used to check if the candidate is at the edge. Default is 0.1.
-
-        Returns
-        -------
-        bool
-            False if the candidate is not at the edge of a segment of the light curve, True otherwise.
-        """
-
-        time = self.time[np.isfinite(self.standardized_flux)].value
-        t_start = self.time.value[i_start]
-        t_stop = self.time.value[i_stop]
-
-        before = np.nonzero((time > t_start - window) & (time < t_start))[0]
-        after = np.nonzero((time > t_stop) & (time < t_stop + window))[0]
-
-        return False if (before.size and after.size) else True
-
+    # Stellar parameters and object info -------------------------------------------------------------------------------
     def query_stellar_parameters(self):
         """
         Query the stellar parameters of the target star.
 
         This method queries various stellar parameters of the target star, such as parallax,
         Gmag, BP-RP, Tmag, and contamination ratio, from Gaia DR3, TIC, and SIMBAD databases.
         It also checks if the target star has an excluded object type.
         """
 
-        self.stellar_parameters = pd.Series(index=STELLAR_PARAMETER_COLUMNS, dtype=object)
+        self._query_basic_info()
+        self._query_object_type()
+        self._query_gaia_dr3()
+        self._query_tic()
 
+    def _query_basic_info(self):
         gaia_dr3_id = query_gaia_dr3_id(self.ticid)
-        self.stellar_parameters.gaia_dr3_source_id = gaia_dr3_id
-        self.stellar_parameters.obs_duration = np.round(
-            self.meta["TIMEDEL"] * np.nonzero(~np.isnan(self.flux.value))[0].size, 4
+        obs_duration = np.round(self.meta["TIMEDEL"] * np.nonzero(~np.isnan(self.flux.value))[0].size, 4)
+
+        self.stellar_parameters = pd.Series(
+            index=[
+                "gaia_dr3_source_id",
+                "obj_type",
+                "Plx",
+                "Gmag",
+                "BP-RP",
+                "Tmag",
+                "cont_ratio",
+                "obs_duration",
+            ],
+            dtype=object,
         )
 
-        # Query parallax, Gmag and BP-RP from Gaia DR3
-        if isinstance(gaia_dr3_id, str):
-            result = VIZIER.query_constraints("I/355/gaiadr3", Source=gaia_dr3_id)[0]
-            plx = result["Plx"].data.data[0]
-            if plx > 0:
-                self.stellar_parameters["Plx"] = np.round(plx, 4)
-            self.stellar_parameters["Gmag"] = np.round(result["Gmag"].data.data[0], 4)
-            self.stellar_parameters["BP-RP"] = np.round(result["BP-RP"].data.data[0], 4)
+        self.stellar_parameters.gaia_dr3_source_id = gaia_dr3_id
+        self.stellar_parameters.obs_duration = obs_duration
 
-        # Query Tmag and contamination ratio from TIC
-        tic_data = Catalogs.query_object(self.label, radius=0.02, catalog="TIC")
-        tic_data.add_index("ID")
-        try:
-            target_row = tic_data.loc[str(self.ticid)]
-            self.stellar_parameters.Tmag = target_row["Tmag"]
-            self.stellar_parameters.cont_ratio = np.round(target_row["contratio"], 4)
-        except KeyError:
-            pass
+    def _query_object_type(self):
+        """
+        Query object info from SIMBAD
+        """
 
-        # Query object info from SIMBAD
         query_result = None
         with warnings.catch_warnings():
             warnings.simplefilter("error", category=UserWarning)
             try:
                 query_result = CUSTOM_SIMBAD.query_object(self.label)
             except TableParseError:
+                if self.stellar_parameters is None:
+                    self._query_basic_info()
                 gaia_dr3_id = self.stellar_parameters.gaia_dr3_source_id
+
                 if isinstance(gaia_dr3_id, str):
                     try:
                         query_result = CUSTOM_SIMBAD.query_object(f"Gaia DR3 {gaia_dr3_id}")
                     except TableParseError:
                         pass
 
-        self.meta["exclude"] = False
+        self.meta["EXCLUDE"] = False
         if query_result is None:
-            self.stellar_parameters.obj_type = np.nan
+            self.stellar_parameters["obj_type"] = np.nan
         else:
             obj_type = query_result["OTYPE"][0]
+            obj_type_list = query_result["OTYPES"][0].split("|")
             self.stellar_parameters.obj_type = obj_type
 
-            if obj_type in EXCLUDED_OTYPES or "CV*" in obj_type.split("|"):
-                self.meta["exclude"] = True
-
-    def detrend(self, window_length=0.3):
-        """
-        Detrend the light curve.
-
-        This method detrends the light curve by masking the eclipses, generating a model,
-        and applying a biweight filter to flatten the light curve. The detrended flux is
-        stored in a new column, and the standardized flux is calculated.
-
-        Parameters
-        ----------
-        window_length : float, optional
-            The window length (in days) for the detrending process. Default is 0.3.
-
-        This method detrends the light curve by removing systematic trends using a rolling
-        window approach. It then standardizes the detrended light curve.
-        """
-
-        masked_lc = self._mask_eclipse()
-        model_flux = self._generate_model()
-        detrended_flux, trend_flux = flatten(
-            self.time.value,
-            masked_lc.flux - model_flux,
-            method="biweight",
-            window_length=window_length,
-            return_trend=True,
-        )
-        trend_flux += model_flux
-        self.add_columns(
-            [detrended_flux * self.flux.unit, trend_flux * self.flux.unit],
-            names=["detrended_flux", "trend_flux"],
-        )
-        self._standardize()
+            if obj_type in EXCLUDED_OTYPES or "CV*" in obj_type_list:
+                self.meta["EXCLUDE"] = True
 
-    def find_candidates(self, n_sigma: float = 3, n_consecutive: int = 2):
+    def _query_gaia_dr3(self):
         """
-        Find the candidates of flares.
-
-        This method identifies potential flare candidates in the detrended light curve.
-        It searches for outliers above a certain threshold and groups them into
-        consecutive events. The method then filters out candidates at the edge of the
-        light curve and stores the candidate information in a DataFrame.
-
-        Parameters
-        ----------
-        n_sigma : float, optional
-            The threshold for identifying flare candidates as a multiple of the standard deviation.
-            Default is 3.
-        n_consecutive : int, optional
-            The minimum number of consecutive data points above the threshold to be considered a
-            candidate. Default is 2.
-
-        This method identifies potential flare candidates in the standardized light curve using
-        the specified threshold and number of consecutive data points.
+        Query parallax, Gmag and BP-RP from Gaia DR3
         """
 
-        self.stellar_parameters.gaia_dr3_source_id = query_gaia_dr3_id(self.ticid)
-        self.stellar_parameters.obs_duration = np.round(
-            self.meta["TIMEDEL"] * np.nonzero(~np.isnan(self.flux.value))[0].size, 4
-        )
-
-        if not self.exclude:
-            i_outliers = np.nonzero(self.standardized_flux > n_sigma)[0]
-
-            i_start_array, i_stop_array = find_consecutive(
-                i_outliers,
-                n_consecutive,
-                gap=1.2 * self.meta["TIMEDEL"],
-                data=self.time.value,
-            )
-
-            if i_start_array is not None:
-                i_start_ext_array, i_stop_ext_array = self._extend_multiple_events(i_start_array, i_stop_array)
+        if self.stellar_parameters is None:
+            self._query_basic_info()
+        gaia_dr3_id = self.stellar_parameters.gaia_dr3_source_id
 
-                at_edge = np.zeros_like(i_start_ext_array, dtype=bool)
-                for i in range(at_edge.size):
-                    at_edge[i] = self._is_at_edge(i_start_ext_array[i], i_stop_ext_array[i])
-
-                if not at_edge.all():
-                    i_start_ext_array = i_start_ext_array[~at_edge]
-                    i_stop_ext_array = i_stop_ext_array[~at_edge]
-
-                    i_peak_array = np.copy(i_start_ext_array)
-                    for i in range(i_start_ext_array.size):
-                        i_peak = self.standardized_flux[i_start_ext_array[i] : i_stop_ext_array[i] + 1].argmax()
-                        i_peak_array[i] += i_peak
-
-                    self.candidates = pd.DataFrame(columns=CANDIDATES_COLUMNS)
-                    self.candidates.i_start = i_start_ext_array
-                    self.candidates.i_peak = i_peak_array
-                    self.candidates.i_stop = i_stop_ext_array
-                    self.candidates.t_start = np.round(self.time.value[i_start_ext_array], 7)
-                    self.candidates.t_peak = np.round(self.time.value[i_peak_array], 7)
-                    self.candidates.t_stop = np.round(self.time.value[i_stop_ext_array], 7)
+        if isinstance(gaia_dr3_id, str):
+            result = VIZIER.query_constraints("I/355/gaiadr3", Source=gaia_dr3_id)[0]
+            plx = result["Plx"].data.data[0]
+            if plx > 0:
+                self.stellar_parameters["Plx"] = np.round(plx, 4)
+            self.stellar_parameters["Gmag"] = np.round(result["Gmag"].data.data[0], 4)
+            self.stellar_parameters["BP-RP"] = np.round(result["BP-RP"].data.data[0], 4)
 
-    def detect_sso(self):
+    def _query_tic(self):
         """
-        Detect if the candidates are caused by SSO encounters.
-
-        This method checks if the flare candidates identified in the light curve are caused by
-        encounters with Solar System Objects (SSOs). It adds a boolean array to the candidates
-        DataFrame indicating whether a candidate is caused by an SSO encounter or not.
+        Query Tmag and contamination ratio from TIC
         """
 
-        if self.candidates is not None:
-            sso = np.zeros(len(self.candidates), dtype=bool)
-            for row in self.candidates.itertuples():
-                sso[row.Index] = self._is_sso(row.i_peak)
-
-            self.candidates.sso = sso
+        tic_data = Catalogs.query_object(self.label, radius=0.02, catalog="TIC")
+        tic_data.add_index("ID")
+        try:
+            target_row = tic_data.loc[str(self.ticid)]
+            self.stellar_parameters["Tmag"] = target_row["Tmag"]
+            self.stellar_parameters["cont_ratio"] = np.round(target_row["contratio"], 4)
+        except KeyError:
+            pass
 
-    def calculate_candidate_parameters(self):
+    # Candidate parameter calculations ---------------------------------------------------------------------------------
+    def calculate_candidate_parameters(self, validate=True, calculate_energy=True):
         """
         Calculate the parameters of the candidates.
 
         This method calculates various parameters for the identified flare candidates, such as
         flare probability, signal-to-noise ratio (SNR), amplitude, duration, equivalent duration
         (ED), and energy. The calculated parameters are added to the candidates DataFrame.
         """
 
-        if self.candidates is not None:
-            proba_array = np.zeros(len(self.candidates))
-            snr_array = np.zeros(len(self.candidates))
-            for row in self.candidates.itertuples():
-                lc_candidate = self[row.i_start : row.i_stop + 1].remove_nans("standardized_flux")
-                time = lc_candidate.time.value
-                flux = lc_candidate.standardized_flux.value
-
-                if not (np.diff(lc_candidate.cadenceno) == 1).all():
-                    time, flux = fill_gaps(time, flux, lc_candidate.cadenceno)
-
-                if flux.size >= 4:
-                    proba_array[row.Index] = round(get_flare_probability(time, flux), 3)
+        if self.candidate_parameters is not None:
+            snr_array = np.zeros(len(self.candidate_parameters))
+            for row in self.candidate_parameters.itertuples():
+                candidate = self[row.i_start: row.i_stop + 1].remove_nans("standardized_flux")
+                flux = candidate.standardized_flux.value
                 snr_array[row.Index] = round(np.max(flux), 2)
+            self.candidate_parameters["snr"] = snr_array
 
-            self.candidates.flare_prob = proba_array
-            self.candidates.snr = snr_array
+            if validate:
+                self._calculate_prob()
 
             if not self.meta["ZERO_CENTERED"]:
-                if self.stellar_parameters is None:
-                    self.query_stellar_parameters()
-
-                amp = np.zeros(len(self.candidates))
-                dur = np.zeros(len(self.candidates))
-                ed = np.zeros(len(self.candidates))
-                stellar_lum = calculate_stellar_luminosity(self.stellar_parameters.Tmag, self.stellar_parameters.Plx)
+                amp = np.zeros(len(self.candidate_parameters))
+                dur = np.zeros(len(self.candidate_parameters))
+                ed = np.zeros(len(self.candidate_parameters))
 
                 n_row = 0
-                for row in self.candidates.itertuples():
+                for row in self.candidate_parameters.itertuples():
                     time = self.time.value[row.i_start : row.i_stop + 1]
                     flux = self.detrended_flux[row.i_start : row.i_stop + 1]
                     amp[n_row] = np.nanmax(flux) - 1
                     dur[n_row] = (time[-1] - time[0]) * 1440
                     mask = np.isnan(flux)
                     ed[n_row] = np.trapz(flux[~mask] - 1, x=time[~mask] * 86400)
                     n_row += 1
 
-                self.candidates.amp = np.round(amp, 3)
-                self.candidates.dur = np.round(dur, 1)
-                self.candidates.ed = np.round(ed, 2)
-                if np.isnan(stellar_lum):
-                    self.candidates.energy = np.full(len(self.candidates), np.nan)
-                else:
-                    energy = ed * stellar_lum
-                    self.candidates.energy = [np.format_float_scientific(x, precision=2) for x in energy]
+                self.candidate_parameters["amp"] = np.round(amp, 3)
+                self.candidate_parameters["dur"] = np.round(dur, 1)
+                self.candidate_parameters["ed"] = np.round(ed, 2)
+
+                if calculate_energy:
+                    self._calculate_energy(ed)
+
+    def _calculate_prob(self):
+        proba_array = np.zeros(len(self.candidate_parameters))
+        for row in self.candidate_parameters.itertuples():
+            candidate = self[row.i_start : row.i_stop + 1].remove_nans("standardized_flux")
+            time = candidate.time.value
+            flux = candidate.standardized_flux.value
+
+            if not (np.diff(candidate.cadenceno) == 1).all():
+                time, flux = fill_gaps(time, flux, candidate.cadenceno)
+
+            if flux.size >= 4:
+                proba_array[row.Index] = round(get_flare_probability(time, flux), 3)
+        self.candidate_parameters["flare_prob"] = proba_array
+
+    def _calculate_energy(self, ed):
+        if self.stellar_parameters is None:
+            self._query_gaia_dr3()
+            self._query_tic()
+
+        stellar_lum = calculate_stellar_luminosity(self.stellar_parameters.Tmag, self.stellar_parameters.Plx)
+
+        if np.isnan(stellar_lum):
+            self.candidate_parameters["energy"] = np.full(len(self.candidate_parameters), np.nan)
+        else:
+            energy = ed * stellar_lum
+            self.candidate_parameters["energy"] = [np.format_float_scientific(x, precision=2) for x in energy]
 
-    def find_flares(self):
+    # Main pipeline function -------------------------------------------------------------------------------------------
+    def find_flares(self, exclude_cv=True, detect_sso=True, validate=True, calculate_energy=True):
         """
         Find flares in the light curve.
 
         This method performs a series of steps to identify flares in the light curve. It queries
         the stellar parameters of the target star, detrends the light curve, finds the flare
         candidates, detects if the candidates are caused by SSO encounters, and calculates the
         candidate parameters. The results are stored in the class attributes.
         """
 
-        self.query_stellar_parameters()
-        self.detrend()
-        self.find_candidates()
-        self.detect_sso()
-        self.calculate_candidate_parameters()
+        if exclude_cv:
+            self._query_object_type()
+        else:
+            self.meta["EXCLUDE"] = False
+
+        if not self.meta["EXCLUDE"]:
+            self.detrend()
+            self.find_candidates()
+
+            if detect_sso:
+                self.detect_sso()
+
+            self.calculate_candidate_parameters(validate, calculate_energy)
 
+    # Plotting functions -----------------------------------------------------------------------------------------------
     def plot_candidates(self, figure_folder, threshold=0.5):
         """Plot the candidates."""
 
-        if self.candidates is not None:
+        if self.candidate_parameters is not None:
             t_extend = 30.2 * self.meta["TIMEDEL"]
             finite_mask = np.isfinite(self.standardized_flux)
 
-            self.candidates.loc[self.candidates.sso, "flare_prob"] = -999
+            self.candidate_parameters.loc[self.candidate_parameters.sso, "flare_prob"] = -999
             cond_list = [
-                self.candidates.flare_prob >= threshold,
-                self.candidates.flare_prob == -999,
+                self.candidate_parameters.flare_prob >= threshold,
+                self.candidate_parameters.flare_prob == -999,
             ]
             candidate_type_array = np.select(cond_list, ["flare", "sso"], "non-flare")
             color_array = np.select(cond_list, ["tab:red", "tab:orange"], "tab:gray")
             with plt.style.context(lk.MPLSTYLE):
-                for row in self.candidates.itertuples():
+                for row in self.candidate_parameters.itertuples():
                     candidate_type = candidate_type_array[row.Index]
                     color = color_array[row.Index]
                     figure_subfolder = figure_folder / candidate_type
                     figure_subfolder.mkdir(exist_ok=True)
 
                     fig = plt.figure(figsize=(14, 4))
 
@@ -594,15 +657,15 @@
                     ax_original_lc.set_ylabel("")
                     ax_original_lc.set_xticklabels([])
 
                     ax_detrended_lc = fig.add_subplot(223)
                     self.scatter(ax=ax_detrended_lc, column="detrended_flux", label="")
                     ax_detrended_lc.plot(self.time.value, 1 + 3 * self.rolling_std, lw=1, c="tab:gray")
 
-                    for element in self.candidates.itertuples():
+                    for element in self.candidate_parameters.itertuples():
                         alpha = 0.8 if row.Index == element.Index else 0.3
 
                         event_flux = self.detrended_flux[slice(element.i_start, element.i_stop + 1)]
                         extra_fill_region = (np.nanmax(event_flux) - np.nanmin(event_flux)) / 20
                         fill_lower_lim = np.nanmin(event_flux) - extra_fill_region
                         fill_upper_lim = np.nanmax(event_flux) + extra_fill_region
```

### Comparing `flarespy-0.8.4/src/flarespy/utils.py` & `flarespy-0.9.0/src/flarespy/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,41 +20,14 @@
     RFC_MODEL = joblib.load(MODEL_PATH)
 
 CUSTOM_SIMBAD = Simbad()
 CUSTOM_SIMBAD.add_votable_fields("ids")
 
 Gaia.MAIN_GAIA_TABLE = "gaiadr3.gaia_source"
 
-CANDIDATES_COLUMNS = [
-    "i_start",
-    "i_peak",
-    "i_stop",
-    "t_start",
-    "t_peak",
-    "t_stop",
-    "sso",
-    "flare_prob",
-    "snr",
-    "amp",
-    "dur",
-    "ed",
-    "energy",
-]
-
-STELLAR_PARAMETER_COLUMNS = [
-    "gaia_dr3_source_id",
-    "obj_type",
-    "Plx",
-    "Gmag",
-    "BP-RP",
-    "Tmag",
-    "cont_ratio",
-    "obs_duration",
-]
-
 # Zero point TESS flux (from Sullivan 2017)
 TESS_FLUX0 = 4.03e-6 * u.erg / u.s / u.cm**2
 
 
 def extract_features(x):
     abs_energy = np.dot(x, x)
     first_location_of_maximum = np.argmax(x) / len(x)
@@ -154,15 +127,15 @@
     grouped_consecutive_data = [x for x in grouped_data if x.size >= n_consecutive]
 
     if grouped_consecutive_data:
         i_start_array = np.array([x[0] for x in grouped_consecutive_data], dtype=int)
         i_stop_array = np.array([x[-1] for x in grouped_consecutive_data], dtype=int)
         return i_start_array, i_stop_array
     else:
-        return None, None
+        return np.array([], dtype=int), np.array([], dtype=int)
 
 
 def fill_gaps(time, flux, cadenceno):
     """Fill gaps in the data by interpolation."""
 
     newdata = {}
```

### Comparing `flarespy-0.8.4/PKG-INFO` & `flarespy-0.9.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flarespy
-Version: 0.8.4
+Version: 0.9.0
 Summary: Find flares in TESS light curves
 Home-page: https://github.com/keyuxing/flarespy
 License: MIT
 Author: Keyu Xing
 Author-email: kyxing@mail.bnu.edu.cn
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
```

