# Comparing `tmp/hatchling-1.8.1.tar.gz` & `tmp/hatchling-1.9.0.tar.gz`

## Comparing `hatchling-1.8.1.tar` & `hatchling-1.9.0.tar`

### file list

```diff
@@ -1,77 +1,78 @@
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 hatchling-1.8.1/scripts/update_classifiers.py
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 hatchling-1.8.1/scripts/update_licenses.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/__init__.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/__main__.py
--rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/build.py
--rw-r--r--   0        0        0     3576 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/ouroboros.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/bridge/__init__.py
--rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/bridge/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/builders/__init__.py
--rw-r--r--   0        0        0    35736 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/builders/config.py
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/builders/constants.py
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/builders/custom.py
--rw-r--r--   0        0        0    12052 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/builders/sdist.py
--rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/builders/utils.py
--rw-r--r--   0        0        0    22890 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/builders/wheel.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/builders/hooks/__init__.py
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/builders/hooks/custom.py
--rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/builders/hooks/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/builders/hooks/plugin/__init__.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/builders/hooks/plugin/hooks.py
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/builders/hooks/plugin/interface.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/builders/plugin/__init__.py
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/builders/plugin/hooks.py
--rw-r--r--   0        0        0    14256 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/builders/plugin/interface.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/cli/__init__.py
--rw-r--r--   0        0        0     3592 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/cli/build/__init__.py
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/cli/dep/__init__.py
--rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/cli/version/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/dep/__init__.py
--rw-r--r--   0        0        0     4268 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/dep/core.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/licenses/__init__.py
--rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/licenses/parse.py
--rw-r--r--   0        0        0    34571 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/licenses/supported.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/metadata/__init__.py
--rw-r--r--   0        0        0    38672 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/metadata/classifiers.py
--rw-r--r--   0        0        0    49657 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/metadata/core.py
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/metadata/custom.py
--rw-r--r--   0        0        0    10698 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/metadata/spec.py
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/metadata/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/metadata/plugin/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/metadata/plugin/hooks.py
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/metadata/plugin/interface.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/plugin/__init__.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/plugin/exceptions.py
--rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/plugin/manager.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/plugin/specs.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/plugin/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/utils/__init__.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/utils/constants.py
--rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/utils/context.py
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/utils/fs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/version/__init__.py
--rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/version/core.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/version/scheme/__init__.py
--rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/version/scheme/standard.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/version/scheme/plugin/__init__.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/version/scheme/plugin/hooks.py
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/version/scheme/plugin/interface.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/version/source/__init__.py
--rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/version/source/code.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/version/source/regex.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/version/source/plugin/__init__.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/version/source/plugin/hooks.py
--rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 hatchling-1.8.1/src/hatchling/version/source/plugin/interface.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatchling-1.8.1/tests/__init__.py
--rw-r--r--   0        0        0     9662 2020-02-02 00:00:00.000000 hatchling-1.8.1/tests/downstream/integrate.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 hatchling-1.8.1/tests/downstream/requirements.txt
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 hatchling-1.8.1/tests/downstream/datadogpy/data.json
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 hatchling-1.8.1/tests/downstream/datadogpy/pyproject.toml
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 hatchling-1.8.1/tests/downstream/hatch-showcase/data.json
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 hatchling-1.8.1/.gitignore
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 hatchling-1.8.1/LICENSE.txt
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 hatchling-1.8.1/README.md
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 hatchling-1.8.1/pyproject.toml
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 hatchling-1.8.1/PKG-INFO
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 hatchling-1.9.0/scripts/update_classifiers.py
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 hatchling-1.9.0/scripts/update_licenses.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/__init__.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/__main__.py
+-rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/build.py
+-rw-r--r--   0        0        0     5102 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/ouroboros.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/bridge/__init__.py
+-rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/bridge/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/builders/__init__.py
+-rw-r--r--   0        0        0    35453 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/builders/config.py
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/builders/constants.py
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/builders/custom.py
+-rw-r--r--   0        0        0    12052 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/builders/sdist.py
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/builders/utils.py
+-rw-r--r--   0        0        0    22832 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/builders/wheel.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/builders/hooks/__init__.py
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/builders/hooks/custom.py
+-rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/builders/hooks/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/builders/hooks/plugin/__init__.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/builders/hooks/plugin/hooks.py
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/builders/hooks/plugin/interface.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/builders/plugin/__init__.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/builders/plugin/hooks.py
+-rw-r--r--   0        0        0    14256 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/builders/plugin/interface.py
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/cli/__init__.py
+-rw-r--r--   0        0        0     3592 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/cli/build/__init__.py
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/cli/dep/__init__.py
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/cli/metadata/__init__.py
+-rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/cli/version/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/dep/__init__.py
+-rw-r--r--   0        0        0     4254 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/dep/core.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/licenses/__init__.py
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/licenses/parse.py
+-rw-r--r--   0        0        0    34571 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/licenses/supported.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/metadata/__init__.py
+-rw-r--r--   0        0        0    38672 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/metadata/classifiers.py
+-rw-r--r--   0        0        0    50566 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/metadata/core.py
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/metadata/custom.py
+-rw-r--r--   0        0        0    11012 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/metadata/spec.py
+-rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/metadata/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/metadata/plugin/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/metadata/plugin/hooks.py
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/metadata/plugin/interface.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/plugin/__init__.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/plugin/exceptions.py
+-rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/plugin/manager.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/plugin/specs.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/plugin/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/utils/__init__.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/utils/constants.py
+-rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/utils/context.py
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/utils/fs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/version/__init__.py
+-rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/version/core.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/version/scheme/__init__.py
+-rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/version/scheme/standard.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/version/scheme/plugin/__init__.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/version/scheme/plugin/hooks.py
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/version/scheme/plugin/interface.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/version/source/__init__.py
+-rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/version/source/code.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/version/source/regex.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/version/source/plugin/__init__.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/version/source/plugin/hooks.py
+-rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 hatchling-1.9.0/src/hatchling/version/source/plugin/interface.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatchling-1.9.0/tests/__init__.py
+-rw-r--r--   0        0        0     9662 2020-02-02 00:00:00.000000 hatchling-1.9.0/tests/downstream/integrate.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 hatchling-1.9.0/tests/downstream/requirements.txt
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 hatchling-1.9.0/tests/downstream/datadogpy/data.json
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 hatchling-1.9.0/tests/downstream/datadogpy/pyproject.toml
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 hatchling-1.9.0/tests/downstream/hatch-showcase/data.json
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 hatchling-1.9.0/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 hatchling-1.9.0/LICENSE.txt
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 hatchling-1.9.0/README.md
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 hatchling-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 hatchling-1.9.0/PKG-INFO
```

