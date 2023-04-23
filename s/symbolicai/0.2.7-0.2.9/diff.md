# Comparing `tmp/symbolicai-0.2.7-py3-none-any.whl.zip` & `tmp/symbolicai-0.2.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,21 @@
-Zip file size: 4111528 bytes, number of entries: 44
+Zip file size: 4116082 bytes, number of entries: 47
 -rw-r--r--  2.0 unx      358 b- defN 23-Jan-21 19:40 bin/symai
--rw-r--r--  2.0 unx     5162 b- defN 23-Feb-03 12:27 symai/__init__.py
+-rw-r--r--  2.0 unx     5162 b- defN 23-Feb-04 16:27 symai/__init__.py
 -rw-r--r--  2.0 unx       90 b- defN 23-Jan-21 19:50 symai/bin.py
--rw-r--r--  2.0 unx     7732 b- defN 23-Jan-21 19:21 symai/chat.py
--rw-r--r--  2.0 unx     7226 b- defN 23-Jan-18 12:54 symai/components.py
+-rw-r--r--  2.0 unx     7884 b- defN 23-Feb-04 16:22 symai/chat.py
+-rw-r--r--  2.0 unx     7647 b- defN 23-Feb-04 14:45 symai/components.py
 -rw-r--r--  2.0 unx   107089 b- defN 23-Feb-03 10:19 symai/core.py
 -rw-r--r--  2.0 unx    30418 b- defN 23-Jan-24 17:12 symai/functional.py
+-rw-r--r--  2.0 unx      666 b- defN 23-Feb-04 14:56 symai/nesy_client.py
+-rw-r--r--  2.0 unx      782 b- defN 23-Feb-04 15:35 symai/nesy_server.py
 -rw-r--r--  2.0 unx     5215 b- defN 23-Jan-25 11:03 symai/post_processors.py
 -rw-r--r--  2.0 unx    21719 b- defN 23-Jan-21 18:15 symai/pre_processors.py
 -rw-r--r--  2.0 unx    56730 b- defN 23-Jan-25 10:06 symai/prompts.py
+-rw-r--r--  2.0 unx     4747 b- defN 23-Feb-04 16:26 symai/shell.py
 -rw-r--r--  2.0 unx      638 b- defN 23-Jan-23 22:13 symai/symai.config.json
 -rw-r--r--  2.0 unx    25137 b- defN 23-Jan-23 23:06 symai/symbol.py
 -rw-r--r--  2.0 unx      541 b- defN 23-Jan-18 12:54 symai/utils.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jan-18 12:54 symai/backend/__init__.py
 -rw-r--r--  2.0 unx     2146 b- defN 23-Feb-03 10:20 symai/backend/base.py
 -rw-r--r--  2.0 unx     2400 b- defN 23-Feb-03 10:20 symai/backend/engine_clip.py
 -rw-r--r--  2.0 unx     2471 b- defN 23-Jan-21 19:01 symai/backend/engine_crawler.py
@@ -29,18 +32,18 @@
 -rw-r--r--  2.0 unx     2765 b- defN 23-Feb-03 10:20 symai/backend/engine_speech.py
 -rw-r--r--  2.0 unx      893 b- defN 23-Jan-18 12:54 symai/backend/engine_userinput.py
 -rw-r--r--  2.0 unx     1425 b- defN 23-Feb-03 10:20 symai/backend/engine_wolframalpha.py
 -rw-r--r--  2.0 unx       17 b- defN 23-Jan-18 12:54 symai/backend/settings.py
 -rw-r--r--  2.0 unx  8907556 b- defN 23-Jan-18 12:54 symai/backend/driver/chromedriver
 -rw-r--r--  2.0 unx     5600 b- defN 23-Feb-03 10:20 symai/backend/driver/webclient.py
 -rw-r--r--  2.0 unx     6388 b- defN 23-Feb-03 10:20 symai/backend/services/huggingface_causallm_server.py
--rw-r--r--  2.0 unx      653 b- defN 23-Feb-03 10:20 symai/backend/services/huggingface_client.py
+-rw-r--r--  2.0 unx      651 b- defN 23-Feb-04 13:18 symai/backend/services/huggingface_client.py
 -rw-r--r--  2.0 unx     6221 b- defN 23-Feb-03 10:20 symai/backend/services/huggingface_seq2seqlm_server.py
