# Comparing `tmp/mobspy-2.0.2.tar.gz` & `tmp/mobspy-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mobspy-2.0.2.tar", last modified: Thu Apr 20 10:34:06 2023, max compression
+gzip compressed data, was "mobspy-2.0.3.tar", last modified: Sun Apr 23 19:15:42 2023, max compression
```

## Comparing `mobspy-2.0.2.tar` & `mobspy-2.0.3.tar`

### file list

```diff
@@ -1,125 +1,128 @@
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-20 10:34:06.850224 mobspy-2.0.2/
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-20 10:34:06.696133 mobspy-2.0.2/.github/
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-20 10:34:06.704212 mobspy-2.0.2/.github/workflows/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1201 2023-04-03 11:45:17.000000 mobspy-2.0.2/.github/workflows/python-app.yml
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      265 2023-04-05 11:22:48.000000 mobspy-2.0.2/.gitignore
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1068 2023-03-26 13:05:39.000000 mobspy-2.0.2/LICENSE
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     7015 2023-04-20 10:34:06.849565 mobspy-2.0.2/PKG-INFO
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5825 2023-03-29 14:16:39.000000 mobspy-2.0.2/README.md
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-20 10:34:06.696455 mobspy-2.0.2/example_models/
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-20 10:34:06.714243 mobspy-2.0.2/example_models/application_models/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      573 2023-03-26 13:05:39.000000 mobspy-2.0.2/example_models/application_models/AB_2CD.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1446 2023-03-26 13:05:39.000000 mobspy-2.0.2/example_models/application_models/AND_gate.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2653 2023-03-26 13:05:39.000000 mobspy-2.0.2/example_models/application_models/CRISPR_Oscillator.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1435 2023-04-18 11:26:50.000000 mobspy-2.0.2/example_models/application_models/For_The_Trees.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1297 2023-03-31 13:18:09.000000 mobspy-2.0.2/example_models/application_models/NOR_gate.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1244 2023-03-26 13:05:39.000000 mobspy-2.0.2/example_models/application_models/donor_receptor.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1372 2023-03-26 13:05:39.000000 mobspy-2.0.2/example_models/application_models/oscillator.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2901 2023-04-18 11:26:50.000000 mobspy-2.0.2/example_models/application_models/random_walk.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      565 2023-03-26 13:05:39.000000 mobspy-2.0.2/example_models/application_models/simple_repressor.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     3855 2023-03-26 13:05:39.000000 mobspy-2.0.2/example_models/application_models/toggle_switch.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-20 10:34:06.737946 mobspy-2.0.2/example_models/tutorial_models/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1602 2023-03-26 13:05:39.000000 mobspy-2.0.2/example_models/tutorial_models/01_Getting_Started.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1863 2023-03-26 13:05:39.000000 mobspy-2.0.2/example_models/tutorial_models/02_Reaction_Inheritance.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1013 2023-03-26 13:05:39.000000 mobspy-2.0.2/example_models/tutorial_models/02_Reaction_Inheritance_Model.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1769 2023-03-26 13:05:39.000000 mobspy-2.0.2/example_models/tutorial_models/03_Queries.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      946 2023-03-26 13:05:39.000000 mobspy-2.0.2/example_models/tutorial_models/03_Queries.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      989 2023-03-26 13:05:39.000000 mobspy-2.0.2/example_models/tutorial_models/04_Characteristic_Restriction.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1121 2023-03-31 13:18:09.000000 mobspy-2.0.2/example_models/tutorial_models/05_C_Query.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2284 2023-03-31 13:18:09.000000 mobspy-2.0.2/example_models/tutorial_models/06_Round_Robin.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2255 2023-03-26 13:05:39.000000 mobspy-2.0.2/example_models/tutorial_models/07_Rates.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2125 2023-03-31 13:18:09.000000 mobspy-2.0.2/example_models/tutorial_models/08_Units.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      866 2023-03-26 13:05:39.000000 mobspy-2.0.2/example_models/tutorial_models/09_Count_Assignment.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1042 2023-03-26 13:05:39.000000 mobspy-2.0.2/example_models/tutorial_models/09_Count_Assignment.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1589 2023-03-26 13:05:39.000000 mobspy-2.0.2/example_models/tutorial_models/10_Species_Loop.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2074 2023-03-26 13:05:39.000000 mobspy-2.0.2/example_models/tutorial_models/11_Results.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2128 2023-03-26 13:05:39.000000 mobspy-2.0.2/example_models/tutorial_models/12_Hierarchical_plot.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      982 2023-03-26 13:05:39.000000 mobspy-2.0.2/example_models/tutorial_models/13_Born_Species.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      596 2023-04-20 10:30:16.000000 mobspy-2.0.2/for_local_use.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-20 10:34:06.738959 mobspy-2.0.2/images/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    18566 2023-03-26 13:05:39.000000 mobspy-2.0.2/images/img.png
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-20 10:34:06.742895 mobspy-2.0.2/mobspy/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       95 2023-03-26 13:05:39.000000 mobspy-2.0.2/mobspy/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       22 2023-04-20 10:31:23.000000 mobspy-2.0.2/mobspy/_version.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-20 10:34:06.749383 mobspy-2.0.2/mobspy/data_handler/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-03-26 13:05:39.000000 mobspy-2.0.2/mobspy/data_handler/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2207 2023-04-05 18:57:56.000000 mobspy-2.0.2/mobspy/data_handler/process_result_data.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5972 2023-04-20 09:08:12.000000 mobspy-2.0.2/mobspy/data_handler/time_series_object.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-20 10:34:06.765722 mobspy-2.0.2/mobspy/modules/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-03-26 13:05:39.000000 mobspy-2.0.2/mobspy/modules/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4355 2023-04-17 14:42:37.000000 mobspy-2.0.2/mobspy/modules/event_functions.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    12456 2023-04-18 20:56:31.000000 mobspy-2.0.2/mobspy/modules/function_rate_code.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    12663 2023-04-12 21:11:32.000000 mobspy-2.0.2/mobspy/modules/logic_operator_objects.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    57088 2023-04-18 20:51:04.000000 mobspy-2.0.2/mobspy/modules/meta_class.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5239 2023-04-13 11:40:51.000000 mobspy-2.0.2/mobspy/modules/meta_class_utils.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    14961 2023-04-13 12:13:54.000000 mobspy-2.0.2/mobspy/modules/order_operators.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    16482 2023-04-13 12:24:44.000000 mobspy-2.0.2/mobspy/modules/reaction_construction_nb.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     3988 2023-04-17 11:11:45.000000 mobspy-2.0.2/mobspy/modules/set_counts_module.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4143 2023-04-11 11:59:50.000000 mobspy-2.0.2/mobspy/modules/species_string_generator.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6615 2023-04-18 21:25:28.000000 mobspy-2.0.2/mobspy/modules/unit_handler.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-20 10:34:06.768335 mobspy-2.0.2/mobspy/parameter_scripts/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-03-26 13:05:39.000000 mobspy-2.0.2/mobspy/parameter_scripts/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2211 2023-04-07 15:35:28.000000 mobspy-2.0.2/mobspy/parameter_scripts/parameter_reader.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-20 10:34:06.775603 mobspy-2.0.2/mobspy/parameters/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1463 2023-03-26 13:05:39.000000 mobspy-2.0.2/mobspy/parameters/README.md
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-03-26 13:05:39.000000 mobspy-2.0.2/mobspy/parameters/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1035 2023-03-28 13:07:30.000000 mobspy-2.0.2/mobspy/parameters/default_reader.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1117 2023-04-07 15:35:28.000000 mobspy-2.0.2/mobspy/parameters/example_reader.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-20 10:34:06.778128 mobspy-2.0.2/mobspy/plot_params/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-03-26 13:05:39.000000 mobspy-2.0.2/mobspy/plot_params/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      184 2023-03-26 13:05:39.000000 mobspy-2.0.2/mobspy/plot_params/default_plot_reader.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1232 2023-03-26 13:05:39.000000 mobspy-2.0.2/mobspy/plot_params/example_plot_reader.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-20 10:34:06.782813 mobspy-2.0.2/mobspy/plot_scripts/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-03-26 13:05:39.000000 mobspy-2.0.2/mobspy/plot_scripts/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6445 2023-04-19 11:27:03.000000 mobspy-2.0.2/mobspy/plot_scripts/default_plots.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    14387 2023-04-17 13:43:18.000000 mobspy-2.0.2/mobspy/plot_scripts/hierarchical_plot.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1846 2023-04-20 09:16:42.000000 mobspy-2.0.2/mobspy/plot_scripts/process_plot_data.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     3566 2023-04-20 08:51:56.000000 mobspy-2.0.2/mobspy/plot_scripts/statistics_calculations.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-20 10:34:06.787807 mobspy-2.0.2/mobspy/sbml_simulator/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8118 2023-04-08 16:53:54.000000 mobspy-2.0.2/mobspy/sbml_simulator/SBMLWriter.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-03-26 13:05:39.000000 mobspy-2.0.2/mobspy/sbml_simulator/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      936 2023-04-08 16:40:14.000000 mobspy-2.0.2/mobspy/sbml_simulator/builder.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    12536 2023-04-17 15:49:48.000000 mobspy-2.0.2/mobspy/sbml_simulator/run.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    26192 2023-04-19 08:48:20.000000 mobspy-2.0.2/mobspy/simulation.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-20 10:34:06.789705 mobspy-2.0.2/mobspy/simulation_logging/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-03-26 13:05:39.000000 mobspy-2.0.2/mobspy/simulation_logging/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1013 2023-04-13 12:13:25.000000 mobspy-2.0.2/mobspy/simulation_logging/log_scripts.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-20 10:34:06.747010 mobspy-2.0.2/mobspy.egg-info/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     7015 2023-04-20 10:34:06.000000 mobspy-2.0.2/mobspy.egg-info/PKG-INFO
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     3563 2023-04-20 10:34:06.000000 mobspy-2.0.2/mobspy.egg-info/SOURCES.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        1 2023-04-20 10:34:06.000000 mobspy-2.0.2/mobspy.egg-info/dependency_links.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       76 2023-04-20 10:34:06.000000 mobspy-2.0.2/mobspy.egg-info/requires.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        7 2023-04-20 10:34:06.000000 mobspy-2.0.2/mobspy.egg-info/top_level.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       77 2023-03-26 13:05:39.000000 mobspy-2.0.2/requirements.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       38 2023-04-20 10:34:06.850385 mobspy-2.0.2/setup.cfg
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      767 2023-03-26 13:05:39.000000 mobspy-2.0.2/setup.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    18793 2023-04-18 21:34:52.000000 mobspy-2.0.2/test_script.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-20 10:34:06.848113 mobspy-2.0.2/test_tools/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      170 2023-03-26 13:05:39.000000 mobspy-2.0.2/test_tools/model_1.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      239 2023-03-28 14:54:04.000000 mobspy-2.0.2/test_tools/model_10.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      299 2023-03-29 10:35:15.000000 mobspy-2.0.2/test_tools/model_11.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      393 2023-03-31 14:53:54.000000 mobspy-2.0.2/test_tools/model_12.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      490 2023-03-31 16:58:04.000000 mobspy-2.0.2/test_tools/model_13.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      487 2023-03-31 17:23:20.000000 mobspy-2.0.2/test_tools/model_14.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      550 2023-04-03 08:42:24.000000 mobspy-2.0.2/test_tools/model_15.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      286 2023-04-04 18:39:28.000000 mobspy-2.0.2/test_tools/model_16.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      273 2023-04-05 14:12:52.000000 mobspy-2.0.2/test_tools/model_17.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      118 2023-04-06 11:09:14.000000 mobspy-2.0.2/test_tools/model_18.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      970 2023-04-06 13:23:26.000000 mobspy-2.0.2/test_tools/model_19.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      396 2023-03-26 13:05:39.000000 mobspy-2.0.2/test_tools/model_2.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      326 2023-04-06 13:24:46.000000 mobspy-2.0.2/test_tools/model_20.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1453 2023-04-11 12:17:19.000000 mobspy-2.0.2/test_tools/model_21.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      435 2023-04-11 15:31:51.000000 mobspy-2.0.2/test_tools/model_22.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      186 2023-04-12 16:26:56.000000 mobspy-2.0.2/test_tools/model_23.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      605 2023-04-17 14:45:24.000000 mobspy-2.0.2/test_tools/model_24.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       81 2023-04-18 11:30:58.000000 mobspy-2.0.2/test_tools/model_25.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      507 2023-04-18 20:45:48.000000 mobspy-2.0.2/test_tools/model_26.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      145 2023-04-18 21:30:11.000000 mobspy-2.0.2/test_tools/model_27.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     3154 2023-03-26 13:05:39.000000 mobspy-2.0.2/test_tools/model_3.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      727 2023-03-26 13:05:39.000000 mobspy-2.0.2/test_tools/model_4.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      559 2023-03-26 13:05:39.000000 mobspy-2.0.2/test_tools/model_5.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      353 2023-03-26 13:05:39.000000 mobspy-2.0.2/test_tools/model_6.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1352 2023-03-26 13:05:39.000000 mobspy-2.0.2/test_tools/model_7.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      443 2023-03-28 21:23:58.000000 mobspy-2.0.2/test_tools/model_8.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      736 2023-03-28 08:26:08.000000 mobspy-2.0.2/test_tools/model_9.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       60 2023-03-26 13:05:39.000000 mobspy-2.0.2/useful_parameters.json
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-23 19:15:42.269219 mobspy-2.0.3/
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-23 19:15:42.147516 mobspy-2.0.3/.github/
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-23 19:15:42.158559 mobspy-2.0.3/.github/workflows/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1201 2023-04-03 11:45:17.000000 mobspy-2.0.3/.github/workflows/python-app.yml
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      265 2023-04-05 11:22:48.000000 mobspy-2.0.3/.gitignore
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1068 2023-03-26 13:05:39.000000 mobspy-2.0.3/LICENSE
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     7015 2023-04-23 19:15:42.267710 mobspy-2.0.3/PKG-INFO
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5825 2023-03-29 14:16:39.000000 mobspy-2.0.3/README.md
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-23 19:15:42.148165 mobspy-2.0.3/example_models/
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-23 19:15:42.171569 mobspy-2.0.3/example_models/application_models/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      573 2023-03-26 13:05:39.000000 mobspy-2.0.3/example_models/application_models/AB_2CD.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1446 2023-03-26 13:05:39.000000 mobspy-2.0.3/example_models/application_models/AND_gate.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2653 2023-03-26 13:05:39.000000 mobspy-2.0.3/example_models/application_models/CRISPR_Oscillator.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1435 2023-04-18 11:26:50.000000 mobspy-2.0.3/example_models/application_models/For_The_Trees.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1297 2023-03-31 13:18:09.000000 mobspy-2.0.3/example_models/application_models/NOR_gate.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1244 2023-03-26 13:05:39.000000 mobspy-2.0.3/example_models/application_models/donor_receptor.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1372 2023-03-26 13:05:39.000000 mobspy-2.0.3/example_models/application_models/oscillator.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2901 2023-04-18 11:26:50.000000 mobspy-2.0.3/example_models/application_models/random_walk.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      565 2023-03-26 13:05:39.000000 mobspy-2.0.3/example_models/application_models/simple_repressor.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     3855 2023-03-26 13:05:39.000000 mobspy-2.0.3/example_models/application_models/toggle_switch.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-23 19:15:42.191472 mobspy-2.0.3/example_models/tutorial_models/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1602 2023-03-26 13:05:39.000000 mobspy-2.0.3/example_models/tutorial_models/01_Getting_Started.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1863 2023-03-26 13:05:39.000000 mobspy-2.0.3/example_models/tutorial_models/02_Reaction_Inheritance.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1013 2023-03-26 13:05:39.000000 mobspy-2.0.3/example_models/tutorial_models/02_Reaction_Inheritance_Model.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1769 2023-03-26 13:05:39.000000 mobspy-2.0.3/example_models/tutorial_models/03_Queries.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      946 2023-03-26 13:05:39.000000 mobspy-2.0.3/example_models/tutorial_models/03_Queries.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      989 2023-03-26 13:05:39.000000 mobspy-2.0.3/example_models/tutorial_models/04_Characteristic_Restriction.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1121 2023-03-31 13:18:09.000000 mobspy-2.0.3/example_models/tutorial_models/05_C_Query.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2284 2023-03-31 13:18:09.000000 mobspy-2.0.3/example_models/tutorial_models/06_Round_Robin.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2255 2023-03-26 13:05:39.000000 mobspy-2.0.3/example_models/tutorial_models/07_Rates.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2125 2023-03-31 13:18:09.000000 mobspy-2.0.3/example_models/tutorial_models/08_Units.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      866 2023-03-26 13:05:39.000000 mobspy-2.0.3/example_models/tutorial_models/09_Count_Assignment.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1042 2023-03-26 13:05:39.000000 mobspy-2.0.3/example_models/tutorial_models/09_Count_Assignment.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1589 2023-03-26 13:05:39.000000 mobspy-2.0.3/example_models/tutorial_models/10_Species_Loop.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2074 2023-03-26 13:05:39.000000 mobspy-2.0.3/example_models/tutorial_models/11_Results.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2128 2023-03-26 13:05:39.000000 mobspy-2.0.3/example_models/tutorial_models/12_Hierarchical_plot.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      982 2023-03-26 13:05:39.000000 mobspy-2.0.3/example_models/tutorial_models/13_Born_Species.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      255 2023-04-23 19:10:29.000000 mobspy-2.0.3/for_local_use.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-23 19:15:42.192835 mobspy-2.0.3/images/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    18566 2023-03-26 13:05:39.000000 mobspy-2.0.3/images/img.png
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-23 19:15:42.198020 mobspy-2.0.3/mobspy/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       95 2023-03-26 13:05:39.000000 mobspy-2.0.3/mobspy/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       22 2023-04-23 19:15:34.000000 mobspy-2.0.3/mobspy/_version.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-23 19:15:42.205512 mobspy-2.0.3/mobspy/data_handler/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-03-26 13:05:39.000000 mobspy-2.0.3/mobspy/data_handler/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2207 2023-04-23 18:41:27.000000 mobspy-2.0.3/mobspy/data_handler/process_result_data.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5972 2023-04-20 09:08:12.000000 mobspy-2.0.3/mobspy/data_handler/time_series_object.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-23 19:15:42.218128 mobspy-2.0.3/mobspy/modules/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-03-26 13:05:39.000000 mobspy-2.0.3/mobspy/modules/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4355 2023-04-17 14:42:37.000000 mobspy-2.0.3/mobspy/modules/event_functions.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    12825 2023-04-21 13:25:09.000000 mobspy-2.0.3/mobspy/modules/function_rate_code.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    12663 2023-04-12 21:11:32.000000 mobspy-2.0.3/mobspy/modules/logic_operator_objects.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    57658 2023-04-23 16:02:06.000000 mobspy-2.0.3/mobspy/modules/meta_class.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5239 2023-04-13 11:40:51.000000 mobspy-2.0.3/mobspy/modules/meta_class_utils.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    14961 2023-04-13 12:13:54.000000 mobspy-2.0.3/mobspy/modules/order_operators.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    16482 2023-04-13 12:24:44.000000 mobspy-2.0.3/mobspy/modules/reaction_construction_nb.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4088 2023-04-20 15:42:12.000000 mobspy-2.0.3/mobspy/modules/set_counts_module.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4143 2023-04-11 11:59:50.000000 mobspy-2.0.3/mobspy/modules/species_string_generator.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6615 2023-04-18 21:25:28.000000 mobspy-2.0.3/mobspy/modules/unit_handler.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-23 19:15:42.219619 mobspy-2.0.3/mobspy/parameter_scripts/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-03-26 13:05:39.000000 mobspy-2.0.3/mobspy/parameter_scripts/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2211 2023-04-07 15:35:28.000000 mobspy-2.0.3/mobspy/parameter_scripts/parameter_reader.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-23 19:15:42.223327 mobspy-2.0.3/mobspy/parameters/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1463 2023-03-26 13:05:39.000000 mobspy-2.0.3/mobspy/parameters/README.md
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-03-26 13:05:39.000000 mobspy-2.0.3/mobspy/parameters/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1035 2023-03-28 13:07:30.000000 mobspy-2.0.3/mobspy/parameters/default_reader.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1117 2023-04-07 15:35:28.000000 mobspy-2.0.3/mobspy/parameters/example_reader.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-23 19:15:42.227163 mobspy-2.0.3/mobspy/plot_params/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-03-26 13:05:39.000000 mobspy-2.0.3/mobspy/plot_params/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      184 2023-03-26 13:05:39.000000 mobspy-2.0.3/mobspy/plot_params/default_plot_reader.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1266 2023-04-21 19:43:28.000000 mobspy-2.0.3/mobspy/plot_params/example_plot_reader.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-23 19:15:42.230023 mobspy-2.0.3/mobspy/plot_scripts/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-03-26 13:05:39.000000 mobspy-2.0.3/mobspy/plot_scripts/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6445 2023-04-19 11:27:03.000000 mobspy-2.0.3/mobspy/plot_scripts/default_plots.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    14508 2023-04-20 22:03:28.000000 mobspy-2.0.3/mobspy/plot_scripts/hierarchical_plot.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1846 2023-04-20 09:16:42.000000 mobspy-2.0.3/mobspy/plot_scripts/process_plot_data.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     3566 2023-04-20 08:51:56.000000 mobspy-2.0.3/mobspy/plot_scripts/statistics_calculations.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-23 19:15:42.234491 mobspy-2.0.3/mobspy/sbml_simulator/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8118 2023-04-08 16:53:54.000000 mobspy-2.0.3/mobspy/sbml_simulator/SBMLWriter.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-03-26 13:05:39.000000 mobspy-2.0.3/mobspy/sbml_simulator/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      936 2023-04-08 16:40:14.000000 mobspy-2.0.3/mobspy/sbml_simulator/builder.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    12536 2023-04-17 15:49:48.000000 mobspy-2.0.3/mobspy/sbml_simulator/run.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    26518 2023-04-23 18:48:25.000000 mobspy-2.0.3/mobspy/simulation.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-23 19:15:42.236459 mobspy-2.0.3/mobspy/simulation_logging/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-03-26 13:05:39.000000 mobspy-2.0.3/mobspy/simulation_logging/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1013 2023-04-13 12:13:25.000000 mobspy-2.0.3/mobspy/simulation_logging/log_scripts.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-23 19:15:42.202456 mobspy-2.0.3/mobspy.egg-info/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     7015 2023-04-23 19:15:41.000000 mobspy-2.0.3/mobspy.egg-info/PKG-INFO
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     3635 2023-04-23 19:15:41.000000 mobspy-2.0.3/mobspy.egg-info/SOURCES.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        1 2023-04-23 19:15:41.000000 mobspy-2.0.3/mobspy.egg-info/dependency_links.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       76 2023-04-23 19:15:41.000000 mobspy-2.0.3/mobspy.egg-info/requires.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        7 2023-04-23 19:15:41.000000 mobspy-2.0.3/mobspy.egg-info/top_level.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       77 2023-03-26 13:05:39.000000 mobspy-2.0.3/requirements.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       38 2023-04-23 19:15:42.269433 mobspy-2.0.3/setup.cfg
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      767 2023-03-26 13:05:39.000000 mobspy-2.0.3/setup.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    20965 2023-04-23 19:13:59.000000 mobspy-2.0.3/test_script.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-23 19:15:42.265261 mobspy-2.0.3/test_tools/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      170 2023-03-26 13:05:39.000000 mobspy-2.0.3/test_tools/model_1.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      239 2023-03-28 14:54:04.000000 mobspy-2.0.3/test_tools/model_10.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      299 2023-03-29 10:35:15.000000 mobspy-2.0.3/test_tools/model_11.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      393 2023-03-31 14:53:54.000000 mobspy-2.0.3/test_tools/model_12.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      490 2023-03-31 16:58:04.000000 mobspy-2.0.3/test_tools/model_13.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      487 2023-03-31 17:23:20.000000 mobspy-2.0.3/test_tools/model_14.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      550 2023-04-03 08:42:24.000000 mobspy-2.0.3/test_tools/model_15.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      286 2023-04-04 18:39:28.000000 mobspy-2.0.3/test_tools/model_16.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      273 2023-04-05 14:12:52.000000 mobspy-2.0.3/test_tools/model_17.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      118 2023-04-06 11:09:14.000000 mobspy-2.0.3/test_tools/model_18.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      970 2023-04-06 13:23:26.000000 mobspy-2.0.3/test_tools/model_19.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      396 2023-03-26 13:05:39.000000 mobspy-2.0.3/test_tools/model_2.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      326 2023-04-06 13:24:46.000000 mobspy-2.0.3/test_tools/model_20.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1453 2023-04-11 12:17:19.000000 mobspy-2.0.3/test_tools/model_21.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      435 2023-04-11 15:31:51.000000 mobspy-2.0.3/test_tools/model_22.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      186 2023-04-12 16:26:56.000000 mobspy-2.0.3/test_tools/model_23.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      605 2023-04-17 14:45:24.000000 mobspy-2.0.3/test_tools/model_24.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       81 2023-04-18 11:30:58.000000 mobspy-2.0.3/test_tools/model_25.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      507 2023-04-18 20:45:48.000000 mobspy-2.0.3/test_tools/model_26.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      145 2023-04-18 21:30:11.000000 mobspy-2.0.3/test_tools/model_27.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      400 2023-04-20 13:29:32.000000 mobspy-2.0.3/test_tools/model_28.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      395 2023-04-20 13:29:51.000000 mobspy-2.0.3/test_tools/model_29.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     3154 2023-03-26 13:05:39.000000 mobspy-2.0.3/test_tools/model_3.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      468 2023-04-21 18:32:12.000000 mobspy-2.0.3/test_tools/model_30.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      727 2023-03-26 13:05:39.000000 mobspy-2.0.3/test_tools/model_4.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      559 2023-03-26 13:05:39.000000 mobspy-2.0.3/test_tools/model_5.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      353 2023-03-26 13:05:39.000000 mobspy-2.0.3/test_tools/model_6.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1352 2023-03-26 13:05:39.000000 mobspy-2.0.3/test_tools/model_7.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      443 2023-03-28 21:23:58.000000 mobspy-2.0.3/test_tools/model_8.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      736 2023-03-28 08:26:08.000000 mobspy-2.0.3/test_tools/model_9.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       60 2023-03-26 13:05:39.000000 mobspy-2.0.3/useful_parameters.json
```

### Comparing `mobspy-2.0.2/.github/workflows/python-app.yml` & `mobspy-2.0.3/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.2/LICENSE` & `mobspy-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.2/PKG-INFO` & `mobspy-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mobspy
-Version: 2.0.2
+Version: 2.0.3
 Summary: A Query-Based Language for Chemical Reaction Networks
 Home-page: https://github.com/ROBACON/mobspy
 License: UNKNOWN
 Description: ![Alt text](/images/img.png "MobsPy")
         
         # MobsPy
