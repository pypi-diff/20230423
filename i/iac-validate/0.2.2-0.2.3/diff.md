# Comparing `tmp/iac_validate-0.2.2.tar.gz` & `tmp/iac_validate-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iac_validate-0.2.2.tar", max compression
+gzip compressed data, was "iac_validate-0.2.3.tar", max compression
```

## Comparing `iac_validate-0.2.2.tar` & `iac_validate-0.2.3.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0    16295 2023-01-05 10:35:59.843550 iac_validate-0.2.2/LICENSE
--rw-r--r--   0        0        0     4063 2023-01-05 10:35:59.843550 iac_validate-0.2.2/README.md
--rw-r--r--   0        0        0      394 2023-01-05 10:35:59.843550 iac_validate-0.2.2/iac_validate/__init__.py
--rw-r--r--   0        0        0      175 2023-01-05 10:35:59.843550 iac_validate-0.2.2/iac_validate/__main__.py
--rw-r--r--   0        0        0      218 2023-01-05 10:35:59.843550 iac_validate-0.2.2/iac_validate/ansible_vault.py
--rw-r--r--   0        0        0        0 2023-01-05 10:35:59.843550 iac_validate-0.2.2/iac_validate/cli/__init__.py
--rw-r--r--   0        0        0     1912 2023-01-05 10:35:59.843550 iac_validate-0.2.2/iac_validate/cli/main.py
--rw-r--r--   0        0        0     1199 2023-01-05 10:35:59.843550 iac_validate-0.2.2/iac_validate/cli/options.py
--rw-r--r--   0        0        0     4782 2023-01-05 10:35:59.843550 iac_validate-0.2.2/iac_validate/validator.py
--rw-r--r--   0        0        0     4809 2023-01-05 10:35:59.843550 iac_validate-0.2.2/iac_validate/yaml.py
--rw-r--r--   0        0        0     1937 2023-01-05 10:35:59.843550 iac_validate-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     5253 1970-01-01 00:00:00.000000 iac_validate-0.2.2/setup.py
--rw-r--r--   0        0        0     5181 1970-01-01 00:00:00.000000 iac_validate-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    16295 2023-04-23 20:16:45.572899 iac_validate-0.2.3/LICENSE
+-rw-r--r--   0        0        0     4063 2023-04-23 20:16:45.572899 iac_validate-0.2.3/README.md
+-rw-r--r--   0        0        0      394 2023-04-23 20:16:45.572899 iac_validate-0.2.3/iac_validate/__init__.py
+-rw-r--r--   0        0        0      175 2023-04-23 20:16:45.572899 iac_validate-0.2.3/iac_validate/__main__.py
+-rw-r--r--   0        0        0      218 2023-04-23 20:16:45.572899 iac_validate-0.2.3/iac_validate/ansible_vault.py
+-rw-r--r--   0        0        0        0 2023-04-23 20:16:45.572899 iac_validate-0.2.3/iac_validate/cli/__init__.py
+-rw-r--r--   0        0        0     1912 2023-04-23 20:16:45.572899 iac_validate-0.2.3/iac_validate/cli/main.py
+-rw-r--r--   0        0        0     1199 2023-04-23 20:16:45.576900 iac_validate-0.2.3/iac_validate/cli/options.py
+-rw-r--r--   0        0        0     5092 2023-04-23 20:16:45.576900 iac_validate-0.2.3/iac_validate/validator.py
+-rw-r--r--   0        0        0     4947 2023-04-23 20:16:45.576900 iac_validate-0.2.3/iac_validate/yaml.py
+-rw-r--r--   0        0        0     1937 2023-04-23 20:16:45.576900 iac_validate-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     5181 1970-01-01 00:00:00.000000 iac_validate-0.2.3/PKG-INFO
```

### Comparing `iac_validate-0.2.2/LICENSE` & `iac_validate-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `iac_validate-0.2.2/README.md` & `iac_validate-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `iac_validate-0.2.2/iac_validate/cli/main.py` & `iac_validate-0.2.3/iac_validate/cli/main.py`

 * *Files identical despite different names*

### Comparing `iac_validate-0.2.2/iac_validate/cli/options.py` & `iac_validate-0.2.3/iac_validate/cli/options.py`

 * *Files identical despite different names*

### Comparing `iac_validate-0.2.2/iac_validate/validator.py` & `iac_validate-0.2.3/iac_validate/validator.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,24 +27,27 @@
             self.schema = yamale.make_schema(schema_path, parser="ruamel")
         self.errors: List[str] = []
         self.rules = {}
         if os.path.exists(rules_path):
             logger.info("Loading rules")
             for filename in os.listdir(rules_path):
                 if filename.endswith(".py"):
