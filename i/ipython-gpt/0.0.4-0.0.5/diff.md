# Comparing `tmp/ipython-gpt-0.0.4.tar.gz` & `tmp/ipython_gpt-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipython-gpt-0.0.4.tar", last modified: Sat Apr 15 14:29:09 2023, max compression
+gzip compressed data, was "ipython_gpt-0.0.5.tar", max compression
```

## Comparing `ipython-gpt-0.0.4.tar` & `ipython_gpt-0.0.5.tar`

### file list

```diff
@@ -1,5 +1,8 @@
--rw-r--r--   0        0        0     3922 2023-04-15 14:28:41.986114 ipython-gpt-0.0.4/README.md
--rw-r--r--   0        0        0     5354 2023-04-15 14:22:53.034120 ipython-gpt-0.0.4/ipython_gpt.py
--rw-r--r--   0        0        0      756 2023-04-15 14:28:24.646013 ipython-gpt-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     4703 2023-04-15 14:29:09.825156 ipython-gpt-0.0.4/setup.py
--rw-r--r--   0        0        0     4671 2023-04-15 14:29:09.825564 ipython-gpt-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-19 07:57:04.045928 ipython_gpt-0.0.5/LICENSE
+-rw-r--r--   0        0        0     4694 2023-04-22 11:45:10.284927 ipython_gpt-0.0.5/README.md
+-rw-r--r--   0        0        0     1365 2023-04-23 14:07:15.071118 ipython_gpt-0.0.5/ipython_gpt/__init__.py
+-rw-r--r--   0        0        0     2009 2023-04-23 14:07:15.071210 ipython_gpt-0.0.5/ipython_gpt/api_client.py
+-rw-r--r--   0        0        0      791 2023-04-23 14:07:13.749778 ipython_gpt-0.0.5/ipython_gpt/displays.py
+-rw-r--r--   0        0        0     5056 2023-04-23 14:07:15.077081 ipython_gpt-0.0.5/ipython_gpt/subcommands.py
+-rw-r--r--   0        0        0     1123 2023-04-23 14:11:42.724604 ipython_gpt-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     5658 1970-01-01 00:00:00.000000 ipython_gpt-0.0.5/PKG-INFO
```

### Comparing `ipython-gpt-0.0.4/README.md` & `ipython_gpt-0.0.5/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 # IPython ChatGPT extension
 
