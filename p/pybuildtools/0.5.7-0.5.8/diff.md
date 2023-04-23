# Comparing `tmp/pybuildtools-0.5.7.tar.gz` & `tmp/pybuildtools-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybuildtools-0.5.7.tar", max compression
+gzip compressed data, was "pybuildtools-0.5.8.tar", max compression
```

## Comparing `pybuildtools-0.5.7.tar` & `pybuildtools-0.5.8.tar`

### file list

```diff
@@ -1,69 +1,73 @@
--rw-r--r--   0        0        0     1085 2022-04-28 03:59:26.731217 pybuildtools-0.5.7/LICENSE
--rw-r--r--   0        0        0     2524 2020-06-12 05:01:15.360686 pybuildtools-0.5.7/README.md
--rw-r--r--   0        0        0     1443 2022-01-02 00:20:35.159580 pybuildtools-0.5.7/buildtools/__init__.py
--rw-r--r--   0        0        0     4852 2022-01-02 00:20:35.315580 pybuildtools-0.5.7/buildtools/_os_utils_linux.py
--rw-r--r--   0        0        0     4985 2022-01-02 00:20:35.167580 pybuildtools-0.5.7/buildtools/_os_utils_win32.py
--rw-r--r--   0        0        0     4119 2022-04-10 23:58:02.965724 pybuildtools-0.5.7/buildtools/as3.py
--rw-r--r--   0        0        0     6638 2022-05-26 20:31:45.223260 pybuildtools-0.5.7/buildtools/bt_logging.py
--rw-r--r--   0        0        0     2336 2022-01-02 00:20:35.167580 pybuildtools-0.5.7/buildtools/buildsystem/CCompiler.py
--rw-r--r--   0        0        0     1251 2022-01-02 00:20:35.167580 pybuildtools-0.5.7/buildtools/buildsystem/__init__.py
--rw-r--r--   0        0        0     1896 2022-01-02 00:20:35.167580 pybuildtools-0.5.7/buildtools/buildsystem/baseproject.py
--rw-r--r--   0        0        0        0 2016-03-09 08:33:59.525584 pybuildtools-0.5.7/buildtools/buildsystem/gcc.py
--rw-r--r--   0        0        0     2165 2022-01-02 00:20:35.159580 pybuildtools-0.5.7/buildtools/buildsystem/msbuild.py
--rw-r--r--   0        0        0    10714 2022-01-02 00:20:35.159580 pybuildtools-0.5.7/buildtools/buildsystem/prebuild.py
--rw-r--r--   0        0        0    25104 2022-01-02 00:20:35.167580 pybuildtools-0.5.7/buildtools/buildsystem/visualstudio.py
--rw-r--r--   0        0        0     3130 2022-04-10 23:59:46.976807 pybuildtools-0.5.7/buildtools/cli.py
--rw-r--r--   0        0        0    12818 2022-04-11 00:02:46.811262 pybuildtools-0.5.7/buildtools/config.py
--rw-r--r--   0        0        0      888 2022-05-26 21:09:24.072440 pybuildtools-0.5.7/buildtools/consts.py
--rw-r--r--   0        0        0     1507 2022-01-02 00:20:35.167580 pybuildtools-0.5.7/buildtools/error.py
--rw-r--r--   0        0        0        0 2016-03-09 08:33:59.525584 pybuildtools-0.5.7/buildtools/ext/__init__.py
--rw-r--r--   0        0        0        0 2016-03-09 08:33:59.525584 pybuildtools-0.5.7/buildtools/ext/salt/__init__.py
--rw-r--r--   0        0        0    14607 2022-04-11 03:07:37.825054 pybuildtools-0.5.7/buildtools/ext/salt/jinja_ext.py
--rw-r--r--   0        0        0     4163 2022-04-11 00:18:04.147824 pybuildtools-0.5.7/buildtools/http.py
--rw-r--r--   0        0        0     7697 2022-04-11 00:40:52.069432 pybuildtools-0.5.7/buildtools/indentation.py
--rw-r--r--   0        0        0     1775 2022-01-02 00:20:35.167580 pybuildtools-0.5.7/buildtools/lxml_utils.py
--rw-r--r--   0        0        0    17139 2022-05-24 02:07:28.365863 pybuildtools-0.5.7/buildtools/maestro/__init__.py
--rw-r--r--   0        0        0    17051 2022-08-08 03:26:30.953399 pybuildtools-0.5.7/buildtools/maestro/base_target.py
--rw-r--r--   0        0        0     6475 2022-08-07 23:04:09.389150 pybuildtools-0.5.7/buildtools/maestro/coffeescript.py
--rw-r--r--   0        0        0     3331 2022-01-02 00:20:35.167580 pybuildtools-0.5.7/buildtools/maestro/convert_data.py
--rw-r--r--   0        0        0     2683 2022-08-07 23:39:33.514115 pybuildtools-0.5.7/buildtools/maestro/docs.py
--rw-r--r--   0        0        0        0 2020-01-06 05:44:12.351832 pybuildtools-0.5.7/buildtools/maestro/enumwriters/__init__.py
--rw-r--r--   0        0        0     6301 2022-08-07 22:47:19.967395 pybuildtools-0.5.7/buildtools/maestro/enumwriters/coffee.py
--rw-r--r--   0        0        0     1426 2022-05-23 21:48:56.060450 pybuildtools-0.5.7/buildtools/maestro/enumwriters/enumwriter.py
--rw-r--r--   0        0        0     7409 2022-08-07 22:47:33.355318 pybuildtools-0.5.7/buildtools/maestro/enumwriters/php.py
--rw-r--r--   0        0        0     3223 2022-08-07 22:48:32.242959 pybuildtools-0.5.7/buildtools/maestro/enumwriters/python.py
--rw-r--r--   0        0        0     8210 2022-08-07 22:49:38.682525 pybuildtools-0.5.7/buildtools/maestro/enumwriters/types.py
--rw-r--r--   0        0        0    16708 2022-08-08 03:48:26.723829 pybuildtools-0.5.7/buildtools/maestro/fileio.py
--rw-r--r--   0        0        0     2392 2022-05-23 21:52:15.126516 pybuildtools-0.5.7/buildtools/maestro/genenum.py
--rw-r--r--   0        0        0     8233 2022-01-02 00:20:35.167580 pybuildtools-0.5.7/buildtools/maestro/git.py
--rw-r--r--   0        0        0     2341 2022-01-02 00:20:35.167580 pybuildtools-0.5.7/buildtools/maestro/jinja2.py
--rw-r--r--   0        0        0     9371 2023-04-19 23:52:37.733616 pybuildtools-0.5.7/buildtools/maestro/nuitka.py
--rw-r--r--   0        0        0     8244 2022-01-02 00:20:35.167580 pybuildtools-0.5.7/buildtools/maestro/package_managers.py
--rw-r--r--   0        0        0     2866 2022-08-08 01:58:55.584152 pybuildtools-0.5.7/buildtools/maestro/shell.py
--rw-r--r--   0        0        0     2210 2022-01-02 00:20:35.167580 pybuildtools-0.5.7/buildtools/maestro/utils.py
--rw-r--r--   0        0        0    23491 2022-08-08 02:16:35.587000 pybuildtools-0.5.7/buildtools/maestro/web.py
--rw-r--r--   0        0        0    26397 2022-04-11 03:13:52.442499 pybuildtools-0.5.7/buildtools/os_utils.py
--rw-r--r--   0        0        0        0 2016-03-09 08:33:59.525584 pybuildtools-0.5.7/buildtools/posix/__init__.py
--rw-r--r--   0        0        0     5105 2022-01-02 00:20:35.315580 pybuildtools-0.5.7/buildtools/posix/elf.py
--rw-r--r--   0        0        0     4438 2022-04-04 17:43:42.560641 pybuildtools-0.5.7/buildtools/pygit2_callbacks.py
--rw-r--r--   0        0        0     3121 2022-03-19 21:22:21.894105 pybuildtools-0.5.7/buildtools/qconfig5.py
--rw-r--r--   0        0        0        0 2016-03-09 08:33:59.525584 pybuildtools-0.5.7/buildtools/repo/__init__.py
--rw-r--r--   0        0        0     1541 2022-01-02 00:20:35.167580 pybuildtools-0.5.7/buildtools/repo/base.py
--rw-r--r--   0        0        0    11331 2022-01-02 00:20:35.167580 pybuildtools-0.5.7/buildtools/repo/git.py
--rw-r--r--   0        0        0     7985 2022-01-02 00:20:35.167580 pybuildtools-0.5.7/buildtools/repo/hg.py
--rw-r--r--   0        0        0     4747 2022-01-02 00:20:35.159580 pybuildtools-0.5.7/buildtools/timing.py
--rw-r--r--   0        0        0     6979 2022-08-07 23:44:05.712677 pybuildtools-0.5.7/buildtools/twisted_utils.py
--rw-r--r--   0        0        0       83 2022-08-07 23:37:12.778841 pybuildtools-0.5.7/buildtools/types.py
--rw-r--r--   0        0        0     2642 2022-04-11 00:43:48.188066 pybuildtools-0.5.7/buildtools/utils.py
--rw-r--r--   0        0        0     1326 2022-01-02 00:20:35.315580 pybuildtools-0.5.7/buildtools/wrapper/__init__.py
--rw-r--r--   0        0        0     1808 2022-01-02 00:20:35.315580 pybuildtools-0.5.7/buildtools/wrapper/ant.py
--rw-r--r--   0        0        0     2445 2022-01-02 00:20:35.315580 pybuildtools-0.5.7/buildtools/wrapper/ccache.py
--rw-r--r--   0        0        0     2788 2022-01-02 00:20:35.315580 pybuildtools-0.5.7/buildtools/wrapper/cmake.py
--rw-r--r--   0        0        0     1699 2022-01-02 00:20:35.315580 pybuildtools-0.5.7/buildtools/wrapper/cotire.py
--rw-r--r--   0        0        0     3596 2022-01-02 00:20:35.315580 pybuildtools-0.5.7/buildtools/wrapper/distcc.py
--rw-r--r--   0        0        0     5550 2022-01-02 00:20:35.315580 pybuildtools-0.5.7/buildtools/wrapper/fpm.py
--rw-r--r--   0        0        0     4343 2022-01-02 00:20:35.315580 pybuildtools-0.5.7/buildtools/wrapper/git.py
--rw-r--r--   0        0        0        0 2016-03-09 08:33:59.525584 pybuildtools-0.5.7/buildtools/wrapper/repo/__init__.py
--rw-r--r--   0        0        0     1355 2023-04-20 00:34:04.972568 pybuildtools-0.5.7/pyproject.toml
--rw-r--r--   0        0        0     3990 1970-01-01 00:00:00.000000 pybuildtools-0.5.7/setup.py
--rw-r--r--   0        0        0     3898 1970-01-01 00:00:00.000000 pybuildtools-0.5.7/PKG-INFO
+-rw-r--r--   0        0        0     1085 2022-04-28 03:59:26.731217 pybuildtools-0.5.8/LICENSE
+-rw-r--r--   0        0        0     2524 2020-06-12 05:01:15.360686 pybuildtools-0.5.8/README.md
+-rw-r--r--   0        0        0     1443 2022-01-02 00:20:35.159580 pybuildtools-0.5.8/buildtools/__init__.py
+-rw-r--r--   0        0        0     4852 2022-01-02 00:20:35.315580 pybuildtools-0.5.8/buildtools/_os_utils_linux.py
+-rw-r--r--   0        0        0     4985 2022-01-02 00:20:35.167580 pybuildtools-0.5.8/buildtools/_os_utils_win32.py
+-rw-r--r--   0        0        0     4119 2022-04-10 23:58:02.965724 pybuildtools-0.5.8/buildtools/as3.py
+-rw-r--r--   0        0        0     6638 2022-05-26 20:31:45.223260 pybuildtools-0.5.8/buildtools/bt_logging.py
+-rw-r--r--   0        0        0     2336 2022-01-02 00:20:35.167580 pybuildtools-0.5.8/buildtools/buildsystem/CCompiler.py
+-rw-r--r--   0        0        0     1251 2022-01-02 00:20:35.167580 pybuildtools-0.5.8/buildtools/buildsystem/__init__.py
+-rw-r--r--   0        0        0     1896 2022-01-02 00:20:35.167580 pybuildtools-0.5.8/buildtools/buildsystem/baseproject.py
+-rw-r--r--   0        0        0        0 2016-03-09 08:33:59.525584 pybuildtools-0.5.8/buildtools/buildsystem/gcc.py
+-rw-r--r--   0        0        0     2165 2022-01-02 00:20:35.159580 pybuildtools-0.5.8/buildtools/buildsystem/msbuild.py
+-rw-r--r--   0        0        0    10714 2022-01-02 00:20:35.159580 pybuildtools-0.5.8/buildtools/buildsystem/prebuild.py
+-rw-r--r--   0        0        0    25104 2022-01-02 00:20:35.167580 pybuildtools-0.5.8/buildtools/buildsystem/visualstudio.py
+-rw-r--r--   0        0        0        0 2023-04-20 05:41:36.306401 pybuildtools-0.5.8/buildtools/cli/__init__.py
+-rw-r--r--   0        0        0      145 2023-04-20 05:46:57.351963 pybuildtools-0.5.8/buildtools/cli/nuitka_plus/README.md
+-rw-r--r--   0        0        0        0 2023-04-20 05:40:08.183068 pybuildtools-0.5.8/buildtools/cli/nuitka_plus/__init__.py
+-rw-r--r--   0        0        0      521 2023-04-21 00:16:51.099447 pybuildtools-0.5.8/buildtools/cli/nuitka_plus/__main__.py
+-rw-r--r--   0        0        0     3130 2022-04-10 23:59:46.976807 pybuildtools-0.5.8/buildtools/cli.py
+-rw-r--r--   0        0        0    12818 2022-04-11 00:02:46.811262 pybuildtools-0.5.8/buildtools/config.py
+-rw-r--r--   0        0        0      888 2022-05-26 21:09:24.072440 pybuildtools-0.5.8/buildtools/consts.py
+-rw-r--r--   0        0        0     1507 2022-01-02 00:20:35.167580 pybuildtools-0.5.8/buildtools/error.py
+-rw-r--r--   0        0        0        0 2016-03-09 08:33:59.525584 pybuildtools-0.5.8/buildtools/ext/__init__.py
+-rw-r--r--   0        0        0        0 2016-03-09 08:33:59.525584 pybuildtools-0.5.8/buildtools/ext/salt/__init__.py
+-rw-r--r--   0        0        0    14607 2022-04-11 03:07:37.825054 pybuildtools-0.5.8/buildtools/ext/salt/jinja_ext.py
+-rw-r--r--   0        0        0     4179 2023-04-20 06:02:51.757946 pybuildtools-0.5.8/buildtools/http.py
+-rw-r--r--   0        0        0     7697 2022-04-11 00:40:52.069432 pybuildtools-0.5.8/buildtools/indentation.py
+-rw-r--r--   0        0        0     1775 2022-01-02 00:20:35.167580 pybuildtools-0.5.8/buildtools/lxml_utils.py
+-rw-r--r--   0        0        0    17139 2022-05-24 02:07:28.365863 pybuildtools-0.5.8/buildtools/maestro/__init__.py
+-rw-r--r--   0        0        0    17051 2022-08-08 03:26:30.953399 pybuildtools-0.5.8/buildtools/maestro/base_target.py
+-rw-r--r--   0        0        0     6475 2022-08-07 23:04:09.389150 pybuildtools-0.5.8/buildtools/maestro/coffeescript.py
+-rw-r--r--   0        0        0     3331 2022-01-02 00:20:35.167580 pybuildtools-0.5.8/buildtools/maestro/convert_data.py
+-rw-r--r--   0        0        0     2683 2022-08-07 23:39:33.514115 pybuildtools-0.5.8/buildtools/maestro/docs.py
+-rw-r--r--   0        0        0        0 2020-01-06 05:44:12.351832 pybuildtools-0.5.8/buildtools/maestro/enumwriters/__init__.py
+-rw-r--r--   0        0        0     6301 2022-08-07 22:47:19.967395 pybuildtools-0.5.8/buildtools/maestro/enumwriters/coffee.py
+-rw-r--r--   0        0        0     1426 2022-05-23 21:48:56.060450 pybuildtools-0.5.8/buildtools/maestro/enumwriters/enumwriter.py
+-rw-r--r--   0        0        0     7409 2022-08-07 22:47:33.355318 pybuildtools-0.5.8/buildtools/maestro/enumwriters/php.py
+-rw-r--r--   0        0        0     3223 2022-08-07 22:48:32.242959 pybuildtools-0.5.8/buildtools/maestro/enumwriters/python.py
+-rw-r--r--   0        0        0     8210 2022-08-07 22:49:38.682525 pybuildtools-0.5.8/buildtools/maestro/enumwriters/types.py
+-rw-r--r--   0        0        0    16708 2022-08-08 03:48:26.723829 pybuildtools-0.5.8/buildtools/maestro/fileio.py
+-rw-r--r--   0        0        0     2392 2022-05-23 21:52:15.126516 pybuildtools-0.5.8/buildtools/maestro/genenum.py
+-rw-r--r--   0        0        0     8233 2022-01-02 00:20:35.167580 pybuildtools-0.5.8/buildtools/maestro/git.py
+-rw-r--r--   0        0        0     2341 2022-01-02 00:20:35.167580 pybuildtools-0.5.8/buildtools/maestro/jinja2.py
+-rw-r--r--   0        0        0    13368 2023-04-21 03:42:07.717124 pybuildtools-0.5.8/buildtools/maestro/nuitka.py
+-rw-r--r--   0        0        0     8244 2022-01-02 00:20:35.167580 pybuildtools-0.5.8/buildtools/maestro/package_managers.py
+-rw-r--r--   0        0        0     2866 2022-08-08 01:58:55.584152 pybuildtools-0.5.8/buildtools/maestro/shell.py
+-rw-r--r--   0        0        0     2210 2022-01-02 00:20:35.167580 pybuildtools-0.5.8/buildtools/maestro/utils.py
+-rw-r--r--   0        0        0    23491 2022-08-08 02:16:35.587000 pybuildtools-0.5.8/buildtools/maestro/web.py
+-rw-r--r--   0        0        0    26397 2022-04-11 03:13:52.442499 pybuildtools-0.5.8/buildtools/os_utils.py
+-rw-r--r--   0        0        0        0 2016-03-09 08:33:59.525584 pybuildtools-0.5.8/buildtools/posix/__init__.py
+-rw-r--r--   0        0        0     5105 2022-01-02 00:20:35.315580 pybuildtools-0.5.8/buildtools/posix/elf.py
+-rw-r--r--   0        0        0     4438 2022-04-04 17:43:42.560641 pybuildtools-0.5.8/buildtools/pygit2_callbacks.py
+-rw-r--r--   0        0        0     3121 2022-03-19 21:22:21.894105 pybuildtools-0.5.8/buildtools/qconfig5.py
+-rw-r--r--   0        0        0        0 2016-03-09 08:33:59.525584 pybuildtools-0.5.8/buildtools/repo/__init__.py
+-rw-r--r--   0        0        0     1541 2022-01-02 00:20:35.167580 pybuildtools-0.5.8/buildtools/repo/base.py
+-rw-r--r--   0        0        0    11331 2022-01-02 00:20:35.167580 pybuildtools-0.5.8/buildtools/repo/git.py
+-rw-r--r--   0        0        0     7985 2022-01-02 00:20:35.167580 pybuildtools-0.5.8/buildtools/repo/hg.py
+-rw-r--r--   0        0        0     4747 2022-01-02 00:20:35.159580 pybuildtools-0.5.8/buildtools/timing.py
+-rw-r--r--   0        0        0     6979 2022-08-07 23:44:05.712677 pybuildtools-0.5.8/buildtools/twisted_utils.py
+-rw-r--r--   0        0        0       83 2022-08-07 23:37:12.778841 pybuildtools-0.5.8/buildtools/types.py
+-rw-r--r--   0        0        0     2642 2022-04-11 00:43:48.188066 pybuildtools-0.5.8/buildtools/utils.py
+-rw-r--r--   0        0        0     1326 2022-01-02 00:20:35.315580 pybuildtools-0.5.8/buildtools/wrapper/__init__.py
+-rw-r--r--   0        0        0     1808 2022-01-02 00:20:35.315580 pybuildtools-0.5.8/buildtools/wrapper/ant.py
+-rw-r--r--   0        0        0     2445 2022-01-02 00:20:35.315580 pybuildtools-0.5.8/buildtools/wrapper/ccache.py
+-rw-r--r--   0        0        0     2788 2022-01-02 00:20:35.315580 pybuildtools-0.5.8/buildtools/wrapper/cmake.py
+-rw-r--r--   0        0        0     1699 2022-01-02 00:20:35.315580 pybuildtools-0.5.8/buildtools/wrapper/cotire.py
+-rw-r--r--   0        0        0     3596 2022-01-02 00:20:35.315580 pybuildtools-0.5.8/buildtools/wrapper/distcc.py
+-rw-r--r--   0        0        0     5550 2022-01-02 00:20:35.315580 pybuildtools-0.5.8/buildtools/wrapper/fpm.py
+-rw-r--r--   0        0        0     4343 2022-01-02 00:20:35.315580 pybuildtools-0.5.8/buildtools/wrapper/git.py
+-rw-r--r--   0        0        0        0 2016-03-09 08:33:59.525584 pybuildtools-0.5.8/buildtools/wrapper/repo/__init__.py
+-rw-r--r--   0        0        0     1355 2023-04-20 00:43:01.385829 pybuildtools-0.5.8/pyproject.toml
+-rw-r--r--   0        0        0     4040 1970-01-01 00:00:00.000000 pybuildtools-0.5.8/setup.py
+-rw-r--r--   0        0        0     3898 1970-01-01 00:00:00.000000 pybuildtools-0.5.8/PKG-INFO
```

### Comparing `pybuildtools-0.5.7/LICENSE` & `pybuildtools-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pybuildtools-0.5.7/README.md` & `pybuildtools-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `pybuildtools-0.5.7/buildtools/__init__.py` & `pybuildtools-0.5.8/buildtools/__init__.py`

 * *Files identical despite different names*

