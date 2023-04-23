# Comparing `tmp/devchat-0.1.0.tar.gz` & `tmp/devchat-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devchat-0.1.0.tar", last modified: Mon Apr 17 14:16:20 2023, max compression
+gzip compressed data, was "devchat-0.1.1.tar", last modified: Sun Apr 23 13:13:47 2023, max compression
```

## Comparing `devchat-0.1.0.tar` & `devchat-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,27 @@
-drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-04-17 14:16:20.492434 devchat-0.1.0/
--rw-r--r--   0 basicthinker   (501) staff       (20)    11357 2023-04-17 07:54:02.000000 devchat-0.1.0/LICENSE
--rw-r--r--   0 basicthinker   (501) staff       (20)       73 2023-04-17 14:16:20.492257 devchat-0.1.0/PKG-INFO
--rw-r--r--   0 basicthinker   (501) staff       (20)       44 2023-04-17 09:53:56.000000 devchat-0.1.0/README.md
-drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-04-17 14:16:20.490696 devchat-0.1.0/devchat/
--rw-r--r--   0 basicthinker   (501) staff       (20)        0 2023-04-17 08:20:09.000000 devchat-0.1.0/devchat/__init__.py
--rw-r--r--   0 basicthinker   (501) staff       (20)       37 2023-04-17 10:00:47.000000 devchat-0.1.0/devchat/_cli.py
-drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-04-17 14:16:20.491714 devchat-0.1.0/devchat.egg-info/
--rw-r--r--   0 basicthinker   (501) staff       (20)       73 2023-04-17 14:16:20.000000 devchat-0.1.0/devchat.egg-info/PKG-INFO
--rw-r--r--   0 basicthinker   (501) staff       (20)      253 2023-04-17 14:16:20.000000 devchat-0.1.0/devchat.egg-info/SOURCES.txt
--rw-r--r--   0 basicthinker   (501) staff       (20)        1 2023-04-17 14:16:20.000000 devchat-0.1.0/devchat.egg-info/dependency_links.txt
--rw-r--r--   0 basicthinker   (501) staff       (20)       46 2023-04-17 14:16:20.000000 devchat-0.1.0/devchat.egg-info/entry_points.txt
--rw-r--r--   0 basicthinker   (501) staff       (20)        8 2023-04-17 14:16:20.000000 devchat-0.1.0/devchat.egg-info/top_level.txt
--rw-r--r--   0 basicthinker   (501) staff       (20)      102 2023-04-17 09:50:08.000000 devchat-0.1.0/pyproject.toml
--rw-r--r--   0 basicthinker   (501) staff       (20)       38 2023-04-17 14:16:20.492476 devchat-0.1.0/setup.cfg
--rw-r--r--   0 basicthinker   (501) staff       (20)      234 2023-04-17 09:49:34.000000 devchat-0.1.0/setup.py
-drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-04-17 14:16:20.491891 devchat-0.1.0/tests/
--rw-r--r--   0 basicthinker   (501) staff       (20)      247 2023-04-17 14:07:53.000000 devchat-0.1.0/tests/test_cli.py
+drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-04-23 13:13:47.984140 devchat-0.1.1/
+-rw-r--r--   0 basicthinker   (501) staff       (20)    11357 2023-04-17 07:54:02.000000 devchat-0.1.1/LICENSE
+-rw-r--r--   0 basicthinker   (501) staff       (20)       73 2023-04-23 13:13:47.984020 devchat-0.1.1/PKG-INFO
+-rw-r--r--   0 basicthinker   (501) staff       (20)       44 2023-04-17 09:53:56.000000 devchat-0.1.1/README.md
+drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-04-23 13:13:47.982713 devchat-0.1.1/devchat/
+-rw-r--r--   0 basicthinker   (501) staff       (20)        0 2023-04-17 08:20:09.000000 devchat-0.1.1/devchat/__init__.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     4607 2023-04-23 12:43:58.000000 devchat-0.1.1/devchat/_cli.py
+drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-04-23 13:13:47.983549 devchat-0.1.1/devchat/chat/
+-rw-r--r--   0 basicthinker   (501) staff       (20)       43 2023-04-23 12:43:58.000000 devchat-0.1.1/devchat/chat/__init__.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     1203 2023-04-23 12:43:58.000000 devchat-0.1.1/devchat/chat/chat.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     3198 2023-04-23 12:43:58.000000 devchat-0.1.1/devchat/chat/openai_chat.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     2999 2023-04-23 12:43:58.000000 devchat-0.1.1/devchat/message.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     3687 2023-04-23 12:43:58.000000 devchat-0.1.1/devchat/prompt.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)      332 2023-04-23 12:43:58.000000 devchat-0.1.1/devchat/utils.py
+drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-04-23 13:13:47.983249 devchat-0.1.1/devchat.egg-info/
+-rw-r--r--   0 basicthinker   (501) staff       (20)       73 2023-04-23 13:13:47.000000 devchat-0.1.1/devchat.egg-info/PKG-INFO
+-rw-r--r--   0 basicthinker   (501) staff       (20)      424 2023-04-23 13:13:47.000000 devchat-0.1.1/devchat.egg-info/SOURCES.txt
+-rw-r--r--   0 basicthinker   (501) staff       (20)        1 2023-04-23 13:13:47.000000 devchat-0.1.1/devchat.egg-info/dependency_links.txt
+-rw-r--r--   0 basicthinker   (501) staff       (20)       46 2023-04-23 13:13:47.000000 devchat-0.1.1/devchat.egg-info/entry_points.txt
+-rw-r--r--   0 basicthinker   (501) staff       (20)        8 2023-04-23 13:13:47.000000 devchat-0.1.1/devchat.egg-info/top_level.txt
+-rw-r--r--   0 basicthinker   (501) staff       (20)      102 2023-04-17 09:50:08.000000 devchat-0.1.1/pyproject.toml
+-rw-r--r--   0 basicthinker   (501) staff       (20)       38 2023-04-23 13:13:47.984174 devchat-0.1.1/setup.cfg
+-rw-r--r--   0 basicthinker   (501) staff       (20)      234 2023-04-23 13:11:39.000000 devchat-0.1.1/setup.py
+drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-04-23 13:13:47.983868 devchat-0.1.1/tests/
+-rw-r--r--   0 basicthinker   (501) staff       (20)     1175 2023-04-23 12:43:58.000000 devchat-0.1.1/tests/test_cli.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     2049 2023-04-23 12:43:58.000000 devchat-0.1.1/tests/test_message.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     3033 2023-04-23 12:43:58.000000 devchat-0.1.1/tests/test_prompt.py
```

### Comparing `devchat-0.1.0/LICENSE` & `devchat-0.1.1/LICENSE`

 * *Files identical despite different names*

