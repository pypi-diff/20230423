# Comparing `tmp/wagtailmedia-0.8.0.tar.gz` & `tmp/wagtailmedia-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtailmedia-0.8.0.tar", last modified: Sat Sep 11 10:44:15 2021, max compression
+gzip compressed data, was "wagtailmedia-0.9.0.tar", last modified: Tue Feb 22 11:14:00 2022, max compression
```

## Comparing `wagtailmedia-0.8.0.tar` & `wagtailmedia-0.9.0.tar`

### file list

```diff
@@ -1,91 +1,94 @@
-drwxr-xr-x   0 dan        (502) staff       (20)        0 2021-09-11 10:44:15.805666 wagtailmedia-0.8.0/
--rw-r--r--   0 dan        (502) staff       (20)      519 2019-12-01 14:27:03.000000 wagtailmedia-0.8.0/.editorconfig
--rw-r--r--   0 dan        (502) staff       (20)     9294 2021-09-11 10:18:20.000000 wagtailmedia-0.8.0/CHANGELOG.md
--rw-r--r--   0 dan        (502) staff       (20)     1545 2019-12-01 14:27:03.000000 wagtailmedia-0.8.0/LICENSE
--rw-r--r--   0 dan        (502) staff       (20)      290 2021-09-05 14:33:28.000000 wagtailmedia-0.8.0/MANIFEST.in
--rw-r--r--   0 dan        (502) staff       (20)    10415 2021-09-11 10:44:15.806539 wagtailmedia-0.8.0/PKG-INFO
--rw-r--r--   0 dan        (502) staff       (20)     9018 2021-09-11 10:10:14.000000 wagtailmedia-0.8.0/README.md
--rw-r--r--   0 dan        (502) staff       (20)     1459 2020-11-20 23:38:58.000000 wagtailmedia-0.8.0/SPECIFICATION.md
--rw-r--r--   0 dan        (502) staff       (20)      384 2021-08-30 12:16:32.000000 wagtailmedia-0.8.0/pyproject.toml
--rw-r--r--   0 dan        (502) staff       (20)      757 2021-09-11 10:44:15.810560 wagtailmedia-0.8.0/setup.cfg
--rw-r--r--   0 dan        (502) staff       (20)     2120 2021-08-30 12:16:32.000000 wagtailmedia-0.8.0/setup.py
-drwxr-xr-x   0 dan        (502) staff       (20)        0 2021-09-11 10:44:15.755067 wagtailmedia-0.8.0/src/
-drwxr-xr-x   0 dan        (502) staff       (20)        0 2021-09-11 10:44:15.767019 wagtailmedia-0.8.0/src/wagtailmedia/
--rw-r--r--   0 dan        (502) staff       (20)       86 2021-09-11 10:17:53.000000 wagtailmedia-0.8.0/src/wagtailmedia/__init__.py
-drwxr-xr-x   0 dan        (502) staff       (20)        0 2021-09-11 10:44:15.768810 wagtailmedia-0.8.0/src/wagtailmedia/__pycache__/
--rw-r--r--   0 dan        (502) staff       (20)      262 2021-09-11 10:44:15.000000 wagtailmedia-0.8.0/src/wagtailmedia/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 dan        (502) staff       (20)      398 2021-09-11 10:10:14.000000 wagtailmedia-0.8.0/src/wagtailmedia/admin.py
--rw-r--r--   0 dan        (502) staff       (20)      802 2021-09-05 11:47:43.000000 wagtailmedia-0.8.0/src/wagtailmedia/admin_urls.py
--rw-r--r--   0 dan        (502) staff       (20)      350 2021-08-30 12:16:32.000000 wagtailmedia-0.8.0/src/wagtailmedia/apps.py
--rw-r--r--   0 dan        (502) staff       (20)     3441 2021-09-05 11:47:43.000000 wagtailmedia-0.8.0/src/wagtailmedia/blocks.py
--rw-r--r--   0 dan        (502) staff       (20)      145 2021-09-11 10:10:14.000000 wagtailmedia-0.8.0/src/wagtailmedia/deprecation.py
--rw-r--r--   0 dan        (502) staff       (20)      906 2021-09-05 11:47:43.000000 wagtailmedia-0.8.0/src/wagtailmedia/edit_handlers.py
--rw-r--r--   0 dan        (502) staff       (20)     2339 2021-09-11 10:10:14.000000 wagtailmedia-0.8.0/src/wagtailmedia/forms.py
-drwxr-xr-x   0 dan        (502) staff       (20)        0 2021-09-11 10:44:15.769043 wagtailmedia-0.8.0/src/wagtailmedia/locale/
--rw-r--r--   0 dan        (502) staff       (20)        0 2021-08-30 12:16:32.000000 wagtailmedia-0.8.0/src/wagtailmedia/locale/.gitkeep
-drwxr-xr-x   0 dan        (502) staff       (20)        0 2021-09-11 10:44:15.755628 wagtailmedia-0.8.0/src/wagtailmedia/locale/de/
-drwxr-xr-x   0 dan        (502) staff       (20)        0 2021-09-11 10:44:15.769534 wagtailmedia-0.8.0/src/wagtailmedia/locale/de/LC_MESSAGES/
--rw-r--r--   0 dan        (502) staff       (20)     5631 2021-08-30 12:16:32.000000 wagtailmedia-0.8.0/src/wagtailmedia/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 dan        (502) staff       (20)     9590 2021-08-30 12:16:32.000000 wagtailmedia-0.8.0/src/wagtailmedia/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 dan        (502) staff       (20)        0 2021-09-11 10:44:15.755875 wagtailmedia-0.8.0/src/wagtailmedia/locale/fr/
-drwxr-xr-x   0 dan        (502) staff       (20)        0 2021-09-11 10:44:15.769989 wagtailmedia-0.8.0/src/wagtailmedia/locale/fr/LC_MESSAGES/
--rw-r--r--   0 dan        (502) staff       (20)     5526 2021-08-30 12:16:32.000000 wagtailmedia-0.8.0/src/wagtailmedia/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 dan        (502) staff       (20)     9462 2021-08-30 12:16:32.000000 wagtailmedia-0.8.0/src/wagtailmedia/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 dan        (502) staff       (20)        0 2021-09-11 10:44:15.756123 wagtailmedia-0.8.0/src/wagtailmedia/locale/zh_Hans/
-drwxr-xr-x   0 dan        (502) staff       (20)        0 2021-09-11 10:44:15.770457 wagtailmedia-0.8.0/src/wagtailmedia/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 dan        (502) staff       (20)     5225 2021-08-30 12:16:32.000000 wagtailmedia-0.8.0/src/wagtailmedia/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0 dan        (502) staff       (20)     9152 2021-08-30 12:16:32.000000 wagtailmedia-0.8.0/src/wagtailmedia/locale/zh_Hans/LC_MESSAGES/django.po
-drwxr-xr-x   0 dan        (502) staff       (20)        0 2021-09-11 10:44:15.772150 wagtailmedia-0.8.0/src/wagtailmedia/migrations/
--rw-r--r--   0 dan        (502) staff       (20)     3843 2021-08-30 12:16:32.000000 wagtailmedia-0.8.0/src/wagtailmedia/migrations/0001_initial.py
--rw-r--r--   0 dan        (502) staff       (20)     2349 2021-08-30 12:16:32.000000 wagtailmedia-0.8.0/src/wagtailmedia/migrations/0002_initial_data.py
--rw-r--r--   0 dan        (502) staff       (20)     1804 2021-08-30 12:16:32.000000 wagtailmedia-0.8.0/src/wagtailmedia/migrations/0003_copy_media_permissions_to_collections.py
--rw-r--r--   0 dan        (502) staff       (20)      661 2021-08-30 12:16:32.000000 wagtailmedia-0.8.0/src/wagtailmedia/migrations/0004_duration_optional_floatfield.py
--rw-r--r--   0 dan        (502) staff       (20)        0 2021-08-30 12:16:32.000000 wagtailmedia-0.8.0/src/wagtailmedia/migrations/__init__.py
--rw-r--r--   0 dan        (502) staff       (20)     5254 2021-09-11 10:10:14.000000 wagtailmedia-0.8.0/src/wagtailmedia/models.py
--rw-r--r--   0 dan        (502) staff       (20)      296 2021-08-30 12:16:32.000000 wagtailmedia-0.8.0/src/wagtailmedia/permissions.py
--rw-r--r--   0 dan        (502) staff       (20)     4041 2021-09-11 10:10:14.000000 wagtailmedia-0.8.0/src/wagtailmedia/settings.py
--rw-r--r--   0 dan        (502) staff       (20)      523 2021-08-30 12:16:32.000000 wagtailmedia-0.8.0/src/wagtailmedia/signal_handlers.py
-drwxr-xr-x   0 dan        (502) staff       (20)        0 2021-09-11 10:44:15.756516 wagtailmedia-0.8.0/src/wagtailmedia/static/
-drwxr-xr-x   0 dan        (502) staff       (20)        0 2021-09-11 10:44:15.756609 wagtailmedia-0.8.0/src/wagtailmedia/static/wagtailmedia/
-drwxr-xr-x   0 dan        (502) staff       (20)        0 2021-09-11 10:44:15.773128 wagtailmedia-0.8.0/src/wagtailmedia/static/wagtailmedia/js/
--rw-r--r--   0 dan        (502) staff       (20)     5321 2021-08-30 12:16:32.000000 wagtailmedia-0.8.0/src/wagtailmedia/static/wagtailmedia/js/media-chooser-modal.js
--rw-r--r--   0 dan        (502) staff       (20)      738 2021-08-30 12:16:32.000000 wagtailmedia-0.8.0/src/wagtailmedia/static/wagtailmedia/js/media-chooser-telepath.js
--rw-r--r--   0 dan        (502) staff       (20)     2075 2021-09-05 11:47:43.000000 wagtailmedia-0.8.0/src/wagtailmedia/static/wagtailmedia/js/media-chooser.js
-drwxr-xr-x   0 dan        (502) staff       (20)        0 2021-09-11 10:44:15.756956 wagtailmedia-0.8.0/src/wagtailmedia/templates/
-drwxr-xr-x   0 dan        (502) staff       (20)        0 2021-09-11 10:44:15.758503 wagtailmedia-0.8.0/src/wagtailmedia/templates/wagtailmedia/
-drwxr-xr-x   0 dan        (502) staff       (20)        0 2021-09-11 10:44:15.773621 wagtailmedia-0.8.0/src/wagtailmedia/templates/wagtailmedia/chooser/
--rw-r--r--   0 dan        (502) staff       (20)     3540 2021-09-05 11:47:43.000000 wagtailmedia-0.8.0/src/wagtailmedia/templates/wagtailmedia/chooser/chooser.html
--rw-r--r--   0 dan        (502) staff       (20)     1294 2021-09-05 11:47:43.000000 wagtailmedia-0.8.0/src/wagtailmedia/templates/wagtailmedia/chooser/results.html
-drwxr-xr-x   0 dan        (502) staff       (20)        0 2021-09-11 10:44:15.773864 wagtailmedia-0.8.0/src/wagtailmedia/templates/wagtailmedia/homepage/
--rw-r--r--   0 dan        (502) staff       (20)      337 2021-08-30 12:16:32.000000 wagtailmedia-0.8.0/src/wagtailmedia/templates/wagtailmedia/homepage/site_summary_media.html
-drwxr-xr-x   0 dan        (502) staff       (20)        0 2021-09-11 10:44:15.799079 wagtailmedia-0.8.0/src/wagtailmedia/templates/wagtailmedia/media/
--rw-r--r--   0 dan        (502) staff       (20)      245 2021-08-30 12:16:32.000000 wagtailmedia-0.8.0/src/wagtailmedia/templates/wagtailmedia/media/_file_field.html
--rw-r--r--   0 dan        (502) staff       (20)      230 2021-08-30 12:16:32.000000 wagtailmedia-0.8.0/src/wagtailmedia/templates/wagtailmedia/media/_file_field_as_li.html
--rw-r--r--   0 dan        (502) staff       (20)      320 2021-08-30 12:16:32.000000 wagtailmedia-0.8.0/src/wagtailmedia/templates/wagtailmedia/media/_thumbnail_field.html
--rw-r--r--   0 dan        (502) staff       (20)      235 2021-08-30 12:16:32.000000 wagtailmedia-0.8.0/src/wagtailmedia/templates/wagtailmedia/media/_thumbnail_field_as_li.html
--rw-r--r--   0 dan        (502) staff       (20)     1805 2021-08-30 12:16:32.000000 wagtailmedia-0.8.0/src/wagtailmedia/templates/wagtailmedia/media/add.html
--rw-r--r--   0 dan        (502) staff       (20)     1068 2021-08-30 12:16:32.000000 wagtailmedia-0.8.0/src/wagtailmedia/templates/wagtailmedia/media/confirm_delete.html
--rw-r--r--   0 dan        (502) staff       (20)     3154 2021-08-30 12:16:32.000000 wagtailmedia-0.8.0/src/wagtailmedia/templates/wagtailmedia/media/edit.html
--rw-r--r--   0 dan        (502) staff       (20)     4084 2021-08-30 12:16:32.000000 wagtailmedia-0.8.0/src/wagtailmedia/templates/wagtailmedia/media/index.html
--rw-r--r--   0 dan        (502) staff       (20)     2210 2021-08-30 12:16:32.000000 wagtailmedia-0.8.0/src/wagtailmedia/templates/wagtailmedia/media/list.html
--rw-r--r--   0 dan        (502) staff       (20)     1433 2021-08-30 12:16:32.000000 wagtailmedia-0.8.0/src/wagtailmedia/templates/wagtailmedia/media/results.html
--rw-r--r--   0 dan        (502) staff       (20)     1903 2021-08-30 12:16:32.000000 wagtailmedia-0.8.0/src/wagtailmedia/templates/wagtailmedia/media/usage.html
-drwxr-xr-x   0 dan        (502) staff       (20)        0 2021-09-11 10:44:15.758147 wagtailmedia-0.8.0/src/wagtailmedia/templates/wagtailmedia/permissions/
-drwxr-xr-x   0 dan        (502) staff       (20)        0 2021-09-11 10:44:15.799653 wagtailmedia-0.8.0/src/wagtailmedia/templates/wagtailmedia/permissions/includes/
--rw-r--r--   0 dan        (502) staff       (20)      252 2021-08-30 12:16:32.000000 wagtailmedia-0.8.0/src/wagtailmedia/templates/wagtailmedia/permissions/includes/media_permissions_formset.html
-drwxr-xr-x   0 dan        (502) staff       (20)        0 2021-09-11 10:44:15.800257 wagtailmedia-0.8.0/src/wagtailmedia/templates/wagtailmedia/widgets/
--rw-r--r--   0 dan        (502) staff       (20)      335 2021-09-05 11:47:43.000000 wagtailmedia-0.8.0/src/wagtailmedia/templates/wagtailmedia/widgets/media_chooser.html
--rw-r--r--   0 dan        (502) staff       (20)      268 2021-08-30 12:16:32.000000 wagtailmedia-0.8.0/src/wagtailmedia/utils.py
-drwxr-xr-x   0 dan        (502) staff       (20)        0 2021-09-11 10:44:15.804312 wagtailmedia-0.8.0/src/wagtailmedia/views/
--rw-r--r--   0 dan        (502) staff       (20)        0 2021-08-30 12:16:32.000000 wagtailmedia-0.8.0/src/wagtailmedia/views/__init__.py
--rw-r--r--   0 dan        (502) staff       (20)     7369 2021-09-05 11:47:43.000000 wagtailmedia-0.8.0/src/wagtailmedia/views/chooser.py
--rw-r--r--   0 dan        (502) staff       (20)     8383 2021-08-30 12:16:32.000000 wagtailmedia-0.8.0/src/wagtailmedia/views/media.py
--rw-r--r--   0 dan        (502) staff       (20)     2792 2021-09-05 11:47:43.000000 wagtailmedia-0.8.0/src/wagtailmedia/wagtail_hooks.py
--rw-r--r--   0 dan        (502) staff       (20)     3916 2021-09-05 11:47:43.000000 wagtailmedia-0.8.0/src/wagtailmedia/widgets.py
-drwxr-xr-x   0 dan        (502) staff       (20)        0 2021-09-11 10:44:15.768579 wagtailmedia-0.8.0/src/wagtailmedia.egg-info/
--rw-r--r--   0 dan        (502) staff       (20)    10415 2021-09-11 10:44:15.000000 wagtailmedia-0.8.0/src/wagtailmedia.egg-info/PKG-INFO
--rw-r--r--   0 dan        (502) staff       (20)     2770 2021-09-11 10:44:15.000000 wagtailmedia-0.8.0/src/wagtailmedia.egg-info/SOURCES.txt
--rw-r--r--   0 dan        (502) staff       (20)        1 2021-09-11 10:44:15.000000 wagtailmedia-0.8.0/src/wagtailmedia.egg-info/dependency_links.txt
--rw-r--r--   0 dan        (502) staff       (20)        1 2021-08-16 22:49:41.000000 wagtailmedia-0.8.0/src/wagtailmedia.egg-info/not-zip-safe
--rw-r--r--   0 dan        (502) staff       (20)       65 2021-09-11 10:44:15.000000 wagtailmedia-0.8.0/src/wagtailmedia.egg-info/requires.txt
--rw-r--r--   0 dan        (502) staff       (20)       13 2021-09-11 10:44:15.000000 wagtailmedia-0.8.0/src/wagtailmedia.egg-info/top_level.txt
+drwxr-xr-x   0 dan        (502) staff       (20)        0 2022-02-22 11:14:00.681942 wagtailmedia-0.9.0/
+-rw-r--r--   0 dan        (502) staff       (20)      519 2019-12-01 14:27:03.000000 wagtailmedia-0.9.0/.editorconfig
+-rw-r--r--   0 dan        (502) staff       (20)     9965 2022-02-22 11:10:19.000000 wagtailmedia-0.9.0/CHANGELOG.md
+-rw-r--r--   0 dan        (502) staff       (20)     1545 2019-12-01 14:27:03.000000 wagtailmedia-0.9.0/LICENSE
+-rw-r--r--   0 dan        (502) staff       (20)      290 2021-09-05 14:33:28.000000 wagtailmedia-0.9.0/MANIFEST.in
+-rw-r--r--   0 dan        (502) staff       (20)    10588 2022-02-22 11:14:00.682218 wagtailmedia-0.9.0/PKG-INFO
+-rw-r--r--   0 dan        (502) staff       (20)     9280 2022-02-22 11:11:14.000000 wagtailmedia-0.9.0/README.md
+-rw-r--r--   0 dan        (502) staff       (20)     1459 2020-11-20 23:38:58.000000 wagtailmedia-0.9.0/SPECIFICATION.md
+-rw-r--r--   0 dan        (502) staff       (20)      384 2021-08-30 12:16:32.000000 wagtailmedia-0.9.0/pyproject.toml
+-rw-r--r--   0 dan        (502) staff       (20)      757 2022-02-22 11:14:00.683580 wagtailmedia-0.9.0/setup.cfg
+-rw-r--r--   0 dan        (502) staff       (20)     2094 2022-02-16 09:16:03.000000 wagtailmedia-0.9.0/setup.py
+drwxr-xr-x   0 dan        (502) staff       (20)        0 2022-02-22 11:14:00.641375 wagtailmedia-0.9.0/src/
+drwxr-xr-x   0 dan        (502) staff       (20)        0 2022-02-22 11:14:00.657084 wagtailmedia-0.9.0/src/wagtailmedia/
+-rw-r--r--   0 dan        (502) staff       (20)      263 2022-02-16 09:16:03.000000 wagtailmedia-0.9.0/src/wagtailmedia/__init__.py
+-rw-r--r--   0 dan        (502) staff       (20)      398 2021-09-11 10:10:14.000000 wagtailmedia-0.9.0/src/wagtailmedia/admin.py
+-rw-r--r--   0 dan        (502) staff       (20)      802 2021-09-05 11:47:43.000000 wagtailmedia-0.9.0/src/wagtailmedia/admin_urls.py
+-rw-r--r--   0 dan        (502) staff       (20)      350 2021-08-30 12:16:32.000000 wagtailmedia-0.9.0/src/wagtailmedia/apps.py
+-rw-r--r--   0 dan        (502) staff       (20)     3441 2021-09-05 11:47:43.000000 wagtailmedia-0.9.0/src/wagtailmedia/blocks.py
+-rw-r--r--   0 dan        (502) staff       (20)      145 2021-09-11 10:10:14.000000 wagtailmedia-0.9.0/src/wagtailmedia/deprecation.py
+-rw-r--r--   0 dan        (502) staff       (20)      906 2021-09-05 11:47:43.000000 wagtailmedia-0.9.0/src/wagtailmedia/edit_handlers.py
+-rw-r--r--   0 dan        (502) staff       (20)     2303 2022-01-23 11:32:20.000000 wagtailmedia-0.9.0/src/wagtailmedia/forms.py
+drwxr-xr-x   0 dan        (502) staff       (20)        0 2022-02-22 11:14:00.659610 wagtailmedia-0.9.0/src/wagtailmedia/locale/
+-rw-r--r--   0 dan        (502) staff       (20)        0 2021-08-30 12:16:32.000000 wagtailmedia-0.9.0/src/wagtailmedia/locale/.gitkeep
+drwxr-xr-x   0 dan        (502) staff       (20)        0 2022-02-22 11:14:00.641748 wagtailmedia-0.9.0/src/wagtailmedia/locale/de/
+drwxr-xr-x   0 dan        (502) staff       (20)        0 2022-02-22 11:14:00.660397 wagtailmedia-0.9.0/src/wagtailmedia/locale/de/LC_MESSAGES/
+-rw-r--r--   0 dan        (502) staff       (20)     5631 2021-08-30 12:16:32.000000 wagtailmedia-0.9.0/src/wagtailmedia/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 dan        (502) staff       (20)     9590 2021-08-30 12:16:32.000000 wagtailmedia-0.9.0/src/wagtailmedia/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 dan        (502) staff       (20)        0 2022-02-22 11:14:00.641981 wagtailmedia-0.9.0/src/wagtailmedia/locale/fr/
+drwxr-xr-x   0 dan        (502) staff       (20)        0 2022-02-22 11:14:00.661446 wagtailmedia-0.9.0/src/wagtailmedia/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 dan        (502) staff       (20)     5526 2021-08-30 12:16:32.000000 wagtailmedia-0.9.0/src/wagtailmedia/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 dan        (502) staff       (20)     9462 2021-08-30 12:16:32.000000 wagtailmedia-0.9.0/src/wagtailmedia/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 dan        (502) staff       (20)        0 2022-02-22 11:14:00.642261 wagtailmedia-0.9.0/src/wagtailmedia/locale/uk/
+drwxr-xr-x   0 dan        (502) staff       (20)        0 2022-02-22 11:14:00.662560 wagtailmedia-0.9.0/src/wagtailmedia/locale/uk/LC_MESSAGES/
+-rw-r--r--   0 dan        (502) staff       (20)     8210 2022-01-23 10:24:08.000000 wagtailmedia-0.9.0/src/wagtailmedia/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0 dan        (502) staff       (20)    14699 2022-01-23 10:24:08.000000 wagtailmedia-0.9.0/src/wagtailmedia/locale/uk/LC_MESSAGES/django.po
+drwxr-xr-x   0 dan        (502) staff       (20)        0 2022-02-22 11:14:00.642453 wagtailmedia-0.9.0/src/wagtailmedia/locale/zh_Hans/
+drwxr-xr-x   0 dan        (502) staff       (20)        0 2022-02-22 11:14:00.663960 wagtailmedia-0.9.0/src/wagtailmedia/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 dan        (502) staff       (20)     5225 2021-08-30 12:16:32.000000 wagtailmedia-0.9.0/src/wagtailmedia/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0 dan        (502) staff       (20)     9152 2021-08-30 12:16:32.000000 wagtailmedia-0.9.0/src/wagtailmedia/locale/zh_Hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 dan        (502) staff       (20)        0 2022-02-22 11:14:00.666764 wagtailmedia-0.9.0/src/wagtailmedia/migrations/
+-rw-r--r--   0 dan        (502) staff       (20)     3843 2021-08-30 12:16:32.000000 wagtailmedia-0.9.0/src/wagtailmedia/migrations/0001_initial.py
+-rw-r--r--   0 dan        (502) staff       (20)     2349 2021-08-30 12:16:32.000000 wagtailmedia-0.9.0/src/wagtailmedia/migrations/0002_initial_data.py
+-rw-r--r--   0 dan        (502) staff       (20)     1804 2021-08-30 12:16:32.000000 wagtailmedia-0.9.0/src/wagtailmedia/migrations/0003_copy_media_permissions_to_collections.py
+-rw-r--r--   0 dan        (502) staff       (20)      661 2021-08-30 12:16:32.000000 wagtailmedia-0.9.0/src/wagtailmedia/migrations/0004_duration_optional_floatfield.py
+-rw-r--r--   0 dan        (502) staff       (20)        0 2021-08-30 12:16:32.000000 wagtailmedia-0.9.0/src/wagtailmedia/migrations/__init__.py
+-rw-r--r--   0 dan        (502) staff       (20)     5290 2021-10-29 09:40:56.000000 wagtailmedia-0.9.0/src/wagtailmedia/models.py
+-rw-r--r--   0 dan        (502) staff       (20)      296 2021-08-30 12:16:32.000000 wagtailmedia-0.9.0/src/wagtailmedia/permissions.py
+-rw-r--r--   0 dan        (502) staff       (20)     4041 2021-09-11 10:10:14.000000 wagtailmedia-0.9.0/src/wagtailmedia/settings.py
+-rw-r--r--   0 dan        (502) staff       (20)      523 2021-08-30 12:16:32.000000 wagtailmedia-0.9.0/src/wagtailmedia/signal_handlers.py
+drwxr-xr-x   0 dan        (502) staff       (20)        0 2022-02-22 11:14:00.643031 wagtailmedia-0.9.0/src/wagtailmedia/static/
+drwxr-xr-x   0 dan        (502) staff       (20)        0 2022-02-22 11:14:00.643183 wagtailmedia-0.9.0/src/wagtailmedia/static/wagtailmedia/
+drwxr-xr-x   0 dan        (502) staff       (20)        0 2022-02-22 11:14:00.668616 wagtailmedia-0.9.0/src/wagtailmedia/static/wagtailmedia/js/
+-rw-r--r--   0 dan        (502) staff       (20)     5321 2021-08-30 12:16:32.000000 wagtailmedia-0.9.0/src/wagtailmedia/static/wagtailmedia/js/media-chooser-modal.js
+-rw-r--r--   0 dan        (502) staff       (20)      738 2021-08-30 12:16:32.000000 wagtailmedia-0.9.0/src/wagtailmedia/static/wagtailmedia/js/media-chooser-telepath.js
+-rw-r--r--   0 dan        (502) staff       (20)     2075 2021-09-05 11:47:43.000000 wagtailmedia-0.9.0/src/wagtailmedia/static/wagtailmedia/js/media-chooser.js
+drwxr-xr-x   0 dan        (502) staff       (20)        0 2022-02-22 11:14:00.643548 wagtailmedia-0.9.0/src/wagtailmedia/templates/
+drwxr-xr-x   0 dan        (502) staff       (20)        0 2022-02-22 11:14:00.644186 wagtailmedia-0.9.0/src/wagtailmedia/templates/wagtailmedia/
+drwxr-xr-x   0 dan        (502) staff       (20)        0 2022-02-22 11:14:00.670531 wagtailmedia-0.9.0/src/wagtailmedia/templates/wagtailmedia/chooser/
+-rw-r--r--   0 dan        (502) staff       (20)     3540 2021-09-05 11:47:43.000000 wagtailmedia-0.9.0/src/wagtailmedia/templates/wagtailmedia/chooser/chooser.html
+-rw-r--r--   0 dan        (502) staff       (20)     1294 2022-01-23 22:28:34.000000 wagtailmedia-0.9.0/src/wagtailmedia/templates/wagtailmedia/chooser/results.html
+drwxr-xr-x   0 dan        (502) staff       (20)        0 2022-02-22 11:14:00.671311 wagtailmedia-0.9.0/src/wagtailmedia/templates/wagtailmedia/homepage/
+-rw-r--r--   0 dan        (502) staff       (20)      337 2022-02-09 11:16:29.000000 wagtailmedia-0.9.0/src/wagtailmedia/templates/wagtailmedia/homepage/site_summary_media.html
+drwxr-xr-x   0 dan        (502) staff       (20)        0 2022-02-22 11:14:00.678346 wagtailmedia-0.9.0/src/wagtailmedia/templates/wagtailmedia/media/
+-rw-r--r--   0 dan        (502) staff       (20)      245 2021-08-30 12:16:32.000000 wagtailmedia-0.9.0/src/wagtailmedia/templates/wagtailmedia/media/_file_field.html
+-rw-r--r--   0 dan        (502) staff       (20)      230 2021-08-30 12:16:32.000000 wagtailmedia-0.9.0/src/wagtailmedia/templates/wagtailmedia/media/_file_field_as_li.html
+-rw-r--r--   0 dan        (502) staff       (20)      320 2021-08-30 12:16:32.000000 wagtailmedia-0.9.0/src/wagtailmedia/templates/wagtailmedia/media/_thumbnail_field.html
+-rw-r--r--   0 dan        (502) staff       (20)      235 2021-08-30 12:16:32.000000 wagtailmedia-0.9.0/src/wagtailmedia/templates/wagtailmedia/media/_thumbnail_field_as_li.html
+-rw-r--r--   0 dan        (502) staff       (20)     1805 2021-08-30 12:16:32.000000 wagtailmedia-0.9.0/src/wagtailmedia/templates/wagtailmedia/media/add.html
+-rw-r--r--   0 dan        (502) staff       (20)     1068 2021-08-30 12:16:32.000000 wagtailmedia-0.9.0/src/wagtailmedia/templates/wagtailmedia/media/confirm_delete.html
+-rw-r--r--   0 dan        (502) staff       (20)     3154 2021-08-30 12:16:32.000000 wagtailmedia-0.9.0/src/wagtailmedia/templates/wagtailmedia/media/edit.html
+-rw-r--r--   0 dan        (502) staff       (20)     4084 2022-01-23 22:28:34.000000 wagtailmedia-0.9.0/src/wagtailmedia/templates/wagtailmedia/media/index.html
+-rw-r--r--   0 dan        (502) staff       (20)     2210 2021-08-30 12:16:32.000000 wagtailmedia-0.9.0/src/wagtailmedia/templates/wagtailmedia/media/list.html
+-rw-r--r--   0 dan        (502) staff       (20)     1433 2022-01-23 22:23:29.000000 wagtailmedia-0.9.0/src/wagtailmedia/templates/wagtailmedia/media/results.html
+-rw-r--r--   0 dan        (502) staff       (20)     1903 2021-08-30 12:16:32.000000 wagtailmedia-0.9.0/src/wagtailmedia/templates/wagtailmedia/media/usage.html
+drwxr-xr-x   0 dan        (502) staff       (20)        0 2022-02-22 11:14:00.644057 wagtailmedia-0.9.0/src/wagtailmedia/templates/wagtailmedia/permissions/
+drwxr-xr-x   0 dan        (502) staff       (20)        0 2022-02-22 11:14:00.678971 wagtailmedia-0.9.0/src/wagtailmedia/templates/wagtailmedia/permissions/includes/
+-rw-r--r--   0 dan        (502) staff       (20)      252 2021-08-30 12:16:32.000000 wagtailmedia-0.9.0/src/wagtailmedia/templates/wagtailmedia/permissions/includes/media_permissions_formset.html
+drwxr-xr-x   0 dan        (502) staff       (20)        0 2022-02-22 11:14:00.679573 wagtailmedia-0.9.0/src/wagtailmedia/templates/wagtailmedia/widgets/
+-rw-r--r--   0 dan        (502) staff       (20)      335 2021-09-05 11:47:43.000000 wagtailmedia-0.9.0/src/wagtailmedia/templates/wagtailmedia/widgets/media_chooser.html
+-rw-r--r--   0 dan        (502) staff       (20)      268 2021-08-30 12:16:32.000000 wagtailmedia-0.9.0/src/wagtailmedia/utils.py
+-rw-r--r--   0 dan        (502) staff       (20)       22 2022-02-22 11:11:53.000000 wagtailmedia-0.9.0/src/wagtailmedia/version.py
+drwxr-xr-x   0 dan        (502) staff       (20)        0 2022-02-22 11:14:00.681126 wagtailmedia-0.9.0/src/wagtailmedia/views/
+-rw-r--r--   0 dan        (502) staff       (20)        0 2021-08-30 12:16:32.000000 wagtailmedia-0.9.0/src/wagtailmedia/views/__init__.py
+-rw-r--r--   0 dan        (502) staff       (20)     7369 2022-01-23 22:28:34.000000 wagtailmedia-0.9.0/src/wagtailmedia/views/chooser.py
+-rw-r--r--   0 dan        (502) staff       (20)     8383 2022-01-23 22:28:34.000000 wagtailmedia-0.9.0/src/wagtailmedia/views/media.py
+-rw-r--r--   0 dan        (502) staff       (20)     3436 2022-02-16 09:30:59.000000 wagtailmedia-0.9.0/src/wagtailmedia/wagtail_hooks.py
+-rw-r--r--   0 dan        (502) staff       (20)     3916 2021-09-05 11:47:43.000000 wagtailmedia-0.9.0/src/wagtailmedia/widgets.py
+drwxr-xr-x   0 dan        (502) staff       (20)        0 2022-02-22 11:14:00.659375 wagtailmedia-0.9.0/src/wagtailmedia.egg-info/
+-rw-r--r--   0 dan        (502) staff       (20)    10588 2022-02-22 11:14:00.000000 wagtailmedia-0.9.0/src/wagtailmedia.egg-info/PKG-INFO
+-rw-r--r--   0 dan        (502) staff       (20)     2843 2022-02-22 11:14:00.000000 wagtailmedia-0.9.0/src/wagtailmedia.egg-info/SOURCES.txt
+-rw-r--r--   0 dan        (502) staff       (20)        1 2022-02-22 11:14:00.000000 wagtailmedia-0.9.0/src/wagtailmedia.egg-info/dependency_links.txt
+-rw-r--r--   0 dan        (502) staff       (20)        1 2022-01-23 11:13:58.000000 wagtailmedia-0.9.0/src/wagtailmedia.egg-info/not-zip-safe
+-rw-r--r--   0 dan        (502) staff       (20)       63 2022-02-22 11:14:00.000000 wagtailmedia-0.9.0/src/wagtailmedia.egg-info/requires.txt
+-rw-r--r--   0 dan        (502) staff       (20)       13 2022-02-22 11:14:00.000000 wagtailmedia-0.9.0/src/wagtailmedia.egg-info/top_level.txt
```

### Comparing `wagtailmedia-0.8.0/.editorconfig` & `wagtailmedia-0.9.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `wagtailmedia-0.8.0/CHANGELOG.md` & `wagtailmedia-0.9.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,24 @@
 
 # Changelog
 
 ## Unreleased
 -
 
+## [0.9.0] - 2022-02-22
+
+### Added
+- Wagtail 2.15 support ([#143](https://github.com/torchbox/wagtailmedia/pull/143)). Thanks @gasman
+- Ukrainian translation ([#145](https://github.com/torchbox/wagtailmedia/pull/145)). Thanks [@yuriifabirovskyi](https://github.com/yuriifabirovskyi)
+- Wagtail 2.16 and Django 4.0 support
+- Note about `collectstatic` in installation notes. Thanks [@G-kodes](https://github.com/G-kodes)
+
+### Fixed
+- Import issues due to module-level call to `get_media_base_form()` ([#148](https://github.com/torchbox/wagtailmedia/pull/148)). Thanks [@jsma](https://github.com/jsma)
+
 ## [0.8.0] - 2021-09-11
 
 - Updated test targets to include Wagtail 2.14
 - Changed the chooser uploader forms to use correctly instantiated forms ([#135](https://github.com/torchbox/wagtailmedia/pull/135))
 - Fixed the media chooser block compatibility with Wagtail 2.13 ([#136](https://github.com/torchbox/wagtailmedia/pull/136). Thanks [@efes](https://github.com/ephes))
 - Added tag-based filters ([#132](https://github.com/torchbox/wagtailmedia/pull/132). Thanks [@th3hamm0r](https://github.com/th3hamm0r))
 - Added `default_auto_field` for Django 3.2+ ([#134](https://github.com/torchbox/wagtailmedia/pull/134). Thanks [@hyperstown](https://github.com/hyperstown))
@@ -87,15 +98,15 @@
 ### Added
 
 - Support Wagtail 2.4 & 2.5 ([#43](https://github.com/torchbox/wagtailmedia/pull/43)). Thanks to [@DanSGraham](https://github.com/DanSGraham), [@evanwinter](https://github.com/evanwinter), [@kaduuuken](https://github.com/kaduuuken), [@pahacofome](https://github.com/pahacofome), [@kaedroho](https://github.com/kaedroho), [@thibaudcolas](https://github.com/thibaudcolas) for submitting various issues & PRs for this 🎉.
 - In CI, unit tests now run against combinations of Python 3.5, 3.6, 3.7, Django 1.11, 2.0, 2.1, 2.2, Wagtail 2.2, 2.3, 2.4, 2.5. ([#43](https://github.com/torchbox/wagtailmedia/pull/43), thanks to [@kaedroho](https://github.com/kaedroho)).
 
 ### Changed
 
-- Thanks to the [Wagtail 2.2 chooser API upgrade](https://docs.wagtail.io/en/v2.4/releases/2.2.html?highlight=render_modal_workflow#javascript-templates-in-modal-workflows-are-deprecated), it should now be possible to use `wagtailmedia` with a Content Security Policy without [`unsafe-eval`](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Content-Security-Policy/script-src) ([#43](https://github.com/torchbox/wagtailmedia/pull/43)).
+- Thanks to the [Wagtail 2.2 chooser API upgrade](https://docs.wagtail.org/en/v2.4/releases/2.2.html?highlight=render_modal_workflow#javascript-templates-in-modal-workflows-are-deprecated), it should now be possible to use `wagtailmedia` with a Content Security Policy without [`unsafe-eval`](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Content-Security-Policy/script-src) ([#43](https://github.com/torchbox/wagtailmedia/pull/43)).
 
 ### Removed
 
 - Remove support for Wagtail 2.1, 2.0, and below. For compatibility with Wagtail 2.1 and 2.0, use the [v0.2.0 release](https://pypi.org/project/wagtailmedia/0.2.0/).
 
 ## [0.2.0] - 2018-05-24
 
@@ -128,14 +139,15 @@
 
 ## [0.1.1] - 2016-05-26
 
 Initial release
 
 ---
 
+[0.8.0]: https://github.com/torchbox/wagtailmedia/releases/tag/v0.9.0
 [0.8.0]: https://github.com/torchbox/wagtailmedia/releases/tag/v0.8.0
 [0.7.1]: https://github.com/torchbox/wagtailmedia/releases/tag/v0.7.1
 [0.7.0]: https://github.com/torchbox/wagtailmedia/releases/tag/v0.7.0
 [0.6.0]: https://github.com/torchbox/wagtailmedia/releases/tag/v0.6.0
 [0.5.0]: https://github.com/torchbox/wagtailmedia/releases/tag/v0.5.0
 [0.4.0]: https://github.com/torchbox/wagtailmedia/releases/tag/v0.4.0
 [0.3.1]: https://github.com/torchbox/wagtailmedia/releases/tag/v0.3.1
```

