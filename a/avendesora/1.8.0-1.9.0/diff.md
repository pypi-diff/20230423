# Comparing `tmp/avendesora-1.8.0.tar.gz` & `tmp/avendesora-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/avendesora-1.8.0.tar", last modified: Thu Nov 23 17:23:14 2017, max compression
+gzip compressed data, was "dist/avendesora-1.9.0.tar", last modified: Tue Dec 26 02:26:38 2017, max compression
```

## Comparing `avendesora-1.8.0.tar` & `avendesora-1.9.0.tar`

### file list

```diff
@@ -1,107 +1,109 @@
-drwxr-xr-x   0 ken       (1000) officers   (501)        0 2017-11-23 17:23:14.000000 avendesora-1.8.0/
--rw-r--r--   0 ken       (1000) officers   (501)    29484 2017-11-23 16:59:19.000000 avendesora-1.8.0/README.rst
-drwxr-xr-x   0 ken       (1000) officers   (501)        0 2017-11-23 17:23:14.000000 avendesora-1.8.0/avendesora/
--rw-r--r--   0 ken       (1000) officers   (501)    30823 2017-11-21 19:23:23.000000 avendesora-1.8.0/avendesora/preferences.py
--rw-r--r--   0 ken       (1000) officers   (501)    76947 2016-01-05 06:40:14.000000 avendesora-1.8.0/avendesora/words
--rw-r--r--   0 ken       (1000) officers   (501)     1694 2017-11-20 05:31:06.000000 avendesora-1.8.0/avendesora/dictionary.py
--rw-r--r--   0 ken       (1000) officers   (501)     4245 2017-11-20 05:31:32.000000 avendesora-1.8.0/avendesora/title.py
--rw-r--r--   0 ken       (1000) officers   (501)    14806 2017-11-21 19:23:13.000000 avendesora-1.8.0/avendesora/generator.py
--rw-r--r--   0 ken       (1000) officers   (501)     1730 2017-11-20 05:30:57.000000 avendesora-1.8.0/avendesora/editors.py
--rw-r--r--   0 ken       (1000) officers   (501)     2359 2017-11-19 03:53:22.000000 avendesora-1.8.0/avendesora/collection.py
--rw-r--r--   0 ken       (1000) officers   (501)    12811 2017-11-20 05:31:38.000000 avendesora-1.8.0/avendesora/writer.py
--rw-r--r--   0 ken       (1000) officers   (501)     2307 2017-11-20 05:30:40.000000 avendesora-1.8.0/avendesora/browsers.py
--rw-r--r--   0 ken       (1000) officers   (501)      908 2017-11-23 16:59:19.000000 avendesora-1.8.0/avendesora/__init__.py
--rw-r--r--   0 ken       (1000) officers   (501)    33835 2017-11-21 19:23:09.000000 avendesora-1.8.0/avendesora/account.py
--rw-r--r--   0 ken       (1000) officers   (501)    13747 2017-11-21 19:23:16.000000 avendesora-1.8.0/avendesora/obscure.py
--rw-r--r--   0 ken       (1000) officers   (501)     9165 2017-11-20 05:31:12.000000 avendesora-1.8.0/avendesora/gpg.py
--rw-r--r--   0 ken       (1000) officers   (501)     6953 2017-11-22 01:55:35.000000 avendesora-1.8.0/avendesora/utilities.py
--rw-r--r--   0 ken       (1000) officers   (501)    34668 2017-11-21 05:08:57.000000 avendesora-1.8.0/avendesora/secrets.py
--rw-r--r--   0 ken       (1000) officers   (501)    26884 2017-11-20 05:31:23.000000 avendesora-1.8.0/avendesora/recognize.py
--rw-r--r--   0 ken       (1000) officers   (501)     4103 2017-11-20 05:30:47.000000 avendesora-1.8.0/avendesora/config.py
--rw-r--r--   0 ken       (1000) officers   (501)     2101 2017-11-20 05:31:04.000000 avendesora-1.8.0/avendesora/main.py
--rw-r--r--   0 ken       (1000) officers   (501)     2240 2017-11-19 03:53:45.000000 avendesora-1.8.0/avendesora/cursor.py
--rw-r--r--   0 ken       (1000) officers   (501)     1017 2017-11-20 05:36:13.000000 avendesora-1.8.0/avendesora/error.py
--rw-r--r--   0 ken       (1000) officers   (501)    49753 2017-11-22 01:55:31.000000 avendesora-1.8.0/avendesora/command.py
--rw-r--r--   0 ken       (1000) officers   (501)     3506 2017-11-19 03:53:54.000000 avendesora-1.8.0/avendesora/dialog.py
--rw-r--r--   0 ken       (1000) officers   (501)     2055 2017-11-19 03:53:40.000000 avendesora-1.8.0/avendesora/charsets.py
--rw-r--r--   0 ken       (1000) officers   (501)    72032 2017-11-21 03:36:46.000000 avendesora-1.8.0/avendesora/help.py
-drwxr-xr-x   0 ken       (1000) officers   (501)        0 2017-11-23 17:23:14.000000 avendesora-1.8.0/tests/
--rw-r--r--   0 ken       (1000) officers   (501)     7574 2017-11-12 08:59:35.000000 avendesora-1.8.0/tests/test_avendesora.py
-drwxr-xr-x   0 ken       (1000) officers   (501)        0 2017-11-23 17:23:14.000000 avendesora-1.8.0/tests/avendesora/
--rw-r--r--   0 ken       (1000) officers   (501)    30823 2017-11-21 19:23:23.000000 avendesora-1.8.0/tests/avendesora/preferences.py
--rw-r--r--   0 ken       (1000) officers   (501)    76947 2016-01-05 06:40:14.000000 avendesora-1.8.0/tests/avendesora/words
--rw-r--r--   0 ken       (1000) officers   (501)     1694 2017-11-20 05:31:06.000000 avendesora-1.8.0/tests/avendesora/dictionary.py
--rw-r--r--   0 ken       (1000) officers   (501)     4245 2017-11-20 05:31:32.000000 avendesora-1.8.0/tests/avendesora/title.py
--rw-r--r--   0 ken       (1000) officers   (501)    14806 2017-11-21 19:23:13.000000 avendesora-1.8.0/tests/avendesora/generator.py
--rw-r--r--   0 ken       (1000) officers   (501)     1730 2017-11-20 05:30:57.000000 avendesora-1.8.0/tests/avendesora/editors.py
--rw-r--r--   0 ken       (1000) officers   (501)     2359 2017-11-19 03:53:22.000000 avendesora-1.8.0/tests/avendesora/collection.py
--rw-r--r--   0 ken       (1000) officers   (501)    12811 2017-11-20 05:31:38.000000 avendesora-1.8.0/tests/avendesora/writer.py
--rw-r--r--   0 ken       (1000) officers   (501)     2307 2017-11-20 05:30:40.000000 avendesora-1.8.0/tests/avendesora/browsers.py
--rw-r--r--   0 ken       (1000) officers   (501)      908 2017-11-23 16:59:19.000000 avendesora-1.8.0/tests/avendesora/__init__.py
--rw-r--r--   0 ken       (1000) officers   (501)    33835 2017-11-21 19:23:09.000000 avendesora-1.8.0/tests/avendesora/account.py
--rw-r--r--   0 ken       (1000) officers   (501)    13747 2017-11-21 19:23:16.000000 avendesora-1.8.0/tests/avendesora/obscure.py
--rw-r--r--   0 ken       (1000) officers   (501)     9165 2017-11-20 05:31:12.000000 avendesora-1.8.0/tests/avendesora/gpg.py
--rw-r--r--   0 ken       (1000) officers   (501)     6953 2017-11-22 01:55:35.000000 avendesora-1.8.0/tests/avendesora/utilities.py
--rw-r--r--   0 ken       (1000) officers   (501)    34668 2017-11-21 05:08:57.000000 avendesora-1.8.0/tests/avendesora/secrets.py
--rw-r--r--   0 ken       (1000) officers   (501)    26884 2017-11-20 05:31:23.000000 avendesora-1.8.0/tests/avendesora/recognize.py
--rw-r--r--   0 ken       (1000) officers   (501)     4103 2017-11-20 05:30:47.000000 avendesora-1.8.0/tests/avendesora/config.py
--rw-r--r--   0 ken       (1000) officers   (501)     2101 2017-11-20 05:31:04.000000 avendesora-1.8.0/tests/avendesora/main.py
--rw-r--r--   0 ken       (1000) officers   (501)     2240 2017-11-19 03:53:45.000000 avendesora-1.8.0/tests/avendesora/cursor.py
--rw-r--r--   0 ken       (1000) officers   (501)     1017 2017-11-20 05:36:13.000000 avendesora-1.8.0/tests/avendesora/error.py
--rw-r--r--   0 ken       (1000) officers   (501)    49753 2017-11-22 01:55:31.000000 avendesora-1.8.0/tests/avendesora/command.py
--rw-r--r--   0 ken       (1000) officers   (501)     3506 2017-11-19 03:53:54.000000 avendesora-1.8.0/tests/avendesora/dialog.py
--rw-r--r--   0 ken       (1000) officers   (501)     2055 2017-11-19 03:53:40.000000 avendesora-1.8.0/tests/avendesora/charsets.py
--rw-r--r--   0 ken       (1000) officers   (501)    72032 2017-11-21 03:36:46.000000 avendesora-1.8.0/tests/avendesora/help.py
--rw-r--r--   0 ken       (1000) officers   (501)       46 2016-07-20 04:57:11.000000 avendesora-1.8.0/tests/pytest.ini
--rw-r--r--   0 ken       (1000) officers   (501)    93679 2017-11-20 08:20:54.000000 avendesora-1.8.0/tests/test_help.py
-drwxr-xr-x   0 ken       (1000) officers   (501)        0 2017-11-23 17:23:14.000000 avendesora-1.8.0/tests/home/
-drwxr-xr-x   0 ken       (1000) officers   (501)        0 2017-11-23 17:23:14.000000 avendesora-1.8.0/tests/home/.gnupg/
--rw-------   0 ken       (1000) officers   (501)      600 2016-07-19 05:08:36.000000 avendesora-1.8.0/tests/home/.gnupg/random_seed
--rw-------   0 ken       (1000) officers   (501)     1280 2016-05-24 07:00:47.000000 avendesora-1.8.0/tests/home/.gnupg/trustdb.gpg
-drwxr-xr-x   0 ken       (1000) officers   (501)        0 2017-11-23 17:23:14.000000 avendesora-1.8.0/tests/home/.gnupg/private-keys-v1.d/
--rw-------   0 ken       (1000) officers   (501)      977 2016-05-24 07:01:12.000000 avendesora-1.8.0/tests/home/.gnupg/private-keys-v1.d/32489E4B20C131A366C6711687E2712C8C64A62E.key
--rw-------   0 ken       (1000) officers   (501)      977 2016-05-24 07:01:12.000000 avendesora-1.8.0/tests/home/.gnupg/private-keys-v1.d/2840F86F07D2EEF141115D06F6B9CD52B4D37F06.key
--rw-------   0 ken       (1000) officers   (501)        0 2016-05-24 07:00:47.000000 avendesora-1.8.0/tests/home/.gnupg/pubring.gpg
--rw-------   0 ken       (1000) officers   (501)     1375 2016-05-24 07:00:47.000000 avendesora-1.8.0/tests/home/.gnupg/pubring.kbx
--rw-------   0 ken       (1000) officers   (501)        0 2016-05-24 07:00:47.000000 avendesora-1.8.0/tests/home/.gnupg/secring.gpg
-drwxr-xr-x   0 ken       (1000) officers   (501)        0 2017-11-23 17:23:14.000000 avendesora-1.8.0/tests/home/gnupg/
--rw-------   0 ken       (1000) officers   (501)      600 2016-07-19 05:08:36.000000 avendesora-1.8.0/tests/home/gnupg/random_seed
--rw-------   0 ken       (1000) officers   (501)     1280 2016-05-24 07:00:47.000000 avendesora-1.8.0/tests/home/gnupg/trustdb.gpg
-drwxr-xr-x   0 ken       (1000) officers   (501)        0 2017-11-23 17:23:14.000000 avendesora-1.8.0/tests/home/gnupg/private-keys-v1.d/
--rw-------   0 ken       (1000) officers   (501)      977 2016-05-24 07:01:12.000000 avendesora-1.8.0/tests/home/gnupg/private-keys-v1.d/32489E4B20C131A366C6711687E2712C8C64A62E.key
--rw-------   0 ken       (1000) officers   (501)      977 2016-05-24 07:01:12.000000 avendesora-1.8.0/tests/home/gnupg/private-keys-v1.d/2840F86F07D2EEF141115D06F6B9CD52B4D37F06.key
--rw-------   0 ken       (1000) officers   (501)        0 2016-05-24 07:00:47.000000 avendesora-1.8.0/tests/home/gnupg/pubring.gpg
--rw-------   0 ken       (1000) officers   (501)     1375 2016-05-24 07:00:47.000000 avendesora-1.8.0/tests/home/gnupg/pubring.kbx
--rw-------   0 ken       (1000) officers   (501)        0 2016-05-24 07:00:47.000000 avendesora-1.8.0/tests/home/gnupg/secring.gpg
-drwxr-xr-x   0 ken       (1000) officers   (501)        0 2017-11-23 17:23:14.000000 avendesora-1.8.0/tests/home/.config/
-drwxr-xr-x   0 ken       (1000) officers   (501)        0 2017-11-23 17:23:14.000000 avendesora-1.8.0/tests/home/.config/avendesora/
--rw-r--r--   0 ken       (1000) officers   (501)      746 2017-11-21 05:09:08.000000 avendesora-1.8.0/tests/home/.config/avendesora/hashes
--rw-r--r--   0 ken       (1000) officers   (501)     3501 2016-12-22 01:04:38.000000 avendesora-1.8.0/tests/home/.config/avendesora/accounts
--rw-r--r--   0 ken       (1000) officers   (501)      313 2017-11-12 10:23:40.000000 avendesora-1.8.0/tests/home/.config/avendesora/key
--rw-r--r--   0 ken       (1000) officers   (501)     4698 2017-01-08 22:21:53.000000 avendesora-1.8.0/tests/home/.config/avendesora/stealth_accounts
--rw-------   0 ken       (1000) officers   (501)      596 2017-11-12 10:54:37.000000 avendesora-1.8.0/tests/home/.config/avendesora/key.gpg
--rw-r--r--   0 ken       (1000) officers   (501)      329 2017-01-08 22:21:56.000000 avendesora-1.8.0/tests/home/.config/avendesora/accounts_files
--rw-r--r--   0 ken       (1000) officers   (501)      864 2017-11-12 16:55:52.000000 avendesora-1.8.0/tests/home/.config/avendesora/config
-drwxr-xr-x   0 ken       (1000) officers   (501)        0 2017-11-23 17:23:14.000000 avendesora-1.8.0/tests/home/config/
-drwxr-xr-x   0 ken       (1000) officers   (501)        0 2017-11-23 17:23:14.000000 avendesora-1.8.0/tests/home/config/avendesora/
--rw-r--r--   0 ken       (1000) officers   (501)      746 2017-11-21 05:09:08.000000 avendesora-1.8.0/tests/home/config/avendesora/hashes
--rw-r--r--   0 ken       (1000) officers   (501)     3501 2016-12-22 01:04:38.000000 avendesora-1.8.0/tests/home/config/avendesora/accounts
--rw-r--r--   0 ken       (1000) officers   (501)      313 2017-11-12 10:23:40.000000 avendesora-1.8.0/tests/home/config/avendesora/key
--rw-r--r--   0 ken       (1000) officers   (501)     4698 2017-01-08 22:21:53.000000 avendesora-1.8.0/tests/home/config/avendesora/stealth_accounts
--rw-------   0 ken       (1000) officers   (501)      596 2017-11-12 10:54:37.000000 avendesora-1.8.0/tests/home/config/avendesora/key.gpg
--rw-r--r--   0 ken       (1000) officers   (501)      329 2017-01-08 22:21:56.000000 avendesora-1.8.0/tests/home/config/avendesora/accounts_files
--rw-r--r--   0 ken       (1000) officers   (501)      864 2017-11-12 16:55:52.000000 avendesora-1.8.0/tests/home/config/avendesora/config
--rw-r--r--   0 ken       (1000) officers   (501)     4797 2017-11-12 08:59:39.000000 avendesora-1.8.0/tests/test_api.py
--rw-r--r--   0 ken       (1000) officers   (501)      103 2016-12-19 06:25:32.000000 avendesora-1.8.0/tests/.coveragerc
--rw-r--r--   0 ken       (1000) officers   (501)    32472 2016-01-05 08:31:48.000000 avendesora-1.8.0/LICENSE
--rw-r--r--   0 ken       (1000) officers   (501)    36410 2017-11-23 17:23:14.000000 avendesora-1.8.0/PKG-INFO
--rw-r--r--   0 ken       (1000) officers   (501)     2889 2017-11-23 16:59:19.000000 avendesora-1.8.0/setup.py
--rw-r--r--   0 ken       (1000) officers   (501)       38 2017-11-23 17:23:14.000000 avendesora-1.8.0/setup.cfg
--rw-r--r--   0 ken       (1000) officers   (501)      170 2016-01-05 08:31:48.000000 avendesora-1.8.0/MANIFEST.in
-drwxr-xr-x   0 ken       (1000) officers   (501)        0 2017-11-23 17:23:14.000000 avendesora-1.8.0/avendesora.egg-info/
--rw-r--r--   0 ken       (1000) officers   (501)       65 2017-11-23 17:23:14.000000 avendesora-1.8.0/avendesora.egg-info/requires.txt
--rw-r--r--   0 ken       (1000) officers   (501)     2698 2017-11-23 17:23:14.000000 avendesora-1.8.0/avendesora.egg-info/SOURCES.txt
--rw-r--r--   0 ken       (1000) officers   (501)        1 2017-11-23 17:23:14.000000 avendesora-1.8.0/avendesora.egg-info/dependency_links.txt
--rw-r--r--   0 ken       (1000) officers   (501)    36410 2017-11-23 17:23:14.000000 avendesora-1.8.0/avendesora.egg-info/PKG-INFO
--rw-r--r--   0 ken       (1000) officers   (501)       53 2017-11-23 17:23:14.000000 avendesora-1.8.0/avendesora.egg-info/entry_points.txt
--rw-r--r--   0 ken       (1000) officers   (501)       11 2017-11-23 17:23:14.000000 avendesora-1.8.0/avendesora.egg-info/top_level.txt
+drwxr-xr-x   0 ken       (1000) officers   (501)        0 2017-12-26 02:26:38.000000 avendesora-1.9.0/
+-rw-r--r--   0 ken       (1000) officers   (501)    29483 2017-12-26 02:21:24.000000 avendesora-1.9.0/README.rst
+drwxr-xr-x   0 ken       (1000) officers   (501)        0 2017-12-26 02:26:38.000000 avendesora-1.9.0/avendesora/
+-rw-r--r--   0 ken       (1000) officers   (501)    30864 2017-12-26 01:28:05.000000 avendesora-1.9.0/avendesora/preferences.py
+-rw-r--r--   0 ken       (1000) officers   (501)    76947 2016-01-05 06:40:14.000000 avendesora-1.9.0/avendesora/words
+-rw-r--r--   0 ken       (1000) officers   (501)     1694 2017-11-20 05:31:06.000000 avendesora-1.9.0/avendesora/dictionary.py
+-rw-r--r--   0 ken       (1000) officers   (501)     4245 2017-11-20 05:31:32.000000 avendesora-1.9.0/avendesora/title.py
+-rw-r--r--   0 ken       (1000) officers   (501)    15057 2017-12-12 08:27:21.000000 avendesora-1.9.0/avendesora/generator.py
+-rw-r--r--   0 ken       (1000) officers   (501)     1730 2017-11-20 05:30:57.000000 avendesora-1.9.0/avendesora/editors.py
+-rw-r--r--   0 ken       (1000) officers   (501)     4084 2017-12-26 01:27:10.000000 avendesora-1.9.0/avendesora/collection.py
+-rw-r--r--   0 ken       (1000) officers   (501)    12811 2017-11-20 05:31:38.000000 avendesora-1.9.0/avendesora/writer.py
+-rw-r--r--   0 ken       (1000) officers   (501)     2307 2017-11-20 05:30:40.000000 avendesora-1.9.0/avendesora/browsers.py
+-rw-r--r--   0 ken       (1000) officers   (501)     3275 2017-12-20 21:12:13.000000 avendesora-1.9.0/avendesora/otp.py
+-rw-r--r--   0 ken       (1000) officers   (501)      979 2017-12-26 02:21:24.000000 avendesora-1.9.0/avendesora/__init__.py
+-rw-r--r--   0 ken       (1000) officers   (501)    34818 2017-12-26 01:26:11.000000 avendesora-1.9.0/avendesora/account.py
+-rw-r--r--   0 ken       (1000) officers   (501)    13747 2017-11-21 19:23:16.000000 avendesora-1.9.0/avendesora/obscure.py
+-rw-r--r--   0 ken       (1000) officers   (501)     9390 2017-12-12 08:27:28.000000 avendesora-1.9.0/avendesora/gpg.py
+-rw-r--r--   0 ken       (1000) officers   (501)     7063 2017-12-12 06:52:44.000000 avendesora-1.9.0/avendesora/utilities.py
+-rw-r--r--   0 ken       (1000) officers   (501)    34668 2017-11-21 05:08:57.000000 avendesora-1.9.0/avendesora/secrets.py
+-rw-r--r--   0 ken       (1000) officers   (501)    26884 2017-11-20 05:31:23.000000 avendesora-1.9.0/avendesora/recognize.py
+-rw-r--r--   0 ken       (1000) officers   (501)     4103 2017-11-20 05:30:47.000000 avendesora-1.9.0/avendesora/config.py
+-rw-r--r--   0 ken       (1000) officers   (501)     2201 2017-12-26 01:27:27.000000 avendesora-1.9.0/avendesora/main.py
+-rw-r--r--   0 ken       (1000) officers   (501)     2240 2017-11-19 03:53:45.000000 avendesora-1.9.0/avendesora/cursor.py
+-rw-r--r--   0 ken       (1000) officers   (501)     1017 2017-11-20 05:36:13.000000 avendesora-1.9.0/avendesora/error.py
+-rw-r--r--   0 ken       (1000) officers   (501)    52892 2017-12-26 01:27:21.000000 avendesora-1.9.0/avendesora/command.py
+-rw-r--r--   0 ken       (1000) officers   (501)     3506 2017-11-19 03:53:54.000000 avendesora-1.9.0/avendesora/dialog.py
+-rw-r--r--   0 ken       (1000) officers   (501)     2055 2017-11-19 03:53:40.000000 avendesora-1.9.0/avendesora/charsets.py
+-rw-r--r--   0 ken       (1000) officers   (501)    73071 2017-12-26 01:27:55.000000 avendesora-1.9.0/avendesora/help.py
+drwxr-xr-x   0 ken       (1000) officers   (501)        0 2017-12-26 02:26:38.000000 avendesora-1.9.0/tests/
+-rw-r--r--   0 ken       (1000) officers   (501)     7916 2017-12-15 22:21:32.000000 avendesora-1.9.0/tests/test_avendesora.py
+drwxr-xr-x   0 ken       (1000) officers   (501)        0 2017-12-26 02:26:38.000000 avendesora-1.9.0/tests/avendesora/
+-rw-r--r--   0 ken       (1000) officers   (501)    30864 2017-12-26 01:28:05.000000 avendesora-1.9.0/tests/avendesora/preferences.py
+-rw-r--r--   0 ken       (1000) officers   (501)    76947 2016-01-05 06:40:14.000000 avendesora-1.9.0/tests/avendesora/words
+-rw-r--r--   0 ken       (1000) officers   (501)     1694 2017-11-20 05:31:06.000000 avendesora-1.9.0/tests/avendesora/dictionary.py
+-rw-r--r--   0 ken       (1000) officers   (501)     4245 2017-11-20 05:31:32.000000 avendesora-1.9.0/tests/avendesora/title.py
+-rw-r--r--   0 ken       (1000) officers   (501)    15057 2017-12-12 08:27:21.000000 avendesora-1.9.0/tests/avendesora/generator.py
+-rw-r--r--   0 ken       (1000) officers   (501)     1730 2017-11-20 05:30:57.000000 avendesora-1.9.0/tests/avendesora/editors.py
+-rw-r--r--   0 ken       (1000) officers   (501)     4084 2017-12-26 01:27:10.000000 avendesora-1.9.0/tests/avendesora/collection.py
+-rw-r--r--   0 ken       (1000) officers   (501)    12811 2017-11-20 05:31:38.000000 avendesora-1.9.0/tests/avendesora/writer.py
+-rw-r--r--   0 ken       (1000) officers   (501)     2307 2017-11-20 05:30:40.000000 avendesora-1.9.0/tests/avendesora/browsers.py
+-rw-r--r--   0 ken       (1000) officers   (501)     3275 2017-12-20 21:12:13.000000 avendesora-1.9.0/tests/avendesora/otp.py
+-rw-r--r--   0 ken       (1000) officers   (501)      979 2017-12-26 02:21:24.000000 avendesora-1.9.0/tests/avendesora/__init__.py
+-rw-r--r--   0 ken       (1000) officers   (501)    34818 2017-12-26 01:26:11.000000 avendesora-1.9.0/tests/avendesora/account.py
+-rw-r--r--   0 ken       (1000) officers   (501)    13747 2017-11-21 19:23:16.000000 avendesora-1.9.0/tests/avendesora/obscure.py
+-rw-r--r--   0 ken       (1000) officers   (501)     9390 2017-12-12 08:27:28.000000 avendesora-1.9.0/tests/avendesora/gpg.py
+-rw-r--r--   0 ken       (1000) officers   (501)     7063 2017-12-12 06:52:44.000000 avendesora-1.9.0/tests/avendesora/utilities.py
+-rw-r--r--   0 ken       (1000) officers   (501)    34668 2017-11-21 05:08:57.000000 avendesora-1.9.0/tests/avendesora/secrets.py
+-rw-r--r--   0 ken       (1000) officers   (501)    26884 2017-11-20 05:31:23.000000 avendesora-1.9.0/tests/avendesora/recognize.py
+-rw-r--r--   0 ken       (1000) officers   (501)     4103 2017-11-20 05:30:47.000000 avendesora-1.9.0/tests/avendesora/config.py
+-rw-r--r--   0 ken       (1000) officers   (501)     2201 2017-12-26 01:27:27.000000 avendesora-1.9.0/tests/avendesora/main.py
+-rw-r--r--   0 ken       (1000) officers   (501)     2240 2017-11-19 03:53:45.000000 avendesora-1.9.0/tests/avendesora/cursor.py
+-rw-r--r--   0 ken       (1000) officers   (501)     1017 2017-11-20 05:36:13.000000 avendesora-1.9.0/tests/avendesora/error.py
+-rw-r--r--   0 ken       (1000) officers   (501)    52892 2017-12-26 01:27:21.000000 avendesora-1.9.0/tests/avendesora/command.py
+-rw-r--r--   0 ken       (1000) officers   (501)     3506 2017-11-19 03:53:54.000000 avendesora-1.9.0/tests/avendesora/dialog.py
+-rw-r--r--   0 ken       (1000) officers   (501)     2055 2017-11-19 03:53:40.000000 avendesora-1.9.0/tests/avendesora/charsets.py
+-rw-r--r--   0 ken       (1000) officers   (501)    73071 2017-12-26 01:27:55.000000 avendesora-1.9.0/tests/avendesora/help.py
+-rw-r--r--   0 ken       (1000) officers   (501)       46 2016-07-20 04:57:11.000000 avendesora-1.9.0/tests/pytest.ini
+-rw-r--r--   0 ken       (1000) officers   (501)    96449 2017-12-26 01:31:43.000000 avendesora-1.9.0/tests/test_help.py
+drwxr-xr-x   0 ken       (1000) officers   (501)        0 2017-12-26 02:26:38.000000 avendesora-1.9.0/tests/home/
+drwxr-xr-x   0 ken       (1000) officers   (501)        0 2017-12-26 02:26:38.000000 avendesora-1.9.0/tests/home/.gnupg/
+-rw-------   0 ken       (1000) officers   (501)      600 2016-07-19 05:08:36.000000 avendesora-1.9.0/tests/home/.gnupg/random_seed
+-rw-------   0 ken       (1000) officers   (501)     1280 2016-05-24 07:00:47.000000 avendesora-1.9.0/tests/home/.gnupg/trustdb.gpg
+drwxr-xr-x   0 ken       (1000) officers   (501)        0 2017-12-26 02:26:38.000000 avendesora-1.9.0/tests/home/.gnupg/private-keys-v1.d/
+-rw-------   0 ken       (1000) officers   (501)      977 2016-05-24 07:01:12.000000 avendesora-1.9.0/tests/home/.gnupg/private-keys-v1.d/32489E4B20C131A366C6711687E2712C8C64A62E.key
+-rw-------   0 ken       (1000) officers   (501)      977 2016-05-24 07:01:12.000000 avendesora-1.9.0/tests/home/.gnupg/private-keys-v1.d/2840F86F07D2EEF141115D06F6B9CD52B4D37F06.key
+-rw-------   0 ken       (1000) officers   (501)        0 2016-05-24 07:00:47.000000 avendesora-1.9.0/tests/home/.gnupg/pubring.gpg
+-rw-------   0 ken       (1000) officers   (501)     1375 2016-05-24 07:00:47.000000 avendesora-1.9.0/tests/home/.gnupg/pubring.kbx
+-rw-------   0 ken       (1000) officers   (501)        0 2016-05-24 07:00:47.000000 avendesora-1.9.0/tests/home/.gnupg/secring.gpg
+drwxr-xr-x   0 ken       (1000) officers   (501)        0 2017-12-26 02:26:38.000000 avendesora-1.9.0/tests/home/gnupg/
+-rw-------   0 ken       (1000) officers   (501)      600 2016-07-19 05:08:36.000000 avendesora-1.9.0/tests/home/gnupg/random_seed
+-rw-------   0 ken       (1000) officers   (501)     1280 2016-05-24 07:00:47.000000 avendesora-1.9.0/tests/home/gnupg/trustdb.gpg
+drwxr-xr-x   0 ken       (1000) officers   (501)        0 2017-12-26 02:26:38.000000 avendesora-1.9.0/tests/home/gnupg/private-keys-v1.d/
+-rw-------   0 ken       (1000) officers   (501)      977 2016-05-24 07:01:12.000000 avendesora-1.9.0/tests/home/gnupg/private-keys-v1.d/32489E4B20C131A366C6711687E2712C8C64A62E.key
+-rw-------   0 ken       (1000) officers   (501)      977 2016-05-24 07:01:12.000000 avendesora-1.9.0/tests/home/gnupg/private-keys-v1.d/2840F86F07D2EEF141115D06F6B9CD52B4D37F06.key
+-rw-------   0 ken       (1000) officers   (501)        0 2016-05-24 07:00:47.000000 avendesora-1.9.0/tests/home/gnupg/pubring.gpg
+-rw-------   0 ken       (1000) officers   (501)     1375 2016-05-24 07:00:47.000000 avendesora-1.9.0/tests/home/gnupg/pubring.kbx
+-rw-------   0 ken       (1000) officers   (501)        0 2016-05-24 07:00:47.000000 avendesora-1.9.0/tests/home/gnupg/secring.gpg
+drwxr-xr-x   0 ken       (1000) officers   (501)        0 2017-12-26 02:26:38.000000 avendesora-1.9.0/tests/home/.config/
+drwxr-xr-x   0 ken       (1000) officers   (501)        0 2017-12-26 02:26:38.000000 avendesora-1.9.0/tests/home/.config/avendesora/
+-rw-r--r--   0 ken       (1000) officers   (501)      746 2017-11-21 05:09:08.000000 avendesora-1.9.0/tests/home/.config/avendesora/hashes
+-rw-r--r--   0 ken       (1000) officers   (501)     3540 2017-12-15 22:21:56.000000 avendesora-1.9.0/tests/home/.config/avendesora/accounts
+-rw-r--r--   0 ken       (1000) officers   (501)      313 2017-11-12 10:23:40.000000 avendesora-1.9.0/tests/home/.config/avendesora/key
+-rw-r--r--   0 ken       (1000) officers   (501)     4698 2017-01-08 22:21:53.000000 avendesora-1.9.0/tests/home/.config/avendesora/stealth_accounts
+-rw-------   0 ken       (1000) officers   (501)      596 2017-11-12 10:54:37.000000 avendesora-1.9.0/tests/home/.config/avendesora/key.gpg
+-rw-r--r--   0 ken       (1000) officers   (501)      329 2017-01-08 22:21:56.000000 avendesora-1.9.0/tests/home/.config/avendesora/accounts_files
+-rw-r--r--   0 ken       (1000) officers   (501)      864 2017-11-12 16:55:52.000000 avendesora-1.9.0/tests/home/.config/avendesora/config
+drwxr-xr-x   0 ken       (1000) officers   (501)        0 2017-12-26 02:26:38.000000 avendesora-1.9.0/tests/home/config/
+drwxr-xr-x   0 ken       (1000) officers   (501)        0 2017-12-26 02:26:38.000000 avendesora-1.9.0/tests/home/config/avendesora/
+-rw-r--r--   0 ken       (1000) officers   (501)      746 2017-11-21 05:09:08.000000 avendesora-1.9.0/tests/home/config/avendesora/hashes
+-rw-r--r--   0 ken       (1000) officers   (501)     3540 2017-12-15 22:21:56.000000 avendesora-1.9.0/tests/home/config/avendesora/accounts
+-rw-r--r--   0 ken       (1000) officers   (501)      313 2017-11-12 10:23:40.000000 avendesora-1.9.0/tests/home/config/avendesora/key
+-rw-r--r--   0 ken       (1000) officers   (501)     4698 2017-01-08 22:21:53.000000 avendesora-1.9.0/tests/home/config/avendesora/stealth_accounts
+-rw-------   0 ken       (1000) officers   (501)      596 2017-11-12 10:54:37.000000 avendesora-1.9.0/tests/home/config/avendesora/key.gpg
+-rw-r--r--   0 ken       (1000) officers   (501)      329 2017-01-08 22:21:56.000000 avendesora-1.9.0/tests/home/config/avendesora/accounts_files
+-rw-r--r--   0 ken       (1000) officers   (501)      864 2017-11-12 16:55:52.000000 avendesora-1.9.0/tests/home/config/avendesora/config
+-rw-r--r--   0 ken       (1000) officers   (501)     4797 2017-11-12 08:59:39.000000 avendesora-1.9.0/tests/test_api.py
+-rw-r--r--   0 ken       (1000) officers   (501)      103 2016-12-19 06:25:32.000000 avendesora-1.9.0/tests/.coveragerc
+-rw-r--r--   0 ken       (1000) officers   (501)    32472 2016-01-05 08:31:48.000000 avendesora-1.9.0/LICENSE
+-rw-r--r--   0 ken       (1000) officers   (501)    36409 2017-12-26 02:26:38.000000 avendesora-1.9.0/PKG-INFO
+-rw-r--r--   0 ken       (1000) officers   (501)     2964 2017-12-26 02:21:24.000000 avendesora-1.9.0/setup.py
+-rw-r--r--   0 ken       (1000) officers   (501)       38 2017-12-26 02:26:38.000000 avendesora-1.9.0/setup.cfg
+-rw-r--r--   0 ken       (1000) officers   (501)      170 2016-01-05 08:31:48.000000 avendesora-1.9.0/MANIFEST.in
+drwxr-xr-x   0 ken       (1000) officers   (501)        0 2017-12-26 02:26:38.000000 avendesora-1.9.0/avendesora.egg-info/
+-rw-r--r--   0 ken       (1000) officers   (501)       71 2017-12-26 02:26:37.000000 avendesora-1.9.0/avendesora.egg-info/requires.txt
+-rw-r--r--   0 ken       (1000) officers   (501)     2740 2017-12-26 02:26:37.000000 avendesora-1.9.0/avendesora.egg-info/SOURCES.txt
+-rw-r--r--   0 ken       (1000) officers   (501)        1 2017-12-26 02:26:37.000000 avendesora-1.9.0/avendesora.egg-info/dependency_links.txt
+-rw-r--r--   0 ken       (1000) officers   (501)    36409 2017-12-26 02:26:37.000000 avendesora-1.9.0/avendesora.egg-info/PKG-INFO
+-rw-r--r--   0 ken       (1000) officers   (501)       53 2017-12-26 02:26:37.000000 avendesora-1.9.0/avendesora.egg-info/entry_points.txt
+-rw-r--r--   0 ken       (1000) officers   (501)       11 2017-12-26 02:26:37.000000 avendesora-1.9.0/avendesora.egg-info/top_level.txt
```

### Comparing `avendesora-1.8.0/README.rst` & `avendesora-1.9.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Avendesora Collaborative Password Utility
+Avendesora Collaborative Password Manager
 =========================================
 
 *Avendesora, the leaf of the Tree of Life is the key.*
 
 .. image:: https://img.shields.io/travis/KenKundert/avendesora/master.svg
     :target: https://travis-ci.org/KenKundert/avendesora
 
