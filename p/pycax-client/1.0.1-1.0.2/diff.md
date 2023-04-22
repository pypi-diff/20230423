# Comparing `tmp/pycax-client-1.0.1.tar.gz` & `tmp/pycax-client-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycax-client-1.0.1.tar", last modified: Fri Apr 21 18:11:49 2023, max compression
+gzip compressed data, was "pycax-client-1.0.2.tar", last modified: Sat Apr 22 22:48:27 2023, max compression
```

## Comparing `pycax-client-1.0.1.tar` & `pycax-client-1.0.2.tar`

### file list

```diff
@@ -1,66 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:11:49.548825 pycax-client-1.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:11:49.536825 pycax-client-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:11:49.540825 pycax-client-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-21 18:11:27.000000 pycax-client-1.0.1/.github/workflows/deploy-docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-21 18:11:27.000000 pycax-client-1.0.1/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-21 18:11:27.000000 pycax-client-1.0.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-21 18:11:27.000000 pycax-client-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-04-21 18:11:27.000000 pycax-client-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-21 18:11:27.000000 pycax-client-1.0.1/CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-21 18:11:27.000000 pycax-client-1.0.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-21 18:11:27.000000 pycax-client-1.0.1/Changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-04-21 18:11:27.000000 pycax-client-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-21 18:11:27.000000 pycax-client-1.0.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-04-21 18:11:49.548825 pycax-client-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-04-21 18:11:27.000000 pycax-client-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:11:49.540825 pycax-client-1.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7779 2023-04-21 18:11:27.000000 pycax-client-1.0.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-21 18:11:27.000000 pycax-client-1.0.1/docs/changelog_link.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9522 2023-04-21 18:11:27.000000 pycax-client-1.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-21 18:11:27.000000 pycax-client-1.0.1/docs/datasets.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:11:49.544825 pycax-client-1.0.1/docs/favicon_io/
--rw-r--r--   0 runner    (1001) docker     (123)    56389 2023-04-21 18:11:27.000000 pycax-client-1.0.1/docs/favicon_io/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (123)   345695 2023-04-21 18:11:27.000000 pycax-client-1.0.1/docs/favicon_io/android-chrome-512x512.png
--rw-r--r--   0 runner    (1001) docker     (123)    50361 2023-04-21 18:11:27.000000 pycax-client-1.0.1/docs/favicon_io/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-21 18:11:27.000000 pycax-client-1.0.1/docs/favicon_io/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-04-21 18:11:27.000000 pycax-client-1.0.1/docs/favicon_io/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-04-21 18:11:27.000000 pycax-client-1.0.1/docs/favicon_io/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-21 18:11:27.000000 pycax-client-1.0.1/docs/favicon_io/site.webmanifest
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-21 18:11:27.000000 pycax-client-1.0.1/docs/hli.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-04-21 18:11:27.000000 pycax-client-1.0.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7242 2023-04-21 18:11:27.000000 pycax-client-1.0.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)   534563 2023-04-21 18:11:27.000000 pycax-client-1.0.1/docs/pycaxlogo.png
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-21 18:11:27.000000 pycax-client-1.0.1/docs/tables.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:11:49.544825 pycax-client-1.0.1/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-21 18:11:27.000000 pycax-client-1.0.1/notebooks/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    26167 2023-04-21 18:11:27.000000 pycax-client-1.0.1/notebooks/usage_guide.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:11:49.544825 pycax-client-1.0.1/pycax/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-21 18:11:27.000000 pycax-client-1.0.1/pycax/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-21 18:11:27.000000 pycax-client-1.0.1/pycax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-21 18:11:49.000000 pycax-client-1.0.1/pycax/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-04-21 18:11:27.000000 pycax-client-1.0.1/pycax/caxutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:11:49.544825 pycax-client-1.0.1/pycax/data/
--rw-r--r--   0 runner    (1001) docker     (123)     7265 2023-04-21 18:11:27.000000 pycax-client-1.0.1/pycax/data/xport_colnames_json.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:11:49.544825 pycax-client-1.0.1/pycax/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-21 18:11:27.000000 pycax-client-1.0.1/pycax/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-21 18:11:27.000000 pycax-client-1.0.1/pycax/datasets/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-21 18:11:27.000000 pycax-client-1.0.1/pycax/datasets/test_datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:11:49.544825 pycax-client-1.0.1/pycax/hli/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-21 18:11:27.000000 pycax-client-1.0.1/pycax/hli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-04-21 18:11:27.000000 pycax-client-1.0.1/pycax/hli/hli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-04-21 18:11:27.000000 pycax-client-1.0.1/pycax/hli/test_hli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:11:49.544825 pycax-client-1.0.1/pycax/tables/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-21 18:11:27.000000 pycax-client-1.0.1/pycax/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-04-21 18:11:27.000000 pycax-client-1.0.1/pycax/tables/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-04-21 18:11:27.000000 pycax-client-1.0.1/pycax/tables/test_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:11:49.544825 pycax-client-1.0.1/pycax_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-04-21 18:11:49.000000 pycax-client-1.0.1/pycax_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-21 18:11:49.000000 pycax-client-1.0.1/pycax_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 18:11:49.000000 pycax-client-1.0.1/pycax_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-21 18:11:49.000000 pycax-client-1.0.1/pycax_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-21 18:11:49.000000 pycax-client-1.0.1/pycax_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-21 18:11:27.000000 pycax-client-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-21 18:11:27.000000 pycax-client-1.0.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-21 18:11:27.000000 pycax-client-1.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-21 18:11:49.548825 pycax-client-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-21 18:11:27.000000 pycax-client-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:48:27.583400 pycax-client-1.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:48:27.575400 pycax-client-1.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:48:27.575400 pycax-client-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-22 22:48:10.000000 pycax-client-1.0.2/.github/workflows/deploy-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-22 22:48:10.000000 pycax-client-1.0.2/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-22 22:48:10.000000 pycax-client-1.0.2/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-22 22:48:10.000000 pycax-client-1.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-04-22 22:48:10.000000 pycax-client-1.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-22 22:48:10.000000 pycax-client-1.0.2/CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-22 22:48:10.000000 pycax-client-1.0.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-22 22:48:10.000000 pycax-client-1.0.2/Changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-22 22:48:10.000000 pycax-client-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-22 22:48:10.000000 pycax-client-1.0.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-04-22 22:48:27.583400 pycax-client-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-04-22 22:48:10.000000 pycax-client-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-04-22 22:48:10.000000 pycax-client-1.0.2/RELEASING.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:48:27.579400 pycax-client-1.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7779 2023-04-22 22:48:10.000000 pycax-client-1.0.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-22 22:48:10.000000 pycax-client-1.0.2/docs/changelog_link.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9522 2023-04-22 22:48:10.000000 pycax-client-1.0.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-22 22:48:10.000000 pycax-client-1.0.2/docs/datasets.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:48:27.579400 pycax-client-1.0.2/docs/favicon_io/
+-rw-r--r--   0 runner    (1001) docker     (123)    56389 2023-04-22 22:48:10.000000 pycax-client-1.0.2/docs/favicon_io/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (123)   345695 2023-04-22 22:48:10.000000 pycax-client-1.0.2/docs/favicon_io/android-chrome-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (123)    50361 2023-04-22 22:48:10.000000 pycax-client-1.0.2/docs/favicon_io/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-22 22:48:10.000000 pycax-client-1.0.2/docs/favicon_io/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-04-22 22:48:10.000000 pycax-client-1.0.2/docs/favicon_io/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-04-22 22:48:10.000000 pycax-client-1.0.2/docs/favicon_io/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-22 22:48:10.000000 pycax-client-1.0.2/docs/favicon_io/site.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-22 22:48:10.000000 pycax-client-1.0.2/docs/hli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-04-22 22:48:10.000000 pycax-client-1.0.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7242 2023-04-22 22:48:10.000000 pycax-client-1.0.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)   534563 2023-04-22 22:48:10.000000 pycax-client-1.0.2/docs/pycaxlogo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-22 22:48:10.000000 pycax-client-1.0.2/docs/tables.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:48:27.579400 pycax-client-1.0.2/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-22 22:48:10.000000 pycax-client-1.0.2/notebooks/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    24562 2023-04-22 22:48:10.000000 pycax-client-1.0.2/notebooks/usage_guide.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:48:27.579400 pycax-client-1.0.2/pycax/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-22 22:48:10.000000 pycax-client-1.0.2/pycax/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-22 22:48:10.000000 pycax-client-1.0.2/pycax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-22 22:48:27.000000 pycax-client-1.0.2/pycax/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-04-22 22:48:10.000000 pycax-client-1.0.2/pycax/caxutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:48:27.579400 pycax-client-1.0.2/pycax/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     7265 2023-04-22 22:48:10.000000 pycax-client-1.0.2/pycax/data/xport_colnames_json.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:48:27.579400 pycax-client-1.0.2/pycax/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-22 22:48:10.000000 pycax-client-1.0.2/pycax/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-22 22:48:10.000000 pycax-client-1.0.2/pycax/datasets/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-22 22:48:10.000000 pycax-client-1.0.2/pycax/datasets/test_datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:48:27.579400 pycax-client-1.0.2/pycax/hli/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-22 22:48:10.000000 pycax-client-1.0.2/pycax/hli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-04-22 22:48:10.000000 pycax-client-1.0.2/pycax/hli/hli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-04-22 22:48:10.000000 pycax-client-1.0.2/pycax/hli/test_hli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:48:27.579400 pycax-client-1.0.2/pycax/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-22 22:48:10.000000 pycax-client-1.0.2/pycax/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-04-22 22:48:10.000000 pycax-client-1.0.2/pycax/tables/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-04-22 22:48:10.000000 pycax-client-1.0.2/pycax/tables/test_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:48:27.583400 pycax-client-1.0.2/pycax_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-04-22 22:48:27.000000 pycax-client-1.0.2/pycax_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-22 22:48:27.000000 pycax-client-1.0.2/pycax_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 22:48:27.000000 pycax-client-1.0.2/pycax_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-22 22:48:27.000000 pycax-client-1.0.2/pycax_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-22 22:48:27.000000 pycax-client-1.0.2/pycax_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-22 22:48:10.000000 pycax-client-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-22 22:48:10.000000 pycax-client-1.0.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-22 22:48:10.000000 pycax-client-1.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-22 22:48:27.583400 pycax-client-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-22 22:48:10.000000 pycax-client-1.0.2/setup.py
```

### Comparing `pycax-client-1.0.1/.github/workflows/deploy-docs.yml` & `pycax-client-1.0.2/.github/workflows/deploy-docs.yml`

 * *Files identical despite different names*

### Comparing `pycax-client-1.0.1/.github/workflows/pypi.yml` & `pycax-client-1.0.2/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `pycax-client-1.0.1/.github/workflows/tests.yml` & `pycax-client-1.0.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `pycax-client-1.0.1/.pre-commit-config.yaml` & `pycax-client-1.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pycax-client-1.0.1/CONDUCT.md` & `pycax-client-1.0.2/CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pycax-client-1.0.1/CONTRIBUTING.md` & `pycax-client-1.0.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pycax-client-1.0.1/PKG-INFO` & `pycax-client-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycax-client
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python client for CAX
 Home-page: https://github.com/nwfsc-math-bio/pycax
 Author: Eli Holmes and Mari Williams
 Author-email: eli.holmes@noaa.gov
 License: MIT
 Project-URL: Documentation, https://nwfsc-math-bio.github.io/pycax
 Project-URL: Bug Tracker, https://github.com/nwfsc-math-bio/pycax/issues
