# Comparing `tmp/zigzag-dse-2.3.4.tar.gz` & `tmp/zigzag-dse-2.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zigzag-dse-2.3.4.tar", last modified: Sat Apr 22 12:48:25 2023, max compression
+gzip compressed data, was "zigzag-dse-2.3.5.tar", last modified: Sat Apr 22 22:36:10 2023, max compression
```

## Comparing `zigzag-dse-2.3.4.tar` & `zigzag-dse-2.3.5.tar`

### file list

```diff
@@ -1,251 +1,251 @@
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 12:48:25.051751 zigzag-dse-2.3.4/
--rw-r--r--   0 asymons   (1000) asymons   (1000)     1522 2022-06-17 07:16:25.000000 zigzag-dse-2.3.4/LICENSE
--rw-r--r--   0 asymons   (1000) asymons   (1000)       88 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/MANIFEST.in
--rw-r--r--   0 asymons   (1000) asymons   (1000)     8918 2023-04-22 12:48:25.041751 zigzag-dse-2.3.4/PKG-INFO
--rw-r--r--   0 asymons   (1000) asymons   (1000)     6596 2023-03-14 15:21:48.000000 zigzag-dse-2.3.4/README.md
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 12:48:24.991751 zigzag-dse-2.3.4/docs/
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 12:48:25.001751 zigzag-dse-2.3.4/docs/source/
--rw-r--r--   0 asymons   (1000) asymons   (1000)     2594 2023-03-14 15:21:19.000000 zigzag-dse-2.3.4/docs/source/conf.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     1587 2023-04-22 12:48:16.000000 zigzag-dse-2.3.4/pyproject.toml
--rw-r--r--   0 asymons   (1000) asymons   (1000)       38 2023-04-22 12:48:25.051751 zigzag-dse-2.3.4/setup.cfg
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 12:48:25.001751 zigzag-dse-2.3.4/zigzag/
--rw-r--r--   0 asymons   (1000) asymons   (1000)       22 2023-04-22 12:48:16.000000 zigzag-dse-2.3.4/zigzag/__init__.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     2497 2022-11-06 07:09:28.000000 zigzag-dse-2.3.4/zigzag/__main__.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     4451 2023-04-15 15:25:43.000000 zigzag-dse-2.3.4/zigzag/api.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 12:48:25.001751 zigzag-dse-2.3.4/zigzag/classes/
--rw-r--r--   0 asymons   (1000) asymons   (1000)        0 2022-11-06 21:40:40.000000 zigzag-dse-2.3.4/zigzag/classes/__init__.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 12:48:25.001751 zigzag-dse-2.3.4/zigzag/classes/cacti/
--rw-r--r--   0 asymons   (1000) asymons   (1000)      291 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/README.md
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 12:48:25.001751 zigzag-dse-2.3.4/zigzag/classes/cacti/__pycache__/
--rw-r--r--   0 asymons   (1000) asymons   (1000)     3423 2023-04-22 12:35:57.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/__pycache__/cacti_parser.cpython-310.pyc
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 12:48:25.011751 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/
--rw-r--r--   0 asymons   (1000) asymons   (1000)     6576 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/2DDRAM_Samsung2GbDDR2.cfg
--rw-r--r--   0 asymons   (1000) asymons   (1000)     6555 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/2DDRAM_micron1Gb.cfg
--rw-r--r--   0 asymons   (1000) asymons   (1000)     6920 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/3DDRAM_Samsung3D8Gb_extened.cfg
--rw-r--r--   0 asymons   (1000) asymons   (1000)     5324 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/README
--rw-r--r--   0 asymons   (1000) asymons   (1000)     9282 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/TSV.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     3322 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/TSV.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)    41184 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/Ucache.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     3607 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/Ucache.h
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 12:48:25.011751 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/__pycache__/
--rw-r--r--   0 asymons   (1000) asymons   (1000)    13713 2023-04-16 14:07:27.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/__pycache__/cacti_config_creator.cpython-310.pyc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     5116 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/arbiter.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     2771 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/arbiter.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)     2057 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/area.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     2416 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/area.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)     8474 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/bank.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     2664 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/bank.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)    29279 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/basic_circuit.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     7364 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/basic_circuit.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)    11041 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/cache.cfg_temp
--rw-r--r--   0 asymons   (1000) asymons   (1000)    32713 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/cache_old.cfg.out
--rwxr-xr-x   0 asymons   (1000) asymons   (1000)  2421320 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/cacti
--rw-r--r--   0 asymons   (1000) asymons   (1000)      173 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/cacti.i
--rw-r--r--   0 asymons   (1000) asymons   (1000)     1334 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/cacti.mk
--rw-r--r--   0 asymons   (1000) asymons   (1000)    25297 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/cacti_config_creator.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     5586 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/cacti_interface.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)    27215 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/cacti_interface.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)     3569 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/cacti_top.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     7561 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/component.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     2837 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/component.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)     9565 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/const.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)     5001 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/contention.dat
--rw-r--r--   0 asymons   (1000) asymons   (1000)     7349 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/crossbar.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     3204 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/crossbar.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)     9849 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/ddr3.cfg
--rw-r--r--   0 asymons   (1000) asymons   (1000)    62337 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/decoder.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     7405 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/decoder.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)     3712 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/dram.cfg
--rw-r--r--   0 asymons   (1000) asymons   (1000)     9750 2023-04-22 12:43:51.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/example_mem_pool.yaml
--rw-r--r--   0 asymons   (1000) asymons   (1000)    17411 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/extio.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)      878 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/extio.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)    46185 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/extio_technology.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     9068 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/extio_technology.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)    23772 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/htree2.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     3595 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/htree2.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)   133713 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/io.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     2116 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/io.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)     9850 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/lpddr.cfg
--rw-r--r--   0 asymons   (1000) asymons   (1000)     7217 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/main.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)      407 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/makefile
--rw-r--r--   0 asymons   (1000) asymons   (1000)    94813 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/mat.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     6122 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/mat.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)    16630 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/memcad.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)      553 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/memcad.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)    11483 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/memcad_parameters.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     4490 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/memcad_parameters.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)    29014 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/memorybus.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     5426 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/memorybus.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)    19629 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/nuca.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     3306 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/nuca.h
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 12:48:25.031751 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/obj_dbg/
--rw-r--r--   0 asymons   (1000) asymons   (1000)   134304 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/obj_dbg/TSV.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   352744 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/obj_dbg/Ucache.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   157960 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/obj_dbg/arbiter.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   124352 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/obj_dbg/area.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   156624 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/obj_dbg/bank.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   155192 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/obj_dbg/basic_circuit.o
--rwxr-xr-x   0 asymons   (1000) asymons   (1000)  2421320 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/obj_dbg/cacti
--rw-r--r--   0 asymons   (1000) asymons   (1000)   175768 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/obj_dbg/cacti_interface.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   159768 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/obj_dbg/component.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   160680 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/obj_dbg/crossbar.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   207224 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/obj_dbg/decoder.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   145592 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/obj_dbg/extio.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   180464 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/obj_dbg/extio_technology.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   178384 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/obj_dbg/htree2.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   411960 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/obj_dbg/io.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   192248 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/obj_dbg/main.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   270320 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/obj_dbg/mat.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   569648 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/obj_dbg/memcad.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   280416 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/obj_dbg/memcad_parameters.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   204480 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/obj_dbg/memorybus.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   256824 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/obj_dbg/nuca.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   313848 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/obj_dbg/parameter.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   124400 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/obj_dbg/powergating.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   175432 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/obj_dbg/router.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   128080 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/obj_dbg/subarray.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   144976 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/obj_dbg/technology.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   228000 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/obj_dbg/uca.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   232752 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/obj_dbg/wire.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   111980 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/parameter.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)    20306 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/parameter.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)     5286 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/powergating.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     3055 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/powergating.h
--rwxr-xr-x   0 asymons   (1000) asymons   (1000)     1886 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/regression.test
--rw-r--r--   0 asymons   (1000) asymons   (1000)    10212 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/router.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     3721 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/router.h
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 12:48:25.031751 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/sample_config_files/
--rw-r--r--   0 asymons   (1000) asymons   (1000)     8781 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/sample_config_files/ddr3_cache.cfg
--rw-r--r--   0 asymons   (1000) asymons   (1000)     8768 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/sample_config_files/diff_ddr3_cache.cfg
--rw-r--r--   0 asymons   (1000) asymons   (1000)     8780 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/sample_config_files/lpddr3_cache.cfg
--rw-r--r--   0 asymons   (1000) asymons   (1000)     8784 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/sample_config_files/wideio_cache.cfg
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 12:48:25.031751 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/self_gen/
--rw-r--r--   0 asymons   (1000) asymons   (1000)     9545 2023-04-22 12:43:51.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/self_gen/cache.cfg
--rw-r--r--   0 asymons   (1000) asymons   (1000)      579 2023-04-22 12:43:51.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/self_gen/cache.cfg.out
--rw-r--r--   0 asymons   (1000) asymons   (1000)     8332 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/subarray.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     2542 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/subarray.h
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 12:48:25.031751 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/tech_params/
--rw-r--r--   0 asymons   (1000) asymons   (1000)       25 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/tech_params/16nm.dat
--rw-r--r--   0 asymons   (1000) asymons   (1000)    23666 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/tech_params/180nm-old.dat
--rw-r--r--   0 asymons   (1000) asymons   (1000)     3842 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/tech_params/180nm.dat
--rw-r--r--   0 asymons   (1000) asymons   (1000)     4575 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/tech_params/22nm.dat
--rw-r--r--   0 asymons   (1000) asymons   (1000)     4759 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/tech_params/32nm.dat
--rw-r--r--   0 asymons   (1000) asymons   (1000)     4755 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/tech_params/45nm.dat
--rw-r--r--   0 asymons   (1000) asymons   (1000)    24571 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/tech_params/65nm-old.dat
--rw-r--r--   0 asymons   (1000) asymons   (1000)     4758 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/tech_params/65nm.dat
--rw-r--r--   0 asymons   (1000) asymons   (1000)    24570 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/tech_params/90nm-old.dat
--rw-r--r--   0 asymons   (1000) asymons   (1000)     4742 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/tech_params/90nm.dat
--rw-r--r--   0 asymons   (1000) asymons   (1000)    15087 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/technology.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)    41317 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/uca.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     4035 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/uca.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)     2064 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/version_cacti.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)    29856 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/wire.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     4375 2023-03-27 09:38:39.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/wire.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)     6110 2023-04-22 12:47:35.000000 zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_parser.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 12:48:25.031751 zigzag-dse-2.3.4/zigzag/classes/cost_model/
--rw-r--r--   0 asymons   (1000) asymons   (1000)    62023 2023-04-16 12:43:30.000000 zigzag-dse-2.3.4/zigzag/classes/cost_model/cost_model.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 12:48:24.991751 zigzag-dse-2.3.4/zigzag/classes/hardware/
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 12:48:25.031751 zigzag-dse-2.3.4/zigzag/classes/hardware/architecture/
--rw-r--r--   0 asymons   (1000) asymons   (1000)     1278 2023-04-16 13:43:29.000000 zigzag-dse-2.3.4/zigzag/classes/hardware/architecture/accelerator.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     9441 2023-04-07 09:22:11.000000 zigzag-dse-2.3.4/zigzag/classes/hardware/architecture/adder_hierarchy.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     6031 2023-04-07 09:22:16.000000 zigzag-dse-2.3.4/zigzag/classes/hardware/architecture/core.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)      918 2023-04-07 09:22:20.000000 zigzag-dse-2.3.4/zigzag/classes/hardware/architecture/dimension.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)    11764 2023-04-07 09:22:26.000000 zigzag-dse-2.3.4/zigzag/classes/hardware/architecture/memory_hierarchy.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     3351 2023-04-07 09:22:31.000000 zigzag-dse-2.3.4/zigzag/classes/hardware/architecture/memory_instance.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)    12231 2023-04-07 09:22:36.000000 zigzag-dse-2.3.4/zigzag/classes/hardware/architecture/memory_level.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     3014 2023-04-07 09:22:40.000000 zigzag-dse-2.3.4/zigzag/classes/hardware/architecture/operational_array.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     1874 2023-04-07 09:22:44.000000 zigzag-dse-2.3.4/zigzag/classes/hardware/architecture/operational_unit.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 12:48:24.991751 zigzag-dse-2.3.4/zigzag/classes/io/
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 12:48:25.031751 zigzag-dse-2.3.4/zigzag/classes/io/accelerator/
--rw-r--r--   0 asymons   (1000) asymons   (1000)     2805 2022-11-06 21:24:03.000000 zigzag-dse-2.3.4/zigzag/classes/io/accelerator/parser.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 12:48:25.031751 zigzag-dse-2.3.4/zigzag/classes/io/onnx/
--rw-r--r--   0 asymons   (1000) asymons   (1000)     9127 2023-04-15 11:49:50.000000 zigzag-dse-2.3.4/zigzag/classes/io/onnx/conv.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)      884 2023-04-07 09:12:40.000000 zigzag-dse-2.3.4/zigzag/classes/io/onnx/default.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     5382 2023-04-07 09:12:45.000000 zigzag-dse-2.3.4/zigzag/classes/io/onnx/gemm.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     3679 2023-04-07 09:12:49.000000 zigzag-dse-2.3.4/zigzag/classes/io/onnx/matmul.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     4912 2023-04-07 09:12:53.000000 zigzag-dse-2.3.4/zigzag/classes/io/onnx/model.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     1163 2023-04-07 09:12:58.000000 zigzag-dse-2.3.4/zigzag/classes/io/onnx/parser.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     4391 2023-04-07 09:13:02.000000 zigzag-dse-2.3.4/zigzag/classes/io/onnx/utils.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 12:48:25.031751 zigzag-dse-2.3.4/zigzag/classes/mapping/
--rw-r--r--   0 asymons   (1000) asymons   (1000)    40951 2023-04-07 09:24:31.000000 zigzag-dse-2.3.4/zigzag/classes/mapping/combined_mapping.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)      637 2023-04-07 09:24:42.000000 zigzag-dse-2.3.4/zigzag/classes/mapping/loop.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     9386 2023-04-07 09:24:55.000000 zigzag-dse-2.3.4/zigzag/classes/mapping/mapping_assist_funcs.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 12:48:25.031751 zigzag-dse-2.3.4/zigzag/classes/mapping/memory/
--rw-r--r--   0 asymons   (1000) asymons   (1000)        0 2023-04-07 09:25:08.000000 zigzag-dse-2.3.4/zigzag/classes/mapping/memory/data_layout.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 12:48:25.041751 zigzag-dse-2.3.4/zigzag/classes/mapping/spatial/
--rw-r--r--   0 asymons   (1000) asymons   (1000)     7607 2023-04-07 09:25:03.000000 zigzag-dse-2.3.4/zigzag/classes/mapping/spatial/spatial_mapping.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 12:48:25.041751 zigzag-dse-2.3.4/zigzag/classes/mapping/temporal/
--rw-r--r--   0 asymons   (1000) asymons   (1000)      380 2023-04-07 09:25:12.000000 zigzag-dse-2.3.4/zigzag/classes/mapping/temporal/temporal_loop.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     7412 2023-04-07 09:25:16.000000 zigzag-dse-2.3.4/zigzag/classes/mapping/temporal/temporal_mapping.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 12:48:24.991751 zigzag-dse-2.3.4/zigzag/classes/opt/
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 12:48:25.041751 zigzag-dse-2.3.4/zigzag/classes/opt/spatial/
--rw-r--r--   0 asymons   (1000) asymons   (1000)     7044 2023-04-07 09:30:21.000000 zigzag-dse-2.3.4/zigzag/classes/opt/spatial/generator.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 12:48:24.991751 zigzag-dse-2.3.4/zigzag/classes/opt/temporal/
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 12:48:25.041751 zigzag-dse-2.3.4/zigzag/classes/opt/temporal/loma/
--rw-r--r--   0 asymons   (1000) asymons   (1000)    11591 2023-04-07 09:29:56.000000 zigzag-dse-2.3.4/zigzag/classes/opt/temporal/loma/engine.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)      489 2023-04-07 09:30:00.000000 zigzag-dse-2.3.4/zigzag/classes/opt/temporal/loma/loop.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)    15479 2023-04-07 09:30:04.000000 zigzag-dse-2.3.4/zigzag/classes/opt/temporal/loma/memory_allocator.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     2837 2023-04-07 09:30:07.000000 zigzag-dse-2.3.4/zigzag/classes/opt/temporal/loma/multipermute.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 12:48:25.041751 zigzag-dse-2.3.4/zigzag/classes/opt/temporal/salsa/
--rw-r--r--   0 asymons   (1000) asymons   (1000)     8726 2023-04-07 09:30:11.000000 zigzag-dse-2.3.4/zigzag/classes/opt/temporal/salsa/engine.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     3616 2023-04-07 09:30:15.000000 zigzag-dse-2.3.4/zigzag/classes/opt/temporal/salsa/state.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 12:48:25.041751 zigzag-dse-2.3.4/zigzag/classes/stages/
--rw-r--r--   0 asymons   (1000) asymons   (1000)     2054 2023-04-07 09:02:40.000000 zigzag-dse-2.3.4/zigzag/classes/stages/CostModelStage.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     1552 2023-04-07 09:03:00.000000 zigzag-dse-2.3.4/zigzag/classes/stages/DumpStage.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     3240 2023-04-07 09:02:56.000000 zigzag-dse-2.3.4/zigzag/classes/stages/GeneralParameterIteratorStage.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     2105 2023-04-07 09:02:49.000000 zigzag-dse-2.3.4/zigzag/classes/stages/LomaStage.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     2163 2023-04-07 09:27:10.000000 zigzag-dse-2.3.4/zigzag/classes/stages/MainInputParserStages.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)      966 2023-04-07 09:03:11.000000 zigzag-dse-2.3.4/zigzag/classes/stages/ONNXModelParserStage.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     1568 2023-04-07 09:03:29.000000 zigzag-dse-2.3.4/zigzag/classes/stages/PlotTemporalMappingsStage.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     6204 2023-04-07 09:03:44.000000 zigzag-dse-2.3.4/zigzag/classes/stages/ReduceStages.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     6260 2023-04-07 09:03:58.000000 zigzag-dse-2.3.4/zigzag/classes/stages/RunOptStages.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     6546 2023-04-07 09:04:04.000000 zigzag-dse-2.3.4/zigzag/classes/stages/SalsaStage.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     6997 2023-04-15 12:05:47.000000 zigzag-dse-2.3.4/zigzag/classes/stages/SaveStage.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     8158 2023-04-07 09:04:25.000000 zigzag-dse-2.3.4/zigzag/classes/stages/SpatialMappingConversionStage.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     3906 2023-04-07 09:05:11.000000 zigzag-dse-2.3.4/zigzag/classes/stages/SpatialMappingGeneratorStage.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     2593 2023-04-07 09:05:30.000000 zigzag-dse-2.3.4/zigzag/classes/stages/Stage.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     4046 2023-04-07 09:05:44.000000 zigzag-dse-2.3.4/zigzag/classes/stages/TemporalOrderingConversionStage.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     1187 2023-04-07 09:05:50.000000 zigzag-dse-2.3.4/zigzag/classes/stages/WorkloadStage.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     2821 2023-04-07 09:28:15.000000 zigzag-dse-2.3.4/zigzag/classes/stages/__init__.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 12:48:25.041751 zigzag-dse-2.3.4/zigzag/classes/workload/
--rw-r--r--   0 asymons   (1000) asymons   (1000)     2468 2023-04-07 09:17:48.000000 zigzag-dse-2.3.4/zigzag/classes/workload/dnn_workload.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     2210 2023-04-07 09:17:53.000000 zigzag-dse-2.3.4/zigzag/classes/workload/dummy_node.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)    21102 2023-04-07 09:19:32.000000 zigzag-dse-2.3.4/zigzag/classes/workload/layer_node.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     1542 2023-04-07 09:18:04.000000 zigzag-dse-2.3.4/zigzag/classes/workload/onnx_workload.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)    14521 2023-04-07 09:18:09.000000 zigzag-dse-2.3.4/zigzag/classes/workload/test_layer_node.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 12:48:25.001751 zigzag-dse-2.3.4/zigzag/inputs/
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 12:48:25.001751 zigzag-dse-2.3.4/zigzag/inputs/examples/
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 12:48:25.041751 zigzag-dse-2.3.4/zigzag/inputs/examples/hardware/
--rw-r--r--   0 asymons   (1000) asymons   (1000)     8448 2023-04-16 14:01:57.000000 zigzag-dse-2.3.4/zigzag/inputs/examples/hardware/Ascend_like.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     5849 2023-04-16 14:01:57.000000 zigzag-dse-2.3.4/zigzag/inputs/examples/hardware/Edge_TPU_like.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     5746 2023-04-16 14:01:57.000000 zigzag-dse-2.3.4/zigzag/inputs/examples/hardware/Eyeriss_like.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     7098 2023-04-16 14:01:57.000000 zigzag-dse-2.3.4/zigzag/inputs/examples/hardware/Meta_prototype.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     5112 2023-04-16 14:01:57.000000 zigzag-dse-2.3.4/zigzag/inputs/examples/hardware/TPU_like.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     7287 2023-04-16 14:01:57.000000 zigzag-dse-2.3.4/zigzag/inputs/examples/hardware/Tesla_NPU_like.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 12:48:25.041751 zigzag-dse-2.3.4/zigzag/inputs/examples/mapping/
--rw-r--r--   0 asymons   (1000) asymons   (1000)      561 2023-04-15 09:48:43.000000 zigzag-dse-2.3.4/zigzag/inputs/examples/mapping/assend_like.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)      196 2023-04-15 09:48:46.000000 zigzag-dse-2.3.4/zigzag/inputs/examples/mapping/default.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)      832 2023-04-15 09:48:50.000000 zigzag-dse-2.3.4/zigzag/inputs/examples/mapping/edge_tpu_like.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)      560 2023-04-15 09:48:52.000000 zigzag-dse-2.3.4/zigzag/inputs/examples/mapping/meta_prototype_like.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)      610 2023-04-15 09:48:56.000000 zigzag-dse-2.3.4/zigzag/inputs/examples/mapping/tesla_npu_like.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)      557 2023-04-15 09:49:08.000000 zigzag-dse-2.3.4/zigzag/inputs/examples/mapping/tpu_like.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 12:48:25.041751 zigzag-dse-2.3.4/zigzag/inputs/examples/workload/
--rw-r--r--   0 asymons   (1000) asymons   (1000)     4067 2023-01-16 14:56:40.000000 zigzag-dse-2.3.4/zigzag/inputs/examples/workload/alexnet.onnx
--rw-r--r--   0 asymons   (1000) asymons   (1000)    71724 2022-12-09 21:20:28.000000 zigzag-dse-2.3.4/zigzag/inputs/examples/workload/mobilenetv2.onnx
--rw-r--r--   0 asymons   (1000) asymons   (1000)    18600 2023-04-15 09:55:05.000000 zigzag-dse-2.3.4/zigzag/inputs/examples/workload/resnet18.onnx
--rw-r--r--   0 asymons   (1000) asymons   (1000)    19065 2023-04-15 09:49:14.000000 zigzag-dse-2.3.4/zigzag/inputs/examples/workload/resnet18.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)      504 2022-10-27 21:43:16.000000 zigzag-dse-2.3.4/zigzag/utils.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 12:48:25.001751 zigzag-dse-2.3.4/zigzag/visualization/
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 12:48:25.041751 zigzag-dse-2.3.4/zigzag/visualization/graph/
--rw-r--r--   0 asymons   (1000) asymons   (1000)     1527 2023-04-15 09:49:36.000000 zigzag-dse-2.3.4/zigzag/visualization/graph/memory_hierarchy.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     1280 2023-04-15 09:49:41.000000 zigzag-dse-2.3.4/zigzag/visualization/graph/workload.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 12:48:25.041751 zigzag-dse-2.3.4/zigzag/visualization/results/
--rw-r--r--   0 asymons   (1000) asymons   (1000)     8773 2023-04-16 16:18:26.000000 zigzag-dse-2.3.4/zigzag/visualization/results/plot_cme.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     3951 2023-04-15 09:49:53.000000 zigzag-dse-2.3.4/zigzag/visualization/results/print_mapping.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 12:48:25.041751 zigzag-dse-2.3.4/zigzag_dse.egg-info/
--rw-r--r--   0 asymons   (1000) asymons   (1000)     8918 2023-04-22 12:48:24.000000 zigzag-dse-2.3.4/zigzag_dse.egg-info/PKG-INFO
--rw-r--r--   0 asymons   (1000) asymons   (1000)     9580 2023-04-22 12:48:24.000000 zigzag-dse-2.3.4/zigzag_dse.egg-info/SOURCES.txt
--rw-r--r--   0 asymons   (1000) asymons   (1000)        1 2023-04-22 12:48:24.000000 zigzag-dse-2.3.4/zigzag_dse.egg-info/dependency_links.txt
--rw-r--r--   0 asymons   (1000) asymons   (1000)       52 2023-04-22 12:48:24.000000 zigzag-dse-2.3.4/zigzag_dse.egg-info/entry_points.txt
--rw-r--r--   0 asymons   (1000) asymons   (1000)      137 2023-04-22 12:48:24.000000 zigzag-dse-2.3.4/zigzag_dse.egg-info/requires.txt
--rw-r--r--   0 asymons   (1000) asymons   (1000)       27 2023-04-22 12:48:24.000000 zigzag-dse-2.3.4/zigzag_dse.egg-info/top_level.txt
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 22:36:10.111489 zigzag-dse-2.3.5/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     1522 2022-06-17 07:16:25.000000 zigzag-dse-2.3.5/LICENSE
+-rw-r--r--   0 asymons   (1000) asymons   (1000)       88 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/MANIFEST.in
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     8918 2023-04-22 22:36:10.111489 zigzag-dse-2.3.5/PKG-INFO
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     6596 2023-03-14 15:21:48.000000 zigzag-dse-2.3.5/README.md
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 22:36:10.041489 zigzag-dse-2.3.5/docs/
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 22:36:10.041489 zigzag-dse-2.3.5/docs/source/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     2594 2023-03-14 15:21:19.000000 zigzag-dse-2.3.5/docs/source/conf.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     1601 2023-04-22 22:36:00.000000 zigzag-dse-2.3.5/pyproject.toml
+-rw-r--r--   0 asymons   (1000) asymons   (1000)       38 2023-04-22 22:36:10.111489 zigzag-dse-2.3.5/setup.cfg
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 22:36:10.051489 zigzag-dse-2.3.5/zigzag/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)       22 2023-04-22 22:36:00.000000 zigzag-dse-2.3.5/zigzag/__init__.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     2497 2022-11-06 07:09:28.000000 zigzag-dse-2.3.5/zigzag/__main__.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     4451 2023-04-15 15:25:43.000000 zigzag-dse-2.3.5/zigzag/api.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 22:36:10.051489 zigzag-dse-2.3.5/zigzag/classes/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)        0 2022-11-06 21:40:40.000000 zigzag-dse-2.3.5/zigzag/classes/__init__.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 22:36:10.051489 zigzag-dse-2.3.5/zigzag/classes/cacti/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      291 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/README.md
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 22:36:10.051489 zigzag-dse-2.3.5/zigzag/classes/cacti/__pycache__/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     3412 2023-04-22 21:31:11.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/__pycache__/cacti_parser.cpython-310.pyc
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 22:36:10.061489 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     6576 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/2DDRAM_Samsung2GbDDR2.cfg
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     6555 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/2DDRAM_micron1Gb.cfg
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     6920 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/3DDRAM_Samsung3D8Gb_extened.cfg
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     5324 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/README
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     9282 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/TSV.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     3322 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/TSV.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    41184 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/Ucache.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     3607 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/Ucache.h
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 22:36:10.061489 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/__pycache__/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    13713 2023-04-16 14:07:27.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/__pycache__/cacti_config_creator.cpython-310.pyc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     5116 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/arbiter.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     2771 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/arbiter.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     2057 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/area.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     2416 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/area.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     8474 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/bank.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     2664 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/bank.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    29279 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/basic_circuit.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     7364 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/basic_circuit.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    11041 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/cache.cfg_temp
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    32713 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/cache_old.cfg.out
+-rwxr-xr-x   0 asymons   (1000) asymons   (1000)  2421320 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/cacti
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      173 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/cacti.i
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     1334 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/cacti.mk
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    25297 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/cacti_config_creator.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     5586 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/cacti_interface.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    27215 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/cacti_interface.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     3569 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/cacti_top.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     7561 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/component.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     2837 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/component.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     9565 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/const.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     5001 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/contention.dat
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     7349 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/crossbar.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     3204 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/crossbar.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     9849 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/ddr3.cfg
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    62337 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/decoder.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     7405 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/decoder.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     3712 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/dram.cfg
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     9750 2023-04-22 22:34:40.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/example_mem_pool.yaml
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    17411 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/extio.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      878 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/extio.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    46185 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/extio_technology.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     9068 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/extio_technology.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    23772 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/htree2.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     3595 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/htree2.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   133713 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/io.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     2116 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/io.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     9850 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/lpddr.cfg
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     7217 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/main.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      407 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/makefile
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    94813 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/mat.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     6122 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/mat.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    16630 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/memcad.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      553 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/memcad.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    11483 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/memcad_parameters.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     4490 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/memcad_parameters.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    29014 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/memorybus.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     5426 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/memorybus.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    19629 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/nuca.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     3306 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/nuca.h
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 22:36:10.081489 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/obj_dbg/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   134304 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/obj_dbg/TSV.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   352744 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/obj_dbg/Ucache.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   157960 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/obj_dbg/arbiter.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   124352 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/obj_dbg/area.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   156624 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/obj_dbg/bank.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   155192 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/obj_dbg/basic_circuit.o
+-rwxr-xr-x   0 asymons   (1000) asymons   (1000)  2421320 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/obj_dbg/cacti
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   175768 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/obj_dbg/cacti_interface.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   159768 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/obj_dbg/component.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   160680 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/obj_dbg/crossbar.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   207224 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/obj_dbg/decoder.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   145592 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/obj_dbg/extio.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   180464 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/obj_dbg/extio_technology.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   178384 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/obj_dbg/htree2.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   411960 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/obj_dbg/io.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   192248 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/obj_dbg/main.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   270320 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/obj_dbg/mat.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   569648 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/obj_dbg/memcad.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   280416 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/obj_dbg/memcad_parameters.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   204480 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/obj_dbg/memorybus.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   256824 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/obj_dbg/nuca.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   313848 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/obj_dbg/parameter.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   124400 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/obj_dbg/powergating.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   175432 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/obj_dbg/router.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   128080 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/obj_dbg/subarray.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   144976 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/obj_dbg/technology.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   228000 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/obj_dbg/uca.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   232752 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/obj_dbg/wire.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   111980 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/parameter.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    20306 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/parameter.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     5286 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/powergating.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     3055 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/powergating.h
+-rwxr-xr-x   0 asymons   (1000) asymons   (1000)     1886 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/regression.test
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    10212 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/router.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     3721 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/router.h
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 22:36:10.081489 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/sample_config_files/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     8781 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/sample_config_files/ddr3_cache.cfg
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     8768 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/sample_config_files/diff_ddr3_cache.cfg
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     8780 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/sample_config_files/lpddr3_cache.cfg
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     8784 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/sample_config_files/wideio_cache.cfg
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 22:36:10.091489 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/self_gen/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     9545 2023-04-22 22:34:40.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/self_gen/cache.cfg
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      579 2023-04-22 22:34:40.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/self_gen/cache.cfg.out
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     8332 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/subarray.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     2542 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/subarray.h
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 22:36:10.091489 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/tech_params/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)       25 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/tech_params/16nm.dat
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    23666 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/tech_params/180nm-old.dat
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     3842 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/tech_params/180nm.dat
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     4575 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/tech_params/22nm.dat
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     4759 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/tech_params/32nm.dat
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     4755 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/tech_params/45nm.dat
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    24571 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/tech_params/65nm-old.dat
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     4758 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/tech_params/65nm.dat
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    24570 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/tech_params/90nm-old.dat
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     4742 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/tech_params/90nm.dat
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    15087 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/technology.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    41317 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/uca.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     4035 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/uca.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     2064 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/version_cacti.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    29856 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/wire.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     4375 2023-03-27 09:38:39.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/wire.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     6110 2023-04-22 12:58:13.000000 zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_parser.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 22:36:10.091489 zigzag-dse-2.3.5/zigzag/classes/cost_model/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    62023 2023-04-16 12:43:30.000000 zigzag-dse-2.3.5/zigzag/classes/cost_model/cost_model.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 22:36:10.041489 zigzag-dse-2.3.5/zigzag/classes/hardware/
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 22:36:10.091489 zigzag-dse-2.3.5/zigzag/classes/hardware/architecture/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     1278 2023-04-16 13:43:29.000000 zigzag-dse-2.3.5/zigzag/classes/hardware/architecture/accelerator.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     9441 2023-04-07 09:22:11.000000 zigzag-dse-2.3.5/zigzag/classes/hardware/architecture/adder_hierarchy.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     6031 2023-04-07 09:22:16.000000 zigzag-dse-2.3.5/zigzag/classes/hardware/architecture/core.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      918 2023-04-07 09:22:20.000000 zigzag-dse-2.3.5/zigzag/classes/hardware/architecture/dimension.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    11764 2023-04-07 09:22:26.000000 zigzag-dse-2.3.5/zigzag/classes/hardware/architecture/memory_hierarchy.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     3351 2023-04-07 09:22:31.000000 zigzag-dse-2.3.5/zigzag/classes/hardware/architecture/memory_instance.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    12231 2023-04-07 09:22:36.000000 zigzag-dse-2.3.5/zigzag/classes/hardware/architecture/memory_level.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     3014 2023-04-07 09:22:40.000000 zigzag-dse-2.3.5/zigzag/classes/hardware/architecture/operational_array.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     1874 2023-04-07 09:22:44.000000 zigzag-dse-2.3.5/zigzag/classes/hardware/architecture/operational_unit.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 22:36:10.041489 zigzag-dse-2.3.5/zigzag/classes/io/
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 22:36:10.091489 zigzag-dse-2.3.5/zigzag/classes/io/accelerator/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     2805 2022-11-06 21:24:03.000000 zigzag-dse-2.3.5/zigzag/classes/io/accelerator/parser.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 22:36:10.091489 zigzag-dse-2.3.5/zigzag/classes/io/onnx/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     9127 2023-04-15 11:49:50.000000 zigzag-dse-2.3.5/zigzag/classes/io/onnx/conv.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      884 2023-04-07 09:12:40.000000 zigzag-dse-2.3.5/zigzag/classes/io/onnx/default.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     5382 2023-04-07 09:12:45.000000 zigzag-dse-2.3.5/zigzag/classes/io/onnx/gemm.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     3679 2023-04-07 09:12:49.000000 zigzag-dse-2.3.5/zigzag/classes/io/onnx/matmul.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     4912 2023-04-07 09:12:53.000000 zigzag-dse-2.3.5/zigzag/classes/io/onnx/model.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     1163 2023-04-07 09:12:58.000000 zigzag-dse-2.3.5/zigzag/classes/io/onnx/parser.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     4391 2023-04-07 09:13:02.000000 zigzag-dse-2.3.5/zigzag/classes/io/onnx/utils.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 22:36:10.091489 zigzag-dse-2.3.5/zigzag/classes/mapping/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    40951 2023-04-07 09:24:31.000000 zigzag-dse-2.3.5/zigzag/classes/mapping/combined_mapping.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      637 2023-04-07 09:24:42.000000 zigzag-dse-2.3.5/zigzag/classes/mapping/loop.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     9386 2023-04-07 09:24:55.000000 zigzag-dse-2.3.5/zigzag/classes/mapping/mapping_assist_funcs.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 22:36:10.091489 zigzag-dse-2.3.5/zigzag/classes/mapping/memory/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)        0 2023-04-07 09:25:08.000000 zigzag-dse-2.3.5/zigzag/classes/mapping/memory/data_layout.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 22:36:10.091489 zigzag-dse-2.3.5/zigzag/classes/mapping/spatial/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     7607 2023-04-07 09:25:03.000000 zigzag-dse-2.3.5/zigzag/classes/mapping/spatial/spatial_mapping.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 22:36:10.091489 zigzag-dse-2.3.5/zigzag/classes/mapping/temporal/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      380 2023-04-07 09:25:12.000000 zigzag-dse-2.3.5/zigzag/classes/mapping/temporal/temporal_loop.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     7412 2023-04-07 09:25:16.000000 zigzag-dse-2.3.5/zigzag/classes/mapping/temporal/temporal_mapping.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 22:36:10.041489 zigzag-dse-2.3.5/zigzag/classes/opt/
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 22:36:10.091489 zigzag-dse-2.3.5/zigzag/classes/opt/spatial/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     7044 2023-04-07 09:30:21.000000 zigzag-dse-2.3.5/zigzag/classes/opt/spatial/generator.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 22:36:10.041489 zigzag-dse-2.3.5/zigzag/classes/opt/temporal/
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 22:36:10.091489 zigzag-dse-2.3.5/zigzag/classes/opt/temporal/loma/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    11591 2023-04-07 09:29:56.000000 zigzag-dse-2.3.5/zigzag/classes/opt/temporal/loma/engine.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      489 2023-04-07 09:30:00.000000 zigzag-dse-2.3.5/zigzag/classes/opt/temporal/loma/loop.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    15479 2023-04-07 09:30:04.000000 zigzag-dse-2.3.5/zigzag/classes/opt/temporal/loma/memory_allocator.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     2837 2023-04-07 09:30:07.000000 zigzag-dse-2.3.5/zigzag/classes/opt/temporal/loma/multipermute.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 22:36:10.101489 zigzag-dse-2.3.5/zigzag/classes/opt/temporal/salsa/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     8726 2023-04-07 09:30:11.000000 zigzag-dse-2.3.5/zigzag/classes/opt/temporal/salsa/engine.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     3616 2023-04-07 09:30:15.000000 zigzag-dse-2.3.5/zigzag/classes/opt/temporal/salsa/state.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 22:36:10.101489 zigzag-dse-2.3.5/zigzag/classes/stages/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     2054 2023-04-07 09:02:40.000000 zigzag-dse-2.3.5/zigzag/classes/stages/CostModelStage.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     1552 2023-04-07 09:03:00.000000 zigzag-dse-2.3.5/zigzag/classes/stages/DumpStage.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     3240 2023-04-07 09:02:56.000000 zigzag-dse-2.3.5/zigzag/classes/stages/GeneralParameterIteratorStage.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     2105 2023-04-07 09:02:49.000000 zigzag-dse-2.3.5/zigzag/classes/stages/LomaStage.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     2163 2023-04-07 09:27:10.000000 zigzag-dse-2.3.5/zigzag/classes/stages/MainInputParserStages.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      966 2023-04-07 09:03:11.000000 zigzag-dse-2.3.5/zigzag/classes/stages/ONNXModelParserStage.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     1568 2023-04-07 09:03:29.000000 zigzag-dse-2.3.5/zigzag/classes/stages/PlotTemporalMappingsStage.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     6204 2023-04-07 09:03:44.000000 zigzag-dse-2.3.5/zigzag/classes/stages/ReduceStages.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     6260 2023-04-07 09:03:58.000000 zigzag-dse-2.3.5/zigzag/classes/stages/RunOptStages.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     6546 2023-04-07 09:04:04.000000 zigzag-dse-2.3.5/zigzag/classes/stages/SalsaStage.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     6997 2023-04-15 12:05:47.000000 zigzag-dse-2.3.5/zigzag/classes/stages/SaveStage.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     8158 2023-04-07 09:04:25.000000 zigzag-dse-2.3.5/zigzag/classes/stages/SpatialMappingConversionStage.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     3906 2023-04-07 09:05:11.000000 zigzag-dse-2.3.5/zigzag/classes/stages/SpatialMappingGeneratorStage.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     2593 2023-04-07 09:05:30.000000 zigzag-dse-2.3.5/zigzag/classes/stages/Stage.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     4046 2023-04-07 09:05:44.000000 zigzag-dse-2.3.5/zigzag/classes/stages/TemporalOrderingConversionStage.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     1187 2023-04-07 09:05:50.000000 zigzag-dse-2.3.5/zigzag/classes/stages/WorkloadStage.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     2821 2023-04-07 09:28:15.000000 zigzag-dse-2.3.5/zigzag/classes/stages/__init__.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 22:36:10.101489 zigzag-dse-2.3.5/zigzag/classes/workload/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     2468 2023-04-07 09:17:48.000000 zigzag-dse-2.3.5/zigzag/classes/workload/dnn_workload.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     2210 2023-04-07 09:17:53.000000 zigzag-dse-2.3.5/zigzag/classes/workload/dummy_node.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    21102 2023-04-07 09:19:32.000000 zigzag-dse-2.3.5/zigzag/classes/workload/layer_node.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     1542 2023-04-07 09:18:04.000000 zigzag-dse-2.3.5/zigzag/classes/workload/onnx_workload.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    14521 2023-04-07 09:18:09.000000 zigzag-dse-2.3.5/zigzag/classes/workload/test_layer_node.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 22:36:10.041489 zigzag-dse-2.3.5/zigzag/inputs/
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 22:36:10.041489 zigzag-dse-2.3.5/zigzag/inputs/examples/
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 22:36:10.101489 zigzag-dse-2.3.5/zigzag/inputs/examples/hardware/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     8448 2023-04-16 14:01:57.000000 zigzag-dse-2.3.5/zigzag/inputs/examples/hardware/Ascend_like.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     5849 2023-04-16 14:01:57.000000 zigzag-dse-2.3.5/zigzag/inputs/examples/hardware/Edge_TPU_like.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     5746 2023-04-16 14:01:57.000000 zigzag-dse-2.3.5/zigzag/inputs/examples/hardware/Eyeriss_like.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     7098 2023-04-16 14:01:57.000000 zigzag-dse-2.3.5/zigzag/inputs/examples/hardware/Meta_prototype.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     5112 2023-04-16 14:01:57.000000 zigzag-dse-2.3.5/zigzag/inputs/examples/hardware/TPU_like.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     7287 2023-04-16 14:01:57.000000 zigzag-dse-2.3.5/zigzag/inputs/examples/hardware/Tesla_NPU_like.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 22:36:10.101489 zigzag-dse-2.3.5/zigzag/inputs/examples/mapping/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      561 2023-04-15 09:48:43.000000 zigzag-dse-2.3.5/zigzag/inputs/examples/mapping/assend_like.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      196 2023-04-15 09:48:46.000000 zigzag-dse-2.3.5/zigzag/inputs/examples/mapping/default.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      832 2023-04-15 09:48:50.000000 zigzag-dse-2.3.5/zigzag/inputs/examples/mapping/edge_tpu_like.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      560 2023-04-15 09:48:52.000000 zigzag-dse-2.3.5/zigzag/inputs/examples/mapping/meta_prototype_like.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      610 2023-04-15 09:48:56.000000 zigzag-dse-2.3.5/zigzag/inputs/examples/mapping/tesla_npu_like.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      557 2023-04-15 09:49:08.000000 zigzag-dse-2.3.5/zigzag/inputs/examples/mapping/tpu_like.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 22:36:10.101489 zigzag-dse-2.3.5/zigzag/inputs/examples/workload/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     4067 2023-01-16 14:56:40.000000 zigzag-dse-2.3.5/zigzag/inputs/examples/workload/alexnet.onnx
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    71724 2022-12-09 21:20:28.000000 zigzag-dse-2.3.5/zigzag/inputs/examples/workload/mobilenetv2.onnx
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    18600 2023-04-15 09:55:05.000000 zigzag-dse-2.3.5/zigzag/inputs/examples/workload/resnet18.onnx
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    19065 2023-04-15 09:49:14.000000 zigzag-dse-2.3.5/zigzag/inputs/examples/workload/resnet18.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      504 2022-10-27 21:43:16.000000 zigzag-dse-2.3.5/zigzag/utils.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 22:36:10.041489 zigzag-dse-2.3.5/zigzag/visualization/
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 22:36:10.101489 zigzag-dse-2.3.5/zigzag/visualization/graph/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     1527 2023-04-15 09:49:36.000000 zigzag-dse-2.3.5/zigzag/visualization/graph/memory_hierarchy.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     1280 2023-04-15 09:49:41.000000 zigzag-dse-2.3.5/zigzag/visualization/graph/workload.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 22:36:10.101489 zigzag-dse-2.3.5/zigzag/visualization/results/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     8773 2023-04-16 16:18:26.000000 zigzag-dse-2.3.5/zigzag/visualization/results/plot_cme.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     3951 2023-04-15 09:49:53.000000 zigzag-dse-2.3.5/zigzag/visualization/results/print_mapping.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-22 22:36:10.101489 zigzag-dse-2.3.5/zigzag_dse.egg-info/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     8918 2023-04-22 22:36:10.000000 zigzag-dse-2.3.5/zigzag_dse.egg-info/PKG-INFO
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     9580 2023-04-22 22:36:10.000000 zigzag-dse-2.3.5/zigzag_dse.egg-info/SOURCES.txt
+-rw-r--r--   0 asymons   (1000) asymons   (1000)        1 2023-04-22 22:36:10.000000 zigzag-dse-2.3.5/zigzag_dse.egg-info/dependency_links.txt
+-rw-r--r--   0 asymons   (1000) asymons   (1000)       52 2023-04-22 22:36:10.000000 zigzag-dse-2.3.5/zigzag_dse.egg-info/entry_points.txt
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      144 2023-04-22 22:36:10.000000 zigzag-dse-2.3.5/zigzag_dse.egg-info/requires.txt
+-rw-r--r--   0 asymons   (1000) asymons   (1000)       27 2023-04-22 22:36:10.000000 zigzag-dse-2.3.5/zigzag_dse.egg-info/top_level.txt
```

### Comparing `zigzag-dse-2.3.4/LICENSE` & `zigzag-dse-2.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/PKG-INFO` & `zigzag-dse-2.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zigzag-dse
-Version: 2.3.4
+Version: 2.3.5
 Summary: ZigZag - Deep Learning Hardware Design Space Exploration
 Author-email: Arne Symons <arne.symons@kuleuven.be>, Linyan Mei <linyan.mei@kuleuven.be>
 License: BSD 3-Clause License
         
         Copyright (c) 2021, ZigZag-Project
         All rights reserved.
