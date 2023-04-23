# Comparing `tmp/cvxpygen-0.2.2.tar.gz` & `tmp/cvxpygen-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxpygen-0.2.2.tar", last modified: Sun Apr  2 15:35:37 2023, max compression
+gzip compressed data, was "cvxpygen-0.2.3.tar", last modified: Sun Apr 23 15:22:51 2023, max compression
```

## Comparing `cvxpygen-0.2.2.tar` & `cvxpygen-0.2.3.tar`

### file list

```diff
@@ -1,205 +1,209 @@
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-02 15:35:37.721787 cvxpygen-0.2.2/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    11349 2022-02-24 20:19:58.000000 cvxpygen-0.2.2/LICENSE
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1051 2022-03-18 03:22:21.000000 cvxpygen-0.2.2/MANIFEST.in
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     8461 2023-04-02 15:35:37.722114 cvxpygen-0.2.2/PKG-INFO
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     8042 2023-04-02 14:37:32.000000 cvxpygen-0.2.2/README.md
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-02 15:35:37.532602 cvxpygen-0.2.2/cvxpygen/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)        0 2022-02-24 05:57:25.000000 cvxpygen-0.2.2/cvxpygen/__init__.py
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    33467 2023-04-02 15:35:19.000000 cvxpygen-0.2.2/cvxpygen/cpg.py
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-02 15:35:37.518207 cvxpygen-0.2.2/cvxpygen/solvers/
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-02 15:35:37.549084 cvxpygen-0.2.2/cvxpygen/solvers/ecos/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     6148 2021-11-04 03:37:05.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/.DS_Store
--rw-r--r--   0 maximilianschaller   (501) staff       (20)       87 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/.bumpversion.cfg
--rw-r--r--   0 maximilianschaller   (501) staff       (20)       42 2022-02-23 21:43:27.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/.git
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      296 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/.gitignore
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      477 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/.travis.yml
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     4753 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/CMakeLists.txt
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     7272 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/CONTRIBUTING.md
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    35147 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/COPYING
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     3377 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/Makefile
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     4290 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/README.md
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    86113 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/README.pdf
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1476 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/ecos.mk
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-02 15:35:37.552049 cvxpygen-0.2.2/cvxpygen/solvers/ecos/ecos_bb/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    40478 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/ecos_bb/ecos_bb.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    11665 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/ecos_bb/ecos_bb_preproc.c
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-02 15:35:37.516556 cvxpygen-0.2.2/cvxpygen/solvers/ecos/external/
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-02 15:35:37.553071 cvxpygen-0.2.2/cvxpygen/solvers/ecos/external/SuiteSparse_config/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     6482 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/external/SuiteSparse_config/SuiteSparse_config.h
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-02 15:35:37.554890 cvxpygen-0.2.2/cvxpygen/solvers/ecos/external/amd/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     2027 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/external/amd/Makefile
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     8897 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/external/amd/README.txt
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-02 15:35:37.557753 cvxpygen-0.2.2/cvxpygen/solvers/ecos/external/amd/include/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    18328 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/external/amd/include/amd.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     9097 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/external/amd/include/amd_internal.h
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-02 15:35:37.586012 cvxpygen-0.2.2/cvxpygen/solvers/ecos/external/amd/src/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     5710 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/external/amd/src/amd_1.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    64873 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/external/amd/src/amd_2.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     4877 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/external/amd/src/amd_aat.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1786 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/external/amd/src/amd_control.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1253 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/external/amd/src/amd_defaults.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     5012 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/external/amd/src/amd_dump.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     3181 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/external/amd/src/amd_global.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     4173 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/external/amd/src/amd_info.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     5913 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/external/amd/src/amd_order.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     3703 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/external/amd/src/amd_post_tree.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     5509 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/external/amd/src/amd_postorder.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     3808 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/external/amd/src/amd_preprocess.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     2980 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/external/amd/src/amd_valid.c
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-02 15:35:37.590164 cvxpygen-0.2.2/cvxpygen/solvers/ecos/external/ldl/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      763 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/external/ldl/Makefile
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     5779 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/external/ldl/README.txt
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-02 15:35:37.597198 cvxpygen-0.2.2/cvxpygen/solvers/ecos/external/ldl/include/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     3988 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/external/ldl/include/ldl.h
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-02 15:35:37.599077 cvxpygen-0.2.2/cvxpygen/solvers/ecos/external/ldl/src/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    20401 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/external/ldl/src/ldl.c
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-02 15:35:37.617670 cvxpygen-0.2.2/cvxpygen/solvers/ecos/include/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     6290 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/include/cone.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1332 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/include/ctrlc.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    82553 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/include/data.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    12623 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/include/ecos.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     6689 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/include/ecos_bb.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1359 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/include/equil.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     2804 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/include/expcone.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     3882 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/include/glblopts.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     4968 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/include/kkt.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     2712 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/include/spla.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     3241 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/include/splamm.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1717 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/include/timer.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      822 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/include/wright_omega.h
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-02 15:35:37.629986 cvxpygen-0.2.2/cvxpygen/solvers/ecos/src/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    15297 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/src/cone.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     2721 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/src/ctrlc.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    54621 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/src/ecos.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    10355 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/src/equil.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     5076 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/src/expcone.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    14221 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/src/kkt.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    32391 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/src/preproc.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     3510 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/src/runecos.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     4039 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/src/runecos_exp.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     4091 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/src/spla.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     9590 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/src/splamm.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     2578 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/src/timer.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1962 2021-10-28 22:01:39.000000 cvxpygen-0.2.2/cvxpygen/solvers/ecos/src/wright_omega.c
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-02 15:35:37.630834 cvxpygen-0.2.2/cvxpygen/solvers/osqp-python/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    11357 2021-11-03 20:08:49.000000 cvxpygen-0.2.2/cvxpygen/solvers/osqp-python/LICENSE
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-02 15:35:37.640210 cvxpygen-0.2.2/cvxpygen/solvers/scs/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     6148 2022-02-23 21:12:10.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/.DS_Store
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      296 2022-03-01 03:33:41.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/.bumpversion.cfg
--rw-r--r--   0 maximilianschaller   (501) staff       (20)       41 2022-02-23 21:43:27.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/.git
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      488 2022-03-01 03:33:41.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/.gitignore
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1009 2022-03-01 03:33:41.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/CITATION.cff
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    11683 2022-03-01 03:33:41.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/CMakeLists.txt
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1110 2021-11-08 20:11:48.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/LICENSE.txt
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     7382 2022-03-01 03:33:41.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/Makefile
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      922 2022-03-01 03:33:41.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/README.md
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-02 15:35:37.644932 cvxpygen-0.2.2/cvxpygen/solvers/scs/cmake/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     8748 2021-11-08 20:11:48.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/cmake/AddInstallRPATHSupport.cmake
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     2499 2021-11-08 20:11:48.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/cmake/AddUninstallTarget.cmake
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    28861 2021-11-08 20:11:48.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/cmake/InstallBasicPackageFiles.cmake
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      286 2022-03-01 03:33:41.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/cmake/scs_types.h.in
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-02 15:35:37.661145 cvxpygen-0.2.2/cvxpygen/solvers/scs/include/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     3035 2022-03-01 03:33:41.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/include/aa.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1611 2022-03-01 03:33:41.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/include/cones.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      581 2021-11-08 20:11:48.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/include/ctrlc.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     5119 2022-03-01 03:33:41.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/include/glbopts.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      804 2022-03-01 03:33:41.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/include/linalg.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     2193 2022-03-01 03:33:41.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/include/linsys.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      493 2022-03-01 03:33:41.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/include/normalize.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      571 2022-03-01 03:33:41.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/include/rw.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    10042 2022-03-01 03:33:41.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/include/scs.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1010 2021-11-08 20:11:48.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/include/scs_blas.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      437 2022-03-01 03:33:41.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/include/scs_types.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     2747 2022-03-01 03:33:41.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/include/scs_work.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1217 2022-03-01 03:33:41.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/include/util.h
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-02 15:35:37.664827 cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-02 15:35:37.520488 cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/cpu/
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-02 15:35:37.666403 cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/cpu/direct/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    11554 2022-03-01 03:33:41.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/cpu/direct/private.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      768 2022-03-01 03:33:41.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/cpu/direct/private.h
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-02 15:35:37.668019 cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/cpu/indirect/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     9228 2022-03-01 03:33:41.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/cpu/indirect/private.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      681 2022-03-01 03:33:41.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/cpu/indirect/private.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     2586 2022-03-01 03:33:41.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/csparse.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      995 2021-11-08 23:08:19.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/csparse.h
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-02 15:35:37.521699 cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/external/
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-02 15:35:37.684080 cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/external/amd/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     2068 2022-03-01 03:33:41.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/external/amd/LICENSE.txt
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    14798 2022-03-01 03:33:41.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/external/amd/SuiteSparse_config.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     9151 2022-03-01 03:33:41.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/external/amd/SuiteSparse_config.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    17956 2021-11-08 20:11:48.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/external/amd/amd.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     5716 2021-11-08 20:11:48.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/external/amd/amd_1.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    64847 2021-11-08 20:11:48.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/external/amd/amd_2.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     4868 2021-11-08 20:11:48.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/external/amd/amd_aat.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1876 2021-11-08 20:11:48.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/external/amd/amd_control.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1259 2021-11-08 20:11:48.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/external/amd/amd_defaults.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     5012 2021-11-08 20:11:48.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/external/amd/amd_dump.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      941 2021-11-08 20:11:48.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/external/amd/amd_global.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     4299 2021-11-08 20:11:48.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/external/amd/amd_info.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     7706 2021-11-08 23:08:19.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/external/amd/amd_internal.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     6084 2022-03-01 03:33:41.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/external/amd/amd_order.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     3703 2021-11-08 20:11:48.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/external/amd/amd_post_tree.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     5509 2021-11-08 20:11:48.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/external/amd/amd_postorder.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     3808 2021-11-08 20:11:48.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/external/amd/amd_preprocess.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     2980 2021-11-08 20:11:48.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/external/amd/amd_valid.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      528 2021-11-08 20:11:48.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/external/amd/changes
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-02 15:35:37.688771 cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/external/qdldl/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    11357 2021-11-08 20:11:48.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/external/qdldl/LICENSE
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     4865 2021-11-08 20:11:48.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/external/qdldl/README.md
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      210 2021-11-08 23:08:19.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/external/qdldl/changes
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     7683 2021-11-08 23:08:19.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/external/qdldl/qdldl.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     6397 2021-11-08 23:08:19.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/external/qdldl/qdldl.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      533 2021-11-08 23:08:19.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/external/qdldl/qdldl_types.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    12027 2022-03-01 03:33:41.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/scs_matrix.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1839 2022-03-01 03:33:41.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/scs_matrix.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     4444 2022-03-01 03:33:41.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/scs.mk
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-02 15:35:37.700370 cvxpygen-0.2.2/cvxpygen/solvers/scs/src/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    14893 2022-03-01 03:33:41.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/src/aa.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    26617 2022-03-01 03:33:41.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/src/cones.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1770 2021-11-08 23:08:19.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/src/ctrlc.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     3996 2022-03-01 03:33:41.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/src/linalg.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     2556 2022-03-01 03:33:41.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/src/normalize.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    13982 2022-03-01 03:33:41.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/src/rw.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    39399 2022-03-01 03:33:41.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/src/scs.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      147 2022-03-01 03:33:41.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/src/scs_version.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     3529 2022-03-01 03:33:41.000000 cvxpygen-0.2.2/cvxpygen/solvers/scs/src/util.c
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-02 15:35:37.704557 cvxpygen-0.2.2/cvxpygen/template/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1649 2022-02-11 21:46:09.000000 cvxpygen-0.2.2/cvxpygen/template/CMakeLists.txt
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    11349 2022-02-24 20:19:58.000000 cvxpygen-0.2.2/cvxpygen/template/LICENSE
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     7450 2023-04-02 14:37:32.000000 cvxpygen-0.2.2/cvxpygen/template/README.html
--rw-r--r--   0 maximilianschaller   (501) staff       (20)        0 2023-04-02 15:35:19.000000 cvxpygen-0.2.2/cvxpygen/template/__init__.py
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     3968 2022-02-11 21:37:48.000000 cvxpygen-0.2.2/cvxpygen/template/setup.py
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    79351 2023-04-02 14:37:32.000000 cvxpygen-0.2.2/cvxpygen/utils.py
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-02 15:35:37.536206 cvxpygen-0.2.2/cvxpygen.egg-info/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     8461 2023-04-02 15:35:37.000000 cvxpygen-0.2.2/cvxpygen.egg-info/PKG-INFO
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     6497 2023-04-02 15:35:37.000000 cvxpygen-0.2.2/cvxpygen.egg-info/SOURCES.txt
--rw-r--r--   0 maximilianschaller   (501) staff       (20)        1 2023-04-02 15:35:37.000000 cvxpygen-0.2.2/cvxpygen.egg-info/dependency_links.txt
--rw-r--r--   0 maximilianschaller   (501) staff       (20)       94 2023-04-02 15:35:37.000000 cvxpygen-0.2.2/cvxpygen.egg-info/requires.txt
--rw-r--r--   0 maximilianschaller   (501) staff       (20)       24 2023-04-02 15:35:37.000000 cvxpygen-0.2.2/cvxpygen.egg-info/top_level.txt
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      144 2023-01-23 08:33:33.000000 cvxpygen-0.2.2/environment.yml
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-02 15:35:37.713344 cvxpygen-0.2.2/examples/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     7288 2022-02-28 20:59:47.000000 cvxpygen-0.2.2/examples/ADP.ipynb
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     8008 2022-02-28 20:59:47.000000 cvxpygen-0.2.2/examples/MPC.ipynb
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     7887 2022-03-01 02:23:31.000000 cvxpygen-0.2.2/examples/actuator.ipynb
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     8539 2022-02-28 20:59:47.000000 cvxpygen-0.2.2/examples/charging.ipynb
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1906 2023-04-02 13:09:25.000000 cvxpygen-0.2.2/examples/main.py
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     6388 2022-02-28 20:59:47.000000 cvxpygen-0.2.2/examples/network.ipynb
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     3212 2022-01-15 02:10:19.000000 cvxpygen-0.2.2/examples/nnLS.ipynb
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     8685 2022-02-28 20:59:47.000000 cvxpygen-0.2.2/examples/portfolio.ipynb
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     5892 2022-02-28 20:59:47.000000 cvxpygen-0.2.2/examples/resource.ipynb
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    11483 2022-02-02 20:55:58.000000 cvxpygen-0.2.2/examples/testing.ipynb
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-02 15:35:37.715930 cvxpygen-0.2.2/examples/visualization/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     2316 2021-10-02 02:58:17.000000 cvxpygen-0.2.2/examples/visualization/actuator.py
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     4401 2021-10-04 23:32:35.000000 cvxpygen-0.2.2/examples/visualization/network.py
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1281 2021-10-04 17:36:58.000000 cvxpygen-0.2.2/examples/visualization/resource.py
--rw-r--r--   0 maximilianschaller   (501) staff       (20)       79 2023-04-02 15:35:37.722914 cvxpygen-0.2.2/setup.cfg
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1352 2023-04-02 15:35:19.000000 cvxpygen-0.2.2/setup.py
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-02 15:35:37.718102 cvxpygen-0.2.2/test/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)        0 2023-04-02 15:02:12.000000 cvxpygen-0.2.2/test/__init__.py
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     3590 2023-04-02 15:02:12.000000 cvxpygen-0.2.2/test/cpg_solver.py
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     4275 2023-04-02 15:02:12.000000 cvxpygen-0.2.2/test/setup.py
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-02 15:35:37.720954 cvxpygen-0.2.2/tests/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     4431 2023-04-02 14:29:53.000000 cvxpygen-0.2.2/tests/test_E2E_LP.py
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     7703 2023-04-02 14:29:53.000000 cvxpygen-0.2.2/tests/test_E2E_QP.py
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     3768 2023-04-02 14:29:53.000000 cvxpygen-0.2.2/tests/test_E2E_SOCP.py
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1319 2022-09-10 09:35:02.000000 cvxpygen-0.2.2/tests/utils_test.py
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-23 15:22:51.904600 cvxpygen-0.2.3/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    11349 2022-02-24 20:19:58.000000 cvxpygen-0.2.3/LICENSE
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1051 2022-03-18 03:22:21.000000 cvxpygen-0.2.3/MANIFEST.in
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     8732 2023-04-23 15:22:51.904744 cvxpygen-0.2.3/PKG-INFO
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     8313 2023-04-23 12:28:59.000000 cvxpygen-0.2.3/README.md
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-23 15:22:51.760278 cvxpygen-0.2.3/cvxpygen/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)        0 2022-02-24 05:57:25.000000 cvxpygen-0.2.3/cvxpygen/__init__.py
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    36709 2023-04-23 14:43:15.000000 cvxpygen-0.2.3/cvxpygen/cpg.py
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-23 15:22:51.747061 cvxpygen-0.2.3/cvxpygen/solvers/
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-23 15:22:51.776435 cvxpygen-0.2.3/cvxpygen/solvers/ecos/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     6148 2021-11-04 03:37:05.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/.DS_Store
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)       87 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/.bumpversion.cfg
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)       42 2022-02-23 21:43:27.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/.git
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      296 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/.gitignore
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      477 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/.travis.yml
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     4753 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/CMakeLists.txt
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     7272 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/CONTRIBUTING.md
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    35147 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/COPYING
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     3377 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/Makefile
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     4290 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/README.md
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    86113 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/README.pdf
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1476 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/ecos.mk
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-23 15:22:51.778607 cvxpygen-0.2.3/cvxpygen/solvers/ecos/ecos_bb/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    40478 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/ecos_bb/ecos_bb.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    11665 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/ecos_bb/ecos_bb_preproc.c
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-23 15:22:51.745902 cvxpygen-0.2.3/cvxpygen/solvers/ecos/external/
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-23 15:22:51.779258 cvxpygen-0.2.3/cvxpygen/solvers/ecos/external/SuiteSparse_config/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     6482 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/external/SuiteSparse_config/SuiteSparse_config.h
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-23 15:22:51.781335 cvxpygen-0.2.3/cvxpygen/solvers/ecos/external/amd/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     2027 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/external/amd/Makefile
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     8897 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/external/amd/README.txt
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-23 15:22:51.782861 cvxpygen-0.2.3/cvxpygen/solvers/ecos/external/amd/include/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    18328 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/external/amd/include/amd.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     9097 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/external/amd/include/amd_internal.h
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-23 15:22:51.802592 cvxpygen-0.2.3/cvxpygen/solvers/ecos/external/amd/src/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     5710 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/external/amd/src/amd_1.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    64873 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/external/amd/src/amd_2.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     4877 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/external/amd/src/amd_aat.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1786 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/external/amd/src/amd_control.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1253 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/external/amd/src/amd_defaults.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     5012 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/external/amd/src/amd_dump.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     3181 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/external/amd/src/amd_global.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     4173 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/external/amd/src/amd_info.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     5913 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/external/amd/src/amd_order.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     3703 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/external/amd/src/amd_post_tree.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     5509 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/external/amd/src/amd_postorder.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     3808 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/external/amd/src/amd_preprocess.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     2980 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/external/amd/src/amd_valid.c
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-23 15:22:51.804180 cvxpygen-0.2.3/cvxpygen/solvers/ecos/external/ldl/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      763 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/external/ldl/Makefile
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     5779 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/external/ldl/README.txt
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-23 15:22:51.805006 cvxpygen-0.2.3/cvxpygen/solvers/ecos/external/ldl/include/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     3988 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/external/ldl/include/ldl.h
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-23 15:22:51.805817 cvxpygen-0.2.3/cvxpygen/solvers/ecos/external/ldl/src/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    20401 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/external/ldl/src/ldl.c
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-23 15:22:51.817416 cvxpygen-0.2.3/cvxpygen/solvers/ecos/include/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     6290 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/include/cone.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1332 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/include/ctrlc.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    82553 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/include/data.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    12623 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/include/ecos.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     6689 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/include/ecos_bb.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1359 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/include/equil.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     2804 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/include/expcone.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     3882 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/include/glblopts.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     4968 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/include/kkt.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     2712 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/include/spla.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     3241 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/include/splamm.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1717 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/include/timer.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      822 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/include/wright_omega.h
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-23 15:22:51.829722 cvxpygen-0.2.3/cvxpygen/solvers/ecos/src/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    15297 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/src/cone.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     2721 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/src/ctrlc.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    54621 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/src/ecos.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    10355 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/src/equil.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     5076 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/src/expcone.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    14221 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/src/kkt.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    32391 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/src/preproc.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     3510 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/src/runecos.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     4039 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/src/runecos_exp.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     4091 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/src/spla.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     9590 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/src/splamm.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     2578 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/src/timer.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1962 2021-10-28 22:01:39.000000 cvxpygen-0.2.3/cvxpygen/solvers/ecos/src/wright_omega.c
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-23 15:22:51.830826 cvxpygen-0.2.3/cvxpygen/solvers/osqp-python/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    11357 2021-11-03 20:08:49.000000 cvxpygen-0.2.3/cvxpygen/solvers/osqp-python/LICENSE
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-23 15:22:51.840041 cvxpygen-0.2.3/cvxpygen/solvers/scs/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     6148 2022-02-23 21:12:10.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/.DS_Store
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      296 2022-03-01 03:33:41.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/.bumpversion.cfg
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)       41 2022-02-23 21:43:27.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/.git
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      488 2022-03-01 03:33:41.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/.gitignore
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1009 2022-03-01 03:33:41.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/CITATION.cff
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    11683 2022-03-01 03:33:41.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/CMakeLists.txt
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1110 2021-11-08 20:11:48.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/LICENSE.txt
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     7382 2022-03-01 03:33:41.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/Makefile
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      922 2022-03-01 03:33:41.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/README.md
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-23 15:22:51.844813 cvxpygen-0.2.3/cvxpygen/solvers/scs/cmake/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     8748 2021-11-08 20:11:48.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/cmake/AddInstallRPATHSupport.cmake
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     2499 2021-11-08 20:11:48.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/cmake/AddUninstallTarget.cmake
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    28861 2021-11-08 20:11:48.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/cmake/InstallBasicPackageFiles.cmake
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      286 2022-03-01 03:33:41.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/cmake/scs_types.h.in
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-23 15:22:51.854238 cvxpygen-0.2.3/cvxpygen/solvers/scs/include/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     3035 2022-03-01 03:33:41.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/include/aa.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1611 2022-03-01 03:33:41.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/include/cones.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      581 2021-11-08 20:11:48.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/include/ctrlc.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     5119 2022-03-01 03:33:41.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/include/glbopts.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      804 2022-03-01 03:33:41.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/include/linalg.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     2193 2022-03-01 03:33:41.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/include/linsys.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      493 2022-03-01 03:33:41.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/include/normalize.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      571 2022-03-01 03:33:41.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/include/rw.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    10042 2022-03-01 03:33:41.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/include/scs.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1010 2021-11-08 20:11:48.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/include/scs_blas.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      437 2022-03-01 03:33:41.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/include/scs_types.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     2747 2022-03-01 03:33:41.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/include/scs_work.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1217 2022-03-01 03:33:41.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/include/util.h
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-23 15:22:51.856992 cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-23 15:22:51.748934 cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/cpu/
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-23 15:22:51.858179 cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/cpu/direct/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    11554 2022-03-01 03:33:41.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/cpu/direct/private.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      768 2022-03-01 03:33:41.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/cpu/direct/private.h
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-23 15:22:51.859648 cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/cpu/indirect/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     9228 2022-03-01 03:33:41.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/cpu/indirect/private.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      681 2022-03-01 03:33:41.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/cpu/indirect/private.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     2586 2022-03-01 03:33:41.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/csparse.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      995 2021-11-08 23:08:19.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/csparse.h
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-23 15:22:51.749942 cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/external/
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-23 15:22:51.873111 cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/external/amd/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     2068 2022-03-01 03:33:41.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/external/amd/LICENSE.txt
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    14798 2022-03-01 03:33:41.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/external/amd/SuiteSparse_config.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     9151 2022-03-01 03:33:41.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/external/amd/SuiteSparse_config.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    17956 2021-11-08 20:11:48.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/external/amd/amd.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     5716 2021-11-08 20:11:48.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/external/amd/amd_1.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    64847 2021-11-08 20:11:48.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/external/amd/amd_2.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     4868 2021-11-08 20:11:48.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/external/amd/amd_aat.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1876 2021-11-08 20:11:48.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/external/amd/amd_control.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1259 2021-11-08 20:11:48.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/external/amd/amd_defaults.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     5012 2021-11-08 20:11:48.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/external/amd/amd_dump.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      941 2021-11-08 20:11:48.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/external/amd/amd_global.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     4299 2021-11-08 20:11:48.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/external/amd/amd_info.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     7706 2021-11-08 23:08:19.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/external/amd/amd_internal.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     6084 2022-03-01 03:33:41.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/external/amd/amd_order.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     3703 2021-11-08 20:11:48.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/external/amd/amd_post_tree.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     5509 2021-11-08 20:11:48.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/external/amd/amd_postorder.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     3808 2021-11-08 20:11:48.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/external/amd/amd_preprocess.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     2980 2021-11-08 20:11:48.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/external/amd/amd_valid.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      528 2021-11-08 20:11:48.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/external/amd/changes
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-23 15:22:51.877227 cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/external/qdldl/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    11357 2021-11-08 20:11:48.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/external/qdldl/LICENSE
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     4865 2021-11-08 20:11:48.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/external/qdldl/README.md
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      210 2021-11-08 23:08:19.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/external/qdldl/changes
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     7683 2021-11-08 23:08:19.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/external/qdldl/qdldl.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     6397 2021-11-08 23:08:19.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/external/qdldl/qdldl.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      533 2021-11-08 23:08:19.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/external/qdldl/qdldl_types.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    12027 2022-03-01 03:33:41.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/scs_matrix.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1839 2022-03-01 03:33:41.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/scs_matrix.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     4444 2022-03-01 03:33:41.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/scs.mk
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-23 15:22:51.886204 cvxpygen-0.2.3/cvxpygen/solvers/scs/src/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    14893 2022-03-01 03:33:41.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/src/aa.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    26617 2022-03-01 03:33:41.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/src/cones.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1770 2021-11-08 23:08:19.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/src/ctrlc.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     3996 2022-03-01 03:33:41.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/src/linalg.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     2556 2022-03-01 03:33:41.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/src/normalize.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    13982 2022-03-01 03:33:41.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/src/rw.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    39399 2022-03-01 03:33:41.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/src/scs.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      147 2022-03-01 03:33:41.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/src/scs_version.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     3529 2022-03-01 03:33:41.000000 cvxpygen-0.2.3/cvxpygen/solvers/scs/src/util.c
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-23 15:22:51.889268 cvxpygen-0.2.3/cvxpygen/template/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1649 2022-02-11 21:46:09.000000 cvxpygen-0.2.3/cvxpygen/template/CMakeLists.txt
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    11349 2022-02-24 20:19:58.000000 cvxpygen-0.2.3/cvxpygen/template/LICENSE
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     7450 2023-04-02 14:37:32.000000 cvxpygen-0.2.3/cvxpygen/template/README.html
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)        0 2023-04-02 15:35:19.000000 cvxpygen-0.2.3/cvxpygen/template/__init__.py
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     3968 2022-02-11 21:37:48.000000 cvxpygen-0.2.3/cvxpygen/template/setup.py
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    79619 2023-04-23 12:28:59.000000 cvxpygen-0.2.3/cvxpygen/utils.py
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-23 15:22:51.765198 cvxpygen-0.2.3/cvxpygen.egg-info/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     8732 2023-04-23 15:22:51.000000 cvxpygen-0.2.3/cvxpygen.egg-info/PKG-INFO
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     6562 2023-04-23 15:22:51.000000 cvxpygen-0.2.3/cvxpygen.egg-info/SOURCES.txt
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)        1 2023-04-23 15:22:51.000000 cvxpygen-0.2.3/cvxpygen.egg-info/dependency_links.txt
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)       94 2023-04-23 15:22:51.000000 cvxpygen-0.2.3/cvxpygen.egg-info/requires.txt
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)       34 2023-04-23 15:22:51.000000 cvxpygen-0.2.3/cvxpygen.egg-info/top_level.txt
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      144 2023-01-23 08:33:33.000000 cvxpygen-0.2.3/environment.yml
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-23 15:22:51.895116 cvxpygen-0.2.3/examples/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     7288 2022-02-28 20:59:47.000000 cvxpygen-0.2.3/examples/ADP.ipynb
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     8006 2023-04-23 15:21:28.000000 cvxpygen-0.2.3/examples/MPC.ipynb
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     7887 2022-03-01 02:23:31.000000 cvxpygen-0.2.3/examples/actuator.ipynb
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     8539 2022-02-28 20:59:47.000000 cvxpygen-0.2.3/examples/charging.ipynb
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1906 2023-04-23 15:21:28.000000 cvxpygen-0.2.3/examples/main.py
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     6388 2022-02-28 20:59:47.000000 cvxpygen-0.2.3/examples/network.ipynb
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     3212 2022-01-15 02:10:19.000000 cvxpygen-0.2.3/examples/nnLS.ipynb
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     8685 2022-02-28 20:59:47.000000 cvxpygen-0.2.3/examples/portfolio.ipynb
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     5892 2022-02-28 20:59:47.000000 cvxpygen-0.2.3/examples/resource.ipynb
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    11483 2022-02-02 20:55:58.000000 cvxpygen-0.2.3/examples/testing.ipynb
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-23 15:22:51.897258 cvxpygen-0.2.3/examples/visualization/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     2316 2021-10-02 02:58:17.000000 cvxpygen-0.2.3/examples/visualization/actuator.py
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     4401 2021-10-04 23:32:35.000000 cvxpygen-0.2.3/examples/visualization/network.py
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1281 2021-10-04 17:36:58.000000 cvxpygen-0.2.3/examples/visualization/resource.py
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-23 15:22:51.899356 cvxpygen-0.2.3/nonneg_LS/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)        0 2023-04-23 14:32:02.000000 cvxpygen-0.2.3/nonneg_LS/__init__.py
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     3019 2023-04-23 14:32:06.000000 cvxpygen-0.2.3/nonneg_LS/cpg_solver.py
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     3992 2023-04-23 14:32:06.000000 cvxpygen-0.2.3/nonneg_LS/setup.py
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)       79 2023-04-23 15:22:51.905470 cvxpygen-0.2.3/setup.cfg
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1352 2023-04-23 15:22:41.000000 cvxpygen-0.2.3/setup.py
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-23 15:22:51.901151 cvxpygen-0.2.3/test/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)        0 2023-04-02 15:02:12.000000 cvxpygen-0.2.3/test/__init__.py
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     3590 2023-04-02 15:02:12.000000 cvxpygen-0.2.3/test/cpg_solver.py
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     4275 2023-04-02 15:02:12.000000 cvxpygen-0.2.3/test/setup.py
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2023-04-23 15:22:51.904146 cvxpygen-0.2.3/tests/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     4431 2023-04-02 14:29:53.000000 cvxpygen-0.2.3/tests/test_E2E_LP.py
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     8735 2023-04-23 14:48:24.000000 cvxpygen-0.2.3/tests/test_E2E_QP.py
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     3768 2023-04-02 14:29:53.000000 cvxpygen-0.2.3/tests/test_E2E_SOCP.py
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1445 2023-04-23 12:28:59.000000 cvxpygen-0.2.3/tests/utils_test.py
```

### Comparing `cvxpygen-0.2.2/LICENSE` & `cvxpygen-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/MANIFEST.in` & `cvxpygen-0.2.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/PKG-INFO` & `cvxpygen-0.2.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvxpygen
-Version: 0.2.2
+Version: 0.2.3
 Summary: Code generation with CVXPY
 Home-page: https://github.com/cvxgrp/cvxpygen
 Author: Maximilian Schaller, Goran Banjac, Bartolomeo Stellato, Steven Diamond, Akshay Agrawal, Stephen Boyd
 Author-email: mschall@stanford.edu, goranbanjac1989@gmail.com, bstellato@princeton.edu, diamond@cs.stanford.edu, akshayka@cs.stanford.edu, boyd@stanford.edu
 License: Apache License, Version 2.0
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -103,21 +103,22 @@
 
 cpg.generate_code(problem, code_dir='nonneg_LS', solver='SCS')
 ```
 
 where the generated code is stored inside `nonneg_LS` and the `SCS` solver is used. 
 Next to the positional argument `problem`, all keyword arguments for the `generate_code()` method are summarized below.
 
-| Argument         | Meaning       | Default       |
-| -------------    | ------------- | ------------- |
-| `code_dir`       | directory for code to be stored in                                 | `'CPG_code'` |
-| `solver`         | canonical solver to generate code with                             | CVXPY default |
-| `unroll`         | unroll loops in canonicalization code                              | `False` |
-| `prefix`         | prefix for unique code symbols when dealing with multiple problems | `''`
-| `wrapper`        | compile Python wrapper for CVXPY interface                         | `True` |
+| Argument         | Meaning       | Type          | Default       |
+| -------------    | ------------- | ------------- | ------------- |
+| `code_dir`       | directory for code to be stored in                                 | String          | `'CPG_code'`  |
+| `solver`         | canonical solver to generate code with                             | String          | CVXPY default |
+| `enable_settings`| enabled settings that are otherwise locked by embedded solver      | List of Strings | `[]`          |
+| `unroll`         | unroll loops in canonicalization code                              | Bool            | `False`       |
+| `prefix`         | prefix for unique code symbols when dealing with multiple problems | String          | `''`          |
+| `wrapper`        | compile Python wrapper for CVXPY interface                         | Bool            | `True`        |
 
 You can find an overview of the code generation result in `nonneg_LS/README.html`.
 
 ### 2. Solve & Compare
 
 As summarized in the second part of [``examples/main.py``](https://github.com/cvxgrp/cvxpygen/blob/master/examples/main.py), after assigning parameter values, you can solve the problem both conventionally and via the generated code, which is wrapped inside the custom CVXPY solve method ``cpg_solve``.
```

