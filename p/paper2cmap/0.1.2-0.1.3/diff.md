# Comparing `tmp/paper2cmap-0.1.2.tar.gz` & `tmp/paper2cmap-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paper2cmap-0.1.2.tar", last modified: Sat Apr 22 08:52:41 2023, max compression
+gzip compressed data, was "paper2cmap-0.1.3.tar", last modified: Sun Apr 23 06:24:56 2023, max compression
```

## Comparing `paper2cmap-0.1.2.tar` & `paper2cmap-0.1.3.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-22 08:52:41.781001 paper2cmap-0.1.2/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1065 2023-04-21 13:31:25.000000 paper2cmap-0.1.2/LICENSE
--rw-rw-r--   0 weitian   (1000) weitian   (1000)       41 2023-04-22 02:05:11.000000 paper2cmap-0.1.2/MANIFEST.in
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     5465 2023-04-22 08:52:41.781001 paper2cmap-0.1.2/PKG-INFO
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     3686 2023-04-22 08:39:00.000000 paper2cmap-0.1.2/README.md
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-22 08:52:41.773001 paper2cmap-0.1.2/paper2cmap/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      179 2023-04-22 08:52:16.000000 paper2cmap-0.1.2/paper2cmap/__init__.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     5243 2023-04-22 08:39:00.000000 paper2cmap-0.1.2/paper2cmap/cmapgpt.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     2368 2023-04-21 16:55:29.000000 paper2cmap-0.1.2/paper2cmap/llm.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      409 2023-04-21 11:49:55.000000 paper2cmap-0.1.2/paper2cmap/logger.py
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-22 08:52:41.777001 paper2cmap-0.1.2/paper2cmap/metas/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1157 2023-04-22 08:39:00.000000 paper2cmap-0.1.2/paper2cmap/metas/generate_examples.json
--rw-rw-r--   0 weitian   (1000) weitian   (1000)        8 2023-04-22 08:39:00.000000 paper2cmap-0.1.2/paper2cmap/metas/merge_and_prune_examples.json
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     2798 2023-04-22 08:39:00.000000 paper2cmap-0.1.2/paper2cmap/metas/prompts.yaml
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     5485 2023-04-22 08:51:30.000000 paper2cmap-0.1.2/paper2cmap/paper2cmap.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     3700 2023-04-22 08:39:00.000000 paper2cmap-0.1.2/paper2cmap/paper_reader.py
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-22 08:52:41.777001 paper2cmap-0.1.2/paper2cmap.egg-info/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     5465 2023-04-22 08:52:41.000000 paper2cmap-0.1.2/paper2cmap.egg-info/PKG-INFO
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      540 2023-04-22 08:52:41.000000 paper2cmap-0.1.2/paper2cmap.egg-info/SOURCES.txt
--rw-rw-r--   0 weitian   (1000) weitian   (1000)        1 2023-04-22 08:52:41.000000 paper2cmap-0.1.2/paper2cmap.egg-info/dependency_links.txt
--rw-rw-r--   0 weitian   (1000) weitian   (1000)       53 2023-04-22 08:52:41.000000 paper2cmap-0.1.2/paper2cmap.egg-info/requires.txt
--rw-rw-r--   0 weitian   (1000) weitian   (1000)       11 2023-04-22 08:52:41.000000 paper2cmap-0.1.2/paper2cmap.egg-info/top_level.txt
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      816 2023-04-22 08:51:54.000000 paper2cmap-0.1.2/pyproject.toml
--rw-rw-r--   0 weitian   (1000) weitian   (1000)       38 2023-04-22 08:52:41.781001 paper2cmap-0.1.2/setup.cfg
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-22 08:52:41.781001 paper2cmap-0.1.2/tests/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1979 2023-04-22 08:39:00.000000 paper2cmap-0.1.2/tests/test_cmapgpt.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      400 2023-04-22 08:39:00.000000 paper2cmap-0.1.2/tests/test_paper2cmap.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      474 2023-04-22 08:39:00.000000 paper2cmap-0.1.2/tests/test_paper_reader.py
+drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-23 06:24:56.421042 paper2cmap-0.1.3/
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     1065 2023-04-21 13:31:25.000000 paper2cmap-0.1.3/LICENSE
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)       41 2023-04-22 02:05:11.000000 paper2cmap-0.1.3/MANIFEST.in
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     5465 2023-04-23 06:24:56.421042 paper2cmap-0.1.3/PKG-INFO
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     3686 2023-04-22 08:39:00.000000 paper2cmap-0.1.3/README.md
+drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-23 06:24:56.417042 paper2cmap-0.1.3/paper2cmap/
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      179 2023-04-23 06:12:32.000000 paper2cmap-0.1.3/paper2cmap/__init__.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     6508 2023-04-23 06:07:47.000000 paper2cmap-0.1.3/paper2cmap/cmapgpt.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     2368 2023-04-21 16:55:29.000000 paper2cmap-0.1.3/paper2cmap/llm.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      409 2023-04-21 11:49:55.000000 paper2cmap-0.1.3/paper2cmap/logger.py
+drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-23 06:24:56.421042 paper2cmap-0.1.3/paper2cmap/metas/
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      947 2023-04-23 05:43:45.000000 paper2cmap-0.1.3/paper2cmap/metas/generate_examples.json
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      675 2023-04-23 06:03:31.000000 paper2cmap-0.1.3/paper2cmap/metas/merge_and_prune_examples.json
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)        8 2023-04-23 04:53:06.000000 paper2cmap-0.1.3/paper2cmap/metas/preprocess_examples.json
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     3068 2023-04-23 06:01:30.000000 paper2cmap-0.1.3/paper2cmap/metas/prompts.yaml
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     5603 2023-04-23 06:07:21.000000 paper2cmap-0.1.3/paper2cmap/paper2cmap.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     3700 2023-04-22 08:39:00.000000 paper2cmap-0.1.3/paper2cmap/paper_reader.py
+drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-23 06:24:56.421042 paper2cmap-0.1.3/paper2cmap.egg-info/
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     5465 2023-04-23 06:24:56.000000 paper2cmap-0.1.3/paper2cmap.egg-info/PKG-INFO
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      582 2023-04-23 06:24:56.000000 paper2cmap-0.1.3/paper2cmap.egg-info/SOURCES.txt
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)        1 2023-04-23 06:24:56.000000 paper2cmap-0.1.3/paper2cmap.egg-info/dependency_links.txt
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)       53 2023-04-23 06:24:56.000000 paper2cmap-0.1.3/paper2cmap.egg-info/requires.txt
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)       11 2023-04-23 06:24:56.000000 paper2cmap-0.1.3/paper2cmap.egg-info/top_level.txt
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      816 2023-04-23 06:12:26.000000 paper2cmap-0.1.3/pyproject.toml
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)       38 2023-04-23 06:24:56.421042 paper2cmap-0.1.3/setup.cfg
+drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-23 06:24:56.421042 paper2cmap-0.1.3/tests/
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     2075 2023-04-23 05:18:04.000000 paper2cmap-0.1.3/tests/test_cmapgpt.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      400 2023-04-22 08:39:00.000000 paper2cmap-0.1.3/tests/test_paper2cmap.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      474 2023-04-22 08:39:00.000000 paper2cmap-0.1.3/tests/test_paper_reader.py
```

### Comparing `paper2cmap-0.1.2/LICENSE` & `paper2cmap-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `paper2cmap-0.1.2/PKG-INFO` & `paper2cmap-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper2cmap
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package that automatically generates a concept map for a PDF document using LLM.
 Author-email: weitian <weitian.bnu@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Tian Wei
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `paper2cmap-0.1.2/README.md` & `paper2cmap-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `paper2cmap-0.1.2/paper2cmap/cmapgpt.py` & `paper2cmap-0.1.3/paper2cmap/cmapgpt.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,26 +20,37 @@
 
 class CMapGPT():
     def __init__(self, chatbot: ChatOpenAI | AzureChatOpenAI) -> None:
         self._prompt_config = yaml.load(
             open(pkg_resources.resource_filename('paper2cmap', 'metas/prompts.yaml'), "r"),
             Loader=yaml.FullLoader
             )
+        self._preprocess_system_prompt = self._prompt_config["preprocess"]["system"]
+        self._preprocess_user_prompt = self._prompt_config["preprocess"]["user"]
         self._generate_system_prompt = self._prompt_config["generate"]["system"]
         self._generate_user_prompt = self._prompt_config["generate"]["user"]
         self._merge_and_prune_system_prompt = self._prompt_config["merge_and_prune"]["system"]
         self._merge_and_prune_user_prompt = self._prompt_config["merge_and_prune"]["user"]
 
+        self._preprocess_examples = json.load(
+            open(pkg_resources.resource_filename('paper2cmap', 'metas/preprocess_examples.json'), "r")
+            )
         self._generate_examples = json.load(
             open(pkg_resources.resource_filename('paper2cmap', 'metas/generate_examples.json'), "r")
             )
         self._merge_and_prune_examples = json.load(
             open(pkg_resources.resource_filename('paper2cmap', 'metas/merge_and_prune_examples.json'), "r")
             )
 
+        self.preprocess_prompt = self._create_prompt(
+            system_prompt=self._preprocess_system_prompt,
+            user_prompt=self._preprocess_user_prompt,
+            user_prompt_vars=["text"],
+            examples=self._preprocess_examples
+        )
         self.generate_prompt = self._create_prompt(
             system_prompt=self._generate_system_prompt,
             user_prompt=self._generate_user_prompt,
             user_prompt_vars=["text", "max_num_concepts", "max_num_relationships"],
             examples=self._generate_examples
         )
         self.merge_and_prune_prompt = self._create_prompt(
@@ -82,44 +93,58 @@
                         template_format="jinja2"
                     )
                 )
             )
 
         return ChatPromptTemplate.from_messages([system_message_prompt, *examples_message_prompts, human_message_prompt])
 
+    def preprocess(self, text: str) -> str:
+        """
+        Preprocess the given text to be ready for concept map generation.
+        Currently we summarize the text into few simple sentences as preprocessing.
+
+        :param text: str, the text input to the model.
+        :return: str, the preprocessed text.
+        """
+        inputs = self.preprocess_prompt.format_prompt(text=text)
+        logger.debug(f"[CMapGPT] Preprocess Prompt: {inputs.to_string()}")
+        response = self.chatbot(inputs.to_messages()).content
+        logger.debug(f"[CMapGPT] Preprocess Result: {response}")
+        return response
+
     def generate(self, text: str, max_num_concepts: int = 10, max_num_relationships: int = 30) -> List[Dict]:
         """
         Generate a concept map from the given text.
 
         :param text: str, the text input to the model.
         :param max_num_concepts: int, the maximum number of concepts to generate.
         :param max_num_relationships: int, the maximum number of relationships to generate.
         :return: List[Dict], the generated concept map.
         """
         inputs = self.generate_prompt.format_prompt(
             text=text,
             max_num_concepts=max_num_concepts,
             max_num_relationships=max_num_relationships
         )
-        logger.debug(f"[CMapGPT] Prompt: {inputs.to_string()}")
+        logger.debug(f"[CMapGPT] Generate Prompt: {inputs.to_string()}")
         response = self.chatbot(inputs.to_messages()).content
-        logger.debug(f"[CMapGPT] Result: {response}")
+        logger.debug(f"[CMapGPT] Generate Result: {response}")
         return json.loads(response)
 
     def merge_and_prune(self, cmap: List[Dict], max_num_concepts: int = 10, max_num_relationships: int = 30) -> List[Dict]:
         """
         Merge and prune the given concept map.
 
         :param cmap: List[Dict], the concept map to merge and prune.
         :param max_num_concepts: int, the maximum number of concepts to generate.
         :param max_num_relationships: int, the maximum number of relationships to generate.
         :return: List[Dict], the merged and pruned concept map.
         """
         inputs = self.merge_and_prune_prompt.format_prompt(
-            cmap=cmap,
+            cmap=json.dumps(cmap),
             max_num_concepts=max_num_concepts,
             max_num_relationships=max_num_relationships
         )
-        logger.debug(f"[CMapGPT] Prompt: {inputs.to_string()}")
+        logger.debug(f"[CMapGPT] Merge&Prune Prompt: {inputs.to_string()}")
         response = self.chatbot(inputs.to_messages()).content
-        logger.debug(f"[CMapGPT] Result: {response}")
+        logger.debug(f"[CMapGPT] Merge&Prune Result: {response}")
         return json.loads(response)
```