```

### Comparing `zigzag-dse-2.3.4/README.md` & `zigzag-dse-2.3.5/README.md`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/docs/source/conf.py` & `zigzag-dse-2.3.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/pyproject.toml` & `zigzag-dse-2.3.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 where = ["."]  # ["."] by default
 include = ["*"]  # ["*"] by default
 exclude = ["inputs*", "outputs*", "docs*"]
 namespaces = true  # true by default
 
 [project]
 name = "zigzag-dse"
-version = "2.3.4"
+version = "2.3.5"
 description = "ZigZag - Deep Learning Hardware Design Space Exploration"
 readme = "README.md"
 authors = [{ name = "Arne Symons", email = "arne.symons@kuleuven.be" }, { name = "Linyan Mei", email = "linyan.mei@kuleuven.be" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python",
@@ -25,14 +25,15 @@
     'numpy',
     'networkx',
     'sympy',
     'matplotlib',
     'onnx',
     'tqdm',
     'multiprocessing_on_dill',
+    'pyyaml',
     'tomli; python_version < "3.11"',
 ]
 requires-python = ">=3.9"
 
 
 [project.optional-dependencies]
 dev = ["bumpver", "pip-tools", "build", "twine"]
@@ -40,15 +41,15 @@
 [project.urls]
 Homepage = "https://github.com/ZigZag-Project/zigzag"
 
 [project.scripts]
 realpython = "zigzag.__main__:main"
 
 [tool.bumpver]
-current_version = "2.3.4"
+current_version = "2.3.5"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `zigzag-dse-2.3.4/zigzag/__main__.py` & `zigzag-dse-2.3.5/zigzag/__main__.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/api.py` & `zigzag-dse-2.3.5/zigzag/api.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/__pycache__/cacti_parser.cpython-310.pyc` & `zigzag-dse-2.3.5/zigzag/classes/cacti/__pycache__/cacti_parser.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Apr 22 12:35:25 2023 UTC, .py size: 6106 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 8dd4 4364 da17 0000  o.........Cd....
+00000000: 6f0d 0d0a 0000 0000 e5d9 4364 de17 0000  o.........Cd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3c00 0000 6400  .....@...s<...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6503  d.l.Z.d.d.l.Z.e.
 00000050: a004 6505 a101 5a06 4700 6402 6403 8400  ..e...Z.G.d.d...
 00000060: 6403 8302 5a07 6401 5300 2904 e900 0000  d...Z.d.S.).....
 00000070: 004e 6300 0000 0000 0000 0000 0000 0000  .Nc.............
