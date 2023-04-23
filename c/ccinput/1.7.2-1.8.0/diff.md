# Comparing `tmp/ccinput-1.7.2.tar.gz` & `tmp/ccinput-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccinput-1.7.2.tar", last modified: Tue Mar 21 18:17:15 2023, max compression
+gzip compressed data, was "ccinput-1.8.0.tar", last modified: Sun Apr 23 15:50:23 2023, max compression
```

## Comparing `ccinput-1.7.2.tar` & `ccinput-1.8.0.tar`

### file list

```diff
@@ -1,46 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 18:17:15.289958 ccinput-1.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-03-21 18:16:52.000000 ccinput-1.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-21 18:16:52.000000 ccinput-1.7.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-03-21 18:17:15.289958 ccinput-1.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-03-21 18:16:52.000000 ccinput-1.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 18:17:15.293958 ccinput-1.7.2/ccinput/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-21 18:16:52.000000 ccinput-1.7.2/ccinput/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-21 18:17:15.293958 ccinput-1.7.2/ccinput/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    18388 2023-03-21 18:16:52.000000 ccinput-1.7.2/ccinput/calculation.py
--rw-r--r--   0 runner    (1001) docker     (123)    75068 2023-03-21 18:16:52.000000 ccinput-1.7.2/ccinput/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-03-21 18:16:52.000000 ccinput-1.7.2/ccinput/documentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 18:17:15.285958 ccinput-1.7.2/ccinput/drivers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 18:16:52.000000 ccinput-1.7.2/ccinput/drivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-03-21 18:16:52.000000 ccinput-1.7.2/ccinput/drivers/pysis.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-03-21 18:16:52.000000 ccinput-1.7.2/ccinput/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 18:17:15.289958 ccinput-1.7.2/ccinput/packages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 18:16:52.000000 ccinput-1.7.2/ccinput/packages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15455 2023-03-21 18:16:52.000000 ccinput-1.7.2/ccinput/packages/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-03-21 18:16:52.000000 ccinput-1.7.2/ccinput/packages/nwchem.py
--rw-r--r--   0 runner    (1001) docker     (123)    15963 2023-03-21 18:16:52.000000 ccinput-1.7.2/ccinput/packages/orca.py
--rw-r--r--   0 runner    (1001) docker     (123)    13127 2023-03-21 18:16:52.000000 ccinput-1.7.2/ccinput/packages/xtb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-03-21 18:16:52.000000 ccinput-1.7.2/ccinput/presets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 18:17:15.289958 ccinput-1.7.2/ccinput/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 18:16:52.000000 ccinput-1.7.2/ccinput/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12339 2023-03-21 18:16:52.000000 ccinput-1.7.2/ccinput/tests/test_calculation.py
--rw-r--r--   0 runner    (1001) docker     (123)    38742 2023-03-21 18:16:52.000000 ccinput-1.7.2/ccinput/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)   111131 2023-03-21 18:16:52.000000 ccinput-1.7.2/ccinput/tests/test_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)    57036 2023-03-21 18:16:52.000000 ccinput-1.7.2/ccinput/tests/test_orca.py
--rw-r--r--   0 runner    (1001) docker     (123)    13218 2023-03-21 18:16:52.000000 ccinput-1.7.2/ccinput/tests/test_pysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-03-21 18:16:52.000000 ccinput-1.7.2/ccinput/tests/test_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)    22171 2023-03-21 18:16:52.000000 ccinput-1.7.2/ccinput/tests/test_xtb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-03-21 18:16:52.000000 ccinput-1.7.2/ccinput/tests/testing_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    13061 2023-03-21 18:16:52.000000 ccinput-1.7.2/ccinput/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    14984 2023-03-21 18:16:52.000000 ccinput-1.7.2/ccinput/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 18:17:15.285958 ccinput-1.7.2/ccinput.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-03-21 18:17:15.000000 ccinput-1.7.2/ccinput.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-03-21 18:17:15.000000 ccinput-1.7.2/ccinput.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 18:17:15.000000 ccinput-1.7.2/ccinput.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-21 18:17:15.000000 ccinput-1.7.2/ccinput.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 18:17:15.000000 ccinput-1.7.2/ccinput.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-21 18:17:15.000000 ccinput-1.7.2/ccinput.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-21 18:17:15.000000 ccinput-1.7.2/ccinput.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-03-21 18:16:52.000000 ccinput-1.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-03-21 18:17:15.289958 ccinput-1.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-03-21 18:16:52.000000 ccinput-1.7.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-03-21 18:16:52.000000 ccinput-1.7.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:50:23.621481 ccinput-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-23 15:49:46.000000 ccinput-1.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-23 15:49:46.000000 ccinput-1.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-04-23 15:50:23.621481 ccinput-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-04-23 15:49:46.000000 ccinput-1.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:50:23.621481 ccinput-1.8.0/ccinput/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-23 15:49:46.000000 ccinput-1.8.0/ccinput/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-23 15:50:23.621481 ccinput-1.8.0/ccinput/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18388 2023-04-23 15:49:46.000000 ccinput-1.8.0/ccinput/calculation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76266 2023-04-23 15:49:46.000000 ccinput-1.8.0/ccinput/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-23 15:49:46.000000 ccinput-1.8.0/ccinput/documentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:50:23.621481 ccinput-1.8.0/ccinput/drivers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 15:49:46.000000 ccinput-1.8.0/ccinput/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-04-23 15:49:46.000000 ccinput-1.8.0/ccinput/drivers/pysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-23 15:49:46.000000 ccinput-1.8.0/ccinput/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:50:23.621481 ccinput-1.8.0/ccinput/packages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 15:49:46.000000 ccinput-1.8.0/ccinput/packages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15455 2023-04-23 15:49:46.000000 ccinput-1.8.0/ccinput/packages/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-04-23 15:49:46.000000 ccinput-1.8.0/ccinput/packages/nwchem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15963 2023-04-23 15:49:46.000000 ccinput-1.8.0/ccinput/packages/orca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-04-23 15:49:46.000000 ccinput-1.8.0/ccinput/packages/psi4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9286 2023-04-23 15:49:46.000000 ccinput-1.8.0/ccinput/packages/qchem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13127 2023-04-23 15:49:46.000000 ccinput-1.8.0/ccinput/packages/xtb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-04-23 15:49:46.000000 ccinput-1.8.0/ccinput/presets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:50:23.621481 ccinput-1.8.0/ccinput/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 15:49:46.000000 ccinput-1.8.0/ccinput/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12339 2023-04-23 15:49:46.000000 ccinput-1.8.0/ccinput/tests/test_calculation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38742 2023-04-23 15:49:46.000000 ccinput-1.8.0/ccinput/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)   111131 2023-04-23 15:49:46.000000 ccinput-1.8.0/ccinput/tests/test_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57036 2023-04-23 15:49:46.000000 ccinput-1.8.0/ccinput/tests/test_orca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-23 15:49:46.000000 ccinput-1.8.0/ccinput/tests/test_psi4.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13218 2023-04-23 15:49:46.000000 ccinput-1.8.0/ccinput/tests/test_pysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47385 2023-04-23 15:49:46.000000 ccinput-1.8.0/ccinput/tests/test_qchem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-04-23 15:49:46.000000 ccinput-1.8.0/ccinput/tests/test_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22171 2023-04-23 15:49:46.000000 ccinput-1.8.0/ccinput/tests/test_xtb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-04-23 15:49:46.000000 ccinput-1.8.0/ccinput/tests/testing_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13072 2023-04-23 15:49:46.000000 ccinput-1.8.0/ccinput/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15174 2023-04-23 15:49:46.000000 ccinput-1.8.0/ccinput/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:50:23.617481 ccinput-1.8.0/ccinput.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-04-23 15:50:23.000000 ccinput-1.8.0/ccinput.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-23 15:50:23.000000 ccinput-1.8.0/ccinput.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 15:50:23.000000 ccinput-1.8.0/ccinput.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-23 15:50:23.000000 ccinput-1.8.0/ccinput.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 15:50:23.000000 ccinput-1.8.0/ccinput.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-23 15:50:23.000000 ccinput-1.8.0/ccinput.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-23 15:50:23.000000 ccinput-1.8.0/ccinput.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-23 15:49:46.000000 ccinput-1.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-23 15:50:23.621481 ccinput-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-23 15:49:46.000000 ccinput-1.8.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-04-23 15:49:46.000000 ccinput-1.8.0/versioneer.py
```

### Comparing `ccinput-1.7.2/LICENSE` & `ccinput-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ccinput-1.7.2/PKG-INFO` & `ccinput-1.8.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccinput
-Version: 1.7.2
+Version: 1.8.0
 Summary: Computational Chemistry Input Generator
 Home-page: http://github.com/cyllab/ccinput
 Author: Raphaël Robidas
 Author-email: Raphael.Robidas@USherbrooke.ca
 License: BSD 3-Clause
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
@@ -124,29 +124,25 @@
 
 ## Usage
 `ccinput` supports a wide range of options, including different solvation radii, density fitting and multiple basis sets. As of now, Gaussian 16, ORCA 5 and xtb are supported, and more packages will be added in the future.
 
 ### From the command line
 Simply use the `ccinput` command with the desired parameters:
 ```
-usage: ccinput [-h] [--basis_set BASIS_SET] [--solvent SOLVENT]
-               [--solvation_model SOLVATION_MODEL]
-               [--solvation_radii SOLVATION_RADII]
-               [--custom_solvation_radii CUSTOM_SOLVATION_RADII]
-               [--specifications SPECIFICATIONS]
-               [--density_fitting DENSITY_FITTING]
-               [--custom_basis_sets CUSTOM_BASIS_SETS] [--xyz XYZ]
-               [--file FILE [FILE ...]] [--output OUTPUT]
-               [--constraints CONSTRAINTS] [--freeze ATOM [ATOM ...]]
-               [--scan ATOM [ATOM ...]] [--from FROM] [--to TO]
-               [--nsteps NSTEPS] [--step STEP] [--nproc NPROC] [--mem MEM]
-               [--charge CHARGE] [--mult MULT] [--parse_name] [--d3 | --d3bj]
-               [--name NAME] [--aux_name AUX_NAME] [--header HEADER]
-               [--save SAVE] [--preset [PRESET]] [--version]
+
+usage: ccinput [-h] [--basis_set BASIS_SET] [--solvent SOLVENT] [--solvation_model SOLVATION_MODEL] 
+               [--solvation_radii SOLVATION_RADII] [--custom_solvation_radii CUSTOM_SOLVATION_RADII] 
+               [--specifications SPECIFICATIONS] [--density_fitting DENSITY_FITTING] [--custom_basis_sets CUSTOM_BASIS_SETS] 
+               [--xyz XYZ] [--file FILE [FILE ...]] [--output OUTPUT] [--constraints CONSTRAINTS] [--freeze ATOM [ATOM ...]] 
+               [--scan ATOM [ATOM ...]] [--from FROM] [--to TO] [--nsteps NSTEPS] [--step STEP] [--nproc NPROC] [--mem MEM] 
+               [--charge CHARGE] [--mult MULT] [--parse_name] [--trust_me] [--d3 | --d3bj] [--name NAME] 
+               [--aux_name AUX_NAME] [--header HEADER] [--save SAVE] [--preset [PRESET]] [--driver {none,ORCA,pysis}] 
+               [--version] [--fragments FRAGMENTS]
                [software] [type] [method]
+
 ```
 
 More detailed information about each option can be obtained with the `ccinput -h` command.
 
 ### As Python library
 The function `gen_input` returns input files as a single strings with the correct whitespace.
