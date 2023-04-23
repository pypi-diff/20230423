# Comparing `tmp/cli_command_parser-2023.4.7.tar.gz` & `tmp/cli_command_parser-2023.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cli_command_parser-2023.4.7.tar", last modified: Fri Apr  7 12:09:56 2023, max compression
+gzip compressed data, was "cli_command_parser-2023.4.8.tar", last modified: Sat Apr  8 14:59:10 2023, max compression
```

## Comparing `cli_command_parser-2023.4.7.tar` & `cli_command_parser-2023.4.8.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 12:09:56.513235 cli_command_parser-2023.4.7/
--rw-rw-rw-   0        0        0    11341 2022-09-17 20:57:36.000000 cli_command_parser-2023.4.7/LICENSE
--rw-rw-rw-   0        0        0       64 2022-09-17 20:57:36.000000 cli_command_parser-2023.4.7/MANIFEST.in
--rw-rw-rw-   0        0        0     4713 2023-04-07 12:09:56.513235 cli_command_parser-2023.4.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-07 12:09:56.336222 cli_command_parser-2023.4.7/lib/
-drwxrwxrwx   0        0        0        0 2023-04-07 12:09:56.419238 cli_command_parser-2023.4.7/lib/cli_command_parser/
--rw-rw-rw-   0        0        0     1016 2022-09-17 20:57:36.000000 cli_command_parser-2023.4.7/lib/cli_command_parser/__init__.py
--rw-rw-rw-   0        0        0      114 2022-09-17 20:57:36.000000 cli_command_parser-2023.4.7/lib/cli_command_parser/__main__.py
--rw-rw-rw-   0        0        0      295 2023-04-07 12:09:46.000000 cli_command_parser-2023.4.7/lib/cli_command_parser/__version__.py
--rw-rw-rw-   0        0        0      463 2022-09-17 20:57:36.000000 cli_command_parser-2023.4.7/lib/cli_command_parser/actions.py
--rw-rw-rw-   0        0        0     3017 2022-10-15 14:00:15.000000 cli_command_parser-2023.4.7/lib/cli_command_parser/annotations.py
--rw-rw-rw-   0        0        0    19746 2023-03-30 11:44:47.000000 cli_command_parser-2023.4.7/lib/cli_command_parser/command_parameters.py
--rw-rw-rw-   0        0        0    12491 2023-03-31 11:57:05.000000 cli_command_parser-2023.4.7/lib/cli_command_parser/commands.py
--rw-rw-rw-   0        0        0     7682 2023-01-14 20:20:57.000000 cli_command_parser-2023.4.7/lib/cli_command_parser/compat.py
--rw-rw-rw-   0        0        0    15521 2023-04-07 12:09:39.000000 cli_command_parser-2023.4.7/lib/cli_command_parser/config.py
--rw-rw-rw-   0        0        0    16854 2023-03-30 11:44:47.000000 cli_command_parser-2023.4.7/lib/cli_command_parser/context.py
-drwxrwxrwx   0        0        0        0 2023-04-07 12:09:56.447236 cli_command_parser-2023.4.7/lib/cli_command_parser/conversion/
--rw-rw-rw-   0        0        0      234 2023-04-06 21:32:03.000000 cli_command_parser-2023.4.7/lib/cli_command_parser/conversion/__init__.py
--rw-rw-rw-   0        0        0       54 2023-04-06 21:32:03.000000 cli_command_parser-2023.4.7/lib/cli_command_parser/conversion/__main__.py
--rw-rw-rw-   0        0        0    12802 2023-04-06 21:32:03.000000 cli_command_parser-2023.4.7/lib/cli_command_parser/conversion/argparse_ast.py
--rw-rw-rw-   0        0        0     1356 2023-04-06 21:32:03.000000 cli_command_parser-2023.4.7/lib/cli_command_parser/conversion/argparse_utils.py
--rw-rw-rw-   0        0        0    21165 2023-04-07 12:09:39.000000 cli_command_parser-2023.4.7/lib/cli_command_parser/conversion/command_builder.py
--rw-rw-rw-   0        0        0     1660 2023-04-06 21:32:03.000000 cli_command_parser-2023.4.7/lib/cli_command_parser/conversion/utils.py
--rw-rw-rw-   0        0        0     7403 2023-04-07 12:09:39.000000 cli_command_parser-2023.4.7/lib/cli_command_parser/conversion/visitor.py
--rw-rw-rw-   0        0        0     9792 2022-09-24 13:23:00.000000 cli_command_parser-2023.4.7/lib/cli_command_parser/core.py
--rw-rw-rw-   0        0        0    13416 2023-03-29 11:48:12.000000 cli_command_parser-2023.4.7/lib/cli_command_parser/documentation.py
--rw-rw-rw-   0        0        0     4800 2022-09-17 20:57:36.000000 cli_command_parser-2023.4.7/lib/cli_command_parser/error_handling.py
--rw-rw-rw-   0        0        0     7775 2022-11-12 17:12:38.000000 cli_command_parser-2023.4.7/lib/cli_command_parser/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-07 12:09:56.463237 cli_command_parser-2023.4.7/lib/cli_command_parser/formatting/
--rw-rw-rw-   0        0        0        0 2022-09-17 20:57:36.000000 cli_command_parser-2023.4.7/lib/cli_command_parser/formatting/__init__.py
--rw-rw-rw-   0        0        0     6557 2022-09-24 13:23:00.000000 cli_command_parser-2023.4.7/lib/cli_command_parser/formatting/commands.py
--rw-rw-rw-   0        0        0    20593 2023-03-29 11:48:12.000000 cli_command_parser-2023.4.7/lib/cli_command_parser/formatting/params.py
--rw-rw-rw-   0        0        0     8572 2022-09-18 21:50:31.000000 cli_command_parser-2023.4.7/lib/cli_command_parser/formatting/restructured_text.py
--rw-rw-rw-   0        0        0     5440 2023-04-06 21:32:03.000000 cli_command_parser-2023.4.7/lib/cli_command_parser/formatting/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-07 12:09:56.485236 cli_command_parser-2023.4.7/lib/cli_command_parser/inputs/
--rw-rw-rw-   0        0        0     2101 2022-09-17 20:57:36.000000 cli_command_parser-2023.4.7/lib/cli_command_parser/inputs/__init__.py
--rw-rw-rw-   0        0        0     1418 2022-09-17 20:57:36.000000 cli_command_parser-2023.4.7/lib/cli_command_parser/inputs/base.py
--rw-rw-rw-   0        0        0     6313 2022-09-17 20:57:36.000000 cli_command_parser-2023.4.7/lib/cli_command_parser/inputs/choices.py
--rw-rw-rw-   0        0        0     1122 2022-09-17 20:57:36.000000 cli_command_parser-2023.4.7/lib/cli_command_parser/inputs/exceptions.py
--rw-rw-rw-   0        0        0     8408 2023-01-14 18:15:47.000000 cli_command_parser-2023.4.7/lib/cli_command_parser/inputs/files.py
--rw-rw-rw-   0        0        0     7242 2023-01-14 18:15:47.000000 cli_command_parser-2023.4.7/lib/cli_command_parser/inputs/numeric.py
--rw-rw-rw-   0        0        0    19507 2022-09-17 20:57:36.000000 cli_command_parser-2023.4.7/lib/cli_command_parser/inputs/time.py
--rw-rw-rw-   0        0        0     6490 2023-01-14 20:20:57.000000 cli_command_parser-2023.4.7/lib/cli_command_parser/inputs/utils.py
--rw-rw-rw-   0        0        0     8145 2023-01-15 15:08:06.000000 cli_command_parser-2023.4.7/lib/cli_command_parser/metadata.py
--rw-rw-rw-   0        0        0     6538 2022-09-19 11:52:48.000000 cli_command_parser-2023.4.7/lib/cli_command_parser/nargs.py
-drwxrwxrwx   0        0        0        0 2023-04-07 12:09:56.512236 cli_command_parser-2023.4.7/lib/cli_command_parser/parameters/
--rw-rw-rw-   0        0        0      300 2022-09-17 20:57:36.000000 cli_command_parser-2023.4.7/lib/cli_command_parser/parameters/__init__.py
--rw-rw-rw-   0        0        0    25575 2023-04-01 22:51:43.000000 cli_command_parser-2023.4.7/lib/cli_command_parser/parameters/base.py
--rw-rw-rw-   0        0        0    17128 2022-09-18 21:50:31.000000 cli_command_parser-2023.4.7/lib/cli_command_parser/parameters/choice_map.py
--rw-rw-rw-   0        0        0    10236 2023-03-31 11:57:05.000000 cli_command_parser-2023.4.7/lib/cli_command_parser/parameters/groups.py
--rw-rw-rw-   0        0        0     6452 2023-03-30 11:44:47.000000 cli_command_parser-2023.4.7/lib/cli_command_parser/parameters/option_strings.py
--rw-rw-rw-   0        0        0    19899 2023-03-30 11:44:47.000000 cli_command_parser-2023.4.7/lib/cli_command_parser/parameters/options.py
--rw-rw-rw-   0        0        0     2039 2022-09-17 20:57:36.000000 cli_command_parser-2023.4.7/lib/cli_command_parser/parameters/pass_thru.py
--rw-rw-rw-   0        0        0     3566 2022-09-17 20:57:36.000000 cli_command_parser-2023.4.7/lib/cli_command_parser/parameters/positionals.py
--rw-rw-rw-   0        0        0    11704 2022-09-19 11:52:48.000000 cli_command_parser-2023.4.7/lib/cli_command_parser/parse_tree.py
--rw-rw-rw-   0        0        0    14238 2022-09-17 20:57:36.000000 cli_command_parser-2023.4.7/lib/cli_command_parser/parser.py
--rw-rw-rw-   0        0        0     9623 2023-04-01 22:51:43.000000 cli_command_parser-2023.4.7/lib/cli_command_parser/testing.py
--rw-rw-rw-   0        0        0     1795 2023-01-14 18:15:47.000000 cli_command_parser-2023.4.7/lib/cli_command_parser/typing.py
--rw-rw-rw-   0        0        0     4548 2023-01-14 20:20:57.000000 cli_command_parser-2023.4.7/lib/cli_command_parser/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-07 12:09:56.427236 cli_command_parser-2023.4.7/lib/cli_command_parser.egg-info/
--rw-rw-rw-   0        0        0     4713 2023-04-07 12:09:56.000000 cli_command_parser-2023.4.7/lib/cli_command_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2314 2023-04-07 12:09:56.000000 cli_command_parser-2023.4.7/lib/cli_command_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 12:09:56.000000 cli_command_parser-2023.4.7/lib/cli_command_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       81 2023-04-07 12:09:56.000000 cli_command_parser-2023.4.7/lib/cli_command_parser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-07 12:09:56.000000 cli_command_parser-2023.4.7/lib/cli_command_parser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      324 2022-09-17 20:57:36.000000 cli_command_parser-2023.4.7/pyproject.toml
--rw-rw-rw-   0        0        0     3483 2023-04-07 12:09:39.000000 cli_command_parser-2023.4.7/readme.rst
--rw-rw-rw-   0        0        0       99 2022-09-17 20:57:36.000000 cli_command_parser-2023.4.7/requirements-dev.txt
--rw-rw-rw-   0        0        0     1333 2023-04-07 12:09:56.514234 cli_command_parser-2023.4.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-08 14:59:10.626959 cli_command_parser-2023.4.8/
+-rw-rw-rw-   0        0        0    11341 2022-09-17 20:57:36.000000 cli_command_parser-2023.4.8/LICENSE
+-rw-rw-rw-   0        0        0       64 2022-09-17 20:57:36.000000 cli_command_parser-2023.4.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     4713 2023-04-08 14:59:10.626959 cli_command_parser-2023.4.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-08 14:59:10.476958 cli_command_parser-2023.4.8/lib/
+drwxrwxrwx   0        0        0        0 2023-04-08 14:59:10.550958 cli_command_parser-2023.4.8/lib/cli_command_parser/
+-rw-rw-rw-   0        0        0     1016 2022-09-17 20:57:36.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/__init__.py
+-rw-rw-rw-   0        0        0      114 2022-09-17 20:57:36.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/__main__.py
+-rw-rw-rw-   0        0        0      295 2023-04-08 14:59:00.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/__version__.py
+-rw-rw-rw-   0        0        0      463 2022-09-17 20:57:36.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/actions.py
+-rw-rw-rw-   0        0        0     3017 2022-10-15 14:00:15.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/annotations.py
+-rw-rw-rw-   0        0        0    19746 2023-03-30 11:44:47.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/command_parameters.py
+-rw-rw-rw-   0        0        0    12491 2023-03-31 11:57:05.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/commands.py
+-rw-rw-rw-   0        0        0     9032 2023-04-08 14:58:49.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/compat.py
+-rw-rw-rw-   0        0        0    15521 2023-04-07 12:09:39.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/config.py
+-rw-rw-rw-   0        0        0    16854 2023-03-30 11:44:47.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/context.py
+drwxrwxrwx   0        0        0        0 2023-04-08 14:59:10.583958 cli_command_parser-2023.4.8/lib/cli_command_parser/conversion/
+-rw-rw-rw-   0        0        0      234 2023-04-06 21:32:03.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/conversion/__init__.py
+-rw-rw-rw-   0        0        0       54 2023-04-06 21:32:03.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/conversion/__main__.py
+-rw-rw-rw-   0        0        0    12802 2023-04-06 21:32:03.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/conversion/argparse_ast.py
+-rw-rw-rw-   0        0        0     1356 2023-04-06 21:32:03.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/conversion/argparse_utils.py
+-rw-rw-rw-   0        0        0    21945 2023-04-08 14:58:49.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/conversion/command_builder.py
+-rw-rw-rw-   0        0        0     1660 2023-04-06 21:32:03.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/conversion/utils.py
+-rw-rw-rw-   0        0        0     7403 2023-04-07 12:09:39.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/conversion/visitor.py
+-rw-rw-rw-   0        0        0     9792 2022-09-24 13:23:00.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/core.py
+-rw-rw-rw-   0        0        0    13416 2023-03-29 11:48:12.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/documentation.py
+-rw-rw-rw-   0        0        0     4800 2022-09-17 20:57:36.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/error_handling.py
+-rw-rw-rw-   0        0        0     7775 2022-11-12 17:12:38.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-08 14:59:10.597958 cli_command_parser-2023.4.8/lib/cli_command_parser/formatting/
+-rw-rw-rw-   0        0        0        0 2022-09-17 20:57:36.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/formatting/__init__.py
+-rw-rw-rw-   0        0        0     6557 2022-09-24 13:23:00.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/formatting/commands.py
+-rw-rw-rw-   0        0        0    20639 2023-04-08 14:58:49.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/formatting/params.py
+-rw-rw-rw-   0        0        0     8572 2022-09-18 21:50:31.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/formatting/restructured_text.py
+-rw-rw-rw-   0        0        0     5440 2023-04-06 21:32:03.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/formatting/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-08 14:59:10.606958 cli_command_parser-2023.4.8/lib/cli_command_parser/inputs/
+-rw-rw-rw-   0        0        0     2125 2023-04-08 14:58:49.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/inputs/__init__.py
+-rw-rw-rw-   0        0        0     1438 2023-04-08 14:58:49.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/inputs/base.py
+-rw-rw-rw-   0        0        0     6313 2022-09-17 20:57:36.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/inputs/choices.py
+-rw-rw-rw-   0        0        0     1113 2023-04-08 14:58:49.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/inputs/exceptions.py
+-rw-rw-rw-   0        0        0     8563 2023-04-08 14:58:49.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/inputs/files.py
+-rw-rw-rw-   0        0        0     7318 2023-04-08 14:58:49.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/inputs/numeric.py
+-rw-rw-rw-   0        0        0    21286 2023-04-08 14:58:49.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/inputs/time.py
+-rw-rw-rw-   0        0        0     6490 2023-01-14 20:20:57.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/inputs/utils.py
+-rw-rw-rw-   0        0        0     8145 2023-01-15 15:08:06.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/metadata.py
+-rw-rw-rw-   0        0        0     6538 2022-09-19 11:52:48.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/nargs.py
+drwxrwxrwx   0        0        0        0 2023-04-08 14:59:10.626959 cli_command_parser-2023.4.8/lib/cli_command_parser/parameters/
+-rw-rw-rw-   0        0        0      300 2022-09-17 20:57:36.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/parameters/__init__.py
+-rw-rw-rw-   0        0        0    25629 2023-04-08 14:58:49.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/parameters/base.py
+-rw-rw-rw-   0        0        0    17128 2022-09-18 21:50:31.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/parameters/choice_map.py
+-rw-rw-rw-   0        0        0    10236 2023-03-31 11:57:05.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/parameters/groups.py
+-rw-rw-rw-   0        0        0     6452 2023-03-30 11:44:47.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/parameters/option_strings.py
+-rw-rw-rw-   0        0        0    19899 2023-03-30 11:44:47.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/parameters/options.py
+-rw-rw-rw-   0        0        0     2039 2022-09-17 20:57:36.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/parameters/pass_thru.py
+-rw-rw-rw-   0        0        0     3566 2022-09-17 20:57:36.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/parameters/positionals.py
+-rw-rw-rw-   0        0        0    11704 2022-09-19 11:52:48.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/parse_tree.py
+-rw-rw-rw-   0        0        0    14238 2022-09-17 20:57:36.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/parser.py
+-rw-rw-rw-   0        0        0     9623 2023-04-01 22:51:43.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/testing.py
+-rw-rw-rw-   0        0        0     1795 2023-01-14 18:15:47.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/typing.py
+-rw-rw-rw-   0        0        0     4548 2023-01-14 20:20:57.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-08 14:59:10.559958 cli_command_parser-2023.4.8/lib/cli_command_parser.egg-info/
+-rw-rw-rw-   0        0        0     4713 2023-04-08 14:59:10.000000 cli_command_parser-2023.4.8/lib/cli_command_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2314 2023-04-08 14:59:10.000000 cli_command_parser-2023.4.8/lib/cli_command_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-08 14:59:10.000000 cli_command_parser-2023.4.8/lib/cli_command_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       81 2023-04-08 14:59:10.000000 cli_command_parser-2023.4.8/lib/cli_command_parser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-08 14:59:10.000000 cli_command_parser-2023.4.8/lib/cli_command_parser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      324 2022-09-17 20:57:36.000000 cli_command_parser-2023.4.8/pyproject.toml
+-rw-rw-rw-   0        0        0     3483 2023-04-07 12:09:39.000000 cli_command_parser-2023.4.8/readme.rst
+-rw-rw-rw-   0        0        0       99 2022-09-17 20:57:36.000000 cli_command_parser-2023.4.8/requirements-dev.txt
+-rw-rw-rw-   0        0        0     1333 2023-04-08 14:59:10.628958 cli_command_parser-2023.4.8/setup.cfg
```

### Comparing `cli_command_parser-2023.4.7/LICENSE` & `cli_command_parser-2023.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.4.7/PKG-INFO` & `cli_command_parser-2023.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli_command_parser
-Version: 2023.4.7
+Version: 2023.4.8
 Summary: CLI Command Parser
 Home-page: https://github.com/dskrypa/cli_command_parser
 Author: Doug Skrypa
 Author-email: dskrypa@gmail.com
 License: Apache 2.0
 Project-URL: Source, https://github.com/dskrypa/cli_command_parser
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cli_command_parser-2023.4.7/lib/cli_command_parser/__init__.py` & `cli_command_parser-2023.4.8/lib/cli_command_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.4.7/lib/cli_command_parser/annotations.py` & `cli_command_parser-2023.4.8/lib/cli_command_parser/annotations.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.4.7/lib/cli_command_parser/command_parameters.py` & `cli_command_parser-2023.4.8/lib/cli_command_parser/command_parameters.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.4.7/lib/cli_command_parser/commands.py` & `cli_command_parser-2023.4.8/lib/cli_command_parser/commands.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.4.7/lib/cli_command_parser/compat.py` & `cli_command_parser-2023.4.8/lib/cli_command_parser/compat.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,21 +7,23 @@
 The :class:`WCTextWrapper` in this module extends the stdlib :class:`python:textwrap.TextWrapper` to support wide
 characters.
 """
 
 from collections.abc import Callable
 from textwrap import TextWrapper
 from threading import RLock
-from typing import List, Generic, _GenericAlias  # noqa
+from typing import List, Generic, _GenericAlias, _SpecialForm  # noqa
 
 try:
     from wcwidth import wcswidth
 except ImportError:
     wcswidth = len
 
+__all__ = ['get_origin', 'cached_property', 'WCTextWrapper', 'Literal']
+
 
 # region typing
 
 
 def get_origin(tp):  # pylint: disable=C0103
     # Copied from 3.8
     if isinstance(tp, _GenericAlias):
@@ -37,14 +39,51 @@
         res = tp.__args__
         if get_origin(tp) is Callable and res[0] is not Ellipsis:
             res = (list(res[:-1]), res[-1])
         return res
     return ()
 
 
+try:
+    from typing import Literal
+except ImportError:  # Python 3.7
+
+    class _LiteralSpecialForm(_SpecialForm, _root=True):
+        def __repr__(self) -> str:
+            return f'compat.{self._name}'
+
+        def __getitem__(self, parameters):
+            if not isinstance(parameters, tuple):
+                parameters = (parameters,)
+            return _GenericAlias(self, parameters)
+
+    _LITERAL_DOCSTRING = """
+    Special typing form to define literal types (a.k.a. value types).
+
+    This form can be used to indicate to type checkers that the corresponding
+    variable or function parameter has a value equivalent to the provided
+    literal (or one of several literals):
+
+      def validate_simple(data: Any) -> Literal[True]:  # always returns True
+          ...
+
+      MODE = Literal['r', 'rb', 'w', 'wb']
+      def open_helper(file: str, mode: MODE) -> str:
+          ...
+
+      open_helper('/some/path', 'r')  # Passes type check
+      open_helper('/other/path', 'typo')  # Error in type checker
+
+    Literal[...] cannot be subclassed. At runtime, an arbitrary value
+    is allowed as type argument to Literal[...], but type checkers may
+    impose restrictions.
+    """
+    Literal = _LiteralSpecialForm('Literal', doc=_LITERAL_DOCSTRING)
+
+
 # endregion
 
 # region functools
 
 
 _NOT_FOUND = object()
```

### Comparing `cli_command_parser-2023.4.7/lib/cli_command_parser/config.py` & `cli_command_parser-2023.4.8/lib/cli_command_parser/config.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.4.7/lib/cli_command_parser/context.py` & `cli_command_parser-2023.4.8/lib/cli_command_parser/context.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.4.7/lib/cli_command_parser/conversion/argparse_ast.py` & `cli_command_parser-2023.4.8/lib/cli_command_parser/conversion/argparse_ast.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.4.7/lib/cli_command_parser/conversion/argparse_utils.py` & `cli_command_parser-2023.4.8/lib/cli_command_parser/conversion/argparse_utils.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.4.7/lib/cli_command_parser/conversion/command_builder.py` & `cli_command_parser-2023.4.8/lib/cli_command_parser/conversion/command_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,29 +54,30 @@
         for converts_cls, converter_cls in cls._ac_converter_map.items():
             if issubclass(ast_obj, converts_cls):
                 return converter_cls
         raise TypeError(f'No Converter is registered for {ast_obj.__class__.__name__} objects')
 
     @classmethod
     def init_group(cls: Type[C], parent: CollectionConverter, ast_objs: List[AC]) -> ConverterGroup[C]:
-        return ConverterGroup(parent, [cls(ast_obj, parent) for ast_obj in ast_objs])
+        return ConverterGroup(parent, cls, [cls(ast_obj, parent) for ast_obj in ast_objs])
 
     def convert(self, indent: int = 0) -> str:
         return '\n'.join(self.format_lines(indent))
 
     @abstractmethod
     def format_lines(self, indent: int = 0) -> Iterator[str]:
         raise NotImplementedError
 
 
 class ConverterGroup(Generic[C]):
-    __slots__ = ('parent', 'members')
+    __slots__ = ('parent', 'member_type', 'members')
 
-    def __init__(self, parent: CollectionConverter, members: List[C]):
+    def __init__(self, parent: CollectionConverter, member_type: Type[C], members: List[C]):
         self.parent = parent
+        self.member_type = member_type
         self.members = members
 
     def __len__(self) -> int:
         return len(self.members)
 
     def __getitem__(self, index: int) -> C:
         return self.members[index]
@@ -121,16 +122,20 @@
             elif hasattr(child_group[0], 'descendant_args'):
                 for child in child_group:
                     yield from child.descendant_args()
             elif isinstance(child_group[0], ParamConverter):
                 yield from child_group
 
     def format_members(self, prefix: str, indent: int = 4) -> Iterator[str]:
+        last = False
         for child_group in self.grouped_children:
+            if last and child_group and issubclass(child_group.member_type, GroupConverter):
+                yield ''
             yield from child_group.format_all(indent)
+            last = bool(child_group)
 
         if not any(cg for cg in self.grouped_children):
             yield f'{prefix}    pass'
 
 
 class ParserConverter(CollectionConverter, converts=AstArgumentParser):
     _auto_gen_disclaimer = '# This is an automatically generated name that should probably be updated'
@@ -148,14 +153,16 @@
     def descendant_args(self) -> Iterator[ParamConverter]:
         yield from super().descendant_args()
         for sp_converter in self.sub_parser_converters:
             yield from sp_converter.descendant_args()
 
     def format_lines(self, indent: int = 0) -> Iterator[str]:
         suffix = f'  {self._auto_gen_disclaimer}' if self.parent is None else ''
+        # TODO: Add _init_command_ and/or main methods
+        # TODO: If subparsers have no unique args, use action methods instead?
         yield '\n'
         yield f'class {self.name}({self._get_args()}):{suffix}'
         yield from self.format_members('')
         for sp_converter in self.sub_parser_converters:
             yield from sp_converter.format_lines()
 
     def _get_args(self) -> str:
@@ -183,26 +190,26 @@
         return self._custom_name or f'Command{next(self.counter)}'
 
     @cached_property
     def _custom_name(self) -> OptStr:
         if not self.is_sub_parser:
             return None
         name = literal_eval_or_none(self.ast_obj.init_func_kwargs.get('name'))
-        if not name or ' ' in name or not name[0].isalpha():
+        if not name or not name[0].isalpha():
             return None
-        return name.title().replace('_', '').replace('-', '')
+        return name.title().replace(' ', '').replace('_', '').replace('-', '')
 
     @cached_property
     def _choices(self) -> Tuple[OptStr, OptStr]:
         if not self.is_sub_parser:
             return None, None
         name = self.ast_obj.init_func_kwargs.get('name')
         aliases = self.ast_obj.init_func_raw_kwargs.get('aliases')
         if not aliases:
-            if name and (not self._custom_name or '-' in name):
+            if name and (not self._custom_name or '-' in name or ' ' in name):
                 return 'choice', name
             return None, None
         elif isinstance(aliases, (Attribute, Name, Subscript, GeneratorExp, DictComp, ListComp, SetComp)):
             value = unparse(aliases)  # noqa
             if name:
                 return 'choices', f'({name}, *{value})'
             return 'choices', (f'tuple{value}' if isinstance(aliases, GeneratorExp) else value)
@@ -234,15 +241,15 @@
 
 
 class GroupConverter(CollectionConverter, converts=ArgGroup):
     ast_obj: ArgGroup
 
     def format_lines(self, indent: int = 4) -> Iterator[str]:
         prefix = ' ' * indent
-        yield f'\n{prefix}with ParamGroup({self._get_args()}):'
+        yield f'{prefix}with ParamGroup({self._get_args()}):'
         yield from self.format_members(prefix, indent + 4)
 
     def _get_args(self) -> str:
         # log.debug(f'Processing args for {self.ast_obj._init_func_bound}')
         description = self.ast_obj.init_func_kwargs.get('description')
         title = self.ast_obj.init_func_kwargs.get('title')
         if title:
@@ -278,15 +285,15 @@
             return True
         if self.is_pass_thru and not other.is_pass_thru:
             return False
         return self.num < other.num
 
     @classmethod
     def init_group(cls, parent: CollectionConverter, args: List[ParserArg]) -> ParamConverterGroup:
-        return ParamConverterGroup(parent, [cls(arg, parent, i) for i, arg in enumerate(args)])
+        return ParamConverterGroup(parent, cls, [cls(arg, parent, i) for i, arg in enumerate(args)])
 
     def format_lines(self, indent: int = 4) -> Iterator[str]:
         yield self.format(indent)
 
     def format(self, indent: int = 4) -> str:
         param_cls, args_obj = self.get_cls_and_kwargs()
         arg_str = args_obj.to_str(*self.get_pos_args())
@@ -361,21 +368,24 @@
 
         if self.is_positional:
             if action and action not in ('store', 'append'):
                 raise ConversionError(f'{self.ast_obj}: action={action!r} is not supported for Positional parameters')
             return 'Positional', ParamArgs.init_positional(action, **kwargs)
         elif self.is_option:
             kwargs['name_mode'] = self.name_mode
+            if not action and 'const' in kwargs:
+                action = 'append_const' if 'nargs' in kwargs else 'store_const'
             if action:
                 if action in ('store_true', 'store_false', 'store_const', 'append_const'):
                     return 'Flag', FlagArgs.init_flag(action, **kwargs)
                 elif action == 'count':
                     return 'Counter', FlagArgs.init_counter(**kwargs)
                 elif action not in ('store', 'append'):
                     raise ConversionError(f'{self.ast_obj}: action={action!r} is not supported for Option parameters')
+
             return 'Option', OptionArgs.init_option(self.ast_obj, action, **kwargs)
 
         raise ConversionError(f'Unable to determine a suitable Parameter type for {self.ast_obj!r}')
 
     # endregion
 
     # region High Level Param Type
@@ -526,41 +536,49 @@
     type: OptStr = None
     nargs: OptStr = None
     choices: OptStr = None
 
     @classmethod
     def init_positional(cls, action: OptStr = None, nargs: OptStr = None, **kwargs):
         if nargs is not None:
-            nargs_obj = Nargs(literal_eval(nargs))
+            parsed = literal_eval_or_none(nargs)
+            if parsed is not None:
+                nargs_obj = Nargs(parsed)
+                if action in ('store', None) and nargs_obj == 1:
+                    action = nargs = None
+            else:
+                nargs_obj = None
         else:
             nargs_obj = Nargs(1)
-        if (action == 'store' and nargs_obj == 1) or (action == 'append' and nargs_obj != Nargs(1)):
+
+        if nargs_obj is not None and action == 'append' and nargs_obj != Nargs(1):
             action = None
         return cls.from_kwargs(action=action, nargs=nargs, **kwargs)
 
 
 @dataclass
 class OptionArgs(ParamArgs):
     name_mode: OptStr = None
 
     @classmethod
     def init_option(cls, arg: ParserArg, action: OptStr = None, nargs: OptStr = None, const: OptStr = None, **kwargs):
         if const:
             log.warning(f'{arg}: ignoring const={const!r} - it is only supported for Flag and Counter parameters')
 
+        if nargs == "'*'":
+            nargs = "'+'"
         if action == 'append':
             if not nargs:
                 log.debug(f"{arg}: using default nargs='+' because action={action!r} and no nargs value was provided")
                 nargs = "'+'"
             action = None
         elif action == 'store':
             if nargs == '1':
                 nargs = None
-            if not nargs:
-                action = None
+            action = None
 
         return cls.from_kwargs(action=repr(action) if action else None, nargs=nargs, **kwargs)
 
 
 @dataclass
 class FlagArgs(OptionArgs):
     const: OptStr = None
```

### Comparing `cli_command_parser-2023.4.7/lib/cli_command_parser/conversion/utils.py` & `cli_command_parser-2023.4.8/lib/cli_command_parser/conversion/utils.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.4.7/lib/cli_command_parser/conversion/visitor.py` & `cli_command_parser-2023.4.8/lib/cli_command_parser/conversion/visitor.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.4.7/lib/cli_command_parser/core.py` & `cli_command_parser-2023.4.8/lib/cli_command_parser/core.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.4.7/lib/cli_command_parser/documentation.py` & `cli_command_parser-2023.4.8/lib/cli_command_parser/documentation.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.4.7/lib/cli_command_parser/error_handling.py` & `cli_command_parser-2023.4.8/lib/cli_command_parser/error_handling.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.4.7/lib/cli_command_parser/exceptions.py` & `cli_command_parser-2023.4.8/lib/cli_command_parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.4.7/lib/cli_command_parser/formatting/commands.py` & `cli_command_parser-2023.4.8/lib/cli_command_parser/formatting/commands.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.4.7/lib/cli_command_parser/formatting/params.py` & `cli_command_parser-2023.4.8/lib/cli_command_parser/formatting/params.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,16 @@
 
 
 class ParamHelpFormatter:
     __slots__ = ('param',)
     _param_cls_fmt_cls_map = {}
     required_formatter_map: BoolFormatterMap = {False: '[{}]'.format}
 
-    def __init_subclass__(cls, param_cls: Type[ParamOrGroup] = None):  # noqa
+    def __init_subclass__(cls, param_cls: Type[ParamOrGroup] = None, **kwargs):
+        super().__init_subclass__(**kwargs)
         if param_cls is not None:
             cls._param_cls_fmt_cls_map[param_cls] = cls
 
     @classmethod
     def for_param_cls(cls, param_cls: Type[ParamOrGroup]):
         try:
             return cls._param_cls_fmt_cls_map[param_cls]
```

### Comparing `cli_command_parser-2023.4.7/lib/cli_command_parser/formatting/restructured_text.py` & `cli_command_parser-2023.4.8/lib/cli_command_parser/formatting/restructured_text.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.4.7/lib/cli_command_parser/formatting/utils.py` & `cli_command_parser-2023.4.8/lib/cli_command_parser/formatting/utils.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.4.7/lib/cli_command_parser/inputs/__init__.py` & `cli_command_parser-2023.4.8/lib/cli_command_parser/inputs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,25 +12,25 @@
 from ..exceptions import ParameterDefinitionError as _ParameterDefinitionError
 from .exceptions import InputValidationError, InvalidChoiceError
 from .utils import StatMode, FileWrapper
 from .base import InputType
 from .choices import Choices, ChoiceMap, EnumChoices
 from .files import Path, File, Serialized, Json, Pickle
 from .numeric import Range, NumRange
-from .time import Day, Month, DateTime, Date, Time, DTFormatMode
+from .time import Day, Month, TimeDelta, DateTime, Date, Time, DTFormatMode
 
 if _t.TYPE_CHECKING:
     from ..typing import TypeFunc, InputTypeFunc, ChoicesType
 
 # fmt: off
 __all__ = [
     'StatMode', 'FileWrapper', 'Path', 'File', 'Serialized', 'Json', 'Pickle',
     'Range', 'NumRange',
     'Choices', 'ChoiceMap', 'EnumChoices',
-    'Day', 'Month', 'DateTime', 'Date', 'Time', 'DTFormatMode',
+    'Day', 'Month', 'TimeDelta', 'DateTime', 'Date', 'Time', 'DTFormatMode',
     'normalize_input_type',
 ]
 # fmt: on
 
 
 def normalize_input_type(type_func: InputTypeFunc, param_choices: ChoicesType) -> _t.Optional[TypeFunc]:
     choices_provided = param_choices is not None
```

### Comparing `cli_command_parser-2023.4.7/lib/cli_command_parser/inputs/base.py` & `cli_command_parser-2023.4.8/lib/cli_command_parser/inputs/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 
 from ..typing import T
 
 __all__ = ['InputType']
 
 
 class InputType(Generic[T], ABC):
+    __slots__ = ()
+
     @abstractmethod
     def __call__(self, value: str) -> T:
         """Process the parsed argument and convert it to the desired type"""
         raise NotImplementedError
 
     def is_valid_type(self, value: str) -> bool:  # pylint: disable=W0613
         """
