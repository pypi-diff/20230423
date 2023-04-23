# Comparing `tmp/Qcover-2.3.0.tar.gz` & `tmp/Qcover-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Qcover-2.3.0.tar", last modified: Tue Apr  4 07:14:43 2023, max compression
+gzip compressed data, was "Qcover-2.4.0.tar", last modified: Sun Apr 23 09:13:05 2023, max compression
```

## Comparing `Qcover-2.3.0.tar` & `Qcover-2.4.0.tar`

### file list

```diff
@@ -1,67 +1,68 @@
-drwxrwxrwx   0 ntyz      (1000) ntyz      (1000)        0 2023-04-04 07:14:43.814313 Qcover-2.3.0/
--rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)    11558 2021-12-27 08:01:43.000000 Qcover-2.3.0/LICENSE
--rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     8394 2023-04-04 07:14:43.804177 Qcover-2.3.0/PKG-INFO
-drwxrwxrwx   0 ntyz      (1000) ntyz      (1000)        0 2023-04-04 07:14:43.313080 Qcover-2.3.0/Qcover/
--rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)      577 2023-04-04 07:13:04.000000 Qcover-2.3.0/Qcover/__init__.py
-drwxrwxrwx   0 ntyz      (1000) ntyz      (1000)        0 2023-04-04 07:14:43.473644 Qcover-2.3.0/Qcover/applications/
--rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)      171 2022-03-16 08:40:56.000000 Qcover-2.3.0/Qcover/applications/__init__.py
--rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     4908 2023-02-27 08:33:06.000000 Qcover-2.3.0/Qcover/applications/common.py
--rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     9750 2022-03-18 08:59:21.000000 Qcover-2.3.0/Qcover/applications/general_01_programming.py
--rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     4376 2022-03-18 09:30:22.000000 Qcover-2.3.0/Qcover/applications/graph_color.py
--rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     5447 2022-03-18 09:31:58.000000 Qcover-2.3.0/Qcover/applications/max_2_sat.py
--rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     3785 2023-02-27 06:35:19.000000 Qcover-2.3.0/Qcover/applications/max_cut.py
--rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     5309 2022-03-18 09:02:32.000000 Qcover-2.3.0/Qcover/applications/minimum_vertex_cover.py
--rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     3985 2022-03-18 09:02:47.000000 Qcover-2.3.0/Qcover/applications/number_partition.py
--rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     7185 2022-03-18 09:05:30.000000 Qcover-2.3.0/Qcover/applications/qadratic_knapsack.py
--rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     6207 2022-03-18 09:07:17.000000 Qcover-2.3.0/Qcover/applications/quadratic_assignment.py
--rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     6388 2022-03-18 09:08:29.000000 Qcover-2.3.0/Qcover/applications/set_packing.py
--rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     6533 2022-03-18 09:27:59.000000 Qcover-2.3.0/Qcover/applications/set_partitioning.py
--rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     1607 2022-03-18 09:27:37.000000 Qcover-2.3.0/Qcover/applications/sherrington_kirkpatrick.py
-drwxrwxrwx   0 ntyz      (1000) ntyz      (1000)        0 2023-04-04 07:14:43.593169 Qcover-2.3.0/Qcover/backends/
--rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)      573 2022-04-01 05:42:58.000000 Qcover-2.3.0/Qcover/backends/__init__.py
--rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     1321 2022-08-10 03:01:43.000000 Qcover-2.3.0/Qcover/backends/backend.py
--rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     8194 2022-09-07 03:11:02.000000 Qcover-2.3.0/Qcover/backends/circuitbycirq.py
--rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     8394 2022-08-10 02:25:58.000000 Qcover-2.3.0/Qcover/backends/circuitbyprojectq.py
--rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)    12833 2022-10-21 13:23:25.000000 Qcover-2.3.0/Qcover/backends/circuitbyqiskit.py
--rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)    13174 2022-08-17 08:49:21.000000 Qcover-2.3.0/Qcover/backends/circuitbyqiskit_statistic.py
--rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     7941 2022-08-10 02:26:19.000000 Qcover-2.3.0/Qcover/backends/circuitbyqton.py
--rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     8852 2022-08-10 03:02:26.000000 Qcover-2.3.0/Qcover/backends/circuitbyqulacs.py
--rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     5505 2022-10-21 13:18:00.000000 Qcover-2.3.0/Qcover/backends/circuitbytensor.py
-drwxrwxrwx   0 ntyz      (1000) ntyz      (1000)        0 2023-04-04 07:14:43.615621 Qcover-2.3.0/Qcover/compiler/
--rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)      118 2022-09-30 09:31:05.000000 Qcover-2.3.0/Qcover/compiler/__init__.py
--rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)    40519 2023-04-03 08:23:48.000000 Qcover-2.3.0/Qcover/compiler/compilerforQAOA.py
--rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)    12265 2023-04-03 08:22:33.000000 Qcover-2.3.0/Qcover/compiler/hardware_library.py
--rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)    13820 2022-09-02 08:04:41.000000 Qcover-2.3.0/Qcover/core.py
--rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     2624 2022-06-26 02:25:59.000000 Qcover-2.3.0/Qcover/exceptions.py
-drwxrwxrwx   0 ntyz      (1000) ntyz      (1000)        0 2023-04-04 07:14:43.726004 Qcover-2.3.0/Qcover/optimizers/
--rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     2227 2022-08-17 07:56:55.000000 Qcover-2.3.0/Qcover/optimizers/COBYLA.py
--rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     6349 2022-02-08 07:12:19.000000 Qcover-2.3.0/Qcover/optimizers/Fourier.py
--rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     2224 2022-06-22 13:12:01.000000 Qcover-2.3.0/Qcover/optimizers/Gradient_Descent.py
--rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     4812 2022-06-09 07:47:25.000000 Qcover-2.3.0/Qcover/optimizers/Interp.py
--rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     2460 2022-06-09 07:47:34.000000 Qcover-2.3.0/Qcover/optimizers/L_BFGS_B.py
--rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     2890 2022-07-07 08:20:31.000000 Qcover-2.3.0/Qcover/optimizers/SHGO.py
--rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     2336 2022-06-09 07:47:41.000000 Qcover-2.3.0/Qcover/optimizers/SLSQP.py
--rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     3172 2022-06-22 13:45:02.000000 Qcover-2.3.0/Qcover/optimizers/SPSA.py
--rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     1697 2022-06-24 02:38:44.000000 Qcover-2.3.0/Qcover/optimizers/Simulated_Annealing.py
--rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)      494 2022-07-07 07:33:00.000000 Qcover-2.3.0/Qcover/optimizers/__init__.py
--rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)      267 2022-02-08 03:40:09.000000 Qcover-2.3.0/Qcover/optimizers/optimizer.py
-drwxrwxrwx   0 ntyz      (1000) ntyz      (1000)        0 2023-04-04 07:14:43.766039 Qcover-2.3.0/Qcover/research/
--rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     7295 2023-02-27 09:19:50.000000 Qcover-2.3.0/Qcover/research/Ent_TMI.py
--rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     5536 2022-09-02 08:09:52.000000 Qcover-2.3.0/Qcover/research/GHZ_Generate.py
--rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     5737 2022-09-02 03:01:48.000000 Qcover-2.3.0/Qcover/research/QAOA_Generate.py
--rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)        0 2022-05-30 09:03:08.000000 Qcover-2.3.0/Qcover/research/__init__.py
--rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     6350 2023-02-27 09:07:40.000000 Qcover-2.3.0/Qcover/research/scrambling-OTOC.py
-drwxrwxrwx   0 ntyz      (1000) ntyz      (1000)        0 2023-04-04 07:14:43.802180 Qcover-2.3.0/Qcover/simulator/
--rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)      155 2022-04-01 05:13:15.000000 Qcover-2.3.0/Qcover/simulator/__init__.py
--rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     6053 2023-02-27 08:53:58.000000 Qcover-2.3.0/Qcover/simulator/qton.py
--rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     3009 2022-09-01 02:55:28.000000 Qcover-2.3.0/Qcover/utils.py
--rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)       95 2023-04-04 07:13:04.000000 Qcover-2.3.0/Qcover/version.py
-drwxrwxrwx   0 ntyz      (1000) ntyz      (1000)        0 2023-04-04 07:14:43.333850 Qcover-2.3.0/Qcover.egg-info/
--rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     8394 2023-04-04 07:14:43.000000 Qcover-2.3.0/Qcover.egg-info/PKG-INFO
--rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     1712 2023-04-04 07:14:43.000000 Qcover-2.3.0/Qcover.egg-info/SOURCES.txt
--rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)        1 2023-04-04 07:14:43.000000 Qcover-2.3.0/Qcover.egg-info/dependency_links.txt
--rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)      204 2023-04-04 07:14:43.000000 Qcover-2.3.0/Qcover.egg-info/requires.txt
--rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)        7 2023-04-04 07:14:43.000000 Qcover-2.3.0/Qcover.egg-info/top_level.txt
--rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     7262 2022-10-24 07:20:18.000000 Qcover-2.3.0/README.md
--rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)       38 2023-04-04 07:14:43.814313 Qcover-2.3.0/setup.cfg
--rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     2815 2022-10-08 06:52:08.000000 Qcover-2.3.0/setup.py
+drwxrwxrwx   0 ntyz      (1000) ntyz      (1000)        0 2023-04-23 09:13:05.119565 Qcover-2.4.0/
+-rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)    11558 2021-12-27 08:01:43.000000 Qcover-2.4.0/LICENSE
+-rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     8394 2023-04-23 09:13:05.118567 Qcover-2.4.0/PKG-INFO
+drwxrwxrwx   0 ntyz      (1000) ntyz      (1000)        0 2023-04-23 09:13:05.043783 Qcover-2.4.0/Qcover/
+-rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)      577 2023-04-23 09:07:20.000000 Qcover-2.4.0/Qcover/__init__.py
+drwxrwxrwx   0 ntyz      (1000) ntyz      (1000)        0 2023-04-23 09:13:05.069696 Qcover-2.4.0/Qcover/applications/
+-rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)      171 2022-03-16 08:40:56.000000 Qcover-2.4.0/Qcover/applications/__init__.py
+-rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     5005 2023-04-15 13:14:34.000000 Qcover-2.4.0/Qcover/applications/common.py
+-rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     9750 2022-03-18 08:59:21.000000 Qcover-2.4.0/Qcover/applications/general_01_programming.py
+-rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     4376 2022-03-18 09:30:22.000000 Qcover-2.4.0/Qcover/applications/graph_color.py
+-rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     5447 2022-03-18 09:31:58.000000 Qcover-2.4.0/Qcover/applications/max_2_sat.py
+-rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     3785 2023-02-27 06:35:19.000000 Qcover-2.4.0/Qcover/applications/max_cut.py
+-rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     5309 2022-03-18 09:02:32.000000 Qcover-2.4.0/Qcover/applications/minimum_vertex_cover.py
+-rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     3985 2022-03-18 09:02:47.000000 Qcover-2.4.0/Qcover/applications/number_partition.py
+-rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     7185 2022-03-18 09:05:30.000000 Qcover-2.4.0/Qcover/applications/qadratic_knapsack.py
+-rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     6207 2022-03-18 09:07:17.000000 Qcover-2.4.0/Qcover/applications/quadratic_assignment.py
+-rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     6388 2022-03-18 09:08:29.000000 Qcover-2.4.0/Qcover/applications/set_packing.py
+-rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     6533 2022-03-18 09:27:59.000000 Qcover-2.4.0/Qcover/applications/set_partitioning.py
+-rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     1607 2022-03-18 09:27:37.000000 Qcover-2.4.0/Qcover/applications/sherrington_kirkpatrick.py
+drwxrwxrwx   0 ntyz      (1000) ntyz      (1000)        0 2023-04-23 09:13:05.085654 Qcover-2.4.0/Qcover/backends/
+-rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)      640 2023-04-23 08:14:47.000000 Qcover-2.4.0/Qcover/backends/__init__.py
+-rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     1081 2023-04-15 11:10:00.000000 Qcover-2.4.0/Qcover/backends/backend.py
+-rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     8194 2022-09-07 03:11:02.000000 Qcover-2.4.0/Qcover/backends/circuitbycirq.py
+-rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     8394 2022-08-10 02:25:58.000000 Qcover-2.4.0/Qcover/backends/circuitbyprojectq.py
+-rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)    12853 2023-04-14 11:08:26.000000 Qcover-2.4.0/Qcover/backends/circuitbyqiskit.py
+-rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)    13360 2023-04-14 11:04:52.000000 Qcover-2.4.0/Qcover/backends/circuitbyqiskit_statistic.py
+-rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     7941 2022-08-10 02:26:19.000000 Qcover-2.4.0/Qcover/backends/circuitbyqton.py
+-rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     1397 2023-04-23 08:13:53.000000 Qcover-2.4.0/Qcover/backends/circuitbyquafu.py
+-rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     8855 2023-04-23 08:10:47.000000 Qcover-2.4.0/Qcover/backends/circuitbyqulacs.py
+-rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     5734 2023-04-15 12:28:44.000000 Qcover-2.4.0/Qcover/backends/circuitbytensor.py
+drwxrwxrwx   0 ntyz      (1000) ntyz      (1000)        0 2023-04-23 09:13:05.089646 Qcover-2.4.0/Qcover/compiler/
+-rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)      118 2022-09-30 09:31:05.000000 Qcover-2.4.0/Qcover/compiler/__init__.py
+-rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)    44753 2023-04-17 14:38:22.000000 Qcover-2.4.0/Qcover/compiler/compilerforQAOA.py
+-rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)    12955 2023-04-14 09:59:46.000000 Qcover-2.4.0/Qcover/compiler/hardware_library.py
+-rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)    13820 2022-09-02 08:04:41.000000 Qcover-2.4.0/Qcover/core.py
+-rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     2624 2022-06-26 02:25:59.000000 Qcover-2.4.0/Qcover/exceptions.py
+drwxrwxrwx   0 ntyz      (1000) ntyz      (1000)        0 2023-04-23 09:13:05.106598 Qcover-2.4.0/Qcover/optimizers/
+-rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     2227 2022-08-17 07:56:55.000000 Qcover-2.4.0/Qcover/optimizers/COBYLA.py
+-rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     6349 2022-02-08 07:12:19.000000 Qcover-2.4.0/Qcover/optimizers/Fourier.py
+-rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     2224 2022-06-22 13:12:01.000000 Qcover-2.4.0/Qcover/optimizers/Gradient_Descent.py
+-rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     4812 2022-06-09 07:47:25.000000 Qcover-2.4.0/Qcover/optimizers/Interp.py
+-rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     2460 2022-06-09 07:47:34.000000 Qcover-2.4.0/Qcover/optimizers/L_BFGS_B.py
+-rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     2890 2022-07-07 08:20:31.000000 Qcover-2.4.0/Qcover/optimizers/SHGO.py
+-rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     2336 2022-06-09 07:47:41.000000 Qcover-2.4.0/Qcover/optimizers/SLSQP.py
+-rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     3172 2022-06-22 13:45:02.000000 Qcover-2.4.0/Qcover/optimizers/SPSA.py
+-rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     1697 2022-06-24 02:38:44.000000 Qcover-2.4.0/Qcover/optimizers/Simulated_Annealing.py
+-rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)      494 2022-07-07 07:33:00.000000 Qcover-2.4.0/Qcover/optimizers/__init__.py
+-rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)      267 2022-02-08 03:40:09.000000 Qcover-2.4.0/Qcover/optimizers/optimizer.py
+drwxrwxrwx   0 ntyz      (1000) ntyz      (1000)        0 2023-04-23 09:13:05.112582 Qcover-2.4.0/Qcover/research/
+-rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     7295 2023-02-27 09:19:50.000000 Qcover-2.4.0/Qcover/research/Ent_TMI.py
+-rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     5536 2022-09-02 08:09:52.000000 Qcover-2.4.0/Qcover/research/GHZ_Generate.py
+-rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     5737 2022-09-02 03:01:48.000000 Qcover-2.4.0/Qcover/research/QAOA_Generate.py
+-rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)        0 2022-05-30 09:03:08.000000 Qcover-2.4.0/Qcover/research/__init__.py
+-rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     6350 2023-02-27 09:07:40.000000 Qcover-2.4.0/Qcover/research/scrambling-OTOC.py
+drwxrwxrwx   0 ntyz      (1000) ntyz      (1000)        0 2023-04-23 09:13:05.117571 Qcover-2.4.0/Qcover/simulator/
+-rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)      155 2022-04-01 05:13:15.000000 Qcover-2.4.0/Qcover/simulator/__init__.py
+-rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     6053 2023-02-27 08:53:58.000000 Qcover-2.4.0/Qcover/simulator/qton.py
+-rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     3009 2022-09-01 02:55:28.000000 Qcover-2.4.0/Qcover/utils.py
+-rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)       95 2023-04-23 09:07:16.000000 Qcover-2.4.0/Qcover/version.py
+drwxrwxrwx   0 ntyz      (1000) ntyz      (1000)        0 2023-04-23 09:13:05.050749 Qcover-2.4.0/Qcover.egg-info/
+-rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     8394 2023-04-23 09:13:04.000000 Qcover-2.4.0/Qcover.egg-info/PKG-INFO
+-rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     1746 2023-04-23 09:13:04.000000 Qcover-2.4.0/Qcover.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)        1 2023-04-23 09:13:04.000000 Qcover-2.4.0/Qcover.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)      175 2023-04-23 09:13:04.000000 Qcover-2.4.0/Qcover.egg-info/requires.txt
+-rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)        7 2023-04-23 09:13:04.000000 Qcover-2.4.0/Qcover.egg-info/top_level.txt
+-rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     7262 2022-10-24 07:20:18.000000 Qcover-2.4.0/README.md
+-rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)       38 2023-04-23 09:13:05.119565 Qcover-2.4.0/setup.cfg
+-rwxrwxrwx   0 ntyz      (1000) ntyz      (1000)     2688 2023-04-18 06:00:38.000000 Qcover-2.4.0/setup.py
```

### Comparing `Qcover-2.3.0/LICENSE` & `Qcover-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Qcover-2.3.0/PKG-INFO` & `Qcover-2.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Qcover
-Version: 2.3.0
+Version: 2.4.0
 Summary: Quantum computing solver
 Home-page: https://github.com/BAQIS-Quantum/Qcover
 Author: ntyz&finleyzhuang
 Author-email: puyn@baqis.ac.cn
 License: Apache-2.0 License
 Project-URL: Bug Reports, https://github.com/BAQIS-Quantum/Qcover/issues
 Project-URL: Source, https://github.com/BAQIS-Quantum/Qcover