```

### Comparing `ccinput-1.7.2/README.md` & `ccinput-1.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -106,29 +106,25 @@
 
 ## Usage
 `ccinput` supports a wide range of options, including different solvation radii, density fitting and multiple basis sets. As of now, Gaussian 16, ORCA 5 and xtb are supported, and more packages will be added in the future.
 
 ### From the command line
 Simply use the `ccinput` command with the desired parameters:
 ```
-usage: ccinput [-h] [--basis_set BASIS_SET] [--solvent SOLVENT]
-               [--solvation_model SOLVATION_MODEL]
-               [--solvation_radii SOLVATION_RADII]
-               [--custom_solvation_radii CUSTOM_SOLVATION_RADII]
-               [--specifications SPECIFICATIONS]
-               [--density_fitting DENSITY_FITTING]
-               [--custom_basis_sets CUSTOM_BASIS_SETS] [--xyz XYZ]
-               [--file FILE [FILE ...]] [--output OUTPUT]
-               [--constraints CONSTRAINTS] [--freeze ATOM [ATOM ...]]
-               [--scan ATOM [ATOM ...]] [--from FROM] [--to TO]
-               [--nsteps NSTEPS] [--step STEP] [--nproc NPROC] [--mem MEM]
-               [--charge CHARGE] [--mult MULT] [--parse_name] [--d3 | --d3bj]
-               [--name NAME] [--aux_name AUX_NAME] [--header HEADER]
-               [--save SAVE] [--preset [PRESET]] [--version]
+
+usage: ccinput [-h] [--basis_set BASIS_SET] [--solvent SOLVENT] [--solvation_model SOLVATION_MODEL] 
+               [--solvation_radii SOLVATION_RADII] [--custom_solvation_radii CUSTOM_SOLVATION_RADII] 
+               [--specifications SPECIFICATIONS] [--density_fitting DENSITY_FITTING] [--custom_basis_sets CUSTOM_BASIS_SETS] 
+               [--xyz XYZ] [--file FILE [FILE ...]] [--output OUTPUT] [--constraints CONSTRAINTS] [--freeze ATOM [ATOM ...]] 
+               [--scan ATOM [ATOM ...]] [--from FROM] [--to TO] [--nsteps NSTEPS] [--step STEP] [--nproc NPROC] [--mem MEM] 
+               [--charge CHARGE] [--mult MULT] [--parse_name] [--trust_me] [--d3 | --d3bj] [--name NAME] 
+               [--aux_name AUX_NAME] [--header HEADER] [--save SAVE] [--preset [PRESET]] [--driver {none,ORCA,pysis}] 
+               [--version] [--fragments FRAGMENTS]
                [software] [type] [method]
+
 ```
 
 More detailed information about each option can be obtained with the `ccinput -h` command.
 
 ### As Python library
 The function `gen_input` returns input files as a single strings with the correct whitespace.
