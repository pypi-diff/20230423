# Comparing `tmp/khl-1.0.7.tar.gz` & `tmp/khl-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "khl-1.0.7.tar", max compression
+gzip compressed data, was "khl-2.0.0.tar", max compression
```

## Comparing `khl-1.0.7.tar` & `khl-2.0.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1065 2023-03-05 17:17:58.027493 khl-1.0.7/LICENSE
--rw-r--r--   0        0        0     5525 2023-04-22 10:15:25.994692 khl-1.0.7/README.md
--rw-r--r--   0        0        0     2297 2023-04-22 10:54:10.906352 khl-1.0.7/khl/__init__.py
--rw-r--r--   0        0        0     8829 2023-03-10 16:38:07.463209 khl-1.0.7/khl/preprocess.py
--rw-r--r--   0        0        0     2426 2023-03-10 17:49:51.106914 khl-1.0.7/khl/stop_words.py
--rw-r--r--   0        0        0     3274 2023-03-10 16:26:00.431309 khl-1.0.7/khl/teams_orgs.py
--rw-r--r--   0        0        0    31173 2023-04-22 10:53:40.734066 khl-1.0.7/khl/utils.py
--rw-r--r--   0        0        0     8346 2023-03-05 17:17:58.031493 khl-1.0.7/khl/wrong_lemmas.py
--rw-r--r--   0        0        0     1589 2023-04-22 10:54:16.494404 khl-1.0.7/pyproject.toml
--rw-r--r--   0        0        0     6466 1970-01-01 00:00:00.000000 khl-1.0.7/setup.py
--rw-r--r--   0        0        0     6248 1970-01-01 00:00:00.000000 khl-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-03-05 17:17:58.027493 khl-2.0.0/LICENSE
+-rw-r--r--   0        0        0     5409 2023-04-23 14:40:41.764203 khl-2.0.0/README.md
+-rw-r--r--   0        0        0     2266 2023-04-23 14:40:56.976257 khl-2.0.0/khl/__init__.py
+-rw-r--r--   0        0        0     8710 2023-04-23 14:40:41.764203 khl-2.0.0/khl/preprocess.py
+-rw-r--r--   0        0        0     2416 2023-04-23 09:41:56.980021 khl-2.0.0/khl/stop_words.py
+-rw-r--r--   0        0        0     3274 2023-03-10 16:26:00.431309 khl-2.0.0/khl/teams_orgs.py
+-rw-r--r--   0        0        0    31158 2023-04-23 14:40:41.764203 khl-2.0.0/khl/utils.py
+-rw-r--r--   0        0        0     8346 2023-03-05 17:17:58.031493 khl-2.0.0/khl/wrong_lemmas.py
+-rw-r--r--   0        0        0     1589 2023-04-23 14:41:12.808314 khl-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     6354 1970-01-01 00:00:00.000000 khl-2.0.0/setup.py
+-rw-r--r--   0        0        0     6132 1970-01-01 00:00:00.000000 khl-2.0.0/PKG-INFO
```

### Comparing `khl-1.0.7/LICENSE` & `khl-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `khl-1.0.7/README.md` & `khl-2.0.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ## Usage
 
 To get started right away with basic usage:
 
 ```python
 from khl import text_to_codes
 
