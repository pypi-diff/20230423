# Comparing `tmp/jawanndenn-2.5.0.tar.gz` & `tmp/jawanndenn-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jawanndenn-2.5.0.tar", last modified: Tue Jul 20 15:57:47 2021, max compression
+gzip compressed data, was "jawanndenn-2.6.0.tar", last modified: Sun Apr 23 01:55:42 2023, max compression
```

## Comparing `jawanndenn-2.5.0.tar` & `jawanndenn-2.6.0.tar`

### file list

```diff
@@ -1,161 +1,165 @@
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-07-20 15:57:47.729542 jawanndenn-2.5.0/
--rw-r--r--   0 sping     (1000) sping     (1000)     1587 2020-08-16 00:42:21.000000 jawanndenn-2.5.0/.dockerignore
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-07-20 15:57:47.695542 jawanndenn-2.5.0/.github/
--rw-r--r--   0 sping     (1000) sping     (1000)      436 2020-08-05 17:04:17.000000 jawanndenn-2.5.0/.github/dependabot.yml
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-07-20 15:57:47.696542 jawanndenn-2.5.0/.github/workflows/
--rw-r--r--   0 sping     (1000) sping     (1000)     1138 2021-04-27 17:33:20.000000 jawanndenn-2.5.0/.github/workflows/build_and_test_using_docker.yml
--rw-r--r--   0 sping     (1000) sping     (1000)      403 2020-01-26 15:52:37.000000 jawanndenn-2.5.0/.github/workflows/dockerignore_detect_out_of_sync.yml
--rw-r--r--   0 sping     (1000) sping     (1000)      797 2021-04-27 17:33:20.000000 jawanndenn-2.5.0/.github/workflows/pre_commit_detect_outdated.yml
--rw-r--r--   0 sping     (1000) sping     (1000)      779 2021-04-27 17:33:20.000000 jawanndenn-2.5.0/.github/workflows/run_pre_commit.yml
--rw-r--r--   0 sping     (1000) sping     (1000)       40 2016-11-01 21:45:41.000000 jawanndenn-2.5.0/.gitignore
--rw-r--r--   0 sping     (1000) sping     (1000)      745 2021-07-16 22:24:39.000000 jawanndenn-2.5.0/.pre-commit-config.yaml
--rw-r--r--   0 sping     (1000) sping     (1000)     1578 2020-08-16 00:42:21.000000 jawanndenn-2.5.0/Dockerfile
--rw-r--r--   0 sping     (1000) sping     (1000)    10898 2021-07-20 15:57:47.729542 jawanndenn-2.5.0/PKG-INFO
--rw-r--r--   0 sping     (1000) sping     (1000)     9856 2021-07-20 15:51:59.000000 jawanndenn-2.5.0/README.rst
--rw-r--r--   0 sping     (1000) sping     (1000)      139 2021-02-14 22:53:06.000000 jawanndenn-2.5.0/crontab
--rw-r--r--   0 sping     (1000) sping     (1000)     3206 2020-10-22 16:08:11.000000 jawanndenn-2.5.0/docker-compose.yml
--rwxr-xr-x   0 sping     (1000) sping     (1000)      985 2020-08-11 21:08:17.000000 jawanndenn-2.5.0/docker-entrypoint.sh
--rwxr-xr-x   0 sping     (1000) sping     (1000)      708 2020-01-26 15:52:37.000000 jawanndenn-2.5.0/generate_whitelist_dockerignore_file.sh
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-07-20 15:57:47.698542 jawanndenn-2.5.0/jawanndenn/
--rw-r--r--   0 sping     (1000) sping     (1000)       57 2019-12-02 19:28:12.000000 jawanndenn-2.5.0/jawanndenn/__init__.py
--rw-r--r--   0 sping     (1000) sping     (1000)     6374 2020-04-17 18:23:54.000000 jawanndenn-2.5.0/jawanndenn/__main__.py
--rw-r--r--   0 sping     (1000) sping     (1000)      397 2019-12-19 22:38:26.000000 jawanndenn-2.5.0/jawanndenn/asgi.py
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-07-20 15:57:47.699542 jawanndenn-2.5.0/jawanndenn/management/
--rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-08-16 00:42:21.000000 jawanndenn-2.5.0/jawanndenn/management/__init__.py
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-07-20 15:57:47.699542 jawanndenn-2.5.0/jawanndenn/management/commands/
--rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-08-16 00:42:21.000000 jawanndenn-2.5.0/jawanndenn/management/commands/__init__.py
--rw-r--r--   0 sping     (1000) sping     (1000)      452 2020-08-16 00:42:21.000000 jawanndenn-2.5.0/jawanndenn/management/commands/prune_expired_polls.py
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-07-20 15:57:47.699542 jawanndenn-2.5.0/jawanndenn/management/commands/tests/
--rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-08-16 00:42:21.000000 jawanndenn-2.5.0/jawanndenn/management/commands/tests/__init__.py
--rw-r--r--   0 sping     (1000) sping     (1000)     1024 2020-08-16 00:42:21.000000 jawanndenn-2.5.0/jawanndenn/management/commands/tests/test_prune_expired_polls.py
--rw-r--r--   0 sping     (1000) sping     (1000)     1410 2019-12-02 19:28:12.000000 jawanndenn-2.5.0/jawanndenn/markup.py
--rw-r--r--   0 sping     (1000) sping     (1000)      202 2021-07-20 15:56:55.000000 jawanndenn-2.5.0/jawanndenn/metadata.py
--rw-r--r--   0 sping     (1000) sping     (1000)     1277 2020-08-07 18:17:21.000000 jawanndenn-2.5.0/jawanndenn/middleware.py
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-07-20 15:57:47.700542 jawanndenn-2.5.0/jawanndenn/migrations/
--rw-r--r--   0 sping     (1000) sping     (1000)     3233 2020-07-26 23:40:32.000000 jawanndenn-2.5.0/jawanndenn/migrations/0001_initial.py
--rw-r--r--   0 sping     (1000) sping     (1000)      467 2020-08-15 23:54:51.000000 jawanndenn-2.5.0/jawanndenn/migrations/0002_django_extensions_3_0_0.py
--rw-r--r--   0 sping     (1000) sping     (1000)      392 2020-08-16 00:42:21.000000 jawanndenn-2.5.0/jawanndenn/migrations/0003_poll_expires_at.py
--rw-r--r--   0 sping     (1000) sping     (1000)        0 2019-12-02 19:28:12.000000 jawanndenn-2.5.0/jawanndenn/migrations/__init__.py
--rw-r--r--   0 sping     (1000) sping     (1000)     1742 2020-08-16 00:42:21.000000 jawanndenn-2.5.0/jawanndenn/models.py
--rw-r--r--   0 sping     (1000) sping     (1000)     1918 2020-08-17 11:21:30.000000 jawanndenn-2.5.0/jawanndenn/serializers.py
--rw-r--r--   0 sping     (1000) sping     (1000)     6205 2021-02-16 01:51:24.000000 jawanndenn-2.5.0/jawanndenn/settings.py
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-07-20 15:57:47.691542 jawanndenn-2.5.0/jawanndenn/static/
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-07-20 15:57:47.688542 jawanndenn-2.5.0/jawanndenn/static/3rdparty/
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-07-20 15:57:47.700542 jawanndenn-2.5.0/jawanndenn/static/3rdparty/github-buttons-4.0.1/
--rw-r--r--   0 sping     (1000) sping     (1000)      545 2020-05-20 19:48:30.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/github-buttons-4.0.1/LICENSE.md
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-07-20 15:57:47.700542 jawanndenn-2.5.0/jawanndenn/static/3rdparty/github-buttons-4.0.1/docs/
--rw-r--r--   0 sping     (1000) sping     (1000)     5419 2020-05-20 19:48:30.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/github-buttons-4.0.1/docs/github-btn.html
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-07-20 15:57:47.701542 jawanndenn-2.5.0/jawanndenn/static/3rdparty/jquery-3.5.1/
--rw-r--r--   0 sping     (1000) sping     (1000)     1095 2020-05-10 22:05:44.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/jquery-3.5.1/LICENSE.txt
--rw-r--r--   0 sping     (1000) sping     (1000)    89476 2020-05-04 23:02:39.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/jquery-3.5.1/jquery-3.5.1.min.js
--rw-r--r--   0 sping     (1000) sping     (1000)   137986 2020-05-04 23:02:39.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/jquery-3.5.1/jquery-3.5.1.min.map
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-07-20 15:57:47.701542 jawanndenn-2.5.0/jawanndenn/static/3rdparty/materialize-1.0.0/
--rw-r--r--   0 sping     (1000) sping     (1000)     1083 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/materialize-1.0.0/LICENSE
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-07-20 15:57:47.702542 jawanndenn-2.5.0/jawanndenn/static/3rdparty/materialize-1.0.0/css/
--rw-r--r--   0 sping     (1000) sping     (1000)   179245 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/materialize-1.0.0/css/materialize.css
--rw-r--r--   0 sping     (1000) sping     (1000)   141841 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/materialize-1.0.0/css/materialize.min.css
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-07-20 15:57:47.703542 jawanndenn-2.5.0/jawanndenn/static/3rdparty/materialize-1.0.0/js/
--rw-r--r--   0 sping     (1000) sping     (1000)   371026 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/materialize-1.0.0/js/materialize.js
--rw-r--r--   0 sping     (1000) sping     (1000)   181114 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/materialize-1.0.0/js/materialize.min.js
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-07-20 15:57:47.704542 jawanndenn-2.5.0/jawanndenn/static/3rdparty/noty-2.4.1/
--rw-r--r--   0 sping     (1000) sping     (1000)     1057 2019-11-30 21:03:50.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/noty-2.4.1/LICENSE.txt
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-07-20 15:57:47.686542 jawanndenn-2.5.0/jawanndenn/static/3rdparty/noty-2.4.1/js/
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-07-20 15:57:47.686542 jawanndenn-2.5.0/jawanndenn/static/3rdparty/noty-2.4.1/js/noty/
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-07-20 15:57:47.705542 jawanndenn-2.5.0/jawanndenn/static/3rdparty/noty-2.4.1/js/noty/packaged/
--rw-r--r--   0 sping     (1000) sping     (1000)    32688 2019-11-30 21:03:50.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/noty-2.4.1/js/noty/packaged/jquery.noty.packaged.min.js
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-07-20 15:57:47.706542 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/
--rw-r--r--   0 sping     (1000) sping     (1000)    11358 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/COPYING
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-07-20 15:57:47.706542 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/css/
--rw-r--r--   0 sping     (1000) sping     (1000)    13602 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/css/roboto.css
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-07-20 15:57:47.727542 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/
--rw-r--r--   0 sping     (1000) sping     (1000)    58088 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-100.eot
--rw-r--r--   0 sping     (1000) sping     (1000)    49675 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-100.svg
--rw-r--r--   0 sping     (1000) sping     (1000)   132100 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-100.ttf
--rw-r--r--   0 sping     (1000) sping     (1000)    64700 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-100.woff
--rw-r--r--   0 sping     (1000) sping     (1000)    49988 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-100.woff2
--rw-r--r--   0 sping     (1000) sping     (1000)    62556 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-100italic.eot
--rw-r--r--   0 sping     (1000) sping     (1000)    56194 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-100italic.svg
--rw-r--r--   0 sping     (1000) sping     (1000)   135068 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-100italic.ttf
--rw-r--r--   0 sping     (1000) sping     (1000)    69568 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-100italic.woff
--rw-r--r--   0 sping     (1000) sping     (1000)    53900 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-100italic.woff2
--rw-r--r--   0 sping     (1000) sping     (1000)    59393 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-300.eot
--rw-r--r--   0 sping     (1000) sping     (1000)    49248 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-300.svg
--rw-r--r--   0 sping     (1000) sping     (1000)   130640 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-300.ttf
--rw-r--r--   0 sping     (1000) sping     (1000)    65784 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-300.woff
--rw-r--r--   0 sping     (1000) sping     (1000)    50812 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-300.woff2
--rw-r--r--   0 sping     (1000) sping     (1000)    64726 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-300italic.eot
--rw-r--r--   0 sping     (1000) sping     (1000)    54885 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-300italic.svg
--rw-r--r--   0 sping     (1000) sping     (1000)   134996 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-300italic.ttf
--rw-r--r--   0 sping     (1000) sping     (1000)    71248 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-300italic.woff
--rw-r--r--   0 sping     (1000) sping     (1000)    55724 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-300italic.woff2
--rw-r--r--   0 sping     (1000) sping     (1000)    60298 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-500.eot
--rw-r--r--   0 sping     (1000) sping     (1000)    48624 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-500.svg
--rw-r--r--   0 sping     (1000) sping     (1000)   132100 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-500.ttf
--rw-r--r--   0 sping     (1000) sping     (1000)    66456 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-500.woff
--rw-r--r--   0 sping     (1000) sping     (1000)    51400 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-500.woff2
--rw-r--r--   0 sping     (1000) sping     (1000)    65334 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-500italic.eot
--rw-r--r--   0 sping     (1000) sping     (1000)    53825 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-500italic.svg
--rw-r--r--   0 sping     (1000) sping     (1000)   135908 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-500italic.ttf
--rw-r--r--   0 sping     (1000) sping     (1000)    71640 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-500italic.woff
--rw-r--r--   0 sping     (1000) sping     (1000)    55912 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-500italic.woff2
--rw-r--r--   0 sping     (1000) sping     (1000)    59829 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-700.eot
--rw-r--r--   0 sping     (1000) sping     (1000)    48982 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-700.svg
--rw-r--r--   0 sping     (1000) sping     (1000)   131008 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-700.ttf
--rw-r--r--   0 sping     (1000) sping     (1000)    66260 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-700.woff
--rw-r--r--   0 sping     (1000) sping     (1000)    51088 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-700.woff2
--rw-r--r--   0 sping     (1000) sping     (1000)    64455 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-700italic.eot
--rw-r--r--   0 sping     (1000) sping     (1000)    53453 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-700italic.svg
--rw-r--r--   0 sping     (1000) sping     (1000)   134500 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-700italic.ttf
--rw-r--r--   0 sping     (1000) sping     (1000)    70756 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-700italic.woff
--rw-r--r--   0 sping     (1000) sping     (1000)    55192 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-700italic.woff2
--rw-r--r--   0 sping     (1000) sping     (1000)    59887 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-900.eot
--rw-r--r--   0 sping     (1000) sping     (1000)    48022 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-900.svg
--rw-r--r--   0 sping     (1000) sping     (1000)   131608 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-900.ttf
--rw-r--r--   0 sping     (1000) sping     (1000)    66412 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-900.woff
--rw-r--r--   0 sping     (1000) sping     (1000)    51212 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-900.woff2
--rw-r--r--   0 sping     (1000) sping     (1000)    65948 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-900italic.eot
--rw-r--r--   0 sping     (1000) sping     (1000)    53240 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-900italic.svg
--rw-r--r--   0 sping     (1000) sping     (1000)   136420 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-900italic.ttf
--rw-r--r--   0 sping     (1000) sping     (1000)    72360 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-900italic.woff
--rw-r--r--   0 sping     (1000) sping     (1000)    56556 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-900italic.woff2
--rw-r--r--   0 sping     (1000) sping     (1000)    64104 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-italic.eot
--rw-r--r--   0 sping     (1000) sping     (1000)    54053 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-italic.svg
--rw-r--r--   0 sping     (1000) sping     (1000)   133248 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-italic.ttf
--rw-r--r--   0 sping     (1000) sping     (1000)    70252 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-italic.woff
--rw-r--r--   0 sping     (1000) sping     (1000)    54984 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-italic.woff2
--rw-r--r--   0 sping     (1000) sping     (1000)    59644 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-regular.eot
--rw-r--r--   0 sping     (1000) sping     (1000)    48974 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-regular.svg
--rw-r--r--   0 sping     (1000) sping     (1000)   131916 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-regular.ttf
--rw-r--r--   0 sping     (1000) sping     (1000)    66044 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-regular.woff
--rw-r--r--   0 sping     (1000) sping     (1000)    51116 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-regular.woff2
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-07-20 15:57:47.727542 jawanndenn-2.5.0/jawanndenn/static/css/
--rw-r--r--   0 sping     (1000) sping     (1000)     4318 2020-05-11 15:36:18.000000 jawanndenn-2.5.0/jawanndenn/static/css/style.css
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-07-20 15:57:47.727542 jawanndenn-2.5.0/jawanndenn/static/html/
--rw-r--r--   0 sping     (1000) sping     (1000)      869 2020-05-20 19:49:42.000000 jawanndenn-2.5.0/jawanndenn/static/html/footer.htm
--rw-r--r--   0 sping     (1000) sping     (1000)     2400 2020-05-20 19:44:46.000000 jawanndenn-2.5.0/jawanndenn/static/html/poll.htm
--rw-r--r--   0 sping     (1000) sping     (1000)     2475 2020-05-20 19:44:43.000000 jawanndenn-2.5.0/jawanndenn/static/html/setup.htm
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-07-20 15:57:47.728542 jawanndenn-2.5.0/jawanndenn/static/js/
--rw-r--r--   0 sping     (1000) sping     (1000)     1054 2019-12-23 19:38:24.000000 jawanndenn-2.5.0/jawanndenn/static/js/html.js
--rw-r--r--   0 sping     (1000) sping     (1000)     6625 2020-05-20 19:34:30.000000 jawanndenn-2.5.0/jawanndenn/static/js/poll.js
--rw-r--r--   0 sping     (1000) sping     (1000)     4369 2020-08-16 00:42:21.000000 jawanndenn-2.5.0/jawanndenn/static/js/setup.js
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-07-20 15:57:47.728542 jawanndenn-2.5.0/jawanndenn/tests/
--rw-r--r--   0 sping     (1000) sping     (1000)        0 2019-12-01 21:56:57.000000 jawanndenn-2.5.0/jawanndenn/tests/__init__.py
--rw-r--r--   0 sping     (1000) sping     (1000)      870 2020-08-13 10:07:19.000000 jawanndenn-2.5.0/jawanndenn/tests/factories.py
--rw-r--r--   0 sping     (1000) sping     (1000)     1726 2019-12-01 21:56:57.000000 jawanndenn-2.5.0/jawanndenn/tests/test_markup.py
--rw-r--r--   0 sping     (1000) sping     (1000)      974 2020-08-07 18:17:36.000000 jawanndenn-2.5.0/jawanndenn/tests/test_middleware.py
--rw-r--r--   0 sping     (1000) sping     (1000)     6897 2020-08-17 19:13:29.000000 jawanndenn-2.5.0/jawanndenn/tests/test_views.py
--rw-r--r--   0 sping     (1000) sping     (1000)     3810 2020-05-21 17:16:42.000000 jawanndenn-2.5.0/jawanndenn/urls.py
--rw-r--r--   0 sping     (1000) sping     (1000)     4166 2020-07-26 23:40:32.000000 jawanndenn-2.5.0/jawanndenn/views.py
--rw-r--r--   0 sping     (1000) sping     (1000)      397 2019-12-02 19:28:12.000000 jawanndenn-2.5.0/jawanndenn/wsgi.py
--rw-r--r--   0 sping     (1000) sping     (1000)    46311 2020-05-11 15:49:45.000000 jawanndenn-2.5.0/jawanndenn-setup.png
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-07-20 15:57:47.699542 jawanndenn-2.5.0/jawanndenn.egg-info/
--rw-r--r--   0 sping     (1000) sping     (1000)    10898 2021-07-20 15:57:47.000000 jawanndenn-2.5.0/jawanndenn.egg-info/PKG-INFO
--rw-r--r--   0 sping     (1000) sping     (1000)    10379 2021-07-20 15:57:47.000000 jawanndenn-2.5.0/jawanndenn.egg-info/SOURCES.txt
--rw-r--r--   0 sping     (1000) sping     (1000)        1 2021-07-20 15:57:47.000000 jawanndenn-2.5.0/jawanndenn.egg-info/dependency_links.txt
--rw-r--r--   0 sping     (1000) sping     (1000)       57 2021-07-20 15:57:47.000000 jawanndenn-2.5.0/jawanndenn.egg-info/entry_points.txt
--rw-r--r--   0 sping     (1000) sping     (1000)      225 2021-07-20 15:57:47.000000 jawanndenn-2.5.0/jawanndenn.egg-info/requires.txt
--rw-r--r--   0 sping     (1000) sping     (1000)       11 2021-07-20 15:57:47.000000 jawanndenn-2.5.0/jawanndenn.egg-info/top_level.txt
--rwxr-xr-x   0 sping     (1000) sping     (1000)      631 2019-12-02 19:28:12.000000 jawanndenn-2.5.0/manage.py
--rw-r--r--   0 sping     (1000) sping     (1000)      805 2021-07-16 22:24:39.000000 jawanndenn-2.5.0/requirements.txt
--rw-r--r--   0 sping     (1000) sping     (1000)       38 2021-07-20 15:57:47.729542 jawanndenn-2.5.0/setup.cfg
--rwxr-xr-x   0 sping     (1000) sping     (1000)     2639 2021-04-27 17:46:18.000000 jawanndenn-2.5.0/setup.py
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-04-23 01:55:42.059081 jawanndenn-2.6.0/
+-rw-r--r--   0 sping     (1000) sping     (1000)     1587 2020-08-16 00:42:21.000000 jawanndenn-2.6.0/.dockerignore
+-rw-r--r--   0 sping     (1000) sping     (1000)      205 2023-01-29 23:59:34.000000 jawanndenn-2.6.0/.flake8
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-04-23 01:55:42.025081 jawanndenn-2.6.0/.github/
+-rw-r--r--   0 sping     (1000) sping     (1000)      436 2020-08-05 17:04:17.000000 jawanndenn-2.6.0/.github/dependabot.yml
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-04-23 01:55:42.026081 jawanndenn-2.6.0/.github/workflows/
+-rw-r--r--   0 sping     (1000) sping     (1000)     1234 2023-04-21 17:36:59.000000 jawanndenn-2.6.0/.github/workflows/build_and_test_using_docker.yml
+-rw-r--r--   0 sping     (1000) sping     (1000)      451 2023-04-21 17:36:59.000000 jawanndenn-2.6.0/.github/workflows/dockerignore_detect_out_of_sync.yml
+-rw-r--r--   0 sping     (1000) sping     (1000)     2082 2023-04-21 17:36:59.000000 jawanndenn-2.6.0/.github/workflows/pre_commit_detect_outdated.yml
+-rw-r--r--   0 sping     (1000) sping     (1000)      898 2023-04-23 00:21:46.000000 jawanndenn-2.6.0/.github/workflows/run_pre_commit.yml
+-rw-r--r--   0 sping     (1000) sping     (1000)       51 2023-04-23 01:47:25.000000 jawanndenn-2.6.0/.gitignore
+-rw-r--r--   0 sping     (1000) sping     (1000)       28 2023-01-29 23:59:34.000000 jawanndenn-2.6.0/.isort.cfg
+-rw-r--r--   0 sping     (1000) sping     (1000)      818 2023-04-23 00:21:46.000000 jawanndenn-2.6.0/.pre-commit-config.yaml
+-rw-r--r--   0 sping     (1000) sping     (1000)      126 2023-01-29 23:59:34.000000 jawanndenn-2.6.0/.style.yapf
+-rw-r--r--   0 sping     (1000) sping     (1000)     1527 2023-04-03 18:20:51.000000 jawanndenn-2.6.0/Dockerfile
+-rw-r--r--   0 sping     (1000) sping     (1000)    14575 2023-04-23 01:55:42.058081 jawanndenn-2.6.0/PKG-INFO
+-rw-r--r--   0 sping     (1000) sping     (1000)    13553 2023-04-03 18:09:20.000000 jawanndenn-2.6.0/README.rst
+-rw-r--r--   0 sping     (1000) sping     (1000)      139 2021-02-14 22:53:06.000000 jawanndenn-2.6.0/crontab
+-rw-r--r--   0 sping     (1000) sping     (1000)     3206 2023-04-03 19:10:40.000000 jawanndenn-2.6.0/docker-compose.yml
+-rwxr-xr-x   0 sping     (1000) sping     (1000)      985 2020-08-11 21:08:17.000000 jawanndenn-2.6.0/docker-entrypoint.sh
+-rwxr-xr-x   0 sping     (1000) sping     (1000)      708 2020-01-26 15:52:37.000000 jawanndenn-2.6.0/generate_whitelist_dockerignore_file.sh
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-04-23 01:55:42.029081 jawanndenn-2.6.0/jawanndenn/
+-rw-r--r--   0 sping     (1000) sping     (1000)       57 2019-12-02 19:28:12.000000 jawanndenn-2.6.0/jawanndenn/__init__.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     6542 2023-01-29 23:59:34.000000 jawanndenn-2.6.0/jawanndenn/__main__.py
+-rw-r--r--   0 sping     (1000) sping     (1000)      397 2019-12-19 22:38:26.000000 jawanndenn-2.6.0/jawanndenn/asgi.py
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-04-23 01:55:42.030081 jawanndenn-2.6.0/jawanndenn/management/
+-rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-08-16 00:42:21.000000 jawanndenn-2.6.0/jawanndenn/management/__init__.py
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-04-23 01:55:42.031081 jawanndenn-2.6.0/jawanndenn/management/commands/
+-rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-08-16 00:42:21.000000 jawanndenn-2.6.0/jawanndenn/management/commands/__init__.py
+-rw-r--r--   0 sping     (1000) sping     (1000)      430 2023-01-29 23:59:34.000000 jawanndenn-2.6.0/jawanndenn/management/commands/prune_expired_polls.py
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-04-23 01:55:42.031081 jawanndenn-2.6.0/jawanndenn/management/commands/tests/
+-rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-08-16 00:42:21.000000 jawanndenn-2.6.0/jawanndenn/management/commands/tests/__init__.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     1012 2023-01-29 23:59:34.000000 jawanndenn-2.6.0/jawanndenn/management/commands/tests/test_prune_expired_polls.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     1384 2023-01-29 23:59:34.000000 jawanndenn-2.6.0/jawanndenn/markup.py
+-rw-r--r--   0 sping     (1000) sping     (1000)      202 2023-04-23 01:52:37.000000 jawanndenn-2.6.0/jawanndenn/metadata.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     1610 2023-01-29 23:59:34.000000 jawanndenn-2.6.0/jawanndenn/middleware.py
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-04-23 01:55:42.032081 jawanndenn-2.6.0/jawanndenn/migrations/
+-rw-r--r--   0 sping     (1000) sping     (1000)     4446 2023-01-29 23:59:34.000000 jawanndenn-2.6.0/jawanndenn/migrations/0001_initial.py
+-rw-r--r--   0 sping     (1000) sping     (1000)      467 2020-08-15 23:54:51.000000 jawanndenn-2.6.0/jawanndenn/migrations/0002_django_extensions_3_0_0.py
+-rw-r--r--   0 sping     (1000) sping     (1000)      392 2020-08-16 00:42:21.000000 jawanndenn-2.6.0/jawanndenn/migrations/0003_poll_expires_at.py
+-rw-r--r--   0 sping     (1000) sping     (1000)        0 2019-12-02 19:28:12.000000 jawanndenn-2.6.0/jawanndenn/migrations/__init__.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     1626 2023-01-29 23:59:34.000000 jawanndenn-2.6.0/jawanndenn/models.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     1836 2023-01-29 23:59:34.000000 jawanndenn-2.6.0/jawanndenn/serializers.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     6301 2023-04-23 00:21:46.000000 jawanndenn-2.6.0/jawanndenn/settings.py
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-04-23 01:55:42.021081 jawanndenn-2.6.0/jawanndenn/static/
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-04-23 01:55:42.020081 jawanndenn-2.6.0/jawanndenn/static/3rdparty/
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-04-23 01:55:42.032081 jawanndenn-2.6.0/jawanndenn/static/3rdparty/github-buttons-4.0.1/
+-rw-r--r--   0 sping     (1000) sping     (1000)      545 2020-05-20 19:48:30.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/github-buttons-4.0.1/LICENSE.md
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-04-23 01:55:42.033081 jawanndenn-2.6.0/jawanndenn/static/3rdparty/github-buttons-4.0.1/docs/
+-rw-r--r--   0 sping     (1000) sping     (1000)     5419 2020-05-20 19:48:30.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/github-buttons-4.0.1/docs/github-btn.html
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-04-23 01:55:42.033081 jawanndenn-2.6.0/jawanndenn/static/3rdparty/jquery-3.5.1/
+-rw-r--r--   0 sping     (1000) sping     (1000)     1095 2020-05-10 22:05:44.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/jquery-3.5.1/LICENSE.txt
+-rw-r--r--   0 sping     (1000) sping     (1000)    89476 2020-05-04 23:02:39.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/jquery-3.5.1/jquery-3.5.1.min.js
+-rw-r--r--   0 sping     (1000) sping     (1000)   137986 2020-05-04 23:02:39.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/jquery-3.5.1/jquery-3.5.1.min.map
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-04-23 01:55:42.034081 jawanndenn-2.6.0/jawanndenn/static/3rdparty/materialize-1.0.0/
+-rw-r--r--   0 sping     (1000) sping     (1000)     1083 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/materialize-1.0.0/LICENSE
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-04-23 01:55:42.035081 jawanndenn-2.6.0/jawanndenn/static/3rdparty/materialize-1.0.0/css/
+-rw-r--r--   0 sping     (1000) sping     (1000)   179245 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/materialize-1.0.0/css/materialize.css
+-rw-r--r--   0 sping     (1000) sping     (1000)   141841 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/materialize-1.0.0/css/materialize.min.css
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-04-23 01:55:42.036081 jawanndenn-2.6.0/jawanndenn/static/3rdparty/materialize-1.0.0/js/
+-rw-r--r--   0 sping     (1000) sping     (1000)   371026 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/materialize-1.0.0/js/materialize.js
+-rw-r--r--   0 sping     (1000) sping     (1000)   181114 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/materialize-1.0.0/js/materialize.min.js
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-04-23 01:55:42.036081 jawanndenn-2.6.0/jawanndenn/static/3rdparty/noty-2.4.1/
+-rw-r--r--   0 sping     (1000) sping     (1000)     1057 2019-11-30 21:03:50.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/noty-2.4.1/LICENSE.txt
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-04-23 01:55:42.020081 jawanndenn-2.6.0/jawanndenn/static/3rdparty/noty-2.4.1/js/
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-04-23 01:55:42.020081 jawanndenn-2.6.0/jawanndenn/static/3rdparty/noty-2.4.1/js/noty/
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-04-23 01:55:42.036081 jawanndenn-2.6.0/jawanndenn/static/3rdparty/noty-2.4.1/js/noty/packaged/
+-rw-r--r--   0 sping     (1000) sping     (1000)    32688 2019-11-30 21:03:50.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/noty-2.4.1/js/noty/packaged/jquery.noty.packaged.min.js
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-04-23 01:55:42.037081 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/
+-rw-r--r--   0 sping     (1000) sping     (1000)    11358 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/COPYING
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-04-23 01:55:42.037081 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/css/
+-rw-r--r--   0 sping     (1000) sping     (1000)    13602 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/css/roboto.css
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-04-23 01:55:42.055081 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/
+-rw-r--r--   0 sping     (1000) sping     (1000)    58088 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-100.eot
+-rw-r--r--   0 sping     (1000) sping     (1000)    49675 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-100.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)   132100 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-100.ttf
+-rw-r--r--   0 sping     (1000) sping     (1000)    64700 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-100.woff
+-rw-r--r--   0 sping     (1000) sping     (1000)    49988 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-100.woff2
+-rw-r--r--   0 sping     (1000) sping     (1000)    62556 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-100italic.eot
+-rw-r--r--   0 sping     (1000) sping     (1000)    56194 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-100italic.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)   135068 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-100italic.ttf
+-rw-r--r--   0 sping     (1000) sping     (1000)    69568 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-100italic.woff
+-rw-r--r--   0 sping     (1000) sping     (1000)    53900 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-100italic.woff2
+-rw-r--r--   0 sping     (1000) sping     (1000)    59393 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-300.eot
+-rw-r--r--   0 sping     (1000) sping     (1000)    49248 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-300.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)   130640 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-300.ttf
+-rw-r--r--   0 sping     (1000) sping     (1000)    65784 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-300.woff
+-rw-r--r--   0 sping     (1000) sping     (1000)    50812 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-300.woff2
+-rw-r--r--   0 sping     (1000) sping     (1000)    64726 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-300italic.eot
+-rw-r--r--   0 sping     (1000) sping     (1000)    54885 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-300italic.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)   134996 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-300italic.ttf
+-rw-r--r--   0 sping     (1000) sping     (1000)    71248 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-300italic.woff
+-rw-r--r--   0 sping     (1000) sping     (1000)    55724 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-300italic.woff2
+-rw-r--r--   0 sping     (1000) sping     (1000)    60298 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-500.eot
+-rw-r--r--   0 sping     (1000) sping     (1000)    48624 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-500.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)   132100 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-500.ttf
+-rw-r--r--   0 sping     (1000) sping     (1000)    66456 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-500.woff
+-rw-r--r--   0 sping     (1000) sping     (1000)    51400 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-500.woff2
+-rw-r--r--   0 sping     (1000) sping     (1000)    65334 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-500italic.eot
+-rw-r--r--   0 sping     (1000) sping     (1000)    53825 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-500italic.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)   135908 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-500italic.ttf
+-rw-r--r--   0 sping     (1000) sping     (1000)    71640 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-500italic.woff
+-rw-r--r--   0 sping     (1000) sping     (1000)    55912 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-500italic.woff2
+-rw-r--r--   0 sping     (1000) sping     (1000)    59829 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-700.eot
+-rw-r--r--   0 sping     (1000) sping     (1000)    48982 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-700.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)   131008 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-700.ttf
+-rw-r--r--   0 sping     (1000) sping     (1000)    66260 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-700.woff
+-rw-r--r--   0 sping     (1000) sping     (1000)    51088 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-700.woff2
+-rw-r--r--   0 sping     (1000) sping     (1000)    64455 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-700italic.eot
+-rw-r--r--   0 sping     (1000) sping     (1000)    53453 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-700italic.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)   134500 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-700italic.ttf
+-rw-r--r--   0 sping     (1000) sping     (1000)    70756 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-700italic.woff
+-rw-r--r--   0 sping     (1000) sping     (1000)    55192 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-700italic.woff2
+-rw-r--r--   0 sping     (1000) sping     (1000)    59887 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-900.eot
+-rw-r--r--   0 sping     (1000) sping     (1000)    48022 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-900.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)   131608 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-900.ttf
+-rw-r--r--   0 sping     (1000) sping     (1000)    66412 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-900.woff
+-rw-r--r--   0 sping     (1000) sping     (1000)    51212 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-900.woff2
+-rw-r--r--   0 sping     (1000) sping     (1000)    65948 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-900italic.eot
+-rw-r--r--   0 sping     (1000) sping     (1000)    53240 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-900italic.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)   136420 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-900italic.ttf
+-rw-r--r--   0 sping     (1000) sping     (1000)    72360 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-900italic.woff
+-rw-r--r--   0 sping     (1000) sping     (1000)    56556 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-900italic.woff2
+-rw-r--r--   0 sping     (1000) sping     (1000)    64104 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-italic.eot
+-rw-r--r--   0 sping     (1000) sping     (1000)    54053 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-italic.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)   133248 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-italic.ttf
+-rw-r--r--   0 sping     (1000) sping     (1000)    70252 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-italic.woff
+-rw-r--r--   0 sping     (1000) sping     (1000)    54984 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-italic.woff2
+-rw-r--r--   0 sping     (1000) sping     (1000)    59644 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-regular.eot
+-rw-r--r--   0 sping     (1000) sping     (1000)    48974 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-regular.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)   131916 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-regular.ttf
+-rw-r--r--   0 sping     (1000) sping     (1000)    66044 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-regular.woff
+-rw-r--r--   0 sping     (1000) sping     (1000)    51116 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-regular.woff2
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-04-23 01:55:42.055081 jawanndenn-2.6.0/jawanndenn/static/css/
+-rw-r--r--   0 sping     (1000) sping     (1000)     4318 2020-05-11 15:36:18.000000 jawanndenn-2.6.0/jawanndenn/static/css/style.css
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-04-23 01:55:42.056081 jawanndenn-2.6.0/jawanndenn/static/html/
+-rw-r--r--   0 sping     (1000) sping     (1000)      869 2020-05-20 19:49:42.000000 jawanndenn-2.6.0/jawanndenn/static/html/footer.htm
+-rw-r--r--   0 sping     (1000) sping     (1000)     2400 2022-01-21 18:19:51.000000 jawanndenn-2.6.0/jawanndenn/static/html/poll.htm
+-rw-r--r--   0 sping     (1000) sping     (1000)     2475 2022-01-21 18:19:51.000000 jawanndenn-2.6.0/jawanndenn/static/html/setup.htm
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-04-23 01:55:42.057081 jawanndenn-2.6.0/jawanndenn/static/js/
+-rw-r--r--   0 sping     (1000) sping     (1000)     1054 2019-12-23 19:38:24.000000 jawanndenn-2.6.0/jawanndenn/static/js/html.js
+-rw-r--r--   0 sping     (1000) sping     (1000)     6625 2020-05-20 19:34:30.000000 jawanndenn-2.6.0/jawanndenn/static/js/poll.js
+-rw-r--r--   0 sping     (1000) sping     (1000)     4369 2020-08-16 00:42:21.000000 jawanndenn-2.6.0/jawanndenn/static/js/setup.js
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-04-23 01:55:42.058081 jawanndenn-2.6.0/jawanndenn/tests/
+-rw-r--r--   0 sping     (1000) sping     (1000)        0 2019-12-01 21:56:57.000000 jawanndenn-2.6.0/jawanndenn/tests/__init__.py
+-rw-r--r--   0 sping     (1000) sping     (1000)      874 2023-01-29 23:59:34.000000 jawanndenn-2.6.0/jawanndenn/tests/factories.py
+-rw-r--r--   0 sping     (1000) sping     (1000)      236 2023-01-29 23:37:03.000000 jawanndenn-2.6.0/jawanndenn/tests/helpers.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     1389 2023-01-29 23:59:34.000000 jawanndenn-2.6.0/jawanndenn/tests/test_markup.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     1134 2023-01-29 23:59:34.000000 jawanndenn-2.6.0/jawanndenn/tests/test_middleware.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     7174 2023-01-29 23:59:34.000000 jawanndenn-2.6.0/jawanndenn/tests/test_views.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     3718 2023-04-23 01:46:18.000000 jawanndenn-2.6.0/jawanndenn/urls.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     4696 2023-04-23 01:46:18.000000 jawanndenn-2.6.0/jawanndenn/views.py
+-rw-r--r--   0 sping     (1000) sping     (1000)      397 2019-12-02 19:28:12.000000 jawanndenn-2.6.0/jawanndenn/wsgi.py
+-rw-r--r--   0 sping     (1000) sping     (1000)    46311 2020-05-11 15:49:45.000000 jawanndenn-2.6.0/jawanndenn-setup.png
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-04-23 01:55:42.030081 jawanndenn-2.6.0/jawanndenn.egg-info/
+-rw-r--r--   0 sping     (1000) sping     (1000)    14575 2023-04-23 01:55:41.000000 jawanndenn-2.6.0/jawanndenn.egg-info/PKG-INFO
+-rw-r--r--   0 sping     (1000) sping     (1000)    10438 2023-04-23 01:55:41.000000 jawanndenn-2.6.0/jawanndenn.egg-info/SOURCES.txt
+-rw-r--r--   0 sping     (1000) sping     (1000)        1 2023-04-23 01:55:41.000000 jawanndenn-2.6.0/jawanndenn.egg-info/dependency_links.txt
+-rw-r--r--   0 sping     (1000) sping     (1000)       56 2023-04-23 01:55:41.000000 jawanndenn-2.6.0/jawanndenn.egg-info/entry_points.txt
+-rw-r--r--   0 sping     (1000) sping     (1000)      225 2023-04-23 01:55:41.000000 jawanndenn-2.6.0/jawanndenn.egg-info/requires.txt
+-rw-r--r--   0 sping     (1000) sping     (1000)       11 2023-04-23 01:55:41.000000 jawanndenn-2.6.0/jawanndenn.egg-info/top_level.txt
+-rwxr-xr-x   0 sping     (1000) sping     (1000)      637 2023-01-29 23:59:34.000000 jawanndenn-2.6.0/manage.py
+-rw-r--r--   0 sping     (1000) sping     (1000)    33427 2023-04-21 17:36:59.000000 jawanndenn-2.6.0/requirements.txt
+-rw-r--r--   0 sping     (1000) sping     (1000)       38 2023-04-23 01:55:42.059081 jawanndenn-2.6.0/setup.cfg
+-rwxr-xr-x   0 sping     (1000) sping     (1000)     2628 2023-04-23 01:51:12.000000 jawanndenn-2.6.0/setup.py
```

### Comparing `jawanndenn-2.5.0/.dockerignore` & `jawanndenn-2.6.0/.dockerignore`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/.github/workflows/build_and_test_using_docker.yml` & `jawanndenn-2.6.0/.github/workflows/build_and_test_using_docker.yml`

 * *Files 21% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 on:
 - pull_request
 - push
 
 jobs:
   build_and_test:
     name: Build and test using Docker