```

### Comparing `mobspy-2.0.2/README.md` & `mobspy-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.2/example_models/application_models/AB_2CD.py` & `mobspy-2.0.3/example_models/application_models/AB_2CD.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.2/example_models/application_models/AND_gate.py` & `mobspy-2.0.3/example_models/application_models/AND_gate.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.2/example_models/application_models/CRISPR_Oscillator.py` & `mobspy-2.0.3/example_models/application_models/CRISPR_Oscillator.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.2/example_models/application_models/For_The_Trees.py` & `mobspy-2.0.3/example_models/application_models/For_The_Trees.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.2/example_models/application_models/NOR_gate.py` & `mobspy-2.0.3/example_models/application_models/NOR_gate.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.2/example_models/application_models/donor_receptor.py` & `mobspy-2.0.3/example_models/application_models/donor_receptor.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.2/example_models/application_models/oscillator.py` & `mobspy-2.0.3/example_models/application_models/oscillator.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.2/example_models/application_models/random_walk.py` & `mobspy-2.0.3/example_models/application_models/random_walk.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.2/example_models/application_models/simple_repressor.py` & `mobspy-2.0.3/example_models/application_models/simple_repressor.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.2/example_models/application_models/toggle_switch.py` & `mobspy-2.0.3/example_models/application_models/toggle_switch.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.2/example_models/tutorial_models/01_Getting_Started.py` & `mobspy-2.0.3/example_models/tutorial_models/01_Getting_Started.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.2/example_models/tutorial_models/02_Reaction_Inheritance.py` & `mobspy-2.0.3/example_models/tutorial_models/02_Reaction_Inheritance.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.2/example_models/tutorial_models/02_Reaction_Inheritance_Model.txt` & `mobspy-2.0.3/example_models/tutorial_models/02_Reaction_Inheritance_Model.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.2/example_models/tutorial_models/03_Queries.py` & `mobspy-2.0.3/example_models/tutorial_models/03_Queries.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.2/example_models/tutorial_models/03_Queries.txt` & `mobspy-2.0.3/example_models/tutorial_models/03_Queries.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.2/example_models/tutorial_models/04_Characteristic_Restriction.py` & `mobspy-2.0.3/example_models/tutorial_models/04_Characteristic_Restriction.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.2/example_models/tutorial_models/05_C_Query.py` & `mobspy-2.0.3/example_models/tutorial_models/05_C_Query.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.2/example_models/tutorial_models/06_Round_Robin.py` & `mobspy-2.0.3/example_models/tutorial_models/06_Round_Robin.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.2/example_models/tutorial_models/07_Rates.py` & `mobspy-2.0.3/example_models/tutorial_models/07_Rates.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.2/example_models/tutorial_models/08_Units.py` & `mobspy-2.0.3/example_models/tutorial_models/08_Units.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.2/example_models/tutorial_models/09_Count_Assignment.py` & `mobspy-2.0.3/example_models/tutorial_models/09_Count_Assignment.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.2/example_models/tutorial_models/09_Count_Assignment.txt` & `mobspy-2.0.3/example_models/tutorial_models/09_Count_Assignment.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.2/example_models/tutorial_models/10_Species_Loop.py` & `mobspy-2.0.3/example_models/tutorial_models/10_Species_Loop.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.2/example_models/tutorial_models/11_Results.py` & `mobspy-2.0.3/example_models/tutorial_models/11_Results.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.2/example_models/tutorial_models/12_Hierarchical_plot.py` & `mobspy-2.0.3/example_models/tutorial_models/12_Hierarchical_plot.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.2/example_models/tutorial_models/13_Born_Species.py` & `mobspy-2.0.3/example_models/tutorial_models/13_Born_Species.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.2/images/img.png` & `mobspy-2.0.3/images/img.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.2/mobspy/data_handler/process_result_data.py` & `mobspy-2.0.3/mobspy/data_handler/process_result_data.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.2/mobspy/data_handler/time_series_object.py` & `mobspy-2.0.3/mobspy/data_handler/time_series_object.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.2/mobspy/modules/event_functions.py` & `mobspy-2.0.3/mobspy/modules/event_functions.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.2/mobspy/modules/function_rate_code.py` & `mobspy-2.0.3/mobspy/modules/function_rate_code.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,14 +113,26 @@
             Adds characteristic to the set of characteristics when checking for all
             referred characteristics by the user
 
             :param characteristic: (str) characteristic to add to the set
         """
         self._stocked_characteristics.add(characteristic)
 
+    def get_name(self):
+        """
+            Returns: The name of the species the reactant is in string format
+        """
+        return self._species_object.get_name()
+
+    def get_characteristics(self):
+        """
+            Returns: The characteristics of the species in this given state
+        """
+        return set(self.species_string.split('_dot_')[1:])
+
 
 def extract_reaction_rate(combination_of_reactant_species, reactant_string_list
                           , reaction_rate_function, type_of_model, dimension, function_rate_arguments=None):
     """
         This function is responsible for returning the reaction rate string for the model construction. To do this it
         does a different action depending on the type of the reaction_rate_function (we consider constants as functions)
         It passes the rate as a string expression in MobsPy standard units
