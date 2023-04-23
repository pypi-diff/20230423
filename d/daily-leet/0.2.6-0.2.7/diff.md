# Comparing `tmp/daily_leet-0.2.6.tar.gz` & `tmp/daily_leet-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daily_leet-0.2.6.tar", max compression
+gzip compressed data, was "daily_leet-0.2.7.tar", max compression
```

## Comparing `daily_leet-0.2.6.tar` & `daily_leet-0.2.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1619 2023-02-17 12:27:54.420158 daily_leet-0.2.6/README.md
--rw-r--r--   0        0        0        0 2023-02-13 11:38:36.804389 daily_leet-0.2.6/daily_leet/__init__.py
--rw-r--r--   0        0        0       29 2023-02-13 19:03:37.532315 daily_leet-0.2.6/daily_leet/__main__.py
--rw-r--r--   0        0        0       38 2023-02-13 14:04:22.244935 daily_leet-0.2.6/daily_leet/constants.py
--rw-r--r--   0        0        0     3679 2023-02-15 19:21:27.258695 daily_leet-0.2.6/daily_leet/fetch_data.py
--rw-r--r--   0        0        0      641 2023-02-15 19:20:11.894502 daily_leet-0.2.6/daily_leet/language_support/__init__.py
--rw-r--r--   0        0        0     1255 2023-04-09 07:20:12.220504 daily_leet-0.2.6/daily_leet/language_support/cpp.py
--rw-r--r--   0        0        0     5798 2023-02-17 12:01:58.880128 daily_leet-0.2.6/daily_leet/language_support/golang.py
--rw-r--r--   0        0        0      751 2023-02-16 09:35:12.727637 daily_leet-0.2.6/daily_leet/language_support/python3.py
--rw-r--r--   0        0        0     3283 2023-02-17 12:02:08.241591 daily_leet-0.2.6/daily_leet/language_support/rust.py
--rw-r--r--   0        0        0     1111 2023-02-17 12:00:25.080482 daily_leet-0.2.6/daily_leet/language_support/types.py
--rw-r--r--   0        0        0      787 2023-02-15 19:21:39.494048 daily_leet-0.2.6/daily_leet/language_support/utils.py
--rw-r--r--   0        0        0     4410 2023-02-17 12:27:43.663270 daily_leet-0.2.6/daily_leet/main.py
--rw-r--r--   0        0        0      603 2023-02-16 09:35:40.928766 daily_leet-0.2.6/daily_leet/utils.py
--rw-r--r--   0        0        0      569 2023-04-09 07:20:26.435833 daily_leet-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     2461 1970-01-01 00:00:00.000000 daily_leet-0.2.6/setup.py
--rw-r--r--   0        0        0     2116 1970-01-01 00:00:00.000000 daily_leet-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1619 2023-02-17 12:27:54.420158 daily_leet-0.2.7/README.md
+-rw-r--r--   0        0        0        0 2023-02-13 11:38:36.804389 daily_leet-0.2.7/daily_leet/__init__.py
+-rw-r--r--   0        0        0       29 2023-02-13 19:03:37.532315 daily_leet-0.2.7/daily_leet/__main__.py
+-rw-r--r--   0        0        0       38 2023-02-13 14:04:22.244935 daily_leet-0.2.7/daily_leet/constants.py
+-rw-r--r--   0        0        0     3679 2023-02-15 19:21:27.258695 daily_leet-0.2.7/daily_leet/fetch_data.py
+-rw-r--r--   0        0        0      641 2023-02-15 19:20:11.894502 daily_leet-0.2.7/daily_leet/language_support/__init__.py
+-rw-r--r--   0        0        0     1255 2023-04-09 07:20:12.220504 daily_leet-0.2.7/daily_leet/language_support/cpp.py
+-rw-r--r--   0        0        0     5798 2023-02-17 12:01:58.880128 daily_leet-0.2.7/daily_leet/language_support/golang.py
+-rw-r--r--   0        0        0      751 2023-02-16 09:35:12.727637 daily_leet-0.2.7/daily_leet/language_support/python3.py
+-rw-r--r--   0        0        0     3283 2023-02-17 12:02:08.241591 daily_leet-0.2.7/daily_leet/language_support/rust.py
+-rw-r--r--   0        0        0     1111 2023-02-17 12:00:25.080482 daily_leet-0.2.7/daily_leet/language_support/types.py
+-rw-r--r--   0        0        0      787 2023-02-15 19:21:39.494048 daily_leet-0.2.7/daily_leet/language_support/utils.py
+-rw-r--r--   0        0        0     4642 2023-04-23 11:23:14.715427 daily_leet-0.2.7/daily_leet/main.py
+-rw-r--r--   0        0        0      603 2023-02-16 09:35:40.928766 daily_leet-0.2.7/daily_leet/utils.py
+-rw-r--r--   0        0        0      569 2023-04-23 11:23:37.477647 daily_leet-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     2461 1970-01-01 00:00:00.000000 daily_leet-0.2.7/setup.py
+-rw-r--r--   0        0        0     2116 1970-01-01 00:00:00.000000 daily_leet-0.2.7/PKG-INFO
```

### Comparing `daily_leet-0.2.6/README.md` & `daily_leet-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `daily_leet-0.2.6/daily_leet/fetch_data.py` & `daily_leet-0.2.7/daily_leet/fetch_data.py`

 * *Files identical despite different names*

