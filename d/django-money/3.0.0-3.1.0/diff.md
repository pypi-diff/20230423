# Comparing `tmp/django-money-3.0.0.tar.gz` & `tmp/django-money-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/tmp/tmp7x7jxrdx/tmpuoffln75/django-money-3.0.0.tar", last modified: Mon Jun 20 14:21:52 2022, max compression
+gzip compressed data, was "django-money-3.1.0.tar", last modified: Sun Apr 23 20:53:17 2023, max compression
```

## Comparing `django-money-3.0.0.tar` & `django-money-3.1.0.tar`

### file list

```diff
@@ -1,60 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-20 14:21:52.000000 django-money-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (116)     1755 2022-06-20 14:21:34.000000 django-money-3.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (116)       87 2022-06-20 14:21:34.000000 django-money-3.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)    16720 2022-06-20 14:21:52.000000 django-money-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)    15404 2022-06-20 14:21:34.000000 django-money-3.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-20 14:21:52.000000 django-money-3.0.0/django_money.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)    16720 2022-06-20 14:21:51.000000 django-money-3.0.0/django_money.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1471 2022-06-20 14:21:52.000000 django-money-3.0.0/django_money.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-06-20 14:21:52.000000 django-money-3.0.0/django_money.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      135 2022-06-20 14:21:52.000000 django-money-3.0.0/django_money.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        8 2022-06-20 14:21:52.000000 django-money-3.0.0/django_money.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-20 14:21:52.000000 django-money-3.0.0/djmoney/
--rw-r--r--   0 runner    (1001) docker     (116)      247 2022-06-20 14:21:34.000000 django-money-3.0.0/djmoney/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      564 2022-06-20 14:21:34.000000 django-money-3.0.0/djmoney/_compat.py
--rw-r--r--   0 runner    (1001) docker     (116)      644 2022-06-20 14:21:34.000000 django-money-3.0.0/djmoney/admin.py
--rw-r--r--   0 runner    (1001) docker     (116)      426 2022-06-20 14:21:34.000000 django-money-3.0.0/djmoney/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-20 14:21:52.000000 django-money-3.0.0/djmoney/contrib/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-06-20 14:21:34.000000 django-money-3.0.0/djmoney/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-20 14:21:52.000000 django-money-3.0.0/djmoney/contrib/django_rest_framework/
--rw-r--r--   0 runner    (1001) docker     (116)       61 2022-06-20 14:21:34.000000 django-money-3.0.0/djmoney/contrib/django_rest_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3005 2022-06-20 14:21:34.000000 django-money-3.0.0/djmoney/contrib/django_rest_framework/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-20 14:21:52.000000 django-money-3.0.0/djmoney/contrib/exchange/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-06-20 14:21:34.000000 django-money-3.0.0/djmoney/contrib/exchange/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      380 2022-06-20 14:21:34.000000 django-money-3.0.0/djmoney/contrib/exchange/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-20 14:21:52.000000 django-money-3.0.0/djmoney/contrib/exchange/backends/
--rw-r--r--   0 runner    (1001) docker     (116)      104 2022-06-20 14:21:34.000000 django-money-3.0.0/djmoney/contrib/exchange/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2350 2022-06-20 14:21:34.000000 django-money-3.0.0/djmoney/contrib/exchange/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (116)      548 2022-06-20 14:21:34.000000 django-money-3.0.0/djmoney/contrib/exchange/backends/fixer.py
--rw-r--r--   0 runner    (1001) docker     (116)      688 2022-06-20 14:21:34.000000 django-money-3.0.0/djmoney/contrib/exchange/backends/openexchangerates.py
--rw-r--r--   0 runner    (1001) docker     (116)       81 2022-06-20 14:21:34.000000 django-money-3.0.0/djmoney/contrib/exchange/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-20 14:21:52.000000 django-money-3.0.0/djmoney/contrib/exchange/management/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-06-20 14:21:34.000000 django-money-3.0.0/djmoney/contrib/exchange/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      638 2022-06-20 14:21:34.000000 django-money-3.0.0/djmoney/contrib/exchange/management/base.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-20 14:21:52.000000 django-money-3.0.0/djmoney/contrib/exchange/management/commands/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-06-20 14:21:34.000000 django-money-3.0.0/djmoney/contrib/exchange/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      915 2022-06-20 14:21:34.000000 django-money-3.0.0/djmoney/contrib/exchange/management/commands/clear_rates.py
--rw-r--r--   0 runner    (1001) docker     (116)      369 2022-06-20 14:21:34.000000 django-money-3.0.0/djmoney/contrib/exchange/management/commands/update_rates.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-20 14:21:52.000000 django-money-3.0.0/djmoney/contrib/exchange/migrations/
--rw-r--r--   0 runner    (1001) docker     (116)     1390 2022-06-20 14:21:34.000000 django-money-3.0.0/djmoney/contrib/exchange/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-06-20 14:21:34.000000 django-money-3.0.0/djmoney/contrib/exchange/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3861 2022-06-20 14:21:34.000000 django-money-3.0.0/djmoney/contrib/exchange/models.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-20 14:21:52.000000 django-money-3.0.0/djmoney/forms/
--rw-r--r--   0 runner    (1001) docker     (116)       61 2022-06-20 14:21:34.000000 django-money-3.0.0/djmoney/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3548 2022-06-20 14:21:34.000000 django-money-3.0.0/djmoney/forms/fields.py
--rw-r--r--   0 runner    (1001) docker     (116)      833 2022-06-20 14:21:34.000000 django-money-3.0.0/djmoney/forms/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-20 14:21:52.000000 django-money-3.0.0/djmoney/models/
--rw-r--r--   0 runner    (1001) docker     (116)      101 2022-06-20 14:21:34.000000 django-money-3.0.0/djmoney/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    13006 2022-06-20 14:21:34.000000 django-money-3.0.0/djmoney/models/fields.py
--rw-r--r--   0 runner    (1001) docker     (116)     9355 2022-06-20 14:21:34.000000 django-money-3.0.0/djmoney/models/managers.py
--rw-r--r--   0 runner    (1001) docker     (116)     2001 2022-06-20 14:21:34.000000 django-money-3.0.0/djmoney/models/validators.py
--rw-r--r--   0 runner    (1001) docker     (116)     5673 2022-06-20 14:21:34.000000 django-money-3.0.0/djmoney/money.py
--rw-r--r--   0 runner    (1001) docker     (116)     2361 2022-06-20 14:21:34.000000 django-money-3.0.0/djmoney/serializers.py
--rw-r--r--   0 runner    (1001) docker     (116)     1666 2022-06-20 14:21:34.000000 django-money-3.0.0/djmoney/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-20 14:21:52.000000 django-money-3.0.0/djmoney/templatetags/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-06-20 14:21:34.000000 django-money-3.0.0/djmoney/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3393 2022-06-20 14:21:34.000000 django-money-3.0.0/djmoney/templatetags/djmoney.py
--rw-r--r--   0 runner    (1001) docker     (116)     1074 2022-06-20 14:21:34.000000 django-money-3.0.0/djmoney/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)      158 2022-06-20 14:21:34.000000 django-money-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)      569 2022-06-20 14:21:52.000000 django-money-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     2832 2022-06-20 14:21:34.000000 django-money-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 20:53:17.332533 django-money-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-23 20:53:09.000000 django-money-3.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-23 20:53:09.000000 django-money-3.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    16751 2023-04-23 20:53:17.332533 django-money-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15435 2023-04-23 20:53:09.000000 django-money-3.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 20:53:17.328533 django-money-3.1.0/django_money.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16751 2023-04-23 20:53:17.000000 django-money-3.1.0/django_money.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-04-23 20:53:17.000000 django-money-3.1.0/django_money.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 20:53:17.000000 django-money-3.1.0/django_money.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-23 20:53:17.000000 django-money-3.1.0/django_money.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-23 20:53:17.000000 django-money-3.1.0/django_money.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 20:53:17.328533 django-money-3.1.0/djmoney/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 20:53:17.328533 django-money-3.1.0/djmoney/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 20:53:17.328533 django-money-3.1.0/djmoney/contrib/django_rest_framework/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/contrib/django_rest_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/contrib/django_rest_framework/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 20:53:17.328533 django-money-3.1.0/djmoney/contrib/exchange/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/contrib/exchange/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/contrib/exchange/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 20:53:17.332533 django-money-3.1.0/djmoney/contrib/exchange/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/contrib/exchange/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/contrib/exchange/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/contrib/exchange/backends/fixer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/contrib/exchange/backends/openexchangerates.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/contrib/exchange/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 20:53:17.332533 django-money-3.1.0/djmoney/contrib/exchange/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/contrib/exchange/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/contrib/exchange/management/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 20:53:17.332533 django-money-3.1.0/djmoney/contrib/exchange/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/contrib/exchange/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/contrib/exchange/management/commands/clear_rates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/contrib/exchange/management/commands/update_rates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 20:53:17.332533 django-money-3.1.0/djmoney/contrib/exchange/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/contrib/exchange/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/contrib/exchange/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/contrib/exchange/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 20:53:17.332533 django-money-3.1.0/djmoney/forms/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/forms/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/forms/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 20:53:17.332533 django-money-3.1.0/djmoney/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13006 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/models/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/models/managers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/models/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/money.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 20:53:17.332533 django-money-3.1.0/djmoney/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/templatetags/djmoney.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-23 20:53:09.000000 django-money-3.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-23 20:53:17.332533 django-money-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-04-23 20:53:09.000000 django-money-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 20:53:17.332533 django-money-3.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-23 20:53:09.000000 django-money-3.1.0/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-04-23 20:53:09.000000 django-money-3.1.0/tests/test_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7192 2023-04-23 20:53:09.000000 django-money-3.1.0/tests/test_managers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39496 2023-04-23 20:53:09.000000 django-money-3.1.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-04-23 20:53:09.000000 django-money-3.1.0/tests/test_money.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-23 20:53:09.000000 django-money-3.1.0/tests/test_reversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-04-23 20:53:09.000000 django-money-3.1.0/tests/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-23 20:53:09.000000 django-money-3.1.0/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-04-23 20:53:09.000000 django-money-3.1.0/tests/test_tags.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-money-3.0.0/LICENSE.txt` & `django-money-3.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-money-3.0.0/PKG-INFO` & `django-money-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-money
-Version: 3.0.0
+Version: 3.1.0
 Summary: Adds support for using money and currency fields in django models and forms. Uses py-moneyed as the money implementation.
 Home-page: https://github.com/django-money/django-money
 Maintainer: Greg Reinbach
 Maintainer-email: greg@reinbach.com
 License: BSD
 Keywords: django,py-money,money
 Platform: Any