### Comparing `wagtailmedia-0.8.0/LICENSE` & `wagtailmedia-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtailmedia-0.8.0/PKG-INFO` & `wagtailmedia-0.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtailmedia
-Version: 0.8.0
+Version: 0.9.0
 Summary: A module for Wagtail that provides functionality similar to wagtail.documents module, but for audio and video files.
 Home-page: https://github.com/torchbox/wagtailmedia
 Author: Mikalai Radchuk
 Author-email: hello@torchbox.com
 Maintainer: Dan Braghis
 Maintainer-email: dan.braghis@torchbox.com
 License: BSD
@@ -14,21 +14,19 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 2
 Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
@@ -42,36 +40,36 @@
 
 Install using pip:
 
 ```sh
 pip install wagtailmedia
 ```
 
-`wagtailmedia` is compatible with Wagtail 2.7 and above. Check out older releases for compatibility with older versions of Wagtail.
+`wagtailmedia` is compatible with Wagtail 2.11 and above. Check out older releases for compatibility with older versions of Wagtail.
 
 ### Settings
 
 In your settings file, add `wagtailmedia` to `INSTALLED_APPS`:
 
 ```python
 INSTALLED_APPS = [
     # ...
-    'wagtailmedia',
+    "wagtailmedia",
     # ...
 ]
 ```
 
 All wagtailmedia settings are defined in a single `WAGTAILMEDIA` dictionary in your settings file:
 
 ```python
 # settings.py
 
 WAGTAILMEDIA = {
     "MEDIA_MODEL": "",  # string, dotted-notation. Defaults to "wagtailmedia.Media"
-    "MEDIA_FORM_BASE": "",   # strind, dotted-notation. Defaults to an empty string
+    "MEDIA_FORM_BASE": "",  # string, dotted-notation. Defaults to an empty string
     "AUDIO_EXTENSIONS": [],  # list of extensions
     "VIDEO_EXTENSIONS": [],  # list of extensions
 }
 ```
 
 `AUDIO_EXTENSIONS` defaults to "aac", "aiff", "flac", "m4a", "m4b", "mp3", "ogg" and "wav".
 `VIDEO_EXTENSIONS` defaults to "avi", "h264", "m4v", "mkv", "mov", "mp4", "mpeg", "mpg", "ogv" and "webm".