### Comparing `pybuildtools-0.5.7/buildtools/_os_utils_linux.py` & `pybuildtools-0.5.8/buildtools/_os_utils_linux.py`

 * *Files identical despite different names*

### Comparing `pybuildtools-0.5.7/buildtools/_os_utils_win32.py` & `pybuildtools-0.5.8/buildtools/_os_utils_win32.py`

 * *Files identical despite different names*

### Comparing `pybuildtools-0.5.7/buildtools/as3.py` & `pybuildtools-0.5.8/buildtools/as3.py`

 * *Files identical despite different names*

### Comparing `pybuildtools-0.5.7/buildtools/bt_logging.py` & `pybuildtools-0.5.8/buildtools/bt_logging.py`

 * *Files identical despite different names*

### Comparing `pybuildtools-0.5.7/buildtools/buildsystem/CCompiler.py` & `pybuildtools-0.5.8/buildtools/buildsystem/CCompiler.py`

 * *Files identical despite different names*

### Comparing `pybuildtools-0.5.7/buildtools/buildsystem/__init__.py` & `pybuildtools-0.5.8/buildtools/buildsystem/__init__.py`

 * *Files identical despite different names*

### Comparing `pybuildtools-0.5.7/buildtools/buildsystem/baseproject.py` & `pybuildtools-0.5.8/buildtools/buildsystem/baseproject.py`

 * *Files identical despite different names*

