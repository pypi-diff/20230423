# Comparing `tmp/pinyin_jyutping-0.7.tar.gz` & `tmp/pinyin_jyutping-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinyin_jyutping-0.7.tar", last modified: Thu Apr 13 03:41:48 2023, max compression
+gzip compressed data, was "pinyin_jyutping-0.8.tar", last modified: Sun Apr 23 12:43:40 2023, max compression
```

## Comparing `pinyin_jyutping-0.7.tar` & `pinyin_jyutping-0.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-04-13 03:41:48.470336 pinyin_jyutping-0.7/
--rw-r--r--   0 luc       (1000) luc       (1000)    35149 2023-03-31 01:12:26.000000 pinyin_jyutping-0.7/LICENSE
--rw-r--r--   0 luc       (1000) luc       (1000)       81 2023-03-31 01:12:26.000000 pinyin_jyutping-0.7/MANIFEST.in
--rw-r--r--   0 luc       (1000) luc       (1000)     2515 2023-04-13 03:41:48.469336 pinyin_jyutping-0.7/PKG-INFO
--rw-r--r--   0 luc       (1000) luc       (1000)     2158 2023-04-13 03:37:57.000000 pinyin_jyutping-0.7/README.rst
-drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-04-13 03:41:48.468336 pinyin_jyutping-0.7/pinyin_jyutping/
--rw-r--r--   0 luc       (1000) luc       (1000)     2148 2023-04-13 03:37:57.000000 pinyin_jyutping-0.7/pinyin_jyutping/__init__.py
--rw-r--r--   0 luc       (1000) luc       (1000)     2883 2023-03-31 01:12:26.000000 pinyin_jyutping-0.7/pinyin_jyutping/cache.py
--rw-r--r--   0 luc       (1000) luc       (1000)     8063 2023-03-31 01:12:26.000000 pinyin_jyutping-0.7/pinyin_jyutping/constants.py
--rw-r--r--   0 luc       (1000) luc       (1000)     7157 2023-04-13 03:37:57.000000 pinyin_jyutping-0.7/pinyin_jyutping/conversion.py
--rw-r--r--   0 luc       (1000) luc       (1000)      373 2023-03-31 01:12:26.000000 pinyin_jyutping-0.7/pinyin_jyutping/data.py
--rw-r--r--   0 luc       (1000) luc       (1000)  8583143 2023-03-31 01:12:26.000000 pinyin_jyutping-0.7/pinyin_jyutping/dict.txt.big
--rw-r--r--   0 luc       (1000) luc       (1000)      107 2023-03-31 01:12:26.000000 pinyin_jyutping-0.7/pinyin_jyutping/errors.py
--rw-r--r--   0 luc       (1000) luc       (1000)    10976 2023-04-13 03:37:57.000000 pinyin_jyutping-0.7/pinyin_jyutping/logic.py
--rw-r--r--   0 luc       (1000) luc       (1000)    11907 2023-03-31 01:12:26.000000 pinyin_jyutping-0.7/pinyin_jyutping/parser.py
--rw-r--r--   0 luc       (1000) luc       (1000) 18950460 2023-04-13 03:41:46.000000 pinyin_jyutping-0.7/pinyin_jyutping/pinyin_jyutping.pkl
--rw-r--r--   0 luc       (1000) luc       (1000)     2411 2023-03-31 01:12:26.000000 pinyin_jyutping-0.7/pinyin_jyutping/syllables.py
-drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-04-13 03:41:48.469336 pinyin_jyutping-0.7/pinyin_jyutping.egg-info/
--rw-r--r--   0 luc       (1000) luc       (1000)     2515 2023-04-13 03:41:47.000000 pinyin_jyutping-0.7/pinyin_jyutping.egg-info/PKG-INFO
--rw-r--r--   0 luc       (1000) luc       (1000)      578 2023-04-13 03:41:48.000000 pinyin_jyutping-0.7/pinyin_jyutping.egg-info/SOURCES.txt
--rw-r--r--   0 luc       (1000) luc       (1000)        1 2023-04-13 03:41:47.000000 pinyin_jyutping-0.7/pinyin_jyutping.egg-info/dependency_links.txt
--rw-r--r--   0 luc       (1000) luc       (1000)        1 2023-04-13 03:39:10.000000 pinyin_jyutping-0.7/pinyin_jyutping.egg-info/not-zip-safe
--rw-r--r--   0 luc       (1000) luc       (1000)        6 2023-04-13 03:41:48.000000 pinyin_jyutping-0.7/pinyin_jyutping.egg-info/requires.txt
--rw-r--r--   0 luc       (1000) luc       (1000)       16 2023-04-13 03:41:48.000000 pinyin_jyutping-0.7/pinyin_jyutping.egg-info/top_level.txt
--rw-r--r--   0 luc       (1000) luc       (1000)       38 2023-04-13 03:41:48.470336 pinyin_jyutping-0.7/setup.cfg
--rw-r--r--   0 luc       (1000) luc       (1000)      796 2023-04-13 03:41:08.000000 pinyin_jyutping-0.7/setup.py
+drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-04-23 12:43:40.358409 pinyin_jyutping-0.8/
+-rw-r--r--   0 luc       (1000) luc       (1000)    35149 2023-03-31 01:12:26.000000 pinyin_jyutping-0.8/LICENSE
+-rw-r--r--   0 luc       (1000) luc       (1000)       81 2023-03-31 01:12:26.000000 pinyin_jyutping-0.8/MANIFEST.in
+-rw-r--r--   0 luc       (1000) luc       (1000)     2655 2023-04-23 12:43:40.358409 pinyin_jyutping-0.8/PKG-INFO
+-rw-r--r--   0 luc       (1000) luc       (1000)     2303 2023-04-23 12:42:22.000000 pinyin_jyutping-0.8/README.rst
+drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-04-23 12:43:40.357409 pinyin_jyutping-0.8/pinyin_jyutping/
+-rw-r--r--   0 luc       (1000) luc       (1000)     2148 2023-04-13 03:37:57.000000 pinyin_jyutping-0.8/pinyin_jyutping/__init__.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     2883 2023-03-31 01:12:26.000000 pinyin_jyutping-0.8/pinyin_jyutping/cache.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     8063 2023-03-31 01:12:26.000000 pinyin_jyutping-0.8/pinyin_jyutping/constants.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     7367 2023-04-23 12:42:22.000000 pinyin_jyutping-0.8/pinyin_jyutping/conversion.py
+-rw-r--r--   0 luc       (1000) luc       (1000)      373 2023-03-31 01:12:26.000000 pinyin_jyutping-0.8/pinyin_jyutping/data.py
+-rw-r--r--   0 luc       (1000) luc       (1000)  8583143 2023-03-31 01:12:26.000000 pinyin_jyutping-0.8/pinyin_jyutping/dict.txt.big
+-rw-r--r--   0 luc       (1000) luc       (1000)      107 2023-03-31 01:12:26.000000 pinyin_jyutping-0.8/pinyin_jyutping/errors.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    10976 2023-04-13 03:37:57.000000 pinyin_jyutping-0.8/pinyin_jyutping/logic.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    11907 2023-03-31 01:12:26.000000 pinyin_jyutping-0.8/pinyin_jyutping/parser.py
+-rw-r--r--   0 luc       (1000) luc       (1000) 18950460 2023-04-23 12:43:38.000000 pinyin_jyutping-0.8/pinyin_jyutping/pinyin_jyutping.pkl
+-rw-r--r--   0 luc       (1000) luc       (1000)     2411 2023-03-31 01:12:26.000000 pinyin_jyutping-0.8/pinyin_jyutping/syllables.py
+drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-04-23 12:43:40.358409 pinyin_jyutping-0.8/pinyin_jyutping.egg-info/
+-rw-r--r--   0 luc       (1000) luc       (1000)     2655 2023-04-23 12:43:39.000000 pinyin_jyutping-0.8/pinyin_jyutping.egg-info/PKG-INFO
+-rw-r--r--   0 luc       (1000) luc       (1000)      578 2023-04-23 12:43:40.000000 pinyin_jyutping-0.8/pinyin_jyutping.egg-info/SOURCES.txt
+-rw-r--r--   0 luc       (1000) luc       (1000)        1 2023-04-23 12:43:39.000000 pinyin_jyutping-0.8/pinyin_jyutping.egg-info/dependency_links.txt
+-rw-r--r--   0 luc       (1000) luc       (1000)        1 2023-04-13 03:39:10.000000 pinyin_jyutping-0.8/pinyin_jyutping.egg-info/not-zip-safe
+-rw-r--r--   0 luc       (1000) luc       (1000)        6 2023-04-23 12:43:40.000000 pinyin_jyutping-0.8/pinyin_jyutping.egg-info/requires.txt
+-rw-r--r--   0 luc       (1000) luc       (1000)       16 2023-04-23 12:43:40.000000 pinyin_jyutping-0.8/pinyin_jyutping.egg-info/top_level.txt
+-rw-r--r--   0 luc       (1000) luc       (1000)       38 2023-04-23 12:43:40.358409 pinyin_jyutping-0.8/setup.cfg
+-rw-r--r--   0 luc       (1000) luc       (1000)      796 2023-04-23 12:43:01.000000 pinyin_jyutping-0.8/setup.py
```

### Comparing `pinyin_jyutping-0.7/LICENSE` & `pinyin_jyutping-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pinyin_jyutping-0.7/PKG-INFO` & `pinyin_jyutping-0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinyin_jyutping
-Version: 0.7
+Version: 0.8
 Summary: Convert a Chinese sentence to Pinyin or Jyutping
 Home-page: https://github.com/Language-Tools/pinyin-jyutping
 Author: LucW
 Author-email: languagetools@mailc.net
 License: GPL
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -25,46 +25,51 @@
 
     $ pip install pinyin_jyutping
 
 Usage
 -----
 
 **Pinyin**