@@ -16,46 +16,43 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![pypi](https://img.shields.io/pypi/v/pycax-client.svg)](https://pypi.python.org/pypi-client/pycax-client)
 [![github](https://img.shields.io/github/v/release/nwfsc-math-bio/pycax?color=brightgreen&label=GitHub)](https://github.com/nwfsc-math-bio/pycax/releases/latest)
 [![docs](https://github.com/nwfsc-math-bio/pycax/actions/workflows/deploy-docs.yml/badge.svg)](https://nwfsc-math-bio.github.io/pycax)
 [![tests](https://github.com/nwfsc-math-bio/pycax/actions/workflows/tests.yml/badge.svg)](https://github.com/nwfsc-math-bio/pycax/actions/workflows/tests.yml)
 [![coverage](https://nwfsc-math-bio.github.io/pycax/coverage.svg)](https://nwfsc-math-bio.github.io/pycax/_codecoverage/index.html)
 
 pycx <img src="docs/pycaxlogo.png" align="right" width="20%"  hspace="20" vspace="20"/>
 ========
 
-
 <!--
-[![pypi](https://img.shields.io/pypi/v/pycax-client.svg)](https://pypi.python.org/pypi-client/pycax-client)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/pycax-client.svg)](https://anaconda.org/conda-forge/pycax-client)
 -->
 
-pycax is an Python client for the [Coordinated Assessments API](https://www.streamnet.org/resources/exchange-tools/rest-api-documentation/). Make sure to review the [StreamNet Terms of Use](https://nwfsc-math-bio.github.io/rCAX/articles/terms.html) for these data, the [StreamNet Data Policy](https://www.streamnet.org/resources/exchange-tools/data-agreements/) and the [citation information](https://www.streamnet.org/resources/citing-sn/) for database queries. pycax was developed by the Northwest Fisheries Science Center Math Bio Program.
+pycax is an Python client for the [Coordinated Assessments API](https://www.streamnet.org/resources/exchange-tools/rest-api-documentation/). Make sure to review the [StreamNet Terms of Use](https://nwfsc-math-bio.github.io/rCAX/articles/terms.html) for these data, the [StreamNet Data Policy](https://www.streamnet.org/resources/exchange-tools/data-agreements/) and the [citation information](https://www.streamnet.org/resources/citing-sn/) for database queries. pycax was developed by the Northwest Fisheries Science Center Math Bio Program by Elizabeth Holmes and Mari Williams.
 
 NWFSC Math Bio CAX REST API clients:
 
 * Python client: [pycax on GitHub at nwfsc-math-bio/pycax](https://github.com/nwfsc-math-bio/pycax)
 * R client: [rCAX on GitHub at nwfsc-math-bio/rCAX](https://github.com/nwfsc-math-bio/rCAX)
 
 ## Installation
 
-<!--
 From pypi
 
 ```bash
 pip install pycax-client
 ```
--->
 
-Development version
+From GitHub (development version)
 
 ```bash
 pip install git+git://github.com/nwfsc-math-bio/pycax.git#egg=pycax-client
 ```
 
 
 ## Documentation
@@ -91,25 +88,25 @@
 python3 -m pip install -e .
 # test your installation
 python3 -m pytest
 # test and generate a coverage report
 python3 -m pytest -rxs --cov=pycax --cov-report term-missing ./pycax
 # make the documentation in docs/_build/html
 cd docs # pycax/docs
-make clean html codecov linkcheck
+make clean html codecov # linkcheck # linkcheck not working
 ```
 
 ## Credits
 
 Thanks to the developers of [pyobis](https://github.com/iobis/pyobis) package who created a package that was easy to use as a full template for a REST API client with tests, documentation files, and GitHub Actions and included the instructions and requirements for local development. The structure of pycax mimics pyobis structure but was adapted and changed for the CAX API. The [pygbif](https://github.com/gbif/pygbif) package is similar (and seems to have influenced pyobis). pygbif source was used for reference and study though no code directly used. Some pygbif code may appear in pycax if pyobis used pygbif functions for reference. Notably the Sphinx documentation configuration files seem to originate from pygbif.
 
 <hr>
 
 ### Disclaimer
 
 This repository is a scientific product and is not official communication of the National Oceanic and Atmospheric Administration, or the United States Department of Commerce. All NOAA GitHub project content is provided on an ‘as is’ basis and the user assumes responsibility for its use. Any claims against the Department of Commerce or Department of Commerce bureaus stemming from the use of this GitHub project will be governed by all applicable Federal law. Any reference to specific commercial products, processes, or services by service mark, trademark, manufacturer, or otherwise, does not constitute or imply their endorsement, recommendation or favoring by the Department of Commerce. The Department of Commerce seal and logo, or the seal and logo of a DOC bureau, shall not be used in any manner to imply endorsement of any commercial product or activity by DOC or the United States Government.
 
 ### License
 
-This content was created by U.S. Government employees as part of their official duties. This content is not subject to copyright in the United States (17 U.S.C. §105) and is in the public domain within the United States of America. Additionally, copyright is waived worldwide through the CC0 1.0 Universal public domain dedication.
+This content was created by U.S. Government employees as part of their official duties. This content is not subject to copyright in the United States (17 U.S.C. §105) and is in the public domain within the United States of America. Additionally, copyright is waived worldwide through the MIT License.
```

### Comparing `pycax-client-1.0.1/README.md` & `pycax-client-1.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,36 @@
+[![pypi](https://img.shields.io/pypi/v/pycax-client.svg)](https://pypi.python.org/pypi-client/pycax-client)
 [![github](https://img.shields.io/github/v/release/nwfsc-math-bio/pycax?color=brightgreen&label=GitHub)](https://github.com/nwfsc-math-bio/pycax/releases/latest)
 [![docs](https://github.com/nwfsc-math-bio/pycax/actions/workflows/deploy-docs.yml/badge.svg)](https://nwfsc-math-bio.github.io/pycax)
 [![tests](https://github.com/nwfsc-math-bio/pycax/actions/workflows/tests.yml/badge.svg)](https://github.com/nwfsc-math-bio/pycax/actions/workflows/tests.yml)
 [![coverage](https://nwfsc-math-bio.github.io/pycax/coverage.svg)](https://nwfsc-math-bio.github.io/pycax/_codecoverage/index.html)
 
 pycx <img src="docs/pycaxlogo.png" align="right" width="20%"  hspace="20" vspace="20"/>
 ========
 
-
 <!--
-[![pypi](https://img.shields.io/pypi/v/pycax-client.svg)](https://pypi.python.org/pypi-client/pycax-client)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/pycax-client.svg)](https://anaconda.org/conda-forge/pycax-client)
 -->
 
-pycax is an Python client for the [Coordinated Assessments API](https://www.streamnet.org/resources/exchange-tools/rest-api-documentation/). Make sure to review the [StreamNet Terms of Use](https://nwfsc-math-bio.github.io/rCAX/articles/terms.html) for these data, the [StreamNet Data Policy](https://www.streamnet.org/resources/exchange-tools/data-agreements/) and the [citation information](https://www.streamnet.org/resources/citing-sn/) for database queries. pycax was developed by the Northwest Fisheries Science Center Math Bio Program.
+pycax is an Python client for the [Coordinated Assessments API](https://www.streamnet.org/resources/exchange-tools/rest-api-documentation/). Make sure to review the [StreamNet Terms of Use](https://nwfsc-math-bio.github.io/rCAX/articles/terms.html) for these data, the [StreamNet Data Policy](https://www.streamnet.org/resources/exchange-tools/data-agreements/) and the [citation information](https://www.streamnet.org/resources/citing-sn/) for database queries. pycax was developed by the Northwest Fisheries Science Center Math Bio Program by Elizabeth Holmes and Mari Williams.
 
 NWFSC Math Bio CAX REST API clients:
 
 * Python client: [pycax on GitHub at nwfsc-math-bio/pycax](https://github.com/nwfsc-math-bio/pycax)
 * R client: [rCAX on GitHub at nwfsc-math-bio/rCAX](https://github.com/nwfsc-math-bio/rCAX)
 
 ## Installation
 
-<!--
 From pypi
 
 ```bash
 pip install pycax-client
 ```
--->
 
-Development version
+From GitHub (development version)
 
 ```bash
 pip install git+git://github.com/nwfsc-math-bio/pycax.git#egg=pycax-client
 ```
 
 
 ## Documentation
@@ -69,25 +66,25 @@
 python3 -m pip install -e .
 # test your installation
 python3 -m pytest
 # test and generate a coverage report
 python3 -m pytest -rxs --cov=pycax --cov-report term-missing ./pycax
 # make the documentation in docs/_build/html
 cd docs # pycax/docs
-make clean html codecov linkcheck
+make clean html codecov # linkcheck # linkcheck not working
 ```
 
 ## Credits
 
 Thanks to the developers of [pyobis](https://github.com/iobis/pyobis) package who created a package that was easy to use as a full template for a REST API client with tests, documentation files, and GitHub Actions and included the instructions and requirements for local development. The structure of pycax mimics pyobis structure but was adapted and changed for the CAX API. The [pygbif](https://github.com/gbif/pygbif) package is similar (and seems to have influenced pyobis). pygbif source was used for reference and study though no code directly used. Some pygbif code may appear in pycax if pyobis used pygbif functions for reference. Notably the Sphinx documentation configuration files seem to originate from pygbif.
 
 <hr>
 
 ### Disclaimer
 
 This repository is a scientific product and is not official communication of the National Oceanic and Atmospheric Administration, or the United States Department of Commerce. All NOAA GitHub project content is provided on an ‘as is’ basis and the user assumes responsibility for its use. Any claims against the Department of Commerce or Department of Commerce bureaus stemming from the use of this GitHub project will be governed by all applicable Federal law. Any reference to specific commercial products, processes, or services by service mark, trademark, manufacturer, or otherwise, does not constitute or imply their endorsement, recommendation or favoring by the Department of Commerce. The Department of Commerce seal and logo, or the seal and logo of a DOC bureau, shall not be used in any manner to imply endorsement of any commercial product or activity by DOC or the United States Government.
 
 ### License
 
-This content was created by U.S. Government employees as part of their official duties. This content is not subject to copyright in the United States (17 U.S.C. §105) and is in the public domain within the United States of America. Additionally, copyright is waived worldwide through the CC0 1.0 Universal public domain dedication.
+This content was created by U.S. Government employees as part of their official duties. This content is not subject to copyright in the United States (17 U.S.C. §105) and is in the public domain within the United States of America. Additionally, copyright is waived worldwide through the MIT License.
```

### Comparing `pycax-client-1.0.1/docs/Makefile` & `pycax-client-1.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pycax-client-1.0.1/docs/conf.py` & `pycax-client-1.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pycax-client-1.0.1/docs/favicon_io/android-chrome-192x192.png` & `pycax-client-1.0.2/docs/favicon_io/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `pycax-client-1.0.1/docs/favicon_io/android-chrome-512x512.png` & `pycax-client-1.0.2/docs/favicon_io/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `pycax-client-1.0.1/docs/favicon_io/apple-touch-icon.png` & `pycax-client-1.0.2/docs/favicon_io/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `pycax-client-1.0.1/docs/favicon_io/favicon-16x16.png` & `pycax-client-1.0.2/docs/favicon_io/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `pycax-client-1.0.1/docs/favicon_io/favicon-32x32.png` & `pycax-client-1.0.2/docs/favicon_io/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `pycax-client-1.0.1/docs/favicon_io/favicon.ico` & `pycax-client-1.0.2/docs/favicon_io/favicon.ico`

 * *Files identical despite different names*

### Comparing `pycax-client-1.0.1/docs/make.bat` & `pycax-client-1.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pycax-client-1.0.1/docs/pycaxlogo.png` & `pycax-client-1.0.2/docs/pycaxlogo.png`

 * *Files identical despite different names*

### Comparing `pycax-client-1.0.1/docs/tables.rst` & `pycax-client-1.0.2/docs/tables.rst`

 * *Files identical despite different names*

### Comparing `pycax-client-1.0.1/pycax/__init__.py` & `pycax-client-1.0.2/pycax/__init__.py`

 * *Files identical despite different names*

### Comparing `pycax-client-1.0.1/pycax/caxutils.py` & `pycax-client-1.0.2/pycax/caxutils.py`

 * *Files identical despite different names*

### Comparing `pycax-client-1.0.1/pycax/data/xport_colnames_json.txt` & `pycax-client-1.0.2/pycax/data/xport_colnames_json.txt`

 * *Files identical despite different names*

### Comparing `pycax-client-1.0.1/pycax/datasets/datasets.py` & `pycax-client-1.0.2/pycax/datasets/datasets.py`

 * *Files identical despite different names*

### Comparing `pycax-client-1.0.1/pycax/datasets/test_datasets.py` & `pycax-client-1.0.2/pycax/datasets/test_datasets.py`

 * *Files identical despite different names*

### Comparing `pycax-client-1.0.1/pycax/hli/hli.py` & `pycax-client-1.0.2/pycax/hli/hli.py`

 * *Files identical despite different names*

### Comparing `pycax-client-1.0.1/pycax/hli/test_hli.py` & `pycax-client-1.0.2/pycax/hli/test_hli.py`

 * *Files identical despite different names*

### Comparing `pycax-client-1.0.1/pycax/tables/tables.py` & `pycax-client-1.0.2/pycax/tables/tables.py`

 * *Files identical despite different names*

### Comparing `pycax-client-1.0.1/pycax/tables/test_tables.py` & `pycax-client-1.0.2/pycax/tables/test_tables.py`

 * *Files identical despite different names*

### Comparing `pycax-client-1.0.1/pycax_client.egg-info/PKG-INFO` & `pycax-client-1.0.2/pycax_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycax-client
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python client for CAX
 Home-page: https://github.com/nwfsc-math-bio/pycax
 Author: Eli Holmes and Mari Williams
 Author-email: eli.holmes@noaa.gov
 License: MIT
 Project-URL: Documentation, https://nwfsc-math-bio.github.io/pycax
 Project-URL: Bug Tracker, https://github.com/nwfsc-math-bio/pycax/issues
@@ -16,46 +16,43 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![pypi](https://img.shields.io/pypi/v/pycax-client.svg)](https://pypi.python.org/pypi-client/pycax-client)
 [![github](https://img.shields.io/github/v/release/nwfsc-math-bio/pycax?color=brightgreen&label=GitHub)](https://github.com/nwfsc-math-bio/pycax/releases/latest)
 [![docs](https://github.com/nwfsc-math-bio/pycax/actions/workflows/deploy-docs.yml/badge.svg)](https://nwfsc-math-bio.github.io/pycax)
 [![tests](https://github.com/nwfsc-math-bio/pycax/actions/workflows/tests.yml/badge.svg)](https://github.com/nwfsc-math-bio/pycax/actions/workflows/tests.yml)
 [![coverage](https://nwfsc-math-bio.github.io/pycax/coverage.svg)](https://nwfsc-math-bio.github.io/pycax/_codecoverage/index.html)
 
 pycx <img src="docs/pycaxlogo.png" align="right" width="20%"  hspace="20" vspace="20"/>
 ========
 
-
 <!--
-[![pypi](https://img.shields.io/pypi/v/pycax-client.svg)](https://pypi.python.org/pypi-client/pycax-client)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/pycax-client.svg)](https://anaconda.org/conda-forge/pycax-client)
 -->
 
-pycax is an Python client for the [Coordinated Assessments API](https://www.streamnet.org/resources/exchange-tools/rest-api-documentation/). Make sure to review the [StreamNet Terms of Use](https://nwfsc-math-bio.github.io/rCAX/articles/terms.html) for these data, the [StreamNet Data Policy](https://www.streamnet.org/resources/exchange-tools/data-agreements/) and the [citation information](https://www.streamnet.org/resources/citing-sn/) for database queries. pycax was developed by the Northwest Fisheries Science Center Math Bio Program.
+pycax is an Python client for the [Coordinated Assessments API](https://www.streamnet.org/resources/exchange-tools/rest-api-documentation/). Make sure to review the [StreamNet Terms of Use](https://nwfsc-math-bio.github.io/rCAX/articles/terms.html) for these data, the [StreamNet Data Policy](https://www.streamnet.org/resources/exchange-tools/data-agreements/) and the [citation information](https://www.streamnet.org/resources/citing-sn/) for database queries. pycax was developed by the Northwest Fisheries Science Center Math Bio Program by Elizabeth Holmes and Mari Williams.
 
 NWFSC Math Bio CAX REST API clients:
 
 * Python client: [pycax on GitHub at nwfsc-math-bio/pycax](https://github.com/nwfsc-math-bio/pycax)
 * R client: [rCAX on GitHub at nwfsc-math-bio/rCAX](https://github.com/nwfsc-math-bio/rCAX)
 
 ## Installation
 
-<!--
 From pypi
 
 ```bash
 pip install pycax-client
 ```
--->
 
-Development version
+From GitHub (development version)
 
 ```bash
 pip install git+git://github.com/nwfsc-math-bio/pycax.git#egg=pycax-client
 ```
 
 
 ## Documentation
@@ -91,25 +88,25 @@
 python3 -m pip install -e .
 # test your installation
 python3 -m pytest
 # test and generate a coverage report
 python3 -m pytest -rxs --cov=pycax --cov-report term-missing ./pycax
 # make the documentation in docs/_build/html
 cd docs # pycax/docs
-make clean html codecov linkcheck
+make clean html codecov # linkcheck # linkcheck not working
 ```
 
 ## Credits
 
 Thanks to the developers of [pyobis](https://github.com/iobis/pyobis) package who created a package that was easy to use as a full template for a REST API client with tests, documentation files, and GitHub Actions and included the instructions and requirements for local development. The structure of pycax mimics pyobis structure but was adapted and changed for the CAX API. The [pygbif](https://github.com/gbif/pygbif) package is similar (and seems to have influenced pyobis). pygbif source was used for reference and study though no code directly used. Some pygbif code may appear in pycax if pyobis used pygbif functions for reference. Notably the Sphinx documentation configuration files seem to originate from pygbif.
 
 <hr>
 
 ### Disclaimer
 
 This repository is a scientific product and is not official communication of the National Oceanic and Atmospheric Administration, or the United States Department of Commerce. All NOAA GitHub project content is provided on an ‘as is’ basis and the user assumes responsibility for its use. Any claims against the Department of Commerce or Department of Commerce bureaus stemming from the use of this GitHub project will be governed by all applicable Federal law. Any reference to specific commercial products, processes, or services by service mark, trademark, manufacturer, or otherwise, does not constitute or imply their endorsement, recommendation or favoring by the Department of Commerce. The Department of Commerce seal and logo, or the seal and logo of a DOC bureau, shall not be used in any manner to imply endorsement of any commercial product or activity by DOC or the United States Government.
 
 ### License
 
-This content was created by U.S. Government employees as part of their official duties. This content is not subject to copyright in the United States (17 U.S.C. §105) and is in the public domain within the United States of America. Additionally, copyright is waived worldwide through the CC0 1.0 Universal public domain dedication.
+This content was created by U.S. Government employees as part of their official duties. This content is not subject to copyright in the United States (17 U.S.C. §105) and is in the public domain within the United States of America. Additionally, copyright is waived worldwide through the MIT License.
```

### Comparing `pycax-client-1.0.1/pycax_client.egg-info/SOURCES.txt` & `pycax-client-1.0.2/pycax_client.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 .pre-commit-config.yaml
 CONDUCT.md
 CONTRIBUTING.md
 Changelog.rst
 LICENSE
 Makefile
 README.md
+RELEASING.md
 pyproject.toml
 requirements-dev.txt
 requirements.txt
 setup.cfg
 setup.py
 .github/workflows/deploy-docs.yml
 .github/workflows/pypi.yml
```

### Comparing `pycax-client-1.0.1/setup.cfg` & `pycax-client-1.0.2/setup.cfg`

 * *Files identical despite different names*

