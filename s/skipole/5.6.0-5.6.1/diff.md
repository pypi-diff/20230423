# Comparing `tmp/skipole-5.6.0.tar.gz` & `tmp/skipole-5.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skipole-5.6.0.tar", last modified: Fri Mar 31 13:45:13 2023, max compression
+gzip compressed data, was "skipole-5.6.1.tar", last modified: Sat Apr 22 21:55:19 2023, max compression
```

## Comparing `skipole-5.6.0.tar` & `skipole-5.6.1.tar`

### file list

```diff
@@ -1,81 +1,81 @@
--rw-r--r--   0        0        0     1083 2023-03-13 22:29:51.000000 skipole-5.6.0/LICENSE
--rw-r--r--   0        0        0     3108 2023-03-09 17:15:52.000000 skipole-5.6.0/README.md
--rw-r--r--   0        0        0      652 2023-03-31 13:29:01.000000 skipole-5.6.0/pyproject.toml
--rw-r--r--   0        0        0    12374 2023-03-14 15:51:15.000000 skipole-5.6.0/skipole/__init__.py
--rw-r--r--   0        0        0     6217 2023-03-14 15:48:58.000000 skipole-5.6.0/skipole/__main__.py
--rw-r--r--   0        0        0        0 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/ski/__init__.py
--rw-r--r--   0        0        0    13408 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/ski/dump_project.py
--rw-r--r--   0        0        0     7316 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/ski/excepts.py
--rw-r--r--   0        0        0    13948 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/ski/folder_class_definition.py
--rw-r--r--   0        0        0    65570 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/ski/page_class_definition.py
--rw-r--r--   0        0        0    87796 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/ski/project_class_definition.py
--rw-r--r--   0        0        0    38224 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/ski/read_json.py
--rw-r--r--   0        0        0    19088 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/ski/responders/__init__.py
--rw-r--r--   0        0        0    30231 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/ski/responders/checkers.py
--rw-r--r--   0        0        0    10690 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/ski/responders/navigators.py
--rw-r--r--   0        0        0    35881 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/ski/responders/submitters.py
--rw-r--r--   0        0        0    23819 2023-03-31 13:33:27.000000 skipole-5.6.0/skipole/ski/skiboot.py
--rw-r--r--   0        0        0    42472 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/ski/tag.py
--rw-r--r--   0        0        0     6829 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/ski/validators/__init__.py
--rw-r--r--   0        0        0     6169 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/ski/validators/basic.py
--rw-r--r--   0        0        0     3623 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/ski/validators/paths.py
--rw-r--r--   0        0        0    81450 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/ski/widgets/__init__.py
--rw-r--r--   0        0        0    30300 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/ski/widgets/checkbox.py
--rw-r--r--   0        0        0    25542 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/ski/widgets/confirm.py
--rw-r--r--   0        0        0     7832 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/ski/widgets/debug_tools.py
--rw-r--r--   0        0        0    15969 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/ski/widgets/dropdown.py
--rw-r--r--   0        0        0    16436 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/ski/widgets/error_messages.py
--rw-r--r--   0        0        0     2362 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/ski/widgets/footers.py
--rw-r--r--   0        0        0    34637 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/ski/widgets/headers.py
--rw-r--r--   0        0        0    20807 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/ski/widgets/info.py
--rw-r--r--   0        0        0    33443 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/ski/widgets/inputforms.py
--rw-r--r--   0        0        0    55725 2023-03-31 13:06:11.000000 skipole-5.6.0/skipole/ski/widgets/inputtables.py
--rw-r--r--   0        0        0   103036 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/ski/widgets/inputtext.py
--rw-r--r--   0        0        0   141485 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/ski/widgets/links.py
--rw-r--r--   0        0        0    18537 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/ski/widgets/lists.py
--rw-r--r--   0        0        0    25272 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/ski/widgets/logins.py
--rw-r--r--   0        0        0    33440 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/ski/widgets/paras.py
--rw-r--r--   0        0        0    24454 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/ski/widgets/radio.py
--rw-r--r--   0        0        0    24121 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/ski/widgets/svgbasics.py
--rw-r--r--   0        0        0   112572 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/ski/widgets/svggraphs.py
--rw-r--r--   0        0        0    40706 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/ski/widgets/svgmeters.py
--rw-r--r--   0        0        0    22543 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/ski/widgets/tables.py
--rw-r--r--   0        0        0    11640 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/ski/widgets/textarea.py
--rw-r--r--   0        0        0    19986 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/ski/widgets/upload.py
--rw-r--r--   0        0        0     1442 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/skis.py
--rw-r--r--   0        0        0       86 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/skis/data/defaults.json
--rw-r--r--   0        0        0    31135 2023-03-31 13:33:59.000000 skipole-5.6.0/skipole/skis/data/project.json
--rw-r--r--   0        0        0     2563 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/skis/data/textblocks_json/en.json
--rw-r--r--   0        0        0     1524 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/skis/static/css/theme1.css
--rw-r--r--   0        0        0     1524 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/skis/static/css/theme2.css
--rw-r--r--   0        0        0     1524 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/skis/static/css/theme3.css
--rw-r--r--   0        0        0     1524 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/skis/static/css/theme4.css
--rw-r--r--   0        0        0    23363 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/skis/static/css/w3.css
--rw-r--r--   0        0        0     4111 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/skis/static/js/basic.js
--rw-r--r--   0        0        0    10105 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/skis/static/js/checkbox.js
--rw-r--r--   0        0        0    18982 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/skis/static/js/confirm.js
--rw-r--r--   0        0        0     2623 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/skis/static/js/debug_tools.js
--rw-r--r--   0        0        0     5460 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/skis/static/js/dropdown.js
--rw-r--r--   0        0        0    12557 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/skis/static/js/error_messages.js
--rw-r--r--   0        0        0      901 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/skis/static/js/footers.js
--rw-r--r--   0        0        0    22423 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/skis/static/js/headers.js
--rw-r--r--   0        0        0     5592 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/skis/static/js/info.js
--rw-r--r--   0        0        0    18833 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/skis/static/js/inputforms.js
--rw-r--r--   0        0        0    22809 2023-03-30 22:04:38.000000 skipole-5.6.0/skipole/skis/static/js/inputtables.js
--rw-r--r--   0        0        0    33480 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/skis/static/js/inputtext.js
--rw-r--r--   0        0        0    89476 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/skis/static/js/jquery-3.5.1.min.js
--rw-r--r--   0        0        0    67496 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/skis/static/js/links.js
--rw-r--r--   0        0        0    12288 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/skis/static/js/lists.js
--rw-r--r--   0        0        0     8094 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/skis/static/js/logins.js
--rw-r--r--   0        0        0    32273 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/skis/static/js/paras.js
--rw-r--r--   0        0        0     1165 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/skis/static/js/paths.js
--rw-r--r--   0        0        0     3986 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/skis/static/js/radio.js
--rw-r--r--   0        0        0    31948 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/skis/static/js/skipole.js
--rw-r--r--   0        0        0    10529 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/skis/static/js/svgbasics.js
--rw-r--r--   0        0        0    16505 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/skis/static/js/svggraphs.js
--rw-r--r--   0        0        0     7060 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/skis/static/js/svgmeters.js
--rw-r--r--   0        0        0     4373 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/skis/static/js/tables.js
--rw-r--r--   0        0        0     2287 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/skis/static/js/textarea.js
--rw-r--r--   0        0        0     3001 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/skis/static/js/upload.js
--rw-r--r--   0        0        0     9268 2023-03-09 17:15:52.000000 skipole-5.6.0/skipole/textblocks.py
--rw-r--r--   0        0        0     3653 1970-01-01 00:00:00.000000 skipole-5.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-03-13 22:29:51.000000 skipole-5.6.1/LICENSE
+-rw-r--r--   0        0        0     3108 2023-03-09 17:15:52.000000 skipole-5.6.1/README.md
+-rw-r--r--   0        0        0      652 2023-04-13 08:25:22.000000 skipole-5.6.1/pyproject.toml
+-rw-r--r--   0        0        0    12374 2023-03-14 15:51:15.000000 skipole-5.6.1/skipole/__init__.py
+-rw-r--r--   0        0        0     6217 2023-03-14 15:48:58.000000 skipole-5.6.1/skipole/__main__.py
+-rw-r--r--   0        0        0        0 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/ski/__init__.py
+-rw-r--r--   0        0        0    13408 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/ski/dump_project.py
+-rw-r--r--   0        0        0     7316 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/ski/excepts.py
+-rw-r--r--   0        0        0    13948 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/ski/folder_class_definition.py
+-rw-r--r--   0        0        0    65570 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/ski/page_class_definition.py
+-rw-r--r--   0        0        0    87796 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/ski/project_class_definition.py
+-rw-r--r--   0        0        0    38224 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/ski/read_json.py
+-rw-r--r--   0        0        0    19088 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/ski/responders/__init__.py
+-rw-r--r--   0        0        0    30231 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/ski/responders/checkers.py
+-rw-r--r--   0        0        0    10690 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/ski/responders/navigators.py
+-rw-r--r--   0        0        0    35881 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/ski/responders/submitters.py
+-rw-r--r--   0        0        0    23819 2023-04-13 08:24:25.000000 skipole-5.6.1/skipole/ski/skiboot.py
+-rw-r--r--   0        0        0    42472 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/ski/tag.py
+-rw-r--r--   0        0        0     6829 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/ski/validators/__init__.py
+-rw-r--r--   0        0        0     8010 2023-04-17 23:29:11.000000 skipole-5.6.1/skipole/ski/validators/basic.py
+-rw-r--r--   0        0        0     3623 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/ski/validators/paths.py
+-rw-r--r--   0        0        0    81450 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/ski/widgets/__init__.py
+-rw-r--r--   0        0        0    30300 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/ski/widgets/checkbox.py
+-rw-r--r--   0        0        0    25542 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/ski/widgets/confirm.py
+-rw-r--r--   0        0        0     7832 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/ski/widgets/debug_tools.py
+-rw-r--r--   0        0        0    15969 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/ski/widgets/dropdown.py
+-rw-r--r--   0        0        0    16436 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/ski/widgets/error_messages.py
+-rw-r--r--   0        0        0     2362 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/ski/widgets/footers.py
+-rw-r--r--   0        0        0    34637 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/ski/widgets/headers.py
+-rw-r--r--   0        0        0    20807 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/ski/widgets/info.py
+-rw-r--r--   0        0        0    33443 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/ski/widgets/inputforms.py
+-rw-r--r--   0        0        0    56580 2023-04-14 14:06:12.000000 skipole-5.6.1/skipole/ski/widgets/inputtables.py
+-rw-r--r--   0        0        0   103333 2023-04-18 09:19:28.000000 skipole-5.6.1/skipole/ski/widgets/inputtext.py
+-rw-r--r--   0        0        0   141485 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/ski/widgets/links.py
+-rw-r--r--   0        0        0    18537 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/ski/widgets/lists.py
+-rw-r--r--   0        0        0    25272 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/ski/widgets/logins.py
+-rw-r--r--   0        0        0    33440 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/ski/widgets/paras.py
+-rw-r--r--   0        0        0    24454 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/ski/widgets/radio.py
+-rw-r--r--   0        0        0    24121 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/ski/widgets/svgbasics.py
+-rw-r--r--   0        0        0   112572 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/ski/widgets/svggraphs.py
+-rw-r--r--   0        0        0    40706 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/ski/widgets/svgmeters.py
+-rw-r--r--   0        0        0    22543 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/ski/widgets/tables.py
+-rw-r--r--   0        0        0    11640 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/ski/widgets/textarea.py
+-rw-r--r--   0        0        0    19986 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/ski/widgets/upload.py
+-rw-r--r--   0        0        0     1442 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/skis.py
+-rw-r--r--   0        0        0       86 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/skis/data/defaults.json
+-rw-r--r--   0        0        0    31135 2023-04-13 08:25:01.000000 skipole-5.6.1/skipole/skis/data/project.json
+-rw-r--r--   0        0        0     2563 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/skis/data/textblocks_json/en.json
+-rw-r--r--   0        0        0     1524 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/skis/static/css/theme1.css
+-rw-r--r--   0        0        0     1524 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/skis/static/css/theme2.css
+-rw-r--r--   0        0        0     1524 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/skis/static/css/theme3.css
+-rw-r--r--   0        0        0     1524 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/skis/static/css/theme4.css
+-rw-r--r--   0        0        0    23363 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/skis/static/css/w3.css
+-rw-r--r--   0        0        0     4515 2023-04-18 22:16:52.000000 skipole-5.6.1/skipole/skis/static/js/basic.js
+-rw-r--r--   0        0        0    10105 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/skis/static/js/checkbox.js
+-rw-r--r--   0        0        0    18982 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/skis/static/js/confirm.js
+-rw-r--r--   0        0        0     2623 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/skis/static/js/debug_tools.js
+-rw-r--r--   0        0        0     5460 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/skis/static/js/dropdown.js
+-rw-r--r--   0        0        0    12557 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/skis/static/js/error_messages.js
+-rw-r--r--   0        0        0      901 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/skis/static/js/footers.js
+-rw-r--r--   0        0        0    22423 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/skis/static/js/headers.js
+-rw-r--r--   0        0        0     5592 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/skis/static/js/info.js
+-rw-r--r--   0        0        0    18833 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/skis/static/js/inputforms.js
+-rw-r--r--   0        0        0    25467 2023-04-14 13:29:18.000000 skipole-5.6.1/skipole/skis/static/js/inputtables.js
+-rw-r--r--   0        0        0    33804 2023-04-18 09:23:00.000000 skipole-5.6.1/skipole/skis/static/js/inputtext.js
+-rw-r--r--   0        0        0    89476 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/skis/static/js/jquery-3.5.1.min.js
+-rw-r--r--   0        0        0    67496 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/skis/static/js/links.js
+-rw-r--r--   0        0        0    12288 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/skis/static/js/lists.js
+-rw-r--r--   0        0        0     8094 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/skis/static/js/logins.js
+-rw-r--r--   0        0        0    32273 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/skis/static/js/paras.js
+-rw-r--r--   0        0        0     1165 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/skis/static/js/paths.js
+-rw-r--r--   0        0        0     3986 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/skis/static/js/radio.js
+-rw-r--r--   0        0        0    31948 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/skis/static/js/skipole.js
+-rw-r--r--   0        0        0    10529 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/skis/static/js/svgbasics.js
+-rw-r--r--   0        0        0    16505 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/skis/static/js/svggraphs.js
+-rw-r--r--   0        0        0     7060 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/skis/static/js/svgmeters.js
+-rw-r--r--   0        0        0     4373 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/skis/static/js/tables.js
+-rw-r--r--   0        0        0     2287 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/skis/static/js/textarea.js
+-rw-r--r--   0        0        0     3001 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/skis/static/js/upload.js
+-rw-r--r--   0        0        0     9268 2023-03-09 17:15:52.000000 skipole-5.6.1/skipole/textblocks.py
+-rw-r--r--   0        0        0     3653 1970-01-01 00:00:00.000000 skipole-5.6.1/PKG-INFO
```

### Comparing `skipole-5.6.0/LICENSE` & `skipole-5.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/README.md` & `skipole-5.6.1/README.md`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/pyproject.toml` & `skipole-5.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "skipole"
 authors = [{name = "Bernard Czenkusz", email = "bernie@skipole.co.uk"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License","Operating System :: OS Independent","Topic :: Internet :: WWW/HTTP :: WSGI :: Application"]
-version = "5.6.0"
+version = "5.6.1"
 description="A WSGI Application generator"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords=['wsgi','application','web','framework']
 
 
 [project.urls]
```

