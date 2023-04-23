# Comparing `tmp/carculator_utils-1.0.4.tar.gz` & `tmp/carculator_utils-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carculator_utils-1.0.4.tar", last modified: Fri Feb 10 20:56:14 2023, max compression
+gzip compressed data, was "carculator_utils-1.0.5.tar", last modified: Sun Apr 23 11:18:06 2023, max compression
```

## Comparing `carculator_utils-1.0.4.tar` & `carculator_utils-1.0.5.tar`

### file list

```diff
@@ -1,165 +1,169 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 20:56:14.749654 carculator_utils-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-02-10 20:56:14.749654 carculator_utils-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 20:56:14.689654 carculator_utils-1.0.4/carculator_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    13413 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/background_systems.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 20:56:14.689654 carculator_utils-1.0.4/carculator_utils/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 20:56:14.729654 carculator_utils-1.0.4/carculator_utils/data/IAM/
--rw-r--r--   0 runner    (1001) docker     (123)    82764 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/IAM/A_matrix.csv
--rw-r--r--   0 runner    (1001) docker     (123)   614740 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-NPi_2030.csv
--rw-r--r--   0 runner    (1001) docker     (123)   614741 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-NPi_2040.csv
--rw-r--r--   0 runner    (1001) docker     (123)   614739 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-NPi_2050.csv
--rw-r--r--   0 runner    (1001) docker     (123)   614739 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg1150_2030.csv
--rw-r--r--   0 runner    (1001) docker     (123)   614741 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg1150_2040.csv
--rw-r--r--   0 runner    (1001) docker     (123)   614741 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg1150_2050.csv
--rw-r--r--   0 runner    (1001) docker     (123)   614739 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg500_2030.csv
--rw-r--r--   0 runner    (1001) docker     (123)   614741 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg500_2040.csv
--rw-r--r--   0 runner    (1001) docker     (123)   614741 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg500_2050.csv
--rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-NPi_2005.csv
--rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-NPi_2010.csv
--rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-NPi_2020.csv
--rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg1150_2005.csv
--rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg1150_2010.csv
--rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg1150_2020.csv
--rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg500_2005.csv
--rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg500_2010.csv
--rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg500_2020.csv
--rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_static_ 3.8 cutoff.csv
--rw-r--r--   0 runner    (1001) docker     (123)   129388 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-NPi_2030.csv
--rw-r--r--   0 runner    (1001) docker     (123)   129388 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-NPi_2040.csv
--rw-r--r--   0 runner    (1001) docker     (123)   129388 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-NPi_2050.csv
--rw-r--r--   0 runner    (1001) docker     (123)   129388 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg1150_2030.csv
--rw-r--r--   0 runner    (1001) docker     (123)   129389 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg1150_2040.csv
--rw-r--r--   0 runner    (1001) docker     (123)   129389 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg1150_2050.csv
--rw-r--r--   0 runner    (1001) docker     (123)   129389 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg500_2030.csv
--rw-r--r--   0 runner    (1001) docker     (123)   129389 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg500_2040.csv
--rw-r--r--   0 runner    (1001) docker     (123)   129388 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg500_2050.csv
--rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-NPi_2005.csv
--rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-NPi_2010.csv
--rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-NPi_2020.csv
--rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg1150_2005.csv
--rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg1150_2010.csv
--rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg1150_2020.csv
--rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg500_2005.csv
--rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg500_2010.csv
--rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg500_2020.csv
--rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_endpoint_static_ 3.8 cutoff.csv
--rw-r--r--   0 runner    (1001) docker     (123)   744503 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-NPi_2030.csv
--rw-r--r--   0 runner    (1001) docker     (123)   744505 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-NPi_2040.csv
--rw-r--r--   0 runner    (1001) docker     (123)   744507 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-NPi_2050.csv
--rw-r--r--   0 runner    (1001) docker     (123)   744503 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg1150_2030.csv
--rw-r--r--   0 runner    (1001) docker     (123)   744508 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg1150_2040.csv
--rw-r--r--   0 runner    (1001) docker     (123)   744510 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg1150_2050.csv
--rw-r--r--   0 runner    (1001) docker     (123)   744503 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg500_2030.csv
--rw-r--r--   0 runner    (1001) docker     (123)   744510 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg500_2040.csv
--rw-r--r--   0 runner    (1001) docker     (123)   744512 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg500_2050.csv
--rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-NPi_2005.csv
--rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-NPi_2010.csv
--rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-NPi_2020.csv
--rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg1150_2005.csv
--rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg1150_2010.csv
--rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg1150_2020.csv
--rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg500_2005.csv
--rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg500_2010.csv
--rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg500_2020.csv
--rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_midpoint_static_ 3.8 cutoff.csv
--rw-r--r--   0 runner    (1001) docker     (123)    94289 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/IAM/dict_inputs_A_matrix.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 20:56:14.729654 carculator_utils-1.0.4/carculator_utils/data/driving cycle/
--rw-r--r--   0 runner    (1001) docker     (123)   623589 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/driving cycle/bus.csv
--rw-r--r--   0 runner    (1001) docker     (123)   102616 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/driving cycle/car.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/driving cycle/dc_specs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)   392181 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/driving cycle/truck.csv
--rw-r--r--   0 runner    (1001) docker     (123)    63435 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/driving cycle/two-wheeler.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 20:56:14.729654 carculator_utils-1.0.4/carculator_utils/data/electricity/
--rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/electricity/cumulative_electricity_losses.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/electricity/elec_tech_map.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    98629 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/electricity/electricity_mixes.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 20:56:14.733654 carculator_utils-1.0.4/carculator_utils/data/emission_factors/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 20:56:14.733654 carculator_utils-1.0.4/carculator_utils/data/emission_factors/bus/
--rw-r--r--   0 runner    (1001) docker     (123)    81444 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/emission_factors/bus/EF_HBEFA42_exhaust.csv
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/emission_factors/bus/NMHC_species.csv
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/emission_factors/bus/degradation_EF.csv
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/emission_factors/bus/engine_wear.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/emission_factors/bus/propulsion_noise_coefficients.csv
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/emission_factors/bus/rolling_noise_coefficients.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 20:56:14.733654 carculator_utils-1.0.4/carculator_utils/data/emission_factors/car/
--rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/emission_factors/car/EF_HBEFA42_exhaust.csv
--rw-r--r--   0 runner    (1001) docker     (123)    28435 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/emission_factors/car/EF_HBEFA42_non_exhaust.csv
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/emission_factors/car/NMHC_species.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/emission_factors/car/degradation_EF.csv
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/emission_factors/car/engine_wear.csv
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/emission_factors/car/propulsion_noise_coefficients.csv
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/emission_factors/car/rolling_noise_coefficients.csv
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/emission_factors/euro_classes.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/emission_factors/exhaust_and_noise_flows.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/emission_factors/exhaust_flows.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/emission_factors/noise_flows.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 20:56:14.733654 carculator_utils-1.0.4/carculator_utils/data/emission_factors/truck/
--rw-r--r--   0 runner    (1001) docker     (123)    28747 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/emission_factors/truck/EF_HBEFA42_exhaust.csv
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/emission_factors/truck/NMHC_species.csv
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/emission_factors/truck/degradation_EF.csv
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/emission_factors/truck/engine_wear.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/emission_factors/truck/propulsion_noise_coefficients.csv
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/emission_factors/truck/rolling_noise_coefficients.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 20:56:14.737654 carculator_utils-1.0.4/carculator_utils/data/emission_factors/two-wheeler/
--rw-r--r--   0 runner    (1001) docker     (123)    12638 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/emission_factors/two-wheeler/EF_HBEFA42_exhaust.csv
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/emission_factors/two-wheeler/NMHC_species.csv
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/emission_factors/two-wheeler/engine_wear.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/emission_factors/two-wheeler/propulsion_noise_coefficients.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 20:56:14.745654 carculator_utils-1.0.4/carculator_utils/data/export/
--rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/export/ei37_to_ei35.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/export/ei37_to_ei36.csv
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/export/ei38_to_ei37.csv
--rw-r--r--   0 runner    (1001) docker     (123)   154654 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/export/references.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/export/rename_parameters.yml
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/export/rename_powertrains.yml
--rw-r--r--   0 runner    (1001) docker     (123)    57797 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/export/simapro-biosphere.json
--rw-r--r--   0 runner    (1001) docker     (123)  6503006 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/export/simapro-technosphere-3.5.csv
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/export/simapro_blacklist.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/export/simapro_fields.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 20:56:14.745654 carculator_utils-1.0.4/carculator_utils/data/fuel/
--rw-r--r--   0 runner    (1001) docker     (123)    14496 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/fuel/S_concentration_fuel.csv
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/fuel/default_fuels.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/fuel/fuel_specs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/fuel/share_bio_cng.csv
--rw-r--r--   0 runner    (1001) docker     (123)    14782 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/fuel/share_bio_diesel.csv
--rw-r--r--   0 runner    (1001) docker     (123)    14606 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/fuel/share_bio_gasoline.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 20:56:14.745654 carculator_utils-1.0.4/carculator_utils/data/gradient/
--rw-r--r--   0 runner    (1001) docker     (123)   751813 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/gradient/bus.csv
--rw-r--r--   0 runner    (1001) docker     (123)    71480 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/gradient/car.csv
--rw-r--r--   0 runner    (1001) docker     (123)   764385 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/gradient/truck.csv
--rw-r--r--   0 runner    (1001) docker     (123)    44045 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/gradient/two-wheeler.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 20:56:14.749654 carculator_utils-1.0.4/carculator_utils/data/lcia/
--rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/lcia/dict_impact_categories.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/lcia/impact_source_categories.yml
--rw-r--r--   0 runner    (1001) docker     (123)     8132 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/monthly_avg_temp.csv
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/data/purchase_cost_params.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/driving_cycles.py
--rw-r--r--   0 runner    (1001) docker     (123)    18130 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/energy_consumption.py
--rw-r--r--   0 runner    (1001) docker     (123)    42348 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/export.py
--rw-r--r--   0 runner    (1001) docker     (123)    17078 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/hot_emissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    68008 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)    51632 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9258 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/noise_emissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/particulates_emissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/carculator_utils/vehicle_input_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 20:56:14.689654 carculator_utils-1.0.4/carculator_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-02-10 20:56:14.000000 carculator_utils-1.0.4/carculator_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8796 2023-02-10 20:56:14.000000 carculator_utils-1.0.4/carculator_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-10 20:56:14.000000 carculator_utils-1.0.4/carculator_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-02-10 20:56:14.000000 carculator_utils-1.0.4/carculator_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-10 20:56:14.000000 carculator_utils-1.0.4/carculator_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-10 20:56:14.749654 carculator_utils-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 20:56:14.749654 carculator_utils-1.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-02-10 20:56:07.000000 carculator_utils-1.0.4/tests/test_vehicle_input_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:18:06.868886 carculator_utils-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-04-23 11:18:06.864886 carculator_utils-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:18:06.792886 carculator_utils-1.0.5/carculator_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13413 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/background_systems.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:18:06.792886 carculator_utils-1.0.5/carculator_utils/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:18:06.840886 carculator_utils-1.0.5/carculator_utils/data/IAM/
+-rw-r--r--   0 runner    (1001) docker     (123)    82764 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/A_matrix.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   614740 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-NPi_2030.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   614741 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-NPi_2040.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   614739 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-NPi_2050.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   614739 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg1150_2030.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   614741 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg1150_2040.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   614741 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg1150_2050.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   614739 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg500_2030.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   614741 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg500_2040.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   614741 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg500_2050.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-NPi_2005.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-NPi_2010.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-NPi_2020.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg1150_2005.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg1150_2010.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg1150_2020.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg500_2005.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg500_2010.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg500_2020.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_static_ 3.8 cutoff.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   129388 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-NPi_2030.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   129388 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-NPi_2040.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   129388 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-NPi_2050.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   129388 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg1150_2030.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   129389 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg1150_2040.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   129389 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg1150_2050.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   129389 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg500_2030.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   129389 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg500_2040.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   129388 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg500_2050.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-NPi_2005.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-NPi_2010.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-NPi_2020.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg1150_2005.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg1150_2010.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg1150_2020.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg500_2005.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg500_2010.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg500_2020.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint_static_ 3.8 cutoff.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   744503 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-NPi_2030.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   744505 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-NPi_2040.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   744507 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-NPi_2050.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   744503 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg1150_2030.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   744508 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg1150_2040.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   744510 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg1150_2050.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   744503 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg500_2030.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   744510 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg500_2040.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   744512 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg500_2050.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-NPi_2005.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-NPi_2010.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-NPi_2020.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg1150_2005.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg1150_2010.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg1150_2020.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg500_2005.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg500_2010.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg500_2020.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint_static_ 3.8 cutoff.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    94289 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/dict_inputs_A_matrix.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:18:06.844886 carculator_utils-1.0.5/carculator_utils/data/driving cycle/
+-rw-r--r--   0 runner    (1001) docker     (123)   623589 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/driving cycle/bus.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   102616 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/driving cycle/car.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/driving cycle/dc_specs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   392181 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/driving cycle/truck.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    63435 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/driving cycle/two-wheeler.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:18:06.844886 carculator_utils-1.0.5/carculator_utils/data/efficiency/
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/efficiency/bus.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    12959 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/efficiency/car.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/efficiency/truck.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:18:06.844886 carculator_utils-1.0.5/carculator_utils/data/electricity/
+-rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/electricity/cumulative_electricity_losses.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/electricity/elec_tech_map.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    98629 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/electricity/electricity_mixes.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:18:06.844886 carculator_utils-1.0.5/carculator_utils/data/emission_factors/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:18:06.848886 carculator_utils-1.0.5/carculator_utils/data/emission_factors/bus/
+-rw-r--r--   0 runner    (1001) docker     (123)    81444 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/emission_factors/bus/EF_HBEFA42_exhaust.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/emission_factors/bus/NMHC_species.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/emission_factors/bus/degradation_EF.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/emission_factors/bus/engine_wear.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/emission_factors/bus/propulsion_noise_coefficients.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/emission_factors/bus/rolling_noise_coefficients.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:18:06.848886 carculator_utils-1.0.5/carculator_utils/data/emission_factors/car/
+-rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/emission_factors/car/EF_HBEFA42_exhaust.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    28435 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/emission_factors/car/EF_HBEFA42_non_exhaust.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/emission_factors/car/NMHC_species.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/emission_factors/car/degradation_EF.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/emission_factors/car/engine_wear.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/emission_factors/car/propulsion_noise_coefficients.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/emission_factors/car/rolling_noise_coefficients.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/emission_factors/euro_classes.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/emission_factors/exhaust_and_noise_flows.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/emission_factors/exhaust_flows.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/emission_factors/noise_flows.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:18:06.848886 carculator_utils-1.0.5/carculator_utils/data/emission_factors/truck/
+-rw-r--r--   0 runner    (1001) docker     (123)    28747 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/emission_factors/truck/EF_HBEFA42_exhaust.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/emission_factors/truck/NMHC_species.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/emission_factors/truck/degradation_EF.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/emission_factors/truck/engine_wear.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/emission_factors/truck/propulsion_noise_coefficients.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/emission_factors/truck/rolling_noise_coefficients.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:18:06.852886 carculator_utils-1.0.5/carculator_utils/data/emission_factors/two-wheeler/
+-rw-r--r--   0 runner    (1001) docker     (123)    12638 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/emission_factors/two-wheeler/EF_HBEFA42_exhaust.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/emission_factors/two-wheeler/NMHC_species.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/emission_factors/two-wheeler/engine_wear.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/emission_factors/two-wheeler/propulsion_noise_coefficients.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:18:06.860886 carculator_utils-1.0.5/carculator_utils/data/export/
+-rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/export/ei37_to_ei35.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/export/ei37_to_ei36.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/export/ei38_to_ei37.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   154654 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/export/references.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/export/rename_parameters.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/export/rename_powertrains.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    57797 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/export/simapro-biosphere.json
+-rw-r--r--   0 runner    (1001) docker     (123)  6503006 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/export/simapro-technosphere-3.5.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/export/simapro_blacklist.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/export/simapro_fields.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:18:06.864886 carculator_utils-1.0.5/carculator_utils/data/fuel/
+-rw-r--r--   0 runner    (1001) docker     (123)    14496 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/fuel/S_concentration_fuel.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/fuel/default_fuels.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/fuel/fuel_specs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/fuel/share_bio_cng.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    14782 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/fuel/share_bio_diesel.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    14606 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/fuel/share_bio_gasoline.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:18:06.864886 carculator_utils-1.0.5/carculator_utils/data/gradient/
+-rw-r--r--   0 runner    (1001) docker     (123)   751813 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/gradient/bus.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    71480 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/gradient/car.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   764385 2023-04-23 11:17:53.000000 carculator_utils-1.0.5/carculator_utils/data/gradient/truck.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    44045 2023-04-23 11:17:53.000000 carculator_utils-1.0.5/carculator_utils/data/gradient/two-wheeler.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:18:06.864886 carculator_utils-1.0.5/carculator_utils/data/lcia/
+-rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-04-23 11:17:53.000000 carculator_utils-1.0.5/carculator_utils/data/lcia/dict_impact_categories.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-23 11:17:53.000000 carculator_utils-1.0.5/carculator_utils/data/lcia/impact_source_categories.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     8132 2023-04-23 11:17:53.000000 carculator_utils-1.0.5/carculator_utils/data/monthly_avg_temp.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-23 11:17:53.000000 carculator_utils-1.0.5/carculator_utils/data/purchase_cost_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-04-23 11:17:53.000000 carculator_utils-1.0.5/carculator_utils/driving_cycles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20712 2023-04-23 11:17:53.000000 carculator_utils-1.0.5/carculator_utils/energy_consumption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42445 2023-04-23 11:17:53.000000 carculator_utils-1.0.5/carculator_utils/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17078 2023-04-23 11:17:53.000000 carculator_utils-1.0.5/carculator_utils/hot_emissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68287 2023-04-23 11:17:53.000000 carculator_utils-1.0.5/carculator_utils/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51632 2023-04-23 11:17:53.000000 carculator_utils-1.0.5/carculator_utils/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9258 2023-04-23 11:17:53.000000 carculator_utils-1.0.5/carculator_utils/noise_emissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-04-23 11:17:53.000000 carculator_utils-1.0.5/carculator_utils/particulates_emissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-23 11:17:53.000000 carculator_utils-1.0.5/carculator_utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-04-23 11:17:53.000000 carculator_utils-1.0.5/carculator_utils/vehicle_input_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:18:06.792886 carculator_utils-1.0.5/carculator_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-04-23 11:18:06.000000 carculator_utils-1.0.5/carculator_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8924 2023-04-23 11:18:06.000000 carculator_utils-1.0.5/carculator_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 11:18:06.000000 carculator_utils-1.0.5/carculator_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-23 11:18:06.000000 carculator_utils-1.0.5/carculator_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-23 11:18:06.000000 carculator_utils-1.0.5/carculator_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-23 11:17:53.000000 carculator_utils-1.0.5/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-23 11:17:53.000000 carculator_utils-1.0.5/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-23 11:17:53.000000 carculator_utils-1.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 11:18:06.868886 carculator_utils-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-23 11:17:53.000000 carculator_utils-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:18:06.864886 carculator_utils-1.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-23 11:17:53.000000 carculator_utils-1.0.5/tests/test_vehicle_input_parameters.py
```

### Comparing `carculator_utils-1.0.4/CODE_OF_CONDUCT.md` & `carculator_utils-1.0.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/CONTRIBUTING.md` & `carculator_utils-1.0.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/LICENSE` & `carculator_utils-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/PKG-INFO` & `carculator_utils-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carculator_utils
-Version: 1.0.4
+Version: 1.0.5
 Summary: Provides convenience functions for carculator_utils
 Home-page: https://github.com/romainsacchi/carculator_utils
 Author: Romain Sacchi <romain.sacchi@psi.ch>
 License: BSD 3-Clause License
         
         Copyright (c) 2020, Paul Scherrer Institut
