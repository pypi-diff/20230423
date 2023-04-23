# Comparing `tmp/commitizen-2.9.0.tar.gz` & `tmp/commitizen-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commitizen-2.9.0.tar", last modified: Wed Dec  2 08:43:36 2020, max compression
+gzip compressed data, was "commitizen-3.0.0.tar", max compression
```

## Comparing `commitizen-2.9.0.tar` & `commitizen-3.0.0.tar`

### file list

```diff
@@ -1,47 +1,50 @@
--rw-r--r--   0        0        0     1065 2020-12-02 08:41:44.537948 commitizen-2.9.0/LICENSE
--rw-r--r--   0        0        0      593 2020-12-02 08:41:44.537948 commitizen-2.9.0/commitizen/__init__.py
--rw-r--r--   0        0        0       71 2020-12-02 08:41:44.537948 commitizen-2.9.0/commitizen/__main__.py
--rw-r--r--   0        0        0       22 2020-12-02 08:41:44.537948 commitizen-2.9.0/commitizen/__version__.py
--rw-r--r--   0        0        0     7229 2020-12-02 08:41:44.537948 commitizen-2.9.0/commitizen/bump.py
--rw-r--r--   0        0        0     8469 2020-12-02 08:41:44.537948 commitizen-2.9.0/commitizen/changelog.py
--rw-r--r--   0        0        0     3431 2020-12-02 08:41:44.537948 commitizen-2.9.0/commitizen/changelog_parser.py
--rw-r--r--   0        0        0    10742 2020-12-02 08:41:44.537948 commitizen-2.9.0/commitizen/cli.py
--rw-r--r--   0        0        0      520 2020-12-02 08:41:44.537948 commitizen-2.9.0/commitizen/cmd.py
--rw-r--r--   0        0        0      420 2020-12-02 08:41:44.537948 commitizen-2.9.0/commitizen/commands/__init__.py
--rw-r--r--   0        0        0     6943 2020-12-02 08:41:44.537948 commitizen-2.9.0/commitizen/commands/bump.py
--rw-r--r--   0        0        0     4805 2020-12-02 08:41:44.537948 commitizen-2.9.0/commitizen/commands/changelog.py
--rw-r--r--   0        0        0     3582 2020-12-02 08:41:44.537948 commitizen-2.9.0/commitizen/commands/check.py
--rw-r--r--   0        0        0     2653 2020-12-02 08:41:44.537948 commitizen-2.9.0/commitizen/commands/commit.py
--rw-r--r--   0        0        0      364 2020-12-02 08:41:44.537948 commitizen-2.9.0/commitizen/commands/example.py
--rw-r--r--   0        0        0      350 2020-12-02 08:41:44.537948 commitizen-2.9.0/commitizen/commands/info.py
--rw-r--r--   0        0        0     5772 2020-12-02 08:41:44.537948 commitizen-2.9.0/commitizen/commands/init.py
--rw-r--r--   0        0        0      325 2020-12-02 08:41:44.537948 commitizen-2.9.0/commitizen/commands/list_cz.py
--rw-r--r--   0        0        0      341 2020-12-02 08:41:44.537948 commitizen-2.9.0/commitizen/commands/schema.py
--rw-r--r--   0        0        0     1071 2020-12-02 08:41:44.537948 commitizen-2.9.0/commitizen/commands/version.py
--rw-r--r--   0        0        0     1079 2020-12-02 08:41:44.537948 commitizen-2.9.0/commitizen/config/__init__.py
--rw-r--r--   0        0        0      894 2020-12-02 08:41:44.537948 commitizen-2.9.0/commitizen/config/base_config.py
--rw-r--r--   0        0        0     1286 2020-12-02 08:41:44.537948 commitizen-2.9.0/commitizen/config/json_config.py
--rw-r--r--   0        0        0     1303 2020-12-02 08:41:44.537948 commitizen-2.9.0/commitizen/config/toml_config.py
--rw-r--r--   0        0        0      641 2020-12-02 08:41:44.537948 commitizen-2.9.0/commitizen/cz/__init__.py
--rw-r--r--   0        0        0     2844 2020-12-02 08:41:44.537948 commitizen-2.9.0/commitizen/cz/base.py
--rw-r--r--   0        0        0       64 2020-12-02 08:41:44.537948 commitizen-2.9.0/commitizen/cz/conventional_commits/__init__.py
--rw-r--r--   0        0        0     6477 2020-12-02 08:41:44.537948 commitizen-2.9.0/commitizen/cz/conventional_commits/conventional_commits.py
--rw-r--r--   0        0        0     1285 2020-12-02 08:41:44.537948 commitizen-2.9.0/commitizen/cz/conventional_commits/conventional_commits_info.txt
--rw-r--r--   0        0        0       50 2020-12-02 08:41:44.537948 commitizen-2.9.0/commitizen/cz/customize/__init__.py
--rw-r--r--   0        0        0     2095 2020-12-02 08:41:44.537948 commitizen-2.9.0/commitizen/cz/customize/customize.py
--rw-r--r--   0        0        0        0 2020-12-02 08:41:44.537948 commitizen-2.9.0/commitizen/cz/customize/customize_info.txt
--rw-r--r--   0        0        0       88 2020-12-02 08:41:44.537948 commitizen-2.9.0/commitizen/cz/exceptions.py
--rw-r--r--   0        0        0       57 2020-12-02 08:41:44.537948 commitizen-2.9.0/commitizen/cz/jira/__init__.py
--rw-r--r--   0        0        0     2682 2020-12-02 08:41:44.537948 commitizen-2.9.0/commitizen/cz/jira/jira.py
--rw-r--r--   0        0        0     1940 2020-12-02 08:41:44.537948 commitizen-2.9.0/commitizen/cz/jira/jira_info.txt
--rw-r--r--   0        0        0      272 2020-12-02 08:41:44.537948 commitizen-2.9.0/commitizen/cz/utils.py
--rw-r--r--   0        0        0     1264 2020-12-02 08:41:44.537948 commitizen-2.9.0/commitizen/defaults.py
--rw-r--r--   0        0        0     3529 2020-12-02 08:41:44.537948 commitizen-2.9.0/commitizen/exceptions.py
--rw-r--r--   0        0        0      639 2020-12-02 08:41:44.537948 commitizen-2.9.0/commitizen/factory.py
--rw-r--r--   0        0        0     3975 2020-12-02 08:41:44.537948 commitizen-2.9.0/commitizen/git.py
--rw-r--r--   0        0        0      552 2020-12-02 08:41:44.537948 commitizen-2.9.0/commitizen/out.py
--rw-r--r--   0        0        0      405 2020-12-02 08:41:44.537948 commitizen-2.9.0/commitizen/templates/keep_a_changelog_template.j2
--rw-r--r--   0        0        0     5594 2020-12-02 08:41:44.537948 commitizen-2.9.0/docs/README.md
--rw-r--r--   0        0        0     2414 2020-12-02 08:41:44.549948 commitizen-2.9.0/pyproject.toml
--rw-r--r--   0        0        0     6948 2020-12-02 08:43:36.402368 commitizen-2.9.0/setup.py
--rw-r--r--   0        0        0     6616 2020-12-02 08:43:36.402778 commitizen-2.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-23 05:55:10.670575 commitizen-3.0.0/LICENSE
+-rw-r--r--   0        0        0      593 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/__init__.py
+-rw-r--r--   0        0        0       71 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/__main__.py
+-rw-r--r--   0        0        0       22 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/__version__.py
+-rw-r--r--   0        0        0     8613 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/bump.py
+-rw-r--r--   0        0        0    11909 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/changelog.py
+-rw-r--r--   0        0        0     3431 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/changelog_parser.py
+-rw-r--r--   0        0        0    16605 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/cli.py
+-rw-r--r--   0        0        0     1112 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/cmd.py
+-rw-r--r--   0        0        0      420 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/commands/__init__.py
+-rw-r--r--   0        0        0    13755 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/commands/bump.py
+-rw-r--r--   0        0        0     6845 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/commands/changelog.py
+-rw-r--r--   0        0        0     5067 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/commands/check.py
+-rw-r--r--   0        0        0     3059 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/commands/commit.py
+-rw-r--r--   0        0        0      364 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/commands/example.py
+-rw-r--r--   0        0        0      350 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/commands/info.py
+-rw-r--r--   0        0        0    12935 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/commands/init.py
+-rw-r--r--   0        0        0      325 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/commands/list_cz.py
+-rw-r--r--   0        0        0      341 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/commands/schema.py
+-rw-r--r--   0        0        0     1488 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/commands/version.py
+-rw-r--r--   0        0        0     1229 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/config/__init__.py
+-rw-r--r--   0        0        0      915 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/config/base_config.py
+-rw-r--r--   0        0        0     1384 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/config/json_config.py
+-rw-r--r--   0        0        0     1753 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/config/toml_config.py
+-rw-r--r--   0        0        0     1438 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/config/yaml_config.py
+-rw-r--r--   0        0        0     1226 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/cz/__init__.py
+-rw-r--r--   0        0        0     2951 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/cz/base.py
+-rw-r--r--   0        0        0       64 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/cz/conventional_commits/__init__.py
+-rw-r--r--   0        0        0     7043 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/cz/conventional_commits/conventional_commits.py
+-rw-r--r--   0        0        0     1285 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/cz/conventional_commits/conventional_commits_info.txt
+-rw-r--r--   0        0        0       50 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/cz/customize/__init__.py
+-rw-r--r--   0        0        0     2801 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/cz/customize/customize.py
+-rw-r--r--   0        0        0        0 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/cz/customize/customize_info.txt
+-rw-r--r--   0        0        0       88 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/cz/exceptions.py
+-rw-r--r--   0        0        0       57 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/cz/jira/__init__.py
+-rw-r--r--   0        0        0     2678 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/cz/jira/jira.py
+-rw-r--r--   0        0        0     1940 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/cz/jira/jira_info.txt
+-rw-r--r--   0        0        0      272 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/cz/utils.py
+-rw-r--r--   0        0        0     3253 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/defaults.py
+-rw-r--r--   0        0        0     4575 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/exceptions.py
+-rw-r--r--   0        0        0      639 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/factory.py
+-rw-r--r--   0        0        0     6916 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/git.py
+-rw-r--r--   0        0        0      951 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/hooks.py
+-rw-r--r--   0        0        0      745 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/out.py
+-rw-r--r--   0        0        0     6657 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/providers.py
+-rw-r--r--   0        0        0      405 2023-04-23 05:55:10.670575 commitizen-3.0.0/commitizen/templates/keep_a_changelog_template.j2
+-rw-r--r--   0        0        0     2400 2023-04-23 05:55:10.674575 commitizen-3.0.0/commitizen/version_types.py
+-rw-r--r--   0        0        0     5800 2023-04-23 05:55:10.674575 commitizen-3.0.0/docs/README.md
+-rw-r--r--   0        0        0     3958 2023-04-23 05:55:10.682575 commitizen-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     7633 1970-01-01 00:00:00.000000 commitizen-3.0.0/PKG-INFO
```

### Comparing `commitizen-2.9.0/LICENSE` & `commitizen-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `commitizen-2.9.0/commitizen/__init__.py` & `commitizen-3.0.0/commitizen/__init__.py`

 * *Files identical despite different names*

