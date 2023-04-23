# Comparing `tmp/nox-2022.8.7.tar.gz` & `tmp/nox-2023.4.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nox-2022.8.7.tar", last modified: Mon Aug  8 00:27:17 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `nox-2022.8.7.tar` & `nox-2023.4.22.tar`

### file list

```diff
@@ -1,60 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 00:27:17.104719 nox-2022.8.7/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-08-08 00:27:06.000000 nox-2022.8.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-08-08 00:27:06.000000 nox-2022.8.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4096 2022-08-08 00:27:17.104719 nox-2022.8.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2793 2022-08-08 00:27:06.000000 nox-2022.8.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 00:27:17.096720 nox-2022.8.7/nox/
--rw-r--r--   0 runner    (1001) docker     (121)      994 2022-08-08 00:27:06.000000 nox-2022.8.7/nox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1861 2022-08-08 00:27:06.000000 nox-2022.8.7/nox/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3926 2022-08-08 00:27:06.000000 nox-2022.8.7/nox/_decorators.py
--rw-r--r--   0 runner    (1001) docker     (121)    11308 2022-08-08 00:27:06.000000 nox-2022.8.7/nox/_option_set.py
--rw-r--r--   0 runner    (1001) docker     (121)    16841 2022-08-08 00:27:06.000000 nox-2022.8.7/nox/_options.py
--rw-r--r--   0 runner    (1001) docker     (121)     6186 2022-08-08 00:27:06.000000 nox-2022.8.7/nox/_parametrize.py
--rw-r--r--   0 runner    (1001) docker     (121)     1270 2022-08-08 00:27:06.000000 nox-2022.8.7/nox/_typing.py
--rw-r--r--   0 runner    (1001) docker     (121)     3997 2022-08-08 00:27:06.000000 nox-2022.8.7/nox/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     4204 2022-08-08 00:27:06.000000 nox-2022.8.7/nox/command.py
--rw-r--r--   0 runner    (1001) docker     (121)     4501 2022-08-08 00:27:06.000000 nox-2022.8.7/nox/logger.py
--rw-r--r--   0 runner    (1001) docker     (121)    13925 2022-08-08 00:27:06.000000 nox-2022.8.7/nox/manifest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2698 2022-08-08 00:27:06.000000 nox-2022.8.7/nox/popen.py
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-08-08 00:27:06.000000 nox-2022.8.7/nox/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     2942 2022-08-08 00:27:06.000000 nox-2022.8.7/nox/registry.py
--rw-r--r--   0 runner    (1001) docker     (121)    29692 2022-08-08 00:27:06.000000 nox-2022.8.7/nox/sessions.py
--rw-r--r--   0 runner    (1001) docker     (121)    13667 2022-08-08 00:27:06.000000 nox-2022.8.7/nox/tasks.py
--rw-r--r--   0 runner    (1001) docker     (121)     1173 2022-08-08 00:27:06.000000 nox-2022.8.7/nox/tox_to_nox.jinja2
--rw-r--r--   0 runner    (1001) docker     (121)     1743 2022-08-08 00:27:06.000000 nox-2022.8.7/nox/tox_to_nox.py
--rw-r--r--   0 runner    (1001) docker     (121)    17375 2022-08-08 00:27:06.000000 nox-2022.8.7/nox/virtualenv.py
--rw-r--r--   0 runner    (1001) docker     (121)     2176 2022-08-08 00:27:06.000000 nox-2022.8.7/nox/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 00:27:17.100720 nox-2022.8.7/nox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4096 2022-08-08 00:27:17.000000 nox-2022.8.7/nox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1193 2022-08-08 00:27:17.000000 nox-2022.8.7/nox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-08 00:27:17.000000 nox-2022.8.7/nox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-08-08 00:27:17.000000 nox-2022.8.7/nox.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-08 00:27:16.000000 nox-2022.8.7/nox.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-08-08 00:27:17.000000 nox-2022.8.7/nox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-08-08 00:27:17.000000 nox-2022.8.7/nox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2680 2022-08-08 00:27:06.000000 nox-2022.8.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      171 2022-08-08 00:27:17.104719 nox-2022.8.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 00:27:17.100720 nox-2022.8.7/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 00:27:17.104719 nox-2022.8.7/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (121)      639 2022-08-08 00:27:06.000000 nox-2022.8.7/tests/resources/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (121)      941 2022-08-08 00:27:06.000000 nox-2022.8.7/tests/resources/noxfile_multiple_sessions.py
--rw-r--r--   0 runner    (1001) docker     (121)      790 2022-08-08 00:27:06.000000 nox-2022.8.7/tests/resources/noxfile_nested.py
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-08-08 00:27:06.000000 nox-2022.8.7/tests/resources/noxfile_normalization.py
--rw-r--r--   0 runner    (1001) docker     (121)      784 2022-08-08 00:27:06.000000 nox-2022.8.7/tests/resources/noxfile_options.py
--rw-r--r--   0 runner    (1001) docker     (121)      922 2022-08-08 00:27:06.000000 nox-2022.8.7/tests/resources/noxfile_options_pythons.py
--rw-r--r--   0 runner    (1001) docker     (121)      207 2022-08-08 00:27:06.000000 nox-2022.8.7/tests/resources/noxfile_pythons.py
--rw-r--r--   0 runner    (1001) docker     (121)      810 2022-08-08 00:27:06.000000 nox-2022.8.7/tests/resources/noxfile_spaces.py
--rw-r--r--   0 runner    (1001) docker     (121)     3559 2022-08-08 00:27:06.000000 nox-2022.8.7/tests/test__option_set.py
--rw-r--r--   0 runner    (1001) docker     (121)     8523 2022-08-08 00:27:06.000000 nox-2022.8.7/tests/test__parametrize.py
--rw-r--r--   0 runner    (1001) docker     (121)     3768 2022-08-08 00:27:06.000000 nox-2022.8.7/tests/test__version.py
--rw-r--r--   0 runner    (1001) docker     (121)     3592 2022-08-08 00:27:06.000000 nox-2022.8.7/tests/test_action_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)    13945 2022-08-08 00:27:06.000000 nox-2022.8.7/tests/test_command.py
--rw-r--r--   0 runner    (1001) docker     (121)     3116 2022-08-08 00:27:06.000000 nox-2022.8.7/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (121)    21782 2022-08-08 00:27:06.000000 nox-2022.8.7/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (121)    13212 2022-08-08 00:27:06.000000 nox-2022.8.7/tests/test_manifest.py
--rw-r--r--   0 runner    (1001) docker     (121)     3576 2022-08-08 00:27:06.000000 nox-2022.8.7/tests/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (121)    36767 2022-08-08 00:27:06.000000 nox-2022.8.7/tests/test_sessions.py
--rw-r--r--   0 runner    (1001) docker     (121)    18723 2022-08-08 00:27:06.000000 nox-2022.8.7/tests/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (121)     6546 2022-08-08 00:27:06.000000 nox-2022.8.7/tests/test_tox_to_nox.py
--rw-r--r--   0 runner    (1001) docker     (121)    25063 2022-08-08 00:27:06.000000 nox-2022.8.7/tests/test_virtualenv.py
--rw-r--r--   0 runner    (1001) docker     (121)     3274 2022-08-08 00:27:06.000000 nox-2022.8.7/tests/test_workflow.py
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 nox-2023.4.22/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 nox-2023.4.22/.readthedocs.yml
+-rw-r--r--   0        0        0    20137 2020-02-02 00:00:00.000000 nox-2023.4.22/CHANGELOG.md
+-rw-r--r--   0        0        0     3345 2020-02-02 00:00:00.000000 nox-2023.4.22/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 nox-2023.4.22/CONTRIBUTING.md
+-rw-r--r--   0        0        0     4403 2020-02-02 00:00:00.000000 nox-2023.4.22/action.yml
+-rw-r--r--   0        0        0     4677 2020-02-02 00:00:00.000000 nox-2023.4.22/noxfile.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 nox-2023.4.22/requirements-conda-test.txt
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 nox-2023.4.22/requirements-dev.txt
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 nox-2023.4.22/requirements-test.txt
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nox-2023.4.22/.github/FUNDING.yml
+-rw-r--r--   0        0        0     2669 2020-02-02 00:00:00.000000 nox-2023.4.22/.github/action_helper.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 nox-2023.4.22/.github/dependabot.yml
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 nox-2023.4.22/.github/ISSUE_TEMPLATE/bug.yml
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nox-2023.4.22/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 nox-2023.4.22/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 nox-2023.4.22/.github/workflows/action.yml
+-rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 nox-2023.4.22/.github/workflows/ci.yml
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 nox-2023.4.22/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 nox-2023.4.22/.ruff_cache/CACHEDIR.TAG
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 nox-2023.4.22/docs/CHANGELOG.md -> ../CHANGELOG.md
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 nox-2023.4.22/docs/CONTRIBUTING.md -> ../CONTRIBUTING.md
+-rw-r--r--   0        0        0     7644 2020-02-02 00:00:00.000000 nox-2023.4.22/docs/Makefile
+-rw-r--r--   0        0        0    10422 2020-02-02 00:00:00.000000 nox-2023.4.22/docs/conf.py
+-rw-r--r--   0        0        0    14342 2020-02-02 00:00:00.000000 nox-2023.4.22/docs/config.rst
+-rw-r--r--   0        0        0     5001 2020-02-02 00:00:00.000000 nox-2023.4.22/docs/cookbook.rst
+-rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 nox-2023.4.22/docs/index.rst
+-rw-r--r--   0        0        0    14211 2020-02-02 00:00:00.000000 nox-2023.4.22/docs/tutorial.rst
+-rw-r--r--   0        0        0    15441 2020-02-02 00:00:00.000000 nox-2023.4.22/docs/usage.rst
+-rw-r--r--   0        0        0  3379966 2020-02-02 00:00:00.000000 nox-2023.4.22/docs/_static/alice-full.png
+-rw-r--r--   0        0        0    10140 2020-02-02 00:00:00.000000 nox-2023.4.22/docs/_static/alice.gif
+-rw-r--r--   0        0        0   507218 2020-02-02 00:00:00.000000 nox-2023.4.22/docs/_static/alice.png
+-rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 nox-2023.4.22/docs/_static/custom.css
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 nox-2023.4.22/nox/__init__.py
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 nox-2023.4.22/nox/__main__.py
+-rw-r--r--   0        0        0     3929 2020-02-02 00:00:00.000000 nox-2023.4.22/nox/_decorators.py
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 nox-2023.4.22/nox/_option_set.py
+-rw-r--r--   0        0        0    17571 2020-02-02 00:00:00.000000 nox-2023.4.22/nox/_options.py
+-rw-r--r--   0        0        0     6172 2020-02-02 00:00:00.000000 nox-2023.4.22/nox/_parametrize.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 nox-2023.4.22/nox/_typing.py
+-rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 nox-2023.4.22/nox/_version.py
+-rw-r--r--   0        0        0     4091 2020-02-02 00:00:00.000000 nox-2023.4.22/nox/command.py
+-rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 nox-2023.4.22/nox/logger.py
+-rw-r--r--   0        0        0    13856 2020-02-02 00:00:00.000000 nox-2023.4.22/nox/manifest.py
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 nox-2023.4.22/nox/popen.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 nox-2023.4.22/nox/py.typed
+-rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 nox-2023.4.22/nox/registry.py
+-rw-r--r--   0        0        0    30558 2020-02-02 00:00:00.000000 nox-2023.4.22/nox/sessions.py
+-rw-r--r--   0        0        0    14603 2020-02-02 00:00:00.000000 nox-2023.4.22/nox/tasks.py
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 nox-2023.4.22/nox/tox_to_nox.jinja2
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 nox-2023.4.22/nox/tox_to_nox.py
+-rw-r--r--   0        0        0    17325 2020-02-02 00:00:00.000000 nox-2023.4.22/nox/virtualenv.py
+-rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 nox-2023.4.22/nox/workflow.py
+-rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 nox-2023.4.22/tests/test__option_set.py
+-rw-r--r--   0        0        0     8521 2020-02-02 00:00:00.000000 nox-2023.4.22/tests/test__parametrize.py
+-rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 nox-2023.4.22/tests/test__version.py
+-rw-r--r--   0        0        0     3241 2020-02-02 00:00:00.000000 nox-2023.4.22/tests/test_action_helper.py
+-rw-r--r--   0        0        0    14956 2020-02-02 00:00:00.000000 nox-2023.4.22/tests/test_command.py
+-rw-r--r--   0        0        0     3116 2020-02-02 00:00:00.000000 nox-2023.4.22/tests/test_logger.py
+-rw-r--r--   0        0        0    22551 2020-02-02 00:00:00.000000 nox-2023.4.22/tests/test_main.py
+-rw-r--r--   0        0        0    13208 2020-02-02 00:00:00.000000 nox-2023.4.22/tests/test_manifest.py
+-rw-r--r--   0        0        0     3576 2020-02-02 00:00:00.000000 nox-2023.4.22/tests/test_registry.py
+-rw-r--r--   0        0        0    36811 2020-02-02 00:00:00.000000 nox-2023.4.22/tests/test_sessions.py
+-rw-r--r--   0        0        0    20403 2020-02-02 00:00:00.000000 nox-2023.4.22/tests/test_tasks.py
+-rw-r--r--   0        0        0     6546 2020-02-02 00:00:00.000000 nox-2023.4.22/tests/test_tox_to_nox.py
+-rw-r--r--   0        0        0    24503 2020-02-02 00:00:00.000000 nox-2023.4.22/tests/test_virtualenv.py
+-rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 nox-2023.4.22/tests/test_workflow.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 nox-2023.4.22/tests/resources/noxfile.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 nox-2023.4.22/tests/resources/noxfile_multiple_sessions.py
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 nox-2023.4.22/tests/resources/noxfile_nested.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 nox-2023.4.22/tests/resources/noxfile_normalization.py
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 nox-2023.4.22/tests/resources/noxfile_options.py
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 nox-2023.4.22/tests/resources/noxfile_options_pythons.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 nox-2023.4.22/tests/resources/noxfile_pythons.py
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 nox-2023.4.22/tests/resources/noxfile_spaces.py
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 nox-2023.4.22/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 nox-2023.4.22/LICENSE
+-rw-r--r--   0        0        0     2793 2020-02-02 00:00:00.000000 nox-2023.4.22/README.md
+-rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 nox-2023.4.22/pyproject.toml
+-rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 nox-2023.4.22/PKG-INFO
```

