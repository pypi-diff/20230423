# Comparing `tmp/vise-0.7.0.tar.gz` & `tmp/vise-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vise-0.7.0.tar", last modified: Wed Jan  4 06:29:09 2023, max compression
+gzip compressed data, was "dist/vise-0.7.1.tar", last modified: Sun Apr 23 00:27:13 2023, max compression
```

## Comparing `vise-0.7.0.tar` & `vise-0.7.1.tar`

### file list

```diff
@@ -1,180 +1,179 @@
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-01-04 06:29:09.002639 vise-0.7.0/
--rw-r--r--   0 kumagai    (501) staff       (20)      179 2020-12-23 04:48:27.000000 vise-0.7.0/MANIFEST.in
--rw-r--r--   0 kumagai    (501) staff       (20)     4389 2023-01-04 06:29:09.002167 vise-0.7.0/PKG-INFO
--rw-r--r--   0 kumagai    (501) staff       (20)     3247 2022-07-28 01:56:51.000000 vise-0.7.0/README.md
--rw-r--r--   0 kumagai    (501) staff       (20)       38 2023-01-04 06:29:09.002810 vise-0.7.0/setup.cfg
--rw-r--r--   0 kumagai    (501) staff       (20)     1460 2022-06-27 23:50:06.000000 vise-0.7.0/setup.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-01-04 06:29:08.750855 vise-0.7.0/vise/
--rw-r--r--   0 kumagai    (501) staff       (20)       37 2020-05-15 22:51:22.000000 vise-0.7.0/vise/__init__.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-01-04 06:29:08.766472 vise-0.7.0/vise/analyzer/
--rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-15 22:51:22.000000 vise-0.7.0/vise/analyzer/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1633 2021-03-06 05:00:49.000000 vise-0.7.0/vise/analyzer/atom_grouping_type.py
--rwxr-xr-x   0 kumagai    (501) staff       (20)     7574 2022-10-21 08:31:12.000000 vise-0.7.0/vise/analyzer/band_edge_properties.py
--rw-r--r--   0 kumagai    (501) staff       (20)     7667 2022-12-06 07:44:43.000000 vise-0.7.0/vise/analyzer/dielectric_function.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-01-04 06:29:08.771067 vise-0.7.0/vise/analyzer/dielectric_function_data/
--rw-r--r--   0 kumagai    (501) staff       (20)     3188 2020-11-07 08:48:51.000000 vise-0.7.0/vise/analyzer/dielectric_function_data/GaAs.csv
--rw-r--r--   0 kumagai    (501) staff       (20)     3474 2020-11-07 08:58:34.000000 vise-0.7.0/vise/analyzer/dielectric_function_data/Si.csv
--rw-r--r--   0 kumagai    (501) staff       (20)     1422 2020-11-12 08:22:54.000000 vise-0.7.0/vise/analyzer/dielectric_function_data/exp_dielectric_func.py
--rw-r--r--   0 kumagai    (501) staff       (20)     9493 2022-12-06 07:09:21.000000 vise-0.7.0/vise/analyzer/dos_data.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2222 2021-05-25 08:13:08.000000 vise-0.7.0/vise/analyzer/effective_mass.py
--rw-r--r--   0 kumagai    (501) staff       (20)    12797 2022-09-10 03:08:43.000000 vise-0.7.0/vise/analyzer/plot_band.py
--rw-r--r--   0 kumagai    (501) staff       (20)    12057 2022-09-12 04:32:47.000000 vise-0.7.0/vise/analyzer/plot_band_dos.py
--rw-r--r--   0 kumagai    (501) staff       (20)     6509 2022-10-12 07:02:26.000000 vise-0.7.0/vise/analyzer/plot_brillouin_zone.py
--rw-r--r--   0 kumagai    (501) staff       (20)     7891 2022-12-06 07:45:00.000000 vise-0.7.0/vise/analyzer/plot_diele_func_data.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4553 2022-12-06 07:30:30.000000 vise-0.7.0/vise/analyzer/plot_dos.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-01-04 06:29:08.780465 vise-0.7.0/vise/analyzer/vasp/
--rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-15 22:51:22.000000 vise-0.7.0/vise/analyzer/vasp/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2231 2022-08-19 06:07:54.000000 vise-0.7.0/vise/analyzer/vasp/band_edge_properties.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2968 2022-12-06 07:08:20.000000 vise-0.7.0/vise/analyzer/vasp/dos_data.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1474 2021-08-06 10:07:19.000000 vise-0.7.0/vise/analyzer/vasp/handle_volumetric_data.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1866 2022-09-23 02:12:27.000000 vise-0.7.0/vise/analyzer/vasp/make_diele_func.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1242 2021-06-24 07:47:02.000000 vise-0.7.0/vise/analyzer/vasp/make_effective_mass.py
--rw-r--r--   0 kumagai    (501) staff       (20)     3658 2022-10-04 04:01:43.000000 vise-0.7.0/vise/analyzer/vasp/make_irreps.py
--rw-r--r--   0 kumagai    (501) staff       (20)     6229 2022-10-06 05:30:09.000000 vise-0.7.0/vise/analyzer/vasp/plot_band.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-01-04 06:29:08.785943 vise-0.7.0/vise/analyzer/vesta/
--rw-r--r--   0 kumagai    (501) staff       (20)       61 2021-03-12 02:41:40.000000 vise-0.7.0/vise/analyzer/vesta/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4183 2021-03-02 07:24:45.000000 vise-0.7.0/vise/analyzer/vesta/element_colors.py
--rw-r--r--   0 kumagai    (501) staff       (20)    12453 2021-07-05 05:51:09.000000 vise-0.7.0/vise/analyzer/vesta/vesta_file.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-01-04 06:29:08.838265 vise-0.7.0/vise/atom_energies/
--rw-r--r--   0 kumagai    (501) staff       (20)       95 2020-05-18 00:09:10.000000 vise-0.7.0/vise/atom_energies/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)      290 2020-11-30 06:52:18.000000 vise-0.7.0/vise/atom_energies/atom_energy.py
--rw-r--r--   0 kumagai    (501) staff       (20)      515 2020-08-11 09:15:50.000000 vise-0.7.0/vise/atom_energies/atom_magnetization_hund.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)     1217 2021-08-04 07:35:01.000000 vise-0.7.0/vise/atom_energies/get_energy.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2267 2022-07-05 01:18:05.000000 vise-0.7.0/vise/atom_energies/make_atom_vasp_set.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1135 2020-11-30 02:31:47.000000 vise-0.7.0/vise/atom_energies/mp_atom_energy.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)      709 2020-11-30 02:31:47.000000 vise-0.7.0/vise/atom_energies/mp_atom_mag.yaml
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-01-04 06:29:08.843343 vise-0.7.0/vise/cli/
--rw-r--r--   0 kumagai    (501) staff       (20)       72 2020-05-15 22:51:22.000000 vise-0.7.0/vise/cli/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)    13924 2022-12-26 01:46:16.000000 vise-0.7.0/vise/cli/main.py
--rw-r--r--   0 kumagai    (501) staff       (20)    14143 2023-01-04 06:28:21.000000 vise-0.7.0/vise/cli/main_functions.py
--rw-r--r--   0 kumagai    (501) staff       (20)     3506 2020-10-03 03:00:38.000000 vise-0.7.0/vise/cli/main_tools.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4944 2021-08-06 10:08:41.000000 vise-0.7.0/vise/cli/main_util.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2216 2021-05-05 00:16:26.000000 vise-0.7.0/vise/cli/main_util_functions.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4294 2022-11-14 04:27:07.000000 vise-0.7.0/vise/defaults.py
--rw-r--r--   0 kumagai    (501) staff       (20)      134 2020-05-15 22:51:22.000000 vise-0.7.0/vise/error.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-01-04 06:29:08.856258 vise-0.7.0/vise/input_set/
--rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-15 22:51:22.000000 vise-0.7.0/vise/input_set/__init__.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-01-04 06:29:08.864526 vise-0.7.0/vise/input_set/datasets/
--rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-15 22:51:22.000000 vise-0.7.0/vise/input_set/datasets/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2483 2022-11-14 04:02:39.000000 vise-0.7.0/vise/input_set/datasets/dataset_util.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1642 2022-12-19 07:34:18.000000 vise-0.7.0/vise/input_set/datasets/incar_flags.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)      685 2020-05-15 22:51:22.000000 vise-0.7.0/vise/input_set/datasets/kpar_set.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)    14502 2020-05-15 22:51:22.000000 vise-0.7.0/vise/input_set/datasets/kpt_centering.py
--rw-r--r--   0 kumagai    (501) staff       (20)      294 2020-05-15 22:51:22.000000 vise-0.7.0/vise/input_set/datasets/magmom.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)     1516 2020-05-15 22:51:22.000000 vise-0.7.0/vise/input_set/datasets/potcar_set.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4024 2020-12-23 01:37:43.000000 vise-0.7.0/vise/input_set/datasets/potcar_set.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)      623 2021-05-06 06:02:40.000000 vise-0.7.0/vise/input_set/datasets/u_parameter_set.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)      574 2020-05-15 22:51:22.000000 vise-0.7.0/vise/input_set/datasets/unoccupied_bands.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)     1141 2022-07-23 04:43:00.000000 vise-0.7.0/vise/input_set/fft_grids.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4155 2022-12-19 07:31:57.000000 vise-0.7.0/vise/input_set/incar.py
--rw-r--r--   0 kumagai    (501) staff       (20)    12667 2022-11-30 06:56:02.000000 vise-0.7.0/vise/input_set/incar_settings_generator.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4026 2022-11-14 04:20:42.000000 vise-0.7.0/vise/input_set/input_options.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1360 2020-05-15 22:51:22.000000 vise-0.7.0/vise/input_set/kpoints.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1279 2020-05-15 22:51:22.000000 vise-0.7.0/vise/input_set/kpoints_mode.py
--rw-r--r--   0 kumagai    (501) staff       (20)      914 2020-05-15 22:51:22.000000 vise-0.7.0/vise/input_set/potcar_generator.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4022 2021-08-04 07:35:03.000000 vise-0.7.0/vise/input_set/prior_info.py
--rw-r--r--   0 kumagai    (501) staff       (20)     7936 2022-11-14 04:29:55.000000 vise-0.7.0/vise/input_set/structure_kpoints_generator.py
--rw-r--r--   0 kumagai    (501) staff       (20)     3912 2022-10-06 08:28:55.000000 vise-0.7.0/vise/input_set/task.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4131 2022-11-04 09:21:10.000000 vise-0.7.0/vise/input_set/vasp_input_files.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1322 2022-10-21 08:42:57.000000 vise-0.7.0/vise/input_set/vise_log.py
--rw-r--r--   0 kumagai    (501) staff       (20)      956 2020-06-03 03:20:45.000000 vise-0.7.0/vise/input_set/xc.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-01-04 06:29:08.867820 vise-0.7.0/vise/tests/
--rw-r--r--   0 kumagai    (501) staff       (20)       96 2020-05-15 22:51:22.000000 vise-0.7.0/vise/tests/__init__.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-01-04 06:29:08.875827 vise-0.7.0/vise/tests/analyzer/
--rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-15 22:51:22.000000 vise-0.7.0/vise/tests/analyzer/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1503 2020-11-30 08:10:26.000000 vise-0.7.0/vise/tests/analyzer/test_atom_grouping_type.py
--rw-r--r--   0 kumagai    (501) staff       (20)     8181 2022-09-30 06:32:39.000000 vise-0.7.0/vise/tests/analyzer/test_band_edge_properties.py
--rw-r--r--   0 kumagai    (501) staff       (20)     3441 2022-11-03 04:27:22.000000 vise-0.7.0/vise/tests/analyzer/test_dielectric_function.py
--rw-r--r--   0 kumagai    (501) staff       (20)    10283 2022-11-14 23:40:17.000000 vise-0.7.0/vise/tests/analyzer/test_dos_data.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1951 2021-05-25 08:12:05.000000 vise-0.7.0/vise/tests/analyzer/test_effective_mass.py
--rw-r--r--   0 kumagai    (501) staff       (20)    12879 2022-09-13 00:24:09.000000 vise-0.7.0/vise/tests/analyzer/test_plot_band.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1576 2022-09-12 00:48:30.000000 vise-0.7.0/vise/tests/analyzer/test_plot_band_dos.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2099 2022-10-21 06:44:45.000000 vise-0.7.0/vise/tests/analyzer/test_plot_brillouin_zone.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2639 2022-12-06 07:46:00.000000 vise-0.7.0/vise/tests/analyzer/test_plot_diele_func_data.py
--rw-r--r--   0 kumagai    (501) staff       (20)     7869 2022-12-06 07:02:33.000000 vise-0.7.0/vise/tests/analyzer/test_plot_dos.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-01-04 06:29:08.904791 vise-0.7.0/vise/tests/analyzer/vasp/
--rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-15 22:51:22.000000 vise-0.7.0/vise/tests/analyzer/vasp/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2282 2021-03-06 04:52:09.000000 vise-0.7.0/vise/tests/analyzer/vasp/test_band_edge_properties.py
--rw-r--r--   0 kumagai    (501) staff       (20)     3504 2021-03-06 04:52:35.000000 vise-0.7.0/vise/tests/analyzer/vasp/test_dos_data.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1607 2022-10-21 07:15:26.000000 vise-0.7.0/vise/tests/analyzer/vasp/test_handle_volumetric_data.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1900 2022-09-23 00:52:48.000000 vise-0.7.0/vise/tests/analyzer/vasp/test_make_diele_func.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2517 2021-06-24 07:56:18.000000 vise-0.7.0/vise/tests/analyzer/vasp/test_make_effective_mass.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2015 2022-09-13 01:26:49.000000 vise-0.7.0/vise/tests/analyzer/vasp/test_make_irreps.py
--rw-r--r--   0 kumagai    (501) staff       (20)     5783 2022-10-06 05:29:21.000000 vise-0.7.0/vise/tests/analyzer/vasp/test_plot_band.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-01-04 06:29:08.909564 vise-0.7.0/vise/tests/cli/
--rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-15 22:51:22.000000 vise-0.7.0/vise/tests/cli/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)     8707 2022-12-06 07:49:28.000000 vise-0.7.0/vise/tests/cli/test_main.py
--rw-r--r--   0 kumagai    (501) staff       (20)    10973 2023-01-04 06:19:42.000000 vise-0.7.0/vise/tests/cli/test_main_functions.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1683 2022-07-29 02:57:51.000000 vise-0.7.0/vise/tests/cli/test_main_tools.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2249 2021-04-30 01:10:17.000000 vise-0.7.0/vise/tests/cli/test_main_util.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2463 2021-05-04 23:31:17.000000 vise-0.7.0/vise/tests/cli/test_main_util_functions.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1785 2022-09-10 03:00:55.000000 vise-0.7.0/vise/tests/conftest.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-01-04 06:29:08.911660 vise-0.7.0/vise/tests/helpers/
--rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-14 10:39:18.000000 vise-0.7.0/vise/tests/helpers/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)     5735 2022-11-16 01:51:02.000000 vise-0.7.0/vise/tests/helpers/assertion.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4419 2022-09-30 04:31:05.000000 vise-0.7.0/vise/tests/helpers/test_assersion.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-01-04 06:29:08.941960 vise-0.7.0/vise/tests/input_set/
--rw-r--r--   0 kumagai    (501) staff       (20)       96 2020-05-15 22:51:22.000000 vise-0.7.0/vise/tests/input_set/__init__.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-01-04 06:29:08.964934 vise-0.7.0/vise/tests/input_set/datasets/
--rw-r--r--   0 kumagai    (501) staff       (20)       96 2020-05-15 22:51:22.000000 vise-0.7.0/vise/tests/input_set/datasets/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1519 2022-11-14 04:00:11.000000 vise-0.7.0/vise/tests/input_set/datasets/test_dataset_util.py
--rw-r--r--   0 kumagai    (501) staff       (20)      780 2020-05-15 22:51:22.000000 vise-0.7.0/vise/tests/input_set/datasets/test_potcar_set.py
--rw-r--r--   0 kumagai    (501) staff       (20)      232 2022-01-27 04:37:06.000000 vise-0.7.0/vise/tests/input_set/test_fft_grids.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1569 2022-12-19 07:32:46.000000 vise-0.7.0/vise/tests/input_set/test_incar.py
--rw-r--r--   0 kumagai    (501) staff       (20)     8997 2022-11-14 04:40:23.000000 vise-0.7.0/vise/tests/input_set/test_incar_settings_generator.py
--rw-r--r--   0 kumagai    (501) staff       (20)     3796 2022-07-26 07:16:22.000000 vise-0.7.0/vise/tests/input_set/test_input_options.py
--rw-r--r--   0 kumagai    (501) staff       (20)      533 2020-05-15 22:51:22.000000 vise-0.7.0/vise/tests/input_set/test_kpoints_mode.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1555 2021-03-05 09:50:13.000000 vise-0.7.0/vise/tests/input_set/test_potcar_generator.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2565 2022-07-01 00:59:32.000000 vise-0.7.0/vise/tests/input_set/test_prior_info.py
--rw-r--r--   0 kumagai    (501) staff       (20)     9329 2022-07-26 03:58:12.000000 vise-0.7.0/vise/tests/input_set/test_structure_kpoints_generator.py
--rw-r--r--   0 kumagai    (501) staff       (20)     3410 2022-10-06 08:28:37.000000 vise-0.7.0/vise/tests/input_set/test_task.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1573 2022-11-14 04:18:29.000000 vise-0.7.0/vise/tests/input_set/test_vasp_input_files.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1211 2022-10-21 08:43:44.000000 vise-0.7.0/vise/tests/input_set/test_vise_log.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1162 2021-03-02 02:37:28.000000 vise-0.7.0/vise/tests/input_set/test_xc.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4762 2022-11-06 00:50:42.000000 vise-0.7.0/vise/tests/test_defaults.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1784 2022-10-21 08:06:31.000000 vise-0.7.0/vise/tests/test_user_settings.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-01-04 06:29:08.973013 vise-0.7.0/vise/tests/util/
--rw-r--r--   0 kumagai    (501) staff       (20)       96 2020-05-15 22:51:22.000000 vise-0.7.0/vise/tests/util/__init__.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-01-04 06:29:08.974510 vise-0.7.0/vise/tests/util/phonopy/
--rw-r--r--   0 kumagai    (501) staff       (20)       96 2020-05-15 22:51:22.000000 vise-0.7.0/vise/tests/util/phonopy/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)     3100 2021-08-06 10:08:41.000000 vise-0.7.0/vise/tests/util/phonopy/test_phonopy_input.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1499 2020-05-15 22:51:22.000000 vise-0.7.0/vise/tests/util/test_bravais_lattice.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2441 2021-03-05 09:50:13.000000 vise-0.7.0/vise/tests/util/test_centering.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4437 2020-05-15 22:51:22.000000 vise-0.7.0/vise/tests/util/test_file_transfer.py
--rw-r--r--   0 kumagai    (501) staff       (20)      217 2020-08-02 02:24:25.000000 vise-0.7.0/vise/tests/util/test_logger.py
--rw-r--r--   0 kumagai    (501) staff       (20)      511 2020-05-15 22:51:22.000000 vise-0.7.0/vise/tests/util/test_matplotlib.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1500 2022-09-28 23:59:57.000000 vise-0.7.0/vise/tests/util/test_mix_in.py
--rw-r--r--   0 kumagai    (501) staff       (20)      232 2021-04-18 02:48:05.000000 vise-0.7.0/vise/tests/util/test_string.py
--rw-r--r--   0 kumagai    (501) staff       (20)     9778 2021-07-31 08:14:24.000000 vise-0.7.0/vise/tests/util/test_structure_symmetrizer.py
--rw-r--r--   0 kumagai    (501) staff       (20)      471 2021-08-01 00:43:34.000000 vise-0.7.0/vise/tests/util/test_valence_orbitals_from_potcar.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2143 2022-11-15 04:24:17.000000 vise-0.7.0/vise/user_settings.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-01-04 06:29:08.999401 vise-0.7.0/vise/util/
--rw-r--r--   0 kumagai    (501) staff       (20)     3450 2021-09-15 23:40:59.000000 vise-0.7.0/vise/util/Hermann-Mauguin.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-15 22:51:22.000000 vise-0.7.0/vise/util/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)     6228 2020-05-15 22:51:22.000000 vise-0.7.0/vise/util/bravais_lattice.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1786 2020-05-14 03:15:55.000000 vise-0.7.0/vise/util/centering.py
--rw-r--r--   0 kumagai    (501) staff       (20)      304 2020-11-12 05:19:29.000000 vise-0.7.0/vise/util/dash_helper.py
--rw-r--r--   0 kumagai    (501) staff       (20)      788 2021-05-30 03:06:06.000000 vise-0.7.0/vise/util/enum.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2746 2020-11-30 22:31:41.000000 vise-0.7.0/vise/util/file_transfer.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1234 2021-05-01 05:11:26.000000 vise-0.7.0/vise/util/logger.py
--rw-r--r--   0 kumagai    (501) staff       (20)      802 2020-05-15 22:51:22.000000 vise-0.7.0/vise/util/matplotlib.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2752 2022-09-30 04:31:19.000000 vise-0.7.0/vise/util/mix_in.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-01-04 06:29:09.001412 vise-0.7.0/vise/util/phonopy/
--rw-r--r--   0 kumagai    (501) staff       (20)       96 2020-05-15 22:51:22.000000 vise-0.7.0/vise/util/phonopy/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4058 2022-09-06 01:13:47.000000 vise-0.7.0/vise/util/phonopy/phonopy_input.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2043 2021-08-11 05:37:35.000000 vise-0.7.0/vise/util/plotly_util.py
--rw-r--r--   0 kumagai    (501) staff       (20)      986 2022-07-29 03:01:33.000000 vise-0.7.0/vise/util/str_related_tools.py
--rw-r--r--   0 kumagai    (501) staff       (20)      786 2021-04-20 00:50:10.000000 vise-0.7.0/vise/util/string.py
--rw-r--r--   0 kumagai    (501) staff       (20)      486 2021-03-05 09:50:13.000000 vise-0.7.0/vise/util/structure_handler.py
--rw-r--r--   0 kumagai    (501) staff       (20)    13330 2022-11-14 04:29:55.000000 vise-0.7.0/vise/util/structure_symmetrizer.py
--rw-r--r--   0 kumagai    (501) staff       (20)      229 2021-05-02 02:13:00.000000 vise-0.7.0/vise/util/typing.py
--rw-r--r--   0 kumagai    (501) staff       (20)      226 2021-07-05 05:51:09.000000 vise-0.7.0/vise/util/unit_conversion.py
--rw-r--r--   0 kumagai    (501) staff       (20)      419 2021-07-05 06:55:26.000000 vise-0.7.0/vise/util/valence_orbitals_from_potcar.py
--rw-r--r--   0 kumagai    (501) staff       (20)      117 2023-01-04 06:28:42.000000 vise-0.7.0/vise/version.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-01-04 06:29:08.755013 vise-0.7.0/vise.egg-info/
--rw-r--r--   0 kumagai    (501) staff       (20)     4389 2023-01-04 06:29:08.000000 vise-0.7.0/vise.egg-info/PKG-INFO
--rw-r--r--   0 kumagai    (501) staff       (20)     5354 2023-01-04 06:29:08.000000 vise-0.7.0/vise.egg-info/SOURCES.txt
--rw-r--r--   0 kumagai    (501) staff       (20)        1 2023-01-04 06:29:08.000000 vise-0.7.0/vise.egg-info/dependency_links.txt
--rw-r--r--   0 kumagai    (501) staff       (20)       81 2023-01-04 06:29:08.000000 vise-0.7.0/vise.egg-info/entry_points.txt
--rw-r--r--   0 kumagai    (501) staff       (20)      163 2023-01-04 06:29:08.000000 vise-0.7.0/vise.egg-info/requires.txt
--rw-r--r--   0 kumagai    (501) staff       (20)        5 2023-01-04 06:29:08.000000 vise-0.7.0/vise.egg-info/top_level.txt
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-04-23 00:27:13.330232 vise-0.7.1/
+-rw-r--r--   0 kumagai    (501) staff       (20)      179 2020-12-23 04:48:27.000000 vise-0.7.1/MANIFEST.in
+-rw-r--r--   0 kumagai    (501) staff       (20)     4389 2023-04-23 00:27:13.329938 vise-0.7.1/PKG-INFO
+-rw-r--r--   0 kumagai    (501) staff       (20)     3247 2022-07-28 01:56:51.000000 vise-0.7.1/README.md
+-rw-r--r--   0 kumagai    (501) staff       (20)       38 2023-04-23 00:27:13.330326 vise-0.7.1/setup.cfg
+-rw-r--r--   0 kumagai    (501) staff       (20)     1460 2022-06-27 23:50:06.000000 vise-0.7.1/setup.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-04-23 00:27:13.130392 vise-0.7.1/vise/
+-rw-r--r--   0 kumagai    (501) staff       (20)       37 2020-05-15 22:51:22.000000 vise-0.7.1/vise/__init__.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-04-23 00:27:13.144455 vise-0.7.1/vise/analyzer/
+-rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-15 22:51:22.000000 vise-0.7.1/vise/analyzer/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1633 2021-03-06 05:00:49.000000 vise-0.7.1/vise/analyzer/atom_grouping_type.py
+-rwxr-xr-x   0 kumagai    (501) staff       (20)     7574 2022-10-21 08:31:12.000000 vise-0.7.1/vise/analyzer/band_edge_properties.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     7667 2022-12-06 07:44:43.000000 vise-0.7.1/vise/analyzer/dielectric_function.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-04-23 00:27:13.148730 vise-0.7.1/vise/analyzer/dielectric_function_data/
+-rw-r--r--   0 kumagai    (501) staff       (20)     3188 2020-11-07 08:48:51.000000 vise-0.7.1/vise/analyzer/dielectric_function_data/GaAs.csv
+-rw-r--r--   0 kumagai    (501) staff       (20)     3474 2020-11-07 08:58:34.000000 vise-0.7.1/vise/analyzer/dielectric_function_data/Si.csv
+-rw-r--r--   0 kumagai    (501) staff       (20)     1422 2020-11-12 08:22:54.000000 vise-0.7.1/vise/analyzer/dielectric_function_data/exp_dielectric_func.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     9812 2023-03-05 02:28:14.000000 vise-0.7.1/vise/analyzer/dos_data.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2222 2021-05-25 08:13:08.000000 vise-0.7.1/vise/analyzer/effective_mass.py
+-rw-r--r--   0 kumagai    (501) staff       (20)    12797 2022-09-10 03:08:43.000000 vise-0.7.1/vise/analyzer/plot_band.py
+-rw-r--r--   0 kumagai    (501) staff       (20)    12057 2022-09-12 04:32:47.000000 vise-0.7.1/vise/analyzer/plot_band_dos.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     6509 2022-10-12 07:02:26.000000 vise-0.7.1/vise/analyzer/plot_brillouin_zone.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     7891 2022-12-06 07:45:00.000000 vise-0.7.1/vise/analyzer/plot_diele_func_data.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4553 2022-12-06 07:30:30.000000 vise-0.7.1/vise/analyzer/plot_dos.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-04-23 00:27:13.160482 vise-0.7.1/vise/analyzer/vasp/
+-rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-15 22:51:22.000000 vise-0.7.1/vise/analyzer/vasp/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2231 2022-08-19 06:07:54.000000 vise-0.7.1/vise/analyzer/vasp/band_edge_properties.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2968 2022-12-06 07:08:20.000000 vise-0.7.1/vise/analyzer/vasp/dos_data.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1474 2021-08-06 10:07:19.000000 vise-0.7.1/vise/analyzer/vasp/handle_volumetric_data.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1866 2022-09-23 02:12:27.000000 vise-0.7.1/vise/analyzer/vasp/make_diele_func.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1242 2021-06-24 07:47:02.000000 vise-0.7.1/vise/analyzer/vasp/make_effective_mass.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     3658 2022-10-04 04:01:43.000000 vise-0.7.1/vise/analyzer/vasp/make_irreps.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     6229 2022-10-06 05:30:09.000000 vise-0.7.1/vise/analyzer/vasp/plot_band.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-04-23 00:27:13.186033 vise-0.7.1/vise/analyzer/vesta/
+-rw-r--r--   0 kumagai    (501) staff       (20)       61 2021-03-12 02:41:40.000000 vise-0.7.1/vise/analyzer/vesta/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4183 2021-03-02 07:24:45.000000 vise-0.7.1/vise/analyzer/vesta/element_colors.py
+-rw-r--r--   0 kumagai    (501) staff       (20)    12453 2021-07-05 05:51:09.000000 vise-0.7.1/vise/analyzer/vesta/vesta_file.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-04-23 00:27:13.192979 vise-0.7.1/vise/atom_energies/
+-rw-r--r--   0 kumagai    (501) staff       (20)       95 2020-05-18 00:09:10.000000 vise-0.7.1/vise/atom_energies/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      290 2020-11-30 06:52:18.000000 vise-0.7.1/vise/atom_energies/atom_energy.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      515 2020-08-11 09:15:50.000000 vise-0.7.1/vise/atom_energies/atom_magnetization_hund.yaml
+-rw-r--r--   0 kumagai    (501) staff       (20)     1217 2021-08-04 07:35:01.000000 vise-0.7.1/vise/atom_energies/get_energy.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2267 2022-07-05 01:18:05.000000 vise-0.7.1/vise/atom_energies/make_atom_vasp_set.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1135 2020-11-30 02:31:47.000000 vise-0.7.1/vise/atom_energies/mp_atom_energy.yaml
+-rw-r--r--   0 kumagai    (501) staff       (20)      709 2020-11-30 02:31:47.000000 vise-0.7.1/vise/atom_energies/mp_atom_mag.yaml
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-04-23 00:27:13.197467 vise-0.7.1/vise/cli/
+-rw-r--r--   0 kumagai    (501) staff       (20)       72 2020-05-15 22:51:22.000000 vise-0.7.1/vise/cli/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)    14069 2023-04-22 22:01:47.000000 vise-0.7.1/vise/cli/main.py
+-rw-r--r--   0 kumagai    (501) staff       (20)    14642 2023-04-22 22:07:43.000000 vise-0.7.1/vise/cli/main_functions.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     3506 2020-10-03 03:00:38.000000 vise-0.7.1/vise/cli/main_tools.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4944 2021-08-06 10:08:41.000000 vise-0.7.1/vise/cli/main_util.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2216 2021-05-05 00:16:26.000000 vise-0.7.1/vise/cli/main_util_functions.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4294 2022-11-14 04:27:07.000000 vise-0.7.1/vise/defaults.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      134 2020-05-15 22:51:22.000000 vise-0.7.1/vise/error.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-04-23 00:27:13.206475 vise-0.7.1/vise/input_set/
+-rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-15 22:51:22.000000 vise-0.7.1/vise/input_set/__init__.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-04-23 00:27:13.211344 vise-0.7.1/vise/input_set/datasets/
+-rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-15 22:51:22.000000 vise-0.7.1/vise/input_set/datasets/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2594 2023-04-22 23:04:53.000000 vise-0.7.1/vise/input_set/datasets/dataset_util.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1642 2022-12-19 07:34:18.000000 vise-0.7.1/vise/input_set/datasets/incar_flags.yaml
+-rw-r--r--   0 kumagai    (501) staff       (20)      685 2020-05-15 22:51:22.000000 vise-0.7.1/vise/input_set/datasets/kpar_set.yaml
+-rw-r--r--   0 kumagai    (501) staff       (20)      294 2020-05-15 22:51:22.000000 vise-0.7.1/vise/input_set/datasets/magmom.yaml
+-rw-r--r--   0 kumagai    (501) staff       (20)     1516 2020-05-15 22:51:22.000000 vise-0.7.1/vise/input_set/datasets/potcar_set.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4024 2020-12-23 01:37:43.000000 vise-0.7.1/vise/input_set/datasets/potcar_set.yaml
+-rw-r--r--   0 kumagai    (501) staff       (20)      623 2021-05-06 06:02:40.000000 vise-0.7.1/vise/input_set/datasets/u_parameter_set.yaml
+-rw-r--r--   0 kumagai    (501) staff       (20)      574 2020-05-15 22:51:22.000000 vise-0.7.1/vise/input_set/datasets/unoccupied_bands.yaml
+-rw-r--r--   0 kumagai    (501) staff       (20)     1141 2022-07-23 04:43:00.000000 vise-0.7.1/vise/input_set/fft_grids.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4149 2023-04-22 23:06:02.000000 vise-0.7.1/vise/input_set/incar.py
+-rw-r--r--   0 kumagai    (501) staff       (20)    12667 2022-11-30 06:56:02.000000 vise-0.7.1/vise/input_set/incar_settings_generator.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4026 2022-11-14 04:20:42.000000 vise-0.7.1/vise/input_set/input_options.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1360 2020-05-15 22:51:22.000000 vise-0.7.1/vise/input_set/kpoints.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1279 2020-05-15 22:51:22.000000 vise-0.7.1/vise/input_set/kpoints_mode.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      914 2020-05-15 22:51:22.000000 vise-0.7.1/vise/input_set/potcar_generator.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4022 2021-08-04 07:35:03.000000 vise-0.7.1/vise/input_set/prior_info.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     8136 2023-04-22 21:47:54.000000 vise-0.7.1/vise/input_set/structure_kpoints_generator.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     3912 2022-10-06 08:28:55.000000 vise-0.7.1/vise/input_set/task.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4131 2022-11-04 09:21:10.000000 vise-0.7.1/vise/input_set/vasp_input_files.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1322 2022-10-21 08:42:57.000000 vise-0.7.1/vise/input_set/vise_log.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      956 2020-06-03 03:20:45.000000 vise-0.7.1/vise/input_set/xc.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-04-23 00:27:13.213846 vise-0.7.1/vise/tests/
+-rw-r--r--   0 kumagai    (501) staff       (20)       96 2020-05-15 22:51:22.000000 vise-0.7.1/vise/tests/__init__.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-04-23 00:27:13.220763 vise-0.7.1/vise/tests/analyzer/
+-rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-15 22:51:22.000000 vise-0.7.1/vise/tests/analyzer/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1503 2020-11-30 08:10:26.000000 vise-0.7.1/vise/tests/analyzer/test_atom_grouping_type.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     8181 2022-09-30 06:32:39.000000 vise-0.7.1/vise/tests/analyzer/test_band_edge_properties.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     3441 2022-11-03 04:27:22.000000 vise-0.7.1/vise/tests/analyzer/test_dielectric_function.py
+-rw-r--r--   0 kumagai    (501) staff       (20)    10283 2023-01-31 00:31:50.000000 vise-0.7.1/vise/tests/analyzer/test_dos_data.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1951 2021-05-25 08:12:05.000000 vise-0.7.1/vise/tests/analyzer/test_effective_mass.py
+-rw-r--r--   0 kumagai    (501) staff       (20)    12879 2022-09-13 00:24:09.000000 vise-0.7.1/vise/tests/analyzer/test_plot_band.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1576 2022-09-12 00:48:30.000000 vise-0.7.1/vise/tests/analyzer/test_plot_band_dos.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2099 2022-10-21 06:44:45.000000 vise-0.7.1/vise/tests/analyzer/test_plot_brillouin_zone.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2639 2022-12-06 07:46:00.000000 vise-0.7.1/vise/tests/analyzer/test_plot_diele_func_data.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     7869 2022-12-06 07:02:33.000000 vise-0.7.1/vise/tests/analyzer/test_plot_dos.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-04-23 00:27:13.225056 vise-0.7.1/vise/tests/analyzer/vasp/
+-rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-15 22:51:22.000000 vise-0.7.1/vise/tests/analyzer/vasp/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2282 2021-03-06 04:52:09.000000 vise-0.7.1/vise/tests/analyzer/vasp/test_band_edge_properties.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     3504 2021-03-06 04:52:35.000000 vise-0.7.1/vise/tests/analyzer/vasp/test_dos_data.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1607 2022-10-21 07:15:26.000000 vise-0.7.1/vise/tests/analyzer/vasp/test_handle_volumetric_data.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1900 2022-09-23 00:52:48.000000 vise-0.7.1/vise/tests/analyzer/vasp/test_make_diele_func.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2517 2021-06-24 07:56:18.000000 vise-0.7.1/vise/tests/analyzer/vasp/test_make_effective_mass.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2015 2022-09-13 01:26:49.000000 vise-0.7.1/vise/tests/analyzer/vasp/test_make_irreps.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     5783 2022-10-06 05:29:21.000000 vise-0.7.1/vise/tests/analyzer/vasp/test_plot_band.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-04-23 00:27:13.228501 vise-0.7.1/vise/tests/cli/
+-rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-15 22:51:22.000000 vise-0.7.1/vise/tests/cli/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     8832 2023-04-22 22:01:47.000000 vise-0.7.1/vise/tests/cli/test_main.py
+-rw-r--r--   0 kumagai    (501) staff       (20)    11040 2023-04-22 22:12:44.000000 vise-0.7.1/vise/tests/cli/test_main_functions.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1683 2022-07-29 02:57:51.000000 vise-0.7.1/vise/tests/cli/test_main_tools.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2249 2021-04-30 01:10:17.000000 vise-0.7.1/vise/tests/cli/test_main_util.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2463 2021-05-04 23:31:17.000000 vise-0.7.1/vise/tests/cli/test_main_util_functions.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1785 2022-09-10 03:00:55.000000 vise-0.7.1/vise/tests/conftest.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-04-23 00:27:13.229881 vise-0.7.1/vise/tests/helpers/
+-rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-14 10:39:18.000000 vise-0.7.1/vise/tests/helpers/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     5858 2023-01-31 00:32:00.000000 vise-0.7.1/vise/tests/helpers/assertion.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4419 2022-09-30 04:31:05.000000 vise-0.7.1/vise/tests/helpers/test_assersion.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-04-23 00:27:13.237230 vise-0.7.1/vise/tests/input_set/
+-rw-r--r--   0 kumagai    (501) staff       (20)       96 2020-05-15 22:51:22.000000 vise-0.7.1/vise/tests/input_set/__init__.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-04-23 00:27:13.239008 vise-0.7.1/vise/tests/input_set/datasets/
+-rw-r--r--   0 kumagai    (501) staff       (20)       96 2020-05-15 22:51:22.000000 vise-0.7.1/vise/tests/input_set/datasets/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1519 2022-11-14 04:00:11.000000 vise-0.7.1/vise/tests/input_set/datasets/test_dataset_util.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      780 2020-05-15 22:51:22.000000 vise-0.7.1/vise/tests/input_set/datasets/test_potcar_set.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      232 2022-01-27 04:37:06.000000 vise-0.7.1/vise/tests/input_set/test_fft_grids.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1667 2023-04-22 23:04:07.000000 vise-0.7.1/vise/tests/input_set/test_incar.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     8997 2022-11-14 04:40:23.000000 vise-0.7.1/vise/tests/input_set/test_incar_settings_generator.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     3796 2022-07-26 07:16:22.000000 vise-0.7.1/vise/tests/input_set/test_input_options.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      533 2020-05-15 22:51:22.000000 vise-0.7.1/vise/tests/input_set/test_kpoints_mode.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1555 2021-03-05 09:50:13.000000 vise-0.7.1/vise/tests/input_set/test_potcar_generator.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2565 2022-07-01 00:59:32.000000 vise-0.7.1/vise/tests/input_set/test_prior_info.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     9329 2023-03-08 02:30:32.000000 vise-0.7.1/vise/tests/input_set/test_structure_kpoints_generator.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     3410 2022-10-06 08:28:37.000000 vise-0.7.1/vise/tests/input_set/test_task.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1573 2022-11-14 04:18:29.000000 vise-0.7.1/vise/tests/input_set/test_vasp_input_files.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1211 2022-10-21 08:43:44.000000 vise-0.7.1/vise/tests/input_set/test_vise_log.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1162 2021-03-02 02:37:28.000000 vise-0.7.1/vise/tests/input_set/test_xc.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4762 2022-11-06 00:50:42.000000 vise-0.7.1/vise/tests/test_defaults.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1784 2022-10-21 08:06:31.000000 vise-0.7.1/vise/tests/test_user_settings.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-04-23 00:27:13.290516 vise-0.7.1/vise/tests/util/
+-rw-r--r--   0 kumagai    (501) staff       (20)       96 2020-05-15 22:51:22.000000 vise-0.7.1/vise/tests/util/__init__.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-04-23 00:27:13.292175 vise-0.7.1/vise/tests/util/phonopy/
+-rw-r--r--   0 kumagai    (501) staff       (20)       96 2020-05-15 22:51:22.000000 vise-0.7.1/vise/tests/util/phonopy/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     3100 2021-08-06 10:08:41.000000 vise-0.7.1/vise/tests/util/phonopy/test_phonopy_input.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1499 2020-05-15 22:51:22.000000 vise-0.7.1/vise/tests/util/test_bravais_lattice.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2441 2021-03-05 09:50:13.000000 vise-0.7.1/vise/tests/util/test_centering.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4437 2020-05-15 22:51:22.000000 vise-0.7.1/vise/tests/util/test_file_transfer.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      217 2020-08-02 02:24:25.000000 vise-0.7.1/vise/tests/util/test_logger.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      511 2020-05-15 22:51:22.000000 vise-0.7.1/vise/tests/util/test_matplotlib.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1500 2022-09-28 23:59:57.000000 vise-0.7.1/vise/tests/util/test_mix_in.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      232 2021-04-18 02:48:05.000000 vise-0.7.1/vise/tests/util/test_string.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     9778 2021-07-31 08:14:24.000000 vise-0.7.1/vise/tests/util/test_structure_symmetrizer.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      471 2021-08-01 00:43:34.000000 vise-0.7.1/vise/tests/util/test_valence_orbitals_from_potcar.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2143 2022-11-15 04:24:17.000000 vise-0.7.1/vise/user_settings.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-04-23 00:27:13.308520 vise-0.7.1/vise/util/
+-rw-r--r--   0 kumagai    (501) staff       (20)     3450 2021-09-15 23:40:59.000000 vise-0.7.1/vise/util/Hermann-Mauguin.yaml
+-rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-15 22:51:22.000000 vise-0.7.1/vise/util/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     6893 2023-03-07 23:24:41.000000 vise-0.7.1/vise/util/bravais_lattice.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1786 2020-05-14 03:15:55.000000 vise-0.7.1/vise/util/centering.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      304 2020-11-12 05:19:29.000000 vise-0.7.1/vise/util/dash_helper.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      788 2021-05-30 03:06:06.000000 vise-0.7.1/vise/util/enum.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2746 2020-11-30 22:31:41.000000 vise-0.7.1/vise/util/file_transfer.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1234 2021-05-01 05:11:26.000000 vise-0.7.1/vise/util/logger.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      802 2020-05-15 22:51:22.000000 vise-0.7.1/vise/util/matplotlib.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2752 2022-09-30 04:31:19.000000 vise-0.7.1/vise/util/mix_in.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-04-23 00:27:13.329227 vise-0.7.1/vise/util/phonopy/
+-rw-r--r--   0 kumagai    (501) staff       (20)       96 2020-05-15 22:51:22.000000 vise-0.7.1/vise/util/phonopy/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4058 2022-09-06 01:13:47.000000 vise-0.7.1/vise/util/phonopy/phonopy_input.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2043 2021-08-11 05:37:35.000000 vise-0.7.1/vise/util/plotly_util.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      986 2022-07-29 03:01:33.000000 vise-0.7.1/vise/util/str_related_tools.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      786 2021-04-20 00:50:10.000000 vise-0.7.1/vise/util/string.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      486 2021-03-05 09:50:13.000000 vise-0.7.1/vise/util/structure_handler.py
+-rw-r--r--   0 kumagai    (501) staff       (20)    13330 2022-11-14 04:29:55.000000 vise-0.7.1/vise/util/structure_symmetrizer.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      229 2021-05-02 02:13:00.000000 vise-0.7.1/vise/util/typing.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      226 2021-07-05 05:51:09.000000 vise-0.7.1/vise/util/unit_conversion.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      419 2021-07-05 06:55:26.000000 vise-0.7.1/vise/util/valence_orbitals_from_potcar.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      117 2023-04-23 00:26:10.000000 vise-0.7.1/vise/version.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-04-23 00:27:13.132941 vise-0.7.1/vise.egg-info/
+-rw-r--r--   0 kumagai    (501) staff       (20)     4389 2023-04-23 00:27:12.000000 vise-0.7.1/vise.egg-info/PKG-INFO
+-rw-r--r--   0 kumagai    (501) staff       (20)     5313 2023-04-23 00:27:12.000000 vise-0.7.1/vise.egg-info/SOURCES.txt
+-rw-r--r--   0 kumagai    (501) staff       (20)        1 2023-04-23 00:27:12.000000 vise-0.7.1/vise.egg-info/dependency_links.txt
+-rw-r--r--   0 kumagai    (501) staff       (20)       81 2023-04-23 00:27:12.000000 vise-0.7.1/vise.egg-info/entry_points.txt
+-rw-r--r--   0 kumagai    (501) staff       (20)      163 2023-04-23 00:27:12.000000 vise-0.7.1/vise.egg-info/requires.txt
+-rw-r--r--   0 kumagai    (501) staff       (20)        5 2023-04-23 00:27:12.000000 vise-0.7.1/vise.egg-info/top_level.txt
```

### Comparing `vise-0.7.0/PKG-INFO` & `vise-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vise
-Version: 0.7.0
+Version: 0.7.1
 Summary: Package for handling io of vasp package in kumagai group at IMR, Tohoku university
 Home-page: https://github.com/kumagai-group/vise
 Author: Yu Kumagai
 Author-email: yukumagai@tohoku.ac.jp
 License: MIT license
 Description: ![PyPI - License](https://img.shields.io/pypi/l/vise?color=blue)
         ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/vise)