-    runs-on: ubuntu-18.04
+    runs-on: ubuntu-22.04
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@8e5e7e5ab8b370d6c329ec480221332ada57f0ab  # v3.5.2
 
-      - name: Set up Python 3.8
-        uses: actions/setup-python@v2.2.2
+      - name: Set up Python 3.10
+        uses: actions/setup-python@d27e3f3d7c64b4bbf8e4abfb9b63b83e846e0435  # v4.5.0
         with:
-          python-version: 3.8
+          python-version: '3.10'
 
       - name: Install dependencies
         run: |-
           pip install \
             --disable-pip-version-check \
             --user \
             --no-warn-script-location \
```

### Comparing `jawanndenn-2.5.0/.github/workflows/run_pre_commit.yml` & `jawanndenn-2.6.0/.github/workflows/run_pre_commit.yml`

 * *Files 15% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 on:
 - pull_request
 - push
 
 jobs:
   run_pre_commit:
     name: Run pre-commit on all files
-    runs-on: ubuntu-18.04
+    runs-on: ubuntu-22.04
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@8e5e7e5ab8b370d6c329ec480221332ada57f0ab  # v3.5.2
 
-      - name: Set up Python 3.8
-        uses: actions/setup-python@v2.2.2
+      - name: Set up Python 3.10
+        uses: actions/setup-python@d27e3f3d7c64b4bbf8e4abfb9b63b83e846e0435  # v4.5.0
         with:
-          python-version: 3.8
+          python-version: '3.10'
 
       - name: Install pre-commit
         run: |-
           pip install \
             --disable-pip-version-check \
             --user \
             --no-warn-script-location \
@@ -27,8 +27,8 @@
 
       - name: Install pre-commit hooks
         run: |-
           pre-commit install --install-hooks
 
       - name: Run pre-commit on all files
         run: |-
-          pre-commit run --all-files
+          pre-commit run --all-files --show-diff-on-failure
```