@@ -91,15 +89,18 @@
 ```
 
 Note that this only works in development mode (`DEBUG = True`);
 in production, you will need to configure your web server to serve files from `MEDIA_ROOT`.
 For further details, see the Django documentation: [Serving files uploaded by a user during development](https://docs.djangoproject.com/en/stable/howto/static-files/#serving-files-uploaded-by-a-user-during-development)
 and [Deploying static files](https://docs.djangoproject.com/en/stable/howto/static-files/deployment/).
 
-With this configuration in place, you are ready to run `./manage.py migrate` to create the database tables used by wagtailmedia.
+With this configuration in place, you are ready to run `./manage.py migrate` to create the database tables used by `wagtailmedia`.
+
+`wagtailmedia` loads additional assets for the chooser panel interface.
+Run `./manage.py collectstatic` after the migrations step to collect all the required assets.
 
 ### Custom `Media` model
 
 The `Media` model can be customised. To do this, you need
 to add a new model to your project that inherits from `wagtailmedia.models.AbstractMedia`.
 
 Then set the `MEDIA_MODEL` attribute in the `WAGTAILMEDIA` settings dictionary to point to it:
@@ -131,15 +132,16 @@
 Called when rendering the media chooser view, to allow the media listing QuerySet to be customised.
 The callable passed into the hook will receive the current media QuerySet and the request object,
 and must return a Media QuerySet (either the original one, or a new one).
 
 ```python
 from wagtail.core import hooks
 
