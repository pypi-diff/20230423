# Comparing `tmp/pyllms-0.1.8.tar.gz` & `tmp/pyllms-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyllms-0.1.8.tar", last modified: Fri Apr 21 16:52:40 2023, max compression
+gzip compressed data, was "pyllms-0.1.9.tar", last modified: Sun Apr 23 03:41:14 2023, max compression
```

## Comparing `pyllms-0.1.8.tar` & `pyllms-0.1.9.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-21 16:52:40.509910 pyllms-0.1.8/
--rw-r--r--   0 prelovac   (502) staff       (20)     1068 2023-04-10 01:29:26.000000 pyllms-0.1.8/LICENSE
--rw-r--r--   0 prelovac   (502) staff       (20)    14670 2023-04-21 16:52:40.509549 pyllms-0.1.8/PKG-INFO
--rw-r--r--   0 prelovac   (502) staff       (20)    13429 2023-04-21 16:52:18.000000 pyllms-0.1.8/README.md
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-21 16:52:40.504559 pyllms-0.1.8/llms/
--rw-r--r--   0 prelovac   (502) staff       (20)      295 2023-04-13 02:24:28.000000 pyllms-0.1.8/llms/__init__.py
--rw-r--r--   0 prelovac   (502) staff       (20)    18089 2023-04-21 16:50:45.000000 pyllms-0.1.8/llms/llms.py
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-21 16:52:40.507639 pyllms-0.1.8/llms/providers/
--rw-r--r--   0 prelovac   (502) staff       (20)      107 2023-04-09 20:11:29.000000 pyllms-0.1.8/llms/providers/__init__.py
--rw-r--r--   0 prelovac   (502) staff       (20)     2333 2023-04-13 21:39:49.000000 pyllms-0.1.8/llms/providers/ai21.py
--rw-r--r--   0 prelovac   (502) staff       (20)     6657 2023-04-21 16:48:57.000000 pyllms-0.1.8/llms/providers/anthropic.py
--rw-r--r--   0 prelovac   (502) staff       (20)     5645 2023-04-21 16:48:57.000000 pyllms-0.1.8/llms/providers/openai.py
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-21 16:52:40.509164 pyllms-0.1.8/pyllms.egg-info/
--rw-r--r--   0 prelovac   (502) staff       (20)    14670 2023-04-21 16:52:40.000000 pyllms-0.1.8/pyllms.egg-info/PKG-INFO
--rw-r--r--   0 prelovac   (502) staff       (20)      308 2023-04-21 16:52:40.000000 pyllms-0.1.8/pyllms.egg-info/SOURCES.txt
--rw-r--r--   0 prelovac   (502) staff       (20)        1 2023-04-21 16:52:40.000000 pyllms-0.1.8/pyllms.egg-info/dependency_links.txt
--rw-r--r--   0 prelovac   (502) staff       (20)       69 2023-04-21 16:52:40.000000 pyllms-0.1.8/pyllms.egg-info/requires.txt
--rw-r--r--   0 prelovac   (502) staff       (20)        5 2023-04-21 16:52:40.000000 pyllms-0.1.8/pyllms.egg-info/top_level.txt
--rw-r--r--   0 prelovac   (502) staff       (20)       38 2023-04-21 16:52:40.510003 pyllms-0.1.8/setup.cfg
--rw-r--r--   0 prelovac   (502) staff       (20)     1780 2023-04-21 16:50:58.000000 pyllms-0.1.8/setup.py
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-23 03:41:14.560379 pyllms-0.1.9/
+-rw-r--r--   0 prelovac   (502) staff       (20)     1068 2023-04-10 01:29:26.000000 pyllms-0.1.9/LICENSE
+-rw-r--r--   0 prelovac   (502) staff       (20)    16914 2023-04-23 03:41:14.560065 pyllms-0.1.9/PKG-INFO
+-rw-r--r--   0 prelovac   (502) staff       (20)    15601 2023-04-23 03:36:41.000000 pyllms-0.1.9/README.md
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-23 03:41:14.554361 pyllms-0.1.9/llms/
+-rw-r--r--   0 prelovac   (502) staff       (20)      295 2023-04-13 02:24:28.000000 pyllms-0.1.9/llms/__init__.py
+-rw-r--r--   0 prelovac   (502) staff       (20)    19018 2023-04-23 03:31:42.000000 pyllms-0.1.9/llms/llms.py
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-23 03:41:14.558381 pyllms-0.1.9/llms/providers/
+-rw-r--r--   0 prelovac   (502) staff       (20)      228 2023-04-23 02:39:46.000000 pyllms-0.1.9/llms/providers/__init__.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     2449 2023-04-23 01:59:45.000000 pyllms-0.1.9/llms/providers/ai21.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     2696 2023-04-23 02:28:11.000000 pyllms-0.1.9/llms/providers/aleph.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     6612 2023-04-23 03:05:56.000000 pyllms-0.1.9/llms/providers/anthropic.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     3641 2023-04-23 02:28:09.000000 pyllms-0.1.9/llms/providers/cohere.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     2551 2023-04-23 03:25:52.000000 pyllms-0.1.9/llms/providers/huggingface.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     5558 2023-04-23 01:59:45.000000 pyllms-0.1.9/llms/providers/openai.py
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-23 03:41:14.559726 pyllms-0.1.9/pyllms.egg-info/
+-rw-r--r--   0 prelovac   (502) staff       (20)    16914 2023-04-23 03:41:14.000000 pyllms-0.1.9/pyllms.egg-info/PKG-INFO
+-rw-r--r--   0 prelovac   (502) staff       (20)      387 2023-04-23 03:41:14.000000 pyllms-0.1.9/pyllms.egg-info/SOURCES.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)        1 2023-04-23 03:41:14.000000 pyllms-0.1.9/pyllms.egg-info/dependency_links.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)       85 2023-04-23 03:41:14.000000 pyllms-0.1.9/pyllms.egg-info/requires.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)        5 2023-04-23 03:41:14.000000 pyllms-0.1.9/pyllms.egg-info/top_level.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)       38 2023-04-23 03:41:14.560469 pyllms-0.1.9/setup.cfg
+-rw-r--r--   0 prelovac   (502) staff       (20)     1882 2023-04-23 03:37:05.000000 pyllms-0.1.9/setup.py
```

### Comparing `pyllms-0.1.8/LICENSE` & `pyllms-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyllms-0.1.8/PKG-INFO` & `pyllms-0.1.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pyllms
-Version: 0.1.8
-Summary: Minimal Python library to connect to LLMs (OpenAI, Anthropic, AI21), with a built-in model performance benchmark.
+Version: 0.1.9
+Summary: Minimal Python library to connect to LLMs (OpenAI, Anthropic, AI21, Cohere, Aleph-Alpha, HuggingfaceHub), with a built-in model performance benchmark.
 Author: Vladimir Prelovac
 Author-email: vlad@kagi.com
 Project-URL: Documentation, https://github.com/kagisearch/pyllms
 Project-URL: Source Code, https://github.com/kagisearch/pyllms
 Project-URL: Issue Tracker, https://github.com/kagisearch/pyllms/issues