### Comparing `cvxpygen-0.2.2/README.md` & `cvxpygen-0.2.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -90,21 +90,22 @@
 
 cpg.generate_code(problem, code_dir='nonneg_LS', solver='SCS')
 ```
 
 where the generated code is stored inside `nonneg_LS` and the `SCS` solver is used. 
 Next to the positional argument `problem`, all keyword arguments for the `generate_code()` method are summarized below.
 
-| Argument         | Meaning       | Default       |
-| -------------    | ------------- | ------------- |
-| `code_dir`       | directory for code to be stored in                                 | `'CPG_code'` |
-| `solver`         | canonical solver to generate code with                             | CVXPY default |
-| `unroll`         | unroll loops in canonicalization code                              | `False` |
-| `prefix`         | prefix for unique code symbols when dealing with multiple problems | `''`
-| `wrapper`        | compile Python wrapper for CVXPY interface                         | `True` |
+| Argument         | Meaning       | Type          | Default       |
+| -------------    | ------------- | ------------- | ------------- |
+| `code_dir`       | directory for code to be stored in                                 | String          | `'CPG_code'`  |
+| `solver`         | canonical solver to generate code with                             | String          | CVXPY default |
+| `enable_settings`| enabled settings that are otherwise locked by embedded solver      | List of Strings | `[]`          |
+| `unroll`         | unroll loops in canonicalization code                              | Bool            | `False`       |
+| `prefix`         | prefix for unique code symbols when dealing with multiple problems | String          | `''`          |
+| `wrapper`        | compile Python wrapper for CVXPY interface                         | Bool            | `True`        |
 
 You can find an overview of the code generation result in `nonneg_LS/README.html`.
 
 ### 2. Solve & Compare
 
 As summarized in the second part of [``examples/main.py``](https://github.com/cvxgrp/cvxpygen/blob/master/examples/main.py), after assigning parameter values, you can solve the problem both conventionally and via the generated code, which is wrapped inside the custom CVXPY solve method ``cpg_solve``.
```

