# Comparing `tmp/dragonfly-schema-1.9.0.tar.gz` & `tmp/dragonfly-schema-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dragonfly-schema-1.9.0.tar", last modified: Mon Mar  6 14:50:54 2023, max compression
+gzip compressed data, was "dist/dragonfly-schema-1.9.1.tar", last modified: Sun Apr 23 20:10:24 2023, max compression
```

## Comparing `dragonfly-schema-1.9.0.tar` & `dragonfly-schema-1.9.1.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:50:54.000000 dragonfly-schema-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-06 14:49:26.000000 dragonfly-schema-1.9.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:50:54.000000 dragonfly-schema-1.9.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:50:54.000000 dragonfly-schema-1.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-03-06 14:49:26.000000 dragonfly-schema-1.9.0/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-03-06 14:49:26.000000 dragonfly-schema-1.9.0/.github/workflows/dependency-release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-06 14:49:26.000000 dragonfly-schema-1.9.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-03-06 14:49:26.000000 dragonfly-schema-1.9.0/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-03-06 14:49:26.000000 dragonfly-schema-1.9.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-03-06 14:49:26.000000 dragonfly-schema-1.9.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-06 14:49:26.000000 dragonfly-schema-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-03-06 14:50:54.000000 dragonfly-schema-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-03-06 14:49:26.000000 dragonfly-schema-1.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-03-06 14:49:26.000000 dragonfly-schema-1.9.0/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-06 14:49:26.000000 dragonfly-schema-1.9.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:50:54.000000 dragonfly-schema-1.9.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 14:49:26.000000 dragonfly-schema-1.9.0/docs/.nojekyll
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-03-06 14:49:26.000000 dragonfly-schema-1.9.0/docs/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-03-06 14:49:26.000000 dragonfly-schema-1.9.0/docs/model.html
--rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-03-06 14:49:26.000000 dragonfly-schema-1.9.0/docs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:50:54.000000 dragonfly-schema-1.9.0/dragonfly_schema/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-03-06 14:49:26.000000 dragonfly-schema-1.9.0/dragonfly_schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:50:54.000000 dragonfly-schema-1.9.0/dragonfly_schema/energy/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-06 14:49:26.000000 dragonfly-schema-1.9.0/dragonfly_schema/energy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-03-06 14:49:26.000000 dragonfly-schema-1.9.0/dragonfly_schema/energy/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    13445 2023-03-06 14:49:26.000000 dragonfly-schema-1.9.0/dragonfly_schema/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:50:54.000000 dragonfly-schema-1.9.0/dragonfly_schema/radiance/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-06 14:49:26.000000 dragonfly-schema-1.9.0/dragonfly_schema/radiance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-03-06 14:49:26.000000 dragonfly-schema-1.9.0/dragonfly_schema/radiance/gridpar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-03-06 14:49:26.000000 dragonfly-schema-1.9.0/dragonfly_schema/radiance/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-03-06 14:49:26.000000 dragonfly-schema-1.9.0/dragonfly_schema/roof.py
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-03-06 14:49:26.000000 dragonfly-schema-1.9.0/dragonfly_schema/shading_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-03-06 14:49:26.000000 dragonfly-schema-1.9.0/dragonfly_schema/skylight_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9096 2023-03-06 14:49:26.000000 dragonfly-schema-1.9.0/dragonfly_schema/window_parameter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:50:54.000000 dragonfly-schema-1.9.0/dragonfly_schema.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-03-06 14:50:54.000000 dragonfly-schema-1.9.0/dragonfly_schema.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-03-06 14:50:54.000000 dragonfly-schema-1.9.0/dragonfly_schema.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 14:50:54.000000 dragonfly-schema-1.9.0/dragonfly_schema.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-06 14:50:54.000000 dragonfly-schema-1.9.0/dragonfly_schema.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-06 14:50:54.000000 dragonfly-schema-1.9.0/dragonfly_schema.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-06 14:49:26.000000 dragonfly-schema-1.9.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:50:54.000000 dragonfly-schema-1.9.0/samples/
--rw-r--r--   0 runner    (1001) docker     (123)    22598 2023-03-06 14:49:26.000000 dragonfly-schema-1.9.0/samples/building_simple.json
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-03-06 14:49:26.000000 dragonfly-schema-1.9.0/samples/context_shade_two_tree_canopy.json
--rw-r--r--   0 runner    (1001) docker     (123)    90404 2023-03-06 14:49:26.000000 dragonfly-schema-1.9.0/samples/model_complete_simple.dfjson
--rw-r--r--   0 runner    (1001) docker     (123)   112149 2023-03-06 14:49:26.000000 dragonfly-schema-1.9.0/samples/model_with_doors_skylights.dfjson
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-03-06 14:49:26.000000 dragonfly-schema-1.9.0/samples/room2d_simple.json
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-06 14:49:26.000000 dragonfly-schema-1.9.0/samples/shading_par_extruded_border.json
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-03-06 14:49:26.000000 dragonfly-schema-1.9.0/samples/shading_par_louvers_by_count.json
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-03-06 14:49:26.000000 dragonfly-schema-1.9.0/samples/shading_par_louvers_by_distance.json
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-06 14:49:26.000000 dragonfly-schema-1.9.0/samples/shading_par_overhang.json
--rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-03-06 14:49:26.000000 dragonfly-schema-1.9.0/samples/story_air_boundary.json
--rw-r--r--   0 runner    (1001) docker     (123)     9468 2023-03-06 14:49:26.000000 dragonfly-schema-1.9.0/samples/story_simple.json
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-03-06 14:49:26.000000 dragonfly-schema-1.9.0/samples/window_par_detailed_rectangular_windows.json
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-03-06 14:49:26.000000 dragonfly-schema-1.9.0/samples/window_par_detailed_windows.json
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-03-06 14:49:26.000000 dragonfly-schema-1.9.0/samples/window_par_repeating_window_ratio.json
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-03-06 14:49:26.000000 dragonfly-schema-1.9.0/samples/window_par_repeating_window_width_height.json
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-06 14:49:26.000000 dragonfly-schema-1.9.0/samples/window_par_simple_window_ratio.json
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-06 14:49:26.000000 dragonfly-schema-1.9.0/samples/window_par_single_window.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:50:54.000000 dragonfly-schema-1.9.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 14:49:26.000000 dragonfly-schema-1.9.0/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-03-06 14:49:26.000000 dragonfly-schema-1.9.0/scripts/export_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     9703 2023-03-06 14:49:26.000000 dragonfly-schema-1.9.0/scripts/sample_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-03-06 14:49:26.000000 dragonfly-schema-1.9.0/scripts/sample_shading_par.py
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-03-06 14:49:26.000000 dragonfly-schema-1.9.0/scripts/sample_window_par.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-06 14:50:54.000000 dragonfly-schema-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-03-06 14:49:26.000000 dragonfly-schema-1.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:50:54.000000 dragonfly-schema-1.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 14:49:26.000000 dragonfly-schema-1.9.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-03-06 14:49:26.000000 dragonfly-schema-1.9.0/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-03-06 14:49:26.000000 dragonfly-schema-1.9.0/tests/test_openapi_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-03-06 14:49:26.000000 dragonfly-schema-1.9.0/tests/test_shading_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-03-06 14:49:26.000000 dragonfly-schema-1.9.0/tests/test_window_parameter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 20:10:24.000000 dragonfly-schema-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-23 20:09:03.000000 dragonfly-schema-1.9.1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 20:10:24.000000 dragonfly-schema-1.9.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 20:10:24.000000 dragonfly-schema-1.9.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-04-23 20:09:03.000000 dragonfly-schema-1.9.1/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-23 20:09:03.000000 dragonfly-schema-1.9.1/.github/workflows/dependency-release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-23 20:09:03.000000 dragonfly-schema-1.9.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-23 20:09:03.000000 dragonfly-schema-1.9.1/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-23 20:09:03.000000 dragonfly-schema-1.9.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-23 20:09:03.000000 dragonfly-schema-1.9.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-23 20:09:03.000000 dragonfly-schema-1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-23 20:10:24.000000 dragonfly-schema-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-23 20:09:03.000000 dragonfly-schema-1.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-23 20:09:03.000000 dragonfly-schema-1.9.1/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-23 20:09:03.000000 dragonfly-schema-1.9.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 20:10:24.000000 dragonfly-schema-1.9.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 20:09:03.000000 dragonfly-schema-1.9.1/docs/.nojekyll
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-23 20:09:03.000000 dragonfly-schema-1.9.1/docs/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-23 20:09:03.000000 dragonfly-schema-1.9.1/docs/model.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-04-23 20:09:03.000000 dragonfly-schema-1.9.1/docs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 20:10:24.000000 dragonfly-schema-1.9.1/dragonfly_schema/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-23 20:09:03.000000 dragonfly-schema-1.9.1/dragonfly_schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 20:10:24.000000 dragonfly-schema-1.9.1/dragonfly_schema/energy/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-23 20:09:03.000000 dragonfly-schema-1.9.1/dragonfly_schema/energy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-04-23 20:09:03.000000 dragonfly-schema-1.9.1/dragonfly_schema/energy/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13445 2023-04-23 20:09:03.000000 dragonfly-schema-1.9.1/dragonfly_schema/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 20:10:24.000000 dragonfly-schema-1.9.1/dragonfly_schema/radiance/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-23 20:09:03.000000 dragonfly-schema-1.9.1/dragonfly_schema/radiance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-04-23 20:09:03.000000 dragonfly-schema-1.9.1/dragonfly_schema/radiance/gridpar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-04-23 20:09:03.000000 dragonfly-schema-1.9.1/dragonfly_schema/radiance/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-23 20:09:03.000000 dragonfly-schema-1.9.1/dragonfly_schema/roof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-04-23 20:09:03.000000 dragonfly-schema-1.9.1/dragonfly_schema/shading_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-04-23 20:09:03.000000 dragonfly-schema-1.9.1/dragonfly_schema/skylight_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9649 2023-04-23 20:09:03.000000 dragonfly-schema-1.9.1/dragonfly_schema/window_parameter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 20:10:24.000000 dragonfly-schema-1.9.1/dragonfly_schema.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-23 20:10:24.000000 dragonfly-schema-1.9.1/dragonfly_schema.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-04-23 20:10:24.000000 dragonfly-schema-1.9.1/dragonfly_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 20:10:24.000000 dragonfly-schema-1.9.1/dragonfly_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-23 20:10:24.000000 dragonfly-schema-1.9.1/dragonfly_schema.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-23 20:10:24.000000 dragonfly-schema-1.9.1/dragonfly_schema.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-23 20:09:03.000000 dragonfly-schema-1.9.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 20:10:24.000000 dragonfly-schema-1.9.1/samples/
+-rw-r--r--   0 runner    (1001) docker     (123)    22598 2023-04-23 20:09:03.000000 dragonfly-schema-1.9.1/samples/building_simple.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-23 20:09:03.000000 dragonfly-schema-1.9.1/samples/context_shade_two_tree_canopy.json
+-rw-r--r--   0 runner    (1001) docker     (123)    90404 2023-04-23 20:09:03.000000 dragonfly-schema-1.9.1/samples/model_complete_simple.dfjson
+-rw-r--r--   0 runner    (1001) docker     (123)   112149 2023-04-23 20:09:03.000000 dragonfly-schema-1.9.1/samples/model_with_doors_skylights.dfjson
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-23 20:09:03.000000 dragonfly-schema-1.9.1/samples/room2d_simple.json
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-23 20:09:03.000000 dragonfly-schema-1.9.1/samples/shading_par_extruded_border.json
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-23 20:09:03.000000 dragonfly-schema-1.9.1/samples/shading_par_louvers_by_count.json
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-23 20:09:03.000000 dragonfly-schema-1.9.1/samples/shading_par_louvers_by_distance.json
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-23 20:09:03.000000 dragonfly-schema-1.9.1/samples/shading_par_overhang.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-04-23 20:09:03.000000 dragonfly-schema-1.9.1/samples/story_air_boundary.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9468 2023-04-23 20:09:03.000000 dragonfly-schema-1.9.1/samples/story_simple.json
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-23 20:09:03.000000 dragonfly-schema-1.9.1/samples/window_par_detailed_rectangular_windows.json
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-23 20:09:03.000000 dragonfly-schema-1.9.1/samples/window_par_detailed_windows.json
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-23 20:09:03.000000 dragonfly-schema-1.9.1/samples/window_par_repeating_window_ratio.json
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-23 20:09:03.000000 dragonfly-schema-1.9.1/samples/window_par_repeating_window_width_height.json
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-23 20:09:03.000000 dragonfly-schema-1.9.1/samples/window_par_simple_window_ratio.json
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-23 20:09:03.000000 dragonfly-schema-1.9.1/samples/window_par_single_window.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 20:10:24.000000 dragonfly-schema-1.9.1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 20:09:03.000000 dragonfly-schema-1.9.1/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-23 20:09:03.000000 dragonfly-schema-1.9.1/scripts/export_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9703 2023-04-23 20:09:03.000000 dragonfly-schema-1.9.1/scripts/sample_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-23 20:09:03.000000 dragonfly-schema-1.9.1/scripts/sample_shading_par.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-04-23 20:09:03.000000 dragonfly-schema-1.9.1/scripts/sample_window_par.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-23 20:10:24.000000 dragonfly-schema-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-23 20:09:03.000000 dragonfly-schema-1.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 20:10:24.000000 dragonfly-schema-1.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 20:09:03.000000 dragonfly-schema-1.9.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-23 20:09:03.000000 dragonfly-schema-1.9.1/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-23 20:09:03.000000 dragonfly-schema-1.9.1/tests/test_openapi_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-23 20:09:03.000000 dragonfly-schema-1.9.1/tests/test_shading_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-23 20:09:03.000000 dragonfly-schema-1.9.1/tests/test_window_parameter.py
```

### Comparing `dragonfly-schema-1.9.0/.github/workflows/ci.yaml` & `dragonfly-schema-1.9.1/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.0/.github/workflows/dependency-release.yaml` & `dragonfly-schema-1.9.1/.github/workflows/dependency-release.yaml`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.0/.releaserc.json` & `dragonfly-schema-1.9.1/.releaserc.json`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.0/LICENSE` & `dragonfly-schema-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.0/PKG-INFO` & `dragonfly-schema-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dragonfly-schema
-Version: 1.9.0
+Version: 1.9.1
 Summary: Dragonfly Data-Model Objects
 Home-page: https://github.com/ladybug-tools/dragonfly-schema
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Operating System :: OS Independent
```

### Comparing `dragonfly-schema-1.9.0/README.md` & `dragonfly-schema-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.0/docs/index.html` & `dragonfly-schema-1.9.1/docs/index.html`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.0/docs/model.html` & `dragonfly-schema-1.9.1/docs/model.html`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.0/docs.py` & `dragonfly-schema-1.9.1/docs.py`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.0/dragonfly_schema/energy/properties.py` & `dragonfly-schema-1.9.1/dragonfly_schema/energy/properties.py`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.0/dragonfly_schema/model.py` & `dragonfly-schema-1.9.1/dragonfly_schema/model.py`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.0/dragonfly_schema/radiance/gridpar.py` & `dragonfly-schema-1.9.1/dragonfly_schema/radiance/gridpar.py`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.0/dragonfly_schema/radiance/properties.py` & `dragonfly-schema-1.9.1/dragonfly_schema/radiance/properties.py`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.0/dragonfly_schema/roof.py` & `dragonfly-schema-1.9.1/dragonfly_schema/roof.py`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.0/dragonfly_schema/shading_parameter.py` & `dragonfly-schema-1.9.1/dragonfly_schema/shading_parameter.py`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.0/dragonfly_schema/skylight_parameter.py` & `dragonfly-schema-1.9.1/dragonfly_schema/skylight_parameter.py`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.0/dragonfly_schema/window_parameter.py` & `dragonfly-schema-1.9.1/dragonfly_schema/window_parameter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,28 @@
 """Window Parameters with instructions for generating windows."""
 from pydantic import Field, root_validator, constr, conlist, confloat
 from typing import List
 
 from honeybee_schema._base import NoExtraBaseModel
 
 