```

### Comparing `Qcover-2.3.0/Qcover/__init__.py` & `Qcover-2.4.0/Qcover/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import pkgutil
 
 # Allow extending this namespace. Please note that currently this line needs
 # to be placed *before* the wrapper imports or any non-import code AND *before*
 # importing the package you want to allow extensions for (in this case `backends`).
 __path__ = pkgutil.extend_path(__path__, __name__)
-__version__ = '2.3.0'
+__version__ = '2.4.0'
 __license__ = 'Apache-2.0 License'
 
 from Qcover.applications import *
 from Qcover.backends import *
 from Qcover.optimizers import *
```

### Comparing `Qcover-2.3.0/Qcover/applications/common.py` & `Qcover-2.4.0/Qcover/applications/common.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 """ common module """
 import time
 import random
 from collections import OrderedDict, defaultdict
 
 import numpy as np
 import networkx as nx
-from qiskit.aqua import aqua_globals
-from qiskit.aqua.operators import StateFn
+# from qiskit.aqua import aqua_globals
+# from qiskit.aqua.operators import StateFn
+
+from qiskit.utils import algorithm_globals
+# from qiskit.opflow import StateFn
 
 
 def get_ising_matrix(qubo_mat: np.array):
     """
     calculate the ising matrix according to the Q matrix of problems.
 
     Args:
@@ -142,11 +145,11 @@
         savefile (str or None): write numbers to this file.
         seed (Union(int,None)): random seed - if None, will not initialize.
 
     Returns:
         numpy.ndarray: the list of integer numbers.
     """
     if seed:
-        aqua_globals.random_seed = seed
+        algorithm_globals.random_seed = seed
 
-    number_list = aqua_globals.random.integers(low=weight_range[0], high=(weight_range[1] + 1), size=n)
+    number_list = algorithm_globals.random.integers(low=weight_range[0], high=(weight_range[1] + 1), size=n)
     return number_list
```

### Comparing `Qcover-2.3.0/Qcover/applications/general_01_programming.py` & `Qcover-2.4.0/Qcover/applications/general_01_programming.py`

 * *Files identical despite different names*

### Comparing `Qcover-2.3.0/Qcover/applications/graph_color.py` & `Qcover-2.4.0/Qcover/applications/graph_color.py`

 * *Files identical despite different names*

### Comparing `Qcover-2.3.0/Qcover/applications/max_2_sat.py` & `Qcover-2.4.0/Qcover/applications/max_2_sat.py`

 * *Files identical despite different names*

### Comparing `Qcover-2.3.0/Qcover/applications/max_cut.py` & `Qcover-2.4.0/Qcover/applications/max_cut.py`

 * *Files identical despite different names*

### Comparing `Qcover-2.3.0/Qcover/applications/minimum_vertex_cover.py` & `Qcover-2.4.0/Qcover/applications/minimum_vertex_cover.py`

 * *Files identical despite different names*

### Comparing `Qcover-2.3.0/Qcover/applications/number_partition.py` & `Qcover-2.4.0/Qcover/applications/number_partition.py`

 * *Files identical despite different names*

### Comparing `Qcover-2.3.0/Qcover/applications/qadratic_knapsack.py` & `Qcover-2.4.0/Qcover/applications/qadratic_knapsack.py`

 * *Files identical despite different names*

### Comparing `Qcover-2.3.0/Qcover/applications/quadratic_assignment.py` & `Qcover-2.4.0/Qcover/applications/quadratic_assignment.py`

 * *Files identical despite different names*

### Comparing `Qcover-2.3.0/Qcover/applications/set_packing.py` & `Qcover-2.4.0/Qcover/applications/set_packing.py`

 * *Files identical despite different names*

### Comparing `Qcover-2.3.0/Qcover/applications/set_partitioning.py` & `Qcover-2.4.0/Qcover/applications/set_partitioning.py`

 * *Files identical despite different names*

### Comparing `Qcover-2.3.0/Qcover/applications/sherrington_kirkpatrick.py` & `Qcover-2.4.0/Qcover/applications/sherrington_kirkpatrick.py`

 * *Files identical despite different names*

### Comparing `Qcover-2.3.0/Qcover/backends/backend.py` & `Qcover-2.4.0/Qcover/backends/backend.py`

 * *Files 19% similar despite different names*

```diff
@@ -27,30 +27,18 @@
         self._edges_weight = edges_weight
         self._is_parallel = False if is_parallel is None else is_parallel
 
         self._element_to_graph = None
         self._pargs = None
         self._element_expectation = dict()
 
-    # @abstractmethod
-    # def get_operator(self, *args):
-    #     pass
-
     @abstractmethod
     def get_expectation(self, *args):
         pass
 
     @abstractmethod
     def expectation_calculation(self):
         pass
 
     @abstractmethod
-    def get_result_counts(self, params):
-        pass
-
-    @abstractmethod
     def optimization_visualization(self):
         pass
-
-    @abstractmethod
-    def sampling_visualization(self, counts):
-        pass
```

### Comparing `Qcover-2.3.0/Qcover/backends/circuitbycirq.py` & `Qcover-2.4.0/Qcover/backends/circuitbycirq.py`

 * *Files identical despite different names*

### Comparing `Qcover-2.3.0/Qcover/backends/circuitbyprojectq.py` & `Qcover-2.4.0/Qcover/backends/circuitbyprojectq.py`

 * *Files identical despite different names*

### Comparing `Qcover-2.3.0/Qcover/backends/circuitbyqiskit.py` & `Qcover-2.4.0/Qcover/backends/circuitbyqiskit.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 import time
 from collections import defaultdict, Callable
 import numpy as np
 import matplotlib.pyplot as plt
 from multiprocessing import Pool, cpu_count
 
 from qiskit import QuantumCircuit, QuantumRegister, ClassicalRegister, Aer, assemble, BasicAer, transpile
-from qiskit.aqua import QuantumInstance, aqua_globals
-from qiskit.aqua.operators import PauliExpectation, CircuitSampler, StateFn, CircuitOp, CircuitStateFn, \
+
+from qiskit.utils import QuantumInstance
+from qiskit.opflow import PauliExpectation, CircuitSampler, StateFn, CircuitOp, CircuitStateFn, \
     MatrixExpectation, X, Y, Z, I
 
 from Qcover.utils import get_graph_weights
 from Qcover.backends import Backend
 import warnings
 warnings.filterwarnings("ignore")
 
@@ -134,23 +135,24 @@
             weight = self._nodes_weight[original_e]
             op = self.get_operator([node_to_qubit[original_e]], len(node_list))
         else:
             weight = self._edges_weight[original_e]
             op = self.get_operator([node_to_qubit[original_e[0]], node_to_qubit[original_e[1]]], len(node_list))
 
         if self._expectation_calc_method == "statevector":
-            circ.save_statevector()
+            # circ.save_statevector()
             sim = Aer.get_backend('qasm_simulator')  #aer
+            circ.save_statevector()
             result = sim.run(circ, seed_simulator=47, nshots=102400).result()
             out_state = result.get_statevector()
             exp_res = np.matmul(np.matmul(out_state.conj().T, op), out_state).real
 
         elif self._expectation_calc_method == "sample":
-            subc = CircuitStateFn(circ)
             backend = Aer.get_backend('qasm_simulator')
+            subc = CircuitStateFn(circ)
             q_instance = QuantumInstance(backend, shots=1024)
             measurable_expression = StateFn(op, is_measurement=True).compose(subc)
             expectation = PauliExpectation().convert(measurable_expression)
             sampler = CircuitSampler(q_instance).convert(expectation)
             exp_res = sampler.eval().real
 
         elif self._expectation_calc_method == "statistic":
```

### Comparing `Qcover-2.3.0/Qcover/backends/circuitbyqiskit_statistic.py` & `Qcover-2.4.0/Qcover/backends/circuitbyqiskit_statistic.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,21 @@
 import time
 from collections import defaultdict, Callable
 import numpy as np
 import matplotlib.pyplot as plt
 from multiprocessing import Pool, cpu_count
 
 from qiskit import QuantumCircuit, QuantumRegister, ClassicalRegister, Aer, assemble, BasicAer, transpile
-from qiskit.aqua import QuantumInstance, aqua_globals
-from qiskit.aqua.operators import PauliExpectation, CircuitSampler, StateFn, CircuitOp, CircuitStateFn, \
+
+# from qiskit.aqua import QuantumInstance, aqua_globals
+# from qiskit.aqua.operators import PauliExpectation, CircuitSampler, StateFn, CircuitOp, CircuitStateFn, \
+#     MatrixExpectation, X, Y, Z, I
+
+from qiskit.utils import QuantumInstance
+from qiskit.opflow import PauliExpectation, CircuitSampler, StateFn, CircuitOp, CircuitStateFn, \
     MatrixExpectation, X, Y, Z, I
 
 from Qcover.utils import get_graph_weights
 from Qcover.backends import Backend
 import warnings
 warnings.filterwarnings("ignore")
```

### Comparing `Qcover-2.3.0/Qcover/backends/circuitbyqton.py` & `Qcover-2.4.0/Qcover/backends/circuitbyqton.py`

 * *Files identical despite different names*

### Comparing `Qcover-2.3.0/Qcover/backends/circuitbyqulacs.py` & `Qcover-2.4.0/Qcover/backends/circuitbyqulacs.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 class CircuitByQulacs(Backend):
     """generate a instance of CircuitByQulacs"""
 
     def __init__(self,
                  research: str = "QAOA",
                  is_parallel: bool = None) -> None:
-        """initialize a instance of CircuitByCirq"""
+        """initialize a instance of CircuitByQualacs"""
         super(CircuitByQulacs, self).__init__()
 
         self._p = None
         self._origin_graph = None
         self._is_parallel = False if is_parallel is None else is_parallel
         self._research = research
