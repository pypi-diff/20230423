# Comparing `tmp/carculator-1.8.1.tar.gz` & `tmp/carculator-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carculator-1.8.1.tar", last modified: Mon Feb 13 10:07:28 2023, max compression
+gzip compressed data, was "carculator-1.8.2.tar", last modified: Sun Apr 23 14:12:33 2023, max compression
```

## Comparing `carculator-1.8.1.tar` & `carculator-1.8.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 10:07:28.669100 carculator-1.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-02-13 10:07:20.000000 carculator-1.8.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-02-13 10:07:20.000000 carculator-1.8.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-02-13 10:07:20.000000 carculator-1.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-02-13 10:07:20.000000 carculator-1.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9647 2023-02-13 10:07:28.669100 carculator-1.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-02-13 10:07:20.000000 carculator-1.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 10:07:28.665100 carculator-1.8.1/carculator/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-02-13 10:07:20.000000 carculator-1.8.1/carculator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-02-13 10:07:20.000000 carculator-1.8.1/carculator/car_input_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 10:07:28.669100 carculator-1.8.1/carculator/data/
--rw-r--r--   0 runner    (1001) docker     (123)   939226 2023-02-13 10:07:20.000000 carculator-1.8.1/carculator/data/default_parameters.json
--rw-r--r--   0 runner    (1001) docker     (123)     9485 2023-02-13 10:07:20.000000 carculator-1.8.1/carculator/data/extra_parameters.json
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-02-13 10:07:20.000000 carculator-1.8.1/carculator/data/purchase_cost_params.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7830 2023-02-13 10:07:20.000000 carculator-1.8.1/carculator/inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)    19534 2023-02-13 10:07:20.000000 carculator-1.8.1/carculator/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 10:07:28.665100 carculator-1.8.1/carculator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9647 2023-02-13 10:07:28.000000 carculator-1.8.1/carculator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-02-13 10:07:28.000000 carculator-1.8.1/carculator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 10:07:28.000000 carculator-1.8.1/carculator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-13 10:07:28.000000 carculator-1.8.1/carculator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-13 10:07:28.000000 carculator-1.8.1/carculator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-02-13 10:07:20.000000 carculator-1.8.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-02-13 10:07:20.000000 carculator-1.8.1/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-13 10:07:20.000000 carculator-1.8.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-13 10:07:28.669100 carculator-1.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-02-13 10:07:20.000000 carculator-1.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 10:07:28.669100 carculator-1.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-02-13 10:07:20.000000 carculator-1.8.1/tests/test_energy_consumption.py
--rw-r--r--   0 runner    (1001) docker     (123)     8416 2023-02-13 10:07:20.000000 carculator-1.8.1/tests/test_inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)     7780 2023-02-13 10:07:20.000000 carculator-1.8.1/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-02-13 10:07:20.000000 carculator-1.8.1/tests/test_vehicle_input_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:12:33.885304 carculator-1.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-04-23 14:12:24.000000 carculator-1.8.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-23 14:12:24.000000 carculator-1.8.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-23 14:12:24.000000 carculator-1.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-23 14:12:24.000000 carculator-1.8.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9760 2023-04-23 14:12:33.885304 carculator-1.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-04-23 14:12:24.000000 carculator-1.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:12:33.881304 carculator-1.8.2/carculator/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-23 14:12:24.000000 carculator-1.8.2/carculator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-23 14:12:24.000000 carculator-1.8.2/carculator/car_input_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:12:33.885304 carculator-1.8.2/carculator/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   939226 2023-04-23 14:12:24.000000 carculator-1.8.2/carculator/data/default_parameters.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9485 2023-04-23 14:12:24.000000 carculator-1.8.2/carculator/data/extra_parameters.json
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-23 14:12:24.000000 carculator-1.8.2/carculator/data/purchase_cost_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7830 2023-04-23 14:12:24.000000 carculator-1.8.2/carculator/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19953 2023-04-23 14:12:24.000000 carculator-1.8.2/carculator/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:12:33.881304 carculator-1.8.2/carculator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9760 2023-04-23 14:12:33.000000 carculator-1.8.2/carculator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-23 14:12:33.000000 carculator-1.8.2/carculator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 14:12:33.000000 carculator-1.8.2/carculator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-23 14:12:33.000000 carculator-1.8.2/carculator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-23 14:12:33.000000 carculator-1.8.2/carculator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-23 14:12:24.000000 carculator-1.8.2/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-23 14:12:24.000000 carculator-1.8.2/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-23 14:12:24.000000 carculator-1.8.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 14:12:33.885304 carculator-1.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-23 14:12:24.000000 carculator-1.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:12:33.885304 carculator-1.8.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-23 14:12:24.000000 carculator-1.8.2/tests/test_energy_consumption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8416 2023-04-23 14:12:24.000000 carculator-1.8.2/tests/test_inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7780 2023-04-23 14:12:24.000000 carculator-1.8.2/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-23 14:12:24.000000 carculator-1.8.2/tests/test_vehicle_input_parameters.py
```

### Comparing `carculator-1.8.1/CODE_OF_CONDUCT.md` & `carculator-1.8.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `carculator-1.8.1/CONTRIBUTING.md` & `carculator-1.8.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `carculator-1.8.1/LICENSE` & `carculator-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `carculator-1.8.1/PKG-INFO` & `carculator-1.8.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carculator
-Version: 1.8.1
+Version: 1.8.2
 Summary: Prospective life cycle assessment of vehicles made blazing fast
 Home-page: https://github.com/romainsacchi/carculator
 Author: Romain Sacchi <romain.sacchi@psi.ch>, Chris Mutel <christopher.mutel@psi.ch>
 License: BSD 3-Clause License
         
         Copyright (c) 2020, Paul Scherrer Institut
         
@@ -122,67 +122,68 @@
 
 We recommend the installation on **Python 3.7 or above**.
 
 ### Installation of the latest version, using conda
 
     conda install -c romainsacchi carculator
 
-### Installation of a stable release (1.3.1) from Pypi
+### Installation of a stable release from Pypi
 
     pip install carculator
 
 ## Usage
 
 ### As a Python library
 
 Calculate the fuel efficiency (or ``Tank to wheel`` energy requirement) in km/L of petrol-equivalent of current SUVs for the driving cycle WLTC 3.4
 over 800 Monte Carlo iterations:
 
 ```python
