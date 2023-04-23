# Comparing `tmp/giftmaster-0.0.9.tar.gz` & `tmp/giftmaster-0.1.54.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giftmaster-0.0.9.tar", last modified: Sun Feb  6 04:21:40 2022, max compression
+gzip compressed data, was "giftmaster-0.1.54.tar", last modified: Sun Apr 23 15:14:44 2023, max compression
```

## Comparing `giftmaster-0.0.9.tar` & `giftmaster-0.1.54.tar`

### file list

```diff
@@ -1,46 +1,48 @@
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2022-02-06 04:21:40.708921 giftmaster-0.0.9/
--rw-r--r--   0 mtm        (501) staff       (20)     7294 2022-02-04 20:07:10.000000 giftmaster-0.0.9/.cirrus.yml
--rw-r--r--   0 mtm        (501) staff       (20)      593 2022-02-04 20:07:10.000000 giftmaster-0.0.9/.coveragerc
--rw-r--r--   0 mtm        (501) staff       (20)      550 2022-02-04 20:07:10.000000 giftmaster-0.0.9/.gitignore
--rw-r--r--   0 mtm        (501) staff       (20)       58 2022-02-04 20:07:10.000000 giftmaster-0.0.9/.isort.cfg
--rw-r--r--   0 mtm        (501) staff       (20)     1330 2022-02-04 20:07:10.000000 giftmaster-0.0.9/.pre-commit-config.yaml
--rw-r--r--   0 mtm        (501) staff       (20)      490 2022-02-04 20:07:10.000000 giftmaster-0.0.9/.readthedocs.yml
--rw-r--r--   0 mtm        (501) staff       (20)       87 2022-02-04 20:07:10.000000 giftmaster-0.0.9/AUTHORS.rst
--rw-r--r--   0 mtm        (501) staff       (20)      128 2022-02-04 20:07:10.000000 giftmaster-0.0.9/CHANGELOG.rst
--rw-r--r--   0 mtm        (501) staff       (20)    13862 2022-02-04 20:07:10.000000 giftmaster-0.0.9/CONTRIBUTING.rst
--rw-r--r--   0 mtm        (501) staff       (20)    15922 2022-02-04 20:07:10.000000 giftmaster-0.0.9/LICENSE.txt
--rw-r--r--   0 mtm        (501) staff       (20)     2588 2022-02-06 04:21:40.709154 giftmaster-0.0.9/PKG-INFO
--rw-r--r--   0 mtm        (501) staff       (20)     2103 2022-02-04 20:07:10.000000 giftmaster-0.0.9/README.rst
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2022-02-06 04:21:40.703386 giftmaster-0.0.9/docs/
--rw-r--r--   0 mtm        (501) staff       (20)     1154 2022-02-04 20:07:10.000000 giftmaster-0.0.9/docs/Makefile
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2022-02-06 04:21:40.703903 giftmaster-0.0.9/docs/_static/
--rw-r--r--   0 mtm        (501) staff       (20)       18 2022-02-04 20:07:10.000000 giftmaster-0.0.9/docs/_static/.gitignore
--rw-r--r--   0 mtm        (501) staff       (20)       41 2022-02-04 20:07:10.000000 giftmaster-0.0.9/docs/authors.rst
--rw-r--r--   0 mtm        (501) staff       (20)       43 2022-02-04 20:07:10.000000 giftmaster-0.0.9/docs/changelog.rst
--rw-r--r--   0 mtm        (501) staff       (20)     9757 2022-02-04 20:07:10.000000 giftmaster-0.0.9/docs/conf.py
--rw-r--r--   0 mtm        (501) staff       (20)       33 2022-02-04 20:07:10.000000 giftmaster-0.0.9/docs/contributing.rst
--rw-r--r--   0 mtm        (501) staff       (20)     2325 2022-02-04 20:07:10.000000 giftmaster-0.0.9/docs/index.rst
--rw-r--r--   0 mtm        (501) staff       (20)       67 2022-02-04 20:07:10.000000 giftmaster-0.0.9/docs/license.rst
--rw-r--r--   0 mtm        (501) staff       (20)       39 2022-02-04 20:07:10.000000 giftmaster-0.0.9/docs/readme.rst
--rw-r--r--   0 mtm        (501) staff       (20)      233 2022-02-04 20:07:10.000000 giftmaster-0.0.9/docs/requirements.txt
--rw-r--r--   0 mtm        (501) staff       (20)      355 2022-02-04 20:07:10.000000 giftmaster-0.0.9/pyproject.toml
--rw-r--r--   0 mtm        (501) staff       (20)     1311 2022-02-06 04:21:40.710164 giftmaster-0.0.9/setup.cfg
--rw-r--r--   0 mtm        (501) staff       (20)      707 2022-02-04 20:07:10.000000 giftmaster-0.0.9/setup.py
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2022-02-06 04:21:40.687884 giftmaster-0.0.9/src/
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2022-02-06 04:21:40.705323 giftmaster-0.0.9/src/giftmaster/
--rw-r--r--   0 mtm        (501) staff       (20)      577 2022-02-04 20:07:10.000000 giftmaster-0.0.9/src/giftmaster/__init__.py
--rw-r--r--   0 mtm        (501) staff       (20)     2394 2022-02-06 04:14:20.000000 giftmaster-0.0.9/src/giftmaster/signtool.py
--rw-r--r--   0 mtm        (501) staff       (20)     3962 2022-02-06 04:21:12.000000 giftmaster-0.0.9/src/giftmaster/skeleton.py
--rw-r--r--   0 mtm        (501) staff       (20)      456 2022-02-04 21:38:03.000000 giftmaster-0.0.9/src/giftmaster/timestamp.py
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2022-02-06 04:21:40.708003 giftmaster-0.0.9/src/giftmaster.egg-info/
--rw-r--r--   0 mtm        (501) staff       (20)     2588 2022-02-06 04:21:40.000000 giftmaster-0.0.9/src/giftmaster.egg-info/PKG-INFO
--rw-r--r--   0 mtm        (501) staff       (20)      790 2022-02-06 04:21:40.000000 giftmaster-0.0.9/src/giftmaster.egg-info/SOURCES.txt
--rw-r--r--   0 mtm        (501) staff       (20)        1 2022-02-06 04:21:40.000000 giftmaster-0.0.9/src/giftmaster.egg-info/dependency_links.txt
--rw-r--r--   0 mtm        (501) staff       (20)       56 2022-02-06 04:21:40.000000 giftmaster-0.0.9/src/giftmaster.egg-info/entry_points.txt
--rw-r--r--   0 mtm        (501) staff       (20)        1 2022-02-04 20:15:39.000000 giftmaster-0.0.9/src/giftmaster.egg-info/not-zip-safe
--rw-r--r--   0 mtm        (501) staff       (20)      124 2022-02-06 04:21:40.000000 giftmaster-0.0.9/src/giftmaster.egg-info/requires.txt
--rw-r--r--   0 mtm        (501) staff       (20)       11 2022-02-06 04:21:40.000000 giftmaster-0.0.9/src/giftmaster.egg-info/top_level.txt
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2022-02-06 04:21:40.708614 giftmaster-0.0.9/tests/
--rw-r--r--   0 mtm        (501) staff       (20)      278 2022-02-04 20:07:10.000000 giftmaster-0.0.9/tests/conftest.py
--rw-r--r--   0 mtm        (501) staff       (20)      826 2022-02-04 21:40:08.000000 giftmaster-0.0.9/tests/test_skeleton.py
--rw-r--r--   0 mtm        (501) staff       (20)     2007 2022-02-04 20:07:10.000000 giftmaster-0.0.9/tox.ini
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-23 15:14:44.199430 giftmaster-0.1.54/
+-rw-r--r--   0 mtm        (501) staff       (20)     7843 2022-10-29 23:46:59.000000 giftmaster-0.1.54/.cirrus.yml
+-rw-r--r--   0 mtm        (501) staff       (20)      593 2022-02-04 20:07:10.000000 giftmaster-0.1.54/.coveragerc
+-rw-r--r--   0 mtm        (501) staff       (20)      550 2022-02-04 20:07:10.000000 giftmaster-0.1.54/.gitignore
+-rw-r--r--   0 mtm        (501) staff       (20)       58 2022-02-04 20:07:10.000000 giftmaster-0.1.54/.isort.cfg
+-rw-r--r--   0 mtm        (501) staff       (20)     1330 2022-02-04 20:07:10.000000 giftmaster-0.1.54/.pre-commit-config.yaml
+-rw-r--r--   0 mtm        (501) staff       (20)      490 2022-02-04 20:07:10.000000 giftmaster-0.1.54/.readthedocs.yml
+-rw-r--r--   0 mtm        (501) staff       (20)       87 2022-02-04 20:07:10.000000 giftmaster-0.1.54/AUTHORS.rst
+-rw-r--r--   0 mtm        (501) staff       (20)      128 2022-02-04 20:07:10.000000 giftmaster-0.1.54/CHANGELOG.rst
+-rw-r--r--   0 mtm        (501) staff       (20)    13862 2022-02-04 20:07:10.000000 giftmaster-0.1.54/CONTRIBUTING.rst
+-rw-r--r--   0 mtm        (501) staff       (20)    15922 2022-02-04 20:07:10.000000 giftmaster-0.1.54/LICENSE.txt
+-rw-r--r--   0 mtm        (501) staff       (20)     2587 2023-04-23 15:14:44.199681 giftmaster-0.1.54/PKG-INFO
+-rw-r--r--   0 mtm        (501) staff       (20)     2103 2022-02-04 20:07:10.000000 giftmaster-0.1.54/README.rst
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-23 15:14:44.186027 giftmaster-0.1.54/docs/
+-rw-r--r--   0 mtm        (501) staff       (20)     1154 2022-02-04 20:07:10.000000 giftmaster-0.1.54/docs/Makefile
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-23 15:14:44.187393 giftmaster-0.1.54/docs/_static/
+-rw-r--r--   0 mtm        (501) staff       (20)       18 2022-02-04 20:07:10.000000 giftmaster-0.1.54/docs/_static/.gitignore
+-rw-r--r--   0 mtm        (501) staff       (20)       41 2022-02-04 20:07:10.000000 giftmaster-0.1.54/docs/authors.rst
+-rw-r--r--   0 mtm        (501) staff       (20)       43 2022-02-04 20:07:10.000000 giftmaster-0.1.54/docs/changelog.rst
+-rw-r--r--   0 mtm        (501) staff       (20)     9757 2022-02-04 20:07:10.000000 giftmaster-0.1.54/docs/conf.py
+-rw-r--r--   0 mtm        (501) staff       (20)       33 2022-02-04 20:07:10.000000 giftmaster-0.1.54/docs/contributing.rst
+-rw-r--r--   0 mtm        (501) staff       (20)     2325 2022-02-04 20:07:10.000000 giftmaster-0.1.54/docs/index.rst
+-rw-r--r--   0 mtm        (501) staff       (20)       67 2022-02-04 20:07:10.000000 giftmaster-0.1.54/docs/license.rst
+-rw-r--r--   0 mtm        (501) staff       (20)       39 2022-02-04 20:07:10.000000 giftmaster-0.1.54/docs/readme.rst
+-rw-r--r--   0 mtm        (501) staff       (20)      233 2022-02-04 20:07:10.000000 giftmaster-0.1.54/docs/requirements.txt
+-rw-r--r--   0 mtm        (501) staff       (20)      355 2022-02-04 20:07:10.000000 giftmaster-0.1.54/pyproject.toml
+-rw-r--r--   0 mtm        (501) staff       (20)     1316 2023-04-23 15:14:44.201179 giftmaster-0.1.54/setup.cfg
+-rw-r--r--   0 mtm        (501) staff       (20)      707 2022-02-04 20:07:10.000000 giftmaster-0.1.54/setup.py
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-23 15:14:44.168588 giftmaster-0.1.54/src/
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-23 15:14:44.192505 giftmaster-0.1.54/src/giftmaster/
+-rw-r--r--   0 mtm        (501) staff       (20)      577 2022-02-04 20:07:10.000000 giftmaster-0.1.54/src/giftmaster/__init__.py
+-rw-r--r--   0 mtm        (501) staff       (20)     1784 2022-02-15 06:24:57.000000 giftmaster-0.1.54/src/giftmaster/args.py
+-rw-r--r--   0 mtm        (501) staff       (20)     1417 2022-02-15 06:29:02.000000 giftmaster-0.1.54/src/giftmaster/logger.py
+-rw-r--r--   0 mtm        (501) staff       (20)     4718 2023-04-23 15:13:57.000000 giftmaster-0.1.54/src/giftmaster/signtool.py
+-rw-r--r--   0 mtm        (501) staff       (20)     1577 2022-02-26 07:06:58.000000 giftmaster-0.1.54/src/giftmaster/skeleton.py
+-rw-r--r--   0 mtm        (501) staff       (20)      456 2022-02-15 20:24:25.000000 giftmaster-0.1.54/src/giftmaster/timestamp.py
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-23 15:14:44.197567 giftmaster-0.1.54/src/giftmaster.egg-info/
+-rw-r--r--   0 mtm        (501) staff       (20)     2587 2023-04-23 15:14:44.000000 giftmaster-0.1.54/src/giftmaster.egg-info/PKG-INFO
+-rw-r--r--   0 mtm        (501) staff       (20)      838 2023-04-23 15:14:44.000000 giftmaster-0.1.54/src/giftmaster.egg-info/SOURCES.txt
+-rw-r--r--   0 mtm        (501) staff       (20)        1 2023-04-23 15:14:44.000000 giftmaster-0.1.54/src/giftmaster.egg-info/dependency_links.txt
+-rw-r--r--   0 mtm        (501) staff       (20)       55 2023-04-23 15:14:44.000000 giftmaster-0.1.54/src/giftmaster.egg-info/entry_points.txt
+-rw-r--r--   0 mtm        (501) staff       (20)        1 2022-10-02 20:49:51.000000 giftmaster-0.1.54/src/giftmaster.egg-info/not-zip-safe
+-rw-r--r--   0 mtm        (501) staff       (20)      117 2023-04-23 15:14:44.000000 giftmaster-0.1.54/src/giftmaster.egg-info/requires.txt
+-rw-r--r--   0 mtm        (501) staff       (20)       11 2023-04-23 15:14:44.000000 giftmaster-0.1.54/src/giftmaster.egg-info/top_level.txt
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-23 15:14:44.198900 giftmaster-0.1.54/tests/
+-rw-r--r--   0 mtm        (501) staff       (20)      278 2022-02-04 20:07:10.000000 giftmaster-0.1.54/tests/conftest.py
+-rw-r--r--   0 mtm        (501) staff       (20)     2347 2022-02-08 00:13:30.000000 giftmaster-0.1.54/tests/test_skeleton.py
+-rw-r--r--   0 mtm        (501) staff       (20)     2030 2022-02-08 00:27:22.000000 giftmaster-0.1.54/tox.ini
```

### Comparing `giftmaster-0.0.9/.cirrus.yml` & `giftmaster-0.1.54/.cirrus.yml`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
   clean_workspace_script:
     # Avoid information carried from one run to the other
     - rm -rf .coverage junit-*.xml .tox
   # The following scripts are also used in Windows, be aware the shell is not POSIX
   build_script: &build
     - python -m tox -e build  # Ensure PEP517-style build works
   test_script: &test
-    - python -m tox -- -rfEx --durations 10 --color yes
+    - python -m tox -- -rfEx --durations 10 --color yes --verbose
     # ^  tox is better if invoked as a module on Windows/OSX
 
 
 # Deep clone script for POSIX environments (required for setuptools-scm)
 .clone_script: &clone |
   if [ -z "$CIRRUS_PR" ]; then
     git clone --recursive --branch=$CIRRUS_BRANCH https://x-access-token:${CIRRUS_REPO_CLONE_TOKEN}@github.com/${CIRRUS_REPO_FULL_NAME}.git $CIRRUS_WORKING_DIR
@@ -53,14 +53,15 @@
     git reset --hard $CIRRUS_CHANGE_IN_REPO
   fi
 
 
 # ---- Task definitions ----
 
 linux_mac_task:
+  only_if: "$skip_these_tests == '1'"  #blocking these test from running
   # Use custom cloning since otherwise git tags are missing
   clone_script: *clone
   matrix:
     - name: test (Linux - 3.6)
       container: {image: "python:3.6-buster"}
     - name: test (Linux - 3.7)
       container: {image: "python:3.7-buster"}
@@ -111,20 +112,20 @@
       git reset --hard %CIRRUS_CHANGE_IN_REPO%
     ) ELSE (
       git clone --recursive https://x-access-token:%CIRRUS_REPO_CLONE_TOKEN%@github.com/%CIRRUS_REPO_FULL_NAME%.git %CIRRUS_WORKING_DIR% &
       git fetch origin pull/%CIRRUS_PR%/head:pull/%CIRRUS_PR% &
       git reset --hard %CIRRUS_CHANGE_IN_REPO%
     )
   windows_container:
-    image: "python:3.8-windowsservercore"
+    image: "cirrusci/windowsservercore:2019"
     os_version: 2019
   env:
     # Single quotes are used bellow to escape Windows backslash and % (YAML restrictions).
-    PYTHON_HOME: 'C:\Python'
-    PYTHON_APPDATA: '%APPDATA%\Python\Python38'
+    PYTHON_HOME: 'C:\Python310'
+    PYTHON_APPDATA: '%APPDATA%\Python\Python310'
     # ^  update when python version changes
     GIT_HOME: 'C:\tools\GitForWindows.2.34.1\tools'
     # ^ update when git version changes
     HOME: '%USERPROFILE%'
     USERNAME: ContainerAdministrator
     # ^  ensure USERNAME is set in Windows, so the getpass module doesn't raise exceptions
     PATH: '%HOME%\.local\bin\;%PYTHON_APPDATA%\Scripts\;%PYTHON_HOME%\;%PYTHON_HOME%\Scripts\;C:\tools\;%GIT_HOME%\cmd\;%PATH%'
@@ -132,14 +133,20 @@
     PIP_CACHE: '%LocalAppData%\pip\Cache'
     PIP_TRUSTED_HOST: 'pypi.org pypi.python.org files.pythonhosted.org'
     PIP_CONFIG_FILE: '%AppData%\pip\pip.ini'
     COVERAGE: 'NO'
   pip_cache:
     folder: '%PIP_CACHE%'
   install_script:
+    - choco config set cacheLocation %CIRRUS_WORKING_DIR%/.chocolatey
+    - choco feature enable -n allowGlobalConfirmation
+    - choco feature disable -n showDownloadProgress
+    - choco install python
+    - python -m pip install --upgrade pip
+    - choco install windows-sdk-10.1 --override-arguments --install-args="'/quiet /features Optionid.MSIInstallTools Optionid.SigningTools'"
     # Activate long file paths to avoid some errors
     - REG ADD "HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\FileSystem" /v LongPathsEnabled /t REG_DWORD /d 1 /f
     # Set Windows encoding to UTF-8
     - REG ADD "HKEY_CURRENT_USER\Software\Microsoft\Command Processor" /v Autorun /t REG_SZ /d "@chcp 65001>nul" /f
     - python -m ensurepip
     - python -m pip install --upgrade --user pip setuptools certifi tox
   prepare_script: *prepare
@@ -148,14 +155,15 @@
     # CMD is not capable of globbing, so we have to use PowerShell
     - ps: (rm -Recurse -Force -ErrorAction SilentlyContinue .tox,junit-*.xml)
   build_script: *build
   test_script: *test
 
 
 coverage_task:
+  only_if: "$skip_these_tests == '1'"  #blocking these test from running
   name: coverage (Linux - 3.6)
   clone_script: *clone
   container: {image: "python:3.6-buster"}
   env:
     COVERAGE: yes
     PRE_COMMIT_HOME: ${HOME}/.cache/pre-commit
   depends_on:
```

