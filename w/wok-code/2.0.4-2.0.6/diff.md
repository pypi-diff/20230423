# Comparing `tmp/wok_code-2.0.4.tar.gz` & `tmp/wok_code-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wok_code-2.0.4.tar", last modified: Fri Jan 13 17:54:10 2023, max compression
+gzip compressed data, was "wok_code-2.0.6.tar", last modified: Sun Apr 23 14:00:37 2023, max compression
```

## Comparing `wok_code-2.0.4.tar` & `wok_code-2.0.6.tar`

### file list

```diff
@@ -1,61 +1,72 @@
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-01-13 17:54:10.000000 wok_code-2.0.4/
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-01-13 17:54:10.000000 wok_code-2.0.4/wok_code.egg-info/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        9 2023-01-13 17:54:09.000000 wok_code-2.0.4/wok_code.egg-info/top_level.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-01-13 17:54:09.000000 wok_code-2.0.4/wok_code.egg-info/dependency_links.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2022-12-09 06:35:40.000000 wok_code-2.0.4/wok_code.egg-info/not-zip-safe
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      782 2023-01-13 17:54:09.000000 wok_code-2.0.4/wok_code.egg-info/entry_points.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1528 2023-01-13 17:54:09.000000 wok_code-2.0.4/wok_code.egg-info/SOURCES.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       64 2023-01-13 17:54:09.000000 wok_code-2.0.4/wok_code.egg-info/requires.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1730 2023-01-13 17:54:09.000000 wok_code-2.0.4/wok_code.egg-info/PKG-INFO
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       38 2023-01-13 17:54:10.000000 wok_code-2.0.4/setup.cfg
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-01-13 17:54:10.000000 wok_code-2.0.4/wok_code/
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      164 2022-12-09 05:08:44.000000 wok_code-2.0.4/wok_code/__main__.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     3017 2023-01-12 05:57:23.000000 wok_code-2.0.4/wok_code/do_gitignore.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     7186 2023-01-09 05:27:54.000000 wok_code-2.0.4/wok_code/gen_addons_table.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      205 2022-12-09 05:08:44.000000 wok_code-2.0.4/wok_code/rm_dir_with_space.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-01-13 17:54:10.000000 wok_code-2.0.4/wok_code/tests/
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     6539 2023-01-09 05:27:54.000000 wok_code-2.0.4/wok_code/tests/test_gen_readme.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     4951 2023-01-09 05:27:54.000000 wok_code-2.0.4/wok_code/tests/devel_tools_test_01.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1063 2023-01-09 05:27:54.000000 wok_code-2.0.4/wok_code/tests/wok_code_test_02.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     9775 2022-12-09 05:08:44.000000 wok_code-2.0.4/wok_code/tests/__license_mgnt.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     2028 2022-12-09 05:08:44.000000 wok_code-2.0.4/wok_code/tests/test_filepo.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       24 2022-12-09 05:08:44.000000 wok_code-2.0.4/wok_code/tests/__init__.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     7257 2023-01-09 05:27:54.000000 wok_code-2.0.4/wok_code/ssh.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     8380 2023-01-09 05:27:54.000000 wok_code-2.0.4/wok_code/pypi.sh
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     6744 2023-01-09 05:27:54.000000 wok_code-2.0.4/wok_code/cvt_csv_2_xml.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-01-13 17:54:10.000000 wok_code-2.0.4/wok_code/scripts/
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    75091 2023-01-10 12:50:37.000000 wok_code-2.0.4/wok_code/scripts/please.sh
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    71159 2023-01-09 05:27:54.000000 wok_code-2.0.4/wok_code/scripts/to_pep8.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     3577 2023-01-13 05:39:07.000000 wok_code-2.0.4/wok_code/scripts/setup.info
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     6457 2023-01-09 05:27:54.000000 wok_code-2.0.4/wok_code/scripts/main.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     4990 2023-01-09 05:27:54.000000 wok_code-2.0.4/wok_code/scripts/makepo_it.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    21516 2023-01-09 05:27:54.000000 wok_code-2.0.4/wok_code/scripts/cvt_csv_coa.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    17906 2023-01-09 05:27:54.000000 wok_code-2.0.4/wok_code/scripts/dist_pkg.sh
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1225 2023-01-09 05:27:54.000000 wok_code-2.0.4/wok_code/scripts/generate_random_codes.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    30241 2023-01-09 05:27:54.000000 wok_code-2.0.4/wok_code/scripts/wget_odoo_repositories.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      992 2022-12-09 05:08:44.000000 wok_code-2.0.4/wok_code/scripts/dist_pkg.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     6576 2023-01-09 05:27:54.000000 wok_code-2.0.4/wok_code/scripts/do_migrate.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    25546 2023-01-09 05:27:54.000000 wok_code-2.0.4/wok_code/scripts/odoo_translation_old.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    83147 2023-01-09 05:27:54.000000 wok_code-2.0.4/wok_code/scripts/gen_readme.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    10098 2023-01-09 05:27:54.000000 wok_code-2.0.4/wok_code/scripts/lint_2_compare.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    36336 2023-01-09 05:27:54.000000 wok_code-2.0.4/wok_code/scripts/deploy_odoo.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    40023 2023-01-13 05:00:37.000000 wok_code-2.0.4/wok_code/scripts/odoo_translation.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    31823 2023-01-09 05:27:54.000000 wok_code-2.0.4/wok_code/scripts/odoo_dependencies.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    10070 2022-12-09 05:08:44.000000 wok_code-2.0.4/wok_code/scripts/license_mgnt.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     5357 2023-01-09 05:27:54.000000 wok_code-2.0.4/wok_code/scripts/cvt_csv_2_rst.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     2875 2023-01-09 05:27:54.000000 wok_code-2.0.4/wok_code/scripts/please.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     6171 2023-01-09 05:27:54.000000 wok_code-2.0.4/wok_code/scripts/do_odoo_site.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      522 2022-12-09 05:08:44.000000 wok_code-2.0.4/wok_code/scripts/__init__.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     2176 2022-12-09 05:08:44.000000 wok_code-2.0.4/wok_code/eval_gtin.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    32295 2023-01-09 05:27:54.000000 wok_code-2.0.4/wok_code/topep8
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1150 2022-12-09 05:08:44.000000 wok_code-2.0.4/wok_code/cvt_script.man
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1672 2022-12-09 05:08:44.000000 wok_code-2.0.4/wok_code/to_oca.2p8
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2646 2022-12-09 05:08:44.000000 wok_code-2.0.4/wok_code/do_set_utf8.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     6849 2022-12-09 05:08:44.000000 wok_code-2.0.4/wok_code/please.man
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     2667 2022-12-09 05:08:44.000000 wok_code-2.0.4/wok_code/to_zero.2p8
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     5228 2022-12-09 05:08:44.000000 wok_code-2.0.4/wok_code/to_pep8.2p8
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       46 2022-12-09 05:08:44.000000 wok_code-2.0.4/wok_code/__init__.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    20983 2023-01-09 05:27:54.000000 wok_code-2.0.4/wok_code/cvt_script
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     3577 2023-01-09 05:27:54.000000 wok_code-2.0.4/setup.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1730 2023-01-13 17:54:10.000000 wok_code-2.0.4/PKG-INFO
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    46523 2023-01-13 17:54:09.000000 wok_code-2.0.4/README.rst
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-23 14:00:37.516086 wok_code-2.0.6/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1607 2023-04-23 14:00:37.516086 wok_code-2.0.6/PKG-INFO
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    47023 2023-04-23 14:00:36.000000 wok_code-2.0.6/README.rst
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       38 2023-04-23 14:00:37.516086 wok_code-2.0.6/setup.cfg
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     3729 2023-04-21 12:32:35.000000 wok_code-2.0.6/setup.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-23 14:00:37.516086 wok_code-2.0.6/wok_code/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       81 2023-01-27 10:18:10.000000 wok_code-2.0.6/wok_code/__init__.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      164 2022-12-09 05:08:44.000000 wok_code-2.0.6/wok_code/__main__.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     6744 2023-03-25 15:14:36.000000 wok_code-2.0.6/wok_code/cvt_csv_2_xml.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    20904 2023-04-15 08:02:21.000000 wok_code-2.0.6/wok_code/cvt_script
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1150 2022-12-09 05:08:44.000000 wok_code-2.0.6/wok_code/cvt_script.man
+-rw-r--r--   0 odoo      (1000) odoo      (1000)    11286 2023-03-25 15:14:36.000000 wok_code-2.0.6/wok_code/do_git_checkout_new_branch.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     3052 2023-02-12 19:40:51.000000 wok_code-2.0.6/wok_code/do_gitignore.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2646 2022-12-09 05:08:44.000000 wok_code-2.0.6/wok_code/do_set_utf8.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     2176 2022-12-09 05:08:44.000000 wok_code-2.0.6/wok_code/eval_gtin.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     7186 2023-03-25 15:14:36.000000 wok_code-2.0.6/wok_code/gen_addons_table.py
+-rwxr-xr-x   0 odoo      (1000) odoo      (1000)     1413 2022-12-13 19:22:06.000000 wok_code-2.0.6/wok_code/install_python_3_from_source.sh
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     3082 2023-04-23 10:48:07.000000 wok_code-2.0.6/wok_code/pgconf.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     6896 2023-01-21 13:24:11.000000 wok_code-2.0.6/wok_code/please.man
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     8389 2023-03-25 15:14:36.000000 wok_code-2.0.6/wok_code/pypi.sh
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      205 2022-12-09 05:08:44.000000 wok_code-2.0.6/wok_code/rm_dir_with_space.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-23 14:00:37.516086 wok_code-2.0.6/wok_code/scripts/
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      606 2023-04-21 11:43:14.000000 wok_code-2.0.6/wok_code/scripts/__init__.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-23 14:00:37.516086 wok_code-2.0.6/wok_code/scripts/config/
+-rw-r--r--   0 odoo      (1000) odoo      (1000)      373 2023-04-12 10:49:14.000000 wok_code-2.0.6/wok_code/scripts/config/globals.yml
+-rw-r--r--   0 odoo      (1000) odoo      (1000)        0 2023-04-12 07:23:52.000000 wok_code-2.0.6/wok_code/scripts/config/globals_xml.yml
+-rw-r--r--   0 odoo      (1000) odoo      (1000)      893 2023-04-12 07:02:48.000000 wok_code-2.0.6/wok_code/scripts/config/to_new_api.yml
+-rw-r--r--   0 odoo      (1000) odoo      (1000)      224 2023-04-12 07:55:02.000000 wok_code-2.0.6/wok_code/scripts/config/to_odoo_py2.yml
+-rw-r--r--   0 odoo      (1000) odoo      (1000)      173 2023-04-12 07:50:10.000000 wok_code-2.0.6/wok_code/scripts/config/to_odoo_py3.yml
+-rw-r--r--   0 odoo      (1000) odoo      (1000)      698 2023-04-12 06:43:18.000000 wok_code-2.0.6/wok_code/scripts/config/to_old_api.yml
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     5357 2023-03-25 15:14:36.000000 wok_code-2.0.6/wok_code/scripts/cvt_csv_2_rst.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    21516 2023-03-25 15:14:36.000000 wok_code-2.0.6/wok_code/scripts/cvt_csv_coa.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    40728 2023-04-14 14:10:51.000000 wok_code-2.0.6/wok_code/scripts/deploy_odoo.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      992 2022-12-09 05:08:44.000000 wok_code-2.0.6/wok_code/scripts/dist_pkg.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    17827 2023-04-15 08:02:21.000000 wok_code-2.0.6/wok_code/scripts/dist_pkg.sh
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    26398 2023-04-17 21:30:54.000000 wok_code-2.0.6/wok_code/scripts/do_migrate.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     5937 2023-04-14 14:07:01.000000 wok_code-2.0.6/wok_code/scripts/do_odoo_site.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    83221 2023-04-03 11:40:32.000000 wok_code-2.0.6/wok_code/scripts/gen_readme.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1225 2023-03-25 15:14:36.000000 wok_code-2.0.6/wok_code/scripts/generate_random_codes.py
+-rw-r--r--   0 odoo      (1000) odoo      (1000)    10070 2023-01-27 08:05:01.000000 wok_code-2.0.6/wok_code/scripts/license_mgnt.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    10100 2023-03-25 15:14:36.000000 wok_code-2.0.6/wok_code/scripts/lint_2_compare.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     6457 2023-03-25 15:14:36.000000 wok_code-2.0.6/wok_code/scripts/main.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     4990 2023-03-25 15:14:36.000000 wok_code-2.0.6/wok_code/scripts/makepo_it.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    31823 2023-03-25 15:14:36.000000 wok_code-2.0.6/wok_code/scripts/odoo_dependencies.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    40102 2023-03-25 15:14:36.000000 wok_code-2.0.6/wok_code/scripts/odoo_translation.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    25546 2023-04-14 14:07:09.000000 wok_code-2.0.6/wok_code/scripts/odoo_translation_old.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    22434 2023-04-14 14:07:18.000000 wok_code-2.0.6/wok_code/scripts/please.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    63670 2023-04-15 08:02:21.000000 wok_code-2.0.6/wok_code/scripts/please.sh
+-rw-r--r--   0 odoo      (1000) odoo      (1000)     7066 2023-04-14 14:09:03.000000 wok_code-2.0.6/wok_code/scripts/please_apache.py
+-rw-r--r--   0 odoo      (1000) odoo      (1000)     5550 2023-03-25 15:14:36.000000 wok_code-2.0.6/wok_code/scripts/please_z0bug.py
+-rw-r--r--   0 odoo      (1000) odoo      (1000)      992 2022-12-09 05:08:44.000000 wok_code-2.0.6/wok_code/scripts/run_odoo_debug.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     3729 2023-04-23 13:50:03.000000 wok_code-2.0.6/wok_code/scripts/setup.info
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    71159 2023-03-25 15:14:36.000000 wok_code-2.0.6/wok_code/scripts/to_pep8.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    30263 2023-04-02 15:30:34.000000 wok_code-2.0.6/wok_code/scripts/wget_odoo_repositories.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     7804 2023-03-25 15:14:36.000000 wok_code-2.0.6/wok_code/ssh.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-23 14:00:37.516086 wok_code-2.0.6/wok_code/tests/
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     2028 2022-12-09 05:08:44.000000 wok_code-2.0.6/wok_code/tests/test_filepo.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     6539 2023-03-25 15:14:36.000000 wok_code-2.0.6/wok_code/tests/test_gen_readme.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     4939 2023-03-25 15:14:36.000000 wok_code-2.0.6/wok_code/tests/test_license_mgnt.py
+-rw-r--r--   0 odoo      (1000) odoo      (1000)     2229 2023-04-14 14:09:46.000000 wok_code-2.0.6/wok_code/tests/test_please.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1672 2022-12-09 05:08:44.000000 wok_code-2.0.6/wok_code/to_oca.2p8
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     5228 2022-12-09 05:08:44.000000 wok_code-2.0.6/wok_code/to_pep8.2p8
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     2667 2022-12-09 05:08:44.000000 wok_code-2.0.6/wok_code/to_zero.2p8
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    32228 2023-04-15 08:02:21.000000 wok_code-2.0.6/wok_code/topep8
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-23 14:00:37.516086 wok_code-2.0.6/wok_code.egg-info/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1607 2023-04-23 14:00:37.000000 wok_code-2.0.6/wok_code.egg-info/PKG-INFO
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1896 2023-04-23 14:00:37.000000 wok_code-2.0.6/wok_code.egg-info/SOURCES.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-04-23 14:00:37.000000 wok_code-2.0.6/wok_code.egg-info/dependency_links.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      838 2023-04-23 14:00:37.000000 wok_code-2.0.6/wok_code.egg-info/entry_points.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2022-12-09 06:35:40.000000 wok_code-2.0.6/wok_code.egg-info/not-zip-safe
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       68 2023-04-23 14:00:37.000000 wok_code-2.0.6/wok_code.egg-info/requires.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        9 2023-04-23 14:00:37.000000 wok_code-2.0.6/wok_code.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `wok_code-2.0.4/wok_code.egg-info/entry_points.txt` & `wok_code-2.0.6/wok_code.egg-info/entry_points.txt`

 * *Files 22% similar despite different names*

```diff
@@ -7,11 +7,12 @@
 do_odoo_site.py = wok_code.scripts.do_odoo_site:main
 gen_readme.py = wok_code.scripts.gen_readme:main
 lint_2_compare = wok_code.scripts.lint_2_compare:main
 makepo_it.py = wok_code.scripts.makepo_it:main
 odoo_dependencies.py = wok_code.scripts.odoo_dependencies:main
 odoo_translation.py = wok_code.scripts.odoo_translation:main
 please = wok_code.scripts.please:main
+run_odoo_debug = odoo_score.scripts.run_odoo_debug:main
 to_pep8.py = wok_code.scripts.to_pep8:main
 wget_odoo_repositories.py = wok_code.scripts.wget_odoo_repositories:main
 wok_code-info = wok_code.scripts.main:main
```

### Comparing `wok_code-2.0.4/wok_code.egg-info/SOURCES.txt` & `wok_code-2.0.6/wok_code.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 README.rst
 setup.py
 wok_code/__init__.py
 wok_code/__main__.py
 wok_code/cvt_csv_2_xml.py
 wok_code/cvt_script
 wok_code/cvt_script.man
+wok_code/do_git_checkout_new_branch.py
 wok_code/do_gitignore.py
 wok_code/do_set_utf8.py
 wok_code/eval_gtin.py
 wok_code/gen_addons_table.py
+wok_code/install_python_3_from_source.sh
+wok_code/pgconf.py
 wok_code/please.man
 wok_code/pypi.sh
 wok_code/rm_dir_with_space.py
 wok_code/ssh.py
 wok_code/to_oca.2p8
 wok_code/to_pep8.2p8
 wok_code/to_zero.2p8
@@ -39,16 +42,23 @@
 wok_code/scripts/main.py
 wok_code/scripts/makepo_it.py
 wok_code/scripts/odoo_dependencies.py
 wok_code/scripts/odoo_translation.py
 wok_code/scripts/odoo_translation_old.py
 wok_code/scripts/please.py
 wok_code/scripts/please.sh
+wok_code/scripts/please_apache.py
+wok_code/scripts/please_z0bug.py
+wok_code/scripts/run_odoo_debug.py
 wok_code/scripts/setup.info
 wok_code/scripts/to_pep8.py
 wok_code/scripts/wget_odoo_repositories.py
-wok_code/tests/__init__.py
-wok_code/tests/__license_mgnt.py
-wok_code/tests/devel_tools_test_01.py
+wok_code/scripts/config/globals.yml
+wok_code/scripts/config/globals_xml.yml
+wok_code/scripts/config/to_new_api.yml
+wok_code/scripts/config/to_odoo_py2.yml
+wok_code/scripts/config/to_odoo_py3.yml
+wok_code/scripts/config/to_old_api.yml
 wok_code/tests/test_filepo.py
 wok_code/tests/test_gen_readme.py
-wok_code/tests/wok_code_test_02.py
+wok_code/tests/test_license_mgnt.py
+wok_code/tests/test_please.py
```

### Comparing `wok_code-2.0.4/wok_code.egg-info/PKG-INFO` & `wok_code-2.0.6/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,41 @@
-Metadata-Version: 1.2
-Name: wok-code
-Version: 2.0.4
+Metadata-Version: 2.1
+Name: wok_code
+Version: 2.0.6
 Summary: Python developers tools
 Home-page: https://zeroincombenze-tools.readthedocs.io
 Author: Antonio Maria Vigliotti
 Author-email: antoniomaria.vigliotti@gmail.com
 License: Affero GPL
