# Comparing `tmp/django-minio-storage-0.3.8.tar.gz` & `tmp/django-minio-storage-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-minio-storage-0.3.8.tar", last modified: Thu Jul  9 12:59:38 2020, max compression
+gzip compressed data, was "django-minio-storage-0.5.0.tar", last modified: Sun Apr 23 11:01:30 2023, max compression
```

## Comparing `django-minio-storage-0.3.8.tar` & `django-minio-storage-0.5.0.tar`

### file list

```diff
@@ -1,64 +1,70 @@
-drwxrwxr-x   0 t         (1000) t         (1000)        0 2020-07-09 12:59:38.177765 django-minio-storage-0.3.8/
--rw-r--r--   0 t         (1000) t         (1000)      197 2019-10-16 20:54:45.000000 django-minio-storage-0.3.8/.editorconfig
--rw-r--r--   0 t         (1000) t         (1000)       92 2019-10-16 20:50:16.000000 django-minio-storage-0.3.8/.flake8rc
--rw-rw-r--   0 t         (1000) t         (1000)      100 2019-12-16 11:38:04.000000 django-minio-storage-0.3.8/.gitignore
--rw-rw-r--   0 t         (1000) t         (1000)      259 2019-10-17 17:09:29.000000 django-minio-storage-0.3.8/.isort.cfg
--rw-rw-r--   0 t         (1000) t         (1000)     1448 2019-10-18 12:43:28.000000 django-minio-storage-0.3.8/.travis.yml
--rw-rw-r--   0 t         (1000) t         (1000)     3073 2020-07-09 12:58:41.000000 django-minio-storage-0.3.8/CHANGELOG.md
--rw-r--r--   0 t         (1000) t         (1000)       43 2018-07-12 19:09:03.000000 django-minio-storage-0.3.8/CONTRIBUTING.md
--rw-r--r--   0 t         (1000) t         (1000)    11004 2018-07-12 19:09:03.000000 django-minio-storage-0.3.8/LICENSE-APACHE
--rw-r--r--   0 t         (1000) t         (1000)     1102 2018-07-12 19:09:03.000000 django-minio-storage-0.3.8/LICENSE-MIT
--rw-rw-r--   0 t         (1000) t         (1000)      653 2020-07-09 12:59:38.173765 django-minio-storage-0.3.8/PKG-INFO
--rw-r--r--   0 t         (1000) t         (1000)      965 2018-07-12 19:09:03.000000 django-minio-storage-0.3.8/README.md
--rw-rw-r--   0 t         (1000) t         (1000)      137 2019-10-22 03:11:11.000000 django-minio-storage-0.3.8/dev-requirements.txt
-drwxrwxr-x   0 t         (1000) t         (1000)        0 2020-07-09 12:59:38.157765 django-minio-storage-0.3.8/django_minio_storage.egg-info/
--rw-rw-r--   0 t         (1000) t         (1000)      653 2020-07-09 12:59:38.000000 django-minio-storage-0.3.8/django_minio_storage.egg-info/PKG-INFO
--rw-rw-r--   0 t         (1000) t         (1000)     1372 2020-07-09 12:59:38.000000 django-minio-storage-0.3.8/django_minio_storage.egg-info/SOURCES.txt
--rw-rw-r--   0 t         (1000) t         (1000)        1 2020-07-09 12:59:38.000000 django-minio-storage-0.3.8/django_minio_storage.egg-info/dependency_links.txt
--rw-rw-r--   0 t         (1000) t         (1000)       53 2020-07-09 12:59:38.000000 django-minio-storage-0.3.8/django_minio_storage.egg-info/requires.txt
--rw-rw-r--   0 t         (1000) t         (1000)       75 2020-07-09 12:59:38.000000 django-minio-storage-0.3.8/django_minio_storage.egg-info/top_level.txt
--rw-r--r--   0 t         (1000) t         (1000)      249 2018-07-12 19:09:03.000000 django-minio-storage-0.3.8/docker-compose.yml
-drwxrwxr-x   0 t         (1000) t         (1000)        0 2020-07-09 12:59:38.161765 django-minio-storage-0.3.8/docs/
--rw-r--r--   0 t         (1000) t         (1000)      229 2018-07-12 19:09:12.000000 django-minio-storage-0.3.8/docs/contributing.md
--rw-r--r--   0 t         (1000) t         (1000)       71 2018-07-12 19:09:12.000000 django-minio-storage-0.3.8/docs/contributors.md
--rw-r--r--   0 t         (1000) t         (1000)      636 2019-10-17 17:15:25.000000 django-minio-storage-0.3.8/docs/development.md
--rw-r--r--   0 t         (1000) t         (1000)      626 2019-10-17 17:18:18.000000 django-minio-storage-0.3.8/docs/index.md
--rw-r--r--   0 t         (1000) t         (1000)    12348 2018-07-12 19:09:12.000000 django-minio-storage-0.3.8/docs/licences.md
--rw-rw-r--   0 t         (1000) t         (1000)     5617 2020-07-09 12:57:56.000000 django-minio-storage-0.3.8/docs/usage.md
-drwxrwxr-x   0 t         (1000) t         (1000)        0 2020-07-09 12:59:38.161765 django-minio-storage-0.3.8/minio_storage/
--rw-rw-r--   0 t         (1000) t         (1000)        0 2019-10-21 23:34:38.000000 django-minio-storage-0.3.8/minio_storage/__init__.py
--rw-rw-r--   0 t         (1000) t         (1000)      102 2019-10-18 04:51:16.000000 django-minio-storage-0.3.8/minio_storage/apps.py
--rw-rw-r--   0 t         (1000) t         (1000)      773 2019-10-28 06:17:19.000000 django-minio-storage-0.3.8/minio_storage/errors.py
--rw-rw-r--   0 t         (1000) t         (1000)     4416 2019-12-16 11:38:04.000000 django-minio-storage-0.3.8/minio_storage/files.py
-drwxrwxr-x   0 t         (1000) t         (1000)        0 2020-07-09 12:59:38.161765 django-minio-storage-0.3.8/minio_storage/management/
--rw-rw-r--   0 t         (1000) t         (1000)        0 2019-10-18 04:51:45.000000 django-minio-storage-0.3.8/minio_storage/management/__init__.py
-drwxrwxr-x   0 t         (1000) t         (1000)        0 2020-07-09 12:59:38.161765 django-minio-storage-0.3.8/minio_storage/management/commands/
--rw-rw-r--   0 t         (1000) t         (1000)        0 2019-10-18 04:51:56.000000 django-minio-storage-0.3.8/minio_storage/management/commands/__init__.py
--rw-rw-r--   0 t         (1000) t         (1000)     8296 2019-10-22 18:18:07.000000 django-minio-storage-0.3.8/minio_storage/management/commands/minio.py
--rw-rw-r--   0 t         (1000) t         (1000)     4048 2019-10-18 08:18:30.000000 django-minio-storage-0.3.8/minio_storage/policy.py
--rw-rw-r--   0 t         (1000) t         (1000)    16310 2020-07-09 12:57:56.000000 django-minio-storage-0.3.8/minio_storage/storage.py
--rw-r--r--   0 t         (1000) t         (1000)      235 2018-07-12 19:09:03.000000 django-minio-storage-0.3.8/mkdocs.yml
--rw-rw-r--   0 t         (1000) t         (1000)       40 2019-10-16 22:34:52.000000 django-minio-storage-0.3.8/pyproject.toml
--rw-rw-r--   0 t         (1000) t         (1000)       38 2020-07-09 12:59:38.177765 django-minio-storage-0.3.8/setup.cfg
--rw-rw-r--   0 t         (1000) t         (1000)      970 2019-10-29 01:23:53.000000 django-minio-storage-0.3.8/setup.py
-drwxrwxr-x   0 t         (1000) t         (1000)        0 2020-07-09 12:59:38.165765 django-minio-storage-0.3.8/tests/
--rw-r--r--   0 t         (1000) t         (1000)        0 2018-07-12 19:09:12.000000 django-minio-storage-0.3.8/tests/__init__.py
-drwxrwxr-x   0 t         (1000) t         (1000)        0 2020-07-09 12:59:38.169765 django-minio-storage-0.3.8/tests/django_minio_storage_tests/
--rw-r--r--   0 t         (1000) t         (1000)        0 2018-07-12 19:09:12.000000 django-minio-storage-0.3.8/tests/django_minio_storage_tests/__init__.py
--rw-rw-r--   0 t         (1000) t         (1000)     4156 2019-10-16 20:47:52.000000 django-minio-storage-0.3.8/tests/django_minio_storage_tests/settings.py
--rw-rw-r--   0 t         (1000) t         (1000)      775 2019-10-16 20:47:52.000000 django-minio-storage-0.3.8/tests/django_minio_storage_tests/urls.py
--rw-rw-r--   0 t         (1000) t         (1000)      429 2019-10-16 20:47:52.000000 django-minio-storage-0.3.8/tests/django_minio_storage_tests/wsgi.py
--rwxrwxr-x   0 t         (1000) t         (1000)      283 2019-10-16 20:47:52.000000 django-minio-storage-0.3.8/tests/manage.py
-drwxrwxr-x   0 t         (1000) t         (1000)        0 2020-07-09 12:59:38.169765 django-minio-storage-0.3.8/tests/test_app/
--rw-r--r--   0 t         (1000) t         (1000)        0 2018-07-12 19:09:12.000000 django-minio-storage-0.3.8/tests/test_app/__init__.py
-drwxrwxr-x   0 t         (1000) t         (1000)        0 2020-07-09 12:59:38.173765 django-minio-storage-0.3.8/tests/test_app/tests/
--rw-r--r--   0 t         (1000) t         (1000)        0 2018-07-12 19:09:12.000000 django-minio-storage-0.3.8/tests/test_app/tests/__init__.py
--rw-rw-r--   0 t         (1000) t         (1000)     6152 2020-07-09 12:57:56.000000 django-minio-storage-0.3.8/tests/test_app/tests/bucket_tests.py
--rw-rw-r--   0 t         (1000) t         (1000)     4500 2019-10-22 18:13:14.000000 django-minio-storage-0.3.8/tests/test_app/tests/custom_storage_class_tests.py
--rw-rw-r--   0 t         (1000) t         (1000)     1656 2019-10-16 21:51:18.000000 django-minio-storage-0.3.8/tests/test_app/tests/delete_tests.py
--rw-rw-r--   0 t         (1000) t         (1000)     5381 2019-10-22 03:11:01.000000 django-minio-storage-0.3.8/tests/test_app/tests/managementcommand_tests.py
--rw-rw-r--   0 t         (1000) t         (1000)    10148 2020-07-09 12:57:56.000000 django-minio-storage-0.3.8/tests/test_app/tests/retrieve_tests.py
--rw-rw-r--   0 t         (1000) t         (1000)     4061 2020-02-22 17:00:21.000000 django-minio-storage-0.3.8/tests/test_app/tests/upload_tests.py
--rw-rw-r--   0 t         (1000) t         (1000)     1939 2019-10-17 19:18:53.000000 django-minio-storage-0.3.8/tests/test_app/tests/utils.py
--rw-r--r--   0 t         (1000) t         (1000)    79300 2018-07-12 19:09:12.000000 django-minio-storage-0.3.8/tests/watermelon-cat.jpg
--rw-rw-r--   0 t         (1000) t         (1000)     1220 2020-07-09 12:57:51.000000 django-minio-storage-0.3.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:01:30.946837 django-minio-storage-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/.flake8rc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:01:30.934837 django-minio-storage-0.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:01:30.938837 django-minio-storage-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11004 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/LICENSE-APACHE
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/LICENSE-MIT
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-23 11:01:30.946837 django-minio-storage-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:01:30.938837 django-minio-storage-0.5.0/django_minio_storage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-23 11:01:30.000000 django-minio-storage-0.5.0/django_minio_storage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-23 11:01:30.000000 django-minio-storage-0.5.0/django_minio_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 11:01:30.000000 django-minio-storage-0.5.0/django_minio_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-23 11:01:30.000000 django-minio-storage-0.5.0/django_minio_storage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-23 11:01:30.000000 django-minio-storage-0.5.0/django_minio_storage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:01:30.942837 django-minio-storage-0.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/docs/contributors.md
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/docs/development.md
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12348 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/docs/licences.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/docs-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:01:30.942837 django-minio-storage-0.5.0/minio_storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/minio_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/minio_storage/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/minio_storage/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/minio_storage/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:01:30.942837 django-minio-storage-0.5.0/minio_storage/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/minio_storage/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:01:30.942837 django-minio-storage-0.5.0/minio_storage/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/minio_storage/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/minio_storage/management/commands/minio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/minio_storage/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16648 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/minio_storage/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-23 11:01:30.000000 django-minio-storage-0.5.0/minio_storage/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 11:01:30.946837 django-minio-storage-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:01:30.942837 django-minio-storage-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:01:30.942837 django-minio-storage-0.5.0/tests/django_minio_storage_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/tests/django_minio_storage_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/tests/django_minio_storage_tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/tests/django_minio_storage_tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/tests/django_minio_storage_tests/wsgi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      283 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/tests/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:01:30.946837 django-minio-storage-0.5.0/tests/test_app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/tests/test_app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:01:30.946837 django-minio-storage-0.5.0/tests/test_app/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/tests/test_app/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/tests/test_app/tests/bucket_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/tests/test_app/tests/custom_storage_class_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/tests/test_app/tests/delete_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/tests/test_app/tests/managementcommand_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10141 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/tests/test_app/tests/retrieve_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/tests/test_app/tests/upload_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/tests/test_app/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79300 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/tests/watermelon-cat.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/tox.ini
```

### Comparing `django-minio-storage-0.3.8/CHANGELOG.md` & `django-minio-storage-0.5.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+## 0.5.0
+
+Switched the minio-py client library version from `<7` to `>=7`.
+
+Minimum Django version is now 3.2
+
+Minimum Python version is now 3.8
+
+## 0.3.9
+
+The minio client is now deconstructable by Django, fixes migrations.
+
 ## 0.3.8
 
 Improved presigned urls with non standard base urls
 
 ## 0.3.7
 
 Removed accidentally left over debug print from previous release
