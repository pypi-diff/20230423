# Comparing `tmp/dlrepo-0.5.tar.gz` & `tmp/dlrepo-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlrepo-0.5.tar", last modified: Thu Jan  6 11:04:43 2022, max compression
+gzip compressed data, was "dlrepo-0.8.tar", last modified: Tue Jan 18 08:09:46 2022, max compression
```

## Comparing `dlrepo-0.5.tar` & `dlrepo-0.8.tar`

### file list

```diff
@@ -1,93 +1,110 @@
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-01-06 11:04:43.278651 dlrepo-0.5/
--rw-r--r--   0 robin     (1000) robin     (1000)     1558 2021-12-17 14:03:58.000000 dlrepo-0.5/LICENSE
--rw-r--r--   0 robin     (1000) robin     (1000)      305 2022-01-05 15:03:36.000000 dlrepo-0.5/MANIFEST.in
--rw-r--r--   0 robin     (1000) robin     (1000)     3380 2022-01-05 13:12:54.000000 dlrepo-0.5/Makefile
--rw-r--r--   0 robin     (1000) robin     (1000)     4552 2022-01-06 11:04:43.278651 dlrepo-0.5/PKG-INFO
--rw-r--r--   0 robin     (1000) robin     (1000)     3507 2022-01-05 14:13:57.000000 dlrepo-0.5/README.md
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-01-06 11:04:43.274651 dlrepo-0.5/dlrepo/
--rw-r--r--   0 robin     (1000) robin     (1000)        0 2022-01-04 22:31:27.000000 dlrepo-0.5/dlrepo/__init__.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2983 2022-01-05 13:12:54.000000 dlrepo-0.5/dlrepo/__main__.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3737 2022-01-05 13:12:54.000000 dlrepo-0.5/dlrepo/cleanup.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-01-06 11:04:43.274651 dlrepo-0.5/dlrepo/fs/
--rw-r--r--   0 robin     (1000) robin     (1000)    12078 2022-01-05 09:06:37.000000 dlrepo-0.5/dlrepo/fs/__init__.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2619 2022-01-04 22:31:27.000000 dlrepo-0.5/dlrepo/fs/branch.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4825 2022-01-04 22:31:27.000000 dlrepo-0.5/dlrepo/fs/container.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4608 2022-01-04 22:31:27.000000 dlrepo-0.5/dlrepo/fs/fmt.py
--rw-r--r--   0 robin     (1000) robin     (1000)     5267 2022-01-04 22:31:27.000000 dlrepo-0.5/dlrepo/fs/job.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3632 2022-01-06 11:01:02.000000 dlrepo-0.5/dlrepo/fs/product.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6558 2022-01-06 10:59:33.000000 dlrepo-0.5/dlrepo/fs/tag.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2800 2022-01-04 22:31:27.000000 dlrepo-0.5/dlrepo/fs/util.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-01-06 11:04:43.274651 dlrepo-0.5/dlrepo/static/
--rw-r--r--   0 robin     (1000) robin     (1000)     1088 2022-01-04 22:31:27.000000 dlrepo-0.5/dlrepo/static/favicon.svg
--rw-r--r--   0 robin     (1000) robin     (1000)     1627 2022-01-04 22:31:27.000000 dlrepo-0.5/dlrepo/static/locked.svg
--rw-r--r--   0 robin     (1000) robin     (1000)     2150 2022-01-04 22:31:27.000000 dlrepo-0.5/dlrepo/static/logo.svg
--rw-r--r--   0 robin     (1000) robin     (1000)     1661 2022-01-04 22:31:27.000000 dlrepo-0.5/dlrepo/static/released.svg
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-01-06 11:04:43.274651 dlrepo-0.5/dlrepo/templates/
--rw-r--r--   0 robin     (1000) robin     (1000)      992 2022-01-04 22:31:27.000000 dlrepo-0.5/dlrepo/templates/autoindex.html
--rw-r--r--   0 robin     (1000) robin     (1000)     1460 2022-01-05 16:02:46.000000 dlrepo-0.5/dlrepo/templates/base.html
--rw-r--r--   0 robin     (1000) robin     (1000)     1066 2022-01-06 10:29:17.000000 dlrepo-0.5/dlrepo/templates/branch.html
--rw-r--r--   0 robin     (1000) robin     (1000)      595 2022-01-06 09:32:38.000000 dlrepo-0.5/dlrepo/templates/branches.html
--rw-r--r--   0 robin     (1000) robin     (1000)     1852 2022-01-06 09:54:04.000000 dlrepo-0.5/dlrepo/templates/home.html
--rw-r--r--   0 robin     (1000) robin     (1000)     1973 2022-01-04 22:31:27.000000 dlrepo-0.5/dlrepo/templates/job.html
--rw-r--r--   0 robin     (1000) robin     (1000)      649 2022-01-06 09:32:38.000000 dlrepo-0.5/dlrepo/templates/product.html
--rw-r--r--   0 robin     (1000) robin     (1000)     1206 2022-01-06 09:32:38.000000 dlrepo-0.5/dlrepo/templates/product_branch.html
--rw-r--r--   0 robin     (1000) robin     (1000)      722 2022-01-06 09:32:38.000000 dlrepo-0.5/dlrepo/templates/product_variant.html
--rw-r--r--   0 robin     (1000) robin     (1000)     1283 2022-01-04 22:31:27.000000 dlrepo-0.5/dlrepo/templates/product_version.html
--rw-r--r--   0 robin     (1000) robin     (1000)      694 2022-01-06 09:54:04.000000 dlrepo-0.5/dlrepo/templates/products.html
--rw-r--r--   0 robin     (1000) robin     (1000)      599 2022-01-06 09:32:38.000000 dlrepo-0.5/dlrepo/templates/tag.html
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-01-06 11:04:43.278651 dlrepo-0.5/dlrepo/views/
--rw-r--r--   0 robin     (1000) robin     (1000)     6994 2022-01-06 11:00:59.000000 dlrepo-0.5/dlrepo/views/__init__.py
--rw-r--r--   0 robin     (1000) robin     (1000)     5630 2022-01-04 22:31:27.000000 dlrepo-0.5/dlrepo/views/artifact.py
--rw-r--r--   0 robin     (1000) robin     (1000)    13473 2022-01-05 09:06:48.000000 dlrepo-0.5/dlrepo/views/auth.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4210 2022-01-06 10:41:37.000000 dlrepo-0.5/dlrepo/views/branch.py
--rw-r--r--   0 robin     (1000) robin     (1000)    10464 2022-01-04 22:31:27.000000 dlrepo-0.5/dlrepo/views/container.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3041 2022-01-05 09:06:49.000000 dlrepo-0.5/dlrepo/views/errors.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6124 2022-01-04 22:31:27.000000 dlrepo-0.5/dlrepo/views/fmt.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4029 2022-01-04 22:31:27.000000 dlrepo-0.5/dlrepo/views/job.py
--rw-r--r--   0 robin     (1000) robin     (1000)     8079 2022-01-06 10:41:37.000000 dlrepo-0.5/dlrepo/views/product.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3094 2022-01-04 22:31:27.000000 dlrepo-0.5/dlrepo/views/tag.py
--rw-r--r--   0 robin     (1000) robin     (1000)     5123 2022-01-05 10:22:52.000000 dlrepo-0.5/dlrepo/views/util.py
--rwxr-xr-x   0 robin     (1000) robin     (1000)    25511 2021-12-18 20:41:18.000000 dlrepo-0.5/dlrepo-cli
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-01-06 11:04:43.274651 dlrepo-0.5/dlrepo.egg-info/
--rw-r--r--   0 robin     (1000) robin     (1000)     4552 2022-01-06 11:04:43.000000 dlrepo-0.5/dlrepo.egg-info/PKG-INFO
--rw-r--r--   0 robin     (1000) robin     (1000)     1786 2022-01-06 11:04:43.000000 dlrepo-0.5/dlrepo.egg-info/SOURCES.txt
--rw-r--r--   0 robin     (1000) robin     (1000)        1 2022-01-06 11:04:43.000000 dlrepo-0.5/dlrepo.egg-info/dependency_links.txt
--rw-r--r--   0 robin     (1000) robin     (1000)      102 2022-01-06 11:04:43.000000 dlrepo-0.5/dlrepo.egg-info/entry_points.txt
--rw-r--r--   0 robin     (1000) robin     (1000)        1 2021-12-19 09:26:12.000000 dlrepo-0.5/dlrepo.egg-info/not-zip-safe
--rw-r--r--   0 robin     (1000) robin     (1000)       41 2022-01-06 11:04:43.000000 dlrepo-0.5/dlrepo.egg-info/requires.txt
--rw-r--r--   0 robin     (1000) robin     (1000)        7 2022-01-06 11:04:43.000000 dlrepo-0.5/dlrepo.egg-info/top_level.txt
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-01-06 11:04:43.278651 dlrepo-0.5/docs/
--rw-r--r--   0 robin     (1000) robin     (1000)     3327 2022-01-05 14:09:31.000000 dlrepo-0.5/docs/dlrepo-acls.5.scdoc
--rw-r--r--   0 robin     (1000) robin     (1000)    20253 2022-01-06 08:11:12.000000 dlrepo-0.5/docs/dlrepo-api.7.scdoc
--rw-r--r--   0 robin     (1000) robin     (1000)     1717 2022-01-05 14:09:31.000000 dlrepo-0.5/docs/dlrepo-cleanup.8.scdoc
--rw-r--r--   0 robin     (1000) robin     (1000)     5666 2022-01-05 14:09:31.000000 dlrepo-0.5/docs/dlrepo-cli.1.scdoc
--rw-r--r--   0 robin     (1000) robin     (1000)     6746 2022-01-06 08:11:18.000000 dlrepo-0.5/docs/dlrepo-config.5.scdoc
--rw-r--r--   0 robin     (1000) robin     (1000)     6517 2022-01-05 14:09:31.000000 dlrepo-0.5/docs/dlrepo-layout.7.scdoc
--rw-r--r--   0 robin     (1000) robin     (1000)     1726 2022-01-05 14:09:31.000000 dlrepo-0.5/docs/dlrepo.7.scdoc
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-01-06 11:04:43.278651 dlrepo-0.5/etc/
--rw-r--r--   0 robin     (1000) robin     (1000)      660 2022-01-06 08:11:41.000000 dlrepo-0.5/etc/default
--rw-r--r--   0 robin     (1000) robin     (1000)      488 2022-01-04 22:31:27.000000 dlrepo-0.5/etc/dlrepo-cleanup.service
--rw-r--r--   0 robin     (1000) robin     (1000)      146 2022-01-04 22:31:27.000000 dlrepo-0.5/etc/dlrepo-cleanup.timer
--rw-r--r--   0 robin     (1000) robin     (1000)      655 2022-01-04 22:31:27.000000 dlrepo-0.5/etc/dlrepo.service
--rw-r--r--   0 robin     (1000) robin     (1000)      200 2022-01-04 22:31:27.000000 dlrepo-0.5/etc/dlrepo.socket
--rw-r--r--   0 robin     (1000) robin     (1000)      628 2022-01-04 22:31:27.000000 dlrepo-0.5/etc/nginx.conf
--rw-r--r--   0 robin     (1000) robin     (1000)     1132 2021-12-29 22:04:39.000000 dlrepo-0.5/pylintrc
--rw-r--r--   0 robin     (1000) robin     (1000)       83 2022-01-04 22:31:28.000000 dlrepo-0.5/requirements-dev.txt
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-01-06 11:04:43.278651 dlrepo-0.5/scss/
--rw-r--r--   0 robin     (1000) robin     (1000)     1391 2022-01-06 09:54:04.000000 dlrepo-0.5/scss/components.scss
--rw-r--r--   0 robin     (1000) robin     (1000)     1872 2022-01-05 10:26:56.000000 dlrepo-0.5/scss/layout.scss
--rw-r--r--   0 robin     (1000) robin     (1000)      225 2022-01-04 22:31:27.000000 dlrepo-0.5/scss/main.scss
--rw-r--r--   0 robin     (1000) robin     (1000)     2876 2022-01-04 22:31:27.000000 dlrepo-0.5/scss/normalize.scss
--rw-r--r--   0 robin     (1000) robin     (1000)     2579 2022-01-06 09:54:04.000000 dlrepo-0.5/scss/sections.scss
--rw-r--r--   0 robin     (1000) robin     (1000)      574 2022-01-04 22:31:27.000000 dlrepo-0.5/scss/variables.scss
--rw-r--r--   0 robin     (1000) robin     (1000)      381 2022-01-06 11:04:43.278651 dlrepo-0.5/setup.cfg
--rw-r--r--   0 robin     (1000) robin     (1000)     1410 2022-01-06 11:03:54.000000 dlrepo-0.5/setup.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-01-06 11:04:43.278651 dlrepo-0.5/tests/
--rw-r--r--   0 robin     (1000) robin     (1000)     1957 2022-01-05 13:12:54.000000 dlrepo-0.5/tests/conftest.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-01-06 11:04:43.278651 dlrepo-0.5/tests/test_auth/
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-01-06 11:04:43.278651 dlrepo-0.5/tests/test_auth/acls/
--rw-r--r--   0 robin     (1000) robin     (1000)        7 2022-01-04 22:31:28.000000 dlrepo-0.5/tests/test_auth/acls/group1
--rw-r--r--   0 robin     (1000) robin     (1000)       23 2022-01-04 22:31:28.000000 dlrepo-0.5/tests/test_auth/acls/group2
--rw-r--r--   0 robin     (1000) robin     (1000)       92 2022-01-04 22:31:28.000000 dlrepo-0.5/tests/test_auth/acls/group3
--rw-r--r--   0 robin     (1000) robin     (1000)       47 2022-01-04 22:31:28.000000 dlrepo-0.5/tests/test_auth/auth
--rw-r--r--   0 robin     (1000) robin     (1000)     3085 2022-01-05 08:08:34.000000 dlrepo-0.5/tests/test_auth.py
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-01-18 08:09:46.826271 dlrepo-0.8/
+-rw-r--r--   0 robin     (1000) robin     (1000)     1558 2021-12-17 14:03:58.000000 dlrepo-0.8/LICENSE
+-rw-r--r--   0 robin     (1000) robin     (1000)      305 2022-01-05 15:03:36.000000 dlrepo-0.8/MANIFEST.in
+-rw-r--r--   0 robin     (1000) robin     (1000)     3380 2022-01-05 13:12:54.000000 dlrepo-0.8/Makefile
+-rw-r--r--   0 robin     (1000) robin     (1000)     4552 2022-01-18 08:09:46.826271 dlrepo-0.8/PKG-INFO
+-rw-r--r--   0 robin     (1000) robin     (1000)     3507 2022-01-05 14:13:57.000000 dlrepo-0.8/README.md
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-01-18 08:09:46.822271 dlrepo-0.8/dlrepo/
+-rw-r--r--   0 robin     (1000) robin     (1000)        0 2022-01-04 22:31:27.000000 dlrepo-0.8/dlrepo/__init__.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     2983 2022-01-05 13:12:54.000000 dlrepo-0.8/dlrepo/__main__.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3737 2022-01-05 13:12:54.000000 dlrepo-0.8/dlrepo/cleanup.py
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-01-18 08:09:46.822271 dlrepo-0.8/dlrepo/fs/
+-rw-r--r--   0 robin     (1000) robin     (1000)    11697 2022-01-11 14:08:09.000000 dlrepo-0.8/dlrepo/fs/__init__.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     2619 2022-01-04 22:31:27.000000 dlrepo-0.8/dlrepo/fs/branch.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     4825 2022-01-04 22:31:27.000000 dlrepo-0.8/dlrepo/fs/container.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     6729 2022-01-12 09:53:51.000000 dlrepo-0.8/dlrepo/fs/fmt.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     5267 2022-01-04 22:31:27.000000 dlrepo-0.8/dlrepo/fs/job.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3632 2022-01-06 11:01:02.000000 dlrepo-0.8/dlrepo/fs/product.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     6558 2022-01-06 10:59:33.000000 dlrepo-0.8/dlrepo/fs/tag.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3284 2022-01-11 14:08:09.000000 dlrepo-0.8/dlrepo/fs/util.py
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-01-18 08:09:46.822271 dlrepo-0.8/dlrepo/static/
+-rw-r--r--   0 robin     (1000) robin     (1000)     1088 2022-01-04 22:31:27.000000 dlrepo-0.8/dlrepo/static/favicon.svg
+-rw-r--r--   0 robin     (1000) robin     (1000)     1627 2022-01-04 22:31:27.000000 dlrepo-0.8/dlrepo/static/locked.svg
+-rw-r--r--   0 robin     (1000) robin     (1000)     2150 2022-01-04 22:31:27.000000 dlrepo-0.8/dlrepo/static/logo.svg
+-rw-r--r--   0 robin     (1000) robin     (1000)     1661 2022-01-04 22:31:27.000000 dlrepo-0.8/dlrepo/static/released.svg
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-01-18 08:09:46.822271 dlrepo-0.8/dlrepo/templates/
+-rw-r--r--   0 robin     (1000) robin     (1000)     1083 2022-01-12 10:44:58.000000 dlrepo-0.8/dlrepo/templates/autoindex.html
+-rw-r--r--   0 robin     (1000) robin     (1000)     1460 2022-01-05 16:02:46.000000 dlrepo-0.8/dlrepo/templates/base.html
+-rw-r--r--   0 robin     (1000) robin     (1000)     1066 2022-01-06 10:29:17.000000 dlrepo-0.8/dlrepo/templates/branch.html
+-rw-r--r--   0 robin     (1000) robin     (1000)      595 2022-01-06 09:32:38.000000 dlrepo-0.8/dlrepo/templates/branches.html
+-rw-r--r--   0 robin     (1000) robin     (1000)     1852 2022-01-06 09:54:04.000000 dlrepo-0.8/dlrepo/templates/home.html
+-rw-r--r--   0 robin     (1000) robin     (1000)     2088 2022-01-12 10:44:58.000000 dlrepo-0.8/dlrepo/templates/job.html
+-rw-r--r--   0 robin     (1000) robin     (1000)      649 2022-01-06 09:32:38.000000 dlrepo-0.8/dlrepo/templates/product.html
+-rw-r--r--   0 robin     (1000) robin     (1000)     1206 2022-01-06 09:32:38.000000 dlrepo-0.8/dlrepo/templates/product_branch.html
+-rw-r--r--   0 robin     (1000) robin     (1000)      722 2022-01-06 09:32:38.000000 dlrepo-0.8/dlrepo/templates/product_variant.html
+-rw-r--r--   0 robin     (1000) robin     (1000)     1398 2022-01-12 10:44:58.000000 dlrepo-0.8/dlrepo/templates/product_version.html
+-rw-r--r--   0 robin     (1000) robin     (1000)      694 2022-01-06 09:54:04.000000 dlrepo-0.8/dlrepo/templates/products.html
+-rw-r--r--   0 robin     (1000) robin     (1000)      599 2022-01-06 09:32:38.000000 dlrepo-0.8/dlrepo/templates/tag.html
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-01-18 08:09:46.822271 dlrepo-0.8/dlrepo/views/
+-rw-r--r--   0 robin     (1000) robin     (1000)     7040 2022-01-12 10:44:58.000000 dlrepo-0.8/dlrepo/views/__init__.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     6191 2022-01-17 09:20:23.000000 dlrepo-0.8/dlrepo/views/artifact.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    13473 2022-01-05 09:06:48.000000 dlrepo-0.8/dlrepo/views/auth.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     4210 2022-01-06 10:41:37.000000 dlrepo-0.8/dlrepo/views/branch.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    10470 2022-01-11 14:07:54.000000 dlrepo-0.8/dlrepo/views/container.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3041 2022-01-05 09:06:49.000000 dlrepo-0.8/dlrepo/views/errors.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     7295 2022-01-12 10:44:58.000000 dlrepo-0.8/dlrepo/views/fmt.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     4107 2022-01-12 10:44:58.000000 dlrepo-0.8/dlrepo/views/job.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     8179 2022-01-12 10:44:58.000000 dlrepo-0.8/dlrepo/views/product.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3094 2022-01-04 22:31:27.000000 dlrepo-0.8/dlrepo/views/tag.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     6201 2022-01-12 10:44:58.000000 dlrepo-0.8/dlrepo/views/util.py
+-rwxr-xr-x   0 robin     (1000) robin     (1000)    25511 2021-12-18 20:41:18.000000 dlrepo-0.8/dlrepo-cli
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-01-18 08:09:46.822271 dlrepo-0.8/dlrepo.egg-info/
+-rw-r--r--   0 robin     (1000) robin     (1000)     4552 2022-01-18 08:09:46.000000 dlrepo-0.8/dlrepo.egg-info/PKG-INFO
+-rw-r--r--   0 robin     (1000) robin     (1000)     2176 2022-01-18 08:09:46.000000 dlrepo-0.8/dlrepo.egg-info/SOURCES.txt
+-rw-r--r--   0 robin     (1000) robin     (1000)        1 2022-01-18 08:09:46.000000 dlrepo-0.8/dlrepo.egg-info/dependency_links.txt
+-rw-r--r--   0 robin     (1000) robin     (1000)      102 2022-01-18 08:09:46.000000 dlrepo-0.8/dlrepo.egg-info/entry_points.txt
+-rw-r--r--   0 robin     (1000) robin     (1000)        1 2021-12-19 09:26:12.000000 dlrepo-0.8/dlrepo.egg-info/not-zip-safe
+-rw-r--r--   0 robin     (1000) robin     (1000)       41 2022-01-18 08:09:46.000000 dlrepo-0.8/dlrepo.egg-info/requires.txt
+-rw-r--r--   0 robin     (1000) robin     (1000)        7 2022-01-18 08:09:46.000000 dlrepo-0.8/dlrepo.egg-info/top_level.txt
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-01-18 08:09:46.822271 dlrepo-0.8/docs/
+-rw-r--r--   0 robin     (1000) robin     (1000)     3327 2022-01-05 14:09:31.000000 dlrepo-0.8/docs/dlrepo-acls.5.scdoc
+-rw-r--r--   0 robin     (1000) robin     (1000)    22288 2022-01-12 10:44:58.000000 dlrepo-0.8/docs/dlrepo-api.7.scdoc
+-rw-r--r--   0 robin     (1000) robin     (1000)     1717 2022-01-05 14:09:31.000000 dlrepo-0.8/docs/dlrepo-cleanup.8.scdoc
+-rw-r--r--   0 robin     (1000) robin     (1000)     5666 2022-01-05 14:09:31.000000 dlrepo-0.8/docs/dlrepo-cli.1.scdoc
+-rw-r--r--   0 robin     (1000) robin     (1000)     7599 2022-01-11 14:08:09.000000 dlrepo-0.8/docs/dlrepo-config.5.scdoc
+-rw-r--r--   0 robin     (1000) robin     (1000)     6967 2022-01-11 14:08:09.000000 dlrepo-0.8/docs/dlrepo-layout.7.scdoc
+-rw-r--r--   0 robin     (1000) robin     (1000)     1726 2022-01-05 14:09:31.000000 dlrepo-0.8/docs/dlrepo.7.scdoc
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-01-18 08:09:46.822271 dlrepo-0.8/etc/
+-rw-r--r--   0 robin     (1000) robin     (1000)      686 2022-01-11 14:08:09.000000 dlrepo-0.8/etc/default
+-rw-r--r--   0 robin     (1000) robin     (1000)      488 2022-01-04 22:31:27.000000 dlrepo-0.8/etc/dlrepo-cleanup.service
+-rw-r--r--   0 robin     (1000) robin     (1000)      146 2022-01-04 22:31:27.000000 dlrepo-0.8/etc/dlrepo-cleanup.timer
+-rw-r--r--   0 robin     (1000) robin     (1000)      655 2022-01-04 22:31:27.000000 dlrepo-0.8/etc/dlrepo.service
+-rw-r--r--   0 robin     (1000) robin     (1000)      200 2022-01-04 22:31:27.000000 dlrepo-0.8/etc/dlrepo.socket
+-rw-r--r--   0 robin     (1000) robin     (1000)      628 2022-01-04 22:31:27.000000 dlrepo-0.8/etc/nginx.conf
+-rwxr-xr-x   0 robin     (1000) robin     (1000)     1230 2022-01-17 17:25:24.000000 dlrepo-0.8/etc/post-process.sh
+-rw-r--r--   0 robin     (1000) robin     (1000)     1132 2021-12-29 22:04:39.000000 dlrepo-0.8/pylintrc
+-rw-r--r--   0 robin     (1000) robin     (1000)       83 2022-01-04 22:31:28.000000 dlrepo-0.8/requirements-dev.txt
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-01-18 08:09:46.826271 dlrepo-0.8/scss/
+-rw-r--r--   0 robin     (1000) robin     (1000)     1395 2022-01-18 08:07:30.000000 dlrepo-0.8/scss/components.scss
+-rw-r--r--   0 robin     (1000) robin     (1000)     1872 2022-01-05 10:26:56.000000 dlrepo-0.8/scss/layout.scss
+-rw-r--r--   0 robin     (1000) robin     (1000)      225 2022-01-04 22:31:27.000000 dlrepo-0.8/scss/main.scss
+-rw-r--r--   0 robin     (1000) robin     (1000)     2876 2022-01-04 22:31:27.000000 dlrepo-0.8/scss/normalize.scss
+-rw-r--r--   0 robin     (1000) robin     (1000)     2711 2022-01-12 10:44:58.000000 dlrepo-0.8/scss/sections.scss
+-rw-r--r--   0 robin     (1000) robin     (1000)      574 2022-01-18 08:02:10.000000 dlrepo-0.8/scss/variables.scss
+-rw-r--r--   0 robin     (1000) robin     (1000)      381 2022-01-18 08:09:46.826271 dlrepo-0.8/setup.cfg
+-rw-r--r--   0 robin     (1000) robin     (1000)     1410 2022-01-18 08:08:28.000000 dlrepo-0.8/setup.py
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-01-18 08:09:46.826271 dlrepo-0.8/tests/
+-rw-r--r--   0 robin     (1000) robin     (1000)     2234 2022-01-11 14:21:33.000000 dlrepo-0.8/tests/conftest.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     1795 2022-01-12 10:44:58.000000 dlrepo-0.8/tests/test_archive.py
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-01-18 08:09:46.826271 dlrepo-0.8/tests/test_auth/
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-01-18 08:09:46.826271 dlrepo-0.8/tests/test_auth/acls/
+-rw-r--r--   0 robin     (1000) robin     (1000)        7 2022-01-04 22:31:28.000000 dlrepo-0.8/tests/test_auth/acls/group1
+-rw-r--r--   0 robin     (1000) robin     (1000)       23 2022-01-04 22:31:28.000000 dlrepo-0.8/tests/test_auth/acls/group2
+-rw-r--r--   0 robin     (1000) robin     (1000)       92 2022-01-04 22:31:28.000000 dlrepo-0.8/tests/test_auth/acls/group3
+-rw-r--r--   0 robin     (1000) robin     (1000)       47 2022-01-04 22:31:28.000000 dlrepo-0.8/tests/test_auth/auth
+-rw-r--r--   0 robin     (1000) robin     (1000)     3303 2022-01-11 14:18:30.000000 dlrepo-0.8/tests/test_auth.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     1879 2022-01-12 10:44:58.000000 dlrepo-0.8/tests/test_digests.py
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-01-18 08:09:46.826271 dlrepo-0.8/tests/test_post_process/
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-01-18 08:09:46.818271 dlrepo-0.8/tests/test_post_process/branches/
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-01-18 08:09:46.818271 dlrepo-0.8/tests/test_post_process/branches/branch/
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-01-18 08:09:46.818271 dlrepo-0.8/tests/test_post_process/branches/branch/tag/
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-01-18 08:09:46.818271 dlrepo-0.8/tests/test_post_process/branches/branch/tag/job/
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-01-18 08:09:46.826271 dlrepo-0.8/tests/test_post_process/branches/branch/tag/job/fmt/
+-rw-r--r--   0 robin     (1000) robin     (1000)        4 2022-01-11 14:29:05.000000 dlrepo-0.8/tests/test_post_process/branches/branch/tag/job/fmt/file.txt
+-rw-r--r--   0 robin     (1000) robin     (1000)        4 2022-01-11 14:29:10.000000 dlrepo-0.8/tests/test_post_process/branches/branch/tag/job/fmt/file2.txt
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-01-18 08:09:46.826271 dlrepo-0.8/tests/test_post_process/branches/branch/tag/job/fmt-error/
+-rw-r--r--   0 robin     (1000) robin     (1000)        7 2022-01-11 14:50:20.000000 dlrepo-0.8/tests/test_post_process/branches/branch/tag/job/fmt-error/file3.txt
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-01-18 08:09:46.826271 dlrepo-0.8/tests/test_post_process/branches/branch/tag/job/fmt-ignored/
+-rw-r--r--   0 robin     (1000) robin     (1000)        7 2022-01-11 14:50:01.000000 dlrepo-0.8/tests/test_post_process/branches/branch/tag/job/fmt-ignored/foo.txt
+-rwxr-xr-x   0 robin     (1000) robin     (1000)      162 2022-01-11 15:13:43.000000 dlrepo-0.8/tests/test_post_process/post-process.sh
+-rw-r--r--   0 robin     (1000) robin     (1000)     2328 2022-01-11 15:23:27.000000 dlrepo-0.8/tests/test_post_process.py
```

### Comparing `dlrepo-0.5/LICENSE` & `dlrepo-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dlrepo-0.5/Makefile` & `dlrepo-0.8/Makefile`

 * *Files identical despite different names*

### Comparing `dlrepo-0.5/PKG-INFO` & `dlrepo-0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlrepo
-Version: 0.5
+Version: 0.8
 Summary: Artifact repository
 Home-page: https://sr.ht/~rjarry/dlrepo/
 Author: Robin Jarry
 Author-email: robin@jarry.cc
 License: BSD-3-Clause
 Description: # dlrepo