@@ -49,17 +49,17 @@
 .. image:: https://img.shields.io/pypi/v/django-money.svg
    :target: https://pypi.python.org/pypi/django-money
    :alt: PyPI
 
 A little Django app that uses `py-moneyed <https://github.com/py-moneyed/py-moneyed>`__ to add support for Money
 fields in your models and forms.
 
-* Django versions supported: 2.2, 3.2, 4.0, 4.1
-* Python versions supported: 3.7, 3.8, 3.9, 3.10
-* PyPy versions supported: PyPy3
+* Django versions supported: 2.2, 3.2, 4.0, 4.1, 4.2
+* Python versions supported: 3.7, 3.8, 3.9, 3.10, 3.11
+* PyPy versions supported: PyPy3 (for Django <= 4.0)
 
 If you need support for older versions of Django and Python, please refer to older releases mentioned in `the release notes <https://django-money.readthedocs.io/en/latest/changes.html>`__.
 
 Through the dependency `py-moneyed <https://github.com/py-moneyed/py-moneyed>`__, ``django-money`` gets:
 
 * Support for proper Money value handling (using the standard Money
   design pattern)
```

### Comparing `django-money-3.0.0/README.rst` & `django-money-3.1.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 .. image:: https://img.shields.io/pypi/v/django-money.svg
    :target: https://pypi.python.org/pypi/django-money
    :alt: PyPI
 
 A little Django app that uses `py-moneyed <https://github.com/py-moneyed/py-moneyed>`__ to add support for Money
 fields in your models and forms.
 
