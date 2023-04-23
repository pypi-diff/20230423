# Comparing `tmp/django-minio-storage-0.3.7.tar.gz` & `tmp/django-minio-storage-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-minio-storage-0.3.7.tar", last modified: Wed Feb 26 08:25:46 2020, max compression
+gzip compressed data, was "dist/django-minio-storage-0.3.8.tar", last modified: Thu Jul  9 12:59:38 2020, max compression
```

## Comparing `django-minio-storage-0.3.7.tar` & `django-minio-storage-0.3.8.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxr-x   0 thomasf   (1000) thomasf   (1000)        0 2020-02-26 08:25:46.000000 django-minio-storage-0.3.7/
--rw-r--r--   0 thomasf   (1000) thomasf   (1000)      197 2019-10-16 20:54:45.000000 django-minio-storage-0.3.7/.editorconfig
--rw-r--r--   0 thomasf   (1000) thomasf   (1000)       92 2019-10-16 20:50:16.000000 django-minio-storage-0.3.7/.flake8rc
--rw-rw-r--   0 thomasf   (1000) thomasf   (1000)      100 2019-12-16 11:38:04.000000 django-minio-storage-0.3.7/.gitignore
--rw-rw-r--   0 thomasf   (1000) thomasf   (1000)      259 2019-10-17 17:09:29.000000 django-minio-storage-0.3.7/.isort.cfg
--rw-rw-r--   0 thomasf   (1000) thomasf   (1000)     1448 2019-10-18 12:43:28.000000 django-minio-storage-0.3.7/.travis.yml
--rw-rw-r--   0 thomasf   (1000) thomasf   (1000)     3010 2020-02-26 08:24:31.000000 django-minio-storage-0.3.7/CHANGELOG.md
--rw-r--r--   0 thomasf   (1000) thomasf   (1000)       43 2018-07-12 19:09:03.000000 django-minio-storage-0.3.7/CONTRIBUTING.md
--rw-r--r--   0 thomasf   (1000) thomasf   (1000)    11004 2018-07-12 19:09:03.000000 django-minio-storage-0.3.7/LICENSE-APACHE
--rw-r--r--   0 thomasf   (1000) thomasf   (1000)     1102 2018-07-12 19:09:03.000000 django-minio-storage-0.3.7/LICENSE-MIT
--rw-rw-r--   0 thomasf   (1000) thomasf   (1000)      653 2020-02-26 08:25:46.000000 django-minio-storage-0.3.7/PKG-INFO
--rw-r--r--   0 thomasf   (1000) thomasf   (1000)      965 2018-07-12 19:09:03.000000 django-minio-storage-0.3.7/README.md
--rw-rw-r--   0 thomasf   (1000) thomasf   (1000)      137 2019-10-22 03:11:11.000000 django-minio-storage-0.3.7/dev-requirements.txt
-drwxrwxr-x   0 thomasf   (1000) thomasf   (1000)        0 2020-02-26 08:25:46.000000 django-minio-storage-0.3.7/django_minio_storage.egg-info/
--rw-rw-r--   0 thomasf   (1000) thomasf   (1000)      653 2020-02-26 08:25:46.000000 django-minio-storage-0.3.7/django_minio_storage.egg-info/PKG-INFO
--rw-rw-r--   0 thomasf   (1000) thomasf   (1000)     1372 2020-02-26 08:25:46.000000 django-minio-storage-0.3.7/django_minio_storage.egg-info/SOURCES.txt
--rw-rw-r--   0 thomasf   (1000) thomasf   (1000)        1 2020-02-26 08:25:46.000000 django-minio-storage-0.3.7/django_minio_storage.egg-info/dependency_links.txt
--rw-rw-r--   0 thomasf   (1000) thomasf   (1000)       53 2020-02-26 08:25:46.000000 django-minio-storage-0.3.7/django_minio_storage.egg-info/requires.txt
--rw-rw-r--   0 thomasf   (1000) thomasf   (1000)       75 2020-02-26 08:25:46.000000 django-minio-storage-0.3.7/django_minio_storage.egg-info/top_level.txt
--rw-r--r--   0 thomasf   (1000) thomasf   (1000)      249 2018-07-12 19:09:03.000000 django-minio-storage-0.3.7/docker-compose.yml
-drwxrwxr-x   0 thomasf   (1000) thomasf   (1000)        0 2020-02-26 08:25:46.000000 django-minio-storage-0.3.7/docs/
--rw-r--r--   0 thomasf   (1000) thomasf   (1000)      229 2018-07-12 19:09:12.000000 django-minio-storage-0.3.7/docs/contributing.md
--rw-r--r--   0 thomasf   (1000) thomasf   (1000)       71 2018-07-12 19:09:12.000000 django-minio-storage-0.3.7/docs/contributors.md
--rw-r--r--   0 thomasf   (1000) thomasf   (1000)      636 2019-10-17 17:15:25.000000 django-minio-storage-0.3.7/docs/development.md
--rw-r--r--   0 thomasf   (1000) thomasf   (1000)      626 2019-10-17 17:18:18.000000 django-minio-storage-0.3.7/docs/index.md
--rw-r--r--   0 thomasf   (1000) thomasf   (1000)    12348 2018-07-12 19:09:12.000000 django-minio-storage-0.3.7/docs/licences.md
--rw-rw-r--   0 thomasf   (1000) thomasf   (1000)     5744 2020-02-22 17:03:43.000000 django-minio-storage-0.3.7/docs/usage.md
-drwxrwxr-x   0 thomasf   (1000) thomasf   (1000)        0 2020-02-26 08:25:46.000000 django-minio-storage-0.3.7/minio_storage/
--rw-rw-r--   0 thomasf   (1000) thomasf   (1000)        0 2019-10-21 23:34:38.000000 django-minio-storage-0.3.7/minio_storage/__init__.py
--rw-rw-r--   0 thomasf   (1000) thomasf   (1000)      102 2019-10-18 04:51:16.000000 django-minio-storage-0.3.7/minio_storage/apps.py
--rw-rw-r--   0 thomasf   (1000) thomasf   (1000)      773 2019-10-28 06:17:19.000000 django-minio-storage-0.3.7/minio_storage/errors.py
--rw-rw-r--   0 thomasf   (1000) thomasf   (1000)     4416 2019-12-16 11:38:04.000000 django-minio-storage-0.3.7/minio_storage/files.py
-drwxrwxr-x   0 thomasf   (1000) thomasf   (1000)        0 2020-02-26 08:25:46.000000 django-minio-storage-0.3.7/minio_storage/management/
--rw-rw-r--   0 thomasf   (1000) thomasf   (1000)        0 2019-10-18 04:51:45.000000 django-minio-storage-0.3.7/minio_storage/management/__init__.py
-drwxrwxr-x   0 thomasf   (1000) thomasf   (1000)        0 2020-02-26 08:25:46.000000 django-minio-storage-0.3.7/minio_storage/management/commands/
--rw-rw-r--   0 thomasf   (1000) thomasf   (1000)        0 2019-10-18 04:51:56.000000 django-minio-storage-0.3.7/minio_storage/management/commands/__init__.py
--rw-rw-r--   0 thomasf   (1000) thomasf   (1000)     8296 2019-10-22 18:18:07.000000 django-minio-storage-0.3.7/minio_storage/management/commands/minio.py
--rw-rw-r--   0 thomasf   (1000) thomasf   (1000)     4048 2019-10-18 08:18:30.000000 django-minio-storage-0.3.7/minio_storage/policy.py
--rw-rw-r--   0 thomasf   (1000) thomasf   (1000)    14343 2020-02-26 08:20:12.000000 django-minio-storage-0.3.7/minio_storage/storage.py
--rw-r--r--   0 thomasf   (1000) thomasf   (1000)      235 2018-07-12 19:09:03.000000 django-minio-storage-0.3.7/mkdocs.yml
--rw-rw-r--   0 thomasf   (1000) thomasf   (1000)       40 2019-10-16 22:34:52.000000 django-minio-storage-0.3.7/pyproject.toml
--rw-rw-r--   0 thomasf   (1000) thomasf   (1000)       38 2020-02-26 08:25:46.000000 django-minio-storage-0.3.7/setup.cfg
--rw-rw-r--   0 thomasf   (1000) thomasf   (1000)      970 2019-10-29 01:23:53.000000 django-minio-storage-0.3.7/setup.py
-drwxrwxr-x   0 thomasf   (1000) thomasf   (1000)        0 2020-02-26 08:25:46.000000 django-minio-storage-0.3.7/tests/
--rw-r--r--   0 thomasf   (1000) thomasf   (1000)        0 2018-07-12 19:09:12.000000 django-minio-storage-0.3.7/tests/__init__.py
-drwxrwxr-x   0 thomasf   (1000) thomasf   (1000)        0 2020-02-26 08:25:46.000000 django-minio-storage-0.3.7/tests/django_minio_storage_tests/
--rw-r--r--   0 thomasf   (1000) thomasf   (1000)        0 2018-07-12 19:09:12.000000 django-minio-storage-0.3.7/tests/django_minio_storage_tests/__init__.py
--rw-rw-r--   0 thomasf   (1000) thomasf   (1000)     4156 2019-10-16 20:47:52.000000 django-minio-storage-0.3.7/tests/django_minio_storage_tests/settings.py
--rw-rw-r--   0 thomasf   (1000) thomasf   (1000)      775 2019-10-16 20:47:52.000000 django-minio-storage-0.3.7/tests/django_minio_storage_tests/urls.py
--rw-rw-r--   0 thomasf   (1000) thomasf   (1000)      429 2019-10-16 20:47:52.000000 django-minio-storage-0.3.7/tests/django_minio_storage_tests/wsgi.py
--rwxrwxr-x   0 thomasf   (1000) thomasf   (1000)      283 2019-10-16 20:47:52.000000 django-minio-storage-0.3.7/tests/manage.py
-drwxrwxr-x   0 thomasf   (1000) thomasf   (1000)        0 2020-02-26 08:25:46.000000 django-minio-storage-0.3.7/tests/test_app/
--rw-r--r--   0 thomasf   (1000) thomasf   (1000)        0 2018-07-12 19:09:12.000000 django-minio-storage-0.3.7/tests/test_app/__init__.py
-drwxrwxr-x   0 thomasf   (1000) thomasf   (1000)        0 2020-02-26 08:25:46.000000 django-minio-storage-0.3.7/tests/test_app/tests/
--rw-r--r--   0 thomasf   (1000) thomasf   (1000)        0 2018-07-12 19:09:12.000000 django-minio-storage-0.3.7/tests/test_app/tests/__init__.py
--rw-rw-r--   0 thomasf   (1000) thomasf   (1000)     6366 2019-12-16 11:38:11.000000 django-minio-storage-0.3.7/tests/test_app/tests/bucket_tests.py
--rw-rw-r--   0 thomasf   (1000) thomasf   (1000)     4500 2019-10-22 18:13:14.000000 django-minio-storage-0.3.7/tests/test_app/tests/custom_storage_class_tests.py
--rw-rw-r--   0 thomasf   (1000) thomasf   (1000)     1656 2019-10-16 21:51:18.000000 django-minio-storage-0.3.7/tests/test_app/tests/delete_tests.py
--rw-rw-r--   0 thomasf   (1000) thomasf   (1000)     5381 2019-10-22 03:11:01.000000 django-minio-storage-0.3.7/tests/test_app/tests/managementcommand_tests.py
--rw-rw-r--   0 thomasf   (1000) thomasf   (1000)     9870 2020-02-22 16:05:51.000000 django-minio-storage-0.3.7/tests/test_app/tests/retrieve_tests.py
--rw-rw-r--   0 thomasf   (1000) thomasf   (1000)     4061 2020-02-22 17:00:21.000000 django-minio-storage-0.3.7/tests/test_app/tests/upload_tests.py
--rw-rw-r--   0 thomasf   (1000) thomasf   (1000)     1939 2019-10-17 19:18:53.000000 django-minio-storage-0.3.7/tests/test_app/tests/utils.py
--rw-r--r--   0 thomasf   (1000) thomasf   (1000)    79300 2018-07-12 19:09:12.000000 django-minio-storage-0.3.7/tests/watermelon-cat.jpg
--rw-rw-r--   0 thomasf   (1000) thomasf   (1000)     1214 2019-10-22 06:44:10.000000 django-minio-storage-0.3.7/tox.ini
+drwxrwxr-x   0 t         (1000) t         (1000)        0 2020-07-09 12:59:38.177765 django-minio-storage-0.3.8/
+-rw-r--r--   0 t         (1000) t         (1000)      197 2019-10-16 20:54:45.000000 django-minio-storage-0.3.8/.editorconfig
+-rw-r--r--   0 t         (1000) t         (1000)       92 2019-10-16 20:50:16.000000 django-minio-storage-0.3.8/.flake8rc
+-rw-rw-r--   0 t         (1000) t         (1000)      100 2019-12-16 11:38:04.000000 django-minio-storage-0.3.8/.gitignore
+-rw-rw-r--   0 t         (1000) t         (1000)      259 2019-10-17 17:09:29.000000 django-minio-storage-0.3.8/.isort.cfg
+-rw-rw-r--   0 t         (1000) t         (1000)     1448 2019-10-18 12:43:28.000000 django-minio-storage-0.3.8/.travis.yml
+-rw-rw-r--   0 t         (1000) t         (1000)     3073 2020-07-09 12:58:41.000000 django-minio-storage-0.3.8/CHANGELOG.md
+-rw-r--r--   0 t         (1000) t         (1000)       43 2018-07-12 19:09:03.000000 django-minio-storage-0.3.8/CONTRIBUTING.md
+-rw-r--r--   0 t         (1000) t         (1000)    11004 2018-07-12 19:09:03.000000 django-minio-storage-0.3.8/LICENSE-APACHE
+-rw-r--r--   0 t         (1000) t         (1000)     1102 2018-07-12 19:09:03.000000 django-minio-storage-0.3.8/LICENSE-MIT
+-rw-rw-r--   0 t         (1000) t         (1000)      653 2020-07-09 12:59:38.173765 django-minio-storage-0.3.8/PKG-INFO
+-rw-r--r--   0 t         (1000) t         (1000)      965 2018-07-12 19:09:03.000000 django-minio-storage-0.3.8/README.md
+-rw-rw-r--   0 t         (1000) t         (1000)      137 2019-10-22 03:11:11.000000 django-minio-storage-0.3.8/dev-requirements.txt
+drwxrwxr-x   0 t         (1000) t         (1000)        0 2020-07-09 12:59:38.157765 django-minio-storage-0.3.8/django_minio_storage.egg-info/
+-rw-rw-r--   0 t         (1000) t         (1000)      653 2020-07-09 12:59:38.000000 django-minio-storage-0.3.8/django_minio_storage.egg-info/PKG-INFO
+-rw-rw-r--   0 t         (1000) t         (1000)     1372 2020-07-09 12:59:38.000000 django-minio-storage-0.3.8/django_minio_storage.egg-info/SOURCES.txt
+-rw-rw-r--   0 t         (1000) t         (1000)        1 2020-07-09 12:59:38.000000 django-minio-storage-0.3.8/django_minio_storage.egg-info/dependency_links.txt
+-rw-rw-r--   0 t         (1000) t         (1000)       53 2020-07-09 12:59:38.000000 django-minio-storage-0.3.8/django_minio_storage.egg-info/requires.txt
+-rw-rw-r--   0 t         (1000) t         (1000)       75 2020-07-09 12:59:38.000000 django-minio-storage-0.3.8/django_minio_storage.egg-info/top_level.txt
+-rw-r--r--   0 t         (1000) t         (1000)      249 2018-07-12 19:09:03.000000 django-minio-storage-0.3.8/docker-compose.yml
+drwxrwxr-x   0 t         (1000) t         (1000)        0 2020-07-09 12:59:38.161765 django-minio-storage-0.3.8/docs/
+-rw-r--r--   0 t         (1000) t         (1000)      229 2018-07-12 19:09:12.000000 django-minio-storage-0.3.8/docs/contributing.md
+-rw-r--r--   0 t         (1000) t         (1000)       71 2018-07-12 19:09:12.000000 django-minio-storage-0.3.8/docs/contributors.md
+-rw-r--r--   0 t         (1000) t         (1000)      636 2019-10-17 17:15:25.000000 django-minio-storage-0.3.8/docs/development.md
+-rw-r--r--   0 t         (1000) t         (1000)      626 2019-10-17 17:18:18.000000 django-minio-storage-0.3.8/docs/index.md
+-rw-r--r--   0 t         (1000) t         (1000)    12348 2018-07-12 19:09:12.000000 django-minio-storage-0.3.8/docs/licences.md
+-rw-rw-r--   0 t         (1000) t         (1000)     5617 2020-07-09 12:57:56.000000 django-minio-storage-0.3.8/docs/usage.md
+drwxrwxr-x   0 t         (1000) t         (1000)        0 2020-07-09 12:59:38.161765 django-minio-storage-0.3.8/minio_storage/
+-rw-rw-r--   0 t         (1000) t         (1000)        0 2019-10-21 23:34:38.000000 django-minio-storage-0.3.8/minio_storage/__init__.py
+-rw-rw-r--   0 t         (1000) t         (1000)      102 2019-10-18 04:51:16.000000 django-minio-storage-0.3.8/minio_storage/apps.py
+-rw-rw-r--   0 t         (1000) t         (1000)      773 2019-10-28 06:17:19.000000 django-minio-storage-0.3.8/minio_storage/errors.py
+-rw-rw-r--   0 t         (1000) t         (1000)     4416 2019-12-16 11:38:04.000000 django-minio-storage-0.3.8/minio_storage/files.py
+drwxrwxr-x   0 t         (1000) t         (1000)        0 2020-07-09 12:59:38.161765 django-minio-storage-0.3.8/minio_storage/management/
+-rw-rw-r--   0 t         (1000) t         (1000)        0 2019-10-18 04:51:45.000000 django-minio-storage-0.3.8/minio_storage/management/__init__.py
+drwxrwxr-x   0 t         (1000) t         (1000)        0 2020-07-09 12:59:38.161765 django-minio-storage-0.3.8/minio_storage/management/commands/
+-rw-rw-r--   0 t         (1000) t         (1000)        0 2019-10-18 04:51:56.000000 django-minio-storage-0.3.8/minio_storage/management/commands/__init__.py
+-rw-rw-r--   0 t         (1000) t         (1000)     8296 2019-10-22 18:18:07.000000 django-minio-storage-0.3.8/minio_storage/management/commands/minio.py
+-rw-rw-r--   0 t         (1000) t         (1000)     4048 2019-10-18 08:18:30.000000 django-minio-storage-0.3.8/minio_storage/policy.py
+-rw-rw-r--   0 t         (1000) t         (1000)    16310 2020-07-09 12:57:56.000000 django-minio-storage-0.3.8/minio_storage/storage.py
+-rw-r--r--   0 t         (1000) t         (1000)      235 2018-07-12 19:09:03.000000 django-minio-storage-0.3.8/mkdocs.yml
+-rw-rw-r--   0 t         (1000) t         (1000)       40 2019-10-16 22:34:52.000000 django-minio-storage-0.3.8/pyproject.toml
+-rw-rw-r--   0 t         (1000) t         (1000)       38 2020-07-09 12:59:38.177765 django-minio-storage-0.3.8/setup.cfg
+-rw-rw-r--   0 t         (1000) t         (1000)      970 2019-10-29 01:23:53.000000 django-minio-storage-0.3.8/setup.py
+drwxrwxr-x   0 t         (1000) t         (1000)        0 2020-07-09 12:59:38.165765 django-minio-storage-0.3.8/tests/
+-rw-r--r--   0 t         (1000) t         (1000)        0 2018-07-12 19:09:12.000000 django-minio-storage-0.3.8/tests/__init__.py
+drwxrwxr-x   0 t         (1000) t         (1000)        0 2020-07-09 12:59:38.169765 django-minio-storage-0.3.8/tests/django_minio_storage_tests/
+-rw-r--r--   0 t         (1000) t         (1000)        0 2018-07-12 19:09:12.000000 django-minio-storage-0.3.8/tests/django_minio_storage_tests/__init__.py
+-rw-rw-r--   0 t         (1000) t         (1000)     4156 2019-10-16 20:47:52.000000 django-minio-storage-0.3.8/tests/django_minio_storage_tests/settings.py
+-rw-rw-r--   0 t         (1000) t         (1000)      775 2019-10-16 20:47:52.000000 django-minio-storage-0.3.8/tests/django_minio_storage_tests/urls.py
+-rw-rw-r--   0 t         (1000) t         (1000)      429 2019-10-16 20:47:52.000000 django-minio-storage-0.3.8/tests/django_minio_storage_tests/wsgi.py
+-rwxrwxr-x   0 t         (1000) t         (1000)      283 2019-10-16 20:47:52.000000 django-minio-storage-0.3.8/tests/manage.py
+drwxrwxr-x   0 t         (1000) t         (1000)        0 2020-07-09 12:59:38.169765 django-minio-storage-0.3.8/tests/test_app/
+-rw-r--r--   0 t         (1000) t         (1000)        0 2018-07-12 19:09:12.000000 django-minio-storage-0.3.8/tests/test_app/__init__.py
+drwxrwxr-x   0 t         (1000) t         (1000)        0 2020-07-09 12:59:38.173765 django-minio-storage-0.3.8/tests/test_app/tests/
+-rw-r--r--   0 t         (1000) t         (1000)        0 2018-07-12 19:09:12.000000 django-minio-storage-0.3.8/tests/test_app/tests/__init__.py
+-rw-rw-r--   0 t         (1000) t         (1000)     6152 2020-07-09 12:57:56.000000 django-minio-storage-0.3.8/tests/test_app/tests/bucket_tests.py
+-rw-rw-r--   0 t         (1000) t         (1000)     4500 2019-10-22 18:13:14.000000 django-minio-storage-0.3.8/tests/test_app/tests/custom_storage_class_tests.py
+-rw-rw-r--   0 t         (1000) t         (1000)     1656 2019-10-16 21:51:18.000000 django-minio-storage-0.3.8/tests/test_app/tests/delete_tests.py
+-rw-rw-r--   0 t         (1000) t         (1000)     5381 2019-10-22 03:11:01.000000 django-minio-storage-0.3.8/tests/test_app/tests/managementcommand_tests.py
+-rw-rw-r--   0 t         (1000) t         (1000)    10148 2020-07-09 12:57:56.000000 django-minio-storage-0.3.8/tests/test_app/tests/retrieve_tests.py
+-rw-rw-r--   0 t         (1000) t         (1000)     4061 2020-02-22 17:00:21.000000 django-minio-storage-0.3.8/tests/test_app/tests/upload_tests.py
+-rw-rw-r--   0 t         (1000) t         (1000)     1939 2019-10-17 19:18:53.000000 django-minio-storage-0.3.8/tests/test_app/tests/utils.py
+-rw-r--r--   0 t         (1000) t         (1000)    79300 2018-07-12 19:09:12.000000 django-minio-storage-0.3.8/tests/watermelon-cat.jpg
+-rw-rw-r--   0 t         (1000) t         (1000)     1220 2020-07-09 12:57:51.000000 django-minio-storage-0.3.8/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-minio-storage-0.3.7/.travis.yml` & `django-minio-storage-0.3.8/.travis.yml`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.3.7/CHANGELOG.md` & `django-minio-storage-0.3.8/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 0.3.8
+
+Improved presigned urls with non standard base urls
+
 ## 0.3.7
 
 Removed accidentally left over debug print from previous release
 
 ## 0.3.6
 
 ### support adding default meta data
```

