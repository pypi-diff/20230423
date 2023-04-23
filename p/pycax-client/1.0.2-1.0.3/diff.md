# Comparing `tmp/pycax-client-1.0.2.tar.gz` & `tmp/pycax-client-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycax-client-1.0.2.tar", last modified: Sat Apr 22 22:48:27 2023, max compression
+gzip compressed data, was "pycax-client-1.0.3.tar", last modified: Sun Apr 23 18:32:03 2023, max compression
```

## Comparing `pycax-client-1.0.2.tar` & `pycax-client-1.0.3.tar`

### file list

```diff
@@ -1,67 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:48:27.583400 pycax-client-1.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:48:27.575400 pycax-client-1.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:48:27.575400 pycax-client-1.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-22 22:48:10.000000 pycax-client-1.0.2/.github/workflows/deploy-docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-22 22:48:10.000000 pycax-client-1.0.2/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-22 22:48:10.000000 pycax-client-1.0.2/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-22 22:48:10.000000 pycax-client-1.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-04-22 22:48:10.000000 pycax-client-1.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-22 22:48:10.000000 pycax-client-1.0.2/CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-22 22:48:10.000000 pycax-client-1.0.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-22 22:48:10.000000 pycax-client-1.0.2/Changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-22 22:48:10.000000 pycax-client-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-22 22:48:10.000000 pycax-client-1.0.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-04-22 22:48:27.583400 pycax-client-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-04-22 22:48:10.000000 pycax-client-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-04-22 22:48:10.000000 pycax-client-1.0.2/RELEASING.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:48:27.579400 pycax-client-1.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7779 2023-04-22 22:48:10.000000 pycax-client-1.0.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-22 22:48:10.000000 pycax-client-1.0.2/docs/changelog_link.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9522 2023-04-22 22:48:10.000000 pycax-client-1.0.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-22 22:48:10.000000 pycax-client-1.0.2/docs/datasets.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:48:27.579400 pycax-client-1.0.2/docs/favicon_io/
--rw-r--r--   0 runner    (1001) docker     (123)    56389 2023-04-22 22:48:10.000000 pycax-client-1.0.2/docs/favicon_io/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (123)   345695 2023-04-22 22:48:10.000000 pycax-client-1.0.2/docs/favicon_io/android-chrome-512x512.png
--rw-r--r--   0 runner    (1001) docker     (123)    50361 2023-04-22 22:48:10.000000 pycax-client-1.0.2/docs/favicon_io/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-22 22:48:10.000000 pycax-client-1.0.2/docs/favicon_io/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-04-22 22:48:10.000000 pycax-client-1.0.2/docs/favicon_io/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-04-22 22:48:10.000000 pycax-client-1.0.2/docs/favicon_io/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-22 22:48:10.000000 pycax-client-1.0.2/docs/favicon_io/site.webmanifest
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-22 22:48:10.000000 pycax-client-1.0.2/docs/hli.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-04-22 22:48:10.000000 pycax-client-1.0.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7242 2023-04-22 22:48:10.000000 pycax-client-1.0.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)   534563 2023-04-22 22:48:10.000000 pycax-client-1.0.2/docs/pycaxlogo.png
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-22 22:48:10.000000 pycax-client-1.0.2/docs/tables.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:48:27.579400 pycax-client-1.0.2/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-22 22:48:10.000000 pycax-client-1.0.2/notebooks/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    24562 2023-04-22 22:48:10.000000 pycax-client-1.0.2/notebooks/usage_guide.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:48:27.579400 pycax-client-1.0.2/pycax/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-22 22:48:10.000000 pycax-client-1.0.2/pycax/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-22 22:48:10.000000 pycax-client-1.0.2/pycax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-22 22:48:27.000000 pycax-client-1.0.2/pycax/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-04-22 22:48:10.000000 pycax-client-1.0.2/pycax/caxutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:48:27.579400 pycax-client-1.0.2/pycax/data/
--rw-r--r--   0 runner    (1001) docker     (123)     7265 2023-04-22 22:48:10.000000 pycax-client-1.0.2/pycax/data/xport_colnames_json.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:48:27.579400 pycax-client-1.0.2/pycax/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-22 22:48:10.000000 pycax-client-1.0.2/pycax/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-22 22:48:10.000000 pycax-client-1.0.2/pycax/datasets/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-22 22:48:10.000000 pycax-client-1.0.2/pycax/datasets/test_datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:48:27.579400 pycax-client-1.0.2/pycax/hli/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-22 22:48:10.000000 pycax-client-1.0.2/pycax/hli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-04-22 22:48:10.000000 pycax-client-1.0.2/pycax/hli/hli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-04-22 22:48:10.000000 pycax-client-1.0.2/pycax/hli/test_hli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:48:27.579400 pycax-client-1.0.2/pycax/tables/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-22 22:48:10.000000 pycax-client-1.0.2/pycax/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-04-22 22:48:10.000000 pycax-client-1.0.2/pycax/tables/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-04-22 22:48:10.000000 pycax-client-1.0.2/pycax/tables/test_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:48:27.583400 pycax-client-1.0.2/pycax_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-04-22 22:48:27.000000 pycax-client-1.0.2/pycax_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-22 22:48:27.000000 pycax-client-1.0.2/pycax_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 22:48:27.000000 pycax-client-1.0.2/pycax_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-22 22:48:27.000000 pycax-client-1.0.2/pycax_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-22 22:48:27.000000 pycax-client-1.0.2/pycax_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-22 22:48:10.000000 pycax-client-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-22 22:48:10.000000 pycax-client-1.0.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-22 22:48:10.000000 pycax-client-1.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-22 22:48:27.583400 pycax-client-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-22 22:48:10.000000 pycax-client-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:32:03.658842 pycax-client-1.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:32:03.650841 pycax-client-1.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:32:03.650841 pycax-client-1.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-23 18:31:46.000000 pycax-client-1.0.3/.github/workflows/deploy-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-23 18:31:46.000000 pycax-client-1.0.3/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-23 18:31:46.000000 pycax-client-1.0.3/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-23 18:31:46.000000 pycax-client-1.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-04-23 18:31:46.000000 pycax-client-1.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-04-23 18:31:46.000000 pycax-client-1.0.3/CITATION
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-23 18:31:46.000000 pycax-client-1.0.3/CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-23 18:31:46.000000 pycax-client-1.0.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-23 18:31:46.000000 pycax-client-1.0.3/Changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-23 18:31:46.000000 pycax-client-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-23 18:31:46.000000 pycax-client-1.0.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-04-23 18:32:03.658842 pycax-client-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-04-23 18:31:46.000000 pycax-client-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-04-23 18:31:46.000000 pycax-client-1.0.3/RELEASING.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:32:03.654842 pycax-client-1.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7779 2023-04-23 18:31:46.000000 pycax-client-1.0.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-23 18:31:46.000000 pycax-client-1.0.3/docs/changelog_link.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9522 2023-04-23 18:31:46.000000 pycax-client-1.0.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-23 18:31:46.000000 pycax-client-1.0.3/docs/datasets.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:32:03.654842 pycax-client-1.0.3/docs/favicon_io/
+-rw-r--r--   0 runner    (1001) docker     (123)    56389 2023-04-23 18:31:46.000000 pycax-client-1.0.3/docs/favicon_io/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (123)   345695 2023-04-23 18:31:46.000000 pycax-client-1.0.3/docs/favicon_io/android-chrome-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (123)    50361 2023-04-23 18:31:46.000000 pycax-client-1.0.3/docs/favicon_io/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-23 18:31:46.000000 pycax-client-1.0.3/docs/favicon_io/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-04-23 18:31:46.000000 pycax-client-1.0.3/docs/favicon_io/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-04-23 18:31:46.000000 pycax-client-1.0.3/docs/favicon_io/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-23 18:31:46.000000 pycax-client-1.0.3/docs/favicon_io/site.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-23 18:31:46.000000 pycax-client-1.0.3/docs/hli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-04-23 18:31:46.000000 pycax-client-1.0.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7242 2023-04-23 18:31:46.000000 pycax-client-1.0.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)   534563 2023-04-23 18:31:46.000000 pycax-client-1.0.3/docs/pycaxlogo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-23 18:31:46.000000 pycax-client-1.0.3/docs/tables.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:32:03.654842 pycax-client-1.0.3/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-23 18:31:46.000000 pycax-client-1.0.3/notebooks/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    24562 2023-04-23 18:31:46.000000 pycax-client-1.0.3/notebooks/usage_guide.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:32:03.654842 pycax-client-1.0.3/pycax/
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-04-23 18:31:46.000000 pycax-client-1.0.3/pycax/CITATION
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-23 18:31:46.000000 pycax-client-1.0.3/pycax/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-23 18:31:46.000000 pycax-client-1.0.3/pycax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-23 18:32:03.000000 pycax-client-1.0.3/pycax/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-04-23 18:31:46.000000 pycax-client-1.0.3/pycax/caxutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:32:03.654842 pycax-client-1.0.3/pycax/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     7265 2023-04-23 18:31:46.000000 pycax-client-1.0.3/pycax/data/xport_colnames_json.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:32:03.654842 pycax-client-1.0.3/pycax/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-23 18:31:46.000000 pycax-client-1.0.3/pycax/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-23 18:31:46.000000 pycax-client-1.0.3/pycax/datasets/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-23 18:31:46.000000 pycax-client-1.0.3/pycax/datasets/test_datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:32:03.654842 pycax-client-1.0.3/pycax/hli/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-23 18:31:46.000000 pycax-client-1.0.3/pycax/hli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-04-23 18:31:46.000000 pycax-client-1.0.3/pycax/hli/hli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-04-23 18:31:46.000000 pycax-client-1.0.3/pycax/hli/test_hli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:32:03.654842 pycax-client-1.0.3/pycax/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-23 18:31:46.000000 pycax-client-1.0.3/pycax/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-04-23 18:31:46.000000 pycax-client-1.0.3/pycax/tables/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-04-23 18:31:46.000000 pycax-client-1.0.3/pycax/tables/test_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:32:03.658842 pycax-client-1.0.3/pycax_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-04-23 18:32:03.000000 pycax-client-1.0.3/pycax_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-23 18:32:03.000000 pycax-client-1.0.3/pycax_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 18:32:03.000000 pycax-client-1.0.3/pycax_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-23 18:32:03.000000 pycax-client-1.0.3/pycax_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-23 18:32:03.000000 pycax-client-1.0.3/pycax_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-23 18:31:46.000000 pycax-client-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-23 18:31:46.000000 pycax-client-1.0.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-23 18:31:46.000000 pycax-client-1.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-23 18:32:03.658842 pycax-client-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-23 18:31:46.000000 pycax-client-1.0.3/setup.py
```

### Comparing `pycax-client-1.0.2/.github/workflows/deploy-docs.yml` & `pycax-client-1.0.3/.github/workflows/deploy-docs.yml`

 * *Files identical despite different names*

### Comparing `pycax-client-1.0.2/.github/workflows/pypi.yml` & `pycax-client-1.0.3/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `pycax-client-1.0.2/.github/workflows/tests.yml` & `pycax-client-1.0.3/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `pycax-client-1.0.2/.pre-commit-config.yaml` & `pycax-client-1.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pycax-client-1.0.2/CONDUCT.md` & `pycax-client-1.0.3/CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pycax-client-1.0.2/CONTRIBUTING.md` & `pycax-client-1.0.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pycax-client-1.0.2/Changelog.rst` & `pycax-client-1.0.3/Changelog.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 Changelog
 =========
 
