# Comparing `tmp/use_case_registry-1.4.8.tar.gz` & `tmp/use_case_registry-1.4.9.tar.gz`

## Comparing `use_case_registry-1.4.8.tar` & `use_case_registry-1.4.9.tar`

### file list

```diff
@@ -1,54 +1,53 @@
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/.tool-versions
--rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/Makefile
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/mkdocs.yml
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/.github/CODEOWNERS
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/.github/workflows/audit.yml
--rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/.github/workflows/coverage.yml
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/.github/workflows/release.yml
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/.github/workflows/test.yml
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/.github/workflows/update_docs.yml
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/.vscode/settings.json
--rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/docs/index.md
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/docs/general-thoughts/clean-architecture/index.md
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/docs/general-thoughts/error-handling/index.md
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/docs/general-thoughts/one-use-case-one-workflow/index.md
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/requirements/core.txt
--rw-r--r--   0        0        0     4672 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/requirements/dev.txt
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/requirements/sqlalchemy.txt
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/scripts/release_github.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/tests/__init__.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/tests/test_enums.py
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/tests/test_registry.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/tests/assets/templates/target-based/config-1.yml
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/tests/assets/templates/target-based/config-2.yml
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/tests/assets/templates/target-based/config-3.yml
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/tests/assets/templates/target-based/config-4.yml
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/tests/assets/templates/target-based/config-5.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/tests/base/__init__.py
--rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/tests/base/test_command.py
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/tests/base/test_repository.py
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/tests/base/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/tests/parsers/__init__.py
--rw-r--r--   0        0        0     3293 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/tests/parsers/test_target_based.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/use_case_registry/__about__.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/use_case_registry/__init__.py
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/use_case_registry/enums.py
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/use_case_registry/errors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/use_case_registry/py.typed
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/use_case_registry/registry.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/use_case_registry/base/__init__.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/use_case_registry/base/command.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/use_case_registry/base/repository.py
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/use_case_registry/base/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/use_case_registry/internals/__init__.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/use_case_registry/internals/errors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/use_case_registry/pasers/__init__.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/use_case_registry/pasers/macros.py
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/use_case_registry/pasers/target_based.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/.gitignore
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/LICENSE.txt
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/README.md
--rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/pyproject.toml
--rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/PKG-INFO
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/.tool-versions
+-rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/Makefile
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/mkdocs.yml
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/.github/CODEOWNERS
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/.github/workflows/audit.yml
+-rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/.github/workflows/release.yml
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/.github/workflows/test.yml
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/.github/workflows/update_docs.yml
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/.vscode/settings.json
+-rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/docs/index.md
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/docs/general-thoughts/clean-architecture/index.md
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/docs/general-thoughts/error-handling/index.md
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/docs/general-thoughts/one-use-case-one-workflow/index.md
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/requirements/core.txt
+-rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/requirements/dev.txt
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/requirements/sqlalchemy.txt
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/scripts/release_github.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/tests/__init__.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/tests/test_enums.py
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/tests/test_registry.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/tests/assets/templates/target-based/config-1.yml
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/tests/assets/templates/target-based/config-2.yml
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/tests/assets/templates/target-based/config-3.yml
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/tests/assets/templates/target-based/config-4.yml
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/tests/assets/templates/target-based/config-5.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/tests/base/__init__.py
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/tests/base/test_command.py
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/tests/base/test_repository.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/tests/parsers/__init__.py
+-rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/tests/parsers/test_target_based.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/use_case_registry/__about__.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/use_case_registry/__init__.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/use_case_registry/enums.py
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/use_case_registry/errors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/use_case_registry/py.typed
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/use_case_registry/registry.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/use_case_registry/base/__init__.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/use_case_registry/base/command.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/use_case_registry/base/repository.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/use_case_registry/base/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/use_case_registry/internals/__init__.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/use_case_registry/internals/errors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/use_case_registry/pasers/__init__.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/use_case_registry/pasers/macros.py
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/use_case_registry/pasers/target_based.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/.gitignore
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/LICENSE.txt
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/README.md
+-rw-r--r--   0        0        0     3978 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/pyproject.toml
+-rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/PKG-INFO
```

