# Comparing `tmp/clodoo-2.0.3.tar.gz` & `tmp/clodoo-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/clodoo-2.0.3.tar", last modified: Fri Jan 13 17:57:26 2023, max compression
+gzip compressed data, was "clodoo-2.0.4.tar", last modified: Sun Apr 23 14:03:09 2023, max compression
```

## Comparing `clodoo-2.0.3.tar` & `clodoo-2.0.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-01-13 17:57:26.000000 clodoo-2.0.3/
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-01-13 17:57:26.000000 clodoo-2.0.3/clodoo/
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      164 2022-12-09 05:08:44.000000 clodoo-2.0.3/clodoo/__main__.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5934 2022-12-11 06:35:48.000000 clodoo-2.0.3/clodoo/update_coa.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    47741 2022-12-11 06:35:48.000000 clodoo-2.0.3/clodoo/clodoocore.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    21634 2022-12-11 06:35:48.000000 clodoo-2.0.3/clodoo/odoo_install_repository
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    29780 2022-12-11 06:35:48.000000 clodoo-2.0.3/clodoo/transodoo.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    23436 2022-12-11 06:35:48.000000 clodoo-2.0.3/clodoo/clodoolib.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-01-13 17:57:26.000000 clodoo-2.0.3/clodoo/scripts/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2616 2022-12-11 06:35:59.000000 clodoo-2.0.3/clodoo/scripts/setup.info
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6510 2022-12-11 06:35:48.000000 clodoo-2.0.3/clodoo/scripts/main.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       43 2022-12-09 05:08:44.000000 clodoo-2.0.3/clodoo/scripts/__init__.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)   232736 2022-12-11 06:35:48.000000 clodoo-2.0.3/clodoo/clodoo.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    23215 2022-12-09 05:08:44.000000 clodoo-2.0.3/clodoo/transodoo.xlsx
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    14545 2022-12-11 06:35:48.000000 clodoo-2.0.3/clodoo/manage_odoo
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    20723 2022-12-11 06:35:48.000000 clodoo-2.0.3/clodoo/manage_db
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     3077 2022-12-11 06:35:48.000000 clodoo-2.0.3/clodoo/check_one2many.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     8612 2022-12-11 06:35:48.000000 clodoo-2.0.3/clodoo/export_db_model.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     8765 2022-12-11 06:35:48.000000 clodoo-2.0.3/clodoo/moduli_da_installare.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      701 2022-12-09 05:08:44.000000 clodoo-2.0.3/clodoo/__init__.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    97606 2022-12-11 06:35:48.000000 clodoo-2.0.3/clodoo/migrate_odoo_db.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    31367 2022-12-11 06:35:48.000000 clodoo-2.0.3/clodoo/odoorc
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       38 2023-01-13 17:57:26.000000 clodoo-2.0.3/setup.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2665 2023-01-08 15:02:02.000000 clodoo-2.0.3/setup.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1623 2023-01-13 17:57:26.000000 clodoo-2.0.3/PKG-INFO
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    17499 2023-01-13 17:57:26.000000 clodoo-2.0.3/README.rst
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-01-13 17:57:26.000000 clodoo-2.0.3/clodoo.egg-info/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        7 2023-01-13 17:57:26.000000 clodoo-2.0.3/clodoo.egg-info/top_level.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-01-13 17:57:26.000000 clodoo-2.0.3/clodoo.egg-info/dependency_links.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2022-12-09 08:50:55.000000 clodoo-2.0.3/clodoo.egg-info/not-zip-safe
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       58 2023-01-13 17:57:26.000000 clodoo-2.0.3/clodoo.egg-info/entry_points.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      654 2023-01-13 17:57:26.000000 clodoo-2.0.3/clodoo.egg-info/SOURCES.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      100 2023-01-13 17:57:26.000000 clodoo-2.0.3/clodoo.egg-info/requires.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1623 2023-01-13 17:57:26.000000 clodoo-2.0.3/clodoo.egg-info/PKG-INFO
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-23 14:03:09.626909 clodoo-2.0.4/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1508 2023-04-23 14:03:09.626909 clodoo-2.0.4/PKG-INFO
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    17642 2023-04-23 14:03:09.000000 clodoo-2.0.4/README.rst
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-23 14:03:09.626909 clodoo-2.0.4/clodoo/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      701 2022-12-09 05:08:44.000000 clodoo-2.0.4/clodoo/__init__.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      164 2022-12-09 05:08:44.000000 clodoo-2.0.4/clodoo/__main__.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     3079 2023-04-12 10:17:46.000000 clodoo-2.0.4/clodoo/check_one2many.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)   232767 2023-04-12 10:17:48.000000 clodoo-2.0.4/clodoo/clodoo.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    47741 2023-03-29 15:04:13.000000 clodoo-2.0.4/clodoo/clodoocore.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    23867 2023-04-12 10:17:47.000000 clodoo-2.0.4/clodoo/clodoolib.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     8614 2023-04-12 10:17:53.000000 clodoo-2.0.4/clodoo/export_db_model.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    20743 2023-04-12 10:17:50.000000 clodoo-2.0.4/clodoo/manage_db
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    14549 2023-04-12 10:17:50.000000 clodoo-2.0.4/clodoo/manage_odoo
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    97608 2023-04-12 10:17:51.000000 clodoo-2.0.4/clodoo/migrate_odoo_db.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     8769 2023-04-12 10:17:47.000000 clodoo-2.0.4/clodoo/moduli_da_installare.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    21638 2023-04-12 10:17:49.000000 clodoo-2.0.4/clodoo/odoo_install_repository
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    32125 2023-04-23 10:03:30.000000 clodoo-2.0.4/clodoo/odoorc
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-23 14:03:09.626909 clodoo-2.0.4/clodoo/scripts/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       43 2022-12-09 05:08:44.000000 clodoo-2.0.4/clodoo/scripts/__init__.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6510 2023-03-29 15:04:13.000000 clodoo-2.0.4/clodoo/scripts/main.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2665 2023-04-23 13:43:15.000000 clodoo-2.0.4/clodoo/scripts/setup.info
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    29780 2023-03-29 15:04:13.000000 clodoo-2.0.4/clodoo/transodoo.py
+-rw-r--r--   0 odoo      (1000) odoo      (1000)    24448 2023-04-02 18:39:37.000000 clodoo-2.0.4/clodoo/transodoo.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5936 2023-04-12 10:17:51.000000 clodoo-2.0.4/clodoo/update_coa.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-23 14:03:09.626909 clodoo-2.0.4/clodoo.egg-info/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1508 2023-04-23 14:03:09.000000 clodoo-2.0.4/clodoo.egg-info/PKG-INFO
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      654 2023-04-23 14:03:09.000000 clodoo-2.0.4/clodoo.egg-info/SOURCES.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-04-23 14:03:09.000000 clodoo-2.0.4/clodoo.egg-info/dependency_links.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       58 2023-04-23 14:03:09.000000 clodoo-2.0.4/clodoo.egg-info/entry_points.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2022-12-09 08:50:55.000000 clodoo-2.0.4/clodoo.egg-info/not-zip-safe
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       96 2023-04-23 14:03:09.000000 clodoo-2.0.4/clodoo.egg-info/requires.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        7 2023-04-23 14:03:09.000000 clodoo-2.0.4/clodoo.egg-info/top_level.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       38 2023-04-23 14:03:09.626909 clodoo-2.0.4/setup.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2665 2023-03-29 15:04:13.000000 clodoo-2.0.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `clodoo-2.0.3/clodoo/update_coa.py` & `clodoo-2.0.4/clodoo/update_coa.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 try:
     from z0lib import z0lib
 except ImportError:
     import z0lib
 # import pdb
 
 
-__version__ = "2.0.3"
+__version__ = "2.0.4"
 
 
 msg_time = time.time()
 
 
 def msg_burst(text):
     global msg_time
@@ -50,15 +50,15 @@
     parser.add_argument("-h")
     parser.add_argument(
         "-c",
         "--config",
         help="configuration command file",
         dest="conf_fn",
         metavar="file",
-        default="./import_partners.conf",
+        default="./import_partners.config",
     )
     parser.add_argument(
         "-d", "--dbname", help="DB name", dest="db_name", metavar="file", default=""
     )
     parser.add_argument("-n")
     parser.add_argument("-q")
     parser.add_argument("-V")
```

### Comparing `clodoo-2.0.3/clodoo/clodoocore.py` & `clodoo-2.0.4/clodoo/clodoocore.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 standard_library.install_aliases()  # noqa: E402
 
 
 STS_FAILED = 1
 STS_SUCCESS = 0
 
 
-__version__ = "2.0.3"
+__version__ = "2.0.4"
 
 
 #############################################################################
 # Low level (driver) functions
 def psql_connect(ctx):
     cr = False
     if postgres_drive and ctx.get("psycopg2", False):
```

### Comparing `clodoo-2.0.3/clodoo/odoo_install_repository` & `clodoo-2.0.4/clodoo/odoo_install_repository`

 * *Files 1% similar despite different names*

```diff
@@ -33,26 +33,26 @@
 . $ODOOLIBDIR
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "ODOOLIBDIR=$ODOOLIBDIR"
 TESTDIR=$(findpkg "" "$TDIR . .." "tests")
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "TESTDIR=$TESTDIR"
 RUNDIR=$(readlink -e $TESTDIR/..)
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "RUNDIR=$RUNDIR"
 
-# DIST_CONF=$(findpkg ".z0tools.conf" "$PYPATH")
-# TCONF="$HOME/.z0tools.conf"
+# DIST_CONF=$(findpkg ".z0tools.config" "$PYPATH")
+# TCONF="$HOME/.z0tools.config"
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
 
 rmdir_if_exists() {
     #rmdir_if_exists (DSTPATH REPOS odoo_vid new_vid)
     local DSTPATH="$1" REPOS="$2" odoo_vid="$3" new_vid="$4"
     local b fn CWD
     local odoo_fver=$(build_odoo_param FULLVER "$odoo_vid")
     if [[ -d $DSTPATH ]]; then
```

### Comparing `clodoo-2.0.3/clodoo/transodoo.py` & `clodoo-2.0.4/clodoo/transodoo.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     from z0lib.z0lib import z0lib
 except ImportError:
     try:
         from z0lib import z0lib
     except ImportError:
         import z0lib
 
-__version__ = "2.0.3"
+__version__ = "2.0.4"
 VERSIONS = [
     "6.1",
     "7.0",
     "8.0",
     "9.0",
     "10.0",
     "11.0",
```

### Comparing `clodoo-2.0.3/clodoo/clodoolib.py` & `clodoo-2.0.4/clodoo/clodoolib.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,27 +35,27 @@
 
 from os0 import os0
 
 standard_library.install_aliases()  # noqa: E402
 
 # Apply for configuration file (True/False)
 APPLY_CONF = True
-# Default configuration file (i.e. myfile.conf or False for default)
-CONF_FN = "./clodoo.conf"
-# Read Odoo configuration file (False or /etc/odoo-server.conf)
+# Default configuration file (i.e. myfile.config or False for default)
+CONF_FN = "./clodoo.config"
+# Read Odoo configuration file (False or /etc/odoo-server.config)
 ODOO_CONF = [
-    "/etc/odoo/odoo-server.conf",
-    "/etc/odoo/odoo.conf",
-    "/etc/odoo-server.conf",
-    "/etc/odoo.conf",
-    "/etc/openerp/openerp-server.conf",
-    "/etc/openerp-server.conf",
-    "/etc/odoo/openerp-server.conf",
+    "/etc/odoo/odoo-server.config",
+    "/etc/odoo/odoo.config",
+    "/etc/odoo-server.config",
+    "/etc/odoo.config",
+    "/etc/openerp/openerp-server.config",
+    "/etc/openerp-server.config",
+    "/etc/odoo/openerp-server.config",
 ]
-# Read Odoo configuration file (False or /etc/openerp-server.conf)
+# Read Odoo configuration file (False or /etc/openerp-server.config)
 OE_CONF = False
 # Warning: if following LX have no values LX=(), if have 1 value LX=(value,)
 # list of string parameters in [options] of config file
 LX_CFG_S = (
     "db_name",
     "db_user",
     "db_password",
@@ -194,15 +194,15 @@
 # switch values of options
 LX_OPT_ARGS = {}
 DEFDCT = {}
 
 msg_time = time.time()
 
 
-__version__ = "2.0.3"
+__version__ = "2.0.4"
 
 
 #############################################################################
 # Message and output
 #
 def init_logger(ctx):
     if ctx["quiet_mode"]:
@@ -539,15 +539,15 @@
 
 
 def fullname_conf(ctx):
     if ctx.get("conf_fn"):
         confs = []
         for confn in ctx["conf_fn"].split(","):
             if not os.path.isfile(confn):
-                for path in (".", "./confs", "./conf", "./code"):
+                for path in (".", "./confs", "./config", "./code"):
                     if os.path.isfile("%s/%s" % (path, confn)):
                         confn = "%s/%s" % (path, confn)
                         break
             confs.append(confn)
         if len(confs) == 1:
             ctx["conf_fn"] = confs[0]
         else:
@@ -570,15 +570,15 @@
                     fnver = build_odoo_param("CONFN", ctx[ver])
                     if os.path.isfile(fnver) and fnver not in ctx["conf_fns"]:
                         ctx["conf_fns"].insert(0, fnver)
                         version_is_set = True
         return ctx, version_is_set
 
     if not ctx.get("conf_fn", None):
-        ctx["conf_fn"] = ctx.get("caller", "clodoo") + ".conf"
+        ctx["conf_fn"] = ctx.get("caller", "clodoo") + ".config"
     ctx = fullname_conf(ctx)
     ctx["conf_fns"] = ctx["conf_fn"].split(",")
     ctx, version_is_set = set_confs(ctx)
     ctx["_conf_obj"] = ConfigParser.RawConfigParser(default_conf(ctx))
     ctx["conf_fns"] = ctx["_conf_obj"].read(ctx["conf_fns"])
     if not ctx["conf_fns"]:
         raise IOError("No configuration file found!")
@@ -811,17 +811,30 @@
     elif v.find(".") >= 0:
         odoo_fver = v
     else:
         odoo_fver = v + ".0"
     return odoo_fver
 
 
+def build_odoo_VER(
+    item, odoo_vid=None, debug=None, suppl=None, git_org=None, multi=None
+):
+    return __version__
+
+
 def build_odoo_param(
     item, odoo_vid=None, debug=None, suppl=None, git_org=None, multi=None
 ):
+    fct = "build_odoo_%s" % item
+    if fct in globals():
+        return globals()[fct](odoo_vid=odoo_vid,
+                              debug=debug,
+                              suppl=suppl,
+                              git_org=git_org,
+                              multi=multi)
     odoorc = os.path.join(os.path.dirname(__file__), "odoorc")
     if multi:
         cmd = 'opt_multi=1 %s %s "%s" "%s" "%s"' % (
             odoorc,
             item,
             odoo_vid,
             suppl or "",
```

### Comparing `clodoo-2.0.3/clodoo/scripts/setup.info` & `clodoo-2.0.4/clodoo/scripts/setup.info`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         "python-plus",
         "unidecode==1.2.0",
         "z0lib",
     ]
 
 setup(
     name="clodoo",
-    version="2.0.3",
+    version="2.0.4",
     description="Do massive operations on Odoo Cloud",
     long_description="""
 Clodoo is a set of tools to manage to manage multiple Odoo installations with many DBs.
 
 With clodoo you can do massive operations on 1 or more Odoo databases based on
 different Odoo versions. Main operation are:
 
@@ -51,14 +51,15 @@
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: GNU Affero General Public License v3",
         "Operating System :: POSIX",
         "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
         "Intended Audience :: Developers",
         "Topic :: Software Development",
     ],
     keywords="odoo",
     url="https://zeroincombenze-tools.readthedocs.io",
     project_urls={
         "Documentation": "https://zeroincombenze-tools.readthedocs.io",
```

### Comparing `clodoo-2.0.3/clodoo/scripts/main.py` & `clodoo-2.0.4/clodoo/scripts/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
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

### Comparing `clodoo-2.0.3/clodoo/clodoo.py` & `clodoo-2.0.4/clodoo/clodoo.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,20 +107,20 @@
 full_model     load all field values, even if not in csv
 header_id      id of header when import header/details files
 lang           language, format lang_COUNTRY, i.e. it_IT (default en_US)
 name2          if present, is merged with name
 name_first     if present with name last, are merged to compose name
 name_last      if present with name first, are merged to compose name
 street2        if present and just numeric, is merged with street
-zeroadm_mail   default user mail from conf file or <def_mail> if -D switch
-zeroadm_login  default admin username from conf file
-oneadm_mail    default user2 mail from conf file or <def_mail> if -D switch
-oneadm_login   default admin2 username from conf file
-botadm_mail    default bot user mail from conf file or <def_mail> if -D switch
-botadm_login   default bot username from conf file
+zeroadm_mail   default user mail from config file or <def_mail> if -D switch
+zeroadm_login  default admin username from config file
+oneadm_mail    default user2 mail from config file or <def_mail> if -D switch
+oneadm_login   default admin2 username from config file
+botadm_mail    default bot user mail from config file or <def_mail> if -D switch
+botadm_login   default bot username from config file
 _today         date.today()
 _current_year  date.today().year
 _last_year'    date.today().year - 1
 TNL_DICT       dictionary with field translation, format csv_name: field_name;
                i.e {'partner_name': 'name'}
                or csv_position: field_name, i.e. {'0': 'name'}
 TNL_VALUE      dictionary with value translation for field;
@@ -234,15 +234,15 @@
     from clodoo.transodoo import read_stored_dict, translate_from_to
 
 # TMP
 from subprocess import PIPE, Popen
 
 standard_library.install_aliases()  # noqa: E402
 
-__version__ = "2.0.3"
+__version__ = "2.0.4"
 
 # Apply for configuration file (True/False)
 APPLY_CONF = True
 STS_FAILED = 1
 STS_SUCCESS = 0
 
 PAY_MOVE_STS_2_DRAFT = ['posted']
@@ -739,15 +739,15 @@
     else:
         action_name = None
     return action_name
 
 
 def do_group_action(ctx, action):
     """Do group actions (recursive)"""
-    if ctx['dbg_mode'] or 'test_unit_mode' not in ctx:
+    if ctx.get('dbg_mode') or 'test_unit_mode' not in ctx:
         msg = "> do_group_action(%s)" % action
         msg_log(ctx, ctx['level'] + 1, msg)
     conf_obj = ctx['_conf_obj']
     sts = STS_SUCCESS
     if conf_obj.has_option(get_real_actname(ctx, action), 'actions'):
         # Local environment for group actions
         lctx = create_local_parms(ctx, action)
@@ -781,15 +781,15 @@
 
 
 def do_single_action(ctx, action):
     """Do single action (recursive)"""
     if isaction(ctx, action):
         if action == '' or action is False or action is None:
             return STS_SUCCESS
-        if ctx['dbg_mode']:
+        if ctx.get('dbg_mode'):
             msg = "> do_single_action(%s)" % action
             msg_log(ctx, ctx['level'] + 1, msg)
         if ctx.get('db_name', '') == 'auto':
             if action not in ("help", "list_actions", "show_params", "new_db"):
                 ctx['db_name'] = get_dbname(ctx, action)
                 lgiuser = do_login(ctx)
                 if not lgiuser:
@@ -1134,15 +1134,15 @@
     print("%s- u. country_id = %d " % (ident, ctx.get('user_country_id', 0)))
     print("%s- u. company_id = %d " % (ident, ctx.get('user_company_id', 0)))
     return STS_SUCCESS
 
 
 def act_unit_test(ctx):
     """This function does nothing, it acts just for unit test"""
-    msg_log(ctx, ctx['level'], globals()[inspect.stack()[0][3]].__doc__)
+    msg_log(ctx, ctx.get('level', 0), globals()[inspect.stack()[0][3]].__doc__)
     return STS_SUCCESS
 
 
 def act_run_unit_tests(ctx):
     """ "Run module unit test (no yet avaiable)"""
     msg_log(ctx, ctx['level'], globals()[inspect.stack()[0][3]].__doc__)
     try:
@@ -5594,28 +5594,28 @@
     if not lgiuser:
         return None
     setup_model = 'zi.dbmgr.db.create.database.wizard'
     values = executeL8(ctx, setup_model, 'default_get', [])
     db_name = values['name']
     setup_id = executeL8(ctx, setup_model, 'create', values)
     executeL8(ctx, setup_model, 'execute', [setup_id], None)
-    fd = open('clodoo_last.conf', 'w')
+    fd = open('clodoo_last.config', 'w')
     fd.write('db_name=%s\n' % db_name)
     fd.close()
     return db_name
 
 
 def get_dbname(ctx, action):
     if ctx['db_name'] == 'auto':
         if action == 'login':
             dbname = ctx['catalog_db']
         elif action == 'new_db':
             dbname = ctx['db_name']
         else:
-            fd = open('clodoo_last.conf', 'r')
+            fd = open('clodoo_last.config', 'r')
             line = fd.readline()
             fd.close()
             dbname = line.split('=')[1].split()[0]
     else:
         dbname = ctx['db_name']
     return dbname
```

### Comparing `clodoo-2.0.3/clodoo/manage_odoo` & `clodoo-2.0.4/clodoo/manage_odoo`

 * *Files 1% similar despite different names*

```diff
@@ -27,26 +27,26 @@
 [[ -z "$Z0LIBDIR" ]] && echo "Library file z0librc not found in <$PYPATH>!" && exit 72
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "Z0LIBDIR=$Z0LIBDIR"
 ODOOLIBDIR=$(findpkg odoorc "$PYPATH" "clodoo")
 [[ -z "$ODOOLIBDIR" ]] && echo "Library file odoorc not found!" && exit 72
 . $ODOOLIBDIR
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "ODOOLIBDIR=$ODOOLIBDIR"
 
-# DIST_CONF=$(findpkg ".z0tools.conf" "$PYPATH")
-# TCONF="$HOME/.z0tools.conf"
+# DIST_CONF=$(findpkg ".z0tools.config" "$PYPATH")
+# TCONF="$HOME/.z0tools.config"
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
 
 
 explore() {
 # explore(odoo_vid excl_list)
     local res=OCB
     local pkgdir=$(build_odoo_param HOME "$1" "" "$opt_org" "$opt_deploy")
     for fn in $pkgdir/*; do
```

### Comparing `clodoo-2.0.3/clodoo/manage_db` & `clodoo-2.0.4/clodoo/manage_db`

 * *Files 1% similar despite different names*

```diff
@@ -32,26 +32,26 @@
 . $ODOOLIBDIR
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "ODOOLIBDIR=$ODOOLIBDIR"
 TESTDIR=$(findpkg "" "$TDIR . .." "tests")
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "TESTDIR=$TESTDIR"
 RUNDIR=$(readlink -e $TESTDIR/..)
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "RUNDIR=$RUNDIR"
 
-# DIST_CONF=$(findpkg ".z0tools.conf" "$PYPATH")
-# TCONF="$HOME/.z0tools.conf"
+# DIST_CONF=$(findpkg ".z0tools.config" "$PYPATH")
+# TCONF="$HOME/.z0tools.config"
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
 
 
 up_oemod() {
 #up_oemod(DB branch)
     local DB=$1
     local oe_version=$2
     local passed_file=./upd_oemod_passed.log
@@ -149,15 +149,15 @@
       CFLOOP="$PHASE_LIST"
     fi
 }
 
 set_opt_conf() {
     local x
     cf=""
-    for x in $opt_conf $opt_conf.conf code/$opt_conf code/$opt_conf.conf; do
+    for x in $opt_conf $opt_conf.config code/$opt_conf code/$opt_conf.config; do
       if [[ -f "$x" ]]; then
         cf=$x
         break
       fi
     done
     if [[ -n "$cf" ]]; then
       opts_cf="-c $cf"
@@ -251,15 +251,15 @@
     if [[ ! -d code ]]; then
       echo "Directory code/ not found!"
       exit 1
     fi
     [[ $action == "update" ]] && set_opt_conf
     declare_cfloop
     for cf in $CFLOOP; do
-      if [ ! -f code/z0_install_$cf.conf ]; then
+      if [ ! -f code/z0_install_$cf.config ]; then
         echo "Configuration file z0_install_$cf.conf not found!"
         exit 1
       fi
     done
     [ -f ~/.openerp_serverrc ] && run_traced "rm -f ~/.openerp_serverrc"
     [ -f .odoorc ] && run_traced "rm -f .odoorc"
     if [ $action == "update" ]; then
@@ -274,15 +274,15 @@
         [ $opt_exit -ne 0 ] && exit 1
         break
       fi
       DBlist=${DBlist//,/ }
     fi
     sts=0
     cf0=""
-    [[ -f ./clodoo.conf ]] && cf0="$(readlink -f ./clodoo.conf),"
+    [[ -f ./clodoo.config ]] && cf0="$(readlink -f ./clodoo.config),"
     for cf in $CFLOOP; do
       # TODO FIX
        opts=
       if [[ $cf == "01" ]]; then
         if [[ $action == "install" ]]; then
           if [[ -n "$opt_db" ]]; then
             optdb="-d $opt_db -lit_IT"
@@ -296,15 +296,15 @@
           sts=1
         fi
       elif [[ $cf == "00" ]]; then
         if [[ $action == "install" ]]; then
           if [[ -n "$opt_db" ]]; then
             db=$opt_db
           else
-            db=$(cat clodoo_last.conf|awk -F= '{print $2}')
+            db=$(cat clodoo_last.config|awk -F= '{print $2}')
           fi
           if [ $opt_del -eq 0 ]; then
             [ $opt_verbose -gt 0 ] && echo "Warning: you must enable dropping DB using -D switch"
             sts=1
           else
             if $(psql -l|grep -q $db); then
               datadir=$(build_odoo_param DDIR $odoo_vid search)
@@ -349,15 +349,15 @@
             s=$?; [ $s -ne 0 -a $sts -eq 0 ] && sts=$s
             [ $sts -ne 0 -a $opt_exit -ne 0 ] && break
           done
         else
           if [ -n "$opt_db" ]; then
             db=$opt_db
           else
-            db=$(cat clodoo_last.conf|awk -F= '{print $2}')
+            db=$(cat clodoo_last.config|awk -F= '{print $2}')
           fi
           run_traced "nice $TDIR/clodoo.py $OPTS -b$odoo_fver -c ${cf0}code/z0_install_$cf.conf -d $db -r$xmlport $opt_with_demo $opts"
           s=$?; [ $s -ne 0 -a $sts -eq 0 ] && sts=$s
         fi
       fi
       [ $sts -ne 0 -a $opt_exit -ne 0 ] && break
     done
@@ -433,15 +433,15 @@
   elif [ "$action" == "rename_phase" ]; then
     if [  -z "$cmdlist" ]; then
       echo "Missed phase rename!"
       echo "$THIS rename_phase old=new"
       sts=1
     else
       IFS== read old new <<< "$cmdlist"
-      confn=$(ls code/*${old}.conf 2>/dev/null|head -n1)
+      confn=$(ls code/*${old}.config 2>/dev/null|head -n1)
       if [ -z "$confn" ]; then
         echo "phase $old not found!"
         sts=1
       else
         new_confn=${confn/$old/$new}
         echo "mv $confn $new_confn"
         mv $confn $new_confn
```

### Comparing `clodoo-2.0.3/clodoo/check_one2many.py` & `clodoo-2.0.4/clodoo/check_one2many.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     try:
         from z0lib import z0lib
     except ImportError:
         import z0lib
 # import pdb
 
 
-__version__ = "2.0.3"
+__version__ = "2.0.4"
 msg_time = time.time()
 
 
 def msg_burst(text):
     global msg_time
     t = time.time() - msg_time
     if t > 3:
@@ -37,15 +37,15 @@
 parser.add_argument("-h")
 parser.add_argument(
     "-c",
     "--config",
     help="configuration command file",
     dest="conf_fn",
     metavar="file",
-    default="./inv2draft_n_restore.conf",
+    default="./inv2draft_n_restore.config",
 )
 parser.add_argument(
     "-d", "--dbname", help="DB name", dest="db_name", metavar="file", default="demo"
 )
 parser.add_argument("-n")
 parser.add_argument("-q")
 parser.add_argument("-V")
```

### Comparing `clodoo-2.0.3/clodoo/export_db_model.py` & `clodoo-2.0.4/clodoo/export_db_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     try:
         from z0lib import z0lib
     except ImportError:
         import z0lib
 # import pdb
 
 
-__version__ = "2.0.3"
+__version__ = "2.0.4"
 
 
 CACHE = {}
 
 
 def get_symbolic_value(ctx, model, name, value):
     name_model = "ir.model.data"
@@ -191,15 +191,15 @@
 )
 parser.add_argument(
     "-c",
     "--config",
     help="configuration command file",
     dest="conf_fn",
     metavar="file",
-    default="./clodoo.conf",
+    default="./clodoo.config",
 )
 parser.add_argument(
     "-d",
     "--dbname",
     help="DB name to connect",
     dest="db_name",
     metavar="file",
```

### Comparing `clodoo-2.0.3/clodoo/moduli_da_installare.py` & `clodoo-2.0.4/clodoo/moduli_da_installare.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     try:
         from z0lib import z0lib
     except ImportError:
         import z0lib
 # import transodoo
 # import pdb
 
-__version__ = "2.0.3"
+__version__ = "2.0.4"
 
 
 VERSIONS = ["vg7", "61", "70", "80", "90", "100", "110", "120"]
 VERSIONS_PLUS = ["vg7", "61", "70", "80", "90", "100", "110", "120", "0"]
 ALIAS = {}
 
 
@@ -99,15 +99,15 @@
 parser.add_argument("-h")
 parser.add_argument(
     "-c",
     "--config",
     help="configuration command file",
     dest="conf_fn",
     metavar="file",
-    default="./clodoo.conf",
+    default="./clodoo.config",
 )
 parser.add_argument(
     "-d",
     "--dbname",
     help="DB name to connect",
     dest="db_name",
     metavar="file",
@@ -179,15 +179,15 @@
     for row in reader:
         if not hdr:
             hdr = True
             continue
         # print row[1]
         add_elem(mod2xtl, "vg7", get_realname(row[1]))
 
-with open("code/z0_install_10.conf", "rb") as f:
+with open("code/z0_install_10.config", "rb") as f:
     lines = f.read().split("\n")
     for line in lines:
         if line.startswith("install_modules_"):
             pv = line.split("=")
             prm = pv[0]
             ver = prm[16:]
             id = ver.split(".")[0] + ver.split(".")[1]
```

### Comparing `clodoo-2.0.3/clodoo/__init__.py` & `clodoo-2.0.4/clodoo/__init__.py`

 * *Files identical despite different names*

### Comparing `clodoo-2.0.3/clodoo/migrate_odoo_db.py` & `clodoo-2.0.4/clodoo/migrate_odoo_db.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 00000290: 2020 2020 6672 6f6d 207a 306c 6962 2069      from z0lib i
 000002a0: 6d70 6f72 7420 7a30 6c69 620a 2020 2020  mport z0lib.    
 000002b0: 6578 6365 7074 2049 6d70 6f72 7445 7272  except ImportErr
 000002c0: 6f72 3a0a 2020 2020 2020 2020 696d 706f  or:.        impo
 000002d0: 7274 207a 306c 6962 0a69 6d70 6f72 7420  rt z0lib.import 
 000002e0: 7472 616e 736f 646f 6f0a 2320 696d 706f  transodoo.# impo
 000002f0: 7274 2070 6462 0a0a 0a5f 5f76 6572 7369  rt pdb...__versi
-00000300: 6f6e 5f5f 203d 2022 322e 302e 3322 0a4d  on__ = "2.0.3".M
+00000300: 6f6e 5f5f 203d 2022 322e 302e 3422 0a4d  on__ = "2.0.4".M
 00000310: 4158 5f44 4545 5020 3d20 3230 0a53 5953  AX_DEEP = 20.SYS
 00000320: 5445 4d5f 4d4f 4445 4c5f 524f 4f54 203d  TEM_MODEL_ROOT =
 00000330: 205b 0a20 2020 2027 6261 7365 2e63 6f6e   [.    'base.con
 00000340: 6669 672e 272c 0a20 2020 2027 6261 7365  fig.',.    'base
 00000350: 5f69 6d70 6f72 742e 272c 0a20 2020 2027  _import.',.    '
 00000360: 6261 7365 2e6c 616e 6775 6167 652e 272c  base.language.',
 00000370: 0a20 2020 2027 6261 7365 2e6d 6f64 756c  .    'base.modul
@@ -4163,1939 +4163,1939 @@
 00010420: 7072 6570 6172 655f 636f 6e66 6967 5f66  prepare_config_f
 00010430: 696c 6528 6374 782c 2073 7263 5f63 6f6e  ile(ctx, src_con
 00010440: 6669 672c 206f 755f 7665 725f 7061 7468  fig, ou_ver_path
 00010450: 3d4e 6f6e 652c 2070 6174 6873 3d4e 6f6e  =None, paths=Non
 00010460: 6529 3a0a 2020 2020 6966 206f 755f 7665  e):.    if ou_ve
 00010470: 725f 7061 7468 3a0a 2020 2020 2020 2020  r_path:.        
 00010480: 7372 635f 6c63 6f6e 6620 3d20 276f 7065  src_lconf = 'ope
-00010490: 6e75 7067 7261 6465 2e63 6f6e 6627 0a20  nupgrade.conf'. 
-000104a0: 2020 2020 2020 2066 756c 6c5f 6c63 6f6e         full_lcon
-000104b0: 6620 3d20 6f73 2e70 6174 682e 6a6f 696e  f = os.path.join
-000104c0: 286f 755f 7665 725f 7061 7468 2c20 7372  (ou_ver_path, sr
-000104d0: 635f 6c63 6f6e 6629 0a20 2020 2065 6c73  c_lconf).    els
-000104e0: 653a 0a20 2020 2020 2020 2073 7263 5f6c  e:.        src_l
-000104f0: 636f 6e66 203d 2063 6c6f 646f 6f2e 6275  conf = clodoo.bu
-00010500: 696c 645f 6f64 6f6f 5f70 6172 616d 280a  ild_odoo_param(.
-00010510: 2020 2020 2020 2020 2020 2020 274c 434f              'LCO
-00010520: 4e46 4e27 2c20 6f64 6f6f 5f76 6964 3d63  NFN', odoo_vid=c
-00010530: 7478 5b27 7372 635f 7669 6427 5d2c 206d  tx['src_vid'], m
-00010540: 756c 7469 3d54 7275 6529 0a20 2020 2020  ulti=True).     
-00010550: 2020 2066 756c 6c5f 6c63 6f6e 6620 3d20     full_lconf = 
-00010560: 6f73 2e70 6174 682e 6a6f 696e 286f 732e  os.path.join(os.
-00010570: 7061 7468 2e65 7870 616e 6475 7365 7228  path.expanduser(
-00010580: 277e 2729 2c0a 2020 2020 2020 2020 2020  '~'),.          
+00010490: 6e75 7067 7261 6465 2e63 6f6e 6669 6727  nupgrade.config'
+000104a0: 0a20 2020 2020 2020 2066 756c 6c5f 6c63  .        full_lc
+000104b0: 6f6e 6620 3d20 6f73 2e70 6174 682e 6a6f  onf = os.path.jo
+000104c0: 696e 286f 755f 7665 725f 7061 7468 2c20  in(ou_ver_path, 
+000104d0: 7372 635f 6c63 6f6e 6629 0a20 2020 2065  src_lconf).    e
+000104e0: 6c73 653a 0a20 2020 2020 2020 2073 7263  lse:.        src
+000104f0: 5f6c 636f 6e66 203d 2063 6c6f 646f 6f2e  _lconf = clodoo.
+00010500: 6275 696c 645f 6f64 6f6f 5f70 6172 616d  build_odoo_param
+00010510: 280a 2020 2020 2020 2020 2020 2020 274c  (.            'L
+00010520: 434f 4e46 4e27 2c20 6f64 6f6f 5f76 6964  CONFN', odoo_vid
+00010530: 3d63 7478 5b27 7372 635f 7669 6427 5d2c  =ctx['src_vid'],
+00010540: 206d 756c 7469 3d54 7275 6529 0a20 2020   multi=True).   
+00010550: 2020 2020 2066 756c 6c5f 6c63 6f6e 6620       full_lconf 
+00010560: 3d20 6f73 2e70 6174 682e 6a6f 696e 286f  = os.path.join(o
+00010570: 732e 7061 7468 2e65 7870 616e 6475 7365  s.path.expanduse
+00010580: 7228 277e 2729 2c0a 2020 2020 2020 2020  r('~'),.        
 00010590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000105a0: 2020 2020 2020 2020 7372 635f 6c63 6f6e          src_lcon
-000105b0: 6629 0a20 2020 2020 2020 2066 6f72 2066  f).        for f
-000105c0: 6e20 696e 2028 272e 6f70 656e 6572 705f  n in ('.openerp_
-000105d0: 7365 7276 6572 7263 272c 2027 2e6f 646f  serverrc', '.odo
-000105e0: 6f72 6327 293a 0a20 2020 2020 2020 2020  orc'):.         
-000105f0: 2020 2074 6d70 5f6c 636f 6e66 203d 206f     tmp_lconf = o
-00010600: 732e 7061 7468 2e6a 6f69 6e28 6f73 2e70  s.path.join(os.p
-00010610: 6174 682e 6578 7061 6e64 7573 6572 2827  ath.expanduser('
-00010620: 7e27 292c 2066 6e29 0a20 2020 2020 2020  ~'), fn).       
-00010630: 2020 2020 2069 6620 6f73 2e70 6174 682e       if os.path.
-00010640: 6973 6669 6c65 2874 6d70 5f6c 636f 6e66  isfile(tmp_lconf
-00010650: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00010660: 2020 206f 732e 7265 6d6f 7665 2874 6d70     os.remove(tmp
-00010670: 5f6c 636f 6e66 290a 2020 2020 6966 2070  _lconf).    if p
-00010680: 6174 6873 3a0a 2020 2020 2020 2020 7372  aths:.        sr
-00010690: 635f 636f 6e66 6967 2e73 6574 2827 6f70  c_config.set('op
-000106a0: 7469 6f6e 7327 2c20 2761 6464 6f6e 735f  tions', 'addons_
-000106b0: 7061 7468 272c 2027 2c27 2e6a 6f69 6e28  path', ','.join(
-000106c0: 7061 7468 7329 290a 2020 2020 6966 206f  paths)).    if o
-000106d0: 755f 7665 725f 7061 7468 3a0a 2020 2020  u_ver_path:.    
-000106e0: 2020 2020 7372 635f 636f 6e66 6967 2e73      src_config.s
-000106f0: 6574 2827 6f70 7469 6f6e 7327 2c20 2772  et('options', 'r
-00010700: 6f6f 745f 7061 7468 272c 206f 755f 7665  oot_path', ou_ve
-00010710: 725f 7061 7468 290a 2020 2020 7372 635f  r_path).    src_
-00010720: 636f 6e66 6967 2e77 7269 7465 286f 7065  config.write(ope
-00010730: 6e28 6675 6c6c 5f6c 636f 6e66 2c20 2777  n(full_lconf, 'w
-00010740: 2b27 2929 0a20 2020 2073 7263 5f63 6f6e  +')).    src_con
-00010750: 6669 672e 7265 6164 2866 756c 6c5f 6c63  fig.read(full_lc
-00010760: 6f6e 6629 0a20 2020 2072 6574 7572 6e20  onf).    return 
-00010770: 6675 6c6c 5f6c 636f 6e66 0a0a 0a64 6566  full_lconf...def
-00010780: 2068 6172 645f 636c 6561 6e5f 6d6f 6475   hard_clean_modu
-00010790: 6c65 2863 7478 2c20 6d6f 6475 6c65 5f6e  le(ctx, module_n
-000107a0: 616d 6529 3a0a 2020 2020 6465 6620 6472  ame):.    def dr
-000107b0: 6f70 5f64 6174 615f 7461 626c 6528 6374  op_data_table(ct
-000107c0: 782c 206d 6f64 656c 2c20 6d6f 6475 6c65  x, model, module
-000107d0: 5f6e 616d 652c 2063 6f6c 6e3d 4e6f 6e65  _name, coln=None
-000107e0: 2c20 6964 3d4e 6f6e 6529 3a0a 2020 2020  , id=None):.    
-000107f0: 2020 2020 636f 6c6e 203d 2063 6f6c 6e20      coln = coln 
-00010800: 6f72 2027 6d6f 6475 6c65 270a 2020 2020  or 'module'.    
-00010810: 2020 2020 6966 2069 643a 0a20 2020 2020      if id:.     
-00010820: 2020 2020 2020 2071 7565 7279 203d 2022         query = "
-00010830: 6465 6c65 7465 2066 726f 6d20 2573 2077  delete from %s w
-00010840: 6865 7265 2025 733d 2564 2220 2520 286d  here %s=%d" % (m
-00010850: 6f64 656c 2c20 636f 6c6e 2c20 6964 290a  odel, coln, id).
-00010860: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00010870: 2020 2020 2020 2020 2020 7175 6572 7920            query 
-00010880: 3d20 2264 656c 6574 6520 6672 6f6d 2025  = "delete from %
-00010890: 7320 7768 6572 6520 2573 3d27 2573 2722  s where %s='%s'"
-000108a0: 2025 2028 6d6f 6465 6c2c 2063 6f6c 6e2c   % (model, coln,
-000108b0: 206d 6f64 756c 655f 6e61 6d65 290a 2020   module_name).  
-000108c0: 2020 2020 2020 7265 6373 203d 2065 7865        recs = exe
-000108d0: 635f 7371 6c28 6374 782c 2071 7565 7279  c_sql(ctx, query
-000108e0: 290a 0a20 2020 2071 7565 7279 203d 2022  )..    query = "
-000108f0: 7365 6c65 6374 2069 642c 6e61 6d65 2c73  select id,name,s
-00010900: 7461 7465 2066 726f 6d20 6972 5f6d 6f64  tate from ir_mod
-00010910: 756c 655f 6d6f 6475 6c65 2077 6865 7265  ule_module where
-00010920: 206e 616d 653d 2725 7327 2220 2520 5c0a   name='%s'" % \.
-00010930: 2020 2020 2020 2020 2020 2020 6d6f 6475              modu
-00010940: 6c65 5f6e 616d 650a 2020 2020 7265 6373  le_name.    recs
-00010950: 203d 2065 7865 635f 7371 6c28 6374 782c   = exec_sql(ctx,
-00010960: 2071 7565 7279 2c20 7265 7370 6f6e 7365   query, response
-00010970: 3d54 7275 6529 0a20 2020 2069 6620 6e6f  =True).    if no
-00010980: 7420 6c65 6e28 7265 6373 293a 0a20 2020  t len(recs):.   
-00010990: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
-000109a0: 7374 6174 6520 3d20 7265 6373 5b30 5d5b  state = recs[0][
-000109b0: 325d 0a20 2020 2069 6420 3d20 7265 6373  2].    id = recs
-000109c0: 5b30 5d5b 305d 0a20 2020 2069 6620 7374  [0][0].    if st
-000109d0: 6174 6520 3d3d 2027 696e 7374 616c 6c65  ate == 'installe
-000109e0: 6427 3a0a 2020 2020 2020 2020 7265 7475  d':.        retu
-000109f0: 726e 0a20 2020 2064 726f 705f 6461 7461  rn.    drop_data
-00010a00: 5f74 6162 6c65 2863 7478 2c20 2769 725f  _table(ctx, 'ir_
-00010a10: 6d6f 6465 6c5f 6461 7461 272c 206d 6f64  model_data', mod
-00010a20: 756c 655f 6e61 6d65 290a 2020 2020 6472  ule_name).    dr
-00010a30: 6f70 5f64 6174 615f 7461 626c 6528 6374  op_data_table(ct
-00010a40: 782c 2027 6972 5f6d 6f64 756c 655f 6d6f  x, 'ir_module_mo
-00010a50: 6475 6c65 5f64 6570 656e 6465 6e63 7927  dule_dependency'
-00010a60: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00010a70: 2020 2020 2020 6d6f 6475 6c65 5f6e 616d        module_nam
-00010a80: 652c 2063 6f6c 6e3d 276d 6f64 756c 655f  e, coln='module_
-00010a90: 6964 272c 2069 643d 6964 290a 2020 2020  id', id=id).    
-00010aa0: 6472 6f70 5f64 6174 615f 7461 626c 6528  drop_data_table(
-00010ab0: 6374 782c 2027 6972 5f74 7261 6e73 6c61  ctx, 'ir_transla
-00010ac0: 7469 6f6e 272c 206d 6f64 756c 655f 6e61  tion', module_na
-00010ad0: 6d65 290a 2020 2020 7365 745f 756e 696e  me).    set_unin
-00010ae0: 7374 616c 6c65 645f 6279 5f73 716c 2863  stalled_by_sql(c
-00010af0: 7478 2c20 5b5f 6228 6d6f 6475 6c65 5f6e  tx, [_b(module_n
-00010b00: 616d 6529 5d29 0a0a 0a64 6566 2066 6978  ame)])...def fix
-00010b10: 5f62 7567 5f70 7265 2873 7263 5f63 7478  _bug_pre(src_ctx
-00010b20: 2c20 7467 745f 6374 782c 2073 7263 5f66  , tgt_ctx, src_f
-00010b30: 756c 6c5f 6c63 6f6e 662c 2073 7263 5f70  ull_lconf, src_p
-00010b40: 6174 6873 293a 0a20 2020 2073 6176 6564  aths):.    saved
-00010b50: 5f64 622c 2073 7263 5f63 7478 5b27 6462  _db, src_ctx['db
-00010b60: 5f6e 616d 6527 5d20 3d20 7372 635f 6374  _name'] = src_ct
-00010b70: 785b 2764 625f 6e61 6d65 275d 2c20 7467  x['db_name'], tg
-00010b80: 745f 6374 785b 2764 625f 6e61 6d65 275d  t_ctx['db_name']
-00010b90: 0a20 2020 2069 6620 2873 7263 5f63 7478  .    if (src_ctx
-00010ba0: 5b27 7372 635f 6f64 6f6f 5f66 7665 7227  ['src_odoo_fver'
-00010bb0: 5d20 3d3d 2027 372e 3027 2061 6e64 0a20  ] == '7.0' and. 
-00010bc0: 2020 2020 2020 2020 2020 2074 6774 5f63             tgt_c
-00010bd0: 7478 5b27 7467 745f 6f64 6f6f 5f66 7665  tx['tgt_odoo_fve
-00010be0: 7227 5d20 3d3d 2027 382e 3027 293a 0a20  r'] == '8.0'):. 
-00010bf0: 2020 2020 2020 2071 7565 7279 203d 2027         query = '
-00010c00: 2727 7570 6461 7465 2069 725f 7569 5f76  ''update ir_ui_v
-00010c10: 6965 770a 2020 2020 2020 2020 2020 2020  iew.            
-00010c20: 2020 2020 7365 7420 6172 6368 3d52 4547      set arch=REG
-00010c30: 4558 505f 5245 504c 4143 4528 6172 6368  EXP_REPLACE(arch
-00010c40: 2c20 273c 6669 656c 6420 6e61 6d65 3d22  , '<field name="
-00010c50: 6d65 6e75 5f69 6422 2e2a 2f3e 272c 2027  menu_id".*/>', '
-00010c60: 2729 0a20 2020 2020 2020 2020 2020 2020  ').             
-00010c70: 2020 2077 6865 7265 206d 6f64 656c 3d27     where model='
-00010c80: 7265 732e 7573 6572 7327 2061 6e64 0a20  res.users' and. 
-00010c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ca0: 2020 2020 2061 7263 6820 6c69 6b65 2027       arch like '
-00010cb0: 253c 6669 656c 6420 6e61 6d65 3d5f 6d65  %<field name=_me
-00010cc0: 6e75 5f69 645f 2527 3b27 2727 0a20 2020  nu_id_%';'''.   
-00010cd0: 2020 2020 2065 7865 635f 7371 6c28 7372       exec_sql(sr
-00010ce0: 635f 6374 782c 2071 7565 7279 290a 2020  c_ctx, query).  
-00010cf0: 2020 656c 6966 2028 7372 635f 6374 785b    elif (src_ctx[
-00010d00: 2773 7263 5f6f 646f 6f5f 6676 6572 275d  'src_odoo_fver']
-00010d10: 203d 3d20 2738 2e30 2720 616e 640a 2020   == '8.0' and.  
-00010d20: 2020 2020 2020 2020 2020 7467 745f 6374            tgt_ct
-00010d30: 785b 2774 6774 5f6f 646f 6f5f 6676 6572  x['tgt_odoo_fver
-00010d40: 275d 203d 3d20 2739 2e30 2729 3a0a 2020  '] == '9.0'):.  
-00010d50: 2020 2020 2020 6966 2027 6163 636f 756e        if 'accoun
-00010d60: 745f 7061 796d 656e 7427 2069 6e20 7372  t_payment' in sr
-00010d70: 635f 6374 785b 2773 7263 5f6d 6f64 756c  c_ctx['src_modul
-00010d80: 655f 6c69 7374 275d 3a0a 2020 2020 2020  e_list']:.      
-00010d90: 2020 2020 2020 7374 7320 3d20 636c 6f64        sts = clod
-00010da0: 6f6f 2e61 6374 5f69 6e73 7461 6c6c 5f6d  oo.act_install_m
-00010db0: 6f64 756c 6573 280a 2020 2020 2020 2020  odules(.        
-00010dc0: 2020 2020 2020 2020 7372 635f 6374 782c          src_ctx,
-00010dd0: 206d 6f64 756c 655f 6c69 7374 3d5b 2761   module_list=['a
-00010de0: 6363 6f75 6e74 5f62 616e 6b69 6e67 5f70  ccount_banking_p
-00010df0: 6179 6d65 6e74 5f65 7870 6f72 7427 5d29  ayment_export'])
-00010e00: 0a20 2020 2073 7263 5f63 7478 5b27 6462  .    src_ctx['db
-00010e10: 5f6e 616d 6527 5d20 3d20 7361 7665 645f  _name'] = saved_
-00010e20: 6462 0a0a 0a64 6566 2066 6978 5f62 7567  db...def fix_bug
-00010e30: 5f70 6f73 7428 7372 635f 6374 782c 2074  _post(src_ctx, t
-00010e40: 6774 5f63 7478 2c20 7467 745f 6675 6c6c  gt_ctx, tgt_full
-00010e50: 5f6c 636f 6e66 2c20 7467 745f 7061 7468  _lconf, tgt_path
-00010e60: 7329 3a0a 2020 2020 6966 2028 7372 635f  s):.    if (src_
-00010e70: 6374 785b 2773 7263 5f6f 646f 6f5f 6676  ctx['src_odoo_fv
-00010e80: 6572 275d 203d 3d20 2737 2e30 2720 616e  er'] == '7.0' an
-00010e90: 640a 2020 2020 2020 2020 2020 2020 7467  d.            tg
-00010ea0: 745f 6374 785b 2774 6774 5f6f 646f 6f5f  t_ctx['tgt_odoo_
-00010eb0: 6676 6572 275d 203d 3d20 2738 2e30 2729  fver'] == '8.0')
-00010ec0: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
-00010ed0: 0a64 6566 206d 6967 7261 7465 5f6f 646f  .def migrate_odo
-00010ee0: 6f28 7372 635f 6374 782c 2074 6774 5f63  o(src_ctx, tgt_c
-00010ef0: 7478 2c20 7372 635f 636f 6e66 6967 2c20  tx, src_config, 
-00010f00: 7467 745f 636f 6e66 6967 2c20 7068 6173  tgt_config, phas
-00010f10: 653d 4e6f 6e65 293a 0a0a 2020 2020 6465  e=None):..    de
-00010f20: 6620 6765 745f 7772 6f6e 675f 6d6f 6475  f get_wrong_modu
-00010f30: 6c65 7328 6374 782c 2062 6164 5f6d 6f64  les(ctx, bad_mod
-00010f40: 756c 655f 6c69 7374 3d4e 6f6e 6529 3a0a  ule_list=None):.
-00010f50: 2020 2020 2020 2020 6966 2073 7263 5f63          if src_c
-00010f60: 7478 5b27 6472 795f 7275 6e27 5d3a 0a20  tx['dry_run']:. 
-00010f70: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00010f80: 6e20 5b5d 0a20 2020 2020 2020 2069 6620  n [].        if 
-00010f90: 6261 645f 6d6f 6475 6c65 5f6c 6973 743a  bad_module_list:
-00010fa0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00010fb0: 6c65 6e28 6261 645f 6d6f 6475 6c65 5f6c  len(bad_module_l
-00010fc0: 6973 7429 203d 3d20 313a 0a20 2020 2020  ist) == 1:.     
-00010fd0: 2020 2020 2020 2020 2020 2071 7565 7279             query
-00010fe0: 203d 2027 2727 7365 6c65 6374 2069 642c   = '''select id,
-00010ff0: 6e61 6d65 2c73 7461 7465 2066 726f 6d20  name,state from 
-00011000: 6972 5f6d 6f64 756c 655f 6d6f 6475 6c65  ir_module_module
-00011010: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011020: 2020 2020 2020 2020 2020 2020 7768 6572              wher
-00011030: 6520 7374 6174 6520 6e6f 7420 696e 0a20  e state not in. 
-00011040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011050: 2020 2020 2020 2020 2020 2827 696e 7374            ('inst
-00011060: 616c 6c65 6427 2c20 2775 6e69 6e73 7461  alled', 'uninsta
-00011070: 6c6c 6564 272c 2027 756e 696e 7374 616c  lled', 'uninstal
-00011080: 6c61 626c 6527 2920 616e 640a 2020 2020  lable') and.    
+000105a0: 2020 2020 2020 2020 2020 7372 635f 6c63            src_lc
+000105b0: 6f6e 6629 0a20 2020 2020 2020 2066 6f72  onf).        for
+000105c0: 2066 6e20 696e 2028 272e 6f70 656e 6572   fn in ('.opener
+000105d0: 705f 7365 7276 6572 7263 272c 2027 2e6f  p_serverrc', '.o
+000105e0: 646f 6f72 6327 293a 0a20 2020 2020 2020  doorc'):.       
+000105f0: 2020 2020 2074 6d70 5f6c 636f 6e66 203d       tmp_lconf =
+00010600: 206f 732e 7061 7468 2e6a 6f69 6e28 6f73   os.path.join(os
+00010610: 2e70 6174 682e 6578 7061 6e64 7573 6572  .path.expanduser
+00010620: 2827 7e27 292c 2066 6e29 0a20 2020 2020  ('~'), fn).     
+00010630: 2020 2020 2020 2069 6620 6f73 2e70 6174         if os.pat
+00010640: 682e 6973 6669 6c65 2874 6d70 5f6c 636f  h.isfile(tmp_lco
+00010650: 6e66 293a 0a20 2020 2020 2020 2020 2020  nf):.           
+00010660: 2020 2020 206f 732e 7265 6d6f 7665 2874       os.remove(t
+00010670: 6d70 5f6c 636f 6e66 290a 2020 2020 6966  mp_lconf).    if
+00010680: 2070 6174 6873 3a0a 2020 2020 2020 2020   paths:.        
+00010690: 7372 635f 636f 6e66 6967 2e73 6574 2827  src_config.set('
+000106a0: 6f70 7469 6f6e 7327 2c20 2761 6464 6f6e  options', 'addon
+000106b0: 735f 7061 7468 272c 2027 2c27 2e6a 6f69  s_path', ','.joi
+000106c0: 6e28 7061 7468 7329 290a 2020 2020 6966  n(paths)).    if
+000106d0: 206f 755f 7665 725f 7061 7468 3a0a 2020   ou_ver_path:.  
+000106e0: 2020 2020 2020 7372 635f 636f 6e66 6967        src_config
+000106f0: 2e73 6574 2827 6f70 7469 6f6e 7327 2c20  .set('options', 
+00010700: 2772 6f6f 745f 7061 7468 272c 206f 755f  'root_path', ou_
+00010710: 7665 725f 7061 7468 290a 2020 2020 7372  ver_path).    sr
+00010720: 635f 636f 6e66 6967 2e77 7269 7465 286f  c_config.write(o
+00010730: 7065 6e28 6675 6c6c 5f6c 636f 6e66 2c20  pen(full_lconf, 
+00010740: 2777 2b27 2929 0a20 2020 2073 7263 5f63  'w+')).    src_c
+00010750: 6f6e 6669 672e 7265 6164 2866 756c 6c5f  onfig.read(full_
+00010760: 6c63 6f6e 6629 0a20 2020 2072 6574 7572  lconf).    retur
+00010770: 6e20 6675 6c6c 5f6c 636f 6e66 0a0a 0a64  n full_lconf...d
+00010780: 6566 2068 6172 645f 636c 6561 6e5f 6d6f  ef hard_clean_mo
+00010790: 6475 6c65 2863 7478 2c20 6d6f 6475 6c65  dule(ctx, module
+000107a0: 5f6e 616d 6529 3a0a 2020 2020 6465 6620  _name):.    def 
+000107b0: 6472 6f70 5f64 6174 615f 7461 626c 6528  drop_data_table(
+000107c0: 6374 782c 206d 6f64 656c 2c20 6d6f 6475  ctx, model, modu
+000107d0: 6c65 5f6e 616d 652c 2063 6f6c 6e3d 4e6f  le_name, coln=No
+000107e0: 6e65 2c20 6964 3d4e 6f6e 6529 3a0a 2020  ne, id=None):.  
+000107f0: 2020 2020 2020 636f 6c6e 203d 2063 6f6c        coln = col
+00010800: 6e20 6f72 2027 6d6f 6475 6c65 270a 2020  n or 'module'.  
+00010810: 2020 2020 2020 6966 2069 643a 0a20 2020        if id:.   
+00010820: 2020 2020 2020 2020 2071 7565 7279 203d           query =
+00010830: 2022 6465 6c65 7465 2066 726f 6d20 2573   "delete from %s
+00010840: 2077 6865 7265 2025 733d 2564 2220 2520   where %s=%d" % 
+00010850: 286d 6f64 656c 2c20 636f 6c6e 2c20 6964  (model, coln, id
+00010860: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+00010870: 2020 2020 2020 2020 2020 2020 7175 6572              quer
+00010880: 7920 3d20 2264 656c 6574 6520 6672 6f6d  y = "delete from
+00010890: 2025 7320 7768 6572 6520 2573 3d27 2573   %s where %s='%s
+000108a0: 2722 2025 2028 6d6f 6465 6c2c 2063 6f6c  '" % (model, col
+000108b0: 6e2c 206d 6f64 756c 655f 6e61 6d65 290a  n, module_name).
+000108c0: 2020 2020 2020 2020 7265 6373 203d 2065          recs = e
+000108d0: 7865 635f 7371 6c28 6374 782c 2071 7565  xec_sql(ctx, que
+000108e0: 7279 290a 0a20 2020 2071 7565 7279 203d  ry)..    query =
+000108f0: 2022 7365 6c65 6374 2069 642c 6e61 6d65   "select id,name
+00010900: 2c73 7461 7465 2066 726f 6d20 6972 5f6d  ,state from ir_m
+00010910: 6f64 756c 655f 6d6f 6475 6c65 2077 6865  odule_module whe
+00010920: 7265 206e 616d 653d 2725 7327 2220 2520  re name='%s'" % 
+00010930: 5c0a 2020 2020 2020 2020 2020 2020 6d6f  \.            mo
+00010940: 6475 6c65 5f6e 616d 650a 2020 2020 7265  dule_name.    re
+00010950: 6373 203d 2065 7865 635f 7371 6c28 6374  cs = exec_sql(ct
+00010960: 782c 2071 7565 7279 2c20 7265 7370 6f6e  x, query, respon
+00010970: 7365 3d54 7275 6529 0a20 2020 2069 6620  se=True).    if 
+00010980: 6e6f 7420 6c65 6e28 7265 6373 293a 0a20  not len(recs):. 
+00010990: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
+000109a0: 2020 7374 6174 6520 3d20 7265 6373 5b30    state = recs[0
+000109b0: 5d5b 325d 0a20 2020 2069 6420 3d20 7265  ][2].    id = re
+000109c0: 6373 5b30 5d5b 305d 0a20 2020 2069 6620  cs[0][0].    if 
+000109d0: 7374 6174 6520 3d3d 2027 696e 7374 616c  state == 'instal
+000109e0: 6c65 6427 3a0a 2020 2020 2020 2020 7265  led':.        re
+000109f0: 7475 726e 0a20 2020 2064 726f 705f 6461  turn.    drop_da
+00010a00: 7461 5f74 6162 6c65 2863 7478 2c20 2769  ta_table(ctx, 'i
+00010a10: 725f 6d6f 6465 6c5f 6461 7461 272c 206d  r_model_data', m
+00010a20: 6f64 756c 655f 6e61 6d65 290a 2020 2020  odule_name).    
+00010a30: 6472 6f70 5f64 6174 615f 7461 626c 6528  drop_data_table(
+00010a40: 6374 782c 2027 6972 5f6d 6f64 756c 655f  ctx, 'ir_module_
+00010a50: 6d6f 6475 6c65 5f64 6570 656e 6465 6e63  module_dependenc
+00010a60: 7927 2c0a 2020 2020 2020 2020 2020 2020  y',.            
+00010a70: 2020 2020 2020 2020 6d6f 6475 6c65 5f6e          module_n
+00010a80: 616d 652c 2063 6f6c 6e3d 276d 6f64 756c  ame, coln='modul
+00010a90: 655f 6964 272c 2069 643d 6964 290a 2020  e_id', id=id).  
+00010aa0: 2020 6472 6f70 5f64 6174 615f 7461 626c    drop_data_tabl
+00010ab0: 6528 6374 782c 2027 6972 5f74 7261 6e73  e(ctx, 'ir_trans
+00010ac0: 6c61 7469 6f6e 272c 206d 6f64 756c 655f  lation', module_
+00010ad0: 6e61 6d65 290a 2020 2020 7365 745f 756e  name).    set_un
+00010ae0: 696e 7374 616c 6c65 645f 6279 5f73 716c  installed_by_sql
+00010af0: 2863 7478 2c20 5b5f 6228 6d6f 6475 6c65  (ctx, [_b(module
+00010b00: 5f6e 616d 6529 5d29 0a0a 0a64 6566 2066  _name)])...def f
+00010b10: 6978 5f62 7567 5f70 7265 2873 7263 5f63  ix_bug_pre(src_c
+00010b20: 7478 2c20 7467 745f 6374 782c 2073 7263  tx, tgt_ctx, src
+00010b30: 5f66 756c 6c5f 6c63 6f6e 662c 2073 7263  _full_lconf, src
+00010b40: 5f70 6174 6873 293a 0a20 2020 2073 6176  _paths):.    sav
+00010b50: 6564 5f64 622c 2073 7263 5f63 7478 5b27  ed_db, src_ctx['
+00010b60: 6462 5f6e 616d 6527 5d20 3d20 7372 635f  db_name'] = src_
+00010b70: 6374 785b 2764 625f 6e61 6d65 275d 2c20  ctx['db_name'], 
+00010b80: 7467 745f 6374 785b 2764 625f 6e61 6d65  tgt_ctx['db_name
+00010b90: 275d 0a20 2020 2069 6620 2873 7263 5f63  '].    if (src_c
+00010ba0: 7478 5b27 7372 635f 6f64 6f6f 5f66 7665  tx['src_odoo_fve
+00010bb0: 7227 5d20 3d3d 2027 372e 3027 2061 6e64  r'] == '7.0' and
+00010bc0: 0a20 2020 2020 2020 2020 2020 2074 6774  .            tgt
+00010bd0: 5f63 7478 5b27 7467 745f 6f64 6f6f 5f66  _ctx['tgt_odoo_f
+00010be0: 7665 7227 5d20 3d3d 2027 382e 3027 293a  ver'] == '8.0'):
+00010bf0: 0a20 2020 2020 2020 2071 7565 7279 203d  .        query =
+00010c00: 2027 2727 7570 6461 7465 2069 725f 7569   '''update ir_ui
+00010c10: 5f76 6965 770a 2020 2020 2020 2020 2020  _view.          
+00010c20: 2020 2020 2020 7365 7420 6172 6368 3d52        set arch=R
+00010c30: 4547 4558 505f 5245 504c 4143 4528 6172  EGEXP_REPLACE(ar
+00010c40: 6368 2c20 273c 6669 656c 6420 6e61 6d65  ch, '<field name
+00010c50: 3d22 6d65 6e75 5f69 6422 2e2a 2f3e 272c  ="menu_id".*/>',
+00010c60: 2027 2729 0a20 2020 2020 2020 2020 2020   '').           
+00010c70: 2020 2020 2077 6865 7265 206d 6f64 656c       where model
+00010c80: 3d27 7265 732e 7573 6572 7327 2061 6e64  ='res.users' and
+00010c90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010ca0: 2020 2020 2020 2061 7263 6820 6c69 6b65         arch like
+00010cb0: 2027 253c 6669 656c 6420 6e61 6d65 3d5f   '%<field name=_
+00010cc0: 6d65 6e75 5f69 645f 2527 3b27 2727 0a20  menu_id_%';'''. 
+00010cd0: 2020 2020 2020 2065 7865 635f 7371 6c28         exec_sql(
+00010ce0: 7372 635f 6374 782c 2071 7565 7279 290a  src_ctx, query).
+00010cf0: 2020 2020 656c 6966 2028 7372 635f 6374      elif (src_ct
+00010d00: 785b 2773 7263 5f6f 646f 6f5f 6676 6572  x['src_odoo_fver
+00010d10: 275d 203d 3d20 2738 2e30 2720 616e 640a  '] == '8.0' and.
+00010d20: 2020 2020 2020 2020 2020 2020 7467 745f              tgt_
+00010d30: 6374 785b 2774 6774 5f6f 646f 6f5f 6676  ctx['tgt_odoo_fv
+00010d40: 6572 275d 203d 3d20 2739 2e30 2729 3a0a  er'] == '9.0'):.
+00010d50: 2020 2020 2020 2020 6966 2027 6163 636f          if 'acco
+00010d60: 756e 745f 7061 796d 656e 7427 2069 6e20  unt_payment' in 
+00010d70: 7372 635f 6374 785b 2773 7263 5f6d 6f64  src_ctx['src_mod
+00010d80: 756c 655f 6c69 7374 275d 3a0a 2020 2020  ule_list']:.    
+00010d90: 2020 2020 2020 2020 7374 7320 3d20 636c          sts = cl
+00010da0: 6f64 6f6f 2e61 6374 5f69 6e73 7461 6c6c  odoo.act_install
+00010db0: 5f6d 6f64 756c 6573 280a 2020 2020 2020  _modules(.      
+00010dc0: 2020 2020 2020 2020 2020 7372 635f 6374            src_ct
+00010dd0: 782c 206d 6f64 756c 655f 6c69 7374 3d5b  x, module_list=[
+00010de0: 2761 6363 6f75 6e74 5f62 616e 6b69 6e67  'account_banking
+00010df0: 5f70 6179 6d65 6e74 5f65 7870 6f72 7427  _payment_export'
+00010e00: 5d29 0a20 2020 2073 7263 5f63 7478 5b27  ]).    src_ctx['
+00010e10: 6462 5f6e 616d 6527 5d20 3d20 7361 7665  db_name'] = save
+00010e20: 645f 6462 0a0a 0a64 6566 2066 6978 5f62  d_db...def fix_b
+00010e30: 7567 5f70 6f73 7428 7372 635f 6374 782c  ug_post(src_ctx,
+00010e40: 2074 6774 5f63 7478 2c20 7467 745f 6675   tgt_ctx, tgt_fu
+00010e50: 6c6c 5f6c 636f 6e66 2c20 7467 745f 7061  ll_lconf, tgt_pa
+00010e60: 7468 7329 3a0a 2020 2020 6966 2028 7372  ths):.    if (sr
+00010e70: 635f 6374 785b 2773 7263 5f6f 646f 6f5f  c_ctx['src_odoo_
+00010e80: 6676 6572 275d 203d 3d20 2737 2e30 2720  fver'] == '7.0' 
+00010e90: 616e 640a 2020 2020 2020 2020 2020 2020  and.            
+00010ea0: 7467 745f 6374 785b 2774 6774 5f6f 646f  tgt_ctx['tgt_odo
+00010eb0: 6f5f 6676 6572 275d 203d 3d20 2738 2e30  o_fver'] == '8.0
+00010ec0: 2729 3a0a 2020 2020 2020 2020 7061 7373  '):.        pass
+00010ed0: 0a0a 0a64 6566 206d 6967 7261 7465 5f6f  ...def migrate_o
+00010ee0: 646f 6f28 7372 635f 6374 782c 2074 6774  doo(src_ctx, tgt
+00010ef0: 5f63 7478 2c20 7372 635f 636f 6e66 6967  _ctx, src_config
+00010f00: 2c20 7467 745f 636f 6e66 6967 2c20 7068  , tgt_config, ph
+00010f10: 6173 653d 4e6f 6e65 293a 0a0a 2020 2020  ase=None):..    
+00010f20: 6465 6620 6765 745f 7772 6f6e 675f 6d6f  def get_wrong_mo
+00010f30: 6475 6c65 7328 6374 782c 2062 6164 5f6d  dules(ctx, bad_m
+00010f40: 6f64 756c 655f 6c69 7374 3d4e 6f6e 6529  odule_list=None)
+00010f50: 3a0a 2020 2020 2020 2020 6966 2073 7263  :.        if src
+00010f60: 5f63 7478 5b27 6472 795f 7275 6e27 5d3a  _ctx['dry_run']:
+00010f70: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00010f80: 7572 6e20 5b5d 0a20 2020 2020 2020 2069  urn [].        i
+00010f90: 6620 6261 645f 6d6f 6475 6c65 5f6c 6973  f bad_module_lis
+00010fa0: 743a 0a20 2020 2020 2020 2020 2020 2069  t:.            i
+00010fb0: 6620 6c65 6e28 6261 645f 6d6f 6475 6c65  f len(bad_module
+00010fc0: 5f6c 6973 7429 203d 3d20 313a 0a20 2020  _list) == 1:.   
+00010fd0: 2020 2020 2020 2020 2020 2020 2071 7565               que
+00010fe0: 7279 203d 2027 2727 7365 6c65 6374 2069  ry = '''select i
+00010ff0: 642c 6e61 6d65 2c73 7461 7465 2066 726f  d,name,state fro
+00011000: 6d20 6972 5f6d 6f64 756c 655f 6d6f 6475  m ir_module_modu
+00011010: 6c65 0a20 2020 2020 2020 2020 2020 2020  le.             
+00011020: 2020 2020 2020 2020 2020 2020 2020 7768                wh
+00011030: 6572 6520 7374 6174 6520 6e6f 7420 696e  ere state not in
+00011040: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011050: 2020 2020 2020 2020 2020 2020 2827 696e              ('in
+00011060: 7374 616c 6c65 6427 2c20 2775 6e69 6e73  stalled', 'unins
+00011070: 7461 6c6c 6564 272c 2027 756e 696e 7374  talled', 'uninst
+00011080: 616c 6c61 626c 6527 2920 616e 640a 2020  allable') and.  
 00011090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000110a0: 2020 2020 2020 206e 616d 6520 3d20 2725         name = '%
-000110b0: 7327 3b27 2727 2025 2062 6164 5f6d 6f64  s';''' % bad_mod
-000110c0: 756c 655f 6c69 7374 5b30 5d0a 2020 2020  ule_list[0].    
-000110d0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-000110e0: 2020 2020 2020 2020 2020 2020 2020 7175                qu
-000110f0: 6572 7920 3d20 2727 2773 656c 6563 7420  ery = '''select 
-00011100: 6964 2c6e 616d 652c 7374 6174 6520 6672  id,name,state fr
-00011110: 6f6d 2069 725f 6d6f 6475 6c65 5f6d 6f64  om ir_module_mod
-00011120: 756c 650a 2020 2020 2020 2020 2020 2020  ule.            
-00011130: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-00011140: 6865 7265 2073 7461 7465 206e 6f74 2069  here state not i
-00011150: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
-00011160: 2020 2020 2020 2020 2020 2020 2028 2769               ('i
-00011170: 6e73 7461 6c6c 6564 272c 2027 756e 696e  nstalled', 'unin
-00011180: 7374 616c 6c65 6427 2c20 2775 6e69 6e73  stalled', 'unins
-00011190: 7461 6c6c 6162 6c65 2729 2061 6e64 0a20  tallable') and. 
-000111a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000111b0: 2020 2020 2020 2020 2020 6e61 6d65 2069            name i
-000111c0: 6e20 2825 7329 3b27 2727 2025 2028 0a20  n (%s);''' % (. 
-000111d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000111e0: 2020 2020 2020 2020 2020 2020 2020 2227                "'
-000111f0: 2573 2722 2025 2022 272c 2722 2e6a 6f69  %s'" % "','".joi
-00011200: 6e28 6261 645f 6d6f 6475 6c65 5f6c 6973  n(bad_module_lis
-00011210: 7429 290a 0a20 2020 2020 2020 2065 6c73  t))..        els
-00011220: 653a 0a20 2020 2020 2020 2020 2020 2071  e:.            q
-00011230: 7565 7279 203d 2027 2727 7365 6c65 6374  uery = '''select
-00011240: 2069 642c 6e61 6d65 2c73 7461 7465 2066   id,name,state f
-00011250: 726f 6d20 6972 5f6d 6f64 756c 655f 6d6f  rom ir_module_mo
-00011260: 6475 6c65 0a20 2020 2020 2020 2020 2020  dule.           
-00011270: 2020 2020 2020 2020 2020 2020 7768 6572              wher
-00011280: 6520 7374 6174 6520 6e6f 7420 696e 0a20  e state not in. 
-00011290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000112a0: 2020 2020 2020 2827 696e 7374 616c 6c65        ('installe
-000112b0: 6427 2c20 2775 6e69 6e73 7461 6c6c 6564  d', 'uninstalled
-000112c0: 272c 2027 756e 696e 7374 616c 6c61 626c  ', 'uninstallabl
-000112d0: 6527 293b 2727 270a 2020 2020 2020 2020  e');'''.        
-000112e0: 726f 7773 203d 2065 7865 635f 7371 6c28  rows = exec_sql(
-000112f0: 6374 782c 2071 7565 7279 2c20 7265 7370  ctx, query, resp
-00011300: 6f6e 7365 3d54 7275 6529 0a20 2020 2020  onse=True).     
-00011310: 2020 2077 726f 6e67 5f6c 6973 7420 3d20     wrong_list = 
-00011320: 5b5d 0a20 2020 2020 2020 2066 6f72 2072  [].        for r
-00011330: 6f77 2069 6e20 726f 7773 3a0a 2020 2020  ow in rows:.    
-00011340: 2020 2020 2020 2020 6966 206e 6f74 2062          if not b
-00011350: 6164 5f6d 6f64 756c 655f 6c69 7374 206f  ad_module_list o
-00011360: 7220 726f 775b 315d 206e 6f74 2069 6e20  r row[1] not in 
-00011370: 6261 645f 6d6f 6475 6c65 5f6c 6973 743a  bad_module_list:
-00011380: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011390: 2077 726f 6e67 5f6c 6973 742e 6170 7065   wrong_list.appe
-000113a0: 6e64 2872 6f77 5b31 5d29 0a20 2020 2020  nd(row[1]).     
-000113b0: 2020 2072 6574 7572 6e20 7772 6f6e 675f     return wrong_
-000113c0: 6c69 7374 0a0a 2020 2020 6465 6620 7275  list..    def ru
-000113d0: 6e5f 6f70 656e 7570 6772 6164 6528 7467  n_openupgrade(tg
-000113e0: 745f 6374 782c 206f 755f 7665 725f 7061  t_ctx, ou_ver_pa
-000113f0: 7468 2c20 7467 745f 6675 6c6c 5f6c 636f  th, tgt_full_lco
-00011400: 6e66 293a 0a20 2020 2020 2020 206f 7570  nf):.        oup
-00011410: 6174 685f 7363 7269 7074 203d 2046 616c  ath_script = Fal
-00011420: 7365 0a20 2020 2020 2020 2066 6f72 2070  se.        for p
-00011430: 2069 6e20 2827 272c 2027 6f64 6f6f 272c   in ('', 'odoo',
-00011440: 2027 6f70 656e 6572 7027 2c20 2773 6572   'openerp', 'ser
-00011450: 7665 7227 293a 0a20 2020 2020 2020 2020  ver'):.         
-00011460: 2020 2069 6620 6f75 7061 7468 5f73 6372     if oupath_scr
-00011470: 6970 743a 0a20 2020 2020 2020 2020 2020  ipt:.           
-00011480: 2020 2020 2062 7265 616b 0a20 2020 2020       break.     
-00011490: 2020 2020 2020 2066 6f72 206e 2069 6e20         for n in 
-000114a0: 2827 6f64 6f6f 2d62 696e 272c 2027 6f70  ('odoo-bin', 'op
-000114b0: 656e 6572 702d 7365 7276 6572 2729 3a0a  enerp-server'):.
-000114c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000114d0: 6966 2070 3a0a 2020 2020 2020 2020 2020  if p:.          
-000114e0: 2020 2020 2020 2020 2020 7363 7269 7074            script
-000114f0: 203d 206f 732e 7061 7468 2e6a 6f69 6e28   = os.path.join(
-00011500: 6f75 5f76 6572 5f70 6174 682c 2070 2c20  ou_ver_path, p, 
-00011510: 6e29 0a20 2020 2020 2020 2020 2020 2020  n).             
-00011520: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00011530: 2020 2020 2020 2020 2020 2020 2073 6372               scr
-00011540: 6970 7420 3d20 6f73 2e70 6174 682e 6a6f  ipt = os.path.jo
-00011550: 696e 286f 755f 7665 725f 7061 7468 2c20  in(ou_ver_path, 
-00011560: 6e29 0a20 2020 2020 2020 2020 2020 2020  n).             
-00011570: 2020 2069 6620 6f73 2e70 6174 682e 6973     if os.path.is
-00011580: 6669 6c65 2873 6372 6970 7429 3a0a 2020  file(script):.  
+000110a0: 2020 2020 2020 2020 206e 616d 6520 3d20           name = 
+000110b0: 2725 7327 3b27 2727 2025 2062 6164 5f6d  '%s';''' % bad_m
+000110c0: 6f64 756c 655f 6c69 7374 5b30 5d0a 2020  odule_list[0].  
+000110d0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+000110e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000110f0: 7175 6572 7920 3d20 2727 2773 656c 6563  query = '''selec
+00011100: 7420 6964 2c6e 616d 652c 7374 6174 6520  t id,name,state 
+00011110: 6672 6f6d 2069 725f 6d6f 6475 6c65 5f6d  from ir_module_m
+00011120: 6f64 756c 650a 2020 2020 2020 2020 2020  odule.          
+00011130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011140: 2077 6865 7265 2073 7461 7465 206e 6f74   where state not
+00011150: 2069 6e0a 2020 2020 2020 2020 2020 2020   in.            
+00011160: 2020 2020 2020 2020 2020 2020 2020 2028                 (
+00011170: 2769 6e73 7461 6c6c 6564 272c 2027 756e  'installed', 'un
+00011180: 696e 7374 616c 6c65 6427 2c20 2775 6e69  installed', 'uni
+00011190: 6e73 7461 6c6c 6162 6c65 2729 2061 6e64  nstallable') and
+000111a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000111b0: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
+000111c0: 2069 6e20 2825 7329 3b27 2727 2025 2028   in (%s);''' % (
+000111d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000111e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000111f0: 2227 2573 2722 2025 2022 272c 2722 2e6a  "'%s'" % "','".j
+00011200: 6f69 6e28 6261 645f 6d6f 6475 6c65 5f6c  oin(bad_module_l
+00011210: 6973 7429 290a 0a20 2020 2020 2020 2065  ist))..        e
+00011220: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00011230: 2071 7565 7279 203d 2027 2727 7365 6c65   query = '''sele
+00011240: 6374 2069 642c 6e61 6d65 2c73 7461 7465  ct id,name,state
+00011250: 2066 726f 6d20 6972 5f6d 6f64 756c 655f   from ir_module_
+00011260: 6d6f 6475 6c65 0a20 2020 2020 2020 2020  module.         
+00011270: 2020 2020 2020 2020 2020 2020 2020 7768                wh
+00011280: 6572 6520 7374 6174 6520 6e6f 7420 696e  ere state not in
+00011290: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000112a0: 2020 2020 2020 2020 2827 696e 7374 616c          ('instal
+000112b0: 6c65 6427 2c20 2775 6e69 6e73 7461 6c6c  led', 'uninstall
+000112c0: 6564 272c 2027 756e 696e 7374 616c 6c61  ed', 'uninstalla
+000112d0: 626c 6527 293b 2727 270a 2020 2020 2020  ble');'''.      
+000112e0: 2020 726f 7773 203d 2065 7865 635f 7371    rows = exec_sq
+000112f0: 6c28 6374 782c 2071 7565 7279 2c20 7265  l(ctx, query, re
+00011300: 7370 6f6e 7365 3d54 7275 6529 0a20 2020  sponse=True).   
+00011310: 2020 2020 2077 726f 6e67 5f6c 6973 7420       wrong_list 
+00011320: 3d20 5b5d 0a20 2020 2020 2020 2066 6f72  = [].        for
+00011330: 2072 6f77 2069 6e20 726f 7773 3a0a 2020   row in rows:.  
+00011340: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
+00011350: 2062 6164 5f6d 6f64 756c 655f 6c69 7374   bad_module_list
+00011360: 206f 7220 726f 775b 315d 206e 6f74 2069   or row[1] not i
+00011370: 6e20 6261 645f 6d6f 6475 6c65 5f6c 6973  n bad_module_lis
+00011380: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
+00011390: 2020 2077 726f 6e67 5f6c 6973 742e 6170     wrong_list.ap
+000113a0: 7065 6e64 2872 6f77 5b31 5d29 0a20 2020  pend(row[1]).   
+000113b0: 2020 2020 2072 6574 7572 6e20 7772 6f6e       return wron
+000113c0: 675f 6c69 7374 0a0a 2020 2020 6465 6620  g_list..    def 
+000113d0: 7275 6e5f 6f70 656e 7570 6772 6164 6528  run_openupgrade(
+000113e0: 7467 745f 6374 782c 206f 755f 7665 725f  tgt_ctx, ou_ver_
+000113f0: 7061 7468 2c20 7467 745f 6675 6c6c 5f6c  path, tgt_full_l
+00011400: 636f 6e66 293a 0a20 2020 2020 2020 206f  conf):.        o
+00011410: 7570 6174 685f 7363 7269 7074 203d 2046  upath_script = F
+00011420: 616c 7365 0a20 2020 2020 2020 2066 6f72  alse.        for
+00011430: 2070 2069 6e20 2827 272c 2027 6f64 6f6f   p in ('', 'odoo
+00011440: 272c 2027 6f70 656e 6572 7027 2c20 2773  ', 'openerp', 's
+00011450: 6572 7665 7227 293a 0a20 2020 2020 2020  erver'):.       
+00011460: 2020 2020 2069 6620 6f75 7061 7468 5f73       if oupath_s
+00011470: 6372 6970 743a 0a20 2020 2020 2020 2020  cript:.         
+00011480: 2020 2020 2020 2062 7265 616b 0a20 2020         break.   
+00011490: 2020 2020 2020 2020 2066 6f72 206e 2069           for n i
+000114a0: 6e20 2827 6f64 6f6f 2d62 696e 272c 2027  n ('odoo-bin', '
+000114b0: 6f70 656e 6572 702d 7365 7276 6572 2729  openerp-server')
+000114c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000114d0: 2020 6966 2070 3a0a 2020 2020 2020 2020    if p:.        
+000114e0: 2020 2020 2020 2020 2020 2020 7363 7269              scri
+000114f0: 7074 203d 206f 732e 7061 7468 2e6a 6f69  pt = os.path.joi
+00011500: 6e28 6f75 5f76 6572 5f70 6174 682c 2070  n(ou_ver_path, p
+00011510: 2c20 6e29 0a20 2020 2020 2020 2020 2020  , n).           
+00011520: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00011530: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00011540: 6372 6970 7420 3d20 6f73 2e70 6174 682e  cript = os.path.
+00011550: 6a6f 696e 286f 755f 7665 725f 7061 7468  join(ou_ver_path
+00011560: 2c20 6e29 0a20 2020 2020 2020 2020 2020  , n).           
+00011570: 2020 2020 2069 6620 6f73 2e70 6174 682e       if os.path.
+00011580: 6973 6669 6c65 2873 6372 6970 7429 3a0a  isfile(script):.
 00011590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000115a0: 2020 6f75 7061 7468 5f73 6372 6970 7420    oupath_script 
-000115b0: 3d20 7363 7269 7074 0a20 2020 2020 2020  = script.       
-000115c0: 2020 2020 2020 2020 2020 2020 2062 7265               bre
-000115d0: 616b 0a20 2020 2020 2020 2069 6620 7372  ak.        if sr
-000115e0: 635f 6374 785b 276e 6f5f 7665 6e76 275d  c_ctx['no_venv']
-000115f0: 3a0a 2020 2020 2020 2020 2020 2020 7374  :.            st
-00011600: 7320 3d20 7275 6e5f 7472 6163 6564 286f  s = run_traced(o
-00011610: 7570 6174 685f 7363 7269 7074 2c0a 2020  upath_script,.  
+000115a0: 2020 2020 6f75 7061 7468 5f73 6372 6970      oupath_scrip
+000115b0: 7420 3d20 7363 7269 7074 0a20 2020 2020  t = script.     
+000115c0: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+000115d0: 7265 616b 0a20 2020 2020 2020 2069 6620  reak.        if 
+000115e0: 7372 635f 6374 785b 276e 6f5f 7665 6e76  src_ctx['no_venv
+000115f0: 275d 3a0a 2020 2020 2020 2020 2020 2020  ']:.            
+00011600: 7374 7320 3d20 7275 6e5f 7472 6163 6564  sts = run_traced
+00011610: 286f 7570 6174 685f 7363 7269 7074 2c0a  (oupath_script,.
 00011620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011630: 2020 2020 2020 2020 2020 2027 2d63 272c             '-c',
-00011640: 2074 6774 5f66 756c 6c5f 6c63 6f6e 662c   tgt_full_lconf,
-00011650: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011660: 2020 2020 2020 2020 2020 2020 2020 272d                '-
-00011670: 6427 2c20 7467 745f 6374 785b 2764 625f  d', tgt_ctx['db_
-00011680: 6e61 6d65 275d 2c0a 2020 2020 2020 2020  name'],.        
+00011630: 2020 2020 2020 2020 2020 2020 2027 2d63               '-c
+00011640: 272c 2074 6774 5f66 756c 6c5f 6c63 6f6e  ', tgt_full_lcon
+00011650: 662c 0a20 2020 2020 2020 2020 2020 2020  f,.             
+00011660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011670: 272d 6427 2c20 7467 745f 6374 785b 2764  '-d', tgt_ctx['d
+00011680: 625f 6e61 6d65 275d 2c0a 2020 2020 2020  b_name'],.      
 00011690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000116a0: 2020 2020 2027 2d75 272c 2027 616c 6c27       '-u', 'all'
-000116b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000116c0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-000116d0: 2d2d 7374 6f70 2d61 6674 6572 2d69 6e69  --stop-after-ini
-000116e0: 7427 2c0a 2020 2020 2020 2020 2020 2020  t',.            
+000116a0: 2020 2020 2020 2027 2d75 272c 2027 616c         '-u', 'al
+000116b0: 6c27 2c0a 2020 2020 2020 2020 2020 2020  l',.            
+000116c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000116d0: 2027 2d2d 7374 6f70 2d61 6674 6572 2d69   '--stop-after-i
+000116e0: 6e69 7427 2c0a 2020 2020 2020 2020 2020  nit',.          
 000116f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011700: 2027 2d2d 6e6f 2d78 6d6c 7270 6327 2c0a   '--no-xmlrpc',.
-00011710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011720: 2020 2020 2020 2020 2020 2020 2027 2d2d               '--
-00011730: 6c6f 6766 696c 653d 2573 2720 2520 7467  logfile=%s' % tg
-00011740: 745f 6374 785b 276c 6f67 6669 6c65 275d  t_ctx['logfile']
-00011750: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-00011760: 2020 2020 2020 2020 2020 2020 7363 7269              scri
-00011770: 7074 203d 206f 732e 7061 7468 2e6a 6f69  pt = os.path.joi
-00011780: 6e28 6f75 5f76 6572 5f70 6174 682c 2027  n(ou_ver_path, '
-00011790: 6d69 6772 6174 652e 7368 2729 0a20 2020  migrate.sh').   
-000117a0: 2020 2020 2020 2020 2066 6420 3d20 6f70           fd = op
-000117b0: 656e 2873 6372 6970 742c 2027 7727 290a  en(script, 'w').
-000117c0: 2020 2020 2020 2020 2020 2020 6664 2e77              fd.w
-000117d0: 7269 7465 2827 6364 2025 735c 6e27 2025  rite('cd %s\n' %
-000117e0: 2074 6774 5f63 7478 5b27 7665 6e76 5f6f   tgt_ctx['venv_o
-000117f0: 7570 6174 6827 5d29 0a20 2020 2020 2020  upath']).       
-00011800: 2020 2020 2066 642e 7772 6974 6528 6227       fd.write(b'
-00011810: 736f 7572 6365 202e 2f62 696e 2f61 6374  source ./bin/act
-00011820: 6976 6174 655c 6e27 290a 2020 2020 2020  ivate\n').      
-00011830: 2020 2020 2020 6664 2e77 7269 7465 2862        fd.write(b
-00011840: 2725 7320 2d63 2025 7320 2d64 2025 7320  '%s -c %s -d %s 
-00011850: 2d75 2061 6c6c 202d 2d73 746f 702d 6166  -u all --stop-af
-00011860: 7465 722d 696e 6974 202d 2d6e 6f2d 786d  ter-init --no-xm
-00011870: 6c72 7063 270a 2020 2020 2020 2020 2020  lrpc'.          
-00011880: 2020 2020 2020 2020 2020 2062 2720 2d2d             b' --
-00011890: 6c6f 6766 696c 653d 2573 5c6e 2720 2520  logfile=%s\n' % 
-000118a0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-000118b0: 2020 2020 2020 2020 2020 206f 7570 6174             oupat
-000118c0: 685f 7363 7269 7074 2c20 7467 745f 6675  h_script, tgt_fu
-000118d0: 6c6c 5f6c 636f 6e66 2c0a 2020 2020 2020  ll_lconf,.      
+00011700: 2020 2027 2d2d 6e6f 2d78 6d6c 7270 6327     '--no-xmlrpc'
+00011710: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00011720: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00011730: 2d2d 6c6f 6766 696c 653d 2573 2720 2520  --logfile=%s' % 
+00011740: 7467 745f 6374 785b 276c 6f67 6669 6c65  tgt_ctx['logfile
+00011750: 275d 290a 2020 2020 2020 2020 656c 7365  ']).        else
+00011760: 3a0a 2020 2020 2020 2020 2020 2020 7363  :.            sc
+00011770: 7269 7074 203d 206f 732e 7061 7468 2e6a  ript = os.path.j
+00011780: 6f69 6e28 6f75 5f76 6572 5f70 6174 682c  oin(ou_ver_path,
+00011790: 2027 6d69 6772 6174 652e 7368 2729 0a20   'migrate.sh'). 
+000117a0: 2020 2020 2020 2020 2020 2066 6420 3d20             fd = 
+000117b0: 6f70 656e 2873 6372 6970 742c 2027 7727  open(script, 'w'
+000117c0: 290a 2020 2020 2020 2020 2020 2020 6664  ).            fd
+000117d0: 2e77 7269 7465 2827 6364 2025 735c 6e27  .write('cd %s\n'
+000117e0: 2025 2074 6774 5f63 7478 5b27 7665 6e76   % tgt_ctx['venv
+000117f0: 5f6f 7570 6174 6827 5d29 0a20 2020 2020  _oupath']).     
+00011800: 2020 2020 2020 2066 642e 7772 6974 6528         fd.write(
+00011810: 6227 736f 7572 6365 202e 2f62 696e 2f61  b'source ./bin/a
+00011820: 6374 6976 6174 655c 6e27 290a 2020 2020  ctivate\n').    
+00011830: 2020 2020 2020 2020 6664 2e77 7269 7465          fd.write
+00011840: 2862 2725 7320 2d63 2025 7320 2d64 2025  (b'%s -c %s -d %
+00011850: 7320 2d75 2061 6c6c 202d 2d73 746f 702d  s -u all --stop-
+00011860: 6166 7465 722d 696e 6974 202d 2d6e 6f2d  after-init --no-
+00011870: 786d 6c72 7063 270a 2020 2020 2020 2020  xmlrpc'.        
+00011880: 2020 2020 2020 2020 2020 2020 2062 2720               b' 
+00011890: 2d2d 6c6f 6766 696c 653d 2573 5c6e 2720  --logfile=%s\n' 
+000118a0: 2520 280a 2020 2020 2020 2020 2020 2020  % (.            
+000118b0: 2020 2020 2020 2020 2020 2020 206f 7570               oup
+000118c0: 6174 685f 7363 7269 7074 2c20 7467 745f  ath_script, tgt_
+000118d0: 6675 6c6c 5f6c 636f 6e66 2c0a 2020 2020  full_lconf,.    
 000118e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000118f0: 2020 2074 6774 5f63 7478 5b27 6462 5f6e     tgt_ctx['db_n
-00011900: 616d 6527 5d2c 0a20 2020 2020 2020 2020  ame'],.         
+000118f0: 2020 2020 2074 6774 5f63 7478 5b27 6462       tgt_ctx['db
+00011900: 5f6e 616d 6527 5d2c 0a20 2020 2020 2020  _name'],.       
 00011910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011920: 7467 745f 6374 785b 276c 6f67 6669 6c65  tgt_ctx['logfile
-00011930: 275d 2929 0a20 2020 2020 2020 2020 2020  '])).           
-00011940: 2066 642e 7772 6974 6528 6227 7374 733d   fd.write(b'sts=
-00011950: 243f 5c6e 2729 0a20 2020 2020 2020 2020  $?\n').         
-00011960: 2020 2066 642e 7772 6974 6528 6227 6465     fd.write(b'de
-00011970: 6163 7469 7661 7465 5c6e 2729 0a20 2020  activate\n').   
-00011980: 2020 2020 2020 2020 2066 642e 7772 6974           fd.writ
-00011990: 6528 6227 6578 6974 2024 7374 735c 6e27  e(b'exit $sts\n'
-000119a0: 290a 2020 2020 2020 2020 2020 2020 6664  ).            fd
-000119b0: 2e63 6c6f 7365 2829 0a20 2020 2020 2020  .close().       
-000119c0: 2020 2020 206f 732e 6368 6d6f 6428 7363       os.chmod(sc
-000119d0: 7269 7074 2c20 306f 3734 3429 0a20 2020  ript, 0o744).   
-000119e0: 2020 2020 2020 2020 2073 7473 203d 2030           sts = 0
-000119f0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00011a00: 6e6f 7420 7372 635f 6374 785b 2764 7279  not src_ctx['dry
-00011a10: 5f72 756e 275d 3a0a 2020 2020 2020 2020  _run']:.        
-00011a20: 2020 2020 2020 2020 7374 7320 3d20 6f73          sts = os
-00011a30: 2e73 7973 7465 6d28 7363 7269 7074 290a  .system(script).
-00011a40: 2020 2020 2020 2020 6966 2073 7473 3a0a          if sts:.
-00011a50: 2020 2020 2020 2020 2020 2020 6f73 302e              os0.
-00011a60: 776c 6f67 2827 2a2a 2a20 5265 7475 726e  wlog('*** Return
-00011a70: 2063 6f64 6520 2564 202a 2a2a 2729 0a20   code %d ***'). 
-00011a80: 2020 2020 2020 2065 6c69 6620 6e6f 7420         elif not 
-00011a90: 7372 635f 6374 785b 2764 7279 5f72 756e  src_ctx['dry_run
-00011aa0: 275d 3a0a 2020 2020 2020 2020 2020 2020  ']:.            
-00011ab0: 7469 6d65 2e73 6c65 6570 2835 290a 0a20  time.sleep(5).. 
-00011ac0: 2020 2070 6861 7365 203d 2070 6861 7365     phase = phase
-00011ad0: 206f 7220 320a 2020 2020 7467 745f 7361   or 2.    tgt_sa
-00011ae0: 7665 645f 6663 6f6e 6620 3d20 7467 745f  ved_fconf = tgt_
-00011af0: 6374 785b 2763 6f6e 665f 666e 275d 0a20  ctx['conf_fn']. 
-00011b00: 2020 2073 7263 5f66 756c 6c5f 6c63 6f6e     src_full_lcon
-00011b10: 6620 3d20 7072 6570 6172 655f 636f 6e66  f = prepare_conf
-00011b20: 6967 5f66 696c 6528 7372 635f 6374 782c  ig_file(src_ctx,
-00011b30: 2073 7263 5f63 6f6e 6669 6729 0a20 2020   src_config).   
-00011b40: 2069 6620 2873 7263 5f63 7478 5b27 7372   if (src_ctx['sr
-00011b50: 635f 7669 6427 5d20 3d3d 2073 7263 5f63  c_vid'] == src_c
-00011b60: 7478 5b27 6672 6f6d 5f62 7261 6e63 6827  tx['from_branch'
-00011b70: 5d20 616e 640a 2020 2020 2020 2020 2020  ] and.          
-00011b80: 2020 6765 745f 7772 6f6e 675f 6d6f 6475    get_wrong_modu
-00011b90: 6c65 7328 7372 635f 6374 7829 293a 0a20  les(src_ctx)):. 
-00011ba0: 2020 2020 2020 2069 6620 7068 6173 6520         if phase 
-00011bb0: 3d3d 2031 3a0a 2020 2020 2020 2020 2020  == 1:.          
-00011bc0: 2020 6f73 302e 776c 6f67 2827 2a2a 2a20    os0.wlog('*** 
-00011bd0: 556e 7374 6162 6c65 2069 6e73 7461 6c6c  Unstable install
-00011be0: 6174 696f 6e20 2a2a 2a27 290a 2020 2020  ation ***').    
-00011bf0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00011c00: 2020 2020 2020 6f73 302e 776c 6f67 2827        os0.wlog('
-00011c10: 2a2a 2a20 556e 7374 6162 6c65 2069 6e73  *** Unstable ins
-00011c20: 7461 6c6c 6174 696f 6e3a 2074 7279 2074  tallation: try t
-00011c30: 6f20 636f 7272 6563 7420 6572 726f 7273  o correct errors
-00011c40: 202a 2a2a 2729 0a20 2020 2020 2020 2020   ***').         
-00011c50: 2020 2072 756e 5f6f 646f 6f5f 616c 6c74     run_odoo_allt
-00011c60: 6573 7428 7372 635f 6374 785b 2774 6774  est(src_ctx['tgt
-00011c70: 5f76 6964 275d 2c20 7372 635f 6675 6c6c  _vid'], src_full
-00011c80: 5f6c 636f 6e66 2c0a 2020 2020 2020 2020  _lconf,.        
+00011920: 2020 7467 745f 6374 785b 276c 6f67 6669    tgt_ctx['logfi
+00011930: 6c65 275d 2929 0a20 2020 2020 2020 2020  le'])).         
+00011940: 2020 2066 642e 7772 6974 6528 6227 7374     fd.write(b'st
+00011950: 733d 243f 5c6e 2729 0a20 2020 2020 2020  s=$?\n').       
+00011960: 2020 2020 2066 642e 7772 6974 6528 6227       fd.write(b'
+00011970: 6465 6163 7469 7661 7465 5c6e 2729 0a20  deactivate\n'). 
+00011980: 2020 2020 2020 2020 2020 2066 642e 7772             fd.wr
+00011990: 6974 6528 6227 6578 6974 2024 7374 735c  ite(b'exit $sts\
+000119a0: 6e27 290a 2020 2020 2020 2020 2020 2020  n').            
+000119b0: 6664 2e63 6c6f 7365 2829 0a20 2020 2020  fd.close().     
+000119c0: 2020 2020 2020 206f 732e 6368 6d6f 6428         os.chmod(
+000119d0: 7363 7269 7074 2c20 306f 3734 3429 0a20  script, 0o744). 
+000119e0: 2020 2020 2020 2020 2020 2073 7473 203d             sts =
+000119f0: 2030 0a20 2020 2020 2020 2020 2020 2069   0.            i
+00011a00: 6620 6e6f 7420 7372 635f 6374 785b 2764  f not src_ctx['d
+00011a10: 7279 5f72 756e 275d 3a0a 2020 2020 2020  ry_run']:.      
+00011a20: 2020 2020 2020 2020 2020 7374 7320 3d20            sts = 
+00011a30: 6f73 2e73 7973 7465 6d28 7363 7269 7074  os.system(script
+00011a40: 290a 2020 2020 2020 2020 6966 2073 7473  ).        if sts
+00011a50: 3a0a 2020 2020 2020 2020 2020 2020 6f73  :.            os
+00011a60: 302e 776c 6f67 2827 2a2a 2a20 5265 7475  0.wlog('*** Retu
+00011a70: 726e 2063 6f64 6520 2564 202a 2a2a 2729  rn code %d ***')
+00011a80: 0a20 2020 2020 2020 2065 6c69 6620 6e6f  .        elif no
+00011a90: 7420 7372 635f 6374 785b 2764 7279 5f72  t src_ctx['dry_r
+00011aa0: 756e 275d 3a0a 2020 2020 2020 2020 2020  un']:.          
+00011ab0: 2020 7469 6d65 2e73 6c65 6570 2835 290a    time.sleep(5).
+00011ac0: 0a20 2020 2070 6861 7365 203d 2070 6861  .    phase = pha
+00011ad0: 7365 206f 7220 320a 2020 2020 7467 745f  se or 2.    tgt_
+00011ae0: 7361 7665 645f 6663 6f6e 6620 3d20 7467  saved_fconf = tg
+00011af0: 745f 6374 785b 2763 6f6e 665f 666e 275d  t_ctx['conf_fn']
+00011b00: 0a20 2020 2073 7263 5f66 756c 6c5f 6c63  .    src_full_lc
+00011b10: 6f6e 6620 3d20 7072 6570 6172 655f 636f  onf = prepare_co
+00011b20: 6e66 6967 5f66 696c 6528 7372 635f 6374  nfig_file(src_ct
+00011b30: 782c 2073 7263 5f63 6f6e 6669 6729 0a20  x, src_config). 
+00011b40: 2020 2069 6620 2873 7263 5f63 7478 5b27     if (src_ctx['
+00011b50: 7372 635f 7669 6427 5d20 3d3d 2073 7263  src_vid'] == src
+00011b60: 5f63 7478 5b27 6672 6f6d 5f62 7261 6e63  _ctx['from_branc
+00011b70: 6827 5d20 616e 640a 2020 2020 2020 2020  h'] and.        
+00011b80: 2020 2020 6765 745f 7772 6f6e 675f 6d6f      get_wrong_mo
+00011b90: 6475 6c65 7328 7372 635f 6374 7829 293a  dules(src_ctx)):
+00011ba0: 0a20 2020 2020 2020 2069 6620 7068 6173  .        if phas
+00011bb0: 6520 3d3d 2031 3a0a 2020 2020 2020 2020  e == 1:.        
+00011bc0: 2020 2020 6f73 302e 776c 6f67 2827 2a2a      os0.wlog('**
+00011bd0: 2a20 556e 7374 6162 6c65 2069 6e73 7461  * Unstable insta
+00011be0: 6c6c 6174 696f 6e20 2a2a 2a27 290a 2020  llation ***').  
+00011bf0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00011c00: 2020 2020 2020 2020 6f73 302e 776c 6f67          os0.wlog
+00011c10: 2827 2a2a 2a20 556e 7374 6162 6c65 2069  ('*** Unstable i
+00011c20: 6e73 7461 6c6c 6174 696f 6e3a 2074 7279  nstallation: try
+00011c30: 2074 6f20 636f 7272 6563 7420 6572 726f   to correct erro
+00011c40: 7273 202a 2a2a 2729 0a20 2020 2020 2020  rs ***').       
+00011c50: 2020 2020 2072 756e 5f6f 646f 6f5f 616c       run_odoo_al
+00011c60: 6c74 6573 7428 7372 635f 6374 785b 2774  ltest(src_ctx['t
+00011c70: 6774 5f76 6964 275d 2c20 7372 635f 6675  gt_vid'], src_fu
+00011c80: 6c6c 5f6c 636f 6e66 2c0a 2020 2020 2020  ll_lconf,.      
 00011c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ca0: 2020 2020 2073 7263 5f63 7478 5b27 6462       src_ctx['db
-00011cb0: 5f6e 616d 6527 5d2c 2073 7263 5f63 7478  _name'], src_ctx
-00011cc0: 5b27 6c6f 6766 696c 6527 5d29 0a20 2020  ['logfile']).   
-00011cd0: 2020 2020 2020 2020 2062 6164 5f6d 6f64           bad_mod
-00011ce0: 756c 6573 203d 2067 6574 5f77 726f 6e67  ules = get_wrong
-00011cf0: 5f6d 6f64 756c 6573 2873 7263 5f63 7478  _modules(src_ctx
-00011d00: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-00011d10: 2062 6164 5f6d 6f64 756c 6573 3a0a 2020   bad_modules:.  
-00011d20: 2020 2020 2020 2020 2020 2020 2020 6f73                os
-00011d30: 302e 776c 6f67 2827 2a2a 2a20 556e 7374  0.wlog('*** Unst
-00011d40: 6162 6c65 2069 6e73 7461 6c6c 6174 696f  able installatio
-00011d50: 6e20 6475 6520 746f 2025 7320 2a2a 2a27  n due to %s ***'
-00011d60: 2025 2062 6164 5f6d 6f64 756c 6573 290a   % bad_modules).
-00011d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011d80: 6f73 302e 776c 6f67 2827 2a2a 2a20 4d49  os0.wlog('*** MI
-00011d90: 4752 4154 494f 4e20 5354 4f50 5045 4420  GRATION STOPPED 
-00011da0: 2a2a 2a27 290a 2020 2020 2020 2020 2020  ***').          
-00011db0: 2020 2020 2020 7379 732e 6578 6974 2831        sys.exit(1
-00011dc0: 290a 0a20 2020 2073 7263 5f70 6174 6873  )..    src_paths
-00011dd0: 203d 2063 6f6e 6669 675f 6765 745f 6c69   = config_get_li
-00011de0: 7374 2873 7263 5f63 6f6e 6669 672c 2027  st(src_config, '
-00011df0: 6164 646f 6e73 5f70 6174 6827 290a 2020  addons_path').  
-00011e00: 2020 7467 745f 7061 7468 7320 3d20 636f    tgt_paths = co
-00011e10: 6e66 6967 5f67 6574 5f6c 6973 7428 7467  nfig_get_list(tg
-00011e20: 745f 636f 6e66 6967 2c20 2761 6464 6f6e  t_config, 'addon
-00011e30: 735f 7061 7468 2729 0a20 2020 206f 7330  s_path').    os0
-00011e40: 2e77 6c6f 6728 2761 6464 6f6e 735f 7061  .wlog('addons_pa
-00011e50: 7468 3d25 7327 2025 2073 7263 5f70 6174  th=%s' % src_pat
-00011e60: 6873 290a 2020 2020 6966 2070 6861 7365  hs).    if phase
-00011e70: 203e 2031 206f 7220 7372 635f 6374 785b   > 1 or src_ctx[
-00011e80: 2773 7263 5f76 6964 275d 203d 3d20 7372  'src_vid'] == sr
-00011e90: 635f 6374 785b 2766 726f 6d5f 6272 616e  c_ctx['from_bran
-00011ea0: 6368 275d 3a0a 2020 2020 2020 2020 6f73  ch']:.        os
-00011eb0: 302e 776c 6f67 2827 5465 7374 2063 6f6e  0.wlog('Test con
-00011ec0: 6e65 6374 696f 6e20 746f 2073 6f75 7263  nection to sourc
-00011ed0: 6520 6462 2025 7327 2025 2073 7263 5f63  e db %s' % src_c
-00011ee0: 7478 5b27 6462 5f6e 616d 6527 5d29 0a20  tx['db_name']). 
-00011ef0: 2020 2020 2020 2075 6964 2c20 7372 635f         uid, src_
-00011f00: 6374 7820 3d20 636c 6f64 6f6f 2e6f 6572  ctx = clodoo.oer
-00011f10: 705f 7365 745f 656e 7628 0a20 2020 2020  p_set_env(.     
-00011f20: 2020 2020 2020 2063 7478 3d73 7263 5f63         ctx=src_c
-00011f30: 7478 2c20 636f 6e66 6e3d 7372 635f 6675  tx, confn=src_fu
-00011f40: 6c6c 5f6c 636f 6e66 2c20 6462 3d73 7263  ll_lconf, db=src
-00011f50: 5f63 7478 5b27 6462 5f6e 616d 6527 5d29  _ctx['db_name'])
-00011f60: 0a20 2020 2020 2020 2023 2046 4958 206f  .        # FIX o
-00011f70: 6572 705f 7365 745f 656e 7620 6368 616e  erp_set_env chan
-00011f80: 6765 2064 7279 5f72 756e 0a20 2020 2020  ge dry_run.     
-00011f90: 2020 2073 7263 5f63 7478 5b27 6472 795f     src_ctx['dry_
-00011fa0: 7275 6e27 5d20 3d20 7467 745f 6374 785b  run'] = tgt_ctx[
-00011fb0: 2764 7279 5f72 756e 275d 0a20 2020 2020  'dry_run'].     
-00011fc0: 2020 2069 6620 7068 6173 6520 3e20 313a     if phase > 1:
-00011fd0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00011fe0: 2873 7263 5f63 7478 5b27 6f70 745f 7361  (src_ctx['opt_sa
-00011ff0: 6665 275d 2061 6e64 0a20 2020 2020 2020  fe'] and.       
-00012000: 2020 2020 2020 2020 2020 2020 2073 7263               src
-00012010: 5f63 7478 5b27 7372 635f 7669 6427 5d20  _ctx['src_vid'] 
-00012020: 3d3d 2073 7263 5f63 7478 5b27 6672 6f6d  == src_ctx['from
-00012030: 5f62 7261 6e63 6827 5d29 3a0a 2020 2020  _branch']):.    
-00012040: 2020 2020 2020 2020 2020 2020 636c 6f64              clod
-00012050: 6f6f 2e61 6374 5f63 6865 636b 5f63 6f6e  oo.act_check_con
-00012060: 6669 6728 7372 635f 6374 7829 0a20 2020  fig(src_ctx).   
-00012070: 2020 2020 2020 2020 2069 6620 2873 7263           if (src
-00012080: 5f63 7478 5b27 756e 696e 7374 616c 6c5f  _ctx['uninstall_
-00012090: 6d6f 6475 6c65 7327 5d20 616e 640a 2020  modules'] and.  
+00011ca0: 2020 2020 2020 2073 7263 5f63 7478 5b27         src_ctx['
+00011cb0: 6462 5f6e 616d 6527 5d2c 2073 7263 5f63  db_name'], src_c
+00011cc0: 7478 5b27 6c6f 6766 696c 6527 5d29 0a20  tx['logfile']). 
+00011cd0: 2020 2020 2020 2020 2020 2062 6164 5f6d             bad_m
+00011ce0: 6f64 756c 6573 203d 2067 6574 5f77 726f  odules = get_wro
+00011cf0: 6e67 5f6d 6f64 756c 6573 2873 7263 5f63  ng_modules(src_c
+00011d00: 7478 290a 2020 2020 2020 2020 2020 2020  tx).            
+00011d10: 6966 2062 6164 5f6d 6f64 756c 6573 3a0a  if bad_modules:.
+00011d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011d30: 6f73 302e 776c 6f67 2827 2a2a 2a20 556e  os0.wlog('*** Un
+00011d40: 7374 6162 6c65 2069 6e73 7461 6c6c 6174  stable installat
+00011d50: 696f 6e20 6475 6520 746f 2025 7320 2a2a  ion due to %s **
+00011d60: 2a27 2025 2062 6164 5f6d 6f64 756c 6573  *' % bad_modules
+00011d70: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00011d80: 2020 6f73 302e 776c 6f67 2827 2a2a 2a20    os0.wlog('*** 
+00011d90: 4d49 4752 4154 494f 4e20 5354 4f50 5045  MIGRATION STOPPE
+00011da0: 4420 2a2a 2a27 290a 2020 2020 2020 2020  D ***').        
+00011db0: 2020 2020 2020 2020 7379 732e 6578 6974          sys.exit
+00011dc0: 2831 290a 0a20 2020 2073 7263 5f70 6174  (1)..    src_pat
+00011dd0: 6873 203d 2063 6f6e 6669 675f 6765 745f  hs = config_get_
+00011de0: 6c69 7374 2873 7263 5f63 6f6e 6669 672c  list(src_config,
+00011df0: 2027 6164 646f 6e73 5f70 6174 6827 290a   'addons_path').
+00011e00: 2020 2020 7467 745f 7061 7468 7320 3d20      tgt_paths = 
+00011e10: 636f 6e66 6967 5f67 6574 5f6c 6973 7428  config_get_list(
+00011e20: 7467 745f 636f 6e66 6967 2c20 2761 6464  tgt_config, 'add
+00011e30: 6f6e 735f 7061 7468 2729 0a20 2020 206f  ons_path').    o
+00011e40: 7330 2e77 6c6f 6728 2761 6464 6f6e 735f  s0.wlog('addons_
+00011e50: 7061 7468 3d25 7327 2025 2073 7263 5f70  path=%s' % src_p
+00011e60: 6174 6873 290a 2020 2020 6966 2070 6861  aths).    if pha
+00011e70: 7365 203e 2031 206f 7220 7372 635f 6374  se > 1 or src_ct
+00011e80: 785b 2773 7263 5f76 6964 275d 203d 3d20  x['src_vid'] == 
+00011e90: 7372 635f 6374 785b 2766 726f 6d5f 6272  src_ctx['from_br
+00011ea0: 616e 6368 275d 3a0a 2020 2020 2020 2020  anch']:.        
+00011eb0: 6f73 302e 776c 6f67 2827 5465 7374 2063  os0.wlog('Test c
+00011ec0: 6f6e 6e65 6374 696f 6e20 746f 2073 6f75  onnection to sou
+00011ed0: 7263 6520 6462 2025 7327 2025 2073 7263  rce db %s' % src
+00011ee0: 5f63 7478 5b27 6462 5f6e 616d 6527 5d29  _ctx['db_name'])
+00011ef0: 0a20 2020 2020 2020 2075 6964 2c20 7372  .        uid, sr
+00011f00: 635f 6374 7820 3d20 636c 6f64 6f6f 2e6f  c_ctx = clodoo.o
+00011f10: 6572 705f 7365 745f 656e 7628 0a20 2020  erp_set_env(.   
+00011f20: 2020 2020 2020 2020 2063 7478 3d73 7263           ctx=src
+00011f30: 5f63 7478 2c20 636f 6e66 6e3d 7372 635f  _ctx, confn=src_
+00011f40: 6675 6c6c 5f6c 636f 6e66 2c20 6462 3d73  full_lconf, db=s
+00011f50: 7263 5f63 7478 5b27 6462 5f6e 616d 6527  rc_ctx['db_name'
+00011f60: 5d29 0a20 2020 2020 2020 2023 2046 4958  ]).        # FIX
+00011f70: 206f 6572 705f 7365 745f 656e 7620 6368   oerp_set_env ch
+00011f80: 616e 6765 2064 7279 5f72 756e 0a20 2020  ange dry_run.   
+00011f90: 2020 2020 2073 7263 5f63 7478 5b27 6472       src_ctx['dr
+00011fa0: 795f 7275 6e27 5d20 3d20 7467 745f 6374  y_run'] = tgt_ct
+00011fb0: 785b 2764 7279 5f72 756e 275d 0a20 2020  x['dry_run'].   
+00011fc0: 2020 2020 2069 6620 7068 6173 6520 3e20       if phase > 
+00011fd0: 313a 0a20 2020 2020 2020 2020 2020 2069  1:.            i
+00011fe0: 6620 2873 7263 5f63 7478 5b27 6f70 745f  f (src_ctx['opt_
+00011ff0: 7361 6665 275d 2061 6e64 0a20 2020 2020  safe'] and.     
+00012000: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00012010: 7263 5f63 7478 5b27 7372 635f 7669 6427  rc_ctx['src_vid'
+00012020: 5d20 3d3d 2073 7263 5f63 7478 5b27 6672  ] == src_ctx['fr
+00012030: 6f6d 5f62 7261 6e63 6827 5d29 3a0a 2020  om_branch']):.  
+00012040: 2020 2020 2020 2020 2020 2020 2020 636c                cl
+00012050: 6f64 6f6f 2e61 6374 5f63 6865 636b 5f63  odoo.act_check_c
+00012060: 6f6e 6669 6728 7372 635f 6374 7829 0a20  onfig(src_ctx). 
+00012070: 2020 2020 2020 2020 2020 2069 6620 2873             if (s
+00012080: 7263 5f63 7478 5b27 756e 696e 7374 616c  rc_ctx['uninstal
+00012090: 6c5f 6d6f 6475 6c65 7327 5d20 616e 640a  l_modules'] and.
 000120a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000120b0: 2020 7372 635f 6374 785b 2773 7263 5f76    src_ctx['src_v
-000120c0: 6964 275d 203d 3d20 7372 635f 6374 785b  id'] == src_ctx[
-000120d0: 2766 726f 6d5f 6272 616e 6368 275d 293a  'from_branch']):
-000120e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000120f0: 2066 6f72 206d 6f64 756c 6520 696e 2073   for module in s
-00012100: 7263 5f63 7478 5b27 756e 696e 7374 616c  rc_ctx['uninstal
-00012110: 6c5f 6d6f 6475 6c65 7327 5d2e 7370 6c69  l_modules'].spli
-00012120: 7428 272c 2729 3a0a 2020 2020 2020 2020  t(','):.        
-00012130: 2020 2020 2020 2020 2020 2020 6472 6f70              drop
-00012140: 5f6d 6f64 756c 6528 7372 635f 6374 782c  _module(src_ctx,
-00012150: 206d 6f64 756c 652c 2066 6f72 6365 3d54   module, force=T
-00012160: 7275 6529 0a20 2020 2020 2020 2073 7263  rue).        src
-00012170: 5f63 7478 5b27 7372 635f 6d6f 6475 6c65  _ctx['src_module
-00012180: 5f6c 6973 7427 5d20 3d20 6f64 6f6f 5f64  _list'] = odoo_d
-00012190: 6570 656e 6465 6e63 6965 7328 0a20 2020  ependencies(.   
-000121a0: 2020 2020 2020 2020 2073 7263 5f63 7478           src_ctx
-000121b0: 2c20 276d 6f64 272c 2073 7263 5f63 7478  , 'mod', src_ctx
-000121c0: 5b27 6462 5f6e 616d 6527 5d2c 2073 7263  ['db_name'], src
-000121d0: 5f66 756c 6c5f 6c63 6f6e 662c 2073 7263  _full_lconf, src
-000121e0: 5f70 6174 6873 2c0a 2020 2020 2020 2020  _paths,.        
-000121f0: 2020 2020 7372 635f 6374 785b 2773 7263      src_ctx['src
-00012200: 5f6f 646f 6f5f 6676 6572 275d 290a 2020  _odoo_fver']).  
-00012210: 2020 2020 2020 6f73 302e 776c 6f67 2827        os0.wlog('
-00012220: 4d6f 6475 6c65 206c 6973 7420 746f 206d  Module list to m
-00012230: 6967 7261 7465 3d25 7327 2025 2073 7263  igrate=%s' % src
-00012240: 5f63 7478 5b27 7372 635f 6d6f 6475 6c65  _ctx['src_module
-00012250: 5f6c 6973 7427 5d29 0a20 2020 2069 6620  _list']).    if 
-00012260: 6e6f 7420 7372 635f 6374 782e 6765 7428  not src_ctx.get(
-00012270: 276f 7269 6769 6e61 6c5f 6d6f 6475 6c65  'original_module
-00012280: 5f6c 6973 7427 293a 0a20 2020 2020 2020  _list'):.       
-00012290: 2073 7263 5f63 7478 5b27 6f72 6967 696e   src_ctx['origin
-000122a0: 616c 5f6d 6f64 756c 655f 6c69 7374 275d  al_module_list']
-000122b0: 203d 2073 7263 5f63 7478 5b27 7372 635f   = src_ctx['src_
-000122c0: 6d6f 6475 6c65 5f6c 6973 7427 5d0a 2020  module_list'].  
-000122d0: 2020 7372 635f 616c 6c5f 6d6f 6475 6c65    src_all_module
-000122e0: 5f6c 6973 7420 3d20 6f64 6f6f 5f64 6570  _list = odoo_dep
-000122f0: 656e 6465 6e63 6965 7328 0a20 2020 2020  endencies(.     
-00012300: 2020 2073 7263 5f63 7478 2c20 276d 6f64     src_ctx, 'mod
-00012310: 272c 2046 616c 7365 2c20 4661 6c73 652c  ', False, False,
-00012320: 2073 7263 5f70 6174 6873 2c0a 2020 2020   src_paths,.    
-00012330: 2020 2020 7372 635f 6374 785b 2773 7263      src_ctx['src
-00012340: 5f6f 646f 6f5f 6676 6572 275d 290a 2020  _odoo_fver']).  
-00012350: 2020 7467 745f 616c 6c5f 6d6f 6475 6c65    tgt_all_module
-00012360: 5f6c 6973 7420 3d20 6f64 6f6f 5f64 6570  _list = odoo_dep
-00012370: 656e 6465 6e63 6965 7328 0a20 2020 2020  endencies(.     
-00012380: 2020 2074 6774 5f63 7478 2c20 276d 6f64     tgt_ctx, 'mod
-00012390: 272c 2046 616c 7365 2c20 4661 6c73 652c  ', False, False,
-000123a0: 2074 6774 5f70 6174 6873 2c0a 2020 2020   tgt_paths,.    
-000123b0: 2020 2020 7467 745f 6374 785b 2774 6774      tgt_ctx['tgt
-000123c0: 5f6f 646f 6f5f 6676 6572 275d 290a 2020  _odoo_fver']).  
-000123d0: 2020 7372 635f 6374 785b 2774 6e6c 5f6d    src_ctx['tnl_m
-000123e0: 6f64 756c 655f 6c69 7374 275d 2c20 6261  odule_list'], ba
-000123f0: 645f 6d6f 6475 6c65 5f6c 6973 7420 3d20  d_module_list = 
-00012400: 5c0a 2020 2020 2020 2020 646f 5f74 6e6c  \.        do_tnl
-00012410: 5f6d 6f64 756c 655f 6c69 7374 2873 7263  _module_list(src
-00012420: 5f63 7478 2c0a 2020 2020 2020 2020 2020  _ctx,.          
+000120b0: 2020 2020 7372 635f 6374 785b 2773 7263      src_ctx['src
+000120c0: 5f76 6964 275d 203d 3d20 7372 635f 6374  _vid'] == src_ct
+000120d0: 785b 2766 726f 6d5f 6272 616e 6368 275d  x['from_branch']
+000120e0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+000120f0: 2020 2066 6f72 206d 6f64 756c 6520 696e     for module in
+00012100: 2073 7263 5f63 7478 5b27 756e 696e 7374   src_ctx['uninst
+00012110: 616c 6c5f 6d6f 6475 6c65 7327 5d2e 7370  all_modules'].sp
+00012120: 6c69 7428 272c 2729 3a0a 2020 2020 2020  lit(','):.      
+00012130: 2020 2020 2020 2020 2020 2020 2020 6472                dr
+00012140: 6f70 5f6d 6f64 756c 6528 7372 635f 6374  op_module(src_ct
+00012150: 782c 206d 6f64 756c 652c 2066 6f72 6365  x, module, force
+00012160: 3d54 7275 6529 0a20 2020 2020 2020 2073  =True).        s
+00012170: 7263 5f63 7478 5b27 7372 635f 6d6f 6475  rc_ctx['src_modu
+00012180: 6c65 5f6c 6973 7427 5d20 3d20 6f64 6f6f  le_list'] = odoo
+00012190: 5f64 6570 656e 6465 6e63 6965 7328 0a20  _dependencies(. 
+000121a0: 2020 2020 2020 2020 2020 2073 7263 5f63             src_c
+000121b0: 7478 2c20 276d 6f64 272c 2073 7263 5f63  tx, 'mod', src_c
+000121c0: 7478 5b27 6462 5f6e 616d 6527 5d2c 2073  tx['db_name'], s
+000121d0: 7263 5f66 756c 6c5f 6c63 6f6e 662c 2073  rc_full_lconf, s
+000121e0: 7263 5f70 6174 6873 2c0a 2020 2020 2020  rc_paths,.      
+000121f0: 2020 2020 2020 7372 635f 6374 785b 2773        src_ctx['s
+00012200: 7263 5f6f 646f 6f5f 6676 6572 275d 290a  rc_odoo_fver']).
+00012210: 2020 2020 2020 2020 6f73 302e 776c 6f67          os0.wlog
+00012220: 2827 4d6f 6475 6c65 206c 6973 7420 746f  ('Module list to
+00012230: 206d 6967 7261 7465 3d25 7327 2025 2073   migrate=%s' % s
+00012240: 7263 5f63 7478 5b27 7372 635f 6d6f 6475  rc_ctx['src_modu
+00012250: 6c65 5f6c 6973 7427 5d29 0a20 2020 2069  le_list']).    i
+00012260: 6620 6e6f 7420 7372 635f 6374 782e 6765  f not src_ctx.ge
+00012270: 7428 276f 7269 6769 6e61 6c5f 6d6f 6475  t('original_modu
+00012280: 6c65 5f6c 6973 7427 293a 0a20 2020 2020  le_list'):.     
+00012290: 2020 2073 7263 5f63 7478 5b27 6f72 6967     src_ctx['orig
+000122a0: 696e 616c 5f6d 6f64 756c 655f 6c69 7374  inal_module_list
+000122b0: 275d 203d 2073 7263 5f63 7478 5b27 7372  '] = src_ctx['sr
+000122c0: 635f 6d6f 6475 6c65 5f6c 6973 7427 5d0a  c_module_list'].
+000122d0: 2020 2020 7372 635f 616c 6c5f 6d6f 6475      src_all_modu
+000122e0: 6c65 5f6c 6973 7420 3d20 6f64 6f6f 5f64  le_list = odoo_d
+000122f0: 6570 656e 6465 6e63 6965 7328 0a20 2020  ependencies(.   
+00012300: 2020 2020 2073 7263 5f63 7478 2c20 276d       src_ctx, 'm
+00012310: 6f64 272c 2046 616c 7365 2c20 4661 6c73  od', False, Fals
+00012320: 652c 2073 7263 5f70 6174 6873 2c0a 2020  e, src_paths,.  
+00012330: 2020 2020 2020 7372 635f 6374 785b 2773        src_ctx['s
+00012340: 7263 5f6f 646f 6f5f 6676 6572 275d 290a  rc_odoo_fver']).
+00012350: 2020 2020 7467 745f 616c 6c5f 6d6f 6475      tgt_all_modu
+00012360: 6c65 5f6c 6973 7420 3d20 6f64 6f6f 5f64  le_list = odoo_d
+00012370: 6570 656e 6465 6e63 6965 7328 0a20 2020  ependencies(.   
+00012380: 2020 2020 2074 6774 5f63 7478 2c20 276d       tgt_ctx, 'm
+00012390: 6f64 272c 2046 616c 7365 2c20 4661 6c73  od', False, Fals
+000123a0: 652c 2074 6774 5f70 6174 6873 2c0a 2020  e, tgt_paths,.  
+000123b0: 2020 2020 2020 7467 745f 6374 785b 2774        tgt_ctx['t
+000123c0: 6774 5f6f 646f 6f5f 6676 6572 275d 290a  gt_odoo_fver']).
+000123d0: 2020 2020 7372 635f 6374 785b 2774 6e6c      src_ctx['tnl
+000123e0: 5f6d 6f64 756c 655f 6c69 7374 275d 2c20  _module_list'], 
+000123f0: 6261 645f 6d6f 6475 6c65 5f6c 6973 7420  bad_module_list 
+00012400: 3d20 5c0a 2020 2020 2020 2020 646f 5f74  = \.        do_t
+00012410: 6e6c 5f6d 6f64 756c 655f 6c69 7374 2873  nl_module_list(s
+00012420: 7263 5f63 7478 2c0a 2020 2020 2020 2020  rc_ctx,.        
 00012430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012440: 2073 7263 5f63 7478 5b27 7372 635f 6d6f   src_ctx['src_mo
-00012450: 6475 6c65 5f6c 6973 7427 5d2c 0a20 2020  dule_list'],.   
+00012440: 2020 2073 7263 5f63 7478 5b27 7372 635f     src_ctx['src_
+00012450: 6d6f 6475 6c65 5f6c 6973 7427 5d2c 0a20  module_list'],. 
 00012460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012470: 2020 2020 2020 2020 7372 635f 6374 785b          src_ctx[
-00012480: 2773 7263 5f6f 646f 6f5f 6676 6572 275d  'src_odoo_fver']
-00012490: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000124a0: 2020 2020 2020 2020 2020 2020 2074 6774               tgt
-000124b0: 5f63 7478 5b27 7467 745f 6f64 6f6f 5f66  _ctx['tgt_odoo_f
-000124c0: 7665 7227 5d2c 0a20 2020 2020 2020 2020  ver'],.         
+00012470: 2020 2020 2020 2020 2020 7372 635f 6374            src_ct
+00012480: 785b 2773 7263 5f6f 646f 6f5f 6676 6572  x['src_odoo_fver
+00012490: 275d 2c0a 2020 2020 2020 2020 2020 2020  '],.            
+000124a0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+000124b0: 6774 5f63 7478 5b27 7467 745f 6f64 6f6f  gt_ctx['tgt_odoo
+000124c0: 5f66 7665 7227 5d2c 0a20 2020 2020 2020  _fver'],.       
 000124d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000124e0: 2020 7467 745f 616c 6c5f 6d6f 6475 6c65    tgt_all_module
-000124f0: 5f6c 6973 742c 0a20 2020 2020 2020 2020  _list,.         
+000124e0: 2020 2020 7467 745f 616c 6c5f 6d6f 6475      tgt_all_modu
+000124f0: 6c65 5f6c 6973 742c 0a20 2020 2020 2020  le_list,.       
 00012500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012510: 2020 7075 7265 3d54 7275 6529 0a20 2020    pure=True).   
-00012520: 206f 7330 2e77 6c6f 6728 0a20 2020 2020   os0.wlog(.     
-00012530: 2020 2027 5472 616e 736c 6174 6564 206c     'Translated l
-00012540: 6973 7420 6166 7465 7220 6d69 6772 6174  ist after migrat
-00012550: 696f 6e3d 2573 2720 2520 7372 635f 6374  ion=%s' % src_ct
-00012560: 785b 2774 6e6c 5f6d 6f64 756c 655f 6c69  x['tnl_module_li
-00012570: 7374 275d 290a 2020 2020 6675 6c6c 5f74  st']).    full_t
-00012580: 6e6c 5f6d 6f64 756c 655f 6c69 7374 203d  nl_module_list =
-00012590: 206f 646f 6f5f 6465 7065 6e64 656e 6369   odoo_dependenci
-000125a0: 6573 280a 2020 2020 2020 2020 7467 745f  es(.        tgt_
-000125b0: 6374 782c 2027 6465 7027 2c20 4661 6c73  ctx, 'dep', Fals
-000125c0: 652c 2046 616c 7365 2c20 7467 745f 7061  e, False, tgt_pa
-000125d0: 7468 732c 0a20 2020 2020 2020 2074 6774  ths,.        tgt
-000125e0: 5f63 7478 5b27 7372 635f 6f64 6f6f 5f66  _ctx['src_odoo_f
-000125f0: 7665 7227 5d2c 206d 6174 6368 6573 3d73  ver'], matches=s
-00012600: 7263 5f63 7478 5b27 746e 6c5f 6d6f 6475  rc_ctx['tnl_modu
-00012610: 6c65 5f6c 6973 7427 5d29 0a20 2020 206f  le_list']).    o
-00012620: 7330 2e77 6c6f 6728 0a20 2020 2020 2020  s0.wlog(.       
-00012630: 2027 5461 7267 6574 206c 6973 7420 7769   'Target list wi
-00012640: 7468 2064 6570 656e 6465 6e63 6965 733d  th dependencies=
-00012650: 2573 2720 2520 6675 6c6c 5f74 6e6c 5f6d  %s' % full_tnl_m
-00012660: 6f64 756c 655f 6c69 7374 290a 2020 2020  odule_list).    
-00012670: 6f73 302e 776c 6f67 280a 2020 2020 2020  os0.wlog(.      
-00012680: 2020 274e 6f74 2061 7661 6961 626c 6520    'Not avaiable 
-00012690: 6d6f 6475 6c65 7320 6f6e 2074 6172 6765  modules on targe
-000126a0: 743d 2573 2720 2520 6261 645f 6d6f 6475  t=%s' % bad_modu
-000126b0: 6c65 5f6c 6973 7429 0a20 2020 2069 6620  le_list).    if 
-000126c0: 2862 6164 5f6d 6f64 756c 655f 6c69 7374  (bad_module_list
-000126d0: 2061 6e64 0a20 2020 2020 2020 2020 2020   and.           
-000126e0: 2073 7263 5f63 7478 5b27 7265 6475 6374   src_ctx['reduct
-000126f0: 6564 5f6d 6f64 756c 655f 7365 7427 5d20  ed_module_set'] 
-00012700: 616e 640a 2020 2020 2020 2020 2020 2020  and.            
-00012710: 6e6f 7420 7372 635f 6374 785b 2764 7279  not src_ctx['dry
-00012720: 5f72 756e 275d 293a 0a20 2020 2020 2020  _run']):.       
-00012730: 2066 6f72 2069 2c6d 6f64 756c 6520 696e   for i,module in
-00012740: 2065 6e75 6d65 7261 7465 2862 6164 5f6d   enumerate(bad_m
-00012750: 6f64 756c 655f 6c69 7374 293a 0a20 2020  odule_list):.   
-00012760: 2020 2020 2020 2020 2073 7473 203d 2064           sts = d
-00012770: 726f 705f 6d6f 6475 6c65 2873 7263 5f63  rop_module(src_c
-00012780: 7478 2c20 6d6f 6475 6c65 290a 2020 2020  tx, module).    
-00012790: 2020 2020 2020 2020 6966 2073 7473 3a0a          if sts:.
-000127a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000127b0: 6465 6c20 6261 645f 6d6f 6475 6c65 5f6c  del bad_module_l
-000127c0: 6973 745b 695d 0a20 2020 2073 6f66 745f  ist[i].    soft_
-000127d0: 756e 696e 7374 616c 6c5f 6c69 7374 203d  uninstall_list =
-000127e0: 2068 6172 645f 756e 696e 7374 616c 6c5f   hard_uninstall_
-000127f0: 6c69 7374 203d 205b 5d0a 2020 2020 6966  list = [].    if
-00012800: 2074 6774 5f63 7478 5b27 6f63 615f 6d69   tgt_ctx['oca_mi
-00012810: 6772 6174 6527 5d20 616e 6420 7467 745f  grate'] and tgt_
-00012820: 6374 785b 2774 6774 5f6f 646f 6f5f 7665  ctx['tgt_odoo_ve
-00012830: 7227 5d20 3c20 3130 3a0a 2020 2020 2020  r'] < 10:.      
-00012840: 2020 6f75 5f76 6572 5f70 6174 6820 3d20    ou_ver_path = 
-00012850: 6c6f 6164 5f6f 7065 6e75 7067 7261 6465  load_openupgrade
-00012860: 2874 6774 5f63 7478 2c20 7467 745f 6374  (tgt_ctx, tgt_ct
-00012870: 785b 2774 6774 5f6f 646f 6f5f 6676 6572  x['tgt_odoo_fver
-00012880: 275d 290a 2020 2020 2020 2020 636d 6420  ']).        cmd 
-00012890: 3d20 6f73 2e70 6174 682e 6a6f 696e 286f  = os.path.join(o
-000128a0: 755f 7665 725f 7061 7468 2c20 2773 6372  u_ver_path, 'scr
-000128b0: 6970 7473 272c 2027 6d69 6772 6174 652e  ipts', 'migrate.
-000128c0: 7079 2729 0a20 2020 2020 2020 2069 6620  py').        if 
-000128d0: 7372 635f 6374 785b 276e 6f5f 7665 6e76  src_ctx['no_venv
-000128e0: 275d 3a0a 2020 2020 2020 2020 2020 2020  ']:.            
-000128f0: 7275 6e5f 7472 6163 6564 2863 6d64 2c0a  run_traced(cmd,.
-00012900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012910: 2020 2020 2020 2027 2d43 272c 2073 7263         '-C', src
-00012920: 5f66 756c 6c5f 6c63 6f6e 662c 0a20 2020  _full_lconf,.   
+00012510: 2020 2020 7075 7265 3d54 7275 6529 0a20      pure=True). 
+00012520: 2020 206f 7330 2e77 6c6f 6728 0a20 2020     os0.wlog(.   
+00012530: 2020 2020 2027 5472 616e 736c 6174 6564       'Translated
+00012540: 206c 6973 7420 6166 7465 7220 6d69 6772   list after migr
+00012550: 6174 696f 6e3d 2573 2720 2520 7372 635f  ation=%s' % src_
+00012560: 6374 785b 2774 6e6c 5f6d 6f64 756c 655f  ctx['tnl_module_
+00012570: 6c69 7374 275d 290a 2020 2020 6675 6c6c  list']).    full
+00012580: 5f74 6e6c 5f6d 6f64 756c 655f 6c69 7374  _tnl_module_list
+00012590: 203d 206f 646f 6f5f 6465 7065 6e64 656e   = odoo_dependen
+000125a0: 6369 6573 280a 2020 2020 2020 2020 7467  cies(.        tg
+000125b0: 745f 6374 782c 2027 6465 7027 2c20 4661  t_ctx, 'dep', Fa
+000125c0: 6c73 652c 2046 616c 7365 2c20 7467 745f  lse, False, tgt_
+000125d0: 7061 7468 732c 0a20 2020 2020 2020 2074  paths,.        t
+000125e0: 6774 5f63 7478 5b27 7372 635f 6f64 6f6f  gt_ctx['src_odoo
+000125f0: 5f66 7665 7227 5d2c 206d 6174 6368 6573  _fver'], matches
+00012600: 3d73 7263 5f63 7478 5b27 746e 6c5f 6d6f  =src_ctx['tnl_mo
+00012610: 6475 6c65 5f6c 6973 7427 5d29 0a20 2020  dule_list']).   
+00012620: 206f 7330 2e77 6c6f 6728 0a20 2020 2020   os0.wlog(.     
+00012630: 2020 2027 5461 7267 6574 206c 6973 7420     'Target list 
+00012640: 7769 7468 2064 6570 656e 6465 6e63 6965  with dependencie
+00012650: 733d 2573 2720 2520 6675 6c6c 5f74 6e6c  s=%s' % full_tnl
+00012660: 5f6d 6f64 756c 655f 6c69 7374 290a 2020  _module_list).  
+00012670: 2020 6f73 302e 776c 6f67 280a 2020 2020    os0.wlog(.    
+00012680: 2020 2020 274e 6f74 2061 7661 6961 626c      'Not avaiabl
+00012690: 6520 6d6f 6475 6c65 7320 6f6e 2074 6172  e modules on tar
+000126a0: 6765 743d 2573 2720 2520 6261 645f 6d6f  get=%s' % bad_mo
+000126b0: 6475 6c65 5f6c 6973 7429 0a20 2020 2069  dule_list).    i
+000126c0: 6620 2862 6164 5f6d 6f64 756c 655f 6c69  f (bad_module_li
+000126d0: 7374 2061 6e64 0a20 2020 2020 2020 2020  st and.         
+000126e0: 2020 2073 7263 5f63 7478 5b27 7265 6475     src_ctx['redu
+000126f0: 6374 6564 5f6d 6f64 756c 655f 7365 7427  cted_module_set'
+00012700: 5d20 616e 640a 2020 2020 2020 2020 2020  ] and.          
+00012710: 2020 6e6f 7420 7372 635f 6374 785b 2764    not src_ctx['d
+00012720: 7279 5f72 756e 275d 293a 0a20 2020 2020  ry_run']):.     
+00012730: 2020 2066 6f72 2069 2c6d 6f64 756c 6520     for i,module 
+00012740: 696e 2065 6e75 6d65 7261 7465 2862 6164  in enumerate(bad
+00012750: 5f6d 6f64 756c 655f 6c69 7374 293a 0a20  _module_list):. 
+00012760: 2020 2020 2020 2020 2020 2073 7473 203d             sts =
+00012770: 2064 726f 705f 6d6f 6475 6c65 2873 7263   drop_module(src
+00012780: 5f63 7478 2c20 6d6f 6475 6c65 290a 2020  _ctx, module).  
+00012790: 2020 2020 2020 2020 2020 6966 2073 7473            if sts
+000127a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000127b0: 2020 6465 6c20 6261 645f 6d6f 6475 6c65    del bad_module
+000127c0: 5f6c 6973 745b 695d 0a20 2020 2073 6f66  _list[i].    sof
+000127d0: 745f 756e 696e 7374 616c 6c5f 6c69 7374  t_uninstall_list
+000127e0: 203d 2068 6172 645f 756e 696e 7374 616c   = hard_uninstal
+000127f0: 6c5f 6c69 7374 203d 205b 5d0a 2020 2020  l_list = [].    
+00012800: 6966 2074 6774 5f63 7478 5b27 6f63 615f  if tgt_ctx['oca_
+00012810: 6d69 6772 6174 6527 5d20 616e 6420 7467  migrate'] and tg
+00012820: 745f 6374 785b 2774 6774 5f6f 646f 6f5f  t_ctx['tgt_odoo_
+00012830: 7665 7227 5d20 3c20 3130 3a0a 2020 2020  ver'] < 10:.    
+00012840: 2020 2020 6f75 5f76 6572 5f70 6174 6820      ou_ver_path 
+00012850: 3d20 6c6f 6164 5f6f 7065 6e75 7067 7261  = load_openupgra
+00012860: 6465 2874 6774 5f63 7478 2c20 7467 745f  de(tgt_ctx, tgt_
+00012870: 6374 785b 2774 6774 5f6f 646f 6f5f 6676  ctx['tgt_odoo_fv
+00012880: 6572 275d 290a 2020 2020 2020 2020 636d  er']).        cm
+00012890: 6420 3d20 6f73 2e70 6174 682e 6a6f 696e  d = os.path.join
+000128a0: 286f 755f 7665 725f 7061 7468 2c20 2773  (ou_ver_path, 's
+000128b0: 6372 6970 7473 272c 2027 6d69 6772 6174  cripts', 'migrat
+000128c0: 652e 7079 2729 0a20 2020 2020 2020 2069  e.py').        i
+000128d0: 6620 7372 635f 6374 785b 276e 6f5f 7665  f src_ctx['no_ve
+000128e0: 6e76 275d 3a0a 2020 2020 2020 2020 2020  nv']:.          
+000128f0: 2020 7275 6e5f 7472 6163 6564 2863 6d64    run_traced(cmd
+00012900: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00012910: 2020 2020 2020 2020 2027 2d43 272c 2073           '-C', s
+00012920: 7263 5f66 756c 6c5f 6c63 6f6e 662c 0a20  rc_full_lconf,. 
 00012930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012940: 2020 2020 272d 4427 2c20 7372 635f 6374      '-D', src_ct
-00012950: 785b 2764 625f 6e61 6d65 275d 2c0a 2020  x['db_name'],.  
+00012940: 2020 2020 2020 272d 4427 2c20 7372 635f        '-D', src_
+00012950: 6374 785b 2764 625f 6e61 6d65 275d 2c0a  ctx['db_name'],.
 00012960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012970: 2020 2020 2027 2d42 272c 2073 7263 5f63       '-B', src_c
-00012980: 7478 5b27 6f70 745f 6f75 7061 7468 275d  tx['opt_oupath']
-00012990: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000129a0: 2020 2020 2020 2020 2027 2d52 272c 2074           '-R', t
-000129b0: 6774 5f63 7478 5b27 7467 745f 6f64 6f6f  gt_ctx['tgt_odoo
-000129c0: 5f66 7665 7227 5d29 0a20 2020 2020 2020  _fver']).       
-000129d0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-000129e0: 2020 2073 6372 6970 7420 3d20 6f73 2e70     script = os.p
-000129f0: 6174 682e 6a6f 696e 286f 755f 7665 725f  ath.join(ou_ver_
-00012a00: 7061 7468 2c20 276d 6967 7261 7465 2e73  path, 'migrate.s
-00012a10: 6827 290a 2020 2020 2020 2020 2020 2020  h').            
-00012a20: 6664 203d 206f 7065 6e28 7363 7269 7074  fd = open(script
-00012a30: 2c20 2777 2729 0a20 2020 2020 2020 2020  , 'w').         
-00012a40: 2020 2066 642e 7772 6974 6528 2763 6420     fd.write('cd 
-00012a50: 2573 5c6e 2720 2520 7467 745f 6374 785b  %s\n' % tgt_ctx[
-00012a60: 2776 656e 765f 6f75 7061 7468 275d 290a  'venv_oupath']).
-00012a70: 2020 2020 2020 2020 2020 2020 6664 2e77              fd.w
-00012a80: 7269 7465 2827 736f 7572 6365 202e 2f62  rite('source ./b
-00012a90: 696e 2f61 6374 6976 6174 655c 6e27 290a  in/activate\n').
-00012aa0: 2020 2020 2020 2020 2020 2020 6664 2e77              fd.w
-00012ab0: 7269 7465 2827 2573 202d 4320 2573 202d  rite('%s -C %s -
-00012ac0: 4420 2573 202d 4220 2573 202d 5220 2573  D %s -B %s -R %s
-00012ad0: 5c6e 2720 2520 280a 2020 2020 2020 2020  \n' % (.        
-00012ae0: 2020 2020 2020 2020 636d 642c 2073 7263          cmd, src
-00012af0: 5f66 756c 6c5f 6c63 6f6e 662c 0a20 2020  _full_lconf,.   
-00012b00: 2020 2020 2020 2020 2020 2020 2073 7263               src
-00012b10: 5f63 7478 5b27 6462 5f6e 616d 6527 5d2c  _ctx['db_name'],
-00012b20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012b30: 2073 7263 5f63 7478 5b27 6f70 745f 6f75   src_ctx['opt_ou
-00012b40: 7061 7468 275d 2c0a 2020 2020 2020 2020  path'],.        
-00012b50: 2020 2020 2020 2020 7467 745f 6374 785b          tgt_ctx[
-00012b60: 2774 6774 5f6f 646f 6f5f 6676 6572 275d  'tgt_odoo_fver']
-00012b70: 2929 0a20 2020 2020 2020 2020 2020 2066  )).            f
-00012b80: 642e 7772 6974 6528 2764 6561 6374 6976  d.write('deactiv
-00012b90: 6174 655c 6e27 290a 2020 2020 2020 2020  ate\n').        
-00012ba0: 2020 2020 6664 2e63 6c6f 7365 2829 0a20      fd.close(). 
-00012bb0: 2020 2020 2020 2020 2020 206f 732e 6368             os.ch
-00012bc0: 6d6f 6428 7363 7269 7074 2c20 306f 3734  mod(script, 0o74
-00012bd0: 3429 0a20 2020 2020 2020 2020 2020 2069  4).            i
-00012be0: 6620 6e6f 7420 7372 635f 6374 785b 2764  f not src_ctx['d
-00012bf0: 7279 5f72 756e 275d 3a0a 2020 2020 2020  ry_run']:.      
-00012c00: 2020 2020 2020 2020 2020 6f73 2e73 7973            os.sys
-00012c10: 7465 6d28 7363 7269 7074 290a 2020 2020  tem(script).    
-00012c20: 2020 2020 6966 206e 6f74 2073 7263 5f63      if not src_c
-00012c30: 7478 5b27 6472 795f 7275 6e27 5d3a 0a20  tx['dry_run']:. 
-00012c40: 2020 2020 2020 2020 2020 2074 696d 652e             time.
-00012c50: 736c 6565 7028 3529 0a20 2020 2020 2020  sleep(5).       
-00012c60: 2074 6d70 5f64 626e 616d 6520 3d20 6e65   tmp_dbname = ne
-00012c70: 775f 6462 6e61 6d65 2873 7263 5f63 7478  w_dbname(src_ctx
-00012c80: 5b27 6462 5f6e 616d 6527 5d2c 0a20 2020  ['db_name'],.   
+00012970: 2020 2020 2020 2027 2d42 272c 2073 7263         '-B', src
+00012980: 5f63 7478 5b27 6f70 745f 6f75 7061 7468  _ctx['opt_oupath
+00012990: 275d 2c0a 2020 2020 2020 2020 2020 2020  '],.            
+000129a0: 2020 2020 2020 2020 2020 2027 2d52 272c             '-R',
+000129b0: 2074 6774 5f63 7478 5b27 7467 745f 6f64   tgt_ctx['tgt_od
+000129c0: 6f6f 5f66 7665 7227 5d29 0a20 2020 2020  oo_fver']).     
+000129d0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+000129e0: 2020 2020 2073 6372 6970 7420 3d20 6f73       script = os
+000129f0: 2e70 6174 682e 6a6f 696e 286f 755f 7665  .path.join(ou_ve
+00012a00: 725f 7061 7468 2c20 276d 6967 7261 7465  r_path, 'migrate
+00012a10: 2e73 6827 290a 2020 2020 2020 2020 2020  .sh').          
+00012a20: 2020 6664 203d 206f 7065 6e28 7363 7269    fd = open(scri
+00012a30: 7074 2c20 2777 2729 0a20 2020 2020 2020  pt, 'w').       
+00012a40: 2020 2020 2066 642e 7772 6974 6528 2763       fd.write('c
+00012a50: 6420 2573 5c6e 2720 2520 7467 745f 6374  d %s\n' % tgt_ct
+00012a60: 785b 2776 656e 765f 6f75 7061 7468 275d  x['venv_oupath']
+00012a70: 290a 2020 2020 2020 2020 2020 2020 6664  ).            fd
+00012a80: 2e77 7269 7465 2827 736f 7572 6365 202e  .write('source .
+00012a90: 2f62 696e 2f61 6374 6976 6174 655c 6e27  /bin/activate\n'
+00012aa0: 290a 2020 2020 2020 2020 2020 2020 6664  ).            fd
+00012ab0: 2e77 7269 7465 2827 2573 202d 4320 2573  .write('%s -C %s
+00012ac0: 202d 4420 2573 202d 4220 2573 202d 5220   -D %s -B %s -R 
+00012ad0: 2573 5c6e 2720 2520 280a 2020 2020 2020  %s\n' % (.      
+00012ae0: 2020 2020 2020 2020 2020 636d 642c 2073            cmd, s
+00012af0: 7263 5f66 756c 6c5f 6c63 6f6e 662c 0a20  rc_full_lconf,. 
+00012b00: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00012b10: 7263 5f63 7478 5b27 6462 5f6e 616d 6527  rc_ctx['db_name'
+00012b20: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+00012b30: 2020 2073 7263 5f63 7478 5b27 6f70 745f     src_ctx['opt_
+00012b40: 6f75 7061 7468 275d 2c0a 2020 2020 2020  oupath'],.      
+00012b50: 2020 2020 2020 2020 2020 7467 745f 6374            tgt_ct
+00012b60: 785b 2774 6774 5f6f 646f 6f5f 6676 6572  x['tgt_odoo_fver
+00012b70: 275d 2929 0a20 2020 2020 2020 2020 2020  '])).           
+00012b80: 2066 642e 7772 6974 6528 2764 6561 6374   fd.write('deact
+00012b90: 6976 6174 655c 6e27 290a 2020 2020 2020  ivate\n').      
+00012ba0: 2020 2020 2020 6664 2e63 6c6f 7365 2829        fd.close()
+00012bb0: 0a20 2020 2020 2020 2020 2020 206f 732e  .            os.
+00012bc0: 6368 6d6f 6428 7363 7269 7074 2c20 306f  chmod(script, 0o
+00012bd0: 3734 3429 0a20 2020 2020 2020 2020 2020  744).           
+00012be0: 2069 6620 6e6f 7420 7372 635f 6374 785b   if not src_ctx[
+00012bf0: 2764 7279 5f72 756e 275d 3a0a 2020 2020  'dry_run']:.    
+00012c00: 2020 2020 2020 2020 2020 2020 6f73 2e73              os.s
+00012c10: 7973 7465 6d28 7363 7269 7074 290a 2020  ystem(script).  
+00012c20: 2020 2020 2020 6966 206e 6f74 2073 7263        if not src
+00012c30: 5f63 7478 5b27 6472 795f 7275 6e27 5d3a  _ctx['dry_run']:
+00012c40: 0a20 2020 2020 2020 2020 2020 2074 696d  .            tim
+00012c50: 652e 736c 6565 7028 3529 0a20 2020 2020  e.sleep(5).     
+00012c60: 2020 2074 6d70 5f64 626e 616d 6520 3d20     tmp_dbname = 
+00012c70: 6e65 775f 6462 6e61 6d65 2873 7263 5f63  new_dbname(src_c
+00012c80: 7478 5b27 6462 5f6e 616d 6527 5d2c 0a20  tx['db_name'],. 
 00012c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ca0: 2020 2020 2020 2020 2020 2020 2074 6774               tgt
-00012cb0: 5f63 7478 5b27 7467 745f 6f64 6f6f 5f76  _ctx['tgt_odoo_v
-00012cc0: 6572 275d 2c0a 2020 2020 2020 2020 2020  er'],.          
+00012ca0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00012cb0: 6774 5f63 7478 5b27 7467 745f 6f64 6f6f  gt_ctx['tgt_odoo
+00012cc0: 5f76 6572 275d 2c0a 2020 2020 2020 2020  _ver'],.        
 00012cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ce0: 2020 2020 2020 7467 745f 6374 785b 276f        tgt_ctx['o
-00012cf0: 6361 5f6d 6967 7261 7465 275d 290a 2020  ca_migrate']).  
-00012d00: 2020 2020 2020 6966 206e 6f74 2073 7263        if not src
-00012d10: 5f63 7478 5b27 6472 795f 7275 6e27 5d3a  _ctx['dry_run']:
-00012d20: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00012d30: 7467 745f 6374 785b 2764 625f 6e61 6d65  tgt_ctx['db_name
-00012d40: 275d 2021 3d20 746d 705f 6462 6e61 6d65  '] != tmp_dbname
-00012d50: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00012d60: 2020 7265 6e5f 6462 2874 6d70 5f64 626e    ren_db(tmp_dbn
-00012d70: 616d 652c 2074 6774 5f63 7478 5b27 6462  ame, tgt_ctx['db
-00012d80: 5f6e 616d 6527 5d2c 2073 7263 5f63 7478  _name'], src_ctx
-00012d90: 5b27 6462 5f75 7365 7227 5d29 0a20 2020  ['db_user']).   
-00012da0: 2020 2020 2020 2020 2069 6620 7372 635f           if src_
-00012db0: 6374 785b 2764 625f 7573 6572 275d 2021  ctx['db_user'] !
-00012dc0: 3d20 7467 745f 6374 785b 2764 625f 7573  = tgt_ctx['db_us
-00012dd0: 6572 275d 3a0a 2020 2020 2020 2020 2020  er']:.          
-00012de0: 2020 2020 2020 7265 6173 7369 676e 5f64        reassign_d
-00012df0: 625f 6f77 6e65 7228 7467 745f 6374 782c  b_owner(tgt_ctx,
-00012e00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012ce0: 2020 2020 2020 2020 7467 745f 6374 785b          tgt_ctx[
+00012cf0: 276f 6361 5f6d 6967 7261 7465 275d 290a  'oca_migrate']).
+00012d00: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
+00012d10: 7263 5f63 7478 5b27 6472 795f 7275 6e27  rc_ctx['dry_run'
+00012d20: 5d3a 0a20 2020 2020 2020 2020 2020 2069  ]:.            i
+00012d30: 6620 7467 745f 6374 785b 2764 625f 6e61  f tgt_ctx['db_na
+00012d40: 6d65 275d 2021 3d20 746d 705f 6462 6e61  me'] != tmp_dbna
+00012d50: 6d65 3a0a 2020 2020 2020 2020 2020 2020  me:.            
+00012d60: 2020 2020 7265 6e5f 6462 2874 6d70 5f64      ren_db(tmp_d
+00012d70: 626e 616d 652c 2074 6774 5f63 7478 5b27  bname, tgt_ctx['
+00012d80: 6462 5f6e 616d 6527 5d2c 2073 7263 5f63  db_name'], src_c
+00012d90: 7478 5b27 6462 5f75 7365 7227 5d29 0a20  tx['db_user']). 
+00012da0: 2020 2020 2020 2020 2020 2069 6620 7372             if sr
+00012db0: 635f 6374 785b 2764 625f 7573 6572 275d  c_ctx['db_user']
+00012dc0: 2021 3d20 7467 745f 6374 785b 2764 625f   != tgt_ctx['db_
+00012dd0: 7573 6572 275d 3a0a 2020 2020 2020 2020  user']:.        
+00012de0: 2020 2020 2020 2020 7265 6173 7369 676e          reassign
+00012df0: 5f64 625f 6f77 6e65 7228 7467 745f 6374  _db_owner(tgt_ct
+00012e00: 782c 0a20 2020 2020 2020 2020 2020 2020  x,.             
 00012e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012e20: 2020 2074 6774 5f63 7478 5b27 6462 5f6e     tgt_ctx['db_n
-00012e30: 616d 6527 5d2c 0a20 2020 2020 2020 2020  ame'],.         
+00012e20: 2020 2020 2074 6774 5f63 7478 5b27 6462       tgt_ctx['db
+00012e30: 5f6e 616d 6527 5d2c 0a20 2020 2020 2020  _name'],.       
 00012e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012e50: 2020 2020 2020 2020 2073 7263 5f63 7478           src_ctx
-00012e60: 5b27 6462 5f75 7365 7227 5d2c 0a20 2020  ['db_user'],.   
+00012e50: 2020 2020 2020 2020 2020 2073 7263 5f63             src_c
+00012e60: 7478 5b27 6462 5f75 7365 7227 5d2c 0a20  tx['db_user'],. 
 00012e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012e80: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00012e90: 6774 5f63 7478 5b27 6462 5f75 7365 7227  gt_ctx['db_user'
-00012ea0: 5d29 0a20 2020 2020 2020 2074 6774 5f66  ]).        tgt_f
-00012eb0: 756c 6c5f 6c63 6f6e 6620 3d20 7467 745f  ull_lconf = tgt_
-00012ec0: 6374 785b 2763 6f6e 665f 666e 275d 0a20  ctx['conf_fn']. 
-00012ed0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00012ee0: 206f 755f 7665 725f 7061 7468 203d 206c   ou_ver_path = l
-00012ef0: 6f61 645f 6f70 656e 7570 6772 6164 6528  oad_openupgrade(
-00012f00: 7467 745f 6374 782c 2074 6774 5f63 7478  tgt_ctx, tgt_ctx
-00012f10: 5b27 7467 745f 6f64 6f6f 5f66 7665 7227  ['tgt_odoo_fver'
-00012f20: 5d29 0a20 2020 2020 2020 2069 6620 6e6f  ]).        if no
-00012f30: 7420 7372 635f 6374 785b 2764 7279 5f72  t src_ctx['dry_r
-00012f40: 756e 275d 3a0a 2020 2020 2020 2020 2020  un']:.          
-00012f50: 2020 6c6f 6164 5f6f 7065 6e75 7067 7261    load_openupgra
-00012f60: 6465 6c69 6228 7372 635f 6374 782c 2074  delib(src_ctx, t
-00012f70: 6774 5f63 7478 5b27 7467 745f 6f64 6f6f  gt_ctx['tgt_odoo
-00012f80: 5f66 7665 7227 5d29 0a20 2020 2020 2020  _fver']).       
-00012f90: 2069 6620 7467 745f 6374 785b 2775 7064   if tgt_ctx['upd
-00012fa0: 5f74 7261 6e73 6c61 7469 6f6e 275d 3a0a  _translation']:.
-00012fb0: 2020 2020 2020 2020 2020 2020 6164 645f              add_
-00012fc0: 7665 7273 696f 6e65 645f 746e 6c28 7372  versioned_tnl(sr
-00012fd0: 635f 6374 782c 2073 7263 5f63 7478 5b27  c_ctx, src_ctx['
-00012fe0: 7372 635f 6f64 6f6f 5f66 7665 7227 5d2c  src_odoo_fver'],
-00012ff0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013000: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00013010: 6774 5f63 7478 5b27 7467 745f 6f64 6f6f  gt_ctx['tgt_odoo
-00013020: 5f66 7665 7227 5d29 0a20 2020 2020 2020  _fver']).       
-00013030: 2061 6464 6f6e 735f 7061 7468 203d 206f   addons_path = o
-00013040: 732e 7061 7468 2e6a 6f69 6e28 6f75 5f76  s.path.join(ou_v
-00013050: 6572 5f70 6174 682c 2027 6164 646f 6e73  er_path, 'addons
-00013060: 2729 0a20 2020 2020 2020 2069 6620 7467  ').        if tg
-00013070: 745f 6374 785b 2774 6774 5f6f 646f 6f5f  t_ctx['tgt_odoo_
-00013080: 7665 7227 5d20 3c20 3130 3a0a 2020 2020  ver'] < 10:.    
-00013090: 2020 2020 2020 2020 726f 6f74 5f70 6174          root_pat
-000130a0: 6820 3d20 6f73 2e70 6174 682e 6a6f 696e  h = os.path.join
-000130b0: 286f 755f 7665 725f 7061 7468 2c20 276f  (ou_ver_path, 'o
-000130c0: 7065 6e65 7270 272c 2027 6164 646f 6e73  penerp', 'addons
-000130d0: 2729 0a20 2020 2020 2020 2065 6c73 653a  ').        else:
-000130e0: 0a20 2020 2020 2020 2020 2020 2072 6f6f  .            roo
-000130f0: 745f 7061 7468 203d 206f 732e 7061 7468  t_path = os.path
-00013100: 2e6a 6f69 6e28 6f75 5f76 6572 5f70 6174  .join(ou_ver_pat
-00013110: 682c 2027 6f64 6f6f 272c 2027 6164 646f  h, 'odoo', 'addo
-00013120: 6e73 2729 0a20 2020 2020 2020 2069 6620  ns').        if 
-00013130: 6e6f 7420 7372 635f 6374 785b 2764 7279  not src_ctx['dry
-00013140: 5f72 756e 275d 3a0a 2020 2020 2020 2020  _run']:.        
-00013150: 2020 2020 666f 7220 7265 706f 2069 6e20      for repo in 
-00013160: 7467 745f 7061 7468 733a 0a20 2020 2020  tgt_paths:.     
-00013170: 2020 2020 2020 2020 2020 2066 6f72 206e             for n
-00013180: 616d 6520 696e 206f 732e 6c69 7374 6469  ame in os.listdi
-00013190: 7228 7265 706f 293a 0a20 2020 2020 2020  r(repo):.       
-000131a0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-000131b0: 286f 732e 7061 7468 2e69 7364 6972 286f  (os.path.isdir(o
-000131c0: 732e 7061 7468 2e6a 6f69 6e28 7265 706f  s.path.join(repo
-000131d0: 2c20 6e61 6d65 2929 2061 6e64 0a20 2020  , name)) and.   
+00012e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012e90: 2074 6774 5f63 7478 5b27 6462 5f75 7365   tgt_ctx['db_use
+00012ea0: 7227 5d29 0a20 2020 2020 2020 2074 6774  r']).        tgt
+00012eb0: 5f66 756c 6c5f 6c63 6f6e 6620 3d20 7467  _full_lconf = tg
+00012ec0: 745f 6374 785b 2763 6f6e 665f 666e 275d  t_ctx['conf_fn']
+00012ed0: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
+00012ee0: 2020 206f 755f 7665 725f 7061 7468 203d     ou_ver_path =
+00012ef0: 206c 6f61 645f 6f70 656e 7570 6772 6164   load_openupgrad
+00012f00: 6528 7467 745f 6374 782c 2074 6774 5f63  e(tgt_ctx, tgt_c
+00012f10: 7478 5b27 7467 745f 6f64 6f6f 5f66 7665  tx['tgt_odoo_fve
+00012f20: 7227 5d29 0a20 2020 2020 2020 2069 6620  r']).        if 
+00012f30: 6e6f 7420 7372 635f 6374 785b 2764 7279  not src_ctx['dry
+00012f40: 5f72 756e 275d 3a0a 2020 2020 2020 2020  _run']:.        
+00012f50: 2020 2020 6c6f 6164 5f6f 7065 6e75 7067      load_openupg
+00012f60: 7261 6465 6c69 6228 7372 635f 6374 782c  radelib(src_ctx,
+00012f70: 2074 6774 5f63 7478 5b27 7467 745f 6f64   tgt_ctx['tgt_od
+00012f80: 6f6f 5f66 7665 7227 5d29 0a20 2020 2020  oo_fver']).     
+00012f90: 2020 2069 6620 7467 745f 6374 785b 2775     if tgt_ctx['u
+00012fa0: 7064 5f74 7261 6e73 6c61 7469 6f6e 275d  pd_translation']
+00012fb0: 3a0a 2020 2020 2020 2020 2020 2020 6164  :.            ad
+00012fc0: 645f 7665 7273 696f 6e65 645f 746e 6c28  d_versioned_tnl(
+00012fd0: 7372 635f 6374 782c 2073 7263 5f63 7478  src_ctx, src_ctx
+00012fe0: 5b27 7372 635f 6f64 6f6f 5f66 7665 7227  ['src_odoo_fver'
+00012ff0: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+00013000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013010: 2074 6774 5f63 7478 5b27 7467 745f 6f64   tgt_ctx['tgt_od
+00013020: 6f6f 5f66 7665 7227 5d29 0a20 2020 2020  oo_fver']).     
+00013030: 2020 2061 6464 6f6e 735f 7061 7468 203d     addons_path =
+00013040: 206f 732e 7061 7468 2e6a 6f69 6e28 6f75   os.path.join(ou
+00013050: 5f76 6572 5f70 6174 682c 2027 6164 646f  _ver_path, 'addo
+00013060: 6e73 2729 0a20 2020 2020 2020 2069 6620  ns').        if 
+00013070: 7467 745f 6374 785b 2774 6774 5f6f 646f  tgt_ctx['tgt_odo
+00013080: 6f5f 7665 7227 5d20 3c20 3130 3a0a 2020  o_ver'] < 10:.  
+00013090: 2020 2020 2020 2020 2020 726f 6f74 5f70            root_p
+000130a0: 6174 6820 3d20 6f73 2e70 6174 682e 6a6f  ath = os.path.jo
+000130b0: 696e 286f 755f 7665 725f 7061 7468 2c20  in(ou_ver_path, 
+000130c0: 276f 7065 6e65 7270 272c 2027 6164 646f  'openerp', 'addo
+000130d0: 6e73 2729 0a20 2020 2020 2020 2065 6c73  ns').        els
+000130e0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+000130f0: 6f6f 745f 7061 7468 203d 206f 732e 7061  oot_path = os.pa
+00013100: 7468 2e6a 6f69 6e28 6f75 5f76 6572 5f70  th.join(ou_ver_p
+00013110: 6174 682c 2027 6f64 6f6f 272c 2027 6164  ath, 'odoo', 'ad
+00013120: 646f 6e73 2729 0a20 2020 2020 2020 2069  dons').        i
+00013130: 6620 6e6f 7420 7372 635f 6374 785b 2764  f not src_ctx['d
+00013140: 7279 5f72 756e 275d 3a0a 2020 2020 2020  ry_run']:.      
+00013150: 2020 2020 2020 666f 7220 7265 706f 2069        for repo i
+00013160: 6e20 7467 745f 7061 7468 733a 0a20 2020  n tgt_paths:.   
+00013170: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+00013180: 206e 616d 6520 696e 206f 732e 6c69 7374   name in os.list
+00013190: 6469 7228 7265 706f 293a 0a20 2020 2020  dir(repo):.     
+000131a0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000131b0: 6620 286f 732e 7061 7468 2e69 7364 6972  f (os.path.isdir
+000131c0: 286f 732e 7061 7468 2e6a 6f69 6e28 7265  (os.path.join(re
+000131d0: 706f 2c20 6e61 6d65 2929 2061 6e64 0a20  po, name)) and. 
 000131e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000131f0: 2020 2020 2020 2020 206e 6f74 206f 732e           not os.
-00013200: 7061 7468 2e69 7364 6972 280a 2020 2020  path.isdir(.    
+000131f0: 2020 2020 2020 2020 2020 206e 6f74 206f             not o
+00013200: 732e 7061 7468 2e69 7364 6972 280a 2020  s.path.isdir(.  
 00013210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013220: 2020 2020 2020 2020 2020 2020 6f73 2e70              os.p
-00013230: 6174 682e 6a6f 696e 2861 6464 6f6e 735f  ath.join(addons_
-00013240: 7061 7468 2c20 6e61 6d65 2929 2061 6e64  path, name)) and
-00013250: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013260: 2020 2020 2020 2020 2020 2020 206e 6f74               not
-00013270: 206f 732e 7061 7468 2e69 7364 6972 286f   os.path.isdir(o
-00013280: 732e 7061 7468 2e6a 6f69 6e28 726f 6f74  s.path.join(root
-00013290: 5f70 6174 682c 206e 616d 6529 2929 3a0a  _path, name))):.
-000132a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000132b0: 2020 2020 2020 2020 6f73 2e73 796d 6c69          os.symli
-000132c0: 6e6b 286f 732e 7061 7468 2e6a 6f69 6e28  nk(os.path.join(
-000132d0: 7265 706f 2c20 6e61 6d65 292c 0a20 2020  repo, name),.   
+00013220: 2020 2020 2020 2020 2020 2020 2020 6f73                os
+00013230: 2e70 6174 682e 6a6f 696e 2861 6464 6f6e  .path.join(addon
+00013240: 735f 7061 7468 2c20 6e61 6d65 2929 2061  s_path, name)) a
+00013250: 6e64 0a20 2020 2020 2020 2020 2020 2020  nd.             
+00013260: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00013270: 6f74 206f 732e 7061 7468 2e69 7364 6972  ot os.path.isdir
+00013280: 286f 732e 7061 7468 2e6a 6f69 6e28 726f  (os.path.join(ro
+00013290: 6f74 5f70 6174 682c 206e 616d 6529 2929  ot_path, name)))
+000132a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000132b0: 2020 2020 2020 2020 2020 6f73 2e73 796d            os.sym
+000132c0: 6c69 6e6b 286f 732e 7061 7468 2e6a 6f69  link(os.path.joi
+000132d0: 6e28 7265 706f 2c20 6e61 6d65 292c 0a20  n(repo, name),. 
 000132e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000132f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013300: 6f73 2e70 6174 682e 6a6f 696e 2861 6464  os.path.join(add
-00013310: 6f6e 735f 7061 7468 2c20 6e61 6d65 2929  ons_path, name))
-00013320: 0a20 2020 2020 2020 2074 6774 5f70 6174  .        tgt_pat
-00013330: 6873 203d 205b 5d0a 2020 2020 2020 2020  hs = [].        
-00013340: 7467 745f 7061 7468 732e 696e 7365 7274  tgt_paths.insert
-00013350: 2830 2c20 6164 646f 6e73 5f70 6174 6829  (0, addons_path)
-00013360: 0a20 2020 2020 2020 2074 6774 5f70 6174  .        tgt_pat
-00013370: 6873 2e69 6e73 6572 7428 302c 2072 6f6f  hs.insert(0, roo
-00013380: 745f 7061 7468 290a 2020 2020 2020 2020  t_path).        
-00013390: 7467 745f 6675 6c6c 5f6c 636f 6e66 203d  tgt_full_lconf =
-000133a0: 2070 7265 7061 7265 5f63 6f6e 6669 675f   prepare_config_
-000133b0: 6669 6c65 2874 6774 5f63 7478 2c20 7467  file(tgt_ctx, tg
-000133c0: 745f 636f 6e66 6967 2c0a 2020 2020 2020  t_config,.      
+00013300: 2020 6f73 2e70 6174 682e 6a6f 696e 2861    os.path.join(a
+00013310: 6464 6f6e 735f 7061 7468 2c20 6e61 6d65  ddons_path, name
+00013320: 2929 0a20 2020 2020 2020 2074 6774 5f70  )).        tgt_p
+00013330: 6174 6873 203d 205b 5d0a 2020 2020 2020  aths = [].      
+00013340: 2020 7467 745f 7061 7468 732e 696e 7365    tgt_paths.inse
+00013350: 7274 2830 2c20 6164 646f 6e73 5f70 6174  rt(0, addons_pat
+00013360: 6829 0a20 2020 2020 2020 2074 6774 5f70  h).        tgt_p
+00013370: 6174 6873 2e69 6e73 6572 7428 302c 2072  aths.insert(0, r
+00013380: 6f6f 745f 7061 7468 290a 2020 2020 2020  oot_path).      
+00013390: 2020 7467 745f 6675 6c6c 5f6c 636f 6e66    tgt_full_lconf
+000133a0: 203d 2070 7265 7061 7265 5f63 6f6e 6669   = prepare_confi
+000133b0: 675f 6669 6c65 2874 6774 5f63 7478 2c20  g_file(tgt_ctx, 
+000133c0: 7467 745f 636f 6e66 6967 2c0a 2020 2020  tgt_config,.    
 000133d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000133e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000133f0: 2020 2020 2020 206f 755f 7665 725f 7061         ou_ver_pa
-00013400: 7468 3d6f 755f 7665 725f 7061 7468 2c0a  th=ou_ver_path,.
-00013410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000133f0: 2020 2020 2020 2020 206f 755f 7665 725f           ou_ver_
+00013400: 7061 7468 3d6f 755f 7665 725f 7061 7468  path=ou_ver_path
+00013410: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
 00013420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013430: 2020 2020 2020 2020 2020 2020 2070 6174               pat
-00013440: 6873 3d74 6774 5f70 6174 6873 290a 2020  hs=tgt_paths).  
-00013450: 2020 2020 2020 6966 206e 6f74 2073 7263        if not src
-00013460: 5f63 7478 5b27 6472 795f 7275 6e27 5d3a  _ctx['dry_run']:
-00013470: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00013480: 6e6f 7420 636f 7079 5f64 6228 7372 635f  not copy_db(src_
-00013490: 6374 782c 2073 7263 5f63 7478 5b27 6462  ctx, src_ctx['db
-000134a0: 5f6e 616d 6527 5d2c 2074 6774 5f63 7478  _name'], tgt_ctx
-000134b0: 5b27 6462 5f6e 616d 6527 5d29 3a0a 2020  ['db_name']):.  
-000134c0: 2020 2020 2020 2020 2020 2020 2020 6578                ex
-000134d0: 6974 2831 290a 2020 2020 2020 2020 2020  it(1).          
-000134e0: 2020 6669 785f 6275 675f 7072 6528 7372    fix_bug_pre(sr
-000134f0: 635f 6374 782c 2074 6774 5f63 7478 2c20  c_ctx, tgt_ctx, 
-00013500: 7372 635f 6675 6c6c 5f6c 636f 6e66 2c20  src_full_lconf, 
-00013510: 7372 635f 7061 7468 7329 0a20 2020 2020  src_paths).     
-00013520: 2020 2020 2020 2069 6620 7372 635f 6374         if src_ct
-00013530: 785b 2764 625f 7573 6572 275d 2021 3d20  x['db_user'] != 
-00013540: 7467 745f 6374 785b 2764 625f 7573 6572  tgt_ctx['db_user
-00013550: 275d 3a0a 2020 2020 2020 2020 2020 2020  ']:.            
-00013560: 2020 2020 7265 6173 7369 676e 5f64 625f      reassign_db_
-00013570: 6f77 6e65 7228 7467 745f 6374 782c 0a20  owner(tgt_ctx,. 
-00013580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013430: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00013440: 6174 6873 3d74 6774 5f70 6174 6873 290a  aths=tgt_paths).
+00013450: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
+00013460: 7263 5f63 7478 5b27 6472 795f 7275 6e27  rc_ctx['dry_run'
+00013470: 5d3a 0a20 2020 2020 2020 2020 2020 2069  ]:.            i
+00013480: 6620 6e6f 7420 636f 7079 5f64 6228 7372  f not copy_db(sr
+00013490: 635f 6374 782c 2073 7263 5f63 7478 5b27  c_ctx, src_ctx['
+000134a0: 6462 5f6e 616d 6527 5d2c 2074 6774 5f63  db_name'], tgt_c
+000134b0: 7478 5b27 6462 5f6e 616d 6527 5d29 3a0a  tx['db_name']):.
+000134c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000134d0: 6578 6974 2831 290a 2020 2020 2020 2020  exit(1).        
+000134e0: 2020 2020 6669 785f 6275 675f 7072 6528      fix_bug_pre(
+000134f0: 7372 635f 6374 782c 2074 6774 5f63 7478  src_ctx, tgt_ctx
+00013500: 2c20 7372 635f 6675 6c6c 5f6c 636f 6e66  , src_full_lconf
+00013510: 2c20 7372 635f 7061 7468 7329 0a20 2020  , src_paths).   
+00013520: 2020 2020 2020 2020 2069 6620 7372 635f           if src_
+00013530: 6374 785b 2764 625f 7573 6572 275d 2021  ctx['db_user'] !
+00013540: 3d20 7467 745f 6374 785b 2764 625f 7573  = tgt_ctx['db_us
+00013550: 6572 275d 3a0a 2020 2020 2020 2020 2020  er']:.          
+00013560: 2020 2020 2020 7265 6173 7369 676e 5f64        reassign_d
+00013570: 625f 6f77 6e65 7228 7467 745f 6374 782c  b_owner(tgt_ctx,
+00013580: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00013590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000135a0: 2074 6774 5f63 7478 5b27 6462 5f6e 616d   tgt_ctx['db_nam
-000135b0: 6527 5d2c 0a20 2020 2020 2020 2020 2020  e'],.           
+000135a0: 2020 2074 6774 5f63 7478 5b27 6462 5f6e     tgt_ctx['db_n
+000135b0: 616d 6527 5d2c 0a20 2020 2020 2020 2020  ame'],.         
 000135c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000135d0: 2020 2020 2020 2073 7263 5f63 7478 5b27         src_ctx['
-000135e0: 6462 5f75 7365 7227 5d2c 0a20 2020 2020  db_user'],.     
+000135d0: 2020 2020 2020 2020 2073 7263 5f63 7478           src_ctx
+000135e0: 5b27 6462 5f75 7365 7227 5d2c 0a20 2020  ['db_user'],.   
 000135f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013600: 2020 2020 2020 2020 2020 2020 2074 6774               tgt
-00013610: 5f63 7478 5b27 6462 5f75 7365 7227 5d29  _ctx['db_user'])
-00013620: 0a20 2020 2020 2020 2020 2020 2023 2053  .            # S
-00013630: 6f6d 6520 6d6f 6475 6c65 7320 6e6f 7420  ome modules not 
-00013640: 6176 6169 6c61 626c 6520 6f6e 2069 6e74  available on int
-00013650: 6572 6d65 6469 6174 6520 7665 7273 696f  ermediate versio
-00013660: 6e20 6d69 6768 7420 6265 0a20 2020 2020  n might be.     
-00013670: 2020 2020 2020 2023 2061 7661 696c 6162         # availab
-00013680: 6c65 206f 6e20 6375 7272 656e 7420 7461  le on current ta
-00013690: 7267 6574 206f 646f 6f20 7665 7273 696f  rget odoo versio
-000136a0: 6e0a 2020 2020 2020 2020 2020 2020 6966  n.            if
-000136b0: 2074 6774 5f63 7478 5b27 7472 795f 7265   tgt_ctx['try_re
-000136c0: 696e 7374 616c 6c27 5d3a 0a20 2020 2020  install']:.     
-000136d0: 2020 2020 2020 2020 2020 206d 6f64 756c             modul
-000136e0: 6573 5f74 6f5f 7265 7374 6f72 6520 3d20  es_to_restore = 
-000136f0: 6261 645f 6c69 7374 203d 205b 5d0a 2020  bad_list = [].  
-00013700: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00013710: 2073 7263 5f63 7478 5b27 6f72 6967 696e   src_ctx['origin
-00013720: 616c 5f6d 6f64 756c 655f 6c69 7374 275d  al_module_list']
-00013730: 2021 3d20 7372 635f 6374 785b 0a20 2020   != src_ctx[.   
+00013600: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00013610: 6774 5f63 7478 5b27 6462 5f75 7365 7227  gt_ctx['db_user'
+00013620: 5d29 0a20 2020 2020 2020 2020 2020 2023  ]).            #
+00013630: 2053 6f6d 6520 6d6f 6475 6c65 7320 6e6f   Some modules no
+00013640: 7420 6176 6169 6c61 626c 6520 6f6e 2069  t available on i
+00013650: 6e74 6572 6d65 6469 6174 6520 7665 7273  ntermediate vers
+00013660: 696f 6e20 6d69 6768 7420 6265 0a20 2020  ion might be.   
+00013670: 2020 2020 2020 2020 2023 2061 7661 696c           # avail
+00013680: 6162 6c65 206f 6e20 6375 7272 656e 7420  able on current 
+00013690: 7461 7267 6574 206f 646f 6f20 7665 7273  target odoo vers
+000136a0: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
+000136b0: 6966 2074 6774 5f63 7478 5b27 7472 795f  if tgt_ctx['try_
+000136c0: 7265 696e 7374 616c 6c27 5d3a 0a20 2020  reinstall']:.   
+000136d0: 2020 2020 2020 2020 2020 2020 206d 6f64               mod
+000136e0: 756c 6573 5f74 6f5f 7265 7374 6f72 6520  ules_to_restore 
+000136f0: 3d20 6261 645f 6c69 7374 203d 205b 5d0a  = bad_list = [].
+00013700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013710: 6966 2073 7263 5f63 7478 5b27 6f72 6967  if src_ctx['orig
+00013720: 696e 616c 5f6d 6f64 756c 655f 6c69 7374  inal_module_list
+00013730: 275d 2021 3d20 7372 635f 6374 785b 0a20  '] != src_ctx[. 
 00013740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013750: 2020 2020 2027 7372 635f 6d6f 6475 6c65       'src_module
-00013760: 5f6c 6973 7427 5d3a 0a20 2020 2020 2020  _list']:.       
-00013770: 2020 2020 2020 2020 2020 2020 206d 6f64               mod
-00013780: 756c 6573 5f74 6f5f 7265 7374 6f72 652c  ules_to_restore,
-00013790: 2062 6164 5f6c 6973 7420 3d20 646f 5f74   bad_list = do_t
-000137a0: 6e6c 5f6d 6f64 756c 655f 6c69 7374 280a  nl_module_list(.
-000137b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000137c0: 2020 2020 2020 2020 7467 745f 6374 782c          tgt_ctx,
-000137d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000137e0: 2020 2020 2020 2020 2073 7263 5f63 7478           src_ctx
-000137f0: 5b27 6f72 6967 696e 616c 5f6d 6f64 756c  ['original_modul
-00013800: 655f 6c69 7374 275d 2c0a 2020 2020 2020  e_list'],.      
+00013750: 2020 2020 2020 2027 7372 635f 6d6f 6475         'src_modu
+00013760: 6c65 5f6c 6973 7427 5d3a 0a20 2020 2020  le_list']:.     
+00013770: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00013780: 6f64 756c 6573 5f74 6f5f 7265 7374 6f72  odules_to_restor
+00013790: 652c 2062 6164 5f6c 6973 7420 3d20 646f  e, bad_list = do
+000137a0: 5f74 6e6c 5f6d 6f64 756c 655f 6c69 7374  _tnl_module_list
+000137b0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+000137c0: 2020 2020 2020 2020 2020 7467 745f 6374            tgt_ct
+000137d0: 782c 0a20 2020 2020 2020 2020 2020 2020  x,.             
+000137e0: 2020 2020 2020 2020 2020 2073 7263 5f63             src_c
+000137f0: 7478 5b27 6f72 6967 696e 616c 5f6d 6f64  tx['original_mod
+00013800: 756c 655f 6c69 7374 275d 2c0a 2020 2020  ule_list'],.    
 00013810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013820: 2020 7372 635f 6374 785b 2766 726f 6d5f    src_ctx['from_
-00013830: 6f64 6f6f 5f66 7665 7227 5d2c 0a20 2020  odoo_fver'],.   
+00013820: 2020 2020 7372 635f 6374 785b 2766 726f      src_ctx['fro
+00013830: 6d5f 6f64 6f6f 5f66 7665 7227 5d2c 0a20  m_odoo_fver'],. 
 00013840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013850: 2020 2020 2074 6774 5f63 7478 5b27 7467       tgt_ctx['tg
-00013860: 745f 6f64 6f6f 5f66 7665 7227 5d2c 0a20  t_odoo_fver'],. 
-00013870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013880: 2020 2020 2020 2074 6774 5f61 6c6c 5f6d         tgt_all_m
-00013890: 6f64 756c 655f 6c69 7374 2c0a 2020 2020  odule_list,.    
+00013850: 2020 2020 2020 2074 6774 5f63 7478 5b27         tgt_ctx['
+00013860: 7467 745f 6f64 6f6f 5f66 7665 7227 5d2c  tgt_odoo_fver'],
+00013870: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013880: 2020 2020 2020 2020 2074 6774 5f61 6c6c           tgt_all
+00013890: 5f6d 6f64 756c 655f 6c69 7374 2c0a 2020  _module_list,.  
 000138a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000138b0: 2020 2020 7075 7265 3d54 7275 6529 0a20      pure=True). 
-000138c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000138d0: 2020 206d 6f64 756c 6573 5f74 6f5f 7265     modules_to_re
-000138e0: 7374 6f72 6520 3d20 6c69 7374 2873 6574  store = list(set
-000138f0: 286d 6f64 756c 6573 5f74 6f5f 7265 7374  (modules_to_rest
-00013900: 6f72 6529 202d 0a20 2020 2020 2020 2020  ore) -.         
+000138b0: 2020 2020 2020 7075 7265 3d54 7275 6529        pure=True)
+000138c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000138d0: 2020 2020 206d 6f64 756c 6573 5f74 6f5f       modules_to_
+000138e0: 7265 7374 6f72 6520 3d20 6c69 7374 2873  restore = list(s
+000138f0: 6574 286d 6f64 756c 6573 5f74 6f5f 7265  et(modules_to_re
+00013900: 7374 6f72 6529 202d 0a20 2020 2020 2020  store) -.       
 00013910: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013930: 2020 2020 2073 6574 2873 7263 5f63 7478       set(src_ctx
-00013940: 5b27 7372 635f 6d6f 6475 6c65 5f6c 6973  ['src_module_lis
-00013950: 7427 5d29 290a 2020 2020 2020 2020 2020  t'])).          
-00013960: 2020 2020 2020 2020 2020 6966 206d 6f64            if mod
-00013970: 756c 6573 5f74 6f5f 7265 7374 6f72 653a  ules_to_restore:
-00013980: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013990: 2020 2020 2020 2020 2073 6574 5f69 6e73           set_ins
-000139a0: 7461 6c6c 6564 5f62 795f 7371 6c28 7467  talled_by_sql(tg
-000139b0: 745f 6374 782c 206d 6f64 756c 6573 5f74  t_ctx, modules_t
-000139c0: 6f5f 7265 7374 6f72 6529 0a20 2020 2020  o_restore).     
-000139d0: 2020 2020 2020 2064 726f 705f 7365 7373         drop_sess
-000139e0: 696f 6e28 7467 745f 6374 782c 2074 6774  ion(tgt_ctx, tgt
-000139f0: 5f63 7478 5b27 6462 5f6e 616d 6527 5d2c  _ctx['db_name'],
-00013a00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013a10: 2020 2020 2020 2020 2020 6f64 6f6f 5f76            odoo_v
-00013a20: 6964 3d74 6774 5f63 7478 5b27 7467 745f  id=tgt_ctx['tgt_
-00013a30: 7669 6427 5d29 0a20 2020 2020 2020 2072  vid']).        r
-00013a40: 756e 5f6f 7065 6e75 7067 7261 6465 2874  un_openupgrade(t
-00013a50: 6774 5f63 7478 2c20 6f75 5f76 6572 5f70  gt_ctx, ou_ver_p
-00013a60: 6174 682c 2074 6774 5f66 756c 6c5f 6c63  ath, tgt_full_lc
-00013a70: 6f6e 6629 0a20 2020 2020 2020 2069 6620  onf).        if 
-00013a80: 6e6f 7420 7372 635f 6374 785b 2764 7279  not src_ctx['dry
-00013a90: 5f72 756e 275d 3a0a 2020 2020 2020 2020  _run']:.        
-00013aa0: 2020 2020 6669 785f 6275 675f 706f 7374      fix_bug_post
-00013ab0: 2873 7263 5f63 7478 2c20 7467 745f 6374  (src_ctx, tgt_ct
-00013ac0: 782c 2073 7263 5f66 756c 6c5f 6c63 6f6e  x, src_full_lcon
-00013ad0: 662c 2073 7263 5f70 6174 6873 290a 0a20  f, src_paths).. 
-00013ae0: 2020 2023 2054 6573 7420 666f 7220 6e6f     # Test for no
-00013af0: 7420 6d69 6772 6174 6564 206d 6f64 756c  t migrated modul
-00013b00: 6573 0a20 2020 2074 6774 5f63 7478 5b27  es.    tgt_ctx['
-00013b10: 636f 6e66 5f66 6e27 5d20 3d20 7467 745f  conf_fn'] = tgt_
-00013b20: 7361 7665 645f 6663 6f6e 660a 2020 2020  saved_fconf.    
-00013b30: 746f 5f75 6e69 6e73 7461 6c6c 5f6c 6973  to_uninstall_lis
-00013b40: 7420 3d20 6765 745f 7772 6f6e 675f 6d6f  t = get_wrong_mo
-00013b50: 6475 6c65 7328 7467 745f 6374 7829 0a20  dules(tgt_ctx). 
-00013b60: 2020 2069 6620 746f 5f75 6e69 6e73 7461     if to_uninsta
-00013b70: 6c6c 5f6c 6973 743a 0a20 2020 2020 2020  ll_list:.       
-00013b80: 206f 7330 2e77 6c6f 6728 272a 2a2a 2057   os0.wlog('*** W
-00013b90: 726f 6e67 2073 7461 7465 2066 6f72 206d  rong state for m
-00013ba0: 6f64 756c 6573 2025 7320 2a2a 2a27 2025  odules %s ***' %
-00013bb0: 2074 6f5f 756e 696e 7374 616c 6c5f 6c69   to_uninstall_li
-00013bc0: 7374 290a 2020 2020 6861 7264 5f75 6e69  st).    hard_uni
-00013bd0: 6e73 7461 6c6c 5f6c 6973 7420 3d20 6c69  nstall_list = li
-00013be0: 7374 280a 2020 2020 2020 2020 7365 7428  st(.        set(
-00013bf0: 746f 5f75 6e69 6e73 7461 6c6c 5f6c 6973  to_uninstall_lis
-00013c00: 7429 2026 2073 6574 284d 4f44 554c 4553  t) & set(MODULES
-00013c10: 5f32 5f4c 4541 5645 5f42 4548 494e 4429  _2_LEAVE_BEHIND)
-00013c20: 290a 2020 2020 736f 6674 5f75 6e69 6e73  ).    soft_unins
-00013c30: 7461 6c6c 5f6c 6973 7420 3d20 6c69 7374  tall_list = list
-00013c40: 280a 2020 2020 2020 2020 7365 7428 746f  (.        set(to
-00013c50: 5f75 6e69 6e73 7461 6c6c 5f6c 6973 7429  _uninstall_list)
-00013c60: 202d 2073 6574 2868 6172 645f 756e 696e   - set(hard_unin
-00013c70: 7374 616c 6c5f 6c69 7374 2929 0a20 2020  stall_list)).   
-00013c80: 2069 6620 736f 6674 5f75 6e69 6e73 7461   if soft_uninsta
-00013c90: 6c6c 5f6c 6973 743a 0a20 2020 2020 2020  ll_list:.       
-00013ca0: 2073 6574 5f75 6e69 6e73 7461 6c6c 6564   set_uninstalled
-00013cb0: 5f62 795f 7371 6c28 7467 745f 6374 782c  _by_sql(tgt_ctx,
-00013cc0: 2073 6f66 745f 756e 696e 7374 616c 6c5f   soft_uninstall_
-00013cd0: 6c69 7374 290a 2020 2020 6966 2068 6172  list).    if har
-00013ce0: 645f 756e 696e 7374 616c 6c5f 6c69 7374  d_uninstall_list
-00013cf0: 3a0a 2020 2020 2020 2020 6f73 302e 776c  :.        os0.wl
-00013d00: 6f67 2827 2a2a 2a20 556e 7374 6162 6c65  og('*** Unstable
-00013d10: 2044 423a 2077 726f 6e67 206d 6f64 756c   DB: wrong modul
-00013d20: 6520 7374 6174 6520 2573 202a 2a2a 2720  e state %s ***' 
-00013d30: 250a 2020 2020 2020 2020 2020 2020 2020  %.              
-00013d40: 2020 2068 6172 645f 756e 696e 7374 616c     hard_uninstal
-00013d50: 6c5f 6c69 7374 290a 2020 2020 666f 7220  l_list).    for 
-00013d60: 6d6f 6475 6c65 2069 6e20 6861 7264 5f75  module in hard_u
-00013d70: 6e69 6e73 7461 6c6c 5f6c 6973 743a 0a20  ninstall_list:. 
-00013d80: 2020 2020 2020 206f 7330 2e77 6c6f 6728         os0.wlog(
-00013d90: 2720 202b 2b20 4861 7264 2075 6e69 6e73  '  ++ Hard unins
-00013da0: 7461 6c6c 3a20 2573 2720 2520 6d6f 6475  tall: %s' % modu
-00013db0: 6c65 290a 2020 2020 2020 2020 6861 7264  le).        hard
-00013dc0: 5f63 6c65 616e 5f6d 6f64 756c 6528 7467  _clean_module(tg
-00013dd0: 745f 6374 782c 206d 6f64 756c 6529 0a20  t_ctx, module). 
-00013de0: 2020 2069 6620 736f 6674 5f75 6e69 6e73     if soft_unins
-00013df0: 7461 6c6c 5f6c 6973 7420 6f72 2068 6172  tall_list or har
-00013e00: 645f 756e 696e 7374 616c 6c5f 6c69 7374  d_uninstall_list
-00013e10: 3a0a 2020 2020 2020 2020 6261 645f 6d6f  :.        bad_mo
-00013e20: 6475 6c65 7320 3d20 6c69 7374 2873 6574  dules = list(set
-00013e30: 2873 6f66 745f 756e 696e 7374 616c 6c5f  (soft_uninstall_
-00013e40: 6c69 7374 2920 7c20 7365 7428 6861 7264  list) | set(hard
-00013e50: 5f75 6e69 6e73 7461 6c6c 5f6c 6973 7429  _uninstall_list)
-00013e60: 290a 2020 2020 2020 2020 7275 6e5f 6f64  ).        run_od
-00013e70: 6f6f 5f61 6c6c 7465 7374 2874 6774 5f63  oo_alltest(tgt_c
-00013e80: 7478 5b27 7467 745f 7669 6427 5d2c 2074  tx['tgt_vid'], t
-00013e90: 6774 5f63 7478 5b27 636f 6e66 5f66 6e27  gt_ctx['conf_fn'
-00013ea0: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-00013eb0: 2020 2020 2020 2020 2020 2020 7467 745f              tgt_
-00013ec0: 6374 785b 2764 625f 6e61 6d65 275d 2c20  ctx['db_name'], 
-00013ed0: 7467 745f 6374 785b 276c 6f67 6669 6c65  tgt_ctx['logfile
-00013ee0: 275d 2c0a 2020 2020 2020 2020 2020 2020  '],.            
-00013ef0: 2020 2020 2020 2020 2020 2020 206d 6f64               mod
-00013f00: 756c 6573 3d62 6164 5f6d 6f64 756c 6573  ules=bad_modules
-00013f10: 290a 2020 2020 656c 6966 2074 6774 5f63  ).    elif tgt_c
-00013f20: 7478 5b27 6f70 745f 7361 6665 275d 2061  tx['opt_safe'] a
-00013f30: 6e64 206e 6f74 2073 7263 5f63 7478 5b27  nd not src_ctx['
-00013f40: 6472 795f 7275 6e27 5d3a 0a20 2020 2020  dry_run']:.     
-00013f50: 2020 2072 756e 5f6f 646f 6f5f 616c 6c74     run_odoo_allt
-00013f60: 6573 7428 7467 745f 6374 785b 2774 6774  est(tgt_ctx['tgt
-00013f70: 5f76 6964 275d 2c20 7467 745f 6374 785b  _vid'], tgt_ctx[
-00013f80: 2763 6f6e 665f 666e 275d 2c0a 2020 2020  'conf_fn'],.    
+00013930: 2020 2020 2020 2073 6574 2873 7263 5f63         set(src_c
+00013940: 7478 5b27 7372 635f 6d6f 6475 6c65 5f6c  tx['src_module_l
+00013950: 6973 7427 5d29 290a 2020 2020 2020 2020  ist'])).        
+00013960: 2020 2020 2020 2020 2020 2020 6966 206d              if m
+00013970: 6f64 756c 6573 5f74 6f5f 7265 7374 6f72  odules_to_restor
+00013980: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00013990: 2020 2020 2020 2020 2020 2073 6574 5f69             set_i
+000139a0: 6e73 7461 6c6c 6564 5f62 795f 7371 6c28  nstalled_by_sql(
+000139b0: 7467 745f 6374 782c 206d 6f64 756c 6573  tgt_ctx, modules
+000139c0: 5f74 6f5f 7265 7374 6f72 6529 0a20 2020  _to_restore).   
+000139d0: 2020 2020 2020 2020 2064 726f 705f 7365           drop_se
+000139e0: 7373 696f 6e28 7467 745f 6374 782c 2074  ssion(tgt_ctx, t
+000139f0: 6774 5f63 7478 5b27 6462 5f6e 616d 6527  gt_ctx['db_name'
+00013a00: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+00013a10: 2020 2020 2020 2020 2020 2020 6f64 6f6f              odoo
+00013a20: 5f76 6964 3d74 6774 5f63 7478 5b27 7467  _vid=tgt_ctx['tg
+00013a30: 745f 7669 6427 5d29 0a20 2020 2020 2020  t_vid']).       
+00013a40: 2072 756e 5f6f 7065 6e75 7067 7261 6465   run_openupgrade
+00013a50: 2874 6774 5f63 7478 2c20 6f75 5f76 6572  (tgt_ctx, ou_ver
+00013a60: 5f70 6174 682c 2074 6774 5f66 756c 6c5f  _path, tgt_full_
+00013a70: 6c63 6f6e 6629 0a20 2020 2020 2020 2069  lconf).        i
+00013a80: 6620 6e6f 7420 7372 635f 6374 785b 2764  f not src_ctx['d
+00013a90: 7279 5f72 756e 275d 3a0a 2020 2020 2020  ry_run']:.      
+00013aa0: 2020 2020 2020 6669 785f 6275 675f 706f        fix_bug_po
+00013ab0: 7374 2873 7263 5f63 7478 2c20 7467 745f  st(src_ctx, tgt_
+00013ac0: 6374 782c 2073 7263 5f66 756c 6c5f 6c63  ctx, src_full_lc
+00013ad0: 6f6e 662c 2073 7263 5f70 6174 6873 290a  onf, src_paths).
+00013ae0: 0a20 2020 2023 2054 6573 7420 666f 7220  .    # Test for 
+00013af0: 6e6f 7420 6d69 6772 6174 6564 206d 6f64  not migrated mod
+00013b00: 756c 6573 0a20 2020 2074 6774 5f63 7478  ules.    tgt_ctx
+00013b10: 5b27 636f 6e66 5f66 6e27 5d20 3d20 7467  ['conf_fn'] = tg
+00013b20: 745f 7361 7665 645f 6663 6f6e 660a 2020  t_saved_fconf.  
+00013b30: 2020 746f 5f75 6e69 6e73 7461 6c6c 5f6c    to_uninstall_l
+00013b40: 6973 7420 3d20 6765 745f 7772 6f6e 675f  ist = get_wrong_
+00013b50: 6d6f 6475 6c65 7328 7467 745f 6374 7829  modules(tgt_ctx)
+00013b60: 0a20 2020 2069 6620 746f 5f75 6e69 6e73  .    if to_unins
+00013b70: 7461 6c6c 5f6c 6973 743a 0a20 2020 2020  tall_list:.     
+00013b80: 2020 206f 7330 2e77 6c6f 6728 272a 2a2a     os0.wlog('***
+00013b90: 2057 726f 6e67 2073 7461 7465 2066 6f72   Wrong state for
+00013ba0: 206d 6f64 756c 6573 2025 7320 2a2a 2a27   modules %s ***'
+00013bb0: 2025 2074 6f5f 756e 696e 7374 616c 6c5f   % to_uninstall_
+00013bc0: 6c69 7374 290a 2020 2020 6861 7264 5f75  list).    hard_u
+00013bd0: 6e69 6e73 7461 6c6c 5f6c 6973 7420 3d20  ninstall_list = 
+00013be0: 6c69 7374 280a 2020 2020 2020 2020 7365  list(.        se
+00013bf0: 7428 746f 5f75 6e69 6e73 7461 6c6c 5f6c  t(to_uninstall_l
+00013c00: 6973 7429 2026 2073 6574 284d 4f44 554c  ist) & set(MODUL
+00013c10: 4553 5f32 5f4c 4541 5645 5f42 4548 494e  ES_2_LEAVE_BEHIN
+00013c20: 4429 290a 2020 2020 736f 6674 5f75 6e69  D)).    soft_uni
+00013c30: 6e73 7461 6c6c 5f6c 6973 7420 3d20 6c69  nstall_list = li
+00013c40: 7374 280a 2020 2020 2020 2020 7365 7428  st(.        set(
+00013c50: 746f 5f75 6e69 6e73 7461 6c6c 5f6c 6973  to_uninstall_lis
+00013c60: 7429 202d 2073 6574 2868 6172 645f 756e  t) - set(hard_un
+00013c70: 696e 7374 616c 6c5f 6c69 7374 2929 0a20  install_list)). 
+00013c80: 2020 2069 6620 736f 6674 5f75 6e69 6e73     if soft_unins
+00013c90: 7461 6c6c 5f6c 6973 743a 0a20 2020 2020  tall_list:.     
+00013ca0: 2020 2073 6574 5f75 6e69 6e73 7461 6c6c     set_uninstall
+00013cb0: 6564 5f62 795f 7371 6c28 7467 745f 6374  ed_by_sql(tgt_ct
+00013cc0: 782c 2073 6f66 745f 756e 696e 7374 616c  x, soft_uninstal
+00013cd0: 6c5f 6c69 7374 290a 2020 2020 6966 2068  l_list).    if h
+00013ce0: 6172 645f 756e 696e 7374 616c 6c5f 6c69  ard_uninstall_li
+00013cf0: 7374 3a0a 2020 2020 2020 2020 6f73 302e  st:.        os0.
+00013d00: 776c 6f67 2827 2a2a 2a20 556e 7374 6162  wlog('*** Unstab
+00013d10: 6c65 2044 423a 2077 726f 6e67 206d 6f64  le DB: wrong mod
+00013d20: 756c 6520 7374 6174 6520 2573 202a 2a2a  ule state %s ***
+00013d30: 2720 250a 2020 2020 2020 2020 2020 2020  ' %.            
+00013d40: 2020 2020 2068 6172 645f 756e 696e 7374       hard_uninst
+00013d50: 616c 6c5f 6c69 7374 290a 2020 2020 666f  all_list).    fo
+00013d60: 7220 6d6f 6475 6c65 2069 6e20 6861 7264  r module in hard
+00013d70: 5f75 6e69 6e73 7461 6c6c 5f6c 6973 743a  _uninstall_list:
+00013d80: 0a20 2020 2020 2020 206f 7330 2e77 6c6f  .        os0.wlo
+00013d90: 6728 2720 202b 2b20 4861 7264 2075 6e69  g('  ++ Hard uni
+00013da0: 6e73 7461 6c6c 3a20 2573 2720 2520 6d6f  nstall: %s' % mo
+00013db0: 6475 6c65 290a 2020 2020 2020 2020 6861  dule).        ha
+00013dc0: 7264 5f63 6c65 616e 5f6d 6f64 756c 6528  rd_clean_module(
+00013dd0: 7467 745f 6374 782c 206d 6f64 756c 6529  tgt_ctx, module)
+00013de0: 0a20 2020 2069 6620 736f 6674 5f75 6e69  .    if soft_uni
+00013df0: 6e73 7461 6c6c 5f6c 6973 7420 6f72 2068  nstall_list or h
+00013e00: 6172 645f 756e 696e 7374 616c 6c5f 6c69  ard_uninstall_li
+00013e10: 7374 3a0a 2020 2020 2020 2020 6261 645f  st:.        bad_
+00013e20: 6d6f 6475 6c65 7320 3d20 6c69 7374 2873  modules = list(s
+00013e30: 6574 2873 6f66 745f 756e 696e 7374 616c  et(soft_uninstal
+00013e40: 6c5f 6c69 7374 2920 7c20 7365 7428 6861  l_list) | set(ha
+00013e50: 7264 5f75 6e69 6e73 7461 6c6c 5f6c 6973  rd_uninstall_lis
+00013e60: 7429 290a 2020 2020 2020 2020 7275 6e5f  t)).        run_
+00013e70: 6f64 6f6f 5f61 6c6c 7465 7374 2874 6774  odoo_alltest(tgt
+00013e80: 5f63 7478 5b27 7467 745f 7669 6427 5d2c  _ctx['tgt_vid'],
+00013e90: 2074 6774 5f63 7478 5b27 636f 6e66 5f66   tgt_ctx['conf_f
+00013ea0: 6e27 5d2c 0a20 2020 2020 2020 2020 2020  n'],.           
+00013eb0: 2020 2020 2020 2020 2020 2020 2020 7467                tg
+00013ec0: 745f 6374 785b 2764 625f 6e61 6d65 275d  t_ctx['db_name']
+00013ed0: 2c20 7467 745f 6374 785b 276c 6f67 6669  , tgt_ctx['logfi
+00013ee0: 6c65 275d 2c0a 2020 2020 2020 2020 2020  le'],.          
+00013ef0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00013f00: 6f64 756c 6573 3d62 6164 5f6d 6f64 756c  odules=bad_modul
+00013f10: 6573 290a 2020 2020 656c 6966 2074 6774  es).    elif tgt
+00013f20: 5f63 7478 5b27 6f70 745f 7361 6665 275d  _ctx['opt_safe']
+00013f30: 2061 6e64 206e 6f74 2073 7263 5f63 7478   and not src_ctx
+00013f40: 5b27 6472 795f 7275 6e27 5d3a 0a20 2020  ['dry_run']:.   
+00013f50: 2020 2020 2072 756e 5f6f 646f 6f5f 616c       run_odoo_al
+00013f60: 6c74 6573 7428 7467 745f 6374 785b 2774  ltest(tgt_ctx['t
+00013f70: 6774 5f76 6964 275d 2c20 7467 745f 6374  gt_vid'], tgt_ct
+00013f80: 785b 2763 6f6e 665f 666e 275d 2c0a 2020  x['conf_fn'],.  
 00013f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013fa0: 2020 2020 2074 6774 5f63 7478 5b27 6462       tgt_ctx['db
-00013fb0: 5f6e 616d 6527 5d2c 2074 6774 5f63 7478  _name'], tgt_ctx
-00013fc0: 5b27 6c6f 6766 696c 6527 5d29 0a20 2020  ['logfile']).   
-00013fd0: 2062 6164 5f6d 6f64 756c 6573 203d 2067   bad_modules = g
-00013fe0: 6574 5f77 726f 6e67 5f6d 6f64 756c 6573  et_wrong_modules
-00013ff0: 2874 6774 5f63 7478 290a 2020 2020 6966  (tgt_ctx).    if
-00014000: 2062 6164 5f6d 6f64 756c 6573 3a0a 2020   bad_modules:.  
-00014010: 2020 2020 2020 6f73 302e 776c 6f67 2827        os0.wlog('
-00014020: 2a2a 2a20 556e 7374 6162 6c65 2044 4220  *** Unstable DB 
-00014030: 6166 7465 7220 636c 6561 6e3a 2077 726f  after clean: wro
-00014040: 6e67 206d 6f64 756c 6520 7374 6174 6520  ng module state 
-00014050: 2573 202a 2a2a 2720 250a 2020 2020 2020  %s ***' %.      
-00014060: 2020 2020 2020 2020 2020 2062 6164 5f6d             bad_m
-00014070: 6f64 756c 6573 290a 2020 2020 2020 2020  odules).        
-00014080: 6861 7264 5f75 6e69 6e73 7461 6c6c 5f6c  hard_uninstall_l
-00014090: 6973 7420 3d20 6c69 7374 280a 2020 2020  ist = list(.    
-000140a0: 2020 2020 2020 2020 7365 7428 6261 645f          set(bad_
-000140b0: 6d6f 6475 6c65 7329 2026 2073 6574 284d  modules) & set(M
-000140c0: 4f44 554c 4553 5f32 5f4c 4541 5645 5f42  ODULES_2_LEAVE_B
-000140d0: 4548 494e 4429 290a 2020 2020 2020 2020  EHIND)).        
-000140e0: 6261 645f 6d6f 6475 6c65 7320 3d20 6c69  bad_modules = li
-000140f0: 7374 280a 2020 2020 2020 2020 2020 2020  st(.            
-00014100: 7365 7428 6261 645f 6d6f 6475 6c65 7329  set(bad_modules)
-00014110: 202d 2073 6574 284d 4f44 554c 4553 5f32   - set(MODULES_2
-00014120: 5f4c 4541 5645 5f42 4548 494e 4429 290a  _LEAVE_BEHIND)).
-00014130: 2020 2020 2020 2020 6966 2062 6164 5f6d          if bad_m
-00014140: 6f64 756c 6573 3a0a 2020 2020 2020 2020  odules:.        
-00014150: 2020 2020 7365 745f 756e 696e 7374 616c      set_uninstal
-00014160: 6c65 645f 6279 5f73 716c 2874 6774 5f63  led_by_sql(tgt_c
-00014170: 7478 2c20 6261 645f 6d6f 6475 6c65 7329  tx, bad_modules)
-00014180: 0a20 2020 2020 2020 2069 6620 6861 7264  .        if hard
-00014190: 5f75 6e69 6e73 7461 6c6c 5f6c 6973 743a  _uninstall_list:
-000141a0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-000141b0: 206d 6f64 756c 6520 696e 2068 6172 645f   module in hard_
-000141c0: 756e 696e 7374 616c 6c5f 6c69 7374 3a0a  uninstall_list:.
-000141d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000141e0: 6f73 302e 776c 6f67 2827 2020 2b2b 2048  os0.wlog('  ++ H
-000141f0: 6172 6420 756e 696e 7374 616c 6c3a 2025  ard uninstall: %
-00014200: 7327 2025 206d 6f64 756c 6529 0a20 2020  s' % module).   
-00014210: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00014220: 6e6f 7420 7372 635f 6374 785b 2764 7279  not src_ctx['dry
-00014230: 5f72 756e 275d 3a0a 2020 2020 2020 2020  _run']:.        
-00014240: 2020 2020 2020 2020 2020 2020 6861 7264              hard
-00014250: 5f63 6c65 616e 5f6d 6f64 756c 6528 7467  _clean_module(tg
-00014260: 745f 6374 782c 206d 6f64 756c 6529 0a0a  t_ctx, module)..
-00014270: 2020 2020 6966 206e 6f74 2073 7263 5f63      if not src_c
-00014280: 7478 5b27 6472 795f 7275 6e27 5d3a 0a20  tx['dry_run']:. 
-00014290: 2020 2020 2020 206f 7330 2e77 6c6f 6728         os0.wlog(
-000142a0: 2754 6573 7420 636f 6e6e 6563 7469 6f6e  'Test connection
-000142b0: 2074 6f20 7461 7267 6574 2064 6220 2573   to target db %s
-000142c0: 2720 2520 7467 745f 6374 785b 2764 625f  ' % tgt_ctx['db_
-000142d0: 6e61 6d65 275d 290a 2020 2020 2020 2020  name']).        
-000142e0: 7569 642c 2074 6774 5f63 7478 203d 2063  uid, tgt_ctx = c
-000142f0: 6c6f 646f 6f2e 6f65 7270 5f73 6574 5f65  lodoo.oerp_set_e
-00014300: 6e76 280a 2020 2020 2020 2020 2020 2020  nv(.            
-00014310: 6374 783d 7467 745f 6374 782c 2063 6f6e  ctx=tgt_ctx, con
-00014320: 666e 3d74 6774 5f66 756c 6c5f 6c63 6f6e  fn=tgt_full_lcon
-00014330: 662c 2064 623d 7467 745f 6374 785b 2764  f, db=tgt_ctx['d
-00014340: 625f 6e61 6d65 275d 290a 2020 2020 2020  b_name']).      
-00014350: 2020 2320 4649 5820 6f65 7270 5f73 6574    # FIX oerp_set
-00014360: 5f65 6e76 2063 6861 6e67 6520 6472 795f  _env change dry_
-00014370: 7275 6e0a 2020 2020 2020 2020 7372 635f  run.        src_
-00014380: 6374 785b 2764 7279 5f72 756e 275d 203d  ctx['dry_run'] =
-00014390: 2074 6774 5f63 7478 5b27 6472 795f 7275   tgt_ctx['dry_ru
-000143a0: 6e27 5d0a 0a20 2020 2072 6574 7572 6e20  n']..    return 
-000143b0: 7467 745f 6675 6c6c 5f6c 636f 6e66 0a0a  tgt_full_lconf..
-000143c0: 0a64 6566 206d 6967 7261 7465 5f64 6174  .def migrate_dat
-000143d0: 6162 6173 655f 7061 7373 2873 7263 5f63  abase_pass(src_c
-000143e0: 7478 2c20 7467 745f 6374 782c 2070 6861  tx, tgt_ctx, pha
-000143f0: 7365 3d4e 6f6e 6529 3a0a 2020 2020 7068  se=None):.    ph
-00014400: 6173 6520 3d20 7068 6173 6520 6f72 2032  ase = phase or 2
-00014410: 0a20 2020 2064 6973 6162 6c65 5f76 656e  .    disable_ven
-00014420: 7620 3d20 4661 6c73 650a 2020 2020 6966  v = False.    if
-00014430: 2070 6861 7365 203d 3d20 313a 0a20 2020   phase == 1:.   
-00014440: 2020 2020 2073 6176 6564 5f64 7279 5f72       saved_dry_r
-00014450: 756e 203d 2073 7263 5f63 7478 5b27 6472  un = src_ctx['dr
-00014460: 795f 7275 6e27 5d0a 2020 2020 2020 2020  y_run'].        
-00014470: 7372 635f 6374 785b 2764 7279 5f72 756e  src_ctx['dry_run
-00014480: 275d 203d 2054 7275 650a 2020 2020 2020  '] = True.      
-00014490: 2020 7467 745f 6374 785b 2764 7279 5f72    tgt_ctx['dry_r
-000144a0: 756e 275d 203d 2073 7263 5f63 7478 5b27  un'] = src_ctx['
-000144b0: 6472 795f 7275 6e27 5d0a 2020 2020 7768  dry_run'].    wh
-000144c0: 696c 6520 313a 0a20 2020 2020 2020 206f  ile 1:.        o
-000144d0: 7330 2e77 6c6f 6728 272d 2720 2a20 3830  s0.wlog('-' * 80
-000144e0: 290a 2020 2020 2020 2020 7372 635f 6374  ).        src_ct
-000144f0: 782c 2074 6774 5f63 7478 2c20 7372 635f  x, tgt_ctx, src_
-00014500: 636f 6e66 6967 2c20 7467 745f 636f 6e66  config, tgt_conf
-00014510: 6967 203d 2061 646a 7573 745f 6374 7828  ig = adjust_ctx(
-00014520: 7372 635f 6374 782c 2074 6774 5f63 7478  src_ctx, tgt_ctx
-00014530: 290a 2020 2020 2020 2020 666f 7220 7061  ).        for pa
-00014540: 7261 6d20 696e 2028 2776 6964 272c 2027  ram in ('vid', '
-00014550: 6f64 6f6f 5f66 7665 7227 2c20 276f 646f  odoo_fver', 'odo
-00014560: 6f5f 7665 7227 293a 0a20 2020 2020 2020  o_ver'):.       
-00014570: 2020 2020 206f 7330 2e77 6c6f 6728 2750       os0.wlog('P
-00014580: 6173 7320 2564 206d 6967 7261 7469 6f6e  ass %d migration
-00014590: 3a20 2573 2066 726f 6d20 2573 2074 6f20  : %s from %s to 
-000145a0: 2573 202e 2e27 2025 0a20 2020 2020 2020  %s ..' %.       
-000145b0: 2020 2020 2020 2020 2020 2870 6861 7365            (phase
-000145c0: 2c20 7061 7261 6d2c 0a20 2020 2020 2020  , param,.       
-000145d0: 2020 2020 2020 2020 2020 2073 7263 5f63             src_c
-000145e0: 7478 5b27 7372 635f 2573 2720 2520 7061  tx['src_%s' % pa
-000145f0: 7261 6d5d 2c20 7467 745f 6374 785b 2774  ram], tgt_ctx['t
-00014600: 6774 5f25 7327 2025 2070 6172 616d 5d29  gt_%s' % param])
-00014610: 290a 2020 2020 2020 2020 666f 7220 7061  ).        for pa
-00014620: 7261 6d20 696e 2028 2764 625f 6e61 6d65  ram in ('db_name
-00014630: 272c 2027 636f 6e66 5f66 6e27 2c20 2778  ', 'conf_fn', 'x
-00014640: 6d6c 7270 635f 706f 7274 272c 2027 6462  mlrpc_port', 'db
-00014650: 5f75 7365 7227 293a 0a20 2020 2020 2020  _user'):.       
-00014660: 2020 2020 206f 7330 2e77 6c6f 6728 2750       os0.wlog('P
-00014670: 6173 7320 2564 206d 6967 7261 7469 6f6e  ass %d migration
-00014680: 3a20 2573 2066 726f 6d20 2573 2074 6f20  : %s from %s to 
-00014690: 2573 202e 2e27 2025 0a20 2020 2020 2020  %s ..' %.       
-000146a0: 2020 2020 2020 2020 2020 2870 6861 7365            (phase
-000146b0: 2c20 7061 7261 6d2c 2073 7263 5f63 7478  , param, src_ctx
-000146c0: 5b70 6172 616d 5d2c 2074 6774 5f63 7478  [param], tgt_ctx
-000146d0: 5b70 6172 616d 5d29 290a 2020 2020 2020  [param])).      
-000146e0: 2020 6966 2070 6861 7365 203d 3d20 313a    if phase == 1:
-000146f0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00014700: 6e6f 7420 6f73 2e70 6174 682e 6973 6469  not os.path.isdi
-00014710: 7228 7467 745f 6374 785b 2776 656e 765f  r(tgt_ctx['venv_
-00014720: 6f75 7061 7468 275d 293a 0a20 2020 2020  oupath']):.     
-00014730: 2020 2020 2020 2020 2020 206f 7330 2e77             os0.w
-00014740: 6c6f 6728 2744 6972 6563 746f 7279 2025  log('Directory %
-00014750: 7320 6e6f 7420 666f 756e 6421 2720 2520  s not found!' % 
-00014760: 7467 745f 6374 785b 2776 656e 765f 6f75  tgt_ctx['venv_ou
-00014770: 7061 7468 275d 290a 2020 2020 2020 2020  path']).        
-00014780: 2020 2020 2020 2020 6469 7361 626c 655f          disable_
-00014790: 7665 6e76 203d 2054 7275 650a 2020 2020  venv = True.    
-000147a0: 2020 2020 656c 6966 206e 6f74 2073 7263      elif not src
-000147b0: 5f63 7478 5b27 6472 795f 7275 6e27 5d3a  _ctx['dry_run']:
-000147c0: 0a20 2020 2020 2020 2020 2020 2064 726f  .            dro
-000147d0: 705f 6462 2873 7263 5f63 7478 2c20 7467  p_db(src_ctx, tg
-000147e0: 745f 6374 782c 2074 6774 5f63 7478 5b27  t_ctx, tgt_ctx['
-000147f0: 6462 5f6e 616d 6527 5d2c 0a20 2020 2020  db_name'],.     
-00014800: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00014810: 6577 5f64 626e 616d 6528 7372 635f 6374  ew_dbname(src_ct
-00014820: 785b 2764 625f 6e61 6d65 275d 2c0a 2020  x['db_name'],.  
+00013fa0: 2020 2020 2020 2074 6774 5f63 7478 5b27         tgt_ctx['
+00013fb0: 6462 5f6e 616d 6527 5d2c 2074 6774 5f63  db_name'], tgt_c
+00013fc0: 7478 5b27 6c6f 6766 696c 6527 5d29 0a20  tx['logfile']). 
+00013fd0: 2020 2062 6164 5f6d 6f64 756c 6573 203d     bad_modules =
+00013fe0: 2067 6574 5f77 726f 6e67 5f6d 6f64 756c   get_wrong_modul
+00013ff0: 6573 2874 6774 5f63 7478 290a 2020 2020  es(tgt_ctx).    
+00014000: 6966 2062 6164 5f6d 6f64 756c 6573 3a0a  if bad_modules:.
+00014010: 2020 2020 2020 2020 6f73 302e 776c 6f67          os0.wlog
+00014020: 2827 2a2a 2a20 556e 7374 6162 6c65 2044  ('*** Unstable D
+00014030: 4220 6166 7465 7220 636c 6561 6e3a 2077  B after clean: w
+00014040: 726f 6e67 206d 6f64 756c 6520 7374 6174  rong module stat
+00014050: 6520 2573 202a 2a2a 2720 250a 2020 2020  e %s ***' %.    
+00014060: 2020 2020 2020 2020 2020 2020 2062 6164               bad
+00014070: 5f6d 6f64 756c 6573 290a 2020 2020 2020  _modules).      
+00014080: 2020 6861 7264 5f75 6e69 6e73 7461 6c6c    hard_uninstall
+00014090: 5f6c 6973 7420 3d20 6c69 7374 280a 2020  _list = list(.  
+000140a0: 2020 2020 2020 2020 2020 7365 7428 6261            set(ba
+000140b0: 645f 6d6f 6475 6c65 7329 2026 2073 6574  d_modules) & set
+000140c0: 284d 4f44 554c 4553 5f32 5f4c 4541 5645  (MODULES_2_LEAVE
+000140d0: 5f42 4548 494e 4429 290a 2020 2020 2020  _BEHIND)).      
+000140e0: 2020 6261 645f 6d6f 6475 6c65 7320 3d20    bad_modules = 
+000140f0: 6c69 7374 280a 2020 2020 2020 2020 2020  list(.          
+00014100: 2020 7365 7428 6261 645f 6d6f 6475 6c65    set(bad_module
+00014110: 7329 202d 2073 6574 284d 4f44 554c 4553  s) - set(MODULES
+00014120: 5f32 5f4c 4541 5645 5f42 4548 494e 4429  _2_LEAVE_BEHIND)
+00014130: 290a 2020 2020 2020 2020 6966 2062 6164  ).        if bad
+00014140: 5f6d 6f64 756c 6573 3a0a 2020 2020 2020  _modules:.      
+00014150: 2020 2020 2020 7365 745f 756e 696e 7374        set_uninst
+00014160: 616c 6c65 645f 6279 5f73 716c 2874 6774  alled_by_sql(tgt
+00014170: 5f63 7478 2c20 6261 645f 6d6f 6475 6c65  _ctx, bad_module
+00014180: 7329 0a20 2020 2020 2020 2069 6620 6861  s).        if ha
+00014190: 7264 5f75 6e69 6e73 7461 6c6c 5f6c 6973  rd_uninstall_lis
+000141a0: 743a 0a20 2020 2020 2020 2020 2020 2066  t:.            f
+000141b0: 6f72 206d 6f64 756c 6520 696e 2068 6172  or module in har
+000141c0: 645f 756e 696e 7374 616c 6c5f 6c69 7374  d_uninstall_list
+000141d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000141e0: 2020 6f73 302e 776c 6f67 2827 2020 2b2b    os0.wlog('  ++
+000141f0: 2048 6172 6420 756e 696e 7374 616c 6c3a   Hard uninstall:
+00014200: 2025 7327 2025 206d 6f64 756c 6529 0a20   %s' % module). 
+00014210: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00014220: 6620 6e6f 7420 7372 635f 6374 785b 2764  f not src_ctx['d
+00014230: 7279 5f72 756e 275d 3a0a 2020 2020 2020  ry_run']:.      
+00014240: 2020 2020 2020 2020 2020 2020 2020 6861                ha
+00014250: 7264 5f63 6c65 616e 5f6d 6f64 756c 6528  rd_clean_module(
+00014260: 7467 745f 6374 782c 206d 6f64 756c 6529  tgt_ctx, module)
+00014270: 0a0a 2020 2020 6966 206e 6f74 2073 7263  ..    if not src
+00014280: 5f63 7478 5b27 6472 795f 7275 6e27 5d3a  _ctx['dry_run']:
+00014290: 0a20 2020 2020 2020 206f 7330 2e77 6c6f  .        os0.wlo
+000142a0: 6728 2754 6573 7420 636f 6e6e 6563 7469  g('Test connecti
+000142b0: 6f6e 2074 6f20 7461 7267 6574 2064 6220  on to target db 
+000142c0: 2573 2720 2520 7467 745f 6374 785b 2764  %s' % tgt_ctx['d
+000142d0: 625f 6e61 6d65 275d 290a 2020 2020 2020  b_name']).      
+000142e0: 2020 7569 642c 2074 6774 5f63 7478 203d    uid, tgt_ctx =
+000142f0: 2063 6c6f 646f 6f2e 6f65 7270 5f73 6574   clodoo.oerp_set
+00014300: 5f65 6e76 280a 2020 2020 2020 2020 2020  _env(.          
+00014310: 2020 6374 783d 7467 745f 6374 782c 2063    ctx=tgt_ctx, c
+00014320: 6f6e 666e 3d74 6774 5f66 756c 6c5f 6c63  onfn=tgt_full_lc
+00014330: 6f6e 662c 2064 623d 7467 745f 6374 785b  onf, db=tgt_ctx[
+00014340: 2764 625f 6e61 6d65 275d 290a 2020 2020  'db_name']).    
+00014350: 2020 2020 2320 4649 5820 6f65 7270 5f73      # FIX oerp_s
+00014360: 6574 5f65 6e76 2063 6861 6e67 6520 6472  et_env change dr
+00014370: 795f 7275 6e0a 2020 2020 2020 2020 7372  y_run.        sr
+00014380: 635f 6374 785b 2764 7279 5f72 756e 275d  c_ctx['dry_run']
+00014390: 203d 2074 6774 5f63 7478 5b27 6472 795f   = tgt_ctx['dry_
+000143a0: 7275 6e27 5d0a 0a20 2020 2072 6574 7572  run']..    retur
+000143b0: 6e20 7467 745f 6675 6c6c 5f6c 636f 6e66  n tgt_full_lconf
+000143c0: 0a0a 0a64 6566 206d 6967 7261 7465 5f64  ...def migrate_d
+000143d0: 6174 6162 6173 655f 7061 7373 2873 7263  atabase_pass(src
+000143e0: 5f63 7478 2c20 7467 745f 6374 782c 2070  _ctx, tgt_ctx, p
+000143f0: 6861 7365 3d4e 6f6e 6529 3a0a 2020 2020  hase=None):.    
+00014400: 7068 6173 6520 3d20 7068 6173 6520 6f72  phase = phase or
+00014410: 2032 0a20 2020 2064 6973 6162 6c65 5f76   2.    disable_v
+00014420: 656e 7620 3d20 4661 6c73 650a 2020 2020  env = False.    
+00014430: 6966 2070 6861 7365 203d 3d20 313a 0a20  if phase == 1:. 
+00014440: 2020 2020 2020 2073 6176 6564 5f64 7279         saved_dry
+00014450: 5f72 756e 203d 2073 7263 5f63 7478 5b27  _run = src_ctx['
+00014460: 6472 795f 7275 6e27 5d0a 2020 2020 2020  dry_run'].      
+00014470: 2020 7372 635f 6374 785b 2764 7279 5f72    src_ctx['dry_r
+00014480: 756e 275d 203d 2054 7275 650a 2020 2020  un'] = True.    
+00014490: 2020 2020 7467 745f 6374 785b 2764 7279      tgt_ctx['dry
+000144a0: 5f72 756e 275d 203d 2073 7263 5f63 7478  _run'] = src_ctx
+000144b0: 5b27 6472 795f 7275 6e27 5d0a 2020 2020  ['dry_run'].    
+000144c0: 7768 696c 6520 313a 0a20 2020 2020 2020  while 1:.       
+000144d0: 206f 7330 2e77 6c6f 6728 272d 2720 2a20   os0.wlog('-' * 
+000144e0: 3830 290a 2020 2020 2020 2020 7372 635f  80).        src_
+000144f0: 6374 782c 2074 6774 5f63 7478 2c20 7372  ctx, tgt_ctx, sr
+00014500: 635f 636f 6e66 6967 2c20 7467 745f 636f  c_config, tgt_co
+00014510: 6e66 6967 203d 2061 646a 7573 745f 6374  nfig = adjust_ct
+00014520: 7828 7372 635f 6374 782c 2074 6774 5f63  x(src_ctx, tgt_c
+00014530: 7478 290a 2020 2020 2020 2020 666f 7220  tx).        for 
+00014540: 7061 7261 6d20 696e 2028 2776 6964 272c  param in ('vid',
+00014550: 2027 6f64 6f6f 5f66 7665 7227 2c20 276f   'odoo_fver', 'o
+00014560: 646f 6f5f 7665 7227 293a 0a20 2020 2020  doo_ver'):.     
+00014570: 2020 2020 2020 206f 7330 2e77 6c6f 6728         os0.wlog(
+00014580: 2750 6173 7320 2564 206d 6967 7261 7469  'Pass %d migrati
+00014590: 6f6e 3a20 2573 2066 726f 6d20 2573 2074  on: %s from %s t
+000145a0: 6f20 2573 202e 2e27 2025 0a20 2020 2020  o %s ..' %.     
+000145b0: 2020 2020 2020 2020 2020 2020 2870 6861              (pha
+000145c0: 7365 2c20 7061 7261 6d2c 0a20 2020 2020  se, param,.     
+000145d0: 2020 2020 2020 2020 2020 2020 2073 7263               src
+000145e0: 5f63 7478 5b27 7372 635f 2573 2720 2520  _ctx['src_%s' % 
+000145f0: 7061 7261 6d5d 2c20 7467 745f 6374 785b  param], tgt_ctx[
+00014600: 2774 6774 5f25 7327 2025 2070 6172 616d  'tgt_%s' % param
+00014610: 5d29 290a 2020 2020 2020 2020 666f 7220  ])).        for 
+00014620: 7061 7261 6d20 696e 2028 2764 625f 6e61  param in ('db_na
+00014630: 6d65 272c 2027 636f 6e66 5f66 6e27 2c20  me', 'conf_fn', 
+00014640: 2778 6d6c 7270 635f 706f 7274 272c 2027  'xmlrpc_port', '
+00014650: 6462 5f75 7365 7227 293a 0a20 2020 2020  db_user'):.     
+00014660: 2020 2020 2020 206f 7330 2e77 6c6f 6728         os0.wlog(
+00014670: 2750 6173 7320 2564 206d 6967 7261 7469  'Pass %d migrati
+00014680: 6f6e 3a20 2573 2066 726f 6d20 2573 2074  on: %s from %s t
+00014690: 6f20 2573 202e 2e27 2025 0a20 2020 2020  o %s ..' %.     
+000146a0: 2020 2020 2020 2020 2020 2020 2870 6861              (pha
+000146b0: 7365 2c20 7061 7261 6d2c 2073 7263 5f63  se, param, src_c
+000146c0: 7478 5b70 6172 616d 5d2c 2074 6774 5f63  tx[param], tgt_c
+000146d0: 7478 5b70 6172 616d 5d29 290a 2020 2020  tx[param])).    
+000146e0: 2020 2020 6966 2070 6861 7365 203d 3d20      if phase == 
+000146f0: 313a 0a20 2020 2020 2020 2020 2020 2069  1:.            i
+00014700: 6620 6e6f 7420 6f73 2e70 6174 682e 6973  f not os.path.is
+00014710: 6469 7228 7467 745f 6374 785b 2776 656e  dir(tgt_ctx['ven
+00014720: 765f 6f75 7061 7468 275d 293a 0a20 2020  v_oupath']):.   
+00014730: 2020 2020 2020 2020 2020 2020 206f 7330               os0
+00014740: 2e77 6c6f 6728 2744 6972 6563 746f 7279  .wlog('Directory
+00014750: 2025 7320 6e6f 7420 666f 756e 6421 2720   %s not found!' 
+00014760: 2520 7467 745f 6374 785b 2776 656e 765f  % tgt_ctx['venv_
+00014770: 6f75 7061 7468 275d 290a 2020 2020 2020  oupath']).      
+00014780: 2020 2020 2020 2020 2020 6469 7361 626c            disabl
+00014790: 655f 7665 6e76 203d 2054 7275 650a 2020  e_venv = True.  
+000147a0: 2020 2020 2020 656c 6966 206e 6f74 2073        elif not s
+000147b0: 7263 5f63 7478 5b27 6472 795f 7275 6e27  rc_ctx['dry_run'
+000147c0: 5d3a 0a20 2020 2020 2020 2020 2020 2064  ]:.            d
+000147d0: 726f 705f 6462 2873 7263 5f63 7478 2c20  rop_db(src_ctx, 
+000147e0: 7467 745f 6374 782c 2074 6774 5f63 7478  tgt_ctx, tgt_ctx
+000147f0: 5b27 6462 5f6e 616d 6527 5d2c 0a20 2020  ['db_name'],.   
+00014800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014810: 206e 6577 5f64 626e 616d 6528 7372 635f   new_dbname(src_
+00014820: 6374 785b 2764 625f 6e61 6d65 275d 2c0a  ctx['db_name'],.
 00014830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014840: 2020 2020 2020 2020 2020 2020 2074 6774               tgt
-00014850: 5f63 7478 5b27 7467 745f 6f64 6f6f 5f76  _ctx['tgt_odoo_v
-00014860: 6572 275d 2c0a 2020 2020 2020 2020 2020  er'],.          
+00014840: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00014850: 6774 5f63 7478 5b27 7467 745f 6f64 6f6f  gt_ctx['tgt_odoo
+00014860: 5f76 6572 275d 2c0a 2020 2020 2020 2020  _ver'],.        
 00014870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014880: 2020 2020 2074 6774 5f63 7478 5b27 6f63       tgt_ctx['oc
-00014890: 615f 6d69 6772 6174 6527 5d29 290a 2020  a_migrate'])).  
-000148a0: 2020 2020 2020 6675 6c6c 5f6c 636f 6e66        full_lconf
-000148b0: 203d 206d 6967 7261 7465 5f6f 646f 6f28   = migrate_odoo(
-000148c0: 7372 635f 6374 782c 2074 6774 5f63 7478  src_ctx, tgt_ctx
-000148d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00014880: 2020 2020 2020 2074 6774 5f63 7478 5b27         tgt_ctx['
+00014890: 6f63 615f 6d69 6772 6174 6527 5d29 290a  oca_migrate'])).
+000148a0: 2020 2020 2020 2020 6675 6c6c 5f6c 636f          full_lco
+000148b0: 6e66 203d 206d 6967 7261 7465 5f6f 646f  nf = migrate_odo
+000148c0: 6f28 7372 635f 6374 782c 2074 6774 5f63  o(src_ctx, tgt_c
+000148d0: 7478 2c0a 2020 2020 2020 2020 2020 2020  tx,.            
 000148e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000148f0: 2020 2020 7372 635f 636f 6e66 6967 2c20      src_config, 
-00014900: 7467 745f 636f 6e66 6967 2c20 7068 6173  tgt_config, phas
-00014910: 653d 7068 6173 6529 0a20 2020 2020 2020  e=phase).       
-00014920: 2069 6620 7467 745f 6374 785b 2774 6774   if tgt_ctx['tgt
-00014930: 5f6f 646f 6f5f 7665 7227 5d20 3e3d 2073  _odoo_ver'] >= s
-00014940: 7263 5f63 7478 5b27 6669 6e61 6c5f 7665  rc_ctx['final_ve
-00014950: 7227 5d3a 0a20 2020 2020 2020 2020 2020  r']:.           
-00014960: 2069 6620 6469 7361 626c 655f 7665 6e76   if disable_venv
-00014970: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00014980: 2020 7372 635f 6374 785b 2776 656e 765f    src_ctx['venv_
-00014990: 6f75 7061 7468 275d 203d 2073 7263 5f63  oupath'] = src_c
-000149a0: 7478 5b27 6f70 745f 6f75 7061 7468 275d  tx['opt_oupath']
-000149b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000149c0: 2074 6774 5f63 7478 5b27 7665 6e76 5f6f   tgt_ctx['venv_o
-000149d0: 7570 6174 6827 5d20 3d20 7372 635f 6374  upath'] = src_ct
-000149e0: 785b 2776 656e 765f 6f75 7061 7468 275d  x['venv_oupath']
-000149f0: 0a20 2020 2020 2020 2020 2020 2062 7265  .            bre
-00014a00: 616b 0a20 2020 2020 2020 2069 6620 6e6f  ak.        if no
-00014a10: 7420 7372 635f 6374 785b 276e 6f5f 7665  t src_ctx['no_ve
-00014a20: 6e76 275d 2061 6e64 206e 6f74 2073 7263  nv'] and not src
-00014a30: 5f63 7478 5b27 6472 795f 7275 6e27 5d3a  _ctx['dry_run']:
-00014a40: 0a20 2020 2020 2020 2020 2020 2076 656e  .            ven
-00014a50: 765f 7061 7468 203d 206f 732e 7061 7468  v_path = os.path
-00014a60: 2e6a 6f69 6e28 7467 745f 6374 785b 2776  .join(tgt_ctx['v
-00014a70: 656e 765f 6f75 7061 7468 275d 2c20 276f  env_oupath'], 'o
-00014a80: 7065 6e75 7067 7261 6465 2729 0a20 2020  penupgrade').   
-00014a90: 2020 2020 2020 2020 2023 2054 4f44 4f0a           # TODO.
-00014aa0: 2020 2020 2020 2020 2020 2020 2320 6966              # if
-00014ab0: 206e 6f74 206f 732e 7061 7468 2e69 7364   not os.path.isd
-00014ac0: 6972 2876 656e 765f 7061 7468 293a 0a20  ir(venv_path):. 
-00014ad0: 2020 2020 2020 2020 2020 2023 2020 2020             #    
-00014ae0: 6f73 2e75 6e6c 696e 6b28 6f73 2e70 6174  os.unlink(os.pat
-00014af0: 682e 6a6f 696e 2876 656e 765f 7061 7468  h.join(venv_path
-00014b00: 2c20 6f75 5f76 6572 5f70 6174 6829 290a  , ou_ver_path)).
-00014b10: 2020 2020 2020 2020 7372 635f 6374 782c          src_ctx,
-00014b20: 2074 6774 5f63 7478 203d 2073 6869 6674   tgt_ctx = shift
-00014b30: 5f63 7478 2873 7263 5f63 7478 2c20 7467  _ctx(src_ctx, tg
-00014b40: 745f 6374 782c 2070 6861 7365 3d70 6861  t_ctx, phase=pha
-00014b50: 7365 290a 0a20 2020 2069 6620 7068 6173  se)..    if phas
-00014b60: 6520 3d3d 2031 3a0a 2020 2020 2020 2020  e == 1:.        
-00014b70: 7372 635f 6374 785b 2764 7279 5f72 756e  src_ctx['dry_run
-00014b80: 275d 203d 2073 6176 6564 5f64 7279 5f72  '] = saved_dry_r
-00014b90: 756e 0a20 2020 2020 2020 2074 6774 5f63  un.        tgt_c
-00014ba0: 7478 5b27 6472 795f 7275 6e27 5d20 3d20  tx['dry_run'] = 
-00014bb0: 7372 635f 6374 785b 2764 7279 5f72 756e  src_ctx['dry_run
-00014bc0: 275d 0a0a 0a64 6566 206d 6967 7261 7465  ']...def migrate
-00014bd0: 5f64 6174 6162 6173 6528 7372 635f 6374  _database(src_ct
-00014be0: 782c 2074 6774 5f63 7478 293a 0a20 2020  x, tgt_ctx):.   
-00014bf0: 2069 6620 7372 635f 6374 785b 2770 6861   if src_ctx['pha
-00014c00: 7365 5f31 275d 3a0a 2020 2020 2020 2020  se_1']:.        
-00014c10: 7372 635f 6374 7820 3d20 696e 6974 5f63  src_ctx = init_c
-00014c20: 7478 2873 7263 5f63 7478 290a 2020 2020  tx(src_ctx).    
-00014c30: 2020 2020 6d69 6772 6174 655f 6461 7461      migrate_data
-00014c40: 6261 7365 5f70 6173 7328 7372 635f 6374  base_pass(src_ct
-00014c50: 782c 2074 6774 5f63 7478 2c20 7068 6173  x, tgt_ctx, phas
-00014c60: 653d 3129 0a20 2020 2020 2020 2066 6f72  e=1).        for
-00014c70: 206e 6d20 696e 2028 276f 7269 6769 6e61   nm in ('origina
-00014c80: 6c5f 6d6f 6475 6c65 5f6c 6973 7427 2c29  l_module_list',)
-00014c90: 3a0a 2020 2020 2020 2020 2020 2020 6465  :.            de
-00014ca0: 6c20 7372 635f 6374 785b 6e6d 5d0a 2020  l src_ctx[nm].  
-00014cb0: 2020 7372 635f 6374 7820 3d20 696e 6974    src_ctx = init
-00014cc0: 5f63 7478 2873 7263 5f63 7478 290a 2020  _ctx(src_ctx).  
-00014cd0: 2020 6d69 6772 6174 655f 6461 7461 6261    migrate_databa
-00014ce0: 7365 5f70 6173 7328 7372 635f 6374 782c  se_pass(src_ctx,
-00014cf0: 2074 6774 5f63 7478 2c20 7068 6173 653d   tgt_ctx, phase=
-00014d00: 3229 0a20 2020 2070 7269 6e74 2827 4461  2).    print('Da
-00014d10: 7461 6261 7365 2025 7320 7375 6363 6573  tabase %s succes
-00014d20: 7366 756c 6c79 206d 696f 6772 6174 6564  sfully miograted
-00014d30: 2069 6e74 6f20 2573 2720 2520 280a 2020   into %s' % (.  
-00014d40: 2020 2020 2020 7372 635f 6374 785b 2766        src_ctx['f
-00014d50: 726f 6d5f 6462 6e61 6d65 275d 2c20 7467  rom_dbname'], tg
-00014d60: 745f 6374 785b 2764 625f 6e61 6d65 275d  t_ctx['db_name']
-00014d70: 2929 0a0a 0a64 6566 2070 6172 7365 5f63  ))...def parse_c
-00014d80: 7478 2873 7263 5f63 7478 293a 0a20 2020  tx(src_ctx):.   
-00014d90: 2067 6c6f 6261 6c20 4445 465f 434f 4e46   global DEF_CONF
-00014da0: 0a20 2020 2069 6620 6e6f 7420 7372 635f  .    if not src_
-00014db0: 6374 785b 2766 726f 6d5f 6272 616e 6368  ctx['from_branch
-00014dc0: 275d 2061 6e64 206e 6f74 2073 7263 5f63  '] and not src_c
-00014dd0: 7478 5b27 6672 6f6d 5f63 6f6e 666e 275d  tx['from_confn']
-00014de0: 3a0a 2020 2020 2020 2020 7261 6973 6520  :.        raise 
-00014df0: 4b65 7945 7272 6f72 2827 4d69 7373 6564  KeyError('Missed
-00014e00: 206f 7269 6769 6e61 6c20 6f64 6f6f 2076   original odoo v
-00014e10: 6572 7369 6f6e 2120 506c 6561 7365 2075  ersion! Please u
-00014e20: 7365 202d 4620 7377 6974 6368 2729 0a20  se -F switch'). 
-00014e30: 2020 2065 6c69 6620 7372 635f 6374 785b     elif src_ctx[
-00014e40: 2766 726f 6d5f 6272 616e 6368 275d 3a0a  'from_branch']:.
-00014e50: 2020 2020 2020 2020 7372 635f 6374 785b          src_ctx[
-00014e60: 2773 7263 5f6f 646f 6f5f 6676 6572 275d  'src_odoo_fver']
-00014e70: 203d 2063 6c6f 646f 6f2e 6275 696c 645f   = clodoo.build_
-00014e80: 6f64 6f6f 5f70 6172 616d 280a 2020 2020  odoo_param(.    
-00014e90: 2020 2020 2020 2020 2746 554c 4c56 4552          'FULLVER
-00014ea0: 272c 206f 646f 6f5f 7669 643d 7372 635f  ', odoo_vid=src_
-00014eb0: 6374 785b 2766 726f 6d5f 6272 616e 6368  ctx['from_branch
-00014ec0: 275d 2c20 6d75 6c74 693d 5472 7565 290a  '], multi=True).
-00014ed0: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
-00014ee0: 7263 5f63 7478 5b27 6672 6f6d 5f63 6f6e  rc_ctx['from_con
-00014ef0: 666e 275d 3a0a 2020 2020 2020 2020 2020  fn']:.          
-00014f00: 2020 7372 635f 6374 785b 2766 726f 6d5f    src_ctx['from_
-00014f10: 636f 6e66 6e27 5d20 3d20 636c 6f64 6f6f  confn'] = clodoo
-00014f20: 2e62 7569 6c64 5f6f 646f 6f5f 7061 7261  .build_odoo_para
-00014f30: 6d28 0a20 2020 2020 2020 2020 2020 2020  m(.             
-00014f40: 2020 2027 434f 4e46 4e27 2c20 6f64 6f6f     'CONFN', odoo
-00014f50: 5f76 6964 3d73 7263 5f63 7478 5b27 6672  _vid=src_ctx['fr
-00014f60: 6f6d 5f62 7261 6e63 6827 5d2c 206d 756c  om_branch'], mul
-00014f70: 7469 3d54 7275 6529 0a20 2020 2069 6620  ti=True).    if 
-00014f80: 6e6f 7420 6f73 2e70 6174 682e 6973 6669  not os.path.isfi
-00014f90: 6c65 2873 7263 5f63 7478 5b27 6672 6f6d  le(src_ctx['from
-00014fa0: 5f63 6f6e 666e 275d 293a 0a20 2020 2020  _confn']):.     
-00014fb0: 2020 2072 6169 7365 2049 4f45 7272 6f72     raise IOError
-00014fc0: 2827 4669 6c65 2025 7320 6e6f 7420 666f  ('File %s not fo
-00014fd0: 756e 6427 2025 2073 7263 5f63 7478 5b27  und' % src_ctx['
-00014fe0: 6672 6f6d 5f63 6f6e 666e 275d 290a 2020  from_confn']).  
-00014ff0: 2020 6966 206e 6f74 2073 7263 5f63 7478    if not src_ctx
-00015000: 5b27 6672 6f6d 5f62 7261 6e63 6827 5d3a  ['from_branch']:
-00015010: 0a20 2020 2020 2020 2073 7263 5f63 6f6e  .        src_con
-00015020: 6669 6720 3d20 436f 6e66 6967 5061 7273  fig = ConfigPars
-00015030: 6572 2e53 6166 6543 6f6e 6669 6750 6172  er.SafeConfigPar
-00015040: 7365 7228 290a 2020 2020 2020 2020 7372  ser().        sr
-00015050: 635f 636f 6e66 6967 2e72 6561 6428 7372  c_config.read(sr
-00015060: 635f 6374 785b 2766 726f 6d5f 636f 6e66  c_ctx['from_conf
-00015070: 6e27 5d29 0a20 2020 2020 2020 2073 7263  n']).        src
-00015080: 5f63 7478 5b27 7372 635f 6f64 6f6f 5f66  _ctx['src_odoo_f
-00015090: 7665 7227 5d20 3d20 7372 635f 636f 6e66  ver'] = src_conf
-000150a0: 6967 2e67 6574 2827 6f70 7469 6f6e 7327  ig.get('options'
-000150b0: 2c20 276f 655f 7665 7273 696f 6e27 290a  , 'oe_version').
-000150c0: 2020 2020 2020 2020 7372 635f 6374 785b          src_ctx[
-000150d0: 2766 726f 6d5f 6272 616e 6368 275d 203d  'from_branch'] =
-000150e0: 2073 7263 5f63 7478 5b27 7372 635f 6f64   src_ctx['src_od
-000150f0: 6f6f 5f66 7665 7227 5d0a 2020 2020 7372  oo_fver'].    sr
-00015100: 635f 6374 785b 2773 7263 5f6f 646f 6f5f  c_ctx['src_odoo_
-00015110: 7665 7227 5d20 3d20 636c 6f64 6f6f 2e62  ver'] = clodoo.b
-00015120: 7569 6c64 5f6f 646f 6f5f 7061 7261 6d28  uild_odoo_param(
-00015130: 0a20 2020 2020 2020 2020 2020 2027 4d41  .            'MA
-00015140: 4a56 4552 272c 206f 646f 6f5f 7669 643d  JVER', odoo_vid=
-00015150: 7372 635f 6374 785b 2766 726f 6d5f 6272  src_ctx['from_br
-00015160: 616e 6368 275d 2c20 6d75 6c74 693d 5472  anch'], multi=Tr
-00015170: 7565 290a 0a20 2020 2069 6620 6e6f 7420  ue)..    if not 
-00015180: 7372 635f 6374 785b 2766 696e 616c 5f62  src_ctx['final_b
-00015190: 7261 6e63 6827 5d20 616e 6420 6e6f 7420  ranch'] and not 
-000151a0: 7372 635f 6374 785b 2766 696e 616c 5f63  src_ctx['final_c
-000151b0: 6f6e 666e 275d 3a0a 2020 2020 2020 2020  onfn']:.        
-000151c0: 7261 6973 6520 4b65 7945 7272 6f72 2827  raise KeyError('
-000151d0: 4d69 7373 6564 2066 696e 616c 206f 646f  Missed final odo
-000151e0: 6f20 7665 7273 696f 6e21 2050 6c65 6173  o version! Pleas
-000151f0: 6520 7573 6520 2d62 2073 7769 7463 6827  e use -b switch'
-00015200: 290a 2020 2020 656c 6966 2073 7263 5f63  ).    elif src_c
-00015210: 7478 5b27 6669 6e61 6c5f 6272 616e 6368  tx['final_branch
-00015220: 275d 3a0a 2020 2020 2020 2020 7372 635f  ']:.        src_
-00015230: 6374 785b 2774 6774 5f6f 646f 6f5f 6676  ctx['tgt_odoo_fv
-00015240: 6572 275d 203d 2063 6c6f 646f 6f2e 6275  er'] = clodoo.bu
-00015250: 696c 645f 6f64 6f6f 5f70 6172 616d 280a  ild_odoo_param(.
-00015260: 2020 2020 2020 2020 2020 2020 2746 554c              'FUL
-00015270: 4c56 4552 272c 206f 646f 6f5f 7669 643d  LVER', odoo_vid=
-00015280: 7372 635f 6374 785b 2766 696e 616c 5f62  src_ctx['final_b
-00015290: 7261 6e63 6827 5d2c 206d 756c 7469 3d54  ranch'], multi=T
-000152a0: 7275 6529 0a20 2020 2020 2020 2069 6620  rue).        if 
-000152b0: 6e6f 7420 7372 635f 6374 785b 2766 696e  not src_ctx['fin
-000152c0: 616c 5f63 6f6e 666e 275d 3a0a 2020 2020  al_confn']:.    
-000152d0: 2020 2020 2020 2020 7372 635f 6374 785b          src_ctx[
-000152e0: 2766 696e 616c 5f63 6f6e 666e 275d 203d  'final_confn'] =
-000152f0: 2063 6c6f 646f 6f2e 6275 696c 645f 6f64   clodoo.build_od
-00015300: 6f6f 5f70 6172 616d 280a 2020 2020 2020  oo_param(.      
-00015310: 2020 2020 2020 2020 2020 2743 4f4e 464e            'CONFN
-00015320: 272c 206f 646f 6f5f 7669 643d 7372 635f  ', odoo_vid=src_
-00015330: 6374 785b 2766 696e 616c 5f62 7261 6e63  ctx['final_branc
-00015340: 6827 5d2c 206d 756c 7469 3d54 7275 6529  h'], multi=True)
-00015350: 0a20 2020 2069 6620 6e6f 7420 6f73 2e70  .    if not os.p
-00015360: 6174 682e 6973 6669 6c65 2873 7263 5f63  ath.isfile(src_c
-00015370: 7478 5b27 6669 6e61 6c5f 636f 6e66 6e27  tx['final_confn'
-00015380: 5d29 3a0a 2020 2020 2020 2020 7261 6973  ]):.        rais
-00015390: 6520 494f 4572 726f 7228 2746 696c 6520  e IOError('File 
-000153a0: 2573 206e 6f74 2066 6f75 6e64 2720 2520  %s not found' % 
-000153b0: 7372 635f 6374 785b 2766 696e 616c 5f63  src_ctx['final_c
-000153c0: 6f6e 666e 275d 290a 2020 2020 6966 206e  onfn']).    if n
-000153d0: 6f74 2073 7263 5f63 7478 5b27 6669 6e61  ot src_ctx['fina
-000153e0: 6c5f 6272 616e 6368 275d 3a0a 2020 2020  l_branch']:.    
-000153f0: 2020 2020 7467 745f 636f 6e66 6967 203d      tgt_config =
-00015400: 2043 6f6e 6669 6750 6172 7365 722e 5361   ConfigParser.Sa
-00015410: 6665 436f 6e66 6967 5061 7273 6572 2829  feConfigParser()
-00015420: 0a20 2020 2020 2020 2074 6774 5f63 6f6e  .        tgt_con
-00015430: 6669 672e 7265 6164 2873 7263 5f63 7478  fig.read(src_ctx
-00015440: 5b27 6669 6e61 6c5f 636f 6e66 6e27 5d29  ['final_confn'])
-00015450: 0a20 2020 2020 2020 2073 7263 5f63 7478  .        src_ctx
-00015460: 5b27 7467 745f 6f64 6f6f 5f66 7665 7227  ['tgt_odoo_fver'
-00015470: 5d20 3d20 7467 745f 636f 6e66 6967 2e67  ] = tgt_config.g
-00015480: 6574 2827 6f70 7469 6f6e 7327 2c20 276f  et('options', 'o
-00015490: 655f 7665 7273 696f 6e27 290a 2020 2020  e_version').    
-000154a0: 2020 2020 7372 635f 6374 785b 2766 696e      src_ctx['fin
-000154b0: 616c 5f62 7261 6e63 6827 5d20 3d20 7372  al_branch'] = sr
-000154c0: 635f 6374 785b 2774 6774 5f6f 646f 6f5f  c_ctx['tgt_odoo_
-000154d0: 6676 6572 275d 0a20 2020 2073 7263 5f63  fver'].    src_c
-000154e0: 7478 5b27 7467 745f 6f64 6f6f 5f76 6572  tx['tgt_odoo_ver
-000154f0: 275d 203d 2063 6c6f 646f 6f2e 6275 696c  '] = clodoo.buil
-00015500: 645f 6f64 6f6f 5f70 6172 616d 280a 2020  d_odoo_param(.  
-00015510: 2020 2020 2020 2020 2020 274d 414a 5645            'MAJVE
-00015520: 5227 2c20 6f64 6f6f 5f76 6964 3d73 7263  R', odoo_vid=src
-00015530: 5f63 7478 5b27 6669 6e61 6c5f 6272 616e  _ctx['final_bran
-00015540: 6368 275d 2c20 6d75 6c74 693d 5472 7565  ch'], multi=True
-00015550: 290a 0a20 2020 2069 6620 2828 7372 635f  )..    if ((src_
-00015560: 6374 785b 2773 7263 5f6f 646f 6f5f 7665  ctx['src_odoo_ve
-00015570: 7227 5d20 3e3d 2073 7263 5f63 7478 5b27  r'] >= src_ctx['
-00015580: 7467 745f 6f64 6f6f 5f76 6572 275d 2061  tgt_odoo_ver'] a
-00015590: 6e64 0a20 2020 2020 2020 2020 2020 206e  nd.            n
-000155a0: 6f74 2073 7263 5f63 7478 5b27 7365 6c5f  ot src_ctx['sel_
-000155b0: 6d6f 6465 6c27 5d29 206f 720a 2020 2020  model']) or.    
-000155c0: 2020 2020 2873 7263 5f63 7478 5b27 7372      (src_ctx['sr
-000155d0: 635f 6f64 6f6f 5f76 6572 275d 203e 2073  c_odoo_ver'] > s
-000155e0: 7263 5f63 7478 5b27 7467 745f 6f64 6f6f  rc_ctx['tgt_odoo
-000155f0: 5f76 6572 275d 2061 6e64 0a20 2020 2020  _ver'] and.     
-00015600: 2020 2020 2020 2073 7263 5f63 7478 5b27         src_ctx['
-00015610: 7365 6c5f 6d6f 6465 6c27 5d29 293a 0a20  sel_model'])):. 
-00015620: 2020 2020 2020 2072 6169 7365 204b 6579         raise Key
-00015630: 4572 726f 7228 2746 696e 616c 2076 6572  Error('Final ver
-00015640: 7369 6f6e 206d 7573 7420 6265 2067 7265  sion must be gre
-00015650: 6174 6572 2074 6861 6e20 6f72 6967 696e  ater than origin
-00015660: 616c 2076 6572 7369 6f6e 2729 0a0a 2020  al version')..  
-00015670: 2020 6966 206e 6f74 2073 7263 5f63 7478    if not src_ctx
-00015680: 5b27 6f70 745f 6f75 7061 7468 275d 3a0a  ['opt_oupath']:.
-00015690: 2020 2020 2020 2020 7372 635f 6374 785b          src_ctx[
-000156a0: 276f 7074 5f6f 7570 6174 6827 5d20 3d20  'opt_oupath'] = 
-000156b0: 6f73 2e70 6174 682e 6a6f 696e 286f 732e  os.path.join(os.
-000156c0: 7061 7468 2e65 7870 616e 6475 7365 7228  path.expanduser(
-000156d0: 277e 2729 2c20 2774 6d70 2729 0a20 2020  '~'), 'tmp').   
-000156e0: 2069 6620 6e6f 7420 7372 635f 6374 785b   if not src_ctx[
-000156f0: 276f 7074 5f6f 756c 7061 7468 275d 3a0a  'opt_oulpath']:.
-00015700: 2020 2020 2020 2020 7372 635f 6374 785b          src_ctx[
-00015710: 276f 7074 5f6f 756c 7061 7468 275d 203d  'opt_oulpath'] =
-00015720: 206f 732e 7061 7468 2e6a 6f69 6e28 7372   os.path.join(sr
-00015730: 635f 6374 785b 276f 7074 5f6f 7570 6174  c_ctx['opt_oupat
-00015740: 6827 5d2c 0a20 2020 2020 2020 2020 2020  h'],.           
+000148f0: 2020 2020 2020 7372 635f 636f 6e66 6967        src_config
+00014900: 2c20 7467 745f 636f 6e66 6967 2c20 7068  , tgt_config, ph
+00014910: 6173 653d 7068 6173 6529 0a20 2020 2020  ase=phase).     
+00014920: 2020 2069 6620 7467 745f 6374 785b 2774     if tgt_ctx['t
+00014930: 6774 5f6f 646f 6f5f 7665 7227 5d20 3e3d  gt_odoo_ver'] >=
+00014940: 2073 7263 5f63 7478 5b27 6669 6e61 6c5f   src_ctx['final_
+00014950: 7665 7227 5d3a 0a20 2020 2020 2020 2020  ver']:.         
+00014960: 2020 2069 6620 6469 7361 626c 655f 7665     if disable_ve
+00014970: 6e76 3a0a 2020 2020 2020 2020 2020 2020  nv:.            
+00014980: 2020 2020 7372 635f 6374 785b 2776 656e      src_ctx['ven
+00014990: 765f 6f75 7061 7468 275d 203d 2073 7263  v_oupath'] = src
+000149a0: 5f63 7478 5b27 6f70 745f 6f75 7061 7468  _ctx['opt_oupath
+000149b0: 275d 0a20 2020 2020 2020 2020 2020 2020  '].             
+000149c0: 2020 2074 6774 5f63 7478 5b27 7665 6e76     tgt_ctx['venv
+000149d0: 5f6f 7570 6174 6827 5d20 3d20 7372 635f  _oupath'] = src_
+000149e0: 6374 785b 2776 656e 765f 6f75 7061 7468  ctx['venv_oupath
+000149f0: 275d 0a20 2020 2020 2020 2020 2020 2062  '].            b
+00014a00: 7265 616b 0a20 2020 2020 2020 2069 6620  reak.        if 
+00014a10: 6e6f 7420 7372 635f 6374 785b 276e 6f5f  not src_ctx['no_
+00014a20: 7665 6e76 275d 2061 6e64 206e 6f74 2073  venv'] and not s
+00014a30: 7263 5f63 7478 5b27 6472 795f 7275 6e27  rc_ctx['dry_run'
+00014a40: 5d3a 0a20 2020 2020 2020 2020 2020 2076  ]:.            v
+00014a50: 656e 765f 7061 7468 203d 206f 732e 7061  env_path = os.pa
+00014a60: 7468 2e6a 6f69 6e28 7467 745f 6374 785b  th.join(tgt_ctx[
+00014a70: 2776 656e 765f 6f75 7061 7468 275d 2c20  'venv_oupath'], 
+00014a80: 276f 7065 6e75 7067 7261 6465 2729 0a20  'openupgrade'). 
+00014a90: 2020 2020 2020 2020 2020 2023 2054 4f44             # TOD
+00014aa0: 4f0a 2020 2020 2020 2020 2020 2020 2320  O.            # 
+00014ab0: 6966 206e 6f74 206f 732e 7061 7468 2e69  if not os.path.i
+00014ac0: 7364 6972 2876 656e 765f 7061 7468 293a  sdir(venv_path):
+00014ad0: 0a20 2020 2020 2020 2020 2020 2023 2020  .            #  
+00014ae0: 2020 6f73 2e75 6e6c 696e 6b28 6f73 2e70    os.unlink(os.p
+00014af0: 6174 682e 6a6f 696e 2876 656e 765f 7061  ath.join(venv_pa
+00014b00: 7468 2c20 6f75 5f76 6572 5f70 6174 6829  th, ou_ver_path)
+00014b10: 290a 2020 2020 2020 2020 7372 635f 6374  ).        src_ct
+00014b20: 782c 2074 6774 5f63 7478 203d 2073 6869  x, tgt_ctx = shi
+00014b30: 6674 5f63 7478 2873 7263 5f63 7478 2c20  ft_ctx(src_ctx, 
+00014b40: 7467 745f 6374 782c 2070 6861 7365 3d70  tgt_ctx, phase=p
+00014b50: 6861 7365 290a 0a20 2020 2069 6620 7068  hase)..    if ph
+00014b60: 6173 6520 3d3d 2031 3a0a 2020 2020 2020  ase == 1:.      
+00014b70: 2020 7372 635f 6374 785b 2764 7279 5f72    src_ctx['dry_r
+00014b80: 756e 275d 203d 2073 6176 6564 5f64 7279  un'] = saved_dry
+00014b90: 5f72 756e 0a20 2020 2020 2020 2074 6774  _run.        tgt
+00014ba0: 5f63 7478 5b27 6472 795f 7275 6e27 5d20  _ctx['dry_run'] 
+00014bb0: 3d20 7372 635f 6374 785b 2764 7279 5f72  = src_ctx['dry_r
+00014bc0: 756e 275d 0a0a 0a64 6566 206d 6967 7261  un']...def migra
+00014bd0: 7465 5f64 6174 6162 6173 6528 7372 635f  te_database(src_
+00014be0: 6374 782c 2074 6774 5f63 7478 293a 0a20  ctx, tgt_ctx):. 
+00014bf0: 2020 2069 6620 7372 635f 6374 785b 2770     if src_ctx['p
+00014c00: 6861 7365 5f31 275d 3a0a 2020 2020 2020  hase_1']:.      
+00014c10: 2020 7372 635f 6374 7820 3d20 696e 6974    src_ctx = init
+00014c20: 5f63 7478 2873 7263 5f63 7478 290a 2020  _ctx(src_ctx).  
+00014c30: 2020 2020 2020 6d69 6772 6174 655f 6461        migrate_da
+00014c40: 7461 6261 7365 5f70 6173 7328 7372 635f  tabase_pass(src_
+00014c50: 6374 782c 2074 6774 5f63 7478 2c20 7068  ctx, tgt_ctx, ph
+00014c60: 6173 653d 3129 0a20 2020 2020 2020 2066  ase=1).        f
+00014c70: 6f72 206e 6d20 696e 2028 276f 7269 6769  or nm in ('origi
+00014c80: 6e61 6c5f 6d6f 6475 6c65 5f6c 6973 7427  nal_module_list'
+00014c90: 2c29 3a0a 2020 2020 2020 2020 2020 2020  ,):.            
+00014ca0: 6465 6c20 7372 635f 6374 785b 6e6d 5d0a  del src_ctx[nm].
+00014cb0: 2020 2020 7372 635f 6374 7820 3d20 696e      src_ctx = in
+00014cc0: 6974 5f63 7478 2873 7263 5f63 7478 290a  it_ctx(src_ctx).
+00014cd0: 2020 2020 6d69 6772 6174 655f 6461 7461      migrate_data
+00014ce0: 6261 7365 5f70 6173 7328 7372 635f 6374  base_pass(src_ct
+00014cf0: 782c 2074 6774 5f63 7478 2c20 7068 6173  x, tgt_ctx, phas
+00014d00: 653d 3229 0a20 2020 2070 7269 6e74 2827  e=2).    print('
+00014d10: 4461 7461 6261 7365 2025 7320 7375 6363  Database %s succ
+00014d20: 6573 7366 756c 6c79 206d 696f 6772 6174  essfully miograt
+00014d30: 6564 2069 6e74 6f20 2573 2720 2520 280a  ed into %s' % (.
+00014d40: 2020 2020 2020 2020 7372 635f 6374 785b          src_ctx[
+00014d50: 2766 726f 6d5f 6462 6e61 6d65 275d 2c20  'from_dbname'], 
+00014d60: 7467 745f 6374 785b 2764 625f 6e61 6d65  tgt_ctx['db_name
+00014d70: 275d 2929 0a0a 0a64 6566 2070 6172 7365  ']))...def parse
+00014d80: 5f63 7478 2873 7263 5f63 7478 293a 0a20  _ctx(src_ctx):. 
+00014d90: 2020 2067 6c6f 6261 6c20 4445 465f 434f     global DEF_CO
+00014da0: 4e46 0a20 2020 2069 6620 6e6f 7420 7372  NF.    if not sr
+00014db0: 635f 6374 785b 2766 726f 6d5f 6272 616e  c_ctx['from_bran
+00014dc0: 6368 275d 2061 6e64 206e 6f74 2073 7263  ch'] and not src
+00014dd0: 5f63 7478 5b27 6672 6f6d 5f63 6f6e 666e  _ctx['from_confn
+00014de0: 275d 3a0a 2020 2020 2020 2020 7261 6973  ']:.        rais
+00014df0: 6520 4b65 7945 7272 6f72 2827 4d69 7373  e KeyError('Miss
+00014e00: 6564 206f 7269 6769 6e61 6c20 6f64 6f6f  ed original odoo
+00014e10: 2076 6572 7369 6f6e 2120 506c 6561 7365   version! Please
+00014e20: 2075 7365 202d 4620 7377 6974 6368 2729   use -F switch')
+00014e30: 0a20 2020 2065 6c69 6620 7372 635f 6374  .    elif src_ct
+00014e40: 785b 2766 726f 6d5f 6272 616e 6368 275d  x['from_branch']
+00014e50: 3a0a 2020 2020 2020 2020 7372 635f 6374  :.        src_ct
+00014e60: 785b 2773 7263 5f6f 646f 6f5f 6676 6572  x['src_odoo_fver
+00014e70: 275d 203d 2063 6c6f 646f 6f2e 6275 696c  '] = clodoo.buil
+00014e80: 645f 6f64 6f6f 5f70 6172 616d 280a 2020  d_odoo_param(.  
+00014e90: 2020 2020 2020 2020 2020 2746 554c 4c56            'FULLV
+00014ea0: 4552 272c 206f 646f 6f5f 7669 643d 7372  ER', odoo_vid=sr
+00014eb0: 635f 6374 785b 2766 726f 6d5f 6272 616e  c_ctx['from_bran
+00014ec0: 6368 275d 2c20 6d75 6c74 693d 5472 7565  ch'], multi=True
+00014ed0: 290a 2020 2020 2020 2020 6966 206e 6f74  ).        if not
+00014ee0: 2073 7263 5f63 7478 5b27 6672 6f6d 5f63   src_ctx['from_c
+00014ef0: 6f6e 666e 275d 3a0a 2020 2020 2020 2020  onfn']:.        
+00014f00: 2020 2020 7372 635f 6374 785b 2766 726f      src_ctx['fro
+00014f10: 6d5f 636f 6e66 6e27 5d20 3d20 636c 6f64  m_confn'] = clod
+00014f20: 6f6f 2e62 7569 6c64 5f6f 646f 6f5f 7061  oo.build_odoo_pa
+00014f30: 7261 6d28 0a20 2020 2020 2020 2020 2020  ram(.           
+00014f40: 2020 2020 2027 434f 4e46 4e27 2c20 6f64       'CONFN', od
+00014f50: 6f6f 5f76 6964 3d73 7263 5f63 7478 5b27  oo_vid=src_ctx['
+00014f60: 6672 6f6d 5f62 7261 6e63 6827 5d2c 206d  from_branch'], m
+00014f70: 756c 7469 3d54 7275 6529 0a20 2020 2069  ulti=True).    i
+00014f80: 6620 6e6f 7420 6f73 2e70 6174 682e 6973  f not os.path.is
+00014f90: 6669 6c65 2873 7263 5f63 7478 5b27 6672  file(src_ctx['fr
+00014fa0: 6f6d 5f63 6f6e 666e 275d 293a 0a20 2020  om_confn']):.   
+00014fb0: 2020 2020 2072 6169 7365 2049 4f45 7272       raise IOErr
+00014fc0: 6f72 2827 4669 6c65 2025 7320 6e6f 7420  or('File %s not 
+00014fd0: 666f 756e 6427 2025 2073 7263 5f63 7478  found' % src_ctx
+00014fe0: 5b27 6672 6f6d 5f63 6f6e 666e 275d 290a  ['from_confn']).
+00014ff0: 2020 2020 6966 206e 6f74 2073 7263 5f63      if not src_c
+00015000: 7478 5b27 6672 6f6d 5f62 7261 6e63 6827  tx['from_branch'
+00015010: 5d3a 0a20 2020 2020 2020 2073 7263 5f63  ]:.        src_c
+00015020: 6f6e 6669 6720 3d20 436f 6e66 6967 5061  onfig = ConfigPa
+00015030: 7273 6572 2e53 6166 6543 6f6e 6669 6750  rser.SafeConfigP
+00015040: 6172 7365 7228 290a 2020 2020 2020 2020  arser().        
+00015050: 7372 635f 636f 6e66 6967 2e72 6561 6428  src_config.read(
+00015060: 7372 635f 6374 785b 2766 726f 6d5f 636f  src_ctx['from_co
+00015070: 6e66 6e27 5d29 0a20 2020 2020 2020 2073  nfn']).        s
+00015080: 7263 5f63 7478 5b27 7372 635f 6f64 6f6f  rc_ctx['src_odoo
+00015090: 5f66 7665 7227 5d20 3d20 7372 635f 636f  _fver'] = src_co
+000150a0: 6e66 6967 2e67 6574 2827 6f70 7469 6f6e  nfig.get('option
+000150b0: 7327 2c20 276f 655f 7665 7273 696f 6e27  s', 'oe_version'
+000150c0: 290a 2020 2020 2020 2020 7372 635f 6374  ).        src_ct
+000150d0: 785b 2766 726f 6d5f 6272 616e 6368 275d  x['from_branch']
+000150e0: 203d 2073 7263 5f63 7478 5b27 7372 635f   = src_ctx['src_
+000150f0: 6f64 6f6f 5f66 7665 7227 5d0a 2020 2020  odoo_fver'].    
+00015100: 7372 635f 6374 785b 2773 7263 5f6f 646f  src_ctx['src_odo
+00015110: 6f5f 7665 7227 5d20 3d20 636c 6f64 6f6f  o_ver'] = clodoo
+00015120: 2e62 7569 6c64 5f6f 646f 6f5f 7061 7261  .build_odoo_para
+00015130: 6d28 0a20 2020 2020 2020 2020 2020 2027  m(.            '
+00015140: 4d41 4a56 4552 272c 206f 646f 6f5f 7669  MAJVER', odoo_vi
+00015150: 643d 7372 635f 6374 785b 2766 726f 6d5f  d=src_ctx['from_
+00015160: 6272 616e 6368 275d 2c20 6d75 6c74 693d  branch'], multi=
+00015170: 5472 7565 290a 0a20 2020 2069 6620 6e6f  True)..    if no
+00015180: 7420 7372 635f 6374 785b 2766 696e 616c  t src_ctx['final
+00015190: 5f62 7261 6e63 6827 5d20 616e 6420 6e6f  _branch'] and no
+000151a0: 7420 7372 635f 6374 785b 2766 696e 616c  t src_ctx['final
+000151b0: 5f63 6f6e 666e 275d 3a0a 2020 2020 2020  _confn']:.      
+000151c0: 2020 7261 6973 6520 4b65 7945 7272 6f72    raise KeyError
+000151d0: 2827 4d69 7373 6564 2066 696e 616c 206f  ('Missed final o
+000151e0: 646f 6f20 7665 7273 696f 6e21 2050 6c65  doo version! Ple
+000151f0: 6173 6520 7573 6520 2d62 2073 7769 7463  ase use -b switc
+00015200: 6827 290a 2020 2020 656c 6966 2073 7263  h').    elif src
+00015210: 5f63 7478 5b27 6669 6e61 6c5f 6272 616e  _ctx['final_bran
+00015220: 6368 275d 3a0a 2020 2020 2020 2020 7372  ch']:.        sr
+00015230: 635f 6374 785b 2774 6774 5f6f 646f 6f5f  c_ctx['tgt_odoo_
+00015240: 6676 6572 275d 203d 2063 6c6f 646f 6f2e  fver'] = clodoo.
+00015250: 6275 696c 645f 6f64 6f6f 5f70 6172 616d  build_odoo_param
+00015260: 280a 2020 2020 2020 2020 2020 2020 2746  (.            'F
+00015270: 554c 4c56 4552 272c 206f 646f 6f5f 7669  ULLVER', odoo_vi
+00015280: 643d 7372 635f 6374 785b 2766 696e 616c  d=src_ctx['final
+00015290: 5f62 7261 6e63 6827 5d2c 206d 756c 7469  _branch'], multi
+000152a0: 3d54 7275 6529 0a20 2020 2020 2020 2069  =True).        i
+000152b0: 6620 6e6f 7420 7372 635f 6374 785b 2766  f not src_ctx['f
+000152c0: 696e 616c 5f63 6f6e 666e 275d 3a0a 2020  inal_confn']:.  
+000152d0: 2020 2020 2020 2020 2020 7372 635f 6374            src_ct
+000152e0: 785b 2766 696e 616c 5f63 6f6e 666e 275d  x['final_confn']
+000152f0: 203d 2063 6c6f 646f 6f2e 6275 696c 645f   = clodoo.build_
+00015300: 6f64 6f6f 5f70 6172 616d 280a 2020 2020  odoo_param(.    
+00015310: 2020 2020 2020 2020 2020 2020 2743 4f4e              'CON
+00015320: 464e 272c 206f 646f 6f5f 7669 643d 7372  FN', odoo_vid=sr
+00015330: 635f 6374 785b 2766 696e 616c 5f62 7261  c_ctx['final_bra
+00015340: 6e63 6827 5d2c 206d 756c 7469 3d54 7275  nch'], multi=Tru
+00015350: 6529 0a20 2020 2069 6620 6e6f 7420 6f73  e).    if not os
+00015360: 2e70 6174 682e 6973 6669 6c65 2873 7263  .path.isfile(src
+00015370: 5f63 7478 5b27 6669 6e61 6c5f 636f 6e66  _ctx['final_conf
+00015380: 6e27 5d29 3a0a 2020 2020 2020 2020 7261  n']):.        ra
+00015390: 6973 6520 494f 4572 726f 7228 2746 696c  ise IOError('Fil
+000153a0: 6520 2573 206e 6f74 2066 6f75 6e64 2720  e %s not found' 
+000153b0: 2520 7372 635f 6374 785b 2766 696e 616c  % src_ctx['final
+000153c0: 5f63 6f6e 666e 275d 290a 2020 2020 6966  _confn']).    if
+000153d0: 206e 6f74 2073 7263 5f63 7478 5b27 6669   not src_ctx['fi
+000153e0: 6e61 6c5f 6272 616e 6368 275d 3a0a 2020  nal_branch']:.  
+000153f0: 2020 2020 2020 7467 745f 636f 6e66 6967        tgt_config
+00015400: 203d 2043 6f6e 6669 6750 6172 7365 722e   = ConfigParser.
+00015410: 5361 6665 436f 6e66 6967 5061 7273 6572  SafeConfigParser
+00015420: 2829 0a20 2020 2020 2020 2074 6774 5f63  ().        tgt_c
+00015430: 6f6e 6669 672e 7265 6164 2873 7263 5f63  onfig.read(src_c
+00015440: 7478 5b27 6669 6e61 6c5f 636f 6e66 6e27  tx['final_confn'
+00015450: 5d29 0a20 2020 2020 2020 2073 7263 5f63  ]).        src_c
+00015460: 7478 5b27 7467 745f 6f64 6f6f 5f66 7665  tx['tgt_odoo_fve
+00015470: 7227 5d20 3d20 7467 745f 636f 6e66 6967  r'] = tgt_config
+00015480: 2e67 6574 2827 6f70 7469 6f6e 7327 2c20  .get('options', 
+00015490: 276f 655f 7665 7273 696f 6e27 290a 2020  'oe_version').  
+000154a0: 2020 2020 2020 7372 635f 6374 785b 2766        src_ctx['f
+000154b0: 696e 616c 5f62 7261 6e63 6827 5d20 3d20  inal_branch'] = 
+000154c0: 7372 635f 6374 785b 2774 6774 5f6f 646f  src_ctx['tgt_odo
+000154d0: 6f5f 6676 6572 275d 0a20 2020 2073 7263  o_fver'].    src
+000154e0: 5f63 7478 5b27 7467 745f 6f64 6f6f 5f76  _ctx['tgt_odoo_v
+000154f0: 6572 275d 203d 2063 6c6f 646f 6f2e 6275  er'] = clodoo.bu
+00015500: 696c 645f 6f64 6f6f 5f70 6172 616d 280a  ild_odoo_param(.
+00015510: 2020 2020 2020 2020 2020 2020 274d 414a              'MAJ
+00015520: 5645 5227 2c20 6f64 6f6f 5f76 6964 3d73  VER', odoo_vid=s
+00015530: 7263 5f63 7478 5b27 6669 6e61 6c5f 6272  rc_ctx['final_br
+00015540: 616e 6368 275d 2c20 6d75 6c74 693d 5472  anch'], multi=Tr
+00015550: 7565 290a 0a20 2020 2069 6620 2828 7372  ue)..    if ((sr
+00015560: 635f 6374 785b 2773 7263 5f6f 646f 6f5f  c_ctx['src_odoo_
+00015570: 7665 7227 5d20 3e3d 2073 7263 5f63 7478  ver'] >= src_ctx
+00015580: 5b27 7467 745f 6f64 6f6f 5f76 6572 275d  ['tgt_odoo_ver']
+00015590: 2061 6e64 0a20 2020 2020 2020 2020 2020   and.           
+000155a0: 206e 6f74 2073 7263 5f63 7478 5b27 7365   not src_ctx['se
+000155b0: 6c5f 6d6f 6465 6c27 5d29 206f 720a 2020  l_model']) or.  
+000155c0: 2020 2020 2020 2873 7263 5f63 7478 5b27        (src_ctx['
+000155d0: 7372 635f 6f64 6f6f 5f76 6572 275d 203e  src_odoo_ver'] >
+000155e0: 2073 7263 5f63 7478 5b27 7467 745f 6f64   src_ctx['tgt_od
+000155f0: 6f6f 5f76 6572 275d 2061 6e64 0a20 2020  oo_ver'] and.   
+00015600: 2020 2020 2020 2020 2073 7263 5f63 7478           src_ctx
+00015610: 5b27 7365 6c5f 6d6f 6465 6c27 5d29 293a  ['sel_model'])):
+00015620: 0a20 2020 2020 2020 2072 6169 7365 204b  .        raise K
+00015630: 6579 4572 726f 7228 2746 696e 616c 2076  eyError('Final v
+00015640: 6572 7369 6f6e 206d 7573 7420 6265 2067  ersion must be g
+00015650: 7265 6174 6572 2074 6861 6e20 6f72 6967  reater than orig
+00015660: 696e 616c 2076 6572 7369 6f6e 2729 0a0a  inal version')..
+00015670: 2020 2020 6966 206e 6f74 2073 7263 5f63      if not src_c
+00015680: 7478 5b27 6f70 745f 6f75 7061 7468 275d  tx['opt_oupath']
+00015690: 3a0a 2020 2020 2020 2020 7372 635f 6374  :.        src_ct
+000156a0: 785b 276f 7074 5f6f 7570 6174 6827 5d20  x['opt_oupath'] 
+000156b0: 3d20 6f73 2e70 6174 682e 6a6f 696e 286f  = os.path.join(o
+000156c0: 732e 7061 7468 2e65 7870 616e 6475 7365  s.path.expanduse
+000156d0: 7228 277e 2729 2c20 2774 6d70 2729 0a20  r('~'), 'tmp'). 
+000156e0: 2020 2069 6620 6e6f 7420 7372 635f 6374     if not src_ct
+000156f0: 785b 276f 7074 5f6f 756c 7061 7468 275d  x['opt_oulpath']
+00015700: 3a0a 2020 2020 2020 2020 7372 635f 6374  :.        src_ct
+00015710: 785b 276f 7074 5f6f 756c 7061 7468 275d  x['opt_oulpath']
+00015720: 203d 206f 732e 7061 7468 2e6a 6f69 6e28   = os.path.join(
+00015730: 7372 635f 6374 785b 276f 7074 5f6f 7570  src_ctx['opt_oup
+00015740: 6174 6827 5d2c 0a20 2020 2020 2020 2020  ath'],.         
 00015750: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00015760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015770: 2020 2027 6f70 656e 7570 6772 6164 656c     'openupgradel
-00015780: 6962 2729 0a0a 2020 2020 6966 2073 7263  ib')..    if src
-00015790: 5f63 7478 5b27 6669 6e61 6c5f 6462 6e61  _ctx['final_dbna
-000157a0: 6d65 275d 2061 6e64 206e 6f74 2073 7263  me'] and not src
-000157b0: 5f63 7478 5b27 6672 6f6d 5f64 626e 616d  _ctx['from_dbnam
-000157c0: 6527 5d3a 0a20 2020 2020 2020 2073 7263  e']:.        src
-000157d0: 5f63 7478 5b27 6672 6f6d 5f64 626e 616d  _ctx['from_dbnam
-000157e0: 6527 5d2c 2073 7263 5f63 7478 5b27 6669  e'], src_ctx['fi
-000157f0: 6e61 6c5f 6462 6e61 6d65 275d 203d 205c  nal_dbname'] = \
-00015800: 0a20 2020 2020 2020 2020 2020 2073 7263  .            src
-00015810: 5f63 7478 5b27 6669 6e61 6c5f 6462 6e61  _ctx['final_dbna
-00015820: 6d65 275d 2c20 2725 735f 3230 3231 2720  me'], '%s_2021' 
-00015830: 2520 7372 635f 6374 785b 2766 696e 616c  % src_ctx['final
-00015840: 5f64 626e 616d 6527 5d0a 2020 2020 656c  _dbname'].    el
-00015850: 6966 206e 6f74 2073 7263 5f63 7478 5b27  if not src_ctx['
-00015860: 6669 6e61 6c5f 6462 6e61 6d65 275d 2061  final_dbname'] a
-00015870: 6e64 2073 7263 5f63 7478 5b27 6672 6f6d  nd src_ctx['from
-00015880: 5f64 626e 616d 6527 5d3a 0a20 2020 2020  _dbname']:.     
-00015890: 2020 2073 7263 5f63 7478 5b27 6669 6e61     src_ctx['fina
-000158a0: 6c5f 6462 6e61 6d65 275d 203d 2027 2573  l_dbname'] = '%s
-000158b0: 5f32 3032 3127 2025 2073 7263 5f63 7478  _2021' % src_ctx
-000158c0: 5b27 6672 6f6d 5f64 626e 616d 6527 5d0a  ['from_dbname'].
-000158d0: 2020 2020 656c 6966 206e 6f74 2073 7263      elif not src
-000158e0: 5f63 7478 5b27 6669 6e61 6c5f 6462 6e61  _ctx['final_dbna
-000158f0: 6d65 275d 2061 6e64 206e 6f74 2073 7263  me'] and not src
-00015900: 5f63 7478 5b27 6672 6f6d 5f64 626e 616d  _ctx['from_dbnam
-00015910: 6527 5d3a 0a20 2020 2020 2020 2072 6169  e']:.        rai
-00015920: 7365 204b 6579 4572 726f 7228 274d 6973  se KeyError('Mis
-00015930: 7365 6420 6461 7461 6261 7365 2074 6f20  sed database to 
-00015940: 7570 6772 6164 6521 2050 6c65 6173 6520  upgrade! Please 
-00015950: 7573 6520 2d64 2073 7769 7463 6827 290a  use -d switch').
-00015960: 0a20 2020 2069 6620 6e6f 7420 7372 635f  .    if not src_
-00015970: 6374 785b 276c 6f67 666e 275d 3a0a 2020  ctx['logfn']:.  
-00015980: 2020 2020 2020 6966 2073 7263 5f63 7478        if src_ctx
-00015990: 5b27 6f63 615f 6d69 6772 6174 6527 5d3a  ['oca_migrate']:
-000159a0: 0a20 2020 2020 2020 2020 2020 2073 7263  .            src
-000159b0: 5f63 7478 5b27 6c6f 6766 6e27 5d20 3d20  _ctx['logfn'] = 
-000159c0: 6f73 2e70 6174 682e 6a6f 696e 2873 7263  os.path.join(src
-000159d0: 5f63 7478 5b27 6f70 745f 6f75 7061 7468  _ctx['opt_oupath
-000159e0: 275d 2c0a 2020 2020 2020 2020 2020 2020  '],.            
+00015770: 2020 2020 2027 6f70 656e 7570 6772 6164       'openupgrad
+00015780: 656c 6962 2729 0a0a 2020 2020 6966 2073  elib')..    if s
+00015790: 7263 5f63 7478 5b27 6669 6e61 6c5f 6462  rc_ctx['final_db
+000157a0: 6e61 6d65 275d 2061 6e64 206e 6f74 2073  name'] and not s
+000157b0: 7263 5f63 7478 5b27 6672 6f6d 5f64 626e  rc_ctx['from_dbn
+000157c0: 616d 6527 5d3a 0a20 2020 2020 2020 2073  ame']:.        s
+000157d0: 7263 5f63 7478 5b27 6672 6f6d 5f64 626e  rc_ctx['from_dbn
+000157e0: 616d 6527 5d2c 2073 7263 5f63 7478 5b27  ame'], src_ctx['
+000157f0: 6669 6e61 6c5f 6462 6e61 6d65 275d 203d  final_dbname'] =
+00015800: 205c 0a20 2020 2020 2020 2020 2020 2073   \.            s
+00015810: 7263 5f63 7478 5b27 6669 6e61 6c5f 6462  rc_ctx['final_db
+00015820: 6e61 6d65 275d 2c20 2725 735f 3230 3231  name'], '%s_2021
+00015830: 2720 2520 7372 635f 6374 785b 2766 696e  ' % src_ctx['fin
+00015840: 616c 5f64 626e 616d 6527 5d0a 2020 2020  al_dbname'].    
+00015850: 656c 6966 206e 6f74 2073 7263 5f63 7478  elif not src_ctx
+00015860: 5b27 6669 6e61 6c5f 6462 6e61 6d65 275d  ['final_dbname']
+00015870: 2061 6e64 2073 7263 5f63 7478 5b27 6672   and src_ctx['fr
+00015880: 6f6d 5f64 626e 616d 6527 5d3a 0a20 2020  om_dbname']:.   
+00015890: 2020 2020 2073 7263 5f63 7478 5b27 6669       src_ctx['fi
+000158a0: 6e61 6c5f 6462 6e61 6d65 275d 203d 2027  nal_dbname'] = '
+000158b0: 2573 5f32 3032 3127 2025 2073 7263 5f63  %s_2021' % src_c
+000158c0: 7478 5b27 6672 6f6d 5f64 626e 616d 6527  tx['from_dbname'
+000158d0: 5d0a 2020 2020 656c 6966 206e 6f74 2073  ].    elif not s
+000158e0: 7263 5f63 7478 5b27 6669 6e61 6c5f 6462  rc_ctx['final_db
+000158f0: 6e61 6d65 275d 2061 6e64 206e 6f74 2073  name'] and not s
+00015900: 7263 5f63 7478 5b27 6672 6f6d 5f64 626e  rc_ctx['from_dbn
+00015910: 616d 6527 5d3a 0a20 2020 2020 2020 2072  ame']:.        r
+00015920: 6169 7365 204b 6579 4572 726f 7228 274d  aise KeyError('M
+00015930: 6973 7365 6420 6461 7461 6261 7365 2074  issed database t
+00015940: 6f20 7570 6772 6164 6521 2050 6c65 6173  o upgrade! Pleas
+00015950: 6520 7573 6520 2d64 2073 7769 7463 6827  e use -d switch'
+00015960: 290a 0a20 2020 2069 6620 6e6f 7420 7372  )..    if not sr
+00015970: 635f 6374 785b 276c 6f67 666e 275d 3a0a  c_ctx['logfn']:.
+00015980: 2020 2020 2020 2020 6966 2073 7263 5f63          if src_c
+00015990: 7478 5b27 6f63 615f 6d69 6772 6174 6527  tx['oca_migrate'
+000159a0: 5d3a 0a20 2020 2020 2020 2020 2020 2073  ]:.            s
+000159b0: 7263 5f63 7478 5b27 6c6f 6766 6e27 5d20  rc_ctx['logfn'] 
+000159c0: 3d20 6f73 2e70 6174 682e 6a6f 696e 2873  = os.path.join(s
+000159d0: 7263 5f63 7478 5b27 6f70 745f 6f75 7061  rc_ctx['opt_oupa
+000159e0: 7468 275d 2c0a 2020 2020 2020 2020 2020  th'],.          
 000159f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00015a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015a10: 276d 6967 7261 7465 5f62 795f 6f70 656e  'migrate_by_open
-00015a20: 7570 6772 6164 652e 6c6f 6727 290a 2020  upgrade.log').  
-00015a30: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00015a40: 2020 2020 2020 2020 7372 635f 6374 785b          src_ctx[
-00015a50: 276c 6f67 666e 275d 203d 206f 732e 7061  'logfn'] = os.pa
-00015a60: 7468 2e6a 6f69 6e28 7372 635f 6374 785b  th.join(src_ctx[
-00015a70: 276f 7074 5f6f 7570 6174 6827 5d2c 0a20  'opt_oupath'],. 
-00015a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015a10: 2020 276d 6967 7261 7465 5f62 795f 6f70    'migrate_by_op
+00015a20: 656e 7570 6772 6164 652e 6c6f 6727 290a  enupgrade.log').
+00015a30: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00015a40: 2020 2020 2020 2020 2020 7372 635f 6374            src_ct
+00015a50: 785b 276c 6f67 666e 275d 203d 206f 732e  x['logfn'] = os.
+00015a60: 7061 7468 2e6a 6f69 6e28 7372 635f 6374  path.join(src_ct
+00015a70: 785b 276f 7074 5f6f 7570 6174 6827 5d2c  x['opt_oupath'],
+00015a80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00015a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015aa0: 2020 2020 2020 2020 2020 2027 6d69 6772             'migr
-00015ab0: 6174 655f 6f64 6f6f 5f64 622e 6c6f 6727  ate_odoo_db.log'
-00015ac0: 290a 2020 2020 7372 635f 6374 785b 276c  ).    src_ctx['l
-00015ad0: 6f67 6669 6c65 275d 203d 206f 732e 7061  ogfile'] = os.pa
-00015ae0: 7468 2e6a 6f69 6e28 7372 635f 6374 785b  th.join(src_ctx[
-00015af0: 276f 7074 5f6f 7570 6174 6827 5d2c 0a20  'opt_oupath'],. 
-00015b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015aa0: 2020 2020 2020 2020 2020 2020 2027 6d69               'mi
+00015ab0: 6772 6174 655f 6f64 6f6f 5f64 622e 6c6f  grate_odoo_db.lo
+00015ac0: 6727 290a 2020 2020 7372 635f 6374 785b  g').    src_ctx[
+00015ad0: 276c 6f67 6669 6c65 275d 203d 206f 732e  'logfile'] = os.
+00015ae0: 7061 7468 2e6a 6f69 6e28 7372 635f 6374  path.join(src_ct
+00015af0: 785b 276f 7074 5f6f 7570 6174 6827 5d2c  x['opt_oupath'],
+00015b00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00015b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015b20: 2020 2020 2027 6d69 6772 6174 655f 6f64       'migrate_od
-00015b30: 6f6f 5f64 622d 7365 7276 6572 2e6c 6f67  oo_db-server.log
-00015b40: 2729 0a20 2020 2073 7263 5f63 7478 5b27  ').    src_ctx['
-00015b50: 6669 6e61 6c5f 7665 7227 5d20 3d20 7372  final_ver'] = sr
-00015b60: 635f 6374 785b 2774 6774 5f6f 646f 6f5f  c_ctx['tgt_odoo_
-00015b70: 7665 7227 5d0a 2020 2020 7467 745f 6374  ver'].    tgt_ct
-00015b80: 7820 3d20 7372 635f 6374 782e 636f 7079  x = src_ctx.copy
-00015b90: 2829 0a20 2020 2044 4546 5f43 4f4e 4620  ().    DEF_CONF 
-00015ba0: 3d20 636c 6f64 6f6f 2e64 6566 6175 6c74  = clodoo.default
-00015bb0: 5f63 6f6e 6628 7372 635f 6374 7829 0a20  _conf(src_ctx). 
-00015bc0: 2020 2072 6574 7572 6e20 7372 635f 6374     return src_ct
-00015bd0: 782c 2074 6774 5f63 7478 0a0a 0a5f 4445  x, tgt_ctx..._DE
-00015be0: 5052 4543 4154 4544 5f4d 4f44 554c 4553  PRECATED_MODULES
-00015bf0: 203d 205b 0a20 2020 2028 2261 6363 6f75   = [.    ("accou
-00015c00: 6e74 5f61 6e61 6c79 7469 635f 616e 616c  nt_analytic_anal
-00015c10: 7973 6973 222c 2022 6f63 615f 6d6f 7665  ysis", "oca_move
-00015c20: 6422 2c20 2263 6f6e 7472 6163 7422 2c0a  d", "contract",.
-00015c30: 2020 2020 2020 2020 224d 6f76 6564 2074          "Moved t
-00015c40: 6f20 4f43 412f 636f 6e74 7261 6374 2229  o OCA/contract")
-00015c50: 2c0a 2020 2020 2822 6163 636f 756e 745f  ,.    ("account_
-00015c60: 616e 616c 7974 6963 5f70 6c61 6e73 222c  analytic_plans",
-00015c70: 2022 6f63 615f 6d6f 7665 6422 2c20 2261   "oca_moved", "a
-00015c80: 6363 6f75 6e74 5f61 6e61 6c79 7469 635f  ccount_analytic_
-00015c90: 6469 7374 7269 6275 7469 6f6e 222c 0a20  distribution",. 
-00015ca0: 2020 2020 2020 2022 4d6f 7665 6420 746f         "Moved to
-00015cb0: 204f 4341 2f61 6363 6f75 6e74 5f61 6e61   OCA/account_ana
-00015cc0: 6c79 7469 6322 292c 0a20 2020 2028 2261  lytic"),.    ("a
-00015cd0: 6363 6f75 6e74 5f61 6e67 6c6f 5f73 6178  ccount_anglo_sax
-00015ce0: 6f6e 222c 2022 7265 6d6f 7665 6422 292c  on", "removed"),
-00015cf0: 0a20 2020 2028 2261 6363 6f75 6e74 5f62  .    ("account_b
-00015d00: 616e 6b5f 7374 6174 656d 656e 745f 6578  ank_statement_ex
-00015d10: 7465 6e73 696f 6e73 222c 2022 7265 6d6f  tensions", "remo
-00015d20: 7665 6422 292c 0a20 2020 2028 2261 6363  ved"),.    ("acc
-00015d30: 6f75 6e74 5f63 6861 7274 222c 2022 6d65  ount_chart", "me
-00015d40: 7267 6564 222c 2022 6163 636f 756e 7422  rged", "account"
-00015d50: 292c 0a20 2020 2028 2261 6363 6f75 6e74  ),.    ("account
-00015d60: 5f63 6865 636b 5f77 7269 7469 6e67 222c  _check_writing",
-00015d70: 2022 7265 6e61 6d65 6422 2c20 2261 6363   "renamed", "acc
-00015d80: 6f75 6e74 5f63 6865 636b 5f70 7269 6e74  ount_check_print
-00015d90: 696e 6722 292c 0a20 2020 2028 2261 6363  ing"),.    ("acc
-00015da0: 6f75 6e74 5f66 6f6c 6c6f 7775 7022 2c20  ount_followup", 
-00015db0: 2272 656d 6f76 6564 2229 2c0a 2020 2020  "removed"),.    
-00015dc0: 2822 6163 636f 756e 745f 7061 796d 656e  ("account_paymen
-00015dd0: 7422 2c20 226f 6361 5f6d 6f76 6564 222c  t", "oca_moved",
-00015de0: 2022 6163 636f 756e 745f 7061 796d 656e   "account_paymen
-00015df0: 745f 6f72 6465 7222 2c0a 2020 2020 2020  t_order",.      
-00015e00: 2020 224d 6f76 6564 2074 6f20 4f43 412f    "Moved to OCA/
-00015e10: 6261 6e6b 2d70 6179 6d65 6e74 2229 2c0a  bank-payment"),.
-00015e20: 2020 2020 2822 6163 636f 756e 745f 7365      ("account_se
-00015e30: 7175 656e 6365 222c 2022 7265 6d6f 7665  quence", "remove
-00015e40: 6422 292c 0a20 2020 2028 2261 6e61 6c79  d"),.    ("analy
-00015e50: 7469 635f 636f 6e74 7261 6374 5f68 725f  tic_contract_hr_
-00015e60: 6578 7065 6e73 6522 2c20 2272 656d 6f76  expense", "remov
-00015e70: 6564 2229 2c0a 2020 2020 2822 616e 616c  ed"),.    ("anal
-00015e80: 7974 6963 5f75 7365 725f 6675 6e63 7469  ytic_user_functi
-00015e90: 6f6e 222c 2022 7265 6d6f 7665 6422 292c  on", "removed"),
-00015ea0: 0a20 2020 2028 2261 6e67 6c6f 5f73 6178  .    ("anglo_sax
-00015eb0: 6f6e 5f64 726f 7073 6869 7070 696e 6722  on_dropshipping"
-00015ec0: 2c20 2272 656d 6f76 6564 2229 2c0a 2020  , "removed"),.  
-00015ed0: 2020 2822 6175 7468 5f6f 7065 6e69 6422    ("auth_openid"
-00015ee0: 2c20 2272 656d 6f76 6564 2229 2c0a 2020  , "removed"),.  
-00015ef0: 2020 2822 6261 7365 5f72 6570 6f72 745f    ("base_report_
-00015f00: 6465 7369 676e 6572 222c 2022 7265 6d6f  designer", "remo
-00015f10: 7665 6422 292c 0a20 2020 2028 2263 6f6e  ved"),.    ("con
-00015f20: 7461 6374 7322 2c20 226d 6572 6765 6422  tacts", "merged"
-00015f30: 2c20 226d 6169 6c22 292c 0a20 2020 2028  , "mail"),.    (
-00015f40: 2263 726d 5f68 656c 7064 6573 6b22 2c20  "crm_helpdesk", 
-00015f50: 2272 656d 6f76 6564 2229 2c0a 2020 2020  "removed"),.    
-00015f60: 2822 6372 6d5f 6d61 7373 5f6d 6169 6c69  ("crm_mass_maili
-00015f70: 6e67 222c 2022 7265 6d6f 7665 6422 292c  ng", "removed"),
-00015f80: 0a20 2020 2028 2263 726d 5f70 726f 6669  .    ("crm_profi
-00015f90: 6c69 6e67 222c 2022 7265 6d6f 7665 6422  ling", "removed"
-00015fa0: 292c 0a20 2020 2028 2265 6469 222c 2022  ),.    ("edi", "
-00015fb0: 7265 6d6f 7665 6422 292c 0a20 2020 2028  removed"),.    (
-00015fc0: 2265 6d61 696c 5f74 656d 706c 6174 6522  "email_template"
-00015fd0: 2c20 226d 6572 6765 6422 2c20 226d 6169  , "merged", "mai
-00015fe0: 6c5f 7465 6d70 6c61 7465 2229 2c0a 2020  l_template"),.  
-00015ff0: 2020 2822 6872 5f61 7070 6c69 6361 6e74    ("hr_applicant
-00016000: 5f64 6f63 756d 656e 7422 2c20 2272 656d  _document", "rem
-00016010: 6f76 6564 2229 2c0a 2020 2020 2822 6872  oved"),.    ("hr
-00016020: 5f74 696d 6573 6865 6574 5f69 6e76 6f69  _timesheet_invoi
-00016030: 6365 222c 2022 7265 6d6f 7665 6422 292c  ce", "removed"),
-00016040: 0a20 2020 2028 2269 6d5f 6368 6174 222c  .    ("im_chat",
-00016050: 2022 6d65 7267 6564 222c 2022 6d61 696c   "merged", "mail
-00016060: 2229 2c0a 2020 2020 2822 6b6e 6f77 6c65  "),.    ("knowle
-00016070: 6467 6522 2c20 226f 6361 5f6d 6f76 6564  dge", "oca_moved
-00016080: 222c 2022 6b6e 6f77 6c65 6467 6522 2c20  ", "knowledge", 
-00016090: 224d 6f76 6564 2074 6f20 4f43 412f 6b6e  "Moved to OCA/kn
-000160a0: 6f77 6c65 6467 6522 292c 0a20 2020 2028  owledge"),.    (
-000160b0: 226c 3130 6e5f 6265 5f63 6f64 6122 2c20  "l10n_be_coda", 
-000160c0: 2272 656d 6f76 6564 2229 2c0a 2020 2020  "removed"),.    
-000160d0: 2822 6c31 306e 5f66 725f 7269 6222 2c20  ("l10n_fr_rib", 
-000160e0: 2272 656d 6f76 6564 2229 2c0a 2020 2020  "removed"),.    
-000160f0: 2822 6d61 726b 6574 696e 675f 6372 6d22  ("marketing_crm"
-00016100: 2c20 226d 6572 6765 6422 2c20 2263 726d  , "merged", "crm
-00016110: 2229 2c0a 2020 2020 2822 6d75 6c74 695f  "),.    ("multi_
-00016120: 636f 6d70 616e 7922 2c20 2272 656d 6f76  company", "remov
-00016130: 6564 2229 2c0a 2020 2020 2822 706f 7274  ed"),.    ("port
-00016140: 616c 5f63 6c61 696d 222c 2022 7265 6e61  al_claim", "rena
-00016150: 6d65 6422 2c20 2277 6562 7369 7465 5f63  med", "website_c
-00016160: 726d 5f63 6c61 696d 2229 2c0a 2020 2020  rm_claim"),.    
-00016170: 2822 706f 7274 616c 5f70 726f 6a65 6374  ("portal_project
-00016180: 222c 2022 6d65 7267 6564 222c 2022 7072  ", "merged", "pr
-00016190: 6f6a 6563 7422 292c 0a20 2020 2028 2270  oject"),.    ("p
-000161a0: 6f72 7461 6c5f 7072 6f6a 6563 745f 6973  ortal_project_is
-000161b0: 7375 6522 2c20 226d 6572 6765 6422 2c20  sue", "merged", 
-000161c0: 2270 726f 6a65 6374 5f69 7373 7565 2229  "project_issue")
-000161d0: 2c0a 2020 2020 2822 7072 6f63 7572 656d  ,.    ("procurem
-000161e0: 656e 745f 6a69 745f 7374 6f63 6b22 2c20  ent_jit_stock", 
-000161f0: 226d 6572 6765 6422 2c20 2270 726f 6375  "merged", "procu
-00016200: 7265 6d65 6e74 5f6a 6974 2229 2c0a 2020  rement_jit"),.  
-00016210: 2020 2822 7075 7263 6861 7365 5f61 6e61    ("purchase_ana
-00016220: 6c79 7469 635f 706c 616e 7322 2c20 226f  lytic_plans", "o
-00016230: 6361 5f6d 6f76 6564 222c 2022 7075 7263  ca_moved", "purc
-00016240: 6861 7365 5f61 6e61 6c79 7469 635f 6469  hase_analytic_di
-00016250: 7374 7269 6275 7469 6f6e 222c 0a20 2020  stribution",.   
-00016260: 2020 2020 2022 4d6f 7665 6420 746f 204f       "Moved to O
-00016270: 4341 2f61 6363 6f75 6e74 2d61 6e61 6c79  CA/account-analy
-00016280: 7469 6322 292c 0a20 2020 2028 2270 7572  tic"),.    ("pur
-00016290: 6368 6173 655f 646f 7562 6c65 5f76 616c  chase_double_val
-000162a0: 6964 6174 696f 6e22 2c20 2272 656d 6f76  idation", "remov
-000162b0: 6564 2229 2c0a 2020 2020 2822 7361 6c65  ed"),.    ("sale
-000162c0: 5f61 6e61 6c79 7469 635f 706c 616e 7322  _analytic_plans"
-000162d0: 2c20 226f 6361 5f6d 6f76 6564 222c 2022  , "oca_moved", "
-000162e0: 7361 6c65 5f61 6e61 6c79 7469 635f 6469  sale_analytic_di
-000162f0: 7374 7269 6275 7469 6f6e 222c 0a20 2020  stribution",.   
-00016300: 2020 2020 2022 4d6f 7665 6420 746f 204f       "Moved to O
-00016310: 4341 2f61 6363 6f75 6e74 2d61 6e61 6c79  CA/account-analy
-00016320: 7469 6322 292c 0a20 2020 2028 2273 616c  tic"),.    ("sal
-00016330: 655f 6a6f 7572 6e61 6c22 2c20 2272 656d  e_journal", "rem
-00016340: 6f76 6564 2229 2c0a 2020 2020 2822 7368  oved"),.    ("sh
-00016350: 6172 6522 2c20 2272 656d 6f76 6564 2229  are", "removed")
-00016360: 2c0a 2020 2020 2822 7374 6f63 6b5f 696e  ,.    ("stock_in
-00016370: 766f 6963 655f 6469 7265 6374 6c79 222c  voice_directly",
-00016380: 2022 7265 6d6f 7665 6422 292c 0a20 2020   "removed"),.   
-00016390: 2028 2277 6562 5f61 7069 222c 2022 7265   ("web_api", "re
-000163a0: 6d6f 7665 6422 292c 0a20 2020 2028 2277  moved"),.    ("w
-000163b0: 6562 5f67 616e 7474 222c 2022 6d65 7267  eb_gantt", "merg
-000163c0: 6564 222c 2022 7765 6222 292c 0a20 2020  ed", "web"),.   
-000163d0: 2028 2277 6562 5f67 7261 7068 222c 2022   ("web_graph", "
-000163e0: 6d65 7267 6564 222c 2022 7765 6222 292c  merged", "web"),
-000163f0: 0a20 2020 2028 2277 6562 5f6b 616e 6261  .    ("web_kanba
-00016400: 6e5f 7370 6172 6b6c 696e 6522 2c20 226d  n_sparkline", "m
-00016410: 6572 6765 6422 2c20 2277 6562 2229 2c0a  erged", "web"),.
-00016420: 2020 2020 2822 7765 625f 7465 7374 7322      ("web_tests"
-00016430: 2c20 226d 6572 6765 6422 2c20 2277 6562  , "merged", "web
-00016440: 2229 2c0a 2020 2020 2822 7765 625f 7465  "),.    ("web_te
-00016450: 7374 735f 6465 6d6f 222c 2022 7265 6d6f  sts_demo", "remo
-00016460: 7665 6422 292c 0a20 2020 2028 2277 6562  ved"),.    ("web
-00016470: 7369 7465 5f63 6572 7469 6669 6361 7469  site_certificati
-00016480: 6f6e 222c 2022 7265 6d6f 7665 6422 292c  on", "removed"),
-00016490: 0a20 2020 2028 2277 6562 7369 7465 5f69  .    ("website_i
-000164a0: 6e73 7461 6e74 636c 6963 6b22 2c20 2272  nstantclick", "r
-000164b0: 656d 6f76 6564 2229 2c0a 2020 2020 2822  emoved"),.    ("
-000164c0: 7765 6273 6974 655f 6d61 696c 5f67 726f  website_mail_gro
-000164d0: 7570 222c 2022 7265 6e61 6d65 6422 2c20  up", "renamed", 
-000164e0: 2277 6562 7369 7465 5f6d 6169 6c5f 6368  "website_mail_ch
-000164f0: 616e 6e65 6c22 292c 0a20 2020 2028 2277  annel"),.    ("w
-00016500: 6562 7369 7465 5f72 6570 6f72 7422 2c20  ebsite_report", 
-00016510: 226d 6572 6765 6422 2c20 2272 6570 6f72  "merged", "repor
-00016520: 7422 292c 0a5d 0a0a 6966 205f 5f6e 616d  t"),.]..if __nam
-00016530: 655f 5f20 3d3d 2022 5f5f 6d61 696e 5f5f  e__ == "__main__
-00016540: 223a 0a20 2020 2070 6172 7365 7220 3d20  ":.    parser = 
-00016550: 7a30 6c69 622e 7061 7273 656f 7074 6172  z0lib.parseoptar
-00016560: 6773 2822 4d69 6772 6174 6520 4f64 6f6f  gs("Migrate Odoo
-00016570: 2044 4222 2c0a 2020 2020 2020 2020 2020   DB",.          
+00015b20: 2020 2020 2020 2027 6d69 6772 6174 655f         'migrate_
+00015b30: 6f64 6f6f 5f64 622d 7365 7276 6572 2e6c  odoo_db-server.l
+00015b40: 6f67 2729 0a20 2020 2073 7263 5f63 7478  og').    src_ctx
+00015b50: 5b27 6669 6e61 6c5f 7665 7227 5d20 3d20  ['final_ver'] = 
+00015b60: 7372 635f 6374 785b 2774 6774 5f6f 646f  src_ctx['tgt_odo
+00015b70: 6f5f 7665 7227 5d0a 2020 2020 7467 745f  o_ver'].    tgt_
+00015b80: 6374 7820 3d20 7372 635f 6374 782e 636f  ctx = src_ctx.co
+00015b90: 7079 2829 0a20 2020 2044 4546 5f43 4f4e  py().    DEF_CON
+00015ba0: 4620 3d20 636c 6f64 6f6f 2e64 6566 6175  F = clodoo.defau
+00015bb0: 6c74 5f63 6f6e 6628 7372 635f 6374 7829  lt_conf(src_ctx)
+00015bc0: 0a20 2020 2072 6574 7572 6e20 7372 635f  .    return src_
+00015bd0: 6374 782c 2074 6774 5f63 7478 0a0a 0a5f  ctx, tgt_ctx..._
+00015be0: 4445 5052 4543 4154 4544 5f4d 4f44 554c  DEPRECATED_MODUL
+00015bf0: 4553 203d 205b 0a20 2020 2028 2261 6363  ES = [.    ("acc
+00015c00: 6f75 6e74 5f61 6e61 6c79 7469 635f 616e  ount_analytic_an
+00015c10: 616c 7973 6973 222c 2022 6f63 615f 6d6f  alysis", "oca_mo
+00015c20: 7665 6422 2c20 2263 6f6e 7472 6163 7422  ved", "contract"
+00015c30: 2c0a 2020 2020 2020 2020 224d 6f76 6564  ,.        "Moved
+00015c40: 2074 6f20 4f43 412f 636f 6e74 7261 6374   to OCA/contract
+00015c50: 2229 2c0a 2020 2020 2822 6163 636f 756e  "),.    ("accoun
+00015c60: 745f 616e 616c 7974 6963 5f70 6c61 6e73  t_analytic_plans
+00015c70: 222c 2022 6f63 615f 6d6f 7665 6422 2c20  ", "oca_moved", 
+00015c80: 2261 6363 6f75 6e74 5f61 6e61 6c79 7469  "account_analyti
+00015c90: 635f 6469 7374 7269 6275 7469 6f6e 222c  c_distribution",
+00015ca0: 0a20 2020 2020 2020 2022 4d6f 7665 6420  .        "Moved 
+00015cb0: 746f 204f 4341 2f61 6363 6f75 6e74 5f61  to OCA/account_a
+00015cc0: 6e61 6c79 7469 6322 292c 0a20 2020 2028  nalytic"),.    (
+00015cd0: 2261 6363 6f75 6e74 5f61 6e67 6c6f 5f73  "account_anglo_s
+00015ce0: 6178 6f6e 222c 2022 7265 6d6f 7665 6422  axon", "removed"
+00015cf0: 292c 0a20 2020 2028 2261 6363 6f75 6e74  ),.    ("account
+00015d00: 5f62 616e 6b5f 7374 6174 656d 656e 745f  _bank_statement_
+00015d10: 6578 7465 6e73 696f 6e73 222c 2022 7265  extensions", "re
+00015d20: 6d6f 7665 6422 292c 0a20 2020 2028 2261  moved"),.    ("a
+00015d30: 6363 6f75 6e74 5f63 6861 7274 222c 2022  ccount_chart", "
+00015d40: 6d65 7267 6564 222c 2022 6163 636f 756e  merged", "accoun
+00015d50: 7422 292c 0a20 2020 2028 2261 6363 6f75  t"),.    ("accou
+00015d60: 6e74 5f63 6865 636b 5f77 7269 7469 6e67  nt_check_writing
+00015d70: 222c 2022 7265 6e61 6d65 6422 2c20 2261  ", "renamed", "a
+00015d80: 6363 6f75 6e74 5f63 6865 636b 5f70 7269  ccount_check_pri
+00015d90: 6e74 696e 6722 292c 0a20 2020 2028 2261  nting"),.    ("a
+00015da0: 6363 6f75 6e74 5f66 6f6c 6c6f 7775 7022  ccount_followup"
+00015db0: 2c20 2272 656d 6f76 6564 2229 2c0a 2020  , "removed"),.  
+00015dc0: 2020 2822 6163 636f 756e 745f 7061 796d    ("account_paym
+00015dd0: 656e 7422 2c20 226f 6361 5f6d 6f76 6564  ent", "oca_moved
+00015de0: 222c 2022 6163 636f 756e 745f 7061 796d  ", "account_paym
+00015df0: 656e 745f 6f72 6465 7222 2c0a 2020 2020  ent_order",.    
+00015e00: 2020 2020 224d 6f76 6564 2074 6f20 4f43      "Moved to OC
+00015e10: 412f 6261 6e6b 2d70 6179 6d65 6e74 2229  A/bank-payment")
+00015e20: 2c0a 2020 2020 2822 6163 636f 756e 745f  ,.    ("account_
+00015e30: 7365 7175 656e 6365 222c 2022 7265 6d6f  sequence", "remo
+00015e40: 7665 6422 292c 0a20 2020 2028 2261 6e61  ved"),.    ("ana
+00015e50: 6c79 7469 635f 636f 6e74 7261 6374 5f68  lytic_contract_h
+00015e60: 725f 6578 7065 6e73 6522 2c20 2272 656d  r_expense", "rem
+00015e70: 6f76 6564 2229 2c0a 2020 2020 2822 616e  oved"),.    ("an
+00015e80: 616c 7974 6963 5f75 7365 725f 6675 6e63  alytic_user_func
+00015e90: 7469 6f6e 222c 2022 7265 6d6f 7665 6422  tion", "removed"
+00015ea0: 292c 0a20 2020 2028 2261 6e67 6c6f 5f73  ),.    ("anglo_s
+00015eb0: 6178 6f6e 5f64 726f 7073 6869 7070 696e  axon_dropshippin
+00015ec0: 6722 2c20 2272 656d 6f76 6564 2229 2c0a  g", "removed"),.
+00015ed0: 2020 2020 2822 6175 7468 5f6f 7065 6e69      ("auth_openi
+00015ee0: 6422 2c20 2272 656d 6f76 6564 2229 2c0a  d", "removed"),.
+00015ef0: 2020 2020 2822 6261 7365 5f72 6570 6f72      ("base_repor
+00015f00: 745f 6465 7369 676e 6572 222c 2022 7265  t_designer", "re
+00015f10: 6d6f 7665 6422 292c 0a20 2020 2028 2263  moved"),.    ("c
+00015f20: 6f6e 7461 6374 7322 2c20 226d 6572 6765  ontacts", "merge
+00015f30: 6422 2c20 226d 6169 6c22 292c 0a20 2020  d", "mail"),.   
+00015f40: 2028 2263 726d 5f68 656c 7064 6573 6b22   ("crm_helpdesk"
+00015f50: 2c20 2272 656d 6f76 6564 2229 2c0a 2020  , "removed"),.  
+00015f60: 2020 2822 6372 6d5f 6d61 7373 5f6d 6169    ("crm_mass_mai
+00015f70: 6c69 6e67 222c 2022 7265 6d6f 7665 6422  ling", "removed"
+00015f80: 292c 0a20 2020 2028 2263 726d 5f70 726f  ),.    ("crm_pro
+00015f90: 6669 6c69 6e67 222c 2022 7265 6d6f 7665  filing", "remove
+00015fa0: 6422 292c 0a20 2020 2028 2265 6469 222c  d"),.    ("edi",
+00015fb0: 2022 7265 6d6f 7665 6422 292c 0a20 2020   "removed"),.   
+00015fc0: 2028 2265 6d61 696c 5f74 656d 706c 6174   ("email_templat
+00015fd0: 6522 2c20 226d 6572 6765 6422 2c20 226d  e", "merged", "m
+00015fe0: 6169 6c5f 7465 6d70 6c61 7465 2229 2c0a  ail_template"),.
+00015ff0: 2020 2020 2822 6872 5f61 7070 6c69 6361      ("hr_applica
+00016000: 6e74 5f64 6f63 756d 656e 7422 2c20 2272  nt_document", "r
+00016010: 656d 6f76 6564 2229 2c0a 2020 2020 2822  emoved"),.    ("
+00016020: 6872 5f74 696d 6573 6865 6574 5f69 6e76  hr_timesheet_inv
+00016030: 6f69 6365 222c 2022 7265 6d6f 7665 6422  oice", "removed"
+00016040: 292c 0a20 2020 2028 2269 6d5f 6368 6174  ),.    ("im_chat
+00016050: 222c 2022 6d65 7267 6564 222c 2022 6d61  ", "merged", "ma
+00016060: 696c 2229 2c0a 2020 2020 2822 6b6e 6f77  il"),.    ("know
+00016070: 6c65 6467 6522 2c20 226f 6361 5f6d 6f76  ledge", "oca_mov
+00016080: 6564 222c 2022 6b6e 6f77 6c65 6467 6522  ed", "knowledge"
+00016090: 2c20 224d 6f76 6564 2074 6f20 4f43 412f  , "Moved to OCA/
+000160a0: 6b6e 6f77 6c65 6467 6522 292c 0a20 2020  knowledge"),.   
+000160b0: 2028 226c 3130 6e5f 6265 5f63 6f64 6122   ("l10n_be_coda"
+000160c0: 2c20 2272 656d 6f76 6564 2229 2c0a 2020  , "removed"),.  
+000160d0: 2020 2822 6c31 306e 5f66 725f 7269 6222    ("l10n_fr_rib"
+000160e0: 2c20 2272 656d 6f76 6564 2229 2c0a 2020  , "removed"),.  
+000160f0: 2020 2822 6d61 726b 6574 696e 675f 6372    ("marketing_cr
+00016100: 6d22 2c20 226d 6572 6765 6422 2c20 2263  m", "merged", "c
+00016110: 726d 2229 2c0a 2020 2020 2822 6d75 6c74  rm"),.    ("mult
+00016120: 695f 636f 6d70 616e 7922 2c20 2272 656d  i_company", "rem
+00016130: 6f76 6564 2229 2c0a 2020 2020 2822 706f  oved"),.    ("po
+00016140: 7274 616c 5f63 6c61 696d 222c 2022 7265  rtal_claim", "re
+00016150: 6e61 6d65 6422 2c20 2277 6562 7369 7465  named", "website
+00016160: 5f63 726d 5f63 6c61 696d 2229 2c0a 2020  _crm_claim"),.  
+00016170: 2020 2822 706f 7274 616c 5f70 726f 6a65    ("portal_proje
+00016180: 6374 222c 2022 6d65 7267 6564 222c 2022  ct", "merged", "
+00016190: 7072 6f6a 6563 7422 292c 0a20 2020 2028  project"),.    (
+000161a0: 2270 6f72 7461 6c5f 7072 6f6a 6563 745f  "portal_project_
+000161b0: 6973 7375 6522 2c20 226d 6572 6765 6422  issue", "merged"
+000161c0: 2c20 2270 726f 6a65 6374 5f69 7373 7565  , "project_issue
+000161d0: 2229 2c0a 2020 2020 2822 7072 6f63 7572  "),.    ("procur
+000161e0: 656d 656e 745f 6a69 745f 7374 6f63 6b22  ement_jit_stock"
+000161f0: 2c20 226d 6572 6765 6422 2c20 2270 726f  , "merged", "pro
+00016200: 6375 7265 6d65 6e74 5f6a 6974 2229 2c0a  curement_jit"),.
+00016210: 2020 2020 2822 7075 7263 6861 7365 5f61      ("purchase_a
+00016220: 6e61 6c79 7469 635f 706c 616e 7322 2c20  nalytic_plans", 
+00016230: 226f 6361 5f6d 6f76 6564 222c 2022 7075  "oca_moved", "pu
+00016240: 7263 6861 7365 5f61 6e61 6c79 7469 635f  rchase_analytic_
+00016250: 6469 7374 7269 6275 7469 6f6e 222c 0a20  distribution",. 
+00016260: 2020 2020 2020 2022 4d6f 7665 6420 746f         "Moved to
+00016270: 204f 4341 2f61 6363 6f75 6e74 2d61 6e61   OCA/account-ana
+00016280: 6c79 7469 6322 292c 0a20 2020 2028 2270  lytic"),.    ("p
+00016290: 7572 6368 6173 655f 646f 7562 6c65 5f76  urchase_double_v
+000162a0: 616c 6964 6174 696f 6e22 2c20 2272 656d  alidation", "rem
+000162b0: 6f76 6564 2229 2c0a 2020 2020 2822 7361  oved"),.    ("sa
+000162c0: 6c65 5f61 6e61 6c79 7469 635f 706c 616e  le_analytic_plan
+000162d0: 7322 2c20 226f 6361 5f6d 6f76 6564 222c  s", "oca_moved",
+000162e0: 2022 7361 6c65 5f61 6e61 6c79 7469 635f   "sale_analytic_
+000162f0: 6469 7374 7269 6275 7469 6f6e 222c 0a20  distribution",. 
+00016300: 2020 2020 2020 2022 4d6f 7665 6420 746f         "Moved to
+00016310: 204f 4341 2f61 6363 6f75 6e74 2d61 6e61   OCA/account-ana
+00016320: 6c79 7469 6322 292c 0a20 2020 2028 2273  lytic"),.    ("s
+00016330: 616c 655f 6a6f 7572 6e61 6c22 2c20 2272  ale_journal", "r
+00016340: 656d 6f76 6564 2229 2c0a 2020 2020 2822  emoved"),.    ("
+00016350: 7368 6172 6522 2c20 2272 656d 6f76 6564  share", "removed
+00016360: 2229 2c0a 2020 2020 2822 7374 6f63 6b5f  "),.    ("stock_
+00016370: 696e 766f 6963 655f 6469 7265 6374 6c79  invoice_directly
+00016380: 222c 2022 7265 6d6f 7665 6422 292c 0a20  ", "removed"),. 
+00016390: 2020 2028 2277 6562 5f61 7069 222c 2022     ("web_api", "
+000163a0: 7265 6d6f 7665 6422 292c 0a20 2020 2028  removed"),.    (
+000163b0: 2277 6562 5f67 616e 7474 222c 2022 6d65  "web_gantt", "me
+000163c0: 7267 6564 222c 2022 7765 6222 292c 0a20  rged", "web"),. 
+000163d0: 2020 2028 2277 6562 5f67 7261 7068 222c     ("web_graph",
+000163e0: 2022 6d65 7267 6564 222c 2022 7765 6222   "merged", "web"
+000163f0: 292c 0a20 2020 2028 2277 6562 5f6b 616e  ),.    ("web_kan
+00016400: 6261 6e5f 7370 6172 6b6c 696e 6522 2c20  ban_sparkline", 
+00016410: 226d 6572 6765 6422 2c20 2277 6562 2229  "merged", "web")
+00016420: 2c0a 2020 2020 2822 7765 625f 7465 7374  ,.    ("web_test
+00016430: 7322 2c20 226d 6572 6765 6422 2c20 2277  s", "merged", "w
+00016440: 6562 2229 2c0a 2020 2020 2822 7765 625f  eb"),.    ("web_
+00016450: 7465 7374 735f 6465 6d6f 222c 2022 7265  tests_demo", "re
+00016460: 6d6f 7665 6422 292c 0a20 2020 2028 2277  moved"),.    ("w
+00016470: 6562 7369 7465 5f63 6572 7469 6669 6361  ebsite_certifica
+00016480: 7469 6f6e 222c 2022 7265 6d6f 7665 6422  tion", "removed"
+00016490: 292c 0a20 2020 2028 2277 6562 7369 7465  ),.    ("website
+000164a0: 5f69 6e73 7461 6e74 636c 6963 6b22 2c20  _instantclick", 
+000164b0: 2272 656d 6f76 6564 2229 2c0a 2020 2020  "removed"),.    
+000164c0: 2822 7765 6273 6974 655f 6d61 696c 5f67  ("website_mail_g
+000164d0: 726f 7570 222c 2022 7265 6e61 6d65 6422  roup", "renamed"
+000164e0: 2c20 2277 6562 7369 7465 5f6d 6169 6c5f  , "website_mail_
+000164f0: 6368 616e 6e65 6c22 292c 0a20 2020 2028  channel"),.    (
+00016500: 2277 6562 7369 7465 5f72 6570 6f72 7422  "website_report"
+00016510: 2c20 226d 6572 6765 6422 2c20 2272 6570  , "merged", "rep
+00016520: 6f72 7422 292c 0a5d 0a0a 6966 205f 5f6e  ort"),.]..if __n
+00016530: 616d 655f 5f20 3d3d 2022 5f5f 6d61 696e  ame__ == "__main
+00016540: 5f5f 223a 0a20 2020 2070 6172 7365 7220  __":.    parser 
+00016550: 3d20 7a30 6c69 622e 7061 7273 656f 7074  = z0lib.parseopt
+00016560: 6172 6773 2822 4d69 6772 6174 6520 4f64  args("Migrate Od
+00016570: 6f6f 2044 4222 2c0a 2020 2020 2020 2020  oo DB",.        
 00016580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016590: 2020 2020 2020 22c2 a920 3230 3139 2d32        ".. 2019-2
-000165a0: 3120 6279 2053 4853 2d41 5620 732e 722e  1 by SHS-AV s.r.
-000165b0: 6c2e 222c 0a20 2020 2020 2020 2020 2020  l.",.           
+00016590: 2020 2020 2020 2020 22c2 a920 3230 3139          ".. 2019
+000165a0: 2d32 3120 6279 2053 4853 2d41 5620 732e  -21 by SHS-AV s.
+000165b0: 722e 6c2e 222c 0a20 2020 2020 2020 2020  r.l.",.         
 000165c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000165d0: 2020 2020 2076 6572 7369 6f6e 3d5f 5f76       version=__v
-000165e0: 6572 7369 6f6e 5f5f 290a 2020 2020 7061  ersion__).    pa
-000165f0: 7273 6572 2e61 6464 5f61 7267 756d 656e  rser.add_argumen
-00016600: 7428 272d 6827 290a 2020 2020 7061 7273  t('-h').    pars
-00016610: 6572 2e61 6464 5f61 7267 756d 656e 7428  er.add_argument(
-00016620: 222d 4222 2c20 222d 2d6f 7065 6e75 7067  "-B", "--openupg
-00016630: 7261 6465 2d62 7261 6e63 682d 7061 7468  rade-branch-path
-00016640: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00016650: 2020 2020 2020 2020 2020 2068 656c 703d             help=
-00016660: 226f 7065 6e75 7067 7261 6465 2062 7261  "openupgrade bra
-00016670: 6e63 6820 7061 7468 222c 0a20 2020 2020  nch path",.     
+000165d0: 2020 2020 2020 2076 6572 7369 6f6e 3d5f         version=_
+000165e0: 5f76 6572 7369 6f6e 5f5f 290a 2020 2020  _version__).    
+000165f0: 7061 7273 6572 2e61 6464 5f61 7267 756d  parser.add_argum
+00016600: 656e 7428 272d 6827 290a 2020 2020 7061  ent('-h').    pa
+00016610: 7273 6572 2e61 6464 5f61 7267 756d 656e  rser.add_argumen
+00016620: 7428 222d 4222 2c20 222d 2d6f 7065 6e75  t("-B", "--openu
+00016630: 7067 7261 6465 2d62 7261 6e63 682d 7061  pgrade-branch-pa
+00016640: 7468 222c 0a20 2020 2020 2020 2020 2020  th",.           
+00016650: 2020 2020 2020 2020 2020 2020 2068 656c               hel
+00016660: 703d 226f 7065 6e75 7067 7261 6465 2062  p="openupgrade b
+00016670: 7261 6e63 6820 7061 7468 222c 0a20 2020  ranch path",.   
 00016680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016690: 2020 2064 6573 743d 226f 7074 5f6f 7570     dest="opt_oup
-000166a0: 6174 6822 2c0a 2020 2020 2020 2020 2020  ath",.          
-000166b0: 2020 2020 2020 2020 2020 2020 2020 6d65                me
-000166c0: 7461 7661 723d 2270 6174 6822 290a 2020  tavar="path").  
-000166d0: 2020 7061 7273 6572 2e61 6464 5f61 7267    parser.add_arg
-000166e0: 756d 656e 7428 272d 6227 2c20 272d 2d62  ument('-b', '--b
-000166f0: 7261 6e63 6827 2c0a 2020 2020 2020 2020  ranch',.        
+00016690: 2020 2020 2064 6573 743d 226f 7074 5f6f       dest="opt_o
+000166a0: 7570 6174 6822 2c0a 2020 2020 2020 2020  upath",.        
+000166b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000166c0: 6d65 7461 7661 723d 2270 6174 6822 290a  metavar="path").
+000166d0: 2020 2020 7061 7273 6572 2e61 6464 5f61      parser.add_a
+000166e0: 7267 756d 656e 7428 272d 6227 2c20 272d  rgument('-b', '-
+000166f0: 2d62 7261 6e63 6827 2c0a 2020 2020 2020  -branch',.      
 00016700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016710: 6163 7469 6f6e 3d27 7374 6f72 6527 2c0a  action='store',.
-00016720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016730: 2020 2020 2020 2020 6465 7374 3d27 6669          dest='fi
-00016740: 6e61 6c5f 6272 616e 6368 272c 0a20 2020  nal_branch',.   
+00016710: 2020 6163 7469 6f6e 3d27 7374 6f72 6527    action='store'
+00016720: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00016730: 2020 2020 2020 2020 2020 6465 7374 3d27            dest='
+00016740: 6669 6e61 6c5f 6272 616e 6368 272c 0a20  final_branch',. 
 00016750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016760: 2020 2020 206d 6574 6176 6172 3d27 7665       metavar='ve
-00016770: 7273 696f 6e27 290a 2020 2020 7061 7273  rsion').    pars
-00016780: 6572 2e61 6464 5f61 7267 756d 656e 7428  er.add_argument(
-00016790: 222d 4322 2c20 222d 2d62 792d 636f 6d70  "-C", "--by-comp
-000167a0: 616e 7922 2c0a 2020 2020 2020 2020 2020  any",.          
-000167b0: 2020 2020 2020 2020 2020 2020 2020 6163                ac
-000167c0: 7469 6f6e 3d22 7374 6f72 655f 7472 7565  tion="store_true
-000167d0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-000167e0: 2020 2020 2020 2020 2020 2068 656c 703d             help=
-000167f0: 2273 656c 6563 7420 6f6e 6c79 2072 6563  "select only rec
-00016800: 6f72 6473 206f 6620 6d61 696e 2063 6f6d  ords of main com
-00016810: 7061 6e79 222c 0a20 2020 2020 2020 2020  pany",.         
-00016820: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00016830: 6573 743d 2262 795f 636f 6d70 616e 7922  est="by_company"
-00016840: 290a 2020 2020 7061 7273 6572 2e61 6464  ).    parser.add
-00016850: 5f61 7267 756d 656e 7428 222d 6322 2c20  _argument("-c", 
-00016860: 222d 2d74 6774 2d63 6f6e 6669 6722 2c0a  "--tgt-config",.
-00016870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016880: 2020 2020 2020 2020 6865 6c70 3d22 7461          help="ta
-00016890: 7267 6574 2044 4220 636f 6e66 6967 7572  rget DB configur
-000168a0: 6174 696f 6e20 6669 6c65 222c 0a20 2020  ation file",.   
+00016760: 2020 2020 2020 206d 6574 6176 6172 3d27         metavar='
+00016770: 7665 7273 696f 6e27 290a 2020 2020 7061  version').    pa
+00016780: 7273 6572 2e61 6464 5f61 7267 756d 656e  rser.add_argumen
+00016790: 7428 222d 4322 2c20 222d 2d62 792d 636f  t("-C", "--by-co
+000167a0: 6d70 616e 7922 2c0a 2020 2020 2020 2020  mpany",.        
+000167b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000167c0: 6163 7469 6f6e 3d22 7374 6f72 655f 7472  action="store_tr
+000167d0: 7565 222c 0a20 2020 2020 2020 2020 2020  ue",.           
+000167e0: 2020 2020 2020 2020 2020 2020 2068 656c               hel
+000167f0: 703d 2273 656c 6563 7420 6f6e 6c79 2072  p="select only r
+00016800: 6563 6f72 6473 206f 6620 6d61 696e 2063  ecords of main c
+00016810: 6f6d 7061 6e79 222c 0a20 2020 2020 2020  ompany",.       
+00016820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016830: 2064 6573 743d 2262 795f 636f 6d70 616e   dest="by_compan
+00016840: 7922 290a 2020 2020 7061 7273 6572 2e61  y").    parser.a
+00016850: 6464 5f61 7267 756d 656e 7428 222d 6322  dd_argument("-c"
+00016860: 2c20 222d 2d74 6774 2d63 6f6e 6669 6722  , "--tgt-config"
+00016870: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00016880: 2020 2020 2020 2020 2020 6865 6c70 3d22            help="
+00016890: 7461 7267 6574 2044 4220 636f 6e66 6967  target DB config
+000168a0: 7572 6174 696f 6e20 6669 6c65 222c 0a20  uration file",. 
 000168b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000168c0: 2020 2020 2064 6573 743d 2266 696e 616c       dest="final
-000168d0: 5f63 6f6e 666e 222c 0a20 2020 2020 2020  _confn",.       
+000168c0: 2020 2020 2020 2064 6573 743d 2266 696e         dest="fin
+000168d0: 616c 5f63 6f6e 666e 222c 0a20 2020 2020  al_confn",.     
 000168e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000168f0: 206d 6574 6176 6172 3d22 6669 6c65 2229   metavar="file")
-00016900: 0a20 2020 2070 6172 7365 722e 6164 645f  .    parser.add_
-00016910: 6172 6775 6d65 6e74 2822 2d44 222c 2022  argument("-D", "
-00016920: 2d2d 6465 6c2d 6462 2d69 662d 6578 6973  --del-db-if-exis
-00016930: 7422 2c0a 2020 2020 2020 2020 2020 2020  t",.            
-00016940: 2020 2020 2020 2020 2020 2020 6163 7469              acti
-00016950: 6f6e 3d22 7374 6f72 655f 7472 7565 222c  on="store_true",
-00016960: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016970: 2020 2020 2020 2020 2064 6573 743d 226f           dest="o
-00016980: 7074 5f64 656c 2229 0a20 2020 2070 6172  pt_del").    par
-00016990: 7365 722e 6164 645f 6172 6775 6d65 6e74  ser.add_argument
-000169a0: 2822 2d64 222c 2022 2d2d 7467 742d 6462  ("-d", "--tgt-db
-000169b0: 5f6e 616d 6522 2c0a 2020 2020 2020 2020  _name",.        
+000168f0: 2020 206d 6574 6176 6172 3d22 6669 6c65     metavar="file
+00016900: 2229 0a20 2020 2070 6172 7365 722e 6164  ").    parser.ad
+00016910: 645f 6172 6775 6d65 6e74 2822 2d44 222c  d_argument("-D",
+00016920: 2022 2d2d 6465 6c2d 6462 2d69 662d 6578   "--del-db-if-ex
+00016930: 6973 7422 2c0a 2020 2020 2020 2020 2020  ist",.          
+00016940: 2020 2020 2020 2020 2020 2020 2020 6163                ac
+00016950: 7469 6f6e 3d22 7374 6f72 655f 7472 7565  tion="store_true
+00016960: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00016970: 2020 2020 2020 2020 2020 2064 6573 743d             dest=
+00016980: 226f 7074 5f64 656c 2229 0a20 2020 2070  "opt_del").    p
+00016990: 6172 7365 722e 6164 645f 6172 6775 6d65  arser.add_argume
+000169a0: 6e74 2822 2d64 222c 2022 2d2d 7467 742d  nt("-d", "--tgt-
+000169b0: 6462 5f6e 616d 6522 2c0a 2020 2020 2020  db_name",.      
 000169c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000169d0: 6865 6c70 3d22 7461 7267 6574 2064 6174  help="target dat
-000169e0: 6162 6173 6520 6e61 6d65 222c 0a20 2020  abase name",.   
+000169d0: 2020 6865 6c70 3d22 7461 7267 6574 2064    help="target d
+000169e0: 6174 6162 6173 6520 6e61 6d65 222c 0a20  atabase name",. 
 000169f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016a00: 2020 2020 2064 6573 743d 2266 696e 616c       dest="final
-00016a10: 5f64 626e 616d 6522 2c0a 2020 2020 2020  _dbname",.      
+00016a00: 2020 2020 2020 2064 6573 743d 2266 696e         dest="fin
+00016a10: 616c 5f64 626e 616d 6522 2c0a 2020 2020  al_dbname",.    
 00016a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016a30: 2020 6d65 7461 7661 723d 226e 616d 6522    metavar="name"
-00016a40: 290a 2020 2020 7061 7273 6572 2e61 6464  ).    parser.add
-00016a50: 5f61 7267 756d 656e 7428 222d 4522 2c20  _argument("-E", 
-00016a60: 222d 2d6e 6f2d 7665 6e76 222c 0a20 2020  "--no-venv",.   
+00016a30: 2020 2020 6d65 7461 7661 723d 226e 616d      metavar="nam
+00016a40: 6522 290a 2020 2020 7061 7273 6572 2e61  e").    parser.a
+00016a50: 6464 5f61 7267 756d 656e 7428 222d 4522  dd_argument("-E"
+00016a60: 2c20 222d 2d6e 6f2d 7665 6e76 222c 0a20  , "--no-venv",. 
 00016a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016a80: 2020 2020 2068 656c 703d 2264 6973 6162       help="disab
-00016a90: 6c65 2076 6972 7475 616c 656e 7622 2c0a  le virtualenv",.
-00016aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ab0: 2020 2020 2020 2020 6163 7469 6f6e 3d27          action='
-00016ac0: 7374 6f72 655f 7472 7565 272c 0a20 2020  store_true',.   
+00016a80: 2020 2020 2020 2068 656c 703d 2264 6973         help="dis
+00016a90: 6162 6c65 2076 6972 7475 616c 656e 7622  able virtualenv"
+00016aa0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00016ab0: 2020 2020 2020 2020 2020 6163 7469 6f6e            action
+00016ac0: 3d27 7374 6f72 655f 7472 7565 272c 0a20  ='store_true',. 
 00016ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ae0: 2020 2020 2064 6573 743d 226e 6f5f 7665       dest="no_ve
-00016af0: 6e76 2229 0a20 2020 2070 6172 7365 722e  nv").    parser.
-00016b00: 6164 645f 6172 6775 6d65 6e74 2827 2d46  add_argument('-F
-00016b10: 272c 2027 2d2d 6672 6f6d 2d6f 646f 6f2d  ', '--from-odoo-
-00016b20: 7665 7227 2c0a 2020 2020 2020 2020 2020  ver',.          
-00016b30: 2020 2020 2020 2020 2020 2020 2020 6163                ac
-00016b40: 7469 6f6e 3d27 7374 6f72 6527 2c0a 2020  tion='store',.  
+00016ae0: 2020 2020 2020 2064 6573 743d 226e 6f5f         dest="no_
+00016af0: 7665 6e76 2229 0a20 2020 2070 6172 7365  venv").    parse
+00016b00: 722e 6164 645f 6172 6775 6d65 6e74 2827  r.add_argument('
+00016b10: 2d46 272c 2027 2d2d 6672 6f6d 2d6f 646f  -F', '--from-odo
+00016b20: 6f2d 7665 7227 2c0a 2020 2020 2020 2020  o-ver',.        
+00016b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016b40: 6163 7469 6f6e 3d27 7374 6f72 6527 2c0a  action='store',.
 00016b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016b60: 2020 2020 2020 6465 7374 3d27 6672 6f6d        dest='from
-00016b70: 5f62 7261 6e63 6827 2c0a 2020 2020 2020  _branch',.      
+00016b60: 2020 2020 2020 2020 6465 7374 3d27 6672          dest='fr
+00016b70: 6f6d 5f62 7261 6e63 6827 2c0a 2020 2020  om_branch',.    
 00016b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016b90: 2020 6d65 7461 7661 723d 2276 6572 2229    metavar="ver")
-00016ba0: 0a20 2020 2070 6172 7365 722e 6164 645f  .    parser.add_
-00016bb0: 6172 6775 6d65 6e74 2822 2d49 222c 2022  argument("-I", "
-00016bc0: 2d2d 696d 6167 6522 2c0a 2020 2020 2020  --image",.      
+00016b90: 2020 2020 6d65 7461 7661 723d 2276 6572      metavar="ver
+00016ba0: 2229 0a20 2020 2070 6172 7365 722e 6164  ").    parser.ad
+00016bb0: 645f 6172 6775 6d65 6e74 2822 2d49 222c  d_argument("-I",
+00016bc0: 2022 2d2d 696d 6167 6522 2c0a 2020 2020   "--image",.    
 00016bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016be0: 2020 6865 6c70 3d22 696d 6167 6520 6d6f    help="image mo
-00016bf0: 6465 222c 0a20 2020 2020 2020 2020 2020  de",.           
-00016c00: 2020 2020 2020 2020 2020 2020 2061 6374               act
-00016c10: 696f 6e3d 2773 746f 7265 5f74 7275 6527  ion='store_true'
-00016c20: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00016c30: 2020 2020 2020 2020 2020 6465 7374 3d22            dest="
-00016c40: 696d 6167 655f 6d6f 6465 222c 0a20 2020  image_mode",.   
+00016be0: 2020 2020 6865 6c70 3d22 696d 6167 6520      help="image 
+00016bf0: 6d6f 6465 222c 0a20 2020 2020 2020 2020  mode",.         
+00016c00: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00016c10: 6374 696f 6e3d 2773 746f 7265 5f74 7275  ction='store_tru
+00016c20: 6527 2c0a 2020 2020 2020 2020 2020 2020  e',.            
+00016c30: 2020 2020 2020 2020 2020 2020 6465 7374              dest
+00016c40: 3d22 696d 6167 655f 6d6f 6465 222c 0a20  ="image_mode",. 
 00016c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016c60: 2020 2020 2064 6566 6175 6c74 3d46 616c       default=Fal
-00016c70: 7365 290a 2020 2020 7061 7273 6572 2e61  se).    parser.a
-00016c80: 6464 5f61 7267 756d 656e 7428 222d 6922  dd_argument("-i"
-00016c90: 2c20 222d 2d69 6473 222c 0a20 2020 2020  , "--ids",.     
+00016c60: 2020 2020 2020 2064 6566 6175 6c74 3d46         default=F
+00016c70: 616c 7365 290a 2020 2020 7061 7273 6572  alse).    parser
+00016c80: 2e61 6464 5f61 7267 756d 656e 7428 222d  .add_argument("-
+00016c90: 6922 2c20 222d 2d69 6473 222c 0a20 2020  i", "--ids",.   
 00016ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016cb0: 2020 2068 656c 703d 2269 6473 2074 6f20     help="ids to 
-00016cc0: 6d69 6772 6174 6522 2c0a 2020 2020 2020  migrate",.      
+00016cb0: 2020 2020 2068 656c 703d 2269 6473 2074       help="ids t
+00016cc0: 6f20 6d69 6772 6174 6522 2c0a 2020 2020  o migrate",.    
 00016cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ce0: 2020 6465 7374 3d22 7365 6c5f 6964 7322    dest="sel_ids"
-00016cf0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00016d00: 2020 2020 2020 2020 2020 6d65 7461 7661            metava
-00016d10: 723d 226c 6973 7422 290a 2020 2020 7061  r="list").    pa
-00016d20: 7273 6572 2e61 6464 5f61 7267 756d 656e  rser.add_argumen
-00016d30: 7428 222d 4a22 2c20 222d 2d74 7279 2d72  t("-J", "--try-r
-00016d40: 6569 6e73 7461 6c6c 222c 0a20 2020 2020  einstall",.     
+00016ce0: 2020 2020 6465 7374 3d22 7365 6c5f 6964      dest="sel_id
+00016cf0: 7322 2c0a 2020 2020 2020 2020 2020 2020  s",.            
+00016d00: 2020 2020 2020 2020 2020 2020 6d65 7461              meta
+00016d10: 7661 723d 226c 6973 7422 290a 2020 2020  var="list").    
+00016d20: 7061 7273 6572 2e61 6464 5f61 7267 756d  parser.add_argum
+00016d30: 656e 7428 222d 4a22 2c20 222d 2d74 7279  ent("-J", "--try
+00016d40: 2d72 6569 6e73 7461 6c6c 222c 0a20 2020  -reinstall",.   
 00016d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016d60: 2020 2068 656c 703d 2274 7279 2074 6f20     help="try to 
-00016d70: 7265 696e 7374 616c 6c22 2c0a 2020 2020  reinstall",.    
+00016d60: 2020 2020 2068 656c 703d 2274 7279 2074       help="try t
+00016d70: 6f20 7265 696e 7374 616c 6c22 2c0a 2020  o reinstall",.  
 00016d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016d90: 2020 2020 6163 7469 6f6e 3d27 7374 6f72      action='stor
-00016da0: 655f 7472 7565 272c 0a20 2020 2020 2020  e_true',.       
+00016d90: 2020 2020 2020 6163 7469 6f6e 3d27 7374        action='st
+00016da0: 6f72 655f 7472 7565 272c 0a20 2020 2020  ore_true',.     
 00016db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016dc0: 2064 6573 743d 2274 7279 5f72 6569 6e73   dest="try_reins
-00016dd0: 7461 6c6c 222c 0a20 2020 2020 2020 2020  tall",.         
-00016de0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00016df0: 6566 6175 6c74 3d46 616c 7365 290a 2020  efault=False).  
-00016e00: 2020 7061 7273 6572 2e61 6464 5f61 7267    parser.add_arg
-00016e10: 756d 656e 7428 222d 4b22 2c20 222d 2d63  ument("-K", "--c
-00016e20: 6f6d 6d61 6e64 2d66 696c 6522 2c0a 2020  ommand-file",.  
+00016dc0: 2020 2064 6573 743d 2274 7279 5f72 6569     dest="try_rei
+00016dd0: 6e73 7461 6c6c 222c 0a20 2020 2020 2020  nstall",.       
+00016de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016df0: 2064 6566 6175 6c74 3d46 616c 7365 290a   default=False).
+00016e00: 2020 2020 7061 7273 6572 2e61 6464 5f61      parser.add_a
+00016e10: 7267 756d 656e 7428 222d 4b22 2c20 222d  rgument("-K", "-
+00016e20: 2d63 6f6d 6d61 6e64 2d66 696c 6522 2c0a  -command-file",.
 00016e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016e40: 2020 2020 2020 6865 6c70 3d22 6d69 6772        help="migr
-00016e50: 6174 696f 6e20 636f 6d6d 616e 6420 6669  ation command fi
-00016e60: 6c65 222c 0a20 2020 2020 2020 2020 2020  le",.           
-00016e70: 2020 2020 2020 2020 2020 2020 2064 6573               des
-00016e80: 743d 2263 6f6d 6d61 6e64 5f66 696c 6522  t="command_file"
-00016e90: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00016ea0: 2020 2020 2020 2020 2020 6d65 7461 7661            metava
-00016eb0: 723d 2266 696c 6522 2c0a 2020 2020 2020  r="file",.      
+00016e40: 2020 2020 2020 2020 6865 6c70 3d22 6d69          help="mi
+00016e50: 6772 6174 696f 6e20 636f 6d6d 616e 6420  gration command 
+00016e60: 6669 6c65 222c 0a20 2020 2020 2020 2020  file",.         
+00016e70: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00016e80: 6573 743d 2263 6f6d 6d61 6e64 5f66 696c  est="command_fil
+00016e90: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
+00016ea0: 2020 2020 2020 2020 2020 2020 6d65 7461              meta
+00016eb0: 7661 723d 2266 696c 6522 2c0a 2020 2020  var="file",.    
 00016ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ed0: 2020 6465 6661 756c 743d 272e 2f6d 6967    default='./mig
-00016ee0: 7261 7465 5f6f 646f 6f2e 6373 7627 290a  rate_odoo.csv').
-00016ef0: 2020 2020 7061 7273 6572 2e61 6464 5f61      parser.add_a
-00016f00: 7267 756d 656e 7428 222d 6b22 2c20 222d  rgument("-k", "-
-00016f10: 2d64 6566 6175 6c74 2d62 6568 6176 696f  -default-behavio
-00016f20: 7222 2c0a 2020 2020 2020 2020 2020 2020  r",.            
-00016f30: 2020 2020 2020 2020 2020 2020 6865 6c70              help
-00016f40: 3d22 6465 6661 756c 7420 6265 6861 7669  ="default behavi
-00016f50: 6f72 222c 0a20 2020 2020 2020 2020 2020  or",.           
-00016f60: 2020 2020 2020 2020 2020 2020 2061 6374               act
-00016f70: 696f 6e3d 2273 746f 7265 5f74 7275 6522  ion="store_true"
-00016f80: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00016f90: 2020 2020 2020 2020 2020 6465 7374 3d22            dest="
-00016fa0: 6465 6661 756c 745f 6265 6861 7669 6f72  default_behavior
-00016fb0: 2229 0a20 2020 2070 6172 7365 722e 6164  ").    parser.ad
-00016fc0: 645f 6172 6775 6d65 6e74 2822 2d6c 222c  d_argument("-l",
-00016fd0: 2022 2d2d 6669 6c65 2d6c 6f67 222c 0a20   "--file-log",. 
-00016fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ff0: 2020 2020 2020 2068 656c 703d 226c 6f67         help="log
-00017000: 2066 696c 6522 2c0a 2020 2020 2020 2020   file",.        
+00016ed0: 2020 2020 6465 6661 756c 743d 272e 2f6d      default='./m
+00016ee0: 6967 7261 7465 5f6f 646f 6f2e 6373 7627  igrate_odoo.csv'
+00016ef0: 290a 2020 2020 7061 7273 6572 2e61 6464  ).    parser.add
+00016f00: 5f61 7267 756d 656e 7428 222d 6b22 2c20  _argument("-k", 
+00016f10: 222d 2d64 6566 6175 6c74 2d62 6568 6176  "--default-behav
+00016f20: 696f 7222 2c0a 2020 2020 2020 2020 2020  ior",.          
+00016f30: 2020 2020 2020 2020 2020 2020 2020 6865                he
+00016f40: 6c70 3d22 6465 6661 756c 7420 6265 6861  lp="default beha
+00016f50: 7669 6f72 222c 0a20 2020 2020 2020 2020  vior",.         
+00016f60: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00016f70: 6374 696f 6e3d 2273 746f 7265 5f74 7275  ction="store_tru
+00016f80: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
+00016f90: 2020 2020 2020 2020 2020 2020 6465 7374              dest
+00016fa0: 3d22 6465 6661 756c 745f 6265 6861 7669  ="default_behavi
+00016fb0: 6f72 2229 0a20 2020 2070 6172 7365 722e  or").    parser.
+00016fc0: 6164 645f 6172 6775 6d65 6e74 2822 2d6c  add_argument("-l
+00016fd0: 222c 2022 2d2d 6669 6c65 2d6c 6f67 222c  ", "--file-log",
+00016fe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016ff0: 2020 2020 2020 2020 2068 656c 703d 226c           help="l
+00017000: 6f67 2066 696c 6522 2c0a 2020 2020 2020  og file",.      
 00017010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017020: 6465 7374 3d22 6c6f 6766 6e22 2c0a 2020  dest="logfn",.  
+00017020: 2020 6465 7374 3d22 6c6f 6766 6e22 2c0a    dest="logfn",.
 00017030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017040: 2020 2020 2020 6d65 7461 7661 723d 2266        metavar="f
-00017050: 696c 6522 290a 2020 2020 7061 7273 6572  ile").    parser
-00017060: 2e61 6464 5f61 7267 756d 656e 7428 222d  .add_argument("-
-00017070: 4d22 2c20 222d 2d6f 6361 2d6d 6967 7261  M", "--oca-migra
-00017080: 7465 222c 0a20 2020 2020 2020 2020 2020  te",.           
-00017090: 2020 2020 2020 2020 2020 2020 2061 6374               act
-000170a0: 696f 6e3d 2273 746f 7265 5f74 7275 6522  ion="store_true"
-000170b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000170c0: 2020 2020 2020 2020 2020 6465 7374 3d22            dest="
-000170d0: 6f63 615f 6d69 6772 6174 6522 2c0a 2020  oca_migrate",.  
+00017040: 2020 2020 2020 2020 6d65 7461 7661 723d          metavar=
+00017050: 2266 696c 6522 290a 2020 2020 7061 7273  "file").    pars
+00017060: 6572 2e61 6464 5f61 7267 756d 656e 7428  er.add_argument(
+00017070: 222d 4d22 2c20 222d 2d6f 6361 2d6d 6967  "-M", "--oca-mig
+00017080: 7261 7465 222c 0a20 2020 2020 2020 2020  rate",.         
+00017090: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+000170a0: 6374 696f 6e3d 2273 746f 7265 5f74 7275  ction="store_tru
+000170b0: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
+000170c0: 2020 2020 2020 2020 2020 2020 6465 7374              dest
+000170d0: 3d22 6f63 615f 6d69 6772 6174 6522 2c0a  ="oca_migrate",.
 000170e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000170f0: 2020 2020 2020 6865 6c70 3d22 7573 6520        help="use 
-00017100: 4f43 4120 6d69 6772 6174 6520 2866 696e  OCA migrate (fin
-00017110: 616c 2076 6572 7369 6f6e 203c 2031 302e  al version < 10.
-00017120: 3029 2229 0a20 2020 2070 6172 7365 722e  0)").    parser.
-00017130: 6164 645f 6172 6775 6d65 6e74 2822 2d6d  add_argument("-m
-00017140: 222c 2022 2d2d 7365 6c2d 6d6f 6465 6c22  ", "--sel-model"
-00017150: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00017160: 2020 2020 2020 2020 2020 6865 6c70 3d22            help="
-00017170: 6d6f 6465 6c20 746f 206d 6967 7261 7465  model to migrate
-00017180: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00017190: 2020 2020 2020 2020 2020 2064 6573 743d             dest=
-000171a0: 2273 656c 5f6d 6f64 656c 222c 0a20 2020  "sel_model",.   
+000170f0: 2020 2020 2020 2020 6865 6c70 3d22 7573          help="us
+00017100: 6520 4f43 4120 6d69 6772 6174 6520 2866  e OCA migrate (f
+00017110: 696e 616c 2076 6572 7369 6f6e 203c 2031  inal version < 1
+00017120: 302e 3029 2229 0a20 2020 2070 6172 7365  0.0)").    parse
+00017130: 722e 6164 645f 6172 6775 6d65 6e74 2822  r.add_argument("
+00017140: 2d6d 222c 2022 2d2d 7365 6c2d 6d6f 6465  -m", "--sel-mode
+00017150: 6c22 2c0a 2020 2020 2020 2020 2020 2020  l",.            
+00017160: 2020 2020 2020 2020 2020 2020 6865 6c70              help
+00017170: 3d22 6d6f 6465 6c20 746f 206d 6967 7261  ="model to migra
+00017180: 7465 222c 0a20 2020 2020 2020 2020 2020  te",.           
+00017190: 2020 2020 2020 2020 2020 2020 2064 6573               des
+000171a0: 743d 2273 656c 5f6d 6f64 656c 222c 0a20  t="sel_model",. 
 000171b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000171c0: 2020 2020 206d 6574 6176 6172 3d22 6e61       metavar="na
-000171d0: 6d65 2229 0a20 2020 2070 6172 7365 722e  me").    parser.
-000171e0: 6164 645f 6172 6775 6d65 6e74 2827 2d6e  add_argument('-n
-000171f0: 2729 0a20 2020 2070 6172 7365 722e 6164  ').    parser.ad
-00017200: 645f 6172 6775 6d65 6e74 2822 2d4f 222c  d_argument("-O",
-00017210: 2022 2d2d 6f70 656e 7570 6772 6164 656c   "--openupgradel
-00017220: 6962 2d70 6174 6822 2c0a 2020 2020 2020  ib-path",.      
+000171c0: 2020 2020 2020 206d 6574 6176 6172 3d22         metavar="
+000171d0: 6e61 6d65 2229 0a20 2020 2070 6172 7365  name").    parse
+000171e0: 722e 6164 645f 6172 6775 6d65 6e74 2827  r.add_argument('
+000171f0: 2d6e 2729 0a20 2020 2070 6172 7365 722e  -n').    parser.
+00017200: 6164 645f 6172 6775 6d65 6e74 2822 2d4f  add_argument("-O
+00017210: 222c 2022 2d2d 6f70 656e 7570 6772 6164  ", "--openupgrad
+00017220: 656c 6962 2d70 6174 6822 2c0a 2020 2020  elib-path",.    
 00017230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017240: 2020 6865 6c70 3d22 4f70 656e 7570 6772    help="Openupgr
-00017250: 6164 656c 6962 2070 6174 6822 2c0a 2020  adelib path",.  
+00017240: 2020 2020 6865 6c70 3d22 4f70 656e 7570      help="Openup
+00017250: 6772 6164 656c 6962 2070 6174 6822 2c0a  gradelib path",.
 00017260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017270: 2020 2020 2020 6465 7374 3d22 6f70 745f        dest="opt_
-00017280: 6f75 6c70 6174 6822 2c0a 2020 2020 2020  oulpath",.      
+00017270: 2020 2020 2020 2020 6465 7374 3d22 6f70          dest="op
+00017280: 745f 6f75 6c70 6174 6822 2c0a 2020 2020  t_oulpath",.    
 00017290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000172a0: 2020 6d65 7461 7661 723d 2270 6174 6822    metavar="path"
-000172b0: 290a 2020 2020 7061 7273 6572 2e61 6464  ).    parser.add
-000172c0: 5f61 7267 756d 656e 7428 272d 7127 290a  _argument('-q').
-000172d0: 2020 2020 7061 7273 6572 2e61 6464 5f61      parser.add_a
-000172e0: 7267 756d 656e 7428 222d 5222 2c20 222d  rgument("-R", "-
-000172f0: 2d72 6564 7563 7465 642d 6d6f 6475 6c65  -reducted-module
-00017300: 2d73 6574 222c 0a20 2020 2020 2020 2020  -set",.         
-00017310: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00017320: 6374 696f 6e3d 2773 746f 7265 5f74 7275  ction='store_tru
-00017330: 6527 2c0a 2020 2020 2020 2020 2020 2020  e',.            
-00017340: 2020 2020 2020 2020 2020 2020 6465 7374              dest
-00017350: 3d22 7265 6475 6374 6564 5f6d 6f64 756c  ="reducted_modul
-00017360: 655f 7365 7422 2c0a 2020 2020 2020 2020  e_set",.        
+000172a0: 2020 2020 6d65 7461 7661 723d 2270 6174      metavar="pat
+000172b0: 6822 290a 2020 2020 7061 7273 6572 2e61  h").    parser.a
+000172c0: 6464 5f61 7267 756d 656e 7428 272d 7127  dd_argument('-q'
+000172d0: 290a 2020 2020 7061 7273 6572 2e61 6464  ).    parser.add
+000172e0: 5f61 7267 756d 656e 7428 222d 5222 2c20  _argument("-R", 
+000172f0: 222d 2d72 6564 7563 7465 642d 6d6f 6475  "--reducted-modu
+00017300: 6c65 2d73 6574 222c 0a20 2020 2020 2020  le-set",.       
+00017310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017320: 2061 6374 696f 6e3d 2773 746f 7265 5f74   action='store_t
+00017330: 7275 6527 2c0a 2020 2020 2020 2020 2020  rue',.          
+00017340: 2020 2020 2020 2020 2020 2020 2020 6465                de
+00017350: 7374 3d22 7265 6475 6374 6564 5f6d 6f64  st="reducted_mod
+00017360: 756c 655f 7365 7422 2c0a 2020 2020 2020  ule_set",.      
 00017370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017380: 6465 6661 756c 743d 4661 6c73 6529 0a20  default=False). 
-00017390: 2020 2070 6172 7365 722e 6164 645f 6172     parser.add_ar
-000173a0: 6775 6d65 6e74 2822 2d53 222c 2022 2d2d  gument("-S", "--
-000173b0: 7361 6665 2d6d 6f64 6522 2c0a 2020 2020  safe-mode",.    
+00017380: 2020 6465 6661 756c 743d 4661 6c73 6529    default=False)
+00017390: 0a20 2020 2070 6172 7365 722e 6164 645f  .    parser.add_
+000173a0: 6172 6775 6d65 6e74 2822 2d53 222c 2022  argument("-S", "
+000173b0: 2d2d 7361 6665 2d6d 6f64 6522 2c0a 2020  --safe-mode",.  
 000173c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000173d0: 2020 2020 6163 7469 6f6e 3d22 7374 6f72      action="stor
-000173e0: 655f 7472 7565 222c 0a20 2020 2020 2020  e_true",.       
+000173d0: 2020 2020 2020 6163 7469 6f6e 3d22 7374        action="st
+000173e0: 6f72 655f 7472 7565 222c 0a20 2020 2020  ore_true",.     
 000173f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017400: 2064 6573 743d 226f 7074 5f73 6166 6522   dest="opt_safe"
-00017410: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00017420: 2020 2020 2020 2020 2020 6865 6c70 3d22            help="
-00017430: 7361 6665 206d 6f64 6522 290a 2020 2020  safe mode").    
-00017440: 7061 7273 6572 2e61 6464 5f61 7267 756d  parser.add_argum
-00017450: 656e 7428 222d 7322 2c20 222d 2d75 7365  ent("-s", "--use
-00017460: 2d73 796e 6368 726f 222c 0a20 2020 2020  -synchro",.     
+00017400: 2020 2064 6573 743d 226f 7074 5f73 6166     dest="opt_saf
+00017410: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
+00017420: 2020 2020 2020 2020 2020 2020 6865 6c70              help
+00017430: 3d22 7361 6665 206d 6f64 6522 290a 2020  ="safe mode").  
+00017440: 2020 7061 7273 6572 2e61 6464 5f61 7267    parser.add_arg
+00017450: 756d 656e 7428 222d 7322 2c20 222d 2d75  ument("-s", "--u
+00017460: 7365 2d73 796e 6368 726f 222c 0a20 2020  se-synchro",.   
 00017470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017480: 2020 2068 656c 703d 2275 7365 206d 6f64     help="use mod
-00017490: 756c 6520 7379 6e63 6872 6f22 2c0a 2020  ule synchro",.  
+00017480: 2020 2020 2068 656c 703d 2275 7365 206d       help="use m
+00017490: 6f64 756c 6520 7379 6e63 6872 6f22 2c0a  odule synchro",.
 000174a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000174b0: 2020 2020 2020 6163 7469 6f6e 3d27 7374        action='st
-000174c0: 6f72 655f 7472 7565 272c 0a20 2020 2020  ore_true',.     
+000174b0: 2020 2020 2020 2020 6163 7469 6f6e 3d27          action='
+000174c0: 7374 6f72 655f 7472 7565 272c 0a20 2020  store_true',.   
 000174d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000174e0: 2020 2064 6573 743d 2275 7365 5f73 796e     dest="use_syn
-000174f0: 6368 726f 222c 0a20 2020 2020 2020 2020  chro",.         
-00017500: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00017510: 6566 6175 6c74 3d46 616c 7365 290a 2020  efault=False).  
-00017520: 2020 7061 7273 6572 2e61 6464 5f61 7267    parser.add_arg
-00017530: 756d 656e 7428 222d 5422 2c20 222d 2d75  ument("-T", "--u
-00017540: 7064 2d74 7261 6e73 6c61 7469 6f6e 222c  pd-translation",
-00017550: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017560: 2020 2020 2020 2020 2061 6374 696f 6e3d           action=
-00017570: 2773 746f 7265 5f74 7275 6527 2c0a 2020  'store_true',.  
+000174e0: 2020 2020 2064 6573 743d 2275 7365 5f73       dest="use_s
+000174f0: 796e 6368 726f 222c 0a20 2020 2020 2020  ynchro",.       
+00017500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017510: 2064 6566 6175 6c74 3d46 616c 7365 290a   default=False).
+00017520: 2020 2020 7061 7273 6572 2e61 6464 5f61      parser.add_a
+00017530: 7267 756d 656e 7428 222d 5422 2c20 222d  rgument("-T", "-
+00017540: 2d75 7064 2d74 7261 6e73 6c61 7469 6f6e  -upd-translation
+00017550: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00017560: 2020 2020 2020 2020 2020 2061 6374 696f             actio
+00017570: 6e3d 2773 746f 7265 5f74 7275 6527 2c0a  n='store_true',.
 00017580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017590: 2020 2020 2020 6465 7374 3d22 7570 645f        dest="upd_
-000175a0: 7472 616e 736c 6174 696f 6e22 2c0a 2020  translation",.  
+00017590: 2020 2020 2020 2020 6465 7374 3d22 7570          dest="up
+000175a0: 645f 7472 616e 736c 6174 696f 6e22 2c0a  d_translation",.
 000175b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000175c0: 2020 2020 2020 6465 6661 756c 743d 4661        default=Fa
-000175d0: 6c73 6529 0a20 2020 2070 6172 7365 722e  lse).    parser.
-000175e0: 6164 645f 6172 6775 6d65 6e74 2822 2d55  add_argument("-U
-000175f0: 222c 2022 2d2d 7573 6572 222c 0a20 2020  ", "--user",.   
+000175c0: 2020 2020 2020 2020 6465 6661 756c 743d          default=
+000175d0: 4661 6c73 6529 0a20 2020 2070 6172 7365  False).    parse
+000175e0: 722e 6164 645f 6172 6775 6d65 6e74 2822  r.add_argument("
+000175f0: 2d55 222c 2022 2d2d 7573 6572 222c 0a20  -U", "--user",. 
 00017600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017610: 2020 2020 2068 656c 703d 226c 6f67 696e       help="login
-00017620: 2075 7365 726e 616d 6522 2c0a 2020 2020   username",.    
+00017610: 2020 2020 2020 2068 656c 703d 226c 6f67         help="log
+00017620: 696e 2075 7365 726e 616d 6522 2c0a 2020  in username",.  
 00017630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017640: 2020 2020 6465 7374 3d22 6c67 695f 7573      dest="lgi_us
-00017650: 6572 222c 0a20 2020 2020 2020 2020 2020  er",.           
-00017660: 2020 2020 2020 2020 2020 2020 206d 6574               met
-00017670: 6176 6172 3d22 7573 6572 6e61 6d65 222c  avar="username",
-00017680: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017690: 2020 2020 2020 2020 2064 6566 6175 6c74           default
-000176a0: 3d22 6164 6d69 6e22 290a 2020 2020 7061  ="admin").    pa
-000176b0: 7273 6572 2e61 6464 5f61 7267 756d 656e  rser.add_argumen
-000176c0: 7428 272d 5627 290a 2020 2020 7061 7273  t('-V').    pars
-000176d0: 6572 2e61 6464 5f61 7267 756d 656e 7428  er.add_argument(
-000176e0: 272d 7627 290a 2020 2020 7061 7273 6572  '-v').    parser
-000176f0: 2e61 6464 5f61 7267 756d 656e 7428 222d  .add_argument("-
-00017700: 5722 2c20 222d 2d77 6570 2d6c 6f67 222c  W", "--wep-log",
-00017710: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017720: 2020 2020 2020 2020 2068 656c 703d 2264           help="d
-00017730: 656c 206c 6f67 7320 6265 666f 7265 206d  el logs before m
-00017740: 6967 7261 7469 6f6e 222c 0a20 2020 2020  igration",.     
+00017640: 2020 2020 2020 6465 7374 3d22 6c67 695f        dest="lgi_
+00017650: 7573 6572 222c 0a20 2020 2020 2020 2020  user",.         
+00017660: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00017670: 6574 6176 6172 3d22 7573 6572 6e61 6d65  etavar="username
+00017680: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00017690: 2020 2020 2020 2020 2020 2064 6566 6175             defau
+000176a0: 6c74 3d22 6164 6d69 6e22 290a 2020 2020  lt="admin").    
+000176b0: 7061 7273 6572 2e61 6464 5f61 7267 756d  parser.add_argum
+000176c0: 656e 7428 272d 5627 290a 2020 2020 7061  ent('-V').    pa
+000176d0: 7273 6572 2e61 6464 5f61 7267 756d 656e  rser.add_argumen
+000176e0: 7428 272d 7627 290a 2020 2020 7061 7273  t('-v').    pars
+000176f0: 6572 2e61 6464 5f61 7267 756d 656e 7428  er.add_argument(
+00017700: 222d 5722 2c20 222d 2d77 6570 2d6c 6f67  "-W", "--wep-log
+00017710: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00017720: 2020 2020 2020 2020 2020 2068 656c 703d             help=
+00017730: 2264 656c 206c 6f67 7320 6265 666f 7265  "del logs before
+00017740: 206d 6967 7261 7469 6f6e 222c 0a20 2020   migration",.   
 00017750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017760: 2020 2061 6374 696f 6e3d 2773 746f 7265     action='store
-00017770: 5f74 7275 6527 2c0a 2020 2020 2020 2020  _true',.        
+00017760: 2020 2020 2061 6374 696f 6e3d 2773 746f       action='sto
+00017770: 7265 5f74 7275 6527 2c0a 2020 2020 2020  re_true',.      
 00017780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017790: 6465 7374 3d22 7765 705f 6c6f 6773 222c  dest="wep_logs",
-000177a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000177b0: 2020 2020 2020 2020 2064 6566 6175 6c74           default
-000177c0: 3d46 616c 7365 290a 2020 2020 7061 7273  =False).    pars
-000177d0: 6572 2e61 6464 5f61 7267 756d 656e 7428  er.add_argument(
-000177e0: 222d 7722 2c20 222d 2d73 7263 2d63 6f6e  "-w", "--src-con
-000177f0: 6669 6722 2c0a 2020 2020 2020 2020 2020  fig",.          
-00017800: 2020 2020 2020 2020 2020 2020 2020 6865                he
-00017810: 6c70 3d22 736f 7572 6365 2044 4220 636f  lp="source DB co
-00017820: 6e66 6967 7572 6174 696f 6e20 6669 6c65  nfiguration file
-00017830: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00017840: 2020 2020 2020 2020 2020 2064 6573 743d             dest=
-00017850: 2266 726f 6d5f 636f 6e66 6e22 2c0a 2020  "from_confn",.  
+00017790: 2020 6465 7374 3d22 7765 705f 6c6f 6773    dest="wep_logs
+000177a0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+000177b0: 2020 2020 2020 2020 2020 2064 6566 6175             defau
+000177c0: 6c74 3d46 616c 7365 290a 2020 2020 7061  lt=False).    pa
+000177d0: 7273 6572 2e61 6464 5f61 7267 756d 656e  rser.add_argumen
+000177e0: 7428 222d 7722 2c20 222d 2d73 7263 2d63  t("-w", "--src-c
+000177f0: 6f6e 6669 6722 2c0a 2020 2020 2020 2020  onfig",.        
+00017800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017810: 6865 6c70 3d22 736f 7572 6365 2044 4220  help="source DB 
+00017820: 636f 6e66 6967 7572 6174 696f 6e20 6669  configuration fi
+00017830: 6c65 222c 0a20 2020 2020 2020 2020 2020  le",.           
+00017840: 2020 2020 2020 2020 2020 2020 2064 6573               des
+00017850: 743d 2266 726f 6d5f 636f 6e66 6e22 2c0a  t="from_confn",.
 00017860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017870: 2020 2020 2020 6d65 7461 7661 723d 2266        metavar="f
-00017880: 696c 6522 290a 2020 2020 7061 7273 6572  ile").    parser
-00017890: 2e61 6464 5f61 7267 756d 656e 7428 222d  .add_argument("-
-000178a0: 5922 2c20 222d 2d75 6e69 6e73 7461 6c6c  Y", "--uninstall
-000178b0: 2d6d 6f64 756c 6573 222c 0a20 2020 2020  -modules",.     
+00017870: 2020 2020 2020 2020 6d65 7461 7661 723d          metavar=
+00017880: 2266 696c 6522 290a 2020 2020 7061 7273  "file").    pars
+00017890: 6572 2e61 6464 5f61 7267 756d 656e 7428  er.add_argument(
+000178a0: 222d 5922 2c20 222d 2d75 6e69 6e73 7461  "-Y", "--uninsta
+000178b0: 6c6c 2d6d 6f64 756c 6573 222c 0a20 2020  ll-modules",.   
 000178c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000178d0: 2020 2068 656c 703d 226d 6f64 756c 6573     help="modules
-000178e0: 2074 6f20 756e 696e 7374 616c 6c61 2062   to uninstalla b
-000178f0: 6566 6f72 6520 6d69 6772 6174 696f 6e22  efore migration"
-00017900: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00017910: 2020 2020 2020 2020 2020 6465 7374 3d22            dest="
-00017920: 756e 696e 7374 616c 6c5f 6d6f 6475 6c65  uninstall_module
-00017930: 7322 2c0a 2020 2020 2020 2020 2020 2020  s",.            
-00017940: 2020 2020 2020 2020 2020 2020 6d65 7461              meta
-00017950: 7661 723d 226c 6973 7422 290a 2020 2020  var="list").    
-00017960: 7061 7273 6572 2e61 6464 5f61 7267 756d  parser.add_argum
-00017970: 656e 7428 222d 7922 2c20 222d 2d61 7373  ent("-y", "--ass
-00017980: 756d 652d 7965 7322 2c0a 2020 2020 2020  ume-yes",.      
+000178d0: 2020 2020 2068 656c 703d 226d 6f64 756c       help="modul
+000178e0: 6573 2074 6f20 756e 696e 7374 616c 6c61  es to uninstalla
+000178f0: 2062 6566 6f72 6520 6d69 6772 6174 696f   before migratio
+00017900: 6e22 2c0a 2020 2020 2020 2020 2020 2020  n",.            
+00017910: 2020 2020 2020 2020 2020 2020 6465 7374              dest
+00017920: 3d22 756e 696e 7374 616c 6c5f 6d6f 6475  ="uninstall_modu
+00017930: 6c65 7322 2c0a 2020 2020 2020 2020 2020  les",.          
+00017940: 2020 2020 2020 2020 2020 2020 2020 6d65                me
+00017950: 7461 7661 723d 226c 6973 7422 290a 2020  tavar="list").  
+00017960: 2020 7061 7273 6572 2e61 6464 5f61 7267    parser.add_arg
+00017970: 756d 656e 7428 222d 7922 2c20 222d 2d61  ument("-y", "--a
+00017980: 7373 756d 652d 7965 7322 2c0a 2020 2020  ssume-yes",.    
 00017990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000179a0: 2020 6865 6c70 3d22 6173 7375 6d65 2079    help="assume y
-000179b0: 6573 222c 0a20 2020 2020 2020 2020 2020  es",.           
-000179c0: 2020 2020 2020 2020 2020 2020 2061 6374               act
-000179d0: 696f 6e3d 2773 746f 7265 5f74 7275 6527  ion='store_true'
-000179e0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000179f0: 2020 2020 2020 2020 2020 6465 7374 3d22            dest="
-00017a00: 6173 7375 6d65 5f79 6573 222c 0a20 2020  assume_yes",.   
+000179a0: 2020 2020 6865 6c70 3d22 6173 7375 6d65      help="assume
+000179b0: 2079 6573 222c 0a20 2020 2020 2020 2020   yes",.         
+000179c0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+000179d0: 6374 696f 6e3d 2773 746f 7265 5f74 7275  ction='store_tru
+000179e0: 6527 2c0a 2020 2020 2020 2020 2020 2020  e',.            
+000179f0: 2020 2020 2020 2020 2020 2020 6465 7374              dest
+00017a00: 3d22 6173 7375 6d65 5f79 6573 222c 0a20  ="assume_yes",. 
 00017a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017a20: 2020 2020 2064 6566 6175 6c74 3d46 616c       default=Fal
-00017a30: 7365 290a 2020 2020 7061 7273 6572 2e61  se).    parser.a
-00017a40: 6464 5f61 7267 756d 656e 7428 222d 7a22  dd_argument("-z"
-00017a50: 2c20 222d 2d73 7263 2d64 625f 6e61 6d65  , "--src-db_name
-00017a60: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00017a70: 2020 2020 2020 2020 2020 2068 656c 703d             help=
-00017a80: 2273 6f75 7263 6520 6461 7461 6261 7365  "source database
-00017a90: 206e 616d 6522 2c0a 2020 2020 2020 2020   name",.        
+00017a20: 2020 2020 2020 2064 6566 6175 6c74 3d46         default=F
+00017a30: 616c 7365 290a 2020 2020 7061 7273 6572  alse).    parser
+00017a40: 2e61 6464 5f61 7267 756d 656e 7428 222d  .add_argument("-
+00017a50: 7a22 2c20 222d 2d73 7263 2d64 625f 6e61  z", "--src-db_na
+00017a60: 6d65 222c 0a20 2020 2020 2020 2020 2020  me",.           
+00017a70: 2020 2020 2020 2020 2020 2020 2068 656c               hel
+00017a80: 703d 2273 6f75 7263 6520 6461 7461 6261  p="source databa
+00017a90: 7365 206e 616d 6522 2c0a 2020 2020 2020  se name",.      
 00017aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017ab0: 6465 7374 3d22 6672 6f6d 5f64 626e 616d  dest="from_dbnam
-00017ac0: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
-00017ad0: 2020 2020 2020 2020 2020 2020 6d65 7461              meta
-00017ae0: 7661 723d 226e 616d 6522 290a 2020 2020  var="name").    
-00017af0: 7061 7273 6572 2e61 6464 5f61 7267 756d  parser.add_argum
-00017b00: 656e 7428 222d 3122 2c20 222d 2d64 6f2d  ent("-1", "--do-
-00017b10: 7061 7373 3122 2c0a 2020 2020 2020 2020  pass1",.        
+00017ab0: 2020 6465 7374 3d22 6672 6f6d 5f64 626e    dest="from_dbn
+00017ac0: 616d 6522 2c0a 2020 2020 2020 2020 2020  ame",.          
+00017ad0: 2020 2020 2020 2020 2020 2020 2020 6d65                me
+00017ae0: 7461 7661 723d 226e 616d 6522 290a 2020  tavar="name").  
+00017af0: 2020 7061 7273 6572 2e61 6464 5f61 7267    parser.add_arg
+00017b00: 756d 656e 7428 222d 3122 2c20 222d 2d64  ument("-1", "--d
+00017b10: 6f2d 7061 7373 3122 2c0a 2020 2020 2020  o-pass1",.      
 00017b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017b30: 6865 6c70 3d22 6578 6563 2070 6173 7320  help="exec pass 
-00017b40: 3122 2c0a 2020 2020 2020 2020 2020 2020  1",.            
-00017b50: 2020 2020 2020 2020 2020 2020 6163 7469              acti
-00017b60: 6f6e 3d27 7374 6f72 655f 7472 7565 272c  on='store_true',
-00017b70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017b80: 2020 2020 2020 2020 2064 6573 743d 2270           dest="p
-00017b90: 6861 7365 5f31 2229 0a0a 2020 2020 7372  hase_1")..    sr
-00017ba0: 635f 6374 7820 3d20 7061 7273 6572 2e70  c_ctx = parser.p
-00017bb0: 6172 7365 6f70 7461 7267 7328 7379 732e  arseoptargs(sys.
-00017bc0: 6172 6776 5b31 3a5d 2c20 6170 706c 795f  argv[1:], apply_
-00017bd0: 636f 6e66 3d46 616c 7365 290a 2020 2020  conf=False).    
-00017be0: 7372 635f 6374 782c 2074 6774 5f63 7478  src_ctx, tgt_ctx
-00017bf0: 203d 2070 6172 7365 5f63 7478 2873 7263   = parse_ctx(src
-00017c00: 5f63 7478 290a 2020 2020 6966 2073 7263  _ctx).    if src
-00017c10: 5f63 7478 5b27 7765 705f 6c6f 6773 275d  _ctx['wep_logs']
-00017c20: 3a0a 2020 2020 2020 2020 7765 705f 6c6f  :.        wep_lo
-00017c30: 6773 2873 7263 5f63 7478 290a 2020 2020  gs(src_ctx).    
-00017c40: 6f73 302e 7365 745f 746c 6f67 5f66 696c  os0.set_tlog_fil
-00017c50: 6528 7372 635f 6374 785b 276c 6f67 666e  e(src_ctx['logfn
-00017c60: 275d 2c20 6563 686f 3d54 7275 6529 0a20  '], echo=True). 
-00017c70: 2020 206f 7330 2e77 6c6f 6728 273d 2720     os0.wlog('=' 
-00017c80: 2a20 3830 290a 2020 2020 6f73 302e 776c  * 80).    os0.wl
-00017c90: 6f67 2822 4d69 6772 6174 696f 6e20 6461  og("Migration da
-00017ca0: 7461 6261 7365 2025 7320 6265 6769 6e6e  tabase %s beginn
-00017cb0: 696e 6720 2e2e 2e22 2c20 5f5f 7665 7273  ing ...", __vers
-00017cc0: 696f 6e5f 5f29 0a20 2020 2069 6620 7372  ion__).    if sr
-00017cd0: 635f 6374 785b 2773 656c 5f6d 6f64 656c  c_ctx['sel_model
-00017ce0: 275d 3a0a 2020 2020 2020 2020 6d69 6772  ']:.        migr
-00017cf0: 6174 655f 7365 6c5f 7461 626c 6573 2873  ate_sel_tables(s
-00017d00: 7263 5f63 7478 2c20 7467 745f 6374 7829  rc_ctx, tgt_ctx)
-00017d10: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
-00017d20: 2020 206d 6967 7261 7465 5f64 6174 6162     migrate_datab
-00017d30: 6173 6528 7372 635f 6374 782c 2074 6774  ase(src_ctx, tgt
-00017d40: 5f63 7478 290a                           _ctx).
+00017b30: 2020 6865 6c70 3d22 6578 6563 2070 6173    help="exec pas
+00017b40: 7320 3122 2c0a 2020 2020 2020 2020 2020  s 1",.          
+00017b50: 2020 2020 2020 2020 2020 2020 2020 6163                ac
+00017b60: 7469 6f6e 3d27 7374 6f72 655f 7472 7565  tion='store_true
+00017b70: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+00017b80: 2020 2020 2020 2020 2020 2064 6573 743d             dest=
+00017b90: 2270 6861 7365 5f31 2229 0a0a 2020 2020  "phase_1")..    
+00017ba0: 7372 635f 6374 7820 3d20 7061 7273 6572  src_ctx = parser
+00017bb0: 2e70 6172 7365 6f70 7461 7267 7328 7379  .parseoptargs(sy
+00017bc0: 732e 6172 6776 5b31 3a5d 2c20 6170 706c  s.argv[1:], appl
+00017bd0: 795f 636f 6e66 3d46 616c 7365 290a 2020  y_conf=False).  
+00017be0: 2020 7372 635f 6374 782c 2074 6774 5f63    src_ctx, tgt_c
+00017bf0: 7478 203d 2070 6172 7365 5f63 7478 2873  tx = parse_ctx(s
+00017c00: 7263 5f63 7478 290a 2020 2020 6966 2073  rc_ctx).    if s
+00017c10: 7263 5f63 7478 5b27 7765 705f 6c6f 6773  rc_ctx['wep_logs
+00017c20: 275d 3a0a 2020 2020 2020 2020 7765 705f  ']:.        wep_
+00017c30: 6c6f 6773 2873 7263 5f63 7478 290a 2020  logs(src_ctx).  
+00017c40: 2020 6f73 302e 7365 745f 746c 6f67 5f66    os0.set_tlog_f
+00017c50: 696c 6528 7372 635f 6374 785b 276c 6f67  ile(src_ctx['log
+00017c60: 666e 275d 2c20 6563 686f 3d54 7275 6529  fn'], echo=True)
+00017c70: 0a20 2020 206f 7330 2e77 6c6f 6728 273d  .    os0.wlog('=
+00017c80: 2720 2a20 3830 290a 2020 2020 6f73 302e  ' * 80).    os0.
+00017c90: 776c 6f67 2822 4d69 6772 6174 696f 6e20  wlog("Migration 
+00017ca0: 6461 7461 6261 7365 2025 7320 6265 6769  database %s begi
+00017cb0: 6e6e 696e 6720 2e2e 2e22 2c20 5f5f 7665  nning ...", __ve
+00017cc0: 7273 696f 6e5f 5f29 0a20 2020 2069 6620  rsion__).    if 
+00017cd0: 7372 635f 6374 785b 2773 656c 5f6d 6f64  src_ctx['sel_mod
+00017ce0: 656c 275d 3a0a 2020 2020 2020 2020 6d69  el']:.        mi
+00017cf0: 6772 6174 655f 7365 6c5f 7461 626c 6573  grate_sel_tables
+00017d00: 2873 7263 5f63 7478 2c20 7467 745f 6374  (src_ctx, tgt_ct
+00017d10: 7829 0a20 2020 2065 6c73 653a 0a20 2020  x).    else:.   
+00017d20: 2020 2020 206d 6967 7261 7465 5f64 6174       migrate_dat
+00017d30: 6162 6173 6528 7372 635f 6374 782c 2074  abase(src_ctx, t
+00017d40: 6774 5f63 7478 290a                      gt_ctx).
```

### Comparing `clodoo-2.0.3/clodoo/odoorc` & `clodoo-2.0.4/clodoo/odoorc`

 * *Files 2% similar despite different names*

```diff
@@ -38,47 +38,50 @@
 # PKGNAME      Package (module) name
 # PKGPATH      Home directory of Odoo module (i.e. /opt/odoo/11.0/l10n-italy/l10n_it)
 # REPOS        Repository name
 # ROOT         Odoo home directory of specific vid/version (i.e. /opt/odoo/11.0)
 # RORIGIN      Remote git origin of Odoo repository (actual value|default)
 # RPCPORT      Xmlrpc port in multi-version environment
 # RUPSTREAM    Remote git upstream of Odoo repository (actual value|default)
+# SESS_PATH    Werkzeug session path
 # SVCNAME      Service name to start/stop Odoo service
 # URL          URL to source git project (default value, deprecated: use GIT_URL)
 # URL_BRANCH   URL tp specific version of source git project (default value)
 # USER         Deprecated: use DB_USER
 # VCS          If GIT repository return "git" otherwise return ""
 # VDIR         Virtual directory
 # VENV         Return 1 if path is in virtualenv
+# _VER         odoorc version
+# _FILE        odoorc file
 #
 # -------------------------------
 # Environment variables
 # ODOO_DB_USER"     -> db username (def odoo%(MAJVER)s)
 # ODOO_GIT_ORGID    -> default git organization
 # ODOO_GIT_HOSTNAME -> git hostname (def github.com)
 # ODOO_GIT_PROT     -> default protcocl (git|https) for default git organization
 # ODOO_GIT_SHORT    -> regex of git organizzations with short name (def /(oca)/)
 # ODOO_GIT_MULTI    -> multi version environment
 #
 
-#__version__=2.0.3
+__version__=2.0.4
 
 
 ODOO_FVERS="16\.0|15\.0|14\.0|13\.0|12\.0|11\.0|10\.0|9\.0|8\.0|7\.0|6\.1"
 ODOO_VERS="16|15|14|13|12|11|10|9|8|7|6"
 DEFMLIST="OCB account-analytic account-budgeting account-closing
  account-consolidation account-financial-reporting account-financial-tools
  account-fiscal-rule account-invoice-reporting account-invoicing
  account-payment account-reconcile ansible-odoo apps-store bank-payment
  bank-statement-import brand business-requirement calendar commission
  community-data-files connector contract contribute-md-template
  credit-control crm currency data-protection ddmrp delivery-carrier department
  dms donation e-commerce edi event field-service fleet geospatial helpdesk
  hr hr-attendance hr-expense hr-holidays infrastructure intrastat-extrastat
- iot knowledge l10n-italy maintenance management-system
+ iot knowledge l10n-italy maintenance management-system mgmtsystem
  manufacture manufacture-reporting margin-analysis
  mis-builder mis-builder-contrib multi-company operating-unit partner-contact
  payroll pms pos product-attribute product-configurator product-kitting
  product-pack product-variant program project project-agile project-reporting
  purchase-reporting purchase-workflow queue report-print-send reporting-engine
  rma role-policy sale-financial sale-reporting sale-workflow search-engine
  server-auth server-backend server-brand server-env server-tools server-ux
@@ -197,22 +200,24 @@
             [[ ! $r =~ $rex && ! $r =~ $INVALID_MODNAMES_RE ]] && REPOS=$r && PRJPATH=$1
         fi
     fi
     echo "$PKGNAME|$PKGPATH|$PARENTDIR|$REPOS|$PRJPATH"
 }
 
 build_odoo_param() {
-    # build_odoo_param(ALL|BIN|CONFN|DB_USER|DDIR|DIRLEVEL|FLOG|FPID|FULLVER|FULL_SVCNAME|GIT_BRANCH|GIT_OPTS|GIT_ORG|GIT_ORGNM|GIT_PROT|GIT_URL|HOME|INVALID_MODNAMES|INVALID_MODNAMES_RE|LICENSE|LCONFN|LPPORT|MAJVER|MANIFEST|OCB_SUBDIRS|OCB_SUBDIRS_RE|OPTS_ASM|PARENTDIR|PKGNAME|PKGPATH|REPOS|ROOT|RORIGIN|RPCPORT|RUPSTREAM|SVCNAME|UPSTREAM|URL|URL_BRANCH|USER|VCS|VDIR|VENV
+    # build_odoo_param(ALL|BIN|CONFN|DB_USER|DDIR|DIRLEVEL|FLOG|FPID|FULLVER|FULL_SVCNAME|GIT_BRANCH|GIT_OPTS|GIT_ORG|GIT_ORGNM|GIT_PROT|GIT_URL|HOME|INVALID_MODNAMES|INVALID_MODNAMES_RE|LICENSE|LCONFN|LPPORT|MAJVER|MANIFEST|OCB_SUBDIRS|OCB_SUBDIRS_RE|OPTS_ASM|PARENTDIR|PKGNAME|PKGPATH|REPOS|ROOT|RORIGIN|RPCPORT|RUPSTREAM|SESS_PATH|SVCNAME|UPSTREAM|URL|URL_BRANCH|USER|VCS|VDIR|VENV
     #                  vid [(search|DEBUG|default|tree|SERVER|<rptname>|<modname>)] [oca|zero|zero-http|zero-git|librerp|flectra] [(search|DEBUG|default|tree|SERVER)])
     [[ :$SHELLOPTS: =~ :xtrace: ]] && set +x && local SETX="set -x"
     if [[ $1 =~ (INVALID_MODNAMES|INVALID_MODNAMES_RE|OCB_SUBDIRS|OCB_SUBDIRS_RE) ]]; then
         echo "${!1}"
         $SETX
         return
     fi
+    [[ $1 == "_VER" ]] && echo $__version__ && return
+    [[ $1 == "_FILE" ]] && echo ${BASH_SOURCE-} && return
     READLINK=$(which greadlink 2>/dev/null) || READLINK=$(which readlink 2>/dev/null)
     local ODOO_ROOT
     local VENV=0 main exorg spec
     local ITEM=$1 ROOT PARENTDIR PRJPATH
     local DIRLEVEL FULLVER LICENSE MAJVER odoo_vid noenv_vid MULTIVER REPOS
     local GIT_URL GIT_ORG GIT_ORGID GIT_ORGNM GIT_PROT GIT_OPTS ORGSFX OPTS_ASM
     local RGIT_ORGID RGIT_ORGNM
@@ -269,15 +274,15 @@
                 [[ -z "$PARENTDIR" ]] && PARENTDIR=$($READLINK -e $cdir/..)
                 odoo_vid=$(basename $cdir)
                 [[ $VENV -eq 0 && -f $cdir/venv_odoo/bin/activate ]] && VENV=1 && VDIR=$($READLINK -e $cdir/venv_odoo)
                 [[ $VENV -eq 0 && -f $cdir/../venv_odoo/bin/activate ]] && VENV=1 && VDIR=$($READLINK -e $cdir/../venv_odoo)
                 [[ $VENV -eq 0 && -f $cdir/../VENV-${odoo_vid}/bin/activate ]] && VENV=1 && VDIR=$($READLINK -e $cdir/../VENV-${odoo_vid})
                 [[ $odoo  == "odoo" ]] && cdir=$($READLINK -e $cdir/..) && odoo_vid=$(basename $cdir)
                 FULLVER=$(find_odoo_ver $cdir)
-                [[ -f $cdir/venv_odoo/bin/activate ]] && VENV=1 && VDIR=$cdir/venv_odoo
+                [[ $VENV -eq 0 && -f $cdir/venv_odoo/bin/activate ]] && VENV=1 && VDIR=$cdir/venv_odoo
             elif $(is_repos "$cdir"); then
                 r=$(basename $cdir)
                 [[ ! $r =~ $rex ]] && REPOS=$r && PRJPATH=$cdir
                 [[ -z "$PARENTDIR" ]] && PARENTDIR=$($READLINK -e $cdir/..)
                 [[ -z "$PARENTDIR" ]] && PARENTDIR=$($READLINK -e $cdir/..)
                 if [[ -z "$PKGNAME" ]]; then
                     IFS="|" read PKGNAME PKGPATH PARENTIDR REPOS PRJPATH <<< $(traverse "$cdir" "$PKGNAME" "$PKGPATH" "$PARENTIDR" "$REPOS" "$PRJPATH")
@@ -288,14 +293,15 @@
                 [[ -z "$PARENTDIR" ]] && PARENTDIR=$($READLINK -e $cdir/..)
                 if [[ -z "$PKGNAME" ]]; then
                     IFS="|" read PKGNAME PKGPATH PARENTIDR REPOS PRJPATH <<< $(traverse "$cdir" "$PKGNAME" "$PKGPATH" "$PARENTIDR" "$REPOS" "$PRJPATH")
                 fi
             elif [[ -z "$PKGNAME" ]]; then
                 IFS="|" read PKGNAME PKGPATH PARENTIDR REPOS PRJPATH <<< $(traverse "$cdir" "$PKGNAME" "$PKGPATH" "$PARENTIDR" "$REPOS" "$PRJPATH")
             fi
+            [[ $VENV -eq 0 && -f $cdir/venv_odoo/bin/activate ]] && VENV=1 && VDIR=$($READLINK -e $cdir/venv_odoo)
             if [[ -z "$GIT_ORGNM" && -d $cdir/.git ]] && $(cd $cdir && git status -s &>/dev/null); then
                 x=$(cd $cdir && git rev-parse --show-toplevel 2>/dev/null)
                 if [[ -z $x || $x == $cdir ]]; then
                     GIT_URL=$(cd $cdir && git remote get-url --push origin 2>/dev/null)
                     RUPSTREAM=$(cd $cdir && git remote get-url --push upstream 2>/dev/null)
                     RORIGIN=$(cd $cdir && git remote get-url --push origin 2>/dev/null)
                     if [[ -n "$GIT_URL" ]]; then
@@ -303,14 +309,15 @@
                         GIT_PROT=$(echo $GIT_URL|awk -F: '{print $1}')
                         VCS="git"
                     fi
                     GIT_BRANCH=$(cd $cdir && git branch --list|grep "^\* "|cut -d" " -f2|head -n1|tr -d "\n")
                 fi
             fi
             [[ $cdir == $ODOO_ROOT ]] && break
+            [[ $ITEM == "VDIR" && -n $VDIR ]] && break
             [[ ! $cdir == "/" ]] && cdir=$($READLINK -e $cdir/..) || cdir=
         done
     else
         IFS=/ read odoo_vid x <<<$2
         [[ -n $x ]] && REPOS=$x
         [[ $odoo_vid =~ ^VENV ]] && VENV=1 && VDIR="$ODOO_ROOT/$odoo_vid"
     fi
@@ -396,15 +403,15 @@
           LICENSE=$(echo $LICENSE|grep --color=never -Eo [A-Z]+|head -n1)
         fi
         echo $LICENSE
         $SETX
         return
     fi
     if [[ -z $ROOT ]]; then
-        if [[ $MULTIVER -eq 0 || $exorg -eq 0 || $main -ne 0 || ( -z $GIT_ORGID && $odoo_vid =~ $ref ) || ( -n $ODOO_GIT_ORGID && ( $GIT_ORGID == $ODOO_GIT_ORGID || $GIT_ORGID =~ ^$ODOO_GIT_ORGID$ ) && $odoo_vid =~ $ref ) || $odoo_vid =~ $reo ]]; then
+        if [[ -n $odoo_vid && ( $MULTIVER -eq 0 || $exorg -eq 0 || $main -ne 0 || ( -z $GIT_ORGID && $odoo_vid =~ $ref ) || ( -n $ODOO_GIT_ORGID && ( $GIT_ORGID == $ODOO_GIT_ORGID || $GIT_ORGID =~ ^$ODOO_GIT_ORGID$ ) && $odoo_vid =~ $ref ) || $odoo_vid =~ $reo ) ]]; then
             [[ $VENV -ne 0 ]] && ROOT=$ODOO_ROOT/$odoo_vid/odoo || ROOT=$ODOO_ROOT/$odoo_vid
         elif [[ $GIT_ORGID == "librerp6" ]]; then
             [[ $VENV -ne 0 ]] && ROOT=$ODOO_ROOT/${GIT_ORGID}/odoo || ROOT=$ODOO_ROOT/${GIT_ORGID}
         elif [[ $GIT_ORGID =~ ^$SHORT ]]; then
             [[ $VENV -ne 0 ]] && ROOT=$ODOO_ROOT/${GIT_ORGID}${MAJVER}/odoo || ROOT=$ODOO_ROOT/${GIT_ORGID}${MAJVER}
         else
             [[ $VENV -ne 0 ]] && ROOT=$ODOO_ROOT/odoo$MAJVER-$GIT_ORGID/odoo || ROOT=$ODOO_ROOT/odoo$MAJVER-$GIT_ORGID
@@ -467,15 +474,15 @@
         DB_USER="openerp"
     elif [[ $MULTIVER -ne 0 ]]; then
         DB_USER=${ODOO_DB_USER/\%(MAJVER)s/$MAJVER}
         DB_USER=${DB_USER/\%(ORGSFX)s/$ORGSFX}
     else
         DB_USER="odoo"
     fi
-    [[ -z "$VDIR" ]] && VDIR="$ODOO_ROOT/$FULLVER/venv_odoo"
+    [[ -z "$VDIR" ]] && VDIR="$ROOT/venv_odoo"
     if [[ "$ITEM" =~ ^(DB_USER|FULLVER|GIT_BRANCH|GIT_OPTS|GIT_ORG|GIT_ORGID|GIT_ORGNM|GIT_URL|MAJVER|OPTS_ASM|PARENTDIR|PKGNAME|PKGPATH|REPOS|ROOT|RORIGIN|RUPSTREAM|URL|URL_BRANCH|VCS|VDIR|VENV)$ ]]; then
         echo "${!ITEM}"
         $SETX
         return
     fi
     if [[ $ITEM == "ALL" ]]; then
         echo "|$FULLVER|$REPOS|$PKGPATH|$PKGNAME|"
@@ -535,26 +542,29 @@
         echo $p
         $SETX
         return
     elif [[ $ITEM == "LCONFN" ]]; then
         [[ $MAJVER -ge 10 ]] && echo ".odoorc" || echo ".openerp_serverrc"
         $SETX
         return
-    elif [[ $ITEM == "DDIR" ]]; then
-        [[ $VENV -ne 0 ]] && p="$(dirname $ROOT)/$odoo_vid/.local/share" || p="$(dirname $ROOT)/.local/share"
+    elif [[ $ITEM =~ (DDIR|SESS_PATH) ]]; then
+        # [[ $VENV -ne 0 ]] && p="$(dirname $ROOT)/$odoo_vid/.local/share" || p="$(dirname $ROOT)/.local/share"
+        p="$(dirname $ROOT)"
+        [[ $(basename $p) == "odoo" ]] && p="$(dirname $p)"
+        p="$p/.local/share"
         if [[ $MAJVER -lt 8 ]]; then
-            p="$ROOT/openerp/filestore"
-        elif [[ $odoo_vid =~ ^($ODOO_ROOT/)?VENV ]]; then
-            p="$ODOO_ROOT/VENV-$FULLVER/.local/share/Odoo"
+            [[ $ITEM == "DDIR" ]] && p="$ROOT/openerp/filestore" || p="/tmp/oe-sessions-odoo"
+        # elif [[ $odoo_vid =~ ^($ODOO_ROOT/)?VENV ]]; then
+        #     p="$ODOO_ROOT/VENV-$FULLVER/.local/share/Odoo"
         elif [[ $noenv_vid =~ ^(v|V) ]]; then
-            p="$p/Odoo"
+            [[ $ITEM == "DDIR" ]] && p="$p/Odoo" || p="$p/Odoo/sessions"
         elif [[ $MULTIVER -ne 0 && $VENV -eq 0 ]]; then
-            p="$p/Odoo$MAJVER"
+            [[ $ITEM == "DDIR" ]] && p="$p/Odoo$MAJVER" || p="$p/Odoo$MAJVER/sessions"
         else
-            p="$p/Odoo"
+            [[ $ITEM == "DDIR" ]] && p="$p/Odoo" || p="$p/Odoo/sessions"
         fi
         if [[ $spec =~ search ]]; then
             pd=$p
             p1=/etc/odoo/
             p11=/etc/
             p4=.conf
         else
```

### Comparing `clodoo-2.0.3/setup.py` & `clodoo-2.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         "python-plus",
         "unidecode==1.2.0",
         "z0lib",
     ]
 
 setup(
     name="clodoo",
-    version="2.0.3",
+    version="2.0.4",
     description="Do massive operations on Odoo Cloud",
     long_description="""
 Clodoo is a set of tools to manage to manage multiple Odoo installations with many DBs.
 
 With clodoo you can do massive operations on 1 or more Odoo databases based on
 different Odoo versions. Main operation are:
```

### Comparing `clodoo-2.0.3/PKG-INFO` & `clodoo-2.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,38 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: clodoo
-Version: 2.0.3
+Version: 2.0.4
 Summary: Do massive operations on Odoo Cloud
 Home-page: https://zeroincombenze-tools.readthedocs.io
 Author: Antonio Maria Vigliotti
 Author-email: antoniomaria.vigliotti@gmail.com
 License: Affero GPL
-Project-URL: Source, https://github.com/zeroincombenze/tools
 Project-URL: Documentation, https://zeroincombenze-tools.readthedocs.io
-Description: 
-        Clodoo is a set of tools to manage to manage multiple Odoo installations with many DBs.
-        
-        With clodoo you can do massive operations on 1 or more Odoo databases based on
-        different Odoo versions. Main operation are:
-        
-        * create consistent database to run tests
-        * repeat consistent action on many db with same or different Odoo version
-        * repeat above actions on every new database
-        
-        clodoo is also a PYPI package to simplify RPC connection to Odoo.
-        The PYPI package is a hub to oerplib and odoorpc packages, so generic python client
-        can execute any command to any Odoo version server (from 6.1 to 13.0)
-        
+Project-URL: Source, https://github.com/zeroincombenze/tools
 Keywords: odoo
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
+
+
+Clodoo is a set of tools to manage to manage multiple Odoo installations with many DBs.
+
+With clodoo you can do massive operations on 1 or more Odoo databases based on
+different Odoo versions. Main operation are:
+
+* create consistent database to run tests
+* repeat consistent action on many db with same or different Odoo version
+* repeat above actions on every new database
+
+clodoo is also a PYPI package to simplify RPC connection to Odoo.
+The PYPI package is a hub to oerplib and odoorpc packages, so generic python client
+can execute any command to any Odoo version server (from 6.1 to 13.0)
+
+
```

### Comparing `clodoo-2.0.3/README.rst` & `clodoo-2.0.4/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 ============
-clodoo 2.0.3
+clodoo 2.0.4
 ============
 
 
 
 |Maturity| |Build Status| |Coverage Status| |license gpl|
 
 
@@ -323,14 +323,20 @@
     ./install_tools.sh -Ud
     source /opt/odoo/devel/activate_tools
 
 
 History
 -------
 
+2.0.4 (2023-03-29)
+~~~~~~~~~~~~~~~~~~
+
+* [IMP] odoorc: minor improvements
+* [IMP] transodoo.py: minor improvements
+
 2.0.3 (2022-12-09)
 ~~~~~~~~~~~~~~~~~~
 
 * [FIX] odoorc: GIT_BRANCH sometimes fails
 
 2.0.2 (2022-10-20)
 ~~~~~~~~~~~~~~~~~~
@@ -382,21 +388,24 @@
 SHS-AV s.r.l. <https://www.shs-av.com/>
 
 
 Contributors
 ------------
 
 * Antonio M. Vigliotti <info@shs-av.com>
+Contributors
+------------
+
 
 
 |
 
 This module is part of tools project.
 
-Last Update / Ultimo aggiornamento: 2022-12-11
+Last Update / Ultimo aggiornamento: 2023-04-23
 
 .. |Maturity| image:: https://img.shields.io/badge/maturity-Beta-yellow.png
     :target: https://odoo-community.org/page/development-status
     :alt: 
 .. |Build Status| image:: https://travis-ci.org/zeroincombenze/tools.svg?branch=master
     :target: https://travis-ci.com/zeroincombenze/tools
     :alt: github.com
```

### Comparing `clodoo-2.0.3/clodoo.egg-info/SOURCES.txt` & `clodoo-2.0.4/clodoo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clodoo-2.0.3/clodoo.egg-info/PKG-INFO` & `clodoo-2.0.4/clodoo.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,38 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: clodoo
-Version: 2.0.3
+Version: 2.0.4
 Summary: Do massive operations on Odoo Cloud
 Home-page: https://zeroincombenze-tools.readthedocs.io
 Author: Antonio Maria Vigliotti
 Author-email: antoniomaria.vigliotti@gmail.com
 License: Affero GPL
-Project-URL: Source, https://github.com/zeroincombenze/tools
 Project-URL: Documentation, https://zeroincombenze-tools.readthedocs.io
-Description: 
-        Clodoo is a set of tools to manage to manage multiple Odoo installations with many DBs.
-        
-        With clodoo you can do massive operations on 1 or more Odoo databases based on
-        different Odoo versions. Main operation are:
-        
-        * create consistent database to run tests
-        * repeat consistent action on many db with same or different Odoo version
-        * repeat above actions on every new database
-        
-        clodoo is also a PYPI package to simplify RPC connection to Odoo.
-        The PYPI package is a hub to oerplib and odoorpc packages, so generic python client
-        can execute any command to any Odoo version server (from 6.1 to 13.0)
-        
+Project-URL: Source, https://github.com/zeroincombenze/tools
 Keywords: odoo
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
+
+
+Clodoo is a set of tools to manage to manage multiple Odoo installations with many DBs.
+
+With clodoo you can do massive operations on 1 or more Odoo databases based on
+different Odoo versions. Main operation are:
+
+* create consistent database to run tests
+* repeat consistent action on many db with same or different Odoo version
+* repeat above actions on every new database
+
+clodoo is also a PYPI package to simplify RPC connection to Odoo.
+The PYPI package is a hub to oerplib and odoorpc packages, so generic python client
+can execute any command to any Odoo version server (from 6.1 to 13.0)
+
+
```