### Comparing `commitizen-2.9.0/commitizen/bump.py` & `commitizen-3.0.0/commitizen/bump.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,40 +1,40 @@
+import os
 import re
+import sys
+import typing
 from collections import OrderedDict
 from itertools import zip_longest
 from string import Template
-from typing import List, Optional, Union
+from typing import List, Optional, Tuple, Type, Union
 
 from packaging.version import Version
 
-from commitizen.defaults import (
-    MAJOR,
-    MINOR,
-    PATCH,
-    bump_map,
-    bump_message,
-    bump_pattern,
-)
+from commitizen.defaults import MAJOR, MINOR, PATCH, bump_message
 from commitizen.exceptions import CurrentVersionNotFoundError
-from commitizen.git import GitCommit
+from commitizen.git import GitCommit, smart_open
+
+if sys.version_info >= (3, 8):
+    from commitizen.version_types import VersionProtocol
+else:
+    # workaround mypy issue for 3.7 python
+    VersionProtocol = typing.Any
 
 
 def find_increment(
-    commits: List[GitCommit],
-    regex: str = bump_pattern,
-    increments_map: Union[dict, OrderedDict] = bump_map,
+    commits: List[GitCommit], regex: str, increments_map: Union[dict, OrderedDict]
 ) -> Optional[str]:
 
     if isinstance(increments_map, dict):
         increments_map = OrderedDict(increments_map)
 
     # Most important cases are major and minor.
     # Everything else will be considered patch.
     select_pattern = re.compile(regex)
-    increment = None
+    increment: Optional[str] = None
 
     for commit in commits:
         for message in commit.message.split("\n"):
             result = select_pattern.search(message)
             if result:
                 found_keyword = result.group(0)
                 new_increment = None
@@ -49,15 +49,17 @@
                     increment = new_increment
                 elif increment == "PATCH" or increment is None:
                     increment = new_increment
 
     return increment
 
 
-def prerelease_generator(current_version: str, prerelease: Optional[str] = None) -> str:
+def prerelease_generator(
+    current_version: str, prerelease: Optional[str] = None, offset: int = 0
+) -> str:
     """Generate prerelease
 
     X.YaN   # Alpha release
     X.YbN   # Beta release
     X.YrcN  # Release Candidate
     X.Y  # Final
 
@@ -69,19 +71,31 @@
 
     version = Version(current_version)
     # version.pre is needed for mypy check
     if version.is_prerelease and version.pre and prerelease.startswith(version.pre[0]):
         prev_prerelease: int = version.pre[1]
         new_prerelease_number = prev_prerelease + 1
     else:
-        new_prerelease_number = 0
+        new_prerelease_number = offset
     pre_version = f"{prerelease}{new_prerelease_number}"
     return pre_version
 
 
+def devrelease_generator(devrelease: int = None) -> str:
+    """Generate devrelease
+
+    The devrelease version should be passed directly and is not
+    inferred based on the previous version.
+    """
+    if devrelease is None:
+        return ""
+
+    return f"dev{devrelease}"
+
+
 def semver_generator(current_version: str, increment: str = None) -> str:
     version = Version(current_version)
     prev_release = list(version.release)
     increments = [MAJOR, MINOR, PATCH]
     increments_version = dict(zip_longest(increments, prev_release, fillvalue=0))
 
     # This flag means that current version
@@ -107,100 +121,127 @@
     )
 
 
 def generate_version(
     current_version: str,
     increment: str,
     prerelease: Optional[str] = None,
+    prerelease_offset: int = 0,
+    devrelease: Optional[int] = None,
     is_local_version: bool = False,
-) -> Version:
+    version_type_cls: Optional[Type[VersionProtocol]] = None,
+) -> VersionProtocol:
     """Based on the given increment a proper semver will be generated.
 
     For now the rules and versioning scheme is based on
     python's PEP 0440.
     More info: https://www.python.org/dev/peps/pep-0440/
 
     Example:
         PATCH 1.0.0 -> 1.0.1
         MINOR 1.0.0 -> 1.1.0
         MAJOR 1.0.0 -> 2.0.0
     """
+    if version_type_cls is None:
+        version_type_cls = Version
     if is_local_version:
-        version = Version(current_version)
-        pre_version = prerelease_generator(str(version.local), prerelease=prerelease)
+        version = version_type_cls(current_version)
+        dev_version = devrelease_generator(devrelease=devrelease)
+        pre_version = prerelease_generator(
+            str(version.local), prerelease=prerelease, offset=prerelease_offset
+        )
         semver = semver_generator(str(version.local), increment=increment)
 
-        return Version(f"{version.public}+{semver}{pre_version}")
+        return version_type_cls(f"{version.public}+{semver}{pre_version}{dev_version}")
     else:
-        pre_version = prerelease_generator(current_version, prerelease=prerelease)
+        dev_version = devrelease_generator(devrelease=devrelease)
+        pre_version = prerelease_generator(
+            current_version, prerelease=prerelease, offset=prerelease_offset
+        )
         semver = semver_generator(current_version, increment=increment)
 
         # TODO: post version
-        # TODO: dev version
-        return Version(f"{semver}{pre_version}")
+        return version_type_cls(f"{semver}{pre_version}{dev_version}")
 
 
 def update_version_in_files(
     current_version: str, new_version: str, files: List[str], *, check_consistency=False
-):
+) -> None:
     """Change old version to the new one in every file given.
 
     Note that this version is not the tag formatted one.
     So for example, your tag could look like `v1.0.0` while your version in
     the package like `1.0.0`.
     """
     # TODO: separate check step and write step
     for location in files:
-        filepath, *regexes = location.split(":", maxsplit=1)
-        regex = regexes[0] if regexes else None
-
-        # Read in the file
-        file_content = []
-        current_version_found = False
-        with open(filepath, "r") as version_file:
-            for line in version_file:
-                if regex:
-                    match = re.search(regex, line)
-                    if not match:
-                        file_content.append(line)
-                        continue
-
-                # Replace the target string
-                if current_version in line:
-                    current_version_found = True
-                    file_content.append(line.replace(current_version, new_version))
-                else:
-                    file_content.append(line)
+        drive, tail = os.path.splitdrive(location)
+        path, _, regex = tail.partition(":")
+        filepath = drive + path
+        if not regex:
+            regex = _version_to_regex(current_version)
+
+        current_version_found, version_file = _bump_with_regex(
+            filepath, current_version, new_version, regex
+        )
 
         if check_consistency and not current_version_found:
             raise CurrentVersionNotFoundError(
                 f"Current version {current_version} is not found in {location}.\n"
                 "The version defined in commitizen configuration and the ones in "
                 "version_files are possibly inconsistent."
             )
 
         # Write the file out again
-        with open(filepath, "w") as file:
-            file.write("".join(file_content))
+        with smart_open(filepath, "w") as file:
+            file.write(version_file)
+
+
+def _bump_with_regex(
+    version_filepath: str, current_version: str, new_version: str, regex: str
+) -> Tuple[bool, str]:
+    current_version_found = False
+    lines = []
+    pattern = re.compile(regex)
+    with open(version_filepath, "r") as f:
+        for line in f:
+            if pattern.search(line):
+                bumped_line = line.replace(current_version, new_version)
+                if bumped_line != line:
+                    current_version_found = True
+                lines.append(bumped_line)
+            else:
+                lines.append(line)
+    return current_version_found, "".join(lines)
+
+
+def _version_to_regex(version: str) -> str:
+    return version.replace(".", r"\.").replace("+", r"\+")
 
 
-def create_tag(version: Union[Version, str], tag_format: Optional[str] = None):
+def normalize_tag(
+    version: Union[VersionProtocol, str],
+    tag_format: Optional[str] = None,
+    version_type_cls: Optional[Type[VersionProtocol]] = None,
+) -> str:
     """The tag and the software version might be different.
 
     That's why this function exists.
 
     Example:
     | tag | version (PEP 0440) |
     | --- | ------- |
     | v0.9.0 | 0.9.0 |
     | ver1.0.0 | 1.0.0 |
     | ver1.0.0.a0 | 1.0.0a0 |
     """
+    if version_type_cls is None:
+        version_type_cls = Version
     if isinstance(version, str):
-        version = Version(version)
+        version = version_type_cls(version)
 
     if not tag_format:
         return str(version)
 
     major, minor, patch = version.release
     prerelease = ""
     # version.pre is needed for mypy check
```

### Comparing `commitizen-2.9.0/commitizen/changelog.py` & `commitizen-3.0.0/commitizen/changelog.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,64 +20,81 @@
 - [x] Generate full or partial changelog
 - [x] Include in tree from file all the extra comments added manually
 - [x] Add unreleased value
 - [x] hook after message is parsed (add extra information like hyperlinks)
 - [x] hook after changelog is generated (api calls)
 - [x] add support for change_type maps
 """
+
 import os
 import re
-from collections import defaultdict
+import sys
+import typing
+from collections import OrderedDict, defaultdict
 from datetime import date
-from typing import Callable, Dict, Iterable, List, Optional
+from typing import Callable, Dict, Iterable, List, Optional, Tuple, Type
 
 from jinja2 import Environment, PackageLoader
+from packaging.version import InvalidVersion, Version
 
 from commitizen import defaults
+from commitizen.bump import normalize_tag
+from commitizen.exceptions import InvalidConfigurationError, NoCommitsFoundError
 from commitizen.git import GitCommit, GitTag
 
-CATEGORIES = [
-    ("fix", "fix"),
-    ("breaking", "BREAKING CHANGES"),
-    ("feat", "feat"),
-    ("refactor", "refactor"),
-    ("perf", "perf"),
-    ("test", "test"),
-    ("build", "build"),
-    ("ci", "ci"),
-    ("chore", "chore"),
-]
-
-
-def transform_change_type(change_type: str) -> str:
-    # TODO: Use again to parse, for this we have to wait until the maps get
-    # defined again.
-    _change_type_lower = change_type.lower()
-    for match_value, output in CATEGORIES:
-        if re.search(match_value, _change_type_lower):
-            return output
-    else:
-        raise ValueError(f"Could not match a change_type with {change_type}")
+if sys.version_info >= (3, 8):
+    from commitizen.version_types import VersionProtocol
+else:
+    # workaround mypy issue for 3.7 python
+    VersionProtocol = typing.Any
 
 
 def get_commit_tag(commit: GitCommit, tags: List[GitTag]) -> Optional[GitTag]:
     return next((tag for tag in tags if tag.rev == commit.rev), None)
 
 