```

### Comparing `vise-0.7.0/README.md` & `vise-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/setup.py` & `vise-0.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/analyzer/atom_grouping_type.py` & `vise-0.7.1/vise/analyzer/atom_grouping_type.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/analyzer/band_edge_properties.py` & `vise-0.7.1/vise/analyzer/band_edge_properties.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/analyzer/dielectric_function.py` & `vise-0.7.1/vise/analyzer/dielectric_function.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/analyzer/dielectric_function_data/GaAs.csv` & `vise-0.7.1/vise/analyzer/dielectric_function_data/GaAs.csv`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/analyzer/dielectric_function_data/Si.csv` & `vise-0.7.1/vise/analyzer/dielectric_function_data/Si.csv`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/analyzer/dielectric_function_data/exp_dielectric_func.py` & `vise-0.7.1/vise/analyzer/dielectric_function_data/exp_dielectric_func.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/analyzer/dos_data.py` & `vise-0.7.1/vise/analyzer/dos_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 #  Copyright (c) 2020. Distributed under the terms of the MIT License.
 from collections import defaultdict
 from copy import copy, deepcopy
-from dataclasses import dataclass
+from dataclasses import dataclass, fields
 from functools import reduce
 from typing import Dict, Optional, List
 
 import numpy as np
 import pandas as pd
 from monty.json import MSONable
 from vise.util.logger import get_logger
 from vise.util.mix_in import ToJsonFileMixIn, ToCsvFileMixIn
 
 logger = get_logger(__name__)
 
 
 @dataclass