+
 generate the best solution:
+
 >>> import pinyin_jyutping
 >>> p = pinyin_jyutping.PinyinJyutping()
 >>> p.pinyin('忘拿一些东西了')
 'wàng ná yīxiē dōngxī le'
 >>> p.pinyin('忘拿一些东西了', tone_numbers=True)
 'wang4 na2 yi1xie1 dong1xi1 le5'    
 >>> p.pinyin('忘拿一些东西了', tone_numbers=True, spaces=True)
 'wang4 na2 yi1 xie1 dong1 xi1 le5'    
 
 generate all possible solutions:
+
 >>> import pinyin_jyutping
 >>> p = pinyin_jyutping.PinyinJyutping()
 >>> p.pinyin_all_solutions('忘拿一些东西了')
-[['wàng'], ['ná'], ['yīxiē'], ['dōngxī', 'dōngxi'], ['le', 'liǎo', 'liào']]
+{'word_list': ['忘', '拿', '一些', '东西', '了'], 'solutions': [['wàng'], ['ná'], ['yīxiē'], ['dōngxī', 'dōngxi'], ['le', 'liǎo', 'liào']]}
 
 **Jyutping**
 
 generate the best solution:
+
 >>> import pinyin_jyutping
 >>> j = pinyin_jyutping.PinyinJyutping()
 >>> j.jyutping('我出去攞野食')
 'ngǒ cēothêoi ló jěsik'
 >>> j.jyutping('我出去攞野食', tone_numbers=True)
 'ngo5 ceot1heoi3 lo2 je5sik6'
 >>> j.jyutping('我出去攞野食', tone_numbers=True, spaces=True)
 'ngo5 ceot1 heoi3 lo2 je5 sik6'    
 
 generate all possible solutions:
+
 >>> import pinyin_jyutping
 >>> j = pinyin_jyutping.PinyinJyutping()
 >>> j.jyutping_all_solutions('我出去攞野食')
-[['ngǒ'], ['cēothêoi'], ['ló', 'lō'], ['jěsik', 'jězi', 'jěsit', 'jězik']]
+{'word_list': ['我', '出去', '攞', '野食'], 'solutions': [['ngǒ'], ['cēothêoi'], ['ló', 'lō'], ['jěsik', 'jězi', 'jěsit', 'jězik']]}
 
 How it works
 ------------
 
 Uses the Jieba library (https://github.com/fxsjy/jieba) to tokenize the sentence. Then words are converted to Pinyin/Jyutping either as a whole, or character by character, using the CC-Canto dictionary (http://cantonese.org/about.html). The Jyutping diacritic conversion is not standard but originally described here: http://www.cantonese.sheik.co.uk/phorum/read.php?1,127274,129006
```

### Comparing `pinyin_jyutping-0.7/README.rst` & `pinyin_jyutping-0.8/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -12,46 +12,51 @@
 
     $ pip install pinyin_jyutping
 
 Usage
 -----
 
 **Pinyin**
+
 generate the best solution:
+
 >>> import pinyin_jyutping
 >>> p = pinyin_jyutping.PinyinJyutping()
 >>> p.pinyin('忘拿一些东西了')
 'wàng ná yīxiē dōngxī le'
 >>> p.pinyin('忘拿一些东西了', tone_numbers=True)
 'wang4 na2 yi1xie1 dong1xi1 le5'    
 >>> p.pinyin('忘拿一些东西了', tone_numbers=True, spaces=True)
 'wang4 na2 yi1 xie1 dong1 xi1 le5'    
 
 generate all possible solutions:
+
 >>> import pinyin_jyutping
 >>> p = pinyin_jyutping.PinyinJyutping()
 >>> p.pinyin_all_solutions('忘拿一些东西了')
-[['wàng'], ['ná'], ['yīxiē'], ['dōngxī', 'dōngxi'], ['le', 'liǎo', 'liào']]
+{'word_list': ['忘', '拿', '一些', '东西', '了'], 'solutions': [['wàng'], ['ná'], ['yīxiē'], ['dōngxī', 'dōngxi'], ['le', 'liǎo', 'liào']]}
 
 **Jyutping**
 
 generate the best solution:
+
 >>> import pinyin_jyutping
 >>> j = pinyin_jyutping.PinyinJyutping()
 >>> j.jyutping('我出去攞野食')
 'ngǒ cēothêoi ló jěsik'
 >>> j.jyutping('我出去攞野食', tone_numbers=True)
 'ngo5 ceot1heoi3 lo2 je5sik6'
 >>> j.jyutping('我出去攞野食', tone_numbers=True, spaces=True)
 'ngo5 ceot1 heoi3 lo2 je5 sik6'    
 
 generate all possible solutions:
+
 >>> import pinyin_jyutping
 >>> j = pinyin_jyutping.PinyinJyutping()
 >>> j.jyutping_all_solutions('我出去攞野食')
-[['ngǒ'], ['cēothêoi'], ['ló', 'lō'], ['jěsik', 'jězi', 'jěsit', 'jězik']]
+{'word_list': ['我', '出去', '攞', '野食'], 'solutions': [['ngǒ'], ['cēothêoi'], ['ló', 'lō'], ['jěsik', 'jězi', 'jěsit', 'jězik']]}
 
 How it works
 ------------
 
 Uses the Jieba library (https://github.com/fxsjy/jieba) to tokenize the sentence. Then words are converted to Pinyin/Jyutping either as a whole, or character by character, using the CC-Canto dictionary (http://cantonese.org/about.html). The Jyutping diacritic conversion is not standard but originally described here: http://www.cantonese.sheik.co.uk/phorum/read.php?1,127274,129006
```

### Comparing `pinyin_jyutping-0.7/pinyin_jyutping/__init__.py` & `pinyin_jyutping-0.8/pinyin_jyutping/__init__.py`

 * *Files identical despite different names*

### Comparing `pinyin_jyutping-0.7/pinyin_jyutping/cache.py` & `pinyin_jyutping-0.8/pinyin_jyutping/cache.py`

 * *Files identical despite different names*

### Comparing `pinyin_jyutping-0.7/pinyin_jyutping/constants.py` & `pinyin_jyutping-0.8/pinyin_jyutping/constants.py`

 * *Files identical despite different names*

### Comparing `pinyin_jyutping-0.7/pinyin_jyutping/conversion.py` & `pinyin_jyutping-0.8/pinyin_jyutping/conversion.py`

 * *Files 3% similar despite different names*

```diff
@@ -84,20 +84,26 @@
     word_list = tokenize(text)
     word_list = improve_tokenization(word_map, word_list)
     return word_list
 
 def convert_to_romanization(word_map, text, tone_numbers, spaces):
     solution_list = []
     word_list = tokenize_to_word_list(word_map, text)
-    return render_all_romanization_solutions(word_map, word_list, tone_numbers, spaces)
+    solutions = render_all_romanization_solutions(word_map, word_list, tone_numbers, spaces)
+    return {
+        'word_list': word_list, 
+        'solutions': solutions
+    }
 
 def convert_single_solution(word_map, text, tone_numbers, spaces):
     # first, get all solutions
-    all_solutions = convert_to_romanization(word_map, text, tone_numbers, spaces)
+    data = convert_to_romanization(word_map, text, tone_numbers, spaces)
+    all_solutions = data['solutions']
     # just assemble the most probable solution for each word
+    logger.debug(f'convert_single_solution, all_solutions: {pprint.pformat(all_solutions)}')
     return ' '.join(word_solutions[0] for word_solutions in all_solutions)
 
 def convert_pinyin_single_solution(data, text, tone_numbers, spaces):
     word_map = data.pinyin_map
     return convert_single_solution(word_map, text, tone_numbers, spaces)
 
 def convert_jyutping_single_solution(data, text, tone_numbers, spaces):
```

### Comparing `pinyin_jyutping-0.7/pinyin_jyutping/dict.txt.big` & `pinyin_jyutping-0.8/pinyin_jyutping/dict.txt.big`

 * *Files identical despite different names*

### Comparing `pinyin_jyutping-0.7/pinyin_jyutping/logic.py` & `pinyin_jyutping-0.8/pinyin_jyutping/logic.py`

 * *Files identical despite different names*

### Comparing `pinyin_jyutping-0.7/pinyin_jyutping/parser.py` & `pinyin_jyutping-0.8/pinyin_jyutping/parser.py`

 * *Files identical despite different names*

### Comparing `pinyin_jyutping-0.7/pinyin_jyutping/pinyin_jyutping.pkl` & `pinyin_jyutping-0.8/pinyin_jyutping/pinyin_jyutping.pkl`

 * *Files identical despite different names*

### Comparing `pinyin_jyutping-0.7/pinyin_jyutping/syllables.py` & `pinyin_jyutping-0.8/pinyin_jyutping/syllables.py`

 * *Files identical despite different names*

### Comparing `pinyin_jyutping-0.7/pinyin_jyutping.egg-info/PKG-INFO` & `pinyin_jyutping-0.8/pinyin_jyutping.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinyin-jyutping
-Version: 0.7
+Version: 0.8
 Summary: Convert a Chinese sentence to Pinyin or Jyutping
 Home-page: https://github.com/Language-Tools/pinyin-jyutping
 Author: LucW
 Author-email: languagetools@mailc.net
 License: GPL
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -25,46 +25,51 @@
 
     $ pip install pinyin_jyutping
 
 Usage
 -----
 
 **Pinyin**
+
 generate the best solution:
+
 >>> import pinyin_jyutping
 >>> p = pinyin_jyutping.PinyinJyutping()
 >>> p.pinyin('忘拿一些东西了')
 'wàng ná yīxiē dōngxī le'
 >>> p.pinyin('忘拿一些东西了', tone_numbers=True)
 'wang4 na2 yi1xie1 dong1xi1 le5'    
 >>> p.pinyin('忘拿一些东西了', tone_numbers=True, spaces=True)
 'wang4 na2 yi1 xie1 dong1 xi1 le5'    
 
 generate all possible solutions:
+
 >>> import pinyin_jyutping
 >>> p = pinyin_jyutping.PinyinJyutping()
 >>> p.pinyin_all_solutions('忘拿一些东西了')
-[['wàng'], ['ná'], ['yīxiē'], ['dōngxī', 'dōngxi'], ['le', 'liǎo', 'liào']]
+{'word_list': ['忘', '拿', '一些', '东西', '了'], 'solutions': [['wàng'], ['ná'], ['yīxiē'], ['dōngxī', 'dōngxi'], ['le', 'liǎo', 'liào']]}
 
 **Jyutping**
 
 generate the best solution:
+
 >>> import pinyin_jyutping
 >>> j = pinyin_jyutping.PinyinJyutping()
 >>> j.jyutping('我出去攞野食')
 'ngǒ cēothêoi ló jěsik'
 >>> j.jyutping('我出去攞野食', tone_numbers=True)
 'ngo5 ceot1heoi3 lo2 je5sik6'
 >>> j.jyutping('我出去攞野食', tone_numbers=True, spaces=True)
 'ngo5 ceot1 heoi3 lo2 je5 sik6'    
 
 generate all possible solutions:
+
 >>> import pinyin_jyutping
 >>> j = pinyin_jyutping.PinyinJyutping()
 >>> j.jyutping_all_solutions('我出去攞野食')
-[['ngǒ'], ['cēothêoi'], ['ló', 'lō'], ['jěsik', 'jězi', 'jěsit', 'jězik']]
+{'word_list': ['我', '出去', '攞', '野食'], 'solutions': [['ngǒ'], ['cēothêoi'], ['ló', 'lō'], ['jěsik', 'jězi', 'jěsit', 'jězik']]}
 
 How it works
 ------------
 
 Uses the Jieba library (https://github.com/fxsjy/jieba) to tokenize the sentence. Then words are converted to Pinyin/Jyutping either as a whole, or character by character, using the CC-Canto dictionary (http://cantonese.org/about.html). The Jyutping diacritic conversion is not standard but originally described here: http://www.cantonese.sheik.co.uk/phorum/read.php?1,127274,129006
```

### Comparing `pinyin_jyutping-0.7/pinyin_jyutping.egg-info/SOURCES.txt` & `pinyin_jyutping-0.8/pinyin_jyutping.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pinyin_jyutping-0.7/setup.py` & `pinyin_jyutping-0.8/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 # build instructions
 #  python3 setup.py sdist
 # twine upload dist/*
 
 setup(name='pinyin_jyutping',
-      version='0.7',
+      version='0.8',
       description='Convert a Chinese sentence to Pinyin or Jyutping',
       long_description=open('README.rst', encoding='utf-8').read(),
       url='https://github.com/Language-Tools/pinyin-jyutping',
       author='LucW',
       author_email='languagetools@mailc.net',
       classifiers=[
         'Programming Language :: Python :: 3.7',
```

