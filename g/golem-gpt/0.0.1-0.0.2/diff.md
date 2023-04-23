# Comparing `tmp/golem-gpt-0.0.1.tar.gz` & `tmp/golem-gpt-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "golem-gpt-0.0.1.tar", last modified: Sun Apr 23 14:25:19 2023, max compression
+gzip compressed data, was "golem-gpt-0.0.2.tar", last modified: Sun Apr 23 21:47:45 2023, max compression
```

## Comparing `golem-gpt-0.0.1.tar` & `golem-gpt-0.0.2.tar`

### file list

```diff
@@ -1,74 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:25:19.874290 golem-gpt-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-23 14:25:01.000000 golem-gpt-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-04-23 14:25:19.874290 golem-gpt-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-04-23 14:25:01.000000 golem-gpt-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:25:19.870290 golem-gpt-0.0.1/golem_gpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-04-23 14:25:19.000000 golem-gpt-0.0.1/golem_gpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-04-23 14:25:19.000000 golem-gpt-0.0.1/golem_gpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 14:25:19.000000 golem-gpt-0.0.1/golem_gpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-23 14:25:19.000000 golem-gpt-0.0.1/golem_gpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-23 14:25:19.000000 golem-gpt-0.0.1/golem_gpt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:25:19.870290 golem-gpt-0.0.1/golemgpt/
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-23 14:25:01.000000 golem-gpt-0.0.1/golemgpt/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:25:19.870290 golem-gpt-0.0.1/golemgpt/actions/
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-23 14:25:01.000000 golem-gpt-0.0.1/golemgpt/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-23 14:25:01.000000 golem-gpt-0.0.1/golemgpt/actions/ask_google.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-23 14:25:01.000000 golem-gpt-0.0.1/golemgpt/actions/ask_human_input.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-23 14:25:01.000000 golem-gpt-0.0.1/golemgpt/actions/create_python_script.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-23 14:25:01.000000 golem-gpt-0.0.1/golemgpt/actions/create_shell_script.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-23 14:25:01.000000 golem-gpt-0.0.1/golemgpt/actions/delegate_job.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-23 14:25:01.000000 golem-gpt-0.0.1/golemgpt/actions/explain.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-23 14:25:01.000000 golem-gpt-0.0.1/golemgpt/actions/finish_job.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-23 14:25:01.000000 golem-gpt-0.0.1/golemgpt/actions/get_local_date.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-23 14:25:01.000000 golem-gpt-0.0.1/golemgpt/actions/get_os_details.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-23 14:25:01.000000 golem-gpt-0.0.1/golemgpt/actions/http_download.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-23 14:25:01.000000 golem-gpt-0.0.1/golemgpt/actions/read_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-23 14:25:01.000000 golem-gpt-0.0.1/golemgpt/actions/reject_job.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-23 14:25:01.000000 golem-gpt-0.0.1/golemgpt/actions/run_script.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-23 14:25:01.000000 golem-gpt-0.0.1/golemgpt/actions/write_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:25:19.870290 golem-gpt-0.0.1/golemgpt/codex/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-23 14:25:01.000000 golem-gpt-0.0.1/golemgpt/codex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-23 14:25:01.000000 golem-gpt-0.0.1/golemgpt/codex/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-23 14:25:01.000000 golem-gpt-0.0.1/golemgpt/codex/reasonable.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-23 14:25:01.000000 golem-gpt-0.0.1/golemgpt/codex/unaware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:25:19.870290 golem-gpt-0.0.1/golemgpt/cognitron/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-23 14:25:01.000000 golem-gpt-0.0.1/golemgpt/cognitron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-23 14:25:01.000000 golem-gpt-0.0.1/golemgpt/cognitron/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-04-23 14:25:01.000000 golem-gpt-0.0.1/golemgpt/cognitron/openai.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:25:19.870290 golem-gpt-0.0.1/golemgpt/golems/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-23 14:25:01.000000 golem-gpt-0.0.1/golemgpt/golems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-04-23 14:25:01.000000 golem-gpt-0.0.1/golemgpt/golems/general.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:25:19.874290 golem-gpt-0.0.1/golemgpt/golems/roles/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 14:25:01.000000 golem-gpt-0.0.1/golemgpt/golems/roles/artist.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-23 14:25:01.000000 golem-gpt-0.0.1/golemgpt/golems/roles/director.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 14:25:01.000000 golem-gpt-0.0.1/golemgpt/golems/roles/programmer.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 14:25:01.000000 golem-gpt-0.0.1/golemgpt/golems/roles/reviewer.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 14:25:01.000000 golem-gpt-0.0.1/golemgpt/golems/roles/security.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 14:25:01.000000 golem-gpt-0.0.1/golemgpt/golems/roles/webdesigner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:25:19.874290 golem-gpt-0.0.1/golemgpt/lexicon/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-23 14:25:01.000000 golem-gpt-0.0.1/golemgpt/lexicon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-04-23 14:25:01.000000 golem-gpt-0.0.1/golemgpt/lexicon/general.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-23 14:25:01.000000 golem-gpt-0.0.1/golemgpt/lexicon/prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:25:19.874290 golem-gpt-0.0.1/golemgpt/memory/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-23 14:25:01.000000 golem-gpt-0.0.1/golemgpt/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-04-23 14:25:01.000000 golem-gpt-0.0.1/golemgpt/memory/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-23 14:25:01.000000 golem-gpt-0.0.1/golemgpt/memory/localfiles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:25:19.874290 golem-gpt-0.0.1/golemgpt/runners/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-23 14:25:01.000000 golem-gpt-0.0.1/golemgpt/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-23 14:25:01.000000 golem-gpt-0.0.1/golemgpt/runners/alwaysask.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-23 14:25:01.000000 golem-gpt-0.0.1/golemgpt/runners/justdo.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-23 14:25:01.000000 golem-gpt-0.0.1/golemgpt/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:25:19.874290 golem-gpt-0.0.1/golemgpt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-23 14:25:01.000000 golem-gpt-0.0.1/golemgpt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-23 14:25:01.000000 golem-gpt-0.0.1/golemgpt/utils/console.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-23 14:25:01.000000 golem-gpt-0.0.1/golemgpt/utils/environ.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-23 14:25:01.000000 golem-gpt-0.0.1/golemgpt/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-23 14:25:01.000000 golem-gpt-0.0.1/golemgpt/utils/http.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:25:19.874290 golem-gpt-0.0.1/golemgpt/utils/images/
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-23 14:25:01.000000 golem-gpt-0.0.1/golemgpt/utils/images/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-23 14:25:01.000000 golem-gpt-0.0.1/golemgpt/utils/images/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-23 14:25:01.000000 golem-gpt-0.0.1/golemgpt/utils/images/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-23 14:25:01.000000 golem-gpt-0.0.1/golemgpt/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-23 14:25:01.000000 golem-gpt-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-23 14:25:01.000000 golem-gpt-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 14:25:19.874290 golem-gpt-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:47:45.579488 golem-gpt-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-23 21:47:26.000000 golem-gpt-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-04-23 21:47:45.579488 golem-gpt-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-04-23 21:47:26.000000 golem-gpt-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:47:45.575488 golem-gpt-0.0.2/golem_gpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-04-23 21:47:45.000000 golem-gpt-0.0.2/golem_gpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-23 21:47:45.000000 golem-gpt-0.0.2/golem_gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 21:47:45.000000 golem-gpt-0.0.2/golem_gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-23 21:47:45.000000 golem-gpt-0.0.2/golem_gpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-23 21:47:45.000000 golem-gpt-0.0.2/golem_gpt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:47:45.575488 golem-gpt-0.0.2/golemgpt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-23 21:47:26.000000 golem-gpt-0.0.2/golemgpt/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:47:45.575488 golem-gpt-0.0.2/golemgpt/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-23 21:47:26.000000 golem-gpt-0.0.2/golemgpt/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-23 21:47:26.000000 golem-gpt-0.0.2/golemgpt/actions/ask_google.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-23 21:47:26.000000 golem-gpt-0.0.2/golemgpt/actions/ask_human_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-23 21:47:26.000000 golem-gpt-0.0.2/golemgpt/actions/create_python_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-23 21:47:26.000000 golem-gpt-0.0.2/golemgpt/actions/create_shell_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-23 21:47:26.000000 golem-gpt-0.0.2/golemgpt/actions/delegate_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-23 21:47:26.000000 golem-gpt-0.0.2/golemgpt/actions/explain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-23 21:47:26.000000 golem-gpt-0.0.2/golemgpt/actions/finish_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-23 21:47:26.000000 golem-gpt-0.0.2/golemgpt/actions/get_local_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-23 21:47:26.000000 golem-gpt-0.0.2/golemgpt/actions/get_os_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-23 21:47:26.000000 golem-gpt-0.0.2/golemgpt/actions/http_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-23 21:47:26.000000 golem-gpt-0.0.2/golemgpt/actions/read_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-23 21:47:26.000000 golem-gpt-0.0.2/golemgpt/actions/reject_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-23 21:47:26.000000 golem-gpt-0.0.2/golemgpt/actions/run_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-23 21:47:26.000000 golem-gpt-0.0.2/golemgpt/actions/summarize_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-23 21:47:26.000000 golem-gpt-0.0.2/golemgpt/actions/write_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:47:45.575488 golem-gpt-0.0.2/golemgpt/codex/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-23 21:47:26.000000 golem-gpt-0.0.2/golemgpt/codex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-23 21:47:26.000000 golem-gpt-0.0.2/golemgpt/codex/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-23 21:47:26.000000 golem-gpt-0.0.2/golemgpt/codex/reasonable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-23 21:47:26.000000 golem-gpt-0.0.2/golemgpt/codex/unaware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:47:45.575488 golem-gpt-0.0.2/golemgpt/cognitron/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-23 21:47:26.000000 golem-gpt-0.0.2/golemgpt/cognitron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-23 21:47:26.000000 golem-gpt-0.0.2/golemgpt/cognitron/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-04-23 21:47:26.000000 golem-gpt-0.0.2/golemgpt/cognitron/openai.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:47:45.575488 golem-gpt-0.0.2/golemgpt/golems/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-23 21:47:26.000000 golem-gpt-0.0.2/golemgpt/golems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-04-23 21:47:26.000000 golem-gpt-0.0.2/golemgpt/golems/general.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:47:45.579488 golem-gpt-0.0.2/golemgpt/golems/roles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 21:47:26.000000 golem-gpt-0.0.2/golemgpt/golems/roles/artist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-23 21:47:26.000000 golem-gpt-0.0.2/golemgpt/golems/roles/director.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 21:47:26.000000 golem-gpt-0.0.2/golemgpt/golems/roles/programmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 21:47:26.000000 golem-gpt-0.0.2/golemgpt/golems/roles/reviewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 21:47:26.000000 golem-gpt-0.0.2/golemgpt/golems/roles/security.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 21:47:26.000000 golem-gpt-0.0.2/golemgpt/golems/roles/webdesigner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:47:45.579488 golem-gpt-0.0.2/golemgpt/lexicon/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-23 21:47:26.000000 golem-gpt-0.0.2/golemgpt/lexicon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-04-23 21:47:26.000000 golem-gpt-0.0.2/golemgpt/lexicon/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-04-23 21:47:26.000000 golem-gpt-0.0.2/golemgpt/lexicon/prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:47:45.579488 golem-gpt-0.0.2/golemgpt/memory/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-23 21:47:26.000000 golem-gpt-0.0.2/golemgpt/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-04-23 21:47:26.000000 golem-gpt-0.0.2/golemgpt/memory/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-23 21:47:26.000000 golem-gpt-0.0.2/golemgpt/memory/localfiles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:47:45.579488 golem-gpt-0.0.2/golemgpt/runners/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-23 21:47:26.000000 golem-gpt-0.0.2/golemgpt/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-23 21:47:26.000000 golem-gpt-0.0.2/golemgpt/runners/alwaysask.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-23 21:47:26.000000 golem-gpt-0.0.2/golemgpt/runners/justdo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-23 21:47:26.000000 golem-gpt-0.0.2/golemgpt/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:47:45.579488 golem-gpt-0.0.2/golemgpt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-23 21:47:26.000000 golem-gpt-0.0.2/golemgpt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-23 21:47:26.000000 golem-gpt-0.0.2/golemgpt/utils/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-23 21:47:26.000000 golem-gpt-0.0.2/golemgpt/utils/environ.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-23 21:47:26.000000 golem-gpt-0.0.2/golemgpt/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-23 21:47:26.000000 golem-gpt-0.0.2/golemgpt/utils/http.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:47:45.579488 golem-gpt-0.0.2/golemgpt/utils/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-23 21:47:26.000000 golem-gpt-0.0.2/golemgpt/utils/images/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-23 21:47:26.000000 golem-gpt-0.0.2/golemgpt/utils/images/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-23 21:47:26.000000 golem-gpt-0.0.2/golemgpt/utils/images/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-23 21:47:26.000000 golem-gpt-0.0.2/golemgpt/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-23 21:47:26.000000 golem-gpt-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-23 21:47:26.000000 golem-gpt-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 21:47:45.579488 golem-gpt-0.0.2/setup.cfg
```

### Comparing `golem-gpt-0.0.1/LICENSE` & `golem-gpt-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `golem-gpt-0.0.1/PKG-INFO` & `golem-gpt-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: golem-gpt
-Version: 0.0.1
+Version: 0.0.2
 Summary: Framework for building actionable agents on top of GPT-4
 Author-email: Alexey Kinev <rudy@05bit.com>
 Project-URL: Homepage, https://github.com/Dingolytics/golem-gpt
 Project-URL: Bug Tracker, https://github.com/Dingolytics/golem-gpt/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Golem-GPT 
 =========
 
-![Docker Image Size (latest by date)](https://img.shields.io/docker/image-size/dingolytics/golem-gpt?sort=date)
+![PyPI](https://img.shields.io/pypi/v/golem-gpt) ![PyPI - Status](https://img.shields.io/pypi/status/golem-gpt) ![Docker Image Size (latest by date)](https://img.shields.io/docker/image-size/dingolytics/golem-gpt?sort=date)
 
 ⚠️ **This is an experimental development. Run it on your own risk!** ⚠️
 
 Framework for building actionable agents to achieve goals specified
 by user, powered by [OpenAI](https://openai.com) [GPT-4](https://openai.com/research/gpt-4)
 and [GPT-3.5](https://platform.openai.com/docs/models/gpt-3-5)
 
@@ -43,21 +43,28 @@
 OPENAI_API_KEY=...
 OPENAI_ORG_ID=...
 OPENAI_MODEL=gpt-4
 ```
 
 *(For `gpt-4` model you should have an early access enabled, it's not publicly available yet).*
 
-Run it:
+Run it via Docker Compose:
 
 ```bash
 docker compose build && docker compose run app
 ```
 
-It's also better to run it inside Docker to have it isolated. Because
+or via Python:
+
+```bash
+pip install --upgrade golem-gpt
+python -m golemgpt
+```
+
+❗️ It's safer to run it inside Docker to have it isolated. Because
 Golem can access an environment and filesystem, so it's better to keep
 it inside a container.
 
 
 Architecture
 ------------
```

### Comparing `golem-gpt-0.0.1/README.md` & `golem-gpt-0.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Golem-GPT 
 =========
 
-![Docker Image Size (latest by date)](https://img.shields.io/docker/image-size/dingolytics/golem-gpt?sort=date)
+![PyPI](https://img.shields.io/pypi/v/golem-gpt) ![PyPI - Status](https://img.shields.io/pypi/status/golem-gpt) ![Docker Image Size (latest by date)](https://img.shields.io/docker/image-size/dingolytics/golem-gpt?sort=date)
 
 ⚠️ **This is an experimental development. Run it on your own risk!** ⚠️
 
 Framework for building actionable agents to achieve goals specified
 by user, powered by [OpenAI](https://openai.com) [GPT-4](https://openai.com/research/gpt-4)
 and [GPT-3.5](https://platform.openai.com/docs/models/gpt-3-5)
 
@@ -28,21 +28,28 @@
 OPENAI_API_KEY=...
 OPENAI_ORG_ID=...
 OPENAI_MODEL=gpt-4
 ```
 
 *(For `gpt-4` model you should have an early access enabled, it's not publicly available yet).*
 
-Run it:
+Run it via Docker Compose:
 
 ```bash
 docker compose build && docker compose run app
 ```
 
-It's also better to run it inside Docker to have it isolated. Because
+or via Python:
+
+```bash
+pip install --upgrade golem-gpt
+python -m golemgpt
+```
+
+❗️ It's safer to run it inside Docker to have it isolated. Because
 Golem can access an environment and filesystem, so it's better to keep
 it inside a container.
 
 
 Architecture
 ------------
```

### Comparing `golem-gpt-0.0.1/golem_gpt.egg-info/PKG-INFO` & `golem-gpt-0.0.2/golem_gpt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: golem-gpt
-Version: 0.0.1
+Version: 0.0.2
 Summary: Framework for building actionable agents on top of GPT-4
 Author-email: Alexey Kinev <rudy@05bit.com>
 Project-URL: Homepage, https://github.com/Dingolytics/golem-gpt
 Project-URL: Bug Tracker, https://github.com/Dingolytics/golem-gpt/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Golem-GPT 
 =========
 
-![Docker Image Size (latest by date)](https://img.shields.io/docker/image-size/dingolytics/golem-gpt?sort=date)
+![PyPI](https://img.shields.io/pypi/v/golem-gpt) ![PyPI - Status](https://img.shields.io/pypi/status/golem-gpt) ![Docker Image Size (latest by date)](https://img.shields.io/docker/image-size/dingolytics/golem-gpt?sort=date)
 
 ⚠️ **This is an experimental development. Run it on your own risk!** ⚠️
 
 Framework for building actionable agents to achieve goals specified
 by user, powered by [OpenAI](https://openai.com) [GPT-4](https://openai.com/research/gpt-4)
 and [GPT-3.5](https://platform.openai.com/docs/models/gpt-3-5)
 
@@ -43,21 +43,28 @@
 OPENAI_API_KEY=...
 OPENAI_ORG_ID=...
 OPENAI_MODEL=gpt-4
 ```
 
 *(For `gpt-4` model you should have an early access enabled, it's not publicly available yet).*
 
-Run it:
+Run it via Docker Compose:
 
 ```bash
 docker compose build && docker compose run app
 ```
 
-It's also better to run it inside Docker to have it isolated. Because
+or via Python:
+
+```bash
+pip install --upgrade golem-gpt
+python -m golemgpt
+```
+
+❗️ It's safer to run it inside Docker to have it isolated. Because
 Golem can access an environment and filesystem, so it's better to keep
 it inside a container.
 
 
 Architecture
 ------------
```

### Comparing `golem-gpt-0.0.1/golem_gpt.egg-info/SOURCES.txt` & `golem-gpt-0.0.2/golem_gpt.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 golemgpt/actions/finish_job.py
 golemgpt/actions/get_local_date.py
 golemgpt/actions/get_os_details.py
 golemgpt/actions/http_download.py
 golemgpt/actions/read_file.py
 golemgpt/actions/reject_job.py
 golemgpt/actions/run_script.py
+golemgpt/actions/summarize_file.py
 golemgpt/actions/write_file.py
 golemgpt/codex/__init__.py
 golemgpt/codex/base.py
 golemgpt/codex/reasonable.py
 golemgpt/codex/unaware.py
 golemgpt/cognitron/__init__.py
 golemgpt/cognitron/base.py
```

### Comparing `golem-gpt-0.0.1/golemgpt/__main__.py` & `golem-gpt-0.0.2/golemgpt/__main__.py`

 * *Files identical despite different names*

### Comparing `golem-gpt-0.0.1/golemgpt/actions/__init__.py` & `golem-gpt-0.0.2/golemgpt/actions/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,27 +7,29 @@
 from .finish_job import finish_job_action
 from .get_local_date import get_local_date_action
 from .get_os_details import get_os_details_action
 from .http_download import http_download_action
 from .read_file import read_file_action
 from .reject_job import reject_job_action
 from .run_script import run_script_action
+from .summarize_file import summarize_file_action
 from .write_file import write_file_action
 
 __all__ = [
     'ALL_KNOWN_ACTIONS',
 ]
 
 ALL_KNOWN_ACTIONS = {
     'ask_human_input': ask_human_input_action,
     'ask_google': ask_google_action,
     #
     'http_download': http_download_action,
     #
     'read_file': read_file_action,
+    'summarize_file': summarize_file_action,
     'write_file': write_file_action,
     #
     'get_local_date': get_local_date_action,
     'get_os_details': get_os_details_action,
     #
     'create_python_script': create_python_script_action,
     'create_shell_script': create_shell_script_action,
```

### Comparing `golem-gpt-0.0.1/golemgpt/actions/http_download.py` & `golem-gpt-0.0.2/golemgpt/actions/http_download.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,17 +15,20 @@
 ) -> str:
     """Make an HTTP request and return its content."""
     try:
         path = workpath(out_filename)
     except ValueError:
         return f"File {out_filename} is outside of working dir."
 
-    http_download(
+    response = http_download(
         method=method, url=url, path=path, headers=headers,
         json=body if isinstance(body, (dict, list)) else None,
         body=body if isinstance(body, str) else None,
     )
 
+    if response.status in (401, 403):
+        return "HTTP request failed: maybe ask user for credentials?"
+
     file_size = path.stat().st_size
     return HTTP_REQUEST_PROMPT.format(
         out_filename=out_filename, file_size=file_size
     )
```

### Comparing `golem-gpt-0.0.1/golemgpt/actions/read_file.py` & `golem-gpt-0.0.2/golemgpt/actions/read_file.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,20 @@
-from pathlib import Path
+from golemgpt.utils import workpath
+from .summarize_file import summarize_file_action
 
-MAX_SIZE = 8096
+MAX_RAW_SIZE = 8096
 
 
 def read_file_action(filename: str, **kwargs) -> str:
     """Read a file and return its content."""
-    cwd = Path.cwd().absolute()
-    path = Path(Path.cwd() / filename).absolute()
-
-    if cwd in path.parents:
-        relname = path.relative_to(cwd)
-    else:
-        return f"Rejected, file {filename} is outside of working dir."
-
-    if not path.exists():
-        return f"Rejected, file {relname} does not exist."
-
+    path = workpath(filename, check_exists=True)
     file_size = path.stat().st_size
-    if path.stat().st_size > MAX_SIZE:
-        return f"File exists, but is too large ({file_size} bytes)."
-
+    if file_size > MAX_RAW_SIZE:
+        hint = kwargs.get('summazie_hint') or "essential data is needed"
+        return summarize_file_action(
+            filename, hint=hint, **kwargs
+        )
+        # raise PathRejected(
+        #     f"Error, file '{filename}' is too large ({file_size} bytes)."
+        # )
     with path.open("r") as file:
         return file.read()
```

### Comparing `golem-gpt-0.0.1/golemgpt/actions/run_script.py` & `golem-gpt-0.0.2/golemgpt/actions/run_script.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 import subprocess
 from golemgpt.utils import workpath
 
 
 def run_script_action(name: str, **kwargs) -> str:
     """Run a script and return its output."""
-    try:
-        path = workpath(name)
-    except ValueError as exc:
-        return f"Rejected: {exc}."
+    path = workpath(name)
 
     if not path.exists():
-        return f"Rejected: script {name} does not exist."
+        return f"Script {name} does not exist, can you create it?"
 
     if name.endswith('.py'):
         process = subprocess.Popen(['python', name])
     elif name.endswith('.sh'):
         process = subprocess.Popen(['sh', name])
     else:
         return f"Rejected: script {name} is not a Bash or Python script."
```

### Comparing `golem-gpt-0.0.1/golemgpt/codex/reasonable.py` & `golem-gpt-0.0.2/golemgpt/codex/reasonable.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from golemgpt.utils import console
 from golemgpt.utils.exceptions import AlignAcionsError
 from .base import BaseCodex, BaseCodexLexicon
 
 
 class ReasonableCodexLexicon(BaseCodexLexicon):
     def align_actions_prompt(self, action_plan: list) -> str:
-        question = f"In this action plan unharmful? Action:\n{action_plan}"
+        question = f"In this action plan unharmful? Actions: {action_plan}"
         return f"Answer just 'yes' or 'no'. {question}"
 
 
 class ReasonableCodex(BaseCodex):
     check_actions_depth = 3
     name = 'reasonable-codex'
     lexicon = ReasonableCodexLexicon()
 
     def align_actions(self, action_plan: list) -> str:
         check_actions = action_plan[:self.check_actions_depth]
         prompt = self.lexicon.align_actions_prompt(check_actions)
-        console.message(self.name, prompt)
+        brief = self.lexicon.align_actions_prompt('[...]')
+        # console.debug(self.name, prompt)
+        console.message(self.name, brief)
         if self.cognitron.ask_yesno(prompt):
             return True
-        raise AlignAcionsError()
+        raise AlignAcionsError(prompt)
```

### Comparing `golem-gpt-0.0.1/golemgpt/cognitron/base.py` & `golem-gpt-0.0.2/golemgpt/cognitron/base.py`

 * *Files identical despite different names*

### Comparing `golem-gpt-0.0.1/golemgpt/cognitron/openai.py` & `golem-gpt-0.0.2/golemgpt/cognitron/openai.py`

 * *Files identical despite different names*

### Comparing `golem-gpt-0.0.1/golemgpt/golems/general.py` & `golem-gpt-0.0.2/golemgpt/golems/general.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 from golemgpt.lexicon import GeneralLexicon
 from golemgpt.runners import JustDoRunner
 from golemgpt.settings import Settings
 from golemgpt.memory import BaseMemory
 from golemgpt.utils import console, genkey
 from golemgpt.cognitron.openai import OpenAICognitron
 from golemgpt.utils.exceptions import (
-    JobFinished, JobRejected, ParseActionsError, AlignAcionsError
+    GolemError, AlignAcionsError, JobFinished, JobRejected,
+    ParseActionsError, PathRejected,
 )
 
 DEFAULT_NAME = 'Golem-GPT'
 
 DEFAULT_RETRY_PLAN_ATTEMPTS = 3
 
 
@@ -55,17 +56,22 @@
                     self.plan_actions(outcome)
                     self.align_actions(outcome)
                 outcome = self.run_action()
             except JobFinished:
                 break
             except JobRejected:
                 break
-            except AlignAcionsError:
+            except PathRejected:
+                break
+            except AlignAcionsError as exc:
                 # TODO: Implement a retry plan mechanism after misalignment
+                console.info(f"Actions rejected: {exc}")
                 break
+            except GolemError as exc:
+                outcome = str(exc)
         #
         console.info(f"Job completed: {self.job_key}")
 
     def initialize(self) -> None:
         """Initialize the job state from memory or from scratch."""
         console.debug(f"Syncing job state with memory: {self.job_key}")
         self.memory.load(self.job_key)
@@ -77,25 +83,28 @@
                 self.memory.messages.append(message)
         else:
             self.goals = self.memory.goals
             assert self.goals
 
         self.memory.save()
     
-    def cognitron(self, memory: BaseMemory, **options) -> OpenAICognitron:
+    def cognitron(self, spawn: bool = False, **options) -> OpenAICognitron:
         """Return a Cognitron instance."""
+        if spawn:
+            key = f'{self.job_key}.{genkey()}'
+            memory = self.memory.spawn(key)
+        else:
+            memory = self.memory
         return self.cognitron_class(
             settings=self.settings, memory=memory, **options
         )
 
     def codex(self, **options) -> BaseCodex:
         """Return a Codex instance."""
-        key = f'{self.job_key}.{genkey()}'
-        memory = self.memory.spawn(key)
-        cognitron = self.cognitron(memory, name='', **options)
+        cognitron = self.cognitron(spawn=True, name='', **options)
         return self.codex_class(cognitron)
 
     def run_action(self) -> str:
         """Run the next action in the plan."""
         if not self.action_plan:
             raise JobFinished()
         action_item = self.action_plan.pop(0)
@@ -103,15 +112,15 @@
         if not result:
             return ''
         return self.lexicon.action_result_prompt(action, result)
 
     def plan_actions(self, prompt: str, attempt: int = 0) -> None:
         """Ask to update the plan based on the prompt."""
         console.message(self.name, prompt)
-        reply = self.cognitron(self.memory).communicate(prompt)
+        reply = self.cognitron().communicate(prompt)
         try:
             self.action_plan = self.lexicon.parse_reply(reply)
         except ParseActionsError:
             self.try_restore_plan(reply, attempt + 1)
 
     def align_actions(self, prompt: str) -> List[str]:
         """Align the action plan with the codex."""
@@ -132,12 +141,10 @@
         # Try to plan again after remainder about the format:
         remainder = self.lexicon.remind_format_prompt()
         self.plan_actions(remainder, attempt + 1)
 
     # TODO: Extract helper dialogs to a separate class (?)
     def helper_yesno(self, question: str) -> bool:
         """Guess if the reply is a yes or no."""
-        prompt = self.lexicon.guess_yesno_prompt(question)
-        key = f'{self.job_key}.{genkey()}'
-        memory = self.memory.spawn(key)
-        cognitron = self.cognitron(memory, name='Helper')
+        prompt = self.lexicon.yesno_prompt(question)
+        cognitron = self.cognitron(spawn=True, name='Helper')
         return cognitron.ask_yesno(prompt)
```

### Comparing `golem-gpt-0.0.1/golemgpt/golems/roles/director.py` & `golem-gpt-0.0.2/golemgpt/golems/roles/director.py`

 * *Files identical despite different names*

### Comparing `golem-gpt-0.0.1/golemgpt/lexicon/general.py` & `golem-gpt-0.0.2/golemgpt/lexicon/general.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     def action_result_prompt(self, action: str, result: str) -> str:
         return f'Completed "{action}" with result:\n{result}'
 
     def remind_format_prompt(self) -> str:
         return 'If finished, just use a single "finish_job" action.'
 
     def guess_finish_prompt(self, reply: str) -> str:
-        preamble = self.lexicon.find_preamble(reply)
+        preamble = self.find_preamble(reply)
         statement = preamble or reply
         return (
             "Does the following mean current job is finished "
             "(optional ask to start a new one)?"
             f"\n\n{statement}"
         )
```

### Comparing `golem-gpt-0.0.1/golemgpt/lexicon/prompts.py` & `golem-gpt-0.0.2/golemgpt/lexicon/prompts.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,16 +19,15 @@
 
 KNOWN_ACTIONS_PROMT = """
 You can use the following actions, higher in the list means
 the higher priority:
 
 - get_os_details:
 - get_local_date:
-- summarize_file: filename, hint, out_filename
-- read_file: filename
+- read_file: filename, summazie_hint
 - write_file: filename, content
 - http_download: url, method, headers, body, out_filename
 - run_script: name
 - ask_human_input: query
 - ask_google: query, out_filename
 - explain: comment
 - reject_job: message
```

### Comparing `golem-gpt-0.0.1/golemgpt/memory/base.py` & `golem-gpt-0.0.2/golemgpt/memory/base.py`

 * *Files identical despite different names*

### Comparing `golem-gpt-0.0.1/golemgpt/memory/localfiles.py` & `golem-gpt-0.0.2/golemgpt/memory/localfiles.py`

 * *Files identical despite different names*

### Comparing `golem-gpt-0.0.1/golemgpt/runners/justdo.py` & `golem-gpt-0.0.2/golemgpt/runners/justdo.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,10 +18,10 @@
 
     def __call__(self, action_item: dict, golem: Any) -> Tuple[str, str]:
         for key in action_item:
             if key not in self.known_actions:
                 raise UnknownAction(key)
             action_fn = self.known_actions[key]
             kwargs = action_item[key]
-            result = action_fn(**kwargs)
+            result = action_fn(golem=golem, **kwargs)
             break
         return (key, result)
```

### Comparing `golem-gpt-0.0.1/golemgpt/utils/console.py` & `golem-gpt-0.0.2/golemgpt/utils/console.py`

 * *Files identical despite different names*

### Comparing `golem-gpt-0.0.1/golemgpt/utils/exceptions.py` & `golem-gpt-0.0.2/golemgpt/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `golem-gpt-0.0.1/golemgpt/utils/http.py` & `golem-gpt-0.0.2/golemgpt/utils/http.py`

 * *Files identical despite different names*

### Comparing `golem-gpt-0.0.1/golemgpt/utils/images/__main__.py` & `golem-gpt-0.0.2/golemgpt/utils/images/__main__.py`

 * *Files identical despite different names*

### Comparing `golem-gpt-0.0.1/golemgpt/utils/images/prompt.py` & `golem-gpt-0.0.2/golemgpt/utils/images/prompt.py`

 * *Files identical despite different names*

### Comparing `golem-gpt-0.0.1/pyproject.toml` & `golem-gpt-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "golem-gpt"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Alexey Kinev", email="rudy@05bit.com" },
 ]
 description = "Framework for building actionable agents on top of GPT-4"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
+    "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 dynamic = ["dependencies"]
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
```

