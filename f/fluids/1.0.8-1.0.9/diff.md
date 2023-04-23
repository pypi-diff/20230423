# Comparing `tmp/fluids-1.0.8.tar.gz` & `tmp/fluids-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fluids-1.0.8.tar", last modified: Wed Jun  2 03:16:07 2021, max compression
+gzip compressed data, was "dist/fluids-1.0.9.tar", last modified: Thu Jun 17 02:08:27 2021, max compression
```

## Comparing `fluids-1.0.8.tar` & `fluids-1.0.9.tar`

### file list

```diff
@@ -1,432 +1,432 @@
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/fluids/
--rw-r--r--   0 caleb     (1000) caleb     (1000)     2417 2021-04-16 05:52:44.000000 fluids-1.0.8/fluids/typing_utils.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)   112045 2021-05-15 22:44:13.000000 fluids-1.0.8/fluids/flow_meter.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)    18040 2021-04-16 05:52:44.000000 fluids-1.0.8/fluids/saltation.py
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/fluids/numerics/
--rw-r--r--   0 caleb     (1000) caleb     (1000)     3862 2021-04-16 05:52:51.000000 fluids-1.0.8/fluids/numerics/special.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)    16944 2021-05-15 22:44:13.000000 fluids-1.0.8/fluids/numerics/arrays.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)   195006 2021-06-02 03:14:57.000000 fluids-1.0.8/fluids/numerics/__init__.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)     9555 2021-04-16 05:52:44.000000 fluids-1.0.8/fluids/numerics/doubledouble.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)    49249 2021-04-16 05:52:44.000000 fluids-1.0.8/fluids/drag.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)    11282 2021-04-16 05:52:44.000000 fluids-1.0.8/fluids/filters.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)    13529 2021-04-16 05:52:44.000000 fluids-1.0.8/fluids/mixing.py
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/fluids/data/
--rw-r--r--   0 caleb     (1000) caleb     (1000)     5042 2021-03-25 00:34:47.000000 fluids-1.0.8/fluids/data/ASTM E11 sieves.csv
--rw-r--r--   0 caleb     (1000) caleb     (1000)    14711 2021-03-25 00:34:47.000000 fluids-1.0.8/fluids/data/Miller 2E 1990 smooth bends Kb.csv
--rw-r--r--   0 caleb     (1000) caleb     (1000)  2225703 2021-03-25 00:34:47.000000 fluids-1.0.8/fluids/data/isd-history-cleaned.tsv
--rw-r--r--   0 caleb     (1000) caleb     (1000)     5333 2021-03-25 00:34:47.000000 fluids-1.0.8/fluids/data/ISO 3310-1 sieves.csv
--rw-r--r--   0 caleb     (1000) caleb     (1000)     5274 2021-03-25 00:34:47.000000 fluids-1.0.8/fluids/data/residential power.csv
--rw-r--r--   0 caleb     (1000) caleb     (1000)     6479 2021-03-25 00:34:47.000000 fluids-1.0.8/fluids/data/Miller 2E 1990 conical diffuser Kd.csv
--rw-r--r--   0 caleb     (1000) caleb     (1000)     1602 2021-03-25 00:34:47.000000 fluids-1.0.8/fluids/data/Miller 2E 1990 conical contractions K part 2.csv
--rw-r--r--   0 caleb     (1000) caleb     (1000)     3126 2021-03-25 00:34:47.000000 fluids-1.0.8/fluids/data/Miller 2E 1990 entrances rounded beveled K.csv
--rw-r--r--   0 caleb     (1000) caleb     (1000)     3022 2021-03-25 00:34:47.000000 fluids-1.0.8/fluids/data/Miller 2E 1990 abrupt contraction K.csv
--rw-r--r--   0 caleb     (1000) caleb     (1000)     4189 2021-03-25 00:34:47.000000 fluids-1.0.8/fluids/data/3 phase power.csv
--rw-r--r--   0 caleb     (1000) caleb     (1000)     3219 2021-03-25 00:34:47.000000 fluids-1.0.8/fluids/data/Miller 2E 1990 conical contractions K part 1.csv
--rw-r--r--   0 caleb     (1000) caleb     (1000)     1280 2021-03-25 00:34:47.000000 fluids-1.0.8/fluids/data/Miller 2E 1990 Kb mitre bend.csv
--rw-r--r--   0 caleb     (1000) caleb     (1000)     4671 2021-03-25 00:34:47.000000 fluids-1.0.8/fluids/data/Miller 2E 1990 smooth bends outlet tangent length correction.csv
--rw-r--r--   0 caleb     (1000) caleb     (1000)     5228 2021-03-25 00:34:47.000000 fluids-1.0.8/fluids/data/Miller 2E 1990 smooth bends Re correction.csv
--rw-r--r--   0 caleb     (1000) caleb     (1000)    94589 2021-04-16 05:52:44.000000 fluids-1.0.8/fluids/two_phase_voidage.py
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/fluids/optional/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    16938 2021-03-25 00:34:47.000000 fluids-1.0.8/fluids/optional/hwm93.pyf
--rw-r--r--   0 caleb     (1000) caleb     (1000)     7675 2021-03-25 00:34:47.000000 fluids-1.0.8/fluids/optional/irradiance.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)    26906 2021-04-16 05:52:44.000000 fluids-1.0.8/fluids/optional/pychebfun.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)     4848 2021-03-25 00:34:47.000000 fluids-1.0.8/fluids/optional/dwm07b104i.dat
--rw-r--r--   0 caleb     (1000) caleb     (1000)   193608 2021-03-25 00:34:47.000000 fluids-1.0.8/fluids/optional/hwm123114.bin
--rw-r--r--   0 caleb     (1000) caleb     (1000)    49589 2021-04-16 05:52:44.000000 fluids-1.0.8/fluids/optional/spa.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)    11324 2021-03-25 00:34:47.000000 fluids-1.0.8/fluids/optional/hwm14.pyf
--rw-r--r--   0 caleb     (1000) caleb     (1000)        1 2021-03-25 00:34:47.000000 fluids-1.0.8/fluids/optional/__init__.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)   128715 2021-04-16 05:52:44.000000 fluids-1.0.8/fluids/optional/hwm93.for
--rw-r--r--   0 caleb     (1000) caleb     (1000)     1500 2021-03-25 00:34:47.000000 fluids-1.0.8/fluids/optional/gd2qd.dat
--rw-r--r--   0 caleb     (1000) caleb     (1000)    45278 2021-04-16 05:52:44.000000 fluids-1.0.8/fluids/optional/hwm14.f90
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/fluids/constants/
--rw-r--r--   0 caleb     (1000) caleb     (1000)     4007 2021-04-16 05:52:44.000000 fluids-1.0.8/fluids/constants/constants.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)     1219 2021-03-25 00:34:47.000000 fluids-1.0.8/fluids/constants/__init__.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)   118261 2021-04-16 05:52:44.000000 fluids-1.0.8/fluids/particle_size_distribution.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)    13428 2021-04-16 05:52:44.000000 fluids-1.0.8/fluids/separator.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)    60066 2021-05-15 22:44:13.000000 fluids-1.0.8/fluids/control_valve.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)     1697 2021-03-25 00:34:47.000000 fluids-1.0.8/fluids/numba_vectorized.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)   191227 2021-04-16 05:52:44.000000 fluids-1.0.8/fluids/geometry.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)    78285 2021-04-16 05:52:44.000000 fluids-1.0.8/fluids/core.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)    64944 2021-04-16 05:52:44.000000 fluids-1.0.8/fluids/piping.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)    68255 2021-04-16 05:52:44.000000 fluids-1.0.8/fluids/pump.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)    26242 2021-06-02 03:14:57.000000 fluids-1.0.8/fluids/units.py
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/fluids/nrlmsise00/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    49353 2021-03-25 00:34:47.000000 fluids-1.0.8/fluids/nrlmsise00/nrlmsise_00_data.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)      492 2021-03-25 00:34:47.000000 fluids-1.0.8/fluids/nrlmsise00/README
--rw-r--r--   0 caleb     (1000) caleb     (1000)     8830 2021-04-16 05:52:44.000000 fluids-1.0.8/fluids/nrlmsise00/nrlmsise_00_header.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)    51726 2021-04-16 05:52:44.000000 fluids-1.0.8/fluids/nrlmsise00/nrlmsise_00.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)     1101 2021-03-25 00:34:47.000000 fluids-1.0.8/fluids/nrlmsise00/LICENSE
--rw-r--r--   0 caleb     (1000) caleb     (1000)     1557 2021-03-25 00:34:47.000000 fluids-1.0.8/fluids/nrlmsise00/__init__.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)    76351 2021-04-16 05:52:44.000000 fluids-1.0.8/fluids/compressible.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)    22965 2021-04-16 05:52:44.000000 fluids-1.0.8/fluids/safety_valve.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)    44037 2021-04-16 05:52:44.000000 fluids-1.0.8/fluids/packed_bed.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50613 2021-04-16 05:52:44.000000 fluids-1.0.8/fluids/atmosphere.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)   108611 2021-04-16 05:52:44.000000 fluids-1.0.8/fluids/two_phase.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)    22292 2021-05-22 16:40:51.000000 fluids-1.0.8/fluids/jet_pump.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)     5797 2021-06-02 03:14:57.000000 fluids-1.0.8/fluids/__init__.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)   186646 2021-04-16 05:52:44.000000 fluids-1.0.8/fluids/fittings.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)    36698 2021-04-23 01:52:59.000000 fluids-1.0.8/fluids/design_climate.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)    26914 2021-04-16 05:52:44.000000 fluids-1.0.8/fluids/open_flow.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)    27172 2021-04-16 05:52:44.000000 fluids-1.0.8/fluids/packed_tower.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)     2785 2021-04-16 05:52:44.000000 fluids-1.0.8/fluids/vectorized.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)    28892 2021-06-02 03:14:57.000000 fluids-1.0.8/fluids/numba.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)   151898 2021-04-16 05:52:44.000000 fluids-1.0.8/fluids/friction.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)     8007 2021-06-02 03:16:07.000000 fluids-1.0.8/PKG-INFO
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/docs/
--rw-r--r--   0 caleb     (1000) caleb     (1000)      342 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/fluids.compressible.rst
--rw-r--r--   0 caleb     (1000) caleb     (1000)      279 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/fluids.piping.rst
--rw-r--r--   0 caleb     (1000) caleb     (1000)      377 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/fluids.drag.rst
--rw-r--r--   0 caleb     (1000) caleb     (1000)      162 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/fluids.mixing.rst
--rw-r--r--   0 caleb     (1000) caleb     (1000)      289 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/fluids.filters.rst
--rw-r--r--   0 caleb     (1000) caleb     (1000)     6201 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/fluids.numba.rst
--rw-r--r--   0 caleb     (1000) caleb     (1000)      308 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/fluids.fittings.rst
--rw-r--r--   0 caleb     (1000) caleb     (1000)      263 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/fluids.jet_pump.rst
--rw-r--r--   0 caleb     (1000) caleb     (1000)      207 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/fluids.separator.rst
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/docs/fittings/
--rw-r--r--   0 caleb     (1000) caleb     (1000)     9244 2020-12-29 16:52:12.000000 fluids-1.0.8/docs/fittings/flush_mounted_rounded_entrance.png
--rw-r--r--   0 caleb     (1000) caleb     (1000)    34889 2020-12-29 16:52:12.000000 fluids-1.0.8/docs/fittings/contraction_sharp.png
--rw-r--r--   0 caleb     (1000) caleb     (1000)    11753 2020-12-29 16:52:12.000000 fluids-1.0.8/docs/fittings/diffuser_conical.png
--rw-r--r--   0 caleb     (1000) caleb     (1000)    14568 2020-12-29 16:52:12.000000 fluids-1.0.8/docs/fittings/flush_mounted_beveled_entrance.png
--rw-r--r--   0 caleb     (1000) caleb     (1000)    23375 2020-12-29 16:52:12.000000 fluids-1.0.8/docs/fittings/entrance_mounted_at_an_angle.png
--rw-r--r--   0 caleb     (1000) caleb     (1000)    23817 2020-12-29 16:52:12.000000 fluids-1.0.8/docs/fittings/contraction_round.png
--rw-r--r--   0 caleb     (1000) caleb     (1000)    11213 2020-12-29 16:52:12.000000 fluids-1.0.8/docs/fittings/sharp_edged_entrace_extended_mount.png
--rw-r--r--   0 caleb     (1000) caleb     (1000)    15004 2020-12-29 16:52:12.000000 fluids-1.0.8/docs/fittings/flush_mounted_beveled_orifice_entrance.png
--rw-r--r--   0 caleb     (1000) caleb     (1000)    21218 2020-12-29 16:52:12.000000 fluids-1.0.8/docs/fittings/contraction_beveled.png
--rw-r--r--   0 caleb     (1000) caleb     (1000)     6808 2020-12-29 16:52:12.000000 fluids-1.0.8/docs/fittings/flush_mounted_sharp_edged_entrance.png
--rw-r--r--   0 caleb     (1000) caleb     (1000)    33757 2020-12-29 16:52:12.000000 fluids-1.0.8/docs/fittings/bend_rounded.png
--rw-r--r--   0 caleb     (1000) caleb     (1000)    35629 2020-12-29 16:52:12.000000 fluids-1.0.8/docs/fittings/curved_wall_diffuser.png
--rw-r--r--   0 caleb     (1000) caleb     (1000)    25762 2020-12-29 16:52:12.000000 fluids-1.0.8/docs/fittings/bend_miter.png
--rw-r--r--   0 caleb     (1000) caleb     (1000)     4892 2020-12-29 16:52:12.000000 fluids-1.0.8/docs/fittings/flush_mounted_exit.png
--rw-r--r--   0 caleb     (1000) caleb     (1000)    26546 2020-12-29 16:52:12.000000 fluids-1.0.8/docs/fittings/contraction_conical.png
--rw-r--r--   0 caleb     (1000) caleb     (1000)     3883 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/fluids.units.rst
--rw-r--r--   0 caleb     (1000) caleb     (1000)      265 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/fluids.open_flow.rst
--rw-r--r--   0 caleb     (1000) caleb     (1000)      293 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/fluids.core.rst
--rw-r--r--   0 caleb     (1000) caleb     (1000)     2125 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/fluids.vectorized.rst
--rw-r--r--   0 caleb     (1000) caleb     (1000)      176 2020-12-29 16:52:12.000000 fluids-1.0.8/docs/data.rst
--rw-r--r--   0 caleb     (1000) caleb     (1000)      244 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/fluids.geometry.rst
--rw-r--r--   0 caleb     (1000) caleb     (1000)      253 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/fluids.two_phase_voidage.rst
--rw-r--r--   0 caleb     (1000) caleb     (1000)       67 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/robots.txt
--rw-r--r--   0 caleb     (1000) caleb     (1000)      303 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/fluids.control_valve.rst
--rw-r--r--   0 caleb     (1000) caleb     (1000)      261 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/fluids.friction.rst
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/docs/plots/
--rw-r--r--   0 caleb     (1000) caleb     (1000)      490 2020-12-29 16:52:12.000000 fluids-1.0.8/docs/plots/entrance_rounded_plot.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)      734 2020-12-29 16:52:12.000000 fluids-1.0.8/docs/plots/entrance_beveled_plot.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)     1259 2020-12-29 16:52:12.000000 fluids-1.0.8/docs/plots/ft_Crane_plot.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)      850 2020-12-29 16:52:12.000000 fluids-1.0.8/docs/plots/bend_rounded_Crane_plot.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)     1481 2020-12-29 16:52:12.000000 fluids-1.0.8/docs/plots/diffuser_conical_plot.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)      457 2020-12-29 16:52:12.000000 fluids-1.0.8/docs/plots/entrance_distance_plot.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)     1275 2020-12-29 16:52:12.000000 fluids-1.0.8/docs/plots/bend_miter_plot.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)     1411 2020-12-29 16:52:12.000000 fluids-1.0.8/docs/plots/contraction_conical_plot.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)      768 2020-12-29 16:52:12.000000 fluids-1.0.8/docs/plots/contraction_round_plot.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)      395 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/fluids.flow_meter.rst
--rw-r--r--   0 caleb     (1000) caleb     (1000)       69 2020-12-29 16:52:12.000000 fluids-1.0.8/docs/modules.rst
--rw-r--r--   0 caleb     (1000) caleb     (1000)      228 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/fluids.saltation.rst
--rw-r--r--   0 caleb     (1000) caleb     (1000)    11113 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/conf.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)      541 2020-12-29 16:52:12.000000 fluids-1.0.8/docs/fluids.rst
--rw-r--r--   0 caleb     (1000) caleb     (1000)      227 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/fluids.safety_valve.rst
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/docs/_static/
--rw-r--r--   0 caleb     (1000) caleb     (1000)     2769 2020-12-29 16:52:12.000000 fluids-1.0.8/docs/_static/copybutton.js
--rw-r--r--   0 caleb     (1000) caleb     (1000)      249 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/fluids.packed_bed.rst
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/docs/Data/
--rw-r--r--   0 caleb     (1000) caleb     (1000)   498338 2020-12-29 16:52:12.000000 fluids-1.0.8/docs/Data/Pipe Schedules.ipynb
--rw-r--r--   0 caleb     (1000) caleb     (1000)   107873 2020-12-29 16:52:12.000000 fluids-1.0.8/docs/Data/Sieve Sizes for Particle Size Distributions.ipynb
--rw-r--r--   0 caleb     (1000) caleb     (1000)    18627 2020-12-29 16:52:12.000000 fluids-1.0.8/docs/Data/Friction.ipynb
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/docs/Examples/
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/
--rw-r--r--   0 caleb     (1000) caleb     (1000)     4316 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.14 Bernoulli's Theorem-Water.ipynb
--rw-r--r--   0 caleb     (1000) caleb     (1000)     3394 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.21 Gases at Sonic Velocity.ipynb
--rw-r--r--   0 caleb     (1000) caleb     (1000)     2932 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.11 Flat heating Coils - Water.ipynb
--rw-r--r--   0 caleb     (1000) caleb     (1000)     3696 2020-12-29 16:52:12.000000 fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.22 Compressible Fluids at Subsonic Velocity.ipynb
--rw-r--r--   0 caleb     (1000) caleb     (1000)     2785 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.27 Sizing Control Valves for Liquid Service.ipynb
--rw-r--r--   0 caleb     (1000) caleb     (1000)     3715 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.19 Water.ipynb
--rw-r--r--   0 caleb     (1000) caleb     (1000)     2198 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.8 Laminar flow in Valves, Fittings, and Pipe - SAE oil through a pipe and globe valve.ipynb
--rw-r--r--   0 caleb     (1000) caleb     (1000)     4787 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.7 Laminar flow in Valves, Fittings, and Pipe - System from Example 7.6.ipynb
--rw-r--r--   0 caleb     (1000) caleb     (1000)     1895 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.2 L, L over D and K from Kv for Conventional Type Valves.ipynb
--rw-r--r--   0 caleb     (1000) caleb     (1000)     3322 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.26 Pipe Partially Filled with Flowing Water.ipynb
--rw-r--r--   0 caleb     (1000) caleb     (1000)     2970 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.35 Hydraulic Resistance of a Converging Tee.ipynb
--rw-r--r--   0 caleb     (1000) caleb     (1000)     2455 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.4 Venturi Type Valves.ipynb
--rw-r--r--   0 caleb     (1000) caleb     (1000)     3548 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.29 Orifice Flow Rate Calculation.ipynb
--rw-r--r--   0 caleb     (1000) caleb     (1000)     3240 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.23 Flow Through Orifice Meters.ipynb
--rw-r--r--   0 caleb     (1000) caleb     (1000)     3043 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.5 Lift Check Valves.ipynb
--rw-r--r--   0 caleb     (1000) caleb     (1000)     3226 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.20 Steam at Sonic Velocity.ipynb
--rw-r--r--   0 caleb     (1000) caleb     (1000)     2503 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.32 NPSH Available Calculation.ipynb
--rw-r--r--   0 caleb     (1000) caleb     (1000)     2528 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.17 Sizing of Pump for Oil Pipelines.ipynb
--rw-r--r--   0 caleb     (1000) caleb     (1000)     2179 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.34 Pump Power and Operating Cost.ipynb
--rw-r--r--   0 caleb     (1000) caleb     (1000)     5510 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.18 Gas.ipynb
--rw-r--r--   0 caleb     (1000) caleb     (1000)     2216 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.28 Checking for Choked Flow Conditions in a Control Valve.ipynb
--rw-r--r--   0 caleb     (1000) caleb     (1000)     6337 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.10 Piping Systems - Steam.ipynb
--rw-r--r--   0 caleb     (1000) caleb     (1000)     2553 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.15 Power Required for Pumping.ipynb
--rw-r--r--   0 caleb     (1000) caleb     (1000)     3921 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.16 Air Lines.ipynb
--rw-r--r--   0 caleb     (1000) caleb     (1000)     4423 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.30 Nozzle Sizing Calculations.ipynb
--rw-r--r--   0 caleb     (1000) caleb     (1000)     4313 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.6 Reduced Port Ball Valve.ipynb
--rw-r--r--   0 caleb     (1000) caleb     (1000)     4791 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.12 Orifice Size for Given Pressure Drop and Velocity.ipynb
--rw-r--r--   0 caleb     (1000) caleb     (1000)     5013 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.9 Laminar Flow in Valves, Fittings, and Pipe.ipynb
--rw-r--r--   0 caleb     (1000) caleb     (1000)     3701 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.25 Rectangular Duct - Application of Hydraulic Radius to Flow Problems.ipynb
--rw-r--r--   0 caleb     (1000) caleb     (1000)     1979 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.1 Smooth Pipe (Plastic).ipynb
--rw-r--r--   0 caleb     (1000) caleb     (1000)     3060 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.13 Flow given in English Units - Oil.ipynb
--rw-r--r--   0 caleb     (1000) caleb     (1000)     3051 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.36 Hydraulic Resistance of a Diverging Wye.ipynb
--rw-r--r--   0 caleb     (1000) caleb     (1000)     4984 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.24 Laminar Flow.ipynb
--rw-r--r--   0 caleb     (1000) caleb     (1000)     2150 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.3 L, L over D, K, and Kv for Conventional Type Valves.ipynb
--rw-r--r--   0 caleb     (1000) caleb     (1000)     1827 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.33 Pump Affinity Rules.ipynb
--rw-r--r--   0 caleb     (1000) caleb     (1000)      181 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/fluids.two_phase.rst
--rw-r--r--   0 caleb     (1000) caleb     (1000)    65664 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/tutorial.rst
--rw-r--r--   0 caleb     (1000) caleb     (1000)      179 2020-12-29 16:52:12.000000 fluids-1.0.8/docs/fluids.particle_size_distribution.rst
--rw-r--r--   0 caleb     (1000) caleb     (1000)      238 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/fluids.atmosphere.rst
--rw-r--r--   0 caleb     (1000) caleb     (1000)     3883 2020-12-29 16:52:12.000000 fluids-1.0.8/docs/examples.rst
--rw-r--r--   0 caleb     (1000) caleb     (1000)    16335 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/developers.rst
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/docs/_templates/
--rw-r--r--   0 caleb     (1000) caleb     (1000)      204 2020-12-29 16:52:12.000000 fluids-1.0.8/docs/_templates/layout.html
--rw-r--r--   0 caleb     (1000) caleb     (1000)     3819 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/index.rst
--rw-r--r--   0 caleb     (1000) caleb     (1000)      289 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/fluids.packed_tower.rst
--rw-r--r--   0 caleb     (1000) caleb     (1000)      195 2021-04-16 05:52:44.000000 fluids-1.0.8/docs/fluids.pump.rst
--rw-r--r--   0 caleb     (1000) caleb     (1000)       76 2020-12-29 16:52:12.000000 fluids-1.0.8/AUTHORS
--rw-r--r--   0 caleb     (1000) caleb     (1000)      672 2021-04-16 05:52:44.000000 fluids-1.0.8/pytest.ini
--rw-r--r--   0 caleb     (1000) caleb     (1000)       38 2021-06-02 03:16:07.000000 fluids-1.0.8/setup.cfg
--rw-r--r--   0 caleb     (1000) caleb     (1000)     3936 2021-06-02 03:14:57.000000 fluids-1.0.8/setup.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)      514 2020-12-29 16:52:12.000000 fluids-1.0.8/MANIFEST.in
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    10555 2021-04-16 05:52:44.000000 fluids-1.0.8/tests/test_jet_pump.py
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1989/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1989/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1957/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1957/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1971/
--rw-r--r--   0 caleb     (1000) caleb     (1000)        9 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1971/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1988/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    51013 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1988/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1952/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    51013 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1952/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/2013/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/2013/724050-13743.op
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/2013/722324-03071.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1978/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1978/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1951/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1951/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1959/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1959/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1999/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1999/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1969/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    23908 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1969/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1986/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1986/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1945/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1945/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1991/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1991/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1972/
--rw-r--r--   0 caleb     (1000) caleb     (1000)        9 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1972/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/2009/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/2009/724050-13743.op
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/2009/722324-03071.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/2003/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/2003/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1994/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1994/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1980/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    51013 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1980/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/2019/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/2019/724050-13743.op
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/2019/722324-03071.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1944/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    51013 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1944/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1995/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1995/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1984/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    51013 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1984/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1958/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1958/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1942/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1942/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1941/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1941/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1955/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1955/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1961/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1961/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/2017/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/2017/724050-13743.op
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/2017/722324-03071.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1992/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    51013 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1992/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1950/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1950/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1993/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1993/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1938/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1938/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1966/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    36140 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1966/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1987/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1987/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1983/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1983/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/2011/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/2011/724050-13743.op
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50735 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/2011/722324-03071.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1981/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1981/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/2018/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/2018/724050-13743.op
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/2018/722324-03071.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/2016/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    51013 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/2016/724050-13743.op
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50179 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/2016/722324-03071.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1940/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    51013 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1940/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1962/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1962/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1936/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    17097 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1936/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1973/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50735 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1973/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1998/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1998/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1967/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    35167 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1967/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1997/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1997/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1946/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    34333 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1946/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/2006/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/2006/724050-13743.op
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/2006/722324-03071.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1990/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1990/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1943/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1943/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1985/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1985/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1954/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1954/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1977/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1977/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/2002/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/2002/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1964/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    51013 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1964/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/2008/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    51013 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/2008/724050-13743.op
--rw-r--r--   0 caleb     (1000) caleb     (1000)    51013 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/2008/722324-03071.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1965/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1965/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1949/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1949/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1963/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1963/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/2004/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    51013 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/2004/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/2012/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    51013 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/2012/724050-13743.op
--rw-r--r--   0 caleb     (1000) caleb     (1000)    51013 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/2012/722324-03071.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1976/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    51013 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1976/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/2007/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/2007/724050-13743.op
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/2007/722324-03071.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/2014/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/2014/724050-13743.op
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50040 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/2014/722324-03071.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1975/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50735 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1975/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1974/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1974/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1979/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1979/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/2000/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    51013 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/2000/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1960/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    51013 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1960/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/2015/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/2015/724050-13743.op
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/2015/722324-03071.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1937/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1937/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1953/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1953/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/2005/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/2005/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/2001/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/2001/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1947/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1947/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1982/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1982/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1996/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    51013 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1996/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1948/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    51013 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1948/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/2010/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/2010/724050-13743.op
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/2010/722324-03071.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/2020/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    51013 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/2020/724050-13743.op
--rw-r--r--   0 caleb     (1000) caleb     (1000)    51013 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/2020/722324-03071.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1968/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    35445 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1968/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1970/
--rw-r--r--   0 caleb     (1000) caleb     (1000)        9 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1970/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1939/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1939/724050-13743.op
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/gsod/1956/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    51013 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/gsod/1956/724050-13743.op
--rw-r--r--   0 caleb     (1000) caleb     (1000)     2789 2021-06-02 03:14:57.000000 fluids-1.0.8/tests/test_filters.py
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/spa/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    19177 2021-04-16 05:52:44.000000 fluids-1.0.8/tests/spa/test_spa.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)    32807 2021-06-02 03:14:57.000000 fluids-1.0.8/tests/test_particle_size_distribution.py
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/particle_size_distribution/
--rw-r--r--   0 caleb     (1000) caleb     (1000)   213450 2020-12-29 16:52:12.000000 fluids-1.0.8/tests/particle_size_distribution/unsoda_distributions_20140206.csv
--rw-r--r--   0 caleb     (1000) caleb     (1000)    17588 2021-06-02 03:14:57.000000 fluids-1.0.8/tests/test_control_valve.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)     8180 2021-06-02 03:14:57.000000 fluids-1.0.8/tests/test_drag.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)     4237 2021-04-16 05:52:44.000000 fluids-1.0.8/tests/test_nrlmsise00_full.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)    30952 2021-06-02 03:14:57.000000 fluids-1.0.8/tests/test_fittings.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)     2626 2021-06-02 03:14:57.000000 fluids-1.0.8/tests/manual_runner.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)    22261 2021-04-16 05:52:44.000000 fluids-1.0.8/tests/test_fittings_fits.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)     9215 2021-04-16 05:52:44.000000 fluids-1.0.8/tests/test_nrlmsise00_file_output.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)    16157 2021-04-16 05:52:44.000000 fluids-1.0.8/tests/test_atmosphere.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)     6365 2021-04-16 05:52:44.000000 fluids-1.0.8/tests/test_numerics_special.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)     8921 2021-06-02 03:14:57.000000 fluids-1.0.8/tests/test_two_phase_voidage.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)    12866 2021-06-02 03:14:57.000000 fluids-1.0.8/tests/test_compressible.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)     3855 2021-06-02 03:14:57.000000 fluids-1.0.8/tests/test_packed_tower.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)    20096 2021-06-02 03:14:57.000000 fluids-1.0.8/tests/test_friction.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)     1397 2020-12-29 16:52:12.000000 fluids-1.0.8/tests/make_test_stubs.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)    55155 2021-04-23 01:52:59.000000 fluids-1.0.8/tests/test_design_climate.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)    59966 2021-04-16 05:52:44.000000 fluids-1.0.8/tests/test_geometry.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)    32492 2021-04-16 05:52:44.000000 fluids-1.0.8/tests/test_numba.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)     7385 2021-06-02 03:14:57.000000 fluids-1.0.8/tests/test_piping.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)     9777 2021-04-16 05:52:44.000000 fluids-1.0.8/tests/test_numerics_doubledouble.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)     5478 2021-06-02 03:14:57.000000 fluids-1.0.8/tests/test_separator.py
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/tests/nrlmsise00/
--rw-r--r--   0 caleb     (1000) caleb     (1000)     2327 2020-12-29 16:52:12.000000 fluids-1.0.8/tests/nrlmsise00/known_data_hours.txt
--rw-r--r--   0 caleb     (1000) caleb     (1000)    17556 2020-12-29 16:52:12.000000 fluids-1.0.8/tests/nrlmsise00/known_data_latitudes.txt
--rw-r--r--   0 caleb     (1000) caleb     (1000)    95803 2020-12-29 16:52:12.000000 fluids-1.0.8/tests/nrlmsise00/known_data_height.txt
--rw-r--r--   0 caleb     (1000) caleb     (1000)    35016 2020-12-29 16:52:12.000000 fluids-1.0.8/tests/nrlmsise00/known_data_longitudes.txt
--rw-r--r--   0 caleb     (1000) caleb     (1000)    35501 2020-12-29 16:52:12.000000 fluids-1.0.8/tests/nrlmsise00/known_data_day_of_year.txt
--rw-r--r--   0 caleb     (1000) caleb     (1000)    86520 2020-12-29 16:52:12.000000 fluids-1.0.8/tests/nrlmsise00/known_data_high_height.txt
--rw-r--r--   0 caleb     (1000) caleb     (1000)     6299 2020-12-29 16:52:12.000000 fluids-1.0.8/tests/nrlmsise00/data_from_C_version.txt
--rw-r--r--   0 caleb     (1000) caleb     (1000)     1193 2020-12-29 16:52:12.000000 fluids-1.0.8/tests/nrlmsise00/__init__.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)     9439 2021-06-02 03:14:57.000000 fluids-1.0.8/tests/test_core.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)    32260 2021-06-02 03:14:57.000000 fluids-1.0.8/tests/test_numerics.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)    18338 2021-06-02 03:14:57.000000 fluids-1.0.8/tests/test_units.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)     2033 2021-04-16 05:52:44.000000 fluids-1.0.8/tests/test_vectorized.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)     2897 2021-06-02 03:14:57.000000 fluids-1.0.8/tests/test_open_flow.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)     2500 2021-04-16 05:52:44.000000 fluids-1.0.8/tests/test_utils.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)    26245 2021-06-02 03:14:57.000000 fluids-1.0.8/tests/test_two_phase.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)    47234 2021-06-02 03:14:57.000000 fluids-1.0.8/tests/test_flow_meter.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)     1193 2020-12-29 16:52:12.000000 fluids-1.0.8/tests/__init__.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)     2323 2021-06-02 03:14:57.000000 fluids-1.0.8/tests/test_mixing.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)     8016 2021-06-02 03:14:57.000000 fluids-1.0.8/tests/test_pump.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)     5156 2021-06-02 03:14:57.000000 fluids-1.0.8/tests/test_packed_bed.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)     3295 2021-06-02 03:14:57.000000 fluids-1.0.8/tests/test_safety_valve.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)     2545 2021-06-02 03:14:57.000000 fluids-1.0.8/tests/test_saltation.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)     1090 2021-04-16 05:52:44.000000 fluids-1.0.8/LICENSE.txt
--rw-r--r--   0 caleb     (1000) caleb     (1000)     4595 2021-04-16 05:52:44.000000 fluids-1.0.8/README.rst
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-02 03:16:07.000000 fluids-1.0.8/fluids.egg-info/
--rw-r--r--   0 caleb     (1000) caleb     (1000)        7 2021-06-02 03:16:07.000000 fluids-1.0.8/fluids.egg-info/top_level.txt
--rw-r--r--   0 caleb     (1000) caleb     (1000)     8007 2021-06-02 03:16:07.000000 fluids-1.0.8/fluids.egg-info/PKG-INFO
--rw-r--r--   0 caleb     (1000) caleb     (1000)    11717 2021-06-02 03:16:07.000000 fluids-1.0.8/fluids.egg-info/SOURCES.txt
--rw-r--r--   0 caleb     (1000) caleb     (1000)        1 2021-06-02 03:16:07.000000 fluids-1.0.8/fluids.egg-info/dependency_links.txt
--rw-r--r--   0 caleb     (1000) caleb     (1000)       88 2021-06-02 03:16:07.000000 fluids-1.0.8/fluids.egg-info/requires.txt
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:26.000000 fluids-1.0.9/fluids/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     2417 2021-04-16 05:52:44.000000 fluids-1.0.9/fluids/typing_utils.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)   112045 2021-05-15 22:44:13.000000 fluids-1.0.9/fluids/flow_meter.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    18040 2021-04-16 05:52:44.000000 fluids-1.0.9/fluids/saltation.py
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/fluids/numerics/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     3862 2021-04-16 05:52:51.000000 fluids-1.0.9/fluids/numerics/special.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    16944 2021-05-15 22:44:13.000000 fluids-1.0.9/fluids/numerics/arrays.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)   195006 2021-06-02 03:14:57.000000 fluids-1.0.9/fluids/numerics/__init__.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     9555 2021-04-16 05:52:44.000000 fluids-1.0.9/fluids/numerics/doubledouble.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    49249 2021-04-16 05:52:44.000000 fluids-1.0.9/fluids/drag.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    11282 2021-04-16 05:52:44.000000 fluids-1.0.9/fluids/filters.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    13529 2021-04-16 05:52:44.000000 fluids-1.0.9/fluids/mixing.py
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/fluids/data/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     5042 2021-03-25 00:34:47.000000 fluids-1.0.9/fluids/data/ASTM E11 sieves.csv
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    14711 2021-03-25 00:34:47.000000 fluids-1.0.9/fluids/data/Miller 2E 1990 smooth bends Kb.csv
+-rw-r--r--   0 caleb     (1000) caleb     (1000)  2225703 2021-03-25 00:34:47.000000 fluids-1.0.9/fluids/data/isd-history-cleaned.tsv
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     5333 2021-03-25 00:34:47.000000 fluids-1.0.9/fluids/data/ISO 3310-1 sieves.csv
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     5274 2021-03-25 00:34:47.000000 fluids-1.0.9/fluids/data/residential power.csv
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     6479 2021-03-25 00:34:47.000000 fluids-1.0.9/fluids/data/Miller 2E 1990 conical diffuser Kd.csv
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     1602 2021-03-25 00:34:47.000000 fluids-1.0.9/fluids/data/Miller 2E 1990 conical contractions K part 2.csv
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     3126 2021-03-25 00:34:47.000000 fluids-1.0.9/fluids/data/Miller 2E 1990 entrances rounded beveled K.csv
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     3022 2021-03-25 00:34:47.000000 fluids-1.0.9/fluids/data/Miller 2E 1990 abrupt contraction K.csv
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     4189 2021-03-25 00:34:47.000000 fluids-1.0.9/fluids/data/3 phase power.csv
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     3219 2021-03-25 00:34:47.000000 fluids-1.0.9/fluids/data/Miller 2E 1990 conical contractions K part 1.csv
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     1280 2021-03-25 00:34:47.000000 fluids-1.0.9/fluids/data/Miller 2E 1990 Kb mitre bend.csv
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     4671 2021-03-25 00:34:47.000000 fluids-1.0.9/fluids/data/Miller 2E 1990 smooth bends outlet tangent length correction.csv
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     5228 2021-03-25 00:34:47.000000 fluids-1.0.9/fluids/data/Miller 2E 1990 smooth bends Re correction.csv
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    94589 2021-04-16 05:52:44.000000 fluids-1.0.9/fluids/two_phase_voidage.py
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/fluids/optional/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    16938 2021-03-25 00:34:47.000000 fluids-1.0.9/fluids/optional/hwm93.pyf
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     7675 2021-03-25 00:34:47.000000 fluids-1.0.9/fluids/optional/irradiance.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    26906 2021-04-16 05:52:44.000000 fluids-1.0.9/fluids/optional/pychebfun.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     4848 2021-03-25 00:34:47.000000 fluids-1.0.9/fluids/optional/dwm07b104i.dat
+-rw-r--r--   0 caleb     (1000) caleb     (1000)   193608 2021-03-25 00:34:47.000000 fluids-1.0.9/fluids/optional/hwm123114.bin
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    49589 2021-04-16 05:52:44.000000 fluids-1.0.9/fluids/optional/spa.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    11324 2021-03-25 00:34:47.000000 fluids-1.0.9/fluids/optional/hwm14.pyf
+-rw-r--r--   0 caleb     (1000) caleb     (1000)        1 2021-03-25 00:34:47.000000 fluids-1.0.9/fluids/optional/__init__.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)   128715 2021-04-16 05:52:44.000000 fluids-1.0.9/fluids/optional/hwm93.for
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     1500 2021-03-25 00:34:47.000000 fluids-1.0.9/fluids/optional/gd2qd.dat
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    45278 2021-04-16 05:52:44.000000 fluids-1.0.9/fluids/optional/hwm14.f90
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:26.000000 fluids-1.0.9/fluids/constants/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     4038 2021-06-17 02:07:09.000000 fluids-1.0.9/fluids/constants/constants.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     1219 2021-03-25 00:34:47.000000 fluids-1.0.9/fluids/constants/__init__.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)   118261 2021-04-16 05:52:44.000000 fluids-1.0.9/fluids/particle_size_distribution.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    13428 2021-04-16 05:52:44.000000 fluids-1.0.9/fluids/separator.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    60066 2021-05-15 22:44:13.000000 fluids-1.0.9/fluids/control_valve.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     1697 2021-03-25 00:34:47.000000 fluids-1.0.9/fluids/numba_vectorized.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)   191227 2021-04-16 05:52:44.000000 fluids-1.0.9/fluids/geometry.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    78285 2021-04-16 05:52:44.000000 fluids-1.0.9/fluids/core.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    64944 2021-04-16 05:52:44.000000 fluids-1.0.9/fluids/piping.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    68255 2021-04-16 05:52:44.000000 fluids-1.0.9/fluids/pump.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    26242 2021-06-02 03:14:57.000000 fluids-1.0.9/fluids/units.py
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/fluids/nrlmsise00/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    49353 2021-03-25 00:34:47.000000 fluids-1.0.9/fluids/nrlmsise00/nrlmsise_00_data.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)      492 2021-03-25 00:34:47.000000 fluids-1.0.9/fluids/nrlmsise00/README
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     8830 2021-04-16 05:52:44.000000 fluids-1.0.9/fluids/nrlmsise00/nrlmsise_00_header.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    51726 2021-04-16 05:52:44.000000 fluids-1.0.9/fluids/nrlmsise00/nrlmsise_00.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     1101 2021-03-25 00:34:47.000000 fluids-1.0.9/fluids/nrlmsise00/LICENSE
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     1557 2021-03-25 00:34:47.000000 fluids-1.0.9/fluids/nrlmsise00/__init__.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    76351 2021-04-16 05:52:44.000000 fluids-1.0.9/fluids/compressible.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    22965 2021-04-16 05:52:44.000000 fluids-1.0.9/fluids/safety_valve.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    44037 2021-04-16 05:52:44.000000 fluids-1.0.9/fluids/packed_bed.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50613 2021-04-16 05:52:44.000000 fluids-1.0.9/fluids/atmosphere.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)   108611 2021-04-16 05:52:44.000000 fluids-1.0.9/fluids/two_phase.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    22292 2021-05-22 16:40:51.000000 fluids-1.0.9/fluids/jet_pump.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     5797 2021-06-17 02:05:07.000000 fluids-1.0.9/fluids/__init__.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)   186646 2021-04-16 05:52:44.000000 fluids-1.0.9/fluids/fittings.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    36698 2021-04-23 01:52:59.000000 fluids-1.0.9/fluids/design_climate.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    26914 2021-04-16 05:52:44.000000 fluids-1.0.9/fluids/open_flow.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    27172 2021-04-16 05:52:44.000000 fluids-1.0.9/fluids/packed_tower.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     2785 2021-04-16 05:52:44.000000 fluids-1.0.9/fluids/vectorized.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    28892 2021-06-02 03:14:57.000000 fluids-1.0.9/fluids/numba.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)   151898 2021-04-16 05:52:44.000000 fluids-1.0.9/fluids/friction.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     8007 2021-06-17 02:08:27.000000 fluids-1.0.9/PKG-INFO
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:26.000000 fluids-1.0.9/docs/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)      342 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/fluids.compressible.rst
+-rw-r--r--   0 caleb     (1000) caleb     (1000)      279 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/fluids.piping.rst
+-rw-r--r--   0 caleb     (1000) caleb     (1000)      377 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/fluids.drag.rst
+-rw-r--r--   0 caleb     (1000) caleb     (1000)      162 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/fluids.mixing.rst
+-rw-r--r--   0 caleb     (1000) caleb     (1000)      289 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/fluids.filters.rst
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     6201 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/fluids.numba.rst
+-rw-r--r--   0 caleb     (1000) caleb     (1000)      308 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/fluids.fittings.rst
+-rw-r--r--   0 caleb     (1000) caleb     (1000)      263 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/fluids.jet_pump.rst
+-rw-r--r--   0 caleb     (1000) caleb     (1000)      207 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/fluids.separator.rst
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:26.000000 fluids-1.0.9/docs/fittings/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     9244 2020-12-29 16:52:12.000000 fluids-1.0.9/docs/fittings/flush_mounted_rounded_entrance.png
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    34889 2020-12-29 16:52:12.000000 fluids-1.0.9/docs/fittings/contraction_sharp.png
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    11753 2020-12-29 16:52:12.000000 fluids-1.0.9/docs/fittings/diffuser_conical.png
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    14568 2020-12-29 16:52:12.000000 fluids-1.0.9/docs/fittings/flush_mounted_beveled_entrance.png
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    23375 2020-12-29 16:52:12.000000 fluids-1.0.9/docs/fittings/entrance_mounted_at_an_angle.png
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    23817 2020-12-29 16:52:12.000000 fluids-1.0.9/docs/fittings/contraction_round.png
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    11213 2020-12-29 16:52:12.000000 fluids-1.0.9/docs/fittings/sharp_edged_entrace_extended_mount.png
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    15004 2020-12-29 16:52:12.000000 fluids-1.0.9/docs/fittings/flush_mounted_beveled_orifice_entrance.png
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    21218 2020-12-29 16:52:12.000000 fluids-1.0.9/docs/fittings/contraction_beveled.png
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     6808 2020-12-29 16:52:12.000000 fluids-1.0.9/docs/fittings/flush_mounted_sharp_edged_entrance.png
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    33757 2020-12-29 16:52:12.000000 fluids-1.0.9/docs/fittings/bend_rounded.png
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    35629 2020-12-29 16:52:12.000000 fluids-1.0.9/docs/fittings/curved_wall_diffuser.png
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    25762 2020-12-29 16:52:12.000000 fluids-1.0.9/docs/fittings/bend_miter.png
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     4892 2020-12-29 16:52:12.000000 fluids-1.0.9/docs/fittings/flush_mounted_exit.png
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    26546 2020-12-29 16:52:12.000000 fluids-1.0.9/docs/fittings/contraction_conical.png
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     3883 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/fluids.units.rst
+-rw-r--r--   0 caleb     (1000) caleb     (1000)      265 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/fluids.open_flow.rst
+-rw-r--r--   0 caleb     (1000) caleb     (1000)      293 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/fluids.core.rst
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     2125 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/fluids.vectorized.rst
+-rw-r--r--   0 caleb     (1000) caleb     (1000)      176 2020-12-29 16:52:12.000000 fluids-1.0.9/docs/data.rst
+-rw-r--r--   0 caleb     (1000) caleb     (1000)      244 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/fluids.geometry.rst
+-rw-r--r--   0 caleb     (1000) caleb     (1000)      253 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/fluids.two_phase_voidage.rst
+-rw-r--r--   0 caleb     (1000) caleb     (1000)       67 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/robots.txt
+-rw-r--r--   0 caleb     (1000) caleb     (1000)      303 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/fluids.control_valve.rst
+-rw-r--r--   0 caleb     (1000) caleb     (1000)      261 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/fluids.friction.rst
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:26.000000 fluids-1.0.9/docs/plots/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)      490 2020-12-29 16:52:12.000000 fluids-1.0.9/docs/plots/entrance_rounded_plot.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)      734 2020-12-29 16:52:12.000000 fluids-1.0.9/docs/plots/entrance_beveled_plot.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     1259 2020-12-29 16:52:12.000000 fluids-1.0.9/docs/plots/ft_Crane_plot.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)      850 2020-12-29 16:52:12.000000 fluids-1.0.9/docs/plots/bend_rounded_Crane_plot.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     1481 2020-12-29 16:52:12.000000 fluids-1.0.9/docs/plots/diffuser_conical_plot.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)      457 2020-12-29 16:52:12.000000 fluids-1.0.9/docs/plots/entrance_distance_plot.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     1275 2020-12-29 16:52:12.000000 fluids-1.0.9/docs/plots/bend_miter_plot.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     1411 2020-12-29 16:52:12.000000 fluids-1.0.9/docs/plots/contraction_conical_plot.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)      768 2020-12-29 16:52:12.000000 fluids-1.0.9/docs/plots/contraction_round_plot.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)      395 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/fluids.flow_meter.rst
+-rw-r--r--   0 caleb     (1000) caleb     (1000)       69 2020-12-29 16:52:12.000000 fluids-1.0.9/docs/modules.rst
+-rw-r--r--   0 caleb     (1000) caleb     (1000)      228 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/fluids.saltation.rst
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    11113 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/conf.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)      541 2020-12-29 16:52:12.000000 fluids-1.0.9/docs/fluids.rst
+-rw-r--r--   0 caleb     (1000) caleb     (1000)      227 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/fluids.safety_valve.rst
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:26.000000 fluids-1.0.9/docs/_static/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     2769 2020-12-29 16:52:12.000000 fluids-1.0.9/docs/_static/copybutton.js
+-rw-r--r--   0 caleb     (1000) caleb     (1000)      249 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/fluids.packed_bed.rst
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:26.000000 fluids-1.0.9/docs/Data/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)   498338 2020-12-29 16:52:12.000000 fluids-1.0.9/docs/Data/Pipe Schedules.ipynb
+-rw-r--r--   0 caleb     (1000) caleb     (1000)   107873 2020-12-29 16:52:12.000000 fluids-1.0.9/docs/Data/Sieve Sizes for Particle Size Distributions.ipynb
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    18627 2020-12-29 16:52:12.000000 fluids-1.0.9/docs/Data/Friction.ipynb
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:26.000000 fluids-1.0.9/docs/Examples/
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:26.000000 fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     4316 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.14 Bernoulli's Theorem-Water.ipynb
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     3394 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.21 Gases at Sonic Velocity.ipynb
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     2932 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.11 Flat heating Coils - Water.ipynb
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     3696 2020-12-29 16:52:12.000000 fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.22 Compressible Fluids at Subsonic Velocity.ipynb
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     2785 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.27 Sizing Control Valves for Liquid Service.ipynb
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     3715 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.19 Water.ipynb
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     2198 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.8 Laminar flow in Valves, Fittings, and Pipe - SAE oil through a pipe and globe valve.ipynb
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     4787 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.7 Laminar flow in Valves, Fittings, and Pipe - System from Example 7.6.ipynb
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     1895 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.2 L, L over D and K from Kv for Conventional Type Valves.ipynb
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     3322 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.26 Pipe Partially Filled with Flowing Water.ipynb
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     2970 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.35 Hydraulic Resistance of a Converging Tee.ipynb
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     2455 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.4 Venturi Type Valves.ipynb
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     3548 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.29 Orifice Flow Rate Calculation.ipynb
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     3240 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.23 Flow Through Orifice Meters.ipynb
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     3043 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.5 Lift Check Valves.ipynb
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     3226 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.20 Steam at Sonic Velocity.ipynb
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     2503 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.32 NPSH Available Calculation.ipynb
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     2528 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.17 Sizing of Pump for Oil Pipelines.ipynb
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     2179 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.34 Pump Power and Operating Cost.ipynb
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     5510 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.18 Gas.ipynb
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     2216 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.28 Checking for Choked Flow Conditions in a Control Valve.ipynb
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     6337 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.10 Piping Systems - Steam.ipynb
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     2553 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.15 Power Required for Pumping.ipynb
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     3921 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.16 Air Lines.ipynb
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     4423 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.30 Nozzle Sizing Calculations.ipynb
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     4313 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.6 Reduced Port Ball Valve.ipynb
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     4791 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.12 Orifice Size for Given Pressure Drop and Velocity.ipynb
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     5013 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.9 Laminar Flow in Valves, Fittings, and Pipe.ipynb
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     3701 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.25 Rectangular Duct - Application of Hydraulic Radius to Flow Problems.ipynb
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     1979 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.1 Smooth Pipe (Plastic).ipynb
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     3060 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.13 Flow given in English Units - Oil.ipynb
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     3051 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.36 Hydraulic Resistance of a Diverging Wye.ipynb
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     4984 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.24 Laminar Flow.ipynb
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     2150 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.3 L, L over D, K, and Kv for Conventional Type Valves.ipynb
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     1827 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.33 Pump Affinity Rules.ipynb
+-rw-r--r--   0 caleb     (1000) caleb     (1000)      181 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/fluids.two_phase.rst
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    65664 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/tutorial.rst
+-rw-r--r--   0 caleb     (1000) caleb     (1000)      179 2020-12-29 16:52:12.000000 fluids-1.0.9/docs/fluids.particle_size_distribution.rst
+-rw-r--r--   0 caleb     (1000) caleb     (1000)      238 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/fluids.atmosphere.rst
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     3883 2020-12-29 16:52:12.000000 fluids-1.0.9/docs/examples.rst
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    16335 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/developers.rst
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:26.000000 fluids-1.0.9/docs/_templates/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)      204 2020-12-29 16:52:12.000000 fluids-1.0.9/docs/_templates/layout.html
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     3819 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/index.rst
+-rw-r--r--   0 caleb     (1000) caleb     (1000)      289 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/fluids.packed_tower.rst
+-rw-r--r--   0 caleb     (1000) caleb     (1000)      195 2021-04-16 05:52:44.000000 fluids-1.0.9/docs/fluids.pump.rst
+-rw-r--r--   0 caleb     (1000) caleb     (1000)       76 2020-12-29 16:52:12.000000 fluids-1.0.9/AUTHORS
+-rw-r--r--   0 caleb     (1000) caleb     (1000)      672 2021-04-16 05:52:44.000000 fluids-1.0.9/pytest.ini
+-rw-r--r--   0 caleb     (1000) caleb     (1000)       38 2021-06-17 02:08:27.000000 fluids-1.0.9/setup.cfg
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     3936 2021-06-17 02:04:56.000000 fluids-1.0.9/setup.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)      514 2020-12-29 16:52:12.000000 fluids-1.0.9/MANIFEST.in
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    10555 2021-04-16 05:52:44.000000 fluids-1.0.9/tests/test_jet_pump.py
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:26.000000 fluids-1.0.9/tests/gsod/
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1989/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1989/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1957/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1957/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1971/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)        9 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1971/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1988/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    51013 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1988/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1952/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    51013 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1952/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/2013/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/2013/724050-13743.op
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/2013/722324-03071.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1978/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1978/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1951/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1951/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1959/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1959/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1999/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1999/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1969/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    23908 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1969/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1986/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1986/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1945/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1945/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1991/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1991/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1972/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)        9 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1972/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/2009/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/2009/724050-13743.op
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/2009/722324-03071.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/2003/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/2003/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1994/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1994/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1980/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    51013 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1980/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/2019/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/2019/724050-13743.op
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/2019/722324-03071.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1944/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    51013 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1944/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1995/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1995/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1984/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    51013 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1984/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1958/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1958/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1942/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1942/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1941/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1941/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1955/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1955/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1961/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1961/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/2017/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/2017/724050-13743.op
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/2017/722324-03071.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1992/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    51013 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1992/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1950/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1950/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1993/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1993/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1938/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1938/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1966/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    36140 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1966/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1987/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1987/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1983/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1983/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/2011/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/2011/724050-13743.op
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50735 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/2011/722324-03071.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1981/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1981/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/2018/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/2018/724050-13743.op
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/2018/722324-03071.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/2016/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    51013 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/2016/724050-13743.op
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50179 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/2016/722324-03071.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1940/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    51013 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1940/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1962/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1962/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1936/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    17097 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1936/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1973/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50735 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1973/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1998/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1998/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1967/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    35167 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1967/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1997/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1997/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1946/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    34333 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1946/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/2006/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/2006/724050-13743.op
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/2006/722324-03071.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1990/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1990/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1943/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1943/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1985/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1985/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1954/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1954/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1977/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1977/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/2002/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/2002/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1964/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    51013 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1964/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/2008/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    51013 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/2008/724050-13743.op
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    51013 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/2008/722324-03071.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1965/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1965/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1949/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1949/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1963/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1963/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/2004/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    51013 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/2004/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/2012/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    51013 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/2012/724050-13743.op
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    51013 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/2012/722324-03071.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1976/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    51013 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1976/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/2007/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/2007/724050-13743.op
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/2007/722324-03071.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/2014/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/2014/724050-13743.op
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50040 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/2014/722324-03071.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1975/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50735 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1975/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1974/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1974/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1979/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1979/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/2000/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    51013 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/2000/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1960/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    51013 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1960/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/2015/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/2015/724050-13743.op
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/2015/722324-03071.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1937/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1937/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1953/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1953/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/2005/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/2005/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/2001/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/2001/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1947/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1947/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1982/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1982/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1996/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    51013 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1996/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1948/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    51013 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1948/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/2010/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/2010/724050-13743.op
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/2010/722324-03071.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/2020/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    51013 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/2020/724050-13743.op
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    51013 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/2020/722324-03071.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1968/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    35445 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1968/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1970/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)        9 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1970/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1939/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    50874 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1939/724050-13743.op
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/gsod/1956/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    51013 2021-06-02 03:58:44.000000 fluids-1.0.9/tests/gsod/1956/724050-13743.op
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     2789 2021-06-02 03:14:57.000000 fluids-1.0.9/tests/test_filters.py
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/spa/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    19177 2021-04-16 05:52:44.000000 fluids-1.0.9/tests/spa/test_spa.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    32807 2021-06-02 03:14:57.000000 fluids-1.0.9/tests/test_particle_size_distribution.py
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/particle_size_distribution/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)   213450 2020-12-29 16:52:12.000000 fluids-1.0.9/tests/particle_size_distribution/unsoda_distributions_20140206.csv
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    17588 2021-06-02 03:14:57.000000 fluids-1.0.9/tests/test_control_valve.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     8180 2021-06-02 03:14:57.000000 fluids-1.0.9/tests/test_drag.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     4237 2021-04-16 05:52:44.000000 fluids-1.0.9/tests/test_nrlmsise00_full.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    30952 2021-06-02 03:14:57.000000 fluids-1.0.9/tests/test_fittings.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     2626 2021-06-02 03:14:57.000000 fluids-1.0.9/tests/manual_runner.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    22261 2021-04-16 05:52:44.000000 fluids-1.0.9/tests/test_fittings_fits.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     9215 2021-04-16 05:52:44.000000 fluids-1.0.9/tests/test_nrlmsise00_file_output.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    16157 2021-04-16 05:52:44.000000 fluids-1.0.9/tests/test_atmosphere.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     6365 2021-04-16 05:52:44.000000 fluids-1.0.9/tests/test_numerics_special.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     8921 2021-06-02 03:14:57.000000 fluids-1.0.9/tests/test_two_phase_voidage.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    12866 2021-06-02 03:14:57.000000 fluids-1.0.9/tests/test_compressible.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     3855 2021-06-02 03:14:57.000000 fluids-1.0.9/tests/test_packed_tower.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    20096 2021-06-02 03:14:57.000000 fluids-1.0.9/tests/test_friction.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     1397 2020-12-29 16:52:12.000000 fluids-1.0.9/tests/make_test_stubs.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    55155 2021-04-23 01:52:59.000000 fluids-1.0.9/tests/test_design_climate.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    59966 2021-04-16 05:52:44.000000 fluids-1.0.9/tests/test_geometry.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    32492 2021-04-16 05:52:44.000000 fluids-1.0.9/tests/test_numba.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     7385 2021-06-02 03:14:57.000000 fluids-1.0.9/tests/test_piping.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     9777 2021-04-16 05:52:44.000000 fluids-1.0.9/tests/test_numerics_doubledouble.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     5478 2021-06-02 03:14:57.000000 fluids-1.0.9/tests/test_separator.py
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:27.000000 fluids-1.0.9/tests/nrlmsise00/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     2327 2020-12-29 16:52:12.000000 fluids-1.0.9/tests/nrlmsise00/known_data_hours.txt
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    17556 2020-12-29 16:52:12.000000 fluids-1.0.9/tests/nrlmsise00/known_data_latitudes.txt
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    95803 2020-12-29 16:52:12.000000 fluids-1.0.9/tests/nrlmsise00/known_data_height.txt
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    35016 2020-12-29 16:52:12.000000 fluids-1.0.9/tests/nrlmsise00/known_data_longitudes.txt
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    35501 2020-12-29 16:52:12.000000 fluids-1.0.9/tests/nrlmsise00/known_data_day_of_year.txt
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    86520 2020-12-29 16:52:12.000000 fluids-1.0.9/tests/nrlmsise00/known_data_high_height.txt
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     6299 2020-12-29 16:52:12.000000 fluids-1.0.9/tests/nrlmsise00/data_from_C_version.txt
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     1193 2020-12-29 16:52:12.000000 fluids-1.0.9/tests/nrlmsise00/__init__.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     9439 2021-06-02 03:14:57.000000 fluids-1.0.9/tests/test_core.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    32260 2021-06-02 03:14:57.000000 fluids-1.0.9/tests/test_numerics.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    18338 2021-06-02 03:14:57.000000 fluids-1.0.9/tests/test_units.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     2033 2021-04-16 05:52:44.000000 fluids-1.0.9/tests/test_vectorized.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     2897 2021-06-02 03:14:57.000000 fluids-1.0.9/tests/test_open_flow.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     2500 2021-04-16 05:52:44.000000 fluids-1.0.9/tests/test_utils.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    26245 2021-06-02 03:14:57.000000 fluids-1.0.9/tests/test_two_phase.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    47234 2021-06-02 03:14:57.000000 fluids-1.0.9/tests/test_flow_meter.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     1193 2020-12-29 16:52:12.000000 fluids-1.0.9/tests/__init__.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     2323 2021-06-02 03:14:57.000000 fluids-1.0.9/tests/test_mixing.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     8016 2021-06-02 03:14:57.000000 fluids-1.0.9/tests/test_pump.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     5156 2021-06-02 03:14:57.000000 fluids-1.0.9/tests/test_packed_bed.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     3295 2021-06-02 03:14:57.000000 fluids-1.0.9/tests/test_safety_valve.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     2545 2021-06-02 03:14:57.000000 fluids-1.0.9/tests/test_saltation.py
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     1090 2021-04-16 05:52:44.000000 fluids-1.0.9/LICENSE.txt
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     4595 2021-04-16 05:52:44.000000 fluids-1.0.9/README.rst
+drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-06-17 02:08:26.000000 fluids-1.0.9/fluids.egg-info/
+-rw-r--r--   0 caleb     (1000) caleb     (1000)        7 2021-06-17 02:08:26.000000 fluids-1.0.9/fluids.egg-info/top_level.txt
+-rw-r--r--   0 caleb     (1000) caleb     (1000)     8007 2021-06-17 02:08:26.000000 fluids-1.0.9/fluids.egg-info/PKG-INFO
+-rw-r--r--   0 caleb     (1000) caleb     (1000)    11717 2021-06-17 02:08:26.000000 fluids-1.0.9/fluids.egg-info/SOURCES.txt
+-rw-r--r--   0 caleb     (1000) caleb     (1000)        1 2021-06-17 02:08:26.000000 fluids-1.0.9/fluids.egg-info/dependency_links.txt
+-rw-r--r--   0 caleb     (1000) caleb     (1000)       88 2021-06-17 02:08:26.000000 fluids-1.0.9/fluids.egg-info/requires.txt
```

### Comparing `fluids-1.0.8/fluids/typing_utils.py` & `fluids-1.0.9/fluids/typing_utils.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/flow_meter.py` & `fluids-1.0.9/fluids/flow_meter.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/saltation.py` & `fluids-1.0.9/fluids/saltation.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/numerics/special.py` & `fluids-1.0.9/fluids/numerics/special.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/numerics/arrays.py` & `fluids-1.0.9/fluids/numerics/arrays.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/numerics/__init__.py` & `fluids-1.0.9/fluids/numerics/__init__.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/numerics/doubledouble.py` & `fluids-1.0.9/fluids/numerics/doubledouble.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/drag.py` & `fluids-1.0.9/fluids/drag.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/filters.py` & `fluids-1.0.9/fluids/filters.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/mixing.py` & `fluids-1.0.9/fluids/mixing.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/data/ASTM E11 sieves.csv` & `fluids-1.0.9/fluids/data/ASTM E11 sieves.csv`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/data/Miller 2E 1990 smooth bends Kb.csv` & `fluids-1.0.9/fluids/data/Miller 2E 1990 smooth bends Kb.csv`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/data/isd-history-cleaned.tsv` & `fluids-1.0.9/fluids/data/isd-history-cleaned.tsv`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/data/ISO 3310-1 sieves.csv` & `fluids-1.0.9/fluids/data/ISO 3310-1 sieves.csv`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/data/residential power.csv` & `fluids-1.0.9/fluids/data/residential power.csv`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/data/Miller 2E 1990 conical diffuser Kd.csv` & `fluids-1.0.9/fluids/data/Miller 2E 1990 conical diffuser Kd.csv`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/data/Miller 2E 1990 conical contractions K part 2.csv` & `fluids-1.0.9/fluids/data/Miller 2E 1990 conical contractions K part 2.csv`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/data/Miller 2E 1990 entrances rounded beveled K.csv` & `fluids-1.0.9/fluids/data/Miller 2E 1990 entrances rounded beveled K.csv`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/data/Miller 2E 1990 abrupt contraction K.csv` & `fluids-1.0.9/fluids/data/Miller 2E 1990 abrupt contraction K.csv`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/data/3 phase power.csv` & `fluids-1.0.9/fluids/data/3 phase power.csv`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/data/Miller 2E 1990 conical contractions K part 1.csv` & `fluids-1.0.9/fluids/data/Miller 2E 1990 conical contractions K part 1.csv`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/data/Miller 2E 1990 Kb mitre bend.csv` & `fluids-1.0.9/fluids/data/Miller 2E 1990 Kb mitre bend.csv`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/data/Miller 2E 1990 smooth bends outlet tangent length correction.csv` & `fluids-1.0.9/fluids/data/Miller 2E 1990 smooth bends outlet tangent length correction.csv`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/data/Miller 2E 1990 smooth bends Re correction.csv` & `fluids-1.0.9/fluids/data/Miller 2E 1990 smooth bends Re correction.csv`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/two_phase_voidage.py` & `fluids-1.0.9/fluids/two_phase_voidage.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/optional/hwm93.pyf` & `fluids-1.0.9/fluids/optional/hwm93.pyf`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/optional/irradiance.py` & `fluids-1.0.9/fluids/optional/irradiance.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/optional/pychebfun.py` & `fluids-1.0.9/fluids/optional/pychebfun.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/optional/dwm07b104i.dat` & `fluids-1.0.9/fluids/optional/dwm07b104i.dat`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/optional/hwm123114.bin` & `fluids-1.0.9/fluids/optional/hwm123114.bin`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/optional/spa.py` & `fluids-1.0.9/fluids/optional/spa.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/optional/hwm14.pyf` & `fluids-1.0.9/fluids/optional/hwm14.pyf`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/optional/hwm93.for` & `fluids-1.0.9/fluids/optional/hwm93.for`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/optional/gd2qd.dat` & `fluids-1.0.9/fluids/optional/gd2qd.dat`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/optional/hwm14.f90` & `fluids-1.0.9/fluids/optional/hwm14.f90`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/constants/constants.py` & `fluids-1.0.9/fluids/constants/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,7 +171,10 @@
 dyn = dyne = 1e-5
 lbf = pound_force = pound * g
 kgf = kilogram_force = g # * 1 kg
 
 
 deg2rad = 0.017453292519943295769 # Multiple an angle in degrees by this to get radians
 rad2deg = 57.295779513082320877# Multiple an angle in radians by this to get degrees
+
+
+root_two = 1.4142135623730951
```