-                    file_path = os.path.join(rules_path, filename)
-                    spec = importlib.util.spec_from_file_location(
-                        "iac_validate.rules", file_path
-                    )
-                    if spec is not None:
-                        mod = importlib.util.module_from_spec(spec)
-                        sys.modules["iac_validate.rules"] = mod
-                        if spec.loader is not None:
-                            spec.loader.exec_module(mod)
-                            self.rules[mod.Rule.id] = mod.Rule
+                    try:
+                        file_path = os.path.join(rules_path, filename)
+                        spec = importlib.util.spec_from_file_location(
+                            "iac_validate.rules", file_path
+                        )
+                        if spec is not None:
+                            mod = importlib.util.module_from_spec(spec)
+                            sys.modules["iac_validate.rules"] = mod
+                            if spec.loader is not None:
+                                spec.loader.exec_module(mod)
+                                self.rules[mod.Rule.id] = mod.Rule
+                    except:  # noqa: E722
+                        logger.error("Failed loading rule: {}".format(filename))
 
     def _validate_syntax_file(self, file_path: str, strict: bool = True) -> None:
         """Run syntactic validation for a single file"""
         filename = os.path.basename(file_path)
         if os.path.isfile(file_path) and (".yaml" in filename or ".yml" in filename):
             logger.info("Validate file: %s", filename)
 
@@ -119,11 +122,14 @@
                 logger.error(msg)
                 self.errors.append(msg)
         return error
 
     def write_output(self, input_paths: List[str], path: str) -> None:
         if self.data is None:
             self.data = load_yaml_files(input_paths)
-        with open(path, "w") as fh:
-            y = yaml.YAML()
-            y.default_flow_style = False
-            y.dump(self.data, fh)
+        try:
+            with open(path, "w") as fh:
+                y = yaml.YAML()
+                y.default_flow_style = False
+                y.dump(self.data, fh)
+        except:  # noqa: E722
+            logger.error("Cannot write file: {}".format(path))
```

### Comparing `iac_validate-0.2.2/iac_validate/yaml.py` & `iac_validate-0.2.3/iac_validate/yaml.py`

 * *Files 3% similar despite different names*

```diff
@@ -129,19 +129,24 @@
     destination.append(source_item)
 
 
 def merge_dict(
     source: Dict[Any, Any], destination: Dict[Any, Any], merge_list_items: bool = True
 ) -> Dict[Any, Any]:
     """Merge two nested dict/list structures."""
+    if not source:
+        return destination
     for key, value in source.items():
         if isinstance(value, dict):
             # get node or create one
             node = destination.setdefault(key, {})
-            merge_dict(value, node, merge_list_items)
+            if node is None:
+                destination[key] = value
+            else:
+                merge_dict(value, node, merge_list_items)
         elif isinstance(value, list):
             if key not in destination:
                 destination[key] = value
             if isinstance(destination[key], list):
                 for i in value:
                     merge_list_item(i, destination[key], merge_list_items)
         else:
```

### Comparing `iac_validate-0.2.2/pyproject.toml` & `iac_validate-0.2.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 documentation = "https://github.com/netascode/iac-validate"
 homepage = "https://github.com/netascode/iac-validate"
 license = "LICENSE"
 maintainers = ["Daniel Schmidt <danischm@cisco.com>"]
 name = "iac-validate"
 readme = "README.md"
 repository = "https://github.com/netascode/iac-validate"
-version = "0.2.2"
+version = "0.2.3"
 
 [tool.poetry.scripts]
 iac-validate = "iac_validate.cli.main:main"
 
 [tool.poetry.dependencies]
 click = "^8.0.4"
 errorhandler = "^2.0.1"