### Comparing `pybuildtools-0.5.7/buildtools/buildsystem/msbuild.py` & `pybuildtools-0.5.8/buildtools/buildsystem/msbuild.py`

 * *Files identical despite different names*

### Comparing `pybuildtools-0.5.7/buildtools/buildsystem/prebuild.py` & `pybuildtools-0.5.8/buildtools/buildsystem/prebuild.py`

 * *Files identical despite different names*

### Comparing `pybuildtools-0.5.7/buildtools/buildsystem/visualstudio.py` & `pybuildtools-0.5.8/buildtools/buildsystem/visualstudio.py`

 * *Files identical despite different names*

### Comparing `pybuildtools-0.5.7/buildtools/cli.py` & `pybuildtools-0.5.8/buildtools/cli.py`

 * *Files identical despite different names*

### Comparing `pybuildtools-0.5.7/buildtools/config.py` & `pybuildtools-0.5.8/buildtools/config.py`

 * *Files identical despite different names*

### Comparing `pybuildtools-0.5.7/buildtools/consts.py` & `pybuildtools-0.5.8/buildtools/consts.py`

 * *Files identical despite different names*

### Comparing `pybuildtools-0.5.7/buildtools/error.py` & `pybuildtools-0.5.8/buildtools/error.py`

 * *Files identical despite different names*