```

### Comparing `cli_command_parser-2023.4.7/lib/cli_command_parser/inputs/choices.py` & `cli_command_parser-2023.4.8/lib/cli_command_parser/inputs/choices.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.4.7/lib/cli_command_parser/inputs/exceptions.py` & `cli_command_parser-2023.4.8/lib/cli_command_parser/inputs/exceptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,12 +21,13 @@
     def __init__(self, invalid: Any, choices: Collection[Any], type_str: str = 'choice'):  # pylint: disable=W0231
         self.invalid = invalid
         self.choices = choices
         self.type_str = type_str
 
     def __str__(self) -> str:
         if isinstance(self.invalid, Collection) and not isinstance(self.invalid, str):
-            bad_str = '{}s: {}'.format(self.type_str, ', '.join(map(repr, self.invalid)))
+            bad_str = f'{self.type_str}s: {", ".join(map(repr, self.invalid))}'
         else:
             bad_str = f'{self.type_str}: {self.invalid!r}'
+
         choices_str = ', '.join(map(repr, self.choices))
         return f'invalid {bad_str} (choose from: {choices_str})'
```

### Comparing `cli_command_parser-2023.4.7/lib/cli_command_parser/inputs/files.py` & `cli_command_parser-2023.4.8/lib/cli_command_parser/inputs/files.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,18 @@
         self.use_windows_fix = use_windows_fix
 
     def __repr__(self) -> str:
         non_defaults = ', '.join(f'{k}={v!r}' for k, v in self.__dict__.items())
         return f'<{self.__class__.__name__}({non_defaults})>'
 
     def fix_default(self, value: Optional[T]) -> Optional[T]:
+        """
+        Fixes the default value to conform to the expected return type for this input.  Allows the default value for a
+        path to be provided as a string, for example.
+        """
         if value is None:
             return value
         return self(value)
 
     def validated_path(self, path: PathLike) -> _Path:
         if not isinstance(path, _Path):
             path = path.strip()
@@ -88,15 +92,14 @@
             raise ValueError('it is not readable')
         if self.writable and not os.access(path, os.W_OK):
             raise ValueError('it is not writable')
         return path
 
 
 class Path(FileInput[_Path]):
-    # noinspection PyUnresolvedReferences
     """
     :param exists: If set, then the provided path must already exist if True, or must not already exist if False.
       Default: existence is not checked.
     :param expand: Whether tilde (``~``) should be expanded.
     :param resolve: Whether the path should be fully resolved to its absolute path, with symlinks resolved, or not.
     :param type: To restrict the acceptable types of files/directories that are accepted, specify the
       :class:`StatMode` that matches the desired type.  By default, any type is accepted.  To accept specifically
```

### Comparing `cli_command_parser-2023.4.7/lib/cli_command_parser/inputs/numeric.py` & `cli_command_parser-2023.4.8/lib/cli_command_parser/inputs/numeric.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 __all__ = ['Range', 'NumRange']
 
 _range = range
 
 
 class NumericInput(InputType[NT], ABC):
+    __slots__ = ()
     type: NumType
 
     def is_valid_type(self, value: str) -> bool:
         try:
             self.type(value)
         except (ValueError, TypeError):
             return False
@@ -102,14 +103,15 @@
       behavior for handling them in this context.
     :param min: The minimum allowed value, or None to have no lower bound
     :param max: The maximum allowed value, or None to have no upper bound
     :param include_min: Whether the minimum is inclusive (default: True)
     :param include_max: Whether the maximum is inclusive (default: False)
     """
 