+1.0.3 (2023-04-23)
+------------------
+- MINOR:
+    - typo on Readme
+    - created badge for source code link
+    - use full url for logo so it works on PyPi.org page
+    - added CITATION file and DOI badge
+
 1.0.2 (2023-04-22)
 ------------------
 - MAJOR:
     - none. 
 - MINOR:
     - cleaned up the index page of documentation
     - fixed license file
     - added install from pip instructions
-- PATCH:
-     - NA
 
 1.0.0 (2023-04-21)
 ------------------
 - MAJOR:
     - none. first release for pypi yet
 - MINOR:
     - added a very simple usage Jupyter notebook
```

### Comparing `pycax-client-1.0.2/LICENSE` & `pycax-client-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pycax-client-1.0.2/PKG-INFO` & `pycax-client-1.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycax-client
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python client for CAX
 Home-page: https://github.com/nwfsc-math-bio/pycax
 Author: Eli Holmes and Mari Williams
 Author-email: eli.holmes@noaa.gov
 License: MIT
 Project-URL: Documentation, https://nwfsc-math-bio.github.io/pycax
 Project-URL: Bug Tracker, https://github.com/nwfsc-math-bio/pycax/issues
@@ -21,23 +21,25 @@
 License-File: LICENSE
 
 [![pypi](https://img.shields.io/pypi/v/pycax-client.svg)](https://pypi.python.org/pypi-client/pycax-client)
 [![github](https://img.shields.io/github/v/release/nwfsc-math-bio/pycax?color=brightgreen&label=GitHub)](https://github.com/nwfsc-math-bio/pycax/releases/latest)
 [![docs](https://github.com/nwfsc-math-bio/pycax/actions/workflows/deploy-docs.yml/badge.svg)](https://nwfsc-math-bio.github.io/pycax)
 [![tests](https://github.com/nwfsc-math-bio/pycax/actions/workflows/tests.yml/badge.svg)](https://github.com/nwfsc-math-bio/pycax/actions/workflows/tests.yml)
 [![coverage](https://nwfsc-math-bio.github.io/pycax/coverage.svg)](https://nwfsc-math-bio.github.io/pycax/_codecoverage/index.html)
+[![PyPi license](https://badgen.net/pypi/license/pycax-client/)](https://pypi.org/project/pycax-client/)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7855729.svg)](https://doi.org/10.5281/zenodo.7855729)
 
-pycx <img src="docs/pycaxlogo.png" align="right" width="20%"  hspace="20" vspace="20"/>
+pycax <img src="https://raw.githubusercontent.com/nwfsc-math-bio/pycax/main/docs/pycaxlogo.png" align="right" width="20%"  hspace="20" vspace="20"/>
 ========
 
 <!--
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/pycax-client.svg)](https://anaconda.org/conda-forge/pycax-client)
 -->
 
-pycax is an Python client for the [Coordinated Assessments API](https://www.streamnet.org/resources/exchange-tools/rest-api-documentation/). Make sure to review the [StreamNet Terms of Use](https://nwfsc-math-bio.github.io/rCAX/articles/terms.html) for these data, the [StreamNet Data Policy](https://www.streamnet.org/resources/exchange-tools/data-agreements/) and the [citation information](https://www.streamnet.org/resources/citing-sn/) for database queries. pycax was developed by the Northwest Fisheries Science Center Math Bio Program by Elizabeth Holmes and Mari Williams.
+pycax is a Python client for the Coordinated Assessments [REST API](https://www.streamnet.org/resources/exchange-tools/rest-api-documentation/). Make sure to review the [StreamNet Terms of Use](https://nwfsc-math-bio.github.io/rCAX/articles/terms.html) for these data, the [StreamNet Data Policy](https://www.streamnet.org/resources/exchange-tools/data-agreements/) and the [citation information](https://www.streamnet.org/resources/citing-sn/) for database queries. pycax was developed by the Northwest Fisheries Science Center Math Bio Program by Elizabeth Holmes and Mari Williams.
 
 NWFSC Math Bio CAX REST API clients:
 
 * Python client: [pycax on GitHub at nwfsc-math-bio/pycax](https://github.com/nwfsc-math-bio/pycax)
 * R client: [rCAX on GitHub at nwfsc-math-bio/rCAX](https://github.com/nwfsc-math-bio/rCAX)
 
 ## Installation
@@ -50,15 +52,14 @@
 
 From GitHub (development version)
 
 ```bash
 pip install git+git://github.com/nwfsc-math-bio/pycax.git#egg=pycax-client
 ```
 
-
 ## Documentation
 
 The official documentation is hosted on GitHub Pages [https://nwfsc-math-bio.github.io/pycax](https://nwfsc-math-bio.github.io/pycax).
 
 ## Library API
 
 `pycax` is split up into modules for each of the groups of API methods.
@@ -91,14 +92,22 @@
 # test and generate a coverage report
 python3 -m pytest -rxs --cov=pycax --cov-report term-missing ./pycax
 # make the documentation in docs/_build/html
 cd docs # pycax/docs
 make clean html codecov # linkcheck # linkcheck not working
 ```
 
+## Citation
+
+Holmes, E. E and M. Williams. 2023. pycax: a Python client for the Coordinated Assessments data exchange REST API. vX.X.X. doi:10.5281/zenodo.7855729.
+
+Make sure to include a citation for the Coordinated Assessments Partnership (CAP) data tables that you use. For details on citing CAP content see: https://www.streamnet.org/resources/citing-sn/
+
+See [CITATION](https://github.com/nwfsc-math-bio/pycax/blob/main/CITATION) file for bibtex version.
+
 ## Credits
 
 Thanks to the developers of [pyobis](https://github.com/iobis/pyobis) package who created a package that was easy to use as a full template for a REST API client with tests, documentation files, and GitHub Actions and included the instructions and requirements for local development. The structure of pycax mimics pyobis structure but was adapted and changed for the CAX API. The [pygbif](https://github.com/gbif/pygbif) package is similar (and seems to have influenced pyobis). pygbif source was used for reference and study though no code directly used. Some pygbif code may appear in pycax if pyobis used pygbif functions for reference. Notably the Sphinx documentation configuration files seem to originate from pygbif.
 
 <hr>
 
 ### Disclaimer
```

### Comparing `pycax-client-1.0.2/README.md` & `pycax-client-1.0.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 [![pypi](https://img.shields.io/pypi/v/pycax-client.svg)](https://pypi.python.org/pypi-client/pycax-client)
 [![github](https://img.shields.io/github/v/release/nwfsc-math-bio/pycax?color=brightgreen&label=GitHub)](https://github.com/nwfsc-math-bio/pycax/releases/latest)
 [![docs](https://github.com/nwfsc-math-bio/pycax/actions/workflows/deploy-docs.yml/badge.svg)](https://nwfsc-math-bio.github.io/pycax)
 [![tests](https://github.com/nwfsc-math-bio/pycax/actions/workflows/tests.yml/badge.svg)](https://github.com/nwfsc-math-bio/pycax/actions/workflows/tests.yml)
 [![coverage](https://nwfsc-math-bio.github.io/pycax/coverage.svg)](https://nwfsc-math-bio.github.io/pycax/_codecoverage/index.html)
+[![PyPi license](https://badgen.net/pypi/license/pycax-client/)](https://pypi.org/project/pycax-client/)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7855729.svg)](https://doi.org/10.5281/zenodo.7855729)
 
-pycx <img src="docs/pycaxlogo.png" align="right" width="20%"  hspace="20" vspace="20"/>
+pycax <img src="https://raw.githubusercontent.com/nwfsc-math-bio/pycax/main/docs/pycaxlogo.png" align="right" width="20%"  hspace="20" vspace="20"/>
 ========
 
 <!--
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/pycax-client.svg)](https://anaconda.org/conda-forge/pycax-client)
 -->
 
-pycax is an Python client for the [Coordinated Assessments API](https://www.streamnet.org/resources/exchange-tools/rest-api-documentation/). Make sure to review the [StreamNet Terms of Use](https://nwfsc-math-bio.github.io/rCAX/articles/terms.html) for these data, the [StreamNet Data Policy](https://www.streamnet.org/resources/exchange-tools/data-agreements/) and the [citation information](https://www.streamnet.org/resources/citing-sn/) for database queries. pycax was developed by the Northwest Fisheries Science Center Math Bio Program by Elizabeth Holmes and Mari Williams.
+pycax is a Python client for the Coordinated Assessments [REST API](https://www.streamnet.org/resources/exchange-tools/rest-api-documentation/). Make sure to review the [StreamNet Terms of Use](https://nwfsc-math-bio.github.io/rCAX/articles/terms.html) for these data, the [StreamNet Data Policy](https://www.streamnet.org/resources/exchange-tools/data-agreements/) and the [citation information](https://www.streamnet.org/resources/citing-sn/) for database queries. pycax was developed by the Northwest Fisheries Science Center Math Bio Program by Elizabeth Holmes and Mari Williams.
 
 NWFSC Math Bio CAX REST API clients:
 
 * Python client: [pycax on GitHub at nwfsc-math-bio/pycax](https://github.com/nwfsc-math-bio/pycax)
 * R client: [rCAX on GitHub at nwfsc-math-bio/rCAX](https://github.com/nwfsc-math-bio/rCAX)
 
 ## Installation
@@ -28,15 +30,14 @@
 
 From GitHub (development version)
 
 ```bash
 pip install git+git://github.com/nwfsc-math-bio/pycax.git#egg=pycax-client
 ```
 
-
 ## Documentation
 
 The official documentation is hosted on GitHub Pages [https://nwfsc-math-bio.github.io/pycax](https://nwfsc-math-bio.github.io/pycax).
 
 ## Library API
 
 `pycax` is split up into modules for each of the groups of API methods.
@@ -69,14 +70,22 @@
 # test and generate a coverage report
 python3 -m pytest -rxs --cov=pycax --cov-report term-missing ./pycax
 # make the documentation in docs/_build/html
 cd docs # pycax/docs
 make clean html codecov # linkcheck # linkcheck not working
 ```
 
+## Citation
+
+Holmes, E. E and M. Williams. 2023. pycax: a Python client for the Coordinated Assessments data exchange REST API. vX.X.X. doi:10.5281/zenodo.7855729.
+
+Make sure to include a citation for the Coordinated Assessments Partnership (CAP) data tables that you use. For details on citing CAP content see: https://www.streamnet.org/resources/citing-sn/
+
+See [CITATION](https://github.com/nwfsc-math-bio/pycax/blob/main/CITATION) file for bibtex version.
+
 ## Credits
 
 Thanks to the developers of [pyobis](https://github.com/iobis/pyobis) package who created a package that was easy to use as a full template for a REST API client with tests, documentation files, and GitHub Actions and included the instructions and requirements for local development. The structure of pycax mimics pyobis structure but was adapted and changed for the CAX API. The [pygbif](https://github.com/gbif/pygbif) package is similar (and seems to have influenced pyobis). pygbif source was used for reference and study though no code directly used. Some pygbif code may appear in pycax if pyobis used pygbif functions for reference. Notably the Sphinx documentation configuration files seem to originate from pygbif.
 
 <hr>
 
 ### Disclaimer
```

### Comparing `pycax-client-1.0.2/RELEASING.md` & `pycax-client-1.0.3/RELEASING.md`

 * *Files identical despite different names*

### Comparing `pycax-client-1.0.2/docs/Makefile` & `pycax-client-1.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pycax-client-1.0.2/docs/conf.py` & `pycax-client-1.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pycax-client-1.0.2/docs/favicon_io/android-chrome-192x192.png` & `pycax-client-1.0.3/docs/favicon_io/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `pycax-client-1.0.2/docs/favicon_io/android-chrome-512x512.png` & `pycax-client-1.0.3/docs/favicon_io/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `pycax-client-1.0.2/docs/favicon_io/apple-touch-icon.png` & `pycax-client-1.0.3/docs/favicon_io/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `pycax-client-1.0.2/docs/favicon_io/favicon-16x16.png` & `pycax-client-1.0.3/docs/favicon_io/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `pycax-client-1.0.2/docs/favicon_io/favicon-32x32.png` & `pycax-client-1.0.3/docs/favicon_io/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `pycax-client-1.0.2/docs/favicon_io/favicon.ico` & `pycax-client-1.0.3/docs/favicon_io/favicon.ico`

 * *Files identical despite different names*

### Comparing `pycax-client-1.0.2/docs/index.rst` & `pycax-client-1.0.3/docs/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 pycax |version|
 ===============
 
 .. |pypi| 
 
-|docs| |coverage|
+|docs| |coverage| |license| |source code| |DOI|
 
-`Source on GitHub at nwfsc-math-bio/pycax <https://github.com/nwfsc-math-bio/pycax>`__
-
-pycax is a Python client for the `Coordinated Assessments API <https://www.streamnet.org/resources/exchange-tools/rest-api-documentation/>`__. Coordinated Assessments data eXchange (CAX) is developed by the Coordinated Assessments Partnership (CAP). CAP is a collaborative process to efficiently share and provide access to standardized derived information, such as fish population-scale high-level indicators (HLIs) and supporting metrics. Participants in CAP include state fish and wildlife management agencies, tribes, federal agencies such as National Oceanic and Atmospheric Administration Fisheries (NOAA Fisheries) and Bonneville Power Administration (BPA), and others. CAP is co-sponsored by StreamNet and Pacific Northwest Aquatic Monitoring Partnership (PNAMP). Make sure to review the `StreamNet Terms of Use <https://nwfsc-math-bio.github.io/rCAX/articles/terms.html>`__ for these data, the `StreamNet Data Policy <https://www.streamnet.org/resources/exchange-tools/data-agreements/>`__ and the citation information from `StreamNet <https://www.streamnet.org/resources/citing-sn/>`__ and `PNAMP <https://www.pnamp.org/project/data-citation-and-attribution>`__ for database queries. pycax authors: Eli Holmes and Mari Williams, Northwest Fisheries Science Center, NOAA Fisheries.
+pycax is a Python client for the Coordinated Assessments data exchange `REST API <https://www.streamnet.org/resources/exchange-tools/rest-api-documentation/>`__. Coordinated Assessments data eXchange (CAX) is developed by the Coordinated Assessments Partnership (CAP). CAP is a collaborative process to efficiently share and provide access to standardized derived information, such as fish population-scale high-level indicators (HLIs) and supporting metrics. Participants in CAP include state fish and wildlife management agencies, tribes, federal agencies such as National Oceanic and Atmospheric Administration Fisheries (NOAA Fisheries) and Bonneville Power Administration (BPA), and others. CAP is co-sponsored by StreamNet and Pacific Northwest Aquatic Monitoring Partnership (PNAMP). Make sure to review the `StreamNet Terms of Use <https://nwfsc-math-bio.github.io/rCAX/articles/terms.html>`__ for these data, the `StreamNet Data Policy <https://www.streamnet.org/resources/exchange-tools/data-agreements/>`__ and the citation information from `StreamNet <https://www.streamnet.org/resources/citing-sn/>`__ and `PNAMP <https://www.pnamp.org/project/data-citation-and-attribution>`__ for database queries. pycax authors: Eli Holmes and Mari Williams, Northwest Fisheries Science Center, NOAA Fisheries.
 
 Other CAX clients: `rCAX` a R client, `nwfsc-math-bio/rCAX <https://nwfsc-math-bio.github.io/rCAX>`__
 
 Installation
 ============
 
 from pypi
@@ -86,14 +84,23 @@
    :target: https://pypi.python.org/pypi-client/pycax
 
 .. |docs| image:: https://github.com/nwfsc-math-bio/pycax/actions/workflows/deploy-docs.yml/badge.svg
    :target: https://nwfsc-math-bio.github.io/pycax
    
 .. |coverage| image:: https://nwfsc-math-bio.github.io/pycax/coverage.svg
    :target: https://nwfsc-math-bio.github.io/pycax/_codecoverage/index.html
+   
+.. |source code| image:: https://img.shields.io/badge/-Source%20code-61DAFB?logo=github&logoColor=white&style=flat
+   :target: https://github.com/nwfsc-math-bio/pycax
+   
+.. |license| image:: https://badgen.net/pypi/license/pycax-client/
+
+.. |DOI| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.7855729.svg
+   :target: https://doi.org/10.5281/zenodo.7855729
+
 
 
 
 Contents
 ========
 
 .. toctree::
```

### Comparing `pycax-client-1.0.2/docs/make.bat` & `pycax-client-1.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pycax-client-1.0.2/docs/pycaxlogo.png` & `pycax-client-1.0.3/docs/pycaxlogo.png`

 * *Files identical despite different names*

### Comparing `pycax-client-1.0.2/docs/tables.rst` & `pycax-client-1.0.3/docs/tables.rst`

 * *Files identical despite different names*

### Comparing `pycax-client-1.0.2/notebooks/usage_guide.ipynb` & `pycax-client-1.0.3/notebooks/usage_guide.ipynb`

 * *Files identical despite different names*

### Comparing `pycax-client-1.0.2/pycax/caxutils.py` & `pycax-client-1.0.3/pycax/caxutils.py`

 * *Files identical despite different names*

### Comparing `pycax-client-1.0.2/pycax/data/xport_colnames_json.txt` & `pycax-client-1.0.3/pycax/data/xport_colnames_json.txt`

 * *Files identical despite different names*

### Comparing `pycax-client-1.0.2/pycax/datasets/datasets.py` & `pycax-client-1.0.3/pycax/datasets/datasets.py`

 * *Files identical despite different names*

### Comparing `pycax-client-1.0.2/pycax/datasets/test_datasets.py` & `pycax-client-1.0.3/pycax/datasets/test_datasets.py`

 * *Files identical despite different names*

### Comparing `pycax-client-1.0.2/pycax/hli/hli.py` & `pycax-client-1.0.3/pycax/hli/hli.py`

 * *Files identical despite different names*

### Comparing `pycax-client-1.0.2/pycax/hli/test_hli.py` & `pycax-client-1.0.3/pycax/hli/test_hli.py`

 * *Files identical despite different names*

### Comparing `pycax-client-1.0.2/pycax/tables/tables.py` & `pycax-client-1.0.3/pycax/tables/tables.py`

 * *Files identical despite different names*

### Comparing `pycax-client-1.0.2/pycax/tables/test_tables.py` & `pycax-client-1.0.3/pycax/tables/test_tables.py`

 * *Files identical despite different names*

### Comparing `pycax-client-1.0.2/pycax_client.egg-info/PKG-INFO` & `pycax-client-1.0.3/pycax_client.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycax-client
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python client for CAX
 Home-page: https://github.com/nwfsc-math-bio/pycax
 Author: Eli Holmes and Mari Williams
 Author-email: eli.holmes@noaa.gov
 License: MIT
 Project-URL: Documentation, https://nwfsc-math-bio.github.io/pycax
 Project-URL: Bug Tracker, https://github.com/nwfsc-math-bio/pycax/issues
@@ -21,23 +21,25 @@
 License-File: LICENSE
 
 [![pypi](https://img.shields.io/pypi/v/pycax-client.svg)](https://pypi.python.org/pypi-client/pycax-client)
 [![github](https://img.shields.io/github/v/release/nwfsc-math-bio/pycax?color=brightgreen&label=GitHub)](https://github.com/nwfsc-math-bio/pycax/releases/latest)
 [![docs](https://github.com/nwfsc-math-bio/pycax/actions/workflows/deploy-docs.yml/badge.svg)](https://nwfsc-math-bio.github.io/pycax)
 [![tests](https://github.com/nwfsc-math-bio/pycax/actions/workflows/tests.yml/badge.svg)](https://github.com/nwfsc-math-bio/pycax/actions/workflows/tests.yml)
 [![coverage](https://nwfsc-math-bio.github.io/pycax/coverage.svg)](https://nwfsc-math-bio.github.io/pycax/_codecoverage/index.html)
+[![PyPi license](https://badgen.net/pypi/license/pycax-client/)](https://pypi.org/project/pycax-client/)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7855729.svg)](https://doi.org/10.5281/zenodo.7855729)
 
-pycx <img src="docs/pycaxlogo.png" align="right" width="20%"  hspace="20" vspace="20"/>
+pycax <img src="https://raw.githubusercontent.com/nwfsc-math-bio/pycax/main/docs/pycaxlogo.png" align="right" width="20%"  hspace="20" vspace="20"/>
 ========
 
 <!--
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/pycax-client.svg)](https://anaconda.org/conda-forge/pycax-client)
 -->
 
-pycax is an Python client for the [Coordinated Assessments API](https://www.streamnet.org/resources/exchange-tools/rest-api-documentation/). Make sure to review the [StreamNet Terms of Use](https://nwfsc-math-bio.github.io/rCAX/articles/terms.html) for these data, the [StreamNet Data Policy](https://www.streamnet.org/resources/exchange-tools/data-agreements/) and the [citation information](https://www.streamnet.org/resources/citing-sn/) for database queries. pycax was developed by the Northwest Fisheries Science Center Math Bio Program by Elizabeth Holmes and Mari Williams.
+pycax is a Python client for the Coordinated Assessments [REST API](https://www.streamnet.org/resources/exchange-tools/rest-api-documentation/). Make sure to review the [StreamNet Terms of Use](https://nwfsc-math-bio.github.io/rCAX/articles/terms.html) for these data, the [StreamNet Data Policy](https://www.streamnet.org/resources/exchange-tools/data-agreements/) and the [citation information](https://www.streamnet.org/resources/citing-sn/) for database queries. pycax was developed by the Northwest Fisheries Science Center Math Bio Program by Elizabeth Holmes and Mari Williams.
 
 NWFSC Math Bio CAX REST API clients:
 
 * Python client: [pycax on GitHub at nwfsc-math-bio/pycax](https://github.com/nwfsc-math-bio/pycax)
 * R client: [rCAX on GitHub at nwfsc-math-bio/rCAX](https://github.com/nwfsc-math-bio/rCAX)
 
 ## Installation
@@ -50,15 +52,14 @@
 
 From GitHub (development version)
 
 ```bash
 pip install git+git://github.com/nwfsc-math-bio/pycax.git#egg=pycax-client
 ```
 
-
 ## Documentation
 
 The official documentation is hosted on GitHub Pages [https://nwfsc-math-bio.github.io/pycax](https://nwfsc-math-bio.github.io/pycax).
 
 ## Library API
 
 `pycax` is split up into modules for each of the groups of API methods.
@@ -91,14 +92,22 @@
 # test and generate a coverage report
 python3 -m pytest -rxs --cov=pycax --cov-report term-missing ./pycax
 # make the documentation in docs/_build/html
 cd docs # pycax/docs
 make clean html codecov # linkcheck # linkcheck not working
 ```
 
+## Citation
+
+Holmes, E. E and M. Williams. 2023. pycax: a Python client for the Coordinated Assessments data exchange REST API. vX.X.X. doi:10.5281/zenodo.7855729.
+
+Make sure to include a citation for the Coordinated Assessments Partnership (CAP) data tables that you use. For details on citing CAP content see: https://www.streamnet.org/resources/citing-sn/
+
+See [CITATION](https://github.com/nwfsc-math-bio/pycax/blob/main/CITATION) file for bibtex version.
+
 ## Credits
 
 Thanks to the developers of [pyobis](https://github.com/iobis/pyobis) package who created a package that was easy to use as a full template for a REST API client with tests, documentation files, and GitHub Actions and included the instructions and requirements for local development. The structure of pycax mimics pyobis structure but was adapted and changed for the CAX API. The [pygbif](https://github.com/gbif/pygbif) package is similar (and seems to have influenced pyobis). pygbif source was used for reference and study though no code directly used. Some pygbif code may appear in pycax if pyobis used pygbif functions for reference. Notably the Sphinx documentation configuration files seem to originate from pygbif.
 
 <hr>
 
 ### Disclaimer
```

### Comparing `pycax-client-1.0.2/pycax_client.egg-info/SOURCES.txt` & `pycax-client-1.0.3/pycax_client.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 .gitignore
 .pre-commit-config.yaml
+CITATION
 CONDUCT.md
 CONTRIBUTING.md
 Changelog.rst
 LICENSE
 Makefile
 README.md
 RELEASING.md
@@ -29,14 +30,15 @@
 docs/favicon_io/apple-touch-icon.png
 docs/favicon_io/favicon-16x16.png
 docs/favicon_io/favicon-32x32.png
 docs/favicon_io/favicon.ico
 docs/favicon_io/site.webmanifest
 notebooks/README.md
 notebooks/usage_guide.ipynb
+pycax/CITATION
 pycax/MANIFEST.in
 pycax/__init__.py
 pycax/_version.py
 pycax/caxutils.py
 pycax/data/xport_colnames_json.txt
 pycax/datasets/__init__.py
 pycax/datasets/datasets.py
```

### Comparing `pycax-client-1.0.2/setup.cfg` & `pycax-client-1.0.3/setup.cfg`

 * *Files identical despite different names*