### Comparing `fluids-1.0.8/fluids/constants/__init__.py` & `fluids-1.0.9/fluids/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/particle_size_distribution.py` & `fluids-1.0.9/fluids/particle_size_distribution.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/separator.py` & `fluids-1.0.9/fluids/separator.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/control_valve.py` & `fluids-1.0.9/fluids/control_valve.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/numba_vectorized.py` & `fluids-1.0.9/fluids/numba_vectorized.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/geometry.py` & `fluids-1.0.9/fluids/geometry.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/core.py` & `fluids-1.0.9/fluids/core.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/piping.py` & `fluids-1.0.9/fluids/piping.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/pump.py` & `fluids-1.0.9/fluids/pump.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/units.py` & `fluids-1.0.9/fluids/units.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/nrlmsise00/nrlmsise_00_data.py` & `fluids-1.0.9/fluids/nrlmsise00/nrlmsise_00_data.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/nrlmsise00/nrlmsise_00_header.py` & `fluids-1.0.9/fluids/nrlmsise00/nrlmsise_00_header.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/nrlmsise00/nrlmsise_00.py` & `fluids-1.0.9/fluids/nrlmsise00/nrlmsise_00.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/nrlmsise00/LICENSE` & `fluids-1.0.9/fluids/nrlmsise00/LICENSE`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/nrlmsise00/__init__.py` & `fluids-1.0.9/fluids/nrlmsise00/__init__.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/compressible.py` & `fluids-1.0.9/fluids/compressible.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/safety_valve.py` & `fluids-1.0.9/fluids/safety_valve.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/packed_bed.py` & `fluids-1.0.9/fluids/packed_bed.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/atmosphere.py` & `fluids-1.0.9/fluids/atmosphere.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/two_phase.py` & `fluids-1.0.9/fluids/two_phase.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/jet_pump.py` & `fluids-1.0.9/fluids/jet_pump.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/__init__.py` & `fluids-1.0.9/fluids/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,14 +147,14 @@
 
 def load_types():
     from fluids.typing_utils import type_module
     for m in submodules:
         type_module(m)
 
 