### Comparing `paper2cmap-0.1.2/paper2cmap/llm.py` & `paper2cmap-0.1.3/paper2cmap/llm.py`

 * *Files identical despite different names*

### Comparing `paper2cmap-0.1.2/paper2cmap/metas/prompts.yaml` & `paper2cmap-0.1.3/paper2cmap/metas/prompts.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,41 @@
+preprocess:
+  system: >-
+    Given a piece of text, your task is to summarize it in a few sentences.
+    Your summary should use simple subject-verb-object sentence structures as much as possible, avoid using complex sentence structures such as clauses.
+    Your summary should also capture the key concepts and relationships in the text, and provide an accurate and concise description of its content.
+
+  user: >-
+    {{text}}
+
 generate:
   system: >-
     A concept map is a graph that shows how different concepts are connected to each other.
     It consists of nodes which represent concepts, and links which represent relationships between concepts.
-    A concept is a domain-specific entity that typically can be described in no more than 5 words or phrases. It MUST be a noun or gerund phrase.
-    A relationship is a phrase that describes a connection between two concepts in no more than 10 words or phrase. It MUST be a verb or preposition phrase.
-    A concept map MUST be formated as a JSON string: [{"source": "source concept", "target": "target concept", "relationship": "relationship from source to target"}].
-    Notice ["source", "relationship", "target"] MUST compose a valid sentence!!!
+    A concept is a domain-specific entity that typically can be described in no more than 3 words or phrases. It MUST be a noun or gerund phrase.
+    A relationship is a phrase that describes a connection between two concepts in no more than 5 words or phrase. It MUST be a verb or preposition phrase.
+    A concept map MUST be formated as a JSON string: [[source, relationship, target]].
+    Notice [source, relationship, target] MUST be a valid sentence!!!
 
   user: >-
     Now I input the text {\n {{text}} \n}, your task is to generate a concept map that contains the MOST central concepts and relationships from the text.
     You should rephrase the concepts and relationships phrase to make them more concise and natural.
     Pay attention to the direction of the relationship. For example, if the relationship is "is a part of", it means the source concept is a part of the target concept.
     Your output should have no more than {{max_num_concepts}} concepts and {{max_num_relationships}} relationships.