```

### Comparing `dlrepo-0.5/README.md` & `dlrepo-0.8/README.md`

 * *Files identical despite different names*

### Comparing `dlrepo-0.5/dlrepo/__main__.py` & `dlrepo-0.8/dlrepo/__main__.py`

 * *Files identical despite different names*

### Comparing `dlrepo-0.5/dlrepo/cleanup.py` & `dlrepo-0.8/dlrepo/cleanup.py`

 * *Files identical despite different names*

### Comparing `dlrepo-0.5/dlrepo/fs/__init__.py` & `dlrepo-0.8/dlrepo/fs/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 # Copyright (c) 2021 Julien Floret
 # Copyright (c) 2021 Robin Jarry
 # SPDX-License-Identifier: BSD-3-Clause
 
-import hashlib
+import asyncio
 import logging
 import os
 from pathlib import Path
 import shutil
 import time
 from typing import Awaitable, Callable, Iterator, Optional
 
 from cachetools import LFUCache
 
 from .branch import Branch
 from .container import ContainerRegistry
 from .product import Product
-from .util import human_readable, parse_digest
+from .util import CHUNK_SIZE, file_digest, human_readable, parse_digest
 
 
 LOG = logging.getLogger(__name__)
-CHUNK_SIZE = int(os.getenv("DLREPO_CHUNK_SIZE", str(256 * 1024)))
 
 
 # --------------------------------------------------------------------------------------
 class AbstractRepository:
     def __init__(self, path: str):
         self._path = Path(path)
         self.parent = None