-* Django versions supported: 2.2, 3.2, 4.0, 4.1
-* Python versions supported: 3.7, 3.8, 3.9, 3.10
-* PyPy versions supported: PyPy3
+* Django versions supported: 2.2, 3.2, 4.0, 4.1, 4.2
+* Python versions supported: 3.7, 3.8, 3.9, 3.10, 3.11
+* PyPy versions supported: PyPy3 (for Django <= 4.0)
 
 If you need support for older versions of Django and Python, please refer to older releases mentioned in `the release notes <https://django-money.readthedocs.io/en/latest/changes.html>`__.
 
 Through the dependency `py-moneyed <https://github.com/py-moneyed/py-moneyed>`__, ``django-money`` gets:
 
 * Support for proper Money value handling (using the standard Money
   design pattern)
```

### Comparing `django-money-3.0.0/django_money.egg-info/PKG-INFO` & `django-money-3.1.0/django_money.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-money
-Version: 3.0.0
+Version: 3.1.0
 Summary: Adds support for using money and currency fields in django models and forms. Uses py-moneyed as the money implementation.
 Home-page: https://github.com/django-money/django-money
 Maintainer: Greg Reinbach
 Maintainer-email: greg@reinbach.com
 License: BSD
 Keywords: django,py-money,money
 Platform: Any