-    You output MUST be a valid JSON string without any additional note.
+    Your output MUST be a valid JSON string without any additional note.
     If you can't extract concepts or relationships from the input text, return an empty JSON [].
 
 merge_and_prune:
   system: >-
     A concept map is a graph that shows how different concepts are connected to each other.
     It consists of nodes which represent concepts, and links which represent relationships between concepts.
-    A concept is a domain-specific entity that typically can be described in no more than 5 words or phrases. It MUST be a noun or gerund phrase.
-    A relationship is a phrase that describes a connection between two concepts in no more than 10 words or phrase. It MUST be a verb or preposition phrase.
-    A concept map MUST be formated as a JSON string: [{"source": "source concept", "target": "target concept", "relationship": "relationship from source to target"}],
-    Notice ["source", "relationship", "target"] MUST compose a valid sentence!!!
+    A concept is a domain-specific entity that typically can be described in no more than 3 words or phrases. It MUST be a noun or gerund phrase.
+    A relationship is a phrase that describes a connection between two concepts in no more than 5 words or phrase. It MUST be a verb or preposition phrase.
+    A concept map MUST be formated as a JSON string: [[source, relationship, target]].
+    Notice [source, relationship, target] MUST be a valid sentence!!!
   
   user: >-
-    Now I input a concept map {\n {{cmap}} \n}, your task is to merge the similar concept nodes and prune unimportant or infrequent concepts and relationships.
+    Now I input a concept map {\n {{cmap}} \n}, your task is to generate a new concept map which merges similar concepts and prune unimportant relationships in the input concept map.
     You should rephrase the concepts and relationships phrase to make them more concise and natural.
     Your output should have no more than {{max_num_concepts}} concepts and {{max_num_relationships}} relationships.
