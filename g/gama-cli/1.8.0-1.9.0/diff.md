# Comparing `tmp/gama_cli-1.8.0.tar.gz` & `tmp/gama_cli-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gama_cli-1.8.0.tar", last modified: Fri Apr 14 02:18:10 2023, max compression
+gzip compressed data, was "gama_cli-1.9.0.tar", last modified: Sun Apr 16 23:29:12 2023, max compression
```

## Comparing `gama_cli-1.8.0.tar` & `gama_cli-1.9.0.tar`

### file list

```diff
@@ -1,62 +1,56 @@
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-14 02:18:10.343063 gama_cli-1.8.0/
--rw-rw-r--   0 runner    (1000) runner    (1001)     2302 2023-04-14 02:18:10.343063 gama_cli-1.8.0/PKG-INFO
--rw-rw-r--   0 runner    (1000) runner    (1001)     1664 2023-04-14 02:17:24.000000 gama_cli-1.8.0/README.md
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-14 02:18:10.343063 gama_cli-1.8.0/gama_cli/
--rw-rw-r--   0 runner    (1000) runner    (1001)        0 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/__init__.py
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-14 02:18:10.339063 gama_cli-1.8.0/gama_cli/assets/
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-14 02:18:10.343063 gama_cli-1.8.0/gama_cli/assets/greenstream/
--rw-rw-r--   0 runner    (1000) runner    (1001)      173 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/assets/greenstream/config.sim.yml
--rw-rw-r--   0 runner    (1000) runner    (1001)      597 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/assets/greenstream/config.stubs.yml
--rw-rw-r--   0 runner    (1000) runner    (1001)      583 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/assets/greenstream/config.variant.bravo.yml
--rw-rw-r--   0 runner    (1000) runner    (1001)      184 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/assets/greenstream/config.variant.educat.yml
--rw-rw-r--   0 runner    (1000) runner    (1001)     2539 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/banner.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     3133 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/cli.py
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-14 02:18:10.343063 gama_cli-1.8.0/gama_cli/config/
--rw-rw-r--   0 runner    (1000) runner    (1001)     1632 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/config/gama_gs.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     2418 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/config/gama_vessel.py
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-14 02:18:10.339063 gama_cli-1.8.0/gama_cli/docker/
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-14 02:18:10.343063 gama_cli-1.8.0/gama_cli/docker/gs/
--rw-rw-r--   0 runner    (1000) runner    (1001)      503 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/docker/gs/docker-compose.dev.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)       73 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/docker/gs/docker-compose.network-host.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      172 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/docker/gs/docker-compose.network-shared.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      640 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/docker/gs/docker-compose.network-vpn.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)       68 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/docker/gs/docker-compose.prod.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      157 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/docker/gs/docker-compose.warthog-combo.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      430 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/docker/gs/docker-compose.yaml
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-14 02:18:10.343063 gama_cli-1.8.0/gama_cli/docker/sim/
--rw-rw-r--   0 runner    (1000) runner    (1001)     1038 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/docker/sim/docker-compose.dev.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      744 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/docker/sim/docker-compose.standalone.yaml
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-14 02:18:10.343063 gama_cli-1.8.0/gama_cli/docker/vessel/
--rw-rw-r--   0 runner    (1000) runner    (1001)     2582 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/docker/vessel/docker-compose.dev.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      193 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/docker/vessel/docker-compose.gpu.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      175 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/docker/vessel/docker-compose.network-host.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      459 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/docker/vessel/docker-compose.network-shared.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      912 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/docker/vessel/docker-compose.network-vpn.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      308 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/docker/vessel/docker-compose.prod.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      723 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/docker/vessel/docker-compose.variant-bravo.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      607 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/docker/vessel/docker-compose.variant-educat.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)     1942 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/docker/vessel/docker-compose.yaml
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-14 02:18:10.343063 gama_cli-1.8.0/gama_cli/groups/
--rw-rw-r--   0 runner    (1000) runner    (1001)        0 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/groups/__init__.py
--rw-rw-r--   0 runner    (1000) runner    (1001)      839 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/groups/attach.py
--rw-rw-r--   0 runner    (1000) runner    (1001)      327 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/groups/docker.py
--rw-rw-r--   0 runner    (1000) runner    (1001)      249 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/groups/git.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     5893 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/groups/gs.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     1905 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/groups/misc.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     1168 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/groups/setup.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     4772 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/groups/sim.py
--rw-rw-r--   0 runner    (1000) runner    (1001)    12547 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/groups/vessel.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     5037 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/helpers.py
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-14 02:18:10.343063 gama_cli-1.8.0/gama_cli/schemas/
--rw-rw-r--   0 runner    (1000) runner    (1001)     1118 2023-04-14 02:17:58.000000 gama_cli-1.8.0/gama_cli/schemas/gama_gs.schema.json
--rw-rw-r--   0 runner    (1000) runner    (1001)     2976 2023-04-14 02:17:58.000000 gama_cli-1.8.0/gama_cli/schemas/gama_vessel.schema.json
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-14 02:18:10.343063 gama_cli-1.8.0/gama_cli.egg-info/
--rw-rw-r--   0 runner    (1000) runner    (1001)     2302 2023-04-14 02:18:10.000000 gama_cli-1.8.0/gama_cli.egg-info/PKG-INFO
--rw-rw-r--   0 runner    (1000) runner    (1001)     1779 2023-04-14 02:18:10.000000 gama_cli-1.8.0/gama_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)        1 2023-04-14 02:18:10.000000 gama_cli-1.8.0/gama_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)       46 2023-04-14 02:18:10.000000 gama_cli-1.8.0/gama_cli.egg-info/entry_points.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)       78 2023-04-14 02:18:10.000000 gama_cli-1.8.0/gama_cli.egg-info/requires.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)        9 2023-04-14 02:18:10.000000 gama_cli-1.8.0/gama_cli.egg-info/top_level.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)        1 2023-04-14 02:17:57.000000 gama_cli-1.8.0/gama_cli.egg-info/zip-safe
--rw-rw-r--   0 runner    (1000) runner    (1001)     1002 2023-04-14 02:18:10.343063 gama_cli-1.8.0/setup.cfg
--rw-rw-r--   0 runner    (1000) runner    (1001)       38 2023-04-14 02:17:24.000000 gama_cli-1.8.0/setup.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-16 23:29:12.377755 gama_cli-1.9.0/
+-rw-rw-r--   0 runner    (1000) runner    (1001)     2342 2023-04-16 23:29:12.377755 gama_cli-1.9.0/PKG-INFO
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1708 2023-04-16 23:28:20.000000 gama_cli-1.9.0/README.md
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-16 23:29:12.373755 gama_cli-1.9.0/gama_cli/
+-rw-rw-r--   0 runner    (1000) runner    (1001)        0 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/__init__.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-16 23:29:12.373755 gama_cli-1.9.0/gama_cli/assets/
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-16 23:29:12.377755 gama_cli-1.9.0/gama_cli/assets/greenstream/
+-rw-rw-r--   0 runner    (1000) runner    (1001)      173 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/assets/greenstream/config.sim.yml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      597 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/assets/greenstream/config.stubs.yml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      583 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/assets/greenstream/config.variant.bravo.yml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      184 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/assets/greenstream/config.variant.educat.yml
+-rw-rw-r--   0 runner    (1000) runner    (1001)     2539 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/banner.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     2522 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/cli.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-16 23:29:12.373755 gama_cli-1.9.0/gama_cli/docker/
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-16 23:29:12.377755 gama_cli-1.9.0/gama_cli/docker/gs/
+-rw-rw-r--   0 runner    (1000) runner    (1001)      517 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/docker/gs/docker-compose.dev.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)       73 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/docker/gs/docker-compose.network-host.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      172 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/docker/gs/docker-compose.network-shared.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      640 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/docker/gs/docker-compose.network-vpn.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)       68 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/docker/gs/docker-compose.prod.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      157 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/docker/gs/docker-compose.warthog-combo.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      458 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/docker/gs/docker-compose.yaml
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-16 23:29:12.377755 gama_cli-1.9.0/gama_cli/docker/sim/
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1038 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/docker/sim/docker-compose.dev.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      744 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/docker/sim/docker-compose.standalone.yaml
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-16 23:29:12.377755 gama_cli-1.9.0/gama_cli/docker/vessel/
+-rw-rw-r--   0 runner    (1000) runner    (1001)     2632 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/docker/vessel/docker-compose.dev.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      193 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/docker/vessel/docker-compose.gpu.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      175 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/docker/vessel/docker-compose.network-host.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      459 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/docker/vessel/docker-compose.network-shared.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      912 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/docker/vessel/docker-compose.network-vpn.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      308 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/docker/vessel/docker-compose.prod.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      735 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/docker/vessel/docker-compose.variant-bravo.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      619 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/docker/vessel/docker-compose.variant-educat.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1970 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/docker/vessel/docker-compose.yaml
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-16 23:29:12.377755 gama_cli-1.9.0/gama_cli/groups/
+-rw-rw-r--   0 runner    (1000) runner    (1001)        0 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/groups/__init__.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)      839 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/groups/attach.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)      327 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/groups/docker.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)      249 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/groups/git.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     6513 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/groups/gs.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1905 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/groups/misc.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1168 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/groups/setup.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     4772 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/groups/sim.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)    12958 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/groups/vessel.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     4697 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/helpers.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-16 23:29:12.373755 gama_cli-1.9.0/gama_cli.egg-info/
+-rw-rw-r--   0 runner    (1000) runner    (1001)     2342 2023-04-16 23:29:12.000000 gama_cli-1.9.0/gama_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1643 2023-04-16 23:29:12.000000 gama_cli-1.9.0/gama_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)        1 2023-04-16 23:29:12.000000 gama_cli-1.9.0/gama_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)       46 2023-04-16 23:29:12.000000 gama_cli-1.9.0/gama_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)       73 2023-04-16 23:29:12.000000 gama_cli-1.9.0/gama_cli.egg-info/requires.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)        9 2023-04-16 23:29:12.000000 gama_cli-1.9.0/gama_cli.egg-info/top_level.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)        1 2023-04-16 23:28:58.000000 gama_cli-1.9.0/gama_cli.egg-info/zip-safe
+-rw-rw-r--   0 runner    (1000) runner    (1001)      992 2023-04-16 23:29:12.377755 gama_cli-1.9.0/setup.cfg
+-rw-rw-r--   0 runner    (1000) runner    (1001)       38 2023-04-16 23:28:20.000000 gama_cli-1.9.0/setup.py
```

### Comparing `gama_cli-1.8.0/PKG-INFO` & `gama_cli-1.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: gama_cli
-Version: 1.8.0
+Version: 1.9.0
 Summary: A CLI for interacting with the GAMA platform