@@ -66,15 +65,15 @@
         self, uuid: str, stream: Callable[[int], Awaitable[bytes]]
     ) -> int:
         raise NotImplementedError()
 
     def cancel_upload(self, uuid: str):
         raise NotImplementedError()
 
-    def finalize_upload(self, uuid: str, digest: str) -> Path:
+    async def finalize_upload(self, uuid: str, digest: str) -> Path:
         raise NotImplementedError()
 
     def link_blob(self, digest: str, target: Path):
         raise NotImplementedError()
 
     def link_blob_ignore_quota(self, digest: str, target: Path):
         raise NotImplementedError()
@@ -145,16 +144,18 @@
         self, uuid: str, stream: Callable[[int], Awaitable[bytes]]
     ) -> int:
         return await _stream_to_file(stream, self.upload_path(uuid))
 
     def cancel_upload(self, uuid: str):
         self.upload_path(uuid).unlink()
 
-    def finalize_upload(self, uuid: str, digest: str) -> Path:
-        return _check_and_move(self.upload_path(uuid), self.blob_path(digest), digest)
+    async def finalize_upload(self, uuid: str, digest: str) -> Path:
+        return await _check_and_move(
+            self.upload_path(uuid), self.blob_path(digest), digest
+        )
 
     def link_blob(self, digest: str, target: Path):
         _hardlink(self.blob_path(digest), target)
 
     def link_blob_ignore_quota(self, digest: str, target: Path):
         _hardlink(self.blob_path(digest), target)
 
