# Comparing `tmp/pydmt-0.1.79.tar.gz` & `tmp/pydmt-0.1.80.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydmt-0.1.79.tar", last modified: Fri Apr 21 14:50:53 2023, max compression
+gzip compressed data, was "pydmt-0.1.80.tar", last modified: Sun Apr 23 21:26:05 2023, max compression
```

## Comparing `pydmt-0.1.79.tar` & `pydmt-0.1.80.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-21 14:50:53.765725 pydmt-0.1.79/
--rw-rw-r--   0 mark      (1000) mark      (1000)     1069 2023-04-21 14:49:35.000000 pydmt-0.1.79/LICENSE
--rw-r--r--   0 mark      (1000) mark      (1000)     1364 2023-04-21 14:50:53.765725 pydmt-0.1.79/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      391 2023-04-21 14:49:35.000000 pydmt-0.1.79/README.rst
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-21 14:50:53.760725 pydmt-0.1.79/pydmt/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2017-12-02 11:42:36.000000 pydmt-0.1.79/pydmt/__init__.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-21 14:50:53.761725 pydmt-0.1.79/pydmt/api/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2017-12-02 11:42:36.000000 pydmt-0.1.79/pydmt/api/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)     4112 2022-07-01 10:06:39.000000 pydmt-0.1.79/pydmt/api/builder.py
--rw-r--r--   0 mark      (1000) mark      (1000)      179 2022-05-04 08:29:53.000000 pydmt-0.1.79/pydmt/api/copy.py
--rw-r--r--   0 mark      (1000) mark      (1000)      321 2022-05-04 08:30:05.000000 pydmt-0.1.79/pydmt/api/fail.py
--rw-r--r--   0 mark      (1000) mark      (1000)      613 2020-09-20 14:25:08.000000 pydmt-0.1.79/pydmt/api/feature.py
--rw-r--r--   0 mark      (1000) mark      (1000)      821 2022-07-01 10:05:31.000000 pydmt-0.1.79/pydmt/api/one_source_one_target.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-21 14:50:53.762725 pydmt-0.1.79/pydmt/builders/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2017-12-02 11:42:36.000000 pydmt-0.1.79/pydmt/builders/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1381 2022-10-12 19:15:22.000000 pydmt-0.1.79/pydmt/builders/apt.py
--rw-r--r--   0 mark      (1000) mark      (1000)      428 2023-04-21 14:45:52.000000 pydmt-0.1.79/pydmt/builders/make.py
--rw-r--r--   0 mark      (1000) mark      (1000)     2978 2022-07-01 10:04:42.000000 pydmt-0.1.79/pydmt/builders/mako.py
--rw-r--r--   0 mark      (1000) mark      (1000)      493 2022-07-01 09:58:33.000000 pydmt-0.1.79/pydmt/builders/npm.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1390 2022-10-15 00:29:42.000000 pydmt-0.1.79/pydmt/builders/reqs.py
--rw-r--r--   0 mark      (1000) mark      (1000)     4170 2022-10-15 12:44:01.000000 pydmt-0.1.79/pydmt/builders/sphinx.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1524 2023-04-21 14:45:15.000000 pydmt-0.1.79/pydmt/builders/venv.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1584 2023-04-21 14:45:35.000000 pydmt-0.1.79/pydmt/builders/venv_full.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1276 2022-10-11 06:48:27.000000 pydmt-0.1.79/pydmt/builders/yaml.py
--rw-r--r--   0 mark      (1000) mark      (1000)     2230 2022-06-25 07:24:09.000000 pydmt-0.1.79/pydmt/configs.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-21 14:50:53.763725 pydmt-0.1.79/pydmt/core/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2017-12-02 11:42:36.000000 pydmt-0.1.79/pydmt/core/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)     2755 2022-05-25 15:17:23.000000 pydmt-0.1.79/pydmt/core/cache.py
--rw-r--r--   0 mark      (1000) mark      (1000)       50 2020-06-19 19:56:59.000000 pydmt-0.1.79/pydmt/core/graph.py
--rw-r--r--   0 mark      (1000) mark      (1000)     5744 2022-07-01 10:15:48.000000 pydmt-0.1.79/pydmt/core/pydmt.py
--rw-r--r--   0 mark      (1000) mark      (1000)      491 2017-12-02 11:42:36.000000 pydmt-0.1.79/pydmt/core/tempdir.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-21 14:50:53.763725 pydmt-0.1.79/pydmt/features/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2017-12-02 11:42:36.000000 pydmt-0.1.79/pydmt/features/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)      518 2022-07-01 09:55:35.000000 pydmt-0.1.79/pydmt/features/apt.py
--rw-r--r--   0 mark      (1000) mark      (1000)      374 2022-05-09 23:30:17.000000 pydmt-0.1.79/pydmt/features/make.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1422 2022-05-04 08:25:10.000000 pydmt-0.1.79/pydmt/features/mako.py
--rw-r--r--   0 mark      (1000) mark      (1000)      380 2022-05-04 08:20:12.000000 pydmt-0.1.79/pydmt/features/npm.py
--rw-r--r--   0 mark      (1000) mark      (1000)      469 2022-05-05 02:02:20.000000 pydmt-0.1.79/pydmt/features/reqs.py
--rw-r--r--   0 mark      (1000) mark      (1000)      340 2022-05-18 11:32:53.000000 pydmt-0.1.79/pydmt/features/sphinx.py
--rw-r--r--   0 mark      (1000) mark      (1000)      392 2022-05-09 05:06:11.000000 pydmt-0.1.79/pydmt/features/venv.py
--rw-r--r--   0 mark      (1000) mark      (1000)      325 2022-05-09 04:57:20.000000 pydmt-0.1.79/pydmt/features/venv_full.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1010 2022-05-04 08:23:35.000000 pydmt-0.1.79/pydmt/features/yaml.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-21 14:50:53.764725 pydmt-0.1.79/pydmt/helpers/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2020-05-31 02:02:11.000000 pydmt-0.1.79/pydmt/helpers/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)      823 2022-06-25 06:57:04.000000 pydmt-0.1.79/pydmt/helpers/apt.py
--rw-r--r--   0 mark      (1000) mark      (1000)      129 2022-05-16 19:51:40.000000 pydmt-0.1.79/pydmt/helpers/composites.py
--rw-r--r--   0 mark      (1000) mark      (1000)      959 2022-05-18 14:23:43.000000 pydmt-0.1.79/pydmt/helpers/deb.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1022 2022-05-18 18:42:27.000000 pydmt-0.1.79/pydmt/helpers/deb_python_package.py
--rw-r--r--   0 mark      (1000) mark      (1000)      314 2022-05-29 13:25:55.000000 pydmt-0.1.79/pydmt/helpers/files.py
--rw-r--r--   0 mark      (1000) mark      (1000)      198 2022-05-16 01:59:39.000000 pydmt-0.1.79/pydmt/helpers/general.py
--rw-r--r--   0 mark      (1000) mark      (1000)      313 2022-06-25 06:56:24.000000 pydmt-0.1.79/pydmt/helpers/git.py
--rw-r--r--   0 mark      (1000) mark      (1000)      465 2022-05-19 21:23:46.000000 pydmt-0.1.79/pydmt/helpers/github.py
--rw-r--r--   0 mark      (1000) mark      (1000)       72 2022-05-15 16:42:20.000000 pydmt-0.1.79/pydmt/helpers/messages.py
--rw-r--r--   0 mark      (1000) mark      (1000)      165 2022-10-15 00:39:08.000000 pydmt-0.1.79/pydmt/helpers/misc.py
--rw-r--r--   0 mark      (1000) mark      (1000)      269 2022-05-19 21:19:00.000000 pydmt-0.1.79/pydmt/helpers/pkgs.py
--rw-r--r--   0 mark      (1000) mark      (1000)      218 2022-05-18 18:52:21.000000 pydmt-0.1.79/pydmt/helpers/project.py
--rw-r--r--   0 mark      (1000) mark      (1000)     4895 2023-03-08 23:18:25.000000 pydmt-0.1.79/pydmt/helpers/python.py
--rw-r--r--   0 mark      (1000) mark      (1000)      775 2022-05-19 21:09:23.000000 pydmt-0.1.79/pydmt/helpers/signature.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1150 2022-05-16 02:02:20.000000 pydmt-0.1.79/pydmt/helpers/snipplets.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1333 2022-10-12 19:19:30.000000 pydmt-0.1.79/pydmt/helpers/urls.py
--rw-r--r--   0 mark      (1000) mark      (1000)     4961 2022-10-14 23:14:11.000000 pydmt-0.1.79/pydmt/main.py
--rw-r--r--   0 mark      (1000) mark      (1000)      175 2023-04-21 14:49:47.000000 pydmt-0.1.79/pydmt/static.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-21 14:50:53.765725 pydmt-0.1.79/pydmt/utils/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2017-12-02 11:42:36.000000 pydmt-0.1.79/pydmt/utils/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1174 2022-07-01 10:02:49.000000 pydmt-0.1.79/pydmt/utils/digest.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1044 2021-09-07 01:45:29.000000 pydmt-0.1.79/pydmt/utils/digester.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1244 2021-09-14 23:18:59.000000 pydmt-0.1.79/pydmt/utils/filesystem.py
--rw-r--r--   0 mark      (1000) mark      (1000)      178 2022-05-25 15:06:52.000000 pydmt-0.1.79/pydmt/utils/logging.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      265 2021-09-16 23:27:43.000000 pydmt-0.1.79/pydmt/utils/php.py
--rw-r--r--   0 mark      (1000) mark      (1000)     2822 2022-10-15 00:35:27.000000 pydmt-0.1.79/pydmt/utils/python.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1337 2023-04-21 14:48:53.000000 pydmt-0.1.79/pydmt/utils/subprocess.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-21 14:50:53.761725 pydmt-0.1.79/pydmt.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)     1364 2023-04-21 14:50:53.000000 pydmt-0.1.79/pydmt.egg-info/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)     1602 2023-04-21 14:50:53.000000 pydmt-0.1.79/pydmt.egg-info/SOURCES.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        1 2023-04-21 14:50:53.000000 pydmt-0.1.79/pydmt.egg-info/dependency_links.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       42 2023-04-21 14:50:53.000000 pydmt-0.1.79/pydmt.egg-info/entry_points.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       77 2023-04-21 14:50:53.000000 pydmt-0.1.79/pydmt.egg-info/requires.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        6 2023-04-21 14:50:53.000000 pydmt-0.1.79/pydmt.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       67 2023-04-21 14:50:53.765725 pydmt-0.1.79/setup.cfg
--rw-r--r--   0 mark      (1000) mark      (1000)     1859 2023-04-21 14:49:47.000000 pydmt-0.1.79/setup.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-23 21:26:05.710924 pydmt-0.1.80/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1069 2023-04-23 21:25:33.000000 pydmt-0.1.80/LICENSE
+-rw-r--r--   0 mark      (1000) mark      (1000)     1364 2023-04-23 21:26:05.710924 pydmt-0.1.80/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      391 2023-04-23 21:25:54.000000 pydmt-0.1.80/README.rst
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-23 21:26:05.705924 pydmt-0.1.80/pydmt/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2017-12-02 11:42:36.000000 pydmt-0.1.80/pydmt/__init__.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-23 21:26:05.706924 pydmt-0.1.80/pydmt/api/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2017-12-02 11:42:36.000000 pydmt-0.1.80/pydmt/api/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     4112 2022-07-01 10:06:39.000000 pydmt-0.1.80/pydmt/api/builder.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      179 2022-05-04 08:29:53.000000 pydmt-0.1.80/pydmt/api/copy.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      321 2022-05-04 08:30:05.000000 pydmt-0.1.80/pydmt/api/fail.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      613 2020-09-20 14:25:08.000000 pydmt-0.1.80/pydmt/api/feature.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      821 2022-07-01 10:05:31.000000 pydmt-0.1.80/pydmt/api/one_source_one_target.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-23 21:26:05.707924 pydmt-0.1.80/pydmt/builders/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2017-12-02 11:42:36.000000 pydmt-0.1.80/pydmt/builders/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1381 2022-10-12 19:15:22.000000 pydmt-0.1.80/pydmt/builders/apt.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      428 2023-04-21 14:45:52.000000 pydmt-0.1.80/pydmt/builders/make.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     2978 2022-07-01 10:04:42.000000 pydmt-0.1.80/pydmt/builders/mako.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      493 2022-07-01 09:58:33.000000 pydmt-0.1.80/pydmt/builders/npm.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1390 2022-10-15 00:29:42.000000 pydmt-0.1.80/pydmt/builders/reqs.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     4170 2022-10-15 12:44:01.000000 pydmt-0.1.80/pydmt/builders/sphinx.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1524 2023-04-21 14:45:15.000000 pydmt-0.1.80/pydmt/builders/venv.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1584 2023-04-21 14:45:35.000000 pydmt-0.1.80/pydmt/builders/venv_full.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1276 2022-10-11 06:48:27.000000 pydmt-0.1.80/pydmt/builders/yaml.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     2230 2022-06-25 07:24:09.000000 pydmt-0.1.80/pydmt/configs.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-23 21:26:05.707924 pydmt-0.1.80/pydmt/core/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2017-12-02 11:42:36.000000 pydmt-0.1.80/pydmt/core/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     2755 2022-05-25 15:17:23.000000 pydmt-0.1.80/pydmt/core/cache.py
+-rw-r--r--   0 mark      (1000) mark      (1000)       50 2020-06-19 19:56:59.000000 pydmt-0.1.80/pydmt/core/graph.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     5744 2022-07-01 10:15:48.000000 pydmt-0.1.80/pydmt/core/pydmt.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      491 2017-12-02 11:42:36.000000 pydmt-0.1.80/pydmt/core/tempdir.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-23 21:26:05.708924 pydmt-0.1.80/pydmt/features/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2017-12-02 11:42:36.000000 pydmt-0.1.80/pydmt/features/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      518 2022-07-01 09:55:35.000000 pydmt-0.1.80/pydmt/features/apt.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      374 2022-05-09 23:30:17.000000 pydmt-0.1.80/pydmt/features/make.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1422 2022-05-04 08:25:10.000000 pydmt-0.1.80/pydmt/features/mako.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      380 2022-05-04 08:20:12.000000 pydmt-0.1.80/pydmt/features/npm.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      469 2022-05-05 02:02:20.000000 pydmt-0.1.80/pydmt/features/reqs.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      340 2022-05-18 11:32:53.000000 pydmt-0.1.80/pydmt/features/sphinx.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      392 2022-05-09 05:06:11.000000 pydmt-0.1.80/pydmt/features/venv.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      325 2022-05-09 04:57:20.000000 pydmt-0.1.80/pydmt/features/venv_full.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1010 2022-05-04 08:23:35.000000 pydmt-0.1.80/pydmt/features/yaml.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-23 21:26:05.709924 pydmt-0.1.80/pydmt/helpers/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2020-05-31 02:02:11.000000 pydmt-0.1.80/pydmt/helpers/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      823 2022-06-25 06:57:04.000000 pydmt-0.1.80/pydmt/helpers/apt.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      129 2022-05-16 19:51:40.000000 pydmt-0.1.80/pydmt/helpers/composites.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      959 2022-05-18 14:23:43.000000 pydmt-0.1.80/pydmt/helpers/deb.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1022 2022-05-18 18:42:27.000000 pydmt-0.1.80/pydmt/helpers/deb_python_package.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      314 2022-05-29 13:25:55.000000 pydmt-0.1.80/pydmt/helpers/files.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      198 2022-05-16 01:59:39.000000 pydmt-0.1.80/pydmt/helpers/general.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      313 2022-06-25 06:56:24.000000 pydmt-0.1.80/pydmt/helpers/git.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      465 2022-05-19 21:23:46.000000 pydmt-0.1.80/pydmt/helpers/github.py
+-rw-r--r--   0 mark      (1000) mark      (1000)       72 2022-05-15 16:42:20.000000 pydmt-0.1.80/pydmt/helpers/messages.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      165 2022-10-15 00:39:08.000000 pydmt-0.1.80/pydmt/helpers/misc.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      269 2022-05-19 21:19:00.000000 pydmt-0.1.80/pydmt/helpers/pkgs.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      218 2022-05-18 18:52:21.000000 pydmt-0.1.80/pydmt/helpers/project.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     4895 2023-03-08 23:18:25.000000 pydmt-0.1.80/pydmt/helpers/python.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      775 2022-05-19 21:09:23.000000 pydmt-0.1.80/pydmt/helpers/signature.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1150 2022-05-16 02:02:20.000000 pydmt-0.1.80/pydmt/helpers/snipplets.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1333 2022-10-12 19:19:30.000000 pydmt-0.1.80/pydmt/helpers/urls.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     4961 2022-10-14 23:14:11.000000 pydmt-0.1.80/pydmt/main.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      175 2023-04-23 21:25:54.000000 pydmt-0.1.80/pydmt/static.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-23 21:26:05.709924 pydmt-0.1.80/pydmt/utils/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2017-12-02 11:42:36.000000 pydmt-0.1.80/pydmt/utils/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1174 2022-07-01 10:02:49.000000 pydmt-0.1.80/pydmt/utils/digest.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1044 2021-09-07 01:45:29.000000 pydmt-0.1.80/pydmt/utils/digester.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1244 2021-09-14 23:18:59.000000 pydmt-0.1.80/pydmt/utils/filesystem.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      178 2022-05-25 15:06:52.000000 pydmt-0.1.80/pydmt/utils/logging.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      265 2021-09-16 23:27:43.000000 pydmt-0.1.80/pydmt/utils/php.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     2822 2022-10-15 00:35:27.000000 pydmt-0.1.80/pydmt/utils/python.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1337 2023-04-21 14:48:53.000000 pydmt-0.1.80/pydmt/utils/subprocess.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-23 21:26:05.706924 pydmt-0.1.80/pydmt.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)     1364 2023-04-23 21:26:05.000000 pydmt-0.1.80/pydmt.egg-info/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)     1602 2023-04-23 21:26:05.000000 pydmt-0.1.80/pydmt.egg-info/SOURCES.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        1 2023-04-23 21:26:05.000000 pydmt-0.1.80/pydmt.egg-info/dependency_links.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       42 2023-04-23 21:26:05.000000 pydmt-0.1.80/pydmt.egg-info/entry_points.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       77 2023-04-23 21:26:05.000000 pydmt-0.1.80/pydmt.egg-info/requires.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        6 2023-04-23 21:26:05.000000 pydmt-0.1.80/pydmt.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       67 2023-04-23 21:26:05.710924 pydmt-0.1.80/setup.cfg
+-rw-r--r--   0 mark      (1000) mark      (1000)     1859 2023-04-23 21:25:54.000000 pydmt-0.1.80/setup.py
```

### Comparing `pydmt-0.1.79/LICENSE` & `pydmt-0.1.80/LICENSE`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.79/PKG-INFO` & `pydmt-0.1.80/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pydmt
-Version: 0.1.79
-Summary: python dependency management tool
+Version: 0.1.80
+Summary: Python dependency management tool
 Home-page: https://veltzer.github.io/pydmt
 Download-URL: https://github.com/veltzer/pydmt
 Author: Mark Veltzer
 Author-email: mark.veltzer@gmail.com
 Maintainer: Mark Veltzer
 Maintainer-email: mark.veltzer@gmail.com
 License: MIT
@@ -35,10 +35,10 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
 
 project website: https://veltzer.github.io/pydmt
 
 author: Mark Veltzer
 
-version: 0.1.79
+version: 0.1.80
 
 	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2017, 2018, 2019, 2020, 2021, 2022, 2023
```