@@ -64,151 +64,151 @@
 000003f0: 6670 da0b 6d65 6d6f 7279 5f70 6f6f 6cda  fp..memory_pool.
 00000400: 0869 6e73 7461 6e63 6572 0800 0000 7209  .instancer....r.
 00000410: 0000 0072 0a00 0000 da09 7265 6164 5f63  ...r......read_c
 00000420: 6f73 74da 0a77 7269 7465 5f63 6f73 7472  ost..write_costr
 00000430: 0f00 0000 7210 0000 0072 1100 0000 da0a  ....r....r......
 00000440: 6361 6368 655f 7369 7a65 7203 0000 0072  cache_sizer....r
 00000450: 0300 0000 7205 0000 00da 0b69 7465 6d5f  ....r......item_
-00000460: 6578 6973 7473 1300 0000 7336 0000 000c  exists....s6....
+00000460: 6578 6973 7473 1300 0000 732c 0000 000c  exists....s,....
 00000470: 0b0c 011c ff08 0308 0110 020c 0110 0114  ................
-00000480: 0114 0110 0110 0110 0110 0106 0302 ff06  ................
-00000490: 0202 fe06 0302 fd06 0402 fc06 0502 fb06  ................
-000004a0: 0702 8004 027a 1743 6163 7469 5061 7273  .....z.CactiPars
-000004b0: 6572 2e69 7465 6d5f 6578 6973 7473 630a  er.item_existsc.
-000004c0: 0000 0000 0000 0000 0000 000b 0000 0015  ................
-000004d0: 0000 0043 0000 0073 7200 0000 7400 a001  ...C...sr...t...
-000004e0: 6401 7c09 6402 7402 7c01 8301 6403 7402  d.|.d.t.|...d.t.
-000004f0: 7403 7c02 6404 1b00 8301 8301 6405 7402  t.|.d.......d.t.
-00000500: 7c03 8301 6406 7402 7c04 8301 6407 7402  |...d.t.|...d.t.
-00000510: 7c05 8301 6408 7402 7c06 8301 6409 7402  |...d.t.|...d.t.
-00000520: 7c07 8301 640a 7402 7c08 8301 6712 a101  |...d.t.|...g...
-00000530: 7d0a 7c0a 640b 6b03 7237 7404 640c 7c0a  }.|.d.k.r7t.d.|.
-00000540: 9b00 640d 9d03 8301 8201 6400 5300 290e  ..d.......d.S.).
-00000550: 4e5a 0670 7974 686f 6e7a 0a2d 2d6d 656d  NZ.pythonz.--mem
-00000560: 5f74 7970 657a 0c2d 2d63 6163 6865 5f73  _typez.--cache_s
-00000570: 697a 65e9 0800 0000 7a0e 2d2d 494f 5f62  ize.....z.--IO_b
-00000580: 7573 5f77 6964 7468 7a0c 2d2d 6578 5f72  us_widthz.--ex_r
-00000590: 645f 706f 7274 7a0c 2d2d 6578 5f77 725f  d_portz.--ex_wr_
-000005a0: 706f 7274 7a0c 2d2d 7264 5f77 725f 706f  portz.--rd_wr_po
-000005b0: 7274 7a0c 2d2d 6261 6e6b 5f63 6f75 6e74  rtz.--bank_count
-000005c0: 7a0f 2d2d 6d65 6d5f 706f 6f6c 5f70 6174  z.--mem_pool_pat
-000005d0: 6872 0100 0000 7a2f 4361 6374 6920 7375  hr....z/Cacti su
-000005e0: 6270 726f 6365 7373 2063 616c 6c20 6661  bprocess call fa
-000005f0: 696c 6564 2077 6974 6820 7265 7475 726e  iled with return
-00000600: 2076 616c 7565 20da 012e 2905 da0a 7375   value ...)...su
-00000610: 6270 726f 6365 7373 da04 6361 6c6c da03  bprocess..call..
-00000620: 7374 7272 1600 0000 da11 4368 696c 6450  strr......ChildP
-00000630: 726f 6365 7373 4572 726f 7229 0b72 0400  rocessError).r..
-00000640: 0000 7217 0000 0072 1800 0000 7219 0000  ..r....r....r...
-00000650: 0072 1a00 0000 721b 0000 0072 1c00 0000  .r....r....r....
-00000660: 721d 0000 0072 1e00 0000 da0e 6361 6374  r....r......cact
-00000670: 695f 746f 705f 7061 7468 da01 7072 0300  i_top_path..pr..
-00000680: 0000 7203 0000 0072 0500 0000 da0b 6372  ..r....r......cr
-00000690: 6561 7465 5f69 7465 6d39 0000 0073 3400  eate_item9...s4.
-000006a0: 0000 040f 0202 0201 0201 0601 0201 0e01  ................
-000006b0: 0201 0601 0201 0601 0201 0601 0201 0601  ................
-000006c0: 0201 0601 0201 0601 02ee 04ff 0817 0201  ................
-000006d0: 0a01 04ff 04ff 7a17 4361 6374 6950 6172  ......z.CactiPar
-000006e0: 7365 722e 6372 6561 7465 5f69 7465 6d63  ser.create_itemc
-000006f0: 0a00 0000 0000 0000 0000 0000 1a00 0000  ................
-00000700: 0f00 0000 4300 0000 731e 0200 0074 006a  ....C...s....t.j
-00000710: 01a0 027c 09a1 0173 0e74 0364 017c 099b  ...|...s.t.d.|..
-00000720: 0064 029d 0383 0182 0174 04a0 0564 037c  .d.......t...d.|
-00000730: 029b 0064 047c 039b 009d 04a1 0101 007c  ...d.|.........|
-00000740: 0164 056b 0272 4764 067d 0a74 067c 0264  .d.k.rGd.}.t.|.d
-00000750: 0714 0083 017d 0b74 067c 0383 017d 0c74  .....}.t.|...}.t
-00000760: 04a0 0564 087c 019b 0064 097c 0a9b 0064  ...d.|...d.|...d
-00000770: 0a7c 029b 0064 097c 0b9b 0064 0b7c 039b  .|...d.|...d.|..
-00000780: 0064 097c 0c9b 0064 029d 0da1 0101 007c  .d.|...d.......|
-00000790: 0a7d 017c 0b7d 027c 0c7d 037c 00a0 077c  .}.|.}.|.}.|...|
-000007a0: 017c 027c 037c 047c 057c 067c 077c 08a1  .|.|.|.|.|.|.|..
-000007b0: 0873 607c 00a0 087c 017c 027c 037c 047c  .s`|...|.|.|.|.|
-000007c0: 057c 067c 077c 087c 09a1 0901 0074 097c  .|.|.|.|.....t.|
-000007d0: 0864 0c83 028f 0d7d 0d74 0aa0 0b7c 0da1  .d.....}.t...|..
-000007e0: 017d 0e57 0064 0004 0004 0083 0301 006e  .}.W.d.........n
-000007f0: 0831 0073 7577 0101 0001 0001 0059 0001  .1.suw.......Y..
-00000800: 007c 0e64 006b 0372 f97c 0e44 005d 787d  .|.d.k.r.|.D.]x}
-00000810: 0f74 067c 0e7c 0f19 0064 0d19 0083 017d  .t.|.|...d.....}
-00000820: 107c 0e7c 0f19 0064 0e19 007d 1174 067c  .|.|...d...}.t.|
-00000830: 0e7c 0f19 0064 0f19 0083 017d 127c 0e7c  .|...d.....}.|.|
-00000840: 0f19 0064 1019 0064 1119 0064 1214 007d  ...d...d...d...}
-00000850: 137c 0e7c 0f19 0064 1019 0064 1319 0064  .|.|...d...d...d
-00000860: 1214 007d 1474 067c 0e7c 0f19 0064 1419  ...}.t.|.|...d..
-00000870: 0083 017d 1574 067c 0e7c 0f19 0064 1519  ...}.t.|.|...d..
-00000880: 0083 017d 1674 067c 0e7c 0f19 0064 1619  ...}.t.|.|...d..
-00000890: 0083 017d 1774 067c 0e7c 0f19 0064 1719  ...}.t.|.|...d..
-000008a0: 0083 017d 187c 0e7c 0f19 0064 1819 007d  ...}.|.|...d...}
-000008b0: 197c 017c 196b 0272 f87c 027c 186b 0272  .|.|.k.r.|.|.k.r
-000008c0: f87c 107c 036b 0272 f87c 047c 156b 0272  .|.|.k.r.|.|.k.r
-000008d0: f87c 057c 166b 0272 f87c 067c 176b 0272  .|.|.k.r.|.|.k.r
-000008e0: f87c 187c 107c 107c 137c 147c 117c 127c  .|.|.|.|.|.|.|.|
-000008f0: 157c 167c 1766 0a02 0001 0053 0071 8074  .|.|.f.....S.q.t
-00000900: 0c64 197c 029b 0264 1a7c 039b 0264 1b7c  .d.|...d.|...d.|
-00000910: 049b 0264 1c7c 059b 0264 1d7c 069b 0264  ...d.|...d.|...d
-00000920: 1e7c 079b 029d 0c83 0182 0129 1f4e 7a1e  .|.........).Nz.
-00000930: 4361 6374 6920 746f 7020 6669 6c65 2064  Cacti top file d
-00000940: 6f65 736e 2774 2065 7869 7374 3a20 7227  oesn't exist: r'
-00000950: 0000 007a 2e45 7874 7261 6374 696e 6720  ...z.Extracting 
-00000960: 6d65 6d6f 7279 2063 6f73 7473 2077 6974  memory costs wit
-00000970: 6820 4341 4354 4920 666f 7220 7369 7a65  h CACTI for size
-00000980: 203d 207a 0c20 616e 6420 725f 6277 203d   = z. and r_bw =
-00000990: 205a 0272 66da 0473 7261 6de9 8000 0000   Z.rf..sram.....
-000009a0: 7a05 5479 7065 207a 0420 2d3e 207a 072e  z.Type z. -> z..
-000009b0: 2053 697a 6520 7a05 2e20 4257 2072 0700   Size z.. BW r..
-000009c0: 0000 7208 0000 0072 0900 0000 720a 0000  ..r....r....r...
-000009d0: 0072 0b00 0000 720c 0000 0072 0d00 0000  .r....r....r....
-000009e0: 720e 0000 0072 0f00 0000 7210 0000 0072  r....r....r....r
-000009f0: 1100 0000 7212 0000 00da 0b6d 656d 6f72  ....r......memor
-00000a00: 795f 7479 7065 7a29 4e6f 206d 6174 6368  y_typez)No match
-00000a10: 2069 6e20 4361 6374 6920 6d65 6d6f 7279   in Cacti memory
-00000a20: 2070 6f6f 6c20 666f 756e 6420 7369 7a65   pool found size
-00000a30: 3d7a 072c 2072 5f62 773d 7a09 2c20 725f  =z., r_bw=z., r_
-00000a40: 706f 7274 3d7a 092c 2077 5f70 6f72 743d  port=z., w_port=
-00000a50: 7a0a 2c20 7277 5f70 6f72 743d 7a07 2c20  z., rw_port=z., 
-00000a60: 6261 6e6b 3d29 0dda 026f 73da 0470 6174  bank=)...os..pat
-00000a70: 68da 0665 7869 7374 73da 1146 696c 654e  h..exists..FileN
-00000a80: 6f74 466f 756e 6445 7272 6f72 da06 6c6f  otFoundError..lo
-00000a90: 6767 6572 da04 696e 666f 7216 0000 0072  gger..infor....r
-00000aa0: 2500 0000 722e 0000 0072 1300 0000 7214  %...r....r....r.
-00000ab0: 0000 0072 1500 0000 da13 4d6f 6475 6c65  ...r......Module
-00000ac0: 4e6f 7446 6f75 6e64 4572 726f 7229 1a72  NotFoundError).r
-00000ad0: 0400 0000 7217 0000 0072 1800 0000 7219  ....r....r....r.
-00000ae0: 0000 0072 1a00 0000 721b 0000 0072 1c00  ...r....r....r..
-00000af0: 0000 721d 0000 0072 1e00 0000 722c 0000  ..r....r....r,..
-00000b00: 005a 0c6e 6577 5f6d 656d 5f74 7970 65da  .Z.new_mem_type.
-00000b10: 086e 6577 5f73 697a 655a 086e 6577 5f72  .new_sizeZ.new_r
-00000b20: 5f62 7772 1f00 0000 7220 0000 0072 2100  _bwr....r ...r!.
-00000b30: 0000 7208 0000 0072 0900 0000 720a 0000  ..r....r....r...
-00000b40: 0072 2200 0000 7223 0000 0072 0f00 0000  .r"...r#...r....
-00000b50: 7210 0000 0072 1100 0000 7224 0000 0072  r....r....r$...r
-00000b60: 3100 0000 7203 0000 0072 0300 0000 7205  1...r....r....r.
-00000b70: 0000 00da 0867 6574 5f69 7465 6d64 0000  .....get_itemd..
-00000b80: 0073 8e00 0000 0c0c 1001 0402 0e01 04ff  .s..............
-00000b90: 0804 0401 0c01 0801 0401 2801 04ff 0403  ..........(.....
-00000ba0: 0401 0401 0402 1001 04ff 0403 0201 0201  ................
-00000bb0: 0201 0201 0201 0201 0201 0201 0201 04f7  ................
-00000bc0: 0c0c 0c01 1cff 0803 0801 1002 0c01 1001  ................
-00000bd0: 1401 1401 1001 1001 1001 1001 0c01 0603  ................
-00000be0: 02ff 0602 02fe 0603 02fd 0604 02fc 0605  ................
-00000bf0: 02fb 0606 02fa 020a 0201 0201 0201 0201  ................
-00000c00: 0201 0201 0201 0201 0201 08f6 0280 020e  ................
-00000c10: 2601 04ff 7a14 4361 6374 6950 6172 7365  &...z.CactiParse
-00000c20: 722e 6765 745f 6974 656d 4e29 0fda 085f  r.get_itemN)..._
-00000c30: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
-00000c40: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
-00000c50: 5f72 3200 0000 7233 0000 00da 0764 6972  _r2...r3.....dir
-00000c60: 6e61 6d65 da08 7265 616c 7061 7468 da08  name..realpath..
-00000c70: 5f5f 6669 6c65 5f5f 5a0a 6361 6374 695f  __file__Z.cacti_
-00000c80: 7061 7468 5a0d 4d45 4d5f 504f 4f4c 5f50  pathZ.MEM_POOL_P
-00000c90: 4154 485a 0e43 4143 5449 5f54 4f50 5f50  ATHZ.CACTI_TOP_P
-00000ca0: 4154 4872 0600 0000 7225 0000 0072 2e00  ATHr....r%...r..
-00000cb0: 0000 723a 0000 0072 0300 0000 7203 0000  ..r:...r....r...
-00000cc0: 0072 0300 0000 7205 0000 0072 0200 0000  .r....r....r....
-00000cd0: 0a00 0000 731a 0000 0008 0014 020a 010a  ....s...........
-00000ce0: 0108 0202 0c0a f702 2f02 010a f602 3402  ......../.....4.
-00000cf0: 010e f672 0200 0000 2908 7214 0000 0072  ...r....).r....r
-00000d00: 3200 0000 7228 0000 00da 076c 6f67 6769  2...r(.....loggi
-00000d10: 6e67 da09 6765 744c 6f67 6765 7272 3b00  ng..getLoggerr;.
-00000d20: 0000 7236 0000 0072 0200 0000 7203 0000  ..r6...r....r...
-00000d30: 0072 0300 0000 7203 0000 0072 0500 0000  .r....r....r....
-00000d40: da08 3c6d 6f64 756c 653e 0100 0000 730c  ..<module>....s.
-00000d50: 0000 0008 0008 0108 0108 020a 0212 03    ...............
+00000480: 0114 0110 0110 0110 0110 0108 0308 0108  ................
+00000490: 0108 0108 0106 0202 8004 027a 1743 6163  ...........z.Cac
+000004a0: 7469 5061 7273 6572 2e69 7465 6d5f 6578  tiParser.item_ex
+000004b0: 6973 7473 630a 0000 0000 0000 0000 0000  istsc...........
+000004c0: 000b 0000 0015 0000 0043 0000 0073 7200  .........C...sr.
+000004d0: 0000 7400 a001 6401 7c09 6402 7402 7c01  ..t...d.|.d.t.|.
+000004e0: 8301 6403 7402 7403 7c02 6404 1b00 8301  ..d.t.t.|.d.....
+000004f0: 8301 6405 7402 7c03 8301 6406 7402 7c04  ..d.t.|...d.t.|.
+00000500: 8301 6407 7402 7c05 8301 6408 7402 7c06  ..d.t.|...d.t.|.
+00000510: 8301 6409 7402 7c07 8301 640a 7402 7c08  ..d.t.|...d.t.|.
+00000520: 8301 6712 a101 7d0a 7c0a 640b 6b03 7237  ..g...}.|.d.k.r7
+00000530: 7404 640c 7c0a 9b00 640d 9d03 8301 8201  t.d.|...d.......
+00000540: 6400 5300 290e 4e5a 0670 7974 686f 6e7a  d.S.).NZ.pythonz
+00000550: 0a2d 2d6d 656d 5f74 7970 657a 0c2d 2d63  .--mem_typez.--c
+00000560: 6163 6865 5f73 697a 65e9 0800 0000 7a0e  ache_size.....z.
+00000570: 2d2d 494f 5f62 7573 5f77 6964 7468 7a0c  --IO_bus_widthz.
+00000580: 2d2d 6578 5f72 645f 706f 7274 7a0c 2d2d  --ex_rd_portz.--
+00000590: 6578 5f77 725f 706f 7274 7a0c 2d2d 7264  ex_wr_portz.--rd
+000005a0: 5f77 725f 706f 7274 7a0c 2d2d 6261 6e6b  _wr_portz.--bank
+000005b0: 5f63 6f75 6e74 7a0f 2d2d 6d65 6d5f 706f  _countz.--mem_po
+000005c0: 6f6c 5f70 6174 6872 0100 0000 7a2f 4361  ol_pathr....z/Ca
+000005d0: 6374 6920 7375 6270 726f 6365 7373 2063  cti subprocess c
+000005e0: 616c 6c20 6661 696c 6564 2077 6974 6820  all failed with 
+000005f0: 7265 7475 726e 2076 616c 7565 20da 012e  return value ...
+00000600: 2905 da0a 7375 6270 726f 6365 7373 da04  )...subprocess..
+00000610: 6361 6c6c da03 7374 7272 1600 0000 da11  call..strr......
+00000620: 4368 696c 6450 726f 6365 7373 4572 726f  ChildProcessErro
+00000630: 7229 0b72 0400 0000 7217 0000 0072 1800  r).r....r....r..
+00000640: 0000 7219 0000 0072 1a00 0000 721b 0000  ..r....r....r...
+00000650: 0072 1c00 0000 721d 0000 0072 1e00 0000  .r....r....r....
+00000660: da0e 6361 6374 695f 746f 705f 7061 7468  ..cacti_top_path
+00000670: da01 7072 0300 0000 7203 0000 0072 0500  ..pr....r....r..
+00000680: 0000 da0b 6372 6561 7465 5f69 7465 6d39  ....create_item9
+00000690: 0000 0073 3400 0000 040f 0202 0201 0201  ...s4...........
+000006a0: 0601 0201 0e01 0201 0601 0201 0601 0201  ................
+000006b0: 0601 0201 0601 0201 0601 0201 0601 02ee  ................
+000006c0: 04ff 0817 0201 0a01 04ff 04ff 7a17 4361  ............z.Ca
+000006d0: 6374 6950 6172 7365 722e 6372 6561 7465  ctiParser.create
+000006e0: 5f69 7465 6d63 0a00 0000 0000 0000 0000  _itemc..........
+000006f0: 0000 1a00 0000 0f00 0000 4300 0000 7320  ..........C...s 
+00000700: 0200 0074 006a 01a0 027c 09a1 0173 0e74  ...t.j...|...s.t
+00000710: 0364 017c 099b 0064 029d 0383 0182 0174  .d.|...d.......t
+00000720: 04a0 0564 037c 029b 0064 047c 039b 0064  ...d.|...d.|...d
+00000730: 029d 05a1 0101 007c 0164 056b 0272 4864  .......|.d.k.rHd
+00000740: 067d 0a74 067c 0264 0714 0083 017d 0b74  .}.t.|.d.....}.t
+00000750: 067c 0383 017d 0c74 04a0 0764 087c 019b  .|...}.t...d.|..
+00000760: 0064 097c 0a9b 0064 0a7c 029b 0064 097c  .d.|...d.|...d.|
+00000770: 0b9b 0064 0b7c 039b 0064 097c 0c9b 0064  ...d.|...d.|...d
+00000780: 029d 0da1 0101 007c 0a7d 017c 0b7d 027c  .......|.}.|.}.|
+00000790: 0c7d 037c 00a0 087c 017c 027c 037c 047c  .}.|...|.|.|.|.|
+000007a0: 057c 067c 077c 08a1 0873 617c 00a0 097c  .|.|.|...sa|...|
+000007b0: 017c 027c 037c 047c 057c 067c 077c 087c  .|.|.|.|.|.|.|.|
+000007c0: 09a1 0901 0074 0a7c 0864 0c83 028f 0d7d  .....t.|.d.....}
+000007d0: 0d74 0ba0 0c7c 0da1 017d 0e57 0064 0004  .t...|...}.W.d..
+000007e0: 0004 0083 0301 006e 0831 0073 7677 0101  .......n.1.svw..
+000007f0: 0001 0001 0059 0001 007c 0e64 006b 0372  .....Y...|.d.k.r
+00000800: fa7c 0e44 005d 787d 0f74 067c 0e7c 0f19  .|.D.]x}.t.|.|..
+00000810: 0064 0d19 0083 017d 107c 0e7c 0f19 0064  .d.....}.|.|...d
+00000820: 0e19 007d 1174 067c 0e7c 0f19 0064 0f19  ...}.t.|.|...d..
+00000830: 0083 017d 127c 0e7c 0f19 0064 1019 0064  ...}.|.|...d...d
+00000840: 1119 0064 1214 007d 137c 0e7c 0f19 0064  ...d...}.|.|...d
+00000850: 1019 0064 1319 0064 1214 007d 1474 067c  ...d...d...}.t.|
+00000860: 0e7c 0f19 0064 1419 0083 017d 1574 067c  .|...d.....}.t.|
+00000870: 0e7c 0f19 0064 1519 0083 017d 1674 067c  .|...d.....}.t.|
+00000880: 0e7c 0f19 0064 1619 0083 017d 1774 067c  .|...d.....}.t.|
+00000890: 0e7c 0f19 0064 1719 0083 017d 187c 0e7c  .|...d.....}.|.|
+000008a0: 0f19 0064 1819 007d 197c 017c 196b 0272  ...d...}.|.|.k.r
+000008b0: f97c 027c 186b 0272 f97c 107c 036b 0272  .|.|.k.r.|.|.k.r
+000008c0: f97c 047c 156b 0272 f97c 057c 166b 0272  .|.|.k.r.|.|.k.r
+000008d0: f97c 067c 176b 0272 f97c 187c 107c 107c  .|.|.k.r.|.|.|.|
+000008e0: 137c 147c 117c 127c 157c 167c 1766 0a02  .|.|.|.|.|.|.f..
+000008f0: 0001 0053 0071 8174 0d64 197c 029b 0264  ...S.q.t.d.|...d
+00000900: 1a7c 039b 0264 1b7c 049b 0264 1c7c 059b  .|...d.|...d.|..
+00000910: 0264 1d7c 069b 0264 1e7c 079b 029d 0c83  .d.|...d.|......
+00000920: 0182 0129 1f4e 7a1e 4361 6374 6920 746f  ...).Nz.Cacti to
+00000930: 7020 6669 6c65 2064 6f65 736e 2774 2065  p file doesn't e
+00000940: 7869 7374 3a20 7227 0000 007a 2e45 7874  xist: r'...z.Ext
+00000950: 7261 6374 696e 6720 6d65 6d6f 7279 2063  racting memory c
+00000960: 6f73 7473 2077 6974 6820 4341 4354 4920  osts with CACTI 
+00000970: 666f 7220 7369 7a65 203d 207a 0c20 616e  for size = z. an
+00000980: 6420 725f 6277 203d 205a 0272 66da 0473  d r_bw = Z.rf..s
+00000990: 7261 6de9 8000 0000 7a05 5479 7065 207a  ram.....z.Type z
+000009a0: 0420 2d3e 207a 072e 2053 697a 6520 7a05  . -> z.. Size z.
+000009b0: 2e20 4257 2072 0700 0000 7208 0000 0072  . BW r....r....r
+000009c0: 0900 0000 720a 0000 0072 0b00 0000 720c  ....r....r....r.
+000009d0: 0000 0072 0d00 0000 720e 0000 0072 0f00  ...r....r....r..
+000009e0: 0000 7210 0000 0072 1100 0000 7212 0000  ..r....r....r...
+000009f0: 00da 0b6d 656d 6f72 795f 7479 7065 7a29  ...memory_typez)
+00000a00: 4e6f 206d 6174 6368 2069 6e20 4361 6374  No match in Cact
+00000a10: 6920 6d65 6d6f 7279 2070 6f6f 6c20 666f  i memory pool fo
+00000a20: 756e 6420 7369 7a65 3d7a 072c 2072 5f62  und size=z., r_b
+00000a30: 773d 7a09 2c20 725f 706f 7274 3d7a 092c  w=z., r_port=z.,
+00000a40: 2077 5f70 6f72 743d 7a0a 2c20 7277 5f70   w_port=z., rw_p
+00000a50: 6f72 743d 7a07 2c20 6261 6e6b 3d29 0eda  ort=z., bank=)..
+00000a60: 026f 73da 0470 6174 68da 0665 7869 7374  .os..path..exist
+00000a70: 73da 1146 696c 654e 6f74 466f 756e 6445  s..FileNotFoundE
+00000a80: 7272 6f72 da06 6c6f 6767 6572 da04 696e  rror..logger..in
+00000a90: 666f 7216 0000 00da 0777 6172 6e69 6e67  for......warning
+00000aa0: 7225 0000 0072 2e00 0000 7213 0000 0072  r%...r....r....r
+00000ab0: 1400 0000 7215 0000 00da 134d 6f64 756c  ....r......Modul
+00000ac0: 654e 6f74 466f 756e 6445 7272 6f72 291a  eNotFoundError).
+00000ad0: 7204 0000 0072 1700 0000 7218 0000 0072  r....r....r....r
+00000ae0: 1900 0000 721a 0000 0072 1b00 0000 721c  ....r....r....r.
+00000af0: 0000 0072 1d00 0000 721e 0000 0072 2c00  ...r....r....r,.
+00000b00: 0000 5a0c 6e65 775f 6d65 6d5f 7479 7065  ..Z.new_mem_type
+00000b10: da08 6e65 775f 7369 7a65 5a08 6e65 775f  ..new_sizeZ.new_
+00000b20: 725f 6277 721f 0000 0072 2000 0000 7221  r_bwr....r ...r!
+00000b30: 0000 0072 0800 0000 7209 0000 0072 0a00  ...r....r....r..
+00000b40: 0000 7222 0000 0072 2300 0000 720f 0000  ..r"...r#...r...
+00000b50: 0072 1000 0000 7211 0000 0072 2400 0000  .r....r....r$...
+00000b60: 7231 0000 0072 0300 0000 7203 0000 0072  r1...r....r....r
+00000b70: 0500 0000 da08 6765 745f 6974 656d 6400  ......get_itemd.
+00000b80: 0000 7382 0000 000c 0c10 0104 0210 0104  ..s.............
+00000b90: ff08 0404 010c 0108 0104 0128 0104 ff04  ...........(....
+00000ba0: 0304 0104 0104 0210 0104 ff04 0302 0102  ................
+00000bb0: 0102 0102 0102 0102 0102 0102 0102 0104  ................
+00000bc0: f70c 0c0c 011c ff08 0308 0110 020c 0110  ................
+00000bd0: 0114 0114 0110 0110 0110 0110 010c 0108  ................
+00000be0: 0308 0108 0108 0108 0108 0102 0402 0102  ................
+00000bf0: 0102 0102 0102 0102 0102 0102 0102 0108  ................
+00000c00: f602 8002 0e26 0104 ff7a 1443 6163 7469  .....&...z.Cacti
+00000c10: 5061 7273 6572 2e67 6574 5f69 7465 6d4e  Parser.get_itemN
+00000c20: 290f da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
+00000c30: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
+00000c40: 6e61 6d65 5f5f 7232 0000 0072 3300 0000  name__r2...r3...
+00000c50: da07 6469 726e 616d 65da 0872 6561 6c70  ..dirname..realp
+00000c60: 6174 68da 085f 5f66 696c 655f 5f5a 0a63  ath..__file__Z.c
+00000c70: 6163 7469 5f70 6174 685a 0d4d 454d 5f50  acti_pathZ.MEM_P
+00000c80: 4f4f 4c5f 5041 5448 5a0e 4341 4354 495f  OOL_PATHZ.CACTI_
+00000c90: 544f 505f 5041 5448 7206 0000 0072 2500  TOP_PATHr....r%.
+00000ca0: 0000 722e 0000 0072 3b00 0000 7203 0000  ..r....r;...r...
+00000cb0: 0072 0300 0000 7203 0000 0072 0500 0000  .r....r....r....
+00000cc0: 7202 0000 000a 0000 0073 1a00 0000 0800  r........s......
+00000cd0: 1402 0a01 0a01 0802 020c 0af7 022f 0201  ............./..
+00000ce0: 0af6 0234 0201 0ef6 7202 0000 0029 0872  ...4....r....).r
+00000cf0: 1400 0000 7232 0000 0072 2800 0000 da07  ....r2...r(.....
+00000d00: 6c6f 6767 696e 67da 0967 6574 4c6f 6767  logging..getLogg
+00000d10: 6572 723c 0000 0072 3600 0000 7202 0000  err<...r6...r...
+00000d20: 0072 0300 0000 7203 0000 0072 0300 0000  .r....r....r....
+00000d30: 7205 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00000d40: 0000 0073 0c00 0000 0800 0801 0801 0802  ...s............
+00000d50: 0a02 1203                                ....
```

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/2DDRAM_Samsung2GbDDR2.cfg` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/2DDRAM_Samsung2GbDDR2.cfg`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/2DDRAM_micron1Gb.cfg` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/2DDRAM_micron1Gb.cfg`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/3DDRAM_Samsung3D8Gb_extened.cfg` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/3DDRAM_Samsung3D8Gb_extened.cfg`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/README` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/README`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/TSV.cc` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/TSV.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/TSV.h` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/TSV.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/Ucache.cc` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/Ucache.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/Ucache.h` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/Ucache.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/__pycache__/cacti_config_creator.cpython-310.pyc` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/__pycache__/cacti_config_creator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/arbiter.cc` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/arbiter.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/arbiter.h` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/arbiter.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/area.cc` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/area.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/area.h` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/area.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/bank.cc` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/bank.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/bank.h` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/bank.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/basic_circuit.cc` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/basic_circuit.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/basic_circuit.h` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/basic_circuit.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/cache.cfg_temp` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/cache.cfg_temp`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/cache_old.cfg.out` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/cache_old.cfg.out`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/cacti` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/cacti`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/cacti.mk` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/cacti.mk`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/cacti_config_creator.py` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/cacti_config_creator.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/cacti_interface.cc` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/cacti_interface.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/cacti_interface.h` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/cacti_interface.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/cacti_top.py` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/cacti_top.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/component.cc` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/component.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/component.h` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/component.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/const.h` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/const.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/contention.dat` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/contention.dat`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/crossbar.cc` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/crossbar.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/crossbar.h` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/crossbar.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/ddr3.cfg` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/ddr3.cfg`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/decoder.cc` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/decoder.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/decoder.h` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/decoder.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/dram.cfg` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/dram.cfg`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/example_mem_pool.yaml` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/example_mem_pool.yaml`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/extio.cc` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/extio.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/extio.h` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/extio.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/extio_technology.cc` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/extio_technology.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/extio_technology.h` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/extio_technology.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/htree2.cc` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/htree2.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/htree2.h` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/htree2.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/io.cc` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/io.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/io.h` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/io.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/lpddr.cfg` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/lpddr.cfg`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/main.cc` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/main.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/mat.cc` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/mat.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/mat.h` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/mat.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/memcad.cc` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/memcad.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/memcad.h` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/memcad.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/memcad_parameters.cc` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/memcad_parameters.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/memcad_parameters.h` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/memcad_parameters.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/memorybus.cc` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/memorybus.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/memorybus.h` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/memorybus.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/nuca.cc` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/nuca.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/nuca.h` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/nuca.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/obj_dbg/TSV.o` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/obj_dbg/TSV.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/obj_dbg/Ucache.o` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/obj_dbg/Ucache.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/obj_dbg/arbiter.o` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/obj_dbg/arbiter.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/obj_dbg/area.o` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/obj_dbg/area.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/obj_dbg/bank.o` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/obj_dbg/bank.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/obj_dbg/basic_circuit.o` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/obj_dbg/basic_circuit.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/obj_dbg/cacti` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/obj_dbg/cacti`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/obj_dbg/cacti_interface.o` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/obj_dbg/cacti_interface.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/obj_dbg/component.o` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/obj_dbg/component.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/obj_dbg/crossbar.o` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/obj_dbg/crossbar.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/obj_dbg/decoder.o` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/obj_dbg/decoder.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/obj_dbg/extio.o` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/obj_dbg/extio.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/obj_dbg/extio_technology.o` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/obj_dbg/extio_technology.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/obj_dbg/htree2.o` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/obj_dbg/htree2.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/obj_dbg/io.o` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/obj_dbg/io.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/obj_dbg/main.o` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/obj_dbg/main.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/obj_dbg/mat.o` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/obj_dbg/mat.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/obj_dbg/memcad.o` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/obj_dbg/memcad.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/obj_dbg/memcad_parameters.o` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/obj_dbg/memcad_parameters.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/obj_dbg/memorybus.o` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/obj_dbg/memorybus.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/obj_dbg/nuca.o` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/obj_dbg/nuca.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/obj_dbg/parameter.o` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/obj_dbg/parameter.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/obj_dbg/powergating.o` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/obj_dbg/powergating.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/obj_dbg/router.o` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/obj_dbg/router.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/obj_dbg/subarray.o` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/obj_dbg/subarray.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/obj_dbg/technology.o` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/obj_dbg/technology.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/obj_dbg/uca.o` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/obj_dbg/uca.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/obj_dbg/wire.o` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/obj_dbg/wire.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/parameter.cc` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/parameter.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/parameter.h` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/parameter.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/powergating.cc` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/powergating.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/powergating.h` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/powergating.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/regression.test` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/regression.test`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/router.cc` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/router.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/router.h` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/router.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/sample_config_files/ddr3_cache.cfg` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/sample_config_files/ddr3_cache.cfg`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/sample_config_files/diff_ddr3_cache.cfg` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/sample_config_files/diff_ddr3_cache.cfg`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/sample_config_files/lpddr3_cache.cfg` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/sample_config_files/lpddr3_cache.cfg`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/sample_config_files/wideio_cache.cfg` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/sample_config_files/wideio_cache.cfg`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/self_gen/cache.cfg` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/self_gen/cache.cfg`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/self_gen/cache.cfg.out` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/self_gen/cache.cfg.out`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/subarray.cc` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/subarray.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/subarray.h` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/subarray.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/tech_params/180nm-old.dat` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/tech_params/180nm-old.dat`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/tech_params/180nm.dat` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/tech_params/180nm.dat`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/tech_params/22nm.dat` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/tech_params/22nm.dat`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/tech_params/32nm.dat` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/tech_params/32nm.dat`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/tech_params/45nm.dat` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/tech_params/45nm.dat`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/tech_params/65nm-old.dat` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/tech_params/65nm-old.dat`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/tech_params/65nm.dat` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/tech_params/65nm.dat`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/tech_params/90nm-old.dat` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/tech_params/90nm-old.dat`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/tech_params/90nm.dat` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/tech_params/90nm.dat`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/technology.cc` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/technology.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/uca.cc` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/uca.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/uca.h` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/uca.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/version_cacti.h` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/version_cacti.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/wire.cc` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/wire.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_master/wire.h` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_master/wire.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cacti/cacti_parser.py` & `zigzag-dse-2.3.5/zigzag/classes/cacti/cacti_parser.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/cost_model/cost_model.py` & `zigzag-dse-2.3.5/zigzag/classes/cost_model/cost_model.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/hardware/architecture/accelerator.py` & `zigzag-dse-2.3.5/zigzag/classes/hardware/architecture/accelerator.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/hardware/architecture/adder_hierarchy.py` & `zigzag-dse-2.3.5/zigzag/classes/hardware/architecture/adder_hierarchy.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/hardware/architecture/core.py` & `zigzag-dse-2.3.5/zigzag/classes/hardware/architecture/core.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/hardware/architecture/dimension.py` & `zigzag-dse-2.3.5/zigzag/classes/hardware/architecture/dimension.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/hardware/architecture/memory_hierarchy.py` & `zigzag-dse-2.3.5/zigzag/classes/hardware/architecture/memory_hierarchy.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/hardware/architecture/memory_instance.py` & `zigzag-dse-2.3.5/zigzag/classes/hardware/architecture/memory_instance.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/hardware/architecture/memory_level.py` & `zigzag-dse-2.3.5/zigzag/classes/hardware/architecture/memory_level.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/hardware/architecture/operational_array.py` & `zigzag-dse-2.3.5/zigzag/classes/hardware/architecture/operational_array.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/hardware/architecture/operational_unit.py` & `zigzag-dse-2.3.5/zigzag/classes/hardware/architecture/operational_unit.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/io/accelerator/parser.py` & `zigzag-dse-2.3.5/zigzag/classes/io/accelerator/parser.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/io/onnx/conv.py` & `zigzag-dse-2.3.5/zigzag/classes/io/onnx/conv.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/io/onnx/default.py` & `zigzag-dse-2.3.5/zigzag/classes/io/onnx/default.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/io/onnx/gemm.py` & `zigzag-dse-2.3.5/zigzag/classes/io/onnx/gemm.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/io/onnx/matmul.py` & `zigzag-dse-2.3.5/zigzag/classes/io/onnx/matmul.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/io/onnx/model.py` & `zigzag-dse-2.3.5/zigzag/classes/io/onnx/model.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/io/onnx/parser.py` & `zigzag-dse-2.3.5/zigzag/classes/io/onnx/parser.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/io/onnx/utils.py` & `zigzag-dse-2.3.5/zigzag/classes/io/onnx/utils.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/mapping/combined_mapping.py` & `zigzag-dse-2.3.5/zigzag/classes/mapping/combined_mapping.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/mapping/loop.py` & `zigzag-dse-2.3.5/zigzag/classes/mapping/loop.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/mapping/mapping_assist_funcs.py` & `zigzag-dse-2.3.5/zigzag/classes/mapping/mapping_assist_funcs.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/mapping/spatial/spatial_mapping.py` & `zigzag-dse-2.3.5/zigzag/classes/mapping/spatial/spatial_mapping.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/mapping/temporal/temporal_mapping.py` & `zigzag-dse-2.3.5/zigzag/classes/mapping/temporal/temporal_mapping.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/opt/spatial/generator.py` & `zigzag-dse-2.3.5/zigzag/classes/opt/spatial/generator.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/opt/temporal/loma/engine.py` & `zigzag-dse-2.3.5/zigzag/classes/opt/temporal/loma/engine.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/opt/temporal/loma/memory_allocator.py` & `zigzag-dse-2.3.5/zigzag/classes/opt/temporal/loma/memory_allocator.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/opt/temporal/loma/multipermute.py` & `zigzag-dse-2.3.5/zigzag/classes/opt/temporal/loma/multipermute.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/opt/temporal/salsa/engine.py` & `zigzag-dse-2.3.5/zigzag/classes/opt/temporal/salsa/engine.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/opt/temporal/salsa/state.py` & `zigzag-dse-2.3.5/zigzag/classes/opt/temporal/salsa/state.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/stages/CostModelStage.py` & `zigzag-dse-2.3.5/zigzag/classes/stages/CostModelStage.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/stages/DumpStage.py` & `zigzag-dse-2.3.5/zigzag/classes/stages/DumpStage.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/stages/GeneralParameterIteratorStage.py` & `zigzag-dse-2.3.5/zigzag/classes/stages/GeneralParameterIteratorStage.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/stages/LomaStage.py` & `zigzag-dse-2.3.5/zigzag/classes/stages/LomaStage.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/stages/MainInputParserStages.py` & `zigzag-dse-2.3.5/zigzag/classes/stages/MainInputParserStages.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/stages/ONNXModelParserStage.py` & `zigzag-dse-2.3.5/zigzag/classes/stages/ONNXModelParserStage.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/stages/PlotTemporalMappingsStage.py` & `zigzag-dse-2.3.5/zigzag/classes/stages/PlotTemporalMappingsStage.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/stages/ReduceStages.py` & `zigzag-dse-2.3.5/zigzag/classes/stages/ReduceStages.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/stages/RunOptStages.py` & `zigzag-dse-2.3.5/zigzag/classes/stages/RunOptStages.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/stages/SalsaStage.py` & `zigzag-dse-2.3.5/zigzag/classes/stages/SalsaStage.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/stages/SaveStage.py` & `zigzag-dse-2.3.5/zigzag/classes/stages/SaveStage.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/stages/SpatialMappingConversionStage.py` & `zigzag-dse-2.3.5/zigzag/classes/stages/SpatialMappingConversionStage.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/stages/SpatialMappingGeneratorStage.py` & `zigzag-dse-2.3.5/zigzag/classes/stages/SpatialMappingGeneratorStage.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/stages/Stage.py` & `zigzag-dse-2.3.5/zigzag/classes/stages/Stage.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/stages/TemporalOrderingConversionStage.py` & `zigzag-dse-2.3.5/zigzag/classes/stages/TemporalOrderingConversionStage.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/stages/WorkloadStage.py` & `zigzag-dse-2.3.5/zigzag/classes/stages/WorkloadStage.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/stages/__init__.py` & `zigzag-dse-2.3.5/zigzag/classes/stages/__init__.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/workload/dnn_workload.py` & `zigzag-dse-2.3.5/zigzag/classes/workload/dnn_workload.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/workload/dummy_node.py` & `zigzag-dse-2.3.5/zigzag/classes/workload/dummy_node.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/workload/layer_node.py` & `zigzag-dse-2.3.5/zigzag/classes/workload/layer_node.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/workload/onnx_workload.py` & `zigzag-dse-2.3.5/zigzag/classes/workload/onnx_workload.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/classes/workload/test_layer_node.py` & `zigzag-dse-2.3.5/zigzag/classes/workload/test_layer_node.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/inputs/examples/hardware/Ascend_like.py` & `zigzag-dse-2.3.5/zigzag/inputs/examples/hardware/Ascend_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/inputs/examples/hardware/Edge_TPU_like.py` & `zigzag-dse-2.3.5/zigzag/inputs/examples/hardware/Edge_TPU_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/inputs/examples/hardware/Eyeriss_like.py` & `zigzag-dse-2.3.5/zigzag/inputs/examples/hardware/Eyeriss_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/inputs/examples/hardware/Meta_prototype.py` & `zigzag-dse-2.3.5/zigzag/inputs/examples/hardware/Meta_prototype.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/inputs/examples/hardware/TPU_like.py` & `zigzag-dse-2.3.5/zigzag/inputs/examples/hardware/TPU_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/inputs/examples/hardware/Tesla_NPU_like.py` & `zigzag-dse-2.3.5/zigzag/inputs/examples/hardware/Tesla_NPU_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/inputs/examples/mapping/assend_like.py` & `zigzag-dse-2.3.5/zigzag/inputs/examples/mapping/assend_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/inputs/examples/mapping/edge_tpu_like.py` & `zigzag-dse-2.3.5/zigzag/inputs/examples/mapping/edge_tpu_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/inputs/examples/mapping/meta_prototype_like.py` & `zigzag-dse-2.3.5/zigzag/inputs/examples/mapping/meta_prototype_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/inputs/examples/mapping/tesla_npu_like.py` & `zigzag-dse-2.3.5/zigzag/inputs/examples/mapping/tesla_npu_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/inputs/examples/mapping/tpu_like.py` & `zigzag-dse-2.3.5/zigzag/inputs/examples/mapping/tpu_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/inputs/examples/workload/alexnet.onnx` & `zigzag-dse-2.3.5/zigzag/inputs/examples/workload/alexnet.onnx`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/inputs/examples/workload/mobilenetv2.onnx` & `zigzag-dse-2.3.5/zigzag/inputs/examples/workload/mobilenetv2.onnx`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/inputs/examples/workload/resnet18.onnx` & `zigzag-dse-2.3.5/zigzag/inputs/examples/workload/resnet18.onnx`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/inputs/examples/workload/resnet18.py` & `zigzag-dse-2.3.5/zigzag/inputs/examples/workload/resnet18.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/visualization/graph/memory_hierarchy.py` & `zigzag-dse-2.3.5/zigzag/visualization/graph/memory_hierarchy.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/visualization/graph/workload.py` & `zigzag-dse-2.3.5/zigzag/visualization/graph/workload.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/visualization/results/plot_cme.py` & `zigzag-dse-2.3.5/zigzag/visualization/results/plot_cme.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag/visualization/results/print_mapping.py` & `zigzag-dse-2.3.5/zigzag/visualization/results/print_mapping.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.4/zigzag_dse.egg-info/PKG-INFO` & `zigzag-dse-2.3.5/zigzag_dse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zigzag-dse
-Version: 2.3.4
+Version: 2.3.5
 Summary: ZigZag - Deep Learning Hardware Design Space Exploration
 Author-email: Arne Symons <arne.symons@kuleuven.be>, Linyan Mei <linyan.mei@kuleuven.be>
 License: BSD 3-Clause License
         
         Copyright (c) 2021, ZigZag-Project
         All rights reserved.
```

### Comparing `zigzag-dse-2.3.4/zigzag_dse.egg-info/SOURCES.txt` & `zigzag-dse-2.3.5/zigzag_dse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