-@hooks.register('construct_media_chooser_queryset')
+
+@hooks.register("construct_media_chooser_queryset")
 def show_my_uploaded_media_only(media, request):
     # Only show uploaded media
     media = media.filter(uploaded_by_user=request.user)
 
     return media
 ```
 
@@ -160,26 +162,26 @@
 
 
 class BlogPageWithMedia(Page):
     author = models.CharField(max_length=255)
     date = models.DateField("Post date")
     body = RichTextField(blank=False)
     featured_media = models.ForeignKey(
-        'wagtailmedia.Media',
+        "wagtailmedia.Media",
         null=True,
         blank=True,
         on_delete=models.SET_NULL,
-        related_name='+'
+        related_name="+",
     )
 
     content_panels = Page.content_panels + [
-        FieldPanel('author'),
-        FieldPanel('date'),
-        FieldPanel('body'),
-        MediaChooserPanel('featured_media'),
+        FieldPanel("author"),
+        FieldPanel("date"),
+        FieldPanel("body"),
+        MediaChooserPanel("featured_media"),
     ]
 ```
 
 The `MediaChooserPanel` accepts the `media_type` keyword argument (kwarg) to limit the types of media that can be chosen or uploaded.
 At the moment only "audio" (`MediaChooserPanel(media_type="audio")`) and "video" (`MediaChooserPanel(media_type="audio")`) are supported,
 and any other type will make the chooser behave as if it did not get any kwarg.
 