-lemmas_coder = {
+coder = {
     '': 0,     # placeholder
     '???': 1,  # unknown
     '.': 2,
     'и': 3,
     'в': 4,
     '-': 5,
     ':': 6,
@@ -48,32 +48,32 @@
 text = """
     1 апреля 2023 года в Москве в матче ⅛ финала против „Спартака” Иван Иванов забил свой 100—й гол за карьеру.
     «Динамо Мск» - «Спартак» 2:1 ОТ (1:0 0:1 0:0 1:0) Голы забили: Иванов, Петров и Сидоров.
 """
 
 codes = text_to_codes(
     text=text,
-    lemmas_coder=lemmas_coder,
-    stop_words_=["в", "за", "и", "свой"],  # stop words to drop
-    replace_ners_=True,                    # replace named entities ("Иван Иванов" -> "per", "Спартак" -> "org", "Москва" -> "loc")
-    replace_dates_=True,                   # replace dates ("1 апреля 2023 года" -> "date")
-    replace_penalties_=True,               # replace penalties ("5+20" -> "pen")
-    exclude_unknown=True,                  # drop lemma that not presented in lemmas_coder
-    max_len=20,                            # get sequence of codes of length 20
+    coder=coder,
+    stop_words_=["за", "и", "свой"],  # stop words to drop
+    replace_ners_=True,               # replace named entities ("Иван Иванов" -> "per", "Спартак" -> "org", "Москва" -> "loc")
+    replace_dates_=True,              # replace dates ("1 апреля 2023 года" -> "date")
+    replace_penalties_=True,          # replace penalties ("5+20" -> "pen")
+    exclude_unknown=True,             # drop lemma that not presented in coder
+    max_len=20,                       # get sequence of codes of length 20
 )
-# codes = [0, 0, 0, 0, 0, 14, 13, 7, 15, 12, 11, 9, 10, 2, 18, 10, 9, 6, 17, 2]
+# codes = [0, 0, 0, 14, 4, 13, 4, 7, 15, 12, 11, 9, 10, 2, 18, 10, 9, 6, 17, 2]
 ```
 
 ```text_to_codes``` is a very high level function. What's happens under hood see in [Lower level usage](#lower-level-usage).
 
-## What is `lemmas_coder`?
-`lemmas_coder` is just a dictionary where each lemma is represented with unique integer code.
+## What is `coder`?
+`coder` is just a dictionary where each lemma is represented with unique integer code.
 Note that first two elements are reserved for *placeholder* and *unknown* elements.
 
-It is possible to get `lemmas_coder` from frequency dictionary file (see in [Get lemmas coder](#2-get-lemmas-coder)).
+It is possible to get `coder` from frequency dictionary file (see in [Get lemmas coder](#2-get-lemmas-coder)).
 Frequency dictionary file is a **json**-file with dictionary where key is lemma and value is how many times this lemma occurred in your whole dataset.
 Preferably it should be sorted in descending order of values.  
 `example_frequency_dictionary.json`:
 
 ```json
 {
   ".": 1000,
@@ -106,59 +106,59 @@
 from khl import stop_words
 from khl import utils
 from khl import preprocess
 ```
 
 #### 2. Get lemmas coder<a id="2-get-lemmas-coder"></a>
 ```python
-lemmas_coder = preprocess.get_lemmas_coder("example_frequency_dictionary.json")
+coder = preprocess.get_coder("example_frequency_dictionary.json")
 ```
 
 #### 3. Define text
 ```python
 text = """
     1 апреля 2023 года в Москве в матче ⅛ финала против „Спартака” Иван Иванов забил свой 100—й гол за карьеру.
     «Динамо Мск» - «Спартак» 2:1 ОТ (1:0 0:1 0:0 1:0) Голы забили: Иванов, Петров и Сидоров.
 """
 ```
 
 #### 4. Unify
 ```python
-unified_text = utils.unify_text(text)
+unified_text = utils.unify(text)
 # "1 апреля 2023 года в Москве в матче 1/8 финала против 'Спартака' Иван Иванов забил свой 100-й гол за карьеру. 'Динамо Мск' - 'Спартак' 2:1 ОТ (1:0 0:1 0:0 1:0) Голы забили: Иванов, Петров и Сидоров."
 ```
 
 #### 5. Simplify
 ```python
-simplified_text = utils.simplify_text(
+simplified_text = utils.simplify(
     text=unified_text,
     replace_ners_=True,
     replace_dates_=True,
     replace_penalties_=True,
 )
 # 'date в loc в матче финала против org per забил свой гол за карьеру. org org Голы забили: per per per.'
 ```
 
 #### 6. Lemmatize
 ```python
 lemmas = preprocess.lemmatize(text=simplified_text, stop_words_=stop_words)
-# ['date', 'loc', 'матч', 'финал', 'против', 'org', 'per', 'забить', 'гол', 'карьера', '.', 'orgs', 'гол', 'забить', ':', 'pers', '.']
+# ['date', 'в', 'loc', 'в', 'матч', 'финал', 'против', 'org', 'per', 'забить', 'гол', 'карьера', '.', 'orgs', 'гол', 'забить', ':', 'pers', '.']
 ```
 
 #### 7. Transform to codes
 ```python
 codes = preprocess.lemmas_to_codes(
     lemmas=lemmas,
-    lemmas_coder=lemmas_coder,
+    coder=coder,
     exclude_unknown=True,
     max_len=20,
 )
-# [0, 0, 0, 0, 0, 14, 13, 7, 15, 12, 11, 9, 10, 2, 18, 10, 9, 6, 17, 2]
+# [0, 0, 0, 14, 4, 13, 4, 7, 15, 12, 11, 9, 10, 2, 18, 10, 9, 6, 17, 2]
 ```
 
 #### 8. Transform to lemmas back (just to look which lemmas are presented in codes sequence)
 ```python
 print(
-    preprocess.codes_to_lemmas(codes=codes, lemmas_coder=lemmas_coder)
+    preprocess.codes_to_lemmas(codes=codes, coder=coder)
 )
-# ['', '', '', '', '', 'date', 'loc', 'матч', 'против', 'org', 'per', 'забить', 'гол', '.', 'orgs', 'гол', 'забить', ':', 'pers', '.']
+# ['', '', '', 'date', 'в', 'loc', 'в', 'матч', 'против', 'org', 'per', 'забить', 'гол', '.', 'orgs', 'гол', 'забить', ':', 'pers', '.']
 ```
```

### Comparing `khl-1.0.7/khl/__init__.py` & `khl-2.0.0/khl/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 """Подготовка русскоязычных текстов хоккейных новостей для обучения нейронных сетей."""
 
-__version__ = "1.0.7"
+__version__ = "2.0.0"
 
 from typing import Dict, List, Optional
 
 from khl import preprocess, utils
 from khl.stop_words import stop_words
 
 
 def text_to_codes(
     text: str,
-    lemmas_coder: Dict[preprocess.Lemma, preprocess.Code],
+    coder: Dict[preprocess.Lemma, preprocess.Code],
     stop_words_: Optional[List[preprocess.Lemma]] = stop_words,
     replace_ners_: bool = True,
     replace_dates_: bool = True,
     replace_penalties_: bool = True,
     exclude_unknown: bool = True,
     max_len: Optional[int] = None,
 ) -> List[preprocess.Code]:
     """
     Преобразует текст в последовательность кодов.
 
     args:
       text: текст новости
-      lemmas_coder: словарь, в котором каждая лемма однозначно
+      coder: словарь, в котором каждая лемма однозначно
         идентифицируется со своим целочисленным кодом
       stop_words_: стоп-слова для исключения
       replace_ners_: если True, то в тексте имена людей заменяются на
         слово 'per', названия команд заменяются на слово 'org',
         названия городов заменяются на слово 'loc'
       replace_dates_: если True, то в тексте даты заменяются на слово 'date'
       replace_penalties_: если True, то в тексте удаления вида '2+10'
         заменяются на слово 'pen'
       exclude_unknown: если True, то слова, которых нет в частотном словаре,
         отбрасываются; если False, то слова, которых нет в частотном словаре,
         заменяются на код неизвестного слова
       max_len: длина последовательности на выходе
     """
-    text = utils.unify_text(text)
-    text = utils.simplify_text(text, replace_ners_, replace_dates_, replace_penalties_)
+    text = utils.unify(text)
+    text = utils.simplify(text, replace_ners_, replace_dates_, replace_penalties_)
     lemmas = preprocess.lemmatize(text, stop_words_)
-    codes = preprocess.lemmas_to_codes(lemmas, lemmas_coder, exclude_unknown, max_len)
+    codes = preprocess.lemmas_to_codes(lemmas, coder, exclude_unknown, max_len)
     return codes
```

### Comparing `khl-1.0.7/khl/preprocess.py` & `khl-2.0.0/khl/preprocess.py`

 * *Files 13% similar despite different names*

```diff
@@ -156,64 +156,64 @@
     [10, 10, 200, 200, 200] -> [10, 200].
     """
     return [code for code, _ in groupby(codes)]
 
 
 def lemmas_to_codes(
     lemmas: List[Lemma],
-    lemmas_coder: Dict[Lemma, Code],
+    coder: Dict[Lemma, Code],
     exclude_unknown: bool = True,
     max_len: Optional[int] = None,
 ) -> List[Code]:
     """
     Преобразует последовательность лемм в последовательность их кодов.
 
     exclude_unknown:
       если True, то леммы, которых нет в частотном словаре, отбрасываются;
       если False, то для лемм, которых нет в частотном словаре,
         проставляется код неизвестного слова
     """
     codes = []
     for lemma in lemmas:
         if not exclude_unknown:
-            codes.append(lemmas_coder.get(lemma, lemmas_coder[UNKNOWN]))
-        elif lemma in lemmas_coder:
-            codes.append(lemmas_coder[lemma])
+            codes.append(coder.get(lemma, coder[UNKNOWN]))
+        elif lemma in coder:
+            codes.append(coder[lemma])
         else:
             continue
     codes = _merge_codes(codes)
     if max_len is None:
         return codes
     elif len(codes) >= max_len:  # pragma: no mutate
         return codes[:max_len]
     else:
-        return _fill_placeholders(codes, lemmas_coder, max_len)
+        return _fill_placeholders(codes, coder, max_len)
 
 
 def _fill_placeholders(
     codes: List[Code],
-    lemmas_coder: Dict[Lemma, Code],
+    coder: Dict[Lemma, Code],
     max_len: int,
 ) -> List[Code]:
     """Заполняет список кодов символами-заполнителями."""
-    filled_codes = [lemmas_coder[PLACEHOLDER]] * (max_len - len(codes))
+    filled_codes = [coder[PLACEHOLDER]] * (max_len - len(codes))
     filled_codes.extend(codes)
     return filled_codes
 
 
-def codes_to_lemmas(codes: List[Code], lemmas_coder: Dict[Lemma, Code]) -> List[Lemma]:
+def codes_to_lemmas(codes: List[Code], coder: Dict[Lemma, Code]) -> List[Lemma]:
     """Преобразует последовательность кодов в последовательность их лемм."""
-    reversed_lemmas_coder = {value: key for key, value in lemmas_coder.items()}
+    reversed_coder = {value: key for key, value in coder.items()}
     lemmas = []
     for code in codes:
-        lemmas.append(reversed_lemmas_coder[code])
+        lemmas.append(reversed_coder[code])
     return lemmas
 
 
-def get_lemmas_coder(frequency_dictionary_file: Union[Path, str]) -> Dict[Lemma, Code]:
+def get_coder(frequency_dictionary_file: Union[Path, str]) -> Dict[Lemma, Code]:
     """
     Получение словаря кодового представления лемм из частотного словаря лемм.
 
     frequency_dictionary_file - частотный словарь лемм:
       json-ка со словарем, где ключи - леммы,
       а значения - сколько раз данная лемма встретилась во всем датасете.
       Желательно, чтобы данный словарь был отсортирован в порядке убывания значений.
@@ -221,13 +221,13 @@
       {".": 1000, "и": 500, "команда": 200, "гол": 100}
 
     Возвращает словарь (кодер), в котором каждой лемме присвоен свой уникальный код.
     Первые 2 элемента кодера зарезервированы:
       0 - символ-заполнитель
       1 - неизвестное слово
     """
-    lemmas_coder = {PLACEHOLDER: 0, UNKNOWN: 1}
+    coder = {PLACEHOLDER: 0, UNKNOWN: 1}
     with open(frequency_dictionary_file, "r", encoding="utf-8") as fr:
         freq_dict = json.load(fr)
-    for freq, word in enumerate(freq_dict, len(lemmas_coder)):
-        lemmas_coder[word] = freq
-    return lemmas_coder
+    for freq, word in enumerate(freq_dict, len(coder)):
+        coder[word] = freq
+    return coder
```

### Comparing `khl-1.0.7/khl/stop_words.py` & `khl-2.0.0/khl/stop_words.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
     "а",
     "абсолютно",
     "аж",
     "более",
     "больше",
     "бы",
     "быстро",
-    "в",
     "во",
     "ведь",
     "весь",
     "вместе",
     "вновь",
     "вовсе",
     "вообще",
```

### Comparing `khl-1.0.7/khl/teams_orgs.py` & `khl-2.0.0/khl/teams_orgs.py`

 * *Files identical despite different names*

### Comparing `khl-1.0.7/khl/utils.py` & `khl-2.0.0/khl/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 segmenter = Segmenter()
 morph_vocab = MorphVocab()  # pragma: no mutate
 emb = NewsEmbedding()  # pragma: no mutate
 ner_tagger = NewsNERTagger(emb)
 
 
-def unify_text(text: str) -> str:
+def unify(text: str) -> str:
     """Приведение текстов новостей к единому виду."""
     for symbol in ['"', "`", "«", "»", "„", "“", "”"]:
         text = text.replace(symbol, "'")
     for symbol in ["—", "–", "−"]:
         text = text.replace(symbol, "-")
     text = (
         text.replace("⅛", "1/8")
@@ -710,28 +710,28 @@
 
 
 def delete_ending_colon_dash(text: str) -> str:
     """'Текст : - ' -> 'Текст'."""
     return text.rstrip(" -:")
 
 
-def simplify_text(
+def simplify(
     text: str,
     replace_ners_: bool = True,
     replace_dates_: bool = True,
     replace_penalties_: bool = True,
 ) -> str:
     """
     Упрощение текста хоккейной новости.
 
     Избавление от элементов текста новости, не несущих
     особой смысловой нагрузки для машинного обучения.
 
     Пример использования:
-      simplify_text(
+      simplify(
         text="1 января 2020 года Иван Иванов в Москве забил гол в ворота Спартака, а также заработал 5+10 за грубость",  # noqa
         replace_ners_=True,
         replace_dates_=True,
         replace_penalties=True,
       ) -> "date per в loc забил гол в ворота org а также заработал pen за грубость"
 
     Последовательность действий:
```

### Comparing `khl-1.0.7/khl/wrong_lemmas.py` & `khl-2.0.0/khl/wrong_lemmas.py`

 * *Files identical despite different names*

### Comparing `khl-1.0.7/pyproject.toml` & `khl-2.0.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "khl"
-version = "1.0.7"
+version = "2.0.0"
 description = "Preparing russian hockey news for machine learning"
 readme = "README.md"
 license = "MIT"
 authors = ["Rishat Fayzullin <nilluziaf@gmail.com>"]
 repository = "https://github.com/Rishat-F/khl"
 keywords = ["khl", "news", "nlp", "preprocessing", "ml"]
```

### Comparing `khl-1.0.7/setup.py` & `khl-2.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['natasha==1.4.0']
 
 setup_kwargs = {
     'name': 'khl',
-    'version': '1.0.7',
+    'version': '2.0.0',
     'description': 'Preparing russian hockey news for machine learning',
-    'long_description': '![Khl Logo](https://raw.githubusercontent.com/Rishat-F/khl/master/data/logo.png)\n\n<h1 align="center">No Water - Ice Only</h1>\n\nPreparing russian hockey news for machine learning.\n\n**Unify -> Simplify -> Preprocess** text and feed your neural model.\n\n## Installation\n\n*Khl* is available on PyPI:\n\n```console\n$ pip install khl\n```\nIt requires Python 3.8+ to run.\n\n## Usage\n\nTo get started right away with basic usage:\n\n```python\nfrom khl import text_to_codes\n\nlemmas_coder = {\n    \'\': 0,     # placeholder\n    \'???\': 1,  # unknown\n    \'.\': 2,\n    \'и\': 3,\n    \'в\': 4,\n    \'-\': 5,\n    \':\': 6,\n    \'матч\': 7,\n    \'за\': 8,\n    \'забить\': 9,\n    \'гол\': 10,\n    \'per\': 11,   # person entity\n    \'org\': 12,   # organization entity\n    \'loc\': 13,   # location entity\n    \'date\': 14,  # date entity\n    \'против\': 15,\n    \'год\': 16,\n    \'pers\': 17,  # few persons entity\n    \'orgs\': 18,  # few organizations entity\n    \'свой\': 19\n}\n\ntext = """\n    1 апреля 2023 года в Москве в матче ⅛ финала против „Спартака” Иван Иванов забил свой 100—й гол за карьеру.\n    «Динамо Мск» - «Спартак» 2:1 ОТ (1:0 0:1 0:0 1:0) Голы забили: Иванов, Петров и Сидоров.\n"""\n\ncodes = text_to_codes(\n    text=text,\n    lemmas_coder=lemmas_coder,\n    stop_words_=["в", "за", "и", "свой"],  # stop words to drop\n    replace_ners_=True,                    # replace named entities ("Иван Иванов" -> "per", "Спартак" -> "org", "Москва" -> "loc")\n    replace_dates_=True,                   # replace dates ("1 апреля 2023 года" -> "date")\n    replace_penalties_=True,               # replace penalties ("5+20" -> "pen")\n    exclude_unknown=True,                  # drop lemma that not presented in lemmas_coder\n    max_len=20,                            # get sequence of codes of length 20\n)\n# codes = [0, 0, 0, 0, 0, 14, 13, 7, 15, 12, 11, 9, 10, 2, 18, 10, 9, 6, 17, 2]\n```\n\n```text_to_codes``` is a very high level function. What\'s happens under hood see in [Lower level usage](#lower-level-usage).\n\n## What is `lemmas_coder`?\n`lemmas_coder` is just a dictionary where each lemma is represented with unique integer code.\nNote that first two elements are reserved for *placeholder* and *unknown* elements.\n\nIt is possible to get `lemmas_coder` from frequency dictionary file (see in [Get lemmas coder](#2-get-lemmas-coder)).\nFrequency dictionary file is a **json**-file with dictionary where key is lemma and value is how many times this lemma occurred in your whole dataset.\nPreferably it should be sorted in descending order of values.  \n`example_frequency_dictionary.json`:\n\n```json\n{\n  ".": 1000,\n  "и": 500,\n  "в": 400,\n  "-": 300,\n  ":": 300,\n  "матч": 290,\n  "за": 250,\n  "забить": 240,\n  "гол": 230,\n  "per": 200,\n  "org": 150,\n  "loc": 150,\n  "date": 100,\n  "против": 90,\n  "год": 70,\n  "pers": 40,\n  "orgs": 30,\n  "свой": 20\n}\n```\n\nYou could make and use your own frequency dictionary or download [this dictionary](https://github.com/Rishat-F/khl/blob/master/data/frequency_dictionary.json) created by myself.\n\n## Lower level usage<a id="lower-level-usage"></a>\n\n#### 1. Make imports\n```python\nfrom khl import stop_words\nfrom khl import utils\nfrom khl import preprocess\n```\n\n#### 2. Get lemmas coder<a id="2-get-lemmas-coder"></a>\n```python\nlemmas_coder = preprocess.get_lemmas_coder("example_frequency_dictionary.json")\n```\n\n#### 3. Define text\n```python\ntext = """\n    1 апреля 2023 года в Москве в матче ⅛ финала против „Спартака” Иван Иванов забил свой 100—й гол за карьеру.\n    «Динамо Мск» - «Спартак» 2:1 ОТ (1:0 0:1 0:0 1:0) Голы забили: Иванов, Петров и Сидоров.\n"""\n```\n\n#### 4. Unify\n```python\nunified_text = utils.unify_text(text)\n# "1 апреля 2023 года в Москве в матче 1/8 финала против \'Спартака\' Иван Иванов забил свой 100-й гол за карьеру. \'Динамо Мск\' - \'Спартак\' 2:1 ОТ (1:0 0:1 0:0 1:0) Голы забили: Иванов, Петров и Сидоров."\n```\n\n#### 5. Simplify\n```python\nsimplified_text = utils.simplify_text(\n    text=unified_text,\n    replace_ners_=True,\n    replace_dates_=True,\n    replace_penalties_=True,\n)\n# \'date в loc в матче финала против org per забил свой гол за карьеру. org org Голы забили: per per per.\'\n```\n\n#### 6. Lemmatize\n```python\nlemmas = preprocess.lemmatize(text=simplified_text, stop_words_=stop_words)\n# [\'date\', \'loc\', \'матч\', \'финал\', \'против\', \'org\', \'per\', \'забить\', \'гол\', \'карьера\', \'.\', \'orgs\', \'гол\', \'забить\', \':\', \'pers\', \'.\']\n```\n\n#### 7. Transform to codes\n```python\ncodes = preprocess.lemmas_to_codes(\n    lemmas=lemmas,\n    lemmas_coder=lemmas_coder,\n    exclude_unknown=True,\n    max_len=20,\n)\n# [0, 0, 0, 0, 0, 14, 13, 7, 15, 12, 11, 9, 10, 2, 18, 10, 9, 6, 17, 2]\n```\n\n#### 8. Transform to lemmas back (just to look which lemmas are presented in codes sequence)\n```python\nprint(\n    preprocess.codes_to_lemmas(codes=codes, lemmas_coder=lemmas_coder)\n)\n# [\'\', \'\', \'\', \'\', \'\', \'date\', \'loc\', \'матч\', \'против\', \'org\', \'per\', \'забить\', \'гол\', \'.\', \'orgs\', \'гол\', \'забить\', \':\', \'pers\', \'.\']\n```\n',
+    'long_description': '![Khl Logo](https://raw.githubusercontent.com/Rishat-F/khl/master/data/logo.png)\n\n<h1 align="center">No Water - Ice Only</h1>\n\nPreparing russian hockey news for machine learning.\n\n**Unify -> Simplify -> Preprocess** text and feed your neural model.\n\n## Installation\n\n*Khl* is available on PyPI:\n\n```console\n$ pip install khl\n```\nIt requires Python 3.8+ to run.\n\n## Usage\n\nTo get started right away with basic usage:\n\n```python\nfrom khl import text_to_codes\n\ncoder = {\n    \'\': 0,     # placeholder\n    \'???\': 1,  # unknown\n    \'.\': 2,\n    \'и\': 3,\n    \'в\': 4,\n    \'-\': 5,\n    \':\': 6,\n    \'матч\': 7,\n    \'за\': 8,\n    \'забить\': 9,\n    \'гол\': 10,\n    \'per\': 11,   # person entity\n    \'org\': 12,   # organization entity\n    \'loc\': 13,   # location entity\n    \'date\': 14,  # date entity\n    \'против\': 15,\n    \'год\': 16,\n    \'pers\': 17,  # few persons entity\n    \'orgs\': 18,  # few organizations entity\n    \'свой\': 19\n}\n\ntext = """\n    1 апреля 2023 года в Москве в матче ⅛ финала против „Спартака” Иван Иванов забил свой 100—й гол за карьеру.\n    «Динамо Мск» - «Спартак» 2:1 ОТ (1:0 0:1 0:0 1:0) Голы забили: Иванов, Петров и Сидоров.\n"""\n\ncodes = text_to_codes(\n    text=text,\n    coder=coder,\n    stop_words_=["за", "и", "свой"],  # stop words to drop\n    replace_ners_=True,               # replace named entities ("Иван Иванов" -> "per", "Спартак" -> "org", "Москва" -> "loc")\n    replace_dates_=True,              # replace dates ("1 апреля 2023 года" -> "date")\n    replace_penalties_=True,          # replace penalties ("5+20" -> "pen")\n    exclude_unknown=True,             # drop lemma that not presented in coder\n    max_len=20,                       # get sequence of codes of length 20\n)\n# codes = [0, 0, 0, 14, 4, 13, 4, 7, 15, 12, 11, 9, 10, 2, 18, 10, 9, 6, 17, 2]\n```\n\n```text_to_codes``` is a very high level function. What\'s happens under hood see in [Lower level usage](#lower-level-usage).\n\n## What is `coder`?\n`coder` is just a dictionary where each lemma is represented with unique integer code.\nNote that first two elements are reserved for *placeholder* and *unknown* elements.\n\nIt is possible to get `coder` from frequency dictionary file (see in [Get lemmas coder](#2-get-lemmas-coder)).\nFrequency dictionary file is a **json**-file with dictionary where key is lemma and value is how many times this lemma occurred in your whole dataset.\nPreferably it should be sorted in descending order of values.  \n`example_frequency_dictionary.json`:\n\n```json\n{\n  ".": 1000,\n  "и": 500,\n  "в": 400,\n  "-": 300,\n  ":": 300,\n  "матч": 290,\n  "за": 250,\n  "забить": 240,\n  "гол": 230,\n  "per": 200,\n  "org": 150,\n  "loc": 150,\n  "date": 100,\n  "против": 90,\n  "год": 70,\n  "pers": 40,\n  "orgs": 30,\n  "свой": 20\n}\n```\n\nYou could make and use your own frequency dictionary or download [this dictionary](https://github.com/Rishat-F/khl/blob/master/data/frequency_dictionary.json) created by myself.\n\n## Lower level usage<a id="lower-level-usage"></a>\n\n#### 1. Make imports\n```python\nfrom khl import stop_words\nfrom khl import utils\nfrom khl import preprocess\n```\n\n#### 2. Get lemmas coder<a id="2-get-lemmas-coder"></a>\n```python\ncoder = preprocess.get_coder("example_frequency_dictionary.json")\n```\n\n#### 3. Define text\n```python\ntext = """\n    1 апреля 2023 года в Москве в матче ⅛ финала против „Спартака” Иван Иванов забил свой 100—й гол за карьеру.\n    «Динамо Мск» - «Спартак» 2:1 ОТ (1:0 0:1 0:0 1:0) Голы забили: Иванов, Петров и Сидоров.\n"""\n```\n\n#### 4. Unify\n```python\nunified_text = utils.unify(text)\n# "1 апреля 2023 года в Москве в матче 1/8 финала против \'Спартака\' Иван Иванов забил свой 100-й гол за карьеру. \'Динамо Мск\' - \'Спартак\' 2:1 ОТ (1:0 0:1 0:0 1:0) Голы забили: Иванов, Петров и Сидоров."\n```\n\n#### 5. Simplify\n```python\nsimplified_text = utils.simplify(\n    text=unified_text,\n    replace_ners_=True,\n    replace_dates_=True,\n    replace_penalties_=True,\n)\n# \'date в loc в матче финала против org per забил свой гол за карьеру. org org Голы забили: per per per.\'\n```\n\n#### 6. Lemmatize\n```python\nlemmas = preprocess.lemmatize(text=simplified_text, stop_words_=stop_words)\n# [\'date\', \'в\', \'loc\', \'в\', \'матч\', \'финал\', \'против\', \'org\', \'per\', \'забить\', \'гол\', \'карьера\', \'.\', \'orgs\', \'гол\', \'забить\', \':\', \'pers\', \'.\']\n```\n\n#### 7. Transform to codes\n```python\ncodes = preprocess.lemmas_to_codes(\n    lemmas=lemmas,\n    coder=coder,\n    exclude_unknown=True,\n    max_len=20,\n)\n# [0, 0, 0, 14, 4, 13, 4, 7, 15, 12, 11, 9, 10, 2, 18, 10, 9, 6, 17, 2]\n```\n\n#### 8. Transform to lemmas back (just to look which lemmas are presented in codes sequence)\n```python\nprint(\n    preprocess.codes_to_lemmas(codes=codes, coder=coder)\n)\n# [\'\', \'\', \'\', \'date\', \'в\', \'loc\', \'в\', \'матч\', \'против\', \'org\', \'per\', \'забить\', \'гол\', \'.\', \'orgs\', \'гол\', \'забить\', \':\', \'pers\', \'.\']\n```\n',
     'author': 'Rishat Fayzullin',
     'author_email': 'nilluziaf@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Rishat-F/khl',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `khl-1.0.7/PKG-INFO` & `khl-2.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khl
-Version: 1.0.7
+Version: 2.0.0
 Summary: Preparing russian hockey news for machine learning
 Home-page: https://github.com/Rishat-F/khl
 License: MIT
 Keywords: khl,news,nlp,preprocessing,ml
 Author: Rishat Fayzullin
 Author-email: nilluziaf@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -38,15 +38,15 @@
 ## Usage
 
 To get started right away with basic usage:
 
 ```python
 from khl import text_to_codes
 
-lemmas_coder = {
+coder = {
     '': 0,     # placeholder
     '???': 1,  # unknown
     '.': 2,
     'и': 3,
     'в': 4,
     '-': 5,
     ':': 6,
@@ -68,32 +68,32 @@
 text = """
     1 апреля 2023 года в Москве в матче ⅛ финала против „Спартака” Иван Иванов забил свой 100—й гол за карьеру.
     «Динамо Мск» - «Спартак» 2:1 ОТ (1:0 0:1 0:0 1:0) Голы забили: Иванов, Петров и Сидоров.
 """
 
 codes = text_to_codes(
     text=text,
-    lemmas_coder=lemmas_coder,
-    stop_words_=["в", "за", "и", "свой"],  # stop words to drop
-    replace_ners_=True,                    # replace named entities ("Иван Иванов" -> "per", "Спартак" -> "org", "Москва" -> "loc")
-    replace_dates_=True,                   # replace dates ("1 апреля 2023 года" -> "date")
-    replace_penalties_=True,               # replace penalties ("5+20" -> "pen")
-    exclude_unknown=True,                  # drop lemma that not presented in lemmas_coder
-    max_len=20,                            # get sequence of codes of length 20
+    coder=coder,
+    stop_words_=["за", "и", "свой"],  # stop words to drop
+    replace_ners_=True,               # replace named entities ("Иван Иванов" -> "per", "Спартак" -> "org", "Москва" -> "loc")
+    replace_dates_=True,              # replace dates ("1 апреля 2023 года" -> "date")
+    replace_penalties_=True,          # replace penalties ("5+20" -> "pen")
+    exclude_unknown=True,             # drop lemma that not presented in coder
+    max_len=20,                       # get sequence of codes of length 20
 )
-# codes = [0, 0, 0, 0, 0, 14, 13, 7, 15, 12, 11, 9, 10, 2, 18, 10, 9, 6, 17, 2]
+# codes = [0, 0, 0, 14, 4, 13, 4, 7, 15, 12, 11, 9, 10, 2, 18, 10, 9, 6, 17, 2]
 ```
 
 ```text_to_codes``` is a very high level function. What's happens under hood see in [Lower level usage](#lower-level-usage).
 
-## What is `lemmas_coder`?
-`lemmas_coder` is just a dictionary where each lemma is represented with unique integer code.
+## What is `coder`?
+`coder` is just a dictionary where each lemma is represented with unique integer code.
 Note that first two elements are reserved for *placeholder* and *unknown* elements.
 
-It is possible to get `lemmas_coder` from frequency dictionary file (see in [Get lemmas coder](#2-get-lemmas-coder)).
+It is possible to get `coder` from frequency dictionary file (see in [Get lemmas coder](#2-get-lemmas-coder)).
 Frequency dictionary file is a **json**-file with dictionary where key is lemma and value is how many times this lemma occurred in your whole dataset.
 Preferably it should be sorted in descending order of values.  
 `example_frequency_dictionary.json`:
 
 ```json
 {
   ".": 1000,
@@ -126,60 +126,60 @@
 from khl import stop_words
 from khl import utils
 from khl import preprocess
 ```
 
 #### 2. Get lemmas coder<a id="2-get-lemmas-coder"></a>
 ```python
-lemmas_coder = preprocess.get_lemmas_coder("example_frequency_dictionary.json")
+coder = preprocess.get_coder("example_frequency_dictionary.json")
 ```
 
 #### 3. Define text
 ```python
 text = """
     1 апреля 2023 года в Москве в матче ⅛ финала против „Спартака” Иван Иванов забил свой 100—й гол за карьеру.
     «Динамо Мск» - «Спартак» 2:1 ОТ (1:0 0:1 0:0 1:0) Голы забили: Иванов, Петров и Сидоров.
 """
 ```
 
 #### 4. Unify
 ```python
-unified_text = utils.unify_text(text)
+unified_text = utils.unify(text)
 # "1 апреля 2023 года в Москве в матче 1/8 финала против 'Спартака' Иван Иванов забил свой 100-й гол за карьеру. 'Динамо Мск' - 'Спартак' 2:1 ОТ (1:0 0:1 0:0 1:0) Голы забили: Иванов, Петров и Сидоров."
 ```
 
 #### 5. Simplify
 ```python
-simplified_text = utils.simplify_text(
+simplified_text = utils.simplify(
     text=unified_text,
     replace_ners_=True,
     replace_dates_=True,
     replace_penalties_=True,
 )
 # 'date в loc в матче финала против org per забил свой гол за карьеру. org org Голы забили: per per per.'
 ```
 
 #### 6. Lemmatize
 ```python
 lemmas = preprocess.lemmatize(text=simplified_text, stop_words_=stop_words)
-# ['date', 'loc', 'матч', 'финал', 'против', 'org', 'per', 'забить', 'гол', 'карьера', '.', 'orgs', 'гол', 'забить', ':', 'pers', '.']
+# ['date', 'в', 'loc', 'в', 'матч', 'финал', 'против', 'org', 'per', 'забить', 'гол', 'карьера', '.', 'orgs', 'гол', 'забить', ':', 'pers', '.']
 ```
 
 #### 7. Transform to codes
 ```python
 codes = preprocess.lemmas_to_codes(
     lemmas=lemmas,
-    lemmas_coder=lemmas_coder,
+    coder=coder,
     exclude_unknown=True,
     max_len=20,
 )
-# [0, 0, 0, 0, 0, 14, 13, 7, 15, 12, 11, 9, 10, 2, 18, 10, 9, 6, 17, 2]
+# [0, 0, 0, 14, 4, 13, 4, 7, 15, 12, 11, 9, 10, 2, 18, 10, 9, 6, 17, 2]
 ```
 
 #### 8. Transform to lemmas back (just to look which lemmas are presented in codes sequence)
 ```python
 print(
-    preprocess.codes_to_lemmas(codes=codes, lemmas_coder=lemmas_coder)
+    preprocess.codes_to_lemmas(codes=codes, coder=coder)
 )
-# ['', '', '', '', '', 'date', 'loc', 'матч', 'против', 'org', 'per', 'забить', 'гол', '.', 'orgs', 'гол', 'забить', ':', 'pers', '.']
+# ['', '', '', 'date', 'в', 'loc', 'в', 'матч', 'против', 'org', 'per', 'забить', 'гол', '.', 'orgs', 'гол', 'забить', ':', 'pers', '.']
 ```
```