### Comparing `use_case_registry-1.4.8/Makefile` & `use_case_registry-1.4.9/Makefile`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.8/mkdocs.yml` & `use_case_registry-1.4.9/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.8/.github/ISSUE_TEMPLATE/bug_report.md` & `use_case_registry-1.4.9/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.8/.github/ISSUE_TEMPLATE/feature_request.md` & `use_case_registry-1.4.9/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.8/.github/workflows/audit.yml` & `use_case_registry-1.4.9/.github/workflows/audit.yml`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.8/.github/workflows/coverage.yml` & `use_case_registry-1.4.9/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.8/.github/workflows/release.yml` & `use_case_registry-1.4.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.8/.github/workflows/test.yml` & `use_case_registry-1.4.9/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.8/.vscode/settings.json` & `use_case_registry-1.4.9/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.8/docs/index.md` & `use_case_registry-1.4.9/docs/index.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.8/docs/general-thoughts/clean-architecture/index.md` & `use_case_registry-1.4.9/docs/general-thoughts/clean-architecture/index.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.8/docs/general-thoughts/error-handling/index.md` & `use_case_registry-1.4.9/docs/general-thoughts/error-handling/index.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.8/docs/general-thoughts/one-use-case-one-workflow/index.md` & `use_case_registry-1.4.9/docs/general-thoughts/one-use-case-one-workflow/index.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.8/requirements/core.txt` & `use_case_registry-1.4.9/requirements/core.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 #
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
 #    pip-compile --no-emit-trusted-host --output-file=requirements/core.txt --resolver=backtracking pyproject.toml
 #
-attrs==22.2.0
-    # via jsonschema
 jinja2==3.1.2
     # via use_case_registry (pyproject.toml)
-jsonschema==4.17.3
-    # via use_case_registry (pyproject.toml)
 markupsafe==2.1.2
     # via jinja2
 mashumaro[orjson,yaml]==3.6
     # via use_case_registry (pyproject.toml)
 orjson==3.8.10
     # via mashumaro
-pyrsistent==0.19.3
-    # via jsonschema
+pydantic==1.10.7
+    # via use_case_registry (pyproject.toml)
 pyyaml==6.0
     # via mashumaro
 result==0.9.0
     # via use_case_registry (pyproject.toml)
 typing-extensions==4.5.0
     # via
     #   mashumaro
+    #   pydantic
     #   result
```

### Comparing `use_case_registry-1.4.8/requirements/dev.txt` & `use_case_registry-1.4.9/requirements/dev.txt`

 * *Files 3% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
 #    pip-compile --extra=dev --extra=sqlalchemy --no-emit-trusted-host --output-file=requirements/dev.txt --resolver=backtracking pyproject.toml
 #
 anyio==3.6.2
     # via httpcore
-attrs==22.2.0
-    # via jsonschema
 black==23.3.0
     # via use_case_registry (pyproject.toml)
 build==0.10.0
     # via pip-tools
 certifi==2022.12.7
     # via
     #   httpcore
@@ -68,16 +66,14 @@
 jaraco-classes==3.2.3
     # via keyring
 jinja2==3.1.2
     # via
     #   mkdocs
     #   mkdocs-material
     #   use_case_registry (pyproject.toml)
-jsonschema==4.17.3
-    # via use_case_registry (pyproject.toml)
 keyring==23.13.1
     # via hatch
 markdown==3.3.7
     # via
     #   mkdocs
     #   mkdocs-material
     #   pymdown-extensions
@@ -130,26 +126,26 @@
     #   virtualenv
 pluggy==1.0.0
     # via
     #   hatchling
     #   pytest
 ptyprocess==0.7.0
     # via pexpect
+pydantic==1.10.7
+    # via use_case_registry (pyproject.toml)
 pygments==2.15.0
     # via
     #   mkdocs-material
     #   rich
 pymdown-extensions==9.11
     # via mkdocs-material
 pyperclip==1.8.2
     # via hatch
 pyproject-hooks==1.0.0
     # via build
-pyrsistent==0.19.3
-    # via jsonschema
 pytest==7.3.0
     # via
     #   pytest-cov
     #   pytest-env
     #   use_case_registry (pyproject.toml)
 pytest-cov==4.0.0
     # via use_case_registry (pyproject.toml)
@@ -210,14 +206,15 @@
 types-pyyaml==6.0.12.9
     # via use_case_registry (pyproject.toml)
 typing-extensions==4.5.0
     # via
     #   black
     #   mashumaro
     #   mypy
+    #   pydantic
     #   result
     #   sqlalchemy
 urllib3==1.26.15
     # via requests
 userpath==1.8.0
     # via hatch
 virtualenv==20.21.0
```