-This extension allows you to use ChatGPT directly from your Jupyter Notebook or IPython Shell.
+[![Black badge](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![prettier badge](https://img.shields.io/badge/code_style-prettier-ff69b4.svg?logo=prettier&logoColor=white)](https://github.com/prettier/prettier)
+[![pre-commit](https://img.shields.io/badge/pre--commit-active-yellow?logo=pre-commit&logoColor=white)](https://pre-commit.com/)4
+[![test](https://img.shields.io/github/actions/workflow/status/santiagobasulto/ipython-gpt/test.yaml?logo=github&logoColor=white)](https://github.com/santiagobasulto/ipython-gpt/actions/workflows/test.yaml)
+
+This extension allows you to use ChatGPT directly from your Jupyter Notebook or IPython Shell ([Demo](https://github.com/santiagobasulto/ipython-gpt/blob/master/Demo.ipynb)).
 
 <img width="900" alt="IPython GPT, a Jupyter/IPython interface for Chat GPT" src="https://user-images.githubusercontent.com/872296/232230454-44529ea4-920e-4294-9d61-550771a4a95e.png">
 
 <img width="900" alt="IPython GPT, a Jupyter/IPython interface for Chat GPT" src="https://user-images.githubusercontent.com/872296/232230492-9bc50342-9d78-4adb-8168-2f94fcbc3b73.png">
 
-**Important!** This is a very early and raw version, I have a lot of things to improve regarding code quality and missing functionality.
+**Important!** This is a very early and raw version, I have a lot of things to improve regarding code quality and missing functionality. Check [this issue](https://github.com/santiagobasulto/ipython-gpt/issues/4) for a rough "roadmap".
 
 ## Installation
+
 ```python
 !pip install ipython-gpt
 ```
 
 Then in your notebook or ipython shell:
 
 ```ipython
@@ -31,39 +37,37 @@
 
 There are a few other ways to set the API KEY, but the envvar is the recommended one.
 
 ## ChatGPT API
 
 The command `%%chat` interfaces with ChatGPT. It accepts multiple parameters (see Usage). Here's an example:
 
-
 ```python
 %%chat --max-tokens=25
 
 What's the purpose of life?
 ...
 
 >>> CHAT RESPONSE
 ```
 
 **Important** by default, the `%%chat` command preserves the conversation to give the Agent some context, in the same way that ChatGPT works. You can "reset" its status passing the flag `--reset-conversation`.
 
-
 ```python
 %%chat --reset-conversation
 
 How can I avoid pandas using scientific notation in outputs, and do it globally?
 ...
 ...
 >>> CHAT RESPONSE
 ```
 
 ## Agent's role (system message) and other chat parameters
 
-By default, the Chat is started with the role: *"You're a python data science coding assistant"*. You can change that by passing something different in your first `%%chat`:
+By default, the Chat is started with the role: _"You're a python data science coding assistant"_. You can change that by passing something different in your first `%%chat`:
 
 ```ipython
 %%chat --system-message="You're a R Data Science assistant"
 
 Your message...
 ```
 
@@ -81,52 +85,47 @@
 
 ```ipython
 %chat_config --system-message="You're an R data scientist coding assistant specialized in visualizations" --model "other model" --reset-conversation
 ```
 
 Invoke it without parameters to see the defaults set:
 
-
 ```python
 %chat_config
 ...
 
 >>>
 ##### Conf set:
 
 * **Default model**: gpt-3.5-turbo
 * **Default system message**: You're a python data science coding assistant
 * **Chat history length**: 0
 ```
 
-
 ## Other methods
 
 #### Display available models
 
 Usage:
+
 ```bash
 %chat_models [--all-models]
 ```
 
-
 ```python
 %chat_models
 ```
 
-
 ##### Available models:
 
-	- gpt-3.5-turbo-0301
-	- gpt-3.5-turbo
-
+    - gpt-3.5-turbo-0301
+    - gpt-3.5-turbo
 
 #### Display usage and accepted parameters
 
-
 ```python
 %reload_ext ipython_gpt
 %chat_help
 ...
 
 
     usage: ipykernel_launcher.py [-h] [--openai-api-key OPENAI_API_KEY]
@@ -136,10 +135,10 @@
                                  [--temperature TEMPERATURE]
                                  [--max-tokens MAX_TOKENS] [--all-models]
 
 ```
 
 ## Alternative authentication
 
-Aside from setting the environment variable, you can also set `OPENAI_API_KEY` as a global variable in your notebook, or pass it directly as a parameter in any method ``--openai-api-key=YOUR-KEY`.
+Aside from setting the environment variable, you can also set `OPENAI_API_KEY` as a global variable in your notebook, or pass it directly as a parameter in any method `--openai-api-key=YOUR-KEY`.
 
 These alternative methods are NOT recommended, as you might leak your API Key in the notebooks' history, stored in `.ipynb_checkpoints`.
```

### Comparing `ipython-gpt-0.0.4/setup.py` & `ipython_gpt-0.0.5/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,170 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: ipython-gpt
+Version: 0.0.5
+Summary: A Jupyter/IPython extension to use ChatGPT
+Home-page: https://github.com/santiagobasulto/ipython-gpt
+License: MIT
+Keywords: ipython,jupyter,chatgpt,openai
+Author: Santiago Basulto
+Author-email: santiago.basulto@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: Framework :: IPython
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Utilities
+Requires-Dist: ipython (>=8.12.0,<9.0.0)
+Project-URL: Repository, https://github.com/santiagobasulto/ipython-gpt
+Description-Content-Type: text/markdown
 
-modules = \
-['ipython_gpt']
-install_requires = \
-['requests>=2.28.2,<3.0.0']
-
-setup_kwargs = {
-    'name': 'ipython-gpt',
-    'version': '0.0.4',
-    'description': 'A Jupyter/IPython extension to use ChatGPT',
-    'long_description': '# IPython ChatGPT extension\n\nThis extension allows you to use ChatGPT directly from your Jupyter Notebook or IPython Shell.\n\n<img width="900" alt="IPython GPT, a Jupyter/IPython interface for Chat GPT" src="https://user-images.githubusercontent.com/872296/232230454-44529ea4-920e-4294-9d61-550771a4a95e.png">\n\n<img width="900" alt="IPython GPT, a Jupyter/IPython interface for Chat GPT" src="https://user-images.githubusercontent.com/872296/232230492-9bc50342-9d78-4adb-8168-2f94fcbc3b73.png">\n\n**Important!** This is a very early and raw version, I have a lot of things to improve regarding code quality and missing functionality.\n\n## Installation\n```python\n!pip install ipython-gpt\n```\n\nThen in your notebook or ipython shell:\n\n```ipython\n%load_ext ipython_gpt\n```\n\n## Setup\n\nYou must first generate an API key at OpenAI (https://platform.openai.com/account/api-keys) and set is an environment variable `OPENAI_API_KEY`. You can do it by modifying your `.bashrc/.zshrc` or starting jupyter with it:\n\n```bash\n$ OPENAI_API_KEY=[YOUR-KEY] jupyter lab\n# ...\n$ OPENAI_API_KEY=[YOUR-KEY] ipython\n```\n\nThere are a few other ways to set the API KEY, but the envvar is the recommended one.\n\n## ChatGPT API\n\nThe command `%%chat` interfaces with ChatGPT. It accepts multiple parameters (see Usage). Here\'s an example:\n\n\n```python\n%%chat --max-tokens=25\n\nWhat\'s the purpose of life?\n...\n\n>>> CHAT RESPONSE\n```\n\n**Important** by default, the `%%chat` command preserves the conversation to give the Agent some context, in the same way that ChatGPT works. You can "reset" its status passing the flag `--reset-conversation`.\n\n\n```python\n%%chat --reset-conversation\n\nHow can I avoid pandas using scientific notation in outputs, and do it globally?\n...\n...\n>>> CHAT RESPONSE\n```\n\n## Agent\'s role (system message) and other chat parameters\n\nBy default, the Chat is started with the role: *"You\'re a python data science coding assistant"*. You can change that by passing something different in your first `%%chat`:\n\n```ipython\n%%chat --system-message="You\'re a R Data Science assistant"\n\nYour message...\n```\n\nOnce the conversation has started, you can\'t change the original message, as the context is preserved. To do so, you must reset the conversation:\n\n```ipython\n%%chat --system-message="You\'re a R Data Science assistant" --reset-conversation\n\nYour message...\n```\n\n## Setting global config\n\nYou can change the defaults using the `%chat_config` line magic:\n\n```ipython\n%chat_config --system-message="You\'re an R data scientist coding assistant specialized in visualizations" --model "other model" --reset-conversation\n```\n\nInvoke it without parameters to see the defaults set:\n\n\n```python\n%chat_config\n...\n\n>>>\n##### Conf set:\n\n* **Default model**: gpt-3.5-turbo\n* **Default system message**: You\'re a python data science coding assistant\n* **Chat history length**: 0\n```\n\n\n## Other methods\n\n#### Display available models\n\nUsage:\n```bash\n%chat_models [--all-models]\n```\n\n\n```python\n%chat_models\n```\n\n\n##### Available models:\n\n\t- gpt-3.5-turbo-0301\n\t- gpt-3.5-turbo\n\n\n#### Display usage and accepted parameters\n\n\n```python\n%reload_ext ipython_gpt\n%chat_help\n...\n\n\n    usage: ipykernel_launcher.py [-h] [--openai-api-key OPENAI_API_KEY]\n                                 [--reset-conversation]\n                                 [--system-message SYSTEM_MESSAGE]\n                                 [--no-system-message] [--model MODEL]\n                                 [--temperature TEMPERATURE]\n                                 [--max-tokens MAX_TOKENS] [--all-models]\n\n```\n\n## Alternative authentication\n\nAside from setting the environment variable, you can also set `OPENAI_API_KEY` as a global variable in your notebook, or pass it directly as a parameter in any method ``--openai-api-key=YOUR-KEY`.\n\nThese alternative methods are NOT recommended, as you might leak your API Key in the notebooks\' history, stored in `.ipynb_checkpoints`.\n',
-    'author': 'Santiago Basulto',
-    'author_email': 'santiago.basulto@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/santiagobasulto/ipython-gpt',
-    'py_modules': modules,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
+# IPython ChatGPT extension
 
+[![Black badge](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![prettier badge](https://img.shields.io/badge/code_style-prettier-ff69b4.svg?logo=prettier&logoColor=white)](https://github.com/prettier/prettier)
+[![pre-commit](https://img.shields.io/badge/pre--commit-active-yellow?logo=pre-commit&logoColor=white)](https://pre-commit.com/)4
+[![test](https://img.shields.io/github/actions/workflow/status/santiagobasulto/ipython-gpt/test.yaml?logo=github&logoColor=white)](https://github.com/santiagobasulto/ipython-gpt/actions/workflows/test.yaml)
+
+This extension allows you to use ChatGPT directly from your Jupyter Notebook or IPython Shell ([Demo](https://github.com/santiagobasulto/ipython-gpt/blob/master/Demo.ipynb)).
+
+<img width="900" alt="IPython GPT, a Jupyter/IPython interface for Chat GPT" src="https://user-images.githubusercontent.com/872296/232230454-44529ea4-920e-4294-9d61-550771a4a95e.png">
+
+<img width="900" alt="IPython GPT, a Jupyter/IPython interface for Chat GPT" src="https://user-images.githubusercontent.com/872296/232230492-9bc50342-9d78-4adb-8168-2f94fcbc3b73.png">
+
+**Important!** This is a very early and raw version, I have a lot of things to improve regarding code quality and missing functionality. Check [this issue](https://github.com/santiagobasulto/ipython-gpt/issues/4) for a rough "roadmap".
+
+## Installation
+
+```python
+!pip install ipython-gpt
+```
+
+Then in your notebook or ipython shell:
+
+```ipython
+%load_ext ipython_gpt
+```
+
+## Setup
+
+You must first generate an API key at OpenAI (https://platform.openai.com/account/api-keys) and set is an environment variable `OPENAI_API_KEY`. You can do it by modifying your `.bashrc/.zshrc` or starting jupyter with it:
+
+```bash
+$ OPENAI_API_KEY=[YOUR-KEY] jupyter lab
+# ...
+$ OPENAI_API_KEY=[YOUR-KEY] ipython
+```
+
+There are a few other ways to set the API KEY, but the envvar is the recommended one.
+
+## ChatGPT API
+
+The command `%%chat` interfaces with ChatGPT. It accepts multiple parameters (see Usage). Here's an example:
+
+```python
+%%chat --max-tokens=25
+
+What's the purpose of life?
+...
+
+>>> CHAT RESPONSE
+```
+
+**Important** by default, the `%%chat` command preserves the conversation to give the Agent some context, in the same way that ChatGPT works. You can "reset" its status passing the flag `--reset-conversation`.
+
+```python
+%%chat --reset-conversation
+
+How can I avoid pandas using scientific notation in outputs, and do it globally?
+...
+...
+>>> CHAT RESPONSE
+```
+
+## Agent's role (system message) and other chat parameters
+
+By default, the Chat is started with the role: _"You're a python data science coding assistant"_. You can change that by passing something different in your first `%%chat`:
+
+```ipython
+%%chat --system-message="You're a R Data Science assistant"
+
+Your message...
+```
+
+Once the conversation has started, you can't change the original message, as the context is preserved. To do so, you must reset the conversation:
+
+```ipython
+%%chat --system-message="You're a R Data Science assistant" --reset-conversation
+
+Your message...
+```
+
+## Setting global config
+
+You can change the defaults using the `%chat_config` line magic:
+
+```ipython
+%chat_config --system-message="You're an R data scientist coding assistant specialized in visualizations" --model "other model" --reset-conversation
+```
+
+Invoke it without parameters to see the defaults set:
+
+```python
+%chat_config
+...
+
+>>>
+##### Conf set:
+
+* **Default model**: gpt-3.5-turbo
+* **Default system message**: You're a python data science coding assistant
+* **Chat history length**: 0
+```
+
+## Other methods
+
+#### Display available models
+
+Usage:
+
+```bash
+%chat_models [--all-models]
+```
+
+```python
+%chat_models
+```
+
+##### Available models:
+
+    - gpt-3.5-turbo-0301
+    - gpt-3.5-turbo
+
+#### Display usage and accepted parameters
+
+```python
+%reload_ext ipython_gpt
+%chat_help
+...
+
+
+    usage: ipykernel_launcher.py [-h] [--openai-api-key OPENAI_API_KEY]
+                                 [--reset-conversation]
+                                 [--system-message SYSTEM_MESSAGE]
+                                 [--no-system-message] [--model MODEL]
+                                 [--temperature TEMPERATURE]
+                                 [--max-tokens MAX_TOKENS] [--all-models]
+
+```
+
+## Alternative authentication
+
+Aside from setting the environment variable, you can also set `OPENAI_API_KEY` as a global variable in your notebook, or pass it directly as a parameter in any method `--openai-api-key=YOUR-KEY`.
+
+These alternative methods are NOT recommended, as you might leak your API Key in the notebooks' history, stored in `.ipynb_checkpoints`.
 
-setup(**setup_kwargs)
```