### Comparing `hatchling-1.8.1/scripts/update_classifiers.py` & `hatchling-1.9.0/scripts/update_classifiers.py`

 * *Files identical despite different names*

### Comparing `hatchling-1.8.1/scripts/update_licenses.py` & `hatchling-1.9.0/scripts/update_licenses.py`

 * *Files identical despite different names*

### Comparing `hatchling-1.8.1/src/hatchling/ouroboros.py` & `hatchling-1.9.0/src/hatchling/ouroboros.py`

 * *Files 23% similar despite different names*

```diff
@@ -32,15 +32,15 @@
             'Topic :: Software Development :: Build Tools',
             'Topic :: Software Development :: Libraries :: Python Modules',
         ],
         'dependencies': [
             'editables>=0.3',
             'importlib-metadata; python_version < "3.8"',
             'packaging>=21.3',
-            'pathspec>=0.9',
+            'pathspec>=0.10.1',
             'pluggy>=1.0.0',
             'tomli>=1.2.2; python_version < "3.11"',
         ],
         'scripts': {'hatchling': 'hatchling.cli:hatchling'},
         'dynamic': ['version'],
     },
     'tool': {
@@ -91,12 +91,52 @@
 def get_requires_for_build_wheel(config_settings=None):
     """
     https://peps.python.org/pep-0517/#get-requires-for-build-wheel
     """
     return CONFIG['project']['dependencies']
 
 
+def prepare_metadata_for_build_wheel(metadata_directory, config_settings=None):
+    """
+    https://peps.python.org/pep-0517/#prepare-metadata-for-build-wheel
+    """
+    from hatchling.builders.wheel import WheelBuilder
+
+    builder = WheelBuilder(os.getcwd(), config=CONFIG)
+
+    directory = os.path.join(metadata_directory, f'{builder.artifact_project_id}.dist-info')
+    if not os.path.isdir(directory):
+        os.mkdir(directory)
+
+    with open(os.path.join(directory, 'METADATA'), 'w', encoding='utf-8') as f:
+        f.write(builder.config.core_metadata_constructor(builder.metadata))
+
+    return os.path.basename(directory)
+
+
 def get_requires_for_build_editable(config_settings=None):
     """
     https://peps.python.org/pep-0660/#get-requires-for-build-editable
     """
     return CONFIG['project']['dependencies']
+
+
+def prepare_metadata_for_build_editable(metadata_directory, config_settings=None):
+    """
+    https://peps.python.org/pep-0660/#prepare-metadata-for-build-editable
+    """
+    from hatchling.builders.wheel import EDITABLES_MINIMUM_VERSION, WheelBuilder
+
+    builder = WheelBuilder(os.getcwd(), config=CONFIG)
+
+    directory = os.path.join(metadata_directory, f'{builder.artifact_project_id}.dist-info')
+    if not os.path.isdir(directory):
+        os.mkdir(directory)
+
+    extra_dependencies = []
+    if not builder.config.dev_mode_dirs and builder.config.dev_mode_exact:
+        extra_dependencies.append(f'editables~={EDITABLES_MINIMUM_VERSION}')
+
+    with open(os.path.join(directory, 'METADATA'), 'w', encoding='utf-8') as f:
+        f.write(builder.config.core_metadata_constructor(builder.metadata, extra_dependencies=extra_dependencies))
+
+    return os.path.basename(directory)
```

