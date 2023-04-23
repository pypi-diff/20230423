# Comparing `tmp/mash-shell-0.2.4.tar.gz` & `tmp/mash-shell-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mash-shell-0.2.4.tar", last modified: Sat Apr 15 12:08:04 2023, max compression
+gzip compressed data, was "mash-shell-0.2.5.tar", last modified: Sun Apr 23 19:27:43 2023, max compression
```

## Comparing `mash-shell-0.2.4.tar` & `mash-shell-0.2.5.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-15 12:08:04.576626 mash-shell-0.2.4/
--rw-r--r--   0 mark       (501) staff       (20)    35149 2022-11-28 19:29:51.000000 mash-shell-0.2.4/LICENSE
--rw-r--r--   0 mark       (501) staff       (20)     8540 2023-04-15 12:08:04.576160 mash-shell-0.2.4/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)     7972 2023-04-15 12:07:40.000000 mash-shell-0.2.4/README.md
--rw-r--r--   0 mark       (501) staff       (20)      736 2023-04-15 12:05:55.000000 mash-shell-0.2.4/pyproject.toml
--rw-r--r--   0 mark       (501) staff       (20)      161 2023-03-18 10:23:14.000000 mash-shell-0.2.4/requirements.txt
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-04-15 12:08:04.576732 mash-shell-0.2.4/setup.cfg
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-15 12:08:04.532470 mash-shell-0.2.4/src/
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-15 12:08:04.539770 mash-shell-0.2.4/src/examples/
--rw-r--r--   0 mark       (501) staff       (20)       91 2023-03-18 13:42:50.000000 mash-shell-0.2.4/src/examples/_extend_path.py
--rwxr-xr-x   0 mark       (501) staff       (20)     2059 2023-03-18 13:42:50.000000 mash-shell-0.2.4/src/examples/discoverable.py
--rwxr-xr-x   0 mark       (501) staff       (20)      965 2023-03-22 06:58:11.000000 mash-shell-0.2.4/src/examples/discoverable_api.py
--rw-r--r--   0 mark       (501) staff       (20)     1004 2023-04-08 06:46:34.000000 mash-shell-0.2.4/src/examples/discoverable_with_oas.py
--rwxr-xr-x   0 mark       (501) staff       (20)      785 2023-03-18 13:42:50.000000 mash-shell-0.2.4/src/examples/filesystem.py
--rw-r--r--   0 mark       (501) staff       (20)     1126 2023-03-24 06:51:08.000000 mash-shell-0.2.4/src/examples/ms_graph_api.py
--rwxr-xr-x   0 mark       (501) staff       (20)     3477 2023-03-18 13:42:50.000000 mash-shell-0.2.4/src/examples/object_parser.py
--rwxr-xr-x   0 mark       (501) staff       (20)     1324 2023-04-11 19:57:54.000000 mash-shell-0.2.4/src/examples/shell_example.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-15 12:08:04.549569 mash-shell-0.2.4/src/mash/
--rw-r--r--   0 mark       (501) staff       (20)       43 2023-03-18 13:42:50.000000 mash-shell-0.2.4/src/mash/__main__.py
--rwxr-xr-x   0 mark       (501) staff       (20)     2209 2023-03-18 14:32:23.000000 mash-shell-0.2.4/src/mash/cli.py
--rw-r--r--   0 mark       (501) staff       (20)     2479 2023-04-11 19:57:54.000000 mash-shell-0.2.4/src/mash/doc_inference.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-15 12:08:04.553050 mash-shell-0.2.4/src/mash/filesystem/
--rw-r--r--   0 mark       (501) staff       (20)      121 2023-03-18 13:42:50.000000 mash-shell-0.2.4/src/mash/filesystem/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)     6953 2023-04-11 19:57:54.000000 mash-shell-0.2.4/src/mash/filesystem/discoverable.py
--rw-r--r--   0 mark       (501) staff       (20)    10629 2023-04-10 07:54:42.000000 mash-shell-0.2.4/src/mash/filesystem/filesystem.py
--rw-r--r--   0 mark       (501) staff       (20)     3252 2023-03-18 14:32:23.000000 mash-shell-0.2.4/src/mash/filesystem/scope.py
--rw-r--r--   0 mark       (501) staff       (20)     4627 2023-03-24 08:15:55.000000 mash-shell-0.2.4/src/mash/filesystem/view.py
--rw-r--r--   0 mark       (501) staff       (20)     3455 2023-03-18 13:42:50.000000 mash-shell-0.2.4/src/mash/html_table.py
--rw-r--r--   0 mark       (501) staff       (20)     2048 2023-03-18 13:42:50.000000 mash-shell-0.2.4/src/mash/html_table_data.py
--rw-r--r--   0 mark       (501) staff       (20)     5161 2023-03-24 07:32:34.000000 mash-shell-0.2.4/src/mash/io_util.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-15 12:08:04.556437 mash-shell-0.2.4/src/mash/object_parser/
--rw-r--r--   0 mark       (501) staff       (20)      733 2023-03-18 13:42:50.000000 mash-shell-0.2.4/src/mash/object_parser/errors.py
--rw-r--r--   0 mark       (501) staff       (20)     8289 2023-03-18 13:42:50.000000 mash-shell-0.2.4/src/mash/object_parser/factory.py
--rw-r--r--   0 mark       (501) staff       (20)     4505 2023-03-18 13:42:50.000000 mash-shell-0.2.4/src/mash/object_parser/oas.py
--rw-r--r--   0 mark       (501) staff       (20)     1727 2023-03-18 14:24:14.000000 mash-shell-0.2.4/src/mash/object_parser/object_parser.py
--rw-r--r--   0 mark       (501) staff       (20)     1129 2023-03-18 13:42:50.000000 mash-shell-0.2.4/src/mash/object_parser/object_parser_standards.py
--rw-r--r--   0 mark       (501) staff       (20)     4322 2023-03-18 13:42:50.000000 mash-shell-0.2.4/src/mash/object_parser/spec.py
--rwxr-xr-x   0 mark       (501) staff       (20)      574 2023-03-18 13:42:50.000000 mash-shell-0.2.4/src/mash/object_parser_server.py
--rw-r--r--   0 mark       (501) staff       (20)     8032 2023-03-18 13:42:50.000000 mash-shell-0.2.4/src/mash/parallel.py
--rw-r--r--   0 mark       (501) staff       (20)     4176 2023-03-18 13:42:50.000000 mash-shell-0.2.4/src/mash/parallel_requests.py
--rw-r--r--   0 mark       (501) staff       (20)     9208 2023-03-18 13:42:50.000000 mash-shell-0.2.4/src/mash/pipeline.py
--rw-r--r--   0 mark       (501) staff       (20)      230 2023-03-18 13:42:50.000000 mash-shell-0.2.4/src/mash/progress_bar.py
--rw-r--r--   0 mark       (501) staff       (20)     2761 2023-03-18 13:42:50.000000 mash-shell-0.2.4/src/mash/server.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-15 12:08:04.560509 mash-shell-0.2.4/src/mash/shell/
--rw-r--r--   0 mark       (501) staff       (20)      215 2023-04-11 19:57:54.000000 mash-shell-0.2.4/src/mash/shell/__init__.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-15 12:08:04.565784 mash-shell-0.2.4/src/mash/shell/ast/
--rw-r--r--   0 mark       (501) staff       (20)      880 2023-04-15 11:14:26.000000 mash-shell-0.2.4/src/mash/shell/ast/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)     4686 2023-04-15 11:49:14.000000 mash-shell-0.2.4/src/mash/shell/ast/conditions.py
--rw-r--r--   0 mark       (501) staff       (20)     1740 2023-04-15 11:25:14.000000 mash-shell-0.2.4/src/mash/shell/ast/function_definition.py
--rw-r--r--   0 mark       (501) staff       (20)     5572 2023-04-15 11:49:14.000000 mash-shell-0.2.4/src/mash/shell/ast/infix.py
--rw-r--r--   0 mark       (501) staff       (20)     4735 2023-04-15 11:49:14.000000 mash-shell-0.2.4/src/mash/shell/ast/node.py
--rw-r--r--   0 mark       (501) staff       (20)     2799 2023-04-15 11:49:14.000000 mash-shell-0.2.4/src/mash/shell/ast/nodes.py
--rw-r--r--   0 mark       (501) staff       (20)     3158 2023-04-15 11:49:14.000000 mash-shell-0.2.4/src/mash/shell/ast/term.py
--rw-r--r--   0 mark       (501) staff       (20)    10999 2023-04-15 11:22:15.000000 mash-shell-0.2.4/src/mash/shell/base.py
--rw-r--r--   0 mark       (501) staff       (20)     6330 2023-04-15 10:44:24.000000 mash-shell-0.2.4/src/mash/shell/cmd2.py
--rw-r--r--   0 mark       (501) staff       (20)      136 2023-03-18 14:32:23.000000 mash-shell-0.2.4/src/mash/shell/errors.py
--rw-r--r--   0 mark       (501) staff       (20)     2139 2023-04-15 11:49:00.000000 mash-shell-0.2.4/src/mash/shell/function.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-15 12:08:04.568200 mash-shell-0.2.4/src/mash/shell/grammer/
--rw-r--r--   0 mark       (501) staff       (20)     1018 2023-04-15 08:36:37.000000 mash-shell-0.2.4/src/mash/shell/grammer/delimiters.py
--rw-r--r--   0 mark       (501) staff       (20)    13517 2023-04-15 11:21:14.000000 mash-shell-0.2.4/src/mash/shell/grammer/lex_yacc.py
--rw-r--r--   0 mark       (501) staff       (20)    24815 2023-04-15 11:17:58.000000 mash-shell-0.2.4/src/mash/shell/grammer/parsetab.py
--rw-r--r--   0 mark       (501) staff       (20)     4085 2023-04-15 11:21:01.000000 mash-shell-0.2.4/src/mash/shell/grammer/parsing.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-15 12:08:04.569401 mash-shell-0.2.4/src/mash/shell/internals/
--rw-r--r--   0 mark       (501) staff       (20)     4570 2023-04-15 11:49:14.000000 mash-shell-0.2.4/src/mash/shell/internals/helpers.py
--rw-r--r--   0 mark       (501) staff       (20)     2348 2023-04-15 11:24:38.000000 mash-shell-0.2.4/src/mash/shell/internals/if_statement.py
--rw-r--r--   0 mark       (501) staff       (20)    24815 2023-04-10 18:49:45.000000 mash-shell-0.2.4/src/mash/shell/parsetab.py
--rwxr-xr-x   0 mark       (501) staff       (20)    11586 2023-04-15 11:49:14.000000 mash-shell-0.2.4/src/mash/shell/shell.py
--rw-r--r--   0 mark       (501) staff       (20)     6367 2023-04-11 19:57:54.000000 mash-shell-0.2.4/src/mash/shell/with_filesystem.py
--rw-r--r--   0 mark       (501) staff       (20)     3223 2023-04-15 11:46:06.000000 mash-shell-0.2.4/src/mash/subshell.py
--rw-r--r--   0 mark       (501) staff       (20)    18188 2023-04-11 18:51:45.000000 mash-shell-0.2.4/src/mash/util.py
--rw-r--r--   0 mark       (501) staff       (20)     4024 2023-03-18 13:42:50.000000 mash-shell-0.2.4/src/mash/verify_server.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-15 12:08:04.572121 mash-shell-0.2.4/src/mash_shell.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)     8540 2023-04-15 12:08:04.000000 mash-shell-0.2.4/src/mash_shell.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)     1984 2023-04-15 12:08:04.000000 mash-shell-0.2.4/src/mash_shell.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-04-15 12:08:04.000000 mash-shell-0.2.4/src/mash_shell.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)      161 2023-04-15 12:08:04.000000 mash-shell-0.2.4/src/mash_shell.egg-info/requires.txt
--rw-r--r--   0 mark       (501) staff       (20)       18 2023-04-15 12:08:04.000000 mash-shell-0.2.4/src/mash_shell.egg-info/top_level.txt
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-15 12:08:04.575610 mash-shell-0.2.4/test/
--rw-r--r--   0 mark       (501) staff       (20)      822 2022-12-04 19:37:35.000000 mash-shell-0.2.4/test/test_html_table.py
--rw-r--r--   0 mark       (501) staff       (20)     1106 2023-03-18 14:17:38.000000 mash-shell-0.2.4/test/test_parallel.py
--rw-r--r--   0 mark       (501) staff       (20)    10304 2023-03-18 14:16:22.000000 mash-shell-0.2.4/test/test_pipeline.py
--rw-r--r--   0 mark       (501) staff       (20)     4054 2023-03-18 14:32:23.000000 mash-shell-0.2.4/test/test_server.py
--rw-r--r--   0 mark       (501) staff       (20)     8153 2022-12-11 09:47:43.000000 mash-shell-0.2.4/test/test_util.py
--rw-r--r--   0 mark       (501) staff       (20)     2500 2022-12-04 19:39:10.000000 mash-shell-0.2.4/test/test_verify_server.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-23 19:27:43.193546 mash-shell-0.2.5/
+-rw-r--r--   0 mark       (501) staff       (20)    35149 2022-11-28 19:29:51.000000 mash-shell-0.2.5/LICENSE
+-rw-r--r--   0 mark       (501) staff       (20)     8824 2023-04-23 19:27:43.192740 mash-shell-0.2.5/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)     8256 2023-04-23 07:49:30.000000 mash-shell-0.2.5/README.md
+-rw-r--r--   0 mark       (501) staff       (20)      736 2023-04-23 19:27:30.000000 mash-shell-0.2.5/pyproject.toml
+-rw-r--r--   0 mark       (501) staff       (20)      161 2023-03-18 10:23:14.000000 mash-shell-0.2.5/requirements.txt
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-04-23 19:27:43.193709 mash-shell-0.2.5/setup.cfg
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-23 19:27:43.099550 mash-shell-0.2.5/src/
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-23 19:27:43.111259 mash-shell-0.2.5/src/examples/
+-rw-r--r--   0 mark       (501) staff       (20)       91 2023-03-18 13:42:50.000000 mash-shell-0.2.5/src/examples/_extend_path.py
+-rwxr-xr-x   0 mark       (501) staff       (20)     2059 2023-03-18 13:42:50.000000 mash-shell-0.2.5/src/examples/discoverable.py
+-rwxr-xr-x   0 mark       (501) staff       (20)      965 2023-03-22 06:58:11.000000 mash-shell-0.2.5/src/examples/discoverable_api.py
+-rw-r--r--   0 mark       (501) staff       (20)     1019 2023-04-23 07:55:55.000000 mash-shell-0.2.5/src/examples/discoverable_with_oas.py
+-rwxr-xr-x   0 mark       (501) staff       (20)      785 2023-03-18 13:42:50.000000 mash-shell-0.2.5/src/examples/filesystem.py
+-rw-r--r--   0 mark       (501) staff       (20)     1126 2023-03-24 06:51:08.000000 mash-shell-0.2.5/src/examples/ms_graph_api.py
+-rwxr-xr-x   0 mark       (501) staff       (20)     3477 2023-03-18 13:42:50.000000 mash-shell-0.2.5/src/examples/object_parser.py
+-rwxr-xr-x   0 mark       (501) staff       (20)     1324 2023-04-11 19:57:54.000000 mash-shell-0.2.5/src/examples/shell_example.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-23 19:27:43.127605 mash-shell-0.2.5/src/mash/
+-rw-r--r--   0 mark       (501) staff       (20)       43 2023-03-18 13:42:50.000000 mash-shell-0.2.5/src/mash/__main__.py
+-rwxr-xr-x   0 mark       (501) staff       (20)     2209 2023-03-18 14:32:23.000000 mash-shell-0.2.5/src/mash/cli.py
+-rw-r--r--   0 mark       (501) staff       (20)     2479 2023-04-11 19:57:54.000000 mash-shell-0.2.5/src/mash/doc_inference.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-23 19:27:43.134285 mash-shell-0.2.5/src/mash/filesystem/
+-rw-r--r--   0 mark       (501) staff       (20)      121 2023-03-18 13:42:50.000000 mash-shell-0.2.5/src/mash/filesystem/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)     6953 2023-04-15 12:12:40.000000 mash-shell-0.2.5/src/mash/filesystem/discoverable.py
+-rw-r--r--   0 mark       (501) staff       (20)    10642 2023-04-23 06:48:12.000000 mash-shell-0.2.5/src/mash/filesystem/filesystem.py
+-rw-r--r--   0 mark       (501) staff       (20)     3252 2023-03-18 14:32:23.000000 mash-shell-0.2.5/src/mash/filesystem/scope.py
+-rw-r--r--   0 mark       (501) staff       (20)     4662 2023-04-23 08:14:44.000000 mash-shell-0.2.5/src/mash/filesystem/view.py
+-rw-r--r--   0 mark       (501) staff       (20)     3455 2023-03-18 13:42:50.000000 mash-shell-0.2.5/src/mash/html_table.py
+-rw-r--r--   0 mark       (501) staff       (20)     2048 2023-03-18 13:42:50.000000 mash-shell-0.2.5/src/mash/html_table_data.py
+-rw-r--r--   0 mark       (501) staff       (20)     5161 2023-03-24 07:32:34.000000 mash-shell-0.2.5/src/mash/io_util.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-23 19:27:43.141885 mash-shell-0.2.5/src/mash/object_parser/
+-rw-r--r--   0 mark       (501) staff       (20)      733 2023-03-18 13:42:50.000000 mash-shell-0.2.5/src/mash/object_parser/errors.py
+-rw-r--r--   0 mark       (501) staff       (20)     8289 2023-03-18 13:42:50.000000 mash-shell-0.2.5/src/mash/object_parser/factory.py
+-rw-r--r--   0 mark       (501) staff       (20)     4505 2023-03-18 13:42:50.000000 mash-shell-0.2.5/src/mash/object_parser/oas.py
+-rw-r--r--   0 mark       (501) staff       (20)     1727 2023-03-18 14:24:14.000000 mash-shell-0.2.5/src/mash/object_parser/object_parser.py
+-rw-r--r--   0 mark       (501) staff       (20)     1129 2023-03-18 13:42:50.000000 mash-shell-0.2.5/src/mash/object_parser/object_parser_standards.py
+-rw-r--r--   0 mark       (501) staff       (20)     4322 2023-03-18 13:42:50.000000 mash-shell-0.2.5/src/mash/object_parser/spec.py
+-rwxr-xr-x   0 mark       (501) staff       (20)      574 2023-03-18 13:42:50.000000 mash-shell-0.2.5/src/mash/object_parser_server.py
+-rw-r--r--   0 mark       (501) staff       (20)     8032 2023-03-18 13:42:50.000000 mash-shell-0.2.5/src/mash/parallel.py
+-rw-r--r--   0 mark       (501) staff       (20)     4176 2023-03-18 13:42:50.000000 mash-shell-0.2.5/src/mash/parallel_requests.py
+-rw-r--r--   0 mark       (501) staff       (20)     9208 2023-03-18 13:42:50.000000 mash-shell-0.2.5/src/mash/pipeline.py
+-rw-r--r--   0 mark       (501) staff       (20)      230 2023-03-18 13:42:50.000000 mash-shell-0.2.5/src/mash/progress_bar.py
+-rw-r--r--   0 mark       (501) staff       (20)     2761 2023-03-18 13:42:50.000000 mash-shell-0.2.5/src/mash/server.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-23 19:27:43.150903 mash-shell-0.2.5/src/mash/shell/
+-rw-r--r--   0 mark       (501) staff       (20)      215 2023-04-11 19:57:54.000000 mash-shell-0.2.5/src/mash/shell/__init__.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-23 19:27:43.161655 mash-shell-0.2.5/src/mash/shell/ast/
+-rw-r--r--   0 mark       (501) staff       (20)      880 2023-04-15 11:14:26.000000 mash-shell-0.2.5/src/mash/shell/ast/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)     4686 2023-04-15 11:49:14.000000 mash-shell-0.2.5/src/mash/shell/ast/conditions.py
+-rw-r--r--   0 mark       (501) staff       (20)     1740 2023-04-15 11:25:14.000000 mash-shell-0.2.5/src/mash/shell/ast/function_definition.py
+-rw-r--r--   0 mark       (501) staff       (20)     5723 2023-04-23 08:24:39.000000 mash-shell-0.2.5/src/mash/shell/ast/infix.py
+-rw-r--r--   0 mark       (501) staff       (20)     4735 2023-04-15 11:49:14.000000 mash-shell-0.2.5/src/mash/shell/ast/node.py
+-rw-r--r--   0 mark       (501) staff       (20)     2738 2023-04-23 08:25:52.000000 mash-shell-0.2.5/src/mash/shell/ast/nodes.py
+-rw-r--r--   0 mark       (501) staff       (20)     3158 2023-04-23 06:48:12.000000 mash-shell-0.2.5/src/mash/shell/ast/term.py
+-rw-r--r--   0 mark       (501) staff       (20)    10985 2023-04-16 15:55:13.000000 mash-shell-0.2.5/src/mash/shell/base.py
+-rw-r--r--   0 mark       (501) staff       (20)     6330 2023-04-15 10:44:24.000000 mash-shell-0.2.5/src/mash/shell/cmd2.py
+-rw-r--r--   0 mark       (501) staff       (20)      136 2023-03-18 14:32:23.000000 mash-shell-0.2.5/src/mash/shell/errors.py
+-rw-r--r--   0 mark       (501) staff       (20)     2139 2023-04-15 11:49:00.000000 mash-shell-0.2.5/src/mash/shell/function.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-23 19:27:43.172328 mash-shell-0.2.5/src/mash/shell/grammer/
+-rw-r--r--   0 mark       (501) staff       (20)      965 2023-04-16 15:54:19.000000 mash-shell-0.2.5/src/mash/shell/grammer/delimiters.py
+-rw-r--r--   0 mark       (501) staff       (20)    13347 2023-04-23 07:07:47.000000 mash-shell-0.2.5/src/mash/shell/grammer/lex_yacc.py
+-rw-r--r--   0 mark       (501) staff       (20)    24815 2023-04-15 11:17:58.000000 mash-shell-0.2.5/src/mash/shell/grammer/parsetab.py
+-rw-r--r--   0 mark       (501) staff       (20)     4272 2023-04-23 07:21:26.000000 mash-shell-0.2.5/src/mash/shell/grammer/parsing.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-23 19:27:43.177254 mash-shell-0.2.5/src/mash/shell/internals/
+-rw-r--r--   0 mark       (501) staff       (20)     4570 2023-04-15 11:49:14.000000 mash-shell-0.2.5/src/mash/shell/internals/helpers.py
+-rw-r--r--   0 mark       (501) staff       (20)     2348 2023-04-15 11:24:38.000000 mash-shell-0.2.5/src/mash/shell/internals/if_statement.py
+-rw-r--r--   0 mark       (501) staff       (20)    24815 2023-04-10 18:49:45.000000 mash-shell-0.2.5/src/mash/shell/parsetab.py
+-rwxr-xr-x   0 mark       (501) staff       (20)    11208 2023-04-23 07:36:36.000000 mash-shell-0.2.5/src/mash/shell/shell.py
+-rw-r--r--   0 mark       (501) staff       (20)     6593 2023-04-23 08:15:29.000000 mash-shell-0.2.5/src/mash/shell/with_filesystem.py
+-rw-r--r--   0 mark       (501) staff       (20)     3223 2023-04-15 11:46:06.000000 mash-shell-0.2.5/src/mash/subshell.py
+-rw-r--r--   0 mark       (501) staff       (20)    18188 2023-04-11 18:51:45.000000 mash-shell-0.2.5/src/mash/util.py
+-rw-r--r--   0 mark       (501) staff       (20)     4024 2023-03-18 13:42:50.000000 mash-shell-0.2.5/src/mash/verify_server.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-23 19:27:43.180965 mash-shell-0.2.5/src/mash_shell.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)     8824 2023-04-23 19:27:43.000000 mash-shell-0.2.5/src/mash_shell.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)     1984 2023-04-23 19:27:43.000000 mash-shell-0.2.5/src/mash_shell.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-04-23 19:27:43.000000 mash-shell-0.2.5/src/mash_shell.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)      161 2023-04-23 19:27:43.000000 mash-shell-0.2.5/src/mash_shell.egg-info/requires.txt
+-rw-r--r--   0 mark       (501) staff       (20)       18 2023-04-23 19:27:43.000000 mash-shell-0.2.5/src/mash_shell.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-23 19:27:43.191671 mash-shell-0.2.5/test/
+-rw-r--r--   0 mark       (501) staff       (20)      822 2022-12-04 19:37:35.000000 mash-shell-0.2.5/test/test_html_table.py
+-rw-r--r--   0 mark       (501) staff       (20)     1106 2023-03-18 14:17:38.000000 mash-shell-0.2.5/test/test_parallel.py
+-rw-r--r--   0 mark       (501) staff       (20)    10304 2023-03-18 14:16:22.000000 mash-shell-0.2.5/test/test_pipeline.py
+-rw-r--r--   0 mark       (501) staff       (20)     4054 2023-03-18 14:32:23.000000 mash-shell-0.2.5/test/test_server.py
+-rw-r--r--   0 mark       (501) staff       (20)     8153 2022-12-11 09:47:43.000000 mash-shell-0.2.5/test/test_util.py
+-rw-r--r--   0 mark       (501) staff       (20)     2500 2022-12-04 19:39:10.000000 mash-shell-0.2.5/test/test_verify_server.py
```

### Comparing `mash-shell-0.2.4/LICENSE` & `mash-shell-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.4/PKG-INFO` & `mash-shell-0.2.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mash-shell
-Version: 0.2.4
+Version: 0.2.5
 Summary: A shell and other utils
 Author-email: voschezang <mark.voschezang@student.uva.nl>
 Project-URL: Homepage, https://github.com/voschezang/mash
 Project-URL: Bug Tracker, https://github.com/voschezang/mash/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: System :: Shells
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -97,16 +97,16 @@
 
 ## Filesystem (CRUD Operations)
 
 See `examples/filesystem.py` and `examples/discoverable.py`.
 
 | Example             | Description                                                  |
 | ------------------- | ------------------------------------------------------------ |