```

### Comparing `ccinput-1.7.2/ccinput/calculation.py` & `ccinput-1.8.0/ccinput/calculation.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.7.2/ccinput/constants.py` & `ccinput-1.8.0/ccinput/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,23 +26,23 @@
 LOWERCASE_ATOMIC_SYMBOLS = {}
 
 for el in periodictable.elements:
     ATOMIC_NUMBER[el.symbol] = el.number
     ATOMIC_SYMBOL[el.number] = el.symbol
     LOWERCASE_ATOMIC_SYMBOLS[el.symbol.lower()] = el.symbol
 
+# Synonyms for each type of calculation
 # The first synonym will be used as detailed name in the documentation
 SYN_TYPES = {
     CalcType.SP: [
         "Single-point Energy",
         "sp",
         "singlepoint",
         "singlepointenergy",
         "energy",
-        "scf",
     ],
     CalcType.OPT: [
         "Geometrical Optimisation",
         "opt",
         "optimize",
         "optimise",
         "optimisation",
@@ -100,14 +100,17 @@
         "Minimum energy path",
         "mep",
         "minimumenergypath",
         "minimalenergypath",
         "neb",
         "nudgedelasticband",
         "reactionpath",
+        "Freezing String Method",
+        "Freezing String",
+        "fsm",
     ],
     CalcType.MO: [
         "MO Calculation",
         "mo",
         "mocalc",
         "mocalculation",
         "molecularorbitals",
@@ -154,26 +157,31 @@
         "dlpnoccsdt",
         "dlpnoqcisd",
         "dlpnoqcisdt",
     ],
     # Everything else is assumed to be DFT, because it most likely is
 }
 
