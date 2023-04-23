# Comparing `tmp/thonny-4.1.0b1.tar.gz` & `tmp/thonny-4.1.0b1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thonny-4.1.0b1.tar", last modified: Sun Apr 23 18:29:50 2023, max compression
+gzip compressed data, was "thonny-4.1.0b1.dev0.tar", last modified: Sat Apr 22 07:29:17 2023, max compression
```

## Comparing `thonny-4.1.0b1.tar` & `thonny-4.1.0b1.dev0.tar`

### file list

```diff
@@ -1,703 +1,703 @@
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.859300 thonny-4.1.0b1/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    76100 2023-04-23 18:23:35.000000 thonny-4.1.0b1/CHANGELOG.rst
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     4974 2023-04-18 15:57:23.000000 thonny-4.1.0b1/CREDITS.rst
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1081 2023-04-18 15:57:23.000000 thonny-4.1.0b1/LICENSE.txt
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      317 2023-04-18 15:57:23.000000 thonny-4.1.0b1/MANIFEST.in
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1753 2023-04-23 18:29:50.859128 thonny-4.1.0b1/PKG-INFO
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      742 2023-04-18 15:57:23.000000 thonny-4.1.0b1/README.rst
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.734985 thonny-4.1.0b1/licenses/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    11347 2023-04-18 15:57:23.000000 thonny-4.1.0b1/licenses/ECLIPSE-ICONS-LICENSE.txt
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.702597 thonny-4.1.0b1/packaging/
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.740772 thonny-4.1.0b1/packaging/icons/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1591 2023-04-18 15:57:23.000000 thonny-4.1.0b1/packaging/icons/thonny-128x128.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      214 2023-04-18 15:57:23.000000 thonny-4.1.0b1/packaging/icons/thonny-16x16.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     3077 2023-04-18 15:57:23.000000 thonny-4.1.0b1/packaging/icons/thonny-192x192.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      324 2023-04-18 15:57:23.000000 thonny-4.1.0b1/packaging/icons/thonny-2.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      542 2023-04-18 15:57:23.000000 thonny-4.1.0b1/packaging/icons/thonny-22x22.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     3823 2023-04-18 15:57:23.000000 thonny-4.1.0b1/packaging/icons/thonny-256x256.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      624 2023-04-18 15:57:23.000000 thonny-4.1.0b1/packaging/icons/thonny-32x32.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      914 2023-04-18 15:57:23.000000 thonny-4.1.0b1/packaging/icons/thonny-48x48.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      933 2023-04-18 15:57:23.000000 thonny-4.1.0b1/packaging/icons/thonny-64x64.png
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.743764 thonny-4.1.0b1/packaging/linux/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     3261 2023-04-23 18:22:19.000000 thonny-4.1.0b1/packaging/linux/org.thonny.Thonny.appdata.xml
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      339 2023-04-18 15:57:23.000000 thonny-4.1.0b1/packaging/linux/org.thonny.Thonny.desktop
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      976 2023-04-18 15:57:23.000000 thonny-4.1.0b1/packaging/linux/thonny.1
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      305 2023-04-18 15:57:23.000000 thonny-4.1.0b1/pyproject.toml
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      180 2023-04-18 15:57:23.000000 thonny-4.1.0b1/requirements.txt
--rw-r--r--   0 aivarannamaa   (502) staff       (20)       38 2023-04-23 18:29:50.859352 thonny-4.1.0b1/setup.cfg
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     3517 2023-04-18 15:57:23.000000 thonny-4.1.0b1/setup.py
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.751519 thonny-4.1.0b1/thonny/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)        7 2023-04-23 06:39:17.000000 thonny-4.1.0b1/thonny/VERSION
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    16347 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/__init__.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)       78 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/__main__.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    34909 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/assistance.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     6202 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/ast_utils.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    33389 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/backend.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    53486 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/base_file_browser.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    21845 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/codeview.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    23478 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/common.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     6423 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/config.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     5700 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/config_ui.py
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.754625 thonny-4.1.0b1/thonny/dbus/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      691 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/dbus/org.freedesktop.DBus.ObjectManager.xml
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    11220 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/dbus/org.freedesktop.UDisks2.xml
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      335 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/defaults.ini
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    12741 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/editor_helpers.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    42942 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/editors.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1554 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/export.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     3503 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/first_run.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     9415 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/gridtable.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    10702 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/jedi_utils.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     2411 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/languages.py
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.755495 thonny-4.1.0b1/thonny/locale/
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.704014 thonny-4.1.0b1/thonny/locale/ar_AR/
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.755916 thonny-4.1.0b1/thonny/locale/ar_AR/LC_MESSAGES/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    37201 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/ar_AR/LC_MESSAGES/thonny.mo
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    55586 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/ar_AR/LC_MESSAGES/thonny.po
--rw-r--r--   0 aivarannamaa   (502) staff       (20)       77 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/compile_mo.bat
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.704390 thonny-4.1.0b1/thonny/locale/cs_CZ/
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.756379 thonny-4.1.0b1/thonny/locale/cs_CZ/LC_MESSAGES/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    28884 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/cs_CZ/LC_MESSAGES/thonny.mo
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    52358 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/cs_CZ/LC_MESSAGES/thonny.po
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.704758 thonny-4.1.0b1/thonny/locale/de_DE/
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.756859 thonny-4.1.0b1/thonny/locale/de_DE/LC_MESSAGES/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    35927 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/de_DE/LC_MESSAGES/thonny.mo
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    58829 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/de_DE/LC_MESSAGES/thonny.po
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.705125 thonny-4.1.0b1/thonny/locale/el_GR/
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.757292 thonny-4.1.0b1/thonny/locale/el_GR/LC_MESSAGES/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    45499 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/el_GR/LC_MESSAGES/thonny.mo
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    64554 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/el_GR/LC_MESSAGES/thonny.po
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.705535 thonny-4.1.0b1/thonny/locale/en_US/
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.757730 thonny-4.1.0b1/thonny/locale/en_US/LC_MESSAGES/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      471 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/en_US/LC_MESSAGES/thonny.mo
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    29903 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/en_US/LC_MESSAGES/thonny.po
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.706128 thonny-4.1.0b1/thonny/locale/es_ES/
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.758345 thonny-4.1.0b1/thonny/locale/es_ES/HELP_CONTENT/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     4610 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/es_ES/HELP_CONTENT/debuggers.rst
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     5448 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/es_ES/HELP_CONTENT/debugging.rst
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     2156 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/es_ES/HELP_CONTENT/errors.rst
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.758851 thonny-4.1.0b1/thonny/locale/es_ES/LC_MESSAGES/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    35880 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/es_ES/LC_MESSAGES/thonny.mo
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    56087 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/es_ES/LC_MESSAGES/thonny.po
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.706519 thonny-4.1.0b1/thonny/locale/et_EE/
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.759403 thonny-4.1.0b1/thonny/locale/et_EE/LC_MESSAGES/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    33577 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/et_EE/LC_MESSAGES/thonny.mo
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    53876 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/et_EE/LC_MESSAGES/thonny.po
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.706912 thonny-4.1.0b1/thonny/locale/fa_IR/
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.759868 thonny-4.1.0b1/thonny/locale/fa_IR/LC_MESSAGES/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    38874 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/fa_IR/LC_MESSAGES/thonny.mo
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    57261 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/fa_IR/LC_MESSAGES/thonny.po
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.707342 thonny-4.1.0b1/thonny/locale/fi_FI/
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.760360 thonny-4.1.0b1/thonny/locale/fi_FI/LC_MESSAGES/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    27028 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/fi_FI/LC_MESSAGES/thonny.mo
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    51530 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/fi_FI/LC_MESSAGES/thonny.po
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.708023 thonny-4.1.0b1/thonny/locale/fr_FR/
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.763360 thonny-4.1.0b1/thonny/locale/fr_FR/HELP_CONTENT/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1739 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/fr_FR/HELP_CONTENT/birdseye.rst
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     4885 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/fr_FR/HELP_CONTENT/debuggers.rst
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     5999 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/fr_FR/HELP_CONTENT/debugging.rst
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1272 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/fr_FR/HELP_CONTENT/dock.rst
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     2364 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/fr_FR/HELP_CONTENT/errors.rst
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1558 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/fr_FR/HELP_CONTENT/flask.rst
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      781 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/fr_FR/HELP_CONTENT/index.rst
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1009 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/fr_FR/HELP_CONTENT/modes.rst
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     2955 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/fr_FR/HELP_CONTENT/packages.rst
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     2556 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/fr_FR/HELP_CONTENT/plotter.rst
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1293 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/fr_FR/HELP_CONTENT/program_arguments.rst
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     4026 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/fr_FR/HELP_CONTENT/shell.rst
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      646 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/fr_FR/HELP_CONTENT/turtle.rst
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.763815 thonny-4.1.0b1/thonny/locale/fr_FR/LC_MESSAGES/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    34584 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/fr_FR/LC_MESSAGES/thonny.mo
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    56604 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/fr_FR/LC_MESSAGES/thonny.po
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.708391 thonny-4.1.0b1/thonny/locale/hu_HU/
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.764320 thonny-4.1.0b1/thonny/locale/hu_HU/LC_MESSAGES/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    29029 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/hu_HU/LC_MESSAGES/thonny.mo
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    52830 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/hu_HU/LC_MESSAGES/thonny.po
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.708796 thonny-4.1.0b1/thonny/locale/hy_AM/
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.764791 thonny-4.1.0b1/thonny/locale/hy_AM/LC_MESSAGES/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    41398 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/hy_AM/LC_MESSAGES/thonny.mo
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    59817 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/hy_AM/LC_MESSAGES/thonny.po
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.709187 thonny-4.1.0b1/thonny/locale/it_IT/
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.765222 thonny-4.1.0b1/thonny/locale/it_IT/LC_MESSAGES/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    29164 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/it_IT/LC_MESSAGES/thonny.mo
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    52783 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/it_IT/LC_MESSAGES/thonny.po
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.709630 thonny-4.1.0b1/thonny/locale/ja_JP/
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.765709 thonny-4.1.0b1/thonny/locale/ja_JP/LC_MESSAGES/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    39069 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/ja_JP/LC_MESSAGES/thonny.mo
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    59722 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/ja_JP/LC_MESSAGES/thonny.po
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.710429 thonny-4.1.0b1/thonny/locale/ko_KR/
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.768539 thonny-4.1.0b1/thonny/locale/ko_KR/HELP_CONTENT/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1744 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/ko_KR/HELP_CONTENT/birdseye.rst
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     4901 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/ko_KR/HELP_CONTENT/debuggers.rst
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     6151 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/ko_KR/HELP_CONTENT/debugging.rst
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1292 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/ko_KR/HELP_CONTENT/dock.rst
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     2503 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/ko_KR/HELP_CONTENT/errors.rst
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     2108 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/ko_KR/HELP_CONTENT/flask.rst
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      886 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/ko_KR/HELP_CONTENT/index.rst
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1142 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/ko_KR/HELP_CONTENT/modes.rst
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     2719 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/ko_KR/HELP_CONTENT/packages.rst
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     2482 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/ko_KR/HELP_CONTENT/plotter.rst
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1245 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/ko_KR/HELP_CONTENT/program_arguments.rst
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     4213 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/ko_KR/HELP_CONTENT/shell.rst
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      646 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/ko_KR/HELP_CONTENT/turtle.rst
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.769002 thonny-4.1.0b1/thonny/locale/ko_KR/LC_MESSAGES/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    29558 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/ko_KR/LC_MESSAGES/thonny.mo
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    51805 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/ko_KR/LC_MESSAGES/thonny.po
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.710896 thonny-4.1.0b1/thonny/locale/lt_LT/
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.769491 thonny-4.1.0b1/thonny/locale/lt_LT/LC_MESSAGES/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    26421 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/lt_LT/LC_MESSAGES/thonny.mo
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    40681 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/lt_LT/LC_MESSAGES/thonny.po
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.711774 thonny-4.1.0b1/thonny/locale/nb_NO/
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.770432 thonny-4.1.0b1/thonny/locale/nb_NO/HELP_CONTENT/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     6043 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/nb_NO/HELP_CONTENT/debugging.rst
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     2084 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/nb_NO/HELP_CONTENT/errors.rst
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      754 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/nb_NO/HELP_CONTENT/index.rst
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     3988 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/nb_NO/HELP_CONTENT/shell.rst
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.770935 thonny-4.1.0b1/thonny/locale/nb_NO/LC_MESSAGES/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    23574 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/nb_NO/LC_MESSAGES/thonny.mo
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    49831 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/nb_NO/LC_MESSAGES/thonny.po
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.712234 thonny-4.1.0b1/thonny/locale/nl_NL/
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.771453 thonny-4.1.0b1/thonny/locale/nl_NL/LC_MESSAGES/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    27734 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/nl_NL/LC_MESSAGES/thonny.mo
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    48672 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/nl_NL/LC_MESSAGES/thonny.po
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.712692 thonny-4.1.0b1/thonny/locale/nn_NO/
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.771889 thonny-4.1.0b1/thonny/locale/nn_NO/LC_MESSAGES/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    21613 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/nn_NO/LC_MESSAGES/thonny.mo
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    49202 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/nn_NO/LC_MESSAGES/thonny.po
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.713138 thonny-4.1.0b1/thonny/locale/pl_PL/
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.772374 thonny-4.1.0b1/thonny/locale/pl_PL/LC_MESSAGES/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    28441 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/pl_PL/LC_MESSAGES/thonny.mo
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    52478 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/pl_PL/LC_MESSAGES/thonny.po
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.713854 thonny-4.1.0b1/thonny/locale/pt_BR/
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.775231 thonny-4.1.0b1/thonny/locale/pt_BR/HELP_CONTENT/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1528 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/pt_BR/HELP_CONTENT/assistant.rst
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1558 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/pt_BR/HELP_CONTENT/birdseye.rst
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     4485 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/pt_BR/HELP_CONTENT/debuggers.rst
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     5245 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/pt_BR/HELP_CONTENT/debugging.rst
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1330 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/pt_BR/HELP_CONTENT/dock.rst
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     2096 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/pt_BR/HELP_CONTENT/errors.rst
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     2003 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/pt_BR/HELP_CONTENT/flask.rst
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      740 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/pt_BR/HELP_CONTENT/index.rst
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      920 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/pt_BR/HELP_CONTENT/modes.rst
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     2977 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/pt_BR/HELP_CONTENT/packages.rst
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     2308 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/pt_BR/HELP_CONTENT/plotter.rst
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1230 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/pt_BR/HELP_CONTENT/program_arguments.rst
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     4024 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/pt_BR/HELP_CONTENT/shell.rst
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      649 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/pt_BR/HELP_CONTENT/turtle.rst
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.775719 thonny-4.1.0b1/thonny/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    35547 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/pt_BR/LC_MESSAGES/thonny.mo
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    55866 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/pt_BR/LC_MESSAGES/thonny.po
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.714217 thonny-4.1.0b1/thonny/locale/pt_PT/
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.776287 thonny-4.1.0b1/thonny/locale/pt_PT/LC_MESSAGES/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    26955 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/pt_PT/LC_MESSAGES/thonny.mo
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    40981 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/pt_PT/LC_MESSAGES/thonny.po
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1512 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/register_updates.py
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.714597 thonny-4.1.0b1/thonny/locale/ro_RO/
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.776795 thonny-4.1.0b1/thonny/locale/ro_RO/LC_MESSAGES/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    32776 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/ro_RO/LC_MESSAGES/thonny.mo
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    51239 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/ro_RO/LC_MESSAGES/thonny.po
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.714971 thonny-4.1.0b1/thonny/locale/ru_RU/
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.777288 thonny-4.1.0b1/thonny/locale/ru_RU/LC_MESSAGES/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    46239 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/ru_RU/LC_MESSAGES/thonny.mo
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    66723 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/ru_RU/LC_MESSAGES/thonny.po
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.715468 thonny-4.1.0b1/thonny/locale/sk_SK/
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.777803 thonny-4.1.0b1/thonny/locale/sk_SK/LC_MESSAGES/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    34201 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/sk_SK/LC_MESSAGES/thonny.mo
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    55163 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/sk_SK/LC_MESSAGES/thonny.po
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.715885 thonny-4.1.0b1/thonny/locale/sl_SI/
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.778308 thonny-4.1.0b1/thonny/locale/sl_SI/LC_MESSAGES/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    33078 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/sl_SI/LC_MESSAGES/thonny.mo
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    54237 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/sl_SI/LC_MESSAGES/thonny.po
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.716359 thonny-4.1.0b1/thonny/locale/sq_AL/
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.778823 thonny-4.1.0b1/thonny/locale/sq_AL/LC_MESSAGES/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    34380 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/sq_AL/LC_MESSAGES/thonny.mo
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    54032 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/sq_AL/LC_MESSAGES/thonny.po
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.716771 thonny-4.1.0b1/thonny/locale/sv_SE/
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.779328 thonny-4.1.0b1/thonny/locale/sv_SE/LC_MESSAGES/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     9758 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/sv_SE/LC_MESSAGES/thonny.mo
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    33357 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/sv_SE/LC_MESSAGES/thonny.po
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.717169 thonny-4.1.0b1/thonny/locale/ta_IN/
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.779829 thonny-4.1.0b1/thonny/locale/ta_IN/LC_MESSAGES/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    61109 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/ta_IN/LC_MESSAGES/thonny.mo
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    80796 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/ta_IN/LC_MESSAGES/thonny.po
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.717532 thonny-4.1.0b1/thonny/locale/th_TH/
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.780287 thonny-4.1.0b1/thonny/locale/th_TH/LC_MESSAGES/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    50299 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/th_TH/LC_MESSAGES/thonny.mo
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    69932 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/th_TH/LC_MESSAGES/thonny.po
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    42558 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/thonny.pot
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.717864 thonny-4.1.0b1/thonny/locale/tr_TR/
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.780759 thonny-4.1.0b1/thonny/locale/tr_TR/LC_MESSAGES/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    26908 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/tr_TR/LC_MESSAGES/thonny.mo
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    41183 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/tr_TR/LC_MESSAGES/thonny.po
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.718169 thonny-4.1.0b1/thonny/locale/uk_UA/
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.781212 thonny-4.1.0b1/thonny/locale/uk_UA/LC_MESSAGES/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    34630 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/uk_UA/LC_MESSAGES/thonny.mo
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    48861 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/uk_UA/LC_MESSAGES/thonny.po
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      108 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/update_pot.bat
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.718500 thonny-4.1.0b1/thonny/locale/vi_VN/
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.781916 thonny-4.1.0b1/thonny/locale/vi_VN/LC_MESSAGES/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    35515 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/vi_VN/LC_MESSAGES/thonny.mo
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    57308 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/vi_VN/LC_MESSAGES/thonny.po
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.718838 thonny-4.1.0b1/thonny/locale/zh_CN/
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.782602 thonny-4.1.0b1/thonny/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    31548 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/zh_CN/LC_MESSAGES/thonny.mo
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    54185 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/zh_CN/LC_MESSAGES/thonny.po
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.719290 thonny-4.1.0b1/thonny/locale/zh_TW/
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.783220 thonny-4.1.0b1/thonny/locale/zh_TW/LC_MESSAGES/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    32353 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/zh_TW/LC_MESSAGES/thonny.mo
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    52653 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/locale/zh_TW/LC_MESSAGES/thonny.po
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     4243 2023-04-23 13:50:33.000000 thonny-4.1.0b1/thonny/memory.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    17771 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/misc_utils.py
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.793017 thonny-4.1.0b1/thonny/plugins/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)       17 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/__init__.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     5075 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/about.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     2652 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/assistant_config_page.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     7502 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/ast_view.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    18878 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/autocomplete.py
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.794194 thonny-4.1.0b1/thonny/plugins/backend/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)       17 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/backend/__init__.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1494 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/backend/birdseye_backend.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     2145 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/backend/dock_user_windows_backend.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1604 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/backend/flask_backend.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1116 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/backend/matplotlib_backend.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     2802 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/backend/pgzero_backend.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    11570 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/backend_config_page.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    19598 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/base_syntax_themes.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    24698 2023-04-23 18:14:14.000000 thonny-4.1.0b1/thonny/plugins/base_ui_themes.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     2483 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/birdseye_frontend.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     5647 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/calltip.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     6276 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/cells.py
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.794867 thonny-4.1.0b1/thonny/plugins/circuitpython/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      396 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/circuitpython/__init__.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     4461 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/circuitpython/cirpy_back.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     4238 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/circuitpython/cirpy_front.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    14106 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/clean_ui_themes.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    12566 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/coloring.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     5561 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/commenting_indenting.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     2683 2023-04-22 09:05:00.000000 thonny-4.1.0b1/thonny/plugins/common_editing_commands.py
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.795714 thonny-4.1.0b1/thonny/plugins/cpython_backend/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      226 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/cpython_backend/__init__.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    51717 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/cpython_backend/cp_back.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1883 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/cpython_backend/cp_launcher.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    57896 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/cpython_backend/cp_tracers.py
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.796353 thonny-4.1.0b1/thonny/plugins/cpython_frontend/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      920 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/cpython_frontend/__init__.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    18540 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/cpython_frontend/cp_front.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1926 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/cpython_frontend/cp_pip_gui.py
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.797028 thonny-4.1.0b1/thonny/plugins/cpython_ssh/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      808 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/cpython_ssh/__init__.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     7613 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/cpython_ssh/cps_back.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     5685 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/cpython_ssh/cps_front.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      361 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/cpython_ssh/cps_pip_gui.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    49636 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/debugger.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      812 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/dock_user_windows_frontend.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     3703 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/editor_config_page.py
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.797447 thonny-4.1.0b1/thonny/plugins/esp/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     2446 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/esp/__init__.py
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.797785 thonny-4.1.0b1/thonny/plugins/esp/esp32_api_stubs/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    18158 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/esp/esp32_api_stubs/esp32.pyi
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      555 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/esp/esp32_api_stubs/mp-1.18-esp32.txt
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      988 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/esp/esp_back.py
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.798137 thonny-4.1.0b1/thonny/plugins/ev3/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     4254 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/ev3/__init__.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      996 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/ev3/ev3_back.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     6623 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/event_logging.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1535 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/event_view.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    20730 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/files.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    18116 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/find_replace.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     5383 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/general_config_page.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     4520 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/goto_definition.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     2987 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/heap.py
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.801276 thonny-4.1.0b1/thonny/plugins/help/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     2508 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/help/__init__.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1366 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/help/assistant.rst
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1410 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/help/birdseye.rst
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     4009 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/help/debuggers.rst
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     5114 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/help/debugging.rst
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1131 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/help/dock.rst
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1969 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/help/errors.rst
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1764 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/help/flask.rst
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      677 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/help/index.rst
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      816 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/help/modes.rst
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     2633 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/help/packages.rst
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     2183 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/help/plotter.rst
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1038 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/help/program_arguments.rst
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     3650 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/help/shell.rst
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      569 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/help/turtle.rst
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     4104 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/highlight_names.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     4178 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/locals_marker.py
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.801631 thonny-4.1.0b1/thonny/plugins/microbit/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     7039 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/microbit/__init__.py
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.806144 thonny-4.1.0b1/thonny/plugins/microbit/api_stubs/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)       20 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/microbit/api_stubs/antigravity.pyi
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      184 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/microbit/api_stubs/array.pyi
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1299 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/microbit/api_stubs/audio.pyi
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      402 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/microbit/api_stubs/collections.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      186 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/microbit/api_stubs/gc.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)       68 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/microbit/api_stubs/love.pyi
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      204 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/microbit/api_stubs/machine.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      617 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/microbit/api_stubs/math.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    33816 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/microbit/api_stubs/microbit.pyi
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      218 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/microbit/api_stubs/micropython.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     8815 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/microbit/api_stubs/music.pyi
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     3287 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/microbit/api_stubs/neopixel.pyi
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      916 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/microbit/api_stubs/os.pyi
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     6453 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/microbit/api_stubs/radio.pyi
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1486 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/microbit/api_stubs/random.pyi
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1676 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/microbit/api_stubs/speech.pyi
--rw-r--r--   0 aivarannamaa   (502) staff       (20)       66 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/microbit/api_stubs/struct.pyi
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     4365 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/microbit/api_stubs/sys.pyi
--rw-r--r--   0 aivarannamaa   (502) staff       (20)       85 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/microbit/api_stubs/this.pyi
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      187 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/microbit/api_stubs/time.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     7935 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/microbit/api_stubs/uarray.pyi
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      402 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/microbit/api_stubs/ucollections.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     2138 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/microbit/api_stubs/ustruct.pyi
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     9148 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/microbit/api_stubs/utime.pyi
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      880 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/microbit/microbit_back.py
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.808930 thonny-4.1.0b1/thonny/plugins/micropython/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1914 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/micropython/__init__.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    64546 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/micropython/bare_metal_backend.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    21237 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/micropython/base_flashing_dialog.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     6269 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/micropython/connection.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    20159 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/micropython/esptool_dialog.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      345 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/micropython/miniterm_wrapper.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    52302 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/micropython/mp_back.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)       88 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/micropython/mp_common.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    36776 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/micropython/mp_front.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    13352 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/micropython/os_mp_backend.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     4819 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/micropython/pip_gui.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     6515 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/micropython/serial_connection.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1621 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/micropython/ssh_connection.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1862 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/micropython/subprocess_connection.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     9964 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/micropython/uf2dialog.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     4561 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/micropython/webrepl_connection.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     6307 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/misc_analyzers.py
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.809082 thonny-4.1.0b1/thonny/plugins/mypy/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     4134 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/mypy/__init__.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     2102 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/notes.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    26582 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/object_inspector.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     5194 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/outline.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     8057 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/paren_matcher.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      734 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pgzero_frontend.py
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.809268 thonny-4.1.0b1/thonny/plugins/pi/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    12209 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/__init__.py
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.823290 thonny-4.1.0b1/thonny/plugins/pi/res/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      206 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/Ukraine.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      328 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/Ukraine48.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1525 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_debug-run-cursor.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1525 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_debug-run-cursor48.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      668 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_debug-run.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1012 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_debug-run48.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      590 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_debug-step-into.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      894 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_debug-step-into48.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      586 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_debug-step-out.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      882 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_debug-step-out48.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      577 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_debug-step-over.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      861 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_debug-step-over48.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      403 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_document-new.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      530 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_document-new48.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      731 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_document-open.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1221 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_document-open48.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      691 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_document-save.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1082 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_document-save48.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1146 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_media-playback-start.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1806 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_media-playback-start48.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      993 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_process-stop.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1476 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_process-stop48.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1082 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_quit.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1741 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_quit48.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1133 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_resume.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1763 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_resume48.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      177 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_scrollbar-button-down-insens.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      208 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_scrollbar-button-down.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      160 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_scrollbar-button-left-insens.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      207 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_scrollbar-button-left.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      173 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_scrollbar-button-right-insens.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      202 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_scrollbar-button-right.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      175 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_scrollbar-button-up-insens.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      187 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_scrollbar-button-up.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      633 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_window-close-act.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      423 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_window-close.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1488 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_zoom.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     2349 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_zoom48.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1589 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/debug-run-cursor.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1589 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/debug-run-cursor48.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      746 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/debug-run.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1150 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/debug-run48.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      659 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/debug-step-into.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      980 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/debug-step-into48.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      644 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/debug-step-out.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      976 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/debug-step-out48.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      637 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/debug-step-over.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      962 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/debug-step-over48.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      445 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/document-new.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      611 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/document-new48.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      800 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/document-open.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1354 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/document-open48.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      770 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/document-save.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1223 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/document-save48.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1337 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/media-playback-start.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     2072 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/media-playback-start48.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1139 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/process-stop.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1663 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/process-stop48.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1207 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/quit.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1988 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/quit48.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1258 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/resume.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1977 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/resume48.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     2866 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/scrollbar-button-down-insens.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     2857 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/scrollbar-button-down.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     2857 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/scrollbar-button-left-insens.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     2834 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/scrollbar-button-left.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     2865 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/scrollbar-button-right-insens.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     2858 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/scrollbar-button-right.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     2859 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/scrollbar-button-up-insens.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     2862 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/scrollbar-button-up.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    16273 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/window-close-act.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      505 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/window-close.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1513 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/zoom.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     2561 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pi/res/zoom48.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    55548 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pip_gui.py
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.823685 thonny-4.1.0b1/thonny/plugins/prime_inventor/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1774 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/prime_inventor/__init__.py
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.823859 thonny-4.1.0b1/thonny/plugins/prime_inventor/api_stubs/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    19398 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/prime_inventor/api_stubs/hub.pyi
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      663 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/prime_inventor/prime_inventor_back.py
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.824269 thonny-4.1.0b1/thonny/plugins/printing/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     2778 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/printing/__init__.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1382 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/printing/template.html
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.824633 thonny-4.1.0b1/thonny/plugins/pylint/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     6186 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pylint/__init__.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)   155507 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pylint/messages.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1131 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/pythontutor.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1514 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/remove_old_data_dir.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    13491 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/replayer.py
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.825147 thonny-4.1.0b1/thonny/plugins/rp2040/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1692 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/rp2040/__init__.py
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.825534 thonny-4.1.0b1/thonny/plugins/rp2040/api_stubs/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      344 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/rp2040/api_stubs/mp-1.18-pico.txt
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     9549 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/rp2040/api_stubs/rp2.pyi
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      891 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/rp2040/rp2040_back.py
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.825763 thonny-4.1.0b1/thonny/plugins/rpi_pico/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     2003 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/rpi_pico/__init__.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     3051 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/run_debug_config_page.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     2564 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/shell_config_page.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     3497 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/shell_macro.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     8449 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/statement_boxes.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    25880 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/stdlib_error_helpers.py
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.826143 thonny-4.1.0b1/thonny/plugins/system_shell/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     2183 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/system_shell/__init__.py
--rwxr-xr-x   0 aivarannamaa   (502) staff       (20)     5377 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/system_shell/explain_environment.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1375 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/terminal_config_page.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     9267 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/theme_and_font_config_page.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      763 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/thonny_folders.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     4599 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/todo_view.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     6327 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/tomorrow_syntax_theme.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     5411 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/plugins/variables.py
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.854407 thonny-4.1.0b1/thonny/res/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      832 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/16x16-blank.gif
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      807 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/1x1-white.gif
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      270 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/PrintLnkTarget.vbs
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      171 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/Ukraine.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     5430 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/Ukraine_2x.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      682 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_create_disabled_variants.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      832 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_16x16-blank.gif
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      807 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_1x1-white.gif
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      837 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_arrow-down.gif
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      734 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_birdseye.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      199 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_boxdot.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      169 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_boxdot_light.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      192 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_boxminus.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      160 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_boxminus_light.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      212 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_boxplus.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      176 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_boxplus_light.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      224 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_boxx.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      179 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_boxx_light.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      908 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_broken.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      917 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_closed-folder.gif
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      577 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_debug-current-script.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1320 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_debug-current-script_2x.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      877 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_delete.gif
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      907 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_folder.gif
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      881 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_generic-file.gif
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      895 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_hard-drive.gif
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      553 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_harddisk.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1177 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_harddisk_2x.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      745 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_help.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1897 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_help_2x.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      654 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_information.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1555 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_information_2x.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      428 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_nav-backward.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      756 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_nav-backward_2x.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      420 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_nav-forward.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      749 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_nav-forward_2x.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      320 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_new-file.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      376 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_new-file_Linux.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      868 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_new-file_Linux_2x.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      502 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_open-file.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      495 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_open-file_Linux.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1217 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_open-file_Linux_2x.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      935 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_open_folder.gif
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      613 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_outline-class.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1324 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_outline-class_2x.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      928 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_outline-method.gif
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      929 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_python-file.gif
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      945 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_python-icon.gif
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      461 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_quit.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      780 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_quit_2x.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      469 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_resume.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      885 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_resume_2x.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      620 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_run-current-script.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1281 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_run-current-script_2x.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      339 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_run-to-cursor.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      612 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_run-to-cursor_2x.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      460 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_save-file.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      944 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_save-file_2x_alt.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      604 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_save-file_Linux.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1611 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_save-file_Linux_2x.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      518 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_save-file_alt.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      615 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_star.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1489 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_star_2x.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      421 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_step-into.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      760 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_step-into_2x.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      404 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_step-out.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      726 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_step-out_2x.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      530 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_step-over.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1034 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_step-over_2x.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      630 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_stop.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1888 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_stop_2x.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      837 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_tab-close-active-clam-dark.gif
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      837 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_tab-close-active-clam.gif
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      837 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_tab-close-active.gif
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      842 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_tab-close-clam.gif
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      842 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_tab-close.gif
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      511 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_terminal.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1255 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_terminal_2x.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      934 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_text-file.gif
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     5186 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_thonny.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      469 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/_disabled_zoom.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      837 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/arrow-down.gif
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1225 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/birdseye.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      282 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/boxdot.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      258 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/boxdot_light.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      272 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/boxminus.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1170 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/boxminus_light.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      288 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/boxplus.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1179 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/boxplus_light.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      312 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/boxx.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      264 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/boxx_light.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1535 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/broken.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1111 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/closed-folder.gif
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      563 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/debug-current-script.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1453 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/debug-current-script_2x.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      900 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/delete.gif
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      386 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/folder.gif
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      238 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/generic-file.gif
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1019 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/hard-drive.gif
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      847 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/harddisk.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1519 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/harddisk_2x.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      932 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/help.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     2231 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/help_2x.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      863 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/information.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1910 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/information_2x.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      347 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/nav-backward.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      652 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/nav-backward_2x.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      344 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/nav-forward.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      644 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/nav-forward_2x.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      299 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/new-file.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      477 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/new-file_Linux.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1008 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/new-file_Linux_2x.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      567 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/open-file.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      672 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/open-file_Linux.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1550 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/open-file_Linux_2x.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1108 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/open_folder.gif
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      628 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/outline-class.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1129 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/outline-class_2x.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      578 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/outline-method.gif
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      626 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/python-file.gif
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1049 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/python-icon.gif
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     2430 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/python-icon_2x.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      561 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/quit.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      984 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/quit_2x.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      539 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/resume.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1046 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/resume_2x.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      620 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/run-current-script.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1226 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/run-current-script_2x.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      252 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/run-to-cursor.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      492 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/run-to-cursor_2x.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      543 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/save-file.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1151 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/save-file_2x_alt.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      911 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/save-file_Linux.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1971 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/save-file_Linux_2x.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      617 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/save-file_alt.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      950 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/star.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1800 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/star_2x.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      356 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/step-into.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      761 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/step-into_2x.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      379 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/step-out.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      798 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/step-out_2x.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      457 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/step-over.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1014 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/step-over_2x.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      718 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/stop.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     3595 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/stop_2x.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)       58 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/tab-close-active-clam-dark.gif
--rw-r--r--   0 aivarannamaa   (502) staff       (20)       58 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/tab-close-active-clam.gif
--rw-r--r--   0 aivarannamaa   (502) staff       (20)       58 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/tab-close-active.gif
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      842 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/tab-close-clam.gif
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      842 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/tab-close.gif
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      668 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/terminal.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1488 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/terminal_2x.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      627 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/text-file.gif
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    16652 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/thonny.ico
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     5134 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/thonny.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      894 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/thonny_small.ico
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      468 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/res/zoom.png
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    33753 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/roughparse.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    17497 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/rst_utils.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    57393 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/running.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    80009 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/shell.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     8048 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/terminal.py
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.854691 thonny-4.1.0b1/thonny/test/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)       17 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/test/__init__.py
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.855303 thonny-4.1.0b1/thonny/test/plugins/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)       17 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/test/plugins/__init__.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      598 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/test/plugins/test_locals_marker.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     3360 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/test/plugins/test_name_highlighter.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      336 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/test/plugins/test_pip_gui.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1173 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/test/test_common.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    45325 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/tktextext.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     2262 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/token_utils.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     4914 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/udisks.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    83339 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/ui_utils.py
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.727253 thonny-4.1.0b1/thonny/vendored_libs/
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.856739 thonny-4.1.0b1/thonny/vendored_libs/filelock/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1315 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/vendored_libs/filelock/__init__.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     8896 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/vendored_libs/filelock/_api.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      399 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/vendored_libs/filelock/_error.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1650 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/vendored_libs/filelock/_soft.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1578 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/vendored_libs/filelock/_unix.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      594 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/vendored_libs/filelock/_util.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1890 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/vendored_libs/filelock/_windows.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)        0 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/vendored_libs/filelock/py.typed
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      160 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/vendored_libs/filelock/version.py
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.858828 thonny-4.1.0b1/thonny/vendored_libs/pipkin/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1738 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/vendored_libs/pipkin/__init__.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     2114 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/vendored_libs/pipkin/__main__.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    16912 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/vendored_libs/pipkin/adapters.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    33595 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/vendored_libs/pipkin/bare_metal.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      355 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/vendored_libs/pipkin/common.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     6235 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/vendored_libs/pipkin/connection.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    10546 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/vendored_libs/pipkin/parser.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    18946 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/vendored_libs/pipkin/proxy.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     6599 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/vendored_libs/pipkin/serial_connection.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    27862 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/vendored_libs/pipkin/session.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     6702 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/vendored_libs/pipkin/util.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     4580 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/vendored_libs/pipkin/webrepl_connection.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    98557 2023-04-22 09:49:24.000000 thonny-4.1.0b1/thonny/workbench.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    16632 2023-04-18 15:57:23.000000 thonny-4.1.0b1/thonny/workdlg.py
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-04-23 18:29:50.754213 thonny-4.1.0b1/thonny.egg-info/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1753 2023-04-23 18:29:50.000000 thonny-4.1.0b1/thonny.egg-info/PKG-INFO
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    21822 2023-04-23 18:29:50.000000 thonny-4.1.0b1/thonny.egg-info/SOURCES.txt
--rw-r--r--   0 aivarannamaa   (502) staff       (20)        1 2023-04-23 18:29:50.000000 thonny-4.1.0b1/thonny.egg-info/dependency_links.txt
--rw-r--r--   0 aivarannamaa   (502) staff       (20)       37 2023-04-23 18:29:50.000000 thonny-4.1.0b1/thonny.egg-info/entry_points.txt
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      120 2023-04-23 18:29:50.000000 thonny-4.1.0b1/thonny.egg-info/requires.txt
--rw-r--r--   0 aivarannamaa   (502) staff       (20)        7 2023-04-23 18:29:50.000000 thonny-4.1.0b1/thonny.egg-info/top_level.txt
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.883777 thonny-4.1.0b1.dev0/
+-rw-r--r--   0 aivar      (501) staff       (20)    74167 2023-01-14 19:52:25.000000 thonny-4.1.0b1.dev0/CHANGELOG.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     4974 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/CREDITS.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     1081 2023-01-14 19:52:25.000000 thonny-4.1.0b1.dev0/LICENSE.txt
+-rw-r--r--   0 aivar      (501) staff       (20)      317 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/MANIFEST.in
+-rw-r--r--   0 aivar      (501) staff       (20)     1759 2023-04-22 07:29:17.883102 thonny-4.1.0b1.dev0/PKG-INFO
+-rw-r--r--   0 aivar      (501) staff       (20)      742 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/README.rst
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.031992 thonny-4.1.0b1.dev0/licenses/
+-rw-r--r--   0 aivar      (501) staff       (20)    11347 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/licenses/ECLIPSE-ICONS-LICENSE.txt
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.942441 thonny-4.1.0b1.dev0/packaging/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.046904 thonny-4.1.0b1.dev0/packaging/icons/
+-rw-r--r--   0 aivar      (501) staff       (20)     1591 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/packaging/icons/thonny-128x128.png
+-rw-r--r--   0 aivar      (501) staff       (20)      214 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/packaging/icons/thonny-16x16.png
+-rw-r--r--   0 aivar      (501) staff       (20)     3077 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/packaging/icons/thonny-192x192.png
+-rw-r--r--   0 aivar      (501) staff       (20)      324 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/packaging/icons/thonny-2.png
+-rw-r--r--   0 aivar      (501) staff       (20)      542 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/packaging/icons/thonny-22x22.png
+-rw-r--r--   0 aivar      (501) staff       (20)     3823 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/packaging/icons/thonny-256x256.png
+-rw-r--r--   0 aivar      (501) staff       (20)      624 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/packaging/icons/thonny-32x32.png
+-rw-r--r--   0 aivar      (501) staff       (20)      914 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/packaging/icons/thonny-48x48.png
+-rw-r--r--   0 aivar      (501) staff       (20)      933 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/packaging/icons/thonny-64x64.png
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.051037 thonny-4.1.0b1.dev0/packaging/linux/
+-rw-r--r--   0 aivar      (501) staff       (20)     3099 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/packaging/linux/org.thonny.Thonny.appdata.xml
+-rw-r--r--   0 aivar      (501) staff       (20)      339 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/packaging/linux/org.thonny.Thonny.desktop
+-rw-r--r--   0 aivar      (501) staff       (20)      976 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/packaging/linux/thonny.1
+-rw-r--r--   0 aivar      (501) staff       (20)      305 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/pyproject.toml
+-rw-r--r--   0 aivar      (501) staff       (20)      180 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/requirements.txt
+-rw-r--r--   0 aivar      (501) staff       (20)       38 2023-04-22 07:29:17.883965 thonny-4.1.0b1.dev0/setup.cfg
+-rw-r--r--   0 aivar      (501) staff       (20)     3517 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/setup.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.140302 thonny-4.1.0b1.dev0/thonny/
+-rw-r--r--   0 aivar      (501) staff       (20)       11 2023-04-22 07:29:07.000000 thonny-4.1.0b1.dev0/thonny/VERSION
+-rw-r--r--   0 aivar      (501) staff       (20)    16347 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/__init__.py
+-rw-r--r--   0 aivar      (501) staff       (20)       78 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/__main__.py
+-rw-r--r--   0 aivar      (501) staff       (20)    34909 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/assistance.py
+-rw-r--r--   0 aivar      (501) staff       (20)     6202 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/ast_utils.py
+-rw-r--r--   0 aivar      (501) staff       (20)    33389 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/backend.py
+-rw-r--r--   0 aivar      (501) staff       (20)    53486 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/base_file_browser.py
+-rw-r--r--   0 aivar      (501) staff       (20)    21845 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/codeview.py
+-rw-r--r--   0 aivar      (501) staff       (20)    23478 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/common.py
+-rw-r--r--   0 aivar      (501) staff       (20)     6423 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/config.py
+-rw-r--r--   0 aivar      (501) staff       (20)     5700 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/config_ui.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.155650 thonny-4.1.0b1.dev0/thonny/dbus/
+-rw-r--r--   0 aivar      (501) staff       (20)      691 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/dbus/org.freedesktop.DBus.ObjectManager.xml
+-rw-r--r--   0 aivar      (501) staff       (20)    11220 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/dbus/org.freedesktop.UDisks2.xml
+-rw-r--r--   0 aivar      (501) staff       (20)      335 2020-11-02 17:21:06.000000 thonny-4.1.0b1.dev0/thonny/defaults.ini
+-rw-r--r--   0 aivar      (501) staff       (20)    12741 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/editor_helpers.py
+-rw-r--r--   0 aivar      (501) staff       (20)    42942 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/editors.py
+-rw-r--r--   0 aivar      (501) staff       (20)     1554 2020-11-15 16:51:08.000000 thonny-4.1.0b1.dev0/thonny/export.py
+-rw-r--r--   0 aivar      (501) staff       (20)     3503 2020-09-02 21:27:22.000000 thonny-4.1.0b1.dev0/thonny/first_run.py
+-rw-r--r--   0 aivar      (501) staff       (20)     9415 2020-09-03 11:18:16.000000 thonny-4.1.0b1.dev0/thonny/gridtable.py
+-rw-r--r--   0 aivar      (501) staff       (20)    10702 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/jedi_utils.py
+-rw-r--r--   0 aivar      (501) staff       (20)     2411 2023-01-14 19:52:25.000000 thonny-4.1.0b1.dev0/thonny/languages.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.163535 thonny-4.1.0b1.dev0/thonny/locale/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.946627 thonny-4.1.0b1.dev0/thonny/locale/ar_AR/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.165002 thonny-4.1.0b1.dev0/thonny/locale/ar_AR/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    37201 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/ar_AR/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    55586 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/ar_AR/LC_MESSAGES/thonny.po
+-rw-r--r--   0 aivar      (501) staff       (20)       77 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/locale/compile_mo.bat
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.947342 thonny-4.1.0b1.dev0/thonny/locale/cs_CZ/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.177380 thonny-4.1.0b1.dev0/thonny/locale/cs_CZ/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    28884 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/cs_CZ/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    52358 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/cs_CZ/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.948052 thonny-4.1.0b1.dev0/thonny/locale/de_DE/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.180001 thonny-4.1.0b1.dev0/thonny/locale/de_DE/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    35927 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/de_DE/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    58829 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/de_DE/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.948567 thonny-4.1.0b1.dev0/thonny/locale/el_GR/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.193640 thonny-4.1.0b1.dev0/thonny/locale/el_GR/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    45499 2021-02-22 20:19:16.000000 thonny-4.1.0b1.dev0/thonny/locale/el_GR/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    64554 2021-02-22 20:19:16.000000 thonny-4.1.0b1.dev0/thonny/locale/el_GR/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.949041 thonny-4.1.0b1.dev0/thonny/locale/en_US/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.197870 thonny-4.1.0b1.dev0/thonny/locale/en_US/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)      471 2020-02-18 07:08:34.000000 thonny-4.1.0b1.dev0/thonny/locale/en_US/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    29903 2020-02-18 07:08:34.000000 thonny-4.1.0b1.dev0/thonny/locale/en_US/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.950076 thonny-4.1.0b1.dev0/thonny/locale/es_ES/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.210270 thonny-4.1.0b1.dev0/thonny/locale/es_ES/HELP_CONTENT/
+-rw-r--r--   0 aivar      (501) staff       (20)     4610 2021-04-30 13:51:14.000000 thonny-4.1.0b1.dev0/thonny/locale/es_ES/HELP_CONTENT/debuggers.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     5448 2021-04-30 13:51:14.000000 thonny-4.1.0b1.dev0/thonny/locale/es_ES/HELP_CONTENT/debugging.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     2156 2021-04-30 13:51:14.000000 thonny-4.1.0b1.dev0/thonny/locale/es_ES/HELP_CONTENT/errors.rst
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.213051 thonny-4.1.0b1.dev0/thonny/locale/es_ES/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    35880 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/es_ES/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    56087 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/es_ES/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.951250 thonny-4.1.0b1.dev0/thonny/locale/et_EE/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.218666 thonny-4.1.0b1.dev0/thonny/locale/et_EE/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    33577 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/et_EE/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    53876 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/et_EE/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.953802 thonny-4.1.0b1.dev0/thonny/locale/fa_IR/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.222327 thonny-4.1.0b1.dev0/thonny/locale/fa_IR/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    38874 2021-01-06 13:30:09.000000 thonny-4.1.0b1.dev0/thonny/locale/fa_IR/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    57261 2021-01-06 13:30:09.000000 thonny-4.1.0b1.dev0/thonny/locale/fa_IR/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.954704 thonny-4.1.0b1.dev0/thonny/locale/fi_FI/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.224882 thonny-4.1.0b1.dev0/thonny/locale/fi_FI/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    27028 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/fi_FI/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    51530 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/fi_FI/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.956207 thonny-4.1.0b1.dev0/thonny/locale/fr_FR/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.240167 thonny-4.1.0b1.dev0/thonny/locale/fr_FR/HELP_CONTENT/
+-rw-r--r--   0 aivar      (501) staff       (20)     1739 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/locale/fr_FR/HELP_CONTENT/birdseye.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     4885 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/locale/fr_FR/HELP_CONTENT/debuggers.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     5999 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/locale/fr_FR/HELP_CONTENT/debugging.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     1272 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/locale/fr_FR/HELP_CONTENT/dock.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     2364 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/locale/fr_FR/HELP_CONTENT/errors.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     1558 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/locale/fr_FR/HELP_CONTENT/flask.rst
+-rw-r--r--   0 aivar      (501) staff       (20)      781 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/locale/fr_FR/HELP_CONTENT/index.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     1009 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/locale/fr_FR/HELP_CONTENT/modes.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     2955 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/locale/fr_FR/HELP_CONTENT/packages.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     2556 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/locale/fr_FR/HELP_CONTENT/plotter.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     1293 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/locale/fr_FR/HELP_CONTENT/program_arguments.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     4026 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/locale/fr_FR/HELP_CONTENT/shell.rst
+-rw-r--r--   0 aivar      (501) staff       (20)      646 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/locale/fr_FR/HELP_CONTENT/turtle.rst
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.243114 thonny-4.1.0b1.dev0/thonny/locale/fr_FR/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    34584 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/fr_FR/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    56604 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/fr_FR/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.957019 thonny-4.1.0b1.dev0/thonny/locale/hu_HU/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.245907 thonny-4.1.0b1.dev0/thonny/locale/hu_HU/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    29029 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/hu_HU/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    52830 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/hu_HU/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.957700 thonny-4.1.0b1.dev0/thonny/locale/hy_AM/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.247658 thonny-4.1.0b1.dev0/thonny/locale/hy_AM/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    41398 2021-01-06 13:30:09.000000 thonny-4.1.0b1.dev0/thonny/locale/hy_AM/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    59817 2021-01-06 13:30:09.000000 thonny-4.1.0b1.dev0/thonny/locale/hy_AM/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.958458 thonny-4.1.0b1.dev0/thonny/locale/it_IT/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.251834 thonny-4.1.0b1.dev0/thonny/locale/it_IT/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    29164 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/it_IT/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    52783 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/it_IT/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.959156 thonny-4.1.0b1.dev0/thonny/locale/ja_JP/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.255297 thonny-4.1.0b1.dev0/thonny/locale/ja_JP/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    39069 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/ja_JP/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    59722 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/ja_JP/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.960212 thonny-4.1.0b1.dev0/thonny/locale/ko_KR/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.271644 thonny-4.1.0b1.dev0/thonny/locale/ko_KR/HELP_CONTENT/
+-rw-r--r--   0 aivar      (501) staff       (20)     1744 2021-04-30 13:51:14.000000 thonny-4.1.0b1.dev0/thonny/locale/ko_KR/HELP_CONTENT/birdseye.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     4901 2021-04-30 13:51:14.000000 thonny-4.1.0b1.dev0/thonny/locale/ko_KR/HELP_CONTENT/debuggers.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     6151 2021-04-30 13:51:14.000000 thonny-4.1.0b1.dev0/thonny/locale/ko_KR/HELP_CONTENT/debugging.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     1292 2021-04-30 13:51:14.000000 thonny-4.1.0b1.dev0/thonny/locale/ko_KR/HELP_CONTENT/dock.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     2503 2021-04-30 13:51:14.000000 thonny-4.1.0b1.dev0/thonny/locale/ko_KR/HELP_CONTENT/errors.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     2108 2021-04-30 13:51:14.000000 thonny-4.1.0b1.dev0/thonny/locale/ko_KR/HELP_CONTENT/flask.rst
+-rw-r--r--   0 aivar      (501) staff       (20)      886 2021-04-30 13:51:14.000000 thonny-4.1.0b1.dev0/thonny/locale/ko_KR/HELP_CONTENT/index.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     1142 2021-04-30 13:51:14.000000 thonny-4.1.0b1.dev0/thonny/locale/ko_KR/HELP_CONTENT/modes.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     2719 2021-04-30 13:51:14.000000 thonny-4.1.0b1.dev0/thonny/locale/ko_KR/HELP_CONTENT/packages.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     2482 2021-04-30 13:51:14.000000 thonny-4.1.0b1.dev0/thonny/locale/ko_KR/HELP_CONTENT/plotter.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     1245 2021-04-30 13:51:14.000000 thonny-4.1.0b1.dev0/thonny/locale/ko_KR/HELP_CONTENT/program_arguments.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     4213 2021-04-30 13:51:14.000000 thonny-4.1.0b1.dev0/thonny/locale/ko_KR/HELP_CONTENT/shell.rst
+-rw-r--r--   0 aivar      (501) staff       (20)      646 2021-04-30 13:51:14.000000 thonny-4.1.0b1.dev0/thonny/locale/ko_KR/HELP_CONTENT/turtle.rst
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.275312 thonny-4.1.0b1.dev0/thonny/locale/ko_KR/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    29558 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/ko_KR/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    51805 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/ko_KR/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.960874 thonny-4.1.0b1.dev0/thonny/locale/lt_LT/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.278391 thonny-4.1.0b1.dev0/thonny/locale/lt_LT/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    26421 2019-11-03 18:24:01.000000 thonny-4.1.0b1.dev0/thonny/locale/lt_LT/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    40681 2021-01-14 21:04:27.000000 thonny-4.1.0b1.dev0/thonny/locale/lt_LT/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.962410 thonny-4.1.0b1.dev0/thonny/locale/nb_NO/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.283596 thonny-4.1.0b1.dev0/thonny/locale/nb_NO/HELP_CONTENT/
+-rw-r--r--   0 aivar      (501) staff       (20)     6043 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/nb_NO/HELP_CONTENT/debugging.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     2084 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/nb_NO/HELP_CONTENT/errors.rst
+-rw-r--r--   0 aivar      (501) staff       (20)      754 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/nb_NO/HELP_CONTENT/index.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     3988 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/nb_NO/HELP_CONTENT/shell.rst
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.285107 thonny-4.1.0b1.dev0/thonny/locale/nb_NO/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    23574 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/nb_NO/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    49831 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/nb_NO/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.963317 thonny-4.1.0b1.dev0/thonny/locale/nl_NL/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.288007 thonny-4.1.0b1.dev0/thonny/locale/nl_NL/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    27734 2021-02-17 13:22:04.000000 thonny-4.1.0b1.dev0/thonny/locale/nl_NL/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    48672 2021-02-17 13:22:04.000000 thonny-4.1.0b1.dev0/thonny/locale/nl_NL/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.963899 thonny-4.1.0b1.dev0/thonny/locale/nn_NO/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.290718 thonny-4.1.0b1.dev0/thonny/locale/nn_NO/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    21613 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/nn_NO/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    49202 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/nn_NO/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.964463 thonny-4.1.0b1.dev0/thonny/locale/pl_PL/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.292611 thonny-4.1.0b1.dev0/thonny/locale/pl_PL/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    28441 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/pl_PL/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    52478 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/pl_PL/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.965430 thonny-4.1.0b1.dev0/thonny/locale/pt_BR/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.310047 thonny-4.1.0b1.dev0/thonny/locale/pt_BR/HELP_CONTENT/
+-rw-r--r--   0 aivar      (501) staff       (20)     1528 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/locale/pt_BR/HELP_CONTENT/assistant.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     1558 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/locale/pt_BR/HELP_CONTENT/birdseye.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     4485 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/locale/pt_BR/HELP_CONTENT/debuggers.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     5245 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/locale/pt_BR/HELP_CONTENT/debugging.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     1330 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/locale/pt_BR/HELP_CONTENT/dock.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     2096 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/locale/pt_BR/HELP_CONTENT/errors.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     2003 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/locale/pt_BR/HELP_CONTENT/flask.rst
+-rw-r--r--   0 aivar      (501) staff       (20)      740 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/locale/pt_BR/HELP_CONTENT/index.rst
+-rw-r--r--   0 aivar      (501) staff       (20)      920 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/locale/pt_BR/HELP_CONTENT/modes.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     2977 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/locale/pt_BR/HELP_CONTENT/packages.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     2308 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/locale/pt_BR/HELP_CONTENT/plotter.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     1230 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/locale/pt_BR/HELP_CONTENT/program_arguments.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     4024 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/locale/pt_BR/HELP_CONTENT/shell.rst
+-rw-r--r--   0 aivar      (501) staff       (20)      649 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/locale/pt_BR/HELP_CONTENT/turtle.rst
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.312904 thonny-4.1.0b1.dev0/thonny/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    35547 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/pt_BR/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    55866 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/pt_BR/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.966538 thonny-4.1.0b1.dev0/thonny/locale/pt_PT/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.314839 thonny-4.1.0b1.dev0/thonny/locale/pt_PT/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    26955 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/locale/pt_PT/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    40981 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/locale/pt_PT/LC_MESSAGES/thonny.po
+-rw-r--r--   0 aivar      (501) staff       (20)     1512 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/locale/register_updates.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.967303 thonny-4.1.0b1.dev0/thonny/locale/ro_RO/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.316738 thonny-4.1.0b1.dev0/thonny/locale/ro_RO/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    32776 2021-02-17 13:22:04.000000 thonny-4.1.0b1.dev0/thonny/locale/ro_RO/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    51239 2021-02-17 13:22:04.000000 thonny-4.1.0b1.dev0/thonny/locale/ro_RO/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.968158 thonny-4.1.0b1.dev0/thonny/locale/ru_RU/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.320814 thonny-4.1.0b1.dev0/thonny/locale/ru_RU/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    46239 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/ru_RU/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    66723 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/ru_RU/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.968792 thonny-4.1.0b1.dev0/thonny/locale/sk_SK/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.324152 thonny-4.1.0b1.dev0/thonny/locale/sk_SK/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    34201 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/sk_SK/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    55163 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/sk_SK/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.970134 thonny-4.1.0b1.dev0/thonny/locale/sl_SI/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.328139 thonny-4.1.0b1.dev0/thonny/locale/sl_SI/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    33078 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/sl_SI/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    54237 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/sl_SI/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.973340 thonny-4.1.0b1.dev0/thonny/locale/sq_AL/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.330738 thonny-4.1.0b1.dev0/thonny/locale/sq_AL/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    34380 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/sq_AL/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    54032 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/sq_AL/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.976378 thonny-4.1.0b1.dev0/thonny/locale/sv_SE/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.332374 thonny-4.1.0b1.dev0/thonny/locale/sv_SE/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)     9758 2020-07-06 19:08:58.000000 thonny-4.1.0b1.dev0/thonny/locale/sv_SE/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    33357 2020-07-06 19:08:58.000000 thonny-4.1.0b1.dev0/thonny/locale/sv_SE/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.979226 thonny-4.1.0b1.dev0/thonny/locale/ta_IN/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.333951 thonny-4.1.0b1.dev0/thonny/locale/ta_IN/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    61109 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/ta_IN/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    80796 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/ta_IN/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.980766 thonny-4.1.0b1.dev0/thonny/locale/th_TH/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.339321 thonny-4.1.0b1.dev0/thonny/locale/th_TH/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    50299 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/th_TH/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    69932 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/th_TH/LC_MESSAGES/thonny.po
+-rw-r--r--   0 aivar      (501) staff       (20)    42558 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/locale/thonny.pot
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.981948 thonny-4.1.0b1.dev0/thonny/locale/tr_TR/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.342940 thonny-4.1.0b1.dev0/thonny/locale/tr_TR/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    26908 2019-11-18 18:57:56.000000 thonny-4.1.0b1.dev0/thonny/locale/tr_TR/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    41183 2019-11-18 18:57:56.000000 thonny-4.1.0b1.dev0/thonny/locale/tr_TR/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.982927 thonny-4.1.0b1.dev0/thonny/locale/uk_UA/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.347207 thonny-4.1.0b1.dev0/thonny/locale/uk_UA/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    34630 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/locale/uk_UA/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    48861 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/locale/uk_UA/LC_MESSAGES/thonny.po
+-rw-r--r--   0 aivar      (501) staff       (20)      108 2020-11-15 16:51:08.000000 thonny-4.1.0b1.dev0/thonny/locale/update_pot.bat
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.985003 thonny-4.1.0b1.dev0/thonny/locale/vi_VN/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.349322 thonny-4.1.0b1.dev0/thonny/locale/vi_VN/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    35515 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/vi_VN/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    57308 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/vi_VN/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.986907 thonny-4.1.0b1.dev0/thonny/locale/zh_CN/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.351057 thonny-4.1.0b1.dev0/thonny/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    31548 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/zh_CN/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    54185 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/zh_CN/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.987942 thonny-4.1.0b1.dev0/thonny/locale/zh_TW/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.354466 thonny-4.1.0b1.dev0/thonny/locale/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    32353 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/zh_TW/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    52653 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/zh_TW/LC_MESSAGES/thonny.po
+-rw-r--r--   0 aivar      (501) staff       (20)     4243 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/memory.py
+-rw-r--r--   0 aivar      (501) staff       (20)    17771 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/misc_utils.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.422508 thonny-4.1.0b1.dev0/thonny/plugins/
+-rw-r--r--   0 aivar      (501) staff       (20)       17 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/__init__.py
+-rw-r--r--   0 aivar      (501) staff       (20)     5075 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/plugins/about.py
+-rw-r--r--   0 aivar      (501) staff       (20)     2652 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/plugins/assistant_config_page.py
+-rw-r--r--   0 aivar      (501) staff       (20)     7502 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/plugins/ast_view.py
+-rw-r--r--   0 aivar      (501) staff       (20)    18878 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/plugins/autocomplete.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.430244 thonny-4.1.0b1.dev0/thonny/plugins/backend/
+-rw-r--r--   0 aivar      (501) staff       (20)       17 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/backend/__init__.py
+-rw-r--r--   0 aivar      (501) staff       (20)     1494 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/plugins/backend/birdseye_backend.py
+-rw-r--r--   0 aivar      (501) staff       (20)     2145 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/plugins/backend/dock_user_windows_backend.py
+-rw-r--r--   0 aivar      (501) staff       (20)     1604 2023-04-22 07:29:07.000000 thonny-4.1.0b1.dev0/thonny/plugins/backend/flask_backend.py
+-rw-r--r--   0 aivar      (501) staff       (20)     1116 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/plugins/backend/matplotlib_backend.py
+-rw-r--r--   0 aivar      (501) staff       (20)     2802 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/plugins/backend/pgzero_backend.py
+-rw-r--r--   0 aivar      (501) staff       (20)    11570 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/plugins/backend_config_page.py
+-rw-r--r--   0 aivar      (501) staff       (20)    19598 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/plugins/base_syntax_themes.py
+-rw-r--r--   0 aivar      (501) staff       (20)    23891 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/plugins/base_ui_themes.py
+-rw-r--r--   0 aivar      (501) staff       (20)     2483 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/plugins/birdseye_frontend.py
+-rw-r--r--   0 aivar      (501) staff       (20)     5647 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/plugins/calltip.py
+-rw-r--r--   0 aivar      (501) staff       (20)     6276 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/plugins/cells.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.432920 thonny-4.1.0b1.dev0/thonny/plugins/circuitpython/
+-rw-r--r--   0 aivar      (501) staff       (20)      396 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/plugins/circuitpython/__init__.py
+-rw-r--r--   0 aivar      (501) staff       (20)     4461 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/plugins/circuitpython/cirpy_back.py
+-rw-r--r--   0 aivar      (501) staff       (20)     4238 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/plugins/circuitpython/cirpy_front.py
+-rw-r--r--   0 aivar      (501) staff       (20)    14106 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/plugins/clean_ui_themes.py
+-rw-r--r--   0 aivar      (501) staff       (20)    12566 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/coloring.py
+-rw-r--r--   0 aivar      (501) staff       (20)     5561 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/plugins/commenting_indenting.py
+-rw-r--r--   0 aivar      (501) staff       (20)     2683 2020-09-02 21:27:22.000000 thonny-4.1.0b1.dev0/thonny/plugins/common_editing_commands.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.437427 thonny-4.1.0b1.dev0/thonny/plugins/cpython_backend/
+-rw-r--r--   0 aivar      (501) staff       (20)      226 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/cpython_backend/__init__.py
+-rw-r--r--   0 aivar      (501) staff       (20)    51717 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/plugins/cpython_backend/cp_back.py
+-rw-r--r--   0 aivar      (501) staff       (20)     1883 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/plugins/cpython_backend/cp_launcher.py
+-rw-r--r--   0 aivar      (501) staff       (20)    57896 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/plugins/cpython_backend/cp_tracers.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.444018 thonny-4.1.0b1.dev0/thonny/plugins/cpython_frontend/
+-rw-r--r--   0 aivar      (501) staff       (20)      920 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/cpython_frontend/__init__.py
+-rw-r--r--   0 aivar      (501) staff       (20)    18540 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/plugins/cpython_frontend/cp_front.py
+-rw-r--r--   0 aivar      (501) staff       (20)     1926 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/cpython_frontend/cp_pip_gui.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.449771 thonny-4.1.0b1.dev0/thonny/plugins/cpython_ssh/
+-rw-r--r--   0 aivar      (501) staff       (20)      808 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/cpython_ssh/__init__.py
+-rw-r--r--   0 aivar      (501) staff       (20)     7613 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/plugins/cpython_ssh/cps_back.py
+-rw-r--r--   0 aivar      (501) staff       (20)     5685 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/plugins/cpython_ssh/cps_front.py
+-rw-r--r--   0 aivar      (501) staff       (20)      361 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/cpython_ssh/cps_pip_gui.py
+-rw-r--r--   0 aivar      (501) staff       (20)    49636 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/plugins/debugger.py
+-rw-r--r--   0 aivar      (501) staff       (20)      812 2020-09-02 21:27:22.000000 thonny-4.1.0b1.dev0/thonny/plugins/dock_user_windows_frontend.py
+-rw-r--r--   0 aivar      (501) staff       (20)     3703 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/editor_config_page.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.451084 thonny-4.1.0b1.dev0/thonny/plugins/esp/
+-rw-r--r--   0 aivar      (501) staff       (20)     2446 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/plugins/esp/__init__.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.453171 thonny-4.1.0b1.dev0/thonny/plugins/esp/esp32_api_stubs/
+-rw-r--r--   0 aivar      (501) staff       (20)    18158 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/esp/esp32_api_stubs/esp32.pyi
+-rw-r--r--   0 aivar      (501) staff       (20)      555 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/esp/esp32_api_stubs/mp-1.18-esp32.txt
+-rw-r--r--   0 aivar      (501) staff       (20)      988 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/plugins/esp/esp_back.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.455284 thonny-4.1.0b1.dev0/thonny/plugins/ev3/
+-rw-r--r--   0 aivar      (501) staff       (20)     4254 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/ev3/__init__.py
+-rw-r--r--   0 aivar      (501) staff       (20)      996 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/plugins/ev3/ev3_back.py
+-rw-r--r--   0 aivar      (501) staff       (20)     6623 2021-07-25 16:05:48.000000 thonny-4.1.0b1.dev0/thonny/plugins/event_logging.py
+-rw-r--r--   0 aivar      (501) staff       (20)     1535 2020-09-02 21:27:22.000000 thonny-4.1.0b1.dev0/thonny/plugins/event_view.py
+-rw-r--r--   0 aivar      (501) staff       (20)    20730 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/files.py
+-rw-r--r--   0 aivar      (501) staff       (20)    18116 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/plugins/find_replace.py
+-rw-r--r--   0 aivar      (501) staff       (20)     5383 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/general_config_page.py
+-rw-r--r--   0 aivar      (501) staff       (20)     4520 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/goto_definition.py
+-rw-r--r--   0 aivar      (501) staff       (20)     2987 2020-11-15 16:51:08.000000 thonny-4.1.0b1.dev0/thonny/plugins/heap.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.472442 thonny-4.1.0b1.dev0/thonny/plugins/help/
+-rw-r--r--   0 aivar      (501) staff       (20)     2508 2020-12-04 16:41:08.000000 thonny-4.1.0b1.dev0/thonny/plugins/help/__init__.py
+-rw-r--r--   0 aivar      (501) staff       (20)     1366 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/plugins/help/assistant.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     1410 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/plugins/help/birdseye.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     4009 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/plugins/help/debuggers.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     5114 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/help/debugging.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     1131 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/plugins/help/dock.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     1969 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/help/errors.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     1764 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/plugins/help/flask.rst
+-rw-r--r--   0 aivar      (501) staff       (20)      677 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/help/index.rst
+-rw-r--r--   0 aivar      (501) staff       (20)      816 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/plugins/help/modes.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     2633 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/plugins/help/packages.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     2183 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/help/plotter.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     1038 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/plugins/help/program_arguments.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     3650 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/plugins/help/shell.rst
+-rw-r--r--   0 aivar      (501) staff       (20)      569 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/help/turtle.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     4104 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/plugins/highlight_names.py
+-rw-r--r--   0 aivar      (501) staff       (20)     4178 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/locals_marker.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.475282 thonny-4.1.0b1.dev0/thonny/plugins/microbit/
+-rw-r--r--   0 aivar      (501) staff       (20)     7039 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/plugins/microbit/__init__.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.502717 thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/
+-rw-r--r--   0 aivar      (501) staff       (20)       20 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/antigravity.pyi
+-rw-r--r--   0 aivar      (501) staff       (20)      184 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/array.pyi
+-rw-r--r--   0 aivar      (501) staff       (20)     1299 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/audio.pyi
+-rw-r--r--   0 aivar      (501) staff       (20)      402 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/collections.py
+-rw-r--r--   0 aivar      (501) staff       (20)      186 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/gc.py
+-rw-r--r--   0 aivar      (501) staff       (20)       68 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/love.pyi
+-rw-r--r--   0 aivar      (501) staff       (20)      204 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/machine.py
+-rw-r--r--   0 aivar      (501) staff       (20)      617 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/math.py
+-rw-r--r--   0 aivar      (501) staff       (20)    33816 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/microbit.pyi
+-rw-r--r--   0 aivar      (501) staff       (20)      218 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/micropython.py
+-rw-r--r--   0 aivar      (501) staff       (20)     8815 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/music.pyi
+-rw-r--r--   0 aivar      (501) staff       (20)     3287 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/neopixel.pyi
+-rw-r--r--   0 aivar      (501) staff       (20)      916 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/os.pyi
+-rw-r--r--   0 aivar      (501) staff       (20)     6453 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/radio.pyi
+-rw-r--r--   0 aivar      (501) staff       (20)     1486 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/random.pyi
+-rw-r--r--   0 aivar      (501) staff       (20)     1676 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/speech.pyi
+-rw-r--r--   0 aivar      (501) staff       (20)       66 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/struct.pyi
+-rw-r--r--   0 aivar      (501) staff       (20)     4365 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/sys.pyi
+-rw-r--r--   0 aivar      (501) staff       (20)       85 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/this.pyi
+-rw-r--r--   0 aivar      (501) staff       (20)      187 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/time.py
+-rw-r--r--   0 aivar      (501) staff       (20)     7935 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/uarray.pyi
+-rw-r--r--   0 aivar      (501) staff       (20)      402 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/ucollections.py
+-rw-r--r--   0 aivar      (501) staff       (20)     2138 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/ustruct.pyi
+-rw-r--r--   0 aivar      (501) staff       (20)     9148 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/utime.pyi
+-rw-r--r--   0 aivar      (501) staff       (20)      880 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/plugins/microbit/microbit_back.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.525368 thonny-4.1.0b1.dev0/thonny/plugins/micropython/
+-rw-r--r--   0 aivar      (501) staff       (20)     1914 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/plugins/micropython/__init__.py
+-rw-r--r--   0 aivar      (501) staff       (20)    64546 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/plugins/micropython/bare_metal_backend.py
+-rw-r--r--   0 aivar      (501) staff       (20)    21237 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/plugins/micropython/base_flashing_dialog.py
+-rw-r--r--   0 aivar      (501) staff       (20)     6269 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/micropython/connection.py
+-rw-r--r--   0 aivar      (501) staff       (20)    20159 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/plugins/micropython/esptool_dialog.py
+-rw-r--r--   0 aivar      (501) staff       (20)      345 2020-11-02 17:21:06.000000 thonny-4.1.0b1.dev0/thonny/plugins/micropython/miniterm_wrapper.py
+-rw-r--r--   0 aivar      (501) staff       (20)    52302 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/plugins/micropython/mp_back.py
+-rw-r--r--   0 aivar      (501) staff       (20)       88 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/micropython/mp_common.py
+-rw-r--r--   0 aivar      (501) staff       (20)    36776 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/plugins/micropython/mp_front.py
+-rw-r--r--   0 aivar      (501) staff       (20)    13352 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/plugins/micropython/os_mp_backend.py
+-rw-r--r--   0 aivar      (501) staff       (20)     4819 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/micropython/pip_gui.py
+-rw-r--r--   0 aivar      (501) staff       (20)     6515 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/plugins/micropython/serial_connection.py
+-rw-r--r--   0 aivar      (501) staff       (20)     1621 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/micropython/ssh_connection.py
+-rw-r--r--   0 aivar      (501) staff       (20)     1862 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/micropython/subprocess_connection.py
+-rw-r--r--   0 aivar      (501) staff       (20)     9964 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/plugins/micropython/uf2dialog.py
+-rw-r--r--   0 aivar      (501) staff       (20)     4561 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/plugins/micropython/webrepl_connection.py
+-rw-r--r--   0 aivar      (501) staff       (20)     6307 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/plugins/misc_analyzers.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.526981 thonny-4.1.0b1.dev0/thonny/plugins/mypy/
+-rw-r--r--   0 aivar      (501) staff       (20)     4134 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/mypy/__init__.py
+-rw-r--r--   0 aivar      (501) staff       (20)     2102 2020-09-02 21:27:22.000000 thonny-4.1.0b1.dev0/thonny/plugins/notes.py
+-rw-r--r--   0 aivar      (501) staff       (20)    26582 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/plugins/object_inspector.py
+-rw-r--r--   0 aivar      (501) staff       (20)     5194 2021-04-30 13:51:14.000000 thonny-4.1.0b1.dev0/thonny/plugins/outline.py
+-rw-r--r--   0 aivar      (501) staff       (20)     8057 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/plugins/paren_matcher.py
+-rw-r--r--   0 aivar      (501) staff       (20)      734 2020-09-02 21:27:22.000000 thonny-4.1.0b1.dev0/thonny/plugins/pgzero_frontend.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.527966 thonny-4.1.0b1.dev0/thonny/plugins/pi/
+-rw-r--r--   0 aivar      (501) staff       (20)    12209 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/__init__.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.625185 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/
+-rw-r--r--   0 aivar      (501) staff       (20)      206 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/Ukraine.png
+-rw-r--r--   0 aivar      (501) staff       (20)      328 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/Ukraine48.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1525 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_debug-run-cursor.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1525 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_debug-run-cursor48.png
+-rw-r--r--   0 aivar      (501) staff       (20)      668 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_debug-run.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1012 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_debug-run48.png
+-rw-r--r--   0 aivar      (501) staff       (20)      590 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_debug-step-into.png
+-rw-r--r--   0 aivar      (501) staff       (20)      894 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_debug-step-into48.png
+-rw-r--r--   0 aivar      (501) staff       (20)      586 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_debug-step-out.png
+-rw-r--r--   0 aivar      (501) staff       (20)      882 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_debug-step-out48.png
+-rw-r--r--   0 aivar      (501) staff       (20)      577 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_debug-step-over.png
+-rw-r--r--   0 aivar      (501) staff       (20)      861 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_debug-step-over48.png
+-rw-r--r--   0 aivar      (501) staff       (20)      403 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_document-new.png
+-rw-r--r--   0 aivar      (501) staff       (20)      530 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_document-new48.png
+-rw-r--r--   0 aivar      (501) staff       (20)      731 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_document-open.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1221 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_document-open48.png
+-rw-r--r--   0 aivar      (501) staff       (20)      691 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_document-save.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1082 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_document-save48.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1146 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_media-playback-start.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1806 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_media-playback-start48.png
+-rw-r--r--   0 aivar      (501) staff       (20)      993 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_process-stop.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1476 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_process-stop48.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1082 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_quit.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1741 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_quit48.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1133 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_resume.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1763 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_resume48.png
+-rw-r--r--   0 aivar      (501) staff       (20)      177 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_scrollbar-button-down-insens.png
+-rw-r--r--   0 aivar      (501) staff       (20)      208 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_scrollbar-button-down.png
+-rw-r--r--   0 aivar      (501) staff       (20)      160 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_scrollbar-button-left-insens.png
+-rw-r--r--   0 aivar      (501) staff       (20)      207 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_scrollbar-button-left.png
+-rw-r--r--   0 aivar      (501) staff       (20)      173 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_scrollbar-button-right-insens.png
+-rw-r--r--   0 aivar      (501) staff       (20)      202 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_scrollbar-button-right.png
+-rw-r--r--   0 aivar      (501) staff       (20)      175 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_scrollbar-button-up-insens.png
+-rw-r--r--   0 aivar      (501) staff       (20)      187 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_scrollbar-button-up.png
+-rw-r--r--   0 aivar      (501) staff       (20)      633 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_window-close-act.png
+-rw-r--r--   0 aivar      (501) staff       (20)      423 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_window-close.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1488 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_zoom.png
+-rw-r--r--   0 aivar      (501) staff       (20)     2349 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_zoom48.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1589 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/debug-run-cursor.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1589 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/debug-run-cursor48.png
+-rw-r--r--   0 aivar      (501) staff       (20)      746 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/debug-run.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1150 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/debug-run48.png
+-rw-r--r--   0 aivar      (501) staff       (20)      659 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/debug-step-into.png
+-rw-r--r--   0 aivar      (501) staff       (20)      980 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/debug-step-into48.png
+-rw-r--r--   0 aivar      (501) staff       (20)      644 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/debug-step-out.png
+-rw-r--r--   0 aivar      (501) staff       (20)      976 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/debug-step-out48.png
+-rw-r--r--   0 aivar      (501) staff       (20)      637 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/debug-step-over.png
+-rw-r--r--   0 aivar      (501) staff       (20)      962 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/debug-step-over48.png
+-rw-r--r--   0 aivar      (501) staff       (20)      445 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/document-new.png
+-rw-r--r--   0 aivar      (501) staff       (20)      611 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/document-new48.png
+-rw-r--r--   0 aivar      (501) staff       (20)      800 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/document-open.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1354 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/document-open48.png
+-rw-r--r--   0 aivar      (501) staff       (20)      770 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/document-save.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1223 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/document-save48.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1337 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/media-playback-start.png
+-rw-r--r--   0 aivar      (501) staff       (20)     2072 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/media-playback-start48.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1139 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/process-stop.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1663 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/process-stop48.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1207 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/quit.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1988 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/quit48.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1258 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/resume.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1977 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/resume48.png
+-rw-r--r--   0 aivar      (501) staff       (20)     2866 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/scrollbar-button-down-insens.png
+-rw-r--r--   0 aivar      (501) staff       (20)     2857 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/scrollbar-button-down.png
+-rw-r--r--   0 aivar      (501) staff       (20)     2857 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/scrollbar-button-left-insens.png
+-rw-r--r--   0 aivar      (501) staff       (20)     2834 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/scrollbar-button-left.png
+-rw-r--r--   0 aivar      (501) staff       (20)     2865 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/scrollbar-button-right-insens.png
+-rw-r--r--   0 aivar      (501) staff       (20)     2858 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/scrollbar-button-right.png
+-rw-r--r--   0 aivar      (501) staff       (20)     2859 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/scrollbar-button-up-insens.png
+-rw-r--r--   0 aivar      (501) staff       (20)     2862 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/scrollbar-button-up.png
+-rw-r--r--   0 aivar      (501) staff       (20)    16273 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/window-close-act.png
+-rw-r--r--   0 aivar      (501) staff       (20)      505 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/window-close.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1513 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/zoom.png
+-rw-r--r--   0 aivar      (501) staff       (20)     2561 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/zoom48.png
+-rw-r--r--   0 aivar      (501) staff       (20)    55548 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/plugins/pip_gui.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.626815 thonny-4.1.0b1.dev0/thonny/plugins/prime_inventor/
+-rw-r--r--   0 aivar      (501) staff       (20)     1774 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/plugins/prime_inventor/__init__.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.629023 thonny-4.1.0b1.dev0/thonny/plugins/prime_inventor/api_stubs/
+-rw-r--r--   0 aivar      (501) staff       (20)    19398 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/prime_inventor/api_stubs/hub.pyi
+-rw-r--r--   0 aivar      (501) staff       (20)      663 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/prime_inventor/prime_inventor_back.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.631280 thonny-4.1.0b1.dev0/thonny/plugins/printing/
+-rw-r--r--   0 aivar      (501) staff       (20)     2778 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/printing/__init__.py
+-rw-r--r--   0 aivar      (501) staff       (20)     1382 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/printing/template.html
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.633208 thonny-4.1.0b1.dev0/thonny/plugins/pylint/
+-rw-r--r--   0 aivar      (501) staff       (20)     6186 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/pylint/__init__.py
+-rw-r--r--   0 aivar      (501) staff       (20)   155507 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/pylint/messages.py
+-rw-r--r--   0 aivar      (501) staff       (20)     1131 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/pythontutor.py
+-rw-r--r--   0 aivar      (501) staff       (20)     1514 2020-09-29 16:35:00.000000 thonny-4.1.0b1.dev0/thonny/plugins/remove_old_data_dir.py
+-rw-r--r--   0 aivar      (501) staff       (20)    13491 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/plugins/replayer.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.635136 thonny-4.1.0b1.dev0/thonny/plugins/rp2040/
+-rw-r--r--   0 aivar      (501) staff       (20)     1692 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/plugins/rp2040/__init__.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.641796 thonny-4.1.0b1.dev0/thonny/plugins/rp2040/api_stubs/
+-rw-r--r--   0 aivar      (501) staff       (20)      344 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/rp2040/api_stubs/mp-1.18-pico.txt
+-rw-r--r--   0 aivar      (501) staff       (20)     9549 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/rp2040/api_stubs/rp2.pyi
+-rw-r--r--   0 aivar      (501) staff       (20)      891 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/plugins/rp2040/rp2040_back.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.643267 thonny-4.1.0b1.dev0/thonny/plugins/rpi_pico/
+-rw-r--r--   0 aivar      (501) staff       (20)     2003 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/rpi_pico/__init__.py
+-rw-r--r--   0 aivar      (501) staff       (20)     3051 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/plugins/run_debug_config_page.py
+-rw-r--r--   0 aivar      (501) staff       (20)     2564 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/shell_config_page.py
+-rw-r--r--   0 aivar      (501) staff       (20)     3497 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/plugins/shell_macro.py
+-rw-r--r--   0 aivar      (501) staff       (20)     8449 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/plugins/statement_boxes.py
+-rw-r--r--   0 aivar      (501) staff       (20)    25880 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/plugins/stdlib_error_helpers.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.647794 thonny-4.1.0b1.dev0/thonny/plugins/system_shell/
+-rw-r--r--   0 aivar      (501) staff       (20)     2183 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/system_shell/__init__.py
+-rwxr-xr-x   0 aivar      (501) staff       (20)     5377 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/plugins/system_shell/explain_environment.py
+-rw-r--r--   0 aivar      (501) staff       (20)     1375 2020-09-02 21:27:22.000000 thonny-4.1.0b1.dev0/thonny/plugins/terminal_config_page.py
+-rw-r--r--   0 aivar      (501) staff       (20)     9267 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/plugins/theme_and_font_config_page.py
+-rw-r--r--   0 aivar      (501) staff       (20)      763 2020-09-02 21:27:22.000000 thonny-4.1.0b1.dev0/thonny/plugins/thonny_folders.py
+-rw-r--r--   0 aivar      (501) staff       (20)     4599 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/plugins/todo_view.py
+-rw-r--r--   0 aivar      (501) staff       (20)     6327 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/tomorrow_syntax_theme.py
+-rw-r--r--   0 aivar      (501) staff       (20)     5411 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/variables.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.848070 thonny-4.1.0b1.dev0/thonny/res/
+-rw-r--r--   0 aivar      (501) staff       (20)      832 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/16x16-blank.gif
+-rw-r--r--   0 aivar      (501) staff       (20)      807 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/1x1-white.gif
+-rw-r--r--   0 aivar      (501) staff       (20)      270 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/PrintLnkTarget.vbs
+-rw-r--r--   0 aivar      (501) staff       (20)      171 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/res/Ukraine.png
+-rw-r--r--   0 aivar      (501) staff       (20)     5430 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/res/Ukraine_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      682 2020-09-02 21:27:22.000000 thonny-4.1.0b1.dev0/thonny/res/_create_disabled_variants.py
+-rw-r--r--   0 aivar      (501) staff       (20)      832 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_16x16-blank.gif
+-rw-r--r--   0 aivar      (501) staff       (20)      807 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_1x1-white.gif
+-rw-r--r--   0 aivar      (501) staff       (20)      837 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_arrow-down.gif
+-rw-r--r--   0 aivar      (501) staff       (20)      734 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_birdseye.png
+-rw-r--r--   0 aivar      (501) staff       (20)      199 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_boxdot.png
+-rw-r--r--   0 aivar      (501) staff       (20)      169 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_boxdot_light.png
+-rw-r--r--   0 aivar      (501) staff       (20)      192 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_boxminus.png
+-rw-r--r--   0 aivar      (501) staff       (20)      160 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_boxminus_light.png
+-rw-r--r--   0 aivar      (501) staff       (20)      212 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_boxplus.png
+-rw-r--r--   0 aivar      (501) staff       (20)      176 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_boxplus_light.png
+-rw-r--r--   0 aivar      (501) staff       (20)      224 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_boxx.png
+-rw-r--r--   0 aivar      (501) staff       (20)      179 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_boxx_light.png
+-rw-r--r--   0 aivar      (501) staff       (20)      908 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_broken.png
+-rw-r--r--   0 aivar      (501) staff       (20)      917 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_closed-folder.gif
+-rw-r--r--   0 aivar      (501) staff       (20)      577 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_debug-current-script.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1320 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_debug-current-script_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      877 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_delete.gif
+-rw-r--r--   0 aivar      (501) staff       (20)      907 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_folder.gif
+-rw-r--r--   0 aivar      (501) staff       (20)      881 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_generic-file.gif
+-rw-r--r--   0 aivar      (501) staff       (20)      895 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_hard-drive.gif
+-rw-r--r--   0 aivar      (501) staff       (20)      553 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_harddisk.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1177 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_harddisk_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      745 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_help.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1897 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_help_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      654 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_information.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1555 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_information_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      428 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_nav-backward.png
+-rw-r--r--   0 aivar      (501) staff       (20)      756 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_nav-backward_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      420 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_nav-forward.png
+-rw-r--r--   0 aivar      (501) staff       (20)      749 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_nav-forward_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      320 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_new-file.png
+-rw-r--r--   0 aivar      (501) staff       (20)      376 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_new-file_Linux.png
+-rw-r--r--   0 aivar      (501) staff       (20)      868 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_new-file_Linux_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      502 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_open-file.png
+-rw-r--r--   0 aivar      (501) staff       (20)      495 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_open-file_Linux.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1217 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_open-file_Linux_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      935 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_open_folder.gif
+-rw-r--r--   0 aivar      (501) staff       (20)      613 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_outline-class.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1324 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_outline-class_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      928 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_outline-method.gif
+-rw-r--r--   0 aivar      (501) staff       (20)      929 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_python-file.gif
+-rw-r--r--   0 aivar      (501) staff       (20)      945 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_python-icon.gif
+-rw-r--r--   0 aivar      (501) staff       (20)      461 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_quit.png
+-rw-r--r--   0 aivar      (501) staff       (20)      780 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_quit_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      469 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_resume.png
+-rw-r--r--   0 aivar      (501) staff       (20)      885 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_resume_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      620 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_run-current-script.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1281 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_run-current-script_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      339 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_run-to-cursor.png
+-rw-r--r--   0 aivar      (501) staff       (20)      612 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_run-to-cursor_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      460 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_save-file.png
+-rw-r--r--   0 aivar      (501) staff       (20)      944 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_save-file_2x_alt.png
+-rw-r--r--   0 aivar      (501) staff       (20)      604 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_save-file_Linux.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1611 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_save-file_Linux_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      518 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_save-file_alt.png
+-rw-r--r--   0 aivar      (501) staff       (20)      615 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_star.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1489 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_star_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      421 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_step-into.png
+-rw-r--r--   0 aivar      (501) staff       (20)      760 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_step-into_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      404 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_step-out.png
+-rw-r--r--   0 aivar      (501) staff       (20)      726 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_step-out_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      530 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_step-over.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1034 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_step-over_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      630 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_stop.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1888 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_stop_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      837 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_tab-close-active-clam-dark.gif
+-rw-r--r--   0 aivar      (501) staff       (20)      837 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_tab-close-active-clam.gif
+-rw-r--r--   0 aivar      (501) staff       (20)      837 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_tab-close-active.gif
+-rw-r--r--   0 aivar      (501) staff       (20)      842 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_tab-close-clam.gif
+-rw-r--r--   0 aivar      (501) staff       (20)      842 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_tab-close.gif
+-rw-r--r--   0 aivar      (501) staff       (20)      511 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_terminal.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1255 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_terminal_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      934 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_text-file.gif
+-rw-r--r--   0 aivar      (501) staff       (20)     5186 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_thonny.png
+-rw-r--r--   0 aivar      (501) staff       (20)      469 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_zoom.png
+-rw-r--r--   0 aivar      (501) staff       (20)      837 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/arrow-down.gif
+-rw-r--r--   0 aivar      (501) staff       (20)     1225 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/birdseye.png
+-rw-r--r--   0 aivar      (501) staff       (20)      282 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/boxdot.png
+-rw-r--r--   0 aivar      (501) staff       (20)      258 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/boxdot_light.png
+-rw-r--r--   0 aivar      (501) staff       (20)      272 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/boxminus.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1170 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/boxminus_light.png
+-rw-r--r--   0 aivar      (501) staff       (20)      288 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/boxplus.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1179 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/boxplus_light.png
+-rw-r--r--   0 aivar      (501) staff       (20)      312 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/boxx.png
+-rw-r--r--   0 aivar      (501) staff       (20)      264 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/boxx_light.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1535 2020-11-15 16:51:08.000000 thonny-4.1.0b1.dev0/thonny/res/broken.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1111 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/closed-folder.gif
+-rw-r--r--   0 aivar      (501) staff       (20)      563 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/debug-current-script.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1453 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/debug-current-script_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      900 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/delete.gif
+-rw-r--r--   0 aivar      (501) staff       (20)      386 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/folder.gif
+-rw-r--r--   0 aivar      (501) staff       (20)      238 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/generic-file.gif
+-rw-r--r--   0 aivar      (501) staff       (20)     1019 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/hard-drive.gif
+-rw-r--r--   0 aivar      (501) staff       (20)      847 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/harddisk.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1519 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/harddisk_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      932 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/help.png
+-rw-r--r--   0 aivar      (501) staff       (20)     2231 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/help_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      863 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/information.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1910 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/information_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      347 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/nav-backward.png
+-rw-r--r--   0 aivar      (501) staff       (20)      652 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/nav-backward_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      344 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/nav-forward.png
+-rw-r--r--   0 aivar      (501) staff       (20)      644 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/nav-forward_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      299 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/new-file.png
+-rw-r--r--   0 aivar      (501) staff       (20)      477 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/new-file_Linux.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1008 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/new-file_Linux_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      567 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/open-file.png
+-rw-r--r--   0 aivar      (501) staff       (20)      672 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/open-file_Linux.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1550 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/open-file_Linux_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1108 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/open_folder.gif
+-rw-r--r--   0 aivar      (501) staff       (20)      628 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/outline-class.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1129 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/outline-class_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      578 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/outline-method.gif
+-rw-r--r--   0 aivar      (501) staff       (20)      626 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/python-file.gif
+-rw-r--r--   0 aivar      (501) staff       (20)     1049 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/python-icon.gif
+-rw-r--r--   0 aivar      (501) staff       (20)     2430 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/res/python-icon_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      561 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/quit.png
+-rw-r--r--   0 aivar      (501) staff       (20)      984 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/quit_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      539 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/resume.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1046 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/resume_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      620 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/run-current-script.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1226 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/run-current-script_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      252 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/run-to-cursor.png
+-rw-r--r--   0 aivar      (501) staff       (20)      492 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/run-to-cursor_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      543 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/save-file.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1151 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/save-file_2x_alt.png
+-rw-r--r--   0 aivar      (501) staff       (20)      911 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/save-file_Linux.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1971 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/save-file_Linux_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      617 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/save-file_alt.png
+-rw-r--r--   0 aivar      (501) staff       (20)      950 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/star.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1800 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/star_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      356 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/step-into.png
+-rw-r--r--   0 aivar      (501) staff       (20)      761 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/step-into_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      379 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/step-out.png
+-rw-r--r--   0 aivar      (501) staff       (20)      798 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/step-out_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      457 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/step-over.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1014 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/step-over_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      718 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/stop.png
+-rw-r--r--   0 aivar      (501) staff       (20)     3595 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/res/stop_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)       58 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/tab-close-active-clam-dark.gif
+-rw-r--r--   0 aivar      (501) staff       (20)       58 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/tab-close-active-clam.gif
+-rw-r--r--   0 aivar      (501) staff       (20)       58 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/tab-close-active.gif
+-rw-r--r--   0 aivar      (501) staff       (20)      842 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/tab-close-clam.gif
+-rw-r--r--   0 aivar      (501) staff       (20)      842 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/tab-close.gif
+-rw-r--r--   0 aivar      (501) staff       (20)      668 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/terminal.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1488 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/terminal_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      627 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/text-file.gif
+-rw-r--r--   0 aivar      (501) staff       (20)    16652 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/thonny.ico
+-rw-r--r--   0 aivar      (501) staff       (20)     5134 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/thonny.png
+-rw-r--r--   0 aivar      (501) staff       (20)      894 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/thonny_small.ico
+-rw-r--r--   0 aivar      (501) staff       (20)      468 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/zoom.png
+-rw-r--r--   0 aivar      (501) staff       (20)    33753 2020-09-03 11:18:16.000000 thonny-4.1.0b1.dev0/thonny/roughparse.py
+-rw-r--r--   0 aivar      (501) staff       (20)    17497 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/rst_utils.py
+-rw-r--r--   0 aivar      (501) staff       (20)    57393 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/running.py
+-rw-r--r--   0 aivar      (501) staff       (20)    80009 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/shell.py
+-rw-r--r--   0 aivar      (501) staff       (20)     8048 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/terminal.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.851479 thonny-4.1.0b1.dev0/thonny/test/
+-rw-r--r--   0 aivar      (501) staff       (20)       17 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/test/__init__.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.856958 thonny-4.1.0b1.dev0/thonny/test/plugins/
+-rw-r--r--   0 aivar      (501) staff       (20)       17 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/test/plugins/__init__.py
+-rw-r--r--   0 aivar      (501) staff       (20)      598 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/test/plugins/test_locals_marker.py
+-rw-r--r--   0 aivar      (501) staff       (20)     3360 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/test/plugins/test_name_highlighter.py
+-rw-r--r--   0 aivar      (501) staff       (20)      336 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/test/plugins/test_pip_gui.py
+-rw-r--r--   0 aivar      (501) staff       (20)     1173 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/test/test_common.py
+-rw-r--r--   0 aivar      (501) staff       (20)    45325 2023-02-15 20:47:32.000000 thonny-4.1.0b1.dev0/thonny/tktextext.py
+-rw-r--r--   0 aivar      (501) staff       (20)     2262 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/token_utils.py
+-rw-r--r--   0 aivar      (501) staff       (20)     4914 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/udisks.py
+-rw-r--r--   0 aivar      (501) staff       (20)    83339 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/ui_utils.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.014799 thonny-4.1.0b1.dev0/thonny/vendored_libs/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.866424 thonny-4.1.0b1.dev0/thonny/vendored_libs/filelock/
+-rw-r--r--   0 aivar      (501) staff       (20)     1315 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/vendored_libs/filelock/__init__.py
+-rw-r--r--   0 aivar      (501) staff       (20)     8896 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/vendored_libs/filelock/_api.py
+-rw-r--r--   0 aivar      (501) staff       (20)      399 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/vendored_libs/filelock/_error.py
+-rw-r--r--   0 aivar      (501) staff       (20)     1650 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/vendored_libs/filelock/_soft.py
+-rw-r--r--   0 aivar      (501) staff       (20)     1578 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/vendored_libs/filelock/_unix.py
+-rw-r--r--   0 aivar      (501) staff       (20)      594 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/vendored_libs/filelock/_util.py
+-rw-r--r--   0 aivar      (501) staff       (20)     1890 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/vendored_libs/filelock/_windows.py
+-rw-r--r--   0 aivar      (501) staff       (20)        0 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/vendored_libs/filelock/py.typed
+-rw-r--r--   0 aivar      (501) staff       (20)      160 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/vendored_libs/filelock/version.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.882086 thonny-4.1.0b1.dev0/thonny/vendored_libs/pipkin/
+-rw-r--r--   0 aivar      (501) staff       (20)     1738 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/vendored_libs/pipkin/__init__.py
+-rw-r--r--   0 aivar      (501) staff       (20)     2114 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/vendored_libs/pipkin/__main__.py
+-rw-r--r--   0 aivar      (501) staff       (20)    16912 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/vendored_libs/pipkin/adapters.py
+-rw-r--r--   0 aivar      (501) staff       (20)    33595 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/vendored_libs/pipkin/bare_metal.py
+-rw-r--r--   0 aivar      (501) staff       (20)      355 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/vendored_libs/pipkin/common.py
+-rw-r--r--   0 aivar      (501) staff       (20)     6235 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/vendored_libs/pipkin/connection.py
+-rw-r--r--   0 aivar      (501) staff       (20)    10546 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/vendored_libs/pipkin/parser.py
+-rw-r--r--   0 aivar      (501) staff       (20)    18946 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/vendored_libs/pipkin/proxy.py
+-rw-r--r--   0 aivar      (501) staff       (20)     6599 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/vendored_libs/pipkin/serial_connection.py
+-rw-r--r--   0 aivar      (501) staff       (20)    27862 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/vendored_libs/pipkin/session.py
+-rw-r--r--   0 aivar      (501) staff       (20)     6702 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/vendored_libs/pipkin/util.py
+-rw-r--r--   0 aivar      (501) staff       (20)     4580 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/vendored_libs/pipkin/webrepl_connection.py
+-rw-r--r--   0 aivar      (501) staff       (20)    98557 2023-04-22 07:29:07.000000 thonny-4.1.0b1.dev0/thonny/workbench.py
+-rw-r--r--   0 aivar      (501) staff       (20)    16632 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/workdlg.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.151038 thonny-4.1.0b1.dev0/thonny.egg-info/
+-rw-r--r--   0 aivar      (501) staff       (20)     1759 2023-04-22 07:29:16.000000 thonny-4.1.0b1.dev0/thonny.egg-info/PKG-INFO
+-rw-r--r--   0 aivar      (501) staff       (20)    21822 2023-04-22 07:29:16.000000 thonny-4.1.0b1.dev0/thonny.egg-info/SOURCES.txt
+-rw-r--r--   0 aivar      (501) staff       (20)        1 2023-04-22 07:29:16.000000 thonny-4.1.0b1.dev0/thonny.egg-info/dependency_links.txt
+-rw-r--r--   0 aivar      (501) staff       (20)       38 2023-04-22 07:29:16.000000 thonny-4.1.0b1.dev0/thonny.egg-info/entry_points.txt
+-rw-r--r--   0 aivar      (501) staff       (20)      120 2023-04-22 07:29:16.000000 thonny-4.1.0b1.dev0/thonny.egg-info/requires.txt
+-rw-r--r--   0 aivar      (501) staff       (20)        7 2023-04-22 07:29:16.000000 thonny-4.1.0b1.dev0/thonny.egg-info/top_level.txt
```

### Comparing `thonny-4.1.0b1/CHANGELOG.rst` & `thonny-4.1.0b1.dev0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,54 +1,11 @@
 ===============
 Version history
 ===============
 
