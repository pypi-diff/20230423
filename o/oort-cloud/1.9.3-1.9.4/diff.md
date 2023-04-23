# Comparing `tmp/oort-cloud-1.9.3.tar.gz` & `tmp/oort-cloud-1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oort-cloud-1.9.3.tar", last modified: Fri Aug 20 09:43:05 2021, max compression
+gzip compressed data, was "oort-cloud-1.9.4.tar", last modified: Sat Oct  9 08:31:53 2021, max compression
```

## Comparing `oort-cloud-1.9.3.tar` & `oort-cloud-1.9.4.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-20 09:43:05.293046 oort-cloud-1.9.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      337 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2109 2021-08-20 09:43:05.293046 oort-cloud-1.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1000 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-20 09:43:05.281046 oort-cloud-1.9.3/oort/
--rw-r--r--   0 runner    (1001) docker     (121)       37 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/oort/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-20 09:43:05.281046 oort-cloud-1.9.3/oort/cli/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/oort/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15519 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/oort/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    10237 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/oort/cli/folders.py
--rw-r--r--   0 runner    (1001) docker     (121)     2045 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/oort/cli/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1681 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/oort/cli/options.py
--rw-r--r--   0 runner    (1001) docker     (121)     7173 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/oort/cli/supervisor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-20 09:43:05.281046 oort-cloud-1.9.3/oort/server/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/oort/server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-20 09:43:05.281046 oort-cloud-1.9.3/oort/server/app/
--rw-r--r--   0 runner    (1001) docker     (121)      376 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/oort/server/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6125 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/oort/server/app/context.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-20 09:43:05.277046 oort-cloud-1.9.3/oort/server/app/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-20 09:43:05.281046 oort-cloud-1.9.3/oort/server/app/static/css/
--rw-r--r--   0 runner    (1001) docker     (121)    31030 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/oort/server/app/static/css/font-awesome.min.css
--rw-r--r--   0 runner    (1001) docker     (121)    15097 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/oort/server/app/static/css/main.css
--rw-r--r--   0 runner    (1001) docker     (121)     1891 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/oort/server/app/static/css/oort.css
--rw-r--r--   0 runner    (1001) docker     (121)    78366 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/oort/server/app/static/css/style.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-20 09:43:05.285046 oort-cloud-1.9.3/oort/server/app/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (121)   444379 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/oort/server/app/static/fonts/fontawesome-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (121)   165548 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/oort/server/app/static/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (121)    98024 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/oort/server/app/static/fonts/fontawesome-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (121)    77160 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/oort/server/app/static/fonts/fontawesome-webfont.woff2
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-20 09:43:05.285046 oort-cloud-1.9.3/oort/server/app/static/img/
--rw-r--r--   0 runner    (1001) docker     (121)    26318 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/oort/server/app/static/img/favicon-310.png
--rw-r--r--   0 runner    (1001) docker     (121)     1806 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/oort/server/app/static/img/icon-dataset-xsmall.png
--rw-r--r--   0 runner    (1001) docker     (121)    30968 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/oort/server/app/static/img/icon-dataset.png
--rw-r--r--   0 runner    (1001) docker     (121)   101527 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/oort/server/app/static/img/icon-night-log.png
--rw-r--r--   0 runner    (1001) docker     (121)   530710 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/oort/server/app/static/img/icon-observing-run.png
--rw-r--r--   0 runner    (1001) docker     (121)   127792 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/oort/server/app/static/img/icon-observing-site.png
--rw-r--r--   0 runner    (1001) docker     (121)   113035 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/oort/server/app/static/img/icon-smalltelescope.png
--rw-r--r--   0 runner    (1001) docker     (121)   144021 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/oort/server/app/static/img/icon-telescope.png
--rw-r--r--   0 runner    (1001) docker     (121)    11009 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/oort/server/app/static/img/logo-circle.png
--rw-r--r--   0 runner    (1001) docker     (121)    12768 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/oort/server/app/static/img/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-20 09:43:05.289046 oort-cloud-1.9.3/oort/server/app/static/js/
--rw-r--r--   0 runner    (1001) docker     (121)     2806 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/oort/server/app/static/js/active-table.js
--rw-r--r--   0 runner    (1001) docker     (121)     1972 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/oort/server/app/static/js/errors-table.js
--rw-r--r--   0 runner    (1001) docker     (121)     2452 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/oort/server/app/static/js/finished-table.js
--rw-r--r--   0 runner    (1001) docker     (121)     2101 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/oort/server/app/static/js/main-app.js
--rw-r--r--   0 runner    (1001) docker     (121)     1144 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/oort/server/app/static/js/pending-table.js
--rw-r--r--   0 runner    (1001) docker     (121)     2028 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/oort/server/app/static/js/utils.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-20 09:43:05.289046 oort-cloud-1.9.3/oort/server/app/templates/
--rw-r--r--   0 runner    (1001) docker     (121)    11296 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/oort/server/app/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (121)     2518 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/oort/server/app/views.py
--rw-r--r--   0 runner    (1001) docker     (121)     2513 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/oort/server/errors.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1220 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/oort/server/main.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-20 09:43:05.289046 oort-cloud-1.9.3/oort/server/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/oort/server/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      723 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/oort/server/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-20 09:43:05.289046 oort-cloud-1.9.3/oort/shared/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/oort/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4727 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/oort/shared/config.py
--rw-r--r--   0 runner    (1001) docker     (121)      966 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/oort/shared/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)      149 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/oort/shared/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     3407 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/oort/shared/identity.py
--rw-r--r--   0 runner    (1001) docker     (121)     6338 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/oort/shared/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     3146 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/oort/shared/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-20 09:43:05.289046 oort-cloud-1.9.3/oort/uploader/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/oort/uploader/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-20 09:43:05.289046 oort-cloud-1.9.3/oort/uploader/engine/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/oort/uploader/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      452 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/oort/uploader/engine/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     3405 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/oort/uploader/engine/eventhandler.py
--rw-r--r--   0 runner    (1001) docker     (121)    13534 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/oort/uploader/engine/packer.py
--rw-r--r--   0 runner    (1001) docker     (121)     5077 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/oort/uploader/engine/pathsobserver.py
--rw-r--r--   0 runner    (1001) docker     (121)     8681 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/oort/uploader/engine/preparator.py
--rw-r--r--   0 runner    (1001) docker     (121)     8220 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/oort/uploader/engine/uploader.py
--rw-r--r--   0 runner    (1001) docker     (121)     2401 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/oort/uploader/engine/walker.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2548 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/oort/uploader/engine/zipper.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1192 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/oort/uploader/main.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-20 09:43:05.293046 oort-cloud-1.9.3/oort_cloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2109 2021-08-20 09:43:05.000000 oort-cloud-1.9.3/oort_cloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2738 2021-08-20 09:43:05.000000 oort-cloud-1.9.3/oort_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-20 09:43:05.000000 oort-cloud-1.9.3/oort_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       44 2021-08-20 09:43:05.000000 oort-cloud-1.9.3/oort_cloud.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-20 09:43:05.000000 oort-cloud-1.9.3/oort_cloud.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      105 2021-08-20 09:43:05.000000 oort-cloud-1.9.3/oort_cloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2021-08-20 09:43:05.000000 oort-cloud-1.9.3/oort_cloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       67 2021-08-20 09:43:05.297046 oort-cloud-1.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1987 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-20 09:43:05.293046 oort-cloud-1.9.3/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-20 09:43:05.293046 oort-cloud-1.9.3/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/tests/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5187 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/tests/cli/test_cli_folders_parse.py
--rw-r--r--   0 runner    (1001) docker     (121)     1854 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/tests/cli/test_cli_folders_save.py
--rw-r--r--   0 runner    (1001) docker     (121)      516 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/tests/cli/test_cli_options.py
--rw-r--r--   0 runner    (1001) docker     (121)     2027 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/tests/cli/test_cli_supervisor.py
--rw-r--r--   0 runner    (1001) docker     (121)     4142 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/tests/cli/test_cli_upload.py
--rw-r--r--   0 runner    (1001) docker     (121)     3175 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/tests/cli/test_cli_watch.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-20 09:43:05.293046 oort-cloud-1.9.3/tests/server/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/tests/server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-20 09:43:05.293046 oort-cloud-1.9.3/tests/uploader/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/tests/uploader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1471 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/tests/uploader/test_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)     1306 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/tests/uploader/test_observer.py
--rw-r--r--   0 runner    (1001) docker     (121)    18611 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/tests/uploader/test_packer.py
--rw-r--r--   0 runner    (1001) docker     (121)     5353 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/tests/uploader/test_preparator.py
--rw-r--r--   0 runner    (1001) docker     (121)     3433 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/tests/uploader/test_uploader.py
--rw-r--r--   0 runner    (1001) docker     (121)     1708 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/tests/uploader/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3512 2021-08-20 09:42:55.000000 oort-cloud-1.9.3/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-09 08:31:53.448262 oort-cloud-1.9.4/
+-rw-r--r--   0 runner    (1001) docker     (121)     1069 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      337 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1963 2021-10-09 08:31:53.448262 oort-cloud-1.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1000 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-09 08:31:53.436262 oort-cloud-1.9.4/oort/
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/oort/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-09 08:31:53.436262 oort-cloud-1.9.4/oort/cli/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/oort/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15519 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/oort/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10237 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/oort/cli/folders.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2045 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/oort/cli/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1681 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/oort/cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7173 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/oort/cli/supervisor.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-09 08:31:53.436262 oort-cloud-1.9.4/oort/server/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/oort/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-09 08:31:53.436262 oort-cloud-1.9.4/oort/server/app/
+-rw-r--r--   0 runner    (1001) docker     (121)      376 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/oort/server/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6125 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/oort/server/app/context.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-09 08:31:53.432262 oort-cloud-1.9.4/oort/server/app/static/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-09 08:31:53.436262 oort-cloud-1.9.4/oort/server/app/static/css/
+-rw-r--r--   0 runner    (1001) docker     (121)    31030 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/oort/server/app/static/css/font-awesome.min.css
+-rw-r--r--   0 runner    (1001) docker     (121)    15097 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/oort/server/app/static/css/main.css
+-rw-r--r--   0 runner    (1001) docker     (121)     1891 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/oort/server/app/static/css/oort.css
+-rw-r--r--   0 runner    (1001) docker     (121)    78366 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/oort/server/app/static/css/style.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-09 08:31:53.436262 oort-cloud-1.9.4/oort/server/app/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (121)   444379 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/oort/server/app/static/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (121)   165548 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/oort/server/app/static/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (121)    98024 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/oort/server/app/static/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (121)    77160 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/oort/server/app/static/fonts/fontawesome-webfont.woff2
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-09 08:31:53.440262 oort-cloud-1.9.4/oort/server/app/static/img/
+-rw-r--r--   0 runner    (1001) docker     (121)    26318 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/oort/server/app/static/img/favicon-310.png
+-rw-r--r--   0 runner    (1001) docker     (121)     1806 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/oort/server/app/static/img/icon-dataset-xsmall.png
+-rw-r--r--   0 runner    (1001) docker     (121)    30968 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/oort/server/app/static/img/icon-dataset.png
+-rw-r--r--   0 runner    (1001) docker     (121)   101527 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/oort/server/app/static/img/icon-night-log.png
+-rw-r--r--   0 runner    (1001) docker     (121)   530710 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/oort/server/app/static/img/icon-observing-run.png
+-rw-r--r--   0 runner    (1001) docker     (121)   127792 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/oort/server/app/static/img/icon-observing-site.png
+-rw-r--r--   0 runner    (1001) docker     (121)   113035 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/oort/server/app/static/img/icon-smalltelescope.png
+-rw-r--r--   0 runner    (1001) docker     (121)   144021 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/oort/server/app/static/img/icon-telescope.png
+-rw-r--r--   0 runner    (1001) docker     (121)    11009 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/oort/server/app/static/img/logo-circle.png
+-rw-r--r--   0 runner    (1001) docker     (121)    12768 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/oort/server/app/static/img/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-09 08:31:53.440262 oort-cloud-1.9.4/oort/server/app/static/js/
+-rw-r--r--   0 runner    (1001) docker     (121)     2806 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/oort/server/app/static/js/active-table.js
+-rw-r--r--   0 runner    (1001) docker     (121)     1972 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/oort/server/app/static/js/errors-table.js
+-rw-r--r--   0 runner    (1001) docker     (121)     2452 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/oort/server/app/static/js/finished-table.js
+-rw-r--r--   0 runner    (1001) docker     (121)     2101 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/oort/server/app/static/js/main-app.js
+-rw-r--r--   0 runner    (1001) docker     (121)     1144 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/oort/server/app/static/js/pending-table.js
+-rw-r--r--   0 runner    (1001) docker     (121)     2028 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/oort/server/app/static/js/utils.js
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-09 08:31:53.440262 oort-cloud-1.9.4/oort/server/app/templates/
+-rw-r--r--   0 runner    (1001) docker     (121)    11296 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/oort/server/app/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (121)     2518 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/oort/server/app/views.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2513 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/oort/server/errors.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1220 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/oort/server/main.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-09 08:31:53.440262 oort-cloud-1.9.4/oort/server/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/oort/server/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      723 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/oort/server/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-09 08:31:53.444262 oort-cloud-1.9.4/oort/shared/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/oort/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4727 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/oort/shared/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)      966 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/oort/shared/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)      149 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/oort/shared/errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3407 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/oort/shared/identity.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6338 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/oort/shared/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3146 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/oort/shared/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-09 08:31:53.444262 oort-cloud-1.9.4/oort/uploader/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/oort/uploader/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-09 08:31:53.444262 oort-cloud-1.9.4/oort/uploader/engine/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/oort/uploader/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      452 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/oort/uploader/engine/errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3405 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/oort/uploader/engine/eventhandler.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13534 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/oort/uploader/engine/packer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5077 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/oort/uploader/engine/pathsobserver.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8681 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/oort/uploader/engine/preparator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8789 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/oort/uploader/engine/uploader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2419 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/oort/uploader/engine/walker.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2548 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/oort/uploader/engine/zipper.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1192 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/oort/uploader/main.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-09 08:31:53.444262 oort-cloud-1.9.4/oort_cloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1963 2021-10-09 08:31:53.000000 oort-cloud-1.9.4/oort_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2738 2021-10-09 08:31:53.000000 oort-cloud-1.9.4/oort_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-09 08:31:53.000000 oort-cloud-1.9.4/oort_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       44 2021-10-09 08:31:53.000000 oort-cloud-1.9.4/oort_cloud.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-09 08:31:53.000000 oort-cloud-1.9.4/oort_cloud.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2021-10-09 08:31:53.000000 oort-cloud-1.9.4/oort_cloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       11 2021-10-09 08:31:53.000000 oort-cloud-1.9.4/oort_cloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       67 2021-10-09 08:31:53.448262 oort-cloud-1.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2147 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-09 08:31:53.444262 oort-cloud-1.9.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-09 08:31:53.444262 oort-cloud-1.9.4/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/tests/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5187 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/tests/cli/test_cli_folders_parse.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1854 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/tests/cli/test_cli_folders_save.py
+-rw-r--r--   0 runner    (1001) docker     (121)      516 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/tests/cli/test_cli_options.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2137 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/tests/cli/test_cli_supervisor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4142 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/tests/cli/test_cli_upload.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3175 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/tests/cli/test_cli_watch.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-09 08:31:53.444262 oort-cloud-1.9.4/tests/server/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/tests/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-09 08:31:53.448262 oort-cloud-1.9.4/tests/uploader/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/tests/uploader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1471 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/tests/uploader/test_handler.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1306 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/tests/uploader/test_observer.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18611 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/tests/uploader/test_packer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5353 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/tests/uploader/test_preparator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3433 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/tests/uploader/test_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1708 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/tests/uploader/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3512 2021-10-09 08:31:45.000000 oort-cloud-1.9.4/tests/utils.py
```

### Comparing `oort-cloud-1.9.3/LICENSE` & `oort-cloud-1.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/PKG-INFO` & `oort-cloud-1.9.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,61 +1,67 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: oort-cloud
-Version: 1.9.3
+Version: 1.9.4
 Summary: Oort utility to upload all your files in Arcsecond.io's cloud storage.
 Home-page: https://github.com/arcsecond-io/oort
 Author: Cedric Foellmi
 Author-email: cedric@arcsecond.io
 License: MIT