### Comparing `use_case_registry-1.4.8/requirements/sqlalchemy.txt` & `use_case_registry-1.4.9/requirements/sqlalchemy.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 #
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
 #    pip-compile --extra=sqlalchemy --no-emit-trusted-host --output-file=requirements/sqlalchemy.txt --resolver=backtracking pyproject.toml
 #
-attrs==22.2.0
-    # via jsonschema
 jinja2==3.1.2
     # via use_case_registry (pyproject.toml)
-jsonschema==4.17.3
-    # via use_case_registry (pyproject.toml)
 markupsafe==2.1.2
     # via jinja2
 mashumaro[orjson,yaml]==3.6
     # via use_case_registry (pyproject.toml)
 orjson==3.8.10
     # via mashumaro
-pyrsistent==0.19.3
-    # via jsonschema
+pydantic==1.10.7
+    # via use_case_registry (pyproject.toml)
 pyyaml==6.0
     # via mashumaro
 result==0.9.0
     # via use_case_registry (pyproject.toml)
 sqlalchemy==2.0.9
     # via use_case_registry (pyproject.toml)
 typing-extensions==4.5.0
     # via
     #   mashumaro
+    #   pydantic
     #   result
     #   sqlalchemy
```

### Comparing `use_case_registry-1.4.8/scripts/release_github.py` & `use_case_registry-1.4.9/scripts/release_github.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.8/tests/test_registry.py` & `use_case_registry-1.4.9/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.8/tests/base/test_command.py` & `use_case_registry-1.4.9/tests/base/test_command.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Tests for command."""
 from dataclasses import dataclass
 from typing import Any
 
 import pytest
+from pydantic import BaseModel, Field
 from result import Ok, Result
 
 from use_case_registry import UseCaseRegistry
 from use_case_registry.base.command import BaseCommand, ICommandInput
 from use_case_registry.base.utils import validate_inputs
 from use_case_registry.errors import CommandInputValidationError, UseCaseExecutionError
 
@@ -20,34 +21,18 @@
     """Example command input."""
 
     name: str
     last_name: str
     age: int
 
 
-SCHEMA = {
-    "type": "object",
-    "properties": {
-        "name": {
-            "type": "string",
-            "maxLength": 9,
-        },
-        "last_name": {
-            "type": "string",
-        },
-        "age": {
-            "type": "integer",
-            "minimum": 1,
-        },
-    },
-    "sdsrequired": [
-        "name",
-        "last_name",
-    ],
-}
+class _Schema(BaseModel):
+    name: str = Field(max_length=9)
+    last_name: str
+    age: int = Field(gt=0)
 
 
 class ExampleCommand(BaseCommand):
     """Example command."""
 
     def execute(
         self,
@@ -58,15 +43,15 @@
 
         return Ok()
 
 
 def test_validate_command_pass() -> None:
     """Test validate command passes."""
     inputs = ExampleCommandInput(name="tomas", last_name="perez", age=10)
-    validate_inputs(inputs=inputs.to_dict(), schema=SCHEMA).unwrap()
+    validate_inputs(inputs=inputs.to_dict(), schema=_Schema).unwrap()
 
 
 @pytest.mark.parametrize(
     argnames="inputs",
     argvalues=[
         ExampleCommandInput(
             name="tomas" * 5,
@@ -78,10 +63,10 @@
             last_name="perez",
             age=10,
         ),
     ],
 )
 def test_validate_command_fails(inputs: ICommandInput) -> None:
     """Test validate command fails."""
-    validation_err = validate_inputs(inputs=inputs.to_dict(), schema=SCHEMA).err()
+    validation_err = validate_inputs(inputs=inputs.to_dict(), schema=_Schema).err()
 
     assert isinstance(validation_err, CommandInputValidationError)
```

### Comparing `use_case_registry-1.4.8/tests/base/test_repository.py` & `use_case_registry-1.4.9/tests/base/test_repository.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.8/tests/parsers/test_target_based.py` & `use_case_registry-1.4.9/tests/parsers/test_target_based.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,27 @@
 """Test target-based parser."""
 import os
 import pathlib
 from typing import Any
 from unittest import mock
 
 import pytest
+from pydantic import BaseModel
 
 from use_case_registry.errors import CommandInputValidationError, EnvVarMissingError
 from use_case_registry.pasers.target_based import TargetBasedConfigParser
 
-SCHEMA = {
-    "type": "object",
-    "properties": {
-        "name": {
-            "type": "string",
-        },
-        "last_name": {
-            "type": "string",
-        },
-    },
-    "required": [
-        "name",
-        "last_name",
-    ],
-}
+
+class _Schema(BaseModel):
+    name: str
+    last_name: str
+
+
+class _OtherSchema(BaseModel):
+    other: str
 
 
 class TestTargetBasedConfigParser:  # noqa: D101
     @mock.patch.dict(
         os.environ,
         {
             "EXECUTION_ENV_MOCKED": "mock",
@@ -53,50 +47,38 @@
             ),
         ],
     )
     def test_parse_works(self, template: str, expected_result: dict[str, Any]) -> None:
         """Test parse works as expected."""
         folder = pathlib.Path().cwd().joinpath("tests/assets/templates/target-based/")
         parser = TargetBasedConfigParser(path_to_folder=folder)
-        result = parser.parse(template=template, schema=SCHEMA)
+        result = parser.parse(template=template, schema=_Schema)
         assert result == expected_result
 
     @pytest.mark.parametrize(
         argnames=["template", "schema"],
         argvalues=[
             (
                 "config-2.yml",
-                SCHEMA,
+                _Schema,
             ),
             (
                 "config-5.yml",
-                SCHEMA,
+                _Schema,
             ),
             (
                 "config-1.yml",
-                {
-                    "type": "object",
-                    "properties": {
-                        "other-name": {
-                            "type": "string",
-                        },
-                        "other": {
-                            "type": "string",
-                        },
-                    },
-                    "required": [
-                        "other-name",
-                        "other",
-                    ],
-                },
+                _OtherSchema,
             ),
         ],
     )
     def test_parse_fails_validation(
-        self, template: str, schema: dict[str, Any],
+        self,
+        template: str,
+        schema: type[BaseModel],
     ) -> None:
         """Test parse works as expected."""
         folder = pathlib.Path().cwd().joinpath("tests/assets/templates/target-based/")
         parser = TargetBasedConfigParser(path_to_folder=folder)
         with pytest.raises(CommandInputValidationError):
             parser.parse(template=template, schema=schema)
 
@@ -107,8 +89,8 @@
         ],
     )
     def test_parse_fails_missing_env_var(self, template: str) -> None:
         """Test parse works as expected."""
         folder = pathlib.Path().cwd().joinpath("tests/assets/templates/target-based/")
         parser = TargetBasedConfigParser(path_to_folder=folder)
         with pytest.raises(EnvVarMissingError):
-            parser.parse(template=template, schema=SCHEMA)
+            parser.parse(template=template, schema=_Schema)
```

### Comparing `use_case_registry-1.4.8/use_case_registry/enums.py` & `use_case_registry-1.4.9/use_case_registry/enums.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.8/use_case_registry/errors.py` & `use_case_registry-1.4.9/use_case_registry/errors.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """Custom defined errors."""
 
 import pathlib
-from typing import Any, Union
+from typing import TYPE_CHECKING, Any, Union
 
 from use_case_registry import UseCaseRegistry
 
+if TYPE_CHECKING:
+    from pydantic.error_wrappers import ErrorDict
+
 
 class CommandInputValidationError(Exception):
     """Raised when command input values does pass validation check."""
 
-    def __init__(self, msg: Union[str, list[str]]) -> None:
+    def __init__(self, msg: Union[str, list["ErrorDict"]]) -> None:
         """Construct class."""
         super().__init__(msg)
 
 
 class UseCaseExecutionError(Exception):
     """Raised when there's an error executing a workflow."""
