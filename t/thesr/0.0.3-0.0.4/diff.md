# Comparing `tmp/thesr-0.0.3.tar.gz` & `tmp/thesr-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thesr-0.0.3.tar", last modified: Thu Mar 30 21:34:12 2023, max compression
+gzip compressed data, was "thesr-0.0.4.tar", last modified: Sun Apr 23 16:28:48 2023, max compression
```

## Comparing `thesr-0.0.3.tar` & `thesr-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0 john      (1000) john      (1000)        0 2023-03-30 21:34:12.464127 thesr-0.0.3/
--rwxrwxrwx   0 john      (1000) john      (1000)    35147 2023-03-03 20:34:52.000000 thesr-0.0.3/LICENSE.txt
--rwxrwxrwx   0 john      (1000) john      (1000)     3804 2023-03-30 21:34:12.464127 thesr-0.0.3/PKG-INFO
--rwxrwxrwx   0 john      (1000) john      (1000)     3417 2023-03-30 21:30:26.000000 thesr-0.0.3/README.md
--rwxrwxrwx   0 john      (1000) john      (1000)      100 2023-03-30 21:24:00.000000 thesr-0.0.3/pyproject.toml
--rwxrwxrwx   0 john      (1000) john      (1000)       78 2023-03-30 21:34:12.469548 thesr-0.0.3/setup.cfg
--rwxrwxrwx   0 john      (1000) john      (1000)      870 2023-03-30 21:23:54.000000 thesr-0.0.3/setup.py
-drwxrwxrwx   0 john      (1000) john      (1000)        0 2023-03-30 21:34:12.442041 thesr-0.0.3/thesr/
--rwxrwxrwx   0 john      (1000) john      (1000)        0 2023-03-03 20:35:58.000000 thesr-0.0.3/thesr/__init__.py
--rwxrwxrwx   0 john      (1000) john      (1000)     6746 2023-03-30 21:29:51.000000 thesr-0.0.3/thesr/thesr.py
-drwxrwxrwx   0 john      (1000) john      (1000)        0 2023-03-30 21:34:12.461030 thesr-0.0.3/thesr.egg-info/
--rwxrwxrwx   0 john      (1000) john      (1000)     3804 2023-03-30 21:34:12.000000 thesr-0.0.3/thesr.egg-info/PKG-INFO
--rwxrwxrwx   0 john      (1000) john      (1000)      232 2023-03-30 21:34:12.000000 thesr-0.0.3/thesr.egg-info/SOURCES.txt
--rwxrwxrwx   0 john      (1000) john      (1000)        1 2023-03-30 21:34:12.000000 thesr-0.0.3/thesr.egg-info/dependency_links.txt
--rwxrwxrwx   0 john      (1000) john      (1000)       44 2023-03-30 21:34:12.000000 thesr-0.0.3/thesr.egg-info/requires.txt
--rwxrwxrwx   0 john      (1000) john      (1000)        6 2023-03-30 21:34:12.000000 thesr-0.0.3/thesr.egg-info/top_level.txt
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-23 16:28:48.671367 thesr-0.0.4/
+-rw-r--r--   0 john      (1000) john      (1000)    35147 2023-03-04 03:45:59.000000 thesr-0.0.4/LICENSE.txt
+-rw-r--r--   0 john      (1000) john      (1000)     3804 2023-04-23 16:28:48.671367 thesr-0.0.4/PKG-INFO
+-rw-r--r--   0 john      (1000) john      (1000)     3417 2023-04-22 18:43:05.000000 thesr-0.0.4/README.md
+-rw-r--r--   0 john      (1000) john      (1000)      100 2023-04-23 16:27:14.000000 thesr-0.0.4/pyproject.toml
+-rw-r--r--   0 john      (1000) john      (1000)       78 2023-04-23 16:28:48.675368 thesr-0.0.4/setup.cfg
+-rw-r--r--   0 john      (1000) john      (1000)      870 2023-04-23 16:27:10.000000 thesr-0.0.4/setup.py
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-23 16:28:48.671367 thesr-0.0.4/thesr/
+-rw-r--r--   0 john      (1000) john      (1000)        0 2023-03-04 03:45:59.000000 thesr-0.0.4/thesr/__init__.py
+-rw-r--r--   0 john      (1000) john      (1000)     8321 2023-04-23 16:26:55.000000 thesr-0.0.4/thesr/thesr.py
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-23 16:28:48.671367 thesr-0.0.4/thesr.egg-info/
+-rw-r--r--   0 john      (1000) john      (1000)     3804 2023-04-23 16:28:48.000000 thesr-0.0.4/thesr.egg-info/PKG-INFO
+-rw-r--r--   0 john      (1000) john      (1000)      232 2023-04-23 16:28:48.000000 thesr-0.0.4/thesr.egg-info/SOURCES.txt
+-rw-r--r--   0 john      (1000) john      (1000)        1 2023-04-23 16:28:48.000000 thesr-0.0.4/thesr.egg-info/dependency_links.txt
+-rw-r--r--   0 john      (1000) john      (1000)       44 2023-04-23 16:28:48.000000 thesr-0.0.4/thesr.egg-info/requires.txt
+-rw-r--r--   0 john      (1000) john      (1000)        6 2023-04-23 16:28:48.000000 thesr-0.0.4/thesr.egg-info/top_level.txt
```

### Comparing `thesr-0.0.3/LICENSE.txt` & `thesr-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `thesr-0.0.3/PKG-INFO` & `thesr-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: thesr
-Version: 0.0.3
+Version: 0.0.4
 Summary: thesaurus (and also dictionary)
 Home-page: https://github.com/treatmesubj/Thesaurus_Rex
-Download-URL: https://github.com/treatmesubj/Thesaurus_Rex/archive/refs/tags/v0.0.3.tar.gz
+Download-URL: https://github.com/treatmesubj/Thesaurus_Rex/archive/refs/tags/v0.0.4.tar.gz
 Author: John Hupperts
 Author-email: jrock4503@hotmail.com
 License: gpl-3.0
 Project-URL: Source, https://github.com/treatmesubj/Thesaurus_Rex
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# Thesaurus Rex
+# Thesaurus-Rex
 Thesaurus tool that fetches a word's homonyms, synonyms, and antonyms from [Thesaurus.com](https://www.thesaurus.com/). It's also a dictionary tool that fetches definitions from [Webster](https://www.merriam-webster.com/). It fetches etymology information from [etymonline](https://www.etymonline.com/).
 
 ### Installation
 - from [PyPI](https://pypi.org/project/thesr): `pip install thesr`
 - from [GitHub](https://github.com/treatmesubj/Thesaurus_Rex): `pip install "git+https://github.com/treatmesubj/Thesaurus_Rex"`
 
 ### Usage
```