-| `ls [PATH]`         | List the items in a directory. Use the current working directory by default. Alias: `list` |
-| `cd`, `use [PATH]`  | Change the current working directory. Alias: `use`           |
+| `list [PATH]`       | List the items in a directory. Use the current working directory by default. Alias: `l` |
+| `cd [PATH]`         | Change the current working directory. Alias: `use`           |
 | `get NAME`          | Retrieve a file.                                             |
 | `set NAME VALUE`    | Modify a file.                                               |
 | `new NAME [NAME..]` | Create new directories.                                      |
 | `show [NAME]`       | Display detailed information about a directory.              |
 | `cp`, `mv`, `rm`    | Modify files. I.e. copy, move, rename or remove files.       |
 | `home [PATH]`       | Set home directory.                                          |
 | `reset`             | Refresh cached values.                                       |
@@ -210,14 +210,29 @@
 department_750, department_14
 ```
 
 
 
 # Library & Tools
 
+Repository structure
+
+```sh
+src
+├── examples
+├── lib # mash shell scripts
+└── mash
+    ├── filesystem # Directory-based datastructures: FileSystem, View
+    ├── object_parser # Parse JSON objects
+    └── shell # Shell, ShellWithFileSystem
+test
+```
+
+
+
 ## Setup
 
 Using a `Makefile` for convenience.
 
 ```sh
 make install
 make test
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mash-shell Version: 0.2.4 Summary: A shell and
+Metadata-Version: 2.1 Name: mash-shell Version: 0.2.5 Summary: A shell and
 other utils Author-email: voschezang
 voschezang@student.uva.nl> Project-URL: Homepage, https://github.com/
 voschezang/mash Project-URL: Bug Tracker, https://github.com/voschezang/mash/
 issues Classifier: Programming Language :: Python :: 3 Classifier: Topic ::
 System :: Shells Classifier: License :: OSI Approved :: GNU General Public
 License v3 (GPLv3) Classifier: Operating System :: OS Independent Requires-
 Python: >=3.10 Description-Content-Type: text/markdown License-File: LICENSE !