+    __slots__ = ('type', 'snap', 'min', 'max', 'include_min', 'include_max')
     snap: bool
     min: Number
     max: Number
     include_min: bool
     include_max: bool
 
     def __init__(
@@ -150,20 +152,20 @@
         self.include_max = include_max
 
     def __repr__(self) -> str:
         return f'<{self.__class__.__name__}({self.type!r}, snap={self.snap!r})[{self._range_str()}]>'
 
     def _range_str(self, var: str = 'N') -> str:
         if self.min is not None:
-            min_str = '{} {} '.format(self.min, '<=' if self.include_min else '<')
+            min_str = f'{self.min} {"<=" if self.include_min else "<"} '
         else:
             min_str = ''
 
         if self.max is not None:
-            max_str = ' {} {}'.format('<=' if self.include_max else '<', self.max)
+            max_str = f' {"<=" if self.include_max else "<"} {self.max}'
         else:
             max_str = ''
 
         return f'{min_str}{var}{max_str}'
 
     def handle_invalid(self, bound: Number, inclusive: bool, snap_dir: int) -> Number:
         """
```

### Comparing `cli_command_parser-2023.4.7/lib/cli_command_parser/inputs/time.py` & `cli_command_parser-2023.4.8/lib/cli_command_parser/inputs/time.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,23 +21,29 @@
 from datetime import datetime, date, time, timedelta
 from enum import Enum
 from locale import LC_ALL, setlocale
 from threading import RLock
 from typing import Union, Iterator, Collection, Sequence, Optional, TypeVar, Type, overload
 from typing import Tuple, Dict
 
+try:
+    from typing import Literal
+except ImportError:
+    from ..compat import Literal
+
 from ..typing import T, Bool, Locale, TimeBound
 from ..utils import MissingMixin
 from .base import InputType
 from .exceptions import InputValidationError, InvalidChoiceError
 
-__all__ = ['DTFormatMode', 'Day', 'Month', 'DateTime', 'Date', 'Time']
+__all__ = ['DTFormatMode', 'Day', 'Month', 'TimeDelta', 'DateTime', 'Date', 'Time']
 
 DT = TypeVar('DT')
-
+TimeUnit = Literal['days', 'seconds', 'microseconds', 'milliseconds', 'minutes', 'hours', 'weeks']
+_TIMEDELTA_UNITS = {'days', 'seconds', 'microseconds', 'milliseconds', 'minutes', 'hours', 'weeks'}
 DEFAULT_DATE_FMT = '%Y-%m-%d'
 DEFAULT_TIME_FMT = '%H:%M:%S'
 DEFAULT_DT_FMT = '%Y-%m-%d %H:%M:%S'
 
 
 class different_locale:
     """
@@ -70,18 +76,23 @@
     def __exit__(self, exc_type, exc_val, exc_tb):
         if self.locale:
             setlocale(LC_ALL, self.original)
         self._lock.release()
 
 
 class DTInput(InputType[T], ABC):
+    __slots__ = ('locale',)
     dt_type: str
     locale: Optional[Locale]
 
-    def __init_subclass__(cls, dt_type: str = None):  # noqa
+    def __init_subclass__(cls, dt_type: str = None, **kwargs):
+        """
+        :param dt_type: Used in InvalidChoiceError / ValueError messages
+        """
+        super().__init_subclass__(**kwargs)
         cls.dt_type = dt_type
 
     def __init__(self, locale: Locale = None):
         self.locale = locale
 
     @abstractmethod
     def choice_str(self, choice_delim: str = ',', sort_choices: bool = False) -> str:
@@ -100,14 +111,15 @@
     FULL = 'full'                   #: The full name of a given date/time unit
     ABBREVIATION = 'abbreviation'   #: The abbreviation of a given date/time unit
     NUMERIC = 'numeric'             #: The numeric representation of a given date/time unit
     NUMERIC_ISO = 'numeric_iso'     #: The ISO numeric representation of a given date/time unit
 
 
 class CalendarUnitInput(DTInput[Union[str, int]], ABC):
+    __slots__ = ('full', 'abbreviation', 'numeric', 'out_format', 'out_locale')
     _formats: Dict[DTFormatMode, Sequence[Union[str, int]]]
     _min_index: int = 0
 
     def __init_subclass__(cls, min_index: int = 0, **kwargs):
         super().__init_subclass__(**kwargs)
         cls._min_index = min_index
 
@@ -216,14 +228,15 @@
             with different_locale(self.out_locale):
                 return names_or_abbreviations[normalized]
 
         raise ValueError(f'Unexpected output format={out_mode!r} for {self.dt_type}={normalized}')
 
 
 class Day(CalendarUnitInput, dt_type='day of the week'):
+    __slots__ = ('iso',)
     _formats = {
         DTFormatMode.FULL: day_name,
         DTFormatMode.ABBREVIATION: day_abbr,
         DTFormatMode.NUMERIC: range(7),
         DTFormatMode.NUMERIC_ISO: range(1, 8),
     }
 
@@ -271,14 +284,15 @@
             raise InputValidationError(
                 f'Invalid weekday={dow_num} - expected a value'
                 f' between {start} ({day_name[0]}) and {stop} ({day_name[6]})'
             )
 
 
 class Month(CalendarUnitInput, dt_type='month', min_index=1):
+    __slots__ = ()
     _formats = {
         DTFormatMode.FULL: month_name,
         DTFormatMode.ABBREVIATION: month_abbr,
         DTFormatMode.NUMERIC: range(13),
     }
 
     @overload
@@ -321,25 +335,55 @@
                 f'Invalid month={month} - expected a value between 1 ({month_name[1]}) and 12 ({month_name[12]})'
             )
 
 
 # endregion
 
 
