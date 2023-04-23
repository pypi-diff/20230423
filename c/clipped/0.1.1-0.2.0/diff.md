# Comparing `tmp/clipped-0.1.1.tar.gz` & `tmp/clipped-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clipped-0.1.1.tar", last modified: Sun Apr 16 10:41:37 2023, max compression
+gzip compressed data, was "clipped-0.2.0.tar", last modified: Sun Apr 23 10:34:51 2023, max compression
```

## Comparing `clipped-0.1.1.tar` & `clipped-0.2.0.tar`

### file list

```diff
@@ -1,79 +1,80 @@
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-16 10:41:37.724623 clipped-0.1.1/
--rw-r--r--   0 mourad     (501) staff       (20)      174 2023-04-16 10:40:33.000000 clipped-0.1.1/MANIFEST.in
--rw-r--r--   0 mourad     (501) staff       (20)     2012 2023-04-16 10:41:37.724722 clipped-0.1.1/PKG-INFO
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-16 10:41:37.714692 clipped-0.1.1/clipped/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/__init__.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-16 10:41:37.716468 clipped-0.1.1/clipped/config/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/config/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)       91 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/config/constants.py
--rw-r--r--   0 mourad     (501) staff       (20)       40 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/config/exceptions.py
--rw-r--r--   0 mourad     (501) staff       (20)     4022 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/config/manager.py
--rw-r--r--   0 mourad     (501) staff       (20)     6164 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/config/parser.py
--rw-r--r--   0 mourad     (501) staff       (20)      527 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/config/patch_strategy.py
--rw-r--r--   0 mourad     (501) staff       (20)    14928 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/config/schema.py
--rw-r--r--   0 mourad     (501) staff       (20)     8892 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/config/spec.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-16 10:41:37.717209 clipped-0.1.1/clipped/decorators/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/decorators/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)      646 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/decorators/cached_property.py
--rw-r--r--   0 mourad     (501) staff       (20)     4355 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/decorators/deprecation.py
--rw-r--r--   0 mourad     (501) staff       (20)     1923 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/decorators/memoization.py
--rw-r--r--   0 mourad     (501) staff       (20)     2686 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/decorators/signals.py
--rw-r--r--   0 mourad     (501) staff       (20)     6256 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/formatting.py
--rw-r--r--   0 mourad     (501) staff       (20)      824 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/manager_interface.py
--rw-r--r--   0 mourad     (501) staff       (20)      203 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/pkg.py
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/py.typed
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-16 10:41:37.718868 clipped-0.1.1/clipped/types/
--rw-r--r--   0 mourad     (501) staff       (20)     3748 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/types/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     1298 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/types/docker_image.py
--rw-r--r--   0 mourad     (501) staff       (20)     1889 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/types/email.py
--rw-r--r--   0 mourad     (501) staff       (20)     1033 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/types/gcs.py
--rw-r--r--   0 mourad     (501) staff       (20)      693 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/types/lists.py
--rw-r--r--   0 mourad     (501) staff       (20)      158 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/types/numbers.py
--rw-r--r--   0 mourad     (501) staff       (20)     1142 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/types/ref_or_obj.py
--rw-r--r--   0 mourad     (501) staff       (20)     1019 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/types/s3.py
--rw-r--r--   0 mourad     (501) staff       (20)     1265 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/types/uri.py
--rw-r--r--   0 mourad     (501) staff       (20)      683 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/types/uuids.py
--rw-r--r--   0 mourad     (501) staff       (20)     3179 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/types/wasb.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-16 10:41:37.724471 clipped-0.1.1/clipped/utils/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     1004 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/bools.py
--rw-r--r--   0 mourad     (501) staff       (20)      143 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/click.py
--rw-r--r--   0 mourad     (501) staff       (20)      665 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/cmd.py
--rw-r--r--   0 mourad     (501) staff       (20)      570 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/coroutine.py
--rw-r--r--   0 mourad     (501) staff       (20)      755 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/csv.py
--rw-r--r--   0 mourad     (501) staff       (20)     7568 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/dates.py
--rw-r--r--   0 mourad     (501) staff       (20)     3354 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/dicts.py
--rw-r--r--   0 mourad     (501) staff       (20)      496 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/encoding.py
--rw-r--r--   0 mourad     (501) staff       (20)     1093 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/enums.py
--rw-r--r--   0 mourad     (501) staff       (20)     2001 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/env.py
--rw-r--r--   0 mourad     (501) staff       (20)     4737 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/git.py
--rw-r--r--   0 mourad     (501) staff       (20)     1827 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/hashing.py
--rw-r--r--   0 mourad     (501) staff       (20)     1175 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/http.py
--rw-r--r--   0 mourad     (501) staff       (20)     3363 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/humanize.py
--rw-r--r--   0 mourad     (501) staff       (20)     1327 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/imports.py
--rw-r--r--   0 mourad     (501) staff       (20)     1695 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/indentation.py
--rw-r--r--   0 mourad     (501) staff       (20)      420 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/json.py
--rw-r--r--   0 mourad     (501) staff       (20)     1163 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/lists.py
--rw-r--r--   0 mourad     (501) staff       (20)      113 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/logging.py
--rw-r--r--   0 mourad     (501) staff       (20)     1280 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/np.py
--rw-r--r--   0 mourad     (501) staff       (20)     8484 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/paths.py
--rw-r--r--   0 mourad     (501) staff       (20)      674 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/query_params.py
--rw-r--r--   0 mourad     (501) staff       (20)     1134 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/requests.py
--rw-r--r--   0 mourad     (501) staff       (20)     1041 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/responses.py
--rw-r--r--   0 mourad     (501) staff       (20)      595 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/sanitizers.py
--rw-r--r--   0 mourad     (501) staff       (20)      676 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/serialization.py
--rw-r--r--   0 mourad     (501) staff       (20)     2674 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/strings.py
--rw-r--r--   0 mourad     (501) staff       (20)     1115 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/tz.py
--rw-r--r--   0 mourad     (501) staff       (20)     4040 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/units.py
--rw-r--r--   0 mourad     (501) staff       (20)      269 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/urls.py
--rw-r--r--   0 mourad     (501) staff       (20)      614 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/validation.py
--rw-r--r--   0 mourad     (501) staff       (20)     1128 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/versions.py
--rw-r--r--   0 mourad     (501) staff       (20)     1068 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/workers.py
--rw-r--r--   0 mourad     (501) staff       (20)      546 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/yaml.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-16 10:41:37.715278 clipped-0.1.1/clipped.egg-info/
--rw-r--r--   0 mourad     (501) staff       (20)     2012 2023-04-16 10:41:37.000000 clipped-0.1.1/clipped.egg-info/PKG-INFO
--rw-r--r--   0 mourad     (501) staff       (20)     1796 2023-04-16 10:41:37.000000 clipped-0.1.1/clipped.egg-info/SOURCES.txt
--rw-r--r--   0 mourad     (501) staff       (20)        1 2023-04-16 10:41:37.000000 clipped-0.1.1/clipped.egg-info/dependency_links.txt
--rw-r--r--   0 mourad     (501) staff       (20)        8 2023-04-16 10:41:37.000000 clipped-0.1.1/clipped.egg-info/top_level.txt
--rw-r--r--   0 mourad     (501) staff       (20)     1033 2023-04-16 10:41:37.725202 clipped-0.1.1/setup.cfg
--rw-r--r--   0 mourad     (501) staff       (20)     2345 2023-04-16 10:40:33.000000 clipped-0.1.1/setup.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-23 10:34:51.466678 clipped-0.2.0/
+-rw-r--r--   0 mourad     (501) staff       (20)      174 2023-04-23 10:32:52.000000 clipped-0.2.0/MANIFEST.in
+-rw-r--r--   0 mourad     (501) staff       (20)     2012 2023-04-23 10:34:51.466792 clipped-0.2.0/PKG-INFO
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-23 10:34:51.451210 clipped-0.2.0/clipped/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/__init__.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-23 10:34:51.454227 clipped-0.2.0/clipped/config/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/config/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)       91 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/config/constants.py
+-rw-r--r--   0 mourad     (501) staff       (20)       40 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/config/exceptions.py
+-rw-r--r--   0 mourad     (501) staff       (20)     4022 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/config/manager.py
+-rw-r--r--   0 mourad     (501) staff       (20)     6164 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/config/parser.py
+-rw-r--r--   0 mourad     (501) staff       (20)      527 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/config/patch_strategy.py
+-rw-r--r--   0 mourad     (501) staff       (20)    14833 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/config/schema.py
+-rw-r--r--   0 mourad     (501) staff       (20)     8892 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/config/spec.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-23 10:34:51.455383 clipped-0.2.0/clipped/decorators/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/decorators/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)      646 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/decorators/cached_property.py
+-rw-r--r--   0 mourad     (501) staff       (20)     4355 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/decorators/deprecation.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1923 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/decorators/memoization.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2686 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/decorators/signals.py
+-rw-r--r--   0 mourad     (501) staff       (20)     6256 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/formatting.py
+-rw-r--r--   0 mourad     (501) staff       (20)      824 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/manager_interface.py
+-rw-r--r--   0 mourad     (501) staff       (20)      203 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/pkg.py
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/py.typed
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-23 10:34:51.458042 clipped-0.2.0/clipped/types/
+-rw-r--r--   0 mourad     (501) staff       (20)     3862 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/types/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1298 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/types/docker_image.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1889 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/types/email.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1033 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/types/gcs.py
+-rw-r--r--   0 mourad     (501) staff       (20)      698 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/types/lists.py
+-rw-r--r--   0 mourad     (501) staff       (20)      158 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/types/numbers.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1142 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/types/ref_or_obj.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1019 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/types/s3.py
+-rw-r--r--   0 mourad     (501) staff       (20)      965 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/types/strings.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1265 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/types/uri.py
+-rw-r--r--   0 mourad     (501) staff       (20)      688 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/types/uuids.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3179 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/types/wasb.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-23 10:34:51.466462 clipped-0.2.0/clipped/utils/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/utils/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1004 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/utils/bools.py
+-rw-r--r--   0 mourad     (501) staff       (20)      143 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/utils/click.py
+-rw-r--r--   0 mourad     (501) staff       (20)      665 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/utils/cmd.py
+-rw-r--r--   0 mourad     (501) staff       (20)      570 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/utils/coroutine.py
+-rw-r--r--   0 mourad     (501) staff       (20)      755 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/utils/csv.py
+-rw-r--r--   0 mourad     (501) staff       (20)     7568 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/utils/dates.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3354 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/utils/dicts.py
+-rw-r--r--   0 mourad     (501) staff       (20)      496 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/utils/encoding.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1093 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/utils/enums.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2001 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/utils/env.py
+-rw-r--r--   0 mourad     (501) staff       (20)     4737 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/utils/git.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1827 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/utils/hashing.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1175 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/utils/http.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3363 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/utils/humanize.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1327 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/utils/imports.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1695 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/utils/indentation.py
+-rw-r--r--   0 mourad     (501) staff       (20)      420 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/utils/json.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1163 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/utils/lists.py
+-rw-r--r--   0 mourad     (501) staff       (20)      113 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/utils/logging.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1280 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/utils/np.py
+-rw-r--r--   0 mourad     (501) staff       (20)     8484 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/utils/paths.py
+-rw-r--r--   0 mourad     (501) staff       (20)      674 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/utils/query_params.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1134 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/utils/requests.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1041 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/utils/responses.py
+-rw-r--r--   0 mourad     (501) staff       (20)      595 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/utils/sanitizers.py
+-rw-r--r--   0 mourad     (501) staff       (20)      676 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/utils/serialization.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2674 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/utils/strings.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1115 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/utils/tz.py
+-rw-r--r--   0 mourad     (501) staff       (20)     4040 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/utils/units.py
+-rw-r--r--   0 mourad     (501) staff       (20)      269 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/utils/urls.py
+-rw-r--r--   0 mourad     (501) staff       (20)      614 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/utils/validation.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1128 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/utils/versions.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1068 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/utils/workers.py
+-rw-r--r--   0 mourad     (501) staff       (20)      546 2023-04-23 10:32:52.000000 clipped-0.2.0/clipped/utils/yaml.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-23 10:34:51.451969 clipped-0.2.0/clipped.egg-info/
+-rw-r--r--   0 mourad     (501) staff       (20)     2012 2023-04-23 10:34:51.000000 clipped-0.2.0/clipped.egg-info/PKG-INFO
+-rw-r--r--   0 mourad     (501) staff       (20)     1821 2023-04-23 10:34:51.000000 clipped-0.2.0/clipped.egg-info/SOURCES.txt
+-rw-r--r--   0 mourad     (501) staff       (20)        1 2023-04-23 10:34:51.000000 clipped-0.2.0/clipped.egg-info/dependency_links.txt
+-rw-r--r--   0 mourad     (501) staff       (20)        8 2023-04-23 10:34:51.000000 clipped-0.2.0/clipped.egg-info/top_level.txt
+-rw-r--r--   0 mourad     (501) staff       (20)     1033 2023-04-23 10:34:51.467331 clipped-0.2.0/setup.cfg
+-rw-r--r--   0 mourad     (501) staff       (20)     2345 2023-04-23 10:32:52.000000 clipped-0.2.0/setup.py
```

### Comparing `clipped-0.1.1/PKG-INFO` & `clipped-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipped
-Version: 0.1.1
+Version: 0.2.0
 Summary: Common shortcuts and utils.
 Home-page: https://github.com/mmourafiq/clipped
 Author: Mourad Mourafiq
 Author-email: mourad.mourafiq@gmail.com
 Maintainer: Mourad Mourafiq
 Maintainer-email: mourad.mourafiq@gmail.com
 License: Apache 2.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: clipped Version: 0.1.1 Summary: Common shortcuts