### Comparing `cvxpygen-0.2.2/cvxpygen/cpg.py` & `cvxpygen-0.2.3/cvxpygen/cpg.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 from cvxpy.problems.objective import Maximize
 from cvxpy.cvxcore.python import canonInterface as cI
 from cvxpy.expressions.variable import upper_tri_to_full
 from cvxpy.reductions.solvers.conic_solvers.scs_conif import SCS
 from cvxpy.reductions.solvers.conic_solvers.ecos_conif import ECOS
 
 
-def generate_code(problem, code_dir='CPG_code', solver=None, unroll=False, prefix='', wrapper=True):
+def generate_code(problem, code_dir='CPG_code', solver=None, enable_settings=[], unroll=False, prefix='', wrapper=True):
     """
     Generate C code for CVXPY problem and (optionally) python wrapper
     """
 
     sys.stdout.write('Generating code with CVXPYgen ...\n')
 
     cvxpygen_directory = os.path.dirname(os.path.realpath(__file__))
@@ -435,23 +435,71 @@
             else:
                 canon_p[p_id] = canon_p_data
 
         canon_p_id_to_mapping[p_id] = mapping.tocsr()
         canon_p_id_to_changes[p_id] = mapping[:, :-1].nnz > 0
         canon_p_id_to_size[p_id] = mapping.shape[0]
 
