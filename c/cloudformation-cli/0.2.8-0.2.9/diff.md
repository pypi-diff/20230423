# Comparing `tmp/cloudformation-cli-0.2.8.tar.gz` & `tmp/cloudformation-cli-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudformation-cli-0.2.8.tar", last modified: Mon May  3 16:55:31 2021, max compression
+gzip compressed data, was "cloudformation-cli-0.2.9.tar", last modified: Tue May 11 00:37:31 2021, max compression
```

## Comparing `cloudformation-cli-0.2.8.tar` & `cloudformation-cli-0.2.9.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-03 16:55:31.447713 cloudformation-cli-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      128 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     8738 2021-05-03 16:55:31.447713 cloudformation-cli-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6625 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      828 2021-05-03 16:55:31.447713 cloudformation-cli-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2536 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-03 16:55:31.427713 cloudformation-cli-0.2.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-03 16:55:31.435713 cloudformation-cli-0.2.8/src/cloudformation_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8738 2021-05-03 16:55:31.000000 cloudformation-cli-0.2.8/src/cloudformation_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2666 2021-05-03 16:55:31.000000 cloudformation-cli-0.2.8/src/cloudformation_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-03 16:55:31.000000 cloudformation-cli-0.2.8/src/cloudformation_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       73 2021-05-03 16:55:31.000000 cloudformation-cli-0.2.8/src/cloudformation_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      268 2021-05-03 16:55:31.000000 cloudformation-cli-0.2.8/src/cloudformation_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2021-05-03 16:55:31.000000 cloudformation-cli-0.2.8/src/cloudformation_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-03 16:55:31.000000 cloudformation-cli-0.2.8/src/cloudformation_cli.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-03 16:55:31.427713 cloudformation-cli-0.2.8/src/rpdk/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-03 16:55:31.443713 cloudformation-cli-0.2.8/src/rpdk/core/
--rw-r--r--   0 runner    (1001) docker     (121)      101 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3534 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/boto_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1767 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/build_image.py
--rw-r--r--   0 runner    (1001) docker     (121)     5439 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-03 16:55:31.443713 cloudformation-cli-0.2.8/src/rpdk/core/contract/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/contract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      232 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/contract/contract_plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)      877 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/contract/interface.py
--rw-r--r--   0 runner    (1001) docker     (121)    23267 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/contract/resource_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     9062 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/contract/resource_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-03 16:55:31.443713 cloudformation-cli-0.2.8/src/rpdk/core/contract/suite/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/contract/suite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4562 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/contract/suite/contract_asserts.py
--rw-r--r--   0 runner    (1001) docker     (121)     5915 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/contract/suite/handler_commons.py
--rw-r--r--   0 runner    (1001) docker     (121)     2594 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/contract/suite/handler_create.py
--rw-r--r--   0 runner    (1001) docker     (121)     3597 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/contract/suite/handler_delete.py
--rw-r--r--   0 runner    (1001) docker     (121)      482 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/contract/suite/handler_misc.py
--rw-r--r--   0 runner    (1001) docker     (121)      544 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/contract/suite/handler_read.py
--rw-r--r--   0 runner    (1001) docker     (121)     3019 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/contract/suite/handler_update.py
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/contract/suite/handler_update_invalid.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-03 16:55:31.443713 cloudformation-cli-0.2.8/src/rpdk/core/data/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-03 16:55:31.431713 cloudformation-cli-0.2.8/src/rpdk/core/data/examples/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-03 16:55:31.443713 cloudformation-cli-0.2.8/src/rpdk/core/data/examples/module/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/data/examples/module/sample.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-03 16:55:31.443713 cloudformation-cli-0.2.8/src/rpdk/core/data/examples/resource/
--rw-r--r--   0 runner    (1001) docker     (121)     4328 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/data/examples/resource/initech.tps.report.v1.json
--rw-r--r--   0 runner    (1001) docker     (121)      866 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/data/logging.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     4076 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/data/managed-upload-infrastructure.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      416 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/data/pytest-contract.ini
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-03 16:55:31.447713 cloudformation-cli-0.2.8/src/rpdk/core/data/schema/
--rw-r--r--   0 runner    (1001) docker     (121)     5901 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/data/schema/meta-schema.json
--rw-r--r--   0 runner    (1001) docker     (121)    17025 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/data/schema/provider.definition.schema.modules.v1.json
--rw-r--r--   0 runner    (1001) docker     (121)    20456 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/data/schema/provider.definition.schema.v1.json
--rw-r--r--   0 runner    (1001) docker     (121)    12521 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/data_loaders.py
--rw-r--r--   0 runner    (1001) docker     (121)      885 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3858 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-03 16:55:31.447713 cloudformation-cli-0.2.8/src/rpdk/core/fragment/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/fragment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11966 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/fragment/generator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1691 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/fragment/lint_warning_printer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1868 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/fragment/module_fragment_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)      593 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/generate.py
--rw-r--r--   0 runner    (1001) docker     (121)     5336 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/init.py
--rw-r--r--   0 runner    (1001) docker     (121)     3711 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/invoke.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-03 16:55:31.447713 cloudformation-cli-0.2.8/src/rpdk/core/jsonutils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/jsonutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7485 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/jsonutils/flattener.py
--rw-r--r--   0 runner    (1001) docker     (121)     3394 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/jsonutils/inliner.py
--rw-r--r--   0 runner    (1001) docker     (121)     3189 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/jsonutils/pointer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1569 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/jsonutils/renamer.py
--rw-r--r--   0 runner    (1001) docker     (121)     8611 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/jsonutils/resolver.py
--rw-r--r--   0 runner    (1001) docker     (121)     7684 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/jsonutils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-03 16:55:31.447713 cloudformation-cli-0.2.8/src/rpdk/core/module/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1453 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/module/init_module.py
--rw-r--r--   0 runner    (1001) docker     (121)     1596 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/plugin_base.py
--rw-r--r--   0 runner    (1001) docker     (121)      614 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/plugin_registry.py
--rw-r--r--   0 runner    (1001) docker     (121)    33830 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/project.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-03 16:55:31.447713 cloudformation-cli-0.2.8/src/rpdk/core/resource/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2990 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/resource/init_resource.py
--rw-r--r--   0 runner    (1001) docker     (121)     1510 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/submit.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-03 16:55:31.447713 cloudformation-cli-0.2.8/src/rpdk/core/templates/
--rw-r--r--   0 runner    (1001) docker     (121)     2793 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/templates/docs-readme.md
--rw-r--r--   0 runner    (1001) docker     (121)     2021 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/templates/docs-subproperty.md
--rw-r--r--   0 runner    (1001) docker     (121)      120 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/templates/inputs.json
--rw-r--r--   0 runner    (1001) docker     (121)      982 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/templates/resource-role.yml
--rw-r--r--   0 runner    (1001) docker     (121)      653 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/templates/template.yml
--rw-r--r--   0 runner    (1001) docker     (121)     9355 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/test.py
--rw-r--r--   0 runner    (1001) docker     (121)     7049 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-03 16:55:31.447713 cloudformation-cli-0.2.8/src/rpdk/core/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2079 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/utils/init_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      433 2021-05-03 16:55:23.000000 cloudformation-cli-0.2.8/src/rpdk/core/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-11 00:37:31.375785 cloudformation-cli-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    11358 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      128 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     8962 2021-05-11 00:37:31.375785 cloudformation-cli-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     6841 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      828 2021-05-11 00:37:31.379786 cloudformation-cli-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2536 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-11 00:37:31.367785 cloudformation-cli-0.2.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-11 00:37:31.371785 cloudformation-cli-0.2.9/src/cloudformation_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     8962 2021-05-11 00:37:31.000000 cloudformation-cli-0.2.9/src/cloudformation_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2666 2021-05-11 00:37:31.000000 cloudformation-cli-0.2.9/src/cloudformation_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-11 00:37:31.000000 cloudformation-cli-0.2.9/src/cloudformation_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       73 2021-05-11 00:37:31.000000 cloudformation-cli-0.2.9/src/cloudformation_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      268 2021-05-11 00:37:31.000000 cloudformation-cli-0.2.9/src/cloudformation_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2021-05-11 00:37:31.000000 cloudformation-cli-0.2.9/src/cloudformation_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-11 00:37:31.000000 cloudformation-cli-0.2.9/src/cloudformation_cli.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-11 00:37:31.367785 cloudformation-cli-0.2.9/src/rpdk/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-11 00:37:31.371785 cloudformation-cli-0.2.9/src/rpdk/core/
+-rw-r--r--   0 runner    (1001) docker     (121)      101 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3534 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/boto_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1767 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/build_image.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5439 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-11 00:37:31.371785 cloudformation-cli-0.2.9/src/rpdk/core/contract/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/contract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      232 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/contract/contract_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (121)      877 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/contract/interface.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23997 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/contract/resource_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9062 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/contract/resource_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-11 00:37:31.375785 cloudformation-cli-0.2.9/src/rpdk/core/contract/suite/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/contract/suite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4562 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/contract/suite/contract_asserts.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5915 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/contract/suite/handler_commons.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2594 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/contract/suite/handler_create.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3597 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/contract/suite/handler_delete.py
+-rw-r--r--   0 runner    (1001) docker     (121)      482 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/contract/suite/handler_misc.py
+-rw-r--r--   0 runner    (1001) docker     (121)      544 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/contract/suite/handler_read.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3019 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/contract/suite/handler_update.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1078 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/contract/suite/handler_update_invalid.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-11 00:37:31.375785 cloudformation-cli-0.2.9/src/rpdk/core/data/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-11 00:37:31.367785 cloudformation-cli-0.2.9/src/rpdk/core/data/examples/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-11 00:37:31.375785 cloudformation-cli-0.2.9/src/rpdk/core/data/examples/module/
+-rw-r--r--   0 runner    (1001) docker     (121)     1070 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/data/examples/module/sample.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-11 00:37:31.375785 cloudformation-cli-0.2.9/src/rpdk/core/data/examples/resource/
+-rw-r--r--   0 runner    (1001) docker     (121)     4328 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/data/examples/resource/initech.tps.report.v1.json
+-rw-r--r--   0 runner    (1001) docker     (121)      866 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/data/logging.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     4076 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/data/managed-upload-infrastructure.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      416 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/data/pytest-contract.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-11 00:37:31.375785 cloudformation-cli-0.2.9/src/rpdk/core/data/schema/
+-rw-r--r--   0 runner    (1001) docker     (121)     5901 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/data/schema/meta-schema.json
+-rw-r--r--   0 runner    (1001) docker     (121)    17025 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/data/schema/provider.definition.schema.modules.v1.json
+-rw-r--r--   0 runner    (1001) docker     (121)    20456 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/data/schema/provider.definition.schema.v1.json
+-rw-r--r--   0 runner    (1001) docker     (121)    12521 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/data_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (121)      885 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3858 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-11 00:37:31.375785 cloudformation-cli-0.2.9/src/rpdk/core/fragment/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/fragment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11966 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/fragment/generator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1691 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/fragment/lint_warning_printer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1868 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/fragment/module_fragment_reader.py
+-rw-r--r--   0 runner    (1001) docker     (121)      593 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/generate.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5336 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/init.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3711 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/invoke.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-11 00:37:31.375785 cloudformation-cli-0.2.9/src/rpdk/core/jsonutils/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/jsonutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7485 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/jsonutils/flattener.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3394 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/jsonutils/inliner.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3189 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/jsonutils/pointer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1569 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/jsonutils/renamer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8611 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/jsonutils/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7684 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/jsonutils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-11 00:37:31.375785 cloudformation-cli-0.2.9/src/rpdk/core/module/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1453 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/module/init_module.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1596 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/plugin_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)      614 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/plugin_registry.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33848 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/project.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-11 00:37:31.375785 cloudformation-cli-0.2.9/src/rpdk/core/resource/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2990 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/resource/init_resource.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1510 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/submit.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-11 00:37:31.375785 cloudformation-cli-0.2.9/src/rpdk/core/templates/
+-rw-r--r--   0 runner    (1001) docker     (121)     2793 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/templates/docs-readme.md
+-rw-r--r--   0 runner    (1001) docker     (121)     2021 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/templates/docs-subproperty.md
+-rw-r--r--   0 runner    (1001) docker     (121)      120 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/templates/inputs.json
+-rw-r--r--   0 runner    (1001) docker     (121)      982 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/templates/resource-role.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      653 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/templates/template.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     9959 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7049 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-11 00:37:31.375785 cloudformation-cli-0.2.9/src/rpdk/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2079 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/utils/init_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      433 2021-05-11 00:37:23.000000 cloudformation-cli-0.2.9/src/rpdk/core/validate.py
```

### Comparing `cloudformation-cli-0.2.8/LICENSE` & `cloudformation-cli-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-0.2.8/PKG-INFO` & `cloudformation-cli-0.2.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudformation-cli
-Version: 0.2.8
+Version: 0.2.9
 Summary: UNKNOWN
 Home-page: https://github.com/aws-cloudformation/aws-cloudformation-rpdk/
 Author: Amazon Web Services
 Author-email: aws-cloudformation-developers@amazon.com
 License: Apache License 2.0
 Description: [![CloudFormation CLI](https://github.com/aws-cloudformation/cloudformation-cli/actions/workflows/pr-ci.yaml/badge.svg?branch=master)](https://github.com/aws-cloudformation/cloudformation-cli/actions/workflows/pr-ci.yaml)
         
@@ -60,14 +60,15 @@
         
         ```bash
         cfn test
         cfn test -- -k contract_delete_update #to run a single test
         cfn test --tb=long #exhaustive, informative traceback formatting
         cfn test --enforce-timeout 60 #set the RL handler timeout to 60 seconds and CUD handler timeout to 120 seconds.
         cfn test --enforce-timeout 60 -- -k contract_delete_update # combine args
+        cfn test --log-group-name cw_log_group --log-role-arn log_delivery_role_arn # Handler logs generated by contract tests will be delivered to the specified cw_log_group using the credentials from log_delivery_role_arn
         ```
         
         ### Command: validate
         
         To validate the schema, use the `validate` command.
         
         This command is automatically run whenever one attempts to submit a resource or module. Errors will prevent you from submitting your resource/module. Module fragments will additionally be validated via [`cfn-lint`](https://github.com/aws-cloudformation/cfn-python-lint/) (but resulting warnings will not cause this step to fail).
```

### Comparing `cloudformation-cli-0.2.8/README.md` & `cloudformation-cli-0.2.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 
 ```bash
 cfn test
 cfn test -- -k contract_delete_update #to run a single test
 cfn test --tb=long #exhaustive, informative traceback formatting
 cfn test --enforce-timeout 60 #set the RL handler timeout to 60 seconds and CUD handler timeout to 120 seconds.
 cfn test --enforce-timeout 60 -- -k contract_delete_update # combine args
+cfn test --log-group-name cw_log_group --log-role-arn log_delivery_role_arn # Handler logs generated by contract tests will be delivered to the specified cw_log_group using the credentials from log_delivery_role_arn
 ```
 
 ### Command: validate
 
 To validate the schema, use the `validate` command.
 
 This command is automatically run whenever one attempts to submit a resource or module. Errors will prevent you from submitting your resource/module. Module fragments will additionally be validated via [`cfn-lint`](https://github.com/aws-cloudformation/cfn-python-lint/) (but resulting warnings will not cause this step to fail).
```

### Comparing `cloudformation-cli-0.2.8/setup.cfg` & `cloudformation-cli-0.2.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-0.2.8/setup.py` & `cloudformation-cli-0.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-0.2.8/src/cloudformation_cli.egg-info/PKG-INFO` & `cloudformation-cli-0.2.9/src/cloudformation_cli.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudformation-cli
-Version: 0.2.8
+Version: 0.2.9
 Summary: UNKNOWN
 Home-page: https://github.com/aws-cloudformation/aws-cloudformation-rpdk/
 Author: Amazon Web Services
 Author-email: aws-cloudformation-developers@amazon.com
 License: Apache License 2.0
 Description: [![CloudFormation CLI](https://github.com/aws-cloudformation/cloudformation-cli/actions/workflows/pr-ci.yaml/badge.svg?branch=master)](https://github.com/aws-cloudformation/cloudformation-cli/actions/workflows/pr-ci.yaml)
         
@@ -60,14 +60,15 @@
         
         ```bash
         cfn test
         cfn test -- -k contract_delete_update #to run a single test
         cfn test --tb=long #exhaustive, informative traceback formatting
         cfn test --enforce-timeout 60 #set the RL handler timeout to 60 seconds and CUD handler timeout to 120 seconds.
         cfn test --enforce-timeout 60 -- -k contract_delete_update # combine args
+        cfn test --log-group-name cw_log_group --log-role-arn log_delivery_role_arn # Handler logs generated by contract tests will be delivered to the specified cw_log_group using the credentials from log_delivery_role_arn
         ```
         
         ### Command: validate
         
         To validate the schema, use the `validate` command.
         
         This command is automatically run whenever one attempts to submit a resource or module. Errors will prevent you from submitting your resource/module. Module fragments will additionally be validated via [`cfn-lint`](https://github.com/aws-cloudformation/cfn-python-lint/) (but resulting warnings will not cause this step to fail).
```

### Comparing `cloudformation-cli-0.2.8/src/cloudformation_cli.egg-info/SOURCES.txt` & `cloudformation-cli-0.2.9/src/cloudformation_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-0.2.8/src/rpdk/core/boto_helpers.py` & `cloudformation-cli-0.2.9/src/rpdk/core/boto_helpers.py`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-0.2.8/src/rpdk/core/build_image.py` & `cloudformation-cli-0.2.9/src/rpdk/core/build_image.py`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-0.2.8/src/rpdk/core/cli.py` & `cloudformation-cli-0.2.9/src/rpdk/core/cli.py`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-0.2.8/src/rpdk/core/contract/interface.py` & `cloudformation-cli-0.2.9/src/rpdk/core/contract/interface.py`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-0.2.8/src/rpdk/core/contract/resource_client.py` & `cloudformation-cli-0.2.9/src/rpdk/core/contract/resource_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -126,20 +126,26 @@
         endpoint,
         region,
         schema,
         overrides,
         inputs=None,
         role_arn=None,
         timeout_in_seconds="30",
+        type_name=None,
+        log_group_name=None,
+        log_role_arn=None,
         docker_image=None,
         executable_entrypoint=None,
     ):  # pylint: disable=too-many-arguments
         self._schema = schema
         self._session = create_sdk_session(region)
         self._role_arn = role_arn
+        self._type_name = type_name
+        self._log_group_name = log_group_name
+        self._log_role_arn = log_role_arn
         self.region = region
         self.account = get_account(
             self._session,
             get_temporary_credentials(self._session, LOWER_CAMEL_CRED_KEYS, role_arn),
         )
         self._function_name = function_name
         if endpoint.startswith("http://"):
@@ -415,32 +421,40 @@
     def make_request(
         desired_resource_state,
         previous_resource_state,
         region,
         account,
         action,
         creds,
+        type_name,
+        log_group_name,
+        log_creds,
         token,
         callback_context=None,
-        **kwargs
+        **kwargs,
     ):
-        return {
+        request_body = {
             "requestData": {
                 "callerCredentials": creds,
                 "resourceProperties": desired_resource_state,
                 "previousResourceProperties": previous_resource_state,
                 "logicalResourceId": token,
             },
             "region": region,
             "awsAccountId": account,
             "action": action,
             "callbackContext": callback_context,
             "bearerToken": token,
+            "resourceType": type_name,
             **kwargs,
         }
+        if log_group_name and log_creds:
+            request_body["requestData"]["providerCredentials"] = log_creds
+            request_body["requestData"]["providerLogGroupName"] = log_group_name
+        return request_body
 
     @staticmethod
     def generate_token():
         return str(uuid4())
 
     def assert_time(self, start_time, end_time, action):
         timeout_in_seconds = (
@@ -492,16 +506,21 @@
             previous_model,
             self.region,
             self.account,
             action,
             get_temporary_credentials(
                 self._session, LOWER_CAMEL_CRED_KEYS, self._role_arn
             ),
+            self._type_name,
+            self._log_group_name,
+            get_temporary_credentials(
+                self._session, LOWER_CAMEL_CRED_KEYS, self._log_role_arn
+            ),
             self.generate_token(),
-            **kwargs
+            **kwargs,
         )
 
     def _call(self, payload):
         request_without_write_properties = prune_properties(
             payload["requestData"]["resourceProperties"], self.write_only_paths
         )
```

### Comparing `cloudformation-cli-0.2.8/src/rpdk/core/contract/resource_generator.py` & `cloudformation-cli-0.2.9/src/rpdk/core/contract/resource_generator.py`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-0.2.8/src/rpdk/core/contract/suite/contract_asserts.py` & `cloudformation-cli-0.2.9/src/rpdk/core/contract/suite/contract_asserts.py`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-0.2.8/src/rpdk/core/contract/suite/handler_commons.py` & `cloudformation-cli-0.2.9/src/rpdk/core/contract/suite/handler_commons.py`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-0.2.8/src/rpdk/core/contract/suite/handler_create.py` & `cloudformation-cli-0.2.9/src/rpdk/core/contract/suite/handler_create.py`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-0.2.8/src/rpdk/core/contract/suite/handler_delete.py` & `cloudformation-cli-0.2.9/src/rpdk/core/contract/suite/handler_delete.py`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-0.2.8/src/rpdk/core/contract/suite/handler_read.py` & `cloudformation-cli-0.2.9/src/rpdk/core/contract/suite/handler_read.py`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-0.2.8/src/rpdk/core/contract/suite/handler_update.py` & `cloudformation-cli-0.2.9/src/rpdk/core/contract/suite/handler_update.py`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-0.2.8/src/rpdk/core/contract/suite/handler_update_invalid.py` & `cloudformation-cli-0.2.9/src/rpdk/core/contract/suite/handler_update_invalid.py`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-0.2.8/src/rpdk/core/data/examples/module/sample.json` & `cloudformation-cli-0.2.9/src/rpdk/core/data/examples/module/sample.json`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-0.2.8/src/rpdk/core/data/examples/resource/initech.tps.report.v1.json` & `cloudformation-cli-0.2.9/src/rpdk/core/data/examples/resource/initech.tps.report.v1.json`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-0.2.8/src/rpdk/core/data/logging.yaml` & `cloudformation-cli-0.2.9/src/rpdk/core/data/logging.yaml`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-0.2.8/src/rpdk/core/data/managed-upload-infrastructure.yaml` & `cloudformation-cli-0.2.9/src/rpdk/core/data/managed-upload-infrastructure.yaml`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-0.2.8/src/rpdk/core/data/schema/meta-schema.json` & `cloudformation-cli-0.2.9/src/rpdk/core/data/schema/meta-schema.json`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-0.2.8/src/rpdk/core/data/schema/provider.definition.schema.modules.v1.json` & `cloudformation-cli-0.2.9/src/rpdk/core/data/schema/provider.definition.schema.modules.v1.json`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-0.2.8/src/rpdk/core/data/schema/provider.definition.schema.v1.json` & `cloudformation-cli-0.2.9/src/rpdk/core/data/schema/provider.definition.schema.v1.json`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-0.2.8/src/rpdk/core/data_loaders.py` & `cloudformation-cli-0.2.9/src/rpdk/core/data_loaders.py`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-0.2.8/src/rpdk/core/exceptions.py` & `cloudformation-cli-0.2.9/src/rpdk/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-0.2.8/src/rpdk/core/filters.py` & `cloudformation-cli-0.2.9/src/rpdk/core/filters.py`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-0.2.8/src/rpdk/core/fragment/generator.py` & `cloudformation-cli-0.2.9/src/rpdk/core/fragment/generator.py`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-0.2.8/src/rpdk/core/fragment/lint_warning_printer.py` & `cloudformation-cli-0.2.9/src/rpdk/core/fragment/lint_warning_printer.py`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-0.2.8/src/rpdk/core/fragment/module_fragment_reader.py` & `cloudformation-cli-0.2.9/src/rpdk/core/fragment/module_fragment_reader.py`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-0.2.8/src/rpdk/core/generate.py` & `cloudformation-cli-0.2.9/src/rpdk/core/generate.py`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-0.2.8/src/rpdk/core/init.py` & `cloudformation-cli-0.2.9/src/rpdk/core/init.py`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-0.2.8/src/rpdk/core/invoke.py` & `cloudformation-cli-0.2.9/src/rpdk/core/invoke.py`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-0.2.8/src/rpdk/core/jsonutils/flattener.py` & `cloudformation-cli-0.2.9/src/rpdk/core/jsonutils/flattener.py`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-0.2.8/src/rpdk/core/jsonutils/inliner.py` & `cloudformation-cli-0.2.9/src/rpdk/core/jsonutils/inliner.py`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-0.2.8/src/rpdk/core/jsonutils/pointer.py` & `cloudformation-cli-0.2.9/src/rpdk/core/jsonutils/pointer.py`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-0.2.8/src/rpdk/core/jsonutils/renamer.py` & `cloudformation-cli-0.2.9/src/rpdk/core/jsonutils/renamer.py`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-0.2.8/src/rpdk/core/jsonutils/resolver.py` & `cloudformation-cli-0.2.9/src/rpdk/core/jsonutils/resolver.py`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-0.2.8/src/rpdk/core/jsonutils/utils.py` & `cloudformation-cli-0.2.9/src/rpdk/core/jsonutils/utils.py`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-0.2.8/src/rpdk/core/module/init_module.py` & `cloudformation-cli-0.2.9/src/rpdk/core/module/init_module.py`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-0.2.8/src/rpdk/core/plugin_base.py` & `cloudformation-cli-0.2.9/src/rpdk/core/plugin_base.py`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-0.2.8/src/rpdk/core/plugin_registry.py` & `cloudformation-cli-0.2.9/src/rpdk/core/plugin_registry.py`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-0.2.8/src/rpdk/core/project.py` & `cloudformation-cli-0.2.9/src/rpdk/core/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,14 +61,15 @@
     "go1.x",
     "python3.6",
     "python3.7",
     "python3.8",
     "dotnetcore2.1",
     "nodejs10.x",
     "nodejs12.x",
+    "nodejs14.x",
 }
 
 SETTINGS_VALIDATOR = Draft7Validator(
     {
         "properties": {
             "artifact_type": {"type": "string"},
             "language": {"type": "string"},
```

### Comparing `cloudformation-cli-0.2.8/src/rpdk/core/resource/init_resource.py` & `cloudformation-cli-0.2.9/src/rpdk/core/resource/init_resource.py`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-0.2.8/src/rpdk/core/submit.py` & `cloudformation-cli-0.2.9/src/rpdk/core/submit.py`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-0.2.8/src/rpdk/core/templates/docs-readme.md` & `cloudformation-cli-0.2.9/src/rpdk/core/templates/docs-readme.md`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-0.2.8/src/rpdk/core/templates/docs-subproperty.md` & `cloudformation-cli-0.2.9/src/rpdk/core/templates/docs-subproperty.md`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-0.2.8/src/rpdk/core/templates/resource-role.yml` & `cloudformation-cli-0.2.9/src/rpdk/core/templates/resource-role.yml`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-0.2.8/src/rpdk/core/templates/template.yml` & `cloudformation-cli-0.2.9/src/rpdk/core/templates/template.yml`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-0.2.8/src/rpdk/core/test.py` & `cloudformation-cli-0.2.9/src/rpdk/core/test.py`

 * *Files 3% similar despite different names*

```diff
@@ -212,14 +212,17 @@
             args.endpoint,
             args.region,
             project.schema,
             overrides,
             inputs,
             args.role_arn,
             args.enforce_timeout,
+            project.type_name,
+            args.log_group_name,
+            args.log_role_arn,
             executable_entrypoint=project.executable_entrypoint,
             docker_image=args.docker_image,
         )
     )
 
     with temporary_ini_file() as path:
         pytest_args = ["-c", path, "-m", get_marker_options(project.schema)]
@@ -251,14 +254,26 @@
 
     parser.add_argument(
         "--enforce-timeout",
         default=DEFAULT_TIMEOUT,
         help="Enforce a different timeout for handlers",
     )
 
+    parser.add_argument(
+        "--log-group-name",
+        help="The log group to which contract tests lambda handler logs will be delivered. "
+        "Specified log group doesn't have to exist as long as log-role-arn specified has logs:CreateLogGroup "
+        "permission. Need to be used together with --log-role-arn",
+    )
+
+    parser.add_argument(
+        "--log-role-arn",
+        help="Role for delivering contract tests lambda handler logs. Need to be used together with --log-group-name",
+    )
+
     parser.add_argument("passed_to_pytest", nargs="*", help=SUPPRESS)
 
     parser.add_argument(
         "--docker-image",
         help="Docker image name to run. If specified, invoke will use docker instead "
         "of SAM",
     )
```

### Comparing `cloudformation-cli-0.2.8/src/rpdk/core/upload.py` & `cloudformation-cli-0.2.9/src/rpdk/core/upload.py`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-0.2.8/src/rpdk/core/utils/init_utils.py` & `cloudformation-cli-0.2.9/src/rpdk/core/utils/init_utils.py`

 * *Files identical despite different names*