+Metadata-Version: 2.1 Name: clipped Version: 0.2.0 Summary: Common shortcuts
 and utils. Home-page: https://github.com/mmourafiq/clipped Author: Mourad
 Mourafiq Author-email: mourad.mourafiq@gmail.com Maintainer: Mourad Mourafiq
 Maintainer-email: mourad.mourafiq@gmail.com License: Apache 2.0 Keywords:
 cli,configuration,utils,setup Platform: any Classifier: Intended Audience ::
 Information Technology Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Science/Research Classifier: Operating System :: OS Independent Classifier:
```

### Comparing `clipped-0.1.1/clipped/config/manager.py` & `clipped-0.2.0/clipped/config/manager.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.1/clipped/config/parser.py` & `clipped-0.2.0/clipped/config/parser.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.1/clipped/config/patch_strategy.py` & `clipped-0.2.0/clipped/config/patch_strategy.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.1/clipped/config/schema.py` & `clipped-0.2.0/clipped/config/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,18 +41,14 @@
             data["kind"] = data.pop("kind", self._IDENTIFIER)
         super().__init__(**data)
 
     @classmethod
     def get_identifier(cls):
         return cls._IDENTIFIER
 
-    @staticmethod
-    def _dump(obj_dict: Dict) -> str:
-        return orjson_dumps(obj_dict)
-
     def to_light_dict(
         self,
         humanize_values: bool = False,
         include_attrs: List[str] = None,
         exclude_attrs: List[str] = None,
     ) -> Dict[str, Any]:
         obj_dict = self.to_dict(humanize_values=humanize_values)