@@ -253,17 +254,17 @@
         self, uuid: str, stream: Callable[[int], Awaitable[bytes]]
     ) -> int:
         try:
             return await _stream_to_file(stream, self.base.upload_path(uuid), self)
         finally:
             self.disk_usage_save()
 
-    def finalize_upload(self, uuid: str, digest: str) -> Path:
+    async def finalize_upload(self, uuid: str, digest: str) -> Path:
         try:
-            return _check_and_move(
+            return await _check_and_move(
                 self.base.upload_path(uuid), self.base.blob_path(digest), digest, self
             )
         finally:
             self.disk_usage_save()
 
     def blob_path(self, digest: str, parent: Optional[Path] = None) -> Path:
         return self.base.blob_path(digest, parent=parent)
@@ -318,34 +319,20 @@
         dst.unlink()
     if user_repo is not None:
         user_repo.disk_usage_add(src.stat().st_size)
     os.link(src, dst)
 
 
 # --------------------------------------------------------------------------------------
-def _file_digest(algo: str, path: Path) -> str:
-    h = hashlib.new(algo)
-    buf = bytearray(CHUNK_SIZE)
-    view = memoryview(buf)
-    # TODO: call blocking stuff (open, readinto) in a thread?
-    with path.open("rb") as f:
-        while True:
-            n = f.readinto(buf)
-            if not n:
-                break
-            h.update(view[:n])
-    return h.hexdigest()
-
-
-# --------------------------------------------------------------------------------------
-def _check_and_move(
+async def _check_and_move(
     src: Path, dst: Path, digest: str, user_repo: Optional[UserRepository] = None
 ):
     algo, dig = parse_digest(digest.lower())
-    if _file_digest(algo, src) != dig:
+    loop = asyncio.get_running_loop()
+    if await loop.run_in_executor(None, file_digest, algo, src) != dig:
         if user_repo is not None:
             user_repo.disk_usage_rm(src.stat().st_size)
         src.unlink()
         try:
             os.removedirs(src.parent)
         except OSError:
             pass
```

### Comparing `dlrepo-0.5/dlrepo/fs/branch.py` & `dlrepo-0.8/dlrepo/fs/branch.py`

 * *Files identical despite different names*

### Comparing `dlrepo-0.5/dlrepo/fs/container.py` & `dlrepo-0.8/dlrepo/fs/container.py`

 * *Files identical despite different names*

### Comparing `dlrepo-0.5/dlrepo/fs/fmt.py` & `dlrepo-0.8/dlrepo/views/job.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,150 +1,120 @@
 # Copyright (c) 2021 Julien Floret
 # Copyright (c) 2021 Robin Jarry
 # SPDX-License-Identifier: BSD-3-Clause
 
-import json
-import logging
-import os
-from pathlib import Path
-from typing import Awaitable, Callable, Dict, Iterator, List, Tuple
+from aiohttp import web
+import aiohttp_jinja2
 
-from cachetools import LRUCache, cachedmethod
+from .util import BaseView, TarResponse
 
-from .util import SubDir
 
-
-LOG = logging.getLogger(__name__)
+# --------------------------------------------------------------------------------------
+class JobArchiveView(BaseView):
+    @classmethod
+    def urls(cls):
+        yield "/branches/{branch}/{tag}/{job}.tar"
+        yield "/~{user}/branches/{branch}/{tag}/{job}.tar"
+
+    def _get_job(self):
+        match = self.request.match_info
+        if match["tag"] in ("latest", "stable") and self.request.method != "GET":
+            raise web.HTTPMethodNotAllowed(self.request.method, ["GET"])
+        try:
+            return (
+                self.repo()
+                .get_branch(match["branch"])
+                .get_tag(match["tag"])
+                .get_job(match["job"])
+            )
+        except FileNotFoundError as e:
+            raise web.HTTPNotFound() from e
+
+    def _digests(self, job):
+        digests = {}
+        for fmt in job.get_formats():
+            if self.access_granted(fmt.url()):
+                for f, digest in fmt.get_digests().items():
+                    digests[f"{fmt.name}/{f}"] = digest
+        return digests
+
+    async def get(self):
+        job = self._get_job()
+        url = job.url().rstrip("/") + ".tar"
+        if url != self.request.path:
+            raise web.HTTPFound(url)
+        return TarResponse(self._digests(job), job.path(), job.archive_name())
 
 
 # --------------------------------------------------------------------------------------
-class ArtifactFormat(SubDir):
-    """
-    TODO
-    """
-
-    def url_bit(self) -> str:
-        return self.name
-
-    def get_files(self) -> Iterator[str]:
-        for root, dirs, files in os.walk(self._path):
-            dirs.sort()
-            files.sort()
-            for f in files:
-                f = Path(root, f)
-                if self._is_reserved_file(f):
-                    continue
-                if f.is_file():
-                    yield str(f.relative_to(self._path))
-
-    def archive_name(self) -> str:
-        return f"{self.parent.archive_name()}-{self.name}"
-
-    _is_reserved_cache = LRUCache(4096)
-
-    @cachedmethod(lambda self: self._is_reserved_cache)
-    def _is_reserved_file(self, path, *, resolve=False):
-        internal = self._internal_path()
-        digests = self._digest_path()
-        dirty = self._dirty_path()
-        if resolve:
-            internal = internal.resolve()
-            digests = digests.resolve()
-            dirty = dirty.resolve()
-        return path in (internal, digests, dirty)
-
-    def list_dir(self, relpath: str) -> Tuple[List[str], List[str]]:
-        path = self.get_filepath(relpath)
-        if not path.is_dir():
-            raise NotADirectoryError(relpath)
-        dirs = []
-        files = []
-        for e in path.iterdir():
-            if self._is_reserved_file(e, resolve=True):
-                continue
-            if e.is_dir():
-                dirs.append(e.name)
-            elif e.is_file():
-                files.append(e.name)
-        return dirs, files
-
-    def _check_filepath(self, relpath: str) -> Path:
-        if relpath.startswith("/") or any(x in (".", "..") for x in relpath.split("/")):
-            raise PermissionError(relpath)
-        path = self._path / relpath
-        if self._is_reserved_file(path):
-            raise PermissionError(relpath)
-        return path
-
-    def get_filepath(self, relpath: str) -> Path:
-        return self._check_filepath(relpath).resolve(strict=True)
-
-    def get_digests(self) -> Dict[str, str]:
-        try:
-            return json.loads(self._digest_path().read_text())
-        except (OSError, ValueError):
-            return {}
-
-    def _digest_path(self) -> Path:
-        return self._path / ".digests"
-
-    async def add_file(
-        self,
-        relpath: str,
-        read: Callable[[int], Awaitable[bytes]],
-        digest: str,
-    ):
-        self._check_filepath(relpath)
-        uuid = self.root().next_upload()
-        await self.root().update_upload(uuid, read)
-        self.root().finalize_upload(uuid, digest)
-        # avoid counting disk usage twice (already counted in update_upload()
-        self.link_file(digest, relpath, ignore_quota=True)
-
-    def link_file(self, digest: str, relpath: str, ignore_quota: bool = False):
-        was_dirty = self.is_dirty()
-        self.set_dirty(True)
-        try:
-            path = self._check_filepath(relpath)
-            if ignore_quota:
-                self.root().link_blob_ignore_quota(digest, path)
-            else:
-                self.root().link_blob(digest, path)
-        except:
-            if not was_dirty:
-                self.set_dirty(False)
-            raise
-        # update digests file
-        digests = self.get_digests()
-        digests[relpath] = digest
-        self._digest_path().write_text(json.dumps(digests))
-
-    def _internal_path(self) -> Path:
-        return self._path / ".internal"
-
-    def is_internal(self) -> bool:
-        return self._internal_path().is_file()
-
-    def set_internal(self, internal: bool):
-        path = self._internal_path()
-        if internal:
-            path.touch()
-        elif path.is_file():
-            path.unlink()
-
-    def _dirty_path(self) -> Path:
-        return self._path / ".dirty"
-
-    def is_dirty(self) -> bool:
-        return self._dirty_path().is_file()
-
-    def set_dirty(self, dirty: bool):
-        path = self._dirty_path()
-        if dirty:
-            path.parent.mkdir(mode=0o755, parents=True, exist_ok=True)
-            path.touch()
-        elif path.is_file():
-            path.unlink()
-            try:
-                os.removedirs(path.parent)
-            except OSError:
-                pass
+class JobView(JobArchiveView):
+    @classmethod
+    def urls(cls):
+        yield "/branches/{branch}/{tag}/{job}"
+        yield "/branches/{branch}/{tag}/{job}/"
+        yield "/~{user}/branches/{branch}/{tag}/{job}"
+        yield "/~{user}/branches/{branch}/{tag}/{job}/"
+
+    async def get(self):
+        """
+        Get info about a job including metadata and artifact formats.
+        """
+        job = self._get_job()
+        if not job.exists():
+            raise web.HTTPNotFound()
+        if job.url() != self.request.path:
+            raise web.HTTPFound(job.url())
+        html = "html" in self.request.headers.get("Accept", "json")
+        data = {"job": job.get_metadata()}
+        formats = []
+        for f in job.get_formats():
+            if self.access_granted(f.url()):
+                if html:
+                    formats.append({"name": f.name, "internal": f.is_internal()})
+                else:
+                    formats.append(f.name)
+        data["job"]["artifact_formats"] = formats
+        if html:
+            return aiohttp_jinja2.render_template("job.html", self.request, data)
+        return web.json_response(data)
+
+    async def put(self):
+        try:
+            locked = (await self.json_body())["job"]["locked"]
+            if not isinstance(locked, bool):
+                raise TypeError()
+        except (TypeError, KeyError) as e:
+            raise web.HTTPBadRequest(reason="Invalid parameters") from e
+        try:
+            self._get_job().set_locked(locked)
+        except FileNotFoundError as e:
+            raise web.HTTPNotFound() from e
+        return web.Response()
+
+    async def patch(self):
+        """
+        Update the metadata of a job.
+        """
+        try:
+            data = (await self.json_body())["job"]
+            if not isinstance(data, dict):
+                raise TypeError()
+        except (TypeError, KeyError) as e:
+            raise web.HTTPBadRequest(reason="Invalid parameters") from e
+        try:
+            self._get_job().add_metadata(data)
+        except FileExistsError as e:
+            raise web.HTTPBadRequest(reason=str(e)) from e
+        return web.Response()
+
+    async def delete(self):
+        """
+        Delete a job and all its contents.
+        """
+        try:
+            job = self._get_job()
+            job.delete()
+        except FileNotFoundError as e:
+            raise web.HTTPNotFound() from e
+        except OSError as e:
+            raise web.HTTPBadRequest(reason=str(e)) from e
+        return web.Response()
```

### Comparing `dlrepo-0.5/dlrepo/fs/job.py` & `dlrepo-0.8/dlrepo/fs/job.py`

 * *Files identical despite different names*

### Comparing `dlrepo-0.5/dlrepo/fs/product.py` & `dlrepo-0.8/dlrepo/fs/product.py`

 * *Files identical despite different names*

### Comparing `dlrepo-0.5/dlrepo/fs/tag.py` & `dlrepo-0.8/dlrepo/fs/tag.py`

 * *Files identical despite different names*

### Comparing `dlrepo-0.5/dlrepo/fs/util.py` & `dlrepo-0.8/dlrepo/fs/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright (c) 2021 Julien Floret
 # Copyright (c) 2021 Robin Jarry
 # SPDX-License-Identifier: BSD-3-Clause
 
 import hashlib
+import os
 from pathlib import Path
 import re
 from typing import Iterator, Tuple, Union
 
 
 # --------------------------------------------------------------------------------------
 class SubDir:
@@ -85,14 +86,31 @@
     match = ALGO_RE.match(digest)
     if not match:
         raise ValueError(f"invalid digest: {digest}")
     return match.groups()
 
 
 # --------------------------------------------------------------------------------------
+CHUNK_SIZE = int(os.getenv("DLREPO_CHUNK_SIZE", str(256 * 1024)))
+
+
+def file_digest(algo: str, path: Path) -> str:
+    h = hashlib.new(algo)
+    buf = bytearray(CHUNK_SIZE)
+    view = memoryview(buf)
+    with path.open("rb") as f:
+        while True:
+            n = f.readinto(buf)
+            if not n:
+                break
+            h.update(view[:n])
+    return h.hexdigest()
+
+
+# --------------------------------------------------------------------------------------
 def human_readable(value):
     if value == 0:
         return "0"
     units = ("K", "M", "G", "T")
     i = 0
     unit = ""
     while value >= 1000 and i < len(units):
```

### Comparing `dlrepo-0.5/dlrepo/static/favicon.svg` & `dlrepo-0.8/dlrepo/static/favicon.svg`

 * *Files identical despite different names*

### Comparing `dlrepo-0.5/dlrepo/static/locked.svg` & `dlrepo-0.8/dlrepo/static/locked.svg`

 * *Files identical despite different names*

### Comparing `dlrepo-0.5/dlrepo/static/logo.svg` & `dlrepo-0.8/dlrepo/static/logo.svg`

 * *Files identical despite different names*

### Comparing `dlrepo-0.5/dlrepo/static/released.svg` & `dlrepo-0.8/dlrepo/static/released.svg`

 * *Files identical despite different names*

### Comparing `dlrepo-0.5/dlrepo/templates/autoindex.html` & `dlrepo-0.8/dlrepo/templates/autoindex.html`

 * *Files 20% similar despite different names*

```diff
@@ -14,16 +14,21 @@
 {{breadcrumbs(["products", product, variant, product_branch, version] + path )}}
 {% endif %}
 {% endblock %}
 
 {% block page_content %}
 {% set width = (artifact_format.dirs + artifact_format.files)|map('length')|max|default(80) %}
 {% set width = [width, 10]|max %}
-<section class="autoindex" style="column-width: {{width * 0.6}}em;">
+<section class="autoindex" style="column-width: {{width * 0.8}}em;">
 {% for d in artifact_format.dirs|sort(case_sensitive=true) %}
-  <a href="{{d}}/" class="directory">{{d}}/</a>
+  <div>
+    <a href="{{d}}/" class="directory">{{d}}/</a>
+  </div>
 {% endfor %}
 {% for f in artifact_format.files|sort(case_sensitive=true) %}
-  <a href="{{f}}" class="file">{{f}}</a>
+  <div>
+    <a href="{{f}}" class="file">{{f}}</a>
+    <a href="{{f}}.sha256" class="digest">sha256</a>
+  </div>
 {% endfor %}
 </div>
 {% endblock %}
```

#### html2text {}

```diff
@@ -3,11 +3,13 @@
 breadcrumbs %} {% set path = [artifact_format.name] %} {% if
 artifact_format.relpath %} {% do path.extend(artifact_format.relpath.split("/
 ")) %} {% endif %} {% if branch %} {{breadcrumbs(["branches", branch, tag, job]
 + path )}} {% else %} {{breadcrumbs(["products", product, variant,
 product_branch, version] + path )}} {% endif %} {% endblock %} {% block
 page_content %} {% set width = (artifact_format.dirs +
 artifact_format.files)|map('length')|max|default(80) %} {% set width = [width,
-10]|max %}  {% for d in artifact_format.dirs|sort(case_sensitive=true) %} {
-{d}}/ {% endfor %} {% for f in artifact_format.files|sort(case_sensitive=true)
-%} {{f}} {% endfor %}
+10]|max %}  {% for d in artifact_format.dirs|sort(case_sensitive=true) %}
+{{d}}/
+{% endfor %} {% for f in artifact_format.files|sort(case_sensitive=true) %}
+{{f}} sha256
+{% endfor %}
 {% endblock %}