### Comparing `skipole-5.6.0/skipole/__init__.py` & `skipole-5.6.1/skipole/__init__.py`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/__main__.py` & `skipole-5.6.1/skipole/__main__.py`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/ski/dump_project.py` & `skipole-5.6.1/skipole/ski/dump_project.py`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/ski/excepts.py` & `skipole-5.6.1/skipole/ski/excepts.py`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/ski/folder_class_definition.py` & `skipole-5.6.1/skipole/ski/folder_class_definition.py`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/ski/page_class_definition.py` & `skipole-5.6.1/skipole/ski/page_class_definition.py`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/ski/project_class_definition.py` & `skipole-5.6.1/skipole/ski/project_class_definition.py`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/ski/read_json.py` & `skipole-5.6.1/skipole/ski/read_json.py`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/ski/responders/__init__.py` & `skipole-5.6.1/skipole/ski/responders/__init__.py`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/ski/responders/checkers.py` & `skipole-5.6.1/skipole/ski/responders/checkers.py`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/ski/responders/navigators.py` & `skipole-5.6.1/skipole/ski/responders/navigators.py`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/ski/responders/submitters.py` & `skipole-5.6.1/skipole/ski/responders/submitters.py`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/ski/skiboot.py` & `skipole-5.6.1/skipole/ski/skiboot.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 
 import os, copy, collections
 
 # Configuration defaults
 
 _CFG = {
-"version"         : "5.6.0",             # The skipole version
+"version"         : "5.6.1",             # The skipole version
 "default_language": 'en',                # The default language of the project
 "debug"           : False                # The debug mode, True shows exceptions on server error
 }
 
 # As projects are created they are added to this PROJECT_REGISTER list, but as projects
 # become sub-projects by being added to a root, they are removed from this register, so
 # it becomes a list of a single item, the final root project.