```

### Comparing `carculator_utils-1.0.4/README.md` & `carculator_utils-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/__init__.py` & `carculator_utils-1.0.5/carculator_utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "NoiseEmissionsModel",
     "HotEmissionsModel",
     "Inventory",
     "BackgroundSystemModel",
     "ExportInventory",
     "VehicleInputParameters",
 )
-__version__ = (1, 0, 4)
+__version__ = (1, 0, 5)
 
 from pathlib import Path
 
 DATA_DIR = Path(__file__).resolve().parent / "data"
 
 from .background_systems import BackgroundSystemModel
 from .driving_cycles import get_standard_driving_cycle_and_gradient
```

### Comparing `carculator_utils-1.0.4/carculator_utils/array.py` & `carculator_utils-1.0.5/carculator_utils/array.py`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/background_systems.py` & `carculator_utils-1.0.5/carculator_utils/background_systems.py`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/IAM/A_matrix.csv` & `carculator_utils-1.0.5/carculator_utils/data/IAM/A_matrix.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-NPi_2030.csv` & `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-NPi_2030.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-NPi_2040.csv` & `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-NPi_2040.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-NPi_2050.csv` & `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-NPi_2050.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg1150_2030.csv` & `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg1150_2030.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg1150_2040.csv` & `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg1150_2040.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg1150_2050.csv` & `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg1150_2050.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg500_2030.csv` & `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg500_2030.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg500_2040.csv` & `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg500_2040.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg500_2050.csv` & `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg500_2050.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-NPi_2005.csv` & `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-NPi_2005.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-NPi_2010.csv` & `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-NPi_2010.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-NPi_2020.csv` & `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-NPi_2020.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg1150_2005.csv` & `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg1150_2005.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg1150_2010.csv` & `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg1150_2010.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg1150_2020.csv` & `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg1150_2020.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg500_2005.csv` & `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg500_2005.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg500_2010.csv` & `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg500_2010.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg500_2020.csv` & `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg500_2020.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_static_ 3.8 cutoff.csv` & `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_static_ 3.8 cutoff.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-NPi_2030.csv` & `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-NPi_2030.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-NPi_2040.csv` & `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-NPi_2040.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-NPi_2050.csv` & `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-NPi_2050.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg1150_2030.csv` & `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg1150_2030.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg1150_2040.csv` & `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg1150_2040.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg1150_2050.csv` & `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg1150_2050.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg500_2030.csv` & `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg500_2030.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg500_2040.csv` & `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg500_2040.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg500_2050.csv` & `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg500_2050.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-NPi_2005.csv` & `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-NPi_2005.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-NPi_2010.csv` & `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-NPi_2010.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-NPi_2020.csv` & `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-NPi_2020.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg1150_2005.csv` & `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg1150_2005.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg1150_2010.csv` & `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg1150_2010.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg1150_2020.csv` & `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg1150_2020.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg500_2005.csv` & `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg500_2005.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg500_2010.csv` & `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg500_2010.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg500_2020.csv` & `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg500_2020.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_endpoint_static_ 3.8 cutoff.csv` & `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint_static_ 3.8 cutoff.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-NPi_2030.csv` & `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-NPi_2030.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-NPi_2040.csv` & `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-NPi_2040.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-NPi_2050.csv` & `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-NPi_2050.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg1150_2030.csv` & `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg1150_2030.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg1150_2040.csv` & `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg1150_2040.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg1150_2050.csv` & `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg1150_2050.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg500_2030.csv` & `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg500_2030.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg500_2040.csv` & `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg500_2040.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg500_2050.csv` & `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg500_2050.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-NPi_2005.csv` & `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-NPi_2005.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-NPi_2010.csv` & `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-NPi_2010.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-NPi_2020.csv` & `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-NPi_2020.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg1150_2005.csv` & `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg1150_2005.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg1150_2010.csv` & `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg1150_2010.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg1150_2020.csv` & `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg1150_2020.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg500_2005.csv` & `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg500_2005.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg500_2010.csv` & `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg500_2010.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg500_2020.csv` & `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg500_2020.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/IAM/B_matrix_recipe_midpoint_static_ 3.8 cutoff.csv` & `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint_static_ 3.8 cutoff.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/IAM/dict_inputs_A_matrix.csv` & `carculator_utils-1.0.5/carculator_utils/data/IAM/dict_inputs_A_matrix.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/driving cycle/bus.csv` & `carculator_utils-1.0.5/carculator_utils/data/driving cycle/bus.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/driving cycle/car.csv` & `carculator_utils-1.0.5/carculator_utils/data/driving cycle/car.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/driving cycle/dc_specs.yaml` & `carculator_utils-1.0.5/carculator_utils/data/driving cycle/dc_specs.yaml`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/driving cycle/truck.csv` & `carculator_utils-1.0.5/carculator_utils/data/driving cycle/truck.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/driving cycle/two-wheeler.csv` & `carculator_utils-1.0.5/carculator_utils/data/driving cycle/two-wheeler.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/electricity/cumulative_electricity_losses.csv` & `carculator_utils-1.0.5/carculator_utils/data/electricity/cumulative_electricity_losses.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/electricity/elec_tech_map.yaml` & `carculator_utils-1.0.5/carculator_utils/data/electricity/elec_tech_map.yaml`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/electricity/electricity_mixes.csv` & `carculator_utils-1.0.5/carculator_utils/data/electricity/electricity_mixes.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/emission_factors/bus/EF_HBEFA42_exhaust.csv` & `carculator_utils-1.0.5/carculator_utils/data/emission_factors/bus/EF_HBEFA42_exhaust.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/emission_factors/bus/propulsion_noise_coefficients.csv` & `carculator_utils-1.0.5/carculator_utils/data/emission_factors/bus/propulsion_noise_coefficients.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/emission_factors/bus/rolling_noise_coefficients.csv` & `carculator_utils-1.0.5/carculator_utils/data/emission_factors/bus/rolling_noise_coefficients.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/emission_factors/car/EF_HBEFA42_exhaust.csv` & `carculator_utils-1.0.5/carculator_utils/data/emission_factors/car/EF_HBEFA42_exhaust.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/emission_factors/car/EF_HBEFA42_non_exhaust.csv` & `carculator_utils-1.0.5/carculator_utils/data/emission_factors/car/EF_HBEFA42_non_exhaust.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/emission_factors/car/NMHC_species.csv` & `carculator_utils-1.0.5/carculator_utils/data/emission_factors/car/NMHC_species.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/emission_factors/car/degradation_EF.csv` & `carculator_utils-1.0.5/carculator_utils/data/emission_factors/car/degradation_EF.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/emission_factors/car/engine_wear.csv` & `carculator_utils-1.0.5/carculator_utils/data/emission_factors/car/engine_wear.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/emission_factors/euro_classes.yaml` & `carculator_utils-1.0.5/carculator_utils/data/emission_factors/euro_classes.yaml`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/emission_factors/exhaust_and_noise_flows.yaml` & `carculator_utils-1.0.5/carculator_utils/data/emission_factors/exhaust_and_noise_flows.yaml`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/emission_factors/exhaust_flows.yaml` & `carculator_utils-1.0.5/carculator_utils/data/emission_factors/exhaust_flows.yaml`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/emission_factors/noise_flows.yaml` & `carculator_utils-1.0.5/carculator_utils/data/emission_factors/noise_flows.yaml`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/emission_factors/truck/EF_HBEFA42_exhaust.csv` & `carculator_utils-1.0.5/carculator_utils/data/emission_factors/truck/EF_HBEFA42_exhaust.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/emission_factors/truck/propulsion_noise_coefficients.csv` & `carculator_utils-1.0.5/carculator_utils/data/emission_factors/truck/propulsion_noise_coefficients.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/emission_factors/truck/rolling_noise_coefficients.csv` & `carculator_utils-1.0.5/carculator_utils/data/emission_factors/truck/rolling_noise_coefficients.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/emission_factors/two-wheeler/EF_HBEFA42_exhaust.csv` & `carculator_utils-1.0.5/carculator_utils/data/emission_factors/two-wheeler/EF_HBEFA42_exhaust.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/emission_factors/two-wheeler/propulsion_noise_coefficients.csv` & `carculator_utils-1.0.5/carculator_utils/data/emission_factors/two-wheeler/propulsion_noise_coefficients.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/export/ei37_to_ei35.csv` & `carculator_utils-1.0.5/carculator_utils/data/export/ei37_to_ei35.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/export/ei37_to_ei36.csv` & `carculator_utils-1.0.5/carculator_utils/data/export/ei37_to_ei36.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/export/ei38_to_ei37.csv` & `carculator_utils-1.0.5/carculator_utils/data/export/ei38_to_ei37.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/export/references.csv` & `carculator_utils-1.0.5/carculator_utils/data/export/references.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/export/rename_parameters.yml` & `carculator_utils-1.0.5/carculator_utils/data/export/rename_parameters.yml`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/export/simapro-biosphere.json` & `carculator_utils-1.0.5/carculator_utils/data/export/simapro-biosphere.json`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/export/simapro-technosphere-3.5.csv` & `carculator_utils-1.0.5/carculator_utils/data/export/simapro-technosphere-3.5.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/export/simapro_fields.yml` & `carculator_utils-1.0.5/carculator_utils/data/export/simapro_fields.yml`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/fuel/S_concentration_fuel.csv` & `carculator_utils-1.0.5/carculator_utils/data/fuel/S_concentration_fuel.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/fuel/default_fuels.yaml` & `carculator_utils-1.0.5/carculator_utils/data/fuel/default_fuels.yaml`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/fuel/fuel_specs.yaml` & `carculator_utils-1.0.5/carculator_utils/data/fuel/fuel_specs.yaml`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/fuel/share_bio_cng.csv` & `carculator_utils-1.0.5/carculator_utils/data/fuel/share_bio_cng.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/fuel/share_bio_diesel.csv` & `carculator_utils-1.0.5/carculator_utils/data/fuel/share_bio_diesel.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/fuel/share_bio_gasoline.csv` & `carculator_utils-1.0.5/carculator_utils/data/fuel/share_bio_gasoline.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/gradient/bus.csv` & `carculator_utils-1.0.5/carculator_utils/data/gradient/bus.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/gradient/car.csv` & `carculator_utils-1.0.5/carculator_utils/data/gradient/car.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/gradient/truck.csv` & `carculator_utils-1.0.5/carculator_utils/data/gradient/truck.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/gradient/two-wheeler.csv` & `carculator_utils-1.0.5/carculator_utils/data/gradient/two-wheeler.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/lcia/dict_impact_categories.csv` & `carculator_utils-1.0.5/carculator_utils/data/lcia/dict_impact_categories.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/lcia/impact_source_categories.yml` & `carculator_utils-1.0.5/carculator_utils/data/lcia/impact_source_categories.yml`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/monthly_avg_temp.csv` & `carculator_utils-1.0.5/carculator_utils/data/monthly_avg_temp.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/data/purchase_cost_params.yaml` & `carculator_utils-1.0.5/carculator_utils/data/purchase_cost_params.yaml`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/driving_cycles.py` & `carculator_utils-1.0.5/carculator_utils/driving_cycles.py`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/energy_consumption.py` & `carculator_utils-1.0.5/carculator_utils/energy_consumption.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import csv
 from typing import Any, List, Tuple, Union
 
 import numexpr as ne
 import numpy as np
 import pandas as pd
 import xarray as xr