-Home-page: https://github.com/Greenroom-Robotics/gama_cli
+Home-page: https://github.com/Greenroom-Robotics/gama
 Author: Greenroom Robotics
 Author-email: team@greenroomrobotics.com
 Maintainer: David Revay
 Maintainer-email: david.revay@greenroomrobotics.com
 License: Copyright (C) 2023, Greenroom Robotics
 Keywords: colcon
 Classifier: Development Status :: 3 - Alpha
@@ -20,15 +20,17 @@
 
 ![GAMA CLI](./docs/gama_cli.png)
 
 Publicly available on [PyPi](https://pypi.org/project/gama-cli/) for convenience but if you don't work at Greenroom Robotics, you probably don't want to use this.
 
 ## Install
 
-* For development: `pip install -e ./tools/gama_cli`
+* For development:
+  * `pip install -e ./libs/gama_config`
+  * `pip install -e ./tools/gama_cli`
 * For production: `pip install gama-cli`
 * You may also need to `export PATH=$PATH:~/.local/bin` if you don't have `~/.local/bin` in your path
 * Install autocomplete:
   * bash: `echo 'eval "$(_GAMA_CLI_COMPLETE=bash_source gama_cli)"' >> ~/.bashrc`
   * zsh: `echo 'eval "$(_GAMA_CLI_COMPLETE=zsh_source gama_cli)"' >> ~/.zshrc` (this is much nicer)
 
 ## Usage
```

### Comparing `gama_cli-1.8.0/README.md` & `gama_cli-1.9.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 
 ![GAMA CLI](./docs/gama_cli.png)
 
 Publicly available on [PyPi](https://pypi.org/project/gama-cli/) for convenience but if you don't work at Greenroom Robotics, you probably don't want to use this.
 
 ## Install
 
-* For development: `pip install -e ./tools/gama_cli`
+* For development:
+  * `pip install -e ./libs/gama_config`
+  * `pip install -e ./tools/gama_cli`
 * For production: `pip install gama-cli`
 * You may also need to `export PATH=$PATH:~/.local/bin` if you don't have `~/.local/bin` in your path
 * Install autocomplete:
   * bash: `echo 'eval "$(_GAMA_CLI_COMPLETE=bash_source gama_cli)"' >> ~/.bashrc`
   * zsh: `echo 'eval "$(_GAMA_CLI_COMPLETE=zsh_source gama_cli)"' >> ~/.zshrc` (this is much nicer)
 
 ## Usage
```

### Comparing `gama_cli-1.8.0/gama_cli/assets/greenstream/config.stubs.yml` & `gama_cli-1.9.0/gama_cli/assets/greenstream/config.stubs.yml`

 * *Files identical despite different names*

### Comparing `gama_cli-1.8.0/gama_cli/assets/greenstream/config.variant.bravo.yml` & `gama_cli-1.9.0/gama_cli/assets/greenstream/config.variant.bravo.yml`

 * *Files identical despite different names*

### Comparing `gama_cli-1.8.0/gama_cli/banner.py` & `gama_cli-1.9.0/gama_cli/banner.py`

 * *Files identical despite different names*

### Comparing `gama_cli-1.8.0/gama_cli/docker/gs/docker-compose.network-vpn.yaml` & `gama_cli-1.9.0/gama_cli/docker/gs/docker-compose.network-vpn.yaml`

 * *Files identical despite different names*

### Comparing `gama_cli-1.8.0/gama_cli/docker/sim/docker-compose.dev.yaml` & `gama_cli-1.9.0/gama_cli/docker/sim/docker-compose.dev.yaml`

 * *Files identical despite different names*

### Comparing `gama_cli-1.8.0/gama_cli/docker/sim/docker-compose.standalone.yaml` & `gama_cli-1.9.0/gama_cli/docker/sim/docker-compose.standalone.yaml`

 * *Files identical despite different names*

### Comparing `gama_cli-1.8.0/gama_cli/docker/vessel/docker-compose.dev.yaml` & `gama_cli-1.9.0/gama_cli/docker/vessel/docker-compose.dev.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
       - ./projects/gama_ui/vite.config.ts:/app/vite.config.ts
       - ./projects/gama_ui/yarn.lock:/app/yarn.lock
     command: yarn dev
 
   gama_vessel:
     entrypoint: ./scripts/watch.sh ./scripts/build.sh
     build:
+      dockerfile: projects/gama_vessel/Dockerfile
       secrets:
         - apt_conf
         - API_TOKEN_GITHUB
     volumes:
       - ./projects/gama_ui/src/generated/ros:/home/ros/gama_vessel/generated/ros
       - ./projects/gama_vessel/src:/home/ros/gama_vessel/src
       - ./projects/gama_vessel/scripts:/home/ros/gama_vessel/scripts
```

### Comparing `gama_cli-1.8.0/gama_cli/docker/vessel/docker-compose.network-vpn.yaml` & `gama_cli-1.9.0/gama_cli/docker/vessel/docker-compose.network-vpn.yaml`

 * *Files identical despite different names*

### Comparing `gama_cli-1.8.0/gama_cli/docker/vessel/docker-compose.variant-bravo.yaml` & `gama_cli-1.9.0/gama_cli/docker/vessel/docker-compose.variant-bravo.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         VITE_GAMA_VARIANT: whiskey_bravo
     environment:
       VITE_GAMA_VARIANT: whiskey_bravo
 
   gama_vessel:
     image: ghcr.io/greenroom-robotics/gama_vessel_whiskey_bravo:${GAMA_VERSION:-latest}
     build:
-      context: ./projects/gama_vessel
+      dockerfile: projects/gama_vessel/Dockerfile
       args:
         - PACKAGE_NAME=whiskey_bravo_bringup
     environment:
       - LOG_STALE_MINUTES=43800 # in minutes
     command: ./scripts/launch.sh whiskey_bravo_bringup vessel.launch.py ${GAMA_VESSEL_COMMAND_ARGS:-}
 
   gama_greenstream:
```

### Comparing `gama_cli-1.8.0/gama_cli/docker/vessel/docker-compose.variant-educat.yaml` & `gama_cli-1.9.0/gama_cli/docker/vessel/docker-compose.variant-educat.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -9,13 +9,13 @@
         VITE_GAMA_VARIANT: educat
     environment:
       VITE_GAMA_VARIANT: educat
 
   gama_vessel:
     image: ghcr.io/greenroom-robotics/gama_vessel_educat:${GAMA_VERSION:-latest}
     build:
-      context: ./projects/gama_vessel
+      dockerfile: projects/gama_vessel/Dockerfile
       args:
         - PACKAGE_NAME=educat_bringup
     environment:
       - LOG_STALE_MINUTES=43800 # in minutes
     command: ./scripts/launch.sh educat_bringup vessel.launch.py ${GAMA_VESSEL_COMMAND_ARGS:-}
```

### Comparing `gama_cli-1.8.0/gama_cli/docker/vessel/docker-compose.yaml` & `gama_cli-1.9.0/gama_cli/docker/vessel/docker-compose.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 
   gama_vessel:
     container_name: gama_vessel
     environment:
       - DISPLAY
     volumes:
       - ./log:/home/ros/.ros/log
+      - ./.gama:/home/.gama
       - /tmp/.X11-unix:/tmp/.X11-unix:rw
       - /dev:/dev
     privileged: true
 
   lookout:
     container_name: lookout
     image: ghcr.io/greenroom-robotics/lookout
```

### Comparing `gama_cli-1.8.0/gama_cli/groups/attach.py` & `gama_cli-1.9.0/gama_cli/groups/attach.py`

 * *Files identical despite different names*

### Comparing `gama_cli-1.8.0/gama_cli/groups/gs.py` & `gama_cli-1.9.0/gama_cli/groups/gs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from typing import List, Optional
 import click
 import os
 
-from gama_cli.config.gama_gs import (
+from gama_config.gama_gs import (
     Network,
     Mode,
     LogLevel,
-    read_gama_gs_config,
+    read_gs_config,
     GamaGsConfig,
-    GAMA_GS_CONFIG_PATH,
-    write_gama_gs_config,
+    get_gs_config_path,
+    write_gs_config,
 )
 from gama_cli.helpers import (
     docker_compose_path,
     get_project_root,
     docker_bake,
     maybe_ignore_build,
     maybe_ignore_prod,
@@ -65,15 +65,15 @@
 def up(
     build: bool,
     args: List[str],
 ):
     """Starts the ground-station"""
     dev_mode = os.environ["GAMA_CLI_DEV_MODE"] == "true"
 
-    config = read_gama_gs_config()
+    config = read_gs_config()
     build = maybe_ignore_build(dev_mode, build)
     prod = maybe_ignore_prod(dev_mode, config.prod)
 
     docker = DockerClient(
         compose_files=_get_compose_files(mode=config.mode, network=config.network, prod=prod),
         compose_project_directory=get_project_root(),
     )
@@ -81,23 +81,33 @@
     buttons = "True" if config.mode == Mode.WARTHOG_COMBO else "False"
 
     gama_gs_command_args = f"mode:={config.mode.value} buttons:={buttons} remote_cmd_override:={config.remote_cmd_override}"
 
     if config.log_level:
         gama_gs_command_args += f" log_level:={config.log_level.value}"
 
+    fields = [
+        "ddsrouter_groundstation_ip",
+        "ddsrouter_groundstation_port",
+        "ddsrouter_vessel_ip",
+        "ddsrouter_vessel_port",
+    ]
+    for field in fields:
+        if getattr(config, field):
+            gama_gs_command_args += f" {field}:='{getattr(config, field)}'"
+
     os.environ["GAMA_GS_COMMAND_ARGS"] = gama_gs_command_args
     docker.compose.up(detach=True, build=build)
 
 
 @click.command(name="down")
 @click.argument("args", nargs=-1)
 def down(args: List[str]):
     """Stops the ground-station"""
-    config = read_gama_gs_config()
+    config = read_gs_config()
 
     docker = DockerClient(
         compose_files=_get_compose_files(config.mode),
         compose_project_directory=get_project_root(),
     )
     docker.compose.down()
 
@@ -117,21 +127,28 @@
                 "Failed to pull GAMA files. Have you ran `gama_cli authenticate` ?",
                 fg="yellow",
             )
         )
 
 
 @click.command(name="configure")
-def configure():  # type: ignore
+@click.option("--default", is_flag=True, help="Use default values")
+def configure(default: bool):  # type: ignore
     """Configure GAMA Ground Station"""
+
+    if default:
+        config = GamaGsConfig()
+        write_gs_config(config)
+        return
+
     # Check if the file exists
-    if os.path.exists(GAMA_GS_CONFIG_PATH):
+    if os.path.exists(get_gs_config_path()):
         click.echo(
             click.style(
-                f"GAMA Ground Station config already exists: {GAMA_GS_CONFIG_PATH}",
+                f"GAMA Ground Station config already exists: {get_gs_config_path()}",
                 fg="yellow",
             )
         )
         result = click.prompt(
             "Do you want to overwrite it?", default="y", type=click.Choice(["y", "n"])
         )
         if result == "n":
@@ -149,16 +166,18 @@
         prod=click.prompt("Prod", type=bool, default=True),
         remote_cmd_override=click.prompt("Remote Command Override", type=bool, default=False),
         log_level=click.prompt(
             "Log Level",
             type=click.Choice([log_level.value for log_level in LogLevel]),
             default=LogLevel.INFO.value,
         ),
+        ddsrouter_vessel_ip=click.prompt("DDS Router Vessel IP", default=""),
+        ddsrouter_groundstation_ip=click.prompt("DDS Router Groundstation IP", default=""),
     )
-    write_gama_gs_config(config)
+    write_gs_config(config)
 
 
 @click.command(name="build")
 def build():
     """Builds the ground-station"""
     docker = DockerClient(
         compose_files=_get_compose_files(),
```

### Comparing `gama_cli-1.8.0/gama_cli/groups/misc.py` & `gama_cli-1.9.0/gama_cli/groups/misc.py`

 * *Files identical despite different names*

### Comparing `gama_cli-1.8.0/gama_cli/groups/setup.py` & `gama_cli-1.9.0/gama_cli/groups/setup.py`

 * *Files identical despite different names*

### Comparing `gama_cli-1.8.0/gama_cli/groups/sim.py` & `gama_cli-1.9.0/gama_cli/groups/sim.py`

 * *Files identical despite different names*

### Comparing `gama_cli-1.8.0/gama_cli/groups/vessel.py` & `gama_cli-1.9.0/gama_cli/groups/vessel.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import os
 from typing import List
 import click
 
-from gama_cli.config.gama_vessel import (
+from gama_config.gama_vessel import (
     Variant,
     Network,
     Mode,
-    read_gama_vessel_config,
-    GAMA_VESSEL_CONFIG_PATH,
+    read_vessel_config,
+    get_vessel_config_path,
     LogLevel,
-    write_gama_vessel_config,
+    write_vessel_config,
     GamaVesselConfig,
 )
 from gama_cli.helpers import (
     call,
     docker_compose_path,
     get_project_root,
     docker_bake,
@@ -104,15 +104,15 @@
     "service",
     required=False,
     type=click.Choice(SERVICES),
 )
 @click.argument("args", nargs=-1)
 def build(service: str, args: List[str]):  # type: ignore
     """Build the vessel"""
-    config = read_gama_vessel_config()
+    config = read_vessel_config()
 
     docker = DockerClient(
         compose_files=_get_compose_files(),
         compose_project_directory=get_project_root(),
     )
 
     os.environ["GAMA_VARIANT"] = config.variant.value
@@ -237,15 +237,15 @@
     build: bool,
     service: str,
     args: List[str],
 ):
     """Starts the vessel"""
     dev_mode = os.environ["GAMA_CLI_DEV_MODE"] == "true"
 
-    config = read_gama_vessel_config()
+    config = read_vessel_config()
     build = maybe_ignore_build(dev_mode, build)
     prod = maybe_ignore_prod(dev_mode, config.prod)
 
     docker = DockerClient(
         compose_files=_get_compose_files(
             gpu=config.extensions.lookout,
             network=config.network,
@@ -263,18 +263,18 @@
     if config.ubiquity_ip:
         vessel_launch_command_args += f" ubiquity_ip:='{config.ubiquity_ip}'"
     if config.log_level:
         vessel_launch_command_args += f" log_level:='{config.log_level.value}'"
 
     # TODO - use config.__dataclass_fields__ and iterate through the Dict[str, Field]
     fields = [
-        "ddsrouter_remote_ip",
-        "ddsrouter_remote_port",
-        "ddsrouter_listen_ip",
-        "ddsrouter_listen_port",
+        "ddsrouter_groundstation_ip",
+        "ddsrouter_groundstation_port",
+        "ddsrouter_vessel_ip",
+        "ddsrouter_vessel_port",
     ]
     for field in fields:
         if getattr(config, field):
             vessel_launch_command_args += f" {field}:='{getattr(config, field)}'"
 
     os.environ["GAMA_VERSION"] = get_gama_version()
     os.environ["GAMA_VARIANT"] = config.variant.value
@@ -316,26 +316,27 @@
 @click.argument("args", nargs=-1)
 def down(args: List[str]):  # type: ignore
     """Stops the vessel"""
     docker = DockerClient(
         compose_files=_get_compose_files(),
         compose_project_directory=get_project_root(),
     )
-    docker.compose.down()
+    # set timeout to 20 secs (default 10) to allow for graceful shutdown of rosbag et al
+    docker.compose.down(timeout=20)
 
 
 @click.command(name="install")
 @click.option(
     "--variant",
     type=click.Choice(Variant),  # type: ignore
     help="Which variant of GAMA to install?",
 )
 def install(variant: Variant):  # type: ignore
     """Install GAMA on a vessel"""
-    config = read_gama_vessel_config()
+    config = read_vessel_config()
     variant = variant or config.variant
     docker = DockerClient(
         compose_files=_get_compose_files(variant=variant),
         compose_project_directory=get_project_root(),
     )
     try:
         docker.compose.pull(
@@ -354,56 +355,61 @@
                 "Failed to pull GAMA files. Have you ran `gama_cli authenticate` ?",
                 fg="yellow",
             )
         )
 
 
 @click.command(name="configure")
-def configure():  # type: ignore
+@click.option("--default", is_flag=True, help="Use default values")
+def configure(default: bool):  # type: ignore
     """Configure GAMA Vessel"""
 
-    # Check if the file exists
-    if os.path.exists(GAMA_VESSEL_CONFIG_PATH):
-        click.echo(
-            click.style(
-                f"GAMA Vessel config already exists: {GAMA_VESSEL_CONFIG_PATH}",
-                fg="yellow",
+    if default:
+        config = GamaVesselConfig()
+        write_vessel_config(config)
+    else:
+        # Check if the file exists
+        if os.path.exists(get_vessel_config_path()):
+            click.echo(
+                click.style(
+                    f"GAMA Vessel config already exists: {get_vessel_config_path()}",
+                    fg="yellow",
+                )
             )
-        )
-        result = click.prompt(
-            "Do you want to overwrite it?", default="y", type=click.Choice(["y", "n"])
-        )
-        if result == "n":
-            return
+            result = click.prompt(
+                "Do you want to overwrite it?", default="y", type=click.Choice(["y", "n"])
+            )
+            if result == "n":
+                return
 
-    config = GamaVesselConfig(
-        variant=click.prompt(
-            "Variant",
-            default=Variant.WHISKEY_BRAVO,
-            type=click.Choice([item.value for item in Variant]),
-        ),
-        ubiquity_user=click.prompt("Ubiquity username", default=""),
-        ubiquity_pass=click.prompt("Ubiquity password", default=""),
-        ubiquity_ip=click.prompt("Ubiquity ip", default=""),
-        mode=click.prompt(
-            "Mode", default=Mode.HARDWARE, type=click.Choice([item.value for item in Mode])
-        ),
-        prod=click.prompt("Prod", default=True, type=bool),
-        network=click.prompt(
-            "Network",
-            default=Network.HOST,
-            type=click.Choice([item.value for item in Network]),
-        ),
-        log_level=click.prompt(
-            "Log level",
-            default=LogLevel.INFO,
-            type=click.Choice([item.value for item in LogLevel]),
-        ),
-    )
-    write_gama_vessel_config(config)
+        config = GamaVesselConfig(
+            variant=click.prompt(
+                "Variant",
+                default=Variant.WHISKEY_BRAVO,
+                type=click.Choice([item.value for item in Variant]),
+            ),
+            ubiquity_user=click.prompt("Ubiquity username", default=""),
+            ubiquity_pass=click.prompt("Ubiquity password", default=""),
+            ubiquity_ip=click.prompt("Ubiquity ip", default=""),
+            mode=click.prompt(
+                "Mode", default=Mode.HARDWARE, type=click.Choice([item.value for item in Mode])
+            ),
+            prod=click.prompt("Prod", default=True, type=bool),
+            network=click.prompt(
+                "Network",
+                default=Network.HOST,
+                type=click.Choice([item.value for item in Network]),
+            ),
+            log_level=click.prompt(
+                "Log level",
+                default=LogLevel.INFO,
+                type=click.Choice([item.value for item in LogLevel]),
+            ),
+        )
+        write_vessel_config(config)
 
     # Now that the GAMA config has been written. Let's write the greenstream config...
     # Check if it exists
     if os.path.exists(GREENSTREAM_CONFIG_DEST_PATH):
         click.echo(
             click.style(
                 f"Greenstream config already exists: {GREENSTREAM_CONFIG_DEST_PATH}",
```

### Comparing `gama_cli-1.8.0/gama_cli/helpers.py` & `gama_cli-1.9.0/gama_cli/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 import click
 import os
 from pathlib import Path
 import subprocess
 import yaml
 import platform
 from python_on_whales.utils import ValidPath
-from dataclasses import asdict
-from enum import Enum
 import pkg_resources
 
 
 def get_project_root() -> Path:
     """Project root is the parent of the config directory. Probably..."""
     p = Path.cwd()
     while len(p.parts) > 1:
@@ -141,26 +139,14 @@
         bake_command,
         shell=True,
         check=True,
         cwd=get_project_root(),
     )
 
 
-def dacite_to_dict(obj):
-    def dict_factory(data):
-        def convert_value(obj):
-            if isinstance(obj, Enum):
-                return obj.value
-            return obj
-
-        return {k: convert_value(v) for k, v in data}
-
-    return asdict(obj, dict_factory=dict_factory)
-
-
 def maybe_ignore_build(dev_mode: bool, build: bool):
     """Force build false in non-dev mode"""
     if dev_mode:
         return build
     if build:
         click.echo(click.style("Ignoring --build flag in non-dev mode", fg="yellow"))
     return False
```

### Comparing `gama_cli-1.8.0/gama_cli.egg-info/PKG-INFO` & `gama_cli-1.9.0/gama_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: gama-cli
-Version: 1.8.0
+Version: 1.9.0
 Summary: A CLI for interacting with the GAMA platform
-Home-page: https://github.com/Greenroom-Robotics/gama_cli
+Home-page: https://github.com/Greenroom-Robotics/gama
 Author: Greenroom Robotics
 Author-email: team@greenroomrobotics.com
 Maintainer: David Revay
 Maintainer-email: david.revay@greenroomrobotics.com
 License: Copyright (C) 2023, Greenroom Robotics
 Keywords: colcon
 Classifier: Development Status :: 3 - Alpha
@@ -20,15 +20,17 @@
 
 ![GAMA CLI](./docs/gama_cli.png)
 
 Publicly available on [PyPi](https://pypi.org/project/gama-cli/) for convenience but if you don't work at Greenroom Robotics, you probably don't want to use this.
 
 ## Install
 
-* For development: `pip install -e ./tools/gama_cli`
+* For development:
+  * `pip install -e ./libs/gama_config`
+  * `pip install -e ./tools/gama_cli`
 * For production: `pip install gama-cli`
 * You may also need to `export PATH=$PATH:~/.local/bin` if you don't have `~/.local/bin` in your path
 * Install autocomplete:
   * bash: `echo 'eval "$(_GAMA_CLI_COMPLETE=bash_source gama_cli)"' >> ~/.bashrc`
   * zsh: `echo 'eval "$(_GAMA_CLI_COMPLETE=zsh_source gama_cli)"' >> ~/.zshrc` (this is much nicer)
 
 ## Usage
```

### Comparing `gama_cli-1.8.0/gama_cli.egg-info/SOURCES.txt` & `gama_cli-1.9.0/gama_cli.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -12,16 +12,14 @@
 gama_cli.egg-info/requires.txt
 gama_cli.egg-info/top_level.txt
 gama_cli.egg-info/zip-safe
 gama_cli/assets/greenstream/config.sim.yml
 gama_cli/assets/greenstream/config.stubs.yml
 gama_cli/assets/greenstream/config.variant.bravo.yml
 gama_cli/assets/greenstream/config.variant.educat.yml
-gama_cli/config/gama_gs.py
-gama_cli/config/gama_vessel.py
 gama_cli/docker/gs/docker-compose.dev.yaml
 gama_cli/docker/gs/docker-compose.network-host.yaml
 gama_cli/docker/gs/docker-compose.network-shared.yaml
 gama_cli/docker/gs/docker-compose.network-vpn.yaml
 gama_cli/docker/gs/docker-compose.prod.yaml
 gama_cli/docker/gs/docker-compose.warthog-combo.yaml
 gama_cli/docker/gs/docker-compose.yaml
@@ -40,10 +38,8 @@
 gama_cli/groups/attach.py
 gama_cli/groups/docker.py
 gama_cli/groups/git.py
 gama_cli/groups/gs.py
 gama_cli/groups/misc.py
 gama_cli/groups/setup.py
 gama_cli/groups/sim.py
-gama_cli/groups/vessel.py
-gama_cli/schemas/gama_gs.schema.json
-gama_cli/schemas/gama_vessel.schema.json
+gama_cli/groups/vessel.py
```

### Comparing `gama_cli-1.8.0/setup.cfg` & `gama_cli-1.9.0/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = gama_cli
-version = 1.8.0
-url = https://github.com/Greenroom-Robotics/gama_cli
+version = 1.9.0
+url = https://github.com/Greenroom-Robotics/gama
 author = Greenroom Robotics
 author_email = team@greenroomrobotics.com
 maintainer = David Revay
 maintainer_email = david.revay@greenroomrobotics.com
 classifiers = 
 	Development Status :: 3 - Alpha
 	Environment :: Plugins
@@ -23,17 +23,16 @@
 packages = find:
 install_requires = 
 	toml~=0.10
 	setuptools
 	colorama
 	click
 	python-on-whales
-	dacite
 	PyYAML
-	dc-schema
+	gama_config
 zip_safe = true
 
 [options.package_data]
 gama_cli = 
 	**/*.json
 	**/*.py
 	**/**/*.yaml
```