```

### Comparing `skipole-5.6.0/skipole/ski/tag.py` & `skipole-5.6.1/skipole/ski/tag.py`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/ski/validators/__init__.py` & `skipole-5.6.1/skipole/ski/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/ski/validators/basic.py` & `skipole-5.6.1/skipole/ski/validators/basic.py`

 * *Files 17% similar despite different names*

```diff
@@ -125,19 +125,65 @@
         "Sets an argument value"
         Validator.__setitem__(self, arg_name, value)
         try:
             intval = int(value)
         except Exception:
             raise ValidateError(message = 'values given must be integers')
         if arg_name == 'maxval':
-            if intval < 1:
-                raise ValidateError(message = 'A maximum value of of at least 1 is expected')
-        if arg_name == 'minval':
-            if intval < 0:
-                raise ValidateError(message = 'A minimum value of least 0 is expected')
+            if 'minval' in self._val_args:
+                if intval <= self._val_args['minval']:
+                    raise ValidateError(message = 'A maximum value greater than the minimum value is expected')
+        elif arg_name == 'minval':
+            if 'maxval' in self._val_args:
+                if intval >= self._val_args['maxval']:
+                    raise ValidateError(message = 'A minimum value less than the maximum value is expected')
+        else:
+            raise ValidateError(message = 'Invalid argument')
+        self._val_args[arg_name] = intval
+
+    def _check(self, widgfield, item, environ, lang, form_data, call_data, caller_page_ident):
+        try:
+            i = int(item)
+        except Exception:
+            return '', False
+        if self["maxval"] < self["minval"]:
+            return '', False
+        if i > self["maxval"]:
+            return str(self["maxval"]), True
+        if i < self["minval"]:
+            return str(self["minval"]), True
+        return str(i), True
+
+
+
+class StrictIntMinMax(Validator):
+    """Check integer, limit value to between min and max value, raise error if input not an integer string
+       or if it is beyond the range."""
+
+    arg_descriptions = {'maxval':255,
+                        'minval':0}
+
+
+    def __setitem__(self, arg_name, value):
+        "Sets an argument value"
+        Validator.__setitem__(self, arg_name, value)
+        try:
+            intval = int(value)
+        except Exception:
+            raise ValidateError(message = 'values given must be integers')
+        if arg_name == 'maxval':
+            if 'minval' in self._val_args:
+                if intval <= self._val_args['minval']:
+                    raise ValidateError(message = 'A maximum value greater than the minimum value is expected')
+        elif arg_name == 'minval':
+            if 'maxval' in self._val_args:
+                if intval >= self._val_args['maxval']:
+                    raise ValidateError(message = 'A minimum value less than the maximum value is expected')
+        else:
+            raise ValidateError(message = 'Invalid argument')
         self._val_args[arg_name] = intval
 
     def _check(self, widgfield, item, environ, lang, form_data, call_data, caller_page_ident):
         try:
             i = int(item)
         except Exception:
             return '', False
@@ -146,14 +192,15 @@
         if i > self["maxval"]:
             return str(self["maxval"]), False
         if i < self["minval"]:
             return str(self["minval"]), False
         return str(i), True
 
 
+
 class AlphaNumUnder(Validator):
     "Checks the value is alphanumric or underscore only"
 
     arg_descriptions = {}   # Takes no arguments
 
     def _check(self, widgfield, item, environ, lang, form_data, call_data, caller_page_ident):
         "Return item, True if item is alphanumeric or underscore only"
@@ -188,9 +235,7 @@
         self._val_args[arg_name] = value
 
     def _check(self, widgfield, item, environ, lang, form_data, call_data, caller_page_ident):
         "Return item, True if pattern search successfull"
         if re.search(self._val_args['pattern'],item) is None:
             return '', False
         return item, True
-
-
```