@@ -49,17 +49,17 @@
 .. image:: https://img.shields.io/pypi/v/django-money.svg
    :target: https://pypi.python.org/pypi/django-money
    :alt: PyPI
 
 A little Django app that uses `py-moneyed <https://github.com/py-moneyed/py-moneyed>`__ to add support for Money
 fields in your models and forms.
 
-* Django versions supported: 2.2, 3.2, 4.0, 4.1
-* Python versions supported: 3.7, 3.8, 3.9, 3.10
-* PyPy versions supported: PyPy3
+* Django versions supported: 2.2, 3.2, 4.0, 4.1, 4.2
+* Python versions supported: 3.7, 3.8, 3.9, 3.10, 3.11
+* PyPy versions supported: PyPy3 (for Django <= 4.0)
 
 If you need support for older versions of Django and Python, please refer to older releases mentioned in `the release notes <https://django-money.readthedocs.io/en/latest/changes.html>`__.
 
 Through the dependency `py-moneyed <https://github.com/py-moneyed/py-moneyed>`__, ``django-money`` gets:
 
 * Support for proper Money value handling (using the standard Money
   design pattern)
```

### Comparing `django-money-3.0.0/djmoney/_compat.py` & `django-money-3.1.0/djmoney/_compat.py`

 * *Files identical despite different names*

### Comparing `django-money-3.0.0/djmoney/admin.py` & `django-money-3.1.0/djmoney/admin.py`

 * *Files identical despite different names*

### Comparing `django-money-3.0.0/djmoney/contrib/django_rest_framework/fields.py` & `django-money-3.1.0/djmoney/contrib/django_rest_framework/fields.py`

 * *Files identical despite different names*

### Comparing `django-money-3.0.0/djmoney/contrib/exchange/backends/base.py` & `django-money-3.1.0/djmoney/contrib/exchange/backends/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 import ssl
 from decimal import Decimal
+from typing import Optional
 from urllib.parse import parse_qsl, urlparse, urlunparse
-from urllib.request import urlopen
+from urllib.request import Request, urlopen
 
 from django.db.transaction import atomic
 from django.utils.http import urlencode
 
 from djmoney import settings
 
 from ..models import ExchangeBackend, Rate
@@ -15,16 +16,16 @@
 try:
     import certifi
 except ImportError:
     raise ImportError("Please install dependency certifi - pip install certifi")
 
 
 class BaseExchangeBackend:
-    name = None
-    url = None
+    name: Optional[str] = None
+    url: Optional[str] = None
 
     def get_rates(self, **kwargs):
         """
         Returns a mapping <currency>: <rate>.
         """
         raise NotImplementedError
 