### Comparing `daily_leet-0.2.6/daily_leet/language_support/__init__.py` & `daily_leet-0.2.7/daily_leet/language_support/__init__.py`

 * *Files identical despite different names*

### Comparing `daily_leet-0.2.6/daily_leet/language_support/cpp.py` & `daily_leet-0.2.7/daily_leet/language_support/cpp.py`

 * *Files identical despite different names*

### Comparing `daily_leet-0.2.6/daily_leet/language_support/golang.py` & `daily_leet-0.2.7/daily_leet/language_support/golang.py`

 * *Files identical despite different names*

### Comparing `daily_leet-0.2.6/daily_leet/language_support/python3.py` & `daily_leet-0.2.7/daily_leet/language_support/python3.py`

 * *Files identical despite different names*

### Comparing `daily_leet-0.2.6/daily_leet/language_support/rust.py` & `daily_leet-0.2.7/daily_leet/language_support/rust.py`

 * *Files identical despite different names*

### Comparing `daily_leet-0.2.6/daily_leet/language_support/types.py` & `daily_leet-0.2.7/daily_leet/language_support/types.py`

 * *Files identical despite different names*

### Comparing `daily_leet-0.2.6/daily_leet/language_support/utils.py` & `daily_leet-0.2.7/daily_leet/language_support/utils.py`

 * *Files identical despite different names*

### Comparing `daily_leet-0.2.6/daily_leet/main.py` & `daily_leet-0.2.7/daily_leet/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,25 +25,29 @@
 ) -> Path:
     try:
         set_cookie(session)
     except Exception as e:
         raise typer.BadParameter(f"Failed to get cookie from {LEETCODE_HOST}, {e}")
 
     with BasicSpinner() as progress:
+        start_time = progress.get_time()
         progress.add_task(description="fetching code snippet...", total=None)
         code_snippet = get_code_snippet(session, title_slug, lang_slug)
-        time = progress.get_time()
-        progress.print(f"[bold green]fetched code snippet in {time:.2f}s[/bold green]")
+        elapsed_time = progress.get_time() - start_time
+        progress.print(
+            f"[bold green]fetched code snippet in {elapsed_time:.2f}s[/bold green]"
+        )
 
     with BasicSpinner() as progress:
+        start_time = progress.get_time()
         progress.add_task(description="fetching example test cases...", total=None)
         example_test_cases = get_example_test_cases(session, title_slug)
-        time = progress.get_time()
+        elapsed_time = progress.get_time() - start_time
         progress.print(
-            f"[bold green]fetched example test cases in {time:.2f}s[/bold green]"
+            f"[bold green]fetched example test cases in {elapsed_time:.2f}s[/bold green]"
         )
 
     typer.echo(f"Creating files for {title_slug} in {lang_slug.value}...")
     main_file_path = create_files(
         lang_slug, title_slug, code_snippet, example_test_cases
     )
 