```

### Comparing `Qcover-2.3.0/Qcover/backends/circuitbytensor.py` & `Qcover-2.4.0/Qcover/backends/circuitbytensor.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,35 +2,36 @@
 import os
 import time
 import warnings
 from collections import defaultdict, Callable
 import matplotlib.pyplot as plt
 from multiprocessing import Pool, cpu_count
 import quimb as qu
+import quimb.tensor as qtn
 from multiprocessing import cpu_count
 from Qcover.backends import Backend
+from Qcover.utils import get_graph_weights
 
 
 class CircuitByTensor(Backend):
     """generate a instance of tensor network circuit generated by quimb"""
 
     def __init__(self,
-                 nodes_weight: list = None,
-                 edges_weight: list = None,
                  contract_opt: str = 'greedy',
                  is_parallel: bool = None) -> None:
 
         """initialize a instance of tensor network circuit:"""
 
         super(CircuitByTensor, self).__init__()
         self._p = None
-        self._nodes_weight = nodes_weight
-        self._edges_weight = edges_weight
+        self._nodes_weight = None
+        self._edges_weight = None
         self._is_parallel = False if is_parallel is None else is_parallel
         self._opt = contract_opt
+        self._origin_graph = None
 
         self._element_to_graph = None
         self._pargs = None
         self._expectation_path = []
         self._element_expectation = dict()
 
     @property
@@ -49,29 +50,28 @@
             original_e, graph = element_graph[0]
 
         node_to_qubit = defaultdict(int)
         node_list = list(graph.nodes)
         for i in range(len(node_list)):
             node_to_qubit[node_list[i]] = i
 
+        circ = qtn.Circuit(len(graph.nodes))
         gamma_list, beta_list = self._pargs[: p], self._pargs[p:]
-        circ = qu.tensor.Circuit(len(graph.nodes))
-
         for k in range(p):
             for nd in graph.nodes:
                 u = node_to_qubit[nd]
                 if k == 0:
                     circ.apply_gate('H', u)
                 circ.apply_gate('rz', 2 * gamma_list[k] * self._nodes_weight[nd], u)
 
             for edge in graph.edges:
                 u, v = node_to_qubit[edge[0]], node_to_qubit[edge[1]]
                 if u == v:
                     continue
-                circ.apply_gate('RZZ', -gamma_list[k] * self._edges_weight[edge[0], edge[1]], u, v)
+                circ.apply_gate('RZZ', 2 * gamma_list[k] * self._edges_weight[edge[0], edge[1]], u, v)
 
             for nd in graph.nodes:
                 circ.apply_gate('rx', 2 * beta_list[k], node_to_qubit[nd])
 
         if isinstance(original_e, int):
             weight = self._nodes_weight[original_e]
             where = node_to_qubit[original_e]
@@ -80,14 +80,18 @@
             weight = self._edges_weight[original_e]
             ZZ = qu.pauli('Z') & qu.pauli('Z')
             where = (node_to_qubit[original_e[0]], node_to_qubit[original_e[1]])
             exp_res = circ.local_expectation(ZZ, where, optimize=self._opt)
         return weight, exp_res.real
 
     def expectation_calculation(self, p=None):
+        if self._nodes_weight is None or self._edges_weight is None:
+            nodes_weight, edges_weight = get_graph_weights(self._origin_graph)
+            self._nodes_weight, self._edges_weight = nodes_weight, edges_weight
+
         self._element_expectation = {}
         if self._is_parallel:
             return self.expectation_calculation_parallel(p)
         else:
             return self.expectation_calculation_serial(p)
 
     def expectation_calculation_serial(self, p=None):
```

### Comparing `Qcover-2.3.0/Qcover/compiler/compilerforQAOA.py` & `Qcover-2.4.0/Qcover/compiler/compilerforQAOA.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 import networkx as nx
-# import itertools
-# import numpy as np
 import random
-from qiskit import QuantumCircuit, QuantumRegister
 import math
 from collections import defaultdict
 import copy
 import re
 import matplotlib.pyplot as plt
 import os
 from .hardware_library import BuildLibrary
@@ -76,41 +73,40 @@
             for i in range(0, self._logical_qubits):
                 qubits_mapping[i] = phys_qubits_order[i]
             return qubits_mapping
         else:
             print("Error: physical qubits must be larger than logical qubits")
 
     def QAOA_logical_circuit(self):
-        lc = QuantumRegister(len(self._nodes), 'l')
-        logical_circ = QuantumCircuit(lc)
+        logical_circ = quafuQC(len(self._nodes))
         graph_edges = dict(
             [(tuple(sorted(list(self._edges)[i][0:2])), list(self._edges)[i][2]) for i in range(0, len(self._edges))])
         graph_nodes = dict(self._nodes)
         gamma, beta = self._optimal_params[:self._p], self._optimal_params[self._p:]
         for i in range(len(graph_nodes)):
             logical_circ.h(i)
         for k in range(0, self._p):
-            # logical_circ.barrier()
             for u, v in graph_nodes.items():
-                logical_circ.rz(2 * gamma[k] * v, u)
+                logical_circ.rz(u, 2 * gamma[k] * v)
             for u, v in graph_edges.items():
-                logical_circ.rzz(2 * gamma[k] * v, u[0], u[1])
+                logical_circ.rzz(u[0], u[1], 2 * gamma[k] * v)
             for u, v in graph_nodes.items():
-                logical_circ.rx(2 * beta[k], u)
+                logical_circ.rx(u, 2 * beta[k])
         return logical_circ
 
     def sorted_nodes_degree(self):
         """
         Returns:
             sort_nodes (np.array): nodes are sorted by node degree in descending order
         """
         node_degree = dict(self._g.degree)
-        sort_degree = sorted(node_degree.items(), key=lambda kv: kv[1], reverse=True)
+        # sort_degree = sorted(node_degree.items(), key=lambda kv: kv[1], reverse=True)
+        sort_degree = sorted(node_degree.items(), key=lambda kv: kv[1], reverse=False)
         sort_nodes = [sort_degree[i][0] for i in range(len(sort_degree))]