### Comparing `nox-2022.8.7/LICENSE` & `nox-2023.4.22/LICENSE`

 * *Files identical despite different names*

### Comparing `nox-2022.8.7/PKG-INFO` & `nox-2023.4.22/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: nox
-Version: 2022.8.7
+Version: 2023.4.22
 Summary: Flexible test automation.
-Author: Alethea Katherine Flowers
-Author-email: me@thea.codes
-License: Apache-2.0
 Project-URL: bug-tracker, https://github.com/wntrblm/nox/issues
 Project-URL: documentation, https://nox.thea.codes
 Project-URL: homepage, https://github.com/wntrblm/nox
 Project-URL: repository, https://github.com/wntrblm/nox
+Author: Alethea Katherine Flowers
+Author-email: me@thea.codes
+License: Apache-2.0
+License-File: LICENSE
 Keywords: automation,testing,tox
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
@@ -21,19 +22,27 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Testing
 Requires-Python: >=3.7
-Description-Content-Type: text/markdown
+Requires-Dist: argcomplete<4.0,>=1.9.4
+Requires-Dist: colorlog<7.0.0,>=2.6.1
+Requires-Dist: importlib-metadata; python_version < '3.8'
+Requires-Dist: packaging>=20.9
+Requires-Dist: typing-extensions>=3.7.4; python_version < '3.8'
+Requires-Dist: virtualenv>=14
 Provides-Extra: tox_to_nox
-License-File: LICENSE
+Requires-Dist: jinja2; extra == 'tox_to_nox'
+Requires-Dist: tox<4; extra == 'tox_to_nox'
+Description-Content-Type: text/markdown
 
 <p align="center">
 <img src="https://github.com/wntrblm/nox/raw/main/docs/_static/alice.png" alt="logo" width=50%>
 </p>
 
 # Nox
```

### Comparing `nox-2022.8.7/README.md` & `nox-2023.4.22/README.md`

 * *Files identical despite different names*

### Comparing `nox-2022.8.7/nox/__init__.py` & `nox-2023.4.22/nox/__init__.py`

 * *Files identical despite different names*

### Comparing `nox-2022.8.7/nox/__main__.py` & `nox-2023.4.22/nox/__main__.py`

 * *Files identical despite different names*

### Comparing `nox-2022.8.7/nox/_decorators.py` & `nox-2023.4.22/nox/_decorators.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 
 from __future__ import annotations
 
 import copy
 import functools
 import inspect
 import types
-from typing import Any, Callable, Iterable, TypeVar, cast
+from typing import TYPE_CHECKING, Any, Callable, Iterable, TypeVar, cast
 
 from . import _typing
 
-if _typing.TYPE_CHECKING:
+if TYPE_CHECKING:
     from ._parametrize import Param
 
 
 class FunctionDecorator:
     def __new__(
         cls, func: Callable[..., Any], *args: Any, **kwargs: Any
     ) -> FunctionDecorator:
@@ -64,15 +64,15 @@
         tags: list[str] | None = None,
     ):
         self.func = func
         self.python = python
         self.reuse_venv = reuse_venv
         self.venv_backend = venv_backend
         self.venv_params = venv_params