@@ -41,17 +42,20 @@
     def get_params(self):
         """
         Default GET parameters for the request.
         """
         return {}
 
     def get_response(self, **params):
-        url = self.get_url(**params)
+        headers = {
+            "User-Agent": "Mozilla/5.0",
+        }
+        request = Request(self.get_url(**params), headers=headers)
         context = ssl.create_default_context(cafile=certifi.where())
-        response = urlopen(url, context=context)
+        response = urlopen(request, context=context)
         return response.read()
 
     def parse_json(self, response):
         if isinstance(response, bytes):
             response = response.decode("utf-8")
         return json.loads(response, parse_float=Decimal)
```

### Comparing `django-money-3.0.0/djmoney/contrib/exchange/backends/fixer.py` & `django-money-3.1.0/djmoney/contrib/exchange/backends/fixer.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,8 +11,8 @@
     def __init__(self, url=settings.FIXER_URL, access_key=settings.FIXER_ACCESS_KEY):
         if access_key is None:
             raise ImproperlyConfigured("settings.FIXER_ACCESS_KEY should be set to use FixerBackend")
         self.url = url
         self.access_key = access_key
 
     def get_params(self):
-        return {"access_key": self.access_key}
+        return {"apikey": self.access_key}
```

### Comparing `django-money-3.0.0/djmoney/contrib/exchange/backends/openexchangerates.py` & `django-money-3.1.0/djmoney/contrib/exchange/backends/openexchangerates.py`

 * *Files identical despite different names*

### Comparing `django-money-3.0.0/djmoney/contrib/exchange/management/base.py` & `django-money-3.1.0/djmoney/contrib/exchange/management/base.py`

 * *Files identical despite different names*

### Comparing `django-money-3.0.0/djmoney/contrib/exchange/management/commands/clear_rates.py` & `django-money-3.1.0/djmoney/contrib/exchange/management/commands/clear_rates.py`

 * *Files identical despite different names*

### Comparing `django-money-3.0.0/djmoney/contrib/exchange/migrations/0001_initial.py` & `django-money-3.1.0/djmoney/contrib/exchange/migrations/0001_initial.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # Generated by Django 2.0.4 on 2018-04-03 08:42
+from typing import List, Tuple
 
 import django.db.models.deletion
 from django.db import migrations, models
 
 from djmoney.settings import CURRENCY_CODE_MAX_LENGTH
 
 
 class Migration(migrations.Migration):
 
     initial = True
 
