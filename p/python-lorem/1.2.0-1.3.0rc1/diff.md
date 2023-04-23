# Comparing `tmp/python-lorem-1.2.0.tar.gz` & `tmp/python-lorem-1.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-lorem-1.2.0.tar", last modified: Tue Nov  1 02:04:31 2022, max compression
+gzip compressed data, was "python-lorem-1.3.0rc1.tar", last modified: Sun Apr 23 06:32:02 2023, max compression
```

## Comparing `python-lorem-1.2.0.tar` & `python-lorem-1.3.0rc1.tar`

### file list

```diff
@@ -1,19 +1,17 @@
-drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2022-11-01 02:04:31.576965 python-lorem-1.2.0/
--rw-r--r--   0 jarryshaw   (501) staff       (20)     1518 2019-09-26 13:31:00.000000 python-lorem-1.2.0/LICENSE
--rw-r--r--   0 jarryshaw   (501) staff       (20)      131 2019-09-27 11:37:20.000000 python-lorem-1.2.0/MANIFEST.in
--rw-r--r--   0 jarryshaw   (501) staff       (20)     3344 2022-11-01 02:04:31.577174 python-lorem-1.2.0/PKG-INFO
--rw-r--r--   0 jarryshaw   (501) staff       (20)     2765 2022-11-01 01:57:16.000000 python-lorem-1.2.0/README.md
-drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2022-11-01 02:04:31.568901 python-lorem-1.2.0/docs/
-drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2022-11-01 02:04:31.574245 python-lorem-1.2.0/docs/source/
--rw-r--r--   0 jarryshaw   (501) staff       (20)     3198 2022-11-01 01:59:18.000000 python-lorem-1.2.0/docs/source/conf.py
--rw-r--r--   0 jarryshaw   (501) staff       (20)    17466 2022-11-01 01:55:37.000000 python-lorem-1.2.0/lorem.py
--rw-r--r--   0 jarryshaw   (501) staff       (20)      100 2020-10-07 16:54:20.000000 python-lorem-1.2.0/pyproject.toml
-drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2022-11-01 02:04:31.576543 python-lorem-1.2.0/python_lorem.egg-info/
--rw-r--r--   0 jarryshaw   (501) staff       (20)     3344 2022-11-01 02:04:29.000000 python-lorem-1.2.0/python_lorem.egg-info/PKG-INFO
--rw-r--r--   0 jarryshaw   (501) staff       (20)      281 2022-11-01 02:04:31.000000 python-lorem-1.2.0/python_lorem.egg-info/SOURCES.txt
--rw-r--r--   0 jarryshaw   (501) staff       (20)        1 2022-11-01 02:04:29.000000 python-lorem-1.2.0/python_lorem.egg-info/dependency_links.txt
--rw-r--r--   0 jarryshaw   (501) staff       (20)       17 2022-11-01 02:04:29.000000 python-lorem-1.2.0/python_lorem.egg-info/top_level.txt
--rw-r--r--   0 jarryshaw   (501) staff       (20)        1 2022-11-01 02:04:29.000000 python-lorem-1.2.0/python_lorem.egg-info/zip-safe
--rw-r--r--   0 jarryshaw   (501) staff       (20)      131 2022-11-01 02:04:31.577705 python-lorem-1.2.0/setup.cfg
--rw-r--r--   0 jarryshaw   (501) staff       (20)     4611 2022-11-01 01:57:35.000000 python-lorem-1.2.0/setup.py
--rw-r--r--   0 jarryshaw   (501) staff       (20)     8420 2022-11-01 02:01:03.000000 python-lorem-1.2.0/test_lorem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:32:02.891667 python-lorem-1.3.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-23 06:31:49.000000 python-lorem-1.3.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-23 06:31:49.000000 python-lorem-1.3.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-04-23 06:32:02.891667 python-lorem-1.3.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-23 06:31:49.000000 python-lorem-1.3.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    17541 2023-04-23 06:31:49.000000 python-lorem-1.3.0rc1/lorem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-04-23 06:31:49.000000 python-lorem-1.3.0rc1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:32:02.891667 python-lorem-1.3.0rc1/python_lorem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-04-23 06:32:02.000000 python-lorem-1.3.0rc1/python_lorem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-23 06:32:02.000000 python-lorem-1.3.0rc1/python_lorem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 06:32:02.000000 python-lorem-1.3.0rc1/python_lorem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-23 06:32:02.000000 python-lorem-1.3.0rc1/python_lorem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-23 06:32:02.000000 python-lorem-1.3.0rc1/python_lorem.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 06:32:02.000000 python-lorem-1.3.0rc1/python_lorem.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-23 06:32:02.891667 python-lorem-1.3.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-04-23 06:31:49.000000 python-lorem-1.3.0rc1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-04-23 06:31:49.000000 python-lorem-1.3.0rc1/test_lorem.py
```

### Comparing `python-lorem-1.2.0/LICENSE` & `python-lorem-1.3.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-lorem-1.2.0/PKG-INFO` & `python-lorem-1.3.0rc1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 Metadata-Version: 2.1
 Name: python-lorem