### Comparing `giftmaster-0.0.9/.coveragerc` & `giftmaster-0.1.54/.coveragerc`

 * *Files identical despite different names*

### Comparing `giftmaster-0.0.9/.gitignore` & `giftmaster-0.1.54/.gitignore`

 * *Files identical despite different names*

### Comparing `giftmaster-0.0.9/.pre-commit-config.yaml` & `giftmaster-0.1.54/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `giftmaster-0.0.9/CONTRIBUTING.rst` & `giftmaster-0.1.54/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `giftmaster-0.0.9/LICENSE.txt` & `giftmaster-0.1.54/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `giftmaster-0.0.9/PKG-INFO` & `giftmaster-0.1.54/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: giftmaster
-Version: 0.0.9
+Version: 0.1.54
 Summary: Add a short description here!
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: Taylor Monacelli
 Author-email: taylormonacelli@gmail.com
 License: MPL-2.0
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
@@ -77,9 +77,7 @@
 .. _pre-commit: https://pre-commit.com/
 
 Note
 ====
 
 This project has been set up using PyScaffold 4.1.4. For details and usage
 information on PyScaffold see https://pyscaffold.org/.
-
-
```

### Comparing `giftmaster-0.0.9/README.rst` & `giftmaster-0.1.54/README.rst`

 * *Files identical despite different names*

### Comparing `giftmaster-0.0.9/docs/Makefile` & `giftmaster-0.1.54/docs/Makefile`

 * *Files identical despite different names*

### Comparing `giftmaster-0.0.9/docs/conf.py` & `giftmaster-0.1.54/docs/conf.py`

 * *Files identical despite different names*

### Comparing `giftmaster-0.0.9/docs/index.rst` & `giftmaster-0.1.54/docs/index.rst`

 * *Files identical despite different names*

### Comparing `giftmaster-0.0.9/setup.cfg` & `giftmaster-0.1.54/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -32,26 +32,25 @@
 
 [options.extras_require]
 testing = 
 	setuptools
 	pytest
 	pytest-cov
 	pip-tools