-        self.should_warn = should_warn or dict()
+        self.should_warn = should_warn or {}
         self.tags = tags or []
 
     def __call__(self, *args: Any, **kwargs: Any) -> Any:
         return self.func(*args, **kwargs)
 
     def copy(self, name: str | None = None) -> Func:
         return Func(
```

### Comparing `nox-2022.8.7/nox/_option_set.py` & `nox-2023.4.22/nox/_option_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,14 +33,16 @@
 
     Args:
         name (str): The name used to refer to the group.
         args: Passed through to``ArgumentParser.add_argument_group``.
         kwargs: Passed through to``ArgumentParser.add_argument_group``.
     """
 
+    __slots__ = ("name", "args", "kwargs")
+
     def __init__(self, name: str, *args: Any, **kwargs: Any) -> None:
         self.name = name
         self.args = args
         self.kwargs = kwargs
 
 
 class Option:
@@ -195,17 +197,17 @@
     finalization, callable defaults, and strongly typed namespaces for tests.
     """
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         self.parser_args = args
         self.parser_kwargs = kwargs
         self.options: collections.OrderedDict[str, Option] = collections.OrderedDict()
-        self.groups: collections.OrderedDict[
-            str, OptionGroup
-        ] = collections.OrderedDict()
+        self.groups: collections.OrderedDict[str, OptionGroup] = (
+            collections.OrderedDict()
+        )
 
     def add_options(self, *args: Option) -> None:
         """Adds a sequence of Options to the OptionSet.
 
         Args:
             args (Sequence[Options])
         """
@@ -231,15 +233,15 @@
 
         groups = {
             name: parser.add_argument_group(*option_group.args, **option_group.kwargs)
             for name, option_group in self.groups.items()
         }
 
         for option in self.options.values():
-            if option.hidden is True:
+            if option.hidden:
                 continue
 
             # Every option must have a group (except for hidden options)
             if option.group is None:
                 raise ValueError(
                     f"Option {option.name} must either have a group or be hidden."
                 )
```

### Comparing `nox-2022.8.7/nox/_options.py` & `nox-2023.4.22/nox/_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from __future__ import annotations
 
 import argparse
 import functools
 import os
 import sys
-from typing import Any, Sequence
+from typing import Any, Callable, Sequence
 
 from nox import _option_set
 from nox.tasks import discover_manifest, filter_manifest, load_nox_module
 
 """All of Nox's configuration options."""
 
 options = _option_set.OptionSet(
@@ -44,16 +44,18 @@
         "python",
         "Python options",
         "These arguments are used to control which Python version(s) to use.",
     ),
     _option_set.OptionGroup(
         "environment",
         "Environment options",
-        "These arguments are used to control Nox's creation and usage of virtual"
-        " environments.",
+        (
+            "These arguments are used to control Nox's creation and usage of virtual"
+            " environments."
+        ),
     ),
     _option_set.OptionGroup(
         "execution",
         "Execution options",
         "These arguments are used to control execution of sessions.",
     ),
     _option_set.OptionGroup(
@@ -136,40 +138,50 @@
             command-line.
         noxfile_Args (_option_set.Namespace): The options specified in the
             Noxfile.
     """
     return command_args.envdir or noxfile_args.envdir or ".nox"
 
 
-def _sessions_default() -> list[str] | None:
-    """Looks at the NOXSESSION env var to set the default value for sessions."""
-    nox_env = os.environ.get("NOXSESSION")
-    env_sessions = nox_env.split(",") if nox_env else None
-    return env_sessions
+def default_env_var_list_factory(env_var: str) -> Callable[[], list[str] | None]:
+    """Looks at the env var to set the default value for a list of env vars.
+
+    Args:
+        env_var (str): The name of the environment variable to look up.
+
+    Returns:
+        A callback that retrieves a list from a comma-delimited environment variable.
+    """
+
+    def _default_list() -> list[str] | None:
+        env_value = os.environ.get(env_var)
+        return env_value.split(",") if env_value else None
+
+    return _default_list
 
 
 def _color_finalizer(value: bool, args: argparse.Namespace) -> bool:
     """Figures out the correct value for "color" based on the two color flags.
 
     Args:
         value (bool): The current value of the "color" option.
         args (_option_set.Namespace): The values for all options.
 
     Returns:
         The new value for the "color" option.
     """
-    if args.forcecolor is True and args.nocolor is True:
+    if args.forcecolor and args.nocolor:
         raise _option_set.ArgumentError(
             None, "Can not specify both --no-color and --force-color."
         )
 
-    if args.forcecolor is True:
+    if args.forcecolor:
         return True
 
-    if args.nocolor is True:
+    if args.nocolor:
         return False
 
     return sys.stdout.isatty()
 
 
 def _force_pythons_finalizer(
     value: Sequence[str], args: argparse.Namespace
@@ -213,14 +225,15 @@
     return posargs[dash_index + 1 :]
 
 
 def _session_completer(
     prefix: str, parsed_args: argparse.Namespace, **kwargs: Any
 ) -> list[str]:
     global_config = parsed_args
+    global_config.list_sessions = True
     module = load_nox_module(global_config)
     manifest = discover_manifest(module, global_config)
     filtered_manifest = filter_manifest(manifest, global_config)
     if isinstance(filtered_manifest, int):
         return []
     return [
         session.friendly_name for session, _ in filtered_manifest.list_all_sessions()
@@ -249,35 +262,43 @@
         "--list-sessions",
         "--list",
         group=options.groups["sessions"],
         action="store_true",
         help="List all available sessions and exit.",
     ),
     _option_set.Option(
+        "json",
+        "--json",
+        group=options.groups["sessions"],
+        action="store_true",
+        help="JSON output formatting. Requires list-sessions currently.",
+    ),
+    _option_set.Option(
         "sessions",
         "-s",
         "-e",
         "--sessions",
         "--session",
         group=options.groups["sessions"],
         noxfile=True,
         merge_func=functools.partial(_sessions_and_keywords_merge_func, "sessions"),
         nargs="*",
-        default=_sessions_default,
+        default=default_env_var_list_factory("NOXSESSION"),
         help="Which sessions to run. By default, all sessions will run.",
         completer=_session_completer,
     ),
     _option_set.Option(
         "pythons",
         "-p",
         "--pythons",
         "--python",
         group=options.groups["python"],
         noxfile=True,
         nargs="*",
+        default=default_env_var_list_factory("NOXPYTHON"),
         help="Only run sessions that use the given python interpreter versions.",
     ),
     _option_set.Option(
         "keywords",
         "-k",
         "--keywords",
         group=options.groups["sessions"],
@@ -400,22 +421,24 @@
     ),
     _option_set.Option(
         "extra_pythons",
         "--extra-pythons",
         "--extra-python",
         group=options.groups["python"],
         nargs="*",
+        default=default_env_var_list_factory("NOXEXTRAPYTHON"),
         help="Additionally, run sessions using the given python interpreter versions.",
     ),
     _option_set.Option(
         "force_pythons",
         "--force-pythons",
         "--force-python",
         group=options.groups["python"],
         nargs="*",
+        default=default_env_var_list_factory("NOXFORCEPYTHON"),
         help=(
             "Run sessions with the given interpreters instead of those listed in the"
             " Noxfile. This is a shorthand for ``--python=X.Y --extra-python=X.Y``."
         ),
         finalizer_func=_force_pythons_finalizer,
     ),
     *_option_set.make_flag_pair(
@@ -506,15 +529,15 @@
     ),
     # Stores the original working directory that Nox was invoked from,
     # since it could be different from the Noxfile's directory.
     _option_set.Option(
         "invoked_from",
         group=None,
         hidden=True,
-        default=lambda: os.getcwd(),
+        default=os.getcwd,
     ),
 )
 
 
 """Options that are configurable in the Noxfile.
 
 By setting properties on ``nox.options`` you can specify command line
```

### Comparing `nox-2022.8.7/nox/_parametrize.py` & `nox-2023.4.22/nox/_parametrize.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
     def __init__(
         self,
         *args: Any,
         arg_names: Sequence[str] | None = None,
         id: str | None = None,
     ) -> None:
-        self.args = tuple(args)
+        self.args = args
         self.id = id
 
         if arg_names is None:
             arg_names = ()
 
         self.arg_names = tuple(arg_names)
 
@@ -49,15 +49,15 @@
         return dict(zip(self.arg_names, self.args))
 
     def __str__(self) -> str:
         if self.id:
             return self.id
         else:
             call_spec = self.call_spec
-            args = [f"{k}={call_spec[k]!r}" for k in call_spec.keys()]
+            args = [f"{k}={call_spec[k]!r}" for k in call_spec]
             return ", ".join(args)
 
     __repr__ = __str__
 
     def copy(self) -> Param:
         new = self.__class__(*self.args, arg_names=self.arg_names, id=self.id)
         return new
```

### Comparing `nox-2022.8.7/nox/_version.py` & `nox-2023.4.22/nox/_version.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 class InvalidVersionSpecifier(Exception):
     """The ``nox.needs_version`` specifier cannot be parsed."""
 
 
 def get_nox_version() -> str:
     """Return the version of the installed Nox package."""
-    return metadata.version("nox")  # type: ignore[no-untyped-call, no-any-return]
+    return metadata.version("nox")
 
 
 def _parse_string_constant(node: ast.AST) -> str | None:  # pragma: no cover
     """Return the value of a string constant."""
     if sys.version_info < (3, 8):
         if isinstance(node, ast.Str) and isinstance(node.s, str):
             return node.s
@@ -82,15 +82,15 @@
     try:
         specifiers = SpecifierSet(needs_version)
     except InvalidSpecifier as error:
         message = f"Cannot parse `nox.needs_version`: {error}"
         with contextlib.suppress(InvalidVersion):
             Version(needs_version)
             message += f", did you mean '>= {needs_version}'?"
-        raise InvalidVersionSpecifier(message)
+        raise InvalidVersionSpecifier(message) from error
 
     if not specifiers.contains(version, prereleases=True):
         raise VersionCheckFailed(
             f"The Noxfile requires Nox {specifiers}, you have {version}"
         )
```

### Comparing `nox-2022.8.7/nox/command.py` & `nox-2023.4.22/nox/command.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,19 +12,18 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 import os
 import shlex
+import shutil
 import sys
 from typing import Any, Iterable, Sequence
 
-import py
-
 from nox.logger import logger
 from nox.popen import popen
 
 if sys.version_info < (3, 8):  # pragma: no cover
     from typing_extensions import Literal
 else:  # pragma: no cover
     from typing import Literal
@@ -36,26 +35,22 @@
     def __init__(self, reason: str | None = None) -> None:
         super().__init__(reason)
         self.reason = reason
 
 
 def which(program: str, paths: list[str] | None) -> str:
     """Finds the full path to an executable."""
-    full_path = None
-
-    if paths:
-        full_path = py.path.local.sysfind(program, paths=paths)
-
-    if full_path:
-        return full_path.strpath  # type: ignore[no-any-return]
-
-    full_path = py.path.local.sysfind(program)
+    if paths is not None:
+        full_path = shutil.which(program, path=os.pathsep.join(paths))
+        if full_path:
+            return full_path
 
+    full_path = shutil.which(program)
     if full_path:
-        return full_path.strpath  # type: ignore[no-any-return]
+        return full_path
 
     logger.error(f"Program {program} not found.")
     raise CommandFailed(f"Program {program} not found")
 
 
 def _clean_env(env: dict[str, str] | None) -> dict[str, str] | None:
     if env is None:
@@ -67,16 +62,15 @@
     clean_env["SYSTEMROOT"] = os.environ.get("SYSTEMROOT", "")
 
     clean_env.update(env)
     return clean_env
 
 
 def _shlex_join(args: Sequence[str]) -> str:
-    # shlex.join() was added in Python 3.8
-    return " ".join(shlex.quote(arg) for arg in args)
+    return " ".join(shlex.quote(os.fspath(arg)) for arg in args)
 
 
 def run(
     args: Sequence[str],
     *,
     env: dict[str, str] | None = None,
     silent: bool = False,
@@ -117,15 +111,15 @@
                     " external=True into run() to silence this message."
                 )
 
     env = _clean_env(env)
 
     try:
         return_code, output = popen(
-            [cmd_path] + list(args), silent=silent, env=env, **popen_kws
+            [cmd_path, *list(args)], silent=silent, env=env, **popen_kws
         )
 
         if return_code not in success_codes:
             suffix = ":" if silent else ""
             logger.error(
                 f"Command {full_cmd} failed with exit code {return_code}{suffix}"
             )
```

### Comparing `nox-2022.8.7/nox/logger.py` & `nox-2023.4.22/nox/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,31 +93,30 @@
 
 
 logging.setLoggerClass(LoggerWithSuccessAndOutput)
 logger = cast(LoggerWithSuccessAndOutput, logging.getLogger("nox"))
 
 
 def _get_formatter(color: bool, add_timestamp: bool) -> logging.Formatter:
-    if color is True:
+    if color:
         return NoxColoredFormatter(
             reset=True,
             log_colors={
                 "DEBUG": "cyan",
                 "INFO": "blue",
                 "WARNING": "yellow",
                 "ERROR": "red",
                 "CRITICAL": "red,bg_white",
                 "SUCCESS": "green",
             },
             style="%",
             secondary_log_colors=None,
             add_timestamp=add_timestamp,
         )
-    else:
-        return NoxFormatter(add_timestamp=add_timestamp)
+    return NoxFormatter(add_timestamp=add_timestamp)
 
 
 def setup_logging(
     color: bool, verbose: bool = False, add_timestamp: bool = False
 ) -> None:  # pragma: no cover
     """Setup logging.
```

### Comparing `nox-2022.8.7/nox/manifest.py` & `nox-2023.4.22/nox/manifest.py`

 * *Files 2% similar despite different names*

```diff
@@ -229,15 +229,14 @@
                 # Otherwise, add the extra specified python.
                 assert isinstance(func.python, str)
                 func.python = _unique_list(func.python, *extra_pythons)
 
         # If the func has the python attribute set to a list, we'll need
         # to expand them.
         if isinstance(func.python, (list, tuple, set)):
-
             for python in func.python:
                 single_func = func.copy()
                 single_func.python = python
                 sessions.extend(self.make_session(name, single_func, multi=True))
 
             return sessions
 
@@ -250,15 +249,15 @@
             if func.python:
                 long_names.append(f"{name}-{func.python}")
 
             return [SessionRunner(name, long_names, func, self._config, self)]
 
         # Since this function is parametrized, we need to add a distinct
         # session for each permutation.
-        parametrize = func.parametrize  # type: ignore[attr-defined]
+        parametrize = func.parametrize
         calls = Call.generate_calls(func, parametrize)
         for call in calls:
             long_names = []
             if not multi:
                 long_names.append(f"{name}{call.session_signature}")
             if func.python:
                 long_names.append(f"{name}-{func.python}{call.session_signature}")
@@ -329,30 +328,27 @@
     returns False.
     """
 
     def __init__(self, keywords: set[str]) -> None:
         self._keywords = keywords
 
     def __getitem__(self, variable_name: str) -> bool:
-        for keyword in self._keywords:
-            if variable_name in keyword:
-                return True
-        return False
+        return any(variable_name in keyword for keyword in self._keywords)
 
     def __iter__(self) -> Iterator[str]:
         return iter(self._keywords)
 
     def __len__(self) -> int:
         return len(self._keywords)
 
 
 def keyword_match(expression: str, keywords: Iterable[str]) -> Any:
     """See if an expression matches the given set of keywords."""
     locals = KeywordLocals(set(keywords))
-    return eval(expression, {}, locals)
+    return eval(expression, {}, locals)  # noqa: PGH001
 
 
 def _null_session_func_(session: Session) -> None:
     """A no-op session for patemetrized sessions with no available params."""
     session.skip("This session had no parameters available.")
```

### Comparing `nox-2022.8.7/nox/popen.py` & `nox-2023.4.22/nox/popen.py`

 * *Files identical despite different names*

### Comparing `nox-2022.8.7/nox/registry.py` & `nox-2023.4.22/nox/registry.py`

 * *Files identical despite different names*

### Comparing `nox-2022.8.7/nox/sessions.py` & `nox-2023.4.22/nox/sessions.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,36 +11,57 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 import argparse
+import contextlib
 import enum
 import hashlib
 import os
 import pathlib
 import re
 import sys
 import unicodedata
 from types import TracebackType
-from typing import Any, Callable, Iterable, Mapping, Sequence
-
-import py
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Generator,
+    Iterable,
+    Mapping,
+    NoReturn,
+    Sequence,
+)
 
 import nox.command
-from nox import _typing
 from nox._decorators import Func
 from nox.logger import logger
 from nox.virtualenv import CondaEnv, PassthroughEnv, ProcessEnv, VirtualEnv
 
-if _typing.TYPE_CHECKING:
+if TYPE_CHECKING:
     from nox.manifest import Manifest
 
 
+@contextlib.contextmanager
+def _chdir(path: str) -> Generator[None, None, None]:
+    """
+    Change the current working directory to the given path.
+    Follows python 3.11's chdir behaviour.
+    """
+    cwd = os.getcwd()
+    try:
+        os.chdir(path)
+        yield
+    finally:
+        os.chdir(cwd)
+
+
 def _normalize_path(envdir: str, path: str | bytes) -> str:
     """Normalizes a string to be a "safe" filesystem path for a virtualenv."""
     if isinstance(path, bytes):
         path = path.decode("utf-8")
 
     path = unicodedata.normalize("NFKD", path).encode("ascii", "ignore")
     path = path.decode("ascii")
@@ -68,19 +89,19 @@
     """Double-quote package install arguments in case they contain '>' or '<' symbols"""
 
     # routine used to handle a single arg
     def _dblquote_pkg_install_arg(pkg_req_str: str) -> str:
         # sanity check: we need an even number of double-quotes
         if pkg_req_str.count('"') % 2 != 0:
             raise ValueError(
-                f"ill-formated argument with odd number of quotes: {pkg_req_str}"
+                f"ill-formatted argument with odd number of quotes: {pkg_req_str}"
             )
 
         if "<" in pkg_req_str or ">" in pkg_req_str:
-            if pkg_req_str[0] == '"' and pkg_req_str[-1] == '"':
+            if pkg_req_str[0] == pkg_req_str[-1] == '"':
                 # already double-quoted string
                 return pkg_req_str
             else:
                 # need to double-quote string
                 if '"' in pkg_req_str:
                     raise ValueError(f"Cannot escape requirement string: {pkg_req_str}")
                 return f'"{pkg_req_str}"'
@@ -242,15 +263,15 @@
     ) -> Any:
         """Legacy support for running a function through :func`run`."""
         self.log(f"{func}(args={args!r}, kwargs={kwargs!r})")
         try:
             return func(*args, **kwargs)
         except Exception as e:
             logger.exception(f"Function {func!r} raised {e!r}.")