```

### Comparing `mobspy-2.0.2/mobspy/modules/logic_operator_objects.py` & `mobspy-2.0.3/mobspy/modules/logic_operator_objects.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.2/mobspy/modules/meta_class.py` & `mobspy-2.0.3/mobspy/modules/meta_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,18 +99,22 @@
         """
         # Check to see if all species are named
         names_used = set()
         # Removing repeated elements to ensure only one meta-species in the simulation
         meta_species_to_simulate = meta_species_to_simulate.remove_repeated_elements()
         black_listed_names = {'Time', 'Rev', 'All'}
         for i, species in enumerate(meta_species_to_simulate):
+            if '_dot_' in species.get_name():
+                simlog.error(f'In species: {species.get_name()} \n _dot_ cannot be used in meta-species names')
             if species.get_name() in black_listed_names:
                 simlog.error(f'The name {species.get_name()} is not allowed for meta-species please change it')
             if '$' in species.get_name():
-                simlog.error('An error has occurred and one of the species was not named')
+                simlog.error(f'In species: {species.get_name()} \n'
+                             f'An error has occurred and one of the species was either not named or named with the '
+                             f'restricted $ symbol')
             if species.get_name() in names_used:
                 simlog.error(f'Names must be unique for all species\n' +
                              f'The repeated name is {species.get_name()} in position {i}\n' +
                              f'Another possibility could be a repeated meta-species in the model')
             names_used.add(species.get_name())
 
         # Order the species references for later usage
@@ -529,41 +533,38 @@
             p = Reacting_Species(other, set())
         else:
             p = other
 
         reaction = Reactions(self.list_of_reactants, p.list_of_reactants)
         return reaction
 
+    # Reacting_Species call
     def __call__(self, quantity):
         """
             The call operator here is used to add counts to species non-default state. This stores the characteristics
             that have been called using the dot operator to assign the count after the call operation
 
             :param quantity: (int, float, Quantity) count to be assigned to the species
         """
         species_object = self.list_of_reactants[0]['object']
+        characteristics = self.list_of_reactants[0]['characteristics']
         simulation_under_context = self.list_of_reactants[0]['object']._simulation_context
 
         if type(quantity) == int or type(quantity) == float or isinstance(quantity, Quantity):
             if len(self.list_of_reactants) != 1:
                 simlog.error('Assignment used incorrectly. Only one species at a time', stack_index=2)
-            species_object = species_object
-            characteristics = self.list_of_reactants[0]['characteristics']
             quantity_dict = species_object.add_quantities(characteristics, quantity)
-        elif type(quantity) == Reacting_Species and simulation_under_context is not None:
-            simlog.error(f'Assignments of counts using meta-species are only allowed under events in '
-                         f'simulation context', stack_index=2)
-        else:
+        elif simulation_under_context is None:
             simlog.error(f'Reactant_Species count assignment does not support the type {type(quantity)}',
                          stack_index=2)
 
         if simulation_under_context is not None:
             try:
                 if type(quantity) == str:
-                    quantity_dict = self.add_quantities('std$', quantity)
+                    quantity_dict = species_object.add_quantities(characteristics, quantity)
                 simulation_under_context.current_event_count_data.append({'species': species_object,
                                                                           'characteristics': quantity_dict[
                                                                               'characteristics'],
                                                                           'quantity': quantity_dict[
                                                                               'quantity']})
             except Exception as e:
                 simlog.error(str(e) + '\n Only species count assignments are allowed in a model context')
@@ -573,14 +574,17 @@
     def __getattr__(self, characteristic):
         """
             This is the implementation of the .dot operation. Adds characteristics to the species and/or perform
             queries
 
             :param characteristic: (str) characteristic for the query
         """
+        if characteristic == '_ipython_canary_method_should_not_exist_':
+            return 0
+
         Species.check_if_valid_characteristic(characteristic)
 
         for reactant in self.list_of_reactants:
 
             species_object = reactant['object']
             characteristics_from_references = mcu.unite_characteristics(species_object.get_references())
 
@@ -981,28 +985,33 @@
             This adds characteristics using the following manner Species.characteristic
             If it is the first time is called we add it to the set of characteristics
             Second time, it just creates a Reacting_Species for reaction construction
 
             :param characteristic: (str) characteristic to be added or to be use as a query in the reaction
             :return: Reacting_Species with the characteristic added for querying
         """
