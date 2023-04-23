# Comparing `tmp/hak-0.0.8.tar.gz` & `tmp/hak-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hak-0.0.8.tar", last modified: Wed Apr 19 10:19:54 2023, max compression
+gzip compressed data, was "hak-0.0.9.tar", last modified: Wed Apr 19 10:43:20 2023, max compression
```

## Comparing `hak-0.0.8.tar` & `hak-0.0.9.tar`

### file list

```diff
@@ -1,369 +1,369 @@
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.990774 hak-0.0.8/
--rw-rw-r--   0 a         (1009) a         (1010)     1068 2023-04-19 01:55:38.000000 hak-0.0.8/LICENSE
--rw-rw-r--   0 a         (1009) a         (1010)      994 2023-04-19 10:19:54.990774 hak-0.0.8/PKG-INFO
--rw-rw-r--   0 a         (1009) a         (1010)      406 2023-04-19 03:24:53.000000 hak-0.0.8/README.md
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.982773 hak-0.0.8/hak/
--rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.8/hak/__init__.py
--rw-rw-r--   0 a         (1009) a         (1010)      140 2023-04-19 01:55:38.000000 hak-0.0.8/hak/a_equals_b.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.982773 hak-0.0.8/hak/bool/
--rw-rw-r--   0 a         (1009) a         (1010)       86 2023-04-19 01:55:38.000000 hak-0.0.8/hak/bool/fake.py
--rw-rw-r--   0 a         (1009) a         (1010)      103 2023-04-19 01:55:38.000000 hak-0.0.8/hak/bool/is_a.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.982773 hak-0.0.8/hak/bool/or_none/
--rw-rw-r--   0 a         (1009) a         (1010)      160 2023-04-19 01:55:38.000000 hak-0.0.8/hak/bool/or_none/fake.py
--rw-rw-r--   0 a         (1009) a         (1010)      125 2023-04-19 01:55:38.000000 hak-0.0.8/hak/bool/or_none/is_a.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.982773 hak-0.0.8/hak/bools/
--rw-rw-r--   0 a         (1009) a         (1010)      139 2023-04-19 01:55:38.000000 hak-0.0.8/hak/bools/count_true.py
--rw-rw-r--   0 a         (1009) a         (1010)      249 2023-04-19 01:55:38.000000 hak-0.0.8/hak/calculate_duration_bar_width.py
--rw-rw-r--   0 a         (1009) a         (1010)      758 2023-04-19 01:55:38.000000 hak-0.0.8/hak/check_if_ok_to_proceed.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.982773 hak-0.0.8/hak/date/
--rw-rw-r--   0 a         (1009) a         (1010)      143 2023-04-19 01:55:38.000000 hak-0.0.8/hak/date/is_a.py
--rw-rw-r--   0 a         (1009) a         (1010)      347 2023-04-19 01:55:38.000000 hak-0.0.8/hak/date/is_first_second_or_third_day_of_month.py
--rw-rw-r--   0 a         (1009) a         (1010)      414 2023-04-19 01:55:38.000000 hak-0.0.8/hak/date/is_first_week_of_quarter.py
--rw-rw-r--   0 a         (1009) a         (1010)      208 2023-04-19 01:55:38.000000 hak-0.0.8/hak/date/is_monday.py
--rw-rw-r--   0 a         (1009) a         (1010)      462 2023-04-19 01:55:38.000000 hak-0.0.8/hak/date/is_weekday.py
--rw-rw-r--   0 a         (1009) a         (1010)      467 2023-04-19 01:55:38.000000 hak-0.0.8/hak/date/is_weekend.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.982773 hak-0.0.8/hak/date/public_holiday/
--rw-rw-r--   0 a         (1009) a         (1010)     5617 2023-04-19 01:55:38.000000 hak-0.0.8/hak/date/public_holiday/is_a.py
--rw-rw-r--   0 a         (1009) a         (1010)      385 2023-04-19 01:55:38.000000 hak-0.0.8/hak/date/select_from_last_n_days.py
--rw-rw-r--   0 a         (1009) a         (1010)      146 2023-04-19 01:55:38.000000 hak-0.0.8/hak/date/to_dd_mm_yyyy_str.py
--rw-rw-r--   0 a         (1009) a         (1010)      605 2023-04-19 03:01:25.000000 hak-0.0.8/hak/date/to_utc_timestamp.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.978773 hak-0.0.8/hak/date/year/
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.982773 hak-0.0.8/hak/date/year/easter_sunday/
--rw-rw-r--   0 a         (1009) a         (1010)     1006 2023-04-19 01:55:38.000000 hak-0.0.8/hak/date/year/easter_sunday/get.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.982773 hak-0.0.8/hak/datetime/
--rw-rw-r--   0 a         (1009) a         (1010)      149 2023-04-19 01:55:38.000000 hak-0.0.8/hak/datetime/is_a.py
--rw-rw-r--   0 a         (1009) a         (1010)      272 2023-04-19 01:55:38.000000 hak-0.0.8/hak/datetime/select_from_last_n_days.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.982773 hak-0.0.8/hak/dict/
--rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.8/hak/dict/__init__.py
--rw-rw-r--   0 a         (1009) a         (1010)      215 2023-04-19 01:55:38.000000 hak-0.0.8/hak/dict/convert_to_sql_insertable.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.982773 hak-0.0.8/hak/dict/frequencies/
--rw-rw-r--   0 a         (1009) a         (1010)      356 2023-04-19 01:55:38.000000 hak-0.0.8/hak/dict/frequencies/choose.py
--rw-rw-r--   0 a         (1009) a         (1010)      376 2023-04-19 01:55:38.000000 hak-0.0.8/hak/dict/frequencies/make_from_strings.py
--rw-rw-r--   0 a         (1009) a         (1010)      187 2023-04-19 01:55:38.000000 hak-0.0.8/hak/dict/get_or_default.py
--rw-rw-r--   0 a         (1009) a         (1010)      190 2023-04-19 01:55:38.000000 hak-0.0.8/hak/dict/is_a.py
--rw-rw-r--   0 a         (1009) a         (1010)      116 2023-04-19 01:55:38.000000 hak-0.0.8/hak/dict/make_from_key_value_lists.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.982773 hak-0.0.8/hak/dict/proposed_dismantlement/
--rw-rw-r--   0 a         (1009) a         (1010)     1520 2023-04-19 01:55:38.000000 hak-0.0.8/hak/dict/proposed_dismantlement/show.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.982773 hak-0.0.8/hak/dict/test_durations/
--rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.8/hak/dict/test_durations/__init__.py
--rw-rw-r--   0 a         (1009) a         (1010)      134 2023-04-19 01:55:38.000000 hak-0.0.8/hak/dict/test_durations/to_tuple_list_sorted_by_duration.py
--rw-rw-r--   0 a         (1009) a         (1010)     4011 2023-04-19 01:55:38.000000 hak-0.0.8/hak/dict/to_max_line_width_str.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.982773 hak-0.0.8/hak/dicts/
--rw-rw-r--   0 a         (1009) a         (1010)      151 2023-04-19 01:55:38.000000 hak-0.0.8/hak/dicts/a_into_b.py
--rw-rw-r--   0 a         (1009) a         (1010)     1200 2023-04-19 01:55:38.000000 hak-0.0.8/hak/dicts/compare.py
--rw-rw-r--   0 a         (1009) a         (1010)      195 2023-04-19 01:55:38.000000 hak-0.0.8/hak/dicts/is_a.py
--rw-rw-r--   0 a         (1009) a         (1010)      663 2023-04-19 01:55:38.000000 hak-0.0.8/hak/dicts/merge_freq_dicts.py
--rw-rw-r--   0 a         (1009) a         (1010)      251 2023-04-19 01:55:38.000000 hak-0.0.8/hak/dicts/reindex.py
--rw-rw-r--   0 a         (1009) a         (1010)      203 2023-04-19 01:55:38.000000 hak-0.0.8/hak/dicts/sort_by_key.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.982773 hak-0.0.8/hak/directories/
--rw-rw-r--   0 a         (1009) a         (1010)      567 2023-04-19 01:55:38.000000 hak-0.0.8/hak/directories/exist.py
--rw-rw-r--   0 a         (1009) a         (1010)      432 2023-04-19 01:55:38.000000 hak-0.0.8/hak/directories/make.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.986774 hak-0.0.8/hak/directory/
--rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.8/hak/directory/__init__.py
--rw-rw-r--   0 a         (1009) a         (1010)     1548 2023-04-19 01:55:38.000000 hak-0.0.8/hak/directory/compress_to_tar.py
--rw-rw-r--   0 a         (1009) a         (1010)      674 2023-04-19 05:28:56.000000 hak-0.0.8/hak/directory/empty.py
--rw-rw-r--   0 a         (1009) a         (1010)       88 2023-04-19 01:55:38.000000 hak-0.0.8/hak/directory/exists.py
--rw-rw-r--   0 a         (1009) a         (1010)     1203 2023-04-19 10:13:05.000000 hak-0.0.8/hak/directory/get_most_recently_modified.py
--rw-rw-r--   0 a         (1009) a         (1010)      650 2023-04-19 01:55:38.000000 hak-0.0.8/hak/directory/is_module.py
--rw-rw-r--   0 a         (1009) a         (1010)      667 2023-04-19 10:09:51.000000 hak-0.0.8/hak/directory/make.py
--rw-rw-r--   0 a         (1009) a         (1010)      782 2023-04-19 01:55:38.000000 hak-0.0.8/hak/directory/remove.py
--rw-rw-r--   0 a         (1009) a         (1010)     3692 2023-04-19 01:55:38.000000 hak-0.0.8/hak/duration.py
--rw-rw-r--   0 a         (1009) a         (1010)     2021 2023-04-19 01:55:38.000000 hak-0.0.8/hak/duration_bar.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.986774 hak-0.0.8/hak/fake/
--rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.8/hak/fake/__init__.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.986774 hak-0.0.8/hak/fake/os/
--rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.8/hak/fake/os/__init__.py
--rw-rw-r--   0 a         (1009) a         (1010)      418 2023-04-19 01:55:38.000000 hak-0.0.8/hak/fake/os/system.py
--rw-rw-r--   0 a         (1009) a         (1010)      424 2023-04-19 01:55:38.000000 hak-0.0.8/hak/fake/printer.py
--rw-rw-r--   0 a         (1009) a         (1010)       45 2023-04-19 01:55:38.000000 hak-0.0.8/hak/fake/sleep.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.986774 hak-0.0.8/hak/fake/subprocess/
--rw-rw-r--   0 a         (1009) a         (1010)     5854 2023-04-19 04:41:24.000000 hak-0.0.8/hak/fake/subprocess/run.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.986774 hak-0.0.8/hak/file/
--rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 10:16:12.000000 hak-0.0.8/hak/file/__init__.py
--rw-rw-r--   0 a         (1009) a         (1010)      785 2023-04-19 01:55:38.000000 hak-0.0.8/hak/file/decrypt.py
--rw-rw-r--   0 a         (1009) a         (1010)      929 2023-04-19 01:55:38.000000 hak-0.0.8/hak/file/encrypt.py
--rw-rw-r--   0 a         (1009) a         (1010)      697 2023-04-19 01:55:38.000000 hak-0.0.8/hak/file/load.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.986774 hak-0.0.8/hak/file/pickle/
--rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.8/hak/file/pickle/__init__.py
--rw-rw-r--   0 a         (1009) a         (1010)     1253 2023-04-19 01:55:38.000000 hak-0.0.8/hak/file/pickle/load_if_exists.py
--rw-rw-r--   0 a         (1009) a         (1010)      906 2023-04-19 01:55:38.000000 hak-0.0.8/hak/file/pickle/save.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.986774 hak-0.0.8/hak/file/py/
--rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.8/hak/file/py/__init__.py
--rw-rw-r--   0 a         (1009) a         (1010)      546 2023-04-19 01:55:38.000000 hak-0.0.8/hak/file/py/create.py
--rw-rw-r--   0 a         (1009) a         (1010)     2644 2023-04-19 01:55:38.000000 hak-0.0.8/hak/file/py/dismantle.py
--rw-rw-r--   0 a         (1009) a         (1010)     3819 2023-04-19 01:55:38.000000 hak-0.0.8/hak/file/py/extract_fn.py
--rw-rw-r--   0 a         (1009) a         (1010)       84 2023-04-19 01:55:38.000000 hak-0.0.8/hak/file/py/is_a.py
--rw-rw-r--   0 a         (1009) a         (1010)      337 2023-04-19 01:55:38.000000 hak-0.0.8/hak/file/remove.py
--rw-rw-r--   0 a         (1009) a         (1010)      956 2023-04-19 01:55:38.000000 hak-0.0.8/hak/file/save.py
--rw-rw-r--   0 a         (1009) a         (1010)      761 2023-04-19 01:55:38.000000 hak-0.0.8/hak/file/save_lines.py
--rw-rw-r--   0 a         (1009) a         (1010)      308 2023-04-19 01:55:38.000000 hak-0.0.8/hak/file/save_lines_or_string.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.978773 hak-0.0.8/hak/file/secret/
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.986774 hak-0.0.8/hak/file/secret/password/
--rw-rw-r--   0 a         (1009) a         (1010)      680 2023-04-19 01:55:38.000000 hak-0.0.8/hak/file/secret/password/get.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.986774 hak-0.0.8/hak/file/secret/username/
--rw-rw-r--   0 a         (1009) a         (1010)      713 2023-04-19 01:55:38.000000 hak-0.0.8/hak/file/secret/username/get.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.986774 hak-0.0.8/hak/file/tar/
--rw-rw-r--   0 a         (1009) a         (1010)     1562 2023-04-19 01:55:38.000000 hak-0.0.8/hak/file/tar/extract.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.986774 hak-0.0.8/hak/file/zip/
--rw-rw-r--   0 a         (1009) a         (1010)      487 2023-04-19 01:55:38.000000 hak-0.0.8/hak/file/zip/extract.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.978773 hak-0.0.8/hak/files/
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.986774 hak-0.0.8/hak/files/pyfiles/
--rw-rw-r--   0 a         (1009) a         (1010)     1765 2023-04-19 04:43:12.000000 hak-0.0.8/hak/files/pyfiles/dismantle.py
--rw-rw-r--   0 a         (1009) a         (1010)      100 2023-04-19 01:55:38.000000 hak-0.0.8/hak/find_first_parenthesis.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.986774 hak-0.0.8/hak/float/
--rw-rw-r--   0 a         (1009) a         (1010)       70 2023-04-19 01:55:38.000000 hak-0.0.8/hak/float/epsilon.py
--rw-rw-r--   0 a         (1009) a         (1010)      106 2023-04-19 01:55:38.000000 hak-0.0.8/hak/float/is_a.py
--rw-rw-r--   0 a         (1009) a         (1010)      106 2023-04-19 01:55:38.000000 hak-0.0.8/hak/float/is_not.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.986774 hak-0.0.8/hak/float/nan/
--rw-rw-r--   0 a         (1009) a         (1010)      151 2023-04-19 01:55:38.000000 hak-0.0.8/hak/float/nan/to_none.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.986774 hak-0.0.8/hak/function/
--rw-rw-r--   0 a         (1009) a         (1010)      211 2023-04-19 01:55:38.000000 hak-0.0.8/hak/function/function.py
--rw-rw-r--   0 a         (1009) a         (1010)      423 2023-04-19 01:55:38.000000 hak-0.0.8/hak/function/write_to_file.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.986774 hak-0.0.8/hak/int/
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.986774 hak-0.0.8/hak/int/days/
--rw-rw-r--   0 a         (1009) a         (1010)      227 2023-04-19 01:55:38.000000 hak-0.0.8/hak/int/days/a_to_b_inclusive.py
--rw-rw-r--   0 a         (1009) a         (1010)      661 2023-04-19 01:55:38.000000 hak-0.0.8/hak/int/get_prime_factorisation.py
--rw-rw-r--   0 a         (1009) a         (1010)      104 2023-04-19 01:55:38.000000 hak-0.0.8/hak/int/is_a.py
--rw-rw-r--   0 a         (1009) a         (1010)      426 2023-04-19 01:55:38.000000 hak-0.0.8/hak/int/is_prime.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.986774 hak-0.0.8/hak/int/year/
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.986774 hak-0.0.8/hak/int/year/days/
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.986774 hak-0.0.8/hak/int/year/days/count/
--rw-rw-r--   0 a         (1009) a         (1010)      128 2023-04-19 01:55:38.000000 hak-0.0.8/hak/int/year/days/count/get.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.986774 hak-0.0.8/hak/int/year/days/first/
--rw-rw-r--   0 a         (1009) a         (1010)      154 2023-04-19 01:55:38.000000 hak-0.0.8/hak/int/year/days/first/get.py
--rw-rw-r--   0 a         (1009) a         (1010)      420 2023-04-19 01:55:38.000000 hak-0.0.8/hak/int/year/days/get.py
--rw-rw-r--   0 a         (1009) a         (1010)      153 2023-04-19 01:55:38.000000 hak-0.0.8/hak/int/year/now.py
--rw-rw-r--   0 a         (1009) a         (1010)      448 2023-04-19 01:55:38.000000 hak-0.0.8/hak/l.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.986774 hak-0.0.8/hak/list/
--rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.8/hak/list/__init__.py
--rw-rw-r--   0 a         (1009) a         (1010)      116 2023-04-19 01:55:38.000000 hak-0.0.8/hak/list/is_a.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.986774 hak-0.0.8/hak/list/strings/
--rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.8/hak/list/strings/__init__.py
--rw-rw-r--   0 a         (1009) a         (1010)      130 2023-04-19 04:41:08.000000 hak-0.0.8/hak/list/strings/add_src_funks_prefix.py
--rw-rw-r--   0 a         (1009) a         (1010)      586 2023-04-19 01:55:38.000000 hak-0.0.8/hak/list/strings/compare.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.986774 hak-0.0.8/hak/list/strings/contain/
--rw-rw-r--   0 a         (1009) a         (1010)      145 2023-04-19 04:43:23.000000 hak-0.0.8/hak/list/strings/contain/version.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.986774 hak-0.0.8/hak/list/strings/filepaths/
--rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.8/hak/list/strings/filepaths/__init__.py
--rw-rw-r--   0 a         (1009) a         (1010)     1228 2023-04-19 04:38:09.000000 hak-0.0.8/hak/list/strings/filepaths/get.py
--rw-rw-r--   0 a         (1009) a         (1010)     2222 2023-04-19 04:44:27.000000 hak-0.0.8/hak/list/strings/find_first_diff.py
--rw-rw-r--   0 a         (1009) a         (1010)      434 2023-04-19 04:45:12.000000 hak-0.0.8/hak/list/strings/make_patch_version_change_to_py.py
--rw-rw-r--   0 a         (1009) a         (1010)      293 2023-04-19 04:47:46.000000 hak-0.0.8/hak/list/strings/module_names_from_py_filenames.py
--rw-rw-r--   0 a         (1009) a         (1010)      410 2023-04-19 04:48:58.000000 hak-0.0.8/hak/list/strings/patch_setup_cfg.py
--rw-rw-r--   0 a         (1009) a         (1010)      622 2023-04-19 04:51:45.000000 hak-0.0.8/hak/list/strings/patch_setup_py.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.986774 hak-0.0.8/hak/list/strings/pyfiles/
--rw-rw-r--   0 a         (1009) a         (1010)     1514 2023-04-19 04:52:08.000000 hak-0.0.8/hak/list/strings/pyfiles/filter_out_items.py
--rw-rw-r--   0 a         (1009) a         (1010)      766 2023-04-19 05:00:37.000000 hak-0.0.8/hak/list/strings/show_diff.py
--rw-rw-r--   0 a         (1009) a         (1010)      647 2023-04-19 05:00:56.000000 hak-0.0.8/hak/list/strings/to_dict.py
--rw-rw-r--   0 a         (1009) a         (1010)      357 2023-04-19 05:01:35.000000 hak-0.0.8/hak/list/strings/two_char_combinations.py
--rw-rw-r--   0 a         (1009) a         (1010)      115 2023-04-19 01:55:38.000000 hak-0.0.8/hak/list/to_comma_separated_str.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.986774 hak-0.0.8/hak/lists/
--rw-rw-r--   0 a         (1009) a         (1010)      216 2023-04-19 01:55:38.000000 hak-0.0.8/hak/lists/merge.py
--rw-rw-r--   0 a         (1009) a         (1010)     1131 2023-04-19 01:55:38.000000 hak-0.0.8/hak/load_durations_if_exists.py
--rw-rw-r--   0 a         (1009) a         (1010)      123 2023-04-19 01:55:38.000000 hak-0.0.8/hak/log_2.py
--rw-rw-r--   0 a         (1009) a         (1010)       84 2023-04-19 01:55:38.000000 hak-0.0.8/hak/nop.py
--rw-rw-r--   0 a         (1009) a         (1010)       91 2023-04-19 01:55:38.000000 hak-0.0.8/hak/nop_state_x.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.986774 hak-0.0.8/hak/patch/
--rw-rw-r--   0 a         (1009) a         (1010)     7860 2023-04-19 09:15:38.000000 hak-0.0.8/hak/patch/do.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.986774 hak-0.0.8/hak/period/
--rw-rw-r--   0 a         (1009) a         (1010)      333 2023-04-19 01:55:38.000000 hak-0.0.8/hak/period/contains_day.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.986774 hak-0.0.8/hak/pip/
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.986774 hak-0.0.8/hak/pip/dist_tar/
--rw-rw-r--   0 a         (1009) a         (1010)     3119 2023-04-19 07:21:09.000000 hak-0.0.8/hak/pip/dist_tar/make.py
--rw-rw-r--   0 a         (1009) a         (1010)      804 2023-04-19 07:34:45.000000 hak-0.0.8/hak/pip/dist_tar/remove.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.986774 hak-0.0.8/hak/pip/setup/
--rw-rw-r--   0 a         (1009) a         (1010)     1305 2023-04-19 04:43:59.000000 hak-0.0.8/hak/pip/setup/update.py
--rw-rw-r--   0 a         (1009) a         (1010)     1792 2023-04-19 08:32:41.000000 hak-0.0.8/hak/pip/upload.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.986774 hak-0.0.8/hak/pip/version/
--rw-rw-r--   0 a         (1009) a         (1010)      837 2023-04-19 01:55:38.000000 hak-0.0.8/hak/pip/version/get.py
--rw-rw-r--   0 a         (1009) a         (1010)      120 2023-04-19 01:55:38.000000 hak-0.0.8/hak/pip/version/to_str.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.986774 hak-0.0.8/hak/pyfiles/
--rw-rw-r--   0 a         (1009) a         (1010)      157 2023-04-19 01:55:38.000000 hak-0.0.8/hak/pyfiles/format.py
--rw-rw-r--   0 a         (1009) a         (1010)      838 2023-04-19 04:33:37.000000 hak-0.0.8/hak/pyfiles/format_and_commit.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.986774 hak-0.0.8/hak/report/
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.986774 hak-0.0.8/hak/report/fail/
--rw-rw-r--   0 a         (1009) a         (1010)      814 2023-04-19 01:55:38.000000 hak-0.0.8/hak/report/fail/no_xyz.py
--rw-rw-r--   0 a         (1009) a         (1010)     1914 2023-04-19 01:55:38.000000 hak-0.0.8/hak/report/fail/xyz.py
--rw-rw-r--   0 a         (1009) a         (1010)     1440 2023-04-19 01:55:38.000000 hak-0.0.8/hak/report/fail/z_return_neq_y_return.py
--rw-rw-r--   0 a         (1009) a         (1010)     1601 2023-04-19 01:55:38.000000 hak-0.0.8/hak/report/fail/z_stdo_neq_y_stdo.py
--rw-rw-r--   0 a         (1009) a         (1010)      887 2023-04-19 01:55:38.000000 hak-0.0.8/hak/report/property_failure.py
--rw-rw-r--   0 a         (1009) a         (1010)      729 2023-04-19 01:55:38.000000 hak-0.0.8/hak/report/success.py
--rw-rw-r--   0 a         (1009) a         (1010)      394 2023-04-19 01:55:38.000000 hak-0.0.8/hak/report/summarise_file.py
--rw-rw-r--   0 a         (1009) a         (1010)      758 2023-04-19 01:55:38.000000 hak-0.0.8/hak/save_durations.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.986774 hak-0.0.8/hak/schedule/
--rw-rw-r--   0 a         (1009) a         (1010)     3465 2023-04-19 01:55:38.000000 hak-0.0.8/hak/schedule/make.py
--rw-rw-r--   0 a         (1009) a         (1010)      559 2023-04-19 01:55:38.000000 hak-0.0.8/hak/select_text_colour_from_width.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.986774 hak-0.0.8/hak/session/
--rw-rw-r--   0 a         (1009) a         (1010)      146 2023-04-19 01:55:38.000000 hak-0.0.8/hak/session/is_a.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.986774 hak-0.0.8/hak/set/
--rw-rw-r--   0 a         (1009) a         (1010)      114 2023-04-19 01:55:38.000000 hak-0.0.8/hak/set/is_a.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.982773 hak-0.0.8/hak/setup/
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.986774 hak-0.0.8/hak/setup/cfg/
--rw-rw-r--   0 a         (1009) a         (1010)     1531 2023-04-19 07:22:45.000000 hak-0.0.8/hak/setup/cfg/update.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.986774 hak-0.0.8/hak/setup/py/
--rw-rw-r--   0 a         (1009) a         (1010)     1633 2023-04-19 07:24:59.000000 hak-0.0.8/hak/setup/py/update.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.990774 hak-0.0.8/hak/string/
--rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/__init__.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.990774 hak-0.0.8/hak/string/alphanumeric/
--rw-rw-r--   0 a         (1009) a         (1010)      264 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/alphanumeric/fake.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.990774 hak-0.0.8/hak/string/append/
--rw-rw-r--   0 a         (1009) a         (1010)       54 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/append/new_line.py
--rw-rw-r--   0 a         (1009) a         (1010)      541 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/camel_to_snake.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.990774 hak-0.0.8/hak/string/char/
--rw-rw-r--   0 a         (1009) a         (1010)      322 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/char/find_all_indices.py
--rw-rw-r--   0 a         (1009) a         (1010)      128 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/char/is_digit.py
--rw-rw-r--   0 a         (1009) a         (1010)      207 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/char/is_upper.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.990774 hak-0.0.8/hak/string/chars/
--rw-rw-r--   0 a         (1009) a         (1010)      561 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/chars/remove.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.990774 hak-0.0.8/hak/string/colour/
--rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/colour/__init__.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.990774 hak-0.0.8/hak/string/colour/bright/
--rw-rw-r--   0 a         (1009) a         (1010)      162 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/colour/bright/blue.py
--rw-rw-r--   0 a         (1009) a         (1010)      162 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/colour/bright/cyan.py
--rw-rw-r--   0 a         (1009) a         (1010)      164 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/colour/bright/green.py
--rw-rw-r--   0 a         (1009) a         (1010)      168 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/colour/bright/magenta.py
--rw-rw-r--   0 a         (1009) a         (1010)      160 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/colour/bright/red.py
--rw-rw-r--   0 a         (1009) a         (1010)      164 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/colour/bright/white.py
--rw-rw-r--   0 a         (1009) a         (1010)      166 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/colour/bright/yellow.py
--rw-rw-r--   0 a         (1009) a         (1010)      130 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/colour/danger.py
--rw-rw-r--   0 a         (1009) a         (1010)      174 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/colour/danger_if_zero.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.990774 hak-0.0.8/hak/string/colour/dark/
--rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/colour/dark/__init__.py
--rw-rw-r--   0 a         (1009) a         (1010)      148 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/colour/dark/blue.py
--rw-rw-r--   0 a         (1009) a         (1010)      148 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/colour/dark/cyan.py
--rw-rw-r--   0 a         (1009) a         (1010)      154 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/colour/dark/default.py
--rw-rw-r--   0 a         (1009) a         (1010)      150 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/colour/dark/green.py
--rw-rw-r--   0 a         (1009) a         (1010)      154 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/colour/dark/magenta.py
--rw-rw-r--   0 a         (1009) a         (1010)      146 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/colour/dark/red.py
--rw-rw-r--   0 a         (1009) a         (1010)      150 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/colour/dark/white.py
--rw-rw-r--   0 a         (1009) a         (1010)      152 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/colour/dark/yellow.py
--rw-rw-r--   0 a         (1009) a         (1010)       64 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/colour/data.py
--rw-rw-r--   0 a         (1009) a         (1010)      131 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/colour/info.py
--rw-rw-r--   0 a         (1009) a         (1010)      131 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/colour/primary.py
--rw-rw-r--   0 a         (1009) a         (1010)     2261 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/colour/rainbow.py
--rw-rw-r--   0 a         (1009) a         (1010)      134 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/colour/secondary.py
--rw-rw-r--   0 a         (1009) a         (1010)      267 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/colour/tgfr.py
--rw-rw-r--   0 a         (1009) a         (1010)      135 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/colour/warning.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.990774 hak-0.0.8/hak/string/contains/
--rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/contains/__init__.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.990774 hak-0.0.8/hak/string/contains/function/
--rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/contains/function/__init__.py
--rw-rw-r--   0 a         (1009) a         (1010)      341 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/contains/function/run.py
--rw-rw-r--   0 a         (1009) a         (1010)      192 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/contains/function/test.py
--rw-rw-r--   0 a         (1009) a         (1010)      224 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/contains/l.py
--rw-rw-r--   0 a         (1009) a         (1010)       76 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/contains/version.py
--rw-rw-r--   0 a         (1009) a         (1010)      105 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/count_x_in_y.py
--rw-rw-r--   0 a         (1009) a         (1010)      996 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/delete_character_safely.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.990774 hak-0.0.8/hak/string/digits/
--rw-rw-r--   0 a         (1009) a         (1010)      202 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/digits/remove.py
--rw-rw-r--   0 a         (1009) a         (1010)      111 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/double_single_quotes.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.990774 hak-0.0.8/hak/string/family_name/
--rw-rw-r--   0 a         (1009) a         (1010)   115522 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/family_name/fake.py
--rw-rw-r--   0 a         (1009) a         (1010)      303 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/family_name/is_a.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.990774 hak-0.0.8/hak/string/filename/
--rw-rw-r--   0 a         (1009) a         (1010)      126 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/filename/to_module_name.py
--rw-rw-r--   0 a         (1009) a         (1010)      209 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/find_last_comma_index.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.990774 hak-0.0.8/hak/string/fn_name/
--rw-rw-r--   0 a         (1009) a         (1010)      226 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/fn_name/is_ignorable.py
--rw-rw-r--   0 a         (1009) a         (1010)     5035 2023-04-19 05:00:49.000000 hak-0.0.8/hak/string/format.py
--rw-rw-r--   0 a         (1009) a         (1010)       73 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/has_at_symbol.py
--rw-rw-r--   0 a         (1009) a         (1010)      132 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/has_digit.py
--rw-rw-r--   0 a         (1009) a         (1010)      131 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/has_lowercase.py
--rw-rw-r--   0 a         (1009) a         (1010)      259 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/has_other_char.py
--rw-rw-r--   0 a         (1009) a         (1010)      172 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/has_seven_digits.py
--rw-rw-r--   0 a         (1009) a         (1010)      132 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/has_uppercase.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.990774 hak-0.0.8/hak/string/hbar/
--rw-rw-r--   0 a         (1009) a         (1010)      122 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/hbar/make.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.982773 hak-0.0.8/hak/string/header/
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.990774 hak-0.0.8/hak/string/header/python_file/
--rw-rw-r--   0 a         (1009) a         (1010)      314 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/header/python_file/make.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.990774 hak-0.0.8/hak/string/header/test_table/
--rw-rw-r--   0 a         (1009) a         (1010)      461 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/header/test_table/make.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.990774 hak-0.0.8/hak/string/indent/
--rw-rw-r--   0 a         (1009) a         (1010)      137 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/indent/run_if_class_method.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.990774 hak-0.0.8/hak/string/insert/
--rw-rw-r--   0 a         (1009) a         (1010)      602 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/insert/new_line_after_last_import_line.py
--rw-rw-r--   0 a         (1009) a         (1010)      278 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/insert/new_line_before_comment.py
--rw-rw-r--   0 a         (1009) a         (1010)      584 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/insert/new_line_before_def.py
--rw-rw-r--   0 a         (1009) a         (1010)      251 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/insert/new_line_before_if_main.py
--rw-rw-r--   0 a         (1009) a         (1010)      666 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/insert/new_line_before_lambda.py
--rw-rw-r--   0 a         (1009) a         (1010)      292 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/insert/new_line_before_new_line_and_cea_.py
--rw-rw-r--   0 a         (1009) a         (1010)      102 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/is_a.py
--rw-rw-r--   0 a         (1009) a         (1010)      124 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/is_or_none.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.990774 hak-0.0.8/hak/string/json/
--rw-rw-r--   0 a         (1009) a         (1010)      179 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/json/is_a.py
--rw-rw-r--   0 a         (1009) a         (1010)      548 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/lambdarise.py
--rw-rw-r--   0 a         (1009) a         (1010)      360 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/make_content_without_function.py
--rw-rw-r--   0 a         (1009) a         (1010)      325 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/make_function_text.py
--rw-rw-r--   0 a         (1009) a         (1010)      338 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/make_initial_content.py
--rw-rw-r--   0 a         (1009) a         (1010)      319 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/make_new_function_text.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.990774 hak-0.0.8/hak/string/password/
--rw-rw-r--   0 a         (1009) a         (1010)     1179 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/password/create.py
--rw-rw-r--   0 a         (1009) a         (1010)      534 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/password/has_chars_from_3_sets.py
--rw-rw-r--   0 a         (1009) a         (1010)      207 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/pop_left.py
--rw-rw-r--   0 a         (1009) a         (1010)      219 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/pop_right.py
--rw-rw-r--   0 a         (1009) a         (1010)      151 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/prepend_import.py
--rw-rw-r--   0 a         (1009) a         (1010)      756 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/print_and_return_false.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.990774 hak-0.0.8/hak/string/refactor/
--rw-rw-r--   0 a         (1009) a         (1010)     1218 2023-04-19 05:01:09.000000 hak-0.0.8/hak/string/refactor/by_two_char_combinations.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.990774 hak-0.0.8/hak/string/remove/
--rw-rw-r--   0 a         (1009) a         (1010)      211 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/remove/empty_line_spaces.py
--rw-rw-r--   0 a         (1009) a         (1010)      162 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/remove/empty_lines.py
--rw-rw-r--   0 a         (1009) a         (1010)      441 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/remove/extra_new_line_following_class_definition.py
--rw-rw-r--   0 a         (1009) a         (1010)      210 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/remove/first_new_line_if_starts_with_new_line.py
--rw-rw-r--   0 a         (1009) a         (1010)       81 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/remove/whitespace_between_newlines.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.990774 hak-0.0.8/hak/string/replace/
--rw-rw-r--   0 a         (1009) a         (1010)      241 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/replace/double_new_line_with_single_new_line.py
--rw-rw-r--   0 a         (1009) a         (1010)      129 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/replace/single_new_line_with_empty_string.py
--rw-rw-r--   0 a         (1009) a         (1010)      251 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/replace/triple_new_line_with_double_new_line.py
--rw-rw-r--   0 a         (1009) a         (1010)      483 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/replace_unprintable.py
--rw-rw-r--   0 a         (1009) a         (1010)     3361 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/separate_function_from_context.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.990774 hak-0.0.8/hak/string/single_line_function/
--rw-rw-r--   0 a         (1009) a         (1010)      428 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/single_line_function/is_a.py
--rw-rw-r--   0 a         (1009) a         (1010)      463 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/single_line_function/to_lambda_str.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.990774 hak-0.0.8/hak/string/spaces/
--rw-rw-r--   0 a         (1009) a         (1010)      111 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/spaces/count.py
--rw-rw-r--   0 a         (1009) a         (1010)      320 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/split_fn_name_and_text.py
--rw-rw-r--   0 a         (1009) a         (1010)      344 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/strip_unprintable.py
--rw-rw-r--   0 a         (1009) a         (1010)      265 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/to_cond_freq_dict.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.990774 hak-0.0.8/hak/string/token/
--rw-rw-r--   0 a         (1009) a         (1010)     1263 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/token/substitute.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.990774 hak-0.0.8/hak/string/yyyymmdd/
--rw-rw-r--   0 a         (1009) a         (1010)      238 2023-04-19 01:55:38.000000 hak-0.0.8/hak/string/yyyymmdd/to_date.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.982773 hak-0.0.8/hak/subprocess/
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.990774 hak-0.0.8/hak/subprocess/completed_process/
--rw-rw-r--   0 a         (1009) a         (1010)      655 2023-04-19 01:55:38.000000 hak-0.0.8/hak/subprocess/completed_process/to_str.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.990774 hak-0.0.8/hak/system/
--rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.8/hak/system/__init__.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.990774 hak-0.0.8/hak/system/git/
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.990774 hak-0.0.8/hak/system/git/commit/
--rw-rw-r--   0 a         (1009) a         (1010)     2515 2023-04-19 01:55:38.000000 hak-0.0.8/hak/system/git/commit/run.py
--rw-rw-r--   0 a         (1009) a         (1010)      384 2023-04-19 01:55:38.000000 hak-0.0.8/hak/system/git/commit_if_test_and_app_ok.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.990774 hak-0.0.8/hak/system/git/gitignore/
--rw-rw-r--   0 a         (1009) a         (1010)      631 2023-04-19 01:55:38.000000 hak-0.0.8/hak/system/git/gitignore/make.py
--rw-rw-r--   0 a         (1009) a         (1010)      486 2023-04-19 03:03:56.000000 hak-0.0.8/hak/system/git/init.py
--rw-rw-r--   0 a         (1009) a         (1010)      725 2023-04-19 01:55:38.000000 hak-0.0.8/hak/system/git/log_oneline.py
--rw-rw-r--   0 a         (1009) a         (1010)      866 2023-04-19 01:55:38.000000 hak-0.0.8/hak/system/git/push_after_delay.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.990774 hak-0.0.8/hak/system/screen/
--rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.8/hak/system/screen/__init__.py
--rw-rw-r--   0 a         (1009) a         (1010)      786 2023-04-19 01:55:38.000000 hak-0.0.8/hak/system/screen/clear.py
--rw-rw-r--   0 a         (1009) a         (1010)     3119 2023-04-19 01:55:38.000000 hak-0.0.8/hak/terminal.py
--rw-rw-r--   0 a         (1009) a         (1010)      337 2023-04-19 01:55:38.000000 hak-0.0.8/hak/ternary.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.990774 hak-0.0.8/hak/test/
--rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.8/hak/test/__init__.py
--rw-rw-r--   0 a         (1009) a         (1010)     2578 2023-04-19 01:55:38.000000 hak-0.0.8/hak/test/check_final_line.py
--rw-rw-r--   0 a         (1009) a         (1010)     2689 2023-04-19 01:55:38.000000 hak-0.0.8/hak/test/check_line_lengths.py
--rw-rw-r--   0 a         (1009) a         (1010)     2843 2023-04-19 01:55:38.000000 hak-0.0.8/hak/test/do.py
--rw-rw-r--   0 a         (1009) a         (1010)     2450 2023-04-19 01:55:38.000000 hak-0.0.8/hak/test/final_line_check.py
--rw-rw-r--   0 a         (1009) a         (1010)      774 2023-04-19 01:55:38.000000 hak-0.0.8/hak/test/line_lengths_check.py
--rw-rw-r--   0 a         (1009) a         (1010)      926 2023-04-19 01:55:38.000000 hak-0.0.8/hak/test/oldest_file_print.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.990774 hak-0.0.8/hak/tup/
--rw-rw-r--   0 a         (1009) a         (1010)      176 2023-04-19 01:55:38.000000 hak-0.0.8/hak/tup/is_a.py
--rw-rw-r--   0 a         (1009) a         (1010)      617 2023-04-19 01:55:38.000000 hak-0.0.8/hak/update_duration.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:19:54.982773 hak-0.0.8/hak.egg-info/
--rw-rw-r--   0 a         (1009) a         (1010)      994 2023-04-19 10:19:54.000000 hak-0.0.8/hak.egg-info/PKG-INFO
--rw-rw-r--   0 a         (1009) a         (1010)     7947 2023-04-19 10:19:54.000000 hak-0.0.8/hak.egg-info/SOURCES.txt
--rw-rw-r--   0 a         (1009) a         (1010)        1 2023-04-19 10:19:54.000000 hak-0.0.8/hak.egg-info/dependency_links.txt
--rw-rw-r--   0 a         (1009) a         (1010)     1633 2023-04-19 10:19:54.000000 hak-0.0.8/hak.egg-info/top_level.txt
--rw-rw-r--   0 a         (1009) a         (1010)      536 2023-04-19 10:19:54.994774 hak-0.0.8/setup.cfg
--rw-rw-r--   0 a         (1009) a         (1010)     2781 2023-04-19 10:19:54.000000 hak-0.0.8/setup.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.718405 hak-0.0.9/
+-rw-rw-r--   0 a         (1009) a         (1010)     1068 2023-04-19 01:55:38.000000 hak-0.0.9/LICENSE
+-rw-rw-r--   0 a         (1009) a         (1010)      994 2023-04-19 10:43:20.718405 hak-0.0.9/PKG-INFO
+-rw-rw-r--   0 a         (1009) a         (1010)      406 2023-04-19 03:24:53.000000 hak-0.0.9/README.md
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.706405 hak-0.0.9/hak/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.9/hak/__init__.py
+-rw-rw-r--   0 a         (1009) a         (1010)      140 2023-04-19 01:55:38.000000 hak-0.0.9/hak/a_equals_b.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.706405 hak-0.0.9/hak/bool/
+-rw-rw-r--   0 a         (1009) a         (1010)       86 2023-04-19 01:55:38.000000 hak-0.0.9/hak/bool/fake.py
+-rw-rw-r--   0 a         (1009) a         (1010)      103 2023-04-19 01:55:38.000000 hak-0.0.9/hak/bool/is_a.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.706405 hak-0.0.9/hak/bool/or_none/
+-rw-rw-r--   0 a         (1009) a         (1010)      160 2023-04-19 01:55:38.000000 hak-0.0.9/hak/bool/or_none/fake.py
+-rw-rw-r--   0 a         (1009) a         (1010)      125 2023-04-19 01:55:38.000000 hak-0.0.9/hak/bool/or_none/is_a.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.706405 hak-0.0.9/hak/bools/
+-rw-rw-r--   0 a         (1009) a         (1010)      139 2023-04-19 01:55:38.000000 hak-0.0.9/hak/bools/count_true.py
+-rw-rw-r--   0 a         (1009) a         (1010)      249 2023-04-19 01:55:38.000000 hak-0.0.9/hak/calculate_duration_bar_width.py
+-rw-rw-r--   0 a         (1009) a         (1010)      758 2023-04-19 01:55:38.000000 hak-0.0.9/hak/check_if_ok_to_proceed.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.706405 hak-0.0.9/hak/date/
+-rw-rw-r--   0 a         (1009) a         (1010)      143 2023-04-19 01:55:38.000000 hak-0.0.9/hak/date/is_a.py
+-rw-rw-r--   0 a         (1009) a         (1010)      347 2023-04-19 01:55:38.000000 hak-0.0.9/hak/date/is_first_second_or_third_day_of_month.py
+-rw-rw-r--   0 a         (1009) a         (1010)      414 2023-04-19 01:55:38.000000 hak-0.0.9/hak/date/is_first_week_of_quarter.py
+-rw-rw-r--   0 a         (1009) a         (1010)      208 2023-04-19 01:55:38.000000 hak-0.0.9/hak/date/is_monday.py
+-rw-rw-r--   0 a         (1009) a         (1010)      462 2023-04-19 01:55:38.000000 hak-0.0.9/hak/date/is_weekday.py
+-rw-rw-r--   0 a         (1009) a         (1010)      467 2023-04-19 01:55:38.000000 hak-0.0.9/hak/date/is_weekend.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/date/public_holiday/
+-rw-rw-r--   0 a         (1009) a         (1010)     5617 2023-04-19 01:55:38.000000 hak-0.0.9/hak/date/public_holiday/is_a.py
+-rw-rw-r--   0 a         (1009) a         (1010)      385 2023-04-19 01:55:38.000000 hak-0.0.9/hak/date/select_from_last_n_days.py
+-rw-rw-r--   0 a         (1009) a         (1010)      146 2023-04-19 01:55:38.000000 hak-0.0.9/hak/date/to_dd_mm_yyyy_str.py
+-rw-rw-r--   0 a         (1009) a         (1010)      605 2023-04-19 03:01:25.000000 hak-0.0.9/hak/date/to_utc_timestamp.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.706405 hak-0.0.9/hak/date/year/
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/date/year/easter_sunday/
+-rw-rw-r--   0 a         (1009) a         (1010)     1006 2023-04-19 01:55:38.000000 hak-0.0.9/hak/date/year/easter_sunday/get.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/datetime/
+-rw-rw-r--   0 a         (1009) a         (1010)      149 2023-04-19 01:55:38.000000 hak-0.0.9/hak/datetime/is_a.py
+-rw-rw-r--   0 a         (1009) a         (1010)      272 2023-04-19 01:55:38.000000 hak-0.0.9/hak/datetime/select_from_last_n_days.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/dict/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.9/hak/dict/__init__.py
+-rw-rw-r--   0 a         (1009) a         (1010)      215 2023-04-19 01:55:38.000000 hak-0.0.9/hak/dict/convert_to_sql_insertable.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/dict/frequencies/
+-rw-rw-r--   0 a         (1009) a         (1010)      356 2023-04-19 01:55:38.000000 hak-0.0.9/hak/dict/frequencies/choose.py
+-rw-rw-r--   0 a         (1009) a         (1010)      376 2023-04-19 01:55:38.000000 hak-0.0.9/hak/dict/frequencies/make_from_strings.py
+-rw-rw-r--   0 a         (1009) a         (1010)      187 2023-04-19 01:55:38.000000 hak-0.0.9/hak/dict/get_or_default.py
+-rw-rw-r--   0 a         (1009) a         (1010)      190 2023-04-19 01:55:38.000000 hak-0.0.9/hak/dict/is_a.py
+-rw-rw-r--   0 a         (1009) a         (1010)      116 2023-04-19 01:55:38.000000 hak-0.0.9/hak/dict/make_from_key_value_lists.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/dict/proposed_dismantlement/
+-rw-rw-r--   0 a         (1009) a         (1010)     1520 2023-04-19 01:55:38.000000 hak-0.0.9/hak/dict/proposed_dismantlement/show.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/dict/test_durations/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.9/hak/dict/test_durations/__init__.py
+-rw-rw-r--   0 a         (1009) a         (1010)      134 2023-04-19 01:55:38.000000 hak-0.0.9/hak/dict/test_durations/to_tuple_list_sorted_by_duration.py
+-rw-rw-r--   0 a         (1009) a         (1010)     4011 2023-04-19 01:55:38.000000 hak-0.0.9/hak/dict/to_max_line_width_str.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/dicts/
+-rw-rw-r--   0 a         (1009) a         (1010)      151 2023-04-19 01:55:38.000000 hak-0.0.9/hak/dicts/a_into_b.py
+-rw-rw-r--   0 a         (1009) a         (1010)     1200 2023-04-19 01:55:38.000000 hak-0.0.9/hak/dicts/compare.py
+-rw-rw-r--   0 a         (1009) a         (1010)      195 2023-04-19 01:55:38.000000 hak-0.0.9/hak/dicts/is_a.py
+-rw-rw-r--   0 a         (1009) a         (1010)      663 2023-04-19 01:55:38.000000 hak-0.0.9/hak/dicts/merge_freq_dicts.py
+-rw-rw-r--   0 a         (1009) a         (1010)      251 2023-04-19 01:55:38.000000 hak-0.0.9/hak/dicts/reindex.py
+-rw-rw-r--   0 a         (1009) a         (1010)      203 2023-04-19 01:55:38.000000 hak-0.0.9/hak/dicts/sort_by_key.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/directories/
+-rw-rw-r--   0 a         (1009) a         (1010)      567 2023-04-19 01:55:38.000000 hak-0.0.9/hak/directories/exist.py
+-rw-rw-r--   0 a         (1009) a         (1010)      432 2023-04-19 01:55:38.000000 hak-0.0.9/hak/directories/make.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/directory/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.9/hak/directory/__init__.py
+-rw-rw-r--   0 a         (1009) a         (1010)     1548 2023-04-19 01:55:38.000000 hak-0.0.9/hak/directory/compress_to_tar.py
+-rw-rw-r--   0 a         (1009) a         (1010)      674 2023-04-19 05:28:56.000000 hak-0.0.9/hak/directory/empty.py
+-rw-rw-r--   0 a         (1009) a         (1010)       88 2023-04-19 01:55:38.000000 hak-0.0.9/hak/directory/exists.py
+-rw-rw-r--   0 a         (1009) a         (1010)     1239 2023-04-19 10:43:13.000000 hak-0.0.9/hak/directory/get_most_recently_modified.py
+-rw-rw-r--   0 a         (1009) a         (1010)      650 2023-04-19 01:55:38.000000 hak-0.0.9/hak/directory/is_module.py
+-rw-rw-r--   0 a         (1009) a         (1010)      667 2023-04-19 10:09:51.000000 hak-0.0.9/hak/directory/make.py
+-rw-rw-r--   0 a         (1009) a         (1010)      782 2023-04-19 01:55:38.000000 hak-0.0.9/hak/directory/remove.py
+-rw-rw-r--   0 a         (1009) a         (1010)     3692 2023-04-19 01:55:38.000000 hak-0.0.9/hak/duration.py
+-rw-rw-r--   0 a         (1009) a         (1010)     2021 2023-04-19 01:55:38.000000 hak-0.0.9/hak/duration_bar.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/fake/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.9/hak/fake/__init__.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/fake/os/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.9/hak/fake/os/__init__.py
+-rw-rw-r--   0 a         (1009) a         (1010)      418 2023-04-19 01:55:38.000000 hak-0.0.9/hak/fake/os/system.py
+-rw-rw-r--   0 a         (1009) a         (1010)      424 2023-04-19 01:55:38.000000 hak-0.0.9/hak/fake/printer.py
+-rw-rw-r--   0 a         (1009) a         (1010)       45 2023-04-19 01:55:38.000000 hak-0.0.9/hak/fake/sleep.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/fake/subprocess/
+-rw-rw-r--   0 a         (1009) a         (1010)     5854 2023-04-19 04:41:24.000000 hak-0.0.9/hak/fake/subprocess/run.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/file/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 10:16:12.000000 hak-0.0.9/hak/file/__init__.py
+-rw-rw-r--   0 a         (1009) a         (1010)      785 2023-04-19 01:55:38.000000 hak-0.0.9/hak/file/decrypt.py
+-rw-rw-r--   0 a         (1009) a         (1010)      929 2023-04-19 01:55:38.000000 hak-0.0.9/hak/file/encrypt.py
+-rw-rw-r--   0 a         (1009) a         (1010)      697 2023-04-19 01:55:38.000000 hak-0.0.9/hak/file/load.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/file/pickle/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.9/hak/file/pickle/__init__.py
+-rw-rw-r--   0 a         (1009) a         (1010)     1253 2023-04-19 01:55:38.000000 hak-0.0.9/hak/file/pickle/load_if_exists.py
+-rw-rw-r--   0 a         (1009) a         (1010)      906 2023-04-19 01:55:38.000000 hak-0.0.9/hak/file/pickle/save.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/file/py/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.9/hak/file/py/__init__.py
+-rw-rw-r--   0 a         (1009) a         (1010)      546 2023-04-19 01:55:38.000000 hak-0.0.9/hak/file/py/create.py
+-rw-rw-r--   0 a         (1009) a         (1010)     2644 2023-04-19 01:55:38.000000 hak-0.0.9/hak/file/py/dismantle.py
+-rw-rw-r--   0 a         (1009) a         (1010)     3819 2023-04-19 01:55:38.000000 hak-0.0.9/hak/file/py/extract_fn.py
+-rw-rw-r--   0 a         (1009) a         (1010)       84 2023-04-19 01:55:38.000000 hak-0.0.9/hak/file/py/is_a.py
+-rw-rw-r--   0 a         (1009) a         (1010)      337 2023-04-19 01:55:38.000000 hak-0.0.9/hak/file/remove.py
+-rw-rw-r--   0 a         (1009) a         (1010)      956 2023-04-19 01:55:38.000000 hak-0.0.9/hak/file/save.py
+-rw-rw-r--   0 a         (1009) a         (1010)      761 2023-04-19 01:55:38.000000 hak-0.0.9/hak/file/save_lines.py
+-rw-rw-r--   0 a         (1009) a         (1010)      308 2023-04-19 01:55:38.000000 hak-0.0.9/hak/file/save_lines_or_string.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.706405 hak-0.0.9/hak/file/secret/
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/file/secret/password/
+-rw-rw-r--   0 a         (1009) a         (1010)      680 2023-04-19 01:55:38.000000 hak-0.0.9/hak/file/secret/password/get.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/file/secret/username/
+-rw-rw-r--   0 a         (1009) a         (1010)      713 2023-04-19 01:55:38.000000 hak-0.0.9/hak/file/secret/username/get.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/file/tar/
+-rw-rw-r--   0 a         (1009) a         (1010)     1562 2023-04-19 01:55:38.000000 hak-0.0.9/hak/file/tar/extract.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/file/zip/
+-rw-rw-r--   0 a         (1009) a         (1010)      487 2023-04-19 01:55:38.000000 hak-0.0.9/hak/file/zip/extract.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.706405 hak-0.0.9/hak/files/
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/files/pyfiles/
+-rw-rw-r--   0 a         (1009) a         (1010)     1765 2023-04-19 04:43:12.000000 hak-0.0.9/hak/files/pyfiles/dismantle.py
+-rw-rw-r--   0 a         (1009) a         (1010)      100 2023-04-19 01:55:38.000000 hak-0.0.9/hak/find_first_parenthesis.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/float/
+-rw-rw-r--   0 a         (1009) a         (1010)       70 2023-04-19 01:55:38.000000 hak-0.0.9/hak/float/epsilon.py
+-rw-rw-r--   0 a         (1009) a         (1010)      106 2023-04-19 01:55:38.000000 hak-0.0.9/hak/float/is_a.py
+-rw-rw-r--   0 a         (1009) a         (1010)      106 2023-04-19 01:55:38.000000 hak-0.0.9/hak/float/is_not.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/float/nan/
+-rw-rw-r--   0 a         (1009) a         (1010)      151 2023-04-19 01:55:38.000000 hak-0.0.9/hak/float/nan/to_none.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/function/
+-rw-rw-r--   0 a         (1009) a         (1010)      211 2023-04-19 01:55:38.000000 hak-0.0.9/hak/function/function.py
+-rw-rw-r--   0 a         (1009) a         (1010)      423 2023-04-19 01:55:38.000000 hak-0.0.9/hak/function/write_to_file.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/int/
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/int/days/
+-rw-rw-r--   0 a         (1009) a         (1010)      227 2023-04-19 01:55:38.000000 hak-0.0.9/hak/int/days/a_to_b_inclusive.py
+-rw-rw-r--   0 a         (1009) a         (1010)      661 2023-04-19 01:55:38.000000 hak-0.0.9/hak/int/get_prime_factorisation.py
+-rw-rw-r--   0 a         (1009) a         (1010)      104 2023-04-19 01:55:38.000000 hak-0.0.9/hak/int/is_a.py
+-rw-rw-r--   0 a         (1009) a         (1010)      426 2023-04-19 01:55:38.000000 hak-0.0.9/hak/int/is_prime.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/int/year/
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/int/year/days/
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/int/year/days/count/
+-rw-rw-r--   0 a         (1009) a         (1010)      128 2023-04-19 01:55:38.000000 hak-0.0.9/hak/int/year/days/count/get.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/int/year/days/first/
+-rw-rw-r--   0 a         (1009) a         (1010)      154 2023-04-19 01:55:38.000000 hak-0.0.9/hak/int/year/days/first/get.py
+-rw-rw-r--   0 a         (1009) a         (1010)      420 2023-04-19 01:55:38.000000 hak-0.0.9/hak/int/year/days/get.py
+-rw-rw-r--   0 a         (1009) a         (1010)      153 2023-04-19 01:55:38.000000 hak-0.0.9/hak/int/year/now.py
+-rw-rw-r--   0 a         (1009) a         (1010)      448 2023-04-19 01:55:38.000000 hak-0.0.9/hak/l.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/list/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.9/hak/list/__init__.py
+-rw-rw-r--   0 a         (1009) a         (1010)      116 2023-04-19 01:55:38.000000 hak-0.0.9/hak/list/is_a.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/list/strings/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.9/hak/list/strings/__init__.py
+-rw-rw-r--   0 a         (1009) a         (1010)      130 2023-04-19 04:41:08.000000 hak-0.0.9/hak/list/strings/add_src_funks_prefix.py
+-rw-rw-r--   0 a         (1009) a         (1010)      586 2023-04-19 01:55:38.000000 hak-0.0.9/hak/list/strings/compare.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/list/strings/contain/
+-rw-rw-r--   0 a         (1009) a         (1010)      145 2023-04-19 04:43:23.000000 hak-0.0.9/hak/list/strings/contain/version.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/list/strings/filepaths/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.9/hak/list/strings/filepaths/__init__.py
+-rw-rw-r--   0 a         (1009) a         (1010)     1228 2023-04-19 04:38:09.000000 hak-0.0.9/hak/list/strings/filepaths/get.py
+-rw-rw-r--   0 a         (1009) a         (1010)     2222 2023-04-19 04:44:27.000000 hak-0.0.9/hak/list/strings/find_first_diff.py
+-rw-rw-r--   0 a         (1009) a         (1010)      434 2023-04-19 04:45:12.000000 hak-0.0.9/hak/list/strings/make_patch_version_change_to_py.py
+-rw-rw-r--   0 a         (1009) a         (1010)      293 2023-04-19 04:47:46.000000 hak-0.0.9/hak/list/strings/module_names_from_py_filenames.py
+-rw-rw-r--   0 a         (1009) a         (1010)      410 2023-04-19 04:48:58.000000 hak-0.0.9/hak/list/strings/patch_setup_cfg.py
+-rw-rw-r--   0 a         (1009) a         (1010)      622 2023-04-19 04:51:45.000000 hak-0.0.9/hak/list/strings/patch_setup_py.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/list/strings/pyfiles/
+-rw-rw-r--   0 a         (1009) a         (1010)     1514 2023-04-19 04:52:08.000000 hak-0.0.9/hak/list/strings/pyfiles/filter_out_items.py
+-rw-rw-r--   0 a         (1009) a         (1010)      766 2023-04-19 05:00:37.000000 hak-0.0.9/hak/list/strings/show_diff.py
+-rw-rw-r--   0 a         (1009) a         (1010)      647 2023-04-19 05:00:56.000000 hak-0.0.9/hak/list/strings/to_dict.py
+-rw-rw-r--   0 a         (1009) a         (1010)      357 2023-04-19 05:01:35.000000 hak-0.0.9/hak/list/strings/two_char_combinations.py
+-rw-rw-r--   0 a         (1009) a         (1010)      115 2023-04-19 01:55:38.000000 hak-0.0.9/hak/list/to_comma_separated_str.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/lists/
+-rw-rw-r--   0 a         (1009) a         (1010)      216 2023-04-19 01:55:38.000000 hak-0.0.9/hak/lists/merge.py
+-rw-rw-r--   0 a         (1009) a         (1010)     1131 2023-04-19 01:55:38.000000 hak-0.0.9/hak/load_durations_if_exists.py
+-rw-rw-r--   0 a         (1009) a         (1010)      123 2023-04-19 01:55:38.000000 hak-0.0.9/hak/log_2.py
+-rw-rw-r--   0 a         (1009) a         (1010)       84 2023-04-19 01:55:38.000000 hak-0.0.9/hak/nop.py
+-rw-rw-r--   0 a         (1009) a         (1010)       91 2023-04-19 01:55:38.000000 hak-0.0.9/hak/nop_state_x.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/patch/
+-rw-rw-r--   0 a         (1009) a         (1010)     7860 2023-04-19 09:15:38.000000 hak-0.0.9/hak/patch/do.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/period/
+-rw-rw-r--   0 a         (1009) a         (1010)      333 2023-04-19 01:55:38.000000 hak-0.0.9/hak/period/contains_day.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/pip/
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/pip/dist_tar/
+-rw-rw-r--   0 a         (1009) a         (1010)     3119 2023-04-19 07:21:09.000000 hak-0.0.9/hak/pip/dist_tar/make.py
+-rw-rw-r--   0 a         (1009) a         (1010)      804 2023-04-19 07:34:45.000000 hak-0.0.9/hak/pip/dist_tar/remove.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/pip/setup/
+-rw-rw-r--   0 a         (1009) a         (1010)     1305 2023-04-19 04:43:59.000000 hak-0.0.9/hak/pip/setup/update.py
+-rw-rw-r--   0 a         (1009) a         (1010)     1792 2023-04-19 08:32:41.000000 hak-0.0.9/hak/pip/upload.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/pip/version/
+-rw-rw-r--   0 a         (1009) a         (1010)      837 2023-04-19 01:55:38.000000 hak-0.0.9/hak/pip/version/get.py
+-rw-rw-r--   0 a         (1009) a         (1010)      120 2023-04-19 01:55:38.000000 hak-0.0.9/hak/pip/version/to_str.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/pyfiles/
+-rw-rw-r--   0 a         (1009) a         (1010)      157 2023-04-19 01:55:38.000000 hak-0.0.9/hak/pyfiles/format.py
+-rw-rw-r--   0 a         (1009) a         (1010)      838 2023-04-19 04:33:37.000000 hak-0.0.9/hak/pyfiles/format_and_commit.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/report/
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.714405 hak-0.0.9/hak/report/fail/
+-rw-rw-r--   0 a         (1009) a         (1010)      814 2023-04-19 01:55:38.000000 hak-0.0.9/hak/report/fail/no_xyz.py
+-rw-rw-r--   0 a         (1009) a         (1010)     1914 2023-04-19 01:55:38.000000 hak-0.0.9/hak/report/fail/xyz.py
+-rw-rw-r--   0 a         (1009) a         (1010)     1440 2023-04-19 01:55:38.000000 hak-0.0.9/hak/report/fail/z_return_neq_y_return.py
+-rw-rw-r--   0 a         (1009) a         (1010)     1601 2023-04-19 01:55:38.000000 hak-0.0.9/hak/report/fail/z_stdo_neq_y_stdo.py
+-rw-rw-r--   0 a         (1009) a         (1010)      887 2023-04-19 01:55:38.000000 hak-0.0.9/hak/report/property_failure.py
+-rw-rw-r--   0 a         (1009) a         (1010)      729 2023-04-19 01:55:38.000000 hak-0.0.9/hak/report/success.py
+-rw-rw-r--   0 a         (1009) a         (1010)      394 2023-04-19 01:55:38.000000 hak-0.0.9/hak/report/summarise_file.py
+-rw-rw-r--   0 a         (1009) a         (1010)      758 2023-04-19 01:55:38.000000 hak-0.0.9/hak/save_durations.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.714405 hak-0.0.9/hak/schedule/
+-rw-rw-r--   0 a         (1009) a         (1010)     3465 2023-04-19 01:55:38.000000 hak-0.0.9/hak/schedule/make.py
+-rw-rw-r--   0 a         (1009) a         (1010)      559 2023-04-19 01:55:38.000000 hak-0.0.9/hak/select_text_colour_from_width.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.714405 hak-0.0.9/hak/session/
+-rw-rw-r--   0 a         (1009) a         (1010)      146 2023-04-19 01:55:38.000000 hak-0.0.9/hak/session/is_a.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.714405 hak-0.0.9/hak/set/
+-rw-rw-r--   0 a         (1009) a         (1010)      114 2023-04-19 01:55:38.000000 hak-0.0.9/hak/set/is_a.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.706405 hak-0.0.9/hak/setup/
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.714405 hak-0.0.9/hak/setup/cfg/
+-rw-rw-r--   0 a         (1009) a         (1010)     1531 2023-04-19 07:22:45.000000 hak-0.0.9/hak/setup/cfg/update.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.714405 hak-0.0.9/hak/setup/py/
+-rw-rw-r--   0 a         (1009) a         (1010)     1633 2023-04-19 07:24:59.000000 hak-0.0.9/hak/setup/py/update.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.714405 hak-0.0.9/hak/string/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/__init__.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.714405 hak-0.0.9/hak/string/alphanumeric/
+-rw-rw-r--   0 a         (1009) a         (1010)      264 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/alphanumeric/fake.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.714405 hak-0.0.9/hak/string/append/
+-rw-rw-r--   0 a         (1009) a         (1010)       54 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/append/new_line.py
+-rw-rw-r--   0 a         (1009) a         (1010)      541 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/camel_to_snake.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.714405 hak-0.0.9/hak/string/char/
+-rw-rw-r--   0 a         (1009) a         (1010)      322 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/char/find_all_indices.py
+-rw-rw-r--   0 a         (1009) a         (1010)      128 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/char/is_digit.py
+-rw-rw-r--   0 a         (1009) a         (1010)      207 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/char/is_upper.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.714405 hak-0.0.9/hak/string/chars/
+-rw-rw-r--   0 a         (1009) a         (1010)      561 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/chars/remove.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.714405 hak-0.0.9/hak/string/colour/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/colour/__init__.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.714405 hak-0.0.9/hak/string/colour/bright/
+-rw-rw-r--   0 a         (1009) a         (1010)      162 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/colour/bright/blue.py
+-rw-rw-r--   0 a         (1009) a         (1010)      162 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/colour/bright/cyan.py
+-rw-rw-r--   0 a         (1009) a         (1010)      164 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/colour/bright/green.py
+-rw-rw-r--   0 a         (1009) a         (1010)      168 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/colour/bright/magenta.py
+-rw-rw-r--   0 a         (1009) a         (1010)      160 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/colour/bright/red.py
+-rw-rw-r--   0 a         (1009) a         (1010)      164 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/colour/bright/white.py
+-rw-rw-r--   0 a         (1009) a         (1010)      166 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/colour/bright/yellow.py
+-rw-rw-r--   0 a         (1009) a         (1010)      130 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/colour/danger.py
+-rw-rw-r--   0 a         (1009) a         (1010)      174 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/colour/danger_if_zero.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.714405 hak-0.0.9/hak/string/colour/dark/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/colour/dark/__init__.py
+-rw-rw-r--   0 a         (1009) a         (1010)      148 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/colour/dark/blue.py
+-rw-rw-r--   0 a         (1009) a         (1010)      148 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/colour/dark/cyan.py
+-rw-rw-r--   0 a         (1009) a         (1010)      154 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/colour/dark/default.py
+-rw-rw-r--   0 a         (1009) a         (1010)      150 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/colour/dark/green.py
+-rw-rw-r--   0 a         (1009) a         (1010)      154 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/colour/dark/magenta.py
+-rw-rw-r--   0 a         (1009) a         (1010)      146 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/colour/dark/red.py
+-rw-rw-r--   0 a         (1009) a         (1010)      150 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/colour/dark/white.py
+-rw-rw-r--   0 a         (1009) a         (1010)      152 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/colour/dark/yellow.py
+-rw-rw-r--   0 a         (1009) a         (1010)       64 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/colour/data.py
+-rw-rw-r--   0 a         (1009) a         (1010)      131 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/colour/info.py
+-rw-rw-r--   0 a         (1009) a         (1010)      131 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/colour/primary.py
+-rw-rw-r--   0 a         (1009) a         (1010)     2261 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/colour/rainbow.py
+-rw-rw-r--   0 a         (1009) a         (1010)      134 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/colour/secondary.py
+-rw-rw-r--   0 a         (1009) a         (1010)      267 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/colour/tgfr.py
+-rw-rw-r--   0 a         (1009) a         (1010)      135 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/colour/warning.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.714405 hak-0.0.9/hak/string/contains/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/contains/__init__.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.714405 hak-0.0.9/hak/string/contains/function/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/contains/function/__init__.py
+-rw-rw-r--   0 a         (1009) a         (1010)      341 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/contains/function/run.py
+-rw-rw-r--   0 a         (1009) a         (1010)      192 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/contains/function/test.py
+-rw-rw-r--   0 a         (1009) a         (1010)      224 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/contains/l.py
+-rw-rw-r--   0 a         (1009) a         (1010)       76 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/contains/version.py
+-rw-rw-r--   0 a         (1009) a         (1010)      105 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/count_x_in_y.py
+-rw-rw-r--   0 a         (1009) a         (1010)      996 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/delete_character_safely.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.714405 hak-0.0.9/hak/string/digits/
+-rw-rw-r--   0 a         (1009) a         (1010)      202 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/digits/remove.py
+-rw-rw-r--   0 a         (1009) a         (1010)      111 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/double_single_quotes.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.714405 hak-0.0.9/hak/string/family_name/
+-rw-rw-r--   0 a         (1009) a         (1010)   115522 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/family_name/fake.py
+-rw-rw-r--   0 a         (1009) a         (1010)      303 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/family_name/is_a.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.714405 hak-0.0.9/hak/string/filename/
+-rw-rw-r--   0 a         (1009) a         (1010)      126 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/filename/to_module_name.py
+-rw-rw-r--   0 a         (1009) a         (1010)      209 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/find_last_comma_index.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.714405 hak-0.0.9/hak/string/fn_name/
+-rw-rw-r--   0 a         (1009) a         (1010)      226 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/fn_name/is_ignorable.py
+-rw-rw-r--   0 a         (1009) a         (1010)     5035 2023-04-19 05:00:49.000000 hak-0.0.9/hak/string/format.py
+-rw-rw-r--   0 a         (1009) a         (1010)       73 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/has_at_symbol.py
+-rw-rw-r--   0 a         (1009) a         (1010)      132 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/has_digit.py
+-rw-rw-r--   0 a         (1009) a         (1010)      131 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/has_lowercase.py
+-rw-rw-r--   0 a         (1009) a         (1010)      259 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/has_other_char.py
+-rw-rw-r--   0 a         (1009) a         (1010)      172 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/has_seven_digits.py
+-rw-rw-r--   0 a         (1009) a         (1010)      132 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/has_uppercase.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.714405 hak-0.0.9/hak/string/hbar/
+-rw-rw-r--   0 a         (1009) a         (1010)      122 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/hbar/make.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.706405 hak-0.0.9/hak/string/header/
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.714405 hak-0.0.9/hak/string/header/python_file/
+-rw-rw-r--   0 a         (1009) a         (1010)      314 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/header/python_file/make.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.714405 hak-0.0.9/hak/string/header/test_table/
+-rw-rw-r--   0 a         (1009) a         (1010)      461 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/header/test_table/make.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.714405 hak-0.0.9/hak/string/indent/
+-rw-rw-r--   0 a         (1009) a         (1010)      137 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/indent/run_if_class_method.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.714405 hak-0.0.9/hak/string/insert/
+-rw-rw-r--   0 a         (1009) a         (1010)      602 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/insert/new_line_after_last_import_line.py
+-rw-rw-r--   0 a         (1009) a         (1010)      278 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/insert/new_line_before_comment.py
+-rw-rw-r--   0 a         (1009) a         (1010)      584 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/insert/new_line_before_def.py
+-rw-rw-r--   0 a         (1009) a         (1010)      251 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/insert/new_line_before_if_main.py
+-rw-rw-r--   0 a         (1009) a         (1010)      666 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/insert/new_line_before_lambda.py
+-rw-rw-r--   0 a         (1009) a         (1010)      292 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/insert/new_line_before_new_line_and_cea_.py
+-rw-rw-r--   0 a         (1009) a         (1010)      102 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/is_a.py
+-rw-rw-r--   0 a         (1009) a         (1010)      124 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/is_or_none.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.714405 hak-0.0.9/hak/string/json/
+-rw-rw-r--   0 a         (1009) a         (1010)      179 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/json/is_a.py
+-rw-rw-r--   0 a         (1009) a         (1010)      548 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/lambdarise.py
+-rw-rw-r--   0 a         (1009) a         (1010)      360 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/make_content_without_function.py
+-rw-rw-r--   0 a         (1009) a         (1010)      325 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/make_function_text.py
+-rw-rw-r--   0 a         (1009) a         (1010)      338 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/make_initial_content.py
+-rw-rw-r--   0 a         (1009) a         (1010)      319 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/make_new_function_text.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.714405 hak-0.0.9/hak/string/password/
+-rw-rw-r--   0 a         (1009) a         (1010)     1179 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/password/create.py
+-rw-rw-r--   0 a         (1009) a         (1010)      534 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/password/has_chars_from_3_sets.py
+-rw-rw-r--   0 a         (1009) a         (1010)      207 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/pop_left.py
+-rw-rw-r--   0 a         (1009) a         (1010)      219 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/pop_right.py
+-rw-rw-r--   0 a         (1009) a         (1010)      151 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/prepend_import.py
+-rw-rw-r--   0 a         (1009) a         (1010)      756 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/print_and_return_false.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.714405 hak-0.0.9/hak/string/refactor/
+-rw-rw-r--   0 a         (1009) a         (1010)     1218 2023-04-19 05:01:09.000000 hak-0.0.9/hak/string/refactor/by_two_char_combinations.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.714405 hak-0.0.9/hak/string/remove/
+-rw-rw-r--   0 a         (1009) a         (1010)      211 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/remove/empty_line_spaces.py
+-rw-rw-r--   0 a         (1009) a         (1010)      162 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/remove/empty_lines.py
+-rw-rw-r--   0 a         (1009) a         (1010)      441 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/remove/extra_new_line_following_class_definition.py
+-rw-rw-r--   0 a         (1009) a         (1010)      210 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/remove/first_new_line_if_starts_with_new_line.py
+-rw-rw-r--   0 a         (1009) a         (1010)       81 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/remove/whitespace_between_newlines.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.718405 hak-0.0.9/hak/string/replace/
+-rw-rw-r--   0 a         (1009) a         (1010)      241 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/replace/double_new_line_with_single_new_line.py
+-rw-rw-r--   0 a         (1009) a         (1010)      129 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/replace/single_new_line_with_empty_string.py
+-rw-rw-r--   0 a         (1009) a         (1010)      251 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/replace/triple_new_line_with_double_new_line.py
+-rw-rw-r--   0 a         (1009) a         (1010)      483 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/replace_unprintable.py
+-rw-rw-r--   0 a         (1009) a         (1010)     3361 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/separate_function_from_context.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.718405 hak-0.0.9/hak/string/single_line_function/
+-rw-rw-r--   0 a         (1009) a         (1010)      428 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/single_line_function/is_a.py
+-rw-rw-r--   0 a         (1009) a         (1010)      463 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/single_line_function/to_lambda_str.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.718405 hak-0.0.9/hak/string/spaces/
+-rw-rw-r--   0 a         (1009) a         (1010)      111 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/spaces/count.py
+-rw-rw-r--   0 a         (1009) a         (1010)      320 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/split_fn_name_and_text.py
+-rw-rw-r--   0 a         (1009) a         (1010)      344 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/strip_unprintable.py
+-rw-rw-r--   0 a         (1009) a         (1010)      265 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/to_cond_freq_dict.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.718405 hak-0.0.9/hak/string/token/
+-rw-rw-r--   0 a         (1009) a         (1010)     1263 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/token/substitute.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.718405 hak-0.0.9/hak/string/yyyymmdd/
+-rw-rw-r--   0 a         (1009) a         (1010)      238 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/yyyymmdd/to_date.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.706405 hak-0.0.9/hak/subprocess/
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.718405 hak-0.0.9/hak/subprocess/completed_process/
+-rw-rw-r--   0 a         (1009) a         (1010)      655 2023-04-19 01:55:38.000000 hak-0.0.9/hak/subprocess/completed_process/to_str.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.718405 hak-0.0.9/hak/system/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.9/hak/system/__init__.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.718405 hak-0.0.9/hak/system/git/
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.718405 hak-0.0.9/hak/system/git/commit/
+-rw-rw-r--   0 a         (1009) a         (1010)     2515 2023-04-19 01:55:38.000000 hak-0.0.9/hak/system/git/commit/run.py
+-rw-rw-r--   0 a         (1009) a         (1010)      384 2023-04-19 01:55:38.000000 hak-0.0.9/hak/system/git/commit_if_test_and_app_ok.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.718405 hak-0.0.9/hak/system/git/gitignore/
+-rw-rw-r--   0 a         (1009) a         (1010)      631 2023-04-19 01:55:38.000000 hak-0.0.9/hak/system/git/gitignore/make.py
+-rw-rw-r--   0 a         (1009) a         (1010)      486 2023-04-19 03:03:56.000000 hak-0.0.9/hak/system/git/init.py
+-rw-rw-r--   0 a         (1009) a         (1010)      725 2023-04-19 01:55:38.000000 hak-0.0.9/hak/system/git/log_oneline.py
+-rw-rw-r--   0 a         (1009) a         (1010)      866 2023-04-19 01:55:38.000000 hak-0.0.9/hak/system/git/push_after_delay.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.718405 hak-0.0.9/hak/system/screen/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.9/hak/system/screen/__init__.py
+-rw-rw-r--   0 a         (1009) a         (1010)      786 2023-04-19 01:55:38.000000 hak-0.0.9/hak/system/screen/clear.py
+-rw-rw-r--   0 a         (1009) a         (1010)     3119 2023-04-19 01:55:38.000000 hak-0.0.9/hak/terminal.py
+-rw-rw-r--   0 a         (1009) a         (1010)      337 2023-04-19 01:55:38.000000 hak-0.0.9/hak/ternary.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.718405 hak-0.0.9/hak/test/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.9/hak/test/__init__.py
+-rw-rw-r--   0 a         (1009) a         (1010)     2578 2023-04-19 01:55:38.000000 hak-0.0.9/hak/test/check_final_line.py
+-rw-rw-r--   0 a         (1009) a         (1010)     2689 2023-04-19 01:55:38.000000 hak-0.0.9/hak/test/check_line_lengths.py
+-rw-rw-r--   0 a         (1009) a         (1010)     2843 2023-04-19 01:55:38.000000 hak-0.0.9/hak/test/do.py
+-rw-rw-r--   0 a         (1009) a         (1010)     2450 2023-04-19 01:55:38.000000 hak-0.0.9/hak/test/final_line_check.py
+-rw-rw-r--   0 a         (1009) a         (1010)      774 2023-04-19 01:55:38.000000 hak-0.0.9/hak/test/line_lengths_check.py
+-rw-rw-r--   0 a         (1009) a         (1010)      926 2023-04-19 01:55:38.000000 hak-0.0.9/hak/test/oldest_file_print.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.718405 hak-0.0.9/hak/tup/
+-rw-rw-r--   0 a         (1009) a         (1010)      176 2023-04-19 01:55:38.000000 hak-0.0.9/hak/tup/is_a.py
+-rw-rw-r--   0 a         (1009) a         (1010)      617 2023-04-19 01:55:38.000000 hak-0.0.9/hak/update_duration.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.706405 hak-0.0.9/hak.egg-info/
+-rw-rw-r--   0 a         (1009) a         (1010)      994 2023-04-19 10:43:20.000000 hak-0.0.9/hak.egg-info/PKG-INFO
+-rw-rw-r--   0 a         (1009) a         (1010)     7947 2023-04-19 10:43:20.000000 hak-0.0.9/hak.egg-info/SOURCES.txt
+-rw-rw-r--   0 a         (1009) a         (1010)        1 2023-04-19 10:43:20.000000 hak-0.0.9/hak.egg-info/dependency_links.txt
+-rw-rw-r--   0 a         (1009) a         (1010)     1633 2023-04-19 10:43:20.000000 hak-0.0.9/hak.egg-info/top_level.txt
+-rw-rw-r--   0 a         (1009) a         (1010)      536 2023-04-19 10:43:20.718405 hak-0.0.9/setup.cfg
+-rw-rw-r--   0 a         (1009) a         (1010)     2781 2023-04-19 10:43:20.000000 hak-0.0.9/setup.py
```

### Comparing `hak-0.0.8/LICENSE` & `hak-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/PKG-INFO` & `hak-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hak
-Version: 0.0.8
+Version: 0.0.9
 Summary: Function Test Pair Toolbox
 Home-page: https://github.com/JohnForbes/hak
 Author: @JohnRForbes
 Author-email: john.robert.forbes@gmail.com
 License: MIT
 Description: # hak
         This project is a collection of function test pairs for common tasks.