```

### Comparing `iac_validate-0.2.2/setup.py` & `iac_validate-0.2.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,134 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: iac-validate
+Version: 0.2.3
+Summary: A CLI tool to perform syntactic and semantic validation of YAML files.
+Home-page: https://github.com/netascode/iac-validate
+License: LICENSE
+Author: Daniel Schmidt
+Author-email: danischm@cisco.com
+Maintainer: Daniel Schmidt
+Maintainer-email: danischm@cisco.com
+Requires-Python: >=3.7,<4.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: click (>=8.0.4,<9.0.0)
+Requires-Dist: errorhandler (>=2.0.1,<3.0.0)
+Requires-Dist: importlib-metadata (>=2.0.0,<3.0.0) ; python_version < "3.8"
+Requires-Dist: ruamel-yaml (>0.16.10)
+Requires-Dist: yamale (>=4.0.3,<5.0.0)
+Project-URL: Documentation, https://github.com/netascode/iac-validate
+Project-URL: Repository, https://github.com/netascode/iac-validate
+Description-Content-Type: text/markdown
+
+[![Tests](https://github.com/netascode/iac-validate/actions/workflows/test.yml/badge.svg)](https://github.com/netascode/iac-validate/actions/workflows/test.yml)
+![Python Support](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-informational "Python Support: 3.7, 3.8, 3.9, 3.10, 3.11")
+
+# iac-validate
+
+A CLI tool to perform syntactic and semantic validation of YAML files.
+
+```
+$ iac-validate -h
+Usage: iac-validate [OPTIONS] [PATHS]...
+
+  A CLI tool to perform syntactic and semantic validation of YAML files.
+
+Options:
+  --version              Show the version and exit.
+  -v, --verbosity LVL    Either CRITICAL, ERROR, WARNING, INFO or DEBUG
+  -s, --schema FILE      Path to schema file. (optional, default:
+                         '.schema.yaml', env: IAC_VALIDATE_SCHEMA)
+  -r, --rules DIRECTORY  Path to semantic rules. (optional, default:
+                         '.rules/', env: IAC_VALIDATE_RULES)
+  -o, --output FILE      Write merged content from YAML files to a new YAML
+                         file. (optional, env: IAC_VALIDATE_OUTPUT)
+  --non-strict           Accept unexpected elements in YAML files.
+  -h, --help             Show this message and exit.
+```
+
+Syntactic validation is done by basic YAML syntax validation (e.g., indentation) and by providing a [Yamale](https://github.com/23andMe/Yamale) schema and validating all YAML files against that schema. Semantic validation is done by providing a set of rules (implemented in Python) which are then validated against the YAML data. Every rule is implemented as a Python class and should be placed in a `.py` file located in the `--rules` path.
+
+Each `.py` file must have a single class named `Rule`. This class must have the following attributes: `id`, `description` and `severity`. It must implement a `classmethod()` named `match` that has a single function argument `data` which is the data read from all YAML files. It should return a list of strings, one for each rule violation with a descriptive message. A sample rule can be found below.
+
+```python
+class Rule:
+    id = "101"
+    description = "Verify child naming restrictions"
+    severity = "HIGH"
+
+    @classmethod
+    def match(cls, data):
+        results = []
+        try:
+            for child in data["root"]["children"]:
+                if child["name"] == "FORBIDDEN":
+                    results.append("root.children.name" + " - " + str(child["name"]))
+        except KeyError:
+            pass
+        return results
+```
+
+## Installation
+
+Python 3.7+ is required to install `iac-validate`. Don't have Python 3.7 or later? See [Python 3 Installation & Setup Guide](https://realpython.com/installing-python/).
+
+`iac-validate` can be installed in a virtual environment using `pip`:
+
+```
+pip install iac-validate
+```
+
+## Pre-Commit Hook
+
+The tool can be integrated via a [pre-commit](https://pre-commit.com/) hook with the following config (`.pre-commit-config.yaml`), assuming the default values (`.schema.yaml`, `.rules/`) are appropriate:
+
+```
+repos:
+  - repo: https://github.com/netascode/iac-validate
+    rev: v0.1.6
+    hooks:
+      - id: iac-validate
+```
+
+In case the schema or validation rules are located somewhere else the required CLI arguments can be added like this:
+
+```
+repos:
+  - repo: https://github.com/netascode/iac-validate
+    rev: v0.1.6
+    hooks:
+      - id: iac-validate
+        args:
+          - '-s'
+          - 'my_schema.yaml'
+          - '-r'
+          - 'rules/'
+```
+
+## Ansible Vault Support
+
+Values can be encrypted using [Ansible Vault](https://docs.ansible.com/ansible/latest/user_guide/vault.html). This requires Ansible (`ansible-vault` command) to be installed and the following two environment variables to be defined:
+
+```
+export ANSIBLE_VAULT_ID=dev
+export ANSIBLE_VAULT_PASSWORD=Password123
+```
+
+`ANSIBLE_VAULT_ID` is optional, and if not defined will be omitted.
+
+## Additional Tags
+
+### Reading Environment Variables
+
+The `!env` YAML tag can be used to read values from environment variables.
+
+```yaml
+root:
+  name: !env VAR_NAME
+```
 
-packages = \
-['iac_validate', 'iac_validate.cli']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['click>=8.0.4,<9.0.0',
- 'errorhandler>=2.0.1,<3.0.0',
- 'ruamel-yaml>0.16.10',
- 'yamale>=4.0.3,<5.0.0']
-
-extras_require = \
-{':python_version < "3.8"': ['importlib-metadata>=2.0.0,<3.0.0']}
-
-entry_points = \
-{'console_scripts': ['iac-validate = iac_validate.cli.main:main']}
-
-setup_kwargs = {
-    'name': 'iac-validate',
-    'version': '0.2.2',
-    'description': 'A CLI tool to perform syntactic and semantic validation of YAML files.',
-    'long_description': '[![Tests](https://github.com/netascode/iac-validate/actions/workflows/test.yml/badge.svg)](https://github.com/netascode/iac-validate/actions/workflows/test.yml)\n![Python Support](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-informational "Python Support: 3.7, 3.8, 3.9, 3.10, 3.11")\n\n# iac-validate\n\nA CLI tool to perform syntactic and semantic validation of YAML files.\n\n```\n$ iac-validate -h\nUsage: iac-validate [OPTIONS] [PATHS]...\n\n  A CLI tool to perform syntactic and semantic validation of YAML files.\n\nOptions:\n  --version              Show the version and exit.\n  -v, --verbosity LVL    Either CRITICAL, ERROR, WARNING, INFO or DEBUG\n  -s, --schema FILE      Path to schema file. (optional, default:\n                         \'.schema.yaml\', env: IAC_VALIDATE_SCHEMA)\n  -r, --rules DIRECTORY  Path to semantic rules. (optional, default:\n                         \'.rules/\', env: IAC_VALIDATE_RULES)\n  -o, --output FILE      Write merged content from YAML files to a new YAML\n                         file. (optional, env: IAC_VALIDATE_OUTPUT)\n  --non-strict           Accept unexpected elements in YAML files.\n  -h, --help             Show this message and exit.\n```\n\nSyntactic validation is done by basic YAML syntax validation (e.g., indentation) and by providing a [Yamale](https://github.com/23andMe/Yamale) schema and validating all YAML files against that schema. Semantic validation is done by providing a set of rules (implemented in Python) which are then validated against the YAML data. Every rule is implemented as a Python class and should be placed in a `.py` file located in the `--rules` path.\n\nEach `.py` file must have a single class named `Rule`. This class must have the following attributes: `id`, `description` and `severity`. It must implement a `classmethod()` named `match` that has a single function argument `data` which is the data read from all YAML files. It should return a list of strings, one for each rule violation with a descriptive message. A sample rule can be found below.\n\n```python\nclass Rule:\n    id = "101"\n    description = "Verify child naming restrictions"\n    severity = "HIGH"\n\n    @classmethod\n    def match(cls, data):\n        results = []\n        try:\n            for child in data["root"]["children"]:\n                if child["name"] == "FORBIDDEN":\n                    results.append("root.children.name" + " - " + str(child["name"]))\n        except KeyError:\n            pass\n        return results\n```\n\n## Installation\n\nPython 3.7+ is required to install `iac-validate`. Don\'t have Python 3.7 or later? See [Python 3 Installation & Setup Guide](https://realpython.com/installing-python/).\n\n`iac-validate` can be installed in a virtual environment using `pip`:\n\n```\npip install iac-validate\n```\n\n## Pre-Commit Hook\n\nThe tool can be integrated via a [pre-commit](https://pre-commit.com/) hook with the following config (`.pre-commit-config.yaml`), assuming the default values (`.schema.yaml`, `.rules/`) are appropriate:\n\n```\nrepos:\n  - repo: https://github.com/netascode/iac-validate\n    rev: v0.1.6\n    hooks:\n      - id: iac-validate\n```\n\nIn case the schema or validation rules are located somewhere else the required CLI arguments can be added like this:\n\n```\nrepos:\n  - repo: https://github.com/netascode/iac-validate\n    rev: v0.1.6\n    hooks:\n      - id: iac-validate\n        args:\n          - \'-s\'\n          - \'my_schema.yaml\'\n          - \'-r\'\n          - \'rules/\'\n```\n\n## Ansible Vault Support\n\nValues can be encrypted using [Ansible Vault](https://docs.ansible.com/ansible/latest/user_guide/vault.html). This requires Ansible (`ansible-vault` command) to be installed and the following two environment variables to be defined:\n\n```\nexport ANSIBLE_VAULT_ID=dev\nexport ANSIBLE_VAULT_PASSWORD=Password123\n```\n\n`ANSIBLE_VAULT_ID` is optional, and if not defined will be omitted.\n\n## Additional Tags\n\n### Reading Environment Variables\n\nThe `!env` YAML tag can be used to read values from environment variables.\n\n```yaml\nroot:\n  name: !env VAR_NAME\n```\n',
-    'author': 'Daniel Schmidt',
-    'author_email': 'danischm@cisco.com',
-    'maintainer': 'Daniel Schmidt',
-    'maintainer_email': 'danischm@cisco.com',
-    'url': 'https://github.com/netascode/iac-validate',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