-4.1.0b1 (2023-04-23)
-====================
-
-New
----
-* Enhance esptool GUI (propose known MicroPython and CircuitPython downloads; allow setting baud rate and start address; allow querying device info), #2707, #1600, #2536, #1171, #2657
-* Ensure Thonny's backends don't get confused by other installations, #2616
-* Detect and warn if user module is shadowing a library module, #384
-* Make serial port description in interpreter selection menu more descriptive
-* Added pt_BR translation for all help pages, #2673, by @mgmalheiros
-* Add Pololu MicroPython downloads to UF2 flasher
-* Use UDisks to find mounted filesystems on Linux, #2683 by jwillikers
-
-Dependency changes
-------------------
-* Upgrade bundled Python from 3.10.9 to 3.10.11
-* Upgrade bundled Tk from 8.6.12 to 8.6.13
-* Upgrade bundled Pylint from 2.15 to 2.17
-* Upgrade bundled MyPy from 0.991 to 1.2
-
-Fixes
------
-* Fix a potential autocompletion error, #2162
-* Experiment with better MicroPython raw paste fallback, #2624
-* Fix sys.sdtout.write return value, #2629
-* Remove unnecessary shebangs, #2645
-* Add option for saving unnamed editors before Run/Debug, #2619
-* Fix blank editors in macOS, again, #2425
-* Fix todo view, #2681, by @kr-g
-* Minor corrections for English help pages, #2674, by @mgmalheiros
-* Upgrade bundled esptool from 4.4 to 4.5
-* Allow Linux installer to use existing Python 3.11 and 3.12, #2676
-* Require saving before using fast debugger, #2699, by @michaellass
-* Add missing translation sites in editors.py, #2705 by @nicolasdespres
-* Restore MicroPython completions in the shell, #2467, #2419
-* Don't use deprecated FLASK_ENV environment variable.
-* Add better shortcut for increasing font size in macOS, #2725
-* Avoid falling back to Python menu in simple mode on macOS, #2729
-* Various improvements to "Kind of Aqua" UI theme, #2760
-* Fix double paste with Command-V when CapsLock on, #2753
-* Fix Cut with Command-X when CapsLock on, #2753
-
-
 4.0.2 (2023-01-14)
 ==================
 * Fix Mypy logging error in the Assistant, #2491 by @kr-g and @solsword
 * Fix AttributeError on save, #2454
 * Add Thonny version as environment value for user programs, #2494 by @kr-g
 * Make `__file__` contain absolute path, #2497
 * Start SSH preparation command with space to avoid adding it to shell history, #2563 by @isaacl