+def get_version(tag: GitTag) -> Optional[Version]:
+    version = None
+    try:
+        version = Version(tag.name)
+    except InvalidVersion:
+        pass
+    return version
+
+
+def tag_included_in_changelog(
+    tag: GitTag, used_tags: List, merge_prerelease: bool
+) -> bool:
+    if tag in used_tags:
+        return False
+
+    version = get_version(tag)
+    if version is None:
+        return False
+
+    if merge_prerelease and version.is_prerelease:
+        return False
+
+    return True
+
+
 def generate_tree_from_commits(
     commits: List[GitCommit],
     tags: List[GitTag],
     commit_parser: str,
-    changelog_pattern: str = defaults.bump_pattern,
+    changelog_pattern: str,
     unreleased_version: Optional[str] = None,
     change_type_map: Optional[Dict[str, str]] = None,
     changelog_message_builder_hook: Optional[Callable] = None,
+    merge_prerelease: bool = False,
 ) -> Iterable[Dict]:
     pat = re.compile(changelog_pattern)
     map_pat = re.compile(commit_parser, re.MULTILINE)
+    body_map_pat = re.compile(commit_parser, re.MULTILINE | re.DOTALL)
+
     # Check if the latest commit is not tagged
     latest_commit = commits[0]
     current_tag: Optional[GitTag] = get_commit_tag(latest_commit, tags)
 
     current_tag_name: str = unreleased_version or "Unreleased"
     current_tag_date: str = ""
     if unreleased_version is not None:
@@ -87,51 +104,80 @@
         current_tag_date = current_tag.date
 
     changes: Dict = defaultdict(list)
     used_tags: List = [current_tag]
     for commit in commits:
         commit_tag = get_commit_tag(commit, tags)
 
-        if commit_tag is not None and commit_tag not in used_tags:
+        if commit_tag is not None and tag_included_in_changelog(
+            commit_tag, used_tags, merge_prerelease
+        ):
             used_tags.append(commit_tag)
             yield {
                 "version": current_tag_name,
                 "date": current_tag_date,
                 "changes": changes,
             }
-            # TODO: Check if tag matches the version pattern, otherwie skip it.
-            # This in order to prevent tags that are not versions.
             current_tag_name = commit_tag.name
             current_tag_date = commit_tag.date
             changes = defaultdict(list)
 
         matches = pat.match(commit.message)
         if not matches:
             continue
 
+        # Process subject from commit message
         message = map_pat.match(commit.message)
-        message_body = map_pat.search(commit.body)
         if message:
             parsed_message: Dict = message.groupdict()
             # change_type becomes optional by providing None
             change_type = parsed_message.pop("change_type", None)
 
             if change_type_map:
                 change_type = change_type_map.get(change_type, change_type)
             if changelog_message_builder_hook:
                 parsed_message = changelog_message_builder_hook(parsed_message, commit)
             changes[change_type].append(parsed_message)
-        if message_body:
+
+        # Process body from commit message
+        body_parts = commit.body.split("\n\n")
+        for body_part in body_parts:
+            message_body = body_map_pat.match(body_part)
+            if not message_body:
+                continue
             parsed_message_body: Dict = message_body.groupdict()
+
             change_type = parsed_message_body.pop("change_type", None)
+            if change_type_map:
+                change_type = change_type_map.get(change_type, change_type)
             changes[change_type].append(parsed_message_body)
 
     yield {"version": current_tag_name, "date": current_tag_date, "changes": changes}
 
 
+def order_changelog_tree(tree: Iterable, change_type_order: List[str]) -> Iterable:
+    if len(set(change_type_order)) != len(change_type_order):
+        raise InvalidConfigurationError(
+            f"Change types contain duplicates types ({change_type_order})"
+        )
+
+    sorted_tree = []
+    for entry in tree:
+        ordered_change_types = change_type_order + sorted(
+            set(entry["changes"].keys()) - set(change_type_order)
+        )
+        changes = [
+            (ct, entry["changes"][ct])
+            for ct in ordered_change_types
+            if ct in entry["changes"]
+        ]
+        sorted_tree.append({**entry, **{"changes": OrderedDict(changes)}})
+    return sorted_tree
+
+
 def render_changelog(tree: Iterable) -> str:
     loader = PackageLoader("commitizen", "templates")
     env = Environment(loader=loader, trim_blocks=True)
     jinja_template = env.get_template("keep_a_changelog_template.j2")
     changelog: str = jinja_template.render(tree=tree)
     return changelog
 
@@ -197,33 +243,33 @@
         "unreleased_start": unreleased_start,
         "unreleased_end": unreleased_end,
         "latest_version": latest_version,
         "latest_version_position": latest_version_position,
     }
 
 
-def incremental_build(new_content: str, lines: List, metadata: Dict) -> List:
+def incremental_build(new_content: str, lines: List[str], metadata: Dict) -> List[str]:
     """Takes the original lines and updates with new_content.
 
-    The metadata holds information enough to remove the old unreleased and
-    where to place the new content
+    The metadata governs how to remove the old unreleased section and where to place the
+    new content.
 
     Args:
         lines: The lines from the changelog
         new_content: This should be placed somewhere in the lines
         metadata: Information about the changelog
 
     Returns:
         Updated lines
     """
     unreleased_start = metadata.get("unreleased_start")
     unreleased_end = metadata.get("unreleased_end")
     latest_version_position = metadata.get("latest_version_position")
     skip = False
-    output_lines: List = []
+    output_lines: List[str] = []
     for index, line in enumerate(lines):
         if index == unreleased_start:
             skip = True
         elif index == unreleased_end:
             skip = False
             if (
                 latest_version_position is None
@@ -232,19 +278,92 @@
                 and latest_version_position > unreleased_end
             ):
                 continue
 
         if skip:
             continue
 
-        if (
-            isinstance(latest_version_position, int)
-            and index == latest_version_position
-        ):
-
-            output_lines.append(new_content)
-            output_lines.append("\n")
+        if index == latest_version_position:
+            output_lines.extend([new_content, "\n"])
 
         output_lines.append(line)
     if not isinstance(latest_version_position, int):
+        if output_lines and output_lines[-1].strip():
+            # Ensure at least one blank line between existing and new content.
+            output_lines.append("\n")
         output_lines.append(new_content)
     return output_lines
+
+
+def get_smart_tag_range(
+    tags: List[GitTag], newest: str, oldest: Optional[str] = None
+) -> List[GitTag]:
+    """Smart because it finds the N+1 tag.
+
+    This is because we need to find until the next tag
+    """
+    accumulator = []
+    keep = False
+    if not oldest:
+        oldest = newest
+    for index, tag in enumerate(tags):
+        if tag.name == newest:
+            keep = True
+        if keep:
+            accumulator.append(tag)
+        if tag.name == oldest:
+            keep = False
+            try:
+                accumulator.append(tags[index + 1])
+            except IndexError:
+                pass
+            break
+    return accumulator
+
+
+def get_oldest_and_newest_rev(
+    tags: List[GitTag],
+    version: str,
+    tag_format: str,
+    version_type_cls: Optional[Type[VersionProtocol]] = None,
+) -> Tuple[Optional[str], Optional[str]]:
+    """Find the tags for the given version.
+
+    `version` may come in different formats:
+    - `0.1.0..0.4.0`: as a range
+    - `0.3.0`: as a single version
+    """
+    oldest: Optional[str] = None
+    newest: Optional[str] = None
+    try:
+        oldest, newest = version.split("..")
+    except ValueError:
+        newest = version
+
+    newest_tag = normalize_tag(
+        newest, tag_format=tag_format, version_type_cls=version_type_cls
+    )
+
+    oldest_tag = None
+    if oldest:
+        oldest_tag = normalize_tag(
+            oldest, tag_format=tag_format, version_type_cls=version_type_cls
+        )
+
+    tags_range = get_smart_tag_range(tags, newest=newest_tag, oldest=oldest_tag)
+    if not tags_range:
+        raise NoCommitsFoundError("Could not find a valid revision range.")
+
+    oldest_rev: Optional[str] = tags_range[-1].name
+    newest_rev = newest_tag
+
+    # check if it's the first tag created
+    # and it's also being requested as part of the range
+    if oldest_rev == tags[-1].name and oldest_rev == oldest_tag:
+        return None, newest_rev
+
+    # when they are the same, and it's also the
+    # first tag created
+    if oldest_rev == newest_rev:
+        return None, newest_rev
+
+    return oldest_rev, newest_rev
```

### Comparing `commitizen-2.9.0/commitizen/changelog_parser.py` & `commitizen-3.0.0/commitizen/changelog_parser.py`

 * *Files identical despite different names*

### Comparing `commitizen-2.9.0/commitizen/commands/changelog.py` & `commitizen-3.0.0/commitizen/commands/changelog.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 import os.path
 from difflib import SequenceMatcher
 from operator import itemgetter
 from typing import Callable, Dict, List, Optional
 
-from commitizen import changelog, factory, git, out
+from commitizen import bump, changelog, defaults, factory, git, out, version_types
 from commitizen.config import BaseConfig
 from commitizen.exceptions import (
     DryRunExit,
     NoCommitsFoundError,
     NoPatternMapError,
     NoRevisionError,
     NotAGitProjectError,
+    NotAllowed,
 )
-from commitizen.git import GitTag
-
-
-def similar(a, b):
-    return SequenceMatcher(None, a, b).ratio()
+from commitizen.git import GitTag, smart_open
 
 
 class Changelog:
     """Generate a changelog based on the commit history."""
 
     def __init__(self, config: BaseConfig, args):
         if not git.is_git_project():
@@ -39,14 +36,29 @@
             "changelog_incremental"
         )
         self.dry_run = args["dry_run"]
         self.unreleased_version = args["unreleased_version"]
         self.change_type_map = (
             self.config.settings.get("change_type_map") or self.cz.change_type_map
         )