```

### Comparing `hak-0.0.8/hak/check_if_ok_to_proceed.py` & `hak-0.0.9/hak/check_if_ok_to_proceed.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/date/public_holiday/is_a.py` & `hak-0.0.9/hak/date/public_holiday/is_a.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/date/to_utc_timestamp.py` & `hak-0.0.9/hak/date/to_utc_timestamp.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/date/year/easter_sunday/get.py` & `hak-0.0.9/hak/date/year/easter_sunday/get.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/dict/proposed_dismantlement/show.py` & `hak-0.0.9/hak/dict/proposed_dismantlement/show.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/dict/to_max_line_width_str.py` & `hak-0.0.9/hak/dict/to_max_line_width_str.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/dicts/compare.py` & `hak-0.0.9/hak/dicts/compare.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/dicts/merge_freq_dicts.py` & `hak-0.0.9/hak/dicts/merge_freq_dicts.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/directories/exist.py` & `hak-0.0.9/hak/directories/exist.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/directory/compress_to_tar.py` & `hak-0.0.9/hak/directory/compress_to_tar.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/directory/empty.py` & `hak-0.0.9/hak/directory/empty.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/directory/get_most_recently_modified.py` & `hak-0.0.9/hak/directory/get_most_recently_modified.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 from hak.directory.make import f as mkdirine
 from hak.file.save import f as save
 from hak.directory.remove import f as rmdir
 from hak.string.print_and_return_false import f as pf
 from os.path import getmtime
 from hak.list.strings.filepaths.get import f as get_filepaths