-Project-URL: Source, https://github.com/zeroincombenze/tools
 Project-URL: Documentation, https://zeroincombenze-tools.readthedocs.io
-Description: 
-        Various tools at your fingertips.
-        
-        The available tools are:
-        
-        * cvt_csv_2_rst.py: convert csv file into rst file
-        * cvt_csv_2_xml.py: convert csv file into xml file
-        * cvt_script: parse bash script and convert to meet company standard
-        * gen_readme.py: generate documentation files, mainly README.rst
-        * odoo_dependency.py: show odoo dependencies and/or Odoo module tree
-        * odoo_translation.py: manage Odoo translation
-        * pep8: parse source .py file to meet pep8 and convert across Odoo versions
-        * please: developer shell
-        * wget_odoo_repositories.py: get repository names from github.com
-        
+Project-URL: Source, https://github.com/zeroincombenze/tools
 Keywords: linux travis development
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
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Operating System :: OS Independent
+
+
+Various tools at your fingertips.
+
+The available tools are:
+
+* cvt_csv_2_rst.py: convert csv file into rst file
+* cvt_csv_2_xml.py: convert csv file into xml file
+* cvt_script: parse bash script and convert to meet company standard
+* gen_readme.py: generate documentation files, mainly README.rst
+* odoo_dependency.py: show odoo dependencies and/or Odoo module tree
+* odoo_translation.py: manage Odoo translation
+* pep8: parse source .py file to meet pep8 and convert across Odoo versions
+* please: developer shell
+* wget_odoo_repositories.py: get repository names from github.com
+
+
```

### Comparing `wok_code-2.0.4/wok_code/do_gitignore.py` & `wok_code-2.0.6/wok_code/do_gitignore.py`

 * *Files 8% similar despite different names*

```diff
@@ -71,15 +71,16 @@
         submodules = []
         for fn in os.listdir(path):
             if fn in (
                 'addons_kalamitica',
                 'coverage',
                 'generic',
                 'nardo_modules',
-                'venv_odoo'
+                'venv_odoo',
+                'website-themes',
             ):
                 submodules.append('/%s' % fn)
                 continue
             ffn = os.path.join(path, fn)
             if os.path.isdir(os.path.join(ffn, '.git')):
                 submodules.append('/%s' % fn)
         return do_create_gitignore(path, submodules)
```

### Comparing `wok_code-2.0.4/wok_code/gen_addons_table.py` & `wok_code-2.0.6/wok_code/gen_addons_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from past.builtins import cmp
 
 standard_library.install_aliases()  # noqa: E402
 
 
 MARKERS = r'(\[//\]: # \(addons\))|(\[//\]: # \(end addons\))'
 MANIFESTS = ('__openerp__.py', '__manifest__.py')
-__version__ = "2.0.4"
+__version__ = "2.0.6"
 
 
 class UserError(Exception):
     def __init__(self, msg):
         self.msg = msg
```

### Comparing `wok_code-2.0.4/wok_code/tests/test_gen_readme.py` & `wok_code-2.0.6/wok_code/tests/test_gen_readme.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import os
 import sys
 
 from python_plus import _c
 from z0lib import z0lib
 from zerobug import z0test, z0testodoo
 
-__version__ = "2.0.4"
+__version__ = "2.0.6"
 
 MODULE_ID = 'z0bug_odoo'
 TEST_FAILED = 1
 TEST_SUCCESS = 0
 ODOO_VERSIONS = ('7.0', '10.0', '12.0')
 
 DESCR_FN = r"""Lorem ipsum
```

### Comparing `wok_code-2.0.4/wok_code/tests/devel_tools_test_01.py` & `wok_code-2.0.6/wok_code/tests/test_license_mgnt.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (C) 2015-2023 SHS-AV s.r.l. (<http://www.zeroincombenze.org>)
 # License AGPL-3.0 or later (http://www.gnu.org/licenses/agpl).
 """
     Devel Tools unit test library for python programs Regression Test Suite
 """
-
-# import pdb
 import os
 import sys
 
-from wok_code import license_mgnt
+from wok_code.scripts import license_mgnt
 from zerobug import z0test, z0testodoo
 
-__version__ = "2.0.4"
+__version__ = "2.0.6"
 
 MODULE_ID = 'devel_tool'
 TEST_FAILED = 1
 TEST_SUCCESS = 0
 
 
 def version():
@@ -43,40 +41,40 @@
 
 class RegressionTest:
     def __init__(self, z0bug):
         self.Z = z0bug
 
     def create_file_author_1(self, path):
         fn = os.path.join(path, 'authors.txt')
-        with open(fn, 'wb') as fd:
+        with open(fn, 'w') as fd:
             fd.write("""* Powerp <http://www.powerp.it/>""")
 
     def create_file_contributor_1(self, path):
         fn = os.path.join(path, 'contributors.txt')
-        with open(fn, 'wb') as fd:
+        with open(fn, 'w') as fd:
             fd.write("""* <antonio.vigliotti@libero.it>""")
 
     def create_file_manifest_1(self, path):
         fn = os.path.join(path, '__manifest__.py')
-        with open(fn, 'wb') as fd:
+        with open(fn, 'w') as fd:
             fd.write(MANIFEST_1)
 
     def create_file_author_2(self, path):
         fn = os.path.join(path, 'authors.txt')
-        with open(fn, 'wb') as fd:
+        with open(fn, 'w') as fd:
             fd.write(AUTHOR_2)
 
     def create_file_contributor_2(self, path):
         fn = os.path.join(path, 'contributors.txt')
-        with open(fn, 'wb') as fd:
+        with open(fn, 'w') as fd:
             fd.write(CONTRIBUTORS_2)
 
     def create_file_manifest_2(self, path):
         fn = os.path.join(path, '__manifest__.py')
-        with open(fn, 'wb') as fd:
+        with open(fn, 'w') as fd:
             fd.write(MANIFEST_2)
 
     def prepare_env(self, z0ctx, odoo_ver=None, step=None):
         step = step or 1
         if not odoo_ver:
             raise (ValueError, 'No odoo version supplied')
         odoo_root = z0testodoo.build_odoo_env(z0ctx, odoo_ver)
```

### Comparing `wok_code-2.0.4/wok_code/tests/__license_mgnt.py` & `wok_code-2.0.6/wok_code/scripts/license_mgnt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,16 @@
-#!/usr/bin/env python
 # -*- coding: utf-8 -*-
 import os
-import re
 from datetime import datetime
+import re
+
+try:
+    from python_plus.python_plus import _u
+except ImportError:
+    from python_plus import _u
 
 COPY = {
     'zero': {
         'author': 'SHS-AV s.r.l.',
         'website': 'https://www.zeroincombenze.it',
         'devman': 'Antonio M. Vigliotti <antoniomaria.vigliotti@gmail.com>',
         'github-user': 'zeroincombenze',
@@ -24,14 +28,20 @@
     },
     'powerp': {
         'author': 'powERP enterprise network',
         'website': 'https://www.powerp.it',
         'devman': 'powERP enterprise network',
         'github-user': 'PowERP-cloud',
     },
+    'librerp': {
+        'author': 'LibrERP enterprise network',
+        'website': 'https://www.librerp.it',
+        'devman': 'LibrERP enterprise network',
+        'github-user': 'LibrERP-network',
+    },
     'didotech': {
         'author': 'Didotech s.r.l.',
         'website': 'https://www.didotech.com',
         'github-user': 'iw3hxn',
     },
 }
 ALIAS = {'shs-av': 'shs', 'zeroincombenze': 'zero'}
@@ -69,16 +79,16 @@
         elif email and email not in self.contributors:
             self.contributors[email] = [name, email, years]
         elif name and name not in self.authors:
             self.authors[name] = [name, website, years]
         self.purge_duplicate()
 
     def parse_file(self, author_file):
-        with open(author_file, 'rb') as fd:
-            for line in fd.read().split('\n'):
+        with open(author_file, 'r') as fd:
+            for line in _u(fd.read().split('\n')):
                 self.add_copyright(*self.extract_info_from_line(line))
 
     def purge_duplicate(self):
         for name in self.authors.copy().keys():
             website = self.authors[name][1]
             for org_id in self.org_ids.keys():
                 if (
@@ -168,15 +178,15 @@
                                     years = '%s-%s' % (years, line[ipos:ii])
                                 else:
                                     years = '%s-%s' % (years, str(self.cur_year)[-2:])
                             elif years != str(self.cur_year):
                                 years = '%s-%s' % (years, str(self.cur_year)[-2:])
                         elif years != str(self.cur_year):
                             years = '%s-%s' % (years, str(self.cur_year)[-2:])
-                org_id, name, website, email = from_rst_line(line[ipos:].strip())
+                org_id, name, website, email, dummy = from_rst_line(line[ipos:].strip())
             return org_id, name, website, email, years
 
         line = line.replace('`__', '').replace('`', '')
         if line.startswith('*'):
             return from_rst_line(line[1:].strip())
         elif line.startswith('#'):
             return from_comment_line(line[1:].strip())
```

### Comparing `wok_code-2.0.4/wok_code/tests/test_filepo.py` & `wok_code-2.0.6/wok_code/tests/test_filepo.py`

 * *Files identical despite different names*

### Comparing `wok_code-2.0.4/wok_code/ssh.py` & `wok_code-2.0.6/wok_code/ssh.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 import os
 import sys
 
-__version__ = '2.0.4'
+__version__ = '2.0.6'
 
 
 def get_remote_user():
     local_user = os.environ['USER']
     user = None
     default_user = None
     for key, item in DATA[host].items():
@@ -37,34 +37,30 @@
         param, user, host) if param else 'ssh %s@%s' % (user, host)
 
 
 def get_cmd_rsync(host, user, source, dest, recurse):
     param = DATA[host][user].get('param', "")
     port = ""
     if param.startswith("-p"):
-        port = param.split(" ")[0]
+        port = param.split(" ")[1]
         param = ""
     passwd = DATA[host][user].get('passwd')
     if recurse and not source.endswith("/"):
         source = "%s/" % source
     if recurse and not dest.endswith("/"):
         dest = "%s/" % dest
     if source.startswith("@"):
-        if port:
-            source = "%s@%s:%s:%s" % (user, host, source[1:], port)
-        else:
-            source = "%s@%s:%s" % (user, host, source[1:])
+        source = "%s@%s:%s" % (user, host, source[1:])
     elif dest.startswith("@"):
-        if port:
-            dest = "%s@%s:%s:%s" % (user, host, dest[1:], port)
-        else:
-            dest = "%s@%s:%s" % (user, host, dest[1:])
+        dest = "%s@%s:%s" % (user, host, dest[1:])
     if passwd:
         os.environ['SSHPASS'] = passwd
         return 'sshpass -e rsync -avz %s %s %s' % (param, source, dest)
+    if port:
+        return 'rsync -avz -e \'ssh -p %s\' %s %s %s' % (port, param, source, dest)
     return 'rsync -avz %s %s %s' % (param, source, dest)
 
 
 def get_cmd_scp(host, user, source, dest, recurse):
     param = DATA[host][user].get('param', "").replace("-p", "-P")
     if recurse:
         if param.startswith("-"):
@@ -196,14 +192,42 @@
     elif ctr == 2:
         source = param
         ctr += 1
     elif ctr == 3:
         dest = param
         ctr += 1
 
+if (scp or rsync) and user and not source and not dest:
+    # ssh.py -m|s user@host:source dest
+    # ssh.py -m|s source user@host:dest
+    source = host
+    host = ""
+    dest = user
+    user = ""
+    if ":" in source and ":" not in dest:
+        host, source = source.split(":", 1)
+        source = "@" + source
+    elif ":" not in source and ":" in dest:
+        host, dest = dest.split(":", 1)
+        dest = "@" + dest
+    else:
+        print("Invalid params! Use:")
+        print("ssh.py -m|s user@host:source dest")
+        print("ssh.py -m|s source user@host:dest")
+        exit(1)
+    if "@" in host:
+        user, host = host.split("@", 1)
+elif (scp or rsync) and user and source and not dest:
+    dest = source
+    source = user
+    user = ""
+elif do_dir and user and not source:
+    source = user
+    user = ""
+
 if host not in DATA and host in ALIAS:
     host = ALIAS[host]
 if list_host:
     show_host(sel_host=host)
     exit(0)
 if sh_alias:
     show_alias()
@@ -213,22 +237,14 @@
     exit(0)
 if host not in DATA:
     if host:
         print('Host %s not found!' % host)
     show_host()
     exit(1)
 
-if (scp or rsync) and user and source and not dest:
-    dest = source
-    source = user
-    user = ""
-elif do_dir and user and not source:
-    source = user
-    user = ""
-
 if not user:
     user = get_remote_user()
 if not user:
     print('No user supplied!')
     show_host(sel_host=host)
     exit(1)
 if user not in DATA[host]:
```

### Comparing `wok_code-2.0.4/wok_code/pypi.sh` & `wok_code-2.0.6/wok_code/pypi.sh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # set -x
-__version__=2.0.4
+__version__=2.0.6
 if [[ -z $HOME_DEVEL || ! -d $HOME_DEVEL ]]; then
   [[ -d $HOME/odoo/devel ]] && HOME_DEVEL="$HOME/odoo/devel" || HOME_DEVEL="$HOME/devel"
 fi
 
 run_traced() {
     local xcmd="$1"
     local sts=0
@@ -51,23 +51,23 @@
         [[ $1 =~ -.*U ]] && act="update"
         [[ $1 =~ -.*y ]] && opts=${opts}y
         [[ $1 =~ -.*Z ]] && opts=${opts}Z
     fi
     shift
 done
 [[ -n "$opts" ]] && opts="-$opts"
-ACTLIST="cvt_script|diff|dir|docs|git-add|info|install|libdir|list|meld|replace|show|travis|travis-summary|update|update+replace|version"
+HLPCMDLIST="cvt_script|diff|dir|docs|git-add|info|install|libdir|list|meld|replace|show|travis|travis-summary|update|update+replace|version"
 ACT2VME="^(dir|info|show|install|libdir|update|update\+replace|update)$"
 ACT2TOOLS="^(docs|git-add|list|replace|travis|travis-summary|version)$"
 PKGS_LIST="clodoo lisa odoo_score os0 python-plus travis_emulator wok_code z0bug-odoo z0lib zar zerobug"
 PKGS_LIST_RE="(${PKGS_LIST// /|})"
 PKGS_LIST_RE=${PKGS_LIST_RE//-/.}
 ODOO_ROOT=$(dirname $HOME_DEVEL)
-[[ -z "$act" || ! $act =~ ($ACTLIST) ]] && act="help"
-[[ $act == "help" ]] && echo "$0 [-h|-B|-f|-I|-l|-n|-U|-y|-Z] [-d VENV] [-b BRANCH] $ACTLIST|help [PYPI_PKG]" && exit 0
+[[ -z "$act" || ! $act =~ ($HLPCMDLIST) ]] && act="help"
+[[ $act == "help" ]] && echo "$0 [-h|-B|-f|-I|-l|-n|-U|-y|-Z] [-d VENV] [-b BRANCH] $HLPCMDLIST|help [PYPI_PKG]" && exit 0
 b=$(basename $PWD)
 [[ -z "$pypi" && $(dirname $PWD) == $HOME_DEVEL/pypi/$b && $b =~ $PKGS_LIST_RE ]] && pypi=$b
 [[ -z "$pypi" ]] && pypi="$PKGS_LIST" || pypi="${pypi//,/ }"
 [[ -z "$tgtdir" ]] && tgtdir="$ODOO_ROOT/VME/* $HOME_DEVEL/venv" || tgtdir="$(readlink -f $tgtdir)/*"
 [[ $tgtdir =~ ^[~/.] ]] || tgtdir="$ODOO_ROOT/$tgtdir"
 [[ $act =~ $ACT2TOOLS ]] && tgtdir=$HOME_DEVEL/pypi/tools
 [[ -n $branch ]] && branch="(${branch//,/|})"
```

### Comparing `wok_code-2.0.4/wok_code/cvt_csv_2_xml.py` & `wok_code-2.0.6/wok_code/cvt_csv_2_xml.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 try:
     from z0lib import z0lib
 except ImportError:
     import z0lib
 
 
-__version__ = "2.0.4"
+__version__ = "2.0.6"
 
 msg_time = time.time()
 
 
 def msg_burst(text):
     global msg_time
     t = time.time() - msg_time
```

### Comparing `wok_code-2.0.4/wok_code/scripts/please.sh` & `wok_code-2.0.6/wok_code/scripts/please.sh`

 * *Files 20% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # please
 # Developer shell
 #
 # This free software is released under GNU Affero GPL3
 # author: Antonio M. Vigliotti - antoniomaria.vigliotti@gmail.com
 # (C) 2015-2023 by SHS-AV s.r.l. - http://www.shs-av.com - info@shs-av.com
 #
+# set -x  #debug
 READLINK=$(which greadlink 2>/dev/null) || READLINK=$(which readlink 2>/dev/null)
 export READLINK
 # Based on template 2.0.0
 THIS=$(basename "$0")
 TDIR=$(readlink -f $(dirname $0))
 [ $BASH_VERSINFO -lt 4 ] && echo "This script $0 requires bash 4.0+!" && exit 4
 if [[ -z $HOME_DEVEL || ! -d $HOME_DEVEL ]]; then
@@ -38,61 +39,25 @@
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
 
-__version__=2.0.4
+__version__=2.0.4.2
 
-#
-# General Purpose options:
-# -A dont exec odoo test
-# -B exec bash test
-# -b branch: must be 6.1 7.0, 8.0, 9.0 10.0 11.0 12.0 13.0 or 14.0
-# -C commit & push | dont exc clodoo test
-# -c configuration file
-# -D duplicate odoo to another version
-# -d diff
-# -F fetch
-# -f force
-# -H use virtualenv
-# -k keep files
-# -K exec bash, flake8 and pylint tests | run cron environ
-# -j exec tests in project dir rather in test dir
-# -m show missing line in report
-# -n do nothing (dry-run)
-# -o limit push to ids
-# -O run odoo burst
-# -O replace odoo distribution
-# -o OCA directives
-# -P push
-# -p local path
-# -q silent mode
-# -R replace | replica
-# -r rescricted mode (w/o parsing travis.yml file)
-# -S status
-# -T exec regression test
-# -t do nothing (test-mode)
-# -u dont update newer files
-# -V show version
-# -v verbose mode
-# -W whatis
-# -w wep
 
 FIND_EXCL="-not -path '*/build/*' -not -path '*/_build/*' -not -path '*/dist/*' -not -path '*/docs/*' -not -path '*/__to_remove/*' -not -path '*/filestore/*' -not -path '*/.git/*' -not -path '*/html/*' -not -path '*/.idea/*' -not -path '*/latex/*' -not -path '*/__pycache__/*' -not -path '*/.local/*' -not -path '*/.npm/*' -not -path '*/.gem/*' -not -path '*/Trash/*' -not -path '*/VME/*'"
 
 get_dbuser() {
   # get_dbuser odoo_majver
   local u
   for u in $USER odoo openerp postgres; do
@@ -137,15 +102,14 @@
     [[ $opt_force -ne 0 ]] && opts="${opts} -f"
     [[ $opt_verbose -eq 0 ]] && opts="${opts} -q"
     [[ $opt_verbose -eq 1 ]] && opts="${opts} -v"
     [[ $opt_verbose -eq 2 ]] && opts="${opts} -vv"
     [[ $opt_verbose -eq 3 ]] && opts="${opts} -vvv"
 }
 
-
 move() {
   # move(src dst)
   if [ -f "$2" ]; then rm -f $2; fi
   run_traced "cp -p $1 $2"
   run_traced "rm -f $1"
 }
 
@@ -172,252 +136,14 @@
         alt=$(find -L $src/i18n -name '*.po' | head -n1)
         src=
         if [ -n "$alt" ]; then fi=1 break; fi
       fi
     fi
   done
 }
-#
-#add_copyright() {
-#  #add_copyright(file rst zero|oca|powerp)
-#  if [[ "$PRJNAME" == "Odoo" ]]; then
-#    if [[ $2 -eq 1 ]]; then
-#      echo ".. [//]: # (copyright)" >>$1
-#    else
-#      echo "[//]: # (copyright)" >>$1
-#    fi
-#    echo "" >>$1
-#    echo "----" >>$1
-#    echo "" >>$1
-#    if [[ $2 -eq 1 ]]; then
-#      echo "**Odoo** is a trademark of  \`Odoo S.A." >>$1
-#      echo "<https://www.odoo.com/>\`_." >>$1
-#      echo "(formerly OpenERP, formerly TinyERP)" >>$1
-#    else
-#      echo "**Odoo** is a trademark of [Odoo S.A.](https://www.odoo.com/) (formerly OpenERP, formerly TinyERP)" >>$1
-#    fi
-#    echo "" >>$1
-#    if [[ $2 -eq 1 ]]; then
-#      echo "**OCA**, or the  \`Odoo Community Association" >>$1
-#      echo "<http://odoo-community.org/>\`_." >>$1
-#      echo "is a nonprofit organization whose" >>$1
-#    else
-#      echo "**OCA**, or the [Odoo Community Association](http://odoo-community.org/), is a nonprofit organization whose" >>$1
-#    fi
-#    echo "mission is to support the collaborative development of Odoo features and" >>$1
-#    echo "promote its widespread use." >>$1
-#    echo "" >>$1
-#    if [[ "$3" == "powerp" ]]; then
-#      echo "**powERP**, or the [powERP enterprise network](https://www.powerp.it/)" >>$1
-#      echo "is an Italian enterprise network whose mission is to develop high-level" >>$1
-#      echo "addons designed for Italian enterprise companies." >>$1
-#      echo "The powER software, released under Odoo Proprietary License," >>$1
-#      echo "adds new enhanced features to Italian localization." >>$1
-#      echo "La rete di imprese [powERP](https://www.powerp.it/)" >>$1
-#      echo "fornisce, sotto licenza OPL, estensioni evolute della localizzazine italiana." >>$1
-#      echo "Il software è progettato per medie e grandi imprese italiane" >>$1
-#      echo "che richiedono caratteristiche non disponibili nella versione Odoo CE" >>$1
-#      echo "" >>$1
-#    else
-#      if [ $2 -eq 1 ]; then
-#        echo "**zeroincombenze®** is a trademark of \`SHS-AV s.r.l." >>$1
-#        echo "<http://www.shs-av.com/>\`_." >>$1
-#      else
-#        echo "**zeroincombenze®** is a trademark of [SHS-AV s.r.l.](http://www.shs-av.com/)" >>$1
-#      fi
-#      echo "which distributes and promotes **Odoo** ready-to-use on own cloud infrastructure." >>$1
-#      echo "[Zeroincombenze® distribution of Odoo](http://wiki.zeroincombenze.org/en/Odoo)" >>$1
-#      echo "is mainly designed for Italian law and markeplace." >>$1
-#      echo "Users can download from [Zeroincombenze® distribution](https://github.com/zeroincombenze/OCB) and deploy on local server." >>$1
-#      echo "" >>$1
-#    fi
-#    if [ $2 -eq 1 ]; then
-#      echo "" >>$1
-#      echo ".. [//]: # (end copyright)" >>$1
-#    else
-#      echo "[//]: # (end copyright)" >>$1
-#    fi
-#  else
-#    if [ $2 -eq 1 ]; then
-#      echo ".. [//]: # (copyright)" >>$1
-#    else
-#      echo "[//]: # (copyright)" >>$1
-#    fi
-#    echo "" >>$1
-#    echo "----" >>$1
-#    echo "" >>$1
-#    if [ $2 -eq 1 ]; then
-#      echo "**zeroincombenze®** is a trademark of \`SHS-AV s.r.l." >>$1
-#      echo "<http://www.shs-av.com/>\`_." >>$1
-#    else
-#      echo "**zeroincombenze®** is a trademark of [SHS-AV s.r.l.](http://www.shs-av.com/)" >>$1
-#    fi
-#    echo "which distributes and promotes **Odoo** ready-to-use on its own cloud infrastructure." >>$1
-#    echo "" >>$1
-#    echo "Odoo is a trademark of Odoo S.A." >>$1
-#    if [ $2 -eq 1 ]; then
-#      echo "" >>$1
-#      echo ".. [//]: # (end copyright)" >>$1
-#    else
-#      echo "[//]: # (end copyright)" >>$1
-#    fi
-#  fi
-#}
-
-#add_addons() {
-#  #add_addons(file rst zero|oca|oia ORIG)
-#  if [ "$PRJNAME" == "Odoo" ]; then
-#    if [ $2 -eq 1 ]; then
-#      echo ".. [//]: # (addons)" >>$1
-#    else
-#      echo "[//]: # (addons)" >>$1
-#    fi
-#    $TDIR/gen_addons_table.py addons $4 >>$1
-#    if [ $2 -eq 1 ]; then
-#      echo "" >>$1
-#      echo ".. [//]: # (end addons)" >>$1
-#    else
-#      echo "[//]: # (end addons)" >>$1
-#    fi
-#  fi
-#}
-
-#add_install() {
-#  #add_install(file rst zero|oca|oia ORIG)
-#  if [ "$PRJNAME" == "Odoo" ]; then
-#    local pkgs
-#    local gitorg=$3
-#    [ "$3" == "zero" -o "$3" == "oia" ] && gitorg=${3}-http
-#    if [ -z "$REPOSNAME" ]; then
-#      local REPOS=$PKGNAME
-#      local url=$(build_odoo_param GIT_URL '.' "" "$gitorg")
-#      local root=$(build_odoo_param HOME '.')
-#    else
-#      pushd .. >/dev/null
-#      local REPOS=$REPOSNAME
-#      local url=$(build_odoo_param GIT_URL '.' "" "$gitorg")
-#      local root=$(build_odoo_param HOME '.')
-#      popd >/dev/null
-#    fi
-#    if [ $2 -eq 1 ]; then
-#      echo ".. [//]: # (install)" >>$1
-#    else
-#      echo "[//]: # (install)" >>$1
-#    fi
-#    echo "    ODOO_DIR=$root  # here your Odoo dir" >>$1
-#    echo "    BACKUP_DIR=$HOME/backup  # here your backup dir" >>$1
-#    pkgs=$(list_requirements.py -p $PWD -s' ' -P -t python)
-#    pkgs="${pkgs:7}"
-#    if [ -n "$pkgs" ]; then
-#      echo "    for pkg in $pkgs; do" >>$1
-#      echo "        pip install \$pkg" >>$1
-#      echo "    done" >>$1
-#    fi
-#    pkgs=$(list_requirements.py -p $PWD -s' ' -P -t modules)
-#    pkgs="${pkgs:8}"
-#    if [ -n "$pkgs" ]; then
-#      echo "    # Check for <$pkgs> modules" >>$1
-#    fi
-#    echo "    cd /tmp" >>$1
-#    echo "    git clone $url $REPOS" >>$1
-#    echo "    mv \$ODOO_DIR/$REPOS/$PKGNAME/ \$BACKUP_DIR/" >>$1
-#    echo "    mv /tmp/$REPOS/$PKGNAME/ \$ODOO_DIR/" >>$1
-#    if [ $2 -eq 1 ]; then
-#      echo "" >>$1
-#      echo ".. [//]: # (end install)" >>$1
-#    else
-#      echo "[//]: # (end install)" >>$1
-#    fi
-#  fi
-#}
-
-#restore_owner() {
-#  if [ "$USER" != "odoo" ]; then
-#    local fown="odoo:odoo"
-#    # [ "$USER" == "travis" ] && fown="travis:odoo"
-#    if sudo -v &>/dev/null; then
-#      run_traced "sudo chown -R $fown .git"
-#    elif [ "$USER" != "travis" ]; then
-#      run_traced "chown -R $fown .git"
-#    fi
-#  fi
-#}
-
-#expand_macro() {
-#  local t p v lne lne1
-#  lne="$1"
-#  for t in {1..9} LNK_DOCS BTN_DOCS LNK_HELP BTN_HELP; do
-#    p=\${$t}
-#    v=${M[$t]}
-#    lne1="${lne//$p/$v}"
-#    lne="$lne1"
-#  done
-#  echo -n "$lne"
-#}
-
-#get_ver() {
-#  local ver=
-#  if [ -n "$BRANCH" ]; then
-#    if [ "$BRANCH" == "master" ]; then
-#      ver=$BRANCH
-#    else
-#      ver=$(echo $BRANCH | grep --color=never -Eo '[0-9]+' | head -n1)
-#    fi
-#  else
-#    ver=master
-#  fi
-#  [ -n "$1" -a "$ver" == "master" ] && ver=0
-#  echo $ver
-#}
-
-#build_line() {
-#  # build_line(flag replmnt act)
-#  local v w x line
-#  v=${1^^}
-#  w="LNK_${v:1}"
-#  v="BTN_${v:1}"
-#  line="$2"
-#  if [[ "$3" =~ md_BTN ]]; then
-#    if [ -n "${M[$v]}" ]; then
-#      x="${M[$v]}"
-#      line="$line($x)]"
-#    fi
-#    if [ -n "${M[$w]}" ]; then
-#      x="${M[$w]}"
-#      line="$line($x)"
-#    fi
-#  elif [[ "$3" =~ rstBTN_.*/1 ]]; then
-#    if [ -z "$2" ]; then
-#      line=".. image::"
-#    else
-#      line=".. ${line:0:-1} image::"
-#    fi
-#    if [ -n "${M[$v]}" ]; then
-#      x="${M[$v]}"
-#      line="$line $x"
-#    fi
-#  elif [[ "$3" =~ rstBTN_.*/2 ]]; then
-#    if [ -z "$2" ]; then
-#      line="   :target:"
-#    else
-#      line=".. _${line:1:-2}:"
-#    fi
-#    if [ -n "${M[$w]}" ]; then
-#      x="${M[$w]}"
-#      line="$line $x"
-#    fi
-#  elif [ "$3" == "CHPT_lang_en" ]; then
-#    line="[![en](https://github.com/zeroincombenze/grymb/blob/master/flags/en_US.png)](https://www.facebook.com/groups/openerp.italia/)"
-#  elif [ "$3" == "CHPT_lang_it" ]; then
-#    line="[![it](https://github.com/zeroincombenze/grymb/blob/master/flags/it_IT.png)](https://www.facebook.com/groups/openerp.italia/)"
-#  elif [[ $3 =~ CHPT_ ]]; then
-#    :
-#  fi
-#  echo "$line"
-#}
 
 #cvt_doxygenconf() {
 #  local fn=$1
 #  if [ -f $fn ]; then
 #    local fntmp=$fn.tmp
 #    rm -f $fntmp
 #    local line lne submod url p v
@@ -459,158 +185,14 @@
 #      move_n_bak $fntmp $fn
 #    else
 #      rm -f $fntmp
 #    fi
 #  fi
 #}
 
-#cvt_gitmodule() {
-#  #cvt_gitmodule(oca|zero)
-#  if [ -f .gitmodules ]; then
-#    local fn=.gitmodules
-#    local fntmp=$fn.tmp
-#    local urlty=zero-http
-#    rm -f $fntmp
-#    local line lne submod url p v
-#    while IFS= read -r line r || [ -n "$line" ]; do
-#      if [ "${line:0:1}" == "[" -a "${line: -1}" == "]" ]; then
-#        lne="${line:1:-1}"
-#        read p v <<<"$lne"
-#        submod=${v//\"/}
-#      else
-#        lne=$(echo $line)
-#        IFS== read p v <<<$lne
-#        lne=$(echo $p)
-#        if [ "$lne" == "url" ]; then
-#          url=$(build_odoo_param URL '' $submod $urlty)
-#          lne=$(echo $v)
-#          if [ "$lne" != "$url" ]; then
-#            v="${line//$lne/$url}"
-#            line="$v"
-#          fi
-#        fi
-#      fi
-#      echo "$line" >>$fntmp
-#    done <"$fn"
-#    if [ -n "$(diff -q $fn $fntmp)" ]; then
-#      move_n_bak $fntmp $fn
-#    else
-#      rm -f $fntmp
-#    fi
-#  fi
-#}
-
-#cvt_travis() {
-#  # cvt_travis(file_travis oca|zero|oia currpt ORIG)
-#  local fn=$1
-#  local fntmp=$fn.tmp
-#  ORGNM=$(build_odoo_param GIT_ORGNM '' '' $2)
-#  run_traced "tope8 -B -b $odoo_fver $fn"
-#  run_traced "sed -e \"s|ODOO_REPO=.[^/]*|ODOO_REPO=\\\"$ORGNM|\" -i $fn"
-#}
-
-#cvt_file() {
-#  # cvt_file(file oca|zero|powerp travis|readme|manifest currpt ORIG)
-#  local f1=$1
-#  local sts=$STS_SUCCESS
-#  if [ -n "$f1" ]; then
-#    if [ -f "$1" ]; then
-#      local b=$(basename $f1)
-#      local d=$(dirname $f1)
-#      if [[ $f1 =~ $PWD ]]; then
-#        local l=${#PWD}
-#        ((l++))
-#        local ft=${f1:l}
-#      elif [ "${f1:0:2}" == "./" ]; then
-#        local ft=${f1:2}
-#      else
-#        local ft=$f1
-#      fi
-#      local f1_oca=$(dirname $f1)/${b}.oca
-#      local f1_z0i=$(dirname $f1)/${b}.z0i
-#      local f1_oia=$(dirname $f1)/${b}.oia
-#      if [ "$2" == "zero" -o -z "$2" ]; then
-#        local f1_new=$f1_z0i
-#      else
-#        local f1_new=$(dirname $f1)/${b}.$2
-#      fi
-#      if [ "$4" == "zero" -o -z "$4" ]; then
-#        local f1_cur=$f1_z0i
-#      else
-#        local f1_cur=$(dirname $f1)/${b}.$4
-#      fi
-#      if [ "$2" == "$4" -a $opt_force -eq 0 ]; then
-#        local do_proc=0
-#      else
-#        local do_proc=1
-#      fi
-#      local fntmp=$f1.tmp
-#      if [ -f $f1_new ]; then
-#        if [ -f "$f1_oca" -a -f "$f1_oia" -a -f "$f1_zoi" ]; then
-#          :
-#        else
-#          move $f1 $f1_cur
-#        fi
-#        move $f1_new $f1
-#        do_proc=1
-#      elif [ $opt_force -ne 0 -a ! -f $f1_cur -a "$3" != "graph" -a "$3" != "xml" -a "$3" != "css" -a "$3" != "sass" ]; then
-#        if [ -f "$f1_cur" ]; then rm -f $f1_cur; fi
-#        run_traced "cp -p $f1 $f1_cur"
-#        do_proc=1
-#      fi
-##      if [ $opt_orig -gt 0 -a -f ./tmp/$ft ]; then
-##        run_traced "mv -f $f1 ${f1}.bak"
-##        run_traced "cp -p ./tmp/$ft $f1"
-##      fi
-#      if [ "$3" == "travis" ]; then
-#        cvt_travis $f1 "$2" "$4" "$5"
-#      elif [ "$3" == "readme" ] && [ ${test_mode:-0} -ne 0 -o $do_proc -gt 0 ]; then
-#        # cvt_readme $f1 "$2" "$4" "$5"
-#        :
-#      fi
-#      if [ -f $f1_cur ] && [ $opt_force -eq 0 -o "$3" == "manifest" ]; then
-#        diff -q $f1 $f1_cur &>/dev/null
-#        if [ $? -eq 0 ]; then
-#          run_traced "rm -f $f1_cur"
-#        fi
-#      fi
-#    else
-#      echo "File $f1 not found!"
-#    fi
-#  else
-#    local f1=
-#    echo "Missed parameter! use:"
-#    echo "\$ please distribution oca|zero|oia"
-#    sts=$STS_FAILED
-#  fi
-#  return $sts
-#}
-
-#set_remote_info() {
-#  #set_remote_info (REPOSNAME odoo_vid odoo_org)
-#  local REPOSNAME=$1
-#  if [ "$(build_odoo_param VCS $2)" == "git" ]; then
-#    local odoo_fver=$(build_odoo_param FULLVER "$2")
-#    local DUPSTREAM=$(build_odoo_param RUPSTREAM "$2" "default" $3)
-#    local RUPSTREAM=$(build_odoo_param RUPSTREAM "$2" "" $3)
-#    local DORIGIN=$(build_odoo_param RORIGIN "$2" "default" $3)
-#    local RORIGIN=$(build_odoo_param RORIGIN "$2" "" $3)
-#    if [[ ! "$DUPSTREAM" == "$RUPSTREAM" ]]; then
-#      [[ -n "$RUPSTREAM" ]] && run_traced "git remote remove upstream"
-#      [[ -n "$DUPSTREAM" ]] && run_traced "git remote add upstream $DUPSTREAM"
-#    fi
-#    if [[ ! "$DORIGIN" == "$RORIGIN" ]]; then
-#      [[ -n "$RORIGIN" ]] && run_traced "git remote remove origin"
-#      [[ -n "$DORIGIN" ]] && run_traced "git remote add origin $DORIGIN"
-#    fi
-#  elif [ ${test_mode:-0} -eq 0 ]; then
-#    echo "No git repositoy $REPOSNAME!"
-#  fi
-#}
-
 mvfiles() {
   # mvfiles(srcpath, tgtpath, files, owner)
   if [ -z "$3" ]; then
     local l="*"
   else
     local l="$3"
   fi
@@ -1034,117 +616,117 @@
       echo "File $f not found"
       break
     fi
   done
   return $s
 }
 
-do_build() {
-  #do_build pgkname tar
-  local sts=$STS_SUCCESS
-  local rpt=pypi
-  local f i l n p s v x y PKGLIST invalid PASSED
-  local SETUP=./setup.sh
-  local xx="$(get_cfg_value 0 filedel)"
-  local yy="$(get_cfg_value 0 fileignore)"
-  if [ $opt_keep -ne 0 ]; then
-    xx="$xx $yy"
-  else
-    xx="$xx $yy tests/"
-  fi
-  if [ "$PRJNAME" != "Odoo" ]; then
-    run_traced "cd $PKGPATH"
-    # run_traced "mkdir -p tmp"
-    s=$?; [ ${s-0} -ne 0 ] && sts=$s
-    n=$(cat setup.py | grep "name *=" | awk -F= '{print $2}' | grep --color=never -Eo '[a-zA-Z0-9_-]+' | head -n1)
-    v=$(cat setup.py | grep version | grep --color=never -Eo '[0-9]+\.[0-9]+\.[0-9]+' | head -n1)
-    if [ ! -f "$n*$v*tar.gz" -o $opt_force -gt 0 ]; then
-      PKGLIST=$(cat setup.py | grep "# PKGLIST=" | awk -F= '{print $2}')
-      if [ -n "$PKGLIST" ]; then
-        PKGLIST=${PKGLIST//,/ }
-      else
-        if [ "$PRJNAME" == "lisa" ]; then
-          cp ../../clodoo/clodoo/odoorc ./
-          cp ../../z0lib/z0lib/z0librc ./
-        fi
-        x="find . -type f"
-        for f in $xx "setup.*"; do
-          if [ "${f: -1}" == "/" ]; then
-            x="$x -not -path '*/$f*'"
-          else
-            x="$x -not -name '*$f'"
-          fi
-        done
-        eval $x >./tmp.log
-        PKGLIST="$(cat ./tmp.log)"
-        rm -f ./tmp.log
-      fi
-      invalid=
-      for f in $PKGLIST; do
-        if [ -f $f ]; then
-          :
-          #cp $f $PKGPATH/tmp
-        else
-          invalid=$f
-        fi
-      done
-      if [ -n "$invalid" ]; then
-        echo "File $f not found"
-        return 1
-      fi
-      p="$n-$v.tar.gz"
-      if [ -f $p ]; then
-        run_traced "rm -f $p"
-      fi
-      echo "# $p" >$SETUP
-      f=
-      for i in {2..9}; do
-        x=$(echo $PRJPATH | awk -F/ '{print $'$i'}')
-        if [ -n "$x" ]; then
-          f=$f/$x
-          if [ $i -gt 3 ]; then
-            echo "mkdir -p $f" >>$SETUP
-          fi
-        fi
-      done
-      l=${#PKGPATH}
-      f=".${PRJPATH:l}" # subroot
-      l=${#f}
-      ((l++))
-      PASSED=
-      x="-cf"
-      for f in $PKGLIST; do
-        y=$(dirname ./${f:l})
-        if [ "$y" != "." ]; then
-          y=$(dirname ${f:l})
-          if [[ " $PASSED " =~ [[:space:]]$y[[:space:]] ]]; then
-            :
-          else
-            echo "mkdir -p $PRJPATH/$y" >>$SETUP
-            PASSED="$PASSED $y"
-          fi
-          y=$y/
-        else
-          y=
-        fi
-        run_traced "tar $x $p $f"
-        x=${x/c/r}
-        # if [ -f "$f" ]; then rm -f $f; fi
-        echo "cp -p $f $PKGPATH/$y" >>$SETUP
-      done
-      chmod +x $SETUP
-      if [ -x $PRJPATH/setup.sh ]; then
-        run_traced "cp $PRJPATH/setup.sh $SETUP"
-      fi
-      run_traced "tar $x $p $SETUP"
-      run_traced "rm -f $SETUP"
-    fi
-  fi
-  return $sts
-}
+#do_build() {
+#  #do_build pgkname tar
+#  local sts=$STS_SUCCESS
+#  local rpt=pypi
+#  local f i l n p s v x y PKGLIST invalid PASSED
+#  local SETUP=./setup.sh
+#  local xx="$(get_cfg_value 0 filedel)"
+#  local yy="$(get_cfg_value 0 fileignore)"
+#  if [ $opt_keep -ne 0 ]; then
+#    xx="$xx $yy"
+#  else
+#    xx="$xx $yy tests/"
+#  fi
+#  if [ "$PRJNAME" != "Odoo" ]; then
+#    run_traced "cd $PKGPATH"
+#    # run_traced "mkdir -p tmp"
+#    s=$?; [ ${s-0} -ne 0 ] && sts=$s
+#    n=$(cat setup.py | grep "name *=" | awk -F= '{print $2}' | grep --color=never -Eo '[a-zA-Z0-9_-]+' | head -n1)
+#    v=$(cat setup.py | grep version | grep --color=never -Eo '[0-9]+\.[0-9]+\.[0-9]+' | head -n1)
+#    if [ ! -f "$n*$v*tar.gz" -o $opt_force -gt 0 ]; then
+#      PKGLIST=$(cat setup.py | grep "# PKGLIST=" | awk -F= '{print $2}')
+#      if [ -n "$PKGLIST" ]; then
+#        PKGLIST=${PKGLIST//,/ }
+#      else
+#        if [ "$PRJNAME" == "lisa" ]; then
+#          cp ../../clodoo/clodoo/odoorc ./
+#          cp ../../z0lib/z0lib/z0librc ./
+#        fi
+#        x="find . -type f"
+#        for f in $xx "setup.*"; do
+#          if [ "${f: -1}" == "/" ]; then
+#            x="$x -not -path '*/$f*'"
+#          else
+#            x="$x -not -name '*$f'"
+#          fi
+#        done
+#        eval $x >./tmp.log
+#        PKGLIST="$(cat ./tmp.log)"
+#        rm -f ./tmp.log
+#      fi
+#      invalid=
+#      for f in $PKGLIST; do
+#        if [ -f $f ]; then
+#          :
+#          #cp $f $PKGPATH/tmp
+#        else
+#          invalid=$f
+#        fi
+#      done
+#      if [ -n "$invalid" ]; then
+#        echo "File $f not found"
+#        return 1
+#      fi
+#      p="$n-$v.tar.gz"
+#      if [ -f $p ]; then
+#        run_traced "rm -f $p"
+#      fi
+#      echo "# $p" >$SETUP
+#      f=
+#      for i in {2..9}; do
+#        x=$(echo $PRJPATH | awk -F/ '{print $'$i'}')
+#        if [ -n "$x" ]; then
+#          f=$f/$x
+#          if [ $i -gt 3 ]; then
+#            echo "mkdir -p $f" >>$SETUP
+#          fi
+#        fi
+#      done
+#      l=${#PKGPATH}
+#      f=".${PRJPATH:l}" # subroot
+#      l=${#f}
+#      ((l++))
+#      PASSED=
+#      x="-cf"
+#      for f in $PKGLIST; do
+#        y=$(dirname ./${f:l})
+#        if [ "$y" != "." ]; then
+#          y=$(dirname ${f:l})
+#          if [[ " $PASSED " =~ [[:space:]]$y[[:space:]] ]]; then
+#            :
+#          else
+#            echo "mkdir -p $PRJPATH/$y" >>$SETUP
+#            PASSED="$PASSED $y"
+#          fi
+#          y=$y/
+#        else
+#          y=
+#        fi
+#        run_traced "tar $x $p $f"
+#        x=${x/c/r}
+#        # if [ -f "$f" ]; then rm -f $f; fi
+#        echo "cp -p $f $PKGPATH/$y" >>$SETUP
+#      done
+#      chmod +x $SETUP
+#      if [ -x $PRJPATH/setup.sh ]; then
+#        run_traced "cp $PRJPATH/setup.sh $SETUP"
+#      fi
+#      run_traced "tar $x $p $SETUP"
+#      run_traced "rm -f $SETUP"
+#    fi
+#  fi
+#  return $sts
+#}
 
 
 do_docs() {
   wlog "do_docs"
   local docs_dir=./docs
   local author version theme SETUP b f l t x
   local opts src_png odoo_fver REPO
@@ -1849,15 +1431,15 @@
   if [ "$(type -t $cmd)" == "function" ]; then
     eval $cmd "$@"
   else
     echo "Missing object! Use:"
     echo "> please show (docs|licence)"
     echo "show docs        -> show docs using local browser"
     echo "show license     -> show licenses of modules of current Odoo repository"
-    echo "show status      -> show component status"
+    # echo "show status      -> show component status"
     sts=$STS_FAILED
   fi
   return $sts
 }
 
 do_show_docs() {
   if [[ ! "$PRJNAME" == "Odoo" ]]; then
@@ -1883,68 +1465,68 @@
       module=$(basename $path)
       licence=$(grep "[\"']license[\"'] *:" $fn|grep --color=never -Eo "(.GPL-3|OPL-1)")
       printf "Module %-60.60s: $licence\n" $module
     done
   fi
   return 0
 }
-
-do_show_status() {
-  local s v1 v2 v x y
-  local PKGS_LIST=$(get_cfg_value 0 "PKGS_LIST")
-  pushd $HOME/tools >/dev/null
-  local PKGS=$(git status -s | grep -E "^ M" | awk '{print $2}' | awk -F/ '{print $1}' | grep -v "^[0-9]" | sort -u | tr "\n" "|")
-  local PKGS_V=$(git diff -G__version__ --compact-summary | awk '{print $1}' | awk -F/ '{print $1}' | grep -v "^[0-9]" | sort -u | tr "\n" "|")
-  [[ -n "$PKGS" ]] && PKGS="(${PKGS:0:-1})" || PKGS="()"
-  [[ -n "$PKGS_V" ]] && PKGS_V="(${PKGS_V:0:-1})" || PKGS_V="()"
-  popd >/dev/null
-  for pkg in $PKGS_LIST tools; do
-    x=""
-    [[ $opt_force -ne 0 ]] && echo -e "\e[1m[ $pkg ]\e[0m"
-    [[ $opt_force -eq 0 ]] && echo -e "[ $pkg ]"
-    [[ $pkg =~ (python-plus|z0bug-odoo) ]] && pkg="${pkg//-/_}"
-    if [[ $pkg == "tools" ]]; then
-      for fn in egg-info licence_text templates .travis.yml install_tools.sh odoo_default_tnl.xlsx setup.py; do
-        vfdiff -X diff $HOME/$pkg/$fn $HOME_DEVEL/pypi/$pkg/$fn -q >/dev/null
-        if [[ $? -ne 0 ]]; then
-          x="R"
-          [[ $opt_force -ne 0 ]] && vfdiff -X diff $HOME/$pkg/$fn $HOME_DEVEL/pypi/$pkg/$fn
-          break
-        fi
-      done
-    else
-      vfdiff -X diff $HOME/tools/$pkg $HOME_DEVEL/pypi/$pkg/$pkg -q >/dev/null
-      if [[ $? -ne 0 ]]; then
-        x="R"
-        [[ $opt_force -ne 0 ]] && vfdiff -X diff $HOME/tools/$pkg $HOME_DEVEL/pypi/$pkg/$pkg
-      fi
-    fi
-    [[ $PKGS != "()" && $pkg =~ $PKGS ]] && x="$x G"
-    [[ $PKGS_V != "()" && $pkg =~ $PKGS_V ]] && x="$x V"
-    if [[ $pkg == "tools" ]]; then
-      v1=$(grep -E "version" $HOME/tools/setup.py|head -n1|awk -F= '{print $2}'|grep --color=never -Eo "[0-9.]+")
-      v2=$(grep -E "version" $HOME_DEVEL/pypi/$pkg/setup.py|head -n1|awk -F= '{print $2}'|grep --color=never -Eo "[0-9.]+")
-    else
-      v1=$(grep -E "version" $HOME/tools/$pkg/setup.py|head -n1|awk -F= '{print $2}'|grep --color=never -Eo "[0-9.]+")
-      v2=$(grep -E "version" $HOME_DEVEL/pypi/$pkg/setup.py|head -n1|awk -F= '{print $2}'|grep --color=never -Eo "[0-9.]+")
-    fi
-    if [[ $x =~ "R" ]]; then
-      [[ $pkg == "tools" ]] && s="$HOME_DEVEL/pypi/$pkg" || s="$HOME_DEVEL/pypi/$pkg/$pkg"
-      if [[ $v1 == $v2 && ! $x =~ "V" ]]; then
-        v=$(echo $v2 | awk -F. '{if ($NF == 3) {OFS="."; print $1,$2,int($3)+1} else {OFS="."; print $1,$2,$3,int($4)+1}}')
-        echo -e "\e[1m    Execute: cd $s; please version $v2 $v; travis && please replace\e[0m"
-      else
-        echo -e "\e[1m    Execute: cd $s; travis && please replace\e[0m"
-      fi
-    fi
-    [[ $x =~ "G" && $x =~ "V" ]] && echo -e "\e[1m    Package $pkg (new version $v1) have to be pushed on github.com\e[0m"
-    [[ $x =~ "G" && ! $x =~ "V" ]] && echo -e "\e[1m    Package $pkg differs from github.com but it has the same version $v1!!\e[0m"
-  done
-  [[ -f $HOME/tools/egg-info/history.rst ]] && head $HOME/tools/egg-info/history.rst
-}
+#
+#do_show_status() {
+#  local s v1 v2 v x y
+#  local PKGS_LIST=$(get_cfg_value 0 "PKGS_LIST")
+#  pushd $HOME/tools >/dev/null
+#  local PKGS=$(git status -s | grep -E "^ M" | awk '{print $2}' | awk -F/ '{print $1}' | grep -v "^[0-9]" | sort -u | tr "\n" "|")
+#  local PKGS_V=$(git diff -G__version__ --compact-summary | awk '{print $1}' | awk -F/ '{print $1}' | grep -v "^[0-9]" | sort -u | tr "\n" "|")
+#  [[ -n "$PKGS" ]] && PKGS="(${PKGS:0:-1})" || PKGS="()"
+#  [[ -n "$PKGS_V" ]] && PKGS_V="(${PKGS_V:0:-1})" || PKGS_V="()"
+#  popd >/dev/null
+#  for pkg in $PKGS_LIST tools; do
+#    x=""
+#    [[ $opt_force -ne 0 ]] && echo -e "\e[1m[ $pkg ]\e[0m"
+#    [[ $opt_force -eq 0 ]] && echo -e "[ $pkg ]"
+#    [[ $pkg =~ (python-plus|z0bug-odoo) ]] && pkg="${pkg//-/_}"
+#    if [[ $pkg == "tools" ]]; then
+#      for fn in egg-info licence_text templates .travis.yml install_tools.sh odoo_default_tnl.xlsx setup.py; do
+#        vfdiff -X diff $HOME/$pkg/$fn $HOME_DEVEL/pypi/$pkg/$fn -q >/dev/null
+#        if [[ $? -ne 0 ]]; then
+#          x="R"
+#          [[ $opt_force -ne 0 ]] && vfdiff -X diff $HOME/$pkg/$fn $HOME_DEVEL/pypi/$pkg/$fn
+#          break
+#        fi
+#      done
+#    else
+#      vfdiff -X diff $HOME/tools/$pkg $HOME_DEVEL/pypi/$pkg/$pkg -q >/dev/null
+#      if [[ $? -ne 0 ]]; then
+#        x="R"
+#        [[ $opt_force -ne 0 ]] && vfdiff -X diff $HOME/tools/$pkg $HOME_DEVEL/pypi/$pkg/$pkg
+#      fi
+#    fi
+#    [[ $PKGS != "()" && $pkg =~ $PKGS ]] && x="$x G"
+#    [[ $PKGS_V != "()" && $pkg =~ $PKGS_V ]] && x="$x V"
+#    if [[ $pkg == "tools" ]]; then
+#      v1=$(grep -E "version" $HOME/tools/setup.py|head -n1|awk -F= '{print $2}'|grep --color=never -Eo "[0-9.]+")
+#      v2=$(grep -E "version" $HOME_DEVEL/pypi/$pkg/setup.py|head -n1|awk -F= '{print $2}'|grep --color=never -Eo "[0-9.]+")
+#    else
+#      v1=$(grep -E "version" $HOME/tools/$pkg/setup.py|head -n1|awk -F= '{print $2}'|grep --color=never -Eo "[0-9.]+")
+#      v2=$(grep -E "version" $HOME_DEVEL/pypi/$pkg/setup.py|head -n1|awk -F= '{print $2}'|grep --color=never -Eo "[0-9.]+")
+#    fi
+#    if [[ $x =~ "R" ]]; then
+#      [[ $pkg == "tools" ]] && s="$HOME_DEVEL/pypi/$pkg" || s="$HOME_DEVEL/pypi/$pkg/$pkg"
+#      if [[ $v1 == $v2 && ! $x =~ "V" ]]; then
+#        v=$(echo $v2 | awk -F. '{if ($NF == 3) {OFS="."; print $1,$2,int($3)+1} else {OFS="."; print $1,$2,$3,int($4)+1}}')
+#        echo -e "\e[1m    Execute: cd $s; please version $v2 $v; travis && please replace\e[0m"
+#      else
+#        echo -e "\e[1m    Execute: cd $s; travis && please replace\e[0m"
+#      fi
+#    fi
+#    [[ $x =~ "G" && $x =~ "V" ]] && echo -e "\e[1m    Package $pkg (new version $v1) have to be pushed on github.com\e[0m"
+#    [[ $x =~ "G" && ! $x =~ "V" ]] && echo -e "\e[1m    Package $pkg differs from github.com but it has the same version $v1!!\e[0m"
+#  done
+#  [[ -f $HOME/tools/egg-info/history.rst ]] && head $HOME/tools/egg-info/history.rst
+#}
 
 do_version() {
   # do_version([cur_ver [new_ver]])
   local re1 re2 new_ver
   re1="^#? *__version__ *="
   [[ -n $1 ]] && re2="${re1} *([\"'])?$1\1?$" || re2=$re1
   [[ -n $2 ]] && new_ver="$2" || new_ver=""
@@ -2030,17 +1612,27 @@
       fi
     fi
   fi
   return $sts
 }
 
 do_wep() {
+    local f l
     wlog "do_wep '$1' '$2' '$3'"
     clean_dirs "$PKGPATH"
     [[ $opt_force -ne 0 ]] && set_executable
+    if [[ $PRJNAME == "Odoo" && -d $PKGPATH/tests/logs ]]; then
+      l="!"
+      for f in $PKGPATH/tests/logs/*; do
+        echo "$f" | grep -Eq ".*${PKGNAME}_[0-9]{8}.txt$" && [[ $f > $l ]] && l="$f"
+      done
+      for f in $PKGPATH/tests/logs/*; do
+        echo "$f" | grep -Eq ".*${PKGNAME}_[0-9]{8}.txt$" && [[ $f != $l ]] && run_traced "rm -f $f"
+      done
+    fi
     return 0
 }
 
 OPTOPTS=(h        B       b          C        c         D         d        f         k        L         m       n           o        O       p         q           r     t         u       V           v)
 OPTLONG=(help     debug   branch     config   odoo-conf from-date database force     keep     log       ""      dry-run     ""       ""      ""        quiet       ""    test      ""      version     verbose)
 OPTDEST=(opt_help opt_dbg opt_branch opt_conf opt_ocfn  opt_date  opt_db   opt_force opt_keep opt_log   opt_mis opt_dry_run opt_ids  opt_oca opt_dpath opt_verbose opt_r test_mode opt_uop opt_version opt_verbose)
 OPTACTI=("+"      "+"     "="        "="      "="       "="       "="      1         1        "="       1       1           "=>"     1       "="       0           1     1         1       "*"         "+")
@@ -2070,26 +1662,31 @@
 OPTARGS=(actions sub1 sub2 sub3 sub4 sub5 sub6 sub7 sub8 sub9)
 
 parseoptargs "$@"
 if [[ "$opt_version" ]]; then
   echo "$__version__"
   exit 0
 fi
-HLPCMDLIST="help|build|chkconfig|config|docs|duplicate|edit|export|import|lint|list|lsearch|publish|push|pythonhosted|replace|replica|show|test|translate|version|wep"
+HLPCMDLIST="help|chkconfig|config|docs|duplicate|edit|export|import|lint|list|lsearch|publish|push|pythonhosted|replace|replica|show|test|translate|version|wep"
 if [[ $opt_help -gt 0 ]]; then
   print_help "Developer shell\nAction may be on of:\n$HLPCMDLIST" \
     "© 2015-2023 by zeroincombenze®\nhttps://zeroincombenze-tools.readthedocs.io/\nAuthor: antoniomaria.vigliotti@gmail.com"
   exit 0
 fi
 
-opts_travis
+ACT2VME="^(dir|info|show|install|libdir|update|update\+replace|update)$"
+ACT2PYPI="^(docs|git-add|list|replace|travis|travis-summary|version)$"
+ACT2TOOLS="^(docs|git-add|list|replace|travis|travis-summary|version)$"
+PKGS_LIST="clodoo lisa odoo_score os0 python-plus travis_emulator wok_code z0bug-odoo z0lib zar zerobug"
+PKGS_LIST_RE="(${PKGS_LIST// /|})"
+PKGS_LIST_RE=${PKGS_LIST_RE//-/.}
+
+# opts_travis
 conf_default
 [[ $opt_verbose -gt 2 ]] && set -x
-# init_travis
-# prepare_env_travis
 
 sts=$STS_SUCCESS
 sts_bash=127
 sts_flake8=127
 sts_pylint=127
 test_sts=127
 [[ -n $LGITPATH && $PKGNAME == "tools" && $LGITPATH =~ "tools" ]] && LGITPATH=$(dirname $LGITPATH)
@@ -2103,23 +1700,33 @@
 if [[ "$actions" == "help" ]]; then
   man $(dirname $0)/man/man8/$(basename $0).8.gz
 else
   [[ "$PRJNAME" == "Odoo" ]] && odoo_fver=$(build_odoo_param FULLVER ".")
   actions=${actions//+/ }
   actions=${actions//,/ }
   for action in $actions; do
-    if [[ "${action:0:3}" == "if-" ]]; then
-      opt_dry_run=1
-      cmd="do_${action:3}"
-    else
-      cmd="do_${action/-/_}"
-    fi
+    [[ "${action:0:3}" == "if-" ]] && opt_dry_run=1 && cmd="do_${action:3}"
+    cmd="do_${action/-/_}"
     if [[ "$(type -t $cmd)" == "function" ]]; then
-      eval $cmd "'$sub1'" "'$sub2'" "'$sub3'"
-      sts=$?
+      if [[ $PRJNAME == "pypi" && $PKGNAME == "pypi" ]]; then
+        [[ ! $action =~ $ACT2PYPI ]] && echo "Action $action not applicable on this directory" && continue
+        [[ $action =~ $ACT2TOOLS ]] && pkgs_list="$PKGS_LIST tools" || pkgs_list="$PKGS_LIST"
+        for fn in $pkgs_list; do
+          echo -e "\n===[$fn]==="
+          pfn="${fn/-/_}"
+          [[ $fn == "tools" ]] && run_traced "pushd $HOME_DEVEL/pypi/$pfn >/dev/null" || run_traced "pushd $HOME_DEVEL/pypi/$pfn/$pfn >/dev/null"
+          eval $cmd "'$sub1'" "'$sub2'" "'$sub3'"
+          sts=$?
+          run_traced "popd >/dev/null"
+          [[ $sts -ne $STS_SUCCESS ]] && break
+        done
+      else
+        eval $cmd "'$sub1'" "'$sub2'" "'$sub3'"
+        sts=$?
+      fi
     else
       echo "Invalid action!"
       echo "Use $THIS $HLPCMDLIST"
       sts=$STS_FAILED
     fi
     [[ $sts -ne $STS_SUCCESS ]] && break
   done
```

### Comparing `wok_code-2.0.4/wok_code/scripts/to_pep8.py` & `wok_code-2.0.6/wok_code/scripts/to_pep8.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 except ImportError:
     import z0lib
 try:
     from python_plus.python_plus import _c, _u
 except ImportError:
     from python_plus import _c, _u
 
-__version__ = "2.0.4"
+__version__ = "2.0.6"
 
 LICENSES = ('gpl', 'agpl', 'lgpl', 'opl', 'oee')
 METAS = ('0', '6.1', '7.0', '8.0', '9.0', '10.0', '11.0', '12.0', '13.0', '14.0')
 AUTHORS_TEMPLATE = """
 * LibrERP enterprise network <LibrERP-network>
 * SHS-AV s.r.l. <https://www.zeroincombenze.it>
 * Didotech s.r.l. <https://www.didotech.com>
```

### Comparing `wok_code-2.0.4/wok_code/scripts/setup.info` & `wok_code-2.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     install_requires.append('translators')
     install_requires.append('twine')
 else:
     install_requires.append('twine==1.15.0')
 
 setup(
     name='wok_code',
-    version='2.0.4',
+    version='2.0.6',
     description='Python developers tools',
     long_description="""
 Various tools at your fingertips.
 
 The available tools are:
 
 * cvt_csv_2_rst.py: convert csv file into rst file
@@ -55,22 +55,24 @@
     install_requires=install_requires,
     packages=find_packages(exclude=['docs', 'examples', 'tests', 'egg-info', 'junk']),
     package_data={
         '': [
             'scripts/setup.info',
             'scripts/dist_pkg.sh',
             'scripts/please.sh',
+            'scripts/config/*',
             './please.man',
             './cvt_script',
             './cvt_script.man',
             './topep8',
             './to_oca.2p8',
             './to_zero.2p8',
             './to_pep8.2p8',
             './pypi.sh',
+            './install_python_3_from_source.sh',
         ]
     },
     entry_points={
         'console_scripts': [
             'wok_code-info = wok_code.scripts.main:main',
             'cvt_csv_2_rst.py = wok_code.scripts.cvt_csv_2_rst:main',
             'cvt_csv_coa = wok_code.scripts.cvt_csv_coa:main',
@@ -82,11 +84,12 @@
             'lint_2_compare = wok_code.scripts.lint_2_compare:main',
             'makepo_it.py = wok_code.scripts.makepo_it:main',
             'odoo_dependencies.py = wok_code.scripts.odoo_dependencies:main',
             'odoo_translation.py = wok_code.scripts.odoo_translation:main',
             'please = wok_code.scripts.please:main',
             'to_pep8.py = wok_code.scripts.to_pep8:main',
             'wget_odoo_repositories.py = wok_code.scripts.wget_odoo_repositories:main',
+            'run_odoo_debug = odoo_score.scripts.run_odoo_debug:main',
         ]
     },
     zip_safe=False,
 )
```

### Comparing `wok_code-2.0.4/wok_code/scripts/main.py` & `wok_code-2.0.6/wok_code/scripts/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import os
 import sys
 import pkg_resources
 import gzip
 import shutil
 
 
-__version__ = "2.0.4"
+__version__ = "2.0.6"
 
 
 def fake_setup(**kwargs):
     globals()["setup_args"] = kwargs
 
 
 def read_setup():
```

### Comparing `wok_code-2.0.4/wok_code/scripts/makepo_it.py` & `wok_code-2.0.6/wok_code/scripts/makepo_it.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from __future__ import print_function
 
 import os.path
 import sys
 import argparse
 # import pdb
 
-__version__ = "2.0.4"
+__version__ = "2.0.6"
 
 PO_DEFAULT = """
 # Translation of Odoo Server.
 # This file contains the translation of the following modules:
 #   * MODULE
 #
 msgid ""
```

### Comparing `wok_code-2.0.4/wok_code/scripts/cvt_csv_coa.py` & `wok_code-2.0.6/wok_code/scripts/cvt_csv_coa.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 import argparse
 import time
 
 from os0 import os0
 from python_plus import unicodes
 from clodoo import transodoo
 
-__version__ = "2.0.4"
+__version__ = "2.0.6"
 
 msg_time = time.time()
 VALID_ACTIONS = ("export-comparable", "export-full", "export-z0bug", "export-group")
 VERSIONS = ["6.1", "7.0", "8.0", "9.0", "10.0", "11.0", "12.0", "13.0", "14.0"]
 
 
 class CvtCsvFile(object):
```

### Comparing `wok_code-2.0.4/wok_code/scripts/dist_pkg.sh` & `wok_code-2.0.6/wok_code/scripts/dist_pkg.sh`

 * *Files 2% similar despite different names*

```diff
@@ -35,26 +35,24 @@
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
 
-__version__=2.0.4
+__version__=2.0.6
 
 # main
 OPTOPTS=(h        C         c        D        F         f         n            O         o        P         p         q           R         S        u       V           v           W          w         -)
 OPTDEST=(opt_help opt_cpush opt_conf opt_push opt_fetch opt_force opt_dry_run  opt_cpush opt_ids  opt_cpush opt_dpath opt_verbose opt_cpush opt_sts  opt_upd opt_version opt_verbose opt_whatis opt_cpush opt_sync)
 OPTACTI=("+"      "*>"      "="      "*>"     "1>"      1         1            "*>"      "=>"     "*>"      "="       0           "*>"      "=>"     1       "*"         "+"         "=>"       "*>"      "1>")
 OPTDEFL=(1        ""        ""       ""       0         0         0            ""        ""       ""        ""        0           ""        ""       0       ""          -1          ""         ""        0)
 OPTMETA=("help"   "commit"  "file"   ""       "fetch"   ""        "do nothing" ""        "prj_id" "push"    "path"    "quiet"     "replace" "status" "upd"   "version"   "verbose"   "param"    "wep"     "sync")
```

### Comparing `wok_code-2.0.4/wok_code/scripts/generate_random_codes.py` & `wok_code-2.0.6/wok_code/scripts/generate_random_codes.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import sys
 # import os
 import argparse
 from random import random, randint
 import vatnumber
 
 
-__version__ = "2.0.4"
+__version__ = "2.0.6"
 
 
 def gen_vatnumber(opt_args):
     found = False
     while not found:
         seed = "%7.7s%3.03i" % (random() * 10000000, randint(1, 99))
         for i in range(10):
```

### Comparing `wok_code-2.0.4/wok_code/scripts/wget_odoo_repositories.py` & `wok_code-2.0.6/wok_code/scripts/wget_odoo_repositories.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,28 +21,29 @@
 #     from z0lib.z0lib import z0lib
 # except ImportError:
 #     try:
 #         from z0lib import z0lib
 #     except ImportError:
 #         import z0lib
 
-__version__ = '2.0.4'
+__version__ = '2.0.6'
 
 ROOT_URL = 'https://api.github.com/repos/zeroincombenze/'
 USER_URL = 'https://api.github.com/users/'
 REPNAME_ACC_CLO = 'OCB'
 DEVEL_REPS = [
     'Odoo-samples',
     'VME',
     'OpenUpgrade',
     'dotnet',
     'grymb',
     'interface-github',
     'odoorpc',
     'openupgradelib',
+    'project-agile',
     'pylint-odoo',
     'python-plus',
     'rest-framework',
     'runbot-addons',
     'z0bug_odoo',
     'zerobug',
     'zeroincombenze',
@@ -610,15 +611,15 @@
                         ]
                     if not branches or not any(
                         [x for x in branches if x['name'] == opt_args.odoo_vid]
                     ):
                         continue
                 add_repo(name)
             elif opt_args.verbose:
-                print('discaded %s' % name)
+                print('discarded %s' % name)
 
     if repositories:
         cache[git_org] = cache.get(git_org, {})
         cache[git_org][opt_args.odoo_vid] = repositories
         with open(fn, 'w') as fd:
             fd.write(str(cache))
     elif git_org in cache and opt_args.odoo_vid in cache[git_org]:
```

### Comparing `wok_code-2.0.4/wok_code/scripts/dist_pkg.py` & `wok_code-2.0.6/wok_code/scripts/dist_pkg.py`

 * *Files identical despite different names*

### Comparing `wok_code-2.0.4/wok_code/scripts/odoo_translation_old.py` & `wok_code-2.0.6/wok_code/scripts/odoo_translation_old.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     from z0lib import z0lib
 try:
     from clodoo import clodoo
 except ImportError:
     import clodoo
 
 
-__version__ = "2.0.4"
+__version__ = "2.0.6"
 
 MAX_RECS = 100
 PUNCT = [' ', '.', ',', '!', ':']
 TNL_DICT = {}
 TNL_ACTION = {}
 SYNTAX = {'string': re.compile('"([^"\\\n]|\\.|\\\n)*"')}
 VERSIONS = ('16.0', '15.0', '14.0', '13.0', '12.0', '11.0',
```

### Comparing `wok_code-2.0.4/wok_code/scripts/gen_readme.py` & `wok_code-2.0.6/wok_code/scripts/gen_readme.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 
 This software generates the README.rst of OCB, repository and modules.
 It also generates the index.html of the module.
 
 Document may contains macro which format is {{macro_name}}.
 Currently, the follow macros are recognized:
 
-acknowledges
+acknowledges    People acknowledge list
 authors         Authors list
 available_addons
 branch          Odoo version for this repository/module
 certifications  Certificates list
 contact_us
 contributors    Contributors list
 configuration   How to configure
 copyright_notes
 description     English description of the repository/module (mandatory)
 descrizione     Descrizione modulo/progetto in italiano (obbligatoria)
 doc-URL         URL for button documentation
-faq             FAG
+faq             FAQ
 features        Features of the repository/module
 GPL             same of gpl
 git_orgid       Git organization
 gpl             License name: may be A-GPL or L-GPL
 grymb_image_*   Symbol imagae (suffix is a supported symbol name)
 help-URL        URL for button help
 history         Changelog history
@@ -113,15 +113,15 @@
     from python_plus.python_plus import _b, _c, _u
 except ImportError:
     from python_plus import _b, _c, _u
 # import pdb
 standard_library.install_aliases()
 
 
-__version__ = "2.0.4"
+__version__ = "2.0.6"
 
 RED = "\033[1;31m"
 GREEN = "\033[1;32m"
 YELLOW = "\033[1;33m"
 CLEAR = "\033[0;m"
 GIT_USER = {
     "zero": "zeroincombenze",
@@ -2227,14 +2227,15 @@
     parser.add_argument(
         "-w", "--suppress-warning", action="store_true", dest="suppress_warning"
     )
     parser.add_argument(
         "-Y", "--write-man-page", action="store_true", dest="write_man_page"
     )
     ctx = unicodes(parser.parseoptargs(sys.argv[1:]))
+
     ctx["path_name"] = os.path.abspath(ctx["path_name"])
     if not ctx["product_doc"]:
         if "/pypi/" in ctx["path_name"] or ctx["path_name"].endswith("/tools"):
             ctx["product_doc"] = "pypi"
         else:
             ctx["product_doc"] = "odoo"
     if ctx["product_doc"] == "pypi":
@@ -2309,7 +2310,11 @@
                 ctx["odoo_layer"] = "repository"
         else:
             if os.path.isfile(os.path.join(ctx["path_name"], "../setup.py")):
                 ctx["odoo_layer"] = "module"
             else:
                 ctx["odoo_layer"] = "repository"
     return generate_readme(ctx)
+
+
+if __name__ == "__main__":
+    exit(main())
```

### Comparing `wok_code-2.0.4/wok_code/scripts/lint_2_compare.py` & `wok_code-2.0.6/wok_code/scripts/lint_2_compare.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import sys
 import argparse
 from lxml import etree
 
 from python_plus import _b, _u
 from z0lib import z0lib
 
-__version__ = "2.0.4"
+__version__ = "2.0.6"
 
 
 IGNORE_DIRS = (".idea", ".git", "egg-info", "setup")
 
 
 def get_names(left_path, right_path):
     left_base = right_base = ''
@@ -28,15 +28,15 @@
     return left_base, right_base
 
 
 def format_xml(opt_args, source, target):
     with open(source, "r") as fd:
         try:
             root = etree.XML(_b(fd.read()))
-        except SyntaxError as e:
+        except BaseException as e:
             print("%s: ***** Error %s *****" % (source, e))
             root = None
             xml_text = None
     if root is not None:
         try:
             xml_text = _u(etree.tostring(root, pretty_print=True))
         except SyntaxError as e:
```

### Comparing `wok_code-2.0.4/wok_code/scripts/deploy_odoo.py` & `wok_code-2.0.6/wok_code/scripts/deploy_odoo.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,17 +27,17 @@
     from wok_code.scripts.wget_odoo_repositories import main as get_list_from_url
 try:
     from clodoo.clodoo import build_odoo_param
 except ImportError:
     from clodoo import build_odoo_param
 
 
-__version__ = "2.0.4"
+__version__ = "2.0.6"
 
-MANIFEST_FILES = ['__manifest__.py', '__odoo__.py', '__openerp__.py', '__terp__.py']
+MANIFEST_FILES = ["__manifest__.py", "__odoo__.py", "__openerp__.py", "__terp__.py"]
 
 ODOO_VALID_VERSIONS = (
     "16.0",
     "15.0",
     "14.0",
     "13.0",
     "12.0",
@@ -108,25 +108,26 @@
     "oca": "OCA",
     "librerp": "LibrERP-network",
 }
 FMT_PARAMS = {
     "repo": "%(repo)-30.30s",
     "sts": "%(sts)3.3s",
     "branch": "%(branch)-10.10s",
-    "dbranch": "%(branch)-10.10s",
-    "git_org": "%(git_org)-12.12s",
-    "git_url": "%(git_url)-60.60s",
-    "path": "%(path)-48.48s",
+    "dif_branch": "%(branch)-10.10s",
+    "git_org": "%(git_org)-14.14s",
+    "git_url": "%(git_url)-64.64s",
+    "path": "%(path)-56.56s",
     "stash": "%(stash)5.5s",
+    "status": "%(status)s",
 }
 
 
 class OdooDeploy(object):
     """Odoo organization/branch repositories
-    self.repo_list is the reposiotries list of self.repo_info
+    self.repo_list is the repositories list of self.repo_info
     self.repo_info contains repository information
     * BRANCH: git branch
     * PATH: repository path
     * URL: git URL
     * GIT_ORG: git organization
     * STS: os status
     """
@@ -135,223 +136,303 @@
         self.opt_args = opt_args
         self.opt_args.git_orgs = self.opt_args.git_orgs or []
         self.get_addons_from_config_file()
         self.addons_path = []
         self.master_branch = ""
         self.target_path = ""
 
-        if self.opt_args.action == "create-new":
+        if self.opt_args.action in ("clone", "reclone"):
+            if not self.opt_args.odoo_branch:
+                print("***** Missing Odoo branch: 12.0 will be used!")
+                self.opt_args.odoo_branch = "12.0"
+            if not self.opt_args.git_orgs:
+                print("***** Missing git orgs: oca will be used!")
+                self.opt_args.git_orgs = ["oca"]
+
+        if self.opt_args.action == "clone":
             self.master_branch = build_odoo_param(
-                "FULLVER", odoo_vid=opt_args.odoo_branch)
+                "FULLVER", odoo_vid=opt_args.odoo_branch
+            )
+        if (
+            self.opt_args.action in ("clone", "reclone")
+            and not self.opt_args.repos
+        ):
             for git_org in opt_args.git_orgs:
                 self.get_repo_from_github(git_org=git_org)
             if "OCB" not in self.repo_list:
                 git_org = "odoo"
                 self.get_repo_from_github(git_org=git_org, only_ocb=True)
             if opt_args.link_oca and "oca" not in self.opt_args.git_orgs:
                 self.get_repo_from_github(git_org="oca")
 
+        if self.opt_args.repos:
+            self.get_repo_from_switch()
+
         if not self.repo_list and not self.opt_args.target_path:
             self.get_repo_from_config()
 
         if not self.repo_list:
-            self.target_path = self.opt_args.target_path
+            self.target_path = os.path.expanduser(self.opt_args.target_path)
             self.get_repo_from_path()
 
         for repo in self.repo_list:
             path = self.repo_info[repo]["PATH"]
-            git_org = (self.opt_args.git_orgs[0]
-                       if self.opt_args.git_orgs else "oca")
+            git_org = self.opt_args.git_orgs[0] if self.opt_args.git_orgs else "oca"
             if os.path.isdir(path):
                 z0lib.run_traced("cd %s" % path, verbose=False, dry_run=False)
                 sts, repo_branch, git_url, stash_list = self.get_remote_info(
-                    verbose=False)
+                    verbose=False
+                )
                 if sts == 0:
                     org_url, rrepo, git_org = self.data_from_url(git_url)
                 self.repo_info[repo]["GIT_ORG"] = git_org
                 self.repo_info[repo]["URL"] = git_url
                 self.repo_info[repo]["BRANCH"] = repo_branch
                 self.repo_info[repo]["STS"] = sts
                 if stash_list:
                     self.repo_info[repo]["STASH"] = stash_list
             if git_org and git_org not in self.opt_args.git_orgs:
                 self.opt_args.git_orgs.append(git_org)
             if repo == "OCB" or not self.master_branch:
                 self.master_branch = build_odoo_param(
-                    "FULLVER", odoo_vid=self.repo_info[repo]["BRANCH"])
+                    "FULLVER", odoo_vid=self.repo_info[repo]["BRANCH"]
+                )
             if opt_args.action in ("list", "status"):
                 self.add_addons_path(path, repo)
 
         self.git_org = opt_args.git_orgs[0] if opt_args.git_orgs else "oca"
         if self.repo_list:
+            if "OCB" in self.repo_list and self.repo_list[0] != "OCB":
+                del self.repo_list[self.repo_list.index("OCB")]
+                self.repo_list.insert(0, "OCB")
             if self.repo_list[0] == "OCB":
                 self.repo_list = ["OCB"] + sorted(self.repo_list[1:])
             else:
                 self.repo_list = sorted(self.repo_list)
 
     def run_traced(self, cmd, verbose=None):
         verbose = verbose if isinstance(verbose, bool) else self.opt_args.verbose
-        return z0lib.run_traced(cmd, verbose=verbose, dry_run=self.opt_args.dry_run)
+        return z0lib.run_traced(
+            cmd, verbose=verbose, dry_run=self.opt_args.dry_run, disable_alias=True
+        )
 
     def is_module(self, path):
         if not os.path.isdir(path):
             return False
         files = os.listdir(path)
-        filtered = [x for x in files if x in (MANIFEST_FILES + ['__init__.py'])]
-        if len(filtered) == 2 and '__init__.py' in filtered:
-            return os.path.join(path, next(x for x in filtered if x != '__init__.py'))
+        filtered = [x for x in files if x in (MANIFEST_FILES + ["__init__.py"])]
+        if len(filtered) == 2 and "__init__.py" in filtered:
+            return os.path.join(path, next(x for x in filtered if x != "__init__.py"))
         else:
             return False
 
+    def get_git_org_n_url(self, git_org):
+        git_org = git_org or "oca"
+        if git_org.startswith("https:") or git_org.startswith("http:"):
+            git_url = git_org
+            item = git_org.split(":", 1)[1]
+            if item.endswith(".git"):
+                git_org = os.path.basename(os.path.dirname(item))
+            else:
+                git_org = os.path.basename(item)
+            if git_org == "OCA":
+                git_org = "oca"
+        else:
+            if git_org == "zero":
+                git_org = "zeroincombenze"
+            elif git_org == "librerp" and self.opt_args.odoo_branch == "12.0":
+                git_org = "LibrERP-network"
+            elif git_org == "librerp" and self.opt_args.odoo_branch == "6.0":
+                git_org = "iw3hxn"
+            if self.opt_args.use_git:
+                git_url = "git@github.com:%s" % git_org
+            elif git_org == "oca":
+                git_url = "https://github.com/%s" % git_org.upper()
+            else:
+                git_url = "https://github.com/%s" % git_org
+        return git_url, git_org
+
+    def get_repo_from_switch(self):
+        for repo in self.opt_args.repos.split(","):
+            self.repo_info[repo] = {
+                "PATH": self.get_path_of_repo(repo),
+                "#": 1
+            }
+        self.repo_list = sorted(self.repo_info.keys())
+        if "OCB" in self.repo_list:
+            del self.repo_list[self.repo_list.index("OCB")]
+            self.repo_list = ["OCB"] + self.repo_list
+
     def get_repo_from_config(self):
         opt_args = self.opt_args
-        self.master_branch = build_odoo_param(
-            "FULLVER", odoo_vid=opt_args.odoo_branch)
+        self.master_branch = build_odoo_param("FULLVER", odoo_vid=opt_args.odoo_branch)
         if not opt_args.git_orgs:
             opt_args.git_orgs = [
                 build_odoo_param(
                     "GIT_ORGID",
                     odoo_vid=opt_args.odoo_branch,
-                    multi=self.opt_args.multi)
+                    multi=self.opt_args.multi,
+                )
             ]
         for git_org in opt_args.git_orgs:
             if git_org not in ODOO_VALID_GITORGS:
                 print("Invalid git organization: %s" % git_org)
                 exit(1)
         self.git_org = opt_args.git_orgs[0] if opt_args.git_orgs else "oca"
         self.target_path = build_odoo_param(
             "ROOT",
             odoo_vid=opt_args.odoo_branch,
             git_org=self.git_org,
-            multi=self.opt_args.multi)
+            multi=self.opt_args.multi,
+        )
         if re.match(os.environ.get("ODOO_GIT_ORGID", "oca"), git_org):
-            config = os.path.join("/etc/odoo",
-                                  build_odoo_param(
-                                      "CONFN",
-                                      odoo_vid=opt_args.odoo_branch,
-                                      multi=self.opt_args.multi)
-                                  )
+            config = os.path.join(
+                "/etc/odoo",
+                build_odoo_param(
+                    "CONFN", odoo_vid=opt_args.odoo_branch, multi=self.opt_args.multi
+                ),
+            )
         else:
-            config = os.path.join("/etc/odoo",
-                                  build_odoo_param(
-                                      "CONFN",
-                                      odoo_vid=opt_args.odoo_branch,
-                                      git_org=self.git_org,
-                                      multi=self.opt_args.multi)
-                                  )
+            config = os.path.join(
+                "/etc/odoo",
+                build_odoo_param(
+                    "CONFN",
+                    odoo_vid=opt_args.odoo_branch,
+                    git_org=self.git_org,
+                    multi=self.opt_args.multi,
+                ),
+            )
         if os.path.isfile(config):
             self.opt_args.config = config
             self.get_addons_from_config_file()
 
     def get_repo_from_path(self):
+        def analyze_path(path, dir):
+            if self.path_is_ocb(path):
+                self.repo_info["OCB"] = {"PATH": path, "#": 0}
+            elif self.is_git_repo(path=path):
+                self.repo_info[dir] = {"PATH": path, "#": 0}
+                if os.path.islink(path):
+                    self.repo_info[dir]["#"] = 1
+            elif self.is_module(path):
+                repo = os.path.basename(root)
+                if repo == "addons":
+                    repo = os.path.basename(os.path.dirname(root))
+                    if repo in ("odoo", "openerp", os.path.basename(
+                        self.repo_info.get(
+                            "OCB", {}).get("PATH", ""))):
+                        repo = "OCB"
+                if repo in self.repo_info:
+                    self.repo_info[repo]["#"] += 1
+
         if self.target_path:
-            repo = "OCB"
-            if self.is_git_repo(path=self.target_path):
-                self.repo_info[repo] = {"PATH": self.target_path, "#": 0}
-            for root, dirs, files in os.walk(self.target_path,
-                                             topdown=True,
-                                             followlinks=False):
+            # repo = "OCB"
+            # if self.is_git_repo(path=self.target_path):
+            #     self.repo_info[repo] = {"PATH": self.target_path, "#": 0}
+            analyze_path(self.target_path, "OCB")
+            for root, dirs, files in os.walk(
+                self.target_path, topdown=True, followlinks=False
+            ):
+                links = [d for d in dirs if os.path.islink(os.path.join(root, d))]
                 dirs[:] = [
                     d
                     for d in dirs
                     if (
                         not d.startswith(".")
                         and not d.startswith("_")
-                        and not d.endswith('~')
-                        and d not in ("build",
-                                      "debian",
-                                      "dist",
-                                      "doc",
-                                      "docs",
-                                      "egg-info",
-                                      "filestore",
-                                      "history",
-                                      "howtos",
-                                      "images"
-                                      "migrations",
-                                      "redhat",
-                                      "reference",
-                                      "scripts",
-                                      "server",
-                                      "setup",
-                                      "tmp",
-                                      "venv_odoo",
-                                      "win32")
+                        and not d.endswith("~")
+                        and d
+                        not in (
+                            "build",
+                            "debian",
+                            "dist",
+                            "doc",
+                            "docs",
+                            "egg-info",
+                            "filestore",
+                            "history",
+                            "howtos",
+                            "images" "migrations",
+                            "redhat",
+                            "reference",
+                            "scripts",
+                            "server",
+                            "setup",
+                            "static",
+                            "tests",
+                            "tmp",
+                            "venv_odoo",
+                            "win32",
                         )
+                        and not os.path.islink(os.path.join(root, d))
+                    )
                 ]
-                for dir in dirs:
+                for dir in dirs + links:
                     path = os.path.join(root, dir)
-                    if self.path_is_ocb(path):
-                        self.repo_info["OCB"] = {"PATH": path, "#": 0}
-                    elif self.is_git_repo(path=path):
-                        self.repo_info[dir] = {"PATH": path, "#": 0}
-                    elif self.is_module(path):
-                        repo = os.path.basename(root)
-                        if repo == "addons":
-                            repo = os.path.basename(os.path.dirname(root))
-                            if repo == "odoo":
-                                repo = "OCB"
-                        if repo in self.repo_info:
-                            self.repo_info[repo]["#"] += 1
+                    analyze_path(path, dir)
             for repo in [x for x in self.repo_info.keys()]:
                 if self.repo_info[repo]["#"] == 0:
                     del self.repo_info[repo]
             self.repo_list = sorted(self.repo_info.keys())
             if "OCB" in self.repo_list:
                 del self.repo_list[self.repo_list.index("OCB")]
                 self.repo_list = ["OCB"] + self.repo_list
 
     def get_repo_from_github(self, git_org=None, branch=None, only_ocb=None):
         git_org = git_org or self.git_org
         branch = branch or self.opt_args.odoo_branch
         if self.opt_args.target_path:
-            self.target_path = self.opt_args.target_path
+            self.target_path = os.path.expanduser(self.opt_args.target_path)
         else:
             self.target_path = build_odoo_param(
-                "ROOT",
-                odoo_vid=branch,
-                git_org=git_org,
-                multi=self.opt_args.multi)
-        hash_key = git_org + branch.split(".")[0]
-        if self.opt_args.action == "create-new":
-            opts = []
-            if self.opt_args.verbose:
-                opts.append("-v")
-            if self.opt_args.dry_run:
-                opts.append("-D")
-            if branch:
-                opts.append("-b")
-                opts.append(branch)
-            opts.append("-l")
-            opts.append("l10n-italy,l10n-italy-supplemental")
-            opts.append("-G")
-            opts.append(
-                SHORT_NAMES.get(git_org, git_org)
+                "ROOT", odoo_vid=branch, git_org=git_org, multi=self.opt_args.multi
             )
-            opts.append("--return-repos")
-            if only_ocb:
-                content = ["OCB"]
-            else:
-                content = get_list_from_url(opts)
-            for repo in content:
-                if repo not in self.repo_list:
-                    url = DEFAULT_DATA.get(hash_key, {}).get(repo)
-                    if not url:
-                        url = DEFAULT_DATA.get(hash_key, {}).get("URL")
-                    if not url:
-                        url = "https://github.com/%s" % REPO_NAMES.get(git_org, git_org)
-                    url = "%s/%s.git" % (url, repo)
-                    tgtdir = self.get_path_of_repo(repo)
-                    self.repo_list.append(repo)
-                    self.repo_info[repo] = {
-                        "GIT_ORG": git_org,
-                        "BRANCH": branch,
-                        "URL": url,
-                        "PATH": tgtdir,
-                    }
+        hash_key = git_org + branch.split(".")[0]
+        opts = []
+        if self.opt_args.verbose:
+            opts.append("-v")
+        if self.opt_args.dry_run:
+            opts.append("-D")
+        if branch:
+            opts.append("-b")
+            opts.append(branch)
+        opts.append("-l")
+        opts.append(self.opt_args.local_reps)
+        # opts.append("l10n-italy,l10n-italy-supplemental")
+        opts.append("-G")
+        opts.append(SHORT_NAMES.get(git_org, git_org))
+        if self.opt_args.extra:
+            opts.append("-x")
+            opts.append(self.opt_args.extra)
+        opts.append("--return-repos")
+        if only_ocb:
+            content = ["OCB"]
+        else:
+            content = get_list_from_url(opts)
+        for repo in content:
+            if repo not in self.repo_list:
+                url = DEFAULT_DATA.get(hash_key, {}).get(repo)
+                if not url:
+                    url = DEFAULT_DATA.get(hash_key, {}).get("URL")
+                if not url:
+                    if self.opt_args.use_git:
+                        url = "git@github.com:%s" % REPO_NAMES.get(git_org, git_org)
+                    else:
+                        url = "https://github.com/%s" % REPO_NAMES.get(
+                            git_org, git_org
+                        )
+                url = "%s/%s.git" % (url, repo)
+                tgtdir = self.get_path_of_repo(repo)
+                self.repo_list.append(repo)
+                self.repo_info[repo] = {
+                    "GIT_ORG": git_org,
+                    "BRANCH": branch,
+                    "URL": url,
+                    "PATH": tgtdir,
+                }
 
     def data_from_url(self, url):
         if "git@github.com:" in url:
             path = url.split(":")[1]
             uri = url.split("@")[1].split(":")[1]
         elif "@bzr." in url and ":" in url:
             path = url.split(":")[1]
@@ -359,15 +440,15 @@
         elif "https:" in url:
             path = url.split(":")[1]
             uri = url.split(":")[1]
         else:
             path = uri = url
         repo = os.path.basename(path)
         if repo.endswith(".git"):
-            repo = repo[: -4]
+            repo = repo[:-4]
             url = os.path.dirname(url)
         if repo == "odoo":
             repo = "OCB"
         if uri.startswith("bzr"):
             git_org = os.path.splitext(uri[4:])[0]
         else:
             git_org = os.path.splitext(os.path.basename(os.path.dirname(uri)))[0]
@@ -388,34 +469,36 @@
             config = ConfigParser.ConfigParser()
             config.read(self.opt_args.config)
             for path in config.get("options", "addons_path").split(","):
                 if self.is_git_repo(path=path):
                     repo = os.path.basename(path)
                     add_repo(repo, path)
                     continue
-                if (
-                    os.path.basename(path) == "addons"
-                    and os.path.isdir(os.path.join(path, "..", ".git"))
+                if os.path.basename(path) == "addons" and os.path.isdir(
+                    os.path.join(path, "..", ".git")
                 ):
                     path = os.path.dirname(path)
                 if not os.path.isdir(path):
                     print("Path %s does not exist!" % path)
                     continue
                 if not self.is_git_repo(path=path):
                     continue
                 add_repo("OCB", path)
 
     def find_data_dir(self, canonicalize=None):
+        if self.master_branch and int(self.master_branch.split(".")[0]) < 8:
+            return False
         tgtdir = os.path.join(os.environ["HOME"], ".local")
         if os.path.isdir(tgtdir):
             tgtdir = os.path.join(tgtdir, "share")
             if not os.path.isdir(tgtdir) and canonicalize:
                 os.mkdir(tgtdir)
             odoo_master_branch = build_odoo_param(
-                "FULLVER", odoo_vid=self.opt_args.odoo_branch)
+                "FULLVER", odoo_vid=self.opt_args.odoo_branch
+            )
             base = "Odoo%s" % odoo_master_branch.split(".")[0]
             tgtdir = os.path.join(tgtdir, base)
             if not os.path.isdir(tgtdir) and canonicalize:
                 os.mkdir(tgtdir)
             for base in ("addons", "filestore", "sessions"):
                 tgt = os.path.join(tgtdir, base)
                 if not os.path.isdir(tgt) and canonicalize:
@@ -433,48 +516,45 @@
                     content = fd.read()
             updated = False
             for repo in repos:
                 if repo == "OCB":
                     continue
                 if ("\n%s\n" % repo) in content or ("\n/%s\n" % repo) in content:
                     continue
-                content += ("/%s\n" % repo)
+                content += "/%s\n" % repo
                 updated = True
             if updated and not self.opt_args.dry_run:
                 with open(gitignore_fn, "w") as fd:
                     fd.write(content)
 
     def update_conf(self, addons_path=None, git_org=None, branch=None):
         addons_path = addons_path or self.addons_path
         if addons_path:
             data_dir = self.find_data_dir(canonicalize=True)
             if os.path.isfile(self.opt_args.config):
                 config = ConfigParser.ConfigParser()
                 config.read(self.opt_args.config)
                 config.set("options", "addons_path", ",".join(addons_path))
-                config.set("options", "data_dir", data_dir)
+                if data_dir:
+                    config.set("options", "data_dir", data_dir)
                 if not self.opt_args.dry_run:
                     config.write(open(self.opt_args.config, "w+"))
 
     def is_git_repo(self, repo=None, path=None):
         res = bool(repo)
         if repo:
             res = False
             if repo.startswith(".") or repo.startswith("_") or repo in INVALID_NAMES:
                 path = None
             elif not path:
                 path = self.get_path_of_repo(repo)
         if path:
             path = os.path.join(path, repo) if repo else path
-            if (
-                os.path.isdir(os.path.join(path, ".git"))
-                or (not res
-                    and repo
-                    and self.repo_is_ocb(repo)
-                    and self.path_is_ocb(path))
+            if os.path.isdir(os.path.join(path, ".git")) or (
+                not res and repo and self.repo_is_ocb(repo) and self.path_is_ocb(path)
             ):
                 res = path
         return res
 
     def get_alt_gitorg(self, git_org=None):
         git_org = git_org or self.git_org
         return {
@@ -484,27 +564,38 @@
         }.get(git_org)
 
     def repo_is_ocb(self, repo):
         return repo in ("OCB", "odoo")
 
     def path_is_ocb(self, path):
         if (
-            os.path.isfile(os.path.join(path, "odoo-bin"))
-            or os.path.isfile(os.path.join(path, "openerp-server"))
+            os.path.isdir(os.path.join(path, ".git"))
+            and os.path.isdir(os.path.join(path, "addons"))
+            and (
+                (
+                    os.path.isfile(os.path.join(path, "odoo-bin"))
+                    and os.path.isdir(os.path.join(path, "odoo"))
+                )
+                or (
+                    os.path.isfile(os.path.join(path, "openerp-server"))
+                    and os.path.isdir(os.path.join(path, "openerp"))
+                )
+            )
         ):
             return True
         return False
 
     def get_path_of_repo(self, repo):
         tgtdir = self.repo_info.get(repo, {}).get("PATH")
         if not tgtdir:
             if self.repo_is_ocb(repo):
                 tgtdir = self.target_path
             else:
-                tgtdir = os.path.join(self.target_path, repo)
+                tgtdir = os.path.join(self.target_path or self.opt_args.target_path,
+                                      repo)
         return tgtdir
 
     def get_remote_info(self, verbose=True):
         verbose = verbose and self.opt_args.verbose
         branch = self.master_branch
         stash_list = ""
         url = None
@@ -547,15 +638,15 @@
                         continue
                     repo = os.path.basename(path)
                     if not self.is_git_repo(repo):
                         repos.append(repo)
                         dname = os.path.dirname(path)
                         if dname not in dirnames:
                             dirnames[dname] = 0
-                        dirnames[dname] += (2 if repo == "addons" else 1)
+                        dirnames[dname] += 2 if repo == "addons" else 1
                 break
         root = False
         ctr = 0
         for dname in dirnames.keys():
             if dirnames[dname] > ctr:
                 root = dname
                 ctr = dirnames[dname]
@@ -579,20 +670,28 @@
             for base in ("odoo", "openerp"):
                 if os.path.isdir(os.path.join(tgtdir, base)):
                     path = os.path.join(tgtdir, base, "addons")
                     break
             if path:
                 self.addons_path.append(path)
             self.addons_path.append(os.path.join(tgtdir, "addons"))
-            self.addons_path.append(self.find_data_dir())
+            data_dir = self.find_data_dir()
+            if data_dir:
+                self.addons_path.append(data_dir)
         else:
             self.addons_path.append(tgtdir)
 
     def git_clone(
-        self, git_url, tgtdir, branch, master_branch=None, compact=None, link_oca=None,
+        self,
+        git_url,
+        tgtdir,
+        branch,
+        master_branch=None,
+        compact=None,
+        link_oca=None,
     ):
         root = os.path.dirname(tgtdir)
         base = os.path.basename(tgtdir)
         if os.getcwd() != root:
             cmd = "cd %s" % root
             self.run_traced(cmd)
         remote_branch = branch
@@ -611,25 +710,29 @@
             sts, stdout, stderr = self.run_traced(cmd)
             if sts == 0 or self.opt_args.dry_run and "devel" in branch:
                 remote_branch = alt_branch
                 break
         if sts and link_oca and self.opt_args.link_oca:
             git_org = "oca"
             srcdir = build_odoo_param(
-                "ROOT", odoo_vid=branch, multi=self.opt_args.multi, git_org=git_org)
+                "ROOT", odoo_vid=branch, multi=self.opt_args.multi, git_org=git_org
+            )
             if os.path.isdir(srcdir):
                 sts, stdout, stderr = self.run_traced("ln -s %s %s" % (srcdir, tgtdir))
                 remote_branch = branch
         if sts:
             print("Invalid branch %s" % branch)
         return sts, remote_branch
 
     def git_pull(self, tgtdir, branch, master_branch=None):
         if os.getcwd() != tgtdir:
             self.run_traced("cd %s" % tgtdir)
+        if os.path.islink(tgtdir):
+            sts, repo_branch, git_url, stash_list = self.get_remote_info()
+            return sts, repo_branch
         cmd = "git stash"
         self.run_traced(cmd, verbose=False)
         sleep(1)
         sts, repo_branch, git_url, stash_list = self.get_remote_info()
         alt_branches = self.get_alt_branches(branch, master_branch=master_branch)
         if repo_branch != branch and repo_branch not in alt_branches:
             for alt_branch in [branch] + alt_branches:
@@ -660,25 +763,23 @@
             if sts == 0:
                 org_url, repo, repo_org = self.data_from_url(git_url)
         elif self.repo_is_ocb(repo) and not self.opt_args.keep_root_owner:
             git_url = "https://github.com/odoo/odoo.git"
             # repo = "odoo"
         elif repo in self.repo_list:
             repo_branch = self.repo_info[repo].get("BRANCH", branch)
-            git_url = self.repo_info[repo].get("URL")
-            if not git_url:
-                git_url = build_odoo_param(
-                    "GIT_URL",
-                    odoo_vid=repo_branch,
-                    multi=self.opt_args.multi,
-                    git_org=git_org)
+            if repo_branch == "12.0" and git_org == "librerp" and repo == "OCB":
+                git_url = DEFAULT_DATA["librerp12"]["URL"] + "/odoo.git"
+            else:
+                git_url = self.repo_info[repo].get("URL")
+                if not git_url:
+                    git_url, git_org = self.get_git_org_n_url(git_org)
+                    git_url = git_url + "/" + repo + ".git"
         if not git_url:
             return 127
-        # if not git_url.endswith(".git"):
-        #     git_url = "%s/%s.git" % (git_url, repo)
         bakdir = ""
         if os.path.isdir(tgtdir) and self.opt_args.action != "update":
             if self.opt_args.skip_if_exist:
                 return self.git_pull(tgtdir, branch, master_branch=odoo_master_branch)
             elif not self.opt_args.assume_yes:
                 print("Path %s of repo %s already exists!" % (tgtdir, repo))
                 dummy = input("Delete (y/n)? ")
@@ -687,25 +788,29 @@
             if self.repo_is_ocb(repo):
                 bakdir = "%s~" % tgtdir
                 if os.path.isdir(bakdir):
                     cmd = "rm -fR %s" % bakdir
                     self.run_traced(cmd)
                 cmd = "mv %s %s" % (tgtdir, bakdir)
                 self.run_traced(cmd)
-            else:
+            elif not os.path.islink(tgtdir):
                 cmd = "rm -fR %s" % tgtdir
                 self.run_traced(cmd)
         if os.path.isdir(tgtdir) and self.opt_args.action == "update":
             sts, remote_branch = self.git_pull(
-                tgtdir, branch, master_branch=odoo_master_branch)
+                tgtdir, branch, master_branch=odoo_master_branch
+            )
         else:
             sts, remote_branch = self.git_clone(
-                git_url, tgtdir, branch,
+                git_url,
+                tgtdir,
+                branch,
                 master_branch=odoo_master_branch,
-                compact=True if git_org in ("odoo", "oca") else False)
+                compact=True if git_org in ("odoo", "oca") else False,
+            )
         if sts == 0 and not os.path.isdir(tgtdir) and not self.opt_args.dry_run:
             sts = 1
         if repo not in self.repo_list:
             self.repo_list.append(repo)
         self.repo_info[repo]["STS"] = sts
         self.repo_info[repo]["PATH"] = tgtdir
         self.repo_info[repo]["GIT_ORG"] = git_org
@@ -752,58 +857,65 @@
         fmt = fmt.strip()
         print(fmt % datas)
         for repo in self.repo_list:
             datas = {
                 "repo": repo,
                 "sts": self.repo_info[repo].get("STS"),
                 "branch": self.repo_info[repo].get("BRANCH"),
-                "dbranch": self.repo_info[repo].get("BRANCH")
-                if self.repo_info[repo].get("BRANCH") != self.master_branch else "",
+                "dif_branch": self.repo_info[repo].get("BRANCH")
+                if self.repo_info[repo].get("BRANCH") != self.master_branch
+                else "",
                 "git_org": self.repo_info[repo].get("GIT_ORG"),
                 "git_url": self.repo_info[repo].get("URL"),
                 "path": self.repo_info[repo].get("PATH"),
                 "stash": "stash" if self.repo_info[repo].get("STASH") else "",
             }
             print(fmt % datas)
-        print()
-        print(",".join(self.addons_path))
+        if self.opt_args.show_addons:
+            print()
+            print(",".join(self.addons_path))
 
     def list_repo_info(self):
         print("Odoo main version..........: %s" % self.master_branch)
         if self.opt_args.config:
             print("Odoo configuration file....: %s" % self.opt_args.config)
         fmt_list = self.opt_args.format.split(",")
         fmt = ""
         datas = {}
         for item in fmt_list:
             fmt += " " + FMT_PARAMS[item]
             datas[item] = item.upper()
         fmt = fmt.strip()
         print(fmt % datas)
         for repo in self.repo_list:
-            git_org = ""
+            git_org = git_stat = ""
             tgtdir = self.get_path_of_repo(repo)
             self.run_traced("cd %s" % tgtdir, verbose=False)
             sts, repo_branch, git_url, stash_list = self.get_remote_info(verbose=False)
             if sts == 0:
                 org_url, repo, git_org = self.data_from_url(git_url)
+                sts, stdout, stderr = self.run_traced("git status", verbose=False)
+                if sts == 0:
+                    git_stat = stdout
 
             datas = {
                 "repo": repo,
                 "sts": sts,
                 "branch": repo_branch,
-                "dbranch": repo_branch if repo_branch != self.master_branch else "",
+                "dif_branch": repo_branch if repo_branch != self.master_branch else "",
                 "git_org": git_org,
                 "git_url": git_url,
                 "path": tgtdir,
                 "stash": "stash" if self.repo_info[repo].get("STASH") else "",
+                "status": git_stat,
             }
             print(fmt % datas)
-        print()
-        print(",".join(self.addons_path))
+        if self.opt_args.show_addons:
+            print()
+            print(",".join(self.addons_path))
 
     def download_or_pull_repo(self):
         print("Odoo main version..........: %s" % self.master_branch)
         if self.opt_args.config:
             print("Odoo configuration file....: %s" % self.opt_args.config)
         for repo in self.repo_list:
             self.download_single_repo(repo)
@@ -814,92 +926,141 @@
         if self.opt_args.verbose:
             self.list_repo_info()
 
 
 def main(cli_args=None):
     cli_args = cli_args or sys.argv[1:]
     parser = argparse.ArgumentParser(
-        description="Manage Odoo repositories",
-        epilog="© 2021-2023 by SHS-AV s.r.l."
+        description="Manage Odoo repositories", epilog="© 2021-2023 by SHS-AV s.r.l."
+    )
+    parser.add_argument(
+        "-A",
+        "--update-addons-conf",
+        action="store_true",
+        help="Update addons_path in Odoo configuration file",
+    )
+    parser.add_argument(
+        "-a",
+        "--show-addons",
+        action="store_true",
+        help="Show addons_path after action",
     )
-    parser.add_argument("-A", "--update-addons-conf",
-                        action="store_true",
-                        help="Update addons_path in Odoo configuration file")
-    parser.add_argument("-b", "--odoo-branch",
-                        dest="odoo_branch",
-                        default="12.0",
-                        help="Default Odoo version")
-    parser.add_argument("-c", "--config",
-                        help="Odoo configuration file")
+    parser.add_argument(
+        "-b",
+        "--odoo-branch",
+        dest="odoo_branch",
+        default="12.0",
+        help="Default Odoo version",
+    )
+    parser.add_argument("-c", "--config", help="Odoo configuration file")
     parser.add_argument("-D", "--default-gitorg", default="zero")
     # parser.add_argument("-d", "--deployment-mode", help="may be tree,server,odoo")
-    parser.add_argument("-e", "--skip-if-exist", action="store_true")
-    parser.add_argument("-F",
-                        "--format",
-                        help="use 1 or + of sts,repo,branch,git_org,git_url,path,stash",
-                        default="sts,repo,branch,git_org,git_url,path,stash")
-    parser.add_argument("-G", "--git-orgs",
-                        help="Git organizations, comma separated - "
-                             "May be: oca librerp or zero")
-    parser.add_argument("-K", "--keep-root-owner",
-                        action="store_true",
-                        help="keep OCB/odoo organization owner")
-    parser.add_argument("-L", "--list",
-                        action="store_true",
-                        help="deprecated: use 'list' action!")
-    parser.add_argument("-m", "--multi",
-                        action="store_true",
-                        help="Multi version environment")
-    parser.add_argument("-N", "--create-new",
-                        action="store_true",
-                        help="deprecated: use 'create-new' action!")
+    parser.add_argument(
+        "-e", "--skip-if-exist",
+        action="store_true",
+        help="Use this switch  to add missed repositories when you reclone"
+    )
+    parser.add_argument(
+        "-F",
+        "--format",
+        help=("Use 1 or + of " "sts,repo,branch,git_org,git_url,path,stash,status"),
+        default="sts,repo,branch,git_org,git_url,path,stash",
+    )
+    parser.add_argument(
+        "-G",
+        "--git-orgs",
+        help="Git organizations, comma separated - " "May be: oca librerp or zero",
+    )
+    parser.add_argument(
+        "-g",
+        "--use-git",
+        action="store_true",
+        help="When clone use git protocol instead of https",
+    )
+    parser.add_argument(
+        "-K",
+        "--keep-root-owner",
+        action="store_true",
+        help="Keep OCB/odoo organization owner",
+    )
+    parser.add_argument(
+        "-L", "--list", action="store_true", help="Deprecated: use 'list' action!"
+    )
+    parser.add_argument(
+        "-l", "--local-reps",
+        default="l10n-italy,l10n-italy-supplemental",
+        help="Local repositories to load; default: l10n-italy,l10n-italy-supplemental"
+    )
+    parser.add_argument(
+        "-m", "--multi", action="store_true", help="Multi version environment"
+    )
+    parser.add_argument(
+        "-N",
+        "--clone",
+        action="store_true",
+        help="Deprecated: use 'clone' action!",
+    )
     parser.add_argument("-n", "--dry-run", action="store_true")
-    parser.add_argument("-O", "--link-oca",
-                        action="store_true",
-                        help="link to more OCA repositories")
-    parser.add_argument("-p", "--target-path",
-                        help="Local directory")
-    parser.add_argument("-R", "--reclone",
-                        action="store_true",
-                        help="deprecated: use 'reclone' action!")
-    parser.add_argument("-S", "--status",
-                        action="store_true",
-                        help="deprecated: use 'status' action!")
-    parser.add_argument("-U", "--only-update",
-                        action="store_true",
-                        help="deprecated: use 'update' action!")
+    parser.add_argument(
+        "-O", "--link-oca", action="store_true", help="Link to more OCA repositories"
+    )
+    parser.add_argument("-p", "--target-path", help="Local directory")
+    parser.add_argument(
+        "-R", "--reclone", action="store_true", help="Deprecated: use 'reclone' action!"
+    )
+    parser.add_argument(
+        "-r", "--repos",
+        help="Declare specific repositories to managa, comma separated"
+    )
+    parser.add_argument(
+        "-S", "--status", action="store_true", help="Deprecated: use 'status' action!"
+    )
+    parser.add_argument(
+        "-U",
+        "--only-update",
+        action="store_true",
+        help="Deprecated: use 'update' action!",
+    )
     parser.add_argument("-v", "--verbose", action="count", default=0)
     parser.add_argument("-V", "--version", action="version", version=__version__)
+    parser.add_argument(
+        "-x", "--extra",
+        help="May be: all,none,connector,devel,maintainer,oca,odoo,vertical"
+    )
     parser.add_argument("-y", "--assume-yes", action="store_true")
-    parser.add_argument("action",
-                        nargs="?",
-                        help="may be create-new,list,reclone,status,update")
+    parser.add_argument(
+        "action", nargs="?", help="May be clone,list,reclone,status,update"
+    )
     opt_args = parser.parse_args(cli_args)
 
     if not opt_args.action:
-        if opt_args.create_new:
-            opt_args.action = "create-new"
+        if opt_args.clone:
+            opt_args.action = "clone"
         elif opt_args.list:
             opt_args.action = "list"
         elif opt_args.reclone:
             opt_args.action = "reclone"
         elif opt_args.status:
             opt_args.action = "status"
         elif opt_args.only_update:
             opt_args.action = "update"
     opt_args.git_orgs = opt_args.git_orgs.split(",") if opt_args.git_orgs else []
 
     if (
         opt_args.action != "update"
-        and opt_args.action != "create-new"
+        and opt_args.action != "clone"
         and opt_args.action != "reclone"
         and opt_args.action != "list"
         and opt_args.action != "status"
     ):
-        print("No action issued! Please use -U or -N or -R or -L or -S switch")
+        print("No valid action issued!")
+        exit(1)
+
+    if opt_args.repos and not opt_args.target_path:
+        print("No path issued for declared repositories")
         exit(1)
 
     deploy = OdooDeploy(opt_args)
     if opt_args.action == "list":
         deploy.list_data()
     elif opt_args.action == "status":
         deploy.list_repo_info()
```

### Comparing `wok_code-2.0.4/wok_code/scripts/odoo_translation.py` & `wok_code-2.0.6/wok_code/scripts/odoo_translation.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import re
 import collections
 from babel.messages import pofile
 from openpyxl import load_workbook, Workbook
 
 # from python_plus import unicodes
 
-__version__ = "2.0.4"
+__version__ = "2.0.6"
 
 
 MODULE_SEP = "\ufffa"
 
 # (<en>, <it>, <module>, <result>, ovverride)
 TEST_DATA = [
     ("name", "nome", None, "nome"),
@@ -834,22 +834,22 @@
         ):
             self.do_dict_item(msg_orig,
                               msg_tnxl,
                               action="build_dict",
                               is_tag=is_tag)
 
     def build_dict(self):
-        if self.opt_args.file_xlsx:
-            root = self.get_home_devel()
-            if root:
-                dict_name = os.path.join(
-                    root, 'pypi', 'tools', 'odoo_template_tnl.xlsx')
-                if os.path.isfile(dict_name):
-                    self.load_terms_from_xlsx(dict_name)
-            self.load_terms_from_xlsx(self.opt_args.file_xlsx)
+        # if self.opt_args.file_xlsx:
+        #     root = self.get_home_devel()
+        #     if root:
+        #         dict_name = os.path.join(
+        #             root, 'pypi', 'tools', 'odoo_template_tnl.xlsx')
+        #         if os.path.isfile(dict_name):
+        #             self.load_terms_from_xlsx(dict_name)
+        #     self.load_terms_from_xlsx(self.opt_args.file_xlsx)
         if not self.opt_args.module_name:
             target_path = os.path.abspath(self.opt_args.target_path)
             self.do_work_on_path(target_path, None)
             for root, dirs, files in os.walk(target_path,
                                              topdown=True,
                                              followlinks=False):
                 dirs[:] = [
@@ -933,14 +933,15 @@
         "--git-orgs",
         help="Git organizations, comma separated - " "May be: oca librerp or zero",
     )
     parser.add_argument("-l", "--lang", default="it_IT", help="Language")
     parser.add_argument("-m", "--module-name")
     parser.add_argument("-n", "--dry-run", action="store_true")
     parser.add_argument("-p", "--target-path", help="Local directory")
+    parser.add_argument("-q", "--quite", action="store_false")
     parser.add_argument("-T", "--test", action="store_true")
     parser.add_argument("-v", "--verbose", action="count", default=0)
     parser.add_argument("-V", "--version", action="version", version=__version__)
     parser.add_argument("-W", "--rewrite-xlsx",
                         action="store_true",
                         help="Rewrite xlsx file")
     parser.add_argument("-x", "--file-xlsx", help="Default dictionary")
```

### Comparing `wok_code-2.0.4/wok_code/scripts/odoo_dependencies.py` & `wok_code-2.0.6/wok_code/scripts/odoo_dependencies.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
 except ImportError:
     from z0lib import z0lib
 try:
     from clodoo import clodoo
 except ImportError:
     import clodoo
 
-__version__ = '2.0.4'
+__version__ = '2.0.6'
 
 
 MANIFEST_FILES = ['__manifest__.py', '__odoo__.py', '__openerp__.py', '__terp__.py']
 MAX_DEEP = 20
 UNDEF_DEEP = MAX_DEEP + 5
 MISSED = 99
```

### Comparing `wok_code-2.0.4/wok_code/scripts/cvt_csv_2_rst.py` & `wok_code-2.0.6/wok_code/scripts/cvt_csv_2_rst.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 try:
     from z0lib import z0lib
 except ImportError:
     import z0lib
 
 
-__version__ = "2.0.4"
+__version__ = "2.0.6"
 
 msg_time = time.time()
 
 
 def msg_burst(text):
     global msg_time
     t = time.time() - msg_time
```

### Comparing `wok_code-2.0.4/wok_code/scripts/do_odoo_site.py` & `wok_code-2.0.6/wok_code/scripts/do_odoo_site.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 import sys
 import os
 import argparse
-import re
-
+# import re
+try:
+    import ConfigParser
+except ImportError:
+    import configparser as ConfigParser
 
 TEMPLATE = """#############################################
 # Odoo service
 # Domain: <http://%(domain)s>
 #
 <VirtualHost *:80>
     ServerAdmin %(email)s
@@ -72,80 +75,67 @@
     SSLCertificateKeyFile
     Include /etc/letsencrypt/options-ssl-apache.conf
     SSLCertificateChainFile
 </VirtualHost>
 </IfModule>
 """
 
-__version__ = "2.0.4"
+__version__ = "2.0.6"
 
 
 class CreateConfig(object):
 
     def __init__(self, domain, opt_args):
         self.opt_args = opt_args
         if "." in domain:
             self.domain = domain
         else:
             self.domain = "%s.zeroincombenze.it" % domain
+        self.confn = "%s.conf" % self.domain
+
+        self.odoo_config = {}
+        if self.opt_args.odoo_config:
+            if not os.path.isfile(self.opt_args.odoo_config):
+                print("Odoo config file %s not found!" % self.opt_args.odoo_config)
+                return
+            config = ConfigParser.ConfigParser()
+            config.read(self.opt_args.odoo_config)
+            for param in ("http_port", "xmlrpc_port", "longpolling_port"):
+                if config.has_option("options", param):
+                    self.odoo_config[param] = config.getint("options", param)
+
         self.email = "postmaster@%s" % ".".join(self.domain.split(".")[-2:])
         self.site_id = self.domain.split(".")[0]
         self.odoo_major_version = int(opt_args.odoo_version.split('.')[0])
         if opt_args.http_port:
             self.http_port = opt_args.http_port
+        elif self.odoo_config.get("http_port"):
+            self.http_port = self.odoo_config["http_port"]
+        elif self.odoo_config.get("xmlrpc_port"):
+            self.http_port = self.odoo_config["xmlrpc_port"]
         else:
             self.http_port = (8160 + self.odoo_major_version)
-        if int(self.http_port) >= 19000:
+        if opt_args.longpolling_port:
+            self.http_port = opt_args.longpolling_port
+        elif self.odoo_config.get("longpolling_port"):
+            self.longport = self.odoo_config["longpolling_port"]
+        elif int(self.http_port) >= 19000:
             self.longport = "%s" % (int(self.http_port) - 19000 + 100)
         else:
             self.longport = (8130 + self.odoo_major_version)
         params = {
             "domain": self.domain,
             "port": self.http_port,
             "longport": self.longport,
             "email": "%s" % self.email,
         }
         if self.opt_args.https:
             self.http_config = TEMPLATE_HTTPS % params
         else:
             self.http_config = TEMPLATE % params
-        self.confn = "%s.conf" % self.domain
-        self.odoo_config = ""
-        if self.opt_args.odoo_config:
-            if not os.path.isfile(self.opt_args.odoo_config):
-                print("Odoo config file %s not found!" % self.opt_args.odoo_config)
-                return
-            with open(self.opt_args.odoo_config, "r") as fd:
-                odoo_config = fd.read()
-            odoo_config = re.sub(
-                "^logfile = .*",
-                "logfile = /var/log/odoo/odoo12-%s.log" % self.site_id,
-                odoo_config,
-                flags=re.MULTILINE)
-            odoo_config = re.sub(
-                "^pidfile = .*",
-                "pidfile = /var/run/odoo/odoo12-%s.pid" % self.site_id,
-                odoo_config,
-                flags=re.MULTILINE)
-            odoo_config = re.sub(
-                "^longpolling_port = .*",
-                "longpolling_port = %s" % self.longport,
-                odoo_config,
-                flags=re.MULTILINE)
-            odoo_config = re.sub(
-                "^xmlrpc_port = .*",
-                "xmlrpc_port = %s" % self.http_port,
-                odoo_config,
-                flags=re.MULTILINE)
-            odoo_config = re.sub(
-                "^http_port = .*",
-                "http_port = %s" % self.http_port,
-                odoo_config,
-                flags=re.MULTILINE)
-            self.odoo_config = odoo_config
 
     def close(self):
         def write_file(fn, content):
             bakfile = "%s.bak" % fn
             if os.path.isfile(bakfile):
                 os.remove(bakfile)
             if os.path.isfile(fn):
@@ -153,27 +143,28 @@
             with open(fn, "w") as fd:
                 fd.write(content)
                 if self.opt_args.verbose > 0:
                     print("👽 %s" % fn)
 
         if not self.opt_args.dry_run:
             write_file(self.confn, self.http_config)
-            if self.odoo_config:
-                write_file("odoo12-%s.conf" % self.site_id, self.odoo_config)
+            # if self.odoo_config:
+            #     write_file("odoo12-%s.conf" % self.site_id, self.odoo_config)
 
 
 def main(cli_args=None):
     cli_args = cli_args or sys.argv[1:]
     parser = argparse.ArgumentParser(
         description="Create apache config file for Odoo instance",
         epilog="© 2021-2023 by SHS-AV s.r.l."
     )
     parser.add_argument('-b', '--odoo-version', dest="odoo_version", default="12.0")
     parser.add_argument('-c', '--odoo-config', dest="odoo_config")
     parser.add_argument("-n", "--dry-run", dest="dry_run", action="store_true")
+    parser.add_argument('-l', '--longpolling-port')
     parser.add_argument('-p', '--http-port', dest="http_port")
     parser.add_argument('-s', '--https', action="store_true", dest="https")
     parser.add_argument('-v', '--verbose', action='count', default=0)
     parser.add_argument('-V', '--version', action="version", version=__version__)
     parser.add_argument('domain')
     opt_args = parser.parse_args(cli_args)
     sts = 0
```

### Comparing `wok_code-2.0.4/wok_code/eval_gtin.py` & `wok_code-2.0.6/wok_code/eval_gtin.py`

 * *Files identical despite different names*

### Comparing `wok_code-2.0.4/wok_code/topep8` & `wok_code-2.0.6/wok_code/topep8`

 * *Files 1% similar despite different names*

```diff
@@ -31,28 +31,26 @@
 . $ODOOLIBDIR
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "ODOOLIBDIR=$ODOOLIBDIR"
 TRAVISLIBDIR=$(findpkg travisrc "$PYPATH" "travis_emulator")
 [[ -z "$TRAVISLIBDIR" ]] && echo "Library file travisrc not found!" && exit 72
 . $TRAVISLIBDIR
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "TRAVISLIBDIR=$TRAVISLIBDIR"
 
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
 
-__version__=2.0.4
+__version__=2.0.6
 
-[[ -f $TDIR/../../clodoo/list_requirements.py ]] && LISTREQ=$TDIR/../../clodoo/list_requirements.py || LISTREQ=list_requirements.py
+# [[ -f $TDIR/../../python_plus/list_requirements.py ]] && LISTREQ=$TDIR/../../python_plus/list_requirements.py || LISTREQ=list_requirements.py
 YAML_TMPL=~/dev/pypi/z0bug_odd/z0bug_odoo/sample_files/.travis.yml
 NO_APT_GET="(build-essential|curl|git|gradle|gzip|java|lessc|less-plugin-clean-css|nodejs|npm|openssl|python-setuptools|python-simplejson|PhantomJS|rvm|ruby|sass|scss|tesseract|wget|wkhtmltopdf|zip)"
 
 expand_macro() {
   local t p v lne lne1
   lne="$1"
   for t in {1..9} LNK_DOCS BTN_DOCS LNK_HELP BTN_HELP; do
```

### Comparing `wok_code-2.0.4/wok_code/cvt_script.man` & `wok_code-2.0.6/wok_code/cvt_script.man`

 * *Files identical despite different names*

### Comparing `wok_code-2.0.4/wok_code/to_oca.2p8` & `wok_code-2.0.6/wok_code/to_oca.2p8`

 * *Files identical despite different names*

### Comparing `wok_code-2.0.4/wok_code/do_set_utf8.py` & `wok_code-2.0.6/wok_code/do_set_utf8.py`

 * *Files identical despite different names*

### Comparing `wok_code-2.0.4/wok_code/please.man` & `wok_code-2.0.6/wok_code/please.man`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 .\" Manpage for please.
 .\" Contact antoniomaria.vigliotti@gmail.com to correct errors or typos.
 .TH please 8
 .SH NAME
-please \- develeoper shell
+please \- developer shell
 .SH SYNOPSIS
 please [options] action [package]
 .SH DESCRIPTION
 \fBplease\fR is an interactive developer shell aim to help development and testing software.
 .P
 Action is one of:
 .br
 * help
 .br
-* build
-.br
 * chkconfig
 .br
 * commit (deprecated)
 .br
 * config
 .br
 * distribution (deprecated)
@@ -28,14 +26,16 @@
 .br
 * duplicate
 .br
 * export MODULE DB
 .br
 * import
 .br
+* install
+.br
 * list
 .br
 * lsearch
 .br
 * publish
 .br
 * push
@@ -55,22 +55,16 @@
 * test [-b BRANCH] [-B[B]] [-c FILE] [-d DB] [-f]
 .br
 * translate MODULE DB
 .br
 * version
 .br
 * wep
-.P
-\fBbuild\fR
-.RS
-Build a tar file for current PYPI project
 .br
-This action is appliable just to PYPI projects. The tar file is created on project root directory (i.e. ~/dev/pypi/my_project).
-Look at \fBplease status\fR to see projects tree.
-.RE
+* z0bug
 .P
 \fBchkconfig\fR
 .RS
 Display various values of current project.
 .RE
 .P
 \fBcommit\fR
@@ -135,14 +129,20 @@
 \fBimport MODULE DB\fR
 .RS
 Import po file of Odoo project.
 .br
 To declare target version use \fB-b\fR switch
 .RE
 .P
+\fBinstall MODULE\fR
+.RS
+Install some components (currently just python3)
+.br
+.RE
+.P
 \fBlist\fR
 .RS
 List host where to push project.
 .RE
 .P
 \fBlsearch DB TOKEN [-d date][-b odoo_ver]\fR
 .RS
@@ -283,14 +283,23 @@
 \fBtranslate MODULE DB\fR
 .RS
 Translate po file of Odoo project.
 In order to access to database a configuratione file must be supplied with \fB-c\fR switch.
 .br
 To declare target version use \fB-b\fR switch
 .RE
+.P
+\fBz0bug\fR
+.RS
+Execute lint and tests.
+.br
+This command executes the lint and the regression tests.
+In previous version of please this command were called travis;
+travis is now deprecated
+.RE
 .SH OPTIONS
 .TP
 .BR \-L \fIfilename\fR
 Trace file name. Default is /var/log/product.log if user is root, otherwise is ~/product.log
 .TP
 .BR \-n
 Do nothing (dry-run)
```

### Comparing `wok_code-2.0.4/wok_code/to_zero.2p8` & `wok_code-2.0.6/wok_code/to_zero.2p8`

 * *Files identical despite different names*

### Comparing `wok_code-2.0.4/wok_code/to_pep8.2p8` & `wok_code-2.0.6/wok_code/to_pep8.2p8`

 * *Files identical despite different names*

### Comparing `wok_code-2.0.4/wok_code/cvt_script` & `wok_code-2.0.6/wok_code/cvt_script`

 * *Files 2% similar despite different names*

```diff
@@ -25,26 +25,24 @@
     Z0LIBDIR=$(readlink -e $d)
     break
   fi
 done
 [[ -z "$Z0LIBDIR" ]] && echo "Library file z0librc not found in <$PYPATH>!" && exit 72
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "Z0LIBDIR=$Z0LIBDIR"
 
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
 
-__version__=2.0.4
+__version__=2.0.6
 
 #//Only human upgradable code/
 # blk1 => z0librc
 # blk2 => odoorc
 # blk3 => travisrc
 # blk4 => zarrc
 # blk8 => TESTDIR= ...
```

### Comparing `wok_code-2.0.4/setup.py` & `wok_code-2.0.6/wok_code/scripts/setup.info`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     install_requires.append('translators')
     install_requires.append('twine')
 else:
     install_requires.append('twine==1.15.0')
 
 setup(
     name='wok_code',
-    version='2.0.4',
+    version='2.0.6',
     description='Python developers tools',
     long_description="""
 Various tools at your fingertips.
 
 The available tools are:
 
 * cvt_csv_2_rst.py: convert csv file into rst file
@@ -55,22 +55,24 @@
     install_requires=install_requires,
     packages=find_packages(exclude=['docs', 'examples', 'tests', 'egg-info', 'junk']),
     package_data={
         '': [
             'scripts/setup.info',
             'scripts/dist_pkg.sh',
             'scripts/please.sh',
+            'scripts/config/*',
             './please.man',
             './cvt_script',
             './cvt_script.man',
             './topep8',
             './to_oca.2p8',
             './to_zero.2p8',
             './to_pep8.2p8',
             './pypi.sh',
+            './install_python_3_from_source.sh',
         ]
     },
     entry_points={
         'console_scripts': [
             'wok_code-info = wok_code.scripts.main:main',
             'cvt_csv_2_rst.py = wok_code.scripts.cvt_csv_2_rst:main',
             'cvt_csv_coa = wok_code.scripts.cvt_csv_coa:main',
@@ -82,11 +84,12 @@
             'lint_2_compare = wok_code.scripts.lint_2_compare:main',
             'makepo_it.py = wok_code.scripts.makepo_it:main',
             'odoo_dependencies.py = wok_code.scripts.odoo_dependencies:main',
             'odoo_translation.py = wok_code.scripts.odoo_translation:main',
             'please = wok_code.scripts.please:main',
             'to_pep8.py = wok_code.scripts.to_pep8:main',
             'wget_odoo_repositories.py = wok_code.scripts.wget_odoo_repositories:main',
+            'run_odoo_debug = odoo_score.scripts.run_odoo_debug:main',
         ]
     },
     zip_safe=False,
 )