+
+        # This is for IPython notebooks compatibility
+        if characteristic == '_ipython_canary_method_should_not_exist_':
+            return 0
+
         Species.check_if_valid_characteristic(characteristic)
 
         characteristics_from_references = mcu.unite_characteristics(self.get_references())
         characteristics = {characteristic}
 
         if characteristic not in characteristics_from_references and '$' not in characteristic:
             if len(self.get_characteristics()) == 0:
                 self.first_characteristic = characteristic
 
             self.add_characteristic(characteristic)
 
         return Reacting_Species(self, characteristics)
 
-    # Adding counts to species
+    # Species call
     def __call__(self, quantity):
         """
             The __call__ operator handles two things for Species objects
             First, it adds characteristics to the default state of the meta-species if the quantity is a real
             Secondly, it returns the name of the characteristic from a species string that belongs to this meta-species
 
             :param: quantity (int, float, Quantity) = for count assignment
@@ -1016,14 +1025,18 @@
             for cha in str(quantity).split('_dot_')[1:]:
                 if cha in self._characteristics:
                     return cha
             simlog.error(f'{quantity} contains no characteristics from {self._name}', stack_index=2)
         elif type(quantity) == Reacting_Species:
             simlog.error(f'Assignments of counts using meta-species are only allowed under events in '
                          f'simulation context', stack_index=2)
+        elif self._simulation_context is None:
+            simlog.error(f'Reactant_Species count assignment does not support the type {type(quantity)}'
+                         f' if not under a simulation context',
+                         stack_index=2)
 
         if self._simulation_context is not None:
 
             if type(quantity) == str:
                 quantity_dict = self.add_quantities('std$', quantity)
             try:
                 self._simulation_context.current_event_count_data.append({'species': self,
```

### Comparing `mobspy-2.0.2/mobspy/modules/meta_class_utils.py` & `mobspy-2.0.3/mobspy/modules/meta_class_utils.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.2/mobspy/modules/order_operators.py` & `mobspy-2.0.3/mobspy/modules/order_operators.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.2/mobspy/modules/reaction_construction_nb.py` & `mobspy-2.0.3/mobspy/modules/reaction_construction_nb.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.2/mobspy/modules/set_counts_module.py` & `mobspy-2.0.3/mobspy/modules/set_counts_module.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import mobspy.simulation_logging.log_scripts as simlog
 import inspect
-from mobspy.modules.meta_class import List_Species
+from mobspy.modules.meta_class import List_Species, Species, Reacting_Species
 from pint import Quantity
 
 
 def set_counts(count_dic):
     """
         Adds counts to meta-species using a given dictionary. Keys from this dictionary can be either meta-species
         objects or strings. Items must be the assign counts to species
