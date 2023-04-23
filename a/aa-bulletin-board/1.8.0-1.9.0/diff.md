# Comparing `tmp/aa_bulletin_board-1.8.0.tar.gz` & `tmp/aa_bulletin_board-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa_bulletin_board-1.8.0.tar", last modified: Thu Apr 13 14:00:02 2023, max compression
+gzip compressed data, was "aa_bulletin_board-1.9.0.tar", last modified: Sun Apr 16 15:46:27 2023, max compression
```

## Comparing `aa_bulletin_board-1.8.0.tar` & `aa_bulletin_board-1.9.0.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.041726 aa_bulletin_board-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14077 2023-04-13 14:00:02.041726 aa_bulletin_board-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12778 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.037726 aa_bulletin_board-1.8.0/aa_bulletin_board/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/auth_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.033726 aa_bulletin_board-1.8.0/aa_bulletin_board/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.033726 aa_bulletin_board-1.8.0/aa_bulletin_board/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.037726 aa_bulletin_board-1.8.0/aa_bulletin_board/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.033726 aa_bulletin_board-1.8.0/aa_bulletin_board/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.037726 aa_bulletin_board-1.8.0/aa_bulletin_board/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.033726 aa_bulletin_board-1.8.0/aa_bulletin_board/locale/fr_FR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.037726 aa_bulletin_board-1.8.0/aa_bulletin_board/locale/fr_FR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/locale/fr_FR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.033726 aa_bulletin_board-1.8.0/aa_bulletin_board/locale/it_IT/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.037726 aa_bulletin_board-1.8.0/aa_bulletin_board/locale/it_IT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/locale/it_IT/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.033726 aa_bulletin_board-1.8.0/aa_bulletin_board/locale/ja/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.037726 aa_bulletin_board-1.8.0/aa_bulletin_board/locale/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.033726 aa_bulletin_board-1.8.0/aa_bulletin_board/locale/ko_KR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.037726 aa_bulletin_board-1.8.0/aa_bulletin_board/locale/ko_KR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/locale/ko_KR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.033726 aa_bulletin_board-1.8.0/aa_bulletin_board/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.037726 aa_bulletin_board-1.8.0/aa_bulletin_board/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.033726 aa_bulletin_board-1.8.0/aa_bulletin_board/locale/zh_Hans/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.037726 aa_bulletin_board-1.8.0/aa_bulletin_board/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/managers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.037726 aa_bulletin_board-1.8.0/aa_bulletin_board/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/migrations/0002_alter_bulletin_slug.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/migrations/0003_group_restrictions.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.033726 aa_bulletin_board-1.8.0/aa_bulletin_board/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.033726 aa_bulletin_board-1.8.0/aa_bulletin_board/static/aa_bulletin_board/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.041726 aa_bulletin_board-1.8.0/aa_bulletin_board/static/aa_bulletin_board/css/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/static/aa_bulletin_board/css/aa-bootstrap-fix.css
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/static/aa_bulletin_board/css/aa-bootstrap-fix.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/static/aa_bulletin_board/css/aa-bulletin-board.css
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/static/aa_bulletin_board/css/aa-bulletin-board.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.033726 aa_bulletin_board-1.8.0/aa_bulletin_board/static/aa_bulletin_board/libs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.033726 aa_bulletin_board-1.8.0/aa_bulletin_board/static/aa_bulletin_board/libs/sumoselect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.041726 aa_bulletin_board-1.8.0/aa_bulletin_board/static/aa_bulletin_board/libs/sumoselect/3.4.8/
--rw-r--r--   0 runner    (1001) docker     (123)    34280 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/static/aa_bulletin_board/libs/sumoselect/3.4.8/jquery.sumoselect.js
--rw-r--r--   0 runner    (1001) docker     (123)    22226 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/static/aa_bulletin_board/libs/sumoselect/3.4.8/jquery.sumoselect.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     7610 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/static/aa_bulletin_board/libs/sumoselect/3.4.8/sumoselect.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.033726 aa_bulletin_board-1.8.0/aa_bulletin_board/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.041726 aa_bulletin_board-1.8.0/aa_bulletin_board/templates/aa_bulletin_board/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/templates/aa_bulletin_board/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/templates/aa_bulletin_board/bulletin.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.041726 aa_bulletin_board-1.8.0/aa_bulletin_board/templates/aa_bulletin_board/bundles/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/templates/aa_bulletin_board/bundles/aa-bulletin-board-css.html
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/templates/aa_bulletin_board/bundles/sumoselect-css.html
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/templates/aa_bulletin_board/bundles/sumoselect-js.html
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/templates/aa_bulletin_board/dashboard.html
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.033726 aa_bulletin_board-1.8.0/aa_bulletin_board/templates/aa_bulletin_board/partials/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.041726 aa_bulletin_board-1.8.0/aa_bulletin_board/templates/aa_bulletin_board/partials/header/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/templates/aa_bulletin_board/partials/header/page-header.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.041726 aa_bulletin_board-1.8.0/aa_bulletin_board/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/templatetags/aa_bulletin_board_versioned_static.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.041726 aa_bulletin_board-1.8.0/aa_bulletin_board/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/tests/test_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/tests/test_auth_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/tests/test_bulletins.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/tests/test_templatetags.py
--rw-r--r--   0 runner    (1001) docker     (123)     7486 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/tests/test_user_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.037726 aa_bulletin_board-1.8.0/aa_bulletin_board.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14077 2023-04-13 14:00:02.000000 aa_bulletin_board-1.8.0/aa_bulletin_board.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-13 14:00:02.000000 aa_bulletin_board-1.8.0/aa_bulletin_board.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 14:00:02.000000 aa_bulletin_board-1.8.0/aa_bulletin_board.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 14:00:01.000000 aa_bulletin_board-1.8.0/aa_bulletin_board.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-13 14:00:02.000000 aa_bulletin_board-1.8.0/aa_bulletin_board.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-13 14:00:02.000000 aa_bulletin_board-1.8.0/aa_bulletin_board.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-04-13 14:00:02.041726 aa_bulletin_board-1.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:46:27.789470 aa_bulletin_board-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-16 15:46:04.000000 aa_bulletin_board-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-16 15:46:04.000000 aa_bulletin_board-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14348 2023-04-16 15:46:27.789470 aa_bulletin_board-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13049 2023-04-16 15:46:04.000000 aa_bulletin_board-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:46:27.777470 aa_bulletin_board-1.9.0/aa_bulletin_board/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-16 15:46:04.000000 aa_bulletin_board-1.9.0/aa_bulletin_board/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-16 15:46:04.000000 aa_bulletin_board-1.9.0/aa_bulletin_board/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-16 15:46:04.000000 aa_bulletin_board-1.9.0/aa_bulletin_board/auth_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-04-16 15:46:04.000000 aa_bulletin_board-1.9.0/aa_bulletin_board/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-16 15:46:04.000000 aa_bulletin_board-1.9.0/aa_bulletin_board/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:46:27.773470 aa_bulletin_board-1.9.0/aa_bulletin_board/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:46:27.773470 aa_bulletin_board-1.9.0/aa_bulletin_board/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:46:27.781470 aa_bulletin_board-1.9.0/aa_bulletin_board/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-16 15:46:04.000000 aa_bulletin_board-1.9.0/aa_bulletin_board/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-04-16 15:46:04.000000 aa_bulletin_board-1.9.0/aa_bulletin_board/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:46:27.773470 aa_bulletin_board-1.9.0/aa_bulletin_board/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:46:27.781470 aa_bulletin_board-1.9.0/aa_bulletin_board/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-04-16 15:46:04.000000 aa_bulletin_board-1.9.0/aa_bulletin_board/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:46:27.773470 aa_bulletin_board-1.9.0/aa_bulletin_board/locale/fr_FR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:46:27.781470 aa_bulletin_board-1.9.0/aa_bulletin_board/locale/fr_FR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-16 15:46:04.000000 aa_bulletin_board-1.9.0/aa_bulletin_board/locale/fr_FR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:46:27.773470 aa_bulletin_board-1.9.0/aa_bulletin_board/locale/it_IT/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:46:27.781470 aa_bulletin_board-1.9.0/aa_bulletin_board/locale/it_IT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-16 15:46:04.000000 aa_bulletin_board-1.9.0/aa_bulletin_board/locale/it_IT/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:46:27.773470 aa_bulletin_board-1.9.0/aa_bulletin_board/locale/ja/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:46:27.781470 aa_bulletin_board-1.9.0/aa_bulletin_board/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-04-16 15:46:04.000000 aa_bulletin_board-1.9.0/aa_bulletin_board/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:46:27.773470 aa_bulletin_board-1.9.0/aa_bulletin_board/locale/ko_KR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:46:27.781470 aa_bulletin_board-1.9.0/aa_bulletin_board/locale/ko_KR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-16 15:46:04.000000 aa_bulletin_board-1.9.0/aa_bulletin_board/locale/ko_KR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:46:27.773470 aa_bulletin_board-1.9.0/aa_bulletin_board/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:46:27.781470 aa_bulletin_board-1.9.0/aa_bulletin_board/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-04-16 15:46:04.000000 aa_bulletin_board-1.9.0/aa_bulletin_board/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-04-16 15:46:04.000000 aa_bulletin_board-1.9.0/aa_bulletin_board/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:46:27.773470 aa_bulletin_board-1.9.0/aa_bulletin_board/locale/zh_Hans/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:46:27.781470 aa_bulletin_board-1.9.0/aa_bulletin_board/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-04-16 15:46:04.000000 aa_bulletin_board-1.9.0/aa_bulletin_board/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-16 15:46:04.000000 aa_bulletin_board-1.9.0/aa_bulletin_board/managers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:46:27.781470 aa_bulletin_board-1.9.0/aa_bulletin_board/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-04-16 15:46:04.000000 aa_bulletin_board-1.9.0/aa_bulletin_board/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-16 15:46:04.000000 aa_bulletin_board-1.9.0/aa_bulletin_board/migrations/0002_alter_bulletin_slug.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-16 15:46:04.000000 aa_bulletin_board-1.9.0/aa_bulletin_board/migrations/0003_group_restrictions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 15:46:04.000000 aa_bulletin_board-1.9.0/aa_bulletin_board/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-04-16 15:46:04.000000 aa_bulletin_board-1.9.0/aa_bulletin_board/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:46:27.773470 aa_bulletin_board-1.9.0/aa_bulletin_board/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:46:27.773470 aa_bulletin_board-1.9.0/aa_bulletin_board/static/aa_bulletin_board/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:46:27.785470 aa_bulletin_board-1.9.0/aa_bulletin_board/static/aa_bulletin_board/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-16 15:46:04.000000 aa_bulletin_board-1.9.0/aa_bulletin_board/static/aa_bulletin_board/css/aa-bootstrap-fix.css
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-16 15:46:04.000000 aa_bulletin_board-1.9.0/aa_bulletin_board/static/aa_bulletin_board/css/aa-bootstrap-fix.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-04-16 15:46:04.000000 aa_bulletin_board-1.9.0/aa_bulletin_board/static/aa_bulletin_board/css/aa-bulletin-board.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-16 15:46:04.000000 aa_bulletin_board-1.9.0/aa_bulletin_board/static/aa_bulletin_board/css/aa-bulletin-board.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:46:27.773470 aa_bulletin_board-1.9.0/aa_bulletin_board/static/aa_bulletin_board/libs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:46:27.773470 aa_bulletin_board-1.9.0/aa_bulletin_board/static/aa_bulletin_board/libs/sumoselect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:46:27.785470 aa_bulletin_board-1.9.0/aa_bulletin_board/static/aa_bulletin_board/libs/sumoselect/3.4.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    34280 2023-04-16 15:46:04.000000 aa_bulletin_board-1.9.0/aa_bulletin_board/static/aa_bulletin_board/libs/sumoselect/3.4.8/jquery.sumoselect.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22226 2023-04-16 15:46:04.000000 aa_bulletin_board-1.9.0/aa_bulletin_board/static/aa_bulletin_board/libs/sumoselect/3.4.8/jquery.sumoselect.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7610 2023-04-16 15:46:04.000000 aa_bulletin_board-1.9.0/aa_bulletin_board/static/aa_bulletin_board/libs/sumoselect/3.4.8/sumoselect.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:46:27.773470 aa_bulletin_board-1.9.0/aa_bulletin_board/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:46:27.785470 aa_bulletin_board-1.9.0/aa_bulletin_board/templates/aa_bulletin_board/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-16 15:46:04.000000 aa_bulletin_board-1.9.0/aa_bulletin_board/templates/aa_bulletin_board/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-04-16 15:46:04.000000 aa_bulletin_board-1.9.0/aa_bulletin_board/templates/aa_bulletin_board/bulletin.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:46:27.785470 aa_bulletin_board-1.9.0/aa_bulletin_board/templates/aa_bulletin_board/bundles/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-16 15:46:04.000000 aa_bulletin_board-1.9.0/aa_bulletin_board/templates/aa_bulletin_board/bundles/aa-bulletin-board-css.html
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-16 15:46:04.000000 aa_bulletin_board-1.9.0/aa_bulletin_board/templates/aa_bulletin_board/bundles/sumoselect-css.html
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-16 15:46:04.000000 aa_bulletin_board-1.9.0/aa_bulletin_board/templates/aa_bulletin_board/bundles/sumoselect-js.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-04-16 15:46:04.000000 aa_bulletin_board-1.9.0/aa_bulletin_board/templates/aa_bulletin_board/dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-04-16 15:46:04.000000 aa_bulletin_board-1.9.0/aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:46:27.773470 aa_bulletin_board-1.9.0/aa_bulletin_board/templates/aa_bulletin_board/partials/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:46:27.785470 aa_bulletin_board-1.9.0/aa_bulletin_board/templates/aa_bulletin_board/partials/header/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-16 15:46:04.000000 aa_bulletin_board-1.9.0/aa_bulletin_board/templates/aa_bulletin_board/partials/header/page-header.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:46:27.785470 aa_bulletin_board-1.9.0/aa_bulletin_board/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-16 15:46:04.000000 aa_bulletin_board-1.9.0/aa_bulletin_board/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-16 15:46:04.000000 aa_bulletin_board-1.9.0/aa_bulletin_board/templatetags/aa_bulletin_board_versioned_static.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:46:27.785470 aa_bulletin_board-1.9.0/aa_bulletin_board/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-16 15:46:04.000000 aa_bulletin_board-1.9.0/aa_bulletin_board/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-04-16 15:46:04.000000 aa_bulletin_board-1.9.0/aa_bulletin_board/tests/test_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-04-16 15:46:04.000000 aa_bulletin_board-1.9.0/aa_bulletin_board/tests/test_auth_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-04-16 15:46:04.000000 aa_bulletin_board-1.9.0/aa_bulletin_board/tests/test_bulletins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-16 15:46:04.000000 aa_bulletin_board-1.9.0/aa_bulletin_board/tests/test_templatetags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7486 2023-04-16 15:46:04.000000 aa_bulletin_board-1.9.0/aa_bulletin_board/tests/test_user_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-16 15:46:04.000000 aa_bulletin_board-1.9.0/aa_bulletin_board/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-16 15:46:04.000000 aa_bulletin_board-1.9.0/aa_bulletin_board/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-04-16 15:46:04.000000 aa_bulletin_board-1.9.0/aa_bulletin_board/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:46:27.781470 aa_bulletin_board-1.9.0/aa_bulletin_board.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14348 2023-04-16 15:46:27.000000 aa_bulletin_board-1.9.0/aa_bulletin_board.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-16 15:46:27.000000 aa_bulletin_board-1.9.0/aa_bulletin_board.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 15:46:27.000000 aa_bulletin_board-1.9.0/aa_bulletin_board.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 15:46:27.000000 aa_bulletin_board-1.9.0/aa_bulletin_board.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-16 15:46:27.000000 aa_bulletin_board-1.9.0/aa_bulletin_board.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-16 15:46:27.000000 aa_bulletin_board-1.9.0/aa_bulletin_board.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-16 15:46:04.000000 aa_bulletin_board-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-04-16 15:46:27.789470 aa_bulletin_board-1.9.0/setup.cfg
```

### Comparing `aa_bulletin_board-1.8.0/LICENSE` & `aa_bulletin_board-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-1.8.0/PKG-INFO` & `aa_bulletin_board-1.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa_bulletin_board
-Version: 1.8.0
+Version: 1.9.0
 Summary: A simple bulletin board for Alliance Auth
 Home-page: https://github.com/ppfeufer/aa-bulletin-board
 Author: Peter Pfeufer
 Author-email: develop@ppfeufer.de
 Maintainer: Peter Pfeufer
 Maintainer-email: develop@ppfeufer.de
 License: GPL-3.0
