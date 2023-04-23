# Comparing `tmp/travis_emulator-2.0.3.tar.gz` & `tmp/travis_emulator-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/travis_emulator-2.0.3.tar", last modified: Sun Dec  4 19:46:35 2022, max compression
+gzip compressed data, was "travis_emulator-2.0.4.tar", last modified: Sun Apr 23 14:03:50 2023, max compression
```

## Comparing `travis_emulator-2.0.3.tar` & `travis_emulator-2.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2022-12-04 19:46:35.000000 travis_emulator-2.0.3/
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2022-12-04 19:46:35.000000 travis_emulator-2.0.3/travis_emulator/
--rwxr-xr-x   0 odoo      (1000) odoo      (1000)      164 2022-09-09 18:30:58.000000 travis_emulator-2.0.3/travis_emulator/__main__.py
--rw-r--r--   0 odoo      (1000) odoo      (1000)     4853 2022-11-11 07:31:59.000000 travis_emulator-2.0.3/travis_emulator/make_travis_conf.py
--rw-r--r--   0 odoo      (1000) odoo      (1000)     3673 2022-11-05 10:12:53.000000 travis_emulator-2.0.3/travis_emulator/template_travis.yml
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2022-12-04 19:46:35.000000 travis_emulator-2.0.3/travis_emulator/scripts/
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     3275 2022-12-04 19:15:33.000000 travis_emulator-2.0.3/travis_emulator/scripts/setup.info
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     7460 2022-12-04 14:33:09.000000 travis_emulator-2.0.3/travis_emulator/scripts/main.py
--rw-r--r--   0 odoo      (1000) odoo      (1000)       43 2022-10-15 13:09:45.000000 travis_emulator-2.0.3/travis_emulator/scripts/__init__.py
--rwxr-xr-x   0 odoo      (1000) odoo      (1000)     9772 2022-09-09 18:30:58.000000 travis_emulator-2.0.3/travis_emulator/travis.man
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    39094 2022-12-04 14:33:09.000000 travis_emulator-2.0.3/travis_emulator/travisrc
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    46854 2022-12-04 14:33:09.000000 travis_emulator-2.0.3/travis_emulator/travis
--rw-r--r--   0 odoo      (1000) odoo      (1000)       77 2022-11-05 14:11:39.000000 travis_emulator-2.0.3/travis_emulator/__init__.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       38 2022-12-04 19:46:35.000000 travis_emulator-2.0.3/setup.cfg
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     3275 2022-12-04 14:33:09.000000 travis_emulator-2.0.3/setup.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2022-12-04 19:46:35.000000 travis_emulator-2.0.3/travis_emulator.egg-info/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       16 2022-12-04 19:46:35.000000 travis_emulator-2.0.3/travis_emulator.egg-info/top_level.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2022-12-04 19:46:35.000000 travis_emulator-2.0.3/travis_emulator.egg-info/dependency_links.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2022-11-09 12:38:21.000000 travis_emulator-2.0.3/travis_emulator.egg-info/not-zip-safe
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      145 2022-12-04 19:46:35.000000 travis_emulator-2.0.3/travis_emulator.egg-info/entry_points.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      599 2022-12-04 19:46:35.000000 travis_emulator-2.0.3/travis_emulator.egg-info/SOURCES.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       13 2022-12-04 19:46:35.000000 travis_emulator-2.0.3/travis_emulator.egg-info/requires.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2848 2022-12-04 19:46:35.000000 travis_emulator-2.0.3/travis_emulator.egg-info/PKG-INFO
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2848 2022-12-04 19:46:35.000000 travis_emulator-2.0.3/PKG-INFO
--rw-r--r--   0 odoo      (1000) odoo      (1000)    20561 2022-12-04 19:46:35.000000 travis_emulator-2.0.3/README.rst
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-23 14:03:50.035239 travis_emulator-2.0.4/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2607 2023-04-23 14:03:50.035239 travis_emulator-2.0.4/PKG-INFO
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    20883 2023-04-23 14:03:49.000000 travis_emulator-2.0.4/README.rst
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       38 2023-04-23 14:03:50.035239 travis_emulator-2.0.4/setup.cfg
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     3324 2023-04-15 07:38:01.000000 travis_emulator-2.0.4/setup.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-23 14:03:50.035239 travis_emulator-2.0.4/travis_emulator/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       77 2022-12-09 05:08:44.000000 travis_emulator-2.0.4/travis_emulator/__init__.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      164 2022-12-09 05:08:44.000000 travis_emulator-2.0.4/travis_emulator/__main__.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5097 2023-04-14 13:30:50.000000 travis_emulator-2.0.4/travis_emulator/make_travis_conf.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-23 14:03:50.035239 travis_emulator-2.0.4/travis_emulator/scripts/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       43 2022-12-09 05:08:44.000000 travis_emulator-2.0.4/travis_emulator/scripts/__init__.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     7460 2023-04-15 07:33:00.000000 travis_emulator-2.0.4/travis_emulator/scripts/main.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     3324 2023-04-23 13:43:49.000000 travis_emulator-2.0.4/travis_emulator/scripts/setup.info
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     3683 2023-04-13 17:52:56.000000 travis_emulator-2.0.4/travis_emulator/template_travis.yml
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    47417 2023-04-15 08:02:21.000000 travis_emulator-2.0.4/travis_emulator/travis
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     9772 2022-12-09 05:08:44.000000 travis_emulator-2.0.4/travis_emulator/travis.man
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    39019 2023-04-15 08:02:21.000000 travis_emulator-2.0.4/travis_emulator/travisrc
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-23 14:03:50.035239 travis_emulator-2.0.4/travis_emulator.egg-info/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2607 2023-04-23 14:03:50.000000 travis_emulator-2.0.4/travis_emulator.egg-info/PKG-INFO
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      599 2023-04-23 14:03:50.000000 travis_emulator-2.0.4/travis_emulator.egg-info/SOURCES.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-04-23 14:03:50.000000 travis_emulator-2.0.4/travis_emulator.egg-info/dependency_links.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      145 2023-04-23 14:03:50.000000 travis_emulator-2.0.4/travis_emulator.egg-info/entry_points.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2022-12-09 08:51:08.000000 travis_emulator-2.0.4/travis_emulator.egg-info/not-zip-safe
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       13 2023-04-23 14:03:50.000000 travis_emulator-2.0.4/travis_emulator.egg-info/requires.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       16 2023-04-23 14:03:50.000000 travis_emulator-2.0.4/travis_emulator.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `travis_emulator-2.0.3/travis_emulator/make_travis_conf.py` & `travis_emulator-2.0.4/travis_emulator/make_travis_conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,18 +32,19 @@
              and ctx["TRAVIS_PYTHON_VERSION"].startswith("2"))
             or (re.match(r"^ *\- *[\"']?2", line)
                 and ctx["TRAVIS_PYTHON_VERSION"].startswith("3"))
         ):
             line = comment_line(line)
     elif section == "before_install":
         if re.match(r"^ *\- \$HOME/tools/install_tools.sh", line):
+            verbose = "q" if int(ctx["TRAVIS_DEBUG_MODE"]) < 3 else "vv"
             if ctx["TRAVIS_PYTHON_VERSION"].startswith("2"):
-                line = "  - $HOME/tools/install_tools.sh -qpt2"
+                line = "  - $HOME/tools/install_tools.sh -%spt2" % verbose
             else:
-                line = "  - $HOME/tools/install_tools.sh -qpt"
+                line = "  - $HOME/tools/install_tools.sh -%spt" % verbose
     elif section == "install":
         if re.match(r"^ *\- travis_install_env", line):
             if ctx["PRJNAME"] == "Odoo":
                 line = "  - travis_install_env"
             else:
                 line = "  - travis_install_env tools"
     elif section == "env.global":
@@ -86,28 +87,31 @@
     src = cli_args[0]
     tgt = cli_args[1]
     ctx = {
         "PKGNAME": os_env("PKGNAME", os.path.basename(os.getcwd())),
         "PRJNAME": os_env("PRJNAME"),
         "REPOSNAME": os_env("REPOSNAME"),
         "TRAVIS_BRANCH": os_env("TRAVIS_BRANCH", os_env("BRANCH")),
+        "TRAVIS_DEBUG_MODE": os_env("TRAVIS_DEBUG_MODE", "0"),
         "TRAVIS_BUILD_DIR": os_env("TRAVIS_BUILD_DIR", os.getcwd()),
         "TRAVIS_PYTHON_VERSION": os_env("TRAVIS_PYTHON_VERSION"),
         "TRAVIS_REPO_SLUG":
             os_env("TRAVIS_REPO_SLUG", "local/%s" % os.path.basename(os.getcwd())),
     }
     odoo_main_version = ctx["TRAVIS_BRANCH"].split(".")[0]
     ctx["GIT_ORG"] = "zeroincombenze"
     if odoo_main_version.isdigit():
         odoo_main_version = eval(odoo_main_version)
         ctx["ODOO_MAIN_VERSION"] = odoo_main_version
         if odoo_main_version >= 12:
             ctx["GIT_ORG"] = "librerp"
         if odoo_main_version <= 10:
             ctx["TRAVIS_PYTHON_VERSION"] = "2.7"
+        elif odoo_main_version < 14:
+            ctx["TRAVIS_PYTHON_VERSION"] = "3.8"
         else:
             ctx["TRAVIS_PYTHON_VERSION"] = "3.7"
     else:
         ctx["ODOO_MAIN_VERSION"] = 0
 
     contents = section = ""
     with open(src, "r") as fd:
```