+import yaml
 from xarray import DataArray
 
 from . import DATA_DIR
 from .driving_cycles import (
     get_driving_cycle_specs,
     get_standard_driving_cycle_and_gradient,
 )
@@ -41,14 +42,81 @@
 
 
 def get_default_driving_cycle_name(vehicle_type) -> str:
     """Get the default driving cycle name"""
     return list(get_driving_cycle_specs()["columns"][vehicle_type].keys())[0]
 
 
+def get_efficiency_coefficients(vehicle_type: str) -> [Any, None]:
+    # load yaml file to retrieve efficiency coefficients
+
+    # if file does not exist, return None
+    if not (DATA_DIR / "efficiency" / f"{vehicle_type}.yaml").exists():
+        return None
+
+    with open(DATA_DIR / "efficiency" / f"{vehicle_type}.yaml") as f:
+        efficiency_coefficients = yaml.load(f, Loader=yaml.FullLoader)
+
+    return efficiency_coefficients
+
+
+def get_country_temperature(country):
+    """
+    Retrieves mothly average temperature
+    :type country: country for which to retrieve temperature values
+    :return:
+    """
+
+    with open(DATA_DIR / MONTHLY_AVG_TEMP) as f:
+        reader = csv.reader(f, delimiter=";")
+        for row in reader:
+            if row[2] == country:
+                return np.array([float(i) for i in row[3:]])
+
+    print(
+        f"Could not find monthly average temperature series for {country}. "
+        f"Uses those for CH instead."
+    )
+
+    with open(DATA_DIR / MONTHLY_AVG_TEMP) as f:
+        reader = csv.reader(f, delimiter=";")
+        for row in reader:
+            if row[2] == "CH":
+                return np.array([int(i) for i in row[3:]])
+
+
+def convert_to_xr(data):
+    return xr.DataArray(
+        data,
+        dims=["second", "value", "year", "powertrain", "size", "parameter"],
+        coords={
+            "second": range(0, data.shape[0]),
+            "value": range(0, data.shape[1]),
+            "year": range(0, data.shape[2]),
+            "powertrain": range(0, data.shape[3]),
+            "size": range(0, data.shape[4]),
+            "parameter": [
+                "rolling resistance",
+                "air resistance",
+                "gradient resistance",
+                "kinetic energy",
+                "motive energy at wheels",
+                "motive energy",
+                "negative motive energy",
+                "recuperated energy",
+                "power load",
+                "auxiliary energy",
+                "transmission efficiency",
+                "engine efficiency",
+                "velocity",
+            ],
+        },
+    )
+
+
 class EnergyConsumptionModel:
     """
     Calculate energy consumption of a vehicle for a
     given driving cycle and vehicle parameters.
 
     Based on a selected driving cycle, this class calculates
     the acceleration needed and provides
@@ -80,14 +148,15 @@
 
     """
 
     def __init__(
         self,
         vehicle_type: str,
         vehicle_size: List[str],
+        powertrains: List[str],
         cycle: Union[str, np.ndarray],
         gradient: Union[str, np.ndarray],
         rho_air: float = 1.204,
         country: str = "CH",
     ) -> None:
         if not isinstance(vehicle_size, list):
             vehicle_size = [vehicle_size]