```

### Comparing `thonny-4.1.0b1/CREDITS.rst` & `thonny-4.1.0b1.dev0/CREDITS.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/LICENSE.txt` & `thonny-4.1.0b1.dev0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/PKG-INFO` & `thonny-4.1.0b1.dev0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thonny
-Version: 4.1.0b1
+Version: 4.1.0b1.dev0
 Summary: Python IDE for beginners
 Home-page: https://thonny.org
 Author: Aivar Annamaa and others
 Author-email: thonny@googlegroups.com
 License: MIT
 Project-URL: Source code, https://github.com/thonny/thonny
 Project-URL: Bug tracker, https://github.com/thonny/thonny/issues
@@ -38,7 +38,8 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Debuggers
 Classifier: Topic :: Text Editors
 Requires-Python: >=3.8
 License-File: LICENSE.txt
 
 Thonny is a simple Python IDE with features useful for learning programming. See https://thonny.org for more info.
+
```

### Comparing `thonny-4.1.0b1/README.rst` & `thonny-4.1.0b1.dev0/README.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/licenses/ECLIPSE-ICONS-LICENSE.txt` & `thonny-4.1.0b1.dev0/licenses/ECLIPSE-ICONS-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/packaging/icons/thonny-128x128.png` & `thonny-4.1.0b1.dev0/packaging/icons/thonny-128x128.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/packaging/icons/thonny-192x192.png` & `thonny-4.1.0b1.dev0/packaging/icons/thonny-192x192.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/packaging/icons/thonny-22x22.png` & `thonny-4.1.0b1.dev0/packaging/icons/thonny-22x22.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/packaging/icons/thonny-256x256.png` & `thonny-4.1.0b1.dev0/packaging/icons/thonny-256x256.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/packaging/icons/thonny-32x32.png` & `thonny-4.1.0b1.dev0/packaging/icons/thonny-32x32.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/packaging/icons/thonny-48x48.png` & `thonny-4.1.0b1.dev0/packaging/icons/thonny-48x48.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/packaging/icons/thonny-64x64.png` & `thonny-4.1.0b1.dev0/packaging/icons/thonny-64x64.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/packaging/linux/org.thonny.Thonny.appdata.xml` & `thonny-4.1.0b1.dev0/packaging/linux/org.thonny.Thonny.appdata.xml`

 * *Files 2% similar despite different names*

#### Comparing `thonny-4.1.0b1/packaging/linux/org.thonny.Thonny.appdata.xml` & `thonny-4.1.0b1.dev0/packaging/linux/org.thonny.Thonny.appdata.xml`

```diff
@@ -32,19 +32,14 @@
     </screenshot>
   </screenshots>
   <provides>
     <binary>thonny</binary>
   </provides>
   <content_rating type="oars-1.1"/>
   <releases>