-	pytest
 	black
 	isort
 
 [options.entry_points]
 console_scripts = 
 	giftmaster = giftmaster.skeleton:run
 
 [tool:pytest]
 addopts = 
 	--cov giftmaster --cov-report term-missing
-	--verbose
+	--verbose --capture=no
 norecursedirs = 
 	dist
 	build
 	.tox
 testpaths = tests
 
 [devpi:upload]
```

### Comparing `giftmaster-0.0.9/setup.py` & `giftmaster-0.1.54/setup.py`

 * *Files identical despite different names*

### Comparing `giftmaster-0.0.9/src/giftmaster/__init__.py` & `giftmaster-0.1.54/src/giftmaster/__init__.py`

 * *Files identical despite different names*

### Comparing `giftmaster-0.0.9/src/giftmaster.egg-info/PKG-INFO` & `giftmaster-0.1.54/src/giftmaster.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: giftmaster
-Version: 0.0.9
+Version: 0.1.54
 Summary: Add a short description here!
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: Taylor Monacelli
 Author-email: taylormonacelli@gmail.com
 License: MPL-2.0
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
@@ -77,9 +77,7 @@
 .. _pre-commit: https://pre-commit.com/
 
 Note
 ====
 
 This project has been set up using PyScaffold 4.1.4. For details and usage
 information on PyScaffold see https://pyscaffold.org/.