```

### Comparing `dlrepo-0.5/dlrepo/templates/base.html` & `dlrepo-0.8/dlrepo/templates/base.html`

 * *Files identical despite different names*

### Comparing `dlrepo-0.5/dlrepo/templates/branch.html` & `dlrepo-0.8/dlrepo/templates/branch.html`

 * *Files identical despite different names*

### Comparing `dlrepo-0.5/dlrepo/templates/branches.html` & `dlrepo-0.8/dlrepo/templates/branches.html`

 * *Files identical despite different names*

### Comparing `dlrepo-0.5/dlrepo/templates/home.html` & `dlrepo-0.8/dlrepo/templates/home.html`

 * *Files identical despite different names*

### Comparing `dlrepo-0.5/dlrepo/templates/job.html` & `dlrepo-0.8/dlrepo/templates/job.html`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,17 @@
          {% if fmt.internal %}
          title="internal format (not for release)"
          {% endif %}>
       <a href="{{fmt.name}}" class="format">{{fmt.name}}/</a>
       <a href="{{fmt.name}}.tar" class="archive" title="Whole archive">
         {{fmt.name}}.tar
       </a>
+      <a href="{{fmt.name}}.sha256" class="digest" title="SHA-256 digests">
+        {{fmt.name}}.sha256
+      </a>
     </div>
     {% endfor %}
   </div>
 
   <div class="whole-archive">
     <a href="../{{job_name}}.tar" title="Whole archive (large file)">
       {{job_name}}.tar
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 job_name = job.pop("name") %} {% set formats = job.pop("artifact_formats", [])
 %} {% block breadcrumbs %} {{breadcrumbs(['branches', branch, tag, job_name])}}
 {% endblock %} {% block page_content %}
 ***** Files *****
 ===============================================================================
 {% for fmt in formats|sort(attribute="name") %}
 % if fmt.internal %} title="internal format (not for release)" {% endif %}> {
-{fmt.name}}/ {{fmt.name}}.tar
+{fmt.name}}/ {{fmt.name}}.tar {{fmt.name}}.sha256
 {% endfor %}
 {{job_name}}.tar
 {% if formats|selectattr("name", "equalto", "container")|list %} docker pull {
 {request.host}}/{{user + "/" if user}}{{branch}}/{{job_name}}:{{tag}} {% endif
 %}
 ***** Metadata *****
 ===============================================================================
```

### Comparing `dlrepo-0.5/dlrepo/templates/product.html` & `dlrepo-0.8/dlrepo/templates/product.html`

 * *Files identical despite different names*

### Comparing `dlrepo-0.5/dlrepo/templates/product_branch.html` & `dlrepo-0.8/dlrepo/templates/product_branch.html`

 * *Files identical despite different names*

### Comparing `dlrepo-0.5/dlrepo/templates/product_variant.html` & `dlrepo-0.8/dlrepo/templates/product_variant.html`

 * *Files identical despite different names*

### Comparing `dlrepo-0.5/dlrepo/templates/product_version.html` & `dlrepo-0.8/dlrepo/templates/product_version.html`

 * *Files 18% similar despite different names*

```diff
@@ -17,14 +17,17 @@
          {% if fmt.internal %}
          title="internal format (not for release)"
          {% endif %}>
       <a href="{{fmt.name}}" class="format">{{fmt.name}}/</a>
       <a href="{{fmt.name}}.tar" class="archive" title="Whole archive">
         {{fmt.name}}.tar
       </a>
+      <a href="{{fmt.name}}.sha256" class="digest" title="SHA-256 digests">
+        {{fmt.name}}.sha256
+      </a>
     </div>
     {% endfor %}
   </div>
 
   <div class="whole-archive">
     <a href="../{{version.name}}.tar" title="Whole archive (large file)">
       {{product}}-{{variant}}-v{{version.name}}.tar
```

#### html2text {}

```diff
@@ -2,13 +2,13 @@
 SPDX-License-Identifier: BSD-3-Clause #} {% extends "base.html" %} {% block
 breadcrumbs %} {{breadcrumbs(['products', product, variant, product_branch,
 version.name])}} {% endblock %} {% block page_content %}
 ***** Files *****
 ===============================================================================
 {% for fmt in version.artifact_formats|sort(attribute="name") %}
 % if fmt.internal %} title="internal format (not for release)" {% endif %}> {
-{fmt.name}}/ {{fmt.name}}.tar
+{fmt.name}}/ {{fmt.name}}.tar {{fmt.name}}.sha256
 {% endfor %}
 {{product}}-{{variant}}-v{{version.name}}.tar
 {% if version.artifact_formats|selectattr("name", "equalto", "container")|list
 %} docker pull {{request.host}}/{{user + "/" if user}}{{product}}/{{variant}}/{
 {product_branch}}:{{version.name}} {% endif %}  {% endblock %}
```

### Comparing `dlrepo-0.5/dlrepo/templates/products.html` & `dlrepo-0.8/dlrepo/templates/products.html`

 * *Files identical despite different names*

### Comparing `dlrepo-0.5/dlrepo/templates/tag.html` & `dlrepo-0.8/dlrepo/templates/tag.html`

 * *Files identical despite different names*

### Comparing `dlrepo-0.5/dlrepo/views/__init__.py` & `dlrepo-0.8/dlrepo/views/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     CatalogView,
     ManifestReadOnlyView,
     ManifestView,
     NewBlobUploadView,
     RootView,
     TagsListView,
 )
