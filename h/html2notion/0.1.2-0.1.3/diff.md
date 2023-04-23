# Comparing `tmp/html2notion-0.1.2.tar.gz` & `tmp/html2notion-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "html2notion-0.1.2.tar", last modified: Sat Apr 22 07:14:39 2023, max compression
+gzip compressed data, was "html2notion-0.1.3.tar", last modified: Sun Apr 23 04:45:05 2023, max compression
```

## Comparing `html2notion-0.1.2.tar` & `html2notion-0.1.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 feizhao    (501) staff       (20)        0 2023-04-22 07:14:39.323777 html2notion-0.1.2/
--rw-r--r--   0 feizhao    (501) staff       (20)     1064 2023-03-22 13:58:21.000000 html2notion-0.1.2/LICENSE
--rw-r--r--   0 feizhao    (501) staff       (20)     4600 2023-04-22 07:14:39.324396 html2notion-0.1.2/PKG-INFO
--rw-r--r--   0 feizhao    (501) staff       (20)     4111 2023-04-22 07:11:47.000000 html2notion-0.1.2/README.md
-drwxr-xr-x   0 feizhao    (501) staff       (20)        0 2023-04-22 07:14:39.291900 html2notion-0.1.2/html2notion/
--rw-r--r--   0 feizhao    (501) staff       (20)        0 2023-03-18 15:41:01.000000 html2notion-0.1.2/html2notion/__init__.py
--rw-r--r--   0 feizhao    (501) staff       (20)     2953 2023-04-20 14:39:58.000000 html2notion-0.1.2/html2notion/main.py
-drwxr-xr-x   0 feizhao    (501) staff       (20)        0 2023-04-22 07:14:39.304222 html2notion-0.1.2/html2notion/translate/
--rw-r--r--   0 feizhao    (501) staff       (20)        0 2023-04-08 10:17:44.000000 html2notion-0.1.2/html2notion/translate/__init__.py
--rw-r--r--   0 feizhao    (501) staff       (20)     3181 2023-04-20 14:39:58.000000 html2notion-0.1.2/html2notion/translate/batch_import.py
--rw-r--r--   0 feizhao    (501) staff       (20)     2724 2023-04-19 14:40:39.000000 html2notion-0.1.2/html2notion/translate/cos_uploader.py
--rw-r--r--   0 feizhao    (501) staff       (20)     2481 2023-04-20 14:39:58.000000 html2notion-0.1.2/html2notion/translate/html2json.py
--rw-r--r--   0 feizhao    (501) staff       (20)     7894 2023-04-21 14:23:32.000000 html2notion-0.1.2/html2notion/translate/html2json_base.py
--rw-r--r--   0 feizhao    (501) staff       (20)      430 2023-04-19 23:45:05.000000 html2notion-0.1.2/html2notion/translate/html2json_default.py
--rw-r--r--   0 feizhao    (501) staff       (20)     8804 2023-04-21 14:23:32.000000 html2notion-0.1.2/html2notion/translate/html2json_yinxiang.py
--rw-r--r--   0 feizhao    (501) staff       (20)     7030 2023-04-19 15:11:43.000000 html2notion-0.1.2/html2notion/translate/notion_export.py
--rw-r--r--   0 feizhao    (501) staff       (20)     2387 2023-04-20 23:03:16.000000 html2notion-0.1.2/html2notion/translate/notion_import.py
-drwxr-xr-x   0 feizhao    (501) staff       (20)        0 2023-04-22 07:14:39.312506 html2notion-0.1.2/html2notion/utils/
--rw-r--r--   0 feizhao    (501) staff       (20)      427 2023-03-25 00:02:40.000000 html2notion-0.1.2/html2notion/utils/__init__.py
--rw-r--r--   0 feizhao    (501) staff       (20)      828 2023-03-22 13:58:21.000000 html2notion-0.1.2/html2notion/utils/load_config.py
--rw-r--r--   0 feizhao    (501) staff       (20)     1579 2023-04-20 14:39:58.000000 html2notion-0.1.2/html2notion/utils/log.py
--rw-r--r--   0 feizhao    (501) staff       (20)      437 2023-04-21 14:23:32.000000 html2notion-0.1.2/html2notion/utils/timeutil.py
-drwxr-xr-x   0 feizhao    (501) staff       (20)        0 2023-04-22 07:14:39.296640 html2notion-0.1.2/html2notion.egg-info/
--rw-r--r--   0 feizhao    (501) staff       (20)     4600 2023-04-22 07:14:39.000000 html2notion-0.1.2/html2notion.egg-info/PKG-INFO
--rw-r--r--   0 feizhao    (501) staff       (20)      875 2023-04-22 07:14:39.000000 html2notion-0.1.2/html2notion.egg-info/SOURCES.txt
--rw-r--r--   0 feizhao    (501) staff       (20)        1 2023-04-22 07:14:39.000000 html2notion-0.1.2/html2notion.egg-info/dependency_links.txt
--rw-r--r--   0 feizhao    (501) staff       (20)       54 2023-04-22 07:14:39.000000 html2notion-0.1.2/html2notion.egg-info/entry_points.txt
--rw-r--r--   0 feizhao    (501) staff       (20)      170 2023-04-22 07:14:39.000000 html2notion-0.1.2/html2notion.egg-info/requires.txt
--rw-r--r--   0 feizhao    (501) staff       (20)       12 2023-04-22 07:14:39.000000 html2notion-0.1.2/html2notion.egg-info/top_level.txt
--rw-r--r--   0 feizhao    (501) staff       (20)      103 2023-03-18 15:06:24.000000 html2notion-0.1.2/pyproject.toml
--rw-r--r--   0 feizhao    (501) staff       (20)      852 2023-04-22 07:14:39.325533 html2notion-0.1.2/setup.cfg
--rw-r--r--   0 feizhao    (501) staff       (20)       38 2023-03-18 07:34:12.000000 html2notion-0.1.2/setup.py
-drwxr-xr-x   0 feizhao    (501) staff       (20)        0 2023-04-22 07:14:39.321890 html2notion-0.1.2/tests/
--rw-r--r--   0 feizhao    (501) staff       (20)     2892 2023-04-20 14:39:58.000000 html2notion-0.1.2/tests/test_batchimport.py
--rw-r--r--   0 feizhao    (501) staff       (20)     3038 2023-04-20 14:39:58.000000 html2notion-0.1.2/tests/test_cosupload.py
--rw-r--r--   0 feizhao    (501) staff       (20)     2698 2023-04-13 14:42:38.000000 html2notion-0.1.2/tests/test_notionexport.py
--rw-r--r--   0 feizhao    (501) staff       (20)    15597 2023-04-20 14:39:58.000000 html2notion-0.1.2/tests/test_yinxiang.py
+drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-04-23 04:45:05.060841 html2notion-0.1.3/
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     1064 2023-03-22 08:52:55.000000 html2notion-0.1.3/LICENSE
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     4600 2023-04-23 04:45:05.061036 html2notion-0.1.3/PKG-INFO
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     4111 2023-04-23 03:24:11.000000 html2notion-0.1.3/README.md
+drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-04-23 04:45:05.040993 html2notion-0.1.3/html2notion/
+-rw-r--r--   0 daemonzhao   (501) staff       (20)        0 2023-03-20 01:38:35.000000 html2notion-0.1.3/html2notion/__init__.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     3955 2023-04-23 03:47:45.000000 html2notion-0.1.3/html2notion/main.py
+drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-04-23 04:45:05.053144 html2notion-0.1.3/html2notion/translate/
+-rw-r--r--   0 daemonzhao   (501) staff       (20)        0 2023-03-20 01:38:35.000000 html2notion-0.1.3/html2notion/translate/__init__.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     4176 2023-04-23 03:24:11.000000 html2notion-0.1.3/html2notion/translate/batch_import.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     2724 2023-04-19 01:44:49.000000 html2notion-0.1.3/html2notion/translate/cos_uploader.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     2481 2023-04-20 11:03:46.000000 html2notion-0.1.3/html2notion/translate/html2json.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     7894 2023-04-21 09:57:38.000000 html2notion-0.1.3/html2notion/translate/html2json_base.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)      430 2023-04-20 02:17:23.000000 html2notion-0.1.3/html2notion/translate/html2json_default.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     8804 2023-04-21 02:35:36.000000 html2notion-0.1.3/html2notion/translate/html2json_yinxiang.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     7030 2023-04-12 04:47:53.000000 html2notion-0.1.3/html2notion/translate/notion_export.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     2387 2023-04-21 02:20:28.000000 html2notion-0.1.3/html2notion/translate/notion_import.py
+drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-04-23 04:45:05.056801 html2notion-0.1.3/html2notion/utils/
+-rw-r--r--   0 daemonzhao   (501) staff       (20)      427 2023-03-24 02:23:25.000000 html2notion-0.1.3/html2notion/utils/__init__.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)      828 2023-03-22 03:05:54.000000 html2notion-0.1.3/html2notion/utils/load_config.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     1579 2023-04-20 06:50:27.000000 html2notion-0.1.3/html2notion/utils/log.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)      437 2023-04-21 02:46:15.000000 html2notion-0.1.3/html2notion/utils/timeutil.py
+drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-04-23 04:45:05.044729 html2notion-0.1.3/html2notion.egg-info/
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     4600 2023-04-23 04:45:04.000000 html2notion-0.1.3/html2notion.egg-info/PKG-INFO
+-rw-r--r--   0 daemonzhao   (501) staff       (20)      875 2023-04-23 04:45:04.000000 html2notion-0.1.3/html2notion.egg-info/SOURCES.txt
+-rw-r--r--   0 daemonzhao   (501) staff       (20)        1 2023-04-23 04:45:04.000000 html2notion-0.1.3/html2notion.egg-info/dependency_links.txt
+-rw-r--r--   0 daemonzhao   (501) staff       (20)       54 2023-04-23 04:45:04.000000 html2notion-0.1.3/html2notion.egg-info/entry_points.txt
+-rw-r--r--   0 daemonzhao   (501) staff       (20)      170 2023-04-23 04:45:04.000000 html2notion-0.1.3/html2notion.egg-info/requires.txt
+-rw-r--r--   0 daemonzhao   (501) staff       (20)       12 2023-04-23 04:45:04.000000 html2notion-0.1.3/html2notion.egg-info/top_level.txt
+-rw-r--r--   0 daemonzhao   (501) staff       (20)      103 2023-03-20 01:38:35.000000 html2notion-0.1.3/pyproject.toml
+-rw-r--r--   0 daemonzhao   (501) staff       (20)      852 2023-04-23 04:45:05.061683 html2notion-0.1.3/setup.cfg
+-rw-r--r--   0 daemonzhao   (501) staff       (20)       38 2023-03-17 05:39:04.000000 html2notion-0.1.3/setup.py
+drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-04-23 04:45:05.059908 html2notion-0.1.3/tests/
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     2892 2023-04-20 03:22:55.000000 html2notion-0.1.3/tests/test_batchimport.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     3038 2023-04-20 03:22:52.000000 html2notion-0.1.3/tests/test_cosupload.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     2698 2023-04-13 05:01:24.000000 html2notion-0.1.3/tests/test_notionexport.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)    15597 2023-04-20 11:59:35.000000 html2notion-0.1.3/tests/test_yinxiang.py
```

### Comparing `html2notion-0.1.2/LICENSE` & `html2notion-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.2/PKG-INFO` & `html2notion-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html2notion
-Version: 0.1.2
+Version: 0.1.3
 Summary: This tool can accurately convert HTML to Notion notes and is also useful for exporting Evernote notes to Notion.
 Home-page: https://github.com/selfboot/html2notion
 Author: selfboot
 Author-email: xuezaigds@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `html2notion-0.1.2/README.md` & `html2notion-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.2/html2notion/main.py` & `html2notion-0.1.3/html2notion/translate/notion_import.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,79 +1,65 @@
-import argparse
-import os
-import sys
-from pathlib import Path
 import asyncio
+import os
 from aiohttp import ClientSession
+from pathlib import Path
 from notion_client import AsyncClient
-from .utils import setup_logger, read_config, logger, config
-from .translate.notion_import import NotionImporter
-from .translate.batch_import import BatchImport
-
-
-def parse_args():
-    parser = argparse.ArgumentParser(
-        description='Html2notion: Save HTML to your Notion notes quickly and easily, while keeping the original format as much as possible')
-    parser.add_argument('--conf', type=str, help='conf file path', required=True)
-    parser.add_argument('--log', type=str, help='log direct path')
-    parser.add_argument('--batch', type=int, default=15, help='batch save concurrent limit')
-
-    group = parser.add_mutually_exclusive_group(required=True)
-    group.add_argument('--file', type=str, help='Save single html file to notion')
-    group.add_argument('--dir', type=str, help='Save all html files in the dir to notion')
-    return parser.parse_args()
-
+from notion_client.errors import RequestTimeoutError
+from tenacity import retry, stop_after_attempt, wait_exponential, retry_if_exception_type
+from ..utils import logger, test_prepare_conf, config
+from ..translate.html2json import html2json_process
+
+
+class NotionImporter:
+    def __init__(self, session: ClientSession, notion_client):
+        self.session = session
+        self.notion_client = notion_client
+
+    async def process_file(self, file_path: Path):
+        if not file_path.is_file():
+            logger.error(f"{file_path} is not a file.")
+            return
+
+        with file_path.open() as f:
+            content = f.read()
+
+        logger.info(f"Process file {file_path}")
+        if content == "main_hold":                  # local debug
+            await asyncio.sleep(1)
+            return "main_hold"
+
+        notion_data, html_type = html2json_process(file_path)
+        logger.info(f"path: {file_path}, html type: {html_type}")
+
+        create_result = await self.create_new_page(notion_data)
+        logger.info(f"Create notion page: {create_result}")
+        return "succ"
+
+    # Doc of create page: https://developers.notion.com/reference/post-page
+    @retry(stop=stop_after_attempt(5),
+           wait=wait_exponential(multiplier=1, min=3, max=30),
+           retry=retry_if_exception_type(RequestTimeoutError))
+    async def create_new_page(self, notion_data):
+        # logger.debug(f'Create new page: {notion_data["parent"]}, {notion_data["properties"]}')
+        created_page = await self.notion_client.pages.create(
+            **notion_data
+        )
+        return created_page
 
-def prepare_env(args: argparse.Namespace):
-    log_path = Path(args.log) if args.log else Path.cwd() / 'logs/'
-    if not log_path.is_dir():
-        log_path.mkdir(parents=True)
 
-    conf_path = Path(args.conf)
-    if not conf_path.is_file():
-        print(f"Read conf file({conf_path}) failed.")
-        logger.fatal(f"Read conf file({conf_path}) failed.")
-        sys.exit(1)
-
-    setup_logger(log_path)
-    read_config(conf_path)
-    logger.info(f"Read log {log_path}, conf {conf_path}")
+async def main(file_path, notion_api_key):
+    async with ClientSession() as session:
+        async with AsyncClient(auth=notion_api_key) as notion_client:
+            importer = NotionImporter(session, notion_client)
+            result = await importer.process_file(file_path)
+            logger.info(f"Import result: {result}")
 
 
-async def import_single_file(file):
+if __name__ == "__main__":
+    test_prepare_conf()
+    file = Path("./demos/TestCaseB.html")
     notion_api_key = ""
     if 'GITHUB_ACTIONS' in os.environ:
         notion_api_key = os.environ['notion_api_key']
     else:
         notion_api_key = config['notion']['api_key']
-    async with ClientSession() as session:
-        async with AsyncClient(auth=notion_api_key) as notion_client:
-            notion_importer = NotionImporter(session, notion_client)
-            result = await notion_importer.process_file(file)
-            return result
-
-
-def main():
-    args = parse_args()
-    prepare_env(args)
-
-    file_path = Path(args.file) if args.file else None
-    dir_path = Path(args.dir) if args.dir else None
-    max_concurrency = args.batch
-    if file_path and file_path.is_file():
-        logger.info(f"Begin save single html file: {file_path}.")
-        result = asyncio.run(import_single_file(file_path))
-        logger.info(f"Finish save single html file: {file_path}.\n{result}")
-        print(f"File {file_path} saved.")
-    elif dir_path and dir_path.is_dir():
-        logger.info(f"Begin save all html files in the dir: {dir_path}.")
-        batch_import = BatchImport(dir_path, max_concurrency)
-        result = asyncio.run(batch_import.process_directory())
-        logger.info(f"Finish save all html files in the dir: {dir_path}.\n{result}")
-        print(f"Directory {dir_path} saved.")
-    else:
-        print("No impossible.")
-    return
-
-
-if __name__ == '__main__':
-    main()
+    asyncio.run(main(file, notion_api_key))
```