-        return sort_nodes
+        return sort_degree
 
     def scheduled_pattern_rzz_swap(self, qubits_mapping):
         """
         Get the fixed execution pattern of the QAOA circuit.
         Args:
             qubits_mapping (dict): {physical qubit: logical qubit}
                         example: {0: 1, 1: 2, 2: 0}
@@ -164,27 +160,55 @@
         if self._logical_qubits % 2 == 1:
             pattern_rzz_swap.pop(cycle - 1)
             for item in pattern_rzz_swap[0]:
                 rzz_gates_cycle[item[0]] = [0, item[1]]
         return pattern_rzz_swap, rzz_gates_cycle
 
     def best_initial_mapping(self, rzz_gates_cycle, truncation=5):
+        """
+        # Get the best initial mapping from rzz swap gates template.
+        Args:
+            rzz_gates_cycle (dict): rzz gate execution in k-th cycle, {(q1,q2): k, ...}
+            truncation (int):  # The larger the truncation, the more likely it is to find the
+                                # optimal initial mapping, but the time cost increases.
+        Returns:
+            best_phys2logi_mapping: {physical qubit: logical qubit}
+        """
         simple_mapping = self.simple_layout_mapping()
         sorted_nodes = self.sorted_nodes_degree()
         rzz_gates_cycle = {tuple(sorted(k)): v[0] for k, v in rzz_gates_cycle.items()}
         mapping_logi2phys_list = []
-        # mapping_logi2phys_list.append(({sorted_nodes[0]: 0}, 0))
-        for n in range(len(sorted_nodes)):
-            mapping_logi2phys_list.append(({sorted_nodes[0]: n}, 0))
+        # for n in range(len(sorted_nodes)):
+        #     mapping_logi2phys_list.append(({sorted_nodes[0]: n}, 0))
+
+        # The map is initialized in order for nodes with node degree 0.
+        # TODO: In the future it may be initialized with hardware fidelity.
+        degree_zero_map = {}
+        bit = 0
+        for node in sorted_nodes:
+            if node[1]==0:
+                degree_zero_map[node[0]] = bit
+                bit += 1
+            else:
+                break
+
+        for i in range(0, bit):
+            sorted_nodes.pop(0)
+
+        sorted_nodes_big = sorted(sorted_nodes, key=lambda kv: kv[1], reverse=True)
+        for n in range(0, len(sorted_nodes_big)):
+            init_map = copy.deepcopy(degree_zero_map)
+            init_map[sorted_nodes_big[0][0]] = n + bit
+            mapping_logi2phys_list.append((init_map, 0))
+
+
         last_cycle = max(rzz_gates_cycle.values())
-        # truncation = truncation
-        # The larger the truncation, the more likely it is to find the optimal initial mapping,
-        # but the time cost increases.
-        for item in range(1, len(sorted_nodes)):
-            node = sorted_nodes[item]
+
+        for item in range(1, len(sorted_nodes_big)):
+            node = sorted_nodes_big[item][0]
             update_mapping_list = []
             for mapping_path in mapping_logi2phys_list:
                 q2p_path = mapping_path[0]
                 used_physical_bits = list(q2p_path.values())
                 used_logical_bits = list(q2p_path.keys())
                 for phys_bit in range(self._logical_qubits):
                     deepest_cycle = mapping_path[1]
@@ -201,19 +225,21 @@
                             if max_depth > deepest_cycle:
                                 deepest_cycle = max_depth
                             if deepest_cycle == 0:
                                 update_mapping_list.append((q2p_path, deepest_cycle))
                             else:
                                 if [depth for _, depth in update_mapping_list].count(deepest_cycle) < truncation:
                                     update_mapping_list.append((q2p_path, deepest_cycle))
-            mapping_logi2phys_list = copy.deepcopy(update_mapping_list)
+            if len(update_mapping_list)>1000:
+                update_mapping_list = sorted(update_mapping_list, key=lambda x: x[1], reverse=False)
+                mapping_logi2phys_list = copy.deepcopy(update_mapping_list[0:1000])
+            else:
+                mapping_logi2phys_list = copy.deepcopy(update_mapping_list)
 
         mapping_logi2phys_list = sorted(mapping_logi2phys_list, key=lambda x: x[1])
-        # print(mapping_logi2phys_list[0:50])
-        # print(len(mapping_logi2phys_list))
         if mapping_logi2phys_list:
             best_phys2logi_mapping = {v: k for k, v in mapping_logi2phys_list[0][0].items()}
         else:
             best_phys2logi_mapping = simple_mapping
         return best_phys2logi_mapping
 
     def QAOA_physical_circuit(self, pattern_rzz_swap, qubits_mapping):
@@ -312,27 +338,36 @@
             for i in direction:
                 depth = depth + 1
                 for j in range(len(first_gates_scheduled[i])):
                     if first_gates_scheduled[i][j][0] == 'Rz':
                         u = first_gates_scheduled[i][j][1][0]
                         nodes_weight = first_gates_scheduled[i][j][1][1]
                         u = {v: k for k, v in qubits_mapping_initial.items()}[u]
-                        final_gates_scheduled[depth].append(
-                            ('Rz', (u, 2 * gamma[k] * nodes_weight),
-                             (qubits_mapping_initial[u], 2 * gamma[k] * nodes_weight)))
+                        # final_gates_scheduled[depth].append(
+                        #     ('Rz', (u, 2 * gamma[k] * nodes_weight),
+                        #      (qubits_mapping_initial[u], 2 * gamma[k] * nodes_weight)))
+                        if nodes_weight != 0:
+                            final_gates_scheduled[depth].append(
+                                ('Rz', (u, 2 * gamma[k] * nodes_weight),
+                                 (qubits_mapping_initial[u], 2 * gamma[k] * nodes_weight)))
 
                     if first_gates_scheduled[i][j][0] == 'Rzz':
                         u, v = first_gates_scheduled[i][j][1][0]
                         edges_weight = first_gates_scheduled[i][j][1][1]
                         u = {v: k for k, v in qubits_mapping_initial.items()}[u]
                         v = {v: k for k, v in qubits_mapping_initial.items()}[v]
-                        final_gates_scheduled[depth].append(
-                            ('Rzz', ((u, v), 2 * gamma[k] * edges_weight),
-                             ((qubits_mapping_initial[u], qubits_mapping_initial[v]),
-                              2 * gamma[k] * edges_weight)))
+                        # final_gates_scheduled[depth].append(
+                        #     ('Rzz', ((u, v), 2 * gamma[k] * edges_weight),
+                        #      ((qubits_mapping_initial[u], qubits_mapping_initial[v]),
+                        #       2 * gamma[k] * edges_weight)))
+                        if edges_weight != 0:
+                            final_gates_scheduled[depth].append(
+                                ('Rzz', ((u, v), 2 * gamma[k] * edges_weight),
+                                 ((qubits_mapping_initial[u], qubits_mapping_initial[v]),
+                                  2 * gamma[k] * edges_weight)))
 
                     if first_gates_scheduled[i][j][0] == 'SWAP':
                         u, v = first_gates_scheduled[i][j][1]
                         u = {v: k for k, v in qubits_mapping_initial.items()}[u]
                         v = {v: k for k, v in qubits_mapping_initial.items()}[v]
                         final_gates_scheduled[depth].append(
                             ('SWAP', (u, v),
@@ -412,15 +447,15 @@
             if rearrange_gates_scheduled[i]:
                 final_gates_scheduled[k] = rearrange_gates_scheduled[i]
                 k = k + 1
 
         return final_gates_scheduled, qubits_mapping_initial
 
     def gates_decomposition(self, final_gates_scheduled):
-        # gates decomposition
+        # Decompose RZZ gates and SWAP gates into CNOT and single-qubit gates
         hardware_gates_scheduled = list([])
         for i in range(len(final_gates_scheduled)):
             layer_list = list([])
             layer_list1 = list([])
             layer_list2 = list([])
             for j in range(len(final_gates_scheduled[i])):
                 if final_gates_scheduled[i][j][0] == 'H':
@@ -464,88 +499,94 @@
                 hardware_gates_scheduled.append(layer_list1)
             if layer_list2:
                 hardware_gates_scheduled.append(layer_list2)
         return hardware_gates_scheduled
 
     def cnot_gates_optimization(self, hardware_gates_scheduled, physical_qubits=None):
         # CNOT gates optimization
-        # Two identical CNOT gates adjacent to each other are eliminated:
-        # CNOT(i,j)CNOT(i,j) = identity matrix
+        # Two identical CNOT gates adjacent to each other are eliminated: CNOT(i,j)CNOT(i,j) = identity matrix
         depth = len(hardware_gates_scheduled)
         opt_hardware_gates_scheduled = copy.deepcopy(hardware_gates_scheduled)
         for i in range(depth - 1):
             next_list = [hardware_gates_scheduled[i + 1][k][1] for k in
                          range(len(hardware_gates_scheduled[i + 1]))]
             for j in range(len(hardware_gates_scheduled[i])):
                 if hardware_gates_scheduled[i][0][0] == 'CNOT':
                     if hardware_gates_scheduled[i][j][1] in next_list:
                         opt_hardware_gates_scheduled[i].remove(hardware_gates_scheduled[i][j])
                         opt_hardware_gates_scheduled[i + 1].remove(hardware_gates_scheduled[i][j])
         opt_hardware_gates_scheduled = list(filter(None, opt_hardware_gates_scheduled))
 
         if physical_qubits is not None:
-            oq = QuantumRegister(physical_qubits, 'q')
-            optimized_circuit = QuantumCircuit(oq)
+            optimized_circuit = quafuQC(physical_qubits)
             for i in range(len(opt_hardware_gates_scheduled)):
                 for j in range(len(opt_hardware_gates_scheduled[i])):
                     if opt_hardware_gates_scheduled[i][j][0] == 'H':
                         optimized_circuit.h(opt_hardware_gates_scheduled[i][j][1])
                     if opt_hardware_gates_scheduled[i][j][0] == 'Rz':
                         _, v, theta = opt_hardware_gates_scheduled[i][j]
-                        optimized_circuit.rz(theta, v)
+                        optimized_circuit.rz(v, theta)
                     if opt_hardware_gates_scheduled[i][j][0] == 'Rx':
                         _, v, theta = opt_hardware_gates_scheduled[i][j]
-                        optimized_circuit.rx(theta, v)
+                        optimized_circuit.rx(v, theta)
                     if opt_hardware_gates_scheduled[i][j][0] == 'CNOT':
                         _, q = opt_hardware_gates_scheduled[i][j]
-                        optimized_circuit.cx(q[0], q[1])
+                        optimized_circuit.cnot(q[0], q[1])
         else:
             optimized_circuit = None
         return opt_hardware_gates_scheduled, optimized_circuit
 
     def graph_to_qasm(self):
+        # Convert weight graph to openqasm circuit.
         qubits_mapping = self.simple_layout_mapping()
         pattern_rzz_swap, rzz_gates_cycle = self.scheduled_pattern_rzz_swap(qubits_mapping)
         best_phys2logi_mapping = self.best_initial_mapping(rzz_gates_cycle)
-        print('best',best_phys2logi_mapping)
         pattern_rzz_swap_new = defaultdict(list)
         for k, v in pattern_rzz_swap.items():
             for gate in v:
                 pattern_rzz_swap_new[k].append(
                     [(best_phys2logi_mapping[gate[0][0]], best_phys2logi_mapping[gate[0][1]]), gate[1]])
 
         final_gates_scheduled, final_phys2logi_mapping = self.QAOA_physical_circuit(pattern_rzz_swap_new,
                                                                                     best_phys2logi_mapping)
         hardware_gates_scheduled = self.gates_decomposition(final_gates_scheduled)
         opt_hardware_gates_scheduled, ScQ_circuit = self.cnot_gates_optimization(
             hardware_gates_scheduled, physical_qubits=self._physical_qubits)
-        ScQ_circuit.measure_all()
-        openqasm = ScQ_circuit.qasm()
+        # ScQ_circuit.measure_all()
+        openqasm = ScQ_circuit.to_openqasm()
         return openqasm, final_phys2logi_mapping, ScQ_circuit
 
     def scq_qasm(self, openqasm):
+        # Compile openqasm into scq_qasm executed by quafu quantum chips.
         user = User()
         user.save_apitoken(self._apitoken)
         backend = self._cloud_backend
         task = Task()
-        # task.load_account()
         task.config(backend=backend)
         backend_info = task.get_backend_info()
         plt.close()
         calibration_time = backend_info['full_info']["calibration_time"]
         logical_qubits = int(re.findall(r"\d+\.?\d*", openqasm.split('qreg')[1].split(';')[0])[0])
 
         build_library = BuildLibrary(backend=backend, fidelity_threshold=96)
-        if not os.path.exists('LibSubstructure_' + backend + '.txt'):
+
+        dir_path = os.path.dirname(os.path.abspath(__file__))
+        folder_path = os.path.join(dir_path, "backend_library")
+        if not os.path.exists(folder_path):
+            os.mkdir(folder_path)
+
+        file_path = os.path.join(folder_path, 'LibSubstructure_' + backend + '.txt')
+
+        if not os.path.exists(file_path):
             print(
                 "The subgraph library of " + backend + " quantum chip does not exist. Please wait: creating subgraph library!")
             substructure_data = build_library.build_substructure_library()
             print('Complete building!')
         else:
-            with open('LibSubstructure_' + backend + '.txt', 'r', encoding='utf-8') as f:
+            with open(file_path, 'r', encoding='utf-8') as f:
                 substructure_data = eval(f.read())
                 if substructure_data['calibration_time'] != calibration_time:
                     print(
                         "The qubits of " + backend + " quantum chip have been recalibrated. Please wait: updating the subgraph library of the corresponding quantum chip!")
                     build_library.build_substructure_library()
                     print('Complete building!')
                 else:
@@ -553,25 +594,28 @@
                         "The information of qubits are unchanged, and the existing subgraph library is directly called!")
 
         physical_qubits = len(substructure_data['qubit_to_int'])
         scq_qasm = openqasm.replace('qreg q[' + str(logical_qubits),
                                     'qreg q[' + str(physical_qubits))
 
         if backend == "ScQ-P136":
-            scq_qasm = re.sub(r'barrier.*\n', "", scq_qasm)
-            if not os.path.exists('LibSubchain_' + backend + '.txt'):
-                print("The one-dimensional chain library of " + backend + " quantum chip does not exist, and is being created!")
-                chain_data = build_library.chain_library_2D(substructure_data)
+            # scq_qasm = re.sub(r'barrier.*\n', "", scq_qasm)
+            file_path = os.path.join(folder_path, 'LibSubchain_' + backend + '.txt')
+            if not os.path.exists(file_path):
+                print(
+                    "The one-dimensional chain library of " + backend + " quantum chip does not exist, and is being created!")
+                chain_data = build_library.build_chains_from_longest(substructure_data)
                 print('Complete building!')
             else:
-                with open('LibSubchain_' + backend + '.txt', 'r', encoding='utf-8') as f:
+                with open(file_path, 'r', encoding='utf-8') as f:
                     chain_data = eval(f.read())
                     if chain_data['calibration_time'] != calibration_time:
-                        print("Waiting: Building a library of one-dimensional chain structures for the " + backend + " quantum chip!")
-                        chain_data = build_library.chain_library_2D(substructure_data)
+                        print(
+                            "Waiting: Building a library of one-dimensional chain structures for the " + backend + " quantum chip!")
+                        chain_data = build_library.build_chains_from_longest(substructure_data)
                         print('Complete building!')
 
             longset_chain = max(chain_data['subchain_dict'].keys())
             if logical_qubits > longset_chain:
                 raise SystemExit(
                     "Currently, " + backend + " quantum chip supports a maximum of " + str(longset_chain) + " qubits!")
 
@@ -613,20 +657,49 @@
             for coupling in sub_clist:
                 if coupling[0] not in qubits_list:
                     qubits_list.append(coupling[0])
                 if coupling[1] not in qubits_list:
                     qubits_list.append(coupling[1])
             qubits_list = sorted(qubits_list)
 
-        print('physical qubits used:\n', qubits_list)
+        print('Physical qubits used:\n', qubits_list)
 
+        # req_to_q = {q: qubits_list[q] for q in range(len(qubits_list))}
+        # for req, q in sorted(req_to_q.items(), key=lambda item: item[1], reverse=True):
+        #     print('req, q',req, q)
+        #     scq_qasm = scq_qasm.replace('q[' + str(req) + ']', 'q[' + str(q) + ']')
+        # scq_qasm = scq_qasm.replace('meas[', 'c[')
+        # plt.close()
+        # print('scq_qasm \n',scq_qasm)
+
+        # lines = scq_qasm.split('\n')
+        # print('oldlines', lines)
+        old_qubits = []
+        new_qubits = []
         req_to_q = {q: qubits_list[q] for q in range(len(qubits_list))}
         for req, q in sorted(req_to_q.items(), key=lambda item: item[1], reverse=True):
-            scq_qasm = scq_qasm.replace('q[' + str(req) + ']', 'q[' + str(q) + ']')
+            old_qubits.append(req)
+            new_qubits.append(q)
+        old_qubit_pattern = r'q\[(\d+)\]'
+        new_qubit_template = r'q[{}]'
+
+        # Put the 'q[int]' number in a capturing group and replace with the contents of the capturing group
+        def replace_qubits(match):
+            old_qubit = int(match.group(1))
+            if old_qubit in old_qubits:
+                new_qubit = new_qubits[old_qubits.index(old_qubit)]
+                return new_qubit_template.format(new_qubit)
+            else:
+                return match.group(0)
+
+        # Replace the 'q[int]' number in the string with a new number
+        scq_qasm = re.sub(old_qubit_pattern, replace_qubits, scq_qasm)
         scq_qasm = scq_qasm.replace('meas[', 'c[')
+        # lines = scq_qasm.split('\n')
+        # print('newlines', lines)
         plt.close()
         return scq_qasm
 
     def send(self, wait=True, shots=1024, task_name: str = ''):
         """
         Send the task to the quafu cloud platform.
         Args:
@@ -636,35 +709,37 @@
                          without waiting online for the results to return.
             shots (int): The number of sampling of quantum computer.
             task_name (str): The name of the task so that you can query the task status
                              on the quafu cloud platform later.
         Returns:
             task_id (str): The ID number of the task, which can uniquely identify the task.
         """
-        openqasm, final_phys2logi_mapping, _ = self.graph_to_qasm()
+        openqasm, final_phys2logi_mapping, ScQ_circuit = self.graph_to_qasm()
+        print('The depth of compiled circuit: ', len(ScQ_circuit.layered_circuit()[0]))
+        print('The number of CNOT gates: ', openqasm.count('cx'))
+        print('The number of single-qubit gates (Rx,Rz,H): ', openqasm.count('h') +
+              openqasm.count('rx') + openqasm.count('rz'))
         self._logi2phys_mapping = {v: k for k, v in final_phys2logi_mapping.items()}
         scq_qasm = self.scq_qasm(openqasm)
-        # send to quafu cloud
+        # Send to quafu cloud
         qubits = int(re.findall(r"\d+\.?\d*", scq_qasm.split('qreg')[1].split(';')[0])[0])
         q = quafuQC(qubits)
         q.from_openqasm(scq_qasm)
         task = Task()
-        # task.load_account()
         task.config(backend=self._cloud_backend, shots=shots, compile=False)
         task_id = task.send(q, wait=wait, name=task_name, group=task_name).taskid
         print("The task has been submitted to the quafu cloud platform.\nThe task ID is '%s'" % task_id)
         return task_id
 
     def task_status_query(self, task_id: str):
         task = Task()
-        # task.load_account()
         task_status = task.retrieve(task_id).task_status
-        if task_status=='In Queue' or task_status=='Running':
+        if task_status == 'In Queue' or task_status == 'Running':
             print("The current task status is '%s', please wait." % task_status)
-        elif task_status=='Completed':
+        elif task_status == 'Completed':
             print("The task execution has completed and the result has been returned.")
             res = task.retrieve(task_id)
             return res
 
     def right_left_counts_rearrange(self, logi2phys_mapping, counts):
         # The bits are arranged as 0, 1, 2,... from right to the left.
         qubit_str = list(counts.keys())
@@ -689,47 +764,47 @@
 
     def graph_sampling_energy_ising(self, counts):
         # Obtain QAOA energy from circuit sampling results
         counts_energy = {}
         for i in range(len(counts)):
             # 0 -> -1, 1 -> 1
             result1 = [int(u) for u in list(counts[i][0])]
-            # result1.reverse()
             energy1 = 0
             for node in self._nodes:
                 energy1 = energy1 + node[1] * (2 * result1[node[0]] - 1)
             for edge in self._edges:
-                energy1 = energy1 + 2* edge[2] * (2 * result1[edge[0]] - 1) * (2 * result1[edge[1]] - 1)
+                energy1 = energy1 + 2 * edge[2] * (2 * result1[edge[0]] - 1) * (2 * result1[edge[1]] - 1)
             counts_energy[counts[i]] = energy1
         counts_energy = sorted(counts_energy.items(), key=lambda x: x[1])
         return counts_energy
 
     def graph_sampling_energy_qubo(self, counts):
-        # Obtain QUBO cost from circuit sampling results
+        # Obtain QUBO cost from circuit sampling results.
         counts_energy = {}
         import numpy as np
         qubo_mat = np.zeros([len(self._nodes), len(self._nodes)])
         ising_mat = np.zeros([len(self._nodes), len(self._nodes)])
         for edge in self._edges:
             ising_mat[edge[0], edge[1]] = edge[2]
             ising_mat[edge[1], edge[0]] = edge[2]
-            qubo_mat[edge[0], edge[1]] = 4*edge[2]/2.
-            qubo_mat[edge[1], edge[0]] = 4*edge[2]/2.
+            qubo_mat[edge[0], edge[1]] = 4 * edge[2] / 2.
+            qubo_mat[edge[1], edge[0]] = 4 * edge[2] / 2.
         for node in self._nodes:
-            ising_mat[node[0],node[0]] = node[1]
-            qubo_mat[node[0],node[0]] = (node[1]-sum(2.*qubo_mat[node[0]]/4.))*2
+            ising_mat[node[0], node[0]] = node[1]
+            qubo_mat[node[0], node[0]] = (node[1] - sum(2. * qubo_mat[node[0]] / 4.)) * 2
         for i in range(len(counts)):
             result1 = np.array([int(u) for u in list(counts[i][0])])
             energy1 = np.dot(np.dot(result1, qubo_mat), result1)
             counts_energy[counts[i]] = energy1
         counts_energy = sorted(counts_energy.items(), key=lambda x: x[1])
-        # print('qubo_mat',qubo_mat)
         return counts_energy
 
     def results_processing(self, results):
+        # The sampling result is the distribution of hardware physical qubit strings,
+        # and the physical qubits need to be mapped back to the weight graph nodes.
         counts_ScQ0 = results.res
         logi2phys_mapping = self._logi2phys_mapping
         counts_ScQ_new = self.left_right_counts_rearrange(logi2phys_mapping, counts_ScQ0)
         counts_ScQ = sorted(counts_ScQ_new.items(), key=lambda x: x[1], reverse=True)
         counts_ScQ = [(item[0], item[1]) for item in counts_ScQ]
 
         for elem in counts_ScQ:
@@ -737,61 +812,72 @@
                 counts_ScQ.remove(elem)
 
         counts_energy = self.graph_sampling_energy_qubo(counts_ScQ)
         print('Results ((qubits str, number of sampling), QUBO Cost):\n', counts_energy)
         return counts_energy
 
     def visualization(self, counts_energy, problem='MaxCut', solutions=3, problem_graph=None):
-        # draw result
+        """
+            Visualize optimal solutions to combinatorial optimization problems
+            based on sampling results from quafu hardware.
+        Args:
+            counts_energy: self.results_processing()
+            problem: Visualization of two types of problems is currently supported, 'MaxCut' or 'GraphColoring'
+            solutions: Visualize the top "solutions" optimal solutions
+            problem_graph: original problem graph
+        """
         plt.close()
         print('Send results to client:')
-        if problem=='MaxCut':
+        if problem == 'MaxCut':
             for s in range(solutions):
                 optimal_solution = counts_energy[s][0][0]
                 cut_node1 = []
                 cut_node2 = []
                 for i in range(len(optimal_solution)):
                     if optimal_solution[i] == '0':
                         cut_node1.append(i)
                     else:
                         cut_node2.append(i)
                 pos = nx.spring_layout(self._g)
                 # pos = nx.circular_layout(self._g)
-                nx.draw_networkx(self._g, pos=pos, nodelist=cut_node1, node_size=500, node_color='c', font_size=15, width=2)
-                nx.draw_networkx(self._g, pos=pos, nodelist=cut_node2, node_size=500, node_color='r', font_size=15, width=2)
+                nx.draw_networkx(self._g, pos=pos, nodelist=cut_node1, node_size=500, node_color='c', font_size=15,
+                                 width=2)
+                nx.draw_networkx(self._g, pos=pos, nodelist=cut_node2, node_size=500, node_color='r', font_size=15,
+                                 width=2)
                 nx.draw_networkx_edges(self._g, pos, width=2, edge_color='g', arrows=False)
                 # plt.axis('off')
                 plt.tight_layout()
                 plt.show()
-                print('======== Solution ' + str(1+s) + ' ========')
+                print('======== Solution ' + str(1 + s) + ' ========')
                 print('Cluster 1:', sorted(cut_node1))
                 print('Cluster 2:', sorted(cut_node2))
                 print('Cost (QUBO):', counts_energy[s][1])
-        elif problem=='GraphColoring':
+        elif problem == 'GraphColoring':
             import matplotlib.colors
             color_list = ['r', 'c', 'b', 'y', 'm']
             color_list = color_list + list(matplotlib.colors.cnames.values())
             nodes = len(problem_graph.nodes)
-            color_num = int(len(counts_energy[0][0][0])/nodes)
+            color_num = int(len(counts_energy[0][0][0]) / nodes)
             for s in range(solutions):
                 print('======== Solution ' + str(1 + s) + ' ========')
                 optimal_solution = counts_energy[s][0][0]
                 qubo_bits = []
                 for n in range(0, nodes):
-                    qubo_bits.append(optimal_solution[n*color_num:(n+1)*color_num])
+                    qubo_bits.append(optimal_solution[n * color_num:(n + 1) * color_num])
                 color_dic = {}
                 for k in range(nodes):
                     color_dic.setdefault(qubo_bits[k], []).append(k)
                 pos = nx.spring_layout(problem_graph)
                 # pos = nx.circular_layout(self._g)
                 color = 0
                 for bit, node_list in color_dic.items():
-                    nx.draw_networkx(problem_graph, pos=pos, nodelist=node_list, node_size=500, node_color=color_list[color], font_size=15, width=2)
+                    nx.draw_networkx(problem_graph, pos=pos, nodelist=node_list, node_size=500,
+                                     node_color=color_list[color], font_size=15, width=2)
                     color = color + 1
-                    print('Coloring ' + str(color)+ ':', sorted(node_list))
+                    print('Coloring ' + str(color) + ':', sorted(node_list))
                 nx.draw_networkx_edges(problem_graph, pos, width=2, edge_color='g', arrows=False)
                 # plt.axis('off')
                 plt.tight_layout()
                 plt.show()
                 print('Cost (QUBO):', counts_energy[s][1])
         else:
             print('The current version does not support visualization of this type of problem!')
```

### Comparing `Qcover-2.3.0/Qcover/compiler/hardware_library.py` & `Qcover-2.4.0/Qcover/compiler/hardware_library.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,25 +2,22 @@
 import networkx as nx
 from queue import PriorityQueue
 import matplotlib.pyplot as plt
 import copy
 import math
 from collections import defaultdict
 import os
-import re
 from quafu import Task
-import numpy as np
 
 
 class BuildLibrary:
     def __init__(self, backend='ScQ-P10', fidelity_threshold=95):
         self.backend = backend
         self.fidelity_threshold = fidelity_threshold
         task = Task()
-        # task.load_account()
         task.config(backend=self.backend)
         self.backend_info = task.get_backend_info()
         self.calibration_time = self.backend_info['full_info']["calibration_time"]
 
     def get_structure(self):
         """
         Args:
@@ -29,35 +26,17 @@
             int_to_qubit(dict): {0: Q01, 1: Q02, ...}
             qubit_to_int(dict): {Q01: 0, Q02: 0, ...}
             directed_weighted_edges(list):[[qubit1,qubit2,fidelity],...]
             connected_substructure_list(list): [networkx.Graph,...]
         """
 
         json_topo_struct = self.backend_info['full_info']["topological_structure"]
+        int_to_qubit = self.backend_info['mapping']
+        qubit_to_int = {v: k for k, v in int_to_qubit.items()}
 
-        # # not ordered
-        # qubits_list = []
-        # for gate in json_topo_struct.keys():
-        #     qubit = gate.split('_')
-        #     if qubit[0] not in qubits_list:
-        #         qubits_list.append(qubit[0])
-        #     if qubit[1] not in qubits_list:
-        #         qubits_list.append(qubit[1])
-
-        # # ordered
-        qubits_list = []
-        for gate in json_topo_struct.keys():
-            qubit = gate.split('_')
-            qubits_list.append(qubit[0])
-            qubits_list.append(qubit[1])
-        qubits_list = list(set(qubits_list))
-        qubits_list = sorted(qubits_list, key=lambda x: int(re.findall(r"\d+", x)[0]))
-
-        int_to_qubit = {k: v for k, v in enumerate(qubits_list)}
-        qubit_to_int = {v: k for k, v in enumerate(qubits_list)}
         directed_weighted_edges = []
         weighted_edges = []
         edges_dict = {}
         for gate, name_fidelity in json_topo_struct.items():
             gate_qubit = gate.split('_')
             qubit1 = qubit_to_int[gate_qubit[0]]
             qubit2 = qubit_to_int[gate_qubit[1]]
@@ -152,23 +131,58 @@
                 # substructure_dict[qubits].append(sub_graph[j][1])
                 qlist.append(sub_graph[j][1])
             substructure_dict[qubits] = qlist
 
         sorted_weighted_edges = sorted(directed_weighted_edges, key=lambda x: x[2], reverse=True)
         save_substructure = {'calibration_time': self.calibration_time, 'structure': sorted_weighted_edges, 'substructure_dict': substructure_dict,
                              'int_to_qubit': int_to_qubit, 'qubit_to_int': qubit_to_int}
-        # if os.path.exists('LibSubstructure_' + self.backend + '.txt'):
-        #     os.remove('LibSubstructure_' + self.backend + '.txt')
-        with open('LibSubstructure_' + self.backend + '.txt', 'w') as file:
-            # file.write(json.dumps(save_substructure))
+
+        dir_path = os.path.dirname(os.path.abspath(__file__))
+        folder_path = os.path.join(dir_path, "backend_library")
+        if not os.path.exists(folder_path):
+            os.mkdir(folder_path)
+        file_name = 'LibSubstructure_' + self.backend + '.txt'
+        file_path = os.path.join(folder_path, file_name)
+        if os.path.exists(file_path):
+            os.remove(file_path)
+        with open(file_path, 'w') as file:
             file.write(str(save_substructure))
+
+        return save_substructure
+
+    def build_chains_from_all(self, substructure_data):
+        # Find chains from the all sub-chains of 2D chip.
+        chain_dict = self.find_subchains(substructure_data)
+        chain_dict = dict(sorted(chain_dict.items(), key=lambda x: x[0]))
+
+        structure_dict = {}
+        for edge in substructure_data['structure']:
+            structure_dict[(edge[0], edge[1])] = edge[2]
+
+        save_substructure = self.build_chains(chain_dict, structure_dict)
         return save_substructure
 
-    def chain_library_2D(self, substructure_data):
-        # find one-dimensional chain
+    def build_chains_from_longest(self, substructure_data):
+        # Find chains from the longest chain of 2D chip.
+        chain_dict = self.find_subchains(substructure_data)
+        max_chain = max(chain_dict.keys())
+        if len(chain_dict[max_chain]) > 1:
+            longest_chain_dict = {max_chain: [chain_dict[max_chain][0], chain_dict[max_chain][-1]]}
+        else:
+            longest_chain_dict = {max_chain: chain_dict[max_chain][0:1]}
+
+        structure_dict = {}
+        for edge in substructure_data['structure']:
+            structure_dict[(edge[0], edge[1])] = edge[2]
+
+        save_substructure = self.build_chains(longest_chain_dict, structure_dict)
+        return save_substructure
+
+    def find_subchains(self, substructure_data):
+        # Find all sub-chains in a two-dimensional chip
         G = nx.DiGraph()
         G.add_weighted_edges_from(substructure_data['substructure_dict'][len(substructure_data['qubit_to_int'])][0])
         node_degree = dict(G.degree)
         sort_degree = sorted(node_degree.items(), key=lambda kv: kv[1], reverse=False)
         one_link_nodes = [node for node, degree in sort_degree if degree == 2]
         all_oneD_chain = []
         for i in range(len(one_link_nodes)):
@@ -197,51 +211,55 @@
 
         sorted_chain = []
         for chain in all_oneD_chain:
             if sorted(chain) not in sorted_chain:
                 sorted_chain.append(sorted(chain))
                 chain_dict[len(chain)].append(chain)
 
-        chain_dict = dict(sorted(chain_dict.items(), key=lambda x: x[0]))
-        # longset_chain = chain_dict[max(chain_dict.keys())][0]
-
-        structure_dict = {}
-        for edge in substructure_data['structure']:
-            structure_dict[(edge[0], edge[1])] = edge[2]
+        return chain_dict
 
+    def build_chains(self, chain_dict, structure_dict):
         connected_chain_list = []
         for node_number, chain_nodes_list in chain_dict.items():
             for chain_nodes in chain_nodes_list:
                 chain_graph = nx.DiGraph()
                 directed_weighted_edges = []
-                for i in range(len(chain_nodes)-1):
-                    directed_weighted_edges.append([chain_nodes[i], chain_nodes[i+1],
-                                                    structure_dict[(chain_nodes[i], chain_nodes[i+1])]])
-                    directed_weighted_edges.append([chain_nodes[i+1], chain_nodes[i],
-                                                    structure_dict[(chain_nodes[i+1], chain_nodes[i])]])
+                for i in range(len(chain_nodes) - 1):
+                    directed_weighted_edges.append([chain_nodes[i], chain_nodes[i + 1],
+                                                    structure_dict[(chain_nodes[i], chain_nodes[i + 1])]])
+                    directed_weighted_edges.append([chain_nodes[i + 1], chain_nodes[i],
+                                                    structure_dict[(chain_nodes[i + 1], chain_nodes[i])]])
                 chain_graph.add_weighted_edges_from(directed_weighted_edges)
                 connected_chain_list.append([directed_weighted_edges, chain_graph])
 
         subchain_dict = defaultdict(list)
         for chain in connected_chain_list:
-            for qubits in range(2, len(chain[1].nodes())+1):
+            for qubits in range(2, len(chain[1].nodes()) + 1):
                 sub_graph = self.substructure(chain[0], [chain[1]], qubits)
                 for j in range(len(sub_graph)):
                     log_weight_product = 0
                     for edge in sub_graph[j][1]:
                         log_weight_product = log_weight_product + math.log(edge[2])
                     if [log_weight_product, sub_graph[j][1]] not in subchain_dict[qubits]:
                         subchain_dict[qubits].append([log_weight_product, sub_graph[j][1]])
 
         sorted_subchain_dict = {}
         for k, chain_list in subchain_dict.items():
             chain_list = sorted(chain_list, key=lambda x: x[0], reverse=True)
             chain_list = [chain[1] for chain in chain_list]
             sorted_subchain_dict[k] = chain_list
 
-        save_substructure = {'calibration_time': self.calibration_time, 'subchain_dict': sorted_subchain_dict}
-        if os.path.exists('LibSubchain_' + self.backend + '.txt'):
-            os.remove('LibSubchain_' + self.backend + '.txt')
-        with open('LibSubchain_' + self.backend + '.txt', 'w') as file:
-            file.write(str(save_substructure))
-        return save_substructure
+        save_subchains = {'calibration_time': self.calibration_time, 'subchain_dict': sorted_subchain_dict}
+
+        dir_path = os.path.dirname(os.path.abspath(__file__))
+        folder_path = os.path.join(dir_path, "backend_library")
+        if not os.path.exists(folder_path):
+            os.mkdir(folder_path)
+        file_name = 'LibSubchain_' + self.backend + '.txt'
+        file_path = os.path.join(folder_path, file_name)
+        if os.path.exists(file_path):
+            os.remove(file_path)
+        with open(file_path, 'w') as file:
+            file.write(str(save_subchains))
+
+        return save_subchains
```

### Comparing `Qcover-2.3.0/Qcover/core.py` & `Qcover-2.4.0/Qcover/core.py`

 * *Files identical despite different names*

### Comparing `Qcover-2.3.0/Qcover/exceptions.py` & `Qcover-2.4.0/Qcover/exceptions.py`

 * *Files identical despite different names*

### Comparing `Qcover-2.3.0/Qcover/optimizers/COBYLA.py` & `Qcover-2.4.0/Qcover/optimizers/COBYLA.py`

 * *Files identical despite different names*

### Comparing `Qcover-2.3.0/Qcover/optimizers/Fourier.py` & `Qcover-2.4.0/Qcover/optimizers/Fourier.py`

 * *Files identical despite different names*

### Comparing `Qcover-2.3.0/Qcover/optimizers/Gradient_Descent.py` & `Qcover-2.4.0/Qcover/optimizers/Gradient_Descent.py`

 * *Files identical despite different names*

### Comparing `Qcover-2.3.0/Qcover/optimizers/Interp.py` & `Qcover-2.4.0/Qcover/optimizers/Interp.py`

 * *Files identical despite different names*

### Comparing `Qcover-2.3.0/Qcover/optimizers/L_BFGS_B.py` & `Qcover-2.4.0/Qcover/optimizers/L_BFGS_B.py`

 * *Files identical despite different names*

### Comparing `Qcover-2.3.0/Qcover/optimizers/SHGO.py` & `Qcover-2.4.0/Qcover/optimizers/SHGO.py`

 * *Files identical despite different names*

### Comparing `Qcover-2.3.0/Qcover/optimizers/SLSQP.py` & `Qcover-2.4.0/Qcover/optimizers/SLSQP.py`

 * *Files identical despite different names*

### Comparing `Qcover-2.3.0/Qcover/optimizers/SPSA.py` & `Qcover-2.4.0/Qcover/optimizers/SPSA.py`

 * *Files identical despite different names*

### Comparing `Qcover-2.3.0/Qcover/optimizers/Simulated_Annealing.py` & `Qcover-2.4.0/Qcover/optimizers/Simulated_Annealing.py`

 * *Files identical despite different names*

### Comparing `Qcover-2.3.0/Qcover/research/Ent_TMI.py` & `Qcover-2.4.0/Qcover/research/Ent_TMI.py`

 * *Files identical despite different names*

### Comparing `Qcover-2.3.0/Qcover/research/GHZ_Generate.py` & `Qcover-2.4.0/Qcover/research/GHZ_Generate.py`

 * *Files identical despite different names*

### Comparing `Qcover-2.3.0/Qcover/research/QAOA_Generate.py` & `Qcover-2.4.0/Qcover/research/QAOA_Generate.py`

 * *Files identical despite different names*

### Comparing `Qcover-2.3.0/Qcover/research/scrambling-OTOC.py` & `Qcover-2.4.0/Qcover/research/scrambling-OTOC.py`

 * *Files identical despite different names*

### Comparing `Qcover-2.3.0/Qcover/simulator/qton.py` & `Qcover-2.4.0/Qcover/simulator/qton.py`

 * *Files identical despite different names*

### Comparing `Qcover-2.3.0/Qcover/utils.py` & `Qcover-2.4.0/Qcover/utils.py`

 * *Files identical despite different names*

### Comparing `Qcover-2.3.0/Qcover.egg-info/PKG-INFO` & `Qcover-2.4.0/Qcover.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Qcover
-Version: 2.3.0
+Version: 2.4.0
 Summary: Quantum computing solver
 Home-page: https://github.com/BAQIS-Quantum/Qcover
 Author: ntyz&finleyzhuang
 Author-email: puyn@baqis.ac.cn
 License: Apache-2.0 License
 Project-URL: Bug Reports, https://github.com/BAQIS-Quantum/Qcover/issues
 Project-URL: Source, https://github.com/BAQIS-Quantum/Qcover
```

### Comparing `Qcover-2.3.0/Qcover.egg-info/SOURCES.txt` & `Qcover-2.4.0/Qcover.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 Qcover/backends/__init__.py
 Qcover/backends/backend.py
 Qcover/backends/circuitbycirq.py
 Qcover/backends/circuitbyprojectq.py
 Qcover/backends/circuitbyqiskit.py
 Qcover/backends/circuitbyqiskit_statistic.py
 Qcover/backends/circuitbyqton.py
+Qcover/backends/circuitbyquafu.py
 Qcover/backends/circuitbyqulacs.py
 Qcover/backends/circuitbytensor.py
 Qcover/compiler/__init__.py
 Qcover/compiler/compilerforQAOA.py
 Qcover/compiler/hardware_library.py
 Qcover/optimizers/COBYLA.py
 Qcover/optimizers/Fourier.py
```

### Comparing `Qcover-2.3.0/README.md` & `Qcover-2.4.0/README.md`

 * *Files identical despite different names*