### Comparing `django-minio-storage-0.3.7/LICENSE-APACHE` & `django-minio-storage-0.3.8/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.3.7/LICENSE-MIT` & `django-minio-storage-0.3.8/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.3.7/PKG-INFO` & `django-minio-storage-0.3.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-minio-storage
-Version: 0.3.7
+Version: 0.3.8
 Summary: Django file storage using the minio python client
 Home-page: https://github.com/py-pa/django-minio-storage
 Author: Tom Houlé
 Author-email: tom@kafunsho.be
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `django-minio-storage-0.3.7/README.md` & `django-minio-storage-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.3.7/django_minio_storage.egg-info/PKG-INFO` & `django-minio-storage-0.3.8/django_minio_storage.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-minio-storage
-Version: 0.3.7
+Version: 0.3.8
 Summary: Django file storage using the minio python client
 Home-page: https://github.com/py-pa/django-minio-storage
 Author: Tom Houlé
 Author-email: tom@kafunsho.be
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `django-minio-storage-0.3.7/django_minio_storage.egg-info/SOURCES.txt` & `django-minio-storage-0.3.8/django_minio_storage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.3.7/docs/development.md` & `django-minio-storage-0.3.8/docs/development.md`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.3.7/docs/index.md` & `django-minio-storage-0.3.8/docs/index.md`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.3.7/docs/licences.md` & `django-minio-storage-0.3.8/docs/licences.md`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.3.7/docs/usage.md` & `django-minio-storage-0.3.8/docs/usage.md`

 * *Files 6% similar despite different names*