+    # TODO: move this into a config file
     if solver_name == 'OSQP':
 
         # solver settings
         settings_names = ['rho', 'max_iter', 'eps_abs', 'eps_rel', 'eps_prim_inf', 'eps_dual_inf', 'alpha',
                           'scaled_termination', 'check_termination', 'warm_start']
         settings_types = ['c_float', 'c_int', 'c_float', 'c_float', 'c_float', 'c_float', 'c_float', 'c_int', 'c_int',
                           'c_int']
         settings_defaults = []
 
+        # extra settings
+        extra_settings_names = ['verbose', 'polish', 'polish_refine_iter', 'delta']
+        extra_settings_types = ['c_int', 'c_int', 'c_int', 'c_float']
+        extra_settings_defaults = [None] * len(extra_settings_names)
+
+    elif solver_name == 'SCS':
+
+        # solver settings
+        settings_names = ['normalize', 'scale', 'adaptive_scale', 'rho_x', 'max_iters', 'eps_abs',  'eps_rel',
+                          'eps_infeas', 'alpha', 'time_limit_secs', 'verbose', 'warm_start', 'acceleration_lookback',
+                          'acceleration_interval', 'write_data_filename', 'log_csv_filename']
+        settings_types = ['c_int', 'c_float', 'c_int', 'c_float', 'c_int', 'c_float', 'c_float', 'c_float', 'c_float',
+                          'c_float', 'c_int', 'c_int', 'c_int', 'c_int', 'const char*', 'const char*']
+        settings_defaults = ['1', '0.1', '1', '1e-6', '1e5', '1e-4', '1e-4', '1e-7', '1.5', '0', '0', '0', '0', '1',
+                             'SCS_NULL', 'SCS_NULL']
+
+        # extra settings
+        extra_settings_names = []
+        extra_settings_types = []
+        extra_settings_defaults = []
+
+    elif solver_name == 'ECOS':
+
+        # solver settings
+        settings_names = ['feastol', 'abstol', 'reltol', 'feastol_inacc', 'abstol_inacc', 'reltol_inacc', 'maxit']
+        settings_types = ['c_float', 'c_float', 'c_float', 'c_float', 'c_float', 'c_float', 'c_int']
+        settings_defaults = ['1e-8', '1e-8', '1e-8', '1e-4', '5e-5', '5e-5', '100']
+
+        # extra settings
+        extra_settings_names = []
+        extra_settings_types = []
+        extra_settings_defaults = []
+
+    # add extra settings
+    extra_settings_n2t = {n: t for n, t in zip(extra_settings_names, extra_settings_types)}
+    extra_settings_n2d = {n: d for n, d in zip(extra_settings_names, extra_settings_defaults)}
+
+    for s in (set(enable_settings)-set(settings_names)):
+        if s in extra_settings_names:
+            settings_names.append(s)
+            settings_types.append(extra_settings_n2t[s])
+            settings_defaults.append(extra_settings_n2d[s])
+        else:
+            warnings.warn('Cannot enable setting %s for solver %s' % (s, solver_name))
+
+    if solver_name == 'OSQP':
+
         # OSQP codegen
         osqp_obj = osqp.OSQP()
         osqp_obj.setup(P=canon_p_csc['P'], q=canon_p['q'], A=canon_p_csc['A'], l=canon_p['l'], u=canon_p['u'])
         if system() == 'Windows':
             cmake_generator = 'MinGW Makefiles'
         elif system() == 'Linux' or system() == 'Darwin':
             cmake_generator = 'Unix Makefiles'