-            raise nox.command.CommandFailed()
+            raise nox.command.CommandFailed() from e
 
     def run(
         self, *args: str, env: Mapping[str, str] | None = None, **kwargs: Any
     ) -> Any | None:
         """Run a command.
 
         Commands must be specified as a list of strings, for example::
@@ -299,14 +320,24 @@
 
            try:
                session.run("coverage", "run", "-m", "pytest")
            finally:
                # Display coverage report even when tests fail.
                session.run("coverage", "report")
 
+        If you pass ``silent=True``, you can capture the output of a command that would
+        otherwise be shown to the user. For example to get the current Git commit ID::
+
+            out = session.run(
+                "git", "rev-parse", "--short", "HEAD",
+                external=True, silent=True
+            )
+
+            print("Current Git commit is", out.strip())
+
         :param env: A dictionary of environment variables to expose to the
             command. By default, all environment variables are passed.
         :type env: dict or None
         :param bool silent: Silence command output, unless the command fails.
             If ``True``, returns the command output (unless the command fails).
             ``False`` by default.
         :param success_codes: A list of return codes that are considered
@@ -324,14 +355,20 @@
             Default: ``0.3``
         :type interrupt_timeout: float or None
         :param terminate_timeout: The timeout (in seconds) that Nox should wait after it
             sends a terminate signal to its children before sending a kill signal to
             them. Set to ``None`` to never send a kill signal.
             Default: ``0.2``
         :type terminate_timeout: float or None
+        :param stdout: Redirect standard output of the command into a file. Can't be
+            combined with *silent*.
+        :type stdout: file or file descriptor
+        :param stderr: Redirect standard output of the command into a file. Can't be
+            combined with *silent*.
+        :type stderr: file or file descriptor
         """
         if not args:
             raise ValueError("At least one argument required to run().")
 
         if self._runner.global_config.install_only:
             logger.info(f"Skipping {args[0]} run, as --install-only is set.")
             return None
@@ -449,15 +486,15 @@
         To install the current package without clobbering conda-installed
         dependencies::
 
             session.install('.', '--no-deps')
             # Install in editable mode.
             session.install('-e', '.', '--no-deps')
 
-        You can specify a conda channel using `channel=`; a falsy value will
+        You can specify a conda channel using `channel=`; a falsey value will
         not change the current channels. You can specify a list of channels if
         needed.
 
         Additional keyword args are the same as for :meth:`run`.
 
         .. _conda install:
         """
@@ -611,19 +648,19 @@
         """Outputs a warning during the session."""
         logger.warning(*args, **kwargs)
 
     def debug(self, *args: Any, **kwargs: Any) -> None:
         """Outputs a debug-level message during the session."""
         logger.debug(*args, **kwargs)
 
-    def error(self, *args: Any) -> _typing.NoReturn:
+    def error(self, *args: Any) -> NoReturn:
         """Immediately aborts the session and optionally logs an error."""
         raise _SessionQuit(*args)
 
-    def skip(self, *args: Any) -> _typing.NoReturn:
+    def skip(self, *args: Any) -> NoReturn:
         """Immediately skips the session and optionally logs a warning."""
         raise _SessionSkip(*args)
 
 
 class SessionRunner:
     def __init__(
         self,
@@ -711,21 +748,17 @@
 
         self.venv.create()
 
     def execute(self) -> Result:
         logger.warning(f"Running session {self.friendly_name}")
 
         try:
-            # By default, Nox should quietly change to the directory where
-            # the noxfile.py file is located.
-            cwd = py.path.local(
-                os.path.realpath(os.path.dirname(self.global_config.noxfile))
-            ).as_cwd()
+            cwd = os.path.realpath(os.path.dirname(self.global_config.noxfile))
 
-            with cwd:
+            with _chdir(cwd):
                 self._create_venv()
                 session = Session(self)
                 session.env["NOX_CURRENT_SESSION"] = session.name
                 self.func(session)
 
             # Nothing went wrong; return a success.
             return Result(self, Status.SUCCESS)
@@ -786,19 +819,20 @@
         """Return the English imperfect tense for the status.
 
         Returns:
             str: A word or phrase representing the status.
         """
         if self.status == Status.SUCCESS:
             return "was successful"
+
         status = self.status.name.lower()
         if self.reason:
             return f"{status}: {self.reason}"
-        else:
-            return status
+
+        return status
 
     def log(self, message: str) -> None:
         """Log a message using the appropriate log function.
 
         Args:
             message (str): The message to be logged.
         """
```

### Comparing `nox-2022.8.7/nox/tasks.py` & `nox-2023.4.22/nox/tasks.py`

 * *Files 3% similar despite different names*

```diff
@@ -175,14 +175,15 @@
     if global_config.sessions is not None:
         try:
             manifest.filter_by_name(global_config.sessions)
         except KeyError as exc:
             logger.error("Error while collecting sessions.")
             logger.error(exc.args[0])
             return 3
+
     if not manifest and not global_config.list_sessions:
         print("No sessions selected. Please select a session with -s <session name>.\n")
         _produce_listing(manifest, global_config)
         return 0
 
     # Filter by python interpreter versions.
     if global_config.pythons:
@@ -260,29 +261,54 @@
 
     print(
         f"\nsessions marked with {selected_color}*{reset} are selected, sessions marked"
         f" with {skipped_color}-{reset} are skipped."
     )
 
 
+def _produce_json_listing(manifest: Manifest, global_config: Namespace) -> None:
+    report = []
+    for session, selected in manifest.list_all_sessions():
+        if selected:
+            report.append(
+                {
+                    "session": session.friendly_name,
+                    "name": session.name,
+                    "description": session.description or "",
+                    "python": session.func.python,
+                    "tags": session.tags,
+                    "call_spec": getattr(session.func, "call_spec", {}),
+                }
+            )
+    print(json.dumps(report))
+
+
 def honor_list_request(manifest: Manifest, global_config: Namespace) -> Manifest | int:
     """If --list was passed, simply list the manifest and exit cleanly.
 
     Args:
         manifest (~.Manifest): The manifest of sessions to be run.
         global_config (~nox.main.GlobalConfig): The global configuration.
 
     Returns:
         Union[~.Manifest,int]: ``0`` if a listing is all that is requested,
             the manifest otherwise (to be sent to the next task).
     """
-    if not global_config.list_sessions:
+    if not (global_config.list_sessions or global_config.json):
         return manifest
 
-    _produce_listing(manifest, global_config)
+    # JSON output requires list sessions also be specified
+    if global_config.json and not global_config.list_sessions:
+        logger.error("Must specify --list-sessions with --json")
+        return 3
+
+    if global_config.json:
+        _produce_json_listing(manifest, global_config)
+    else:
+        _produce_listing(manifest, global_config)
 
     return 0
 
 
 def run_manifest(manifest: Manifest, global_config: Namespace) -> list[Result]:
     """Run the full manifest of sessions.
```

### Comparing `nox-2022.8.7/nox/tox_to_nox.jinja2` & `nox-2023.4.22/nox/tox_to_nox.jinja2`

 * *Files identical despite different names*

### Comparing `nox-2022.8.7/nox/tox_to_nox.py` & `nox-2023.4.22/nox/tox_to_nox.py`

 * *Files identical despite different names*

### Comparing `nox-2022.8.7/nox/virtualenv.py` & `nox-2023.4.22/nox/virtualenv.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,30 +10,28 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
+import contextlib
 import os
 import platform
 import re
 import shutil
+import subprocess
 import sys
 from socket import gethostbyname
-from typing import Any, Mapping
-
-import py
+from typing import Any, ClassVar, Mapping
 
 import nox
 import nox.command
 from nox.logger import logger
 
-from . import _typing
-
 # Problematic environment variables that are stripped from all commands inside
 # of a virtualenv. See https://github.com/theacodes/nox/issues/44
 _BLACKLISTED_ENV_VARS = frozenset(
     ["PIP_RESPECT_VIRTUALENV", "PIP_REQUIRE_VIRTUALENV", "__PYVENV_LAUNCHER__"]
 )
 _SYSTEM = platform.system()
 _ENABLE_STALENESS_CHECK = "NOX_ENABLE_STALENESS_CHECK" in os.environ
@@ -42,23 +40,23 @@
 class InterpreterNotFound(OSError):
     def __init__(self, interpreter: str) -> None:
         super().__init__(f"Python interpreter {interpreter} not found")
         self.interpreter = interpreter
 
 
 class ProcessEnv:
-    """A environment with a 'bin' directory and a set of 'env' vars."""
+    """An environment with a 'bin' directory and a set of 'env' vars."""
 
     location: str
 
     # Does this environment provide any process isolation?
     is_sandboxed = False
 
     # Special programs that aren't included in the environment.
-    allowed_globals: _typing.ClassVar[tuple[Any, ...]] = ()
+    allowed_globals: ClassVar[tuple[Any, ...]] = ()
 
     def __init__(
         self, bin_paths: None = None, env: Mapping[str, str] | None = None
     ) -> None:
         self._bin_paths = bin_paths
         self.env = os.environ.copy()
         self._reused = False
@@ -67,15 +65,15 @@
             self.env.update(env)
 
         for key in _BLACKLISTED_ENV_VARS:
             self.env.pop(key, None)
 
         if self.bin_paths:
             self.env["PATH"] = os.pathsep.join(
-                self.bin_paths + [self.env.get("PATH", "")]
+                [*self.bin_paths, self.env.get("PATH", "")]
             )
 
     @property
     def bin_paths(self) -> list[str] | None:
         return self._bin_paths
 
     @property
@@ -105,20 +103,24 @@
             be ``py -3.6-32``.
 
     Returns:
         Optional[str]: The full executable path for the Python ``version``,
         if it is found.
     """
     script = "import sys; print(sys.executable)"
-    py_exe = py.path.local.sysfind("py")
+    py_exe = shutil.which("py")
     if py_exe is not None:
-        try:
-            return py_exe.sysexec("-" + version, "-c", script).strip()  # type: ignore[no-any-return]
-        except py.process.cmdexec.Error:
-            return None
+        ret = subprocess.run(
+            [py_exe, f"-{version}", "-c", script],
+            check=False,
+            text=True,
+            capture_output=True,
+        )
+        if ret.returncode == 0 and ret.stdout:
+            return ret.stdout.strip()
     return None
 
 
 def locate_using_path_and_version(version: str) -> str | None:
     """Check the PATH's python interpreter and return it if the version
     matches.
 
@@ -134,23 +136,25 @@
         Optional[str]: The full executable path for the Python ``version``,
         if it is found.
     """
     if not version:
         return None
 
     script = "import platform; print(platform.python_version())"
-    path_python = py.path.local.sysfind("python")
+    path_python = shutil.which("python")
     if path_python:
-        try:
-            prefix = f"{version}."
-            version_string = path_python.sysexec("-c", script).strip()
-            if version_string.startswith(prefix):
-                return str(path_python)
-        except py.process.cmdexec.Error:
-            return None
+        prefix = f"{version}"
+        ret = subprocess.run(
+            [path_python, "-c", script],
+            check=False,
+            text=True,
+            capture_output=True,
+        )
+        if ret.returncode == 0 and ret.stdout and ret.stdout.strip().startswith(prefix):
+            return path_python
 
     return None
 
 
 class PassthroughEnv(ProcessEnv):
     """Represents the environment used to run Nox itself
 
