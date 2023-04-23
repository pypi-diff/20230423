# Comparing `tmp/chatgpt_pre_commit_hooks-0.1.2-py3-none-any.whl.zip` & `tmp/chatgpt_pre_commit_hooks-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,14 @@
-Zip file size: 507237 bytes, number of entries: 15
--rw-r--r--  2.0 unx    80425 b- defN 23-Apr-18 07:15 assets/images/azure-openai-service-key-endpoint.png
--rw-r--r--  2.0 unx   158116 b- defN 23-Apr-18 07:15 assets/images/azure-openai-service-models.png
--rw-r--r--  2.0 unx   161351 b- defN 23-Apr-18 07:15 assets/images/openai-platform-api-key.png
--rw-r--r--  2.0 unx   112924 b- defN 23-Apr-18 07:15 assets/images/openai-platform-org-id.png
--rw-r--r--  2.0 unx       12 b- defN 23-Apr-18 07:15 build/lib/chatgpt_pre_commit_hooks/__init__.py
--rw-r--r--  2.0 unx    11153 b- defN 23-Apr-18 07:15 build/lib/chatgpt_pre_commit_hooks/chatgpt_commit_message.py
--rw-r--r--  2.0 unx       12 b- defN 23-Apr-18 07:15 chatgpt_pre_commit_hooks/__init__.py
--rw-r--r--  2.0 unx    11153 b- defN 23-Apr-18 07:15 chatgpt_pre_commit_hooks/chatgpt_commit_message.py
--rw-r--r--  2.0 unx     4845 b- defN 23-Apr-18 07:15 docs/chatgpt_commit_message.md
--rw-r--r--  2.0 unx     1073 b- defN 23-Apr-18 07:15 chatgpt_pre_commit_hooks-0.1.2.dist-info/LICENSE
--rw-r--r--  2.0 unx    13982 b- defN 23-Apr-18 07:15 chatgpt_pre_commit_hooks-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-18 07:15 chatgpt_pre_commit_hooks-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       96 b- defN 23-Apr-18 07:15 chatgpt_pre_commit_hooks-0.1.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       48 b- defN 23-Apr-18 07:15 chatgpt_pre_commit_hooks-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1501 b- defN 23-Apr-18 07:15 chatgpt_pre_commit_hooks-0.1.2.dist-info/RECORD
-15 files, 556783 bytes uncompressed, 504675 bytes compressed:  9.4%
+Zip file size: 13581 bytes, number of entries: 12
+-rw-r--r--  2.0 unx       21 b- defN 23-Apr-23 06:06 chatgpt_pre_commit_hooks/__init__.py
+-rw-r--r--  2.0 unx     7006 b- defN 23-Apr-23 06:06 chatgpt_pre_commit_hooks/base.py
+-rw-r--r--  2.0 unx     7050 b- defN 23-Apr-23 06:06 chatgpt_pre_commit_hooks/hook_chatgpt_commit_message.py
+-rw-r--r--  2.0 unx      952 b- defN 23-Apr-23 06:06 chatgpt_pre_commit_hooks/logger.py
+-rw-r--r--  2.0 unx     1362 b- defN 23-Apr-23 06:06 chatgpt_pre_commit_hooks/main.py
+-rw-r--r--  2.0 unx      967 b- defN 23-Apr-23 06:06 chatgpt_pre_commit_hooks/utils.py
+-rw-r--r--  2.0 unx     1073 b- defN 23-Apr-23 06:06 chatgpt_pre_commit_hooks-0.1.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx    15915 b- defN 23-Apr-23 06:06 chatgpt_pre_commit_hooks-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-23 06:06 chatgpt_pre_commit_hooks-0.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx      163 b- defN 23-Apr-23 06:06 chatgpt_pre_commit_hooks-0.1.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       25 b- defN 23-Apr-23 06:06 chatgpt_pre_commit_hooks-0.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1145 b- defN 23-Apr-23 06:06 chatgpt_pre_commit_hooks-0.1.3.dist-info/RECORD
+12 files, 35771 bytes uncompressed, 11601 bytes compressed:  67.6%
```

## zipnote {}

```diff
@@ -1,46 +1,37 @@
-Filename: assets/images/azure-openai-service-key-endpoint.png
-Comment: 
-
-Filename: assets/images/azure-openai-service-models.png
-Comment: 
-
-Filename: assets/images/openai-platform-api-key.png
-Comment: 
-
-Filename: assets/images/openai-platform-org-id.png
+Filename: chatgpt_pre_commit_hooks/__init__.py
 Comment: 
 