+from time import sleep
 
 def f(x):
   filepaths = get_filepaths(x, [])
-  newest = {'name': '', 'time': float('inf')}
-  for filename in filepaths:
-    last_modified_time = getmtime(filename)
-    if last_modified_time < newest['time']:
-      newest = {'file': filename, 'time': last_modified_time}
-  return newest['file']
+  latest = {'filepath': '', 'time': 0}
+  for filepath in filepaths:
+    last_modified_time = getmtime(filepath)
+    if last_modified_time > latest['time']:
+      latest = {'filepath': filepath, 'time': last_modified_time}
+  return latest['filepath']
 
 def up():
   x = {}
   x['dir_name'] = './test_directory_get_most_recently_modified'
   
   # Create test directory
   mkdirine(x['dir_name'])
 
   # create old file
   x['old_file_content'] = 'ABC'
   x['old_file_path'] = f"{x['dir_name']}/old_file.txt"
   save(x['old_file_path'], x['old_file_content'])
 
+  sleep(1)
+
   # create new file
   x['new_file_content'] = 'XYZ'
   x['new_file_path'] = f"{x['dir_name']}/new_file.txt"
   save(x['new_file_path'], x['new_file_content'])
 
   return x
 
 dn = lambda x: rmdir(x['dir_name'])
 
 def t():
   x = up()
