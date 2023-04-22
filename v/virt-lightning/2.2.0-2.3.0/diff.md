# Comparing `tmp/virt-lightning-2.2.0.tar.gz` & `tmp/virt-lightning-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "virt-lightning-2.2.0.tar", last modified: Tue Aug 23 16:36:59 2022, max compression
+gzip compressed data, was "virt-lightning-2.3.0.tar", last modified: Sat Apr 22 23:05:16 2023, max compression
```

## Comparing `virt-lightning-2.2.0.tar` & `virt-lightning-2.3.0.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2022-08-23 16:36:59.104854 virt-lightning-2.2.0/
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2022-08-23 16:36:59.098854 virt-lightning-2.2.0/.github/
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2022-08-23 16:36:59.100854 virt-lightning-2.2.0/.github/workflows/
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1176 2022-08-23 15:36:19.000000 virt-lightning-2.2.0/.github/workflows/tests.yml
--rw-r--r--   0 goneri    (1002) goneri    (1002)      897 2022-07-14 16:24:35.000000 virt-lightning-2.2.0/.gitignore
--rw-r--r--   0 goneri    (1002) goneri    (1002)      272 2022-07-14 16:24:35.000000 virt-lightning-2.2.0/DEBUGGING.md
--rw-r--r--   0 goneri    (1002) goneri    (1002)    11358 2022-03-13 22:53:30.000000 virt-lightning-2.2.0/LICENSE-2.0.txt
--rw-r--r--   0 goneri    (1002) goneri    (1002)       97 2022-07-14 16:24:35.000000 virt-lightning-2.2.0/MANIFEST.in
--rw-r--r--   0 goneri    (1002) goneri    (1002)     8100 2022-08-23 16:36:59.104854 virt-lightning-2.2.0/PKG-INFO
--rw-r--r--   0 goneri    (1002) goneri    (1002)     7285 2022-07-22 17:36:35.000000 virt-lightning-2.2.0/README.md
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1402 2022-07-22 17:36:35.000000 virt-lightning-2.2.0/azure-pipelines.yml
--rw-r--r--   0 goneri    (1002) goneri    (1002)     2690 2022-08-23 15:41:22.000000 virt-lightning-2.2.0/changelog.md
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2022-08-23 16:36:59.100854 virt-lightning-2.2.0/conf/
--rw-r--r--   0 goneri    (1002) goneri    (1002)       67 2022-03-13 22:53:30.000000 virt-lightning-2.2.0/conf/example.ini
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2022-08-23 16:36:59.101854 virt-lightning-2.2.0/logo/
--rw-r--r--   0 goneri    (1002) goneri    (1002)    19245 2022-07-14 16:24:35.000000 virt-lightning-2.2.0/logo/logo.png
--rw-r--r--   0 goneri    (1002) goneri    (1002)    13991 2022-07-14 16:24:35.000000 virt-lightning-2.2.0/logo/logo.svg
--rw-r--r--   0 goneri    (1002) goneri    (1002)    11483 2022-07-14 16:24:35.000000 virt-lightning-2.2.0/logo/logo_no_text.png
--rw-r--r--   0 goneri    (1002) goneri    (1002)       28 2022-07-14 16:24:35.000000 virt-lightning-2.2.0/requirements.txt
--rw-r--r--   0 goneri    (1002) goneri    (1002)       38 2022-08-23 16:36:59.104854 virt-lightning-2.2.0/setup.cfg
--rw-r--r--   0 goneri    (1002) goneri    (1002)     2432 2022-08-23 15:42:14.000000 virt-lightning-2.2.0/setup.py
--rw-r--r--   0 goneri    (1002) goneri    (1002)      419 2022-07-14 16:24:35.000000 virt-lightning-2.2.0/test-requirements.txt
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2022-08-23 16:36:59.101854 virt-lightning-2.2.0/tests/
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1881 2022-07-14 16:24:35.000000 virt-lightning-2.2.0/tests/conftest.py
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1033 2022-07-14 16:24:35.000000 virt-lightning-2.2.0/tests/test_configure.py
--rw-r--r--   0 goneri    (1002) goneri    (1002)      820 2022-07-14 16:24:35.000000 virt-lightning-2.2.0/tests/test_domain.py
--rw-r--r--   0 goneri    (1002) goneri    (1002)     2547 2022-07-14 16:24:35.000000 virt-lightning-2.2.0/tests/test_hv.py
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2022-08-23 16:36:59.101854 virt-lightning-2.2.0/tools/
--rw-r--r--   0 goneri    (1002) goneri    (1002)      202 2022-07-14 16:24:35.000000 virt-lightning-2.2.0/tools/release
--rw-r--r--   0 goneri    (1002) goneri    (1002)      910 2022-07-14 16:24:35.000000 virt-lightning-2.2.0/tox.ini
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2022-08-23 16:36:59.102854 virt-lightning-2.2.0/virt-lightning.org/
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1450 2022-07-14 16:24:35.000000 virt-lightning-2.2.0/virt-lightning.org/bench_images_startup.py
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2022-08-23 16:36:59.098854 virt-lightning-2.2.0/virt-lightning.org/etc/
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2022-08-23 16:36:59.098854 virt-lightning-2.2.0/virt-lightning.org/etc/caddy/
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2022-08-23 16:36:59.102854 virt-lightning-2.2.0/virt-lightning.org/etc/caddy/conf.d/
--rw-r--r--   0 goneri    (1002) goneri    (1002)    12732 2022-07-22 17:36:35.000000 virt-lightning-2.2.0/virt-lightning.org/etc/caddy/conf.d/virt-lightning.org.conf
--rwxr-xr-x   0 goneri    (1002) goneri    (1002)      252 2022-07-14 16:24:35.000000 virt-lightning-2.2.0/virt-lightning.org/update.sh
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2022-08-23 16:36:59.098854 virt-lightning-2.2.0/virt-lightning.org/www/
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2022-08-23 16:36:59.102854 virt-lightning-2.2.0/virt-lightning.org/www/images/
--rw-r--r--   0 goneri    (1002) goneri    (1002)      668 2022-07-22 17:36:35.000000 virt-lightning-2.2.0/virt-lightning.org/www/images/index.md
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2022-08-23 16:36:59.103854 virt-lightning-2.2.0/virt_lightning/
--rw-r--r--   0 goneri    (1002) goneri    (1002)      101 2022-07-14 16:24:35.000000 virt-lightning-2.2.0/virt_lightning/__init__.py
--rw-r--r--   0 goneri    (1002) goneri    (1002)    17174 2022-07-22 17:36:35.000000 virt-lightning-2.2.0/virt_lightning/api.py
--rw-r--r--   0 goneri    (1002) goneri    (1002)     2386 2022-07-14 16:24:35.000000 virt-lightning-2.2.0/virt_lightning/configuration.py
--rw-r--r--   0 goneri    (1002) goneri    (1002)    13353 2022-07-14 16:24:35.000000 virt-lightning-2.2.0/virt_lightning/shell.py
--rw-r--r--   0 goneri    (1002) goneri    (1002)      642 2022-07-14 16:24:35.000000 virt-lightning-2.2.0/virt_lightning/symbols.py
--rw-r--r--   0 goneri    (1002) goneri    (1002)     2961 2022-07-14 16:24:35.000000 virt-lightning-2.2.0/virt_lightning/templates.py
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1313 2022-07-14 16:24:35.000000 virt-lightning-2.2.0/virt_lightning/ui.py
--rw-r--r--   0 goneri    (1002) goneri    (1002)      176 2022-08-23 16:36:59.000000 virt-lightning-2.2.0/virt_lightning/version.py
--rw-r--r--   0 goneri    (1002) goneri    (1002)    34959 2022-07-14 20:40:56.000000 virt-lightning-2.2.0/virt_lightning/virt_lightning.py
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2022-08-23 16:36:59.104854 virt-lightning-2.2.0/virt_lightning.egg-info/
--rw-r--r--   0 goneri    (1002) goneri    (1002)     8100 2022-08-23 16:36:59.000000 virt-lightning-2.2.0/virt_lightning.egg-info/PKG-INFO
--rw-r--r--   0 goneri    (1002) goneri    (1002)      979 2022-08-23 16:36:59.000000 virt-lightning-2.2.0/virt_lightning.egg-info/SOURCES.txt
--rw-r--r--   0 goneri    (1002) goneri    (1002)        1 2022-08-23 16:36:59.000000 virt-lightning-2.2.0/virt_lightning.egg-info/dependency_links.txt
--rw-r--r--   0 goneri    (1002) goneri    (1002)       92 2022-08-23 16:36:59.000000 virt-lightning-2.2.0/virt_lightning.egg-info/entry_points.txt
--rw-r--r--   0 goneri    (1002) goneri    (1002)       28 2022-08-23 16:36:59.000000 virt-lightning-2.2.0/virt_lightning.egg-info/requires.txt
--rw-r--r--   0 goneri    (1002) goneri    (1002)       15 2022-08-23 16:36:59.000000 virt-lightning-2.2.0/virt_lightning.egg-info/top_level.txt
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-04-22 23:05:16.377391 virt-lightning-2.3.0/
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-04-22 23:05:16.367391 virt-lightning-2.3.0/.github/
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-04-22 23:05:16.371391 virt-lightning-2.3.0/.github/workflows/
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      836 2023-02-09 19:11:48.000000 virt-lightning-2.3.0/.github/workflows/codeql.yml
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      162 2023-04-19 20:57:19.000000 virt-lightning-2.3.0/.github/workflows/ruff.yml
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     1176 2022-08-23 15:36:19.000000 virt-lightning-2.3.0/.github/workflows/tests.yml
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      643 2023-04-22 22:23:27.000000 virt-lightning-2.3.0/.github/workflows/tox.yml
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      897 2022-07-14 16:24:35.000000 virt-lightning-2.3.0/.gitignore
+-rw-r--r--   0 goneri    (1002) goneri    (1002)    11358 2022-03-13 22:53:30.000000 virt-lightning-2.3.0/LICENSE-2.0.txt
+-rw-r--r--   0 goneri    (1002) goneri    (1002)       97 2022-07-14 16:24:35.000000 virt-lightning-2.3.0/MANIFEST.in
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     7928 2023-04-22 23:05:16.376391 virt-lightning-2.3.0/PKG-INFO
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     7285 2023-02-09 19:11:17.000000 virt-lightning-2.3.0/README.md
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     3048 2023-04-22 23:04:32.000000 virt-lightning-2.3.0/changelog.md
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-04-22 23:05:16.371391 virt-lightning-2.3.0/conf/
+-rw-r--r--   0 goneri    (1002) goneri    (1002)       67 2022-03-13 22:53:30.000000 virt-lightning-2.3.0/conf/example.ini
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-04-22 23:05:16.372391 virt-lightning-2.3.0/logo/
+-rw-r--r--   0 goneri    (1002) goneri    (1002)    19245 2022-07-14 16:24:35.000000 virt-lightning-2.3.0/logo/logo.png
+-rw-r--r--   0 goneri    (1002) goneri    (1002)    13991 2022-07-14 16:24:35.000000 virt-lightning-2.3.0/logo/logo.svg
+-rw-r--r--   0 goneri    (1002) goneri    (1002)    11483 2022-07-14 16:24:35.000000 virt-lightning-2.3.0/logo/logo_no_text.png
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     1583 2023-04-22 22:19:39.000000 virt-lightning-2.3.0/pyproject.toml
+-rw-r--r--   0 goneri    (1002) goneri    (1002)       28 2022-07-14 16:24:35.000000 virt-lightning-2.3.0/requirements.txt
+-rw-r--r--   0 goneri    (1002) goneri    (1002)       38 2023-04-22 23:05:16.377391 virt-lightning-2.3.0/setup.cfg
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      419 2022-07-14 16:24:35.000000 virt-lightning-2.3.0/test-requirements.txt
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-04-22 23:05:16.372391 virt-lightning-2.3.0/tests/
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     1860 2023-04-19 21:06:34.000000 virt-lightning-2.3.0/tests/conftest.py
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      924 2023-04-19 21:06:34.000000 virt-lightning-2.3.0/tests/test_configure.py
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      734 2023-04-19 20:24:56.000000 virt-lightning-2.3.0/tests/test_domain.py
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     2445 2023-04-19 20:58:26.000000 virt-lightning-2.3.0/tests/test_hv.py
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-04-22 23:05:16.373391 virt-lightning-2.3.0/tools/
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      202 2022-07-14 16:24:35.000000 virt-lightning-2.3.0/tools/release
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     1044 2023-04-22 23:01:48.000000 virt-lightning-2.3.0/tox.ini
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-04-22 23:05:16.373391 virt-lightning-2.3.0/virt-lightning.org/
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     1486 2023-04-19 20:31:07.000000 virt-lightning-2.3.0/virt-lightning.org/bench_images_startup.py
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-04-22 23:05:16.367391 virt-lightning-2.3.0/virt-lightning.org/etc/
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-04-22 23:05:16.368391 virt-lightning-2.3.0/virt-lightning.org/etc/caddy/
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-04-22 23:05:16.373391 virt-lightning-2.3.0/virt-lightning.org/etc/caddy/conf.d/
+-rw-r--r--   0 goneri    (1002) goneri    (1002)    15852 2023-04-22 20:00:54.000000 virt-lightning-2.3.0/virt-lightning.org/etc/caddy/conf.d/virt-lightning.org.conf
+-rwxr-xr-x   0 goneri    (1002) goneri    (1002)      252 2022-07-14 16:24:35.000000 virt-lightning-2.3.0/virt-lightning.org/update.sh
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-04-22 23:05:16.368391 virt-lightning-2.3.0/virt-lightning.org/www/
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-04-22 23:05:16.374391 virt-lightning-2.3.0/virt-lightning.org/www/images/
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      861 2023-04-22 20:00:54.000000 virt-lightning-2.3.0/virt-lightning.org/www/images/index.md
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-04-22 23:05:16.375391 virt-lightning-2.3.0/virt_lightning/
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      101 2022-07-14 16:24:35.000000 virt-lightning-2.3.0/virt_lightning/__init__.py
+-rw-r--r--   0 goneri    (1002) goneri    (1002)    17120 2023-04-22 22:19:34.000000 virt-lightning-2.3.0/virt_lightning/api.py
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     2386 2022-07-14 16:24:35.000000 virt-lightning-2.3.0/virt_lightning/configuration.py
+-rw-r--r--   0 goneri    (1002) goneri    (1002)    13492 2023-04-22 22:19:34.000000 virt-lightning-2.3.0/virt_lightning/shell.py
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      642 2022-07-14 16:24:35.000000 virt-lightning-2.3.0/virt_lightning/symbols.py
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     2953 2023-04-19 20:38:48.000000 virt-lightning-2.3.0/virt_lightning/templates.py
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     1313 2023-02-09 19:11:20.000000 virt-lightning-2.3.0/virt_lightning/ui.py
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      160 2023-04-22 23:05:16.000000 virt-lightning-2.3.0/virt_lightning/version.py
+-rw-r--r--   0 goneri    (1002) goneri    (1002)    35300 2023-04-22 22:19:34.000000 virt-lightning-2.3.0/virt_lightning/virt_lightning.py
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-04-22 23:05:16.376391 virt-lightning-2.3.0/virt_lightning.egg-info/
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     7928 2023-04-22 23:05:16.000000 virt-lightning-2.3.0/virt_lightning.egg-info/PKG-INFO
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     1034 2023-04-22 23:05:16.000000 virt-lightning-2.3.0/virt_lightning.egg-info/SOURCES.txt
+-rw-r--r--   0 goneri    (1002) goneri    (1002)        1 2023-04-22 23:05:16.000000 virt-lightning-2.3.0/virt_lightning.egg-info/dependency_links.txt
+-rw-r--r--   0 goneri    (1002) goneri    (1002)       92 2023-04-22 23:05:16.000000 virt-lightning-2.3.0/virt_lightning.egg-info/entry_points.txt
+-rw-r--r--   0 goneri    (1002) goneri    (1002)       40 2023-04-22 23:05:16.000000 virt-lightning-2.3.0/virt_lightning.egg-info/requires.txt
+-rw-r--r--   0 goneri    (1002) goneri    (1002)       15 2023-04-22 23:05:16.000000 virt-lightning-2.3.0/virt_lightning.egg-info/top_level.txt
```

### Comparing `virt-lightning-2.2.0/.github/workflows/tests.yml` & `virt-lightning-2.3.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `virt-lightning-2.2.0/.gitignore` & `virt-lightning-2.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `virt-lightning-2.2.0/LICENSE-2.0.txt` & `virt-lightning-2.3.0/LICENSE-2.0.txt`

 * *Files identical despite different names*

### Comparing `virt-lightning-2.2.0/PKG-INFO` & `virt-lightning-2.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,22 @@
 Metadata-Version: 2.1
 Name: virt-lightning