### Comparing `skipole-5.6.0/skipole/ski/validators/paths.py` & `skipole-5.6.1/skipole/ski/validators/paths.py`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/ski/widgets/__init__.py` & `skipole-5.6.1/skipole/ski/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/ski/widgets/checkbox.py` & `skipole-5.6.1/skipole/ski/widgets/checkbox.py`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/ski/widgets/confirm.py` & `skipole-5.6.1/skipole/ski/widgets/confirm.py`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/ski/widgets/debug_tools.py` & `skipole-5.6.1/skipole/ski/widgets/debug_tools.py`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/ski/widgets/dropdown.py` & `skipole-5.6.1/skipole/ski/widgets/dropdown.py`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/ski/widgets/error_messages.py` & `skipole-5.6.1/skipole/ski/widgets/error_messages.py`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/ski/widgets/footers.py` & `skipole-5.6.1/skipole/ski/widgets/footers.py`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/ski/widgets/headers.py` & `skipole-5.6.1/skipole/ski/widgets/headers.py`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/ski/widgets/info.py` & `skipole-5.6.1/skipole/ski/widgets/info.py`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/ski/widgets/inputforms.py` & `skipole-5.6.1/skipole/ski/widgets/inputforms.py`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/ski/widgets/inputtables.py` & `skipole-5.6.1/skipole/ski/widgets/inputtables.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,34 +171,34 @@
   </tr>
   <!-- rows repeated -->
  </tbody>
 </table>"""
 
 
 
-
-
 class InputTable5(Widget):
-    """Defines a div of four columns, the first just being label text, the second being text input fields,
-       the third and fourth being submit buttons.  Each row of the table is a form, the
-       form action ident is the same for all forms.
-       On error the paragraph TextBlock is changed to the error message."""
+    """A div of four columns, the first just being label text, the second being text input fields,
+    the third and fourth being submit buttons. Each row of the table is a form, the form action ident
+    is the same for all forms and each form has four hidden fields.
+    As well as the input text field each form submits button and value, so which of the two
+    buttons is pressed can be identified."""
 
     # This class does not display any error messages
     display_errors = False
 
     # js_validators is a class attribute, True if javascript validation is enabled
     js_validators=True
 
     arg_descriptions = {
                         'div_class':FieldArg("cssclass", ''),
                         'size':FieldArg("text", ''),
                         'maxlength':FieldArg("text", ''),
                         'required':FieldArg("boolean", False),
-                        'action':FieldArg("url",''),
+                        'action_json':FieldArg("url", ''),
+                        'action':FieldArg("url",'no_javascript'),
                         'button_text1':FieldArg("text", "Submit", valdt=True),
                         'button_text2':FieldArg("text", "Submit", valdt=True),
                         'button1_class':FieldArg("cssclass", ""),
                         'button2_class':FieldArg("cssclass", ""),
                         'col_label':FieldArgList('text'),
                         'label_class':FieldArg("cssclass", ""),
                         'label_style':FieldArg("cssstyle", ""),
@@ -217,15 +217,16 @@
 
     def __init__(self, name=None, brief='', **field_args):
         """
         div_class: the class attribute of each form div
         size: The number of characters appearing in each text input area
         maxlength: The maximum number of characters accepted in each text area
         required: Set True to put the 'required' flag into each input field
