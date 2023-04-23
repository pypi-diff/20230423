# Comparing `tmp/coredis-4.8.3.tar.gz` & `tmp/coredis-4.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coredis-4.8.3.tar", last modified: Sat Nov  5 00:21:12 2022, max compression
+gzip compressed data, was "coredis-4.9.0.tar", last modified: Thu Nov 10 05:41:30 2022, max compression
```

## Comparing `coredis-4.8.3.tar` & `coredis-4.9.0.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-05 00:21:12.848518 coredis-4.8.3/
--rw-r--r--   0 runner    (1001) docker     (121)    32175 2022-11-05 00:20:59.000000 coredis-4.8.3/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1107 2022-11-05 00:20:59.000000 coredis-4.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      251 2022-11-05 00:20:59.000000 coredis-4.8.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7709 2022-11-05 00:21:12.848518 coredis-4.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6616 2022-11-05 00:20:59.000000 coredis-4.8.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-05 00:21:12.848518 coredis-4.8.3/coredis/
--rw-r--r--   0 runner    (1001) docker     (121)      969 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2615 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/_packer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2008 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/_protocols.py
--rw-r--r--   0 runner    (1001) docker     (121)     4347 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/_sidecar.py
--rw-r--r--   0 runner    (1001) docker     (121)    10897 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-11-05 00:21:12.848518 coredis-4.8.3/coredis/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    27830 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-05 00:21:12.840517 coredis-4.8.3/coredis/client/
--rw-r--r--   0 runner    (1001) docker     (121)      214 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    34584 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/client/basic.py
--rw-r--r--   0 runner    (1001) docker     (121)    41381 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/client/cluster.py
--rw-r--r--   0 runner    (1001) docker     (121)    11339 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/client/keydb.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-05 00:21:12.844518 coredis-4.8.3/coredis/commands/
--rw-r--r--   0 runner    (1001) docker     (121)     1009 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18598 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/commands/_key_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)     2533 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/commands/_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     5484 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/commands/_validators.py
--rw-r--r--   0 runner    (1001) docker     (121)     7569 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/commands/_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (121)     3335 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/commands/bitfield.py
--rw-r--r--   0 runner    (1001) docker     (121)    21429 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/commands/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)   244155 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/commands/core.py
--rw-r--r--   0 runner    (1001) docker     (121)    16180 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/commands/function.py
--rw-r--r--   0 runner    (1001) docker     (121)     5129 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/commands/monitor.py
--rw-r--r--   0 runner    (1001) docker     (121)    25199 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/commands/pubsub.py
--rw-r--r--   0 runner    (1001) docker     (121)    12282 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/commands/script.py
--rw-r--r--   0 runner    (1001) docker     (121)     7633 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/commands/sentinel.py
--rw-r--r--   0 runner    (1001) docker     (121)     1368 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/config.py
--rw-r--r--   0 runner    (1001) docker     (121)    27052 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/connection.py
--rw-r--r--   0 runner    (1001) docker     (121)     1048 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     7650 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-05 00:21:12.844518 coredis-4.8.3/coredis/experimental/
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      360 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/globals.py
--rw-r--r--   0 runner    (1001) docker     (121)    11368 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)    42391 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (121)    92091 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/pipeline.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-05 00:21:12.844518 coredis-4.8.3/coredis/pool/
--rw-r--r--   0 runner    (1001) docker     (121)      301 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/pool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16319 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/pool/basic.py
--rw-r--r--   0 runner    (1001) docker     (121)    19507 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/pool/cluster.py
--rw-r--r--   0 runner    (1001) docker     (121)    12521 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/pool/nodemanager.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-05 00:21:12.844518 coredis-4.8.3/coredis/recipes/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/recipes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-05 00:21:12.844518 coredis-4.8.3/coredis/recipes/locks/
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/recipes/locks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      426 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/recipes/locks/extend.lua
--rw-r--r--   0 runner    (1001) docker     (121)     9188 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/recipes/locks/lua_lock.py
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/recipes/locks/release.lua
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-05 00:21:12.844518 coredis-4.8.3/coredis/response/
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/response/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-05 00:21:12.844518 coredis-4.8.3/coredis/response/_callbacks/
--rw-r--r--   0 runner    (1001) docker     (121)    14622 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/response/_callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1062 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/response/_callbacks/acl.py
--rw-r--r--   0 runner    (1001) docker     (121)     6194 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/response/_callbacks/cluster.py
--rw-r--r--   0 runner    (1001) docker     (121)     2917 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/response/_callbacks/command.py
--rw-r--r--   0 runner    (1001) docker     (121)      984 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/response/_callbacks/connection.py
--rw-r--r--   0 runner    (1001) docker     (121)     1891 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/response/_callbacks/geo.py
--rw-r--r--   0 runner    (1001) docker     (121)     2658 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/response/_callbacks/hash.py
--rw-r--r--   0 runner    (1001) docker     (121)     1720 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/response/_callbacks/keys.py
--rw-r--r--   0 runner    (1001) docker     (121)     1012 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/response/_callbacks/module.py
--rw-r--r--   0 runner    (1001) docker     (121)     3232 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/response/_callbacks/script.py
--rw-r--r--   0 runner    (1001) docker     (121)     5023 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/response/_callbacks/sentinel.py
--rw-r--r--   0 runner    (1001) docker     (121)     6977 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/response/_callbacks/server.py
--rw-r--r--   0 runner    (1001) docker     (121)     1458 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/response/_callbacks/sets.py
--rw-r--r--   0 runner    (1001) docker     (121)     5992 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/response/_callbacks/sorted_set.py
--rw-r--r--   0 runner    (1001) docker     (121)     6169 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/response/_callbacks/streams.py
--rw-r--r--   0 runner    (1001) docker     (121)     2126 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/response/_callbacks/strings.py
--rw-r--r--   0 runner    (1001) docker     (121)      734 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/response/_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    11802 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/response/types.py
--rw-r--r--   0 runner    (1001) docker     (121)    16333 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/sentinel.py
--rw-r--r--   0 runner    (1001) docker     (121)     4787 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/speedups.c
--rw-r--r--   0 runner    (1001) docker     (121)      109 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/speedups.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    13218 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/stream.py
--rw-r--r--   0 runner    (1001) docker     (121)    16045 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/tokens.py
--rw-r--r--   0 runner    (1001) docker     (121)     5758 2022-11-05 00:20:59.000000 coredis-4.8.3/coredis/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-05 00:21:12.840517 coredis-4.8.3/coredis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7709 2022-11-05 00:21:12.000000 coredis-4.8.3/coredis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2260 2022-11-05 00:21:12.000000 coredis-4.8.3/coredis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-05 00:21:12.000000 coredis-4.8.3/coredis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-11-05 00:21:12.000000 coredis-4.8.3/coredis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-11-05 00:21:12.000000 coredis-4.8.3/coredis.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-05 00:21:12.848518 coredis-4.8.3/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-11-05 00:20:59.000000 coredis-4.8.3/requirements/build_ext.txt
--rw-r--r--   0 runner    (1001) docker     (121)      191 2022-11-05 00:20:59.000000 coredis-4.8.3/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)      214 2022-11-05 00:20:59.000000 coredis-4.8.3/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-11-05 00:20:59.000000 coredis-4.8.3/requirements/main.txt
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-11-05 00:20:59.000000 coredis-4.8.3/requirements/publishing.txt
--rw-r--r--   0 runner    (1001) docker     (121)      188 2022-11-05 00:20:59.000000 coredis-4.8.3/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1179 2022-11-05 00:21:12.848518 coredis-4.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4427 2022-11-05 00:20:59.000000 coredis-4.8.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    80044 2022-11-05 00:20:59.000000 coredis-4.8.3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 05:41:30.557381 coredis-4.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)    32696 2022-11-10 05:41:23.000000 coredis-4.9.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1107 2022-11-10 05:41:23.000000 coredis-4.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      251 2022-11-10 05:41:23.000000 coredis-4.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     7718 2022-11-10 05:41:30.557381 coredis-4.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     6625 2022-11-10 05:41:23.000000 coredis-4.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 05:41:30.557381 coredis-4.9.0/coredis/
+-rw-r--r--   0 runner    (1001) docker     (121)      969 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2615 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/_packer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2008 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/_protocols.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4347 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/_sidecar.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10897 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      497 2022-11-10 05:41:30.557381 coredis-4.9.0/coredis/_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27830 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 05:41:30.553381 coredis-4.9.0/coredis/client/
+-rw-r--r--   0 runner    (1001) docker     (121)      214 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34716 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/client/basic.py
+-rw-r--r--   0 runner    (1001) docker     (121)    42449 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/client/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11339 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/client/keydb.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 05:41:30.553381 coredis-4.9.0/coredis/commands/
+-rw-r--r--   0 runner    (1001) docker     (121)     1009 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18598 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/commands/_key_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2533 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/commands/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5484 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/commands/_validators.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7585 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/commands/_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3335 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/commands/bitfield.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21429 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/commands/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)   244155 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/commands/core.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16180 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/commands/function.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5129 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/commands/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25199 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/commands/pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12282 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/commands/script.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7633 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/commands/sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1368 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27052 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/connection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1048 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7650 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 05:41:30.553381 coredis-4.9.0/coredis/experimental/
+-rw-r--r--   0 runner    (1001) docker     (121)      126 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      360 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/globals.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11368 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)    46569 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (121)    92091 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/pipeline.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 05:41:30.553381 coredis-4.9.0/coredis/pool/
+-rw-r--r--   0 runner    (1001) docker     (121)      301 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/pool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16319 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/pool/basic.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19507 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/pool/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12521 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/pool/nodemanager.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 05:41:30.553381 coredis-4.9.0/coredis/recipes/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/recipes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 05:41:30.553381 coredis-4.9.0/coredis/recipes/locks/
+-rw-r--r--   0 runner    (1001) docker     (121)       89 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/recipes/locks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      426 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/recipes/locks/extend.lua
+-rw-r--r--   0 runner    (1001) docker     (121)     9244 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/recipes/locks/lua_lock.py
+-rw-r--r--   0 runner    (1001) docker     (121)      225 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/recipes/locks/release.lua
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 05:41:30.553381 coredis-4.9.0/coredis/response/
+-rw-r--r--   0 runner    (1001) docker     (121)       86 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/response/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 05:41:30.557381 coredis-4.9.0/coredis/response/_callbacks/
+-rw-r--r--   0 runner    (1001) docker     (121)    14622 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/response/_callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1062 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/response/_callbacks/acl.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6194 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/response/_callbacks/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2917 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/response/_callbacks/command.py
+-rw-r--r--   0 runner    (1001) docker     (121)      984 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/response/_callbacks/connection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1891 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/response/_callbacks/geo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2658 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/response/_callbacks/hash.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1720 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/response/_callbacks/keys.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1012 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/response/_callbacks/module.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3232 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/response/_callbacks/script.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5023 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/response/_callbacks/sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6977 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/response/_callbacks/server.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1458 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/response/_callbacks/sets.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5992 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/response/_callbacks/sorted_set.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6169 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/response/_callbacks/streams.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2126 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/response/_callbacks/strings.py
+-rw-r--r--   0 runner    (1001) docker     (121)      734 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/response/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11802 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/response/types.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16333 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4787 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/speedups.c
+-rw-r--r--   0 runner    (1001) docker     (121)      109 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/speedups.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)    13218 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/stream.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16045 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5758 2022-11-10 05:41:23.000000 coredis-4.9.0/coredis/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 05:41:30.553381 coredis-4.9.0/coredis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     7718 2022-11-10 05:41:30.000000 coredis-4.9.0/coredis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2260 2022-11-10 05:41:30.000000 coredis-4.9.0/coredis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-10 05:41:30.000000 coredis-4.9.0/coredis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-11-10 05:41:30.000000 coredis-4.9.0/coredis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-11-10 05:41:30.000000 coredis-4.9.0/coredis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 05:41:30.557381 coredis-4.9.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (121)       56 2022-11-10 05:41:23.000000 coredis-4.9.0/requirements/build_ext.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      191 2022-11-10 05:41:23.000000 coredis-4.9.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      214 2022-11-10 05:41:23.000000 coredis-4.9.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-11-10 05:41:23.000000 coredis-4.9.0/requirements/main.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       70 2022-11-10 05:41:23.000000 coredis-4.9.0/requirements/publishing.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      188 2022-11-10 05:41:23.000000 coredis-4.9.0/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1147 2022-11-10 05:41:30.557381 coredis-4.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     4427 2022-11-10 05:41:23.000000 coredis-4.9.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)    80044 2022-11-10 05:41:23.000000 coredis-4.9.0/versioneer.py
```

### Comparing `coredis-4.8.3/HISTORY.rst` & `coredis-4.9.0/HISTORY.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,29 @@
 .. _aredis: https://github.com/NoneGG/aredis
 
 Changelog
 =========
 