-    You output MUST be a valid JSON string without any additional note.
+    Your output MUST be a valid JSON string without any additional note.
     If you can't make it, return the input concept map.
```

### Comparing `paper2cmap-0.1.2/paper2cmap/paper2cmap.py` & `paper2cmap-0.1.3/paper2cmap/paper2cmap.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,17 +69,20 @@
         :return: A list of concept maps.
         """
         cmap_list = []
         for i, section in enumerate(self.paper_reader.sections):
             if max_num_iterations != -1 and i >= max_num_iterations:
                 break
 
+            logger.info(f"[Paper2CMap] Preprocessing section {i}")
+            text = self.cmap_gpt.preprocess(section)
+
             logger.info(f"[Paper2CMap] Generating concept map for section {i}")
             cmap = self.cmap_gpt.generate(
-                text=section,
+                text=text,
                 max_num_concepts=max_num_concepts,
                 max_num_relationships=max_num_relationships
                 )
             logger.info(f"[Paper2CMap] Concept map for section {i}: {cmap}")
             
             cmap_list.append(cmap)
```

### Comparing `paper2cmap-0.1.2/paper2cmap/paper_reader.py` & `paper2cmap-0.1.3/paper2cmap/paper_reader.py`

 * *Files identical despite different names*

### Comparing `paper2cmap-0.1.2/paper2cmap.egg-info/PKG-INFO` & `paper2cmap-0.1.3/paper2cmap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper2cmap
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package that automatically generates a concept map for a PDF document using LLM.
 Author-email: weitian <weitian.bnu@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Tian Wei
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `paper2cmap-0.1.2/paper2cmap.egg-info/SOURCES.txt` & `paper2cmap-0.1.3/paper2cmap.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -11,11 +11,12 @@
 paper2cmap.egg-info/PKG-INFO
 paper2cmap.egg-info/SOURCES.txt
 paper2cmap.egg-info/dependency_links.txt
 paper2cmap.egg-info/requires.txt
 paper2cmap.egg-info/top_level.txt
 paper2cmap/metas/generate_examples.json
 paper2cmap/metas/merge_and_prune_examples.json
+paper2cmap/metas/preprocess_examples.json
 paper2cmap/metas/prompts.yaml
 tests/test_cmapgpt.py
 tests/test_paper2cmap.py
 tests/test_paper_reader.py
```

### Comparing `paper2cmap-0.1.2/pyproject.toml` & `paper2cmap-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "paper2cmap"
-version = "0.1.2"
+version = "0.1.3"
 description = "A package that automatically generates a concept map for a PDF document using LLM."
 readme = "README.md"
 authors = [{ name = "weitian", email = "weitian.bnu@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `paper2cmap-0.1.2/tests/test_cmapgpt.py` & `paper2cmap-0.1.3/tests/test_cmapgpt.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,12 +16,15 @@
     This has shifted the focus of natural language processing research away from the previous paradigm of training specialized supervised models for specific tasks.
     Large language models have most commonly used the transformer architecture, which, since 2018, has become the standard deep learning technique for sequential data (previously, recurrent architectures such as the LSTM were most common).
     LLMs are trained in an unsupervised manner on unannotated text. A left-to-right transformer is trained to maximize the probability assigned to the next word in the training data, given the previous context.
     Alternatively, an LLM may use a bidirectional transformer (as in the example of BERT), which assigns a probability distribution over words given access to both preceding and following context.
     In addition to the task of predicting the next word or "filling in the blanks", LLMs may be trained on auxiliary tasks which test their understanding of the data distribution, such as Next Sentence Prediction (NSP), in which pairs of sentences are presented and the model must predict whether they appear side-by-side in the training corpus.
     """
 
+    text_input = cmap_gpt.preprocess(text_input)
+    print(f"Preprocessed text: {text_input}")
+
     cmap = cmap_gpt.generate(text_input, max_num_concepts=5, max_num_relationships=10)
     print(f"Generated concept map: {cmap}")
 
     cmap = cmap_gpt.merge_and_prune(cmap, max_num_concepts=5, max_num_relationships=10)
     print(f"Merged and pruned concept map: {cmap}")
```