### Comparing `travis_emulator-2.0.3/travis_emulator/template_travis.yml` & `travis_emulator-2.0.4/travis_emulator/template_travis.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Odoo yaml template for travis-ci
-# __version__=2.0.2
+# __version__=2.0.4
 # Can used both in local travis emulator both in travis environment
 # Notice: in local travis emulator macroes are substituted in 2 steps:
 # - format: ${macro} are replaced before execution (at travis.yml read)
 # - format: $macro are replace by shell during execution
 
 language: python
 sudo: false
@@ -13,14 +13,15 @@
     - $HOME/.cache/pip
 
 python:
   - "2.7"
   - "3.6"
   - "3.7"
   - "3.8"
+  - "3.9"
 
 virtualenv:
   system_site_packages: false
 
 git:
   submodules: false
   depth: false
```

### Comparing `travis_emulator-2.0.3/travis_emulator/scripts/setup.info` & `travis_emulator-2.0.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='travis_emulator',
-    version='2.0.3',
+    version='2.0.4',
     description='Travis CI emulator for local develop environment',
     long_description="""
 Travis emulator can emulate TravisCi parsing the **.travis.yml** file in local Linux machine.
 You can test your application before pushing code to github.com web site.
 
 Travis emulator can creates all the build declared in **.travis.yml**;
 all the builds are executed in sequential way.
@@ -44,14 +44,15 @@
         'Development Status :: 4 - Beta',
         'License :: OSI Approved :: GNU Affero General Public License v3',
         'Operating System :: POSIX',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
         'Intended Audience :: Developers',
         'Topic :: Software Development',
         'Topic :: Software Development :: Build Tools',
         'Operating System :: OS Independent',
     ],
     keywords='linux travis development',
     url='https://zeroincombenze-tools.readthedocs.io',
```

### Comparing `travis_emulator-2.0.3/travis_emulator/scripts/main.py` & `travis_emulator-2.0.4/travis_emulator/scripts/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 import os
 import sys
 import pkg_resources
 import gzip
 import shutil
 
 
-__version__ = "2.0.3"
+__version__ = "2.0.4"
 
 
 def fake_setup(**kwargs):
     globals()["setup_args"] = kwargs
 
 
 def read_setup():
```

### Comparing `travis_emulator-2.0.3/travis_emulator/travis.man` & `travis_emulator-2.0.4/travis_emulator/travis.man`

 * *Files identical despite different names*

### Comparing `travis_emulator-2.0.3/travis_emulator/travisrc` & `travis_emulator-2.0.4/travis_emulator/travisrc`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env bash
 #
 # Common file for travis emulator scripts
 #
-#__version__=2.0.3
+#__version__=2.0.4
 
 [[ "${BASH_SOURCE-}" == "$0" ]] && echo "You must source this script: \$ source $0" >&2 && exit 33
 XRGI="^(.*\/|)conf\/.*sample$"
 READLINK=$(which greadlink 2>/dev/null) || READLINK=$(which readlink 2>/dev/null)
 export READLINK
 # Based on template 2.0.0
 THIS=$(basename "$0")
@@ -28,16 +28,14 @@
 [[ -z "$Z0LIBDIR" ]] && echo "Library file z0librc not found in <$PYPATH>!" && exit 72
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "Z0LIBDIR=$Z0LIBDIR"
 ODOOLIBDIR=$(findpkg odoorc "$PYPATH" "clodoo")
 [[ -z "$ODOOLIBDIR" ]] && echo "Library file odoorc not found!" && exit 72
 . $ODOOLIBDIR
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "ODOOLIBDIR=$ODOOLIBDIR"
 
-# DIST_CONF=$(findpkg ".z0tools.conf" "$PYPATH")
-# TCONF="$HOME/.z0tools.conf"
 CFG_init "ALL"
 link_cfg_def
 link_cfg $DIST_CONF $TCONF
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "DIST_CONF=$DIST_CONF" && echo "TCONF=$TCONF"
 get_pypi_param ALL
 RED="\e[1;31m"
 GREEN="\e[1;32m"
@@ -625,15 +623,15 @@
   [[ -z $(get_cfg_value "" "MQT_TEST_DB") ]] && CFG_set "MQT_TEST_DB" "test_odoo"
   [[ -z $(get_cfg_value "" "MQT_DBUSER") ]] && CFG_set "MQT_DBUSER" ""
   [[ -z $(get_cfg_value "" "UNBUFFER") ]] && CFG_set "UNBUFFER" "0"
   [[ -z $(get_cfg_value "" "ME_BOS") ]] && CFG_set "ME_BOS" "test_nightly .test_nightly.conf.sample"
   [[ -z $(get_cfg_value "" "Environment") ]] && CFG_set "Environment" "bash"
   [[ -z $(get_cfg_value "" "virtualenv_opts") ]] && CFG_set "virtualenv_opts" ""
   [[ -z $(get_cfg_value "" "NPM_CONFIG_PREFIX") ]] && CFG_set "NPM_CONFIG_PREFIX" "$HOME/.npm-global"
-  [[ -z $(get_cfg_value "" "PYTHON_MATRIX") ]] && CFG_set "PYTHON_MATRIX" "(2.7|3.6|3.7|3.8)"
+  [[ -z $(get_cfg_value "" "PYTHON_MATRIX") ]] && CFG_set "PYTHON_MATRIX" "(2.7|3.6|3.7|3.8|3.9)"
   [[ -z $(get_cfg_value "" "LOGDIR") ]] && CFG_set "LOGDIR" "$HOME/travis_log"
   # Test disabled by default: they are added to EXCLUDE paramater
   [[ -z $(get_cfg_value "" "GBL_EXCLUDE") ]] && CFG_set "GBL_EXCLUDE" "test_impex,test_ir_actions,test_lint,test_main_flows,test_search,test_user_has_group,test_mimetypes"
 }
 
 #
 # [antoniov: 2022-08-06] TODO: remove early
```

### Comparing `travis_emulator-2.0.3/travis_emulator/travis` & `travis_emulator-2.0.4/travis_emulator/travis`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 #
 # Travis-ci emulator
 # Emulate travis-ci on local machine, to test before upgrade git project
 #
 # This free software is released under GNU Affero GPL3
 # author: Antonio M. Vigliotti - antoniomaria.vigliotti@gmail.com
-# (C) 2015-2022 by SHS-AV s.r.l. - http://www.shs-av.com - info@shs-av.com
+# (C) 2015-2023 by SHS-AV s.r.l. - http://www.shs-av.com - info@shs-av.com
 #
 READLINK=$(which greadlink 2>/dev/null) || READLINK=$(which readlink 2>/dev/null)
 export READLINK
 # Based on template 2.0.0
 THIS=$(basename "$0")
 TDIR=$(readlink -f $(dirname $0))
 [ $BASH_VERSINFO -lt 4 ] && echo "This script $0 requires bash 4.0+!" && exit 4
@@ -38,26 +38,24 @@
 . $TRAVISLIBDIR
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "TRAVISLIBDIR=$TRAVISLIBDIR"
 TESTDIR=$(findpkg "" "$TDIR . .." "tests")
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "TESTDIR=$TESTDIR"
 RUNDIR=$(readlink -e $TESTDIR/..)
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "RUNDIR=$RUNDIR"
 
-# DIST_CONF=$(findpkg ".z0tools.conf" "$PYPATH")
-# TCONF="$HOME/.z0tools.conf"
 CFG_init "ALL"
 link_cfg_def
 link_cfg $DIST_CONF $TCONF
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "DIST_CONF=$DIST_CONF" && echo "TCONF=$TCONF"
 get_pypi_param ALL
 RED="\e[1;31m"
 GREEN="\e[1;32m"
 CLR="\e[0m"
 
-__version__=2.0.3
+__version__=2.0.4
 
 
 store_cfg_param_value() {
   #store_cfg_param_value(tid key value [opt] [section])
   local p
   if [[ $2 =~ ^pip_pkgver__ ]]; then
     if [ -z "$PIPPKGVER" ]; then
@@ -96,25 +94,25 @@
     YML_repo=
   fi
   export TRAVIS_PULL_REQUEST="false"
   export MQT_TEMPLATE_DB="$(get_cfg_value "" "MQT_TEMPLATE_DB")$YML_pid"
   export MQT_TEST_DB="$(get_cfg_value "" "MQT_TEST_DB")$YML_pid"
   # export PGUSER="$(get_cfg_value "" "MQT_DBUSER")"
   [[ -z $PGUSER ]] && export PGUSER=$(get_dbuser)
-  python_ver_req=""
-  python_ver_ena=""
-  [[ -f $PRJPATH/travis.ini ]] && python_ver_ena=$(cat $PRJPATH/travis.ini|grep "^PYPI_RUN_PYVER"|awk -F= '{print $2}'|grep --color=never -Eo "[0-9.]+"|head -n1)
+  python_ver_yaml=""
+  # python_ver_ena=""
+  # [[ -f $PRJPATH/travis.ini ]] && python_ver_ena=$(cat $PRJPATH/travis.ini|grep "^PYPI_RUN_PYVER"|awk -F= '{print $2}'|grep --color=never -Eo "[0-9.]+"|head -n1)
   if [ $opt_dbgmnt -ne 0 ]; then
     [[ -d $HOME_DEVEL/pypi ]] && export YML_lisa=$HOME_DEVEL/pypi/lisa/lisa/lisa
     (($opt_debug)) && export TRAVIS_PDB="true"
   else
     export YML_lisa=lisa
     export YML_mgrodoo=manage_odoo
   fi
-  export TRAVIS_DEBUG_MODE="${opt_dlvl:-1}"
+  # export TRAVIS_DEBUG_MODE="${opt_dlvl:-1}"
   [[ $TRAVIS_DEBUG_MODE -gt 1 ]] && export VERBOSE_MODE=$TRAVIS_DEBUG_MODE
   [[ $osx_d -ne 0 ]] && export TRAVIS_EMULATE_OSX="true"
   ODOO_TNLBOT="${opt_tnl:-0}"
   if [ $opt_full -ne 0 ]; then
     export SYSTEM_SITE_PACKAGES="${opt_syspkg:-false}"
   else
     export SYSTEM_SITE_PACKAGES="${opt_syspkg:-true}"
@@ -201,15 +199,15 @@
   elif [[ "${line:0:1}" == "\"" && "${line: -1}" == "\"" ]]; then
     line=${line//\\\"/\"}
     lne=$(process_yaml_unquote "${line:1:-1}")
   else
     lne=$(process_yaml_unquote "$line")
   fi
   if [[ $YML_sect == "python" ]]; then
-    [[ -z $python_ver_ena || $lne == $python_ver_ena ]] && python_ver_req="$python_ver_req $lne"
+    python_ver_yaml="$python_ver_yaml $lne"
     lne="#"
   elif [[ $YML_sect == "addons.apt.packages" ]]; then
     YML_packages="$YML_packages $lne"
   elif [[ $YML_sect == "env" ]]; then
     YML_env="$YML_env $lne"
   elif [[ $YML_sect == "env.global" ]]; then
     if [[ ${lne:0:7} == "secure:" ]]; then
@@ -776,57 +774,73 @@
 
 process_yaml() {
   # process_yaml ()
   local sts=$STS_SUCCESS
   local i s p v X x
   local line lne line1 lne1
   load_colors
+  export TRAVIS_DEBUG_MODE="${opt_dlvl:-1}"
   if [[ -n $opt_fyaml ]]; then
-    export TRAVIS_YAML_FILE=$opt_fyaml
+      export TRAVIS_YAML_FILE=$opt_fyaml
   else
-    export TRAVIS_YAML_FILE="$PWD/.travis.yml"
-    [[ ! -f $TRAVIS_YAML_FILE ]] && export TRAVIS_YAML_FILE="$PRJPATH/.travis.yml"
-    if [[ ! -f $TRAVIS_YAML_FILE ]]; then
-      [[ ! -d $HOME/tmp ]] && mkdir $HOME/tmp
-      export TRAVIS_YAML_FILE=$HOME/tmp/travis$$.yml
-      mk_travis_conf=$(find $PYPATH -name make_travis_conf.py|head -n1)
-      python $mk_travis_conf $(find $PYPATH -name template_travis.yml|head -n1) $TRAVIS_YAML_FILE
-    fi
+      export TRAVIS_YAML_FILE="$PWD/.travis.yml"
+      [[ ! -f $TRAVIS_YAML_FILE ]] && export TRAVIS_YAML_FILE="$PRJPATH/.travis.yml"
+      if [[ ! -f $TRAVIS_YAML_FILE ]]; then
+          [[ ! -d $HOME/tmp ]] && mkdir $HOME/tmp
+          export TRAVIS_YAML_FILE=$HOME/tmp/travis$$.yml
+          mk_travis_conf=$(readlink -e $TDIR/make_travis_conf.py)
+          [[ -z $mk_travis_conf ]] && mk_travis_conf=$(find $PYPATH -name make_travis_conf.py|head -n1)
+          export TRAVIS_YAML_ORIG=$(find $PYPATH -name template_travis.yml|head -n1)
+          python $mk_travis_conf "$TRAVIS_YAML_ORIG" "$TRAVIS_YAML_FILE"
+      fi
   fi
   if [[ $action == "chkconfig" ]]; then
-    if [[ ! -f $TRAVIS_YAML_FILE ]]; then
-      do_chkconfig
-      return $STS_SUCCESS
-    fi
+      if [[ ! -f $TRAVIS_YAML_FILE ]]; then
+        do_chkconfig
+        return $STS_SUCCESS
+      fi
   fi
   if [[ ! -f $TRAVIS_YAML_FILE ]]; then
-    echo -e "\e[${PS_HDR3_COLOR}mNo configuration file $TRAVIS_YAML_FILE found!\e[${PS_TXT_COLOR}m"
-    return 127
+      echo -e "\e[${PS_HDR3_COLOR}mNo configuration file $TRAVIS_YAML_FILE found!\e[${PS_TXT_COLOR}m"
+      return 127
   fi
 
   echo -e "\e[0;30;107m$(printf '%-80.80s' ' ')\e[0m"
   wlog "\e[${PS_HDR1_COLOR}m$(printf '%-80.80s' '=== Process YAML file ===')\e[0m"
   export TRAVIS_HOME_BRANCH=$PWD
   process_yaml_file "$TRAVIS_YAML_FILE"
   unset PYTHONPATH
   sts=$STS_SUCCESS
 
   if [[ $sts -eq $STS_SUCCESS ]]; then
     [[ -n $opt_trace && ::matrix =~ $opt_trace ]] && debug_shell "::matrix"
-    [[ -z "$python_ver_req" ]] && python_ver_req=$(python --version 2>&1 | grep --color=never -Eo "[0-9]+\.[0-9]+")
-    [[ -z "$opt_pyv" ]] && opt_pyv=$(get_cfg_value "" "PYTHON_MATRIX")
-    [[ -z "$opt_pyv" ]] && opt_pyv="(2.7|3.5|3.6|3.7|3.8)"
-    opt_pyv="${opt_pyv//,/|}"
-    opt_pyv="${opt_pyv// /|}"
-    [[ $opt_pyv =~ ^\( ]] || opt_pyv="($opt_pyv)"
+    [[ -z "$python_ver_yaml" ]] && python_ver_yaml="2.7 3.5 3.6 3.7 3.8 3.9 3.10 3.11"
+    if [[ -n $opt_pyv ]]; then
+      TRAVIS_PYTHON_MATRIX="${opt_pyv//,/ }"
+      python_ver_yaml="$TRAVIS_PYTHON_MATRIX"
+    elif [[ $PRJNAME == "Odoo" ]]; then
+      v=$(build_odoo_param "MAJVER" $BRANCH)
+      TRAVIS_PYTHON_MATRIX="3.7"
+      [[ $v -le 10 ]] && TRAVIS_PYTHON_MATRIX="2.7"
+      [[ $v -ge 15 ]] && TRAVIS_PYTHON_MATRIX="3.8"
+    else
+      TRAVIS_PYTHON_MATRIX=""
+      for v in "2.7" "3.5" "3.6" "3.7" "3.8" "3.9" "3.10" "3.11"; do
+          grep -q "^ *.Programming Language :: Python :: $v" $PKGPATH/setup.py && TRAVIS_PYTHON_MATRIX="$TRAVIS_PYTHON_MATRIX|$v"
+      done
+      TRAVIS_PYTHON_MATRIX="${TRAVIS_PYTHON_MATRIX:1}"
+    fi
+    TRAVIS_PYTHON_MATRIX="${TRAVIS_PYTHON_MATRIX//,/|}"
+    TRAVIS_PYTHON_MATRIX="${TRAVIS_PYTHON_MATRIX// /|}"
+    [[ $TRAVIS_PYTHON_MATRIX =~ ^\( ]] || TRAVIS_PYTHON_MATRIX="($TRAVIS_PYTHON_MATRIX)"
     python_matrix=""
-    for v in $python_ver_req; do
-      [[ $v =~ $opt_pyv ]] && python_matrix="$python_matrix $v"
+    for v in $python_ver_yaml; do
+      [[ $v =~ $TRAVIS_PYTHON_MATRIX ]] && python_matrix="$python_matrix $v"
     done
-    [[ -z $python_matrix && $opt_pyv =~ ^\([0-9.]+\) ]] && python_matrix=${opt_pyv:1: -1}
+    # [[ -z $python_matrix && $TRAVIS_PYTHON_MATRIX =~ ^\([0-9.]+\) ]] && python_matrix=${TRAVIS_PYTHON_MATRIX:1: -1}
     [[ -n "$python_matrix" ]] || python_matrix="3.8"
 
     for TRAVIS_PYTHON_VERSION in $python_matrix; do
       [[ $sts -eq $STS_SUCCESS ]] || break
       echo -e "\e[0;30;107m$(printf '%-80.80s' ' ')\e[0m"
       wlog "\e[${PS_HDR1_COLOR}m===== [Build python $TRAVIS_PYTHON_VERSION] =====\e[0m"
       set_pybin $TRAVIS_PYTHON_VERSION "PYTHON_VERSION"
@@ -873,20 +887,20 @@
         [[ -n $opt_trace && ::build =~ $opt_trace ]] && debug_shell "::build"
         create_virtual_env
 
         wlog "\e[${PS_HDR2_COLOR}m===== [System informations] =====\e[0m"
         TODAY=$(date "+%Y-%m-%d %H:%M:%S")
         for p in TODAY job-id __version__ TCONF YML_lisa YML_mgrodoo YML_repo\
          BRANCH DIST HOME HOME_BRANCH HOME_DEVEL LOGFILE MQT_TEMPLATE_DB MQT_TEST_DB\
-          ODOO_ROOT PATH PKGNAME PKGPATH PIP PIPVER PRJNAME PRJPATH PGUSER\
-           PYPI_CACHED PYTHON PYTHONPATH REPOSNAME\
-            TRAVIS TRAVIS_BRANCH TRAVIS_BUILD_DIR TRAVIS_EMULATE_OSX\
-             TRAVIS_HOME TRAVIS_HOME_BRANCH TRAVIS_PDB TRAVIS_PYTHON_VERSION\
-              TRAVIS_REPO_SLUG TRAVIS_SAVED_HOME TRAVIS_SAVED_HOME_DEVEL\
-               TRAVIS_YAML_FILE SYSTEM_SITE_PACKAGES; do
+          ODOO_ROOT PATH PKGNAME PKGPATH PIP PIPVER PRJNAME PRJPATH PGUSER PYPI_CACHED\
+           PYTHON PYTHONPATH REPOSNAME TRAVIS TRAVIS_BRANCH TRAVIS_BUILD_DIR\
+             TRAVIS_HOME TRAVIS_HOME_BRANCH TRAVIS_PDB TRAVIS_PYTHON_MATRIX\
+              TRAVIS_PYTHON_VERSION TRAVIS_REPO_SLUG TRAVIS_SAVED_HOME\
+               TRAVIS_SAVED_HOME_DEVEL TRAVIS_YAML_FILE TRAVIS_YAML_ORIG\
+                SYSTEM_SITE_PACKAGES; do
           if [[ $p == "job-id" ]]; then
             X=$$
           elif [[ $p == "DIST" ]]; then
             X=$(xuname -a)
           elif [[ $p == "__version__" ]]; then
             X=$__version__
           else
@@ -947,21 +961,16 @@
 process_yaml_echo() {
   # process_yaml_echo(lev, line)
   local lev=$1
   ((lev++))
   local lm="            "
   lm=${lm:0:$lev}
   local lne="$2"
-  if [ $opt_dprj -ne 0 ]; then
-    echo -n "$lm- "
-    process_yaml_run_cmd "$lne"
-  else
-    local line="- $(process_yaml_quote_xtl $lne)"
-    echo "$lm$line"
-  fi
+  local line="- $(process_yaml_quote_xtl $lne)"
+  echo "$lm$line"
 }
 
 load_colors() {
     export PS_TXT_COLOR=$(get_cfg_value "" "PS_TXT_COLOR")
     export PS_RUN_COLOR=$(get_cfg_value "" "PS_RUN_COLOR")
     export PS_NOP_COLOR=$(get_cfg_value "" "PS_NOP_COLOR")
     export PS_HDR1_COLOR=$(get_cfg_value "" "PS_HDR1_COLOR")
@@ -1003,49 +1012,48 @@
       LOGFILE="$LOGDIR/${UMLI}.log"
     fi
     OLD_LOGFILE=${LOGFILE/.log/_old.log}
     # set +x  #debug
 }
 
 
-OPTOPTS=(h        A           B         C         c        D           E         e       F        f         j        k        L          l        M          m       n            O         P           p        q           r     S            T         V           v           X           Y         y       Z)
-OPTLONG=(help     trace-after debug     no-cache  conf     debug-level no-savenv locale  full     force     ''       keep     lint-level logdir   ''         missing dry-run      org       python-brk  pytest   quiet       ''    syspkg       trace     version     verbose     translation yaml-file pyver   zero)
-OPTDEST=(opt_help opt_tafter  opt_debug opt_cache opt_conf opt_dlvl    opt_keepE opt_loc opt_full opt_force opt_dprj opt_keep opt_llvl   opt_flog opt_dbgmnt opt_mis opt_dry_run  opt_org   opt_pybrk   opt_pyth opt_verbose opt_r  opt_syspkg  opt_trace opt_version opt_verbose opt_tnl     opt_fyaml opt_pyv opt_dbgmnt)
-OPTACTI=('+'      "="         1         0         "="      "="         0         "="     1        1         1        1        "="        "="      1          1       "1>"         "="       "="         1        0           1     "="          "="       "*>"        "+"         "="         "="       "="     1)
-OPTDEFL=(0        ""          0         1         ""       ""          1         ""      0        0         0        0        ""         ""       0          0       0            "local"   ""          0        0           0     ""           ""        ""          -1          ""          ""        ""      0)
-OPTMETA=("help"   "regex"     "version" ""        "file"   "number"    ""        "iso"   ""       ""        "dprj"   ""       "number"   "dir"    ""         ""      "do nothing" "git-org" "file:line" ""       "verbose"   "res" "false|true" "regex"   "version"   "verbose"   "0|1"       "file"    "pyver" "")
+OPTOPTS=(h        A           B         C         D           E         e       F        f         k        j       L          l        M          m       n            O         P           p        Q        q           r     S            T         V           v           X           Y         Z)
+OPTLONG=(help     trace-after debug     no-cache  debug-level no-savenv locale  full     force     keep     pyver   lint-level logdir   ''         missing dry-run      org       python-brk  pytest   config   quiet       ''    syspkg       trace     version     verbose     translation yaml-file zero)
+OPTDEST=(opt_help opt_tafter  opt_debug opt_cache opt_dlvl    opt_keepE opt_loc opt_full opt_force opt_keep opt_pyv opt_llvl   opt_flog opt_dbgmnt opt_mis opt_dry_run  opt_org   opt_pybrk   opt_pyth opt_tcfg opt_verbose opt_r  opt_syspkg  opt_trace opt_version opt_verbose opt_tnl     opt_fyaml opt_dbgmnt)
+OPTACTI=('+'      "="         1         0         "="         0         "="     1        1         1        "="     "="        "="      1          1       "1>"         "="       "="         1        "="      0           1     "="          "="       "*>"        "+"         "="         "="       1)
+OPTDEFL=(0        ""          0         1         ""          1         ""      0        0         0        ""      ""         ""       0          0       0            "local"   ""          0        ""       0           0     ""           ""        ""          -1          ""          ""        0)
+OPTMETA=("help"   "regex"     "version" ""        "number"    ""        "iso"   ""       ""        ""       "pyver" "number"   "dir"    ""         ""      "do nothing" "git-org" "file:line" ""       "file"   "verbose"   "res" "false|true" "regex"   "version"   "verbose"   "0|1"       "file"    "")
 OPTHELP=("this help"
   "travis stops after executed yaml statement"
   "debug mode: do not create log"
   "do not use stored PYPI"
-  "configuration file (def .z0tools.conf)"
   "travis_debug_mode: may be 0,1,2,3,8 or 9 (def yaml dependents)"
   "do not save virtual environment into ~/VME/... if does not exist"
   "use locale"
   "run final travis with full features"
   "force to create stored VME or remove recent log (wep-db)"
-  "deprecated: kept just for compatibility"
   "keep DB and virtual environment before and after tests"
+  "test with specific python versions (comma separated)"
   "lint_check_level: may be minimal,reduced,average,nearby,oca; def value from .travis.yml"
   "log directory (def=$ODOO_ROOT/travis_log)"
   "deprecated: kept just for compatibility"
   "show missing line in report coverage"
   "do nothing (dry-run)"
   "prefer python test over bash test when avaiable"
   "git organization, i.e. oca or zeroincombenze"
   "set python breakpoint at file:linenumber"
+  "configuration file (def .z0tools.conf)"
   "silent mode"
   "run restricted mode (deprecated)"
   "use python system packages (def yaml dependents)"
   "trace stops before executing yaml statement"
   "show version"
   "verbose mode"
   "enable translation test (def yaml dependents)"
   "file yaml to process (def .travis.yml)"
-  "test with specific python versions (comma separated)"
   "use local zero-tools")
 OPTARGS=(action sub sub2)
 
 parseoptargs "$@"
 if [[ "$opt_version" ]]; then
   echo "$__version__"
   exit $STS_SUCCESS
@@ -1088,15 +1096,15 @@
     if [[ ! -f $sub ]]; then
       sub=$TOOLS_PATH/travis.yml
     fi
   fi
   process_yaml_file "$sub"
 
   echo "python:"
-  for v in $python_ver_req; do
+  for v in $python_ver_yaml; do
     echo "  - $v"
   done
   echo ""
   echo "virtualenv:"
   echo " - system_site_packages: $SYSTEM_SITE_PACKAGES"
   echo ""
   echo "addons:"
```

### Comparing `travis_emulator-2.0.3/setup.py` & `travis_emulator-2.0.4/travis_emulator/scripts/setup.info`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='travis_emulator',
-    version='2.0.3',
+    version='2.0.4',
     description='Travis CI emulator for local develop environment',
     long_description="""
 Travis emulator can emulate TravisCi parsing the **.travis.yml** file in local Linux machine.
 You can test your application before pushing code to github.com web site.
 
 Travis emulator can creates all the build declared in **.travis.yml**;
 all the builds are executed in sequential way.