--rw-r--r--  2.0 unx      256 b- defN 23-Feb-03 10:20 symai/backend/services/configs/huggingface_causallm.config.json
--rw-r--r--  2.0 unx      264 b- defN 23-Feb-03 10:20 symai/backend/services/configs/huggingface_seq2seqlm.config.json
--rw-r--r--  2.0 unx     1522 b- defN 23-Feb-03 12:28 symbolicai-0.2.7.dist-info/LICENSE
--rw-r--r--  2.0 unx    77253 b- defN 23-Feb-03 12:28 symbolicai-0.2.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-03 12:28 symbolicai-0.2.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       40 b- defN 23-Feb-03 12:28 symbolicai-0.2.7.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 23-Feb-03 12:28 symbolicai-0.2.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     3756 b- defN 23-Feb-03 12:26 symbolicai-0.2.7.dist-info/RECORD
-44 files, 9319077 bytes uncompressed, 4105532 bytes compressed:  55.9%
+-rw-r--r--  2.0 unx      294 b- defN 23-Feb-04 15:01 symai/backend/services/configs/huggingface_causallm.config.json
+-rw-r--r--  2.0 unx      302 b- defN 23-Feb-04 15:02 symai/backend/services/configs/huggingface_seq2seqlm.config.json
+-rw-r--r--  2.0 unx     1522 b- defN 23-Feb-04 16:30 symbolicai-0.2.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx    81465 b- defN 23-Feb-04 16:30 symbolicai-0.2.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Feb-04 16:30 symbolicai-0.2.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx      132 b- defN 23-Feb-04 16:30 symbolicai-0.2.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 23-Feb-04 16:30 symbolicai-0.2.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     3980 b- defN 23-Feb-04 16:28 symbolicai-0.2.9.dist-info/RECORD
+47 files, 9330447 bytes uncompressed, 4109750 bytes compressed:  56.0%
```

## zipnote {}

```diff
@@ -15,23 +15,32 @@
 
 Filename: symai/core.py
 Comment: 
 
 Filename: symai/functional.py
 Comment: 
 
+Filename: symai/nesy_client.py
+Comment: 
+
+Filename: symai/nesy_server.py
+Comment: 
+
 Filename: symai/post_processors.py
 Comment: 
 
 Filename: symai/pre_processors.py
 Comment: 
 
 Filename: symai/prompts.py
 Comment: 
 
+Filename: symai/shell.py
+Comment: 
+
 Filename: symai/symai.config.json
 Comment: 
 
 Filename: symai/symbol.py
 Comment: 
 
 Filename: symai/utils.py
@@ -108,26 +117,26 @@
 
 Filename: symai/backend/services/configs/huggingface_causallm.config.json
 Comment: 
 
 Filename: symai/backend/services/configs/huggingface_seq2seqlm.config.json
 Comment: 
 
-Filename: symbolicai-0.2.7.dist-info/LICENSE
+Filename: symbolicai-0.2.9.dist-info/LICENSE
 Comment: 
 
-Filename: symbolicai-0.2.7.dist-info/METADATA
+Filename: symbolicai-0.2.9.dist-info/METADATA
 Comment: 
 
-Filename: symbolicai-0.2.7.dist-info/WHEEL
+Filename: symbolicai-0.2.9.dist-info/WHEEL
 Comment: 
 
-Filename: symbolicai-0.2.7.dist-info/entry_points.txt
+Filename: symbolicai-0.2.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: symbolicai-0.2.7.dist-info/top_level.txt
+Filename: symbolicai-0.2.9.dist-info/top_level.txt
 Comment: 
 
-Filename: symbolicai-0.2.7.dist-info/RECORD
+Filename: symbolicai-0.2.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## symai/__init__.py

```diff
@@ -1,13 +1,13 @@
 import os
 import json
 import logging
 
 
-SYMAI_VERSION = "0.2.7"
+SYMAI_VERSION = "0.2.9"
 
 
 def _start_symai():
     global _ai_config_
     # check if symai is already initialized
     _ai_config_path_ = os.path.join(os.getcwd(), 'symai.config.json')
     if not os.path.exists(_ai_config_path_):
```