@@ -29,21 +29,21 @@
         found_species = set()
 
         for i in range(len(inspect.stack())):
             local_names = inspect.stack()[i][0].f_locals
             global_names = inspect.stack()[i][0].f_globals
             for key, item in global_names.items():
                 try:
-                    if item.is_species() and type(item) != type:
+                    if isinstance(item, Species) and type(item) != type:
                         found_species.add(item)
                 except AttributeError:
                     pass
             for key, item in local_names.items():
                 try:
-                    if item.is_species() and type(item) != type:
+                    if isinstance(item, Species) and type(item) != type:
                         found_species.add(item)
                 except AttributeError:
                     pass
 
         return found_species
 
     for key in count_dic:
@@ -69,20 +69,20 @@
                 elif spe.get_name() == str_name and already_found:
                     simlog.error(f'There are two different meta-species with the same name. Set_counts cannot resolve',
                                  stack_index=2)
             if not already_found:
                 simlog.error(f'Meta-species with the following name {key} not found', stack_index=2)
         else:
             try:
-                if key.is_spe_or_reac():
-                    if not key.is_species():
+                if isinstance(key, Species) or isinstance(key, Reacting_Species):
+                    if not isinstance(key, Species):
                         if len(key.list_of_reactants) != 1:
                             simlog.error('Assignment used incorrectly. Only one species at a time', stack_index=2)
                         model.add(key.list_of_reactants[0]['object'])