@@ -208,72 +210,78 @@
 
 from wagtailmedia.blocks import AbstractMediaChooserBlock
 
 
 class TestMediaBlock(AbstractMediaChooserBlock):
     def render_basic(self, value, context=None):
         if not value:
-            return ''
+            return ""
 
-        if value.type == 'video':
-            player_code = '''
+        if value.type == "video":
+            player_code = """
             <div>
                 <video width="320" height="240" controls>
                     {0}
                     Your browser does not support the video tag.
                 </video>
             </div>
-            '''
+            """
         else:
-            player_code = '''
+            player_code = """
             <div>
                 <audio controls>
                     {0}
                     Your browser does not support the audio element.
                 </audio>
             </div>
-            '''
+            """
 
-        return format_html(player_code, format_html_join(
-            '\n', "<source{0}>",
-            [[flatatt(s)] for s in value.sources]
-        ))
+        return format_html(
+            player_code,
+            format_html_join(
+                "\n", "<source{0}>", [[flatatt(s)] for s in value.sources]
+            ),
+        )
 
 
 class BlogPage(Page):
     author = models.CharField(max_length=255)
     date = models.DateField("Post date")
-    body = StreamField([
-        ('heading', blocks.CharBlock(classname="full title", icon='title')),
-        ('paragraph', blocks.RichTextBlock(icon='pilcrow')),
-        ('media', TestMediaBlock(icon='media')),
-    ])
+    body = StreamField(
+        [
+            ("heading", blocks.CharBlock(classname="full title", icon="title")),
+            ("paragraph", blocks.RichTextBlock(icon="pilcrow")),
+            ("media", TestMediaBlock(icon="media")),
+        ]
+    )
 
     content_panels = Page.content_panels + [
-        FieldPanel('author'),
-        FieldPanel('date'),
-        StreamFieldPanel('body'),
+        FieldPanel("author"),
+        FieldPanel("date"),
+        StreamFieldPanel("body"),
     ]
 ```
 
 You can also use audio or video-specific choosers:
 
 ```python
 # ...
 from wagtailmedia.blocks import AudioChooserBlock, VideoChooserBlock
 
 
 class BlogPage(Page):
     # ...
 
-    body = StreamField([
-        # ... other block definitions
-        ('audio', AudioChooserBlock(icon='media')),
-        ('video', VideoChooserBlock(icon='media')),
-    ])
+    body = StreamField(
+        [
+            # ... other block definitions
+            ("audio", AudioChooserBlock(icon="media")),
+            ("video", VideoChooserBlock(icon="media")),
+        ]
+    )
 ```
 
 ## Translations
 
 wagtailmedia has translations in French and Chinese. More translations welcome!
 
 ## Contributing
```

### Comparing `wagtailmedia-0.8.0/README.md` & `wagtailmedia-0.9.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -7,36 +7,36 @@
 
 Install using pip:
 
 ```sh
 pip install wagtailmedia
 ```
 
-`wagtailmedia` is compatible with Wagtail 2.7 and above. Check out older releases for compatibility with older versions of Wagtail.
+`wagtailmedia` is compatible with Wagtail 2.11 and above. Check out older releases for compatibility with older versions of Wagtail.
 
 ### Settings
 
 In your settings file, add `wagtailmedia` to `INSTALLED_APPS`:
 
 ```python
 INSTALLED_APPS = [
     # ...
-    'wagtailmedia',
+    "wagtailmedia",
     # ...
 ]
 ```
 
 All wagtailmedia settings are defined in a single `WAGTAILMEDIA` dictionary in your settings file:
 
 ```python
 # settings.py
 
 WAGTAILMEDIA = {
     "MEDIA_MODEL": "",  # string, dotted-notation. Defaults to "wagtailmedia.Media"
-    "MEDIA_FORM_BASE": "",   # strind, dotted-notation. Defaults to an empty string
+    "MEDIA_FORM_BASE": "",  # string, dotted-notation. Defaults to an empty string
     "AUDIO_EXTENSIONS": [],  # list of extensions
     "VIDEO_EXTENSIONS": [],  # list of extensions
 }
 ```
 
 `AUDIO_EXTENSIONS` defaults to "aac", "aiff", "flac", "m4a", "m4b", "mp3", "ogg" and "wav".
 `VIDEO_EXTENSIONS` defaults to "avi", "h264", "m4v", "mkv", "mov", "mp4", "mpeg", "mpg", "ogv" and "webm".
@@ -56,15 +56,18 @@
 ```
 
 Note that this only works in development mode (`DEBUG = True`);
 in production, you will need to configure your web server to serve files from `MEDIA_ROOT`.
 For further details, see the Django documentation: [Serving files uploaded by a user during development](https://docs.djangoproject.com/en/stable/howto/static-files/#serving-files-uploaded-by-a-user-during-development)
 and [Deploying static files](https://docs.djangoproject.com/en/stable/howto/static-files/deployment/).
 
-With this configuration in place, you are ready to run `./manage.py migrate` to create the database tables used by wagtailmedia.
+With this configuration in place, you are ready to run `./manage.py migrate` to create the database tables used by `wagtailmedia`.
+
+`wagtailmedia` loads additional assets for the chooser panel interface.
+Run `./manage.py collectstatic` after the migrations step to collect all the required assets.
 
 ### Custom `Media` model
 
 The `Media` model can be customised. To do this, you need
 to add a new model to your project that inherits from `wagtailmedia.models.AbstractMedia`.
 
 Then set the `MEDIA_MODEL` attribute in the `WAGTAILMEDIA` settings dictionary to point to it:
@@ -96,15 +99,16 @@
 Called when rendering the media chooser view, to allow the media listing QuerySet to be customised.
 The callable passed into the hook will receive the current media QuerySet and the request object,
 and must return a Media QuerySet (either the original one, or a new one).
 
 ```python
 from wagtail.core import hooks
 
-@hooks.register('construct_media_chooser_queryset')
+
+@hooks.register("construct_media_chooser_queryset")
 def show_my_uploaded_media_only(media, request):
     # Only show uploaded media
     media = media.filter(uploaded_by_user=request.user)
 
     return media
 ```
 
@@ -125,26 +129,26 @@
 
 
 class BlogPageWithMedia(Page):
     author = models.CharField(max_length=255)
     date = models.DateField("Post date")
     body = RichTextField(blank=False)
     featured_media = models.ForeignKey(
-        'wagtailmedia.Media',
+        "wagtailmedia.Media",
         null=True,
         blank=True,
         on_delete=models.SET_NULL,
-        related_name='+'
+        related_name="+",
     )
 
     content_panels = Page.content_panels + [
-        FieldPanel('author'),
-        FieldPanel('date'),
-        FieldPanel('body'),
-        MediaChooserPanel('featured_media'),
+        FieldPanel("author"),
+        FieldPanel("date"),
+        FieldPanel("body"),
+        MediaChooserPanel("featured_media"),
     ]
 ```
 
 The `MediaChooserPanel` accepts the `media_type` keyword argument (kwarg) to limit the types of media that can be chosen or uploaded.
 At the moment only "audio" (`MediaChooserPanel(media_type="audio")`) and "video" (`MediaChooserPanel(media_type="audio")`) are supported,
 and any other type will make the chooser behave as if it did not get any kwarg.
 
@@ -173,72 +177,78 @@
 
 from wagtailmedia.blocks import AbstractMediaChooserBlock
 
 
 class TestMediaBlock(AbstractMediaChooserBlock):
     def render_basic(self, value, context=None):
         if not value:
-            return ''
+            return ""
 
-        if value.type == 'video':
-            player_code = '''
+        if value.type == "video":
+            player_code = """
             <div>
                 <video width="320" height="240" controls>
                     {0}
                     Your browser does not support the video tag.
                 </video>
             </div>
-            '''
+            """
         else:
-            player_code = '''
+            player_code = """
             <div>
                 <audio controls>
                     {0}
                     Your browser does not support the audio element.
                 </audio>
             </div>
-            '''
+            """
 
-        return format_html(player_code, format_html_join(
-            '\n', "<source{0}>",
-            [[flatatt(s)] for s in value.sources]
-        ))
+        return format_html(
+            player_code,
+            format_html_join(
+                "\n", "<source{0}>", [[flatatt(s)] for s in value.sources]
+            ),
+        )
 
 
 class BlogPage(Page):
     author = models.CharField(max_length=255)
     date = models.DateField("Post date")
-    body = StreamField([
-        ('heading', blocks.CharBlock(classname="full title", icon='title')),
-        ('paragraph', blocks.RichTextBlock(icon='pilcrow')),
-        ('media', TestMediaBlock(icon='media')),
-    ])
+    body = StreamField(
+        [
+            ("heading", blocks.CharBlock(classname="full title", icon="title")),
+            ("paragraph", blocks.RichTextBlock(icon="pilcrow")),
+            ("media", TestMediaBlock(icon="media")),
+        ]
+    )
 
     content_panels = Page.content_panels + [
-        FieldPanel('author'),
-        FieldPanel('date'),
-        StreamFieldPanel('body'),
+        FieldPanel("author"),
+        FieldPanel("date"),
+        StreamFieldPanel("body"),
     ]
 ```
 
 You can also use audio or video-specific choosers:
 
 ```python
 # ...
 from wagtailmedia.blocks import AudioChooserBlock, VideoChooserBlock
 
 
 class BlogPage(Page):
     # ...
 
-    body = StreamField([
-        # ... other block definitions
-        ('audio', AudioChooserBlock(icon='media')),
-        ('video', VideoChooserBlock(icon='media')),
-    ])
+    body = StreamField(
+        [
+            # ... other block definitions
+            ("audio", AudioChooserBlock(icon="media")),
+            ("video", VideoChooserBlock(icon="media")),
+        ]
+    )
 ```
 
 ## Translations
 
 wagtailmedia has translations in French and Chinese. More translations welcome!
 
 ## Contributing
```

### Comparing `wagtailmedia-0.8.0/SPECIFICATION.md` & `wagtailmedia-0.9.0/SPECIFICATION.md`

 * *Files identical despite different names*

### Comparing `wagtailmedia-0.8.0/setup.cfg` & `wagtailmedia-0.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `wagtailmedia-0.8.0/setup.py` & `wagtailmedia-0.9.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 #!/usr/bin/env python
 
 import io
 
 from setuptools import find_packages, setup
 
-from src.wagtailmedia import __version__
-
 
 # Testing dependencies
 testing_extras = [
     # Required for running the tests
     "mock>=1.0.0",
     # For coverage and PEP8 linting
     "coverage>=3.7.0",
-    "tox==3.23.1",
+    "tox~=3.24",
 ]
 
+version = {}
+with io.open("src/wagtailmedia/version.py") as fp:
+    exec(fp.read(), version)
+
 with io.open("README.md", encoding="utf-8") as readme_file:
     long_description = readme_file.read()
 
 setup(
     name="wagtailmedia",
-    version=__version__,
+    version=version["__version__"],
     description="A module for Wagtail that provides functionality "
     "similar to wagtail.documents module, but for audio and video files.",
     author="Mikalai Radchuk",
     author_email="hello@torchbox.com",
     maintainer="Dan Braghis",
     maintainer_email="dan.braghis@torchbox.com",
     project_urls={
@@ -43,21 +45,19 @@
         "Development Status :: 4 - Beta",
         "Environment :: Web Environment",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Framework :: Django",
         "Framework :: Django :: 2.2",
-        "Framework :: Django :: 3.1",
         "Framework :: Django :: 3.2",
         "Framework :: Wagtail",
         "Framework :: Wagtail :: 2",
         "Topic :: Internet :: WWW/HTTP :: Site Management",
     ],
     install_requires=[
         "wagtail>=2.11",
```

### Comparing `wagtailmedia-0.8.0/src/wagtailmedia/admin_urls.py` & `wagtailmedia-0.9.0/src/wagtailmedia/admin_urls.py`

 * *Files identical despite different names*

### Comparing `wagtailmedia-0.8.0/src/wagtailmedia/blocks.py` & `wagtailmedia-0.9.0/src/wagtailmedia/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtailmedia-0.8.0/src/wagtailmedia/edit_handlers.py` & `wagtailmedia-0.9.0/src/wagtailmedia/edit_handlers.py`

 * *Files identical despite different names*

### Comparing `wagtailmedia-0.8.0/src/wagtailmedia/forms.py` & `wagtailmedia-0.9.0/src/wagtailmedia/forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,29 +41,26 @@
     if base_form_override:
         base_form = import_string(base_form_override)
     else:
         base_form = BaseMediaForm
     return base_form
 
 
-media_base_form = get_media_base_form()
-
-
 def get_media_form(model):
     fields = model.admin_form_fields
     if "collection" not in fields:
         # force addition of the 'collection' field, because leaving it out can
         # cause dubious results when multiple collections exist (e.g adding the
         # media to the root collection where the user may not have permission) -
         # and when only one collection exists, it will get hidden anyway.
         fields = list(fields) + ["collection"]
 
     return modelform_factory(
         model,
-        form=media_base_form,
+        form=get_media_base_form(),
         fields=fields,
     )
 
 
 GroupMediaPermissionFormSet = collection_member_permission_formset_factory(
     Media,
     [
```

### Comparing `wagtailmedia-0.8.0/src/wagtailmedia/locale/de/LC_MESSAGES/django.mo` & `wagtailmedia-0.9.0/src/wagtailmedia/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtailmedia-0.8.0/src/wagtailmedia/locale/de/LC_MESSAGES/django.po` & `wagtailmedia-0.9.0/src/wagtailmedia/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtailmedia-0.8.0/src/wagtailmedia/locale/fr/LC_MESSAGES/django.mo` & `wagtailmedia-0.9.0/src/wagtailmedia/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtailmedia-0.8.0/src/wagtailmedia/locale/fr/LC_MESSAGES/django.po` & `wagtailmedia-0.9.0/src/wagtailmedia/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtailmedia-0.8.0/src/wagtailmedia/locale/zh_Hans/LC_MESSAGES/django.mo` & `wagtailmedia-0.9.0/src/wagtailmedia/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtailmedia-0.8.0/src/wagtailmedia/locale/zh_Hans/LC_MESSAGES/django.po` & `wagtailmedia-0.9.0/src/wagtailmedia/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtailmedia-0.8.0/src/wagtailmedia/migrations/0001_initial.py` & `wagtailmedia-0.9.0/src/wagtailmedia/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtailmedia-0.8.0/src/wagtailmedia/migrations/0002_initial_data.py` & `wagtailmedia-0.9.0/src/wagtailmedia/migrations/0002_initial_data.py`

 * *Files identical despite different names*

### Comparing `wagtailmedia-0.8.0/src/wagtailmedia/migrations/0003_copy_media_permissions_to_collections.py` & `wagtailmedia-0.9.0/src/wagtailmedia/migrations/0003_copy_media_permissions_to_collections.py`

 * *Files identical despite different names*

### Comparing `wagtailmedia-0.8.0/src/wagtailmedia/migrations/0004_duration_optional_floatfield.py` & `wagtailmedia-0.9.0/src/wagtailmedia/migrations/0004_duration_optional_floatfield.py`

 * *Files identical despite different names*

### Comparing `wagtailmedia-0.8.0/src/wagtailmedia/models.py` & `wagtailmedia-0.9.0/src/wagtailmedia/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,15 @@
 
     tags = TaggableManager(help_text=None, blank=True, verbose_name=_("tags"))
 
     objects = MediaQuerySet.as_manager()
 
     search_fields = CollectionMember.search_fields + [
         index.SearchField("title", partial_match=True, boost=10),
+        index.FilterField("title"),
         index.RelatedFields(
             "tags",
             [
                 index.SearchField("name", partial_match=True, boost=10),
             ],
         ),
         index.FilterField("uploaded_by_user"),
```

### Comparing `wagtailmedia-0.8.0/src/wagtailmedia/settings.py` & `wagtailmedia-0.9.0/src/wagtailmedia/settings.py`

 * *Files identical despite different names*

### Comparing `wagtailmedia-0.8.0/src/wagtailmedia/signal_handlers.py` & `wagtailmedia-0.9.0/src/wagtailmedia/signal_handlers.py`

 * *Files identical despite different names*

### Comparing `wagtailmedia-0.8.0/src/wagtailmedia/static/wagtailmedia/js/media-chooser-modal.js` & `wagtailmedia-0.9.0/src/wagtailmedia/static/wagtailmedia/js/media-chooser-modal.js`

 * *Files identical despite different names*

### Comparing `wagtailmedia-0.8.0/src/wagtailmedia/static/wagtailmedia/js/media-chooser-telepath.js` & `wagtailmedia-0.9.0/src/wagtailmedia/static/wagtailmedia/js/media-chooser-telepath.js`

 * *Files identical despite different names*

### Comparing `wagtailmedia-0.8.0/src/wagtailmedia/static/wagtailmedia/js/media-chooser.js` & `wagtailmedia-0.9.0/src/wagtailmedia/static/wagtailmedia/js/media-chooser.js`

 * *Files identical despite different names*

### Comparing `wagtailmedia-0.8.0/src/wagtailmedia/templates/wagtailmedia/chooser/chooser.html` & `wagtailmedia-0.9.0/src/wagtailmedia/templates/wagtailmedia/chooser/chooser.html`

 * *Files identical despite different names*

### Comparing `wagtailmedia-0.8.0/src/wagtailmedia/templates/wagtailmedia/chooser/results.html` & `wagtailmedia-0.9.0/src/wagtailmedia/templates/wagtailmedia/chooser/results.html`

 * *Files identical despite different names*

### Comparing `wagtailmedia-0.8.0/src/wagtailmedia/templates/wagtailmedia/media/add.html` & `wagtailmedia-0.9.0/src/wagtailmedia/templates/wagtailmedia/media/add.html`

 * *Files identical despite different names*

### Comparing `wagtailmedia-0.8.0/src/wagtailmedia/templates/wagtailmedia/media/confirm_delete.html` & `wagtailmedia-0.9.0/src/wagtailmedia/templates/wagtailmedia/media/confirm_delete.html`

 * *Files identical despite different names*

### Comparing `wagtailmedia-0.8.0/src/wagtailmedia/templates/wagtailmedia/media/edit.html` & `wagtailmedia-0.9.0/src/wagtailmedia/templates/wagtailmedia/media/edit.html`

 * *Files identical despite different names*

### Comparing `wagtailmedia-0.8.0/src/wagtailmedia/templates/wagtailmedia/media/index.html` & `wagtailmedia-0.9.0/src/wagtailmedia/templates/wagtailmedia/media/index.html`

 * *Files identical despite different names*

### Comparing `wagtailmedia-0.8.0/src/wagtailmedia/templates/wagtailmedia/media/list.html` & `wagtailmedia-0.9.0/src/wagtailmedia/templates/wagtailmedia/media/list.html`

 * *Files identical despite different names*

### Comparing `wagtailmedia-0.8.0/src/wagtailmedia/templates/wagtailmedia/media/results.html` & `wagtailmedia-0.9.0/src/wagtailmedia/templates/wagtailmedia/media/results.html`

 * *Files identical despite different names*

### Comparing `wagtailmedia-0.8.0/src/wagtailmedia/templates/wagtailmedia/media/usage.html` & `wagtailmedia-0.9.0/src/wagtailmedia/templates/wagtailmedia/media/usage.html`

 * *Files identical despite different names*

### Comparing `wagtailmedia-0.8.0/src/wagtailmedia/views/chooser.py` & `wagtailmedia-0.9.0/src/wagtailmedia/views/chooser.py`

 * *Files identical despite different names*

### Comparing `wagtailmedia-0.8.0/src/wagtailmedia/views/media.py` & `wagtailmedia-0.9.0/src/wagtailmedia/views/media.py`

 * *Files identical despite different names*

### Comparing `wagtailmedia-0.8.0/src/wagtailmedia/widgets.py` & `wagtailmedia-0.9.0/src/wagtailmedia/widgets.py`

 * *Files identical despite different names*

### Comparing `wagtailmedia-0.8.0/src/wagtailmedia.egg-info/PKG-INFO` & `wagtailmedia-0.9.0/src/wagtailmedia.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtailmedia
-Version: 0.8.0
+Version: 0.9.0
 Summary: A module for Wagtail that provides functionality similar to wagtail.documents module, but for audio and video files.
 Home-page: https://github.com/torchbox/wagtailmedia
 Author: Mikalai Radchuk
 Author-email: hello@torchbox.com
 Maintainer: Dan Braghis
 Maintainer-email: dan.braghis@torchbox.com
 License: BSD
@@ -14,21 +14,19 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 2
 Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
@@ -42,36 +40,36 @@
 
 Install using pip:
 
 ```sh
 pip install wagtailmedia
 ```
 
-`wagtailmedia` is compatible with Wagtail 2.7 and above. Check out older releases for compatibility with older versions of Wagtail.
+`wagtailmedia` is compatible with Wagtail 2.11 and above. Check out older releases for compatibility with older versions of Wagtail.
 
 ### Settings
 
 In your settings file, add `wagtailmedia` to `INSTALLED_APPS`:
 
 ```python
 INSTALLED_APPS = [
     # ...
-    'wagtailmedia',
+    "wagtailmedia",
     # ...
 ]
 ```
 
 All wagtailmedia settings are defined in a single `WAGTAILMEDIA` dictionary in your settings file:
 
 ```python
 # settings.py
 
 WAGTAILMEDIA = {
     "MEDIA_MODEL": "",  # string, dotted-notation. Defaults to "wagtailmedia.Media"
-    "MEDIA_FORM_BASE": "",   # strind, dotted-notation. Defaults to an empty string
+    "MEDIA_FORM_BASE": "",  # string, dotted-notation. Defaults to an empty string
     "AUDIO_EXTENSIONS": [],  # list of extensions
     "VIDEO_EXTENSIONS": [],  # list of extensions
 }
 ```
 
 `AUDIO_EXTENSIONS` defaults to "aac", "aiff", "flac", "m4a", "m4b", "mp3", "ogg" and "wav".
 `VIDEO_EXTENSIONS` defaults to "avi", "h264", "m4v", "mkv", "mov", "mp4", "mpeg", "mpg", "ogv" and "webm".
@@ -91,15 +89,18 @@
 ```
 
 Note that this only works in development mode (`DEBUG = True`);
 in production, you will need to configure your web server to serve files from `MEDIA_ROOT`.
 For further details, see the Django documentation: [Serving files uploaded by a user during development](https://docs.djangoproject.com/en/stable/howto/static-files/#serving-files-uploaded-by-a-user-during-development)
 and [Deploying static files](https://docs.djangoproject.com/en/stable/howto/static-files/deployment/).
 
-With this configuration in place, you are ready to run `./manage.py migrate` to create the database tables used by wagtailmedia.
+With this configuration in place, you are ready to run `./manage.py migrate` to create the database tables used by `wagtailmedia`.
+
+`wagtailmedia` loads additional assets for the chooser panel interface.
+Run `./manage.py collectstatic` after the migrations step to collect all the required assets.
 
 ### Custom `Media` model
 
 The `Media` model can be customised. To do this, you need
 to add a new model to your project that inherits from `wagtailmedia.models.AbstractMedia`.
 
 Then set the `MEDIA_MODEL` attribute in the `WAGTAILMEDIA` settings dictionary to point to it:
@@ -131,15 +132,16 @@
 Called when rendering the media chooser view, to allow the media listing QuerySet to be customised.
 The callable passed into the hook will receive the current media QuerySet and the request object,
 and must return a Media QuerySet (either the original one, or a new one).
 
 ```python
 from wagtail.core import hooks
 
-@hooks.register('construct_media_chooser_queryset')
+
+@hooks.register("construct_media_chooser_queryset")
 def show_my_uploaded_media_only(media, request):
     # Only show uploaded media
     media = media.filter(uploaded_by_user=request.user)
 
     return media
 ```
 
@@ -160,26 +162,26 @@
 
 
 class BlogPageWithMedia(Page):
     author = models.CharField(max_length=255)
     date = models.DateField("Post date")
     body = RichTextField(blank=False)
     featured_media = models.ForeignKey(
-        'wagtailmedia.Media',
+        "wagtailmedia.Media",
         null=True,
         blank=True,
         on_delete=models.SET_NULL,
-        related_name='+'
+        related_name="+",
     )
 
     content_panels = Page.content_panels + [
-        FieldPanel('author'),
-        FieldPanel('date'),
-        FieldPanel('body'),
-        MediaChooserPanel('featured_media'),
+        FieldPanel("author"),
+        FieldPanel("date"),
+        FieldPanel("body"),
+        MediaChooserPanel("featured_media"),
     ]
 ```
 
 The `MediaChooserPanel` accepts the `media_type` keyword argument (kwarg) to limit the types of media that can be chosen or uploaded.
 At the moment only "audio" (`MediaChooserPanel(media_type="audio")`) and "video" (`MediaChooserPanel(media_type="audio")`) are supported,
 and any other type will make the chooser behave as if it did not get any kwarg.
 
@@ -208,72 +210,78 @@
 
 from wagtailmedia.blocks import AbstractMediaChooserBlock
 
 
 class TestMediaBlock(AbstractMediaChooserBlock):
     def render_basic(self, value, context=None):
         if not value:
-            return ''
+            return ""
 
-        if value.type == 'video':
-            player_code = '''
+        if value.type == "video":
+            player_code = """
             <div>
                 <video width="320" height="240" controls>
                     {0}
                     Your browser does not support the video tag.
                 </video>
             </div>
