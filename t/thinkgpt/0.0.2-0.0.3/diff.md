# Comparing `tmp/thinkgpt-0.0.2.tar.gz` & `tmp/thinkgpt-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thinkgpt-0.0.2.tar", max compression
+gzip compressed data, was "thinkgpt-0.0.3.tar", max compression
```

## Comparing `thinkgpt-0.0.2.tar` & `thinkgpt-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2023-04-14 15:21:33.490604 thinkgpt-0.0.2/LICENSE
--rw-r--r--   0        0        0     6871 2023-04-20 23:12:15.079797 thinkgpt-0.0.2/README.md
--rw-r--r--   0        0        0      562 2023-04-21 01:19:20.920060 thinkgpt-0.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-14 15:28:05.934649 thinkgpt-0.0.2/thinkgpt/__init__.py
--rw-r--r--   0        0        0     4157 2023-04-16 20:58:23.227617 thinkgpt-0.0.2/thinkgpt/abstract.py
--rw-r--r--   0        0        0     2223 2023-04-15 22:14:39.262945 thinkgpt-0.0.2/thinkgpt/condition.py
--rw-r--r--   0        0        0     3061 2023-04-20 23:52:42.818016 thinkgpt-0.0.2/thinkgpt/gpt_select.py
--rw-r--r--   0        0        0     1165 2023-04-16 03:45:24.127522 thinkgpt-0.0.2/thinkgpt/helper.py
--rw-r--r--   0        0        0     2812 2023-04-16 20:58:23.231671 thinkgpt-0.0.2/thinkgpt/infer.py
--rw-r--r--   0        0        0     4410 2023-04-21 00:39:21.276973 thinkgpt-0.0.2/thinkgpt/llm.py
--rw-r--r--   0        0        0     2509 2023-04-21 00:50:43.413297 thinkgpt-0.0.2/thinkgpt/memory.py
--rw-r--r--   0        0        0     1854 2023-04-15 15:38:08.801502 thinkgpt-0.0.2/thinkgpt/refine.py
--rw-r--r--   0        0        0     3314 2023-04-21 00:43:56.674582 thinkgpt-0.0.2/thinkgpt/summarize.py
--rw-r--r--   0        0        0     7772 1970-01-01 00:00:00.000000 thinkgpt-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-14 15:21:33.490604 thinkgpt-0.0.3/LICENSE
+-rw-r--r--   0        0        0     6871 2023-04-20 23:12:15.079797 thinkgpt-0.0.3/README.md
+-rw-r--r--   0        0        0      562 2023-04-23 02:11:49.925649 thinkgpt-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-14 15:28:05.934649 thinkgpt-0.0.3/thinkgpt/__init__.py
+-rw-r--r--   0        0        0     4157 2023-04-16 20:58:23.227617 thinkgpt-0.0.3/thinkgpt/abstract.py
+-rw-r--r--   0        0        0     2223 2023-04-15 22:14:39.262945 thinkgpt-0.0.3/thinkgpt/condition.py
+-rw-r--r--   0        0        0     3061 2023-04-20 23:52:42.818016 thinkgpt-0.0.3/thinkgpt/gpt_select.py
+-rw-r--r--   0        0        0     1165 2023-04-16 03:45:24.127522 thinkgpt-0.0.3/thinkgpt/helper.py
+-rw-r--r--   0        0        0     2812 2023-04-16 20:58:23.231671 thinkgpt-0.0.3/thinkgpt/infer.py
+-rw-r--r--   0        0        0     4410 2023-04-21 00:39:21.276973 thinkgpt-0.0.3/thinkgpt/llm.py
+-rw-r--r--   0        0        0     2509 2023-04-21 00:50:43.413297 thinkgpt-0.0.3/thinkgpt/memory.py
+-rw-r--r--   0        0        0     1854 2023-04-15 15:38:08.801502 thinkgpt-0.0.3/thinkgpt/refine.py
+-rw-r--r--   0        0        0     3037 2023-04-23 02:20:34.442965 thinkgpt-0.0.3/thinkgpt/summarize.py
+-rw-r--r--   0        0        0     7772 1970-01-01 00:00:00.000000 thinkgpt-0.0.3/PKG-INFO
```

### Comparing `thinkgpt-0.0.2/LICENSE` & `thinkgpt-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `thinkgpt-0.0.2/README.md` & `thinkgpt-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `thinkgpt-0.0.2/pyproject.toml` & `thinkgpt-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "thinkgpt"
-version = "0.0.2"
+version = "0.0.3"
 description = "ThinkGPT is a Python library aimed at implementing Chain of Thoughts for Large Language Models (LLMs), prompting the model to think, reason, and to create generative agents."
 authors = ["Alaeddine Abdessalem <alaeddine-13@live.fr>"]
 license = "Apache 2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.7,<4.0"