### Comparing `pybuildtools-0.5.7/buildtools/ext/salt/jinja_ext.py` & `pybuildtools-0.5.8/buildtools/ext/salt/jinja_ext.py`

 * *Files identical despite different names*

### Comparing `pybuildtools-0.5.7/buildtools/http.py` & `pybuildtools-0.5.8/buildtools/http.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,7 +103,8 @@
                 progress.update(buf_len)
                 #status = status + chr(8) * (len(status) + 1)  - pre-2.6 method
                 #print(status, end='\r')
         if progress is not None:
             progress.close()
     if log_after:
         log.info(f'Downloaded {url} to {output} ({file_size_dl}B)')
+    return True
```

### Comparing `pybuildtools-0.5.7/buildtools/indentation.py` & `pybuildtools-0.5.8/buildtools/indentation.py`

 * *Files identical despite different names*

### Comparing `pybuildtools-0.5.7/buildtools/lxml_utils.py` & `pybuildtools-0.5.8/buildtools/lxml_utils.py`

 * *Files identical despite different names*

### Comparing `pybuildtools-0.5.7/buildtools/maestro/__init__.py` & `pybuildtools-0.5.8/buildtools/maestro/__init__.py`

 * *Files identical despite different names*

### Comparing `pybuildtools-0.5.7/buildtools/maestro/base_target.py` & `pybuildtools-0.5.8/buildtools/maestro/base_target.py`

 * *Files identical despite different names*

### Comparing `pybuildtools-0.5.7/buildtools/maestro/coffeescript.py` & `pybuildtools-0.5.8/buildtools/maestro/coffeescript.py`

 * *Files identical despite different names*

### Comparing `pybuildtools-0.5.7/buildtools/maestro/convert_data.py` & `pybuildtools-0.5.8/buildtools/maestro/convert_data.py`

 * *Files identical despite different names*

### Comparing `pybuildtools-0.5.7/buildtools/maestro/docs.py` & `pybuildtools-0.5.8/buildtools/maestro/docs.py`

 * *Files identical despite different names*

### Comparing `pybuildtools-0.5.7/buildtools/maestro/enumwriters/coffee.py` & `pybuildtools-0.5.8/buildtools/maestro/enumwriters/coffee.py`

 * *Files identical despite different names*

### Comparing `pybuildtools-0.5.7/buildtools/maestro/enumwriters/enumwriter.py` & `pybuildtools-0.5.8/buildtools/maestro/enumwriters/enumwriter.py`

 * *Files identical despite different names*

### Comparing `pybuildtools-0.5.7/buildtools/maestro/enumwriters/php.py` & `pybuildtools-0.5.8/buildtools/maestro/enumwriters/php.py`

 * *Files identical despite different names*

### Comparing `pybuildtools-0.5.7/buildtools/maestro/enumwriters/python.py` & `pybuildtools-0.5.8/buildtools/maestro/enumwriters/python.py`

 * *Files identical despite different names*

### Comparing `pybuildtools-0.5.7/buildtools/maestro/enumwriters/types.py` & `pybuildtools-0.5.8/buildtools/maestro/enumwriters/types.py`

 * *Files identical despite different names*

### Comparing `pybuildtools-0.5.7/buildtools/maestro/fileio.py` & `pybuildtools-0.5.8/buildtools/maestro/fileio.py`

 * *Files identical despite different names*

### Comparing `pybuildtools-0.5.7/buildtools/maestro/genenum.py` & `pybuildtools-0.5.8/buildtools/maestro/genenum.py`

 * *Files identical despite different names*

### Comparing `pybuildtools-0.5.7/buildtools/maestro/git.py` & `pybuildtools-0.5.8/buildtools/maestro/git.py`

 * *Files identical despite different names*

### Comparing `pybuildtools-0.5.7/buildtools/maestro/jinja2.py` & `pybuildtools-0.5.8/buildtools/maestro/jinja2.py`

 * *Files identical despite different names*

### Comparing `pybuildtools-0.5.7/buildtools/maestro/package_managers.py` & `pybuildtools-0.5.8/buildtools/maestro/package_managers.py`

 * *Files identical despite different names*

### Comparing `pybuildtools-0.5.7/buildtools/maestro/shell.py` & `pybuildtools-0.5.8/buildtools/maestro/shell.py`

 * *Files identical despite different names*

### Comparing `pybuildtools-0.5.7/buildtools/maestro/utils.py` & `pybuildtools-0.5.8/buildtools/maestro/utils.py`

 * *Files identical despite different names*

### Comparing `pybuildtools-0.5.7/buildtools/maestro/web.py` & `pybuildtools-0.5.8/buildtools/maestro/web.py`

 * *Files identical despite different names*

### Comparing `pybuildtools-0.5.7/buildtools/os_utils.py` & `pybuildtools-0.5.8/buildtools/os_utils.py`

 * *Files identical despite different names*

### Comparing `pybuildtools-0.5.7/buildtools/posix/elf.py` & `pybuildtools-0.5.8/buildtools/posix/elf.py`

 * *Files identical despite different names*

### Comparing `pybuildtools-0.5.7/buildtools/pygit2_callbacks.py` & `pybuildtools-0.5.8/buildtools/pygit2_callbacks.py`

 * *Files identical despite different names*

### Comparing `pybuildtools-0.5.7/buildtools/qconfig5.py` & `pybuildtools-0.5.8/buildtools/qconfig5.py`

 * *Files identical despite different names*

### Comparing `pybuildtools-0.5.7/buildtools/repo/base.py` & `pybuildtools-0.5.8/buildtools/repo/base.py`

 * *Files identical despite different names*

### Comparing `pybuildtools-0.5.7/buildtools/repo/git.py` & `pybuildtools-0.5.8/buildtools/repo/git.py`

 * *Files identical despite different names*

### Comparing `pybuildtools-0.5.7/buildtools/repo/hg.py` & `pybuildtools-0.5.8/buildtools/repo/hg.py`

 * *Files identical despite different names*

### Comparing `pybuildtools-0.5.7/buildtools/timing.py` & `pybuildtools-0.5.8/buildtools/timing.py`

 * *Files identical despite different names*

### Comparing `pybuildtools-0.5.7/buildtools/twisted_utils.py` & `pybuildtools-0.5.8/buildtools/twisted_utils.py`

 * *Files identical despite different names*

### Comparing `pybuildtools-0.5.7/buildtools/utils.py` & `pybuildtools-0.5.8/buildtools/utils.py`

 * *Files identical despite different names*

### Comparing `pybuildtools-0.5.7/buildtools/wrapper/__init__.py` & `pybuildtools-0.5.8/buildtools/wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `pybuildtools-0.5.7/buildtools/wrapper/ant.py` & `pybuildtools-0.5.8/buildtools/wrapper/ant.py`

 * *Files identical despite different names*