```

### Comparing `wok_code-2.0.4/PKG-INFO` & `wok_code-2.0.6/wok_code.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,41 @@
-Metadata-Version: 1.2
-Name: wok_code
-Version: 2.0.4
+Metadata-Version: 2.1
+Name: wok-code
+Version: 2.0.6
 Summary: Python developers tools
 Home-page: https://zeroincombenze-tools.readthedocs.io
 Author: Antonio Maria Vigliotti
 Author-email: antoniomaria.vigliotti@gmail.com
 License: Affero GPL
-Project-URL: Source, https://github.com/zeroincombenze/tools
 Project-URL: Documentation, https://zeroincombenze-tools.readthedocs.io
-Description: 
-        Various tools at your fingertips.
-        
-        The available tools are:
-        
-        * cvt_csv_2_rst.py: convert csv file into rst file
-        * cvt_csv_2_xml.py: convert csv file into xml file
-        * cvt_script: parse bash script and convert to meet company standard
-        * gen_readme.py: generate documentation files, mainly README.rst
-        * odoo_dependency.py: show odoo dependencies and/or Odoo module tree
-        * odoo_translation.py: manage Odoo translation
-        * pep8: parse source .py file to meet pep8 and convert across Odoo versions
-        * please: developer shell
-        * wget_odoo_repositories.py: get repository names from github.com
-        
+Project-URL: Source, https://github.com/zeroincombenze/tools
 Keywords: linux travis development
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
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Operating System :: OS Independent
+
+
+Various tools at your fingertips.
+
+The available tools are:
+
+* cvt_csv_2_rst.py: convert csv file into rst file
+* cvt_csv_2_xml.py: convert csv file into xml file
+* cvt_script: parse bash script and convert to meet company standard
+* gen_readme.py: generate documentation files, mainly README.rst
+* odoo_dependency.py: show odoo dependencies and/or Odoo module tree
+* odoo_translation.py: manage Odoo translation
+* pep8: parse source .py file to meet pep8 and convert across Odoo versions
+* please: developer shell
+* wget_odoo_repositories.py: get repository names from github.com
+
+
```

### Comparing `wok_code-2.0.4/README.rst` & `wok_code-2.0.6/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 ==============
-wok_code 2.0.4
+wok_code 2.0.6
 ==============
 
 
 
 |Maturity| |Build Status| |Coverage Status| |license gpl|
 
 