+v4.9.0
+------
+Release Date: 2022-11-09
+
+* Feature
+
+  * Update implementation of transactional pipeline and the
+    behavior of the ``transaction`` method exposed by they cluster
+    client to be consistent with the standalone client.
+
+* Breaking changes
+
+  * Pipeline instances passed into the callable ``func`` parameter
+    of the cluster ``transaction`` method will no longer automatically
+    queue commands until a call to ``multi`` is issued to be consistent
+    with the implementation in the standalone client.
+
 v4.8.3
 ------
 Release Date: 2022-11-04
 
 * Bug Fix
 
   * Ensure pipeline commands are written to the socket in one
@@ -1285,7 +1302,8 @@
 ------
 
 * add scan_iter, sscan_iter, hscan_iter, zscan_iter and corresponding unit tests
 * fix bug of `PubSub.run_in_thread`
 * add more examples
 * change `Script.register` to `Script.execute`
 
+
```

### Comparing `coredis-4.8.3/LICENSE` & `coredis-4.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `coredis-4.8.3/PKG-INFO` & `coredis-4.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coredis
-Version: 4.8.3
+Version: 4.9.0
 Summary: Python async client for Redis key-value store
 Home-page: https://github.com/alisaifee/coredis
 Author: Ali-Akber Saifee
 Author-email: ali@indydevs.org
 Maintainer: Ali-Akber Saifee
 Maintainer-email: ali@indydevs.org
 License: MIT
@@ -169,14 +169,15 @@
 
 ### Supported python versions
 
 -   3.7
 -   3.8
 -   3.9
 -   3.10
+-   3.11
 -   PyPy 3.7
 -   PyPy 3.8
 -   PyPy 3.9
 
 
 ### Redis-like backends
```