@@ -15,16 +15,16 @@
 .. image:: https://img.shields.io/pypi/pyversions/avendesora.svg
     :target: https://pypi.python.org/pypi/avendesora/
 
 .. IGNORE: pypi statics are broken and unlikely to be fixed
     .. image:: https://img.shields.io/pypi/dm/avendesora.svg
         :target: https://pypi.python.org/pypi/avendesora/
 
-| Version: 1.8.0
-| Released: 2017-11-23
+| Version: 1.9.0
+| Released: 2017-12-25
 |
 
 Avendesora replaces the Abraxas, which are both alternatives to the traditional 
 password vault.
 
 Please report all bugs and suggestions to avendesora@nurdletech.com
 
@@ -88,15 +88,15 @@
 You will also need to install some operating system commands. On Fedora use::
 
    yum install gnupg2 xdotool xsel
 
 You should also install python-gobject. Conceivably this could be installed with 
 the above pip command, but gobject appears broken in pypi, so it is better use 
 the operating system's package manager to install it.  See the setup.py file for 
-more information.  On Redhat systms use::
+more information.  On Redhat systems use::
 
    yum install python3-gobject
 
 If you would like to use scrypt as a way of encrypting fields, you will need to 
 install scrypt by hand using::
 
    pip3 install --user scrypt