```

### Comparing `use_case_registry-1.4.8/use_case_registry/registry.py` & `use_case_registry-1.4.9/use_case_registry/registry.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.8/use_case_registry/base/command.py` & `use_case_registry-1.4.9/use_case_registry/base/command.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.8/use_case_registry/base/repository.py` & `use_case_registry-1.4.9/use_case_registry/base/repository.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.8/use_case_registry/base/utils.py` & `use_case_registry-1.4.9/use_case_registry/base/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,22 @@
 """Utilities for base process."""
 
 from typing import Any
 
-import jsonschema
-from jsonschema.exceptions import SchemaError, ValidationError
+from pydantic import BaseModel, ValidationError
 from result import Err, Ok, Result
 
 from use_case_registry.errors import CommandInputValidationError
 
 
 def validate_inputs(
-    schema: dict[str, Any],
+    schema: type[BaseModel],
     inputs: dict[str, Any],
 ) -> Result[None, CommandInputValidationError]:
     """Validate inputs."""
-    draft = "$draft"
     try:
-        if draft in schema:
-            schema.pop(draft)
-
-        schema[draft] = "draft-07"
-
-        jsonschema.validate(instance=inputs, schema=schema)
+        schema(**inputs)
 
     except ValidationError as e:
-        return Err(CommandInputValidationError(msg=e.message))
-    except SchemaError as e:
-        return Err(CommandInputValidationError(msg=e.message))
+        return Err(CommandInputValidationError(msg=e.errors()))
 
     return Ok()