+class TimeDelta(InputType[timedelta]):
+    __slots__ = ('unit',)
+
+    def __init__(self, unit: TimeUnit):
+        unit = unit.lower()
+        if unit not in _TIMEDELTA_UNITS:
+            raise TypeError(f'Invalid unit={unit!r} - expected one of: {", ".join(sorted(_TIMEDELTA_UNITS))}')
+        self.unit = unit
+        # TODO: min/max params like NumRange?
+
+    def __call__(self, value: Union[str, int, float]) -> timedelta:
+        if isinstance(value, str):
+            try:
+                value = float(value.replace(',', '').replace('_', ''))  # allow comma or _ between thousands
+            except ValueError as e:
+                raise InputValidationError(
+                    f'Invalid numeric {self.unit}={value!r} - expected an integer or float'
+                ) from e
+
+        return timedelta(**{self.unit: value})
+
+    def fix_default(self, value: Union[int, float, timedelta, None]) -> Optional[timedelta]:
+        if value is None or isinstance(value, timedelta):
+            return value
+        return self(value)
+
+    def format_metavar(self, choice_delim: str = ',', sort_choices: bool = False) -> str:
+        return f'{{{self.unit}}}'
+
+
 # region Date/Time Parse Inputs
 
 
 class DateTimeInput(DTInput[DT], ABC):
     formats: Collection[str]
     _type: Type[DT]
     _earliest: TimeBound = None
     _latest: TimeBound = None
 