### Comparing `coredis-4.8.3/README.md` & `coredis-4.9.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -141,14 +141,15 @@
 
 ### Supported python versions
 
 -   3.7
 -   3.8
 -   3.9
 -   3.10
+-   3.11
 -   PyPy 3.7
 -   PyPy 3.8
 -   PyPy 3.9
 
 
 ### Redis-like backends
```

### Comparing `coredis-4.8.3/coredis/__init__.py` & `coredis-4.9.0/coredis/__init__.py`

 * *Files identical despite different names*

### Comparing `coredis-4.8.3/coredis/_packer.py` & `coredis-4.9.0/coredis/_packer.py`

 * *Files identical despite different names*

### Comparing `coredis-4.8.3/coredis/_protocols.py` & `coredis-4.9.0/coredis/_protocols.py`

 * *Files identical despite different names*

### Comparing `coredis-4.8.3/coredis/_sidecar.py` & `coredis-4.9.0/coredis/_sidecar.py`

 * *Files identical despite different names*

### Comparing `coredis-4.8.3/coredis/_utils.py` & `coredis-4.9.0/coredis/_utils.py`

 * *Files identical despite different names*

### Comparing `coredis-4.8.3/coredis/cache.py` & `coredis-4.9.0/coredis/cache.py`

 * *Files identical despite different names*

### Comparing `coredis-4.8.3/coredis/client/basic.py` & `coredis-4.9.0/coredis/client/basic.py`

 * *Files 1% similar despite different names*

```diff
@@ -918,38 +918,43 @@
     async def pipeline(
         self,
         transaction: Optional[bool] = True,
         watches: Optional[Parameters[KeyT]] = None,
     ) -> "coredis.pipeline.Pipeline[AnyStr]":
         """
         Returns a new pipeline object that can queue multiple commands for
-        later execution. :paramref:`transaction` indicates whether all commands
-        should be executed atomically. Apart from making a group of operations
-        atomic, pipelines are useful for reducing the back-and-forth overhead
-        between the client and server.
+        batch execution.
+
+        :param transaction: indicates whether all commands should be executed atomically.
+        :param watches: If :paramref:`transaction` is True these keys are watched for external
+         changes during the transaction.
         """
         from coredis.pipeline import Pipeline
 
         return Pipeline[AnyStr].proxy(self.connection_pool, transaction, watches)
 
     async def transaction(
         self,
         func: Callable[["coredis.pipeline.Pipeline[AnyStr]"], Coroutine[Any, Any, Any]],
         *watches: KeyT,
+        value_from_callable: bool = False,
+        watch_delay: Optional[float] = None,
         **kwargs: Any,
     ) -> Optional[Any]:
         """
         Convenience method for executing the callable :paramref:`func` as a
         transaction while watching all keys specified in :paramref:`watches`.
-        The :paramref:`func` callable should expect a single argument which is a
-        :class:`coredis.pipeline.Pipeline` object retrieved by calling
-        :meth:`~coredis.Redis.pipeline`.
+
+        :param func: callable should expect a single argument which is a
+         :class:`coredis.pipeline.Pipeline` object retrieved by calling
+         :meth:`~coredis.Redis.pipeline`.
+        :param watches: The keys to watch during the transaction
+        :param value_from_callable: Whether to return the result of transaction or the value
+         returned from :paramref:`func`
         """