-Keywords: llm,llms,large language model,AI,NLP,natural language processing,gpt,chatgpt,openai,anthropic,ai21
+Keywords: llm,llms,large language model,AI,NLP,natural language processing,gpt,chatgpt,openai,anthropic,ai21,cohere,aleph alpha,huggingface hub
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -25,21 +25,21 @@
 License-File: LICENSE
 
 
 # PyLLMs
 
 [![](https://dcbadge.vercel.app/api/server/aDNg6E9szy?compact=true&style=flat)](https://discord.gg/aDNg6E9szy) [![Twitter](https://img.shields.io/twitter/follow/KagiHQ?style=social)](https://twitter.com/KagiHQ) [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/license/mit/) 
 
-PyLLMs is a minimal Python library to connect to LLMs (OpenAI, Anthropic, AI21), with a built-in model performance benchmark. 
+PyLLMs is a minimal Python library to connect to LLMs (OpenAI, Anthropic, AI21, Cohere, Aleph Alpha, HuggingfaceHub) with a built-in model performance benchmark. 
 
-It is ideal for fast prototyping and evaluationg different models thanks to:
-- Connect to top LLMs in few lines of code (currenly OpenAI, Anthropic and AI21 are supported)
+It is ideal for fast prototyping and evaluating different models thanks to:
+- Connect to top LLMs in s few lines of code (currently OpenAI, Anthropic and AI21 are supported)
 - Response meta includes tokens processed, cost and latency standardized across the models
-- Multi-model support: Get completitions from different models at the same time
-- LLM benchmark: Eevaluate models on quality, speed and cost
+- Multi-model support: Get completions from different models at the same time
+- LLM benchmark: Evaluate models on quality, speed and cost
 
 Feel free to reuse and expand. Pull requests are welcome.
 
 ## Installation
 
 Clone this repository and install the package using pip:
 
@@ -166,78 +166,106 @@
 ```
 models=llms.init(model=['gpt-3.5-turbo', 'claude-instant-v1', 'j2-jumbo-instruct'])
 gpt4=llms.init('gpt-4') # optional, evaluator can be ommited and in that case only speed and cost will be evaluated
 models.benchmark(evaluator=gpt4)
 ```
 
 ```
-+---------------------------------------+--------------------+---------------------+-----------------------+---------------------------+-----------------+
-|                 Model                 |       Tokens       |       Cost ($)      |      Latency (s)      |     Speed (tokens/sec)    |    Evaluation   |
-+---------------------------------------+--------------------+---------------------+-----------------------+---------------------------+-----------------+
-| AnthropicProvider (claude-instant-v1) |         33         |       0.00003       |          0.40         |           82.19           |        3        |
-| AnthropicProvider (claude-instant-v1) |        152         |       0.00019       |          1.65         |           91.89           |        10       |
-| AnthropicProvider (claude-instant-v1) |        248         |       0.00031       |          2.18         |           113.74          |        9        |
-| AnthropicProvider (claude-instant-v1) |        209         |       0.00021       |          1.86         |           112.11          |        10       |
-| AnthropicProvider (claude-instant-v1) |         59         |       0.00006       |          0.87         |           68.18           |        10       |
-| AnthropicProvider (claude-instant-v1) |        140         |       0.00018       |          1.46         |           96.10           |        10       |
-| AnthropicProvider (claude-instant-v1) |        245         |       0.00031       |          2.45         |           100.16          |        9        |
-| AnthropicProvider (claude-instant-v1) |        250         |       0.00031       |          2.29         |           109.35          |        9        |
-| AnthropicProvider (claude-instant-v1) |        248         |       0.00031       |          2.17         |           114.50          |        9        |
-| AnthropicProvider (claude-instant-v1) |        323         |       0.00034       |          1.95         |           165.57          |        8        |
-| AnthropicProvider (claude-instant-v1) |        172         |       0.00014       |          0.97         |           177.63          |        10       |
-| AnthropicProvider (claude-instant-v1) | Total Tokens: 2079 | Total Cost: 0.00240 |  Median Latency: 1.86 | Aggregrated speed: 113.98 | Total Score: 97 |
-|     OpenAIProvider (gpt-3.5-turbo)    |         37         |       0.00007       |          1.20         |           30.86           |        7        |
-|     OpenAIProvider (gpt-3.5-turbo)    |         93         |       0.00019       |          2.89         |           32.19           |        1        |
-|     OpenAIProvider (gpt-3.5-turbo)    |        451         |       0.00090       |         18.10         |           24.91           |        10       |
-|     OpenAIProvider (gpt-3.5-turbo)    |        204         |       0.00041       |          5.60         |           36.45           |        10       |
-|     OpenAIProvider (gpt-3.5-turbo)    |        366         |       0.00073       |         16.51         |           22.17           |        10       |
-|     OpenAIProvider (gpt-3.5-turbo)    |        109         |       0.00022       |          3.69         |           29.51           |        10       |
-|     OpenAIProvider (gpt-3.5-turbo)    |        316         |       0.00063       |         11.96         |           26.43           |        10       |
-|     OpenAIProvider (gpt-3.5-turbo)    |        294         |       0.00059       |         10.47         |           28.09           |        10       |
-|     OpenAIProvider (gpt-3.5-turbo)    |        275         |       0.00055       |         10.02         |           27.45           |        10       |
-|     OpenAIProvider (gpt-3.5-turbo)    |        501         |       0.00100       |         16.28         |           30.77           |        10       |
-|     OpenAIProvider (gpt-3.5-turbo)    |        180         |       0.00036       |          3.23         |           55.79           |        10       |
-|     OpenAIProvider (gpt-3.5-turbo)    | Total Tokens: 2826 | Total Cost: 0.00565 | Median Latency: 10.02 |  Aggregrated speed: 28.28 | Total Score: 98 |
-|    AI21Provider (j2-jumbo-instruct)   |         27         |       0.00040       |          0.95         |           28.31           |        3        |
-|    AI21Provider (j2-jumbo-instruct)   |        114         |       0.00171       |          3.10         |           36.81           |        1        |
-|    AI21Provider (j2-jumbo-instruct)   |        195         |       0.00293       |          5.62         |           34.73           |        10       |
-|    AI21Provider (j2-jumbo-instruct)   |        117         |       0.00176       |          2.08         |           56.12           |        10       |
-|    AI21Provider (j2-jumbo-instruct)   |        216         |       0.00324       |          6.12         |           35.27           |        7        |
-|    AI21Provider (j2-jumbo-instruct)   |         67         |       0.00101       |          2.01         |           33.39           |        10       |
-|    AI21Provider (j2-jumbo-instruct)   |        229         |       0.00344       |          6.14         |           37.27           |        10       |
-|    AI21Provider (j2-jumbo-instruct)   |        225         |       0.00337       |          6.21         |           36.26           |        5        |
-|    AI21Provider (j2-jumbo-instruct)   |        218         |       0.00327       |          5.90         |           36.95           |        1        |
-|    AI21Provider (j2-jumbo-instruct)   |        281         |       0.00421       |          6.25         |           44.97           |        1        |
-|    AI21Provider (j2-jumbo-instruct)   |        149         |       0.00224       |          1.56         |           95.81           |        10       |
-|    AI21Provider (j2-jumbo-instruct)   | Total Tokens: 1838 | Total Cost: 0.02757 |  Median Latency: 5.62 |  Aggregrated speed: 40.01 | Total Score: 68 |
-+---------------------------------------+--------------------+---------------------+-----------------------+---------------------------+-----------------+
++--------------------------------+--------------------+---------------------+----------------------+-------------------------+-----------------+
+|             Model              |       Tokens       |       Cost ($)      |     Latency (s)      |    Speed (tokens/sec)   |    Evaluation   |
++--------------------------------+--------------------+---------------------+----------------------+-------------------------+-----------------+
+| OpenAIProvider (gpt-3.5-turbo) |         37         |       0.00007       |         1.47         |          25.19          |        1        |
+| OpenAIProvider (gpt-3.5-turbo) |         93         |       0.00019       |         4.13         |          22.53          |        0        |
+| OpenAIProvider (gpt-3.5-turbo) |        360         |       0.00072       |        18.42         |          19.54          |        5        |
+| OpenAIProvider (gpt-3.5-turbo) |        143         |       0.00029       |         6.76         |          21.15          |        5        |
+| OpenAIProvider (gpt-3.5-turbo) |        112         |       0.00022       |         3.87         |          28.95          |        4        |
+| OpenAIProvider (gpt-3.5-turbo) |         47         |       0.00009       |         1.57         |          29.86          |        5        |
+| OpenAIProvider (gpt-3.5-turbo) |         78         |       0.00016       |         1.52         |          51.19          |        5        |
+| OpenAIProvider (gpt-3.5-turbo) |        254         |       0.00051       |         1.08         |          235.22         |        5        |
+| OpenAIProvider (gpt-3.5-turbo) |        284         |       0.00057       |        11.39         |          24.94          |        5        |
+| OpenAIProvider (gpt-3.5-turbo) |        358         |       0.00072       |        15.77         |          22.71          |        5        |
+| OpenAIProvider (gpt-3.5-turbo) |        485         |       0.00097       |        23.84         |          20.34          |        5        |
+| OpenAIProvider (gpt-3.5-turbo) |        222         |       0.00044       |         3.87         |          57.37          |        5        |
+| OpenAIProvider (gpt-3.5-turbo) | Total Tokens: 2473 | Total Cost: 0.00495 | Median Latency: 4.00 | Aggregated speed: 26.40 | Total Score: 50 |
++--------------------------------+--------------------+---------------------+----------------------+-------------------------+-----------------+
++---------------------------------------+--------------------+---------------------+----------------------+--------------------------+-----------------+
+|                 Model                 |       Tokens       |       Cost ($)      |     Latency (s)      |    Speed (tokens/sec)    |    Evaluation   |
++---------------------------------------+--------------------+---------------------+----------------------+--------------------------+-----------------+
+| AnthropicProvider (claude-instant-v1) |         33         |       0.00010       |         0.85         |          38.63           |        1        |
+| AnthropicProvider (claude-instant-v1) |        152         |       0.00072       |         1.69         |          89.97           |        5        |
+| AnthropicProvider (claude-instant-v1) |         59         |       0.00024       |         0.70         |          84.55           |        5        |
+| AnthropicProvider (claude-instant-v1) |        112         |       0.00054       |         1.31         |          85.18           |        5        |
+| AnthropicProvider (claude-instant-v1) |        191         |       0.00082       |         1.54         |          124.30          |        0        |
+| AnthropicProvider (claude-instant-v1) |         65         |       0.00024       |         0.68         |          95.35           |        5        |
+| AnthropicProvider (claude-instant-v1) |        190         |       0.00082       |         1.54         |          123.19          |        5        |
+| AnthropicProvider (claude-instant-v1) |        276         |       0.00053       |         0.69         |          398.39          |        5        |
+| AnthropicProvider (claude-instant-v1) |        220         |       0.00085       |         1.52         |          144.87          |        5        |
+| AnthropicProvider (claude-instant-v1) |        189         |       0.00072       |         1.21         |          156.10          |        5        |
+| AnthropicProvider (claude-instant-v1) |        326         |       0.00145       |         2.65         |          122.87          |        0        |
+| AnthropicProvider (claude-instant-v1) |        281         |       0.00089       |         1.37         |          204.61          |        5        |
+| AnthropicProvider (claude-instant-v1) | Total Tokens: 2094 | Total Cost: 0.00791 | Median Latency: 1.34 | Aggregated speed: 132.82 | Total Score: 46 |
++---------------------------------------+--------------------+---------------------+----------------------+--------------------------+-----------------+
+
++-----------------------------------------+--------------------+---------------------+----------------------+-------------------------+-----------------+
+|                  Model                  |       Tokens       |       Cost ($)      |     Latency (s)      |    Speed (tokens/sec)   |    Evaluation   |
++-----------------------------------------+--------------------+---------------------+----------------------+-------------------------+-----------------+
+| CohereProvider (command-xlarge-nightly) |         27         |       0.00068       |         0.73         |          37.23          |        1        |
+| CohereProvider (command-xlarge-nightly) |         49         |       0.00122       |         1.04         |          47.03          |        5        |
+| CohereProvider (command-xlarge-nightly) |         31         |       0.00077       |         0.67         |          46.10          |        0        |
+| CohereProvider (command-xlarge-nightly) |         30         |       0.00075       |         0.73         |          41.35          |        0        |
+| CohereProvider (command-xlarge-nightly) |        128         |       0.00320       |         2.89         |          44.27          |        0        |
+| CohereProvider (command-xlarge-nightly) |         38         |       0.00095       |         0.70         |          54.29          |        4        |
+| CohereProvider (command-xlarge-nightly) |         57         |       0.00143       |         0.51         |          111.13         |        5        |
+| CohereProvider (command-xlarge-nightly) |        269         |       0.00673       |         0.98         |          274.23         |        3        |
+| CohereProvider (command-xlarge-nightly) |        230         |       0.00575       |         4.55         |          50.54          |        0        |
+| CohereProvider (command-xlarge-nightly) |        170         |       0.00425       |         2.45         |          69.41          |        0        |
+| CohereProvider (command-xlarge-nightly) |        1502        |       0.03755       |        30.80         |          48.77          |        0        |
+| CohereProvider (command-xlarge-nightly) |        218         |       0.00545       |         2.01         |          108.49         |        4        |
+| CohereProvider (command-xlarge-nightly) | Total Tokens: 2749 | Total Cost: 0.06872 | Median Latency: 1.01 | Aggregated speed: 57.20 | Total Score: 22 |
++-----------------------------------------+--------------------+---------------------+----------------------+-------------------------+-----------------+
 ```
 
 To evaluate models on your own prompts, simply pass a list of questions. The evaluator will automatically evaluate the responses:
 
 ```
 models.benchmark(prompts=["what is the capital of finland", "who won superbowl in the year justin bieber was born"], evaluator=gpt4)
 ```
 
 ## Supported Models
 
 To get a list of supported models, call list(). Models will be shown in the order of least expensive to most expensive.
 
 ```
 >>> model=llms.init()
->>> model.list()
 
-[{'provider': 'AnthropicProvider', 'name': 'claude-instant-v1', 'cost': {'prompt': 0.43, 'completion': 1.45}}, {'provider': 'OpenAIProvider', 'name': 'gpt-3.5-turbo', 'cost': {'prompt': 2.0, 'completion': 2.0}}, {'provider': 'AI21Provider', 'name': 'j2-large', 'cost': {'prompt': 3.0, 'completion': 3.0}}, {'provider': 'AnthropicProvider', 'name': 'claude-v1', 'cost': {'prompt': 2.9, 'completion': 8.6}}, {'provider': 'AI21Provider', 'name': 'j2-grande', 'cost': {'prompt': 10.0, 'completion': 10.0}}, {'provider': 'AI21Provider', 'name': 'j2-grande-instruct', 'cost': {'prompt': 10.0, 'completion': 10.0}}, {'provider': 'AI21Provider', 'name': 'j2-jumbo', 'cost': {'prompt': 15.0, 'completion': 15.0}}, {'provider': 'AI21Provider', 'name': 'j2-jumbo-instruct', 'cost': {'prompt': 15.0, 'completion': 15.0}}, {'provider': 'OpenAIProvider', 'name': 'gpt-4', 'cost': {'prompt': 30.0, 'completion': 60.0}}]
+>>> model.list()
 
 >>> model.list("gpt') # lists only models with 'gpt' in name/provider name
+
+| Provider            | Name                   | Prompt Cost | Completion Cost | Token Limit |
+|---------------------|------------------------|-------------|-----------------|-------------|
+| AI21Provider        | j2-grande-instruct     |        10.0 |            10.0 |        8192 |
+| AI21Provider        | j2-jumbo-instruct      |        15.0 |            15.0 |        8192 |
+| AlephAlphaProvider  | luminous-base          |         6.6 |             7.6 |        2048 |
+| AlephAlphaProvider  | luminous-extended      |         9.9 |            10.9 |        2048 |
+| AlephAlphaProvider  | luminous-supreme       |        38.5 |            42.5 |        2048 |
+| AlephAlphaProvider  | luminous-supreme-control |      48.5 |            53.6 |        2048 |
+| AnthropicProvider   | claude-instant-v1      |        1.63 |            5.51 |        9000 |
+| AnthropicProvider   | claude-v1              |       11.02 |           32.68 |        9000 |
+| CohereProvider      | command-xlarge-beta    |          25 |              25 |        8192 |
+| CohereProvider      | command-xlarge-nightly |          25 |              25 |        8192 |
+| OpenAIProvider      | gpt-3.5-turbo          |         2.0 |             2.0 |        4000 |
+| OpenAIProvider      | gpt-4                  |        30.0 |            60.0 |        8000 |
+
 ```
 
 Useful links:\
 [OpenAI documentation](https://platform.openai.com/docs/api-reference/completions)\
 [Anthropic documentation](https://console.anthropic.com/docs/api/reference#-v1-complete)\
 [AI21 documentation](https://docs.ai21.com/reference/j2-instruct-ref)
-
+[Cohere documentation](https://cohere-sdk.readthedocs.io/en/latest/cohere.html#api)
+[Aleph Alpha documentation](https://aleph-alpha-client.readthedocs.io/en/latest/aleph_alpha_client.html#aleph_alpha_client.CompletionRequest)
 
 ## License
 
 This project is licensed under the MIT License.
```

### Comparing `pyllms-0.1.8/README.md` & `pyllms-0.1.9/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 
 # PyLLMs
 
 [![](https://dcbadge.vercel.app/api/server/aDNg6E9szy?compact=true&style=flat)](https://discord.gg/aDNg6E9szy) [![Twitter](https://img.shields.io/twitter/follow/KagiHQ?style=social)](https://twitter.com/KagiHQ) [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/license/mit/) 
 
-PyLLMs is a minimal Python library to connect to LLMs (OpenAI, Anthropic, AI21), with a built-in model performance benchmark. 
+PyLLMs is a minimal Python library to connect to LLMs (OpenAI, Anthropic, AI21, Cohere, Aleph Alpha, HuggingfaceHub) with a built-in model performance benchmark. 
 
-It is ideal for fast prototyping and evaluationg different models thanks to:
-- Connect to top LLMs in few lines of code (currenly OpenAI, Anthropic and AI21 are supported)
+It is ideal for fast prototyping and evaluating different models thanks to:
+- Connect to top LLMs in s few lines of code (currently OpenAI, Anthropic and AI21 are supported)
 - Response meta includes tokens processed, cost and latency standardized across the models
-- Multi-model support: Get completitions from different models at the same time
-- LLM benchmark: Eevaluate models on quality, speed and cost
+- Multi-model support: Get completions from different models at the same time
+- LLM benchmark: Evaluate models on quality, speed and cost
 
 Feel free to reuse and expand. Pull requests are welcome.
 
 ## Installation
 
 Clone this repository and install the package using pip:
 
@@ -140,78 +140,106 @@
 ```
 models=llms.init(model=['gpt-3.5-turbo', 'claude-instant-v1', 'j2-jumbo-instruct'])
 gpt4=llms.init('gpt-4') # optional, evaluator can be ommited and in that case only speed and cost will be evaluated
 models.benchmark(evaluator=gpt4)
 ```
 
 ```
-+---------------------------------------+--------------------+---------------------+-----------------------+---------------------------+-----------------+
-|                 Model                 |       Tokens       |       Cost ($)      |      Latency (s)      |     Speed (tokens/sec)    |    Evaluation   |
-+---------------------------------------+--------------------+---------------------+-----------------------+---------------------------+-----------------+
-| AnthropicProvider (claude-instant-v1) |         33         |       0.00003       |          0.40         |           82.19           |        3        |
-| AnthropicProvider (claude-instant-v1) |        152         |       0.00019       |          1.65         |           91.89           |        10       |
-| AnthropicProvider (claude-instant-v1) |        248         |       0.00031       |          2.18         |           113.74          |        9        |
-| AnthropicProvider (claude-instant-v1) |        209         |       0.00021       |          1.86         |           112.11          |        10       |
-| AnthropicProvider (claude-instant-v1) |         59         |       0.00006       |          0.87         |           68.18           |        10       |
-| AnthropicProvider (claude-instant-v1) |        140         |       0.00018       |          1.46         |           96.10           |        10       |
-| AnthropicProvider (claude-instant-v1) |        245         |       0.00031       |          2.45         |           100.16          |        9        |
-| AnthropicProvider (claude-instant-v1) |        250         |       0.00031       |          2.29         |           109.35          |        9        |
-| AnthropicProvider (claude-instant-v1) |        248         |       0.00031       |          2.17         |           114.50          |        9        |
-| AnthropicProvider (claude-instant-v1) |        323         |       0.00034       |          1.95         |           165.57          |        8        |
-| AnthropicProvider (claude-instant-v1) |        172         |       0.00014       |          0.97         |           177.63          |        10       |
-| AnthropicProvider (claude-instant-v1) | Total Tokens: 2079 | Total Cost: 0.00240 |  Median Latency: 1.86 | Aggregrated speed: 113.98 | Total Score: 97 |
-|     OpenAIProvider (gpt-3.5-turbo)    |         37         |       0.00007       |          1.20         |           30.86           |        7        |
-|     OpenAIProvider (gpt-3.5-turbo)    |         93         |       0.00019       |          2.89         |           32.19           |        1        |
-|     OpenAIProvider (gpt-3.5-turbo)    |        451         |       0.00090       |         18.10         |           24.91           |        10       |
-|     OpenAIProvider (gpt-3.5-turbo)    |        204         |       0.00041       |          5.60         |           36.45           |        10       |
-|     OpenAIProvider (gpt-3.5-turbo)    |        366         |       0.00073       |         16.51         |           22.17           |        10       |
-|     OpenAIProvider (gpt-3.5-turbo)    |        109         |       0.00022       |          3.69         |           29.51           |        10       |
-|     OpenAIProvider (gpt-3.5-turbo)    |        316         |       0.00063       |         11.96         |           26.43           |        10       |
-|     OpenAIProvider (gpt-3.5-turbo)    |        294         |       0.00059       |         10.47         |           28.09           |        10       |
-|     OpenAIProvider (gpt-3.5-turbo)    |        275         |       0.00055       |         10.02         |           27.45           |        10       |
-|     OpenAIProvider (gpt-3.5-turbo)    |        501         |       0.00100       |         16.28         |           30.77           |        10       |
-|     OpenAIProvider (gpt-3.5-turbo)    |        180         |       0.00036       |          3.23         |           55.79           |        10       |
-|     OpenAIProvider (gpt-3.5-turbo)    | Total Tokens: 2826 | Total Cost: 0.00565 | Median Latency: 10.02 |  Aggregrated speed: 28.28 | Total Score: 98 |
-|    AI21Provider (j2-jumbo-instruct)   |         27         |       0.00040       |          0.95         |           28.31           |        3        |
-|    AI21Provider (j2-jumbo-instruct)   |        114         |       0.00171       |          3.10         |           36.81           |        1        |
-|    AI21Provider (j2-jumbo-instruct)   |        195         |       0.00293       |          5.62         |           34.73           |        10       |
-|    AI21Provider (j2-jumbo-instruct)   |        117         |       0.00176       |          2.08         |           56.12           |        10       |
-|    AI21Provider (j2-jumbo-instruct)   |        216         |       0.00324       |          6.12         |           35.27           |        7        |
-|    AI21Provider (j2-jumbo-instruct)   |         67         |       0.00101       |          2.01         |           33.39           |        10       |
-|    AI21Provider (j2-jumbo-instruct)   |        229         |       0.00344       |          6.14         |           37.27           |        10       |
-|    AI21Provider (j2-jumbo-instruct)   |        225         |       0.00337       |          6.21         |           36.26           |        5        |
-|    AI21Provider (j2-jumbo-instruct)   |        218         |       0.00327       |          5.90         |           36.95           |        1        |
-|    AI21Provider (j2-jumbo-instruct)   |        281         |       0.00421       |          6.25         |           44.97           |        1        |
-|    AI21Provider (j2-jumbo-instruct)   |        149         |       0.00224       |          1.56         |           95.81           |        10       |
-|    AI21Provider (j2-jumbo-instruct)   | Total Tokens: 1838 | Total Cost: 0.02757 |  Median Latency: 5.62 |  Aggregrated speed: 40.01 | Total Score: 68 |
-+---------------------------------------+--------------------+---------------------+-----------------------+---------------------------+-----------------+
++--------------------------------+--------------------+---------------------+----------------------+-------------------------+-----------------+
+|             Model              |       Tokens       |       Cost ($)      |     Latency (s)      |    Speed (tokens/sec)   |    Evaluation   |
++--------------------------------+--------------------+---------------------+----------------------+-------------------------+-----------------+
+| OpenAIProvider (gpt-3.5-turbo) |         37         |       0.00007       |         1.47         |          25.19          |        1        |
+| OpenAIProvider (gpt-3.5-turbo) |         93         |       0.00019       |         4.13         |          22.53          |        0        |
+| OpenAIProvider (gpt-3.5-turbo) |        360         |       0.00072       |        18.42         |          19.54          |        5        |
+| OpenAIProvider (gpt-3.5-turbo) |        143         |       0.00029       |         6.76         |          21.15          |        5        |
+| OpenAIProvider (gpt-3.5-turbo) |        112         |       0.00022       |         3.87         |          28.95          |        4        |
+| OpenAIProvider (gpt-3.5-turbo) |         47         |       0.00009       |         1.57         |          29.86          |        5        |
+| OpenAIProvider (gpt-3.5-turbo) |         78         |       0.00016       |         1.52         |          51.19          |        5        |
+| OpenAIProvider (gpt-3.5-turbo) |        254         |       0.00051       |         1.08         |          235.22         |        5        |
+| OpenAIProvider (gpt-3.5-turbo) |        284         |       0.00057       |        11.39         |          24.94          |        5        |
+| OpenAIProvider (gpt-3.5-turbo) |        358         |       0.00072       |        15.77         |          22.71          |        5        |
+| OpenAIProvider (gpt-3.5-turbo) |        485         |       0.00097       |        23.84         |          20.34          |        5        |
+| OpenAIProvider (gpt-3.5-turbo) |        222         |       0.00044       |         3.87         |          57.37          |        5        |
+| OpenAIProvider (gpt-3.5-turbo) | Total Tokens: 2473 | Total Cost: 0.00495 | Median Latency: 4.00 | Aggregated speed: 26.40 | Total Score: 50 |
++--------------------------------+--------------------+---------------------+----------------------+-------------------------+-----------------+
++---------------------------------------+--------------------+---------------------+----------------------+--------------------------+-----------------+
+|                 Model                 |       Tokens       |       Cost ($)      |     Latency (s)      |    Speed (tokens/sec)    |    Evaluation   |
++---------------------------------------+--------------------+---------------------+----------------------+--------------------------+-----------------+
+| AnthropicProvider (claude-instant-v1) |         33         |       0.00010       |         0.85         |          38.63           |        1        |
+| AnthropicProvider (claude-instant-v1) |        152         |       0.00072       |         1.69         |          89.97           |        5        |
+| AnthropicProvider (claude-instant-v1) |         59         |       0.00024       |         0.70         |          84.55           |        5        |
+| AnthropicProvider (claude-instant-v1) |        112         |       0.00054       |         1.31         |          85.18           |        5        |
+| AnthropicProvider (claude-instant-v1) |        191         |       0.00082       |         1.54         |          124.30          |        0        |
+| AnthropicProvider (claude-instant-v1) |         65         |       0.00024       |         0.68         |          95.35           |        5        |
+| AnthropicProvider (claude-instant-v1) |        190         |       0.00082       |         1.54         |          123.19          |        5        |
+| AnthropicProvider (claude-instant-v1) |        276         |       0.00053       |         0.69         |          398.39          |        5        |
+| AnthropicProvider (claude-instant-v1) |        220         |       0.00085       |         1.52         |          144.87          |        5        |
+| AnthropicProvider (claude-instant-v1) |        189         |       0.00072       |         1.21         |          156.10          |        5        |
+| AnthropicProvider (claude-instant-v1) |        326         |       0.00145       |         2.65         |          122.87          |        0        |
+| AnthropicProvider (claude-instant-v1) |        281         |       0.00089       |         1.37         |          204.61          |        5        |
+| AnthropicProvider (claude-instant-v1) | Total Tokens: 2094 | Total Cost: 0.00791 | Median Latency: 1.34 | Aggregated speed: 132.82 | Total Score: 46 |
++---------------------------------------+--------------------+---------------------+----------------------+--------------------------+-----------------+
+
++-----------------------------------------+--------------------+---------------------+----------------------+-------------------------+-----------------+
+|                  Model                  |       Tokens       |       Cost ($)      |     Latency (s)      |    Speed (tokens/sec)   |    Evaluation   |
++-----------------------------------------+--------------------+---------------------+----------------------+-------------------------+-----------------+
+| CohereProvider (command-xlarge-nightly) |         27         |       0.00068       |         0.73         |          37.23          |        1        |
+| CohereProvider (command-xlarge-nightly) |         49         |       0.00122       |         1.04         |          47.03          |        5        |
+| CohereProvider (command-xlarge-nightly) |         31         |       0.00077       |         0.67         |          46.10          |        0        |
+| CohereProvider (command-xlarge-nightly) |         30         |       0.00075       |         0.73         |          41.35          |        0        |
+| CohereProvider (command-xlarge-nightly) |        128         |       0.00320       |         2.89         |          44.27          |        0        |
+| CohereProvider (command-xlarge-nightly) |         38         |       0.00095       |         0.70         |          54.29          |        4        |
+| CohereProvider (command-xlarge-nightly) |         57         |       0.00143       |         0.51         |          111.13         |        5        |
+| CohereProvider (command-xlarge-nightly) |        269         |       0.00673       |         0.98         |          274.23         |        3        |
+| CohereProvider (command-xlarge-nightly) |        230         |       0.00575       |         4.55         |          50.54          |        0        |
+| CohereProvider (command-xlarge-nightly) |        170         |       0.00425       |         2.45         |          69.41          |        0        |
+| CohereProvider (command-xlarge-nightly) |        1502        |       0.03755       |        30.80         |          48.77          |        0        |
+| CohereProvider (command-xlarge-nightly) |        218         |       0.00545       |         2.01         |          108.49         |        4        |
+| CohereProvider (command-xlarge-nightly) | Total Tokens: 2749 | Total Cost: 0.06872 | Median Latency: 1.01 | Aggregated speed: 57.20 | Total Score: 22 |
++-----------------------------------------+--------------------+---------------------+----------------------+-------------------------+-----------------+
 ```
 
 To evaluate models on your own prompts, simply pass a list of questions. The evaluator will automatically evaluate the responses:
 
 ```
 models.benchmark(prompts=["what is the capital of finland", "who won superbowl in the year justin bieber was born"], evaluator=gpt4)
 ```
 
 ## Supported Models
 
 To get a list of supported models, call list(). Models will be shown in the order of least expensive to most expensive.
 
 ```
 >>> model=llms.init()
->>> model.list()
 
-[{'provider': 'AnthropicProvider', 'name': 'claude-instant-v1', 'cost': {'prompt': 0.43, 'completion': 1.45}}, {'provider': 'OpenAIProvider', 'name': 'gpt-3.5-turbo', 'cost': {'prompt': 2.0, 'completion': 2.0}}, {'provider': 'AI21Provider', 'name': 'j2-large', 'cost': {'prompt': 3.0, 'completion': 3.0}}, {'provider': 'AnthropicProvider', 'name': 'claude-v1', 'cost': {'prompt': 2.9, 'completion': 8.6}}, {'provider': 'AI21Provider', 'name': 'j2-grande', 'cost': {'prompt': 10.0, 'completion': 10.0}}, {'provider': 'AI21Provider', 'name': 'j2-grande-instruct', 'cost': {'prompt': 10.0, 'completion': 10.0}}, {'provider': 'AI21Provider', 'name': 'j2-jumbo', 'cost': {'prompt': 15.0, 'completion': 15.0}}, {'provider': 'AI21Provider', 'name': 'j2-jumbo-instruct', 'cost': {'prompt': 15.0, 'completion': 15.0}}, {'provider': 'OpenAIProvider', 'name': 'gpt-4', 'cost': {'prompt': 30.0, 'completion': 60.0}}]
+>>> model.list()
 
 >>> model.list("gpt') # lists only models with 'gpt' in name/provider name
+
+| Provider            | Name                   | Prompt Cost | Completion Cost | Token Limit |
+|---------------------|------------------------|-------------|-----------------|-------------|
+| AI21Provider        | j2-grande-instruct     |        10.0 |            10.0 |        8192 |
+| AI21Provider        | j2-jumbo-instruct      |        15.0 |            15.0 |        8192 |
+| AlephAlphaProvider  | luminous-base          |         6.6 |             7.6 |        2048 |
+| AlephAlphaProvider  | luminous-extended      |         9.9 |            10.9 |        2048 |
+| AlephAlphaProvider  | luminous-supreme       |        38.5 |            42.5 |        2048 |
+| AlephAlphaProvider  | luminous-supreme-control |      48.5 |            53.6 |        2048 |
+| AnthropicProvider   | claude-instant-v1      |        1.63 |            5.51 |        9000 |
+| AnthropicProvider   | claude-v1              |       11.02 |           32.68 |        9000 |
+| CohereProvider      | command-xlarge-beta    |          25 |              25 |        8192 |
+| CohereProvider      | command-xlarge-nightly |          25 |              25 |        8192 |
+| OpenAIProvider      | gpt-3.5-turbo          |         2.0 |             2.0 |        4000 |
+| OpenAIProvider      | gpt-4                  |        30.0 |            60.0 |        8000 |
+
 ```
 
 Useful links:\
 [OpenAI documentation](https://platform.openai.com/docs/api-reference/completions)\
 [Anthropic documentation](https://console.anthropic.com/docs/api/reference#-v1-complete)\
 [AI21 documentation](https://docs.ai21.com/reference/j2-instruct-ref)
-
+[Cohere documentation](https://cohere-sdk.readthedocs.io/en/latest/cohere.html#api)
+[Aleph Alpha documentation](https://aleph-alpha-client.readthedocs.io/en/latest/aleph_alpha_client.html#aleph_alpha_client.CompletionRequest)
 
 ## License
 
 This project is licensed under the MIT License.
```

### Comparing `pyllms-0.1.8/llms/llms.py` & `pyllms-0.1.9/llms/llms.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import os
-import markdown2
 import statistics
 from prettytable import PrettyTable
 from .providers import OpenAIProvider
 from .providers import AnthropicProvider
 from .providers import AI21Provider
+from .providers import CohereProvider
+from .providers import AlephAlphaProvider
+from .providers import HuggingfaceHubProvider
 import concurrent.futures
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from typing import List, Optional, Tuple
 
 
 class Result:
     def __init__(self, results):
@@ -17,40 +19,49 @@
     @property
     def text(self):
         if len(self._results) == 1:
             return self._results[0]["text"]
         return [result["text"] for result in self._results]
 
     @property
-    def html(self):
-        if len(self._results) == 1:
-            return markdown2.markdown(self._results[0]["text"])
-        return [markdown2.markdown(result["text"]) for result in self._results]
-
-    @property
     def meta(self):
         if len(self._results) == 1:
             return self._results[0]["meta"]
         return [result["meta"] for result in self._results]
 
 
 class LLMS:
     def __init__(
-        self, model=None, openai_api_key=None, anthropic_api_key=None, ai21_api_key=None
+        self,
+        model=None,
+        openai_api_key=None,
+        anthropic_api_key=None,
+        ai21_api_key=None,
+        cohere_api_key=None,
+        alephalpha_api_key=None,
+        huggingfacehub_api_key=None
     ):
-
         if openai_api_key is None:
             openai_api_key = os.getenv("OPENAI_API_KEY")
 
         if anthropic_api_key is None:
             anthropic_api_key = os.getenv("ANTHROPIC_API_KEY")
 
         if ai21_api_key is None:
             ai21_api_key = os.getenv("AI21_API_KEY")
 
+        if cohere_api_key is None:
+            cohere_api_key = os.getenv("COHERE_API_KEY")
+
+        if alephalpha_api_key is None:
+            alephalpha_api_key = os.getenv("ALEPHALPHA_API_KEY")
+
+        if huggingfacehub_api_key is None:
+            huggingfacehub_api_key = os.getenv("HUGGINFACEHUB_API_KEY")    
+
         if model is None:
             model = os.getenv("LLMS_DEFAULT_MODEL")
             if model is None:
                 model = ["gpt-3.5-turbo"]
             else:
                 model = [model]
         elif isinstance(model, str):
@@ -69,21 +80,48 @@
                 self._providers.append(
                     AnthropicProvider(api_key=anthropic_api_key, model=single_model)
                 )
             elif ai21_api_key is not None and single_model in AI21Provider.MODEL_INFO:
                 self._providers.append(
                     AI21Provider(api_key=ai21_api_key, model=single_model)
                 )
+            elif (
+                cohere_api_key is not None and single_model in CohereProvider.MODEL_INFO
+            ):
+                self._providers.append(
+                    CohereProvider(api_key=cohere_api_key, model=single_model)
+                )
+            elif (
+                alephalpha_api_key is not None
+                and single_model in AlephAlphaProvider.MODEL_INFO
+            ):
+                self._providers.append(
+                    AlephAlphaProvider(api_key=alephalpha_api_key, model=single_model)
+                )
+            elif (
+                huggingfacehub_api_key is not None
+                and single_model in HuggingfaceHubProvider.MODEL_INFO
+            ):
+                self._providers.append(
+                    HuggingfaceHubProvider(api_key=huggingfacehub_api_key, model=single_model)
+                )    
             else:
                 raise ValueError("Invalid API key and model combination", single_model)
 
     def list(self, query=None):
         model_info_list = []
 
-        all_providers = [OpenAIProvider, AI21Provider, AnthropicProvider]
+        all_providers = [
+            OpenAIProvider,
+            AI21Provider,
+            AnthropicProvider,
+            CohereProvider,
+            AlephAlphaProvider,
+            HuggingfaceHubProvider
+        ]
 
         for provider in all_providers:
             for model, cost in provider.MODEL_INFO.items():
                 if query and (
                     (query.lower() not in model.lower())
                     and (query.lower() not in provider.__name__.lower())
                 ):
@@ -97,97 +135,93 @@
 
         sorted_list = sorted(
             model_info_list, key=lambda x: x["cost"]["prompt"] + x["cost"]["completion"]
         )
         return sorted_list
 
     def count_tokens(self, content):
-
         results = []
         for provider in self._providers:
             results.append(provider.count_tokens(content))
-        if len(self._providers)>1 :
+        if len(self._providers) > 1:
             return results
         else:
             return results[0]
-        
-    def complete(self, prompt, history=None, system_message=None, **kwargs):
+
+    def complete(self, prompt, **kwargs):
         def _generate(provider):
-           
-            response = provider.complete(prompt, history, **kwargs)
-    
-            formatted_cost = format(response["meta"]["cost"], '.5f')
+            response = provider.complete(prompt, **kwargs)
+
+            formatted_cost = format(response["meta"]["cost"], ".5f")
             formatted_latency = round(response["meta"]["latency"], 2)
-            
+
             response["meta"]["cost"] = formatted_cost
             response["meta"]["latency"] = formatted_latency
 
             return {
                 "text": response["text"],
                 "meta": response["meta"],
                 "provider": provider,
             }
-     
+
         results = []
         with ThreadPoolExecutor() as executor:
             futures = {
                 executor.submit(_generate, provider): provider
                 for provider in self._providers
             }
             for future in as_completed(futures):
                 results.append(future.result())
 
         return Result(results)
 
-    async def acomplete(self,
-                        prompt: str,
-                        history: Optional[List[tuple]] = None,
-                        **kwargs,
-                        ):
+    async def acomplete(
+        self,
+        prompt: str,
+        history: Optional[List[tuple]] = None,
+        **kwargs,
+    ):
         if len(self._providers) > 1:
             raise NotImplementedError("acomplete not supported for multi-models yet.")
         provider = self._providers[0]
-        response = await provider.acomplete(prompt, history, **kwargs)
+        response = await provider.acomplete(prompt, **kwargs)
 
-        formatted_cost = format(response["meta"]["cost"], '.5f')
+        formatted_cost = format(response["meta"]["cost"], ".5f")
         formatted_latency = round(response["meta"]["latency"], 2)
 
         response["meta"]["cost"] = formatted_cost
         response["meta"]["latency"] = formatted_latency
 
-        return Result([{
-            "text": response["text"],
-            "meta": response["meta"],
-            "provider": provider,
-        }])
-
-    def complete_stream(self, prompt, history=None, system_message=None, **kwargs):
-                 
-        if len(self._providers)>1:
-            raise ValueError(
-                "Streaming is possible only with a single model"
-            )
-        if isinstance(self._providers[0], AI21Provider):
-            raise ValueError(
-                "Streaming is not yet supported with AI21 models"
-            )
-            
-        yield from self._providers[0].complete_stream(prompt, history, **kwargs)
+        return Result(
+            [
+                {
+                    "text": response["text"],
+                    "meta": response["meta"],
+                    "provider": provider,
+                }
+            ]
+        )
 
+    def complete_stream(self, prompt, **kwargs):
+        if len(self._providers) > 1:
+            raise ValueError("Streaming is possible only with a single model")
+        if isinstance(self._providers[0], AI21Provider) or isinstance(self._providers[0], AlephAlphaProvider) or isinstance(self._providers[0], HuggingfaceHubProvider):
+            raise ValueError("Streaming is not yet supported with this model")
+
+        yield from self._providers[0].complete_stream(prompt, **kwargs)
 
     def benchmark(self, prompts=None, evaluator=None, show_outputs=False, html=False):
         if not prompts:
             prompts = [
                 "What is the capital of the country where Christopher Columbus was born?",
                 "A glass door has ‘push’ written on it in mirror writing. Should you push or pull it and why?",
                 "Solve the quadratic equation: x^2 - 5x + 6 = 0",
                 "How much is 7! * 3! -1234.5 ?",
                 'translate this sentence by alternating words in gemran and french "it was a beautiful day that thursday and I want skiing outside. it started raining soon although they said it won\'t be until friday, so I went to the pool instead"',
                 "Convert December 21 · 1:00 – 1:50pm pacific to asia/taipei time",
-                "Explain the plot of Cinderella in a sentence where each word has to begin with the next letter in the alphabet from A to Z, without repeating any letters",
                 "In my kitchen there's a table with a cup with a ball inside. I moved the cup to my bed in my bedroom and turned the cup upside down. I grabbed the cup again and moved to the main room. Where's the ball now?",
                 'Capture the essence of this in exactly 7 words: "There’s much that divides us in Northern Ireland though one thing is guaranteed to bring us together: local phrases. Call it slang, call it colloquialisms, we all know only too well how important words are to where we’re from . . . and when it comes to the phrases that make us ‘us,’ we’ve got a lot to say. While you don’t need advance knowledge of the words to fit in, well, it helps. How else will you know where ‘foundered’ sits on the scale of warm to freezing? Or deciding whether that new car purchase is more ‘clinker’ than ‘beezer’? Or appreciating that ‘grand’ can mean exactly that or anything but? If the best way to get to know a nation is to understand their language, then surely tourists must be at times confused about what comes out of our mouths. Throughout the island of Ireland, we have utterly brilliant ways to verbally express ourselves.“I think it’s really important,” says Dr Frank Ferguson, research director for English Language and Literature at Ulster University, about the vitality of slang as part of language."',
                 "Write a Python function that takes a list of integers as input and returns the length of the longest increasing subsequence. An increasing subsequence is a subsequence of the given list where the elements are in strictly increasing order. Your function should have an efficient solution with a time complexity better than O(n^2), where n is the length of the input list. Output only code with no explainations and provide example usage.",
                 "Write a Python function that takes a list of integers as input and returns the maximum sum of non-adjacent elements in the list. The function should return 0 if the input list is empty. Your function should have an efficient solution with a time complexity of O(n), where n is the length of the input list. Output only code with no explainations and provide example usage.",
                 "You are given a 2D binary matrix filled with 0's and 1's. Your task is to write a JavaScript function that finds the largest rectangle containing only 1's and returns its area. Your function should have an efficient solution with a time complexity better than O(n^3), where n is the total number of elements in the input matrix. Output only code with no explainations and provide example usage.",
                 "Given the following messy and unstructured data, extract the names, email addresses, and phone numbers of the individuals listed:\
 John Doe - johndoe (at) email.com (five-five-five) one-two-three-four-five-six-seven\
@@ -222,29 +256,30 @@
 Since the word "push" is written in mirror writing, it suggests that the instruction is intended for people on the other side of the door. Therefore, you should pull the door to open it. You would score this 0 (it is wrong)
 
 
 Your only output should be a list of comma seperated integers representing your evaluation score for each answer. No other output is allowed. For example above your output will be:
 0, 1
 
 """
-            # prompt = "Please evaluate the following answers on a scale of 1 to 10 (10 being the best):\n\n"
+
             prompt = ""
             for i, (query, answer) in enumerate(query_answer_pairs):
                 prompt += f"Query #{i + 1}: {query}\nAnswer #{i + 1}: {answer}\n\n"
-            #            prompt += "Please provide a score for each answer as a list of integers separated by commas, with no additional text or explanation. For example: 6, 10, 10"
-            #print(prompt)
-            #print(evaluator_result)
+            # print(prompt)
+
+            evaluator_result = evaluator.complete(prompt, system_message=system).text
+            # print(evaluator_result)
             scores = evaluator_result.split(",")
             return [int(score.strip()) for score in scores]
 
         model_results = {}
 
         def process_prompt(model, prompt, index):
-            #print(model, index)
-            result = model.complete(prompt)
+            print(model, index)
+            result = model.complete(prompt, max_tokens=1000, temperature=0)
             output_data = {
                 "text": result["text"],
                 "tokens": result["meta"]["tokens"],
                 "latency": result["meta"]["latency"],
                 "cost": result["meta"]["cost"],
                 "prompt_index": index,
             }
@@ -335,47 +370,48 @@
         if not evaluator:
             headers.remove("Evaluation")
 
         table = PrettyTable(headers)
 
         for model in sorted_models:
             model_data = model_results[model]
+
             total_tokens = 0
             total_score = 0
             for index, output_data in enumerate(model_data["outputs"]):
                 total_tokens += output_data["tokens"]
                 if evaluator:
                     total_score += model_results[model]["evaluation"][index]
                 row_data = [
-                    model,
+                    str(model),
                     output_data["text"],
                     output_data["tokens"],
                     f'{output_data["cost"]:.5f}',
                     f'{output_data["latency"]:.2f}',
                     f'{output_data["tokens"]/output_data["latency"]:.2f}',
                 ]
                 if not show_outputs:
                     row_data.remove(output_data["text"])
                 if evaluator:
                     row_data.append(model_results[model]["evaluation"][index])
                 table.add_row(row_data)
 
             if show_outputs:
                 row_data = [
-                    model,
+                    str(model),
                     "",
                     f"Total Tokens: {total_tokens}",
                     f"Total Cost: {model_data['total_cost']:.5f}",
                     f"Median Latency: {model_data['median_latency']:.2f}",
                     f"Aggregated speed: {total_tokens/model_data['total_latency']:.2f}",
                 ]
 
             else:
                 row_data = [
-                    model,
+                    str(model),
                     f"Total Tokens: {total_tokens}",
                     f"Total Cost: {model_data['total_cost']:.5f}",
                     f"Median Latency: {model_data['median_latency']:.2f}",
                     f"Aggregated speed: {total_tokens/model_data['total_latency']:.2f}",
                 ]
             if evaluator:
                 row_data.append(f"Total Score: {total_score}")
```

### Comparing `pyllms-0.1.8/llms/providers/ai21.py` & `pyllms-0.1.9/llms/providers/ai21.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,49 +5,56 @@
 import itertools
 from typing import List, Optional
 
 
 class AI21Provider:
     # per million tokens
     MODEL_INFO = {
-        "j2-jumbo-instruct": {"prompt": 15.0, "completion": 15.0, "token_limit": 8192},
         "j2-grande-instruct": {"prompt": 10.0, "completion": 10.0, "token_limit": 8192},
+        "j2-jumbo-instruct": {"prompt": 15.0, "completion": 15.0, "token_limit": 8192},
     }
 
     def __init__(self, api_key, model=None):
         ai21.api_key = api_key
         if model is None:
-            model = "j2-grande-instruct"
+            model = list(MODEL_INFO.keys())[0]
         self.model = model
 
     def __str__(self):
         return f"{self.__class__.__name__} ({self.model})"
 
-    def complete(self,
-                 prompt: str,
-                 history: Optional[List[tuple]] = None,
-                 temperature: float = 0,
-                 max_tokens: int = 300,
-                 **kwargs):
+    def count_tokens(self, content: str):
+        return anthropic.count_tokens(content)
 
+    def complete(
+        self,
+        prompt: str,
+        history: Optional[List[tuple]] = None,
+        temperature: float = 0,
+        max_tokens: int = 300,
+        **kwargs,
+    ):
         HUMAN_PROMPT = "\n\nHuman:"
         AI_PROMPT = "\n\nAssistant:"
 
         if history is not None:
             role_cycle = itertools.cycle((HUMAN_PROMPT, AI_PROMPT))
             history_messages = itertools.chain.from_iterable(history)
-            history_prompt = "".join(itertools.chain.from_iterable(zip(role_cycle, history_messages)))
+            history_prompt = "".join(
+                itertools.chain.from_iterable(zip(role_cycle, history_messages))
+            )
             prompt = f"{history_prompt}{prompt}"
 
-
-        if 'maxTokens' not in kwargs:
-            kwargs['maxTokens'] = max_tokens  # Add maxTokens to kwargs if not present
+        if "maxTokens" not in kwargs:
+            kwargs["maxTokens"] = max_tokens  # Add maxTokens to kwargs if not present
 
         start_time = time.time()
-        response = ai21.Completion.execute(model=self.model, prompt=prompt, temperature=temperature, **kwargs)
+        response = ai21.Completion.execute(
+            model=self.model, prompt=prompt, temperature=temperature, **kwargs
+        )
         latency = time.time() - start_time
 
         completion = response.completions[0].data.text.strip()
         prompt_tokens = len(response.prompt.tokens)
         completion_tokens = len(response.completions[0].data.tokens)
         total_tokens = prompt_tokens + completion_tokens
```

### Comparing `pyllms-0.1.8/llms/providers/anthropic.py` & `pyllms-0.1.9/llms/providers/anthropic.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,49 +11,55 @@
 class AnthropicProvider:
     MODEL_INFO = {
         "claude-instant-v1": {"prompt": 1.63, "completion": 5.51, "token_limit": 9000},
         "claude-v1": {"prompt": 11.02, "completion": 32.68, "token_limit": 9000},
     }
 
     def __init__(self, api_key=None, model=None):
+        
+        if model is None:
+            model = list(MODEL_INFO.keys())[0]
+        self.model = model
+
         if api_key is None:
             api_key = os.getenv("ANTHROPIC_API_KEY")
         self.client = anthropic.Client(api_key)
 
-        if model is None:
-            model = "claude-instant-v1"
-        self.model = model
 
     def __str__(self):
         return f"{self.__class__.__name__} ({self.model})"
 
-    def count_tokens(self, content:str):
-        raise ValueError(
-                "Count tokens is currently not supported with AI21"
-            )
-
-    def complete(self,
-                 prompt: str,
-                 history: Optional[List[tuple]] = None,
-                 temperature: float = 0,
-                 max_tokens: int = 300,
-                 stop_sequences: Optional[List[str]] = None,
-                 ai_prompt: str = "",
-                 **kwargs
-                 ):
+    def count_tokens(self, content: str):
+        raise ValueError("Count tokens is currently not supported with AI21")
 
-        formatted_prompt = f"{anthropic.HUMAN_PROMPT}{prompt}{anthropic.AI_PROMPT}{ai_prompt}"
+    def complete(
+        self,
+        prompt: str,
+        history: Optional[List[tuple]] = None,
+        temperature: float = 0,
+        max_tokens: int = 300,
+        stop_sequences: Optional[List[str]] = None,
+        ai_prompt: str = "",
+        **kwargs,
+    ):
+        formatted_prompt = (
+            f"{anthropic.HUMAN_PROMPT}{prompt}{anthropic.AI_PROMPT}{ai_prompt}"
+        )
         if history is not None:
             role_cycle = itertools.cycle((anthropic.HUMAN_PROMPT, anthropic.AI_PROMPT))
             history_messages = itertools.chain.from_iterable(history)
-            history_prompt = "".join(itertools.chain.from_iterable(zip(role_cycle, history_messages)))
+            history_prompt = "".join(
+                itertools.chain.from_iterable(zip(role_cycle, history_messages))
+            )
             formatted_prompt = f"{history_prompt}{formatted_prompt}"
 
-        if 'max_tokens_to_sample' not in kwargs:
-            kwargs['max_tokens_to_sample'] = max_tokens  # Add maxTokens to kwargs if not present
+        if "max_tokens_to_sample" not in kwargs:
+            kwargs[
+                "max_tokens_to_sample"
+            ] = max_tokens  # Add maxTokens to kwargs if not present
 
         if stop_sequences is None:
             stop_sequences = [anthropic.HUMAN_PROMPT]
 
         start_time = time.time()
         response = self.client.completion(
             prompt=formatted_prompt,
@@ -83,33 +89,39 @@
                 "tokens_prompt": prompt_tokens,
                 "tokens_completion": completion_tokens,
                 "cost": cost,
                 "latency": latency,
             },
         }
 
-    async def acomplete(self,
-                        prompt: str,
-                        history: Optional[List[tuple]] = None,
-                        temperature: float = 0,
-                        max_tokens: int = 300,
-                        stop_sequences: Optional[List[str]] = None,
-                        ai_prompt: str = "",
-                        **kwargs
-                        ):
-
-        formatted_prompt = f"{anthropic.HUMAN_PROMPT}{prompt}{anthropic.AI_PROMPT}{ai_prompt}"
+    async def acomplete(
+        self,
+        prompt: str,
+        history: Optional[List[tuple]] = None,
+        temperature: float = 0,
+        max_tokens: int = 300,
+        stop_sequences: Optional[List[str]] = None,
+        ai_prompt: str = "",
+        **kwargs,
+    ):
+        formatted_prompt = (
+            f"{anthropic.HUMAN_PROMPT}{prompt}{anthropic.AI_PROMPT}{ai_prompt}"
+        )
         if history is not None:
             role_cycle = itertools.cycle((anthropic.HUMAN_PROMPT, anthropic.AI_PROMPT))
             history_messages = itertools.chain.from_iterable(history)
-            history_prompt = "".join(itertools.chain.from_iterable(zip(role_cycle, history_messages)))
+            history_prompt = "".join(
+                itertools.chain.from_iterable(zip(role_cycle, history_messages))
+            )
             formatted_prompt = f"{history_prompt}{formatted_prompt}"
 
-        if 'max_tokens_to_sample' not in kwargs:
-            kwargs['max_tokens_to_sample'] = max_tokens  # Add maxTokens to kwargs if not present
+        if "max_tokens_to_sample" not in kwargs:
+            kwargs[
+                "max_tokens_to_sample"
+            ] = max_tokens  # Add maxTokens to kwargs if not present
 
         if stop_sequences is None:
             stop_sequences = [anthropic.HUMAN_PROMPT]
 
         start_time = time.time()
         response = await self.client.acompletion(
             prompt=formatted_prompt,
@@ -139,45 +151,45 @@
                 "tokens_prompt": prompt_tokens,
                 "tokens_completion": completion_tokens,
                 "cost": cost,
                 "latency": latency,
             },
         }
 
-    def complete_stream(self,
-                 prompt: str,
-                 history: Optional[List[tuple]] = None,
-                 temperature: float = 0,
-                 max_tokens: int = 300,
-                 **kwargs
-                 ):
-
+    def complete_stream(
+        self,
+        prompt: str,
+        history: Optional[List[tuple]] = None,
+        temperature: float = 0,
+        max_tokens: int = 300,
+        **kwargs,
+    ):
         formatted_prompt = f"{anthropic.HUMAN_PROMPT}{prompt}{anthropic.AI_PROMPT}"
         if history is not None:
             role_cycle = itertools.cycle((anthropic.HUMAN_PROMPT, anthropic.AI_PROMPT))
             history_messages = itertools.chain.from_iterable(history)
-            history_prompt = "".join(itertools.chain.from_iterable(zip(role_cycle, history_messages)))
+            history_prompt = "".join(
+                itertools.chain.from_iterable(zip(role_cycle, history_messages))
+            )
             formatted_prompt = f"{history_prompt}{formatted_prompt}"
 
+        if "max_tokens_to_sample" not in kwargs:
+            kwargs[
+                "max_tokens_to_sample"
+            ] = max_tokens  # Add maxTokens to kwargs if not present
 
-        if 'max_tokens_to_sample' not in kwargs:
-            kwargs['max_tokens_to_sample'] = max_tokens  # Add maxTokens to kwargs if not present
-
-        if 'stream' not in kwargs:
-            kwargs['stream'] = True  # Add stream param if not present
+        if "stream" not in kwargs:
+            kwargs["stream"] = True  # Add stream param if not present
 
         response = self.client.completion_stream(
             prompt=formatted_prompt,
             stop_sequences=[anthropic.HUMAN_PROMPT],
             temperature=temperature,
             model=self.model,
             **kwargs,
         )
-    
+
         last_completion = ""
         for data in response:
-            new_chunk = data['completion'][len(last_completion):]
-            last_completion = data['completion']  
-            yield(new_chunk)
-
-       
-        
+            new_chunk = data["completion"][len(last_completion) :]
+            last_completion = data["completion"]
+            yield (new_chunk)
```

### Comparing `pyllms-0.1.8/llms/providers/openai.py` & `pyllms-0.1.9/llms/providers/openai.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,58 +4,61 @@
 import time
 from typing import List, Optional
 
 
 class OpenAIProvider:
     # cost is per million tokens
     MODEL_INFO = {
-        "gpt-4": {"prompt": 30.0, "completion": 60.0, "token_limit": 8000},
         "gpt-3.5-turbo": {"prompt": 2.0, "completion": 2.0, "token_limit": 4000},
+        "gpt-4": {"prompt": 30.0, "completion": 60.0, "token_limit": 8000},
     }
 
     def __init__(self, api_key, model=None):
         openai.api_key = api_key
         if model is None:
-            model = "gpt-3.5-turbo"
+            model = list(MODEL_INFO.keys())[0]
         self.model = model
 
     def __str__(self):
         return f"{self.__class__.__name__} ({self.model})"
 
-    def count_tokens(self, content:str):
-        enc=tiktoken.encoding_for_model(self.model)
+    def count_tokens(self, content: str):
+        enc = tiktoken.encoding_for_model(self.model)
         return len(enc.encode(content))
 
-    def complete(self,
-                 prompt: str,
-                 history: Optional[List[tuple]] = None,
-                 system_message: str = None,
-                 temperature: float = 0,
-                 **kwargs):
+    def complete(
+        self,
+        prompt: str,
+        history: Optional[List[tuple]] = None,
+        system_message: str = None,
+        temperature: float = 0,
+        **kwargs,
+    ):
         start_time = time.time()
 
         messages = [{"role": "user", "content": prompt}]
 
         if history:
-            role_cycle = itertools.cycle(('user', 'assistant'))
+            role_cycle = itertools.cycle(("user", "assistant"))
             history_messages = itertools.chain.from_iterable(history)
 
-            history = [{"role": role, "content": message}
-                       for role, message in zip(role_cycle, history_messages)
-                       if message is not None]
+            history = [
+                {"role": role, "content": message}
+                for role, message in zip(role_cycle, history_messages)
+                if message is not None
+            ]
             messages = [*history, *messages]
 
         if system_message:
-            messages = [{"role": "system", "content": system_message}, *messages] 
+            messages = [{"role": "system", "content": system_message}, *messages]
 
         response = openai.ChatCompletion.create(
             model=self.model, messages=messages, temperature=temperature, **kwargs
         )
 
-       
         latency = time.time() - start_time
         completion = response.choices[0].message.content.strip()
         usage = response.usage
         prompt_tokens = usage["prompt_tokens"]
         completion_tokens = usage["completion_tokens"]
         total_tokens = usage["total_tokens"]
 
@@ -72,36 +75,39 @@
                 "tokens_prompt": prompt_tokens,  # Add tokens_prompt to meta
                 "tokens_completion": completion_tokens,  # Add tokens_completion to meta
                 "cost": cost,
                 "latency": latency,
             },
         }
 
-    async def acomplete(self,
-                        prompt: str,
-                        history: Optional[List[tuple]] = None,
-                        system_message: str = None,
-                        temperature: float = 0,
-                        **kwargs
-                        ):
+    async def acomplete(
+        self,
+        prompt: str,
+        history: Optional[List[tuple]] = None,
+        system_message: str = None,
+        temperature: float = 0,
+        **kwargs,
+    ):
         start_time = time.time()
 
         messages = [{"role": "user", "content": prompt}]
 
         if history:
-            role_cycle = itertools.cycle(('user', 'assistant'))
+            role_cycle = itertools.cycle(("user", "assistant"))
             history_messages = itertools.chain.from_iterable(history)
 
-            history = [{"role": role, "content": message}
-                       for role, message in zip(role_cycle, history_messages)
-                       if message is not None]
+            history = [
+                {"role": role, "content": message}
+                for role, message in zip(role_cycle, history_messages)
+                if message is not None
+            ]
             messages = [*history, *messages]
 
         if system_message:
-            messages = [{"role": "system", "content": system_message}, *messages] 
+            messages = [{"role": "system", "content": system_message}, *messages]
 
         response = await openai.ChatCompletion.acreate(
             model=self.model, messages=messages, temperature=temperature, **kwargs
         )
 
         latency = time.time() - start_time
         completion = response.choices[0].message.content.strip()
@@ -123,38 +129,41 @@
                 "tokens_prompt": prompt_tokens,  # Add tokens_prompt to meta
                 "tokens_completion": completion_tokens,  # Add tokens_completion to meta
                 "cost": cost,
                 "latency": latency,
             },
         }
 
-    def complete_stream(self,
-                 prompt: str,
-                 history: Optional[List[tuple]] = None,
-                 system_message: str = None,
-                 temperature: float = 0,
-                 **kwargs):
-
+    def complete_stream(
+        self,
+        prompt: str,
+        history: Optional[List[tuple]] = None,
+        system_message: str = None,
+        temperature: float = 0,
+        **kwargs,
+    ):
         messages = [{"role": "user", "content": prompt}]
 
         if history:
-            role_cycle = itertools.cycle(('user', 'assistant'))
+            role_cycle = itertools.cycle(("user", "assistant"))
             history_messages = itertools.chain.from_iterable(history)
 
-            history = [{"role": role, "content": message}
-                       for role, message in zip(role_cycle, history_messages)
-                       if message is not None]
+            history = [
+                {"role": role, "content": message}
+                for role, message in zip(role_cycle, history_messages)
+                if message is not None
+            ]
             messages = [*history, *messages]
 
         if system_message:
-            messages = [{"role": "system", "content": system_message}, *messages] 
+            messages = [{"role": "system", "content": system_message}, *messages]
 
-        if 'stream' not in kwargs:
-            kwargs['stream'] = True  # Add stream param if not present
+        if "stream" not in kwargs:
+            kwargs["stream"] = True  # Add stream param if not present
 
         response = openai.ChatCompletion.create(
             model=self.model, messages=messages, temperature=temperature, **kwargs
         )
 
-        yield from (chunk["choices"][0].get("delta", {}).get("content") for chunk in response)
-       
-
+        yield from (
+            chunk["choices"][0].get("delta", {}).get("content") for chunk in response
+        )
```

### Comparing `pyllms-0.1.8/pyllms.egg-info/PKG-INFO` & `pyllms-0.1.9/pyllms.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pyllms
-Version: 0.1.8
-Summary: Minimal Python library to connect to LLMs (OpenAI, Anthropic, AI21), with a built-in model performance benchmark.
+Version: 0.1.9
+Summary: Minimal Python library to connect to LLMs (OpenAI, Anthropic, AI21, Cohere, Aleph-Alpha, HuggingfaceHub), with a built-in model performance benchmark.
 Author: Vladimir Prelovac
 Author-email: vlad@kagi.com
 Project-URL: Documentation, https://github.com/kagisearch/pyllms
 Project-URL: Source Code, https://github.com/kagisearch/pyllms
 Project-URL: Issue Tracker, https://github.com/kagisearch/pyllms/issues
-Keywords: llm,llms,large language model,AI,NLP,natural language processing,gpt,chatgpt,openai,anthropic,ai21
+Keywords: llm,llms,large language model,AI,NLP,natural language processing,gpt,chatgpt,openai,anthropic,ai21,cohere,aleph alpha,huggingface hub
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -25,21 +25,21 @@
 License-File: LICENSE
 
 
 # PyLLMs
 
 [![](https://dcbadge.vercel.app/api/server/aDNg6E9szy?compact=true&style=flat)](https://discord.gg/aDNg6E9szy) [![Twitter](https://img.shields.io/twitter/follow/KagiHQ?style=social)](https://twitter.com/KagiHQ) [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/license/mit/) 
 
-PyLLMs is a minimal Python library to connect to LLMs (OpenAI, Anthropic, AI21), with a built-in model performance benchmark. 
+PyLLMs is a minimal Python library to connect to LLMs (OpenAI, Anthropic, AI21, Cohere, Aleph Alpha, HuggingfaceHub) with a built-in model performance benchmark. 
 
-It is ideal for fast prototyping and evaluationg different models thanks to:
-- Connect to top LLMs in few lines of code (currenly OpenAI, Anthropic and AI21 are supported)
+It is ideal for fast prototyping and evaluating different models thanks to:
+- Connect to top LLMs in s few lines of code (currently OpenAI, Anthropic and AI21 are supported)
 - Response meta includes tokens processed, cost and latency standardized across the models
-- Multi-model support: Get completitions from different models at the same time
-- LLM benchmark: Eevaluate models on quality, speed and cost
+- Multi-model support: Get completions from different models at the same time
+- LLM benchmark: Evaluate models on quality, speed and cost
 
 Feel free to reuse and expand. Pull requests are welcome.
 
 ## Installation
 
 Clone this repository and install the package using pip:
 
@@ -166,78 +166,106 @@
 ```
 models=llms.init(model=['gpt-3.5-turbo', 'claude-instant-v1', 'j2-jumbo-instruct'])
 gpt4=llms.init('gpt-4') # optional, evaluator can be ommited and in that case only speed and cost will be evaluated
 models.benchmark(evaluator=gpt4)
 ```
 
 ```
-+---------------------------------------+--------------------+---------------------+-----------------------+---------------------------+-----------------+
-|                 Model                 |       Tokens       |       Cost ($)      |      Latency (s)      |     Speed (tokens/sec)    |    Evaluation   |
-+---------------------------------------+--------------------+---------------------+-----------------------+---------------------------+-----------------+
-| AnthropicProvider (claude-instant-v1) |         33         |       0.00003       |          0.40         |           82.19           |        3        |
-| AnthropicProvider (claude-instant-v1) |        152         |       0.00019       |          1.65         |           91.89           |        10       |
-| AnthropicProvider (claude-instant-v1) |        248         |       0.00031       |          2.18         |           113.74          |        9        |
-| AnthropicProvider (claude-instant-v1) |        209         |       0.00021       |          1.86         |           112.11          |        10       |
-| AnthropicProvider (claude-instant-v1) |         59         |       0.00006       |          0.87         |           68.18           |        10       |
-| AnthropicProvider (claude-instant-v1) |        140         |       0.00018       |          1.46         |           96.10           |        10       |
-| AnthropicProvider (claude-instant-v1) |        245         |       0.00031       |          2.45         |           100.16          |        9        |
-| AnthropicProvider (claude-instant-v1) |        250         |       0.00031       |          2.29         |           109.35          |        9        |
-| AnthropicProvider (claude-instant-v1) |        248         |       0.00031       |          2.17         |           114.50          |        9        |
-| AnthropicProvider (claude-instant-v1) |        323         |       0.00034       |          1.95         |           165.57          |        8        |
-| AnthropicProvider (claude-instant-v1) |        172         |       0.00014       |          0.97         |           177.63          |        10       |
-| AnthropicProvider (claude-instant-v1) | Total Tokens: 2079 | Total Cost: 0.00240 |  Median Latency: 1.86 | Aggregrated speed: 113.98 | Total Score: 97 |
-|     OpenAIProvider (gpt-3.5-turbo)    |         37         |       0.00007       |          1.20         |           30.86           |        7        |
-|     OpenAIProvider (gpt-3.5-turbo)    |         93         |       0.00019       |          2.89         |           32.19           |        1        |
-|     OpenAIProvider (gpt-3.5-turbo)    |        451         |       0.00090       |         18.10         |           24.91           |        10       |
-|     OpenAIProvider (gpt-3.5-turbo)    |        204         |       0.00041       |          5.60         |           36.45           |        10       |
-|     OpenAIProvider (gpt-3.5-turbo)    |        366         |       0.00073       |         16.51         |           22.17           |        10       |
-|     OpenAIProvider (gpt-3.5-turbo)    |        109         |       0.00022       |          3.69         |           29.51           |        10       |
-|     OpenAIProvider (gpt-3.5-turbo)    |        316         |       0.00063       |         11.96         |           26.43           |        10       |
-|     OpenAIProvider (gpt-3.5-turbo)    |        294         |       0.00059       |         10.47         |           28.09           |        10       |
-|     OpenAIProvider (gpt-3.5-turbo)    |        275         |       0.00055       |         10.02         |           27.45           |        10       |
-|     OpenAIProvider (gpt-3.5-turbo)    |        501         |       0.00100       |         16.28         |           30.77           |        10       |
-|     OpenAIProvider (gpt-3.5-turbo)    |        180         |       0.00036       |          3.23         |           55.79           |        10       |
-|     OpenAIProvider (gpt-3.5-turbo)    | Total Tokens: 2826 | Total Cost: 0.00565 | Median Latency: 10.02 |  Aggregrated speed: 28.28 | Total Score: 98 |
-|    AI21Provider (j2-jumbo-instruct)   |         27         |       0.00040       |          0.95         |           28.31           |        3        |
-|    AI21Provider (j2-jumbo-instruct)   |        114         |       0.00171       |          3.10         |           36.81           |        1        |
-|    AI21Provider (j2-jumbo-instruct)   |        195         |       0.00293       |          5.62         |           34.73           |        10       |
-|    AI21Provider (j2-jumbo-instruct)   |        117         |       0.00176       |          2.08         |           56.12           |        10       |
-|    AI21Provider (j2-jumbo-instruct)   |        216         |       0.00324       |          6.12         |           35.27           |        7        |
-|    AI21Provider (j2-jumbo-instruct)   |         67         |       0.00101       |          2.01         |           33.39           |        10       |
-|    AI21Provider (j2-jumbo-instruct)   |        229         |       0.00344       |          6.14         |           37.27           |        10       |
-|    AI21Provider (j2-jumbo-instruct)   |        225         |       0.00337       |          6.21         |           36.26           |        5        |
-|    AI21Provider (j2-jumbo-instruct)   |        218         |       0.00327       |          5.90         |           36.95           |        1        |
-|    AI21Provider (j2-jumbo-instruct)   |        281         |       0.00421       |          6.25         |           44.97           |        1        |
-|    AI21Provider (j2-jumbo-instruct)   |        149         |       0.00224       |          1.56         |           95.81           |        10       |
-|    AI21Provider (j2-jumbo-instruct)   | Total Tokens: 1838 | Total Cost: 0.02757 |  Median Latency: 5.62 |  Aggregrated speed: 40.01 | Total Score: 68 |
-+---------------------------------------+--------------------+---------------------+-----------------------+---------------------------+-----------------+
++--------------------------------+--------------------+---------------------+----------------------+-------------------------+-----------------+
+|             Model              |       Tokens       |       Cost ($)      |     Latency (s)      |    Speed (tokens/sec)   |    Evaluation   |
++--------------------------------+--------------------+---------------------+----------------------+-------------------------+-----------------+
+| OpenAIProvider (gpt-3.5-turbo) |         37         |       0.00007       |         1.47         |          25.19          |        1        |
+| OpenAIProvider (gpt-3.5-turbo) |         93         |       0.00019       |         4.13         |          22.53          |        0        |
+| OpenAIProvider (gpt-3.5-turbo) |        360         |       0.00072       |        18.42         |          19.54          |        5        |
+| OpenAIProvider (gpt-3.5-turbo) |        143         |       0.00029       |         6.76         |          21.15          |        5        |
+| OpenAIProvider (gpt-3.5-turbo) |        112         |       0.00022       |         3.87         |          28.95          |        4        |
+| OpenAIProvider (gpt-3.5-turbo) |         47         |       0.00009       |         1.57         |          29.86          |        5        |
+| OpenAIProvider (gpt-3.5-turbo) |         78         |       0.00016       |         1.52         |          51.19          |        5        |
+| OpenAIProvider (gpt-3.5-turbo) |        254         |       0.00051       |         1.08         |          235.22         |        5        |
+| OpenAIProvider (gpt-3.5-turbo) |        284         |       0.00057       |        11.39         |          24.94          |        5        |
+| OpenAIProvider (gpt-3.5-turbo) |        358         |       0.00072       |        15.77         |          22.71          |        5        |
+| OpenAIProvider (gpt-3.5-turbo) |        485         |       0.00097       |        23.84         |          20.34          |        5        |
+| OpenAIProvider (gpt-3.5-turbo) |        222         |       0.00044       |         3.87         |          57.37          |        5        |
+| OpenAIProvider (gpt-3.5-turbo) | Total Tokens: 2473 | Total Cost: 0.00495 | Median Latency: 4.00 | Aggregated speed: 26.40 | Total Score: 50 |
++--------------------------------+--------------------+---------------------+----------------------+-------------------------+-----------------+
++---------------------------------------+--------------------+---------------------+----------------------+--------------------------+-----------------+
+|                 Model                 |       Tokens       |       Cost ($)      |     Latency (s)      |    Speed (tokens/sec)    |    Evaluation   |
++---------------------------------------+--------------------+---------------------+----------------------+--------------------------+-----------------+
+| AnthropicProvider (claude-instant-v1) |         33         |       0.00010       |         0.85         |          38.63           |        1        |
+| AnthropicProvider (claude-instant-v1) |        152         |       0.00072       |         1.69         |          89.97           |        5        |
+| AnthropicProvider (claude-instant-v1) |         59         |       0.00024       |         0.70         |          84.55           |        5        |
+| AnthropicProvider (claude-instant-v1) |        112         |       0.00054       |         1.31         |          85.18           |        5        |
+| AnthropicProvider (claude-instant-v1) |        191         |       0.00082       |         1.54         |          124.30          |        0        |
+| AnthropicProvider (claude-instant-v1) |         65         |       0.00024       |         0.68         |          95.35           |        5        |
+| AnthropicProvider (claude-instant-v1) |        190         |       0.00082       |         1.54         |          123.19          |        5        |
+| AnthropicProvider (claude-instant-v1) |        276         |       0.00053       |         0.69         |          398.39          |        5        |
+| AnthropicProvider (claude-instant-v1) |        220         |       0.00085       |         1.52         |          144.87          |        5        |
+| AnthropicProvider (claude-instant-v1) |        189         |       0.00072       |         1.21         |          156.10          |        5        |
+| AnthropicProvider (claude-instant-v1) |        326         |       0.00145       |         2.65         |          122.87          |        0        |
+| AnthropicProvider (claude-instant-v1) |        281         |       0.00089       |         1.37         |          204.61          |        5        |
+| AnthropicProvider (claude-instant-v1) | Total Tokens: 2094 | Total Cost: 0.00791 | Median Latency: 1.34 | Aggregated speed: 132.82 | Total Score: 46 |
++---------------------------------------+--------------------+---------------------+----------------------+--------------------------+-----------------+
+
++-----------------------------------------+--------------------+---------------------+----------------------+-------------------------+-----------------+
+|                  Model                  |       Tokens       |       Cost ($)      |     Latency (s)      |    Speed (tokens/sec)   |    Evaluation   |
++-----------------------------------------+--------------------+---------------------+----------------------+-------------------------+-----------------+
+| CohereProvider (command-xlarge-nightly) |         27         |       0.00068       |         0.73         |          37.23          |        1        |
+| CohereProvider (command-xlarge-nightly) |         49         |       0.00122       |         1.04         |          47.03          |        5        |
+| CohereProvider (command-xlarge-nightly) |         31         |       0.00077       |         0.67         |          46.10          |        0        |
+| CohereProvider (command-xlarge-nightly) |         30         |       0.00075       |         0.73         |          41.35          |        0        |
+| CohereProvider (command-xlarge-nightly) |        128         |       0.00320       |         2.89         |          44.27          |        0        |
+| CohereProvider (command-xlarge-nightly) |         38         |       0.00095       |         0.70         |          54.29          |        4        |
+| CohereProvider (command-xlarge-nightly) |         57         |       0.00143       |         0.51         |          111.13         |        5        |
+| CohereProvider (command-xlarge-nightly) |        269         |       0.00673       |         0.98         |          274.23         |        3        |
+| CohereProvider (command-xlarge-nightly) |        230         |       0.00575       |         4.55         |          50.54          |        0        |
+| CohereProvider (command-xlarge-nightly) |        170         |       0.00425       |         2.45         |          69.41          |        0        |
+| CohereProvider (command-xlarge-nightly) |        1502        |       0.03755       |        30.80         |          48.77          |        0        |
+| CohereProvider (command-xlarge-nightly) |        218         |       0.00545       |         2.01         |          108.49         |        4        |
+| CohereProvider (command-xlarge-nightly) | Total Tokens: 2749 | Total Cost: 0.06872 | Median Latency: 1.01 | Aggregated speed: 57.20 | Total Score: 22 |
++-----------------------------------------+--------------------+---------------------+----------------------+-------------------------+-----------------+
 ```
 
 To evaluate models on your own prompts, simply pass a list of questions. The evaluator will automatically evaluate the responses:
 
 ```
 models.benchmark(prompts=["what is the capital of finland", "who won superbowl in the year justin bieber was born"], evaluator=gpt4)
 ```
 
 ## Supported Models
 
 To get a list of supported models, call list(). Models will be shown in the order of least expensive to most expensive.
 
 ```
 >>> model=llms.init()
->>> model.list()
 
-[{'provider': 'AnthropicProvider', 'name': 'claude-instant-v1', 'cost': {'prompt': 0.43, 'completion': 1.45}}, {'provider': 'OpenAIProvider', 'name': 'gpt-3.5-turbo', 'cost': {'prompt': 2.0, 'completion': 2.0}}, {'provider': 'AI21Provider', 'name': 'j2-large', 'cost': {'prompt': 3.0, 'completion': 3.0}}, {'provider': 'AnthropicProvider', 'name': 'claude-v1', 'cost': {'prompt': 2.9, 'completion': 8.6}}, {'provider': 'AI21Provider', 'name': 'j2-grande', 'cost': {'prompt': 10.0, 'completion': 10.0}}, {'provider': 'AI21Provider', 'name': 'j2-grande-instruct', 'cost': {'prompt': 10.0, 'completion': 10.0}}, {'provider': 'AI21Provider', 'name': 'j2-jumbo', 'cost': {'prompt': 15.0, 'completion': 15.0}}, {'provider': 'AI21Provider', 'name': 'j2-jumbo-instruct', 'cost': {'prompt': 15.0, 'completion': 15.0}}, {'provider': 'OpenAIProvider', 'name': 'gpt-4', 'cost': {'prompt': 30.0, 'completion': 60.0}}]
+>>> model.list()
 
 >>> model.list("gpt') # lists only models with 'gpt' in name/provider name
+
+| Provider            | Name                   | Prompt Cost | Completion Cost | Token Limit |
+|---------------------|------------------------|-------------|-----------------|-------------|
+| AI21Provider        | j2-grande-instruct     |        10.0 |            10.0 |        8192 |
+| AI21Provider        | j2-jumbo-instruct      |        15.0 |            15.0 |        8192 |
+| AlephAlphaProvider  | luminous-base          |         6.6 |             7.6 |        2048 |
+| AlephAlphaProvider  | luminous-extended      |         9.9 |            10.9 |        2048 |
+| AlephAlphaProvider  | luminous-supreme       |        38.5 |            42.5 |        2048 |
+| AlephAlphaProvider  | luminous-supreme-control |      48.5 |            53.6 |        2048 |
+| AnthropicProvider   | claude-instant-v1      |        1.63 |            5.51 |        9000 |
+| AnthropicProvider   | claude-v1              |       11.02 |           32.68 |        9000 |
+| CohereProvider      | command-xlarge-beta    |          25 |              25 |        8192 |
+| CohereProvider      | command-xlarge-nightly |          25 |              25 |        8192 |
+| OpenAIProvider      | gpt-3.5-turbo          |         2.0 |             2.0 |        4000 |
+| OpenAIProvider      | gpt-4                  |        30.0 |            60.0 |        8000 |
+
 ```
 
 Useful links:\
 [OpenAI documentation](https://platform.openai.com/docs/api-reference/completions)\
 [Anthropic documentation](https://console.anthropic.com/docs/api/reference#-v1-complete)\
 [AI21 documentation](https://docs.ai21.com/reference/j2-instruct-ref)
-
+[Cohere documentation](https://cohere-sdk.readthedocs.io/en/latest/cohere.html#api)
+[Aleph Alpha documentation](https://aleph-alpha-client.readthedocs.io/en/latest/aleph_alpha_client.html#aleph_alpha_client.CompletionRequest)
 
 ## License
 
 This project is licensed under the MIT License.
```

### Comparing `pyllms-0.1.8/setup.py` & `pyllms-0.1.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,28 +5,29 @@
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 _project_homepage = "https://github.com/kagisearch/pyllms"
 
 setup(
     name="pyllms",
-    version="0.1.8",
-    description="Minimal Python library to connect to LLMs (OpenAI, Anthropic, AI21), with a built-in model performance benchmark.",
+    version="0.1.9",
+    description="Minimal Python library to connect to LLMs (OpenAI, Anthropic, AI21, Cohere, Aleph-Alpha, HuggingfaceHub), with a built-in model performance benchmark.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Vladimir Prelovac",
     author_email="vlad@kagi.com",
     packages=find_packages(),
     install_requires=[
         "openai",
         "tiktoken",
         "anthropic",
         "ai21",
+        "cohere",
+        "aleph-alpha-client",
         "huggingface_hub",
-        "markdown2",
         "prettytable",
     ],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
@@ -36,14 +37,14 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Topic :: Scientific/Engineering :: Human Machine Interfaces",
         "Topic :: Text Processing",
     ],
     python_requires=">=3.7",
-    keywords="llm, llms, large language model, AI, NLP, natural language processing, gpt, chatgpt, openai, anthropic, ai21",
+    keywords="llm, llms, large language model, AI, NLP, natural language processing, gpt, chatgpt, openai, anthropic, ai21, cohere, aleph alpha, huggingface hub",
     project_urls={
         "Documentation": _project_homepage,
         "Source Code": _project_homepage,
         "Issue Tracker": _project_homepage+"/issues",
     },
 )
```