-Filename: build/lib/chatgpt_pre_commit_hooks/__init__.py
+Filename: chatgpt_pre_commit_hooks/base.py
 Comment: 
 
-Filename: build/lib/chatgpt_pre_commit_hooks/chatgpt_commit_message.py
+Filename: chatgpt_pre_commit_hooks/hook_chatgpt_commit_message.py
 Comment: 
 
-Filename: chatgpt_pre_commit_hooks/__init__.py
+Filename: chatgpt_pre_commit_hooks/logger.py
 Comment: 
 
-Filename: chatgpt_pre_commit_hooks/chatgpt_commit_message.py
+Filename: chatgpt_pre_commit_hooks/main.py
 Comment: 
 
-Filename: docs/chatgpt_commit_message.md
+Filename: chatgpt_pre_commit_hooks/utils.py
 Comment: 
 
-Filename: chatgpt_pre_commit_hooks-0.1.2.dist-info/LICENSE
+Filename: chatgpt_pre_commit_hooks-0.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: chatgpt_pre_commit_hooks-0.1.2.dist-info/METADATA
+Filename: chatgpt_pre_commit_hooks-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: chatgpt_pre_commit_hooks-0.1.2.dist-info/WHEEL
+Filename: chatgpt_pre_commit_hooks-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: chatgpt_pre_commit_hooks-0.1.2.dist-info/entry_points.txt
+Filename: chatgpt_pre_commit_hooks-0.1.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: chatgpt_pre_commit_hooks-0.1.2.dist-info/top_level.txt
+Filename: chatgpt_pre_commit_hooks-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: chatgpt_pre_commit_hooks-0.1.2.dist-info/RECORD
+Filename: chatgpt_pre_commit_hooks-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## chatgpt_pre_commit_hooks/__init__.py

```diff
@@ -1 +1 @@
-"""Init."""
+"""Hooks package."""
```

## Comparing `chatgpt_pre_commit_hooks-0.1.2.dist-info/LICENSE` & `chatgpt_pre_commit_hooks-0.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `chatgpt_pre_commit_hooks-0.1.2.dist-info/METADATA` & `chatgpt_pre_commit_hooks-0.1.3.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt-pre-commit-hooks
-Version: 0.1.2
+Version: 0.1.3
 Summary: Pre-commit hooks collection that utilizes ChatGPT and OpenAI platform to validate modifications made to the codebase.
 Author-email: Dariusz Porowski <3431813+dariuszporowski@users.noreply.github.com>
 License: MIT
 Project-URL: Homepage, https://github.com/DariuszPorowski/chatgpt-pre-commit-hooks/blob/main/README.md
 Project-URL: Bug Tracker, https://github.com/DariuszPorowski/chatgpt-pre-commit-hooks/issues
 Keywords: chatgpt,openai,pre-commit,pre-commit-hooks,pre-commit-hook
 Classifier: Development Status :: 3 - Alpha
@@ -19,44 +19,45 @@
 Classifier: Topic :: Software Development :: Version Control
 Classifier: Topic :: Software Development :: Version Control :: Git
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai (~=0.27.4)
 Requires-Dist: tiktoken (~=0.3.3)