-        value_from_callable = kwargs.pop("value_from_callable", False)
-        watch_delay = kwargs.pop("watch_delay", None)
         async with await self.pipeline(True) as pipe:
             while True:
                 try:
                     if watches:
                         await pipe.watch(*watches)
                     func_value = await func(pipe)
                     exec_value = await pipe.execute()
```

### Comparing `coredis-4.8.3/coredis/client/cluster.py` & `coredis-4.9.0/coredis/client/cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -1006,23 +1006,29 @@
 
     async def pipeline(
         self,
         transaction: Optional[bool] = None,
         watches: Optional[Parameters[StringT]] = None,
     ) -> "coredis.pipeline.ClusterPipeline[AnyStr]":
         """
-        Pipelines in cluster mode only provide a subset of the functionality
-        of pipelines in standalone mode.
+        Returns a new pipeline object that can queue multiple commands for
+        batch execution. Pipelines in cluster mode only provide a subset of the
+        functionality of pipelines in standalone mode.
 
         Specifically:
 
-        - Transactions are only supported if all commands in the pipeline
-          only access keys which route to the same node.
         - Each command in the pipeline should only access keys on the same node
-        - Transactions with :paramref:`watch` are not supported.
+        - Transactions are disabled by default and are only supported if all
+          watched keys route to the same node as where the commands in the multi/exec
+          part of the pipeline.
+
+        :param transaction: indicates whether all commands should be executed atomically.
+        :param watches: If :paramref:`transaction` is True these keys are watched for external
+         changes during the transaction.
+
         """
         await self.connection_pool.initialize()
 
         from coredis.pipeline import ClusterPipeline
 
         return ClusterPipeline[AnyStr].proxy(
             connection_pool=self.connection_pool,
@@ -1034,31 +1040,46 @@
     async def transaction(
         self,
         func: Callable[
             ["coredis.pipeline.ClusterPipeline[AnyStr]"],
             Coroutine[Any, Any, Any],
         ],
         *watches: StringT,
+        value_from_callable: bool = False,
+        watch_delay: Optional[float] = None,
         **kwargs: Any,
     ) -> Any:
         """
         Convenience method for executing the callable :paramref:`func` as a
         transaction while watching all keys specified in :paramref:`watches`.
-        The :paramref:`func` callable should expect a single argument which is a
-        :class:`~coredis.pipeline.ClusterPipeline` instance retrieved
-        by calling :meth:`~coredis.RedisCluster.pipeline`
+
+        :param func: callable should expect a single argument which is a
+         :class:`coredis.pipeline.ClusterPipeline` object retrieved by calling
+         :meth:`~coredis.RedisCluster.pipeline`.
+        :param watches: The keys to watch during the transaction. The keys should route
+         to the same node as the keys touched by the commands in :paramref:`func`
+        :param value_from_callable: Whether to return the result of transaction or the value
+         returned from :paramref:`func`
 
         .. warning:: Cluster transactions can only be run with commands that
-           route to the same node.
+           route to the same slot.
+
+        .. versionchanged:: 4.9.0
+
+           When the transaction is started with :paramref:`watches` the
+           :class:`~coredis.pipeline.ClusterPipeline` instance passed to :paramref:`func`
+           will not start queuing commands until a call to
+           :meth:`~coredis.pipeline.ClusterPipeline.multi` is made. This makes the cluster
+           implementation consistent with :meth:`coredis.Redis.transaction`
         """
-        value_from_callable = kwargs.pop("value_from_callable", False)
-        watch_delay = kwargs.pop("watch_delay", None)
-        async with await self.pipeline(True, watches=watches) as pipe:
+        async with await self.pipeline(True) as pipe:
             while True:
                 try:
+                    if watches:
+                        await pipe.watch(*watches)
                     func_value = await func(pipe)
                     exec_value = await pipe.execute()
                     return func_value if value_from_callable else exec_value
                 except WatchError:
                     if watch_delay is not None and watch_delay > 0:
                         await asyncio.sleep(watch_delay)
                     continue
```

### Comparing `coredis-4.8.3/coredis/client/keydb.py` & `coredis-4.9.0/coredis/client/keydb.py`

 * *Files identical despite different names*

### Comparing `coredis-4.8.3/coredis/commands/__init__.py` & `coredis-4.9.0/coredis/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `coredis-4.8.3/coredis/commands/_key_spec.py` & `coredis-4.9.0/coredis/commands/_key_spec.py`

 * *Files identical despite different names*

### Comparing `coredis-4.8.3/coredis/commands/_utils.py` & `coredis-4.9.0/coredis/commands/_utils.py`

 * *Files identical despite different names*

### Comparing `coredis-4.8.3/coredis/commands/_validators.py` & `coredis-4.9.0/coredis/commands/_validators.py`

 * *Files identical despite different names*

### Comparing `coredis-4.8.3/coredis/commands/_wrappers.py` & `coredis-4.9.0/coredis/commands/_wrappers.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,15 +189,15 @@
                 client,  # type: ignore
                 command_name,
                 func.__name__,
                 command_details.version_introduced,
                 command_details.version_deprecated,
                 deprecation_reason,
             )
