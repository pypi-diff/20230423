# Comparing `tmp/pheno-utils-0.1.4.tar.gz` & `tmp/pheno-utils-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pheno-utils-0.1.4.tar", last modified: Thu Apr 20 20:23:44 2023, max compression
+gzip compressed data, was "pheno-utils-0.1.5.tar", last modified: Sun Apr 23 11:10:52 2023, max compression
```

## Comparing `pheno-utils-0.1.4.tar` & `pheno-utils-0.1.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-20 20:23:44.902229 pheno-utils-0.1.4/
--rw-r--r--   0 alondmnt   (501) staff       (20)    11357 2023-04-06 20:07:34.000000 pheno-utils-0.1.4/LICENSE
--rw-r--r--   0 alondmnt   (501) staff       (20)      111 2023-04-06 20:07:42.000000 pheno-utils-0.1.4/MANIFEST.in
--rw-r--r--   0 alondmnt   (501) staff       (20)     1479 2023-04-20 20:23:44.901822 pheno-utils-0.1.4/PKG-INFO
--rw-r--r--   0 alondmnt   (501) staff       (20)      446 2023-04-06 20:07:47.000000 pheno-utils-0.1.4/README.md
-drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-20 20:23:44.894069 pheno-utils-0.1.4/pheno_utils/
--rw-r--r--   0 alondmnt   (501) staff       (20)       22 2023-04-20 20:16:55.000000 pheno-utils-0.1.4/pheno_utils/__init__.py
--rw-r--r--   0 alondmnt   (501) staff       (20)    13667 2023-04-20 20:16:56.000000 pheno-utils-0.1.4/pheno_utils/_modidx.py
--rw-r--r--   0 alondmnt   (501) staff       (20)    16963 2023-04-20 20:16:55.000000 pheno-utils-0.1.4/pheno_utils/age_reference_plots.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     5111 2023-04-20 20:16:55.000000 pheno-utils-0.1.4/pheno_utils/basic_analysis.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     2789 2023-04-20 20:16:55.000000 pheno-utils-0.1.4/pheno_utils/basic_plots.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     2517 2023-04-20 20:16:55.000000 pheno-utils-0.1.4/pheno_utils/blandaltman_plots.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     7865 2023-04-20 20:16:55.000000 pheno-utils-0.1.4/pheno_utils/cgm_plots.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     3414 2023-04-20 20:16:55.000000 pheno-utils-0.1.4/pheno_utils/config.py
--rw-r--r--   0 alondmnt   (501) staff       (20)    16326 2023-04-20 20:16:55.000000 pheno-utils-0.1.4/pheno_utils/data_loader.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     2825 2023-04-20 20:16:55.000000 pheno-utils-0.1.4/pheno_utils/dates_plots.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     2113 2023-04-20 20:16:55.000000 pheno-utils-0.1.4/pheno_utils/ecg_analysis.py
--rw-r--r--   0 alondmnt   (501) staff       (20)    13210 2023-04-20 20:16:55.000000 pheno-utils-0.1.4/pheno_utils/sleep_plots.py
-drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-20 20:23:44.901224 pheno-utils-0.1.4/pheno_utils.egg-info/
--rw-r--r--   0 alondmnt   (501) staff       (20)     1479 2023-04-20 20:23:44.000000 pheno-utils-0.1.4/pheno_utils.egg-info/PKG-INFO
--rw-r--r--   0 alondmnt   (501) staff       (20)      625 2023-04-20 20:23:44.000000 pheno-utils-0.1.4/pheno_utils.egg-info/SOURCES.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)        1 2023-04-20 20:23:44.000000 pheno-utils-0.1.4/pheno_utils.egg-info/dependency_links.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)       65 2023-04-20 20:23:44.000000 pheno-utils-0.1.4/pheno_utils.egg-info/entry_points.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)        1 2023-04-06 08:56:36.000000 pheno-utils-0.1.4/pheno_utils.egg-info/not-zip-safe
--rw-r--r--   0 alondmnt   (501) staff       (20)      127 2023-04-20 20:23:44.000000 pheno-utils-0.1.4/pheno_utils.egg-info/requires.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)       12 2023-04-20 20:23:44.000000 pheno-utils-0.1.4/pheno_utils.egg-info/top_level.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)     1068 2023-04-20 20:11:29.000000 pheno-utils-0.1.4/settings.ini
--rw-r--r--   0 alondmnt   (501) staff       (20)       38 2023-04-20 20:23:44.902415 pheno-utils-0.1.4/setup.cfg
--rw-r--r--   0 alondmnt   (501) staff       (20)     2560 2023-04-06 20:07:57.000000 pheno-utils-0.1.4/setup.py
+drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-23 11:10:52.387734 pheno-utils-0.1.5/
+-rw-r--r--   0 alondmnt   (501) staff       (20)    11357 2023-04-06 20:07:34.000000 pheno-utils-0.1.5/LICENSE
+-rw-r--r--   0 alondmnt   (501) staff       (20)      111 2023-04-06 20:07:42.000000 pheno-utils-0.1.5/MANIFEST.in
+-rw-r--r--   0 alondmnt   (501) staff       (20)     1479 2023-04-23 11:10:52.387368 pheno-utils-0.1.5/PKG-INFO
+-rw-r--r--   0 alondmnt   (501) staff       (20)      446 2023-04-06 20:07:47.000000 pheno-utils-0.1.5/README.md
+drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-23 11:10:52.381982 pheno-utils-0.1.5/pheno_utils/
+-rw-r--r--   0 alondmnt   (501) staff       (20)      328 2023-04-23 11:10:17.000000 pheno-utils-0.1.5/pheno_utils/__init__.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)    13667 2023-04-23 11:10:17.000000 pheno-utils-0.1.5/pheno_utils/_modidx.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)    16963 2023-04-23 11:10:17.000000 pheno-utils-0.1.5/pheno_utils/age_reference_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     5111 2023-04-23 11:10:17.000000 pheno-utils-0.1.5/pheno_utils/basic_analysis.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2789 2023-04-23 11:10:17.000000 pheno-utils-0.1.5/pheno_utils/basic_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2517 2023-04-23 11:10:17.000000 pheno-utils-0.1.5/pheno_utils/blandaltman_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     7865 2023-04-23 11:10:17.000000 pheno-utils-0.1.5/pheno_utils/cgm_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     3441 2023-04-23 11:10:17.000000 pheno-utils-0.1.5/pheno_utils/config.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)    16321 2023-04-23 11:10:17.000000 pheno-utils-0.1.5/pheno_utils/data_loader.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2825 2023-04-23 11:10:17.000000 pheno-utils-0.1.5/pheno_utils/dates_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2113 2023-04-23 11:10:17.000000 pheno-utils-0.1.5/pheno_utils/ecg_analysis.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)    13210 2023-04-23 11:10:17.000000 pheno-utils-0.1.5/pheno_utils/sleep_plots.py
+drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-23 11:10:52.386768 pheno-utils-0.1.5/pheno_utils.egg-info/
+-rw-r--r--   0 alondmnt   (501) staff       (20)     1479 2023-04-23 11:10:52.000000 pheno-utils-0.1.5/pheno_utils.egg-info/PKG-INFO
+-rw-r--r--   0 alondmnt   (501) staff       (20)      625 2023-04-23 11:10:52.000000 pheno-utils-0.1.5/pheno_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)        1 2023-04-23 11:10:52.000000 pheno-utils-0.1.5/pheno_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)       65 2023-04-23 11:10:52.000000 pheno-utils-0.1.5/pheno_utils.egg-info/entry_points.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)        1 2023-04-06 08:56:36.000000 pheno-utils-0.1.5/pheno_utils.egg-info/not-zip-safe
+-rw-r--r--   0 alondmnt   (501) staff       (20)      127 2023-04-23 11:10:52.000000 pheno-utils-0.1.5/pheno_utils.egg-info/requires.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)       12 2023-04-23 11:10:52.000000 pheno-utils-0.1.5/pheno_utils.egg-info/top_level.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)     1068 2023-04-23 11:08:21.000000 pheno-utils-0.1.5/settings.ini
+-rw-r--r--   0 alondmnt   (501) staff       (20)       38 2023-04-23 11:10:52.387885 pheno-utils-0.1.5/setup.cfg
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2560 2023-04-06 20:07:57.000000 pheno-utils-0.1.5/setup.py
```

### Comparing `pheno-utils-0.1.4/LICENSE` & `pheno-utils-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.4/PKG-INFO` & `pheno-utils-0.1.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pheno-utils
-Version: 0.1.4
+Version: 0.1.5
 Summary: Pheno data utils - viz, loaders, mergers
 Home-page: https://github.com/hrossman/pheno-utils
 Author: hrossman
 Author-email: hagairossman@gmail.com
 License: Apache Software License 2.0
 Description: pheno-utils
         ================