-Requires-Dist: GitPython (~=3.1.31)
 Provides-Extra: build
 Requires-Dist: build ; extra == 'build'
 Requires-Dist: wheel ; extra == 'build'
 Requires-Dist: twine ; extra == 'build'
 Provides-Extra: dev
 Requires-Dist: ruff ; extra == 'dev'
 Requires-Dist: mypy ; extra == 'dev'
 Requires-Dist: pre-commit ; extra == 'dev'
+Requires-Dist: pyyaml ; extra == 'dev'
+Requires-Dist: types-PyYAML ; extra == 'dev'
 
 # 🤖 ChatGPT / OpenAI pre-commit-hooks
 
 [![pre-commit][pre-commit-image]][pre-commit-link]
 [![PyPI - version][pypi-version-image]][pypi-version-link]
 [![PyPI - python version][pypi-pyversions-image]][pypi-pyversions-link]
 [![PyPI - downloads][pypi-stats-image]][pypi-stats-link]
-[![GitHub - ci][github-ci-image]][github-ci-link]
+[![GitHub - CI][github-ci-image]][github-ci-link]
 
 Pre-commit hooks collection that utilizes ChatGPT and OpenAI platform to validate changes made to the codebase.
 
 - [🎣 Hooks](#-hooks)
   - [`chatgpt-commit-message`](#chatgpt-commit-message)
 - [📥 Prerequisites setup](#-prerequisites-setup)
   - [OpenAI Platform](#openai-platform)
   - [Azure OpenAI Service](#azure-openai-service)
   - [Setting environment variables](#setting-environment-variables)
   - [pre-commit setup](#pre-commit-setup)
 - [📦 Hooks setup](#-hooks-setup)
-  - [Remote repo reference (preferred)](#remote-repo-reference-preferred)
-  - [Local repo reference](#local-repo-reference)
+  - [Remote repository reference (preferred)](#remote-repository-reference-preferred)
+  - [Local repository reference](#local-repository-reference)
 - [🛠️ Advanced configuration](#️-advanced-configuration)
   - [Extra environment variables](#extra-environment-variables)
   - [Arguments](#arguments)
   - [`--env-prefix`](#--env-prefix)
   - [Variables precedence](#variables-precedence)
 - [💸 Payments](#-payments)
 - [👥 Contributing](#-contributing)
@@ -64,15 +65,17 @@
 
 ## 🎣 Hooks
 
 ### `chatgpt-commit-message`
 
 Hook that uses OpenAI's ChatGPT API to generate a summary of changes made to a codebase and use it to populate the commit message automatically.
 
-- Read about hook's specific [configuration](https://github.com/DariuszPorowski/chatgpt-pre-commit-hooks/blob/main/docs/chatgpt_commit_message.md).
+- ⚙️ Read about hook's specific [configuration](https://github.com/DariuszPorowski/chatgpt-pre-commit-hooks/blob/main/docs/chatgpt_commit_message.md).
+
+![chatgpt-commit-message](https://raw.githubusercontent.com/dariuszporowski/chatgpt-pre-commit-hooks/main/docs/assets/demos/chatgpt_commit_message.gif)
 
 ## 📥 Prerequisites setup
 
 Hooks support [OpenAI Platform](https://platform.openai.com) and [Azure OpenAI Service](https://azure.microsoft.com/products/cognitive-services/openai-service).
 
 ### OpenAI Platform
 
@@ -93,42 +96,46 @@
     ```shell
     export OPENAI_API_KEY="sk-xxxxxx"
     export OPENAI_ORGANIZATION="org-xxxxxx"
     ```
 
 > 💡 **HINT**
 >
-> How to setup env vars? see: [Setting environment variables](#setting-environment-variables)
+> How to setup environment variables? see: [Setting environment variables](#setting-environment-variables)
 
 ### Azure OpenAI Service
 
-1. Go to [Azure Portal](https://portal.azure.com), and get `API Key`, `Endpoint` and `Model deployment name`
+1. Go to [Azure Portal](https://portal.azure.com), and get `API Key`, `Endpoint`, `Model deployment name`, and `api-version`.
 
     ![Azure OpenAI API Key and Endpoint](https://raw.githubusercontent.com/dariuszporowski/chatgpt-pre-commit-hooks/main/assets/images/azure-openai-service-key-endpoint.png)
 
     ![Azure OpenAI Model](https://raw.githubusercontent.com/dariuszporowski/chatgpt-pre-commit-hooks/main/assets/images/azure-openai-service-models.png)
 
+    The latest supported `api-version` you can get from [Azure OpenAI Service](https://learn.microsoft.com/en-us/azure/cognitive-services/openai/reference#chat-completions)
+
 1. Store values as an environment variables:
     - `OPENAI_API_TYPE` put `azure` to specified OpenAI provider
     - `OPENAI_API_KEY` for API Key
     - `OPENAI_API_BASE` for Endpoint
-    - `OPENAI_MODEL_NAME` for Model deployment name
+    - `OPENAI_API_VERSION` for `api-version`
+    - `OPENAI_MODEL` for Model deployment name
 
     Example:
 
     ```shell
     export OPENAI_API_TYPE="azure"
-    export OPENAI_API_KEY="sk-xxxxxx"
+    export OPENAI_API_KEY="xxxxxx"
     export OPENAI_API_BASE="https://xxxxxx.openai.azure.com/"
-    export OPENAI_MODEL_NAME="xxxxx-gpt-35-turbo"
+    export OPENAI_API_VERSION="2023-03-15-preview"
+    export OPENAI_MODEL="xxxxx-gpt-35-turbo"
     ```
 
 > 💡 **HINT**
 >
-> How to setup env vars? see: [Setting environment variables](#setting-environment-variables)
+> How to setup environment variables? see: [Setting environment variables](#setting-environment-variables)
 
 ### Setting environment variables
 
 Linux/MacOS example:
 
 ```shell
 export OPENAI_API_KEY="sk-xxxxxx"
@@ -156,73 +163,94 @@
 
 ```shell
 # install using pip
 pip install pre-commit
 
 # check if working - expected print with version like `pre-commit 3.2.2`
 pre-commit --version
+```
 
+Add to your `.pre-commit-config.yaml` top level `default_install_hook_types` section (for more information, follow [Confining hooks to run at certain stages](https://pre-commit.com/#confining-hooks-to-run-at-certain-stages))
+
+```yaml
+default_install_hook_types:
+  - pre-commit # this is default hook type, equivalent to classic `pre-commit install` command
+  - prepare-commit-msg # this type is not enabled by default, please enable it - equivalent to `pre-commit install --hook-type prepare-commit-msg` command
+  - ... # rest of hook types what are you using, if any
+```
+
+next:
+
+```shell
 # setup the git repo for hooks
 pre-commit install
 
-# periodically run updates to your pre-commit config to make sure you always have the latest version of the hooks
+# (optional) periodically run updates to your pre-commit config to make sure you always have the latest version of the hooks
 pre-commit autoupdate
 ```
 
 ## 📦 Hooks setup
 
-### Remote repo reference (preferred)
+### Remote repository reference (preferred)
 
 Add to your `.pre-commit-config.yaml`
 
 ```yaml
+default_install_hook_types:
+  - pre-commit
+  - prepare-commit-msg
 repos:
   - repo: https://github.com/DariuszPorowski/chatgpt-pre-commit-hooks
     rev: vX.Y.Z  # Use the ref you want to point at, see ⚠️ NOTE below!
     hooks:
-      - id: ... # follow 🎣 Hooks section to see available hooks IDs
+      - id: <id1> # follow 🎣 Hooks section to see available hooks IDs
+      - id: <id2> # follow 🎣 Hooks section to see available hooks IDs
+      - id: ...
 ```
 
 Example:
 
 ```yaml
+default_install_hook_types:
+  - pre-commit
+  - prepare-commit-msg
 repos:
   - repo: https://github.com/DariuszPorowski/chatgpt-pre-commit-hooks
-    rev: v0.1.2
+    rev: v0.1.3
     hooks:
       - id: chatgpt-commit-message
 ```
 
 > ⚠️ **NOTE**
 >
 > For the `rev:` always try to use the latest version. You can check the latest release under [GitHub Releases](https://github.com/DariuszPorowski/chatgpt-pre-commit-hooks/releases/latest)
 
-### Local repo reference
+### Local repository reference
 
 1. Install or add [PyPI](https://pypi.org/project/chatgpt-pre-commit-hooks) package to your project.
 
    - if you are using [pip](https://pip.pypa.io):
 
      ```shell
      pip install --upgrade chatgpt-pre-commit-hooks
      ```
 
    - or include it in a `requirements.txt` file in your project:
 
      ```text
-     chatgpt-pre-commit-hooks~=0.1.2
+     chatgpt-pre-commit-hooks~=0.1.3
      ```
 
       and run:
 
      ```shell
      pip install -r requirements.txt
      ```
 
-   - or, even better, in the dev section of your `pyproject.toml` file:
+   - or, even better, in the `dev` section of your `pyproject.toml` file:
 
      ```toml
      [project.optional-dependencies]
      dev = ["chatgpt-pre-commit-hooks"]
      ```
 
       and run:
@@ -236,33 +264,48 @@
      ```shell
      poetry add chatgpt-pre-commit-hooks --group dev
      ```
 
 1. Add to your `.pre-commit-config.yaml`
 
     ```yaml
+    default_install_hook_types:
+      - pre-commit
+      - prepare-commit-msg
     repos:
       - repo: local
         hooks:
           - id: <id> # follow 🎣 Hooks section to see available hooks IDs
-            name: Run <name>
-            entry: <id> # follow 🎣 Hooks section to see available hooks IDs
+            name: <name> # any name you'd like to set
+            entry: chatgpt-pre-commit-hooks
+            args:
+              - "--hook"
+              - "<id>" # follow 🎣 Hooks section to see available hooks IDs
+              - "..." # rest of args what you'd like to set (optional)
             language: system
     ```
 
     Example:
 
     ```yaml
+    default_install_hook_types:
+      - pre-commit
+      - prepare-commit-msg
     repos:
     - repo: local
         hooks:
-      - id: chatgpt-commit-message
-            name: Run ChatGPT commit-message
-            entry: chatgpt-commit-message
-            language: system
+        - id: chatgpt-commit-message
+          name: ChatGPT commit message
+          entry: chatgpt-pre-commit-hooks
+          args:
+            - "--hook"
+            - "chatgpt-commit-message"
+            - "--description"
+            - "--emoji"
+          language: system
     ```
 
 ## 🛠️ Advanced configuration
 
 ### Extra environment variables
 
 In addition to the environment variables listed in the [📥 Prerequisites setup](#-prerequisites-setup) section, you can set several configurations using extra environment variables.
@@ -271,28 +314,31 @@
 |:--------------------|:------:|:---------------:|:---------------------------------------------------------------------------------------------------------------------------------------------|
 | `OPENAI_MAX_TOKENS` |  int   |      1024       | [What are tokens and how to count them?](https://help.openai.com/en/articles/4936856-what-are-tokens-and-how-to-count-them)                  |
 | `OPENAI_MODEL`      | string | `gpt-3.5-turbo` | [Model endpoint compatibility](https://platform.openai.com/docs/models/model-endpoint-compatibility) - check `/v1/chat/completions` endpoint |
 | `OPENAI_PROXY`      | string |    _not set_    | http/https client proxy                                                                                                                      |
 
 ### Arguments
 
-Any environment variable can be overridden by hard-coded args in `pre-commit-config.yaml`, except `OPENAI_API_KEY`, `OPENAI_ORGANIZATION`.
+Any environment variable can be overridden by hard-coded arguments in `pre-commit-config.yaml`, except `OPENAI_API_KEY`, `OPENAI_ORGANIZATION`.
 
 | Name                  |  Type  |  Default  | Description                                                                                                       |
 |:----------------------|:------:|:---------:|:------------------------------------------------------------------------------------------------------------------|
 | `--env-prefix`        | string | _not set_ | Set prefix for environment variables allowing multiple configurations. Read more: [`--env-prefix`](#--env-prefix) |
 | `--openai-max-tokens` |  int   | _not set_ | Overrides `OPENAI_MAX_TOKENS`                                                                                     |
 | `--openai-proxy`      | string | _not set_ | Overrides `OPENAI_PROXY`                                                                                          |
 | `--openai-model`      | string | _not set_ | Overrides `OPENAI_MODEL`                                                                                          |
 | `--openai-api-base`   | string | _not set_ | Overrides `OPENAI_API_BASE`                                                                                       |
 | `--openai-api-type`   | string | _not set_ | Overrides `OPENAI_API_TYPE`                                                                                       |
 
 Example:
 
 ```yaml
+default_install_hook_types:
+  - pre-commit
+  - prepare-commit-msg
 repos:
   - repo: https://github.com/DariuszPorowski/chatgpt-pre-commit-hooks
     rev: vX.Y.Z
     hooks:
       - id: ... # follow 🎣 Hooks section to see available hooks IDs
         args:
           - "--env-prefix"
@@ -300,38 +346,38 @@
           - "--openai-max-tokens"
           - "512"
           - ...
 ```
 
 ### `--env-prefix`
 
-It's a special arg where you can mark prefixes for your environment variables. This allows you to set many configurations depending on the project, account, profile, etc., for example, `personal`, `work`. Fallback is a global environment variable if prefixed is not found.
+It's a special argument where you can mark prefixes for your environment variables. This allows you to set many configurations depending on the project, account, profile, etc., for example, `personal`, `work`. Fallback is a global environment variable if prefixed isn't found.
 
 For instance, if your prefix is `personal`, then the environment variable must be set `PERSONAL__OPENAI_MAX_TOKENS`, meaning the structure is `<prefix>__<base_env_name>` - two underscores `__` between `prefix` and `base_env_name`.
 
 Example:
 
 ```shell
 export PERSONAL__OPENAI_API_KEY="sk-xxxxxx"
 export WORK__OPENAI_API_KEY="sk-xxxxxx"
 ```
 
 ### Variables precedence
 
-1. hard-coded args, e.g. `--openai-max-tokens`
-1. prefixed environment variable, e.g. `PERSONAL__OPENAI_MAX_TOKENS`
-1. global environment variable, e.g. `OPENAI_MAX_TOKENS`
+1. hard-coded arguments, for example `--openai-max-tokens`
+1. prefixed environment variable, for example `PERSONAL__OPENAI_MAX_TOKENS`
+1. global environment variable, for example `OPENAI_MAX_TOKENS`
 
 ## 💸 Payments
 
 Project by default uses `gpt-3.5-turbo` model because of [its lower cost](https://openai.com/pricing). You have to pay for your own OpenAI API requests.
 
 ## 👥 Contributing
 
-Contributions to the project are very welcome! Please follow [Contributing Guide](https://github.com/DariuszPorowski/chatgpt-pre-commit-hooks/blob/main/CONTRIBUTING.md).
+Contributions to the project are welcome! Please follow [Contributing Guide](https://github.com/DariuszPorowski/chatgpt-pre-commit-hooks/blob/main/CONTRIBUTING.md).
 
 ## 📄 License
 
 This project is distributed under the terms of the [MIT](https://opensource.org/licenses/MIT) license.
 
 [github-ci-image]: https://img.shields.io/github/actions/workflow/status/DariuszPorowski/chatgpt-pre-commit-hooks/workflow.ci.yml?style=flat-square&branch=main&event=push
 [github-ci-link]: https://github.com/DariuszPorowski/chatgpt-pre-commit-hooks/actions/workflows/workflow.ci.yml?query=branch%3Amain+event%3Apush
```