```diff
@@ -64,27 +64,25 @@
   string keys and values, example: `{"Cache-Control": "max-age=1000"}`.
   (default: `None`)
 
 - `MINIO_STORAGE_MEDIA_URL`: the base URL for generating urls to objects from
   `MinioMediaStorage`. When not specified or set to `None` it's value will be
   combined from `MINIO_STORAGE_ENDPOINT` and `MINIO_STORAGE_MEDIA_BUCKET_NAME`.
   `MINIO_STORAGE_MEDIA_URL` should contain the full base url including the
-  bucket name without a trailing slash. Please not that when using presigned
-  URLs, the URL itself is a part of the calculated signature so be careful with
-  how `MINIO_STORAGE_MEDIA_URL` is used, normally it should not have to be set
-  at all.
+  bucket name without a trailing slash. Normally, this should not have to be
+  set, but may be useful when the storage and end user must access the server
+  from different endpoints.
 
 - `MINIO_STORAGE_STATIC_URL`: the base URL for generating URLs to objects from
   `MinioStaticStorage`. When not specified or set to `None` it's value will be
   combined from `MINIO_STORAGE_ENDPOINT` and
   `MINIO_STORAGE_STATIC_BUCKET_NAME`. `MINIO_STORAGE_STATIC_URL` should contain
-  the full base url including the bucket name without a trailing slash. Please
-  not that when using presigned URLs, the URL itself is a part of the
-  calculated signature so be careful with how `MINIO_STORAGE_STATIC_URL` is
-  used, normally it should not have to be set at all.
+  the full base url including the bucket name without a trailing slash.
+  Normally, this should not have to be set, but may be useful when the storage
+  and end user must access the server from different endpoints.
 
 - `MINIO_STORAGE_MEDIA_BACKUP_BUCKET`: Bucket to be used to store deleted files.
   The bucket **has to exists**, the storage will not try to create it.
   Required if `MINIO_STORAGE_MEDIA_BACKUP_FORMAT` is set.
 
 - `MINIO_STORAGE_MEDIA_BACKUP_FORMAT`: Path to be used to store deleted files,
   the path can contain Python's `strftime` substitutes, such as `%H`, `%c` and
```

