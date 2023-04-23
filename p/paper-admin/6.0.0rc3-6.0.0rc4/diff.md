# Comparing `tmp/paper-admin-6.0.0rc3.tar.gz` & `tmp/paper-admin-6.0.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paper-admin-6.0.0rc3.tar", last modified: Sat Apr 22 13:02:12 2023, max compression
+gzip compressed data, was "paper-admin-6.0.0rc4.tar", last modified: Sun Apr 23 14:55:17 2023, max compression
```

## Comparing `paper-admin-6.0.0rc3.tar` & `paper-admin-6.0.0rc4.tar`

### file list

```diff
@@ -1,310 +1,310 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.672077 paper-admin-6.0.0rc3/
--rw-r--r--   0 runner    (1001) docker     (123)     9932 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    19847 2023-04-22 13:02:12.672077 paper-admin-6.0.0rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18509 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.616074 paper-admin-6.0.0rc3/paper_admin/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.620074 paper-admin-6.0.0rc3/paper_admin/admin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14140 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/admin/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/admin/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/admin/renderers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/admin/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/admin/widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.608073 paper-admin-6.0.0rc3/paper_admin/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.608073 paper-admin-6.0.0rc3/paper_admin/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.620074 paper-admin-6.0.0rc3/paper_admin/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/locale/ru/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/locale/ru/LC_MESSAGES/djangojs.po
--rw-r--r--   0 runner    (1001) docker     (123)    18172 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/monkey_patch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.620074 paper-admin-6.0.0rc3/paper_admin/patches/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/patches/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.620074 paper-admin-6.0.0rc3/paper_admin/patches/dal/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/patches/dal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/patches/dal/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.608073 paper-admin-6.0.0rc3/paper_admin/patches/dal/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.620074 paper-admin-6.0.0rc3/paper_admin/patches/dal/static/autocomplete_light/
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/patches/dal/static/autocomplete_light/select2.js
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/patches/dal/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.624074 paper-admin-6.0.0rc3/paper_admin/patches/django/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/patches/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/patches/django/changelist.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/patches/django/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/patches/django/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/patches/django/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/patches/django/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.624074 paper-admin-6.0.0rc3/paper_admin/patches/django/prepopulate/
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/patches/django/prepopulate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/patches/django/prepopulate/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.624074 paper-admin-6.0.0rc3/paper_admin/patches/django/renderer/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/patches/django/renderer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/patches/django/renderer/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/patches/django/renderer/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/patches/django/renderer/widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/patches/django/sites.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.624074 paper-admin-6.0.0rc3/paper_admin/patches/django/sortable/
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/patches/django/sortable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/patches/django/sortable/changelist.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/patches/django/sortable/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/patches/django/sortable/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.624074 paper-admin-6.0.0rc3/paper_admin/patches/django/styles/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/patches/django/styles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/patches/django/styles/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.624074 paper-admin-6.0.0rc3/paper_admin/patches/django/tabs/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/patches/django/tabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/patches/django/tabs/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/patches/django/tabs/options.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/patches/django/tabs/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.624074 paper-admin-6.0.0rc3/paper_admin/patches/django/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/patches/django/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/patches/django/widgets/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/patches/django/widgets/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.628075 paper-admin-6.0.0rc3/paper_admin/patches/django_solo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/patches/django_solo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.608073 paper-admin-6.0.0rc3/paper_admin/patches/django_solo/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.608073 paper-admin-6.0.0rc3/paper_admin/patches/django_solo/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.628075 paper-admin-6.0.0rc3/paper_admin/patches/django_solo/templates/admin/solo/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/patches/django_solo/templates/admin/solo/change_form.html
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/patches/django_solo/templates/admin/solo/object_history.html
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/patches/formfield_defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.628075 paper-admin-6.0.0rc3/paper_admin/patches/logentry_admin/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/patches/logentry_admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/patches/logentry_admin/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/patches/logentry_admin/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.608073 paper-admin-6.0.0rc3/paper_admin/patches/logentry_admin/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.608073 paper-admin-6.0.0rc3/paper_admin/patches/logentry_admin/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.608073 paper-admin-6.0.0rc3/paper_admin/patches/logentry_admin/templates/admin/admin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.628075 paper-admin-6.0.0rc3/paper_admin/patches/logentry_admin/templates/admin/admin/logentry/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/patches/logentry_admin/templates/admin/admin/logentry/change_form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.628075 paper-admin-6.0.0rc3/paper_admin/patches/mptt/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/patches/mptt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/patches/mptt/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/patches/mptt/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.608073 paper-admin-6.0.0rc3/paper_admin/patches/mptt/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.628075 paper-admin-6.0.0rc3/paper_admin/patches/mptt/templates/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/patches/mptt/templates/admin/mptt_change_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/patches/mptt/templates/admin/mptt_change_list_results.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.628075 paper-admin-6.0.0rc3/paper_admin/patches/mptt/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/patches/mptt/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/patches/mptt/templatetags/paper_mptt_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.628075 paper-admin-6.0.0rc3/paper_admin/patches/post_office/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/patches/post_office/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/patches/post_office/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/patches/post_office/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.628075 paper-admin-6.0.0rc3/paper_admin/patches/tree_queries/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/patches/tree_queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/patches/tree_queries/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/patches/tree_queries/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/patches/tree_queries/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.612074 paper-admin-6.0.0rc3/paper_admin/patches/tree_queries/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.632075 paper-admin-6.0.0rc3/paper_admin/patches/tree_queries/templates/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/patches/tree_queries/templates/admin/tree_queries_change_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/patches/tree_queries/templates/admin/tree_queries_change_list_results.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.632075 paper-admin-6.0.0rc3/paper_admin/patches/tree_queries/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/patches/tree_queries/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/patches/tree_queries/templatetags/paper_tree_queries_list.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.612074 paper-admin-6.0.0rc3/paper_admin/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.612074 paper-admin-6.0.0rc3/paper_admin/static/admin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.632075 paper-admin-6.0.0rc3/paper_admin/static/admin/img/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/static/admin/img/icon-no.svg
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/static/admin/img/icon-yes.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.612074 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.644075 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/
--rw-r--r--   0 runner    (1001) docker     (123)   104881 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/app.802db2f5c8fabda7425c.js
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/app.802db2f5c8fabda7425c.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)   424992 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/app.802db2f5c8fabda7425c.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    81955 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/app.styles.779e472c0f96c40859ce.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.652076 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   139232 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/assets/Roboto.woff
--rw-r--r--   0 runner    (1001) docker     (123)    85728 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/assets/Roboto.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   141648 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/assets/RobotoBold.woff
--rw-r--r--   0 runner    (1001) docker     (123)    87220 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/assets/RobotoBold.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   161688 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/assets/RobotoBoldItalic.woff
--rw-r--r--   0 runner    (1001) docker     (123)   100928 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/assets/RobotoBoldItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   161288 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/assets/RobotoItalic.woff
--rw-r--r--   0 runner    (1001) docker     (123)   100120 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/assets/RobotoItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   137580 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/assets/RobotoLight.woff
--rw-r--r--   0 runner    (1001) docker     (123)    84520 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/assets/RobotoLight.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   165600 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/assets/RobotoLightItalic.woff
--rw-r--r--   0 runner    (1001) docker     (123)   101884 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/assets/RobotoLightItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   141032 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/assets/RobotoMedium.woff
--rw-r--r--   0 runner    (1001) docker     (123)    87464 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/assets/RobotoMedium.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   102368 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/assets/RobotoMediumItalic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    75068 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/assets/RobotoMediumItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   164360 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/assets/bootstrap-icons.woff
--rw-r--r--   0 runner    (1001) docker     (123)   121340 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/assets/bootstrap-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/assets/cross.svg
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/assets/default_favicon.png
--rw-r--r--   0 runner    (1001) docker     (123)   125964 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/assets/login_bg.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    47315 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/assets/menu_bg.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/assets/sortable.svg
--rw-r--r--   0 runner    (1001) docker     (123)    14958 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/changeform.e4e3561b61eb70807245.js
--rw-r--r--   0 runner    (1001) docker     (123)    72700 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/changeform.e4e3561b61eb70807245.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     9808 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/changelist.52229b67dbe6c9ce1e04.js
--rw-r--r--   0 runner    (1001) docker     (123)    42422 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/changelist.52229b67dbe6c9ce1e04.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-22 13:01:41.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/critical.11e9b5fdb3be652e8277.js
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-22 13:01:41.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/critical.11e9b5fdb3be652e8277.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    17816 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/npm.animejs.0610cb68d4b2f57e8eb8.js
--rw-r--r--   0 runner    (1001) docker     (123)    76238 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/npm.animejs.0610cb68d4b2f57e8eb8.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    73515 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/npm.bootstrap.59081124c9ac6decacff.js
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/npm.bootstrap.59081124c9ac6decacff.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)   259900 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/npm.bootstrap.59081124c9ac6decacff.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/npm.clockpicker.ac0071909818cc80b526.js
--rw-r--r--   0 runner    (1001) docker     (123)    37342 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/npm.clockpicker.ac0071909818cc80b526.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    40658 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/npm.core-js-pure.1bc2fd98475787ba1164.js
--rw-r--r--   0 runner    (1001) docker     (123)   214496 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/npm.core-js-pure.1bc2fd98475787ba1164.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    14600 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/npm.es-abstract.6d963e08114704c8e4d0.js
--rw-r--r--   0 runner    (1001) docker     (123)    56652 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/npm.es-abstract.6d963e08114704c8e4d0.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    96852 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/npm.flatpickr.365327b4124495649c9b.js
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/npm.flatpickr.365327b4124495649c9b.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)   324190 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/npm.flatpickr.365327b4124495649c9b.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    90183 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/npm.jquery.00f10cc5d0570a88ed04.js
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/npm.jquery.00f10cc5d0570a88ed04.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)   472782 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/npm.jquery.00f10cc5d0570a88ed04.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    21003 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/npm.popper.js.fa6168d95a0931432fac.js
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/npm.popper.js.fa6168d95a0931432fac.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)   124107 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/npm.popper.js.fa6168d95a0931432fac.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    77612 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/npm.select2.62432bf0675ff2408a99.js
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/npm.select2.62432bf0675ff2408a99.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)   267313 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/npm.select2.62432bf0675ff2408a99.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    35738 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/npm.sortablejs.73e6a37ecdb386aaa55f.js
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/npm.sortablejs.73e6a37ecdb386aaa55f.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)   175915 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/npm.sortablejs.73e6a37ecdb386aaa55f.js.map
--rw-r--r--   0 runner    (1001) docker     (123)   114414 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/npm.xregexp.98d0b833497d9fd631e9.js
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/npm.xregexp.98d0b833497d9fd631e9.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)   311042 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/npm.xregexp.98d0b833497d9fd631e9.js.map
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/popup.64e2e99cf69da31de176.js
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/popup.64e2e99cf69da31de176.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/runtime.f3efd79e7f1f7f906465.js
--rw-r--r--   0 runner    (1001) docker     (123)    18354 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/runtime.f3efd79e7f1f7f906465.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    76229 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/vendors.bootstrap-icons.329567d3425b7a67d749.css
--rw-r--r--   0 runner    (1001) docker     (123)   150039 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/vendors.bootstrap.6d9ce52aceafe8da2e8c.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.612074 paper-admin-6.0.0rc3/paper_admin/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.656076 paper-admin-6.0.0rc3/paper_admin/templates/admin/
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/admin/actions.html
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/admin/app_index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.612074 paper-admin-6.0.0rc3/paper_admin/templates/admin/auth/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.656076 paper-admin-6.0.0rc3/paper_admin/templates/admin/auth/user/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/admin/auth/user/add_form.html
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/admin/auth/user/change_password.html
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/admin/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     8367 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/admin/base_site.html
--rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/admin/change_form.html
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/admin/change_form_object_tools.html
--rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/admin/change_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/admin/change_list_object_tools.html
--rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/admin/change_list_results.html
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/admin/date_hierarchy.html
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/admin/delete_confirmation.html
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/admin/delete_selected_confirmation.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.660076 paper-admin-6.0.0rc3/paper_admin/templates/admin/edit_inline/
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/admin/edit_inline/_stacked_form.html
--rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/admin/edit_inline/_tabular_form.html
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/admin/edit_inline/stacked.html
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/admin/edit_inline/tabular.html
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/admin/filter.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.660076 paper-admin-6.0.0rc3/paper_admin/templates/admin/includes/
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/admin/includes/fieldset.html
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/admin/includes/object_delete_summary.html
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/admin/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/admin/invalid_setup.html
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/admin/login.html
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/admin/object_history.html
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/admin/pagination.html
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/admin/popup_response.html
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/admin/prepopulated_fields_js.html
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/admin/search_form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.660076 paper-admin-6.0.0rc3/paper_admin/templates/admin/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/admin/widgets/related_widget_wrapper.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.612074 paper-admin-6.0.0rc3/paper_admin/templates/auth/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.660076 paper-admin-6.0.0rc3/paper_admin/templates/auth/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/auth/widgets/read_only_password_hash.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.612074 paper-admin-6.0.0rc3/paper_admin/templates/django/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.612074 paper-admin-6.0.0rc3/paper_admin/templates/django/forms/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.664076 paper-admin-6.0.0rc3/paper_admin/templates/django/forms/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/django/forms/widgets/checkbox_custom.html
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/django/forms/widgets/clearable_file_input.html
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/django/forms/widgets/date.html
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/django/forms/widgets/datetime.html
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/django/forms/widgets/email.html
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/django/forms/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/django/forms/widgets/foreign_key_raw_id.html
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/django/forms/widgets/ip.html
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/django/forms/widgets/many_to_many_raw_id.html
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/django/forms/widgets/multiple_hidden.html
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/django/forms/widgets/multiple_input.html
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/django/forms/widgets/multiwidget.html
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/django/forms/widgets/number.html
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/django/forms/widgets/password.html
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/django/forms/widgets/radio_custom.html
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/django/forms/widgets/radio_option_custom.html
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/django/forms/widgets/select.html
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/django/forms/widgets/select_date.html
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/django/forms/widgets/select_multiple.html
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/django/forms/widgets/splitdatetime.html
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/django/forms/widgets/splithiddendatetime.html
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/django/forms/widgets/switch.html
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/django/forms/widgets/textarea.html
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/django/forms/widgets/time.html
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/django/forms/widgets/url.html
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/django/forms/widgets/uuid.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.664076 paper-admin-6.0.0rc3/paper_admin/templates/paper_admin/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-22 13:01:41.000000 paper-admin-6.0.0rc3/paper_admin/templates/paper_admin/app.critical.html
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-22 13:02:11.000000 paper-admin-6.0.0rc3/paper_admin/templates/paper_admin/app.head.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.668077 paper-admin-6.0.0rc3/paper_admin/templates/paper_admin/filters/
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/paper_admin/filters/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/paper_admin/filters/daterange.html
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/paper_admin/filters/hierarchy.html
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/paper_admin/filters/list.html
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/paper_admin/filters/radio.html
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/paper_admin/filters/select.html
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/paper_admin/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/paper_admin/header_buttons.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.668077 paper-admin-6.0.0rc3/paper_admin/templates/paper_admin/includes/
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/paper_admin/includes/admin_checkbox.html
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/paper_admin/includes/admin_field.html
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/paper_admin/includes/changelist_field.html
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/paper_admin/includes/changelist_tools.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.668077 paper-admin-6.0.0rc3/paper_admin/templates/paper_admin/menu/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/paper_admin/menu/divider.html
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/paper_admin/menu/group.html
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/paper_admin/menu/item.html
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/paper_admin/menu/submenu.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.668077 paper-admin-6.0.0rc3/paper_admin/templates/registration/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/registration/logged_out.html
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/registration/password_change_done.html
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/registration/password_change_form.html
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/registration/password_reset_complete.html
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/registration/password_reset_confirm.html
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/registration/password_reset_done.html
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/registration/password_reset_email.html
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/registration/password_reset_email_alt.html
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templates/registration/password_reset_form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.672077 paper-admin-6.0.0rc3/paper_admin/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templatetags/load_paper.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templatetags/paper_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templatetags/paper_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templatetags/paper_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templatetags/paper_modify.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templatetags/paper_paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/paper_admin/templatetags/paper_styles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:02:12.616074 paper-admin-6.0.0rc3/paper_admin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19847 2023-04-22 13:02:12.000000 paper-admin-6.0.0rc3/paper_admin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-04-22 13:02:12.000000 paper-admin-6.0.0rc3/paper_admin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 13:02:12.000000 paper-admin-6.0.0rc3/paper_admin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 13:02:12.000000 paper-admin-6.0.0rc3/paper_admin.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-22 13:02:12.000000 paper-admin-6.0.0rc3/paper_admin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-22 13:02:12.000000 paper-admin-6.0.0rc3/paper_admin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-04-22 13:02:12.672077 paper-admin-6.0.0rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-22 13:00:59.000000 paper-admin-6.0.0rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.921186 paper-admin-6.0.0rc4/
+-rw-r--r--   0 runner    (1001) docker     (123)     9932 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    19856 2023-04-23 14:55:17.921186 paper-admin-6.0.0rc4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18518 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.881186 paper-admin-6.0.0rc4/paper_admin/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.885186 paper-admin-6.0.0rc4/paper_admin/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14140 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/admin/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/admin/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/admin/renderers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/admin/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/admin/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.877186 paper-admin-6.0.0rc4/paper_admin/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.877186 paper-admin-6.0.0rc4/paper_admin/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.885186 paper-admin-6.0.0rc4/paper_admin/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/locale/ru/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/locale/ru/LC_MESSAGES/djangojs.po
+-rw-r--r--   0 runner    (1001) docker     (123)    18172 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/monkey_patch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.885186 paper-admin-6.0.0rc4/paper_admin/patches/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/patches/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.885186 paper-admin-6.0.0rc4/paper_admin/patches/dal/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/patches/dal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/patches/dal/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.877186 paper-admin-6.0.0rc4/paper_admin/patches/dal/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.885186 paper-admin-6.0.0rc4/paper_admin/patches/dal/static/autocomplete_light/
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/patches/dal/static/autocomplete_light/select2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/patches/dal/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.885186 paper-admin-6.0.0rc4/paper_admin/patches/django/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/patches/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/patches/django/changelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/patches/django/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/patches/django/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/patches/django/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/patches/django/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.885186 paper-admin-6.0.0rc4/paper_admin/patches/django/prepopulate/
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/patches/django/prepopulate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/patches/django/prepopulate/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.885186 paper-admin-6.0.0rc4/paper_admin/patches/django/renderer/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/patches/django/renderer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/patches/django/renderer/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/patches/django/renderer/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/patches/django/renderer/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/patches/django/sites.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.885186 paper-admin-6.0.0rc4/paper_admin/patches/django/sortable/
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/patches/django/sortable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/patches/django/sortable/changelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/patches/django/sortable/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/patches/django/sortable/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.885186 paper-admin-6.0.0rc4/paper_admin/patches/django/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/patches/django/styles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/patches/django/styles/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.885186 paper-admin-6.0.0rc4/paper_admin/patches/django/tabs/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/patches/django/tabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/patches/django/tabs/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/patches/django/tabs/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/patches/django/tabs/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.889186 paper-admin-6.0.0rc4/paper_admin/patches/django/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/patches/django/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/patches/django/widgets/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/patches/django/widgets/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.889186 paper-admin-6.0.0rc4/paper_admin/patches/django_solo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/patches/django_solo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.877186 paper-admin-6.0.0rc4/paper_admin/patches/django_solo/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.877186 paper-admin-6.0.0rc4/paper_admin/patches/django_solo/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.889186 paper-admin-6.0.0rc4/paper_admin/patches/django_solo/templates/admin/solo/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/patches/django_solo/templates/admin/solo/change_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/patches/django_solo/templates/admin/solo/object_history.html
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/patches/formfield_defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.889186 paper-admin-6.0.0rc4/paper_admin/patches/logentry_admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/patches/logentry_admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/patches/logentry_admin/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/patches/logentry_admin/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.877186 paper-admin-6.0.0rc4/paper_admin/patches/logentry_admin/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.877186 paper-admin-6.0.0rc4/paper_admin/patches/logentry_admin/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.877186 paper-admin-6.0.0rc4/paper_admin/patches/logentry_admin/templates/admin/admin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.889186 paper-admin-6.0.0rc4/paper_admin/patches/logentry_admin/templates/admin/admin/logentry/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/patches/logentry_admin/templates/admin/admin/logentry/change_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.889186 paper-admin-6.0.0rc4/paper_admin/patches/mptt/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/patches/mptt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/patches/mptt/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/patches/mptt/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.877186 paper-admin-6.0.0rc4/paper_admin/patches/mptt/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.889186 paper-admin-6.0.0rc4/paper_admin/patches/mptt/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/patches/mptt/templates/admin/mptt_change_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/patches/mptt/templates/admin/mptt_change_list_results.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.889186 paper-admin-6.0.0rc4/paper_admin/patches/mptt/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/patches/mptt/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/patches/mptt/templatetags/paper_mptt_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.889186 paper-admin-6.0.0rc4/paper_admin/patches/post_office/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/patches/post_office/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/patches/post_office/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/patches/post_office/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.889186 paper-admin-6.0.0rc4/paper_admin/patches/tree_queries/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/patches/tree_queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/patches/tree_queries/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/patches/tree_queries/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/patches/tree_queries/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.877186 paper-admin-6.0.0rc4/paper_admin/patches/tree_queries/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.889186 paper-admin-6.0.0rc4/paper_admin/patches/tree_queries/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/patches/tree_queries/templates/admin/tree_queries_change_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/patches/tree_queries/templates/admin/tree_queries_change_list_results.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.889186 paper-admin-6.0.0rc4/paper_admin/patches/tree_queries/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/patches/tree_queries/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/patches/tree_queries/templatetags/paper_tree_queries_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.877186 paper-admin-6.0.0rc4/paper_admin/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.877186 paper-admin-6.0.0rc4/paper_admin/static/admin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.889186 paper-admin-6.0.0rc4/paper_admin/static/admin/img/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/static/admin/img/icon-no.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/static/admin/img/icon-yes.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.877186 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.897186 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)   104881 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/app.802db2f5c8fabda7425c.js
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/app.802db2f5c8fabda7425c.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   424992 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/app.802db2f5c8fabda7425c.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    82039 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/app.styles.9ae55058e746fe5377c3.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.905186 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   139232 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/assets/Roboto.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    85728 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/assets/Roboto.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   141648 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/assets/RobotoBold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    87220 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/assets/RobotoBold.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   161688 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/assets/RobotoBoldItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   100928 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/assets/RobotoBoldItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   161288 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/assets/RobotoItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   100120 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/assets/RobotoItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   137580 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/assets/RobotoLight.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    84520 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/assets/RobotoLight.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   165600 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/assets/RobotoLightItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   101884 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/assets/RobotoLightItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   141032 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/assets/RobotoMedium.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    87464 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/assets/RobotoMedium.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   102368 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/assets/RobotoMediumItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    75068 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/assets/RobotoMediumItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   164360 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/assets/bootstrap-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   121340 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/assets/bootstrap-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/assets/cross.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/assets/default_favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)   125964 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/assets/login_bg.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    47315 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/assets/menu_bg.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/assets/sortable.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    14958 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/changeform.e4e3561b61eb70807245.js
+-rw-r--r--   0 runner    (1001) docker     (123)    72700 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/changeform.e4e3561b61eb70807245.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     9808 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/changelist.52229b67dbe6c9ce1e04.js
+-rw-r--r--   0 runner    (1001) docker     (123)    42422 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/changelist.52229b67dbe6c9ce1e04.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-23 14:54:54.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/critical.11e9b5fdb3be652e8277.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-23 14:54:54.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/critical.11e9b5fdb3be652e8277.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    17816 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/npm.animejs.0610cb68d4b2f57e8eb8.js
+-rw-r--r--   0 runner    (1001) docker     (123)    76238 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/npm.animejs.0610cb68d4b2f57e8eb8.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    73515 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/npm.bootstrap.59081124c9ac6decacff.js
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/npm.bootstrap.59081124c9ac6decacff.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   259900 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/npm.bootstrap.59081124c9ac6decacff.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/npm.clockpicker.ac0071909818cc80b526.js
+-rw-r--r--   0 runner    (1001) docker     (123)    37342 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/npm.clockpicker.ac0071909818cc80b526.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    40658 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/npm.core-js-pure.1bc2fd98475787ba1164.js
+-rw-r--r--   0 runner    (1001) docker     (123)   214496 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/npm.core-js-pure.1bc2fd98475787ba1164.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    14600 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/npm.es-abstract.6d963e08114704c8e4d0.js
+-rw-r--r--   0 runner    (1001) docker     (123)    56652 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/npm.es-abstract.6d963e08114704c8e4d0.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    96852 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/npm.flatpickr.365327b4124495649c9b.js
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/npm.flatpickr.365327b4124495649c9b.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   324190 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/npm.flatpickr.365327b4124495649c9b.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    90183 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/npm.jquery.00f10cc5d0570a88ed04.js
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/npm.jquery.00f10cc5d0570a88ed04.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   472782 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/npm.jquery.00f10cc5d0570a88ed04.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    21003 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/npm.popper.js.fa6168d95a0931432fac.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/npm.popper.js.fa6168d95a0931432fac.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   124107 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/npm.popper.js.fa6168d95a0931432fac.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    77612 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/npm.select2.62432bf0675ff2408a99.js
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/npm.select2.62432bf0675ff2408a99.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   267313 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/npm.select2.62432bf0675ff2408a99.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    35738 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/npm.sortablejs.73e6a37ecdb386aaa55f.js
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/npm.sortablejs.73e6a37ecdb386aaa55f.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   175915 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/npm.sortablejs.73e6a37ecdb386aaa55f.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)   114414 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/npm.xregexp.98d0b833497d9fd631e9.js
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/npm.xregexp.98d0b833497d9fd631e9.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   311042 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/npm.xregexp.98d0b833497d9fd631e9.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/popup.64e2e99cf69da31de176.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/popup.64e2e99cf69da31de176.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/runtime.f3efd79e7f1f7f906465.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18354 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/runtime.f3efd79e7f1f7f906465.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    76229 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/vendors.bootstrap-icons.329567d3425b7a67d749.css
+-rw-r--r--   0 runner    (1001) docker     (123)   150039 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/vendors.bootstrap.6d9ce52aceafe8da2e8c.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.881186 paper-admin-6.0.0rc4/paper_admin/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.909186 paper-admin-6.0.0rc4/paper_admin/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/admin/actions.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/admin/app_index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.881186 paper-admin-6.0.0rc4/paper_admin/templates/admin/auth/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.913186 paper-admin-6.0.0rc4/paper_admin/templates/admin/auth/user/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/admin/auth/user/add_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/admin/auth/user/change_password.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/admin/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8367 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/admin/base_site.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/admin/change_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/admin/change_form_object_tools.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/admin/change_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/admin/change_list_object_tools.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/admin/change_list_results.html
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/admin/date_hierarchy.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/admin/delete_confirmation.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/admin/delete_selected_confirmation.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.913186 paper-admin-6.0.0rc4/paper_admin/templates/admin/edit_inline/
+-rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/admin/edit_inline/_stacked_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/admin/edit_inline/_tabular_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/admin/edit_inline/stacked.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/admin/edit_inline/tabular.html
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/admin/filter.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.913186 paper-admin-6.0.0rc4/paper_admin/templates/admin/includes/
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/admin/includes/fieldset.html
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/admin/includes/object_delete_summary.html
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/admin/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/admin/invalid_setup.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/admin/login.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/admin/object_history.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/admin/pagination.html
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/admin/popup_response.html
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/admin/prepopulated_fields_js.html
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/admin/search_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.913186 paper-admin-6.0.0rc4/paper_admin/templates/admin/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/admin/widgets/related_widget_wrapper.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.881186 paper-admin-6.0.0rc4/paper_admin/templates/auth/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.913186 paper-admin-6.0.0rc4/paper_admin/templates/auth/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/auth/widgets/read_only_password_hash.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.881186 paper-admin-6.0.0rc4/paper_admin/templates/django/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.881186 paper-admin-6.0.0rc4/paper_admin/templates/django/forms/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.917186 paper-admin-6.0.0rc4/paper_admin/templates/django/forms/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/django/forms/widgets/checkbox_custom.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/django/forms/widgets/clearable_file_input.html
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/django/forms/widgets/date.html
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/django/forms/widgets/datetime.html
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/django/forms/widgets/email.html
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/django/forms/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/django/forms/widgets/foreign_key_raw_id.html
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/django/forms/widgets/ip.html
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/django/forms/widgets/many_to_many_raw_id.html
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/django/forms/widgets/multiple_hidden.html
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/django/forms/widgets/multiple_input.html
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/django/forms/widgets/multiwidget.html
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/django/forms/widgets/number.html
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/django/forms/widgets/password.html
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/django/forms/widgets/radio_custom.html
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/django/forms/widgets/radio_option_custom.html
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/django/forms/widgets/select.html
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/django/forms/widgets/select_date.html
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/django/forms/widgets/select_multiple.html
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/django/forms/widgets/splitdatetime.html
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/django/forms/widgets/splithiddendatetime.html
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/django/forms/widgets/switch.html
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/django/forms/widgets/textarea.html
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/django/forms/widgets/time.html
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/django/forms/widgets/url.html
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/django/forms/widgets/uuid.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.917186 paper-admin-6.0.0rc4/paper_admin/templates/paper_admin/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-23 14:54:54.000000 paper-admin-6.0.0rc4/paper_admin/templates/paper_admin/app.critical.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin/templates/paper_admin/app.head.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.917186 paper-admin-6.0.0rc4/paper_admin/templates/paper_admin/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/paper_admin/filters/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/paper_admin/filters/daterange.html
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/paper_admin/filters/hierarchy.html
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/paper_admin/filters/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/paper_admin/filters/radio.html
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/paper_admin/filters/select.html
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/paper_admin/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/paper_admin/header_buttons.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.917186 paper-admin-6.0.0rc4/paper_admin/templates/paper_admin/includes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/paper_admin/includes/admin_checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/paper_admin/includes/admin_field.html
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/paper_admin/includes/changelist_field.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/paper_admin/includes/changelist_tools.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.917186 paper-admin-6.0.0rc4/paper_admin/templates/paper_admin/menu/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/paper_admin/menu/divider.html
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/paper_admin/menu/group.html
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/paper_admin/menu/item.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/paper_admin/menu/submenu.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.921186 paper-admin-6.0.0rc4/paper_admin/templates/registration/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/registration/logged_out.html
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/registration/password_change_done.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/registration/password_change_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/registration/password_reset_complete.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/registration/password_reset_confirm.html
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/registration/password_reset_done.html
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/registration/password_reset_email.html
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/registration/password_reset_email_alt.html
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templates/registration/password_reset_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.921186 paper-admin-6.0.0rc4/paper_admin/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templatetags/load_paper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templatetags/paper_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templatetags/paper_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templatetags/paper_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templatetags/paper_modify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templatetags/paper_paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/paper_admin/templatetags/paper_styles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:55:17.881186 paper-admin-6.0.0rc4/paper_admin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19856 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-23 14:55:17.000000 paper-admin-6.0.0rc4/paper_admin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-04-23 14:55:17.921186 paper-admin-6.0.0rc4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-23 14:54:27.000000 paper-admin-6.0.0rc4/setup.py
```

### Comparing `paper-admin-6.0.0rc3/CHANGELOG.md` & `paper-admin-6.0.0rc4/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/CONTRIBUTING.md` & `paper-admin-6.0.0rc4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/LICENSE` & `paper-admin-6.0.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/PKG-INFO` & `paper-admin-6.0.0rc4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-admin
-Version: 6.0.0rc3
+Version: 6.0.0rc4
 Summary: Custom Django admin interface.
 Home-page: https://github.com/dldevinc/paper-admin
 Author: Mihail Mishakin
 Author-email: x896321475@gmail.com
 Maintainer: Mihail Mishakin
 Maintainer-email: x896321475@gmail.com
 License: BSD license