### Comparing `pybuildtools-0.5.7/buildtools/wrapper/ccache.py` & `pybuildtools-0.5.8/buildtools/wrapper/ccache.py`

 * *Files identical despite different names*

### Comparing `pybuildtools-0.5.7/buildtools/wrapper/cmake.py` & `pybuildtools-0.5.8/buildtools/wrapper/cmake.py`

 * *Files identical despite different names*

### Comparing `pybuildtools-0.5.7/buildtools/wrapper/cotire.py` & `pybuildtools-0.5.8/buildtools/wrapper/cotire.py`

 * *Files identical despite different names*

### Comparing `pybuildtools-0.5.7/buildtools/wrapper/distcc.py` & `pybuildtools-0.5.8/buildtools/wrapper/distcc.py`

 * *Files identical despite different names*

### Comparing `pybuildtools-0.5.7/buildtools/wrapper/fpm.py` & `pybuildtools-0.5.8/buildtools/wrapper/fpm.py`

 * *Files identical despite different names*

### Comparing `pybuildtools-0.5.7/buildtools/wrapper/git.py` & `pybuildtools-0.5.8/buildtools/wrapper/git.py`

 * *Files identical despite different names*

### Comparing `pybuildtools-0.5.7/pyproject.toml` & `pybuildtools-0.5.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pybuildtools"
-version = "0.5.7"
+version = "0.5.8"
 description = "A set of tools for putting together buildscripts and other CLI applications"
 authors = ["Rob Nelson <nexisentertainment@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://gitlab.com/N3X15/python-build-tools"
 repository = "https://gitlab.com/N3X15/python-build-tools.git"
 packages = [
```

### Comparing `pybuildtools-0.5.7/setup.py` & `pybuildtools-0.5.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['buildtools',
  'buildtools.buildsystem',
+ 'buildtools.cli',
+ 'buildtools.cli.nuitka_plus',
  'buildtools.ext',
  'buildtools.ext.salt',
  'buildtools.maestro',
  'buildtools.maestro.enumwriters',
  'buildtools.posix',
  'buildtools.repo',
  'buildtools.wrapper',
@@ -32,15 +34,15 @@
 extras_require = \
 {'all': ['Twisted>=22.10.0,<23.0.0', 'PyQt5>=5.15.9,<6.0.0'],
  'pyqt5': ['PyQt5>=5.15.9,<6.0.0'],
  'twisted': ['Twisted>=22.10.0,<23.0.0']}
 
 setup_kwargs = {
     'name': 'pybuildtools',
-    'version': '0.5.7',
+    'version': '0.5.8',
     'description': 'A set of tools for putting together buildscripts and other CLI applications',
     'long_description': "# python-build-tools\n\nA toolkit containing many powerful utilities, including:\n\n * OS utilities (buildtools.os_utils)\n * Indented logging with colorama support (buildtools.bt_logging.log)\n * The powerful Maestro build management system (buildtools.maestro)\n * A powerful VCS repository wrapper system (buildtools.repo)\n * A mess of other random things.\n\n## os_utils\n```python\nfrom buildtools import os_utils\n\n# Ensure test/ exists\nos_utils.ensureDirExists('test')\n\n# Get copy of current environmental variables.\nENV = os_utils.ENV.clone()\n\n# Add .bin/ to the beginning of PATH in our virtual environment\nENV.prependTo('PATH', '.bin/')\n\n# Remove any duplicate entries from PATH\nENV.removeDuplicatedEntries('PATH')\n\n# Find gcc in our virtual environment (checks PATHEXT on Windows, too!)\n# Returns the path to gcc, or None if it couldn't be found.\nGCC = ENV.which('gcc')\n\n# Ensure bash exists before continuing (same rules as above)\nENV.assertWhich('bash')\n\n# Bring up gcc's help page. Crash if non-0 exit code, echo command to console, and output STDOUT/STDERR to console.\nos_utils.cmd([GCC, '--help'], critical=True, echo=True, show_output=True)\n```\n\n## Logging\n```python\nfrom buildtools import log\n\ndef a():\n  log.info('This will be indented if a() is called in a log block.')\n\nlog.info('No indentation, yet.')\nwith log.warning('A warning. Next line will be indented.'):\n  log.error('Error!')\n  with log.info('The following function\\'s log output will be indented by another layer.')\n    a()\n    log.critical('So will %s!', 'this')\n```\n\n## Maestro\n```python\nfrom buildtools.maestro import BuildMaestro\nfrom buildtools.maestro.fileio import ReplaceTextTarget\nfrom buildtools.maestro.coffeescript import CoffeeBuildTarget\nfrom buildtools.maestro.web import SCSSBuildTarget, SCSSConvertTarget\n\nbm = BuildMaestro()\n\n# Compile CoffeeScript to JS\nbm.add(CoffeeBuildTarget('htdocs/js/vgws.js',                 ['coffee/src/vgws.coffee']))\nbm.add(CoffeeBuildTarget('htdocs/js/editpoll.multichoice.js', ['coffee/editpoll.multichoice.coffee'], dependencies=['htdocs/js/vgws.js']))\nbm.add(CoffeeBuildTarget('htdocs/js/editpoll.option.js',      ['coffee/editpoll.editpoll.coffee'], dependencies=['htdocs/js/vgws.js']))\n\n# Convert CSS to SCSS\nbm.add(SCSSBuildTarget('htdocs/css/style.css', ['style/style.scss'], [], import_paths=['style'], compass=True))\n\n# Compile, taking dependencies into count when ordering operations.\nbm.run()\n\n# Same as above, but providing command line arguments such as --clean, and --rebuild.\nbm.as_app()\n```\n",
     'author': 'Rob Nelson',
     'author_email': 'nexisentertainment@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://gitlab.com/N3X15/python-build-tools',
```

### Comparing `pybuildtools-0.5.7/PKG-INFO` & `pybuildtools-0.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybuildtools
-Version: 0.5.7
+Version: 0.5.8
 Summary: A set of tools for putting together buildscripts and other CLI applications
 Home-page: https://gitlab.com/N3X15/python-build-tools
 License: MIT
 Author: Rob Nelson
 Author-email: nexisentertainment@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