-
-
```

### Comparing `giftmaster-0.0.9/src/giftmaster.egg-info/SOURCES.txt` & `giftmaster-0.1.54/src/giftmaster.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 docs/contributing.rst
 docs/index.rst
 docs/license.rst
 docs/readme.rst
 docs/requirements.txt
 docs/_static/.gitignore
 src/giftmaster/__init__.py
+src/giftmaster/args.py
+src/giftmaster/logger.py
 src/giftmaster/signtool.py
 src/giftmaster/skeleton.py
 src/giftmaster/timestamp.py
 src/giftmaster.egg-info/PKG-INFO
 src/giftmaster.egg-info/SOURCES.txt
 src/giftmaster.egg-info/dependency_links.txt
 src/giftmaster.egg-info/entry_points.txt
```

### Comparing `giftmaster-0.0.9/tox.ini` & `giftmaster-0.1.54/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 setenv =
     TOXINIDIR = {toxinidir}
 passenv =
     HOME
 extras =
     testing
 commands =
-    pytest {posargs}
+    pytest {posargs} --capture=no --verbose
 
 
 [testenv:{build,clean}]
 description =
     build: Build the package in isolation according to PEP517, see https://github.com/pypa/build
     clean: Remove old distribution files and temporary build artifacts (./build and ./dist)
 # https://setuptools.pypa.io/en/stable/build_meta.html#how-to-use-it
```