```

### Comparing `clipped-0.1.1/clipped/config/spec.py` & `clipped-0.2.0/clipped/config/spec.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.1/clipped/decorators/cached_property.py` & `clipped-0.2.0/clipped/decorators/cached_property.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.1/clipped/decorators/deprecation.py` & `clipped-0.2.0/clipped/decorators/deprecation.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.1/clipped/decorators/memoization.py` & `clipped-0.2.0/clipped/decorators/memoization.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.1/clipped/decorators/signals.py` & `clipped-0.2.0/clipped/decorators/signals.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.1/clipped/formatting.py` & `clipped-0.2.0/clipped/formatting.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.1/clipped/manager_interface.py` & `clipped-0.2.0/clipped/manager_interface.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.1/clipped/types/__init__.py` & `clipped-0.2.0/clipped/types/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 )
 
 from clipped.types.docker_image import ImageStr
 from clipped.types.email import EmailStr
 from clipped.types.gcs import GcsPath
 from clipped.types.lists import ListStr
 from clipped.types.s3 import S3Path
+from clipped.types.strings import GenericStr
 from clipped.types.uri import Uri
 from clipped.types.uuids import UUIDStr
 from clipped.types.wasb import WasbPath
 
 URI = "uri"
 AUTH = "auth"
 LIST = "list"