+# Synonyms for each software package
 SYN_SOFTWARE = {
     "gaussian": ["g16", "gaussian16"],
     "orca": ["orca5"],
+    "qchem": [],
     "xtb": [],
+    "psi4": ["psi4"],
 }
 
+# Synonym for each solvent.
+# The keys are "canonical" and used in other dictionaries to refer to each solvent.
 SYN_SOLVENTS = {
     "acetone": ["acetone"],
     "acetonitrile": ["acetonitrile", "acn", "ch3cn", "mecn"],
     "benzene": ["benzene", "c6h6"],
     "dichloromethane": ["ch2cl2", "dcm"],
-    "chloroform": ["chcl3"],
+    "chloroform": ["chcl3", "trichloromethane"],
     "carbondisulfide": ["cs2"],
     "dimethylformamide": ["dmf"],
     "dimethylsulfoxide": ["dmso"],
     "diethylether": ["ether", "et2o"],
     "water": ["h2o"],
     "methanol": ["meoh"],
     "nhexane": ["hexane", "hex"],
@@ -455,15 +463,15 @@
     "mn12sx": [],
     "mn12l": [],
     "vsxc": [],
     "hcth407": [],
     "hcth93": [],
     "hcth147": [],
     "thcth": [],
-    "hf": ["hartreefock"],
+    "hf": ["hartreefock", "scf"],
     "mndo": [],
     "am1": [],
     "pm3": [],
     "pm6": [],
     "pm7": ["pm7r6"],
     "gfn2xtb": ["xtb2", "gfn2"],
     "gfn1xtb": ["xtb1", "gfn1", "gfnxtb"],
@@ -865,14 +873,16 @@
     "w1mtsmall": [],
     "w1dz": [],
     "w1tz": [],
     "w1qz": [],
     "w1opt": [],
 }
 