### Comparing `thesr-0.0.3/README.md` & `thesr-0.0.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Thesaurus Rex
+# Thesaurus-Rex
 Thesaurus tool that fetches a word's homonyms, synonyms, and antonyms from [Thesaurus.com](https://www.thesaurus.com/). It's also a dictionary tool that fetches definitions from [Webster](https://www.merriam-webster.com/). It fetches etymology information from [etymonline](https://www.etymonline.com/).
 
 ### Installation
 - from [PyPI](https://pypi.org/project/thesr): `pip install thesr`
 - from [GitHub](https://github.com/treatmesubj/Thesaurus_Rex): `pip install "git+https://github.com/treatmesubj/Thesaurus_Rex"`
 
 ### Usage
```

### Comparing `thesr-0.0.3/setup.py` & `thesr-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="thesr",
-    version="0.0.3",
+    version="0.0.4",
     license="gpl-3.0",
     author="John Hupperts",
     author_email="jrock4503@hotmail.com",
     description="thesaurus (and also dictionary)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/treatmesubj/Thesaurus_Rex",
-    download_url="https://github.com/treatmesubj/Thesaurus_Rex/archive/refs/tags/v0.0.3.tar.gz",
+    download_url="https://github.com/treatmesubj/Thesaurus_Rex/archive/refs/tags/v0.0.4.tar.gz",
     packages=["thesr"],
     package_dir={"Thesaurus_Rex": "thesr"},
     project_urls={
         "Source": "https://github.com/treatmesubj/Thesaurus_Rex",
     },
     install_requires=[
         "requests",
```

### Comparing `thesr-0.0.3/thesr/thesr.py` & `thesr-0.0.4/thesr/thesr.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,154 +4,212 @@
 import re
 import json
 import random
 from spellchecker import SpellChecker
 import os
 from rich.console import Console
 import argparse
+import socket
+import requests.packages.urllib3.util.connection as urllib3_cn
+
+# from fake_useragent import UserAgent
+
+
+def _allowed_gai_family():
+    # https://github.com/shazow/urllib3/blob/master/urllib3/util/connection.py
+    family = socket.AF_INET
+    # if urllib3_cn.HAS_IPV6:
+    #    family = socket.AF_INET6 # force ipv6 only if it is available
+    return family
+
+
+urllib3_cn.allowed_gai_family = _allowed_gai_family
+# headers = {
+#    "User-Agent": str(UserAgent().random),
+# }
 
 
 def get_random_word():
-    soup = BeautifulSoup(requests.get("https://www.merriam-webster.com/word-of-the-day/calendar").text, 'html.parser')
-    word_elems = soup.select("div.more-words-of-day-container ul.more-wod-items li h2 a")
+    response = requests.get("https://www.merriam-webster.com/word-of-the-day/calendar")
+    soup = BeautifulSoup(
+        response.text,
+        "html.parser",
+    )
+    word_elems = soup.select(
+        "div.more-words-of-day-container ul.more-wod-items li h2 a"
+    )
     words = [word_elem.text for word_elem in word_elems]
-    random_word = words[random.randint(0, len(words)-1)]
+    random_word = words[random.randint(0, len(words) - 1)]
     return random_word
 
 
 def get_defs(word):
-    soup = BeautifulSoup(requests.get(f"https://www.merriam-webster.com/dictionary/{word}").text, 'html.parser')
+    response = requests.get(f"https://www.merriam-webster.com/dictionary/{word}")
+    soup = BeautifulSoup(
+        response.text,
+        "html.parser",
+    )
     dict_entry_elems = soup.select("div[id*='dictionary-entry']")
-    word_class_elems = soup.select("div.row.entry-header a.important-blue-link")[:len(dict_entry_elems)]
+    word_class_elems = soup.select("div.row.entry-header a.important-blue-link")[
+        : len(dict_entry_elems)
+    ]
     zipped_elems = zip(dict_entry_elems, word_class_elems)
 
     homonyms = []
     try:
         for dict_entry_elem, word_class_elem in zipped_elems:
             definitions_elems = dict_entry_elem.select("span.dtText")
             word_class = word_class_elem.text
             for definition_elem in definitions_elems:
                 definition = definition_elem.text[2:]
-                homonyms.append({
-                    'definition': definition,
-                    'word_class': word_class
-                    })
+                homonyms.append({"definition": definition, "word_class": word_class})
         if homonyms:
             return homonyms
     except Exception:
         return
 
 
 def get_syns_ants(word):
-    soup = BeautifulSoup(requests.get(f"http://www.thesaurus.com/browse/{word}", headers={"user-agent": "Mozilla/5.0"}).text, 'html.parser')
-    script = re.search(r'<script>[\s\S]*window\.INITIAL_STATE = (.+);[\s\S]*</script>', soup.prettify()).group(1)
+    response = requests.get(f"http://www.thesaurus.com/browse/{word}")
+    soup = BeautifulSoup(
+        response.text,
+        "html.parser",
+    )
+    script = re.search(
+        r"<script>[\s\S]*window\.INITIAL_STATE = (.+);[\s\S]*</script>", soup.prettify()
+    ).group(1)
     # clean JSON
-    script = script.replace(":undefined", ":\"undefined\"")
-    script = script.replace(":null", ":\"null\"")
+    script = script.replace(":undefined", ':"undefined"')
+    script = script.replace(":null", ':"null"')
 
     j = json.loads(script)
 
     try:
-        posTabs = j['searchData']['tunaApiData']['posTabs']
+        posTabs = j["searchData"]["tunaApiData"]["posTabs"]
     except TypeError:
         return
 
     homonyms = []
     for tab in posTabs:
-        homonyms.append({
-            'word_class': tab['pos'],
-            'definition': tab['definition'],
-            'synonyms': [s['term'] for s in tab['synonyms']],
-            'antonyms': [s['term'] for s in tab['antonyms']]
-            })
+        homonyms.append(
+            {
+                "word_class": tab["pos"],
+                "definition": tab["definition"],
+                "synonyms": [s["term"] for s in tab["synonyms"]],
+                "antonyms": [s["term"] for s in tab["antonyms"]],
+            }
+        )
     return homonyms
 
 
 def get_etymology(word):
-    soup = BeautifulSoup(requests.get(f"https://www.etymonline.com/word/{word}").text, 'html.parser')
+    response = requests.get(f"https://www.etymonline.com/word/{word}")
+    soup = BeautifulSoup(response.text, "html.parser")
     class_elems = soup.select("div[class^='word'] [class^='word__name']")
     etym_elems = soup.select("div[class^='word'] [class^='word__def']")
     zipped_elems = zip(class_elems, etym_elems)
     homonyms = []
     for class_elem, etym_elem in zipped_elems:
-        if 'href' not in class_elem.attrs.keys():
+        if "href" not in class_elem.attrs.keys():
             etym_text = ""
-            for etym_p_elem in etym_elem.select('p'):
+            for etym_p_elem in etym_elem.select("p"):
                 etym_text += f"{etym_p_elem.text}\n"
-            homonyms.append({
-                'etym_desc': etym_text.rstrip('\n'),
-                'word_class': class_elem.text
-                })
+            homonyms.append(
+                {"etym_desc": etym_text.rstrip("\n"), "word_class": class_elem.text}
+            )
     return homonyms
 
 
 class Word:
-    def __init__(self, word, console):
+    def __init__(self, word, console=None):
         self.spelling = word
         self.thesr_homonyms = get_syns_ants(self.spelling)
         self.console = console
 
     def show_syns(self):
         print(f"[{self.spelling}!]", end="\n\n")
         print(f"---Synonyms{'-'*67}")
         if getattr(self, "thesr_homonyms", None):
             for homonym in self.thesr_homonyms:
-                console.print(f"[magenta]{{ {homonym['word_class']}: {homonym['definition']} }}[/magenta] [green]==[/green] [green]{homonym['synonyms'][:10]}[/green]")
+                if self.console:
+                    self.console.print(
+                        f"[magenta]{{ {homonym['word_class']}: {homonym['definition']} }}[/magenta] [green]==[/green] [green]{homonym['synonyms'][:10]}[/green]"
+                    )
+                else:
+                    print(
+                        f"{{ {homonym['word_class']}: {homonym['definition']} }} == {homonym['synonyms'][:10]}"
+                    )
         else:
             print("Sorry, no synonyms found")
-        print('-'*80, '\n')
+        print("-" * 80, "\n")
 
     def show_ants(self):
         print(f"---Antonyms{'-'*67}")
         if getattr(self, "thesr_homonyms", None):
             for homonym in self.thesr_homonyms:
-                console.print(f"[magenta]{{ {homonym['word_class']}: {homonym['definition']} }}[/magenta] [red]=/=[/red] [red]{homonym['antonyms'][:10]}[/red]")
+                if self.console:
+                    self.console.print(
+                        f"[magenta]{{ {homonym['word_class']}: {homonym['definition']} }}[/magenta] [red]=/=[/red] [red]{homonym['antonyms'][:10]}[/red]"
+                    )
+                else:
+                    print(
+                        f"{{ {homonym['word_class']}: {homonym['definition']} }} =/= {homonym['antonyms'][:10]}"
+                    )
         else:
             print("Sorry, no antonyms found")
-        print('-'*80, '\n')
+        print("-" * 80, "\n")
 
     def show_defs(self):
         print(f"---Definitions{'-'*67}")
-        if not getattr(self, 'webster_homonyms', None):
+        if not getattr(self, "webster_homonyms", None):
             self.webster_homonyms = get_defs(self.spelling)
-        if getattr(self, 'webster_homonyms', None):
+        if getattr(self, "webster_homonyms", None):
             for homonym in self.webster_homonyms:
-                console.print(f"[magenta]{{ {homonym['word_class']}: [/magenta][yellow]{homonym['definition']}[/yellow] [magenta]}}[/magenta]")
+                if self.console:
+                    console.print(
+                        f"[magenta]{{ {homonym['word_class']}: [/magenta][yellow]{homonym['definition']}[/yellow] [magenta]}}[/magenta]"
+                    )
+                else:
+                    print(f"{{ {homonym['word_class']}: {homonym['definition']} }}")
         else:
             print(f"Is {self.spelling} a word?")
             candidates = SpellChecker().candidates(self.spelling)
             if candidates:
                 candidates.discard(self.spelling)
                 print(f"Did you mean {candidates}?")
-        print('-'*80, '\n')
+        print("-" * 80, "\n")
 
     def show_etymology(self):
         print(f"---Etymology{'-'*67}")
-        if not getattr(self, 'etymology', None):
+        if not getattr(self, "etymology", None):
             self.etymology = get_etymology(self.spelling)
-        if getattr(self, 'etymology', None):
-            for homonym  in self.etymology:
-                console.print(f"[magenta]{homonym['word_class']}[/magenta]")
-                console.print(f"[white]{homonym['etym_desc']}[/white]")
+        if getattr(self, "etymology", None):
+            for homonym in self.etymology:
+                if self.console:
+                    console.print(f"[magenta]{homonym['word_class']}[/magenta]")
+                    console.print(f"[white]{homonym['etym_desc']}[/white]")
+                else:
+                    print(f"{homonym['word_class']}")
+                    print(f"{homonym['etym_desc']}")
         else:
             print("Sorry, no etymology found")
-        print('-'*80, '\n')
+        print("-" * 80, "\n")
 
 
 if __name__ == "__main__":
     print(
         """
          _____ _                                          
         |_   _| |                                         
           | | | |__   ___  ___  __ _ _   _ _ __ _   _ ___ 
           | | | '_ \\ / _ \\/ __|/ _` | | | | '__| | | / __|
           | | | | | |  __/\\__ \\ (_| | |_| | |  | |_| \\__ \\
           |_| |_| |_|\\___||___/\\__,_|\\__,_|_|   \\__,_|___/ Rex
         """
-            )
+    )
     console = Console()
 
     parser = argparse.ArgumentParser()
     parser.add_argument("--word", "-w", action="store")
     parser.add_argument("--define", "-d", action="store_true")
     parser.add_argument("--etymology", "-e", action="store_true")
     parser.add_argument("--antonyms", "-a", action="store_true")
@@ -167,8 +225,7 @@
 
     if args.define or args.verbose:
         thesr_word.show_defs()
     if args.etymology or args.verbose:
         thesr_word.show_etymology()
     if args.antonyms or args.verbose:
         thesr_word.show_ants()
-
```

### Comparing `thesr-0.0.3/thesr.egg-info/PKG-INFO` & `thesr-0.0.4/thesr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: thesr
-Version: 0.0.3
+Version: 0.0.4
 Summary: thesaurus (and also dictionary)
 Home-page: https://github.com/treatmesubj/Thesaurus_Rex
-Download-URL: https://github.com/treatmesubj/Thesaurus_Rex/archive/refs/tags/v0.0.3.tar.gz
+Download-URL: https://github.com/treatmesubj/Thesaurus_Rex/archive/refs/tags/v0.0.4.tar.gz
 Author: John Hupperts
 Author-email: jrock4503@hotmail.com
 License: gpl-3.0
 Project-URL: Source, https://github.com/treatmesubj/Thesaurus_Rex
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# Thesaurus Rex
+# Thesaurus-Rex
 Thesaurus tool that fetches a word's homonyms, synonyms, and antonyms from [Thesaurus.com](https://www.thesaurus.com/). It's also a dictionary tool that fetches definitions from [Webster](https://www.merriam-webster.com/). It fetches etymology information from [etymonline](https://www.etymonline.com/).
 
 ### Installation
 - from [PyPI](https://pypi.org/project/thesr): `pip install thesr`
 - from [GitHub](https://github.com/treatmesubj/Thesaurus_Rex): `pip install "git+https://github.com/treatmesubj/Thesaurus_Rex"`
 
 ### Usage
```