### Comparing `jawanndenn-2.5.0/.pre-commit-config.yaml` & `jawanndenn-2.6.0/.pre-commit-config.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 exclude: '^jawanndenn/static/3rdparty/'
 
 repos:
   - repo: https://github.com/asottile/pyupgrade
-    rev: v2.21.2
+    rev: v3.3.1
     hooks:
       - id: pyupgrade
         args: ['--py38-plus']
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.0.1
+    rev: v4.4.0
     hooks:
       - id: check-json
       - id: check-yaml
       - id: check-merge-conflict
       - id: end-of-file-fixer
       - id: trailing-whitespace
 
-  - repo: https://gitlab.com/pycqa/flake8
-    rev: 3.9.2
+  - repo: https://github.com/PyCQA/flake8
+    rev: 6.0.0
     hooks:
       - id: flake8
         exclude: '^jawanndenn/migrations/'
 
-  - repo: https://github.com/pre-commit/mirrors-isort
-    rev: v5.9.2
+  - repo: https://github.com/pycqa/isort
+    rev: 5.12.0
     hooks:
       - id: isort
 
   - repo: https://github.com/Lucas-C/pre-commit-hooks-markup
     rev: v1.0.1
     hooks:
       - id: rst-linter
+
+  - repo: https://github.com/google/yapf
+    rev: v0.33.0
+    hooks:
+      - id: yapf
```

### Comparing `jawanndenn-2.5.0/Dockerfile` & `jawanndenn-2.6.0/Dockerfile`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-FROM python:3.8-alpine
+FROM python:3.10-alpine
 
-RUN apk update && apk add \
+RUN echo '@edge-community https://dl-cdn.alpinelinux.org/alpine/edge/community' >> /etc/apk/repositories \
+        && \
+    apk add --update \
         bash \
         diffutils \
         g++ \
         gcc \
         musl-dev \
         postgresql-client \
         postgresql-dev \
-        shadow
+        shadow \
+        supercronic@edge-community
 
+SHELL ["/bin/bash", "-c"]
 RUN mkdir -p /var/mail  # to avoid warning "Creating mailbox file: No such file or directory"
 RUN useradd --create-home --uid 1001 --non-unique jawanndenn
 USER jawanndenn
 ENV PATH=/home/jawanndenn/.local/bin/:${PATH}
 
 
 COPY --chown=jawanndenn:jawanndenn requirements.txt  /tmp/app/
 RUN cd /tmp/app \
         && \
     pip3 install --user --ignore-installed --disable-pip-version-check pip setuptools wheel \
         && \
     hash pip3 \
         && \
-    pip3 install --user -r requirements.txt \
+    pip3 install --user --require-hashes -r requirements.txt \
         && \
     pip3 check \
         && \
-    bash -c "diff -u0 <(pip freeze | sort -f) <(sed -e '/^#/d' -e '/^$/d' requirements.txt | sort -f)"
+    diff -u0 <(pip freeze | sort -f) <(sed -e '/--hash=/d' -e 's/ \\$//' -e '/^#/d' -e '/^$/d' requirements.txt | sort -f)
 
 USER root
-RUN apk update && apk upgrade
-# Enable testing repository for nothing but package "supercronic".
-# It's done down here so that we get as little as possible from testing.
-RUN echo http://dl-cdn.alpinelinux.org/alpine/edge/testing >> /etc/apk/repositories
-RUN apk update && apk add supercronic
+RUN apk upgrade --update
 USER jawanndenn
 
 COPY --chown=jawanndenn:jawanndenn jawanndenn/          /tmp/app/jawanndenn/
 COPY --chown=jawanndenn:jawanndenn setup.py README.rst  /tmp/app/
 RUN cd /tmp/app \
         && \
     pip3 install --user . \
```