## symai/chat.py

```diff
@@ -99,18 +99,19 @@
 class SymbiaChat(ChatBot):
     def forward(self) -> str:
         message = self.narrate('Symbia introduces herself, writes a greeting message and asks how to help.')        
         while True:
             # query user
             usr = self.input(message)
             
+            # TODO: needs model fine-tuning to improve the classification
             # detect context
             ctxt = self.context_choice(usr)
             
-            if 'option 3' in ctxt: # exit
+            if 'exit' in str(usr) or 'quit' in str(usr): # exit
                 self.narrate('Symbia writes goodbye message.', end=True)
                 break # end chat
             
             elif 'option 4' in ctxt: # help
                 message = self.narrate('Symbia writes for each capability one sentence.', 
                                        context=self.capabilities)
                       
@@ -157,7 +158,12 @@
                 except Exception as e:
                     
                     message = self.narrate('Symbia apologizes and explains the user what went wrong.',
                                             context=str(e))
 
             else: # repeat
                 message = self.narrate('Symbia apologizes and asks the user to restate the question and add more context.')
+
+
+def run() -> None:
+    chat = SymbiaChat()
+    chat()
```

## symai/components.py

```diff
@@ -24,14 +24,29 @@
     def __init__(self, expr: Expression, retries: int = 1):
         super().__init__()
         self.expr: Expression = expr
         self.retries: int = retries
     
     def forward(self, sym: Symbol, **kwargs) -> Symbol:
         return sym.ftry(self.expr, retries=self.retries, **kwargs)
+    
+    
+class Lambda(Expression):
+    def __init__(self, callable: Callable):
+        super().__init__()
+        def _callable(*args, **kwargs):
+            kw = {
+                'args': args,
+                'kwargs': kwargs,
+            }
+            return callable(kw)
+        self.callable: Callable = _callable
+    
+    def forward(self, *args, **kwargs) -> Symbol:
+        return self.callable(*args, **kwargs)
 
 
 class Choice(Expression):
     def __init__(self, cases: List[str], default: Optional[str] = None):
         super().__init__()
         self.cases: List[str] = cases
         self.default: Optional[str] = default
```

## symai/backend/services/huggingface_client.py

```diff
@@ -1,18 +1,18 @@
 import rpyc
 import json
 import os
 from box import Box
 
 
 # check if huggingface mdoel is already initialized
-_hf_config_path_ = os.path.join(os.getcwd(), 'huggingface_seq2seqlm.config.json')
+_hf_config_path_ = os.path.join(os.getcwd(), 'huggingface_causallm.config.json')
 if not os.path.exists(_hf_config_path_):
     _parent_dir_ = os.path.dirname(__file__)
-    _hf_config_path_ = os.path.join(_parent_dir_, 'configs', 'huggingface_seq2seqlm.config.json')
+    _hf_config_path_ = os.path.join(_parent_dir_, 'configs', 'huggingface_causallm.config.json')
 # read the huggingface.config.json file
 with open(_hf_config_path_, 'r') as f:
     _args_ = Box(json.load(f))
 
 
 if __name__ == '__main__':
     connection = rpyc.connect('localhost', _args_.port)
```

## symai/backend/services/configs/huggingface_causallm.config.json

### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'huggingface_cache'": "'tmp/cache'"}*

```diff
@@ -1,10 +1,11 @@
 {
     "device": "cuda",
     "dtype": "float16",
+    "huggingface_cache": "tmp/cache",
     "max_tokens": 128,
     "model": "EleutherAI/gpt-j-6B",
     "no_repeat_ngram_size": 1,
     "num_beams": 3,
     "port": 18100,
     "seed": null,
     "temperature": 0.9,
```

## symai/backend/services/configs/huggingface_seq2seqlm.config.json

### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'huggingface_cache'": "'tmp/cache'"}*

```diff
@@ -1,10 +1,11 @@
 {
     "device": "cuda",
     "dtype": "float16",
+    "huggingface_cache": "tmp/cache",
     "max_tokens": 128,
     "model": "allenai/tk-instruct-11b-def",
     "no_repeat_ngram_size": 1,
     "num_beams": 3,
     "port": 18100,
     "seed": null,
     "temperature": 0.9,
```