-    from carculator import *
-import matplotlib.pyplot as plt
 
-cip = CarInputParameters()
-cip.stochastic(800)
-dcts, array = fill_xarray_from_input_parameters(cip)
-cm = CarModel(array, cycle='WLTC 3.4')
-cm.set_all()
-TtW_energy = 1 / (cm.array.sel(size='SUV', year=2020, parameter='TtW energy') / 42000)  # assuming 42 MJ/L petrol
-
-l_powertrains = TtW_energy.powertrain
-[plt.hist(e, bins=50, alpha=.8, label=e.powertrain.values) for e in TtW_energy]
-plt.xlabel('km/L petrol-equivalent')
-plt.ylabel('number of iterations')
-plt.legend()
+    from carculator import *
+    import matplotlib.pyplot as plt
+    
+    cip = CarInputParameters()
+    cip.stochastic(800)
+    dcts, array = fill_xarray_from_input_parameters(cip)
+    cm = CarModel(array, cycle='WLTC 3.4')
+    cm.set_all()
+    TtW_energy = 1 / (cm.array.sel(size='SUV', year=2020, parameter='TtW energy') / 42000)  # assuming 42 MJ/L petrol
+    
+    l_powertrains = TtW_energy.powertrain
+    [plt.hist(e, bins=50, alpha=.8, label=e.powertrain.values) for e in TtW_energy]
+    plt.xlabel('km/L petrol-equivalent')
+    plt.ylabel('number of iterations')
+    plt.legend()
 ```
 
 ![MC results](https://github.com/romainsacchi/carculator/blob/master/docs/_static/img/stochastic_example_ttw.png)
 
 Compare the carbon footprint of electric vehicles with that of rechargeable hybrid vehicles for different size categories today and in the future
 over 500 Monte Carlo iterations:
 
 ```python
-    from carculator import *
 