-Version: 1.2.0
+Version: 1.3.0rc1
 Summary: Lorem ipsum generator.
-Home-page: https://github.com/JarryShaw/lorem
-Download-URL: https://github.com/JarryShaw/lorem/archive/v1.2.0.tar.gz
-Author: Jarry Shaw
-Author-email: jarryshaw@icloud.com
+Author-email: Jarry Shaw <jarryshaw@icloud.com>
 Maintainer: Jarry Shaw
-Maintainer-email: jarryshaw@icloud.com
-License: BSD License
+License: BSD 3-Clause License
+Project-URL: homepage, https://jarryshaw.github.io/lorem/
+Project-URL: documentation, https://jarryshaw.github.io/lorem/
+Project-URL: repository, https://github.com/JarryShaw/lorem
+Project-URL: changelog, https://github.com/JarryShaw/lorem/releases
 Keywords: lorem,loremipsum
-Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
-Obsoletes: lorem
-Obsoletes: loremipsum
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+Provides-Extra: docs
 License-File: LICENSE
 
 Lorem ipsum generator.
 
 In publishing and graphic design, lorem ipsum is a placeholder text commonly
 used to demonstrate the visual form of a document or a typeface without
 relying on meaningful content.
```

### Comparing `python-lorem-1.2.0/README.md` & `python-lorem-1.3.0rc1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -53,14 +53,25 @@
 git pull
 ```
 
 ## Usage
 
 Usage of the `lorem` module is rather simple. Depending on your needs, the
 `lorem` module provides generation of **word**s, **sentence**s, and
-**paragraph**s. Please refer to the [documentation](https://jarryshaw.github.io/lorem/)
+**paragraph**s:
+
+```python
+import lorem
+
+print(lorem.get_sentence(count=3))
+```
+
+> Eu consectetur ad et, exercitation fugiat occaecat exercitation cillum non ullamco, elit mollit est consectetur. In ex proident esse est aute est mollit, id minim lorem tempor sunt elit. Dolor aliqua non eiusmod officia esse adipiscing.
+
+Please refer to the [documentation](https://jarryshaw.github.io/lorem/)
 for more details.
+
 ## Testing
 
 The `lorem` module utilised `unittest.mock` to *patch* the builtin functions
 from `random` module. Test cases can be found in [`test_lorem.py`](test_lorem.py).
 **Contributions are welcome.**
```

### Comparing `python-lorem-1.2.0/lorem.py` & `python-lorem-1.3.0rc1/lorem.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,14 +82,17 @@
 
 __all__ = [
     'LoremGenerator',
     'word', 'sentence', 'paragraph',
     'get_word', 'get_sentence', 'get_paragraph',
 ]
 