-__version__ = '1.0.8'
+__version__ = '1.0.9'
 
 try:
     fluids_dir = os.path.dirname(__file__)
     fluids_data_dir = os.path.join(fluids_dir, 'data')
 except:
     pass
```

### Comparing `fluids-1.0.8/fluids/fittings.py` & `fluids-1.0.9/fluids/fittings.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/design_climate.py` & `fluids-1.0.9/fluids/design_climate.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/open_flow.py` & `fluids-1.0.9/fluids/open_flow.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/packed_tower.py` & `fluids-1.0.9/fluids/packed_tower.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/vectorized.py` & `fluids-1.0.9/fluids/vectorized.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/numba.py` & `fluids-1.0.9/fluids/numba.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids/friction.py` & `fluids-1.0.9/fluids/friction.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/PKG-INFO` & `fluids-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: fluids
-Version: 1.0.8
+Version: 1.0.9
 Summary: Fluid dynamics component of Chemical Engineering Design Library (ChEDL)
 Home-page: https://github.com/CalebBell/fluids
 Author: Caleb Bell
 Author-email: Caleb.Andrew.Bell@gmail.com
 License: MIT
-Download-URL: https://github.com/CalebBell/fluids/tarball/1.0.8
+Download-URL: https://github.com/CalebBell/fluids/tarball/1.0.9
 Description: ======
         fluids
         ======
         
         .. image:: http://img.shields.io/pypi/v/fluids.svg?style=flat
            :target: https://pypi.python.org/pypi/fluids
            :alt: Version_status