-            async with command_cache(callable, *args, **kwargs) as response:
+            async with command_cache(callable, *args, **kwargs) as response:  # type: ignore
                 return response
 
         wrapped.__doc__ = textwrap.dedent(wrapped.__doc__ or "")
         if group:
             wrapped.__doc__ = f"""
 {wrapped.__doc__}
```

### Comparing `coredis-4.8.3/coredis/commands/bitfield.py` & `coredis-4.9.0/coredis/commands/bitfield.py`

 * *Files identical despite different names*

### Comparing `coredis-4.8.3/coredis/commands/constants.py` & `coredis-4.9.0/coredis/commands/constants.py`

 * *Files identical despite different names*

### Comparing `coredis-4.8.3/coredis/commands/core.py` & `coredis-4.9.0/coredis/commands/core.py`

 * *Files identical despite different names*

### Comparing `coredis-4.8.3/coredis/commands/function.py` & `coredis-4.9.0/coredis/commands/function.py`

 * *Files identical despite different names*

### Comparing `coredis-4.8.3/coredis/commands/monitor.py` & `coredis-4.9.0/coredis/commands/monitor.py`

 * *Files identical despite different names*

### Comparing `coredis-4.8.3/coredis/commands/pubsub.py` & `coredis-4.9.0/coredis/commands/pubsub.py`

 * *Files identical despite different names*

### Comparing `coredis-4.8.3/coredis/commands/script.py` & `coredis-4.9.0/coredis/commands/script.py`

 * *Files identical despite different names*

### Comparing `coredis-4.8.3/coredis/commands/sentinel.py` & `coredis-4.9.0/coredis/commands/sentinel.py`

 * *Files identical despite different names*

### Comparing `coredis-4.8.3/coredis/config.py` & `coredis-4.9.0/coredis/config.py`

 * *Files identical despite different names*

### Comparing `coredis-4.8.3/coredis/connection.py` & `coredis-4.9.0/coredis/connection.py`

 * *Files identical despite different names*

### Comparing `coredis-4.8.3/coredis/constants.py` & `coredis-4.9.0/coredis/constants.py`

 * *Files identical despite different names*

### Comparing `coredis-4.8.3/coredis/exceptions.py` & `coredis-4.9.0/coredis/exceptions.py`

 * *Files identical despite different names*

### Comparing `coredis-4.8.3/coredis/parser.py` & `coredis-4.9.0/coredis/parser.py`

 * *Files identical despite different names*

### Comparing `coredis-4.8.3/coredis/pipeline.py` & `coredis-4.9.0/coredis/pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,14 +72,16 @@
     ConnectionError,
     TimeoutError,
     MovedError,
     AskError,
     TryAgainError,
 )
 
+UNWATCH_COMMANDS = {CommandName.DISCARD, CommandName.EXEC, CommandName.UNWATCH}
+
 
 def wrap_pipeline_method(
     kls: PipelineMeta, func: Callable[P, Coroutine[Any, Any, R]]
 ) -> Callable[P, Coroutine[Any, Any, R]]:
     @functools.wraps(func)
     async def wrapper(*args: P.args, **kwargs: P.kwargs) -> R:
         return await func(*args, **kwargs)
@@ -188,15 +190,15 @@
             transaction_result = []
             if success:
                 for c in self.commands:
                     if c.command == CommandName.EXEC:
                         if c.result:
                             transaction_result = cast(List[ResponseType], c.result)
                         else:
-                            raise WatchError()
+                            raise WatchError("Watched variable changed.")
                 for idx, c in enumerate(
                     [
                         _c
                         for _c in sorted(self.commands, key=lambda x: x.position)
                         if _c.command not in {CommandName.MULTI, CommandName.EXEC}
                     ]
                 ):
@@ -264,15 +266,14 @@
     Code iterating over the response list should be able to deal with an
     instance of an exception as a potential value. In general, these will be
     ResponseError exceptions, such as those raised when issuing a command
     on a key of a different datatype.
     """
 
     command_stack: List[PipelineCommand]
-    UNWATCH_COMMANDS = {CommandName.DISCARD, CommandName.EXEC, CommandName.UNWATCH}
 
     def __init__(
         self,
         connection_pool: ConnectionPool,
         transaction: Optional[bool],
         watches: Optional[Parameters[KeyT]] = None,
     ) -> None:
@@ -411,15 +412,15 @@
                     )
             except ConnectionError:
                 # the retry failed so cleanup.
                 conn.disconnect()
                 await self.reset_pipeline()
                 raise
         finally:
-            if command in self.UNWATCH_COMMANDS:
+            if command in UNWATCH_COMMANDS:
                 self.watching = False
             elif command == CommandName.WATCH:
                 self.watching = True
 
     def pipeline_execute_command(
         self,
         command: bytes,
@@ -732,24 +733,40 @@
         watches: Optional[Parameters[KeyT]] = None,
     ) -> None:
         self.command_stack = []
         self.refresh_table_asap = False
         self.connection_pool: ClusterConnectionPool = connection_pool
         self.result_callbacks = result_callbacks
         self._transaction = transaction
+        self._watched_node: Optional[ManagedNode] = None
+        self._watched_connection: Optional[ClusterConnection] = None
         self.watches: Optional[Parameters[KeyT]] = watches or None
         self.watching = False
         self.explicit_transaction = False
         self.cache = None  # not implemented.
 
     async def watch(self, *keys: KeyT) -> bool:
-        raise NotImplementedError
+        if self.explicit_transaction:
+            raise RedisError("Cannot issue a WATCH after a MULTI")
+
+        return await self.immediate_execute_command(
+            CommandName.WATCH, *keys, callback=SimpleStringCallback()
+        )
 
     async def unwatch(self) -> bool:
-        raise NotImplementedError
+        if self._watched_connection:
+            try:
+                return await self._unwatch(self._watched_connection)
+            finally:
+                if self._watched_connection:
+                    self.connection_pool.release(self._watched_connection)
+                    self.watching = False
+                    self._watched_node = None
+                    self._watched_connection = None
+        return True
 
     def __repr__(self):
         return f"{type(self).__name__}"
 
     def __del__(self):
         self.reset_pipeline()
 
@@ -773,14 +790,20 @@
     async def execute_command(
         self,
         command: bytes,
         *args: ValueT,
         callback: Callable[..., Any] = NoopCallback(),  # type: ignore
         **options: Optional[ValueT],
     ) -> ClusterPipelineImpl[AnyStr]:  # type: ignore
+        if (
+            self.watching or command == CommandName.WATCH
+        ) and not self.explicit_transaction:
+            return await self.immediate_execute_command(
+                command, *args, callback=callback, **options
+            )  # type: ignore
         return self.pipeline_execute_command(
             command, *args, callback=callback, **options
         )
 
     def pipeline_execute_command(
         self,
         command: bytes,
@@ -825,15 +848,15 @@
 
     async def execute(self, raise_on_error: bool = True) -> Tuple[object, ...]:
         await self.connection_pool.initialize()
 
         if not self.command_stack:
             return ()
 
-        if self._transaction:
+        if self._transaction or self.explicit_transaction:
             execute = self.send_cluster_transaction
         else:
             execute = self.send_cluster_commands
         try:
             return await execute(raise_on_error)
         finally:
             self.reset_pipeline()
@@ -842,14 +865,18 @@
         """Empties pipeline"""
         self.command_stack = []
 
         self.scripts: Set[Script[AnyStr]] = set()
         # clean up the other instance attributes
         self.watching = False
         self.explicit_transaction = False
+        self._watched_node = None
+        if self._watched_connection:
+            self.connection_pool.release(self._watched_connection)
+            self._watched_connection = None
 
     @clusterdown_wrapper
     async def send_cluster_transaction(
         self, raise_on_error: bool = True
     ) -> Tuple[object, ...]:
         attempt = sorted(self.command_stack, key=lambda x: x.position)
         slots: Set[int] = set()
@@ -859,15 +886,22 @@
                 slots.add(slot)
 
             if len(slots) > 1:
                 raise ClusterTransactionError("Multiple nodes involved in transaction")
         if not slots:
             raise ClusterTransactionError("No slots found for transaction")
         node = self.connection_pool.get_node_by_slot(slots.pop())
-        conn = await self.connection_pool.get_connection_by_node(node)
+
+        if self._watched_node and node.name != self._watched_node.name:
+            raise ClusterTransactionError("Multiple nodes involved in transaction")
+
+        conn = (
+            self._watched_connection
+            or await self.connection_pool.get_connection_by_node(node)
+        )
 
         if self.watches:
             await self._watch(node, conn, self.watches)
         node_commands = NodeCommands(conn, in_transaction=True)
         node_commands.append(ClusterPipelineCommand(CommandName.MULTI, ()))
         node_commands.extend(attempt)
         node_commands.append(ClusterPipelineCommand(CommandName.EXEC, ()))
@@ -1018,40 +1052,95 @@
 
         keys: Tuple[ValueT, ...] = KeySpec.extract_keys((command,) + args)
 
         if not keys:
             raise RedisClusterException(
                 f"No way to dispatch {command} to Redis Cluster. Missing key"
             )
-
         slots = {hash_slot(b(key)) for key in keys}
 
         if len(slots) != 1:
             raise ClusterCrossSlotError(command=command, keys=keys)
         return slots.pop()
 
     def _fail_on_redirect(self, allow_redirections: bool) -> None:
         if not allow_redirections:
             raise RedisClusterException(
                 "ASK & MOVED redirection not allowed in this pipeline"
             )
 
     def multi(self) -> None:
-        raise RedisClusterException("method multi() is not implemented")
+        if self.explicit_transaction:
+            raise RedisError("Cannot issue nested calls to MULTI")
+
+        if self.command_stack:
+            raise RedisError(
+                "Commands without an initial WATCH have already been issued"
+            )
+        self.explicit_transaction = True
 
-    def immediate_execute_command(
+    async def immediate_execute_command(
         self,
-        command: CommandName,
+        command: bytes,
         *args: ValueT,
         callback: Callable[..., Any] = NoopCallback(),
         **kwargs: Optional[ValueT],
     ) -> Any:
-        raise RedisClusterException(
-            "method immediate_execute_command() is not implemented"
-        )
+        slot = self._determine_slot(command, *args)
+        node = self.connection_pool.get_node_by_slot(slot)
+        if command == CommandName.WATCH:
+            if self._watched_node and node.name != self._watched_node.name:
+                raise ClusterTransactionError(
+                    "Cannot issue a watch on a different node in the same transaction"
+                )
+            else:
+                self._watched_node = node
+            self._watched_connection = conn = (
+                self._watched_connection
+                or await self.connection_pool.get_connection_by_node(node)
+            )
+        else:
+            conn = await self.connection_pool.get_connection_by_node(node)
+
+        try:
+            request = await conn.create_request(
+                command, *args, decode=kwargs.get("decode")
+            )
+
+            return callback(
+                await request,
+                version=conn.protocol_version,
+                **kwargs,
+            )
+        except (ConnectionError, TimeoutError) as e:
+            conn.disconnect()
+
+            if not conn.retry_on_timeout and isinstance(e, TimeoutError):
+                raise
+            try:
+                if not self.watching:
+                    request = await conn.create_request(
+                        command, *args, decode=kwargs.get("decode")
+                    )
+                    return callback(
+                        await request, version=conn.protocol_version, **kwargs
+                    )
+            except ConnectionError:
+                # the retry failed so cleanup.
+                conn.disconnect()
+                self.reset_pipeline()
+                raise
+        finally:
+            if command in UNWATCH_COMMANDS:
+                self.watching = False
+            elif command == CommandName.WATCH:
+                self.watching = True
+                # don't release the connection if the command was a watch
+                return
+            self.connection_pool.release(conn)
 
     def load_scripts(self):
         raise RedisClusterException("method load_scripts() is not implemented")
 
     async def _watch(
         self, node: ManagedNode, conn: BaseConnection, keys: Parameters[KeyT]
     ) -> bool:
@@ -1194,25 +1283,38 @@
                 connection_pool,
                 result_callbacks=result_callbacks,
                 transaction=transaction,
                 watches=watches,
             )
         )
 
