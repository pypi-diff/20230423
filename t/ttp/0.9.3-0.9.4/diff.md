# Comparing `tmp/ttp-0.9.3.tar.gz` & `tmp/ttp-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ttp-0.9.3.tar", max compression
+gzip compressed data, was "ttp-0.9.4.tar", max compression
```

## Comparing `ttp-0.9.3.tar` & `ttp-0.9.4.tar`

### file list

```diff
@@ -1,90 +1,90 @@
--rw-r--r--   0        0        0     1065 2022-10-02 22:27:01.097014 ttp-0.9.3/LICENSE
--rw-r--r--   0        0        0     4035 2023-04-15 08:58:06.792729 ttp-0.9.3/pyproject.toml
--rw-r--r--   0        0        0     6414 2022-10-02 12:16:11.776605 ttp-0.9.3/README.md
--rw-r--r--   0        0        0      428 2023-04-14 23:57:06.307808 ttp-0.9.3/ttp/__init__.py
--rw-r--r--   0        0        0        0 2022-10-02 11:16:02.806688 ttp-0.9.3/ttp/formatters/__init__.py
--rw-r--r--   0        0        0      891 2022-10-02 22:39:44.441452 ttp-0.9.3/ttp/formatters/csv_formatter.py
--rw-r--r--   0        0        0     2519 2022-10-02 12:39:58.451379 ttp-0.9.3/ttp/formatters/excel_formatter.py
--rw-r--r--   0        0        0      777 2022-10-02 22:32:58.697313 ttp-0.9.3/ttp/formatters/jinja2_formatter.py
--rw-r--r--   0        0        0      243 2022-10-02 12:00:55.767339 ttp-0.9.3/ttp/formatters/json_formatter.py
--rw-r--r--   0        0        0     1545 2022-10-02 22:05:37.297996 ttp-0.9.3/ttp/formatters/n2g_formatter.py
--rw-r--r--   0        0        0      201 2022-10-02 11:46:07.107045 ttp-0.9.3/ttp/formatters/pprint_formatter.py
--rw-r--r--   0        0        0      115 2022-10-02 11:24:00.008627 ttp-0.9.3/ttp/formatters/raw_formatter.py
--rw-r--r--   0        0        0     2092 2022-10-02 21:54:55.247354 ttp-0.9.3/ttp/formatters/table_formatter.py
--rw-r--r--   0        0        0      812 2022-10-02 22:35:06.089841 ttp-0.9.3/ttp/formatters/tabulate_formatter.py
--rw-r--r--   0        0        0      493 2022-10-02 22:06:16.739838 ttp-0.9.3/ttp/formatters/yaml_formatter.py
--rw-r--r--   0        0        0        0 2022-10-02 11:16:02.810438 ttp-0.9.3/ttp/group/__init__.py
--rw-r--r--   0        0        0      358 2022-10-02 12:32:17.655647 ttp-0.9.3/ttp/group/contains.py
--rw-r--r--   0        0        0      338 2022-10-02 12:28:09.118285 ttp-0.9.3/ttp/group/contains_val.py
--rw-r--r--   0        0        0      376 2022-10-02 12:36:13.997743 ttp-0.9.3/ttp/group/containsall.py
--rw-r--r--   0        0        0      173 2022-10-02 11:36:49.239728 ttp-0.9.3/ttp/group/delete.py
--rw-r--r--   0        0        0      323 2022-10-02 12:24:23.165655 ttp-0.9.3/ttp/group/equal.py
--rw-r--r--   0        0        0      261 2022-10-02 12:06:43.385622 ttp-0.9.3/ttp/group/exclude.py
--rw-r--r--   0        0        0      415 2022-12-03 01:59:53.792168 ttp-0.9.3/ttp/group/exclude_val.py
--rw-r--r--   0        0        0      366 2022-10-02 12:34:00.830761 ttp-0.9.3/ttp/group/excludeall.py
--rw-r--r--   0        0        0      727 2022-10-02 22:29:03.282400 ttp-0.9.3/ttp/group/expand.py
--rw-r--r--   0        0        0     1303 2022-10-02 22:14:41.018871 ttp-0.9.3/ttp/group/itemize.py
--rw-r--r--   0        0        0      361 2022-10-02 12:32:57.284988 ttp-0.9.3/ttp/group/items2dict.py
--rw-r--r--   0        0        0     2526 2022-10-02 12:39:48.142079 ttp-0.9.3/ttp/group/lookup.py
--rw-r--r--   0        0        0      512 2022-10-02 22:09:01.851973 ttp-0.9.3/ttp/group/macro.py
--rw-r--r--   0        0        0      421 2022-10-02 21:54:34.639907 ttp-0.9.3/ttp/group/record.py
--rw-r--r--   0        0        0      686 2022-10-02 22:25:48.517202 ttp-0.9.3/ttp/group/set_.py
--rw-r--r--   0        0        0      671 2022-10-02 22:24:36.018618 ttp-0.9.3/ttp/group/sformat.py
--rw-r--r--   0        0        0      686 2022-10-02 22:25:49.107690 ttp-0.9.3/ttp/group/to_converters.py
--rw-r--r--   0        0        0      386 2022-10-02 12:38:04.642781 ttp-0.9.3/ttp/group/to_ip.py
--rw-r--r--   0        0        0     2768 2022-12-03 02:00:16.317825 ttp-0.9.3/ttp/group/validate_cerberus.py
--rw-r--r--   0        0        0       79 2022-10-02 11:21:04.435047 ttp-0.9.3/ttp/group/void.py
--rw-r--r--   0        0        0        0 2022-10-02 11:16:02.790022 ttp-0.9.3/ttp/input/__init__.py
--rw-r--r--   0        0        0      606 2022-10-02 22:19:20.241356 ttp-0.9.3/ttp/input/commands.py
--rw-r--r--   0        0        0      350 2022-10-02 12:30:51.321783 ttp-0.9.3/ttp/input/macro.py
--rw-r--r--   0        0        0      124 2022-10-02 11:25:45.007132 ttp-0.9.3/ttp/input/test.py
--rw-r--r--   0        0        0        0 2022-10-02 11:16:02.776895 ttp-0.9.3/ttp/lookup/__init__.py
--rw-r--r--   0        0        0     1482 2022-10-02 22:07:38.694082 ttp-0.9.3/ttp/lookup/geoip2.py
--rw-r--r--   0        0        0        0 2022-10-02 11:16:02.799997 ttp-0.9.3/ttp/match/__init__.py
--rw-r--r--   0        0        0      153 2022-12-03 11:52:49.025726 ttp-0.9.3/ttp/match/copy_.py
--rw-r--r--   0        0        0      347 2022-12-03 01:58:48.838563 ttp-0.9.3/ttp/match/count.py
--rw-r--r--   0        0        0     2401 2022-10-02 12:41:34.803860 ttp-0.9.3/ttp/match/dns_lookups.py
--rw-r--r--   0        0        0     2975 2022-10-02 12:35:10.123040 ttp-0.9.3/ttp/match/geoip_lookup.py
--rw-r--r--   0        0        0     6080 2022-12-03 01:58:26.560255 ttp-0.9.3/ttp/match/ip.py
--rw-r--r--   0        0        0      697 2022-10-02 22:26:47.115914 ttp-0.9.3/ttp/match/item.py
--rw-r--r--   0        0        0       64 2022-10-02 11:20:31.576928 ttp-0.9.3/ttp/match/joinmatches.py
--rw-r--r--   0        0        0      248 2022-10-02 12:02:47.361627 ttp-0.9.3/ttp/match/let.py
--rw-r--r--   0        0        0     4237 2022-12-03 01:57:42.950828 ttp-0.9.3/ttp/match/lookup.py
--rw-r--r--   0        0        0      799 2022-10-02 22:34:23.774520 ttp-0.9.3/ttp/match/mac_eui.py
--rw-r--r--   0        0        0      522 2022-10-02 22:10:07.904632 ttp-0.9.3/ttp/match/macro.py
--rw-r--r--   0        0        0      110 2022-10-02 11:23:17.673227 ttp-0.9.3/ttp/match/raise_.py
--rw-r--r--   0        0        0     2084 2022-12-03 01:56:47.519349 ttp-0.9.3/ttp/match/re_.py
--rw-r--r--   0        0        0      141 2022-12-03 01:57:08.150264 ttp-0.9.3/ttp/match/record.py
--rw-r--r--   0        0        0      424 2022-12-03 01:57:21.703876 ttp-0.9.3/ttp/match/set_.py
--rw-r--r--   0        0        0     3251 2022-12-03 02:02:43.751562 ttp-0.9.3/ttp/match/string.py
--rw-r--r--   0        0        0     1036 2022-10-02 22:29:14.953215 ttp-0.9.3/ttp/match/to.py
--rw-r--r--   0        0        0     1249 2022-10-02 22:17:14.438625 ttp-0.9.3/ttp/match/unrange.py
--rw-r--r--   0        0        0     2560 2022-10-02 12:39:24.202585 ttp-0.9.3/ttp/match/uptimeparse.py
--rw-r--r--   0        0        0       79 2022-10-02 11:21:02.412304 ttp-0.9.3/ttp/match/void.py
--rw-r--r--   0        0        0        0 2022-10-02 11:16:02.802945 ttp-0.9.3/ttp/output/__init__.py
--rw-r--r--   0        0        0     3357 2022-10-02 12:32:02.924852 ttp-0.9.3/ttp/output/deepdiffer.py
--rw-r--r--   0        0        0      507 2022-10-02 22:08:21.766679 ttp-0.9.3/ttp/output/is_equal.py
--rw-r--r--   0        0        0      230 2022-10-02 11:56:47.370840 ttp-0.9.3/ttp/output/macro.py
--rw-r--r--   0        0        0     2210 2022-10-02 12:43:48.102403 ttp-0.9.3/ttp/output/transform.py
--rw-r--r--   0        0        0     2011 2022-10-02 21:56:01.269058 ttp-0.9.3/ttp/output/validate_cerberus.py
--rw-r--r--   0        0        0     8469 2022-10-02 12:10:13.579428 ttp-0.9.3/ttp/output/validate_yangson.py
--rw-r--r--   0        0        0        0 2022-10-02 11:16:02.787032 ttp-0.9.3/ttp/patterns/__init__.py
--rw-r--r--   0        0        0      593 2022-10-02 22:17:58.693165 ttp-0.9.3/ttp/patterns/get_pattern.py
--rw-r--r--   0        0        0        0 2022-10-02 11:16:02.793015 ttp-0.9.3/ttp/returners/__init__.py
--rw-r--r--   0        0        0     1680 2022-10-02 22:02:36.320460 ttp-0.9.3/ttp/returners/file_returner.py
--rw-r--r--   0        0        0      197 2022-10-02 11:44:50.079655 ttp-0.9.3/ttp/returners/self_returner.py
--rw-r--r--   0        0        0     2938 2022-10-02 12:35:24.240884 ttp-0.9.3/ttp/returners/syslog_returner.py
--rw-r--r--   0        0        0     1882 2022-10-02 21:58:21.128182 ttp-0.9.3/ttp/returners/terminal_returner.py
--rw-r--r--   0        0        0   156114 2023-04-15 08:28:46.606730 ttp-0.9.3/ttp/ttp.py
--rw-r--r--   0        0        0        0 2022-10-02 11:16:02.769368 ttp-0.9.3/ttp/utils/__init__.py
--rw-r--r--   0        0        0     2778 2022-10-02 12:36:46.909720 ttp-0.9.3/ttp/utils/get_attributes.py
--rw-r--r--   0        0        0      157 2022-10-02 11:32:16.246029 ttp-0.9.3/ttp/utils/guess.py
--rw-r--r--   0        0        0     1157 2022-10-02 22:21:07.735695 ttp-0.9.3/ttp/utils/load_python_exec_py2.py
--rw-r--r--   0        0        0      955 2022-10-02 22:36:33.000288 ttp-0.9.3/ttp/utils/load_python_exec_py3.py
--rw-r--r--   0        0        0    10511 2022-10-02 12:06:18.417379 ttp-0.9.3/ttp/utils/loaders.py
--rw-r--r--   0        0        0     1454 2022-10-02 22:08:49.259463 ttp-0.9.3/ttp/utils/quick_parse.py
--rw-r--r--   0        0        0        0 2022-10-02 11:16:02.814177 ttp-0.9.3/ttp/variable/__init__.py
--rw-r--r--   0        0        0       88 2022-10-02 11:21:26.955490 ttp-0.9.3/ttp/variable/getfilename.py
--rw-r--r--   0        0        0     1792 2022-10-02 21:59:56.076938 ttp-0.9.3/ttp/variable/gethostname.py
--rw-r--r--   0        0        0     1107 2022-10-02 22:24:21.974076 ttp-0.9.3/ttp/variable/time_funcs.py
--rw-r--r--   0        0        0     9570 1970-01-01 00:00:00.000000 ttp-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-10-02 22:27:01.097014 ttp-0.9.4/LICENSE
+-rw-r--r--   0        0        0     4035 2023-04-23 13:26:43.991381 ttp-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0     6414 2022-10-02 12:16:11.776605 ttp-0.9.4/README.md
+-rw-r--r--   0        0        0      428 2023-04-23 13:27:02.097123 ttp-0.9.4/ttp/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-02 11:16:02.806688 ttp-0.9.4/ttp/formatters/__init__.py
+-rw-r--r--   0        0        0      891 2022-10-02 22:39:44.441452 ttp-0.9.4/ttp/formatters/csv_formatter.py
+-rw-r--r--   0        0        0     2519 2022-10-02 12:39:58.451379 ttp-0.9.4/ttp/formatters/excel_formatter.py
+-rw-r--r--   0        0        0      777 2022-10-02 22:32:58.697313 ttp-0.9.4/ttp/formatters/jinja2_formatter.py
+-rw-r--r--   0        0        0      243 2022-10-02 12:00:55.767339 ttp-0.9.4/ttp/formatters/json_formatter.py
+-rw-r--r--   0        0        0     1545 2022-10-02 22:05:37.297996 ttp-0.9.4/ttp/formatters/n2g_formatter.py
+-rw-r--r--   0        0        0      201 2022-10-02 11:46:07.107045 ttp-0.9.4/ttp/formatters/pprint_formatter.py
+-rw-r--r--   0        0        0      115 2022-10-02 11:24:00.008627 ttp-0.9.4/ttp/formatters/raw_formatter.py
+-rw-r--r--   0        0        0     2092 2022-10-02 21:54:55.247354 ttp-0.9.4/ttp/formatters/table_formatter.py
+-rw-r--r--   0        0        0      812 2022-10-02 22:35:06.089841 ttp-0.9.4/ttp/formatters/tabulate_formatter.py
+-rw-r--r--   0        0        0      493 2022-10-02 22:06:16.739838 ttp-0.9.4/ttp/formatters/yaml_formatter.py
+-rw-r--r--   0        0        0        0 2022-10-02 11:16:02.810438 ttp-0.9.4/ttp/group/__init__.py
+-rw-r--r--   0        0        0      358 2022-10-02 12:32:17.655647 ttp-0.9.4/ttp/group/contains.py
+-rw-r--r--   0        0        0      338 2022-10-02 12:28:09.118285 ttp-0.9.4/ttp/group/contains_val.py
+-rw-r--r--   0        0        0      376 2022-10-02 12:36:13.997743 ttp-0.9.4/ttp/group/containsall.py
+-rw-r--r--   0        0        0      173 2022-10-02 11:36:49.239728 ttp-0.9.4/ttp/group/delete.py
+-rw-r--r--   0        0        0      323 2022-10-02 12:24:23.165655 ttp-0.9.4/ttp/group/equal.py
+-rw-r--r--   0        0        0      261 2022-10-02 12:06:43.385622 ttp-0.9.4/ttp/group/exclude.py
+-rw-r--r--   0        0        0      415 2022-12-03 01:59:53.792168 ttp-0.9.4/ttp/group/exclude_val.py
+-rw-r--r--   0        0        0      366 2022-10-02 12:34:00.830761 ttp-0.9.4/ttp/group/excludeall.py
+-rw-r--r--   0        0        0      727 2023-04-23 13:27:49.848124 ttp-0.9.4/ttp/group/expand.py
+-rw-r--r--   0        0        0     1303 2022-10-02 22:14:41.018871 ttp-0.9.4/ttp/group/itemize.py
+-rw-r--r--   0        0        0      361 2022-10-02 12:32:57.284988 ttp-0.9.4/ttp/group/items2dict.py
+-rw-r--r--   0        0        0     2526 2022-10-02 12:39:48.142079 ttp-0.9.4/ttp/group/lookup.py
+-rw-r--r--   0        0        0      512 2022-10-02 22:09:01.851973 ttp-0.9.4/ttp/group/macro.py
+-rw-r--r--   0        0        0      421 2022-10-02 21:54:34.639907 ttp-0.9.4/ttp/group/record.py
+-rw-r--r--   0        0        0      686 2022-10-02 22:25:48.517202 ttp-0.9.4/ttp/group/set_.py
+-rw-r--r--   0        0        0      671 2022-10-02 22:24:36.018618 ttp-0.9.4/ttp/group/sformat.py
+-rw-r--r--   0        0        0      686 2022-10-02 22:25:49.107690 ttp-0.9.4/ttp/group/to_converters.py
+-rw-r--r--   0        0        0      386 2022-10-02 12:38:04.642781 ttp-0.9.4/ttp/group/to_ip.py
+-rw-r--r--   0        0        0     2768 2022-12-03 02:00:16.317825 ttp-0.9.4/ttp/group/validate_cerberus.py
+-rw-r--r--   0        0        0       79 2022-10-02 11:21:04.435047 ttp-0.9.4/ttp/group/void.py
+-rw-r--r--   0        0        0        0 2022-10-02 11:16:02.790022 ttp-0.9.4/ttp/input/__init__.py
+-rw-r--r--   0        0        0      606 2022-10-02 22:19:20.241356 ttp-0.9.4/ttp/input/commands.py
+-rw-r--r--   0        0        0      350 2022-10-02 12:30:51.321783 ttp-0.9.4/ttp/input/macro.py
+-rw-r--r--   0        0        0      124 2022-10-02 11:25:45.007132 ttp-0.9.4/ttp/input/test.py
+-rw-r--r--   0        0        0        0 2022-10-02 11:16:02.776895 ttp-0.9.4/ttp/lookup/__init__.py
+-rw-r--r--   0        0        0     1482 2022-10-02 22:07:38.694082 ttp-0.9.4/ttp/lookup/geoip2.py
+-rw-r--r--   0        0        0        0 2022-10-02 11:16:02.799997 ttp-0.9.4/ttp/match/__init__.py
+-rw-r--r--   0        0        0      153 2022-12-03 11:52:49.025726 ttp-0.9.4/ttp/match/copy_.py
+-rw-r--r--   0        0        0      347 2022-12-03 01:58:48.838563 ttp-0.9.4/ttp/match/count.py
+-rw-r--r--   0        0        0     2401 2022-10-02 12:41:34.803860 ttp-0.9.4/ttp/match/dns_lookups.py
+-rw-r--r--   0        0        0     2975 2022-10-02 12:35:10.123040 ttp-0.9.4/ttp/match/geoip_lookup.py
+-rw-r--r--   0        0        0     6080 2022-12-03 01:58:26.560255 ttp-0.9.4/ttp/match/ip.py
+-rw-r--r--   0        0        0      697 2022-10-02 22:26:47.115914 ttp-0.9.4/ttp/match/item.py
+-rw-r--r--   0        0        0       64 2022-10-02 11:20:31.576928 ttp-0.9.4/ttp/match/joinmatches.py
+-rw-r--r--   0        0        0      248 2022-10-02 12:02:47.361627 ttp-0.9.4/ttp/match/let.py
+-rw-r--r--   0        0        0     4237 2022-12-03 01:57:42.950828 ttp-0.9.4/ttp/match/lookup.py
+-rw-r--r--   0        0        0      799 2022-10-02 22:34:23.774520 ttp-0.9.4/ttp/match/mac_eui.py
+-rw-r--r--   0        0        0      522 2022-10-02 22:10:07.904632 ttp-0.9.4/ttp/match/macro.py
+-rw-r--r--   0        0        0      110 2022-10-02 11:23:17.673227 ttp-0.9.4/ttp/match/raise_.py
+-rw-r--r--   0        0        0     2084 2022-12-03 01:56:47.519349 ttp-0.9.4/ttp/match/re_.py
+-rw-r--r--   0        0        0      141 2022-12-03 01:57:08.150264 ttp-0.9.4/ttp/match/record.py
+-rw-r--r--   0        0        0      424 2022-12-03 01:57:21.703876 ttp-0.9.4/ttp/match/set_.py
+-rw-r--r--   0        0        0     3251 2022-12-03 02:02:43.751562 ttp-0.9.4/ttp/match/string.py
+-rw-r--r--   0        0        0     1036 2022-10-02 22:29:14.953215 ttp-0.9.4/ttp/match/to.py
+-rw-r--r--   0        0        0     1249 2022-10-02 22:17:14.438625 ttp-0.9.4/ttp/match/unrange.py
+-rw-r--r--   0        0        0     2560 2022-10-02 12:39:24.202585 ttp-0.9.4/ttp/match/uptimeparse.py
+-rw-r--r--   0        0        0       79 2022-10-02 11:21:02.412304 ttp-0.9.4/ttp/match/void.py
+-rw-r--r--   0        0        0        0 2022-10-02 11:16:02.802945 ttp-0.9.4/ttp/output/__init__.py
+-rw-r--r--   0        0        0     3357 2022-10-02 12:32:02.924852 ttp-0.9.4/ttp/output/deepdiffer.py
+-rw-r--r--   0        0        0      507 2022-10-02 22:08:21.766679 ttp-0.9.4/ttp/output/is_equal.py
+-rw-r--r--   0        0        0      230 2022-10-02 11:56:47.370840 ttp-0.9.4/ttp/output/macro.py
+-rw-r--r--   0        0        0     2210 2022-10-02 12:43:48.102403 ttp-0.9.4/ttp/output/transform.py
+-rw-r--r--   0        0        0     2011 2022-10-02 21:56:01.269058 ttp-0.9.4/ttp/output/validate_cerberus.py
+-rw-r--r--   0        0        0     8469 2022-10-02 12:10:13.579428 ttp-0.9.4/ttp/output/validate_yangson.py
+-rw-r--r--   0        0        0        0 2022-10-02 11:16:02.787032 ttp-0.9.4/ttp/patterns/__init__.py
+-rw-r--r--   0        0        0      593 2022-10-02 22:17:58.693165 ttp-0.9.4/ttp/patterns/get_pattern.py
+-rw-r--r--   0        0        0        0 2022-10-02 11:16:02.793015 ttp-0.9.4/ttp/returners/__init__.py
+-rw-r--r--   0        0        0     1680 2022-10-02 22:02:36.320460 ttp-0.9.4/ttp/returners/file_returner.py
+-rw-r--r--   0        0        0      197 2022-10-02 11:44:50.079655 ttp-0.9.4/ttp/returners/self_returner.py
+-rw-r--r--   0        0        0     2938 2022-10-02 12:35:24.240884 ttp-0.9.4/ttp/returners/syslog_returner.py
+-rw-r--r--   0        0        0     1882 2022-10-02 21:58:21.128182 ttp-0.9.4/ttp/returners/terminal_returner.py
+-rw-r--r--   0        0        0   156953 2023-04-23 13:26:50.271812 ttp-0.9.4/ttp/ttp.py
+-rw-r--r--   0        0        0        0 2022-10-02 11:16:02.769368 ttp-0.9.4/ttp/utils/__init__.py
+-rw-r--r--   0        0        0     2778 2022-10-02 12:36:46.909720 ttp-0.9.4/ttp/utils/get_attributes.py
+-rw-r--r--   0        0        0      157 2022-10-02 11:32:16.246029 ttp-0.9.4/ttp/utils/guess.py
+-rw-r--r--   0        0        0     1157 2022-10-02 22:21:07.735695 ttp-0.9.4/ttp/utils/load_python_exec_py2.py
+-rw-r--r--   0        0        0      955 2022-10-02 22:36:33.000288 ttp-0.9.4/ttp/utils/load_python_exec_py3.py
+-rw-r--r--   0        0        0    10511 2022-10-02 12:06:18.417379 ttp-0.9.4/ttp/utils/loaders.py
+-rw-r--r--   0        0        0     1454 2022-10-02 22:08:49.259463 ttp-0.9.4/ttp/utils/quick_parse.py
+-rw-r--r--   0        0        0        0 2022-10-02 11:16:02.814177 ttp-0.9.4/ttp/variable/__init__.py
+-rw-r--r--   0        0        0       88 2022-10-02 11:21:26.955490 ttp-0.9.4/ttp/variable/getfilename.py
+-rw-r--r--   0        0        0     1792 2022-10-02 21:59:56.076938 ttp-0.9.4/ttp/variable/gethostname.py
+-rw-r--r--   0        0        0     1107 2022-10-02 22:24:21.974076 ttp-0.9.4/ttp/variable/time_funcs.py
+-rw-r--r--   0        0        0     9570 1970-01-01 00:00:00.000000 ttp-0.9.4/PKG-INFO
```

### Comparing `ttp-0.9.3/LICENSE` & `ttp-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ttp-0.9.3/pyproject.toml` & `ttp-0.9.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ttp"
-version = "0.9.3"
+version = "0.9.4"
 description = "Template Text Parser"
 authors = ["Denis Mulyalin <d.mulyalin@gmail.com>"]
 maintainers = ["Denis Mulyalin <d.mulyalin@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/dmulyalin/ttp"
 repository = "https://github.com/dmulyalin/ttp"
```

### Comparing `ttp-0.9.3/README.md` & `ttp-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `ttp-0.9.3/ttp/formatters/csv_formatter.py` & `ttp-0.9.4/ttp/formatters/csv_formatter.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.3/ttp/formatters/excel_formatter.py` & `ttp-0.9.4/ttp/formatters/excel_formatter.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.3/ttp/formatters/jinja2_formatter.py` & `ttp-0.9.4/ttp/formatters/jinja2_formatter.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.3/ttp/formatters/n2g_formatter.py` & `ttp-0.9.4/ttp/formatters/n2g_formatter.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.3/ttp/formatters/table_formatter.py` & `ttp-0.9.4/ttp/formatters/table_formatter.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.3/ttp/formatters/tabulate_formatter.py` & `ttp-0.9.4/ttp/formatters/tabulate_formatter.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.3/ttp/group/expand.py` & `ttp-0.9.4/ttp/group/expand.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.3/ttp/group/itemize.py` & `ttp-0.9.4/ttp/group/itemize.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.3/ttp/group/lookup.py` & `ttp-0.9.4/ttp/group/lookup.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.3/ttp/group/macro.py` & `ttp-0.9.4/ttp/group/macro.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.3/ttp/group/set_.py` & `ttp-0.9.4/ttp/group/set_.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.3/ttp/group/sformat.py` & `ttp-0.9.4/ttp/group/sformat.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.3/ttp/group/to_converters.py` & `ttp-0.9.4/ttp/group/to_converters.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.3/ttp/group/validate_cerberus.py` & `ttp-0.9.4/ttp/group/validate_cerberus.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.3/ttp/input/commands.py` & `ttp-0.9.4/ttp/input/commands.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.3/ttp/lookup/geoip2.py` & `ttp-0.9.4/ttp/lookup/geoip2.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.3/ttp/match/dns_lookups.py` & `ttp-0.9.4/ttp/match/dns_lookups.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.3/ttp/match/geoip_lookup.py` & `ttp-0.9.4/ttp/match/geoip_lookup.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.3/ttp/match/ip.py` & `ttp-0.9.4/ttp/match/ip.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.3/ttp/match/item.py` & `ttp-0.9.4/ttp/match/item.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.3/ttp/match/lookup.py` & `ttp-0.9.4/ttp/match/lookup.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.3/ttp/match/mac_eui.py` & `ttp-0.9.4/ttp/match/mac_eui.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.3/ttp/match/macro.py` & `ttp-0.9.4/ttp/match/macro.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.3/ttp/match/re_.py` & `ttp-0.9.4/ttp/match/re_.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.3/ttp/match/string.py` & `ttp-0.9.4/ttp/match/string.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.3/ttp/match/to.py` & `ttp-0.9.4/ttp/match/to.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.3/ttp/match/unrange.py` & `ttp-0.9.4/ttp/match/unrange.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.3/ttp/match/uptimeparse.py` & `ttp-0.9.4/ttp/match/uptimeparse.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.3/ttp/output/deepdiffer.py` & `ttp-0.9.4/ttp/output/deepdiffer.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.3/ttp/output/transform.py` & `ttp-0.9.4/ttp/output/transform.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.3/ttp/output/validate_cerberus.py` & `ttp-0.9.4/ttp/output/validate_cerberus.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.3/ttp/output/validate_yangson.py` & `ttp-0.9.4/ttp/output/validate_yangson.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.3/ttp/patterns/get_pattern.py` & `ttp-0.9.4/ttp/patterns/get_pattern.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.3/ttp/returners/file_returner.py` & `ttp-0.9.4/ttp/returners/file_returner.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.3/ttp/returners/syslog_returner.py` & `ttp-0.9.4/ttp/returners/syslog_returner.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.3/ttp/returners/terminal_returner.py` & `ttp-0.9.4/ttp/returners/terminal_returner.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.3/ttp/ttp.py` & `ttp-0.9.4/ttp/ttp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-__version__ = "0.9.3"
+__version__ = "0.9.4"
 
 import re
 import os
 import logging
 import copy
 import ast
 import pickle
@@ -3027,14 +3027,29 @@
                 # transform ELEMENT dict to list and append data to it:
                 self.results = self.value_to_list(
                     DATA=self.results, PATH=result_path, result=result_data
                 )
             else:
                 E.update(result_data)
 
+    def reconstruct_last_element(self, result_data, result_path):
+        """
+        Method to retrieve last element value, make a copy of it and nerge with
+        current results. This is to reconstruct group results for processing in
+        a case where we have tail matches.
+        """
+        # get ELEMENT from self.results by result_path
+        E = self.dict_by_path(PATH=result_path, ELEMENT=self.results)
+        if isinstance(E, list):
+            copied = E[-1].copy()
+        elif isinstance(E, dict):
+            copied = E.copy()
+        copied.update(result_data)
+        return copied
+    
     def start(self, result, PATH, DEFAULTS=None, FUNCTIONS=None, REDICT=""):
         DEFAULTS = DEFAULTS or {}
         FUNCTIONS = FUNCTIONS or []
         # perform group path tracing
         while self.started_groups:
             # check if child group started
             if REDICT["GROUP"].parent_group_id == self.started_groups[-1]:
@@ -3217,27 +3232,30 @@
         return path
 
     def processgrp(self):
         """Method to process group results"""
         # add default values to group results
         for k, v in self.record["DEFAULTS"].items():
             self.record["result"].setdefault(k, v)
+        # if merge_with_last - tail match, attempt to reconstruct group result 
+        # this only will work if self.record["result"] contains enough info to form PATH        
+        if self.record.get("merge_with_last") is True:
+            processed_path = self.form_path(list(self.record["PATH"]))
+            if processed_path:
+                self.record["result"] = self.reconstruct_last_element(self.record["result"], processed_path)
         # process group functions
         for item in self.record["FUNCTIONS"]:
             func_name = item["name"]
             args = item.get("args", [])
             kwargs = item.get("kwargs", {})
             # run group functions
             self.record["result"], flags = self._ttp_["group"][func_name](
                 self.record["result"], *args, **kwargs
             )
-            # if conditions check been false, return False except when
-            # results marked as merge_with_last, this logic is weak but 
-            # simplest to fix issue #103
-            if flags == False and self.record.get("merge_with_last") != True:
+            if flags == False:
                 return False
         processed_path = self.form_path(self.record["PATH"])
         if processed_path:
             self.record["PATH"] = processed_path
         else:
             return False
```

### Comparing `ttp-0.9.3/ttp/utils/get_attributes.py` & `ttp-0.9.4/ttp/utils/get_attributes.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.3/ttp/utils/load_python_exec_py2.py` & `ttp-0.9.4/ttp/utils/load_python_exec_py2.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.3/ttp/utils/load_python_exec_py3.py` & `ttp-0.9.4/ttp/utils/load_python_exec_py3.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.3/ttp/utils/loaders.py` & `ttp-0.9.4/ttp/utils/loaders.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.3/ttp/utils/quick_parse.py` & `ttp-0.9.4/ttp/utils/quick_parse.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.3/ttp/variable/gethostname.py` & `ttp-0.9.4/ttp/variable/gethostname.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.3/ttp/variable/time_funcs.py` & `ttp-0.9.4/ttp/variable/time_funcs.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.3/PKG-INFO` & `ttp-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ttp
-Version: 0.9.3
+Version: 0.9.4
 Summary: Template Text Parser
 Home-page: https://github.com/dmulyalin/ttp
 License: MIT
 Keywords: Parsing,TTP,regex
 Author: Denis Mulyalin
 Author-email: d.mulyalin@gmail.com
 Maintainer: Denis Mulyalin
```