@@ -72,21 +73,23 @@
     S3: S3Path,
     WASB: WasbPath,
     PATH: str,
     METRIC: float,
     METADATA: Dict,
     UUID: UUIDStr,
     EMAIL: EmailStr,
+    "str": GenericStr,
     "date": datetime.date,
     "datetime": datetime.date,
     "timedelta": datetime.timedelta,
 }
 
 
 FORWARDING = {
+    "GenericStr": GenericStr,
     "Uri": Uri,
     "ImageStr": ImageStr,
     "GcsPath": GcsPath,
     "S3Path": S3Path,
     "WasbPath": WasbPath,
     "UUIDStr": UUIDStr,
     "EmailStr": EmailStr,
@@ -149,14 +152,15 @@
     S3,
     S3Path,
     WASB,
     WasbPath,
     EmailStr,
     UUIDStr,
     ListStr,
+    GenericStr,
     datetime.date,
     datetime.datetime,
     datetime.timedelta,
 }
 
 
 COMPATIBLE_TYPES = [
```

### Comparing `clipped-0.1.1/clipped/types/docker_image.py` & `clipped-0.2.0/clipped/types/docker_image.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.1/clipped/types/email.py` & `clipped-0.2.0/clipped/types/email.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.1/clipped/types/gcs.py` & `clipped-0.2.0/clipped/types/gcs.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.1/clipped/types/lists.py` & `clipped-0.2.0/clipped/types/uuids.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from typing import TYPE_CHECKING
+from uuid import UUID
 
-from clipped.utils.lists import to_list
+from pydantic import StrictStr
 
 if TYPE_CHECKING:
     from pydantic.typing import CallableGenerator
 
 
-class ListStr(list):
+class UUIDStr(StrictStr):
     @classmethod
     def __get_validators__(cls) -> "CallableGenerator":
         yield cls.validate
 
     @classmethod
     def validate(cls, value, **kwargs):
-        if isinstance(value, list):
-            return value
         if isinstance(value, str):
-            return to_list(value, check_none=True, check_str=True)
+            return UUID(value).hex
+        if isinstance(value, UUID):
+            return value.hex
         if not value:
             return value
 
         field = kwargs.get("field")
         raise TypeError(
-            f"Field `{field.name}` value be a valid UUID, received `{value}` instead."
+            f"Field `{field.name}` value must be a valid UUID, received `{value}` instead."
         )
```

### Comparing `clipped-0.1.1/clipped/types/ref_or_obj.py` & `clipped-0.2.0/clipped/types/ref_or_obj.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.1/clipped/types/s3.py` & `clipped-0.2.0/clipped/types/s3.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.1/clipped/types/uri.py` & `clipped-0.2.0/clipped/types/uri.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.1/clipped/types/uuids.py` & `clipped-0.2.0/clipped/types/strings.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 from typing import TYPE_CHECKING
 from uuid import UUID
 
-from pydantic import StrictStr
+from clipped.utils.json import orjson_dumps
 
 if TYPE_CHECKING:
     from pydantic.typing import CallableGenerator
 
 
-class UUIDStr(StrictStr):
+class GenericStr(str):
     @classmethod
     def __get_validators__(cls) -> "CallableGenerator":
         yield cls.validate
 
     @classmethod
     def validate(cls, value, **kwargs):
+        base_types = (int, float, dict, list, tuple, set)
+        if isinstance(value, base_types):
+            return orjson_dumps(value)
         if isinstance(value, str):
-            return UUID(value).hex
+            return value
         if isinstance(value, UUID):
             return value.hex
-        if not value:
+        if value is None:
             return value
-
-        field = kwargs.get("field")
-        raise TypeError(
-            f"Field `{field.name}` value be a valid UUID, received `{value}` instead."
-        )
+        try:
+            return str(value)
+        except Exception as e:
+            field = kwargs.get("field")
+            raise TypeError(
+                f"Field `{field.name}` value must be a valid str or a value that can be casted to a str, received `{value}` instead."
+            ) from e
```

### Comparing `clipped-0.1.1/clipped/types/wasb.py` & `clipped-0.2.0/clipped/types/wasb.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.1/clipped/utils/bools.py` & `clipped-0.2.0/clipped/utils/bools.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.1/clipped/utils/cmd.py` & `clipped-0.2.0/clipped/utils/cmd.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.1/clipped/utils/coroutine.py` & `clipped-0.2.0/clipped/utils/coroutine.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.1/clipped/utils/csv.py` & `clipped-0.2.0/clipped/utils/csv.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.1/clipped/utils/dates.py` & `clipped-0.2.0/clipped/utils/dates.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.1/clipped/utils/dicts.py` & `clipped-0.2.0/clipped/utils/dicts.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.1/clipped/utils/enums.py` & `clipped-0.2.0/clipped/utils/enums.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.1/clipped/utils/env.py` & `clipped-0.2.0/clipped/utils/env.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.1/clipped/utils/git.py` & `clipped-0.2.0/clipped/utils/git.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.1/clipped/utils/hashing.py` & `clipped-0.2.0/clipped/utils/hashing.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.1/clipped/utils/http.py` & `clipped-0.2.0/clipped/utils/http.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.1/clipped/utils/humanize.py` & `clipped-0.2.0/clipped/utils/humanize.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.1/clipped/utils/imports.py` & `clipped-0.2.0/clipped/utils/imports.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.1/clipped/utils/indentation.py` & `clipped-0.2.0/clipped/utils/indentation.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.1/clipped/utils/lists.py` & `clipped-0.2.0/clipped/utils/lists.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.1/clipped/utils/np.py` & `clipped-0.2.0/clipped/utils/np.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.1/clipped/utils/paths.py` & `clipped-0.2.0/clipped/utils/paths.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.1/clipped/utils/query_params.py` & `clipped-0.2.0/clipped/utils/query_params.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.1/clipped/utils/requests.py` & `clipped-0.2.0/clipped/utils/requests.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.1/clipped/utils/responses.py` & `clipped-0.2.0/clipped/utils/responses.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.1/clipped/utils/sanitizers.py` & `clipped-0.2.0/clipped/utils/sanitizers.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.1/clipped/utils/serialization.py` & `clipped-0.2.0/clipped/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.1/clipped/utils/strings.py` & `clipped-0.2.0/clipped/utils/strings.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.1/clipped/utils/tz.py` & `clipped-0.2.0/clipped/utils/tz.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.1/clipped/utils/units.py` & `clipped-0.2.0/clipped/utils/units.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.1/clipped/utils/validation.py` & `clipped-0.2.0/clipped/utils/validation.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.1/clipped/utils/versions.py` & `clipped-0.2.0/clipped/utils/versions.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.1/clipped/utils/workers.py` & `clipped-0.2.0/clipped/utils/workers.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.1/clipped/utils/yaml.py` & `clipped-0.2.0/clipped/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.1/clipped.egg-info/PKG-INFO` & `clipped-0.2.0/clipped.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipped
-Version: 0.1.1
+Version: 0.2.0
 Summary: Common shortcuts and utils.
 Home-page: https://github.com/mmourafiq/clipped
 Author: Mourad Mourafiq
 Author-email: mourad.mourafiq@gmail.com
 Maintainer: Mourad Mourafiq
 Maintainer-email: mourad.mourafiq@gmail.com
 License: Apache 2.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: clipped Version: 0.1.1 Summary: Common shortcuts
+Metadata-Version: 2.1 Name: clipped Version: 0.2.0 Summary: Common shortcuts
 and utils. Home-page: https://github.com/mmourafiq/clipped Author: Mourad
 Mourafiq Author-email: mourad.mourafiq@gmail.com Maintainer: Mourad Mourafiq
 Maintainer-email: mourad.mourafiq@gmail.com License: Apache 2.0 Keywords:
 cli,configuration,utils,setup Platform: any Classifier: Intended Audience ::
 Information Technology Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Science/Research Classifier: Operating System :: OS Independent Classifier:
```

### Comparing `clipped-0.1.1/clipped.egg-info/SOURCES.txt` & `clipped-0.2.0/clipped.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 clipped/types/docker_image.py
 clipped/types/email.py
 clipped/types/gcs.py
 clipped/types/lists.py
 clipped/types/numbers.py
 clipped/types/ref_or_obj.py
 clipped/types/s3.py
+clipped/types/strings.py
 clipped/types/uri.py
 clipped/types/uuids.py
 clipped/types/wasb.py
 clipped/utils/__init__.py
 clipped/utils/bools.py
 clipped/utils/click.py
 clipped/utils/cmd.py
```

### Comparing `clipped-0.1.1/setup.cfg` & `clipped-0.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `clipped-0.1.1/setup.py` & `clipped-0.2.0/setup.py`

 * *Files identical despite different names*