-from .fmt import FormatArchiveView, FormatDirView, FormatFileView
+from .fmt import FormatArchiveView, FormatDigestsView, FormatDirView, FormatFileView
 from .job import JobArchiveView, JobView
 from .product import (
     ProductBranchView,
     ProductsView,
     ProductVariantView,
     ProductView,
     VersionArchiveView,
@@ -193,14 +193,15 @@
         # artifacts
         BranchesView,
         BranchView,
         TagView,
         JobArchiveView,
         JobView,
         FormatArchiveView,
+        FormatDigestsView,
         FormatFileView,
         FormatDirView,
         ArtifactView,
         ProductsView,
         ProductView,
         ProductVariantView,
         ProductBranchView,
```

### Comparing `dlrepo-0.5/dlrepo/views/artifact.py` & `dlrepo-0.8/dlrepo/views/artifact.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright (c) 2021 Julien Floret
 # Copyright (c) 2021 Robin Jarry
 # SPDX-License-Identifier: BSD-3-Clause
 
 import hashlib
+import os
 
 from aiohttp import web
 
 from .util import BaseView
 
 
 # --------------------------------------------------------------------------------------
@@ -92,32 +93,43 @@
         fmt = self._get_format()
         artifact = self.request.match_info["artifact"]
         try:
             filepath = fmt.get_filepath(artifact)
         except PermissionError as e:
             raise web.HTTPBadRequest(reason=str(e)) from e
         except FileNotFoundError as e:
+            if artifact.endswith(".sha256"):
+                artifact = artifact[: -len(".sha256")]
+                digest = fmt.get_digests().get(artifact)
+                if digest is not None:
+                    algo, digest = digest.split(":")
+                    if algo == "sha256":
+                        url = fmt.url() + artifact + ".sha256"
+                        if url != self.request.path:
+                            raise web.HTTPFound(url)
+                        artifact = os.path.basename(artifact)
+                        return web.Response(text=f"{digest}  {artifact}\n")
             raise web.HTTPNotFound() from e
         url = fmt.url() + artifact
         if filepath.is_dir():
             if "html" in self.request.headers.get("Accept", "json"):
                 if not url.endswith("/"):
                     raise web.HTTPFound(url + "/")
                 if url != self.request.path:
                     raise web.HTTPFound(url)
                 return await self.autoindex(fmt, artifact)
             raise web.HTTPNotFound()
         if url != self.request.path:
             raise web.HTTPFound(url)
-        headers = {"Content-Length": str(filepath.stat().st_size)}
         digest = fmt.get_digests().get(artifact)
         if not digest and fmt.name == "container":
             algo = filepath.parent.parent.name
             if algo in hashlib.algorithms_guaranteed:
                 digest = f"{algo}:{filepath.name}"
+        headers = {}
         if digest:
             headers["Digest"] = digest
         return web.FileResponse(filepath, headers=headers)
 
     async def put(self):
         fmt = self._get_format(create=True)
         artifact = self.request.match_info["artifact"]
```

### Comparing `dlrepo-0.5/dlrepo/views/auth.py` & `dlrepo-0.8/dlrepo/views/auth.py`

 * *Files identical despite different names*

### Comparing `dlrepo-0.5/dlrepo/views/branch.py` & `dlrepo-0.8/dlrepo/views/branch.py`

 * *Files identical despite different names*

### Comparing `dlrepo-0.5/dlrepo/views/container.py` & `dlrepo-0.8/dlrepo/views/container.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,15 +235,15 @@
 
     async def put(self):
         uuid = self.request.match_info["uuid"]
         try:
             digest = self.request.query["digest"]
             if int(self.request.headers.get("Content-Length", "0")) > 0:
                 await self.repo().update_upload(uuid, self.request.content.read)
-            self.repo().finalize_upload(uuid, digest)
+            await self.repo().finalize_upload(uuid, digest)
         except PermissionError as e:
             raise errors.Denied(str(e)) from e
         except ValueError as e:
             raise errors.BlobUploadInvalid() from e
         except KeyError as e:
             self.repo().cancel_upload(uuid)
             raise errors.BlobUploadInvalid() from e
```

### Comparing `dlrepo-0.5/dlrepo/views/errors.py` & `dlrepo-0.8/dlrepo/views/errors.py`

 * *Files identical despite different names*

### Comparing `dlrepo-0.5/dlrepo/views/fmt.py` & `dlrepo-0.8/dlrepo/views/fmt.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 # Copyright (c) 2021 Julien Floret
 # Copyright (c) 2021 Robin Jarry
 # SPDX-License-Identifier: BSD-3-Clause
 
+import logging
+
 from aiohttp import web
 
 from .util import BaseView, TarResponse
 
 
+LOG = logging.getLogger(__name__)
+
+
 # --------------------------------------------------------------------------------------
 class FormatDirView(BaseView):
     @classmethod
     def urls(cls):
         yield "/branches/{branch}/{tag}/{job}/{format}/"
         yield "/~{user}/branches/{branch}/{tag}/{job}/{format}/"
         yield "/products/{product}/{variant}/{product_branch}/{version}/{format}/"
@@ -34,15 +39,15 @@
         if "html" in self.request.headers.get("Accept", "json"):
             return await self.autoindex(fmt, "")
         data = {
             "artifact_format": {
                 "name": fmt.name,
                 "internal": fmt.is_internal(),
                 "dirty": fmt.is_dirty(),
-                "files": list(fmt.get_files()),
+                "files": list(fmt.get_digests().keys()),
             },
         }
         return web.json_response(data)
 
     async def put(self):
         """
         Change the internal state for a format
@@ -69,17 +74,19 @@
         version = self.request.match_info.get(
             "tag", self.request.match_info.get("version")
         )
         if "product" in self.request.match_info or version in ("latest", "stable"):
             raise web.HTTPMethodNotAllowed("PATCH", ["GET"])
         fmt = _get_format(self.repo(), self.request.match_info)
         try:
+            await fmt.post_process()
             fmt.set_dirty(False)
-        except (TypeError, KeyError) as e:
-            raise web.HTTPBadRequest() from e
+        except OSError as e:
+            LOG.error("post process failed: %s", e)
+            raise web.HTTPInternalServerError(reason="post process failed") from e
         return web.Response()
 
 
 # --------------------------------------------------------------------------------------
 class FormatArchiveView(BaseView):
     @classmethod
     def urls(cls):
@@ -98,15 +105,37 @@
         return web.Response()
 
     async def get(self):
         fmt = _get_format(self.repo(), self.request.match_info)
         url = fmt.url().rstrip("/") + ".tar"
         if url != self.request.path:
             raise web.HTTPFound(url)
-        return TarResponse(fmt.get_files(), fmt.path(), fmt.archive_name())
+        return TarResponse(fmt.get_digests(), fmt.path(), fmt.archive_name())
+
+
+# --------------------------------------------------------------------------------------
+class FormatDigestsView(BaseView):
+    @classmethod
+    def urls(cls):
+        yield "/branches/{branch}/{tag}/{job}/{format}.sha256"
+        yield "/~{user}/branches/{branch}/{tag}/{job}/{format}.sha256"
+        yield "/products/{product}/{variant}/{product_branch}/{version}/{format}.sha256"
+        yield "/~{user}/products/{product}/{variant}/{product_branch}/{version}/{format}.sha256"
+
+    async def get(self):
+        fmt = _get_format(self.repo(), self.request.match_info)
+        url = fmt.url().rstrip("/") + ".sha256"
+        if url != self.request.path:
+            raise web.HTTPFound(url)
+        sha256sums = []
+        for artifact, digest in sorted(fmt.get_digests().items()):
+            algo, digest = digest.split(":")
+            if algo == "sha256":
+                sha256sums.append(f"{digest}  {artifact}\n")
+        return web.Response(text="".join(sha256sums))
 
 
 # --------------------------------------------------------------------------------------
 class FormatFileView(BaseView):
     @classmethod
     def urls(cls):
         yield "/branches/{branch}/{tag}/{job}/{format}"
@@ -115,30 +144,30 @@
         yield "/~{user}/products/{product}/{variant}/{product_branch}/{version}/{format}"
 
     async def head(self):
         fmt = _get_format(self.repo(), self.request.match_info)
         if fmt.is_dirty():
             raise web.HTTPNotFound()
         url = fmt.url()
-        files = list(fmt.get_files())
+        files = list(fmt.get_digests().keys())
         if len(files) == 1:
             url += files[0]
         if url != self.request.path:
             raise web.HTTPFound(url)
         return web.Response()
 
     async def get(self):
         """
         If only one file in $format:
             redirect to /branches/$branch/$tag/$job/$format/$file
         else:
             redirect to /branches/$branch/$tag/$job/$format/
         """
         fmt = _get_format(self.repo(), self.request.match_info)
-        files = list(fmt.get_files())
+        files = list(fmt.get_digests().keys())
         if len(files) == 1 and files[0] != "index.html":
             return web.HTTPFound(fmt.url() + files[0])
         return web.HTTPFound(fmt.url())
 
 
 # --------------------------------------------------------------------------------------
 def _get_format(repo, match_info):
```

### Comparing `dlrepo-0.5/dlrepo/views/product.py` & `dlrepo-0.8/dlrepo/views/product.py`

 * *Files 5% similar despite different names*

```diff
@@ -209,19 +209,23 @@
 # --------------------------------------------------------------------------------------
 class VersionArchiveView(VersionView):
     @classmethod
     def urls(cls):
         yield "/products/{product}/{variant}/{product_branch}/{version}.tar"
         yield "/~{user}/products/{product}/{variant}/{product_branch}/{version}.tar"
 
-    def _files(self, version):
+    def _digests(self, version):
+        digests = {}
         for fmt in version.get_formats():
             if self.access_granted(fmt.url()):
-                for f in fmt.get_files():
-                    yield f"{fmt.name}/{f}"
+                for f, digest in fmt.get_digests().items():
+                    digests[f"{fmt.name}/{f}"] = digest
+        return digests
 
     async def get(self):
         version = self._get_version()
         url = version.url().rstrip("/") + ".tar"
         if url != self.request.path:
             raise web.HTTPFound(version.url())
-        return TarResponse(self._files(version), version.path(), version.archive_name())
+        return TarResponse(
+            self._digests(version), version.path(), version.archive_name()
+        )
```

### Comparing `dlrepo-0.5/dlrepo/views/tag.py` & `dlrepo-0.8/dlrepo/views/tag.py`

 * *Files identical despite different names*

### Comparing `dlrepo-0.5/dlrepo/views/util.py` & `dlrepo-0.8/dlrepo/views/util.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import asyncio
 from http import HTTPStatus
 import json
 import os
 from pathlib import Path
 import tarfile
-from typing import Iterable, Tuple
+from typing import Dict, Tuple
 
 from aiohttp import web
 from aiohttp.abc import AbstractStreamWriter
 import aiohttp_jinja2
 
 from . import auth
 
@@ -65,33 +65,38 @@
             },
         }
         return aiohttp_jinja2.render_template("autoindex.html", self.request, data)
 
 
 # --------------------------------------------------------------------------------------
 class TarResponse(web.StreamResponse):
-    def __init__(self, members: Iterable[str], root_dir: Path, tar_prefix: str = None):
+    def __init__(self, members: Dict[str, str], root_dir: Path, tar_prefix: str = None):
         self._members = members
         self._root_dir = root_dir
         self._tar_prefix = tar_prefix
         super().__init__()
         self.content_type = "application/x-tar"
         if self._tar_prefix is not None:
             filename = self._tar_prefix + ".tar"
             self.headers.add("Content-Disposition", f"attachment; filename={filename}")
 
     async def prepare(self, request: web.Request) -> AbstractStreamWriter:
+        # pylint: disable=too-many-locals
         writer = await super().prepare(request)
         transport = request.transport
         loop = asyncio.get_running_loop()
 
         tar_offset = 0
+        sha256sums = []
 
-        for member in self._members:
+        for member, digest in sorted(self._members.items()):
             info, path = await self._get_tar_info(member)
+            algo, digest = digest.split(":")
+            if algo == "sha256":
+                sha256sums.append(f"{digest}  {member}\n")
 
             buf = info.tobuf(tarfile.PAX_FORMAT, "utf-8")
             await self.write(buf)  # includes http chunk header & trailer
             tar_offset += len(buf)
 
             fobj = await loop.run_in_executor(None, path.open, "rb")
             try:
@@ -106,14 +111,17 @@
                     # add tar member padding (includes http chunk header & trailer)
                     await self.write(self._padding(tarfile.BLOCKSIZE - remainder))
                     blocks += 1
                 tar_offset += blocks * tarfile.BLOCKSIZE
             finally:
                 await loop.run_in_executor(None, fobj.close)
 
+        if sha256sums:
+            tar_offset += await self._write_sha256sums(sha256sums)
+
         # add tar format trailer
         tar_trailer = self._padding(2 * tarfile.BLOCKSIZE)
         tar_offset += 2 * tarfile.BLOCKSIZE
         remainder = tar_offset % tarfile.RECORDSIZE
         if remainder > 0:
             tar_trailer += self._padding(tarfile.RECORDSIZE - remainder)
 
@@ -137,7 +145,31 @@
         st = await loop.run_in_executor(None, path.lstat)
 
         info = tarfile.TarInfo(name)
         info.mode = st.st_mode
         info.size = st.st_size
 
         return info, path
+
+    async def _write_sha256sums(self, sha256sums):
+        name = "SHA256SUMS.txt"
+        if self._tar_prefix is not None:
+            name = f"{self._tar_prefix}/{name}"
+
+        data = "".join(sha256sums).encode("utf-8")
+
+        info = tarfile.TarInfo(name)
+        info.mode = 0o0644
+        info.size = len(data)
+
+        buf = info.tobuf(tarfile.PAX_FORMAT, "utf-8") + data
+        offset = len(buf)
+        blocks, remainder = divmod(info.size, tarfile.BLOCKSIZE)
+        if remainder > 0:
+            # add tar member padding
+            buf += self._padding(tarfile.BLOCKSIZE - remainder)
+            blocks += 1
+        offset += blocks * tarfile.BLOCKSIZE
+
+        await self.write(buf)  # includes http chunk header & trailer
+
+        return offset
```

### Comparing `dlrepo-0.5/dlrepo-cli` & `dlrepo-0.8/dlrepo-cli`

 * *Files identical despite different names*

### Comparing `dlrepo-0.5/dlrepo.egg-info/PKG-INFO` & `dlrepo-0.8/dlrepo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlrepo
-Version: 0.5
+Version: 0.8
 Summary: Artifact repository
 Home-page: https://sr.ht/~rjarry/dlrepo/
 Author: Robin Jarry
 Author-email: robin@jarry.cc
 License: BSD-3-Clause
 Description: # dlrepo
```

### Comparing `dlrepo-0.5/dlrepo.egg-info/SOURCES.txt` & `dlrepo-0.8/dlrepo.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -61,19 +61,28 @@
 docs/dlrepo.7.scdoc
 etc/default
 etc/dlrepo-cleanup.service
 etc/dlrepo-cleanup.timer
 etc/dlrepo.service
 etc/dlrepo.socket
 etc/nginx.conf
+etc/post-process.sh
 scss/components.scss
 scss/layout.scss
 scss/main.scss
 scss/normalize.scss
 scss/sections.scss
 scss/variables.scss
 tests/conftest.py
+tests/test_archive.py
 tests/test_auth.py
+tests/test_digests.py
+tests/test_post_process.py
 tests/test_auth/auth
 tests/test_auth/acls/group1
 tests/test_auth/acls/group2
-tests/test_auth/acls/group3
+tests/test_auth/acls/group3
+tests/test_post_process/post-process.sh
+tests/test_post_process/branches/branch/tag/job/fmt/file.txt
+tests/test_post_process/branches/branch/tag/job/fmt/file2.txt
+tests/test_post_process/branches/branch/tag/job/fmt-error/file3.txt
+tests/test_post_process/branches/branch/tag/job/fmt-ignored/foo.txt
```

### Comparing `dlrepo-0.5/docs/dlrepo-acls.5.scdoc` & `dlrepo-0.8/docs/dlrepo-acls.5.scdoc`

 * *Files identical despite different names*

### Comparing `dlrepo-0.5/docs/dlrepo-api.7.scdoc` & `dlrepo-0.8/docs/dlrepo-api.7.scdoc`

 * *Files 4% similar despite different names*

```diff
@@ -327,15 +327,16 @@
 *Errors:*
 	- _404_: the specified _{job}_ does not exist.
 
 ## GET /branches/{branch}/{tag}/{job}.tar
 ## GET /~{user}/branches/{branch}/{tag}/{job}.tar
 
 Get a tar archive of files contained in all artifact formats of the specified
-_{job}_.
+_{job}_. An extra _SHA256SUMS.txt_ file is appended to allow verification of
+the archive contents after extraction.
 
 *Access:*
 	_ro_
 
 	Only files from the artifact formats that the user has access to are
 	returned.
 *Response:*
@@ -558,15 +559,16 @@
 *Errors:*
 	- _404_: the specified _{job}_ does not exist.
 
 ## GET /products/{product}/{variant}/{product_branch}/{version}.tar
 ## GET /~{user}/products/{product}/{variant}/{product_branch}/{version}.tar
 
 Get a tar archive of files contained in all artifact formats of the specified
-_{version}_.
+_{version}_. An extra _SHA256SUMS.txt_ file is appended to allow verification
+of the archive contents after extraction.
 
 *Access:*
 	_ro_
 
 	Only files from the artifact formats that the user has access to are
 	returned.
 *Response:*
@@ -622,22 +624,40 @@
 	- _404_: the specified _{format}_ does not exist.
 
 ## GET /branches/{branch}/{tag}/{job}/{format}.tar
 ## GET /products/{product}/{variant}/{product_branch}/{version}/{format}.tar
 ## GET /~{user}/branches/{branch}/{tag}/{job}/{format}.tar
 ## GET /~{user}/products/{product}/{variant}/{product_branch}/{version}/{format}.tar
 
-Get a tar archive of files contained in the specified artifact _{format}_.
+Get a tar archive of files contained in the specified artifact _{format}_. An
+extra _SHA256SUMS.txt_ file is appended to allow verification of the archive
+contents after extraction.
 
 *Access:*
 	_ro_
 *Response:*
 	A POSIX tar archive (_application/x-tar_).
 *Errors:*
-	- _404_: the specified _{version}_ does not exist.
+	- _404_: the specified _{format}_ does not exist.
+
+## GET /branches/{branch}/{tag}/{job}/{format}.sha256
+## GET /products/{product}/{variant}/{product_branch}/{version}/{format}.sha256
+## GET /~{user}/branches/{branch}/{tag}/{job}/{format}.sha256
+## GET /~{user}/products/{product}/{variant}/{product_branch}/{version}/{format}.sha256
+
+Get the SHA-256 digests of files in the specified artifact _{format}_.
+
+*Access:*
+	_ro_
+*Response:*
+	A plain text response with one line per file consisting of the SHA-256
+	digest of each file (64 hexadecimal characters) followed by two spaces
+	and the file name.
+*Errors:*
+	- _404_: the specified _{format}_ does not exist.
 
 ## HEAD /branches/{branch}/{tag}/{job}/{format}
 ## HEAD /branches/{branch}/{tag}/{job}/{format}/
 ## HEAD /products/{product}/{variant}/{product_branch}/{version}/{format}
 ## HEAD /products/{product}/{variant}/{product_branch}/{version}/{format}/
 ## HEAD /~{user}/branches/{branch}/{tag}/{job}/{format}
 ## HEAD /~{user}/branches/{branch}/{tag}/{job}/{format}/
@@ -678,21 +698,29 @@
 
 ## PATCH /branches/{branch}/{tag}/{job}/{format}/
 ## PATCH /products/{product}/{variant}/{product_branch}/{version}/{format}/
 ## PATCH /~{user}/branches/{branch}/{tag}/{job}/{format}/
 ## PATCH /~{user}/products/{product}/{variant}/{product_branch}/{version}/{format}/
 
 Clear the _dirty_ flag of the specified _{format}_. This flag is automatically
-set to _true_ when new files are uploaded.
+set to _true_ when new files are uploaded. If a *DLREPO_POST_PROCESS_CMD* is
+configured (see *dlrepo-config*(5)), the command will be executed synchronously
+with the artifact format folder as working directory before returning the
+response to the client.
+
+After the command is finished, all file digests in the _{format}_ will be
+refreshed since they may have been modified by the post process command. The
+_dirty_ flag will only be cleared if the command succeeds.
 
 *Access:*
 	_rw_
 *Errors:*
 	- _404_: the specified _{tag}_ or _{version}_ does not exist.
 	- _405_: _{tag}_ or _{version}_ is either _latest_ or _stable_.
+	- _500_: the post process command failed.
 
 # ARTIFACTS
 
 ## GET /branches/{branch}/{tag}/{job}/{format}/{artifact}
 ## GET /products/{product}/{variant}/{product_branch}/{version}/{format}/{artifact}
 ## GET /~{user}/branches/{branch}/{tag}/{job}/{format}/{artifact}
 ## GET /~{user}/products/{product}/{variant}/{product_branch}/{version}/{format}/{artifact}
@@ -707,14 +735,30 @@
 Digest: sha256:5387a5f82442013ed24e0e3674fac3bdea9d2f85c88c9e5938ad6792f81d7799
 
 	<file binary data>
 *Errors:*
 	- _400_: the requested _{artifact}_ path is invalid.
 	- _404_: the requested _{artifact}_ does not exist.
 
+## GET /branches/{branch}/{tag}/{job}/{format}/{artifact}.sha256
+## GET /products/{product}/{variant}/{product_branch}/{version}/{format}/{artifact}.sha256
+## GET /~{user}/branches/{branch}/{tag}/{job}/{format}/{artifact}.sha256
+## GET /~{user}/products/{product}/{variant}/{product_branch}/{version}/{format}/{artifact}.sha256
+
+Get the SHA-256 digest of the specified _{artifact}_ file.
+
+*Access:*
+	_ro_
+*Response:*
+	The SHA-256 digest of the file (64 hexadecimal characters) followed by
+	two spaces and the file name.
+*Errors:*
+	- _400_: the requested _{artifact}_ path is invalid.
+	- _404_: the requested _{artifact}_ does not exist.
+
 ## HEAD /branches/{branch}/{tag}/{job}/{format}/{artifact}
 ## HEAD /products/{product}/{variant}/{product_branch}/{version}/{format}/{artifact}
 ## HEAD /~{user}/branches/{branch}/{tag}/{job}/{format}/{artifact}
 ## HEAD /~{user}/products/{product}/{variant}/{product_branch}/{version}/{format}/{artifact}
 
 Check if the specified _{artifact}_ file exists. Receive its size in bytes and
 its SHA-256 digest.
```

### Comparing `dlrepo-0.5/docs/dlrepo-cleanup.8.scdoc` & `dlrepo-0.8/docs/dlrepo-cleanup.8.scdoc`

 * *Files identical despite different names*

### Comparing `dlrepo-0.5/docs/dlrepo-cli.1.scdoc` & `dlrepo-0.8/docs/dlrepo-cli.1.scdoc`

 * *Files identical despite different names*

### Comparing `dlrepo-0.5/docs/dlrepo-config.5.scdoc` & `dlrepo-0.8/docs/dlrepo-config.5.scdoc`

 * *Files 12% similar despite different names*

```diff
@@ -48,14 +48,34 @@
 	Only events that are above that level are sent to the system logs.
 	Valid values are _DEBUG_, _INFO_, _WARNING_ and _ERROR_.
 
 *DLREPO_USER_QUOTA* (default: _10737418240_)
 	The maximum disk usage in bytes per user repository. When the user quota
 	is exceeded, new uploads are denied with an explicit error.
 
+*DLREPO_POST_PROCESS_CMD* (optional)
+	Command to execute when finalizing an artifact format. It may be used
+	to perform sensible operations such as packages signing without
+	exposing the private key to the build system.
+
+	The finalization is done automatically when running the *dlrepo-cli*(1)
+	*upload* command. Or, alternatively by performing a _PATCH_ request on
+	an artifact format (see *dlrepo-api*(7)).
+
+	This should be either the path to an executable or its name if it is in
+	the system _PATH_. The command will be executed by the user running the
+	dlrepo daemon process with the artifact format folder as its working
+	directory and no arguments. Any output produced by the command will be
+	sent to the system logs.
+
+	If the command exits with a non-zero code, an error will be returned to
+	the client.
+
+	Example: _/etc/dlrepo/post-process.sh_
+
 *DLREPO_PUBLIC_URL* (optional)
 	If set, it will replace the default URL in the script contents that are
 	returned from the _/cli_ URL.
 
 ## customization
 
 *DLREPO_STATIC_DIR* (optional)
```

### Comparing `dlrepo-0.5/docs/dlrepo-layout.7.scdoc` & `dlrepo-0.8/docs/dlrepo-layout.7.scdoc`

 * *Files 2% similar despite different names*

```diff
@@ -136,14 +136,23 @@
 	```
 	{
 		"foo": "sha256:cea02954c76c9…70107c26c6569fae2",
 		"bar": "sha256:80109520116bf1…1108a0f4e4cf64381",
 		"moo/baz.tgz": "sha256:edd02954f7ac3…901be92d16362aef5",
 	}
 	```
+
+	This file will be refreshed upon _PATCH_ requests on this artifact
+	format if *DLREPO_POST_PROCESS_CMD* is set (see *dlrepo-config*(5))
+	since the command may have modified files.
+_.dirty_
+	Empty file created when a new file is uploaded to this format. If this
+	file is exists, _HEAD_ requests to this artifact format will return
+	a _404 Not found_ error (see *dlrepo-api*(7)). This file is deleted
+	after a _PATCH_ request is made on this format.
 _.internal_ (optional)
 	Empty file created when the artifact format is marked as "internal".
 	This flag is only informative.
 
 ## products/
 
 Contains one folder per product.
```

### Comparing `dlrepo-0.5/docs/dlrepo.7.scdoc` & `dlrepo-0.8/docs/dlrepo.7.scdoc`

 * *Files identical despite different names*

### Comparing `dlrepo-0.5/etc/default` & `dlrepo-0.8/etc/default`

 * *Files 18% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # dlrepo configuration see dlrepo-config(5)
 
 #DLREPO_ROOT_DIR=/var/lib/dlrepo
 #DLREPO_CHUNK_SIZE=262144
 #DLREPO_ORPHAN_BLOB_LIFETIME=600
 #DLREPO_LOG_LEVEL=WARNING
 #DLREPO_USER_QUOTA=10737418240
+#DLREPO_POST_PROCESS_CMD=
 #DLREPO_PUBLIC_URL=
 #DLREPO_TEMPLATES_DIR=
 #DLREPO_STATIC_DIR=
 #DLREPO_AUTH_REALM=dlrepo
 #DLREPO_AUTH_DISABLED=0
 #DLREPO_AUTH_FILE=/etc/dlrepo/auth
 #DLREPO_IGNORE_PASSWORDS=0
```

### Comparing `dlrepo-0.5/etc/dlrepo.service` & `dlrepo-0.8/etc/dlrepo.service`

 * *Files identical despite different names*

### Comparing `dlrepo-0.5/etc/nginx.conf` & `dlrepo-0.8/etc/nginx.conf`

 * *Files identical despite different names*

### Comparing `dlrepo-0.5/pylintrc` & `dlrepo-0.8/pylintrc`

 * *Files identical despite different names*

### Comparing `dlrepo-0.5/scss/components.scss` & `dlrepo-0.8/scss/components.scss`

 * *Files 5% similar despite different names*

```diff
@@ -34,25 +34,25 @@
 a.product {
   padding: $padding;
 }
 
 a.product > img {
   display: inline;
   margin-right: $padding / 2;
-  height: 2rem;
+  height: 1.8rem;
 }
 
 a.product-xl {
-  font-size: 1.2rem;
+  font-size: 1.1rem;
 }
 
 a.product-xl > img {
   display: inline;
   margin-right: $padding;
-  height: 3rem;
+  height: 2.4rem;
 }
 
 a.alias {
   font-style: italic;
   color: lighten($darkgray, 30%);
 }
```

### Comparing `dlrepo-0.5/scss/layout.scss` & `dlrepo-0.8/scss/layout.scss`

 * *Files identical despite different names*

### Comparing `dlrepo-0.5/scss/normalize.scss` & `dlrepo-0.8/scss/normalize.scss`

 * *Files identical despite different names*

### Comparing `dlrepo-0.5/scss/sections.scss` & `dlrepo-0.8/scss/sections.scss`

 * *Files 4% similar despite different names*

```diff
@@ -83,21 +83,27 @@
       border-width: 1px;
       border-radius: $padding;
       border-color: $lightgray;
       display: inline-block;
       padding: 2 * $padding;
       margin: $padding;
 
-      a.format {
+      a {
         display: block;
-        color: $primary;
       }
       a:hover {
         text-decoration: underline;
       }
+      a.format {
+        color: $primary;
+      }
+      a.digest {
+        color: $secondary;
+        font-style: italic;
+      }
     }
     > .artifact-format:hover {
       background-color: lighten($lightgray, 5%);
     }
   }
 
   > .whole-archive {
@@ -138,17 +144,18 @@
 
   .metadata:hover {
     background-color: lighten($lightgray, 5%);
   }
 }
 
 section.autoindex {
-  a {
-    display: block;
-  }
   a:hover {
     text-decoration: underline;
   }
   a.directory {
     color: $primary;
   }
+  a.digest {
+    color: $secondary;
+    font-style: italic;
+  }
 }
```

### Comparing `dlrepo-0.5/scss/variables.scss` & `dlrepo-0.8/scss/variables.scss`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 $secondary: #ff8552;
 $white: #fff;
 $lightgray: #e5e7eb;
 $darkgray: #374151;
 $released: #edffeb;
 $locked: #fffee8;
 $padding: 0.5rem;
-$width: 1200px;
+$width: 1400px;
 $banner_height: 5rem;
 $font_mono:
   ui-monospace,
   SFMono-Regular,
   Menlo,
   Monaco,
   Consolas,
```

### Comparing `dlrepo-0.5/setup.py` & `dlrepo-0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 setuptools.setup(
     name="dlrepo",
     description="Artifact repository",
     long_description=(pathlib.Path(__file__).parent / "README.md").read_text("utf-8"),
     long_description_content_type="text/markdown",
     license="BSD-3-Clause",
-    version="0.5",
+    version="0.8",
     author="Robin Jarry",
     author_email="robin@jarry.cc",
     install_requires=[
         "aiohttp",
         "aiohttp-jinja2",
         "cachetools",
         "bonsai",
```

### Comparing `dlrepo-0.5/tests/conftest.py` & `dlrepo-0.8/tests/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,19 +30,28 @@
     portnum = get_free_tcp_port()
     env = {
         "DLREPO_ROOT_DIR": str(temp_dir),
         "DLREPO_LISTEN_ADDRESS": "127.0.0.1",
         "DLREPO_LISTEN_PORT": str(portnum),
         "DLREPO_TEMPLATES_DIR": str(data_dir / "templates"),
         "DLREPO_STATIC_DIR": str(data_dir / "static"),
-        "DLREPO_ACLS_DIR": str(data_dir / "acls"),
-        "DLREPO_AUTH_FILE": str(data_dir / "auth"),
         "DLREPO_LOG_OUTPUT": "console",
         "DLREPO_LOG_LEVEL": "DEBUG",
     }
+    acls = data_dir / "acls"
+    if acls.is_dir():
+        env["DLREPO_ACLS_DIR"] = str(acls)
+    auth = data_dir / "auth"
+    if auth.is_file():
+        env["DLREPO_AUTH_FILE"] = str(auth)
+    else:
+        env["DLREPO_AUTH_DISABLED"] = "1"
+    post_process = data_dir / "post-process.sh"
+    if post_process.is_file():
+        env["DLREPO_POST_PROCESS_CMD"] = str(post_process)
     with subprocess.Popen([sys.executable, "-m", "dlrepo"], env=env) as proc:
         while proc.poll() is None:
             try:
                 with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
                     s.connect(("127.0.0.1", portnum))
                 break
             except socket.error:
```

### Comparing `dlrepo-0.5/tests/test_auth.py` & `dlrepo-0.8/tests/test_auth.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,14 +65,20 @@
         digest = hashlib.sha256(data).hexdigest()
         resp = await sess.put(
             "/branches/main/tag/job/format/file.txt",
             data=data,
             headers={"Digest": f"sha256:{digest}"},
         )
         assert resp.status == 201
+        resp = await sess.put(
+            "/branches/main/tag/job/format/file2.txt",
+            data=data + b"corrupt",
+            headers={"Digest": f"sha256:{digest}"},
+        )
+        assert resp.status == 422
 
 
 async def test_read_allowed(dlrepo_server):
     url, _ = dlrepo_server
     auth = aiohttp.BasicAuth("foo", "baz")
     async with aiohttp.ClientSession(url, auth=auth) as sess:
         resp = await sess.get("/branches/main/tag/job/format/file.txt")
```