@@ -46,21 +46,21 @@
 arguments: cmd A comma- or newline-separated list of commands optional
 arguments: -h, --help show this help message and exit -v, --verbose -s, --safe
 Safe-mode. Ask for confirmation before executing commands. -f FILE, --file FILE
 Read and run FILE as a commands -r, --reload Reload last session --session
 SESSION Use session SESSION ``` ## Filesystem (CRUD Operations) See `examples/
 filesystem.py` and `examples/discoverable.py`. | Example | Description | | ----
 --------------- | -----------------------------------------------------------
-- | | `ls [PATH]` | List the items in a directory. Use the current working
-directory by default. Alias: `list` | | `cd`, `use [PATH]` | Change the current
-working directory. Alias: `use` | | `get NAME` | Retrieve a file. | | `set NAME
-VALUE` | Modify a file. | | `new NAME [NAME..]` | Create new directories. | |
-`show [NAME]` | Display detailed information about a directory. | | `cp`, `mv`,
-`rm` | Modify files. I.e. copy, move, rename or remove files. | | `home [PATH]`
-| Set home directory. | | `reset` | Refresh cached values. | ## Usage Examples
+- | | `list [PATH]` | List the items in a directory. Use the current working
+directory by default. Alias: `l` | | `cd [PATH]` | Change the current working
+directory. Alias: `use` | | `get NAME` | Retrieve a file. | | `set NAME VALUE`
+| Modify a file. | | `new NAME [NAME..]` | Create new directories. | | `show
+[NAME]` | Display detailed information about a directory. | | `cp`, `mv`, `rm`
+| Modify files. I.e. copy, move, rename or remove files. | | `home [PATH]` |
+Set home directory. | | `reset` | Refresh cached values. | ## Usage Examples
 For real-world examples, see [lib](https://github.com/voschezang/mash/blob/
 main/src/lib/math.sh). ### Example 1 See `src/shell_example.py`. It shows how
 to use a user-definnable mapping of custom functions. It uses the library `quo`
 to create a user-friendly subshell with autocompletion prompts. ```sh # py src/
 shell.py echo hello, echo world hello world ``` ```sh # py src/shell_example.py
 Welcome. Type help or ? to list commands. $ ? Documented commands (type help ):
 ======================================== e example f g h help ls shell $ help g