-                    if key.is_species():
+                    if isinstance(key, Species):
                         model.add(key)
                     key(item)
             except AttributeError:
                 simlog.error('Keys must be either meta-species or strings',
                              stack_index=2)
 
     return List_Species(model)
```

### Comparing `mobspy-2.0.2/mobspy/modules/species_string_generator.py` & `mobspy-2.0.3/mobspy/modules/species_string_generator.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.2/mobspy/modules/unit_handler.py` & `mobspy-2.0.3/mobspy/modules/unit_handler.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.2/mobspy/parameter_scripts/parameter_reader.py` & `mobspy-2.0.3/mobspy/parameter_scripts/parameter_reader.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.2/mobspy/parameters/README.md` & `mobspy-2.0.3/mobspy/parameters/README.md`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.2/mobspy/parameters/default_reader.py` & `mobspy-2.0.3/mobspy/parameters/default_reader.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.2/mobspy/parameters/example_reader.py` & `mobspy-2.0.3/mobspy/parameters/example_reader.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.2/mobspy/plot_params/example_plot_reader.py` & `mobspy-2.0.3/mobspy/plot_params/example_plot_reader.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         'frameon':False,
         'title':'Test_Plot',
         'annotations':['Test_note', 0, 0],
         'pad':1,
         'dpi':3,
         "plots":False,
         "species_to_plot": None,
+        "save_to": 'example.png',
 
         "figures": [{
             "plots": [{
                 "species_to_plot": ["A"]
             }]
         }],
```