-            '''
+            """
         else:
-            player_code = '''
+            player_code = """
             <div>
                 <audio controls>
                     {0}
                     Your browser does not support the audio element.
                 </audio>
             </div>
-            '''
+            """
 
-        return format_html(player_code, format_html_join(
-            '\n', "<source{0}>",
-            [[flatatt(s)] for s in value.sources]
-        ))
+        return format_html(
+            player_code,
+            format_html_join(
+                "\n", "<source{0}>", [[flatatt(s)] for s in value.sources]
+            ),
+        )
 
 
 class BlogPage(Page):
     author = models.CharField(max_length=255)
     date = models.DateField("Post date")
-    body = StreamField([
-        ('heading', blocks.CharBlock(classname="full title", icon='title')),
-        ('paragraph', blocks.RichTextBlock(icon='pilcrow')),
-        ('media', TestMediaBlock(icon='media')),
-    ])
+    body = StreamField(
+        [
+            ("heading", blocks.CharBlock(classname="full title", icon="title")),
+            ("paragraph", blocks.RichTextBlock(icon="pilcrow")),
+            ("media", TestMediaBlock(icon="media")),
+        ]
+    )
 
     content_panels = Page.content_panels + [
-        FieldPanel('author'),
-        FieldPanel('date'),
-        StreamFieldPanel('body'),
+        FieldPanel("author"),
+        FieldPanel("date"),
+        StreamFieldPanel("body"),
     ]
 ```
 
 You can also use audio or video-specific choosers:
 
 ```python
 # ...
 from wagtailmedia.blocks import AudioChooserBlock, VideoChooserBlock
 
 
 class BlogPage(Page):
     # ...
 