### Comparing `html2notion-0.1.2/html2notion/translate/batch_import.py` & `html2notion-0.1.3/html2notion/translate/batch_import.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,69 +1,92 @@
 import asyncio
 import aiohttp
 import os
-import shutil
-import sys
-from tqdm import tqdm
 from pathlib import Path
+from asyncio import Lock
 from notion_client import AsyncClient
+from rich.progress import (
+    BarColumn,
+    MofNCompleteColumn,
+    Progress,
+    TextColumn,
+    TimeRemainingColumn,
+)
 from ..translate.notion_import import NotionImporter
 from ..utils import logger, config
 
 
 class BatchImport:
     def __init__(self, directory: Path, concurrent_limit: int = 10):
         self.directory = directory
         self.concurrent_limit = concurrent_limit
         if 'GITHUB_ACTIONS' in os.environ:
             self.notion_api_key = os.environ['notion_api_key']
         else:
             self.notion_api_key = config['notion']['api_key']
         self.notion_client = AsyncClient(auth=self.notion_api_key)
+        self.all_files = []
+        self.failed_files = []
+        self.success_files = []
+        self.files_lock = Lock()
 
     @staticmethod
-    def print_above(message):
-        term_width, _ = shutil.get_terminal_size()
-        sys.stdout.write('\033[1A')  # Move cursor up one line
-        sys.stdout.write('\r')       # Reset cursor position to the beginning of the line
-        sys.stdout.write(' ' * term_width)  # Fill the entire line with spaces
-        sys.stdout.write('\r')       # Reset cursor position to the beginning of the line again
-        sys.stdout.write(message + '\n')
-
-    @staticmethod
-    async def process_file(session, notion_client, file_path, pbar):
+    async def process_file(session, notion_client, file_path, files_lock, failed_files, success_files):
         logger.info(f"Begin file, file {file_path}")
         notion_import = NotionImporter(session, notion_client)
         if file_path.is_file():