```

### Comparing `thinkgpt-0.0.2/thinkgpt/abstract.py` & `thinkgpt-0.0.3/thinkgpt/abstract.py`

 * *Files identical despite different names*

### Comparing `thinkgpt-0.0.2/thinkgpt/condition.py` & `thinkgpt-0.0.3/thinkgpt/condition.py`

 * *Files identical despite different names*

### Comparing `thinkgpt-0.0.2/thinkgpt/gpt_select.py` & `thinkgpt-0.0.3/thinkgpt/gpt_select.py`

 * *Files identical despite different names*

### Comparing `thinkgpt-0.0.2/thinkgpt/helper.py` & `thinkgpt-0.0.3/thinkgpt/helper.py`

 * *Files identical despite different names*

### Comparing `thinkgpt-0.0.2/thinkgpt/infer.py` & `thinkgpt-0.0.3/thinkgpt/infer.py`

 * *Files identical despite different names*

### Comparing `thinkgpt-0.0.2/thinkgpt/llm.py` & `thinkgpt-0.0.3/thinkgpt/llm.py`

 * *Files identical despite different names*

### Comparing `thinkgpt-0.0.2/thinkgpt/memory.py` & `thinkgpt-0.0.3/thinkgpt/memory.py`

 * *Files identical despite different names*

### Comparing `thinkgpt-0.0.2/thinkgpt/refine.py` & `thinkgpt-0.0.3/thinkgpt/refine.py`

 * *Files identical despite different names*

### Comparing `thinkgpt-0.0.2/thinkgpt/summarize.py` & `thinkgpt-0.0.3/thinkgpt/summarize.py`

 * *Files 16% similar despite different names*

```diff
@@ -41,19 +41,16 @@
     def summarize(self, content: str, max_tokens: int = 4096, instruction_hint: str = '') -> str:
         response = self.summarize_chain.predict(
             # TODO: should retrieve max tokens from the llm if None
             content=content, instruction_hint=instruction_hint, max_tokens=max_tokens
         )
         return response
 
-    def chunked_summarize(self, content: str, max_tokens: int = 4096) -> str:
+    def chunked_summarize(self, content: str, max_tokens: int = 4096, instruction_hint: str = '') -> str:
         num_tokens = self.summarize_chain.llm.get_num_tokens(content)
-        # TODO: actually this is just for https://github.com/muellerberndt/micro-gpt, maybe just put it in the
-        #  downstream
-        instruction_hint = "Do your best to retain all semantic information including tasks performed by the agent, website content, important data points and hyper-links"
 
         if num_tokens > max_tokens:
             avg_chars_per_token = len(content) / num_tokens
             chunk_size = int(avg_chars_per_token * self.summarize_chain.summarizer_chunk_size)
             chunks = textwrap.wrap(content, chunk_size)
             summary_size = int(max_tokens / len(chunks))
             result = ""
```

### Comparing `thinkgpt-0.0.2/PKG-INFO` & `thinkgpt-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thinkgpt
-Version: 0.0.2
+Version: 0.0.3
 Summary: ThinkGPT is a Python library aimed at implementing Chain of Thoughts for Large Language Models (LLMs), prompting the model to think, reason, and to create generative agents.
 License: Apache 2.0
 Author: Alaeddine Abdessalem
 Author-email: alaeddine-13@live.fr
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