### Comparing `django-minio-storage-0.3.7/minio_storage/errors.py` & `django-minio-storage-0.3.8/minio_storage/errors.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.3.7/minio_storage/files.py` & `django-minio-storage-0.3.8/minio_storage/files.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.3.7/minio_storage/management/commands/minio.py` & `django-minio-storage-0.3.8/minio_storage/management/commands/minio.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.3.7/minio_storage/policy.py` & `django-minio-storage-0.3.8/minio_storage/policy.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.3.7/minio_storage/storage.py` & `django-minio-storage-0.3.8/minio_storage/storage.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import datetime
 import mimetypes
 import posixpath
 import typing as T
 import urllib
 from logging import getLogger
 from time import mktime
-from urllib.parse import urlparse
+from urllib.parse import urlsplit, urlunsplit
 
 import minio
 import minio.error as merr
 from django.conf import settings
 from django.core.exceptions import ImproperlyConfigured
 from django.core.files.storage import Storage
 from django.utils import timezone
@@ -70,14 +70,22 @@
         self.assume_bucket_exists = assume_bucket_exists
         self.policy_type = policy_type
         self.presign_urls = presign_urls
         self.object_metadata = object_metadata
 
         self._init_check()
 
+        # A base_url_client is only necessary when using presign_urls
+        if self.presign_urls and self.base_url:
+            # Do this after _init_check, so client's bucket region cache will
+            # already be populated
+            self.base_url_client = self._create_base_url_client(
+                self.client, self.bucket_name, self.base_url
+            )
+
         super().__init__()
 
     def _init_check(self):
         if not self.assume_bucket_exists:
             if self.auto_create_bucket and not self.client.bucket_exists(
                 self.bucket_name
             ):