### Comparing `hatchling-1.8.1/src/hatchling/bridge/app.py` & `hatchling-1.9.0/src/hatchling/bridge/app.py`

 * *Files identical despite different names*

### Comparing `hatchling-1.8.1/src/hatchling/builders/config.py` & `hatchling-1.9.0/src/hatchling/builders/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         self.__dependencies = None
         self.__sources = None
         self.__packages = None
         self.__only_include = None
         self.__force_include = None
         self.__vcs_exclusion_files = None
 
-        # Possible pathspec.PathSpec
+        # Possible pathspec.GitIgnoreSpec
         self.__include_spec = None
         self.__exclude_spec = None
         self.__artifact_spec = None
 
         # These are used to create the pathspecs and will never be `None` after the first match attempt
         self.__include_patterns = None
         self.__exclude_patterns = None
@@ -147,17 +147,15 @@
 
             for relative_path in self.packages:
                 # Matching only at the root requires a forward slash, back slashes do not work. As such,
                 # normalize to forward slashes for consistency.
                 all_include_patterns.append(f"/{relative_path.replace(os.sep, '/')}/")
 
             if all_include_patterns:
-                self.__include_spec = pathspec.PathSpec.from_lines(
-                    pathspec.patterns.GitWildMatchPattern, all_include_patterns
-                )
+                self.__include_spec = pathspec.GitIgnoreSpec.from_lines(all_include_patterns)
 
             self.__include_patterns = all_include_patterns
 
         return self.__include_spec
 
     @property
     def exclude_spec(self):
@@ -183,17 +181,15 @@
 
                 all_exclude_patterns.append(exclude_pattern)
 
             if not self.ignore_vcs:
                 all_exclude_patterns.extend(self.load_vcs_exclusion_patterns())
 
             if all_exclude_patterns:
-                self.__exclude_spec = pathspec.PathSpec.from_lines(
-                    pathspec.patterns.GitWildMatchPattern, all_exclude_patterns
-                )
+                self.__exclude_spec = pathspec.GitIgnoreSpec.from_lines(all_exclude_patterns)
 
             self.__exclude_patterns = all_exclude_patterns
 
         return self.__exclude_spec
 
     @property
     def artifact_spec(self):