-        action: The label or ident of the action page
+        action_json:  if a value set, and client has jscript enabled, this is the page ident, label, url the form calls, expects a json page back.
+        action: The page ident, label, url the form calls, if action_json not set. Expects an html page back.
         button_text1: text appearing on the first buttons - if empty, no button 1 is shown
         button_text2: text appearing on the second buttons - if empty, no button 2 is shown
         button1_class: class set on button1
         button2_class: class set on button2
         col_label: a list of all the text strings appearing in the first column
         label_class: the class to apply to each label
         col_input: a list of all the text strings appearing in the input fields
@@ -257,14 +258,17 @@
 
         # any label:value added to self.jlabels will be set in a javascript fieldvalues attribute for the widget
         if self.wf.input_accepted_class:
             self.jlabels['input_accepted_class'] = self.wf.input_accepted_class
         if self.wf.input_errored_class:
             self.jlabels['input_errored_class'] = self.wf.input_errored_class
 
+        jsonurl = self.get_url(self.wf.action_json)
+        if jsonurl:
+            self.jlabels['url'] = jsonurl
 
         len_label = len(self.wf.col_label)
         len_input = len(self.wf.col_input)
         len_hidden_field1 = len(self.wf.hidden_field1)
         len_hidden_field2 = len(self.wf.hidden_field2)
         len_hidden_field3 = len(self.wf.hidden_field3)
         len_hidden_field4 = len(self.wf.hidden_field4)
@@ -299,16 +303,14 @@
             set_input_errored = self.wf.set_input_errored
         else:
             set_input_errored = {}
 
         input_class = self.wf.input_class
         input_style = self.wf.input_style
 
-
-
         for rownumber in range(rows):
             if rownumber<len_label:
                 col_label = self.wf.col_label[rownumber]
             else:
                 col_label = ''
             if rownumber<len_input:
                 col_input = self.wf.col_input[rownumber]
@@ -370,26 +372,31 @@
                     formrow[1].attribs["class"] = self.wf.input_accepted_class
             elif input_class:
                 formrow[1].attribs["class"] = input_class
 
             if input_style:
                 formrow[1].attribs["style"] = input_style
 