@@ -368,15 +368,15 @@
       -w, --suppress-warning
 
 Examples:
 
 ::
 
     # Update Odoo module documentation
-    cd ~/odoo_12/axitec/l10n_it_balance     # Odoo project directory
+    cd ~/odoo_12/l10n-italy/l10n_it_balance # Odoo project directory
     dir egg-info
     >>> authors.txt contributors.txt description.rst __init__.txt known_issues.rst
     gen_readme.py                           # Generate README.rst of project
     gen_readme.py -H                        # Generate index.html of project
 
     # Create index.rst of pypi module
     cd ~/dev/pypi/devel_tools/devel_tools/docs
@@ -841,20 +841,34 @@
     ./install_tools.sh -Ud
     source /opt/odoo/devel/activate_tools
 
 
 History
 -------
 
-2.0.5 (2022-12-13)
+2.0.6 (2023-02-23)
 ~~~~~~~~~~~~~~~~~~
 
+* [IMP] ssh.py: -m -s switches accept path with user and host
+* [IMP] deploy_odoo: new property status to display
+* [IMP] deploy_odoo: new switches -l and -x
+* [NEW] do_git_checkout_new_branch.py
+* [IMP] do_migrate.py: new features
+* [IMP] run_odoo_debug.sh imported from odoo_score
+* [FIX] run_odoo_debug.sh: ODOO_COMMIT TEST not set when build template
+* [IMP] run_odoo_debug.sh: simulate server_wide_modules parameter for Odoo 7.0-
+
+
+2.0.5 (2023-01-13)
+~~~~~~~~~~~~~~~~~~
+
+* [IMP] please: wep now delete old travis-emulator logs
 * [IMP] install_python_3_from_source.sh: now can install python 3.9
 * [IMP] please: action docs, minor improvements