@@ -216,17 +212,15 @@
                     raise TypeError(f'Pattern #{i} in field `{artifact_location}` must be a string')
                 elif not artifact_pattern:
                     raise ValueError(f'Pattern #{i} in field `{artifact_location}` cannot be an empty string')
 
                 all_artifact_patterns.append(artifact_pattern)
 
             if all_artifact_patterns:
-                self.__artifact_spec = pathspec.PathSpec.from_lines(
-                    pathspec.patterns.GitWildMatchPattern, all_artifact_patterns
-                )
+                self.__artifact_spec = pathspec.GitIgnoreSpec.from_lines(all_artifact_patterns)
 
             self.__artifact_patterns = all_artifact_patterns
 
         return self.__artifact_spec
 
     @property
     def hook_config(self):
@@ -804,17 +798,15 @@
 
     @contextmanager
     def set_build_data(self, build_data):
         try:
             # Include anything the hooks indicate
             build_artifacts = build_data['artifacts']
             if build_artifacts:
-                self.build_artifact_spec = pathspec.PathSpec.from_lines(
-                    pathspec.patterns.GitWildMatchPattern, build_artifacts
-                )
+                self.build_artifact_spec = pathspec.GitIgnoreSpec.from_lines(build_artifacts)
 
             self.build_force_include.update(normalize_inclusion_map(build_data['force_include'], self.root))
 
             for inclusion_map in (self.force_include, self.build_force_include):
                 for source, target in inclusion_map.items():
                     # Ignore source
                     # old/ -> new/
```

### Comparing `hatchling-1.8.1/src/hatchling/builders/custom.py` & `hatchling-1.9.0/src/hatchling/builders/custom.py`

 * *Files identical despite different names*

### Comparing `hatchling-1.8.1/src/hatchling/builders/sdist.py` & `hatchling-1.9.0/src/hatchling/builders/sdist.py`

 * *Files identical despite different names*

### Comparing `hatchling-1.8.1/src/hatchling/builders/utils.py` & `hatchling-1.9.0/src/hatchling/builders/utils.py`

 * *Files identical despite different names*

### Comparing `hatchling-1.8.1/src/hatchling/builders/wheel.py` & `hatchling-1.9.0/src/hatchling/builders/wheel.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,19 +17,14 @@
     normalize_file_permissions,
     normalize_inclusion_map,
     replace_file,
     set_zip_info_mode,
 )
 from hatchling.metadata.spec import DEFAULT_METADATA_VERSION, get_core_metadata_constructors
 