@@ -461,24 +509,37 @@
                          parameters='matrices', force_rewrite=True)
 
         # copy license files
         shutil.copyfile(os.path.join(cvxpygen_directory, 'solvers', 'osqp-python', 'LICENSE'),
                         os.path.join(solver_code_dir, 'LICENSE'))
         shutil.copy(os.path.join(cvxpygen_directory, 'template', 'LICENSE'), code_dir)
 
-    elif solver_name == 'SCS':
+        # modify for extra settings
+        if 'verbose' in enable_settings:
+            utils.replace_in_file(os.path.join(code_dir, 'c', 'solver_code', 'CMakeLists.txt'),
+                [('message(STATUS "Disabling printing for embedded")', 'message(STATUS "Not disabling printing for embedded by user request")'),
+                 ('set(PRINTING OFF)', '')])
+            utils.replace_in_file(os.path.join(code_dir, 'c', 'solver_code', 'include', 'constants.h'),
+                [('# ifdef __cplusplus\n}', '#  define VERBOSE (1)\n\n# ifdef __cplusplus\n}')])
+            utils.replace_in_file(os.path.join(code_dir, 'c', 'solver_code', 'include', 'types.h'),
+                [('} OSQPInfo;', '  c_int status_polish;\n} OSQPInfo;'),
+                 ('} OSQPSettings;', '  c_int polish;\n  c_int verbose;\n} OSQPSettings;'),
+                 ('# ifndef EMBEDDED\n  c_int nthreads; ///< number of threads active\n# endif // ifndef EMBEDDED', '  c_int nthreads;')])
+            utils.replace_in_file(os.path.join(code_dir, 'c', 'solver_code', 'include', 'osqp.h'),
+                [('# ifdef __cplusplus\n}', 'c_int osqp_update_verbose(OSQPWorkspace *work, c_int verbose_new);\n\n# ifdef __cplusplus\n}')])
+            utils.replace_in_file(os.path.join(code_dir, 'c', 'solver_code', 'src', 'osqp', 'util.c'),
+                [('// Print Settings', '/* Print Settings'),
+                 ('LINSYS_SOLVER_NAME[settings->linsys_solver]);', 'LINSYS_SOLVER_NAME[settings->linsys_solver]);*/')])
+            utils.replace_in_file(os.path.join(code_dir, 'c', 'solver_code', 'src', 'osqp', 'osqp.c'),
+                [('void osqp_set_default_settings(OSQPSettings *settings) {', 'void osqp_set_default_settings(OSQPSettings *settings) {\n  settings->verbose = VERBOSE;'),
+                 ('c_int osqp_update_verbose', '#endif // EMBEDDED\n\nc_int osqp_update_verbose'),
+                 ('verbose = verbose_new;\n\n  return 0;\n}\n\n#endif // EMBEDDED', 'verbose = verbose_new;\n\n  return 0;\n}')])
+            
 