```

### Comparing `pheno-utils-0.1.4/pheno_utils/_modidx.py` & `pheno-utils-0.1.5/pheno_utils/_modidx.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.4/pheno_utils/age_reference_plots.py` & `pheno-utils-0.1.5/pheno_utils/age_reference_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.4/pheno_utils/basic_analysis.py` & `pheno-utils-0.1.5/pheno_utils/basic_analysis.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.4/pheno_utils/basic_plots.py` & `pheno-utils-0.1.5/pheno_utils/basic_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.4/pheno_utils/blandaltman_plots.py` & `pheno-utils-0.1.5/pheno_utils/blandaltman_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.4/pheno_utils/cgm_plots.py` & `pheno-utils-0.1.5/pheno_utils/cgm_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.4/pheno_utils/config.py` & `pheno-utils-0.1.5/pheno_utils/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 GLUC_COLOR = "C0"
 FOOD_COLOR = "C1"
 
 DATASETS_PATH = '/home/ec2-user/studies/hpp/'
 COHORT = '10k'
 POPULATION_DATASET = 'population'
-CONFIG_FILES = ['~/.pheno/config', '/efs/.pheno/config']
+CONFIG_FILES = ['.pheno/config', '~/.pheno/config', '/efs/.pheno/config']
 
 for cf in CONFIG_FILES:
     cf = os.path.expanduser(cf)
     if not os.path.isfile(cf):
         continue
     with open(cf, 'r') as f:
         for line in f:
@@ -34,14 +34,15 @@
                 DATASETS_PATH = line.split('=')[1].strip()
             elif line.startswith('POPULATION_DATASET'):
                 POPULATION_DATASET = line.split('=')[1].strip()
             elif line.startswith('COHORT'):
                 COHORT = line.split('=')[1].strip()
                 if (len(COHORT) == 0) or (COHORT == 'None'):
                     COHORT = None
+    break
 
 
 # %% ../nbs/00_config.ipynb 5
 def generate_synthetic_data(n: int = 1000) -> pd.DataFrame:
     """
     Generates a sample DataFrame containing age, gender, and value data.
```

### Comparing `pheno-utils-0.1.4/pheno_utils/data_loader.py` & `pheno-utils-0.1.5/pheno_utils/data_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,18 +216,18 @@
                 fields_in_col = np.unique([col for f in fields for col in df.columns if re.search(f, col)])
             else:
                 fields_in_col = df.columns.intersection(fields).difference(data.columns)
             if len(fields_in_col):
                 data = self.__concat__(data, df[fields_in_col])
 
             fields_in_index = np.setdiff1d(np.intersect1d(df.index.names, fields), data.columns)
-            if len(fields_in_index):
+            for field in fields_in_index:
                 data = self.__concat__(
                     data,
-                    pd.DataFrame(df.index.get_level_values(fields_in_index), index=df.index))
+                    pd.DataFrame(df.index.get_level_values(field), index=df.index))
 
         if len(data):
             data = data.loc[:, ~data.columns.duplicated()]
 
         not_found = np.setdiff1d(fields, data.columns)
         if len(not_found) and not flexible:
             if self.errors == 'raise':
```

### Comparing `pheno-utils-0.1.4/pheno_utils/dates_plots.py` & `pheno-utils-0.1.5/pheno_utils/dates_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.4/pheno_utils/ecg_analysis.py` & `pheno-utils-0.1.5/pheno_utils/ecg_analysis.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.4/pheno_utils/sleep_plots.py` & `pheno-utils-0.1.5/pheno_utils/sleep_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.4/pheno_utils.egg-info/PKG-INFO` & `pheno-utils-0.1.5/pheno_utils.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pheno-utils
-Version: 0.1.4
+Version: 0.1.5
 Summary: Pheno data utils - viz, loaders, mergers
 Home-page: https://github.com/hrossman/pheno-utils
 Author: hrossman
 Author-email: hagairossman@gmail.com
 License: Apache Software License 2.0
 Description: pheno-utils
         ================
```

### Comparing `pheno-utils-0.1.4/pheno_utils.egg-info/SOURCES.txt` & `pheno-utils-0.1.5/pheno_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.4/settings.ini` & `pheno-utils-0.1.5/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = pheno-utils
 lib_name = %(repo)s
-version = 0.1.4
+version = 0.1.5
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = pheno_utils
```

### Comparing `pheno-utils-0.1.4/setup.py` & `pheno-utils-0.1.5/setup.py`

 * *Files identical despite different names*