### Comparing `mobspy-2.0.2/mobspy/plot_scripts/default_plots.py` & `mobspy-2.0.3/mobspy/plot_scripts/default_plots.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.2/mobspy/plot_scripts/hierarchical_plot.py` & `mobspy-2.0.3/mobspy/plot_scripts/hierarchical_plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -373,12 +373,17 @@
     set_figure_characteristics(axis_matrix, plot_params)
 
     # Now we plot
     for figure_index in range(figure_number):
         plot_curves(data, figure_hash(figure_index, axis_matrix), figure_index, plot_params)
 
     # Real default case
-    plt.show()
+
+    save_to = find_parameter(plot_params, 'save_to')
+    if save_to is None:
+        plt.show()
+    else:
+        plt.savefig(save_to)
 
 
 if __name__ == "__main__":
     pass
```

### Comparing `mobspy-2.0.2/mobspy/plot_scripts/process_plot_data.py` & `mobspy-2.0.3/mobspy/plot_scripts/process_plot_data.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.2/mobspy/plot_scripts/statistics_calculations.py` & `mobspy-2.0.3/mobspy/plot_scripts/statistics_calculations.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.2/mobspy/sbml_simulator/SBMLWriter.py` & `mobspy-2.0.3/mobspy/sbml_simulator/SBMLWriter.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.2/mobspy/sbml_simulator/builder.py` & `mobspy-2.0.3/mobspy/sbml_simulator/builder.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.2/mobspy/sbml_simulator/run.py` & `mobspy-2.0.3/mobspy/sbml_simulator/run.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.2/mobspy/simulation.py` & `mobspy-2.0.3/mobspy/simulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,14 +152,17 @@
         #        names[key] = item
         #    for key, item in local_names.items():
         #        names[key] = item
 
         self.model = model
         self.names = names
 
+        if type(model) == set or type(model) == list:
+            model = List_Species(model)
+
         if not isinstance(model, Species) and not isinstance(model, List_Species):
             simlog.error('Model must be formed only by Species objects or List_Species objects \n'
                          f'Model type {type(model)} and it is {model}')
 
         self.orthogonal_vector_structure = mcu.create_orthogonal_vector_structure(model)
 
         # Get all meta - reactions
@@ -268,15 +271,15 @@
 
         unprocessed_data = sbml_run.simulate(self._list_of_parameters, self._list_of_models)
 
         processed_data = []
         for updl in unprocessed_data:
             processed_data.append(dh.convert_data_to_desired_unit(updl, self.parameters['unit_x'],
                                                                   self.parameters['unit_y'],
-                                                                  self.output_concentration,
+                                                                  self.parameters['output_concentration'],
                                                                   self.parameters['volume']))
 
         data_dict = {'data': processed_data,
                      'params': self.parameters,
                      'models': self._list_of_models}
 
         self.results = MobsPyTimeSeries(data_dict)
@@ -391,21 +394,25 @@
                 pass
             else:
                 simlog.error(f'Parameter {name} is not supported', stack_index=2)
 
     def __getattribute__(self, item):
         if item == 'results' and self.__dict__['results'] == {}:
             simlog.error('The results were accessed before the execution of the simulation', stack_index=2)
+
+        if item == 'plot_config':
+            return self.__getattr__(item)
+
         return super().__getattribute__(item)
 
     def __getattr__(self, item):
         """
             __getattr__ override. For the user to be able to set plot parameters as MySim.plot.parameter
         """
-        if item == 'plot':
+        if item == 'plot_config':
             self.__dict__['plot_flag'] = True
         else:
             self.__dict__['plot_flag'] = False
         return self
 
     def configure_parameters(self, config):
         """
@@ -512,14 +519,18 @@
         """
         to_return = []
         for sbml_data in self._list_of_models:
             to_return.append(sbml_builder.build(sbml_data['species_for_sbml'], sbml_data['parameters_for_sbml'],
                                                 sbml_data['reactions_for_sbml'], sbml_data['events_for_sbml']))
         return to_return
 
+    @classmethod
+    def is_simulation(cls):
+        return True
+
 
 class SimulationComposition:
 
     def _compile_multi_simulation(self):
         for sim1 in self.list_of_simulations:
             for sim2 in self.list_of_simulations:
                 if sim1 == sim2:
@@ -610,10 +621,14 @@
 
     def plot_raw(self, parameters_or_file):
         self.base_sim.plot_raw(parameters_or_file)
 
     def generate_sbml(self):
         return self.base_sim.generate_sbml()
 