@@ -89,14 +97,40 @@
                     self.client.set_bucket_policy(
                         self.bucket_name, policy_type.bucket(self.bucket_name)
                     )
 
             elif not self.client.bucket_exists(self.bucket_name):
                 raise OSError(f"The bucket {self.bucket_name} does not exist")
 
+    @staticmethod
+    def _create_base_url_client(client: minio.Minio, bucket_name: str, base_url: str):
+        """
+        Clone a Minio client, using a different endpoint from `base_url`.
+        """
+        base_url_parts = urlsplit(base_url)
+
+        # Clone from the normal client, but with base_url as the endpoint
+        base_url_client = minio.Minio(
+            base_url_parts.netloc,
+            access_key=client._access_key,
+            secret_key=client._secret_key,
+            session_token=client._session_token,
+            secure=base_url_parts.scheme == 'https',
+            # The bucket region may be auto-detected by client (via an HTTP
+            # request), so don't just use client._region
+            region=client._get_bucket_region(bucket_name),
+            http_client=client._http
+        )
+        if hasattr(client, '_credentials'):
+            # Client credentials do not exist prior to minio-py 5.0.7, but
+            # they should be reused if possible
+            base_url_client._credentials = client._credentials
+
+        return base_url_client
+
     def _sanitize_path(self, name):
         v = posixpath.normpath(name).replace("\\", "/")
         if v == ".":
             v = ""
         if name.endswith("/") and not v.endswith("/"):
             v += "/"
         return v