### Comparing `pydmt-0.1.79/pydmt/api/builder.py` & `pydmt-0.1.80/pydmt/api/builder.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.79/pydmt/api/feature.py` & `pydmt-0.1.80/pydmt/api/feature.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.79/pydmt/api/one_source_one_target.py` & `pydmt-0.1.80/pydmt/api/one_source_one_target.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.79/pydmt/builders/apt.py` & `pydmt-0.1.80/pydmt/builders/apt.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.79/pydmt/builders/mako.py` & `pydmt-0.1.80/pydmt/builders/mako.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.79/pydmt/builders/reqs.py` & `pydmt-0.1.80/pydmt/builders/reqs.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.79/pydmt/builders/sphinx.py` & `pydmt-0.1.80/pydmt/builders/sphinx.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.79/pydmt/builders/venv.py` & `pydmt-0.1.80/pydmt/builders/venv.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.79/pydmt/builders/venv_full.py` & `pydmt-0.1.80/pydmt/builders/venv_full.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.79/pydmt/builders/yaml.py` & `pydmt-0.1.80/pydmt/builders/yaml.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.79/pydmt/configs.py` & `pydmt-0.1.80/pydmt/configs.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.79/pydmt/core/cache.py` & `pydmt-0.1.80/pydmt/core/cache.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.79/pydmt/core/pydmt.py` & `pydmt-0.1.80/pydmt/core/pydmt.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.79/pydmt/features/apt.py` & `pydmt-0.1.80/pydmt/features/apt.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.79/pydmt/features/mako.py` & `pydmt-0.1.80/pydmt/features/mako.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.79/pydmt/features/yaml.py` & `pydmt-0.1.80/pydmt/features/yaml.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.79/pydmt/helpers/apt.py` & `pydmt-0.1.80/pydmt/helpers/apt.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.79/pydmt/helpers/deb.py` & `pydmt-0.1.80/pydmt/helpers/deb.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.79/pydmt/helpers/deb_python_package.py` & `pydmt-0.1.80/pydmt/helpers/deb_python_package.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.79/pydmt/helpers/python.py` & `pydmt-0.1.80/pydmt/helpers/python.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.79/pydmt/helpers/signature.py` & `pydmt-0.1.80/pydmt/helpers/signature.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.79/pydmt/helpers/snipplets.py` & `pydmt-0.1.80/pydmt/helpers/snipplets.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.79/pydmt/helpers/urls.py` & `pydmt-0.1.80/pydmt/helpers/urls.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.79/pydmt/main.py` & `pydmt-0.1.80/pydmt/main.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.79/pydmt/utils/digest.py` & `pydmt-0.1.80/pydmt/utils/digest.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.79/pydmt/utils/digester.py` & `pydmt-0.1.80/pydmt/utils/digester.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.79/pydmt/utils/filesystem.py` & `pydmt-0.1.80/pydmt/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.79/pydmt/utils/python.py` & `pydmt-0.1.80/pydmt/utils/python.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.79/pydmt/utils/subprocess.py` & `pydmt-0.1.80/pydmt/utils/subprocess.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.79/pydmt.egg-info/PKG-INFO` & `pydmt-0.1.80/pydmt.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pydmt
-Version: 0.1.79
-Summary: python dependency management tool
+Version: 0.1.80
+Summary: Python dependency management tool
 Home-page: https://veltzer.github.io/pydmt
 Download-URL: https://github.com/veltzer/pydmt
 Author: Mark Veltzer
 Author-email: mark.veltzer@gmail.com
 Maintainer: Mark Veltzer
 Maintainer-email: mark.veltzer@gmail.com
 License: MIT
@@ -35,10 +35,10 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
 
 project website: https://veltzer.github.io/pydmt
 
 author: Mark Veltzer
 
-version: 0.1.79
+version: 0.1.80
 
 	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2017, 2018, 2019, 2020, 2021, 2022, 2023
```

### Comparing `pydmt-0.1.79/pydmt.egg-info/SOURCES.txt` & `pydmt-0.1.80/pydmt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.79/setup.py` & `pydmt-0.1.80/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,26 +5,26 @@
     with open('README.rst') as f:
         return f.read()
 
 
 setuptools.setup(
     # the first three fields are a must according to the documentation
     name="pydmt",
-    version="0.1.79",
+    version="0.1.80",
     packages=[
         "pydmt",
         "pydmt.api",
         "pydmt.builders",
         "pydmt.core",
         "pydmt.features",
         "pydmt.helpers",
         "pydmt.utils",
     ],
     # from here all is optional
-    description="python dependency management tool",
+    description="Python dependency management tool",
     long_description=get_readme(),
     long_description_content_type="text/x-rst",
     author="Mark Veltzer",
     author_email="mark.veltzer@gmail.com",
     maintainer="Mark Veltzer",
     maintainer_email="mark.veltzer@gmail.com",
     keywords=[
```