+        self.change_type_order = (
+            self.config.settings.get("change_type_order")
+            or self.cz.change_type_order
+            or defaults.change_type_order
+        )
+        self.rev_range = args.get("rev_range")
+        self.tag_format = args.get("tag_format") or self.config.settings.get(
+            "tag_format"
+        )
+        self.merge_prerelease = args.get(
+            "merge_prerelease"
+        ) or self.config.settings.get("changelog_merge_prerelease")
+
+        version_type = self.config.settings.get("version_type")
+        self.version_type = version_type and version_types.VERSION_TYPES[version_type]
 
     def _find_incremental_rev(self, latest_version: str, tags: List[GitTag]) -> str:
         """Try to find the 'start_rev'.
 
         We use a similarity approach. We know how to parse the version from the markdown
         changelog, but not the whole tag, we don't even know how's the tag made.
 
@@ -66,70 +78,108 @@
         except ValueError:
             raise NoRevisionError()
         if score < SIMILARITY_THRESHOLD:
             raise NoRevisionError()
         start_rev = tag.name
         return start_rev
 
+    def write_changelog(
+        self, changelog_out: str, lines: List[str], changelog_meta: Dict
+    ):
+        if not isinstance(self.file_name, str):
+            raise NotAllowed(
+                "Changelog file name is broken.\n"
+                "Check the flag `--file-name` in the terminal "
+                f"or the setting `changelog_file` in {self.config.path}"
+            )
+
+        changelog_hook: Optional[Callable] = self.cz.changelog_hook
+        with smart_open(self.file_name, "w") as changelog_file:
+            partial_changelog: Optional[str] = None
+            if self.incremental:
+                new_lines = changelog.incremental_build(
+                    changelog_out, lines, changelog_meta
+                )
+                changelog_out = "".join(new_lines)
+                partial_changelog = changelog_out
+
+            if changelog_hook:
+                changelog_out = changelog_hook(changelog_out, partial_changelog)
+            changelog_file.write(changelog_out)
+
     def __call__(self):
         commit_parser = self.cz.commit_parser
         changelog_pattern = self.cz.changelog_pattern
         start_rev = self.start_rev
         unreleased_version = self.unreleased_version
         changelog_meta: Dict = {}
         change_type_map: Optional[Dict] = self.change_type_map
         changelog_message_builder_hook: Optional[
             Callable
         ] = self.cz.changelog_message_builder_hook
-        changelog_hook: Optional[Callable] = self.cz.changelog_hook
+        merge_prerelease = self.merge_prerelease
+
         if not changelog_pattern or not commit_parser:
             raise NoPatternMapError(
                 f"'{self.config.settings['name']}' rule does not support changelog"
             )
 
+        if self.incremental and self.rev_range:
+            raise NotAllowed("--incremental cannot be combined with a rev_range")
+
+        # Don't continue if no `file_name` specified.
+        assert self.file_name
+
         tags = git.get_tags()
         if not tags:
             tags = []
 
+        end_rev = ""
+
         if self.incremental:
             changelog_meta = changelog.get_metadata(self.file_name)
             latest_version = changelog_meta.get("latest_version")
             if latest_version:
-                start_rev = self._find_incremental_rev(latest_version, tags)
+                latest_tag_version: str = bump.normalize_tag(
+                    latest_version,
+                    tag_format=self.tag_format,
+                    version_type_cls=self.version_type,
+                )
+                start_rev = self._find_incremental_rev(latest_tag_version, tags)
 
-        commits = git.get_commits(start=start_rev, args="--author-date-order")
+        if self.rev_range:
+            start_rev, end_rev = changelog.get_oldest_and_newest_rev(
+                tags,
+                version=self.rev_range,
+                tag_format=self.tag_format,
+                version_type_cls=self.version_type,
+            )
+
+        commits = git.get_commits(start=start_rev, end=end_rev, args="--topo-order")
         if not commits:
             raise NoCommitsFoundError("No commits found")
 
         tree = changelog.generate_tree_from_commits(
             commits,
             tags,
             commit_parser,
             changelog_pattern,
             unreleased_version,
             change_type_map=change_type_map,
             changelog_message_builder_hook=changelog_message_builder_hook,
+            merge_prerelease=merge_prerelease,
         )
+        if self.change_type_order:
+            tree = changelog.order_changelog_tree(tree, self.change_type_order)
         changelog_out = changelog.render_changelog(tree)
         changelog_out = changelog_out.lstrip("\n")
 
         if self.dry_run:
             out.write(changelog_out)
             raise DryRunExit()
 
         lines = []
         if self.incremental and os.path.isfile(self.file_name):
             with open(self.file_name, "r") as changelog_file:
                 lines = changelog_file.readlines()
 
-        with open(self.file_name, "w") as changelog_file:
-            partial_changelog: Optional[str] = None
-            if self.incremental:
-                new_lines = changelog.incremental_build(
-                    changelog_out, lines, changelog_meta
-                )
-                changelog_out = "".join(new_lines)
-                partial_changelog = changelog_out
-
-            if changelog_hook:
-                changelog_out = changelog_hook(changelog_out, partial_changelog)
-            changelog_file.write(changelog_out)
+        self.write_changelog(changelog_out, lines, changelog_meta)
```

### Comparing `commitizen-2.9.0/commitizen/commands/check.py` & `commitizen-3.0.0/commitizen/commands/check.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,55 @@
 import os
 import re
 import sys
-from typing import Dict, Optional
+from typing import Any, Dict, Optional
 
 from commitizen import factory, git, out
 from commitizen.config import BaseConfig
 from commitizen.exceptions import (
     InvalidCommandArgumentError,
     InvalidCommitMessageError,
     NoCommitsFoundError,
 )
 
 
 class Check:
     """Check if the current commit msg matches the commitizen format."""
 
-    def __init__(self, config: BaseConfig, arguments: Dict[str, str], cwd=os.getcwd()):
+    def __init__(self, config: BaseConfig, arguments: Dict[str, Any], cwd=os.getcwd()):
         """Initial check command.
 
         Args:
             config: The config object required for the command to perform its action
             arguments: All the flags provided by the user
             cwd: Current work directory
         """
         self.commit_msg_file: Optional[str] = arguments.get("commit_msg_file")
         self.commit_msg: Optional[str] = arguments.get("message")
         self.rev_range: Optional[str] = arguments.get("rev_range")
+        self.allow_abort: bool = bool(
+            arguments.get("allow_abort", config.settings["allow_abort"])
+        )
 
         self._valid_command_argument()
 
         self.config: BaseConfig = config
         self.cz = factory.commiter_factory(self.config)
 
     def _valid_command_argument(self):
-        number_args_provided = (
-            bool(self.commit_msg_file) + bool(self.commit_msg) + bool(self.rev_range)
+        num_exclusive_args_provided = sum(
+            arg is not None
+            for arg in (self.commit_msg_file, self.commit_msg, self.rev_range)
         )
-        if number_args_provided == 0 and not os.isatty(0):
+        if num_exclusive_args_provided == 0 and not sys.stdin.isatty():
             self.commit_msg: Optional[str] = sys.stdin.read()
-        elif number_args_provided != 1:
+        elif num_exclusive_args_provided != 1:
             raise InvalidCommandArgumentError(
                 (
-                    "One and only one argument is required for check command! "
+                    "Only one of --rev-range, --message, and --commit-msg-file is permitted by check command! "
                     "See 'cz check -h' for more information"
                 )
             )
 
     def __call__(self):
         """Validate if commit messages follows the conventional pattern.
 
@@ -56,15 +60,15 @@
         if not commits:
             raise NoCommitsFoundError(f"No commit found with range: '{self.rev_range}'")
 
         pattern = self.cz.schema_pattern()
         ill_formated_commits = [
             commit
             for commit in commits
-            if not Check.validate_commit_message(commit.message, pattern)
+            if not self.validate_commit_message(commit.message, pattern)
         ]
         displayed_msgs_content = "\n".join(
             [
                 f'commit "{commit.rev}": "{commit.message}"'
                 for commit in ill_formated_commits
             ]
         )
@@ -74,24 +78,66 @@
                 "please enter a commit message in the commitizen format.\n"
                 f"{displayed_msgs_content}\n"
                 f"pattern: {pattern}"
             )
         out.success("Commit validation: successful!")
 
     def _get_commits(self):
+        msg = None
         # Get commit message from file (--commit-msg-file)
-        if self.commit_msg_file:
-            with open(self.commit_msg_file, "r") as commit_file:
-                commit_title = commit_file.readline()
-                commit_body = commit_file.read()
-            return [git.GitCommit(rev="", title=commit_title, body=commit_body)]
-        elif self.commit_msg:
-            return [git.GitCommit(rev="", title="", body=self.commit_msg)]
+        if self.commit_msg_file is not None:
+            # Enter this branch if commit_msg_file is "".
+            with open(self.commit_msg_file, "r", encoding="utf-8") as commit_file:
+                msg = commit_file.read()
+        # Get commit message from command line (--message)
+        elif self.commit_msg is not None:
+            msg = self.commit_msg
+        if msg is not None:
+            msg = self._filter_comments(msg)
+            return [git.GitCommit(rev="", title="", body=msg)]
 
         # Get commit messages from git log (--rev-range)
         return git.get_commits(end=self.rev_range)
 
     @staticmethod
-    def validate_commit_message(commit_msg: str, pattern: str) -> bool:
-        if commit_msg.startswith("Merge") or commit_msg.startswith("Revert"):
+    def _filter_comments(msg: str) -> str:
+        """Filter the commit message by removing comments.
+
+        When using `git commit --verbose`, we exclude the diff that is going to
+        generated, like the following example:
+
+        ```bash
+        ...
+        # ------------------------ >8 ------------------------
+        # Do not modify or remove the line above.
+        # Everything below it will be ignored.
+        diff --git a/... b/...
+        ...
+        ```
+
+        Args:
+            msg: The commit message to filter.
+
+        Returns:
+            The filtered commit message without comments.
+        """
+
+        lines = []
+        for line in msg.split("\n"):
+            if "# ------------------------ >8 ------------------------" in line:
+                break
+            if not line.startswith("#"):
+                lines.append(line)
+        return "\n".join(lines)
+
+    def validate_commit_message(self, commit_msg: str, pattern: str) -> bool:
+        if not commit_msg:
+            return self.allow_abort
+        if (
+            commit_msg.startswith("Merge")
+            or commit_msg.startswith("Revert")
+            or commit_msg.startswith("Pull request")
+            or commit_msg.startswith("fixup!")
+            or commit_msg.startswith("squash!")
+        ):
             return True
         return bool(re.match(pattern, commit_msg))
```

### Comparing `commitizen-2.9.0/commitizen/commands/commit.py` & `commitizen-3.0.0/commitizen/commands/commit.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,41 +12,47 @@
     CustomError,
     DryRunExit,
     NoAnswersError,
     NoCommitBackupError,
     NotAGitProjectError,
     NothingToCommitError,
 )
+from commitizen.git import smart_open
 
 
 class Commit:
     """Show prompt for the user to create a guided commit."""
 
     def __init__(self, config: BaseConfig, arguments: dict):
         if not git.is_git_project():
             raise NotAGitProjectError()
 
         self.config: BaseConfig = config
         self.cz = factory.commiter_factory(self.config)
         self.arguments = arguments