### Comparing `jawanndenn-2.5.0/PKG-INFO` & `jawanndenn-2.6.0/README.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,10 @@
-Metadata-Version: 2.1
-Name: jawanndenn
-Version: 2.5.0
-Summary: Libre alternative to Doodle
-Home-page: https://github.com/hartwork/jawanndenn
-Author: Sebastian Pipping
-Author-email: sebastian@pipping.org
-License: AGPLv3+
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Programming Language :: JavaScript
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
-Classifier: Topic :: Office/Business :: Scheduling
-Requires-Python: >=3.6
-Provides-Extra: tests
-
+.. image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit
+   :target: https://github.com/pre-commit/pre-commit
+   :alt: pre-commit
 .. image:: https://github.com/hartwork/jawanndenn/workflows/Build%20and%20test%20using%20Docker/badge.svg
     :target: https://github.com/hartwork/jawanndenn/actions
 
 
 What is jawanndenn?
 ===================
 
@@ -115,20 +92,132 @@
 ::
 
     JAWANNDENN_POSTGRES_NAME=jawanndenn
     JAWANNDENN_POSTGRES_USER=jawanndenn
     JAWANNDENN_POSTGRES_PASSWORD=dEb2PIcinemA8poH
     JAWANNDENN_SECRET_KEY=606ea88f183a27919d5c27ec7f948906d23fdd7821684eb59e8bcf7377e3853b
 
-Make sure to use your own values!
+Make sure to **adjust these values** after copy and paste!
 
 You can then build and run a docker image using ``docker-compose up --build``.
 
-PostgreSQL data is saved to ``~/.jawanndenn-docker-pgdata/`` on the host system.
 The app is served on ``localhost:54080``.
+PostgreSQL data is saved to ``~/.jawanndenn-docker-pgdata/`` on the host system.
+There is also an instance of Redis used for cross-process rate limiting,
+and a "cron" housekeeping container that will go delete polls that have exceeded their
+configured lifetime, every 60 minutes.
+
+(If you need a low-maintenance SSL reverse proxy in front of jawanndenn,
+`docker-ssl-reverse-proxy <https://github.com/hartwork/docker-ssl-reverse-proxy>`_
+could be of interest.)
+
+There is a few more environment variables that you could want to adjust in your environment.
+Altogether, there are these variables:
+
+
+Environment variables
+---------------------
+
+``DJANGO_SETTINGS_MODULE``
+~~~~~~~~~~~~~~~~~~~~~~~~~~
+Django settings module to use, leave as is, defaults to ``jawanndenn.settings``
+(see ``docker-compose.yml``)
+
+
+``JAWANNDENN_ALLOWED_HOSTS``
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+Hostnames to serve jawanndenn at, list separated by comma,
+is set to ``jawanndenn.de,www.jawanndenn.de`` on the main production server,
+defaults to ``127.0.0.1,0.0.0.0,localhost``
+(see ``jawanndenn/settings.py``)
+
+
+``JAWANNDENN_DEBUG``
+~~~~~~~~~~~~~~~~~~~~
+Debug mode, disabled for all values but ``True``, disabled by default,
+should never be enabled in production for security
+(see ``jawanndenn/settings.py``)
+
+
+``JAWANNDENN_MAX_POLLS``
+~~~~~~~~~~~~~~~~~~~~~~~~
+Maximum total number of polls to store, denial of service protection,
+defaults to ``1000``
+(see ``jawanndenn/settings.py`` and ``docker-compose.yml``)
+
+
+``JAWANNDENN_MAX_VOTES_PER_POLL``
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+Maximum total number of polls to store, denial of service protection,
+defaults to ``40``
+(see ``jawanndenn/settings.py``)
+
+
+``JAWANNDENN_POSTGRES_HOST``
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+Hostname of the PostgreSQL database to connect to; defaults to ``postgres``
+(see ``docker-compose.yml``)
+
+
+``JAWANNDENN_POSTGRES_NAME``
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+Database name of the PostgreSQL database to connect to;
+no default, always required
+
+
+``JAWANNDENN_POSTGRES_PASSWORD``
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+Password for log-in with the PostgreSQL database;
+no default, always required
+
+
+``JAWANNDENN_POSTGRES_PORT``
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+Port of the PostgreSQL database to connect to; defaults to ``5432``
+(see ``docker-compose.yml``)
+
+
+``JAWANNDENN_POSTGRES_USER``
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+Username for log-in with the PostgreSQL database;
+no default, always required
+
+
+``JAWANNDENN_REDIS_HOST``
+~~~~~~~~~~~~~~~~~~~~~~~~~
+Hostname of the Redis database to connect to; defaults to ``redis``
+(see ``docker-compose.yml``)
+
+
+``JAWANNDENN_REDIS_PORT``
+~~~~~~~~~~~~~~~~~~~~~~~~~
+Port of the Redis database to connect to; defaults to ``6379``
+(see ``docker-compose.yml``)
+
+
+``JAWANNDENN_SECRET_KEY``
+~~~~~~~~~~~~~~~~~~~~~~~~~
+`Django secret key <https://docs.djangoproject.com/en/4.0/ref/settings/#secret-key>`_;
+should be long, generated, not used elsewhere; no default, always required
+
+
+``JAWANNDENN_SENTRY_DSN``
+~~~~~~~~~~~~~~~~~~~~~~~~~
+`Data source name (DSN) <https://docs.sentry.io/product/sentry-basics/dsn-explainer/>`_
+for use with `Sentry <https://sentry.io/>`_, disabled/empty by default
+(see ``jawanndenn/settings.py``)
+
+
+``JAWANNDENN_URL_PREFIX``
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+Prefix string to insert into URLs rather after the domain name
+to help with hosting multiple apps under the same domain side by side;
+e.g. prefix ``prefix123`` will result in URLs like ``https://<domain>/prefix123/poll/<id>``;
+empty by default
+(see ``jawanndenn/settings.py``)
 
 
 Command line usage
 ==================
 
 When installed, invocation is as simple as
 
@@ -224,14 +313,15 @@
    -  `Framadata`_ (`Sources`_, ex. `OpenSondage`_, ex. `STUdS`_)
    -  `Nextcloud Polls`_
    -  `Noodle`_
    -  `Nuages`_
    -  `Pleft`_
    -  `Rallly`_
    -  `RDVz`_
+   -  `sowhenthen`_
 
 -  Keep things simple, usable, maintainable
 -  Support invocation from the command line, e.g. for spontaneous polls in a LAN
 -  Have security in mind
 
 Please check out the `list of upcoming features`_.
 
@@ -298,15 +388,14 @@
 .. _Foodle: https://foodl.org/
 .. _on GitHub: https://github.com/UNINETT/Foodle
 .. _DFN scheduler: https://terminplaner.dfn.de/
 .. _DFN Terminplaner+: https://terminplaner2.dfn.de/
 .. _Dudle: https://dudle.inf.tu-dresden.de/
 .. _Nuages: https://nuages.domainepublic.net/
 .. _RDVz: https://sourceforge.net/projects/rdvz/
+.. _sowhenthen: https://github.com/kiyutink/sowhenthen
 .. _Drupal Date picker formatter: http://alternativeto.net/software/date-picker-formatter-dudel-for-drupal/?license=opensource
 .. _Nextcloud Polls: https://github.com/nextcloud/polls
 .. _Noodle: https://github.com/kmerz/noodle
 .. _Rallly: https://github.com/lukevella/Rallly
 .. _list of upcoming features: https://github.com/hartwork/jawanndenn/issues/created_by/hartwork
 .. _@KordonDev: https://github.com/KordonDev
-
-
```

### Comparing `jawanndenn-2.5.0/README.rst` & `jawanndenn-2.6.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,35 @@
+Metadata-Version: 2.1
+Name: jawanndenn
+Version: 2.6.0
+Summary: Libre alternative to Doodle
+Home-page: https://github.com/hartwork/jawanndenn
+Author: Sebastian Pipping
+Author-email: sebastian@pipping.org
+License: AGPLv3+
+Classifier: Development Status :: 4 - Beta
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 2.2
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Programming Language :: JavaScript
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
+Classifier: Topic :: Office/Business :: Scheduling
+Requires-Python: >=3.6
+Provides-Extra: tests
+
+.. image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit
+   :target: https://github.com/pre-commit/pre-commit
+   :alt: pre-commit
 .. image:: https://github.com/hartwork/jawanndenn/workflows/Build%20and%20test%20using%20Docker/badge.svg
     :target: https://github.com/hartwork/jawanndenn/actions
 
 
 What is jawanndenn?
 ===================
 
@@ -89,20 +117,132 @@
 ::
 
     JAWANNDENN_POSTGRES_NAME=jawanndenn
     JAWANNDENN_POSTGRES_USER=jawanndenn
     JAWANNDENN_POSTGRES_PASSWORD=dEb2PIcinemA8poH
     JAWANNDENN_SECRET_KEY=606ea88f183a27919d5c27ec7f948906d23fdd7821684eb59e8bcf7377e3853b
 
-Make sure to use your own values!
+Make sure to **adjust these values** after copy and paste!
 
 You can then build and run a docker image using ``docker-compose up --build``.
 
-PostgreSQL data is saved to ``~/.jawanndenn-docker-pgdata/`` on the host system.
 The app is served on ``localhost:54080``.
+PostgreSQL data is saved to ``~/.jawanndenn-docker-pgdata/`` on the host system.
+There is also an instance of Redis used for cross-process rate limiting,
+and a "cron" housekeeping container that will go delete polls that have exceeded their
+configured lifetime, every 60 minutes.
+
+(If you need a low-maintenance SSL reverse proxy in front of jawanndenn,
+`docker-ssl-reverse-proxy <https://github.com/hartwork/docker-ssl-reverse-proxy>`_
+could be of interest.)
+
+There is a few more environment variables that you could want to adjust in your environment.
+Altogether, there are these variables:
+
+
+Environment variables
+---------------------
+
+``DJANGO_SETTINGS_MODULE``
+~~~~~~~~~~~~~~~~~~~~~~~~~~
+Django settings module to use, leave as is, defaults to ``jawanndenn.settings``
+(see ``docker-compose.yml``)
+
+
+``JAWANNDENN_ALLOWED_HOSTS``
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+Hostnames to serve jawanndenn at, list separated by comma,
+is set to ``jawanndenn.de,www.jawanndenn.de`` on the main production server,
+defaults to ``127.0.0.1,0.0.0.0,localhost``
+(see ``jawanndenn/settings.py``)
+
+
+``JAWANNDENN_DEBUG``
+~~~~~~~~~~~~~~~~~~~~
+Debug mode, disabled for all values but ``True``, disabled by default,
+should never be enabled in production for security
+(see ``jawanndenn/settings.py``)
+
+
+``JAWANNDENN_MAX_POLLS``
+~~~~~~~~~~~~~~~~~~~~~~~~
+Maximum total number of polls to store, denial of service protection,
+defaults to ``1000``
+(see ``jawanndenn/settings.py`` and ``docker-compose.yml``)
+
+
+``JAWANNDENN_MAX_VOTES_PER_POLL``
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+Maximum total number of polls to store, denial of service protection,
+defaults to ``40``
+(see ``jawanndenn/settings.py``)
+
+
+``JAWANNDENN_POSTGRES_HOST``
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+Hostname of the PostgreSQL database to connect to; defaults to ``postgres``
+(see ``docker-compose.yml``)
+
+
+``JAWANNDENN_POSTGRES_NAME``
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+Database name of the PostgreSQL database to connect to;
+no default, always required
+
+
+``JAWANNDENN_POSTGRES_PASSWORD``
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+Password for log-in with the PostgreSQL database;
+no default, always required
+
+
+``JAWANNDENN_POSTGRES_PORT``
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+Port of the PostgreSQL database to connect to; defaults to ``5432``
+(see ``docker-compose.yml``)
+
+
+``JAWANNDENN_POSTGRES_USER``
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+Username for log-in with the PostgreSQL database;
+no default, always required
+
+
+``JAWANNDENN_REDIS_HOST``
+~~~~~~~~~~~~~~~~~~~~~~~~~
+Hostname of the Redis database to connect to; defaults to ``redis``
+(see ``docker-compose.yml``)
+
+
+``JAWANNDENN_REDIS_PORT``
+~~~~~~~~~~~~~~~~~~~~~~~~~
+Port of the Redis database to connect to; defaults to ``6379``
+(see ``docker-compose.yml``)
+
+
+``JAWANNDENN_SECRET_KEY``
+~~~~~~~~~~~~~~~~~~~~~~~~~
+`Django secret key <https://docs.djangoproject.com/en/4.0/ref/settings/#secret-key>`_;
+should be long, generated, not used elsewhere; no default, always required
+
+
+``JAWANNDENN_SENTRY_DSN``
+~~~~~~~~~~~~~~~~~~~~~~~~~
+`Data source name (DSN) <https://docs.sentry.io/product/sentry-basics/dsn-explainer/>`_
+for use with `Sentry <https://sentry.io/>`_, disabled/empty by default
+(see ``jawanndenn/settings.py``)
+
+
+``JAWANNDENN_URL_PREFIX``
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+Prefix string to insert into URLs rather after the domain name
+to help with hosting multiple apps under the same domain side by side;
+e.g. prefix ``prefix123`` will result in URLs like ``https://<domain>/prefix123/poll/<id>``;
+empty by default
+(see ``jawanndenn/settings.py``)
 
 
 Command line usage
 ==================
 
 When installed, invocation is as simple as
 
@@ -198,14 +338,15 @@
    -  `Framadata`_ (`Sources`_, ex. `OpenSondage`_, ex. `STUdS`_)
    -  `Nextcloud Polls`_
    -  `Noodle`_
    -  `Nuages`_
    -  `Pleft`_
    -  `Rallly`_
    -  `RDVz`_
+   -  `sowhenthen`_
 
 -  Keep things simple, usable, maintainable
 -  Support invocation from the command line, e.g. for spontaneous polls in a LAN
 -  Have security in mind
 
 Please check out the `list of upcoming features`_.
 
@@ -272,13 +413,14 @@
 .. _Foodle: https://foodl.org/
 .. _on GitHub: https://github.com/UNINETT/Foodle
 .. _DFN scheduler: https://terminplaner.dfn.de/
 .. _DFN Terminplaner+: https://terminplaner2.dfn.de/
 .. _Dudle: https://dudle.inf.tu-dresden.de/
 .. _Nuages: https://nuages.domainepublic.net/
 .. _RDVz: https://sourceforge.net/projects/rdvz/
+.. _sowhenthen: https://github.com/kiyutink/sowhenthen
 .. _Drupal Date picker formatter: http://alternativeto.net/software/date-picker-formatter-dudel-for-drupal/?license=opensource
 .. _Nextcloud Polls: https://github.com/nextcloud/polls
 .. _Noodle: https://github.com/kmerz/noodle
 .. _Rallly: https://github.com/lukevella/Rallly
 .. _list of upcoming features: https://github.com/hartwork/jawanndenn/issues/created_by/hartwork
 .. _@KordonDev: https://github.com/KordonDev
```

### Comparing `jawanndenn-2.5.0/docker-compose.yml` & `jawanndenn-2.6.0/docker-compose.yml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 networks:
   ssl-reverse-proxy:
     external: yes
 
 services:
   postgres:
-    image: postgres:11.6  # due to postgresql-client version 11.6 in Alpine 3.10
+    image: postgres:15.2  # due to postgresql-client version 15.2 in Alpine 3.17
     volumes:
       - ~/.jawanndenn-docker-pgdata/:/var/lib/postgresql/data
     environment:
       POSTGRES_USER: ${JAWANNDENN_POSTGRES_USER:?}
       POSTGRES_PASSWORD: ${JAWANNDENN_POSTGRES_PASSWORD:?}
       POSTGRES_DB: ${JAWANNDENN_POSTGRES_NAME:?}
     logging:
```

### Comparing `jawanndenn-2.5.0/docker-entrypoint.sh` & `jawanndenn-2.6.0/docker-entrypoint.sh`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/generate_whitelist_dockerignore_file.sh` & `jawanndenn-2.6.0/generate_whitelist_dockerignore_file.sh`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/__main__.py` & `jawanndenn-2.6.0/jawanndenn/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -53,73 +53,86 @@
         with open(filename, 'w', encoding=secret_key_encoding) as f:
             f.write(secret_key)
     return secret_key
 
 
 def _inner_main():
     parser = argparse.ArgumentParser(prog='jawanndenn')
-    parser.add_argument('--debug', action='store_true', default=False,
+    parser.add_argument('--debug',
+                        action='store_true',
+                        default=False,
                         help='Enable debug mode (default: disabled)')
-    parser.add_argument('--host', default='127.0.0.1', metavar='HOST',
+    parser.add_argument('--host',
+                        default='127.0.0.1',
+                        metavar='HOST',
                         help='Hostname or IP address to listen at'
-                             ' (default: %(default)s)')
-    parser.add_argument('--port', default=8080, type=int, metavar='PORT',
+                        ' (default: %(default)s)')
+    parser.add_argument('--port',
+                        default=8080,
+                        type=int,
+                        metavar='PORT',
                         help='Port to listen at (default: %(default)s)')
-    parser.add_argument('--url-prefix', default='', metavar='PATH',
+    parser.add_argument('--url-prefix',
+                        default='',
+                        metavar='PATH',
                         help='Path to prepend to URLs'
-                             ' (default: "%(default)s")')
-    parser.add_argument('--database-sqlite3', default='~/jawanndenn.sqlite3',
+                        ' (default: "%(default)s")')
+    parser.add_argument('--database-sqlite3',
+                        default='~/jawanndenn.sqlite3',
                         metavar='FILE',
                         help='File to write the database to'
-                             ' (default: %(default)s)')
+                        ' (default: %(default)s)')
     parser.add_argument('--django-secret-key-file',
-                        default='~/jawanndenn.secret_key', metavar='FILE',
+                        default='~/jawanndenn.secret_key',
+                        metavar='FILE',
                         help='File to use for Django secret key data'
-                             ' (default: %(default)s)')
+                        ' (default: %(default)s)')
 
     limits = parser.add_argument_group('limit configuration')
-    limits.add_argument('--max-polls', type=int, metavar='COUNT',
+    limits.add_argument('--max-polls',
+                        type=int,
+                        metavar='COUNT',
                         default=DEFAULT_MAX_POLLS,
                         help='Maximum number of polls total'
-                             ' (default: %(default)s)')
-    limits.add_argument('--max-votes-per-poll', type=int, metavar='COUNT',
+                        ' (default: %(default)s)')
+    limits.add_argument('--max-votes-per-poll',
+                        type=int,
+                        metavar='COUNT',
                         default=DEFAULT_MAX_VOTES_PER_POLL,
                         help='Maximum number of votes per poll'
-                             ' (default: %(default)s)')
+                        ' (default: %(default)s)')
 
     export_args = parser.add_argument_group('data import/export arguments')
-    export_args.add_argument('--dumpdata', action='store_true',
+    export_args.add_argument('--dumpdata',
+                             action='store_true',
                              help='Dump a JSON export of the database to '
-                                  'standard output, then quit.')
-    export_args.add_argument('--loaddata', metavar='FILE.json',
+                             'standard output, then quit.')
+    export_args.add_argument('--loaddata',
+                             metavar='FILE.json',
                              help='Load a JSON export of the database from '
-                                  'FILE.json, then quit.')
+                             'FILE.json, then quit.')
 
     options = parser.parse_args()
 
     logging.basicConfig(level=logging.DEBUG if options.debug else logging.INFO)
 
     if not options.dumpdata and not options.loaddata:
         _require_hash_randomization()
 
-    secret_key = _process_django_secret_key_file(
-        os.path.expanduser(options.django_secret_key_file))
+    secret_key = _process_django_secret_key_file(os.path.expanduser(
+        options.django_secret_key_file))
 
     # NOTE: These are read by the the Django settings module
-    os.environ['JAWANNDENN_ALLOWED_HOSTS'] = ','.join([options.host,
-                                                       '127.0.0.1',
-                                                       '0.0.0.0',
-                                                       'localhost'])
+    os.environ['JAWANNDENN_ALLOWED_HOSTS'] = ','.join(
+        [options.host, '127.0.0.1', '0.0.0.0', 'localhost'])
     os.environ['JAWANNDENN_DEBUG'] = str(options.debug)
     os.environ['JAWANNDENN_MAX_POLLS'] = str(options.max_polls)
-    os.environ['JAWANNDENN_MAX_VOTES_PER_POLL'] = str(options
-                                                      .max_votes_per_poll)
+    os.environ['JAWANNDENN_MAX_VOTES_PER_POLL'] = str(options.max_votes_per_poll)
     os.environ['JAWANNDENN_SECRET_KEY'] = secret_key
-    os.environ['JAWANNDENN_SQLITE_FILE'] = os.path.expanduser(
-        options.database_sqlite3)
+    os.environ['JAWANNDENN_SQLITE_FILE'] = os.path.expanduser(options.database_sqlite3)
     os.environ['JAWANNDENN_URL_PREFIX'] = options.url_prefix
 
     os.environ.setdefault('DJANGO_SETTINGS_MODULE', 'jawanndenn.settings')
 
     # Heavy imports are down here to keep --help fast
     from django.core.management import execute_from_command_line
 
@@ -128,26 +141,26 @@
         print()
 
     if options.dumpdata:
         execute_from_command_line(['./manage.py', 'dumpdata'])
     elif options.loaddata:
         print('Importing JSON dump'
               ' -- this may take a few seconds...', file=sys.stderr)
-        execute_from_command_line(['./manage.py', 'loaddata',
-                                   os.path.abspath(options.loaddata)])
+        execute_from_command_line(['./manage.py', 'loaddata', os.path.abspath(options.loaddata)])
     else:
-        sys.exit(subprocess.call([
-            'gunicorn',
-            '--name=jawanndenn',
-            f'--bind={options.host}:{options.port}',
-            '--workers=1',  # due to use of sqlite3 storage
-            '--access-logfile=-',
-            '--logger-class=gunicorn_color.Logger',
-            'jawanndenn.wsgi',
-        ]))
+        sys.exit(
+            subprocess.call([
+                'gunicorn',
+                '--name=jawanndenn',
+                f'--bind={options.host}:{options.port}',
+                '--workers=1',  # due to use of sqlite3 storage
+                '--access-logfile=-',
+                '--logger-class=gunicorn_color.Logger',
+                'jawanndenn.wsgi',
+            ]))
 
 
 def main():
     try:
         _inner_main()
     except KeyboardInterrupt:
         sys.exit(128 + signal.SIGINT)
```

### Comparing `jawanndenn-2.5.0/jawanndenn/management/commands/tests/test_prune_expired_polls.py` & `jawanndenn-2.6.0/jawanndenn/management/commands/tests/test_prune_expired_polls.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 
 from ....models import Poll
 from ....tests.factories import PollFactory
 from ..prune_expired_polls import Command
 
 
 class PruneExpiredPollsTest(TestCase):
+
     def test_deletes_expired_polls_and_those_only(self):
         expired_poll = PollFactory(expires_at=now())
-        not_yet_expired_poll = PollFactory(
-            expires_at=now() + timedelta(minutes=1))
+        not_yet_expired_poll = PollFactory(expires_at=now() + timedelta(minutes=1))
         never_expiring_poll = PollFactory(expires_at=None)
 
         stdout = StringIO()
         Command(stdout=stdout).handle()
 
         with self.assertRaises(Poll.DoesNotExist):
             expired_poll.refresh_from_db()
```

### Comparing `jawanndenn-2.5.0/jawanndenn/markup.py` & `jawanndenn-2.6.0/jawanndenn/markup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,19 +5,15 @@
     ('**', '<strong>', '</strong>'),
     ('*', '<em>', '</em>'),
     ('__', '<strong>', '</strong>'),
     ('_', '<em>', '</em>'),
     ('`', '<tt>', '</tt>'),
 )
 
-_CLOSING_OF = {
-        prefix: closing
-        for prefix, _, closing
-        in _REPLACEMENTS_IN_ORDER
-}
+_CLOSING_OF = {prefix: closing for prefix, _, closing in _REPLACEMENTS_IN_ORDER}
 
 
 def safe_html(text):
     if not isinstance(text, str):
         raise ValueError('Not a string: %s' % text)
 
     # KEEP IN SYNC with javascript client side!