@@ -108,14 +177,15 @@
             self.cycle, self.gradient = get_standard_driving_cycle_and_gradient(
                 vehicle_type, vehicle_size, self.cycle_name
             )
 
         self.country = country
         self.vehicle_type = vehicle_type
         self.vehicle_size = vehicle_size
+        self.powertrains = powertrains
 
         if "Micro" in vehicle_size:
             idx = vehicle_size.index("Micro")
             self.cycle[:, idx] = np.clip(self.cycle[:, idx], 0, 90)
 
         assert len(self.cycle) == len(
             self.gradient
@@ -127,50 +197,28 @@
 
         # Model acceleration as difference in velocity between
         # time steps (1 second)
         # Zero at first value
         self.acceleration = np.zeros_like(self.velocity)
         self.acceleration[1:-1] = (self.velocity[2:, ...] - self.velocity[:-2, ...]) / 2
 
-    def get_country_temperature(self, country):
-        """
-        Retrieves mothly average temperature
-        :type country: country for which to retrieve temperature values
-        :return:
-        """
-
-        with open(DATA_DIR / MONTHLY_AVG_TEMP) as f:
-            reader = csv.reader(f, delimiter=";")
-            for row in reader:
-                if row[2] == country:
-                    return np.array([float(i) for i in row[3:]])
-
-        print(
-            f"Could not find monthly average temperature series for {country}. "
-            f"Uses those for CH instead."
-        )
-
-        with open(DATA_DIR / MONTHLY_AVG_TEMP) as f:
-            reader = csv.reader(f, delimiter=";")
-            for row in reader:
-                if row[2] == "CH":
-                    return np.array([int(i) for i in row[3:]])
+        self.efficiency_coefficients = get_efficiency_coefficients(vehicle_type)
 
     def calculate_hvac_energy(
         self,
         hvac_power,
         battery_cooling_unit,
         battery_heating_unit,
         ambient_temp,
         indoor_temp,
     ) -> tuple[Any, Any, Any, Any]:
         if ambient_temp is not None:
             ambient_temp = np.resize(ambient_temp, (12,))
         else:
-            ambient_temp = self.get_country_temperature(self.country)
+            ambient_temp = get_country_temperature(self.country)
 
         # use ambient temperature if provided, otherwise
         # monthly temperature average (12 values)
         # relation between ambient temperature
         # and HVAC power required
         # from https://doi.org/10.1016/j.energy.2018.12.064
         amb_temp_data_points = np.array([-30, -20, -10, 0, 10, 20, 30, 40])
@@ -268,61 +316,83 @@
         auxiliary_energy = (
             _c(aux_power).T[None, ...]  # Watts
             * np.ones_like(self.velocity)
             * 1000  # m / km
             / 1000  # 1 / (J / kJ)
         )
 
-        efficiency = _c(efficiency)[..., None]
-        efficiency[efficiency == 0] = 1
+        efficiency = _c(efficiency)
 
-        return auxiliary_energy / _o(efficiency).T
+        return auxiliary_energy / _o(efficiency)
 
-    def convert_to_xr(self, data):
-        return xr.DataArray(
-            data,
-            dims=["second", "value", "year", "powertrain", "size", "parameter"],
-            coords={
-                "second": range(0, data.shape[0]),
-                "value": range(0, data.shape[1]),
-                "year": range(0, data.shape[2]),
-                "powertrain": range(0, data.shape[3]),
-                "size": range(0, data.shape[4]),
-                "parameter": [
-                    "rolling resistance",
-                    "air resistance",
-                    "gradient resistance",
-                    "kinetic energy",
-                    "motive energy at wheels",
-                    "motive energy",
-                    "negative motive energy",
-                    "recuperated energy",
-                    "power load",
-                    "auxiliary energy",
-                    "transmission efficiency",
-                    "engine efficiency",
-                    "velocity",
-                ],
-            },
-        )
+    def calculate_efficiency(
+        self,
+        efficiency: xr.DataArray,
+        engine_load: xr.DataArray,
+        efficiency_type: str,
+    ) -> xr.DataArray:
+        if self.efficiency_coefficients is None:
+            return xr.where(efficiency == 0, 1, efficiency)
+
+        # Calculate efficiency based on engine load
+        pwts = {
+            "ICEV-p": "gasoline",
+            "ICEV-d": "diesel",
+            "HEV-p": "gasoline",
+            "HEV-d": "diesel",
+            "ICEV-g": "compressed gas",
+            "PHEV-c-p": "gasoline",
+            "PHEV-c-d": "diesel",
+            "BEV": "electric",
+            "BEV-depot": "electric",
+            "BEV-opp": "electric",
+            "BEV-motion": "electric",
+            "PHEV-e": "electric",
+            "FCEV": "electric",
+        }
+
+        # Calculate efficiency based on engine load
+        for p, pwt in enumerate(self.powertrains):
+            if pwt not in pwts:
+                continue
+
+            efficiency[:, :, :, p] = np.clip(
+                np.interp(
+                    engine_load[:, :, :, p],
+                    np.fromiter(
+                        self.efficiency_coefficients[pwts[pwt]][efficiency_type].keys(),
+                        dtype=float,
+                    ),
+                    np.fromiter(
+                        self.efficiency_coefficients[pwts[pwt]][
+                            efficiency_type
+                        ].values(),
+                        dtype=float,
+                    ),
+                ),
+                0.00,
+                1.0,
+            )
+
+        return efficiency
 
     def motive_energy_per_km(
         self,
         driving_mass: Union[xr.DataArray, np.array],
         rr_coef: Union[xr.DataArray, np.array],
         drag_coef: Union[xr.DataArray, np.array],
         frontal_area: Union[xr.DataArray, np.array],
         electric_motor_power: Union[xr.DataArray, np.array],
         engine_power: Union[xr.DataArray, np.array],
         recuperation_efficiency: Union[xr.DataArray, np.array],
         aux_power: Union[xr.DataArray, np.array],
-        engine_efficiency: Union[xr.DataArray, np.array],
-        transmission_efficiency: Union[xr.DataArray, np.array],
         battery_charge_eff: Union[xr.DataArray, np.array],
         battery_discharge_eff: Union[xr.DataArray, np.array],
+        engine_efficiency: Union[xr.DataArray, np.array, None] = None,
+        transmission_efficiency: Union[xr.DataArray, np.array, None] = None,
         fuel_cell_system_efficiency: Union[xr.DataArray, np.array] = None,
         hvac_power: Union[xr.DataArray, np.array] = None,
         battery_cooling_unit: Union[xr.DataArray, np.array] = None,
         battery_heating_unit: Union[xr.DataArray, np.array] = None,
         heat_pump_cop_cooling: Union[xr.DataArray, np.array] = None,
         heat_pump_cop_heating: Union[xr.DataArray, np.array] = None,
         cooling_consumption: Union[xr.DataArray, np.array] = None,
@@ -365,60 +435,82 @@
         _c = lambda x: x.values if isinstance(x, xr.DataArray) else x
         _o = lambda x: np.where((x == 0) | (x == np.nan), 1, x)
 
         # Calculate the energy used for each second of the drive cycle
         ones = np.ones_like(self.velocity)
 
         # Resistance from the tire rolling: rolling resistance coefficient * driving mass * 9.81
-        rolling_resistance = _c((driving_mass * rr_coef * 9.81).T) * ones
+        rolling_resistance = _c((driving_mass * rr_coef * 9.81).T) * (self.velocity > 0)
 
         # Resistance from the drag: frontal area * drag coefficient * air density * 1/2 * velocity^2
         air_resistance = _c((frontal_area * drag_coef * self.rho_air / 2).T) * np.power(
             self.velocity, 2
         )
 
         # Resistance from road gradient: driving mass * 9.81 * sin(gradient)
-        gradient_resistance = _c((driving_mass * 9.81).T) * np.sin(
-            np.nan_to_num(self.gradient)[:, None, None, None, :]
+        gradient_resistance = (
+            _c((driving_mass * 9.81).T)
+            * np.sin(np.nan_to_num(self.gradient)[:, None, None, None, :])
+            * (self.velocity > 0)
         )
 
         # Inertia: driving mass * acceleration
         inertia = self.acceleration * _c(driving_mass).T
 
         total_resistance = (
             rolling_resistance + air_resistance + gradient_resistance + inertia
         )
+        motive_energy_at_wheels = xr.where(total_resistance < 0, 0, total_resistance)
+        motive_energy = np.zeros_like(motive_energy_at_wheels)
 
-        engine_power = xr.where(engine_power == 0, 1, engine_power)
-        engine_efficiency = xr.where(engine_efficiency == 0, 1, engine_efficiency)
-        transmission_efficiency = xr.where(
-            transmission_efficiency == 0, 1, transmission_efficiency
-        )
-        recuperation_efficiency = xr.where(
-            recuperation_efficiency == 0, 1, recuperation_efficiency
-        )
+        # determining efficiencies
+        engine_load = np.ones_like(motive_energy_at_wheels)
 
-        if fuel_cell_system_efficiency is None:
-            fuel_cell_system_efficiency = np.array([1.0])
+        if engine_efficiency is None:
+            engine_efficiency = np.ones_like(motive_energy_at_wheels)
 
-        fuel_cell_system_efficiency = xr.where(
-            fuel_cell_system_efficiency == 0, 1, fuel_cell_system_efficiency
-        )
+        if transmission_efficiency is None:
+            transmission_efficiency = np.ones_like(motive_energy_at_wheels)
 
-        motive_energy_at_wheels = xr.where(total_resistance < 0, 0, total_resistance)
+        engine_load_iterations = [0, engine_load.mean()]
 
-        if fuel_cell_system_efficiency is None:
-            fuel_cell_system_efficiency = np.array([1.0])
+        # we loop while the last three iterations are roughly equal
+        # or while len(engine_load_iterations) < 10
 
-        motive_energy = (
-            motive_energy_at_wheels
-            / _o(_c(engine_efficiency.T))[None, ...]
-            / _o(_c(transmission_efficiency.T))[None, ...]
-            / _o(_c(fuel_cell_system_efficiency.T))[None, ...]
-        )
+        while len(engine_load_iterations) < 5:
+            engine_efficiency = self.calculate_efficiency(
+                engine_efficiency, engine_load, "engine"
+            )
+
+            transmission_efficiency = self.calculate_efficiency(
+                transmission_efficiency, engine_load, "transmission"
+            )
+
+            recuperation_efficiency = xr.where(
+                recuperation_efficiency == 0, 1, recuperation_efficiency
+            )
+
+            if fuel_cell_system_efficiency is None:
+                fuel_cell_system_efficiency = np.array([1.0])
+
+            fuel_cell_system_efficiency = xr.where(
+                fuel_cell_system_efficiency == 0, 1, fuel_cell_system_efficiency
+            )
+
+            motive_energy = (
+                motive_energy_at_wheels
+                / _o(_c(engine_efficiency))
+                / _o(_c(transmission_efficiency))
+                / _o(_c(fuel_cell_system_efficiency)).T[None, ...]
+            )
+
+            engine_load = np.clip(
+                (motive_energy / (_o(_c(engine_power)).T * 1000)) * self.velocity, 0, 1
+            )
+            engine_load_iterations.append(engine_load.mean())
 
         negative_motive_energy = xr.where(total_resistance > 0, 0, total_resistance)
         recuperated_energy = (
             negative_motive_energy
             * _c(recuperation_efficiency).T[None, ...]
             * _c(battery_charge_eff).T[None, ...]
             * _c(battery_discharge_eff).T[None, ...]
@@ -446,27 +538,27 @@
                 _(air_resistance),
                 _(gradient_resistance),
                 _(inertia),
                 _(motive_energy_at_wheels),
                 _(motive_energy),
                 _(negative_motive_energy),
                 _(recuperated_energy),
-                _((motive_energy + recuperated_energy) / (_c(engine_power).T * 1000)),
+                _(engine_load),
                 _(auxiliary_energy),
-                _(__(_c(transmission_efficiency).T) * np.ones_like(motive_energy)),
-                _(__(_c(engine_efficiency).T) * np.ones_like(motive_energy)),
+                _(transmission_efficiency),
+                _(engine_efficiency),
                 _(self.velocity * np.ones_like(motive_energy)),
             ],
             axis=-1,
         )
 
         all_arrays[..., :-5] /= 1000
         all_arrays[..., -4] /= 1000
         all_arrays[..., :-5] *= _(self.velocity)
-        all_arrays[..., -5] = np.clip(all_arrays[..., -5], 0, 1)
+
         all_arrays[..., 4] = np.where(
             all_arrays[..., 4] > _(engine_power).T,
             _(engine_power).T,
             all_arrays[..., 4],
         )
         all_arrays[..., 5] = np.where(
             all_arrays[..., 5] > _(engine_power).T,
@@ -475,8 +567,8 @@
         )
         all_arrays[..., 7] = np.where(
             all_arrays[..., 7] < _(electric_motor_power).T * -1,
             _(electric_motor_power).T * -1,
             all_arrays[..., 7],
         )
 
-        return self.convert_to_xr(all_arrays).fillna(0)
+        return convert_to_xr(all_arrays).fillna(0)
```

### Comparing `carculator_utils-1.0.4/carculator_utils/export.py` & `carculator_utils-1.0.5/carculator_utils/export.py`

 * *Files 0% similar despite different names*

```diff
@@ -961,14 +961,15 @@
         return os.path.join(directory, filename)
 
     def write_simapro_lci(
         self,
         ecoinvent_version: str,
         directory: str = None,
         filename: str = None,
+        export_format: str = "file",
     ):
         filename = filename or safe_filename(
             f"carculator_export_{datetime.date.today()}"
         )
 
         filename += "_simapro.csv"
 
@@ -978,20 +979,21 @@
             ecoinvent_version=ecoinvent_version,
         )
 
         rows = self.format_data_for_lci_for_simapro(
             data=list_act, ei_version=ecoinvent_version
         )
 
-        with open(filepath_export, "w", newline="", encoding="latin1") as csvFile:
-            writer = csv.writer(csvFile, delimiter=";")
-            for row in rows:
-                writer.writerow(row)
-        csvFile.close()
-        return filepath_export
+        if export_format == "file":
+            with open(filepath_export, "w", newline="", encoding="latin1") as csvFile:
+                writer = csv.writer(csvFile, delimiter=";")
+                for row in rows:
+                    writer.writerow(row)
+            csvFile.close()
+            return filepath_export
 
         # string format
         csvFile = io.StringIO()
         writer = csv.writer(
             csvFile,
             delimiter=";",
             quoting=csv.QUOTE_NONE,
```

### Comparing `carculator_utils-1.0.4/carculator_utils/hot_emissions.py` & `carculator_utils-1.0.5/carculator_utils/hot_emissions.py`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/inventory.py` & `carculator_utils-1.0.5/carculator_utils/inventory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1891,14 +1891,18 @@
         software="brightway2",
         format="bw2io",
     ):
         """
         Export the inventory. Can export to Simapro (as csv), or brightway2 (as bw2io object, file or string).
         :param db_name:
         :param ecoinvent_version: str. "3.5", "3.6", "3.7" or "3.8"
+        :param filename: str. Name of the file to be exported
+        :param directory: str. Directory where the file is saved
+        :param software: str. "brightway2" or "simapro"
+        :param format: str. "bw2io" or "file" or "string"
         ::return: inventory, or the filepath where the file is saved.
         :rtype: list
         """
 
         if self.func_unit != "vkm":
             self.change_functional_unit()
 
@@ -1918,8 +1922,9 @@
             )
 
         else:
             return lci.write_simapro_lci(
                 ecoinvent_version=ecoinvent_version,
                 directory=directory,
                 filename=filename,
+                export_format=format,
             )
```

### Comparing `carculator_utils-1.0.4/carculator_utils/model.py` & `carculator_utils-1.0.5/carculator_utils/model.py`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/noise_emissions.py` & `carculator_utils-1.0.5/carculator_utils/noise_emissions.py`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/particulates_emissions.py` & `carculator_utils-1.0.5/carculator_utils/particulates_emissions.py`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils/vehicle_input_parameters.py` & `carculator_utils-1.0.5/carculator_utils/vehicle_input_parameters.py`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/carculator_utils.egg-info/PKG-INFO` & `carculator_utils-1.0.5/carculator_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carculator-utils
-Version: 1.0.4
+Version: 1.0.5
 Summary: Provides convenience functions for carculator_utils
 Home-page: https://github.com/romainsacchi/carculator_utils
 Author: Romain Sacchi <romain.sacchi@psi.ch>
 License: BSD 3-Clause License
         
         Copyright (c) 2020, Paul Scherrer Institut
```

### Comparing `carculator_utils-1.0.4/carculator_utils.egg-info/SOURCES.txt` & `carculator_utils-1.0.5/carculator_utils.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -87,14 +87,17 @@
 carculator_utils/data/IAM/B_matrix_recipe_midpoint_static_ 3.8 cutoff.csv
 carculator_utils/data/IAM/dict_inputs_A_matrix.csv
 carculator_utils/data/driving cycle/bus.csv
 carculator_utils/data/driving cycle/car.csv
 carculator_utils/data/driving cycle/dc_specs.yaml
 carculator_utils/data/driving cycle/truck.csv
 carculator_utils/data/driving cycle/two-wheeler.csv
+carculator_utils/data/efficiency/bus.yaml
+carculator_utils/data/efficiency/car.yaml
+carculator_utils/data/efficiency/truck.yaml
 carculator_utils/data/electricity/cumulative_electricity_losses.csv
 carculator_utils/data/electricity/elec_tech_map.yaml
 carculator_utils/data/electricity/electricity_mixes.csv
 carculator_utils/data/emission_factors/euro_classes.yaml
 carculator_utils/data/emission_factors/exhaust_and_noise_flows.yaml
 carculator_utils/data/emission_factors/exhaust_flows.yaml
 carculator_utils/data/emission_factors/noise_flows.yaml
```

### Comparing `carculator_utils-1.0.4/readthedocs.yml` & `carculator_utils-1.0.5/readthedocs.yml`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.4/setup.py` & `carculator_utils-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="carculator_utils",
-    version="1.0.4",
+    version="1.0.5",
     packages=packages,
     author="Romain Sacchi <romain.sacchi@psi.ch>",
     python_requires=">=3.9",
     license=open("LICENSE").read(),
     package_data={
         "carculator_utils": package_files(os.path.join("carculator_utils", "data"))
     },
```

### Comparing `carculator_utils-1.0.4/tests/test_vehicle_input_parameters.py` & `carculator_utils-1.0.5/tests/test_vehicle_input_parameters.py`

 * *Files identical despite different names*