-    def __init_subclass__(cls, type: Type[DT]):  # noqa
-        super().__init_subclass__(dt_type=type.__name__)
+    def __init_subclass__(cls, type: Type[DT], **kwargs):  # noqa
+        super().__init_subclass__(dt_type=type.__name__, **kwargs)
         cls._type = type
 
     def __init__(
         self, formats: Collection[str], locale: Locale = None, earliest: TimeBound = None, latest: TimeBound = None
     ):
         super().__init__(locale=locale)
         self.formats = formats
```

### Comparing `cli_command_parser-2023.4.7/lib/cli_command_parser/inputs/utils.py` & `cli_command_parser-2023.4.8/lib/cli_command_parser/inputs/utils.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.4.7/lib/cli_command_parser/metadata.py` & `cli_command_parser-2023.4.8/lib/cli_command_parser/metadata.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.4.7/lib/cli_command_parser/nargs.py` & `cli_command_parser-2023.4.8/lib/cli_command_parser/nargs.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.4.7/lib/cli_command_parser/parameters/base.py` & `cli_command_parser-2023.4.8/lib/cli_command_parser/parameters/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -219,23 +219,24 @@
     # Instance attributes with class defaults
     metavar: str = None
     nargs: Nargs = Nargs(1)                         # Set in subclasses
     type: Optional[Callable[[str], T_co]] = None    # Only set here if not set by __init__ in Option/Positional
     show_default: bool = None
 
     def __init_subclass__(
-        cls, accepts_values: bool = None, accepts_none: bool = None, repr_attrs: Collection[str] = None
+        cls, accepts_values: bool = None, accepts_none: bool = None, repr_attrs: Collection[str] = None, **kwargs
     ):
         """
         :param accepts_values: Indicates whether a given subclass of Parameter accepts values, or not.  :class:`.Flag`
           is an example of a class that does not accept values.
         :param accepts_none: Indicates whether a given subclass of Parameter accepts being specified without a value,
           like :class:`.Flag` and :class:`.Counter`.
         :param repr_attrs: Additional attributes to include in the repr.
         """