@@ -454,15 +454,15 @@
 a situation where you need a secret, such as visiting your bank's website in 
 your browser, then you click on the account name field with your mouse and type 
 your hot key. This runs Avendesora without an account name. In this case, 
 Avendesora uses secret discovery to determine which secret to use and the script 
 that should be used to produce the required information. Generally the script 
 would be to enter the account name, then tab, then the password, and finally 
 return, but you can configure the script as you choose. This is all done as part 
-of configuring discovery. The method for associating Advendesora to a particular 
+of configuring discovery. The method for associating Avendesora to a particular 
 hot key is dependent on your window manager. With Gnome, it requires that you 
 open your Keyboard Shortcuts preferences and create a new shortcut. When you do 
 this, choose 'avendesora value' as the command to run.
 
 
 Python API
 ----------
@@ -497,15 +497,15 @@
 PasswordGenerator():
     Initializes the password generator. You should pass no arguments.
 
 get_account(name, request_seed=False, stealth_name=None):
     Accesses a particular account. Takes a string for the account name or alias.  
     The name is case insensitive and the '-' may be given for '_'.
 
-    Optionally takes a second argument (*request_seed*) that may be a boolean, 
+    Optionally takes a second argument (*request_seed*) that may be a Boolean, 
     a string, or a function that returns a string. The string is used as an 
     additional seed (see: `avendesora help misdirection`), and if True is passed 
     in, the user in queried for the seed.
 
     The stealth name is used as account name if the account is a stealth 
     account.
 
@@ -513,15 +513,15 @@
 get_name():
     return name of account.
 
 get_value(field):
     Returns the value of a particular account attribute given a user-oriented 
     string that describes the desired attribute.  The value requested must be 
     a scalar value, meaning that you must individually request members of arrays 
-    or dictionary attibutes. Here are some examples that demonstrate the various 
+    or dictionary attributes. Here are some examples that demonstrate the various 
     ways of accessing the various kinds of attributes:
 
     .. code-block:: python
 
         passcode = account.get_value()
         username = account.get_value('username')
         both = account.get_value('username: {username}, password: {passcode}')