-        self.temp_file: str = os.path.join(tempfile.gettempdir(), "cz.commit.backup")
+        self.temp_file: str = os.path.join(
+            tempfile.gettempdir(),
+            "cz.commit{user}.backup".format(user=os.environ.get("USER", "")),
+        )
 
     def read_backup_message(self) -> str:
         # Check the commit backup file exists
         if not os.path.isfile(self.temp_file):
             raise NoCommitBackupError()
 
         # Read commit message from backup
         with open(self.temp_file, "r") as f:
             return f.read().strip()
 
     def prompt_commit_questions(self) -> str:
         # Prompt user for the commit message
         cz = self.cz
         questions = cz.questions()
+        for question in filter(lambda q: q["type"] == "list", questions):
+            question["use_shortcuts"] = self.config.settings["use_shortcuts"]
         try:
             answers = questionary.prompt(questions, style=cz.style)
         except ValueError as err:
             root_err = err.__context__
             if isinstance(root_err, CzException):
                 raise CustomError(root_err.__str__())
             raise err
@@ -69,21 +75,26 @@
             m = self.prompt_commit_questions()
 
         out.info(f"\n{m}\n")
 
         if dry_run:
             raise DryRunExit()
 
-        c = git.commit(m)
+        signoff: bool = self.arguments.get("signoff")
+
+        if signoff:
+            c = git.commit(m, "-s")
+        else:
+            c = git.commit(m)
 
         if c.return_code != 0:
             out.error(c.err)
 
             # Create commit backup
-            with open(self.temp_file, "w") as f:
+            with smart_open(self.temp_file, "w") as f:
                 f.write(m)
 
             raise CommitError()
 
         if "nothing added" in c.out or "no changes added to commit" in c.out:
             out.error(c.out)
         else:
```

### Comparing `commitizen-2.9.0/commitizen/commands/version.py` & `commitizen-3.0.0/commitizen/commands/version.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,39 @@
+import platform
+import sys
+
 from commitizen import out
 from commitizen.__version__ import __version__
 from commitizen.config import BaseConfig
+from commitizen.providers import get_provider
 
 
 class Version:
     """Get the version of the installed commitizen or the current project."""
 
     def __init__(self, config: BaseConfig, *args):
         self.config: BaseConfig = config
         self.parameter = args[0]
+        self.operating_system = platform.system()
+        self.python_version = sys.version
 
     def __call__(self):
-        if self.parameter.get("project"):
-            version = self.config.settings["version"]
+        if self.parameter.get("report"):
+            out.write(f"Commitizen Version: {__version__}")
+            out.write(f"Python Version: {self.python_version}")
+            out.write(f"Operating System: {self.operating_system}")
+        elif self.parameter.get("project"):
+            version = get_provider(self.config).get_version()
             if version:
                 out.write(f"{version}")
             else:
                 out.error("No project information in this project.")
         elif self.parameter.get("verbose"):
             out.write(f"Installed Commitizen Version: {__version__}")
-            version = self.config.settings["version"]
+            version = get_provider(self.config).get_version()
             if version:
                 out.write(f"Project Version: {version}")
             else:
                 out.error("No project information in this project.")
         else:
             # if no argument is given, show installed commitizen version
             out.write(f"{__version__}")
```

### Comparing `commitizen-2.9.0/commitizen/config/__init__.py` & `commitizen-3.0.0/commitizen/config/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Union
 
 from commitizen import defaults, git
 
 from .base_config import BaseConfig
 from .json_config import JsonConfig
 from .toml_config import TomlConfig
+from .yaml_config import YAMLConfig
 
 
 def read_cfg() -> BaseConfig:
     conf = BaseConfig()
 
     git_project_root = git.find_git_project_root()
     cfg_search_paths = [Path(".")]
@@ -21,23 +22,25 @@
         for path in cfg_search_paths
         for filename in defaults.config_files
     )
     for filename in cfg_paths:
         if not filename.exists():
             continue
 
-        with open(filename, "r") as f:
-            data: str = f.read()
+        _conf: Union[TomlConfig, JsonConfig, YAMLConfig]
+
+        with open(filename, "rb") as f:
+            data: bytes = f.read()
 
-        _conf: Union[TomlConfig, JsonConfig]
         if "toml" in filename.suffix:
             _conf = TomlConfig(data=data, path=filename)
-
-        if "json" in filename.suffix:
+        elif "json" in filename.suffix:
             _conf = JsonConfig(data=data, path=filename)
+        elif "yaml" in filename.suffix:
+            _conf = YAMLConfig(data=data, path=filename)
 
         if _conf.is_empty_config:
             continue
         else:
             conf = _conf
             break
```

### Comparing `commitizen-2.9.0/commitizen/config/base_config.py` & `commitizen-3.0.0/commitizen/config/base_config.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 from pathlib import Path
-from typing import Any, Dict, Optional, Union
+from typing import Optional, Union
 
-from commitizen.defaults import DEFAULT_SETTINGS
+from commitizen.defaults import DEFAULT_SETTINGS, Settings
 
 
 class BaseConfig:
     def __init__(self):
-        self._settings: Dict[str, Any] = DEFAULT_SETTINGS.copy()
+        self._settings: Settings = DEFAULT_SETTINGS.copy()
         self._path: Optional[Path] = None
 
     @property
-    def settings(self) -> Dict[str, Any]:
+    def settings(self) -> Settings:
         return self._settings
 
     @property
     def path(self) -> Optional[Path]:
         return self._path
 
     def set_key(self, key, value):
         """Set or update a key in the conf.
 
         For now only strings are supported.
         We use to update the version number.
         """
         raise NotImplementedError()
 
-    def update(self, data: dict):
+    def update(self, data: Settings) -> None:
         self._settings.update(data)
 
-    def add_path(self, path: Union[str, Path]):
+    def add_path(self, path: Union[str, Path]) -> None:
         self._path = Path(path)
 
-    def _parse_setting(self, data: str) -> dict:
+    def _parse_setting(self, data: Union[bytes, str]) -> None:
         raise NotImplementedError()
```

### Comparing `commitizen-2.9.0/commitizen/config/json_config.py` & `commitizen-3.0.0/commitizen/config/json_config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 import json
 from pathlib import Path
 from typing import Union
 
+from commitizen.git import smart_open
+
 from .base_config import BaseConfig
 
 
 class JsonConfig(BaseConfig):
-    def __init__(self, *, data: str, path: Union[Path, str]):
+    def __init__(self, *, data: Union[bytes, str], path: Union[Path, str]):
         super(JsonConfig, self).__init__()
         self.is_empty_config = False
         self._parse_setting(data)
         self.add_path(path)
 
     def init_empty_config_content(self):
-        with open(self.path, "a") as json_file:
+        with smart_open(self.path, "a") as json_file:
             json.dump({"commitizen": {}}, json_file)
 
     def set_key(self, key, value):
         """Set or update a key in the conf.
 
         For now only strings are supported.
         We use to update the version number.
         """
-        with open(self.path, "r") as f:
+        with open(self.path, "rb") as f:
             parser = json.load(f)
 
         parser["commitizen"][key] = value
-        with open(self.path, "w") as f:
-            json.dump(parser, f)
+        with smart_open(self.path, "w") as f:
+            json.dump(parser, f, indent=2)
         return self
 
-    def _parse_setting(self, data: str):
+    def _parse_setting(self, data: Union[bytes, str]) -> None:
         """We expect to have a section in .cz.json looking like
 
         ```
         {
             "commitizen": {
                 "name": "cz_conventional_commits"
             }
```

### Comparing `commitizen-2.9.0/commitizen/config/toml_config.py` & `commitizen-3.0.0/commitizen/config/yaml_config.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,49 @@
 from pathlib import Path
 from typing import Union
 
-from tomlkit import exceptions, parse
+import yaml
+
+from commitizen.git import smart_open
 
 from .base_config import BaseConfig
 
 
-class TomlConfig(BaseConfig):
-    def __init__(self, *, data: str, path: Union[Path, str]):
-        super(TomlConfig, self).__init__()
+class YAMLConfig(BaseConfig):
+    def __init__(self, *, data: Union[bytes, str], path: Union[Path, str]):
+        super(YAMLConfig, self).__init__()
         self.is_empty_config = False
         self._parse_setting(data)
         self.add_path(path)
 
     def init_empty_config_content(self):
-        with open(self.path, "a") as toml_file:
-            toml_file.write("[tool.commitizen]")
+        with smart_open(self.path, "a") as json_file:
+            yaml.dump({"commitizen": {}}, json_file, explicit_start=True)
+
+    def _parse_setting(self, data: Union[bytes, str]) -> None:
+        """We expect to have a section in cz.yaml looking like
+
+        ```
+        commitizen:
+          name: cz_conventional_commits
+        ```
+        """
+        doc = yaml.safe_load(data)
+        try:
+            self.settings.update(doc["commitizen"])
+        except (KeyError, TypeError):
+            self.is_empty_config = True
 
     def set_key(self, key, value):
         """Set or update a key in the conf.
 
         For now only strings are supported.
         We use to update the version number.
         """
-        with open(self.path, "r") as f:
-            parser = parse(f.read())
+        with open(self.path, "rb") as yaml_file:
+            parser = yaml.load(yaml_file, Loader=yaml.FullLoader)
 
-        parser["tool"]["commitizen"][key] = value
-        with open(self.path, "w") as f:
-            f.write(parser.as_string())
-        return self
-
-    def _parse_setting(self, data: str):
-        """We expect to have a section in pyproject looking like
+        parser["commitizen"][key] = value
+        with smart_open(self.path, "w") as yaml_file:
+            yaml.dump(parser, yaml_file, explicit_start=True)
 