-Description: # Oort-Cloud for Arcsecond
-        
-        Oort-Cloud is the open-source super-easy-to-use tool for automatically and
-        continuously uploading to [Arcsecond.io](https://www.arcsecond.io) files
-        that are inside a folder.
-        
-        [Arcsecond.io](https://www.arcsecond.io) is a comprehensive cloud platform 
-        for astronomical observations, for individual astronomers, collaborations and 
-        observatories.
-        
-        ## Usage
-        
-        Use pip (see [this page](https://pip.pypa.io/en/stable/installing/) on how to install pip, if you haven't done so):
-        
-        ```bash
-        $ pip install oort-cloud
-        ```
-        
-        Install for the user only (non-root):
-        
-        ```bash
-        $ pip install oort-cloud --user
-        ```
-        
-        Upgrade oort-cloud:
-        
-        ```bash
-        $ pip install oort-cloud --upgrade
-        ```
-        
-        Almost no-step-3 usage (the first one is to login to Arcsecond.io if not yet done):
-        
-        ```bash
-        oort login
-        oort restart
-        oort watch [OPTIONS] folder1 folder2 ...
-        ```
-        
-        See [detailed documentation](https://arcsecond-io.github.io/oort/) for a complete
-        description of all options and capabilities, with screenshots.
-        
 Platform: any
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+License-File: LICENSE
+
+# Oort-Cloud for Arcsecond
+
+Oort-Cloud is the open-source super-easy-to-use tool for automatically and
+continuously uploading to [Arcsecond.io](https://www.arcsecond.io) files
+that are inside a folder.
+
+[Arcsecond.io](https://www.arcsecond.io) is a comprehensive cloud platform 
+for astronomical observations, for individual astronomers, collaborations and 
+observatories.
+
+## Usage
+
+Use pip (see [this page](https://pip.pypa.io/en/stable/installing/) on how to install pip, if you haven't done so):
+
+```bash
+$ pip install oort-cloud
+```
+
+Install for the user only (non-root):
+
+```bash
+$ pip install oort-cloud --user
+```
+
+Upgrade oort-cloud:
+
+```bash
+$ pip install oort-cloud --upgrade
+```
+
+Almost no-step-3 usage (the first one is to login to Arcsecond.io if not yet done):
+
+```bash
+oort login
+oort restart
+oort watch [OPTIONS] folder1 folder2 ...
+```
+
+See [detailed documentation](https://arcsecond-io.github.io/oort/) for a complete
+description of all options and capabilities, with screenshots.
+
+
```

### Comparing `oort-cloud-1.9.3/README.md` & `oort-cloud-1.9.4/README.md`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/oort/cli/cli.py` & `oort-cloud-1.9.4/oort/cli/cli.py`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/oort/cli/folders.py` & `oort-cloud-1.9.4/oort/cli/folders.py`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/oort/cli/helpers.py` & `oort-cloud-1.9.4/oort/cli/helpers.py`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/oort/cli/options.py` & `oort-cloud-1.9.4/oort/cli/options.py`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/oort/cli/supervisor.py` & `oort-cloud-1.9.4/oort/cli/supervisor.py`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/oort/server/app/context.py` & `oort-cloud-1.9.4/oort/server/app/context.py`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/oort/server/app/static/css/font-awesome.min.css` & `oort-cloud-1.9.4/oort/server/app/static/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/oort/server/app/static/css/main.css` & `oort-cloud-1.9.4/oort/server/app/static/css/main.css`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/oort/server/app/static/css/oort.css` & `oort-cloud-1.9.4/oort/server/app/static/css/oort.css`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/oort/server/app/static/css/style.css` & `oort-cloud-1.9.4/oort/server/app/static/css/style.css`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/oort/server/app/static/fonts/fontawesome-webfont.svg` & `oort-cloud-1.9.4/oort/server/app/static/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/oort/server/app/static/fonts/fontawesome-webfont.ttf` & `oort-cloud-1.9.4/oort/server/app/static/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/oort/server/app/static/fonts/fontawesome-webfont.woff` & `oort-cloud-1.9.4/oort/server/app/static/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/oort/server/app/static/fonts/fontawesome-webfont.woff2` & `oort-cloud-1.9.4/oort/server/app/static/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/oort/server/app/static/img/favicon-310.png` & `oort-cloud-1.9.4/oort/server/app/static/img/favicon-310.png`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/oort/server/app/static/img/icon-dataset-xsmall.png` & `oort-cloud-1.9.4/oort/server/app/static/img/icon-dataset-xsmall.png`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/oort/server/app/static/img/icon-dataset.png` & `oort-cloud-1.9.4/oort/server/app/static/img/icon-dataset.png`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/oort/server/app/static/img/icon-night-log.png` & `oort-cloud-1.9.4/oort/server/app/static/img/icon-night-log.png`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/oort/server/app/static/img/icon-observing-run.png` & `oort-cloud-1.9.4/oort/server/app/static/img/icon-observing-run.png`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/oort/server/app/static/img/icon-observing-site.png` & `oort-cloud-1.9.4/oort/server/app/static/img/icon-observing-site.png`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/oort/server/app/static/img/icon-smalltelescope.png` & `oort-cloud-1.9.4/oort/server/app/static/img/icon-smalltelescope.png`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/oort/server/app/static/img/icon-telescope.png` & `oort-cloud-1.9.4/oort/server/app/static/img/icon-telescope.png`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/oort/server/app/static/img/logo-circle.png` & `oort-cloud-1.9.4/oort/server/app/static/img/logo-circle.png`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/oort/server/app/static/img/logo.png` & `oort-cloud-1.9.4/oort/server/app/static/img/logo.png`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/oort/server/app/static/js/active-table.js` & `oort-cloud-1.9.4/oort/server/app/static/js/active-table.js`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/oort/server/app/static/js/errors-table.js` & `oort-cloud-1.9.4/oort/server/app/static/js/errors-table.js`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/oort/server/app/static/js/finished-table.js` & `oort-cloud-1.9.4/oort/server/app/static/js/finished-table.js`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/oort/server/app/static/js/main-app.js` & `oort-cloud-1.9.4/oort/server/app/static/js/main-app.js`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/oort/server/app/static/js/pending-table.js` & `oort-cloud-1.9.4/oort/server/app/static/js/pending-table.js`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/oort/server/app/static/js/utils.js` & `oort-cloud-1.9.4/oort/server/app/static/js/utils.js`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/oort/server/app/templates/index.html` & `oort-cloud-1.9.4/oort/server/app/templates/index.html`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/oort/server/app/views.py` & `oort-cloud-1.9.4/oort/server/app/views.py`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/oort/server/errors.py` & `oort-cloud-1.9.4/oort/server/errors.py`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/oort/server/main.py` & `oort-cloud-1.9.4/oort/server/main.py`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/oort/server/tests/conftest.py` & `oort-cloud-1.9.4/oort/server/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/oort/shared/config.py` & `oort-cloud-1.9.4/oort/shared/config.py`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/oort/shared/constants.py` & `oort-cloud-1.9.4/oort/shared/constants.py`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/oort/shared/identity.py` & `oort-cloud-1.9.4/oort/shared/identity.py`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/oort/shared/models.py` & `oort-cloud-1.9.4/oort/shared/models.py`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/oort/shared/utils.py` & `oort-cloud-1.9.4/oort/shared/utils.py`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/oort/uploader/engine/eventhandler.py` & `oort-cloud-1.9.4/oort/uploader/engine/eventhandler.py`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/oort/uploader/engine/packer.py` & `oort-cloud-1.9.4/oort/uploader/engine/packer.py`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/oort/uploader/engine/pathsobserver.py` & `oort-cloud-1.9.4/oort/uploader/engine/pathsobserver.py`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/oort/uploader/engine/preparator.py` & `oort-cloud-1.9.4/oort/uploader/engine/preparator.py`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/oort/uploader/engine/uploader.py` & `oort-cloud-1.9.4/oort/uploader/engine/uploader.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,36 +41,27 @@
                 self._upload.smart_update(status=Status.UPLOADING.value,
                                           substatus=Substatus.UPLOADING.value,
                                           progress=progress_percent,
                                           duration=duration)
                 if self._display_progress is True:
                     print(f"{progress_percent:.2f}% ({duration:.2f} sec)", end="\r")
 
-        ffps = str(self._final_file_path)
-
-        tag_filepath = f'filepath|{ffps}'
-        tag_folder = f'folder|{self._pack.clean_folder_name}'
-        tag_root = f'root|{self._pack.root_folder_name}'
-        tag_origin = f'origin|{socket.gethostname()}|'
-        tag_uploader = f'uploader|{ArcsecondAPI.username()}'
-        tag_oort = f'oort|{__version__}'
-
-        payload = {'file': ffps, 'tags': [tag_filepath, tag_folder, tag_root, tag_origin, tag_uploader, tag_oort]}
-
         self._async_file_uploader: AsyncFileUploader
         if remote_resource_exists:
             self._logger.info(f"{self.log_prefix} Remote resource exists. Preparing 'Update' APIs.")
-            self._async_file_uploader, error = self._api.update(self._final_file_path.name, payload,
+            self._async_file_uploader, error = self._api.update(self._final_file_path.name,
+                                                                {'file': str(self._final_file_path)},
                                                                 callback=update_upload_progress)
         else:
             self._logger.info(f"{self.log_prefix} Remote resource does not exist. Preparing 'Create' APIs.")
-            self._async_file_uploader, error = self._api.create(payload, callback=update_upload_progress)
+            self._async_file_uploader, error = self._api.create({'file': str(self._final_file_path)},
+                                                                callback=update_upload_progress)
 
         if error is not None:
-            msg = f'{self.log_prefix} API preparation error for {ffps}: {str(error)}'
+            msg = f'{self.log_prefix} API preparation error for {str(self._final_file_path)}: {str(error)}'
             self._logger.error(msg)
 
     def _check_remote_resource_and_file(self):
         _remote_resource_exists = False
         _remote_resource_has_file = False
 
         # self._api contains a reference to the dataset.
@@ -89,15 +80,15 @@
             _remote_resource_has_file = 's3.amazonaws.com' in response.get('file', '')
 
         if _remote_resource_has_file is False:
             self._prepare_file_uploader(_remote_resource_exists)
 
         return _remote_resource_has_file
 
-    def _check(self):
+    def _should_perform_upload(self):
         _should_perform = False
         self._upload.smart_update(started=datetime.now())
 
         try:
             self._upload.smart_update(status=Status.UPLOADING.value, substatus=Substatus.CHECKING.value)
             exists_remotely = self._check_remote_resource_and_file()
 
@@ -115,15 +106,15 @@
                 self._logger.info(f'{self.log_prefix} Already synced.')
                 self._upload.smart_update(status=Status.OK.value, substatus=Substatus.ALREADY_SYNCED.value)
             else:
                 _should_perform = True
 
         return _should_perform
 
-    def _process_error(self, error):
+    def _process_upload_error(self, error):
         status, substatus, error = Status.ERROR.value, Substatus.ERROR.value, str(error)
 
         try:
             error_body = json.loads(error)
         except Exception as err:
             self._logger.error(str(err))
         else:
@@ -131,40 +122,57 @@
                 detail = error_body['detail']
                 error_content = detail[0] if isinstance(detail, list) and len(detail) > 0 else detail
                 if 'already exists in dataset' in error_content:
                     status, substatus, error = Status.OK.value, Substatus.ALREADY_SYNCED.value, ''
 
         self._upload.smart_update(status=status, substatus=substatus, error=error)
 
-    def upload_file(self):
-        self._logger.info(f'{self.log_prefix} Opening upload sequence.')
-
-        if not self._check():
-            return
-
+    def _perform_upload(self):
         self._upload.smart_update(status=Status.UPLOADING.value, substatus=Substatus.STARTING.value, error='')
-        self._logger.info(f'{self.log_prefix} Starting upload ({self._upload.get_formatted_size()})')
+
+        file_size = self._upload.get_formatted_size()
+        self._logger.info(f'{self.log_prefix} Starting upload ({file_size})')
 
         self._async_file_uploader.start()
         _, upload_error = self._async_file_uploader.finish()
 
         ended = datetime.now()
-        self._upload.smart_update(ended=ended, progress=0, duration=(ended - self._upload.started).total_seconds())
+        duration = (ended - self._upload.started).total_seconds()
+        self._upload.smart_update(ended=ended, progress=0, duration=duration)
 
         if upload_error:
             self._logger.info(f'{self.log_prefix} {str(upload_error)}')
-            self._process_error(upload_error)
+            self._process_upload_error(upload_error)
         else:
-            msg = f'{self.log_prefix} Successfully uploaded {self._upload.get_formatted_size()}'
-            msg += f' in {self._upload.duration} seconds.'
-            self._logger.info(msg)
+            self._logger.info(f'{self.log_prefix} Successfully uploaded {file_size} in {duration} seconds.')
             self._upload.smart_update(status=Status.OK.value, substatus=Substatus.DONE.value, error='')
 
+    def _update_file_tags(self):
+        tag_filepath = f'oort|filepath|{str(self._final_file_path)}'
+        tag_folder = f'oort|folder|{self._pack.clean_folder_name}'
+        tag_root = f'oort|root|{self._pack.root_folder_name}'
+        tag_origin = f'oort|origin|{socket.gethostname()}|'
+        tag_uploader = f'oort|uploader|{ArcsecondAPI.username()}'
+        tag_oort = f'oort|version|{__version__}'
+
+        tags = [tag_filepath, tag_folder, tag_root, tag_origin, tag_uploader, tag_oort]
+        _, error = self._api.update(self._final_file_path.name, {'tags': tags})
+
+        if error is not None:
+            self._logger.error(f'{self.log_prefix} {str(error)}')
+
+    def upload_file(self):
+        self._logger.info(f'{self.log_prefix} Opening upload sequence.')
+        if self._should_perform_upload():
+            self._perform_upload()
         self._logger.info(f'{self.log_prefix} Closing upload sequence.')
 
+        self._logger.info(f'{self.log_prefix} Updating file tags.')
+        self._update_file_tags()
+
     @property
     def is_started(self):
         return self._upload.started is not None and self._upload.ended is None
 
     @property
     def is_finished(self):
         return self._upload.started is not None and self._upload.ended is not None
```

### Comparing `oort-cloud-1.9.3/oort/uploader/engine/walker.py` & `oort-cloud-1.9.4/oort/uploader/engine/walker.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 from oort.shared.config import get_oort_logger
 from oort.shared.identity import Identity
 from oort.shared.models import Status
 from oort.shared.utils import is_hidden
 from oort.uploader.engine import packer
 
 
-def walk(folder_path: str, identity: Identity, force, debug: bool):
+def walk(folder_string: str, identity: Identity, force, debug: bool):
     if identity.subdomain:
         check_remote_organisation(identity.subdomain, debug, verbose=False)
 
     log_prefix = '[Walker]'
     logger = get_oort_logger('walker', debug=debug)
-    logger.info(f"{log_prefix} Starting upload walk through {folder_path} and its subfolders...")
+    logger.info(f"{log_prefix} Starting upload walk through {folder_string} and its subfolders...")
     logger.warn(f"{log_prefix} Force flag is {'True' if force else 'False'}")
 
-    root_path = Path(folder_path)
+    root_path = Path(folder_string).resolve()
     # Just in case we pass a file...
     if root_path.is_file():
         root_path = root_path.parent
 
     failed_uploads = []
     success_uploads = []
 
@@ -40,15 +40,15 @@
         pack = packer.UploadPack(str(root_path), str(file_path), identity, force=force)
         status, substatus, error = pack.prepare_and_upload_file(display_progress=True)
         if status == Status.OK.value:
             success_uploads.append(str(file_path))
         else:
             failed_uploads.append((str(file_path), substatus, error))
 
-    msg = f'{log_prefix} Finished upload walk inside folder {folder_path} '
+    msg = f'{log_prefix} Finished upload walk inside folder {folder_string} '
     msg += f'with {len(success_uploads)} successful uploads and {len(failed_uploads)} failed.'
     logger.info(msg)
 
     if len(failed_uploads) > 0:
         logger.error(f'{log_prefix} Here are the failed uploads:')
         for path, substatus, error in failed_uploads:
             logger.error(f'{path} ({substatus}) {error}')
```

### Comparing `oort-cloud-1.9.3/oort/uploader/engine/zipper.py` & `oort-cloud-1.9.4/oort/uploader/engine/zipper.py`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/oort/uploader/main.py` & `oort-cloud-1.9.4/oort/uploader/main.py`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/oort_cloud.egg-info/PKG-INFO` & `oort-cloud-1.9.4/oort_cloud.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,61 +1,67 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: oort-cloud
-Version: 1.9.3
+Version: 1.9.4
 Summary: Oort utility to upload all your files in Arcsecond.io's cloud storage.
 Home-page: https://github.com/arcsecond-io/oort
 Author: Cedric Foellmi
 Author-email: cedric@arcsecond.io
 License: MIT
-Description: # Oort-Cloud for Arcsecond
-        
-        Oort-Cloud is the open-source super-easy-to-use tool for automatically and
-        continuously uploading to [Arcsecond.io](https://www.arcsecond.io) files
-        that are inside a folder.
-        
-        [Arcsecond.io](https://www.arcsecond.io) is a comprehensive cloud platform 
-        for astronomical observations, for individual astronomers, collaborations and 
-        observatories.
-        
-        ## Usage
-        
-        Use pip (see [this page](https://pip.pypa.io/en/stable/installing/) on how to install pip, if you haven't done so):
-        
-        ```bash
-        $ pip install oort-cloud
-        ```
-        
-        Install for the user only (non-root):
-        
-        ```bash
-        $ pip install oort-cloud --user
-        ```
-        
-        Upgrade oort-cloud:
-        
-        ```bash
-        $ pip install oort-cloud --upgrade
-        ```
-        
-        Almost no-step-3 usage (the first one is to login to Arcsecond.io if not yet done):
-        
-        ```bash
-        oort login
-        oort restart
-        oort watch [OPTIONS] folder1 folder2 ...
-        ```
-        
-        See [detailed documentation](https://arcsecond-io.github.io/oort/) for a complete
-        description of all options and capabilities, with screenshots.
-        
 Platform: any
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+License-File: LICENSE
+
+# Oort-Cloud for Arcsecond
+
+Oort-Cloud is the open-source super-easy-to-use tool for automatically and
+continuously uploading to [Arcsecond.io](https://www.arcsecond.io) files
+that are inside a folder.
+
+[Arcsecond.io](https://www.arcsecond.io) is a comprehensive cloud platform 
+for astronomical observations, for individual astronomers, collaborations and 
+observatories.
+
+## Usage
+
+Use pip (see [this page](https://pip.pypa.io/en/stable/installing/) on how to install pip, if you haven't done so):
+
+```bash
+$ pip install oort-cloud
+```
+
+Install for the user only (non-root):
+
+```bash
+$ pip install oort-cloud --user
+```
+
+Upgrade oort-cloud:
+
+```bash
+$ pip install oort-cloud --upgrade
+```
+
+Almost no-step-3 usage (the first one is to login to Arcsecond.io if not yet done):
+
+```bash
+oort login
+oort restart
+oort watch [OPTIONS] folder1 folder2 ...
+```
+
+See [detailed documentation](https://arcsecond-io.github.io/oort/) for a complete
+description of all options and capabilities, with screenshots.
+
+
```

### Comparing `oort-cloud-1.9.3/oort_cloud.egg-info/SOURCES.txt` & `oort-cloud-1.9.4/oort_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/setup.py` & `oort-cloud-1.9.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -45,20 +45,23 @@
     entry_points={
         'console_scripts': [
             'oort = oort.cli.cli:main',
         ],
     },
     classifiers=[
         # As from http://pypi.python.org/pypi?%3Aaction=list_classifiers
-        'Development Status :: 4 - Beta',
+        'Development Status :: 5 - Production/Stable',
         'Environment :: Console',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: MIT License',
         'Operating System :: POSIX',
         'Operating System :: MacOS',
         'Operating System :: Unix',
         'Operating System :: Microsoft :: Windows',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ]
 )
```

### Comparing `oort-cloud-1.9.3/tests/cli/test_cli_folders_parse.py` & `oort-cloud-1.9.4/tests/cli/test_cli_folders_parse.py`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/tests/cli/test_cli_folders_save.py` & `oort-cloud-1.9.4/tests/cli/test_cli_folders_save.py`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/tests/cli/test_cli_options.py` & `oort-cloud-1.9.4/tests/cli/test_cli_options.py`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/tests/cli/test_cli_supervisor.py` & `oort-cloud-1.9.4/tests/cli/test_cli_supervisor.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,16 @@
     stop_supervisor_processes
 )
 from oort.shared.config import get_oort_supervisor_conf_file_path
 
 
 def test_reconfigure_supervisor():
     supervisor_conf_file_path = get_oort_supervisor_conf_file_path()
-    supervisor_conf_file_path.unlink(missing_ok=True)
+    if supervisor_conf_file_path.exists():
+        supervisor_conf_file_path.unlink()  # avoid missing_ok=True parameter which doesn't exist in all Python versions
     reconfigure_supervisor()
     conf = ConfigParser()
     conf.read(str(supervisor_conf_file_path))
     sections = conf.sections()
     assert f'program:{DEFAULT_PROCESSES[0]}' in sections
     assert f'program:{DEFAULT_PROCESSES[1]}' in sections
     assert pathlib.Path(conf.get('program:' + DEFAULT_PROCESSES[0], 'command').split()[-1]).exists()
```

### Comparing `oort-cloud-1.9.3/tests/cli/test_cli_upload.py` & `oort-cloud-1.9.4/tests/cli/test_cli_upload.py`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/tests/cli/test_cli_watch.py` & `oort-cloud-1.9.4/tests/cli/test_cli_watch.py`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/tests/uploader/test_handler.py` & `oort-cloud-1.9.4/tests/uploader/test_handler.py`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/tests/uploader/test_observer.py` & `oort-cloud-1.9.4/tests/uploader/test_observer.py`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/tests/uploader/test_packer.py` & `oort-cloud-1.9.4/tests/uploader/test_packer.py`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/tests/uploader/test_preparator.py` & `oort-cloud-1.9.4/tests/uploader/test_preparator.py`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/tests/uploader/test_uploader.py` & `oort-cloud-1.9.4/tests/uploader/test_uploader.py`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/tests/uploader/test_utils.py` & `oort-cloud-1.9.4/tests/uploader/test_utils.py`

 * *Files identical despite different names*

### Comparing `oort-cloud-1.9.3/tests/utils.py` & `oort-cloud-1.9.4/tests/utils.py`

 * *Files identical despite different names*