-cip = CarInputParameters()
-cip.stochastic(500)
-dcts, array = fill_xarray_from_input_parameters(cip)
-cm = CarModel(array, cycle='WLTC')
-cm.set_all()
-scope = {
-  'powertrain': ['BEV', 'PHEV'],
-}
-ic = InventoryCalculation(cm)
-
-results = ic.calculate_impacts()
-data_MC = results.sel(impact_category='climate change').sum(axis=3).to_dataframe('climate change')
-plt.style.use('seaborn')
-data_MC.unstack(level=[0, 1, 2]).boxplot(showfliers=False, figsize=(20, 5))
-plt.xticks(rotation=70)
-plt.ylabel('kg CO2-eq./vkm')
+    from carculator import *
+    cip = CarInputParameters()
+    cip.stochastic(500)
+    dcts, array = fill_xarray_from_input_parameters(cip)
+    cm = CarModel(array, cycle='WLTC')
+    cm.set_all()
+    scope = {
+      'powertrain': ['BEV', 'PHEV'],
+    }
+    ic = InventoryCalculation(cm)
+    
+    results = ic.calculate_impacts()
+    data_MC = results.sel(impact_category='climate change').sum(axis=3).to_dataframe('climate change')
+    plt.style.use('seaborn')
+    data_MC.unstack(level=[0, 1, 2]).boxplot(showfliers=False, figsize=(20, 5))
+    plt.xticks(rotation=70)
+    plt.ylabel('kg CO2-eq./vkm')
 ```
 
 ![MC results](https://github.com/romainsacchi/carculator/blob/master/docs/_static/img/example_stochastic_BEV_PHEV.png)
 
 For more examples, see [examples](https://github.com/romainsacchi/carculator/blob/master/examples/Examples.ipynb).
 
 ## As a Web app
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: carculator Version: 1.8.1 Summary: Prospective life
+Metadata-Version: 2.1 Name: carculator Version: 1.8.2 Summary: Prospective life
 cycle assessment of vehicles made blazing fast Home-page: https://github.com/
 romainsacchi/carculator Author: Romain Sacchi
 sacchi@psi.ch>, Chris Mutel
 mutel@psi.ch> License: BSD 3-Clause License Copyright (c) 2020, Paul Scherrer
 Institut Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met: *
 Redistributions of source code must retain the above copyright notice, this
@@ -79,23 +79,23 @@
 ``carculator`` was built based on work described in [Uncertain environmental
 footprint of current and future battery electric vehicles by Cox, et al (2018)]
 (https://pubs.acs.org/doi/abs/10.1021/acs.est.8b00261). ## Install
 ``carculator`` is at an early stage of development and is subject to continuous
 change and improvement. Three ways of installing ``carculator`` are suggested.
 We recommend the installation on **Python 3.7 or above**. ### Installation of
 the latest version, using conda conda install -c romainsacchi carculator ###
-Installation of a stable release (1.3.1) from Pypi pip install carculator ##
-Usage ### As a Python library Calculate the fuel efficiency (or ``Tank to
-wheel`` energy requirement) in km/L of petrol-equivalent of current SUVs for
-the driving cycle WLTC 3.4 over 800 Monte Carlo iterations: ```python from
-carculator import * import matplotlib.pyplot as plt cip = CarInputParameters()
-cip.stochastic(800) dcts, array = fill_xarray_from_input_parameters(cip) cm =
-CarModel(array, cycle='WLTC 3.4') cm.set_all() TtW_energy = 1 / (cm.array.sel
-(size='SUV', year=2020, parameter='TtW energy') / 42000) # assuming 42 MJ/
-L petrol l_powertrains = TtW_energy.powertrain [plt.hist(e, bins=50, alpha=.8,
+Installation of a stable release from Pypi pip install carculator ## Usage ###
+As a Python library Calculate the fuel efficiency (or ``Tank to wheel`` energy
+requirement) in km/L of petrol-equivalent of current SUVs for the driving cycle
+WLTC 3.4 over 800 Monte Carlo iterations: ```python from carculator import *
+import matplotlib.pyplot as plt cip = CarInputParameters() cip.stochastic(800)
+dcts, array = fill_xarray_from_input_parameters(cip) cm = CarModel(array,
+cycle='WLTC 3.4') cm.set_all() TtW_energy = 1 / (cm.array.sel(size='SUV',
+year=2020, parameter='TtW energy') / 42000) # assuming 42 MJ/L petrol
+l_powertrains = TtW_energy.powertrain [plt.hist(e, bins=50, alpha=.8,
 label=e.powertrain.values) for e in TtW_energy] plt.xlabel('km/L petrol-
 equivalent') plt.ylabel('number of iterations') plt.legend() ``` ![MC results]
 (https://github.com/romainsacchi/carculator/blob/master/docs/_static/img/
 stochastic_example_ttw.png) Compare the carbon footprint of electric vehicles
 with that of rechargeable hybrid vehicles for different size categories today
 and in the future over 500 Monte Carlo iterations: ```python from carculator
 import * cip = CarInputParameters() cip.stochastic(500) dcts, array =
```

### Comparing `carculator-1.8.1/README.md` & `carculator-1.8.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -68,67 +68,68 @@
 
 We recommend the installation on **Python 3.7 or above**.
 
 ### Installation of the latest version, using conda
 
     conda install -c romainsacchi carculator
 
-### Installation of a stable release (1.3.1) from Pypi
+### Installation of a stable release from Pypi
 
     pip install carculator
 
 ## Usage
 
 ### As a Python library
 
 Calculate the fuel efficiency (or ``Tank to wheel`` energy requirement) in km/L of petrol-equivalent of current SUVs for the driving cycle WLTC 3.4
 over 800 Monte Carlo iterations:
 
 ```python
-    from carculator import *
-import matplotlib.pyplot as plt
 
-cip = CarInputParameters()
-cip.stochastic(800)
-dcts, array = fill_xarray_from_input_parameters(cip)
-cm = CarModel(array, cycle='WLTC 3.4')
-cm.set_all()
-TtW_energy = 1 / (cm.array.sel(size='SUV', year=2020, parameter='TtW energy') / 42000)  # assuming 42 MJ/L petrol
-
-l_powertrains = TtW_energy.powertrain
-[plt.hist(e, bins=50, alpha=.8, label=e.powertrain.values) for e in TtW_energy]
-plt.xlabel('km/L petrol-equivalent')
-plt.ylabel('number of iterations')
-plt.legend()
+    from carculator import *
+    import matplotlib.pyplot as plt
+    
+    cip = CarInputParameters()
+    cip.stochastic(800)
+    dcts, array = fill_xarray_from_input_parameters(cip)
+    cm = CarModel(array, cycle='WLTC 3.4')
+    cm.set_all()
+    TtW_energy = 1 / (cm.array.sel(size='SUV', year=2020, parameter='TtW energy') / 42000)  # assuming 42 MJ/L petrol
+    
+    l_powertrains = TtW_energy.powertrain
+    [plt.hist(e, bins=50, alpha=.8, label=e.powertrain.values) for e in TtW_energy]
+    plt.xlabel('km/L petrol-equivalent')
+    plt.ylabel('number of iterations')
+    plt.legend()
 ```
 
 ![MC results](https://github.com/romainsacchi/carculator/blob/master/docs/_static/img/stochastic_example_ttw.png)
 
 Compare the carbon footprint of electric vehicles with that of rechargeable hybrid vehicles for different size categories today and in the future
 over 500 Monte Carlo iterations:
 
 ```python
-    from carculator import *
 
-cip = CarInputParameters()
-cip.stochastic(500)
-dcts, array = fill_xarray_from_input_parameters(cip)
-cm = CarModel(array, cycle='WLTC')
-cm.set_all()
-scope = {
-  'powertrain': ['BEV', 'PHEV'],
-}
-ic = InventoryCalculation(cm)
-
-results = ic.calculate_impacts()
-data_MC = results.sel(impact_category='climate change').sum(axis=3).to_dataframe('climate change')
-plt.style.use('seaborn')
-data_MC.unstack(level=[0, 1, 2]).boxplot(showfliers=False, figsize=(20, 5))
-plt.xticks(rotation=70)
-plt.ylabel('kg CO2-eq./vkm')
+    from carculator import *
+    cip = CarInputParameters()
+    cip.stochastic(500)
+    dcts, array = fill_xarray_from_input_parameters(cip)
+    cm = CarModel(array, cycle='WLTC')
+    cm.set_all()
+    scope = {
+      'powertrain': ['BEV', 'PHEV'],
+    }
+    ic = InventoryCalculation(cm)
+    
+    results = ic.calculate_impacts()
+    data_MC = results.sel(impact_category='climate change').sum(axis=3).to_dataframe('climate change')
+    plt.style.use('seaborn')
+    data_MC.unstack(level=[0, 1, 2]).boxplot(showfliers=False, figsize=(20, 5))
+    plt.xticks(rotation=70)
+    plt.ylabel('kg CO2-eq./vkm')
 ```
 
 ![MC results](https://github.com/romainsacchi/carculator/blob/master/docs/_static/img/example_stochastic_BEV_PHEV.png)
 
 For more examples, see [examples](https://github.com/romainsacchi/carculator/blob/master/examples/Examples.ipynb).
 
 ## As a Web app
```

#### html2text {}

```diff
@@ -44,23 +44,23 @@
 ``carculator`` was built based on work described in [Uncertain environmental
 footprint of current and future battery electric vehicles by Cox, et al (2018)]
 (https://pubs.acs.org/doi/abs/10.1021/acs.est.8b00261). ## Install
 ``carculator`` is at an early stage of development and is subject to continuous
 change and improvement. Three ways of installing ``carculator`` are suggested.
 We recommend the installation on **Python 3.7 or above**. ### Installation of
 the latest version, using conda conda install -c romainsacchi carculator ###
-Installation of a stable release (1.3.1) from Pypi pip install carculator ##
-Usage ### As a Python library Calculate the fuel efficiency (or ``Tank to
-wheel`` energy requirement) in km/L of petrol-equivalent of current SUVs for
-the driving cycle WLTC 3.4 over 800 Monte Carlo iterations: ```python from
-carculator import * import matplotlib.pyplot as plt cip = CarInputParameters()
-cip.stochastic(800) dcts, array = fill_xarray_from_input_parameters(cip) cm =
-CarModel(array, cycle='WLTC 3.4') cm.set_all() TtW_energy = 1 / (cm.array.sel
-(size='SUV', year=2020, parameter='TtW energy') / 42000) # assuming 42 MJ/
-L petrol l_powertrains = TtW_energy.powertrain [plt.hist(e, bins=50, alpha=.8,
+Installation of a stable release from Pypi pip install carculator ## Usage ###
+As a Python library Calculate the fuel efficiency (or ``Tank to wheel`` energy
+requirement) in km/L of petrol-equivalent of current SUVs for the driving cycle
+WLTC 3.4 over 800 Monte Carlo iterations: ```python from carculator import *
+import matplotlib.pyplot as plt cip = CarInputParameters() cip.stochastic(800)
+dcts, array = fill_xarray_from_input_parameters(cip) cm = CarModel(array,
+cycle='WLTC 3.4') cm.set_all() TtW_energy = 1 / (cm.array.sel(size='SUV',
+year=2020, parameter='TtW energy') / 42000) # assuming 42 MJ/L petrol
+l_powertrains = TtW_energy.powertrain [plt.hist(e, bins=50, alpha=.8,
 label=e.powertrain.values) for e in TtW_energy] plt.xlabel('km/L petrol-
 equivalent') plt.ylabel('number of iterations') plt.legend() ``` ![MC results]
 (https://github.com/romainsacchi/carculator/blob/master/docs/_static/img/
 stochastic_example_ttw.png) Compare the carbon footprint of electric vehicles
 with that of rechargeable hybrid vehicles for different size categories today
 and in the future over 500 Monte Carlo iterations: ```python from carculator
 import * cip = CarInputParameters() cip.stochastic(500) dcts, array =
```

### Comparing `carculator-1.8.1/carculator/__init__.py` & `carculator-1.8.2/carculator/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 __all__ = (
     "CarInputParameters",
     "fill_xarray_from_input_parameters",
     "CarModel",
     "InventoryCar",
     "get_standard_driving_cycle_and_gradient",
 )
-__version__ = (1, 8, 1)
+__version__ = (1, 8, 2)
 
 from pathlib import Path
 
 DATA_DIR = Path(__file__).resolve().parent / "data"
 
 from carculator_utils.array import fill_xarray_from_input_parameters
 from carculator_utils.driving_cycles import get_standard_driving_cycle_and_gradient
```

### Comparing `carculator-1.8.1/carculator/car_input_parameters.py` & `carculator-1.8.2/carculator/car_input_parameters.py`

 * *Files identical despite different names*

### Comparing `carculator-1.8.1/carculator/data/default_parameters.json` & `carculator-1.8.2/carculator/data/default_parameters.json`

 * *Files identical despite different names*

### Comparing `carculator-1.8.1/carculator/data/extra_parameters.json` & `carculator-1.8.2/carculator/data/extra_parameters.json`

 * *Files identical despite different names*

### Comparing `carculator-1.8.1/carculator/data/purchase_cost_params.yaml` & `carculator-1.8.2/carculator/data/purchase_cost_params.yaml`

 * *Files identical despite different names*

### Comparing `carculator-1.8.1/carculator/inventory.py` & `carculator-1.8.2/carculator/inventory.py`

 * *Files identical despite different names*

### Comparing `carculator-1.8.1/carculator/model.py` & `carculator-1.8.2/carculator/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 from itertools import product
-from typing import Dict, List, Union
 
-import numexpr as ne
 import numpy as np
-import xarray as xr
 import yaml
 from carculator_utils.energy_consumption import EnergyConsumptionModel
 from carculator_utils.model import VehicleModel
 
 from . import DATA_DIR
 
 
 class CarModel(VehicleModel):
-
     """
     This class represents the entirety of the vehicles considered, with useful attributes, such as an array that stores
     all the vehicles parameters.
 
     :ivar array: multi-dimensional numpy-like array that contains parameters' value(s)
     :ivar cycle: name of a driving cycle, or custom driving cycle
     :ivar gradient: series of gradients, for each second of the driving cycle
@@ -44,26 +40,25 @@
         :returns: Does not return anything. Modifies ``self.array`` in place.
 
         """
 
         self.ecm = EnergyConsumptionModel(
             vehicle_type="car",
             vehicle_size=list(self.array.coords["size"].values),
+            powertrains=list(self.array.coords["powertrain"].values),
             cycle=self.cycle,
             gradient=self.gradient,
             country=self.country,
         )
 
         diff = 1.0
 
         while diff > 0.0001:
             old_driving_mass = self["driving mass"].sum().values
-
             self.set_vehicle_mass()
-
             self.set_power_parameters()
             self.set_component_masses()
             self.set_auxiliaries()
             self.set_power_battery_properties()
             self.set_battery_properties()
             self.set_energy_stored_properties()
             self.set_recuperation()
@@ -230,16 +225,14 @@
             rr_coef=self["rolling resistance coefficient"],
             drag_coef=self["aerodynamic drag coefficient"],
             frontal_area=self["frontal area"],
             electric_motor_power=self["electric power"],
             engine_power=self["power"],
             recuperation_efficiency=self["recuperation efficiency"],
             aux_power=self["auxiliary power demand"],
-            engine_efficiency=self["engine efficiency"],
-            transmission_efficiency=self["transmission efficiency"],
             battery_charge_eff=self["battery charge efficiency"],
             battery_discharge_eff=self["battery discharge efficiency"],
             fuel_cell_system_efficiency=self["fuel cell system efficiency"],
         )
 
         self.energy = self.energy.assign_coords(
             {
@@ -258,14 +251,32 @@
         self["TtW energy"] = (
             self.energy.sel(
                 parameter=["motive energy", "auxiliary energy", "recuperated energy"]
             ).sum(dim=["second", "parameter"])
             / distance
         ).T
 
+        self["engine efficiency"] = (
+            np.ma.array(
+                self.energy.loc[dict(parameter="engine efficiency")],
+                mask=self.energy.loc[dict(parameter="power load")] == 0,
+            )
+            .mean(axis=0)
+            .T
+        )
+
+        self["transmission efficiency"] = (
+            np.ma.array(
+                self.energy.loc[dict(parameter="transmission efficiency")],
+                mask=self.energy.loc[dict(parameter="power load")] == 0,
+            )
+            .mean(axis=0)
+            .T
+        )
+
         self["TtW energy, combustion mode"] = self["TtW energy"] * (
             self["combustion power share"] > 0
         )
         self["TtW energy, electric mode"] = self["TtW energy"] * (
             self["combustion power share"] == 0
         )
```

### Comparing `carculator-1.8.1/carculator.egg-info/PKG-INFO` & `carculator-1.8.2/carculator.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carculator
-Version: 1.8.1
+Version: 1.8.2
 Summary: Prospective life cycle assessment of vehicles made blazing fast
 Home-page: https://github.com/romainsacchi/carculator
 Author: Romain Sacchi <romain.sacchi@psi.ch>, Chris Mutel <christopher.mutel@psi.ch>
 License: BSD 3-Clause License
         
         Copyright (c) 2020, Paul Scherrer Institut
         
@@ -122,67 +122,68 @@
 
 We recommend the installation on **Python 3.7 or above**.
 
 ### Installation of the latest version, using conda
 
     conda install -c romainsacchi carculator
 
-### Installation of a stable release (1.3.1) from Pypi
+### Installation of a stable release from Pypi
 
     pip install carculator
 
 ## Usage
 
 ### As a Python library
 
 Calculate the fuel efficiency (or ``Tank to wheel`` energy requirement) in km/L of petrol-equivalent of current SUVs for the driving cycle WLTC 3.4
 over 800 Monte Carlo iterations:
 
 ```python
-    from carculator import *
-import matplotlib.pyplot as plt
 
-cip = CarInputParameters()
-cip.stochastic(800)
-dcts, array = fill_xarray_from_input_parameters(cip)
-cm = CarModel(array, cycle='WLTC 3.4')
-cm.set_all()
-TtW_energy = 1 / (cm.array.sel(size='SUV', year=2020, parameter='TtW energy') / 42000)  # assuming 42 MJ/L petrol
-
-l_powertrains = TtW_energy.powertrain
-[plt.hist(e, bins=50, alpha=.8, label=e.powertrain.values) for e in TtW_energy]
-plt.xlabel('km/L petrol-equivalent')
-plt.ylabel('number of iterations')
-plt.legend()
+    from carculator import *
+    import matplotlib.pyplot as plt
+    
+    cip = CarInputParameters()
+    cip.stochastic(800)
+    dcts, array = fill_xarray_from_input_parameters(cip)
+    cm = CarModel(array, cycle='WLTC 3.4')
+    cm.set_all()
+    TtW_energy = 1 / (cm.array.sel(size='SUV', year=2020, parameter='TtW energy') / 42000)  # assuming 42 MJ/L petrol
+    
+    l_powertrains = TtW_energy.powertrain
+    [plt.hist(e, bins=50, alpha=.8, label=e.powertrain.values) for e in TtW_energy]
+    plt.xlabel('km/L petrol-equivalent')
+    plt.ylabel('number of iterations')
+    plt.legend()
 ```
 
 ![MC results](https://github.com/romainsacchi/carculator/blob/master/docs/_static/img/stochastic_example_ttw.png)
 
 Compare the carbon footprint of electric vehicles with that of rechargeable hybrid vehicles for different size categories today and in the future
 over 500 Monte Carlo iterations:
 
 ```python
-    from carculator import *
 
-cip = CarInputParameters()
-cip.stochastic(500)
-dcts, array = fill_xarray_from_input_parameters(cip)
-cm = CarModel(array, cycle='WLTC')
-cm.set_all()
-scope = {
-  'powertrain': ['BEV', 'PHEV'],
-}
-ic = InventoryCalculation(cm)
-
-results = ic.calculate_impacts()
-data_MC = results.sel(impact_category='climate change').sum(axis=3).to_dataframe('climate change')
-plt.style.use('seaborn')
-data_MC.unstack(level=[0, 1, 2]).boxplot(showfliers=False, figsize=(20, 5))
-plt.xticks(rotation=70)
-plt.ylabel('kg CO2-eq./vkm')
+    from carculator import *
+    cip = CarInputParameters()
+    cip.stochastic(500)
+    dcts, array = fill_xarray_from_input_parameters(cip)
+    cm = CarModel(array, cycle='WLTC')
+    cm.set_all()
+    scope = {
+      'powertrain': ['BEV', 'PHEV'],
+    }
+    ic = InventoryCalculation(cm)
+    
+    results = ic.calculate_impacts()
+    data_MC = results.sel(impact_category='climate change').sum(axis=3).to_dataframe('climate change')
+    plt.style.use('seaborn')
+    data_MC.unstack(level=[0, 1, 2]).boxplot(showfliers=False, figsize=(20, 5))
+    plt.xticks(rotation=70)
+    plt.ylabel('kg CO2-eq./vkm')
 ```
 
 ![MC results](https://github.com/romainsacchi/carculator/blob/master/docs/_static/img/example_stochastic_BEV_PHEV.png)
 
 For more examples, see [examples](https://github.com/romainsacchi/carculator/blob/master/examples/Examples.ipynb).
 
 ## As a Web app
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: carculator Version: 1.8.1 Summary: Prospective life
+Metadata-Version: 2.1 Name: carculator Version: 1.8.2 Summary: Prospective life
 cycle assessment of vehicles made blazing fast Home-page: https://github.com/
 romainsacchi/carculator Author: Romain Sacchi
 sacchi@psi.ch>, Chris Mutel
 mutel@psi.ch> License: BSD 3-Clause License Copyright (c) 2020, Paul Scherrer
 Institut Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met: *
 Redistributions of source code must retain the above copyright notice, this
@@ -79,23 +79,23 @@
 ``carculator`` was built based on work described in [Uncertain environmental
 footprint of current and future battery electric vehicles by Cox, et al (2018)]
 (https://pubs.acs.org/doi/abs/10.1021/acs.est.8b00261). ## Install
 ``carculator`` is at an early stage of development and is subject to continuous
 change and improvement. Three ways of installing ``carculator`` are suggested.
 We recommend the installation on **Python 3.7 or above**. ### Installation of
 the latest version, using conda conda install -c romainsacchi carculator ###
-Installation of a stable release (1.3.1) from Pypi pip install carculator ##
-Usage ### As a Python library Calculate the fuel efficiency (or ``Tank to
-wheel`` energy requirement) in km/L of petrol-equivalent of current SUVs for
-the driving cycle WLTC 3.4 over 800 Monte Carlo iterations: ```python from
-carculator import * import matplotlib.pyplot as plt cip = CarInputParameters()
-cip.stochastic(800) dcts, array = fill_xarray_from_input_parameters(cip) cm =
-CarModel(array, cycle='WLTC 3.4') cm.set_all() TtW_energy = 1 / (cm.array.sel
-(size='SUV', year=2020, parameter='TtW energy') / 42000) # assuming 42 MJ/
-L petrol l_powertrains = TtW_energy.powertrain [plt.hist(e, bins=50, alpha=.8,
+Installation of a stable release from Pypi pip install carculator ## Usage ###
+As a Python library Calculate the fuel efficiency (or ``Tank to wheel`` energy
+requirement) in km/L of petrol-equivalent of current SUVs for the driving cycle
+WLTC 3.4 over 800 Monte Carlo iterations: ```python from carculator import *
+import matplotlib.pyplot as plt cip = CarInputParameters() cip.stochastic(800)
+dcts, array = fill_xarray_from_input_parameters(cip) cm = CarModel(array,
+cycle='WLTC 3.4') cm.set_all() TtW_energy = 1 / (cm.array.sel(size='SUV',
+year=2020, parameter='TtW energy') / 42000) # assuming 42 MJ/L petrol
+l_powertrains = TtW_energy.powertrain [plt.hist(e, bins=50, alpha=.8,
 label=e.powertrain.values) for e in TtW_energy] plt.xlabel('km/L petrol-
 equivalent') plt.ylabel('number of iterations') plt.legend() ``` ![MC results]
 (https://github.com/romainsacchi/carculator/blob/master/docs/_static/img/
 stochastic_example_ttw.png) Compare the carbon footprint of electric vehicles
 with that of rechargeable hybrid vehicles for different size categories today
 and in the future over 500 Monte Carlo iterations: ```python from carculator
 import * cip = CarInputParameters() cip.stochastic(500) dcts, array =
```

### Comparing `carculator-1.8.1/carculator.egg-info/SOURCES.txt` & `carculator-1.8.2/carculator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `carculator-1.8.1/readthedocs.yml` & `carculator-1.8.2/readthedocs.yml`

 * *Files identical despite different names*

### Comparing `carculator-1.8.1/setup.py` & `carculator-1.8.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,21 +31,21 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="carculator",
-    version="1.8.1",
+    version="1.8.2",
     packages=packages,
     author="Romain Sacchi <romain.sacchi@psi.ch>, Chris Mutel <christopher.mutel@psi.ch>",
     license=open("LICENSE").read(),
     package_data={"carculator": package_files(os.path.join("carculator", "data"))},
     install_requires=[
-        "carculator_utils>1.0.3",
+        "carculator_utils",
     ],
     url="https://github.com/romainsacchi/carculator",
     description="Prospective life cycle assessment of vehicles made blazing fast",
     long_description_content_type="text/markdown",
     long_description=README,
     classifiers=[
         "Intended Audience :: End Users/Desktop",
```

### Comparing `carculator-1.8.1/tests/test_inventory.py` & `carculator-1.8.2/tests/test_inventory.py`

 * *Files identical despite different names*

### Comparing `carculator-1.8.1/tests/test_model.py` & `carculator-1.8.2/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `carculator-1.8.1/tests/test_vehicle_input_parameters.py` & `carculator-1.8.2/tests/test_vehicle_input_parameters.py`

 * *Files identical despite different names*