-        ```
-        [tool.commitizen]
-        name = "cz_conventional_commits"
-        ```
-        """
-        doc = parse(data)
-        try:
-            self.settings.update(doc["tool"]["commitizen"])
-        except exceptions.NonExistentKey:
-            self.is_empty_config = True
+        return self
```

### Comparing `commitizen-2.9.0/commitizen/cz/base.py` & `commitizen-3.0.0/commitizen/cz/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from abc import ABCMeta, abstractmethod
 from typing import Callable, Dict, List, Optional, Tuple
 
 from prompt_toolkit.styles import Style, merge_styles
 
 from commitizen import git
 from commitizen.config.base_config import BaseConfig
+from commitizen.defaults import Questions
 
 
 class BaseCommitizen(metaclass=ABCMeta):
     bump_pattern: Optional[str] = None
-    bump_map: Optional[dict] = None
+    bump_map: Optional[Dict[str, str]] = None
     default_style_config: List[Tuple[str, str]] = [
         ("qmark", "fg:#ff9d00 bold"),
         ("question", "bold"),
         ("answer", "fg:#ff9d00 bold"),
         ("pointer", "fg:#ff9d00 bold"),
         ("highlighted", "fg:#ff9d00 bold"),
         ("selected", "fg:#cc5454"),
@@ -25,14 +26,15 @@
 
     # The whole subject will be parsed as message by default
     # This allows supporting changelog for any rule system.
     # It can be modified per rule
     commit_parser: Optional[str] = r"(?P<message>.*)"
     changelog_pattern: Optional[str] = r".*"
     change_type_map: Optional[Dict[str, str]] = None
+    change_type_order: Optional[List[str]] = None
 
     # Executed per message parsed by the commitizen
     changelog_message_builder_hook: Optional[
         Callable[[Dict, git.GitCommit], Dict]
     ] = None
 
     # Executed only at the end of the changelog generation
@@ -40,15 +42,15 @@
 
     def __init__(self, config: BaseConfig):
         self.config = config
         if not self.config.settings.get("style"):
             self.config.settings.update({"style": BaseCommitizen.default_style_config})
 
     @abstractmethod
-    def questions(self) -> list:
+    def questions(self) -> Questions:
         """Questions regarding the commit message."""
 
     @abstractmethod
     def message(self, answers: dict) -> str:
         """Format your git message."""
 
     @property
```

### Comparing `commitizen-2.9.0/commitizen/cz/conventional_commits/conventional_commits.py` & `commitizen-3.0.0/commitizen/cz/conventional_commits/conventional_commits.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import re
-from typing import Any, Dict, List
 
 from commitizen import defaults
 from commitizen.cz.base import BaseCommitizen
 from commitizen.cz.utils import multiple_line_breaker, required_validator
+from commitizen.defaults import Questions
 
 __all__ = ["ConventionalCommitsCz"]
 
 
 def parse_scope(text):
     if not text:
         return ""
@@ -27,76 +27,89 @@
     return required_validator(text, msg="Subject is required.")
 
 
 class ConventionalCommitsCz(BaseCommitizen):
     bump_pattern = defaults.bump_pattern
     bump_map = defaults.bump_map
     commit_parser = defaults.commit_parser
-    changelog_pattern = defaults.bump_pattern
+    version_parser = defaults.version_parser
     change_type_map = {
         "feat": "Feat",
         "fix": "Fix",
         "refactor": "Refactor",
         "perf": "Perf",
     }
+    changelog_pattern = defaults.bump_pattern
 
-    def questions(self) -> List[Dict[str, Any]]:
-        questions: List[Dict[str, Any]] = [
+    def questions(self) -> Questions:
+        questions: Questions = [
             {
                 "type": "list",
                 "name": "prefix",
                 "message": "Select the type of change you are committing",
                 "choices": [
                     {
                         "value": "fix",
                         "name": "fix: A bug fix. Correlates with PATCH in SemVer",
+                        "key": "x",
                     },
                     {
                         "value": "feat",
                         "name": "feat: A new feature. Correlates with MINOR in SemVer",
+                        "key": "f",
+                    },
+                    {
+                        "value": "docs",
+                        "name": "docs: Documentation only changes",
+                        "key": "d",
                     },
-                    {"value": "docs", "name": "docs: Documentation only changes"},
                     {
                         "value": "style",
                         "name": (
                             "style: Changes that do not affect the "
                             "meaning of the code (white-space, formatting,"
                             " missing semi-colons, etc)"
                         ),
+                        "key": "s",
                     },
                     {
                         "value": "refactor",
                         "name": (
                             "refactor: A code change that neither fixes "
                             "a bug nor adds a feature"
                         ),
+                        "key": "r",
                     },
                     {
                         "value": "perf",
                         "name": "perf: A code change that improves performance",
+                        "key": "p",
                     },
                     {
                         "value": "test",
                         "name": (
                             "test: Adding missing or correcting " "existing tests"
                         ),
+                        "key": "t",
                     },
                     {
                         "value": "build",
                         "name": (
                             "build: Changes that affect the build system or "
                             "external dependencies (example scopes: pip, docker, npm)"
                         ),
+                        "key": "b",
                     },
                     {
                         "value": "ci",
                         "name": (
                             "ci: Changes to our CI configuration files and "
                             "scripts (example scopes: GitLabCI)"
                         ),
+                        "key": "c",
                     },
                 ],
             },
             {
                 "type": "input",
                 "name": "scope",
                 "message": (
@@ -174,16 +187,19 @@
             "<body>\n"
             "<BLANK LINE>\n"
             "(BREAKING CHANGE: )<footer>"
         )
 
     def schema_pattern(self) -> str:
         PATTERN = (
-            r"(build|ci|docs|feat|fix|perf|refactor|style|test|chore|revert|bump)!?"
-            r"(\(\S+\))?:(\s.*)"
+            r"(?s)"  # To explictly make . match new line
+            r"(build|ci|docs|feat|fix|perf|refactor|style|test|chore|revert|bump)"  # type
+            r"(\(\S+\))?!?:"  # scope
+            r"( [^\n\r]+)"  # subject
+            r"((\n\n.*)|(\s*))?$"
         )
         return PATTERN
 
     def info(self) -> str:
         dir_path = os.path.dirname(os.path.realpath(__file__))
         filepath = os.path.join(dir_path, "conventional_commits_info.txt")
         with open(filepath, "r") as f:
```

### Comparing `commitizen-2.9.0/commitizen/cz/conventional_commits/conventional_commits_info.txt` & `commitizen-3.0.0/commitizen/cz/conventional_commits/conventional_commits_info.txt`

 * *Files identical despite different names*

### Comparing `commitizen-2.9.0/commitizen/cz/jira/jira.py` & `commitizen-3.0.0/commitizen/cz/jira/jira.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import os
-from typing import Any, Dict, List
 
 from commitizen.cz.base import BaseCommitizen
+from commitizen.defaults import Questions
 
 __all__ = ["JiraSmartCz"]
 
 
 class JiraSmartCz(BaseCommitizen):
-    def questions(self) -> List[Dict[str, Any]]:
+    def questions(self) -> Questions:
         questions = [
             {
                 "type": "input",
                 "name": "message",
                 "message": "Git commit message (required):\n",
                 # 'validate': RequiredValidator,
                 "filter": lambda x: x.strip(),
```

### Comparing `commitizen-2.9.0/commitizen/cz/jira/jira_info.txt` & `commitizen-3.0.0/commitizen/cz/jira/jira_info.txt`

 * *Files identical despite different names*

### Comparing `commitizen-2.9.0/commitizen/exceptions.py` & `commitizen-3.0.0/commitizen/exceptions.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,14 +19,23 @@
     CUSTOM_ERROR = 12
     NO_COMMAND_FOUND = 13
     INVALID_COMMIT_MSG = 14
     MISSING_CZ_CUSTOMIZE_CONFIG = 15
     NO_REVISION = 16
     CURRENT_VERSION_NOT_FOUND = 17
     INVALID_COMMAND_ARGUMENT = 18
+    INVALID_CONFIGURATION = 19
+    NOT_ALLOWED = 20
+    NO_INCREMENT = 21
+    UNRECOGNIZED_CHARACTERSET_ENCODING = 22
+    GIT_COMMAND_ERROR = 23
+    INVALID_MANUAL_VERSION = 24
+    INIT_FAILED = 25
+    RUN_HOOK_FAILED = 26
+    VERSION_PROVIDER_UNKNOWN = 27
 
 
 class CommitizenException(Exception):
     def __init__(self, *args, **kwargs):
         self.output_method = kwargs.get("output_method") or out.error
         self.exit_code = self.__class__.exit_code
         if args:
@@ -49,16 +58,16 @@
         super().__init__(*args, **kwargs)
 
 
 class DryRunExit(ExpectedExit):
     pass
 
 
-class NoneIncrementExit(ExpectedExit):
-    pass
+class NoneIncrementExit(CommitizenException):
+    exit_code = ExitCode.NO_INCREMENT
 
 
 class NoCommitizenFoundException(CommitizenException):
     exit_code = ExitCode.NO_COMMITIZEN_FOUND
 
 
 class NotAGitProjectError(CommitizenException):
@@ -133,7 +142,39 @@
 class NoCommandFoundError(CommitizenException):
     exit_code = ExitCode.NO_COMMAND_FOUND
     message = "Command is required"
 
 
 class InvalidCommandArgumentError(CommitizenException):
     exit_code = ExitCode.INVALID_COMMAND_ARGUMENT
+
+
+class InvalidConfigurationError(CommitizenException):
+    exit_code = ExitCode.INVALID_CONFIGURATION
+
+
+class NotAllowed(CommitizenException):
+    exit_code = ExitCode.NOT_ALLOWED
+
+
+class CharacterSetDecodeError(CommitizenException):
+    exit_code = ExitCode.UNRECOGNIZED_CHARACTERSET_ENCODING
+
+
+class GitCommandError(CommitizenException):
+    exit_code = ExitCode.GIT_COMMAND_ERROR
+
+
+class InvalidManualVersion(CommitizenException):
+    exit_code = ExitCode.INVALID_MANUAL_VERSION
+
+
+class InitFailedError(CommitizenException):
+    exit_code = ExitCode.INIT_FAILED
+
+
+class RunHookError(CommitizenException):
+    exit_code = ExitCode.RUN_HOOK_FAILED
+
+
+class VersionProviderUnknown(CommitizenException):
+    exit_code = ExitCode.VERSION_PROVIDER_UNKNOWN
```

### Comparing `commitizen-2.9.0/commitizen/factory.py` & `commitizen-3.0.0/commitizen/factory.py`

 * *Files identical despite different names*

### Comparing `commitizen-2.9.0/docs/README.md` & `commitizen-3.0.0/docs/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,174 +1,161 @@
-[![Github Actions](https://github.com/commitizen-tools/commitizen/workflows/Python%20package/badge.svg?style=flat-square)](https://github.com/commitizen-tools/commitizen/actions)
-[![Conventional
-Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow.svg?style=flat-square)](https://conventionalcommits.org)
-[![PyPI Package latest
-release](https://img.shields.io/pypi/v/commitizen.svg?style=flat-square)](https://pypi.org/project/commitizen/)
-[![Supported
-versions](https://img.shields.io/pypi/pyversions/commitizen.svg?style=flat-square)](https://pypi.org/project/commitizen/)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/commitizen-tools/commitizen/pythonpackage.yml?label=python%20package&logo=github&logoColor=white&style=flat-square)](https://github.com/commitizen-tools/commitizen/actions)
+[![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow.svg?style=flat-square)](https://conventionalcommits.org)
+[![PyPI Package latest release](https://img.shields.io/pypi/v/commitizen.svg?style=flat-square)](https://pypi.org/project/commitizen/)
+[![PyPI Package download count (per month)](https://img.shields.io/pypi/dm/commitizen?style=flat-square)](https://pypi.org/project/commitizen/)
+[![Supported versions](https://img.shields.io/pypi/pyversions/commitizen.svg?style=flat-square)](https://pypi.org/project/commitizen/)
 [![homebrew](https://img.shields.io/homebrew/v/commitizen?color=teal&style=flat-square)](https://formulae.brew.sh/formula/commitizen)
 [![Codecov](https://img.shields.io/codecov/c/github/commitizen-tools/commitizen.svg?style=flat-square)](https://codecov.io/gh/commitizen-tools/commitizen)
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?style=flat-square&logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 
 ![Using commitizen cli](images/demo.gif)
 
 ---
 
 **Documentation:** [https://commitizen-tools.github.io/commitizen/](https://commitizen-tools.github.io/commitizen/)
 
 ---
 
 ## About
 
-Commitizen is a tool designed for teams.
+Commitizen is release management tool designed for teams.
 
-Its main purpose is to define a standard way of committing rules
-and communicating it (using the cli provided by commitizen).
+Commitizen assumes your team uses a standard way of commiting rules
+and from that foundation, it can bump your project's version, create
+the changelog, and update files.
 
-The reasoning behind it is that it is easier to read, and enforces writing
-descriptive commits.
+By default, commitizen uses [conventional commits][conventional_commits], but you
+can build your own set of rules, and publish them.
 
-Besides that, having a convention on your commits makes it possible to
-parse them and use them for something else, like generating automatically
-the version or a changelog.
+Using a standarized set of rules to write commits, makes commits easier to read, and enforces writing
+descriptive commits.
 
-### Commitizen features
+### Features
 
 - Command-line utility to create commits with your rules. Defaults: [Conventional commits][conventional_commits]
-- Display information about your commit rules (commands: schema, example, info)
 - Bump version automatically using [semantic versioning][semver] based on the commits. [Read More](./bump.md)
 - Generate a changelog using [Keep a changelog][keepchangelog]
+- Update your project's version files automatically
+- Display information about your commit rules (commands: schema, example, info)
+- Create your own set of rules and publish them to pip. Read more on [Customization](./customization.md)
 
 ## Requirements
 
-Python 3.6+
+[Python](https://www.python.org/downloads/) `3.7+`
+
+[Poetry](https://python-poetry.org/docs/) `1.2.0+`
 
-[Git][gitscm] `1.8.5.2`+
+[Git][gitscm] `1.8.5.2+`
 
 ## Installation
 
-Global installation
+To make commitizen available in your system
 
 ```bash
-sudo pip3 install -U Commitizen
+pip install --user -U Commitizen
 ```
 
 ### Python project
 
 You can add it to your local project using one of these:
 
 ```bash
 pip install -U commitizen
 ```
 
+for Poetry >= 1.2.0:
+
 ```bash
-poetry add commitizen --dev
+poetry add commitizen --group dev
 ```
 
-### macOS
-
-On macOS, it can also be installed via [homebrew](https://formulae.brew.sh/formula/commitizen):
+for Poetry < 1.2.0:
 
 ```bash
-brew install commitizen
+poetry add commitizen --dev
 ```
 
-## Usage
-
-### Committing
+### macOS
 
-Run in your terminal
+via [homebrew](https://formulae.brew.sh/formula/commitizen):
 
 ```bash
-cz commit
+brew install commitizen
 ```
 
-or the shortcut
-
-```bash
-cz c
-```
+## Usage
 
-### Integrating with Pre-commit
-Commitizen can lint your commit message for you with `cz check`.
-You can integrate this in your [pre-commit](https://pre-commit.com/) config with:
+Most of the time this is the only command you'll run:
 
-```yaml
----
-repos:
-  - repo: https://github.com/commitizen-tools/commitizen
-    rev: master
-    hooks:
-      - id: commitizen
-        stages: [commit-msg]
+```sh
+cz bump
 ```
 
-After the configuration is added, you'll need to run
+On top of that, you can use commitizen to assist you with the creation of commits:
 
 ```sh
-pre-commit install --hook-type commit-msg
+cz commit
 ```
 
-Read more about the `check` command [here](https://commitizen-tools.github.io/commitizen/check/).
+Read more in the section [Getting Started](./getting_started.md).
 
 ### Help
 
-```bash
+```sh
 $ cz --help
-usage: cz [-h] [--debug] [-n NAME] [--version]
-          {init,commit,c,ls,example,info,schema,bump,changelog,ch,check,version}
-          ...
+usage: cz [-h] [--debug] [-n NAME] [-nr NO_RAISE] {init,commit,c,ls,example,info,schema,bump,changelog,ch,check,version} ...
 
 Commitizen is a cli tool to generate conventional commits.
 For more information about the topic go to https://conventionalcommits.org/
 
 optional arguments:
   -h, --help            show this help message and exit
   --debug               use debug mode
-  -n NAME, --name NAME  use the given commitizen (default:
-                        cz_conventional_commits)
-  --version             get the version of the installed commitizen
+  -n NAME, --name NAME  use the given commitizen (default: cz_conventional_commits)
+  -nr NO_RAISE, --no-raise NO_RAISE
+                        comma separated error codes that won't rise error, e.g: cz -nr 1,2,3 bump. See codes at https://commitizen-
+                        tools.github.io/commitizen/exit_codes/
 
 commands:
   {init,commit,c,ls,example,info,schema,bump,changelog,ch,check,version}
     init                init commitizen configuration
     commit (c)          create new commit
     ls                  show available commitizens
     example             show commit example
     info                show information about the cz
     schema              show commit schema
     bump                bump semantic version based on the git log
-    changelog (ch)      generate changelog (note that it will overwrite
-                        existing file)
-    check               validates that a commit message matches the commitizen
-                        schema
-    version             get the version of the installed commitizen or the
-                        current project (default: installed commitizen)
+    changelog (ch)      generate changelog (note that it will overwrite existing file)
+    check               validates that a commit message matches the commitizen schema
+    version             get the version of the installed commitizen or the current project (default: installed commitizen)
 ```
 
-## Third-Party Commitizen Templates
+## Setting up bash completion
 
-See [Third-Party Commitizen Templates](third-party-commitizen.md).
+When using bash as your shell (limited support for zsh, fish, and tcsh is available), Commitizen can use [argcomplete](https://kislyuk.github.io/argcomplete/) for auto-completion. For this argcomplete needs to be enabled.
 
-## FAQ
+argcomplete is installed when you install Commitizen since it's a dependency.
 
-### Why are `revert` and `chore` valid types in the check pattern of cz conventional_commits but not types we can select?
+If Commitizen is installed globally, global activation can be executed:
 
-`revert` and `chore` are added to the "pattern" in `cz check` in order to prevent backward errors, but officially they are not part of conventional commits, we are using the latest [types from Angular](https://github.com/angular/angular/blob/22b96b9/CONTRIBUTING.md#type) (they used to but were removed).
-However, you can create a customized `cz` with those extra types. (See [Customization](https://commitizen-tools.github.io/commitizen/customization/)
-
-See more discussion in issue [#142](https://github.com/commitizen-tools/commitizen/issues/142) and [#36](https://github.com/commitizen-tools/commitizen/issues/36)
+```bash
+sudo activate-global-python-argcomplete
+```
 
-### How to handle revert commits?
+For permanent (but not global) Commitizen activation, use:
 
-```sh
-git revert --no-commit <SHA>
-git commit -m "revert: foo bar"
+```bash
+register-python-argcomplete cz >> ~/.bashrc
 ```
 
-## Contributing
+For one-time activation of argcomplete for Commitizen only, use:
+
+```bash
+eval "$(register-python-argcomplete cz)"
+```
 
-See [Contributing](contributing.md)
+For further information on activation, please visit the [argcomplete website](https://kislyuk.github.io/argcomplete/).
 
 [conventional_commits]: https://www.conventionalcommits.org
 [semver]: https://semver.org/
 [keepchangelog]: https://keepachangelog.com/
 [gitscm]: https://git-scm.com/downloads
```

### Comparing `commitizen-2.9.0/setup.py` & `commitizen-3.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,206 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: commitizen
+Version: 3.0.0
+Summary: Python commitizen client tool
+Home-page: https://github.com/commitizen-tools/commitizen
+License: MIT
+Keywords: commitizen,conventional,commits,git
+Author: Santiago Fraire
+Author-email: santiwilly@gmail.com
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Requires-Dist: argcomplete (>=1.12.1,<2.2)
+Requires-Dist: charset-normalizer (>=2.1.0,<4)
+Requires-Dist: colorama (>=0.4.1,<0.5.0)
+Requires-Dist: decli (>=0.5.2,<0.6.0)
+Requires-Dist: importlib_metadata (>=4.13,<5)
+Requires-Dist: jinja2 (>=2.10.3)
+Requires-Dist: packaging (>=19)
+Requires-Dist: pyyaml (>=3.08)
+Requires-Dist: questionary (>=1.4.0,<2.0.0)
+Requires-Dist: termcolor (>=1.1,<3)
+Requires-Dist: tomlkit (>=0.5.3,<1.0.0)
+Requires-Dist: typing-extensions (>=4.0.1,<5.0.0) ; python_version < "3.8"
+Description-Content-Type: text/markdown
+
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/commitizen-tools/commitizen/pythonpackage.yml?label=python%20package&logo=github&logoColor=white&style=flat-square)](https://github.com/commitizen-tools/commitizen/actions)
+[![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow.svg?style=flat-square)](https://conventionalcommits.org)
+[![PyPI Package latest release](https://img.shields.io/pypi/v/commitizen.svg?style=flat-square)](https://pypi.org/project/commitizen/)
+[![PyPI Package download count (per month)](https://img.shields.io/pypi/dm/commitizen?style=flat-square)](https://pypi.org/project/commitizen/)
+[![Supported versions](https://img.shields.io/pypi/pyversions/commitizen.svg?style=flat-square)](https://pypi.org/project/commitizen/)
+[![homebrew](https://img.shields.io/homebrew/v/commitizen?color=teal&style=flat-square)](https://formulae.brew.sh/formula/commitizen)
+[![Codecov](https://img.shields.io/codecov/c/github/commitizen-tools/commitizen.svg?style=flat-square)](https://codecov.io/gh/commitizen-tools/commitizen)
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?style=flat-square&logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
+
+![Using commitizen cli](images/demo.gif)
+
+---
+
+**Documentation:** [https://commitizen-tools.github.io/commitizen/](https://commitizen-tools.github.io/commitizen/)
+
+---
+
+## About
+
+Commitizen is release management tool designed for teams.
+
+Commitizen assumes your team uses a standard way of commiting rules
+and from that foundation, it can bump your project's version, create
+the changelog, and update files.
+
+By default, commitizen uses [conventional commits][conventional_commits], but you
+can build your own set of rules, and publish them.
+
+Using a standarized set of rules to write commits, makes commits easier to read, and enforces writing
+descriptive commits.
+
+### Features
+
+- Command-line utility to create commits with your rules. Defaults: [Conventional commits][conventional_commits]
+- Bump version automatically using [semantic versioning][semver] based on the commits. [Read More](./bump.md)
+- Generate a changelog using [Keep a changelog][keepchangelog]
+- Update your project's version files automatically
+- Display information about your commit rules (commands: schema, example, info)
+- Create your own set of rules and publish them to pip. Read more on [Customization](./customization.md)
+
+## Requirements
+
+[Python](https://www.python.org/downloads/) `3.7+`
+
+[Poetry](https://python-poetry.org/docs/) `1.2.0+`
+
+[Git][gitscm] `1.8.5.2+`
+
+## Installation
+
+To make commitizen available in your system
+
+```bash
+pip install --user -U Commitizen
+```
+
+### Python project
+
+You can add it to your local project using one of these:
+
+```bash
+pip install -U commitizen
+```
+
+for Poetry >= 1.2.0:
+
+```bash
+poetry add commitizen --group dev
+```
+
+for Poetry < 1.2.0:
+
+```bash
+poetry add commitizen --dev
+```
+
+### macOS
+
+via [homebrew](https://formulae.brew.sh/formula/commitizen):
+
+```bash
+brew install commitizen
+```
+
+## Usage
+
+Most of the time this is the only command you'll run:
+
+```sh
+cz bump
+```
+
+On top of that, you can use commitizen to assist you with the creation of commits:
+
+```sh
+cz commit
+```
+
+Read more in the section [Getting Started](./getting_started.md).
+
+### Help
+
+```sh
+$ cz --help
+usage: cz [-h] [--debug] [-n NAME] [-nr NO_RAISE] {init,commit,c,ls,example,info,schema,bump,changelog,ch,check,version} ...
+
+Commitizen is a cli tool to generate conventional commits.
+For more information about the topic go to https://conventionalcommits.org/
+
+optional arguments:
+  -h, --help            show this help message and exit
+  --debug               use debug mode
+  -n NAME, --name NAME  use the given commitizen (default: cz_conventional_commits)
+  -nr NO_RAISE, --no-raise NO_RAISE
+                        comma separated error codes that won't rise error, e.g: cz -nr 1,2,3 bump. See codes at https://commitizen-
+                        tools.github.io/commitizen/exit_codes/
+
+commands:
+  {init,commit,c,ls,example,info,schema,bump,changelog,ch,check,version}
+    init                init commitizen configuration
+    commit (c)          create new commit
+    ls                  show available commitizens
+    example             show commit example
+    info                show information about the cz
+    schema              show commit schema
+    bump                bump semantic version based on the git log
+    changelog (ch)      generate changelog (note that it will overwrite existing file)
+    check               validates that a commit message matches the commitizen schema
+    version             get the version of the installed commitizen or the current project (default: installed commitizen)
+```
+
+## Setting up bash completion
+
+When using bash as your shell (limited support for zsh, fish, and tcsh is available), Commitizen can use [argcomplete](https://kislyuk.github.io/argcomplete/) for auto-completion. For this argcomplete needs to be enabled.
+
+argcomplete is installed when you install Commitizen since it's a dependency.
+
+If Commitizen is installed globally, global activation can be executed:
+
+```bash
+sudo activate-global-python-argcomplete
+```
+
+For permanent (but not global) Commitizen activation, use:
+
+```bash
+register-python-argcomplete cz >> ~/.bashrc
+```
+
+For one-time activation of argcomplete for Commitizen only, use:
+
+```bash
+eval "$(register-python-argcomplete cz)"
+```
+
+For further information on activation, please visit the [argcomplete website](https://kislyuk.github.io/argcomplete/).
+
+[conventional_commits]: https://www.conventionalcommits.org
+[semver]: https://semver.org/
+[keepchangelog]: https://keepachangelog.com/
+[gitscm]: https://git-scm.com/downloads
 
-packages = \
-['commitizen',
- 'commitizen.commands',
- 'commitizen.config',
- 'commitizen.cz',
- 'commitizen.cz.conventional_commits',
- 'commitizen.cz.customize',
- 'commitizen.cz.jira']
-
-package_data = \
-{'': ['*'], 'commitizen': ['templates/*']}
-
-install_requires = \
-['colorama>=0.4.1,<0.5.0',
- 'decli>=0.5.2,<0.6.0',
- 'jinja2>=2.10.3,<3.0.0',
- 'packaging>=19,<21',
- 'pyyaml>=3.08',
- 'questionary>=1.4.0,<2.0.0',
- 'termcolor>=1.1,<2.0',
- 'tomlkit>=0.5.3,<0.6.0']
-
-entry_points = \
-{'console_scripts': ['cz = commitizen.cli:main',
-                     'git-cz = commitizen.cli:main']}
-
-setup_kwargs = {
-    'name': 'commitizen',
-    'version': '2.9.0',
-    'description': 'Python commitizen client tool',
-    'long_description': '[![Github Actions](https://github.com/commitizen-tools/commitizen/workflows/Python%20package/badge.svg?style=flat-square)](https://github.com/commitizen-tools/commitizen/actions)\n[![Conventional\nCommits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow.svg?style=flat-square)](https://conventionalcommits.org)\n[![PyPI Package latest\nrelease](https://img.shields.io/pypi/v/commitizen.svg?style=flat-square)](https://pypi.org/project/commitizen/)\n[![Supported\nversions](https://img.shields.io/pypi/pyversions/commitizen.svg?style=flat-square)](https://pypi.org/project/commitizen/)\n[![homebrew](https://img.shields.io/homebrew/v/commitizen?color=teal&style=flat-square)](https://formulae.brew.sh/formula/commitizen)\n[![Codecov](https://img.shields.io/codecov/c/github/commitizen-tools/commitizen.svg?style=flat-square)](https://codecov.io/gh/commitizen-tools/commitizen)\n\n![Using commitizen cli](images/demo.gif)\n\n---\n\n**Documentation:** [https://commitizen-tools.github.io/commitizen/](https://commitizen-tools.github.io/commitizen/)\n\n---\n\n## About\n\nCommitizen is a tool designed for teams.\n\nIts main purpose is to define a standard way of committing rules\nand communicating it (using the cli provided by commitizen).\n\nThe reasoning behind it is that it is easier to read, and enforces writing\ndescriptive commits.\n\nBesides that, having a convention on your commits makes it possible to\nparse them and use them for something else, like generating automatically\nthe version or a changelog.\n\n### Commitizen features\n\n- Command-line utility to create commits with your rules. Defaults: [Conventional commits][conventional_commits]\n- Display information about your commit rules (commands: schema, example, info)\n- Bump version automatically using [semantic versioning][semver] based on the commits. [Read More](./bump.md)\n- Generate a changelog using [Keep a changelog][keepchangelog]\n\n## Requirements\n\nPython 3.6+\n\n[Git][gitscm] `1.8.5.2`+\n\n## Installation\n\nGlobal installation\n\n```bash\nsudo pip3 install -U Commitizen\n```\n\n### Python project\n\nYou can add it to your local project using one of these:\n\n```bash\npip install -U commitizen\n```\n\n```bash\npoetry add commitizen --dev\n```\n\n### macOS\n\nOn macOS, it can also be installed via [homebrew](https://formulae.brew.sh/formula/commitizen):\n\n```bash\nbrew install commitizen\n```\n\n## Usage\n\n### Committing\n\nRun in your terminal\n\n```bash\ncz commit\n```\n\nor the shortcut\n\n```bash\ncz c\n```\n\n### Integrating with Pre-commit\nCommitizen can lint your commit message for you with `cz check`.\nYou can integrate this in your [pre-commit](https://pre-commit.com/) config with:\n\n```yaml\n---\nrepos:\n  - repo: https://github.com/commitizen-tools/commitizen\n    rev: master\n    hooks:\n      - id: commitizen\n        stages: [commit-msg]\n```\n\nAfter the configuration is added, you\'ll need to run\n\n```sh\npre-commit install --hook-type commit-msg\n```\n\nRead more about the `check` command [here](https://commitizen-tools.github.io/commitizen/check/).\n\n### Help\n\n```bash\n$ cz --help\nusage: cz [-h] [--debug] [-n NAME] [--version]\n          {init,commit,c,ls,example,info,schema,bump,changelog,ch,check,version}\n          ...\n\nCommitizen is a cli tool to generate conventional commits.\nFor more information about the topic go to https://conventionalcommits.org/\n\noptional arguments:\n  -h, --help            show this help message and exit\n  --debug               use debug mode\n  -n NAME, --name NAME  use the given commitizen (default:\n                        cz_conventional_commits)\n  --version             get the version of the installed commitizen\n\ncommands:\n  {init,commit,c,ls,example,info,schema,bump,changelog,ch,check,version}\n    init                init commitizen configuration\n    commit (c)          create new commit\n    ls                  show available commitizens\n    example             show commit example\n    info                show information about the cz\n    schema              show commit schema\n    bump                bump semantic version based on the git log\n    changelog (ch)      generate changelog (note that it will overwrite\n                        existing file)\n    check               validates that a commit message matches the commitizen\n                        schema\n    version             get the version of the installed commitizen or the\n                        current project (default: installed commitizen)\n```\n\n## Third-Party Commitizen Templates\n\nSee [Third-Party Commitizen Templates](third-party-commitizen.md).\n\n## FAQ\n\n### Why are `revert` and `chore` valid types in the check pattern of cz conventional_commits but not types we can select?\n\n`revert` and `chore` are added to the "pattern" in `cz check` in order to prevent backward errors, but officially they are not part of conventional commits, we are using the latest [types from Angular](https://github.com/angular/angular/blob/22b96b9/CONTRIBUTING.md#type) (they used to but were removed).\nHowever, you can create a customized `cz` with those extra types. (See [Customization](https://commitizen-tools.github.io/commitizen/customization/)\n\nSee more discussion in issue [#142](https://github.com/commitizen-tools/commitizen/issues/142) and [#36](https://github.com/commitizen-tools/commitizen/issues/36)\n\n### How to handle revert commits?\n\n```sh\ngit revert --no-commit <SHA>\ngit commit -m "revert: foo bar"\n```\n\n## Contributing\n\nSee [Contributing](contributing.md)\n\n[conventional_commits]: https://www.conventionalcommits.org\n[semver]: https://semver.org/\n[keepchangelog]: https://keepachangelog.com/\n[gitscm]: https://git-scm.com/downloads\n',
-    'author': 'Santiago Fraire',
-    'author_email': 'santiwilly@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/commitizen-tools/commitizen',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.6.1,<4.0.0',
-}
-
-
-setup(**setup_kwargs)
```

