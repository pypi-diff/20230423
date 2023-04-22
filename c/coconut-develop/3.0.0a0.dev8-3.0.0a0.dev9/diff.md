# Comparing `tmp/coconut-develop-3.0.0a0.dev8.tar.gz` & `tmp/coconut-develop-3.0.0a0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/coconut-develop-3.0.0a0.dev8.tar", last modified: Sat Feb  4 00:20:32 2023, max compression
+gzip compressed data, was "coconut-develop-3.0.0a0.dev9.tar", last modified: Sat Feb 11 01:34:33 2023, max compression
```

## Comparing `coconut-develop-3.0.0a0.dev8.tar` & `coconut-develop-3.0.0a0.dev9.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-04 00:20:32.000000 coconut-develop-3.0.0a0.dev8/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-04 00:20:32.000000 coconut-develop-3.0.0a0.dev8/__coconut__/
--rw-r--r--   0 runner    (1001) docker     (122)    38900 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/__coconut__/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/__coconut__/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     1245 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/__coconut__/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   184696 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/DOCS.md
--rw-r--r--   0 runner    (1001) docker     (122)      106 2023-02-04 00:20:32.000000 coconut-develop-3.0.0a0.dev8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-04 00:20:32.000000 coconut-develop-3.0.0a0.dev8/coconut/
--rw-r--r--   0 runner    (1001) docker     (122)     1486 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/__coconut__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     9734 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)      956 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     4663 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/highlighter.py
--rw-r--r--   0 runner    (1001) docker     (122)     1315 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/__coconut__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)    12684 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/root.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-04 00:20:32.000000 coconut-develop-3.0.0a0.dev8/coconut/icoconut/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-04 00:20:32.000000 coconut-develop-3.0.0a0.dev8/coconut/icoconut/coconut_py2/
--rw-r--r--   0 runner    (1001) docker     (122)      174 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/icoconut/coconut_py2/kernel.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-04 00:20:32.000000 coconut-develop-3.0.0a0.dev8/coconut/icoconut/coconut/
--rw-r--r--   0 runner    (1001) docker     (122)      141 2023-02-04 00:20:31.000000 coconut-develop-3.0.0a0.dev8/coconut/icoconut/coconut/kernel.json
--rw-r--r--   0 runner    (1001) docker     (122)     5621 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/icoconut/embed.py
--rw-r--r--   0 runner    (1001) docker     (122)    11020 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/icoconut/root.py
--rw-r--r--   0 runner    (1001) docker     (122)      783 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/icoconut/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-04 00:20:32.000000 coconut-develop-3.0.0a0.dev8/coconut/icoconut/coconut_py3/
--rw-r--r--   0 runner    (1001) docker     (122)      174 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/icoconut/coconut_py3/kernel.json
--rw-r--r--   0 runner    (1001) docker     (122)     1387 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/icoconut/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-04 00:20:32.000000 coconut-develop-3.0.0a0.dev8/coconut/icoconut/coconut_py/
--rw-r--r--   0 runner    (1001) docker     (122)      172 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/icoconut/coconut_py/kernel.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-04 00:20:32.000000 coconut-develop-3.0.0a0.dev8/coconut/tests/
--rw-r--r--   0 runner    (1001) docker     (122)    27927 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/tests/main_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     4539 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/tests/constants_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      786 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1794 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/tests/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-04 00:20:32.000000 coconut-develop-3.0.0a0.dev8/coconut/tests/src/
--rw-r--r--   0 runner    (1001) docker     (122)      496 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/tests/src/runner.coco
--rw-r--r--   0 runner    (1001) docker     (122)      192 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/tests/src/runnable.coco
--rw-r--r--   0 runner    (1001) docker     (122)    18438 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/tests/src/extras.coco
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-04 00:20:32.000000 coconut-develop-3.0.0a0.dev8/coconut/tests/src/cocotest/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-04 00:20:32.000000 coconut-develop-3.0.0a0.dev8/coconut/tests/src/cocotest/agnostic/
--rw-r--r--   0 runner    (1001) docker     (122)    40119 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/tests/src/cocotest/agnostic/suite.coco
--rw-r--r--   0 runner    (1001) docker     (122)     3773 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/tests/src/cocotest/agnostic/main.coco
--rw-r--r--   0 runner    (1001) docker     (122)     4676 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/tests/src/cocotest/agnostic/specific.coco
--rw-r--r--   0 runner    (1001) docker     (122)       87 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/tests/src/cocotest/agnostic/__init__.coco
--rw-r--r--   0 runner    (1001) docker     (122)    15411 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/tests/src/cocotest/agnostic/tutorial.coco
--rw-r--r--   0 runner    (1001) docker     (122)    42594 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/tests/src/cocotest/agnostic/util.coco
--rw-r--r--   0 runner    (1001) docker     (122)    60147 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/tests/src/cocotest/agnostic/primary.coco
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-04 00:20:32.000000 coconut-develop-3.0.0a0.dev8/coconut/tests/src/cocotest/target_35/
--rw-r--r--   0 runner    (1001) docker     (122)      345 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/tests/src/cocotest/target_35/py35_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-04 00:20:32.000000 coconut-develop-3.0.0a0.dev8/coconut/tests/src/cocotest/target_38/
--rw-r--r--   0 runner    (1001) docker     (122)      255 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/tests/src/cocotest/target_38/py38_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-04 00:20:32.000000 coconut-develop-3.0.0a0.dev8/coconut/tests/src/cocotest/target_36/
--rw-r--r--   0 runner    (1001) docker     (122)     1421 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/tests/src/cocotest/target_36/py36_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-04 00:20:32.000000 coconut-develop-3.0.0a0.dev8/coconut/tests/src/cocotest/non_strict/
--rw-r--r--   0 runner    (1001) docker     (122)     2054 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/tests/src/cocotest/non_strict/non_strict_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-04 00:20:32.000000 coconut-develop-3.0.0a0.dev8/coconut/tests/src/cocotest/target_2/
--rw-r--r--   0 runner    (1001) docker     (122)      356 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/tests/src/cocotest/target_2/py2_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-04 00:20:32.000000 coconut-develop-3.0.0a0.dev8/coconut/tests/src/cocotest/target_sys/
--rw-r--r--   0 runner    (1001) docker     (122)     3356 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/tests/src/cocotest/target_sys/target_sys_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-04 00:20:32.000000 coconut-develop-3.0.0a0.dev8/coconut/tests/src/cocotest/target_3/
--rw-r--r--   0 runner    (1001) docker     (122)     1155 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/tests/src/cocotest/target_3/py3_test.coco
--rw-r--r--   0 runner    (1001) docker     (122)     1444 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13505 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/_pyparsing.py
--rw-r--r--   0 runner    (1001) docker     (122)     1543 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     9212 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/convenience.py
--rw-r--r--   0 runner    (1001) docker     (122)    11609 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/requirements.py
--rw-r--r--   0 runner    (1001) docker     (122)     2850 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/convenience.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-04 00:20:32.000000 coconut-develop-3.0.0a0.dev8/coconut/command/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-04 00:20:32.000000 coconut-develop-3.0.0a0.dev8/coconut/command/resources/
--rw-r--r--   0 runner    (1001) docker     (122)       27 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/command/resources/zcoconut.pth
--rw-r--r--   0 runner    (1001) docker     (122)     2450 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/command/mypy.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/command/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)      778 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      688 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/command/command.pyi
--rw-r--r--   0 runner    (1001) docker     (122)    22145 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/command/util.py
--rw-r--r--   0 runner    (1001) docker     (122)     7911 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/command/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)    40558 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/command/command.py
--rw-r--r--   0 runner    (1001) docker     (122)     2177 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/command/watch.py
--rw-r--r--   0 runner    (1001) docker     (122)    18319 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/terminal.py
--rw-r--r--   0 runner    (1001) docker     (122)    11787 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/util.py
--rw-r--r--   0 runner    (1001) docker     (122)     1210 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5013 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/integrations.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-04 00:20:32.000000 coconut-develop-3.0.0a0.dev8/coconut/compiler/
--rw-r--r--   0 runner    (1001) docker     (122)   178564 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/compiler/compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)    58102 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/compiler/matching.py
--rw-r--r--   0 runner    (1001) docker     (122)      781 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/compiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-04 00:20:32.000000 coconut-develop-3.0.0a0.dev8/coconut/compiler/templates/
--rw-r--r--   0 runner    (1001) docker     (122)    89679 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/compiler/templates/header.py_template
--rw-r--r--   0 runner    (1001) docker     (122)    91660 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/compiler/grammar.py
--rw-r--r--   0 runner    (1001) docker     (122)    45943 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/compiler/util.py
--rw-r--r--   0 runner    (1001) docker     (122)    29756 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/compiler/header.py
--rw-r--r--   0 runner    (1001) docker     (122)    33690 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/coconut/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)      449 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2305 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     6945 2023-02-04 00:20:32.000000 coconut-develop-3.0.0a0.dev8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-04 00:20:32.000000 coconut-develop-3.0.0a0.dev8/_coconut/
--rw-r--r--   0 runner    (1001) docker     (122)     4400 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/_coconut/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/_coconut/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     1253 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/_coconut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)    11385 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/FAQ.md
--rw-r--r--   0 runner    (1001) docker     (122)       63 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)    65152 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/HELP.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-04 00:20:32.000000 coconut-develop-3.0.0a0.dev8/coconut_develop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2284 2023-02-04 00:20:32.000000 coconut-develop-3.0.0a0.dev8/coconut_develop.egg-info/SOURCES.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-04 00:20:32.000000 coconut-develop-3.0.0a0.dev8/xontrib/
--rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/xontrib/coconut.py
--rw-r--r--   0 runner    (1001) docker     (122)     2797 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/setup.py
--rw-r--r--   0 runner    (1001) docker     (122)     3569 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)    13686 2023-02-03 23:31:59.000000 coconut-develop-3.0.0a0.dev8/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-11 01:34:33.807755 coconut-develop-3.0.0a0.dev9/
+-rw-r--r--   0 runner    (1001) docker     (122)    13686 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)   184613 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/DOCS.md
+-rw-r--r--   0 runner    (1001) docker     (122)    11385 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/FAQ.md
+-rw-r--r--   0 runner    (1001) docker     (122)    65152 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/HELP.md
+-rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      449 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     6945 2023-02-11 01:34:33.807755 coconut-develop-3.0.0a0.dev9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3569 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-11 01:34:33.783753 coconut-develop-3.0.0a0.dev9/__coconut__/
+-rw-r--r--   0 runner    (1001) docker     (122)     1245 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/__coconut__/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38900 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/__coconut__/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/__coconut__/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-11 01:34:33.783753 coconut-develop-3.0.0a0.dev9/_coconut/
+-rw-r--r--   0 runner    (1001) docker     (122)     1253 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/_coconut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4400 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/_coconut/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/_coconut/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-11 01:34:33.787754 coconut-develop-3.0.0a0.dev9/coconut/
+-rw-r--r--   0 runner    (1001) docker     (122)     1315 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/__coconut__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1486 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/__coconut__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     1444 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      956 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     1210 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13505 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/_pyparsing.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-11 01:34:33.791754 coconut-develop-3.0.0a0.dev9/coconut/command/
+-rw-r--r--   0 runner    (1001) docker     (122)      778 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/command/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     7911 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/command/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)    40558 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/command/command.py
+-rw-r--r--   0 runner    (1001) docker     (122)      688 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/command/command.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     2450 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/command/mypy.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-11 01:34:33.791754 coconut-develop-3.0.0a0.dev9/coconut/command/resources/
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/command/resources/zcoconut.pth
+-rw-r--r--   0 runner    (1001) docker     (122)    22145 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/command/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2177 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/command/watch.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-11 01:34:33.795754 coconut-develop-3.0.0a0.dev9/coconut/compiler/
+-rw-r--r--   0 runner    (1001) docker     (122)      781 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/compiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   178564 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/compiler/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)    91660 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/compiler/grammar.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29756 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/compiler/header.py
+-rw-r--r--   0 runner    (1001) docker     (122)    58102 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/compiler/matching.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-11 01:34:33.795754 coconut-develop-3.0.0a0.dev9/coconut/compiler/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)    89722 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/compiler/templates/header.py_template
+-rw-r--r--   0 runner    (1001) docker     (122)    45943 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/compiler/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33690 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9212 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/convenience.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2850 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/convenience.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     9734 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4663 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/highlighter.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-11 01:34:33.795754 coconut-develop-3.0.0a0.dev9/coconut/icoconut/
+-rw-r--r--   0 runner    (1001) docker     (122)      783 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/icoconut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1387 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/icoconut/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-11 01:34:33.795754 coconut-develop-3.0.0a0.dev9/coconut/icoconut/coconut/
+-rw-r--r--   0 runner    (1001) docker     (122)      141 2023-02-11 01:34:32.000000 coconut-develop-3.0.0a0.dev9/coconut/icoconut/coconut/kernel.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-11 01:34:33.795754 coconut-develop-3.0.0a0.dev9/coconut/icoconut/coconut_py/
+-rw-r--r--   0 runner    (1001) docker     (122)      172 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/icoconut/coconut_py/kernel.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-11 01:34:33.795754 coconut-develop-3.0.0a0.dev9/coconut/icoconut/coconut_py2/
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/icoconut/coconut_py2/kernel.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-11 01:34:33.795754 coconut-develop-3.0.0a0.dev9/coconut/icoconut/coconut_py3/
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/icoconut/coconut_py3/kernel.json
+-rw-r--r--   0 runner    (1001) docker     (122)     5621 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/icoconut/embed.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11020 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/icoconut/root.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5013 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1543 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)    11609 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12684 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/root.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18319 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/terminal.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-11 01:34:33.799754 coconut-develop-3.0.0a0.dev9/coconut/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      786 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1794 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/tests/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4539 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/tests/constants_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27927 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/tests/main_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-11 01:34:33.799754 coconut-develop-3.0.0a0.dev9/coconut/tests/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-11 01:34:33.779753 coconut-develop-3.0.0a0.dev9/coconut/tests/src/cocotest/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-11 01:34:33.803754 coconut-develop-3.0.0a0.dev9/coconut/tests/src/cocotest/agnostic/
+-rw-r--r--   0 runner    (1001) docker     (122)       87 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/tests/src/cocotest/agnostic/__init__.coco
+-rw-r--r--   0 runner    (1001) docker     (122)     3773 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/tests/src/cocotest/agnostic/main.coco
+-rw-r--r--   0 runner    (1001) docker     (122)    60147 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/tests/src/cocotest/agnostic/primary.coco
+-rw-r--r--   0 runner    (1001) docker     (122)     4676 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/tests/src/cocotest/agnostic/specific.coco
+-rw-r--r--   0 runner    (1001) docker     (122)    40119 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/tests/src/cocotest/agnostic/suite.coco
+-rw-r--r--   0 runner    (1001) docker     (122)    15411 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/tests/src/cocotest/agnostic/tutorial.coco
+-rw-r--r--   0 runner    (1001) docker     (122)    42594 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/tests/src/cocotest/agnostic/util.coco
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-11 01:34:33.803754 coconut-develop-3.0.0a0.dev9/coconut/tests/src/cocotest/non_strict/
+-rw-r--r--   0 runner    (1001) docker     (122)     2054 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/tests/src/cocotest/non_strict/non_strict_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-11 01:34:33.803754 coconut-develop-3.0.0a0.dev9/coconut/tests/src/cocotest/target_2/
+-rw-r--r--   0 runner    (1001) docker     (122)      356 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/tests/src/cocotest/target_2/py2_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-11 01:34:33.803754 coconut-develop-3.0.0a0.dev9/coconut/tests/src/cocotest/target_3/
+-rw-r--r--   0 runner    (1001) docker     (122)     1155 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/tests/src/cocotest/target_3/py3_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-11 01:34:33.803754 coconut-develop-3.0.0a0.dev9/coconut/tests/src/cocotest/target_35/
+-rw-r--r--   0 runner    (1001) docker     (122)      345 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/tests/src/cocotest/target_35/py35_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-11 01:34:33.803754 coconut-develop-3.0.0a0.dev9/coconut/tests/src/cocotest/target_36/
+-rw-r--r--   0 runner    (1001) docker     (122)     1421 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/tests/src/cocotest/target_36/py36_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-11 01:34:33.803754 coconut-develop-3.0.0a0.dev9/coconut/tests/src/cocotest/target_38/
+-rw-r--r--   0 runner    (1001) docker     (122)      255 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/tests/src/cocotest/target_38/py38_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-11 01:34:33.803754 coconut-develop-3.0.0a0.dev9/coconut/tests/src/cocotest/target_sys/
+-rw-r--r--   0 runner    (1001) docker     (122)     3356 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/tests/src/cocotest/target_sys/target_sys_test.coco
+-rw-r--r--   0 runner    (1001) docker     (122)    18600 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/tests/src/extras.coco
+-rw-r--r--   0 runner    (1001) docker     (122)      192 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/tests/src/runnable.coco
+-rw-r--r--   0 runner    (1001) docker     (122)      496 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/tests/src/runner.coco
+-rw-r--r--   0 runner    (1001) docker     (122)    11787 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/coconut/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-11 01:34:33.807755 coconut-develop-3.0.0a0.dev9/coconut_develop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2284 2023-02-11 01:34:33.000000 coconut-develop-3.0.0a0.dev9/coconut_develop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2305 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)       63 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      106 2023-02-11 01:34:33.807755 coconut-develop-3.0.0a0.dev9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2797 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-11 01:34:33.803754 coconut-develop-3.0.0a0.dev9/xontrib/
+-rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-02-11 00:23:20.000000 coconut-develop-3.0.0a0.dev9/xontrib/coconut.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `coconut-develop-3.0.0a0.dev8/__coconut__/__init__.pyi` & `coconut-develop-3.0.0a0.dev9/__coconut__/__init__.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.0a0.dev8/__coconut__/__init__.py` & `coconut-develop-3.0.0a0.dev9/__coconut__/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.0a0.dev8/DOCS.md` & `coconut-develop-3.0.0a0.dev9/DOCS.md`

 * *Files 0% similar despite different names*

```diff
@@ -9990,1555 +9990,1550 @@
 00027050: 6520 696e 6465 7820 7265 7072 6573 656e  e index represen
 00027060: 7469 6e67 2074 6865 2069 6e64 6578 2069  ting the index i
 00027070: 6e20 6561 6368 2069 6e6e 6572 2069 7465  n each inner ite
 00027080: 7261 626c 652e 2053 7570 706f 7274 7320  rable. Supports 
 00027090: 696e 6465 7869 6e67 2e0a 0a46 6f72 205b  indexing...For [
 000270a0: 606e 756d 7079 605d 2823 6e75 6d70 792d  `numpy`](#numpy-
 000270b0: 696e 7465 6772 6174 696f 6e29 206f 626a  integration) obj
-000270c0: 6563 7473 2c20 6566 6665 6374 6976 656c  ects, effectivel
-000270d0: 7920 6571 7569 7661 6c65 6e74 2074 6f3a  y equivalent to:
-000270e0: 0a60 6060 636f 636f 6e75 745f 7079 7468  .```coconut_pyth
-000270f0: 6f6e 0a64 6566 206d 756c 7469 5f65 6e75  on.def multi_enu
-00027100: 6d65 7261 7465 2869 7465 7261 626c 6529  merate(iterable)
-00027110: 3a0a 2020 2020 6974 203d 206e 702e 6e64  :.    it = np.nd
-00027120: 6974 6572 2869 7465 7261 626c 652c 2066  iter(iterable, f
-00027130: 6c61 6773 3d5b 226d 756c 7469 5f69 6e64  lags=["multi_ind
-00027140: 6578 222c 2022 7265 6673 5f6f 6b22 5d29  ex", "refs_ok"])
-00027150: 0a20 2020 2066 6f72 2078 2069 6e20 6974  .    for x in it
-00027160: 3a0a 2020 2020 2020 2020 7969 656c 6420  :.        yield 
-00027170: 6974 2e6d 756c 7469 5f69 6e64 6578 2c20  it.multi_index, 
-00027180: 780a 6060 600a 0a41 6c73 6f20 7375 7070  x.```..Also supp
-00027190: 6f72 7473 2060 6c65 6e60 2066 6f72 205b  orts `len` for [
-000271a0: 606e 756d 7079 605d 2823 6e75 6d70 792d  `numpy`](#numpy-
-000271b0: 696e 7465 6772 6174 696f 6e29 2e0a 0a23  integration)...#
-000271c0: 2323 2323 2045 7861 6d70 6c65 0a0a 2a2a  #### Example..**
-000271d0: 436f 636f 6e75 743a 2a2a 0a60 6060 636f  Coconut:**.```co
-000271e0: 636f 6e75 745f 7079 636f 6e0a 3e3e 3e20  conut_pycon.>>> 
-000271f0: 5b31 2c20 323b 3b20 332c 2034 5d20 7c3e  [1, 2;; 3, 4] |>
-00027200: 206d 756c 7469 5f65 6e75 6d65 7261 7465   multi_enumerate
-00027210: 207c 3e20 6c69 7374 0a5b 2828 302c 2030   |> list.[((0, 0
-00027220: 292c 2031 292c 2028 2830 2c20 3129 2c20  ), 1), ((0, 1), 
-00027230: 3229 2c20 2828 312c 2030 292c 2033 292c  2), ((1, 0), 3),
-00027240: 2028 2831 2c20 3129 2c20 3429 5d0a 6060   ((1, 1), 4)].``
-00027250: 600a 0a2a 2a50 7974 686f 6e3a 2a2a 0a60  `..**Python:**.`
-00027260: 6060 636f 636f 6e75 745f 7079 7468 6f6e  ``coconut_python
-00027270: 0a61 7272 6179 203d 205b 5b31 2c20 325d  .array = [[1, 2]
-00027280: 2c20 5b33 2c20 345d 5d0a 656e 756d 6572  , [3, 4]].enumer
-00027290: 6174 6564 5f61 7272 6179 203d 205b 5d0a  ated_array = [].
-000272a0: 666f 7220 6920 696e 2072 616e 6765 286c  for i in range(l
-000272b0: 656e 2861 7272 6179 2929 3a0a 2020 2020  en(array)):.    
-000272c0: 666f 7220 6a20 696e 2072 616e 6765 286c  for j in range(l
-000272d0: 656e 2861 7272 6179 5b69 5d29 293a 0a20  en(array[i])):. 
-000272e0: 2020 2020 2020 2065 6e75 6d65 7261 7465         enumerate
-000272f0: 645f 6172 7261 792e 6170 7065 6e64 2828  d_array.append((
-00027300: 2869 2c20 6a29 2c20 6172 7261 795b 695d  (i, j), array[i]
-00027310: 5b6a 5d29 290a 6060 600a 0a23 2323 2320  [j])).```..#### 
-00027320: 6067 726f 7570 736f 6660 0a0a 2a2a 6772  `groupsof`..**gr
-00027330: 6f75 7073 6f66 2a2a 285f 6e5f 2c20 5f69  oupsof**(_n_, _i
-00027340: 7465 7261 626c 655f 2c20 5f66 696c 6c76  terable_, _fillv
-00027350: 616c 7565 5f3d 602e 2e2e 6029 0a0a 436f  alue_=`...`)..Co
-00027360: 636f 6e75 7420 7072 6f76 6964 6573 2074  conut provides t
-00027370: 6865 2060 6772 6f75 7073 6f66 6020 6275  he `groupsof` bu
-00027380: 696c 742d 696e 2074 6f20 7370 6c69 7420  ilt-in to split 
-00027390: 616e 2069 7465 7261 626c 6520 696e 746f  an iterable into
-000273a0: 2067 726f 7570 7320 6f66 2061 2073 7065   groups of a spe
-000273b0: 6369 6669 6320 6c65 6e67 7468 2e20 5370  cific length. Sp
-000273c0: 6563 6966 6963 616c 6c79 2c20 6067 726f  ecifically, `gro
-000273d0: 7570 736f 6628 6e2c 2069 7465 7261 626c  upsof(n, iterabl
-000273e0: 6529 6020 7769 6c6c 2073 706c 6974 2060  e)` will split `
-000273f0: 6974 6572 6162 6c65 6020 696e 746f 2074  iterable` into t
-00027400: 7570 6c65 7320 6f66 206c 656e 6774 6820  uples of length 
-00027410: 606e 602c 2077 6974 6820 6f6e 6c79 2074  `n`, with only t
-00027420: 6865 206c 6173 7420 7475 706c 6520 706f  he last tuple po
-00027430: 7465 6e74 6961 6c6c 7920 6f66 2073 697a  tentially of siz
-00027440: 6520 603c 206e 6020 6966 2074 6865 206c  e `< n` if the l
-00027450: 656e 6774 6820 6f66 2060 6974 6572 6162  ength of `iterab
-00027460: 6c65 6020 6973 206e 6f74 2064 6976 6973  le` is not divis
-00027470: 6962 6c65 2062 7920 606e 602e 2049 6620  ible by `n`. If 
-00027480: 7468 6174 2069 7320 6e6f 7420 7468 6520  that is not the 
-00027490: 6465 7369 7265 6420 6265 6861 7669 6f72  desired behavior
-000274a0: 2c20 5f66 696c 6c76 616c 7565 5f20 6361  , _fillvalue_ ca
-000274b0: 6e20 6265 2070 6173 7365 6420 616e 6420  n be passed and 
-000274c0: 7769 6c6c 2062 6520 7573 6564 2074 6f20  will be used to 
-000274d0: 7061 6420 7468 6520 656e 6420 6f66 2074  pad the end of t
-000274e0: 6865 206c 6173 7420 7475 706c 6520 746f  he last tuple to
-000274f0: 206c 656e 6774 6820 606e 602e 0a0a 4164   length `n`...Ad
-00027500: 6469 7469 6f6e 616c 6c79 2c20 6067 726f  ditionally, `gro
-00027510: 7570 736f 6660 2073 7570 706f 7274 7320  upsof` supports 
-00027520: 606c 656e 6020 7768 656e 2060 6974 6572  `len` when `iter
-00027530: 6162 6c65 6020 7375 7070 6f72 7473 2060  able` supports `
-00027540: 6c65 6e60 2e0a 0a23 2323 2323 2045 7861  len`...##### Exa
-00027550: 6d70 6c65 0a0a 2a2a 436f 636f 6e75 743a  mple..**Coconut:
-00027560: 2a2a 0a60 6060 636f 636f 6e75 740a 7061  **.```coconut.pa
-00027570: 6972 7320 3d20 7261 6e67 6528 312c 2031  irs = range(1, 1
-00027580: 3129 207c 3e20 6772 6f75 7073 6f66 2428  1) |> groupsof$(
-00027590: 3229 0a60 6060 0a0a 2a2a 5079 7468 6f6e  2).```..**Python
-000275a0: 3a2a 2a0a 6060 6063 6f63 6f6e 7574 5f70  :**.```coconut_p
-000275b0: 7974 686f 6e0a 7061 6972 7320 3d20 5b5d  ython.pairs = []
-000275c0: 0a67 726f 7570 203d 205b 5d0a 666f 7220  .group = [].for 
-000275d0: 6974 656d 2069 6e20 7261 6e67 6528 312c  item in range(1,
-000275e0: 2031 3129 3a0a 2020 2020 6772 6f75 702e   11):.    group.
-000275f0: 6170 7065 6e64 2869 7465 6d29 0a20 2020  append(item).   
-00027600: 2069 6620 6c65 6e28 6772 6f75 7029 203d   if len(group) =
-00027610: 3d20 323a 0a20 2020 2020 2020 2070 6169  = 2:.        pai
-00027620: 7273 2e61 7070 656e 6428 7475 706c 6528  rs.append(tuple(
-00027630: 6772 6f75 7029 290a 2020 2020 2020 2020  group)).        
-00027640: 6772 6f75 7020 3d20 5b5d 0a69 6620 6772  group = [].if gr
-00027650: 6f75 703a 0a20 2020 2070 6169 7273 2e61  oup:.    pairs.a
-00027660: 7070 656e 6428 7475 706c 6528 6772 6f75  ppend(tuple(grou
-00027670: 7029 290a 6060 600a 0a23 2323 2320 6077  p)).```..#### `w
-00027680: 696e 646f 7773 6f66 600a 0a2a 2a77 696e  indowsof`..**win
-00027690: 646f 7773 6f66 2a2a 285f 7369 7a65 5f2c  dowsof**(_size_,
-000276a0: 205f 6974 6572 6162 6c65 5f2c 205f 6669   _iterable_, _fi
-000276b0: 6c6c 7661 6c75 655f 3d60 2e2e 2e60 2c20  llvalue_=`...`, 
-000276c0: 5f73 7465 705f 3d60 3160 290a 0a60 7769  _step_=`1`)..`wi
-000276d0: 6e64 6f77 736f 6660 2070 726f 6475 6365  ndowsof` produce
-000276e0: 7320 616e 2069 7465 7261 626c 6520 7468  s an iterable th
-000276f0: 6174 2065 6666 6563 7469 7665 6c79 206d  at effectively m
-00027700: 696d 6963 7320 6120 736c 6964 696e 6720  imics a sliding 
-00027710: 7769 6e64 6f77 206f 7665 7220 5f69 7465  window over _ite
-00027720: 7261 626c 655f 206f 6620 7369 7a65 205f  rable_ of size _
-00027730: 7369 7a65 5f2e 205f 7374 6570 5f20 6465  size_. _step_ de
-00027740: 7465 726d 696e 6573 2074 6865 2073 7061  termines the spa
-00027750: 6369 6e67 2062 6574 7765 656e 2077 696e  cing between win
-00027760: 646f 7773 6f66 2e0a 0a49 6620 5f73 697a  dowsof...If _siz
-00027770: 655f 2069 7320 6c61 7267 6572 2074 6861  e_ is larger tha
-00027780: 6e20 5f69 7465 7261 626c 655f 2c20 6077  n _iterable_, `w
-00027790: 696e 646f 7773 6f66 6020 7769 6c6c 2070  indowsof` will p
-000277a0: 726f 6475 6365 2061 6e20 656d 7074 7920  roduce an empty 
-000277b0: 6974 6572 6162 6c65 2e20 4966 2074 6861  iterable. If tha
-000277c0: 7420 6973 206e 6f74 2074 6865 2064 6573  t is not the des
-000277d0: 6972 6564 2062 6568 6176 696f 722c 205f  ired behavior, _
-000277e0: 6669 6c6c 7661 6c75 655f 2063 616e 2062  fillvalue_ can b
-000277f0: 6520 7061 7373 6564 2061 6e64 2077 696c  e passed and wil
-00027800: 6c20 6265 2075 7365 6420 696e 2070 6c61  l be used in pla
-00027810: 6365 206f 6620 6d69 7373 696e 6720 7661  ce of missing va
-00027820: 6c75 6573 2e20 416c 736f 2c20 6966 205f  lues. Also, if _
-00027830: 6669 6c6c 7661 6c75 655f 2069 7320 7061  fillvalue_ is pa
-00027840: 7373 6564 2061 6e64 2074 6865 206c 656e  ssed and the len
-00027850: 6774 6820 6f66 2074 6865 205f 6974 6572  gth of the _iter
-00027860: 6162 6c65 5f20 6973 206e 6f74 2064 6976  able_ is not div
-00027870: 6973 6962 6c65 2062 7920 5f73 7465 705f  isible by _step_
-00027880: 2c20 5f66 696c 6c76 616c 7565 5f20 7769  , _fillvalue_ wi
-00027890: 6c6c 2062 6520 7573 6564 2069 6e20 7468  ll be used in th
-000278a0: 6174 2063 6173 6520 746f 2070 6164 2074  at case to pad t
-000278b0: 6865 206c 6173 7420 7769 6e64 6f77 2061  he last window a
-000278c0: 7320 7765 6c6c 2e20 4e6f 7465 2074 6861  s well. Note tha
-000278d0: 7420 5f66 696c 6c76 616c 7565 5f20 7769  t _fillvalue_ wi
-000278e0: 6c6c 206f 6e6c 7920 6576 6572 2061 7070  ll only ever app
-000278f0: 6561 7220 696e 2074 6865 206c 6173 7420  ear in the last 
-00027900: 7769 6e64 6f77 2e0a 0a41 6464 6974 696f  window...Additio
-00027910: 6e61 6c6c 792c 2060 7769 6e64 6f77 736f  nally, `windowso
-00027920: 6660 2073 7570 706f 7274 7320 606c 656e  f` supports `len
-00027930: 6020 7768 656e 2060 6974 6572 6162 6c65  ` when `iterable
-00027940: 6020 7375 7070 6f72 7473 2060 6c65 6e60  ` supports `len`
-00027950: 2e0a 0a23 2323 2323 2045 7861 6d70 6c65  ...##### Example
-00027960: 0a0a 2a2a 436f 636f 6e75 743a 2a2a 0a60  ..**Coconut:**.`
-00027970: 6060 636f 636f 6e75 740a 6173 7365 7274  ``coconut.assert
-00027980: 2022 3132 3334 3522 207c 3e20 7769 6e64   "12345" |> wind
-00027990: 6f77 736f 6624 2833 2920 7c3e 206c 6973  owsof$(3) |> lis
-000279a0: 7420 3d3d 205b 2822 3122 2c20 2232 222c  t == [("1", "2",
-000279b0: 2022 3322 292c 2028 2232 222c 2022 3322   "3"), ("2", "3"
-000279c0: 2c20 2234 2229 2c20 2822 3322 2c20 2234  , "4"), ("3", "4
-000279d0: 222c 2022 3522 295d 0a60 6060 0a0a 2a2a  ", "5")].```..**
-000279e0: 5079 7468 6f6e 3a2a 2a0a 5f43 616e 2774  Python:**._Can't
-000279f0: 2062 6520 646f 6e65 2077 6974 686f 7574   be done without
-00027a00: 2074 6865 2064 6566 696e 6974 696f 6e20   the definition 
-00027a10: 6f66 2060 7769 6e64 6f77 736f 6660 3b20  of `windowsof`; 
-00027a20: 7365 6520 7468 6520 636f 6d70 696c 6564  see the compiled
-00027a30: 2068 6561 6465 7220 666f 7220 7468 6520   header for the 
-00027a40: 6675 6c6c 2064 6566 696e 6974 696f 6e2e  full definition.
-00027a50: 5f0a 0a23 2323 2320 6063 6f6c 6c65 6374  _..#### `collect
-00027a60: 6279 600a 0a2a 2a63 6f6c 6c65 6374 6279  by`..**collectby
-00027a70: 2a2a 285f 6b65 795c 5f66 756e 635f 2c20  **(_key\_func_, 
-00027a80: 5f69 7465 7261 626c 655f 2c20 5f76 616c  _iterable_, _val
-00027a90: 7565 5c5f 6675 6e63 5f3d 604e 6f6e 6560  ue\_func_=`None`
-00027aa0: 2c20 5f72 6564 7563 655c 5f66 756e 635f  , _reduce\_func_
-00027ab0: 3d60 4e6f 6e65 6029 0a0a 6063 6f6c 6c65  =`None`)..`colle
-00027ac0: 6374 6279 286b 6579 5f66 756e 632c 2069  ctby(key_func, i
-00027ad0: 7465 7261 626c 6529 6020 636f 6c6c 6563  terable)` collec
-00027ae0: 7473 2074 6865 2069 7465 6d73 2069 6e20  ts the items in 
-00027af0: 6069 7465 7261 626c 6560 2069 6e74 6f20  `iterable` into 
-00027b00: 6120 6469 6374 696f 6e61 7279 206f 6620  a dictionary of 
-00027b10: 6c69 7374 7320 6b65 7965 6420 6279 2060  lists keyed by `
-00027b20: 6b65 795f 6675 6e63 2869 7465 6d29 602e  key_func(item)`.
-00027b30: 0a0a 4966 2060 7661 6c75 655f 6675 6e63  ..If `value_func
-00027b40: 6020 6973 2070 6173 7365 642c 2060 636f  ` is passed, `co
-00027b50: 6c6c 6563 7462 7928 6b65 795f 6675 6e63  llectby(key_func
-00027b60: 2c20 6974 6572 6162 6c65 2c20 7661 6c75  , iterable, valu
-00027b70: 655f 6675 6e63 3d76 616c 7565 5f66 756e  e_func=value_fun
-00027b80: 6329 6020 696e 7374 6561 6420 636f 6c6c  c)` instead coll
-00027b90: 6563 7473 2076 616c 7565 5f66 756e 6328  ects value_func(
-00027ba0: 6974 656d 2920 696e 746f 2065 6163 6820  item) into each 
-00027bb0: 6c69 7374 2069 6e73 7465 6164 206f 6620  list instead of 
-00027bc0: 6974 656d 2e0a 0a49 6620 6072 6564 7563  item...If `reduc
-00027bd0: 655f 6675 6e63 6020 6973 2070 6173 7365  e_func` is passe
-00027be0: 642c 2060 636f 6c6c 6563 7462 7928 6b65  d, `collectby(ke
-00027bf0: 795f 6675 6e63 2c20 6974 6572 6162 6c65  y_func, iterable
-00027c00: 2c20 7265 6475 6365 5f66 756e 633d 7265  , reduce_func=re
-00027c10: 6475 6365 5f66 756e 6329 602c 2069 6e73  duce_func)`, ins
-00027c20: 7465 6164 206f 6620 636f 6c6c 6563 7469  tead of collecti
-00027c30: 6e67 2074 6865 2069 7465 6d73 2069 6e74  ng the items int
-00027c40: 6f20 6c69 7374 732c 2072 6564 7563 6573  o lists, reduces
-00027c50: 206f 7665 7220 7468 6520 6974 656d 7320   over the items 
-00027c60: 6f66 2065 6163 6820 6b65 7920 7769 7468  of each key with
-00027c70: 2072 6564 7563 655f 6675 6e63 2c20 6566   reduce_func, ef
-00027c80: 6665 6374 6976 656c 7920 696d 706c 656d  fectively implem
-00027c90: 656e 7469 6e67 2061 204d 6170 5265 6475  enting a MapRedu
-00027ca0: 6365 206f 7065 7261 7469 6f6e 2e0a 0a60  ce operation...`
-00027cb0: 636f 6c6c 6563 7462 7960 2069 7320 6566  collectby` is ef
-00027cc0: 6665 6374 6976 656c 7920 6571 7569 7661  fectively equiva
-00027cd0: 6c65 6e74 2074 6f3a 0a60 6060 636f 636f  lent to:.```coco
-00027ce0: 6e75 745f 7079 7468 6f6e 0a66 726f 6d20  nut_python.from 
-00027cf0: 636f 6c6c 6563 7469 6f6e 7320 696d 706f  collections impo
-00027d00: 7274 2064 6566 6175 6c74 6469 6374 0a0a  rt defaultdict..
-00027d10: 6465 6620 636f 6c6c 6563 7462 7928 6b65  def collectby(ke
-00027d20: 795f 6675 6e63 2c20 6974 6572 6162 6c65  y_func, iterable
-00027d30: 2c20 7661 6c75 655f 6675 6e63 3d69 6465  , value_func=ide
-00027d40: 6e74 2c20 7265 6475 6365 5f66 756e 633d  nt, reduce_func=
-00027d50: 4e6f 6e65 293a 0a20 2020 2063 6f6c 6c65  None):.    colle
-00027d60: 6374 696f 6e20 3d20 6465 6661 756c 7464  ction = defaultd
-00027d70: 6963 7428 6c69 7374 2920 6966 2072 6564  ict(list) if red
-00027d80: 7563 655f 6675 6e63 2069 7320 4e6f 6e65  uce_func is None
-00027d90: 2065 6c73 6520 7b7d 0a20 2020 2066 6f72   else {}.    for
-00027da0: 2069 7465 6d20 696e 2069 7465 7261 626c   item in iterabl
-00027db0: 653a 0a20 2020 2020 2020 206b 6579 203d  e:.        key =
-00027dc0: 206b 6579 5f66 756e 6328 6974 656d 290a   key_func(item).
-00027dd0: 2020 2020 2020 2020 7661 6c75 6520 3d20          value = 
-00027de0: 7661 6c75 655f 6675 6e63 2869 7465 6d29  value_func(item)
-00027df0: 0a20 2020 2020 2020 2069 6620 7265 6475  .        if redu
-00027e00: 6365 5f66 756e 6320 6973 204e 6f6e 653a  ce_func is None:
-00027e10: 0a20 2020 2020 2020 2020 2020 2063 6f6c  .            col
-00027e20: 6c65 6374 696f 6e5b 6b65 795d 2e61 7070  lection[key].app
-00027e30: 656e 6428 7661 6c75 6529 0a20 2020 2020  end(value).     
-00027e40: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00027e50: 2020 2020 206f 6c64 5f76 616c 7565 203d       old_value =
-00027e60: 2063 6f6c 6c65 6374 696f 6e2e 6765 7428   collection.get(
-00027e70: 6b65 792c 2073 656e 7469 6e65 6c29 0a20  key, sentinel). 
-00027e80: 2020 2020 2020 2020 2020 2069 6620 6f6c             if ol
-00027e90: 645f 7661 6c75 6520 6973 206e 6f74 2073  d_value is not s
-00027ea0: 656e 7469 6e65 6c3a 0a20 2020 2020 2020  entinel:.       
-00027eb0: 2020 2020 2020 2020 2076 616c 7565 203d           value =
-00027ec0: 2072 6564 7563 655f 6675 6e63 286f 6c64   reduce_func(old
-00027ed0: 5f76 616c 7565 2c20 7661 6c75 6529 0a20  _value, value). 
-00027ee0: 2020 2020 2020 2020 2020 2063 6f6c 6c65             colle
-00027ef0: 6374 696f 6e5b 6b65 795d 203d 2076 616c  ction[key] = val
-00027f00: 7565 0a20 2020 2072 6574 7572 6e20 636f  ue.    return co
-00027f10: 6c6c 6563 7469 6f6e 0a60 6060 0a0a 6063  llection.```..`c
-00027f20: 6f6c 6c65 6374 6279 6020 6973 2073 696d  ollectby` is sim
-00027f30: 696c 6172 2074 6f20 5b60 6974 6572 746f  ilar to [`iterto
-00027f40: 6f6c 732e 6772 6f75 7062 7960 5d28 6874  ols.groupby`](ht
-00027f50: 7470 733a 2f2f 646f 6373 2e70 7974 686f  tps://docs.pytho
-00027f60: 6e2e 6f72 672f 332f 6c69 6272 6172 792f  n.org/3/library/
-00027f70: 6974 6572 746f 6f6c 732e 6874 6d6c 2369  itertools.html#i
-00027f80: 7465 7274 6f6f 6c73 2e67 726f 7570 6279  tertools.groupby
-00027f90: 2920 6578 6365 7074 2074 6861 7420 6063  ) except that `c
-00027fa0: 6f6c 6c65 6374 6279 6020 6167 6772 6567  ollectby` aggreg
-00027fb0: 6174 6573 2063 6f6d 6d6f 6e20 656c 656d  ates common elem
-00027fc0: 656e 7473 2072 6567 6172 646c 6573 7320  ents regardless 
-00027fd0: 6f66 2074 6865 6972 206f 7264 6572 2069  of their order i
-00027fe0: 6e20 7468 6520 696e 7075 7420 6974 6572  n the input iter
-00027ff0: 6162 6c65 2c20 7768 6572 6561 7320 6067  able, whereas `g
-00028000: 726f 7570 6279 6020 6f6e 6c79 2061 6767  roupby` only agg
-00028010: 7265 6761 7465 7320 636f 6d6d 6f6e 2065  regates common e
-00028020: 6c65 6d65 6e74 7320 7468 6174 2061 7265  lements that are
-00028030: 2061 646a 6163 656e 7420 696e 2074 6865   adjacent in the
-00028040: 2069 6e70 7574 2069 7465 7261 626c 652e   input iterable.
-00028050: 0a0a 2323 2323 2320 4578 616d 706c 650a  ..##### Example.
-00028060: 0a2a 2a43 6f63 6f6e 7574 3a2a 2a0a 6060  .**Coconut:**.``
-00028070: 6063 6f63 6f6e 7574 0a75 7365 725f 6261  `coconut.user_ba
-00028080: 6c61 6e63 6573 203d 2028 0a20 2020 2062  lances = (.    b
-00028090: 616c 616e 6365 5f64 6174 610a 2020 2020  alance_data.    
-000280a0: 7c3e 2063 6f6c 6c65 6374 6279 2428 2e75  |> collectby$(.u
-000280b0: 7365 722c 2076 616c 7565 5f66 756e 633d  ser, value_func=
-000280c0: 2e62 616c 616e 6365 2c20 7265 6475 6365  .balance, reduce
-000280d0: 5f66 756e 633d 282b 2929 0a29 0a60 6060  _func=(+)).).```
-000280e0: 0a0a 2a2a 5079 7468 6f6e 3a2a 2a0a 6060  ..**Python:**.``
-000280f0: 6063 6f63 6f6e 7574 5f70 7974 686f 6e0a  `coconut_python.
-00028100: 6672 6f6d 2063 6f6c 6c65 6374 696f 6e73  from collections
-00028110: 2069 6d70 6f72 7420 6465 6661 756c 7464   import defaultd
-00028120: 6963 740a 0a75 7365 725f 6261 6c61 6e63  ict..user_balanc
-00028130: 6573 203d 2064 6566 6175 6c74 6469 6374  es = defaultdict
-00028140: 2869 6e74 290a 666f 7220 6974 656d 2069  (int).for item i
-00028150: 6e20 6261 6c61 6e63 655f 6461 7461 3a0a  n balance_data:.
-00028160: 2020 2020 7573 6572 5f62 616c 616e 6365      user_balance
-00028170: 735b 6974 656d 2e75 7365 725d 202b 3d20  s[item.user] += 
-00028180: 6974 656d 2e62 616c 616e 6365 0a60 6060  item.balance.```
-00028190: 0a0a 2323 2323 2060 616c 6c5f 6571 7561  ..#### `all_equa
-000281a0: 6c60 0a0a 2a2a 616c 6c5c 5f65 7175 616c  l`..**all\_equal
-000281b0: 2a2a 285f 6974 6572 6162 6c65 5f29 0a0a  **(_iterable_)..
-000281c0: 436f 636f 6e75 7427 7320 6061 6c6c 5f65  Coconut's `all_e
-000281d0: 7175 616c 6020 6275 696c 742d 696e 2074  qual` built-in t
-000281e0: 616b 6573 2069 6e20 616e 2069 7465 7261  akes in an itera
-000281f0: 626c 6520 616e 6420 6465 7465 726d 696e  ble and determin
-00028200: 6573 2077 6865 7468 6572 2061 6c6c 206f  es whether all o
-00028210: 6620 6974 7320 656c 656d 656e 7473 2061  f its elements a
-00028220: 7265 2065 7175 616c 2074 6f20 6561 6368  re equal to each
-00028230: 206f 7468 6572 2e20 6061 6c6c 5f65 7175   other. `all_equ
-00028240: 616c 6020 6173 7375 6d65 7320 7472 616e  al` assumes tran
-00028250: 7369 7469 7669 7479 206f 6620 6571 7561  sitivity of equa
-00028260: 6c69 7479 2061 6e64 2074 6861 7420 6021  lity and that `!
-00028270: 3d60 2069 7320 7468 6520 6e65 6761 7469  =` is the negati
-00028280: 6f6e 206f 6620 603d 3d60 2e20 5370 6563  on of `==`. Spec
-00028290: 6961 6c20 7375 7070 6f72 7420 6973 2070  ial support is p
-000282a0: 726f 7669 6465 6420 666f 7220 5b60 6e75  rovided for [`nu
-000282b0: 6d70 7960 5d28 236e 756d 7079 2d69 6e74  mpy`](#numpy-int
-000282c0: 6567 7261 7469 6f6e 2920 6f62 6a65 6374  egration) object
-000282d0: 732e 0a0a 2323 2323 2320 4578 616d 706c  s...##### Exampl
-000282e0: 650a 0a2a 2a43 6f63 6f6e 7574 3a2a 2a0a  e..**Coconut:**.
-000282f0: 6060 6063 6f63 6f6e 7574 0a61 6c6c 5f65  ```coconut.all_e
-00028300: 7175 616c 285b 312c 2031 2c20 315d 290a  qual([1, 1, 1]).
-00028310: 616c 6c5f 6571 7561 6c28 5b31 2c20 312c  all_equal([1, 1,
-00028320: 2032 5d29 0a60 6060 0a0a 2a2a 5079 7468   2]).```..**Pyth
-00028330: 6f6e 3a2a 2a0a 6060 6063 6f63 6f6e 7574  on:**.```coconut
-00028340: 5f70 7974 686f 6e0a 7365 6e74 696e 656c  _python.sentinel
-00028350: 203d 206f 626a 6563 7428 290a 6465 6620   = object().def 
-00028360: 616c 6c5f 6571 7561 6c28 6974 6572 6162  all_equal(iterab
-00028370: 6c65 293a 0a20 2020 2066 6972 7374 5f69  le):.    first_i
-00028380: 7465 6d20 3d20 7365 6e74 696e 656c 0a20  tem = sentinel. 
-00028390: 2020 2066 6f72 2069 7465 6d20 696e 2069     for item in i
-000283a0: 7465 7261 626c 653a 0a20 2020 2020 2020  terable:.       
-000283b0: 2069 6620 6669 7273 745f 6974 656d 2069   if first_item i
-000283c0: 7320 7365 6e74 696e 656c 3a0a 2020 2020  s sentinel:.    
-000283d0: 2020 2020 2020 2020 6669 7273 745f 6974          first_it
-000283e0: 656d 203d 2069 7465 6d0a 2020 2020 2020  em = item.      
-000283f0: 2020 656c 6966 2066 6972 7374 5f69 7465    elif first_ite
-00028400: 6d20 213d 2069 7465 6d3a 0a20 2020 2020  m != item:.     
-00028410: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-00028420: 6c73 650a 2020 2020 7265 7475 726e 2054  lse.    return T
-00028430: 7275 650a 616c 6c5f 6571 7561 6c28 5b31  rue.all_equal([1
-00028440: 2c20 312c 2031 5d29 0a61 6c6c 5f65 7175  , 1, 1]).all_equ
-00028450: 616c 285b 312c 2031 2c20 325d 290a 6060  al([1, 1, 2]).``
-00028460: 600a 0a23 2323 2320 6070 6172 616c 6c65  `..#### `paralle
-00028470: 6c5f 6d61 7060 0a0a 2a2a 7061 7261 6c6c  l_map`..**parall
-00028480: 656c 5c5f 6d61 702a 2a28 5f66 756e 6374  el\_map**(_funct
-00028490: 696f 6e5f 2c20 2a5f 6974 6572 6162 6c65  ion_, *_iterable
-000284a0: 735f 2c20 2a2c 205f 6368 756e 6b73 697a  s_, *, _chunksiz
-000284b0: 655f 3d60 3160 2c20 5f73 7472 6963 745f  e_=`1`, _strict_
-000284c0: 3d60 4661 6c73 6560 290a 0a43 6f63 6f6e  =`False`)..Cocon
-000284d0: 7574 2070 726f 7669 6465 7320 6120 7061  ut provides a pa
-000284e0: 7261 6c6c 656c 2076 6572 7369 6f6e 206f  rallel version o
-000284f0: 6620 606d 6170 6020 756e 6465 7220 7468  f `map` under th
-00028500: 6520 6e61 6d65 2060 7061 7261 6c6c 656c  e name `parallel
-00028510: 5f6d 6170 602e 2060 7061 7261 6c6c 656c  _map`. `parallel
-00028520: 5f6d 6170 6020 6d61 6b65 7320 7573 6520  _map` makes use 
-00028530: 6f66 206d 756c 7469 706c 6520 7072 6f63  of multiple proc
-00028540: 6573 7365 732c 2061 6e64 2069 7320 7468  esses, and is th
-00028550: 6572 6566 6f72 6520 6d75 6368 2066 6173  erefore much fas
-00028560: 7465 7220 7468 616e 2060 6d61 7060 2066  ter than `map` f
-00028570: 6f72 2043 5055 2d62 6f75 6e64 2074 6173  or CPU-bound tas
-00028580: 6b73 2e20 6070 6172 616c 6c65 6c5f 6d61  ks. `parallel_ma
-00028590: 7060 206e 6576 6572 206c 6f61 6473 2074  p` never loads t
-000285a0: 6865 2065 6e74 6972 6520 696e 7075 7420  he entire input 
-000285b0: 6974 6572 6174 6f72 2069 6e74 6f20 6d65  iterator into me
-000285c0: 6d6f 7279 2c20 7468 6f75 6768 2069 7420  mory, though it 
-000285d0: 646f 6573 2063 6f6e 7375 6d65 2074 6865  does consume the
-000285e0: 2065 6e74 6972 6520 696e 7075 7420 6974   entire input it
-000285f0: 6572 6174 6f72 2061 7320 736f 6f6e 2061  erator as soon a
-00028600: 7320 6120 7369 6e67 6c65 206f 7574 7075  s a single outpu
-00028610: 7420 6973 2072 6571 7565 7374 6564 2e20  t is requested. 
-00028620: 4966 2061 6e79 2065 7863 6570 7469 6f6e  If any exception
-00028630: 7320 6172 6520 7261 6973 6564 2069 6e73  s are raised ins
-00028640: 6964 6520 6f66 2060 7061 7261 6c6c 656c  ide of `parallel
-00028650: 5f6d 6170 602c 2061 2074 7261 6365 6261  _map`, a traceba
-00028660: 636b 2077 696c 6c20 6265 2070 7269 6e74  ck will be print
-00028670: 6564 2061 7320 736f 6f6e 2061 7320 7468  ed as soon as th
-00028680: 6579 2061 7265 2065 6e63 6f75 6e74 6572  ey are encounter
-00028690: 6564 2e0a 0a42 6563 6175 7365 2060 7061  ed...Because `pa
-000286a0: 7261 6c6c 656c 5f6d 6170 6020 7573 6573  rallel_map` uses
-000286b0: 206d 756c 7469 706c 6520 7072 6f63 6573   multiple proces
-000286c0: 7365 7320 666f 7220 6974 7320 6578 6563  ses for its exec
-000286d0: 7574 696f 6e2c 2069 7420 6973 206e 6563  ution, it is nec
-000286e0: 6573 7361 7279 2074 6861 7420 616c 6c20  essary that all 
-000286f0: 6f66 2069 7473 2061 7267 756d 656e 7473  of its arguments
-00028700: 2062 6520 7069 636b 6c65 6162 6c65 2e20   be pickleable. 
-00028710: 4f6e 6c79 206f 626a 6563 7473 2064 6566  Only objects def
-00028720: 696e 6564 2061 7420 7468 6520 6d6f 6475  ined at the modu
-00028730: 6c65 206c 6576 656c 2c20 616e 6420 6e6f  le level, and no
-00028740: 7420 6c61 6d62 6461 732c 206f 626a 6563  t lambdas, objec
-00028750: 7473 2064 6566 696e 6564 2069 6e73 6964  ts defined insid
-00028760: 6520 6f66 2061 2066 756e 6374 696f 6e2c  e of a function,
-00028770: 206f 7220 6f62 6a65 6374 7320 6465 6669   or objects defi
-00028780: 6e65 6420 696e 7369 6465 206f 6620 7468  ned inside of th
-00028790: 6520 696e 7465 7270 7265 7465 722c 2061  e interpreter, a
-000287a0: 7265 2070 6963 6b6c 6561 626c 652e 2046  re pickleable. F
-000287b0: 7572 7468 6572 6d6f 7265 2c20 6f6e 2057  urthermore, on W
-000287c0: 696e 646f 7773 2c20 6974 2069 7320 6e65  indows, it is ne
-000287d0: 6365 7373 6172 7920 7468 6174 2061 6c6c  cessary that all
-000287e0: 2063 616c 6c73 2074 6f20 6070 6172 616c   calls to `paral
-000287f0: 6c65 6c5f 6d61 7060 206f 6363 7572 2069  lel_map` occur i
-00028800: 6e73 6964 6520 6f66 2061 6e20 6069 6620  nside of an `if 
-00028810: 5f5f 6e61 6d65 5f5f 203d 3d20 225f 5f6d  __name__ == "__m
-00028820: 6169 6e5f 5f22 6020 6775 6172 642e 0a0a  ain__"` guard...
-00028830: 6070 6172 616c 6c65 6c5f 6d61 7060 2073  `parallel_map` s
-00028840: 7570 706f 7274 7320 6120 6063 6875 6e6b  upports a `chunk
-00028850: 7369 7a65 6020 6172 6775 6d65 6e74 2c20  size` argument, 
-00028860: 7768 6963 6820 6465 7465 726d 696e 6573  which determines
-00028870: 2068 6f77 206d 616e 7920 6974 656d 7320   how many items 
-00028880: 6172 6520 7061 7373 6564 2074 6f20 6561  are passed to ea
-00028890: 6368 2070 726f 6365 7373 2061 7420 6120  ch process at a 
-000288a0: 7469 6d65 2e20 4c61 7267 6572 2076 616c  time. Larger val
-000288b0: 7565 7320 6f66 205f 6368 756e 6b73 697a  ues of _chunksiz
-000288c0: 655f 2061 7265 2072 6563 6f6d 6d65 6e64  e_ are recommend
-000288d0: 6564 2077 6865 6e20 6465 616c 696e 6720  ed when dealing 
-000288e0: 7769 7468 2076 6572 7920 6c6f 6e67 2069  with very long i
-000288f0: 7465 7261 626c 6573 2e20 4164 6469 7469  terables. Additi
-00028900: 6f6e 616c 6c79 2c20 696e 2074 6865 206d  onally, in the m
-00028910: 756c 7469 2d69 7465 7261 626c 6520 6361  ulti-iterable ca
-00028920: 7365 2c20 5f73 7472 6963 745f 2063 616e  se, _strict_ can
-00028930: 2062 6520 7365 7420 746f 2060 5472 7565   be set to `True
-00028940: 6020 746f 2065 6e73 7572 6520 7468 6174  ` to ensure that
-00028950: 2061 6c6c 2069 7465 7261 626c 6573 2061   all iterables a
-00028960: 7265 2074 6865 2073 616d 6520 6c65 6e67  re the same leng
-00028970: 7468 2e0a 0a49 6620 6d75 6c74 6970 6c65  th...If multiple
-00028980: 2073 6571 7565 6e74 6961 6c20 6361 6c6c   sequential call
-00028990: 7320 746f 2060 7061 7261 6c6c 656c 5f6d  s to `parallel_m
-000289a0: 6170 6020 6e65 6564 2074 6f20 6265 206d  ap` need to be m
-000289b0: 6164 652c 2069 7420 6973 2068 6967 686c  ade, it is highl
-000289c0: 7920 7265 636f 6d6d 656e 6465 6420 7468  y recommended th
-000289d0: 6174 2074 6865 7920 6265 2064 6f6e 6520  at they be done 
-000289e0: 696e 7369 6465 206f 6620 6120 6077 6974  inside of a `wit
-000289f0: 6820 7061 7261 6c6c 656c 5f6d 6170 2e6d  h parallel_map.m
-00028a00: 756c 7469 706c 655f 7365 7175 656e 7469  ultiple_sequenti
-00028a10: 616c 5f63 616c 6c73 2829 3a60 2062 6c6f  al_calls():` blo
-00028a20: 636b 2c20 7768 6963 6820 7769 6c6c 2063  ck, which will c
-00028a30: 6175 7365 2074 6865 2064 6966 6665 7265  ause the differe
-00028a40: 6e74 2063 616c 6c73 2074 6f20 7573 6520  nt calls to use 
-00028a50: 7468 6520 7361 6d65 2070 726f 6365 7373  the same process
-00028a60: 2070 6f6f 6c20 616e 6420 7265 7375 6c74   pool and result
-00028a70: 2069 6e20 6070 6172 616c 6c65 6c5f 6d61   in `parallel_ma
-00028a80: 7060 2069 6d6d 6564 6961 7465 6c79 2072  p` immediately r
-00028a90: 6574 7572 6e69 6e67 2061 206c 6973 7420  eturning a list 
-00028aa0: 7261 7468 6572 2074 6861 6e20 6120 6070  rather than a `p
-00028ab0: 6172 616c 6c65 6c5f 6d61 7060 206f 626a  arallel_map` obj
-00028ac0: 6563 742e 2049 6620 6d75 6c74 6970 6c65  ect. If multiple
-00028ad0: 2073 6571 7565 6e74 6961 6c20 6361 6c6c   sequential call
-00028ae0: 7320 6172 6520 6e65 6365 7373 6172 7920  s are necessary 
-00028af0: 616e 6420 7468 6520 6c61 7a69 6e65 7373  and the laziness
-00028b00: 206f 6620 7061 7261 6c6c 656c 5f6d 6170   of parallel_map
-00028b10: 2069 7320 7265 7175 6972 6564 2c20 7468   is required, th
-00028b20: 656e 2074 6865 2060 7061 7261 6c6c 656c  en the `parallel
-00028b30: 5f6d 6170 6020 6f62 6a65 6374 7320 7368  _map` objects sh
-00028b40: 6f75 6c64 2062 6520 636f 6e73 7472 7563  ould be construc
-00028b50: 7465 6420 6265 666f 7265 2074 6865 2060  ted before the `
-00028b60: 6d75 6c74 6970 6c65 5f73 6571 7565 6e74  multiple_sequent
-00028b70: 6961 6c5f 6361 6c6c 7360 2062 6c6f 636b  ial_calls` block
-00028b80: 2061 6e64 2074 6865 6e20 6f6e 6c79 2069   and then only i
-00028b90: 7465 7261 7465 6420 6f76 6572 206f 6e63  terated over onc
-00028ba0: 6520 696e 7369 6465 2074 6865 2062 6c6f  e inside the blo
-00028bb0: 636b 2e0a 0a60 7061 7261 6c6c 656c 5f6d  ck...`parallel_m
-00028bc0: 6170 2e6d 756c 7469 706c 655f 7365 7175  ap.multiple_sequ
-00028bd0: 656e 7469 616c 5f63 616c 6c73 6020 616c  ential_calls` al
-00028be0: 736f 2073 7570 706f 7274 7320 6120 606d  so supports a `m
-00028bf0: 6178 5f77 6f72 6b65 7273 6020 6172 6775  ax_workers` argu
-00028c00: 6d65 6e74 2074 6f20 7365 7420 7468 6520  ment to set the 
-00028c10: 6e75 6d62 6572 206f 6620 7072 6f63 6573  number of proces
-00028c20: 7365 732e 0a0a 2323 2323 2320 5079 7468  ses...##### Pyth
-00028c30: 6f6e 2044 6f63 730a 0a2a 2a70 6172 616c  on Docs..**paral
-00028c40: 6c65 6c5f 6d61 702a 2a28 5f66 756e 632c  lel_map**(_func,
-00028c50: 205c 2a69 7465 7261 626c 6573 5f2c 205f   \*iterables_, _
-00028c60: 6368 756e 6b73 697a 655f 3d60 3160 290a  chunksize_=`1`).
-00028c70: 0a45 7175 6976 616c 656e 7420 746f 2060  .Equivalent to `
-00028c80: 6d61 7028 6675 6e63 2c20 2a69 7465 7261  map(func, *itera
-00028c90: 626c 6573 2960 2065 7863 6570 7420 5f66  bles)` except _f
-00028ca0: 756e 635f 2069 7320 6578 6563 7574 6564  unc_ is executed
-00028cb0: 2061 7379 6e63 6872 6f6e 6f75 736c 7920   asynchronously 
-00028cc0: 616e 6420 7365 7665 7261 6c20 6361 6c6c  and several call
-00028cd0: 7320 746f 205f 6675 6e63 5f20 6d61 7920  s to _func_ may 
-00028ce0: 6265 206d 6164 6520 636f 6e63 7572 7265  be made concurre
-00028cf0: 6e74 6c79 2e20 4966 2061 2063 616c 6c20  ntly. If a call 
-00028d00: 7261 6973 6573 2061 6e20 6578 6365 7074  raises an except
-00028d10: 696f 6e2c 2074 6865 6e20 7468 6174 2065  ion, then that e
-00028d20: 7863 6570 7469 6f6e 2077 696c 6c20 6265  xception will be
-00028d30: 2072 6169 7365 6420 7768 656e 2069 7473   raised when its
-00028d40: 2076 616c 7565 2069 7320 7265 7472 6965   value is retrie
-00028d50: 7665 6420 6672 6f6d 2074 6865 2069 7465  ved from the ite
-00028d60: 7261 746f 722e 0a0a 6070 6172 616c 6c65  rator...`paralle
-00028d70: 6c5f 6d61 7060 2063 686f 7073 2074 6865  l_map` chops the
-00028d80: 2069 7465 7261 626c 6520 696e 746f 2061   iterable into a
-00028d90: 206e 756d 6265 7220 6f66 2063 6875 6e6b   number of chunk
-00028da0: 7320 7768 6963 6820 6974 2073 7562 6d69  s which it submi
-00028db0: 7473 2074 6f20 7468 6520 7072 6f63 6573  ts to the proces
-00028dc0: 7320 706f 6f6c 2061 7320 7365 7061 7261  s pool as separa
-00028dd0: 7465 2074 6173 6b73 2e20 5468 6520 2861  te tasks. The (a
-00028de0: 7070 726f 7869 6d61 7465 2920 7369 7a65  pproximate) size
-00028df0: 206f 6620 7468 6573 6520 6368 756e 6b73   of these chunks
-00028e00: 2063 616e 2062 6520 7370 6563 6966 6965   can be specifie
-00028e10: 6420 6279 2073 6574 7469 6e67 205f 6368  d by setting _ch
-00028e20: 756e 6b73 697a 655f 2074 6f20 6120 706f  unksize_ to a po
-00028e30: 7369 7469 7665 2069 6e74 6567 6572 2e20  sitive integer. 
-00028e40: 466f 7220 7665 7279 206c 6f6e 6720 6974  For very long it
-00028e50: 6572 6162 6c65 7320 7573 696e 6720 6120  erables using a 
-00028e60: 6c61 7267 6520 7661 6c75 6520 666f 7220  large value for 
-00028e70: 5f63 6875 6e6b 7369 7a65 5f20 6361 6e20  _chunksize_ can 
-00028e80: 6d61 6b65 2074 6865 206a 6f62 2063 6f6d  make the job com
-00028e90: 706c 6574 6520 2a2a 6d75 6368 2a2a 2066  plete **much** f
-00028ea0: 6173 7465 7220 7468 616e 2075 7369 6e67  aster than using
-00028eb0: 2074 6865 2064 6566 6175 6c74 2076 616c   the default val
-00028ec0: 7565 206f 6620 6031 602e 0a0a 2323 2323  ue of `1`...####
-00028ed0: 2320 4578 616d 706c 650a 0a2a 2a43 6f63  # Example..**Coc
-00028ee0: 6f6e 7574 3a2a 2a0a 6060 6063 6f63 6f6e  onut:**.```cocon
-00028ef0: 7574 0a70 6172 616c 6c65 6c5f 6d61 7028  ut.parallel_map(
-00028f00: 706f 7724 2832 292c 2072 616e 6765 2831  pow$(2), range(1
-00028f10: 3030 2929 207c 3e20 6c69 7374 207c 3e20  00)) |> list |> 
-00028f20: 7072 696e 740a 6060 600a 0a2a 2a50 7974  print.```..**Pyt
-00028f30: 686f 6e3a 2a2a 0a60 6060 636f 636f 6e75  hon:**.```coconu
-00028f40: 745f 7079 7468 6f6e 0a69 6d70 6f72 7420  t_python.import 
-00028f50: 6675 6e63 746f 6f6c 730a 6672 6f6d 206d  functools.from m
-00028f60: 756c 7469 7072 6f63 6573 7369 6e67 2069  ultiprocessing i
-00028f70: 6d70 6f72 7420 506f 6f6c 0a77 6974 6820  mport Pool.with 
-00028f80: 506f 6f6c 2829 2061 7320 706f 6f6c 3a0a  Pool() as pool:.
-00028f90: 2020 2020 7072 696e 7428 6c69 7374 2870      print(list(p
-00028fa0: 6f6f 6c2e 696d 6170 2866 756e 6374 6f6f  ool.imap(functoo
-00028fb0: 6c73 2e70 6172 7469 616c 2870 6f77 2c20  ls.partial(pow, 
-00028fc0: 3229 2c20 7261 6e67 6528 3130 3029 2929  2), range(100)))
-00028fd0: 290a 6060 600a 0a23 2323 2320 6063 6f6e  ).```..#### `con
-00028fe0: 6375 7272 656e 745f 6d61 7060 0a0a 2a2a  current_map`..**
-00028ff0: 636f 6e63 7572 7265 6e74 5c5f 6d61 702a  concurrent\_map*
-00029000: 2a28 5f66 756e 6374 696f 6e5f 2c20 2a5f  *(_function_, *_
-00029010: 6974 6572 6162 6c65 735f 2c20 2a2c 205f  iterables_, *, _
-00029020: 6368 756e 6b73 697a 655f 3d60 3160 2c20  chunksize_=`1`, 
-00029030: 5f73 7472 6963 745f 3d60 4661 6c73 6560  _strict_=`False`
-00029040: 290a 0a43 6f63 6f6e 7574 2070 726f 7669  )..Coconut provi
-00029050: 6465 7320 6120 636f 6e63 7572 7265 6e74  des a concurrent
-00029060: 2076 6572 7369 6f6e 206f 6620 5b60 7061   version of [`pa
-00029070: 7261 6c6c 656c 5f6d 6170 605d 2823 7061  rallel_map`](#pa
-00029080: 7261 6c6c 656c 5f6d 6170 2920 756e 6465  rallel_map) unde
-00029090: 7220 7468 6520 6e61 6d65 2060 636f 6e63  r the name `conc
-000290a0: 7572 7265 6e74 5f6d 6170 602e 2060 636f  urrent_map`. `co
-000290b0: 6e63 7572 7265 6e74 5f6d 6170 6020 6265  ncurrent_map` be
-000290c0: 6861 7665 7320 6964 656e 7469 6361 6c6c  haves identicall
-000290d0: 7920 746f 2060 7061 7261 6c6c 656c 5f6d  y to `parallel_m
-000290e0: 6170 6020 2869 6e63 6c75 6469 6e67 2073  ap` (including s
-000290f0: 7570 706f 7274 2066 6f72 2060 636f 6e63  upport for `conc
-00029100: 7572 7265 6e74 5f6d 6170 2e6d 756c 7469  urrent_map.multi
-00029110: 706c 655f 7365 7175 656e 7469 616c 5f63  ple_sequential_c
-00029120: 616c 6c73 6029 2065 7863 6570 7420 7468  alls`) except th
-00029130: 6174 2069 7420 7573 6573 206d 756c 7469  at it uses multi
-00029140: 7468 7265 6164 696e 6720 696e 7374 6561  threading instea
-00029150: 6420 6f66 206d 756c 7469 7072 6f63 6573  d of multiproces
-00029160: 7369 6e67 2c20 616e 6420 6973 2074 6865  sing, and is the
-00029170: 7265 666f 7265 2070 7269 6d61 7269 6c79  refore primarily
-00029180: 2075 7365 6675 6c20 6f6e 6c79 2066 6f72   useful only for
-00029190: 2049 4f2d 626f 756e 6420 7461 736b 7320   IO-bound tasks 
-000291a0: 6475 6520 746f 2043 5079 7468 6f6e 2773  due to CPython's
-000291b0: 2047 6c6f 6261 6c20 496e 7465 7270 7265   Global Interpre
-000291c0: 7465 7220 4c6f 636b 2e0a 0a23 2323 2323  ter Lock...#####
-000291d0: 2050 7974 686f 6e20 446f 6373 0a0a 2a2a   Python Docs..**
-000291e0: 636f 6e63 7572 7265 6e74 5f6d 6170 2a2a  concurrent_map**
-000291f0: 285f 6675 6e63 2c20 5c2a 6974 6572 6162  (_func, \*iterab
-00029200: 6c65 735f 2c20 5f63 6875 6e6b 7369 7a65  les_, _chunksize
-00029210: 5f3d 6031 6029 0a0a 4571 7569 7661 6c65  _=`1`)..Equivale
-00029220: 6e74 2074 6f20 606d 6170 2866 756e 632c  nt to `map(func,
-00029230: 202a 6974 6572 6162 6c65 7329 6020 6578   *iterables)` ex
-00029240: 6365 7074 205f 6675 6e63 5f20 6973 2065  cept _func_ is e
-00029250: 7865 6375 7465 6420 6173 796e 6368 726f  xecuted asynchro
-00029260: 6e6f 7573 6c79 2061 6e64 2073 6576 6572  nously and sever
-00029270: 616c 2063 616c 6c73 2074 6f20 5f66 756e  al calls to _fun
-00029280: 635f 206d 6179 2062 6520 6d61 6465 2063  c_ may be made c
-00029290: 6f6e 6375 7272 656e 746c 792e 2049 6620  oncurrently. If 
-000292a0: 6120 6361 6c6c 2072 6169 7365 7320 616e  a call raises an
-000292b0: 2065 7863 6570 7469 6f6e 2c20 7468 656e   exception, then
-000292c0: 2074 6861 7420 6578 6365 7074 696f 6e20   that exception 
-000292d0: 7769 6c6c 2062 6520 7261 6973 6564 2077  will be raised w
-000292e0: 6865 6e20 6974 7320 7661 6c75 6520 6973  hen its value is
-000292f0: 2072 6574 7269 6576 6564 2066 726f 6d20   retrieved from 
-00029300: 7468 6520 6974 6572 6174 6f72 2e0a 0a60  the iterator...`
-00029310: 636f 6e63 7572 7265 6e74 5f6d 6170 6020  concurrent_map` 
-00029320: 6368 6f70 7320 7468 6520 6974 6572 6162  chops the iterab
-00029330: 6c65 2069 6e74 6f20 6120 6e75 6d62 6572  le into a number
-00029340: 206f 6620 6368 756e 6b73 2077 6869 6368   of chunks which
-00029350: 2069 7420 7375 626d 6974 7320 746f 2074   it submits to t
-00029360: 6865 2074 6872 6561 6420 706f 6f6c 2061  he thread pool a
-00029370: 7320 7365 7061 7261 7465 2074 6173 6b73  s separate tasks
-00029380: 2e20 5468 6520 2861 7070 726f 7869 6d61  . The (approxima
-00029390: 7465 2920 7369 7a65 206f 6620 7468 6573  te) size of thes
-000293a0: 6520 6368 756e 6b73 2063 616e 2062 6520  e chunks can be 
-000293b0: 7370 6563 6966 6965 6420 6279 2073 6574  specified by set
-000293c0: 7469 6e67 205f 6368 756e 6b73 697a 655f  ting _chunksize_
-000293d0: 2074 6f20 6120 706f 7369 7469 7665 2069   to a positive i
-000293e0: 6e74 6567 6572 2e20 466f 7220 7665 7279  nteger. For very
-000293f0: 206c 6f6e 6720 6974 6572 6162 6c65 7320   long iterables 
-00029400: 7573 696e 6720 6120 6c61 7267 6520 7661  using a large va
-00029410: 6c75 6520 666f 7220 5f63 6875 6e6b 7369  lue for _chunksi
-00029420: 7a65 5f20 6361 6e20 6d61 6b65 2074 6865  ze_ can make the
-00029430: 206a 6f62 2063 6f6d 706c 6574 6520 2a2a   job complete **
-00029440: 6d75 6368 2a2a 2066 6173 7465 7220 7468  much** faster th
-00029450: 616e 2075 7369 6e67 2074 6865 2064 6566  an using the def
-00029460: 6175 6c74 2076 616c 7565 206f 6620 6031  ault value of `1
-00029470: 602e 0a0a 2323 2323 2320 4578 616d 706c  `...##### Exampl
-00029480: 650a 0a2a 2a43 6f63 6f6e 7574 3a2a 2a0a  e..**Coconut:**.
-00029490: 6060 6063 6f63 6f6e 7574 0a63 6f6e 6375  ```coconut.concu
-000294a0: 7272 656e 745f 6d61 7028 6765 745f 6461  rrent_map(get_da
-000294b0: 7461 5f66 6f72 5f75 7365 722c 2067 6574  ta_for_user, get
-000294c0: 5f61 6c6c 5f75 7365 7273 2829 2920 7c3e  _all_users()) |>
-000294d0: 206c 6973 7420 7c3e 2070 7269 6e74 0a60   list |> print.`
-000294e0: 6060 0a0a 2a2a 5079 7468 6f6e 3a2a 2a0a  ``..**Python:**.
-000294f0: 6060 6063 6f63 6f6e 7574 5f70 7974 686f  ```coconut_pytho
-00029500: 6e0a 696d 706f 7274 2066 756e 6374 6f6f  n.import functoo
-00029510: 6c73 0a69 6d70 6f72 7420 636f 6e63 7572  ls.import concur
-00029520: 7265 6e74 2e66 7574 7572 6573 0a77 6974  rent.futures.wit
-00029530: 6820 636f 6e63 7572 7265 6e74 2e66 7574  h concurrent.fut
-00029540: 7572 6573 2e54 6872 6561 6450 6f6f 6c45  ures.ThreadPoolE
-00029550: 7865 6375 746f 7228 2920 6173 2065 7865  xecutor() as exe
-00029560: 6375 746f 723a 0a20 2020 2070 7269 6e74  cutor:.    print
-00029570: 286c 6973 7428 6578 6563 7574 6f72 2e6d  (list(executor.m
-00029580: 6170 2867 6574 5f64 6174 615f 666f 725f  ap(get_data_for_
-00029590: 7573 6572 2c20 6765 745f 616c 6c5f 7573  user, get_all_us
-000295a0: 6572 7328 2929 2929 0a60 6060 0a0a 2323  ers()))).```..##
-000295b0: 2323 2060 7465 6560 0a0a 2a2a 7465 652a  ## `tee`..**tee*
-000295c0: 2a28 5f69 7465 7261 626c 655f 2c20 5f6e  *(_iterable_, _n
-000295d0: 5f3d 6032 6029 0a0a 436f 636f 6e75 7420  _=`2`)..Coconut 
-000295e0: 7072 6f76 6964 6573 2061 6e20 6f70 7469  provides an opti
-000295f0: 6d69 7a65 6420 7665 7273 696f 6e20 6f66  mized version of
-00029600: 2060 6974 6572 746f 6f6c 732e 7465 6560   `itertools.tee`
-00029610: 2061 7320 6120 6275 696c 742d 696e 2075   as a built-in u
-00029620: 6e64 6572 2074 6865 206e 616d 6520 6074  nder the name `t
-00029630: 6565 602e 0a0a 5468 6f75 6768 2060 7465  ee`...Though `te
-00029640: 6560 2069 7320 6e6f 7420 6465 7072 6563  e` is not deprec
-00029650: 6174 6564 2c20 5b60 7265 6974 6572 6162  ated, [`reiterab
-00029660: 6c65 605d 2823 7265 6974 6572 6162 6c65  le`](#reiterable
-00029670: 2920 6973 2067 656e 6572 616c 6c79 2072  ) is generally r
-00029680: 6563 6f6d 6d65 6e64 6564 206f 7665 7220  ecommended over 
-00029690: 6074 6565 602e 0a0a 4375 7374 6f6d 2060  `tee`...Custom `
-000296a0: 7465 6560 2f60 7265 6974 6572 6162 6c65  tee`/`reiterable
-000296b0: 6020 696d 706c 656d 656e 7461 7469 6f6e  ` implementation
-000296c0: 7320 666f 7220 6375 7374 6f6d 205b 436f  s for custom [Co
-000296d0: 6e74 6169 6e65 7273 2f43 6f6c 6c65 6374  ntainers/Collect
-000296e0: 696f 6e73 5d28 6874 7470 733a 2f2f 646f  ions](https://do
-000296f0: 6373 2e70 7974 686f 6e2e 6f72 672f 332f  cs.python.org/3/
-00029700: 6c69 6272 6172 792f 636f 6c6c 6563 7469  library/collecti
-00029710: 6f6e 732e 6162 632e 6874 6d6c 2920 7368  ons.abc.html) sh
-00029720: 6f75 6c64 2062 6520 7075 7420 696e 2074  ould be put in t
-00029730: 6865 2060 5f5f 636f 7079 5f5f 6020 6d65  he `__copy__` me
-00029740: 7468 6f64 2e20 4e6f 7465 2074 6861 7420  thod. Note that 
-00029750: 616c 6c20 5b53 6571 7565 6e63 6573 2f4d  all [Sequences/M
-00029760: 6170 7069 6e67 732f 5365 7473 5d28 6874  appings/Sets](ht
-00029770: 7470 733a 2f2f 646f 6373 2e70 7974 686f  tps://docs.pytho
-00029780: 6e2e 6f72 672f 332f 6c69 6272 6172 792f  n.org/3/library/
-00029790: 636f 6c6c 6563 7469 6f6e 732e 6162 632e  collections.abc.
-000297a0: 6874 6d6c 2920 6172 6520 616c 7761 7973  html) are always
-000297b0: 2061 7373 756d 6564 2074 6f20 6265 2072   assumed to be r
-000297c0: 6569 7465 7261 626c 6520 6576 656e 2077  eiterable even w
-000297d0: 6974 686f 7574 2063 616c 6c69 6e67 2060  ithout calling `
-000297e0: 5f5f 636f 7079 5f5f 602e 0a0a 2323 2323  __copy__`...####
-000297f0: 2320 5079 7468 6f6e 2044 6f63 730a 0a2a  # Python Docs..*
-00029800: 2a74 6565 2a2a 285f 6974 6572 6162 6c65  *tee**(_iterable
-00029810: 2c20 6e3d 325f 290a 0a52 6574 7572 6e20  , n=2_)..Return 
-00029820: 5f6e 5f20 696e 6465 7065 6e64 656e 7420  _n_ independent 
-00029830: 6974 6572 6174 6f72 7320 6672 6f6d 2061  iterators from a
-00029840: 2073 696e 676c 6520 6974 6572 6162 6c65   single iterable
-00029850: 2e20 4571 7569 7661 6c65 6e74 2074 6f3a  . Equivalent to:
-00029860: 0a60 6060 636f 636f 6e75 745f 7079 7468  .```coconut_pyth
-00029870: 6f6e 0a64 6566 2074 6565 2869 7465 7261  on.def tee(itera
-00029880: 626c 652c 206e 3d32 293a 0a20 2020 2069  ble, n=2):.    i
-00029890: 7420 3d20 6974 6572 2869 7465 7261 626c  t = iter(iterabl
-000298a0: 6529 0a20 2020 2064 6571 7565 7320 3d20  e).    deques = 
-000298b0: 5b63 6f6c 6c65 6374 696f 6e73 2e64 6571  [collections.deq
-000298c0: 7565 2829 2066 6f72 2069 2069 6e20 7261  ue() for i in ra
-000298d0: 6e67 6528 6e29 5d0a 2020 2020 6465 6620  nge(n)].    def 
-000298e0: 6765 6e28 6d79 6465 7175 6529 3a0a 2020  gen(mydeque):.  
-000298f0: 2020 2020 2020 7768 696c 6520 5472 7565        while True
-00029900: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-00029910: 206e 6f74 206d 7964 6571 7565 3a20 2020   not mydeque:   
-00029920: 2020 2020 2020 2020 2020 2320 7768 656e            # when
-00029930: 2074 6865 206c 6f63 616c 2064 6571 7565   the local deque
-00029940: 2069 7320 656d 7074 790a 2020 2020 2020   is empty.      
-00029950: 2020 2020 2020 2020 2020 6e65 7776 616c            newval
-00029960: 203d 206e 6578 7428 6974 2920 2020 2020   = next(it)     
-00029970: 2020 2320 6665 7463 6820 6120 6e65 7720    # fetch a new 
-00029980: 7661 6c75 6520 616e 640a 2020 2020 2020  value and.      
-00029990: 2020 2020 2020 2020 2020 666f 7220 6420            for d 
-000299a0: 696e 2064 6571 7565 733a 2020 2020 2020  in deques:      
-000299b0: 2020 2320 6c6f 6164 2069 7420 746f 2061    # load it to a
-000299c0: 6c6c 2074 6865 2064 6571 7565 730a 2020  ll the deques.  
-000299d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000299e0: 2020 642e 6170 7065 6e64 286e 6577 7661    d.append(newva
-000299f0: 6c29 0a20 2020 2020 2020 2020 2020 2079  l).            y
-00029a00: 6965 6c64 206d 7964 6571 7565 2e70 6f70  ield mydeque.pop
-00029a10: 6c65 6674 2829 0a20 2020 2072 6574 7572  left().    retur
-00029a20: 6e20 7475 706c 6528 6765 6e28 6429 2066  n tuple(gen(d) f
-00029a30: 6f72 2064 2069 6e20 6465 7175 6573 290a  or d in deques).
-00029a40: 6060 600a 4f6e 6365 2060 7465 6528 2960  ```.Once `tee()`
-00029a50: 2068 6173 206d 6164 6520 6120 7370 6c69   has made a spli
-00029a60: 742c 2074 6865 206f 7269 6769 6e61 6c20  t, the original 
-00029a70: 5f69 7465 7261 626c 655f 2073 686f 756c  _iterable_ shoul
-00029a80: 6420 6e6f 7420 6265 2075 7365 6420 616e  d not be used an
-00029a90: 7977 6865 7265 2065 6c73 653b 206f 7468  ywhere else; oth
-00029aa0: 6572 7769 7365 2c20 7468 6520 5f69 7465  erwise, the _ite
-00029ab0: 7261 626c 655f 2063 6f75 6c64 2067 6574  rable_ could get
-00029ac0: 2061 6476 616e 6365 6420 7769 7468 6f75   advanced withou
-00029ad0: 7420 7468 6520 7465 6520 6f62 6a65 6374  t the tee object
-00029ae0: 7320 6265 696e 6720 696e 666f 726d 6564  s being informed
-00029af0: 2e0a 0a54 6869 7320 6974 6572 746f 6f6c  ...This itertool
-00029b00: 206d 6179 2072 6571 7569 7265 2073 6967   may require sig
-00029b10: 6e69 6669 6361 6e74 2061 7578 696c 6961  nificant auxilia
-00029b20: 7279 2073 746f 7261 6765 2028 6465 7065  ry storage (depe
-00029b30: 6e64 696e 6720 6f6e 2068 6f77 206d 7563  nding on how muc
-00029b40: 6820 7465 6d70 6f72 6172 7920 6461 7461  h temporary data
-00029b50: 206e 6565 6473 2074 6f20 6265 2073 746f   needs to be sto
-00029b60: 7265 6429 2e20 496e 2067 656e 6572 616c  red). In general
-00029b70: 2c20 6966 206f 6e65 2069 7465 7261 746f  , if one iterato
-00029b80: 7220 7573 6573 206d 6f73 7420 6f72 2061  r uses most or a
-00029b90: 6c6c 206f 6620 7468 6520 6461 7461 2062  ll of the data b
-00029ba0: 6566 6f72 6520 616e 6f74 6865 7220 6974  efore another it
-00029bb0: 6572 6174 6f72 2073 7461 7274 732c 2069  erator starts, i
-00029bc0: 7420 6973 2066 6173 7465 7220 746f 2075  t is faster to u
-00029bd0: 7365 2060 6c69 7374 2829 6020 696e 7374  se `list()` inst
-00029be0: 6561 6420 6f66 2060 7465 6528 2960 2e0a  ead of `tee()`..
-00029bf0: 0a23 2323 2323 2045 7861 6d70 6c65 0a0a  .##### Example..
-00029c00: 2a2a 436f 636f 6e75 743a 2a2a 0a60 6060  **Coconut:**.```
-00029c10: 636f 636f 6e75 740a 6f72 6967 696e 616c  coconut.original
-00029c20: 2c20 7465 6d70 203d 2074 6565 286f 7269  , temp = tee(ori
-00029c30: 6769 6e61 6c29 0a73 6c69 6365 6420 3d20  ginal).sliced = 
-00029c40: 7465 6d70 245b 353a 5d0a 6060 600a 0a2a  temp$[5:].```..*
-00029c50: 2a50 7974 686f 6e3a 2a2a 0a60 6060 636f  *Python:**.```co
-00029c60: 636f 6e75 745f 7079 7468 6f6e 0a69 6d70  conut_python.imp
-00029c70: 6f72 7420 6974 6572 746f 6f6c 730a 6f72  ort itertools.or
-00029c80: 6967 696e 616c 2c20 7465 6d70 203d 2069  iginal, temp = i
-00029c90: 7465 7274 6f6f 6c73 2e74 6565 286f 7269  tertools.tee(ori
-00029ca0: 6769 6e61 6c29 0a73 6c69 6365 6420 3d20  ginal).sliced = 
-00029cb0: 6974 6572 746f 6f6c 732e 6973 6c69 6365  itertools.islice
-00029cc0: 2874 656d 702c 2035 2c20 4e6f 6e65 290a  (temp, 5, None).
-00029cd0: 6060 600a 0a23 2323 2320 6063 6f6e 7375  ```..#### `consu
-00029ce0: 6d65 600a 0a2a 2a63 6f6e 7375 6d65 2a2a  me`..**consume**
-00029cf0: 285f 6974 6572 6162 6c65 5f2c 205f 6b65  (_iterable_, _ke
-00029d00: 6570 5c5f 6c61 7374 5f3d 6030 6029 0a0a  ep\_last_=`0`)..
-00029d10: 436f 636f 6e75 7420 7072 6f76 6964 6573  Coconut provides
-00029d20: 2074 6865 2060 636f 6e73 756d 6560 2066   the `consume` f
-00029d30: 756e 6374 696f 6e20 746f 2065 6666 6963  unction to effic
-00029d40: 6965 6e74 6c79 2065 7868 6175 7374 2061  iently exhaust a
-00029d50: 6e20 6974 6572 6174 6f72 2061 6e64 2074  n iterator and t
-00029d60: 6875 7320 7065 7266 6f72 6d20 616e 7920  hus perform any 
-00029d70: 6c61 7a79 2065 7661 6c75 6174 696f 6e20  lazy evaluation 
-00029d80: 636f 6e74 6169 6e65 6420 7769 7468 696e  contained within
-00029d90: 2069 742e 2060 636f 6e73 756d 6560 2074   it. `consume` t
-00029da0: 616b 6573 206f 6e65 206f 7074 696f 6e61  akes one optiona
-00029db0: 6c20 6172 6775 6d65 6e74 2c20 606b 6565  l argument, `kee
-00029dc0: 705f 6c61 7374 602c 2074 6861 7420 6465  p_last`, that de
-00029dd0: 6661 756c 7473 2074 6f20 3020 616e 6420  faults to 0 and 
-00029de0: 7370 6563 6966 6965 7320 686f 7720 6d61  specifies how ma
-00029df0: 6e79 2c20 6966 2061 6e79 2c20 6974 656d  ny, if any, item
-00029e00: 7320 6672 6f6d 2074 6865 2065 6e64 2074  s from the end t
-00029e10: 6f20 7265 7475 726e 2061 7320 6120 7365  o return as a se
-00029e20: 7175 656e 6365 2028 604e 6f6e 6560 2077  quence (`None` w
-00029e30: 696c 6c20 6b65 6570 2061 6c6c 2065 6c65  ill keep all ele
-00029e40: 6d65 6e74 7329 2e0a 0a45 7175 6976 616c  ments)...Equival
-00029e50: 656e 7420 746f 3a0a 6060 6063 6f63 6f6e  ent to:.```cocon
-00029e60: 7574 0a64 6566 2063 6f6e 7375 6d65 2869  ut.def consume(i
-00029e70: 7465 7261 626c 652c 206b 6565 705f 6c61  terable, keep_la
-00029e80: 7374 3d30 293a 0a20 2020 2022 2222 4675  st=0):.    """Fu
-00029e90: 6c6c 7920 6578 6861 7573 7420 6974 6572  lly exhaust iter
-00029ea0: 6162 6c65 2061 6e64 2072 6574 7572 6e20  able and return 
-00029eb0: 7468 6520 6c61 7374 206b 6565 705f 6c61  the last keep_la
-00029ec0: 7374 2065 6c65 6d65 6e74 732e 2222 220a  st elements.""".
-00029ed0: 2020 2020 7265 7475 726e 2063 6f6c 6c65      return colle
-00029ee0: 6374 696f 6e73 2e64 6571 7565 2869 7465  ctions.deque(ite
-00029ef0: 7261 626c 652c 206d 6178 6c65 6e3d 6b65  rable, maxlen=ke
-00029f00: 6570 5f6c 6173 7429 2020 2320 6661 7374  ep_last)  # fast
-00029f10: 6573 7420 7761 7920 746f 2065 7868 6175  est way to exhau
-00029f20: 7374 2061 6e20 6974 6572 6174 6f72 0a60  st an iterator.`
-00029f30: 6060 0a0a 2323 2323 2320 5261 7469 6f6e  ``..##### Ration
-00029f40: 616c 650a 0a49 6e20 7468 6520 7072 6f63  ale..In the proc
-00029f50: 6573 7320 6f66 206c 617a 696c 7920 6170  ess of lazily ap
-00029f60: 706c 7969 6e67 206f 7065 7261 7469 6f6e  plying operation
-00029f70: 7320 746f 2069 7465 7261 746f 7273 2c20  s to iterators, 
-00029f80: 6576 656e 7475 616c 6c79 2061 2070 6f69  eventually a poi
-00029f90: 6e74 2069 7320 7265 6163 6865 6420 7768  nt is reached wh
-00029fa0: 6572 6520 6576 616c 7561 7469 6f6e 206f  ere evaluation o
-00029fb0: 6620 7468 6520 6974 6572 6174 6f72 2069  f the iterator i
-00029fc0: 7320 6e65 6365 7373 6172 792e 2054 6f20  s necessary. To 
-00029fd0: 646f 2074 6869 7320 6566 6669 6369 656e  do this efficien
-00029fe0: 746c 792c 2043 6f63 6f6e 7574 2070 726f  tly, Coconut pro
-00029ff0: 7669 6465 7320 7468 6520 6063 6f6e 7375  vides the `consu
-0002a000: 6d65 6020 6675 6e63 7469 6f6e 2c20 7768  me` function, wh
-0002a010: 6963 6820 7769 6c6c 2066 756c 6c79 2065  ich will fully e
-0002a020: 7868 6175 7374 2074 6865 2069 7465 7261  xhaust the itera
-0002a030: 746f 7220 6769 7665 6e20 746f 2069 742e  tor given to it.
-0002a040: 0a0a 2323 2323 2320 4578 616d 706c 650a  ..##### Example.
-0002a050: 0a2a 2a43 6f63 6f6e 7574 3a2a 2a0a 6060  .**Coconut:**.``
-0002a060: 6063 6f63 6f6e 7574 0a72 616e 6765 2831  `coconut.range(1
-0002a070: 3029 207c 3e20 6d61 7024 2828 7829 202d  0) |> map$((x) -
-0002a080: 3e20 782a 2a32 2920 7c3e 206d 6170 2428  > x**2) |> map$(
-0002a090: 7072 696e 7429 207c 3e20 636f 6e73 756d  print) |> consum
-0002a0a0: 650a 6060 600a 0a2a 2a50 7974 686f 6e3a  e.```..**Python:
-0002a0b0: 2a2a 0a60 6060 636f 636f 6e75 745f 7079  **.```coconut_py
-0002a0c0: 7468 6f6e 0a63 6f6c 6c65 6374 696f 6e73  thon.collections
-0002a0d0: 2e64 6571 7565 286d 6170 2870 7269 6e74  .deque(map(print
-0002a0e0: 2c20 6d61 7028 6c61 6d62 6461 2078 3a20  , map(lambda x: 
-0002a0f0: 782a 2a32 2c20 7261 6e67 6528 3130 2929  x**2, range(10))
-0002a100: 292c 206d 6178 6c65 6e3d 3029 0a60 6060  ), maxlen=0).```
-0002a110: 0a0a 2323 2320 5479 7069 6e67 2d53 7065  ..### Typing-Spe
-0002a120: 6369 6669 6320 4275 696c 742d 496e 730a  cific Built-Ins.
-0002a130: 0a60 6060 7b63 6f6e 7465 6e74 737d 0a2d  .```{contents}.-
-0002a140: 2d2d 0a6c 6f63 616c 3a0a 6465 7074 683a  --.local:.depth:
-0002a150: 2031 0a2d 2d2d 0a60 6060 0a0a 2323 2323   1.---.```..####
-0002a160: 2060 5459 5045 5f43 4845 434b 494e 4760   `TYPE_CHECKING`
-0002a170: 0a0a 5468 6520 6054 5950 455f 4348 4543  ..The `TYPE_CHEC
-0002a180: 4b49 4e47 6020 7661 7269 6162 6c65 2069  KING` variable i
-0002a190: 7320 7365 7420 746f 2060 4661 6c73 6560  s set to `False`
-0002a1a0: 2061 7420 7275 6e74 696d 6520 616e 6420   at runtime and 
-0002a1b0: 6054 7275 6560 2064 7572 696e 6720 7479  `True` during ty
-0002a1c0: 7065 5f63 6865 636b 696e 672c 2061 6c6c  pe_checking, all
-0002a1d0: 6f77 696e 6720 796f 7520 746f 2070 7265  owing you to pre
-0002a1e0: 7665 6e74 2079 6f75 7220 6074 7970 696e  vent your `typin
-0002a1f0: 6760 2069 6d70 6f72 7473 2061 6e64 2060  g` imports and `
-0002a200: 5479 7065 5661 7260 2064 6566 696e 6974  TypeVar` definit
-0002a210: 696f 6e73 2066 726f 6d20 6265 696e 6720  ions from being 
-0002a220: 6578 6563 7574 6564 2061 7420 7275 6e74  executed at runt
-0002a230: 696d 652e 2042 7920 7772 6170 7069 6e67  ime. By wrapping
-0002a240: 2079 6f75 7220 6074 7970 696e 6760 2069   your `typing` i
-0002a250: 6d70 6f72 7473 2069 6e20 616e 2060 6966  mports in an `if
-0002a260: 2054 5950 455f 4348 4543 4b49 4e47 3a60   TYPE_CHECKING:`
-0002a270: 2062 6c6f 636b 2c20 796f 7520 6361 6e20   block, you can 
-0002a280: 6576 656e 2075 7365 2074 6865 205b 6074  even use the [`t
-0002a290: 7970 696e 6760 5d28 6874 7470 733a 2f2f  yping`](https://
-0002a2a0: 646f 6373 2e70 7974 686f 6e2e 6f72 672f  docs.python.org/
-0002a2b0: 332f 6c69 6272 6172 792f 7479 7069 6e67  3/library/typing
-0002a2c0: 2e68 746d 6c29 206d 6f64 756c 6520 6f6e  .html) module on
-0002a2d0: 2050 7974 686f 6e20 7665 7273 696f 6e73   Python versions
-0002a2e0: 2074 6861 7420 646f 6e27 7420 6e61 7469   that don't nati
-0002a2f0: 7665 6c79 2073 7570 706f 7274 2069 742e  vely support it.
-0002a300: 2046 7572 7468 6572 6d6f 7265 2c20 6054   Furthermore, `T
-0002a310: 5950 455f 4348 4543 4b49 4e47 6020 6361  YPE_CHECKING` ca
-0002a320: 6e20 616c 736f 2062 6520 7573 6564 2074  n also be used t
-0002a330: 6f20 6869 6465 2063 6f64 6520 7468 6174  o hide code that
-0002a340: 2069 7320 6d69 7374 7970 6564 2062 7920   is mistyped by 
-0002a350: 6465 6661 756c 742e 0a0a 2323 2323 2320  default...##### 
-0002a360: 5079 7468 6f6e 2044 6f63 730a 0a41 2073  Python Docs..A s
-0002a370: 7065 6369 616c 2063 6f6e 7374 616e 7420  pecial constant 
-0002a380: 7468 6174 2069 7320 6173 7375 6d65 6420  that is assumed 
-0002a390: 746f 2062 6520 6054 7275 6560 2062 7920  to be `True` by 
-0002a3a0: 3372 6420 7061 7274 7920 7374 6174 6963  3rd party static
-0002a3b0: 2074 7970 6520 6368 6563 6b65 7273 2e20   type checkers. 
-0002a3c0: 4974 2069 7320 6046 616c 7365 6020 6174  It is `False` at
-0002a3d0: 2072 756e 7469 6d65 2e20 5573 6167 653a   runtime. Usage:
-0002a3e0: 0a60 6060 636f 636f 6e75 745f 7079 7468  .```coconut_pyth
-0002a3f0: 6f6e 0a69 6620 5459 5045 5f43 4845 434b  on.if TYPE_CHECK
-0002a400: 494e 473a 0a20 2020 2069 6d70 6f72 7420  ING:.    import 
-0002a410: 6578 7065 6e73 6976 655f 6d6f 640a 0a64  expensive_mod..d
-0002a420: 6566 2066 756e 2861 7267 3a20 6578 7065  ef fun(arg: expe
-0002a430: 6e73 6976 655f 6d6f 642e 536f 6d65 5479  nsive_mod.SomeTy
-0002a440: 7065 2920 2d3e 204e 6f6e 653a 0a20 2020  pe) -> None:.   
-0002a450: 206c 6f63 616c 5f76 6172 3a20 6578 7065   local_var: expe
-0002a460: 6e73 6976 655f 6d6f 642e 416e 6f74 6865  nsive_mod.Anothe
-0002a470: 7254 7970 6520 3d20 6f74 6865 725f 6675  rType = other_fu
-0002a480: 6e28 290a 6060 600a 0a23 2323 2323 2045  n().```..##### E
-0002a490: 7861 6d70 6c65 730a 0a2a 2a43 6f63 6f6e  xamples..**Cocon
-0002a4a0: 7574 3a2a 2a0a 6060 6063 6f63 6f6e 7574  ut:**.```coconut
-0002a4b0: 0a69 6620 5459 5045 5f43 4845 434b 494e  .if TYPE_CHECKIN
-0002a4c0: 473a 0a20 2020 2066 726f 6d20 7479 7069  G:.    from typi
-0002a4d0: 6e67 2069 6d70 6f72 7420 4c69 7374 0a78  ng import List.x
-0002a4e0: 3a20 4c69 7374 5b73 7472 5d20 3d20 5b22  : List[str] = ["
-0002a4f0: 6122 2c20 2262 225d 0a60 6060 0a0a 6060  a", "b"].```..``
-0002a500: 6063 6f63 6f6e 7574 0a69 6620 5459 5045  `coconut.if TYPE
-0002a510: 5f43 4845 434b 494e 473a 0a20 2020 2064  _CHECKING:.    d
-0002a520: 6566 2066 6163 746f 7269 616c 286e 3a20  ef factorial(n: 
-0002a530: 696e 7429 202d 3e20 696e 743a 202e 2e2e  int) -> int: ...
-0002a540: 0a65 6c73 653a 0a20 2020 2064 6566 2066  .else:.    def f
-0002a550: 6163 746f 7269 616c 2830 2920 3d20 310a  actorial(0) = 1.
-0002a560: 2020 2020 6164 6470 6174 7465 726e 2064      addpattern d
-0002a570: 6566 2066 6163 746f 7269 616c 286e 2920  ef factorial(n) 
-0002a580: 3d20 6e20 2a20 6661 6374 6f72 6961 6c28  = n * factorial(
-0002a590: 6e2d 3129 0a60 6060 0a0a 2a2a 5079 7468  n-1).```..**Pyth
-0002a5a0: 6f6e 3a2a 2a0a 6060 6063 6f63 6f6e 7574  on:**.```coconut
-0002a5b0: 5f70 7974 686f 6e0a 7472 793a 0a20 2020  _python.try:.   
-0002a5c0: 2066 726f 6d20 7479 7069 6e67 2069 6d70   from typing imp
-0002a5d0: 6f72 7420 5459 5045 5f43 4845 434b 494e  ort TYPE_CHECKIN
-0002a5e0: 470a 6578 6365 7074 2049 6d70 6f72 7445  G.except ImportE
-0002a5f0: 7272 6f72 3a0a 2020 2020 5459 5045 5f43  rror:.    TYPE_C
-0002a600: 4845 434b 494e 4720 3d20 4661 6c73 650a  HECKING = False.
-0002a610: 0a69 6620 5459 5045 5f43 4845 434b 494e  .if TYPE_CHECKIN
-0002a620: 473a 0a20 2020 2066 726f 6d20 7479 7069  G:.    from typi
-0002a630: 6e67 2069 6d70 6f72 7420 4c69 7374 0a78  ng import List.x
-0002a640: 3a20 4c69 7374 5b73 7472 5d20 3d20 5b22  : List[str] = ["
-0002a650: 6122 2c20 2262 225d 0a60 6060 0a0a 6060  a", "b"].```..``
-0002a660: 6063 6f63 6f6e 7574 5f70 7974 686f 6e0a  `coconut_python.
-0002a670: 7472 793a 0a20 2020 2066 726f 6d20 7479  try:.    from ty
-0002a680: 7069 6e67 2069 6d70 6f72 7420 5459 5045  ping import TYPE
-0002a690: 5f43 4845 434b 494e 470a 6578 6365 7074  _CHECKING.except
-0002a6a0: 2049 6d70 6f72 7445 7272 6f72 3a0a 2020   ImportError:.  
-0002a6b0: 2020 5459 5045 5f43 4845 434b 494e 4720    TYPE_CHECKING 
-0002a6c0: 3d20 4661 6c73 650a 0a69 6620 5459 5045  = False..if TYPE
-0002a6d0: 5f43 4845 434b 494e 473a 0a20 2020 2064  _CHECKING:.    d
-0002a6e0: 6566 2066 6163 746f 7269 616c 286e 3a20  ef factorial(n: 
-0002a6f0: 696e 7429 202d 3e20 696e 743a 202e 2e2e  int) -> int: ...
-0002a700: 0a65 6c73 653a 0a20 2020 2064 6566 2066  .else:.    def f
-0002a710: 6163 746f 7269 616c 286e 293a 0a20 2020  actorial(n):.   
-0002a720: 2020 2020 2069 6620 6e20 3d3d 2030 3a0a       if n == 0:.
-0002a730: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0002a740: 726e 2031 0a20 2020 2020 2020 2065 6c73  rn 1.        els
-0002a750: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-0002a760: 6574 7572 6e20 6e20 2a20 6661 6374 6f72  eturn n * factor
-0002a770: 6961 6c28 6e2d 3129 0a60 6060 0a0a 2323  ial(n-1).```..##
-0002a780: 2323 2060 7265 7665 616c 5f74 7970 6560  ## `reveal_type`
-0002a790: 2061 6e64 2060 7265 7665 616c 5f6c 6f63   and `reveal_loc
-0002a7a0: 616c 7360 0a0a 5768 656e 2075 7369 6e67  als`..When using
-0002a7b0: 204d 7950 792c 2060 7265 7665 616c 5f74   MyPy, `reveal_t
-0002a7c0: 7970 6528 3c65 7870 723e 2960 2077 696c  ype(<expr>)` wil
-0002a7d0: 6c20 6361 7573 6520 4d79 5079 2074 6f20  l cause MyPy to 
-0002a7e0: 7072 696e 7420 7468 6520 7479 7065 206f  print the type o
-0002a7f0: 6620 603c 6578 7072 3e60 2061 6e64 2060  f `<expr>` and `
-0002a800: 7265 7665 616c 5f6c 6f63 616c 7328 2960  reveal_locals()`
-0002a810: 2077 696c 6c20 6361 7573 6520 4d79 5079   will cause MyPy
-0002a820: 2074 6f20 7072 696e 7420 7468 6520 7479   to print the ty
-0002a830: 7065 7320 6f66 2074 6865 2063 7572 7265  pes of the curre
-0002a840: 6e74 2060 6c6f 6361 6c73 2829 602e 2041  nt `locals()`. A
-0002a850: 7420 7275 6e74 696d 652c 2060 7265 7665  t runtime, `reve
-0002a860: 616c 5f74 7970 6528 7829 6020 6973 2061  al_type(x)` is a
-0002a870: 6c77 6179 7320 7468 6520 6964 656e 7469  lways the identi
-0002a880: 7479 2066 756e 6374 696f 6e20 616e 6420  ty function and 
-0002a890: 6072 6576 6561 6c5f 6c6f 6361 6c73 2829  `reveal_locals()
-0002a8a0: 6020 616c 7761 7973 2072 6574 7572 6e73  ` always returns
-0002a8b0: 2060 4e6f 6e65 602e 2053 6565 205b 7468   `None`. See [th
-0002a8c0: 6520 4d79 5079 2064 6f63 756d 656e 7461  e MyPy documenta
-0002a8d0: 7469 6f6e 5d28 6874 7470 733a 2f2f 6d79  tion](https://my
-0002a8e0: 7079 2e72 6561 6474 6865 646f 6373 2e69  py.readthedocs.i
-0002a8f0: 6f2f 656e 2f73 7461 626c 652f 636f 6d6d  o/en/stable/comm
-0002a900: 6f6e 5f69 7373 7565 732e 6874 6d6c 2372  on_issues.html#r
-0002a910: 6576 6561 6c2d 7479 7065 2920 666f 7220  eveal-type) for 
-0002a920: 6d6f 7265 2069 6e66 6f72 6d61 7469 6f6e  more information
-0002a930: 2e0a 0a23 2323 2323 2045 7861 6d70 6c65  ...##### Example
-0002a940: 0a0a 2a2a 436f 636f 6e75 743a 2a2a 0a60  ..**Coconut:**.`
-0002a950: 6060 636f 636f 6e75 745f 7079 636f 6e0a  ``coconut_pycon.
-0002a960: 3e20 636f 636f 6e75 7420 2d2d 6d79 7079  > coconut --mypy
-0002a970: 0a43 6f63 6f6e 7574 2049 6e74 6572 7072  .Coconut Interpr
-0002a980: 6574 6572 2076 582e 582e 583a 0a28 656e  eter vX.X.X:.(en
-0002a990: 7465 7220 2765 7869 7428 2927 206f 7220  ter 'exit()' or 
-0002a9a0: 7072 6573 7320 4374 726c 2d44 2074 6f20  press Ctrl-D to 
-0002a9b0: 656e 6429 0a3e 3e3e 2072 6576 6561 6c5f  end).>>> reveal_
-0002a9c0: 7479 7065 2866 6d61 7029 0a3c 6675 6e63  type(fmap).<func
-0002a9d0: 7469 6f6e 2066 6d61 7020 6174 2030 7830  tion fmap at 0x0
-0002a9e0: 3030 3030 3233 3942 3036 4532 3034 303e  0000239B06E2040>
-0002a9f0: 0a3c 7374 7269 6e67 3e3a 3137 3a20 6e6f  .<string>:17: no
-0002aa00: 7465 3a20 5265 7665 616c 6564 2074 7970  te: Revealed typ
-0002aa10: 6520 6973 2027 6465 6620 5b5f 542c 205f  e is 'def [_T, _
-0002aa20: 555d 2028 6675 6e63 3a20 6465 6620 285f  U] (func: def (_
-0002aa30: 5460 2d31 2920 2d3e 205f 5560 2d32 2c20  T`-1) -> _U`-2, 
-0002aa40: 6f62 6a3a 2074 7970 696e 672e 4974 6572  obj: typing.Iter
-0002aa50: 6162 6c65 5b5f 5460 2d31 5d29 202d 3e20  able[_T`-1]) -> 
-0002aa60: 7479 7069 6e67 2e49 7465 7261 626c 655b  typing.Iterable[
-0002aa70: 5f55 602d 325d 270a 3e3e 3e0a 6060 600a  _U`-2]'.>>>.```.
-0002aa80: 0a2a 2a50 7974 686f 6e2a 2a0a 6060 6063  .**Python**.```c
-0002aa90: 6f63 6f6e 7574 5f70 7974 686f 6e0a 7472  oconut_python.tr
-0002aaa0: 793a 0a20 2020 2066 726f 6d20 7479 7069  y:.    from typi
-0002aab0: 6e67 2069 6d70 6f72 7420 5459 5045 5f43  ng import TYPE_C
-0002aac0: 4845 434b 494e 470a 6578 6365 7074 2049  HECKING.except I
-0002aad0: 6d70 6f72 7445 7272 6f72 3a0a 2020 2020  mportError:.    
-0002aae0: 5459 5045 5f43 4845 434b 494e 4720 3d20  TYPE_CHECKING = 
-0002aaf0: 4661 6c73 650a 0a69 6620 6e6f 7420 5459  False..if not TY
-0002ab00: 5045 5f43 4845 434b 494e 473a 0a20 2020  PE_CHECKING:.   
-0002ab10: 2064 6566 2072 6576 6561 6c5f 7479 7065   def reveal_type
-0002ab20: 2878 293a 0a20 2020 2020 2020 2072 6574  (x):.        ret
-0002ab30: 7572 6e20 780a 0a66 726f 6d20 636f 636f  urn x..from coco
-0002ab40: 6e75 742e 5f5f 636f 636f 6e75 745f 5f20  nut.__coconut__ 
-0002ab50: 696d 706f 7274 2066 6d61 700a 7265 7665  import fmap.reve
-0002ab60: 616c 5f74 7970 6528 666d 6170 290a 6060  al_type(fmap).``
-0002ab70: 600a 0a23 2320 436f 636f 6e75 7420 4150  `..## Coconut AP
-0002ab80: 490a 0a60 6060 7b63 6f6e 7465 6e74 737d  I..```{contents}
-0002ab90: 0a2d 2d2d 0a6c 6f63 616c 3a0a 6465 7074  .---.local:.dept
-0002aba0: 683a 2032 0a2d 2d2d 0a60 6060 0a0a 2323  h: 2.---.```..##
-0002abb0: 2320 6063 6f63 6f6e 7574 2e65 6d62 6564  # `coconut.embed
-0002abc0: 600a 0a2a 2a63 6f63 6f6e 7574 2e65 6d62  `..**coconut.emb
-0002abd0: 6564 2a2a 285f 6b65 726e 656c 5f3d 604e  ed**(_kernel_=`N
-0002abe0: 6f6e 6560 2c20 5f64 6570 7468 5f3d 6030  one`, _depth_=`0
-0002abf0: 602c 205c 2a5c 2a5f 6b77 6172 6773 5f29  `, \*\*_kwargs_)
-0002ac00: 0a0a 4966 205f 6b65 726e 656c 5f3d 6046  ..If _kernel_=`F
-0002ac10: 616c 7365 6020 2864 6566 6175 6c74 292c  alse` (default),
-0002ac20: 2065 6d62 6564 7320 6120 436f 636f 6e75   embeds a Coconu
-0002ac30: 7420 4a75 7079 7465 7220 636f 6e73 6f6c  t Jupyter consol
-0002ac40: 6520 696e 6974 6961 6c69 7a65 6420 6672  e initialized fr
-0002ac50: 6f6d 2074 6865 2063 7572 7265 6e74 206c  om the current l
-0002ac60: 6f63 616c 206e 616d 6573 7061 6365 2e20  ocal namespace. 
-0002ac70: 4966 205f 6b65 726e 656c 5f3d 6054 7275  If _kernel_=`Tru
-0002ac80: 6560 2c20 6c61 756e 6368 6573 2061 2043  e`, launches a C
-0002ac90: 6f63 6f6e 7574 204a 7570 7974 6572 206b  oconut Jupyter k
-0002aca0: 6572 6e65 6c20 696e 6974 6961 6c69 7a65  ernel initialize
-0002acb0: 6420 6672 6f6d 2074 6865 206c 6f63 616c  d from the local
-0002acc0: 206e 616d 6573 7061 6365 2074 6861 7420   namespace that 
-0002acd0: 6361 6e20 7468 656e 2062 6520 6174 7461  can then be atta
-0002ace0: 6368 6564 2074 6f2e 2054 6865 205f 6465  ched to. The _de
-0002acf0: 7074 685f 2069 6e64 6963 6174 6573 2068  pth_ indicates h
-0002ad00: 6f77 206d 616e 7920 6164 6469 7469 6f6e  ow many addition
-0002ad10: 616c 2063 616c 6c20 6672 616d 6573 2074  al call frames t
-0002ad20: 6f20 6967 6e6f 7265 2e20 5f6b 7761 7267  o ignore. _kwarg
-0002ad30: 735f 2061 7265 2061 7320 696e 205b 4950  s_ are as in [IP
-0002ad40: 7974 686f 6e2e 656d 6265 645d 2868 7474  ython.embed](htt
-0002ad50: 7073 3a2f 2f69 7079 7468 6f6e 2e72 6561  ps://ipython.rea
-0002ad60: 6474 6865 646f 6373 2e69 6f2f 656e 2f73  dthedocs.io/en/s
-0002ad70: 7461 626c 652f 6170 692f 6765 6e65 7261  table/api/genera
-0002ad80: 7465 642f 4950 7974 686f 6e2e 7465 726d  ted/IPython.term
-0002ad90: 696e 616c 2e65 6d62 6564 2e68 746d 6c23  inal.embed.html#
-0002ada0: 4950 7974 686f 6e2e 7465 726d 696e 616c  IPython.terminal
-0002adb0: 2e65 6d62 6564 2e65 6d62 6564 2920 6f72  .embed.embed) or
-0002adc0: 205b 4950 7974 686f 6e2e 656d 6265 645f   [IPython.embed_
-0002add0: 6b65 726e 656c 5d28 6874 7470 733a 2f2f  kernel](https://
-0002ade0: 6970 7974 686f 6e2e 7265 6164 7468 6564  ipython.readthed
-0002adf0: 6f63 732e 696f 2f65 6e2f 7374 6162 6c65  ocs.io/en/stable
-0002ae00: 2f61 7069 2f67 656e 6572 6174 6564 2f49  /api/generated/I
-0002ae10: 5079 7468 6f6e 2e68 746d 6c23 4950 7974  Python.html#IPyt
-0002ae20: 686f 6e2e 656d 6265 645f 6b65 726e 656c  hon.embed_kernel
-0002ae30: 2920 6261 7365 6420 6f6e 205f 6b65 726e  ) based on _kern
-0002ae40: 656c 5f2e 0a0a 5265 636f 6d6d 656e 6465  el_...Recommende
-0002ae50: 6420 7573 6167 6520 6973 2061 7320 6120  d usage is as a 
-0002ae60: 6465 6275 6767 696e 6720 746f 6f6c 2c20  debugging tool, 
-0002ae70: 7768 6572 6520 7468 6520 636f 6465 2060  where the code `
-0002ae80: 6672 6f6d 2063 6f63 6f6e 7574 2069 6d70  from coconut imp
-0002ae90: 6f72 7420 656d 6265 643b 2065 6d62 6564  ort embed; embed
-0002aea0: 2829 6020 6361 6e20 6265 2069 6e73 6572  ()` can be inser
-0002aeb0: 7465 6420 746f 206c 6175 6e63 6820 616e  ted to launch an
-0002aec0: 2069 6e74 6572 6163 7469 7665 2043 6f63   interactive Coc
-0002aed0: 6f6e 7574 2073 6865 6c6c 2069 6e69 7469  onut shell initi
-0002aee0: 616c 697a 6564 2066 726f 6d20 7468 6174  alized from that
-0002aef0: 2070 6f69 6e74 2e0a 0a23 2323 2041 7574   point...### Aut
-0002af00: 6f6d 6174 6963 2043 6f6d 7069 6c61 7469  omatic Compilati
-0002af10: 6f6e 0a0a 4966 2079 6f75 2064 6f6e 2774  on..If you don't
-0002af20: 2063 6172 6520 6162 6f75 7420 7468 6520   care about the 
-0002af30: 6578 6163 7420 636f 6d70 696c 6174 696f  exact compilatio
-0002af40: 6e20 7061 7261 6d65 7465 7273 2079 6f75  n parameters you
-0002af50: 2077 616e 7420 746f 2075 7365 2c20 6175   want to use, au
-0002af60: 746f 6d61 7469 6320 636f 6d70 696c 6174  tomatic compilat
-0002af70: 696f 6e20 6c65 7473 2043 6f63 6f6e 7574  ion lets Coconut
-0002af80: 2074 616b 6520 6361 7265 206f 6620 6576   take care of ev
-0002af90: 6572 7974 6869 6e67 2066 6f72 2079 6f75  erything for you
-0002afa0: 2e20 4175 746f 6d61 7469 6320 636f 6d70  . Automatic comp
-0002afb0: 696c 6174 696f 6e20 6361 6e20 6265 2065  ilation can be e
-0002afc0: 6e61 626c 6564 2065 6974 6865 7220 6279  nabled either by
-0002afd0: 2069 6d70 6f72 7469 6e67 205b 6063 6f63   importing [`coc
-0002afe0: 6f6e 7574 2e63 6f6e 7665 6e69 656e 6365  onut.convenience
-0002aff0: 605d 2823 636f 636f 6e75 742d 636f 6e76  `](#coconut-conv
-0002b000: 656e 6965 6e63 6529 2062 6566 6f72 6520  enience) before 
-0002b010: 796f 7520 696d 706f 7274 2061 6e79 7468  you import anyth
-0002b020: 696e 6720 656c 7365 2c20 6f72 2062 7920  ing else, or by 
-0002b030: 7275 6e6e 696e 6720 6063 6f63 6f6e 7574  running `coconut
-0002b040: 202d 2d73 6974 652d 696e 7374 616c 6c60   --site-install`
-0002b050: 2e20 4f6e 6365 2061 7574 6f6d 6174 6963  . Once automatic
-0002b060: 2063 6f6d 7069 6c61 7469 6f6e 2069 7320   compilation is 
-0002b070: 656e 6162 6c65 642c 2043 6f63 6f6e 7574  enabled, Coconut
-0002b080: 2077 696c 6c20 6368 6563 6b20 6561 6368   will check each
-0002b090: 206f 6620 796f 7572 2069 6d70 6f72 7473   of your imports
-0002b0a0: 2074 6f20 7365 6520 6966 2079 6f75 2061   to see if you a
-0002b0b0: 7265 2061 7474 656d 7074 696e 6720 746f  re attempting to
-0002b0c0: 2069 6d70 6f72 7420 6120 602e 636f 636f   import a `.coco
-0002b0d0: 6020 6669 6c65 2061 6e64 2c20 6966 2073  ` file and, if s
-0002b0e0: 6f2c 2061 7574 6f6d 6174 6963 616c 6c79  o, automatically
-0002b0f0: 2063 6f6d 7069 6c65 2069 7420 666f 7220   compile it for 
-0002b100: 796f 752e 204e 6f74 6520 7468 6174 2c20  you. Note that, 
-0002b110: 666f 7220 436f 636f 6e75 7420 746f 206b  for Coconut to k
-0002b120: 6e6f 7720 7768 6174 2066 696c 6520 796f  now what file yo
-0002b130: 7520 6172 6520 7472 7969 6e67 2074 6f20  u are trying to 
-0002b140: 696d 706f 7274 2c20 6974 2077 696c 6c20  import, it will 
-0002b150: 6e65 6564 2074 6f20 6265 2061 6363 6573  need to be acces
-0002b160: 7369 626c 6520 7669 6120 6073 7973 2e70  sible via `sys.p
-0002b170: 6174 6860 2c20 6a75 7374 206c 696b 6520  ath`, just like 
-0002b180: 6120 6e6f 726d 616c 2069 6d70 6f72 742e  a normal import.
-0002b190: 0a0a 4175 746f 6d61 7469 6320 636f 6d70  ..Automatic comp
-0002b1a0: 696c 6174 696f 6e20 616c 7761 7973 2063  ilation always c
-0002b1b0: 6f6d 7069 6c65 7320 6d6f 6475 6c65 7320  ompiles modules 
-0002b1c0: 616e 6420 7061 636b 6167 6573 2069 6e2d  and packages in-
-0002b1d0: 706c 6163 652c 2061 6e64 2061 6c77 6179  place, and alway
-0002b1e0: 7320 7573 6573 2060 2d2d 7461 7267 6574  s uses `--target
-0002b1f0: 2073 7973 602e 2041 7574 6f6d 6174 6963   sys`. Automatic
-0002b200: 2063 6f6d 7069 6c61 7469 6f6e 2069 7320   compilation is 
-0002b210: 616c 7761 7973 2061 7661 696c 6162 6c65  always available
-0002b220: 2069 6e20 7468 6520 436f 636f 6e75 7420   in the Coconut 
-0002b230: 696e 7465 7270 7265 7465 722c 2061 6e64  interpreter, and
-0002b240: 2c20 6966 2075 7369 6e67 2074 6865 2043  , if using the C
-0002b250: 6f63 6f6e 7574 2069 6e74 6572 7072 6574  oconut interpret
-0002b260: 6572 2c20 6120 6072 656c 6f61 6460 2062  er, a `reload` b
-0002b270: 7569 6c74 2d69 6e20 6973 2070 726f 7669  uilt-in is provi
-0002b280: 6465 6420 746f 2065 6173 696c 7920 7265  ded to easily re
-0002b290: 6c6f 6164 2069 6d70 6f72 7465 6420 6d6f  load imported mo
-0002b2a0: 6475 6c65 732e 2041 6464 6974 696f 6e61  dules. Additiona
-0002b2b0: 6c6c 792c 2074 6865 2069 6e74 6572 7072  lly, the interpr
-0002b2c0: 6574 6572 2061 6c77 6179 7320 616c 6c6f  eter always allo
-0002b2d0: 7773 2069 6d70 6f72 7469 6e67 2066 726f  ws importing fro
-0002b2e0: 6d20 7468 6520 6375 7272 656e 7420 776f  m the current wo
-0002b2f0: 726b 696e 6720 6469 7265 6374 6f72 792c  rking directory,
-0002b300: 206c 6574 7469 6e67 2079 6f75 2065 6173   letting you eas
-0002b310: 696c 7920 636f 6d70 696c 6520 616e 6420  ily compile and 
-0002b320: 706c 6179 2061 726f 756e 6420 7769 7468  play around with
-0002b330: 2061 2060 2e63 6f63 6f60 2066 696c 6520   a `.coco` file 
-0002b340: 7369 6d70 6c79 2062 7920 7275 6e6e 696e  simply by runnin
-0002b350: 6720 7468 6520 436f 636f 6e75 7420 696e  g the Coconut in
-0002b360: 7465 7270 7265 7465 7220 616e 6420 696d  terpreter and im
-0002b370: 706f 7274 696e 6720 6974 2e0a 0a23 2323  porting it...###
-0002b380: 2043 6f63 6f6e 7574 2045 6e63 6f64 696e   Coconut Encodin
-0002b390: 670a 0a57 6869 6c65 2061 7574 6f6d 6174  g..While automat
-0002b3a0: 6963 2063 6f6d 7069 6c61 7469 6f6e 2069  ic compilation i
-0002b3b0: 7320 7468 6520 7072 6566 6572 7265 6420  s the preferred 
-0002b3c0: 6d65 7468 6f64 2066 6f72 2064 796e 616d  method for dynam
-0002b3d0: 6963 616c 6c79 2063 6f6d 7069 6c69 6e67  ically compiling
-0002b3e0: 2043 6f63 6f6e 7574 2066 696c 6573 2c20   Coconut files, 
-0002b3f0: 6173 2069 7420 6361 6368 6573 2074 6865  as it caches the
-0002b400: 2063 6f6d 7069 6c65 6420 636f 6465 2061   compiled code a
-0002b410: 7320 6120 602e 7079 6020 6669 6c65 2074  s a `.py` file t
-0002b420: 6f20 7072 6576 656e 7420 7265 636f 6d70  o prevent recomp
-0002b430: 696c 6174 696f 6e2c 2043 6f63 6f6e 7574  ilation, Coconut
-0002b440: 2061 6c73 6f20 7375 7070 6f72 7473 2061   also supports a
-0002b450: 2073 7065 6369 616c 0a60 6060 636f 636f   special.```coco
-0002b460: 6e75 740a 2320 636f 6469 6e67 3a20 636f  nut.# coding: co
-0002b470: 636f 6e75 740a 6060 600a 6465 636c 6172  conut.```.declar
-0002b480: 6174 696f 6e20 7768 6963 6820 6361 6e20  ation which can 
-0002b490: 6265 2061 6464 6564 2074 6f20 602e 7079  be added to `.py
-0002b4a0: 6020 6669 6c65 7320 746f 2068 6176 6520  ` files to have 
-0002b4b0: 7468 656d 2074 7265 6174 6564 2061 7320  them treated as 
-0002b4c0: 436f 636f 6e75 7420 6669 6c65 7320 696e  Coconut files in
-0002b4d0: 7374 6561 642e 2054 6f20 7573 6520 7375  stead. To use su
-0002b4e0: 6368 2061 2063 6f64 696e 6720 6465 636c  ch a coding decl
-0002b4f0: 6172 6174 696f 6e2c 2079 6f75 276c 6c20  aration, you'll 
-0002b500: 6e65 6564 2074 6f20 6569 7468 6572 2072  need to either r
-0002b510: 756e 2060 636f 636f 6e75 7420 2d2d 7369  un `coconut --si
-0002b520: 7465 2d69 6e73 7461 6c6c 6020 6f72 2060  te-install` or `
-0002b530: 696d 706f 7274 2063 6f63 6f6e 7574 2e63  import coconut.c
-0002b540: 6f6e 7665 6e69 656e 6365 6020 6174 2073  onvenience` at s
-0002b550: 6f6d 6520 706f 696e 7420 6265 666f 7265  ome point before
-0002b560: 2079 6f75 2066 6972 7374 2061 7474 656d   you first attem
-0002b570: 7074 2074 6f20 696d 706f 7274 2061 2066  pt to import a f
-0002b580: 696c 6520 7769 7468 2061 2060 2320 636f  ile with a `# co
-0002b590: 6469 6e67 3a20 636f 636f 6e75 7460 2064  ding: coconut` d
-0002b5a0: 6563 6c61 7261 7469 6f6e 2e20 4c69 6b65  eclaration. Like
-0002b5b0: 2061 7574 6f6d 6174 6963 2063 6f6d 7069   automatic compi
-0002b5c0: 6c61 7469 6f6e 2c20 636f 6d70 696c 6174  lation, compilat
-0002b5d0: 696f 6e20 6973 2061 6c77 6179 7320 646f  ion is always do
-0002b5e0: 6e65 2077 6974 6820 602d 2d74 6172 6765  ne with `--targe
-0002b5f0: 7420 7379 7360 2061 6e64 2069 7320 616c  t sys` and is al
-0002b600: 7761 7973 2061 7661 696c 6162 6c65 2066  ways available f
-0002b610: 726f 6d20 7468 6520 436f 636f 6e75 7420  rom the Coconut 
-0002b620: 696e 7465 7270 7265 7465 722e 0a0a 2323  interpreter...##
-0002b630: 2320 6063 6f63 6f6e 7574 2e63 6f6e 7665  # `coconut.conve
-0002b640: 6e69 656e 6365 600a 0a49 6e20 6164 6469  nience`..In addi
-0002b650: 7469 6f6e 2074 6f20 656e 6162 6c69 6e67  tion to enabling
-0002b660: 2061 7574 6f6d 6174 6963 2063 6f6d 7069   automatic compi
-0002b670: 6c61 7469 6f6e 2c20 6063 6f63 6f6e 7574  lation, `coconut
-0002b680: 2e63 6f6e 7665 6e69 656e 6365 6020 6361  .convenience` ca
-0002b690: 6e20 616c 736f 2062 6520 7573 6564 2074  n also be used t
-0002b6a0: 6f20 6361 6c6c 2074 6865 2043 6f63 6f6e  o call the Cocon
-0002b6b0: 7574 2063 6f6d 7069 6c65 7220 6672 6f6d  ut compiler from
-0002b6c0: 2063 6f64 6520 696e 7374 6561 6420 6f66   code instead of
-0002b6d0: 2066 726f 6d20 7468 6520 636f 6d6d 616e   from the comman
-0002b6e0: 6420 6c69 6e65 2e20 5365 6520 6265 6c6f  d line. See belo
-0002b6f0: 7720 666f 7220 7370 6563 6966 6963 6174  w for specificat
-0002b700: 696f 6e73 206f 6620 7468 6520 6469 6666  ions of the diff
-0002b710: 6572 656e 7420 636f 6e76 656e 6965 6e63  erent convenienc
-0002b720: 6520 6675 6e63 7469 6f6e 732e 0a0a 2323  e functions...##
-0002b730: 2323 2060 6765 745f 7374 6174 6560 0a0a  ## `get_state`..
-0002b740: 2a2a 636f 636f 6e75 742e 636f 6e76 656e  **coconut.conven
-0002b750: 6965 6e63 652e 6765 745c 5f73 7461 7465  ience.get\_state
-0002b760: 2a2a 285f 7374 6174 655f 3d60 4e6f 6e65  **(_state_=`None
-0002b770: 6029 0a0a 4765 7473 2061 2073 7461 7465  `)..Gets a state
-0002b780: 206f 626a 6563 7420 7768 6963 6820 7374   object which st
-0002b790: 6f72 6573 2074 6865 2063 7572 7265 6e74  ores the current
-0002b7a0: 2063 6f6d 7069 6c61 7469 6f6e 2070 6172   compilation par
-0002b7b0: 616d 6574 6572 732e 2053 7461 7465 206f  ameters. State o
-0002b7c0: 626a 6563 7473 2063 616e 2062 6520 636f  bjects can be co
-0002b7d0: 6e66 6967 7572 6564 2077 6974 6820 5b2a  nfigured with [*
-0002b7e0: 2a73 6574 7570 2a2a 5d28 2373 6574 7570  *setup**](#setup
-0002b7f0: 2920 6f72 205b 2a2a 636d 642a 2a5d 2823  ) or [**cmd**](#
-0002b800: 636d 6429 2061 6e64 2074 6865 6e20 7573  cmd) and then us
-0002b810: 6564 2069 6e20 5b2a 2a70 6172 7365 2a2a  ed in [**parse**
-0002b820: 5d28 2370 6172 7365 2920 6f72 205b 2a2a  ](#parse) or [**
-0002b830: 636f 636f 6e75 745c 5f65 7661 6c2a 2a5d  coconut\_eval**]
-0002b840: 2823 636f 636f 6e75 745f 6576 616c 292e  (#coconut_eval).
-0002b850: 0a0a 4966 205f 7374 6174 655f 2069 7320  ..If _state_ is 
-0002b860: 604e 6f6e 6560 2c20 6765 7473 2061 206e  `None`, gets a n
-0002b870: 6577 2073 7461 7465 206f 626a 6563 742c  ew state object,
-0002b880: 2077 6865 7265 6173 2069 6620 5f73 7461   whereas if _sta
-0002b890: 7465 5f20 6973 2060 4661 6c73 6560 2c20  te_ is `False`, 
-0002b8a0: 7468 6520 676c 6f62 616c 2073 7461 7465  the global state
-0002b8b0: 206f 626a 6563 7420 6973 2072 6574 7572   object is retur
-0002b8c0: 6e65 642e 0a0a 2323 2323 2060 7061 7273  ned...#### `pars
-0002b8d0: 6560 0a0a 2a2a 636f 636f 6e75 742e 636f  e`..**coconut.co
-0002b8e0: 6e76 656e 6965 6e63 652e 7061 7273 652a  nvenience.parse*
-0002b8f0: 2a28 5f63 6f64 655f 3d60 2222 602c 205f  *(_code_=`""`, _
-0002b900: 6d6f 6465 5f3d 6022 7379 7322 602c 205f  mode_=`"sys"`, _
-0002b910: 7374 6174 655f 3d60 4661 6c73 6560 2c20  state_=`False`, 
-0002b920: 5f6b 6565 705c 5f69 6e74 6572 6e61 6c5c  _keep\_internal\
-0002b930: 5f73 7461 7465 5f3d 604e 6f6e 6560 290a  _state_=`None`).
-0002b940: 0a4c 696b 656c 7920 7468 6520 6d6f 7374  .Likely the most
-0002b950: 2075 7365 6675 6c20 6f66 2074 6865 2063   useful of the c
-0002b960: 6f6e 7665 6e69 656e 6365 2066 756e 6374  onvenience funct
-0002b970: 696f 6e73 2c20 6070 6172 7365 6020 7461  ions, `parse` ta
-0002b980: 6b65 7320 436f 636f 6e75 7420 636f 6465  kes Coconut code
-0002b990: 2061 7320 696e 7075 7420 616e 6420 6f75   as input and ou
-0002b9a0: 7470 7574 7320 7468 6520 6571 7569 7661  tputs the equiva
-0002b9b0: 6c65 6e74 2063 6f6d 7069 6c65 6420 5079  lent compiled Py
-0002b9c0: 7468 6f6e 2063 6f64 652e 205f 6d6f 6465  thon code. _mode
-0002b9d0: 5f20 6973 2075 7365 6420 746f 2069 6e64  _ is used to ind
-0002b9e0: 6963 6174 6520 7468 6520 636f 6e74 6578  icate the contex
-0002b9f0: 7420 666f 7220 7468 6520 7061 7273 696e  t for the parsin
-0002ba00: 6720 616e 6420 5f73 7461 7465 5f20 6973  g and _state_ is
-0002ba10: 2074 6865 2073 7461 7465 206f 626a 6563   the state objec
-0002ba20: 7420 7374 6f72 696e 6720 7468 6520 636f  t storing the co
-0002ba30: 6d70 696c 6174 696f 6e20 7061 7261 6d65  mpilation parame
-0002ba40: 7465 7273 2074 6f20 7573 6520 6173 206f  ters to use as o
-0002ba50: 6274 6169 6e65 6420 6672 6f6d 205b 2a2a  btained from [**
-0002ba60: 6765 745f 7374 6174 652a 2a5d 2823 6765  get_state**](#ge
-0002ba70: 745f 7374 6174 6529 2028 6966 2060 4661  t_state) (if `Fa
-0002ba80: 6c73 6560 2c20 7573 6573 2074 6865 2067  lse`, uses the g
-0002ba90: 6c6f 6261 6c20 7374 6174 6520 6f62 6a65  lobal state obje
-0002baa0: 6374 292e 205f 6b65 6570 5c5f 696e 7465  ct). _keep\_inte
-0002bab0: 726e 616c 5c5f 7374 6174 655f 2064 6574  rnal\_state_ det
-0002bac0: 6572 6d69 6e65 7320 7768 6574 6865 7220  ermines whether 
-0002bad0: 7468 6520 7374 6174 6520 6f62 6a65 6374  the state object
-0002bae0: 2077 696c 6c20 6b65 6570 2069 6e74 6572   will keep inter
-0002baf0: 6e61 6c20 7374 6174 6520 2873 7563 6820  nal state (such 
-0002bb00: 6173 2077 6861 7420 5b63 7573 746f 6d20  as what [custom 
-0002bb10: 6f70 6572 6174 6f72 735d 2823 6375 7374  operators](#cust
-0002bb20: 6f6d 2d6f 7065 7261 746f 7273 2920 6861  om-operators) ha
-0002bb30: 7665 2062 6565 6e20 6465 636c 6172 6564  ve been declared
-0002bb40: 29e2 8094 6966 2060 4e6f 6e65 602c 2069  )...if `None`, i
-0002bb50: 6e74 6572 6e61 6c20 7374 6174 6520 7769  nternal state wi
-0002bb60: 6c6c 2062 6520 6b65 7074 2069 6666 2079  ll be kept iff y
-0002bb70: 6f75 2061 7265 206e 6f74 2075 7369 6e67  ou are not using
-0002bb80: 2074 6865 2067 6c6f 6261 6c20 5f73 7461   the global _sta
-0002bb90: 7465 5f2e 0a0a 4966 205f 636f 6465 5f20  te_...If _code_ 
-0002bba0: 6973 206e 6f74 2070 6173 7365 642c 2060  is not passed, `
-0002bbb0: 7061 7273 6560 2077 696c 6c20 6f75 7470  parse` will outp
-0002bbc0: 7574 206a 7573 7420 7468 6520 6769 7665  ut just the give
-0002bbd0: 6e20 5f6d 6f64 655f 2773 2068 6561 6465  n _mode_'s heade
-0002bbe0: 722c 2077 6869 6368 2063 616e 2062 6520  r, which can be 
-0002bbf0: 6578 6563 7574 6564 2074 6f20 7365 7420  executed to set 
-0002bc00: 7570 2061 6e20 6578 6563 7574 696f 6e20  up an execution 
-0002bc10: 656e 7669 726f 6e6d 656e 7420 696e 2077  environment in w
-0002bc20: 6869 6368 2066 7574 7572 6520 636f 6465  hich future code
-0002bc30: 2063 616e 2062 6520 7061 7273 6564 2061   can be parsed a
-0002bc40: 6e64 2065 7865 6375 7465 6420 7769 7468  nd executed with
-0002bc50: 6f75 7420 6120 6865 6164 6572 2e0a 0a45  out a header...E
-0002bc60: 6163 6820 5f6d 6f64 655f 2068 6173 2074  ach _mode_ has t
-0002bc70: 776f 2063 6f6d 706f 6e65 6e74 733a 2077  wo components: w
-0002bc80: 6861 7420 7061 7273 6572 2069 7420 7573  hat parser it us
-0002bc90: 6573 2c20 616e 6420 7768 6174 2068 6561  es, and what hea
-0002bca0: 6465 7220 6974 2070 7265 7065 6e64 732e  der it prepends.
-0002bcb0: 2054 6865 2070 6172 7365 7220 6465 7465   The parser dete
-0002bcc0: 726d 696e 6573 2077 6861 7420 436f 636f  rmines what Coco
-0002bcd0: 6e75 7420 636f 6465 2069 7320 616c 6c6f  nut code is allo
-0002bce0: 7765 6420 6173 2069 6e70 7574 2c20 616e  wed as input, an
-0002bcf0: 6420 7468 6520 6865 6164 6572 2064 6574  d the header det
-0002bd00: 6572 6d69 6e65 7320 686f 7720 7468 6520  ermines how the 
-0002bd10: 636f 6d70 696c 6564 2050 7974 686f 6e20  compiled Python 
-0002bd20: 6361 6e20 6265 2075 7365 642e 2050 6f73  can be used. Pos
-0002bd30: 7369 626c 6520 7661 6c75 6573 206f 6620  sible values of 
-0002bd40: 5f6d 6f64 655f 2061 7265 3a0a 0a2d 2060  _mode_ are:..- `
-0002bd50: 2273 7973 2260 3a20 2874 6865 2064 6566  "sys"`: (the def
-0002bd60: 6175 6c74 290a 2020 2020 2b20 7061 7273  ault).    + pars
-0002bd70: 6572 3a20 6669 6c65 0a20 2020 2020 2020  er: file.       
-0002bd80: 202a 2054 6865 2066 696c 6520 7061 7273   * The file pars
-0002bd90: 6572 2063 616e 2070 6172 7365 2061 6e79  er can parse any
-0002bda0: 2043 6f63 6f6e 7574 2063 6f64 652e 0a20   Coconut code.. 
-0002bdb0: 2020 202b 2068 6561 6465 723a 2073 7973     + header: sys
-0002bdc0: 0a20 2020 2020 2020 202a 2054 6869 7320  .        * This 
-0002bdd0: 6865 6164 6572 2069 6d70 6f72 7473 205b  header imports [
-0002bde0: 6063 6f63 6f6e 7574 2e5f 5f63 6f63 6f6e  `coconut.__cocon
-0002bdf0: 7574 5f5f 605d 2823 636f 636f 6e75 742d  ut__`](#coconut-
-0002be00: 636f 636f 6e75 7429 2074 6f20 6163 6365  coconut) to acce
-0002be10: 7373 2074 6865 206e 6563 6573 7361 7279  ss the necessary
-0002be20: 2043 6f63 6f6e 7574 206f 626a 6563 7473   Coconut objects
-0002be30: 2e0a 2d20 6022 6578 6563 2260 3a0a 2020  ..- `"exec"`:.  
-0002be40: 2020 2b20 7061 7273 6572 3a20 6669 6c65    + parser: file
-0002be50: 0a20 2020 202b 2068 6561 6465 723a 2065  .    + header: e
-0002be60: 7865 630a 2020 2020 2020 2020 2a20 5768  xec.        * Wh
-0002be70: 656e 2070 6173 7365 6420 746f 2060 6578  en passed to `ex
-0002be80: 6563 6020 6174 2074 6865 2067 6c6f 6261  ec` at the globa
-0002be90: 6c20 6c65 7665 6c2c 2074 6869 7320 6865  l level, this he
-0002bea0: 6164 6572 2077 696c 6c20 6372 6561 7465  ader will create
-0002beb0: 2061 6c6c 2074 6865 206e 6563 6573 7361   all the necessa
-0002bec0: 7279 2043 6f63 6f6e 7574 206f 626a 6563  ry Coconut objec
-0002bed0: 7473 2069 7473 656c 6620 696e 7374 6561  ts itself instea
-0002bee0: 6420 6f66 2069 6d70 6f72 7469 6e67 2074  d of importing t
-0002bef0: 6865 6d2e 0a2d 2060 2266 696c 6522 603a  hem..- `"file"`:
-0002bf00: 0a20 2020 202b 2070 6172 7365 723a 2066  .    + parser: f
-0002bf10: 696c 650a 2020 2020 2b20 6865 6164 6572  ile.    + header
-0002bf20: 3a20 6669 6c65 0a20 2020 2020 2020 202a  : file.        *
-0002bf30: 2054 6869 7320 6865 6164 6572 2069 7320   This header is 
-0002bf40: 6d65 616e 7420 746f 2062 6520 7772 6974  meant to be writ
-0002bf50: 7465 6e20 746f 2061 2060 2d2d 7374 616e  ten to a `--stan
-0002bf60: 6461 6c6f 6e65 6020 6669 6c65 2061 6e64  dalone` file and
-0002bf70: 2073 686f 756c 6420 6e6f 7420 6265 2070   should not be p
-0002bf80: 6173 7365 6420 746f 2060 6578 6563 602e  assed to `exec`.
-0002bf90: 0a2d 2060 2270 6163 6b61 6765 2260 3a0a  .- `"package"`:.
-0002bfa0: 2020 2020 2b20 7061 7273 6572 3a20 6669      + parser: fi
-0002bfb0: 6c65 0a20 2020 202b 2068 6561 6465 723a  le.    + header:
-0002bfc0: 2070 6163 6b61 6765 0a20 2020 2020 2020   package.       
-0002bfd0: 202a 2054 6869 7320 6865 6164 6572 2069   * This header i
-0002bfe0: 7320 6d65 616e 7420 746f 2062 6520 7772  s meant to be wr
-0002bff0: 6974 7465 6e20 746f 2061 2060 2d2d 7061  itten to a `--pa
-0002c000: 636b 6167 6560 2066 696c 6520 616e 6420  ckage` file and 
-0002c010: 7368 6f75 6c64 206e 6f74 2062 6520 7061  should not be pa
-0002c020: 7373 6564 2074 6f20 6065 7865 6360 2e0a  ssed to `exec`..
-0002c030: 2d20 6022 626c 6f63 6b22 603a 0a20 2020  - `"block"`:.   
-0002c040: 202b 2070 6172 7365 723a 2066 696c 650a   + parser: file.
-0002c050: 2020 2020 2b20 6865 6164 6572 3a20 6e6f      + header: no
-0002c060: 6e65 0a20 2020 2020 2020 202a 204e 6f20  ne.        * No 
-0002c070: 6865 6164 6572 2069 7320 696e 636c 7564  header is includ
-0002c080: 6564 2c20 7468 7573 2074 6869 7320 6361  ed, thus this ca
-0002c090: 6e20 6f6e 6c79 2062 6520 7061 7373 6564  n only be passed
-0002c0a0: 2074 6f20 6065 7865 6360 2069 6620 636f   to `exec` if co
-0002c0b0: 6465 2077 6974 6820 6120 6865 6164 6572  de with a header
-0002c0c0: 2068 6173 2061 6c72 6561 6479 2062 6565   has already bee
-0002c0d0: 6e20 6578 6563 7574 6564 2061 7420 7468  n executed at th
-0002c0e0: 6520 676c 6f62 616c 206c 6576 656c 2e0a  e global level..
-0002c0f0: 2d20 6022 7369 6e67 6c65 2260 3a0a 2020  - `"single"`:.  
-0002c100: 2020 2b20 7061 7273 6572 3a20 7369 6e67    + parser: sing
-0002c110: 6c65 0a20 2020 2020 2020 202a 2043 616e  le.        * Can
-0002c120: 206f 6e6c 7920 7061 7273 6520 6f6e 6520   only parse one 
-0002c130: 6c69 6e65 206f 6620 436f 636f 6e75 7420  line of Coconut 
-0002c140: 636f 6465 2e0a 2020 2020 2b20 6865 6164  code..    + head
-0002c150: 6572 3a20 6e6f 6e65 0a2d 2060 2265 7661  er: none.- `"eva
-0002c160: 6c22 603a 0a20 2020 202b 2070 6172 7365  l"`:.    + parse
-0002c170: 723a 2065 7661 6c0a 2020 2020 2020 2020  r: eval.        
-0002c180: 2a20 4361 6e20 6f6e 6c79 2070 6172 7365  * Can only parse
-0002c190: 2061 2043 6f63 6f6e 7574 2065 7870 7265   a Coconut expre
-0002c1a0: 7373 696f 6e2c 206e 6f74 2061 2073 7461  ssion, not a sta
-0002c1b0: 7465 6d65 6e74 2e0a 2020 2020 2b20 6865  tement..    + he
-0002c1c0: 6164 6572 3a20 6e6f 6e65 0a2d 2060 226c  ader: none.- `"l
-0002c1d0: 656e 6965 6e74 2260 3a0a 2020 2020 2b20  enient"`:.    + 
-0002c1e0: 7061 7273 6572 3a20 6c65 6e69 656e 740a  parser: lenient.
-0002c1f0: 2020 2020 2020 2020 2a20 4361 6e20 7061          * Can pa
-0002c200: 7273 6520 616e 7920 436f 636f 6e75 7420  rse any Coconut 
-0002c210: 636f 6465 2c20 616c 6c6f 7773 206c 6561  code, allows lea
-0002c220: 6469 6e67 2077 6869 7465 7370 6163 652c  ding whitespace,
-0002c230: 2061 6e64 2068 6173 206e 6f20 7472 6169   and has no trai
-0002c240: 6c69 6e67 206e 6577 6c69 6e65 2e0a 2020  ling newline..  
-0002c250: 2020 2b20 6865 6164 6572 3a20 6e6f 6e65    + header: none
-0002c260: 0a2d 2060 2278 6f6e 7368 2260 3a0a 2020  .- `"xonsh"`:.  
-0002c270: 2020 2b20 7061 7273 6572 3a20 786f 6e73    + parser: xons
-0002c280: 680a 2020 2020 2020 2020 2a20 5061 7273  h.        * Pars
-0002c290: 6573 2043 6f63 6f6e 7574 205b 6078 6f6e  es Coconut [`xon
-0002c2a0: 7368 605d 2868 7474 7073 3a2f 2f78 6f6e  sh`](https://xon
-0002c2b0: 2e73 6829 2063 6f64 6520 666f 7220 7573  .sh) code for us
-0002c2c0: 6520 696e 205b 436f 636f 6e75 7427 7320  e in [Coconut's 
-0002c2d0: 6078 6f6e 7368 6020 7375 7070 6f72 745d  `xonsh` support]
-0002c2e0: 2823 786f 6e73 682d 7375 7070 6f72 7429  (#xonsh-support)
-0002c2f0: 2e0a 2020 2020 2b20 6865 6164 6572 3a20  ..    + header: 
-0002c300: 6e6f 6e65 0a0a 2323 2323 2320 4578 616d  none..##### Exam
-0002c310: 706c 650a 0a60 6060 636f 636f 6e75 745f  ple..```coconut_
-0002c320: 7079 7468 6f6e 0a66 726f 6d20 636f 636f  python.from coco
-0002c330: 6e75 742e 636f 6e76 656e 6965 6e63 6520  nut.convenience 
-0002c340: 696d 706f 7274 2070 6172 7365 0a65 7865  import parse.exe
-0002c350: 6328 7061 7273 6528 2929 0a77 6869 6c65  c(parse()).while
-0002c360: 2054 7275 653a 0a20 2020 2065 7865 6328   True:.    exec(
-0002c370: 7061 7273 6528 696e 7075 7428 292c 206d  parse(input(), m
-0002c380: 6f64 653d 2262 6c6f 636b 2229 290a 6060  ode="block")).``
-0002c390: 600a 0a23 2323 2320 6073 6574 7570 600a  `..#### `setup`.
-0002c3a0: 0a2a 2a63 6f63 6f6e 7574 2e63 6f6e 7665  .**coconut.conve
-0002c3b0: 6e69 656e 6365 2e73 6574 7570 2a2a 285f  nience.setup**(_
-0002c3c0: 7461 7267 6574 5f3d 604e 6f6e 6560 2c20  target_=`None`, 
-0002c3d0: 5f73 7472 6963 745f 3d60 4661 6c73 6560  _strict_=`False`
-0002c3e0: 2c20 5f6d 696e 6966 795f 3d60 4661 6c73  , _minify_=`Fals
-0002c3f0: 6560 2c20 5f6c 696e 655c 5f6e 756d 6265  e`, _line\_numbe
-0002c400: 7273 5f3d 6046 616c 7365 602c 205f 6b65  rs_=`False`, _ke
-0002c410: 6570 5c5f 6c69 6e65 735f 3d60 4661 6c73  ep\_lines_=`Fals
-0002c420: 6560 2c20 5f6e 6f5c 5f74 636f 5f3d 6046  e`, _no\_tco_=`F
-0002c430: 616c 7365 602c 205f 6e6f 5c5f 7772 6170  alse`, _no\_wrap
-0002c440: 5f3d 6046 616c 7365 602c 202a 2c20 5f73  _=`False`, *, _s
-0002c450: 7461 7465 5f3d 6046 616c 7365 6029 0a0a  tate_=`False`)..
-0002c460: 6073 6574 7570 6020 6361 6e20 6265 2075  `setup` can be u
-0002c470: 7365 6420 746f 2073 6574 2075 7020 7468  sed to set up th
-0002c480: 6520 6769 7665 6e20 7374 6174 6520 6f62  e given state ob
-0002c490: 6a65 6374 2077 6974 6820 7468 6520 6769  ject with the gi
-0002c4a0: 7665 6e20 636f 6d6d 616e 642d 6c69 6e65  ven command-line
-0002c4b0: 2066 6c61 6773 2e20 4966 205f 7374 6174   flags. If _stat
-0002c4c0: 655f 2069 7320 6046 616c 7365 602c 2074  e_ is `False`, t
-0002c4d0: 6865 2067 6c6f 6261 6c20 7374 6174 6520  he global state 
-0002c4e0: 6f62 6a65 6374 2069 7320 7573 6564 2e0a  object is used..
-0002c4f0: 0a54 6865 2070 6f73 7369 626c 6520 7661  .The possible va
-0002c500: 6c75 6573 2066 6f72 2065 6163 6820 666c  lues for each fl
-0002c510: 6167 2061 7267 756d 656e 7420 6172 653a  ag argument are:
-0002c520: 0a0a 2d20 5f74 6172 6765 745f 3a20 604e  ..- _target_: `N
-0002c530: 6f6e 6560 2028 6465 6661 756c 7429 2c20  one` (default), 
-0002c540: 6f72 2061 6e79 205b 616c 6c6f 7761 626c  or any [allowabl
-0002c550: 6520 7461 7267 6574 5d28 2361 6c6c 6f77  e target](#allow
-0002c560: 6162 6c65 2d74 6172 6765 7473 290a 2d20  able-targets).- 
-0002c570: 5f73 7472 6963 745f 3a20 6046 616c 7365  _strict_: `False
-0002c580: 6020 2864 6566 6175 6c74 2920 6f72 2060  ` (default) or `
-0002c590: 5472 7565 600a 2d20 5f6d 696e 6966 795f  True`.- _minify_
-0002c5a0: 3a20 6046 616c 7365 6020 2864 6566 6175  : `False` (defau
-0002c5b0: 6c74 2920 6f72 2060 5472 7565 600a 2d20  lt) or `True`.- 
-0002c5c0: 5f6c 696e 655c 5f6e 756d 6265 7273 5f3a  _line\_numbers_:
-0002c5d0: 2060 4661 6c73 6560 2028 6465 6661 756c   `False` (defaul
-0002c5e0: 7429 206f 7220 6054 7275 6560 0a2d 205f  t) or `True`.- _
-0002c5f0: 6b65 6570 5c5f 6c69 6e65 735f 3a20 6046  keep\_lines_: `F
+000270c0: 6563 7473 2c20 7573 6573 205b 606e 702e  ects, uses [`np.
+000270d0: 6e64 6974 6572 605d 2868 7474 7073 3a2f  nditer`](https:/
+000270e0: 2f6e 756d 7079 2e6f 7267 2f64 6f63 2f73  /numpy.org/doc/s
+000270f0: 7461 626c 652f 7265 6665 7265 6e63 652f  table/reference/
+00027100: 6765 6e65 7261 7465 642f 6e75 6d70 792e  generated/numpy.
+00027110: 6e64 6974 6572 2e68 746d 6c29 2075 6e64  nditer.html) und
+00027120: 6572 2074 6865 2068 6f6f 642e 2041 6c73  er the hood. Als
+00027130: 6f20 7375 7070 6f72 7473 2060 6c65 6e60  o supports `len`
+00027140: 2066 6f72 205b 606e 756d 7079 605d 2823   for [`numpy`](#
+00027150: 6e75 6d70 792d 696e 7465 6772 6174 696f  numpy-integratio
+00027160: 6e29 2061 7272 6179 732e 0a0a 2323 2323  n) arrays...####
+00027170: 2320 4578 616d 706c 650a 0a2a 2a43 6f63  # Example..**Coc
+00027180: 6f6e 7574 3a2a 2a0a 6060 6063 6f63 6f6e  onut:**.```cocon
+00027190: 7574 5f70 7963 6f6e 0a3e 3e3e 205b 312c  ut_pycon.>>> [1,
+000271a0: 2032 3b3b 2033 2c20 345d 207c 3e20 6d75   2;; 3, 4] |> mu
+000271b0: 6c74 695f 656e 756d 6572 6174 6520 7c3e  lti_enumerate |>
+000271c0: 206c 6973 740a 5b28 2830 2c20 3029 2c20   list.[((0, 0), 
+000271d0: 3129 2c20 2828 302c 2031 292c 2032 292c  1), ((0, 1), 2),
+000271e0: 2028 2831 2c20 3029 2c20 3329 2c20 2828   ((1, 0), 3), ((
+000271f0: 312c 2031 292c 2034 295d 0a60 6060 0a0a  1, 1), 4)].```..
+00027200: 2a2a 5079 7468 6f6e 3a2a 2a0a 6060 6063  **Python:**.```c
+00027210: 6f63 6f6e 7574 5f70 7974 686f 6e0a 6172  oconut_python.ar
+00027220: 7261 7920 3d20 5b5b 312c 2032 5d2c 205b  ray = [[1, 2], [
+00027230: 332c 2034 5d5d 0a65 6e75 6d65 7261 7465  3, 4]].enumerate
+00027240: 645f 6172 7261 7920 3d20 5b5d 0a66 6f72  d_array = [].for
+00027250: 2069 2069 6e20 7261 6e67 6528 6c65 6e28   i in range(len(
+00027260: 6172 7261 7929 293a 0a20 2020 2066 6f72  array)):.    for
+00027270: 206a 2069 6e20 7261 6e67 6528 6c65 6e28   j in range(len(
+00027280: 6172 7261 795b 695d 2929 3a0a 2020 2020  array[i])):.    
+00027290: 2020 2020 656e 756d 6572 6174 6564 5f61      enumerated_a
+000272a0: 7272 6179 2e61 7070 656e 6428 2828 692c  rray.append(((i,
+000272b0: 206a 292c 2061 7272 6179 5b69 5d5b 6a5d   j), array[i][j]
+000272c0: 2929 0a60 6060 0a0a 2323 2323 2060 6772  )).```..#### `gr
+000272d0: 6f75 7073 6f66 600a 0a2a 2a67 726f 7570  oupsof`..**group
+000272e0: 736f 662a 2a28 5f6e 5f2c 205f 6974 6572  sof**(_n_, _iter
+000272f0: 6162 6c65 5f2c 205f 6669 6c6c 7661 6c75  able_, _fillvalu
+00027300: 655f 3d60 2e2e 2e60 290a 0a43 6f63 6f6e  e_=`...`)..Cocon
+00027310: 7574 2070 726f 7669 6465 7320 7468 6520  ut provides the 
+00027320: 6067 726f 7570 736f 6660 2062 7569 6c74  `groupsof` built
+00027330: 2d69 6e20 746f 2073 706c 6974 2061 6e20  -in to split an 
+00027340: 6974 6572 6162 6c65 2069 6e74 6f20 6772  iterable into gr
+00027350: 6f75 7073 206f 6620 6120 7370 6563 6966  oups of a specif
+00027360: 6963 206c 656e 6774 682e 2053 7065 6369  ic length. Speci
+00027370: 6669 6361 6c6c 792c 2060 6772 6f75 7073  fically, `groups
+00027380: 6f66 286e 2c20 6974 6572 6162 6c65 2960  of(n, iterable)`
+00027390: 2077 696c 6c20 7370 6c69 7420 6069 7465   will split `ite
+000273a0: 7261 626c 6560 2069 6e74 6f20 7475 706c  rable` into tupl
+000273b0: 6573 206f 6620 6c65 6e67 7468 2060 6e60  es of length `n`
+000273c0: 2c20 7769 7468 206f 6e6c 7920 7468 6520  , with only the 
+000273d0: 6c61 7374 2074 7570 6c65 2070 6f74 656e  last tuple poten
+000273e0: 7469 616c 6c79 206f 6620 7369 7a65 2060  tially of size `
+000273f0: 3c20 6e60 2069 6620 7468 6520 6c65 6e67  < n` if the leng
+00027400: 7468 206f 6620 6069 7465 7261 626c 6560  th of `iterable`
+00027410: 2069 7320 6e6f 7420 6469 7669 7369 626c   is not divisibl
+00027420: 6520 6279 2060 6e60 2e20 4966 2074 6861  e by `n`. If tha
+00027430: 7420 6973 206e 6f74 2074 6865 2064 6573  t is not the des
+00027440: 6972 6564 2062 6568 6176 696f 722c 205f  ired behavior, _
+00027450: 6669 6c6c 7661 6c75 655f 2063 616e 2062  fillvalue_ can b
+00027460: 6520 7061 7373 6564 2061 6e64 2077 696c  e passed and wil
+00027470: 6c20 6265 2075 7365 6420 746f 2070 6164  l be used to pad
+00027480: 2074 6865 2065 6e64 206f 6620 7468 6520   the end of the 
+00027490: 6c61 7374 2074 7570 6c65 2074 6f20 6c65  last tuple to le
+000274a0: 6e67 7468 2060 6e60 2e0a 0a41 6464 6974  ngth `n`...Addit
+000274b0: 696f 6e61 6c6c 792c 2060 6772 6f75 7073  ionally, `groups
+000274c0: 6f66 6020 7375 7070 6f72 7473 2060 6c65  of` supports `le
+000274d0: 6e60 2077 6865 6e20 6069 7465 7261 626c  n` when `iterabl
+000274e0: 6560 2073 7570 706f 7274 7320 606c 656e  e` supports `len
+000274f0: 602e 0a0a 2323 2323 2320 4578 616d 706c  `...##### Exampl
+00027500: 650a 0a2a 2a43 6f63 6f6e 7574 3a2a 2a0a  e..**Coconut:**.
+00027510: 6060 6063 6f63 6f6e 7574 0a70 6169 7273  ```coconut.pairs
+00027520: 203d 2072 616e 6765 2831 2c20 3131 2920   = range(1, 11) 
+00027530: 7c3e 2067 726f 7570 736f 6624 2832 290a  |> groupsof$(2).
+00027540: 6060 600a 0a2a 2a50 7974 686f 6e3a 2a2a  ```..**Python:**
+00027550: 0a60 6060 636f 636f 6e75 745f 7079 7468  .```coconut_pyth
+00027560: 6f6e 0a70 6169 7273 203d 205b 5d0a 6772  on.pairs = [].gr
+00027570: 6f75 7020 3d20 5b5d 0a66 6f72 2069 7465  oup = [].for ite
+00027580: 6d20 696e 2072 616e 6765 2831 2c20 3131  m in range(1, 11
+00027590: 293a 0a20 2020 2067 726f 7570 2e61 7070  ):.    group.app
+000275a0: 656e 6428 6974 656d 290a 2020 2020 6966  end(item).    if
+000275b0: 206c 656e 2867 726f 7570 2920 3d3d 2032   len(group) == 2
+000275c0: 3a0a 2020 2020 2020 2020 7061 6972 732e  :.        pairs.
+000275d0: 6170 7065 6e64 2874 7570 6c65 2867 726f  append(tuple(gro
+000275e0: 7570 2929 0a20 2020 2020 2020 2067 726f  up)).        gro
+000275f0: 7570 203d 205b 5d0a 6966 2067 726f 7570  up = [].if group
+00027600: 3a0a 2020 2020 7061 6972 732e 6170 7065  :.    pairs.appe
+00027610: 6e64 2874 7570 6c65 2867 726f 7570 2929  nd(tuple(group))
+00027620: 0a60 6060 0a0a 2323 2323 2060 7769 6e64  .```..#### `wind
+00027630: 6f77 736f 6660 0a0a 2a2a 7769 6e64 6f77  owsof`..**window
+00027640: 736f 662a 2a28 5f73 697a 655f 2c20 5f69  sof**(_size_, _i
+00027650: 7465 7261 626c 655f 2c20 5f66 696c 6c76  terable_, _fillv
+00027660: 616c 7565 5f3d 602e 2e2e 602c 205f 7374  alue_=`...`, _st
+00027670: 6570 5f3d 6031 6029 0a0a 6077 696e 646f  ep_=`1`)..`windo
+00027680: 7773 6f66 6020 7072 6f64 7563 6573 2061  wsof` produces a
+00027690: 6e20 6974 6572 6162 6c65 2074 6861 7420  n iterable that 
+000276a0: 6566 6665 6374 6976 656c 7920 6d69 6d69  effectively mimi
+000276b0: 6373 2061 2073 6c69 6469 6e67 2077 696e  cs a sliding win
+000276c0: 646f 7720 6f76 6572 205f 6974 6572 6162  dow over _iterab
+000276d0: 6c65 5f20 6f66 2073 697a 6520 5f73 697a  le_ of size _siz
+000276e0: 655f 2e20 5f73 7465 705f 2064 6574 6572  e_. _step_ deter
+000276f0: 6d69 6e65 7320 7468 6520 7370 6163 696e  mines the spacin
+00027700: 6720 6265 7477 6565 6e20 7769 6e64 6f77  g between window
+00027710: 736f 662e 0a0a 4966 205f 7369 7a65 5f20  sof...If _size_ 
+00027720: 6973 206c 6172 6765 7220 7468 616e 205f  is larger than _
+00027730: 6974 6572 6162 6c65 5f2c 2060 7769 6e64  iterable_, `wind
+00027740: 6f77 736f 6660 2077 696c 6c20 7072 6f64  owsof` will prod
+00027750: 7563 6520 616e 2065 6d70 7479 2069 7465  uce an empty ite
+00027760: 7261 626c 652e 2049 6620 7468 6174 2069  rable. If that i
+00027770: 7320 6e6f 7420 7468 6520 6465 7369 7265  s not the desire
+00027780: 6420 6265 6861 7669 6f72 2c20 5f66 696c  d behavior, _fil
+00027790: 6c76 616c 7565 5f20 6361 6e20 6265 2070  lvalue_ can be p
+000277a0: 6173 7365 6420 616e 6420 7769 6c6c 2062  assed and will b
+000277b0: 6520 7573 6564 2069 6e20 706c 6163 6520  e used in place 
+000277c0: 6f66 206d 6973 7369 6e67 2076 616c 7565  of missing value
+000277d0: 732e 2041 6c73 6f2c 2069 6620 5f66 696c  s. Also, if _fil
+000277e0: 6c76 616c 7565 5f20 6973 2070 6173 7365  lvalue_ is passe
+000277f0: 6420 616e 6420 7468 6520 6c65 6e67 7468  d and the length
+00027800: 206f 6620 7468 6520 5f69 7465 7261 626c   of the _iterabl
+00027810: 655f 2069 7320 6e6f 7420 6469 7669 7369  e_ is not divisi
+00027820: 626c 6520 6279 205f 7374 6570 5f2c 205f  ble by _step_, _
+00027830: 6669 6c6c 7661 6c75 655f 2077 696c 6c20  fillvalue_ will 
+00027840: 6265 2075 7365 6420 696e 2074 6861 7420  be used in that 
+00027850: 6361 7365 2074 6f20 7061 6420 7468 6520  case to pad the 
+00027860: 6c61 7374 2077 696e 646f 7720 6173 2077  last window as w
+00027870: 656c 6c2e 204e 6f74 6520 7468 6174 205f  ell. Note that _
+00027880: 6669 6c6c 7661 6c75 655f 2077 696c 6c20  fillvalue_ will 
+00027890: 6f6e 6c79 2065 7665 7220 6170 7065 6172  only ever appear
+000278a0: 2069 6e20 7468 6520 6c61 7374 2077 696e   in the last win
+000278b0: 646f 772e 0a0a 4164 6469 7469 6f6e 616c  dow...Additional
+000278c0: 6c79 2c20 6077 696e 646f 7773 6f66 6020  ly, `windowsof` 
+000278d0: 7375 7070 6f72 7473 2060 6c65 6e60 2077  supports `len` w
+000278e0: 6865 6e20 6069 7465 7261 626c 6560 2073  hen `iterable` s
+000278f0: 7570 706f 7274 7320 606c 656e 602e 0a0a  upports `len`...
+00027900: 2323 2323 2320 4578 616d 706c 650a 0a2a  ##### Example..*
+00027910: 2a43 6f63 6f6e 7574 3a2a 2a0a 6060 6063  *Coconut:**.```c
+00027920: 6f63 6f6e 7574 0a61 7373 6572 7420 2231  oconut.assert "1
+00027930: 3233 3435 2220 7c3e 2077 696e 646f 7773  2345" |> windows
+00027940: 6f66 2428 3329 207c 3e20 6c69 7374 203d  of$(3) |> list =
+00027950: 3d20 5b28 2231 222c 2022 3222 2c20 2233  = [("1", "2", "3
+00027960: 2229 2c20 2822 3222 2c20 2233 222c 2022  "), ("2", "3", "
+00027970: 3422 292c 2028 2233 222c 2022 3422 2c20  4"), ("3", "4", 
+00027980: 2235 2229 5d0a 6060 600a 0a2a 2a50 7974  "5")].```..**Pyt
+00027990: 686f 6e3a 2a2a 0a5f 4361 6e27 7420 6265  hon:**._Can't be
+000279a0: 2064 6f6e 6520 7769 7468 6f75 7420 7468   done without th
+000279b0: 6520 6465 6669 6e69 7469 6f6e 206f 6620  e definition of 
+000279c0: 6077 696e 646f 7773 6f66 603b 2073 6565  `windowsof`; see
+000279d0: 2074 6865 2063 6f6d 7069 6c65 6420 6865   the compiled he
+000279e0: 6164 6572 2066 6f72 2074 6865 2066 756c  ader for the ful
+000279f0: 6c20 6465 6669 6e69 7469 6f6e 2e5f 0a0a  l definition._..
+00027a00: 2323 2323 2060 636f 6c6c 6563 7462 7960  #### `collectby`
+00027a10: 0a0a 2a2a 636f 6c6c 6563 7462 792a 2a28  ..**collectby**(
+00027a20: 5f6b 6579 5c5f 6675 6e63 5f2c 205f 6974  _key\_func_, _it
+00027a30: 6572 6162 6c65 5f2c 205f 7661 6c75 655c  erable_, _value\
+00027a40: 5f66 756e 635f 3d60 4e6f 6e65 602c 205f  _func_=`None`, _
+00027a50: 7265 6475 6365 5c5f 6675 6e63 5f3d 604e  reduce\_func_=`N
+00027a60: 6f6e 6560 290a 0a60 636f 6c6c 6563 7462  one`)..`collectb
+00027a70: 7928 6b65 795f 6675 6e63 2c20 6974 6572  y(key_func, iter
+00027a80: 6162 6c65 2960 2063 6f6c 6c65 6374 7320  able)` collects 
+00027a90: 7468 6520 6974 656d 7320 696e 2060 6974  the items in `it
+00027aa0: 6572 6162 6c65 6020 696e 746f 2061 2064  erable` into a d
+00027ab0: 6963 7469 6f6e 6172 7920 6f66 206c 6973  ictionary of lis
+00027ac0: 7473 206b 6579 6564 2062 7920 606b 6579  ts keyed by `key
+00027ad0: 5f66 756e 6328 6974 656d 2960 2e0a 0a49  _func(item)`...I
+00027ae0: 6620 6076 616c 7565 5f66 756e 6360 2069  f `value_func` i
+00027af0: 7320 7061 7373 6564 2c20 6063 6f6c 6c65  s passed, `colle
+00027b00: 6374 6279 286b 6579 5f66 756e 632c 2069  ctby(key_func, i
+00027b10: 7465 7261 626c 652c 2076 616c 7565 5f66  terable, value_f
+00027b20: 756e 633d 7661 6c75 655f 6675 6e63 2960  unc=value_func)`
+00027b30: 2069 6e73 7465 6164 2063 6f6c 6c65 6374   instead collect
+00027b40: 7320 7661 6c75 655f 6675 6e63 2869 7465  s value_func(ite
+00027b50: 6d29 2069 6e74 6f20 6561 6368 206c 6973  m) into each lis
+00027b60: 7420 696e 7374 6561 6420 6f66 2069 7465  t instead of ite
+00027b70: 6d2e 0a0a 4966 2060 7265 6475 6365 5f66  m...If `reduce_f
+00027b80: 756e 6360 2069 7320 7061 7373 6564 2c20  unc` is passed, 
+00027b90: 6063 6f6c 6c65 6374 6279 286b 6579 5f66  `collectby(key_f
+00027ba0: 756e 632c 2069 7465 7261 626c 652c 2072  unc, iterable, r
+00027bb0: 6564 7563 655f 6675 6e63 3d72 6564 7563  educe_func=reduc
+00027bc0: 655f 6675 6e63 2960 2c20 696e 7374 6561  e_func)`, instea
+00027bd0: 6420 6f66 2063 6f6c 6c65 6374 696e 6720  d of collecting 
+00027be0: 7468 6520 6974 656d 7320 696e 746f 206c  the items into l
+00027bf0: 6973 7473 2c20 7265 6475 6365 7320 6f76  ists, reduces ov
+00027c00: 6572 2074 6865 2069 7465 6d73 206f 6620  er the items of 
+00027c10: 6561 6368 206b 6579 2077 6974 6820 7265  each key with re
+00027c20: 6475 6365 5f66 756e 632c 2065 6666 6563  duce_func, effec
+00027c30: 7469 7665 6c79 2069 6d70 6c65 6d65 6e74  tively implement
+00027c40: 696e 6720 6120 4d61 7052 6564 7563 6520  ing a MapReduce 
+00027c50: 6f70 6572 6174 696f 6e2e 0a0a 6063 6f6c  operation...`col
+00027c60: 6c65 6374 6279 6020 6973 2065 6666 6563  lectby` is effec
+00027c70: 7469 7665 6c79 2065 7175 6976 616c 656e  tively equivalen
+00027c80: 7420 746f 3a0a 6060 6063 6f63 6f6e 7574  t to:.```coconut
+00027c90: 5f70 7974 686f 6e0a 6672 6f6d 2063 6f6c  _python.from col
+00027ca0: 6c65 6374 696f 6e73 2069 6d70 6f72 7420  lections import 
+00027cb0: 6465 6661 756c 7464 6963 740a 0a64 6566  defaultdict..def
+00027cc0: 2063 6f6c 6c65 6374 6279 286b 6579 5f66   collectby(key_f
+00027cd0: 756e 632c 2069 7465 7261 626c 652c 2076  unc, iterable, v
+00027ce0: 616c 7565 5f66 756e 633d 6964 656e 742c  alue_func=ident,
+00027cf0: 2072 6564 7563 655f 6675 6e63 3d4e 6f6e   reduce_func=Non
+00027d00: 6529 3a0a 2020 2020 636f 6c6c 6563 7469  e):.    collecti
+00027d10: 6f6e 203d 2064 6566 6175 6c74 6469 6374  on = defaultdict
+00027d20: 286c 6973 7429 2069 6620 7265 6475 6365  (list) if reduce
+00027d30: 5f66 756e 6320 6973 204e 6f6e 6520 656c  _func is None el
+00027d40: 7365 207b 7d0a 2020 2020 666f 7220 6974  se {}.    for it
+00027d50: 656d 2069 6e20 6974 6572 6162 6c65 3a0a  em in iterable:.
+00027d60: 2020 2020 2020 2020 6b65 7920 3d20 6b65          key = ke
+00027d70: 795f 6675 6e63 2869 7465 6d29 0a20 2020  y_func(item).   
+00027d80: 2020 2020 2076 616c 7565 203d 2076 616c       value = val
+00027d90: 7565 5f66 756e 6328 6974 656d 290a 2020  ue_func(item).  
+00027da0: 2020 2020 2020 6966 2072 6564 7563 655f        if reduce_
+00027db0: 6675 6e63 2069 7320 4e6f 6e65 3a0a 2020  func is None:.  
+00027dc0: 2020 2020 2020 2020 2020 636f 6c6c 6563            collec
+00027dd0: 7469 6f6e 5b6b 6579 5d2e 6170 7065 6e64  tion[key].append
+00027de0: 2876 616c 7565 290a 2020 2020 2020 2020  (value).        
+00027df0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00027e00: 2020 6f6c 645f 7661 6c75 6520 3d20 636f    old_value = co
+00027e10: 6c6c 6563 7469 6f6e 2e67 6574 286b 6579  llection.get(key
+00027e20: 2c20 7365 6e74 696e 656c 290a 2020 2020  , sentinel).    
+00027e30: 2020 2020 2020 2020 6966 206f 6c64 5f76          if old_v
+00027e40: 616c 7565 2069 7320 6e6f 7420 7365 6e74  alue is not sent
+00027e50: 696e 656c 3a0a 2020 2020 2020 2020 2020  inel:.          
+00027e60: 2020 2020 2020 7661 6c75 6520 3d20 7265        value = re
+00027e70: 6475 6365 5f66 756e 6328 6f6c 645f 7661  duce_func(old_va
+00027e80: 6c75 652c 2076 616c 7565 290a 2020 2020  lue, value).    
+00027e90: 2020 2020 2020 2020 636f 6c6c 6563 7469          collecti
+00027ea0: 6f6e 5b6b 6579 5d20 3d20 7661 6c75 650a  on[key] = value.
+00027eb0: 2020 2020 7265 7475 726e 2063 6f6c 6c65      return colle
+00027ec0: 6374 696f 6e0a 6060 600a 0a60 636f 6c6c  ction.```..`coll
+00027ed0: 6563 7462 7960 2069 7320 7369 6d69 6c61  ectby` is simila
+00027ee0: 7220 746f 205b 6069 7465 7274 6f6f 6c73  r to [`itertools
+00027ef0: 2e67 726f 7570 6279 605d 2868 7474 7073  .groupby`](https
+00027f00: 3a2f 2f64 6f63 732e 7079 7468 6f6e 2e6f  ://docs.python.o
+00027f10: 7267 2f33 2f6c 6962 7261 7279 2f69 7465  rg/3/library/ite
+00027f20: 7274 6f6f 6c73 2e68 746d 6c23 6974 6572  rtools.html#iter
+00027f30: 746f 6f6c 732e 6772 6f75 7062 7929 2065  tools.groupby) e
+00027f40: 7863 6570 7420 7468 6174 2060 636f 6c6c  xcept that `coll
+00027f50: 6563 7462 7960 2061 6767 7265 6761 7465  ectby` aggregate
+00027f60: 7320 636f 6d6d 6f6e 2065 6c65 6d65 6e74  s common element
+00027f70: 7320 7265 6761 7264 6c65 7373 206f 6620  s regardless of 
+00027f80: 7468 6569 7220 6f72 6465 7220 696e 2074  their order in t
+00027f90: 6865 2069 6e70 7574 2069 7465 7261 626c  he input iterabl
+00027fa0: 652c 2077 6865 7265 6173 2060 6772 6f75  e, whereas `grou
+00027fb0: 7062 7960 206f 6e6c 7920 6167 6772 6567  pby` only aggreg
+00027fc0: 6174 6573 2063 6f6d 6d6f 6e20 656c 656d  ates common elem
+00027fd0: 656e 7473 2074 6861 7420 6172 6520 6164  ents that are ad
+00027fe0: 6a61 6365 6e74 2069 6e20 7468 6520 696e  jacent in the in
+00027ff0: 7075 7420 6974 6572 6162 6c65 2e0a 0a23  put iterable...#
+00028000: 2323 2323 2045 7861 6d70 6c65 0a0a 2a2a  #### Example..**
+00028010: 436f 636f 6e75 743a 2a2a 0a60 6060 636f  Coconut:**.```co
+00028020: 636f 6e75 740a 7573 6572 5f62 616c 616e  conut.user_balan
+00028030: 6365 7320 3d20 280a 2020 2020 6261 6c61  ces = (.    bala
+00028040: 6e63 655f 6461 7461 0a20 2020 207c 3e20  nce_data.    |> 
+00028050: 636f 6c6c 6563 7462 7924 282e 7573 6572  collectby$(.user
+00028060: 2c20 7661 6c75 655f 6675 6e63 3d2e 6261  , value_func=.ba
+00028070: 6c61 6e63 652c 2072 6564 7563 655f 6675  lance, reduce_fu
+00028080: 6e63 3d28 2b29 290a 290a 6060 600a 0a2a  nc=(+)).).```..*
+00028090: 2a50 7974 686f 6e3a 2a2a 0a60 6060 636f  *Python:**.```co
+000280a0: 636f 6e75 745f 7079 7468 6f6e 0a66 726f  conut_python.fro
+000280b0: 6d20 636f 6c6c 6563 7469 6f6e 7320 696d  m collections im
+000280c0: 706f 7274 2064 6566 6175 6c74 6469 6374  port defaultdict
+000280d0: 0a0a 7573 6572 5f62 616c 616e 6365 7320  ..user_balances 
+000280e0: 3d20 6465 6661 756c 7464 6963 7428 696e  = defaultdict(in
+000280f0: 7429 0a66 6f72 2069 7465 6d20 696e 2062  t).for item in b
+00028100: 616c 616e 6365 5f64 6174 613a 0a20 2020  alance_data:.   
+00028110: 2075 7365 725f 6261 6c61 6e63 6573 5b69   user_balances[i
+00028120: 7465 6d2e 7573 6572 5d20 2b3d 2069 7465  tem.user] += ite
+00028130: 6d2e 6261 6c61 6e63 650a 6060 600a 0a23  m.balance.```..#
+00028140: 2323 2320 6061 6c6c 5f65 7175 616c 600a  ### `all_equal`.
+00028150: 0a2a 2a61 6c6c 5c5f 6571 7561 6c2a 2a28  .**all\_equal**(
+00028160: 5f69 7465 7261 626c 655f 290a 0a43 6f63  _iterable_)..Coc
+00028170: 6f6e 7574 2773 2060 616c 6c5f 6571 7561  onut's `all_equa
+00028180: 6c60 2062 7569 6c74 2d69 6e20 7461 6b65  l` built-in take
+00028190: 7320 696e 2061 6e20 6974 6572 6162 6c65  s in an iterable
+000281a0: 2061 6e64 2064 6574 6572 6d69 6e65 7320   and determines 
+000281b0: 7768 6574 6865 7220 616c 6c20 6f66 2069  whether all of i
+000281c0: 7473 2065 6c65 6d65 6e74 7320 6172 6520  ts elements are 
+000281d0: 6571 7561 6c20 746f 2065 6163 6820 6f74  equal to each ot
+000281e0: 6865 722e 2060 616c 6c5f 6571 7561 6c60  her. `all_equal`
+000281f0: 2061 7373 756d 6573 2074 7261 6e73 6974   assumes transit
+00028200: 6976 6974 7920 6f66 2065 7175 616c 6974  ivity of equalit
+00028210: 7920 616e 6420 7468 6174 2060 213d 6020  y and that `!=` 
+00028220: 6973 2074 6865 206e 6567 6174 696f 6e20  is the negation 
+00028230: 6f66 2060 3d3d 602e 2053 7065 6369 616c  of `==`. Special
+00028240: 2073 7570 706f 7274 2069 7320 7072 6f76   support is prov
+00028250: 6964 6564 2066 6f72 205b 606e 756d 7079  ided for [`numpy
+00028260: 605d 2823 6e75 6d70 792d 696e 7465 6772  `](#numpy-integr
+00028270: 6174 696f 6e29 206f 626a 6563 7473 2e0a  ation) objects..
+00028280: 0a23 2323 2323 2045 7861 6d70 6c65 0a0a  .##### Example..
+00028290: 2a2a 436f 636f 6e75 743a 2a2a 0a60 6060  **Coconut:**.```
+000282a0: 636f 636f 6e75 740a 616c 6c5f 6571 7561  coconut.all_equa
+000282b0: 6c28 5b31 2c20 312c 2031 5d29 0a61 6c6c  l([1, 1, 1]).all
+000282c0: 5f65 7175 616c 285b 312c 2031 2c20 325d  _equal([1, 1, 2]
+000282d0: 290a 6060 600a 0a2a 2a50 7974 686f 6e3a  ).```..**Python:
+000282e0: 2a2a 0a60 6060 636f 636f 6e75 745f 7079  **.```coconut_py
+000282f0: 7468 6f6e 0a73 656e 7469 6e65 6c20 3d20  thon.sentinel = 
+00028300: 6f62 6a65 6374 2829 0a64 6566 2061 6c6c  object().def all
+00028310: 5f65 7175 616c 2869 7465 7261 626c 6529  _equal(iterable)
+00028320: 3a0a 2020 2020 6669 7273 745f 6974 656d  :.    first_item
+00028330: 203d 2073 656e 7469 6e65 6c0a 2020 2020   = sentinel.    
+00028340: 666f 7220 6974 656d 2069 6e20 6974 6572  for item in iter
+00028350: 6162 6c65 3a0a 2020 2020 2020 2020 6966  able:.        if
+00028360: 2066 6972 7374 5f69 7465 6d20 6973 2073   first_item is s
+00028370: 656e 7469 6e65 6c3a 0a20 2020 2020 2020  entinel:.       
+00028380: 2020 2020 2066 6972 7374 5f69 7465 6d20       first_item 
+00028390: 3d20 6974 656d 0a20 2020 2020 2020 2065  = item.        e
+000283a0: 6c69 6620 6669 7273 745f 6974 656d 2021  lif first_item !
+000283b0: 3d20 6974 656d 3a0a 2020 2020 2020 2020  = item:.        
+000283c0: 2020 2020 7265 7475 726e 2046 616c 7365      return False
+000283d0: 0a20 2020 2072 6574 7572 6e20 5472 7565  .    return True
+000283e0: 0a61 6c6c 5f65 7175 616c 285b 312c 2031  .all_equal([1, 1
+000283f0: 2c20 315d 290a 616c 6c5f 6571 7561 6c28  , 1]).all_equal(
+00028400: 5b31 2c20 312c 2032 5d29 0a60 6060 0a0a  [1, 1, 2]).```..
+00028410: 2323 2323 2060 7061 7261 6c6c 656c 5f6d  #### `parallel_m
+00028420: 6170 600a 0a2a 2a70 6172 616c 6c65 6c5c  ap`..**parallel\
+00028430: 5f6d 6170 2a2a 285f 6675 6e63 7469 6f6e  _map**(_function
+00028440: 5f2c 202a 5f69 7465 7261 626c 6573 5f2c  _, *_iterables_,
+00028450: 202a 2c20 5f63 6875 6e6b 7369 7a65 5f3d   *, _chunksize_=
+00028460: 6031 602c 205f 7374 7269 6374 5f3d 6046  `1`, _strict_=`F
+00028470: 616c 7365 6029 0a0a 436f 636f 6e75 7420  alse`)..Coconut 
+00028480: 7072 6f76 6964 6573 2061 2070 6172 616c  provides a paral
+00028490: 6c65 6c20 7665 7273 696f 6e20 6f66 2060  lel version of `
+000284a0: 6d61 7060 2075 6e64 6572 2074 6865 206e  map` under the n
+000284b0: 616d 6520 6070 6172 616c 6c65 6c5f 6d61  ame `parallel_ma
+000284c0: 7060 2e20 6070 6172 616c 6c65 6c5f 6d61  p`. `parallel_ma
+000284d0: 7060 206d 616b 6573 2075 7365 206f 6620  p` makes use of 
+000284e0: 6d75 6c74 6970 6c65 2070 726f 6365 7373  multiple process
+000284f0: 6573 2c20 616e 6420 6973 2074 6865 7265  es, and is there
+00028500: 666f 7265 206d 7563 6820 6661 7374 6572  fore much faster
+00028510: 2074 6861 6e20 606d 6170 6020 666f 7220   than `map` for 
+00028520: 4350 552d 626f 756e 6420 7461 736b 732e  CPU-bound tasks.
+00028530: 2060 7061 7261 6c6c 656c 5f6d 6170 6020   `parallel_map` 
+00028540: 6e65 7665 7220 6c6f 6164 7320 7468 6520  never loads the 
+00028550: 656e 7469 7265 2069 6e70 7574 2069 7465  entire input ite
+00028560: 7261 746f 7220 696e 746f 206d 656d 6f72  rator into memor
+00028570: 792c 2074 686f 7567 6820 6974 2064 6f65  y, though it doe
+00028580: 7320 636f 6e73 756d 6520 7468 6520 656e  s consume the en
+00028590: 7469 7265 2069 6e70 7574 2069 7465 7261  tire input itera
+000285a0: 746f 7220 6173 2073 6f6f 6e20 6173 2061  tor as soon as a
+000285b0: 2073 696e 676c 6520 6f75 7470 7574 2069   single output i
+000285c0: 7320 7265 7175 6573 7465 642e 2049 6620  s requested. If 
+000285d0: 616e 7920 6578 6365 7074 696f 6e73 2061  any exceptions a
+000285e0: 7265 2072 6169 7365 6420 696e 7369 6465  re raised inside
+000285f0: 206f 6620 6070 6172 616c 6c65 6c5f 6d61   of `parallel_ma
+00028600: 7060 2c20 6120 7472 6163 6562 6163 6b20  p`, a traceback 
+00028610: 7769 6c6c 2062 6520 7072 696e 7465 6420  will be printed 
+00028620: 6173 2073 6f6f 6e20 6173 2074 6865 7920  as soon as they 
+00028630: 6172 6520 656e 636f 756e 7465 7265 642e  are encountered.
+00028640: 0a0a 4265 6361 7573 6520 6070 6172 616c  ..Because `paral
+00028650: 6c65 6c5f 6d61 7060 2075 7365 7320 6d75  lel_map` uses mu
+00028660: 6c74 6970 6c65 2070 726f 6365 7373 6573  ltiple processes
+00028670: 2066 6f72 2069 7473 2065 7865 6375 7469   for its executi
+00028680: 6f6e 2c20 6974 2069 7320 6e65 6365 7373  on, it is necess
+00028690: 6172 7920 7468 6174 2061 6c6c 206f 6620  ary that all of 
+000286a0: 6974 7320 6172 6775 6d65 6e74 7320 6265  its arguments be
+000286b0: 2070 6963 6b6c 6561 626c 652e 204f 6e6c   pickleable. Onl
+000286c0: 7920 6f62 6a65 6374 7320 6465 6669 6e65  y objects define
+000286d0: 6420 6174 2074 6865 206d 6f64 756c 6520  d at the module 
+000286e0: 6c65 7665 6c2c 2061 6e64 206e 6f74 206c  level, and not l
+000286f0: 616d 6264 6173 2c20 6f62 6a65 6374 7320  ambdas, objects 
+00028700: 6465 6669 6e65 6420 696e 7369 6465 206f  defined inside o
+00028710: 6620 6120 6675 6e63 7469 6f6e 2c20 6f72  f a function, or
+00028720: 206f 626a 6563 7473 2064 6566 696e 6564   objects defined
+00028730: 2069 6e73 6964 6520 6f66 2074 6865 2069   inside of the i
+00028740: 6e74 6572 7072 6574 6572 2c20 6172 6520  nterpreter, are 
+00028750: 7069 636b 6c65 6162 6c65 2e20 4675 7274  pickleable. Furt
+00028760: 6865 726d 6f72 652c 206f 6e20 5769 6e64  hermore, on Wind
+00028770: 6f77 732c 2069 7420 6973 206e 6563 6573  ows, it is neces
+00028780: 7361 7279 2074 6861 7420 616c 6c20 6361  sary that all ca
+00028790: 6c6c 7320 746f 2060 7061 7261 6c6c 656c  lls to `parallel
+000287a0: 5f6d 6170 6020 6f63 6375 7220 696e 7369  _map` occur insi
+000287b0: 6465 206f 6620 616e 2060 6966 205f 5f6e  de of an `if __n
+000287c0: 616d 655f 5f20 3d3d 2022 5f5f 6d61 696e  ame__ == "__main
+000287d0: 5f5f 2260 2067 7561 7264 2e0a 0a60 7061  __"` guard...`pa
+000287e0: 7261 6c6c 656c 5f6d 6170 6020 7375 7070  rallel_map` supp
+000287f0: 6f72 7473 2061 2060 6368 756e 6b73 697a  orts a `chunksiz
+00028800: 6560 2061 7267 756d 656e 742c 2077 6869  e` argument, whi
+00028810: 6368 2064 6574 6572 6d69 6e65 7320 686f  ch determines ho
+00028820: 7720 6d61 6e79 2069 7465 6d73 2061 7265  w many items are
+00028830: 2070 6173 7365 6420 746f 2065 6163 6820   passed to each 
+00028840: 7072 6f63 6573 7320 6174 2061 2074 696d  process at a tim
+00028850: 652e 204c 6172 6765 7220 7661 6c75 6573  e. Larger values
+00028860: 206f 6620 5f63 6875 6e6b 7369 7a65 5f20   of _chunksize_ 
+00028870: 6172 6520 7265 636f 6d6d 656e 6465 6420  are recommended 
+00028880: 7768 656e 2064 6561 6c69 6e67 2077 6974  when dealing wit
+00028890: 6820 7665 7279 206c 6f6e 6720 6974 6572  h very long iter
+000288a0: 6162 6c65 732e 2041 6464 6974 696f 6e61  ables. Additiona
+000288b0: 6c6c 792c 2069 6e20 7468 6520 6d75 6c74  lly, in the mult
+000288c0: 692d 6974 6572 6162 6c65 2063 6173 652c  i-iterable case,
+000288d0: 205f 7374 7269 6374 5f20 6361 6e20 6265   _strict_ can be
+000288e0: 2073 6574 2074 6f20 6054 7275 6560 2074   set to `True` t
+000288f0: 6f20 656e 7375 7265 2074 6861 7420 616c  o ensure that al
+00028900: 6c20 6974 6572 6162 6c65 7320 6172 6520  l iterables are 
+00028910: 7468 6520 7361 6d65 206c 656e 6774 682e  the same length.
+00028920: 0a0a 4966 206d 756c 7469 706c 6520 7365  ..If multiple se
+00028930: 7175 656e 7469 616c 2063 616c 6c73 2074  quential calls t
+00028940: 6f20 6070 6172 616c 6c65 6c5f 6d61 7060  o `parallel_map`
+00028950: 206e 6565 6420 746f 2062 6520 6d61 6465   need to be made
+00028960: 2c20 6974 2069 7320 6869 6768 6c79 2072  , it is highly r
+00028970: 6563 6f6d 6d65 6e64 6564 2074 6861 7420  ecommended that 
+00028980: 7468 6579 2062 6520 646f 6e65 2069 6e73  they be done ins
+00028990: 6964 6520 6f66 2061 2060 7769 7468 2070  ide of a `with p
+000289a0: 6172 616c 6c65 6c5f 6d61 702e 6d75 6c74  arallel_map.mult
+000289b0: 6970 6c65 5f73 6571 7565 6e74 6961 6c5f  iple_sequential_
+000289c0: 6361 6c6c 7328 293a 6020 626c 6f63 6b2c  calls():` block,
+000289d0: 2077 6869 6368 2077 696c 6c20 6361 7573   which will caus
+000289e0: 6520 7468 6520 6469 6666 6572 656e 7420  e the different 
+000289f0: 6361 6c6c 7320 746f 2075 7365 2074 6865  calls to use the
+00028a00: 2073 616d 6520 7072 6f63 6573 7320 706f   same process po
+00028a10: 6f6c 2061 6e64 2072 6573 756c 7420 696e  ol and result in
+00028a20: 2060 7061 7261 6c6c 656c 5f6d 6170 6020   `parallel_map` 
+00028a30: 696d 6d65 6469 6174 656c 7920 7265 7475  immediately retu
+00028a40: 726e 696e 6720 6120 6c69 7374 2072 6174  rning a list rat
+00028a50: 6865 7220 7468 616e 2061 2060 7061 7261  her than a `para
+00028a60: 6c6c 656c 5f6d 6170 6020 6f62 6a65 6374  llel_map` object
+00028a70: 2e20 4966 206d 756c 7469 706c 6520 7365  . If multiple se
+00028a80: 7175 656e 7469 616c 2063 616c 6c73 2061  quential calls a
+00028a90: 7265 206e 6563 6573 7361 7279 2061 6e64  re necessary and
+00028aa0: 2074 6865 206c 617a 696e 6573 7320 6f66   the laziness of
+00028ab0: 2070 6172 616c 6c65 6c5f 6d61 7020 6973   parallel_map is
+00028ac0: 2072 6571 7569 7265 642c 2074 6865 6e20   required, then 
+00028ad0: 7468 6520 6070 6172 616c 6c65 6c5f 6d61  the `parallel_ma
+00028ae0: 7060 206f 626a 6563 7473 2073 686f 756c  p` objects shoul
+00028af0: 6420 6265 2063 6f6e 7374 7275 6374 6564  d be constructed
+00028b00: 2062 6566 6f72 6520 7468 6520 606d 756c   before the `mul
+00028b10: 7469 706c 655f 7365 7175 656e 7469 616c  tiple_sequential
+00028b20: 5f63 616c 6c73 6020 626c 6f63 6b20 616e  _calls` block an
+00028b30: 6420 7468 656e 206f 6e6c 7920 6974 6572  d then only iter
+00028b40: 6174 6564 206f 7665 7220 6f6e 6365 2069  ated over once i
+00028b50: 6e73 6964 6520 7468 6520 626c 6f63 6b2e  nside the block.
+00028b60: 0a0a 6070 6172 616c 6c65 6c5f 6d61 702e  ..`parallel_map.
+00028b70: 6d75 6c74 6970 6c65 5f73 6571 7565 6e74  multiple_sequent
+00028b80: 6961 6c5f 6361 6c6c 7360 2061 6c73 6f20  ial_calls` also 
+00028b90: 7375 7070 6f72 7473 2061 2060 6d61 785f  supports a `max_
+00028ba0: 776f 726b 6572 7360 2061 7267 756d 656e  workers` argumen
+00028bb0: 7420 746f 2073 6574 2074 6865 206e 756d  t to set the num
+00028bc0: 6265 7220 6f66 2070 726f 6365 7373 6573  ber of processes
+00028bd0: 2e0a 0a23 2323 2323 2050 7974 686f 6e20  ...##### Python 
+00028be0: 446f 6373 0a0a 2a2a 7061 7261 6c6c 656c  Docs..**parallel
+00028bf0: 5f6d 6170 2a2a 285f 6675 6e63 2c20 5c2a  _map**(_func, \*
+00028c00: 6974 6572 6162 6c65 735f 2c20 5f63 6875  iterables_, _chu
+00028c10: 6e6b 7369 7a65 5f3d 6031 6029 0a0a 4571  nksize_=`1`)..Eq
+00028c20: 7569 7661 6c65 6e74 2074 6f20 606d 6170  uivalent to `map
+00028c30: 2866 756e 632c 202a 6974 6572 6162 6c65  (func, *iterable
+00028c40: 7329 6020 6578 6365 7074 205f 6675 6e63  s)` except _func
+00028c50: 5f20 6973 2065 7865 6375 7465 6420 6173  _ is executed as
+00028c60: 796e 6368 726f 6e6f 7573 6c79 2061 6e64  ynchronously and
+00028c70: 2073 6576 6572 616c 2063 616c 6c73 2074   several calls t
+00028c80: 6f20 5f66 756e 635f 206d 6179 2062 6520  o _func_ may be 
+00028c90: 6d61 6465 2063 6f6e 6375 7272 656e 746c  made concurrentl
+00028ca0: 792e 2049 6620 6120 6361 6c6c 2072 6169  y. If a call rai
+00028cb0: 7365 7320 616e 2065 7863 6570 7469 6f6e  ses an exception
+00028cc0: 2c20 7468 656e 2074 6861 7420 6578 6365  , then that exce
+00028cd0: 7074 696f 6e20 7769 6c6c 2062 6520 7261  ption will be ra
+00028ce0: 6973 6564 2077 6865 6e20 6974 7320 7661  ised when its va
+00028cf0: 6c75 6520 6973 2072 6574 7269 6576 6564  lue is retrieved
+00028d00: 2066 726f 6d20 7468 6520 6974 6572 6174   from the iterat
+00028d10: 6f72 2e0a 0a60 7061 7261 6c6c 656c 5f6d  or...`parallel_m
+00028d20: 6170 6020 6368 6f70 7320 7468 6520 6974  ap` chops the it
+00028d30: 6572 6162 6c65 2069 6e74 6f20 6120 6e75  erable into a nu
+00028d40: 6d62 6572 206f 6620 6368 756e 6b73 2077  mber of chunks w
+00028d50: 6869 6368 2069 7420 7375 626d 6974 7320  hich it submits 
+00028d60: 746f 2074 6865 2070 726f 6365 7373 2070  to the process p
+00028d70: 6f6f 6c20 6173 2073 6570 6172 6174 6520  ool as separate 
+00028d80: 7461 736b 732e 2054 6865 2028 6170 7072  tasks. The (appr
+00028d90: 6f78 696d 6174 6529 2073 697a 6520 6f66  oximate) size of
+00028da0: 2074 6865 7365 2063 6875 6e6b 7320 6361   these chunks ca
+00028db0: 6e20 6265 2073 7065 6369 6669 6564 2062  n be specified b
+00028dc0: 7920 7365 7474 696e 6720 5f63 6875 6e6b  y setting _chunk
+00028dd0: 7369 7a65 5f20 746f 2061 2070 6f73 6974  size_ to a posit
+00028de0: 6976 6520 696e 7465 6765 722e 2046 6f72  ive integer. For
+00028df0: 2076 6572 7920 6c6f 6e67 2069 7465 7261   very long itera
+00028e00: 626c 6573 2075 7369 6e67 2061 206c 6172  bles using a lar
+00028e10: 6765 2076 616c 7565 2066 6f72 205f 6368  ge value for _ch
+00028e20: 756e 6b73 697a 655f 2063 616e 206d 616b  unksize_ can mak
+00028e30: 6520 7468 6520 6a6f 6220 636f 6d70 6c65  e the job comple
+00028e40: 7465 202a 2a6d 7563 682a 2a20 6661 7374  te **much** fast
+00028e50: 6572 2074 6861 6e20 7573 696e 6720 7468  er than using th
+00028e60: 6520 6465 6661 756c 7420 7661 6c75 6520  e default value 
+00028e70: 6f66 2060 3160 2e0a 0a23 2323 2323 2045  of `1`...##### E
+00028e80: 7861 6d70 6c65 0a0a 2a2a 436f 636f 6e75  xample..**Coconu
+00028e90: 743a 2a2a 0a60 6060 636f 636f 6e75 740a  t:**.```coconut.
+00028ea0: 7061 7261 6c6c 656c 5f6d 6170 2870 6f77  parallel_map(pow
+00028eb0: 2428 3229 2c20 7261 6e67 6528 3130 3029  $(2), range(100)
+00028ec0: 2920 7c3e 206c 6973 7420 7c3e 2070 7269  ) |> list |> pri
+00028ed0: 6e74 0a60 6060 0a0a 2a2a 5079 7468 6f6e  nt.```..**Python
+00028ee0: 3a2a 2a0a 6060 6063 6f63 6f6e 7574 5f70  :**.```coconut_p
+00028ef0: 7974 686f 6e0a 696d 706f 7274 2066 756e  ython.import fun
+00028f00: 6374 6f6f 6c73 0a66 726f 6d20 6d75 6c74  ctools.from mult
+00028f10: 6970 726f 6365 7373 696e 6720 696d 706f  iprocessing impo
+00028f20: 7274 2050 6f6f 6c0a 7769 7468 2050 6f6f  rt Pool.with Poo
+00028f30: 6c28 2920 6173 2070 6f6f 6c3a 0a20 2020  l() as pool:.   
+00028f40: 2070 7269 6e74 286c 6973 7428 706f 6f6c   print(list(pool
+00028f50: 2e69 6d61 7028 6675 6e63 746f 6f6c 732e  .imap(functools.
+00028f60: 7061 7274 6961 6c28 706f 772c 2032 292c  partial(pow, 2),
+00028f70: 2072 616e 6765 2831 3030 2929 2929 0a60   range(100)))).`
+00028f80: 6060 0a0a 2323 2323 2060 636f 6e63 7572  ``..#### `concur
+00028f90: 7265 6e74 5f6d 6170 600a 0a2a 2a63 6f6e  rent_map`..**con
+00028fa0: 6375 7272 656e 745c 5f6d 6170 2a2a 285f  current\_map**(_
+00028fb0: 6675 6e63 7469 6f6e 5f2c 202a 5f69 7465  function_, *_ite
+00028fc0: 7261 626c 6573 5f2c 202a 2c20 5f63 6875  rables_, *, _chu
+00028fd0: 6e6b 7369 7a65 5f3d 6031 602c 205f 7374  nksize_=`1`, _st
+00028fe0: 7269 6374 5f3d 6046 616c 7365 6029 0a0a  rict_=`False`)..
+00028ff0: 436f 636f 6e75 7420 7072 6f76 6964 6573  Coconut provides
+00029000: 2061 2063 6f6e 6375 7272 656e 7420 7665   a concurrent ve
+00029010: 7273 696f 6e20 6f66 205b 6070 6172 616c  rsion of [`paral
+00029020: 6c65 6c5f 6d61 7060 5d28 2370 6172 616c  lel_map`](#paral
+00029030: 6c65 6c5f 6d61 7029 2075 6e64 6572 2074  lel_map) under t
+00029040: 6865 206e 616d 6520 6063 6f6e 6375 7272  he name `concurr
+00029050: 656e 745f 6d61 7060 2e20 6063 6f6e 6375  ent_map`. `concu
+00029060: 7272 656e 745f 6d61 7060 2062 6568 6176  rrent_map` behav
+00029070: 6573 2069 6465 6e74 6963 616c 6c79 2074  es identically t
+00029080: 6f20 6070 6172 616c 6c65 6c5f 6d61 7060  o `parallel_map`
+00029090: 2028 696e 636c 7564 696e 6720 7375 7070   (including supp
+000290a0: 6f72 7420 666f 7220 6063 6f6e 6375 7272  ort for `concurr
+000290b0: 656e 745f 6d61 702e 6d75 6c74 6970 6c65  ent_map.multiple
+000290c0: 5f73 6571 7565 6e74 6961 6c5f 6361 6c6c  _sequential_call
+000290d0: 7360 2920 6578 6365 7074 2074 6861 7420  s`) except that 
+000290e0: 6974 2075 7365 7320 6d75 6c74 6974 6872  it uses multithr
+000290f0: 6561 6469 6e67 2069 6e73 7465 6164 206f  eading instead o
+00029100: 6620 6d75 6c74 6970 726f 6365 7373 696e  f multiprocessin
+00029110: 672c 2061 6e64 2069 7320 7468 6572 6566  g, and is theref
+00029120: 6f72 6520 7072 696d 6172 696c 7920 7573  ore primarily us
+00029130: 6566 756c 206f 6e6c 7920 666f 7220 494f  eful only for IO
+00029140: 2d62 6f75 6e64 2074 6173 6b73 2064 7565  -bound tasks due
+00029150: 2074 6f20 4350 7974 686f 6e27 7320 476c   to CPython's Gl
+00029160: 6f62 616c 2049 6e74 6572 7072 6574 6572  obal Interpreter
+00029170: 204c 6f63 6b2e 0a0a 2323 2323 2320 5079   Lock...##### Py
+00029180: 7468 6f6e 2044 6f63 730a 0a2a 2a63 6f6e  thon Docs..**con
+00029190: 6375 7272 656e 745f 6d61 702a 2a28 5f66  current_map**(_f
+000291a0: 756e 632c 205c 2a69 7465 7261 626c 6573  unc, \*iterables
+000291b0: 5f2c 205f 6368 756e 6b73 697a 655f 3d60  _, _chunksize_=`
+000291c0: 3160 290a 0a45 7175 6976 616c 656e 7420  1`)..Equivalent 
+000291d0: 746f 2060 6d61 7028 6675 6e63 2c20 2a69  to `map(func, *i
+000291e0: 7465 7261 626c 6573 2960 2065 7863 6570  terables)` excep
+000291f0: 7420 5f66 756e 635f 2069 7320 6578 6563  t _func_ is exec
+00029200: 7574 6564 2061 7379 6e63 6872 6f6e 6f75  uted asynchronou
+00029210: 736c 7920 616e 6420 7365 7665 7261 6c20  sly and several 
+00029220: 6361 6c6c 7320 746f 205f 6675 6e63 5f20  calls to _func_ 
+00029230: 6d61 7920 6265 206d 6164 6520 636f 6e63  may be made conc
+00029240: 7572 7265 6e74 6c79 2e20 4966 2061 2063  urrently. If a c
+00029250: 616c 6c20 7261 6973 6573 2061 6e20 6578  all raises an ex
+00029260: 6365 7074 696f 6e2c 2074 6865 6e20 7468  ception, then th
+00029270: 6174 2065 7863 6570 7469 6f6e 2077 696c  at exception wil
+00029280: 6c20 6265 2072 6169 7365 6420 7768 656e  l be raised when
+00029290: 2069 7473 2076 616c 7565 2069 7320 7265   its value is re
+000292a0: 7472 6965 7665 6420 6672 6f6d 2074 6865  trieved from the
+000292b0: 2069 7465 7261 746f 722e 0a0a 6063 6f6e   iterator...`con
+000292c0: 6375 7272 656e 745f 6d61 7060 2063 686f  current_map` cho
+000292d0: 7073 2074 6865 2069 7465 7261 626c 6520  ps the iterable 
+000292e0: 696e 746f 2061 206e 756d 6265 7220 6f66  into a number of
+000292f0: 2063 6875 6e6b 7320 7768 6963 6820 6974   chunks which it
+00029300: 2073 7562 6d69 7473 2074 6f20 7468 6520   submits to the 
+00029310: 7468 7265 6164 2070 6f6f 6c20 6173 2073  thread pool as s
+00029320: 6570 6172 6174 6520 7461 736b 732e 2054  eparate tasks. T
+00029330: 6865 2028 6170 7072 6f78 696d 6174 6529  he (approximate)
+00029340: 2073 697a 6520 6f66 2074 6865 7365 2063   size of these c
+00029350: 6875 6e6b 7320 6361 6e20 6265 2073 7065  hunks can be spe
+00029360: 6369 6669 6564 2062 7920 7365 7474 696e  cified by settin
+00029370: 6720 5f63 6875 6e6b 7369 7a65 5f20 746f  g _chunksize_ to
+00029380: 2061 2070 6f73 6974 6976 6520 696e 7465   a positive inte
+00029390: 6765 722e 2046 6f72 2076 6572 7920 6c6f  ger. For very lo
+000293a0: 6e67 2069 7465 7261 626c 6573 2075 7369  ng iterables usi
+000293b0: 6e67 2061 206c 6172 6765 2076 616c 7565  ng a large value
+000293c0: 2066 6f72 205f 6368 756e 6b73 697a 655f   for _chunksize_
+000293d0: 2063 616e 206d 616b 6520 7468 6520 6a6f   can make the jo
+000293e0: 6220 636f 6d70 6c65 7465 202a 2a6d 7563  b complete **muc
+000293f0: 682a 2a20 6661 7374 6572 2074 6861 6e20  h** faster than 
+00029400: 7573 696e 6720 7468 6520 6465 6661 756c  using the defaul
+00029410: 7420 7661 6c75 6520 6f66 2060 3160 2e0a  t value of `1`..
+00029420: 0a23 2323 2323 2045 7861 6d70 6c65 0a0a  .##### Example..
+00029430: 2a2a 436f 636f 6e75 743a 2a2a 0a60 6060  **Coconut:**.```
+00029440: 636f 636f 6e75 740a 636f 6e63 7572 7265  coconut.concurre
+00029450: 6e74 5f6d 6170 2867 6574 5f64 6174 615f  nt_map(get_data_
+00029460: 666f 725f 7573 6572 2c20 6765 745f 616c  for_user, get_al
+00029470: 6c5f 7573 6572 7328 2929 207c 3e20 6c69  l_users()) |> li
+00029480: 7374 207c 3e20 7072 696e 740a 6060 600a  st |> print.```.
+00029490: 0a2a 2a50 7974 686f 6e3a 2a2a 0a60 6060  .**Python:**.```
+000294a0: 636f 636f 6e75 745f 7079 7468 6f6e 0a69  coconut_python.i
+000294b0: 6d70 6f72 7420 6675 6e63 746f 6f6c 730a  mport functools.
+000294c0: 696d 706f 7274 2063 6f6e 6375 7272 656e  import concurren
+000294d0: 742e 6675 7475 7265 730a 7769 7468 2063  t.futures.with c
+000294e0: 6f6e 6375 7272 656e 742e 6675 7475 7265  oncurrent.future
+000294f0: 732e 5468 7265 6164 506f 6f6c 4578 6563  s.ThreadPoolExec
+00029500: 7574 6f72 2829 2061 7320 6578 6563 7574  utor() as execut
+00029510: 6f72 3a0a 2020 2020 7072 696e 7428 6c69  or:.    print(li
+00029520: 7374 2865 7865 6375 746f 722e 6d61 7028  st(executor.map(
+00029530: 6765 745f 6461 7461 5f66 6f72 5f75 7365  get_data_for_use
+00029540: 722c 2067 6574 5f61 6c6c 5f75 7365 7273  r, get_all_users
+00029550: 2829 2929 290a 6060 600a 0a23 2323 2320  ()))).```..#### 
+00029560: 6074 6565 600a 0a2a 2a74 6565 2a2a 285f  `tee`..**tee**(_
+00029570: 6974 6572 6162 6c65 5f2c 205f 6e5f 3d60  iterable_, _n_=`
+00029580: 3260 290a 0a43 6f63 6f6e 7574 2070 726f  2`)..Coconut pro
+00029590: 7669 6465 7320 616e 206f 7074 696d 697a  vides an optimiz
+000295a0: 6564 2076 6572 7369 6f6e 206f 6620 6069  ed version of `i
+000295b0: 7465 7274 6f6f 6c73 2e74 6565 6020 6173  tertools.tee` as
+000295c0: 2061 2062 7569 6c74 2d69 6e20 756e 6465   a built-in unde
+000295d0: 7220 7468 6520 6e61 6d65 2060 7465 6560  r the name `tee`
+000295e0: 2e0a 0a54 686f 7567 6820 6074 6565 6020  ...Though `tee` 
+000295f0: 6973 206e 6f74 2064 6570 7265 6361 7465  is not deprecate
+00029600: 642c 205b 6072 6569 7465 7261 626c 6560  d, [`reiterable`
+00029610: 5d28 2372 6569 7465 7261 626c 6529 2069  ](#reiterable) i
+00029620: 7320 6765 6e65 7261 6c6c 7920 7265 636f  s generally reco
+00029630: 6d6d 656e 6465 6420 6f76 6572 2060 7465  mmended over `te
+00029640: 6560 2e0a 0a43 7573 746f 6d20 6074 6565  e`...Custom `tee
+00029650: 602f 6072 6569 7465 7261 626c 6560 2069  `/`reiterable` i
+00029660: 6d70 6c65 6d65 6e74 6174 696f 6e73 2066  mplementations f
+00029670: 6f72 2063 7573 746f 6d20 5b43 6f6e 7461  or custom [Conta
+00029680: 696e 6572 732f 436f 6c6c 6563 7469 6f6e  iners/Collection
+00029690: 735d 2868 7474 7073 3a2f 2f64 6f63 732e  s](https://docs.
+000296a0: 7079 7468 6f6e 2e6f 7267 2f33 2f6c 6962  python.org/3/lib
+000296b0: 7261 7279 2f63 6f6c 6c65 6374 696f 6e73  rary/collections
+000296c0: 2e61 6263 2e68 746d 6c29 2073 686f 756c  .abc.html) shoul
+000296d0: 6420 6265 2070 7574 2069 6e20 7468 6520  d be put in the 
+000296e0: 605f 5f63 6f70 795f 5f60 206d 6574 686f  `__copy__` metho
+000296f0: 642e 204e 6f74 6520 7468 6174 2061 6c6c  d. Note that all
+00029700: 205b 5365 7175 656e 6365 732f 4d61 7070   [Sequences/Mapp
+00029710: 696e 6773 2f53 6574 735d 2868 7474 7073  ings/Sets](https
+00029720: 3a2f 2f64 6f63 732e 7079 7468 6f6e 2e6f  ://docs.python.o
+00029730: 7267 2f33 2f6c 6962 7261 7279 2f63 6f6c  rg/3/library/col
+00029740: 6c65 6374 696f 6e73 2e61 6263 2e68 746d  lections.abc.htm
+00029750: 6c29 2061 7265 2061 6c77 6179 7320 6173  l) are always as
+00029760: 7375 6d65 6420 746f 2062 6520 7265 6974  sumed to be reit
+00029770: 6572 6162 6c65 2065 7665 6e20 7769 7468  erable even with
+00029780: 6f75 7420 6361 6c6c 696e 6720 605f 5f63  out calling `__c
+00029790: 6f70 795f 5f60 2e0a 0a23 2323 2323 2050  opy__`...##### P
+000297a0: 7974 686f 6e20 446f 6373 0a0a 2a2a 7465  ython Docs..**te
+000297b0: 652a 2a28 5f69 7465 7261 626c 652c 206e  e**(_iterable, n
+000297c0: 3d32 5f29 0a0a 5265 7475 726e 205f 6e5f  =2_)..Return _n_
+000297d0: 2069 6e64 6570 656e 6465 6e74 2069 7465   independent ite
+000297e0: 7261 746f 7273 2066 726f 6d20 6120 7369  rators from a si
+000297f0: 6e67 6c65 2069 7465 7261 626c 652e 2045  ngle iterable. E
+00029800: 7175 6976 616c 656e 7420 746f 3a0a 6060  quivalent to:.``
+00029810: 6063 6f63 6f6e 7574 5f70 7974 686f 6e0a  `coconut_python.
+00029820: 6465 6620 7465 6528 6974 6572 6162 6c65  def tee(iterable
+00029830: 2c20 6e3d 3229 3a0a 2020 2020 6974 203d  , n=2):.    it =
+00029840: 2069 7465 7228 6974 6572 6162 6c65 290a   iter(iterable).
+00029850: 2020 2020 6465 7175 6573 203d 205b 636f      deques = [co
+00029860: 6c6c 6563 7469 6f6e 732e 6465 7175 6528  llections.deque(
+00029870: 2920 666f 7220 6920 696e 2072 616e 6765  ) for i in range
+00029880: 286e 295d 0a20 2020 2064 6566 2067 656e  (n)].    def gen
+00029890: 286d 7964 6571 7565 293a 0a20 2020 2020  (mydeque):.     
+000298a0: 2020 2077 6869 6c65 2054 7275 653a 0a20     while True:. 
+000298b0: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+000298c0: 7420 6d79 6465 7175 653a 2020 2020 2020  t mydeque:      
+000298d0: 2020 2020 2020 2023 2077 6865 6e20 7468         # when th
+000298e0: 6520 6c6f 6361 6c20 6465 7175 6520 6973  e local deque is
+000298f0: 2065 6d70 7479 0a20 2020 2020 2020 2020   empty.         
+00029900: 2020 2020 2020 206e 6577 7661 6c20 3d20         newval = 
+00029910: 6e65 7874 2869 7429 2020 2020 2020 2023  next(it)       #
+00029920: 2066 6574 6368 2061 206e 6577 2076 616c   fetch a new val
+00029930: 7565 2061 6e64 0a20 2020 2020 2020 2020  ue and.         
+00029940: 2020 2020 2020 2066 6f72 2064 2069 6e20         for d in 
+00029950: 6465 7175 6573 3a20 2020 2020 2020 2023  deques:        #
+00029960: 206c 6f61 6420 6974 2074 6f20 616c 6c20   load it to all 
+00029970: 7468 6520 6465 7175 6573 0a20 2020 2020  the deques.     
+00029980: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00029990: 2e61 7070 656e 6428 6e65 7776 616c 290a  .append(newval).
+000299a0: 2020 2020 2020 2020 2020 2020 7969 656c              yiel
+000299b0: 6420 6d79 6465 7175 652e 706f 706c 6566  d mydeque.poplef
+000299c0: 7428 290a 2020 2020 7265 7475 726e 2074  t().    return t
+000299d0: 7570 6c65 2867 656e 2864 2920 666f 7220  uple(gen(d) for 
+000299e0: 6420 696e 2064 6571 7565 7329 0a60 6060  d in deques).```
+000299f0: 0a4f 6e63 6520 6074 6565 2829 6020 6861  .Once `tee()` ha
+00029a00: 7320 6d61 6465 2061 2073 706c 6974 2c20  s made a split, 
+00029a10: 7468 6520 6f72 6967 696e 616c 205f 6974  the original _it
+00029a20: 6572 6162 6c65 5f20 7368 6f75 6c64 206e  erable_ should n
+00029a30: 6f74 2062 6520 7573 6564 2061 6e79 7768  ot be used anywh
+00029a40: 6572 6520 656c 7365 3b20 6f74 6865 7277  ere else; otherw
+00029a50: 6973 652c 2074 6865 205f 6974 6572 6162  ise, the _iterab
+00029a60: 6c65 5f20 636f 756c 6420 6765 7420 6164  le_ could get ad
+00029a70: 7661 6e63 6564 2077 6974 686f 7574 2074  vanced without t
+00029a80: 6865 2074 6565 206f 626a 6563 7473 2062  he tee objects b
+00029a90: 6569 6e67 2069 6e66 6f72 6d65 642e 0a0a  eing informed...
+00029aa0: 5468 6973 2069 7465 7274 6f6f 6c20 6d61  This itertool ma
+00029ab0: 7920 7265 7175 6972 6520 7369 676e 6966  y require signif
+00029ac0: 6963 616e 7420 6175 7869 6c69 6172 7920  icant auxiliary 
+00029ad0: 7374 6f72 6167 6520 2864 6570 656e 6469  storage (dependi
+00029ae0: 6e67 206f 6e20 686f 7720 6d75 6368 2074  ng on how much t
+00029af0: 656d 706f 7261 7279 2064 6174 6120 6e65  emporary data ne
+00029b00: 6564 7320 746f 2062 6520 7374 6f72 6564  eds to be stored
+00029b10: 292e 2049 6e20 6765 6e65 7261 6c2c 2069  ). In general, i
+00029b20: 6620 6f6e 6520 6974 6572 6174 6f72 2075  f one iterator u
+00029b30: 7365 7320 6d6f 7374 206f 7220 616c 6c20  ses most or all 
+00029b40: 6f66 2074 6865 2064 6174 6120 6265 666f  of the data befo
+00029b50: 7265 2061 6e6f 7468 6572 2069 7465 7261  re another itera
+00029b60: 746f 7220 7374 6172 7473 2c20 6974 2069  tor starts, it i
+00029b70: 7320 6661 7374 6572 2074 6f20 7573 6520  s faster to use 
+00029b80: 606c 6973 7428 2960 2069 6e73 7465 6164  `list()` instead
+00029b90: 206f 6620 6074 6565 2829 602e 0a0a 2323   of `tee()`...##
+00029ba0: 2323 2320 4578 616d 706c 650a 0a2a 2a43  ### Example..**C
+00029bb0: 6f63 6f6e 7574 3a2a 2a0a 6060 6063 6f63  oconut:**.```coc
+00029bc0: 6f6e 7574 0a6f 7269 6769 6e61 6c2c 2074  onut.original, t
+00029bd0: 656d 7020 3d20 7465 6528 6f72 6967 696e  emp = tee(origin
+00029be0: 616c 290a 736c 6963 6564 203d 2074 656d  al).sliced = tem
+00029bf0: 7024 5b35 3a5d 0a60 6060 0a0a 2a2a 5079  p$[5:].```..**Py
+00029c00: 7468 6f6e 3a2a 2a0a 6060 6063 6f63 6f6e  thon:**.```cocon
+00029c10: 7574 5f70 7974 686f 6e0a 696d 706f 7274  ut_python.import
+00029c20: 2069 7465 7274 6f6f 6c73 0a6f 7269 6769   itertools.origi
+00029c30: 6e61 6c2c 2074 656d 7020 3d20 6974 6572  nal, temp = iter
+00029c40: 746f 6f6c 732e 7465 6528 6f72 6967 696e  tools.tee(origin
+00029c50: 616c 290a 736c 6963 6564 203d 2069 7465  al).sliced = ite
+00029c60: 7274 6f6f 6c73 2e69 736c 6963 6528 7465  rtools.islice(te
+00029c70: 6d70 2c20 352c 204e 6f6e 6529 0a60 6060  mp, 5, None).```
+00029c80: 0a0a 2323 2323 2060 636f 6e73 756d 6560  ..#### `consume`
+00029c90: 0a0a 2a2a 636f 6e73 756d 652a 2a28 5f69  ..**consume**(_i
+00029ca0: 7465 7261 626c 655f 2c20 5f6b 6565 705c  terable_, _keep\
+00029cb0: 5f6c 6173 745f 3d60 3060 290a 0a43 6f63  _last_=`0`)..Coc
+00029cc0: 6f6e 7574 2070 726f 7669 6465 7320 7468  onut provides th
+00029cd0: 6520 6063 6f6e 7375 6d65 6020 6675 6e63  e `consume` func
+00029ce0: 7469 6f6e 2074 6f20 6566 6669 6369 656e  tion to efficien
+00029cf0: 746c 7920 6578 6861 7573 7420 616e 2069  tly exhaust an i
+00029d00: 7465 7261 746f 7220 616e 6420 7468 7573  terator and thus
+00029d10: 2070 6572 666f 726d 2061 6e79 206c 617a   perform any laz
+00029d20: 7920 6576 616c 7561 7469 6f6e 2063 6f6e  y evaluation con
+00029d30: 7461 696e 6564 2077 6974 6869 6e20 6974  tained within it
+00029d40: 2e20 6063 6f6e 7375 6d65 6020 7461 6b65  . `consume` take
+00029d50: 7320 6f6e 6520 6f70 7469 6f6e 616c 2061  s one optional a
+00029d60: 7267 756d 656e 742c 2060 6b65 6570 5f6c  rgument, `keep_l
+00029d70: 6173 7460 2c20 7468 6174 2064 6566 6175  ast`, that defau
+00029d80: 6c74 7320 746f 2030 2061 6e64 2073 7065  lts to 0 and spe
+00029d90: 6369 6669 6573 2068 6f77 206d 616e 792c  cifies how many,
+00029da0: 2069 6620 616e 792c 2069 7465 6d73 2066   if any, items f
+00029db0: 726f 6d20 7468 6520 656e 6420 746f 2072  rom the end to r
+00029dc0: 6574 7572 6e20 6173 2061 2073 6571 7565  eturn as a seque
+00029dd0: 6e63 6520 2860 4e6f 6e65 6020 7769 6c6c  nce (`None` will
+00029de0: 206b 6565 7020 616c 6c20 656c 656d 656e   keep all elemen
+00029df0: 7473 292e 0a0a 4571 7569 7661 6c65 6e74  ts)...Equivalent
+00029e00: 2074 6f3a 0a60 6060 636f 636f 6e75 740a   to:.```coconut.
+00029e10: 6465 6620 636f 6e73 756d 6528 6974 6572  def consume(iter
+00029e20: 6162 6c65 2c20 6b65 6570 5f6c 6173 743d  able, keep_last=
+00029e30: 3029 3a0a 2020 2020 2222 2246 756c 6c79  0):.    """Fully
+00029e40: 2065 7868 6175 7374 2069 7465 7261 626c   exhaust iterabl
+00029e50: 6520 616e 6420 7265 7475 726e 2074 6865  e and return the
+00029e60: 206c 6173 7420 6b65 6570 5f6c 6173 7420   last keep_last 
+00029e70: 656c 656d 656e 7473 2e22 2222 0a20 2020  elements.""".   
+00029e80: 2072 6574 7572 6e20 636f 6c6c 6563 7469   return collecti
+00029e90: 6f6e 732e 6465 7175 6528 6974 6572 6162  ons.deque(iterab
+00029ea0: 6c65 2c20 6d61 786c 656e 3d6b 6565 705f  le, maxlen=keep_
+00029eb0: 6c61 7374 2920 2023 2066 6173 7465 7374  last)  # fastest
+00029ec0: 2077 6179 2074 6f20 6578 6861 7573 7420   way to exhaust 
+00029ed0: 616e 2069 7465 7261 746f 720a 6060 600a  an iterator.```.
+00029ee0: 0a23 2323 2323 2052 6174 696f 6e61 6c65  .##### Rationale
+00029ef0: 0a0a 496e 2074 6865 2070 726f 6365 7373  ..In the process
+00029f00: 206f 6620 6c61 7a69 6c79 2061 7070 6c79   of lazily apply
+00029f10: 696e 6720 6f70 6572 6174 696f 6e73 2074  ing operations t
+00029f20: 6f20 6974 6572 6174 6f72 732c 2065 7665  o iterators, eve
+00029f30: 6e74 7561 6c6c 7920 6120 706f 696e 7420  ntually a point 
+00029f40: 6973 2072 6561 6368 6564 2077 6865 7265  is reached where
+00029f50: 2065 7661 6c75 6174 696f 6e20 6f66 2074   evaluation of t
+00029f60: 6865 2069 7465 7261 746f 7220 6973 206e  he iterator is n
+00029f70: 6563 6573 7361 7279 2e20 546f 2064 6f20  ecessary. To do 
+00029f80: 7468 6973 2065 6666 6963 6965 6e74 6c79  this efficiently
+00029f90: 2c20 436f 636f 6e75 7420 7072 6f76 6964  , Coconut provid
+00029fa0: 6573 2074 6865 2060 636f 6e73 756d 6560  es the `consume`
+00029fb0: 2066 756e 6374 696f 6e2c 2077 6869 6368   function, which
+00029fc0: 2077 696c 6c20 6675 6c6c 7920 6578 6861   will fully exha
+00029fd0: 7573 7420 7468 6520 6974 6572 6174 6f72  ust the iterator
+00029fe0: 2067 6976 656e 2074 6f20 6974 2e0a 0a23   given to it...#
+00029ff0: 2323 2323 2045 7861 6d70 6c65 0a0a 2a2a  #### Example..**
+0002a000: 436f 636f 6e75 743a 2a2a 0a60 6060 636f  Coconut:**.```co
+0002a010: 636f 6e75 740a 7261 6e67 6528 3130 2920  conut.range(10) 
+0002a020: 7c3e 206d 6170 2428 2878 2920 2d3e 2078  |> map$((x) -> x
+0002a030: 2a2a 3229 207c 3e20 6d61 7024 2870 7269  **2) |> map$(pri
+0002a040: 6e74 2920 7c3e 2063 6f6e 7375 6d65 0a60  nt) |> consume.`
+0002a050: 6060 0a0a 2a2a 5079 7468 6f6e 3a2a 2a0a  ``..**Python:**.
+0002a060: 6060 6063 6f63 6f6e 7574 5f70 7974 686f  ```coconut_pytho
+0002a070: 6e0a 636f 6c6c 6563 7469 6f6e 732e 6465  n.collections.de
+0002a080: 7175 6528 6d61 7028 7072 696e 742c 206d  que(map(print, m
+0002a090: 6170 286c 616d 6264 6120 783a 2078 2a2a  ap(lambda x: x**
+0002a0a0: 322c 2072 616e 6765 2831 3029 2929 2c20  2, range(10))), 
+0002a0b0: 6d61 786c 656e 3d30 290a 6060 600a 0a23  maxlen=0).```..#
+0002a0c0: 2323 2054 7970 696e 672d 5370 6563 6966  ## Typing-Specif
+0002a0d0: 6963 2042 7569 6c74 2d49 6e73 0a0a 6060  ic Built-Ins..``
+0002a0e0: 607b 636f 6e74 656e 7473 7d0a 2d2d 2d0a  `{contents}.---.
+0002a0f0: 6c6f 6361 6c3a 0a64 6570 7468 3a20 310a  local:.depth: 1.
+0002a100: 2d2d 2d0a 6060 600a 0a23 2323 2320 6054  ---.```..#### `T
+0002a110: 5950 455f 4348 4543 4b49 4e47 600a 0a54  YPE_CHECKING`..T
+0002a120: 6865 2060 5459 5045 5f43 4845 434b 494e  he `TYPE_CHECKIN
+0002a130: 4760 2076 6172 6961 626c 6520 6973 2073  G` variable is s
+0002a140: 6574 2074 6f20 6046 616c 7365 6020 6174  et to `False` at
+0002a150: 2072 756e 7469 6d65 2061 6e64 2060 5472   runtime and `Tr
+0002a160: 7565 6020 6475 7269 6e67 2074 7970 655f  ue` during type_
+0002a170: 6368 6563 6b69 6e67 2c20 616c 6c6f 7769  checking, allowi
+0002a180: 6e67 2079 6f75 2074 6f20 7072 6576 656e  ng you to preven
+0002a190: 7420 796f 7572 2060 7479 7069 6e67 6020  t your `typing` 
+0002a1a0: 696d 706f 7274 7320 616e 6420 6054 7970  imports and `Typ
+0002a1b0: 6556 6172 6020 6465 6669 6e69 7469 6f6e  eVar` definition
+0002a1c0: 7320 6672 6f6d 2062 6569 6e67 2065 7865  s from being exe
+0002a1d0: 6375 7465 6420 6174 2072 756e 7469 6d65  cuted at runtime
+0002a1e0: 2e20 4279 2077 7261 7070 696e 6720 796f  . By wrapping yo
+0002a1f0: 7572 2060 7479 7069 6e67 6020 696d 706f  ur `typing` impo
+0002a200: 7274 7320 696e 2061 6e20 6069 6620 5459  rts in an `if TY
+0002a210: 5045 5f43 4845 434b 494e 473a 6020 626c  PE_CHECKING:` bl
+0002a220: 6f63 6b2c 2079 6f75 2063 616e 2065 7665  ock, you can eve
+0002a230: 6e20 7573 6520 7468 6520 5b60 7479 7069  n use the [`typi
+0002a240: 6e67 605d 2868 7474 7073 3a2f 2f64 6f63  ng`](https://doc
+0002a250: 732e 7079 7468 6f6e 2e6f 7267 2f33 2f6c  s.python.org/3/l
+0002a260: 6962 7261 7279 2f74 7970 696e 672e 6874  ibrary/typing.ht
+0002a270: 6d6c 2920 6d6f 6475 6c65 206f 6e20 5079  ml) module on Py
+0002a280: 7468 6f6e 2076 6572 7369 6f6e 7320 7468  thon versions th
+0002a290: 6174 2064 6f6e 2774 206e 6174 6976 656c  at don't nativel
+0002a2a0: 7920 7375 7070 6f72 7420 6974 2e20 4675  y support it. Fu
+0002a2b0: 7274 6865 726d 6f72 652c 2060 5459 5045  rthermore, `TYPE
+0002a2c0: 5f43 4845 434b 494e 4760 2063 616e 2061  _CHECKING` can a
+0002a2d0: 6c73 6f20 6265 2075 7365 6420 746f 2068  lso be used to h
+0002a2e0: 6964 6520 636f 6465 2074 6861 7420 6973  ide code that is
+0002a2f0: 206d 6973 7479 7065 6420 6279 2064 6566   mistyped by def
+0002a300: 6175 6c74 2e0a 0a23 2323 2323 2050 7974  ault...##### Pyt
+0002a310: 686f 6e20 446f 6373 0a0a 4120 7370 6563  hon Docs..A spec
+0002a320: 6961 6c20 636f 6e73 7461 6e74 2074 6861  ial constant tha
+0002a330: 7420 6973 2061 7373 756d 6564 2074 6f20  t is assumed to 
+0002a340: 6265 2060 5472 7565 6020 6279 2033 7264  be `True` by 3rd
+0002a350: 2070 6172 7479 2073 7461 7469 6320 7479   party static ty
+0002a360: 7065 2063 6865 636b 6572 732e 2049 7420  pe checkers. It 
+0002a370: 6973 2060 4661 6c73 6560 2061 7420 7275  is `False` at ru
+0002a380: 6e74 696d 652e 2055 7361 6765 3a0a 6060  ntime. Usage:.``
+0002a390: 6063 6f63 6f6e 7574 5f70 7974 686f 6e0a  `coconut_python.
+0002a3a0: 6966 2054 5950 455f 4348 4543 4b49 4e47  if TYPE_CHECKING
+0002a3b0: 3a0a 2020 2020 696d 706f 7274 2065 7870  :.    import exp
+0002a3c0: 656e 7369 7665 5f6d 6f64 0a0a 6465 6620  ensive_mod..def 
+0002a3d0: 6675 6e28 6172 673a 2065 7870 656e 7369  fun(arg: expensi
+0002a3e0: 7665 5f6d 6f64 2e53 6f6d 6554 7970 6529  ve_mod.SomeType)
+0002a3f0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 6c6f   -> None:.    lo
+0002a400: 6361 6c5f 7661 723a 2065 7870 656e 7369  cal_var: expensi
+0002a410: 7665 5f6d 6f64 2e41 6e6f 7468 6572 5479  ve_mod.AnotherTy
+0002a420: 7065 203d 206f 7468 6572 5f66 756e 2829  pe = other_fun()
+0002a430: 0a60 6060 0a0a 2323 2323 2320 4578 616d  .```..##### Exam
+0002a440: 706c 6573 0a0a 2a2a 436f 636f 6e75 743a  ples..**Coconut:
+0002a450: 2a2a 0a60 6060 636f 636f 6e75 740a 6966  **.```coconut.if
+0002a460: 2054 5950 455f 4348 4543 4b49 4e47 3a0a   TYPE_CHECKING:.
+0002a470: 2020 2020 6672 6f6d 2074 7970 696e 6720      from typing 
+0002a480: 696d 706f 7274 204c 6973 740a 783a 204c  import List.x: L
+0002a490: 6973 745b 7374 725d 203d 205b 2261 222c  ist[str] = ["a",
+0002a4a0: 2022 6222 5d0a 6060 600a 0a60 6060 636f   "b"].```..```co
+0002a4b0: 636f 6e75 740a 6966 2054 5950 455f 4348  conut.if TYPE_CH
+0002a4c0: 4543 4b49 4e47 3a0a 2020 2020 6465 6620  ECKING:.    def 
+0002a4d0: 6661 6374 6f72 6961 6c28 6e3a 2069 6e74  factorial(n: int
+0002a4e0: 2920 2d3e 2069 6e74 3a20 2e2e 2e0a 656c  ) -> int: ....el
+0002a4f0: 7365 3a0a 2020 2020 6465 6620 6661 6374  se:.    def fact
+0002a500: 6f72 6961 6c28 3029 203d 2031 0a20 2020  orial(0) = 1.   
+0002a510: 2061 6464 7061 7474 6572 6e20 6465 6620   addpattern def 
+0002a520: 6661 6374 6f72 6961 6c28 6e29 203d 206e  factorial(n) = n
+0002a530: 202a 2066 6163 746f 7269 616c 286e 2d31   * factorial(n-1
+0002a540: 290a 6060 600a 0a2a 2a50 7974 686f 6e3a  ).```..**Python:
+0002a550: 2a2a 0a60 6060 636f 636f 6e75 745f 7079  **.```coconut_py
+0002a560: 7468 6f6e 0a74 7279 3a0a 2020 2020 6672  thon.try:.    fr
+0002a570: 6f6d 2074 7970 696e 6720 696d 706f 7274  om typing import
+0002a580: 2054 5950 455f 4348 4543 4b49 4e47 0a65   TYPE_CHECKING.e
+0002a590: 7863 6570 7420 496d 706f 7274 4572 726f  xcept ImportErro
+0002a5a0: 723a 0a20 2020 2054 5950 455f 4348 4543  r:.    TYPE_CHEC
+0002a5b0: 4b49 4e47 203d 2046 616c 7365 0a0a 6966  KING = False..if
+0002a5c0: 2054 5950 455f 4348 4543 4b49 4e47 3a0a   TYPE_CHECKING:.
+0002a5d0: 2020 2020 6672 6f6d 2074 7970 696e 6720      from typing 
+0002a5e0: 696d 706f 7274 204c 6973 740a 783a 204c  import List.x: L
+0002a5f0: 6973 745b 7374 725d 203d 205b 2261 222c  ist[str] = ["a",
+0002a600: 2022 6222 5d0a 6060 600a 0a60 6060 636f   "b"].```..```co
+0002a610: 636f 6e75 745f 7079 7468 6f6e 0a74 7279  conut_python.try
+0002a620: 3a0a 2020 2020 6672 6f6d 2074 7970 696e  :.    from typin
+0002a630: 6720 696d 706f 7274 2054 5950 455f 4348  g import TYPE_CH
+0002a640: 4543 4b49 4e47 0a65 7863 6570 7420 496d  ECKING.except Im
+0002a650: 706f 7274 4572 726f 723a 0a20 2020 2054  portError:.    T
+0002a660: 5950 455f 4348 4543 4b49 4e47 203d 2046  YPE_CHECKING = F
+0002a670: 616c 7365 0a0a 6966 2054 5950 455f 4348  alse..if TYPE_CH
+0002a680: 4543 4b49 4e47 3a0a 2020 2020 6465 6620  ECKING:.    def 
+0002a690: 6661 6374 6f72 6961 6c28 6e3a 2069 6e74  factorial(n: int
+0002a6a0: 2920 2d3e 2069 6e74 3a20 2e2e 2e0a 656c  ) -> int: ....el
+0002a6b0: 7365 3a0a 2020 2020 6465 6620 6661 6374  se:.    def fact
+0002a6c0: 6f72 6961 6c28 6e29 3a0a 2020 2020 2020  orial(n):.      
+0002a6d0: 2020 6966 206e 203d 3d20 303a 0a20 2020    if n == 0:.   
+0002a6e0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0002a6f0: 310a 2020 2020 2020 2020 656c 7365 3a0a  1.        else:.
+0002a700: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0002a710: 726e 206e 202a 2066 6163 746f 7269 616c  rn n * factorial
+0002a720: 286e 2d31 290a 6060 600a 0a23 2323 2320  (n-1).```..#### 
+0002a730: 6072 6576 6561 6c5f 7479 7065 6020 616e  `reveal_type` an
+0002a740: 6420 6072 6576 6561 6c5f 6c6f 6361 6c73  d `reveal_locals
+0002a750: 600a 0a57 6865 6e20 7573 696e 6720 4d79  `..When using My
+0002a760: 5079 2c20 6072 6576 6561 6c5f 7479 7065  Py, `reveal_type
+0002a770: 283c 6578 7072 3e29 6020 7769 6c6c 2063  (<expr>)` will c
+0002a780: 6175 7365 204d 7950 7920 746f 2070 7269  ause MyPy to pri
+0002a790: 6e74 2074 6865 2074 7970 6520 6f66 2060  nt the type of `
+0002a7a0: 3c65 7870 723e 6020 616e 6420 6072 6576  <expr>` and `rev
+0002a7b0: 6561 6c5f 6c6f 6361 6c73 2829 6020 7769  eal_locals()` wi
+0002a7c0: 6c6c 2063 6175 7365 204d 7950 7920 746f  ll cause MyPy to
+0002a7d0: 2070 7269 6e74 2074 6865 2074 7970 6573   print the types
+0002a7e0: 206f 6620 7468 6520 6375 7272 656e 7420   of the current 
+0002a7f0: 606c 6f63 616c 7328 2960 2e20 4174 2072  `locals()`. At r
+0002a800: 756e 7469 6d65 2c20 6072 6576 6561 6c5f  untime, `reveal_
+0002a810: 7479 7065 2878 2960 2069 7320 616c 7761  type(x)` is alwa
+0002a820: 7973 2074 6865 2069 6465 6e74 6974 7920  ys the identity 
+0002a830: 6675 6e63 7469 6f6e 2061 6e64 2060 7265  function and `re
+0002a840: 7665 616c 5f6c 6f63 616c 7328 2960 2061  veal_locals()` a
+0002a850: 6c77 6179 7320 7265 7475 726e 7320 604e  lways returns `N
+0002a860: 6f6e 6560 2e20 5365 6520 5b74 6865 204d  one`. See [the M
+0002a870: 7950 7920 646f 6375 6d65 6e74 6174 696f  yPy documentatio
+0002a880: 6e5d 2868 7474 7073 3a2f 2f6d 7970 792e  n](https://mypy.
+0002a890: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
+0002a8a0: 6e2f 7374 6162 6c65 2f63 6f6d 6d6f 6e5f  n/stable/common_
+0002a8b0: 6973 7375 6573 2e68 746d 6c23 7265 7665  issues.html#reve
+0002a8c0: 616c 2d74 7970 6529 2066 6f72 206d 6f72  al-type) for mor
+0002a8d0: 6520 696e 666f 726d 6174 696f 6e2e 0a0a  e information...
+0002a8e0: 2323 2323 2320 4578 616d 706c 650a 0a2a  ##### Example..*
+0002a8f0: 2a43 6f63 6f6e 7574 3a2a 2a0a 6060 6063  *Coconut:**.```c
+0002a900: 6f63 6f6e 7574 5f70 7963 6f6e 0a3e 2063  oconut_pycon.> c
+0002a910: 6f63 6f6e 7574 202d 2d6d 7970 790a 436f  oconut --mypy.Co
+0002a920: 636f 6e75 7420 496e 7465 7270 7265 7465  conut Interprete
+0002a930: 7220 7658 2e58 2e58 3a0a 2865 6e74 6572  r vX.X.X:.(enter
+0002a940: 2027 6578 6974 2829 2720 6f72 2070 7265   'exit()' or pre
+0002a950: 7373 2043 7472 6c2d 4420 746f 2065 6e64  ss Ctrl-D to end
+0002a960: 290a 3e3e 3e20 7265 7665 616c 5f74 7970  ).>>> reveal_typ
+0002a970: 6528 666d 6170 290a 3c66 756e 6374 696f  e(fmap).<functio
+0002a980: 6e20 666d 6170 2061 7420 3078 3030 3030  n fmap at 0x0000
+0002a990: 3032 3339 4230 3645 3230 3430 3e0a 3c73  0239B06E2040>.<s
+0002a9a0: 7472 696e 673e 3a31 373a 206e 6f74 653a  tring>:17: note:
+0002a9b0: 2052 6576 6561 6c65 6420 7479 7065 2069   Revealed type i
+0002a9c0: 7320 2764 6566 205b 5f54 2c20 5f55 5d20  s 'def [_T, _U] 
+0002a9d0: 2866 756e 633a 2064 6566 2028 5f54 602d  (func: def (_T`-
+0002a9e0: 3129 202d 3e20 5f55 602d 322c 206f 626a  1) -> _U`-2, obj
+0002a9f0: 3a20 7479 7069 6e67 2e49 7465 7261 626c  : typing.Iterabl
+0002aa00: 655b 5f54 602d 315d 2920 2d3e 2074 7970  e[_T`-1]) -> typ
+0002aa10: 696e 672e 4974 6572 6162 6c65 5b5f 5560  ing.Iterable[_U`
+0002aa20: 2d32 5d27 0a3e 3e3e 0a60 6060 0a0a 2a2a  -2]'.>>>.```..**
+0002aa30: 5079 7468 6f6e 2a2a 0a60 6060 636f 636f  Python**.```coco
+0002aa40: 6e75 745f 7079 7468 6f6e 0a74 7279 3a0a  nut_python.try:.
+0002aa50: 2020 2020 6672 6f6d 2074 7970 696e 6720      from typing 
+0002aa60: 696d 706f 7274 2054 5950 455f 4348 4543  import TYPE_CHEC
+0002aa70: 4b49 4e47 0a65 7863 6570 7420 496d 706f  KING.except Impo
+0002aa80: 7274 4572 726f 723a 0a20 2020 2054 5950  rtError:.    TYP
+0002aa90: 455f 4348 4543 4b49 4e47 203d 2046 616c  E_CHECKING = Fal
+0002aaa0: 7365 0a0a 6966 206e 6f74 2054 5950 455f  se..if not TYPE_
+0002aab0: 4348 4543 4b49 4e47 3a0a 2020 2020 6465  CHECKING:.    de
+0002aac0: 6620 7265 7665 616c 5f74 7970 6528 7829  f reveal_type(x)
+0002aad0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+0002aae0: 2078 0a0a 6672 6f6d 2063 6f63 6f6e 7574   x..from coconut
+0002aaf0: 2e5f 5f63 6f63 6f6e 7574 5f5f 2069 6d70  .__coconut__ imp
+0002ab00: 6f72 7420 666d 6170 0a72 6576 6561 6c5f  ort fmap.reveal_
+0002ab10: 7479 7065 2866 6d61 7029 0a60 6060 0a0a  type(fmap).```..
+0002ab20: 2323 2043 6f63 6f6e 7574 2041 5049 0a0a  ## Coconut API..
+0002ab30: 6060 607b 636f 6e74 656e 7473 7d0a 2d2d  ```{contents}.--
+0002ab40: 2d0a 6c6f 6361 6c3a 0a64 6570 7468 3a20  -.local:.depth: 
+0002ab50: 320a 2d2d 2d0a 6060 600a 0a23 2323 2060  2.---.```..### `
+0002ab60: 636f 636f 6e75 742e 656d 6265 6460 0a0a  coconut.embed`..
+0002ab70: 2a2a 636f 636f 6e75 742e 656d 6265 642a  **coconut.embed*
+0002ab80: 2a28 5f6b 6572 6e65 6c5f 3d60 4e6f 6e65  *(_kernel_=`None
+0002ab90: 602c 205f 6465 7074 685f 3d60 3060 2c20  `, _depth_=`0`, 
+0002aba0: 5c2a 5c2a 5f6b 7761 7267 735f 290a 0a49  \*\*_kwargs_)..I
+0002abb0: 6620 5f6b 6572 6e65 6c5f 3d60 4661 6c73  f _kernel_=`Fals
+0002abc0: 6560 2028 6465 6661 756c 7429 2c20 656d  e` (default), em
+0002abd0: 6265 6473 2061 2043 6f63 6f6e 7574 204a  beds a Coconut J
+0002abe0: 7570 7974 6572 2063 6f6e 736f 6c65 2069  upyter console i
+0002abf0: 6e69 7469 616c 697a 6564 2066 726f 6d20  nitialized from 
+0002ac00: 7468 6520 6375 7272 656e 7420 6c6f 6361  the current loca
+0002ac10: 6c20 6e61 6d65 7370 6163 652e 2049 6620  l namespace. If 
+0002ac20: 5f6b 6572 6e65 6c5f 3d60 5472 7565 602c  _kernel_=`True`,
+0002ac30: 206c 6175 6e63 6865 7320 6120 436f 636f   launches a Coco
+0002ac40: 6e75 7420 4a75 7079 7465 7220 6b65 726e  nut Jupyter kern
+0002ac50: 656c 2069 6e69 7469 616c 697a 6564 2066  el initialized f
+0002ac60: 726f 6d20 7468 6520 6c6f 6361 6c20 6e61  rom the local na
+0002ac70: 6d65 7370 6163 6520 7468 6174 2063 616e  mespace that can
+0002ac80: 2074 6865 6e20 6265 2061 7474 6163 6865   then be attache
+0002ac90: 6420 746f 2e20 5468 6520 5f64 6570 7468  d to. The _depth
+0002aca0: 5f20 696e 6469 6361 7465 7320 686f 7720  _ indicates how 
+0002acb0: 6d61 6e79 2061 6464 6974 696f 6e61 6c20  many additional 
+0002acc0: 6361 6c6c 2066 7261 6d65 7320 746f 2069  call frames to i
+0002acd0: 676e 6f72 652e 205f 6b77 6172 6773 5f20  gnore. _kwargs_ 
+0002ace0: 6172 6520 6173 2069 6e20 5b49 5079 7468  are as in [IPyth
+0002acf0: 6f6e 2e65 6d62 6564 5d28 6874 7470 733a  on.embed](https:
+0002ad00: 2f2f 6970 7974 686f 6e2e 7265 6164 7468  //ipython.readth
+0002ad10: 6564 6f63 732e 696f 2f65 6e2f 7374 6162  edocs.io/en/stab
+0002ad20: 6c65 2f61 7069 2f67 656e 6572 6174 6564  le/api/generated
+0002ad30: 2f49 5079 7468 6f6e 2e74 6572 6d69 6e61  /IPython.termina
+0002ad40: 6c2e 656d 6265 642e 6874 6d6c 2349 5079  l.embed.html#IPy
+0002ad50: 7468 6f6e 2e74 6572 6d69 6e61 6c2e 656d  thon.terminal.em
+0002ad60: 6265 642e 656d 6265 6429 206f 7220 5b49  bed.embed) or [I
+0002ad70: 5079 7468 6f6e 2e65 6d62 6564 5f6b 6572  Python.embed_ker
+0002ad80: 6e65 6c5d 2868 7474 7073 3a2f 2f69 7079  nel](https://ipy
+0002ad90: 7468 6f6e 2e72 6561 6474 6865 646f 6373  thon.readthedocs
+0002ada0: 2e69 6f2f 656e 2f73 7461 626c 652f 6170  .io/en/stable/ap
+0002adb0: 692f 6765 6e65 7261 7465 642f 4950 7974  i/generated/IPyt
+0002adc0: 686f 6e2e 6874 6d6c 2349 5079 7468 6f6e  hon.html#IPython
+0002add0: 2e65 6d62 6564 5f6b 6572 6e65 6c29 2062  .embed_kernel) b
+0002ade0: 6173 6564 206f 6e20 5f6b 6572 6e65 6c5f  ased on _kernel_
+0002adf0: 2e0a 0a52 6563 6f6d 6d65 6e64 6564 2075  ...Recommended u
+0002ae00: 7361 6765 2069 7320 6173 2061 2064 6562  sage is as a deb
+0002ae10: 7567 6769 6e67 2074 6f6f 6c2c 2077 6865  ugging tool, whe
+0002ae20: 7265 2074 6865 2063 6f64 6520 6066 726f  re the code `fro
+0002ae30: 6d20 636f 636f 6e75 7420 696d 706f 7274  m coconut import
+0002ae40: 2065 6d62 6564 3b20 656d 6265 6428 2960   embed; embed()`
+0002ae50: 2063 616e 2062 6520 696e 7365 7274 6564   can be inserted
+0002ae60: 2074 6f20 6c61 756e 6368 2061 6e20 696e   to launch an in
+0002ae70: 7465 7261 6374 6976 6520 436f 636f 6e75  teractive Coconu
+0002ae80: 7420 7368 656c 6c20 696e 6974 6961 6c69  t shell initiali
+0002ae90: 7a65 6420 6672 6f6d 2074 6861 7420 706f  zed from that po
+0002aea0: 696e 742e 0a0a 2323 2320 4175 746f 6d61  int...### Automa
+0002aeb0: 7469 6320 436f 6d70 696c 6174 696f 6e0a  tic Compilation.
+0002aec0: 0a49 6620 796f 7520 646f 6e27 7420 6361  .If you don't ca
+0002aed0: 7265 2061 626f 7574 2074 6865 2065 7861  re about the exa
+0002aee0: 6374 2063 6f6d 7069 6c61 7469 6f6e 2070  ct compilation p
+0002aef0: 6172 616d 6574 6572 7320 796f 7520 7761  arameters you wa
+0002af00: 6e74 2074 6f20 7573 652c 2061 7574 6f6d  nt to use, autom
+0002af10: 6174 6963 2063 6f6d 7069 6c61 7469 6f6e  atic compilation
+0002af20: 206c 6574 7320 436f 636f 6e75 7420 7461   lets Coconut ta
+0002af30: 6b65 2063 6172 6520 6f66 2065 7665 7279  ke care of every
+0002af40: 7468 696e 6720 666f 7220 796f 752e 2041  thing for you. A
+0002af50: 7574 6f6d 6174 6963 2063 6f6d 7069 6c61  utomatic compila
+0002af60: 7469 6f6e 2063 616e 2062 6520 656e 6162  tion can be enab
+0002af70: 6c65 6420 6569 7468 6572 2062 7920 696d  led either by im
+0002af80: 706f 7274 696e 6720 5b60 636f 636f 6e75  porting [`coconu
+0002af90: 742e 636f 6e76 656e 6965 6e63 6560 5d28  t.convenience`](
+0002afa0: 2363 6f63 6f6e 7574 2d63 6f6e 7665 6e69  #coconut-conveni
+0002afb0: 656e 6365 2920 6265 666f 7265 2079 6f75  ence) before you
+0002afc0: 2069 6d70 6f72 7420 616e 7974 6869 6e67   import anything
+0002afd0: 2065 6c73 652c 206f 7220 6279 2072 756e   else, or by run
+0002afe0: 6e69 6e67 2060 636f 636f 6e75 7420 2d2d  ning `coconut --
+0002aff0: 7369 7465 2d69 6e73 7461 6c6c 602e 204f  site-install`. O
+0002b000: 6e63 6520 6175 746f 6d61 7469 6320 636f  nce automatic co
+0002b010: 6d70 696c 6174 696f 6e20 6973 2065 6e61  mpilation is ena
+0002b020: 626c 6564 2c20 436f 636f 6e75 7420 7769  bled, Coconut wi
+0002b030: 6c6c 2063 6865 636b 2065 6163 6820 6f66  ll check each of
+0002b040: 2079 6f75 7220 696d 706f 7274 7320 746f   your imports to
+0002b050: 2073 6565 2069 6620 796f 7520 6172 6520   see if you are 
+0002b060: 6174 7465 6d70 7469 6e67 2074 6f20 696d  attempting to im
+0002b070: 706f 7274 2061 2060 2e63 6f63 6f60 2066  port a `.coco` f
+0002b080: 696c 6520 616e 642c 2069 6620 736f 2c20  ile and, if so, 
+0002b090: 6175 746f 6d61 7469 6361 6c6c 7920 636f  automatically co
+0002b0a0: 6d70 696c 6520 6974 2066 6f72 2079 6f75  mpile it for you
+0002b0b0: 2e20 4e6f 7465 2074 6861 742c 2066 6f72  . Note that, for
+0002b0c0: 2043 6f63 6f6e 7574 2074 6f20 6b6e 6f77   Coconut to know
+0002b0d0: 2077 6861 7420 6669 6c65 2079 6f75 2061   what file you a
+0002b0e0: 7265 2074 7279 696e 6720 746f 2069 6d70  re trying to imp
+0002b0f0: 6f72 742c 2069 7420 7769 6c6c 206e 6565  ort, it will nee
+0002b100: 6420 746f 2062 6520 6163 6365 7373 6962  d to be accessib
+0002b110: 6c65 2076 6961 2060 7379 732e 7061 7468  le via `sys.path
+0002b120: 602c 206a 7573 7420 6c69 6b65 2061 206e  `, just like a n
+0002b130: 6f72 6d61 6c20 696d 706f 7274 2e0a 0a41  ormal import...A
+0002b140: 7574 6f6d 6174 6963 2063 6f6d 7069 6c61  utomatic compila
+0002b150: 7469 6f6e 2061 6c77 6179 7320 636f 6d70  tion always comp
+0002b160: 696c 6573 206d 6f64 756c 6573 2061 6e64  iles modules and
+0002b170: 2070 6163 6b61 6765 7320 696e 2d70 6c61   packages in-pla
+0002b180: 6365 2c20 616e 6420 616c 7761 7973 2075  ce, and always u
+0002b190: 7365 7320 602d 2d74 6172 6765 7420 7379  ses `--target sy
+0002b1a0: 7360 2e20 4175 746f 6d61 7469 6320 636f  s`. Automatic co
+0002b1b0: 6d70 696c 6174 696f 6e20 6973 2061 6c77  mpilation is alw
+0002b1c0: 6179 7320 6176 6169 6c61 626c 6520 696e  ays available in
+0002b1d0: 2074 6865 2043 6f63 6f6e 7574 2069 6e74   the Coconut int
+0002b1e0: 6572 7072 6574 6572 2c20 616e 642c 2069  erpreter, and, i
+0002b1f0: 6620 7573 696e 6720 7468 6520 436f 636f  f using the Coco
+0002b200: 6e75 7420 696e 7465 7270 7265 7465 722c  nut interpreter,
+0002b210: 2061 2060 7265 6c6f 6164 6020 6275 696c   a `reload` buil
+0002b220: 742d 696e 2069 7320 7072 6f76 6964 6564  t-in is provided
+0002b230: 2074 6f20 6561 7369 6c79 2072 656c 6f61   to easily reloa
+0002b240: 6420 696d 706f 7274 6564 206d 6f64 756c  d imported modul
+0002b250: 6573 2e20 4164 6469 7469 6f6e 616c 6c79  es. Additionally
+0002b260: 2c20 7468 6520 696e 7465 7270 7265 7465  , the interprete
+0002b270: 7220 616c 7761 7973 2061 6c6c 6f77 7320  r always allows 
+0002b280: 696d 706f 7274 696e 6720 6672 6f6d 2074  importing from t
+0002b290: 6865 2063 7572 7265 6e74 2077 6f72 6b69  he current worki
+0002b2a0: 6e67 2064 6972 6563 746f 7279 2c20 6c65  ng directory, le
+0002b2b0: 7474 696e 6720 796f 7520 6561 7369 6c79  tting you easily
+0002b2c0: 2063 6f6d 7069 6c65 2061 6e64 2070 6c61   compile and pla
+0002b2d0: 7920 6172 6f75 6e64 2077 6974 6820 6120  y around with a 
+0002b2e0: 602e 636f 636f 6020 6669 6c65 2073 696d  `.coco` file sim
+0002b2f0: 706c 7920 6279 2072 756e 6e69 6e67 2074  ply by running t
+0002b300: 6865 2043 6f63 6f6e 7574 2069 6e74 6572  he Coconut inter
+0002b310: 7072 6574 6572 2061 6e64 2069 6d70 6f72  preter and impor
+0002b320: 7469 6e67 2069 742e 0a0a 2323 2320 436f  ting it...### Co
+0002b330: 636f 6e75 7420 456e 636f 6469 6e67 0a0a  conut Encoding..
+0002b340: 5768 696c 6520 6175 746f 6d61 7469 6320  While automatic 
+0002b350: 636f 6d70 696c 6174 696f 6e20 6973 2074  compilation is t
+0002b360: 6865 2070 7265 6665 7272 6564 206d 6574  he preferred met
+0002b370: 686f 6420 666f 7220 6479 6e61 6d69 6361  hod for dynamica
+0002b380: 6c6c 7920 636f 6d70 696c 696e 6720 436f  lly compiling Co
+0002b390: 636f 6e75 7420 6669 6c65 732c 2061 7320  conut files, as 
+0002b3a0: 6974 2063 6163 6865 7320 7468 6520 636f  it caches the co
+0002b3b0: 6d70 696c 6564 2063 6f64 6520 6173 2061  mpiled code as a
+0002b3c0: 2060 2e70 7960 2066 696c 6520 746f 2070   `.py` file to p
+0002b3d0: 7265 7665 6e74 2072 6563 6f6d 7069 6c61  revent recompila
+0002b3e0: 7469 6f6e 2c20 436f 636f 6e75 7420 616c  tion, Coconut al
+0002b3f0: 736f 2073 7570 706f 7274 7320 6120 7370  so supports a sp
+0002b400: 6563 6961 6c0a 6060 6063 6f63 6f6e 7574  ecial.```coconut
+0002b410: 0a23 2063 6f64 696e 673a 2063 6f63 6f6e  .# coding: cocon
+0002b420: 7574 0a60 6060 0a64 6563 6c61 7261 7469  ut.```.declarati
+0002b430: 6f6e 2077 6869 6368 2063 616e 2062 6520  on which can be 
+0002b440: 6164 6465 6420 746f 2060 2e70 7960 2066  added to `.py` f
+0002b450: 696c 6573 2074 6f20 6861 7665 2074 6865  iles to have the
+0002b460: 6d20 7472 6561 7465 6420 6173 2043 6f63  m treated as Coc
+0002b470: 6f6e 7574 2066 696c 6573 2069 6e73 7465  onut files inste
+0002b480: 6164 2e20 546f 2075 7365 2073 7563 6820  ad. To use such 
+0002b490: 6120 636f 6469 6e67 2064 6563 6c61 7261  a coding declara
+0002b4a0: 7469 6f6e 2c20 796f 7527 6c6c 206e 6565  tion, you'll nee
+0002b4b0: 6420 746f 2065 6974 6865 7220 7275 6e20  d to either run 
+0002b4c0: 6063 6f63 6f6e 7574 202d 2d73 6974 652d  `coconut --site-
+0002b4d0: 696e 7374 616c 6c60 206f 7220 6069 6d70  install` or `imp
+0002b4e0: 6f72 7420 636f 636f 6e75 742e 636f 6e76  ort coconut.conv
+0002b4f0: 656e 6965 6e63 6560 2061 7420 736f 6d65  enience` at some
+0002b500: 2070 6f69 6e74 2062 6566 6f72 6520 796f   point before yo
+0002b510: 7520 6669 7273 7420 6174 7465 6d70 7420  u first attempt 
+0002b520: 746f 2069 6d70 6f72 7420 6120 6669 6c65  to import a file
+0002b530: 2077 6974 6820 6120 6023 2063 6f64 696e   with a `# codin
+0002b540: 673a 2063 6f63 6f6e 7574 6020 6465 636c  g: coconut` decl
+0002b550: 6172 6174 696f 6e2e 204c 696b 6520 6175  aration. Like au
+0002b560: 746f 6d61 7469 6320 636f 6d70 696c 6174  tomatic compilat
+0002b570: 696f 6e2c 2063 6f6d 7069 6c61 7469 6f6e  ion, compilation
+0002b580: 2069 7320 616c 7761 7973 2064 6f6e 6520   is always done 
+0002b590: 7769 7468 2060 2d2d 7461 7267 6574 2073  with `--target s
+0002b5a0: 7973 6020 616e 6420 6973 2061 6c77 6179  ys` and is alway
+0002b5b0: 7320 6176 6169 6c61 626c 6520 6672 6f6d  s available from
+0002b5c0: 2074 6865 2043 6f63 6f6e 7574 2069 6e74   the Coconut int
+0002b5d0: 6572 7072 6574 6572 2e0a 0a23 2323 2060  erpreter...### `
+0002b5e0: 636f 636f 6e75 742e 636f 6e76 656e 6965  coconut.convenie
+0002b5f0: 6e63 6560 0a0a 496e 2061 6464 6974 696f  nce`..In additio
+0002b600: 6e20 746f 2065 6e61 626c 696e 6720 6175  n to enabling au
+0002b610: 746f 6d61 7469 6320 636f 6d70 696c 6174  tomatic compilat
+0002b620: 696f 6e2c 2060 636f 636f 6e75 742e 636f  ion, `coconut.co
+0002b630: 6e76 656e 6965 6e63 6560 2063 616e 2061  nvenience` can a
+0002b640: 6c73 6f20 6265 2075 7365 6420 746f 2063  lso be used to c
+0002b650: 616c 6c20 7468 6520 436f 636f 6e75 7420  all the Coconut 
+0002b660: 636f 6d70 696c 6572 2066 726f 6d20 636f  compiler from co
+0002b670: 6465 2069 6e73 7465 6164 206f 6620 6672  de instead of fr
+0002b680: 6f6d 2074 6865 2063 6f6d 6d61 6e64 206c  om the command l
+0002b690: 696e 652e 2053 6565 2062 656c 6f77 2066  ine. See below f
+0002b6a0: 6f72 2073 7065 6369 6669 6361 7469 6f6e  or specification
+0002b6b0: 7320 6f66 2074 6865 2064 6966 6665 7265  s of the differe
+0002b6c0: 6e74 2063 6f6e 7665 6e69 656e 6365 2066  nt convenience f
+0002b6d0: 756e 6374 696f 6e73 2e0a 0a23 2323 2320  unctions...#### 
+0002b6e0: 6067 6574 5f73 7461 7465 600a 0a2a 2a63  `get_state`..**c
+0002b6f0: 6f63 6f6e 7574 2e63 6f6e 7665 6e69 656e  oconut.convenien
+0002b700: 6365 2e67 6574 5c5f 7374 6174 652a 2a28  ce.get\_state**(
+0002b710: 5f73 7461 7465 5f3d 604e 6f6e 6560 290a  _state_=`None`).
+0002b720: 0a47 6574 7320 6120 7374 6174 6520 6f62  .Gets a state ob
+0002b730: 6a65 6374 2077 6869 6368 2073 746f 7265  ject which store
+0002b740: 7320 7468 6520 6375 7272 656e 7420 636f  s the current co
+0002b750: 6d70 696c 6174 696f 6e20 7061 7261 6d65  mpilation parame
+0002b760: 7465 7273 2e20 5374 6174 6520 6f62 6a65  ters. State obje
+0002b770: 6374 7320 6361 6e20 6265 2063 6f6e 6669  cts can be confi
+0002b780: 6775 7265 6420 7769 7468 205b 2a2a 7365  gured with [**se
+0002b790: 7475 702a 2a5d 2823 7365 7475 7029 206f  tup**](#setup) o
+0002b7a0: 7220 5b2a 2a63 6d64 2a2a 5d28 2363 6d64  r [**cmd**](#cmd
+0002b7b0: 2920 616e 6420 7468 656e 2075 7365 6420  ) and then used 
+0002b7c0: 696e 205b 2a2a 7061 7273 652a 2a5d 2823  in [**parse**](#
+0002b7d0: 7061 7273 6529 206f 7220 5b2a 2a63 6f63  parse) or [**coc
+0002b7e0: 6f6e 7574 5c5f 6576 616c 2a2a 5d28 2363  onut\_eval**](#c
+0002b7f0: 6f63 6f6e 7574 5f65 7661 6c29 2e0a 0a49  oconut_eval)...I
+0002b800: 6620 5f73 7461 7465 5f20 6973 2060 4e6f  f _state_ is `No
+0002b810: 6e65 602c 2067 6574 7320 6120 6e65 7720  ne`, gets a new 
+0002b820: 7374 6174 6520 6f62 6a65 6374 2c20 7768  state object, wh
+0002b830: 6572 6561 7320 6966 205f 7374 6174 655f  ereas if _state_
+0002b840: 2069 7320 6046 616c 7365 602c 2074 6865   is `False`, the
+0002b850: 2067 6c6f 6261 6c20 7374 6174 6520 6f62   global state ob
+0002b860: 6a65 6374 2069 7320 7265 7475 726e 6564  ject is returned
+0002b870: 2e0a 0a23 2323 2320 6070 6172 7365 600a  ...#### `parse`.
+0002b880: 0a2a 2a63 6f63 6f6e 7574 2e63 6f6e 7665  .**coconut.conve
+0002b890: 6e69 656e 6365 2e70 6172 7365 2a2a 285f  nience.parse**(_
+0002b8a0: 636f 6465 5f3d 6022 2260 2c20 5f6d 6f64  code_=`""`, _mod
+0002b8b0: 655f 3d60 2273 7973 2260 2c20 5f73 7461  e_=`"sys"`, _sta
+0002b8c0: 7465 5f3d 6046 616c 7365 602c 205f 6b65  te_=`False`, _ke
+0002b8d0: 6570 5c5f 696e 7465 726e 616c 5c5f 7374  ep\_internal\_st
+0002b8e0: 6174 655f 3d60 4e6f 6e65 6029 0a0a 4c69  ate_=`None`)..Li
+0002b8f0: 6b65 6c79 2074 6865 206d 6f73 7420 7573  kely the most us
+0002b900: 6566 756c 206f 6620 7468 6520 636f 6e76  eful of the conv
+0002b910: 656e 6965 6e63 6520 6675 6e63 7469 6f6e  enience function
+0002b920: 732c 2060 7061 7273 6560 2074 616b 6573  s, `parse` takes
+0002b930: 2043 6f63 6f6e 7574 2063 6f64 6520 6173   Coconut code as
+0002b940: 2069 6e70 7574 2061 6e64 206f 7574 7075   input and outpu
+0002b950: 7473 2074 6865 2065 7175 6976 616c 656e  ts the equivalen
+0002b960: 7420 636f 6d70 696c 6564 2050 7974 686f  t compiled Pytho
+0002b970: 6e20 636f 6465 2e20 5f6d 6f64 655f 2069  n code. _mode_ i
+0002b980: 7320 7573 6564 2074 6f20 696e 6469 6361  s used to indica
+0002b990: 7465 2074 6865 2063 6f6e 7465 7874 2066  te the context f
+0002b9a0: 6f72 2074 6865 2070 6172 7369 6e67 2061  or the parsing a
+0002b9b0: 6e64 205f 7374 6174 655f 2069 7320 7468  nd _state_ is th
+0002b9c0: 6520 7374 6174 6520 6f62 6a65 6374 2073  e state object s
+0002b9d0: 746f 7269 6e67 2074 6865 2063 6f6d 7069  toring the compi
+0002b9e0: 6c61 7469 6f6e 2070 6172 616d 6574 6572  lation parameter
+0002b9f0: 7320 746f 2075 7365 2061 7320 6f62 7461  s to use as obta
+0002ba00: 696e 6564 2066 726f 6d20 5b2a 2a67 6574  ined from [**get
+0002ba10: 5f73 7461 7465 2a2a 5d28 2367 6574 5f73  _state**](#get_s
+0002ba20: 7461 7465 2920 2869 6620 6046 616c 7365  tate) (if `False
+0002ba30: 602c 2075 7365 7320 7468 6520 676c 6f62  `, uses the glob
+0002ba40: 616c 2073 7461 7465 206f 626a 6563 7429  al state object)
+0002ba50: 2e20 5f6b 6565 705c 5f69 6e74 6572 6e61  . _keep\_interna
+0002ba60: 6c5c 5f73 7461 7465 5f20 6465 7465 726d  l\_state_ determ
+0002ba70: 696e 6573 2077 6865 7468 6572 2074 6865  ines whether the
+0002ba80: 2073 7461 7465 206f 626a 6563 7420 7769   state object wi
+0002ba90: 6c6c 206b 6565 7020 696e 7465 726e 616c  ll keep internal
+0002baa0: 2073 7461 7465 2028 7375 6368 2061 7320   state (such as 
+0002bab0: 7768 6174 205b 6375 7374 6f6d 206f 7065  what [custom ope
+0002bac0: 7261 746f 7273 5d28 2363 7573 746f 6d2d  rators](#custom-
+0002bad0: 6f70 6572 6174 6f72 7329 2068 6176 6520  operators) have 
+0002bae0: 6265 656e 2064 6563 6c61 7265 6429 e280  been declared)..
+0002baf0: 9469 6620 604e 6f6e 6560 2c20 696e 7465  .if `None`, inte
+0002bb00: 726e 616c 2073 7461 7465 2077 696c 6c20  rnal state will 
+0002bb10: 6265 206b 6570 7420 6966 6620 796f 7520  be kept iff you 
+0002bb20: 6172 6520 6e6f 7420 7573 696e 6720 7468  are not using th
+0002bb30: 6520 676c 6f62 616c 205f 7374 6174 655f  e global _state_
+0002bb40: 2e0a 0a49 6620 5f63 6f64 655f 2069 7320  ...If _code_ is 
+0002bb50: 6e6f 7420 7061 7373 6564 2c20 6070 6172  not passed, `par
+0002bb60: 7365 6020 7769 6c6c 206f 7574 7075 7420  se` will output 
+0002bb70: 6a75 7374 2074 6865 2067 6976 656e 205f  just the given _
+0002bb80: 6d6f 6465 5f27 7320 6865 6164 6572 2c20  mode_'s header, 
+0002bb90: 7768 6963 6820 6361 6e20 6265 2065 7865  which can be exe
+0002bba0: 6375 7465 6420 746f 2073 6574 2075 7020  cuted to set up 
+0002bbb0: 616e 2065 7865 6375 7469 6f6e 2065 6e76  an execution env
+0002bbc0: 6972 6f6e 6d65 6e74 2069 6e20 7768 6963  ironment in whic
+0002bbd0: 6820 6675 7475 7265 2063 6f64 6520 6361  h future code ca
+0002bbe0: 6e20 6265 2070 6172 7365 6420 616e 6420  n be parsed and 
+0002bbf0: 6578 6563 7574 6564 2077 6974 686f 7574  executed without
+0002bc00: 2061 2068 6561 6465 722e 0a0a 4561 6368   a header...Each
+0002bc10: 205f 6d6f 6465 5f20 6861 7320 7477 6f20   _mode_ has two 
+0002bc20: 636f 6d70 6f6e 656e 7473 3a20 7768 6174  components: what
+0002bc30: 2070 6172 7365 7220 6974 2075 7365 732c   parser it uses,
+0002bc40: 2061 6e64 2077 6861 7420 6865 6164 6572   and what header
+0002bc50: 2069 7420 7072 6570 656e 6473 2e20 5468   it prepends. Th
+0002bc60: 6520 7061 7273 6572 2064 6574 6572 6d69  e parser determi
+0002bc70: 6e65 7320 7768 6174 2043 6f63 6f6e 7574  nes what Coconut
+0002bc80: 2063 6f64 6520 6973 2061 6c6c 6f77 6564   code is allowed
+0002bc90: 2061 7320 696e 7075 742c 2061 6e64 2074   as input, and t
+0002bca0: 6865 2068 6561 6465 7220 6465 7465 726d  he header determ
+0002bcb0: 696e 6573 2068 6f77 2074 6865 2063 6f6d  ines how the com
+0002bcc0: 7069 6c65 6420 5079 7468 6f6e 2063 616e  piled Python can
+0002bcd0: 2062 6520 7573 6564 2e20 506f 7373 6962   be used. Possib
+0002bce0: 6c65 2076 616c 7565 7320 6f66 205f 6d6f  le values of _mo
+0002bcf0: 6465 5f20 6172 653a 0a0a 2d20 6022 7379  de_ are:..- `"sy
+0002bd00: 7322 603a 2028 7468 6520 6465 6661 756c  s"`: (the defaul
+0002bd10: 7429 0a20 2020 202b 2070 6172 7365 723a  t).    + parser:
+0002bd20: 2066 696c 650a 2020 2020 2020 2020 2a20   file.        * 
+0002bd30: 5468 6520 6669 6c65 2070 6172 7365 7220  The file parser 
+0002bd40: 6361 6e20 7061 7273 6520 616e 7920 436f  can parse any Co
+0002bd50: 636f 6e75 7420 636f 6465 2e0a 2020 2020  conut code..    
+0002bd60: 2b20 6865 6164 6572 3a20 7379 730a 2020  + header: sys.  
+0002bd70: 2020 2020 2020 2a20 5468 6973 2068 6561        * This hea
+0002bd80: 6465 7220 696d 706f 7274 7320 5b60 636f  der imports [`co
+0002bd90: 636f 6e75 742e 5f5f 636f 636f 6e75 745f  conut.__coconut_
+0002bda0: 5f60 5d28 2363 6f63 6f6e 7574 2d63 6f63  _`](#coconut-coc
+0002bdb0: 6f6e 7574 2920 746f 2061 6363 6573 7320  onut) to access 
+0002bdc0: 7468 6520 6e65 6365 7373 6172 7920 436f  the necessary Co
+0002bdd0: 636f 6e75 7420 6f62 6a65 6374 732e 0a2d  conut objects..-
+0002bde0: 2060 2265 7865 6322 603a 0a20 2020 202b   `"exec"`:.    +
+0002bdf0: 2070 6172 7365 723a 2066 696c 650a 2020   parser: file.  
+0002be00: 2020 2b20 6865 6164 6572 3a20 6578 6563    + header: exec
+0002be10: 0a20 2020 2020 2020 202a 2057 6865 6e20  .        * When 
+0002be20: 7061 7373 6564 2074 6f20 6065 7865 6360  passed to `exec`
+0002be30: 2061 7420 7468 6520 676c 6f62 616c 206c   at the global l
+0002be40: 6576 656c 2c20 7468 6973 2068 6561 6465  evel, this heade
+0002be50: 7220 7769 6c6c 2063 7265 6174 6520 616c  r will create al
+0002be60: 6c20 7468 6520 6e65 6365 7373 6172 7920  l the necessary 
+0002be70: 436f 636f 6e75 7420 6f62 6a65 6374 7320  Coconut objects 
+0002be80: 6974 7365 6c66 2069 6e73 7465 6164 206f  itself instead o
+0002be90: 6620 696d 706f 7274 696e 6720 7468 656d  f importing them
+0002bea0: 2e0a 2d20 6022 6669 6c65 2260 3a0a 2020  ..- `"file"`:.  
+0002beb0: 2020 2b20 7061 7273 6572 3a20 6669 6c65    + parser: file
+0002bec0: 0a20 2020 202b 2068 6561 6465 723a 2066  .    + header: f
+0002bed0: 696c 650a 2020 2020 2020 2020 2a20 5468  ile.        * Th
+0002bee0: 6973 2068 6561 6465 7220 6973 206d 6561  is header is mea
+0002bef0: 6e74 2074 6f20 6265 2077 7269 7474 656e  nt to be written
+0002bf00: 2074 6f20 6120 602d 2d73 7461 6e64 616c   to a `--standal
+0002bf10: 6f6e 6560 2066 696c 6520 616e 6420 7368  one` file and sh
+0002bf20: 6f75 6c64 206e 6f74 2062 6520 7061 7373  ould not be pass
+0002bf30: 6564 2074 6f20 6065 7865 6360 2e0a 2d20  ed to `exec`..- 
+0002bf40: 6022 7061 636b 6167 6522 603a 0a20 2020  `"package"`:.   
+0002bf50: 202b 2070 6172 7365 723a 2066 696c 650a   + parser: file.
+0002bf60: 2020 2020 2b20 6865 6164 6572 3a20 7061      + header: pa
+0002bf70: 636b 6167 650a 2020 2020 2020 2020 2a20  ckage.        * 
+0002bf80: 5468 6973 2068 6561 6465 7220 6973 206d  This header is m
+0002bf90: 6561 6e74 2074 6f20 6265 2077 7269 7474  eant to be writt
+0002bfa0: 656e 2074 6f20 6120 602d 2d70 6163 6b61  en to a `--packa
+0002bfb0: 6765 6020 6669 6c65 2061 6e64 2073 686f  ge` file and sho
+0002bfc0: 756c 6420 6e6f 7420 6265 2070 6173 7365  uld not be passe
+0002bfd0: 6420 746f 2060 6578 6563 602e 0a2d 2060  d to `exec`..- `
+0002bfe0: 2262 6c6f 636b 2260 3a0a 2020 2020 2b20  "block"`:.    + 
+0002bff0: 7061 7273 6572 3a20 6669 6c65 0a20 2020  parser: file.   
+0002c000: 202b 2068 6561 6465 723a 206e 6f6e 650a   + header: none.
+0002c010: 2020 2020 2020 2020 2a20 4e6f 2068 6561          * No hea
+0002c020: 6465 7220 6973 2069 6e63 6c75 6465 642c  der is included,
+0002c030: 2074 6875 7320 7468 6973 2063 616e 206f   thus this can o
+0002c040: 6e6c 7920 6265 2070 6173 7365 6420 746f  nly be passed to
+0002c050: 2060 6578 6563 6020 6966 2063 6f64 6520   `exec` if code 
+0002c060: 7769 7468 2061 2068 6561 6465 7220 6861  with a header ha
+0002c070: 7320 616c 7265 6164 7920 6265 656e 2065  s already been e
+0002c080: 7865 6375 7465 6420 6174 2074 6865 2067  xecuted at the g
+0002c090: 6c6f 6261 6c20 6c65 7665 6c2e 0a2d 2060  lobal level..- `
+0002c0a0: 2273 696e 676c 6522 603a 0a20 2020 202b  "single"`:.    +
+0002c0b0: 2070 6172 7365 723a 2073 696e 676c 650a   parser: single.
+0002c0c0: 2020 2020 2020 2020 2a20 4361 6e20 6f6e          * Can on
+0002c0d0: 6c79 2070 6172 7365 206f 6e65 206c 696e  ly parse one lin
+0002c0e0: 6520 6f66 2043 6f63 6f6e 7574 2063 6f64  e of Coconut cod
+0002c0f0: 652e 0a20 2020 202b 2068 6561 6465 723a  e..    + header:
+0002c100: 206e 6f6e 650a 2d20 6022 6576 616c 2260   none.- `"eval"`
+0002c110: 3a0a 2020 2020 2b20 7061 7273 6572 3a20  :.    + parser: 
+0002c120: 6576 616c 0a20 2020 2020 2020 202a 2043  eval.        * C
+0002c130: 616e 206f 6e6c 7920 7061 7273 6520 6120  an only parse a 
+0002c140: 436f 636f 6e75 7420 6578 7072 6573 7369  Coconut expressi
+0002c150: 6f6e 2c20 6e6f 7420 6120 7374 6174 656d  on, not a statem
+0002c160: 656e 742e 0a20 2020 202b 2068 6561 6465  ent..    + heade
+0002c170: 723a 206e 6f6e 650a 2d20 6022 6c65 6e69  r: none.- `"leni
+0002c180: 656e 7422 603a 0a20 2020 202b 2070 6172  ent"`:.    + par
+0002c190: 7365 723a 206c 656e 6965 6e74 0a20 2020  ser: lenient.   
+0002c1a0: 2020 2020 202a 2043 616e 2070 6172 7365       * Can parse
+0002c1b0: 2061 6e79 2043 6f63 6f6e 7574 2063 6f64   any Coconut cod
+0002c1c0: 652c 2061 6c6c 6f77 7320 6c65 6164 696e  e, allows leadin
+0002c1d0: 6720 7768 6974 6573 7061 6365 2c20 616e  g whitespace, an
+0002c1e0: 6420 6861 7320 6e6f 2074 7261 696c 696e  d has no trailin
+0002c1f0: 6720 6e65 776c 696e 652e 0a20 2020 202b  g newline..    +
+0002c200: 2068 6561 6465 723a 206e 6f6e 650a 2d20   header: none.- 
+0002c210: 6022 786f 6e73 6822 603a 0a20 2020 202b  `"xonsh"`:.    +
+0002c220: 2070 6172 7365 723a 2078 6f6e 7368 0a20   parser: xonsh. 
+0002c230: 2020 2020 2020 202a 2050 6172 7365 7320         * Parses 
+0002c240: 436f 636f 6e75 7420 5b60 786f 6e73 6860  Coconut [`xonsh`
+0002c250: 5d28 6874 7470 733a 2f2f 786f 6e2e 7368  ](https://xon.sh
+0002c260: 2920 636f 6465 2066 6f72 2075 7365 2069  ) code for use i
+0002c270: 6e20 5b43 6f63 6f6e 7574 2773 2060 786f  n [Coconut's `xo
+0002c280: 6e73 6860 2073 7570 706f 7274 5d28 2378  nsh` support](#x
+0002c290: 6f6e 7368 2d73 7570 706f 7274 292e 0a20  onsh-support).. 
+0002c2a0: 2020 202b 2068 6561 6465 723a 206e 6f6e     + header: non
+0002c2b0: 650a 0a23 2323 2323 2045 7861 6d70 6c65  e..##### Example
+0002c2c0: 0a0a 6060 6063 6f63 6f6e 7574 5f70 7974  ..```coconut_pyt
+0002c2d0: 686f 6e0a 6672 6f6d 2063 6f63 6f6e 7574  hon.from coconut
+0002c2e0: 2e63 6f6e 7665 6e69 656e 6365 2069 6d70  .convenience imp
+0002c2f0: 6f72 7420 7061 7273 650a 6578 6563 2870  ort parse.exec(p
+0002c300: 6172 7365 2829 290a 7768 696c 6520 5472  arse()).while Tr
+0002c310: 7565 3a0a 2020 2020 6578 6563 2870 6172  ue:.    exec(par
+0002c320: 7365 2869 6e70 7574 2829 2c20 6d6f 6465  se(input(), mode
+0002c330: 3d22 626c 6f63 6b22 2929 0a60 6060 0a0a  ="block")).```..
+0002c340: 2323 2323 2060 7365 7475 7060 0a0a 2a2a  #### `setup`..**
+0002c350: 636f 636f 6e75 742e 636f 6e76 656e 6965  coconut.convenie
+0002c360: 6e63 652e 7365 7475 702a 2a28 5f74 6172  nce.setup**(_tar
+0002c370: 6765 745f 3d60 4e6f 6e65 602c 205f 7374  get_=`None`, _st
+0002c380: 7269 6374 5f3d 6046 616c 7365 602c 205f  rict_=`False`, _
+0002c390: 6d69 6e69 6679 5f3d 6046 616c 7365 602c  minify_=`False`,
+0002c3a0: 205f 6c69 6e65 5c5f 6e75 6d62 6572 735f   _line\_numbers_
+0002c3b0: 3d60 4661 6c73 6560 2c20 5f6b 6565 705c  =`False`, _keep\
+0002c3c0: 5f6c 696e 6573 5f3d 6046 616c 7365 602c  _lines_=`False`,
+0002c3d0: 205f 6e6f 5c5f 7463 6f5f 3d60 4661 6c73   _no\_tco_=`Fals
+0002c3e0: 6560 2c20 5f6e 6f5c 5f77 7261 705f 3d60  e`, _no\_wrap_=`
+0002c3f0: 4661 6c73 6560 2c20 2a2c 205f 7374 6174  False`, *, _stat
+0002c400: 655f 3d60 4661 6c73 6560 290a 0a60 7365  e_=`False`)..`se
+0002c410: 7475 7060 2063 616e 2062 6520 7573 6564  tup` can be used
+0002c420: 2074 6f20 7365 7420 7570 2074 6865 2067   to set up the g
+0002c430: 6976 656e 2073 7461 7465 206f 626a 6563  iven state objec
+0002c440: 7420 7769 7468 2074 6865 2067 6976 656e  t with the given
+0002c450: 2063 6f6d 6d61 6e64 2d6c 696e 6520 666c   command-line fl
+0002c460: 6167 732e 2049 6620 5f73 7461 7465 5f20  ags. If _state_ 
+0002c470: 6973 2060 4661 6c73 6560 2c20 7468 6520  is `False`, the 
+0002c480: 676c 6f62 616c 2073 7461 7465 206f 626a  global state obj
+0002c490: 6563 7420 6973 2075 7365 642e 0a0a 5468  ect is used...Th
+0002c4a0: 6520 706f 7373 6962 6c65 2076 616c 7565  e possible value
+0002c4b0: 7320 666f 7220 6561 6368 2066 6c61 6720  s for each flag 
+0002c4c0: 6172 6775 6d65 6e74 2061 7265 3a0a 0a2d  argument are:..-
+0002c4d0: 205f 7461 7267 6574 5f3a 2060 4e6f 6e65   _target_: `None
+0002c4e0: 6020 2864 6566 6175 6c74 292c 206f 7220  ` (default), or 
+0002c4f0: 616e 7920 5b61 6c6c 6f77 6162 6c65 2074  any [allowable t
+0002c500: 6172 6765 745d 2823 616c 6c6f 7761 626c  arget](#allowabl
+0002c510: 652d 7461 7267 6574 7329 0a2d 205f 7374  e-targets).- _st
+0002c520: 7269 6374 5f3a 2060 4661 6c73 6560 2028  rict_: `False` (
+0002c530: 6465 6661 756c 7429 206f 7220 6054 7275  default) or `Tru
+0002c540: 6560 0a2d 205f 6d69 6e69 6679 5f3a 2060  e`.- _minify_: `
+0002c550: 4661 6c73 6560 2028 6465 6661 756c 7429  False` (default)
+0002c560: 206f 7220 6054 7275 6560 0a2d 205f 6c69   or `True`.- _li
+0002c570: 6e65 5c5f 6e75 6d62 6572 735f 3a20 6046  ne\_numbers_: `F
+0002c580: 616c 7365 6020 2864 6566 6175 6c74 2920  alse` (default) 
+0002c590: 6f72 2060 5472 7565 600a 2d20 5f6b 6565  or `True`.- _kee
+0002c5a0: 705c 5f6c 696e 6573 5f3a 2060 4661 6c73  p\_lines_: `Fals
+0002c5b0: 6560 2028 6465 6661 756c 7429 206f 7220  e` (default) or 
+0002c5c0: 6054 7275 6560 0a2d 205f 6e6f 5c5f 7463  `True`.- _no\_tc
+0002c5d0: 6f5f 3a20 6046 616c 7365 6020 2864 6566  o_: `False` (def
+0002c5e0: 6175 6c74 2920 6f72 2060 5472 7565 600a  ault) or `True`.
+0002c5f0: 2d20 5f6e 6f5c 5f77 7261 705f 3a20 6046  - _no\_wrap_: `F
 0002c600: 616c 7365 6020 2864 6566 6175 6c74 2920  alse` (default) 
-0002c610: 6f72 2060 5472 7565 600a 2d20 5f6e 6f5c  or `True`.- _no\
-0002c620: 5f74 636f 5f3a 2060 4661 6c73 6560 2028  _tco_: `False` (
-0002c630: 6465 6661 756c 7429 206f 7220 6054 7275  default) or `Tru
-0002c640: 6560 0a2d 205f 6e6f 5c5f 7772 6170 5f3a  e`.- _no\_wrap_:
-0002c650: 2060 4661 6c73 6560 2028 6465 6661 756c   `False` (defaul
-0002c660: 7429 206f 7220 6054 7275 6560 0a0a 2323  t) or `True`..##
-0002c670: 2323 2060 636d 6460 0a0a 2a2a 636f 636f  ## `cmd`..**coco
-0002c680: 6e75 742e 636f 6e76 656e 6965 6e63 652e  nut.convenience.
-0002c690: 636d 642a 2a28 5f61 7267 735f 3d60 4e6f  cmd**(_args_=`No
-0002c6a0: 6e65 602c 202a 2c20 5f61 7267 765f 3d60  ne`, *, _argv_=`
-0002c6b0: 4e6f 6e65 602c 205f 696e 7465 7261 6374  None`, _interact
-0002c6c0: 5f3d 6046 616c 7365 602c 205f 6465 6661  _=`False`, _defa
-0002c6d0: 756c 745c 5f74 6172 6765 745f 3d60 4e6f  ult\_target_=`No
-0002c6e0: 6e65 602c 205f 7374 6174 655f 3d60 4661  ne`, _state_=`Fa
-0002c6f0: 6c73 6560 290a 0a45 7865 6375 7465 7320  lse`)..Executes 
-0002c700: 7468 6520 6769 7665 6e20 5f61 7267 735f  the given _args_
-0002c710: 2061 7320 6966 2074 6865 7920 7765 7265   as if they were
-0002c720: 2066 6564 2074 6f20 6063 6f63 6f6e 7574   fed to `coconut
-0002c730: 6020 6f6e 2074 6865 2063 6f6d 6d61 6e64  ` on the command
-0002c740: 2d6c 696e 652c 2077 6974 6820 7468 6520  -line, with the 
-0002c750: 6578 6365 7074 696f 6e20 7468 6174 2075  exception that u
-0002c760: 6e6c 6573 7320 5f69 6e74 6572 6163 745f  nless _interact_
-0002c770: 2069 7320 7472 7565 206f 7220 602d 6960   is true or `-i`
-0002c780: 2069 7320 7061 7373 6564 2c20 7468 6520   is passed, the 
-0002c790: 696e 7465 7270 7265 7465 7220 7769 6c6c  interpreter will
-0002c7a0: 206e 6f74 2062 6520 7374 6172 7465 642e   not be started.
-0002c7b0: 2041 6464 6974 696f 6e61 6c6c 792c 205f   Additionally, _
-0002c7c0: 6172 6776 5f20 6361 6e20 6265 2075 7365  argv_ can be use
-0002c7d0: 6420 746f 2070 6173 7320 696e 2061 7267  d to pass in arg
-0002c7e0: 756d 656e 7473 2061 7320 696e 2060 2d2d  uments as in `--
-0002c7f0: 6172 6776 6020 616e 6420 5f64 6566 6175  argv` and _defau
-0002c800: 6c74 5c5f 7461 7267 6574 5f20 6361 6e20  lt\_target_ can 
-0002c810: 6265 2075 7365 6420 746f 2073 6574 2074  be used to set t
-0002c820: 6865 2064 6566 6175 6c74 2060 2d2d 7461  he default `--ta
-0002c830: 7267 6574 602e 0a0a 4861 7320 7468 6520  rget`...Has the 
-0002c840: 7361 6d65 2065 6666 6563 7420 6f66 2073  same effect of s
-0002c850: 6574 7469 6e67 2074 6865 2063 6f6d 6d61  etting the comma
-0002c860: 6e64 2d6c 696e 6520 666c 6167 7320 6f6e  nd-line flags on
-0002c870: 2074 6865 2067 6976 656e 205f 7374 6174   the given _stat
-0002c880: 655f 206f 626a 6563 7420 6173 2060 7365  e_ object as `se
-0002c890: 7475 7060 2028 7769 7468 2074 6865 2067  tup` (with the g
-0002c8a0: 6c6f 6261 6c20 6073 7461 7465 6020 6f62  lobal `state` ob
-0002c8b0: 6a65 6374 2075 7365 6420 7768 656e 205f  ject used when _
-0002c8c0: 7374 6174 655f 2069 7320 6046 616c 7365  state_ is `False
-0002c8d0: 6029 2e0a 0a23 2323 2320 6063 6f63 6f6e  `)...#### `cocon
-0002c8e0: 7574 5f65 7661 6c60 0a0a 2a2a 636f 636f  ut_eval`..**coco
-0002c8f0: 6e75 742e 636f 6e76 656e 6965 6e63 652e  nut.convenience.
-0002c900: 636f 636f 6e75 745f 6576 616c 2a2a 285f  coconut_eval**(_
-0002c910: 6578 7072 6573 7369 6f6e 5f2c 205f 676c  expression_, _gl
-0002c920: 6f62 616c 735f 3d60 4e6f 6e65 602c 205f  obals_=`None`, _
-0002c930: 6c6f 6361 6c73 5f3d 604e 6f6e 6560 2c20  locals_=`None`, 
-0002c940: 5f73 7461 7465 5f3d 6046 616c 7365 602c  _state_=`False`,
-0002c950: 205f 6b65 6570 5c5f 696e 7465 726e 616c   _keep\_internal
-0002c960: 5c5f 7374 6174 655f 3d60 4e6f 6e65 6029  \_state_=`None`)
-0002c970: 0a0a 5665 7273 696f 6e20 6f66 205b 6065  ..Version of [`e
-0002c980: 7661 6c60 5d28 6874 7470 733a 2f2f 646f  val`](https://do
-0002c990: 6373 2e70 7974 686f 6e2e 6f72 672f 332f  cs.python.org/3/
-0002c9a0: 6c69 6272 6172 792f 6675 6e63 7469 6f6e  library/function
-0002c9b0: 732e 6874 6d6c 2365 7661 6c29 2077 6869  s.html#eval) whi
-0002c9c0: 6368 2063 616e 2065 7661 6c75 6174 6520  ch can evaluate 
-0002c9d0: 436f 636f 6e75 7420 636f 6465 2e0a 0a23  Coconut code...#
-0002c9e0: 2323 2320 6076 6572 7369 6f6e 600a 0a2a  ### `version`..*
-0002c9f0: 2a63 6f63 6f6e 7574 2e63 6f6e 7665 6e69  *coconut.conveni
-0002ca00: 656e 6365 2e76 6572 7369 6f6e 2a2a 282a  ence.version**(*
-0002ca10: 2a5b 2a2a 5f77 6869 6368 5f2a 2a5d 2a2a  *[**_which_**]**
-0002ca20: 290a 0a52 6574 7269 6576 6573 2061 2073  )..Retrieves a s
-0002ca30: 7472 696e 6720 636f 6e74 6169 6e69 6e67  tring containing
-0002ca40: 2069 6e66 6f72 6d61 7469 6f6e 2061 626f   information abo
-0002ca50: 7574 2074 6865 2043 6f63 6f6e 7574 2076  ut the Coconut v
-0002ca60: 6572 7369 6f6e 2e20 5468 6520 6f70 7469  ersion. The opti
-0002ca70: 6f6e 616c 2061 7267 756d 656e 7420 5f77  onal argument _w
-0002ca80: 6869 6368 5f20 6973 2074 6865 2074 7970  hich_ is the typ
-0002ca90: 6520 6f66 2076 6572 7369 6f6e 2069 6e66  e of version inf
-0002caa0: 6f72 6d61 7469 6f6e 2064 6573 6972 6564  ormation desired
-0002cab0: 2e20 506f 7373 6962 6c65 2076 616c 7565  . Possible value
-0002cac0: 7320 6f66 205f 7768 6963 685f 2061 7265  s of _which_ are
-0002cad0: 3a0a 0a2d 2060 226e 756d 2260 3a20 7468  :..- `"num"`: th
-0002cae0: 6520 6e75 6d65 7269 6361 6c20 7665 7273  e numerical vers
-0002caf0: 696f 6e20 2874 6865 2064 6566 6175 6c74  ion (the default
-0002cb00: 290a 2d20 6022 6e61 6d65 2260 3a20 7468  ).- `"name"`: th
-0002cb10: 6520 7665 7273 696f 6e20 636f 6465 6e61  e version codena
-0002cb20: 6d65 0a2d 2060 2273 7065 6322 603a 2074  me.- `"spec"`: t
-0002cb30: 6865 206e 756d 6572 6963 616c 2076 6572  he numerical ver
-0002cb40: 7369 6f6e 2077 6974 6820 7468 6520 636f  sion with the co
-0002cb50: 6465 6e61 6d65 2061 7474 6163 6865 640a  dename attached.
-0002cb60: 2d20 6022 7461 6722 603a 2074 6865 2076  - `"tag"`: the v
-0002cb70: 6572 7369 6f6e 2074 6167 2075 7365 6420  ersion tag used 
-0002cb80: 696e 2047 6974 4875 6220 616e 6420 646f  in GitHub and do
-0002cb90: 6375 6d65 6e74 6174 696f 6e20 5552 4c73  cumentation URLs
-0002cba0: 0a2d 2060 222d 7622 603a 2074 6865 2066  .- `"-v"`: the f
-0002cbb0: 756c 6c20 7374 7269 6e67 2070 7269 6e74  ull string print
-0002cbc0: 6564 2062 7920 6063 6f63 6f6e 7574 202d  ed by `coconut -
-0002cbd0: 7660 0a0a 2323 2323 2060 6175 746f 5f63  v`..#### `auto_c
-0002cbe0: 6f6d 7069 6c61 7469 6f6e 600a 0a2a 2a63  ompilation`..**c
-0002cbf0: 6f63 6f6e 7574 2e63 6f6e 7665 6e69 656e  oconut.convenien
-0002cc00: 6365 2e61 7574 6f5f 636f 6d70 696c 6174  ce.auto_compilat
-0002cc10: 696f 6e2a 2a28 5f6f 6e5f 3d60 5472 7565  ion**(_on_=`True
-0002cc20: 6029 0a0a 5475 726e 7320 5b61 7574 6f6d  `)..Turns [autom
-0002cc30: 6174 6963 2063 6f6d 7069 6c61 7469 6f6e  atic compilation
-0002cc40: 5d28 2361 7574 6f6d 6174 6963 2d63 6f6d  ](#automatic-com
-0002cc50: 7069 6c61 7469 6f6e 2920 6f6e 206f 7220  pilation) on or 
-0002cc60: 6f66 662e 2054 6869 7320 6675 6e63 7469  off. This functi
-0002cc70: 6f6e 2069 7320 6361 6c6c 6564 2061 7574  on is called aut
-0002cc80: 6f6d 6174 6963 616c 6c79 2077 6865 6e20  omatically when 
-0002cc90: 6063 6f63 6f6e 7574 2e63 6f6e 7665 6e69  `coconut.conveni
-0002cca0: 656e 6365 6020 6973 2069 6d70 6f72 7465  ence` is importe
-0002ccb0: 642e 0a0a 2323 2323 2060 7573 655f 636f  d...#### `use_co
-0002ccc0: 636f 6e75 745f 6272 6561 6b70 6f69 6e74  conut_breakpoint
-0002ccd0: 600a 0a2a 2a63 6f63 6f6e 7574 2e63 6f6e  `..**coconut.con
-0002cce0: 7665 6e69 656e 6365 2e75 7365 5f63 6f63  venience.use_coc
-0002ccf0: 6f6e 7574 5f62 7265 616b 706f 696e 742a  onut_breakpoint*
-0002cd00: 2a28 5f6f 6e5f 3d60 5472 7565 6029 0a0a  *(_on_=`True`)..
-0002cd10: 5377 6974 6368 6573 2074 6865 205b 6062  Switches the [`b
-0002cd20: 7265 616b 706f 696e 7460 2062 7569 6c74  reakpoint` built
-0002cd30: 2d69 6e5d 2868 7474 7073 3a2f 2f77 7777  -in](https://www
-0002cd40: 2e70 7974 686f 6e2e 6f72 672f 6465 762f  .python.org/dev/
-0002cd50: 7065 7073 2f70 6570 2d30 3535 332f 2920  peps/pep-0553/) 
-0002cd60: 7768 6963 6820 436f 636f 6e75 7420 6d61  which Coconut ma
-0002cd70: 6b65 7320 756e 6976 6572 7361 6c6c 7920  kes universally 
-0002cd80: 6176 6169 6c61 626c 6520 746f 2075 7365  available to use
-0002cd90: 205b 6063 6f63 6f6e 7574 2e65 6d62 6564   [`coconut.embed
-0002cda0: 605d 2823 636f 636f 6e75 742d 656d 6265  `](#coconut-embe
-0002cdb0: 6429 2069 6e73 7465 6164 206f 6620 5b60  d) instead of [`
-0002cdc0: 7064 622e 7365 745f 7472 6163 6560 5d28  pdb.set_trace`](
-0002cdd0: 6874 7470 733a 2f2f 646f 6373 2e70 7974  https://docs.pyt
-0002cde0: 686f 6e2e 6f72 672f 332f 6c69 6272 6172  hon.org/3/librar
-0002cdf0: 792f 7064 622e 6874 6d6c 2370 6462 2e73  y/pdb.html#pdb.s
-0002ce00: 6574 5f74 7261 6365 2920 286f 7220 756e  et_trace) (or un
-0002ce10: 646f 6573 2074 6861 7420 7377 6974 6368  does that switch
-0002ce20: 2069 6620 606f 6e3d 4661 6c73 6560 292e   if `on=False`).
-0002ce30: 2054 6869 7320 6675 6e63 7469 6f6e 2069   This function i
-0002ce40: 7320 6361 6c6c 6564 2061 7574 6f6d 6174  s called automat
-0002ce50: 6963 616c 6c79 2077 6865 6e20 6063 6f63  ically when `coc
-0002ce60: 6f6e 7574 2e63 6f6e 7665 6e69 656e 6365  onut.convenience
-0002ce70: 6020 6973 2069 6d70 6f72 7465 642e 0a0a  ` is imported...
-0002ce80: 2323 2323 2060 436f 636f 6e75 7445 7863  #### `CoconutExc
-0002ce90: 6570 7469 6f6e 600a 0a49 6620 616e 2065  eption`..If an e
-0002cea0: 7272 6f72 2069 7320 656e 636f 756e 7465  rror is encounte
-0002ceb0: 7265 6420 696e 2061 2063 6f6e 7665 6e69  red in a conveni
-0002cec0: 656e 6365 2066 756e 6374 696f 6e2c 2061  ence function, a
-0002ced0: 2060 436f 636f 6e75 7445 7863 6570 7469   `CoconutExcepti
-0002cee0: 6f6e 6020 696e 7374 616e 6365 206d 6179  on` instance may
-0002cef0: 2062 6520 7261 6973 6564 2e20 6063 6f63   be raised. `coc
-0002cf00: 6f6e 7574 2e63 6f6e 7665 6e69 656e 6365  onut.convenience
-0002cf10: 2e43 6f63 6f6e 7574 4578 6365 7074 696f  .CoconutExceptio
-0002cf20: 6e60 2069 7320 7072 6f76 6964 6564 2074  n` is provided t
-0002cf30: 6f20 616c 6c6f 7720 6361 7463 6869 6e67  o allow catching
-0002cf40: 2073 7563 6820 6572 726f 7273 2e0a 0a23   such errors...#
-0002cf50: 2323 2060 636f 636f 6e75 742e 5f5f 636f  ## `coconut.__co
-0002cf60: 636f 6e75 745f 5f60 0a0a 4974 2069 7320  conut__`..It is 
-0002cf70: 736f 6d65 7469 6d65 7320 7573 6566 756c  sometimes useful
-0002cf80: 2074 6f20 6265 2061 626c 6520 746f 2061   to be able to a
-0002cf90: 6363 6573 7320 436f 636f 6e75 7420 6275  ccess Coconut bu
-0002cfa0: 696c 742d 696e 7320 6672 6f6d 2070 7572  ilt-ins from pur
-0002cfb0: 6520 5079 7468 6f6e 2e20 546f 2061 6363  e Python. To acc
-0002cfc0: 6f6d 706c 6973 6820 7468 6973 2c20 436f  omplish this, Co
-0002cfd0: 636f 6e75 7420 7072 6f76 6964 6573 2060  conut provides `
-0002cfe0: 636f 636f 6e75 742e 5f5f 636f 636f 6e75  coconut.__coconu
-0002cff0: 745f 5f60 2c20 7768 6963 6820 6265 6861  t__`, which beha
-0002d000: 7665 7320 6578 6163 746c 7920 6c69 6b65  ves exactly like
-0002d010: 2074 6865 2060 5f5f 636f 636f 6e75 745f   the `__coconut_
-0002d020: 5f2e 7079 6020 6865 6164 6572 2066 696c  _.py` header fil
-0002d030: 6520 696e 636c 7564 6564 2077 6865 6e20  e included when 
-0002d040: 436f 636f 6e75 7420 6973 2063 6f6d 7069  Coconut is compi
-0002d050: 6c65 6420 696e 2070 6163 6b61 6765 206d  led in package m
-0002d060: 6f64 652e 0a0a 416c 6c20 436f 636f 6e75  ode...All Coconu
-0002d070: 7420 6275 696c 742d 696e 7320 6172 6520  t built-ins are 
-0002d080: 6163 6365 7373 6962 6c65 2066 726f 6d20  accessible from 
-0002d090: 6063 6f63 6f6e 7574 2e5f 5f63 6f63 6f6e  `coconut.__cocon
-0002d0a0: 7574 5f5f 602e 2054 6865 2072 6563 6f6d  ut__`. The recom
-0002d0b0: 6d65 6e64 6564 2077 6179 2074 6f20 696d  mended way to im
-0002d0c0: 706f 7274 2074 6865 6d20 6973 2074 6f20  port them is to 
-0002d0d0: 7573 6520 6066 726f 6d20 636f 636f 6e75  use `from coconu
-0002d0e0: 742e 5f5f 636f 636f 6e75 745f 5f20 696d  t.__coconut__ im
-0002d0f0: 706f 7274 6020 616e 6420 696d 706f 7274  port` and import
-0002d100: 2077 6861 7465 7665 7220 6275 696c 742d   whatever built-
-0002d110: 696e 7320 796f 7527 6c6c 2062 6520 7573  ins you'll be us
-0002d120: 696e 672e 0a0a 2323 2323 2320 4578 616d  ing...##### Exam
-0002d130: 706c 650a 0a60 6060 636f 636f 6e75 745f  ple..```coconut_
-0002d140: 7079 7468 6f6e 0a66 726f 6d20 636f 636f  python.from coco
-0002d150: 6e75 742e 5f5f 636f 636f 6e75 745f 5f20  nut.__coconut__ 
-0002d160: 696d 706f 7274 2070 6172 616c 6c65 6c5f  import parallel_
-0002d170: 6d61 700a 6060 600a                      map.```.
+0002c610: 6f72 2060 5472 7565 600a 0a23 2323 2320  or `True`..#### 
+0002c620: 6063 6d64 600a 0a2a 2a63 6f63 6f6e 7574  `cmd`..**coconut
+0002c630: 2e63 6f6e 7665 6e69 656e 6365 2e63 6d64  .convenience.cmd
+0002c640: 2a2a 285f 6172 6773 5f3d 604e 6f6e 6560  **(_args_=`None`
+0002c650: 2c20 2a2c 205f 6172 6776 5f3d 604e 6f6e  , *, _argv_=`Non
+0002c660: 6560 2c20 5f69 6e74 6572 6163 745f 3d60  e`, _interact_=`
+0002c670: 4661 6c73 6560 2c20 5f64 6566 6175 6c74  False`, _default
+0002c680: 5c5f 7461 7267 6574 5f3d 604e 6f6e 6560  \_target_=`None`
+0002c690: 2c20 5f73 7461 7465 5f3d 6046 616c 7365  , _state_=`False
+0002c6a0: 6029 0a0a 4578 6563 7574 6573 2074 6865  `)..Executes the
+0002c6b0: 2067 6976 656e 205f 6172 6773 5f20 6173   given _args_ as
+0002c6c0: 2069 6620 7468 6579 2077 6572 6520 6665   if they were fe
+0002c6d0: 6420 746f 2060 636f 636f 6e75 7460 206f  d to `coconut` o
+0002c6e0: 6e20 7468 6520 636f 6d6d 616e 642d 6c69  n the command-li
+0002c6f0: 6e65 2c20 7769 7468 2074 6865 2065 7863  ne, with the exc
+0002c700: 6570 7469 6f6e 2074 6861 7420 756e 6c65  eption that unle
+0002c710: 7373 205f 696e 7465 7261 6374 5f20 6973  ss _interact_ is
+0002c720: 2074 7275 6520 6f72 2060 2d69 6020 6973   true or `-i` is
+0002c730: 2070 6173 7365 642c 2074 6865 2069 6e74   passed, the int
+0002c740: 6572 7072 6574 6572 2077 696c 6c20 6e6f  erpreter will no
+0002c750: 7420 6265 2073 7461 7274 6564 2e20 4164  t be started. Ad
+0002c760: 6469 7469 6f6e 616c 6c79 2c20 5f61 7267  ditionally, _arg
+0002c770: 765f 2063 616e 2062 6520 7573 6564 2074  v_ can be used t
+0002c780: 6f20 7061 7373 2069 6e20 6172 6775 6d65  o pass in argume
+0002c790: 6e74 7320 6173 2069 6e20 602d 2d61 7267  nts as in `--arg
+0002c7a0: 7660 2061 6e64 205f 6465 6661 756c 745c  v` and _default\
+0002c7b0: 5f74 6172 6765 745f 2063 616e 2062 6520  _target_ can be 
+0002c7c0: 7573 6564 2074 6f20 7365 7420 7468 6520  used to set the 
+0002c7d0: 6465 6661 756c 7420 602d 2d74 6172 6765  default `--targe
+0002c7e0: 7460 2e0a 0a48 6173 2074 6865 2073 616d  t`...Has the sam
+0002c7f0: 6520 6566 6665 6374 206f 6620 7365 7474  e effect of sett
+0002c800: 696e 6720 7468 6520 636f 6d6d 616e 642d  ing the command-
+0002c810: 6c69 6e65 2066 6c61 6773 206f 6e20 7468  line flags on th
+0002c820: 6520 6769 7665 6e20 5f73 7461 7465 5f20  e given _state_ 
+0002c830: 6f62 6a65 6374 2061 7320 6073 6574 7570  object as `setup
+0002c840: 6020 2877 6974 6820 7468 6520 676c 6f62  ` (with the glob
+0002c850: 616c 2060 7374 6174 6560 206f 626a 6563  al `state` objec
+0002c860: 7420 7573 6564 2077 6865 6e20 5f73 7461  t used when _sta
+0002c870: 7465 5f20 6973 2060 4661 6c73 6560 292e  te_ is `False`).
+0002c880: 0a0a 2323 2323 2060 636f 636f 6e75 745f  ..#### `coconut_
+0002c890: 6576 616c 600a 0a2a 2a63 6f63 6f6e 7574  eval`..**coconut
+0002c8a0: 2e63 6f6e 7665 6e69 656e 6365 2e63 6f63  .convenience.coc
+0002c8b0: 6f6e 7574 5f65 7661 6c2a 2a28 5f65 7870  onut_eval**(_exp
+0002c8c0: 7265 7373 696f 6e5f 2c20 5f67 6c6f 6261  ression_, _globa
+0002c8d0: 6c73 5f3d 604e 6f6e 6560 2c20 5f6c 6f63  ls_=`None`, _loc
+0002c8e0: 616c 735f 3d60 4e6f 6e65 602c 205f 7374  als_=`None`, _st
+0002c8f0: 6174 655f 3d60 4661 6c73 6560 2c20 5f6b  ate_=`False`, _k
+0002c900: 6565 705c 5f69 6e74 6572 6e61 6c5c 5f73  eep\_internal\_s
+0002c910: 7461 7465 5f3d 604e 6f6e 6560 290a 0a56  tate_=`None`)..V
+0002c920: 6572 7369 6f6e 206f 6620 5b60 6576 616c  ersion of [`eval
+0002c930: 605d 2868 7474 7073 3a2f 2f64 6f63 732e  `](https://docs.
+0002c940: 7079 7468 6f6e 2e6f 7267 2f33 2f6c 6962  python.org/3/lib
+0002c950: 7261 7279 2f66 756e 6374 696f 6e73 2e68  rary/functions.h
+0002c960: 746d 6c23 6576 616c 2920 7768 6963 6820  tml#eval) which 
+0002c970: 6361 6e20 6576 616c 7561 7465 2043 6f63  can evaluate Coc
+0002c980: 6f6e 7574 2063 6f64 652e 0a0a 2323 2323  onut code...####
+0002c990: 2060 7665 7273 696f 6e60 0a0a 2a2a 636f   `version`..**co
+0002c9a0: 636f 6e75 742e 636f 6e76 656e 6965 6e63  conut.convenienc
+0002c9b0: 652e 7665 7273 696f 6e2a 2a28 2a2a 5b2a  e.version**(**[*
+0002c9c0: 2a5f 7768 6963 685f 2a2a 5d2a 2a29 0a0a  *_which_**]**)..
+0002c9d0: 5265 7472 6965 7665 7320 6120 7374 7269  Retrieves a stri
+0002c9e0: 6e67 2063 6f6e 7461 696e 696e 6720 696e  ng containing in
+0002c9f0: 666f 726d 6174 696f 6e20 6162 6f75 7420  formation about 
+0002ca00: 7468 6520 436f 636f 6e75 7420 7665 7273  the Coconut vers
+0002ca10: 696f 6e2e 2054 6865 206f 7074 696f 6e61  ion. The optiona
+0002ca20: 6c20 6172 6775 6d65 6e74 205f 7768 6963  l argument _whic
+0002ca30: 685f 2069 7320 7468 6520 7479 7065 206f  h_ is the type o
+0002ca40: 6620 7665 7273 696f 6e20 696e 666f 726d  f version inform
+0002ca50: 6174 696f 6e20 6465 7369 7265 642e 2050  ation desired. P
+0002ca60: 6f73 7369 626c 6520 7661 6c75 6573 206f  ossible values o
+0002ca70: 6620 5f77 6869 6368 5f20 6172 653a 0a0a  f _which_ are:..
+0002ca80: 2d20 6022 6e75 6d22 603a 2074 6865 206e  - `"num"`: the n
+0002ca90: 756d 6572 6963 616c 2076 6572 7369 6f6e  umerical version
+0002caa0: 2028 7468 6520 6465 6661 756c 7429 0a2d   (the default).-
+0002cab0: 2060 226e 616d 6522 603a 2074 6865 2076   `"name"`: the v
+0002cac0: 6572 7369 6f6e 2063 6f64 656e 616d 650a  ersion codename.
+0002cad0: 2d20 6022 7370 6563 2260 3a20 7468 6520  - `"spec"`: the 
+0002cae0: 6e75 6d65 7269 6361 6c20 7665 7273 696f  numerical versio
+0002caf0: 6e20 7769 7468 2074 6865 2063 6f64 656e  n with the coden
+0002cb00: 616d 6520 6174 7461 6368 6564 0a2d 2060  ame attached.- `
+0002cb10: 2274 6167 2260 3a20 7468 6520 7665 7273  "tag"`: the vers
+0002cb20: 696f 6e20 7461 6720 7573 6564 2069 6e20  ion tag used in 
+0002cb30: 4769 7448 7562 2061 6e64 2064 6f63 756d  GitHub and docum
+0002cb40: 656e 7461 7469 6f6e 2055 524c 730a 2d20  entation URLs.- 
+0002cb50: 6022 2d76 2260 3a20 7468 6520 6675 6c6c  `"-v"`: the full
+0002cb60: 2073 7472 696e 6720 7072 696e 7465 6420   string printed 
+0002cb70: 6279 2060 636f 636f 6e75 7420 2d76 600a  by `coconut -v`.
+0002cb80: 0a23 2323 2320 6061 7574 6f5f 636f 6d70  .#### `auto_comp
+0002cb90: 696c 6174 696f 6e60 0a0a 2a2a 636f 636f  ilation`..**coco
+0002cba0: 6e75 742e 636f 6e76 656e 6965 6e63 652e  nut.convenience.
+0002cbb0: 6175 746f 5f63 6f6d 7069 6c61 7469 6f6e  auto_compilation
+0002cbc0: 2a2a 285f 6f6e 5f3d 6054 7275 6560 290a  **(_on_=`True`).
+0002cbd0: 0a54 7572 6e73 205b 6175 746f 6d61 7469  .Turns [automati
+0002cbe0: 6320 636f 6d70 696c 6174 696f 6e5d 2823  c compilation](#
+0002cbf0: 6175 746f 6d61 7469 632d 636f 6d70 696c  automatic-compil
+0002cc00: 6174 696f 6e29 206f 6e20 6f72 206f 6666  ation) on or off
+0002cc10: 2e20 5468 6973 2066 756e 6374 696f 6e20  . This function 
+0002cc20: 6973 2063 616c 6c65 6420 6175 746f 6d61  is called automa
+0002cc30: 7469 6361 6c6c 7920 7768 656e 2060 636f  tically when `co
+0002cc40: 636f 6e75 742e 636f 6e76 656e 6965 6e63  conut.convenienc
+0002cc50: 6560 2069 7320 696d 706f 7274 6564 2e0a  e` is imported..
+0002cc60: 0a23 2323 2320 6075 7365 5f63 6f63 6f6e  .#### `use_cocon
+0002cc70: 7574 5f62 7265 616b 706f 696e 7460 0a0a  ut_breakpoint`..
+0002cc80: 2a2a 636f 636f 6e75 742e 636f 6e76 656e  **coconut.conven
+0002cc90: 6965 6e63 652e 7573 655f 636f 636f 6e75  ience.use_coconu
+0002cca0: 745f 6272 6561 6b70 6f69 6e74 2a2a 285f  t_breakpoint**(_
+0002ccb0: 6f6e 5f3d 6054 7275 6560 290a 0a53 7769  on_=`True`)..Swi
+0002ccc0: 7463 6865 7320 7468 6520 5b60 6272 6561  tches the [`brea
+0002ccd0: 6b70 6f69 6e74 6020 6275 696c 742d 696e  kpoint` built-in
+0002cce0: 5d28 6874 7470 733a 2f2f 7777 772e 7079  ](https://www.py
+0002ccf0: 7468 6f6e 2e6f 7267 2f64 6576 2f70 6570  thon.org/dev/pep
+0002cd00: 732f 7065 702d 3035 3533 2f29 2077 6869  s/pep-0553/) whi
+0002cd10: 6368 2043 6f63 6f6e 7574 206d 616b 6573  ch Coconut makes
+0002cd20: 2075 6e69 7665 7273 616c 6c79 2061 7661   universally ava
+0002cd30: 696c 6162 6c65 2074 6f20 7573 6520 5b60  ilable to use [`
+0002cd40: 636f 636f 6e75 742e 656d 6265 6460 5d28  coconut.embed`](
+0002cd50: 2363 6f63 6f6e 7574 2d65 6d62 6564 2920  #coconut-embed) 
+0002cd60: 696e 7374 6561 6420 6f66 205b 6070 6462  instead of [`pdb
+0002cd70: 2e73 6574 5f74 7261 6365 605d 2868 7474  .set_trace`](htt
+0002cd80: 7073 3a2f 2f64 6f63 732e 7079 7468 6f6e  ps://docs.python
+0002cd90: 2e6f 7267 2f33 2f6c 6962 7261 7279 2f70  .org/3/library/p
+0002cda0: 6462 2e68 746d 6c23 7064 622e 7365 745f  db.html#pdb.set_
+0002cdb0: 7472 6163 6529 2028 6f72 2075 6e64 6f65  trace) (or undoe
+0002cdc0: 7320 7468 6174 2073 7769 7463 6820 6966  s that switch if
+0002cdd0: 2060 6f6e 3d46 616c 7365 6029 2e20 5468   `on=False`). Th
+0002cde0: 6973 2066 756e 6374 696f 6e20 6973 2063  is function is c
+0002cdf0: 616c 6c65 6420 6175 746f 6d61 7469 6361  alled automatica
+0002ce00: 6c6c 7920 7768 656e 2060 636f 636f 6e75  lly when `coconu
+0002ce10: 742e 636f 6e76 656e 6965 6e63 6560 2069  t.convenience` i
+0002ce20: 7320 696d 706f 7274 6564 2e0a 0a23 2323  s imported...###
+0002ce30: 2320 6043 6f63 6f6e 7574 4578 6365 7074  # `CoconutExcept
+0002ce40: 696f 6e60 0a0a 4966 2061 6e20 6572 726f  ion`..If an erro
+0002ce50: 7220 6973 2065 6e63 6f75 6e74 6572 6564  r is encountered
+0002ce60: 2069 6e20 6120 636f 6e76 656e 6965 6e63   in a convenienc
+0002ce70: 6520 6675 6e63 7469 6f6e 2c20 6120 6043  e function, a `C
+0002ce80: 6f63 6f6e 7574 4578 6365 7074 696f 6e60  oconutException`
+0002ce90: 2069 6e73 7461 6e63 6520 6d61 7920 6265   instance may be
+0002cea0: 2072 6169 7365 642e 2060 636f 636f 6e75   raised. `coconu
+0002ceb0: 742e 636f 6e76 656e 6965 6e63 652e 436f  t.convenience.Co
+0002cec0: 636f 6e75 7445 7863 6570 7469 6f6e 6020  conutException` 
+0002ced0: 6973 2070 726f 7669 6465 6420 746f 2061  is provided to a
+0002cee0: 6c6c 6f77 2063 6174 6368 696e 6720 7375  llow catching su
+0002cef0: 6368 2065 7272 6f72 732e 0a0a 2323 2320  ch errors...### 
+0002cf00: 6063 6f63 6f6e 7574 2e5f 5f63 6f63 6f6e  `coconut.__cocon
+0002cf10: 7574 5f5f 600a 0a49 7420 6973 2073 6f6d  ut__`..It is som
+0002cf20: 6574 696d 6573 2075 7365 6675 6c20 746f  etimes useful to
+0002cf30: 2062 6520 6162 6c65 2074 6f20 6163 6365   be able to acce
+0002cf40: 7373 2043 6f63 6f6e 7574 2062 7569 6c74  ss Coconut built
+0002cf50: 2d69 6e73 2066 726f 6d20 7075 7265 2050  -ins from pure P
+0002cf60: 7974 686f 6e2e 2054 6f20 6163 636f 6d70  ython. To accomp
+0002cf70: 6c69 7368 2074 6869 732c 2043 6f63 6f6e  lish this, Cocon
+0002cf80: 7574 2070 726f 7669 6465 7320 6063 6f63  ut provides `coc
+0002cf90: 6f6e 7574 2e5f 5f63 6f63 6f6e 7574 5f5f  onut.__coconut__
+0002cfa0: 602c 2077 6869 6368 2062 6568 6176 6573  `, which behaves
+0002cfb0: 2065 7861 6374 6c79 206c 696b 6520 7468   exactly like th
+0002cfc0: 6520 605f 5f63 6f63 6f6e 7574 5f5f 2e70  e `__coconut__.p
+0002cfd0: 7960 2068 6561 6465 7220 6669 6c65 2069  y` header file i
+0002cfe0: 6e63 6c75 6465 6420 7768 656e 2043 6f63  ncluded when Coc
+0002cff0: 6f6e 7574 2069 7320 636f 6d70 696c 6564  onut is compiled
+0002d000: 2069 6e20 7061 636b 6167 6520 6d6f 6465   in package mode
+0002d010: 2e0a 0a41 6c6c 2043 6f63 6f6e 7574 2062  ...All Coconut b
+0002d020: 7569 6c74 2d69 6e73 2061 7265 2061 6363  uilt-ins are acc
+0002d030: 6573 7369 626c 6520 6672 6f6d 2060 636f  essible from `co
+0002d040: 636f 6e75 742e 5f5f 636f 636f 6e75 745f  conut.__coconut_
+0002d050: 5f60 2e20 5468 6520 7265 636f 6d6d 656e  _`. The recommen
+0002d060: 6465 6420 7761 7920 746f 2069 6d70 6f72  ded way to impor
+0002d070: 7420 7468 656d 2069 7320 746f 2075 7365  t them is to use
+0002d080: 2060 6672 6f6d 2063 6f63 6f6e 7574 2e5f   `from coconut._
+0002d090: 5f63 6f63 6f6e 7574 5f5f 2069 6d70 6f72  _coconut__ impor
+0002d0a0: 7460 2061 6e64 2069 6d70 6f72 7420 7768  t` and import wh
+0002d0b0: 6174 6576 6572 2062 7569 6c74 2d69 6e73  atever built-ins
+0002d0c0: 2079 6f75 276c 6c20 6265 2075 7369 6e67   you'll be using
+0002d0d0: 2e0a 0a23 2323 2323 2045 7861 6d70 6c65  ...##### Example
+0002d0e0: 0a0a 6060 6063 6f63 6f6e 7574 5f70 7974  ..```coconut_pyt
+0002d0f0: 686f 6e0a 6672 6f6d 2063 6f63 6f6e 7574  hon.from coconut
+0002d100: 2e5f 5f63 6f63 6f6e 7574 5f5f 2069 6d70  .__coconut__ imp
+0002d110: 6f72 7420 7061 7261 6c6c 656c 5f6d 6170  ort parallel_map
+0002d120: 0a60 6060 0a                             .```.
```

### Comparing `coconut-develop-3.0.0a0.dev8/coconut/__coconut__.pyi` & `coconut-develop-3.0.0a0.dev9/coconut/__coconut__.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.0a0.dev8/coconut/exceptions.py` & `coconut-develop-3.0.0a0.dev9/coconut/exceptions.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.0a0.dev8/coconut/__init__.pyi` & `coconut-develop-3.0.0a0.dev9/coconut/__init__.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.0a0.dev8/coconut/highlighter.py` & `coconut-develop-3.0.0a0.dev9/coconut/highlighter.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.0a0.dev8/coconut/__coconut__.py` & `coconut-develop-3.0.0a0.dev9/coconut/__coconut__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.0a0.dev8/coconut/root.py` & `coconut-develop-3.0.0a0.dev9/coconut/root.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # -----------------------------------------------------------------------------------------------------------------------
 # VERSION:
 # -----------------------------------------------------------------------------------------------------------------------
 
 VERSION = "3.0.0"
 VERSION_NAME = None
 # False for release, int >= 1 for develop
-DEVELOP = 8
+DEVELOP = 9
 ALPHA = True  # for pre releases rather than post releases
 
 # -----------------------------------------------------------------------------------------------------------------------
 # UTILITIES:
 # -----------------------------------------------------------------------------------------------------------------------
```

### Comparing `coconut-develop-3.0.0a0.dev8/coconut/icoconut/embed.py` & `coconut-develop-3.0.0a0.dev9/coconut/icoconut/embed.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.0a0.dev8/coconut/icoconut/root.py` & `coconut-develop-3.0.0a0.dev9/coconut/icoconut/root.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.0a0.dev8/coconut/icoconut/__init__.py` & `coconut-develop-3.0.0a0.dev9/coconut/icoconut/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.0a0.dev8/coconut/icoconut/__main__.py` & `coconut-develop-3.0.0a0.dev9/coconut/icoconut/__main__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.0a0.dev8/coconut/tests/main_test.py` & `coconut-develop-3.0.0a0.dev9/coconut/tests/main_test.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.0a0.dev8/coconut/tests/constants_test.py` & `coconut-develop-3.0.0a0.dev9/coconut/tests/constants_test.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.0a0.dev8/coconut/tests/__init__.py` & `coconut-develop-3.0.0a0.dev9/coconut/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.0a0.dev8/coconut/tests/__main__.py` & `coconut-develop-3.0.0a0.dev9/coconut/tests/__main__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.0a0.dev8/coconut/tests/src/extras.coco` & `coconut-develop-3.0.0a0.dev9/coconut/tests/src/extras.coco`

 * *Files 1% similar despite different names*

```diff
@@ -416,14 +416,17 @@
     )
     assert non_zero_diags([1,0,1;;0,1,0;;1,0,1])
     assert not non_zero_diags([1,0,0;;0,1,0;;1,0,1])
     enumeration = multi_enumerate(np.array([1, 2;; 3, 4]))
     assert len(enumeration) == 4  # type: ignore
     assert enumeration[2] == ((1, 0), 3)  # type: ignore
     assert list(enumeration) == [((0, 0), 1), ((0, 1), 2), ((1, 0), 3), ((1, 1), 4)]
+    for ind, x in multi_enumerate(np.array([1, 2])):
+        assert ind `isinstance` tuple, (type(ind), ind)
+        assert x `isinstance` np.int32, (type(x), x)
     assert all_equal(np.array([]))
     assert all_equal(np.array([1]))
     assert all_equal(np.array([1, 1]))
     assert all_equal(np.array([1, 1;; 1, 1]))
     assert not all_equal(np.array([1, 1;; 1, 2]))
     assert (
         cartesian_product(np.array([1, 2]), np.array([3, 4]))
```

### Comparing `coconut-develop-3.0.0a0.dev8/coconut/tests/src/cocotest/agnostic/suite.coco` & `coconut-develop-3.0.0a0.dev9/coconut/tests/src/cocotest/agnostic/suite.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.0a0.dev8/coconut/tests/src/cocotest/agnostic/main.coco` & `coconut-develop-3.0.0a0.dev9/coconut/tests/src/cocotest/agnostic/main.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.0a0.dev8/coconut/tests/src/cocotest/agnostic/specific.coco` & `coconut-develop-3.0.0a0.dev9/coconut/tests/src/cocotest/agnostic/specific.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.0a0.dev8/coconut/tests/src/cocotest/agnostic/tutorial.coco` & `coconut-develop-3.0.0a0.dev9/coconut/tests/src/cocotest/agnostic/tutorial.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.0a0.dev8/coconut/tests/src/cocotest/agnostic/util.coco` & `coconut-develop-3.0.0a0.dev9/coconut/tests/src/cocotest/agnostic/util.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.0a0.dev8/coconut/tests/src/cocotest/agnostic/primary.coco` & `coconut-develop-3.0.0a0.dev9/coconut/tests/src/cocotest/agnostic/primary.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.0a0.dev8/coconut/tests/src/cocotest/target_36/py36_test.coco` & `coconut-develop-3.0.0a0.dev9/coconut/tests/src/cocotest/target_36/py36_test.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.0a0.dev8/coconut/tests/src/cocotest/non_strict/non_strict_test.coco` & `coconut-develop-3.0.0a0.dev9/coconut/tests/src/cocotest/non_strict/non_strict_test.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.0a0.dev8/coconut/tests/src/cocotest/target_sys/target_sys_test.coco` & `coconut-develop-3.0.0a0.dev9/coconut/tests/src/cocotest/target_sys/target_sys_test.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.0a0.dev8/coconut/tests/src/cocotest/target_3/py3_test.coco` & `coconut-develop-3.0.0a0.dev9/coconut/tests/src/cocotest/target_3/py3_test.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.0a0.dev8/coconut/__init__.py` & `coconut-develop-3.0.0a0.dev9/coconut/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.0a0.dev8/coconut/_pyparsing.py` & `coconut-develop-3.0.0a0.dev9/coconut/_pyparsing.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.0a0.dev8/coconut/main.py` & `coconut-develop-3.0.0a0.dev9/coconut/main.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.0a0.dev8/coconut/convenience.py` & `coconut-develop-3.0.0a0.dev9/coconut/convenience.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.0a0.dev8/coconut/requirements.py` & `coconut-develop-3.0.0a0.dev9/coconut/requirements.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.0a0.dev8/coconut/convenience.pyi` & `coconut-develop-3.0.0a0.dev9/coconut/convenience.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.0a0.dev8/coconut/command/mypy.py` & `coconut-develop-3.0.0a0.dev9/coconut/command/mypy.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.0a0.dev8/coconut/command/__init__.py` & `coconut-develop-3.0.0a0.dev9/coconut/command/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.0a0.dev8/coconut/command/command.pyi` & `coconut-develop-3.0.0a0.dev9/coconut/command/command.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.0a0.dev8/coconut/command/util.py` & `coconut-develop-3.0.0a0.dev9/coconut/command/util.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.0a0.dev8/coconut/command/cli.py` & `coconut-develop-3.0.0a0.dev9/coconut/command/cli.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.0a0.dev8/coconut/command/command.py` & `coconut-develop-3.0.0a0.dev9/coconut/command/command.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.0a0.dev8/coconut/command/watch.py` & `coconut-develop-3.0.0a0.dev9/coconut/command/watch.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.0a0.dev8/coconut/terminal.py` & `coconut-develop-3.0.0a0.dev9/coconut/terminal.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.0a0.dev8/coconut/util.py` & `coconut-develop-3.0.0a0.dev9/coconut/util.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.0a0.dev8/coconut/__main__.py` & `coconut-develop-3.0.0a0.dev9/coconut/__main__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.0a0.dev8/coconut/integrations.py` & `coconut-develop-3.0.0a0.dev9/coconut/integrations.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.0a0.dev8/coconut/compiler/compiler.py` & `coconut-develop-3.0.0a0.dev9/coconut/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.0a0.dev8/coconut/compiler/matching.py` & `coconut-develop-3.0.0a0.dev9/coconut/compiler/matching.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.0a0.dev8/coconut/compiler/__init__.py` & `coconut-develop-3.0.0a0.dev9/coconut/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.0a0.dev8/coconut/compiler/templates/header.py_template` & `coconut-develop-3.0.0a0.dev9/coconut/compiler/templates/header.py_template`

 * *Files 0% similar despite different names*

```diff
@@ -965,16 +965,17 @@
     def __copy__(self):
         return self.__class__(self.get_new_iter())
     @property
     def is_numpy(self):
         return self.iter.__class__.__module__ in _coconut.numpy_modules
     def __iter__(self):
         if self.is_numpy:
-            it = _coconut.numpy.nditer(self.iter, flags=["multi_index", "refs_ok"])
+            it = _coconut.numpy.nditer(self.iter, ["multi_index", "refs_ok"], [["readonly"]])
             for x in it:
+                x, = x.flatten()
                 yield it.multi_index, x
         else:
             ind = [-1]
             its = [_coconut.iter(self.iter)]
             while its:
                 ind[-1] += 1
                 try:
```

### Comparing `coconut-develop-3.0.0a0.dev8/coconut/compiler/grammar.py` & `coconut-develop-3.0.0a0.dev9/coconut/compiler/grammar.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.0a0.dev8/coconut/compiler/util.py` & `coconut-develop-3.0.0a0.dev9/coconut/compiler/util.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.0a0.dev8/coconut/compiler/header.py` & `coconut-develop-3.0.0a0.dev9/coconut/compiler/header.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.0a0.dev8/coconut/constants.py` & `coconut-develop-3.0.0a0.dev9/coconut/constants.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.0a0.dev8/conf.py` & `coconut-develop-3.0.0a0.dev9/conf.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.0a0.dev8/PKG-INFO` & `coconut-develop-3.0.0a0.dev9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coconut-develop
-Version: 3.0.0a0.dev8
+Version: 3.0.0a0.dev9
 Summary: Simple, elegant, Pythonic functional programming.
 Home-page: http://coconut-lang.org
 Author: Evan Hubinger
 Author-email: evanjhub@gmail.com
 License: Apache 2.0
 Keywords: functional,programming,language,compiler,pattern,pattern-matching,algebraic,data type,data types,lambda,lambdas,lazy,evaluation,lazy list,lazy lists,tail,recursion,call,recursive,infix,function,composition,compose,partial,application,currying,curry,pipeline,pipe,unicode,operator,operators,frozenset,literal,syntax,destructuring,assignment,fold,datamaker,prepattern,iterator,none,coalesce,coalescing,statement,lru_cache,memoization,backport,typing,embed,PEP 622,overrides,islice,itertools,functools,TYPE_CHECKING,Expected,breakpoint,help,reduce,takewhile,dropwhile,tee,count,makedata,consume,parallel_map,addpattern,recursive_iterator,concurrent_map,fmap,starmap,reiterable,scan,groupsof,memoize,zip_longest,override,flatten,ident,call,safe_call,flip,const,lift,all_equal,collectby,multi_enumerate,cartesian_product,multiset,cycle,windowsof,py_chr,py_hex,py_input,py_int,py_map,py_object,py_oct,py_open,py_print,py_range,py_str,py_super,py_zip,py_filter,py_reversed,py_enumerate,py_raw_input,py_xrange,py_repr,py_breakpoint,_namedtuple_of,reveal_type,reveal_locals,MatchError,__fmap__,__iter_getitem__,async,await,data,match,case,cases,where,addpattern,then,operator,type,λ
 Platform: UNKNOWN
```

### Comparing `coconut-develop-3.0.0a0.dev8/_coconut/__init__.pyi` & `coconut-develop-3.0.0a0.dev9/_coconut/__init__.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.0a0.dev8/_coconut/__init__.py` & `coconut-develop-3.0.0a0.dev9/_coconut/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.0a0.dev8/LICENSE.txt` & `coconut-develop-3.0.0a0.dev9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.0a0.dev8/FAQ.md` & `coconut-develop-3.0.0a0.dev9/FAQ.md`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.0a0.dev8/HELP.md` & `coconut-develop-3.0.0a0.dev9/HELP.md`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.0a0.dev8/coconut_develop.egg-info/SOURCES.txt` & `coconut-develop-3.0.0a0.dev9/coconut_develop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.0a0.dev8/xontrib/coconut.py` & `coconut-develop-3.0.0a0.dev9/xontrib/coconut.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.0a0.dev8/setup.py` & `coconut-develop-3.0.0a0.dev9/setup.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.0a0.dev8/README.rst` & `coconut-develop-3.0.0a0.dev9/README.rst`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.0a0.dev8/CONTRIBUTING.md` & `coconut-develop-3.0.0a0.dev9/CONTRIBUTING.md`

 * *Files identical despite different names*