-        # solver settings
-        settings_names = ['normalize', 'scale', 'adaptive_scale', 'rho_x', 'max_iters', 'eps_abs',  'eps_rel',
-                          'eps_infeas', 'alpha', 'time_limit_secs', 'verbose', 'warm_start', 'acceleration_lookback',
-                          'acceleration_interval', 'write_data_filename', 'log_csv_filename']
-        settings_types = ['c_int', 'c_float', 'c_int', 'c_float', 'c_int', 'c_float', 'c_float', 'c_float', 'c_float',
-                          'c_float', 'c_int', 'c_int', 'c_int', 'c_int', 'const char*', 'const char*']
-        settings_defaults = ['1', '0.1', '1', '1e-6', '1e5', '1e-4', '1e-4', '1e-7', '1.5', '0', '0', '0', '0', '1',
-                             'SCS_NULL', 'SCS_NULL']
+    elif solver_name == 'SCS':
 
         # copy sources
         if os.path.isdir(solver_code_dir):
             shutil.rmtree(solver_code_dir)
         os.mkdir(solver_code_dir)
         dirs_to_copy = ['src', 'include', 'linsys', 'cmake']
         for dtc in dirs_to_copy:
@@ -524,19 +585,14 @@
                                         "os.path.join('c', 'solver_code', 'include'),\n" +
                                         indent + "os.path.join('c', 'solver_code', 'linsys'),")
         with open(os.path.join(code_dir, 'setup.py'), 'w') as f:
             f.write(setup_text)
 
     elif solver_name == 'ECOS':
 
-        # solver settings
-        settings_names = ['feastol', 'abstol', 'reltol', 'feastol_inacc', 'abstol_inacc', 'reltol_inacc', 'maxit']
-        settings_types = ['c_float', 'c_float', 'c_float', 'c_float', 'c_float', 'c_float', 'c_int']
-        settings_defaults = ['1e-8', '1e-8', '1e-8', '1e-4', '5e-5', '5e-5', '100']
-
         # copy sources
         if os.path.isdir(solver_code_dir):
             shutil.rmtree(solver_code_dir)
         os.mkdir(solver_code_dir)
         dirs_to_copy = ['src', 'include', 'external', 'ecos_bb']
         for dtc in dirs_to_copy:
             shutil.copytree(os.path.join(cvxpygen_directory, 'solvers', 'ecos', dtc), os.path.join(solver_code_dir, dtc))