```

### Comparing `fluids-1.0.8/docs/fluids.numba.rst` & `fluids-1.0.9/docs/fluids.numba.rst`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/fittings/flush_mounted_rounded_entrance.png` & `fluids-1.0.9/docs/fittings/flush_mounted_rounded_entrance.png`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/fittings/contraction_sharp.png` & `fluids-1.0.9/docs/fittings/contraction_sharp.png`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/fittings/diffuser_conical.png` & `fluids-1.0.9/docs/fittings/diffuser_conical.png`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/fittings/flush_mounted_beveled_entrance.png` & `fluids-1.0.9/docs/fittings/flush_mounted_beveled_entrance.png`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/fittings/entrance_mounted_at_an_angle.png` & `fluids-1.0.9/docs/fittings/entrance_mounted_at_an_angle.png`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/fittings/contraction_round.png` & `fluids-1.0.9/docs/fittings/contraction_round.png`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/fittings/sharp_edged_entrace_extended_mount.png` & `fluids-1.0.9/docs/fittings/sharp_edged_entrace_extended_mount.png`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/fittings/flush_mounted_beveled_orifice_entrance.png` & `fluids-1.0.9/docs/fittings/flush_mounted_beveled_orifice_entrance.png`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/fittings/contraction_beveled.png` & `fluids-1.0.9/docs/fittings/contraction_beveled.png`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/fittings/flush_mounted_sharp_edged_entrance.png` & `fluids-1.0.9/docs/fittings/flush_mounted_sharp_edged_entrance.png`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/fittings/bend_rounded.png` & `fluids-1.0.9/docs/fittings/bend_rounded.png`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/fittings/curved_wall_diffuser.png` & `fluids-1.0.9/docs/fittings/curved_wall_diffuser.png`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/fittings/bend_miter.png` & `fluids-1.0.9/docs/fittings/bend_miter.png`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/fittings/flush_mounted_exit.png` & `fluids-1.0.9/docs/fittings/flush_mounted_exit.png`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/fittings/contraction_conical.png` & `fluids-1.0.9/docs/fittings/contraction_conical.png`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/fluids.units.rst` & `fluids-1.0.9/docs/fluids.units.rst`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/fluids.vectorized.rst` & `fluids-1.0.9/docs/fluids.vectorized.rst`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/plots/entrance_beveled_plot.py` & `fluids-1.0.9/docs/plots/entrance_beveled_plot.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/plots/ft_Crane_plot.py` & `fluids-1.0.9/docs/plots/ft_Crane_plot.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/plots/bend_rounded_Crane_plot.py` & `fluids-1.0.9/docs/plots/bend_rounded_Crane_plot.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/plots/diffuser_conical_plot.py` & `fluids-1.0.9/docs/plots/diffuser_conical_plot.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/plots/bend_miter_plot.py` & `fluids-1.0.9/docs/plots/bend_miter_plot.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/plots/contraction_conical_plot.py` & `fluids-1.0.9/docs/plots/contraction_conical_plot.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/plots/contraction_round_plot.py` & `fluids-1.0.9/docs/plots/contraction_round_plot.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/conf.py` & `fluids-1.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/fluids.rst` & `fluids-1.0.9/docs/fluids.rst`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/_static/copybutton.js` & `fluids-1.0.9/docs/_static/copybutton.js`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/Data/Pipe Schedules.ipynb` & `fluids-1.0.9/docs/Data/Pipe Schedules.ipynb`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/Data/Sieve Sizes for Particle Size Distributions.ipynb` & `fluids-1.0.9/docs/Data/Sieve Sizes for Particle Size Distributions.ipynb`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/Data/Friction.ipynb` & `fluids-1.0.9/docs/Data/Friction.ipynb`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.14 Bernoulli's Theorem-Water.ipynb` & `fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.14 Bernoulli's Theorem-Water.ipynb`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.21 Gases at Sonic Velocity.ipynb` & `fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.21 Gases at Sonic Velocity.ipynb`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.11 Flat heating Coils - Water.ipynb` & `fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.11 Flat heating Coils - Water.ipynb`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.22 Compressible Fluids at Subsonic Velocity.ipynb` & `fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.22 Compressible Fluids at Subsonic Velocity.ipynb`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.27 Sizing Control Valves for Liquid Service.ipynb` & `fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.27 Sizing Control Valves for Liquid Service.ipynb`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.19 Water.ipynb` & `fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.19 Water.ipynb`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.8 Laminar flow in Valves, Fittings, and Pipe - SAE oil through a pipe and globe valve.ipynb` & `fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.8 Laminar flow in Valves, Fittings, and Pipe - SAE oil through a pipe and globe valve.ipynb`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.7 Laminar flow in Valves, Fittings, and Pipe - System from Example 7.6.ipynb` & `fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.7 Laminar flow in Valves, Fittings, and Pipe - System from Example 7.6.ipynb`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.2 L, L over D and K from Kv for Conventional Type Valves.ipynb` & `fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.2 L, L over D and K from Kv for Conventional Type Valves.ipynb`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.26 Pipe Partially Filled with Flowing Water.ipynb` & `fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.26 Pipe Partially Filled with Flowing Water.ipynb`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.35 Hydraulic Resistance of a Converging Tee.ipynb` & `fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.35 Hydraulic Resistance of a Converging Tee.ipynb`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.4 Venturi Type Valves.ipynb` & `fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.4 Venturi Type Valves.ipynb`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.29 Orifice Flow Rate Calculation.ipynb` & `fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.29 Orifice Flow Rate Calculation.ipynb`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.23 Flow Through Orifice Meters.ipynb` & `fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.23 Flow Through Orifice Meters.ipynb`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.5 Lift Check Valves.ipynb` & `fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.5 Lift Check Valves.ipynb`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.20 Steam at Sonic Velocity.ipynb` & `fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.20 Steam at Sonic Velocity.ipynb`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.32 NPSH Available Calculation.ipynb` & `fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.32 NPSH Available Calculation.ipynb`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.17 Sizing of Pump for Oil Pipelines.ipynb` & `fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.17 Sizing of Pump for Oil Pipelines.ipynb`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.34 Pump Power and Operating Cost.ipynb` & `fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.34 Pump Power and Operating Cost.ipynb`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.18 Gas.ipynb` & `fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.18 Gas.ipynb`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.28 Checking for Choked Flow Conditions in a Control Valve.ipynb` & `fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.28 Checking for Choked Flow Conditions in a Control Valve.ipynb`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.10 Piping Systems - Steam.ipynb` & `fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.10 Piping Systems - Steam.ipynb`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.15 Power Required for Pumping.ipynb` & `fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.15 Power Required for Pumping.ipynb`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.16 Air Lines.ipynb` & `fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.16 Air Lines.ipynb`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.30 Nozzle Sizing Calculations.ipynb` & `fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.30 Nozzle Sizing Calculations.ipynb`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.6 Reduced Port Ball Valve.ipynb` & `fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.6 Reduced Port Ball Valve.ipynb`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.12 Orifice Size for Given Pressure Drop and Velocity.ipynb` & `fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.12 Orifice Size for Given Pressure Drop and Velocity.ipynb`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.9 Laminar Flow in Valves, Fittings, and Pipe.ipynb` & `fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.9 Laminar Flow in Valves, Fittings, and Pipe.ipynb`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.25 Rectangular Duct - Application of Hydraulic Radius to Flow Problems.ipynb` & `fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.25 Rectangular Duct - Application of Hydraulic Radius to Flow Problems.ipynb`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.1 Smooth Pipe (Plastic).ipynb` & `fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.1 Smooth Pipe (Plastic).ipynb`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.13 Flow given in English Units - Oil.ipynb` & `fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.13 Flow given in English Units - Oil.ipynb`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.36 Hydraulic Resistance of a Diverging Wye.ipynb` & `fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.36 Hydraulic Resistance of a Diverging Wye.ipynb`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.24 Laminar Flow.ipynb` & `fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.24 Laminar Flow.ipynb`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.3 L, L over D, K, and Kv for Conventional Type Valves.ipynb` & `fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.3 L, L over D, K, and Kv for Conventional Type Valves.ipynb`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/Examples/Crane TP 410 Solved Problems/7.33 Pump Affinity Rules.ipynb` & `fluids-1.0.9/docs/Examples/Crane TP 410 Solved Problems/7.33 Pump Affinity Rules.ipynb`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/tutorial.rst` & `fluids-1.0.9/docs/tutorial.rst`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/examples.rst` & `fluids-1.0.9/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/developers.rst` & `fluids-1.0.9/docs/developers.rst`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/docs/index.rst` & `fluids-1.0.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/pytest.ini` & `fluids-1.0.9/pytest.ini`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/setup.py` & `fluids-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,16 +64,16 @@
             'sedimentation engineering pipeline process simulation particle '
             'size distribution')
 
 setup(
     name='fluids',
     packages=['fluids'],
     license='MIT',
-    version='1.0.8',
-    download_url='https://github.com/CalebBell/fluids/tarball/1.0.8',
+    version='1.0.9',
+    download_url='https://github.com/CalebBell/fluids/tarball/1.0.9',
     description=description,
     long_description=open('README.rst').read(),
     install_requires=["numpy>=1.5.0", "scipy>=0.9.0"],
     extras_require={
         'Coverage documentation':  ['wsgiref>=0.1.2', 'coverage>=4.0.3', 'pint']
     },
     author='Caleb Bell',
```