+# Key: canonical basis set identifier (in ccinput)
+# Value: key in the Basis Set Exchange package
 # Not all basis sets below will be in SYN_BASIS_SETS (to complete).
 # ccinput will still attempt to find the key for the indexified input string.
 # Only orbital basis sets are included below.
 BASIS_SET_EXCHANGE_KEY = {
     "2zapanr": "2ZaPa-NR",
     "2zapanrcv": "2ZaPa-NR-CV",
     "321g": "3-21G",
@@ -1431,14 +1441,15 @@
     "x2ctzvpalls": "x2c-TZVPall-s",
     "x2ctzvppall": "x2c-TZVPPall",
     "x2ctzvppall2c": "x2c-TZVPPall-2c",
     "x2ctzvppalls": "x2c-TZVPPall-s",
 }
 
 
+# Specific keyword for each package (value) based on the canonical name (key)
 SOFTWARE_METHODS = {
     "orca": {
         "hfs": "HFS",
         "xalpha": "XAlpha",
         "lsd": "LSD",
         "vwn5": "VWN5",
         "vwn3": "VWN3",
@@ -1586,21 +1597,37 @@
         "thcth": "tHCTH",
         "am1": "AM1",
         "pm3": "PM3",
         "pm6": "PM6",
         "pm7": "PM7",
         "hf": "HF",
     },
+    "qchem": {
+        "am1": "am1",
+        "b3lyp": "b3lyp",
+        "hf": "hf",
+        "m062x": "m06-2x",
+        "pbe0": "pbe0",
+    },
     "xtb": {
         "gfn2xtb": "gfn2-xtb",
         "gfn1xtb": "gfn1-xtb",
         "gfn0xtb": "gfn0-xtb",
         "gfnff": "gfn-ff",
         "gfn2xtbgfnff": "gfn2-xtb//gfn-ff",
     },
+    "psi4": {
+        "hf": "scf",
+        "blyp": "blyp",
+        "b3lyp": "b3lyp",
+        "pbe": "pbe",
+        "pw91": "pw91",
+        "revpbe": "revpbe",
+        "rpbe": "rpbe",
+    },
 }
 
 SOFTWARE_BASIS_SETS = {
     "orca": {
         "sto3g": "STO-3G",
         "mini": "MINI",
         "minis": "MINIS",
@@ -2024,14 +2051,26 @@
         "sdd": "SDD",
         "sddall": "SDDAll",
         "dgdzvp": "DGDZVP",
         "dgdzvp2": "DGDZVP2",
         "gdtzvp": "DGTZVP",
         "cbsb7": "cbsb7",
     },
+    "qchem": {
+        "321g": "3-21g",
+        "631+gdp": "6-31+g(d,p)",
+        "def2svp": "def2-svp",
+        "def2tzvp": "def2-tzvp",
+    },
+    "psi4": {
+        "sto3g": "sto-3g",
+        "631g": "6-31G",
+        "ccpvdz": "cc-pVDZ",
+        "def2tzvp": "def2-tzvp",
+    },
 }
 
 SOFTWARE_SOLVENTS = {
     "gaussian": {
         "water": "water",
         "acetonitrile": "acetonitrile",
         "methanol": "methanol",
@@ -2401,14 +2440,18 @@
         "triethylamine": "triethylamine",
         "nundecane": "n-undecane",
         "xylenemixture": "xylene (mixture)",
         "mxylene": "m-xylene",
         "oxylene": "o-xylene",
         "pxylene": "p-xylene",
     },
+    "qchem": {
+        "chloroform": "trichloromethane",
+        "noctanol": "octanol",
+    },
     "xtb": {
         "acetone": "acetone",
         "acetonitrile": "acetonitrile",
         "benzene": "benzene",
         "dichloromethane": "ch2cl2",
         "chloroform": "chcl3",
         "carbon disulfide": "cs2",
```

### Comparing `ccinput-1.7.2/ccinput/documentation.py` & `ccinput-1.8.0/ccinput/documentation.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.7.2/ccinput/drivers/pysis.py` & `ccinput-1.8.0/ccinput/drivers/pysis.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.7.2/ccinput/packages/gaussian.py` & `ccinput-1.8.0/ccinput/packages/gaussian.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.7.2/ccinput/packages/nwchem.py` & `ccinput-1.8.0/ccinput/packages/nwchem.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.7.2/ccinput/packages/orca.py` & `ccinput-1.8.0/ccinput/packages/orca.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.7.2/ccinput/packages/xtb.py` & `ccinput-1.8.0/ccinput/packages/xtb.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,15 +171,15 @@
         self.input_file += f"atoms: {self.compress_indices(mtd_atoms)}\n"
 
     def handle_specifications(self):
         accuracy = -1
         iterations = -1
         method = "gfn2-xtb"
         opt_level = "tight"
-        rthr = 0.6
+        rthr = 2.0
         ewin = 6
         cmd_arguments = ""
 
         ALLOWED = "qwertyuiopasdfghjklzxcvbnm-1234567890./= "
         clean_specs = "".join(
             [
                 i
```

### Comparing `ccinput-1.7.2/ccinput/presets.py` & `ccinput-1.8.0/ccinput/presets.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.7.2/ccinput/tests/test_calculation.py` & `ccinput-1.8.0/ccinput/tests/test_calculation.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.7.2/ccinput/tests/test_cli.py` & `ccinput-1.8.0/ccinput/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.7.2/ccinput/tests/test_gaussian.py` & `ccinput-1.8.0/ccinput/tests/test_gaussian.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.7.2/ccinput/tests/test_orca.py` & `ccinput-1.8.0/ccinput/tests/test_orca.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.7.2/ccinput/tests/test_pysis.py` & `ccinput-1.8.0/ccinput/tests/test_pysis.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.7.2/ccinput/tests/test_structures.py` & `ccinput-1.8.0/ccinput/tests/test_structures.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.7.2/ccinput/tests/test_xtb.py` & `ccinput-1.8.0/ccinput/tests/test_xtb.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.7.2/ccinput/tests/testing_utilities.py` & `ccinput-1.8.0/ccinput/tests/testing_utilities.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.7.2/ccinput/utilities.py` & `ccinput-1.8.0/ccinput/utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -303,15 +303,15 @@
 def get_solvent(solvent, software, solvation_model="smd"):
     try:
         abs_solvent = get_abs_solvent(solvent)
     except InvalidParameter:
         warn(f"Unknown solvent '{solvent}'")
         return solvent
 
-    if software == "orca" and abs_solvent == "noctanol":
+    if software in ("orca", "qchem") and abs_solvent == "noctanol":
         # Weird exception in ORCA
         if solvation_model == "smd":
             return "1-octanol"
         elif solvation_model == "cpcm":
             return "octanol"
         # Note that ch2cl2 is a valid keyword for SMD, although not listed in the manual
```

### Comparing `ccinput-1.7.2/ccinput/wrapper.py` & `ccinput-1.8.0/ccinput/wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 import sys
 import shlex
 
 from ccinput.__init__ import __version__
 from ccinput.packages.gaussian import GaussianCalculation
 from ccinput.packages.orca import OrcaCalculation
 from ccinput.packages.nwchem import NWChemCalculation
+from ccinput.packages.qchem import QChemCalculation
 from ccinput.packages.xtb import XtbCalculation
 from ccinput.drivers.pysis import PysisDriver
+from ccinput.packages.psi4 import Psi4Calculation
 
 from ccinput.calculation import (
     Calculation,
     Parameters,
     Constraint,
     parse_str_constraints,
     parse_freeze_constraints,
@@ -36,14 +38,16 @@
 SOFTWARE_CLASSES = {
     "gaussian": GaussianCalculation,
     "orca": OrcaCalculation,
     "nwchem": NWChemCalculation,
     "xtb": XtbCalculation,
     "pysis": PysisDriver,
     "pysisyphus": PysisDriver,
+    "qchem": QChemCalculation,
+    "psi4": Psi4Calculation,
 }
 
 
 def process_calculation(calc):
     if calc.driver in ["none", None, ""] or calc.driver == calc.parameters.software:
         cls = SOFTWARE_CLASSES[calc.parameters.software](calc)
     else:
@@ -188,15 +192,17 @@
 def get_parser():
     import argparse
 
     parser = argparse.ArgumentParser(
         description="Generates an input for a computational chemistry package"
     )
     parser.add_argument(
-        "software", nargs="?", help="Desired software package (Gaussian or ORCA)"
+        "software",
+        nargs="?",
+        help="Desired software package (Gaussian, ORCA, Q-Chem, ...)",
     )
 
     parser.add_argument("type", nargs="?", help="Calculation type (opt, freq, sp, ...)")
 
     parser.add_argument(
         "method", nargs="?", help="Computational method (HF, AM1, B3LYP, ...)"
     )
```

### Comparing `ccinput-1.7.2/ccinput.egg-info/PKG-INFO` & `ccinput-1.8.0/ccinput.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccinput
-Version: 1.7.2
+Version: 1.8.0
 Summary: Computational Chemistry Input Generator
 Home-page: http://github.com/cyllab/ccinput
 Author: Raphaël Robidas
 Author-email: Raphael.Robidas@USherbrooke.ca
 License: BSD 3-Clause
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
@@ -124,29 +124,25 @@
 
 ## Usage
 `ccinput` supports a wide range of options, including different solvation radii, density fitting and multiple basis sets. As of now, Gaussian 16, ORCA 5 and xtb are supported, and more packages will be added in the future.
 
 ### From the command line
 Simply use the `ccinput` command with the desired parameters:
 ```
-usage: ccinput [-h] [--basis_set BASIS_SET] [--solvent SOLVENT]
-               [--solvation_model SOLVATION_MODEL]
-               [--solvation_radii SOLVATION_RADII]
-               [--custom_solvation_radii CUSTOM_SOLVATION_RADII]
-               [--specifications SPECIFICATIONS]
-               [--density_fitting DENSITY_FITTING]
-               [--custom_basis_sets CUSTOM_BASIS_SETS] [--xyz XYZ]
-               [--file FILE [FILE ...]] [--output OUTPUT]
-               [--constraints CONSTRAINTS] [--freeze ATOM [ATOM ...]]
-               [--scan ATOM [ATOM ...]] [--from FROM] [--to TO]
-               [--nsteps NSTEPS] [--step STEP] [--nproc NPROC] [--mem MEM]
-               [--charge CHARGE] [--mult MULT] [--parse_name] [--d3 | --d3bj]
-               [--name NAME] [--aux_name AUX_NAME] [--header HEADER]
-               [--save SAVE] [--preset [PRESET]] [--version]
+
+usage: ccinput [-h] [--basis_set BASIS_SET] [--solvent SOLVENT] [--solvation_model SOLVATION_MODEL] 
+               [--solvation_radii SOLVATION_RADII] [--custom_solvation_radii CUSTOM_SOLVATION_RADII] 
+               [--specifications SPECIFICATIONS] [--density_fitting DENSITY_FITTING] [--custom_basis_sets CUSTOM_BASIS_SETS] 
+               [--xyz XYZ] [--file FILE [FILE ...]] [--output OUTPUT] [--constraints CONSTRAINTS] [--freeze ATOM [ATOM ...]] 
+               [--scan ATOM [ATOM ...]] [--from FROM] [--to TO] [--nsteps NSTEPS] [--step STEP] [--nproc NPROC] [--mem MEM] 
+               [--charge CHARGE] [--mult MULT] [--parse_name] [--trust_me] [--d3 | --d3bj] [--name NAME] 
+               [--aux_name AUX_NAME] [--header HEADER] [--save SAVE] [--preset [PRESET]] [--driver {none,ORCA,pysis}] 
+               [--version] [--fragments FRAGMENTS]
                [software] [type] [method]
+
 ```
 
 More detailed information about each option can be obtained with the `ccinput -h` command.
 
 ### As Python library
 The function `gen_input` returns input files as a single strings with the correct whitespace.
```

### Comparing `ccinput-1.7.2/ccinput.egg-info/SOURCES.txt` & `ccinput-1.8.0/ccinput.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -23,17 +23,21 @@
 ccinput.egg-info/top_level.txt
 ccinput/drivers/__init__.py
 ccinput/drivers/pysis.py
 ccinput/packages/__init__.py
 ccinput/packages/gaussian.py
 ccinput/packages/nwchem.py
 ccinput/packages/orca.py
+ccinput/packages/psi4.py
+ccinput/packages/qchem.py
 ccinput/packages/xtb.py
 ccinput/tests/__init__.py
 ccinput/tests/test_calculation.py
 ccinput/tests/test_cli.py
 ccinput/tests/test_gaussian.py
 ccinput/tests/test_orca.py
+ccinput/tests/test_psi4.py
 ccinput/tests/test_pysis.py
+ccinput/tests/test_qchem.py
 ccinput/tests/test_structures.py
 ccinput/tests/test_xtb.py
 ccinput/tests/testing_utilities.py
```

### Comparing `ccinput-1.7.2/setup.py` & `ccinput-1.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.7.2/versioneer.py` & `ccinput-1.8.0/versioneer.py`

 * *Files identical despite different names*