```

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/ecos/.DS_Store` & `cvxpygen-0.2.3/cvxpygen/solvers/ecos/.DS_Store`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/ecos/CMakeLists.txt` & `cvxpygen-0.2.3/cvxpygen/solvers/ecos/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/ecos/CONTRIBUTING.md` & `cvxpygen-0.2.3/cvxpygen/solvers/ecos/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/ecos/COPYING` & `cvxpygen-0.2.3/cvxpygen/solvers/ecos/COPYING`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/ecos/Makefile` & `cvxpygen-0.2.3/cvxpygen/solvers/ecos/Makefile`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/ecos/README.md` & `cvxpygen-0.2.3/cvxpygen/solvers/ecos/README.md`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/ecos/README.pdf` & `cvxpygen-0.2.3/cvxpygen/solvers/ecos/README.pdf`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/ecos/ecos.mk` & `cvxpygen-0.2.3/cvxpygen/solvers/ecos/ecos.mk`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/ecos/ecos_bb/ecos_bb.c` & `cvxpygen-0.2.3/cvxpygen/solvers/ecos/ecos_bb/ecos_bb.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/ecos/ecos_bb/ecos_bb_preproc.c` & `cvxpygen-0.2.3/cvxpygen/solvers/ecos/ecos_bb/ecos_bb_preproc.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/ecos/external/SuiteSparse_config/SuiteSparse_config.h` & `cvxpygen-0.2.3/cvxpygen/solvers/ecos/external/SuiteSparse_config/SuiteSparse_config.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/ecos/external/amd/Makefile` & `cvxpygen-0.2.3/cvxpygen/solvers/ecos/external/amd/Makefile`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/ecos/external/amd/README.txt` & `cvxpygen-0.2.3/cvxpygen/solvers/ecos/external/amd/README.txt`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/ecos/external/amd/include/amd.h` & `cvxpygen-0.2.3/cvxpygen/solvers/ecos/external/amd/include/amd.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/ecos/external/amd/include/amd_internal.h` & `cvxpygen-0.2.3/cvxpygen/solvers/ecos/external/amd/include/amd_internal.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/ecos/external/amd/src/amd_1.c` & `cvxpygen-0.2.3/cvxpygen/solvers/ecos/external/amd/src/amd_1.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/ecos/external/amd/src/amd_2.c` & `cvxpygen-0.2.3/cvxpygen/solvers/ecos/external/amd/src/amd_2.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/ecos/external/amd/src/amd_aat.c` & `cvxpygen-0.2.3/cvxpygen/solvers/ecos/external/amd/src/amd_aat.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/ecos/external/amd/src/amd_control.c` & `cvxpygen-0.2.3/cvxpygen/solvers/ecos/external/amd/src/amd_control.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/ecos/external/amd/src/amd_defaults.c` & `cvxpygen-0.2.3/cvxpygen/solvers/ecos/external/amd/src/amd_defaults.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/ecos/external/amd/src/amd_dump.c` & `cvxpygen-0.2.3/cvxpygen/solvers/ecos/external/amd/src/amd_dump.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/ecos/external/amd/src/amd_global.c` & `cvxpygen-0.2.3/cvxpygen/solvers/ecos/external/amd/src/amd_global.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/ecos/external/amd/src/amd_info.c` & `cvxpygen-0.2.3/cvxpygen/solvers/ecos/external/amd/src/amd_info.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/ecos/external/amd/src/amd_order.c` & `cvxpygen-0.2.3/cvxpygen/solvers/ecos/external/amd/src/amd_order.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/ecos/external/amd/src/amd_post_tree.c` & `cvxpygen-0.2.3/cvxpygen/solvers/ecos/external/amd/src/amd_post_tree.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/ecos/external/amd/src/amd_postorder.c` & `cvxpygen-0.2.3/cvxpygen/solvers/ecos/external/amd/src/amd_postorder.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/ecos/external/amd/src/amd_preprocess.c` & `cvxpygen-0.2.3/cvxpygen/solvers/ecos/external/amd/src/amd_preprocess.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/ecos/external/amd/src/amd_valid.c` & `cvxpygen-0.2.3/cvxpygen/solvers/ecos/external/amd/src/amd_valid.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/ecos/external/ldl/Makefile` & `cvxpygen-0.2.3/cvxpygen/solvers/ecos/external/ldl/Makefile`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/ecos/external/ldl/README.txt` & `cvxpygen-0.2.3/cvxpygen/solvers/ecos/external/ldl/README.txt`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/ecos/external/ldl/include/ldl.h` & `cvxpygen-0.2.3/cvxpygen/solvers/ecos/external/ldl/include/ldl.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/ecos/external/ldl/src/ldl.c` & `cvxpygen-0.2.3/cvxpygen/solvers/ecos/external/ldl/src/ldl.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/ecos/include/cone.h` & `cvxpygen-0.2.3/cvxpygen/solvers/ecos/include/cone.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/ecos/include/ctrlc.h` & `cvxpygen-0.2.3/cvxpygen/solvers/ecos/include/ctrlc.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/ecos/include/data.h` & `cvxpygen-0.2.3/cvxpygen/solvers/ecos/include/data.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/ecos/include/ecos.h` & `cvxpygen-0.2.3/cvxpygen/solvers/ecos/include/ecos.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/ecos/include/ecos_bb.h` & `cvxpygen-0.2.3/cvxpygen/solvers/ecos/include/ecos_bb.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/ecos/include/equil.h` & `cvxpygen-0.2.3/cvxpygen/solvers/ecos/include/equil.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/ecos/include/expcone.h` & `cvxpygen-0.2.3/cvxpygen/solvers/ecos/include/expcone.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/ecos/include/glblopts.h` & `cvxpygen-0.2.3/cvxpygen/solvers/ecos/include/glblopts.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/ecos/include/kkt.h` & `cvxpygen-0.2.3/cvxpygen/solvers/ecos/include/kkt.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/ecos/include/spla.h` & `cvxpygen-0.2.3/cvxpygen/solvers/ecos/include/spla.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/ecos/include/splamm.h` & `cvxpygen-0.2.3/cvxpygen/solvers/ecos/include/splamm.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/ecos/include/timer.h` & `cvxpygen-0.2.3/cvxpygen/solvers/ecos/include/timer.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/ecos/include/wright_omega.h` & `cvxpygen-0.2.3/cvxpygen/solvers/ecos/include/wright_omega.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/ecos/src/cone.c` & `cvxpygen-0.2.3/cvxpygen/solvers/ecos/src/cone.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/ecos/src/ctrlc.c` & `cvxpygen-0.2.3/cvxpygen/solvers/ecos/src/ctrlc.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/ecos/src/ecos.c` & `cvxpygen-0.2.3/cvxpygen/solvers/ecos/src/ecos.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/ecos/src/equil.c` & `cvxpygen-0.2.3/cvxpygen/solvers/ecos/src/equil.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/ecos/src/expcone.c` & `cvxpygen-0.2.3/cvxpygen/solvers/ecos/src/expcone.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/ecos/src/kkt.c` & `cvxpygen-0.2.3/cvxpygen/solvers/ecos/src/kkt.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/ecos/src/preproc.c` & `cvxpygen-0.2.3/cvxpygen/solvers/ecos/src/preproc.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/ecos/src/runecos.c` & `cvxpygen-0.2.3/cvxpygen/solvers/ecos/src/runecos.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/ecos/src/runecos_exp.c` & `cvxpygen-0.2.3/cvxpygen/solvers/ecos/src/runecos_exp.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/ecos/src/spla.c` & `cvxpygen-0.2.3/cvxpygen/solvers/ecos/src/spla.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/ecos/src/splamm.c` & `cvxpygen-0.2.3/cvxpygen/solvers/ecos/src/splamm.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/ecos/src/timer.c` & `cvxpygen-0.2.3/cvxpygen/solvers/ecos/src/timer.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/ecos/src/wright_omega.c` & `cvxpygen-0.2.3/cvxpygen/solvers/ecos/src/wright_omega.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/osqp-python/LICENSE` & `cvxpygen-0.2.3/cvxpygen/solvers/osqp-python/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/.DS_Store` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/.DS_Store`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/CITATION.cff` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/CITATION.cff`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/CMakeLists.txt` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/LICENSE.txt` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/Makefile` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/Makefile`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/README.md` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/README.md`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/cmake/AddInstallRPATHSupport.cmake` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/cmake/AddInstallRPATHSupport.cmake`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/cmake/AddUninstallTarget.cmake` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/cmake/AddUninstallTarget.cmake`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/cmake/InstallBasicPackageFiles.cmake` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/cmake/InstallBasicPackageFiles.cmake`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/include/aa.h` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/include/aa.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/include/cones.h` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/include/cones.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/include/ctrlc.h` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/include/ctrlc.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/include/glbopts.h` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/include/glbopts.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/include/linalg.h` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/include/linalg.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/include/linsys.h` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/include/linsys.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/include/rw.h` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/include/rw.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/include/scs.h` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/include/scs.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/include/scs_blas.h` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/include/scs_blas.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/include/scs_work.h` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/include/scs_work.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/include/util.h` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/include/util.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/cpu/direct/private.c` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/cpu/direct/private.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/cpu/direct/private.h` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/cpu/direct/private.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/cpu/indirect/private.c` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/cpu/indirect/private.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/cpu/indirect/private.h` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/cpu/indirect/private.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/csparse.c` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/csparse.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/csparse.h` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/csparse.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/external/amd/LICENSE.txt` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/external/amd/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/external/amd/SuiteSparse_config.c` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/external/amd/SuiteSparse_config.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/external/amd/SuiteSparse_config.h` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/external/amd/SuiteSparse_config.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/external/amd/amd.h` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/external/amd/amd.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/external/amd/amd_1.c` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/external/amd/amd_1.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/external/amd/amd_2.c` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/external/amd/amd_2.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/external/amd/amd_aat.c` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/external/amd/amd_aat.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/external/amd/amd_control.c` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/external/amd/amd_control.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/external/amd/amd_defaults.c` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/external/amd/amd_defaults.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/external/amd/amd_dump.c` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/external/amd/amd_dump.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/external/amd/amd_global.c` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/external/amd/amd_global.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/external/amd/amd_info.c` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/external/amd/amd_info.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/external/amd/amd_internal.h` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/external/amd/amd_internal.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/external/amd/amd_order.c` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/external/amd/amd_order.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/external/amd/amd_post_tree.c` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/external/amd/amd_post_tree.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/external/amd/amd_postorder.c` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/external/amd/amd_postorder.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/external/amd/amd_preprocess.c` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/external/amd/amd_preprocess.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/external/amd/amd_valid.c` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/external/amd/amd_valid.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/external/amd/changes` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/external/amd/changes`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/external/qdldl/LICENSE` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/external/qdldl/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/external/qdldl/README.md` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/external/qdldl/README.md`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/external/qdldl/qdldl.c` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/external/qdldl/qdldl.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/external/qdldl/qdldl.h` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/external/qdldl/qdldl.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/external/qdldl/qdldl_types.h` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/external/qdldl/qdldl_types.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/scs_matrix.c` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/scs_matrix.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/linsys/scs_matrix.h` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/linsys/scs_matrix.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/scs.mk` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/scs.mk`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/src/aa.c` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/src/aa.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/src/cones.c` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/src/cones.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/src/ctrlc.c` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/src/ctrlc.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/src/linalg.c` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/src/linalg.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/src/normalize.c` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/src/normalize.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/src/rw.c` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/src/rw.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/src/scs.c` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/src/scs.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/solvers/scs/src/util.c` & `cvxpygen-0.2.3/cvxpygen/solvers/scs/src/util.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/template/CMakeLists.txt` & `cvxpygen-0.2.3/cvxpygen/template/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/template/LICENSE` & `cvxpygen-0.2.3/cvxpygen/template/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/template/README.html` & `cvxpygen-0.2.3/cvxpygen/template/README.html`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/template/setup.py` & `cvxpygen-0.2.3/cvxpygen/template/setup.py`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/cvxpygen/utils.py` & `cvxpygen-0.2.3/cvxpygen/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,14 +67,27 @@
     now = datetime.now()
     f.write('\n%s\n' % comment_str)
     f.write('Auto-generated by CVXPYgen %s.\n' % now.strftime("on %B %d, %Y at %H:%M:%S"))
     f.write('Content: %s.\n' % content)
     f.write('%s\n\n' % comment_str[::-1])
 
 
+def replace_in_file(filepath, replacements):
+    """
+    Replace strings in file
+    """
+
+    with open(filepath, 'r') as f:
+        t = f.read()
+    for old, new in replacements:
+        t = t.replace(old, new)
+    with open(filepath, 'w') as f:
+        f.write(t)
+
+
 def replace_inf(v):
     """
     Replace infinity by large number
     """
 
     # check if dealing with csc dict or numpy array
     if type(v) == dict:
```

### Comparing `cvxpygen-0.2.2/cvxpygen.egg-info/PKG-INFO` & `cvxpygen-0.2.3/cvxpygen.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvxpygen
-Version: 0.2.2
+Version: 0.2.3
 Summary: Code generation with CVXPY
 Home-page: https://github.com/cvxgrp/cvxpygen
 Author: Maximilian Schaller, Goran Banjac, Bartolomeo Stellato, Steven Diamond, Akshay Agrawal, Stephen Boyd
 Author-email: mschall@stanford.edu, goranbanjac1989@gmail.com, bstellato@princeton.edu, diamond@cs.stanford.edu, akshayka@cs.stanford.edu, boyd@stanford.edu
 License: Apache License, Version 2.0
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -103,21 +103,22 @@
 
 cpg.generate_code(problem, code_dir='nonneg_LS', solver='SCS')
 ```
 
 where the generated code is stored inside `nonneg_LS` and the `SCS` solver is used. 
 Next to the positional argument `problem`, all keyword arguments for the `generate_code()` method are summarized below.
 
-| Argument         | Meaning       | Default       |
-| -------------    | ------------- | ------------- |
-| `code_dir`       | directory for code to be stored in                                 | `'CPG_code'` |
-| `solver`         | canonical solver to generate code with                             | CVXPY default |
-| `unroll`         | unroll loops in canonicalization code                              | `False` |
-| `prefix`         | prefix for unique code symbols when dealing with multiple problems | `''`
-| `wrapper`        | compile Python wrapper for CVXPY interface                         | `True` |
+| Argument         | Meaning       | Type          | Default       |
+| -------------    | ------------- | ------------- | ------------- |
+| `code_dir`       | directory for code to be stored in                                 | String          | `'CPG_code'`  |
+| `solver`         | canonical solver to generate code with                             | String          | CVXPY default |
+| `enable_settings`| enabled settings that are otherwise locked by embedded solver      | List of Strings | `[]`          |
+| `unroll`         | unroll loops in canonicalization code                              | Bool            | `False`       |
+| `prefix`         | prefix for unique code symbols when dealing with multiple problems | String          | `''`          |
+| `wrapper`        | compile Python wrapper for CVXPY interface                         | Bool            | `True`        |
 
 You can find an overview of the code generation result in `nonneg_LS/README.html`.
 
 ### 2. Solve & Compare
 
 As summarized in the second part of [``examples/main.py``](https://github.com/cvxgrp/cvxpygen/blob/master/examples/main.py), after assigning parameter values, you can solve the problem both conventionally and via the generated code, which is wrapped inside the custom CVXPY solve method ``cpg_solve``.
```