## Comparing `symbolicai-0.2.7.dist-info/LICENSE` & `symbolicai-0.2.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `symbolicai-0.2.7.dist-info/METADATA` & `symbolicai-0.2.9.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symbolicai
-Version: 0.2.7
+Version: 0.2.9
 Summary: A Neuro-Symbolic Framework for Python
 Author-email: Marius-Constantin Dinu <office@alphacoreai.eu>
 License: BSD 3-Clause License        
         Copyright (c) 2023, Marius-Constantin Dinu
         All rights reserved.        
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:        
@@ -37,14 +37,15 @@
 License-File: LICENSE
 Requires-Dist: natsort
 Requires-Dist: numpy
 Requires-Dist: tqdm
 Requires-Dist: python-box
 Requires-Dist: wolframalpha
 Requires-Dist: rpyc
+Requires-Dist: pandas
 Requires-Dist: scikit-learn
 Requires-Dist: torch
 Requires-Dist: torchvision
 Requires-Dist: pyyaml
 Requires-Dist: transformers
 Requires-Dist: openai
 Requires-Dist: google-search-results
@@ -63,15 +64,16 @@
 
 ## **A Neuro-Symbolic Perspective on Large Language Models (LLMs)**
 
 *Building applications with LLMs at its core through our `Symbolic API` leverages the power of classical and differentiable programming in Python.*
 
 Read further [**documentation here**](https://symbolicai.readthedocs.io/).
 
-[![PyPI version](https://badge.fury.io/py/symbolicai.svg)](https://badge.fury.io/py/symbolicai) [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause) [![Twitter](https://img.shields.io/twitter/url/https/twitter.com/langchainai.svg?style=social&label=Follow%20%40DinuMariusC)](https://twitter.com/DinuMariusC) [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/Xpitfire/symbolicai/issues) [![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FXpitfire%2Fsymbolicai&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://hits.seeyoufarm.com)
+[![PyPI version](https://badge.fury.io/py/symbolicai.svg)](https://badge.fury.io/py/symbolicai) [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause) [![Twitter](https://img.shields.io/twitter/url/https/twitter.com/dinumariusc.svg?style=social&label=Follow%20%40DinuMariusC)](https://twitter.com/DinuMariusC) [![Twitter](https://img.shields.io/twitter/url/https/twitter.com/symbolicapi.svg?style=social&label=Follow%20%40SymbolicAI)](https://twitter.com/SymbolicAPI) [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/Xpitfire/symbolicai/issues)
+[![Discord](https://img.shields.io/discord/768087161878085643?label=Discord&logo=Discord&logoColor=white)](https://discord.gg/QYMNnh9ra8) [![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FXpitfire%2Fsymbolicai&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://hits.seeyoufarm.com)
 
 <img src="https://raw.githubusercontent.com/Xpitfire/symbolicai/main/assets/images/preview.gif">
 
 ## Abstract
 
 Conceptually, SymbolicAI is a framework that uses machine learning - and specifically LLMs - at its core, and composes operations based on task-specific prompting. We adopt a divide and conquer approach to decompose a complex problem into smaller problems. Therefore, each operation solves a simple task. By re-combining these operations we can solve the complex problem. Furthermore, our design principles allow us to transition between differentiable and classical programming, and to leverage the power of both worlds.
 
@@ -79,16 +81,21 @@
 
 - [**SymbolicAI**](#symbolicai)
   - [**A Neuro-Symbolic Perspective on Large Language Models (LLMs)**](#a-neuro-symbolic-perspective-on-large-language-models-llms)
   - [Abstract](#abstract)
   - [📖 Table of Contents](#-table-of-contents)
   - [🔧 Get Started](#-get-started)
     - [➡️ Quick Install](#️-quick-install)
+    - [API Keys](#api-keys)
     - [*\[Optional\]* Installs](#optional-installs)
-    - [💯 Use Cases](#-use-cases)
+  - [🦖 Apps](#-apps)
+    - [Shell Command Tool](#shell-command-tool)
+    - [Chatbot](#chatbot)
+    - [💯 Other Use Cases](#-other-use-cases)
+    - [Community demos](#community-demos)
   - [🤷‍♂️ Why SymbolicAI?](#️-why-symbolicai)
   - [ Tell me some more fun facts!](#-tell-me-some-more-fun-facts)
   - [😶‍🌫️ How does it work?](#️-how-does-it-work)
     - [📚 Symbolic operations](#-symbolic-operations)
     - [Ranking objects](#ranking-objects)
     - [Evaluating Expressions by best effort](#evaluating-expressions-by-best-effort)
     - [Dynamic casting](#dynamic-casting)
@@ -114,39 +121,44 @@
     - [OCR Engine](#ocr-engine)
     - [Search Engine](#search-engine)
     - [WebCrawler Engine](#webcrawler-engine)
     - [Drawing Engine](#drawing-engine)
     - [File Engine](#file-engine)
     - [Indexing Engine](#indexing-engine)
     - [CLIP Engine](#clip-engine)
+    - [Local Neuro-Symbolic Engine](#local-neuro-symbolic-engine)
     - [Custom Engine](#custom-engine)
   - [⚡Limitations](#limitations)
   - [🥠 Future Work](#-future-work)
   - [Conclusion](#conclusion)
   - [👥 References, Related Work \& Credits](#-references-related-work--credits)
     - [Comparison to other frameworks](#comparison-to-other-frameworks)
     - [Acknowledgements](#acknowledgements)
     - [Contribution](#contribution)
     - [📜 Citation](#-citation)
     - [📝 License](#-license)
     - [Like this project?](#like-this-project)
     - [📫 Contact](#-contact)
 
 
-
 ## 🔧 Get Started
 
-
 ### ➡️ Quick Install
 
-
 ```bash
 pip install symbolicai
 ```
 
+One can run our framework in two ways:
+
+* using local engines (`experimental`) that are run on your local machine ([see Local Neuro-Symbolic Engine section](#local-neuro-symbolic-engine)), or
+* using engines powered by external APIs, i.e. using OpenAI's API ([see API Keys](#api-keys)).
+
+### API Keys
+
 Before the first run, define exports for the required `API keys` to enable the respective engines. This will register the keys in the internally for subsequent runs. By default `SymbolicAI` currently uses OpenAI's neural engines, i.e. GPT-3 Davinci-003, DALL·E 2 and Embedding Ada-002, for the neuro-symbolic computations, image generation and embeddings computation respectively. However, these modules can easily be replaced with open-source alternatives. Examples are 
 - [OPT](https://huggingface.co/docs/transformers/model_doc/opt) or [Bloom](https://huggingface.co/bigscience/bloom) for neuro-symbolic computations, 
 - [Craiyon](https://www.craiyon.com/) for image generation, 
 - and any [BERT variants](https://huggingface.co/models) for semantic embedding computations. 
 
 To set the OpenAI API Keys use the following command:
 
@@ -253,27 +265,90 @@
     "SPEECH_ENGINE_MODEL": "base",
     "SELENIUM_CHROME_DRIVER_VERSION": "110.0.5481.30",
     "INDEXING_ENGINE_API_KEY": "<PINECONE_API_KEY>",
     "INDEXING_ENGINE_ENVIRONMENT": "us-west1-gcp"
 }
 ```
 
-### 💯 Use Cases
+## 🦖 Apps
+
+Over the course of th next weeks, we will expand our experimental demo apps and provide a set of useful tools that showcase how to interact with our framework. These apps are made available by calling the `sym+<shortcut-name-of-app>` command in your `terminal` or `PowerShell`.
+
+### Shell Command Tool
+
+You can start a basic shell command support tool that translates natural language commands into shell commands. To start the shell command tool, simply run:
+
+```bash
+symsh "<your-query>"
+```
+
+You can also use the `--help` flag to get more information about the tool and available arguments.
+
+```bash
+symsh --help
+```
+
+Here is an example of how to use the tool:
+
+```bash
+$> symsh "PowerShell edit registiry entry"
+
+# :Output:
+# Set-ItemProperty -Path <path> -Name <name> -Value <value>
+
+$> symsh "Set-ItemProperty -Path <path> -Name <name> -Value <value>" --add "path='/Users/myuser' name=Demo value=SymbolicAI"
+
+# :Output:
+# Set-ItemProperty -Path '/Users/myuser' -Name Demo -Value SymbolicAI
+
+$> symsh "Set-ItemProperty -Path '/Users/myuser' -Name Demo -Value SymbolicAI" --del "string quotes"
+
+# :Output:
+# Set-ItemProperty -Path /Users/myuser -Name Demo -Value SymbolicAI
+
+$> symsh "Set-ItemProperty -Path '/Users/myuser' -Name Demo -Value SymbolicAI" --convert "linux"
+
+# :Output:
+# export Demo="SymbolicAI"
+```
+
+### Chatbot
+
+You can start a basic conversation with `Symbia`. `Symbia` is a chatbot that uses `SymbolicAI` to detect the content of your request and switch between different contextual modes to answer your questions. These mode include search engines, speech engines and more. To start the chatbot, simply run:
+
+```bash
+symchat
+```
+
+This will start now a chatbot interface:
+
+```bash
+Symbia: Hi there! I'm Symbia, your virtual assistant. How may I help you?
+$> 
+```
+
+You can exit the conversation by either typing `exit`, `quit` or pressing `Ctrl+C`.
+
+### 💯 Other Use Cases
 
 We compiled a few examples to show how to use our Symbolic API. You can find them in the `notebooks` folder.
 
 - *Basics*: See our basics notebook to get familiar with our API structure ([notebooks/Basics.ipynb](notebooks/Basics.ipynb))
 - *Queries*: See our query manipulation notebook for contextualized operations ([notebooks/Queries.ipynb](notebooks/Queries.ipynb))
 - *News & Docs Generation*: See our news and documentation generation notebook for stream processing ([notebooks/News.ipynb](notebooks/News.ipynb))
 - *ChatBot*: See how to implement a custom chatbot based on semantic narrations ([notebooks/ChatBot.ipynb](notebooks/ChatBot.ipynb))
 
 
 You can solve many more problems with our Symbolic API. We are looking forward to see what you will build with it. Keep us posted on our shared community space on [Discord: AI Is All You Need / SymbolicAI](https://discord.gg/QYMNnh9ra8).
 
 
+### Community demos
+
+We are listing all your cool demos and tools that you build with our framework. If you want to add your project just PM on Twitter at [@SymbolicAPI](https://twitter.com/SymbolicAPI) or via [Discord](https://discord.gg/QYMNnh9ra8).
+
 ## 🤷‍♂️ Why SymbolicAI?
 
 SymbolicAI tries to close the gap between classical programming or Software 1.0 and modern data-driven programming (aka Software 2.0). It is a framework that allows to build software applications, which are able to utilize the power of large language models (LLMs) wtih composability and inheritance - two powerful concepts from the object-oriented classical programming paradigm.
 
 This allows to move along the spectrum between the classical programming realm and data-driven programming realm as illustrated in the following figure:
 
 <img src="https://raw.githubusercontent.com/Xpitfire/symbolicai/main/assets/images/img5.png" width="720px">
@@ -973,14 +1048,49 @@
 ```bash
 :Output:
 array([[9.72840726e-01, 6.34790864e-03, 2.59368378e-03, 3.41371237e-03,
         3.71197984e-03, 8.53193272e-03, 1.03346225e-04, 2.08464009e-03,
         1.77942711e-04, 1.94185617e-04]], dtype=float32)
 ```
 
+### Local Neuro-Symbolic Engine
+
+One can use the a locally hosted instance for the Neuro-Symbolic Engine. Out of the box we provide a Hugging Face client-server backend and host the model `EleutherAI/gpt-j-6B` to perform the inference. As the name suggests this is a six billion parameter model and requires a GPU with ~16GB RAM to run properly. The following example shows how to host and configure the usage of the local Neuro-Symbolic Engine.
+
+Fist we start the backend server:
+
+```bash
+# optional: set cache folder for transformers (Linux/MacOS)
+export TRANSFORMERS_CACHE="<path-to-cache-folder>"
+# start server backend (default model is EleutherAI/gpt-j-6B)
+symsvr
+# initialize server with client call
+symclient
+```
+
+Then use once the following code to set up the local engine:
+
+```python
+from symai.backend.engine_nesy_client import NeSyClientEngine
+# setup local engine
+engine = NeSyClientEngine()
+setting = Expression()
+setting.setup(engines={'neurosymbolic': engine})
+setting.command(time_clock=True)
+```
+
+Now you can use the local engine to perform symbolic computation:
+```python
+# do some symbolic computation with the local engine
+sym = Symbol('cats are cute')
+res = sym.compose()
+...
+```
+
+
 ### Custom Engine
 
 If you want to replace or extend the functionality of our framework, you can do this by customizing the existing engines or creating new engines. The `Symbol` class provides for this functionality some helper methods, such as `command` and `setup`. The `command` method can pass on configurations (as `**kwargs`) to the engines and change functionalities or parameters. The `setup` method can be used to re-initialize an engine with your custom engine implementation which must sub-class the `Engine` class. Both methods can be specified to address one, more or all engines.
 
 Here is an example how to initialize your own engine. We will sub-class the existing `GPT3Engine` and override the `prepare` method. This method is called before the neural computation and can be used to modify the parameters of the actual input prompt that will be passed in for execution. In this example, we will replace the prompt with dummy text for illustration purposes:
```

## Comparing `symbolicai-0.2.7.dist-info/RECORD` & `symbolicai-0.2.9.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 bin/symai,sha256=5d48gMvNOV5S_b0FKxPuKg7O790cnYh3diPQUPG0UwM,358
-symai/__init__.py,sha256=7aK5yUjJlW5paji6U5GA425XWzImmmtTdNJ3nrWm96w,5162
+symai/__init__.py,sha256=Po7V3Z4PbMYx7_CDleor53j0jaGPKScCsvI9nrKX2SE,5162
 symai/bin.py,sha256=lOAbLdnNzpZJq6VMyQSq3f9CkuNccjXfs88ZSE4_Z2U,90
-symai/chat.py,sha256=2FLmCXQM7dCSM4JDto7VcS0X7Yba4LsWmAwaYzRL7-g,7732
-symai/components.py,sha256=4YyFhtPrMc73pgg70dPAgq5XUGDBBR6ZfiihfQQZ2N8,7226
+symai/chat.py,sha256=wOlTdV41BAEygaoZLL8gNn1Oe2KFDyCpim9qAgGkS2c,7884
+symai/components.py,sha256=3GYGBhyqLFzRywxQXMbNekL7rHBQc9d56CB4m6pZwPA,7647
 symai/core.py,sha256=d4mdWrypBwlTm0LQm2ptbiOxa21X0fia3hjhfz1vXMk,107089
 symai/functional.py,sha256=1IAXVq9SHwujUGQMtTN5WyhacJPSgcTqJf9xSg_17ow,30418
+symai/nesy_client.py,sha256=vID1LwNyJCaBWmq37gYlycL_EK4pjtRigA2-rYPTfw4,666
+symai/nesy_server.py,sha256=65qObUKhAUFOuesSvEyMjRz89VvXKliVFizQWy0jBSU,782
 symai/post_processors.py,sha256=Yu38fuf-wWcbm4V70wEQyzGvqsdv3Y-u_FSug9tGPzk,5215
 symai/pre_processors.py,sha256=Y1LRG7GZiFSzrgQPViOCNoCXLMYk1ZzO0wcEpQlFDeU,21719
 symai/prompts.py,sha256=2vZzcQUi5OKcF_6GYfHczvg_Q-cGhD7tIPIC5lRj4H0,56730
+symai/shell.py,sha256=XWk6nSTyERB5g0TdQenPGHm5_n-AdVfp87fCf1U1eKo,4747
 symai/symai.config.json,sha256=MHBmGjVshoSVkpO1x5QcViPWXMkgOTVUoD3dEO-2GjU,638
 symai/symbol.py,sha256=L8PA50p9tH06uQlY5sAfQhjqKA96SNig6ZUNW37za_k,25137
 symai/utils.py,sha256=U7KKS7VBc20yniDlmfSRiNMnU4z0aCltIfIb0FxeC6U,541
 symai/backend/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 symai/backend/base.py,sha256=uSlef7R9-vqUDHdfx6gZvDhnKAyzULAvWrvok956uNU,2146
 symai/backend/engine_clip.py,sha256=Aag3qakALkiy-SSyULf8qu9KZDqCmvvSg1zYeg2ue_E,2400
 symai/backend/engine_crawler.py,sha256=sAXrdwL2TivqzXQZNOLX4oDXP3o95bA_do7JmvjjHTk,2471
@@ -28,17 +31,17 @@
 symai/backend/engine_speech.py,sha256=rj-ShxOXXEYrHdbfB1p_H93mYo_Hc4sYqofeZKbRGY8,2765
 symai/backend/engine_userinput.py,sha256=2C1FA3NIa8rSzpLAfOmQcX_yV4KkgymXXvY4LXLN1jU,893
 symai/backend/engine_wolframalpha.py,sha256=Dw6S6eOnZrvr5AygsjdGQmDrFG3HbTPHF2L7HCnoefs,1425
 symai/backend/settings.py,sha256=TLMA0Bybh5ysXltqH29SrHUNIybmq3_bsxZLpBa_HIU,17
 symai/backend/driver/chromedriver,sha256=9skEK6UCfvtH_G3pBnGG8XKeNnhlVrdMnnCyCaOWkck,8907556
 symai/backend/driver/webclient.py,sha256=aIGpCEtT2g5INCkr_dolxcq01WqIQvxZsDZjHfT8CC8,5600
 symai/backend/services/huggingface_causallm_server.py,sha256=4UD1IEO5iVLZnxASp518l2BbWd9JReOTbxdlp5ljj9k,6388
-symai/backend/services/huggingface_client.py,sha256=Nl1NvtQk49LR0xnbU86xkZO96-SsidyqemyxWXI5XCU,653
+symai/backend/services/huggingface_client.py,sha256=lzOCbyKBsrcK-Jwie0qpi1rNjHrFYF_sJ_ONm_praXQ,651
 symai/backend/services/huggingface_seq2seqlm_server.py,sha256=UEK5r0DL7bYIYSQMYmqCO5HliGwgejm3N5ryNFwQ4WQ,6221
-symai/backend/services/configs/huggingface_causallm.config.json,sha256=vhE4GiSlZztvE919J9PmTHGvJFsTFU8-lxhxIylZg9E,256
-symai/backend/services/configs/huggingface_seq2seqlm.config.json,sha256=hiMRLzC7IakVDKatB85cPDWE7x-XlCK9k3Mtju-r6gY,264
-symbolicai-0.2.7.dist-info/LICENSE,sha256=5rTECOR-2pWyUmoHZSahafvHD5p-bSrSxg-Hslmj96E,1522
-symbolicai-0.2.7.dist-info/METADATA,sha256=CrZI8KKiMXCPLHNeCQRvi4J3juFZNNxqL5_7cNwXVMY,77253
-symbolicai-0.2.7.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-symbolicai-0.2.7.dist-info/entry_points.txt,sha256=S8edgvPZ2IwhBW0Cy4_ho-z4EEXQY1LhuWyG68kYzJo,40
-symbolicai-0.2.7.dist-info/top_level.txt,sha256=bOoIDfpDIvCQtQgXcwVKJvxAKwsxpxo2IL4z92rNJjw,6
-symbolicai-0.2.7.dist-info/RECORD,,
+symai/backend/services/configs/huggingface_causallm.config.json,sha256=NNYK_OTwJ54GtzmDxuxmRigRBSfzwVVT9zieR2wh51M,294
+symai/backend/services/configs/huggingface_seq2seqlm.config.json,sha256=beUOFWlvtp2J6F2HukQnlql1BPO3I7CnmCW-xIVBlf8,302
+symbolicai-0.2.9.dist-info/LICENSE,sha256=5rTECOR-2pWyUmoHZSahafvHD5p-bSrSxg-Hslmj96E,1522
+symbolicai-0.2.9.dist-info/METADATA,sha256=uPMJ-tJdb93pAs9OEH4ma0nanxfVGzmWFML5VFmSRvw,81465
+symbolicai-0.2.9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+symbolicai-0.2.9.dist-info/entry_points.txt,sha256=TbjH2WmTN1gpKksMtQBpiCmJeMkOGG508Csdq5t2oJw,132
+symbolicai-0.2.9.dist-info/top_level.txt,sha256=bOoIDfpDIvCQtQgXcwVKJvxAKwsxpxo2IL4z92rNJjw,6
+symbolicai-0.2.9.dist-info/RECORD,,
```