-try:
-    from editables import EditableProject
-except ImportError:  # no cov
-    EditableProject = None
-
 EDITABLES_MINIMUM_VERSION = '0.3'
 
 
 class WheelArchive:
     def __init__(self, project_id, reproducible):
         """
         https://peps.python.org/pep-0427/#abstract
@@ -331,14 +326,16 @@
     def build_editable(self, directory, **build_data):
         if self.config.dev_mode_dirs:
             return self.build_editable_explicit(directory, **build_data)
         else:
             return self.build_editable_detection(directory, **build_data)
 
     def build_editable_detection(self, directory, **build_data):
+        from editables import EditableProject
+
         build_data['tag'] = self.get_default_tag()
 
         with WheelArchive(self.artifact_project_id, self.config.reproducible) as archive, closing(
             StringIO()
         ) as records:
             exposed_packages = {}
             for included_file in self.recurse_project_files():
```

### Comparing `hatchling-1.8.1/src/hatchling/builders/hooks/custom.py` & `hatchling-1.9.0/src/hatchling/builders/hooks/custom.py`

 * *Files identical despite different names*

### Comparing `hatchling-1.8.1/src/hatchling/builders/hooks/version.py` & `hatchling-1.9.0/src/hatchling/builders/hooks/version.py`

 * *Files identical despite different names*

### Comparing `hatchling-1.8.1/src/hatchling/builders/hooks/plugin/interface.py` & `hatchling-1.9.0/src/hatchling/builders/hooks/plugin/interface.py`

 * *Files identical despite different names*

### Comparing `hatchling-1.8.1/src/hatchling/builders/plugin/interface.py` & `hatchling-1.9.0/src/hatchling/builders/plugin/interface.py`

 * *Files identical despite different names*

### Comparing `hatchling-1.8.1/src/hatchling/cli/__init__.py` & `hatchling-1.9.0/src/hatchling/cli/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 import argparse
 
 from hatchling.cli.build import build_command
 from hatchling.cli.dep import dep_command
+from hatchling.cli.metadata import metadata_command
 from hatchling.cli.version import version_command
 
 
 def hatchling():
     parser = argparse.ArgumentParser(prog='hatchling', allow_abbrev=False)
-    subparsers = parser.add_subparsers(required=True)
+    subparsers = parser.add_subparsers()
 
     defaults = {'metavar': ''}
 
     build_command(subparsers, defaults)
     dep_command(subparsers, defaults)
+    metadata_command(subparsers, defaults)
     version_command(subparsers, defaults)
 
     kwargs = vars(parser.parse_args())
-    command = kwargs.pop('func')
-    command(**kwargs)
+    try:
+        command = kwargs.pop('func')
+    except KeyError:
+        parser.print_help()
+    else:
+        command(**kwargs)
```

### Comparing `hatchling-1.8.1/src/hatchling/cli/build/__init__.py` & `hatchling-1.9.0/src/hatchling/cli/build/__init__.py`

 * *Files identical despite different names*

### Comparing `hatchling-1.8.1/src/hatchling/cli/dep/__init__.py` & `hatchling-1.9.0/src/hatchling/cli/dep/__init__.py`

 * *Files identical despite different names*

### Comparing `hatchling-1.8.1/src/hatchling/cli/version/__init__.py` & `hatchling-1.9.0/src/hatchling/cli/version/__init__.py`

 * *Files identical despite different names*

### Comparing `hatchling-1.8.1/src/hatchling/dep/core.py` & `hatchling-1.9.0/src/hatchling/dep/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import re
 import sys
 
 from packaging.markers import default_environment
 from packaging.requirements import Requirement
 
-try:
+if sys.version_info >= (3, 8):
     from importlib.metadata import Distribution, DistributionFinder
-except ImportError:  # no cov
-    from importlib_metadata import Distribution, DistributionFinder  # type: ignore
+else:
+    from importlib_metadata import Distribution, DistributionFinder
 
 
 class DistributionCache:
     def __init__(self, sys_path):
         self._resolver = Distribution.discover(context=DistributionFinder.Context(path=sys_path))
         self._distributions = {}
         self._search_exhausted = False
```

### Comparing `hatchling-1.8.1/src/hatchling/licenses/parse.py` & `hatchling-1.9.0/src/hatchling/licenses/parse.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,32 @@
 from hatchling.licenses.supported import EXCEPTIONS, LICENSES
 
 
-def normalize_license_expression(license_expression):
-    if not license_expression:
-        return license_expression
+def get_valid_licenses():
+    valid_licenses = LICENSES.copy()
+
+    # https://peps.python.org/pep-0639/#should-custom-license-identifiers-be-allowed
+    public_license = 'LicenseRef-Public-Domain'
+    valid_licenses[public_license.lower()] = {'id': public_license, 'deprecated': False}
+
+    proprietary_license = 'LicenseRef-Proprietary'
+    valid_licenses[proprietary_license.lower()] = {'id': proprietary_license, 'deprecated': False}
+
+    return valid_licenses
+
+
+def normalize_license_expression(raw_license_expression):
+    if not raw_license_expression:
+        return raw_license_expression
+
+    valid_licenses = get_valid_licenses()
 
     # First normalize to lower case so we can look up licenses/exceptions
     # and so boolean operators are Python-compatible
-    license_expression = license_expression.lower()
+    license_expression = raw_license_expression.lower()
 
     # Then pad parentheses so tokenization can be achieved by merely splitting on white space
     license_expression = license_expression.replace('(', ' ( ').replace(')', ' ) ')
 
     # Now we begin parsing
     tokens = license_expression.split()
 
@@ -21,46 +36,47 @@
     python_tokens = []
     for token in tokens:
         if token not in ('or', 'and', 'with', '(', ')'):
             python_tokens.append('False')
         elif token == 'with':
             python_tokens.append('or')
         elif token == '(' and python_tokens and python_tokens[-1] not in ('or', 'and'):
-            raise ValueError('Invalid license expression')
+            raise ValueError(f'invalid license expression: {raw_license_expression}')
         else:
             python_tokens.append(token)
 
     python_expression = ' '.join(python_tokens)
     try:
         assert eval(python_expression) is False
     except Exception:
-        raise ValueError('Invalid license expression')
+        raise ValueError(f'invalid license expression: {raw_license_expression}') from None
 
     # Take a final pass to check for unknown licenses/exceptions
     normalized_tokens = []
     for token in tokens:
         if token in ('or', 'and', 'with', '(', ')'):
             normalized_tokens.append(token.upper())
             continue
 
         if normalized_tokens and normalized_tokens[-1] == 'WITH':
             if token not in EXCEPTIONS:
-                raise ValueError(f'Unknown license exception: {token}')
+                raise ValueError(f'unknown license exception: {token}')
+
             normalized_tokens.append(EXCEPTIONS[token]['id'])
         else:
             if token.endswith('+'):
                 token = token[:-1]
                 suffix = '+'
             else:
                 suffix = ''
 
-            if token not in LICENSES:
-                raise ValueError(f'Unknown license: {token}')
+            if token not in valid_licenses:
+                raise ValueError(f'unknown license: {token}')
 
-            normalized_tokens.append(LICENSES[token]['id'] + suffix)
+            normalized_tokens.append(valid_licenses[token]['id'] + suffix)
 
     # Construct the normalized expression
     normalized_expression = ' '.join(normalized_tokens)
 
     # Fix internal padding for parentheses
     normalized_expression = normalized_expression.replace('( ', '(').replace(' )', ')')
```

### Comparing `hatchling-1.8.1/src/hatchling/licenses/supported.py` & `hatchling-1.9.0/src/hatchling/licenses/supported.py`

 * *Files identical despite different names*

### Comparing `hatchling-1.8.1/src/hatchling/metadata/classifiers.py` & `hatchling-1.9.0/src/hatchling/metadata/classifiers.py`

 * *Files identical despite different names*

### Comparing `hatchling-1.8.1/src/hatchling/metadata/core.py` & `hatchling-1.9.0/src/hatchling/metadata/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import os
+import sys
 from copy import deepcopy
 
 from hatchling.metadata.utils import get_normalized_dependency, is_valid_project_name, normalize_project_name
 from hatchling.utils.constants import DEFAULT_CONFIG_FILE
 from hatchling.utils.fs import locate_file
 
-try:
+if sys.version_info >= (3, 11):
     import tomllib
-except ImportError:
-    import tomli as tomllib  # type: ignore
+else:
+    import tomli as tomllib
 
 
 def load_toml(path):
     with open(path, encoding='utf-8') as f:
         return tomllib.loads(f.read())
 
 
@@ -22,14 +23,16 @@
         self.plugin_manager = plugin_manager
         self._config = config
         self._context = None
         self._build = None
         self._core = None
         self._hatch = None
 
+        self._core_raw_metadata = None
+        self._name = None
         self._version = None
         self._project_file = None
 
         # App already loaded config
         if config is not None and root is not None:
             self._project_file = os.path.join(root, 'pyproject.toml')
 
@@ -43,14 +46,41 @@
             from hatchling.utils.context import Context
 
             self._context = Context(self.root)
 
         return self._context
 
     @property
+    def core_raw_metadata(self):
+        if self._core_raw_metadata is None:
+            if 'project' not in self.config:
+                raise ValueError('Missing `project` metadata table in configuration')
+
+            core_raw_metadata = self.config['project']
+            if not isinstance(core_raw_metadata, dict):
+                raise TypeError('The `project` configuration must be a table')
+
+            self._core_raw_metadata = core_raw_metadata
+
+        return self._core_raw_metadata
+
+    @property
+    def name(self):
+        # Duplicate the name parsing here for situations where it's
+        # needed but metadata plugins might not be available
+        if self._name is None:
+            name = self.core_raw_metadata.get('name', '')
+            if not name:
+                raise ValueError('Missing required field `project.name`')
+
+            self._name = normalize_project_name(name)
+
+        return self._name
+
+    @property
     def version(self):
         """
         https://peps.python.org/pep-0621/#version
         """
         if self._version is None:
             self._set_version()
 
@@ -78,35 +108,28 @@
             self._build = BuildMetadata(self.root, build_metadata)
 
         return self._build
 
     @property
     def core(self):
         if self._core is None:
-            if 'project' not in self.config:
-                raise ValueError('Missing `project` metadata table in configuration')
-
-            core_metadata = self.config['project']
-            if not isinstance(core_metadata, dict):
-                raise TypeError('The `project` configuration must be a table')
-
-            metadata = CoreMetadata(self.root, core_metadata, self.hatch.metadata, self.context)
+            metadata = CoreMetadata(self.root, self.core_raw_metadata, self.hatch.metadata, self.context)
 
             metadata_hooks = self.hatch.metadata.hooks
             if metadata_hooks:
-                static_fields = set(core_metadata)
+                static_fields = set(self.core_raw_metadata)
                 if 'version' in self.hatch.config:
                     self._set_version(metadata)
-                    core_metadata['version'] = self.version
+                    self.core_raw_metadata['version'] = self.version
 
                 for metadata_hook in metadata_hooks.values():
-                    metadata_hook.update(core_metadata)
+                    metadata_hook.update(self.core_raw_metadata)
                     metadata.add_known_classifiers(metadata_hook.get_known_classifiers())
 
-                new_fields = set(core_metadata) - static_fields
+                new_fields = set(self.core_raw_metadata) - static_fields
                 for new_field in new_fields:
                     if new_field in metadata.dynamic:
                         metadata.dynamic.remove(new_field)
                     else:
                         raise ValueError(
                             f'The field `{new_field}` was set dynamically and therefore must be '
                             f'listed in `project.dynamic`'
@@ -533,15 +556,19 @@
 
             if data is None:
                 self._license = ''
                 self._license_expression = ''
             elif isinstance(data, str):
                 from hatchling.licenses.parse import normalize_license_expression
 
-                self._license_expression = normalize_license_expression(data)
+                try:
+                    self._license_expression = normalize_license_expression(data)
+                except ValueError as e:
+                    raise ValueError(f'Error parsing field `project.license` - {e}') from None
+
                 self._license = ''
             elif isinstance(data, dict):
                 if 'file' in data and 'text' in data:
                     raise ValueError('Cannot specify both `file` and `text` in the `project.license` table')
 
                 if 'file' in data:
                     relative_path = data['file']
```

### Comparing `hatchling-1.8.1/src/hatchling/metadata/custom.py` & `hatchling-1.9.0/src/hatchling/metadata/custom.py`

 * *Files identical despite different names*

### Comparing `hatchling-1.8.1/src/hatchling/metadata/spec.py` & `hatchling-1.9.0/src/hatchling/metadata/spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,14 +106,18 @@
 
         for i, line in enumerate(metadata.core.license.splitlines()):
             if i == 0:
                 metadata_file += f'{line}\n'
             else:
                 metadata_file += f'{indent}{line}\n'
 
+    if metadata.core.license_files:
+        for license_file in metadata.core.license_files:
+            metadata_file += f'License-File: {license_file}\n'
+
     if metadata.core.keywords:
         metadata_file += f"Keywords: {','.join(metadata.core.keywords)}\n"
 
     if metadata.core.classifiers:
         for classifier in metadata.core.classifiers:
             metadata_file += f'Classifier: {classifier}\n'
 
@@ -178,14 +182,18 @@
 
         for i, line in enumerate(metadata.core.license.splitlines()):
             if i == 0:
                 metadata_file += f'{line}\n'
             else:
                 metadata_file += f'{indent}{line}\n'
 
+    if metadata.core.license_files:
+        for license_file in metadata.core.license_files:
+            metadata_file += f'License-File: {license_file}\n'
+
     if metadata.core.keywords:
         metadata_file += f"Keywords: {','.join(metadata.core.keywords)}\n"
 
     if metadata.core.classifiers:
         for classifier in metadata.core.classifiers:
             metadata_file += f'Classifier: {classifier}\n'
```

### Comparing `hatchling-1.8.1/src/hatchling/metadata/plugin/interface.py` & `hatchling-1.9.0/src/hatchling/metadata/plugin/interface.py`

 * *Files identical despite different names*

### Comparing `hatchling-1.8.1/src/hatchling/plugin/manager.py` & `hatchling-1.9.0/src/hatchling/plugin/manager.py`

 * *Files identical despite different names*

### Comparing `hatchling-1.8.1/src/hatchling/plugin/specs.py` & `hatchling-1.9.0/src/hatchling/plugin/specs.py`

 * *Files identical despite different names*

### Comparing `hatchling-1.8.1/src/hatchling/plugin/utils.py` & `hatchling-1.9.0/src/hatchling/plugin/utils.py`

 * *Files identical despite different names*

### Comparing `hatchling-1.8.1/src/hatchling/utils/context.py` & `hatchling-1.9.0/src/hatchling/utils/context.py`

 * *Files identical despite different names*

### Comparing `hatchling-1.8.1/src/hatchling/version/core.py` & `hatchling-1.9.0/src/hatchling/version/core.py`

 * *Files identical despite different names*

### Comparing `hatchling-1.8.1/src/hatchling/version/scheme/standard.py` & `hatchling-1.9.0/src/hatchling/version/scheme/standard.py`

 * *Files identical despite different names*

### Comparing `hatchling-1.8.1/src/hatchling/version/scheme/plugin/interface.py` & `hatchling-1.9.0/src/hatchling/version/scheme/plugin/interface.py`

 * *Files identical despite different names*

### Comparing `hatchling-1.8.1/src/hatchling/version/source/code.py` & `hatchling-1.9.0/src/hatchling/version/source/code.py`

 * *Files identical despite different names*

### Comparing `hatchling-1.8.1/src/hatchling/version/source/regex.py` & `hatchling-1.9.0/src/hatchling/version/source/regex.py`

 * *Files identical despite different names*

### Comparing `hatchling-1.8.1/src/hatchling/version/source/plugin/interface.py` & `hatchling-1.9.0/src/hatchling/version/source/plugin/interface.py`

 * *Files identical despite different names*

### Comparing `hatchling-1.8.1/tests/downstream/integrate.py` & `hatchling-1.9.0/tests/downstream/integrate.py`

 * *Files identical despite different names*

### Comparing `hatchling-1.8.1/tests/downstream/datadogpy/pyproject.toml` & `hatchling-1.9.0/tests/downstream/datadogpy/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hatchling-1.8.1/LICENSE.txt` & `hatchling-1.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hatchling-1.8.1/PKG-INFO` & `hatchling-1.9.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: hatchling
-Version: 1.8.1
+Version: 1.9.0
 Summary: Modern, extensible Python build backend
 Project-URL: Homepage, https://hatch.pypa.io/latest/
 Project-URL: Sponsor, https://github.com/sponsors/ofek
 Project-URL: History, https://hatch.pypa.io/dev/history/
 Project-URL: Tracker, https://github.com/pypa/hatch/issues
 Project-URL: Source, https://github.com/pypa/hatch/tree/master/backend
 Author-email: Ofek Lev <oss@ofek.dev>
+License-File: LICENSE.txt
 Keywords: build,hatch,packaging
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
@@ -23,15 +24,15 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Requires-Dist: editables>=0.3
 Requires-Dist: importlib-metadata; python_version < '3.8'
 Requires-Dist: packaging>=21.3
-Requires-Dist: pathspec>=0.9
+Requires-Dist: pathspec>=0.10.1
 Requires-Dist: pluggy>=1.0.0
 Requires-Dist: tomli>=1.2.2; python_version < '3.11'
 Description-Content-Type: text/markdown
 
 # Hatchling
 
 -----
```