+    def multi(self) -> None:
+        """
+        Starts a transactional block of the pipeline after WATCH commands
+        are issued. End the transactional block with :meth:`execute`
+        """
+        self.__wrapped__.multi()  # Only here for documentation purposes.
+
     async def watch(self, *keys: KeyT) -> bool:  # noqa
         """
-        Unsupported for Cluster
+        Watches the values at keys ``keys``
+
+        :raises: :exc:`~coredis.exceptions.ClusterTransactionError`
+         if a watch is issued on a key that resides on a different
+         cluster node than a previous watch.
         """
-        raise NotImplementedError
+        return await self.__wrapped__.watch(
+            *keys
+        )  # Only here for documentation purposes.
 
     async def unwatch(self) -> bool:  # noqa
         """
-        Unsupported for Cluster
+        Unwatches all previously specified keys
         """
-        raise NotImplementedError
+        return await self.__wrapped__.unwatch()  # Only here for documentation purposes.
 
     async def execute(self, raise_on_error: bool = True) -> Tuple[object, ...]:
         """
         Executes all the commands in the current pipeline
         and return the results of the individual batched commands
         """
         # Only here for documentation purposes.
```

### Comparing `coredis-4.8.3/coredis/pipeline.pyi` & `coredis-4.9.0/coredis/pipeline.pyi`

 * *Files identical despite different names*

### Comparing `coredis-4.8.3/coredis/pool/basic.py` & `coredis-4.9.0/coredis/pool/basic.py`

 * *Files identical despite different names*

### Comparing `coredis-4.8.3/coredis/pool/cluster.py` & `coredis-4.9.0/coredis/pool/cluster.py`

 * *Files identical despite different names*

### Comparing `coredis-4.8.3/coredis/pool/nodemanager.py` & `coredis-4.9.0/coredis/pool/nodemanager.py`

 * *Files identical despite different names*

### Comparing `coredis-4.8.3/coredis/recipes/locks/lua_lock.py` & `coredis-4.9.0/coredis/recipes/locks/lua_lock.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,25 +59,25 @@
             await lock.release()
 
         asyncio.run(test())
     """
 
     @classmethod
     @RELEASE_SCRIPT.wraps(client_arg="client")
-    async def lua_release(
+    async def lua_release(  # type: ignore[empty-body]
         cls,
         client: Union[Redis[AnyStr], RedisCluster[AnyStr]],
         name: KeyT,
         expected_token: StringT,
     ) -> int:
         ...
 
     @classmethod
     @EXTEND_SCRIPT.wraps(client_arg="client")
-    async def lua_extend(
+    async def lua_extend(  # type: ignore[empty-body]
         cls,
         client: Union[Redis[AnyStr], RedisCluster[AnyStr]],
         name: KeyT,
         expected_token: StringT,
         additional_time: int,
     ) -> int:
         ...
```

### Comparing `coredis-4.8.3/coredis/response/_callbacks/__init__.py` & `coredis-4.9.0/coredis/response/_callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `coredis-4.8.3/coredis/response/_callbacks/acl.py` & `coredis-4.9.0/coredis/response/_callbacks/acl.py`

 * *Files identical despite different names*

### Comparing `coredis-4.8.3/coredis/response/_callbacks/cluster.py` & `coredis-4.9.0/coredis/response/_callbacks/cluster.py`

 * *Files identical despite different names*

### Comparing `coredis-4.8.3/coredis/response/_callbacks/command.py` & `coredis-4.9.0/coredis/response/_callbacks/command.py`

 * *Files identical despite different names*

### Comparing `coredis-4.8.3/coredis/response/_callbacks/connection.py` & `coredis-4.9.0/coredis/response/_callbacks/connection.py`

 * *Files identical despite different names*

### Comparing `coredis-4.8.3/coredis/response/_callbacks/geo.py` & `coredis-4.9.0/coredis/response/_callbacks/geo.py`

 * *Files identical despite different names*

### Comparing `coredis-4.8.3/coredis/response/_callbacks/hash.py` & `coredis-4.9.0/coredis/response/_callbacks/hash.py`

 * *Files identical despite different names*

### Comparing `coredis-4.8.3/coredis/response/_callbacks/keys.py` & `coredis-4.9.0/coredis/response/_callbacks/keys.py`

 * *Files identical despite different names*

### Comparing `coredis-4.8.3/coredis/response/_callbacks/module.py` & `coredis-4.9.0/coredis/response/_callbacks/module.py`

 * *Files identical despite different names*

### Comparing `coredis-4.8.3/coredis/response/_callbacks/script.py` & `coredis-4.9.0/coredis/response/_callbacks/script.py`

 * *Files identical despite different names*

### Comparing `coredis-4.8.3/coredis/response/_callbacks/sentinel.py` & `coredis-4.9.0/coredis/response/_callbacks/sentinel.py`

 * *Files identical despite different names*

### Comparing `coredis-4.8.3/coredis/response/_callbacks/server.py` & `coredis-4.9.0/coredis/response/_callbacks/server.py`

 * *Files identical despite different names*

### Comparing `coredis-4.8.3/coredis/response/_callbacks/sets.py` & `coredis-4.9.0/coredis/response/_callbacks/sets.py`

 * *Files identical despite different names*

### Comparing `coredis-4.8.3/coredis/response/_callbacks/sorted_set.py` & `coredis-4.9.0/coredis/response/_callbacks/sorted_set.py`

 * *Files identical despite different names*

### Comparing `coredis-4.8.3/coredis/response/_callbacks/streams.py` & `coredis-4.9.0/coredis/response/_callbacks/streams.py`

 * *Files identical despite different names*

### Comparing `coredis-4.8.3/coredis/response/_callbacks/strings.py` & `coredis-4.9.0/coredis/response/_callbacks/strings.py`

 * *Files identical despite different names*

### Comparing `coredis-4.8.3/coredis/response/_utils.py` & `coredis-4.9.0/coredis/response/_utils.py`

 * *Files identical despite different names*

### Comparing `coredis-4.8.3/coredis/response/types.py` & `coredis-4.9.0/coredis/response/types.py`

 * *Files identical despite different names*

### Comparing `coredis-4.8.3/coredis/sentinel.py` & `coredis-4.9.0/coredis/sentinel.py`

 * *Files identical despite different names*

### Comparing `coredis-4.8.3/coredis/speedups.c` & `coredis-4.9.0/coredis/speedups.c`

 * *Files identical despite different names*

### Comparing `coredis-4.8.3/coredis/stream.py` & `coredis-4.9.0/coredis/stream.py`

 * *Files identical despite different names*

### Comparing `coredis-4.8.3/coredis/tokens.py` & `coredis-4.9.0/coredis/tokens.py`

 * *Files identical despite different names*

### Comparing `coredis-4.8.3/coredis/typing.py` & `coredis-4.9.0/coredis/typing.py`

 * *Files identical despite different names*

### Comparing `coredis-4.8.3/coredis.egg-info/PKG-INFO` & `coredis-4.9.0/coredis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coredis
-Version: 4.8.3
+Version: 4.9.0
 Summary: Python async client for Redis key-value store
 Home-page: https://github.com/alisaifee/coredis
 Author: Ali-Akber Saifee
 Author-email: ali@indydevs.org
 Maintainer: Ali-Akber Saifee
 Maintainer-email: ali@indydevs.org
 License: MIT
@@ -169,14 +169,15 @@
 
 ### Supported python versions
 
 -   3.7
 -   3.8
 -   3.9
 -   3.10
+-   3.11
 -   PyPy 3.7
 -   PyPy 3.8
 -   PyPy 3.9
 
 
 ### Redis-like backends
```

### Comparing `coredis-4.8.3/coredis.egg-info/SOURCES.txt` & `coredis-4.9.0/coredis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `coredis-4.8.3/setup.cfg` & `coredis-4.9.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 strict = True
 check_untyped_defs = True
 disallow_any_generics = True
 disallow_any_unimported = True
 disallow_incomplete_defs = True
 disallow_untyped_defs = True
 disallow_untyped_decorators = True
-enable_recursive_aliases = True
 show_error_codes = True
 warn_return_any = True
 warn_unused_ignores = True
 
 [mypy-coredis.response._callbacks.*]
 ignore_errors = True
```

### Comparing `coredis-4.8.3/setup.py` & `coredis-4.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `coredis-4.8.3/versioneer.py` & `coredis-4.9.0/versioneer.py`

 * *Files identical despite different names*