+        super().__init_subclass__(**kwargs)
         actions = set(cls._actions)  # Inherit actions from parent
         actions.update(getattr(cls, '_BasicActionMixin__actions', ()))  # Inherit from mixin, if present
         try:
             actions.update(getattr(cls, f'_{cls.__name__}__actions'))
         except AttributeError:
             pass
         else:
```

### Comparing `cli_command_parser-2023.4.7/lib/cli_command_parser/parameters/choice_map.py` & `cli_command_parser-2023.4.8/lib/cli_command_parser/parameters/choice_map.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.4.7/lib/cli_command_parser/parameters/groups.py` & `cli_command_parser-2023.4.8/lib/cli_command_parser/parameters/groups.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.4.7/lib/cli_command_parser/parameters/option_strings.py` & `cli_command_parser-2023.4.8/lib/cli_command_parser/parameters/option_strings.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.4.7/lib/cli_command_parser/parameters/options.py` & `cli_command_parser-2023.4.8/lib/cli_command_parser/parameters/options.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.4.7/lib/cli_command_parser/parameters/pass_thru.py` & `cli_command_parser-2023.4.8/lib/cli_command_parser/parameters/pass_thru.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.4.7/lib/cli_command_parser/parameters/positionals.py` & `cli_command_parser-2023.4.8/lib/cli_command_parser/parameters/positionals.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.4.7/lib/cli_command_parser/parse_tree.py` & `cli_command_parser-2023.4.8/lib/cli_command_parser/parse_tree.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.4.7/lib/cli_command_parser/parser.py` & `cli_command_parser-2023.4.8/lib/cli_command_parser/parser.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.4.7/lib/cli_command_parser/testing.py` & `cli_command_parser-2023.4.8/lib/cli_command_parser/testing.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.4.7/lib/cli_command_parser/typing.py` & `cli_command_parser-2023.4.8/lib/cli_command_parser/typing.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.4.7/lib/cli_command_parser/utils.py` & `cli_command_parser-2023.4.8/lib/cli_command_parser/utils.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.4.7/lib/cli_command_parser.egg-info/PKG-INFO` & `cli_command_parser-2023.4.8/lib/cli_command_parser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli-command-parser
-Version: 2023.4.7
+Version: 2023.4.8
 Summary: CLI Command Parser
 Home-page: https://github.com/dskrypa/cli_command_parser
 Author: Doug Skrypa
 Author-email: dskrypa@gmail.com
 License: Apache 2.0
 Project-URL: Source, https://github.com/dskrypa/cli_command_parser
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cli_command_parser-2023.4.7/lib/cli_command_parser.egg-info/SOURCES.txt` & `cli_command_parser-2023.4.8/lib/cli_command_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.4.7/readme.rst` & `cli_command_parser-2023.4.8/readme.rst`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.4.7/setup.cfg` & `cli_command_parser-2023.4.8/setup.cfg`

 * *Files identical despite different names*

