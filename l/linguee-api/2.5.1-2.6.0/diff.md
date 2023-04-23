# Comparing `tmp/linguee-api-2.5.1.tar.gz` & `tmp/linguee_api-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linguee-api-2.5.1.tar", max compression
+gzip compressed data, was "linguee_api-2.6.0.tar", max compression
```

## Comparing `linguee-api-2.5.1.tar` & `linguee_api-2.6.0.tar`

### file list

```diff
@@ -1,29 +1,33 @@
--rw-r--r--   0        0        0     1189 2022-11-19 12:39:10.444133 linguee-api-2.5.1/CHANGELOG.md
--rw-r--r--   0        0        0     1082 2022-11-19 10:58:04.345536 linguee-api-2.5.1/LICENSE
--rw-r--r--   0        0        0     8262 2022-11-19 12:31:46.726307 linguee-api-2.5.1/README.md
--rw-r--r--   0        0        0    79885 2022-11-19 10:58:04.346516 linguee-api-2.5.1/docs/linguee-api.png
--rw-r--r--   0        0        0        0 2022-11-19 10:58:04.347006 linguee-api-2.5.1/linguee_api/__init__.py
--rw-r--r--   0        0        0     5099 2022-11-19 10:58:04.347111 linguee-api-2.5.1/linguee_api/api.py
--rw-r--r--   0        0        0      474 2022-11-19 10:58:04.347203 linguee-api-2.5.1/linguee_api/config.py
--rw-r--r--   0        0        0     2202 2022-11-19 10:58:04.347291 linguee-api-2.5.1/linguee_api/const.py
--rw-r--r--   0        0        0        0 2022-11-19 10:58:04.347375 linguee-api-2.5.1/linguee_api/downloaders/__init__.py
--rw-r--r--   0        0        0      424 2022-11-19 10:58:04.347454 linguee-api-2.5.1/linguee_api/downloaders/error_downloader.py
--rw-r--r--   0        0        0      790 2022-11-19 10:58:04.347533 linguee-api-2.5.1/linguee_api/downloaders/file_cache.py
--rw-r--r--   0        0        0     1019 2022-11-19 12:38:09.978546 linguee-api-2.5.1/linguee_api/downloaders/httpx_downloader.py
--rw-r--r--   0        0        0      221 2022-11-19 10:58:04.347693 linguee-api-2.5.1/linguee_api/downloaders/interfaces.py
--rw-r--r--   0        0        0      556 2022-11-19 10:58:04.347767 linguee-api-2.5.1/linguee_api/downloaders/memory_cache.py
--rw-r--r--   0        0        0     4981 2022-11-19 10:58:04.347858 linguee-api-2.5.1/linguee_api/linguee_client.py
--rw-r--r--   0        0        0     5130 2022-11-19 11:45:59.157388 linguee-api-2.5.1/linguee_api/models.py
--rw-r--r--   0        0        0     1494 2022-11-19 11:54:19.223160 linguee-api-2.5.1/linguee_api/parser_utils.py
--rw-r--r--   0        0        0    11248 2022-11-19 11:46:51.856612 linguee-api-2.5.1/linguee_api/parsers.py
--rw-r--r--   0        0        0      592 2022-11-19 10:58:04.348241 linguee-api-2.5.1/linguee_api/utils.py
--rw-r--r--   0        0        0     1397 2022-11-19 12:39:10.443884 linguee-api-2.5.1/pyproject.toml
--rw-r--r--   0        0        0     1269 2022-11-19 10:58:04.349194 linguee-api-2.5.1/tests/conftest.py
--rw-r--r--   0        0        0        0 2022-11-19 10:58:04.349268 linguee-api-2.5.1/tests/parsers/__init__.py
--rw-r--r--   0        0        0      933 2022-11-19 10:58:04.349351 linguee-api-2.5.1/tests/parsers/test_autocompletions.py
--rw-r--r--   0        0        0     6047 2022-11-19 11:53:38.244431 linguee-api-2.5.1/tests/parsers/test_search_result.py
--rw-r--r--   0        0        0      323 2022-11-19 10:58:04.349529 linguee-api-2.5.1/tests/test_api_client.py
--rw-r--r--   0        0        0     1031 2022-11-19 10:58:04.349610 linguee-api-2.5.1/tests/test_downloaders.py
--rw-r--r--   0        0        0     1669 2022-11-19 10:58:04.349694 linguee-api-2.5.1/tests/test_linguee_client.py
--rw-r--r--   0        0        0     9393 2022-11-19 12:39:48.127600 linguee-api-2.5.1/setup.py
--rw-r--r--   0        0        0     9226 2022-11-19 12:39:48.127950 linguee-api-2.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1471 2023-04-23 20:28:03.345255 linguee_api-2.6.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1082 2022-11-19 10:58:04.345536 linguee_api-2.6.0/LICENSE
+-rw-r--r--   0        0        0     8262 2022-11-19 12:31:46.726307 linguee_api-2.6.0/README.md
+-rw-r--r--   0        0        0    79885 2022-11-19 10:58:04.346516 linguee_api-2.6.0/docs/linguee-api.png
+-rw-r--r--   0        0        0        0 2022-11-19 10:58:04.347006 linguee_api-2.6.0/linguee_api/__init__.py
+-rw-r--r--   0        0        0     5112 2022-11-19 14:59:32.903474 linguee_api-2.6.0/linguee_api/api.py
+-rw-r--r--   0        0        0      630 2022-11-19 14:27:50.814467 linguee_api-2.6.0/linguee_api/config.py
+-rw-r--r--   0        0        0     2202 2022-11-19 10:58:04.347291 linguee_api-2.6.0/linguee_api/const.py
+-rw-r--r--   0        0        0        0 2022-11-19 10:58:04.347375 linguee_api-2.6.0/linguee_api/downloaders/__init__.py
+-rw-r--r--   0        0        0      418 2022-11-19 14:30:48.956517 linguee_api-2.6.0/linguee_api/downloaders/error_downloader.py
+-rw-r--r--   0        0        0      911 2022-11-19 14:58:38.549604 linguee_api-2.6.0/linguee_api/downloaders/file_cache.py
+-rw-r--r--   0        0        0     1019 2023-04-22 15:46:33.160338 linguee_api-2.6.0/linguee_api/downloaders/httpx_downloader.py
+-rw-r--r--   0        0        0      836 2022-11-19 14:38:15.268668 linguee_api-2.6.0/linguee_api/downloaders/interfaces.py
+-rw-r--r--   0        0        0      544 2022-11-19 14:59:16.093945 linguee_api-2.6.0/linguee_api/downloaders/memory_cache.py
+-rw-r--r--   0        0        0      384 2022-11-19 14:51:00.329820 linguee_api-2.6.0/linguee_api/downloaders/mock_downloader.py
+-rw-r--r--   0        0        0     1554 2022-11-19 14:58:38.550668 linguee_api-2.6.0/linguee_api/downloaders/sqlite_cache.py
+-rw-r--r--   0        0        0     4981 2022-11-19 10:58:04.347858 linguee_api-2.6.0/linguee_api/linguee_client.py
+-rw-r--r--   0        0        0     5130 2022-11-19 11:45:59.157388 linguee_api-2.6.0/linguee_api/models.py
+-rw-r--r--   0        0        0     1494 2022-11-19 11:54:19.223160 linguee_api-2.6.0/linguee_api/parser_utils.py
+-rw-r--r--   0        0        0    11248 2022-11-19 11:46:51.856612 linguee_api-2.6.0/linguee_api/parsers.py
+-rw-r--r--   0        0        0      592 2022-11-19 10:58:04.348241 linguee_api-2.6.0/linguee_api/utils.py
+-rw-r--r--   0        0        0     1408 2023-04-23 20:28:03.344958 linguee_api-2.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1275 2022-11-19 14:58:38.541829 linguee_api-2.6.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2022-11-19 10:58:04.349268 linguee_api-2.6.0/tests/parsers/__init__.py
+-rw-r--r--   0        0        0      937 2022-11-19 14:30:36.336402 linguee_api-2.6.0/tests/parsers/test_autocompletions.py
+-rw-r--r--   0        0        0     6069 2022-11-19 14:30:23.321620 linguee_api-2.6.0/tests/parsers/test_search_result.py
+-rw-r--r--   0        0        0      323 2022-11-19 10:58:04.349529 linguee_api-2.6.0/tests/test_api_client.py
+-rw-r--r--   0        0        0     1031 2022-11-19 10:58:04.349610 linguee_api-2.6.0/tests/test_downloaders.py
+-rw-r--r--   0        0        0      647 2022-11-19 14:55:08.408860 linguee_api-2.6.0/tests/test_file_cache.py
+-rw-r--r--   0        0        0     1669 2022-11-19 10:58:04.349694 linguee_api-2.6.0/tests/test_linguee_client.py
+-rw-r--r--   0        0        0     1080 2022-11-19 14:58:38.547901 linguee_api-2.6.0/tests/test_memory_cache.py
+-rw-r--r--   0        0        0      703 2022-11-19 14:54:04.114504 linguee_api-2.6.0/tests/test_sqlite_cache.py
+-rw-r--r--   0        0        0     9569 1970-01-01 00:00:00.000000 linguee_api-2.6.0/PKG-INFO
```

### Comparing `linguee-api-2.5.1/CHANGELOG.md` & `linguee_api-2.6.0/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
+## 2.6.0 (2023-04-23)
+
+- Added SQLite cache and made it the default one.
+- Made MemoryCache use LRU.
+- Added tests for all cache classes.
+- Updated Dockerfile to use /cache for file and SQLite caches.
+- Added a sample docker-compose file.
+- Updated FastAPI and httpx dependencies.
+
 ## 2.5.1 (2022-11-19)
 
 - Added FAQ to the README, where provided a clearer explanation of the 503 error.
 
 ## 2.5.0 (2022-11-19)
 
 - Added "follow_corrections" API flag (#23)
```

### Comparing `linguee-api-2.5.1/LICENSE` & `linguee_api-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `linguee-api-2.5.1/README.md` & `linguee_api-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `linguee-api-2.5.1/docs/linguee-api.png` & `linguee_api-2.6.0/docs/linguee-api.png`

 * *Files identical despite different names*

### Comparing `linguee-api-2.5.1/linguee_api/api.py` & `linguee_api-2.6.0/linguee_api/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 
 from linguee_api.config import settings
 from linguee_api.const import (
     FOLLOW_CORRECTIONS_DESCRIPTION,
     LANGUAGE_CODE,
     PROJECT_DESCRIPTION,
 )
-from linguee_api.downloaders.file_cache import FileCache
 from linguee_api.downloaders.httpx_downloader import HTTPXDownloader
 from linguee_api.downloaders.memory_cache import MemoryCache
+from linguee_api.downloaders.sqlite_cache import SQLiteCache
 from linguee_api.linguee_client import LingueeClient
 from linguee_api.models import (
     Autocompletions,
     FollowCorrections,
     ParseError,
     SearchResult,
 )
@@ -26,16 +26,17 @@
     title="Linguee API",
     description=PROJECT_DESCRIPTION,
     version="2.0.0",
 )
 app.add_middleware(SentryAsgiMiddleware)
 
 page_downloader = MemoryCache(
-    upstream=FileCache(
-        cache_directory=settings.cache_directory, upstream=HTTPXDownloader()
+    upstream=SQLiteCache(
+        cache_database=settings.cache_database,
+        upstream=HTTPXDownloader(),
     )
 )
 client = LingueeClient(page_downloader=page_downloader, page_parser=XExtractParser())
 
 
 @app.get("/", include_in_schema=False)
 def index():
```

### Comparing `linguee-api-2.5.1/linguee_api/const.py` & `linguee_api-2.6.0/linguee_api/const.py`

 * *Files identical despite different names*

### Comparing `linguee-api-2.5.1/linguee_api/downloaders/httpx_downloader.py` & `linguee_api-2.6.0/linguee_api/downloaders/httpx_downloader.py`

 * *Files identical despite different names*

### Comparing `linguee-api-2.5.1/linguee_api/downloaders/memory_cache.py` & `linguee_api-2.6.0/linguee_api/downloaders/memory_cache.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,18 @@
-from typing import Dict
+from async_lru import alru_cache
 
 from linguee_api.downloaders.interfaces import IDownloader
 
 
 class MemoryCache(IDownloader):
-    """
-    Memory cache.
+    """Memory cache.
 
     Exposes the downloader interface, but requires the upstream to work and
     keeps records in memory.
     """
 
-    def __init__(self, upstream: IDownloader):
+    def __init__(self, upstream: IDownloader, maxsize: int = 1000):
         self.upstream = upstream
-        self.cache: Dict[str, str] = {}
+        self.download = alru_cache(maxsize=maxsize)(self.download)  # type: ignore
 
     async def download(self, url: str) -> str:
-        if url not in self.cache:
-            self.cache[url] = await self.upstream.download(url)
-        return self.cache[url]
+        return await self.upstream.download(url)
```

### Comparing `linguee-api-2.5.1/linguee_api/linguee_client.py` & `linguee_api-2.6.0/linguee_api/linguee_client.py`

 * *Files identical despite different names*

### Comparing `linguee-api-2.5.1/linguee_api/models.py` & `linguee_api-2.6.0/linguee_api/models.py`

 * *Files identical despite different names*

### Comparing `linguee-api-2.5.1/linguee_api/parser_utils.py` & `linguee_api-2.6.0/linguee_api/parser_utils.py`

 * *Files identical despite different names*

### Comparing `linguee-api-2.5.1/linguee_api/parsers.py` & `linguee_api-2.6.0/linguee_api/parsers.py`

 * *Files identical despite different names*

### Comparing `linguee-api-2.5.1/linguee_api/utils.py` & `linguee_api-2.6.0/linguee_api/utils.py`

 * *Files identical despite different names*

### Comparing `linguee-api-2.5.1/pyproject.toml` & `linguee_api-2.6.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "linguee-api"
-version = "2.5.1"
+version = "2.6.0"
 description = "Linguee API"
 readme = "README.md"
 homepage = "https://github.com/imankulov/linguee-api"
 repository = "https://github.com/imankulov/linguee-api"
 authors = ["Roman Imankulov <roman.imankulov@gmail.com>"]
 license = "MIT"
 classifiers = [
@@ -22,37 +22,38 @@
 packages = [
     { include = "linguee_api" },
     { include = "tests", format = "sdist" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-fastapi = "^0.65.2"
+fastapi = "^0.95.1"
 pydantic = "^1.8.1"
 xextract = "^0.1.8"
-httpx = {version = "1.0.0b0", allow-prereleases = true}
+httpx = "^0.24.0"
 uvicorn = "^0.13.4"
 sentry-sdk = "^1.0.0"
 python-dotenv = "^0.17.0"
 loguru = "^0.5.3"
+aiosqlite = "^0.17.0"
+async-lru = "^1.0.3"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 pytest = "^6.1.2"
 pytest-xdist = "^2.2.1"
 black = "^20.8b1"
 flake8 = "^3.8.4"
 coverage = "^5.4"
 import-linter = "^1.2.1"
 pytest-asyncio = "^0.14.0"
-ipython = "^7.22.0"
+ipython = "^8.10.0"
 click = "^7.1.2"
 asgiref = "^3.3.4"
-tox-poetry-installer = {extras = ["poetry"], version = "^0.8.4"}
+tox-poetry-installer = {extras = ["poetry"], version = "^0.10.2"}
 bump2version = "^1.0.1"
 
 [tool.coverage.run]
 source = ["tests", "linguee_api"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
-
```

### Comparing `linguee-api-2.5.1/tests/conftest.py` & `linguee_api-2.6.0/tests/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import pytest
 from pydantic import BaseSettings, Field
 
 from linguee_api.config import settings
 from linguee_api.const import PROJECT_ROOT
 from linguee_api.downloaders.error_downloader import ErrorDownloader
-from linguee_api.downloaders.file_cache import FileCache
 from linguee_api.downloaders.httpx_downloader import HTTPXDownloader
 from linguee_api.downloaders.interfaces import IDownloader
+from linguee_api.downloaders.sqlite_cache import SQLiteCache
 from linguee_api.linguee_client import LingueeClient
 from linguee_api.parsers import XExtractParser
 
 
 class PytestSettings(BaseSettings):
     """Specific settings for pytest."""
 
@@ -25,17 +25,17 @@
         env_file = (PROJECT_ROOT / ".env").as_posix()
 
 
 pytest_settings = PytestSettings()
 
 
 @pytest.fixture
-def examples_downloader() -> FileCache:
-    return FileCache(
-        cache_directory=settings.cache_directory, upstream=pytest_settings.downloader
+def examples_downloader() -> IDownloader:
+    return SQLiteCache(
+        cache_database=settings.cache_database, upstream=pytest_settings.downloader
     )
 
 
 @pytest.fixture
 def linguee_client(examples_downloader) -> LingueeClient:
     return LingueeClient(
         page_downloader=examples_downloader, page_parser=XExtractParser()
```

### Comparing `linguee-api-2.5.1/tests/parsers/test_autocompletions.py` & `linguee_api-2.6.0/tests/parsers/test_autocompletions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import pytest
 
-from linguee_api.downloaders.file_cache import FileCache
+from linguee_api.downloaders.interfaces import IDownloader
 from linguee_api.linguee_client import get_autocompletions_url
 from linguee_api.models import Autocompletions
 from linguee_api.parsers import XExtractParser
 
 
 @pytest.mark.asyncio
 async def test_parse_autocompletions_should_return_autocompletions(
-    examples_downloader: FileCache,
+    examples_downloader: IDownloader,
 ):
     url = get_autocompletions_url(query="katz", src="de", dst="en")
     page = await examples_downloader.download(url)
     parser = XExtractParser()
     parse_result = parser.parse_autocompletions(page)
 
     a = Autocompletions.AutocompletionItem
```

### Comparing `linguee-api-2.5.1/tests/parsers/test_search_result.py` & `linguee_api-2.6.0/tests/parsers/test_search_result.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Optional
 
 import pytest
 
 from linguee_api.const import LANGUAGE_CODE
-from linguee_api.downloaders.file_cache import FileCache
+from linguee_api.downloaders.interfaces import IDownloader
 from linguee_api.linguee_client import get_search_url
 from linguee_api.models import UsageFrequency
 from linguee_api.parsers import XExtractParser
 
 
 @pytest.mark.parametrize(
     ["query", "src", "dst", "is_not_found"],
@@ -17,28 +17,28 @@
         ("esgotar", "pt", "en", False),
         ("not bad", "en", "pt", False),
         ("xxxxzzzz", "pt", "en", True),
     ],
 )
 @pytest.mark.asyncio
 async def test_parser_should_detect_not_found(
-    examples_downloader: FileCache,
+    examples_downloader: IDownloader,
     query: str,
     src: LANGUAGE_CODE,
     dst: LANGUAGE_CODE,
     is_not_found: bool,
 ):
     url = get_search_url(query=query, src=src, dst=dst, guess_direction=False)
     page = await examples_downloader.download(url)
     assert XExtractParser().is_not_found(page) == is_not_found
 
 
 @pytest.mark.asyncio
 async def test_parser_should_find_translation_examples(
-    examples_downloader: FileCache,
+    examples_downloader: IDownloader,
 ):
     url = get_search_url(query="obrigado", src="pt", dst="en", guess_direction=False)
     page_html = await examples_downloader.download(url)
     page = XExtractParser().parse_search_result_to_page(page_html)
     examples_of_1st_translation = page.lemmas[0].translations[0].examples
     assert examples_of_1st_translation is not None
     assert len(examples_of_1st_translation) == 1
@@ -62,15 +62,15 @@
         ),  # Despite having examples, Linguee provides a correction.
         ("esgotar", "pt", "en", None),
         ("xxxxzzzz", "pt", "en", None),
     ],
 )
 @pytest.mark.asyncio
 async def test_parser_should_find_correction(
-    examples_downloader: FileCache,
+    examples_downloader: IDownloader,
     query: str,
     src: LANGUAGE_CODE,
     dst: LANGUAGE_CODE,
     correction: Optional[str],
 ):
     url = get_search_url(query=query, src=src, dst=dst, guess_direction=False)
     page = await examples_downloader.download(url)
@@ -93,82 +93,82 @@
         ("wünschen", "de", "en"),
         ("envisage", "en", "zh"),
         ("envisage", "en", "sv"),
     ],
 )
 @pytest.mark.asyncio
 async def test_parse_to_dict_should_return_parseable_result(
-    examples_downloader: FileCache,
+    examples_downloader: IDownloader,
     query: str,
     src: LANGUAGE_CODE,
     dst: LANGUAGE_CODE,
 ):
     url = get_search_url(query=query, src=src, dst=dst, guess_direction=False)
     page = await examples_downloader.download(url)
     XExtractParser().parse_search_result_to_page(page)
 
 
 @pytest.mark.asyncio
 async def test_parser_should_find_grammar_info_in_german_verbs(
-    examples_downloader: FileCache,
+    examples_downloader: IDownloader,
 ):
     url = get_search_url(query="bringen", src="de", dst="en", guess_direction=False)
     page_html = await examples_downloader.download(url)
     page = XExtractParser().parse_search_result_to_page(page_html)
     assert page.lemmas[0].grammar_info == "Akk"
 
 
 @pytest.mark.asyncio
 async def test_parser_should_process_examples_without_links(
-    examples_downloader: FileCache,
+    examples_downloader: IDownloader,
 ):
     url = get_search_url(query="einfach", src="de", dst="en", guess_direction=False)
     page_html = await examples_downloader.download(url)
     page = XExtractParser().parse_search_result_to_page(page_html)
     sources = page.external_sources
     assert all([s.src_url.startswith("http") for s in sources])
     assert all([s.dst_url.startswith("http") for s in sources])
 
 
 @pytest.mark.asyncio
 async def test_parser_should_find_almost_always_usage_frequency(
-    examples_downloader: FileCache,
+    examples_downloader: IDownloader,
 ):
     url = get_search_url(query="bacalhau", src="pt", dst="en", guess_direction=False)
     page_html = await examples_downloader.download(url)
     page = XExtractParser().parse_search_result_to_page(page_html)
     assert page.lemmas[0].translations[1].usage_frequency is None
     assert (
         page.lemmas[0].translations[0].usage_frequency == UsageFrequency.ALMOST_ALWAYS
     )
 
 
 @pytest.mark.asyncio
 async def test_parser_should_find_often_usage_frequency(
-    examples_downloader: FileCache,
+    examples_downloader: IDownloader,
 ):
     url = get_search_url(query="placa", src="pt", dst="en", guess_direction=False)
     page_html = await examples_downloader.download(url)
     page = XExtractParser().parse_search_result_to_page(page_html)
     assert page.lemmas[0].translations[1].usage_frequency is None
     assert page.lemmas[0].translations[0].usage_frequency == UsageFrequency.OFTEN
 
 
 @pytest.mark.asyncio
 async def test_parser_should_find_lemma_forms(
-    examples_downloader: FileCache,
+    examples_downloader: IDownloader,
 ):
     url = get_search_url(query="obrigado", src="pt", dst="en", guess_direction=False)
     page_html = await examples_downloader.download(url)
     page = XExtractParser().parse_search_result_to_page(page_html)
     assert page.lemmas[0].forms == []
     assert page.lemmas[1].forms == ["obrigada f sl", "obrigados m pl", "obrigadas f pl"]
 
 
 @pytest.mark.asyncio
 async def test_parser_should_find_lemma_forms_for_verbs(
-    examples_downloader: FileCache,
+    examples_downloader: IDownloader,
 ):
     url = get_search_url(query="shrink", src="en", dst="pt", guess_direction=False)
     page_html = await examples_downloader.download(url)
     page = XExtractParser().parse_search_result_to_page(page_html)
     assert page.lemmas[0].forms == ["shrank or shrunk", "shrunk"]
```

### Comparing `linguee-api-2.5.1/tests/test_downloaders.py` & `linguee_api-2.6.0/tests/test_downloaders.py`

 * *Files identical despite different names*

### Comparing `linguee-api-2.5.1/tests/test_linguee_client.py` & `linguee_api-2.6.0/tests/test_linguee_client.py`

 * *Files identical despite different names*

### Comparing `linguee-api-2.5.1/setup.py` & `linguee_api-2.6.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,246 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: linguee-api
+Version: 2.6.0
+Summary: Linguee API
+Home-page: https://github.com/imankulov/linguee-api
+License: MIT
+Author: Roman Imankulov
+Author-email: roman.imankulov@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: aiosqlite (>=0.17.0,<0.18.0)
+Requires-Dist: async-lru (>=1.0.3,<2.0.0)
+Requires-Dist: fastapi (>=0.95.1,<0.96.0)
+Requires-Dist: httpx (>=0.24.0,<0.25.0)
+Requires-Dist: loguru (>=0.5.3,<0.6.0)
+Requires-Dist: pydantic (>=1.8.1,<2.0.0)
+Requires-Dist: python-dotenv (>=0.17.0,<0.18.0)
+Requires-Dist: sentry-sdk (>=1.0.0,<2.0.0)
+Requires-Dist: uvicorn (>=0.13.4,<0.14.0)
+Requires-Dist: xextract (>=0.1.8,<0.2.0)
+Project-URL: Repository, https://github.com/imankulov/linguee-api
+Description-Content-Type: text/markdown
 
-packages = \
-['linguee_api', 'linguee_api.downloaders', 'tests', 'tests.parsers']
+# Linguee API
 
-package_data = \
-{'': ['*']}
+[Linguee](https://linguee.com) provides excellent dictionary and translation memory service. Unfortunately, there is no way you can get automated access to it. Linguee API fixes the problem. It acts as a proxy and converts their HTML responses to easy-to-use JSON API.
 
-install_requires = \
-['fastapi>=0.65.2,<0.66.0',
- 'httpx==1.0.0b0',
- 'loguru>=0.5.3,<0.6.0',
- 'pydantic>=1.8.1,<2.0.0',
- 'python-dotenv>=0.17.0,<0.18.0',
- 'sentry-sdk>=1.0.0,<2.0.0',
- 'uvicorn>=0.13.4,<0.14.0',
- 'xextract>=0.1.8,<0.2.0']
-
-setup_kwargs = {
-    'name': 'linguee-api',
-    'version': '2.5.1',
-    'description': 'Linguee API',
-    'long_description': '# Linguee API\n\n[Linguee](https://linguee.com) provides excellent dictionary and translation memory service. Unfortunately, there is no way you can get automated access to it. Linguee API fixes the problem. It acts as a proxy and converts their HTML responses to easy-to-use JSON API.\n\n## API endpoints\n\nThe proxy provides three API endpoints: for translations, for examples, and external sources.\n\n![Linguee API](./docs/linguee-api.png)\n\nThe API documentation and the playground is available for the sample installation:\n\n- [Documentation and API playground](https://linguee-api.fly.dev/docs)\n- [The same documentation, but formatted with ReDoc](https://linguee-api.fly.dev/redoc)\n\n## Sample installation\n\nSample installation is available at https://linguee-api.fly.dev.\n\n- Get translations of the word "bacalhau" from Portuguese to English: [https://linguee-api.fly.dev/api/v2/translations?query=bacalhau&src=pt&dst=en](https://linguee-api.fly.dev/api/v2/translations?query=bacalhau&src=pt&dst=en).\n- Get a list of curated examples: [https://linguee-api.fly.dev/api/v2/examples?query=bacalhau&src=pt&dst=en](https://linguee-api.fly.dev/api/v2/examples?query=bacalhau&src=pt&dst=en).\n- Get examples from external sources: [https://linguee-api.fly.dev/api/v2/external_sources?query=bacalhau&src=pt&dst=en](https://linguee-api.fly.dev/api/v2/examples?query=bacalhau&src=pt&dst=en).\n\n## Local installation\n\nInstall the Linguee API.\n\n```shell\n$ pip install linguee-api\n```\n\nRun the API server with `uvicorn` (installed as a dependency.)\n\n```shell\n$ uvicorn linguee_api.api:app\n...\nINFO:     Uvicorn running on http://127.0.0.1:8000 (Press CTRL+C to quit)\n...\n```\n\nOpen http://127.0.0.1:8000. You will be redirected to the API documentation page, where you can test the API.\n\n## Supported languages\n\nAPI supports all the languages, supported by Linguee. As in Linguee, not all language pairs are valid though. Supported languages:\n`bg` (Bulgarian), `cs` (Czech), `da` (Danish), `de` (German), `el` (Greek), `en` (English), `es` (Spanish), `et` (Estonian), `fi` (Finnish), `fr` (French), `hu` (Hungarian), `it` (Italian), `ja` (Japan),`lt` (Lithuanian), `lv` (Latvian), `mt` (Maltese), `nl` (Dutch), `pl` (Polish), `pt` (Portuguese), `ro` (Romanian), `ru` (Russian), `sk` (Slovak), `sl` (Solvene), `sv` (Swedish), `zh` (Chinese).\n\n## Response structure\n\n**Lemmas**\n\nEvery query (a random string) can match several so-called lemma objects.\n\nAccording to Wikipedia, [lemma](https://en.wikipedia.org/wiki/Lemma_(morphology)) is the canonical form, dictionary form, or citation form of a set of words.\n\nIn English, for example, break, breaks, broke, broken, and breaking are forms of the same lexeme, with "break" as the lemma by which they are indexed.\n\nIn the API, lemmas have the only required attribute, "text," but may have optional elements, such as part of speech ("pos") and audio links with pronunciations.\n\n\n**Translations**\n\nEvery lemma has one or more translations. The translation is a lemma in a different language and has a similar structure with the necessary text field and optional part of speech and audio links.\n\n\n**Examples**\n\nIn addition to lemmas, the API returns several usage examples curated by dictionary authors. Examples are the short phrases, annotated with one or more equivalents in different languages. When appropriate, examples may contain the part-of-speech form and audio links.\n\n**External Sources**\n\nOn top of curated examples, Linguee provides links to external sources. The API returns objects containing the phrase snipped in the original language and an equivalent snippet in the translation.\n\n## Usage examples with Python and requests\n\nOnce installed on Heroku, Linguee API can be used as any other API service. I recommend using the [requests](https://docs.python-requests.org/) library.\n\n### Translate a word or a phrase from one language to another with Python\n\nA request to the sample API installation to translate the word "bacalhau" from Portuguese to English.\n\n```python\nimport requests\n\napi_root = "https://linguee-api.fly.dev/api/v2"\nresp = requests.get(f"{api_root}/translations", params={"query": "bacalhau", "src": "pt", "dst": "en"})\nfor lemma in resp.json():\n    for translation in lemma[\'translations\']:\n        print(f"{lemma[\'text\']} -> {translation[\'text\']}")\n```\n\nThis will print:\n\n```\nbacalhau -> cod\nbacalhau -> codfish\n```\n\n### Provide translation examples with Python\n\nA request to the sample API installation to get all usage examples of "bacalhau" along with their translations.\n\n```python\nimport requests\n\napi_root = "https://linguee-api.fly.dev/api/v2"\n\nresp = requests.get(f"{api_root}/examples", params={"query": "bacalhau", "src": "pt", "dst": "en"})\n\nfor example in resp.json():\n    for translation in example["translations"]:\n        print(f"{example[\'text\']} -> {translation[\'text\']}")\n```\n\nThis will print:\n\n```\nbacalhau desfiado -> shredded cod\nlombo de bacalhau -> codfish fillet\n...\nbacalhau do Atlântico -> Atlantic cod\n```\n\n### Get access to real world usage examples with Python\n\nA request to the sample API installation to get all real-world usage examples of "bacalhau" along with their translations.\n\n```python\nimport requests\n\napi_root = "https://linguee-api.fly.dev/api/v2"\n\nresp = requests.get(f"{api_root}/external_sources", params={"query": "bacalhau", "src": "pt", "dst": "en"})\nfor source in resp.json():\n    print(f"{source[\'src\']} -> {source[\'dst\']}")\n```\n\nThis will print a long list of real-world examples like this:\n\n```\nÉ calculado o esforço de [...] pesca de todos os navios que capturam bacalhau. -> The fishing effort of all [...] the vessels catching cod will be calculated.\n```\n\n\n## Bash, curl and jq usage example\n\nOnce installed on Heroku, Linguee API can be used as any other API service.\n\nFor Bash scripts you can use curl and [jq](https://stedolan.github.io/jq/), a command-line JSON parser.\n\n### Translate a word or a phrase from one language to another with Bash\n\nA request to the sample API installation to get all usage examples of "bacalhau" along with their translations.\n\n```bash\ncurl -s \'https://linguee-api.fly.dev/api/v2/translations?query=bacalhau&src=pt&dst=en\' | jq -c \'{text: .[].text, translation: .[].translations[].text}\'\n```\n\nThis will print\n\n```json lines\n{"text":"bacalhau","translation":"cod"}\n{"text":"bacalhau","translation":"codfish"}\n```\n\n### Provide translation examples with Bash\n\nA request to the sample API installation to get all usage examples of "bacalhau" along with their translations.\n\n```shell\ncurl -s \'https://linguee-api.fly.dev/api/v2/examples?query=bacalhau&src=pt&dst=en\' | jq -c \'{text: .[].text, translation: .[].translations[].text}\'\n```\n\nThis will print something like this:\n\n```json lines\n{"text":"bacalhau desfiado","translation":"shredded cod"}\n{"text":"bacalhau desfiado","translation":"codfish fillet"}\n...\n{"text":"bacalhau do Atlântico","translation":"Atlantic cod"}\n```\n\n### Get access to real world usage examples with Bash\n\nA request to the sample API installation to get all real-world usage examples of "bacalhau" along with their translations.\n\n```shell\ncurl -s \'https://linguee-api.fly.dev/api/v2/external_sources?query=bacalhau&src=pt&dst=en\' | jq -c \'{src: .[].src, dst: .[].dst}\'\n```\n\nThis will print a long list of real-world examples like this:\n\n```json lines\n{"src":"É calculado o esforço de [...] pesca de todos os navios que capturam bacalhau.","dst":"The fishing effort of all [...] the vessels catching cod will be calculated."}\n...\n```\n\n## FAQ\n\n### The API server returns "The Linguee server returned 503"\n\nThis error means that the Linguee website temporarily blocks the API client for sending too many requests. If you use the sample API server on https://linguee-api.fly.dev, you can try to send the request later or consider installing your API server, where you won\'t share the same IP address with other users.\n\n## Terms and Conditions\n\nIf you use the API, make sure you comply with\n[Linguee Terms and Conditions](http://www.linguee.com/page/termsAndConditions.php),\nand in particular with that clause:\n\n> Both private and business usage of linguee.com services is free of charge.\n> It is however strictly prohibited to forward on our services to third\n> parties against payment\n',
-    'author': 'Roman Imankulov',
-    'author_email': 'roman.imankulov@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/imankulov/linguee-api',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
+## API endpoints
 
+The proxy provides three API endpoints: for translations, for examples, and external sources.
+
+![Linguee API](./docs/linguee-api.png)
+
+The API documentation and the playground is available for the sample installation:
+
+- [Documentation and API playground](https://linguee-api.fly.dev/docs)
+- [The same documentation, but formatted with ReDoc](https://linguee-api.fly.dev/redoc)
+
+## Sample installation
+
+Sample installation is available at https://linguee-api.fly.dev.
+
+- Get translations of the word "bacalhau" from Portuguese to English: [https://linguee-api.fly.dev/api/v2/translations?query=bacalhau&src=pt&dst=en](https://linguee-api.fly.dev/api/v2/translations?query=bacalhau&src=pt&dst=en).
+- Get a list of curated examples: [https://linguee-api.fly.dev/api/v2/examples?query=bacalhau&src=pt&dst=en](https://linguee-api.fly.dev/api/v2/examples?query=bacalhau&src=pt&dst=en).
+- Get examples from external sources: [https://linguee-api.fly.dev/api/v2/external_sources?query=bacalhau&src=pt&dst=en](https://linguee-api.fly.dev/api/v2/examples?query=bacalhau&src=pt&dst=en).
+
+## Local installation
+
+Install the Linguee API.
+
+```shell
+$ pip install linguee-api
+```
+
+Run the API server with `uvicorn` (installed as a dependency.)
+
+```shell
+$ uvicorn linguee_api.api:app
+...
+INFO:     Uvicorn running on http://127.0.0.1:8000 (Press CTRL+C to quit)
+...
+```
+
+Open http://127.0.0.1:8000. You will be redirected to the API documentation page, where you can test the API.
+
+## Supported languages
+
+API supports all the languages, supported by Linguee. As in Linguee, not all language pairs are valid though. Supported languages:
+`bg` (Bulgarian), `cs` (Czech), `da` (Danish), `de` (German), `el` (Greek), `en` (English), `es` (Spanish), `et` (Estonian), `fi` (Finnish), `fr` (French), `hu` (Hungarian), `it` (Italian), `ja` (Japan),`lt` (Lithuanian), `lv` (Latvian), `mt` (Maltese), `nl` (Dutch), `pl` (Polish), `pt` (Portuguese), `ro` (Romanian), `ru` (Russian), `sk` (Slovak), `sl` (Solvene), `sv` (Swedish), `zh` (Chinese).
+
+## Response structure
+
+**Lemmas**
+
+Every query (a random string) can match several so-called lemma objects.
+
+According to Wikipedia, [lemma](https://en.wikipedia.org/wiki/Lemma_(morphology)) is the canonical form, dictionary form, or citation form of a set of words.
+
+In English, for example, break, breaks, broke, broken, and breaking are forms of the same lexeme, with "break" as the lemma by which they are indexed.
+
+In the API, lemmas have the only required attribute, "text," but may have optional elements, such as part of speech ("pos") and audio links with pronunciations.
+
+
+**Translations**
+
+Every lemma has one or more translations. The translation is a lemma in a different language and has a similar structure with the necessary text field and optional part of speech and audio links.
+
+
+**Examples**
+
+In addition to lemmas, the API returns several usage examples curated by dictionary authors. Examples are the short phrases, annotated with one or more equivalents in different languages. When appropriate, examples may contain the part-of-speech form and audio links.
+
+**External Sources**
+
+On top of curated examples, Linguee provides links to external sources. The API returns objects containing the phrase snipped in the original language and an equivalent snippet in the translation.
+
+## Usage examples with Python and requests
+
+Once installed on Heroku, Linguee API can be used as any other API service. I recommend using the [requests](https://docs.python-requests.org/) library.
+
+### Translate a word or a phrase from one language to another with Python
+
+A request to the sample API installation to translate the word "bacalhau" from Portuguese to English.
+
+```python
+import requests
+
+api_root = "https://linguee-api.fly.dev/api/v2"
+resp = requests.get(f"{api_root}/translations", params={"query": "bacalhau", "src": "pt", "dst": "en"})
+for lemma in resp.json():
+    for translation in lemma['translations']:
+        print(f"{lemma['text']} -> {translation['text']}")
+```
+
+This will print:
+
+```
+bacalhau -> cod
+bacalhau -> codfish
+```
+
+### Provide translation examples with Python
+
+A request to the sample API installation to get all usage examples of "bacalhau" along with their translations.
+
+```python
+import requests
+
+api_root = "https://linguee-api.fly.dev/api/v2"
+
+resp = requests.get(f"{api_root}/examples", params={"query": "bacalhau", "src": "pt", "dst": "en"})
+
+for example in resp.json():
+    for translation in example["translations"]:
+        print(f"{example['text']} -> {translation['text']}")
+```
+
+This will print:
+
+```
+bacalhau desfiado -> shredded cod
+lombo de bacalhau -> codfish fillet
+...
+bacalhau do Atlântico -> Atlantic cod
+```
+
+### Get access to real world usage examples with Python
+
+A request to the sample API installation to get all real-world usage examples of "bacalhau" along with their translations.
+
+```python
+import requests
+
+api_root = "https://linguee-api.fly.dev/api/v2"
+
+resp = requests.get(f"{api_root}/external_sources", params={"query": "bacalhau", "src": "pt", "dst": "en"})
+for source in resp.json():
+    print(f"{source['src']} -> {source['dst']}")
+```
+
+This will print a long list of real-world examples like this:
+
+```
+É calculado o esforço de [...] pesca de todos os navios que capturam bacalhau. -> The fishing effort of all [...] the vessels catching cod will be calculated.
+```
+
+
+## Bash, curl and jq usage example
+
+Once installed on Heroku, Linguee API can be used as any other API service.
+
+For Bash scripts you can use curl and [jq](https://stedolan.github.io/jq/), a command-line JSON parser.
+
+### Translate a word or a phrase from one language to another with Bash
+
+A request to the sample API installation to get all usage examples of "bacalhau" along with their translations.
+
+```bash
+curl -s 'https://linguee-api.fly.dev/api/v2/translations?query=bacalhau&src=pt&dst=en' | jq -c '{text: .[].text, translation: .[].translations[].text}'
+```
+
+This will print
+
+```json lines
+{"text":"bacalhau","translation":"cod"}
+{"text":"bacalhau","translation":"codfish"}
+```
+
+### Provide translation examples with Bash
+
+A request to the sample API installation to get all usage examples of "bacalhau" along with their translations.
+
+```shell
+curl -s 'https://linguee-api.fly.dev/api/v2/examples?query=bacalhau&src=pt&dst=en' | jq -c '{text: .[].text, translation: .[].translations[].text}'
+```
+
+This will print something like this:
+
+```json lines
+{"text":"bacalhau desfiado","translation":"shredded cod"}
+{"text":"bacalhau desfiado","translation":"codfish fillet"}
+...
+{"text":"bacalhau do Atlântico","translation":"Atlantic cod"}
+```
+
+### Get access to real world usage examples with Bash
+
+A request to the sample API installation to get all real-world usage examples of "bacalhau" along with their translations.
+
+```shell
+curl -s 'https://linguee-api.fly.dev/api/v2/external_sources?query=bacalhau&src=pt&dst=en' | jq -c '{src: .[].src, dst: .[].dst}'
+```
+
+This will print a long list of real-world examples like this:
+
+```json lines
+{"src":"É calculado o esforço de [...] pesca de todos os navios que capturam bacalhau.","dst":"The fishing effort of all [...] the vessels catching cod will be calculated."}
+...
+```
+
+## FAQ
+
+### The API server returns "The Linguee server returned 503"
+
+This error means that the Linguee website temporarily blocks the API client for sending too many requests. If you use the sample API server on https://linguee-api.fly.dev, you can try to send the request later or consider installing your API server, where you won't share the same IP address with other users.
+
+## Terms and Conditions
+
+If you use the API, make sure you comply with
+[Linguee Terms and Conditions](http://www.linguee.com/page/termsAndConditions.php),
+and in particular with that clause:
+
+> Both private and business usage of linguee.com services is free of charge.
+> It is however strictly prohibited to forward on our services to third
+> parties against payment
 
-setup(**setup_kwargs)
```

