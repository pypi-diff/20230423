# Comparing `tmp/openxlab-0.0.1.tar.gz` & `tmp/openxlab-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openxlab-0.0.1.tar", last modified: Thu Mar 23 03:47:55 2023, max compression
+gzip compressed data, was "openxlab-0.0.2.tar", last modified: Sun Apr 23 02:04:37 2023, max compression
```

## Comparing `openxlab-0.0.1.tar` & `openxlab-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,59 @@
-drwxr-xr-x   0 huwenxing (200000610) huwenxing (200000610)        0 2023-03-23 03:47:55.000000 openxlab-0.0.1/
--rw-r--r--   0 huwenxing (200000610) huwenxing (200000610)    11357 2023-03-23 03:35:20.000000 openxlab-0.0.1/LICENSE
--rw-r--r--   0 huwenxing (200000610) huwenxing (200000610)     1133 2023-03-23 03:47:55.000000 openxlab-0.0.1/PKG-INFO
--rw-------   0 huwenxing (200000610) huwenxing (200000610)      368 2023-03-23 03:35:24.000000 openxlab-0.0.1/README.md
-drwxr-xr-x   0 huwenxing (200000610) huwenxing (200000610)        0 2023-03-23 03:47:55.000000 openxlab-0.0.1/mmstat/
--rw-r--r--   0 huwenxing (200000610) huwenxing (200000610)        0 2023-03-23 03:35:20.000000 openxlab-0.0.1/mmstat/__init__.py
--rw-r--r--   0 huwenxing (200000610) huwenxing (200000610)      700 2023-03-23 03:35:20.000000 openxlab-0.0.1/mmstat/version.py
-drwxr-xr-x   0 huwenxing (200000610) huwenxing (200000610)        0 2023-03-23 03:47:55.000000 openxlab-0.0.1/openxlab.egg-info/
--rw-r--r--   0 huwenxing (200000610) huwenxing (200000610)     1133 2023-03-23 03:47:54.000000 openxlab-0.0.1/openxlab.egg-info/PKG-INFO
--rw-r--r--   0 huwenxing (200000610) huwenxing (200000610)      222 2023-03-23 03:47:55.000000 openxlab-0.0.1/openxlab.egg-info/SOURCES.txt
--rw-r--r--   0 huwenxing (200000610) huwenxing (200000610)        1 2023-03-23 03:47:54.000000 openxlab-0.0.1/openxlab.egg-info/dependency_links.txt
--rw-r--r--   0 huwenxing (200000610) huwenxing (200000610)        8 2023-03-23 03:47:54.000000 openxlab-0.0.1/openxlab.egg-info/requires.txt
--rw-r--r--   0 huwenxing (200000610) huwenxing (200000610)        7 2023-03-23 03:47:55.000000 openxlab-0.0.1/openxlab.egg-info/top_level.txt
--rw-r--r--   0 huwenxing (200000610) huwenxing (200000610)       38 2023-03-23 03:47:55.000000 openxlab-0.0.1/setup.cfg
--rw-r--r--   0 huwenxing (200000610) huwenxing (200000610)     5124 2023-03-23 03:36:13.000000 openxlab-0.0.1/setup.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-23 02:04:37.274855 openxlab-0.0.2/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1434 2023-04-23 02:04:37.274516 openxlab-0.0.2/PKG-INFO
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1036 2023-04-10 10:02:47.000000 openxlab-0.0.2/README.md
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-23 02:04:37.258949 openxlab-0.0.2/openxlab/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       46 2023-04-10 09:49:22.000000 openxlab-0.0.2/openxlab/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     3138 2023-04-14 09:07:13.000000 openxlab-0.0.2/openxlab/cli.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-23 02:04:37.262584 openxlab-0.0.2/openxlab/config/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-10 09:49:22.000000 openxlab-0.0.2/openxlab/config/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       65 2023-04-23 01:54:21.000000 openxlab-0.0.2/openxlab/config/version.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-23 02:04:37.263016 openxlab-0.0.2/openxlab/demo_cmd/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1076 2023-04-10 10:02:47.000000 openxlab-0.0.2/openxlab/demo_cmd/__init__.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-23 02:04:37.263514 openxlab-0.0.2/openxlab/model/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        7 2023-04-14 08:49:35.000000 openxlab-0.0.2/openxlab/model/__init__.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-23 02:04:37.264392 openxlab-0.0.2/openxlab/model/clients/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-16 03:36:45.000000 openxlab-0.0.2/openxlab/model/clients/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-16 03:45:30.000000 openxlab-0.0.2/openxlab/model/clients/model_client.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     2473 2023-04-20 11:54:06.000000 openxlab-0.0.2/openxlab/model/clients/openapi_client.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-23 02:04:37.267373 openxlab-0.0.2/openxlab/model/commands/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      695 2023-04-14 09:21:09.000000 openxlab-0.0.2/openxlab/model/commands/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      365 2023-04-14 09:06:08.000000 openxlab-0.0.2/openxlab/model/commands/create.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      770 2023-04-18 03:48:11.000000 openxlab-0.0.2/openxlab/model/commands/download.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      365 2023-04-14 09:06:08.000000 openxlab-0.0.2/openxlab/model/commands/inference.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      422 2023-04-18 03:48:11.000000 openxlab-0.0.2/openxlab/model/commands/init.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      358 2023-04-14 09:06:08.000000 openxlab-0.0.2/openxlab/model/commands/list.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      366 2023-04-14 09:06:08.000000 openxlab-0.0.2/openxlab/model/commands/remove.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      390 2023-04-14 09:06:08.000000 openxlab-0.0.2/openxlab/model/commands/upload.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      390 2023-04-14 09:06:08.000000 openxlab-0.0.2/openxlab/model/commands/visibility.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-23 02:04:37.268437 openxlab-0.0.2/openxlab/model/common/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-13 09:38:02.000000 openxlab-0.0.2/openxlab/model/common/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      898 2023-04-23 01:59:35.000000 openxlab-0.0.2/openxlab/model/common/constants.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      831 2023-04-14 05:07:06.000000 openxlab-0.0.2/openxlab/model/common/response_dto.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-23 02:04:37.272263 openxlab-0.0.2/openxlab/model/handler/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      111 2023-04-18 03:48:11.000000 openxlab-0.0.2/openxlab/model/handler/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-13 02:48:29.000000 openxlab-0.0.2/openxlab/model/handler/common.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       26 2023-04-13 03:08:33.000000 openxlab-0.0.2/openxlab/model/handler/create_repository.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     2842 2023-04-20 11:36:51.000000 openxlab-0.0.2/openxlab/model/handler/download_file.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       26 2023-04-13 03:08:33.000000 openxlab-0.0.2/openxlab/model/handler/model_inference.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       26 2023-04-13 03:08:33.000000 openxlab-0.0.2/openxlab/model/handler/model_list.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       29 2023-04-13 03:08:33.000000 openxlab-0.0.2/openxlab/model/handler/query_meta_info.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       41 2023-04-13 03:08:33.000000 openxlab-0.0.2/openxlab/model/handler/remove_repo_or_file.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       32 2023-04-13 03:08:33.000000 openxlab-0.0.2/openxlab/model/handler/update_file.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-23 02:04:37.272798 openxlab-0.0.2/openxlab/types/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-10 11:25:41.000000 openxlab-0.0.2/openxlab/types/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      951 2023-04-10 10:02:47.000000 openxlab-0.0.2/openxlab/types/command_type.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-23 02:04:37.273560 openxlab-0.0.2/openxlab/utils/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       20 2023-04-10 10:02:47.000000 openxlab-0.0.2/openxlab/utils/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     3118 2023-04-10 10:02:47.000000 openxlab-0.0.2/openxlab/utils/file.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-23 02:04:37.274062 openxlab-0.0.2/openxlab/xlab/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      418 2023-04-10 10:02:47.000000 openxlab-0.0.2/openxlab/xlab/__init__.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-23 02:04:37.261724 openxlab-0.0.2/openxlab.egg-info/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1434 2023-04-23 02:04:37.000000 openxlab-0.0.2/openxlab.egg-info/PKG-INFO
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1402 2023-04-23 02:04:37.000000 openxlab-0.0.2/openxlab.egg-info/SOURCES.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        1 2023-04-23 02:04:37.000000 openxlab-0.0.2/openxlab.egg-info/dependency_links.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       48 2023-04-23 02:04:37.000000 openxlab-0.0.2/openxlab.egg-info/entry_points.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       79 2023-04-23 02:04:37.000000 openxlab-0.0.2/openxlab.egg-info/requires.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        9 2023-04-23 02:04:37.000000 openxlab-0.0.2/openxlab.egg-info/top_level.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      283 2023-04-10 10:02:47.000000 openxlab-0.0.2/pyproject.toml
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       38 2023-04-23 02:04:37.275002 openxlab-0.0.2/setup.cfg
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1173 2023-04-23 01:59:14.000000 openxlab-0.0.2/setup.py
```