-  y = x['old_file_path']
+  y = x['new_file_path']
   z = f(x['dir_name'])
   dn(x)
   return y == z or pf([f'x: {x}', f'y: {y}', f'z: {z}'])
```

### Comparing `hak-0.0.8/hak/directory/is_module.py` & `hak-0.0.9/hak/directory/is_module.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/directory/make.py` & `hak-0.0.9/hak/directory/make.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/directory/remove.py` & `hak-0.0.9/hak/directory/remove.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/duration.py` & `hak-0.0.9/hak/duration.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/duration_bar.py` & `hak-0.0.9/hak/duration_bar.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/fake/subprocess/run.py` & `hak-0.0.9/hak/fake/subprocess/run.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/file/decrypt.py` & `hak-0.0.9/hak/file/decrypt.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/file/encrypt.py` & `hak-0.0.9/hak/file/encrypt.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/file/load.py` & `hak-0.0.9/hak/file/load.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/file/pickle/load_if_exists.py` & `hak-0.0.9/hak/file/pickle/load_if_exists.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/file/pickle/save.py` & `hak-0.0.9/hak/file/pickle/save.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/file/py/create.py` & `hak-0.0.9/hak/file/py/create.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/file/py/dismantle.py` & `hak-0.0.9/hak/file/py/dismantle.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/file/py/extract_fn.py` & `hak-0.0.9/hak/file/py/extract_fn.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/file/save.py` & `hak-0.0.9/hak/file/save.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/file/save_lines.py` & `hak-0.0.9/hak/file/save_lines.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/file/secret/password/get.py` & `hak-0.0.9/hak/file/secret/password/get.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/file/secret/username/get.py` & `hak-0.0.9/hak/file/secret/username/get.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/file/tar/extract.py` & `hak-0.0.9/hak/file/tar/extract.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/files/pyfiles/dismantle.py` & `hak-0.0.9/hak/files/pyfiles/dismantle.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/int/get_prime_factorisation.py` & `hak-0.0.9/hak/int/get_prime_factorisation.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/list/strings/compare.py` & `hak-0.0.9/hak/list/strings/compare.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/list/strings/filepaths/get.py` & `hak-0.0.9/hak/list/strings/filepaths/get.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/list/strings/find_first_diff.py` & `hak-0.0.9/hak/list/strings/find_first_diff.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/list/strings/patch_setup_py.py` & `hak-0.0.9/hak/list/strings/patch_setup_py.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/list/strings/pyfiles/filter_out_items.py` & `hak-0.0.9/hak/list/strings/pyfiles/filter_out_items.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/list/strings/show_diff.py` & `hak-0.0.9/hak/list/strings/show_diff.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/list/strings/to_dict.py` & `hak-0.0.9/hak/list/strings/to_dict.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/load_durations_if_exists.py` & `hak-0.0.9/hak/load_durations_if_exists.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/patch/do.py` & `hak-0.0.9/hak/patch/do.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/pip/dist_tar/make.py` & `hak-0.0.9/hak/pip/dist_tar/make.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/pip/dist_tar/remove.py` & `hak-0.0.9/hak/pip/dist_tar/remove.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/pip/setup/update.py` & `hak-0.0.9/hak/pip/setup/update.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/pip/upload.py` & `hak-0.0.9/hak/pip/upload.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/pip/version/get.py` & `hak-0.0.9/hak/pip/version/get.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/pyfiles/format_and_commit.py` & `hak-0.0.9/hak/pyfiles/format_and_commit.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/report/fail/no_xyz.py` & `hak-0.0.9/hak/report/fail/no_xyz.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/report/fail/xyz.py` & `hak-0.0.9/hak/report/fail/xyz.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/report/fail/z_return_neq_y_return.py` & `hak-0.0.9/hak/report/fail/z_return_neq_y_return.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/report/fail/z_stdo_neq_y_stdo.py` & `hak-0.0.9/hak/report/fail/z_stdo_neq_y_stdo.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/report/property_failure.py` & `hak-0.0.9/hak/report/property_failure.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/report/success.py` & `hak-0.0.9/hak/report/success.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/save_durations.py` & `hak-0.0.9/hak/save_durations.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/schedule/make.py` & `hak-0.0.9/hak/schedule/make.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/select_text_colour_from_width.py` & `hak-0.0.9/hak/select_text_colour_from_width.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/setup/cfg/update.py` & `hak-0.0.9/hak/setup/cfg/update.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/setup/py/update.py` & `hak-0.0.9/hak/setup/py/update.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/string/camel_to_snake.py` & `hak-0.0.9/hak/string/camel_to_snake.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/string/chars/remove.py` & `hak-0.0.9/hak/string/chars/remove.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/string/colour/rainbow.py` & `hak-0.0.9/hak/string/colour/rainbow.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/string/delete_character_safely.py` & `hak-0.0.9/hak/string/delete_character_safely.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/string/family_name/fake.py` & `hak-0.0.9/hak/string/family_name/fake.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/string/format.py` & `hak-0.0.9/hak/string/format.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/string/insert/new_line_after_last_import_line.py` & `hak-0.0.9/hak/string/insert/new_line_after_last_import_line.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/string/insert/new_line_before_def.py` & `hak-0.0.9/hak/string/insert/new_line_before_def.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/string/insert/new_line_before_lambda.py` & `hak-0.0.9/hak/string/insert/new_line_before_lambda.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/string/lambdarise.py` & `hak-0.0.9/hak/string/lambdarise.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/string/password/create.py` & `hak-0.0.9/hak/string/password/create.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/string/password/has_chars_from_3_sets.py` & `hak-0.0.9/hak/string/password/has_chars_from_3_sets.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/string/print_and_return_false.py` & `hak-0.0.9/hak/string/print_and_return_false.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/string/refactor/by_two_char_combinations.py` & `hak-0.0.9/hak/string/refactor/by_two_char_combinations.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/string/separate_function_from_context.py` & `hak-0.0.9/hak/string/separate_function_from_context.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/string/token/substitute.py` & `hak-0.0.9/hak/string/token/substitute.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/subprocess/completed_process/to_str.py` & `hak-0.0.9/hak/subprocess/completed_process/to_str.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/system/git/commit/run.py` & `hak-0.0.9/hak/system/git/commit/run.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/system/git/gitignore/make.py` & `hak-0.0.9/hak/system/git/gitignore/make.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/system/git/log_oneline.py` & `hak-0.0.9/hak/system/git/log_oneline.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/system/git/push_after_delay.py` & `hak-0.0.9/hak/system/git/push_after_delay.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/system/screen/clear.py` & `hak-0.0.9/hak/system/screen/clear.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/terminal.py` & `hak-0.0.9/hak/terminal.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/test/check_final_line.py` & `hak-0.0.9/hak/test/check_final_line.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/test/check_line_lengths.py` & `hak-0.0.9/hak/test/check_line_lengths.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/test/do.py` & `hak-0.0.9/hak/test/do.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/test/final_line_check.py` & `hak-0.0.9/hak/test/final_line_check.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/test/line_lengths_check.py` & `hak-0.0.9/hak/test/line_lengths_check.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/test/oldest_file_print.py` & `hak-0.0.9/hak/test/oldest_file_print.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak/update_duration.py` & `hak-0.0.9/hak/update_duration.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak.egg-info/PKG-INFO` & `hak-0.0.9/hak.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hak
-Version: 0.0.8
+Version: 0.0.9
 Summary: Function Test Pair Toolbox
 Home-page: https://github.com/JohnForbes/hak
 Author: @JohnRForbes
 Author-email: john.robert.forbes@gmail.com
 License: MIT
 Description: # hak
         This project is a collection of function test pairs for common tasks.
```

### Comparing `hak-0.0.8/hak.egg-info/SOURCES.txt` & `hak-0.0.9/hak.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/hak.egg-info/top_level.txt` & `hak-0.0.9/hak.egg-info/top_level.txt`

 * *Files identical despite different names*

### Comparing `hak-0.0.8/setup.cfg` & `hak-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hak
-version = 0.0.8
+version = 0.0.9
 author = John Forbes
 author_email = john.robert.forbes@gmail.com
 description = Function Test Pair Toolbox
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/JohnForbes/hak
 license_files = LICENSE
```

### Comparing `hak-0.0.8/setup.py` & `hak-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 from pathlib import Path
 long_description = Path("./README.md").read_text()
 
 setup(
   name='hak',
-  version='0.0.8',
+  version='0.0.9',
   license='MIT',
   description='Function Test Pair Toolbox',
   long_description=long_description,
   long_description_content_type="text/markdown",
   author='@JohnRForbes',
   author_email='john.robert.forbes@gmail.com',
   url='https://github.com/JohnForbes/hak',
```