@@ -558,15 +558,15 @@
     d (description) and v (value).  A format string does not match it if 
     contains a key for a value that is not available. If no format string 
     matches, the value is returned as a string.  The default formats are ('{f} 
     ({d}): {v}', '{f}: {v}').
 
     If a composite field is requested get_value() raises a PasswordError, and 
     the exception contains the *is_collection* and *collection* attributes. The 
-    first is a boolean and the second is the list of available keys.  
+    first is a Boolean and the second is the list of available keys.  
     PassworError returns None for unknown attributes, so it is always safe to 
     access these attributes without checking whether they exist.
 
 get_values(field):
     Used to get the values for a composite field. It iterates through the value 
     and returns a tuple that contains the key and the value for each item in the 
     field.
@@ -609,15 +609,15 @@
                     lines += indent(
                         value.render(('{k}) {d}: {v}', '{k}: {v}'))
                     ).split('\n')
             if keys:
                 value = acct.get_value(name)
                 lines += value.render('{n}: {v}').split('\n')
 
-    get_fields() accepts a boolean argument that if specified and is true will 
+    get_fields() accepts a Boolean argument that if specified and is true will 
     iterate through all fields, including those generally only used by 
     Avendesora, such as aliases and discovery.
 
 
 get_scalar(name, key=None, default=False):
     A lower level interface than get_value that given a name and perhaps a key 
     returns a scalar value.  Also takes an optional default value that is 
@@ -728,11 +728,11 @@
 It is worth browsing all of the available topics at least once to get a sense of 
 all that Avendesora can do.
 
 
 Contributing
 ------------
 
-Please ask questions or report bugs on ``Github Issues 
-<https://github.com/KenKundert/avendesora/issues>``_. I will entertain pull 
+Please ask questions or report bugs on `Github Issues 
+<https://github.com/KenKundert/avendesora/issues>`_. I will entertain pull 
 requests if you make improvements. I am particularly interested in help adapting 
 *Avendesora* for other editors, window managers and distributions.
```

### Comparing `avendesora-1.8.0/avendesora/preferences.py` & `avendesora-1.9.0/avendesora/preferences.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,21 +28,22 @@
 # but should not be found in the config file
 NONCONFIG_SETTINGS = {
     'config_file': 'config',
     'config_doc_file': 'config.doc',
     'settings_dir': user_config_dir('avendesora'),
     'default_accounts_file': 'accounts.gpg',
     'default_stealth_accounts_file': 'stealth_accounts',
-    'charsets_hash': '82bb252a11ac8b6a9a6830809d181b96',
+    'charsets_hash': '0120b695fb247d4993b1595ab087cc15',
     'dict_hash': '11fe5bc734f4a956c37d7cb3da16ab3f',
-    'secrets_hash': '5fc0355b1c9eb0e885ecc26c28e0c60e',
+    'secrets_hash': 'e038c2a9022b23ac9ceda8645d94816b',
     'discard_logfile': False,
     'commonly_mistaken_attributes': {
         'url': 'urls',
         'alias': 'aliases',
+        'description': 'desc',
     }
 }
 
 
 # Config Settings {{{1
 # These are the default values for settings that may be found in the config file
 CONFIG_DEFAULTS = {
@@ -436,15 +437,15 @@
 
         # Character sets
         exclude, LOWERCASE, UPPERCASE, LETTERS, DIGITS, ALPHANUMERIC,
         HEXDIGITS, PUNCTUATION, SYMBOLS, WHITESPACE, PRINTABLE, DISTINGUISHABLE,
 
         # Secrets
         Password, Passphrase, PIN, Question, MixedPassword, PasswordRecipe,
-        BirthDate,
+        BirthDate, OTP,
 
         # Account Discovery
         RecognizeAll, RecognizeAny, RecognizeTitle, RecognizeURL, RecognizeCWD,
         RecognizeHost, RecognizeUser, RecognizeEnvVar, RecognizeNetwork,
     )
     try:
         # You need to install scrypt using 'pip install scrypt' to use Scrypt
@@ -773,15 +774,15 @@
     #
     #     > base64 -d - < <filename>
     #
     # where <filename> contains <hidden_arg>.
     #
 
     from avendesora import (
-        Hidden, Question, Script,
+        Hidden, Question, Script, OTP,
         RecognizeAll, RecognizeAny, RecognizeTitle, RecognizeURL, RecognizeCWD,
         RecognizeHost, RecognizeUser, RecognizeEnvVar, RecognizeNetwork,
         RecognizeFile
     )
 
     CREATED = '{date}'
     ACCOUNTS = {{
```

### Comparing `avendesora-1.8.0/avendesora/words` & `avendesora-1.9.0/avendesora/words`

 * *Files identical despite different names*

### Comparing `avendesora-1.8.0/avendesora/dictionary.py` & `avendesora-1.9.0/avendesora/dictionary.py`

 * *Files identical despite different names*

### Comparing `avendesora-1.8.0/avendesora/title.py` & `avendesora-1.9.0/avendesora/title.py`

 * *Files identical despite different names*

### Comparing `avendesora-1.8.0/avendesora/generator.py` & `avendesora-1.9.0/avendesora/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,22 +66,22 @@
     # Constructor {{{2
     def __init__(self, init=False, gpg_ids=None):
         # initialize avendesora (these should already be done if called from 
         # main, but it is safe to call them again)
         read_config()
         GnuPG.initialize()
 
-        # check the integrity of avendesora
-        validate_components()
-
         # create the avendesora data directory
         if init:
             self._initialize(gpg_ids, init)
             return
 
+        # check the integrity of avendesora
+        validate_components()
+
         # read the accounts files
         self.shared_secrets = {}
         seen = {}
         most_recently_updated = 0
         for filename in get_setting('accounts_files', []):
             path = to_path(get_setting('settings_dir'), filename)
             updated = os.path.getmtime(str(path.resolve()))
@@ -129,14 +129,20 @@
         def split(s, l=72):
             # Break long string into a series of adjacent shorter strings
             if len(s) < l:
                 return '"%s"' % s
             chunks = ['    "%s"' % s[i:i+l] for i in range(0, len(s), l)]
             return '\n' + '\n'.join(chunks) + '\n'
 
+        # create settings directory if it does not exist
+        settings_dir = to_path(get_setting('settings_dir'))
+        if not settings_dir.exists():
+            settings_dir.mkdir(mode=0o700, parents=True)
+            settings_dir.chmod(0o700)
+
         # Create dictionary of available substitutions for CONTENTS strings
         fields = {}
         for key in CONFIG_DEFAULTS:
             value = get_setting(key, expand=False)
             value = render(str(value) if isinstance(value, Path) else value)
             fields.update({key: value})
         for key in NONCONFIG_SETTINGS:
```

### Comparing `avendesora-1.8.0/avendesora/editors.py` & `avendesora-1.9.0/avendesora/editors.py`

 * *Files identical despite different names*

### Comparing `avendesora-1.8.0/avendesora/writer.py` & `avendesora-1.9.0/avendesora/writer.py`

 * *Files identical despite different names*

### Comparing `avendesora-1.8.0/avendesora/browsers.py` & `avendesora-1.9.0/avendesora/browsers.py`

 * *Files identical despite different names*

### Comparing `avendesora-1.8.0/avendesora/__init__.py` & `avendesora-1.9.0/avendesora/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,23 +6,27 @@
 from .error import PasswordError
 from .generator import PasswordGenerator
 from .obscure import Hide, Hidden, GPG
 try:
     from .obscure import Scrypt
 except ImportError:  # no cover
     pass
+try:
+    from .otp import OTP
+except ImportError:  # no cover
+    pass
 from .recognize import (
     RecognizeAll, RecognizeAny, RecognizeTitle, RecognizeURL, RecognizeCWD,
     RecognizeHost, RecognizeUser, RecognizeEnvVar, RecognizeNetwork,
     RecognizeFile
 )
 from .secrets import (
     Password, Passphrase, PIN, Question, MixedPassword, PasswordRecipe,
     BirthDate, SecretExhausted
 )
 
 # the following are used when generating the documentation and are not needed
 # otherwise
 from . import command
 
-__version__ = '1.8.0'
-__released__ = '2017-11-23'
+__version__ = '1.9.0'
+__released__ = '2017-12-25'
```

### Comparing `avendesora-1.8.0/avendesora/account.py` & `avendesora-1.9.0/avendesora/account.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,17 @@
 from .collection import Collection
 from .config import get_setting
 from .error import PasswordError
 from .obscure import ObscuredSecret
 from .preferences import TOOL_FIELDS
 from .recognize import Recognizer
 from .secrets import GeneratedSecret
+from difflib import get_close_matches
 from inform import (
-    Color, codicil, conjoin, cull, debug, is_collection, is_str, log,
+    Color, codicil, conjoin, cull, debug, full_stop, is_collection, is_str, log,
     notify, output, warn, indent,
     ddd, ppp, vvv
 )
 from textwrap import dedent
 try:
     from urllib.parse import urlparse
 except ImportError:
@@ -211,15 +212,34 @@
     # get_account() {{{2
     @staticmethod
     def get_account(name):
         canonical = canonicalize(name)
         try:
             return Account._accounts[canonical]
         except KeyError:
-            raise PasswordError('account not found.', culprit=name)
+            # account not found, assemble message giving suggested account names
+            names = Account._accounts.keys()
+            candidates = get_close_matches(canonical, names, 9, 0.6)
+
+            # do not want to give multiple options all of which are aliases for
+            # the same accounts, so look for up to three unique accounts
+            accounts = []
+            for candidate in candidates:
+                account = Account._accounts[candidate]
+                if account not in accounts:
+                    accounts.append(account)
+                if len(accounts) >= 3:
+                    break
+
+            # generate the message handling 0, 1, 2 or 3 candidates gracefully
+            msg = ['account not found']
+            candidates = conjoin((a.get_name() for a in accounts), conj=' or ')
+            if candidates:
+                msg.append('did you mean {}?'.format(candidates))
+            raise PasswordError(full_stop(', '.join(msg)), culprit=name)
 
     # get_name() {{{2
     @classmethod
     def get_name(cls):
         """Get account name.
 
         Returns:
@@ -282,15 +302,15 @@
             canonical = canonicalize(name)
             Account._accounts[canonical] = cls
             if canonical in seen:
                 if name == account_name:
                     warn('duplicate account name.', culprit=name)
                 else:
                     warn('alias duplicates existing name.', culprit=name)
-                codicil('Seen in %s in %s.' % seen[name])
+                codicil('Seen in %s in %s.' % seen[canonical])
                 codicil('And in %s in %s.' % (account_name, path))
                 break
             else:
                 new[canonical] = (account_name, path)
         seen.update(new)
             # this two step approach to updating seen prevents us from
             # complaining about aliases that duplicate the account name,
@@ -859,15 +879,15 @@
 
         # select the urls
         if not key:
             key = getattr(cls, 'default_url', None)
         try:
             urls = urls[key]
         except KeyError:
-            keys = cull(urls.keys())
+            keys = cull(list(urls.keys()))
             if keys:
                 if key:
                     msg = 'unknown key, choose from {}.'
                 else:
                     msg = 'key required, choose from {}.'
                 raise PasswordError(msg.format(conjoin(keys)), culprit=key)
             else:
```

### Comparing `avendesora-1.8.0/avendesora/obscure.py` & `avendesora-1.9.0/avendesora/obscure.py`

 * *Files identical despite different names*

### Comparing `avendesora-1.8.0/avendesora/gpg.py` & `avendesora-1.9.0/avendesora/gpg.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # You should have received a copy of the GNU General Public License along with
 # this program.  If not, see http://www.gnu.org/licenses/.
 
 
 # Imports {{{1
 from .config import get_setting, override_setting, setting_path
 from .error import PasswordError
-from shlib import to_path, cp, mkdir
+from shlib import to_path, cp
 from inform import (
     conjoin, cull, display, log, narrate, os_error, warn, is_str,
     full_stop
 )
 import gnupg
 try:
     from StringIO import StringIO   # python2
@@ -85,21 +85,25 @@
     def save(self, contents, gpg_ids=None):
         path = self.path
         if not gpg_ids:
             gpg_ids = get_setting('gpg_ids', [])
         if is_str(gpg_ids):
             gpg_ids = gpg_ids.split()
         if not gpg_ids:
-            raise PasswordError('must specify GPG ID.')
+            # raise PasswordError('must specify GPG ID.')
+            log('no gpg id is available, using symmetric encryption.')
 
         use_gpg, use_armor = self._choices()
         if use_gpg:
             try:
                 encoded = contents.encode(get_setting('encoding'))
-                encrypted = self.gpg.encrypt(encoded, gpg_ids, armor=use_armor)
+                if gpg_ids:
+                    encrypted = self.gpg.encrypt(encoded, gpg_ids, armor=use_armor)
+                else:
+                    encrypted = self.gpg.encrypt(encoded, None, symmetric='AES256', armor=use_armor)
                 if not encrypted.ok:
                     msg = ' '.join(cull([
                         'unable to encrypt.',
                         getattr(encrypted, 'stderr', None)
                     ]))
                     raise PasswordError(msg, culprit=path, sep='\n')
                 else:
@@ -242,21 +246,22 @@
             raise PasswordError(full_stop(e), culprit=error_source())
         ActivePythonFile = None
         return contents
 
     def create(self, contents, gpg_ids):
         path = self.path
         try:
-            mkdir(get_setting('settings_dir'))
+            # check to see if file already exists
             if path.exists():
                 # file creation (init) requested, but file already exists
                 # don't overwrite the file, instead read it so the information 
                 # can be used to create any remaining files.
                 display("%s: already exists." % path)
                 return
+
             # create the file
             display('%s: creating.' % path)
             if path.suffix in ['.gpg', '.asc']:
                 narrate('encrypting.', culprit=path)
                 # encrypt it
                 self.save(contents, gpg_ids)
             else:
```

### Comparing `avendesora-1.8.0/avendesora/utilities.py` & `avendesora-1.9.0/avendesora/utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,18 @@
 
 
 # validate_components {{{1
 def validate_components():
     # check permissions on the settings directory
     path = get_setting('settings_dir')
     mask = get_setting('config_dir_mask')
-    permissions = os.stat(path)[ST_MODE]
+    try:
+        permissions = os.stat(path)[ST_MODE]
+    except FileNotFoundError:
+        raise Error('missing, must run initialize.', culprit=path)
     violation = permissions & mask
     recommended = permissions & ~mask & 0o777
     if violation:
         warn(
             "directory permissions are too loose.",
             "Recommend running 'chmod {:o} {}'.".format(recommended, path),
             culprit=path
```

### Comparing `avendesora-1.8.0/avendesora/secrets.py` & `avendesora-1.9.0/avendesora/secrets.py`

 * *Files identical despite different names*

### Comparing `avendesora-1.8.0/avendesora/recognize.py` & `avendesora-1.9.0/avendesora/recognize.py`

 * *Files identical despite different names*

### Comparing `avendesora-1.8.0/avendesora/config.py` & `avendesora-1.9.0/avendesora/config.py`

 * *Files identical despite different names*

### Comparing `avendesora-1.8.0/avendesora/main.py` & `avendesora-1.9.0/avendesora/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 Generates passwords and pass phrases based on stored account information.
 
 Usage:
     avendesora [options] <command> [<args>...]
 
 Options:
-    -h, --help              Output basic usage information.
+    -h, --help        output basic usage information.
 
 Commands:
 {commands}
 
 Use 'avendesora help <command>' for information on a specific command.
 Use 'avendesora help' for list of available help topics.
 """
@@ -55,18 +55,23 @@
         cmdline = docopt(
             __doc__.format(commands=Command.summarize()),
             options_first=True
         )
 
         # start logging
         logfile = BufferedFile(get_setting('log_file'), True)
-        with Inform(logfile=logfile, hanging_indent=False):
-            Command.execute(cmdline['<command>'], cmdline['<args>'])
-            done()
+        Inform(
+            logfile=logfile, hanging_indent=False, stream_policy='header',
+            notify_if_no_tty=True
+        )
+
+        # run the requested command
+        Command.execute(cmdline['<command>'], cmdline['<args>'])
+        done()
     except KeyboardInterrupt:
-        output('Terminated by user.')
+        output('\nTerminated by user.')
         terminate()
     except (PasswordError, Error) as e:
         e.terminate()
     except OSError as e:
         fatal(os_error(e))
     done()
```

### Comparing `avendesora-1.8.0/avendesora/cursor.py` & `avendesora-1.9.0/avendesora/cursor.py`

 * *Files identical despite different names*

### Comparing `avendesora-1.8.0/avendesora/error.py` & `avendesora-1.9.0/avendesora/error.py`

 * *Files identical despite different names*

### Comparing `avendesora-1.8.0/avendesora/command.py` & `avendesora-1.9.0/avendesora/command.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 from .error import PasswordError
 from .generator import PasswordGenerator
 from .gpg import GnuPG, PythonFile
 from .obscure import ObscuredSecret
 from .utilities import query_user, two_columns
 from .writer import get_writer
 from inform import (
-    codicil, columns, cull, debug, error, full_stop, output, warn, conjoin,
-    os_error, is_collection, indent, render, ddd, ppp, vvv
+    codicil, columns, cull, debug, error, full_stop, join, output, warn,
+    conjoin, os_error, is_collection, indent, render, ddd, ppp, vvv
 )
 from shlib import chmod, cp, rm, to_path
 from docopt import docopt
 from textwrap import dedent
 import re
 import sys
 
@@ -722,18 +722,24 @@
 
         # run the generator
         generator = PasswordGenerator()
 
         # find accounts whose name matches the criteria
         to_print = []
         for acct in generator.find_accounts(cmdline['<text>']):
-            aliases = Collection(getattr(acct, 'aliases', [])).values()
-
-            aliases = ' (%s)' % (', '.join(aliases)) if aliases else ''
-            to_print += [acct.get_name() + aliases]
+            aliases = Collection(getattr(acct, 'aliases', []))
+            desc = getattr(acct, 'desc', None)
+            to_print.append(
+                join(acct.get_name(), aliases=aliases, desc=desc, template=(
+                    '{} ({aliases:\v|, }) -- {desc}',
+                    '{} ({aliases:\v|, })',
+                    '{} -- {desc}',
+                    '{}'
+                ))
+            )
         output(cmdline['<text>']+ ':')
         output('    ' + ('\n    '.join(sorted(to_print))))
 
 
 # Help {{{1
 class Help(Command):
     NAMES = 'help', 'h'
@@ -906,15 +912,15 @@
         # run the generator
         generator = PasswordGenerator(init=True, gpg_ids=gpg_ids)
 
 
 # Log {{{1
 class Log(Command):
     NAMES = 'log',
-    DESCRIPTION = 'open the logfile'
+    DESCRIPTION = 'show the logfile'
     USAGE = dedent("""
         Usage:
             avendesora log
     """).strip()
 
     @classmethod
     def help(cls):
@@ -977,14 +983,18 @@
                 credentials = 'usernames.0 usernames.1 passcode'
 
             If credentials is not specified then the first of the following will
             be used if available:
 
                 id: {idents}
                 secret: {secrets}
+
+            If your credentials include more than one secret they will be
+            presented one at a time for one minute each. You can cut the minute
+            short by typing Ctrl-C.
         """).strip()
         return text.format(
             title=title(cls.DESCRIPTION), usage=cls.USAGE,
             idents=idents, secrets=secrets,
         ).strip()
 
     @classmethod
@@ -997,15 +1007,15 @@
 
         # determine the account and output specified information
         account_name = cmdline['<account>']
         writer = get_writer(tty=True)
         account = generator.get_account(account_name, cmdline['--seed'])
         credentials = account.get_scalar('credentials', default=None)
         if credentials:
-            credentials = Collection(credentials)
+            credentials = credentials.split()
         else:
             ids = Collection(get_setting('credential_ids'))
             secrets = Collection(get_setting('credential_secrets'))
             for each in ids:
                 if account.has_field(each):
                     identity = each
                     break
@@ -1077,19 +1087,19 @@
         generator = PasswordGenerator(
             init=cmdline['<name>'], gpg_ids=sorted(gpg_ids)
         )
 
 
 # Phonetic Alphabet {{{1
 class PhoneticAlphabet(Command):
-    NAMES = 'phonetic alphabet p'.split()
-    DESCRIPTION = 'Display NATO phonetic alphabet.'
+    NAMES = 'phonetic', 'alphabet', 'p'
+    DESCRIPTION = 'display NATO phonetic alphabet'
     USAGE = dedent("""
         Usage:
-            avendesora alphebet [<text>]
+            avendesora alphabet [<text>]
             avendesora phonetic [<text>]
             avendesora p [<text>]
     """).strip()
 
     @classmethod
     def help(cls):
         text = dedent("""
@@ -1106,29 +1116,29 @@
     @classmethod
     def run(cls, command, args):
         words = """
             Alfa Bravo Charlie Delta Echo Foxtrot Golf Hotel India Juliett Kilo
             Lima Mike November Oscar Papa Quebec Romeo Sierra Tango Uniform
             Victor Whiskey X-ray Yankee Zulu
         """.split()
-        mapping = {w[0]:w.lower() for w in words}
+        mapping = {w[0].lower():w for w in words}
         mapping.update({
-            '0':'zero', '1':'one', '2':'two', '3':'three', '4':'four',
-            '5':'five', '6':'six', '7':'seven', '8':'eight', '9':'nine'
+            '0':'Zero', '1':'One', '2':'Two', '3':'Three', '4':'Four',
+            '5':'Five', '6':'Six', '7':'Seven', '8':'Eight', '9':'Nine'
         })
 
         # read command line
         cmdline = docopt(cls.USAGE, argv=[command] + args)
         arg = cmdline['<text>']
 
         if arg:
             converted = []
-            for c in arg:
+            for c in arg.lower():
                 converted.append(mapping.get(c, c))
-            output(' '.join(converted))
+            output(' '.join(converted).lower())
         else:
             output('Phonetic alphabet:')
             output(columns(words))
 
 
 # Reveal {{{1
 class Reveal(Command):
@@ -1197,45 +1207,55 @@
 
         # run the generator
         generator = PasswordGenerator()
 
         # search for accounts that match search criteria
         to_print = []
         for acct in generator.search_accounts(cmdline['<text>']):
-            aliases = ', '.join(Collection(getattr(acct, 'aliases', [])).values())
-            aliases = ' (%s)' % (aliases) if aliases else ''
-            to_print += [acct.get_name() + aliases]
+            aliases = Collection(getattr(acct, 'aliases', []))
+            desc = getattr(acct, 'desc', None)
+            to_print.append(
+                join(acct.get_name(), aliases=aliases, desc=desc, template=(
+                    '{} ({aliases:\v|, }) -- {desc}',
+                    '{} ({aliases:\v|, })',
+                    '{} -- {desc}',
+                    '{}'
+                ))
+            )
         output(cmdline['<text>'] + ':')
         output('    ' + ('\n    '.join(sorted(to_print))))
 
 
 # Value {{{1
 class Value(Command):
-    NAMES = 'value', 'val', 'v'
+    NAMES = 'value', 'val', 'v', 'vc'
     DESCRIPTION = 'show an account value'
     USAGE = dedent("""
         Produce an account value. If the value is secret, it is produced only
         temporarily unless --stdout is specified.
 
         Usage:
             avendesora value [options] [<account> [<field>]]
             avendesora val   [options] [<account> [<field>]]
             avendesora v     [options] [<account> [<field>]]
+            avendesora vc    [options] [<account> [<field>]]
 
         Options:
             -c, --clipboard         Write output to clipboard rather than stdout.
             -s, --stdout            Write output to the standard output without
                                     any annotation or protections.
             -S, --seed              Interactively request additional seed for
                                     generated secrets.
             -v, --verbose           Add additional information to log file to
                                     help identify issues in account discovery.
             -T <title>, --title <title>
                                     Use account discovery on this title.
 
+        The 'vc' command is a shortcut for 'value --clipboard'.
+
         You request a scalar value by specifying its name after the account.
         For example:
 
             avendesora value bank pin
 
         If the requested value is composite (an array or dictionary), you should
         also specify a key that indicates which of the composite values you
@@ -1251,22 +1271,44 @@
         The field may be also be a script, with is nothing but a string that it
         output as given except that embedded attributes are replaced by account
         field values. For example:
 
             avendesora value bank '{accounts.checking}: {passcode}'
 
         If no value is requested the result produced is determined by the value
-        of the 'default' attribute. If no value is given for 'default', then the
-        'passcode' attribute is produced (this can be changed by specifying
-        'default_field' in the config file).  If 'default' is a script (see
-        'avendesora help scripts') then the script is executed. A typical script
-        might be 'username: {username}, password: {passcode}'. It is best if the
-        script produces a one line output if it contains secrets. If not a
-        script, the value of 'default' should be the name of another attribute,
-        and the value of that attribute is shown.
+        of the 'default' attribute (this can be changed by specifying
+        'default_field' in the config file). If no value is given for 'default',
+        then the *passcode*, *password*, or *passphrase* attribute is produced
+        (this can be changed by specifying the 'default_field' in the account or
+        the config file).  If 'default' is a script (see 'avendesora help
+        scripts') then the script is executed. A typical script might be
+        'username: {username}, password: {passcode}'. It is best if the script
+        produces a one line output if it contains secrets. If not a script, the
+        value of 'default' should be the name of another attribute, and the
+        value of that attribute is shown.
+
+        Normally the value command attempts to protects secrets. It does so
+        clearing the screen after a minute. If multiple secrets are requested,
+        you must either wait a minute to see each subsequent secret or type
+        Ctrl-C to clear the current secret and move on.  If you use --clipboard,
+        the clipboard is cleared after a minute.  However, if you use --stdout
+        this clearing of the secret does not occur. The --stdout option is
+        generally used with communicating with other Linux commands.  For
+        example, you can send a passcode to the standard input of a command as
+        follows:
+
+            avendesora value --stdout gpg | gpg --passphrase-fd 0 ...
+
+        You can place the username and password on a command line as follows:
+
+            curl --user `avendesora value -s apache '{username}:{passcode}'` ...
+
+        Be aware that it is possible for other users on shared Linux machines to
+        see the command line arguments of your commands, so passing secrets as
+        command arguments should only be used for low value secrets.
 
         If no account is requested, then Avendesora attempts to determine the
         appropriate account through discovery (see 'avendesora help discovery').
         Normally Avendesora is called in this manner from your window manager.
         You would arrange for it to be run when you type a hot key. In this case
         Avendesora determines which account to use from information available
         from the environment, information like the title on active window. In
@@ -1275,30 +1317,53 @@
         The verbose and title options are used when debugging account
         discovery. The verbose option adds more information about the
         discovery process to the logfile (~/.config/avendesora/log.gpg). The
         title option allows you to override the active window title so you can
         debug title-based discovery. Specifying the title option also scrubs
         the output and outputs directly to the standard output rather than
         mimicking the keyboard so as to avoid exposing your secret.
+
+        If the --stdout option is not specified, the value command still writes
+        to the standard output if it is associated with a TTY (if Avendesora is
+        outputting directly to a terminal). If standard output is not a TTY,
+        Avendesora mimics the keyboard and types the desired value directly into
+        the active window.  There are two common situations where standard
+        output is not a TTY: when Avendesora is being run by your window manager
+        in response to you pressing a hot key or when the output of Avendesora
+        is fed into a pipeline.  In the second case, mimicking the keyboard is
+        not what you want; you should use --stdout to assure the chosen value is
+        sent to the pipeline as desired.
     """).strip()
 
     @classmethod
     def run(cls, command, args):
         # read command line
         cmdline = docopt(cls.USAGE, argv=[command] + args)
+        use_clipboard = cmdline['--clipboard'] or cmdline['vc']
+
+        # mute any warnings if using --stdout
+        try:
+            from inform import get_informer
+            if cmdline['--stdout']:
+                get_informer().suppress_output()
+        except ImportError:
+            # remove this once the version 1.11 of inform is formally released
+            # --KSK
+            pass
+
 
         # run the generator
         generator = PasswordGenerator()
 
         # determine the account and output specified information
         account_name = cmdline['<account>']
         if account_name:
             account = generator.get_account(account_name, cmdline['--seed'])
             writer = get_writer(
-                clipboard=cmdline['--clipboard'], stdout=cmdline['--stdout']
+                clipboard=use_clipboard, stdout=cmdline['--stdout']
             )
             writer.display_field(account, cmdline['<field>'])
         else:
             # use discovery to determine account
             account_name, script = generator.discover_account(
                 title=cmdline['--title'], verbose=cmdline['--verbose']
             )
```

### Comparing `avendesora-1.8.0/avendesora/dialog.py` & `avendesora-1.9.0/avendesora/dialog.py`

 * *Files identical despite different names*

### Comparing `avendesora-1.8.0/avendesora/charsets.py` & `avendesora-1.9.0/avendesora/charsets.py`

 * *Files identical despite different names*

### Comparing `avendesora-1.8.0/avendesora/help.py` & `avendesora-1.9.0/avendesora/help.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,16 +27,18 @@
 # this program.  If not, see http://www.gnu.org/licenses/.
 
 
 # Imports {{{1
 from .browsers import StandardBrowser
 from .command import Command
 from .config import get_setting
+from .error import PasswordError
 from .utilities import pager, two_columns
-from inform import error, output
+from difflib import get_close_matches
+from inform import conjoin, full_stop, output
 from textwrap import dedent
 
 # HelpMessage base class {{{1
 class HelpMessage(object):
     URL = None
 
     # get_name() {{{2
@@ -86,15 +88,26 @@
                     return pager(cmd.help())
             for topic in cls.topics():
                 if name == topic.get_name():
                     if browse:
                         return show_in_browser(topic.URL)
                     else:
                         return pager(topic.help())
-            error('topic not found.', culprit=name)
+
+            # topic not found, give some alternatives
+            topics = (
+                [c.get_name() for c in Command.commands()]
+              + [t.get_name() for t in cls.topics()]
+            )
+            candidates = get_close_matches(name, topics, 3, 0.6)
+            msg = ['topic not found']
+            candidates = conjoin(candidates, conj=' or ')
+            if candidates:
+                msg.append('did you mean {}?'.format(candidates))
+            raise PasswordError(full_stop(', '.join(msg)), culprit=name)
         else:
             if browse:
                 return show_in_browser('')
             cls.help()
 
     # summarize {{{2
     @classmethod
@@ -875,15 +888,15 @@
 
                 > avendesora value <accountname> 0
                 questions.0 (oldest aunt): ampere reimburse duster
 
             You can get a list of your questions so you can identify which index
             to use with:
 
-                > avenedesora values <accountname>
+                > avendesora values <accountname>
                 ...
                 questions:
                     0: oldest aunt <reveal with 'avendesora value <accountname> questions.0'>
                     1: title of first job <reveal with 'avendesora value <accountname> questions.1'>
                     2: oldest uncle <reveal with 'avendesora value <accountname> questions.2'>
                     3: savings goal <reveal with 'avendesora value <accountname> questions.3'>
                     4: childhood vacation spot <reveal with 'avendesora value <accountname> questions.4'>
@@ -1240,15 +1253,15 @@
                 A string that is placed between each symbol in the generated
                 password.
             prefix (str):
                 A string added to the front of the generated password.
             suffix (str):
                 A string added to the end of the generated password.
 
-        Examples:
+        Example:
 
             passcode = Password(10)
 
 
         Passphrase
         ----------
 
@@ -1281,15 +1294,15 @@
                 A string that is placed between each symbol in the generated
                 password.
             prefix (str):
                 A string added to the front of the generated password.
             suffix (str):
                 A string added to the end of the generated password.
 
-        Examples:
+        Example:
 
             passcode = Passphrase()
 
 
         PIN
         ---
 
@@ -1312,15 +1325,15 @@
                 accounts contained in an account file.  This argument overrides
                 that behavior and instead explicitly specifies the master seed
                 for this secret.
             version (str):
                 An optional seed. Changing this value will change the generated
                 PIN.
 
-        Examples:
+        Example:
 
             passcode = PIN()
 
 
         Question
         --------
 
@@ -1364,15 +1377,15 @@
                 A string added to the front of the generated password.
             suffix (str):
                 A string added to the end of the generated password.
             answer:
                 The answer. If provided, this would override the generated
                 answer.  May be a string, or it may be an Obscured object.
 
-        Examples:
+        Example:
 
             questions = [
                 Question('Favorite foreign city'),
                 Question('Favorite breed of dog'),
             ]
 
 
@@ -1423,15 +1436,15 @@
                 answer.
             shift_sort(bool):
                 If true, the characters in the password will be sorted so that
                 the characters that require the shift key when typing are placed
                 last, making it easier to type. Use this option if you expect to
                 be typing the password by hand.
 
-        Examples:
+        Example:
 
             passcode = PasswordRecipe('12 2u 2d 2c!@#$%^&*')
 
 
         BirthDate
         ---------
 
@@ -1460,17 +1473,31 @@
                 accounts contained in an account file.  This argument overrides
                 that behavior and instead explicitly specifies the master seed
                 for this secret.
             version (str):
                 An optional seed. Changing this value will change the generated
                 answer.
 
-        Examples:
+        Example:
 
             birthdate = BirthDate(2015, 21, 55)
+
+
+        OTP
+        ---
+
+        Generates a secret that changes once per minute that generally is used
+        as a second factor when authenticating.  It can act as a replacement
+        for, and is fully compatible with, Google Authenticator.  You would
+        provide the text version of the shared secret (the backup code) that is
+        presented to you when first configuring your second factor authentication.
+
+        Example:
+
+            otp = OTP('JBSWY3DPEHPK3PXP')
         """).strip()
         return text
 
 
 # Stealth class {{{1
 class Stealth(HelpMessage):
     DESCRIPTION = "stealth secrets"
```

### Comparing `avendesora-1.8.0/tests/test_avendesora.py` & `avendesora-1.9.0/tests/test_avendesora.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import pytest
 from inform import os_error
 from textwrap import dedent
 import subprocess
 import os
 import pexpect
+import pyotp
 
 # set various environment variables so avendesora uses local gpg key and config
 # directory rather than the users.
 os.environ['HOME'] = 'home'
 
 # change the current working directory to the test directory
 cwd = os.getcwd()
@@ -152,14 +153,15 @@
         names: mybank, mb
         accounts:
             checking: <reveal with 'avendesora value mybank accounts.checking'>
             creditcard: <reveal with 'avendesora value mybank accounts.creditcard'>
             savings: <reveal with 'avendesora value mybank accounts.savings'>
         customer service: 1-866-229-6633
         email: pizzaman@pizza.com
+        otp: <reveal with 'avendesora value mybank otp'>
         passcode: <reveal with 'avendesora value mybank passcode'>
         pin: <reveal with 'avendesora value mybank pin'>
         questions:
             0: What city were you born in? <reveal with 'avendesora value mybank questions.0'>
             1: What street did you grow up on? <reveal with 'avendesora value mybank questions.1'>
             2: What was your childhood nickname? <reveal with 'avendesora value mybank questions.2'>
         urls: https://mb.com
@@ -238,7 +240,15 @@
         avendesora.close()
         result = avendesora.before.decode('utf-8')
     except (pexpect.EOF, pexpect.TIMEOUT):
         result = avendesora.before.decode('utf8')
     except OSError as err:
         result = os_error(err)
     assert result.strip() == 'tRT7vXLeZrbz'
+# test_mybank_otp() {{{1
+def test_mybank_otp():
+    otp = pyotp.TOTP('JBSWY3DPEHPK3PXP')
+    try:
+        result = run('avendesora value --stdout mybank otp')
+    except OSError as err:
+        result = os_error(err)
+    assert result.decode('ascii').strip() == otp.now()
```

### Comparing `avendesora-1.8.0/tests/avendesora/preferences.py` & `avendesora-1.9.0/tests/avendesora/preferences.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,21 +28,22 @@
 # but should not be found in the config file
 NONCONFIG_SETTINGS = {
     'config_file': 'config',
     'config_doc_file': 'config.doc',
     'settings_dir': user_config_dir('avendesora'),
     'default_accounts_file': 'accounts.gpg',
     'default_stealth_accounts_file': 'stealth_accounts',
-    'charsets_hash': '82bb252a11ac8b6a9a6830809d181b96',
+    'charsets_hash': '0120b695fb247d4993b1595ab087cc15',
     'dict_hash': '11fe5bc734f4a956c37d7cb3da16ab3f',
-    'secrets_hash': '5fc0355b1c9eb0e885ecc26c28e0c60e',
+    'secrets_hash': 'e038c2a9022b23ac9ceda8645d94816b',
     'discard_logfile': False,
     'commonly_mistaken_attributes': {
         'url': 'urls',
         'alias': 'aliases',
+        'description': 'desc',
     }
 }
 
 
 # Config Settings {{{1
 # These are the default values for settings that may be found in the config file
 CONFIG_DEFAULTS = {
@@ -436,15 +437,15 @@
 
         # Character sets
         exclude, LOWERCASE, UPPERCASE, LETTERS, DIGITS, ALPHANUMERIC,
         HEXDIGITS, PUNCTUATION, SYMBOLS, WHITESPACE, PRINTABLE, DISTINGUISHABLE,
 
         # Secrets
         Password, Passphrase, PIN, Question, MixedPassword, PasswordRecipe,
-        BirthDate,
+        BirthDate, OTP,
 
         # Account Discovery
         RecognizeAll, RecognizeAny, RecognizeTitle, RecognizeURL, RecognizeCWD,
         RecognizeHost, RecognizeUser, RecognizeEnvVar, RecognizeNetwork,
     )
     try:
         # You need to install scrypt using 'pip install scrypt' to use Scrypt
@@ -773,15 +774,15 @@
     #
     #     > base64 -d - < <filename>
     #
     # where <filename> contains <hidden_arg>.
     #
 
     from avendesora import (
-        Hidden, Question, Script,
+        Hidden, Question, Script, OTP,
         RecognizeAll, RecognizeAny, RecognizeTitle, RecognizeURL, RecognizeCWD,
         RecognizeHost, RecognizeUser, RecognizeEnvVar, RecognizeNetwork,
         RecognizeFile
     )
 
     CREATED = '{date}'
     ACCOUNTS = {{
```

### Comparing `avendesora-1.8.0/tests/avendesora/words` & `avendesora-1.9.0/tests/avendesora/words`

 * *Files identical despite different names*

### Comparing `avendesora-1.8.0/tests/avendesora/dictionary.py` & `avendesora-1.9.0/tests/avendesora/dictionary.py`

 * *Files identical despite different names*

### Comparing `avendesora-1.8.0/tests/avendesora/title.py` & `avendesora-1.9.0/tests/avendesora/title.py`

 * *Files identical despite different names*

### Comparing `avendesora-1.8.0/tests/avendesora/generator.py` & `avendesora-1.9.0/tests/avendesora/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,22 +66,22 @@
     # Constructor {{{2
     def __init__(self, init=False, gpg_ids=None):
         # initialize avendesora (these should already be done if called from 
         # main, but it is safe to call them again)
         read_config()
         GnuPG.initialize()
 
-        # check the integrity of avendesora
-        validate_components()
-
         # create the avendesora data directory
         if init:
             self._initialize(gpg_ids, init)
             return
 
+        # check the integrity of avendesora
+        validate_components()
+
         # read the accounts files
         self.shared_secrets = {}
         seen = {}
         most_recently_updated = 0
         for filename in get_setting('accounts_files', []):
             path = to_path(get_setting('settings_dir'), filename)
             updated = os.path.getmtime(str(path.resolve()))
@@ -129,14 +129,20 @@
         def split(s, l=72):
             # Break long string into a series of adjacent shorter strings
             if len(s) < l:
                 return '"%s"' % s
             chunks = ['    "%s"' % s[i:i+l] for i in range(0, len(s), l)]
             return '\n' + '\n'.join(chunks) + '\n'
 
+        # create settings directory if it does not exist
+        settings_dir = to_path(get_setting('settings_dir'))
+        if not settings_dir.exists():
+            settings_dir.mkdir(mode=0o700, parents=True)
+            settings_dir.chmod(0o700)
+
         # Create dictionary of available substitutions for CONTENTS strings
         fields = {}
         for key in CONFIG_DEFAULTS:
             value = get_setting(key, expand=False)
             value = render(str(value) if isinstance(value, Path) else value)
             fields.update({key: value})
         for key in NONCONFIG_SETTINGS:
```

### Comparing `avendesora-1.8.0/tests/avendesora/editors.py` & `avendesora-1.9.0/tests/avendesora/editors.py`

 * *Files identical despite different names*

### Comparing `avendesora-1.8.0/tests/avendesora/writer.py` & `avendesora-1.9.0/tests/avendesora/writer.py`

 * *Files identical despite different names*

### Comparing `avendesora-1.8.0/tests/avendesora/browsers.py` & `avendesora-1.9.0/tests/avendesora/browsers.py`

 * *Files identical despite different names*

### Comparing `avendesora-1.8.0/tests/avendesora/__init__.py` & `avendesora-1.9.0/tests/avendesora/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,23 +6,27 @@
 from .error import PasswordError
 from .generator import PasswordGenerator
 from .obscure import Hide, Hidden, GPG
 try:
     from .obscure import Scrypt
 except ImportError:  # no cover
     pass
+try:
+    from .otp import OTP
+except ImportError:  # no cover
+    pass
 from .recognize import (
     RecognizeAll, RecognizeAny, RecognizeTitle, RecognizeURL, RecognizeCWD,
     RecognizeHost, RecognizeUser, RecognizeEnvVar, RecognizeNetwork,
     RecognizeFile
 )
 from .secrets import (
     Password, Passphrase, PIN, Question, MixedPassword, PasswordRecipe,
     BirthDate, SecretExhausted
 )
 
 # the following are used when generating the documentation and are not needed
 # otherwise
 from . import command
 
-__version__ = '1.8.0'
-__released__ = '2017-11-23'
+__version__ = '1.9.0'
+__released__ = '2017-12-25'
```

### Comparing `avendesora-1.8.0/tests/avendesora/account.py` & `avendesora-1.9.0/tests/avendesora/account.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,17 @@
 from .collection import Collection
 from .config import get_setting
 from .error import PasswordError
 from .obscure import ObscuredSecret
 from .preferences import TOOL_FIELDS
 from .recognize import Recognizer
 from .secrets import GeneratedSecret
+from difflib import get_close_matches
 from inform import (
-    Color, codicil, conjoin, cull, debug, is_collection, is_str, log,
+    Color, codicil, conjoin, cull, debug, full_stop, is_collection, is_str, log,
     notify, output, warn, indent,
     ddd, ppp, vvv
 )
 from textwrap import dedent
 try:
     from urllib.parse import urlparse
 except ImportError:
@@ -211,15 +212,34 @@
     # get_account() {{{2
     @staticmethod
     def get_account(name):
         canonical = canonicalize(name)
         try:
             return Account._accounts[canonical]
         except KeyError:
-            raise PasswordError('account not found.', culprit=name)
+            # account not found, assemble message giving suggested account names
+            names = Account._accounts.keys()
+            candidates = get_close_matches(canonical, names, 9, 0.6)
+
+            # do not want to give multiple options all of which are aliases for
+            # the same accounts, so look for up to three unique accounts
+            accounts = []
+            for candidate in candidates:
+                account = Account._accounts[candidate]
+                if account not in accounts:
+                    accounts.append(account)
+                if len(accounts) >= 3:
+                    break
+
+            # generate the message handling 0, 1, 2 or 3 candidates gracefully
+            msg = ['account not found']
+            candidates = conjoin((a.get_name() for a in accounts), conj=' or ')
+            if candidates:
+                msg.append('did you mean {}?'.format(candidates))
+            raise PasswordError(full_stop(', '.join(msg)), culprit=name)
 
     # get_name() {{{2
     @classmethod
     def get_name(cls):
         """Get account name.
 
         Returns:
@@ -282,15 +302,15 @@
             canonical = canonicalize(name)
             Account._accounts[canonical] = cls
             if canonical in seen:
                 if name == account_name:
                     warn('duplicate account name.', culprit=name)
                 else:
                     warn('alias duplicates existing name.', culprit=name)
-                codicil('Seen in %s in %s.' % seen[name])
+                codicil('Seen in %s in %s.' % seen[canonical])
                 codicil('And in %s in %s.' % (account_name, path))
                 break
             else:
                 new[canonical] = (account_name, path)
         seen.update(new)
             # this two step approach to updating seen prevents us from
             # complaining about aliases that duplicate the account name,
@@ -859,15 +879,15 @@
 
         # select the urls
         if not key:
             key = getattr(cls, 'default_url', None)
         try:
             urls = urls[key]
         except KeyError:
-            keys = cull(urls.keys())
+            keys = cull(list(urls.keys()))
             if keys:
                 if key:
                     msg = 'unknown key, choose from {}.'
                 else:
                     msg = 'key required, choose from {}.'
                 raise PasswordError(msg.format(conjoin(keys)), culprit=key)
             else:
```

### Comparing `avendesora-1.8.0/tests/avendesora/obscure.py` & `avendesora-1.9.0/tests/avendesora/obscure.py`

 * *Files identical despite different names*

### Comparing `avendesora-1.8.0/tests/avendesora/gpg.py` & `avendesora-1.9.0/tests/avendesora/gpg.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # You should have received a copy of the GNU General Public License along with
 # this program.  If not, see http://www.gnu.org/licenses/.
 
 
 # Imports {{{1
 from .config import get_setting, override_setting, setting_path
 from .error import PasswordError
-from shlib import to_path, cp, mkdir
+from shlib import to_path, cp
 from inform import (
     conjoin, cull, display, log, narrate, os_error, warn, is_str,
     full_stop
 )
 import gnupg
 try:
     from StringIO import StringIO   # python2
@@ -85,21 +85,25 @@
     def save(self, contents, gpg_ids=None):
         path = self.path
         if not gpg_ids:
             gpg_ids = get_setting('gpg_ids', [])
         if is_str(gpg_ids):
             gpg_ids = gpg_ids.split()
         if not gpg_ids:
-            raise PasswordError('must specify GPG ID.')
+            # raise PasswordError('must specify GPG ID.')
+            log('no gpg id is available, using symmetric encryption.')
 
         use_gpg, use_armor = self._choices()
         if use_gpg:
             try:
                 encoded = contents.encode(get_setting('encoding'))
-                encrypted = self.gpg.encrypt(encoded, gpg_ids, armor=use_armor)
+                if gpg_ids:
+                    encrypted = self.gpg.encrypt(encoded, gpg_ids, armor=use_armor)
+                else:
+                    encrypted = self.gpg.encrypt(encoded, None, symmetric='AES256', armor=use_armor)
                 if not encrypted.ok:
                     msg = ' '.join(cull([
                         'unable to encrypt.',
                         getattr(encrypted, 'stderr', None)
                     ]))
                     raise PasswordError(msg, culprit=path, sep='\n')
                 else:
@@ -242,21 +246,22 @@
             raise PasswordError(full_stop(e), culprit=error_source())
         ActivePythonFile = None
         return contents
 
     def create(self, contents, gpg_ids):
         path = self.path
         try:
-            mkdir(get_setting('settings_dir'))
+            # check to see if file already exists
             if path.exists():
                 # file creation (init) requested, but file already exists
                 # don't overwrite the file, instead read it so the information 
                 # can be used to create any remaining files.
                 display("%s: already exists." % path)
                 return
+
             # create the file
             display('%s: creating.' % path)
             if path.suffix in ['.gpg', '.asc']:
                 narrate('encrypting.', culprit=path)
                 # encrypt it
                 self.save(contents, gpg_ids)
             else:
```

### Comparing `avendesora-1.8.0/tests/avendesora/utilities.py` & `avendesora-1.9.0/tests/avendesora/utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,18 @@
 
 
 # validate_components {{{1
 def validate_components():
     # check permissions on the settings directory
     path = get_setting('settings_dir')
     mask = get_setting('config_dir_mask')
-    permissions = os.stat(path)[ST_MODE]
+    try:
+        permissions = os.stat(path)[ST_MODE]
+    except FileNotFoundError:
+        raise Error('missing, must run initialize.', culprit=path)
     violation = permissions & mask
     recommended = permissions & ~mask & 0o777
     if violation:
         warn(
             "directory permissions are too loose.",
             "Recommend running 'chmod {:o} {}'.".format(recommended, path),
             culprit=path
```

### Comparing `avendesora-1.8.0/tests/avendesora/secrets.py` & `avendesora-1.9.0/tests/avendesora/secrets.py`

 * *Files identical despite different names*

### Comparing `avendesora-1.8.0/tests/avendesora/recognize.py` & `avendesora-1.9.0/tests/avendesora/recognize.py`

 * *Files identical despite different names*

### Comparing `avendesora-1.8.0/tests/avendesora/config.py` & `avendesora-1.9.0/tests/avendesora/config.py`

 * *Files identical despite different names*

### Comparing `avendesora-1.8.0/tests/avendesora/main.py` & `avendesora-1.9.0/tests/avendesora/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 Generates passwords and pass phrases based on stored account information.
 
 Usage:
     avendesora [options] <command> [<args>...]
 
 Options:
-    -h, --help              Output basic usage information.
+    -h, --help        output basic usage information.
 
 Commands:
 {commands}
 
 Use 'avendesora help <command>' for information on a specific command.
 Use 'avendesora help' for list of available help topics.
 """
@@ -55,18 +55,23 @@
         cmdline = docopt(
             __doc__.format(commands=Command.summarize()),
             options_first=True
         )
 
         # start logging
         logfile = BufferedFile(get_setting('log_file'), True)
-        with Inform(logfile=logfile, hanging_indent=False):
-            Command.execute(cmdline['<command>'], cmdline['<args>'])
-            done()
+        Inform(
+            logfile=logfile, hanging_indent=False, stream_policy='header',
+            notify_if_no_tty=True
+        )
+
+        # run the requested command
+        Command.execute(cmdline['<command>'], cmdline['<args>'])
+        done()
     except KeyboardInterrupt:
-        output('Terminated by user.')
+        output('\nTerminated by user.')
         terminate()
     except (PasswordError, Error) as e:
         e.terminate()
     except OSError as e:
         fatal(os_error(e))
     done()
```

### Comparing `avendesora-1.8.0/tests/avendesora/cursor.py` & `avendesora-1.9.0/tests/avendesora/cursor.py`

 * *Files identical despite different names*

### Comparing `avendesora-1.8.0/tests/avendesora/error.py` & `avendesora-1.9.0/tests/avendesora/error.py`

 * *Files identical despite different names*

### Comparing `avendesora-1.8.0/tests/avendesora/command.py` & `avendesora-1.9.0/tests/avendesora/command.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 from .error import PasswordError
 from .generator import PasswordGenerator
 from .gpg import GnuPG, PythonFile
 from .obscure import ObscuredSecret
 from .utilities import query_user, two_columns
 from .writer import get_writer
 from inform import (
-    codicil, columns, cull, debug, error, full_stop, output, warn, conjoin,
-    os_error, is_collection, indent, render, ddd, ppp, vvv
+    codicil, columns, cull, debug, error, full_stop, join, output, warn,
+    conjoin, os_error, is_collection, indent, render, ddd, ppp, vvv
 )
 from shlib import chmod, cp, rm, to_path
 from docopt import docopt
 from textwrap import dedent
 import re
 import sys
 
@@ -722,18 +722,24 @@
 
         # run the generator
         generator = PasswordGenerator()
 
         # find accounts whose name matches the criteria
         to_print = []
         for acct in generator.find_accounts(cmdline['<text>']):
-            aliases = Collection(getattr(acct, 'aliases', [])).values()
-
-            aliases = ' (%s)' % (', '.join(aliases)) if aliases else ''
-            to_print += [acct.get_name() + aliases]
+            aliases = Collection(getattr(acct, 'aliases', []))
+            desc = getattr(acct, 'desc', None)
+            to_print.append(
+                join(acct.get_name(), aliases=aliases, desc=desc, template=(
+                    '{} ({aliases:\v|, }) -- {desc}',
+                    '{} ({aliases:\v|, })',
+                    '{} -- {desc}',
+                    '{}'
+                ))
+            )
         output(cmdline['<text>']+ ':')
         output('    ' + ('\n    '.join(sorted(to_print))))
 
 
 # Help {{{1
 class Help(Command):
     NAMES = 'help', 'h'
@@ -906,15 +912,15 @@
         # run the generator
         generator = PasswordGenerator(init=True, gpg_ids=gpg_ids)
 
 
 # Log {{{1
 class Log(Command):
     NAMES = 'log',
-    DESCRIPTION = 'open the logfile'
+    DESCRIPTION = 'show the logfile'
     USAGE = dedent("""
         Usage:
             avendesora log
     """).strip()
 
     @classmethod
     def help(cls):
@@ -977,14 +983,18 @@
                 credentials = 'usernames.0 usernames.1 passcode'
 
             If credentials is not specified then the first of the following will
             be used if available:
 
                 id: {idents}
                 secret: {secrets}
+
+            If your credentials include more than one secret they will be
+            presented one at a time for one minute each. You can cut the minute
+            short by typing Ctrl-C.
         """).strip()
         return text.format(
             title=title(cls.DESCRIPTION), usage=cls.USAGE,
             idents=idents, secrets=secrets,
         ).strip()
 
     @classmethod
@@ -997,15 +1007,15 @@
 
         # determine the account and output specified information
         account_name = cmdline['<account>']
         writer = get_writer(tty=True)
         account = generator.get_account(account_name, cmdline['--seed'])
         credentials = account.get_scalar('credentials', default=None)
         if credentials:
-            credentials = Collection(credentials)
+            credentials = credentials.split()
         else:
             ids = Collection(get_setting('credential_ids'))
             secrets = Collection(get_setting('credential_secrets'))
             for each in ids:
                 if account.has_field(each):
                     identity = each
                     break
@@ -1077,19 +1087,19 @@
         generator = PasswordGenerator(
             init=cmdline['<name>'], gpg_ids=sorted(gpg_ids)
         )
 
 
 # Phonetic Alphabet {{{1
 class PhoneticAlphabet(Command):
-    NAMES = 'phonetic alphabet p'.split()
-    DESCRIPTION = 'Display NATO phonetic alphabet.'
+    NAMES = 'phonetic', 'alphabet', 'p'
+    DESCRIPTION = 'display NATO phonetic alphabet'
     USAGE = dedent("""
         Usage:
-            avendesora alphebet [<text>]
+            avendesora alphabet [<text>]
             avendesora phonetic [<text>]
             avendesora p [<text>]
     """).strip()
 
     @classmethod
     def help(cls):
         text = dedent("""
@@ -1106,29 +1116,29 @@
     @classmethod
     def run(cls, command, args):
         words = """
             Alfa Bravo Charlie Delta Echo Foxtrot Golf Hotel India Juliett Kilo
             Lima Mike November Oscar Papa Quebec Romeo Sierra Tango Uniform
             Victor Whiskey X-ray Yankee Zulu
         """.split()
-        mapping = {w[0]:w.lower() for w in words}
+        mapping = {w[0].lower():w for w in words}
         mapping.update({
-            '0':'zero', '1':'one', '2':'two', '3':'three', '4':'four',
-            '5':'five', '6':'six', '7':'seven', '8':'eight', '9':'nine'
+            '0':'Zero', '1':'One', '2':'Two', '3':'Three', '4':'Four',
+            '5':'Five', '6':'Six', '7':'Seven', '8':'Eight', '9':'Nine'
         })
 
         # read command line
         cmdline = docopt(cls.USAGE, argv=[command] + args)
         arg = cmdline['<text>']
 
         if arg:
             converted = []
-            for c in arg:
+            for c in arg.lower():
                 converted.append(mapping.get(c, c))
-            output(' '.join(converted))
+            output(' '.join(converted).lower())
         else:
             output('Phonetic alphabet:')
             output(columns(words))
 
 
 # Reveal {{{1
 class Reveal(Command):
@@ -1197,45 +1207,55 @@
 
         # run the generator
         generator = PasswordGenerator()
 
         # search for accounts that match search criteria
         to_print = []
         for acct in generator.search_accounts(cmdline['<text>']):
-            aliases = ', '.join(Collection(getattr(acct, 'aliases', [])).values())
-            aliases = ' (%s)' % (aliases) if aliases else ''
-            to_print += [acct.get_name() + aliases]
+            aliases = Collection(getattr(acct, 'aliases', []))
+            desc = getattr(acct, 'desc', None)
+            to_print.append(
+                join(acct.get_name(), aliases=aliases, desc=desc, template=(
+                    '{} ({aliases:\v|, }) -- {desc}',
+                    '{} ({aliases:\v|, })',
+                    '{} -- {desc}',
+                    '{}'
+                ))
+            )
         output(cmdline['<text>'] + ':')
         output('    ' + ('\n    '.join(sorted(to_print))))
 
 
 # Value {{{1
 class Value(Command):
-    NAMES = 'value', 'val', 'v'
+    NAMES = 'value', 'val', 'v', 'vc'
     DESCRIPTION = 'show an account value'
     USAGE = dedent("""
         Produce an account value. If the value is secret, it is produced only
         temporarily unless --stdout is specified.
 
         Usage:
             avendesora value [options] [<account> [<field>]]
             avendesora val   [options] [<account> [<field>]]
             avendesora v     [options] [<account> [<field>]]
+            avendesora vc    [options] [<account> [<field>]]
 
         Options:
             -c, --clipboard         Write output to clipboard rather than stdout.
             -s, --stdout            Write output to the standard output without
                                     any annotation or protections.
             -S, --seed              Interactively request additional seed for
                                     generated secrets.
             -v, --verbose           Add additional information to log file to
                                     help identify issues in account discovery.
             -T <title>, --title <title>
                                     Use account discovery on this title.
 
+        The 'vc' command is a shortcut for 'value --clipboard'.
+
         You request a scalar value by specifying its name after the account.
         For example:
 
             avendesora value bank pin
 
         If the requested value is composite (an array or dictionary), you should
         also specify a key that indicates which of the composite values you
@@ -1251,22 +1271,44 @@
         The field may be also be a script, with is nothing but a string that it
         output as given except that embedded attributes are replaced by account
         field values. For example:
 
             avendesora value bank '{accounts.checking}: {passcode}'
 
         If no value is requested the result produced is determined by the value
-        of the 'default' attribute. If no value is given for 'default', then the
-        'passcode' attribute is produced (this can be changed by specifying
-        'default_field' in the config file).  If 'default' is a script (see
-        'avendesora help scripts') then the script is executed. A typical script
-        might be 'username: {username}, password: {passcode}'. It is best if the
-        script produces a one line output if it contains secrets. If not a
-        script, the value of 'default' should be the name of another attribute,
-        and the value of that attribute is shown.
+        of the 'default' attribute (this can be changed by specifying
+        'default_field' in the config file). If no value is given for 'default',
+        then the *passcode*, *password*, or *passphrase* attribute is produced
+        (this can be changed by specifying the 'default_field' in the account or
+        the config file).  If 'default' is a script (see 'avendesora help
+        scripts') then the script is executed. A typical script might be
+        'username: {username}, password: {passcode}'. It is best if the script
+        produces a one line output if it contains secrets. If not a script, the
+        value of 'default' should be the name of another attribute, and the
+        value of that attribute is shown.
+
+        Normally the value command attempts to protects secrets. It does so
+        clearing the screen after a minute. If multiple secrets are requested,
+        you must either wait a minute to see each subsequent secret or type
+        Ctrl-C to clear the current secret and move on.  If you use --clipboard,
+        the clipboard is cleared after a minute.  However, if you use --stdout
+        this clearing of the secret does not occur. The --stdout option is
+        generally used with communicating with other Linux commands.  For
+        example, you can send a passcode to the standard input of a command as
+        follows:
+
+            avendesora value --stdout gpg | gpg --passphrase-fd 0 ...
+
+        You can place the username and password on a command line as follows:
+
+            curl --user `avendesora value -s apache '{username}:{passcode}'` ...
+
+        Be aware that it is possible for other users on shared Linux machines to
+        see the command line arguments of your commands, so passing secrets as
+        command arguments should only be used for low value secrets.
 
         If no account is requested, then Avendesora attempts to determine the
         appropriate account through discovery (see 'avendesora help discovery').
         Normally Avendesora is called in this manner from your window manager.
         You would arrange for it to be run when you type a hot key. In this case
         Avendesora determines which account to use from information available
         from the environment, information like the title on active window. In
@@ -1275,30 +1317,53 @@
         The verbose and title options are used when debugging account
         discovery. The verbose option adds more information about the
         discovery process to the logfile (~/.config/avendesora/log.gpg). The
         title option allows you to override the active window title so you can
         debug title-based discovery. Specifying the title option also scrubs
         the output and outputs directly to the standard output rather than
         mimicking the keyboard so as to avoid exposing your secret.
+
+        If the --stdout option is not specified, the value command still writes
+        to the standard output if it is associated with a TTY (if Avendesora is
+        outputting directly to a terminal). If standard output is not a TTY,
+        Avendesora mimics the keyboard and types the desired value directly into
+        the active window.  There are two common situations where standard
+        output is not a TTY: when Avendesora is being run by your window manager
+        in response to you pressing a hot key or when the output of Avendesora
+        is fed into a pipeline.  In the second case, mimicking the keyboard is
+        not what you want; you should use --stdout to assure the chosen value is
+        sent to the pipeline as desired.
     """).strip()
 
     @classmethod
     def run(cls, command, args):
         # read command line
         cmdline = docopt(cls.USAGE, argv=[command] + args)
+        use_clipboard = cmdline['--clipboard'] or cmdline['vc']
+
+        # mute any warnings if using --stdout
+        try:
+            from inform import get_informer
+            if cmdline['--stdout']:
+                get_informer().suppress_output()
+        except ImportError:
+            # remove this once the version 1.11 of inform is formally released
+            # --KSK
+            pass
+
 
         # run the generator
         generator = PasswordGenerator()
 
         # determine the account and output specified information
         account_name = cmdline['<account>']
         if account_name:
             account = generator.get_account(account_name, cmdline['--seed'])
             writer = get_writer(
-                clipboard=cmdline['--clipboard'], stdout=cmdline['--stdout']
+                clipboard=use_clipboard, stdout=cmdline['--stdout']
             )
             writer.display_field(account, cmdline['<field>'])
         else:
             # use discovery to determine account
             account_name, script = generator.discover_account(
                 title=cmdline['--title'], verbose=cmdline['--verbose']
             )
```

### Comparing `avendesora-1.8.0/tests/avendesora/dialog.py` & `avendesora-1.9.0/tests/avendesora/dialog.py`

 * *Files identical despite different names*

### Comparing `avendesora-1.8.0/tests/avendesora/charsets.py` & `avendesora-1.9.0/tests/avendesora/charsets.py`

 * *Files identical despite different names*

### Comparing `avendesora-1.8.0/tests/avendesora/help.py` & `avendesora-1.9.0/tests/avendesora/help.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,16 +27,18 @@
 # this program.  If not, see http://www.gnu.org/licenses/.
 
 
 # Imports {{{1
 from .browsers import StandardBrowser
 from .command import Command
 from .config import get_setting
+from .error import PasswordError
 from .utilities import pager, two_columns
-from inform import error, output
+from difflib import get_close_matches
+from inform import conjoin, full_stop, output
 from textwrap import dedent
 
 # HelpMessage base class {{{1
 class HelpMessage(object):
     URL = None
 
     # get_name() {{{2
@@ -86,15 +88,26 @@
                     return pager(cmd.help())
             for topic in cls.topics():
                 if name == topic.get_name():
                     if browse:
                         return show_in_browser(topic.URL)
                     else:
                         return pager(topic.help())
-            error('topic not found.', culprit=name)
+
+            # topic not found, give some alternatives
+            topics = (
+                [c.get_name() for c in Command.commands()]
+              + [t.get_name() for t in cls.topics()]
+            )
+            candidates = get_close_matches(name, topics, 3, 0.6)
+            msg = ['topic not found']
+            candidates = conjoin(candidates, conj=' or ')
+            if candidates:
+                msg.append('did you mean {}?'.format(candidates))
+            raise PasswordError(full_stop(', '.join(msg)), culprit=name)
         else:
             if browse:
                 return show_in_browser('')
             cls.help()
 
     # summarize {{{2
     @classmethod
@@ -875,15 +888,15 @@
 
                 > avendesora value <accountname> 0
                 questions.0 (oldest aunt): ampere reimburse duster
 
             You can get a list of your questions so you can identify which index
             to use with:
 
-                > avenedesora values <accountname>
+                > avendesora values <accountname>
                 ...
                 questions:
                     0: oldest aunt <reveal with 'avendesora value <accountname> questions.0'>
                     1: title of first job <reveal with 'avendesora value <accountname> questions.1'>
                     2: oldest uncle <reveal with 'avendesora value <accountname> questions.2'>
                     3: savings goal <reveal with 'avendesora value <accountname> questions.3'>
                     4: childhood vacation spot <reveal with 'avendesora value <accountname> questions.4'>
@@ -1240,15 +1253,15 @@
                 A string that is placed between each symbol in the generated
                 password.
             prefix (str):
                 A string added to the front of the generated password.
             suffix (str):
                 A string added to the end of the generated password.
 
-        Examples:
+        Example:
 
             passcode = Password(10)
 
 
         Passphrase
         ----------
 
@@ -1281,15 +1294,15 @@
                 A string that is placed between each symbol in the generated
                 password.
             prefix (str):
                 A string added to the front of the generated password.
             suffix (str):
                 A string added to the end of the generated password.
 
-        Examples:
+        Example:
 
             passcode = Passphrase()
 
 
         PIN
         ---
 
@@ -1312,15 +1325,15 @@
                 accounts contained in an account file.  This argument overrides
                 that behavior and instead explicitly specifies the master seed
                 for this secret.
             version (str):
                 An optional seed. Changing this value will change the generated
                 PIN.
 
-        Examples:
+        Example:
 
             passcode = PIN()
 
 
         Question
         --------
 
@@ -1364,15 +1377,15 @@
                 A string added to the front of the generated password.
             suffix (str):
                 A string added to the end of the generated password.
             answer:
                 The answer. If provided, this would override the generated
                 answer.  May be a string, or it may be an Obscured object.
 
-        Examples:
+        Example:
 
             questions = [
                 Question('Favorite foreign city'),
                 Question('Favorite breed of dog'),
             ]
 
 
@@ -1423,15 +1436,15 @@
                 answer.
             shift_sort(bool):
                 If true, the characters in the password will be sorted so that
                 the characters that require the shift key when typing are placed
                 last, making it easier to type. Use this option if you expect to
                 be typing the password by hand.
 
-        Examples:
+        Example:
 
             passcode = PasswordRecipe('12 2u 2d 2c!@#$%^&*')
 
 
         BirthDate
         ---------
 
@@ -1460,17 +1473,31 @@
                 accounts contained in an account file.  This argument overrides
                 that behavior and instead explicitly specifies the master seed
                 for this secret.
             version (str):
                 An optional seed. Changing this value will change the generated
                 answer.
 
-        Examples:
+        Example:
 
             birthdate = BirthDate(2015, 21, 55)
+
+
+        OTP
+        ---
+
+        Generates a secret that changes once per minute that generally is used
+        as a second factor when authenticating.  It can act as a replacement
+        for, and is fully compatible with, Google Authenticator.  You would
+        provide the text version of the shared secret (the backup code) that is
+        presented to you when first configuring your second factor authentication.
+
+        Example:
+
+            otp = OTP('JBSWY3DPEHPK3PXP')
         """).strip()
         return text
 
 
 # Stealth class {{{1
 class Stealth(HelpMessage):
     DESCRIPTION = "stealth secrets"
```

### Comparing `avendesora-1.8.0/tests/test_help.py` & `avendesora-1.9.0/tests/test_help.py`

 * *Files 1% similar despite different names*

```diff
@@ -318,14 +318,18 @@
             credentials = 'usernames.0 usernames.1 passcode'
 
         If credentials is not specified then the first of the following will
         be used if available:
 
             id: username or email
             secret: passcode, password or passphrase
+
+        If your credentials include more than one secret they will be
+        presented one at a time for one minute each. You can cut the minute
+        short by typing Ctrl-C.
     """).strip()
     assert result.decode('utf-8') == expected
 
 # test_edit() {{{1
 def test_edit():
     try:
         result = run('avendesora help edit')
@@ -478,15 +482,15 @@
 # test_log() {{{1
 def test_log():
     try:
         result = run('avendesora help log')
     except OSError as err:
         result = os_error(err)
     expected = dedent("""
-        Open the logfile.
+        Show the logfile.
 
         Usage:
             avendesora log
 
         Opens the logfile in your editor.
 
         You can specify the editor by changing the 'edit_account' setting in
@@ -533,15 +537,15 @@
         result = run('avendesora help phonetic')
     except OSError as err:
         result = os_error(err)
     expected = dedent("""
         Display NATO phonetic alphabet.
 
         Usage:
-            avendesora alphebet [<text>]
+            avendesora alphabet [<text>]
             avendesora phonetic [<text>]
             avendesora p [<text>]
 
         If <text> is given, it is converted character by character to the
         phonetic alphabet. If not given, the entire phonetic alphabet is
         displayed.
     """).strip()
@@ -603,26 +607,29 @@
         Produce an account value. If the value is secret, it is produced only
         temporarily unless --stdout is specified.
 
         Usage:
             avendesora value [options] [<account> [<field>]]
             avendesora val   [options] [<account> [<field>]]
             avendesora v     [options] [<account> [<field>]]
+            avendesora vc    [options] [<account> [<field>]]
 
         Options:
             -c, --clipboard         Write output to clipboard rather than stdout.
             -s, --stdout            Write output to the standard output without
                                     any annotation or protections.
             -S, --seed              Interactively request additional seed for
                                     generated secrets.
             -v, --verbose           Add additional information to log file to
                                     help identify issues in account discovery.
             -T <title>, --title <title>
                                     Use account discovery on this title.
 
+        The 'vc' command is a shortcut for 'value --clipboard'.
+
         You request a scalar value by specifying its name after the account.
         For example:
 
             avendesora value bank pin
 
         If the requested value is composite (an array or dictionary), you should
         also specify a key that indicates which of the composite values you
@@ -638,22 +645,44 @@
         The field may be also be a script, with is nothing but a string that it
         output as given except that embedded attributes are replaced by account
         field values. For example:
 
             avendesora value bank '{accounts.checking}: {passcode}'
 
         If no value is requested the result produced is determined by the value
-        of the 'default' attribute. If no value is given for 'default', then the
-        'passcode' attribute is produced (this can be changed by specifying
-        'default_field' in the config file).  If 'default' is a script (see
-        'avendesora help scripts') then the script is executed. A typical script
-        might be 'username: {username}, password: {passcode}'. It is best if the
-        script produces a one line output if it contains secrets. If not a
-        script, the value of 'default' should be the name of another attribute,
-        and the value of that attribute is shown.
+        of the 'default' attribute (this can be changed by specifying
+        'default_field' in the config file). If no value is given for 'default',
+        then the *passcode*, *password*, or *passphrase* attribute is produced
+        (this can be changed by specifying the 'default_field' in the account or
+        the config file).  If 'default' is a script (see 'avendesora help
+        scripts') then the script is executed. A typical script might be
+        'username: {username}, password: {passcode}'. It is best if the script
+        produces a one line output if it contains secrets. If not a script, the
+        value of 'default' should be the name of another attribute, and the
+        value of that attribute is shown.
+
+        Normally the value command attempts to protects secrets. It does so
+        clearing the screen after a minute. If multiple secrets are requested,
+        you must either wait a minute to see each subsequent secret or type
+        Ctrl-C to clear the current secret and move on.  If you use --clipboard,
+        the clipboard is cleared after a minute.  However, if you use --stdout
+        this clearing of the secret does not occur. The --stdout option is
+        generally used with communicating with other Linux commands.  For
+        example, you can send a passcode to the standard input of a command as
+        follows:
+
+            avendesora value --stdout gpg | gpg --passphrase-fd 0 ...
+
+        You can place the username and password on a command line as follows:
+
+            curl --user `avendesora value -s apache '{username}:{passcode}'` ...
+
+        Be aware that it is possible for other users on shared Linux machines to
+        see the command line arguments of your commands, so passing secrets as
+        command arguments should only be used for low value secrets.
 
         If no account is requested, then Avendesora attempts to determine the
         appropriate account through discovery (see 'avendesora help discovery').
         Normally Avendesora is called in this manner from your window manager.
         You would arrange for it to be run when you type a hot key. In this case
         Avendesora determines which account to use from information available
         from the environment, information like the title on active window. In
@@ -662,14 +691,25 @@
         The verbose and title options are used when debugging account
         discovery. The verbose option adds more information about the
         discovery process to the logfile (~/.config/avendesora/log.gpg). The
         title option allows you to override the active window title so you can
         debug title-based discovery. Specifying the title option also scrubs
         the output and outputs directly to the standard output rather than
         mimicking the keyboard so as to avoid exposing your secret.
+
+        If the --stdout option is not specified, the value command still writes
+        to the standard output if it is associated with a TTY (if Avendesora is
+        outputting directly to a terminal). If standard output is not a TTY,
+        Avendesora mimics the keyboard and types the desired value directly into
+        the active window.  There are two common situations where standard
+        output is not a TTY: when Avendesora is being run by your window manager
+        in response to you pressing a hot key or when the output of Avendesora
+        is fed into a pipeline.  In the second case, mimicking the keyboard is
+        not what you want; you should use --stdout to assure the chosen value is
+        sent to the pipeline as desired.
     """).strip()
     assert result.decode('utf-8') == expected
 
 # test_values() {{{1
 def test_values():
     try:
         result = run('avendesora help values')
@@ -1479,15 +1519,15 @@
 
             > avendesora value <accountname> 0
             questions.0 (oldest aunt): ampere reimburse duster
 
         You can get a list of your questions so you can identify which index
         to use with:
 
-            > avenedesora values <accountname>
+            > avendesora values <accountname>
             ...
             questions:
                 0: oldest aunt <reveal with 'avendesora value <accountname> questions.0'>
                 1: title of first job <reveal with 'avendesora value <accountname> questions.1'>
                 2: oldest uncle <reveal with 'avendesora value <accountname> questions.2'>
                 3: savings goal <reveal with 'avendesora value <accountname> questions.3'>
                 4: childhood vacation spot <reveal with 'avendesora value <accountname> questions.4'>
@@ -1802,15 +1842,15 @@
                 A string that is placed between each symbol in the generated
                 password.
             prefix (str):
                 A string added to the front of the generated password.
             suffix (str):
                 A string added to the end of the generated password.
 
-        Examples:
+        Example:
 
             passcode = Password(10)
 
 
         Passphrase
         ----------
 
@@ -1843,15 +1883,15 @@
                 A string that is placed between each symbol in the generated
                 password.
             prefix (str):
                 A string added to the front of the generated password.
             suffix (str):
                 A string added to the end of the generated password.
 
-        Examples:
+        Example:
 
             passcode = Passphrase()
 
 
         PIN
         ---
 
@@ -1874,15 +1914,15 @@
                 accounts contained in an account file.  This argument overrides
                 that behavior and instead explicitly specifies the master seed
                 for this secret.
             version (str):
                 An optional seed. Changing this value will change the generated
                 PIN.
 
-        Examples:
+        Example:
 
             passcode = PIN()
 
 
         Question
         --------
 
@@ -1926,15 +1966,15 @@
                 A string added to the front of the generated password.
             suffix (str):
                 A string added to the end of the generated password.
             answer:
                 The answer. If provided, this would override the generated
                 answer.  May be a string, or it may be an Obscured object.
 
-        Examples:
+        Example:
 
             questions = [
                 Question('Favorite foreign city'),
                 Question('Favorite breed of dog'),
             ]
 
 
@@ -1985,15 +2025,15 @@
                 answer.
             shift_sort(bool):
                 If true, the characters in the password will be sorted so that
                 the characters that require the shift key when typing are placed
                 last, making it easier to type. Use this option if you expect to
                 be typing the password by hand.
 
-        Examples:
+        Example:
 
             passcode = PasswordRecipe('12 2u 2d 2c!@#$%^&*')
 
 
         BirthDate
         ---------
 
@@ -2022,17 +2062,31 @@
                 accounts contained in an account file.  This argument overrides
                 that behavior and instead explicitly specifies the master seed
                 for this secret.
             version (str):
                 An optional seed. Changing this value will change the generated
                 answer.
 
-        Examples:
+        Example:
 
             birthdate = BirthDate(2015, 21, 55)
+
+
+        OTP
+        ---
+
+        Generates a secret that changes once per minute that generally is used
+        as a second factor when authenticating.  It can act as a replacement
+        for, and is fully compatible with, Google Authenticator.  You would
+        provide the text version of the shared secret (the backup code) that is
+        presented to you when first configuring your second factor authentication.
+
+        Example:
+
+            otp = OTP('JBSWY3DPEHPK3PXP')
     """).strip()
     assert result.decode('utf-8') == expected
 
 # test_stealth() {{{1
 def test_stealth():
     try:
         result = run('avendesora help stealth')
```

### Comparing `avendesora-1.8.0/tests/home/.gnupg/random_seed` & `avendesora-1.9.0/tests/home/.gnupg/random_seed`

 * *Files identical despite different names*

### Comparing `avendesora-1.8.0/tests/home/.gnupg/trustdb.gpg` & `avendesora-1.9.0/tests/home/.gnupg/trustdb.gpg`

 * *Files identical despite different names*

### Comparing `avendesora-1.8.0/tests/home/.gnupg/private-keys-v1.d/32489E4B20C131A366C6711687E2712C8C64A62E.key` & `avendesora-1.9.0/tests/home/.gnupg/private-keys-v1.d/32489E4B20C131A366C6711687E2712C8C64A62E.key`

 * *Files identical despite different names*

### Comparing `avendesora-1.8.0/tests/home/.gnupg/private-keys-v1.d/2840F86F07D2EEF141115D06F6B9CD52B4D37F06.key` & `avendesora-1.9.0/tests/home/.gnupg/private-keys-v1.d/2840F86F07D2EEF141115D06F6B9CD52B4D37F06.key`

 * *Files identical despite different names*

### Comparing `avendesora-1.8.0/tests/home/.gnupg/pubring.kbx` & `avendesora-1.9.0/tests/home/.gnupg/pubring.kbx`

 * *Files identical despite different names*

### Comparing `avendesora-1.8.0/tests/home/gnupg/random_seed` & `avendesora-1.9.0/tests/home/gnupg/random_seed`

 * *Files identical despite different names*

### Comparing `avendesora-1.8.0/tests/home/gnupg/trustdb.gpg` & `avendesora-1.9.0/tests/home/gnupg/trustdb.gpg`

 * *Files identical despite different names*

### Comparing `avendesora-1.8.0/tests/home/gnupg/private-keys-v1.d/32489E4B20C131A366C6711687E2712C8C64A62E.key` & `avendesora-1.9.0/tests/home/gnupg/private-keys-v1.d/32489E4B20C131A366C6711687E2712C8C64A62E.key`

 * *Files identical despite different names*

### Comparing `avendesora-1.8.0/tests/home/gnupg/private-keys-v1.d/2840F86F07D2EEF141115D06F6B9CD52B4D37F06.key` & `avendesora-1.9.0/tests/home/gnupg/private-keys-v1.d/2840F86F07D2EEF141115D06F6B9CD52B4D37F06.key`

 * *Files identical despite different names*

### Comparing `avendesora-1.8.0/tests/home/gnupg/pubring.kbx` & `avendesora-1.9.0/tests/home/gnupg/pubring.kbx`

 * *Files identical despite different names*

### Comparing `avendesora-1.8.0/tests/home/.config/avendesora/hashes` & `avendesora-1.9.0/tests/home/.config/avendesora/hashes`

 * *Files identical despite different names*

### Comparing `avendesora-1.8.0/tests/home/.config/avendesora/accounts` & `avendesora-1.9.0/tests/home/.config/avendesora/accounts`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     Account, Hidden, GPG,
 
     # Character sets
     exclude, LOWERCASE, UPPERCASE, LETTERS, DIGITS, ALPHANUMERIC,
     HEXDIGITS, PUNCTUATION, WHITESPACE, PRINTABLE, DISTINGUISHABLE,
 
     # Secrets
-    Password, Passphrase, PIN, Question, MixedPassword, BirthDate,
+    Password, Passphrase, PIN, Question, MixedPassword, BirthDate, OTP,
 
     # Account Discovery
     RecognizeAll, RecognizeAny, RecognizeTitle, RecognizeURL, RecognizeCWD,
     RecognizeHost, RecognizeUser, RecognizeEnvVar,
 )
 
 master_seed = Hidden(
@@ -109,10 +109,11 @@
     ]
     accounts = {
         'checking':   Hidden('MTIzNDU2Nzg='),
         'savings':    Hidden('MjM0NTY3ODk='),
         'creditcard': Hidden('MzQ1Njc4OTA='),
     }
     customer_service = '1-866-229-6633'
+    otp = OTP('JBSWY3DPEHPK3PXP')
 
 # Include a few unicode characters, but to make sure they work: ±αβγδε
 # vim: filetype=python sw=4 sts=4 et ai ff=unix :
```

### Comparing `avendesora-1.8.0/tests/home/.config/avendesora/stealth_accounts` & `avendesora-1.9.0/tests/home/.config/avendesora/stealth_accounts`

 * *Files identical despite different names*

### Comparing `avendesora-1.8.0/tests/home/.config/avendesora/key.gpg` & `avendesora-1.9.0/tests/home/.config/avendesora/key.gpg`

 * *Files identical despite different names*

### Comparing `avendesora-1.8.0/tests/home/.config/avendesora/config` & `avendesora-1.9.0/tests/home/.config/avendesora/config`

 * *Files identical despite different names*

### Comparing `avendesora-1.8.0/tests/home/config/avendesora/hashes` & `avendesora-1.9.0/tests/home/config/avendesora/hashes`

 * *Files identical despite different names*

### Comparing `avendesora-1.8.0/tests/home/config/avendesora/accounts` & `avendesora-1.9.0/tests/home/config/avendesora/accounts`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     Account, Hidden, GPG,
 
     # Character sets
     exclude, LOWERCASE, UPPERCASE, LETTERS, DIGITS, ALPHANUMERIC,
     HEXDIGITS, PUNCTUATION, WHITESPACE, PRINTABLE, DISTINGUISHABLE,
 
     # Secrets
-    Password, Passphrase, PIN, Question, MixedPassword, BirthDate,
+    Password, Passphrase, PIN, Question, MixedPassword, BirthDate, OTP,
 
     # Account Discovery
     RecognizeAll, RecognizeAny, RecognizeTitle, RecognizeURL, RecognizeCWD,
     RecognizeHost, RecognizeUser, RecognizeEnvVar,
 )
 
 master_seed = Hidden(
@@ -109,10 +109,11 @@
     ]
     accounts = {
         'checking':   Hidden('MTIzNDU2Nzg='),
         'savings':    Hidden('MjM0NTY3ODk='),
         'creditcard': Hidden('MzQ1Njc4OTA='),
     }
     customer_service = '1-866-229-6633'
+    otp = OTP('JBSWY3DPEHPK3PXP')
 
 # Include a few unicode characters, but to make sure they work: ±αβγδε
 # vim: filetype=python sw=4 sts=4 et ai ff=unix :
```

### Comparing `avendesora-1.8.0/tests/home/config/avendesora/stealth_accounts` & `avendesora-1.9.0/tests/home/config/avendesora/stealth_accounts`

 * *Files identical despite different names*

### Comparing `avendesora-1.8.0/tests/home/config/avendesora/key.gpg` & `avendesora-1.9.0/tests/home/config/avendesora/key.gpg`

 * *Files identical despite different names*

### Comparing `avendesora-1.8.0/tests/home/config/avendesora/config` & `avendesora-1.9.0/tests/home/config/avendesora/config`

 * *Files identical despite different names*

### Comparing `avendesora-1.8.0/tests/test_api.py` & `avendesora-1.9.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `avendesora-1.8.0/LICENSE` & `avendesora-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `avendesora-1.8.0/PKG-INFO` & `avendesora-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 1.1
 Name: avendesora
-Version: 1.8.0
+Version: 1.9.0
 Summary: A password generator and account manager.
 Home-page: http://nurdletech.com/linux-utilities/avendesora
 Author: Ken Kundert and Kale Kundert
 Author-email: avendesora@nurdletech.com
 License: GPLv3+
 Download-URL: https://github.com/kenkundert/avendesora/tarball/master
 Description-Content-Type: UNKNOWN
-Description: Avendesora Collaborative Password Utility
+Description: Avendesora Collaborative Password Manager
         =========================================
         
         *Avendesora, the leaf of the Tree of Life is the key.*
         
         .. image:: https://img.shields.io/travis/KenKundert/avendesora/master.svg
             :target: https://travis-ci.org/KenKundert/avendesora
         
@@ -25,16 +25,16 @@
         .. image:: https://img.shields.io/pypi/pyversions/avendesora.svg
             :target: https://pypi.python.org/pypi/avendesora/
         
         .. IGNORE: pypi statics are broken and unlikely to be fixed
             .. image:: https://img.shields.io/pypi/dm/avendesora.svg
                 :target: https://pypi.python.org/pypi/avendesora/
         
-        | Version: 1.8.0
-        | Released: 2017-11-23
+        | Version: 1.9.0
+        | Released: 2017-12-25
         |
         
         Avendesora replaces the Abraxas, which are both alternatives to the traditional 
         password vault.
         
         Please report all bugs and suggestions to avendesora@nurdletech.com
         
@@ -98,15 +98,15 @@
         You will also need to install some operating system commands. On Fedora use::
         
            yum install gnupg2 xdotool xsel
         
         You should also install python-gobject. Conceivably this could be installed with 
         the above pip command, but gobject appears broken in pypi, so it is better use 
         the operating system's package manager to install it.  See the setup.py file for 
-        more information.  On Redhat systms use::
+        more information.  On Redhat systems use::
         
            yum install python3-gobject
         
         If you would like to use scrypt as a way of encrypting fields, you will need to 
         install scrypt by hand using::
         
            pip3 install --user scrypt
@@ -464,15 +464,15 @@
         a situation where you need a secret, such as visiting your bank's website in 
         your browser, then you click on the account name field with your mouse and type 
         your hot key. This runs Avendesora without an account name. In this case, 
         Avendesora uses secret discovery to determine which secret to use and the script 
         that should be used to produce the required information. Generally the script 
         would be to enter the account name, then tab, then the password, and finally 
         return, but you can configure the script as you choose. This is all done as part 
-        of configuring discovery. The method for associating Advendesora to a particular 
+        of configuring discovery. The method for associating Avendesora to a particular 
         hot key is dependent on your window manager. With Gnome, it requires that you 
         open your Keyboard Shortcuts preferences and create a new shortcut. When you do 
         this, choose 'avendesora value' as the command to run.
         
         
         Python API
         ----------
@@ -507,15 +507,15 @@
         PasswordGenerator():
             Initializes the password generator. You should pass no arguments.
         
         get_account(name, request_seed=False, stealth_name=None):
             Accesses a particular account. Takes a string for the account name or alias.  
             The name is case insensitive and the '-' may be given for '_'.
         
-            Optionally takes a second argument (*request_seed*) that may be a boolean, 
+            Optionally takes a second argument (*request_seed*) that may be a Boolean, 
             a string, or a function that returns a string. The string is used as an 
             additional seed (see: `avendesora help misdirection`), and if True is passed 
             in, the user in queried for the seed.
         
             The stealth name is used as account name if the account is a stealth 
             account.
         
@@ -523,15 +523,15 @@
         get_name():
             return name of account.
         
         get_value(field):
             Returns the value of a particular account attribute given a user-oriented 
             string that describes the desired attribute.  The value requested must be 
             a scalar value, meaning that you must individually request members of arrays 
-            or dictionary attibutes. Here are some examples that demonstrate the various 
+            or dictionary attributes. Here are some examples that demonstrate the various 
             ways of accessing the various kinds of attributes:
         
             .. code-block:: python
         
                 passcode = account.get_value()
                 username = account.get_value('username')
                 both = account.get_value('username: {username}, password: {passcode}')
@@ -568,15 +568,15 @@
             d (description) and v (value).  A format string does not match it if 
             contains a key for a value that is not available. If no format string 
             matches, the value is returned as a string.  The default formats are ('{f} 
             ({d}): {v}', '{f}: {v}').
         
             If a composite field is requested get_value() raises a PasswordError, and 
             the exception contains the *is_collection* and *collection* attributes. The 
-            first is a boolean and the second is the list of available keys.  
+            first is a Boolean and the second is the list of available keys.  
             PassworError returns None for unknown attributes, so it is always safe to 
             access these attributes without checking whether they exist.
         
         get_values(field):
             Used to get the values for a composite field. It iterates through the value 
             and returns a tuple that contains the key and the value for each item in the 
             field.
@@ -619,15 +619,15 @@
                             lines += indent(
                                 value.render(('{k}) {d}: {v}', '{k}: {v}'))
                             ).split('\n')
                     if keys:
                         value = acct.get_value(name)
                         lines += value.render('{n}: {v}').split('\n')
         
-            get_fields() accepts a boolean argument that if specified and is true will 
+            get_fields() accepts a Boolean argument that if specified and is true will 
             iterate through all fields, including those generally only used by 
             Avendesora, such as aliases and discovery.
         
         
         get_scalar(name, key=None, default=False):
             A lower level interface than get_value that given a name and perhaps a key 
             returns a scalar value.  Also takes an optional default value that is 
@@ -738,16 +738,16 @@
         It is worth browsing all of the available topics at least once to get a sense of 
         all that Avendesora can do.
         
         
         Contributing
         ------------
         
-        Please ask questions or report bugs on ``Github Issues 
-        <https://github.com/KenKundert/avendesora/issues>``_. I will entertain pull 
+        Please ask questions or report bugs on `Github Issues 
+        <https://github.com/KenKundert/avendesora/issues>`_. I will entertain pull 
         requests if you make improvements. I am particularly interested in help adapting 
         *Avendesora* for other editors, window managers and distributions.
         
 Keywords: avendesora,password,XKCD
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `avendesora-1.8.0/setup.py` & `avendesora-1.9.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 with open('README.rst') as file:
     readme = file.read()
 
 setup(
     name = 'avendesora',
-    version = '1.8.0',
+    version = '1.9.0',
     author = 'Ken Kundert and Kale Kundert',
     author_email = 'avendesora@nurdletech.com',
     description = 'A password generator and account manager.',
     long_description = readme,
     url = 'http://nurdletech.com/linux-utilities/avendesora',
     download_url = 'https://github.com/kenkundert/avendesora/tarball/master',
     license = 'GPLv3+',
@@ -20,15 +20,15 @@
     entry_points = {
         'console_scripts': ['avendesora = avendesora.main:main'],
     },
     install_requires = [
         'appdirs',
         'arrow',
         'docopt',
-        'inform>=1.10',
+        'inform>=1.11',
         #'pygobject',
             # pygobject seems broken in pypi. Instead, do the following:
             # git clone git://git.gnome.org/pygobject
             # pip3.5 install ./pygobject
             # This install will fail if you do not have the right packages
             # installed in linux. For example, gnome-common is one that you will
             # need. Read the error messages carefully to determine
@@ -39,14 +39,16 @@
             #     dnf install libffi-devel
             #     dnf install gobject-introspection-devel
             #     dnf install python3-cairo-devel
         'python-gnupg>=0.4.1',
             # Be careful.  There's a package called 'gnupg' that's an 
             # incompatible fork of 'python-gnupg'.  If both are installed, the 
             # user will probably have compatibility issues.
+        'pyotp',
+            # pyotp is optional, it provides OTP secrets.
         #'scrypt',
             # scrypt is optional. If you install it then Avendesora will offer
             # it. It is not required because it involves compiling C code and so
             # significant additional dependencies such as gcc.
         'shlib>=0.7',
     ],
     setup_requires = 'pytest-runner>=2.0'.split(),
```

### Comparing `avendesora-1.8.0/avendesora.egg-info/SOURCES.txt` & `avendesora-1.9.0/avendesora.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 avendesora/editors.py
 avendesora/error.py
 avendesora/generator.py
 avendesora/gpg.py
 avendesora/help.py
 avendesora/main.py
 avendesora/obscure.py
+avendesora/otp.py
 avendesora/preferences.py
 avendesora/recognize.py
 avendesora/secrets.py
 avendesora/title.py
 avendesora/utilities.py
 avendesora/words
 avendesora/writer.py
@@ -50,14 +51,15 @@
 tests/avendesora/editors.py
 tests/avendesora/error.py
 tests/avendesora/generator.py
 tests/avendesora/gpg.py
 tests/avendesora/help.py
 tests/avendesora/main.py
 tests/avendesora/obscure.py
+tests/avendesora/otp.py
 tests/avendesora/preferences.py
 tests/avendesora/recognize.py
 tests/avendesora/secrets.py
 tests/avendesora/title.py
 tests/avendesora/utilities.py
 tests/avendesora/words
 tests/avendesora/writer.py
```

### Comparing `avendesora-1.8.0/avendesora.egg-info/PKG-INFO` & `avendesora-1.9.0/avendesora.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 1.1
 Name: avendesora
-Version: 1.8.0
+Version: 1.9.0
 Summary: A password generator and account manager.
 Home-page: http://nurdletech.com/linux-utilities/avendesora
 Author: Ken Kundert and Kale Kundert
 Author-email: avendesora@nurdletech.com
 License: GPLv3+
 Download-URL: https://github.com/kenkundert/avendesora/tarball/master
 Description-Content-Type: UNKNOWN
-Description: Avendesora Collaborative Password Utility
+Description: Avendesora Collaborative Password Manager
         =========================================
         
         *Avendesora, the leaf of the Tree of Life is the key.*
         
         .. image:: https://img.shields.io/travis/KenKundert/avendesora/master.svg
             :target: https://travis-ci.org/KenKundert/avendesora
         
@@ -25,16 +25,16 @@
         .. image:: https://img.shields.io/pypi/pyversions/avendesora.svg
             :target: https://pypi.python.org/pypi/avendesora/
         
         .. IGNORE: pypi statics are broken and unlikely to be fixed
             .. image:: https://img.shields.io/pypi/dm/avendesora.svg
                 :target: https://pypi.python.org/pypi/avendesora/
         
-        | Version: 1.8.0
-        | Released: 2017-11-23
+        | Version: 1.9.0
+        | Released: 2017-12-25
         |
         
         Avendesora replaces the Abraxas, which are both alternatives to the traditional 
         password vault.
         
         Please report all bugs and suggestions to avendesora@nurdletech.com
         
@@ -98,15 +98,15 @@
         You will also need to install some operating system commands. On Fedora use::
         
            yum install gnupg2 xdotool xsel
         
         You should also install python-gobject. Conceivably this could be installed with 
         the above pip command, but gobject appears broken in pypi, so it is better use 
         the operating system's package manager to install it.  See the setup.py file for 
-        more information.  On Redhat systms use::
+        more information.  On Redhat systems use::
         
            yum install python3-gobject
         
         If you would like to use scrypt as a way of encrypting fields, you will need to 
         install scrypt by hand using::
         
            pip3 install --user scrypt
@@ -464,15 +464,15 @@
         a situation where you need a secret, such as visiting your bank's website in 
         your browser, then you click on the account name field with your mouse and type 
         your hot key. This runs Avendesora without an account name. In this case, 
         Avendesora uses secret discovery to determine which secret to use and the script 
         that should be used to produce the required information. Generally the script 
         would be to enter the account name, then tab, then the password, and finally 
         return, but you can configure the script as you choose. This is all done as part 
-        of configuring discovery. The method for associating Advendesora to a particular 
+        of configuring discovery. The method for associating Avendesora to a particular 
         hot key is dependent on your window manager. With Gnome, it requires that you 
         open your Keyboard Shortcuts preferences and create a new shortcut. When you do 
         this, choose 'avendesora value' as the command to run.
         
         
         Python API
         ----------
@@ -507,15 +507,15 @@
         PasswordGenerator():
             Initializes the password generator. You should pass no arguments.
         
         get_account(name, request_seed=False, stealth_name=None):
             Accesses a particular account. Takes a string for the account name or alias.  
             The name is case insensitive and the '-' may be given for '_'.
         
-            Optionally takes a second argument (*request_seed*) that may be a boolean, 
+            Optionally takes a second argument (*request_seed*) that may be a Boolean, 
             a string, or a function that returns a string. The string is used as an 
             additional seed (see: `avendesora help misdirection`), and if True is passed 
             in, the user in queried for the seed.
         
             The stealth name is used as account name if the account is a stealth 
             account.
         
@@ -523,15 +523,15 @@
         get_name():
             return name of account.
         
         get_value(field):
             Returns the value of a particular account attribute given a user-oriented 
             string that describes the desired attribute.  The value requested must be 
             a scalar value, meaning that you must individually request members of arrays 
-            or dictionary attibutes. Here are some examples that demonstrate the various 
+            or dictionary attributes. Here are some examples that demonstrate the various 
             ways of accessing the various kinds of attributes:
         
             .. code-block:: python
         
                 passcode = account.get_value()
                 username = account.get_value('username')
                 both = account.get_value('username: {username}, password: {passcode}')
@@ -568,15 +568,15 @@
             d (description) and v (value).  A format string does not match it if 
             contains a key for a value that is not available. If no format string 
             matches, the value is returned as a string.  The default formats are ('{f} 
             ({d}): {v}', '{f}: {v}').
         
             If a composite field is requested get_value() raises a PasswordError, and 
             the exception contains the *is_collection* and *collection* attributes. The 
-            first is a boolean and the second is the list of available keys.  
+            first is a Boolean and the second is the list of available keys.  
             PassworError returns None for unknown attributes, so it is always safe to 
             access these attributes without checking whether they exist.
         
         get_values(field):
             Used to get the values for a composite field. It iterates through the value 
             and returns a tuple that contains the key and the value for each item in the 
             field.
@@ -619,15 +619,15 @@
                             lines += indent(
                                 value.render(('{k}) {d}: {v}', '{k}: {v}'))
                             ).split('\n')
                     if keys:
                         value = acct.get_value(name)
                         lines += value.render('{n}: {v}').split('\n')
         
-            get_fields() accepts a boolean argument that if specified and is true will 
+            get_fields() accepts a Boolean argument that if specified and is true will 
             iterate through all fields, including those generally only used by 
             Avendesora, such as aliases and discovery.
         
         
         get_scalar(name, key=None, default=False):
             A lower level interface than get_value that given a name and perhaps a key 
             returns a scalar value.  Also takes an optional default value that is 
@@ -738,16 +738,16 @@
         It is worth browsing all of the available topics at least once to get a sense of 
         all that Avendesora can do.
         
         
         Contributing
         ------------
         
-        Please ask questions or report bugs on ``Github Issues 
-        <https://github.com/KenKundert/avendesora/issues>``_. I will entertain pull 
+        Please ask questions or report bugs on `Github Issues 
+        <https://github.com/KenKundert/avendesora/issues>`_. I will entertain pull 
         requests if you make improvements. I am particularly interested in help adapting 
         *Avendesora* for other editors, window managers and distributions.
         
 Keywords: avendesora,password,XKCD
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