@@ -199,15 +203,15 @@
         *,
         conda_cmd: str = "conda",
     ):
         self.location_name = location
         self.location = os.path.abspath(location)
         self.interpreter = interpreter
         self.reuse_existing = reuse_existing
-        self.venv_params = venv_params if venv_params else []
+        self.venv_params = venv_params or []
         self.conda_cmd = conda_cmd
         super().__init__(env={"CONDA_PREFIX": self.location})
 
     def _clean_location(self) -> bool:
         """Deletes existing conda environment"""
         if os.path.exists(self.location):
             if self.reuse_existing:
@@ -219,18 +223,16 @@
                     "--yes",
                     "--prefix",
                     self.location,
                     "--all",
                 ]
                 nox.command.run(cmd, silent=True, log=False)
                 # Make sure that location is clean
-                try:
+                with contextlib.suppress(FileNotFoundError):
                     shutil.rmtree(self.location)
-                except FileNotFoundError:
-                    pass
 
         return True
 
     @property
     def bin_paths(self) -> list[str]:
         """Returns the location of the conda env's bin folder."""
         # see https://github.com/conda/conda/blob/f60f0f1643af04ed9a51da3dd4fa242de81e32f4/conda/activate.py#L563-L572
@@ -239,16 +241,16 @@
                 self.location,
                 os.path.join(self.location, "Library", "mingw-w64", "bin"),
                 os.path.join(self.location, "Library", "usr", "bin"),
                 os.path.join(self.location, "Library", "bin"),
                 os.path.join(self.location, "Scripts"),
                 os.path.join(self.location, "bin"),
             ]
-        else:
-            return [os.path.join(self.location, "bin")]
+
+        return [os.path.join(self.location, "bin")]
 
     def create(self) -> bool:
         """Create the conda env."""
         if not self._clean_location():
             logger.debug(f"Re-using existing conda env at {self.location_name}.")
 
             self._reused = True
@@ -258,18 +260,15 @@
         cmd = [self.conda_cmd, "create", "--yes", "--prefix", self.location]
 
         cmd.extend(self.venv_params)
 
         # Ensure the pip package is installed.
         cmd.append("pip")
 
-        if self.interpreter:
-            python_dep = f"python={self.interpreter}"
-        else:
-            python_dep = "python"
+        python_dep = f"python={self.interpreter}" if self.interpreter else "python"
         cmd.append(python_dep)
 
         logger.info(f"Creating conda env in {self.location_name} with {python_dep}")
         nox.command.run(cmd, silent=True, log=nox.options.verbose or False)
 
         return True
 
@@ -324,15 +323,15 @@
     ):
         self.location_name = location
         self.location = os.path.abspath(location)
         self.interpreter = interpreter
         self._resolved: None | str | InterpreterNotFound = None
         self.reuse_existing = reuse_existing
         self.venv_or_virtualenv = "venv" if venv else "virtualenv"
-        self.venv_params = venv_params if venv_params else []
+        self.venv_params = venv_params or []
         super().__init__(env={"VIRTUAL_ENV": self.location})
 
     def _clean_location(self) -> bool:
         """Deletes any existing virtual environment"""
         if os.path.exists(self.location):
             if self.reuse_existing and not _ENABLE_STALENESS_CHECK:
                 return False
@@ -420,15 +419,15 @@
         # part and add Python to the front of it.
         match = re.match(r"^(?P<xy_ver>\d(\.\d+)?)(\.\d+)?$", self.interpreter)
         if match:
             xy_version = match.group("xy_ver")
             cleaned_interpreter = f"python{xy_version}"
 
         # If the cleaned interpreter is on the PATH, go ahead and return it.
-        if py.path.local.sysfind(cleaned_interpreter):
+        if shutil.which(cleaned_interpreter):
             self._resolved = cleaned_interpreter
             return self._resolved
 
         # The rest of this is only applicable to Windows, so if we don't have
         # an interpreter by now, raise.
         if _SYSTEM != "Windows":
             self._resolved = InterpreterNotFound(self.interpreter)
@@ -457,16 +456,15 @@
         raise self._resolved
 
     @property
     def bin_paths(self) -> list[str]:
         """Returns the location of the virtualenv's bin folder."""
         if _SYSTEM == "Windows":
             return [os.path.join(self.location, "Scripts")]
-        else:
-            return [os.path.join(self.location, "bin")]
+        return [os.path.join(self.location, "bin")]
 
     def create(self) -> bool:
         """Create the virtualenv or venv."""
         if not self._clean_location():
             logger.debug(
                 f"Re-using existing virtual environment at {self.location_name}."
             )
```

### Comparing `nox-2022.8.7/nox/workflow.py` & `nox-2023.4.22/nox/workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         for function_ in workflow:
             # Send the previous task's return value if there was one.
             args: list[Any] = []
             if return_value is not None:
                 args.append(return_value)
             return_value = function_(*args, global_config=global_config)
 
-            # If we got a integer value as a result, abort task processing
+            # If we got an integer value as a result, abort task processing
             # and return it.
             if isinstance(return_value, int):
                 return return_value
 
         # All tasks completed, presumably without error.
         return 0
     except KeyboardInterrupt:
```

### Comparing `nox-2022.8.7/tests/resources/noxfile.py` & `nox-2023.4.22/tests/resources/noxfile.py`

 * *Files identical despite different names*

### Comparing `nox-2022.8.7/tests/resources/noxfile_multiple_sessions.py` & `nox-2023.4.22/tests/resources/noxfile_multiple_sessions.py`

 * *Files identical despite different names*

### Comparing `nox-2022.8.7/tests/resources/noxfile_nested.py` & `nox-2023.4.22/tests/resources/noxfile_nested.py`

 * *Files identical despite different names*

### Comparing `nox-2022.8.7/tests/resources/noxfile_options.py` & `nox-2023.4.22/tests/resources/noxfile_options.py`

 * *Files identical despite different names*

### Comparing `nox-2022.8.7/tests/resources/noxfile_options_pythons.py` & `nox-2023.4.22/tests/resources/noxfile_options_pythons.py`

 * *Files identical despite different names*

### Comparing `nox-2022.8.7/tests/resources/noxfile_spaces.py` & `nox-2023.4.22/tests/resources/noxfile_spaces.py`

 * *Files identical despite different names*

### Comparing `nox-2022.8.7/tests/test__option_set.py` & `nox-2023.4.22/tests/test__option_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
                 "option_a", group=optionset.groups["group_a"], default="meep"
             )
         )
 
         namespace = optionset.namespace()
 
         assert hasattr(namespace, "option_a")
-        assert not hasattr(namespace, "non_existant_option")
+        assert not hasattr(namespace, "non_existent_option")
         assert namespace.option_a == "meep"
 
     def test_namespace_values(self):
         optionset = _option_set.OptionSet()
         optionset.add_groups(_option_set.OptionGroup("group_a"))
         optionset.add_options(
             _option_set.Option(
@@ -52,19 +52,19 @@
             )
         )
 
         namespace = optionset.namespace(option_a="moop")
 
         assert namespace.option_a == "moop"
 
-    def test_namespace_non_existant_options_with_values(self):
+    def test_namespace_non_existent_options_with_values(self):
         optionset = _option_set.OptionSet()
 
         with pytest.raises(KeyError):
-            optionset.namespace(non_existant_option="meep")
+            optionset.namespace(non_existent_option="meep")
 
     def test_parser_hidden_option(self):
         optionset = _option_set.OptionSet()
         optionset.add_options(
             _option_set.Option(
                 "oh_boy_i_am_hidden", hidden=True, group=None, default="meep"
             )
```

### Comparing `nox-2022.8.7/tests/test__parametrize.py` & `nox-2023.4.22/tests/test__parametrize.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,14 @@
         {"abc": 2, "def": "b", "foo": "bar"},
         {"abc": 1, "def": "a", "foo": "baz"},
         {"abc": 2, "def": "b", "foo": "baz"},
     ]
 
 
 def test_generate_calls_simple():