@@ -62,19 +66,20 @@
 
     try:
         set_cookie(session)
     except Exception as e:
         raise typer.BadParameter(f"Failed to get cookie from {LEETCODE_HOST}, {e}")
 
     with BasicSpinner() as progress:
+        start_time = progress.get_time()
         progress.add_task(description="fetching daily challenge...", total=None)
         title_slug = get_daily_challenge_title_slug(session)
-        time = progress.get_time()
+        elapsed_time = progress.get_time() - start_time
         progress.print(
-            f"[bold green]fetched daily challenge in {time:.2f}s[/bold green]"
+            f"[bold green]fetched daily challenge in {elapsed_time:.2f}s[/bold green]"
         )
 
     typer.echo(f"Today's problem is: {title_slug}")
 
     lang_slug = to_lang_slug(language)
     main_file_path = fetch_data_and_create_files(session, lang_slug, title_slug)
```

### Comparing `daily_leet-0.2.6/daily_leet/utils.py` & `daily_leet-0.2.7/daily_leet/utils.py`

 * *Files identical despite different names*

### Comparing `daily_leet-0.2.6/pyproject.toml` & `daily_leet-0.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "daily-leet"
-version = "0.2.6"
+version = "0.2.7"
 description = ""
 authors = ["madmaxieee <76544194+madmaxieee@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{ include = "daily_leet" }]
 
 [tool.poetry.scripts]
 leetcode = "daily_leet.main:app"
```

### Comparing `daily_leet-0.2.6/setup.py` & `daily_leet-0.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['requests>=2.28.2,<3.0.0', 'typer[all]>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['leetcode = daily_leet.main:app']}
 
 setup_kwargs = {
     'name': 'daily-leet',
-    'version': '0.2.6',
+    'version': '0.2.7',
     'description': '',
     'long_description': "# `daily-leet`\n\n**Usage**:\n\n```console\n$ daily-leet [OPTIONS] COMMAND [ARGS]...\n```\n\n**Options**:\n\n* `--install-completion`: Install completion for the current shell.\n* `--show-completion`: Show completion for the current shell, to copy it or customize the installation.\n* `--help`: Show this message and exit.\n\n**Commands**:\n\n* `daily`: Fetch today's daily challenge and create...\n* `new`: Fetch data from a problem's description...\n\n## `daily-leet daily`\n\nFetch today's daily challenge and create files for it, then open the problem page in browser and open the main file in editor\n\n**Usage**:\n\n```console\n$ daily-leet daily [OPTIONS] LANGUAGE:{python|python3|py|cpp|c++|go|golang|rust}\n```\n\n**Arguments**:\n\n* `LANGUAGE:{python|python3|py|cpp|c++|go|golang|rust}`: The language you want to use  [required]\n\n**Options**:\n\n* `--help`: Show this message and exit.\n\n## `daily-leet new`\n\nFetch data from a problem's description page and create files for it, then open the problem page in browser and open the main file in editor\n\n**Usage**:\n\n```console\n$ daily-leet new [OPTIONS] LANGUAGE:{python|python3|py|cpp|c++|go|golang|rust}\n```\n\n**Arguments**:\n\n* `LANGUAGE:{python|python3|py|cpp|c++|go|golang|rust}`: The language you want to use  [required]\n\n**Options**:\n\n* `-u, --url TEXT`: The url to fetch data from, usually a problem's description page. e.g. https://leetcode.com/problems/two-sum/. You need to provide either url or problem title.\n* `-t, --title TEXT`: The title of the problem, separated by '-' or ' '. e.g. two-sum. You need to provide either url or problem title.\n* `--help`: Show this message and exit.\n",
     'author': 'madmaxieee',
     'author_email': '76544194+madmaxieee@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `daily_leet-0.2.6/PKG-INFO` & `daily_leet-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daily-leet
-Version: 0.2.6
+Version: 0.2.7
 Summary: 
 Author: madmaxieee
 Author-email: 76544194+madmaxieee@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

