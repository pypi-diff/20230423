# Comparing `tmp/commitizen-3.0.0.tar.gz` & `tmp/commitizen-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commitizen-3.0.0.tar", max compression
+gzip compressed data, was "commitizen-3.0.1.tar", max compression
```

## Comparing `commitizen-3.0.0.tar` & `commitizen-3.0.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1065 2023-04-23 05:55:10.670575 commitizen-3.0.0/LICENSE
--rw-r--r--   0        0        0      593 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/__init__.py
--rw-r--r--   0        0        0       71 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/__main__.py
--rw-r--r--   0        0        0       22 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/__version__.py
--rw-r--r--   0        0        0     8613 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/bump.py
--rw-r--r--   0        0        0    11909 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/changelog.py
--rw-r--r--   0        0        0     3431 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/changelog_parser.py
--rw-r--r--   0        0        0    16605 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/cli.py
--rw-r--r--   0        0        0     1112 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/cmd.py
--rw-r--r--   0        0        0      420 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/commands/__init__.py
--rw-r--r--   0        0        0    13755 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/commands/bump.py
--rw-r--r--   0        0        0     6845 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/commands/changelog.py
--rw-r--r--   0        0        0     5067 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/commands/check.py
--rw-r--r--   0        0        0     3059 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/commands/commit.py
--rw-r--r--   0        0        0      364 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/commands/example.py
--rw-r--r--   0        0        0      350 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/commands/info.py
--rw-r--r--   0        0        0    12935 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/commands/init.py
--rw-r--r--   0        0        0      325 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/commands/list_cz.py
--rw-r--r--   0        0        0      341 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/commands/schema.py
--rw-r--r--   0        0        0     1488 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/commands/version.py
--rw-r--r--   0        0        0     1229 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/config/__init__.py
--rw-r--r--   0        0        0      915 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/config/base_config.py
--rw-r--r--   0        0        0     1384 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/config/json_config.py
--rw-r--r--   0        0        0     1753 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/config/toml_config.py
--rw-r--r--   0        0        0     1438 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/config/yaml_config.py
--rw-r--r--   0        0        0     1226 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/cz/__init__.py
--rw-r--r--   0        0        0     2951 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/cz/base.py
--rw-r--r--   0        0        0       64 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/cz/conventional_commits/__init__.py
--rw-r--r--   0        0        0     7043 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/cz/conventional_commits/conventional_commits.py
--rw-r--r--   0        0        0     1285 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/cz/conventional_commits/conventional_commits_info.txt
--rw-r--r--   0        0        0       50 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/cz/customize/__init__.py
--rw-r--r--   0        0        0     2801 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/cz/customize/customize.py
--rw-r--r--   0        0        0        0 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/cz/customize/customize_info.txt
--rw-r--r--   0        0        0       88 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/cz/exceptions.py
--rw-r--r--   0        0        0       57 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/cz/jira/__init__.py
--rw-r--r--   0        0        0     2678 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/cz/jira/jira.py
--rw-r--r--   0        0        0     1940 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/cz/jira/jira_info.txt
--rw-r--r--   0        0        0      272 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/cz/utils.py
--rw-r--r--   0        0        0     3253 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/defaults.py
--rw-r--r--   0        0        0     4575 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/exceptions.py
--rw-r--r--   0        0        0      639 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/factory.py
--rw-r--r--   0        0        0     6916 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/git.py
--rw-r--r--   0        0        0      951 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/hooks.py
--rw-r--r--   0        0        0      745 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/out.py
--rw-r--r--   0        0        0     6657 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/providers.py
--rw-r--r--   0        0        0      405 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/templates/keep_a_changelog_template.j2
--rw-r--r--   0        0        0     2400 2023-04-23 05:55:10.674575 commitizen-3.0.0/commitizen/version_types.py
--rw-r--r--   0        0        0     5800 2023-04-23 05:55:10.674575 commitizen-3.0.0/docs/README.md
--rw-r--r--   0        0        0     3958 2023-04-23 05:55:10.682575 commitizen-3.0.0/pyproject.toml
--rw-r--r--   0        0        0     7633 1970-01-01 00:00:00.000000 commitizen-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-23 07:23:07.112274 commitizen-3.0.1/LICENSE
+-rw-r--r--   0        0        0      593 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/__init__.py
+-rw-r--r--   0        0        0       71 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/__main__.py
+-rw-r--r--   0        0        0       22 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/__version__.py
+-rw-r--r--   0        0        0     8613 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/bump.py
+-rw-r--r--   0        0        0    11909 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/changelog.py
+-rw-r--r--   0        0        0     3431 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/changelog_parser.py
+-rw-r--r--   0        0        0    16605 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/cli.py
+-rw-r--r--   0        0        0     1112 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/cmd.py
+-rw-r--r--   0        0        0      420 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/commands/__init__.py
+-rw-r--r--   0        0        0    13755 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/commands/bump.py
+-rw-r--r--   0        0        0     6845 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/commands/changelog.py
+-rw-r--r--   0        0        0     5067 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/commands/check.py
+-rw-r--r--   0        0        0     3059 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/commands/commit.py
+-rw-r--r--   0        0        0      364 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/commands/example.py
+-rw-r--r--   0        0        0      350 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/commands/info.py
+-rw-r--r--   0        0        0    12935 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/commands/init.py
+-rw-r--r--   0        0        0      325 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/commands/list_cz.py
+-rw-r--r--   0        0        0      341 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/commands/schema.py
+-rw-r--r--   0        0        0     1488 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/commands/version.py
+-rw-r--r--   0        0        0     1229 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/config/__init__.py
+-rw-r--r--   0        0        0      915 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/config/base_config.py
+-rw-r--r--   0        0        0     1384 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/config/json_config.py
+-rw-r--r--   0        0        0     1753 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/config/toml_config.py
+-rw-r--r--   0        0        0     1438 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/config/yaml_config.py
+-rw-r--r--   0        0        0     1226 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/cz/__init__.py
+-rw-r--r--   0        0        0     2951 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/cz/base.py
+-rw-r--r--   0        0        0       64 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/cz/conventional_commits/__init__.py
+-rw-r--r--   0        0        0     7043 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/cz/conventional_commits/conventional_commits.py
+-rw-r--r--   0        0        0     1285 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/cz/conventional_commits/conventional_commits_info.txt
+-rw-r--r--   0        0        0       50 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/cz/customize/__init__.py
+-rw-r--r--   0        0        0     2801 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/cz/customize/customize.py
+-rw-r--r--   0        0        0        0 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/cz/customize/customize_info.txt
+-rw-r--r--   0        0        0       88 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/cz/exceptions.py
+-rw-r--r--   0        0        0       57 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/cz/jira/__init__.py
+-rw-r--r--   0        0        0     2678 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/cz/jira/jira.py
+-rw-r--r--   0        0        0     1940 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/cz/jira/jira_info.txt
+-rw-r--r--   0        0        0      272 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/cz/utils.py
+-rw-r--r--   0        0        0     3253 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/defaults.py
+-rw-r--r--   0        0        0     4575 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/exceptions.py
+-rw-r--r--   0        0        0      639 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/factory.py
+-rw-r--r--   0        0        0     6916 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/git.py
+-rw-r--r--   0        0        0      951 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/hooks.py
+-rw-r--r--   0        0        0      745 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/out.py
+-rw-r--r--   0        0        0     6657 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/providers.py
+-rw-r--r--   0        0        0      405 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/templates/keep_a_changelog_template.j2
+-rw-r--r--   0        0        0     2400 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/version_types.py
+-rw-r--r--   0        0        0     5800 2023-04-23 07:23:07.116274 commitizen-3.0.1/docs/README.md
+-rw-r--r--   0        0        0     3959 2023-04-23 07:23:07.124274 commitizen-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0     7633 1970-01-01 00:00:00.000000 commitizen-3.0.1/PKG-INFO
```

### Comparing `commitizen-3.0.0/LICENSE` & `commitizen-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.0/commitizen/__init__.py` & `commitizen-3.0.1/commitizen/__init__.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.0/commitizen/bump.py` & `commitizen-3.0.1/commitizen/bump.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.0/commitizen/changelog.py` & `commitizen-3.0.1/commitizen/changelog.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.0/commitizen/changelog_parser.py` & `commitizen-3.0.1/commitizen/changelog_parser.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.0/commitizen/cli.py` & `commitizen-3.0.1/commitizen/cli.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.0/commitizen/cmd.py` & `commitizen-3.0.1/commitizen/cmd.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.0/commitizen/commands/bump.py` & `commitizen-3.0.1/commitizen/commands/bump.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.0/commitizen/commands/changelog.py` & `commitizen-3.0.1/commitizen/commands/changelog.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.0/commitizen/commands/check.py` & `commitizen-3.0.1/commitizen/commands/check.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.0/commitizen/commands/commit.py` & `commitizen-3.0.1/commitizen/commands/commit.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.0/commitizen/commands/init.py` & `commitizen-3.0.1/commitizen/commands/init.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.0/commitizen/commands/version.py` & `commitizen-3.0.1/commitizen/commands/version.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.0/commitizen/config/__init__.py` & `commitizen-3.0.1/commitizen/config/__init__.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.0/commitizen/config/base_config.py` & `commitizen-3.0.1/commitizen/config/base_config.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.0/commitizen/config/json_config.py` & `commitizen-3.0.1/commitizen/config/json_config.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.0/commitizen/config/toml_config.py` & `commitizen-3.0.1/commitizen/config/toml_config.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.0/commitizen/config/yaml_config.py` & `commitizen-3.0.1/commitizen/config/yaml_config.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.0/commitizen/cz/__init__.py` & `commitizen-3.0.1/commitizen/cz/__init__.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.0/commitizen/cz/base.py` & `commitizen-3.0.1/commitizen/cz/base.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.0/commitizen/cz/conventional_commits/conventional_commits.py` & `commitizen-3.0.1/commitizen/cz/conventional_commits/conventional_commits.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.0/commitizen/cz/conventional_commits/conventional_commits_info.txt` & `commitizen-3.0.1/commitizen/cz/conventional_commits/conventional_commits_info.txt`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.0/commitizen/cz/customize/customize.py` & `commitizen-3.0.1/commitizen/cz/customize/customize.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.0/commitizen/cz/jira/jira.py` & `commitizen-3.0.1/commitizen/cz/jira/jira.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.0/commitizen/cz/jira/jira_info.txt` & `commitizen-3.0.1/commitizen/cz/jira/jira_info.txt`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.0/commitizen/defaults.py` & `commitizen-3.0.1/commitizen/defaults.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.0/commitizen/exceptions.py` & `commitizen-3.0.1/commitizen/exceptions.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.0/commitizen/factory.py` & `commitizen-3.0.1/commitizen/factory.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.0/commitizen/git.py` & `commitizen-3.0.1/commitizen/git.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.0/commitizen/hooks.py` & `commitizen-3.0.1/commitizen/hooks.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.0/commitizen/out.py` & `commitizen-3.0.1/commitizen/out.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.0/commitizen/providers.py` & `commitizen-3.0.1/commitizen/providers.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.0/commitizen/version_types.py` & `commitizen-3.0.1/commitizen/version_types.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.0/docs/README.md` & `commitizen-3.0.1/docs/README.md`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.0/pyproject.toml` & `commitizen-3.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.commitizen]
-version = "3.0.0"
+version = "3.0.1"
 tag_format = "v$version"
 version_files = [
   "pyproject.toml:version",
   "commitizen/__version__.py",
   ".pre-commit-config.yaml:rev:.+Commitizen"
 ]
 
 [tool.poetry]
 name = "commitizen"
-version = "3.0.0"
+version = "3.0.1"
 description = "Python commitizen client tool"
 authors = ["Santiago Fraire <santiwilly@gmail.com>"]
 license = "MIT"
 keywords = ["commitizen", "conventional", "commits", "git"]
 readme = "docs/README.md"
 homepage = "https://github.com/commitizen-tools/commitizen"
 # See also: https://pypi.org/classifiers/
@@ -58,15 +58,15 @@
 pytest-regressions = "^2.4.0"
 pytest-freezer = "^0.4.6"
 pytest-xdist = "^3.1.0"
 # code formatter
 black = "^22.10"
 # linter
 ruff = "^0.0.262"
-pre-commit = "^2.6.0"
+pre-commit = "^2.18.0"
 mypy = "^0.931"
 types-PyYAML = "^5.4.3"
 types-termcolor = "^0.1.1"
 # documentation
 mkdocs = "^1.4.2"
 mkdocs-material = "^9.1.6"
```

### Comparing `commitizen-3.0.0/PKG-INFO` & `commitizen-3.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commitizen
-Version: 3.0.0
+Version: 3.0.1
 Summary: Python commitizen client tool
 Home-page: https://github.com/commitizen-tools/commitizen
 License: MIT
 Keywords: commitizen,conventional,commits,git
 Author: Santiago Fraire
 Author-email: santiwilly@gmail.com
 Requires-Python: >=3.7,<4.0
```