-    dependencies = []
+    dependencies: List[Tuple[str, str]] = []
 
     operations = [
         migrations.CreateModel(
             name="ExchangeBackend",
             fields=[
                 ("name", models.CharField(max_length=255, primary_key=True, serialize=False)),
                 ("last_update", models.DateTimeField(auto_now=True)),
```

### Comparing `django-money-3.0.0/djmoney/contrib/exchange/models.py` & `django-money-3.1.0/djmoney/contrib/exchange/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,29 +36,29 @@
 
 def get_rate(source, target, backend=None):
     """
     Returns an exchange rate between source and target currencies.
     Converts exchange rate on the DB side if there is no backends with given base currency.
     Uses data from the default backend if the backend is not specified.
     """
+    if str(source) == str(target):
+        return 1
     if backend is None:
         backend = get_default_backend_name()
     key = f"djmoney:get_rate:{source}:{target}:{backend}"
     result = cache.get(key)
     if result is not None:
         return result
     result = _get_rate(source, target, backend)
     cache.set(key, result, RATES_CACHE_TIMEOUT)
     return result
 
 
 def _get_rate(source, target, backend):
     source, target = str(source), str(target)
-    if str(source) == target:
-        return 1
     rates = Rate.objects.filter(currency__in=(source, target), backend=backend).select_related("backend")
     if not rates:
         raise MissingRate(f"Rate {source} -> {target} does not exist")
     if len(rates) == 1:
         return _try_to_get_rate_directly(source, target, rates[0])
     return _get_rate_via_base(rates, target)
```

### Comparing `django-money-3.0.0/djmoney/forms/fields.py` & `django-money-3.1.0/djmoney/forms/fields.py`

 * *Files identical despite different names*

### Comparing `django-money-3.0.0/djmoney/forms/widgets.py` & `django-money-3.1.0/djmoney/forms/widgets.py`

 * *Files identical despite different names*

### Comparing `django-money-3.0.0/djmoney/models/fields.py` & `django-money-3.1.0/djmoney/models/fields.py`

 * *Files identical despite different names*

### Comparing `django-money-3.0.0/djmoney/models/managers.py` & `django-money-3.1.0/djmoney/models/managers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from functools import wraps
 
 from django.core.exceptions import FieldDoesNotExist
 from django.db.models import NOT_PROVIDED, Case, F, Q
 from django.db.models.constants import LOOKUP_SEP
 from django.db.models.expressions import BaseExpression
-from django.db.models.functions import Cast
+from django.db.models.functions import Cast, Coalesce
 from django.utils.encoding import smart_str
 
 from ..utils import MONEY_CLASSES, get_currency_field_name, prepare_expression
 from .fields import CurrencyField, MoneyField
 
 
 def _get_clean_name(model, name):
@@ -138,15 +138,15 @@
         if isinstance(value, MONEY_CLASSES):
             clean_name = _get_clean_name(model, name)
             kwargs[name] = value.amount
             currency_field_name = get_currency_field_name(clean_name, field)
             kwargs[currency_field_name] = smart_str(value.currency)
         else:
             if isinstance(field, MoneyField):
-                if isinstance(value, (BaseExpression, F)) and not isinstance(value, (Case, Cast)):
+                if isinstance(value, (BaseExpression, F)) and not isinstance(value, (Case, Cast, Coalesce)):
                     clean_name = _get_clean_name(model, name)
                     if not isinstance(value, F):
                         value = prepare_expression(value)
                     if not _is_money_field(model, value, name):
                         continue
                     currency_field_name = get_currency_field_name(clean_name, field)
                     target_field = _get_field(model, value.name)
```

### Comparing `django-money-3.0.0/djmoney/models/validators.py` & `django-money-3.1.0/djmoney/models/validators.py`

 * *Files identical despite different names*

### Comparing `django-money-3.0.0/djmoney/money.py` & `django-money-3.1.0/djmoney/money.py`

 * *Files identical despite different names*

### Comparing `django-money-3.0.0/djmoney/serializers.py` & `django-money-3.1.0/djmoney/serializers.py`

 * *Files identical despite different names*

### Comparing `django-money-3.0.0/djmoney/settings.py` & `django-money-3.1.0/djmoney/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import operator
 from types import MappingProxyType
+from typing import Optional
 
 from django.conf import settings
 
 from moneyed import CURRENCIES, Currency
 
 
 # The default currency, you can define this in your project's settings module
 # This has to be a currency object imported from moneyed
-DEFAULT_CURRENCY: Currency = getattr(settings, "DEFAULT_CURRENCY", None)
+DEFAULT_CURRENCY: Optional[Currency] = getattr(settings, "DEFAULT_CURRENCY", None)
 
 
 # The default currency choices, you can define this in your project's
 # settings module
 PROJECT_CURRENCIES = getattr(settings, "CURRENCIES", None)
 CURRENCY_CHOICES = getattr(settings, "CURRENCY_CHOICES", None)
```

### Comparing `django-money-3.0.0/djmoney/templatetags/djmoney.py` & `django-money-3.1.0/djmoney/templatetags/djmoney.py`

 * *Files identical despite different names*

### Comparing `django-money-3.0.0/djmoney/utils.py` & `django-money-3.1.0/djmoney/utils.py`

 * *Files identical despite different names*

### Comparing `django-money-3.0.0/setup.cfg` & `django-money-3.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-money-3.0.0/setup.py` & `django-money-3.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 
 test_requirements = [
     "pytest>=3.1.0",
     "pytest-django",
     "pytest-pythonpath",
     "pytest-cov",
     "mixer",
+    "mypy",
+    "django-stubs",
 ]
 
 extras_requirements = {
     "test": test_requirements,
     "exchange": ["certifi"],
 }
```