```

### Comparing `jawanndenn-2.5.0/jawanndenn/middleware.py` & `jawanndenn-2.6.0/jawanndenn/middleware.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,34 +15,36 @@
     May raise exception _XForwardedForHeaderAbsentException .
     """
     try:
         value = request.META['HTTP_X_FORWARDED_FOR']
     except KeyError:
         raise _XForwardedForHeaderAbsentException
 
-    if ', ' in value:
-        return value.split(', ')[-1]
-
-    return value
+    # NOTE: This assumes that the outermost trusted
+    #       reverse proxy is resetting header X-Forwarded-For
+    #       rather than appending to an attacker controlled
+    #       value from the client request headers.  Else
+    #       we would need to use the <n>-rightmost value
+    #       instead, where <n> is the number of trusted
+    #       reverse proxies in front of the application.
+    return value.split(',')[0].strip()
 
 
 def set_remote_addr_to_x_forwarded_for(get_response):
     """
     Allow use of rate limiting key "ip" and "user_or_ip"
     (that looks at header REMOTE_ADDR) from behind a reverse proxy.
 
     For more details:
     https://django-ratelimit.readthedocs.io/en/latest/security.html#middleware
     """
 
     @wraps(get_response)
     def process_request(request):
         try:
-            request.META['REMOTE_ADDR'] = (
-                _extract_ip_from_x_forwarded_for_header(request)
-            )
+            request.META['REMOTE_ADDR'] = (_extract_ip_from_x_forwarded_for_header(request))
         except _XForwardedForHeaderAbsentException:
             pass
 
         return get_response(request)
 
     return process_request
```

### Comparing `jawanndenn-2.5.0/jawanndenn/migrations/0001_initial.py` & `jawanndenn-2.6.0/jawanndenn/migrations/0001_initial.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,67 +7,104 @@
 import jawanndenn.models
 
 
 class Migration(migrations.Migration):
 
     initial = True
 
-    dependencies = [
-    ]
+    dependencies = []
 
     operations = [
         migrations.CreateModel(
             name='Poll',
             fields=[
-                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('created', django_extensions.db.fields.CreationDateTimeField(auto_now_add=True, verbose_name='created')),
-                ('modified', django_extensions.db.fields.ModificationDateTimeField(auto_now=True, verbose_name='modified')),
-                ('slug', models.CharField(default=jawanndenn.models._get_random_sha256, max_length=64, unique=True)),
+                ('id',
+                 models.AutoField(auto_created=True,
+                                  primary_key=True,
+                                  serialize=False,
+                                  verbose_name='ID')),
+                ('created',
+                 django_extensions.db.fields.CreationDateTimeField(auto_now_add=True,
+                                                                   verbose_name='created')),
+                ('modified',
+                 django_extensions.db.fields.ModificationDateTimeField(auto_now=True,
+                                                                       verbose_name='modified')),
+                ('slug',
+                 models.CharField(default=jawanndenn.models._get_random_sha256,
+                                  max_length=64,
+                                  unique=True)),
                 ('title', models.CharField(max_length=255)),
                 ('equal_width', models.BooleanField(default=False)),
             ],
             options={
                 'ordering': ('-modified', '-created'),
                 'get_latest_by': 'modified',
                 'abstract': False,
             },
         ),
         migrations.CreateModel(
             name='PollOption',
             fields=[
-                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('id',
+                 models.AutoField(auto_created=True,
+                                  primary_key=True,
+                                  serialize=False,
+                                  verbose_name='ID')),
                 ('position', models.PositiveSmallIntegerField()),
                 ('name', models.CharField(max_length=255)),
-                ('poll', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='options', to='jawanndenn.Poll')),
+                ('poll',
+                 models.ForeignKey(on_delete=django.db.models.deletion.CASCADE,
+                                   related_name='options',
+                                   to='jawanndenn.Poll')),
             ],
             options={
                 'unique_together': {('poll', 'position')},
             },
         ),
         migrations.CreateModel(
             name='Ballot',
             fields=[
-                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('created', django_extensions.db.fields.CreationDateTimeField(auto_now_add=True, verbose_name='created')),
-                ('modified', django_extensions.db.fields.ModificationDateTimeField(auto_now=True, verbose_name='modified')),
+                ('id',
+                 models.AutoField(auto_created=True,
+                                  primary_key=True,
+                                  serialize=False,
+                                  verbose_name='ID')),
+                ('created',
+                 django_extensions.db.fields.CreationDateTimeField(auto_now_add=True,
+                                                                   verbose_name='created')),
+                ('modified',
+                 django_extensions.db.fields.ModificationDateTimeField(auto_now=True,
+                                                                       verbose_name='modified')),
                 ('voter_name', models.CharField(max_length=255)),
-                ('poll', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='ballots', to='jawanndenn.Poll')),
+                ('poll',
+                 models.ForeignKey(on_delete=django.db.models.deletion.CASCADE,
+                                   related_name='ballots',
+                                   to='jawanndenn.Poll')),
             ],
             options={
                 'ordering': ('-modified', '-created'),
                 'get_latest_by': 'modified',
                 'abstract': False,
             },
         ),
         migrations.CreateModel(
             name='Vote',
             fields=[
-                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('id',
+                 models.AutoField(auto_created=True,
+                                  primary_key=True,
+                                  serialize=False,
+                                  verbose_name='ID')),
                 ('yes', models.BooleanField()),
-                ('ballot', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='votes', to='jawanndenn.Ballot')),
-                ('option', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='jawanndenn.PollOption')),
+                ('ballot',
+                 models.ForeignKey(on_delete=django.db.models.deletion.CASCADE,
+                                   related_name='votes',
+                                   to='jawanndenn.Ballot')),
+                ('option',
+                 models.ForeignKey(on_delete=django.db.models.deletion.CASCADE,
+                                   to='jawanndenn.PollOption')),
             ],
             options={
                 'unique_together': {('ballot', 'option')},
             },
         ),
     ]
```

### Comparing `jawanndenn-2.5.0/jawanndenn/models.py` & `jawanndenn-2.6.0/jawanndenn/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,48 +11,45 @@
 
 
 def _get_random_sha256():
     return hashlib.sha256(os.urandom(256 // 8)).hexdigest()
 
 
 class PollQuerySet(models.QuerySet):
+
     def expired(self):
         return self.filter(expires_at__lt=now())
 
 
 class Poll(TimeStampedModel):
-    slug = models.CharField(max_length=64, default=_get_random_sha256,
-                            unique=True)
+    slug = models.CharField(max_length=64, default=_get_random_sha256, unique=True)
     title = models.CharField(max_length=255)
     equal_width = models.BooleanField(default=False)
     expires_at = models.DateTimeField(null=True)
 
     objects = PollQuerySet.as_manager()
 
     def get_absolute_url(self):
         return reverse('poll-detail', args=[self.slug])
 
 
 class PollOption(models.Model):
-    poll = models.ForeignKey(Poll, on_delete=models.CASCADE,
-                             related_name='options')
+    poll = models.ForeignKey(Poll, on_delete=models.CASCADE, related_name='options')
     position = models.PositiveSmallIntegerField()  # starting at 0
     name = models.CharField(max_length=255)
 
     class Meta:
         unique_together = ('poll', 'position')
 
 
 class Ballot(TimeStampedModel):
-    poll = models.ForeignKey(Poll, on_delete=models.CASCADE,
-                             related_name='ballots')
+    poll = models.ForeignKey(Poll, on_delete=models.CASCADE, related_name='ballots')
     voter_name = models.CharField(max_length=255)
 
 
 class Vote(models.Model):
-    ballot = models.ForeignKey(Ballot, related_name='votes',
-                               on_delete=models.CASCADE)
+    ballot = models.ForeignKey(Ballot, related_name='votes', on_delete=models.CASCADE)
     option = models.ForeignKey(PollOption, on_delete=models.CASCADE)
     yes = models.BooleanField()
 
     class Meta:
         unique_together = ('ballot', 'option')
```

### Comparing `jawanndenn-2.5.0/jawanndenn/serializers.py` & `jawanndenn-2.6.0/jawanndenn/serializers.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,52 +1,53 @@
 # Copyright (C) 2019 Sebastian Pipping <sebastian@pipping.org>
 # Licensed under GNU Affero GPL v3 or later
 
 from dateutil.relativedelta import relativedelta
 from django.db import transaction
 from django.utils import timezone
-from rest_framework.fields import (BooleanField, CharField, ChoiceField,
-                                   ListField)
+from rest_framework.fields import BooleanField, CharField, ChoiceField, ListField
 from rest_framework.serializers import Serializer
 
 from jawanndenn.markup import safe_html
 from jawanndenn.models import Poll, PollOption
 
 
 class _PollLifetime:
     MONTH = 'month'
     WEEK = 'week'
     CHOICES = (MONTH, WEEK)
 
     @classmethod
     def to_relativedelta(cls, lifetime):
         return relativedelta(**({
-            cls.MONTH: {'months': 1},
-            cls.WEEK: {'days': 7},
+            cls.MONTH: {
+                'months': 1
+            },
+            cls.WEEK: {
+                'days': 7
+            },
         }[lifetime]))
 
 
 class PollConfigSerializer(Serializer):
     equal_width = BooleanField(default=False)
     title = CharField()
     options = ListField(child=CharField(), allow_empty=False)
-    lifetime = ChoiceField(choices=_PollLifetime.CHOICES,
-                           default=_PollLifetime.MONTH)
+    lifetime = ChoiceField(choices=_PollLifetime.CHOICES, default=_PollLifetime.MONTH)
 
     def create(self, validated_data):
         poll_expires_at = timezone.now() + _PollLifetime.to_relativedelta(
             validated_data['lifetime'])
         poll_equal_width = validated_data['equal_width']
         poll_title = safe_html(validated_data['title'])
-        poll_option_names = [safe_html(str(option_name))
-                             for option_name
-                             in validated_data['options']]
+        poll_option_names = [
+            safe_html(str(option_name)) for option_name in validated_data['options']
+        ]
 
         with transaction.atomic():
             poll = Poll.objects.create(title=poll_title,
                                        expires_at=poll_expires_at,
                                        equal_width=poll_equal_width)
             for i, option_name in enumerate(poll_option_names):
-                PollOption.objects.create(poll=poll, position=i,
-                                          name=option_name)
+                PollOption.objects.create(poll=poll, position=i, name=option_name)
 
             return poll
```

### Comparing `jawanndenn-2.5.0/jawanndenn/settings.py` & `jawanndenn-2.6.0/jawanndenn/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,39 +17,40 @@
 from django.utils.log import DEFAULT_LOGGING
 
 from jawanndenn import DEFAULT_MAX_POLLS, DEFAULT_MAX_VOTES_PER_POLL
 
 # Build paths inside the project like this: os.path.join(BASE_DIR, ...)
 BASE_DIR = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 
-
 # Quick-start development settings - unsuitable for production
 # See https://docs.djangoproject.com/en/2.2/howto/deployment/checklist/
 
 # SECURITY WARNING: keep the secret key used in production secret!
 SECRET_KEY = os.environ['JAWANNDENN_SECRET_KEY']
 
 # SECURITY WARNING: don't run with debug turned on in production!
 DEBUG = os.environ.get('JAWANNDENN_DEBUG', 'False') == 'True'
 
 _ALLOWED_HOSTS_DEFAULT = ','.join([
     '127.0.0.1',
     '0.0.0.0',
     'localhost',
 ])
-ALLOWED_HOSTS = (
-    os.environ.get('JAWANNDENN_ALLOWED_HOSTS') or _ALLOWED_HOSTS_DEFAULT
-).split(',')
+ALLOWED_HOSTS = (os.environ.get('JAWANNDENN_ALLOWED_HOSTS') or _ALLOWED_HOSTS_DEFAULT).split(',')
+CSRF_TRUSTED_ORIGINS = {
+    f'{scheme}://{host}'
+    for scheme in ('http', 'https')
+    for host in ALLOWED_HOSTS
+}
 
 SECURE_REFERRER_POLICY = 'origin'
 
 _USE_POSTGRES = 'JAWANNDENN_SQLITE_FILE' not in os.environ
 _USE_REDIS_CACHE = 'JAWANNDENN_REDIS_HOST' in os.environ
 
-
 # Application definition
 
 INSTALLED_APPS = [
     'django.contrib.admin',
     'django.contrib.auth',
     'django.contrib.contenttypes',
     'django.contrib.sessions',
@@ -57,15 +58,14 @@
     'django.contrib.staticfiles',
     'django_extensions',  # for management command "show_urls"
     'jawanndenn',
 ]
 
 MIDDLEWARE = [
     'jawanndenn.middleware.set_remote_addr_to_x_forwarded_for',
-
     'django.middleware.security.SecurityMiddleware',
     'django.contrib.sessions.middleware.SessionMiddleware',
     'django.middleware.common.CommonMiddleware',
     'django.middleware.csrf.CsrfViewMiddleware',
     'django.contrib.auth.middleware.AuthenticationMiddleware',
     'django.contrib.messages.middleware.MessageMiddleware',
     'django.middleware.clickjacking.XFrameOptionsMiddleware',
@@ -89,15 +89,14 @@
             ],
         },
     },
 ]
 
 WSGI_APPLICATION = 'jawanndenn.wsgi.application'
 
-
 # Database
 # https://docs.djangoproject.com/en/2.2/ref/settings/#databases
 
 if _USE_POSTGRES:
     DATABASES = {
         'default': {
             'ENGINE': 'django.db.backends.postgresql',
@@ -112,24 +111,22 @@
     DATABASES = {
         'default': {
             'ENGINE': 'django.db.backends.sqlite3',
             'NAME': os.environ['JAWANNDENN_SQLITE_FILE'],
         }
     }
 
-
 # Logging
 # https://docs.djangoproject.com/en/2.2/ref/settings/#std:setting-LOGGING
 
 LOGGING = copy.copy(DEFAULT_LOGGING)
 LOGGING['handlers']['console']['filters'].remove('require_debug_true')
 if not DEBUG:
     LOGGING['handlers']['console']['level'] = 'ERROR'
 
-
 # Password validation
 # https://docs.djangoproject.com/en/2.2/ref/settings/#auth-password-validators
 
 AUTH_PASSWORD_VALIDATORS = [
     {
         'NAME': 'django.contrib.auth.password_validation.UserAttributeSimilarityValidator',  # noqa: E501
     },
@@ -140,52 +137,47 @@
         'NAME': 'django.contrib.auth.password_validation.CommonPasswordValidator',  # noqa: E501
     },
     {
         'NAME': 'django.contrib.auth.password_validation.NumericPasswordValidator',  # noqa: E501
     },
 ]
 
-
 # Internationalization
 # https://docs.djangoproject.com/en/2.2/topics/i18n/
 
 LANGUAGE_CODE = 'en-us'
 
 TIME_ZONE = 'UTC'
 
 USE_I18N = True
 
 USE_L10N = True
 
 USE_TZ = True
 
-
 # Settings specific to jawanndenn
 
 JAWANNDENN_URL_PREFIX = os.environ.get('JAWANNDENN_URL_PREFIX', '').strip('/')
 
 if JAWANNDENN_URL_PREFIX != '':
     JAWANNDENN_URL_PREFIX = '/' + JAWANNDENN_URL_PREFIX
 
-JAWANNDENN_MAX_POLLS = int(os.environ.get(
-    'JAWANNDENN_MAX_POLLS', str(DEFAULT_MAX_POLLS)))
-JAWANNDENN_MAX_VOTES_PER_POLL = int(os.environ.get(
-    'JAWANNDENN_MAX_VOTES_PER_POLL', str(DEFAULT_MAX_VOTES_PER_POLL)))
-
+JAWANNDENN_MAX_POLLS = int(os.environ.get('JAWANNDENN_MAX_POLLS', str(DEFAULT_MAX_POLLS)))
+JAWANNDENN_MAX_VOTES_PER_POLL = int(
+    os.environ.get('JAWANNDENN_MAX_VOTES_PER_POLL', str(DEFAULT_MAX_VOTES_PER_POLL)))
 
 # Static files (CSS, JavaScript, Images)
 # https://docs.djangoproject.com/en/2.2/howto/static-files/
 
 STATIC_URL = JAWANNDENN_URL_PREFIX + '/static/'
 
 STATICFILES_DIRS = [
     os.path.join(BASE_DIR, 'jawanndenn', 'static'),
 ]
 
-
 # Rate limiting
 
 if _USE_REDIS_CACHE:
     RATELIMIT_USE_CACHE = 'ratelimit'
 
     _REDIS_URL = 'redis://{}:{}/1'.format(os.environ['JAWANNDENN_REDIS_HOST'],
                                           os.environ['JAWANNDENN_REDIS_PORT'])
@@ -195,15 +187,14 @@
         'BACKEND': 'django_redis.cache.RedisCache',
         'LOCATION': _REDIS_URL,
         'OPTIONS': {
             'SERIALIZER': 'django_redis.serializers.msgpack.MSGPackSerializer',
         },
     }
 
-
 # Sentry integration
 
 _SENTRY_DSN = os.environ.get('JAWANNDENN_SENTRY_DSN')
 
 if _SENTRY_DSN:
     import sentry_sdk
     from sentry_sdk.integrations.django import DjangoIntegration
```

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/github-buttons-4.0.1/LICENSE.md` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/github-buttons-4.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/github-buttons-4.0.1/docs/github-btn.html` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/github-buttons-4.0.1/docs/github-btn.html`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/jquery-3.5.1/LICENSE.txt` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/jquery-3.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/jquery-3.5.1/jquery-3.5.1.min.js` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/jquery-3.5.1/jquery-3.5.1.min.js`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/jquery-3.5.1/jquery-3.5.1.min.map` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/jquery-3.5.1/jquery-3.5.1.min.map`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/materialize-1.0.0/LICENSE` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/materialize-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/materialize-1.0.0/css/materialize.css` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/materialize-1.0.0/css/materialize.css`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/materialize-1.0.0/css/materialize.min.css` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/materialize-1.0.0/css/materialize.min.css`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/materialize-1.0.0/js/materialize.js` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/materialize-1.0.0/js/materialize.js`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/materialize-1.0.0/js/materialize.min.js` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/materialize-1.0.0/js/materialize.min.js`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/noty-2.4.1/LICENSE.txt` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/noty-2.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/noty-2.4.1/js/noty/packaged/jquery.noty.packaged.min.js` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/noty-2.4.1/js/noty/packaged/jquery.noty.packaged.min.js`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/COPYING` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/COPYING`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/css/roboto.css` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/css/roboto.css`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-100.eot` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-100.eot`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-100.svg` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-100.svg`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-100.ttf` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-100.ttf`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-100.woff` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-100.woff`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-100.woff2` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-100.woff2`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-100italic.eot` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-100italic.eot`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-100italic.svg` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-100italic.svg`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-100italic.ttf` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-100italic.ttf`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-100italic.woff` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-100italic.woff`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-100italic.woff2` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-100italic.woff2`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-300.eot` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-300.eot`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-300.svg` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-300.svg`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-300.ttf` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-300.ttf`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-300.woff` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-300.woff`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-300.woff2` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-300.woff2`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-300italic.eot` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-300italic.eot`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-300italic.svg` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-300italic.svg`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-300italic.ttf` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-300italic.ttf`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-300italic.woff` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-300italic.woff`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-300italic.woff2` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-300italic.woff2`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-500.eot` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-500.eot`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-500.svg` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-500.svg`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-500.ttf` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-500.ttf`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-500.woff` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-500.woff`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-500.woff2` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-500.woff2`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-500italic.eot` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-500italic.eot`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-500italic.svg` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-500italic.svg`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-500italic.ttf` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-500italic.ttf`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-500italic.woff` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-500italic.woff`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-500italic.woff2` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-500italic.woff2`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-700.eot` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-700.eot`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-700.svg` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-700.svg`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-700.ttf` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-700.ttf`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-700.woff` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-700.woff`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-700.woff2` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-700.woff2`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-700italic.eot` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-700italic.eot`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-700italic.svg` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-700italic.svg`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-700italic.ttf` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-700italic.ttf`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-700italic.woff` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-700italic.woff`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-700italic.woff2` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-700italic.woff2`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-900.eot` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-900.eot`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-900.svg` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-900.svg`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-900.ttf` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-900.ttf`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-900.woff` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-900.woff`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-900.woff2` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-900.woff2`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-900italic.eot` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-900italic.eot`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-900italic.svg` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-900italic.svg`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-900italic.ttf` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-900italic.ttf`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-900italic.woff` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-900italic.woff`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-900italic.woff2` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-900italic.woff2`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-italic.eot` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-italic.eot`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-italic.svg` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-italic.svg`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-italic.ttf` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-italic.ttf`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-italic.woff` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-italic.woff`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-italic.woff2` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-italic.woff2`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-regular.eot` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-regular.eot`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-regular.svg` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-regular.svg`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-regular.ttf` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-regular.ttf`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-regular.woff` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-regular.woff`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-regular.woff2` & `jawanndenn-2.6.0/jawanndenn/static/3rdparty/roboto-20/fonts/roboto-v20-vietnamese_latin-ext_latin_greek-ext_greek_cyrillic-ext_cyrillic-regular.woff2`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/css/style.css` & `jawanndenn-2.6.0/jawanndenn/static/css/style.css`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/html/footer.htm` & `jawanndenn-2.6.0/jawanndenn/static/html/footer.htm`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/html/poll.htm` & `jawanndenn-2.6.0/jawanndenn/static/html/poll.htm`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/html/setup.htm` & `jawanndenn-2.6.0/jawanndenn/static/html/setup.htm`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/js/html.js` & `jawanndenn-2.6.0/jawanndenn/static/js/html.js`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/js/poll.js` & `jawanndenn-2.6.0/jawanndenn/static/js/poll.js`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/static/js/setup.js` & `jawanndenn-2.6.0/jawanndenn/static/js/setup.js`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn/tests/factories.py` & `jawanndenn-2.6.0/jawanndenn/tests/factories.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,35 +4,39 @@
 from factory import Sequence, SubFactory
 from factory.django import DjangoModelFactory
 
 from jawanndenn.models import Ballot, Poll, PollOption, Vote
 
 
 class PollFactory(DjangoModelFactory):
+
     class Meta:
         model = Poll
 
     title = Sequence(lambda n: f"Title {n}")
 
 
 class PollOptionFactory(DjangoModelFactory):
+
     class Meta:
         model = PollOption
 
     poll = SubFactory(PollFactory)
     position = Sequence(int)
     name = Sequence(lambda n: f"Option {n}")
 
 
 class BallotFactory(DjangoModelFactory):
+
     class Meta:
         model = Ballot
 
     poll = SubFactory(PollFactory)
     voter_name = Sequence(lambda n: f"User {n}")
 
 
 class VoteFactory(DjangoModelFactory):
+
     class Meta:
         model = Vote
 
     option = SubFactory(PollOptionFactory)
```

### Comparing `jawanndenn-2.5.0/jawanndenn/tests/test_markup.py` & `jawanndenn-2.6.0/jawanndenn/tests/test_markup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,57 +3,37 @@
 
 from unittest import TestCase
 
 from jawanndenn.markup import safe_html
 
 
 class SafeHtmlTest(TestCase):
+
     def test_vanilla(self):
-        self.assertEqual(safe_html(
-                'text'),
-                'text')
+        self.assertEqual(safe_html('text'), 'text')
 
     def test_html(self):
-        self.assertEqual(safe_html(
-                '<b>&nbsp;</b>'),
-                '&lt;b&gt;&amp;nbsp;&lt;/b&gt;')
+        self.assertEqual(safe_html('<b>&nbsp;</b>'), '&lt;b&gt;&amp;nbsp;&lt;/b&gt;')
 
     def test_bold(self):
-        self.assertEqual(safe_html(
-                '**text**'),
-                '<strong>text</strong>')
-        self.assertEqual(safe_html(
-                '__text__'),
-                '<strong>text</strong>')
+        self.assertEqual(safe_html('**text**'), '<strong>text</strong>')
+        self.assertEqual(safe_html('__text__'), '<strong>text</strong>')
 
     def test_italic(self):
-        self.assertEqual(safe_html(
-                '*text*'),
-                '<em>text</em>')
-        self.assertEqual(safe_html(
-                '_text_'),
-                '<em>text</em>')
+        self.assertEqual(safe_html('*text*'), '<em>text</em>')
+        self.assertEqual(safe_html('_text_'), '<em>text</em>')
 
     def test_monospace(self):
-        self.assertEqual(safe_html(
-                '`text`'),
-                '<tt>text</tt>')
+        self.assertEqual(safe_html('`text`'), '<tt>text</tt>')
 
     def test_combined(self):
-        self.assertEqual(safe_html(
-                '`__*text*__`'),
-                '<tt><strong><em>text</em></strong></tt>')
-        self.assertEqual(safe_html(
-                '`**_text_**`'),
-                '<tt><strong><em>text</em></strong></tt>')
-        self.assertEqual(safe_html(
-                '_*text*_'),
-                '<em><em>text</em></em>')
+        self.assertEqual(safe_html('`__*text*__`'), '<tt><strong><em>text</em></strong></tt>')
+        self.assertEqual(safe_html('`**_text_**`'), '<tt><strong><em>text</em></strong></tt>')
+        self.assertEqual(safe_html('_*text*_'), '<em><em>text</em></em>')
 
     def test_bad_nesting(self):
-        self.assertEqual(safe_html(
-                '*__text*__'),
-                '<em><strong>text<em><strong></strong></em></strong></em>')
+        self.assertEqual(safe_html('*__text*__'),
+                         '<em><strong>text<em><strong></strong></em></strong></em>')
 
     def test_non_string(self):
         with self.assertRaises(ValueError):
             safe_html(123)
```

### Comparing `jawanndenn-2.5.0/jawanndenn/tests/test_views.py` & `jawanndenn-2.6.0/jawanndenn/tests/test_views.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,26 +9,28 @@
 from django.test import TestCase
 from django.urls import reverse
 from django.utils import timezone
 from django.utils.timezone import now
 from parameterized import parameterized
 
 from jawanndenn.models import Ballot, Poll
-from jawanndenn.tests.factories import (BallotFactory, PollFactory,
-                                        PollOptionFactory, VoteFactory)
+from jawanndenn.tests.factories import BallotFactory, PollFactory, PollOptionFactory, VoteFactory
+from jawanndenn.tests.helpers import RELEASE_SAVEPOINT, SAVEPOINT, SELECT
 
 
 class AdminLoginPageTest(TestCase):
+
     def test(self):
         url = reverse('admin:index')
         response = self.client.get(url, follow=True)
         self.assertContains(response, 'Django administration')
 
 
 class IndexGetViewTest(TestCase):
+
     def test(self):
         url = reverse('frontpage')
 
         response = self.client.get(url)
 
         self.assertContains(response, 'Create a new poll')
 
@@ -41,23 +43,21 @@
             'config': 'not JSON',
         }
         before_creation = timezone.now()
 
         response = self.client.post(self.url, data)
 
         self.assertEqual(response.status_code, HTTPStatus.BAD_REQUEST)
-        self.assertFalse(Poll.objects.filter(created__gte=before_creation)
-                         .exists())
+        self.assertFalse(Poll.objects.filter(created__gte=before_creation).exists())
 
     @parameterized.expand([
         ('month', datetime.date(2020, 9, 16)),
         ('week', datetime.date(2020, 8, 23)),
     ])
-    def test_lifetime_sets_expires_at_properly(self, lifetime,
-                                               expected_expiry_date):
+    def test_lifetime_sets_expires_at_properly(self, lifetime, expected_expiry_date):
         created_at = now().replace(2020, 8, 16)
         data = {
             'config': json.dumps({
                 'lifetime': lifetime,
                 'options': ['option1', 'option2'],
                 'title': 'title1',
             }),
@@ -84,65 +84,67 @@
         }
         before_creation = timezone.now()
 
         response = self.client.post(self.url, data)
 
         poll = Poll.objects.get(created__gte=before_creation)
         self.assertEqual(poll.equal_width, poll_equal_width)
-        self.assertEqual(list(poll.options
-                              .order_by('position')
-                              .values_list('name', flat=True)),
+        self.assertEqual(list(poll.options.order_by('position').values_list('name', flat=True)),
                          poll_option_names)
         self.assertEqual(poll.title, poll_title)
 
         self.assertEqual(response.status_code, HTTPStatus.FOUND)
         self.assertEqual(response.url, poll.get_absolute_url())
 
 
 class PollDataGetViewTest(TestCase):
+
     @classmethod
     def setUpTestData(cls):
         super().setUpTestData()
         cls.poll = PollFactory(equal_width=True)
-        cls.ballot = BallotFactory(poll=cls.poll)
-        cls.votes = [
-            VoteFactory(ballot=cls.ballot, option__poll=cls.poll,
-                        yes=(position == 0))
-            for position
-            in range(2)
-        ]
+        cls.poll_options = [PollOptionFactory(poll=cls.poll) for _ in range(3)]
+        cls.votes_of_ballot = {}
+
+        for user_index in range(2):
+            ballot = BallotFactory(poll=cls.poll)
+            for option_index, option in enumerate(cls.poll_options):
+                vote = VoteFactory(ballot=ballot, option=option, yes=(option_index == user_index))
+                cls.votes_of_ballot.setdefault(ballot, []).append(vote)
 
     def test_poll_exists(self):
         url = reverse('poll-data', args=[self.poll.slug])
         expected_data = {
             'config': {
                 'equal_width': self.poll.equal_width,
-                'options': [v.option.name for v in self.votes],
+                'options': [option.name for option in self.poll_options],
                 'title': self.poll.title,
             },
-            'votes': [
-                [self.ballot.voter_name, [v.yes for v in self.votes]],
-            ],
+            'votes': [[ballot.voter_name, [v.yes for v in votes]]
+                      for ballot, votes in self.votes_of_ballot.items()],
         }
 
-        response = self.client.get(url)
+        with self.assertNumQueries(SAVEPOINT + SELECT("poll") + SELECT("poll option names")
+                                   + SELECT("votes + ballots") + RELEASE_SAVEPOINT):
+            response = self.client.get(url)
 
         actual_data = json.loads(response.content)
         self.assertEqual(actual_data, expected_data)
         self.assertEqual(response.status_code, HTTPStatus.OK)
 
     def test_poll_does_not_exist(self):
         url = reverse('poll-data', args=['whatever'])
 
         response = self.client.get(url)
 
         self.assertEqual(response.status_code, HTTPStatus.NOT_FOUND)
 
 
 class PollGetViewTest(TestCase):
+
     @classmethod
     def setUpTestData(cls):
         super().setUpTestData()
         cls.poll = PollFactory()
 
     def test_poll_exists(self):
         url = self.poll.get_absolute_url()
@@ -156,14 +158,15 @@
 
         response = self.client.get(url)
 
         self.assertEqual(response.status_code, HTTPStatus.NOT_FOUND)
 
 
 class VotePostViewTest(TestCase):
+
     @classmethod
     def setUpTestData(cls):
         super().setUpTestData()
         cls.poll = PollFactory()
         for _ in range(2):
             PollOptionFactory(poll=cls.poll)
 
@@ -175,38 +178,38 @@
             'option0': 'on',
             'option1': 'off',
         }
 
         response = self.client.post(url, data)
 
         ballot = Ballot.objects.get(poll=self.poll)
-        self.assertEqual(list(ballot.votes
-                              .order_by('option__position')
-                              .values_list('yes', flat=True)), [True, False])
+        self.assertEqual(
+            list(ballot.votes.order_by('option__position').values_list('yes', flat=True)),
+            [True, False])
 
         self.assertEqual(response.status_code, HTTPStatus.FOUND)
         self.assertEqual(response.url, self.poll.get_absolute_url())
 
     def test_poll_does_not_exist(self):
         url = reverse('vote', args=['no_such_poll'])
         data = {}
 
         response = self.client.post(url, data)
 
         self.assertEqual(response.status_code, HTTPStatus.NOT_FOUND)
 
 
 class ServeUsingFindersTest(TestCase):
+
     @parameterized.expand([
         # Our app, some arbitrary asset
         ('jawanndenn', 'js/html.js', 'DENY'),
 
         # Our app, asset used in <iframe>
-        ('jawanndenn', '3rdparty/github-buttons-4.0.1/docs/github-btn.html',
-         'sameorigin'),
+        ('jawanndenn', '3rdparty/github-buttons-4.0.1/docs/github-btn.html', 'sameorigin'),
 
         # Arbitrary asset of arbitary other app
         ('django.contrib.admin', 'admin/css/responsive.css', 'DENY'),
     ])
     def test(self, _app, path, expected_x_frame_options):
         url = reverse('static', kwargs={'path': path})
```

### Comparing `jawanndenn-2.5.0/jawanndenn/urls.py` & `jawanndenn-2.6.0/jawanndenn/urls.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,35 +6,34 @@
 
 from django.conf import settings
 from django.contrib import admin
 from django.contrib.staticfiles.views import serve
 from django.http import HttpResponse
 from django.urls import include, path, re_path
 from django.views.defaults import permission_denied
-from ratelimit.decorators import ratelimit
-from ratelimit.exceptions import Ratelimited
+from django_ratelimit.decorators import ratelimit
+from django_ratelimit.exceptions import Ratelimited
 
-from .views import (index_get_view, poll_data_get_view, poll_get_view,
-                    poll_post_view, vote_post_view)
+from .views import (index_get_view, poll_data_get_view, poll_get_view, poll_post_view,
+                    vote_post_view)
 
 
 class _HttpResponseTooManyRequests(HttpResponse):
     status_code = HTTPStatus.TOO_MANY_REQUESTS
 
     def __init__(self):
         super().__init__(f'<h1>{self.status_code} Too Many Requests</h1>',
                          content_type='text/html')
 
 
 def _serve_with_headers_fixed(request, path, insecure=False, **kwargs):
     response = serve(request, path, insecure=insecure, **kwargs)
 
     # Allow loading of github-btn.html in an <iframe>
-    if (path.startswith('3rdparty/github-buttons-')
-            and path.endswith('/docs/github-btn.html')):
+    if (path.startswith('3rdparty/github-buttons-') and path.endswith('/docs/github-btn.html')):
         response['X-Frame-Options'] = 'sameorigin'
 
     return response
 
 
 def _staticfiles_urlpatterns(prefix=None, name='static'):
     '''
@@ -45,15 +44,16 @@
     Also, it uses view _serve_with_headers_fixed above rather than stock
     django.contrib.staticfiles.views.serve to serve files.
     '''
     if prefix is None:
         prefix = settings.STATIC_URL
     return [
         re_path(r'^%s(?P<path>.*)$' % re.escape(prefix.lstrip('/')),
-                _serve_with_headers_fixed, kwargs={
+                _serve_with_headers_fixed,
+                kwargs={
                     'insecure': not settings.DEBUG,
                     'show_indexes': settings.DEBUG,
                 },
                 name=name),
     ]
 
 
@@ -74,39 +74,36 @@
 
     for url_pattern in urlconf_module:
         _decorate_view_of_url_pattern(decorator, url_pattern)
 
     return view
 
 
-_limit_read_access = ratelimit(key='user_or_ip', rate='180/m', block=True)
+_limit_read_access = ratelimit(key='user_or_ip', rate='180/m')
 
-_limit_write_access = ratelimit(key='user_or_ip', rate='30/m', block=True)
+_limit_write_access = ratelimit(key='user_or_ip', rate='30/m')
 
 _app_urlpatterns = [
     path('', _limit_read_access(index_get_view), name='frontpage'),
     path('create', _limit_write_access(poll_post_view), name='poll-creation'),
-    path('data/<poll_id>',
-         _limit_read_access(poll_data_get_view), name='poll-data'),
-    path('poll/<poll_id>',
-         _limit_read_access(poll_get_view), name='poll-detail'),
+    path('data/<poll_id>', _limit_read_access(poll_data_get_view), name='poll-data'),
+    path('poll/<poll_id>', _limit_read_access(poll_get_view), name='poll-detail'),
     path('vote/<poll_id>', _limit_write_access(vote_post_view), name='vote'),
-
-    path('admin/', _decorate_view_triple(_limit_write_access,
-                                         admin.site.urls)),
+    path('admin/', _decorate_view_triple(_limit_write_access, admin.site.urls)),
 ]
 
-if settings.JAWANNDENN_URL_PREFIX:
+_url_prefix = getattr(settings, 'JAWANNDENN_URL_PREFIX', None)
+if _url_prefix:
     from django.views.generic.base import RedirectView
     urlpatterns = [
-        path('', _limit_read_access(
-            RedirectView.as_view(url=settings.JAWANNDENN_URL_PREFIX + '/'))),
-        path(settings.JAWANNDENN_URL_PREFIX.strip('/') + '/',
-             include(_app_urlpatterns)),
+        path('', _limit_read_access(RedirectView.as_view(url=_url_prefix + '/'))),
+        path(_url_prefix.strip('/') + '/', include(_app_urlpatterns)),
     ]
 else:
     urlpatterns = _app_urlpatterns
 
-urlpatterns += [_decorate_view_of_url_pattern(_limit_read_access, url_pattern)
-                for url_pattern in _staticfiles_urlpatterns()]
+urlpatterns += [
+    _decorate_view_of_url_pattern(_limit_read_access, url_pattern)
+    for url_pattern in _staticfiles_urlpatterns()
+]
 
 handler403 = _permission_denied_or_too_many_requests
```

### Comparing `jawanndenn-2.5.0/jawanndenn/views.py` & `jawanndenn-2.6.0/jawanndenn/views.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,42 +2,44 @@
 # Licensed under GNU Affero GPL v3 or later
 
 from functools import wraps
 
 import rapidjson as json  # lgtm [py/import-and-import-from]
 from django.conf import settings
 from django.db import transaction
-from django.http import (HttpResponseBadRequest, HttpResponseNotFound,
-                         JsonResponse)
+from django.http import HttpResponseBadRequest, HttpResponseNotFound, JsonResponse
 from django.shortcuts import redirect
 from django.template.response import TemplateResponse
 from django.views.decorators.http import require_GET, require_POST
 from django.views.defaults import bad_request
 from rapidjson import JSONDecodeError
 from rest_framework.exceptions import ValidationError
 
+from jawanndenn import DEFAULT_MAX_POLLS, DEFAULT_MAX_VOTES_PER_POLL
 from jawanndenn.markup import safe_html
 from jawanndenn.models import Ballot, Poll, Vote
 from jawanndenn.serializers import PollConfigSerializer
 
 
 def _except_poll_does_not_exist(wrappee):
     """Decorator that turns Poll.DoesNotExist into 404 Not Found"""
+
     @wraps(wrappee)
     def wrapper(*args, **kwargs):
         try:
             return wrappee(*args, **kwargs)
         except Poll.DoesNotExist:
             return HttpResponseNotFound('No such poll')
 
     return wrapper
 
 
 def _except_validation_error(wrappee):
     """Decorator that turns ValidationError into 400 Bad Request"""
+
     @wraps(wrappee)
     def wrapper(request, *args, **kwargs):
         try:
             return wrappee(request, *args, **kwargs)
         except ValidationError as exception:
             return bad_request(request, exception)
 
@@ -58,41 +60,50 @@
     except JSONDecodeError:
         raise ValidationError('Poll configuration is not well-formed JSON.')
 
     serializer = PollConfigSerializer(data=config)
     serializer.is_valid(raise_exception=True)
 
     with transaction.atomic():
-        if Poll.objects.count() >= settings.JAWANNDENN_MAX_POLLS:
-            return HttpResponseBadRequest(
-                f'Maximum number of {settings.JAWANNDENN_MAX_POLLS} polls '
-                'reached, please contact the administrator.')
+        max_polls = getattr(settings, 'JAWANNDENN_MAX_POLLS', DEFAULT_MAX_POLLS)
+        if Poll.objects.count() >= max_polls:
+            return HttpResponseBadRequest(f'Maximum number of {max_polls} polls '
+                                          'reached, please contact the administrator.')
 
         poll = serializer.save()
 
     return redirect(poll)
 
 
 @require_GET
 @_except_poll_does_not_exist
 def poll_data_get_view(request, poll_id):
     with transaction.atomic():
         poll = Poll.objects.get(slug=poll_id)
         poll_config = {
             'equal_width': poll.equal_width,
             'title': poll.title,
-            'options': list(poll.options.order_by('position')
-                            .values_list('name', flat=True)),
+            'options': list(poll.options.order_by('position').values_list('name', flat=True)),
         }
-        votes = [
-            [ballot.voter_name, [vote.yes for vote
-                                 in ballot.votes.order_by('option__position')]]
-            for ballot
-            in poll.ballots.order_by('created', 'id')
-        ]
+
+        votes = []
+        ballot = None
+        ballot_votes = []
+
+        for vote in (Vote.objects.filter(ballot__poll=poll).select_related('ballot').order_by(
+                'ballot__created', 'ballot__id', 'option__position')):
+            if vote.ballot != ballot:
+                if ballot is not None:
+                    votes.append([ballot.voter_name, ballot_votes])
+                ballot = vote.ballot
+                ballot_votes = []
+            ballot_votes.append(vote.yes)
+
+        if ballot is not None:
+            votes.append([ballot.voter_name, ballot_votes])
 
     data = {
         'config': poll_config,
         'votes': votes,
     }
 
     return JsonResponse(data)
@@ -108,25 +119,24 @@
 
 @require_POST
 @_except_poll_does_not_exist
 def vote_post_view(request, poll_id):
     with transaction.atomic():
         poll = Poll.objects.get(slug=poll_id)
 
-        if poll.ballots.count() >= settings.JAWANNDENN_MAX_VOTES_PER_POLL:
-            return HttpResponseBadRequest(
-                f'Maximum number of {settings.JAWANNDENN_MAX_VOTES_PER_POLL} '
-                'votes reached for this poll'
-                ', please contact the administrator.')
+        max_votes_per_poll = getattr(settings, 'JAWANNDENN_MAX_VOTES_PER_POLL',
+                                     DEFAULT_MAX_VOTES_PER_POLL)
+        if poll.ballots.count() >= max_votes_per_poll:
+            return HttpResponseBadRequest(f'Maximum number of {max_votes_per_poll} '
+                                          'votes reached for this poll'
+                                          ', please contact the administrator.')
 
         voter_name = safe_html(request.POST.get('voterName'))
         votes = [
-            request.POST.get(f'option{i}', 'off') == 'on'
-            for i
-            in range(poll.options.count())
+            request.POST.get(f'option{i}', 'off') == 'on' for i in range(poll.options.count())
         ]
 
         ballot = Ballot.objects.create(poll=poll, voter_name=voter_name)
         for option, vote in zip(poll.options.order_by('position'), votes):
             Vote.objects.create(ballot=ballot, option=option, yes=vote)
 
     return redirect(poll)
```

### Comparing `jawanndenn-2.5.0/jawanndenn-setup.png` & `jawanndenn-2.6.0/jawanndenn-setup.png`

 * *Files identical despite different names*

### Comparing `jawanndenn-2.5.0/jawanndenn.egg-info/PKG-INFO` & `jawanndenn-2.6.0/jawanndenn.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: jawanndenn
-Version: 2.5.0
+Version: 2.6.0
 Summary: Libre alternative to Doodle
 Home-page: https://github.com/hartwork/jawanndenn
 Author: Sebastian Pipping
 Author-email: sebastian@pipping.org
 License: AGPLv3+
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python
@@ -20,14 +19,17 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Topic :: Office/Business :: Scheduling
 Requires-Python: >=3.6
 Provides-Extra: tests
 
+.. image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit
+   :target: https://github.com/pre-commit/pre-commit
+   :alt: pre-commit
 .. image:: https://github.com/hartwork/jawanndenn/workflows/Build%20and%20test%20using%20Docker/badge.svg
     :target: https://github.com/hartwork/jawanndenn/actions
 
 
 What is jawanndenn?
 ===================
 
@@ -115,20 +117,132 @@
 ::
 
     JAWANNDENN_POSTGRES_NAME=jawanndenn
     JAWANNDENN_POSTGRES_USER=jawanndenn
     JAWANNDENN_POSTGRES_PASSWORD=dEb2PIcinemA8poH
     JAWANNDENN_SECRET_KEY=606ea88f183a27919d5c27ec7f948906d23fdd7821684eb59e8bcf7377e3853b
 
-Make sure to use your own values!
+Make sure to **adjust these values** after copy and paste!
 
 You can then build and run a docker image using ``docker-compose up --build``.
 
-PostgreSQL data is saved to ``~/.jawanndenn-docker-pgdata/`` on the host system.
 The app is served on ``localhost:54080``.
+PostgreSQL data is saved to ``~/.jawanndenn-docker-pgdata/`` on the host system.
+There is also an instance of Redis used for cross-process rate limiting,
+and a "cron" housekeeping container that will go delete polls that have exceeded their
+configured lifetime, every 60 minutes.
+
+(If you need a low-maintenance SSL reverse proxy in front of jawanndenn,
+`docker-ssl-reverse-proxy <https://github.com/hartwork/docker-ssl-reverse-proxy>`_
+could be of interest.)
+
+There is a few more environment variables that you could want to adjust in your environment.
+Altogether, there are these variables:
+
+
+Environment variables
+---------------------
+
+``DJANGO_SETTINGS_MODULE``
+~~~~~~~~~~~~~~~~~~~~~~~~~~
+Django settings module to use, leave as is, defaults to ``jawanndenn.settings``
+(see ``docker-compose.yml``)
+
+
+``JAWANNDENN_ALLOWED_HOSTS``
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+Hostnames to serve jawanndenn at, list separated by comma,
+is set to ``jawanndenn.de,www.jawanndenn.de`` on the main production server,
+defaults to ``127.0.0.1,0.0.0.0,localhost``
+(see ``jawanndenn/settings.py``)
+
+
+``JAWANNDENN_DEBUG``
+~~~~~~~~~~~~~~~~~~~~
+Debug mode, disabled for all values but ``True``, disabled by default,
+should never be enabled in production for security
+(see ``jawanndenn/settings.py``)
+
+
+``JAWANNDENN_MAX_POLLS``
+~~~~~~~~~~~~~~~~~~~~~~~~
+Maximum total number of polls to store, denial of service protection,
+defaults to ``1000``
+(see ``jawanndenn/settings.py`` and ``docker-compose.yml``)
+
+
+``JAWANNDENN_MAX_VOTES_PER_POLL``
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+Maximum total number of polls to store, denial of service protection,
+defaults to ``40``
+(see ``jawanndenn/settings.py``)
+
+
+``JAWANNDENN_POSTGRES_HOST``
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+Hostname of the PostgreSQL database to connect to; defaults to ``postgres``
+(see ``docker-compose.yml``)
+
+
+``JAWANNDENN_POSTGRES_NAME``
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+Database name of the PostgreSQL database to connect to;
+no default, always required
+
+
+``JAWANNDENN_POSTGRES_PASSWORD``
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+Password for log-in with the PostgreSQL database;
+no default, always required
+
+
+``JAWANNDENN_POSTGRES_PORT``
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+Port of the PostgreSQL database to connect to; defaults to ``5432``
+(see ``docker-compose.yml``)
+
+
+``JAWANNDENN_POSTGRES_USER``
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+Username for log-in with the PostgreSQL database;
+no default, always required
+
+
+``JAWANNDENN_REDIS_HOST``
+~~~~~~~~~~~~~~~~~~~~~~~~~
+Hostname of the Redis database to connect to; defaults to ``redis``
+(see ``docker-compose.yml``)
+
+
+``JAWANNDENN_REDIS_PORT``
+~~~~~~~~~~~~~~~~~~~~~~~~~
+Port of the Redis database to connect to; defaults to ``6379``
+(see ``docker-compose.yml``)
+
+
+``JAWANNDENN_SECRET_KEY``
+~~~~~~~~~~~~~~~~~~~~~~~~~
+`Django secret key <https://docs.djangoproject.com/en/4.0/ref/settings/#secret-key>`_;
+should be long, generated, not used elsewhere; no default, always required
+
+
+``JAWANNDENN_SENTRY_DSN``
+~~~~~~~~~~~~~~~~~~~~~~~~~
+`Data source name (DSN) <https://docs.sentry.io/product/sentry-basics/dsn-explainer/>`_
+for use with `Sentry <https://sentry.io/>`_, disabled/empty by default
+(see ``jawanndenn/settings.py``)
+
+
+``JAWANNDENN_URL_PREFIX``
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+Prefix string to insert into URLs rather after the domain name
+to help with hosting multiple apps under the same domain side by side;
+e.g. prefix ``prefix123`` will result in URLs like ``https://<domain>/prefix123/poll/<id>``;
+empty by default
+(see ``jawanndenn/settings.py``)
 
 
 Command line usage
 ==================
 
 When installed, invocation is as simple as
 
@@ -224,14 +338,15 @@
    -  `Framadata`_ (`Sources`_, ex. `OpenSondage`_, ex. `STUdS`_)
    -  `Nextcloud Polls`_
    -  `Noodle`_
    -  `Nuages`_
    -  `Pleft`_
    -  `Rallly`_
    -  `RDVz`_
+   -  `sowhenthen`_
 
 -  Keep things simple, usable, maintainable
 -  Support invocation from the command line, e.g. for spontaneous polls in a LAN
 -  Have security in mind
 
 Please check out the `list of upcoming features`_.
 
@@ -298,15 +413,14 @@
 .. _Foodle: https://foodl.org/
 .. _on GitHub: https://github.com/UNINETT/Foodle
 .. _DFN scheduler: https://terminplaner.dfn.de/
 .. _DFN Terminplaner+: https://terminplaner2.dfn.de/
 .. _Dudle: https://dudle.inf.tu-dresden.de/
 .. _Nuages: https://nuages.domainepublic.net/
 .. _RDVz: https://sourceforge.net/projects/rdvz/
+.. _sowhenthen: https://github.com/kiyutink/sowhenthen
 .. _Drupal Date picker formatter: http://alternativeto.net/software/date-picker-formatter-dudel-for-drupal/?license=opensource
 .. _Nextcloud Polls: https://github.com/nextcloud/polls
 .. _Noodle: https://github.com/kmerz/noodle
 .. _Rallly: https://github.com/lukevella/Rallly
 .. _list of upcoming features: https://github.com/hartwork/jawanndenn/issues/created_by/hartwork
 .. _@KordonDev: https://github.com/KordonDev
-
-
```

### Comparing `jawanndenn-2.5.0/jawanndenn.egg-info/SOURCES.txt` & `jawanndenn-2.6.0/jawanndenn.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 .dockerignore
+.flake8
 .gitignore
+.isort.cfg
 .pre-commit-config.yaml
+.style.yapf
 Dockerfile
 README.rst
 crontab
 docker-compose.yml
 docker-entrypoint.sh
 generate_whitelist_dockerignore_file.sh
 jawanndenn-setup.png
@@ -122,10 +125,11 @@
 jawanndenn/static/html/poll.htm
 jawanndenn/static/html/setup.htm
 jawanndenn/static/js/html.js
 jawanndenn/static/js/poll.js
 jawanndenn/static/js/setup.js
 jawanndenn/tests/__init__.py
 jawanndenn/tests/factories.py
+jawanndenn/tests/helpers.py
 jawanndenn/tests/test_markup.py
 jawanndenn/tests/test_middleware.py
 jawanndenn/tests/test_views.py
```

### Comparing `jawanndenn-2.5.0/manage.py` & `jawanndenn-2.6.0/manage.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,17 +5,15 @@
 
 
 def main():
     os.environ.setdefault('DJANGO_SETTINGS_MODULE', 'jawanndenn.settings')
     try:
         from django.core.management import execute_from_command_line
     except ImportError as exc:
-        raise ImportError(
-            "Couldn't import Django. Are you sure it's installed and "
-            "available on your PYTHONPATH environment variable? Did you "
-            "forget to activate a virtual environment?"
-        ) from exc
+        raise ImportError("Couldn't import Django. Are you sure it's installed and "
+                          "available on your PYTHONPATH environment variable? Did you "
+                          "forget to activate a virtual environment?") from exc
     execute_from_command_line(sys.argv)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `jawanndenn-2.5.0/setup.py` & `jawanndenn-2.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,48 +31,42 @@
             yield os.path.join(relative_root, '*')
 
 
 if __name__ == '__main__':
     setup(
         name=APP_NAME,
         version=VERSION_STR,
-
         license='AGPLv3+',
         description='Libre alternative to Doodle',
         long_description=_read('README.rst'),
-
         author='Sebastian Pipping',
         author_email='sebastian@pipping.org',
         url='https://github.com/hartwork/jawanndenn',
-
         python_requires='>=3.6',
         install_requires=[
             'django>=2.2.7',
             'django-extensions>=2.2.5',
-            'django-ratelimit>=2.0.0',
+            'django-ratelimit>=4.0.0',
             'djangorestframework>=3.11.0',
             'gunicorn>=20.0.4',
             'gunicorn-color>=0.1.0',
             'python-dateutil>=2.8.1',
             'python-rapidjson>=1.0',
         ],
         extras_require=_extras_require,
         tests_require=_tests_require,
-
         packages=find_packages(),
         package_data={
             APP_NAME: list(_collect_package_data(APP_NAME)),
         },
-
         entry_points={
             'console_scripts': [
                 f'{APP_NAME} = {APP_NAME}.__main__:main',
             ],
         },
-
         classifiers=[
             'Development Status :: 4 - Beta',
             'Framework :: Django',
             'Framework :: Django :: 2.2',
             'License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)',  # noqa: E501
             'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',  # noqa: E501
             'Programming Language :: JavaScript',
@@ -80,9 +74,8 @@
             'Programming Language :: Python :: 3',
             'Programming Language :: Python :: 3.6',
             'Programming Language :: Python :: 3.7',
             'Programming Language :: Python :: 3.8',
             'Programming Language :: Python :: 3 :: Only',
             'Topic :: Internet :: WWW/HTTP :: WSGI :: Application',
             'Topic :: Office/Business :: Scheduling',
-        ]
-    )
+        ])
```