```

### Comparing `django-minio-storage-0.3.8/LICENSE-APACHE` & `django-minio-storage-0.5.0/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.3.8/LICENSE-MIT` & `django-minio-storage-0.5.0/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.3.8/README.md` & `django-minio-storage-0.5.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 [![PyPI version](https://badge.fury.io/py/django-minio-storage.svg)](https://badge.fury.io/py/django-minio-storage)
 [![Documentation Status](http://readthedocs.org/projects/django-minio-storage/badge/?version=latest)](http://django-minio-storage.readthedocs.io/en/latest/?badge=latest)
-[![Build Status](https://travis-ci.org/py-pa/django-minio-storage.svg?branch=master)](https://travis-ci.org/py-pa/django-minio-storage)
 
 # django-minio-storage
 
 Use [minio](https://minio.io) for django static and media file storage.
 
 Minio is accessed through the Amazon S3 API, so existing django file storage
 adapters for S3 should work, but in practice they are hard to configure. This
```

### Comparing `django-minio-storage-0.3.8/django_minio_storage.egg-info/SOURCES.txt` & `django-minio-storage-0.5.0/django_minio_storage.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 .editorconfig
 .flake8rc
 .gitignore
 .isort.cfg
-.travis.yml
+.readthedocs.yaml
 CHANGELOG.md
 CONTRIBUTING.md
 LICENSE-APACHE
 LICENSE-MIT
 README.md
 dev-requirements.txt
 docker-compose.yml
+docs-requirements.txt
 mkdocs.yml
 pyproject.toml
 setup.py
 tox.ini
+.github/workflows/release.yml
+.github/workflows/tox.yml
 django_minio_storage.egg-info/PKG-INFO
 django_minio_storage.egg-info/SOURCES.txt
 django_minio_storage.egg-info/dependency_links.txt
 django_minio_storage.egg-info/requires.txt
 django_minio_storage.egg-info/top_level.txt
 docs/contributing.md
 docs/contributors.md
@@ -27,14 +30,15 @@
 docs/usage.md
 minio_storage/__init__.py
 minio_storage/apps.py
 minio_storage/errors.py
 minio_storage/files.py
 minio_storage/policy.py
 minio_storage/storage.py
+minio_storage/version.py
 minio_storage/management/__init__.py
 minio_storage/management/commands/__init__.py
 minio_storage/management/commands/minio.py
 tests/__init__.py
 tests/manage.py
 tests/watermelon-cat.jpg
 tests/django_minio_storage_tests/__init__.py
```

### Comparing `django-minio-storage-0.3.8/docs/development.md` & `django-minio-storage-0.5.0/docs/development.md`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.3.8/docs/index.md` & `django-minio-storage-0.5.0/docs/index.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,13 +6,13 @@
 Minio is accessed through the Amazon S3 API, so existing django file storage
 adapters for S3 should work, but in practice they are hard to configure. This
 project uses the minio python client instead. Inspiration has been drawn from
 `django-s3-storage` and `django-storages`.
 
 # Compatibility
 
-CI is currenlty executed on Python 3.6+ and Django 1.11+.
+CI is currenlty executed on Python 3.8+ and Django 3.2+.
 
 The goal is to have a thoroughly tested, small code base that delegates as much
 as possible to the minio client.
 
 - Release versioning is semver compliant.
```

### Comparing `django-minio-storage-0.3.8/docs/licences.md` & `django-minio-storage-0.5.0/docs/licences.md`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.3.8/docs/usage.md` & `django-minio-storage-0.5.0/docs/usage.md`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.3.8/minio_storage/files.py` & `django-minio-storage-0.5.0/minio_storage/files.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import tempfile
 import typing as T
 from logging import getLogger
 
 from django.core.files.base import File
 from minio import error as merr
+
 from minio_storage.errors import minio_error
 
 if T.TYPE_CHECKING:
     from minio_storage.storage import Storage
 
 logger = getLogger("minio_storage")
 
@@ -40,18 +41,18 @@
         self.name: str = name
         self._mode: str = mode
         self._file = None
 
 
 class ReadOnlyMinioObjectFile(MinioStorageFile, ReadOnlyMixin, NonSeekableMixin):
     """A django File class which directly exposes the underlying minio object. This
-means the the instance doesnt support functions like .seek() and is required to
-be closed to be able to reuse minio connections.
+    means the the instance doesnt support functions like .seek() and is required to
+    be closed to be able to reuse minio connections.
 
-Note: This file class is not tested yet"""
+    Note: This file class is not tested yet"""
 
     def __init__(
         self,
         name: str,
         mode: str,
         storage: "Storage",
         max_memory_size: T.Optional[int] = None,
@@ -69,15 +70,15 @@
         if self._file is None:
             try:
                 obj = self._storage.client.get_object(
                     self._storage.bucket_name, self.name
                 )
                 self._file = obj
                 return self._file
-            except merr.ResponseError as error:
+            except merr.InvalidResponseError as error:
                 logger.warn(error)
                 raise OSError(f"File {self.name} does not exist")
             finally:
                 try:
                     obj.release_conn()
                 except Exception as e:
                     logger.error(str(e))
@@ -93,15 +94,15 @@
             self.file.close()
         finally:
             self.file.release_conn()
 
 
 class ReadOnlySpooledTemporaryFile(MinioStorageFile, ReadOnlyMixin):
     """A django File class which buffers the minio object into a local
-SpooledTemporaryFile. """
+    SpooledTemporaryFile."""
 
     max_memory_size: int = 1024 * 1024 * 10
 
     def __init__(
         self,
         name: str,
         mode: str,
@@ -126,15 +127,15 @@
                 self._file = tempfile.SpooledTemporaryFile(
                     max_size=self.max_memory_size
                 )
                 for d in obj.stream(amt=1024 * 1024):
                     self._file.write(d)
                 self._file.seek(0)
                 return self._file
-            except merr.ResponseError as error:
+            except merr.InvalidResponseError as error:
                 raise minio_error(f"File {self.name} does not exist", error)
             finally:
                 try:
                     obj.release_conn()
                 except Exception as e:
                     logger.error(str(e))
         return self._file
```

### Comparing `django-minio-storage-0.3.8/minio_storage/management/commands/minio.py` & `django-minio-storage-0.5.0/minio_storage/management/commands/minio.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,33 @@
+import argparse
 import json
 import sys
 from string import Template
 from unittest.mock import patch
 
 import minio.error
 from django.core.management.base import BaseCommand, CommandError
 from django.utils.module_loading import import_string
+
 from minio_storage.policy import Policy
 from minio_storage.storage import MinioStorage
-import argparse
 
 
 class Command(BaseCommand):
     help = "verify, list, create and delete minio buckets"
 
     CHECK = "check"
     CREATE = "create"
     DELETE = "delete"
     LIST = "ls"
     POLICY = "policy"
 
     FULL_FORMAT = "$name $size $modified $url $etag"
 
     def add_arguments(self, parser):
-
         group = parser.add_argument_group("minio")
         group.add_argument(
             "--class",
             type=str,
             default="minio_storage.storage.MinioMediaStorage",
             help="Storage class to modify "
             "(media/static are short names for default classes)",
@@ -162,15 +162,15 @@
         list_dirs: bool,
         list_files: bool,
         recursive: bool,
         format: str = None,
         summary: bool = True,
     ):
         try:
-            objs = storage.client.list_objects_v2(
+            objs = storage.client.list_objects(
                 bucket_name, prefix=prefix, recursive=recursive
             )
 
             template = None
             if format is not None and format != "$name":
                 template = Template(format)
 
@@ -195,43 +195,45 @@
                 else:
                     n_files += 1
                     if list_files:
                         self.stdout.write(fmt(o))
 
             if summary:
                 print(f"{n_files} files and {n_dirs} directories", file=sys.stderr)
-        except minio.error.NoSuchBucket:
-            raise CommandError(f"bucket {bucket_name} does not exist")
+        except minio.error.S3Error as e:
+            raise CommandError(f"error reading bucket {bucket_name}") from e
 
     def bucket_create(self, storage, bucket_name):
         try:
             storage.client.make_bucket(bucket_name)
             print(f"created bucket: {bucket_name}", file=sys.stderr)
-        except minio.error.BucketAlreadyOwnedByYou:
-            raise CommandError(f"you have already created {bucket_name}")
+        except minio.error.S3Error as e:
+            raise CommandError(f"error creating {bucket_name}") from e
         return
 
     def bucket_delete(self, storage, bucket_name):
         try:
             storage.client.remove_bucket(bucket_name)
-        except minio.error.NoSuchBucket:
-            raise CommandError(f"bucket {bucket_name} does not exist")
-        except minio.error.BucketNotEmpty:
-            raise CommandError(f"bucket {bucket_name} is not empty")
+        except minio.error.S3Error as err:
+            if err.code == "BucketNotEmpty":
+                raise CommandError(f"bucket {bucket_name} is not empty")
+            elif err.code == "NoSuchBucket":
+                raise CommandError(f"bucket {bucket_name} does not exist")
 
     def policy_get(self, storage, bucket_name):
         try:
             policy = storage.client.get_bucket_policy(bucket_name)
             policy = json.loads(policy)
             policy = json.dumps(policy, ensure_ascii=False, indent=2)
             return policy
-        except minio.error.NoSuchBucket:
-            raise CommandError(f"bucket {bucket_name} does not exist")
-        except minio.error.NoSuchBucketPolicy:
-            raise CommandError(f"bucket {bucket_name} has no policy")
+        except minio.error.S3Error as err:
+            if err.code == "NoSuchBucket":
+                raise CommandError(f"bucket {bucket_name} does not exist")
+            elif err.code == "NoSuchBucketPolicy":
+                raise CommandError(f"bucket {bucket_name} has no policy")
 
     def policy_set(self, storage, bucket_name, policy: Policy):
         try:
             policy = Policy(policy)
             storage.client.set_bucket_policy(bucket_name, policy.bucket(bucket_name))
-        except minio.error.NoSuchBucket as e:
-            raise CommandError(e.message)
+        except minio.error.S3Error as e:
+            raise CommandError(e.message) from e
```

### Comparing `django-minio-storage-0.3.8/minio_storage/policy.py` & `django-minio-storage-0.5.0/minio_storage/policy.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.3.8/minio_storage/storage.py` & `django-minio-storage-0.5.0/minio_storage/storage.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 import datetime
 import mimetypes
 import posixpath
 import typing as T
 import urllib
 from logging import getLogger
-from time import mktime
 from urllib.parse import urlsplit, urlunsplit
 
 import minio
 import minio.error as merr
 from django.conf import settings
 from django.core.exceptions import ImproperlyConfigured
 from django.core.files.storage import Storage
 from django.utils import timezone
 from django.utils.deconstruct import deconstructible
-from minio.helpers import get_target_url
 
 from minio_storage.errors import minio_error
 from minio_storage.files import ReadOnlySpooledTemporaryFile
 from minio_storage.policy import Policy
 
 logger = getLogger("minio_storage")
 
@@ -105,26 +103,27 @@
     def _create_base_url_client(client: minio.Minio, bucket_name: str, base_url: str):
         """
         Clone a Minio client, using a different endpoint from `base_url`.
         """
         base_url_parts = urlsplit(base_url)
 
         # Clone from the normal client, but with base_url as the endpoint
+        credentials = client._provider.retrieve()
         base_url_client = minio.Minio(
             base_url_parts.netloc,
-            access_key=client._access_key,
-            secret_key=client._secret_key,
-            session_token=client._session_token,
-            secure=base_url_parts.scheme == 'https',
+            access_key=credentials.access_key,
+            secret_key=credentials.secret_key,
+            session_token=credentials.session_token,
+            secure=base_url_parts.scheme == "https",
             # The bucket region may be auto-detected by client (via an HTTP
             # request), so don't just use client._region
-            region=client._get_bucket_region(bucket_name),
-            http_client=client._http
+            region=client._get_region(bucket_name, None),
+            http_client=client._http,
         )
-        if hasattr(client, '_credentials'):
+        if hasattr(client, "_credentials"):
             # Client credentials do not exist prior to minio-py 5.0.7, but
             # they should be reused if possible
             base_url_client._credentials = client._credentials
 
         return base_url_client
 
     def _sanitize_path(self, name):
@@ -147,16 +146,16 @@
         content_type = content_type[0] or "application/octet-stream"
         sane_name = self._sanitize_path(name)
         return (content_size, content_type, sane_name)
 
     def _open(self, name, mode="rb"):
         try:
             f = self.file_class(self._sanitize_path(name), mode, self)
-        except merr.MinioError as e:
-            raise minio_error("File {} could not be saved: {}".format(name, str(e)), e)
+        except merr.MinioException as e:
+            raise minio_error(f"File {name} could not be saved: {str(e)}", e)
         return f
 
     def _save(self, name: str, content: bytes) -> str:
         try:
             if hasattr(content, "seek") and callable(content.seek):
                 content.seek(0)
             content_size, content_type, sane_name = self._examine_file(name, content)
@@ -165,22 +164,22 @@
                 sane_name,
                 content,
                 content_size,
                 content_type,
                 metadata=self.object_metadata,
             )
             return sane_name
-        except merr.ResponseError as error:
+        except merr.InvalidResponseError as error:
             raise minio_error(f"File {name} could not be saved", error)
 
     def delete(self, name: str) -> None:
         if self.backup_format and self.backup_bucket:
             try:
                 obj = self.client.get_object(self.bucket_name, name)
-            except merr.ResponseError as error:
+            except merr.InvalidResponseError as error:
                 raise minio_error(
                     "Could not obtain file {} " "to make a copy of it".format(name),
                     error,
                 )
 
             try:
                 content_length = int(obj.getheader("Content-Length"))
@@ -191,39 +190,39 @@
             target_name = "{}{}".format(
                 timezone.now().strftime(self.backup_format), name
             )
             try:
                 self.client.put_object(
                     self.backup_bucket, target_name, obj, content_length
                 )
-            except merr.ResponseError as error:
+            except merr.InvalidResponseError as error:
                 raise minio_error(
                     "Could not make a copy of file "
                     "{} before removing it".format(name),
                     error,
                 )
 
         try:
             self.client.remove_object(self.bucket_name, name)
-        except merr.ResponseError as error:
+        except merr.InvalidResponseError as error:
             raise minio_error(f"Could not remove file {name}", error)
 
     def exists(self, name: str) -> bool:
         try:
             self.client.stat_object(self.bucket_name, self._sanitize_path(name))
             return True
-        except merr.ResponseError as error:
+        except merr.InvalidResponseError as error:
             # TODO - deprecate
             if error.code == "NoSuchKey":
                 return False
             else:
                 raise minio_error(f"Could not stat file {name}", error)
-        except merr.NoSuchKey:
+        except merr.S3Error:
             return False
-        except merr.NoSuchBucket:
+        except merr.S3Error:
             raise
         except Exception as error:
             logger.error(error)
 
     def listdir(self, path: str) -> T.Tuple[T.List, T.List]:
         #  [None, "", "."] is supported to mean the configured root among various
         #  implementations of Storage implementations so we copy that behaviour even if
@@ -238,100 +237,101 @@
         else:
             if not path.endswith("/"):
                 path += "/"
 
         dirs: T.List[str] = []
         files: T.List[str] = []
         try:
-            objects = self.client.list_objects_v2(self.bucket_name, prefix=path)
+            objects = self.client.list_objects(self.bucket_name, prefix=path)
             for o in objects:
                 p = posixpath.relpath(o.object_name, path)
                 if o.is_dir:
                     dirs.append(p)
                 else:
                     files.append(p)
             return dirs, files
-        except merr.NoSuchBucket:
+        except merr.S3Error:
             raise
-        except merr.ResponseError as error:
+        except merr.InvalidResponseError as error:
             raise minio_error(f"Could not list directory {path}", error)
 
     def size(self, name: str) -> int:
         try:
             info = self.client.stat_object(self.bucket_name, name)
             return info.size
-        except merr.ResponseError as error:
+        except merr.InvalidResponseError as error:
             raise minio_error(f"Could not access file size for {name}", error)
 
     def _presigned_url(
         self, name: str, max_age: T.Optional[datetime.timedelta] = None
     ) -> str:
         kwargs = {}
         if max_age is not None:
             kwargs["expires"] = max_age
 
-        client = (
-            self.client
-            if self.base_url is None else
-            self.base_url_client
-        )
+        client = self.client if self.base_url is None else self.base_url_client
         url = client.presigned_get_object(self.bucket_name, name, **kwargs)
 
         if self.base_url is not None:
             url_parts = urlsplit(url)
             base_url_parts = urlsplit(self.base_url)
 
             # It's assumed that self.base_url will contain bucket information,
             # which could be different, so remove the bucket_name component (with 1
             # extra character for the leading "/") from the generated URL
-            url_key_path = url_parts.path[len(self.bucket_name) + 1:]
+            url_key_path = url_parts.path[len(self.bucket_name) + 1 :]
 
             # Prefix the URL with any path content from base_url
             new_url_path = base_url_parts.path + url_key_path
 
             # Reconstruct the URL with an updated path
-            url = urlunsplit((
-                url_parts.scheme,
-                url_parts.netloc,
-                new_url_path,
-                url_parts.query,
-                url_parts.fragment
-            ))
+            url = urlunsplit(
+                (
+                    url_parts.scheme,
+                    url_parts.netloc,
+                    new_url_path,
+                    url_parts.query,
+                    url_parts.fragment,
+                )
+            )
         return url
 
     def url(
         self, name: str, *args, max_age: T.Optional[datetime.timedelta] = None
     ) -> str:
         if self.presign_urls:
             url = self._presigned_url(name, max_age=max_age)
         else:
-            if self.base_url is not None:
 
-                def strip_beg(path):
-                    while path.startswith("/"):
-                        path = path[1:]
-                    return path
-
-                def strip_end(path):
-                    while path.endswith("/"):
-                        path = path[:-1]
-                    return path
+            def strip_beg(path):
+                while path.startswith("/"):
+                    path = path[1:]
+                return path
+
+            def strip_end(path):
+                while path.endswith("/"):
+                    path = path[:-1]
+                return path
 
+            if self.base_url is not None:
                 url = "{}/{}".format(
                     strip_end(self.base_url), urllib.parse.quote(strip_beg(name))
                 )
             else:
-                url = get_target_url(
-                    self.client._endpoint_url,
-                    bucket_name=self.bucket_name,
-                    object_name=name,
-                    # bucket_region=region,
+                url = "{}/{}/{}".format(
+                    strip_end(self.endpoint_url),
+                    self.bucket_name,
+                    urllib.parse.quote(strip_beg(name)),
                 )
         return url
 
+    @property
+    def endpoint_url(self):
+        return self.client._base_url._url.geturl()
+
     def accessed_time(self, name: str) -> datetime.datetime:
         """
         Not available via the S3 API
         """
         return self.modified_time(name)
 
     def created_time(self, name: str) -> datetime.datetime:
@@ -339,16 +339,16 @@
         Not available via the S3 API
         """
         return self.modified_time(name)
 
     def modified_time(self, name: str) -> datetime.datetime:
         try:
             info = self.client.stat_object(self.bucket_name, name)
-            return datetime.datetime.fromtimestamp(mktime(info.last_modified))
-        except merr.ResponseError as error:
+            return info.last_modified
+        except merr.InvalidResponseError as error:
             raise minio_error(
                 f"Could not access modification time for file {name}", error
             )
 
 
 _NoValue = object()
 
@@ -363,15 +363,19 @@
 
 
 def create_minio_client_from_settings(*, minio_kwargs=dict()):
     endpoint = get_setting("MINIO_STORAGE_ENDPOINT")
     access_key = get_setting("MINIO_STORAGE_ACCESS_KEY")
     secret_key = get_setting("MINIO_STORAGE_SECRET_KEY")
     secure = get_setting("MINIO_STORAGE_USE_HTTPS", True)
-    client = minio.Minio(
+    # Making this client deconstructible allows it to be passed directly as
+    # an argument to MinioStorage, since Django needs to be able to
+    # deconstruct all Storage constructor arguments for Storages referenced in
+    # migrations (e.g. when using a custom storage on a FileField).
+    client = deconstructible(minio.Minio)(
         endpoint,
         access_key=access_key,
         secret_key=secret_key,
         secure=secure,
         **minio_kwargs,
     )
     return client
```

### Comparing `django-minio-storage-0.3.8/tests/django_minio_storage_tests/settings.py` & `django-minio-storage-0.5.0/tests/django_minio_storage_tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.3.8/tests/django_minio_storage_tests/urls.py` & `django-minio-storage-0.5.0/tests/django_minio_storage_tests/urls.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,11 +9,11 @@
 Class-based views
     1. Add an import:  from other_app.views import Home
     2. Add a URL to urlpatterns:  url(r'^$', Home.as_view(), name='home')
 Including another URLconf
     1. Import the include() function: from django.conf.urls import url, include
     2. Add a URL to urlpatterns:  url(r'^blog/', include('blog.urls'))
 """
-from django.conf.urls import url
 from django.contrib import admin
+from django.urls import path
 
-urlpatterns = [url(r"^admin/", admin.site.urls)]
+urlpatterns = [path("admin/", admin.site.urls)]
```

### Comparing `django-minio-storage-0.3.8/tests/test_app/tests/bucket_tests.py` & `django-minio-storage-0.5.0/tests/test_app/tests/bucket_tests.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 
-import requests
-
 import minio
+import requests
 from django.core.exceptions import ImproperlyConfigured
 from django.core.files.base import ContentFile
 from django.test import TestCase, override_settings
+
 from minio_storage.policy import Policy
 from minio_storage.storage import MinioMediaStorage, MinioStaticStorage, get_setting
 
 from .utils import BaseTestMixin
 
 
 class BucketTests(BaseTestMixin, TestCase):
@@ -73,15 +73,15 @@
 
     @override_settings(
         MINIO_STORAGE_AUTO_CREATE_MEDIA_BUCKET=True,
         MINIO_STORAGE_AUTO_CREATE_MEDIA_POLICY=False,
     )
     def test_auto_create_no_policy(self):
         ms = MinioMediaStorage()
-        with self.assertRaises(minio.error.NoSuchBucketPolicy):
+        with self.assertRaises(minio.error.S3Error):
             ms.client.get_bucket_policy(ms.bucket_name)
 
     @override_settings(
         MINIO_STORAGE_AUTO_CREATE_MEDIA_POLICY=True,
         MINIO_STORAGE_AUTO_CREATE_MEDIA_BUCKET=True,
     )
     def test_media_policy_auto_true(self):
@@ -92,15 +92,15 @@
             json.loads(ms.client.get_bucket_policy(ms.bucket_name)),
         )
         fn = ms.save("somefile", ContentFile(b"test"))
         self.assertEqual(ms.open(fn).read(), b"test")
         url = ms.url(fn)
         self.assertEqual(requests.get(url).status_code, 200)
         self.assertEqual(
-            requests.get(f"{ms.client._endpoint_url}/{ms.bucket_name}").status_code, 403
+            requests.get(f"{ms.endpoint_url}/{ms.bucket_name}").status_code, 403
         )
 
     @override_settings(
         MINIO_STORAGE_AUTO_CREATE_MEDIA_POLICY="GET_ONLY",
         MINIO_STORAGE_AUTO_CREATE_MEDIA_BUCKET=True,
     )
     def test_media_policy_get(self):
@@ -110,15 +110,15 @@
             Policy.get.bucket(ms.bucket_name, json_encode=False),
             json.loads(ms.client.get_bucket_policy(ms.bucket_name)),
         )
         fn = ms.save("somefile", ContentFile(b"test"))
         self.assertEqual(ms.open(fn).read(), b"test")
         self.assertEqual(requests.get(ms.url(fn)).status_code, 200)
         self.assertEqual(
-            requests.get(f"{ms.client._endpoint_url}/{ms.bucket_name}").status_code, 403
+            requests.get(f"{ms.endpoint_url}/{ms.bucket_name}").status_code, 403
         )
 
     @override_settings(
         MINIO_STORAGE_AUTO_CREATE_MEDIA_POLICY="WRITE_ONLY",
         MINIO_STORAGE_AUTO_CREATE_MEDIA_BUCKET=True,
     )
     def test_media_policy_write(self):
@@ -128,15 +128,15 @@
             Policy.write.bucket(ms.bucket_name, json_encode=False),
             json.loads(ms.client.get_bucket_policy(ms.bucket_name)),
         )
         fn = ms.save("somefile", ContentFile(b"test"))
         self.assertEqual(ms.open(fn).read(), b"test")
         self.assertEqual(requests.get(ms.url(fn)).status_code, 403)
         self.assertEqual(
-            requests.get(f"{ms.client._endpoint_url}/{ms.bucket_name}").status_code, 403
+            requests.get(f"{ms.endpoint_url}/{ms.bucket_name}").status_code, 403
         )
 
     @override_settings(
         MINIO_STORAGE_AUTO_CREATE_MEDIA_POLICY="READ_WRITE",
         MINIO_STORAGE_AUTO_CREATE_MEDIA_BUCKET=True,
     )
     def test_media_policy_rw(self):
```

### Comparing `django-minio-storage-0.3.8/tests/test_app/tests/custom_storage_class_tests.py` & `django-minio-storage-0.5.0/tests/test_app/tests/custom_storage_class_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os
 import shutil
 import tempfile
 
 from django.core.files.base import ContentFile
 from django.test import TestCase, override_settings
 from django.utils.deconstruct import deconstructible
+
 from minio_storage.files import ReadOnlyMinioObjectFile
 from minio_storage.storage import (
     MinioStorage,
     create_minio_client_from_settings,
     get_setting,
 )
 
@@ -37,15 +38,14 @@
     # we want to stream the data directly from minio. Imagine that we need to process
     # large files where we don't want to waste time/ram/disk space on  writing the file
     # to disk two times before processing it.
     #
     file_class = ReadOnlyMinioObjectFile
 
     def __init__(self, bucket_name=None):
-
         # we can create the minio client ourselves or use
         # create_minio_client_from_settings convinience function while providing it with
         # extra args.
         #
         client = create_minio_client_from_settings(minio_kwargs={"region": "us-east-1"})
 
         # or use our own Django setting
@@ -77,29 +77,27 @@
 
         # Create a temporary workspace directory.
         #
         # It's importat that this directory is deleted after we are done so we use the
         # with statement here.
         #
         with tempfile.TemporaryDirectory() as workspace:
-
             # A filename to use for the file inside the working directory.
             #
             filename = os.path.join(workspace, "secret.txt")
 
             # Open a stream with the minio file objenct and the temporary file.
             #
             # We might be processing a lot of files in a loop here so we are going top
             # use the with statement to ensure that both the input stream and output
             # files are closed after the copying is done.
             #
             with open(filename, "wb") as out_file, storage.open(
                 storage_filename
             ) as storage_file:
-
                 # Copy the stream from the http stream to the out_file
                 #
                 shutil.copyfileobj(storage_file.file, out_file)
 
                 #
                 # We are not using the ReadOnlyMinioObjectFile type so we can't seek in
                 # it.
```

### Comparing `django-minio-storage-0.3.8/tests/test_app/tests/delete_tests.py` & `django-minio-storage-0.5.0/tests/test_app/tests/delete_tests.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.3.8/tests/test_app/tests/managementcommand_tests.py` & `django-minio-storage-0.5.0/tests/test_app/tests/managementcommand_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,59 +1,59 @@
 from io import StringIO
 
 import minio
 from django.core.files.base import ContentFile
 from django.core.management import call_command
 from django.core.management.base import CommandError
 from django.test import TestCase, override_settings
+
 from minio_storage.policy import Policy
 
 from .utils import BaseTestMixin, bucket_name
 
 
 @override_settings(
     MINIO_STORAGE_MEDIA_USE_PRESIGNED=False, MINIO_STORAGE_STATIC_USE_PRESIGNED=False
 )
 class CommandsTests(BaseTestMixin, TestCase):
     @override_settings(
         MINIO_STORAGE_AUTO_CREATE_MEDIA_BUCKET=False,
         MINIO_STORAGE_AUTO_CREATE_MEDIA_POLICY=False,
     )
     def test_management_command(self):
-
         storage = self.media_storage
         bucket = self.media_storage.bucket_name
 
         call_command("minio", "check")
 
         with self.assertRaisesRegex(CommandError, f"bucket {bucket} is not empty"):
             call_command("minio", "delete")
 
         try:
             self.obliterate_bucket(self.media_storage.bucket_name)
-        except minio.error.NoSuchBucket:
+        except minio.error.S3Error:
             pass
 
         with self.assertRaisesRegex(CommandError, f"bucket {bucket} does not exist"):
             call_command("minio", "check")
 
         with self.assertRaisesRegex(CommandError, f"bucket {bucket} does not exist"):
             call_command("minio", "policy")
 
-        with self.assertRaisesRegex(CommandError, f"bucket {bucket} does not exist"):
+        with self.assertRaisesRegex(CommandError, f"error reading bucket {bucket}"):
             call_command("minio", "ls")
 
         with self.assertRaisesRegex(CommandError, f"bucket {bucket} does not exist"):
             call_command("minio", "delete")
 
         call_command("minio", "create")
 
         call_command("minio", "check")
 
-        with self.assertRaisesRegex(CommandError, f"you have already created {bucket}"):
+        with self.assertRaisesRegex(CommandError, f"error creating {bucket}"):
             call_command("minio", "create")
 
         with self.assertRaisesRegex(CommandError, f"bucket {bucket} has no policy"):
             call_command("minio", "policy")
 
         for p in [p.value for p in Policy]:
             call_command("minio", "policy", "--set", p)
```

### Comparing `django-minio-storage-0.3.8/tests/test_app/tests/retrieve_tests.py` & `django-minio-storage-0.5.0/tests/test_app/tests/retrieve_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import datetime
 import io
 import os
+import unittest
 
 import requests
-from freezegun import freeze_time
-
 from django.core.files.base import ContentFile
 from django.test import TestCase, override_settings
-from minio.error import NoSuchKey
+from freezegun import freeze_time
+from minio.error import S3Error
+
 from minio_storage.errors import MinIOError
 from minio_storage.storage import MinioMediaStorage
-import unittest
+
 from .utils import BaseTestMixin
 
 
 @override_settings(
     MINIO_STORAGE_MEDIA_USE_PRESIGNED=True, MINIO_STORAGE_STATIC_USE_PRESIGNED=True
 )
 class RetrieveTestsWithRestrictedBucket(BaseTestMixin, TestCase):
@@ -39,15 +40,15 @@
     def test_file_size(self):
         test_file = self.media_storage.save("sizetest.txt", ContentFile(b"1234"))
         self.assertEqual(4, self.media_storage.size(test_file))
 
     def test_size_of_non_existent_throws(self):
         test_file = self.media_storage.save("sizetest.txt", ContentFile(b"1234"))
         self.media_storage.delete(test_file)
-        with self.assertRaises(NoSuchKey):
+        with self.assertRaises(S3Error):
             self.media_storage.size(test_file)
 
     def test_modified_time(self):
         self.assertIsInstance(
             self.media_storage.modified_time(self.new_file), datetime.datetime
         )
 
@@ -58,15 +59,15 @@
 
     def test_created_time(self):
         self.assertIsInstance(
             self.media_storage.created_time(self.new_file), datetime.datetime
         )
 
     def test_modified_time_of_non_existent_throws(self):
-        with self.assertRaises(NoSuchKey):
+        with self.assertRaises(S3Error):
             self.media_storage.modified_time("nonexistent.jpg")
 
     def _listdir_root(self, root):
         self.media_storage.save("dir1/file2.txt", ContentFile(b"meh"))
         test_dir = self.media_storage.listdir(root)
         (dirs, files) = test_dir
         self.assertEqual(dirs, ["dir1"])
@@ -123,15 +124,15 @@
     @unittest.skip("Skipping this test because undecided if it should raise exception")
     def test_opening_non_existing_file_raises_minioerror(self):
         with self.assertRaises(MinIOError):
             self.media_storage.open("this does not exist")
         try:
             self.media_storage.open("this does not exist")
         except MinIOError as e:
-            assert e.cause.__class__ == NoSuchKey
+            assert e.cause.__class__ == S3Error
 
     def test_file_names_are_properly_sanitized(self):
         self.media_storage.save("./meh22222.txt", io.BytesIO(b"stuff"))
 
     def test_url_max_age(self):
         url = self.media_storage.url(
             "test-file", max_age=datetime.timedelta(seconds=10)
```

### Comparing `django-minio-storage-0.3.8/tests/test_app/tests/upload_tests.py` & `django-minio-storage-0.5.0/tests/test_app/tests/upload_tests.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 
 import requests
 from django.conf import settings
 from django.core.files.base import ContentFile, File
 from django.test import TestCase, override_settings
-from minio.error import InvalidAccessKeyId
+from minio.error import S3Error
 
 from minio_storage.storage import MinioMediaStorage
 
 from .utils import BaseTestMixin
 
 
 @override_settings(
@@ -18,15 +18,15 @@
     def test_file_upload_success(self):
         self.media_storage.save("trivial.txt", ContentFile(b"12345"))
 
     @override_settings(
         MINIO_STORAGE_ACCESS_KEY="wrong_key", MINIO_STORAGE_SECRET_KEY="wrong_secret"
     )
     def test_file_upload_fail_incorrect_keys(self):
-        with self.assertRaises(InvalidAccessKeyId):
+        with self.assertRaises(S3Error):
             MinioMediaStorage()
 
     def test_two_files_with_the_same_name_can_be_uploaded(self):
         ivan = self.media_storage.save("pelican.txt", ContentFile(b"Ivan le Pelican"))
         jean = self.media_storage.save("pelican.txt", ContentFile(b"Jean le Pelican"))
         self.assertNotEqual(jean, ivan)
 
@@ -84,23 +84,34 @@
         self.assertFalse(self.media_storage.exists(".hidden_file"))
 
     def test_metadata(self):
         ivan = self.media_storage.save("pelican.txt", ContentFile(b"Ivan le Pelican"))
         res = self.media_storage.client.stat_object(
             self.media_storage.bucket_name, ivan
         )
-        self.assertEqual(res.metadata, {"Content-Type": "text/plain"})
+        metadata_attrs = {
+            "Accept-Ranges",
+            "Content-Length",
+            "Content-Security-Policy",
+            "Content-Type",
+            "ETag",
+            "Last-Modified",
+            "Server",
+            "Vary",
+            "X-Amz-Request-Id",
+            "X-Xss-Protection",
+            "Date",
+        }
+        self.assertTrue(metadata_attrs.issubset(res.metadata.keys()))
 
 
 @override_settings(
     MINIO_STORAGE_MEDIA_OBJECT_METADATA={"Cache-Control": "max-age=1000"},
 )
 class TestDefaultObjectMetadata(BaseTestMixin, TestCase):
     def test_default_metadata(self):
         ivan = self.media_storage.save("pelican.txt", ContentFile(b"Ivan le Pelican"))
         res = self.media_storage.client.stat_object(
             self.media_storage.bucket_name, ivan
         )
-        self.assertEqual(
-            res.metadata,
-            {"Cache-Control": "max-age=1000", "Content-Type": "text/plain"},
-        )
+
+        self.assertEqual(res.metadata["Cache-Control"], "max-age=1000")
```

### Comparing `django-minio-storage-0.3.8/tests/test_app/tests/utils.py` & `django-minio-storage-0.5.0/tests/test_app/tests/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import hashlib
 import os
 import warnings
 
 from django.core.files.base import ContentFile
 from minio import Minio
+
 from minio_storage.storage import MinioMediaStorage, MinioStaticStorage, get_setting
 
 warnings.simplefilter("default")
 warnings.filterwarnings(
     "ignore", message="This usage is deprecated, please use pytest.* instead"
 )
 
@@ -48,10 +49,8 @@
 
     def obliterate_bucket(self, name, client=None):
         if client is None:
             client = self.minio_client()
 
         for obj in client.list_objects(name, "", True):
             client.remove_object(name, obj.object_name)
-        for obj in client.list_incomplete_uploads(name, ""):  # pragma: no cover  # noqa
-            client.remove_incomplete_upload(name, obj.objectname)
         client.remove_bucket(name)
```

### Comparing `django-minio-storage-0.3.8/tests/watermelon-cat.jpg` & `django-minio-storage-0.5.0/tests/watermelon-cat.jpg`

 * *Files identical despite different names*