@@ -44,14 +44,15 @@
         'Development Status :: 4 - Beta',
         'License :: OSI Approved :: GNU Affero General Public License v3',
         'Operating System :: POSIX',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
         'Intended Audience :: Developers',
         'Topic :: Software Development',
         'Topic :: Software Development :: Build Tools',
         'Operating System :: OS Independent',
     ],
     keywords='linux travis development',
     url='https://zeroincombenze-tools.readthedocs.io',
```

### Comparing `travis_emulator-2.0.3/travis_emulator.egg-info/SOURCES.txt` & `travis_emulator-2.0.4/travis_emulator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `travis_emulator-2.0.3/README.rst` & `travis_emulator-2.0.4/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 =====================
-travis_emulator 2.0.3
+travis_emulator 2.0.4
 =====================
 
 
 
 |Maturity| |Build Status| |Coverage Status| |license gpl|
 
 
@@ -271,14 +271,27 @@
 
     `lisa install <pkg>`
 
 
 History
 -------
 
+2.0.4 (2023-03-24)
+~~~~~~~~~~~~~~~~~~
+
+* [IMP] Added python 3.9 to test
+* [IMP] Detect python versions from setup.py
+* [IMP] Option switch for python version become -j
+* [IMP} make_travis recognizes verbose option
+
+2.0.3 (2022-12-09)
+~~~~~~~~~~~~~~~~~~
+
+* [FIX] Best python version recognition
+
 2.0.2.2 (2022-11-08)
 ~~~~~~~~~~~~~~~~~~~~
 
 * [IMP] npm management
 
 2.0.2.1 (2022-11-02)
 ~~~~~~~~~~~~~~~~~~~~
@@ -333,21 +346,24 @@
 SHS-AV s.r.l. <https://www.shs-av.com/>
 
 
 Contributors
 ------------
 
 * Antonio M. Vigliotti <info@shs-av.com>
+Contributors
+------------
+
 
 
 |
 
 This module is part of tools project.
 
-Last Update / Ultimo aggiornamento: 2022-12-04
+Last Update / Ultimo aggiornamento: 2023-04-23
 
 .. |Maturity| image:: https://img.shields.io/badge/maturity-Beta-yellow.png
     :target: https://odoo-community.org/page/development-status
     :alt: 
 .. |Build Status| image:: https://travis-ci.org/zeroincombenze/tools.svg?branch=master
     :target: https://travis-ci.com/zeroincombenze/tools
     :alt: github.com
```