-class SingleWindow(NoExtraBaseModel):
+class _WindowParameterBase(NoExtraBaseModel):
+    """Base class for all window parameters."""
+
+    user_data: dict = Field(
+        default=None,
+        description='Optional dictionary of user data associated with the object.'
+        'All keys and values of this dictionary should be of a standard data '
+        'type to ensure correct serialization of the object (eg. str, float, '
+        'int, list). When a list is used, each item in the list will be assigned '
+        'to the generated Honeybee apertures.'
+    )
+
+
+class SingleWindow(_WindowParameterBase):
     """A single window in the wall center defined by a width * height."""
 
     type: constr(regex='^SingleWindow$') = 'SingleWindow'
 
     width: float = Field(
         ...,
         gt=0,
@@ -31,43 +44,43 @@
     sill_height: float = Field(
         1.0,
         gt=0,
         description='A number for the window sill height.'
     )
 
 
-class SimpleWindowArea(NoExtraBaseModel):
+class SimpleWindowArea(_WindowParameterBase):
     """A single window defined by an absolute area."""
 
     type: constr(regex='^SimpleWindowArea$') = 'SimpleWindowArea'
 
     window_area: float = Field(
         ...,
         gt=0,
         description='A number for the window area in current model units. '
         'If this area is larger than the area of the Wall that it is applied'
         'to, the window will fill the parent Wall at a 99 percent ratio.'
     )
 
 
-class SimpleWindowRatio(NoExtraBaseModel):
+class SimpleWindowRatio(_WindowParameterBase):
     """A single window defined by an area ratio with the base surface."""
 
     type: constr(regex='^SimpleWindowRatio$') = 'SimpleWindowRatio'
 
     window_ratio: float = Field(
         ...,
         gt=0,
         lt=1,
         description='A number between 0 and 1 for the ratio between the window '
         'area and the parent wall surface area.'
     )
 
 
-class RepeatingWindowRatio(NoExtraBaseModel):
+class RepeatingWindowRatio(_WindowParameterBase):
     """Repeating windows derived from an area ratio with the base wall."""
 
     type: constr(regex='^RepeatingWindowRatio$') = 'RepeatingWindowRatio'
 
     window_ratio: float = Field(
         ...,
         gt=0,
@@ -105,15 +118,15 @@
         0,
         ge=0,
         description='An optional number to create a single vertical separation '
         'between top and bottom windows.'
     )
 
 
-class RepeatingWindowWidthHeight(NoExtraBaseModel):
+class RepeatingWindowWidthHeight(_WindowParameterBase):
     """Repeating rectangular windows of a fixed width and height."""
 
     type: constr(regex='^RepeatingWindowWidthHeight$') = 'RepeatingWindowWidthHeight'
 
     window_height: float = Field(
         ...,
         gt=0,
@@ -146,15 +159,15 @@
         ge=0,
         description='A number for the target separation between individual window '
         'centerlines.  If this number is larger than the parent rectangle base, '
         'only one window will be produced.'
     )
 
 
-class RectangularWindows(NoExtraBaseModel):
+class RectangularWindows(_WindowParameterBase):
     """Several rectangular windows, defined by origin, width and height."""
 
     type: constr(regex='^RectangularWindows$') = 'RectangularWindows'
 
     origins: List[conlist(confloat(gt=0), min_items=2, max_items=2)] = Field(
         ...,
         min_items=1,
@@ -199,15 +212,15 @@
             'RectangularWindows origins, widths, and heights ' \
             'must match. origins: {}, widths: {}, heights: {}'.format(
                 len(origins), len(widths), len(heights))
 
         return values
 
 
-class DetailedWindows(NoExtraBaseModel):
+class DetailedWindows(_WindowParameterBase):
     """Several detailed windows defined by 2D Polygons (lists of 2D vertices)."""
 
     type: constr(regex='^DetailedWindows$') = 'DetailedWindows'
 
     polygons: List[
         conlist(conlist(confloat(gt=0), min_items=2, max_items=3), min_items=3)
     ] = Field(
```

### Comparing `dragonfly-schema-1.9.0/dragonfly_schema.egg-info/PKG-INFO` & `dragonfly-schema-1.9.1/dragonfly_schema.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dragonfly-schema
-Version: 1.9.0
+Version: 1.9.1
 Summary: Dragonfly Data-Model Objects
 Home-page: https://github.com/ladybug-tools/dragonfly-schema
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Operating System :: OS Independent
```

### Comparing `dragonfly-schema-1.9.0/dragonfly_schema.egg-info/SOURCES.txt` & `dragonfly-schema-1.9.1/dragonfly_schema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.0/samples/building_simple.json` & `dragonfly-schema-1.9.1/samples/building_simple.json`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.0/samples/context_shade_two_tree_canopy.json` & `dragonfly-schema-1.9.1/samples/context_shade_two_tree_canopy.json`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.0/samples/model_complete_simple.dfjson` & `dragonfly-schema-1.9.1/samples/model_complete_simple.dfjson`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.0/samples/model_with_doors_skylights.dfjson` & `dragonfly-schema-1.9.1/samples/model_with_doors_skylights.dfjson`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.0/samples/room2d_simple.json` & `dragonfly-schema-1.9.1/samples/room2d_simple.json`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.0/samples/story_air_boundary.json` & `dragonfly-schema-1.9.1/samples/story_air_boundary.json`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.0/samples/story_simple.json` & `dragonfly-schema-1.9.1/samples/story_simple.json`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.0/samples/window_par_detailed_windows.json` & `dragonfly-schema-1.9.1/samples/window_par_detailed_windows.json`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.0/scripts/export_samples.py` & `dragonfly-schema-1.9.1/scripts/export_samples.py`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.0/scripts/sample_model.py` & `dragonfly-schema-1.9.1/scripts/sample_model.py`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.0/scripts/sample_shading_par.py` & `dragonfly-schema-1.9.1/scripts/sample_shading_par.py`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.0/scripts/sample_window_par.py` & `dragonfly-schema-1.9.1/scripts/sample_window_par.py`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.0/setup.py` & `dragonfly-schema-1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.0/tests/test_model.py` & `dragonfly-schema-1.9.1/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.0/tests/test_shading_parameter.py` & `dragonfly-schema-1.9.1/tests/test_shading_parameter.py`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.0/tests/test_window_parameter.py` & `dragonfly-schema-1.9.1/tests/test_window_parameter.py`

 * *Files identical despite different names*