-    body = StreamField([
-        # ... other block definitions
-        ('audio', AudioChooserBlock(icon='media')),
-        ('video', VideoChooserBlock(icon='media')),
-    ])
+    body = StreamField(
+        [
+            # ... other block definitions
+            ("audio", AudioChooserBlock(icon="media")),
+            ("video", VideoChooserBlock(icon="media")),
+        ]
+    )
 ```
 
 ## Translations
 
 wagtailmedia has translations in French and Chinese. More translations welcome!
 
 ## Contributing
```

### Comparing `wagtailmedia-0.8.0/src/wagtailmedia.egg-info/SOURCES.txt` & `wagtailmedia-0.9.0/src/wagtailmedia.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -16,28 +16,30 @@
 src/wagtailmedia/edit_handlers.py
 src/wagtailmedia/forms.py
 src/wagtailmedia/models.py
 src/wagtailmedia/permissions.py
 src/wagtailmedia/settings.py
 src/wagtailmedia/signal_handlers.py
 src/wagtailmedia/utils.py
+src/wagtailmedia/version.py
 src/wagtailmedia/wagtail_hooks.py
 src/wagtailmedia/widgets.py
 src/wagtailmedia.egg-info/PKG-INFO
 src/wagtailmedia.egg-info/SOURCES.txt
 src/wagtailmedia.egg-info/dependency_links.txt
 src/wagtailmedia.egg-info/not-zip-safe
 src/wagtailmedia.egg-info/requires.txt
 src/wagtailmedia.egg-info/top_level.txt
-src/wagtailmedia/__pycache__/__init__.cpython-39.pyc
 src/wagtailmedia/locale/.gitkeep
 src/wagtailmedia/locale/de/LC_MESSAGES/django.mo
 src/wagtailmedia/locale/de/LC_MESSAGES/django.po
 src/wagtailmedia/locale/fr/LC_MESSAGES/django.mo
 src/wagtailmedia/locale/fr/LC_MESSAGES/django.po
+src/wagtailmedia/locale/uk/LC_MESSAGES/django.mo
+src/wagtailmedia/locale/uk/LC_MESSAGES/django.po
 src/wagtailmedia/locale/zh_Hans/LC_MESSAGES/django.mo
 src/wagtailmedia/locale/zh_Hans/LC_MESSAGES/django.po
 src/wagtailmedia/migrations/0001_initial.py
 src/wagtailmedia/migrations/0002_initial_data.py
 src/wagtailmedia/migrations/0003_copy_media_permissions_to_collections.py
 src/wagtailmedia/migrations/0004_duration_optional_floatfield.py
 src/wagtailmedia/migrations/__init__.py
```