@@ -79,21 +79,24 @@
 'aquatic', 'penquins': [{'name': 'tux'}]} ]}]} ``` ```sh # note the
 autocompletion $ python src/examples/filesystem.py 'cd world; cd a; cd t; cd
 snakes; ll' python cobra ``` ### With Dynamic Data See `examples/
 discoverable.py`. ```sh # list remote/auto-generated data $ python src/
 examples/discoverable.py 'ls' department_805, department_399 # refresh data,
 then save $ py src/examples/discoverable.py 'ls ; save' department_750,
 department_14 # reload data $ python src/examples/discoverable.py 'ls'
-department_750, department_14 ``` # Library & Tools ## Setup Using a `Makefile`
-for convenience. ```sh make install make test ``` ## Parallelization Utilities
-Some experiments with parallelization, concurrency and `asyncio` in Python. ###
-Test Start a dummy server. ```sh python3 src/server.py ``` Do a simple load
-test ```sh python3 src/parallel.py -v ``` ## Object Parser - [src/
-object_parser/object_parser.py](object_parser.py) parses JSON data and
-instantiate Python objects. - [src/object_parser/oas.py](oas.py) converts
-domain-models to OAS. ### Example ```sh python src/object_parser_example.py ```
-[OAS Example] ### REST API Server ```sh python src/object_parser_server.py ```
-Client ```sh curl -X 'POST' 'http://localhost:5000/v1/organizations' \ -
-H 'Content-Type: application/json' \ -d '{ "board": [ "string" ], "ceo":
-"string", "departments": [ { "manager": "string", "teams": [ { "manager":
-"string", "members": [ "string" ], "team_type": "A", "active": true,
-"capacity": 0, "value": 0 } ] } ] }' ```
+department_750, department_14 ``` # Library & Tools Repository structure ```sh
+src âââ examples âââ lib # mash shell scripts âââ mash
+âââ filesystem # Directory-based datastructures: FileSystem, View
+âââ object_parser # Parse JSON objects âââ shell # Shell,
+ShellWithFileSystem test ``` ## Setup Using a `Makefile` for convenience. ```sh
+make install make test ``` ## Parallelization Utilities Some experiments with
+parallelization, concurrency and `asyncio` in Python. ### Test Start a dummy
+server. ```sh python3 src/server.py ``` Do a simple load test ```sh python3
+src/parallel.py -v ``` ## Object Parser - [src/object_parser/object_parser.py]
+(object_parser.py) parses JSON data and instantiate Python objects. - [src/
+object_parser/oas.py](oas.py) converts domain-models to OAS. ### Example ```sh
+python src/object_parser_example.py ``` [OAS Example] ### REST API Server ```sh
+python src/object_parser_server.py ``` Client ```sh curl -X 'POST' 'http://
+localhost:5000/v1/organizations' \ -H 'Content-Type: application/json' \ -d '
+{ "board": [ "string" ], "ceo": "string", "departments": [ { "manager":
+"string", "teams": [ { "manager": "string", "members": [ "string" ],
+"team_type": "A", "active": true, "capacity": 0, "value": 0 } ] } ] }' ```
```

### Comparing `mash-shell-0.2.4/README.md` & `mash-shell-0.2.5/src/mash_shell.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: mash-shell
+Version: 0.2.5
+Summary: A shell and other utils
+Author-email: voschezang <mark.voschezang@student.uva.nl>
+Project-URL: Homepage, https://github.com/voschezang/mash
+Project-URL: Bug Tracker, https://github.com/voschezang/mash/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: System :: Shells
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ![workflow-badge](https://github.com/voschezang/mash/actions/workflows/python-app.yml/badge.svg)
 <a href="https://pypi.org/project/mash-shell" title="Python versions"><img src="https://img.shields.io/badge/python-3.8%20|%203.10%20|%203.11-blue"/></a>
 <a href="https://pypi.org/project/mash-shell" title="PyPI"><img src="https://img.shields.io/badge/pypi-v0.2.0-blue"/></a>
 
 
 **Docs**:
 [MAIN](https://github.com/voschezang/mash/blob/main/README.md) 
@@ -82,16 +97,16 @@
 
 ## Filesystem (CRUD Operations)
 
 See `examples/filesystem.py` and `examples/discoverable.py`.
 
 | Example             | Description                                                  |
 | ------------------- | ------------------------------------------------------------ |
-| `ls [PATH]`         | List the items in a directory. Use the current working directory by default. Alias: `list` |
-| `cd`, `use [PATH]`  | Change the current working directory. Alias: `use`           |
+| `list [PATH]`       | List the items in a directory. Use the current working directory by default. Alias: `l` |
+| `cd [PATH]`         | Change the current working directory. Alias: `use`           |
 | `get NAME`          | Retrieve a file.                                             |
 | `set NAME VALUE`    | Modify a file.                                               |
 | `new NAME [NAME..]` | Create new directories.                                      |
 | `show [NAME]`       | Display detailed information about a directory.              |
 | `cp`, `mv`, `rm`    | Modify files. I.e. copy, move, rename or remove files.       |
 | `home [PATH]`       | Set home directory.                                          |
 | `reset`             | Refresh cached values.                                       |
@@ -195,14 +210,29 @@
 department_750, department_14
 ```
 
 
 
 # Library & Tools
 
+Repository structure
+
+```sh
+src
+├── examples
+├── lib # mash shell scripts
+└── mash
+    ├── filesystem # Directory-based datastructures: FileSystem, View
+    ├── object_parser # Parse JSON objects
+    └── shell # Shell, ShellWithFileSystem
+test
+```
+
+
+
 ## Setup
 
 Using a `Makefile` for convenience.
 
 ```sh
 make install
 make test
```

#### html2text {}

```diff
@@ -1,8 +1,16 @@
-![workflow-badge](https://github.com/voschezang/mash/actions/workflows/python-
+Metadata-Version: 2.1 Name: mash-shell Version: 0.2.5 Summary: A shell and
+other utils Author-email: voschezang
+voschezang@student.uva.nl> Project-URL: Homepage, https://github.com/
+voschezang/mash Project-URL: Bug Tracker, https://github.com/voschezang/mash/
+issues Classifier: Programming Language :: Python :: 3 Classifier: Topic ::
+System :: Shells Classifier: License :: OSI Approved :: GNU General Public
+License v3 (GPLv3) Classifier: Operating System :: OS Independent Requires-
+Python: >=3.10 Description-Content-Type: text/markdown License-File: LICENSE !
+[workflow-badge](https://github.com/voschezang/mash/actions/workflows/python-
 app.yml/badge.svg) [https://img.shields.io/badge/python-
 3.8%20|%203.10%20|%203.11-blue] [https://img.shields.io/badge/pypi-v0.2.0-blue]
 **Docs**: [MAIN](https://github.com/voschezang/mash/blob/main/README.md) |
 [SHELL.md](https://github.com/voschezang/mash/blob/main/SHELL.md) |
 [REFERENCE.md](https://github.com/voschezang/mash/blob/main/SHELL_REFERENCE.md)
 [A drawing of a terminal] # Mash | My Automation Shell A *shell* that can be
 used to for automation and (REST) resource discovery. It can be used as a [cli]
@@ -38,21 +46,21 @@
 arguments: cmd A comma- or newline-separated list of commands optional
 arguments: -h, --help show this help message and exit -v, --verbose -s, --safe
 Safe-mode. Ask for confirmation before executing commands. -f FILE, --file FILE
 Read and run FILE as a commands -r, --reload Reload last session --session
 SESSION Use session SESSION ``` ## Filesystem (CRUD Operations) See `examples/
 filesystem.py` and `examples/discoverable.py`. | Example | Description | | ----
 --------------- | -----------------------------------------------------------
-- | | `ls [PATH]` | List the items in a directory. Use the current working
-directory by default. Alias: `list` | | `cd`, `use [PATH]` | Change the current
-working directory. Alias: `use` | | `get NAME` | Retrieve a file. | | `set NAME
-VALUE` | Modify a file. | | `new NAME [NAME..]` | Create new directories. | |
-`show [NAME]` | Display detailed information about a directory. | | `cp`, `mv`,
-`rm` | Modify files. I.e. copy, move, rename or remove files. | | `home [PATH]`
-| Set home directory. | | `reset` | Refresh cached values. | ## Usage Examples
+- | | `list [PATH]` | List the items in a directory. Use the current working
+directory by default. Alias: `l` | | `cd [PATH]` | Change the current working
+directory. Alias: `use` | | `get NAME` | Retrieve a file. | | `set NAME VALUE`
+| Modify a file. | | `new NAME [NAME..]` | Create new directories. | | `show
+[NAME]` | Display detailed information about a directory. | | `cp`, `mv`, `rm`
+| Modify files. I.e. copy, move, rename or remove files. | | `home [PATH]` |
+Set home directory. | | `reset` | Refresh cached values. | ## Usage Examples
 For real-world examples, see [lib](https://github.com/voschezang/mash/blob/
 main/src/lib/math.sh). ### Example 1 See `src/shell_example.py`. It shows how
 to use a user-definnable mapping of custom functions. It uses the library `quo`
 to create a user-friendly subshell with autocompletion prompts. ```sh # py src/
 shell.py echo hello, echo world hello world ``` ```sh # py src/shell_example.py
 Welcome. Type help or ? to list commands. $ ? Documented commands (type help ):
 ======================================== e example f g h help ls shell $ help g
@@ -71,21 +79,24 @@
 'aquatic', 'penquins': [{'name': 'tux'}]} ]}]} ``` ```sh # note the
 autocompletion $ python src/examples/filesystem.py 'cd world; cd a; cd t; cd
 snakes; ll' python cobra ``` ### With Dynamic Data See `examples/
 discoverable.py`. ```sh # list remote/auto-generated data $ python src/
 examples/discoverable.py 'ls' department_805, department_399 # refresh data,
 then save $ py src/examples/discoverable.py 'ls ; save' department_750,
 department_14 # reload data $ python src/examples/discoverable.py 'ls'
-department_750, department_14 ``` # Library & Tools ## Setup Using a `Makefile`
-for convenience. ```sh make install make test ``` ## Parallelization Utilities
-Some experiments with parallelization, concurrency and `asyncio` in Python. ###
-Test Start a dummy server. ```sh python3 src/server.py ``` Do a simple load
-test ```sh python3 src/parallel.py -v ``` ## Object Parser - [src/
-object_parser/object_parser.py](object_parser.py) parses JSON data and
-instantiate Python objects. - [src/object_parser/oas.py](oas.py) converts
-domain-models to OAS. ### Example ```sh python src/object_parser_example.py ```
-[OAS Example] ### REST API Server ```sh python src/object_parser_server.py ```
-Client ```sh curl -X 'POST' 'http://localhost:5000/v1/organizations' \ -
-H 'Content-Type: application/json' \ -d '{ "board": [ "string" ], "ceo":
-"string", "departments": [ { "manager": "string", "teams": [ { "manager":
-"string", "members": [ "string" ], "team_type": "A", "active": true,
-"capacity": 0, "value": 0 } ] } ] }' ```
+department_750, department_14 ``` # Library & Tools Repository structure ```sh
+src âââ examples âââ lib # mash shell scripts âââ mash
+âââ filesystem # Directory-based datastructures: FileSystem, View
+âââ object_parser # Parse JSON objects âââ shell # Shell,
+ShellWithFileSystem test ``` ## Setup Using a `Makefile` for convenience. ```sh
+make install make test ``` ## Parallelization Utilities Some experiments with
+parallelization, concurrency and `asyncio` in Python. ### Test Start a dummy
+server. ```sh python3 src/server.py ``` Do a simple load test ```sh python3
+src/parallel.py -v ``` ## Object Parser - [src/object_parser/object_parser.py]
+(object_parser.py) parses JSON data and instantiate Python objects. - [src/
+object_parser/oas.py](oas.py) converts domain-models to OAS. ### Example ```sh
+python src/object_parser_example.py ``` [OAS Example] ### REST API Server ```sh
+python src/object_parser_server.py ``` Client ```sh curl -X 'POST' 'http://
+localhost:5000/v1/organizations' \ -H 'Content-Type: application/json' \ -d '
+{ "board": [ "string" ], "ceo": "string", "departments": [ { "manager":
+"string", "teams": [ { "manager": "string", "members": [ "string" ],
+"team_type": "A", "active": true, "capacity": 0, "value": 0 } ] } ] }' ```
```

### Comparing `mash-shell-0.2.4/pyproject.toml` & `mash-shell-0.2.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mash-shell"
-version = "0.2.4"
+version = "0.2.5"
 authors = [
   { name="voschezang", email="mark.voschezang@student.uva.nl" },
 ]
 description = "A shell and other utils"
 dynamic = ["dependencies"]
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `mash-shell-0.2.4/src/examples/discoverable.py` & `mash-shell-0.2.5/src/examples/discoverable.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.4/src/examples/discoverable_api.py` & `mash-shell-0.2.5/src/examples/discoverable_api.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.4/src/examples/discoverable_with_oas.py` & `mash-shell-0.2.5/src/examples/discoverable_with_oas.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,29 +7,34 @@
 from mash.filesystem.discoverable import observe
 from mash.object_parser.factory import JSONFactory
 from mash.object_parser.oas import OAS, path_create
 from mash.shell import ShellWithFileSystem
 
 from examples.discoverable import Organization
 
-if __name__ == '__main__':
+
+def main() -> str:
     shell = ShellWithFileSystem(data={'repository': Organization},
                                 get_value_method=observe)
     obj = shell.repository
     result = obj.ll()
     obj.init_home(['repository'])
 
     path = []
     result = 'departments'
 
-    # for i in range(7):
-    for i in range(7):
+    for i in range(6):
         key = result.split('\n')[-1]
         path.append(key)
         result = obj.ll(*path)
 
-    json = JSONFactory(Organization).build(obj['repository'])
+    json = JSONFactory(Organization).build(obj)
     oas = OAS()
     oas.extend(json)
     oas['servers'] = [{'url': 'http://localhost:5000/v1'}]
     oas['paths']['/organizations'] = path_create('Organization')
+    return oas
+
+
+if __name__ == '__main__':
+    oas = main()
     print(dumps(oas))
```

### Comparing `mash-shell-0.2.4/src/examples/filesystem.py` & `mash-shell-0.2.5/src/examples/filesystem.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.4/src/examples/ms_graph_api.py` & `mash-shell-0.2.5/src/examples/ms_graph_api.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.4/src/examples/object_parser.py` & `mash-shell-0.2.5/src/examples/object_parser.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.4/src/examples/shell_example.py` & `mash-shell-0.2.5/src/examples/shell_example.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.4/src/mash/cli.py` & `mash-shell-0.2.5/src/mash/cli.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.4/src/mash/doc_inference.py` & `mash-shell-0.2.5/src/mash/doc_inference.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.4/src/mash/filesystem/discoverable.py` & `mash-shell-0.2.5/src/mash/filesystem/discoverable.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.4/src/mash/filesystem/filesystem.py` & `mash-shell-0.2.5/src/mash/filesystem/filesystem.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 #!/usr/bin/python3
-"""A filesystem-like interface for static and dynamic data.
-This can be used to e.g. browse REST APIs.
-"""
 from contextlib import contextmanager
 from enum import Enum
 from pickle import dumps, loads
 from pprint import pformat
 from typing import Callable, Iterable, List, Tuple, Union
 
 from mash.util import accumulate_list, first, has_method, is_Dict_or_List, none
@@ -34,14 +31,18 @@
         return True
 
 
 OPTIONS = [o.value for o in Option]
 
 
 class FileSystem:
+    """A filesystem-like interface for static and dynamic data.
+    This can be used to e.g. browse REST APIs.
+    """
+
     def __init__(self,
                  root: dict = None,
                  home: Path = None,
                  get_hook: Callable[[Key, View], Key] = first,
                  post_cd_hook: Callable = none,
                  **dict_kwds):
```

### Comparing `mash-shell-0.2.4/src/mash/filesystem/scope.py` & `mash-shell-0.2.5/src/mash/filesystem/scope.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.4/src/mash/filesystem/view.py` & `mash-shell-0.2.5/src/mash/filesystem/view.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 Data = Union[dict, list]
 Trace = List[Tuple[Key, Data]]
 Path = List[Union[List[str], str]]
 
 NAME = 'name'
 
 
+class ViewError(ValueError):
+    pass
+
+
 @dataclass
 class View:
     """A tree of dict's. Tree traversal is exposed through the methods `up` and `down`.
     """
     tree: Data
     _trace: Trace = field(default_factory=list)
 
@@ -70,15 +74,15 @@
 
         return range(len(self.tree))
 
     def cp(self, *references: Key):
         *sources, dst = references
 
         if not sources:
-            raise ValueError(
+            raise ViewError(
                 f'At least two arguments are required, but got {references}')
         elif len(sources) == 1:
             src = sources[0]
             self.tree[dst] = self.tree[src]
         else:
             if dst not in self.tree or self.tree[dst] is None:
                 self.tree[dst] = {}
@@ -134,32 +138,32 @@
             if k not in self.tree:
                 keys = self.ls()
                 k = next(find_prefix_matches(str(k), keys))
 
             return k, self.tree[k]
 
         except (KeyError, ValueError):
-            raise ValueError(self._file_not_found(k))
+            raise ViewError(self._file_not_found(k))
 
     def _get_from_list(self, k):
         # convert key to an index
         i = self.infer_index(k)
 
         try:
             return i, self.tree[i]
         except (IndexError, KeyError):
-            raise ValueError(self._file_not_found(k))
+            raise ViewError(self._file_not_found(k))
 
     def _file_not_found(self, k):
         preview_items = (crop(str(s), 10) for s in take(self.ls(), 5))
         preview = crop(', '.join(preview_items), 80)
         return f'No such file or directory: `{k}` not in [{preview}, ..]'
 
 
 def verify_directory(value, name: str):
     error = f'{name} is not a directory'
     if isinstance(value, str) or is_Dict_or_List(value):
-        raise ValueError(error)
+        raise ViewError(error)
     try:
         'some_key' in value
     except TypeError:
-        raise ValueError(error)
+        raise ViewError(error)
```

### Comparing `mash-shell-0.2.4/src/mash/html_table.py` & `mash-shell-0.2.5/src/mash/html_table.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.4/src/mash/html_table_data.py` & `mash-shell-0.2.5/src/mash/html_table_data.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.4/src/mash/io_util.py` & `mash-shell-0.2.5/src/mash/io_util.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.4/src/mash/object_parser/errors.py` & `mash-shell-0.2.5/src/mash/object_parser/errors.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.4/src/mash/object_parser/factory.py` & `mash-shell-0.2.5/src/mash/object_parser/factory.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.4/src/mash/object_parser/oas.py` & `mash-shell-0.2.5/src/mash/object_parser/oas.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.4/src/mash/object_parser/object_parser.py` & `mash-shell-0.2.5/src/mash/object_parser/object_parser.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.4/src/mash/object_parser/object_parser_standards.py` & `mash-shell-0.2.5/src/mash/object_parser/object_parser_standards.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.4/src/mash/object_parser/spec.py` & `mash-shell-0.2.5/src/mash/object_parser/spec.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.4/src/mash/object_parser_server.py` & `mash-shell-0.2.5/src/mash/object_parser_server.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.4/src/mash/parallel.py` & `mash-shell-0.2.5/src/mash/parallel.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.4/src/mash/parallel_requests.py` & `mash-shell-0.2.5/src/mash/parallel_requests.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.4/src/mash/pipeline.py` & `mash-shell-0.2.5/src/mash/pipeline.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.4/src/mash/server.py` & `mash-shell-0.2.5/src/mash/server.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.4/src/mash/shell/ast/__init__.py` & `mash-shell-0.2.5/src/mash/shell/ast/__init__.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.4/src/mash/shell/ast/conditions.py` & `mash-shell-0.2.5/src/mash/shell/ast/conditions.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.4/src/mash/shell/ast/function_definition.py` & `mash-shell-0.2.5/src/mash/shell/ast/function_definition.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.4/src/mash/shell/ast/infix.py` & `mash-shell-0.2.5/src/mash/shell/ast/infix.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from typing import Iterable
 
 from mash.shell.ast.node import Math, Node, run_shell_command
 from mash.shell.ast.nodes import Terms
-from mash.shell.ast.term import Term
+from mash.shell.ast.term import Quoted, Term
 from mash.shell.base import BaseShell
+from mash.shell.errors import ShellError, ShellSyntaxError
 from mash.shell.function import LAST_RESULTS, LAST_RESULTS_INDEX
 from mash.shell.grammer.delimiters import comparators, FALSE, TRUE
-from mash.shell.grammer.parsing import quote_items, to_bool
+from mash.shell.grammer.parsing import quote_items, quote_return_value, to_bool
 from mash.shell.internals.helpers import set_env_variables
 from mash.util import quote_all
 
 
 ################################################################################
 # Infix Operator Expressions
 ################################################################################
@@ -80,15 +81,15 @@
             return
         return k, self.op, values
 
 
 class BinaryExpression(Infix):
     def run(self, prev_result='', shell: BaseShell = None, lazy=False):
         if prev_result not in (TRUE, FALSE):
-            raise NotImplementedError('prev_result was not empty')
+            raise ShellError('Not implemented: prev_result was not empty')
 
         op = self.op
         a = shell.run_commands(self.lhs, run=not lazy)
         b = shell.run_commands(self.rhs, run=not lazy)
 
         line = ' '.join(quote_items([a, op, b]))
 
@@ -151,28 +152,31 @@
         println a b |> map echo
         println a b |> map echo prefix $ suffix
         ```
         """
         # monadic bind
         # https://en.wikipedia.org/wiki/Monad_(functional_programming)
 
-        items = shell.parse(values).values
+        try:
+            items = shell.parse(values).values
+        except ShellSyntaxError:
+            items = [Quoted(values)]
 
         results = []
         for i, item in enumerate(items):
             shell.env[LAST_RESULTS_INDEX] = i
 
             results.append(shell.run_commands(command, item, run=True))
 
         shell.env[LAST_RESULTS_INDEX] = 0
-        agg = delimiter.join(str(r) for r in results)
-        if agg.strip() == '':
+        out = delimiter.join(str(r) for r in results)
+        if out.strip() == '':
             return ''
 
-        return delimiter.join(quote_all(results))
+        return out
 
 
 class LogicExpression(Infix):
     def run(self, prev_result='', shell: BaseShell = None, lazy=False):
         a = shell.run_commands(self.lhs, run=not lazy)
         b = shell.run_commands(self.rhs, run=not lazy)
         if not lazy:
```

### Comparing `mash-shell-0.2.4/src/mash/shell/ast/node.py` & `mash-shell-0.2.5/src/mash/shell/ast/node.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.4/src/mash/shell/ast/nodes.py` & `mash-shell-0.2.5/src/mash/shell/ast/nodes.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,32 +26,32 @@
         self.extend(nodes)
         return self
 
     def extend(self, nodes: Node):
         self._values += nodes.values
 
     def __eq__(self, other):
-        return self.values == other.values and type(self) == type(other)
+        try:
+            return self.values == other.values and type(self) == type(other)
+        except AttributeError:
+            return False
 
     @property
     def data(self) -> str:
         return ' '.join(str(v) for v in self.values)
 
 
 class Terms(Nodes):
     def run(self, prev_result='', shell: BaseShell = None, lazy=False):
         items = self.values
 
         if len(items) >= 2 and not lazy:
             k, *args = items
             # TODO add "prefix" class, instead of this hack for infix operators
-            if k == 'foreach':
-                args = Terms(list(args))
-                return shell._do_foreach(args, prev_result)
-            elif k in ['reduce', 'foldr']:
+            if k in ['reduce', 'foldr']:
                 return shell.foldr(args, prev_result)
 
         return Term.run_terms(items, prev_result, shell, lazy)
 
 
 class Lines(Nodes):
     def run(self, prev_result='', shell: BaseShell = None, lazy=False):
```

### Comparing `mash-shell-0.2.4/src/mash/shell/ast/term.py` & `mash-shell-0.2.5/src/mash/shell/ast/term.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.4/src/mash/shell/base.py` & `mash-shell-0.2.5/src/mash/shell/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         self.locals.set(IF, [])
         self.locals.set(ENV, {})
 
     @property
     def delimiters(self):
         """Return the most recent values of the delimiters.
         """
-        items = delimiters.python + delimiters.bash
+        items = delimiters.all.copy()
         items.remove('=')
         items.remove('#')
         return items
 
     @property
     def _last_if(self):
         return self.locals[IF][-1]
```

### Comparing `mash-shell-0.2.4/src/mash/shell/cmd2.py` & `mash-shell-0.2.5/src/mash/shell/cmd2.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.4/src/mash/shell/function.py` & `mash-shell-0.2.5/src/mash/shell/function.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.4/src/mash/shell/grammer/delimiters.py` & `mash-shell-0.2.5/src/mash/shell/grammer/delimiters.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,11 +38,7 @@
 THEN = Python.THEN.value
 ELSE = Python.ELSE.value
 ELSE_IF_THEN = 'else-if-then'
 
 INLINE_THEN = 'inline-then'
 INLINE_ELSE = 'inline-else'
 
-
-class KeyWords(Enum):
-    AND = 'and'
-    OR = 'or'
```

### Comparing `mash-shell-0.2.4/src/mash/shell/grammer/lex_yacc.py` & `mash-shell-0.2.5/src/mash/shell/grammer/lex_yacc.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,22 +76,14 @@
         r'\('
         return t
 
     def t_RPAREN(t):
         r'\)'
         return t
 
-    # def t_LBRACE(t):
-    #     r'\{'
-    #     return t
-
-    # def t_RBRACE(t):
-    #     r'\}'
-    #     return t
-
     def t_BREAK(t):
         r'[\n\r]|((\;)+[\ \t]*)'
         # semicolon_with_whitespace = r'((\;)+[ \t]*)'
         # newlines = r'(\n+)'
 
         # TOOD if not ;
         t.lexer.lineno += len(t.value)
@@ -198,15 +190,14 @@
         return t
 
     def t_SYMBOL(t):
         r'[\~\+\*\-%&.]+'
         return t
 
     def t_error(t):
-        print(f'Illegal character: `{t.value[0]}`')
         t.lexer.skip(1)
         raise ShellSyntaxError(f'Illegal character: `{t.value[0]}`')
 
     return lex.lex()
 
 
 def tokenize(data: str):
```

### Comparing `mash-shell-0.2.4/src/mash/shell/grammer/parsetab.py` & `mash-shell-0.2.5/src/mash/shell/grammer/parsetab.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.4/src/mash/shell/grammer/parsing.py` & `mash-shell-0.2.5/src/mash/shell/grammer/parsing.py`

 * *Files 4% similar despite different names*

```diff
@@ -130,7 +130,14 @@
 def inline_indent_with(*indent_per_type) -> float:
     for i in indent_per_type:
         if i > 80:
             raise NotImplementedError(f'Indent too large: {i}')
 
     values = ''.join(f'{k:080}' for k in indent_per_type)
     return str('.' + ''.join(values))
+
+
+def quote_return_value(value: str, delimiter='\n') -> str:
+    ignore = list('*!?@<>+')
+    if delimiter in ignore:
+        ignore.remove(delimiter)
+    return quote_all(value, ignore)
```

### Comparing `mash-shell-0.2.4/src/mash/shell/internals/helpers.py` & `mash-shell-0.2.5/src/mash/shell/internals/helpers.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.4/src/mash/shell/internals/if_statement.py` & `mash-shell-0.2.5/src/mash/shell/internals/if_statement.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.4/src/mash/shell/parsetab.py` & `mash-shell-0.2.5/src/mash/shell/parsetab.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.4/src/mash/shell/shell.py` & `mash-shell-0.2.5/src/mash/shell/shell.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,26 +176,14 @@
         if len(items) < 2:
             raise ShellError('Expected multiple arguments')
 
         f, *args = items
         for arg in args:
             self.onecmd(f'{f} {arg}')
 
-    def _do_foreach(self, ast: tuple, prev_results: str) -> Iterable:
-        """Apply a function to every term or word.
-
-        Usage
-        ```sh
-        echo a b |> foreach echo
-        echo a b |> foreach echo prefix $ suffix
-        ```
-        """
-        prev_results = '\n'.join(prev_results.split(' '))
-        return Map.map(ast, prev_results, self, delimiter=' ')
-
     def foldr(self, commands: List[Term], prev_results: str, delimiter='\n'):
         items = parse(prev_results).values
         k, acc, *args = commands
 
         for item in items:
             command = Terms([k, acc] + args)
             acc = self.run_commands(command, item, run=True)
```

### Comparing `mash-shell-0.2.4/src/mash/shell/with_filesystem.py` & `mash-shell-0.2.5/src/mash/shell/with_filesystem.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from functools import partial
 from logging import debug
 
 from mash.filesystem.filesystem import FileSystem, OPTIONS, Option
 from mash.filesystem.discoverable import Discoverable
-from mash.filesystem.view import Path
+from mash.filesystem.view import Path, ViewError
+from mash.io_util import log
 from mash.shell.shell import build, set_completions, set_functions
 from mash.shell.function import ShellFunction as Function
 from mash.util import find_fuzzy_matches, hamming, has_method, is_digit, partial_simple
 
 cd_aliasses = 'cd_aliasses'
 path_delimiter = '/'
 
@@ -38,15 +39,14 @@
             self.shell.add_special_function(option, func)
 
         self.shell._default_method = self.default_method
 
     def _set_shell_functions(self, cls):
         # convert methods to functions
         cd = partial_simple(self.repository.cd)
-        ls = partial_simple(self.repository.ll, delimiter=', ')
         ll = partial_simple(self.repository.ll)
         get = partial_simple(self.get)
         set = partial_simple(self.set)
         new = partial_simple(self.new)
         tree = partial_simple(self.repository.tree)
         pwd = partial_simple(self.pwd)
         home = partial_simple(self.init_home)
@@ -55,30 +55,39 @@
         rm = partial_simple(self.repository.rm)
         # show = partial_simple(self.show)
         show = partial_simple(self.repository.show)
         reset = partial_simple(self.repository.reset)
 
         set_functions({'cd': cd,
                        'use': cd,
-                       'list': ls,
-                       'ls': ls,
-                       'll': ll,
+                       'l': ll,
+                       'list': ll,
                        'get': get,
                        'set': set,
                        'new': new,
                        'tree': tree,
                        'pwd': pwd,
                        'home': home,
                        'cp': cp,
                        'mv': mv,
                        'rm': rm,
                        'show': show,
                        'reset': reset,
                        }, cls)
 
+    def cd(self, *path: str):
+        """Change directory and finally reset the current directory.
+        Stay in the current directory by default.
+        """
+        try:
+            return self.repository.cd(path)
+        except ViewError as e:
+            log(e)
+        return
+
     def pwd(self):
         """Print the path to the current working directory
         """
         return ' '.join(self.repository.full_path)
 
     def get(self, *path: str):
         """Return the value of the file associated with `path`.
```

### Comparing `mash-shell-0.2.4/src/mash/subshell.py` & `mash-shell-0.2.5/src/mash/subshell.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.4/src/mash/util.py` & `mash-shell-0.2.5/src/mash/util.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.4/src/mash/verify_server.py` & `mash-shell-0.2.5/src/mash/verify_server.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.4/src/mash_shell.egg-info/PKG-INFO` & `mash-shell-0.2.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: mash-shell
-Version: 0.2.4
-Summary: A shell and other utils
-Author-email: voschezang <mark.voschezang@student.uva.nl>
-Project-URL: Homepage, https://github.com/voschezang/mash
-Project-URL: Bug Tracker, https://github.com/voschezang/mash/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: System :: Shells
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ![workflow-badge](https://github.com/voschezang/mash/actions/workflows/python-app.yml/badge.svg)
 <a href="https://pypi.org/project/mash-shell" title="Python versions"><img src="https://img.shields.io/badge/python-3.8%20|%203.10%20|%203.11-blue"/></a>
 <a href="https://pypi.org/project/mash-shell" title="PyPI"><img src="https://img.shields.io/badge/pypi-v0.2.0-blue"/></a>
 
 
 **Docs**:
 [MAIN](https://github.com/voschezang/mash/blob/main/README.md) 
@@ -97,16 +82,16 @@
 
 ## Filesystem (CRUD Operations)
 
 See `examples/filesystem.py` and `examples/discoverable.py`.
 
 | Example             | Description                                                  |
 | ------------------- | ------------------------------------------------------------ |
-| `ls [PATH]`         | List the items in a directory. Use the current working directory by default. Alias: `list` |
-| `cd`, `use [PATH]`  | Change the current working directory. Alias: `use`           |
+| `list [PATH]`       | List the items in a directory. Use the current working directory by default. Alias: `l` |
+| `cd [PATH]`         | Change the current working directory. Alias: `use`           |
 | `get NAME`          | Retrieve a file.                                             |
 | `set NAME VALUE`    | Modify a file.                                               |
 | `new NAME [NAME..]` | Create new directories.                                      |
 | `show [NAME]`       | Display detailed information about a directory.              |
 | `cp`, `mv`, `rm`    | Modify files. I.e. copy, move, rename or remove files.       |
 | `home [PATH]`       | Set home directory.                                          |
 | `reset`             | Refresh cached values.                                       |
@@ -210,14 +195,29 @@
 department_750, department_14
 ```
 
 
 
 # Library & Tools
 
+Repository structure
+
+```sh
+src
+├── examples
+├── lib # mash shell scripts
+└── mash
+    ├── filesystem # Directory-based datastructures: FileSystem, View
+    ├── object_parser # Parse JSON objects
+    └── shell # Shell, ShellWithFileSystem
+test
+```
+
+
+
 ## Setup
 
 Using a `Makefile` for convenience.
 
 ```sh
 make install
 make test
```

#### html2text {}

```diff
@@ -1,16 +1,8 @@
-Metadata-Version: 2.1 Name: mash-shell Version: 0.2.4 Summary: A shell and
-other utils Author-email: voschezang
-voschezang@student.uva.nl> Project-URL: Homepage, https://github.com/
-voschezang/mash Project-URL: Bug Tracker, https://github.com/voschezang/mash/
-issues Classifier: Programming Language :: Python :: 3 Classifier: Topic ::
-System :: Shells Classifier: License :: OSI Approved :: GNU General Public
-License v3 (GPLv3) Classifier: Operating System :: OS Independent Requires-
-Python: >=3.10 Description-Content-Type: text/markdown License-File: LICENSE !
-[workflow-badge](https://github.com/voschezang/mash/actions/workflows/python-
+![workflow-badge](https://github.com/voschezang/mash/actions/workflows/python-
 app.yml/badge.svg) [https://img.shields.io/badge/python-
 3.8%20|%203.10%20|%203.11-blue] [https://img.shields.io/badge/pypi-v0.2.0-blue]
 **Docs**: [MAIN](https://github.com/voschezang/mash/blob/main/README.md) |
 [SHELL.md](https://github.com/voschezang/mash/blob/main/SHELL.md) |
 [REFERENCE.md](https://github.com/voschezang/mash/blob/main/SHELL_REFERENCE.md)
 [A drawing of a terminal] # Mash | My Automation Shell A *shell* that can be
 used to for automation and (REST) resource discovery. It can be used as a [cli]
@@ -46,21 +38,21 @@
 arguments: cmd A comma- or newline-separated list of commands optional
 arguments: -h, --help show this help message and exit -v, --verbose -s, --safe
 Safe-mode. Ask for confirmation before executing commands. -f FILE, --file FILE
 Read and run FILE as a commands -r, --reload Reload last session --session
 SESSION Use session SESSION ``` ## Filesystem (CRUD Operations) See `examples/
 filesystem.py` and `examples/discoverable.py`. | Example | Description | | ----
 --------------- | -----------------------------------------------------------
-- | | `ls [PATH]` | List the items in a directory. Use the current working
-directory by default. Alias: `list` | | `cd`, `use [PATH]` | Change the current
-working directory. Alias: `use` | | `get NAME` | Retrieve a file. | | `set NAME
-VALUE` | Modify a file. | | `new NAME [NAME..]` | Create new directories. | |
-`show [NAME]` | Display detailed information about a directory. | | `cp`, `mv`,
-`rm` | Modify files. I.e. copy, move, rename or remove files. | | `home [PATH]`
-| Set home directory. | | `reset` | Refresh cached values. | ## Usage Examples
+- | | `list [PATH]` | List the items in a directory. Use the current working
+directory by default. Alias: `l` | | `cd [PATH]` | Change the current working
+directory. Alias: `use` | | `get NAME` | Retrieve a file. | | `set NAME VALUE`
+| Modify a file. | | `new NAME [NAME..]` | Create new directories. | | `show
+[NAME]` | Display detailed information about a directory. | | `cp`, `mv`, `rm`
+| Modify files. I.e. copy, move, rename or remove files. | | `home [PATH]` |
+Set home directory. | | `reset` | Refresh cached values. | ## Usage Examples
 For real-world examples, see [lib](https://github.com/voschezang/mash/blob/
 main/src/lib/math.sh). ### Example 1 See `src/shell_example.py`. It shows how
 to use a user-definnable mapping of custom functions. It uses the library `quo`
 to create a user-friendly subshell with autocompletion prompts. ```sh # py src/
 shell.py echo hello, echo world hello world ``` ```sh # py src/shell_example.py
 Welcome. Type help or ? to list commands. $ ? Documented commands (type help ):
 ======================================== e example f g h help ls shell $ help g
@@ -79,21 +71,24 @@
 'aquatic', 'penquins': [{'name': 'tux'}]} ]}]} ``` ```sh # note the
 autocompletion $ python src/examples/filesystem.py 'cd world; cd a; cd t; cd
 snakes; ll' python cobra ``` ### With Dynamic Data See `examples/
 discoverable.py`. ```sh # list remote/auto-generated data $ python src/
 examples/discoverable.py 'ls' department_805, department_399 # refresh data,
 then save $ py src/examples/discoverable.py 'ls ; save' department_750,
 department_14 # reload data $ python src/examples/discoverable.py 'ls'
-department_750, department_14 ``` # Library & Tools ## Setup Using a `Makefile`
-for convenience. ```sh make install make test ``` ## Parallelization Utilities
-Some experiments with parallelization, concurrency and `asyncio` in Python. ###
-Test Start a dummy server. ```sh python3 src/server.py ``` Do a simple load
-test ```sh python3 src/parallel.py -v ``` ## Object Parser - [src/
-object_parser/object_parser.py](object_parser.py) parses JSON data and
-instantiate Python objects. - [src/object_parser/oas.py](oas.py) converts
-domain-models to OAS. ### Example ```sh python src/object_parser_example.py ```
-[OAS Example] ### REST API Server ```sh python src/object_parser_server.py ```
-Client ```sh curl -X 'POST' 'http://localhost:5000/v1/organizations' \ -
-H 'Content-Type: application/json' \ -d '{ "board": [ "string" ], "ceo":
-"string", "departments": [ { "manager": "string", "teams": [ { "manager":
-"string", "members": [ "string" ], "team_type": "A", "active": true,
-"capacity": 0, "value": 0 } ] } ] }' ```
+department_750, department_14 ``` # Library & Tools Repository structure ```sh
+src âââ examples âââ lib # mash shell scripts âââ mash
+âââ filesystem # Directory-based datastructures: FileSystem, View
+âââ object_parser # Parse JSON objects âââ shell # Shell,
+ShellWithFileSystem test ``` ## Setup Using a `Makefile` for convenience. ```sh
+make install make test ``` ## Parallelization Utilities Some experiments with
+parallelization, concurrency and `asyncio` in Python. ### Test Start a dummy
+server. ```sh python3 src/server.py ``` Do a simple load test ```sh python3
+src/parallel.py -v ``` ## Object Parser - [src/object_parser/object_parser.py]
+(object_parser.py) parses JSON data and instantiate Python objects. - [src/
+object_parser/oas.py](oas.py) converts domain-models to OAS. ### Example ```sh
+python src/object_parser_example.py ``` [OAS Example] ### REST API Server ```sh
+python src/object_parser_server.py ``` Client ```sh curl -X 'POST' 'http://
+localhost:5000/v1/organizations' \ -H 'Content-Type: application/json' \ -d '
+{ "board": [ "string" ], "ceo": "string", "departments": [ { "manager":
+"string", "teams": [ { "manager": "string", "members": [ "string" ],
+"team_type": "A", "active": true, "capacity": 0, "value": 0 } ] } ] }' ```
```

### Comparing `mash-shell-0.2.4/src/mash_shell.egg-info/SOURCES.txt` & `mash-shell-0.2.5/src/mash_shell.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.4/test/test_html_table.py` & `mash-shell-0.2.5/test/test_html_table.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.4/test/test_parallel.py` & `mash-shell-0.2.5/test/test_parallel.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.4/test/test_pipeline.py` & `mash-shell-0.2.5/test/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.4/test/test_server.py` & `mash-shell-0.2.5/test/test_server.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.4/test/test_util.py` & `mash-shell-0.2.5/test/test_util.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.4/test/test_verify_server.py` & `mash-shell-0.2.5/test/test_verify_server.py`

 * *Files identical despite different names*