+    @classmethod
+    def is_simulation(cls):
+        return True
+
 
 if __name__ == '__main__':
     pass
```

### Comparing `mobspy-2.0.2/mobspy/simulation_logging/log_scripts.py` & `mobspy-2.0.3/mobspy/simulation_logging/log_scripts.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.2/mobspy.egg-info/PKG-INFO` & `mobspy-2.0.3/mobspy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mobspy
-Version: 2.0.2
+Version: 2.0.3
 Summary: A Query-Based Language for Chemical Reaction Networks
 Home-page: https://github.com/ROBACON/mobspy
 License: UNKNOWN
 Description: ![Alt text](/images/img.png "MobsPy")
         
         # MobsPy
```

### Comparing `mobspy-2.0.2/mobspy.egg-info/SOURCES.txt` & `mobspy-2.0.3/mobspy.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -92,14 +92,17 @@
 test_tools/model_21.txt
 test_tools/model_22.txt
 test_tools/model_23.txt
 test_tools/model_24.txt
 test_tools/model_25.txt
 test_tools/model_26.txt
 test_tools/model_27.txt
+test_tools/model_28.txt
+test_tools/model_29.txt
 test_tools/model_3.txt
+test_tools/model_30.txt
 test_tools/model_4.txt
 test_tools/model_5.txt
 test_tools/model_6.txt
 test_tools/model_7.txt
 test_tools/model_8.txt
 test_tools/model_9.txt
```

### Comparing `mobspy-2.0.2/setup.py` & `mobspy-2.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.2/test_script.py` & `mobspy-2.0.3/test_script.py`

 * *Files 6% similar despite different names*

```diff
@@ -759,23 +759,115 @@
 
     A(1)
     S = Simulation(A)
     S.level = -1
     assert compare_model(S.compile(), 'test_tools/model_27.txt')
 
 
+def test_multiple_simulation_counts():
+
+    Age, Color, Size = BaseSpecies()
+
+    Age.young, Age.old,
+    Color.blue, Color.red,
+    Size.small, Size.big
+
+    Tree = Age * Color * Size
+
+    Tree(100), Tree.red.big(150), All[Tree](10), All[Tree.big](100)
+    S = Simulation(Tree)
+    S.level = -1
+    assert compare_model(S.compile(), 'test_tools/model_28.txt')
+
+    model = set_counts({All[Tree]: 30, 'Tree.blue.old': 100})
+    S = Simulation(model)
+    S.level = -1
+    assert compare_model(S.compile(), 'test_tools/model_29.txt')
+
+
+def test_string_events_assignment():
+
+    A = BaseSpecies()
+
+    A.a1, A.a2, A.a3
+
+    S = Simulation(A)
+    S.level = -1
+    with S.event_time(5):
+        All[A](f'{A} + 1')
+
+    with S.event_time(10):
+        All[A.a1](f'{A} + 1')
+
+    with S.event_time(15):
+        A.a1(f'{A} + 1')
+
+    compare_model(S.compile(), 'test_tools/model_30.txt')
+
+
+def test_plotting():
+    Color, Disease = BaseSpecies()
+
+    Color.blue, Color.red, Color.yellow
+    Disease.not_sick, Disease.sick
+
+    Disease.not_sick >> Disease.sick[1]
+
+    Tree = Color * Disease
+
+    Tree.yellow(20), Tree.red(20), Tree.blue(20)
+
+    S = Simulation(Tree)
+    S.level = -1
+    S.method = 'stochastic'
+    S.plot_data = False
+    S.repetitions = 3
+    S.step_size = 0.25
+    S.duration = 3
+    S.run()
+    S.plot_config.save_to = 'test_plot_images/stochastic_tree.png'
+    S.plot_stochastic(Tree.not_sick, Tree.sick)
+
+    S.plot_config.save_to = 'test_plot_images/deterministic_tree.png'
+    S.plot(Tree.not_sick, Tree.sick)
+
+    S.plot_config.save_to = 'test_plot_images/constant_tree.png'
+    S.plot()
+
+    assert os.path.exists('test_plot_images/stochastic_tree.png')
+    assert os.path.exists('test_plot_images/deterministic_tree.png')
+    assert os.path.exists('test_plot_images/constant_tree.png')
+
+
+def test_volume_after_sim():
+
+    A = BaseSpecies()
+
+    Zero >> A[42]
+    A >> Zero[1]
+
+    S = Simulation(A)
+    S.plot_data = False
+    S.level = -1
+    S.volume = 1 * u.milliliter
+    S.run()
+    assert int(S.results[A][-1]) == 42
+
+
 test_list = [test_model_1, test_model_2, test_model_3, test_model_4, test_model_5, test_model_6, test_model_7,
              test_orthogonal_spaces, test_average_value, test_hybrid_sim, test_concatenated_simulation,
              test_event_type, test_reacting_species_event, test_unit_event_test, test_reaction_deactivation,
              test_double_rate, test_single_rate, test_triple_rate, test_stochastic_event_duration,
              test_logic_operator_syntax, test_stack_position, test_empty_arguments,
              test_conditional_between_meta_species, test_conditional_between_meta_species_2,
              test_event_reaction_not_allowed, all_test, all_test_2, test_error_mult, test_set_counts,
              test_bool_error, test_event_all, test_one_value_concatenation_sim, test_crash_after_modification,
-             test_unit_bi_dimension, test_bi_dimensional_rates, test_dimension_in_function_only]
+             test_unit_bi_dimension, test_bi_dimensional_rates, test_dimension_in_function_only,
+             test_multiple_simulation_counts, test_string_events_assignment, test_plotting,
+             test_volume_after_sim]
 
 sub_test = test_list
 
 
 def perform_tests():
 
     any_failed = False
```

### Comparing `mobspy-2.0.2/test_tools/model_15.txt` & `mobspy-2.0.3/test_tools/model_15.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.2/test_tools/model_19.txt` & `mobspy-2.0.3/test_tools/model_19.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.2/test_tools/model_21.txt` & `mobspy-2.0.3/test_tools/model_21.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.2/test_tools/model_24.txt` & `mobspy-2.0.3/test_tools/model_24.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.2/test_tools/model_3.txt` & `mobspy-2.0.3/test_tools/model_3.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.2/test_tools/model_4.txt` & `mobspy-2.0.3/test_tools/model_4.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.2/test_tools/model_5.txt` & `mobspy-2.0.3/test_tools/model_5.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.2/test_tools/model_7.txt` & `mobspy-2.0.3/test_tools/model_7.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.2/test_tools/model_9.txt` & `mobspy-2.0.3/test_tools/model_9.txt`

 * *Files identical despite different names*