@@ -117,16 +151,15 @@
     def _open(self, name, mode="rb"):
         try:
             f = self.file_class(self._sanitize_path(name), mode, self)
         except merr.MinioError as e:
             raise minio_error("File {} could not be saved: {}".format(name, str(e)), e)
         return f
 
-    def _save(self, name, content):
-        # (str, bytes) -> str
+    def _save(self, name: str, content: bytes) -> str:
         try:
             if hasattr(content, "seek") and callable(content.seek):
                 content.seek(0)
             content_size, content_type, sane_name = self._examine_file(name, content)
             self.client.put_object(
                 self.bucket_name,
                 sane_name,
@@ -225,39 +258,55 @@
     def size(self, name: str) -> int:
         try:
             info = self.client.stat_object(self.bucket_name, name)
             return info.size
         except merr.ResponseError as error:
             raise minio_error(f"Could not access file size for {name}", error)
 
-    def url(
-        self, name: str, *args, max_age: T.Optional[datetime.timedelta] = None
+    def _presigned_url(
+        self, name: str, max_age: T.Optional[datetime.timedelta] = None
     ) -> str:
         kwargs = {}
         if max_age is not None:
             kwargs["expires"] = max_age
 
-        # NOTE: Here be dragons, when a external base_url is used the code
-        # below is both using "internal" minio clint APIs and somewhat
-        # subverting how minio/S3 expects urls to be generated in the first
-        # place.
+        client = (
+            self.client
+            if self.base_url is None else
+            self.base_url_client
+        )
+        url = client.presigned_get_object(self.bucket_name, name, **kwargs)
+
+        if self.base_url is not None:
+            url_parts = urlsplit(url)
+            base_url_parts = urlsplit(self.base_url)
+
+            # It's assumed that self.base_url will contain bucket information,
+            # which could be different, so remove the bucket_name component (with 1
+            # extra character for the leading "/") from the generated URL
+            url_key_path = url_parts.path[len(self.bucket_name) + 1:]
+
+            # Prefix the URL with any path content from base_url
+            new_url_path = base_url_parts.path + url_key_path
+
+            # Reconstruct the URL with an updated path
+            url = urlunsplit((
+                url_parts.scheme,
+                url_parts.netloc,
+                new_url_path,
+                url_parts.query,
+                url_parts.fragment
+            ))
+        return url
 
+    def url(
+        self, name: str, *args, max_age: T.Optional[datetime.timedelta] = None
+    ) -> str:
         if self.presign_urls:
-            url = self.client.presigned_get_object(self.bucket_name, name, **kwargs)
-            if self.base_url is not None:
-                parsed_url = urlparse(url)
-                path = parsed_url.path.split(self.bucket_name, 1)[1]
-                url = "{}{}?{}{}{}".format(
-                    self.base_url,
-                    path,
-                    parsed_url.params,
-                    parsed_url.query,
-                    parsed_url.fragment,
-                )
-
+            url = self._presigned_url(name, max_age=max_age)
         else:
             if self.base_url is not None:
 
                 def strip_beg(path):
                     while path.startswith("/"):
                         path = path[1:]
                     return path
```

### Comparing `django-minio-storage-0.3.7/setup.py` & `django-minio-storage-0.3.8/setup.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.3.7/tests/django_minio_storage_tests/settings.py` & `django-minio-storage-0.3.8/tests/django_minio_storage_tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.3.7/tests/django_minio_storage_tests/urls.py` & `django-minio-storage-0.3.8/tests/django_minio_storage_tests/urls.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.3.7/tests/test_app/tests/bucket_tests.py` & `django-minio-storage-0.3.8/tests/test_app/tests/bucket_tests.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,33 +35,23 @@
 
     @override_settings(
         MINIO_STORAGE_MEDIA_BUCKET_NAME="inexistent",
         MINIO_STORAGE_AUTO_CREATE_MEDIA_BUCKET=False,
         MINIO_STORAGE_ASSUME_MEDIA_BUCKET_EXISTS=True,
     )
     def test_media_storage_ignore_bucket_check(self):
-        try:
-            MinioMediaStorage()
-        except OSError:
-            self.assertTrue(False)
-        else:
-            pass
+        MinioMediaStorage()
 
     @override_settings(
         MINIO_STORAGE_STATIC_BUCKET_NAME="inexistent",
         MINIO_STORAGE_AUTO_CREATE_STATIC_BUCKET=False,
         MINIO_STORAGE_ASSUME_STATIC_BUCKET_EXISTS=True,
     )
     def test_static_storage_ignore_bucket_check(self):
-        try:
-            MinioStaticStorage()
-        except OSError:
-            self.assertTrue(False)
-        else:
-            pass
+        MinioStaticStorage()
 
 
 class BucketPolicyTests(BaseTestMixin, TestCase):
     def setUp(self):
         pass
 
     def tearDown(self):
```

### Comparing `django-minio-storage-0.3.7/tests/test_app/tests/custom_storage_class_tests.py` & `django-minio-storage-0.3.8/tests/test_app/tests/custom_storage_class_tests.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.3.7/tests/test_app/tests/delete_tests.py` & `django-minio-storage-0.3.8/tests/test_app/tests/delete_tests.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.3.7/tests/test_app/tests/managementcommand_tests.py` & `django-minio-storage-0.3.8/tests/test_app/tests/managementcommand_tests.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.3.7/tests/test_app/tests/retrieve_tests.py` & `django-minio-storage-0.3.8/tests/test_app/tests/retrieve_tests.py`

 * *Files 3% similar despite different names*

```diff
@@ -180,14 +180,26 @@
         assert endpoint != ""
         media_storage = MinioMediaStorage()
         name = "23/23/aaa/bbb/22"
         url = media_storage.url(name)
         self.assertEqual(url, f"http://{endpoint}/foo/23/23/aaa/bbb/22")
 
     @override_settings(
+        MINIO_STORAGE_MEDIA_USE_PRESIGNED=True,
+        MINIO_STORAGE_MEDIA_URL=None,
+        MINIO_STORAGE_MEDIA_BUCKET_NAME="foo",
+    )
+    def test_presigned_no_base_url(self):
+        endpoint = os.getenv("MINIO_STORAGE_ENDPOINT", "minio:9000")
+        assert endpoint != ""
+        media_storage = MinioMediaStorage()
+        url = media_storage.url("22")
+        self.assertRegex(url, rf"^http://{endpoint}/foo/22\?")
+
+    @override_settings(
         MINIO_STORAGE_MEDIA_USE_PRESIGNED=False,
         MINIO_STORAGE_MEDIA_URL="https://example23.com/foo",
         MINIO_STORAGE_MEDIA_BUCKET_NAME="bar",
     )
     def test_base_url(self):
         media_storage = MinioMediaStorage()
         url = media_storage.url("1")
@@ -205,35 +217,31 @@
 
     @override_settings(
         MINIO_STORAGE_MEDIA_URL="http://example11.com/foo",
         MINIO_STORAGE_MEDIA_USE_PRESIGNED=True,
         MINIO_STORAGE_MEDIA_BUCKET_NAME="bar",
     )
     def test_presigned_base_url(self):
-        # The url generated here probably doenst work in a real situation
         media_storage = MinioMediaStorage()
         url = media_storage.url("1")
         self.assertIn("X-Amz-Signature", url)
-        self.assertIn("http://example11.com/foo", url)
+        self.assertRegex(url, r"^http://example11.com/foo/1\?")
 
     @override_settings(
         MINIO_STORAGE_MEDIA_URL="http://example11.com/foo",
         MINIO_STORAGE_MEDIA_USE_PRESIGNED=True,
         MINIO_STORAGE_MEDIA_BUCKET_NAME="bar",
     )
     def test_presigned_base_url_subpath(self):
-        # The url generated here probably doenst work in a real situation
         media_storage = MinioMediaStorage()
-        name = "1/555/666/777"
-        url = media_storage.url(name)
+        url = media_storage.url("1/555/666/777")
         self.assertIn("X-Amz-Signature", url)
-        self.assertIn("http://example11.com/foo", url)
-        self.assertIn(name, url)
+        self.assertRegex(url, r"^http://example11.com/foo/1/555/666/777\?")
 
-    BASE = "http://ba se/url"
+    BASE = "http://base/url"
     NAME = "Bö/ &öl@:/E"
     ENCODED = "B%C3%B6/%20%26%C3%B6l%40%3A/E"
 
     @override_settings(
         MINIO_STORAGE_MEDIA_URL=None,
         MINIO_STORAGE_MEDIA_USE_PRESIGNED=False,
         MINIO_STORAGE_MEDIA_BUCKET_NAME="encoding",
```

### Comparing `django-minio-storage-0.3.7/tests/test_app/tests/upload_tests.py` & `django-minio-storage-0.3.8/tests/test_app/tests/upload_tests.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.3.7/tests/test_app/tests/utils.py` & `django-minio-storage-0.3.8/tests/test_app/tests/utils.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.3.7/tests/watermelon-cat.jpg` & `django-minio-storage-0.3.8/tests/watermelon-cat.jpg`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.3.7/tox.ini` & `django-minio-storage-0.3.8/tox.ini`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 DJANGO =
         1.11: django111
         2.1: django21
         2.2: django22, lint, docs
         3.0: django30
 
 [testenv]
-commands = pytest
+commands = pytest {posargs}
 setenv =
         PYTHONDONTWRITEBYTECODE=1
         MINIO_STORAGE_ENDPOINT=localhost:9153
         MINIO_STORAGE_ACCESS_KEY=weak_access_key
         MINIO_STORAGE_SECRET_KEY=weak_secret_key
         TOX_ENVNAME={envname}
 deps =
@@ -34,20 +34,20 @@
         minio: minio
         minioknown: minio==4.0.21
         -rdev-requirements.txt
 
 [testenv:lint]
 setenv=
     PYTHONWARNINGS=ignore
-basepython = python3.7
+basepython = python3
 deps = flake8==3.7.8
 commands = flake8 --config .flake8rc
 
 [testenv:docs]
-basepython = python3.7
+basepython = python3
 deps = mkdocs
 commands = mkdocs build
 
 [tox]
 envlist =
        {py36,py37,py38}-django22-minioknown
        py37-django{111,21,30}-minioknown
```