-            response = await notion_import.process_file(file_path)
-            BatchImport.print_above(f"Processed {file_path}")
-            logger.info(f"Finish file {file_path}")
-            pbar.update(1)
-            return response
+            try:
+                response = await notion_import.process_file(file_path)
+                logger.info(f"Finish file {file_path}")
+                async with files_lock:
+                    success_files.append(file_path)
+                return response
+            except Exception as e:
+                logger.error(f"Error processing {file_path}: {str(e)}")
+                async with files_lock:
+                    failed_files.append((file_path, str(e)))
+                return None
+        else:
+            logger.error(f"Error processing {file_path}: File not found")
+            async with files_lock:
+                    failed_files.append((file_path, "File not found"))
+            return None
 
     async def process_directory(self):
         semaphore = asyncio.Semaphore(self.concurrent_limit)
-        html_files = [file_path for file_path in self.directory.glob('*.html') if file_path.name != 'index.html']
-        files_len = len(html_files)
-        pbar = tqdm(total=files_len, bar_format='{l_bar}{bar}|{n_fmt}/{total_fmt}', dynamic_ncols=True)
-        print("")  # Keep a placeholder row
-        BatchImport.print_above("Begin...")
-
-        async def process_file_with_semaphore(session, notion_client, file_path, pbar):
-            async with semaphore:
-                return await self.process_file(session, notion_client, file_path, pbar)
-
-        async with aiohttp.ClientSession() as session:
-            tasks = [
-                process_file_with_semaphore(session, self.notion_client, file_path, pbar)
-                for file_path in html_files
-            ]
-            results = await asyncio.gather(*tasks)
-            await session.close()
-            return results
+        self.all_files = [file_path for file_path in self.directory.glob('*.html') if file_path.name != 'index.html']
+        files_len = len(self.all_files)
+
+        with Progress(
+            TextColumn("[progress.description]{task.description}", justify="right"),
+            BarColumn(),
+            MofNCompleteColumn(),
+            TextColumn(" "),
+            TimeRemainingColumn()
+        ) as progress:
+            # with Progress() as progress:
+            progress.add_task("[cyan]Total", total=files_len,
+                              completed=files_len, update_period=0, style="cyan")
+            success_task_id = progress.add_task(
+                "[green]Success", total=files_len, style="green")
+            failed_task_id = progress.add_task("[red]Failed", total=files_len, style="red")
+            async def process_file_with_semaphore(session, notion_client, file_path):
+                async with semaphore:
+                    result = await self.process_file(session, notion_client, file_path, self.files_lock, self.failed_files, self.success_files)
+                    if result:
+                        progress.update(success_task_id, advance=1)
+                    else:
+                        progress.update(failed_task_id, advance=1)
+                    return result
+
+            async with aiohttp.ClientSession() as session:
+                tasks = [process_file_with_semaphore(session, self.notion_client, file_path) for file_path in self.all_files]
+                results = await asyncio.gather(*tasks)
+                await session.close()
+                return results
 
 
 if __name__ == '__main__':
     from ..utils import test_prepare_conf
     test_prepare_conf()
     from tempfile import TemporaryDirectory
     with TemporaryDirectory() as temp_dir:
```

### Comparing `html2notion-0.1.2/html2notion/translate/cos_uploader.py` & `html2notion-0.1.3/html2notion/translate/cos_uploader.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.2/html2notion/translate/html2json.py` & `html2notion-0.1.3/html2notion/translate/html2json.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.2/html2notion/translate/html2json_base.py` & `html2notion-0.1.3/html2notion/translate/html2json_base.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.2/html2notion/translate/html2json_yinxiang.py` & `html2notion-0.1.3/html2notion/translate/html2json_yinxiang.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.2/html2notion/translate/notion_export.py` & `html2notion-0.1.3/html2notion/translate/notion_export.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.2/html2notion/utils/load_config.py` & `html2notion-0.1.3/html2notion/utils/load_config.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.2/html2notion/utils/log.py` & `html2notion-0.1.3/html2notion/utils/log.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.2/html2notion.egg-info/PKG-INFO` & `html2notion-0.1.3/html2notion.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html2notion
-Version: 0.1.2
+Version: 0.1.3
 Summary: This tool can accurately convert HTML to Notion notes and is also useful for exporting Evernote notes to Notion.
 Home-page: https://github.com/selfboot/html2notion
 Author: selfboot
 Author-email: xuezaigds@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `html2notion-0.1.2/html2notion.egg-info/SOURCES.txt` & `html2notion-0.1.3/html2notion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.2/setup.cfg` & `html2notion-0.1.3/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = html2notion
-version = 0.1.2
+version = 0.1.3
 author = selfboot
 author_email = xuezaigds@gmail.com
 description = This tool can accurately convert HTML to Notion notes and is also useful for exporting Evernote notes to Notion.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/selfboot/html2notion
 license_files = LICENSE
@@ -19,15 +19,15 @@
 	beautifulsoup4>=4.11.2
 	httpcore>=0.16.3
 	httpx>=0.23.3
 	notion-client>=2.0.0
 	PyYAML>=6.0
 	aiohttp>=3.8.4
 	anyio>=3.6.2
-	tqdm>=4.65.0
+	rich>=13.3.4
 	cos-python-sdk-v5>=1.9.23
 	tenacity>=8.2.2
 
 [options.entry_points]
 console_scripts = 
 	html2notion = html2notion.main:main
```

### Comparing `html2notion-0.1.2/tests/test_batchimport.py` & `html2notion-0.1.3/tests/test_batchimport.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.2/tests/test_cosupload.py` & `html2notion-0.1.3/tests/test_cosupload.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.2/tests/test_notionexport.py` & `html2notion-0.1.3/tests/test_notionexport.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.2/tests/test_yinxiang.py` & `html2notion-0.1.3/tests/test_yinxiang.py`

 * *Files identical despite different names*