-Version: 2.2.0
+Version: 2.3.0
 Summary: Deploy your testing VM in a couple of seconds
-Home-page: https://virt-lightning.org
-Author: Gonéri Le Bouder
-Author-email: goneri@lebouder.net
-License: Apache v2.0
-Platform: linux
+Author-email: Gonéri Le Bouder <goneri@lebouder.net>
+Project-URL: Homepage, https://https://virt-lightning.org/
+Project-URL: Source, https://github.com/virt-lightning/virt-lightning
+Keywords: libvirt,cloud,qemu,cloudinit
 Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Topic :: System :: Distributed Computing
+Classifier: Operating System :: POSIX :: Linux
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: test
 License-File: LICENSE-2.0.txt
 
 # 🗲 spawn Cloud instances on libvirt!🗲
 
 
 [![Build Status](https://travis-ci.org/virt-lightning/virt-lightning.svg?branch=master)](https://travis-ci.org/virt-lightning/virt-lightning)
 [![PyPI version](https://badge.fury.io/py/virt-lightning.svg)](https://badge.fury.io/py/virt-lightning)
```

### Comparing `virt-lightning-2.2.0/README.md` & `virt-lightning-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `virt-lightning-2.2.0/changelog.md` & `virt-lightning-2.3.0/changelog.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+# 2.3.0
+
+- tox: add "build" target
+- run tox with Github Action
+- move from setup.py to pyproject.toml
+- cloudinit: add a workaround for the DNS and Fedora
+- github: add a ruff-based test
+- Add CodeQL workflow for GitHub code scanning (#257)
+- Set the Source project URL in setup.py
+- reindent with black
+- Implement disk size parameter for 'start' command
+
 # 2.2.0
 
 - Cosmetic documentation changes
 - Don't try to fetch an image that already exists
 - Add ability to boot old system with no virtio support
 - Use Libvirt default settings when possible
 - Use the VNC display by default
```

### Comparing `virt-lightning-2.2.0/logo/logo.png` & `virt-lightning-2.3.0/logo/logo.png`

 * *Files identical despite different names*

### Comparing `virt-lightning-2.2.0/logo/logo.svg` & `virt-lightning-2.3.0/logo/logo.svg`

 * *Files identical despite different names*

### Comparing `virt-lightning-2.2.0/logo/logo_no_text.png` & `virt-lightning-2.3.0/logo/logo_no_text.png`

 * *Files identical despite different names*

### Comparing `virt-lightning-2.2.0/tests/conftest.py` & `virt-lightning-2.3.0/tests/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-import pytest
+import pathlib
+from unittest.mock import Mock, patch
 
 import libvirt
+import pytest
+
 import virt_lightning.virt_lightning as vl
-import pathlib
-from unittest.mock import patch
-from unittest.mock import Mock
 
 DEFAULT_INI = """
 [main]
 root_password=boby
 """
 
 
-
 def clean_up():
     conn = libvirt.open("test:///default")
     domainIDs = conn.listDomainsID()
     for domainID in domainIDs:
         dom = conn.lookupByID(domainID)
         if dom.state() != libvirt.VIR_DOMAIN_SHUTOFF:
             dom.destroy()
@@ -24,52 +23,56 @@
 
 
 @pytest.fixture
 def hv(scope="function"):
     conn = libvirt.open("test:///default")
     conn.getURI = Mock(return_value="qemu:///system")
     hv = vl.LibvirtHypervisor(conn)
-    with patch.object(pathlib.Path, 'exists') as mock_exists:
+    with patch.object(pathlib.Path, "exists") as mock_exists:
         mock_exists.return_value = False
         hv.init_storage_pool("foo_bar")
     hv.get_qcow_virtual_size = Mock(return_value=2)
     hv.init_network("my_network", "1.0.0.0/24")
     yield hv
     clean_up()
 
 
 @pytest.fixture
 def domain(hv, scope="function"):
     yield hv.create_domain(name="a", distro="b")
     clean_up()
 
+
 @pytest.fixture(autouse=True)
 def kvm_binaries(tmp_path):
     kvm_f = tmp_path / "kvm-dummy"
-    with kvm_f.open(mode='wt') as fd:
+    with kvm_f.open(mode="wt") as fd:
         fd.write("aa")
     vl.KVM_BINARIES = (kvm_f,)
 
+
 @pytest.fixture(autouse=True)
 def qemu_dir(tmp_path):
     qemu_dir = tmp_path / "kvm-dummy"
     if not qemu_dir.exists():
         qemu_dir.mkdir()
     vl.QEMU_DIR = str(qemu_dir)
 
+
 @pytest.fixture(autouse=True)
 def storage_dir(tmp_path):
     pool_dir = tmp_path / "pool"
     upstream_dir = pool_dir / "upstream"
     if not pool_dir.exists():
         pool_dir.mkdir()
     if not upstream_dir.exists():
         upstream_dir.mkdir()
     vl.DEFAULT_STORAGE_DIR = str(pool_dir)
 
+
 @pytest.fixture
 def config_file(tmp_path):
     d = tmp_path / "sub"
     d.mkdir()
     config_file = d / "my_inifile.ini"
     config_file.write_text(DEFAULT_INI)
     return config_file
```

### Comparing `virt-lightning-2.2.0/tests/test_configure.py` & `virt-lightning-2.3.0/tests/test_configure.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,25 @@
 from pathlib import Path
 
 import virt_lightning.configuration
 
+
 def test_default(monkeypatch):
     with monkeypatch.context() as m:
-        m.setattr(
-            virt_lightning.configuration,
-            "DEFAULT_CONFIGFILE",
-            Path("a"))
+        m.setattr(virt_lightning.configuration, "DEFAULT_CONFIGFILE", Path("a"))
         config = virt_lightning.configuration.Configuration()
         assert config.root_password == "root"
 
+
 def test_load_file(monkeypatch, config_file):
     with monkeypatch.context() as m:
-        m.setattr(
-            virt_lightning.configuration,
-            "DEFAULT_CONFIGFILE",
-            Path("a"))
+        m.setattr(virt_lightning.configuration, "DEFAULT_CONFIGFILE", Path("a"))
         config = virt_lightning.configuration.Configuration()
         config.load_file(config_file)
         assert config.root_password == "boby"
 
 
 def test_load_default_config_file(monkeypatch, config_file):
     with monkeypatch.context() as m:
-        m.setattr(
-            virt_lightning.configuration,
-            "DEFAULT_CONFIGFILE",
-            config_file)
+        m.setattr(virt_lightning.configuration, "DEFAULT_CONFIGFILE", config_file)
         config = virt_lightning.configuration.Configuration()
         assert config.root_password == "boby"
```

### Comparing `virt-lightning-2.2.0/tests/test_domain.py` & `virt-lightning-2.3.0/tests/test_domain.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,7 @@
-import virt_lightning
-
-import pathlib
-from unittest.mock import patch
-import libvirt
-
 IF_XML = """
 <domain>
   <devices>
     <interface type='bridge'>
       <mac address='52:54:00:d7:92:5b'/>
     </interface>
   </devices>
@@ -16,15 +10,15 @@
 
 
 def test_name(domain):
     assert domain.name == "a"
 
 
 def test_context(domain):
-    assert domain.context == None
+    assert domain.context is None
     domain.context = "something"
     assert domain.context == "something"
 
 
 def test_load_ssh_key(domain, tmp_path):
     CONTENT = "dummy ssh key"
     p = tmp_path / "id_rsa.pub"
```

### Comparing `virt-lightning-2.2.0/tests/test_hv.py` & `virt-lightning-2.3.0/tests/test_hv.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,10 @@
-import virt_lightning
+from unittest.mock import Mock, patch
 
-import ipaddress
 import libvirt
-import pathlib
-from unittest.mock import call
-from unittest.mock import Mock
-from unittest.mock import patch
 
 
 def test_arch(hv):
     assert hv.arch == "i686"
 
 
 def test_domain_type(hv):
@@ -90,8 +85,8 @@
     mock_mac_addresses.__get__ = Mock(
         return_value=["52:54:00:0f:91:5e", "52:54:00:0f:91:33"]
     )
     domain.ipv4 = "192.168.123.5/24"
     hv.network_obj.XMLDesc = Mock(return_value=NET_XML)
     hv.network_obj.update = Mock()
     hv.remove_domain_from_network(domain)
-    hv.network_obj.update.call_count == 3
+    assert hv.network_obj.update.call_count == 2
```

### Comparing `virt-lightning-2.2.0/tox.ini` & `virt-lightning-2.3.0/tox.ini`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,45 @@
 [tox]
-envlist = pep8,py36,py37,py38,py39,black,mypy
+envlist = flake8,py39,py310,py311,black
 
 [gh-actions]
 python =
-    3.6: py36
-    3.7: py37
-    3.8: py38
     3.9: py39
+    3.10: py310
+    3.11: py311, flake8, black
 
 [testenv]
 deps = -r{toxinidir}/requirements.txt
        -r{toxinidir}/test-requirements.txt
 install_command = pip install -U {packages}
 commands =
     pytest --cov={envsitepackagesdir}/virt_lightning --cov-report html -v {posargs}
 use_developer = True
 
-[testenv:pep8]
-commands = flake8 --exclude=version.py setup.py virt_lightning
+[testenv:flake8]
+commands = flake8 --exclude=version.py virt_lightning
 
 [testenv:black]
 commands =
-    black --diff  --check --exclude=version.py setup.py virt_lightning
+    black --diff  --check --exclude=version.py virt_lightning
 
 [testenv:mypy]
 deps = -r{toxinidir}/requirements.txt
        -r{toxinidir}/test-requirements.txt
        mypy
 commands = mypy . --ignore-missing-imports
 
+[testenv:build]
+deps =
+  build
+skip_install = true
+commands =
+  python -m build
+  python -c "print('finish the upload with: twine upload -s dist/*')"
+
 [testenv:upload]
 deps = twine
 commands = python3 -m twine upload --repository pypi dist/*
 
 [isort]
 line_length=90
 [flake8]
```

### Comparing `virt-lightning-2.2.0/virt-lightning.org/bench_images_startup.py` & `virt-lightning-2.3.0/virt-lightning.org/bench_images_startup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
 
-import io
 import logging
+import pathlib
 import time
+
 import yaml
-import pathlib
+
 import virt_lightning.api as vla
 from virt_lightning.configuration import Configuration
 
 logger = logging.getLogger("virt_lightning")
 logger.setLevel(logging.DEBUG)
 ch = logging.StreamHandler()
 logger.addHandler(ch)
@@ -22,24 +23,33 @@
 log_dir = pathlib.Path("/tmp/log")
 local_dir = pathlib.Path("/var/lib/virt-lightning/pool/upstream/")
 
 configuration = Configuration()
 for distro in distros:
     qcow2_path = local_dir / (distro + ".qcow2")
     if not qcow2_path.exists():
-        print("Fetching {distro}".format(distro=distro))
+        print(f"Fetching {distro}")
         try:
             vla.fetch(configuration=configuration, distro=distro)
         except vla.ImageNotFoundUpstreamError:
             print("Image not found")
             continue
     log_file = log_dir / (distro + ".log")
-    sum = .0
-    for i in range(number_of_runs):
+    sum = 0.0
+    for _i in range(number_of_runs):
         my_fd = log_file.open("w")
         vla.down(configuration)
         start_time = time.time()
-        vla.start(configuration=configuration, distro=distro, enable_console=True, console_fd=my_fd) 
+        vla.start(
+            configuration=configuration,
+            distro=distro,
+            enable_console=True,
+            console_fd=my_fd,
+        )
         elapsed_time = time.time() - start_time
         sum += elapsed_time
-        print("- elapsed_time={elapsed_time:06.2f}".format(elapsed_time=elapsed_time))
-    print("FINAL distro={distro}: {result}".format(distro=distro, result=sum/number_of_runs))
+        print(f"- elapsed_time={elapsed_time:06.2f}")
+    print(
+        "FINAL distro={distro}: {result}".format(
+            distro=distro, result=sum / number_of_runs
+        )
+    )
```

### Comparing `virt-lightning-2.2.0/virt-lightning.org/etc/caddy/conf.d/virt-lightning.org.conf` & `virt-lightning-2.3.0/virt-lightning.org/etc/caddy/conf.d/virt-lightning.org.conf`

 * *Files 12% similar despite different names*

```diff
@@ -9,39 +9,51 @@
     # Fedora
     redir /images/fedora-31/fedora-31.qcow2 https://download.fedoraproject.org/pub/fedora/linux/releases/31/Cloud/x86_64/images/Fedora-Cloud-Base-31-1.9.x86_64.qcow2
     redir /images/fedora-32/fedora-32.qcow2 https://download.fedoraproject.org/pub/fedora/linux/releases/32/Cloud/x86_64/images/Fedora-Cloud-Base-32-1.6.x86_64.qcow2
     redir /images/fedora-33/fedora-33.qcow2 https://download.fedoraproject.org/pub/fedora/linux/releases/33/Cloud/x86_64/images/Fedora-Cloud-Base-33-1.2.x86_64.qcow2
     redir /images/fedora-34/fedora-34.qcow2 https://download.fedoraproject.org/pub/fedora/linux/releases/34/Cloud/x86_64/images/Fedora-Cloud-Base-34-1.2.x86_64.qcow2
     redir /images/fedora-35/fedora-35.qcow2 https://download.fedoraproject.org/pub/fedora/linux/releases/35/Cloud/x86_64/images/Fedora-Cloud-Base-35-1.2.x86_64.qcow2
     redir /images/fedora-36/fedora-36.qcow2 https://download.fedoraproject.org/pub/fedora/linux/releases/36/Cloud/x86_64/images/Fedora-Cloud-Base-36-1.5.x86_64.qcow2
+    redir /images/fedora-37/fedora-37.qcow2 https://download.fedoraproject.org/pub/fedora/linux/releases/37/Cloud/x86_64/images/Fedora-Cloud-Base-37-1.7.x86_64.qcow2
+    redir /images/fedora-38/fedora-38.qcow2 https://download.fedoraproject.org/pub/fedora/linux/releases/38/Cloud/x86_64/images/Fedora-Cloud-Base-38-1.6.x86_64.qcow2
 
     # Debian
     redir /images/debian-9/debian-9.qcow2 https://cdimage.debian.org/cdimage/openstack/current-9/debian-9-openstack-amd64.qcow2
     redir /images/debian-10/debian-10.qcow2 https://cdimage.debian.org/cdimage/openstack/current-10/debian-10-openstack-amd64.qcow2
     redir /images/debian-testing/debian-testing.qcow2 https://cdimage.debian.org/cdimage/openstack/testing/debian-testing-openstack-amd64.qcow2
+    redir /images/debian-11/debian-11.qcow2 https://cdimage.debian.org/cdimage/cloud/bullseye/latest/debian-11-generic-amd64.qcow2
+
+
 
     # CentOS
     redir /images/centos-7/centos-7.qcow2 http://cloud.centos.org/centos/7/images/CentOS-7-x86_64-GenericCloud.qcow2
     redir /images/centos-6/centos-6.qcow2 https://cloud.centos.org/centos/6/images/CentOS-6-x86_64-GenericCloud.qcow2
     redir /images/centos-8/centos-8.qcow2 https://cloud.centos.org/centos/8/x86_64/images/CentOS-8-GenericCloud-8.1.1911-20200113.3.x86_64.qcow2
     redir /images/centos-8-stream/centos-8-stream.qcow2 https://cloud.centos.org/centos/8-stream/x86_64/images/CentOS-Stream-GenericCloud-8-20220125.1.x86_64.qcow2
     redir /images/centos-9-stream/centos-9-stream.qcow2 https://cloud.centos.org/centos/9-stream/x86_64/images/CentOS-Stream-GenericCloud-9-20220330.1.x86_64.qcow2
 
     # AlmaLinux
     redir /images/almalinux-8/almalinux-8.qcow2 https://repo.almalinux.org/almalinux/8/cloud/x86_64/images/AlmaLinux-8-GenericCloud-latest.x86_64.qcow2
     redir /images/almalinux-9/almalinux-9.qcow2 https://repo.almalinux.org/almalinux/9/cloud/x86_64/images/AlmaLinux-9-GenericCloud-latest.x86_64.qcow2
 
+    # RockyLinux
+    redir /images/rockylinux-8/rockylinux-8.qcow2 https://download.rockylinux.org/pub/rocky/8/images/x86_64/Rocky-8-GenericCloud.latest.x86_64.qcow2
+    redir /images/rockylinux-9/rockylinux-9.qcow2 https://download.rockylinux.org/pub/rocky/9/images/x86_64/Rocky-9-GenericCloud.latest.x86_64.qcow2
+
     # Ubuntu
     redir /images/ubuntu-14.04/ubuntu-14.04.qcow2 https://cloud-images.ubuntu.com/trusty/current/trusty-server-cloudimg-amd64-disk1.img
     redir /images/ubuntu-16.04/ubuntu-16.04.qcow2 https://cloud-images.ubuntu.com/xenial/current/xenial-server-cloudimg-amd64-disk1.img
     redir /images/ubuntu-18.04/ubuntu-18.04.qcow2 https://cloud-images.ubuntu.com/bionic/current/bionic-server-cloudimg-amd64.img
     redir /images/ubuntu-19.04/ubuntu-19.04.qcow2 https://cloud-images.ubuntu.com/disco/current/disco-server-cloudimg-amd64.img
     redir /images/ubuntu-19.10/ubuntu-19.10.qcow2 https://cloud-images.ubuntu.com/eoan/current/eoan-server-cloudimg-amd64.img
     redir /images/ubuntu-20.04/ubuntu-20.04.qcow2 https://cloud-images.ubuntu.com/focal/current/focal-server-cloudimg-amd64.img
     redir /images/ubuntu-21.04/ubuntu-21.04.qcow2 https://cloud-images.ubuntu.com/hirsute/current/hirsute-server-cloudimg-amd64.img
+    redir /images/ubuntu-22.04/ubuntu-22.04.qcow2 https://cloud-images.ubuntu.com/jammy/current/jammy-server-cloudimg-amd64.img
+    redir /images/ubuntu-22.10/ubuntu-22.10.qcow2 https://cloud-images.ubuntu.com/kinetic/current/kinetic-server-cloudimg-amd64.img
+    redir /images/ubuntu-23.04/ubuntu-23.04.qcow2 https://cloud-images.ubuntu.com/lunar/current/lunar-server-cloudimg-amd64.img
 
     # Cirros (broken: cannot login, no Python)
     redir /images/cirros-0.4.0/cirros-0.4.0.qcow2 http://download.cirros-cloud.net/0.4.0/cirros-0.4.0-x86_64-disk.img
 
     # OpenSUSE
     redir /images/opensuse-leap-15.2/opensuse-leap-15.2.qcow2 https://download.opensuse.org/repositories/Cloud:/Images:/Leap_15.2/images/openSUSE-Leap-15.2-OpenStack.x86_64.qcow2
 
@@ -77,27 +89,34 @@
     redir /images/openbsd-6.7/openbsd-6.7.qcow2 https://object-storage.public.mtl1.vexxhost.net/swift/v1/1dbafeefbd4f4c80864414a441e72dd2/bsd-cloud-image.org/images/openbsd/6.7/openbsd-6.7.qcow2
     redir /images/openbsd-6.8/openbsd-6.8.qcow2 https://object-storage.public.mtl1.vexxhost.net/swift/v1/1dbafeefbd4f4c80864414a441e72dd2/bsd-cloud-image.org/images/openbsd/6.8/openbsd-6.8.qcow2
     redir /images/openbsd-6.8/openbsd-6.8.yaml https://object-storage.public.mtl1.vexxhost.net/swift/v1/1dbafeefbd4f4c80864414a441e72dd2/bsd-cloud-image.org/images/openbsd/6.8/openbsd-6.8.yaml
     redir /images/openbsd-6.9/openbsd-6.9.qcow2 https://object-storage.public.mtl1.vexxhost.net/swift/v1/1dbafeefbd4f4c80864414a441e72dd2/bsd-cloud-image.org/images/openbsd/6.9/openbsd-6.9.qcow2
     redir /images/openbsd-6.9/openbsd-6.9.yaml https://object-storage.public.mtl1.vexxhost.net/swift/v1/1dbafeefbd4f4c80864414a441e72dd2/bsd-cloud-image.org/images/openbsd/6.9/openbsd-6.9.yaml
     redir /images/openbsd-7.0/openbsd-7.0.qcow2 https://object-storage.public.mtl1.vexxhost.net/swift/v1/1dbafeefbd4f4c80864414a441e72dd2/bsd-cloud-image.org/images/openbsd/7.0/2021-12-11/openbsd-7.0.qcow2
     redir /images/openbsd-7.0/openbsd-7.0.yaml https://object-storage.public.mtl1.vexxhost.net/swift/v1/1dbafeefbd4f4c80864414a441e72dd2/bsd-cloud-image.org/images/openbsd/7.0/2021-12-11/openbsd-7.0.yaml
-
+    redir /images/openbsd-7.1/openbsd-7.1.qcow2 https://object-storage.public.mtl1.vexxhost.net/swift/v1/1dbafeefbd4f4c80864414a441e72dd2/bsd-cloud-image.org/images/openbsd/7.1/2022-06-27/ufs/openbsd-7.1-2022-06-27.qcow2
+    redir /images/openbsd-7.1/openbsd-7.1.yaml https://object-storage.public.mtl1.vexxhost.net/swift/v1/1dbafeefbd4f4c80864414a441e72dd2/bsd-cloud-image.org/images/openbsd/7.1/2022-06-27/ufs/openbsd-7.1-2022-06-27.yaml
+    redir /images/openbsd-7.2/openbsd-7.2.qcow2 https://object-storage.public.mtl1.vexxhost.net/swift/v1/1dbafeefbd4f4c80864414a441e72dd2/bsd-cloud-image.org/images/openbsd/7.2/2022-11-06/ufs/openbsd-7.2-2022-11-06.qcow2
+    redir /images/openbsd-7.2/openbsd-7.2.yaml https://object-storage.public.mtl1.vexxhost.net/swift/v1/1dbafeefbd4f4c80864414a441e72dd2/bsd-cloud-image.org/images/openbsd/7.2/2022-11-06/ufs/openbsd-7.2-2022-11-06.yaml
 
     # DragonFlyBSD
     redir /images/dragonflybsd-5.8.3/dragonflybsd-5.8.3.qcow2 https://object-storage.public.mtl1.vexxhost.net/swift/v1/1dbafeefbd4f4c80864414a441e72dd2/bsd-cloud-image.org/images/dragonflybsd/5.8.3/dragonflybsd-5.8.3.qcow2
     redir /images/dragonflybsd-5.8.3/dragonflybsd-5.8.3.yaml https://object-storage.public.mtl1.vexxhost.net/swift/v1/1dbafeefbd4f4c80864414a441e72dd2/bsd-cloud-image.org/images/dragonflybsd/5.8.3/dragonflybsd-5.8.3.yaml
     redir /images/dragonflybsd-6.0.0/dragonflybsd-6.0.0.qcow2 https://object-storage.public.mtl1.vexxhost.net/swift/v1/1dbafeefbd4f4c80864414a441e72dd2/bsd-cloud-image.org/images/dragonflybsd/6.0.0/dragonflybsd-6.0.0.qcow2
     redir /images/dragonflybsd-6.0.0/dragonflybsd-6.0.0.yaml https://object-storage.public.mtl1.vexxhost.net/swift/v1/1dbafeefbd4f4c80864414a441e72dd2/bsd-cloud-image.org/images/dragonflybsd/6.0.0/dragonflybsd-6.0.0.yaml
     redir /images/dragonflybsd-6.0.0-ufs/dragonflybsd-6.0.0-ufs.qcow2 https://object-storage.public.mtl1.vexxhost.net/swift/v1/1dbafeefbd4f4c80864414a441e72dd2/bsd-cloud-image.org/images/dragonflybsd/6.0.0/dragonflybsd-6.0.0-ufs.qcow2
     redir /images/dragonflybsd-6.0.0-ufs/dragonflybsd-6.0.0-ufs.yaml https://object-storage.public.mtl1.vexxhost.net/swift/v1/1dbafeefbd4f4c80864414a441e72dd2/bsd-cloud-image.org/images/dragonflybsd/6.0.0/dragonflybsd-6.0.0-ufs.yaml
     redir /images/dragonflybsd-6.0.0-hammer2/dragonflybsd-6.0.0-hammer2.qcow2 https://object-storage.public.mtl1.vexxhost.net/swift/v1/1dbafeefbd4f4c80864414a441e72dd2/bsd-cloud-image.org/images/dragonflybsd/6.0.0/dragonflybsd-6.0.0-hammer2.qcow2
     redir /images/dragonflybsd-6.0.0-hammer2/dragonflybsd-6.0.0-hammer2.yaml https://object-storage.public.mtl1.vexxhost.net/swift/v1/1dbafeefbd4f4c80864414a441e72dd2/bsd-cloud-image.org/images/dragonflybsd/6.0.0/dragonflybsd-6.0.0-hammer2.yaml
     redir /images/dragonflybsd-6.0.1-ufs/dragonflybsd-6.0.1-ufs.qcow2 https://object-storage.public.mtl1.vexxhost.net/swift/v1/1dbafeefbd4f4c80864414a441e72dd2/bsd-cloud-image.org/images/dragonflybsd/6.0.1/2021-12-11/dragonflybsd-6.0.1-ufs.qcow2
     redir /images/dragonflybsd-6.0.1-ufs/dragonflybsd-6.0.1-ufs.yaml https://object-storage.public.mtl1.vexxhost.net/swift/v1/1dbafeefbd4f4c80864414a441e72dd2/bsd-cloud-image.org/images/dragonflybsd/6.0.1/2021-12-11/dragonflybsd-6.0.1-ufs.yaml
     redir /images/dragonflybsd-6.0.1-hammer2/dragonflybsd-6.0.1-hammer2.qcow2 https://object-storage.public.mtl1.vexxhost.net/swift/v1/1dbafeefbd4f4c80864414a441e72dd2/bsd-cloud-image.org/images/dragonflybsd/6.0.1/2021-12-11/dragonflybsd-6.0.1-hammer2.qcow2
     redir /images/dragonflybsd-6.0.1-hammer2/dragonflybsd-6.0.1-hammer2.yaml https://object-storage.public.mtl1.vexxhost.net/swift/v1/1dbafeefbd4f4c80864414a441e72dd2/bsd-cloud-image.org/images/dragonflybsd/6.0.1/2021-12-11/dragonflybsd-6.0.1-hammer2.yaml
+    redir /images/dragonflybsd-6.2.2-hammer2/dragonflybsd-6.2.2-hammer2.qcow2 https://object-storage.public.mtl1.vexxhost.net/swift/v1/1dbafeefbd4f4c80864414a441e72dd2/bsd-cloud-image.org/images/dragonflybsd/6.2.2/2022-09-06/hammer2/dragonflybsd-6.2.2-hammer2-2022-09-06.qcow2
+    redir /images/dragonflybsd-6.2.2-hammer2/dragonflybsd-6.2.2-hammer2.yaml https://object-storage.public.mtl1.vexxhost.net/swift/v1/1dbafeefbd4f4c80864414a441e72dd2/bsd-cloud-image.org/images/dragonflybsd/6.2.2/2022-09-06/hammer2/dragonflybsd-6.2.2-hammer2-2022-09-06.yaml
+    redir /images/dragonflybsd-6.2.2-ufs/dragonflybsd-6.2.2-ufs.qcow2 https://object-storage.public.mtl1.vexxhost.net/swift/v1/1dbafeefbd4f4c80864414a441e72dd2/bsd-cloud-image.org/images/dragonflybsd/6.2.2/2022-09-06/ufs/dragonflybsd-6.2.2-ufs-2022-09-06.qcow2
+    redir /images/dragonflybsd-6.2.2-ufs/dragonflybsd-6.2.2-ufs.yaml https://object-storage.public.mtl1.vexxhost.net/swift/v1/1dbafeefbd4f4c80864414a441e72dd2/bsd-cloud-image.org/images/dragonflybsd/6.2.2/2022-09-06/ufs/dragonflybsd-6.2.2-ufs-2022-09-06.yaml
 
 
     # AmazonLinux 2
     redir /images/amazon2-20210126.0/amazon2-20210126.0.qcow2 https://cdn.amazonlinux.com/os-images/2.0.20210126.0/kvm/amzn2-kvm-2.0.20210126.0-x86_64.xfs.gpt.qcow2
 }
```

### Comparing `virt-lightning-2.2.0/virt_lightning/api.py` & `virt-lightning-2.3.0/virt_lightning/api.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 #!/usr/bin/env python3
 
-import collections
-from concurrent.futures import ThreadPoolExecutor
-import logging
-
 import asyncio
+import collections
+import distutils.util
 import ipaddress
-import libvirt
-import re
+import logging
 import pathlib
-
-import urllib.request
+import re
 import sys
-import distutils.util
-from virt_lightning.symbols import get_symbols
-from virt_lightning.configuration import Configuration
+import urllib.request
+from concurrent.futures import ThreadPoolExecutor
+
+import libvirt
 
 import virt_lightning.virt_lightning as vl
+from virt_lightning.configuration import Configuration
+from virt_lightning.symbols import get_symbols
 
 BASE_URL = "https://virt-lightning.org"
 
 logger = logging.getLogger("virt_lightning")
 
 
 def libvirt_callback(userdata, err):
@@ -75,15 +74,15 @@
 
 
 def _connect_libvirt(uri):
     try:
         return libvirt.open(uri)
     except libvirt.libvirtError as e:
         if e.get_error_code() == libvirt.VIR_ERR_AUTH_UNAVAILABLE:
-            raise CannotConnectToLibvirtError()
+            raise CannotConnectToLibvirtError() from None
         raise
 
 
 def _start_domain(hv, host, context, configuration):
     distro = host["distro"]
     if "name" not in host:
         host["name"] = re.sub(r"[^a-zA-Z0-9-]+", "", distro)
@@ -163,21 +162,19 @@
     for host in hosts:
         distro = host.get("distro")
         if distro not in hv.distro_available():
             logger.debug("distro not available: %s, will be fetched", distro)
             try:
                 fetch(hv=hv, distro=distro)
             except ImageNotFoundUpstreamError:
-                raise ImageNotFoundLocallyError(distro)
+                raise ImageNotFoundLocallyError(distro) from None
 
 
 def up(virt_lightning_yaml, configuration, context="default", **kwargs):
-    """
-    Create a list of VM
-    """
+    """Create a list of VM."""
 
     def _lifecycle_callback(conn, dom, state, reason, opaque):  # noqa: N802
         if state == 1:
             logger.info("%s %s QEMU agent found", symbols.CUSTOMS.value, dom.name())
 
     loop = kwargs.get("loop") or asyncio.get_event_loop()
     _register_aio_virt_impl(loop)
@@ -222,24 +219,24 @@
     loop.run_until_complete(deploy())
     logger.info("%s You are all set", symbols.THUMBS_UP.value)
 
 
 def start(
     configuration, context="default", enable_console=False, console_fd=None, **kwargs
 ):
-    """
-    Start a single VM
-    """
+    """Start a single VM."""
     conn = _connect_libvirt(configuration.libvirt_uri)
     hv = vl.LibvirtHypervisor(conn)
     hv.init_network(configuration.network_name, configuration.network_cidr)
     hv.init_storage_pool(configuration.storage_pool)
     host = {
         k: kwargs[k] for k in ["name", "distro", "memory", "vcpus"] if kwargs.get(k)
     }
+    if kwargs.get("disk"):
+        host.update({"disks": [{"size": x} for x in kwargs["disk"]]})
     _ensure_image_exists(hv, [host])
     domain = _start_domain(hv, host, context, configuration)
     if not domain:
         return
 
     loop = kwargs.get("loop") or asyncio.get_event_loop()
 
@@ -277,17 +274,15 @@
         domain.name,
         domain.name,
     )
     return domain
 
 
 def stop(configuration, **kwargs):
-    """
-    Stop and delete a given VM
-    """
+    """Stop and delete a given VM."""
     conn = _connect_libvirt(configuration.libvirt_uri)
     hv = vl.LibvirtHypervisor(conn)
     hv.init_network(configuration.network_name, configuration.network_cidr)
     hv.init_storage_pool(configuration.storage_pool)
     domain = hv.get_domain_by_name(kwargs["name"])
     if not domain:
         vm_list = [d.name for d in hv.list_domains()]
@@ -298,17 +293,15 @@
         else:
             logger.info("No running VM.")
         raise VMNotFoundError(kwargs["name"])
     hv.clean_up(domain)
 
 
 def ansible_inventory(configuration, context="default", **kwargs):
-    """
-    Generate an Ansible inventory based on the running VM
-    """
+    """Generate an Ansible inventory based on the running VM."""
     conn = _connect_libvirt(configuration.libvirt_uri)
     hv = vl.LibvirtHypervisor(conn)
 
     ssh_cmd_template = (
         "{name} ansible_host={ipv4} ansible_user={username} "
         "ansible_python_interpreter={python_interpreter} "
         'ansible_ssh_common_args="-o UserKnownHostsFile=/dev/null '
@@ -331,24 +324,22 @@
             name=domain.name,
             username=domain.username,
             ipv4=domain.ipv4.ip,
             python_interpreter=domain.python_interpreter,
         )  # noqa: T001
 
     for group_name, domains in groups.items():
-        output += "\n[{group_name}]\n".format(group_name=group_name)
+        output += f"\n[{group_name}]\n"
         for domain in domains:
             output += domain.name + "\n"
     return output
 
 
 def ssh_config(configuration, context="default", **kwargs):
-    """
-    Generate an SSH configuration based on the running VM
-    """
+    """Generate an SSH configuration based on the running VM."""
     conn = _connect_libvirt(configuration.libvirt_uri)
     hv = vl.LibvirtHypervisor(conn)
 
     ssh_host_template = (
         "Host {name}\n"
         "     Hostname {ipv4}\n"
         "     User {username}\n"
@@ -370,24 +361,22 @@
             name=domain.name,
             username=domain.username,
             ipv4=domain.ipv4.ip,
             ssh_key_file=domain.ssh_key,
         )
 
     for group_name, domains in groups.items():
-        output += "\n[{group_name}]".format(group_name=group_name)
+        output += f"\n[{group_name}]"
         for domain in domains:
             output += domain.name
     return output
 
 
 def status(configuration, context="default", name=None, **kwargs):
-    """
-    Returns the status of the VM of the envionment
-    """
+    """Returns the status of the VM of the envionment."""
     conn = _connect_libvirt(configuration.libvirt_uri)
     hv = vl.LibvirtHypervisor(conn)
 
     for domain in hv.list_domains():
         if context and context != domain.context:
             continue
         name = domain.name
@@ -399,38 +388,32 @@
             "context": domain.context,
             "username": domain.username,
             "distro": domain.distro,
         }
 
 
 def exec_ssh(configuration, name=None, **kwargs):
-    """
-    Open an SSH connection on a host
-    """
+    """Open an SSH connection on a host."""
     conn = _connect_libvirt(configuration.libvirt_uri)
     hv = vl.LibvirtHypervisor(conn)
     domain = hv.get_domain_by_name(name)
     if not domain:
         raise VMNotFoundError(name)
     domain.exec_ssh()
 
 
 def list_domains(configuration, name=None, **kwargs):
-    """
-    Return a list Python-libvirt instance of the running libvirt VM.
-    """
+    """Return a list Python-libvirt instance of the running libvirt VM."""
     conn = _connect_libvirt(configuration.libvirt_uri)
     hv = vl.LibvirtHypervisor(conn)
     return sorted(hv.list_domains())
 
 
 def down(configuration, context="default", **kwargs):
-    """
-    Stop and remove a running environment.
-    """
+    """Stop and remove a running environment."""
     conn = _connect_libvirt(configuration.libvirt_uri)
     hv = vl.LibvirtHypervisor(conn)
     hv.init_network(configuration.network_name, configuration.network_cidr)
     hv.init_storage_pool(configuration.storage_pool)
     for domain in hv.list_domains():
         if domain.context != context:
             continue
@@ -438,39 +421,33 @@
         hv.clean_up(domain)
 
     if bool(distutils.util.strtobool(configuration.network_auto_clean_up)):
         hv.network_obj.destroy()
 
 
 def distro_list(configuration, **kwargs):
-    """
-    Return a list of VM images that are available on the system.
-    """
+    """Return a list of VM images that are available on the system."""
     conn = _connect_libvirt(configuration.libvirt_uri)
     hv = vl.LibvirtHypervisor(conn)
     hv.init_storage_pool(configuration.storage_pool)
     return hv.distro_available()
 
 
 def storage_dir(configuration, **kwargs):
-    """
-    Return the location of the VM image storage directory.
-    """
+    """Return the location of the VM image storage directory."""
     conn = _connect_libvirt(configuration.libvirt_uri)
     hv = vl.LibvirtHypervisor(conn)
     hv.init_storage_pool(configuration.storage_pool)
     return hv.get_storage_dir()
 
 
 def fetch_from_url(progress_callback=None, url=None, **kwargs):
+    """Retrieve a VM image from a given url
+    - when url is set to None, this means we are trying to fetch from the default url.
     """
-    Retrieve a VM image from a given url
-        - when url is set to None, this means we are trying to fetch from the default url
-    """
-
     target_file = pathlib.PosixPath(
         "{storage_dir}/upstream/{distro}.qcow2".format(**kwargs)
     )
     temp_file = target_file.with_suffix(".temp")
     if target_file.exists():
         logger.info("File already exists: %s", target_file)
         return
@@ -488,15 +465,15 @@
     parent_url = BASE_URL + "/images/{distro}".format(**kwargs) if url is None else url
     try:
         r = urllib.request.urlopen(
             "{url}/{distro}.qcow2".format(url=parent_url, **kwargs)
         )
     except urllib.error.HTTPError as e:
         if e.code == 404:
-            raise ImageNotFoundUpstreamError(kwargs["distro"])
+            raise ImageNotFoundUpstreamError(kwargs["distro"]) from None
         else:
             logger.exception(e)
             raise
     last_modified = r.headers["Last-Modified"]
     logger.debug("Date: %s", last_modified)
     size = r.headers["Content-Length"]
     logger.debug("Size: %s", size)
@@ -518,17 +495,15 @@
             pass
     with target_file.with_suffix(".yaml").open("wb") as fd:
         fd.write(r.read())
     logger.info("Image {distro} is ready!".format(**kwargs))
 
 
 def fetch(configuration=None, progress_callback=None, hv=None, **kwargs):
-    """
-    Retrieve a VM image from Internet.
-    """
+    """Retrieve a VM image from Internet."""
     if hv is None:
         conn = _connect_libvirt(configuration.libvirt_uri)
         hv = vl.LibvirtHypervisor(conn)
         hv.init_storage_pool(configuration.storage_pool)
 
     configuration = configuration if configuration is not None else Configuration()
     image_found = False
```

### Comparing `virt-lightning-2.2.0/virt_lightning/configuration.py` & `virt-lightning-2.3.0/virt_lightning/configuration.py`

 * *Files identical despite different names*

### Comparing `virt-lightning-2.2.0/virt_lightning/shell.py` & `virt-lightning-2.3.0/virt_lightning/shell.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 #!/usr/bin/env python3
 
 import argparse
 import logging
-import pathlib
-import libvirt
 import os
-import yaml
+import pathlib
 import sys
 
+import libvirt
+import yaml
 
 import virt_lightning.api
+import virt_lightning.ui as ui
+import virt_lightning.virt_lightning as vl
 from virt_lightning.configuration import Configuration
 from virt_lightning.symbols import get_symbols
-import virt_lightning.virt_lightning as vl
-import virt_lightning.ui as ui
-
 
 symbols = get_symbols()
 logger = logging.getLogger("virt_lightning")
 logger.setLevel(logging.INFO)
 ch = logging.StreamHandler()
 logger.addHandler(ch)
 
@@ -37,19 +36,17 @@
     libvirt_group = get_local_libvirt_group()
     if not libvirt_group:
         return
     group, gid = libvirt_group
     if gid not in os.getgroups():
         print("Virt-Lightning cannot access the local libvirt service.")  # noqa: T001
         print(  # noqa: T001
-            (
-                f"Your user should probably be in the {group} group. "
-                f"You can add the user {getpass. getuser()} in the group {group} with the "
-                "following command:"
-            )
+            f"Your user should probably be in the {group} group. "
+            f"You can add the user {getpass. getuser()} in the group {group} with the "
+            "following command:"
         )
         print(  # noqa: T001
             f"    sudo usermod --append --groups libvirt {getpass.getuser()}"
         )
 
 
 def console(configuration, name=None, **kwargs):
@@ -121,15 +118,14 @@
         content = yaml.safe_load(fd.read())
         if not isinstance(content, list):
             raise argparse.ArgumentTypeError(f"{value} should be a YAML list.")
         return content
 
 
 def main():
-
     title = "{lightning} Virt-Lightning {lightning}".format(
         lightning=symbols.LIGHTNING.value
     )
 
     usage = """
 usage: vl [--debug DEBUG] [--config CONFIG] COMMAND
 
@@ -224,14 +220,22 @@
         "--show-console",
         help="Suppress console output during VM creation",
         type=bool,
         dest="enable_console",
         default=True,
     )
     start_parser.add_argument("distro", help="Name of the distro", type=str)
+    start_parser.add_argument(
+        "--disk",
+        action="extend",
+        nargs=1,
+        metavar="SIZE",
+        help="Size of disk in GB. Multiple disks might be defined",
+        type=int,
+    )
 
     stop_parser = action_subparsers.add_parser(
         "stop", help="Stop and delete a VM", parents=[parent_parser]
     )
     stop_parser.add_argument("name", help="Name of the VM", type=str)
 
     status_parser = action_subparsers.add_parser(
@@ -308,15 +312,15 @@
         print(  # noqa: T001
             virt_lightning.api.ssh_config(configuration=configuration, **vars(args))
         )
     elif args.action == "distro_list":
         for distro_name in virt_lightning.api.distro_list(
             configuration=configuration, **vars(args)
         ):
-            print("- distro: {0}".format(distro_name))  # noqa: T001
+            print(f"- distro: {distro_name}")  # noqa: T001
     elif args.action == "storage_dir":
         print(  # noqa: T001
             virt_lightning.api.storage_dir(configuration=configuration, **vars(args))
         )
     elif args.action == "status":
         results = {}
         for status in virt_lightning.api.status(
@@ -385,15 +389,15 @@
             print(f"The following instance is not running: {e.name}")  # noqa: T001
             exit(1)
     else:
         try:
             action_func = getattr(virt_lightning.api, args.action)
             action_func(configuration=configuration, **vars(args))
         except virt_lightning.api.VMNotFoundError as e:
-            logger.error("VM {name} not found".format(name=e.name))
+            logger.error(f"VM {e.name} not found")
         except virt_lightning.api.ImageNotFoundLocallyError as e:
             logger.error(
                 (
                     "ℹ️ You may be able to download the image with the "
                     "`vl fetch {name}` command."
                 ).format(name=e.name)
             )
```

### Comparing `virt-lightning-2.2.0/virt_lightning/symbols.py` & `virt-lightning-2.3.0/virt_lightning/symbols.py`

 * *Files identical despite different names*

### Comparing `virt-lightning-2.2.0/virt_lightning/templates.py` & `virt-lightning-2.3.0/virt_lightning/templates.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     <input type='keyboard' bus='ps2'/>
     <graphics type="vnc" port="-1" autoport="yes" listen="127.0.0.1" keymap="en-us">
       <listen type="address" address="127.0.0.1"/>
     </graphics>
     <memballoon model='virtio'></memballoon>
   </devices>
 </domain>
-"""  # NOQA
+"""
 
 BRIDGE_XML = """
 <interface type='network'>
   <source network='virt-lightning'/>
   <model type='virtio'/>
 </interface>
 """
```

### Comparing `virt-lightning-2.2.0/virt_lightning/ui.py` & `virt-lightning-2.3.0/virt_lightning/ui.py`

 * *Files identical despite different names*

### Comparing `virt-lightning-2.2.0/virt_lightning/virt_lightning.py` & `virt-lightning-2.3.0/virt_lightning/virt_lightning.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,36 @@
 #!/usr/bin/env python3
 
-import ipaddress
+import asyncio
 import getpass
+import ipaddress
+import json
 import logging
 import math
 import os
 import pathlib
 import re
 import string
 import subprocess
 import sys
 import tempfile
-import typing
 import uuid
 import xml.etree.ElementTree as ET  # noqa: N817
 
 import libvirt
-
-import json
 import yaml
 
-import asyncio
-
 from virt_lightning.symbols import get_symbols
 
 from .templates import (
     BRIDGE_XML,
-    META_DATA_ENI,
-    NETWORK_DHCP_ENTRY,
     DISK_XML,
     DOMAIN_XML,
+    META_DATA_ENI,
+    NETWORK_DHCP_ENTRY,
     NETWORK_HOST_ENTRY,
     NETWORK_XML,
     STORAGE_POOL_XML,
     STORAGE_VOLUME_XML,
     USER_CREATE_STORAGE_POOL_DIR,
 )
 
@@ -130,29 +127,29 @@
         for k, v in self.get_distro_configuration(domain.distro).items():
             if v:
                 config[k] = v
         for k, v in user_config.items():
             if v:
                 config[k] = v
         domain.groups = config["groups"]
-        domain.load_ssh_key_file(config["ssh_key_file"])
+        domain.load_ssh_key_file(pathlib.Path(config["ssh_key_file"]))
         domain.memory = config["memory"]
         domain.python_interpreter = config["python_interpreter"]
         domain.root_password = config["root_password"]
         domain.username = config["username"]
         domain.vcpus = config["vcpus"]
         domain.default_nic_model = config["default_nic_model"]
         domain.bootcmd = config["bootcmd"]
         domain.runcmd = config["runcmd"]
         domain.meta_data_media_type = config["meta_data_media_type"]
         domain.default_bus_type = config["default_bus_type"]
         if "fqdn" in config:
             domain.fqdn = config["fqdn"]
 
-    def get_distro_configuration(self, distro) -> typing.Dict:
+    def get_distro_configuration(self, distro) -> dict:
         distro_configuration_file = pathlib.PosixPath(
             "{storage_dir}/upstream/{distro}.yaml".format(
                 storage_dir=self.get_storage_dir(), distro=distro
             )
         )
         if not distro_configuration_file.exists():
             return {}
@@ -181,15 +178,15 @@
             ipstr = dom.get_metadata("ipv4")
             if not ipstr:
                 continue
             interface = ipaddress.ip_interface(ipstr)
             used_ips.append(interface)
 
         for ip in self.network:
-            cidr_ip = "{ip}/24".format(ip=ip)
+            cidr_ip = f"{ip}/24"
             interface = ipaddress.IPv4Interface(cidr_ip)
             if int(interface.ip.exploded.split(".")[3]) < 5:
                 continue
             if self._last_free_ipv4 and self._last_free_ipv4 >= interface:
                 continue
             if interface.ip not in [i.ip for i in used_ips]:
                 self._last_free_ipv4 = interface
@@ -211,17 +208,15 @@
         if backing_on:
             backing_file = pathlib.PosixPath(
                 "{path}/upstream/{backing_on}.qcow2".format(
                     path=self.get_storage_dir(), backing_on=backing_on
                 )
             )
             min_size = self.get_qcow_virtual_size(backing_file)
-        disk_path = pathlib.PosixPath(
-            "{path}/{name}.qcow2".format(path=self.get_storage_dir(), name=name)
-        )
+        disk_path = pathlib.PosixPath(f"{self.get_storage_dir()}/{name}.qcow2")
 
         if "/" in name:
             raise TypeError
         if not size:
             size = 20
         if size < min_size:
             size = min_size
@@ -256,55 +251,65 @@
                         "{pool_name} {vol_name}.qcow2"
                     ).format(pool_name=self.storage_pool_obj.name(), vol_name=name)
                 )
                 sys.exit(1)
             raise
 
     def get_openstack_network_data(self, domain):
-
         openstack_network_data = {
             "links": [],
             "networks": [],
             "services": [{"type": "dns", "address": str(self.dns.ip)}],
         }
 
         for i, nic in enumerate(domain.nics):
             openstack_network_data["links"].append(
                 {
-                    "id": "interface{i}".format(i=i),
+                    "id": f"interface{i}",
                     "type": "phy",
                     "ethernet_mac_address": nic["mac"],
                 }
             )
 
             gateway = self.get_network_gateway(nic["network"])
             if nic["ipv4"]:
+                net_dns_nameservers = (
+                    [str(self.dns.ip)] if self.dns.ip in nic["ipv4"].network else []
+                )
                 openstack_network_data["networks"].append(
                     {
-                        "id": "private-ipv4-{i}".format(i=i),
+                        "id": f"private-ipv4-{i}",
                         "type": "ipv4",
-                        "link": "interface{i}".format(i=i),
+                        "link": f"interface{i}",
                         "ip_address": str(nic["ipv4"].ip),
                         "netmask": str(nic["ipv4"].netmask.exploded),
                         "routes": [
                             {
                                 "network": "0.0.0.0",
                                 "netmask": "0.0.0.0",
                                 "gateway": str(gateway.ip),
                             }
                         ],
                         "network_id": domain.dom.UUIDString(),
+                        # Workaround for CloudInit, sources.helpers.openstack read the
+                        # subnet DNS from ths dns_nameservers and ignore the
+                        # services key.
+                        # https://opendev.org/openstack/nova/commit/4b333b989dfc778a8b61db4a1b8552e988a10471
+                        "dns_nameservers": net_dns_nameservers,
+                        "services": [
+                            {"type": "dns", "address": ns} for ns in net_dns_nameservers
+                        ],
                     }
                 )
             else:
                 openstack_network_data["networks"].append(
                     {
-                        "id": "private-ipv4-{i}".format(i=i),
+                        "id": f"private-ipv4-{i}",
                         "type": "ipv4_dhcp",
-                        "link": "interface{i}".format(i=i),
+                        "link": f"interface{i}",
                         "network_id": domain.dom.UUIDString(),
                     }
                 )
 
         return openstack_network_data
 
     def prepare_cloud_init_openstack_iso(self, domain):
@@ -335,15 +340,15 @@
             with openstack_networkdata_file.open("w") as fd:
                 fd.write(json.dumps(self.get_openstack_network_data(domain)))
             openstack_userdata_file = openstack_dir / "user_data"
             with openstack_userdata_file.open("w") as fd:
                 fd.write("#cloud-config\n")
                 fd.write(yaml.dump(domain.user_data, Dumper=yaml.Dumper))
 
-            cidata_file = temp_dir / "{name}-cidata.iso".format(name=domain.name)
+            cidata_file = temp_dir / f"{domain.name}-cidata.iso"
             run_cmd(
                 [
                     str(self.iso_binary),
                     "-output",
                     cidata_file.name,
                     "-ldots",
                     "-allow-lowercase",
@@ -374,15 +379,15 @@
         network_config = []
         for i, nic in enumerate(domain.nics):
             gateway = self.get_network_gateway(nic["network"])
             if nic["ipv4"]:
                 network_config.append(
                     {
                         "type": "physical",
-                        "name": "eth{i}".format(i=i),
+                        "name": f"eth{i}",
                         "mac_address": nic["mac"],
                         "subnets": [
                             {
                                 "type": "static",
                                 "address": str(nic["ipv4"]),
                                 "gateway": str(gateway.ip),
                                 "dns_nameservers": [str(gateway.ip)],
@@ -390,15 +395,15 @@
                         ],
                     }
                 )
             else:
                 network_config.append(
                     {
                         "type": "physical",
-                        "name": "eth{i}".format(i=i),
+                        "name": f"eth{i}",
                         "mac_address": nic["mac"],
                         "subnets": [{"type": "dhcp"}],
                     }
                 )
         domain._network_meta = {"version": 1, "config": network_config}
 
         with tempfile.TemporaryDirectory() as base_temp_dir:
@@ -419,15 +424,15 @@
                         network=str(self.network),
                     )
                 )
             network_config_file = cd_dir / "network-config"
             with network_config_file.open("w") as fd:
                 fd.write(yaml.dump(domain._network_meta, Dumper=yaml.Dumper))
 
-            cidata_file = temp_dir / "{name}-cidata.iso".format(name=domain.name)
+            cidata_file = temp_dir / f"{domain.name}-cidata.iso"
             run_cmd(
                 [
                     str(self.iso_binary),
                     "-output",
                     cidata_file.name,
                     "-volid",
                     "cidata",
@@ -443,15 +448,15 @@
                 st = self.conn.newStream(0)
                 cdrom.upload(st, 0, 1024 * 1024)
                 st.send(fd.read())
                 st.finish()
             return cdrom
 
     def start(self, domain, metadata_format):
-        if metadata_format.get("provider", "") == "nocloud":
+        if metadata_format.get("provider", "") == "nocloud":  # noqa: SIM114
             cloud_init_iso = self.prepare_cloud_init_nocloud_iso(domain)
         elif domain.distro.startswith("rhel-6") or domain.distro.startswith("centos-6"):
             cloud_init_iso = self.prepare_cloud_init_nocloud_iso(domain)
         else:  # OpenStack format is the default
             cloud_init_iso = self.prepare_cloud_init_openstack_iso(domain)
 
         media_type = domain.meta_data_media_type
@@ -576,17 +581,16 @@
         root = ET.fromstring(xml)
         ip = root.find("./ip")
         return ipaddress.IPv4Interface("{address}/{netmask}".format(**ip.attrib))
 
     def reuse_mac_address(self, network_name, domain_name, ipv4):
         network_obj = self.get_network_by_name(network_name)
         for lease in network_obj.DHCPLeases():
-            if lease["hostname"] == domain_name:
-                if lease["ipaddr"] == str(ipv4.ip):
-                    return lease["mac"]
+            if lease["hostname"] == domain_name and lease["ipaddr"] == str(ipv4.ip):
+                return lease["mac"]
 
     def create_network(self, network_name, network_cidr):
         network = ipaddress.ip_network(network_cidr)
         root = ET.fromstring(NETWORK_XML)
         root.find("./name").text = network_name
         root.find("./bridge").attrib["name"] = network_name
         root.find("./ip").attrib = {
@@ -693,34 +697,33 @@
         return self.get_metadata("root_password")
 
     @root_password.setter
     def root_password(self, value):
         self.user_data["disable_root"] = False
         self.user_data["password"] = value
         self.user_data["chpasswd"] = {
-            "list": "root:{value}\n".format(value=value),
+            "list": f"root:{value}\n",
             "expire": False,
         }
         self.user_data["ssh_pwauth"] = True
         self.record_metadata("root_password", value)
 
     @property
     def ssh_key(self):
         return self._ssh_key
 
     @ssh_key.setter
     def ssh_key(self, value):
         self._ssh_key = value
 
     def load_ssh_key_file(self, ssh_key_file):
-        doc_url = "https://help.github.com/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent/#generating-a-new-ssh-key"  # NOQA
+        doc_url = "https://help.github.com/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent/#generating-a-new-ssh-key"
         try:
-            with open(os.path.expanduser(ssh_key_file), "r") as fd:
-                self.ssh_key = fd.read()
-        except IOError:
+            self.ssh_key = ssh_key_file.expanduser().read_text()
+        except OSError:
             logger.error(
                 (
                     "Can not read {filename}. If you don't have any SSH key, "
                     "please follow the steps describe here:\n  {doc_url}"
                 ).format(filename=ssh_key_file, doc_url=doc_url)
             )
             raise
@@ -778,15 +781,15 @@
     def fqdn(self):
         return self.get_metadata("fqdn")
 
     @fqdn.setter
     def fqdn(self, value):
         fqdn_validate = re.compile(r"^[\.a-z0-9]+$", re.IGNORECASE)
         if not value or not fqdn_validate.match(value):
-            logger.error("Invalid FQDN: {value}".format(value=value))
+            logger.error(f"Invalid FQDN: {value}")
             return
         self.user_data["fqdn"] = value
         self.record_metadata("fqdn", value)
 
     @property
     def vcpus(self):
         xml = self.dom.XMLDesc(0)
@@ -824,18 +827,18 @@
         )
         self.dom.setMemoryFlags(value, libvirt.VIR_DOMAIN_AFFECT_CONFIG)
 
     def get_next_block_device(self):
         if not hasattr(self, "blockdev"):
             self.blockdev = list(string.ascii_lowercase)
             self.blockdev.reverse()
-        return "vd{block}".format(block=self.blockdev.pop())
+        return f"vd{self.blockdev.pop()}"
 
     def record_metadata(self, k, v):
-        meta = "<{k} name='{v}' />".format(k=k, v=v)
+        meta = f"<{k} name='{v}' />"
         self.dom.setMetadata(
             libvirt.VIR_DOMAIN_METADATA_ELEMENT,
             meta,
             "vl",
             k,
             libvirt.VIR_DOMAIN_AFFECT_CONFIG,
         )
@@ -866,15 +869,15 @@
         return value.split(",")
 
     @groups.setter
     def groups(self, value):
         self.record_metadata("groups", ",".join(value))
 
     def attach_disk(self, volume, device="disk", disk_type="qcow2"):
-        if device == "cdrom":
+        if device == "cdrom":  # noqa: SIM108
             # virtio does not support ejectable media
             bus = "ide"
         else:
             bus = self.default_bus_type or "virtio"
 
         device_name = self.get_next_block_device()
         disk_root = ET.fromstring(DISK_XML)
@@ -999,9 +1002,9 @@
         os.execlp(
             "ssh",
             "ssh",
             "-o",
             "StrictHostKeyChecking=no",
             "-o",
             "UserKnownHostsFile=/dev/null",
-            "{username}@{ipv4}".format(username=self.username, ipv4=self.ipv4.ip),
+            f"{self.username}@{self.ipv4.ip}",
         )
```

### Comparing `virt-lightning-2.2.0/virt_lightning.egg-info/PKG-INFO` & `virt-lightning-2.3.0/virt_lightning.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,22 @@
 Metadata-Version: 2.1
 Name: virt-lightning
-Version: 2.2.0
+Version: 2.3.0
 Summary: Deploy your testing VM in a couple of seconds
-Home-page: https://virt-lightning.org
-Author: Gonéri Le Bouder
-Author-email: goneri@lebouder.net
-License: Apache v2.0
-Platform: linux
+Author-email: Gonéri Le Bouder <goneri@lebouder.net>
+Project-URL: Homepage, https://https://virt-lightning.org/
+Project-URL: Source, https://github.com/virt-lightning/virt-lightning
+Keywords: libvirt,cloud,qemu,cloudinit
 Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Topic :: System :: Distributed Computing
+Classifier: Operating System :: POSIX :: Linux
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: test
 License-File: LICENSE-2.0.txt
 
 # 🗲 spawn Cloud instances on libvirt!🗲
 
 
 [![Build Status](https://travis-ci.org/virt-lightning/virt-lightning.svg?branch=master)](https://travis-ci.org/virt-lightning/virt-lightning)
 [![PyPI version](https://badge.fury.io/py/virt-lightning.svg)](https://badge.fury.io/py/virt-lightning)
```

### Comparing `virt-lightning-2.2.0/virt_lightning.egg-info/SOURCES.txt` & `virt-lightning-2.3.0/virt_lightning.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 .gitignore
-DEBUGGING.md
 LICENSE-2.0.txt
 MANIFEST.in
 README.md
-azure-pipelines.yml
 changelog.md
+pyproject.toml
 requirements.txt
-setup.py
 test-requirements.txt
 tox.ini
+.github/workflows/codeql.yml
+.github/workflows/ruff.yml
 .github/workflows/tests.yml
+.github/workflows/tox.yml
 conf/example.ini
 logo/logo.png
 logo/logo.svg
 logo/logo_no_text.png
 tests/conftest.py
 tests/test_configure.py
 tests/test_domain.py
```