@@ -52,15 +52,15 @@
 -   [Patches](#Patches)
 -   [Badge](#Badge)
 -   [Admin menu](#Admin-menu)
 -   [Reorderable drag-and-drop lists](#Reorderable-drag-and-drop-lists)
 -   [Form tabs](#Form-tabs)
 -   [HierarchyFilter](#HierarchyFilter)
 -   [Stylization](#Stylization)
-    -   [Fieldset](#Fieldset)
+    -   [Fieldsets](#Fieldsets)
     -   [Table rows](#Table-rows)
     -   [Inline forms](#Inline-forms)
 -   [Settings](#Settings)
 -   [Additional References](#Additional-References)
 
 ## Installation
 
@@ -561,15 +561,39 @@
 
 Result:
 
 ![image](https://user-images.githubusercontent.com/6928240/229168174-a9c32ec8-f87a-4ec9-a875-105eeae61f06.png)
 
 ## Stylization
 
-### Fieldset
+### Table rows
+
+You can use the `get_row_classes` method of the `ModelAdmin`
+class to add custom classes to the rows in the list view.
+
+```python
+from django.contrib import admin
+from .models import Category
+
+
+@admin.register(Category)
+class CategoryAdmin(admin.ModelAdmin):
+
+    def get_row_classes(self, request, obj):
+        if obj.status == "success":
+            return ["table-success"]
+        elif obj.status == "failed":
+            return ["table-danger"]
+        return []
+```
+
+![image](https://user-images.githubusercontent.com/6928240/233795075-d0f85cc2-d34a-43a9-b393-20cd81f96d99.png)
+
+
+### Fieldsets
 
 Django [provides](https://docs.djangoproject.com/en/4.0/ref/contrib/admin/#django.contrib.admin.ModelAdmin.fieldsets)
 a way to add a custom CSS classes to the fieldsets in the admin interface.
 
 To use this feature, specify the `classes` parameter in the `ModelAdmin.fieldsets`
 attribute:
 
@@ -600,38 +624,15 @@
             "fields": (
                 # ...
             )
         }),
     )
 ```
 
-![](https://user-images.githubusercontent.com/6928240/125337870-8f91e180-e360-11eb-9b19-7f903ab30464.png)
-
-### Table rows
-
-You can use the `get_row_classes` method of the `ModelAdmin`
-class to add custom classes to the rows in the list view.
-
-```python
-from django.contrib import admin
-from .models import Category
-
-
-@admin.register(Category)
-class CategoryAdmin(admin.ModelAdmin):
-
-    def get_row_classes(self, request, obj):
-        if obj.status == "success":
-            return ["table-success"]
-        elif obj.status == "failed":
-            return ["table-danger"]
-        return []
-```
-
-![image](https://user-images.githubusercontent.com/6928240/225705910-4f1309e1-93e3-456a-b9d0-f01748faec7b.png)
+![image](https://user-images.githubusercontent.com/6928240/233795448-17d2fa5c-739a-4751-8266-b4b4e879b1c8.png)
 
 ### Inline forms
 
 You can use the `get_form_classes` method of the `ModelAdmin` class
 to add custom classes to the inline forms:
 
 ```python
@@ -652,16 +653,16 @@
         if obj.status == "success":
             return ["table-success"]
         elif obj.status == "failed":
             return ["table-danger"]
         return []
 ```
 
-![image](https://user-images.githubusercontent.com/6928240/225713947-34e29927-b629-4b9a-bf6e-56ec8948de7e.png)
-![image](https://user-images.githubusercontent.com/6928240/225714321-87a33c52-65d8-4175-a118-cb751b92ebb8.png)
+![image](https://user-images.githubusercontent.com/6928240/233794982-1ca7248a-dc54-48c4-aea2-44d0d973d083.png)
+![image](https://user-images.githubusercontent.com/6928240/233795183-c056b82e-8b01-4f7d-9c09-65c0becbdc33.png)
 
 ## Settings
 
 `PAPER_FAVICON`<br>
 The path to the favicon for the admin interface.<br>
 Default: `"paper_admin/dist/assets/default_favicon.png"`
```

### Comparing `paper-admin-6.0.0rc3/README.md` & `paper-admin-6.0.0rc4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 -   [Patches](#Patches)
 -   [Badge](#Badge)
 -   [Admin menu](#Admin-menu)
 -   [Reorderable drag-and-drop lists](#Reorderable-drag-and-drop-lists)
 -   [Form tabs](#Form-tabs)
 -   [HierarchyFilter](#HierarchyFilter)
 -   [Stylization](#Stylization)
-    -   [Fieldset](#Fieldset)
+    -   [Fieldsets](#Fieldsets)
     -   [Table rows](#Table-rows)
     -   [Inline forms](#Inline-forms)
 -   [Settings](#Settings)
 -   [Additional References](#Additional-References)
 
 ## Installation
 
@@ -526,15 +526,39 @@
 
 Result:
 
 ![image](https://user-images.githubusercontent.com/6928240/229168174-a9c32ec8-f87a-4ec9-a875-105eeae61f06.png)
 
 ## Stylization
 
-### Fieldset
+### Table rows
+
+You can use the `get_row_classes` method of the `ModelAdmin`
+class to add custom classes to the rows in the list view.
+
+```python
+from django.contrib import admin
+from .models import Category
+
+
+@admin.register(Category)
+class CategoryAdmin(admin.ModelAdmin):
+
+    def get_row_classes(self, request, obj):
+        if obj.status == "success":
+            return ["table-success"]
+        elif obj.status == "failed":
+            return ["table-danger"]
+        return []
+```
+
+![image](https://user-images.githubusercontent.com/6928240/233795075-d0f85cc2-d34a-43a9-b393-20cd81f96d99.png)
+
+
+### Fieldsets
 
 Django [provides](https://docs.djangoproject.com/en/4.0/ref/contrib/admin/#django.contrib.admin.ModelAdmin.fieldsets)
 a way to add a custom CSS classes to the fieldsets in the admin interface.
 
 To use this feature, specify the `classes` parameter in the `ModelAdmin.fieldsets`
 attribute:
 
@@ -565,38 +589,15 @@
             "fields": (
                 # ...
             )
         }),
     )
 ```
 
-![](https://user-images.githubusercontent.com/6928240/125337870-8f91e180-e360-11eb-9b19-7f903ab30464.png)
-
-### Table rows
-
-You can use the `get_row_classes` method of the `ModelAdmin`
-class to add custom classes to the rows in the list view.
-
-```python
-from django.contrib import admin
-from .models import Category
-
-
-@admin.register(Category)
-class CategoryAdmin(admin.ModelAdmin):
-
-    def get_row_classes(self, request, obj):
-        if obj.status == "success":
-            return ["table-success"]
-        elif obj.status == "failed":
-            return ["table-danger"]
-        return []
-```
-
-![image](https://user-images.githubusercontent.com/6928240/225705910-4f1309e1-93e3-456a-b9d0-f01748faec7b.png)
+![image](https://user-images.githubusercontent.com/6928240/233795448-17d2fa5c-739a-4751-8266-b4b4e879b1c8.png)
 
 ### Inline forms
 
 You can use the `get_form_classes` method of the `ModelAdmin` class
 to add custom classes to the inline forms:
 
 ```python
@@ -617,16 +618,16 @@
         if obj.status == "success":
             return ["table-success"]
         elif obj.status == "failed":
             return ["table-danger"]
         return []
 ```
 
-![image](https://user-images.githubusercontent.com/6928240/225713947-34e29927-b629-4b9a-bf6e-56ec8948de7e.png)
-![image](https://user-images.githubusercontent.com/6928240/225714321-87a33c52-65d8-4175-a118-cb751b92ebb8.png)
+![image](https://user-images.githubusercontent.com/6928240/233794982-1ca7248a-dc54-48c4-aea2-44d0d973d083.png)
+![image](https://user-images.githubusercontent.com/6928240/233795183-c056b82e-8b01-4f7d-9c09-65c0becbdc33.png)
 
 ## Settings
 
 `PAPER_FAVICON`<br>
 The path to the favicon for the admin interface.<br>
 Default: `"paper_admin/dist/assets/default_favicon.png"`
```

### Comparing `paper-admin-6.0.0rc3/package.json` & `paper-admin-6.0.0rc4/package.json`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/admin/filters.py` & `paper-admin-6.0.0rc4/paper_admin/admin/filters.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/admin/renderers.py` & `paper-admin-6.0.0rc4/paper_admin/admin/renderers.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/admin/views.py` & `paper-admin-6.0.0rc4/paper_admin/admin/views.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/admin/widgets.py` & `paper-admin-6.0.0rc4/paper_admin/admin/widgets.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/apps.py` & `paper-admin-6.0.0rc4/paper_admin/apps.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/conf.py` & `paper-admin-6.0.0rc4/paper_admin/conf.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/locale/ru/LC_MESSAGES/django.mo` & `paper-admin-6.0.0rc4/paper_admin/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/locale/ru/LC_MESSAGES/django.po` & `paper-admin-6.0.0rc4/paper_admin/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/locale/ru/LC_MESSAGES/djangojs.mo` & `paper-admin-6.0.0rc4/paper_admin/locale/ru/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/locale/ru/LC_MESSAGES/djangojs.po` & `paper-admin-6.0.0rc4/paper_admin/locale/ru/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/menu.py` & `paper-admin-6.0.0rc4/paper_admin/menu.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/monkey_patch.py` & `paper-admin-6.0.0rc4/paper_admin/monkey_patch.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/patches/dal/static/autocomplete_light/select2.js` & `paper-admin-6.0.0rc4/paper_admin/patches/dal/static/autocomplete_light/select2.js`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/patches/dal/widgets.py` & `paper-admin-6.0.0rc4/paper_admin/patches/dal/widgets.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/patches/django/changelist.py` & `paper-admin-6.0.0rc4/paper_admin/patches/django/changelist.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/patches/django/filters.py` & `paper-admin-6.0.0rc4/paper_admin/patches/django/filters.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/patches/django/helpers.py` & `paper-admin-6.0.0rc4/paper_admin/patches/django/helpers.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/patches/django/options.py` & `paper-admin-6.0.0rc4/paper_admin/patches/django/options.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/patches/django/prepopulate/__init__.py` & `paper-admin-6.0.0rc4/paper_admin/patches/django/prepopulate/__init__.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/patches/django/prepopulate/helpers.py` & `paper-admin-6.0.0rc4/paper_admin/patches/django/prepopulate/helpers.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/patches/django/renderer/auth.py` & `paper-admin-6.0.0rc4/paper_admin/patches/django/renderer/auth.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/patches/django/renderer/options.py` & `paper-admin-6.0.0rc4/paper_admin/patches/django/renderer/options.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/patches/django/renderer/widgets.py` & `paper-admin-6.0.0rc4/paper_admin/patches/django/renderer/widgets.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/patches/django/sites.py` & `paper-admin-6.0.0rc4/paper_admin/patches/django/sites.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/patches/django/sortable/__init__.py` & `paper-admin-6.0.0rc4/paper_admin/patches/django/sortable/__init__.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/patches/django/sortable/changelist.py` & `paper-admin-6.0.0rc4/paper_admin/patches/django/sortable/changelist.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/patches/django/sortable/options.py` & `paper-admin-6.0.0rc4/paper_admin/patches/django/sortable/options.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/patches/django/styles/options.py` & `paper-admin-6.0.0rc4/paper_admin/patches/django/styles/options.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/patches/django/tabs/helpers.py` & `paper-admin-6.0.0rc4/paper_admin/patches/django/tabs/helpers.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/patches/django/tabs/options.py` & `paper-admin-6.0.0rc4/paper_admin/patches/django/tabs/options.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/patches/django/widgets/options.py` & `paper-admin-6.0.0rc4/paper_admin/patches/django/widgets/options.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/patches/django/widgets/widgets.py` & `paper-admin-6.0.0rc4/paper_admin/patches/django/widgets/widgets.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/patches/django_solo/templates/admin/solo/change_form.html` & `paper-admin-6.0.0rc4/paper_admin/patches/django_solo/templates/admin/solo/change_form.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/patches/django_solo/templates/admin/solo/object_history.html` & `paper-admin-6.0.0rc4/paper_admin/patches/django_solo/templates/admin/solo/object_history.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/patches/formfield_defaults.py` & `paper-admin-6.0.0rc4/paper_admin/patches/formfield_defaults.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/patches/logentry_admin/admin.py` & `paper-admin-6.0.0rc4/paper_admin/patches/logentry_admin/admin.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/patches/mptt/admin.py` & `paper-admin-6.0.0rc4/paper_admin/patches/mptt/admin.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/patches/mptt/templatetags/paper_mptt_list.py` & `paper-admin-6.0.0rc4/paper_admin/patches/mptt/templatetags/paper_mptt_list.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/patches/post_office/admin.py` & `paper-admin-6.0.0rc4/paper_admin/patches/post_office/admin.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/patches/tree_queries/admin.py` & `paper-admin-6.0.0rc4/paper_admin/patches/tree_queries/admin.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/patches/tree_queries/templatetags/paper_tree_queries_list.py` & `paper-admin-6.0.0rc4/paper_admin/patches/tree_queries/templatetags/paper_tree_queries_list.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/app.802db2f5c8fabda7425c.js` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/app.802db2f5c8fabda7425c.js`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/app.802db2f5c8fabda7425c.js.map` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/app.802db2f5c8fabda7425c.js.map`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/app.styles.779e472c0f96c40859ce.css` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/app.styles.9ae55058e746fe5377c3.css`

 * *Files 2% similar despite different names*

```diff
@@ -1,6 +1,6 @@
 input[type=number]{-moz-appearance:textfield}input[type=number]:focus,input[type=number]:hover{-moz-appearance:number-input}textarea{resize:none}@font-face{font-display:swap;font-family:Roboto;font-style:normal;font-weight:300;src:url(/static/paper_admin/dist/assets/RobotoLight.woff2) format("woff2"),url(/static/paper_admin/dist/assets/RobotoLight.woff) format("woff")}@font-face{font-display:swap;font-family:Roboto;font-style:normal;font-weight:400;src:url(/static/paper_admin/dist/assets/Roboto.woff2) format("woff2"),url(/static/paper_admin/dist/assets/Roboto.woff) format("woff")}@font-face{font-display:swap;font-family:Roboto;font-style:normal;font-weight:500;src:url(/static/paper_admin/dist/assets/RobotoMedium.woff2) format("woff2"),url(/static/paper_admin/dist/assets/RobotoMedium.woff) format("woff")}@font-face{font-display:swap;font-family:Roboto;font-style:normal;font-weight:700;src:url(/static/paper_admin/dist/assets/RobotoBold.woff2) format("woff2"),url(/static/paper_admin/dist/assets/RobotoBold.woff) format("woff")}@font-face{font-display:swap;font-family:Roboto;font-style:italic;font-weight:300;src:url(/static/paper_admin/dist/assets/RobotoLightItalic.woff2) format("woff2"),url(/static/paper_admin/dist/assets/RobotoLightItalic.woff) format("woff")}@font-face{font-display:swap;font-family:Roboto;font-style:italic;font-weight:400;src:url(/static/paper_admin/dist/assets/RobotoItalic.woff2) format("woff2"),url(/static/paper_admin/dist/assets/RobotoItalic.woff) format("woff")}@font-face{font-display:swap;font-family:Roboto;font-style:italic;font-weight:500;src:url(/static/paper_admin/dist/assets/RobotoMediumItalic.woff2) format("woff2"),url(/static/paper_admin/dist/assets/RobotoMediumItalic.woff) format("woff")}@font-face{font-display:swap;font-family:Roboto;font-style:italic;font-weight:700;src:url(/static/paper_admin/dist/assets/RobotoBoldItalic.woff2) format("woff2"),url(/static/paper_admin/dist/assets/RobotoBoldItalic.woff) format("woff")}:root{--spacer:1rem;--border-radius:0.25rem;--border-radius-lg:0.3rem}body{font-family:Roboto,Helvetica Neue,Arial,sans-serif}.btn>i+span,.dropdown-item>i+span,.nav-link>i+span{margin-left:.25em}@media(min-width:576px){.container-fluid{padding-left:1rem;padding-right:1rem}}.list-default{list-style:none;margin:0;padding:0}.list-default:not(.list-inline) li+li{margin-top:5px}.table-height-hack{height:1px}.table-height-hack__cell{height:inherit}.flatpickr-calendar{animation:none;background:transparent;background:#fff;border:0;border-radius:5px;box-shadow:1px 0 0 #e6e6e6,-1px 0 0 #e6e6e6,0 1px 0 #e6e6e6,0 -1px 0 #e6e6e6,0 3px 13px rgba(0,0,0,.08);box-sizing:border-box;direction:ltr;display:none;font-size:14px;line-height:24px;opacity:0;padding:0;position:absolute;text-align:center;touch-action:manipulation;visibility:hidden;width:307.875px}.flatpickr-calendar.inline,.flatpickr-calendar.open{max-height:640px;opacity:1;visibility:visible}.flatpickr-calendar.open{display:inline-block;z-index:99999}.flatpickr-calendar.animate.open{animation:fpFadeInDown .3s cubic-bezier(.23,1,.32,1)}.flatpickr-calendar.inline{display:block;position:relative;top:2px}.flatpickr-calendar.static{position:absolute;top:calc(100% + 2px)}.flatpickr-calendar.static.open{display:block;z-index:999}.flatpickr-calendar.multiMonth .flatpickr-days .dayContainer:nth-child(n+1) .flatpickr-day.inRange:nth-child(7n+7){box-shadow:none!important}.flatpickr-calendar.multiMonth .flatpickr-days .dayContainer:nth-child(n+2) .flatpickr-day.inRange:nth-child(7n+1){box-shadow:-2px 0 0 #e6e6e6,5px 0 0 #e6e6e6}.flatpickr-calendar .hasTime .dayContainer,.flatpickr-calendar .hasWeeks .dayContainer{border-bottom:0;border-bottom-left-radius:0;border-bottom-right-radius:0}.flatpickr-calendar .hasWeeks .dayContainer{border-left:0}.flatpickr-calendar.hasTime .flatpickr-time{border-top:1px solid #e6e6e6;height:40px}.flatpickr-calendar.noCalendar.hasTime .flatpickr-time{height:auto}.flatpickr-calendar:after,.flatpickr-calendar:before{border:solid transparent;content:"";display:block;height:0;left:22px;pointer-events:none;position:absolute;width:0}.flatpickr-calendar.arrowRight:after,.flatpickr-calendar.arrowRight:before,.flatpickr-calendar.rightMost:after,.flatpickr-calendar.rightMost:before{left:auto;right:22px}.flatpickr-calendar.arrowCenter:after,.flatpickr-calendar.arrowCenter:before{left:50%;right:50%}.flatpickr-calendar:before{border-width:5px;margin:0 -5px}.flatpickr-calendar:after{border-width:4px;margin:0 -4px}.flatpickr-calendar.arrowTop:after,.flatpickr-calendar.arrowTop:before{bottom:100%}.flatpickr-calendar.arrowTop:before{border-bottom-color:#e6e6e6}.flatpickr-calendar.arrowTop:after{border-bottom-color:#fff}.flatpickr-calendar.arrowBottom:after,.flatpickr-calendar.arrowBottom:before{top:100%}.flatpickr-calendar.arrowBottom:before{border-top-color:#e6e6e6}.flatpickr-calendar.arrowBottom:after{border-top-color:#fff}.flatpickr-calendar:focus{outline:0}.flatpickr-wrapper{display:inline-block;position:relative}.flatpickr-months{display:flex}.flatpickr-months .flatpickr-month{fill:rgba(0,0,0,.9);background:transparent;color:rgba(0,0,0,.9);flex:1;height:34px;line-height:1;overflow:hidden;position:relative;text-align:center;-webkit-user-select:none;user-select:none}.flatpickr-months .flatpickr-next-month,.flatpickr-months .flatpickr-prev-month{fill:rgba(0,0,0,.9);color:rgba(0,0,0,.9);cursor:pointer;height:34px;padding:10px;position:absolute;-webkit-text-decoration:none;text-decoration:none;top:0;-webkit-user-select:none;user-select:none;z-index:3}.flatpickr-months .flatpickr-next-month.flatpickr-disabled,.flatpickr-months .flatpickr-prev-month.flatpickr-disabled{display:none}.flatpickr-months .flatpickr-next-month i,.flatpickr-months .flatpickr-prev-month i{position:relative}.flatpickr-months .flatpickr-next-month.flatpickr-prev-month,.flatpickr-months .flatpickr-prev-month.flatpickr-prev-month{left:0}.flatpickr-months .flatpickr-next-month.flatpickr-next-month,.flatpickr-months .flatpickr-prev-month.flatpickr-next-month{right:0}.flatpickr-months .flatpickr-next-month:hover,.flatpickr-months .flatpickr-prev-month:hover{color:#959ea9}.flatpickr-months .flatpickr-next-month:hover svg,.flatpickr-months .flatpickr-prev-month:hover svg{fill:#f64747}.flatpickr-months .flatpickr-next-month svg,.flatpickr-months .flatpickr-prev-month svg{height:14px;width:14px}.flatpickr-months .flatpickr-next-month svg path,.flatpickr-months .flatpickr-prev-month svg path{fill:inherit;transition:fill .1s}.numInputWrapper{height:auto;position:relative}.numInputWrapper input,.numInputWrapper span{display:inline-block}.numInputWrapper input{width:100%}.numInputWrapper input::-ms-clear{display:none}.numInputWrapper input::-webkit-inner-spin-button,.numInputWrapper input::-webkit-outer-spin-button{-webkit-appearance:none;margin:0}.numInputWrapper span{border:1px solid rgba(57,57,57,.15);box-sizing:border-box;cursor:pointer;height:50%;line-height:50%;opacity:0;padding:0 4px 0 2px;position:absolute;right:0;width:14px}.numInputWrapper span:hover{background:rgba(0,0,0,.1)}.numInputWrapper span:active{background:rgba(0,0,0,.2)}.numInputWrapper span:after{content:"";display:block;position:absolute}.numInputWrapper span.arrowUp{border-bottom:0;top:0}.numInputWrapper span.arrowUp:after{border-bottom:4px solid rgba(57,57,57,.6);border-left:4px solid transparent;border-right:4px solid transparent;top:26%}.numInputWrapper span.arrowDown{top:50%}.numInputWrapper span.arrowDown:after{border-left:4px solid transparent;border-right:4px solid transparent;border-top:4px solid rgba(57,57,57,.6);top:40%}.numInputWrapper span svg{height:auto;width:inherit}.numInputWrapper span svg path{fill:rgba(0,0,0,.5)}.numInputWrapper:hover{background:rgba(0,0,0,.05)}.numInputWrapper:hover span{opacity:1}.flatpickr-current-month{color:inherit;display:inline-block;font-size:135%;font-weight:300;height:34px;left:12.5%;line-height:inherit;line-height:1;padding:7.48px 0 0;position:absolute;text-align:center;transform:translateZ(0);width:75%}.flatpickr-current-month span.cur-month{color:inherit;display:inline-block;font-family:inherit;font-weight:700;margin-left:.5ch;padding:0}.flatpickr-current-month span.cur-month:hover{background:rgba(0,0,0,.05)}.flatpickr-current-month .numInputWrapper{display:inline-block;width:6ch;width:7ch\0}.flatpickr-current-month .numInputWrapper span.arrowUp:after{border-bottom-color:rgba(0,0,0,.9)}.flatpickr-current-month .numInputWrapper span.arrowDown:after{border-top-color:rgba(0,0,0,.9)}.flatpickr-current-month input.cur-year{-webkit-appearance:textfield;appearance:textfield;background:transparent;border:0;border-radius:0;box-sizing:border-box;color:inherit;cursor:text;display:inline-block;font-family:inherit;font-size:inherit;font-weight:300;height:auto;line-height:inherit;margin:0;padding:0 0 0 .5ch;vertical-align:baseline;vertical-align:initial}.flatpickr-current-month input.cur-year:focus{outline:0}.flatpickr-current-month input.cur-year[disabled],.flatpickr-current-month input.cur-year[disabled]:hover{background:transparent;color:rgba(0,0,0,.5);font-size:100%;pointer-events:none}.flatpickr-current-month .flatpickr-monthDropdown-months{appearance:menulist;-webkit-appearance:menulist;-moz-appearance:menulist;background:transparent;border:none;border-radius:0;box-sizing:border-box;-webkit-box-sizing:border-box;color:inherit;cursor:pointer;font-family:inherit;font-size:inherit;font-weight:300;height:auto;line-height:inherit;margin:-1px 0 0;outline:none;padding:0 0 0 .5ch;position:relative;vertical-align:baseline;vertical-align:initial;width:auto}.flatpickr-current-month .flatpickr-monthDropdown-months:active,.flatpickr-current-month .flatpickr-monthDropdown-months:focus{outline:none}.flatpickr-current-month .flatpickr-monthDropdown-months:hover{background:rgba(0,0,0,.05)}.flatpickr-current-month .flatpickr-monthDropdown-months .flatpickr-monthDropdown-month{background-color:transparent;outline:none;padding:0}.flatpickr-weekdays{align-items:center;background:transparent;display:flex;height:28px;overflow:hidden;text-align:center;width:100%}.flatpickr-weekdays .flatpickr-weekdaycontainer{display:flex;flex:1}span.flatpickr-weekday{background:transparent;color:rgba(0,0,0,.54);cursor:default;display:block;flex:1;font-size:90%;font-weight:bolder;line-height:1;margin:0;text-align:center}.dayContainer,.flatpickr-weeks{padding:1px 0 0}.flatpickr-days{align-items:flex-start;display:flex;overflow:hidden;position:relative;width:307.875px}.flatpickr-days:focus{outline:0}.dayContainer{box-sizing:border-box;display:inline-block;display:flex;flex-wrap:wrap;-ms-flex-wrap:wrap;justify-content:space-around;max-width:307.875px;min-width:307.875px;opacity:1;outline:0;padding:0;text-align:left;transform:translateZ(0);width:307.875px}.dayContainer+.dayContainer{box-shadow:-1px 0 0 #e6e6e6}.flatpickr-day{background:none;border:1px solid transparent;border-radius:150px;box-sizing:border-box;color:#393939;cursor:pointer;display:inline-block;flex-basis:14.2857143%;font-weight:400;height:39px;justify-content:center;line-height:39px;margin:0;max-width:39px;position:relative;text-align:center;width:14.2857143%}.flatpickr-day.inRange,.flatpickr-day.nextMonthDay.inRange,.flatpickr-day.nextMonthDay.today.inRange,.flatpickr-day.nextMonthDay:focus,.flatpickr-day.nextMonthDay:hover,.flatpickr-day.prevMonthDay.inRange,.flatpickr-day.prevMonthDay.today.inRange,.flatpickr-day.prevMonthDay:focus,.flatpickr-day.prevMonthDay:hover,.flatpickr-day.today.inRange,.flatpickr-day:focus,.flatpickr-day:hover{background:#e6e6e6;border-color:#e6e6e6;cursor:pointer;outline:0}.flatpickr-day.today{border-color:#959ea9}.flatpickr-day.today:focus,.flatpickr-day.today:hover{background:#959ea9;border-color:#959ea9;color:#fff}.flatpickr-day.endRange,.flatpickr-day.endRange.inRange,.flatpickr-day.endRange.nextMonthDay,.flatpickr-day.endRange.prevMonthDay,.flatpickr-day.endRange:focus,.flatpickr-day.endRange:hover,.flatpickr-day.selected,.flatpickr-day.selected.inRange,.flatpickr-day.selected.nextMonthDay,.flatpickr-day.selected.prevMonthDay,.flatpickr-day.selected:focus,.flatpickr-day.selected:hover,.flatpickr-day.startRange,.flatpickr-day.startRange.inRange,.flatpickr-day.startRange.nextMonthDay,.flatpickr-day.startRange.prevMonthDay,.flatpickr-day.startRange:focus,.flatpickr-day.startRange:hover{background:#569ff7;border-color:#569ff7;box-shadow:none;color:#fff}.flatpickr-day.endRange.startRange,.flatpickr-day.selected.startRange,.flatpickr-day.startRange.startRange{border-radius:50px 0 0 50px}.flatpickr-day.endRange.endRange,.flatpickr-day.selected.endRange,.flatpickr-day.startRange.endRange{border-radius:0 50px 50px 0}.flatpickr-day.endRange.startRange+.endRange:not(:nth-child(7n+1)),.flatpickr-day.selected.startRange+.endRange:not(:nth-child(7n+1)),.flatpickr-day.startRange.startRange+.endRange:not(:nth-child(7n+1)){box-shadow:-10px 0 0 #569ff7}.flatpickr-day.endRange.startRange.endRange,.flatpickr-day.selected.startRange.endRange,.flatpickr-day.startRange.startRange.endRange{border-radius:50px}.flatpickr-day.inRange{border-radius:0;box-shadow:-5px 0 0 #e6e6e6,5px 0 0 #e6e6e6}.flatpickr-day.flatpickr-disabled,.flatpickr-day.flatpickr-disabled:hover,.flatpickr-day.nextMonthDay,.flatpickr-day.notAllowed,.flatpickr-day.notAllowed.nextMonthDay,.flatpickr-day.notAllowed.prevMonthDay,.flatpickr-day.prevMonthDay{background:transparent;border-color:transparent;color:rgba(57,57,57,.3);cursor:default}.flatpickr-day.flatpickr-disabled,.flatpickr-day.flatpickr-disabled:hover{color:rgba(57,57,57,.1);cursor:not-allowed}.flatpickr-day.week.selected{border-radius:0;box-shadow:-5px 0 0 #569ff7,5px 0 0 #569ff7}.flatpickr-day.hidden{visibility:hidden}.rangeMode .flatpickr-day{margin-top:1px}.flatpickr-weekwrapper{float:left}.flatpickr-weekwrapper .flatpickr-weeks{box-shadow:1px 0 0 #e6e6e6;padding:0 12px}.flatpickr-weekwrapper .flatpickr-weekday{float:none;line-height:28px;width:100%}.flatpickr-weekwrapper span.flatpickr-day,.flatpickr-weekwrapper span.flatpickr-day:hover{background:transparent;border:none;color:rgba(57,57,57,.3);cursor:default;display:block;max-width:none;width:100%}.flatpickr-innerContainer{box-sizing:border-box;display:block;display:flex;overflow:hidden}.flatpickr-rContainer{box-sizing:border-box;display:inline-block;padding:0}.flatpickr-time{box-sizing:border-box;display:block;display:flex;height:0;line-height:40px;max-height:40px;outline:0;overflow:hidden;text-align:center}.flatpickr-time:after{clear:both;content:"";display:table}.flatpickr-time .numInputWrapper{flex:1;float:left;height:40px;width:40%}.flatpickr-time .numInputWrapper span.arrowUp:after{border-bottom-color:#393939}.flatpickr-time .numInputWrapper span.arrowDown:after{border-top-color:#393939}.flatpickr-time.hasSeconds .numInputWrapper{width:26%}.flatpickr-time.time24hr .numInputWrapper{width:49%}.flatpickr-time input{-webkit-appearance:textfield;appearance:textfield;background:transparent;border:0;border-radius:0;box-shadow:none;box-sizing:border-box;color:#393939;font-size:14px;height:inherit;line-height:inherit;margin:0;padding:0;position:relative;text-align:center}.flatpickr-time input.flatpickr-hour{font-weight:700}.flatpickr-time input.flatpickr-minute,.flatpickr-time input.flatpickr-second{font-weight:400}.flatpickr-time input:focus{border:0;outline:0}.flatpickr-time .flatpickr-am-pm,.flatpickr-time .flatpickr-time-separator{align-self:center;color:#393939;float:left;font-weight:700;height:inherit;line-height:inherit;-webkit-user-select:none;user-select:none;width:2%}.flatpickr-time .flatpickr-am-pm{cursor:pointer;font-weight:400;outline:0;text-align:center;width:18%}.flatpickr-time .flatpickr-am-pm:focus,.flatpickr-time .flatpickr-am-pm:hover,.flatpickr-time input:focus,.flatpickr-time input:hover{background:#eee}.flatpickr-input[readonly]{cursor:pointer}@keyframes fpFadeInDown{0%{opacity:0;transform:translate3d(0,-20px,0)}to{opacity:1;transform:translateZ(0)}}.flatpickr-input+.form-control.input{background-color:#fff;border-bottom-left-radius:.25rem;border-top-left-radius:.25rem}.flatpickr-calendar.arrowTop:after{border-bottom-color:#1090c0}.flatpickr-calendar{color:#fff;font-size:.875rem;line-height:1.25;margin-top:3px;width:262px}.flatpickr-months .flatpickr-month{background-color:#1090c0;border-radius:5px 5px 0 0;color:inherit}.flatpickr-months .flatpickr-next-month svg,.flatpickr-months .flatpickr-prev-month svg{fill:#fff;transition:fill .2s}.flatpickr-months .flatpickr-next-month:hover svg,.flatpickr-months .flatpickr-prev-month:hover svg{fill:hsla(0,0%,100%,.5)}.flatpickr-current-month{display:flex;justify-content:space-around}.flatpickr-current-month .flatpickr-monthDropdown-months{padding:0 16px 0 0}.flatpickr-current-month .flatpickr-monthDropdown-months .flatpickr-monthDropdown-month{background-color:#1090c0;font-weight:300}.flatpickr-weekdays{background-color:#1090c0;padding-left:5px;padding-right:5px}span.flatpickr-weekday{color:inherit}.flatpickr-days{width:100%}.dayContainer{max-width:none;min-width:0;padding:5px;width:100%}.flatpickr-day{height:36px;line-height:36px;max-width:36px}.flatpickr-day.selected{background-color:#9393ea;border-color:#9393ea}.select2-container{box-sizing:border-box;display:inline-block;margin:0;position:relative;vertical-align:middle}.select2-container .select2-selection--single{box-sizing:border-box;cursor:pointer;display:block;height:28px;user-select:none;-webkit-user-select:none}.select2-container .select2-selection--single .select2-selection__rendered{display:block;overflow:hidden;padding-left:8px;padding-right:20px;text-overflow:ellipsis;white-space:nowrap}.select2-container .select2-selection--single .select2-selection__clear{background-color:transparent;border:none;font-size:1em}.select2-container[dir=rtl] .select2-selection--single .select2-selection__rendered{padding-left:20px;padding-right:8px}.select2-container .select2-selection--multiple{box-sizing:border-box;cursor:pointer;display:block;min-height:32px;user-select:none;-webkit-user-select:none}.select2-container .select2-selection--multiple .select2-selection__rendered{display:inline;list-style:none;padding:0}.select2-container .select2-selection--multiple .select2-selection__clear{background-color:transparent;border:none;font-size:1em}.select2-container .select2-search--inline .select2-search__field{border:none;box-sizing:border-box;font-family:sans-serif;font-size:100%;height:18px;margin-left:5px;margin-top:5px;max-width:100%;overflow:hidden;padding:0;resize:none;vertical-align:bottom;word-break:keep-all}.select2-container .select2-search--inline .select2-search__field::-webkit-search-cancel-button{-webkit-appearance:none}.select2-dropdown{border:1px solid #aaa;border-radius:4px;box-sizing:border-box;display:block;left:-100000px;position:absolute;width:100%;z-index:1051}.select2-results{display:block}.select2-results__options{list-style:none;margin:0;padding:0}.select2-results__option{padding:6px;user-select:none;-webkit-user-select:none}.select2-results__option--selectable{cursor:pointer}.select2-container--open .select2-dropdown{left:0}.select2-container--open .select2-dropdown--above{border-bottom:none;border-bottom-left-radius:0;border-bottom-right-radius:0}.select2-container--open .select2-dropdown--below{border-top:none;border-top-left-radius:0;border-top-right-radius:0}.select2-search--dropdown{display:block;padding:4px}.select2-search--dropdown .select2-search__field{box-sizing:border-box;padding:4px;width:100%}.select2-search--dropdown .select2-search__field::-webkit-search-cancel-button{-webkit-appearance:none}.select2-search--dropdown.select2-search--hide{display:none}.select2-close-mask{background-color:#fff;border:0;display:block;filter:alpha(opacity=0);height:auto;left:0;margin:0;min-height:100%;min-width:100%;opacity:0;padding:0;position:fixed;top:0;width:auto;z-index:99}.select2-hidden-accessible{clip:rect(0 0 0 0)!important;border:0!important;-webkit-clip-path:inset(50%)!important;clip-path:inset(50%)!important;height:1px!important;overflow:hidden!important;padding:0!important;position:absolute!important;white-space:nowrap!important;width:1px!important}.select2-container--default .select2-selection--single{background-color:#fff;border:1px solid #aaa;border-radius:4px}.select2-container--default .select2-selection--single .select2-selection__rendered{color:#444;line-height:28px}.select2-container--default .select2-selection--single .select2-selection__clear{cursor:pointer;float:right;font-weight:700;height:26px;margin-right:20px;padding-right:0}.select2-container--default .select2-selection--single .select2-selection__placeholder{color:#999}.select2-container--default .select2-selection--single .select2-selection__arrow{height:26px;position:absolute;right:1px;top:1px;width:20px}.select2-container--default .select2-selection--single .select2-selection__arrow b{border-color:#888 transparent transparent;border-style:solid;border-width:5px 4px 0;height:0;left:50%;margin-left:-4px;margin-top:-2px;position:absolute;top:50%;width:0}.select2-container--default[dir=rtl] .select2-selection--single .select2-selection__clear{float:left}.select2-container--default[dir=rtl] .select2-selection--single .select2-selection__arrow{left:1px;right:auto}.select2-container--default.select2-container--disabled .select2-selection--single{background-color:#eee;cursor:default}.select2-container--default.select2-container--disabled .select2-selection--single .select2-selection__clear{display:none}.select2-container--default.select2-container--open .select2-selection--single .select2-selection__arrow b{border-color:transparent transparent #888;border-width:0 4px 5px}.select2-container--default .select2-selection--multiple{background-color:#fff;border:1px solid #aaa;border-radius:4px;cursor:text;padding-bottom:5px;padding-right:5px;position:relative}.select2-container--default .select2-selection--multiple.select2-selection--clearable{padding-right:25px}.select2-container--default .select2-selection--multiple .select2-selection__clear{cursor:pointer;font-weight:700;height:20px;margin-right:10px;margin-top:5px;padding:1px;position:absolute}.select2-container--default .select2-selection--multiple .select2-selection__choice{background-color:#e4e4e4;border:1px solid #aaa;border-radius:4px;box-sizing:border-box;display:inline-block;margin-left:5px;margin-top:5px;max-width:100%;overflow:hidden;padding:0 0 0 20px;position:relative;text-overflow:ellipsis;vertical-align:bottom;white-space:nowrap}.select2-container--default .select2-selection--multiple .select2-selection__choice__display{cursor:default;padding-left:2px;padding-right:5px}.select2-container--default .select2-selection--multiple .select2-selection__choice__remove{background-color:transparent;border:none;border-bottom-left-radius:4px;border-right:1px solid #aaa;border-top-left-radius:4px;color:#999;cursor:pointer;font-size:1em;font-weight:700;left:0;padding:0 4px;position:absolute;top:0}.select2-container--default .select2-selection--multiple .select2-selection__choice__remove:focus,.select2-container--default .select2-selection--multiple .select2-selection__choice__remove:hover{background-color:#f1f1f1;color:#333;outline:none}.select2-container--default[dir=rtl] .select2-selection--multiple .select2-selection__choice{margin-left:5px;margin-right:auto}.select2-container--default[dir=rtl] .select2-selection--multiple .select2-selection__choice__display{padding-left:5px;padding-right:2px}.select2-container--default[dir=rtl] .select2-selection--multiple .select2-selection__choice__remove{border-bottom-left-radius:0;border-bottom-right-radius:4px;border-left:1px solid #aaa;border-right:none;border-top-left-radius:0;border-top-right-radius:4px}.select2-container--default[dir=rtl] .select2-selection--multiple .select2-selection__clear{float:left;margin-left:10px;margin-right:auto}.select2-container--default.select2-container--focus .select2-selection--multiple{border:1px solid #000;outline:0}.select2-container--default.select2-container--disabled .select2-selection--multiple{background-color:#eee;cursor:default}.select2-container--default.select2-container--disabled .select2-selection__choice__remove{display:none}.select2-container--default.select2-container--open.select2-container--above .select2-selection--multiple,.select2-container--default.select2-container--open.select2-container--above .select2-selection--single{border-top-left-radius:0;border-top-right-radius:0}.select2-container--default.select2-container--open.select2-container--below .select2-selection--multiple,.select2-container--default.select2-container--open.select2-container--below .select2-selection--single{border-bottom-left-radius:0;border-bottom-right-radius:0}.select2-container--default .select2-search--dropdown .select2-search__field{border:1px solid #aaa}.select2-container--default .select2-search--inline .select2-search__field{-webkit-appearance:textfield;background:transparent;border:none;box-shadow:none;outline:0}.select2-container--default .select2-results>.select2-results__options{max-height:200px;overflow-y:auto}.select2-container--default .select2-results__option .select2-results__option{padding-left:1em}.select2-container--default .select2-results__option .select2-results__option .select2-results__group{padding-left:0}.select2-container--default .select2-results__option .select2-results__option .select2-results__option{margin-left:-1em;padding-left:2em}.select2-container--default .select2-results__option .select2-results__option .select2-results__option .select2-results__option{margin-left:-2em;padding-left:3em}.select2-container--default .select2-results__option .select2-results__option .select2-results__option .select2-results__option .select2-results__option{margin-left:-3em;padding-left:4em}.select2-container--default .select2-results__option .select2-results__option .select2-results__option .select2-results__option .select2-results__option .select2-results__option{margin-left:-4em;padding-left:5em}.select2-container--default .select2-results__option .select2-results__option .select2-results__option .select2-results__option .select2-results__option .select2-results__option .select2-results__option{margin-left:-5em;padding-left:6em}.select2-container--default .select2-results__option--group{padding:0}.select2-container--default .select2-results__option--disabled{color:#999}.select2-container--default .select2-results__option--selected{background-color:#ddd}.select2-container--default .select2-results__option--highlighted.select2-results__option--selectable{background-color:#5897fb}.select2-container--default .select2-results__group{cursor:default;display:block;padding:6px}.select2-container--classic .select2-selection--single{background-color:#f7f7f7;background-image:linear-gradient(180deg,#fff 50%,#eee);background-repeat:repeat-x;border:1px solid #aaa;border-radius:4px;filter:progid:DXImageTransform.Microsoft.gradient(startColorstr="#FFFFFFFF",endColorstr="#FFEEEEEE",GradientType=0);outline:0}.select2-container--classic .select2-selection--single:focus{border:1px solid #5897fb}.select2-container--classic .select2-selection--single .select2-selection__rendered{color:#444;line-height:28px}.select2-container--classic .select2-selection--single .select2-selection__clear{cursor:pointer;float:right;font-weight:700;height:26px;margin-right:20px}.select2-container--classic .select2-selection--single .select2-selection__placeholder{color:#999}.select2-container--classic .select2-selection--single .select2-selection__arrow{background-color:#ddd;background-image:linear-gradient(180deg,#eee 50%,#ccc);background-repeat:repeat-x;border:none;border-bottom-right-radius:4px;border-left:1px solid #aaa;border-top-right-radius:4px;filter:progid:DXImageTransform.Microsoft.gradient(startColorstr="#FFEEEEEE",endColorstr="#FFCCCCCC",GradientType=0);height:26px;position:absolute;right:1px;top:1px;width:20px}.select2-container--classic .select2-selection--single .select2-selection__arrow b{border-color:#888 transparent transparent;border-style:solid;border-width:5px 4px 0;height:0;left:50%;margin-left:-4px;margin-top:-2px;position:absolute;top:50%;width:0}.select2-container--classic[dir=rtl] .select2-selection--single .select2-selection__clear{float:left}.select2-container--classic[dir=rtl] .select2-selection--single .select2-selection__arrow{border:none;border-radius:0;border-bottom-left-radius:4px;border-right:1px solid #aaa;border-top-left-radius:4px;left:1px;right:auto}.select2-container--classic.select2-container--open .select2-selection--single{border:1px solid #5897fb}.select2-container--classic.select2-container--open .select2-selection--single .select2-selection__arrow{background:transparent;border:none}.select2-container--classic.select2-container--open .select2-selection--single .select2-selection__arrow b{border-color:transparent transparent #888;border-width:0 4px 5px}.select2-container--classic.select2-container--open.select2-container--above .select2-selection--single{background-image:linear-gradient(180deg,#fff 0,#eee 50%);background-repeat:repeat-x;border-top:none;border-top-left-radius:0;border-top-right-radius:0;filter:progid:DXImageTransform.Microsoft.gradient(startColorstr="#FFFFFFFF",endColorstr="#FFEEEEEE",GradientType=0)}.select2-container--classic.select2-container--open.select2-container--below .select2-selection--single{background-image:linear-gradient(180deg,#eee 50%,#fff);background-repeat:repeat-x;border-bottom:none;border-bottom-left-radius:0;border-bottom-right-radius:0;filter:progid:DXImageTransform.Microsoft.gradient(startColorstr="#FFEEEEEE",endColorstr="#FFFFFFFF",GradientType=0)}.select2-container--classic .select2-selection--multiple{background-color:#fff;border:1px solid #aaa;border-radius:4px;cursor:text;outline:0;padding-bottom:5px;padding-right:5px}.select2-container--classic .select2-selection--multiple:focus{border:1px solid #5897fb}.select2-container--classic .select2-selection--multiple .select2-selection__clear{display:none}.select2-container--classic .select2-selection--multiple .select2-selection__choice{background-color:#e4e4e4;border:1px solid #aaa;border-radius:4px;display:inline-block;margin-left:5px;margin-top:5px;padding:0}.select2-container--classic .select2-selection--multiple .select2-selection__choice__display{cursor:default;padding-left:2px;padding-right:5px}.select2-container--classic .select2-selection--multiple .select2-selection__choice__remove{background-color:transparent;border:none;border-bottom-left-radius:4px;border-top-left-radius:4px;color:#888;cursor:pointer;font-size:1em;font-weight:700;padding:0 4px}.select2-container--classic .select2-selection--multiple .select2-selection__choice__remove:hover{color:#555;outline:none}.select2-container--classic[dir=rtl] .select2-selection--multiple .select2-selection__choice{margin-left:5px;margin-right:auto}.select2-container--classic[dir=rtl] .select2-selection--multiple .select2-selection__choice__display{padding-left:5px;padding-right:2px}.select2-container--classic[dir=rtl] .select2-selection--multiple .select2-selection__choice__remove{border-bottom-left-radius:0;border-bottom-right-radius:4px;border-top-left-radius:0;border-top-right-radius:4px}.select2-container--classic.select2-container--open .select2-selection--multiple{border:1px solid #5897fb}.select2-container--classic.select2-container--open.select2-container--above .select2-selection--multiple{border-top:none;border-top-left-radius:0;border-top-right-radius:0}.select2-container--classic.select2-container--open.select2-container--below .select2-selection--multiple{border-bottom:none;border-bottom-left-radius:0;border-bottom-right-radius:0}.select2-container--classic .select2-search--dropdown .select2-search__field{border:1px solid #aaa;outline:0}.select2-container--classic .select2-search--inline .select2-search__field{box-shadow:none;outline:0}.select2-container--classic .select2-dropdown{background-color:#fff;border:1px solid transparent}.select2-container--classic .select2-dropdown--above{border-bottom:none}.select2-container--classic .select2-dropdown--below{border-top:none}.select2-container--classic .select2-results>.select2-results__options{max-height:200px;overflow-y:auto}.select2-container--classic .select2-results__option--group{padding:0}.select2-container--classic .select2-results__option--disabled{color:grey}.select2-container--classic .select2-results__option--highlighted.select2-results__option--selectable{background-color:#3875d7;color:#fff}.select2-container--classic .select2-results__group{cursor:default;display:block;padding:6px}.select2-container--classic.select2-container--open .select2-dropdown{border-color:#5897fb}.select2-container--default{font-size:1rem;line-height:1.375}.select2-container--default .select2-selection--multiple,.select2-container--default .select2-selection--single{background-color:#fff;border:1px solid #d0d0d0;border-radius:.3rem;outline:none;transition:border-color .15s ease-in-out}.select2-container--default .select2-search--dropdown{padding:4px}.select2-container--default .select2-search--dropdown .select2-search__field{background-color:#fff;border:1px solid #d0d0d0;border-radius:.3rem;color:inherit;font-family:inherit;font-size:inherit;line-height:inherit;outline:none;padding:.375rem}.select2-container--default .select2-selection--single{height:100%}.select2-container--default .select2-selection--single .select2-selection__placeholder{color:#c3c3c3}.select2-container--default .select2-selection--single .select2-selection__rendered{box-sizing:content-box;color:inherit;line-height:inherit;margin-right:24px;min-height:1.375rem;padding:.5rem 0 .5rem .75rem}.select2-container--default .select2-selection--single .select2-selection__arrow{height:100%;top:0;width:24px}.select2-container--default .select2-selection--single .select2-selection__arrow b{border-color:#1d1d1d transparent transparent}.select2-container--default .select2-selection--single .select2-selection__clear{float:none;height:100%;margin-right:24px;padding:0;position:absolute;right:0;top:0}.select2-container--default .select2-selection--single.select2-selection--clearable .select2-selection__rendered{margin-right:48px}.select2-container--default .select2-selection--single:hover{border-color:#d0d0d0;box-shadow:none}.select2-container--default .select2-selection--multiple{box-sizing:content-box;min-height:0;padding:0 0 4px}.select2-container--default .select2-selection--multiple .select2-selection__clear{height:100%;margin:0;padding:0;right:0;top:0}.select2-container--default .select2-selection--multiple .select2-selection__rendered{margin:0}.select2-container--default .select2-selection--multiple .select2-selection__choice{background-color:#e9ecef;border:1px solid #d0d0d0;border-radius:.3rem;color:#1d1d1d;margin:4px 0 0 4px;padding:3px 28px 3px 8px;vertical-align:top}.select2-container--default .select2-selection--multiple .select2-selection__choice__display{padding:0}.select2-container--default .select2-selection--multiple .select2-selection__choice__remove{border:0;border-radius:0;height:100%;left:auto;padding:0;right:0;width:24px}.select2-container--default .select2-selection--multiple .select2-selection__choice__remove:after,.select2-container--default .select2-selection--multiple .select2-selection__choice__remove:before{background:#909090;content:"";height:2px;left:50%;margin-left:-5px;margin-top:-1px;position:absolute;top:50%;transition:background .15s ease-in-out;width:10px}.select2-container--default .select2-selection--multiple .select2-selection__choice__remove:before{transform:rotate(45deg)}.select2-container--default .select2-selection--multiple .select2-selection__choice__remove:after{transform:rotate(-45deg)}.select2-container--default .select2-selection--multiple .select2-selection__choice__remove span{display:none}.select2-container--default .select2-selection--multiple .select2-selection__choice__remove:focus,.select2-container--default .select2-selection--multiple .select2-selection__choice__remove:hover{background-color:#dadfe4}.select2-container--default .select2-selection--multiple .select2-selection__choice__remove:focus:after,.select2-container--default .select2-selection--multiple .select2-selection__choice__remove:focus:before,.select2-container--default .select2-selection--multiple .select2-selection__choice__remove:hover:after,.select2-container--default .select2-selection--multiple .select2-selection__choice__remove:hover:before{background-color:#1d1d1d}.select2-container--default .select2-selection--multiple .select2-search--inline{display:inline-block;vertical-align:top}.select2-container--default .select2-selection--multiple .select2-search--inline .select2-search__field{font-family:inherit;font-size:inherit;height:30px;line-height:inherit;margin-left:8px;margin-top:4px;padding-bottom:4px;padding-top:4px}.select2-container--default .select2-selection--multiple .select2-search--inline .select2-search__field::placeholder{color:#c3c3c3}.select2-container--default .select2-selection--multiple .select2-selection__rendered:empty+.select2-search--inline .select2-search__field{margin-left:.75rem}.select2-container--default .select2-selection--multiple.select2-selection__rendered--clearable{padding-right:24px}.select2-container--default .select2-selection--multiple:hover{border-color:#d0d0d0;box-shadow:none}.select2-container--default .select2-results>.select2-results__options{max-height:300px}.select2-container--default .select2-results__option--highlighted.select2-results__option--selectable{background-color:#79aec8;color:#fff;font-weight:400}.select2-container--default .select2-results__option--highlighted.select2-results__option--selected,.select2-container--default .select2-results__option--selected{background-color:#e9ecef;color:#1d1d1d;font-weight:400}.select2-container--default .select2-results__option--disabled{background-color:transparent;color:#9a9a9a;font-weight:400;transition:background .15s ease-in-out,color .15s ease-in-out}.select2-container--default .select2-results__option--highlighted.select2-results__option--disabled{background-color:#79aec8;color:#fff;font-weight:400}.select2-container--default .select2-results__option--selected.select2-results__option--disabled{background-color:#e9ecef}.select2-container--default.select2-container--focus .select2-selection--multiple,.select2-container--default.select2-container--focus .select2-selection--single,.select2-container--default.select2-container--open .select2-selection--multiple,.select2-container--default.select2-container--open .select2-selection--single{border-color:#444;box-shadow:0 0 0 1px #444}.select2-container--default.select2-container--open .select2-selection--single .select2-selection__arrow b{border-color:transparent transparent #1d1d1d}.select2-dropdown{background-color:#fff;border:1px solid #444;border-radius:.3rem;box-shadow:0 0 0 1px #444;overflow:hidden}.select2-dropdown.select2-dropdown--below{margin-top:1px}.select2-dropdown.select2-dropdown--above{margin-bottom:1px}.select2-results__option{color:#1d1d1d;padding:.5rem .75rem}.select2-search+.select2-results .loading-results,.select2-search+.select2-results .select2-results__message{margin-bottom:4px;padding-bottom:0;padding-top:0}.select2-selection__clear{background-color:transparent;border:none;position:relative;width:24px}.select2-selection__clear:after,.select2-selection__clear:before{background:#909090;content:"";height:2px;left:50%;margin-left:-6px;margin-top:-1px;position:absolute;top:50%;transition:background .15s ease-in-out;width:12px}.select2-selection__clear:before{transform:rotate(45deg)}.select2-selection__clear:after{transform:rotate(-45deg)}.select2-selection__clear span{display:none}.select2-selection__clear:hover:after,.select2-selection__clear:hover:before{background-color:#1d1d1d}.select2-container--small{font-size:.875rem;line-height:1.375}.select2-container--small .select2-selection--multiple,.select2-container--small .select2-selection--single{border-radius:.25rem}.select2-container--small .select2-search--dropdown .select2-search__field{border-radius:.25rem;padding:.28125rem .25rem}.select2-container--small .select2-selection--single .select2-selection__rendered{min-height:1.203125rem;padding:.375rem 0 .375rem .5rem}.select2-container--small .select2-selection--multiple{box-sizing:content-box;min-height:sum(1.203125rem,6px,2px,4px)}.select2-container--small .select2-selection--multiple .select2-selection__choice{border-radius:.25rem;padding:3px sum(28px) 3px 8px}.select2-container--small .select2-selection--multiple .select2-search--inline .select2-search__field{height:sum(1.203125rem,6px,2px)}.select2-container--small.select2-dropdown{border-radius:.25rem}.select2-container--small .select2-results__option{padding:.375rem .5rem}.paper-widget--invalid .select2-selection{border-color:#df7d5c;box-shadow:0 0 0 1px #df7d5c}.js .clearable-file-field input[type=file]{height:.1px;opacity:0;overflow:hidden;position:absolute;width:.1px;z-index:-1}.clearable-file-field input[type=file].focus+label,.clearable-file-field input[type=file]:focus+label{border-color:#444;box-shadow:0 0 0 1px #444}.clearable-file-field__state{margin-right:1.5em}.clearable-file-field__button{max-width:100%}.no-js .clearable-file-field__button{display:none}.clearable-file-field__button span{display:inline-block;max-width:calc(100% - 1.25rem);overflow:hidden;text-overflow:ellipsis;vertical-align:top;white-space:nowrap}@media(min-width:576px){.date-field{max-width:220px}.email-field{max-width:360px}}.file-field{position:relative}@media(min-width:576px){.file-field{max-width:360px}}.file-field input.form-control{clip:rect(0,0,0,0);pointer-events:none;position:absolute}.file-field__addon,.file-field__field{cursor:pointer}.file-field__field--empty,.file-field__field--empty:focus{color:#c3c3c3}@media(min-width:576px){.fk-raw-field,.ip-field,.number-field,.password-field{max-width:360px}}.related-widget-wrapper{align-items:center;display:flex;flex-flow:wrap}.related-widget-wrapper>ul{flex-grow:1}.related-widget-wrapper>ul+.related-widget-wrapper__buttons{display:none}.related-widget-wrapper>.select-field{flex-grow:1}.related-widget-wrapper>.select-field+.related-widget-wrapper__buttons{flex-basis:100%;margin-top:.5rem}@media(min-width:576px){.related-widget-wrapper>.select-field+.related-widget-wrapper__buttons{flex-basis:auto;margin-left:.5rem;margin-top:0}}.related-widget-wrapper>.select-multiple-field{flex-grow:1}.related-widget-wrapper>.select-multiple-field+.related-widget-wrapper__buttons{flex-basis:100%;margin-top:.5rem}@media(min-width:576px){.select-field{max-width:360px}}.select-field .select2,.select-field select{width:100%}.select-date-field{display:flex}@media(min-width:576px){.select-date-field{max-width:360px}}.select-date-field .select-field{max-width:none}.select-date-field .select-field:first-of-type{flex-basis:130px;flex-grow:1;margin-right:10px}.select-date-field .select-field:nth-of-type(2){flex-basis:70px;flex-grow:1;margin-right:10px}.select-date-field .select-field:nth-of-type(3){flex-basis:80px;flex-grow:1}.multi-wrapper{border:1px solid #ccc;border-radius:3px;overflow:hidden;width:100%}.multi-wrapper .non-selected-wrapper,.multi-wrapper .selected-wrapper{box-sizing:border-box;display:inline-block;height:200px;overflow-y:scroll;padding:10px;vertical-align:top;width:50%}.multi-wrapper .non-selected-wrapper{background:#fafafa;border-right:1px solid #ccc}.multi-wrapper .selected-wrapper{background:#fff}.multi-wrapper .header{color:#4f4f4f;cursor:default;font-weight:700;margin-bottom:5px;padding:5px 10px}.multi-wrapper .item{cursor:pointer;display:block;padding:5px 10px}.multi-wrapper .item:hover{background:#ececec;border-radius:2px}.multi-wrapper .item-group{padding:5px 10px}.multi-wrapper .item-group .group-label{display:block;font-size:.875rem;opacity:.5;padding:5px 0}.multi-wrapper .search-input{border:0;border-bottom:1px solid #ccc;border-radius:0;box-sizing:border-box;display:block;font-size:1em;margin:0;outline:0;padding:10px 20px;width:100%}.multi-wrapper .non-selected-wrapper .item.selected{opacity:.5}.multi-wrapper .non-selected-wrapper .item.disabled,.multi-wrapper .selected-wrapper .item.disabled{opacity:.5;-webkit-text-decoration:line-through;text-decoration:line-through}.multi-wrapper .non-selected-wrapper .item.disabled:hover,.multi-wrapper .selected-wrapper .item.disabled:hover{background:inherit;cursor:inherit}.multi-wrapper{border-color:#d0d0d0;border-radius:.3rem;font-size:.875rem;line-height:1.375}.multi-wrapper .search-input{border-color:#d0d0d0;border-top-left-radius:.3rem;border-top-right-radius:.3rem;font-size:1rem;line-height:1.375;padding:.5rem .75rem}.multi-wrapper .search-input::placeholder{color:#c3c3c3}.multi-wrapper .non-selected-wrapper,.multi-wrapper .selected-wrapper{background-color:#fff;height:300px;padding:0}.multi-wrapper .non-selected-wrapper .item.selected,.multi-wrapper .selected-wrapper .item.selected{opacity:1}.multi-wrapper .non-selected-wrapper .item.selected{background-color:#e9ecef;color:#909090}.multi-wrapper .item{padding:.5rem .75rem;-webkit-text-decoration:none;text-decoration:none}.multi-wrapper .item:hover{background-color:#79aec8;border-radius:0;color:#fff}.multi-wrapper .item-group{padding:0}.multi-wrapper .item-group .group-label{color:gray;font-size:inherit;font-weight:500;opacity:1;padding:.5rem .75rem 0}.multi-wrapper .item-group .item{padding-left:1.25rem}.paper-widget--invalid .multi-wrapper{border-color:#df7d5c;box-shadow:0 0 0 1px #df7d5c}.split-datetime-field{display:flex}@media(min-width:576px){.split-datetime-field{max-width:360px}}.split-datetime-field .date-field{flex-basis:220px;flex-grow:1;margin-right:10px}@media(min-width:576px){.split-datetime-field .date-field{max-width:none}}.split-datetime-field .time-field{flex-basis:130px;flex-grow:1}@media(min-width:576px){.split-datetime-field .time-field{max-width:none}}.text-field textarea{max-height:200px}@media(min-width:768px){.text-field textarea{max-height:400px}}
 /*!
  * ClockPicker v{package.version} for Bootstrap (http://weareoutman.github.io/clockpicker/)
  * Copyright 2014 Wang Shenwei.
  * Licensed under MIT (https://github.com/weareoutman/clockpicker/blob/gh-pages/LICENSE)
- */.clockpicker .input-group-addon{cursor:pointer}.clockpicker-moving{cursor:move}.clockpicker-align-left.popover>.arrow{left:25px}.clockpicker-align-top.popover>.arrow{top:17px}.clockpicker-align-right.popover>.arrow{left:auto;right:25px}.clockpicker-align-bottom.popover>.arrow{bottom:6px;top:auto}.clockpicker-popover .popover-title{background-color:#fff;color:#999;font-size:24px;font-weight:700;line-height:30px;text-align:center}.clockpicker-popover .popover-title span{cursor:pointer}.clockpicker-popover .popover-content{background-color:#f8f8f8;padding:12px}.popover-content:last-child{border-bottom-left-radius:5px;border-bottom-right-radius:5px}.clockpicker-plate{-webkit-touch-callout:none;background-color:#fff;border:1px solid #ccc;border-radius:50%;height:200px;overflow:visible;position:relative;-webkit-user-select:none;user-select:none;width:200px}.clockpicker-canvas,.clockpicker-dial{height:200px;left:-1px;position:absolute;top:-1px;width:200px}.clockpicker-minutes{visibility:hidden}.clockpicker-tick{border-radius:50%;color:#666;cursor:pointer;height:26px;line-height:26px;position:absolute;text-align:center;width:26px}.clockpicker-tick.active,.clockpicker-tick:hover{background-color:#c0e5f7;background-color:rgba(0,149,221,.25)}.clockpicker-button{background-color:#fff;background-image:none;border-top-left-radius:0;border-top-right-radius:0;border-width:1px 0 0;margin:0;padding:10px 0}.clockpicker-button:hover{background-color:#ebebeb;background-image:none}.clockpicker-button:focus{outline:none!important}.clockpicker-dial{transition:transform .35s,opacity .35s}.clockpicker-dial-out{opacity:0}.clockpicker-hours.clockpicker-dial-out{transform:scale(1.2)}.clockpicker-minutes.clockpicker-dial-out{transform:scale(.8)}.clockpicker-canvas{transition:opacity 175ms}.clockpicker-canvas-out{opacity:.25}.clockpicker-canvas-bearing,.clockpicker-canvas-fg{stroke:none;fill:#0095dd}.clockpicker-canvas-bg{stroke:none;fill:#c0e5f7}.clockpicker-canvas-bg-trans{fill:rgba(0,149,221,.25)}.clockpicker-canvas line{stroke:#0095dd;stroke-width:1;stroke-linecap:round}.clockpicker-button.am-button{margin:1px}.clockpicker-button.am-button,.clockpicker-button.pm-button{border:1px solid rgba(0,0,0,.2);border-radius:4px;padding:5px}.clockpicker-button.pm-button{margin:1px 1px 1px 136px}@media(min-width:576px){.time-field{max-width:130px}}.clockpicker-popover .popover-title{border-top-left-radius:inherit;border-top-right-radius:inherit}@media(min-width:576px){.uuid-field{max-width:360px}}.btn-square{align-items:center;display:flex;font-size:.875rem;height:2.125rem;justify-content:center;line-height:1;padding:0!important;text-align:center;width:2.125rem}.btn-square.btn-lg{font-size:1rem;height:2.5rem;width:2.5rem}.btn-square.btn-sm{font-size:.875rem;height:1.875rem;width:1.875rem}.btn-square.disabled,.btn-square:disabled{opacity:1}.btn-square.disabled i,.btn-square.disabled[class*=" bi-"]:before,.btn-square.disabled[class^=bi-]:before,.btn-square:disabled i,.btn-square:disabled[class*=" bi-"]:before,.btn-square:disabled[class^=bi-]:before{opacity:.25}.btn-square--primary{color:#6060e0}.btn-square--secondary{color:#606060}.btn-square--success{color:#40b060}.btn-square--info{color:#1090c0}.btn-square--warning{color:#ffc000}.btn-square--danger{color:#d04010}.btn-square--light{color:#e9ecef}.btn-square--dark{color:#1d1d1d}.btn-square-group{display:inline-flex}.btn-square-group>.btn{border-color:#e9ecef}.btn-square-group>.btn:not(:last-child){margin-right:.125rem}.btn-square-group>.btn:focus{z-index:1}.btn-square-group>.btn:not(.disabled):hover,.btn-square-group>.btn:not(:disabled):hover{background-color:#e9ecef}.btn-square-group--table-valign{align-items:center;max-height:40px}.paper-formset__form.paper-card--primary .btn-square-group>.btn:not(.disabled):hover,.paper-formset__form.paper-card--primary .btn-square-group>.btn:not(:disabled):hover,.table-primary .btn-square-group>.btn:not(.disabled):hover,.table-primary .btn-square-group>.btn:not(:disabled):hover{background-color:#bbbbf4}.paper-formset__form.paper-card--secondary .btn-square-group>.btn:not(.disabled):hover,.paper-formset__form.paper-card--secondary .btn-square-group>.btn:not(:disabled):hover,.table-secondary .btn-square-group>.btn:not(.disabled):hover,.table-secondary .btn-square-group>.btn:not(:disabled):hover{background-color:#c8c2c2}.paper-formset__form.paper-card--success .btn-square-group>.btn:not(.disabled):hover,.paper-formset__form.paper-card--success .btn-square-group>.btn:not(:disabled):hover,.table-success .btn-square-group>.btn:not(.disabled):hover,.table-success .btn-square-group>.btn:not(:disabled):hover{background-color:#b5e4c1}.paper-formset__form.paper-card--info .btn-square-group>.btn:not(.disabled):hover,.paper-formset__form.paper-card--info .btn-square-group>.btn:not(:disabled):hover,.table-info .btn-square-group>.btn:not(.disabled):hover,.table-info .btn-square-group>.btn:not(:disabled):hover{background-color:#a5d8ea}.paper-formset__form.paper-card--warning .btn-square-group>.btn:not(.disabled):hover,.paper-formset__form.paper-card--warning .btn-square-group>.btn:not(:disabled):hover,.table-warning .btn-square-group>.btn:not(.disabled):hover,.table-warning .btn-square-group>.btn:not(:disabled):hover{background-color:#ffe79f}.paper-formset__form.paper-card--danger .btn-square-group>.btn:not(.disabled):hover,.paper-formset__form.paper-card--danger .btn-square-group>.btn:not(:disabled):hover,.table-danger .btn-square-group>.btn:not(.disabled):hover,.table-danger .btn-square-group>.btn:not(:disabled):hover{background-color:#f0b8a4}.paper-formset__form.paper-card--light .btn-square-group>.btn:not(.disabled):hover,.paper-formset__form.paper-card--light .btn-square-group>.btn:not(:disabled):hover,.table-light .btn-square-group>.btn:not(.disabled):hover,.table-light .btn-square-group>.btn:not(:disabled):hover{background-color:#e9edf2}.paper-formset__form.paper-card--dark .btn-square-group>.btn:not(.disabled):hover,.paper-formset__form.paper-card--dark .btn-square-group>.btn:not(:disabled):hover,.table-dark .btn-square-group>.btn:not(.disabled):hover,.table-dark .btn-square-group>.btn:not(:disabled):hover{background-color:#b7afaf}.delete-inline{position:relative}.delete-inline__icon{left:0;pointer-events:none;position:absolute;right:0;top:8px}.delete-inline .custom-control{position:static}.delete-inline .custom-control-label{cursor:pointer;opacity:0;transition:opacity .2s}.delete-inline .custom-control-label:after,.delete-inline .custom-control-label:before{background:transparent;border-color:transparent;transform:scale(.8181);transition:none}.delete-inline input{cursor:pointer;height:100%;left:0;opacity:0;position:absolute;top:0;width:100%;z-index:-1}.delete-inline input:focus~.custom-control-label:before{border-color:transparent!important;box-shadow:none}.delete-inline input:active~.custom-control-label:before{background:transparent;border-color:transparent!important}.delete-inline input:checked~.custom-control-label{opacity:1}.delete-inline input:checked~.custom-control-label:before{background-color:#d04010;border-color:#d04010;color:#fff}.delete-inline input:checked~.custom-control-label:after{background-image:url("data:image/svg+xml;charset=utf-8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='22' height='22'%3E%3Cpath fill='none' stroke='%23fff' stroke-linecap='round' stroke-linejoin='round' stroke-width='3' d='m4.5 12 5 5L17 6'/%3E%3C/svg%3E")}.delete-inline input:checked~.delete-inline__icon{opacity:0}.dotted-underline{text-decoration:underline;-webkit-text-decoration:underline dotted rgba(68,68,68,.75);text-decoration:underline dotted rgba(68,68,68,.75);text-decoration-thickness:.25px}.dotted-underline:hover{-webkit-text-decoration:none;text-decoration:none}.paper-breadcrumbs__list{border-bottom:1px solid #e0e5e7;border-radius:0;font-size:.8rem;padding-left:.5rem;padding-right:.5rem}@media(min-width:576px){.paper-breadcrumbs__list{padding-left:1rem;padding-right:1rem}}.paper-card{box-shadow:0 8px 12px rgba(0,0,0,.02)}.paper-card .card-header{border-top-left-radius:.25rem;border-top-right-radius:.25rem}@media(max-width:767.98px){.paper-card .card-header{padding-left:.75rem;padding-right:.75rem}}.paper-card .card-body{background:#fff}@media(max-width:767.98px){.paper-card .card-body{padding-left:.75rem;padding-right:.75rem}}.paper-card .card-body:first-child{border-top-left-radius:.25rem;border-top-right-radius:.25rem}.paper-card .card-body:last-child{border-bottom-left-radius:.25rem;border-bottom-right-radius:.25rem}.paper-card .card-subtitle{color:#444;display:block}.paper-card .card-footer{border-bottom-left-radius:.25rem;border-bottom-right-radius:.25rem}@media(max-width:767.98px){.paper-card .card-footer{padding-left:.75rem;padding-right:.75rem}}.paper-card--danger{border-color:#e78b8b}.paper-card--danger .card-header{background-color:#f4caca;border-color:#e78b8b;color:#212529}.paper-card--danger .card-footer{border-color:#e78b8b}.paper-card--warning{border-color:#e9e92f}.paper-card--warning .card-header{background-color:#fafad0;border-color:#e9e92f;color:#212529}.paper-card--warning .card-footer{border-color:#e9e92f}.paper-card--info{border-color:#96badd}.paper-card--info .card-header{background-color:#d0e0f0;border-color:#96badd;color:#212529}.paper-card--info .card-footer{border-color:#96badd}.paper-card--success{border-color:#8edf8e}.paper-card--success .card-header{background-color:#caf0ca;border-color:#8edf8e;color:#212529}.paper-card--success .card-footer{border-color:#8edf8e}.paper-card--primary{border-color:#6dc9f7}.paper-card--primary .card-header{background-color:#b6e4fb;border-color:#6dc9f7;color:#212529}.paper-card--primary .card-footer{border-color:#6dc9f7}.paper-card--secondary{border-color:#c4c4c4}.paper-card--secondary .card-header{background-color:#eaeaea;border-color:#c4c4c4;color:#212529}.paper-card--secondary .card-footer{border-color:#c4c4c4}.paper-dropzone{min-height:50px;position:relative}.paper-dropzone__overlay{background:rgba(250,226,72,.65);border-radius:.25rem;box-sizing:content-box;height:100%;left:-5px;opacity:0;padding:5px;position:absolute;text-align:center;top:-5px;transition:opacity .1s,background .1s,z-index 0s .1s;width:100%;z-index:-1}.on-drag-file .paper-dropzone__overlay,.ondrag .paper-dropzone__overlay{opacity:1;transition:opacity .1s,background .1s,z-index 0s 0s;z-index:1}.paper-dropzone__overlay--highlighted{background-color:rgba(160,160,255,.65)}.paper-dropzone__hint{left:50%;position:absolute;top:50%;transform:translate(-50%,-50%)}.dz-default{display:none}.paper-environment{background:var(--bg-color);border-bottom:1px solid #333;font-size:.625rem;line-height:1.375;margin-bottom:0;padding:.125rem .75rem;text-align:center;text-transform:uppercase}.paper-error-list{list-style:none;margin:0;padding:0}.paper-error-list.invalid-feedback{margin-top:.25rem}.paper-error-list.invalid-tooltip{margin-top:2px;padding:.25rem .5rem}.paper-error-list:empty{display:none!important}.paper-error-list li:before{content:"• "}.paper-form__label--required:after,.paper-form__row--required .paper-form__label:after{color:#d04010;content:"*";display:inline-block;font-weight:700;margin-left:.125em;position:relative;top:-.2em}.paper-form__label{color:#444;cursor:pointer;font-size:.875rem;font-weight:300;line-height:1.375rem;margin-bottom:0;transition:color .2s}@media(prefers-reduced-motion:reduce){.paper-form__label{transition:none}}@media(max-width:767.98px){.paper-form__label{margin-bottom:.375rem}}.paper-form__label:hover{color:#212529}.paper-form__row{background-color:#fff;padding:.75rem 1rem}@media(max-width:767.98px){.paper-form__row{padding-left:.75rem;padding-right:.75rem}}.paper-form__row:not(:first-of-type){border-top:1px dashed #e9ecef}.paper-card .paper-form__row:last-child{border-bottom-left-radius:inherit;border-bottom-right-radius:inherit}.paper-card>.card-body:first-of-type .paper-form__row:first-child{border-top-left-radius:inherit;border-top-right-radius:inherit}.paper-card>.card-header:first-of-type+.card-body .paper-form__row:first-child{border-top-left-radius:0;border-top-right-radius:0}.paper-form__row--readonly .readonly{font-size:1rem;word-break:break-word}.paper-form__row--invalid{background-color:#ffe0e0}.paper-header{-webkit-backface-visibility:hidden;backface-visibility:hidden;background:#fff;box-shadow:0 0 1px 1px #e0e5e7;min-height:2.75rem;z-index:1021}.paper-header .navbar{box-sizing:content-box;min-height:30px}.paper-header .navbar-nav{margin-right:-.375rem}.paper-header .nav-item{margin-right:.375rem}.paper-header .nav-link{border-radius:.25rem;color:#333;font-size:.875rem;line-height:1.5714285714;min-width:30px;padding-bottom:.25rem;padding-top:.25rem;text-align:center}.paper-header .nav-link:hover,.paper-header .nav-link[aria-expanded=true]{background-color:#e9ecef;color:#6060e0}.paper-header .nav-link:focus{box-shadow:0 0 0 2px #444;outline:0}.paper-header__burger{min-width:32px;text-align:center}.paper-header__burger:hover{color:#1090c0}.paper-header__burger i{display:inline-block;transform:scale(1.75)}.paper-input-group a.input-group-text{background:#f8f9fa;color:#9a9a9a;justify-content:center;min-width:2.25rem}.paper-input-group a.input-group-text:focus{position:relative;z-index:1}.paper-input-group a.input-group-text:hover{color:#9a9a9a;-webkit-text-decoration:none;text-decoration:none}.paper-input-group a.input-group-text[href]{color:#7575e4}.paper-input-group a.input-group-text[href]:not(.disabled):hover{background:#e9ecef;color:#6060e0}.paper-input-group a.input-group-text.disabled{background:#f8f9fa;color:#9a9a9a;cursor:default}.paper-input-group button.input-group-text{background:#f8f9fa;color:#7575e4;justify-content:center;min-width:2.25rem}.paper-input-group button.input-group-text:focus{position:relative;z-index:1}.paper-input-group button.input-group-text:hover{background-color:#e9ecef;color:#6060e0}.paper-input-group button.input-group-text.disabled,.paper-input-group button.input-group-text:disabled{background-color:#f8f9fa;color:#9a9a9a;cursor:default}.paper-input-group label.input-group-text{background-color:#f8f9fa;color:#9a9a9a;justify-content:center;min-width:2.25rem}.paper-input-group label.input-group-text:focus{position:relative;z-index:1}.paper-input-group label.input-group-text:hover{color:#9a9a9a;-webkit-text-decoration:none;text-decoration:none}.paper-input-group label.input-group-text[for]{color:#7575e4}.paper-input-group label.input-group-text[for]:not(.disabled):hover{background-color:#e9ecef;color:#6060e0}.paper-input-group label.input-group-text.disabled{background-color:#f8f9fa;color:#9a9a9a;cursor:default}.paper-input-group a.input-group-text--primary[href]{color:#7575e4}.paper-input-group a.input-group-text--primary[href]:not(.disabled):hover{color:#6060e0}.paper-input-group button.input-group-text--primary{color:#7575e4}.paper-input-group button.input-group-text--primary:not(.disabled):not(:disabled):hover{color:#6060e0}.paper-input-group label.input-group-text--primary[for]{color:#7575e4}.paper-input-group label.input-group-text--primary[for]:not(.disabled):hover{color:#6060e0}.paper-input-group a.input-group-text--secondary[href]{color:#6d6d6d}.paper-input-group a.input-group-text--secondary[href]:not(.disabled):hover{color:#606060}.paper-input-group button.input-group-text--secondary{color:#6d6d6d}.paper-input-group button.input-group-text--secondary:not(.disabled):not(:disabled):hover{color:#606060}.paper-input-group label.input-group-text--secondary[for]{color:#6d6d6d}.paper-input-group label.input-group-text--secondary[for]:not(.disabled):hover{color:#606060}.paper-input-group a.input-group-text--success[href]{color:#4cbe6c}.paper-input-group a.input-group-text--success[href]:not(.disabled):hover{color:#40b060}.paper-input-group button.input-group-text--success{color:#4cbe6c}.paper-input-group button.input-group-text--success:not(.disabled):not(:disabled):hover{color:#40b060}.paper-input-group label.input-group-text--success[for]{color:#4cbe6c}.paper-input-group label.input-group-text--success[for]:not(.disabled):hover{color:#40b060}.paper-input-group a.input-group-text--info[href]{color:#12a2d8}.paper-input-group a.input-group-text--info[href]:not(.disabled):hover{color:#1090c0}.paper-input-group button.input-group-text--info{color:#12a2d8}.paper-input-group button.input-group-text--info:not(.disabled):not(:disabled):hover{color:#1090c0}.paper-input-group label.input-group-text--info[for]{color:#12a2d8}.paper-input-group label.input-group-text--info[for]:not(.disabled):hover{color:#1090c0}.paper-input-group a.input-group-text--warning[href]{color:#ffc61a}.paper-input-group a.input-group-text--warning[href]:not(.disabled):hover{color:#ffc000}.paper-input-group button.input-group-text--warning{color:#ffc61a}.paper-input-group button.input-group-text--warning:not(.disabled):not(:disabled):hover{color:#ffc000}.paper-input-group label.input-group-text--warning[for]{color:#ffc61a}.paper-input-group label.input-group-text--warning[for]:not(.disabled):hover{color:#ffc000}.paper-input-group a.input-group-text--danger[href]{color:#e84712}.paper-input-group a.input-group-text--danger[href]:not(.disabled):hover{color:#d04010}.paper-input-group button.input-group-text--danger{color:#e84712}.paper-input-group button.input-group-text--danger:not(.disabled):not(:disabled):hover{color:#d04010}.paper-input-group label.input-group-text--danger[for]{color:#e84712}.paper-input-group label.input-group-text--danger[for]:not(.disabled):hover{color:#d04010}.paper-input-group a.input-group-text--light[href]{color:#f8f9fa}.paper-input-group a.input-group-text--light[href]:not(.disabled):hover{color:#e9ecef}.paper-input-group button.input-group-text--light{color:#f8f9fa}.paper-input-group button.input-group-text--light:not(.disabled):not(:disabled):hover{color:#e9ecef}.paper-input-group label.input-group-text--light[for]{color:#f8f9fa}.paper-input-group label.input-group-text--light[for]:not(.disabled):hover{color:#e9ecef}.paper-input-group a.input-group-text--dark[href]{color:#2a2a2a}.paper-input-group a.input-group-text--dark[href]:not(.disabled):hover{color:#1d1d1d}.paper-input-group button.input-group-text--dark{color:#2a2a2a}.paper-input-group button.input-group-text--dark:not(.disabled):not(:disabled):hover{color:#1d1d1d}.paper-input-group label.input-group-text--dark[for]{color:#2a2a2a}.paper-input-group label.input-group-text--dark[for]:not(.disabled):hover{color:#1d1d1d}.paper-messages{list-style:none;margin:0;padding:0}.paper-messages:empty{display:none}.paper-message{background-position:6.375px .75rem;background-repeat:no-repeat;background-size:1.203125rem 1.203125rem;border-radius:0 3px 3px 0;border-style:solid;border-width:1px 1px 1px 8px;font-size:.875rem;line-height:1.375;padding:.75rem 2rem}.paper-message:not(:first-child){margin-top:.5rem}.paper-message--error{background-color:#f4caca;background-image:url("data:image/svg+xml;charset=utf-8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='225' height='225'%3E%3Ccircle cx='112.5' cy='112.5' r='92.5' fill='none' stroke='%23d04010' stroke-linejoin='round' stroke-width='20'/%3E%3Cpath fill='%23d04010' stroke='%23d04010' stroke-linecap='round' stroke-linejoin='round' stroke-width='20' d='M115 120.86v-57h-5v57z'/%3E%3Ccircle cx='112.5' cy='157.5' r='12.5' fill='%23d04010'/%3E%3C/svg%3E");border-color:#e78b8b}.paper-message--warning{background-color:#fafad0;background-image:url("data:image/svg+xml;charset=utf-8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='225' height='225'%3E%3Cpath fill='none' stroke='%23ffc000' stroke-linejoin='round' stroke-width='20' d='M215.17 205.17H9.83L112.5 19.83z'/%3E%3Cpath fill='%23ffc000' stroke='%23ffc000' stroke-linecap='round' stroke-linejoin='round' stroke-width='20' d='M110 123v57h5v-57z'/%3E%3Ccircle cx='112.5' cy='86.36' r='12.5' fill='%23ffc000'/%3E%3C/svg%3E");border-color:#e9e92f}.paper-message--debug,.paper-message--info{background-color:#d0e0f0;background-image:url("data:image/svg+xml;charset=utf-8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='225' height='225'%3E%3Ccircle cx='112.5' cy='112.5' r='92.5' fill='none' stroke='%231090c0' stroke-linejoin='round' stroke-width='20'/%3E%3Cpath fill='%231090c0' stroke='%231090c0' stroke-linecap='round' stroke-linejoin='round' stroke-width='20' d='M110 103v57h5v-57z'/%3E%3Ccircle cx='112.5' cy='66.36' r='12.5' fill='%231090c0'/%3E%3C/svg%3E");border-color:#96badd}.paper-message--success{background-color:#caf0ca;background-image:url("data:image/svg+xml;charset=utf-8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='225' height='225'%3E%3Cpath fill='none' stroke='%2340b060' stroke-linecap='round' stroke-linejoin='round' stroke-width='22' d='m68.71 110.45 36.42 36.41 59.75-59.75'/%3E%3Ccircle cx='112.5' cy='112.5' r='92.5' fill='none' stroke='%2340b060' stroke-linejoin='round' stroke-width='20'/%3E%3C/svg%3E");border-color:#8edf8e}.paper-modal-backdrop{opacity:0}.paper-modal .modal-header{padding:.75rem 1rem}.paper-modal .modal-header:empty{display:none}.paper-modal .modal-title{font-size:1.25rem;line-height:1.25}.paper-modal .modal-body{padding:1rem}.paper-modal .modal-footer{padding:.5rem .75rem}.paper-modal .modal-footer:empty{display:none}.paper-modal .close{align-self:stretch;margin:-.75rem -1rem -.75rem auto;padding:0 1rem}.paper-modal--preloader .paper-preloader{margin:10px auto 20px}.paper-modal--danger .modal-content{border-color:#e78b8b}.paper-modal--danger .modal-header{background-color:#f4caca;border-color:#e78b8b;color:#212529}.paper-modal--warning .modal-content{border-color:#e9e92f}.paper-modal--warning .modal-header{background-color:#fafad0;border-color:#e9e92f;color:#212529}.paper-modal--info .modal-content{border-color:#96badd}.paper-modal--info .modal-header{background-color:#d0e0f0;border-color:#96badd;color:#212529}.paper-modal--success .modal-content{border-color:#8edf8e}.paper-modal--success .modal-header{background-color:#caf0ca;border-color:#8edf8e;color:#212529}.paper-modal--primary .modal-content{border-color:#6dc9f7}.paper-modal--primary .modal-header{background-color:#b6e4fb;border-color:#6dc9f7;color:#212529}.paper-modal--secondary .modal-content{border-color:#c4c4c4}.paper-modal--secondary .modal-header{background-color:#eaeaea;border-color:#c4c4c4;color:#212529}.paper-object-list{padding-left:.5rem}.paper-object-list ul{margin-top:.125rem;padding-left:1.375rem}.paper-object-list li{list-style-position:inside}.paper-object-list li:not(:first-child){margin-top:.125rem}.paper-page.js{transition:margin-left .5s}@media(min-width:1200px)and (min-width:0){body:not(.popup) .paper-page{margin-left:14rem}}@media(min-width:1200px)and (min-width:1280px){body:not(.popup) .paper-page{margin-left:16rem}}.paper-page__header h1{font-size:1.5rem;margin-bottom:0}.paper-page__toolbar{display:none}@media(min-width:992px){.paper-page__toolbar{display:block}}@media(min-width:0){.paper-page__toolbar{width:14rem}}@media(min-width:1280px){.paper-page__toolbar{width:15rem}}.paper-page__toolbar:empty{display:none}@keyframes pulse{0%{opacity:1}to{opacity:.5}}@keyframes load{0%{transform:rotate(-35deg)}18%{border-width:6px}50%{border-width:3px}82%{border-width:6px}to{transform:rotate(215deg)}}.paper-preloader{height:70px;overflow:hidden;position:relative;width:140px}.paper-preloader:before{animation:load .9s ease-in-out infinite alternate;border:8px solid transparent;border-left-color:#6060e0;border-radius:50%;content:"";height:200%;position:absolute;width:100%}.paper-preloader__text{animation:pulse .75s linear infinite alternate;bottom:0;font-size:18px;left:0;position:absolute;text-align:center;text-transform:uppercase;width:100%}.sidebar-shadow{background:rgba(0,0,0,.33);height:100%;left:0;opacity:0;position:fixed;top:0;transition:all .5s,visibility .5s 0s;visibility:hidden;width:100%;z-index:1029}@media(min-width:1200px){.sidebar-shadow{display:none}}.sidebar-open .sidebar-shadow{opacity:1;transition:all .5s,visibility 0s 0s;visibility:visible}.paper-sidebar{background:url(/static/paper_admin/dist/assets/menu_bg.jpg);box-shadow:0 0 5px rgba(0,0,0,.66);height:100vh;left:0;position:fixed;top:0;transform:translate(-102%);transition:transform .5s;will-change:transform;z-index:1030}@media(min-width:1200px){.paper-sidebar{transform:translate(0)}}@media(min-width:0){.paper-sidebar{width:14rem}}@media(min-width:1280px){.paper-sidebar{width:16rem}}.sidebar-open .paper-sidebar{transform:translate(0)}.paper-sidebar .navbar{height:100%}.paper-sidebar .navbar-brand{border-bottom:1px solid #333;min-height:2.875rem;padding:.5rem .75rem}.paper-sidebar .navbar-brand-name{color:#fff;font-size:1.125rem;word-break:break-word}.paper-sidebar__menu{margin-top:10px;overflow-y:auto}.paper-sidebar__item-list{background:#101010}.paper-sidebar__item-list--level-1{background:transparent;margin-bottom:20px}.paper-sidebar__item-list--level-2{border-bottom:1px solid #444;position:relative}.paper-sidebar__item-list--level-2:before{background:#444;content:"";height:100%;left:22px;position:absolute;top:0;width:1px;z-index:1}.paper-sidebar__link{align-items:baseline;color:inherit;display:flex;font-size:.875rem;line-height:1.375;padding:.5rem .75rem;transition:all .2s ease-in-out;word-break:break-word}@media(prefers-reduced-motion:reduce){.paper-sidebar__link{transition:none}}.paper-sidebar__link:focus,.paper-sidebar__link:hover{background:hsla(0,0%,100%,.1);color:#fff;outline:none;-webkit-text-decoration:none;text-decoration:none}.paper-sidebar__link>i{flex:0 0 20px;line-height:1;margin-right:.375rem;text-align:left}.active>.paper-sidebar__link{background:rgba(172,172,239,.7);color:#fff}.paper-sidebar__link--trigger{padding-right:34px;position:relative}.paper-sidebar__link--trigger:after{content:"";font:.625rem bootstrap-icons;position:absolute;right:.75rem;top:calc(50% - .375rem);transform:rotate(-90deg);transition:all .2s ease-in-out}@media(prefers-reduced-motion:reduce){.paper-sidebar__link--trigger:after{transition:none}}.paper-sidebar__link--trigger[aria-expanded=true]:after{transform:rotate(0deg)}.paper-sidebar__item{color:hsla(0,0%,100%,.8)}.paper-sidebar__item--level-1{padding-left:0}.paper-sidebar__item--level-1>.paper-sidebar__link>i{font-size:inherit;transform:scale(1.3) translate(5%,-5%)}.paper-sidebar__item--level-1>.paper-sidebar__link:hover{background:hsla(0,0%,100%,.1)}.paper-sidebar__item--level-2{padding-left:22px;position:relative}.paper-sidebar__item--level-2>.paper-sidebar__link:before{background:#101010;border:1px solid #444;border-radius:50%;content:"";height:7px;left:22px;position:absolute;top:17.625px;transform:translate(-3px,-50%);transition:all .2s ease-in-out;width:7px;z-index:1}@media(prefers-reduced-motion:reduce){.paper-sidebar__item--level-2>.paper-sidebar__link:before{transition:none}}.paper-sidebar__item--level-2>.paper-sidebar__link.paper-sidebar__link--trigger:before{left:0}.paper-sidebar__item--level-2>.paper-sidebar__link:focus:before,.paper-sidebar__item--level-2>.paper-sidebar__link:hover:before{background:#acacef}.paper-sidebar__item--level-2.active>.paper-sidebar__link:before{content:none}.paper-sidebar__item--level-2.open>.paper-sidebar__link:before{background:#acacef}.paper-sidebar__item--level-3>.paper-sidebar__divider,.paper-sidebar__item--level-3>.paper-sidebar__link,.paper-sidebar__item--level-4>.paper-sidebar__divider,.paper-sidebar__item--level-4>.paper-sidebar__link{padding-left:24px}.paper-sidebar__divider{background-color:#444;height:1px;padding:0 .75rem}.paper-sidebar__group{color:#606060;font-size:11px;letter-spacing:1px;margin:1.25em 0 .5em;padding:0 .75rem;text-transform:uppercase}.paper-table{background-color:#fff;border:1px solid #e0e5e7;border-collapse:separate;border-radius:.25rem;border-spacing:0;box-shadow:0 8px 12px rgba(0,0,0,.02);vertical-align:top}.paper-table__small-column{width:.1%}.paper-table__sort-button{border-radius:.125rem;color:#606060;font-size:inherit;margin:0 0 0 .125rem;padding:.125rem .375rem;vertical-align:baseline}.paper-table__sort-button--has-prior{padding-right:.6em}.paper-table__sort-button span{font-size:75%;margin-left:.125rem!important}.paper-table__sortable-cell{position:relative;width:1.25rem}.paper-table__sort-handler{align-items:center;background:url(/static/paper_admin/dist/assets/sortable.svg) repeat-y center 5px;background-clip:content-box;background-size:contain;border-right:1px solid #e0e5e7;bottom:0;color:#c3c3c3;cursor:move;display:flex;justify-content:center;left:0;padding:5px 0;position:absolute;right:0;top:0;transition:color .3s}.paper-table__sort-handler.disabled{color:#e9ecef}.paper-table__sort-handler.disabled,tr.disabled .paper-table__sort-handler{cursor:default}tr:not(.disabled) .paper-table__sort-handler:not(.disabled):hover{color:#333}.paper-table td,.paper-table th{border-top:none;padding:.5rem;vertical-align:middle}.paper-table .action-checkbox,.paper-table .action-checkbox-column{padding-right:.25rem}.paper-table td:first-child,.paper-table th:first-child{padding-left:.75rem}.paper-table td:last-child,.paper-table th:last-child{padding-right:.75rem}.paper-table thead th{border-bottom:1px solid #dadada;color:#333;font-size:.75rem;font-weight:500;padding:.5rem;text-transform:uppercase;vertical-align:middle}.paper-table thead th:first-child{border-top-left-radius:.25rem}.paper-table thead th:last-child{border-top-right-radius:.25rem}.paper-table thead th a{color:inherit}.paper-table thead th .dropdown-item{text-transform:none}.paper-table tfoot td{border-top:1px solid #dadada}.paper-table tbody th{font-weight:400}.paper-table tbody tr.selected td,.paper-table tbody tr.selected th{background-color:#fff7e0}.paper-table tbody tr:not(:last-child) td,.paper-table tbody tr:not(:last-child) th{border-bottom:1px solid #e9ecef}.paper-table tbody tr.table-danger td,.paper-table tbody tr.table-danger th,.paper-table--danger thead th{background-color:#f4caca;border-color:#e78b8b}.paper-table tbody tr.table-danger:hover td,.paper-table tbody tr.table-danger:hover th{background-color:#f1bdbd}.paper-table tbody tr.table-warning td,.paper-table tbody tr.table-warning th,.paper-table--warning thead th{background-color:#fafad0;border-color:#e9e92f}.paper-table tbody tr.table-warning:hover td,.paper-table tbody tr.table-warning:hover th{background-color:#f9f9c2}.paper-table tbody tr.table-info td,.paper-table tbody tr.table-info th,.paper-table--info thead th{background-color:#d0e0f0;border-color:#96badd}.paper-table tbody tr.table-info:hover td,.paper-table tbody tr.table-info:hover th{background-color:#c4d8ec}.paper-table tbody tr.table-success td,.paper-table tbody tr.table-success th,.paper-table--success thead th{background-color:#caf0ca;border-color:#8edf8e}.paper-table tbody tr.table-success:hover td,.paper-table tbody tr.table-success:hover th{background-color:#beedbe}.paper-table tbody tr.table-primary td,.paper-table tbody tr.table-primary th,.paper-table--primary thead th{background-color:#b6e4fb;border-color:#6dc9f7}.paper-table tbody tr.table-primary:hover td,.paper-table tbody tr.table-primary:hover th{background-color:#a7dffa}.paper-table tbody tr.table-secondary td,.paper-table tbody tr.table-secondary th,.paper-table--secondary thead th{background-color:#eaeaea;border-color:#c4c4c4}.paper-table tbody tr.table-secondary:hover td,.paper-table tbody tr.table-secondary:hover th{background-color:#e2e2e2}.paper-table--sortable tbody tr{transition:opacity .1s,background-color .3s}.paper-table--sortable tbody tr.sortable-ghost{background-color:#fff2cc!important}.paper-table--sortable tbody tr.disabled{opacity:.3}@media(max-width:767.98px){.paper-widget--checkbox>.custom-control{display:inline-block;vertical-align:top}}.paper-widget--invalid~.invalid-feedback,.paper-widget--invalid~.invalid-tooltip{display:block}.paper-widget--invalid .custom-file-label,.paper-widget--invalid .form-control{border-color:#df7d5c;box-shadow:0 0 0 1px #df7d5c}.paper-widget--invalid .form-control:focus{border-color:#444;box-shadow:0 0 0 1px #444}.paper-widget--invalid .form-control{background-image:url("data:image/svg+xml;charset=utf-8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='12' height='12' fill='none' stroke='%23d04010'%3E%3Ccircle cx='6' cy='6' r='4.5'/%3E%3Cpath stroke-linejoin='round' d='M5.8 3.6h.4L6 6.5z'/%3E%3Ccircle cx='6' cy='8.2' r='.6' fill='%23d04010' stroke='none'/%3E%3C/svg%3E");background-position:right .375rem center;background-repeat:no-repeat;background-size:calc(.6875em + .375rem) calc(.6875em + .375rem);padding-right:calc(.6875em + 1.125rem)}@keyframes form_appear{0%{opacity:0;top:-5vh}to{opacity:1;top:0}}.login{background:url(/static/paper_admin/dist/assets/login_bg.jpg) bottom;background-size:cover}.login:before{background:rgba(0,0,0,.5);bottom:0;content:"";left:0;position:absolute;right:0;top:0;z-index:-1}.login .paper-page{margin-left:0!important}.login-card{animation:form_appear .8s .4s backwards;border-radius:.25rem;max-width:100%;position:relative;width:320px}.password-reset-link a{color:inherit}.paper-actions{align-items:center;display:flex;flex:1 1 auto;flex-wrap:wrap}.paper-actions__action{padding:1px 0}.paper-actions__action select{max-width:340px;min-width:180px;padding-left:.375rem;padding-right:24px;width:auto}.paper-actions__select_across{display:none}.paper-actions__button{margin-right:1rem}.paper-actions__tools{flex:1 0 auto;padding:.375rem 0}.paper-actions__all,.paper-actions__counter{margin-right:.375rem}.paper-actions__clear,.paper-actions__question{margin-left:.375rem}.paper-filter{margin-bottom:.75rem}.paper-filter:not(:first-child){border-top:1px dashed #e9ecef;padding-top:.75rem}.paper-filter__title{font-size:1rem;font-weight:300}.paper-search-form{width:15rem}.paper-search-form__field{position:relative}.paper-search-form__icon{color:#9a9a9a;left:.5rem;line-height:1.375;position:absolute;top:.375rem}.paper-search-form .form-control{padding-left:1.75rem}.paper-search-form .form-control::-webkit-search-cancel-button{-webkit-appearance:none;background:no-repeat url(/static/paper_admin/dist/assets/cross.svg) 50%;cursor:pointer;height:1em;margin:0;width:1em}#result_list .related-widget-wrapper__buttons{display:none}.paper-formset:not(:first-child){margin-top:1.5rem}.paper-formset__form{overflow:hidden}.paper-formset--tabular .paper-formset__form--invalid{background-color:#ffe0e0}.paper-formset--tabular thead th{padding-bottom:.5rem}.paper-tabs{position:relative}.paper-tabs__underline{background-color:#1090c0;height:2px;position:absolute;transition:all .2s}.paper-tabs .nav{display:flex;margin-left:-.375rem;margin-right:-.375rem}.paper-tabs .nav-item{margin-bottom:.375rem;margin-right:.5rem}.paper-tabs .nav-link{color:#606060;font-size:1rem;font-weight:300;padding:.25rem .375rem}.paper-tabs .active,.paper-tabs .nav-link:hover{color:#6060e0}@keyframes arrow{0%{top:.875rem}25%{top:.625rem}75%{top:1.125rem}to{top:.875rem}}.scroll-top-button{align-items:center;background-color:#40b060;border-radius:50%;bottom:2rem;box-shadow:0 2px 6px rgba(0,0,0,.4);cursor:pointer;display:none;font-size:1rem;height:3rem;justify-content:center;opacity:.75;position:fixed;right:1rem;transform:scale(0);transition:all .2s ease-in-out;width:3rem;will-change:transform;z-index:1020}@media(prefers-reduced-motion:reduce){.scroll-top-button{transition:none}}@media(min-width:992px){.scroll-top-button{bottom:2.75rem;display:flex!important;right:2rem}}.scroll-top-button i{-webkit-backface-visibility:hidden;backface-visibility:hidden;color:#fff;will-change:top}.scroll-top-button.show{transform:scale(1)}.scroll-top-button:hover{opacity:1}.scroll-top-button:hover i{animation:arrow 2s linear infinite}.custom-select[multiple]{height:40px}
+ */.clockpicker .input-group-addon{cursor:pointer}.clockpicker-moving{cursor:move}.clockpicker-align-left.popover>.arrow{left:25px}.clockpicker-align-top.popover>.arrow{top:17px}.clockpicker-align-right.popover>.arrow{left:auto;right:25px}.clockpicker-align-bottom.popover>.arrow{bottom:6px;top:auto}.clockpicker-popover .popover-title{background-color:#fff;color:#999;font-size:24px;font-weight:700;line-height:30px;text-align:center}.clockpicker-popover .popover-title span{cursor:pointer}.clockpicker-popover .popover-content{background-color:#f8f8f8;padding:12px}.popover-content:last-child{border-bottom-left-radius:5px;border-bottom-right-radius:5px}.clockpicker-plate{-webkit-touch-callout:none;background-color:#fff;border:1px solid #ccc;border-radius:50%;height:200px;overflow:visible;position:relative;-webkit-user-select:none;user-select:none;width:200px}.clockpicker-canvas,.clockpicker-dial{height:200px;left:-1px;position:absolute;top:-1px;width:200px}.clockpicker-minutes{visibility:hidden}.clockpicker-tick{border-radius:50%;color:#666;cursor:pointer;height:26px;line-height:26px;position:absolute;text-align:center;width:26px}.clockpicker-tick.active,.clockpicker-tick:hover{background-color:#c0e5f7;background-color:rgba(0,149,221,.25)}.clockpicker-button{background-color:#fff;background-image:none;border-top-left-radius:0;border-top-right-radius:0;border-width:1px 0 0;margin:0;padding:10px 0}.clockpicker-button:hover{background-color:#ebebeb;background-image:none}.clockpicker-button:focus{outline:none!important}.clockpicker-dial{transition:transform .35s,opacity .35s}.clockpicker-dial-out{opacity:0}.clockpicker-hours.clockpicker-dial-out{transform:scale(1.2)}.clockpicker-minutes.clockpicker-dial-out{transform:scale(.8)}.clockpicker-canvas{transition:opacity 175ms}.clockpicker-canvas-out{opacity:.25}.clockpicker-canvas-bearing,.clockpicker-canvas-fg{stroke:none;fill:#0095dd}.clockpicker-canvas-bg{stroke:none;fill:#c0e5f7}.clockpicker-canvas-bg-trans{fill:rgba(0,149,221,.25)}.clockpicker-canvas line{stroke:#0095dd;stroke-width:1;stroke-linecap:round}.clockpicker-button.am-button{margin:1px}.clockpicker-button.am-button,.clockpicker-button.pm-button{border:1px solid rgba(0,0,0,.2);border-radius:4px;padding:5px}.clockpicker-button.pm-button{margin:1px 1px 1px 136px}@media(min-width:576px){.time-field{max-width:130px}}.clockpicker-popover .popover-title{border-top-left-radius:inherit;border-top-right-radius:inherit}@media(min-width:576px){.uuid-field{max-width:360px}}.btn-square{align-items:center;display:flex;font-size:.875rem;height:2.125rem;justify-content:center;line-height:1;padding:0!important;text-align:center;width:2.125rem}.btn-square.btn-lg{font-size:1rem;height:2.5rem;width:2.5rem}.btn-square.btn-sm{font-size:.875rem;height:1.875rem;width:1.875rem}.btn-square.disabled,.btn-square:disabled{opacity:1}.btn-square.disabled i,.btn-square.disabled[class*=" bi-"]:before,.btn-square.disabled[class^=bi-]:before,.btn-square:disabled i,.btn-square:disabled[class*=" bi-"]:before,.btn-square:disabled[class^=bi-]:before{opacity:.25}.btn-square--primary{color:#6060e0}.btn-square--secondary{color:#606060}.btn-square--success{color:#40b060}.btn-square--info{color:#1090c0}.btn-square--warning{color:#ffc000}.btn-square--danger{color:#d04010}.btn-square--light{color:#e9ecef}.btn-square--dark{color:#1d1d1d}.btn-square-group{display:inline-flex}.btn-square-group>.btn{border-color:#e9ecef}.btn-square-group>.btn:not(:last-child){margin-right:.125rem}.btn-square-group>.btn:focus{z-index:1}.btn-square-group>.btn:not(.disabled):hover,.btn-square-group>.btn:not(:disabled):hover{background-color:#e9ecef}.btn-square-group--table-valign{align-items:center;max-height:40px}.paper-formset__form.paper-card--primary .btn-square-group>.btn:not(.disabled):hover,.paper-formset__form.paper-card--primary .btn-square-group>.btn:not(:disabled):hover,.table-primary .btn-square-group>.btn:not(.disabled):hover,.table-primary .btn-square-group>.btn:not(:disabled):hover{background-color:#bbbbf4}.paper-formset__form.paper-card--secondary .btn-square-group>.btn:not(.disabled):hover,.paper-formset__form.paper-card--secondary .btn-square-group>.btn:not(:disabled):hover,.table-secondary .btn-square-group>.btn:not(.disabled):hover,.table-secondary .btn-square-group>.btn:not(:disabled):hover{background-color:#c8c2c2}.paper-formset__form.paper-card--success .btn-square-group>.btn:not(.disabled):hover,.paper-formset__form.paper-card--success .btn-square-group>.btn:not(:disabled):hover,.table-success .btn-square-group>.btn:not(.disabled):hover,.table-success .btn-square-group>.btn:not(:disabled):hover{background-color:#b5e4c1}.paper-formset__form.paper-card--info .btn-square-group>.btn:not(.disabled):hover,.paper-formset__form.paper-card--info .btn-square-group>.btn:not(:disabled):hover,.table-info .btn-square-group>.btn:not(.disabled):hover,.table-info .btn-square-group>.btn:not(:disabled):hover{background-color:#a5d8ea}.paper-formset__form.paper-card--warning .btn-square-group>.btn:not(.disabled):hover,.paper-formset__form.paper-card--warning .btn-square-group>.btn:not(:disabled):hover,.table-warning .btn-square-group>.btn:not(.disabled):hover,.table-warning .btn-square-group>.btn:not(:disabled):hover{background-color:#ffe79f}.paper-formset__form.paper-card--danger .btn-square-group>.btn:not(.disabled):hover,.paper-formset__form.paper-card--danger .btn-square-group>.btn:not(:disabled):hover,.table-danger .btn-square-group>.btn:not(.disabled):hover,.table-danger .btn-square-group>.btn:not(:disabled):hover{background-color:#f0b8a4}.paper-formset__form.paper-card--light .btn-square-group>.btn:not(.disabled):hover,.paper-formset__form.paper-card--light .btn-square-group>.btn:not(:disabled):hover,.table-light .btn-square-group>.btn:not(.disabled):hover,.table-light .btn-square-group>.btn:not(:disabled):hover{background-color:#e9edf2}.paper-formset__form.paper-card--dark .btn-square-group>.btn:not(.disabled):hover,.paper-formset__form.paper-card--dark .btn-square-group>.btn:not(:disabled):hover,.table-dark .btn-square-group>.btn:not(.disabled):hover,.table-dark .btn-square-group>.btn:not(:disabled):hover{background-color:#b7afaf}.delete-inline{position:relative}.delete-inline__icon{left:0;pointer-events:none;position:absolute;right:0;top:8px}.delete-inline .custom-control{position:static}.delete-inline .custom-control-label{cursor:pointer;opacity:0;transition:opacity .2s}.delete-inline .custom-control-label:after,.delete-inline .custom-control-label:before{background:transparent;border-color:transparent;transform:scale(.8181);transition:none}.delete-inline input{cursor:pointer;height:100%;left:0;opacity:0;position:absolute;top:0;width:100%;z-index:-1}.delete-inline input:focus~.custom-control-label:before{border-color:transparent!important;box-shadow:none}.delete-inline input:active~.custom-control-label:before{background:transparent;border-color:transparent!important}.delete-inline input:checked~.custom-control-label{opacity:1}.delete-inline input:checked~.custom-control-label:before{background-color:#d04010;border-color:#d04010;color:#fff}.delete-inline input:checked~.custom-control-label:after{background-image:url("data:image/svg+xml;charset=utf-8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='22' height='22'%3E%3Cpath fill='none' stroke='%23fff' stroke-linecap='round' stroke-linejoin='round' stroke-width='3' d='m4.5 12 5 5L17 6'/%3E%3C/svg%3E")}.delete-inline input:checked~.delete-inline__icon{opacity:0}.dotted-underline{text-decoration:underline;-webkit-text-decoration:underline dotted rgba(68,68,68,.75);text-decoration:underline dotted rgba(68,68,68,.75);text-decoration-thickness:.25px}.dotted-underline:hover{-webkit-text-decoration:none;text-decoration:none}.paper-breadcrumbs__list{border-bottom:1px solid #e0e5e7;border-radius:0;font-size:.8rem;padding-left:.5rem;padding-right:.5rem}@media(min-width:576px){.paper-breadcrumbs__list{padding-left:1rem;padding-right:1rem}}.paper-card{box-shadow:0 8px 12px rgba(0,0,0,.02)}.paper-card .card-header{border-top-left-radius:.25rem;border-top-right-radius:.25rem;color:#444}@media(max-width:767.98px){.paper-card .card-header{padding-left:.75rem;padding-right:.75rem}}.paper-card .card-body{background:#fff}@media(max-width:767.98px){.paper-card .card-body{padding-left:.75rem;padding-right:.75rem}}.paper-card .card-body:first-child{border-top-left-radius:.25rem;border-top-right-radius:.25rem}.paper-card .card-body:last-child{border-bottom-left-radius:.25rem;border-bottom-right-radius:.25rem}.paper-card .card-subtitle{color:#444;display:block}.paper-card .card-footer{border-bottom-left-radius:.25rem;border-bottom-right-radius:.25rem}@media(max-width:767.98px){.paper-card .card-footer{padding-left:.75rem;padding-right:.75rem}}.paper-card--danger{border-color:#ffb3b3}.paper-card--danger .card-header{background-color:#fcc;border-color:#ffb3b3;color:#5a6570}.paper-card--danger .card-footer{border-color:#ffb3b3}.paper-card--warning{border-color:#d5ff80}.paper-card--warning .card-header{background-color:#efc;border-color:#d5ff80;color:#5a6570}.paper-card--warning .card-footer{border-color:#d5ff80}.paper-card--success{border-color:#9f9}.paper-card--success .card-header{background-color:#cfc;border-color:#9f9;color:#5a6570}.paper-card--success .card-footer{border-color:#9f9}.paper-card--info{border-color:#9df}.paper-card--info .card-header{background-color:#cef;border-color:#9df;color:#5a6570}.paper-card--info .card-footer{border-color:#9df}.paper-card--primary{border-color:#e3ff57}.paper-card--primary .card-header{background-color:#f0ffa3;border-color:#e3ff57;color:#5a6570}.paper-card--primary .card-footer{border-color:#e3ff57}.paper-card--secondary{border-color:#c4c4c4}.paper-card--secondary .card-header{background-color:#ebebeb;border-color:#c4c4c4;color:#5a6570}.paper-card--secondary .card-footer{border-color:#c4c4c4}.paper-dropzone{min-height:50px;position:relative}.paper-dropzone__overlay{background:rgba(250,226,72,.65);border-radius:.25rem;box-sizing:content-box;height:100%;left:-5px;opacity:0;padding:5px;position:absolute;text-align:center;top:-5px;transition:opacity .1s,background .1s,z-index 0s .1s;width:100%;z-index:-1}.on-drag-file .paper-dropzone__overlay,.ondrag .paper-dropzone__overlay{opacity:1;transition:opacity .1s,background .1s,z-index 0s 0s;z-index:1}.paper-dropzone__overlay--highlighted{background-color:rgba(160,160,255,.65)}.paper-dropzone__hint{left:50%;position:absolute;top:50%;transform:translate(-50%,-50%)}.dz-default{display:none}.paper-environment{background:var(--bg-color);border-bottom:1px solid #333;font-size:.625rem;line-height:1.375;margin-bottom:0;padding:.125rem .75rem;text-align:center;text-transform:uppercase}.paper-error-list{list-style:none;margin:0;padding:0}.paper-error-list.invalid-feedback{margin-top:.25rem}.paper-error-list.invalid-tooltip{margin-top:2px;padding:.25rem .5rem}.paper-error-list:empty{display:none!important}.paper-error-list li:before{content:"• "}.paper-form__label--required:after,.paper-form__row--required .paper-form__label:after{color:#d04010;content:"*";display:inline-block;font-weight:700;margin-left:.125em;position:relative;top:-.2em}.paper-form__label{color:#444;cursor:pointer;font-size:.875rem;font-weight:300;line-height:1.375rem;margin-bottom:0;transition:color .2s}@media(prefers-reduced-motion:reduce){.paper-form__label{transition:none}}@media(max-width:767.98px){.paper-form__label{margin-bottom:.375rem}}.paper-form__label:hover{color:#212529}.paper-form__row{background-color:#fff;padding:.75rem 1rem}@media(max-width:767.98px){.paper-form__row{padding-left:.75rem;padding-right:.75rem}}.paper-form__row:not(:first-of-type){border-top:1px dashed #e9ecef}.paper-card .paper-form__row:last-child{border-bottom-left-radius:inherit;border-bottom-right-radius:inherit}.paper-card>.card-body:first-of-type .paper-form__row:first-child{border-top-left-radius:inherit;border-top-right-radius:inherit}.paper-card>.card-header:first-of-type+.card-body .paper-form__row:first-child{border-top-left-radius:0;border-top-right-radius:0}.paper-form__row--readonly .readonly{font-size:1rem;word-break:break-word}.paper-form__row--invalid{background-color:#ffe0e0}.paper-header{-webkit-backface-visibility:hidden;backface-visibility:hidden;background:#fff;box-shadow:0 0 1px 1px #e0e5e7;min-height:2.75rem;z-index:1021}.paper-header .navbar{box-sizing:content-box;min-height:30px}.paper-header .navbar-nav{margin-right:-.375rem}.paper-header .nav-item{margin-right:.375rem}.paper-header .nav-link{border-radius:.25rem;color:#333;font-size:.875rem;line-height:1.5714285714;min-width:30px;padding-bottom:.25rem;padding-top:.25rem;text-align:center}.paper-header .nav-link:hover,.paper-header .nav-link[aria-expanded=true]{background-color:#e9ecef;color:#6060e0}.paper-header .nav-link:focus{box-shadow:0 0 0 2px #444;outline:0}.paper-header__burger{min-width:32px;text-align:center}.paper-header__burger:hover{color:#1090c0}.paper-header__burger i{display:inline-block;transform:scale(1.75)}.paper-input-group a.input-group-text{background:#f8f9fa;color:#9a9a9a;justify-content:center;min-width:2.25rem}.paper-input-group a.input-group-text:focus{position:relative;z-index:1}.paper-input-group a.input-group-text:hover{color:#9a9a9a;-webkit-text-decoration:none;text-decoration:none}.paper-input-group a.input-group-text[href]{color:#7575e4}.paper-input-group a.input-group-text[href]:not(.disabled):hover{background:#e9ecef;color:#6060e0}.paper-input-group a.input-group-text.disabled{background:#f8f9fa;color:#9a9a9a;cursor:default}.paper-input-group button.input-group-text{background:#f8f9fa;color:#7575e4;justify-content:center;min-width:2.25rem}.paper-input-group button.input-group-text:focus{position:relative;z-index:1}.paper-input-group button.input-group-text:hover{background-color:#e9ecef;color:#6060e0}.paper-input-group button.input-group-text.disabled,.paper-input-group button.input-group-text:disabled{background-color:#f8f9fa;color:#9a9a9a;cursor:default}.paper-input-group label.input-group-text{background-color:#f8f9fa;color:#9a9a9a;justify-content:center;min-width:2.25rem}.paper-input-group label.input-group-text:focus{position:relative;z-index:1}.paper-input-group label.input-group-text:hover{color:#9a9a9a;-webkit-text-decoration:none;text-decoration:none}.paper-input-group label.input-group-text[for]{color:#7575e4}.paper-input-group label.input-group-text[for]:not(.disabled):hover{background-color:#e9ecef;color:#6060e0}.paper-input-group label.input-group-text.disabled{background-color:#f8f9fa;color:#9a9a9a;cursor:default}.paper-input-group a.input-group-text--primary[href]{color:#7575e4}.paper-input-group a.input-group-text--primary[href]:not(.disabled):hover{color:#6060e0}.paper-input-group button.input-group-text--primary{color:#7575e4}.paper-input-group button.input-group-text--primary:not(.disabled):not(:disabled):hover{color:#6060e0}.paper-input-group label.input-group-text--primary[for]{color:#7575e4}.paper-input-group label.input-group-text--primary[for]:not(.disabled):hover{color:#6060e0}.paper-input-group a.input-group-text--secondary[href]{color:#6d6d6d}.paper-input-group a.input-group-text--secondary[href]:not(.disabled):hover{color:#606060}.paper-input-group button.input-group-text--secondary{color:#6d6d6d}.paper-input-group button.input-group-text--secondary:not(.disabled):not(:disabled):hover{color:#606060}.paper-input-group label.input-group-text--secondary[for]{color:#6d6d6d}.paper-input-group label.input-group-text--secondary[for]:not(.disabled):hover{color:#606060}.paper-input-group a.input-group-text--success[href]{color:#4cbe6c}.paper-input-group a.input-group-text--success[href]:not(.disabled):hover{color:#40b060}.paper-input-group button.input-group-text--success{color:#4cbe6c}.paper-input-group button.input-group-text--success:not(.disabled):not(:disabled):hover{color:#40b060}.paper-input-group label.input-group-text--success[for]{color:#4cbe6c}.paper-input-group label.input-group-text--success[for]:not(.disabled):hover{color:#40b060}.paper-input-group a.input-group-text--info[href]{color:#12a2d8}.paper-input-group a.input-group-text--info[href]:not(.disabled):hover{color:#1090c0}.paper-input-group button.input-group-text--info{color:#12a2d8}.paper-input-group button.input-group-text--info:not(.disabled):not(:disabled):hover{color:#1090c0}.paper-input-group label.input-group-text--info[for]{color:#12a2d8}.paper-input-group label.input-group-text--info[for]:not(.disabled):hover{color:#1090c0}.paper-input-group a.input-group-text--warning[href]{color:#ffc61a}.paper-input-group a.input-group-text--warning[href]:not(.disabled):hover{color:#ffc000}.paper-input-group button.input-group-text--warning{color:#ffc61a}.paper-input-group button.input-group-text--warning:not(.disabled):not(:disabled):hover{color:#ffc000}.paper-input-group label.input-group-text--warning[for]{color:#ffc61a}.paper-input-group label.input-group-text--warning[for]:not(.disabled):hover{color:#ffc000}.paper-input-group a.input-group-text--danger[href]{color:#e84712}.paper-input-group a.input-group-text--danger[href]:not(.disabled):hover{color:#d04010}.paper-input-group button.input-group-text--danger{color:#e84712}.paper-input-group button.input-group-text--danger:not(.disabled):not(:disabled):hover{color:#d04010}.paper-input-group label.input-group-text--danger[for]{color:#e84712}.paper-input-group label.input-group-text--danger[for]:not(.disabled):hover{color:#d04010}.paper-input-group a.input-group-text--light[href]{color:#f8f9fa}.paper-input-group a.input-group-text--light[href]:not(.disabled):hover{color:#e9ecef}.paper-input-group button.input-group-text--light{color:#f8f9fa}.paper-input-group button.input-group-text--light:not(.disabled):not(:disabled):hover{color:#e9ecef}.paper-input-group label.input-group-text--light[for]{color:#f8f9fa}.paper-input-group label.input-group-text--light[for]:not(.disabled):hover{color:#e9ecef}.paper-input-group a.input-group-text--dark[href]{color:#2a2a2a}.paper-input-group a.input-group-text--dark[href]:not(.disabled):hover{color:#1d1d1d}.paper-input-group button.input-group-text--dark{color:#2a2a2a}.paper-input-group button.input-group-text--dark:not(.disabled):not(:disabled):hover{color:#1d1d1d}.paper-input-group label.input-group-text--dark[for]{color:#2a2a2a}.paper-input-group label.input-group-text--dark[for]:not(.disabled):hover{color:#1d1d1d}.paper-messages{list-style:none;margin:0;padding:0}.paper-messages:empty{display:none}.paper-message{background-position:6.375px .75rem;background-repeat:no-repeat;background-size:1.203125rem 1.203125rem;border-radius:0 3px 3px 0;border-style:solid;border-width:1px 1px 1px 8px;font-size:.875rem;line-height:1.375;padding:.75rem 2rem}.paper-message:not(:first-child){margin-top:.5rem}.paper-message--error{background-color:#fcc;background-image:url("data:image/svg+xml;charset=utf-8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='225' height='225'%3E%3Ccircle cx='112.5' cy='112.5' r='92.5' fill='none' stroke='%23d04010' stroke-linejoin='round' stroke-width='20'/%3E%3Cpath fill='%23d04010' stroke='%23d04010' stroke-linecap='round' stroke-linejoin='round' stroke-width='20' d='M115 120.86v-57h-5v57z'/%3E%3Ccircle cx='112.5' cy='157.5' r='12.5' fill='%23d04010'/%3E%3C/svg%3E");border-color:#ffb3b3}.paper-message--warning{background-color:#efc;background-image:url("data:image/svg+xml;charset=utf-8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='225' height='225'%3E%3Cpath fill='none' stroke='%23ffc000' stroke-linejoin='round' stroke-width='20' d='M215.17 205.17H9.83L112.5 19.83z'/%3E%3Cpath fill='%23ffc000' stroke='%23ffc000' stroke-linecap='round' stroke-linejoin='round' stroke-width='20' d='M110 123v57h5v-57z'/%3E%3Ccircle cx='112.5' cy='86.36' r='12.5' fill='%23ffc000'/%3E%3C/svg%3E");border-color:#d5ff80}.paper-message--debug,.paper-message--info{background-color:#cef;background-image:url("data:image/svg+xml;charset=utf-8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='225' height='225'%3E%3Ccircle cx='112.5' cy='112.5' r='92.5' fill='none' stroke='%231090c0' stroke-linejoin='round' stroke-width='20'/%3E%3Cpath fill='%231090c0' stroke='%231090c0' stroke-linecap='round' stroke-linejoin='round' stroke-width='20' d='M110 103v57h5v-57z'/%3E%3Ccircle cx='112.5' cy='66.36' r='12.5' fill='%231090c0'/%3E%3C/svg%3E");border-color:#9df}.paper-message--success{background-color:#cfc;background-image:url("data:image/svg+xml;charset=utf-8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='225' height='225'%3E%3Cpath fill='none' stroke='%2340b060' stroke-linecap='round' stroke-linejoin='round' stroke-width='22' d='m68.71 110.45 36.42 36.41 59.75-59.75'/%3E%3Ccircle cx='112.5' cy='112.5' r='92.5' fill='none' stroke='%2340b060' stroke-linejoin='round' stroke-width='20'/%3E%3C/svg%3E");border-color:#9f9}.paper-modal-backdrop{opacity:0}.paper-modal .modal-header{padding:.75rem 1rem}.paper-modal .modal-header:empty{display:none}.paper-modal .modal-title{font-size:1.25rem;line-height:1.25}.paper-modal .modal-body{padding:1rem}.paper-modal .modal-footer{padding:.5rem .75rem}.paper-modal .modal-footer:empty{display:none}.paper-modal .close{align-self:stretch;margin:-.75rem -1rem -.75rem auto;padding:0 1rem}.paper-modal--preloader .paper-preloader{margin:10px auto 20px}.paper-modal--danger .modal-content{border-color:#ffb3b3}.paper-modal--danger .modal-header{background-color:#fcc;border-color:#ffb3b3;color:#212529}.paper-modal--warning .modal-content{border-color:#d5ff80}.paper-modal--warning .modal-header{background-color:#efc;border-color:#d5ff80;color:#212529}.paper-modal--success .modal-content{border-color:#9f9}.paper-modal--success .modal-header{background-color:#cfc;border-color:#9f9;color:#212529}.paper-modal--info .modal-content{border-color:#9df}.paper-modal--info .modal-header{background-color:#cef;border-color:#9df;color:#212529}.paper-modal--primary .modal-content{border-color:#e3ff57}.paper-modal--primary .modal-header{background-color:#f0ffa3;border-color:#e3ff57;color:#212529}.paper-modal--secondary .modal-content{border-color:#c4c4c4}.paper-modal--secondary .modal-header{background-color:#ebebeb;border-color:#c4c4c4;color:#212529}.paper-object-list{padding-left:.5rem}.paper-object-list ul{margin-top:.125rem;padding-left:1.375rem}.paper-object-list li{list-style-position:inside}.paper-object-list li:not(:first-child){margin-top:.125rem}.paper-page.js{transition:margin-left .5s}@media(min-width:1200px)and (min-width:0){body:not(.popup) .paper-page{margin-left:14rem}}@media(min-width:1200px)and (min-width:1280px){body:not(.popup) .paper-page{margin-left:16rem}}.paper-page__header h1{font-size:1.5rem;margin-bottom:0}.paper-page__toolbar{display:none}@media(min-width:992px){.paper-page__toolbar{display:block}}@media(min-width:0){.paper-page__toolbar{width:14rem}}@media(min-width:1280px){.paper-page__toolbar{width:15rem}}.paper-page__toolbar:empty{display:none}@keyframes pulse{0%{opacity:1}to{opacity:.5}}@keyframes load{0%{transform:rotate(-35deg)}18%{border-width:6px}50%{border-width:3px}82%{border-width:6px}to{transform:rotate(215deg)}}.paper-preloader{height:70px;overflow:hidden;position:relative;width:140px}.paper-preloader:before{animation:load .9s ease-in-out infinite alternate;border:8px solid transparent;border-left-color:#6060e0;border-radius:50%;content:"";height:200%;position:absolute;width:100%}.paper-preloader__text{animation:pulse .75s linear infinite alternate;bottom:0;font-size:18px;left:0;position:absolute;text-align:center;text-transform:uppercase;width:100%}.sidebar-shadow{background:rgba(0,0,0,.33);height:100%;left:0;opacity:0;position:fixed;top:0;transition:all .5s,visibility .5s 0s;visibility:hidden;width:100%;z-index:1029}@media(min-width:1200px){.sidebar-shadow{display:none}}.sidebar-open .sidebar-shadow{opacity:1;transition:all .5s,visibility 0s 0s;visibility:visible}.paper-sidebar{background:url(/static/paper_admin/dist/assets/menu_bg.jpg);box-shadow:0 0 5px rgba(0,0,0,.66);height:100vh;left:0;position:fixed;top:0;transform:translate(-102%);transition:transform .5s;will-change:transform;z-index:1030}@media(min-width:1200px){.paper-sidebar{transform:translate(0)}}@media(min-width:0){.paper-sidebar{width:14rem}}@media(min-width:1280px){.paper-sidebar{width:16rem}}.sidebar-open .paper-sidebar{transform:translate(0)}.paper-sidebar .navbar{height:100%}.paper-sidebar .navbar-brand{border-bottom:1px solid #333;min-height:2.875rem;padding:.5rem .75rem}.paper-sidebar .navbar-brand-name{color:#fff;font-size:1.125rem;word-break:break-word}.paper-sidebar__menu{margin-top:10px;overflow-y:auto}.paper-sidebar__item-list{background:#101010}.paper-sidebar__item-list--level-1{background:transparent;margin-bottom:20px}.paper-sidebar__item-list--level-2{border-bottom:1px solid #444;position:relative}.paper-sidebar__item-list--level-2:before{background:#444;content:"";height:100%;left:22px;position:absolute;top:0;width:1px;z-index:1}.paper-sidebar__link{align-items:baseline;color:inherit;display:flex;font-size:.875rem;line-height:1.375;padding:.5rem .75rem;transition:all .2s ease-in-out;word-break:break-word}@media(prefers-reduced-motion:reduce){.paper-sidebar__link{transition:none}}.paper-sidebar__link:focus,.paper-sidebar__link:hover{background:hsla(0,0%,100%,.1);color:#fff;outline:none;-webkit-text-decoration:none;text-decoration:none}.paper-sidebar__link>i{flex:0 0 20px;line-height:1;margin-right:.375rem;text-align:left}.active>.paper-sidebar__link{background:rgba(172,172,239,.7);color:#fff}.paper-sidebar__link--trigger{padding-right:34px;position:relative}.paper-sidebar__link--trigger:after{content:"";font:.625rem bootstrap-icons;position:absolute;right:.75rem;top:calc(50% - .375rem);transform:rotate(-90deg);transition:all .2s ease-in-out}@media(prefers-reduced-motion:reduce){.paper-sidebar__link--trigger:after{transition:none}}.paper-sidebar__link--trigger[aria-expanded=true]:after{transform:rotate(0deg)}.paper-sidebar__item{color:hsla(0,0%,100%,.8)}.paper-sidebar__item--level-1{padding-left:0}.paper-sidebar__item--level-1>.paper-sidebar__link>i{font-size:inherit;transform:scale(1.3) translate(5%,-5%)}.paper-sidebar__item--level-1>.paper-sidebar__link:hover{background:hsla(0,0%,100%,.1)}.paper-sidebar__item--level-2{padding-left:22px;position:relative}.paper-sidebar__item--level-2>.paper-sidebar__link:before{background:#101010;border:1px solid #444;border-radius:50%;content:"";height:7px;left:22px;position:absolute;top:17.625px;transform:translate(-3px,-50%);transition:all .2s ease-in-out;width:7px;z-index:1}@media(prefers-reduced-motion:reduce){.paper-sidebar__item--level-2>.paper-sidebar__link:before{transition:none}}.paper-sidebar__item--level-2>.paper-sidebar__link.paper-sidebar__link--trigger:before{left:0}.paper-sidebar__item--level-2>.paper-sidebar__link:focus:before,.paper-sidebar__item--level-2>.paper-sidebar__link:hover:before{background:#acacef}.paper-sidebar__item--level-2.active>.paper-sidebar__link:before{content:none}.paper-sidebar__item--level-2.open>.paper-sidebar__link:before{background:#acacef}.paper-sidebar__item--level-3>.paper-sidebar__divider,.paper-sidebar__item--level-3>.paper-sidebar__link,.paper-sidebar__item--level-4>.paper-sidebar__divider,.paper-sidebar__item--level-4>.paper-sidebar__link{padding-left:24px}.paper-sidebar__divider{background-color:#444;height:1px;padding:0 .75rem}.paper-sidebar__group{color:#606060;font-size:11px;letter-spacing:1px;margin:1.25em 0 .5em;padding:0 .75rem;text-transform:uppercase}.paper-table{background-color:#fff;border:1px solid #e0e5e7;border-collapse:separate;border-radius:.25rem;border-spacing:0;box-shadow:0 8px 12px rgba(0,0,0,.02);vertical-align:top}.paper-table__small-column{width:.1%}.paper-table__sort-button{border-radius:.125rem;color:#606060;font-size:inherit;margin:0 0 0 .125rem;padding:.125rem .375rem;vertical-align:baseline}.paper-table__sort-button--has-prior{padding-right:.6em}.paper-table__sort-button span{font-size:75%;margin-left:.125rem!important}.paper-table__sortable-cell{position:relative;width:1.25rem}.paper-table__sort-handler{align-items:center;background:url(/static/paper_admin/dist/assets/sortable.svg) repeat-y center 5px;background-clip:content-box;background-size:contain;border-right:1px solid #e0e5e7;bottom:0;color:#c3c3c3;cursor:move;display:flex;justify-content:center;left:0;padding:5px 0;position:absolute;right:0;top:0;transition:color .3s}.paper-table__sort-handler.disabled{color:#e9ecef}.paper-table__sort-handler.disabled,tr.disabled .paper-table__sort-handler{cursor:default}tr:not(.disabled) .paper-table__sort-handler:not(.disabled):hover{color:#333}.paper-table td,.paper-table th{border-top:none;padding:.5rem;vertical-align:middle}.paper-table .action-checkbox,.paper-table .action-checkbox-column{padding-right:.25rem}.paper-table td:first-child,.paper-table th:first-child{padding-left:.75rem}.paper-table td:last-child,.paper-table th:last-child{padding-right:.75rem}.paper-table thead th{border-bottom:1px solid #dadada;color:#333;font-size:.75rem;font-weight:500;padding:.5rem;text-transform:uppercase;vertical-align:middle}.paper-table thead th:first-child{border-top-left-radius:.25rem}.paper-table thead th:last-child{border-top-right-radius:.25rem}.paper-table thead th a{color:inherit}.paper-table thead th .dropdown-item{text-transform:none}.paper-table tfoot td{border-top:1px solid #dadada}.paper-table tbody th{font-weight:400}.paper-table tbody tr.selected td,.paper-table tbody tr.selected th{background-color:#fff7e0}.paper-table tbody tr:not(:last-child) td,.paper-table tbody tr:not(:last-child) th{border-bottom:1px solid #e9ecef}.paper-table tbody tr.table-danger td,.paper-table tbody tr.table-danger th,.paper-table--danger thead th{background-color:#fcc;border-color:#ffb3b3}.paper-table tbody tr.table-danger:hover td,.paper-table tbody tr.table-danger:hover th{background-color:#ffbdbd}.paper-table tbody tr.table-warning td,.paper-table tbody tr.table-warning th,.paper-table--warning thead th{background-color:#efc;border-color:#d5ff80}.paper-table tbody tr.table-warning:hover td,.paper-table tbody tr.table-warning:hover th{background-color:#e9ffbd}.paper-table tbody tr.table-success td,.paper-table tbody tr.table-success th,.paper-table--success thead th{background-color:#cfc;border-color:#9f9}.paper-table tbody tr.table-success:hover td,.paper-table tbody tr.table-success:hover th{background-color:#bdffbd}.paper-table tbody tr.table-info td,.paper-table tbody tr.table-info th,.paper-table--info thead th{background-color:#cef;border-color:#9df}.paper-table tbody tr.table-info:hover td,.paper-table tbody tr.table-info:hover th{background-color:#bde9ff}.paper-table tbody tr.table-primary td,.paper-table tbody tr.table-primary th,.paper-table--primary thead th{background-color:#f0ffa3;border-color:#e3ff57}.paper-table tbody tr.table-primary:hover td,.paper-table tbody tr.table-primary:hover th{background-color:#edff94}.paper-table tbody tr.table-secondary td,.paper-table tbody tr.table-secondary th,.paper-table--secondary thead th{background-color:#ebebeb;border-color:#c4c4c4}.paper-table tbody tr.table-secondary:hover td,.paper-table tbody tr.table-secondary:hover th{background-color:#e3e3e3}.paper-table--sortable tbody tr{transition:opacity .1s,background-color .3s}.paper-table--sortable tbody tr.sortable-ghost{background-color:#fff2cc!important}.paper-table--sortable tbody tr.disabled{opacity:.3}@media(max-width:767.98px){.paper-widget--checkbox>.custom-control{display:inline-block;vertical-align:top}}.paper-widget--invalid~.invalid-feedback,.paper-widget--invalid~.invalid-tooltip{display:block}.paper-widget--invalid .custom-file-label,.paper-widget--invalid .form-control{border-color:#df7d5c;box-shadow:0 0 0 1px #df7d5c}.paper-widget--invalid .form-control:focus{border-color:#444;box-shadow:0 0 0 1px #444}.paper-widget--invalid .form-control{background-image:url("data:image/svg+xml;charset=utf-8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='12' height='12' fill='none' stroke='%23d04010'%3E%3Ccircle cx='6' cy='6' r='4.5'/%3E%3Cpath stroke-linejoin='round' d='M5.8 3.6h.4L6 6.5z'/%3E%3Ccircle cx='6' cy='8.2' r='.6' fill='%23d04010' stroke='none'/%3E%3C/svg%3E");background-position:right .375rem center;background-repeat:no-repeat;background-size:calc(.6875em + .375rem) calc(.6875em + .375rem);padding-right:calc(.6875em + 1.125rem)}@keyframes form_appear{0%{opacity:0;top:-5vh}to{opacity:1;top:0}}.login{background:url(/static/paper_admin/dist/assets/login_bg.jpg) bottom;background-size:cover}.login:before{background:rgba(0,0,0,.5);bottom:0;content:"";left:0;position:absolute;right:0;top:0;z-index:-1}.login .paper-page{margin-left:0!important}.login-card{animation:form_appear .8s .4s backwards;border-radius:.25rem;max-width:100%;position:relative;width:320px}.password-reset-link a{color:inherit}.paper-actions{align-items:center;display:flex;flex:1 1 auto;flex-wrap:wrap}.paper-actions__action{padding:1px 0}.paper-actions__action select{max-width:340px;min-width:180px;padding-left:.375rem;padding-right:24px;width:auto}.paper-actions__select_across{display:none}.paper-actions__button{margin-right:1rem}.paper-actions__tools{flex:1 0 auto;padding:.375rem 0}.paper-actions__all,.paper-actions__counter{margin-right:.375rem}.paper-actions__clear,.paper-actions__question{margin-left:.375rem}.paper-filter{margin-bottom:.75rem}.paper-filter:not(:first-child){border-top:1px dashed #e9ecef;padding-top:.75rem}.paper-filter__title{font-size:1rem;font-weight:300}.paper-search-form{width:15rem}.paper-search-form__field{position:relative}.paper-search-form__icon{color:#9a9a9a;left:.5rem;line-height:1.375;position:absolute;top:.375rem}.paper-search-form .form-control{padding-left:1.75rem}.paper-search-form .form-control::-webkit-search-cancel-button{-webkit-appearance:none;background:no-repeat url(/static/paper_admin/dist/assets/cross.svg) 50%;cursor:pointer;height:1em;margin:0;width:1em}#result_list .related-widget-wrapper__buttons{display:none}.paper-formset:not(:first-child){margin-top:1.5rem}.paper-formset__form{overflow:hidden}.paper-formset__form-caption{color:inherit}.paper-formset--tabular .paper-formset__form--invalid{background-color:#ffe0e0}.paper-formset--tabular thead th{padding-bottom:.5rem}.paper-tabs{position:relative}.paper-page__header+.paper-tabs{margin-top:-.5rem}@media(min-width:992px){.paper-page__header+.paper-tabs{margin-top:0}}.paper-tabs__underline{background-color:#1090c0;height:2px;position:absolute;transition:all .2s}.paper-tabs .nav{display:flex;margin-left:-.375rem;margin-right:-.375rem}.paper-tabs .nav-item{margin-bottom:.375rem;margin-right:.5rem}.paper-tabs .nav-link{color:#606060;font-size:1rem;font-weight:300;padding:.25rem .375rem}.paper-tabs .active,.paper-tabs .nav-link:hover{color:#6060e0}@keyframes arrow{0%{top:.875rem}25%{top:.625rem}75%{top:1.125rem}to{top:.875rem}}.scroll-top-button{align-items:center;background-color:#40b060;border-radius:50%;bottom:2rem;box-shadow:0 2px 6px rgba(0,0,0,.4);cursor:pointer;display:none;font-size:1rem;height:3rem;justify-content:center;opacity:.75;position:fixed;right:1rem;transform:scale(0);transition:all .2s ease-in-out;width:3rem;will-change:transform;z-index:1020}@media(prefers-reduced-motion:reduce){.scroll-top-button{transition:none}}@media(min-width:992px){.scroll-top-button{bottom:2.75rem;display:flex!important;right:2rem}}.scroll-top-button i{-webkit-backface-visibility:hidden;backface-visibility:hidden;color:#fff;will-change:top}.scroll-top-button.show{transform:scale(1)}.scroll-top-button:hover{opacity:1}.scroll-top-button:hover i{animation:arrow 2s linear infinite}.custom-select[multiple]{height:40px}
```

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/assets/Roboto.woff` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/assets/Roboto.woff`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/assets/Roboto.woff2` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/assets/Roboto.woff2`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/assets/RobotoBold.woff` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/assets/RobotoBold.woff`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/assets/RobotoBold.woff2` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/assets/RobotoBold.woff2`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/assets/RobotoBoldItalic.woff` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/assets/RobotoBoldItalic.woff`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/assets/RobotoBoldItalic.woff2` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/assets/RobotoBoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/assets/RobotoItalic.woff` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/assets/RobotoItalic.woff`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/assets/RobotoItalic.woff2` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/assets/RobotoItalic.woff2`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/assets/RobotoLight.woff` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/assets/RobotoLight.woff`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/assets/RobotoLight.woff2` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/assets/RobotoLight.woff2`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/assets/RobotoLightItalic.woff` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/assets/RobotoLightItalic.woff`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/assets/RobotoLightItalic.woff2` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/assets/RobotoLightItalic.woff2`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/assets/RobotoMedium.woff` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/assets/RobotoMedium.woff`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/assets/RobotoMedium.woff2` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/assets/RobotoMedium.woff2`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/assets/RobotoMediumItalic.woff` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/assets/RobotoMediumItalic.woff`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/assets/RobotoMediumItalic.woff2` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/assets/RobotoMediumItalic.woff2`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/assets/bootstrap-icons.woff` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/assets/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/assets/bootstrap-icons.woff2` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/assets/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/assets/default_favicon.png` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/assets/default_favicon.png`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/assets/login_bg.jpg` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/assets/login_bg.jpg`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/assets/menu_bg.jpg` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/assets/menu_bg.jpg`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/assets/sortable.svg` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/assets/sortable.svg`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/changeform.e4e3561b61eb70807245.js` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/changeform.e4e3561b61eb70807245.js`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/changeform.e4e3561b61eb70807245.js.map` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/changeform.e4e3561b61eb70807245.js.map`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/changelist.52229b67dbe6c9ce1e04.js` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/changelist.52229b67dbe6c9ce1e04.js`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/changelist.52229b67dbe6c9ce1e04.js.map` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/changelist.52229b67dbe6c9ce1e04.js.map`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/critical.11e9b5fdb3be652e8277.js` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/critical.11e9b5fdb3be652e8277.js`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/critical.11e9b5fdb3be652e8277.js.map` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/critical.11e9b5fdb3be652e8277.js.map`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/npm.animejs.0610cb68d4b2f57e8eb8.js` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/npm.animejs.0610cb68d4b2f57e8eb8.js`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/npm.animejs.0610cb68d4b2f57e8eb8.js.map` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/npm.animejs.0610cb68d4b2f57e8eb8.js.map`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/npm.bootstrap.59081124c9ac6decacff.js` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/npm.bootstrap.59081124c9ac6decacff.js`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/npm.bootstrap.59081124c9ac6decacff.js.map` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/npm.bootstrap.59081124c9ac6decacff.js.map`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/npm.clockpicker.ac0071909818cc80b526.js` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/npm.clockpicker.ac0071909818cc80b526.js`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/npm.clockpicker.ac0071909818cc80b526.js.map` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/npm.clockpicker.ac0071909818cc80b526.js.map`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/npm.core-js-pure.1bc2fd98475787ba1164.js` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/npm.core-js-pure.1bc2fd98475787ba1164.js`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/npm.core-js-pure.1bc2fd98475787ba1164.js.map` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/npm.core-js-pure.1bc2fd98475787ba1164.js.map`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/npm.es-abstract.6d963e08114704c8e4d0.js` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/npm.es-abstract.6d963e08114704c8e4d0.js`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/npm.es-abstract.6d963e08114704c8e4d0.js.map` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/npm.es-abstract.6d963e08114704c8e4d0.js.map`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/npm.flatpickr.365327b4124495649c9b.js` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/npm.flatpickr.365327b4124495649c9b.js`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/npm.flatpickr.365327b4124495649c9b.js.LICENSE.txt` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/npm.flatpickr.365327b4124495649c9b.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/npm.flatpickr.365327b4124495649c9b.js.map` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/npm.flatpickr.365327b4124495649c9b.js.map`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/npm.jquery.00f10cc5d0570a88ed04.js` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/npm.jquery.00f10cc5d0570a88ed04.js`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/npm.jquery.00f10cc5d0570a88ed04.js.map` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/npm.jquery.00f10cc5d0570a88ed04.js.map`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/npm.popper.js.fa6168d95a0931432fac.js` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/npm.popper.js.fa6168d95a0931432fac.js`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/npm.popper.js.fa6168d95a0931432fac.js.LICENSE.txt` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/npm.popper.js.fa6168d95a0931432fac.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/npm.popper.js.fa6168d95a0931432fac.js.map` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/npm.popper.js.fa6168d95a0931432fac.js.map`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/npm.select2.62432bf0675ff2408a99.js` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/npm.select2.62432bf0675ff2408a99.js`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/npm.select2.62432bf0675ff2408a99.js.map` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/npm.select2.62432bf0675ff2408a99.js.map`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/npm.sortablejs.73e6a37ecdb386aaa55f.js` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/npm.sortablejs.73e6a37ecdb386aaa55f.js`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/npm.sortablejs.73e6a37ecdb386aaa55f.js.map` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/npm.sortablejs.73e6a37ecdb386aaa55f.js.map`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/npm.xregexp.98d0b833497d9fd631e9.js` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/npm.xregexp.98d0b833497d9fd631e9.js`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/npm.xregexp.98d0b833497d9fd631e9.js.LICENSE.txt` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/npm.xregexp.98d0b833497d9fd631e9.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/npm.xregexp.98d0b833497d9fd631e9.js.map` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/npm.xregexp.98d0b833497d9fd631e9.js.map`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/popup.64e2e99cf69da31de176.js.map` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/popup.64e2e99cf69da31de176.js.map`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/runtime.f3efd79e7f1f7f906465.js` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/runtime.f3efd79e7f1f7f906465.js`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/runtime.f3efd79e7f1f7f906465.js.map` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/runtime.f3efd79e7f1f7f906465.js.map`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/vendors.bootstrap-icons.329567d3425b7a67d749.css` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/vendors.bootstrap-icons.329567d3425b7a67d749.css`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/static/paper_admin/dist/vendors.bootstrap.6d9ce52aceafe8da2e8c.css` & `paper-admin-6.0.0rc4/paper_admin/static/paper_admin/dist/vendors.bootstrap.6d9ce52aceafe8da2e8c.css`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/templates/admin/actions.html` & `paper-admin-6.0.0rc4/paper_admin/templates/admin/actions.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/templates/admin/app_index.html` & `paper-admin-6.0.0rc4/paper_admin/templates/admin/app_index.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/templates/admin/auth/user/change_password.html` & `paper-admin-6.0.0rc4/paper_admin/templates/admin/auth/user/change_password.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/templates/admin/base.html` & `paper-admin-6.0.0rc4/paper_admin/templates/admin/base.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/templates/admin/base_site.html` & `paper-admin-6.0.0rc4/paper_admin/templates/admin/base_site.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/templates/admin/change_form.html` & `paper-admin-6.0.0rc4/paper_admin/templates/admin/change_form.html`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 {% endblock %}
 
 
 {% block before_content %}
   {{ block.super }}
 
   {% if tabs %}
-    <div class="paper-tabs mb-3">
+    <div class="paper-tabs mb-2 mb-lg-3">
       <div class="paper-tabs__underline"></div>
       <ul class="nav" role="tablist">
         {% for tab in tabs %}
           <li class="nav-item">
             <a class="nav-link{% if tab.invalid %} text-danger{% endif %}{% if tab.active %} active{% endif %}"
                id="{{ tab.name }}-tab" href="#{{ tab.name }}-panel" role="tab" data-toggle="tab"
                aria-controls="{{ tab.name }}-panel" aria-selected="{{ tab.active|yesno:"true,false" }}">
```

### Comparing `paper-admin-6.0.0rc3/paper_admin/templates/admin/change_form_object_tools.html` & `paper-admin-6.0.0rc4/paper_admin/templates/admin/change_form_object_tools.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/templates/admin/change_list.html` & `paper-admin-6.0.0rc4/paper_admin/templates/admin/change_list.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/templates/admin/change_list_results.html` & `paper-admin-6.0.0rc4/paper_admin/templates/admin/change_list_results.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/templates/admin/date_hierarchy.html` & `paper-admin-6.0.0rc4/paper_admin/templates/admin/date_hierarchy.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/templates/admin/delete_confirmation.html` & `paper-admin-6.0.0rc4/paper_admin/templates/admin/delete_confirmation.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/templates/admin/delete_selected_confirmation.html` & `paper-admin-6.0.0rc4/paper_admin/templates/admin/delete_selected_confirmation.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/templates/admin/edit_inline/_stacked_form.html` & `paper-admin-6.0.0rc4/paper_admin/templates/admin/edit_inline/_stacked_form.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {% load paper_styles %}
 
 <fieldset class="paper-formset__form paper-card card mb-3 {% paper_form_classes inline_form %}{% if inline_form.form.errors %} paper-formset__form--invalid{% endif %}{% if inline_admin_formset.sortable_allowed %} sortable-item{% endif %}{% if inline_form.original or inline_form.show_url %} has_original{% endif %}">
   <div class="card-header py-2">
     <div class="d-flex justify-content-between">
-      <h4 class="paper-formset__form-caption card-title inline-label align-self-center pr-4 mb-0 text-secondary">
+      <h4 class="paper-formset__form-caption card-title inline-label align-self-center pr-4 mb-0">
         {% if inline_form.original %}
           {{ inline_form.original }}
         {% else %}
           {{ inline_admin_formset.opts.verbose_name|capfirst }} #{% if form_index == '__prefix__' %}{{ form_index }}{% else %}{{ form_index|add:1 }}{% endif %}
         {% endif %}
       </h4>
```

### Comparing `paper-admin-6.0.0rc3/paper_admin/templates/admin/edit_inline/_tabular_form.html` & `paper-admin-6.0.0rc4/paper_admin/templates/admin/edit_inline/_tabular_form.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/templates/admin/edit_inline/stacked.html` & `paper-admin-6.0.0rc4/paper_admin/templates/admin/edit_inline/stacked.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/templates/admin/edit_inline/tabular.html` & `paper-admin-6.0.0rc4/paper_admin/templates/admin/edit_inline/tabular.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/templates/admin/filter.html` & `paper-admin-6.0.0rc4/paper_admin/templates/admin/filter.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/templates/admin/includes/fieldset.html` & `paper-admin-6.0.0rc4/paper_admin/templates/admin/includes/fieldset.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/templates/admin/login.html` & `paper-admin-6.0.0rc4/paper_admin/templates/admin/login.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/templates/admin/object_history.html` & `paper-admin-6.0.0rc4/paper_admin/templates/admin/object_history.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/templates/admin/pagination.html` & `paper-admin-6.0.0rc4/paper_admin/templates/admin/pagination.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/templates/admin/popup_response.html` & `paper-admin-6.0.0rc4/paper_admin/templates/admin/popup_response.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/templates/admin/search_form.html` & `paper-admin-6.0.0rc4/paper_admin/templates/admin/search_form.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/templates/admin/widgets/related_widget_wrapper.html` & `paper-admin-6.0.0rc4/paper_admin/templates/admin/widgets/related_widget_wrapper.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/templates/django/forms/widgets/clearable_file_input.html` & `paper-admin-6.0.0rc4/paper_admin/templates/django/forms/widgets/clearable_file_input.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/templates/django/forms/widgets/date.html` & `paper-admin-6.0.0rc4/paper_admin/templates/django/forms/widgets/date.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/templates/django/forms/widgets/email.html` & `paper-admin-6.0.0rc4/paper_admin/templates/django/forms/widgets/email.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/templates/django/forms/widgets/file.html` & `paper-admin-6.0.0rc4/paper_admin/templates/django/forms/widgets/file.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/templates/django/forms/widgets/foreign_key_raw_id.html` & `paper-admin-6.0.0rc4/paper_admin/templates/django/forms/widgets/foreign_key_raw_id.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/templates/django/forms/widgets/password.html` & `paper-admin-6.0.0rc4/paper_admin/templates/django/forms/widgets/password.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/templates/django/forms/widgets/select.html` & `paper-admin-6.0.0rc4/paper_admin/templates/django/forms/widgets/select.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/templates/django/forms/widgets/select_multiple.html` & `paper-admin-6.0.0rc4/paper_admin/templates/django/forms/widgets/select_multiple.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/templates/django/forms/widgets/time.html` & `paper-admin-6.0.0rc4/paper_admin/templates/django/forms/widgets/time.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/templates/django/forms/widgets/url.html` & `paper-admin-6.0.0rc4/paper_admin/templates/django/forms/widgets/url.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/templates/django/forms/widgets/uuid.html` & `paper-admin-6.0.0rc4/paper_admin/templates/django/forms/widgets/uuid.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/templates/paper_admin/app.head.html` & `paper-admin-6.0.0rc4/paper_admin/templates/paper_admin/app.head.html`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-<script defer="defer" src="/static/paper_admin/dist/runtime.f3efd79e7f1f7f906465.js"></script><script defer="defer" src="/static/paper_admin/dist/npm.core-js-pure.1bc2fd98475787ba1164.js"></script><script defer="defer" src="/static/paper_admin/dist/npm.es-abstract.6d963e08114704c8e4d0.js"></script><script defer="defer" src="/static/paper_admin/dist/npm.xregexp.98d0b833497d9fd631e9.js"></script><script defer="defer" src="/static/paper_admin/dist/npm.flatpickr.365327b4124495649c9b.js"></script><script defer="defer" src="/static/paper_admin/dist/npm.bootstrap.59081124c9ac6decacff.js"></script><script defer="defer" src="/static/paper_admin/dist/npm.jquery.00f10cc5d0570a88ed04.js"></script><script defer="defer" src="/static/paper_admin/dist/npm.sortablejs.73e6a37ecdb386aaa55f.js"></script><script defer="defer" src="/static/paper_admin/dist/npm.select2.62432bf0675ff2408a99.js"></script><script defer="defer" src="/static/paper_admin/dist/npm.popper.js.fa6168d95a0931432fac.js"></script><script defer="defer" src="/static/paper_admin/dist/npm.clockpicker.ac0071909818cc80b526.js"></script><script defer="defer" src="/static/paper_admin/dist/npm.animejs.0610cb68d4b2f57e8eb8.js"></script><script defer="defer" src="/static/paper_admin/dist/app.802db2f5c8fabda7425c.js"></script><link href="/static/paper_admin/dist/vendors.bootstrap.6d9ce52aceafe8da2e8c.css" rel="stylesheet"><link href="/static/paper_admin/dist/vendors.bootstrap-icons.329567d3425b7a67d749.css" rel="stylesheet"><link href="/static/paper_admin/dist/app.styles.779e472c0f96c40859ce.css" rel="stylesheet">
+<script defer="defer" src="/static/paper_admin/dist/runtime.f3efd79e7f1f7f906465.js"></script><script defer="defer" src="/static/paper_admin/dist/npm.core-js-pure.1bc2fd98475787ba1164.js"></script><script defer="defer" src="/static/paper_admin/dist/npm.es-abstract.6d963e08114704c8e4d0.js"></script><script defer="defer" src="/static/paper_admin/dist/npm.xregexp.98d0b833497d9fd631e9.js"></script><script defer="defer" src="/static/paper_admin/dist/npm.flatpickr.365327b4124495649c9b.js"></script><script defer="defer" src="/static/paper_admin/dist/npm.bootstrap.59081124c9ac6decacff.js"></script><script defer="defer" src="/static/paper_admin/dist/npm.jquery.00f10cc5d0570a88ed04.js"></script><script defer="defer" src="/static/paper_admin/dist/npm.sortablejs.73e6a37ecdb386aaa55f.js"></script><script defer="defer" src="/static/paper_admin/dist/npm.select2.62432bf0675ff2408a99.js"></script><script defer="defer" src="/static/paper_admin/dist/npm.popper.js.fa6168d95a0931432fac.js"></script><script defer="defer" src="/static/paper_admin/dist/npm.clockpicker.ac0071909818cc80b526.js"></script><script defer="defer" src="/static/paper_admin/dist/npm.animejs.0610cb68d4b2f57e8eb8.js"></script><script defer="defer" src="/static/paper_admin/dist/app.802db2f5c8fabda7425c.js"></script><link href="/static/paper_admin/dist/vendors.bootstrap.6d9ce52aceafe8da2e8c.css" rel="stylesheet"><link href="/static/paper_admin/dist/vendors.bootstrap-icons.329567d3425b7a67d749.css" rel="stylesheet"><link href="/static/paper_admin/dist/app.styles.9ae55058e746fe5377c3.css" rel="stylesheet">
```

### Comparing `paper-admin-6.0.0rc3/paper_admin/templates/paper_admin/filters/checkbox.html` & `paper-admin-6.0.0rc4/paper_admin/templates/paper_admin/filters/checkbox.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/templates/paper_admin/filters/daterange.html` & `paper-admin-6.0.0rc4/paper_admin/templates/paper_admin/filters/daterange.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/templates/paper_admin/filters/hierarchy.html` & `paper-admin-6.0.0rc4/paper_admin/templates/paper_admin/filters/hierarchy.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/templates/paper_admin/filters/list.html` & `paper-admin-6.0.0rc4/paper_admin/templates/paper_admin/filters/list.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/templates/paper_admin/filters/radio.html` & `paper-admin-6.0.0rc4/paper_admin/templates/paper_admin/filters/radio.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/templates/paper_admin/footer.html` & `paper-admin-6.0.0rc4/paper_admin/templates/paper_admin/footer.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/templates/paper_admin/header_buttons.html` & `paper-admin-6.0.0rc4/paper_admin/templates/paper_admin/header_buttons.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/templates/paper_admin/includes/admin_checkbox.html` & `paper-admin-6.0.0rc4/paper_admin/templates/paper_admin/includes/admin_checkbox.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/templates/paper_admin/includes/admin_field.html` & `paper-admin-6.0.0rc4/paper_admin/templates/paper_admin/includes/admin_field.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/templates/paper_admin/includes/changelist_tools.html` & `paper-admin-6.0.0rc4/paper_admin/templates/paper_admin/includes/changelist_tools.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/templates/paper_admin/menu/item.html` & `paper-admin-6.0.0rc4/paper_admin/templates/paper_admin/menu/item.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/templates/paper_admin/menu/submenu.html` & `paper-admin-6.0.0rc4/paper_admin/templates/paper_admin/menu/submenu.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/templates/registration/password_change_form.html` & `paper-admin-6.0.0rc4/paper_admin/templates/registration/password_change_form.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/templates/registration/password_reset_confirm.html` & `paper-admin-6.0.0rc4/paper_admin/templates/registration/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/templates/registration/password_reset_done.html` & `paper-admin-6.0.0rc4/paper_admin/templates/registration/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/templates/registration/password_reset_email.html` & `paper-admin-6.0.0rc4/paper_admin/templates/registration/password_reset_email.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/templates/registration/password_reset_email_alt.html` & `paper-admin-6.0.0rc4/paper_admin/templates/registration/password_reset_email_alt.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/templates/registration/password_reset_form.html` & `paper-admin-6.0.0rc4/paper_admin/templates/registration/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/templatetags/paper_filters.py` & `paper-admin-6.0.0rc4/paper_admin/templatetags/paper_filters.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/templatetags/paper_list.py` & `paper-admin-6.0.0rc4/paper_admin/templatetags/paper_list.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/templatetags/paper_menu.py` & `paper-admin-6.0.0rc4/paper_admin/templatetags/paper_menu.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/templatetags/paper_modify.py` & `paper-admin-6.0.0rc4/paper_admin/templatetags/paper_modify.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/templatetags/paper_paginator.py` & `paper-admin-6.0.0rc4/paper_admin/templatetags/paper_paginator.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin/templatetags/paper_styles.py` & `paper-admin-6.0.0rc4/paper_admin/templatetags/paper_styles.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc3/paper_admin.egg-info/PKG-INFO` & `paper-admin-6.0.0rc4/paper_admin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-admin
-Version: 6.0.0rc3
+Version: 6.0.0rc4
 Summary: Custom Django admin interface.
 Home-page: https://github.com/dldevinc/paper-admin
 Author: Mihail Mishakin
 Author-email: x896321475@gmail.com
 Maintainer: Mihail Mishakin
 Maintainer-email: x896321475@gmail.com
 License: BSD license
@@ -52,15 +52,15 @@
 -   [Patches](#Patches)
 -   [Badge](#Badge)
 -   [Admin menu](#Admin-menu)
 -   [Reorderable drag-and-drop lists](#Reorderable-drag-and-drop-lists)
 -   [Form tabs](#Form-tabs)
 -   [HierarchyFilter](#HierarchyFilter)
 -   [Stylization](#Stylization)
-    -   [Fieldset](#Fieldset)
+    -   [Fieldsets](#Fieldsets)
     -   [Table rows](#Table-rows)
     -   [Inline forms](#Inline-forms)
 -   [Settings](#Settings)
 -   [Additional References](#Additional-References)
 
 ## Installation
 
@@ -561,15 +561,39 @@
 
 Result:
 
 ![image](https://user-images.githubusercontent.com/6928240/229168174-a9c32ec8-f87a-4ec9-a875-105eeae61f06.png)
 
 ## Stylization
 
-### Fieldset
+### Table rows
+
+You can use the `get_row_classes` method of the `ModelAdmin`
+class to add custom classes to the rows in the list view.
+
+```python
+from django.contrib import admin
+from .models import Category
+
+
+@admin.register(Category)
+class CategoryAdmin(admin.ModelAdmin):
+
+    def get_row_classes(self, request, obj):
+        if obj.status == "success":
+            return ["table-success"]
+        elif obj.status == "failed":
+            return ["table-danger"]
+        return []
+```
+
+![image](https://user-images.githubusercontent.com/6928240/233795075-d0f85cc2-d34a-43a9-b393-20cd81f96d99.png)
+
+
+### Fieldsets
 
 Django [provides](https://docs.djangoproject.com/en/4.0/ref/contrib/admin/#django.contrib.admin.ModelAdmin.fieldsets)
 a way to add a custom CSS classes to the fieldsets in the admin interface.
 
 To use this feature, specify the `classes` parameter in the `ModelAdmin.fieldsets`
 attribute:
 
@@ -600,38 +624,15 @@
             "fields": (
                 # ...
             )
         }),
     )
 ```
 
-![](https://user-images.githubusercontent.com/6928240/125337870-8f91e180-e360-11eb-9b19-7f903ab30464.png)
-
-### Table rows
-
-You can use the `get_row_classes` method of the `ModelAdmin`
-class to add custom classes to the rows in the list view.
-
-```python
-from django.contrib import admin
-from .models import Category
-
-
-@admin.register(Category)
-class CategoryAdmin(admin.ModelAdmin):
-
-    def get_row_classes(self, request, obj):
-        if obj.status == "success":
-            return ["table-success"]
-        elif obj.status == "failed":
-            return ["table-danger"]
-        return []
-```
-
-![image](https://user-images.githubusercontent.com/6928240/225705910-4f1309e1-93e3-456a-b9d0-f01748faec7b.png)
+![image](https://user-images.githubusercontent.com/6928240/233795448-17d2fa5c-739a-4751-8266-b4b4e879b1c8.png)
 
 ### Inline forms
 
 You can use the `get_form_classes` method of the `ModelAdmin` class
 to add custom classes to the inline forms:
 
 ```python
@@ -652,16 +653,16 @@
         if obj.status == "success":
             return ["table-success"]
         elif obj.status == "failed":
             return ["table-danger"]
         return []
 ```
 
-![image](https://user-images.githubusercontent.com/6928240/225713947-34e29927-b629-4b9a-bf6e-56ec8948de7e.png)
-![image](https://user-images.githubusercontent.com/6928240/225714321-87a33c52-65d8-4175-a118-cb751b92ebb8.png)
+![image](https://user-images.githubusercontent.com/6928240/233794982-1ca7248a-dc54-48c4-aea2-44d0d973d083.png)
+![image](https://user-images.githubusercontent.com/6928240/233795183-c056b82e-8b01-4f7d-9c09-65c0becbdc33.png)
 
 ## Settings
 
 `PAPER_FAVICON`<br>
 The path to the favicon for the admin interface.<br>
 Default: `"paper_admin/dist/assets/default_favicon.png"`
```

### Comparing `paper-admin-6.0.0rc3/paper_admin.egg-info/SOURCES.txt` & `paper-admin-6.0.0rc4/paper_admin.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 paper_admin/patches/tree_queries/templatetags/__init__.py
 paper_admin/patches/tree_queries/templatetags/paper_tree_queries_list.py
 paper_admin/static/admin/img/icon-no.svg
 paper_admin/static/admin/img/icon-yes.svg
 paper_admin/static/paper_admin/dist/app.802db2f5c8fabda7425c.js
 paper_admin/static/paper_admin/dist/app.802db2f5c8fabda7425c.js.LICENSE.txt
 paper_admin/static/paper_admin/dist/app.802db2f5c8fabda7425c.js.map
-paper_admin/static/paper_admin/dist/app.styles.779e472c0f96c40859ce.css
+paper_admin/static/paper_admin/dist/app.styles.9ae55058e746fe5377c3.css
 paper_admin/static/paper_admin/dist/changeform.e4e3561b61eb70807245.js
 paper_admin/static/paper_admin/dist/changeform.e4e3561b61eb70807245.js.map
 paper_admin/static/paper_admin/dist/changelist.52229b67dbe6c9ce1e04.js
 paper_admin/static/paper_admin/dist/changelist.52229b67dbe6c9ce1e04.js.map
 paper_admin/static/paper_admin/dist/critical.11e9b5fdb3be652e8277.js
 paper_admin/static/paper_admin/dist/critical.11e9b5fdb3be652e8277.js.map
 paper_admin/static/paper_admin/dist/npm.animejs.0610cb68d4b2f57e8eb8.js
```

### Comparing `paper-admin-6.0.0rc3/setup.cfg` & `paper-admin-6.0.0rc4/setup.cfg`

 * *Files identical despite different names*