-class PDos(MSONable):
+class PDos(MSONable, ToJsonFileMixIn):
     s:   np.ndarray  # [by spin][by energy]
     px:  np.ndarray
     py:  np.ndarray
     pz:  np.ndarray
     dxy: np.ndarray
     dyz: np.ndarray
     dxz: np.ndarray
@@ -76,23 +76,33 @@
         for k, v in self.__dict__.items():
             if v is None:
                 args[k] = None
             else:
                 args[k] = v + getattr(other, k)
         return PDos(**args)
 
+    def __eq__(self, other: "PDos"):
+        for k, v in self.__dict__.items():
+            if (v != getattr(other, k)).any():
+                return False
+        return True
+
 
 @dataclass
 class DosData(MSONable):
     energies: List[float]
     total: np.ndarray
     pdos: List[PDos]
     vertical_lines: List[float]
     base_energy: Optional[float] = 0.0
 
+    def __post_init__(self):
+        if isinstance(self.total, list):
+            self.total = np.array(self.total)
+
     @property
     def spin(self):
         return False if len(self.total) == 1 else True
 
     def dos_plot_data(self,
                       grouped_atom_indices: Dict[str, List[int]],
                       energy_range: Optional[List[float]] = None,
```

### Comparing `vise-0.7.0/vise/analyzer/effective_mass.py` & `vise-0.7.1/vise/analyzer/effective_mass.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/analyzer/plot_band.py` & `vise-0.7.1/vise/analyzer/plot_band.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/analyzer/plot_band_dos.py` & `vise-0.7.1/vise/analyzer/plot_band_dos.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/analyzer/plot_brillouin_zone.py` & `vise-0.7.1/vise/analyzer/plot_brillouin_zone.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/analyzer/plot_diele_func_data.py` & `vise-0.7.1/vise/analyzer/plot_diele_func_data.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/analyzer/plot_dos.py` & `vise-0.7.1/vise/analyzer/plot_dos.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/analyzer/vasp/band_edge_properties.py` & `vise-0.7.1/vise/analyzer/vasp/band_edge_properties.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/analyzer/vasp/dos_data.py` & `vise-0.7.1/vise/analyzer/vasp/dos_data.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/analyzer/vasp/handle_volumetric_data.py` & `vise-0.7.1/vise/analyzer/vasp/handle_volumetric_data.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/analyzer/vasp/make_diele_func.py` & `vise-0.7.1/vise/analyzer/vasp/make_diele_func.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/analyzer/vasp/make_effective_mass.py` & `vise-0.7.1/vise/analyzer/vasp/make_effective_mass.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/analyzer/vasp/make_irreps.py` & `vise-0.7.1/vise/analyzer/vasp/make_irreps.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/analyzer/vasp/plot_band.py` & `vise-0.7.1/vise/analyzer/vasp/plot_band.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/analyzer/vesta/element_colors.py` & `vise-0.7.1/vise/analyzer/vesta/element_colors.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/analyzer/vesta/vesta_file.py` & `vise-0.7.1/vise/analyzer/vesta/vesta_file.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/atom_energies/atom_magnetization_hund.yaml` & `vise-0.7.1/vise/atom_energies/atom_magnetization_hund.yaml`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/atom_energies/get_energy.py` & `vise-0.7.1/vise/atom_energies/get_energy.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/atom_energies/make_atom_vasp_set.py` & `vise-0.7.1/vise/atom_energies/make_atom_vasp_set.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/atom_energies/mp_atom_energy.yaml` & `vise-0.7.1/vise/atom_energies/mp_atom_energy.yaml`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/atom_energies/mp_atom_mag.yaml` & `vise-0.7.1/vise/atom_energies/mp_atom_mag.yaml`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/cli/main.py` & `vise-0.7.1/vise/cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,18 @@
         name="vasp_set",
         description="Constructs vasp input set",
         parents=[vasprun_parser, outcar_parser],
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
         aliases=['vs'])
 
     parser_vasp_set.add_argument(
-        "-p", "--poscar", default="POSCAR", type=Path,
+        "-d", "--dirs", nargs="+", type=Path, default=[Path.cwd()],
+        help="Directory paths to be parsed.")
+    parser_vasp_set.add_argument(
+        "-p", "--poscar", default=None, type=Path,
         help="POSCAR-type input structure file name.")
     parser_vasp_set.add_argument(
         "-t", dest="task", default=defaults.task, type=Task,
         choices=Task.name_list(),
         help=f"Task name.")
     parser_vasp_set.add_argument(
         "-x", dest="xc", default=defaults.xc, type=Xc, choices=Xc.name_list(),
@@ -126,15 +129,15 @@
         help="User specifying POTCAR set. E.g., Mg_pv O_h")
     parser_vasp_set.add_argument(
         "-uis", "--user_incar_settings", type=str, nargs="+",
         help="""Overwritten incar settings described with pairs of INCAR tag 
         names and values. These can also be set by vise.yaml, but they are 
         overwritten by this command line options.""")
     parser_vasp_set.add_argument(
-        "-d", "--prev_dir", type=Path,
+        "-pd", "--prev_dir", type=Path,
         help="Parse the previous calculations for better input settings.")
     parser_vasp_set.add_argument(
         "--options", type=str, nargs="+",
         help="Manual options used at CategorizedInputOptions class.")
     parser_vasp_set.add_argument(
         "--uniform_kpt_mode", action="store_true",
         help="""Kpoints with uniform k-point sampling. The k-point sampling mesh
```

### Comparing `vise-0.7.0/vise/cli/main_functions.py` & `vise-0.7.1/vise/cli/main_functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
 #  Copyright (c) 2020. Distributed under the terms of the MIT License.
+import os
 from argparse import Namespace
 from copy import deepcopy
 from pathlib import Path
 
 import yaml
 from pymatgen.core import Structure
 from pymatgen.ext.matproj import MPRester
@@ -142,41 +143,53 @@
 
     Path("prior_info.yaml").write_text(yaml.dump(d), None)
 
 
 class VaspSet:
     def __init__(self, args: Namespace):
         self.args = args
+        if args.prev_dir:
+            self.args.prev_dir = args.prev_dir.absolute()
+        if args.poscar:
+            self.args.poscar = args.poscar.absolute()
 
         try:
             self._prior_info = PriorInfo.load_yaml()
         except FileNotFoundError:
             self._prior_info = PriorInfo()
         self.task = Task.cluster_opt if self._prior_info.is_cluster \
             else args.task
 
-        options = CategorizedInputOptions(
-            structure=self._structure(),
-            task=self.task,
-            xc=args.xc,
-            kpt_density=args.kpt_density,
-            overridden_potcar=self._overridden_potcar(),
-            **self._option_kwargs())
-
-        vif = VaspInputFiles(options, self._overridden_incar_settings())
-        vif.create_input_files(Path.cwd())
-        if hasattr(self, "_file_transfers"):
-            self._file_transfers.transfer()
-        vif.vise_log.to_yaml_file()
+        for _dir in [d.absolute() for d in args.dirs]:
+            if _dir.is_file():
+                logger.info(f"{_dir} is a file, so skipped.")
+                continue
+
+            os.chdir(_dir)
+            options = CategorizedInputOptions(
+                structure=self._structure(),
+                task=self.task,
+                xc=args.xc,
+                kpt_density=args.kpt_density,
+                overridden_potcar=self._overridden_potcar(),
+                **self._option_kwargs())
+
+            vif = VaspInputFiles(options, self._overridden_incar_settings())
+            vif.create_input_files(Path.cwd())
+            if hasattr(self, "_file_transfers"):
+                self._file_transfers.transfer()
+            vif.vise_log.to_yaml_file()
 
     def _structure(self):
         # avoid overlapping structure for e.g., phonon forces.
         if self.args.prev_dir and self.task.fine_to_inherit_structure_from_prev:
             return Structure.from_file(self.args.prev_dir / defaults.contcar)
-        return Structure.from_file(self.args.poscar)
+        if self.args.poscar:
+            return Structure.from_file(self.args.poscar)
+        return Structure.from_file("POSCAR")
 
     def _overridden_incar_settings(self):
         result = deepcopy(defaults.user_incar_settings)
         result.update(self._prior_info.incar)
 
         if self.args.user_incar_settings:
             args = list2dict(self.args.user_incar_settings, all_incar_flags)
```

### Comparing `vise-0.7.0/vise/cli/main_tools.py` & `vise-0.7.1/vise/cli/main_tools.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/cli/main_util.py` & `vise-0.7.1/vise/cli/main_util.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/cli/main_util_functions.py` & `vise-0.7.1/vise/cli/main_util_functions.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/defaults.py` & `vise-0.7.1/vise/defaults.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/input_set/datasets/dataset_util.py` & `vise-0.7.1/vise/input_set/datasets/dataset_util.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,23 +3,25 @@
 from math import ceil
 from pathlib import Path
 from typing import Tuple, List, Dict, Any
 
 from monty.serialization import loadfn
 from pymatgen.core import Composition, Element
 from pymatgen.io.vasp import Potcar
+from pymatgen.io.vasp.inputs import incar_params
 from vise.defaults import defaults
 
 unoccupied_bands = loadfn(Path(__file__).parent / "unoccupied_bands.yaml")
 
 # This incar_flags should be OrderedDict, but from python 3.6, dict uses
 # order-preserving semantics. Besides, it does not affect vasp result.
 incar_categories: Dict[str, Any] = \
-    loadfn(Path(__file__).parent / "incar_flags.yaml")
-all_incar_flags: List[str] = sum(incar_categories.values(), [])
+    dict(loadfn(Path(__file__).parent / "incar_flags.yaml"))
+tag_set = set(tuple(tags) for tags in incar_categories)
+incar_categories["others"] = set(incar_params.keys()) - tag_set
 
 
 def has_f_elements(symbol_list: List[str]):
     return any([Element(el).Z > 56 for el in symbol_list])
 
 
 class LDAU:
```

### Comparing `vise-0.7.0/vise/input_set/datasets/incar_flags.yaml` & `vise-0.7.1/vise/input_set/datasets/incar_flags.yaml`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/input_set/datasets/kpar_set.yaml` & `vise-0.7.1/vise/input_set/datasets/kpar_set.yaml`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/input_set/datasets/potcar_set.py` & `vise-0.7.1/vise/input_set/datasets/potcar_set.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/input_set/datasets/potcar_set.yaml` & `vise-0.7.1/vise/input_set/datasets/potcar_set.yaml`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/input_set/datasets/u_parameter_set.yaml` & `vise-0.7.1/vise/input_set/datasets/u_parameter_set.yaml`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/input_set/datasets/unoccupied_bands.yaml` & `vise-0.7.1/vise/input_set/datasets/unoccupied_bands.yaml`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/input_set/fft_grids.py` & `vise-0.7.1/vise/input_set/fft_grids.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/input_set/incar.py` & `vise-0.7.1/vise/input_set/incar.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,16 +83,16 @@
                         [flag, self.setting_to_str(flag)])
                     input_incar_flags.remove(flag)
 
             if settings_by_category:
                 lines[f"# {category}"] = tabulated_string(settings_by_category)
 
         if input_incar_flags:
-            logger.error(f"{input_incar_flags} may be invalid in INCAR.")
-            lines[f"# others"] = tabulated_string(input_incar_flags)
+            logger.error(f"{input_incar_flags} may be invalid in INCAR.,"
+                         f"We are sorry, but add it by hands")
 
         return "\n\n".join(["\n".join([k, v]) for k, v in lines.items()])
 
     def setting_to_str(self, incar_flag: str) -> str:
         if isinstance(self[incar_flag], list):
             return " ".join([str(i) for i in self[incar_flag]])
         else:
```

### Comparing `vise-0.7.0/vise/input_set/incar_settings_generator.py` & `vise-0.7.1/vise/input_set/incar_settings_generator.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/input_set/input_options.py` & `vise-0.7.1/vise/input_set/input_options.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/input_set/kpoints.py` & `vise-0.7.1/vise/input_set/kpoints.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/input_set/kpoints_mode.py` & `vise-0.7.1/vise/input_set/kpoints_mode.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/input_set/potcar_generator.py` & `vise-0.7.1/vise/input_set/potcar_generator.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/input_set/prior_info.py` & `vise-0.7.1/vise/input_set/prior_info.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/input_set/structure_kpoints_generator.py` & `vise-0.7.1/vise/input_set/structure_kpoints_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,17 @@
             self._structure = self._initial_structure.copy()
         elif self._kpt_mode == KpointsMode.primitive:
             self._structure = self._symmetrizer.primitive
         elif self._kpt_mode == KpointsMode.band:
             self._structure = self._symmetrizer.band_primitive
         else:
             raise NotImplementedError
+        if self._structure != self._initial_structure:
+            logger.info("The input structure is changed. When you do not want "
+                        "to change it, use --uniform_kpt_mode.")
 
     def _make_kpoints(self):
         self._set_num_kpt_list()
         self._set_kpt_shift()
         self._set_kpoints()
 
     def _set_num_kpt_list(self) -> None:
```

### Comparing `vise-0.7.0/vise/input_set/task.py` & `vise-0.7.1/vise/input_set/task.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/input_set/vasp_input_files.py` & `vise-0.7.1/vise/input_set/vasp_input_files.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/input_set/vise_log.py` & `vise-0.7.1/vise/input_set/vise_log.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/input_set/xc.py` & `vise-0.7.1/vise/input_set/xc.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/tests/analyzer/test_atom_grouping_type.py` & `vise-0.7.1/vise/tests/analyzer/test_atom_grouping_type.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/tests/analyzer/test_band_edge_properties.py` & `vise-0.7.1/vise/tests/analyzer/test_band_edge_properties.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/tests/analyzer/test_dielectric_function.py` & `vise-0.7.1/vise/tests/analyzer/test_dielectric_function.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/tests/analyzer/test_dos_data.py` & `vise-0.7.1/vise/tests/analyzer/test_dos_data.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/tests/analyzer/test_effective_mass.py` & `vise-0.7.1/vise/tests/analyzer/test_effective_mass.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/tests/analyzer/test_plot_band.py` & `vise-0.7.1/vise/tests/analyzer/test_plot_band.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/tests/analyzer/test_plot_band_dos.py` & `vise-0.7.1/vise/tests/analyzer/test_plot_band_dos.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/tests/analyzer/test_plot_brillouin_zone.py` & `vise-0.7.1/vise/tests/analyzer/test_plot_brillouin_zone.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/tests/analyzer/test_plot_diele_func_data.py` & `vise-0.7.1/vise/tests/analyzer/test_plot_diele_func_data.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/tests/analyzer/test_plot_dos.py` & `vise-0.7.1/vise/tests/analyzer/test_plot_dos.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/tests/analyzer/vasp/test_band_edge_properties.py` & `vise-0.7.1/vise/tests/analyzer/vasp/test_band_edge_properties.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/tests/analyzer/vasp/test_dos_data.py` & `vise-0.7.1/vise/tests/analyzer/vasp/test_dos_data.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/tests/analyzer/vasp/test_handle_volumetric_data.py` & `vise-0.7.1/vise/tests/analyzer/vasp/test_handle_volumetric_data.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/tests/analyzer/vasp/test_make_diele_func.py` & `vise-0.7.1/vise/tests/analyzer/vasp/test_make_diele_func.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/tests/analyzer/vasp/test_make_effective_mass.py` & `vise-0.7.1/vise/tests/analyzer/vasp/test_make_effective_mass.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/tests/analyzer/vasp/test_make_irreps.py` & `vise-0.7.1/vise/tests/analyzer/vasp/test_make_irreps.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/tests/analyzer/vasp/test_plot_band.py` & `vise-0.7.1/vise/tests/analyzer/vasp/test_plot_band.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/tests/cli/test_main.py` & `vise-0.7.1/vise/tests/cli/test_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,16 @@
     assert parsed_args == expected
 
 
 def test_vasp_set_wo_options():
     parsed_args = parse_args(["vs"])
     # func is a pointer so need to point the same address.
     expected = Namespace(
-        poscar=Path("POSCAR"),
+        dirs=[Path.cwd()],
+        poscar=None,
         task=defaults.task,
         xc=defaults.xc,
         kpt_density=None,
         overridden_potcar=defaults.overridden_potcar,
         user_incar_settings=None,
         prev_dir=None,
         vasprun=defaults.vasprun,
@@ -81,29 +82,31 @@
         func=parsed_args.func,
         )
     assert parsed_args == expected
 
 
 def test_vasp_set_w_options():
     parsed_args = parse_args(["vs",
+                              "-d", "Va_O1_0", "Va_O1_1",
                               "--poscar", "POSCAR-tmp",
                               "-t", "band",
                               "-x", "pbesol",
                               "-k", "4.2",
                               "--potcar", "Mg_pv", "O_h",
                               "--user_incar_settings", "LREAD", "F",
-                              "-d", "c",
+                              "-pd", "c",
                               "--vasprun", "vasprun_1",
                               "--outcar", "OUTCAR_1",
                               "--options", "encut", "800",
                               "--uniform_kpt_mode",
                               "--file_transfer", "WAVECAR", "C",
                               ])
 
     expected = Namespace(
+        dirs=[Path("Va_O1_0"), Path("Va_O1_1")],
         poscar=Path("POSCAR-tmp"),
         task=Task.band,
         xc=Xc.pbesol,
         kpt_density=4.2,
         overridden_potcar=["Mg_pv", "O_h"],
         user_incar_settings=["LREAD", "F"],
         prev_dir=Path("c"),
```

### Comparing `vise-0.7.0/vise/tests/cli/test_main_functions.py` & `vise-0.7.1/vise/tests/cli/test_main_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,45 +15,46 @@
     structure_info, get_most_stable_mp_id_from_formula, \
     get_most_stable_mp_id_from_formula_w_new_mprester
 from vise.defaults import defaults
 from vise.input_set.kpoints_mode import KpointsMode
 from vise.input_set.task import Task
 from vise.input_set.xc import Xc
 
-default_option_args = {"poscar": "POSCAR",
+default_option_args = {"poscar": Path("POSCAR"),
                        "task": Task.structure_opt,
                        "xc": Xc.pbe,
                        "kpt_density": 1.0,
                        "overridden_potcar": ["Mn_pv"]}
 
 default_args = deepcopy(default_option_args)
-default_args.update({"user_incar_settings": None,
+default_args.update({"dirs": [Path.cwd()],
+                     "user_incar_settings": None,
                      "prev_dir": None,
                      "options": None,
                      "file_transfer_type": None,
                      "uniform_kpt_mode": False,
                      "vasprun": Path("vasprun.xml"),
                      "outcar": Path("outcar.xml"),
                      })
 
 
 def test_structure_info(mocker):
-    args = Namespace(poscar="POSCAR", symprec=0.1, angle_tolerance=5,
+    args = Namespace(poscar=Path("POSCAR"), symprec=0.1, angle_tolerance=5,
                      show_conventional=False, show_primitive=False)
     lattice = [[10.0,  0.0,  0.0], [0.0, 10.0,  0.0], [-2.0,  0.0, 10.0]]
     coords = [[0.0, 0.0, 0.0], [0.5, 0.5, 0.0]]
 
     mock = mocker.patch("vise.cli.main_functions.Structure")
     mock.from_file.return_value = Structure(lattice=lattice, species=["H"] * 2,
                                             coords=coords)
     structure_info(args)
-    args = Namespace(poscar="POSCAR", symprec=0.1, angle_tolerance=5,
+    args = Namespace(poscar=Path("POSCAR"), symprec=0.1, angle_tolerance=5,
                      show_conventional=True, show_primitive=False)
     structure_info(args)
-    args = Namespace(poscar="POSCAR", symprec=0.1, angle_tolerance=5,
+    args = Namespace(poscar=Path("POSCAR"), symprec=0.1, angle_tolerance=5,
                      show_conventional=True, show_primitive=True)
     structure_info(args)
 
 
 def test_get_most_stable_mp_id_from_formula():
     actual = get_most_stable_mp_id_from_formula_w_new_mprester("MgO")
     assert actual == "mp-1265"
```

### Comparing `vise-0.7.0/vise/tests/cli/test_main_tools.py` & `vise-0.7.1/vise/tests/cli/test_main_tools.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/tests/cli/test_main_util.py` & `vise-0.7.1/vise/tests/cli/test_main_util.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/tests/cli/test_main_util_functions.py` & `vise-0.7.1/vise/tests/cli/test_main_util_functions.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/tests/conftest.py` & `vise-0.7.1/vise/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/tests/helpers/assertion.py` & `vise-0.7.1/vise/tests/helpers/assertion.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,19 +57,23 @@
 def assert_json_roundtrip(obj, tmpdir):
     tmpdir.chdir()
     obj.to_json_file("a.json")
     actual = loadfn("a.json").as_dict()
     expected = obj.as_dict()
     for k, v in actual.items():
         try:
-            assert v == expected[k]
+            if isinstance(v, np.ndarray):
+                (v == expected[k]).all()
+            else:
+                assert v == expected[k]
         except AssertionError:
             print(k)
             print(v)
             print(expected[k])
+            raise
 
 
 def assert_yaml_roundtrip(obj: ToYamlFileMixIn,
                           tmpdir: LocalPath,
                           expected_text: str,
                           compare_dict: bool = True,
                           compare_items: bool = True):
```

### Comparing `vise-0.7.0/vise/tests/helpers/test_assersion.py` & `vise-0.7.1/vise/tests/helpers/test_assersion.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/tests/input_set/datasets/test_dataset_util.py` & `vise-0.7.1/vise/tests/input_set/datasets/test_dataset_util.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/tests/input_set/datasets/test_potcar_set.py` & `vise-0.7.1/vise/tests/input_set/datasets/test_potcar_set.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/tests/input_set/test_incar.py` & `vise-0.7.1/vise/tests/input_set/test_incar.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,26 +17,31 @@
 
 
 def test_get_string():
     incar = ViseIncar.from_dict({"PREC": "Normal",
                                  "LREAL": False,
                                  "EDIFF": 1.0,
                                  "ISYM": 0,
-                                 "MAGMOM": [3, 3, 3]})
+                                 "MAGMOM": [3, 3, 3],
+                                 "PHON_NSTRUCT": 2})
+    print(incar)
     actual = incar.get_string()
     expected = """# accuracy
 PREC   =  Normal
 LREAL  =  False
 EDIFF  =  1.0
 
 # symmetry
 ISYM  =  0
 
 # spin
-MAGMOM  =  3 3 3"""
+MAGMOM  =  3 3 3
+
+# others
+PHON_NSTRUCT  =  2"""
     assert actual == expected
 
 
 def test_setting_to_str():
     incar = ViseIncar.from_dict({"EDIFF": 1.0,
                                  "MAGMOM": [3, 3, 3]})
     assert incar.setting_to_str("EDIFF") == str(1.0)
```

### Comparing `vise-0.7.0/vise/tests/input_set/test_incar_settings_generator.py` & `vise-0.7.1/vise/tests/input_set/test_incar_settings_generator.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/tests/input_set/test_input_options.py` & `vise-0.7.1/vise/tests/input_set/test_input_options.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/tests/input_set/test_kpoints_mode.py` & `vise-0.7.1/vise/tests/input_set/test_kpoints_mode.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/tests/input_set/test_potcar_generator.py` & `vise-0.7.1/vise/tests/input_set/test_potcar_generator.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/tests/input_set/test_prior_info.py` & `vise-0.7.1/vise/tests/input_set/test_prior_info.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/tests/input_set/test_structure_kpoints_generator.py` & `vise-0.7.1/vise/tests/input_set/test_structure_kpoints_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -219,8 +219,8 @@
     generator.generate_input()
 
     expected = Structure([[-1.591686, 1.591686, 1.591686],
                           [1.591686, -1.591686, 1.591686],
                           [1.591686, 1.591686, -1.591686]],
                          species=["H"], coords=[[0]*3])
     assert generator.structure == expected
-    assert generator.num_kpts == 104
+    assert generator.num_kpts == 100
```

### Comparing `vise-0.7.0/vise/tests/input_set/test_task.py` & `vise-0.7.1/vise/tests/input_set/test_task.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/tests/input_set/test_vasp_input_files.py` & `vise-0.7.1/vise/tests/input_set/test_vasp_input_files.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/tests/input_set/test_vise_log.py` & `vise-0.7.1/vise/tests/input_set/test_vise_log.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/tests/input_set/test_xc.py` & `vise-0.7.1/vise/tests/input_set/test_xc.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/tests/test_defaults.py` & `vise-0.7.1/vise/tests/test_defaults.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/tests/test_user_settings.py` & `vise-0.7.1/vise/tests/test_user_settings.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/tests/util/phonopy/test_phonopy_input.py` & `vise-0.7.1/vise/tests/util/phonopy/test_phonopy_input.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/tests/util/test_bravais_lattice.py` & `vise-0.7.1/vise/tests/util/test_bravais_lattice.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/tests/util/test_centering.py` & `vise-0.7.1/vise/tests/util/test_centering.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/tests/util/test_file_transfer.py` & `vise-0.7.1/vise/tests/util/test_file_transfer.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/tests/util/test_mix_in.py` & `vise-0.7.1/vise/tests/util/test_mix_in.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/tests/util/test_structure_symmetrizer.py` & `vise-0.7.1/vise/tests/util/test_structure_symmetrizer.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/user_settings.py` & `vise-0.7.1/vise/user_settings.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/util/Hermann-Mauguin.yaml` & `vise-0.7.1/vise/util/Hermann-Mauguin.yaml`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/util/bravais_lattice.py` & `vise-0.7.1/vise/util/bravais_lattice.py`

 * *Files 8% similar despite different names*

```diff
@@ -128,15 +128,40 @@
         else:
             raise ValueError
 
         return cls.from_string(bravais_letter)
 
     @property
     def kpt_centering(self) -> List[float]:
-        if self in [self.oF, self.tI, self.cF, self.cI]:
+        """
+        Note: cI does not require gamma centering.
+
+        KPOINTS:
+        test
+        0
+        Gamma
+        2 2 2
+
+        IBZKPT:
+- Gamma center
+Automatically generated mesh
+       3
+Reciprocal lattice
+    0.00000000000000    0.00000000000000    0.00000000000000             1
+    0.50000000000000    0.00000000000000   -0.00000000000000             6
+    0.50000000000000    0.50000000000000    0.50000000000000             1
+
+- Off centering
+Automatically generated mesh
+       2
+Reciprocal lattice
+    0.25000000000000    0.25000000000000    0.25000000000000             2
+   -0.25000000000000    0.25000000000000    0.25000000000000             6
+"""
+        if self in [self.oF, self.tI, self.cF]:
             return [0.0, 0.0, 0.0]
         elif self is self.hP:
             return [0.0, 0.0, 0.5]
         else:
             return [0.5, 0.5, 0.5]
 
     @property
```

### Comparing `vise-0.7.0/vise/util/centering.py` & `vise-0.7.1/vise/util/centering.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/util/enum.py` & `vise-0.7.1/vise/util/enum.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/util/file_transfer.py` & `vise-0.7.1/vise/util/file_transfer.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/util/logger.py` & `vise-0.7.1/vise/util/logger.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/util/matplotlib.py` & `vise-0.7.1/vise/util/matplotlib.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/util/mix_in.py` & `vise-0.7.1/vise/util/mix_in.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/util/phonopy/phonopy_input.py` & `vise-0.7.1/vise/util/phonopy/phonopy_input.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/util/plotly_util.py` & `vise-0.7.1/vise/util/plotly_util.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/util/str_related_tools.py` & `vise-0.7.1/vise/util/str_related_tools.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/util/string.py` & `vise-0.7.1/vise/util/string.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise/util/structure_symmetrizer.py` & `vise-0.7.1/vise/util/structure_symmetrizer.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.0/vise.egg-info/PKG-INFO` & `vise-0.7.1/vise.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vise
-Version: 0.7.0
+Version: 0.7.1
 Summary: Package for handling io of vasp package in kumagai group at IMR, Tohoku university
 Home-page: https://github.com/kumagai-group/vise
 Author: Yu Kumagai
 Author-email: yukumagai@tohoku.ac.jp
 License: MIT license
 Description: ![PyPI - License](https://img.shields.io/pypi/l/vise?color=blue)
         ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/vise)
```

### Comparing `vise-0.7.0/vise.egg-info/SOURCES.txt` & `vise-0.7.1/vise.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,14 @@
 vise/input_set/vasp_input_files.py
 vise/input_set/vise_log.py
 vise/input_set/xc.py
 vise/input_set/datasets/__init__.py
 vise/input_set/datasets/dataset_util.py
 vise/input_set/datasets/incar_flags.yaml
 vise/input_set/datasets/kpar_set.yaml
-vise/input_set/datasets/kpt_centering.py
 vise/input_set/datasets/magmom.yaml
 vise/input_set/datasets/potcar_set.py
 vise/input_set/datasets/potcar_set.yaml
 vise/input_set/datasets/u_parameter_set.yaml
 vise/input_set/datasets/unoccupied_bands.yaml
 vise/tests/__init__.py
 vise/tests/conftest.py
```