-* [IMP] deply_odoo: format output list
+* [IMP] deploy_odoo: format output list
 
 2.0.4 (2022-12-09)
 ~~~~~~~~~~~~~~~~~~
 
 * [FIX] deploy_odoo: update from path
 * [FIX] build_cmd: best recognition of python version
 * [FIX] set_python_version.sh: best recognition of python version
@@ -909,19 +923,14 @@
 * [FIX] please lint|test
 
 2.0.0.1 (2022-09-07)
 ~~~~~~~~~~~~~~~~~~~~
 
 * [FIX] please test: with debug
 
-2.0.0 (2022-08-10)
-~~~~~~~~~~~~~~~~~~
-
-* [REF] Refactoring
-
 
 
 |
 |
 
 Credits
 =======
@@ -932,21 +941,24 @@
 SHS-AV s.r.l. <https://www.shs-av.com/>
 
 
 Contributors
 ------------
 
 * Antonio Maria Vigliotti <antoniomaria.vigliotti@gmail.com>
+Contributors
+------------
+
 
 
 |
 
 This module is part of tools project.
 
-Last Update / Ultimo aggiornamento: 2023-01-13
+Last Update / Ultimo aggiornamento: 2023-04-23
 
 .. |Maturity| image:: https://img.shields.io/badge/maturity-Beta-yellow.png
     :target: https://odoo-community.org/page/development-status
     :alt: 
 .. |Build Status| image:: https://travis-ci.org/zeroincombenze/tools.svg?branch=master
     :target: https://travis-ci.com/zeroincombenze/tools
     :alt: github.com
```