-
     f = mock.Mock()
     f.__name__ = "f"
     f.some_prop = 42
 
     arg_names = ("abc",)
     call_specs = [
         _parametrize.Param(1, arg_names=arg_names),
@@ -195,15 +194,14 @@
     # Make sure wrapping was done correctly.
     for call in calls:
         assert call.some_prop == 42
         assert call.__name__ == "f"
 
 
 def test_generate_calls_multiple_args():
-
     f = mock.Mock()
     f.__name__ = "f"
 
     arg_names = ("foo", "abc")
     call_specs = [
         _parametrize.Param("a", 1, arg_names=arg_names),
         _parametrize.Param("b", 2, arg_names=arg_names),
```

### Comparing `nox-2022.8.7/tests/test__version.py` & `nox-2023.4.22/tests/test__version.py`

 * *Files identical despite different names*

### Comparing `nox-2022.8.7/tests/test_action_helper.py` & `nox-2023.4.22/tests/test_action_helper.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 sys.path.insert(0, str(GITHUB_FOLDER))
 from action_helper import filter_version, setup_action  # noqa: E402
 
 VALID_VERSIONS = {
     "2.7.18": "2.7",
     "3.9-dev": "3.9",
     "3.10": "3.10",
-    "3.11.0.beta1": "3.11",
+    "3.11": "3.11",
     "pypy-3.7": "3.7",
     "pypy-3.8-v7.3.9": "3.8",
     "pypy-3.9": "3.9",
     "pypy3.10": "3.10",
 }
 
 
@@ -38,52 +38,54 @@
 
 def test_filter_version_invalid_minor():
     with pytest.raises(ValueError, match=r"invalid minor python version: 3.x"):
         filter_version("3.x")
 
 
 VALID_VERSION_LISTS = {
-    "3.7, 3.8, 3.9, 3.10, pypy-3.7, pypy-3.8, pypy-3.9": [
-        "::set-output name=interpreter_count::7",
-        "::set-output name=interpreter_0::pypy-3.7",
-        "::set-output name=interpreter_1::pypy-3.8",
-        "::set-output name=interpreter_2::pypy-3.9",
-        "::set-output name=interpreter_3::3.7",
-        "::set-output name=interpreter_4::3.8",
-        "::set-output name=interpreter_5::3.9",
-        "::set-output name=interpreter_6::3.10",
+    "3.7, 3.8, 3.9, 3.10, 3.11, pypy-3.7, pypy-3.8, pypy-3.9": [
+        "interpreter_count=8",
+        "interpreter_0=pypy-3.7",
+        "interpreter_1=pypy-3.8",
+        "interpreter_2=pypy-3.9",
+        "interpreter_3=3.7",
+        "interpreter_4=3.8",
+        "interpreter_5=3.9",
+        "interpreter_6=3.10",
+        "interpreter_7=3.11",
     ],
     "": [
-        "::set-output name=interpreter_count::1",
-        "::set-output name=interpreter_0::3.10",
+        "interpreter_count=1",
+        "interpreter_0=3.11",
     ],
-    "3.10.4": [
-        "::set-output name=interpreter_count::1",
-        "::set-output name=interpreter_0::3.10.4",
+    "3.11.4": [
+        "interpreter_count=1",
+        "interpreter_0=3.11.4",
     ],
     "3.9-dev,pypy3.9-nightly": [
-        "::set-output name=interpreter_count::3",
-        "::set-output name=interpreter_0::pypy3.9-nightly",
-        "::set-output name=interpreter_1::3.9-dev",
-        "::set-output name=interpreter_2::3.10",
+        "interpreter_count=3",
+        "interpreter_0=pypy3.9-nightly",
+        "interpreter_1=3.9-dev",
+        "interpreter_2=3.11",
     ],
-    "3.10, 3.9, 3.8": [
-        "::set-output name=interpreter_count::3",
-        "::set-output name=interpreter_0::3.9",
-        "::set-output name=interpreter_1::3.8",
-        "::set-output name=interpreter_2::3.10",
+    "3.11, 3.10, 3.9, 3.8": [
+        "interpreter_count=4",
+        "interpreter_0=3.10",
+        "interpreter_1=3.9",
+        "interpreter_2=3.8",
+        "interpreter_3=3.11",
     ],
-    ",".join(f"3.{minor}" for minor in range(20)): [
-        "::set-output name=interpreter_count::20"
-    ]
-    + [
-        f"::set-output name=interpreter_{i}::3.{minor}"
-        for i, minor in enumerate(minor_ for minor_ in range(20) if minor_ != 10)
-    ]
-    + ["::set-output name=interpreter_19::3.10"],
+    ",".join(f"3.{minor}" for minor in range(20)): (
+        ["interpreter_count=20"]
+        + [
+            f"interpreter_{i}=3.{minor}"
+            for i, minor in enumerate(minor_ for minor_ in range(20) if minor_ != 11)
+        ]
+        + ["interpreter_19=3.11"]
+    ),
 }
 
 
 @pytest.mark.parametrize("version_list", VALID_VERSION_LISTS.keys())
 def test_setup_action(capsys, version_list):
     setup_action(version_list)
     captured = capsys.readouterr()
```

### Comparing `nox-2022.8.7/tests/test_command.py` & `nox-2023.4.22/tests/test_command.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,18 +14,20 @@
 
 from __future__ import annotations
 
 import ctypes
 import logging
 import os
 import platform
+import shutil
 import signal
 import subprocess
 import sys
 import time
+from pathlib import Path
 from textwrap import dedent
 from unittest import mock
 
 import pytest
 
 import nox.command
 import nox.popen
@@ -53,14 +55,21 @@
 
     out, _ = capsys.readouterr()
 
     assert "123" in result
     assert out == ""
 
 
+@pytest.mark.skipif(shutil.which("git") is None, reason="Needs git")
+def test_run_not_in_path(capsys):
+    # Paths falls back on the environment PATH if the command is not found.
+    result = nox.command.run(["git", "--version"], paths=["."])
+    assert result is True
+
+
 def test_run_verbosity(capsys, caplog):
     caplog.clear()
     with caplog.at_level(logging.DEBUG):
         result = nox.command.run([PYTHON, "-c", "print(123)"], silent=True)
 
         out, _ = capsys.readouterr()
 
@@ -108,14 +117,27 @@
         assert "123" in err
         assert out == ""
 
     # Nothing is logged but the error is still written to stderr
     assert not logs
 
 
+@pytest.mark.skipif(
+    platform.system() == "Windows",
+    reason="See https://github.com/python/cpython/issues/85815",
+)
+def test_run_non_str():
+    result = nox.command.run(
+        [Path(PYTHON), "-c", "import sys; print(sys.argv)", Path(PYTHON)],
+        silent=True,
+    )
+
+    assert PYTHON in result
+
+
 def test_run_env_unicode():
     result = nox.command.run(
         [PYTHON, "-c", 'import os; print(os.environ["SIGIL"])'],
         silent=True,
         env={"SIGIL": "123"},
     )
 
@@ -143,23 +165,27 @@
         silent=True,
         paths=["/non/existent"],
     )
 
     assert "/non/existent" not in result
 
 
-def test_run_path_existent(tmpdir, monkeypatch):
-    executable = tmpdir.join("testexc")
-    executable.ensure("")
+def test_run_path_existent(tmp_path: Path):
+    executable_name = (
+        "testexc.exe" if "windows" in platform.platform().lower() else "testexc"
+    )
+    tmp_path.touch()
+    executable = tmp_path.joinpath(executable_name)
+    executable.touch()
     executable.chmod(0o700)
 
     with mock.patch("nox.command.popen") as mock_command:
         mock_command.return_value = (0, "")
-        nox.command.run(["testexc"], silent=True, paths=[tmpdir.strpath])
-        mock_command.assert_called_with([executable.strpath], env=None, silent=True)
+        nox.command.run([executable_name], silent=True, paths=[str(tmp_path)])
+        mock_command.assert_called_with([str(executable)], env=None, silent=True)
 
 
 def test_run_external_warns(tmpdir, caplog):
     caplog.set_level(logging.WARNING)
 
     nox.command.run([PYTHON, "--version"], silent=True, paths=[tmpdir.strpath])
 
@@ -200,16 +226,18 @@
 
 def test_fail_with_silent(capsys):
     with pytest.raises(nox.command.CommandFailed):
         nox.command.run(
             [
                 PYTHON,
                 "-c",
-                'import sys; sys.stdout.write("out");'
-                'sys.stderr.write("err"); sys.exit(1)',
+                (
+                    'import sys; sys.stdout.write("out");'
+                    'sys.stderr.write("err"); sys.exit(1)'
+                ),
             ],
             silent=True,
         )
         out, err = capsys.readouterr()
         assert "out" in err
         assert "err" in err
 
@@ -360,44 +388,48 @@
 
 def test_custom_stdout(capsys, tmpdir):
     with open(str(tmpdir / "out.txt"), "w+b") as stdout:
         nox.command.run(
             [
                 PYTHON,
                 "-c",
-                'import sys; sys.stdout.write("out");'
-                'sys.stderr.write("err"); sys.exit(0)',
+                (
+                    'import sys; sys.stdout.write("out");'
+                    'sys.stderr.write("err"); sys.exit(0)'
+                ),
             ],
             stdout=stdout,
         )
         out, err = capsys.readouterr()
         assert not out
         assert "out" not in err
         assert "err" not in err
         stdout.seek(0)
         tempfile_contents = stdout.read().decode("utf-8")
         assert "out" in tempfile_contents
         assert "err" in tempfile_contents
 
 
 def test_custom_stdout_silent_flag(capsys, tmpdir):
-    with open(str(tmpdir / "out.txt"), "w+b") as stdout:
+    with open(str(tmpdir / "out.txt"), "w+b") as stdout:  # noqa: SIM117
         with pytest.raises(ValueError, match="silent"):
             nox.command.run([PYTHON, "-c", 'print("hi")'], stdout=stdout, silent=True)
 
 
 def test_custom_stdout_failed_command(capsys, tmpdir):
     with open(str(tmpdir / "out.txt"), "w+b") as stdout:
         with pytest.raises(nox.command.CommandFailed):
             nox.command.run(
                 [
                     PYTHON,
                     "-c",
-                    'import sys; sys.stdout.write("out");'
-                    'sys.stderr.write("err"); sys.exit(1)',
+                    (
+                        'import sys; sys.stdout.write("out");'
+                        'sys.stderr.write("err"); sys.exit(1)'
+                    ),
                 ],
                 stdout=stdout,
             )
         out, err = capsys.readouterr()
         assert not out
         assert "out" not in err
         assert "err" not in err
@@ -409,16 +441,18 @@
 
 def test_custom_stderr(capsys, tmpdir):
     with open(str(tmpdir / "err.txt"), "w+b") as stderr:
         nox.command.run(
             [
                 PYTHON,
                 "-c",
-                'import sys; sys.stdout.write("out");'
-                'sys.stderr.write("err"); sys.exit(0)',
+                (
+                    'import sys; sys.stdout.write("out");'
+                    'sys.stderr.write("err"); sys.exit(0)'
+                ),
             ],
             stderr=stderr,
         )
         out, err = capsys.readouterr()
         assert not err
         assert "out" not in out
         assert "err" not in out
@@ -431,16 +465,18 @@
 def test_custom_stderr_failed_command(capsys, tmpdir):
     with open(str(tmpdir / "out.txt"), "w+b") as stderr:
         with pytest.raises(nox.command.CommandFailed):
             nox.command.run(
                 [
                     PYTHON,
                     "-c",
-                    'import sys; sys.stdout.write("out");'
-                    'sys.stderr.write("err"); sys.exit(1)',
+                    (
+                        'import sys; sys.stdout.write("out");'
+                        'sys.stderr.write("err"); sys.exit(1)'
+                    ),
                 ],
                 stderr=stderr,
             )
         out, err = capsys.readouterr()
         assert not err
         assert "out" not in out
         assert "err" not in out
```

### Comparing `nox-2022.8.7/tests/test_logger.py` & `nox-2023.4.22/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `nox-2022.8.7/tests/test_main.py` & `nox-2023.4.22/tests/test_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,34 +213,55 @@
 
         # Verify that the explicit sessions are listed in the config.
         config = execute.call_args[1]["global_config"]
         assert config.sessions == ["unit tests", "the unit tests"]
 
 
 @pytest.mark.parametrize(
-    "env,sessions", [("foo", ["foo"]), ("foo,bar", ["foo", "bar"])]
+    "var,option,env,values",
+    [
+        ("NOXSESSION", "sessions", "foo", ["foo"]),
+        ("NOXSESSION", "sessions", "foo,bar", ["foo", "bar"]),
+        ("NOXPYTHON", "pythons", "3.9", ["3.9"]),
+        ("NOXPYTHON", "pythons", "3.9,3.10", ["3.9", "3.10"]),
+        ("NOXEXTRAPYTHON", "extra_pythons", "3.9", ["3.9"]),
+        ("NOXEXTRAPYTHON", "extra_pythons", "3.9,3.10", ["3.9", "3.10"]),
+        ("NOXFORCEPYTHON", "force_pythons", "3.9", ["3.9"]),
+        ("NOXFORCEPYTHON", "force_pythons", "3.9,3.10", ["3.9", "3.10"]),
+    ],
+    ids=[
+        "single_session",
+        "multiple_sessions",
+        "single_python",
+        "multiple_pythons",
+        "single_extra_python",
+        "multiple_extra_pythons",
+        "single_force_python",
+        "multiple_force_pythons",
+    ],
 )
-def test_main_session_from_nox_env_var(monkeypatch, env, sessions):
-    monkeypatch.setenv("NOXSESSION", env)
+def test_main_list_option_from_nox_env_var(monkeypatch, var, option, env, values):
+    monkeypatch.setenv(var, env)
     monkeypatch.setattr(sys, "argv", [sys.executable])
 
     with mock.patch("nox.workflow.execute") as execute:
         execute.return_value = 0
 
         # Call the main function.
         with mock.patch.object(sys, "exit") as exit:
             nox.__main__.main()
             exit.assert_called_once_with(0)
         assert execute.called
 
         # Verify that the sessions from the env var are listed in the config.
         config = execute.call_args[1]["global_config"]
-        assert len(config.sessions) == len(sessions)
-        for session in sessions:
-            assert session in config.sessions
+        config_values = getattr(config, option)
+        assert len(config_values) == len(values)
+        for value in values:
+            assert value in config_values
 
 
 def test_main_positional_args(capsys, monkeypatch):
     fake_exit = mock.Mock(side_effect=ValueError("asdf!"))
 
     monkeypatch.setattr(sys, "argv", [sys.executable, "1", "2", "3"])
     with mock.patch.object(sys, "exit", fake_exit), pytest.raises(
@@ -654,20 +675,20 @@
 
     _, err = capsys.readouterr()
 
     assert "color" in err
 
 
 def test_main_force_python(monkeypatch):
-    monkeypatch.setattr(sys, "argv", ["nox", "--force-python=3.10"])
+    monkeypatch.setattr(sys, "argv", ["nox", "--force-python=3.11"])
     with mock.patch("nox.workflow.execute", return_value=0) as execute:
         with mock.patch.object(sys, "exit"):
             nox.__main__.main()
         config = execute.call_args[1]["global_config"]
-    assert config.pythons == config.extra_pythons == ["3.10"]
+    assert config.pythons == config.extra_pythons == ["3.11"]
 
 
 def test_main_reuse_existing_virtualenvs_no_install(monkeypatch):
     monkeypatch.setattr(sys, "argv", ["nox", "-R"])
     with mock.patch("nox.workflow.execute", return_value=0) as execute:
         with mock.patch.object(sys, "exit"):
             nox.__main__.main()
```

### Comparing `nox-2022.8.7/tests/test_manifest.py` & `nox-2023.4.22/tests/test_manifest.py`

 * *Files 0% similar despite different names*

```diff
@@ -444,14 +444,14 @@
     # Define a session and add it to the manifest.
     def my_session(session):
         pass
 
     # the session sets "no venv backend" but declares some pythons
     my_session.python = ["3.7", "3.8"]
     my_session.venv_backend = "none"
-    my_session.should_warn = dict()
+    my_session.should_warn = {}
 
     sessions = manifest.make_session("my_session", my_session)
 
     # check that the pythons were correctly removed (a log warning is also emitted)
     assert sessions[0].func.python is False
     assert sessions[0].func.should_warn == {WARN_PYTHONS_IGNORED: ["3.7", "3.8"]}
```

### Comparing `nox-2022.8.7/tests/test_registry.py` & `nox-2023.4.22/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `nox-2022.8.7/tests/test_sessions.py` & `nox-2023.4.22/tests/test_sessions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1022,16 +1022,18 @@
     def test_execute_check_env(self):
         runner = self.make_runner_with_mock_venv()
 
         def func(session):
             session.run(
                 sys.executable,
                 "-c",
-                'import os; raise SystemExit(0 if os.environ["NOX_CURRENT_SESSION"] =='
-                f" {session.name!r} else 0)",
+                (
+                    "import os; raise SystemExit(0 if"
+                    f' os.environ["NOX_CURRENT_SESSION"] == {session.name!r} else 0)'
+                ),
             )
 
         runner.func = func
 
         result = runner.execute()
 
         assert result
```

### Comparing `nox-2022.8.7/tests/test_tasks.py` & `nox-2023.4.22/tests/test_tasks.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 def session_func():
     pass
 
 
 session_func.python = None
 session_func.venv_backend = None
-session_func.should_warn = dict()
+session_func.should_warn = {}
 session_func.tags = []
 
 
 def session_func_with_python():
     pass
 
 
@@ -397,14 +397,72 @@
     assert return_value == 0
 
     out = capsys.readouterr().out
 
     assert "Hello I'm a docstring" not in out
 
 
+def test_honor_list_json_request(capsys):
+    config = _options.options.namespace(
+        list_sessions=True, noxfile="noxfile.py", json=True
+    )
+    manifest = mock.create_autospec(Manifest)
+    manifest.list_all_sessions.return_value = [
+        (
+            argparse.Namespace(
+                name="bar",
+                friendly_name="foo",
+                description="simple",
+                func=argparse.Namespace(python="123"),
+                tags=[],
+            ),
+            True,
+        ),
+        (
+            argparse.Namespace(),
+            False,
+        ),
+    ]
+    return_value = tasks.honor_list_request(manifest, global_config=config)
+    assert return_value == 0
+    assert json.loads(capsys.readouterr().out) == [
+        {
+            "session": "foo",
+            "name": "bar",
+            "description": "simple",
+            "python": "123",
+            "tags": [],
+            "call_spec": {},
+        }
+    ]
+
+
+def test_refuse_json_nolist_request(caplog):
+    config = _options.options.namespace(
+        list_sessions=False, noxfile="noxfile.py", json=True
+    )
+    manifest = mock.create_autospec(Manifest)
+    manifest.list_all_sessions.return_value = [
+        (
+            argparse.Namespace(
+                name="bar",
+                friendly_name="foo",
+                description="simple",
+                func=argparse.Namespace(python="123"),
+                tags=[],
+            ),
+            True,
+        )
+    ]
+    return_value = tasks.honor_list_request(manifest, global_config=config)
+    assert return_value == 3
+    (record,) = caplog.records
+    assert record.message == "Must specify --list-sessions with --json"
+
+
 def test_empty_session_list_in_noxfile(capsys):
     config = _options.options.namespace(noxfile="noxfile.py", sessions=(), posargs=[])
     manifest = Manifest({"session": session_func}, config)
     return_value = tasks.filter_manifest(manifest, global_config=config)
     assert return_value == 0
     assert "No sessions selected." in capsys.readouterr().out
```

### Comparing `nox-2022.8.7/tests/test_tox_to_nox.py` & `nox-2023.4.22/tests/test_tox_to_nox.py`

 * *Files identical despite different names*

### Comparing `nox-2022.8.7/tests/test_virtualenv.py` & `nox-2023.4.22/tests/test_virtualenv.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,24 +16,32 @@
 
 import os
 import re
 import shutil
 import subprocess
 import sys
 from textwrap import dedent
+from typing import NamedTuple
 from unittest import mock
 
-import py
 import pytest
+import virtualenv
+from packaging import version
 
 import nox.virtualenv
 
 IS_WINDOWS = nox.virtualenv._SYSTEM == "Windows"
 HAS_CONDA = shutil.which("conda") is not None
 RAISE_ERROR = "RAISE_ERROR"
+VIRTUALENV_VERSION = virtualenv.version.version
+
+
+class TextProcessResult(NamedTuple):
+    stdout: str
+    returncode: int = 0
 
 
 @pytest.fixture
 def make_one(tmpdir):
     def factory(*args, **kwargs):
         location = tmpdir.join("venv")
         venv = nox.virtualenv.VirtualEnv(location.strpath, *args, **kwargs)
@@ -49,81 +57,46 @@
         venv = nox.virtualenv.CondaEnv(location.strpath, *args, **kwargs)
         return (venv, location)
 
     return factory
 
 
 @pytest.fixture
-def make_mocked_interpreter_path():
-    """Provides a factory to create a mocked ``path`` object pointing
-    to a python interpreter.
-
-    This mocked ``path`` provides
-        - a ``__str__`` which is equal to the factory's ``path`` parameter
-        - a ``sysexec`` method which returns the value of the
-          factory's ``sysexec_result`` parameter.
-          (the ``sysexec_result`` parameter can be a version string
-          or ``RAISE_ERROR``).
-    """
-
-    def factory(path, sysexec_result):
-        def mock_sysexec(*_):
-            if sysexec_result == RAISE_ERROR:
-                raise py.process.cmdexec.Error(1, 1, "", "", "")
-            else:
-                return sysexec_result
-
-        attrs = {
-            "sysexec.side_effect": mock_sysexec,
-            "__str__": mock.Mock(return_value=path),
-        }
-        mock_python = mock.Mock()
-        mock_python.configure_mock(**attrs)
-
-        return mock_python
-
-    return factory
-
-
-@pytest.fixture
-def patch_sysfind(make_mocked_interpreter_path):
+def patch_sysfind(monkeypatch):
     """Provides a function to patch ``sysfind`` with parameters for tests related
     to locating a Python interpreter in the system ``PATH``.
     """
 
-    def patcher(sysfind, only_find, sysfind_result, sysexec_result):
-        """Returns an extended ``sysfind`` patch object for tests related to locating a
-        Python interpreter in the system ``PATH``.
+    def patcher(only_find, sysfind_result, sysexec_result):
+        """Monkeypatches python discovery, causing specific results to be found.
 
         Args:
-            sysfind: The original sysfind patch object
-            only_find (Tuple[str]): The strings for which ``sysfind`` should be successful,
+            only_find (Tuple[str]): The strings for which ``shutil.which`` should be successful,
                 e.g. ``("python", "python.exe")``
             sysfind_result (Optional[str]): The ``path`` string to create the returned
                 mocked ``path`` object with which will represent the found Python interpreter,
                 or ``None``.
-                This parameter is passed on to ``make_mocked_interpreter_path``.
             sysexec_result (str): A string that should be returned when executing the
                 mocked ``path`` object. Usually a Python version string.
                 Use the global ``RAISE_ERROR`` to have ``sysexec`` fail.
-                This parameter is passed on to ``make_mocked_interpreter_path``.
         """
-        mock_python = make_mocked_interpreter_path(sysfind_result, sysexec_result)
 
-        def mock_sysfind(arg):
+        def special_which(name, path=None):
             if sysfind_result is None:
                 return None
-            elif arg.lower() in only_find:
-                return mock_python
-            else:
-                return None
+            if name.lower() in only_find:
+                return sysfind_result or name
+            return None
+
+        monkeypatch.setattr(shutil, "which", special_which)
 
-        sysfind.side_effect = mock_sysfind
+        def special_run(cmd, *args, **kwargs):
+            return TextProcessResult(sysexec_result)
 
-        return sysfind
+        monkeypatch.setattr(subprocess, "run", special_run)
 
     return patcher
 
 
 def test_process_env_constructor():
     penv = nox.virtualenv.ProcessEnv()
     assert not penv.bin_paths
@@ -174,15 +147,15 @@
         assert dir_.join("lib").check()
 
     # Test running create on an existing environment. It should be deleted.
     dir_.ensure("test.txt")
     venv.create()
     assert not dir_.join("test.txt").check()
 
-    # Test running create on an existing environment with reuse_exising
+    # Test running create on an existing environment with reuse_existing
     # enabled, it should not be deleted.
     dir_.ensure("test.txt")
     assert dir_.join("test.txt").check()
     venv.reuse_existing = True
     venv.create()
     assert dir_.join("test.txt").check()
     assert venv._reused
@@ -252,15 +225,15 @@
 
 @pytest.mark.skipif(not HAS_CONDA, reason="Missing conda command.")
 def test_condaenv_detection(make_conda):
     venv, dir_ = make_conda()
     venv.create()
 
     proc_result = subprocess.run(
-        [py.path.local.sysfind("conda").strpath, "list"],
+        [shutil.which("conda"), "list"],
         env=venv.env,
         check=True,
         capture_output=True,
     )
     output = proc_result.stdout.decode()
     path_regex = re.compile(r"packages in environment at (?P<env_dir>.+):")
 
@@ -372,15 +345,15 @@
         assert dir_.join("lib").check()
 
     # Test running create on an existing environment. It should be deleted.
     dir_.ensure("test.txt")
     venv.create()
     assert not dir_.join("test.txt").check()
 
-    # Test running create on an existing environment with reuse_exising
+    # Test running create on an existing environment with reuse_existing
     # enabled, it should not be deleted.
     dir_.ensure("test.txt")
     assert dir_.join("test.txt").check()
     venv.reuse_existing = True
 
     venv.create()
 
@@ -498,15 +471,41 @@
     reused = not venv.create()
 
     # The environment is detected as virtualenv-style and reused.
     assert reused
 
 
 @enable_staleness_check
-@pytest.mark.skipif(IS_WINDOWS, reason="Avoid spurious failure on Windows.")
+@pytest.mark.skipif(IS_WINDOWS, reason="Avoid 'No pyvenv.cfg file' error on Windows.")
+def test_inner_functions_reusing_venv(make_one):
+    venv, location = make_one(reuse_existing=True)
+    venv.create()
+
+    # Drop a venv-style pyvenv.cfg into the environment.
+    pyvenv_cfg = """\
+    home = /usr/bin
+    include-system-site-packages = false
+    version = 3.10
+    base-prefix = foo
+    """
+    location.join("pyvenv.cfg").write(dedent(pyvenv_cfg))
+
+    base_prefix = venv._read_base_prefix_from_pyvenv_cfg()
+    assert base_prefix == "foo"
+
+    reused_interpreter = venv._check_reused_environment_interpreter()
+    # The created won't match 'foo'
+    assert not reused_interpreter
+
+
+@enable_staleness_check
+@pytest.mark.skipif(
+    version.parse(VIRTUALENV_VERSION) >= version.parse("20.22.0"),
+    reason="Python 2.7 unsupported for virtualenv>=20.22.0",
+)
 def test_create_reuse_python2_environment(make_one):
     venv, location = make_one(reuse_existing=True, interpreter="2.7")
 
     try:
         venv.create()
     except nox.virtualenv.InterpreterNotFound:
         pytest.skip("Requires Python 2.7 installation.")
@@ -543,184 +542,180 @@
         ("3.6", "python3.6"),
         ("3.6.2", "python3.6"),
         ("3.10", "python3.10"),
         ("2.7.15", "python2.7"),
     ],
 )
 @mock.patch("nox.virtualenv._SYSTEM", new="Linux")
-@mock.patch.object(py.path.local, "sysfind", return_value=True)
-def test__resolved_interpreter_numerical_non_windows(
-    sysfind, make_one, input_, expected
-):
+@mock.patch.object(shutil, "which", return_value=True)
+def test__resolved_interpreter_numerical_non_windows(which, make_one, input_, expected):
     venv, _ = make_one(interpreter=input_)
 
     assert venv._resolved_interpreter == expected
-    sysfind.assert_called_once_with(expected)
+    which.assert_called_once_with(expected)
 
 
 @pytest.mark.parametrize("input_", ["2.", "2.7."])
 @mock.patch("nox.virtualenv._SYSTEM", new="Linux")
-@mock.patch.object(py.path.local, "sysfind", return_value=False)
-def test__resolved_interpreter_invalid_numerical_id(sysfind, make_one, input_):
+@mock.patch.object(shutil, "which", return_value=False)
+def test__resolved_interpreter_invalid_numerical_id(which, make_one, input_):
     venv, _ = make_one(interpreter=input_)
 
     with pytest.raises(nox.virtualenv.InterpreterNotFound):
         venv._resolved_interpreter
 
-    sysfind.assert_called_once_with(input_)
+    which.assert_called_once_with(input_)
 
 
 @mock.patch("nox.virtualenv._SYSTEM", new="Linux")
-@mock.patch.object(py.path.local, "sysfind", return_value=False)
-def test__resolved_interpreter_32_bit_non_windows(sysfind, make_one):
+@mock.patch.object(shutil, "which", return_value=False)
+def test__resolved_interpreter_32_bit_non_windows(which, make_one):
     venv, _ = make_one(interpreter="3.6-32")
 
     with pytest.raises(nox.virtualenv.InterpreterNotFound):
         venv._resolved_interpreter
-    sysfind.assert_called_once_with("3.6-32")
+    which.assert_called_once_with("3.6-32")
 
 
 @mock.patch("nox.virtualenv._SYSTEM", new="Linux")
-@mock.patch.object(py.path.local, "sysfind", return_value=True)
-def test__resolved_interpreter_non_windows(sysfind, make_one):
+@mock.patch.object(shutil, "which", return_value=True)
+def test__resolved_interpreter_non_windows(which, make_one):
     # Establish that the interpreter is simply passed through resolution
     # on non-Windows.
     venv, _ = make_one(interpreter="python3.6")
 
     assert venv._resolved_interpreter == "python3.6"
-    sysfind.assert_called_once_with("python3.6")
+    which.assert_called_once_with("python3.6")
 
 
 @mock.patch("nox.virtualenv._SYSTEM", new="Windows")
-@mock.patch.object(py.path.local, "sysfind")
-def test__resolved_interpreter_windows_full_path(sysfind, make_one):
+@mock.patch.object(shutil, "which")
+def test__resolved_interpreter_windows_full_path(which, make_one):
     # Establish that if we get a fully-qualified system path (on Windows
     # or otherwise) and the path exists, that we accept it.
     venv, _ = make_one(interpreter=r"c:\Python36\python.exe")
 
-    sysfind.return_value = py.path.local(venv.interpreter)
+    which.return_value = venv.interpreter
     assert venv._resolved_interpreter == r"c:\Python36\python.exe"
-    sysfind.assert_called_once_with(r"c:\Python36\python.exe")
+    which.assert_called_once_with(r"c:\Python36\python.exe")
 
 
 @pytest.mark.parametrize(
     ["input_", "expected"],
     [
         ("3.7", r"c:\python37-x64\python.exe"),
         ("python3.6", r"c:\python36-x64\python.exe"),
         ("2.7-32", r"c:\python27\python.exe"),
     ],
 )
 @mock.patch("nox.virtualenv._SYSTEM", new="Windows")
-@mock.patch.object(py.path.local, "sysfind")
-def test__resolved_interpreter_windows_pyexe(sysfind, make_one, input_, expected):
+@mock.patch.object(subprocess, "run")
+@mock.patch.object(shutil, "which")
+def test__resolved_interpreter_windows_pyexe(which, run, make_one, input_, expected):
     # Establish that if we get a standard pythonX.Y path, we look it
     # up via the py launcher on Windows.
     venv, _ = make_one(interpreter=input_)
 
+    if input_ == "3.7":
+        input_ = "python3.7"
+
     # Trick the system into thinking that it cannot find python3.6
     # (it likely will on Unix). Also, when the system looks for the
     # py launcher, give it a dummy that returns our test value when
     # run.
-    attrs = {"sysexec.return_value": expected}
-    mock_py = mock.Mock()
-    mock_py.configure_mock(**attrs)
-    sysfind.side_effect = lambda arg: mock_py if arg == "py" else None
+    def special_run(cmd, *args, **kwargs):
+        if cmd[0] == "py":
+            return TextProcessResult(expected)
+        return TextProcessResult("", 1)
+
+    run.side_effect = special_run
+    which.side_effect = lambda x: "py" if x == "py" else None
 
     # Okay now run the test.
     assert venv._resolved_interpreter == expected
-    assert sysfind.call_count == 2
-    if input_ == "3.7":
-        sysfind.assert_has_calls([mock.call("python3.7"), mock.call("py")])
-    else:
-        sysfind.assert_has_calls([mock.call(input_), mock.call("py")])
+    assert which.call_count == 2
+    which.assert_has_calls([mock.call(input_), mock.call("py")])
 
 
 @mock.patch("nox.virtualenv._SYSTEM", new="Windows")
-@mock.patch.object(py.path.local, "sysfind")
-def test__resolved_interpreter_windows_pyexe_fails(sysfind, make_one):
+@mock.patch.object(subprocess, "run")
+@mock.patch.object(shutil, "which")
+def test__resolved_interpreter_windows_pyexe_fails(which, run, make_one):
     # Establish that if the py launcher fails, we give the right error.
     venv, _ = make_one(interpreter="python3.6")
 
     # Trick the nox.virtualenv._SYSTEM into thinking that it cannot find python3.6
     # (it likely will on Unix). Also, when the nox.virtualenv._SYSTEM looks for the
     # py launcher, give it a dummy that fails.
-    attrs = {"sysexec.side_effect": py.process.cmdexec.Error(1, 1, "", "", "")}
-    mock_py = mock.Mock()
-    mock_py.configure_mock(**attrs)
-    sysfind.side_effect = lambda arg: mock_py if arg == "py" else None
+    def special_run(cmd, *args, **kwargs):
+        return TextProcessResult("", 1)
+
+    run.side_effect = special_run
+    which.side_effect = lambda x: "py" if x == "py" else None
 
     # Okay now run the test.
     with pytest.raises(nox.virtualenv.InterpreterNotFound):
         venv._resolved_interpreter
 
-    sysfind.assert_any_call("python3.6")
-    sysfind.assert_any_call("py")
+    which.assert_has_calls([mock.call("python3.6"), mock.call("py")])
 
 
 @mock.patch("nox.virtualenv._SYSTEM", new="Windows")
-@mock.patch.object(py.path.local, "sysfind")
-def test__resolved_interpreter_windows_path_and_version(
-    sysfind, make_one, patch_sysfind
-):
+def test__resolved_interpreter_windows_path_and_version(make_one, patch_sysfind):
     # Establish that if we get a standard pythonX.Y path, we look it
     # up via the path on Windows.
     venv, _ = make_one(interpreter="3.7")
 
     # Trick the system into thinking that it cannot find
     # pythonX.Y up until the python-in-path check at the end.
     # Also, we don't give it a mock py launcher.
     # But we give it a mock python interpreter to find
     # in the system path.
     correct_path = r"c:\python37-x64\python.exe"
     patch_sysfind(
-        sysfind,
         only_find=("python", "python.exe"),
         sysfind_result=correct_path,
         sysexec_result="3.7.3\\n",
     )
 
     # Okay, now run the test.
     assert venv._resolved_interpreter == correct_path
 
 
 @pytest.mark.parametrize("input_", ["2.7", "python3.7", "goofy"])
 @pytest.mark.parametrize("sysfind_result", [r"c:\python37-x64\python.exe", None])
 @pytest.mark.parametrize("sysexec_result", ["3.7.3\\n", RAISE_ERROR])
 @mock.patch("nox.virtualenv._SYSTEM", new="Windows")
-@mock.patch.object(py.path.local, "sysfind")
 def test__resolved_interpreter_windows_path_and_version_fails(
-    sysfind, input_, sysfind_result, sysexec_result, make_one, patch_sysfind
+    input_, sysfind_result, sysexec_result, make_one, patch_sysfind
 ):
     # Establish that if we get a standard pythonX.Y path, we look it
     # up via the path on Windows.
     venv, _ = make_one(interpreter=input_)
 
     # Trick the system into thinking that it cannot find
     # pythonX.Y up until the python-in-path check at the end.
     # Also, we don't give it a mock py launcher.
     # But we give it a mock python interpreter to find
     # in the system path.
-    patch_sysfind(sysfind, ("python", "python.exe"), sysfind_result, sysexec_result)
+    patch_sysfind(("python", "python.exe"), sysfind_result, sysexec_result)
 
     with pytest.raises(nox.virtualenv.InterpreterNotFound):
         venv._resolved_interpreter
 
 
 @mock.patch("nox.virtualenv._SYSTEM", new="Windows")
-@mock.patch.object(py._path.local.LocalPath, "check")
-@mock.patch.object(py.path.local, "sysfind")
-def test__resolved_interpreter_not_found(sysfind, check, make_one):
+@mock.patch.object(shutil, "which")
+def test__resolved_interpreter_not_found(which, make_one):
     # Establish that if an interpreter cannot be found at a standard
     # location on Windows, we raise a useful error.
     venv, _ = make_one(interpreter="python3.6")
 
     # We are on Windows, and nothing can be found.
-    sysfind.return_value = None
-    check.return_value = False
+    which.return_value = None
 
     # Run the test.
     with pytest.raises(nox.virtualenv.InterpreterNotFound):
         venv._resolved_interpreter
 
 
 @mock.patch("nox.virtualenv._SYSTEM", new="Windows")
@@ -730,36 +725,36 @@
     venv, _ = make_one(interpreter="goofy")
 
     with pytest.raises(nox.virtualenv.InterpreterNotFound):
         venv._resolved_interpreter
 
 
 @mock.patch("nox.virtualenv._SYSTEM", new="Linux")
-@mock.patch.object(py.path.local, "sysfind", return_value=True)
-def test__resolved_interpreter_cache_result(sysfind, make_one):
+@mock.patch.object(shutil, "which", return_value=True)
+def test__resolved_interpreter_cache_result(which, make_one):
     venv, _ = make_one(interpreter="3.6")
 
     assert venv._resolved is None
     assert venv._resolved_interpreter == "python3.6"
-    sysfind.assert_called_once_with("python3.6")
+    which.assert_called_once_with("python3.6")
     # Check the cache and call again to make sure it is used.
     assert venv._resolved == "python3.6"
     assert venv._resolved_interpreter == "python3.6"
-    assert sysfind.call_count == 1
+    assert which.call_count == 1
 
 
 @mock.patch("nox.virtualenv._SYSTEM", new="Linux")
-@mock.patch.object(py.path.local, "sysfind", return_value=None)
-def test__resolved_interpreter_cache_failure(sysfind, make_one):
+@mock.patch.object(shutil, "which", return_value=None)
+def test__resolved_interpreter_cache_failure(which, make_one):
     venv, _ = make_one(interpreter="3.7-32")
 
     assert venv._resolved is None
     with pytest.raises(nox.virtualenv.InterpreterNotFound) as exc_info:
         venv._resolved_interpreter
     caught = exc_info.value
 
-    sysfind.assert_called_once_with("3.7-32")
+    which.assert_called_once_with("3.7-32")
     # Check the cache and call again to make sure it is used.
     assert venv._resolved is caught
     with pytest.raises(nox.virtualenv.InterpreterNotFound):
         venv._resolved_interpreter
-    assert sysfind.call_count == 1
+    assert which.call_count == 1
```

### Comparing `nox-2022.8.7/tests/test_workflow.py` & `nox-2023.4.22/tests/test_workflow.py`

 * *Files identical despite different names*