```

### Comparing `use_case_registry-1.4.8/use_case_registry/internals/errors.py` & `use_case_registry-1.4.9/use_case_registry/internals/errors.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.8/use_case_registry/pasers/macros.py` & `use_case_registry-1.4.9/use_case_registry/pasers/macros.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.8/use_case_registry/pasers/target_based.py` & `use_case_registry-1.4.9/use_case_registry/pasers/target_based.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Target based configuration parser."""
 import pathlib
 from typing import Any
 
 import jinja2
 import yaml
+from pydantic import BaseModel
 from result import Ok
 from typing_extensions import assert_never
 
 from use_case_registry.base.utils import validate_inputs
 from use_case_registry.errors import CommandInputValidationError
 from use_case_registry.pasers.macros import env_var
 
@@ -18,15 +19,15 @@
     def __init__(
         self,
         path_to_folder: pathlib.Path,
     ) -> None:
         """Target based configuration file parser."""
         self.path_to_folder = path_to_folder
 
-    def parse(self, template: str, schema: dict[str, Any]) -> dict[str, Any]:
+    def parse(self, template: str, schema: type[BaseModel]) -> dict[str, Any]:
         """Parse file and return especific target config."""
         jinja_env = jinja2.Environment(
             loader=jinja2.FileSystemLoader(
                 searchpath=self.path_to_folder,
                 followlinks=False,
                 encoding="utf-8",
             ),
```

### Comparing `use_case_registry-1.4.8/.gitignore` & `use_case_registry-1.4.9/.gitignore`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.8/LICENSE.txt` & `use_case_registry-1.4.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.8/README.md` & `use_case_registry-1.4.9/README.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.8/pyproject.toml` & `use_case_registry-1.4.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 # https://hatch.pypa.io/latest/config/dependency/
 dependencies = [
   "result",
   "Jinja2",
   "mashumaro[orjson,yaml]",
-  "jsonschema"
+  "pydantic"
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 
 sqlalchemy = [
   "SQLAlchemy"
```

### Comparing `use_case_registry-1.4.8/PKG-INFO` & `use_case_registry-1.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: use_case_registry
-Version: 1.4.8
+Version: 1.4.9
 Summary: Registry class for Use Case implementation. They are basically meaningfull lists with some constraints.
 Project-URL: Homepage, https://github.com/Tomperez98/use-case-registry
 Project-URL: Documentation, https://tomperez98.github.io/use-case-registry/
 Project-URL: Issues, https://github.com/Tomperez98/use-case-registry/issues
 Project-URL: Source, https://github.com/Tomperez98/use-case-registry
 Author-email: Tomas Perez Alvarez <tomasperezalvarez@gmail.com>
 License-Expression: MIT
@@ -14,16 +14,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.9
 Requires-Dist: jinja2
-Requires-Dist: jsonschema
 Requires-Dist: mashumaro[orjson,yaml]
+Requires-Dist: pydantic
 Requires-Dist: result
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: hatch; extra == 'dev'
 Requires-Dist: mkdocs-material; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: pip-tools; extra == 'dev'
```