@@ -42,36 +42,41 @@
 [![codecov](https://codecov.io/gh/ppfeufer/aa-bulletin-board/branch/master/graph/badge.svg?token=UCXABR42QC)](https://codecov.io/gh/ppfeufer/aa-bulletin-board)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](https://github.com/ppfeufer/aa-forum/blob/master/CODE_OF_CONDUCT.md)
 
 [![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/N4N8CL1BY)
 
 Simple bulletin board for [Alliance Auth](https://gitlab.com/allianceauth/allianceauth)
 
-## ⚠️ Before you install this module ⚠️
+
+<!-- TOC -->
+* [AA Bulletin Board](#aa-bulletin-board)
+  * [⚠️ Before You Install This Module ⚠️](#-before-you-install-this-module-)
+  * [Overview](#overview)
+  * [Installation](#installation)
+    * [Step 1: Install the Package](#step-1-install-the-package)
+    * [Step 2: Configure Alliance Auth](#step-2-configure-alliance-auth)
+      * [Settings in `/home/allianceserver/myauth/myauth/settings/local.py`](#settings-in-homeallianceservermyauthmyauthsettingslocalpy)
+      * [Settings in `/home/allianceserver/myauth/myauth/urls.py`](#settings-in-homeallianceservermyauthmyauthurlspy)
+    * [Step 3: Configure Your Webserver](#step-3-configure-your-webserver)
+      * [Apache](#apache)
+      * [Nginx](#nginx)
+    * [Step 4: Finalizing the Installation](#step-4-finalizing-the-installation)
+    * [Step 5: Set Up Permissions](#step-5-set-up-permissions)
+  * [Permissions](#permissions)
+  * [Changelog](#changelog)
+  * [Contributing](#contributing)
+<!-- TOC -->
+
+
+## ⚠️ Before You Install This Module ⚠️
 
 This module needs quite some configuration done before working properly. You need to
 modify your Apache/Nginx configuration as well as the global URL config of Alliance
 Auth. So please only install if you know what you're doing/feel comfortable to make
-these kind of changes. For you own sanity, and mine :-)
-
-## Contents
-- [Overview](#overview)
-    - Features
-    - Screenshots
-- [Installation](#installation)
-    - [Step 1 - Install the package](#step-1---install-the-package)
-    - [Step 2 - Configure Alliance Auth](#step-2---configure-alliance-auth)
-        - [local.py](#settings-in-homeallianceservermyauthmyauthsettingslocalpy)
-        - [urls.py](#settings-in-homeallianceservermyauthmyauthurlspy)
-    - [Step 3 - Configure your webserver](#step-3---configure-your-webserver)
-    - [Step 4 - Finalize the installation](#step-4---finalize-the-installation)
-    - [Step 5 - Set up permissions](#step-5---set-up-permissions)
-- [Permissions](#permissions)
-- [Changelog](#changelog)
-- [Contributing](#contributing)
+these kinds of changes. For your own sanity, and mine :-)
 
 
 ## Overview
 
 Work in progress on this one
 
 
@@ -84,24 +89,24 @@
   [AA installation guide](https://allianceauth.readthedocs.io/en/latest/installation/allianceauth.html)
   or details)
 - Aa Bulletin Board needs a couple of changes made to your Webserver and Alliance
   Auth configuration. So make sure you know how to do so. The steps needed will be
   described in this document, but you need to understand what will be changed.
 
 
-### Step 1 - Install the package
+### Step 1: Install the Package
 
-Make sure you are in the virtual environment (venv) of your Alliance Auth
+Make sure you're in the virtual environment (venv) of your Alliance Auth
 installation Then install the latest release directly from PyPi.
 
 ```shell
 pip install aa-bulletin-board
 ```
 
-### Step 2 - Configure Alliance Auth
+### Step 2: Configure Alliance Auth
 
 #### Settings in `/home/allianceserver/myauth/myauth/settings/local.py`
 
 This is fairly simple, configure your AA settings (`local.py`) as follows:
 
 ```python
 # AA Bulletin Board
@@ -320,39 +325,39 @@
 handler500 = "allianceauth.views.Generic500Redirect"
 handler404 = "allianceauth.views.Generic404Redirect"
 handler403 = "allianceauth.views.Generic403Redirect"
 handler400 = "allianceauth.views.Generic400Redirect"
 ```
 
 
-### Step 3 - Configure your webserver
+### Step 3: Configure Your Webserver
 
-Your webserver needs to know from where to serve the uploaded mages of course, so we
+Your webserver needs to know from where to serve the uploaded images, of course, so we
 have to tell it.
 
 #### Apache
 
 In your vhost configuration you have a line `ProxyPassMatch ^/static !`, which tells
-the server where to find all the static files. We are adding a similar line for the
+the server where to find all the static files. We're adding a similar line for the
 media, right below that one.
 
 Add the following right below the static proxy match:
 ```apache
 ProxyPassMatch ^/media !
 ```
 
 Now we also need to let the server know where to find the media directory we just
 configured the proxy for. To do so, add a new Alias to your configuration. This can
 be done right below the already existing Alias for `/static`:
 ```apache
 Alias "/media" "/var/www/myauth/media/"
 ```
 
-At last a Directory rule is needed as well. Add the following below the already
-existing Directory rule for the static files:
+At last, a Directory rule is needed as well. Add the following code below to the
+already existing Directory rule for the static files:
 
 ```apache
 <Directory "/var/www/myauth/media/">
     Require all granted
 </Directory>
 ```
 
@@ -389,37 +394,37 @@
     autoindex off;
 }
 ```
 
 Restart your Nginx webserver.
 
 
-### Step 4 - Finalize the installation
+### Step 4: Finalizing the Installation
 
 Run static files collection and migrations
 
 ```shell
 python manage.py collectstatic
 python manage.py migrate
 ```
 
 Restart your supervisor services for Auth
 
 
-### Step 5 - Set up permissions
+### Step 5: Set Up Permissions
 
 Now it's time to set up access permissions for your new module. You can do so in
 your admin backend. Read the [Permissions](#permissions) section for more information
 about the available permissions.
 
 
 ## Permissions
 
 | ID                 | Description                   | Notes                                                                           |
-|--------------------|-------------------------------|---------------------------------------------------------------------------------|
+|:-------------------|:------------------------------|:--------------------------------------------------------------------------------|
 | `basic_access`     | Can access the Bulletin Board | Grants read access to the bulletin board                                        |
 | `manage_bulletins` | Can manage bulletins          | Grants the right to edit and delete existing bulletins and create new bulletins |
 
 
 ## Changelog
 
 See [CHANGELOG.md](https://github.com/ppfeufer/aa-bulletin-board/blob/master/CHANGELOG.md)
```

### Comparing `aa_bulletin_board-1.8.0/README.md` & `aa_bulletin_board-1.9.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -11,36 +11,41 @@
 [![codecov](https://codecov.io/gh/ppfeufer/aa-bulletin-board/branch/master/graph/badge.svg?token=UCXABR42QC)](https://codecov.io/gh/ppfeufer/aa-bulletin-board)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](https://github.com/ppfeufer/aa-forum/blob/master/CODE_OF_CONDUCT.md)
 
 [![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/N4N8CL1BY)
 
 Simple bulletin board for [Alliance Auth](https://gitlab.com/allianceauth/allianceauth)
 
-## ⚠️ Before you install this module ⚠️
+
+<!-- TOC -->
+* [AA Bulletin Board](#aa-bulletin-board)
+  * [⚠️ Before You Install This Module ⚠️](#-before-you-install-this-module-)
+  * [Overview](#overview)
+  * [Installation](#installation)
+    * [Step 1: Install the Package](#step-1-install-the-package)
+    * [Step 2: Configure Alliance Auth](#step-2-configure-alliance-auth)
+      * [Settings in `/home/allianceserver/myauth/myauth/settings/local.py`](#settings-in-homeallianceservermyauthmyauthsettingslocalpy)
+      * [Settings in `/home/allianceserver/myauth/myauth/urls.py`](#settings-in-homeallianceservermyauthmyauthurlspy)
+    * [Step 3: Configure Your Webserver](#step-3-configure-your-webserver)
+      * [Apache](#apache)
+      * [Nginx](#nginx)
+    * [Step 4: Finalizing the Installation](#step-4-finalizing-the-installation)
+    * [Step 5: Set Up Permissions](#step-5-set-up-permissions)
+  * [Permissions](#permissions)
+  * [Changelog](#changelog)
+  * [Contributing](#contributing)
+<!-- TOC -->
+
+
+## ⚠️ Before You Install This Module ⚠️
 
 This module needs quite some configuration done before working properly. You need to
 modify your Apache/Nginx configuration as well as the global URL config of Alliance
 Auth. So please only install if you know what you're doing/feel comfortable to make
-these kind of changes. For you own sanity, and mine :-)
-
-## Contents
-- [Overview](#overview)
-    - Features
-    - Screenshots
-- [Installation](#installation)
-    - [Step 1 - Install the package](#step-1---install-the-package)
-    - [Step 2 - Configure Alliance Auth](#step-2---configure-alliance-auth)
-        - [local.py](#settings-in-homeallianceservermyauthmyauthsettingslocalpy)
-        - [urls.py](#settings-in-homeallianceservermyauthmyauthurlspy)
-    - [Step 3 - Configure your webserver](#step-3---configure-your-webserver)
-    - [Step 4 - Finalize the installation](#step-4---finalize-the-installation)
-    - [Step 5 - Set up permissions](#step-5---set-up-permissions)
-- [Permissions](#permissions)
-- [Changelog](#changelog)
-- [Contributing](#contributing)
+these kinds of changes. For your own sanity, and mine :-)
 
 
 ## Overview
 
 Work in progress on this one
 
 
@@ -53,24 +58,24 @@
   [AA installation guide](https://allianceauth.readthedocs.io/en/latest/installation/allianceauth.html)
   or details)
 - Aa Bulletin Board needs a couple of changes made to your Webserver and Alliance
   Auth configuration. So make sure you know how to do so. The steps needed will be
   described in this document, but you need to understand what will be changed.
 
 
-### Step 1 - Install the package
+### Step 1: Install the Package
 
-Make sure you are in the virtual environment (venv) of your Alliance Auth
+Make sure you're in the virtual environment (venv) of your Alliance Auth
 installation Then install the latest release directly from PyPi.
 
 ```shell
 pip install aa-bulletin-board
 ```
 
-### Step 2 - Configure Alliance Auth
+### Step 2: Configure Alliance Auth
 
 #### Settings in `/home/allianceserver/myauth/myauth/settings/local.py`
 
 This is fairly simple, configure your AA settings (`local.py`) as follows:
 
 ```python
 # AA Bulletin Board
@@ -289,39 +294,39 @@
 handler500 = "allianceauth.views.Generic500Redirect"
 handler404 = "allianceauth.views.Generic404Redirect"
 handler403 = "allianceauth.views.Generic403Redirect"
 handler400 = "allianceauth.views.Generic400Redirect"
 ```
 
 
-### Step 3 - Configure your webserver
+### Step 3: Configure Your Webserver
 
-Your webserver needs to know from where to serve the uploaded mages of course, so we
+Your webserver needs to know from where to serve the uploaded images, of course, so we
 have to tell it.
 
 #### Apache
 
 In your vhost configuration you have a line `ProxyPassMatch ^/static !`, which tells
-the server where to find all the static files. We are adding a similar line for the
+the server where to find all the static files. We're adding a similar line for the
 media, right below that one.
 
 Add the following right below the static proxy match:
 ```apache
 ProxyPassMatch ^/media !
 ```
 
 Now we also need to let the server know where to find the media directory we just
 configured the proxy for. To do so, add a new Alias to your configuration. This can
 be done right below the already existing Alias for `/static`:
 ```apache
 Alias "/media" "/var/www/myauth/media/"
 ```
 
-At last a Directory rule is needed as well. Add the following below the already
-existing Directory rule for the static files:
+At last, a Directory rule is needed as well. Add the following code below to the
+already existing Directory rule for the static files:
 
 ```apache
 <Directory "/var/www/myauth/media/">
     Require all granted
 </Directory>
 ```
 
@@ -358,37 +363,37 @@
     autoindex off;
 }
 ```
 
 Restart your Nginx webserver.
 
 
-### Step 4 - Finalize the installation
+### Step 4: Finalizing the Installation
 
 Run static files collection and migrations
 
 ```shell
 python manage.py collectstatic
 python manage.py migrate
 ```
 
 Restart your supervisor services for Auth
 
 
-### Step 5 - Set up permissions
+### Step 5: Set Up Permissions
 
 Now it's time to set up access permissions for your new module. You can do so in
 your admin backend. Read the [Permissions](#permissions) section for more information
 about the available permissions.
 
 
 ## Permissions
 
 | ID                 | Description                   | Notes                                                                           |
-|--------------------|-------------------------------|---------------------------------------------------------------------------------|
+|:-------------------|:------------------------------|:--------------------------------------------------------------------------------|
 | `basic_access`     | Can access the Bulletin Board | Grants read access to the bulletin board                                        |
 | `manage_bulletins` | Can manage bulletins          | Grants the right to edit and delete existing bulletins and create new bulletins |
 
 
 ## Changelog
 
 See [CHANGELOG.md](https://github.com/ppfeufer/aa-bulletin-board/blob/master/CHANGELOG.md)
```

### Comparing `aa_bulletin_board-1.8.0/aa_bulletin_board/auth_hooks.py` & `aa_bulletin_board-1.9.0/aa_bulletin_board/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-1.8.0/aa_bulletin_board/forms.py` & `aa_bulletin_board-1.9.0/aa_bulletin_board/forms.py`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-1.8.0/aa_bulletin_board/helpers.py` & `aa_bulletin_board-1.9.0/aa_bulletin_board/helpers.py`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-1.8.0/aa_bulletin_board/locale/de/LC_MESSAGES/django.mo` & `aa_bulletin_board-1.9.0/aa_bulletin_board/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-1.8.0/aa_bulletin_board/locale/de/LC_MESSAGES/django.po` & `aa_bulletin_board-1.9.0/aa_bulletin_board/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-1.8.0/aa_bulletin_board/locale/es/LC_MESSAGES/django.po` & `aa_bulletin_board-1.9.0/aa_bulletin_board/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-1.8.0/aa_bulletin_board/locale/fr_FR/LC_MESSAGES/django.po` & `aa_bulletin_board-1.9.0/aa_bulletin_board/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-1.8.0/aa_bulletin_board/locale/it_IT/LC_MESSAGES/django.po` & `aa_bulletin_board-1.9.0/aa_bulletin_board/locale/it_IT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-1.8.0/aa_bulletin_board/locale/ja/LC_MESSAGES/django.po` & `aa_bulletin_board-1.9.0/aa_bulletin_board/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-1.8.0/aa_bulletin_board/locale/ko_KR/LC_MESSAGES/django.po` & `aa_bulletin_board-1.9.0/aa_bulletin_board/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-1.8.0/aa_bulletin_board/locale/ru/LC_MESSAGES/django.po` & `aa_bulletin_board-1.9.0/aa_bulletin_board/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
+# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
+#
+#, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-04-11 22:55+0200\n"
-"PO-Revision-Date: 2023-04-11 21:13+0000\n"
-"Last-Translator: \"H. Peter Pfeufer\" <info@ppfeufer.de>\n"
-"Language-Team: Russian <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-bulletin-board/ru/>\n"
-"Language: ru\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"Language-Team: LANGUAGE <LL@li.org>\n"
+"Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
-"n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || ("
-"n%100>=11 && n%100<=14)? 2 : 3);\n"
-"X-Generator: Weblate 4.16.4\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
 #: forms.py:71
 msgid ""
 "Restrict this bulletin to certain groups. If no group restrictions are in "
 "place, everyone who has access to this module can read this bulletin."
 msgstr ""
 
@@ -56,15 +54,15 @@
 #: templates/aa_bulletin_board/dashboard.html:40
 msgid "Edit"
 msgstr ""
 
 #: templates/aa_bulletin_board/bulletin.html:26
 #: templates/aa_bulletin_board/dashboard.html:41
 msgid "Delete"
-msgstr "Удалить"
+msgstr ""
 
 #: templates/aa_bulletin_board/dashboard.html:26
 msgid "This bulletin is restricted to the following group(s):"
 msgstr ""
 
 #: templates/aa_bulletin_board/dashboard.html:37
 msgid "Read more"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `aa_bulletin_board-1.8.0/aa_bulletin_board/managers.py` & `aa_bulletin_board-1.9.0/aa_bulletin_board/managers.py`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-1.8.0/aa_bulletin_board/migrations/0001_initial.py` & `aa_bulletin_board-1.9.0/aa_bulletin_board/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-1.8.0/aa_bulletin_board/migrations/0003_group_restrictions.py` & `aa_bulletin_board-1.9.0/aa_bulletin_board/migrations/0003_group_restrictions.py`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-1.8.0/aa_bulletin_board/models.py` & `aa_bulletin_board-1.9.0/aa_bulletin_board/models.py`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-1.8.0/aa_bulletin_board/static/aa_bulletin_board/css/aa-bulletin-board.css` & `aa_bulletin_board-1.9.0/aa_bulletin_board/static/aa_bulletin_board/css/aa-bulletin-board.css`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-1.8.0/aa_bulletin_board/static/aa_bulletin_board/css/aa-bulletin-board.min.css` & `aa_bulletin_board-1.9.0/aa_bulletin_board/static/aa_bulletin_board/css/aa-bulletin-board.min.css`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-1.8.0/aa_bulletin_board/static/aa_bulletin_board/libs/sumoselect/3.4.8/jquery.sumoselect.js` & `aa_bulletin_board-1.9.0/aa_bulletin_board/static/aa_bulletin_board/libs/sumoselect/3.4.8/jquery.sumoselect.js`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-1.8.0/aa_bulletin_board/static/aa_bulletin_board/libs/sumoselect/3.4.8/jquery.sumoselect.min.js` & `aa_bulletin_board-1.9.0/aa_bulletin_board/static/aa_bulletin_board/libs/sumoselect/3.4.8/jquery.sumoselect.min.js`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-1.8.0/aa_bulletin_board/static/aa_bulletin_board/libs/sumoselect/3.4.8/sumoselect.min.css` & `aa_bulletin_board-1.9.0/aa_bulletin_board/static/aa_bulletin_board/libs/sumoselect/3.4.8/sumoselect.min.css`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-1.8.0/aa_bulletin_board/templates/aa_bulletin_board/bulletin.html` & `aa_bulletin_board-1.9.0/aa_bulletin_board/templates/aa_bulletin_board/bulletin.html`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-1.8.0/aa_bulletin_board/templates/aa_bulletin_board/dashboard.html` & `aa_bulletin_board-1.9.0/aa_bulletin_board/templates/aa_bulletin_board/dashboard.html`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-1.8.0/aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html` & `aa_bulletin_board-1.9.0/aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-1.8.0/aa_bulletin_board/templatetags/aa_bulletin_board_versioned_static.py` & `aa_bulletin_board-1.9.0/aa_bulletin_board/templatetags/aa_bulletin_board_versioned_static.py`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-1.8.0/aa_bulletin_board/tests/test_access.py` & `aa_bulletin_board-1.9.0/aa_bulletin_board/tests/test_access.py`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-1.8.0/aa_bulletin_board/tests/test_auth_hooks.py` & `aa_bulletin_board-1.9.0/aa_bulletin_board/tests/test_auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-1.8.0/aa_bulletin_board/tests/test_bulletins.py` & `aa_bulletin_board-1.9.0/aa_bulletin_board/tests/test_bulletins.py`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-1.8.0/aa_bulletin_board/tests/test_templatetags.py` & `aa_bulletin_board-1.9.0/aa_bulletin_board/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-1.8.0/aa_bulletin_board/tests/test_user_interface.py` & `aa_bulletin_board-1.9.0/aa_bulletin_board/tests/test_user_interface.py`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-1.8.0/aa_bulletin_board/tests/utils.py` & `aa_bulletin_board-1.9.0/aa_bulletin_board/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-1.8.0/aa_bulletin_board/urls.py` & `aa_bulletin_board-1.9.0/aa_bulletin_board/urls.py`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-1.8.0/aa_bulletin_board/views.py` & `aa_bulletin_board-1.9.0/aa_bulletin_board/views.py`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-1.8.0/aa_bulletin_board.egg-info/PKG-INFO` & `aa_bulletin_board-1.9.0/aa_bulletin_board.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-bulletin-board
-Version: 1.8.0
+Version: 1.9.0
 Summary: A simple bulletin board for Alliance Auth
 Home-page: https://github.com/ppfeufer/aa-bulletin-board
 Author: Peter Pfeufer
 Author-email: develop@ppfeufer.de
 Maintainer: Peter Pfeufer
 Maintainer-email: develop@ppfeufer.de
 License: GPL-3.0
@@ -42,36 +42,41 @@
 [![codecov](https://codecov.io/gh/ppfeufer/aa-bulletin-board/branch/master/graph/badge.svg?token=UCXABR42QC)](https://codecov.io/gh/ppfeufer/aa-bulletin-board)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](https://github.com/ppfeufer/aa-forum/blob/master/CODE_OF_CONDUCT.md)
 
 [![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/N4N8CL1BY)
 
 Simple bulletin board for [Alliance Auth](https://gitlab.com/allianceauth/allianceauth)
 
-## ⚠️ Before you install this module ⚠️
+
+<!-- TOC -->
+* [AA Bulletin Board](#aa-bulletin-board)
+  * [⚠️ Before You Install This Module ⚠️](#-before-you-install-this-module-)
+  * [Overview](#overview)
+  * [Installation](#installation)
+    * [Step 1: Install the Package](#step-1-install-the-package)
+    * [Step 2: Configure Alliance Auth](#step-2-configure-alliance-auth)
+      * [Settings in `/home/allianceserver/myauth/myauth/settings/local.py`](#settings-in-homeallianceservermyauthmyauthsettingslocalpy)
+      * [Settings in `/home/allianceserver/myauth/myauth/urls.py`](#settings-in-homeallianceservermyauthmyauthurlspy)
+    * [Step 3: Configure Your Webserver](#step-3-configure-your-webserver)
+      * [Apache](#apache)
+      * [Nginx](#nginx)
+    * [Step 4: Finalizing the Installation](#step-4-finalizing-the-installation)
+    * [Step 5: Set Up Permissions](#step-5-set-up-permissions)
+  * [Permissions](#permissions)
+  * [Changelog](#changelog)
+  * [Contributing](#contributing)
+<!-- TOC -->
+
+
+## ⚠️ Before You Install This Module ⚠️
 
 This module needs quite some configuration done before working properly. You need to
 modify your Apache/Nginx configuration as well as the global URL config of Alliance
 Auth. So please only install if you know what you're doing/feel comfortable to make
-these kind of changes. For you own sanity, and mine :-)
-
-## Contents
-- [Overview](#overview)
-    - Features
-    - Screenshots
-- [Installation](#installation)
-    - [Step 1 - Install the package](#step-1---install-the-package)
-    - [Step 2 - Configure Alliance Auth](#step-2---configure-alliance-auth)
-        - [local.py](#settings-in-homeallianceservermyauthmyauthsettingslocalpy)
-        - [urls.py](#settings-in-homeallianceservermyauthmyauthurlspy)
-    - [Step 3 - Configure your webserver](#step-3---configure-your-webserver)
-    - [Step 4 - Finalize the installation](#step-4---finalize-the-installation)
-    - [Step 5 - Set up permissions](#step-5---set-up-permissions)
-- [Permissions](#permissions)
-- [Changelog](#changelog)
-- [Contributing](#contributing)
+these kinds of changes. For your own sanity, and mine :-)
 
 
 ## Overview
 
 Work in progress on this one
 
 
@@ -84,24 +89,24 @@
   [AA installation guide](https://allianceauth.readthedocs.io/en/latest/installation/allianceauth.html)
   or details)
 - Aa Bulletin Board needs a couple of changes made to your Webserver and Alliance
   Auth configuration. So make sure you know how to do so. The steps needed will be
   described in this document, but you need to understand what will be changed.
 
 
-### Step 1 - Install the package
+### Step 1: Install the Package
 
-Make sure you are in the virtual environment (venv) of your Alliance Auth
+Make sure you're in the virtual environment (venv) of your Alliance Auth
 installation Then install the latest release directly from PyPi.
 
 ```shell
 pip install aa-bulletin-board
 ```
 
-### Step 2 - Configure Alliance Auth
+### Step 2: Configure Alliance Auth
 
 #### Settings in `/home/allianceserver/myauth/myauth/settings/local.py`
 
 This is fairly simple, configure your AA settings (`local.py`) as follows:
 
 ```python
 # AA Bulletin Board
@@ -320,39 +325,39 @@
 handler500 = "allianceauth.views.Generic500Redirect"
 handler404 = "allianceauth.views.Generic404Redirect"
 handler403 = "allianceauth.views.Generic403Redirect"
 handler400 = "allianceauth.views.Generic400Redirect"
 ```
 
 
-### Step 3 - Configure your webserver
+### Step 3: Configure Your Webserver
 
-Your webserver needs to know from where to serve the uploaded mages of course, so we
+Your webserver needs to know from where to serve the uploaded images, of course, so we
 have to tell it.
 
 #### Apache
 
 In your vhost configuration you have a line `ProxyPassMatch ^/static !`, which tells
-the server where to find all the static files. We are adding a similar line for the
+the server where to find all the static files. We're adding a similar line for the
 media, right below that one.
 
 Add the following right below the static proxy match:
 ```apache
 ProxyPassMatch ^/media !
 ```
 
 Now we also need to let the server know where to find the media directory we just
 configured the proxy for. To do so, add a new Alias to your configuration. This can
 be done right below the already existing Alias for `/static`:
 ```apache
 Alias "/media" "/var/www/myauth/media/"
 ```
 
-At last a Directory rule is needed as well. Add the following below the already
-existing Directory rule for the static files:
+At last, a Directory rule is needed as well. Add the following code below to the
+already existing Directory rule for the static files:
 
 ```apache
 <Directory "/var/www/myauth/media/">
     Require all granted
 </Directory>
 ```
 
@@ -389,37 +394,37 @@
     autoindex off;
 }
 ```
 
 Restart your Nginx webserver.
 
 
-### Step 4 - Finalize the installation
+### Step 4: Finalizing the Installation
 
 Run static files collection and migrations
 
 ```shell
 python manage.py collectstatic
 python manage.py migrate
 ```
 
 Restart your supervisor services for Auth
 
 
-### Step 5 - Set up permissions
+### Step 5: Set Up Permissions
 
 Now it's time to set up access permissions for your new module. You can do so in
 your admin backend. Read the [Permissions](#permissions) section for more information
 about the available permissions.
 
 
 ## Permissions
 
 | ID                 | Description                   | Notes                                                                           |
-|--------------------|-------------------------------|---------------------------------------------------------------------------------|
+|:-------------------|:------------------------------|:--------------------------------------------------------------------------------|
 | `basic_access`     | Can access the Bulletin Board | Grants read access to the bulletin board                                        |
 | `manage_bulletins` | Can manage bulletins          | Grants the right to edit and delete existing bulletins and create new bulletins |
 
 
 ## Changelog
 
 See [CHANGELOG.md](https://github.com/ppfeufer/aa-bulletin-board/blob/master/CHANGELOG.md)
```

### Comparing `aa_bulletin_board-1.8.0/aa_bulletin_board.egg-info/SOURCES.txt` & `aa_bulletin_board-1.9.0/aa_bulletin_board.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-1.8.0/setup.cfg` & `aa_bulletin_board-1.9.0/setup.cfg`

 * *Files identical despite different names*