+            # the submit buttons have an onclick function to set their name and value
+            # into the widget javascript object
+
             # 3rd column is a submit button
             if button_value1:
                 formrow.append(tag.ClosedPart(tag_name="input",
                                  attribs ={"name":button_name1,
                                            "value":button_value1,
+                                           "onclick":f"SKIPOLE.widgets['{self.get_id()}'].setbutton(this.name, this.value);",
                                            "class":button1_class,
                                            "type":"submit"}))
             # 4th column is a submit button
             if button_value2:
                 formrow.append(tag.ClosedPart(tag_name="input",
                                  attribs ={"name":button_name2,
                                            "value":button_value2,
+                                           "onclick":f"SKIPOLE.widgets['{self.get_id()}'].setbutton(this.name, this.value);",
                                            "class":button2_class,
                                            "type":"submit"}))
 
             # all submissions always have an 'ident' hidden field to provide the ident of the calling page
             formrow.append(tag.ClosedPart(tag_name="input",
                                           attribs ={"name":'ident',
                                                  "value":ident_value,
```

### Comparing `skipole-5.6.0/skipole/ski/widgets/inputtext.py` & `skipole-5.6.1/skipole/ski/widgets/inputtext.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         if self.wf.type:
             self.attribs["type"] = self.wf.type
         if self.wf.pattern:
             self.attribs["pattern"] = self.wf.pattern
         if self.wf.title:
             self.attribs["title"] = self.wf.title
 
- 
+
     @classmethod
     def description(cls):
         """Returns a text string to illustrate the widget"""
         return """
   <input type='text' />
   <!-- with widget id and class widget_class and input_accepted_class added if
        set_input_accepted is set to True, and input_errored_class added if
@@ -160,15 +160,15 @@
         if self.wf.maxlength:
             self.attribs["maxlength"] = self.wf.maxlength
         if self.wf.disabled:
             self.attribs["disabled"] = "disabled"
         if self.wf.required:
             self.attribs["required"] = "required"
 
- 
+
     @classmethod
     def description(cls):
         """Returns a text string to illustrate the widget"""
         return """
   <input type='password' />
   <!-- with widget id and class widget_class and input_accepted_class added if
        set_input_accepted is set to True, and input_errored_class added if
@@ -603,15 +603,15 @@
         self[0].attribs['for'] = self.jlabels['input_id']
         self[2].attribs['for'] = self.jlabels['input_id']
 
         if self.wf.input_accepted_class:
             self.jlabels['input_accepted_class'] = self.wf.input_accepted_class
         if self.wf.input_errored_class:
             self.jlabels['input_errored_class'] = self.wf.input_errored_class
- 
+
     @classmethod
     def description(cls):
         """Returns a text string to illustrate the widget"""
         return """
 <div>  <!-- with widget id and class widget_class -->
   <label> <!-- with class set to left_class and content to left_label -->
   </label>
@@ -627,15 +627,15 @@
        All divs, label and input field can have class set
        No error display"""
 
     # This class does not display any error messages
     display_errors = False
 
     # js_validators is a class attribute, True if javascript validation is enabled
-    js_validators=True   
+    js_validators=True
 
     arg_descriptions = {
                         'input_accepted_class':FieldArg("cssclass", ''),
                         'input_errored_class':FieldArg("cssclass", ''),
                         'set_input_accepted':FieldArg("boolean", False, jsonset=True),
                         'set_input_errored':FieldArg("boolean", False, jsonset=True),
                         'labeldiv_class':FieldArg("cssclass", ''),
@@ -994,15 +994,15 @@
           <input type="text" />  <!-- class set to input_class -->
             <!-- input text value set to input_text -->
           <button type="submit"> <!-- with class set to button_class -->
             <!-- button_text -->
           </button>
       </span>
     </div>
-    <!-- hidden input fields -->                              
+    <!-- hidden input fields -->
   </form>
 </div>"""
 
 
 
 class SubmitTextInput3(Widget):
     """Defines paragraphs followed by a form with a text input field"""
@@ -1279,15 +1279,15 @@
     </div>
     <div> <!-- class attribute set to buttondiv_class -->
       <label> <!-- with class set to button_label_class and content to button_label -->
       </label>
       <input type=\"submit\" /> <!-- button value set to button_text and class to button_class -->
     </div>
     <!-- hidden input fields -->
-  </form>    
+  </form>
 </div>"""
 
 
 class TwoInputsSubmit1(Widget):
     """Defines a form containing two text input fields."""
 
     error_location = (0,0,0)
@@ -1553,29 +1553,32 @@
     <div> <!-- class attribute set to inputdiv_class -->
       <label> <!-- with class set to label_class and content to label -->
       </label>
       <input type=\"text\" /> <!-- input text value set to input_text1, class to input_class1 -->
       <input type=\"text\" /> <!-- input text value set to input_text2, class to input_class2 -->
       <input type=\"submit\" /> <!-- button value set to button_text and class to button_class -->
     </div>
-    <!-- hidden input fields -->    
+    <!-- hidden input fields -->
   </form>
 </div>"""
 
 
 class SubmitDict1(Widget):
     """Defines a form with a list of input fields followed by a single submit button
        to allow a client to input a dictionary"""
 
     display_errors = False
 
+    # js_validators is a class attribute, True if javascript validation is enabled
+    js_validators=True
+
     arg_descriptions = {'action':FieldArg("url", ''),
                         'button_text':FieldArg("text", "Submit"),
                         'button_class':FieldArg("cssclass", ''),
-                        'input_dict':FieldArgDict('text', valdt=False, senddict=True),
+                        'input_dict':FieldArgDict('text', valdt=True, senddict=True),
                         'input_class':FieldArg("cssclass", ''),
                         'inputdiv_class':FieldArg("cssclass", ''),
                         'inputdiv_style':FieldArg("cssstyle", ''),
                         'ul_class':FieldArg("cssclass", ""),
                         'ul_style':FieldArg("cssstyle", ""),
                         'li_class':FieldArg("cssclass", ""),
                         'li_style':FieldArg("cssstyle", ""),
@@ -1674,14 +1677,22 @@
             self[0][1][0].attribs = {"value":self.wf.button_text, "type":"submit", "class":self.wf.button_class}
         else:
             self[0][1][0].attribs = {"value":self.wf.button_text, "type":"submit"}
 
         # add ident and four hidden fields
         self.add_hiddens(self[0], page)
 
+    def _build_js(self, page, ident_list, environ, call_data, lang):
+        """Sets a submit event handler for javascript validation"""
+        ident=self.get_id()
+        return f"""  $("#{ident} form").on("submit input", function(e) {{
+    SKIPOLE.widgets["{ident}"].eventfunc(e);
+    }});
+"""
+
 
     @classmethod
     def description(cls):
         """Returns a text string to illustrate the widget"""
         return """
 <div> <!-- with widget id and class widget_class -->
   <form method=\"post\"> <!-- action attribute set to action field -->
@@ -1926,15 +1937,15 @@
           <input type="text" />  <!-- class set to input_class -->
             <!-- input text value set to input_text -->
           <button type="submit"> <!-- with class set to button_class -->
             <!-- button_text -->
           </button>
       </span>
     </div>
-    <!-- hidden input fields -->                              
+    <!-- hidden input fields -->
   </form>
 </div>"""
 
 
 
 class SubmitTextInput4(Widget):
     """Defines a form with a text input field, and four hidden fields"""
@@ -2178,13 +2189,10 @@
       </div>
       <div>  <!-- class attribute set to buttondiv_class -->
           <button type="submit"> <!-- with class set to button_class -->
             <!-- button_text -->
           </button>
       </div>
     </div>
-    <!-- hidden input fields -->                              
+    <!-- hidden input fields -->
   </form>
 </div>"""
-
-
-
```

### Comparing `skipole-5.6.0/skipole/ski/widgets/links.py` & `skipole-5.6.1/skipole/ski/widgets/links.py`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/ski/widgets/lists.py` & `skipole-5.6.1/skipole/ski/widgets/lists.py`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/ski/widgets/logins.py` & `skipole-5.6.1/skipole/ski/widgets/logins.py`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/ski/widgets/paras.py` & `skipole-5.6.1/skipole/ski/widgets/paras.py`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/ski/widgets/radio.py` & `skipole-5.6.1/skipole/ski/widgets/radio.py`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/ski/widgets/svgbasics.py` & `skipole-5.6.1/skipole/ski/widgets/svgbasics.py`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/ski/widgets/svggraphs.py` & `skipole-5.6.1/skipole/ski/widgets/svggraphs.py`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/ski/widgets/svgmeters.py` & `skipole-5.6.1/skipole/ski/widgets/svgmeters.py`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/ski/widgets/tables.py` & `skipole-5.6.1/skipole/ski/widgets/tables.py`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/ski/widgets/textarea.py` & `skipole-5.6.1/skipole/ski/widgets/textarea.py`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/ski/widgets/upload.py` & `skipole-5.6.1/skipole/ski/widgets/upload.py`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/skis.py` & `skipole-5.6.1/skipole/skis.py`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/skis/data/project.json` & `skipole-5.6.1/skipole/skis/data/project.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.875%*

 * *Differences: {"'skipole'": "'5.6.1'", "'version'": "'5.6.1'"}*

```diff
@@ -2115,15 +2115,15 @@
             }
         },
         "restricted": false
     },
     "brief": "Library project of static files",
     "default_language": "en",
     "sections": {},
-    "skipole": "5.6.0",
+    "skipole": "5.6.1",
     "specialpages": {
         "general_json": 870,
         "jquery_core": 20,
         "no_javascript": 840,
         "redirector": 830,
         "server_error": 820,
         "ski_basic": 101,
@@ -2157,9 +2157,9 @@
         "theme3_css": 350,
         "theme4_css": 360,
         "url_not_found": 880,
         "validate_error": 810,
         "w3_css": 320
     },
     "url": "/",
-    "version": "5.6.0"
+    "version": "5.6.1"
 }
```

### Comparing `skipole-5.6.0/skipole/skis/data/textblocks_json/en.json` & `skipole-5.6.1/skipole/skis/data/textblocks_json/en.json`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/skis/static/css/theme1.css` & `skipole-5.6.1/skipole/skis/static/css/theme1.css`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/skis/static/css/theme2.css` & `skipole-5.6.1/skipole/skis/static/css/theme2.css`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/skis/static/css/theme3.css` & `skipole-5.6.1/skipole/skis/static/css/theme3.css`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/skis/static/css/theme4.css` & `skipole-5.6.1/skipole/skis/static/css/theme4.css`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/skis/static/css/w3.css` & `skipole-5.6.1/skipole/skis/static/css/w3.css`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/skis/static/js/basic.js` & `skipole-5.6.1/skipole/skis/static/js/basic.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -70,20 +70,32 @@
             return true;
         }
         if (item) {
             return true;
         }
         return false;
     },
-    /* ok if item is an integer string and between or equal to minval - maxval*/
+    /* ok if item is an integer string, leave range test to server*/
     'IntMinMax': function(item, allowed_values, args) {
         if (SKIPOLE.inallowedlist(item, allowed_values)) {
             return true;
         }
-        let reg = /^0-9/;
+        let reg = /[^0-9-]/;
+        if (reg.test(item)) {
+            return false;
+        }
+        /* item is an integer string */
+        return true;
+    },
+    /* ok if item is an integer string and between or equal to minval - maxval*/
+    'StrictIntMinMax': function(item, allowed_values, args) {
+        if (SKIPOLE.inallowedlist(item, allowed_values)) {
+            return true;
+        }
+        let reg = /[^0-9-]/;
         if (reg.test(item)) {
             return false;
         }
         /* item is an integer string */
         let value = parseInt(item, 10);
         if (value < args.minval) {
             return false;
```

### Comparing `skipole-5.6.0/skipole/skis/static/js/checkbox.js` & `skipole-5.6.1/skipole/skis/static/js/checkbox.js`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/skis/static/js/confirm.js` & `skipole-5.6.1/skipole/skis/static/js/confirm.js`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/skis/static/js/debug_tools.js` & `skipole-5.6.1/skipole/skis/static/js/debug_tools.js`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/skis/static/js/dropdown.js` & `skipole-5.6.1/skipole/skis/static/js/dropdown.js`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/skis/static/js/error_messages.js` & `skipole-5.6.1/skipole/skis/static/js/error_messages.js`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/skis/static/js/footers.js` & `skipole-5.6.1/skipole/skis/static/js/footers.js`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/skis/static/js/headers.js` & `skipole-5.6.1/skipole/skis/static/js/headers.js`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/skis/static/js/info.js` & `skipole-5.6.1/skipole/skis/static/js/info.js`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/skis/static/js/inputforms.js` & `skipole-5.6.1/skipole/skis/static/js/inputforms.js`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/skis/static/js/inputtables.js` & `skipole-5.6.1/skipole/skis/static/js/inputtables.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -92,22 +92,14 @@
 
 SKIPOLE.inputtables.InputTable5 = function(widg_id, error_message, fieldmap) {
     SKIPOLE.BaseWidget.call(this, widg_id, error_message, fieldmap);
     this.display_errors = false;
 };
 SKIPOLE.inputtables.InputTable5.prototype = Object.create(SKIPOLE.BaseWidget.prototype);
 SKIPOLE.inputtables.InputTable5.prototype.constructor = SKIPOLE.inputtables.InputTable5;
-SKIPOLE.inputtables.InputTable5.prototype.eventfunc = function(e) {
-    SKIPOLE.skiprefresh = true;
-    let selected_form = $(e.target);
-    if (!SKIPOLE.form_validate(selected_form)) {
-        // prevent the submission if validation failure
-        e.preventDefault();
-    }
-};
 SKIPOLE.inputtables.InputTable5.prototype.setvalues = function(fieldlist, result) {
     if (!this.widg_id) {
         return;
     }
     let the_widg = this.widg;
     // input_accepted and input_errored
     let input_accepted = this.fieldarg_in_result('set_input_accepted', result, fieldlist);
@@ -132,14 +124,79 @@
             if (input_key in input_errored) {
                 self.set_errored(text_input, input_errored[input_key]);
             }
         }
     })
 };
 
+SKIPOLE.inputtables.InputTable5.prototype.setbutton = function(name, value) {
+    // Called by button onclick, to save the name,value of the button
+    // used to submit the form
+    this.button_name = name;
+    this.button_value = value;
+};
+
+SKIPOLE.inputtables.InputTable5.prototype.eventfunc = function(e) {
+    SKIPOLE.skiprefresh = true;
+    let selected_form = $(e.target);
+    if (!SKIPOLE.form_validate(selected_form)) {
+        // prevent the submission if validation failure
+        e.preventDefault();
+    } else {
+        // form validated, if action_json url set, call a json page
+        let jsonurl = this.fieldvalues["url"];
+        if (jsonurl) {
+            // json url set, send data with a request for json and prevent default
+            let self = this
+            let senddata = selected_form.serializeArray();
+            // get the submit button name, value which submitted this form
+            // this is necessary since serializeArray() does not pick up the button name
+            // and value from the form, so an onclick event saves them using setbutton()
+            // and the name,value is pushed on to senddata
+            senddata.push({
+                name: this.button_name,
+                value: this.button_value
+            });
+            e.preventDefault();
+            // respond to json or html
+            $.ajax({
+                    url: jsonurl,
+                    data: senddata
+                })
+                .done(function(result, textStatus, jqXHR) {
+                    if (jqXHR.responseJSON) {
+                        // JSON response
+                        if (self.get_error(result)) {
+                            // if error, set any results received from the json call
+                            SKIPOLE.setfields(result);
+                        } else {
+                            // If no error received, clear any previous error
+                            self.clear_error();
+                            SKIPOLE.setfields(result);
+                        }
+                    } else {
+                        // html response
+                        document.open();
+                        document.write(result);
+                        document.close();
+                    }
+                })
+                .fail(function(jqXHR, textStatus, errorThrown) {
+                    if (jqXHR.status == 400 || jqXHR.status == 404 || jqXHR.status == 500) {
+                        document.open();
+                        document.write(jqXHR.responseText);
+                        document.close();
+                    } else {
+                        SKIPOLE.json_failed(jqXHR, textStatus, errorThrown);
+                    }
+                });
+        }
+    }
+};
+
 
 
 SKIPOLE.inputtables.InputTable4 = function(widg_id, error_message, fieldmap) {
     SKIPOLE.BaseWidget.call(this, widg_id, error_message, fieldmap);
     this.display_errors = false;
 };
 SKIPOLE.inputtables.InputTable4.prototype = Object.create(SKIPOLE.BaseWidget.prototype);
```

### Comparing `skipole-5.6.0/skipole/skis/static/js/inputtext.js` & `skipole-5.6.1/skipole/skis/static/js/inputtext.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -515,14 +515,24 @@
 SKIPOLE.inputtext.SubmitDict1.prototype.setvalues = function(fieldlist, result) {
     if (!this.widg_id) {
         return;
     }
     // sets hidden fields
     this.sethiddenfields(fieldlist, result);
 };
+SKIPOLE.inputtext.SubmitDict1.prototype.eventfunc = function(e) {
+    SKIPOLE.skiprefresh = true;
+    if (e.type == 'submit') {
+        // form submitted
+        if (!SKIPOLE.form_validate(this.widg)) {
+            // prevent the submission if validation failure
+            e.preventDefault();
+        }
+    }
+};
 
 
 
 SKIPOLE.inputtext.SubmitTextInput2 = function(widg_id, error_message, fieldmap) {
     SKIPOLE.BaseWidget.call(this, widg_id, error_message, fieldmap);
 };
 SKIPOLE.inputtext.SubmitTextInput2.prototype = Object.create(SKIPOLE.BaseWidget.prototype);
@@ -616,15 +626,15 @@
                 }
 
             }
         }
 
         // Display the key/value pairs in senddata
         // for (var pair of senddata.entries()) {
-        //    console.log(pair[0]+ ', ' + pair[1]); 
+        //    console.log(pair[0]+ ', ' + pair[1]);
         // }
 
 
         // respond to json or html
         $.ajax({
                 url: url,
                 data: senddata,
```

### Comparing `skipole-5.6.0/skipole/skis/static/js/jquery-3.5.1.min.js` & `skipole-5.6.1/skipole/skis/static/js/jquery-3.5.1.min.js`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/skis/static/js/links.js` & `skipole-5.6.1/skipole/skis/static/js/links.js`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/skis/static/js/lists.js` & `skipole-5.6.1/skipole/skis/static/js/lists.js`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/skis/static/js/logins.js` & `skipole-5.6.1/skipole/skis/static/js/logins.js`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/skis/static/js/paras.js` & `skipole-5.6.1/skipole/skis/static/js/paras.js`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/skis/static/js/paths.js` & `skipole-5.6.1/skipole/skis/static/js/paths.js`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/skis/static/js/radio.js` & `skipole-5.6.1/skipole/skis/static/js/radio.js`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/skis/static/js/skipole.js` & `skipole-5.6.1/skipole/skis/static/js/skipole.js`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/skis/static/js/svgbasics.js` & `skipole-5.6.1/skipole/skis/static/js/svgbasics.js`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/skis/static/js/svggraphs.js` & `skipole-5.6.1/skipole/skis/static/js/svggraphs.js`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/skis/static/js/svgmeters.js` & `skipole-5.6.1/skipole/skis/static/js/svgmeters.js`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/skis/static/js/tables.js` & `skipole-5.6.1/skipole/skis/static/js/tables.js`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/skis/static/js/textarea.js` & `skipole-5.6.1/skipole/skis/static/js/textarea.js`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/skis/static/js/upload.js` & `skipole-5.6.1/skipole/skis/static/js/upload.js`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/skipole/textblocks.py` & `skipole-5.6.1/skipole/textblocks.py`

 * *Files identical despite different names*

### Comparing `skipole-5.6.0/PKG-INFO` & `skipole-5.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skipole
-Version: 5.6.0
+Version: 5.6.1
 Summary: A WSGI Application generator
 Keywords: wsgi,application,web,framework
 Author-email: Bernard Czenkusz <bernie@skipole.co.uk>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