+# version string
+__version__ = '1.3.0rc1'
+
 #: The original lorem ipsum text pool.
 _TEXT = ('ad', 'adipiscing', 'aliqua', 'aliquip', 'amet', 'anim', 'aute', 'cillum', 'commodo',
          'consectetur', 'consequat', 'culpa', 'cupidatat', 'deserunt', 'do', 'dolor', 'dolore',
          'duis', 'ea', 'eiusmod', 'elit', 'enim', 'esse', 'est', 'et', 'eu', 'ex', 'excepteur',
          'exercitation', 'fugiat', 'id', 'in', 'incididunt', 'ipsum', 'irure', 'labore', 'laboris',
          'laborum', 'lorem', 'magna', 'minim', 'mollit', 'nisi', 'non', 'nostrud', 'nulla',
          'occaecat', 'officia', 'pariatur', 'proident', 'qui', 'quis', 'reprehenderit', 'sed',
@@ -226,187 +229,187 @@
         """
         text = self.gen_sentence(comma=comma, word_range=word_range)
         for _ in range(random.randint(*sentence_range) - 1):  # nosec B311
             text += ' ' + self.gen_sentence(comma=comma, word_range=word_range)
         return text
 
 
-def word(pool: 'Iterable[str]' = _TEXT, count: int = 1,  # pylint: disable=dangerous-default-value
-         func: 'Optional[str | Callable[[str], str]]' = None,
-         args: 'tuple[str, ...]' = (), kwargs: 'dict[str, Any]' = {}) -> 'Iterator[str]':
+def word(count: int = 1, func: 'Optional[str | Callable[[str], str]]' = None,
+         args: 'tuple[str, ...]' = (), kwargs: 'dict[str, Any]' = {}, *,
+         pool: 'Iterable[str]' = _TEXT,) -> 'Iterator[str]':  # pylint: disable=dangerous-default-value
     """Generate a list of random words.
 
     .. code-block:: python
 
         >>> list(itertools.cycle(word(count=3), 3))
         ['labore', 'tempor', 'commodo']
         >>> list(itertools.cycle(word(count=3, func='capitalize'), 3))
         ['Ea', 'Lorem', 'Do']
         >>> list(itertools.cycle(word(count=3, func=lambda s: s.upper()), 3))
         ['UT', 'AMET', 'EXCEPTEUR']
 
     Args:
-        pool: List of words to be used as random word pool.
         count: Number of non-repeated random words.
         func: Filter function. It can be an attribute name of :obj:`str`, or a customised
             function that takes the original :obj:`str` and returns the modified :obj:`str`.
         args: Additional positional arguments for ``func``.
         kwargs: Additional keyword arguments for ``func``.
+        pool: List of words to be used as random word pool.
 
     Returns:
         Indefinite random words generator.
 
     """
     lorem = LoremGenerator(pool=pool, dupe=count)
     yield from itertools.cycle(lorem.gen_word(func=func,
                                               args=args,
                                               kwargs=kwargs) for _ in range(count))
 
 
-def sentence(pool: 'Iterable[str]' = _TEXT, count: 'int' = 1,
-             comma: 'tuple[int, int]' = (0, 2),
-             word_range: 'tuple[int, int]' = (4, 8)) -> 'Iterator[str]':
+def sentence(count: 'int' = 1, comma: 'tuple[int, int]' = (0, 2),
+             word_range: 'tuple[int, int]' = (4, 8), *,
+             pool: 'Iterable[str]' = _TEXT) -> 'Iterator[str]':
     """Generate a list of random sentences.
 
     .. code-block:: python
 
         >>> list(itertools.islice(sentence(), 1))
         ['Aute irure et commodo sunt do duis dolor.']
 
     Args:
-        pool: List of words to be used as random word pool.
         count: Number of non-repeated random sentences.
         comma: Random range for number of commas. The function will use :func:`random.randint`
             to choose a random integer as the number of commas.
         word_range: Random range for number of words in each sentence. The function will use
             :func:`random.randint` to choose a random integer as the number of words.
+        pool: List of words to be used as random word pool.
 
     Returns:
         Indefinite random sentence generator.
 
     """
     lorem = LoremGenerator(pool=pool, dupe=count)
     yield from _random_cycle(lorem.gen_sentence(comma=comma,
                                                 word_range=word_range) for _ in range(count))
 
 
-def paragraph(pool: 'Iterable[str]' = _TEXT, count: 'int' = 1,
-              comma: 'tuple[int, int]' = (0, 2),
+def paragraph(count: 'int' = 1, comma: 'tuple[int, int]' = (0, 2),
               word_range: 'tuple[int, int]' = (4, 8),
-              sentence_range: 'tuple[int, int]' = (5, 10)) -> 'Iterator[str]':
+              sentence_range: 'tuple[int, int]' = (5, 10), *,
+              pool: 'Iterable[str]' = _TEXT) -> 'Iterator[str]':
     """Generate a list of random paragraphs.
 
     .. code-block:: python
 
         >>> list(itertools.islice(paragraph(), 1))
         ['Aute sint et cupidatat aliquip. Non exercitation est aliquip voluptate '
             'fugiat, reprehenderit ad occaecat laboris velit consequat. Magna enim '
             'deserunt aute laborum fugiat exercitation. Aliqua ex sunt fugiat in '
             'magna voluptate. Elit nisi exercitation nostrud. Magna proident et '
             'fugiat eiusmod cupidatat fugiat, sit culpa fugiat non ea eu '
             'reprehenderit elit. Proident mollit mollit ut cillum. Nostrud voluptate '
             'aliquip cupidatat anim.']
 
     Args:
-        pool: List of words to be used as random word pool.
         count: Number of non-repeated random paragraphs.
         comma: Random range for number of commas. The function will use :func:`random.randint`
             to choose a random integer as the number of commas.
         word_range: Random range for number of words in each sentence. The function will use
             :func:`random.randint` to choose a random integer as the number of words.
         sentence_range: Random range for number of sentences in each paragraph. The function
             will use :func:`random.randint` to choose a random integer as the number of sentences.
+        pool: List of words to be used as random word pool.
 
     Returns:
         Random paragraph generator.
 
     """
     lorem = LoremGenerator(
         pool=pool,
         dupe=count * random.randint(*word_range) * random.randint(*sentence_range),  # nosec B311
     )
     yield from _random_cycle(lorem.gen_paragraph(comma=comma,
                                                  word_range=word_range,
                                                  sentence_range=sentence_range) for _ in range(count))
 
 
-def get_word(pool: 'Iterable[str]' = _TEXT,  # pylint: disable=dangerous-default-value
-             count: 'int | tuple[int, int]' = 1,
+def get_word(count: 'int | tuple[int, int]' = 1,
              sep: 'str' = ' ',
              func: 'Optional[str | Callable[[str], str]]' = None,
-             args: 'tuple[str, ...]' = (), kwargs: 'dict[str, Any]' = {}) -> 'str':
+             args: 'tuple[str, ...]' = (), kwargs: 'dict[str, Any]' = {},
+             pool: 'Iterable[str]' = _TEXT,) -> 'str':  # pylint: disable=dangerous-default-value
     """Return random words.
 
     .. code-block:: python
 
         >>> get_word(count=3)
         'anim voluptate non'
         >>> get_word(count=3, func='capitalize')
         'Non Labore Ut'
         >>> get_word(count=3, func=lambda s: s.upper())
         'NISI TEMPOR CILLUM'
 
     Args:
-        pool: List of words to be used as random word pool.
         count: Number of random words. To generate random number of words, supply a 2-element
             tuple of :obj:`int`, the function will use :func:`random.randint` to choose a
             random integer as the number of random words.
         sep: Seperator between each word.
         func: Filter function. It can be a function name of :obj:`str`, or a customised
             function that takes the original :obj:`str` and returns the modified :obj:`str`.
         args: Additional positional arguments for ``func``.
         kwargs: Additional keyword arguments for ``func``.
+        pool: List of words to be used as random word pool.
 
     Returns:
         Random words.
 
     """
     if isinstance(count, tuple):
         count = random.randint(*count)  # nosec B311
-    return sep.join(itertools.islice(word(pool, count, func, args, kwargs), count))
+    return sep.join(itertools.islice(word(count, func, args, kwargs, pool=pool), count))
 
 
-def get_sentence(pool: 'Iterable[str]' = _TEXT,
-                 count: 'int | tuple[int, int]' = 1,
+def get_sentence(count: 'int | tuple[int, int]' = 1,
                  sep: 'str' = ' ',
                  comma: 'tuple[int, int]' = (0, 2),
-                 word_range: 'tuple[int, int]' = (4, 8)) -> 'str':
+                 word_range: 'tuple[int, int]' = (4, 8), *,
+                 pool: 'Iterable[str]' = _TEXT) -> 'str':
     """Return random sentences.
 
     .. code-block:: python
 
         >>> get_sentence()
         'Nostrud laboris lorem minim sit culpa, aliqua nostrud in amet, sint pariatur eiusmod esse.'
 
     Args:
-        pool: List of words to be used as random word pool.
         count: Number of random sentences. To generate random number of sentences, supply a
             2-element tuple of :obj:`int`, the function will use :func:`random.randint` to
             choose a random integer as the number of random sentences.
         sep: Seperator between each sentence.
         comma: Random range for number of commas. The function will use :func:`random.randint`
             to choose a random integer as the number of commas.
         word_range: Random range for number of words in each sentence. The function will use
             :func:`random.randint` to choose a random integer as the number of words.
+        pool: List of words to be used as random word pool.
 
     Returns:
         Random sentences.
 
     """
     if isinstance(count, tuple):
         count = random.randint(*count)  # nosec B311
-    return sep.join(itertools.islice(sentence(pool, count, comma, word_range), count))
+    return sep.join(itertools.islice(sentence(count, comma, word_range, pool=pool), count))
 
 
-def get_paragraph(pool: 'Iterable[str]' = _TEXT,
-                  count: 'int | tuple[int, int]' = 1,
+def get_paragraph(count: 'int | tuple[int, int]' = 1,
                   sep: 'str' = os.linesep,
                   comma: 'tuple[int, int]' = (0, 2),
                   word_range: 'tuple[int, int]' = (4, 8),
-                  sentence_range: 'tuple[int, int]' = (5, 10)) -> 'str':
+                  sentence_range: 'tuple[int, int]' = (5, 10), *,
+                  pool: 'Iterable[str]' = _TEXT) -> 'str':
     r"""Return random paragraphs.
 
     .. code-block:: python
 
         >>> get_paragraph()
         'Exercitation magna sunt excepteur irure adipiscing commodo duis. Est '
         'ipsum qui deserunt, deserunt nostrud reprehenderit esse. Do velit '
@@ -414,27 +417,27 @@
         'exercitation veniam officia pariatur velit. Deserunt deserunt sed '
         'consequat laborum consequat dolor. Et consectetur irure sint elit tempor,'
         ' est minim nisi eiusmod id excepteur. Minim cillum veniam sed aliquip '
         'anim sit, pariatur nostrud ex cillum laboris laborum. Laborum ullamco '
         'mollit elit. Amet id incididunt ipsum sed.'
 
     Args:
-        pool: List of words to be used as random word pool.
         count: Number of random paragraphs. To generate random number of paragraphs, supply a
             2-element tuple of :obj:`int`, the function will use :func:`random.randint` to choose
             a random integer as the number of random paragraphs.
         sep: Seperator between each paragraph. The default value is OS-dependent as :data:`os.linsep`
             (``\r\n`` on Windows, ``\n`` on POSIX).
         comma: Random range for number of commas. The function will use :func:`random.randint` to choose
             a random integer as the number of commas.
         word_range: Random range for number of words in each sentence. The function will use
             :func:`random.randint` to choose a random integer as the number of words.
         sentence_range: Random range for number of sentences in each paragraph. The function will use
             :func:`random.randint` to choose a random integer as the number of sentences.
+        pool: List of words to be used as random word pool.
 
     Returns:
         Random paragraphs.
 
     """
     if isinstance(count, tuple):
         count = random.randint(*count)  # nosec B311
-    return sep.join(itertools.islice(paragraph(pool, count, comma, word_range, sentence_range), count))
+    return sep.join(itertools.islice(paragraph(count, comma, word_range, sentence_range, pool=pool), count))
```

### Comparing `python-lorem-1.2.0/python_lorem.egg-info/PKG-INFO` & `python-lorem-1.3.0rc1/python_lorem.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 Metadata-Version: 2.1
 Name: python-lorem
-Version: 1.2.0
+Version: 1.3.0rc1
 Summary: Lorem ipsum generator.
-Home-page: https://github.com/JarryShaw/lorem
-Download-URL: https://github.com/JarryShaw/lorem/archive/v1.2.0.tar.gz
-Author: Jarry Shaw
-Author-email: jarryshaw@icloud.com
+Author-email: Jarry Shaw <jarryshaw@icloud.com>
 Maintainer: Jarry Shaw
-Maintainer-email: jarryshaw@icloud.com
-License: BSD License
+License: BSD 3-Clause License
+Project-URL: homepage, https://jarryshaw.github.io/lorem/
+Project-URL: documentation, https://jarryshaw.github.io/lorem/
+Project-URL: repository, https://github.com/JarryShaw/lorem
+Project-URL: changelog, https://github.com/JarryShaw/lorem/releases
 Keywords: lorem,loremipsum
-Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
-Obsoletes: lorem
-Obsoletes: loremipsum
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+Provides-Extra: docs
 License-File: LICENSE
 
 Lorem ipsum generator.
 
 In publishing and graphic design, lorem ipsum is a placeholder text commonly
 used to demonstrate the visual form of a document or a typeface without
 relying on meaningful content.
```

### Comparing `python-lorem-1.2.0/test_lorem.py` & `python-lorem-1.3.0rc1/test_lorem.py`

 * *Files identical despite different names*