### Comparing `cvxpygen-0.2.2/cvxpygen.egg-info/SOURCES.txt` & `cvxpygen-0.2.3/cvxpygen.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -158,14 +158,17 @@
 examples/nnLS.ipynb
 examples/portfolio.ipynb
 examples/resource.ipynb
 examples/testing.ipynb
 examples/visualization/actuator.py
 examples/visualization/network.py
 examples/visualization/resource.py
+nonneg_LS/__init__.py
+nonneg_LS/cpg_solver.py
+nonneg_LS/setup.py
 test/__init__.py
 test/cpg_solver.py
 test/setup.py
 tests/test_E2E_LP.py
 tests/test_E2E_QP.py
 tests/test_E2E_SOCP.py
 tests/utils_test.py
```

### Comparing `cvxpygen-0.2.2/examples/ADP.ipynb` & `cvxpygen-0.2.3/examples/ADP.ipynb`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/examples/MPC.ipynb` & `cvxpygen-0.2.3/examples/MPC.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999007936507937%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(18, 'objective = cp.Minimize(cp.sum_squares(Psqrt@X[:,H]) + "*

 * *            "cp.sum_squares(Qsqrt@X[:,:H]) + cp.sum_squares(Rsqrt@U))\\n')], delete: [18]}}}"}*

```diff
@@ -53,15 +53,15 @@
                 "Qsqrt = cp.Parameter((n, n), name='Qsqrt')\n",
                 "Rsqrt = cp.Parameter((m, m), name='Rsqrt')\n",
                 "A = cp.Parameter((n, n), name='A')\n",
                 "B = cp.Parameter((n, m), name='B')\n",
                 "x_init = cp.Parameter(n, name='x_init')\n",
                 "\n",
                 "# define objective\n",
-                "objective = cp.Minimize(cp.sum_squares(Psqrt@X[:,H-1]) + cp.sum_squares(Qsqrt@X[:,:H]) + cp.sum_squares(Rsqrt@U))\n",
+                "objective = cp.Minimize(cp.sum_squares(Psqrt@X[:,H]) + cp.sum_squares(Qsqrt@X[:,:H]) + cp.sum_squares(Rsqrt@U))\n",
                 "\n",
                 "# define constraints\n",
                 "constraints = [X[:,1:] == A@X[:,:H]+B@U,\n",
                 "               cp.abs(U) <= 1,\n",
                 "               X[:,0] == x_init]\n",
                 "\n",
                 "# define problem\n",
```

### Comparing `cvxpygen-0.2.2/examples/actuator.ipynb` & `cvxpygen-0.2.3/examples/actuator.ipynb`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/examples/charging.ipynb` & `cvxpygen-0.2.3/examples/charging.ipynb`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/examples/main.py` & `cvxpygen-0.2.3/examples/main.py`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/examples/network.ipynb` & `cvxpygen-0.2.3/examples/network.ipynb`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/examples/nnLS.ipynb` & `cvxpygen-0.2.3/examples/nnLS.ipynb`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/examples/portfolio.ipynb` & `cvxpygen-0.2.3/examples/portfolio.ipynb`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/examples/resource.ipynb` & `cvxpygen-0.2.3/examples/resource.ipynb`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/examples/testing.ipynb` & `cvxpygen-0.2.3/examples/testing.ipynb`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/examples/visualization/actuator.py` & `cvxpygen-0.2.3/examples/visualization/actuator.py`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/examples/visualization/network.py` & `cvxpygen-0.2.3/examples/visualization/network.py`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/examples/visualization/resource.py` & `cvxpygen-0.2.3/examples/visualization/resource.py`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/setup.py` & `cvxpygen-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 MAJOR = 0
 MINOR = 2
-MICRO = 2
+MICRO = 3
 VERSION = '%d.%d.%d' % (MAJOR, MINOR, MICRO)
 
 
 def readme():
     with open('README.md') as f:
         content = f.read()
     return content[:content.find('## Tests')]
```

### Comparing `cvxpygen-0.2.2/test/cpg_solver.py` & `cvxpygen-0.2.3/test/cpg_solver.py`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/test/setup.py` & `cvxpygen-0.2.3/test/setup.py`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/tests/test_E2E_LP.py` & `cvxpygen-0.2.3/tests/test_E2E_LP.py`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/tests/test_E2E_QP.py` & `cvxpygen-0.2.3/tests/test_E2E_QP.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 
 import pytest
 import cvxpy as cp
 import numpy as np
 import glob
 import os
+import io
 import importlib
 import itertools
 import pickle
 import utils_test
 import sys
 sys.path.append('../')
 from cvxpygen import cpg
@@ -218,7 +219,35 @@
     else:
         assert np.linalg.norm(prim_cg, 2) < 1e-3
 
     if dual_py_norm > 1e-6:
         assert np.linalg.norm(dual_cg - dual_py, 2) / dual_py_norm < 0.1
     else:
         assert np.linalg.norm(dual_cg, 2) < 1e-3
+
+    
+def test_OSQP_verbose():
+
+    prob = actuator_problem()
+    prob = assign_data(prob, 'actuator', 0)
+
+    cpg.generate_code(prob, code_dir='test_actuator_OSQP_verbose', solver='OSQP', unroll=False, prefix='actuator_OSQP_verbose', enable_settings=['verbose'])
+    assert len(glob.glob(os.path.join('test_actuator_OSQP_verbose', 'cpg_module.*'))) > 0
+
+    with open('test_actuator_OSQP_verbose/problem.pickle', 'rb') as f:
+        prob = pickle.load(f)
+
+    module = importlib.import_module('test_actuator_OSQP_verbose.cpg_solver')
+    prob.register_solve('CPG', module.cpg_solve)
+
+    prob = assign_data(prob, 'actuaor', 0)
+
+    verbose_output = io.StringIO()
+    sys.stdout = verbose_output
+    
+    _ = utils_test.check(prob, 'OSQP', 'actuator', get_primal_vec, verbose=False)
+    assert 'optimal objective' not in verbose_output.getvalue()
+
+    _ = utils_test.check(prob, 'OSQP', 'actuator', get_primal_vec, verbose=True)
+    assert 'optimal objective' in verbose_output.getvalue()
+
+    sys.stdout = sys.__stdout__
```

### Comparing `cvxpygen-0.2.2/tests/test_E2E_SOCP.py` & `cvxpygen-0.2.3/tests/test_E2E_SOCP.py`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.2.2/tests/utils_test.py` & `cvxpygen-0.2.3/tests/utils_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,30 +8,30 @@
         if constr.args[0].size == 1:
             dual_values.append(np.atleast_1d(constr.dual_value).flatten())
         else:
             dual_values.append(constr.dual_value.flatten())
     return np.concatenate(dual_values)
 
 
-def check(prob, solver, name, func_get_primal_vec):
+def check(prob, solver, name, func_get_primal_vec, **extra_settings):
 
     if solver == 'OSQP':
         val_py = prob.solve(solver='OSQP', eps_abs=1e-3, eps_rel=1e-3, max_iter=4000, polish=False,
-                            adaptive_rho_interval=int(1e6), warm_start=False)
+                            adaptive_rho_interval=int(1e6), warm_start=False, **extra_settings)
     elif solver == 'SCS':
-        val_py = prob.solve(solver='SCS', warm_start=False, verbose=False)
+        val_py = prob.solve(solver='SCS', warm_start=False, verbose=False, **extra_settings)
     else:
-        val_py = prob.solve(solver='ECOS')
+        val_py = prob.solve(solver='ECOS', **extra_settings)
     prim_py = func_get_primal_vec(prob, name)
     dual_py = get_dual_vec(prob)
     if solver == 'OSQP':
-        val_cg = prob.solve(method='CPG', warm_start=False)
+        val_cg = prob.solve(method='CPG', warm_start=False, **extra_settings)
     elif solver == 'SCS':
-        val_cg = prob.solve(method='CPG', warm_start=False, verbose=False)
+        val_cg = prob.solve(method='CPG', warm_start=False, verbose=False, **extra_settings)
     else:
-        val_cg = prob.solve(method='CPG')
+        val_cg = prob.solve(method='CPG', **extra_settings)
     prim_cg = func_get_primal_vec(prob, name)
     dual_cg = get_dual_vec(prob)
     prim_py_norm = np.linalg.norm(prim_py, 2)
     dual_py_norm = np.linalg.norm(dual_py, 2)
 
     return val_py, prim_py, dual_py, val_cg, prim_cg, dual_cg, prim_py_norm, dual_py_norm
```