### Comparing `fluids-1.0.8/MANIFEST.in` & `fluids-1.0.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/test_jet_pump.py` & `fluids-1.0.9/tests/test_jet_pump.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1989/724050-13743.op` & `fluids-1.0.9/tests/gsod/1989/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1957/724050-13743.op` & `fluids-1.0.9/tests/gsod/1957/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1988/724050-13743.op` & `fluids-1.0.9/tests/gsod/1988/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1952/724050-13743.op` & `fluids-1.0.9/tests/gsod/1952/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/2013/724050-13743.op` & `fluids-1.0.9/tests/gsod/2013/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/2013/722324-03071.op` & `fluids-1.0.9/tests/gsod/2013/722324-03071.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1978/724050-13743.op` & `fluids-1.0.9/tests/gsod/1978/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1951/724050-13743.op` & `fluids-1.0.9/tests/gsod/1951/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1959/724050-13743.op` & `fluids-1.0.9/tests/gsod/1959/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1999/724050-13743.op` & `fluids-1.0.9/tests/gsod/1999/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1969/724050-13743.op` & `fluids-1.0.9/tests/gsod/1969/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1986/724050-13743.op` & `fluids-1.0.9/tests/gsod/1986/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1945/724050-13743.op` & `fluids-1.0.9/tests/gsod/1945/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1991/724050-13743.op` & `fluids-1.0.9/tests/gsod/1991/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/2009/724050-13743.op` & `fluids-1.0.9/tests/gsod/2009/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/2009/722324-03071.op` & `fluids-1.0.9/tests/gsod/2009/722324-03071.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/2003/724050-13743.op` & `fluids-1.0.9/tests/gsod/2003/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1994/724050-13743.op` & `fluids-1.0.9/tests/gsod/1994/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1980/724050-13743.op` & `fluids-1.0.9/tests/gsod/1980/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/2019/724050-13743.op` & `fluids-1.0.9/tests/gsod/2019/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/2019/722324-03071.op` & `fluids-1.0.9/tests/gsod/2019/722324-03071.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1944/724050-13743.op` & `fluids-1.0.9/tests/gsod/1944/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1995/724050-13743.op` & `fluids-1.0.9/tests/gsod/1995/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1984/724050-13743.op` & `fluids-1.0.9/tests/gsod/1984/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1958/724050-13743.op` & `fluids-1.0.9/tests/gsod/1958/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1942/724050-13743.op` & `fluids-1.0.9/tests/gsod/1942/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1941/724050-13743.op` & `fluids-1.0.9/tests/gsod/1941/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1955/724050-13743.op` & `fluids-1.0.9/tests/gsod/1955/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1961/724050-13743.op` & `fluids-1.0.9/tests/gsod/1961/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/2017/724050-13743.op` & `fluids-1.0.9/tests/gsod/2017/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/2017/722324-03071.op` & `fluids-1.0.9/tests/gsod/2017/722324-03071.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1992/724050-13743.op` & `fluids-1.0.9/tests/gsod/1992/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1950/724050-13743.op` & `fluids-1.0.9/tests/gsod/1950/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1993/724050-13743.op` & `fluids-1.0.9/tests/gsod/1993/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1938/724050-13743.op` & `fluids-1.0.9/tests/gsod/1938/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1966/724050-13743.op` & `fluids-1.0.9/tests/gsod/1966/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1987/724050-13743.op` & `fluids-1.0.9/tests/gsod/1987/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1983/724050-13743.op` & `fluids-1.0.9/tests/gsod/1983/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/2011/724050-13743.op` & `fluids-1.0.9/tests/gsod/2011/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/2011/722324-03071.op` & `fluids-1.0.9/tests/gsod/2011/722324-03071.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1981/724050-13743.op` & `fluids-1.0.9/tests/gsod/1981/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/2018/724050-13743.op` & `fluids-1.0.9/tests/gsod/2018/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/2018/722324-03071.op` & `fluids-1.0.9/tests/gsod/2018/722324-03071.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/2016/724050-13743.op` & `fluids-1.0.9/tests/gsod/2016/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/2016/722324-03071.op` & `fluids-1.0.9/tests/gsod/2016/722324-03071.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1940/724050-13743.op` & `fluids-1.0.9/tests/gsod/1940/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1962/724050-13743.op` & `fluids-1.0.9/tests/gsod/1962/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1936/724050-13743.op` & `fluids-1.0.9/tests/gsod/1936/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1973/724050-13743.op` & `fluids-1.0.9/tests/gsod/1973/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1998/724050-13743.op` & `fluids-1.0.9/tests/gsod/1998/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1967/724050-13743.op` & `fluids-1.0.9/tests/gsod/1967/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1997/724050-13743.op` & `fluids-1.0.9/tests/gsod/1997/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1946/724050-13743.op` & `fluids-1.0.9/tests/gsod/1946/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/2006/724050-13743.op` & `fluids-1.0.9/tests/gsod/2006/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/2006/722324-03071.op` & `fluids-1.0.9/tests/gsod/2006/722324-03071.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1990/724050-13743.op` & `fluids-1.0.9/tests/gsod/1990/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1943/724050-13743.op` & `fluids-1.0.9/tests/gsod/1943/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1985/724050-13743.op` & `fluids-1.0.9/tests/gsod/1985/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1954/724050-13743.op` & `fluids-1.0.9/tests/gsod/1954/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1977/724050-13743.op` & `fluids-1.0.9/tests/gsod/1977/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/2002/724050-13743.op` & `fluids-1.0.9/tests/gsod/2002/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1964/724050-13743.op` & `fluids-1.0.9/tests/gsod/1964/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/2008/724050-13743.op` & `fluids-1.0.9/tests/gsod/2008/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/2008/722324-03071.op` & `fluids-1.0.9/tests/gsod/2008/722324-03071.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1965/724050-13743.op` & `fluids-1.0.9/tests/gsod/1965/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1949/724050-13743.op` & `fluids-1.0.9/tests/gsod/1949/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1963/724050-13743.op` & `fluids-1.0.9/tests/gsod/1963/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/2004/724050-13743.op` & `fluids-1.0.9/tests/gsod/2004/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/2012/724050-13743.op` & `fluids-1.0.9/tests/gsod/2012/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/2012/722324-03071.op` & `fluids-1.0.9/tests/gsod/2012/722324-03071.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1976/724050-13743.op` & `fluids-1.0.9/tests/gsod/1976/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/2007/724050-13743.op` & `fluids-1.0.9/tests/gsod/2007/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/2007/722324-03071.op` & `fluids-1.0.9/tests/gsod/2007/722324-03071.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/2014/724050-13743.op` & `fluids-1.0.9/tests/gsod/2014/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/2014/722324-03071.op` & `fluids-1.0.9/tests/gsod/2014/722324-03071.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1975/724050-13743.op` & `fluids-1.0.9/tests/gsod/1975/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1974/724050-13743.op` & `fluids-1.0.9/tests/gsod/1974/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1979/724050-13743.op` & `fluids-1.0.9/tests/gsod/1979/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/2000/724050-13743.op` & `fluids-1.0.9/tests/gsod/2000/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1960/724050-13743.op` & `fluids-1.0.9/tests/gsod/1960/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/2015/724050-13743.op` & `fluids-1.0.9/tests/gsod/2015/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/2015/722324-03071.op` & `fluids-1.0.9/tests/gsod/2015/722324-03071.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1937/724050-13743.op` & `fluids-1.0.9/tests/gsod/1937/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1953/724050-13743.op` & `fluids-1.0.9/tests/gsod/1953/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/2005/724050-13743.op` & `fluids-1.0.9/tests/gsod/2005/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/2001/724050-13743.op` & `fluids-1.0.9/tests/gsod/2001/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1947/724050-13743.op` & `fluids-1.0.9/tests/gsod/1947/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1982/724050-13743.op` & `fluids-1.0.9/tests/gsod/1982/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1996/724050-13743.op` & `fluids-1.0.9/tests/gsod/1996/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1948/724050-13743.op` & `fluids-1.0.9/tests/gsod/1948/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/2010/724050-13743.op` & `fluids-1.0.9/tests/gsod/2010/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/2010/722324-03071.op` & `fluids-1.0.9/tests/gsod/2010/722324-03071.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/2020/724050-13743.op` & `fluids-1.0.9/tests/gsod/2020/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/2020/722324-03071.op` & `fluids-1.0.9/tests/gsod/2020/722324-03071.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1968/724050-13743.op` & `fluids-1.0.9/tests/gsod/1968/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1939/724050-13743.op` & `fluids-1.0.9/tests/gsod/1939/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/gsod/1956/724050-13743.op` & `fluids-1.0.9/tests/gsod/1956/724050-13743.op`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/test_filters.py` & `fluids-1.0.9/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/spa/test_spa.py` & `fluids-1.0.9/tests/spa/test_spa.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/test_particle_size_distribution.py` & `fluids-1.0.9/tests/test_particle_size_distribution.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/particle_size_distribution/unsoda_distributions_20140206.csv` & `fluids-1.0.9/tests/particle_size_distribution/unsoda_distributions_20140206.csv`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/test_control_valve.py` & `fluids-1.0.9/tests/test_control_valve.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/test_drag.py` & `fluids-1.0.9/tests/test_drag.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/test_nrlmsise00_full.py` & `fluids-1.0.9/tests/test_nrlmsise00_full.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/test_fittings.py` & `fluids-1.0.9/tests/test_fittings.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/manual_runner.py` & `fluids-1.0.9/tests/manual_runner.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/test_fittings_fits.py` & `fluids-1.0.9/tests/test_fittings_fits.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/test_nrlmsise00_file_output.py` & `fluids-1.0.9/tests/test_nrlmsise00_file_output.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/test_atmosphere.py` & `fluids-1.0.9/tests/test_atmosphere.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/test_numerics_special.py` & `fluids-1.0.9/tests/test_numerics_special.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/test_two_phase_voidage.py` & `fluids-1.0.9/tests/test_two_phase_voidage.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/test_compressible.py` & `fluids-1.0.9/tests/test_compressible.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/test_packed_tower.py` & `fluids-1.0.9/tests/test_packed_tower.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/test_friction.py` & `fluids-1.0.9/tests/test_friction.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/make_test_stubs.py` & `fluids-1.0.9/tests/make_test_stubs.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/test_design_climate.py` & `fluids-1.0.9/tests/test_design_climate.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/test_geometry.py` & `fluids-1.0.9/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/test_numba.py` & `fluids-1.0.9/tests/test_numba.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/test_piping.py` & `fluids-1.0.9/tests/test_piping.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/test_numerics_doubledouble.py` & `fluids-1.0.9/tests/test_numerics_doubledouble.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/test_separator.py` & `fluids-1.0.9/tests/test_separator.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/nrlmsise00/known_data_hours.txt` & `fluids-1.0.9/tests/nrlmsise00/known_data_hours.txt`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/nrlmsise00/known_data_latitudes.txt` & `fluids-1.0.9/tests/nrlmsise00/known_data_latitudes.txt`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/nrlmsise00/known_data_height.txt` & `fluids-1.0.9/tests/nrlmsise00/known_data_height.txt`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/nrlmsise00/known_data_longitudes.txt` & `fluids-1.0.9/tests/nrlmsise00/known_data_longitudes.txt`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/nrlmsise00/known_data_day_of_year.txt` & `fluids-1.0.9/tests/nrlmsise00/known_data_day_of_year.txt`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/nrlmsise00/known_data_high_height.txt` & `fluids-1.0.9/tests/nrlmsise00/known_data_high_height.txt`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/nrlmsise00/data_from_C_version.txt` & `fluids-1.0.9/tests/nrlmsise00/data_from_C_version.txt`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/nrlmsise00/__init__.py` & `fluids-1.0.9/tests/nrlmsise00/__init__.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/test_core.py` & `fluids-1.0.9/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/test_numerics.py` & `fluids-1.0.9/tests/test_numerics.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/test_units.py` & `fluids-1.0.9/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/test_vectorized.py` & `fluids-1.0.9/tests/test_vectorized.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/test_open_flow.py` & `fluids-1.0.9/tests/test_open_flow.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/test_utils.py` & `fluids-1.0.9/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/test_two_phase.py` & `fluids-1.0.9/tests/test_two_phase.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/test_flow_meter.py` & `fluids-1.0.9/tests/test_flow_meter.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/__init__.py` & `fluids-1.0.9/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/test_mixing.py` & `fluids-1.0.9/tests/test_mixing.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/test_pump.py` & `fluids-1.0.9/tests/test_pump.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/test_packed_bed.py` & `fluids-1.0.9/tests/test_packed_bed.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/test_safety_valve.py` & `fluids-1.0.9/tests/test_safety_valve.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/tests/test_saltation.py` & `fluids-1.0.9/tests/test_saltation.py`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/LICENSE.txt` & `fluids-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/README.rst` & `fluids-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `fluids-1.0.8/fluids.egg-info/PKG-INFO` & `fluids-1.0.9/fluids.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: fluids
-Version: 1.0.8
+Version: 1.0.9
 Summary: Fluid dynamics component of Chemical Engineering Design Library (ChEDL)
 Home-page: https://github.com/CalebBell/fluids
 Author: Caleb Bell
 Author-email: Caleb.Andrew.Bell@gmail.com
 License: MIT
-Download-URL: https://github.com/CalebBell/fluids/tarball/1.0.8
+Download-URL: https://github.com/CalebBell/fluids/tarball/1.0.9
 Description: ======
         fluids
         ======
         
         .. image:: http://img.shields.io/pypi/v/fluids.svg?style=flat
            :target: https://pypi.python.org/pypi/fluids
            :alt: Version_status
```

### Comparing `fluids-1.0.8/fluids.egg-info/SOURCES.txt` & `fluids-1.0.9/fluids.egg-info/SOURCES.txt`

 * *Files identical despite different names*