-    <release version="4.1.0b1" date="2023-04-23">
-      <description>
-        <p>Feature pre-release.</p>
-      </description>
-    </release>
     <release version="4.0.1" date="2022-09-11">
       <description>
         <p>Bug-fix release.</p>
       </description>
     </release>
     <release version="4.0.0" date="2022-08-22">
       <description>
```

### Comparing `thonny-4.1.0b1/packaging/linux/thonny.1` & `thonny-4.1.0b1.dev0/packaging/linux/thonny.1`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/setup.py` & `thonny-4.1.0b1.dev0/setup.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/__init__.py` & `thonny-4.1.0b1.dev0/thonny/__init__.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/assistance.py` & `thonny-4.1.0b1.dev0/thonny/assistance.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/ast_utils.py` & `thonny-4.1.0b1.dev0/thonny/ast_utils.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/backend.py` & `thonny-4.1.0b1.dev0/thonny/backend.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/base_file_browser.py` & `thonny-4.1.0b1.dev0/thonny/base_file_browser.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/codeview.py` & `thonny-4.1.0b1.dev0/thonny/codeview.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/common.py` & `thonny-4.1.0b1.dev0/thonny/common.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/config.py` & `thonny-4.1.0b1.dev0/thonny/config.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/config_ui.py` & `thonny-4.1.0b1.dev0/thonny/config_ui.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/dbus/org.freedesktop.DBus.ObjectManager.xml` & `thonny-4.1.0b1.dev0/thonny/dbus/org.freedesktop.DBus.ObjectManager.xml`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/dbus/org.freedesktop.UDisks2.xml` & `thonny-4.1.0b1.dev0/thonny/dbus/org.freedesktop.UDisks2.xml`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/editor_helpers.py` & `thonny-4.1.0b1.dev0/thonny/editor_helpers.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/editors.py` & `thonny-4.1.0b1.dev0/thonny/editors.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/export.py` & `thonny-4.1.0b1.dev0/thonny/export.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/first_run.py` & `thonny-4.1.0b1.dev0/thonny/first_run.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/gridtable.py` & `thonny-4.1.0b1.dev0/thonny/gridtable.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/jedi_utils.py` & `thonny-4.1.0b1.dev0/thonny/jedi_utils.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/languages.py` & `thonny-4.1.0b1.dev0/thonny/languages.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/ar_AR/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/ar_AR/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/ar_AR/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/ar_AR/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/cs_CZ/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/cs_CZ/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/cs_CZ/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/cs_CZ/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/de_DE/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/de_DE/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/de_DE/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/de_DE/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/el_GR/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/el_GR/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/el_GR/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/el_GR/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/en_US/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/en_US/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/es_ES/HELP_CONTENT/debuggers.rst` & `thonny-4.1.0b1.dev0/thonny/locale/es_ES/HELP_CONTENT/debuggers.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/es_ES/HELP_CONTENT/debugging.rst` & `thonny-4.1.0b1.dev0/thonny/locale/es_ES/HELP_CONTENT/debugging.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/es_ES/HELP_CONTENT/errors.rst` & `thonny-4.1.0b1.dev0/thonny/locale/es_ES/HELP_CONTENT/errors.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/es_ES/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/es_ES/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/es_ES/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/es_ES/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/et_EE/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/et_EE/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/et_EE/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/et_EE/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/fa_IR/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/fa_IR/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/fa_IR/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/fa_IR/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/fi_FI/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/fi_FI/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/fi_FI/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/fi_FI/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/fr_FR/HELP_CONTENT/birdseye.rst` & `thonny-4.1.0b1.dev0/thonny/locale/fr_FR/HELP_CONTENT/birdseye.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/fr_FR/HELP_CONTENT/debuggers.rst` & `thonny-4.1.0b1.dev0/thonny/locale/fr_FR/HELP_CONTENT/debuggers.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/fr_FR/HELP_CONTENT/debugging.rst` & `thonny-4.1.0b1.dev0/thonny/locale/fr_FR/HELP_CONTENT/debugging.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/fr_FR/HELP_CONTENT/dock.rst` & `thonny-4.1.0b1.dev0/thonny/locale/fr_FR/HELP_CONTENT/dock.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/fr_FR/HELP_CONTENT/errors.rst` & `thonny-4.1.0b1.dev0/thonny/locale/fr_FR/HELP_CONTENT/errors.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/fr_FR/HELP_CONTENT/flask.rst` & `thonny-4.1.0b1.dev0/thonny/locale/fr_FR/HELP_CONTENT/flask.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/fr_FR/HELP_CONTENT/index.rst` & `thonny-4.1.0b1.dev0/thonny/locale/fr_FR/HELP_CONTENT/index.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/fr_FR/HELP_CONTENT/modes.rst` & `thonny-4.1.0b1.dev0/thonny/locale/fr_FR/HELP_CONTENT/modes.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/fr_FR/HELP_CONTENT/packages.rst` & `thonny-4.1.0b1.dev0/thonny/locale/fr_FR/HELP_CONTENT/packages.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/fr_FR/HELP_CONTENT/plotter.rst` & `thonny-4.1.0b1.dev0/thonny/locale/fr_FR/HELP_CONTENT/plotter.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/fr_FR/HELP_CONTENT/program_arguments.rst` & `thonny-4.1.0b1.dev0/thonny/locale/fr_FR/HELP_CONTENT/program_arguments.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/fr_FR/HELP_CONTENT/shell.rst` & `thonny-4.1.0b1.dev0/thonny/locale/fr_FR/HELP_CONTENT/shell.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/fr_FR/HELP_CONTENT/turtle.rst` & `thonny-4.1.0b1.dev0/thonny/locale/fr_FR/HELP_CONTENT/turtle.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/fr_FR/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/fr_FR/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/fr_FR/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/fr_FR/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/hu_HU/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/hu_HU/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/hu_HU/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/hu_HU/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/hy_AM/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/hy_AM/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/hy_AM/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/hy_AM/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/it_IT/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/it_IT/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/it_IT/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/it_IT/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/ja_JP/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/ja_JP/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/ja_JP/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/ja_JP/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/ko_KR/HELP_CONTENT/birdseye.rst` & `thonny-4.1.0b1.dev0/thonny/locale/ko_KR/HELP_CONTENT/birdseye.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/ko_KR/HELP_CONTENT/debuggers.rst` & `thonny-4.1.0b1.dev0/thonny/locale/ko_KR/HELP_CONTENT/debuggers.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/ko_KR/HELP_CONTENT/debugging.rst` & `thonny-4.1.0b1.dev0/thonny/locale/ko_KR/HELP_CONTENT/debugging.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/ko_KR/HELP_CONTENT/dock.rst` & `thonny-4.1.0b1.dev0/thonny/locale/ko_KR/HELP_CONTENT/dock.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/ko_KR/HELP_CONTENT/errors.rst` & `thonny-4.1.0b1.dev0/thonny/locale/ko_KR/HELP_CONTENT/errors.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/ko_KR/HELP_CONTENT/flask.rst` & `thonny-4.1.0b1.dev0/thonny/locale/ko_KR/HELP_CONTENT/flask.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/ko_KR/HELP_CONTENT/index.rst` & `thonny-4.1.0b1.dev0/thonny/locale/ko_KR/HELP_CONTENT/index.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/ko_KR/HELP_CONTENT/modes.rst` & `thonny-4.1.0b1.dev0/thonny/locale/ko_KR/HELP_CONTENT/modes.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/ko_KR/HELP_CONTENT/packages.rst` & `thonny-4.1.0b1.dev0/thonny/locale/ko_KR/HELP_CONTENT/packages.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/ko_KR/HELP_CONTENT/plotter.rst` & `thonny-4.1.0b1.dev0/thonny/locale/ko_KR/HELP_CONTENT/plotter.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/ko_KR/HELP_CONTENT/program_arguments.rst` & `thonny-4.1.0b1.dev0/thonny/locale/ko_KR/HELP_CONTENT/program_arguments.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/ko_KR/HELP_CONTENT/shell.rst` & `thonny-4.1.0b1.dev0/thonny/locale/ko_KR/HELP_CONTENT/shell.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/ko_KR/HELP_CONTENT/turtle.rst` & `thonny-4.1.0b1.dev0/thonny/locale/ko_KR/HELP_CONTENT/turtle.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/ko_KR/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/ko_KR/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/ko_KR/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/ko_KR/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/lt_LT/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/lt_LT/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/lt_LT/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/lt_LT/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/nb_NO/HELP_CONTENT/debugging.rst` & `thonny-4.1.0b1.dev0/thonny/locale/nb_NO/HELP_CONTENT/debugging.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/nb_NO/HELP_CONTENT/errors.rst` & `thonny-4.1.0b1.dev0/thonny/locale/nb_NO/HELP_CONTENT/errors.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/nb_NO/HELP_CONTENT/index.rst` & `thonny-4.1.0b1.dev0/thonny/locale/nb_NO/HELP_CONTENT/index.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/nb_NO/HELP_CONTENT/shell.rst` & `thonny-4.1.0b1.dev0/thonny/locale/nb_NO/HELP_CONTENT/shell.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/nb_NO/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/nb_NO/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/nb_NO/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/nb_NO/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/nl_NL/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/nl_NL/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/nl_NL/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/nl_NL/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/nn_NO/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/nn_NO/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/nn_NO/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/nn_NO/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/pl_PL/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/pl_PL/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/pl_PL/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/pl_PL/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/pt_BR/HELP_CONTENT/assistant.rst` & `thonny-4.1.0b1.dev0/thonny/locale/pt_BR/HELP_CONTENT/assistant.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/pt_BR/HELP_CONTENT/birdseye.rst` & `thonny-4.1.0b1.dev0/thonny/locale/pt_BR/HELP_CONTENT/birdseye.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/pt_BR/HELP_CONTENT/debuggers.rst` & `thonny-4.1.0b1.dev0/thonny/locale/pt_BR/HELP_CONTENT/debuggers.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/pt_BR/HELP_CONTENT/debugging.rst` & `thonny-4.1.0b1.dev0/thonny/locale/pt_BR/HELP_CONTENT/debugging.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/pt_BR/HELP_CONTENT/dock.rst` & `thonny-4.1.0b1.dev0/thonny/locale/pt_BR/HELP_CONTENT/dock.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/pt_BR/HELP_CONTENT/errors.rst` & `thonny-4.1.0b1.dev0/thonny/locale/pt_BR/HELP_CONTENT/errors.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/pt_BR/HELP_CONTENT/flask.rst` & `thonny-4.1.0b1.dev0/thonny/locale/pt_BR/HELP_CONTENT/flask.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/pt_BR/HELP_CONTENT/index.rst` & `thonny-4.1.0b1.dev0/thonny/locale/pt_BR/HELP_CONTENT/index.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/pt_BR/HELP_CONTENT/modes.rst` & `thonny-4.1.0b1.dev0/thonny/locale/pt_BR/HELP_CONTENT/modes.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/pt_BR/HELP_CONTENT/packages.rst` & `thonny-4.1.0b1.dev0/thonny/locale/pt_BR/HELP_CONTENT/packages.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/pt_BR/HELP_CONTENT/plotter.rst` & `thonny-4.1.0b1.dev0/thonny/locale/pt_BR/HELP_CONTENT/plotter.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/pt_BR/HELP_CONTENT/program_arguments.rst` & `thonny-4.1.0b1.dev0/thonny/locale/pt_BR/HELP_CONTENT/program_arguments.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/pt_BR/HELP_CONTENT/shell.rst` & `thonny-4.1.0b1.dev0/thonny/locale/pt_BR/HELP_CONTENT/shell.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/pt_BR/HELP_CONTENT/turtle.rst` & `thonny-4.1.0b1.dev0/thonny/locale/pt_BR/HELP_CONTENT/turtle.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/pt_BR/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/pt_BR/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/pt_BR/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/pt_BR/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/pt_PT/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/pt_PT/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/pt_PT/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/pt_PT/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/register_updates.py` & `thonny-4.1.0b1.dev0/thonny/locale/register_updates.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/ro_RO/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/ro_RO/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/ro_RO/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/ro_RO/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/ru_RU/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/ru_RU/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/ru_RU/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/ru_RU/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/sk_SK/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/sk_SK/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/sk_SK/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/sk_SK/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/sl_SI/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/sl_SI/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/sl_SI/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/sl_SI/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/sq_AL/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/sq_AL/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/sq_AL/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/sq_AL/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/sv_SE/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/sv_SE/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/sv_SE/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/sv_SE/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/ta_IN/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/ta_IN/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/ta_IN/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/ta_IN/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/th_TH/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/th_TH/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/th_TH/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/th_TH/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/thonny.pot` & `thonny-4.1.0b1.dev0/thonny/locale/thonny.pot`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/tr_TR/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/tr_TR/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/tr_TR/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/tr_TR/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/uk_UA/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/uk_UA/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/uk_UA/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/uk_UA/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/vi_VN/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/vi_VN/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/vi_VN/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/vi_VN/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/zh_CN/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/zh_CN/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/zh_CN/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/zh_CN/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/zh_TW/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/zh_TW/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/locale/zh_TW/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/zh_TW/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/memory.py` & `thonny-4.1.0b1.dev0/thonny/memory.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/misc_utils.py` & `thonny-4.1.0b1.dev0/thonny/misc_utils.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/about.py` & `thonny-4.1.0b1.dev0/thonny/plugins/about.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/assistant_config_page.py` & `thonny-4.1.0b1.dev0/thonny/plugins/assistant_config_page.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/ast_view.py` & `thonny-4.1.0b1.dev0/thonny/plugins/ast_view.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/autocomplete.py` & `thonny-4.1.0b1.dev0/thonny/plugins/autocomplete.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/backend/birdseye_backend.py` & `thonny-4.1.0b1.dev0/thonny/plugins/backend/birdseye_backend.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/backend/dock_user_windows_backend.py` & `thonny-4.1.0b1.dev0/thonny/plugins/backend/dock_user_windows_backend.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/backend/flask_backend.py` & `thonny-4.1.0b1.dev0/thonny/plugins/backend/flask_backend.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/backend/matplotlib_backend.py` & `thonny-4.1.0b1.dev0/thonny/plugins/backend/matplotlib_backend.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/backend/pgzero_backend.py` & `thonny-4.1.0b1.dev0/thonny/plugins/backend/pgzero_backend.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/backend_config_page.py` & `thonny-4.1.0b1.dev0/thonny/plugins/backend_config_page.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/base_syntax_themes.py` & `thonny-4.1.0b1.dev0/thonny/plugins/base_syntax_themes.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/base_ui_themes.py` & `thonny-4.1.0b1.dev0/thonny/plugins/base_ui_themes.py`

 * *Files 2% similar despite different names*

```diff
@@ -377,15 +377,15 @@
         },
         "Heading": {"configure": {"font": "TkHeadingFont", "relief": "raised"}},  # Treeview heading
         "TLabelframe.Label": {"configure": {"foreground": "#0046d5"}},
     }
 
 
 def aqua() -> BasicUiThemeSettings:
-    # https://github.com/tcltk/tk/blob/main/library/ttk/aquaTheme.tcl
+    # https://github.com/tcltk/tk/blob/master/library/ttk/aquaTheme.tcl
     return {
         ".": {
             "configure": {
                 "font": "TkDefaultFont",
                 "background": "systemWindowBody",
                 "foreground": "systemModelessDialogActiveText",
                 "selectbackground": "systemHighlight",
@@ -406,35 +406,15 @@
                 "selectforeground": [
                     ("background", "systemModelessDialogInactiveText"),
                     ("!focus", "systemDialogActiveText"),
                 ],
             },
         },
         "TButton": {"configure": {"anchor": "center", "width": "6"}},
-        # "Toolbutton": {"configure": {"padding": 0}},
-        "Toolbutton": {
-            "configure": {"anchor": "center", "padding": scale(2), "relief": "flat"},
-            "map": {
-                "relief": [
-                    ("disabled", "flat"),
-                    ("selected", "sunken"),
-                    ("pressed", "sunken"),
-                    ("active", "raised"),
-                ],
-                "background": [("disabled", "gray"), ("pressed", "gray"), ("active", "gray")],
-                "lightcolor": [("pressed", "red")],
-                "darkcolor": [("pressed", "red")],
-            },
-            "layout": [
-                (
-                    "Toolbutton.padding",
-                    {"sticky": "nswe", "children": [("Toolbutton.label", {"sticky": "nswe"})]},
-                )
-            ],
-        },
+        "Toolbutton": {"configure": {"padding": 4}},
         "TNotebook": {
             "configure": {"tabmargins": [10, 0], "tabposition": "n", "padding": [18, 8, 18, 17]}
         },
         "TNotebook.Tab": {"configure": {"padding": [12, 3, 12, 2]}},
         "TCombobox": {"configure": {"postoffset": [5, -2, -10, 0]}},
         "Heading": {"configure": {"font": "TkHeadingFont"}},
         "Treeview": {
@@ -598,16 +578,16 @@
         _treeview_settings(),
         _menubutton_settings(),
         # _paned_window_settings(),
         _menu_settings(),
         {
             "TPanedWindow": {"configure": {"background": "systemDialogBackgroundActive"}},
             "TFrame": {"configure": {"background": "systemDialogBackgroundActive"}},
+            "Tab": {"map": {"foreground": [("selected", "white")]}},
             "ViewTab.TLabel": {"configure": {"padding": [scale(5), 0]}},
-            "Tab": {"map": {"foreground": [("selected", "systemSelectedTabTextColor")]}},
             "Active.ViewTab.TLabel": {
                 "configure": {
                     # "font" : "BoldTkDefaultFont",
                     "relief": "sunken",
                     "borderwidth": scale(1),
                 }
             },
```

### Comparing `thonny-4.1.0b1/thonny/plugins/birdseye_frontend.py` & `thonny-4.1.0b1.dev0/thonny/plugins/birdseye_frontend.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/calltip.py` & `thonny-4.1.0b1.dev0/thonny/plugins/calltip.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/cells.py` & `thonny-4.1.0b1.dev0/thonny/plugins/cells.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/circuitpython/cirpy_back.py` & `thonny-4.1.0b1.dev0/thonny/plugins/circuitpython/cirpy_back.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/circuitpython/cirpy_front.py` & `thonny-4.1.0b1.dev0/thonny/plugins/circuitpython/cirpy_front.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/clean_ui_themes.py` & `thonny-4.1.0b1.dev0/thonny/plugins/clean_ui_themes.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/coloring.py` & `thonny-4.1.0b1.dev0/thonny/plugins/coloring.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/commenting_indenting.py` & `thonny-4.1.0b1.dev0/thonny/plugins/commenting_indenting.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/common_editing_commands.py` & `thonny-4.1.0b1.dev0/thonny/plugins/common_editing_commands.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/cpython_backend/cp_back.py` & `thonny-4.1.0b1.dev0/thonny/plugins/cpython_backend/cp_back.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/cpython_backend/cp_launcher.py` & `thonny-4.1.0b1.dev0/thonny/plugins/cpython_backend/cp_launcher.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/cpython_backend/cp_tracers.py` & `thonny-4.1.0b1.dev0/thonny/plugins/cpython_backend/cp_tracers.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/cpython_frontend/__init__.py` & `thonny-4.1.0b1.dev0/thonny/plugins/cpython_frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/cpython_frontend/cp_front.py` & `thonny-4.1.0b1.dev0/thonny/plugins/cpython_frontend/cp_front.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/cpython_frontend/cp_pip_gui.py` & `thonny-4.1.0b1.dev0/thonny/plugins/cpython_frontend/cp_pip_gui.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/cpython_ssh/__init__.py` & `thonny-4.1.0b1.dev0/thonny/plugins/cpython_ssh/__init__.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/cpython_ssh/cps_back.py` & `thonny-4.1.0b1.dev0/thonny/plugins/cpython_ssh/cps_back.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/cpython_ssh/cps_front.py` & `thonny-4.1.0b1.dev0/thonny/plugins/cpython_ssh/cps_front.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/debugger.py` & `thonny-4.1.0b1.dev0/thonny/plugins/debugger.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/dock_user_windows_frontend.py` & `thonny-4.1.0b1.dev0/thonny/plugins/dock_user_windows_frontend.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/editor_config_page.py` & `thonny-4.1.0b1.dev0/thonny/plugins/editor_config_page.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/esp/__init__.py` & `thonny-4.1.0b1.dev0/thonny/plugins/esp/__init__.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/esp/esp32_api_stubs/esp32.pyi` & `thonny-4.1.0b1.dev0/thonny/plugins/esp/esp32_api_stubs/esp32.pyi`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/esp/esp32_api_stubs/mp-1.18-esp32.txt` & `thonny-4.1.0b1.dev0/thonny/plugins/esp/esp32_api_stubs/mp-1.18-esp32.txt`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/esp/esp_back.py` & `thonny-4.1.0b1.dev0/thonny/plugins/esp/esp_back.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/ev3/__init__.py` & `thonny-4.1.0b1.dev0/thonny/plugins/ev3/__init__.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/ev3/ev3_back.py` & `thonny-4.1.0b1.dev0/thonny/plugins/ev3/ev3_back.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/event_logging.py` & `thonny-4.1.0b1.dev0/thonny/plugins/event_logging.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/event_view.py` & `thonny-4.1.0b1.dev0/thonny/plugins/event_view.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/files.py` & `thonny-4.1.0b1.dev0/thonny/plugins/files.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/find_replace.py` & `thonny-4.1.0b1.dev0/thonny/plugins/find_replace.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/general_config_page.py` & `thonny-4.1.0b1.dev0/thonny/plugins/general_config_page.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/goto_definition.py` & `thonny-4.1.0b1.dev0/thonny/plugins/goto_definition.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/heap.py` & `thonny-4.1.0b1.dev0/thonny/plugins/heap.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/help/__init__.py` & `thonny-4.1.0b1.dev0/thonny/plugins/help/__init__.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/help/assistant.rst` & `thonny-4.1.0b1.dev0/thonny/plugins/help/assistant.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/help/birdseye.rst` & `thonny-4.1.0b1.dev0/thonny/plugins/help/birdseye.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/help/debuggers.rst` & `thonny-4.1.0b1.dev0/thonny/plugins/help/debuggers.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/help/debugging.rst` & `thonny-4.1.0b1.dev0/thonny/plugins/help/debugging.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/help/dock.rst` & `thonny-4.1.0b1.dev0/thonny/plugins/help/dock.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/help/errors.rst` & `thonny-4.1.0b1.dev0/thonny/plugins/help/errors.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/help/flask.rst` & `thonny-4.1.0b1.dev0/thonny/plugins/help/flask.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/help/index.rst` & `thonny-4.1.0b1.dev0/thonny/plugins/help/index.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/help/modes.rst` & `thonny-4.1.0b1.dev0/thonny/plugins/help/modes.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/help/packages.rst` & `thonny-4.1.0b1.dev0/thonny/plugins/help/packages.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/help/plotter.rst` & `thonny-4.1.0b1.dev0/thonny/plugins/help/plotter.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/help/program_arguments.rst` & `thonny-4.1.0b1.dev0/thonny/plugins/help/program_arguments.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/help/shell.rst` & `thonny-4.1.0b1.dev0/thonny/plugins/help/shell.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/help/turtle.rst` & `thonny-4.1.0b1.dev0/thonny/plugins/help/turtle.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/highlight_names.py` & `thonny-4.1.0b1.dev0/thonny/plugins/highlight_names.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/locals_marker.py` & `thonny-4.1.0b1.dev0/thonny/plugins/locals_marker.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/microbit/__init__.py` & `thonny-4.1.0b1.dev0/thonny/plugins/microbit/__init__.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/microbit/api_stubs/audio.pyi` & `thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/audio.pyi`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/microbit/api_stubs/math.py` & `thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/math.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/microbit/api_stubs/microbit.pyi` & `thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/microbit.pyi`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/microbit/api_stubs/music.pyi` & `thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/music.pyi`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/microbit/api_stubs/neopixel.pyi` & `thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/neopixel.pyi`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/microbit/api_stubs/os.pyi` & `thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/os.pyi`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/microbit/api_stubs/radio.pyi` & `thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/radio.pyi`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/microbit/api_stubs/random.pyi` & `thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/random.pyi`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/microbit/api_stubs/speech.pyi` & `thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/speech.pyi`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/microbit/api_stubs/sys.pyi` & `thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/sys.pyi`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/microbit/api_stubs/uarray.pyi` & `thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/uarray.pyi`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/microbit/api_stubs/ustruct.pyi` & `thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/ustruct.pyi`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/microbit/api_stubs/utime.pyi` & `thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/utime.pyi`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/microbit/microbit_back.py` & `thonny-4.1.0b1.dev0/thonny/plugins/microbit/microbit_back.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/micropython/__init__.py` & `thonny-4.1.0b1.dev0/thonny/plugins/micropython/__init__.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/micropython/bare_metal_backend.py` & `thonny-4.1.0b1.dev0/thonny/plugins/micropython/bare_metal_backend.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/micropython/base_flashing_dialog.py` & `thonny-4.1.0b1.dev0/thonny/plugins/micropython/base_flashing_dialog.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/micropython/connection.py` & `thonny-4.1.0b1.dev0/thonny/plugins/micropython/connection.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/micropython/esptool_dialog.py` & `thonny-4.1.0b1.dev0/thonny/plugins/micropython/esptool_dialog.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/micropython/mp_back.py` & `thonny-4.1.0b1.dev0/thonny/plugins/micropython/mp_back.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/micropython/mp_front.py` & `thonny-4.1.0b1.dev0/thonny/plugins/micropython/mp_front.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/micropython/os_mp_backend.py` & `thonny-4.1.0b1.dev0/thonny/plugins/micropython/os_mp_backend.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/micropython/pip_gui.py` & `thonny-4.1.0b1.dev0/thonny/plugins/micropython/pip_gui.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/micropython/serial_connection.py` & `thonny-4.1.0b1.dev0/thonny/plugins/micropython/serial_connection.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/micropython/ssh_connection.py` & `thonny-4.1.0b1.dev0/thonny/plugins/micropython/ssh_connection.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/micropython/subprocess_connection.py` & `thonny-4.1.0b1.dev0/thonny/plugins/micropython/subprocess_connection.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/micropython/uf2dialog.py` & `thonny-4.1.0b1.dev0/thonny/plugins/micropython/uf2dialog.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/micropython/webrepl_connection.py` & `thonny-4.1.0b1.dev0/thonny/plugins/micropython/webrepl_connection.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/misc_analyzers.py` & `thonny-4.1.0b1.dev0/thonny/plugins/misc_analyzers.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/mypy/__init__.py` & `thonny-4.1.0b1.dev0/thonny/plugins/mypy/__init__.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/notes.py` & `thonny-4.1.0b1.dev0/thonny/plugins/notes.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/object_inspector.py` & `thonny-4.1.0b1.dev0/thonny/plugins/object_inspector.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/outline.py` & `thonny-4.1.0b1.dev0/thonny/plugins/outline.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/paren_matcher.py` & `thonny-4.1.0b1.dev0/thonny/plugins/paren_matcher.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pgzero_frontend.py` & `thonny-4.1.0b1.dev0/thonny/plugins/pgzero_frontend.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/__init__.py` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/__init__.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_debug-run-cursor.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_debug-run-cursor.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_debug-run-cursor48.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_debug-run-cursor48.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_debug-run.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_debug-run.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_debug-run48.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_debug-run48.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_debug-step-into.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_debug-step-into.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_debug-step-into48.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_debug-step-into48.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_debug-step-out.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_debug-step-out.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_debug-step-out48.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_debug-step-out48.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_debug-step-over.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_debug-step-over.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_debug-step-over48.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_debug-step-over48.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_document-new48.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_document-new48.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_document-open.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_document-open.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_document-open48.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_document-open48.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_document-save.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_document-save.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_document-save48.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_document-save48.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_media-playback-start.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_media-playback-start.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_media-playback-start48.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_media-playback-start48.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_process-stop.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_process-stop.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_process-stop48.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_process-stop48.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_quit.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_quit.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_quit48.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_quit48.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_resume.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_resume.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_resume48.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_resume48.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_window-close-act.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_window-close-act.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_zoom.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_zoom.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/_disabled_zoom48.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_zoom48.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/debug-run-cursor.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/debug-run-cursor.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/debug-run-cursor48.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/debug-run-cursor48.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/debug-run.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/debug-run.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/debug-run48.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/debug-run48.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/debug-step-into.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/debug-step-into.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/debug-step-into48.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/debug-step-into48.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/debug-step-out.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/debug-step-out.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/debug-step-out48.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/debug-step-out48.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/debug-step-over.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/debug-step-over.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/debug-step-over48.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/debug-step-over48.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/document-new48.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/document-new48.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/document-open.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/document-open.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/document-open48.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/document-open48.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/document-save.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/document-save.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/document-save48.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/document-save48.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/media-playback-start.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/media-playback-start.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/media-playback-start48.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/media-playback-start48.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/process-stop.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/process-stop.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/process-stop48.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/process-stop48.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/quit.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/quit.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/quit48.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/quit48.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/resume.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/resume.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/resume48.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/resume48.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/scrollbar-button-down-insens.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/scrollbar-button-down-insens.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/scrollbar-button-down.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/scrollbar-button-down.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/scrollbar-button-left-insens.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/scrollbar-button-left-insens.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/scrollbar-button-left.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/scrollbar-button-left.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/scrollbar-button-right-insens.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/scrollbar-button-right-insens.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/scrollbar-button-right.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/scrollbar-button-right.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/scrollbar-button-up-insens.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/scrollbar-button-up-insens.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/scrollbar-button-up.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/scrollbar-button-up.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/window-close-act.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/window-close-act.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/zoom.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/zoom.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pi/res/zoom48.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/zoom48.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pip_gui.py` & `thonny-4.1.0b1.dev0/thonny/plugins/pip_gui.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/prime_inventor/__init__.py` & `thonny-4.1.0b1.dev0/thonny/plugins/prime_inventor/__init__.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/prime_inventor/api_stubs/hub.pyi` & `thonny-4.1.0b1.dev0/thonny/plugins/prime_inventor/api_stubs/hub.pyi`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/prime_inventor/prime_inventor_back.py` & `thonny-4.1.0b1.dev0/thonny/plugins/prime_inventor/prime_inventor_back.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/printing/__init__.py` & `thonny-4.1.0b1.dev0/thonny/plugins/printing/__init__.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/printing/template.html` & `thonny-4.1.0b1.dev0/thonny/plugins/printing/template.html`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pylint/__init__.py` & `thonny-4.1.0b1.dev0/thonny/plugins/pylint/__init__.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pylint/messages.py` & `thonny-4.1.0b1.dev0/thonny/plugins/pylint/messages.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/pythontutor.py` & `thonny-4.1.0b1.dev0/thonny/plugins/pythontutor.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/remove_old_data_dir.py` & `thonny-4.1.0b1.dev0/thonny/plugins/remove_old_data_dir.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/replayer.py` & `thonny-4.1.0b1.dev0/thonny/plugins/replayer.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/rp2040/__init__.py` & `thonny-4.1.0b1.dev0/thonny/plugins/rp2040/__init__.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/rp2040/api_stubs/rp2.pyi` & `thonny-4.1.0b1.dev0/thonny/plugins/rp2040/api_stubs/rp2.pyi`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/rp2040/rp2040_back.py` & `thonny-4.1.0b1.dev0/thonny/plugins/rp2040/rp2040_back.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/rpi_pico/__init__.py` & `thonny-4.1.0b1.dev0/thonny/plugins/rpi_pico/__init__.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/run_debug_config_page.py` & `thonny-4.1.0b1.dev0/thonny/plugins/run_debug_config_page.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/shell_config_page.py` & `thonny-4.1.0b1.dev0/thonny/plugins/shell_config_page.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/shell_macro.py` & `thonny-4.1.0b1.dev0/thonny/plugins/shell_macro.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/statement_boxes.py` & `thonny-4.1.0b1.dev0/thonny/plugins/statement_boxes.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/stdlib_error_helpers.py` & `thonny-4.1.0b1.dev0/thonny/plugins/stdlib_error_helpers.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/system_shell/__init__.py` & `thonny-4.1.0b1.dev0/thonny/plugins/system_shell/__init__.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/system_shell/explain_environment.py` & `thonny-4.1.0b1.dev0/thonny/plugins/system_shell/explain_environment.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/terminal_config_page.py` & `thonny-4.1.0b1.dev0/thonny/plugins/terminal_config_page.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/theme_and_font_config_page.py` & `thonny-4.1.0b1.dev0/thonny/plugins/theme_and_font_config_page.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/thonny_folders.py` & `thonny-4.1.0b1.dev0/thonny/plugins/thonny_folders.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/todo_view.py` & `thonny-4.1.0b1.dev0/thonny/plugins/todo_view.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/tomorrow_syntax_theme.py` & `thonny-4.1.0b1.dev0/thonny/plugins/tomorrow_syntax_theme.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/plugins/variables.py` & `thonny-4.1.0b1.dev0/thonny/plugins/variables.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/16x16-blank.gif` & `thonny-4.1.0b1.dev0/thonny/res/16x16-blank.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/1x1-white.gif` & `thonny-4.1.0b1.dev0/thonny/res/1x1-white.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/Ukraine_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/Ukraine_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/_create_disabled_variants.py` & `thonny-4.1.0b1.dev0/thonny/res/_create_disabled_variants.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/_disabled_16x16-blank.gif` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_16x16-blank.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/_disabled_1x1-white.gif` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_1x1-white.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/_disabled_arrow-down.gif` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_arrow-down.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/_disabled_birdseye.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_birdseye.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/_disabled_broken.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_broken.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/_disabled_closed-folder.gif` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_closed-folder.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/_disabled_debug-current-script.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_debug-current-script.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/_disabled_debug-current-script_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_debug-current-script_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/_disabled_delete.gif` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_delete.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/_disabled_folder.gif` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_folder.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/_disabled_generic-file.gif` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_generic-file.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/_disabled_hard-drive.gif` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_hard-drive.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/_disabled_harddisk.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_harddisk.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/_disabled_harddisk_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_harddisk_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/_disabled_help.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_help.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/_disabled_help_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_help_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/_disabled_information.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_information.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/_disabled_information_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_information_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/_disabled_nav-backward_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_nav-backward_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/_disabled_nav-forward_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_nav-forward_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/_disabled_new-file_Linux_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_new-file_Linux_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/_disabled_open-file_Linux_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_open-file_Linux_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/_disabled_open_folder.gif` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_open_folder.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/_disabled_outline-class.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_outline-class.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/_disabled_outline-class_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_outline-class_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/_disabled_outline-method.gif` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_outline-method.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/_disabled_python-file.gif` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_python-file.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/_disabled_python-icon.gif` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_python-icon.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/_disabled_quit_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_quit_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/_disabled_resume_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_resume_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/_disabled_run-current-script.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_run-current-script.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/_disabled_run-current-script_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_run-current-script_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/_disabled_run-to-cursor_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_run-to-cursor_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/_disabled_save-file_2x_alt.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_save-file_2x_alt.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/_disabled_save-file_Linux.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_save-file_Linux.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/_disabled_save-file_Linux_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_save-file_Linux_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/_disabled_save-file_alt.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_save-file_alt.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/_disabled_star.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_star.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/_disabled_star_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_star_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/_disabled_step-into_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_step-into_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/_disabled_step-out_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_step-out_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/_disabled_step-over.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_step-over.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/_disabled_step-over_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_step-over_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/_disabled_stop.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_stop.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/_disabled_stop_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_stop_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/_disabled_tab-close-active-clam-dark.gif` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_tab-close-active-clam-dark.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/_disabled_tab-close-active-clam.gif` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_tab-close-active-clam.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/_disabled_tab-close-active.gif` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_tab-close-active.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/_disabled_tab-close-clam.gif` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_tab-close-clam.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/_disabled_tab-close.gif` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_tab-close.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/_disabled_terminal_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_terminal_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/_disabled_text-file.gif` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_text-file.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/_disabled_thonny.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_thonny.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/arrow-down.gif` & `thonny-4.1.0b1.dev0/thonny/res/arrow-down.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/birdseye.png` & `thonny-4.1.0b1.dev0/thonny/res/birdseye.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/boxminus_light.png` & `thonny-4.1.0b1.dev0/thonny/res/boxminus_light.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/boxplus_light.png` & `thonny-4.1.0b1.dev0/thonny/res/boxplus_light.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/broken.png` & `thonny-4.1.0b1.dev0/thonny/res/broken.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/closed-folder.gif` & `thonny-4.1.0b1.dev0/thonny/res/closed-folder.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/debug-current-script.png` & `thonny-4.1.0b1.dev0/thonny/res/debug-current-script.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/debug-current-script_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/debug-current-script_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/delete.gif` & `thonny-4.1.0b1.dev0/thonny/res/delete.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/hard-drive.gif` & `thonny-4.1.0b1.dev0/thonny/res/hard-drive.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/harddisk.png` & `thonny-4.1.0b1.dev0/thonny/res/harddisk.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/harddisk_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/harddisk_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/help.png` & `thonny-4.1.0b1.dev0/thonny/res/help.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/help_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/help_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/information.png` & `thonny-4.1.0b1.dev0/thonny/res/information.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/information_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/information_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/nav-backward_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/nav-backward_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/nav-forward_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/nav-forward_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/new-file_Linux_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/new-file_Linux_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/open-file.png` & `thonny-4.1.0b1.dev0/thonny/res/open-file.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/open-file_Linux.png` & `thonny-4.1.0b1.dev0/thonny/res/open-file_Linux.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/open-file_Linux_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/open-file_Linux_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/open_folder.gif` & `thonny-4.1.0b1.dev0/thonny/res/open_folder.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/outline-class.png` & `thonny-4.1.0b1.dev0/thonny/res/outline-class.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/outline-class_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/outline-class_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/outline-method.gif` & `thonny-4.1.0b1.dev0/thonny/res/outline-method.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/python-file.gif` & `thonny-4.1.0b1.dev0/thonny/res/python-file.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/python-icon.gif` & `thonny-4.1.0b1.dev0/thonny/res/python-icon.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/python-icon_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/python-icon_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/quit.png` & `thonny-4.1.0b1.dev0/thonny/res/quit.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/quit_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/quit_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/resume.png` & `thonny-4.1.0b1.dev0/thonny/res/resume.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/resume_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/resume_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/run-current-script.png` & `thonny-4.1.0b1.dev0/thonny/res/run-current-script.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/run-current-script_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/run-current-script_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/save-file.png` & `thonny-4.1.0b1.dev0/thonny/res/save-file.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/save-file_2x_alt.png` & `thonny-4.1.0b1.dev0/thonny/res/save-file_2x_alt.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/save-file_Linux.png` & `thonny-4.1.0b1.dev0/thonny/res/save-file_Linux.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/save-file_Linux_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/save-file_Linux_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/save-file_alt.png` & `thonny-4.1.0b1.dev0/thonny/res/save-file_alt.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/star.png` & `thonny-4.1.0b1.dev0/thonny/res/star.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/star_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/star_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/step-into_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/step-into_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/step-out_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/step-out_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/step-over_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/step-over_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/stop.png` & `thonny-4.1.0b1.dev0/thonny/res/stop.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/stop_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/stop_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/tab-close-clam.gif` & `thonny-4.1.0b1.dev0/thonny/res/tab-close-clam.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/tab-close.gif` & `thonny-4.1.0b1.dev0/thonny/res/tab-close.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/terminal.png` & `thonny-4.1.0b1.dev0/thonny/res/terminal.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/terminal_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/terminal_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/text-file.gif` & `thonny-4.1.0b1.dev0/thonny/res/text-file.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/thonny.ico` & `thonny-4.1.0b1.dev0/thonny/res/thonny.ico`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/thonny.png` & `thonny-4.1.0b1.dev0/thonny/res/thonny.png`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/res/thonny_small.ico` & `thonny-4.1.0b1.dev0/thonny/res/thonny_small.ico`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/roughparse.py` & `thonny-4.1.0b1.dev0/thonny/roughparse.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/rst_utils.py` & `thonny-4.1.0b1.dev0/thonny/rst_utils.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/running.py` & `thonny-4.1.0b1.dev0/thonny/running.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/shell.py` & `thonny-4.1.0b1.dev0/thonny/shell.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/terminal.py` & `thonny-4.1.0b1.dev0/thonny/terminal.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/test/plugins/test_locals_marker.py` & `thonny-4.1.0b1.dev0/thonny/test/plugins/test_locals_marker.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/test/plugins/test_name_highlighter.py` & `thonny-4.1.0b1.dev0/thonny/test/plugins/test_name_highlighter.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/test/test_common.py` & `thonny-4.1.0b1.dev0/thonny/test/test_common.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/tktextext.py` & `thonny-4.1.0b1.dev0/thonny/tktextext.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/token_utils.py` & `thonny-4.1.0b1.dev0/thonny/token_utils.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/udisks.py` & `thonny-4.1.0b1.dev0/thonny/udisks.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/ui_utils.py` & `thonny-4.1.0b1.dev0/thonny/ui_utils.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/vendored_libs/filelock/__init__.py` & `thonny-4.1.0b1.dev0/thonny/vendored_libs/filelock/__init__.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/vendored_libs/filelock/_api.py` & `thonny-4.1.0b1.dev0/thonny/vendored_libs/filelock/_api.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/vendored_libs/filelock/_soft.py` & `thonny-4.1.0b1.dev0/thonny/vendored_libs/filelock/_soft.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/vendored_libs/filelock/_unix.py` & `thonny-4.1.0b1.dev0/thonny/vendored_libs/filelock/_unix.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/vendored_libs/filelock/_util.py` & `thonny-4.1.0b1.dev0/thonny/vendored_libs/filelock/_util.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/vendored_libs/filelock/_windows.py` & `thonny-4.1.0b1.dev0/thonny/vendored_libs/filelock/_windows.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/vendored_libs/pipkin/__init__.py` & `thonny-4.1.0b1.dev0/thonny/vendored_libs/pipkin/__init__.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/vendored_libs/pipkin/__main__.py` & `thonny-4.1.0b1.dev0/thonny/vendored_libs/pipkin/__main__.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/vendored_libs/pipkin/adapters.py` & `thonny-4.1.0b1.dev0/thonny/vendored_libs/pipkin/adapters.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/vendored_libs/pipkin/bare_metal.py` & `thonny-4.1.0b1.dev0/thonny/vendored_libs/pipkin/bare_metal.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/vendored_libs/pipkin/connection.py` & `thonny-4.1.0b1.dev0/thonny/vendored_libs/pipkin/connection.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/vendored_libs/pipkin/parser.py` & `thonny-4.1.0b1.dev0/thonny/vendored_libs/pipkin/parser.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/vendored_libs/pipkin/proxy.py` & `thonny-4.1.0b1.dev0/thonny/vendored_libs/pipkin/proxy.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/vendored_libs/pipkin/serial_connection.py` & `thonny-4.1.0b1.dev0/thonny/vendored_libs/pipkin/serial_connection.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/vendored_libs/pipkin/session.py` & `thonny-4.1.0b1.dev0/thonny/vendored_libs/pipkin/session.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/vendored_libs/pipkin/util.py` & `thonny-4.1.0b1.dev0/thonny/vendored_libs/pipkin/util.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/vendored_libs/pipkin/webrepl_connection.py` & `thonny-4.1.0b1.dev0/thonny/vendored_libs/pipkin/webrepl_connection.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/workbench.py` & `thonny-4.1.0b1.dev0/thonny/workbench.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny/workdlg.py` & `thonny-4.1.0b1.dev0/thonny/workdlg.py`

 * *Files identical despite different names*

### Comparing `thonny-4.1.0b1/thonny.egg-info/PKG-INFO` & `thonny-4.1.0b1.dev0/thonny.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thonny
-Version: 4.1.0b1
+Version: 4.1.0b1.dev0
 Summary: Python IDE for beginners
 Home-page: https://thonny.org
 Author: Aivar Annamaa and others
 Author-email: thonny@googlegroups.com
 License: MIT
 Project-URL: Source code, https://github.com/thonny/thonny
 Project-URL: Bug tracker, https://github.com/thonny/thonny/issues
@@ -38,7 +38,8 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Debuggers
 Classifier: Topic :: Text Editors
 Requires-Python: >=3.8
 License-File: LICENSE.txt
 
 Thonny is a simple Python IDE with features useful for learning programming. See https://thonny.org for more info.
+
```

### Comparing `thonny-4.1.0b1/thonny.egg-info/SOURCES.txt` & `thonny-4.1.0b1.dev0/thonny.egg-info/SOURCES.txt`

 * *Files identical despite different names*

