# Comparing `tmp/mia-accounting-1.4.1.tar.gz` & `tmp/mia-accounting-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mia-accounting-1.4.1.tar", last modified: Sat Apr 22 10:23:31 2023, max compression
+gzip compressed data, was "mia-accounting-1.5.0.tar", last modified: Sun Apr 23 10:49:14 2023, max compression
```

## Comparing `mia-accounting-1.4.1.tar` & `mia-accounting-1.5.0.tar`

### file list

```diff
@@ -1,304 +1,305 @@
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-22 10:23:31.915888 mia-accounting-1.4.1/
--rw-r--r--   0 imacat    (1000) users      (100)    11358 2015-02-17 18:06:12.000000 mia-accounting-1.4.1/LICENSE
--rw-r--r--   0 imacat    (1000) users      (100)     1070 2023-04-05 11:25:31.000000 mia-accounting-1.4.1/MANIFEST.in
--rw-r--r--   0 imacat    (1000) users      (100)     6670 2023-04-22 10:23:31.915888 mia-accounting-1.4.1/PKG-INFO
--rw-r--r--   0 imacat    (1000) users      (100)     5871 2023-04-11 13:56:49.000000 mia-accounting-1.4.1/README.rst
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-22 10:23:26.376008 mia-accounting-1.4.1/docs/
--rw-r--r--   0 imacat    (1000) users      (100)      638 2023-01-27 04:20:04.000000 mia-accounting-1.4.1/docs/Makefile
--rw-r--r--   0 imacat    (1000) users      (100)      804 2023-01-27 04:20:04.000000 mia-accounting-1.4.1/docs/make.bat
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-22 10:23:26.863997 mia-accounting-1.4.1/docs/source/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-22 10:23:26.895996 mia-accounting-1.4.1/docs/source/_static/
--rw-r--r--   0 imacat    (1000) users      (100)        0 2023-01-27 04:21:08.000000 mia-accounting-1.4.1/docs/source/_static/.keep
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-22 10:23:26.895996 mia-accounting-1.4.1/docs/source/_templates/
--rw-r--r--   0 imacat    (1000) users      (100)        0 2023-01-27 04:21:11.000000 mia-accounting-1.4.1/docs/source/_templates/.keep
--rw-r--r--   0 imacat    (1000) users      (100)     1035 2023-04-18 01:25:56.000000 mia-accounting-1.4.1/docs/source/accounting.account.rst
--rw-r--r--   0 imacat    (1000) users      (100)      959 2023-04-18 01:25:56.000000 mia-accounting-1.4.1/docs/source/accounting.base_account.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1053 2023-04-18 01:25:56.000000 mia-accounting-1.4.1/docs/source/accounting.currency.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1089 2023-04-18 01:25:56.000000 mia-accounting-1.4.1/docs/source/accounting.journal_entry.forms.rst
--rw-r--r--   0 imacat    (1000) users      (100)      937 2023-04-18 01:25:56.000000 mia-accounting-1.4.1/docs/source/accounting.journal_entry.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1162 2023-04-18 01:25:56.000000 mia-accounting-1.4.1/docs/source/accounting.journal_entry.utils.rst
--rw-r--r--   0 imacat    (1000) users      (100)      513 2023-04-18 01:25:56.000000 mia-accounting-1.4.1/docs/source/accounting.option.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1551 2023-04-18 01:25:56.000000 mia-accounting-1.4.1/docs/source/accounting.report.period.rst
--rw-r--r--   0 imacat    (1000) users      (100)     2460 2023-04-18 01:32:44.000000 mia-accounting-1.4.1/docs/source/accounting.report.reports.rst
--rw-r--r--   0 imacat    (1000) users      (100)      861 2023-04-18 01:25:56.000000 mia-accounting-1.4.1/docs/source/accounting.report.rst
--rw-r--r--   0 imacat    (1000) users      (100)     2168 2023-04-18 01:32:44.000000 mia-accounting-1.4.1/docs/source/accounting.report.utils.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1301 2023-04-18 01:32:44.000000 mia-accounting-1.4.1/docs/source/accounting.rst
--rw-r--r--   0 imacat    (1000) users      (100)     2405 2023-04-18 01:32:44.000000 mia-accounting-1.4.1/docs/source/accounting.utils.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1022 2023-04-22 10:22:47.000000 mia-accounting-1.4.1/docs/source/conf.py
--rw-r--r--   0 imacat    (1000) users      (100)     1508 2023-04-06 00:38:39.000000 mia-accounting-1.4.1/docs/source/examples.rst
--rw-r--r--   0 imacat    (1000) users      (100)     2837 2023-04-06 00:21:32.000000 mia-accounting-1.4.1/docs/source/history.rst
--rw-r--r--   0 imacat    (1000) users      (100)      508 2023-04-06 00:11:04.000000 mia-accounting-1.4.1/docs/source/index.rst
--rw-r--r--   0 imacat    (1000) users      (100)     3615 2023-04-11 13:56:49.000000 mia-accounting-1.4.1/docs/source/intro.rst
--rw-r--r--   0 imacat    (1000) users      (100)       53 2023-04-04 10:25:53.000000 mia-accounting-1.4.1/docs/source/modules.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1820 2023-04-22 10:22:47.000000 mia-accounting-1.4.1/pyproject.toml
--rw-r--r--   0 imacat    (1000) users      (100)       38 2023-04-22 10:23:31.915888 mia-accounting-1.4.1/setup.cfg
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-22 10:23:26.336008 mia-accounting-1.4.1/src/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-22 10:23:27.067993 mia-accounting-1.4.1/src/accounting/
--rw-r--r--   0 imacat    (1000) users      (100)     2995 2023-04-17 15:07:31.000000 mia-accounting-1.4.1/src/accounting/__init__.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-22 10:23:27.155991 mia-accounting-1.4.1/src/accounting/account/
--rw-r--r--   0 imacat    (1000) users      (100)     1203 2023-04-10 15:59:48.000000 mia-accounting-1.4.1/src/accounting/account/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3868 2023-04-10 15:59:48.000000 mia-accounting-1.4.1/src/accounting/account/commands.py
--rw-r--r--   0 imacat    (1000) users      (100)     1512 2023-04-04 09:21:35.000000 mia-accounting-1.4.1/src/accounting/account/converters.py
--rw-r--r--   0 imacat    (1000) users      (100)     7145 2023-04-04 09:21:33.000000 mia-accounting-1.4.1/src/accounting/account/forms.py
--rw-r--r--   0 imacat    (1000) users      (100)     2209 2023-04-04 09:21:35.000000 mia-accounting-1.4.1/src/accounting/account/queries.py
--rw-r--r--   0 imacat    (1000) users      (100)     7416 2023-04-09 02:08:22.000000 mia-accounting-1.4.1/src/accounting/account/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-22 10:23:27.227989 mia-accounting-1.4.1/src/accounting/base_account/
--rw-r--r--   0 imacat    (1000) users      (100)     1240 2023-04-10 15:59:48.000000 mia-accounting-1.4.1/src/accounting/base_account/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     1800 2023-04-10 15:59:48.000000 mia-accounting-1.4.1/src/accounting/base_account/commands.py
--rw-r--r--   0 imacat    (1000) users      (100)     1592 2023-04-04 09:21:35.000000 mia-accounting-1.4.1/src/accounting/base_account/converters.py
--rw-r--r--   0 imacat    (1000) users      (100)     1769 2023-04-04 09:21:37.000000 mia-accounting-1.4.1/src/accounting/base_account/queries.py
--rw-r--r--   0 imacat    (1000) users      (100)     1812 2023-04-09 02:08:22.000000 mia-accounting-1.4.1/src/accounting/base_account/views.py
--rw-r--r--   0 imacat    (1000) users      (100)     2138 2023-04-10 15:59:48.000000 mia-accounting-1.4.1/src/accounting/commands.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-22 10:23:27.431985 mia-accounting-1.4.1/src/accounting/currency/
--rw-r--r--   0 imacat    (1000) users      (100)     1312 2023-04-10 15:59:48.000000 mia-accounting-1.4.1/src/accounting/currency/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     2212 2023-04-10 15:59:48.000000 mia-accounting-1.4.1/src/accounting/currency/commands.py
--rw-r--r--   0 imacat    (1000) users      (100)     1556 2023-04-04 09:21:35.000000 mia-accounting-1.4.1/src/accounting/currency/converters.py
--rw-r--r--   0 imacat    (1000) users      (100)     3172 2023-04-04 09:21:36.000000 mia-accounting-1.4.1/src/accounting/currency/forms.py
--rw-r--r--   0 imacat    (1000) users      (100)     1720 2023-04-04 09:21:34.000000 mia-accounting-1.4.1/src/accounting/currency/queries.py
--rw-r--r--   0 imacat    (1000) users      (100)     6609 2023-04-09 02:08:22.000000 mia-accounting-1.4.1/src/accounting/currency/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-22 10:23:27.507983 mia-accounting-1.4.1/src/accounting/data/
--rw-r--r--   0 imacat    (1000) users      (100)    36368 2023-03-14 01:04:26.000000 mia-accounting-1.4.1/src/accounting/data/base_accounts.csv
--rw-r--r--   0 imacat    (1000) users      (100)      370 2023-03-14 01:04:26.000000 mia-accounting-1.4.1/src/accounting/data/currencies.csv
--rw-r--r--   0 imacat    (1000) users      (100)     3144 2023-04-04 09:21:33.000000 mia-accounting-1.4.1/src/accounting/forms.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-22 10:23:27.583981 mia-accounting-1.4.1/src/accounting/journal_entry/
--rw-r--r--   0 imacat    (1000) users      (100)     1376 2023-04-04 09:21:35.000000 mia-accounting-1.4.1/src/accounting/journal_entry/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3283 2023-04-11 16:41:29.000000 mia-accounting-1.4.1/src/accounting/journal_entry/converters.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-22 10:23:27.759978 mia-accounting-1.4.1/src/accounting/journal_entry/forms/
--rw-r--r--   0 imacat    (1000) users      (100)      934 2023-04-04 09:21:37.000000 mia-accounting-1.4.1/src/accounting/journal_entry/forms/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)    11055 2023-04-08 10:12:54.000000 mia-accounting-1.4.1/src/accounting/journal_entry/forms/currency.py
--rw-r--r--   0 imacat    (1000) users      (100)    24553 2023-04-04 09:21:37.000000 mia-accounting-1.4.1/src/accounting/journal_entry/forms/journal_entry.py
--rw-r--r--   0 imacat    (1000) users      (100)    19883 2023-04-17 23:32:14.000000 mia-accounting-1.4.1/src/accounting/journal_entry/forms/line_item.py
--rw-r--r--   0 imacat    (1000) users      (100)     3408 2023-04-04 09:21:35.000000 mia-accounting-1.4.1/src/accounting/journal_entry/forms/reorder.py
--rw-r--r--   0 imacat    (1000) users      (100)     2535 2023-04-04 09:21:32.000000 mia-accounting-1.4.1/src/accounting/journal_entry/template_filters.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-22 10:23:27.871975 mia-accounting-1.4.1/src/accounting/journal_entry/utils/
--rw-r--r--   0 imacat    (1000) users      (100)      729 2023-04-04 09:21:32.000000 mia-accounting-1.4.1/src/accounting/journal_entry/utils/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     1802 2023-04-17 23:37:17.000000 mia-accounting-1.4.1/src/accounting/journal_entry/utils/account_option.py
--rw-r--r--   0 imacat    (1000) users      (100)    12987 2023-04-17 23:42:37.000000 mia-accounting-1.4.1/src/accounting/journal_entry/utils/description_editor.py
--rw-r--r--   0 imacat    (1000) users      (100)    12679 2023-04-04 09:21:35.000000 mia-accounting-1.4.1/src/accounting/journal_entry/utils/operators.py
--rw-r--r--   0 imacat    (1000) users      (100)     3787 2023-04-08 10:12:55.000000 mia-accounting-1.4.1/src/accounting/journal_entry/utils/original_line_items.py
--rw-r--r--   0 imacat    (1000) users      (100)     9472 2023-04-09 02:08:22.000000 mia-accounting-1.4.1/src/accounting/journal_entry/views.py
--rw-r--r--   0 imacat    (1000) users      (100)     3809 2023-04-04 09:21:33.000000 mia-accounting-1.4.1/src/accounting/locale.py
--rw-r--r--   0 imacat    (1000) users      (100)    33510 2023-04-18 00:13:36.000000 mia-accounting-1.4.1/src/accounting/models.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-22 10:23:27.955973 mia-accounting-1.4.1/src/accounting/option/
--rw-r--r--   0 imacat    (1000) users      (100)      993 2023-04-04 09:21:35.000000 mia-accounting-1.4.1/src/accounting/option/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     9762 2023-04-08 00:27:23.000000 mia-accounting-1.4.1/src/accounting/option/forms.py
--rw-r--r--   0 imacat    (1000) users      (100)     2827 2023-04-04 09:21:32.000000 mia-accounting-1.4.1/src/accounting/option/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-22 10:23:28.087971 mia-accounting-1.4.1/src/accounting/report/
--rw-r--r--   0 imacat    (1000) users      (100)     1362 2023-04-08 10:12:56.000000 mia-accounting-1.4.1/src/accounting/report/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3301 2023-04-08 10:12:56.000000 mia-accounting-1.4.1/src/accounting/report/converters.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-22 10:23:28.299966 mia-accounting-1.4.1/src/accounting/report/period/
--rw-r--r--   0 imacat    (1000) users      (100)      793 2023-04-04 09:21:32.000000 mia-accounting-1.4.1/src/accounting/report/period/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3677 2023-04-04 09:21:34.000000 mia-accounting-1.4.1/src/accounting/report/period/chooser.py
--rw-r--r--   0 imacat    (1000) users      (100)     5530 2023-04-04 09:21:35.000000 mia-accounting-1.4.1/src/accounting/report/period/description.py
--rw-r--r--   0 imacat    (1000) users      (100)     1045 2023-04-04 09:21:36.000000 mia-accounting-1.4.1/src/accounting/report/period/month_end.py
--rw-r--r--   0 imacat    (1000) users      (100)     4063 2023-04-04 09:21:31.000000 mia-accounting-1.4.1/src/accounting/report/period/parser.py
--rw-r--r--   0 imacat    (1000) users      (100)     4513 2023-04-04 09:21:32.000000 mia-accounting-1.4.1/src/accounting/report/period/period.py
--rw-r--r--   0 imacat    (1000) users      (100)     4707 2023-04-04 09:21:34.000000 mia-accounting-1.4.1/src/accounting/report/period/shortcuts.py
--rw-r--r--   0 imacat    (1000) users      (100)     3894 2023-04-04 09:21:34.000000 mia-accounting-1.4.1/src/accounting/report/period/specification.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-22 10:23:28.639959 mia-accounting-1.4.1/src/accounting/report/reports/
--rw-r--r--   0 imacat    (1000) users      (100)      946 2023-04-04 09:21:36.000000 mia-accounting-1.4.1/src/accounting/report/reports/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)    17920 2023-04-06 01:50:58.000000 mia-accounting-1.4.1/src/accounting/report/reports/balance_sheet.py
--rw-r--r--   0 imacat    (1000) users      (100)    18935 2023-04-04 09:21:34.000000 mia-accounting-1.4.1/src/accounting/report/reports/income_expenses.py
--rw-r--r--   0 imacat    (1000) users      (100)    11733 2023-04-06 01:50:58.000000 mia-accounting-1.4.1/src/accounting/report/reports/income_statement.py
--rw-r--r--   0 imacat    (1000) users      (100)     8128 2023-04-07 22:59:57.000000 mia-accounting-1.4.1/src/accounting/report/reports/journal.py
--rw-r--r--   0 imacat    (1000) users      (100)    16685 2023-04-04 09:21:31.000000 mia-accounting-1.4.1/src/accounting/report/reports/ledger.py
--rw-r--r--   0 imacat    (1000) users      (100)     8819 2023-04-09 13:02:35.000000 mia-accounting-1.4.1/src/accounting/report/reports/search.py
--rw-r--r--   0 imacat    (1000) users      (100)     8853 2023-04-06 01:50:58.000000 mia-accounting-1.4.1/src/accounting/report/reports/trial_balance.py
--rw-r--r--   0 imacat    (1000) users      (100)     8094 2023-04-18 01:09:36.000000 mia-accounting-1.4.1/src/accounting/report/reports/unapplied.py
--rw-r--r--   0 imacat    (1000) users      (100)     5212 2023-04-18 01:09:36.000000 mia-accounting-1.4.1/src/accounting/report/reports/unapplied_accounts.py
--rw-r--r--   0 imacat    (1000) users      (100)     8164 2023-04-18 01:14:44.000000 mia-accounting-1.4.1/src/accounting/report/reports/unmatched.py
--rw-r--r--   0 imacat    (1000) users      (100)     5193 2023-04-18 01:09:36.000000 mia-accounting-1.4.1/src/accounting/report/reports/unmatched_accounts.py
--rw-r--r--   0 imacat    (1000) users      (100)     1205 2023-04-04 09:21:33.000000 mia-accounting-1.4.1/src/accounting/report/template_filters.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-22 10:23:29.059949 mia-accounting-1.4.1/src/accounting/report/utils/
--rw-r--r--   0 imacat    (1000) users      (100)      711 2023-04-04 09:21:34.000000 mia-accounting-1.4.1/src/accounting/report/utils/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     2996 2023-04-04 09:21:35.000000 mia-accounting-1.4.1/src/accounting/report/utils/base_page_params.py
--rw-r--r--   0 imacat    (1000) users      (100)     1143 2023-04-04 09:21:36.000000 mia-accounting-1.4.1/src/accounting/report/utils/base_report.py
--rw-r--r--   0 imacat    (1000) users      (100)     3340 2023-04-09 04:04:18.000000 mia-accounting-1.4.1/src/accounting/report/utils/csv_export.py
--rw-r--r--   0 imacat    (1000) users      (100)     7369 2023-04-18 01:18:28.000000 mia-accounting-1.4.1/src/accounting/report/utils/offset_matcher.py
--rw-r--r--   0 imacat    (1000) users      (100)     1368 2023-04-04 09:21:37.000000 mia-accounting-1.4.1/src/accounting/report/utils/option_link.py
--rw-r--r--   0 imacat    (1000) users      (100)     7865 2023-04-18 01:17:12.000000 mia-accounting-1.4.1/src/accounting/report/utils/report_chooser.py
--rw-r--r--   0 imacat    (1000) users      (100)     1371 2023-04-17 08:41:57.000000 mia-accounting-1.4.1/src/accounting/report/utils/report_type.py
--rw-r--r--   0 imacat    (1000) users      (100)     4472 2023-04-18 01:14:44.000000 mia-accounting-1.4.1/src/accounting/report/utils/unapplied.py
--rw-r--r--   0 imacat    (1000) users      (100)     2262 2023-04-18 01:14:44.000000 mia-accounting-1.4.1/src/accounting/report/utils/unmatched.py
--rw-r--r--   0 imacat    (1000) users      (100)     5440 2023-04-18 00:59:05.000000 mia-accounting-1.4.1/src/accounting/report/utils/urls.py
--rw-r--r--   0 imacat    (1000) users      (100)    14167 2023-04-18 01:14:44.000000 mia-accounting-1.4.1/src/accounting/report/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-22 10:23:26.336008 mia-accounting-1.4.1/src/accounting/static/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-22 10:23:29.087949 mia-accounting-1.4.1/src/accounting/static/css/
--rw-r--r--   0 imacat    (1000) users      (100)    13431 2023-04-18 00:10:33.000000 mia-accounting-1.4.1/src/accounting/static/css/style.css
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-22 10:23:29.467941 mia-accounting-1.4.1/src/accounting/static/js/
--rw-r--r--   0 imacat    (1000) users      (100)    10921 2023-04-04 10:05:35.000000 mia-accounting-1.4.1/src/accounting/static/js/account-form.js
--rw-r--r--   0 imacat    (1000) users      (100)     1599 2023-04-04 10:05:35.000000 mia-accounting-1.4.1/src/accounting/static/js/account-order.js
--rw-r--r--   0 imacat    (1000) users      (100)     4955 2023-04-04 10:05:35.000000 mia-accounting-1.4.1/src/accounting/static/js/currency-form.js
--rw-r--r--   0 imacat    (1000) users      (100)    38865 2023-04-17 23:44:56.000000 mia-accounting-1.4.1/src/accounting/static/js/description-editor.js
--rw-r--r--   0 imacat    (1000) users      (100)     3564 2023-04-04 10:05:35.000000 mia-accounting-1.4.1/src/accounting/static/js/drag-and-drop-reorder.js
--rw-r--r--   0 imacat    (1000) users      (100)     9211 2023-04-17 23:32:14.000000 mia-accounting-1.4.1/src/accounting/static/js/journal-entry-account-selector.js
--rw-r--r--   0 imacat    (1000) users      (100)    33086 2023-04-17 23:52:58.000000 mia-accounting-1.4.1/src/accounting/static/js/journal-entry-form.js
--rw-r--r--   0 imacat    (1000) users      (100)    19574 2023-04-19 16:28:28.000000 mia-accounting-1.4.1/src/accounting/static/js/journal-entry-line-item-editor.js
--rw-r--r--   0 imacat    (1000) users      (100)     1366 2023-04-04 10:05:35.000000 mia-accounting-1.4.1/src/accounting/static/js/journal-entry-order.js
--rw-r--r--   0 imacat    (1000) users      (100)     1436 2023-04-04 10:05:35.000000 mia-accounting-1.4.1/src/accounting/static/js/material-fab-speed-dial.js
--rw-r--r--   0 imacat    (1000) users      (100)    28660 2023-04-04 10:05:35.000000 mia-accounting-1.4.1/src/accounting/static/js/option-form.js
--rw-r--r--   0 imacat    (1000) users      (100)    11670 2023-04-17 23:40:31.000000 mia-accounting-1.4.1/src/accounting/static/js/original-line-item-selector.js
--rw-r--r--   0 imacat    (1000) users      (100)    10374 2023-04-04 10:05:35.000000 mia-accounting-1.4.1/src/accounting/static/js/period-chooser.js
--rw-r--r--   0 imacat    (1000) users      (100)     2708 2023-04-04 09:21:31.000000 mia-accounting-1.4.1/src/accounting/template_filters.py
--rw-r--r--   0 imacat    (1000) users      (100)     1126 2023-04-04 09:21:34.000000 mia-accounting-1.4.1/src/accounting/template_globals.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-22 10:23:26.336008 mia-accounting-1.4.1/src/accounting/templates/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-22 10:23:29.487940 mia-accounting-1.4.1/src/accounting/templates/accounting/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-22 10:23:29.679936 mia-accounting-1.4.1/src/accounting/templates/accounting/account/
--rw-r--r--   0 imacat    (1000) users      (100)     1034 2023-04-04 10:04:10.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/account/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     4266 2023-04-04 10:04:11.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/account/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1081 2023-04-04 10:04:11.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/account/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-22 10:23:29.695936 mia-accounting-1.4.1/src/accounting/templates/accounting/account/include/
--rw-r--r--   0 imacat    (1000) users      (100)     5704 2023-04-04 10:04:10.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/account/include/form.html
--rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-04 10:04:11.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/account/list.html
--rw-r--r--   0 imacat    (1000) users      (100)     3052 2023-04-04 10:04:12.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/account/order.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-22 10:23:29.751935 mia-accounting-1.4.1/src/accounting/templates/accounting/base-account/
--rw-r--r--   0 imacat    (1000) users      (100)     1581 2023-04-04 10:04:10.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/base-account/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     2065 2023-04-04 10:04:10.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/base-account/list.html
--rw-r--r--   0 imacat    (1000) users      (100)     1035 2023-04-04 10:04:10.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/base.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-22 10:23:29.831933 mia-accounting-1.4.1/src/accounting/templates/accounting/currency/
--rw-r--r--   0 imacat    (1000) users      (100)     1039 2023-04-04 10:04:12.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/currency/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     3883 2023-04-04 10:04:10.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/currency/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1152 2023-04-04 10:04:11.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/currency/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-22 10:23:29.867932 mia-accounting-1.4.1/src/accounting/templates/accounting/currency/include/
--rw-r--r--   0 imacat    (1000) users      (100)     2850 2023-04-04 10:04:10.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/currency/include/form.html
--rw-r--r--   0 imacat    (1000) users      (100)     2576 2023-04-04 10:04:10.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/currency/list.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-22 10:23:29.907931 mia-accounting-1.4.1/src/accounting/templates/accounting/include/
--rw-r--r--   0 imacat    (1000) users      (100)     2706 2023-04-17 15:07:31.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/include/nav.html
--rw-r--r--   0 imacat    (1000) users      (100)     1986 2023-04-04 10:04:11.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/include/pagination.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-22 10:23:29.923931 mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-22 10:23:29.991929 mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/disbursement/
--rw-r--r--   0 imacat    (1000) users      (100)     1149 2023-04-04 23:56:52.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/disbursement/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     2028 2023-04-04 10:04:11.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/disbursement/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1213 2023-04-04 10:04:09.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/disbursement/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-22 10:23:30.023929 mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/disbursement/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1195 2023-04-04 10:04:10.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/disbursement/include/form-currency.html
--rw-r--r--   0 imacat    (1000) users      (100)     2283 2023-04-04 10:04:12.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/disbursement/include/form.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-22 10:23:30.235924 mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/include/
--rw-r--r--   0 imacat    (1000) users      (100)     3406 2023-04-17 23:32:14.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)    14492 2023-04-17 23:42:37.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     3242 2023-04-17 23:11:57.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/include/detail-line-items.html
--rw-r--r--   0 imacat    (1000) users      (100)     4568 2023-04-04 23:56:52.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/include/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     2726 2023-04-04 10:04:10.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/include/form-currency.html
--rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-04 10:04:11.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/include/form-debit-credit.html
--rw-r--r--   0 imacat    (1000) users      (100)     6442 2023-04-17 23:54:15.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/include/form-line-item.html
--rw-r--r--   0 imacat    (1000) users      (100)     4370 2023-04-04 10:04:12.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/include/form.html
--rw-r--r--   0 imacat    (1000) users      (100)     4162 2023-04-04 10:04:11.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     2093 2023-04-04 10:04:11.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/include/order-journal-entry.html
--rw-r--r--   0 imacat    (1000) users      (100)     3791 2023-04-18 00:10:33.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     3083 2023-04-04 23:56:52.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/order.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-22 10:23:30.251924 mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/receipt/
--rw-r--r--   0 imacat    (1000) users      (100)     1134 2023-04-04 23:56:52.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/receipt/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     2025 2023-04-04 10:04:12.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/receipt/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1203 2023-04-04 10:04:11.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/receipt/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-22 10:23:30.255924 mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/receipt/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1194 2023-04-04 10:04:12.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/receipt/include/form-currency.html
--rw-r--r--   0 imacat    (1000) users      (100)     2278 2023-04-04 10:04:11.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/receipt/include/form.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-22 10:23:30.331922 mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/transfer/
--rw-r--r--   0 imacat    (1000) users      (100)     1127 2023-04-04 23:56:52.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/transfer/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     2691 2023-04-04 10:04:09.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/transfer/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1200 2023-04-04 10:04:10.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/transfer/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-22 10:23:30.331922 mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/transfer/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1649 2023-04-04 10:04:11.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html
--rw-r--r--   0 imacat    (1000) users      (100)     2845 2023-04-04 10:04:12.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/transfer/include/form.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-22 10:23:30.339922 mia-accounting-1.4.1/src/accounting/templates/accounting/option/
--rw-r--r--   0 imacat    (1000) users      (100)     2765 2023-04-08 10:12:54.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/option/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     4699 2023-04-08 00:27:23.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/option/form.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-22 10:23:30.343922 mia-accounting-1.4.1/src/accounting/templates/accounting/option/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1851 2023-04-04 10:04:10.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/option/include/form-recurring-expense-income.html
--rw-r--r--   0 imacat    (1000) users      (100)     3214 2023-04-04 10:04:12.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/option/include/form-recurring-item.html
--rw-r--r--   0 imacat    (1000) users      (100)     3301 2023-04-04 10:04:12.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     4276 2023-04-04 10:04:10.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-22 10:23:30.535918 mia-accounting-1.4.1/src/accounting/templates/accounting/report/
--rw-r--r--   0 imacat    (1000) users      (100)     5435 2023-04-18 00:39:27.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/report/balance-sheet.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-22 10:23:30.631916 mia-accounting-1.4.1/src/accounting/templates/accounting/report/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1970 2023-04-04 10:04:12.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/report/include/add-journal-entry-material-fab.html
--rw-r--r--   0 imacat    (1000) users      (100)     1708 2023-04-04 10:04:12.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/report/include/balance-sheet-section.html
--rw-r--r--   0 imacat    (1000) users      (100)     1281 2023-04-04 10:04:10.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/report/include/income-expenses-row-desktop.html
--rw-r--r--   0 imacat    (1000) users      (100)     1760 2023-04-04 10:04:12.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/report/include/income-expenses-row-mobile.html
--rw-r--r--   0 imacat    (1000) users      (100)     1252 2023-04-04 10:04:11.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/report/include/ledger-row-desktop.html
--rw-r--r--   0 imacat    (1000) users      (100)     1429 2023-04-04 10:04:10.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/report/include/ledger-row-mobile.html
--rw-r--r--   0 imacat    (1000) users      (100)     8857 2023-04-04 10:04:12.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/report/include/period-chooser.html
--rw-r--r--   0 imacat    (1000) users      (100)     1933 2023-04-04 23:56:52.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/report/include/search-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     5600 2023-04-18 00:10:33.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/report/include/toolbar-buttons.html
--rw-r--r--   0 imacat    (1000) users      (100)     4841 2023-04-18 00:34:44.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/report/income-expenses.html
--rw-r--r--   0 imacat    (1000) users      (100)     4618 2023-04-18 00:37:47.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/report/income-statement.html
--rw-r--r--   0 imacat    (1000) users      (100)     4202 2023-04-04 10:04:10.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/report/journal.html
--rw-r--r--   0 imacat    (1000) users      (100)     4946 2023-04-18 00:33:38.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/report/ledger.html
--rw-r--r--   0 imacat    (1000) users      (100)     4044 2023-04-04 10:04:11.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/report/search.html
--rw-r--r--   0 imacat    (1000) users      (100)     3710 2023-04-18 00:36:16.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/report/trial-balance.html
--rw-r--r--   0 imacat    (1000) users      (100)     3037 2023-04-18 00:59:05.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/report/unapplied-accounts.html
--rw-r--r--   0 imacat    (1000) users      (100)     3843 2023-04-18 00:59:06.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/report/unapplied.html
--rw-r--r--   0 imacat    (1000) users      (100)     3034 2023-04-18 00:59:05.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/report/unmatched-accounts.html
--rw-r--r--   0 imacat    (1000) users      (100)     6998 2023-04-18 00:59:05.000000 mia-accounting-1.4.1/src/accounting/templates/accounting/report/unmatched.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-22 10:23:30.667915 mia-accounting-1.4.1/src/accounting/translations/
--rw-r--r--   0 imacat    (1000) users      (100)    49437 2023-04-18 01:32:01.000000 mia-accounting-1.4.1/src/accounting/translations/accounting.pot
--rw-r--r--   0 imacat    (1000) users      (100)       80 2023-01-27 03:33:36.000000 mia-accounting-1.4.1/src/accounting/translations/babel.cfg
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-22 10:23:26.336008 mia-accounting-1.4.1/src/accounting/translations/zh_Hans/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-22 10:23:30.687914 mia-accounting-1.4.1/src/accounting/translations/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 imacat    (1000) users      (100)    16202 2023-04-18 01:32:11.000000 mia-accounting-1.4.1/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.mo
--rw-r--r--   0 imacat    (1000) users      (100)    54246 2023-04-18 01:32:11.000000 mia-accounting-1.4.1/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.po
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-22 10:23:26.336008 mia-accounting-1.4.1/src/accounting/translations/zh_Hant/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-22 10:23:30.695914 mia-accounting-1.4.1/src/accounting/translations/zh_Hant/LC_MESSAGES/
--rw-r--r--   0 imacat    (1000) users      (100)    16202 2023-04-18 01:32:11.000000 mia-accounting-1.4.1/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.mo
--rw-r--r--   0 imacat    (1000) users      (100)    54246 2023-04-18 01:32:11.000000 mia-accounting-1.4.1/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.po
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-22 10:23:30.847911 mia-accounting-1.4.1/src/accounting/utils/
--rw-r--r--   0 imacat    (1000) users      (100)      778 2023-04-04 09:21:31.000000 mia-accounting-1.4.1/src/accounting/utils/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     1385 2023-04-04 09:21:35.000000 mia-accounting-1.4.1/src/accounting/utils/cast.py
--rw-r--r--   0 imacat    (1000) users      (100)     3361 2023-04-04 09:21:34.000000 mia-accounting-1.4.1/src/accounting/utils/current_account.py
--rw-r--r--   0 imacat    (1000) users      (100)     1424 2023-04-04 09:21:35.000000 mia-accounting-1.4.1/src/accounting/utils/flash_errors.py
--rw-r--r--   0 imacat    (1000) users      (100)     1030 2023-04-04 09:21:32.000000 mia-accounting-1.4.1/src/accounting/utils/journal_entry_types.py
--rw-r--r--   0 imacat    (1000) users      (100)     2863 2023-04-04 09:21:35.000000 mia-accounting-1.4.1/src/accounting/utils/next_uri.py
--rw-r--r--   0 imacat    (1000) users      (100)     1198 2023-04-08 10:12:55.000000 mia-accounting-1.4.1/src/accounting/utils/offset_alias.py
--rw-r--r--   0 imacat    (1000) users      (100)     6906 2023-04-08 10:12:55.000000 mia-accounting-1.4.1/src/accounting/utils/options.py
--rw-r--r--   0 imacat    (1000) users      (100)    11734 2023-04-04 09:21:36.000000 mia-accounting-1.4.1/src/accounting/utils/pagination.py
--rw-r--r--   0 imacat    (1000) users      (100)     4260 2023-04-04 09:21:37.000000 mia-accounting-1.4.1/src/accounting/utils/permission.py
--rw-r--r--   0 imacat    (1000) users      (100)     1638 2023-04-04 09:21:34.000000 mia-accounting-1.4.1/src/accounting/utils/query.py
--rw-r--r--   0 imacat    (1000) users      (100)     1174 2023-04-04 09:21:34.000000 mia-accounting-1.4.1/src/accounting/utils/random_id.py
--rw-r--r--   0 imacat    (1000) users      (100)     1396 2023-04-04 09:21:37.000000 mia-accounting-1.4.1/src/accounting/utils/strip_text.py
--rw-r--r--   0 imacat    (1000) users      (100)     4970 2023-04-04 09:21:34.000000 mia-accounting-1.4.1/src/accounting/utils/user.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-22 10:23:30.919909 mia-accounting-1.4.1/src/mia_accounting.egg-info/
--rw-r--r--   0 imacat    (1000) users      (100)     6670 2023-04-22 10:23:26.000000 mia-accounting-1.4.1/src/mia_accounting.egg-info/PKG-INFO
--rw-r--r--   0 imacat    (1000) users      (100)    11408 2023-04-22 10:23:26.000000 mia-accounting-1.4.1/src/mia_accounting.egg-info/SOURCES.txt
--rw-r--r--   0 imacat    (1000) users      (100)        1 2023-04-22 10:23:26.000000 mia-accounting-1.4.1/src/mia_accounting.egg-info/dependency_links.txt
--rw-r--r--   0 imacat    (1000) users      (100)       93 2023-04-22 10:23:26.000000 mia-accounting-1.4.1/src/mia_accounting.egg-info/requires.txt
--rw-r--r--   0 imacat    (1000) users      (100)       11 2023-04-22 10:23:26.000000 mia-accounting-1.4.1/src/mia_accounting.egg-info/top_level.txt
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-22 10:23:31.323901 mia-accounting-1.4.1/tests/
--rwxr-xr-x   0 imacat    (1000) users      (100)     4341 2023-04-12 07:04:32.000000 mia-accounting-1.4.1/tests/babel-utils-test-site.py
--rwxr-xr-x   0 imacat    (1000) users      (100)     4297 2023-04-12 07:04:32.000000 mia-accounting-1.4.1/tests/babel-utils.py
--rw-r--r--   0 imacat    (1000) users      (100)    32736 2023-04-10 15:59:48.000000 mia-accounting-1.4.1/tests/test_account.py
--rw-r--r--   0 imacat    (1000) users      (100)     2409 2023-04-10 15:59:48.000000 mia-accounting-1.4.1/tests/test_base_account.py
--rw-r--r--   0 imacat    (1000) users      (100)     6113 2023-04-10 15:59:48.000000 mia-accounting-1.4.1/tests/test_commands.py
--rw-r--r--   0 imacat    (1000) users      (100)    23824 2023-04-10 15:59:48.000000 mia-accounting-1.4.1/tests/test_currency.py
--rw-r--r--   0 imacat    (1000) users      (100)    15999 2023-04-13 01:09:51.000000 mia-accounting-1.4.1/tests/test_description_editor.py
--rw-r--r--   0 imacat    (1000) users      (100)   103461 2023-04-13 01:09:51.000000 mia-accounting-1.4.1/tests/test_journal_entry.py
--rw-r--r--   0 imacat    (1000) users      (100)    38887 2023-04-13 01:09:51.000000 mia-accounting-1.4.1/tests/test_offset.py
--rw-r--r--   0 imacat    (1000) users      (100)    15935 2023-04-13 01:09:51.000000 mia-accounting-1.4.1/tests/test_option.py
--rw-r--r--   0 imacat    (1000) users      (100)    17862 2023-04-18 01:19:22.000000 mia-accounting-1.4.1/tests/test_report.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-22 10:23:31.495897 mia-accounting-1.4.1/tests/test_site/
--rw-r--r--   0 imacat    (1000) users      (100)     4505 2023-04-13 00:49:22.000000 mia-accounting-1.4.1/tests/test_site/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3898 2023-04-13 01:52:58.000000 mia-accounting-1.4.1/tests/test_site/auth.py
--rw-r--r--   0 imacat    (1000) users      (100)    13223 2023-04-13 01:30:40.000000 mia-accounting-1.4.1/tests/test_site/lib.py
--rw-r--r--   0 imacat    (1000) users      (100)     3414 2023-04-04 09:28:44.000000 mia-accounting-1.4.1/tests/test_site/locale.py
--rw-r--r--   0 imacat    (1000) users      (100)    13048 2023-04-13 01:52:58.000000 mia-accounting-1.4.1/tests/test_site/reset.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-22 10:23:31.547896 mia-accounting-1.4.1/tests/test_site/static/
--rw-r--r--   0 imacat    (1000) users      (100)     1420 2023-04-03 07:56:03.000000 mia-accounting-1.4.1/tests/test_site/static/favicon.svg
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-22 10:23:31.659893 mia-accounting-1.4.1/tests/test_site/templates/
--rw-r--r--   0 imacat    (1000) users      (100)     6435 2023-04-12 10:05:13.000000 mia-accounting-1.4.1/tests/test_site/templates/base.html
--rw-r--r--   0 imacat    (1000) users      (100)     1239 2023-04-11 14:27:31.000000 mia-accounting-1.4.1/tests/test_site/templates/home.html
--rw-r--r--   0 imacat    (1000) users      (100)     1532 2023-04-11 14:03:59.000000 mia-accounting-1.4.1/tests/test_site/templates/login.html
--rw-r--r--   0 imacat    (1000) users      (100)     1838 2023-04-12 10:05:13.000000 mia-accounting-1.4.1/tests/test_site/templates/reset.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-22 10:23:31.723892 mia-accounting-1.4.1/tests/test_site/translations/
--rw-r--r--   0 imacat    (1000) users      (100)       80 2023-02-03 05:00:02.000000 mia-accounting-1.4.1/tests/test_site/translations/babel.cfg
--rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-12 09:59:51.000000 mia-accounting-1.4.1/tests/test_site/translations/messages.pot
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-22 10:23:26.336008 mia-accounting-1.4.1/tests/test_site/translations/zh_Hans/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-22 10:23:31.835890 mia-accounting-1.4.1/tests/test_site/translations/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 imacat    (1000) users      (100)     2275 2023-04-12 10:00:18.000000 mia-accounting-1.4.1/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.mo
--rw-r--r--   0 imacat    (1000) users      (100)     3505 2023-04-12 10:00:18.000000 mia-accounting-1.4.1/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.po
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-22 10:23:26.336008 mia-accounting-1.4.1/tests/test_site/translations/zh_Hant/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-22 10:23:31.883889 mia-accounting-1.4.1/tests/test_site/translations/zh_Hant/LC_MESSAGES/
--rw-r--r--   0 imacat    (1000) users      (100)     2275 2023-04-12 10:00:18.000000 mia-accounting-1.4.1/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.mo
--rw-r--r--   0 imacat    (1000) users      (100)     3505 2023-04-12 10:05:13.000000 mia-accounting-1.4.1/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.po
--rw-r--r--   0 imacat    (1000) users      (100)    27794 2023-04-18 01:14:44.000000 mia-accounting-1.4.1/tests/test_unmatched_offset.py
--rw-r--r--   0 imacat    (1000) users      (100)    13640 2023-04-04 09:21:31.000000 mia-accounting-1.4.1/tests/test_utils.py
--rw-r--r--   0 imacat    (1000) users      (100)     5169 2023-04-13 01:09:51.000000 mia-accounting-1.4.1/tests/testlib.py
--rw-r--r--   0 imacat    (1000) users      (100)    16670 2023-04-13 01:09:51.000000 mia-accounting-1.4.1/tests/testlib_journal_entry.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.456268 mia-accounting-1.5.0/
+-rw-r--r--   0 imacat    (1000) users      (100)    11358 2015-02-17 18:06:12.000000 mia-accounting-1.5.0/LICENSE
+-rw-r--r--   0 imacat    (1000) users      (100)     1070 2023-04-05 11:25:31.000000 mia-accounting-1.5.0/MANIFEST.in
+-rw-r--r--   0 imacat    (1000) users      (100)     3412 2023-04-23 10:49:14.456268 mia-accounting-1.5.0/PKG-INFO
+-rw-r--r--   0 imacat    (1000) users      (100)     2525 2023-04-23 10:42:54.000000 mia-accounting-1.5.0/README.rst
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.424269 mia-accounting-1.5.0/docs/
+-rw-r--r--   0 imacat    (1000) users      (100)      638 2023-01-27 04:20:04.000000 mia-accounting-1.5.0/docs/Makefile
+-rw-r--r--   0 imacat    (1000) users      (100)      804 2023-01-27 04:20:04.000000 mia-accounting-1.5.0/docs/make.bat
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.424269 mia-accounting-1.5.0/docs/source/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.424269 mia-accounting-1.5.0/docs/source/_static/
+-rw-r--r--   0 imacat    (1000) users      (100)        0 2023-01-27 04:21:08.000000 mia-accounting-1.5.0/docs/source/_static/.keep
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.424269 mia-accounting-1.5.0/docs/source/_templates/
+-rw-r--r--   0 imacat    (1000) users      (100)        0 2023-01-27 04:21:11.000000 mia-accounting-1.5.0/docs/source/_templates/.keep
+-rw-r--r--   0 imacat    (1000) users      (100)     1035 2023-04-18 01:25:56.000000 mia-accounting-1.5.0/docs/source/accounting.account.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      959 2023-04-18 01:25:56.000000 mia-accounting-1.5.0/docs/source/accounting.base_account.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1053 2023-04-18 01:25:56.000000 mia-accounting-1.5.0/docs/source/accounting.currency.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1089 2023-04-18 01:25:56.000000 mia-accounting-1.5.0/docs/source/accounting.journal_entry.forms.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      937 2023-04-18 01:25:56.000000 mia-accounting-1.5.0/docs/source/accounting.journal_entry.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1162 2023-04-18 01:25:56.000000 mia-accounting-1.5.0/docs/source/accounting.journal_entry.utils.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      513 2023-04-18 01:25:56.000000 mia-accounting-1.5.0/docs/source/accounting.option.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1551 2023-04-18 01:25:56.000000 mia-accounting-1.5.0/docs/source/accounting.report.period.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     2460 2023-04-18 01:32:44.000000 mia-accounting-1.5.0/docs/source/accounting.report.reports.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      861 2023-04-18 01:25:56.000000 mia-accounting-1.5.0/docs/source/accounting.report.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     2168 2023-04-18 01:32:44.000000 mia-accounting-1.5.0/docs/source/accounting.report.utils.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1301 2023-04-18 01:32:44.000000 mia-accounting-1.5.0/docs/source/accounting.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     2405 2023-04-18 01:32:44.000000 mia-accounting-1.5.0/docs/source/accounting.utils.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     7170 2023-04-23 10:48:38.000000 mia-accounting-1.5.0/docs/source/changelog.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1051 2023-04-23 10:42:54.000000 mia-accounting-1.5.0/docs/source/conf.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1508 2023-04-06 00:38:39.000000 mia-accounting-1.5.0/docs/source/examples.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     2837 2023-04-06 00:21:32.000000 mia-accounting-1.5.0/docs/source/history.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      521 2023-04-23 05:51:17.000000 mia-accounting-1.5.0/docs/source/index.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     3462 2023-04-23 10:42:55.000000 mia-accounting-1.5.0/docs/source/intro.rst
+-rw-r--r--   0 imacat    (1000) users      (100)       53 2023-04-04 10:25:53.000000 mia-accounting-1.5.0/docs/source/modules.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1994 2023-04-23 10:42:54.000000 mia-accounting-1.5.0/pyproject.toml
+-rw-r--r--   0 imacat    (1000) users      (100)       38 2023-04-23 10:49:14.456268 mia-accounting-1.5.0/setup.cfg
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.420269 mia-accounting-1.5.0/src/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.428269 mia-accounting-1.5.0/src/accounting/
+-rw-r--r--   0 imacat    (1000) users      (100)     3045 2023-04-23 10:46:14.000000 mia-accounting-1.5.0/src/accounting/__init__.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.428269 mia-accounting-1.5.0/src/accounting/account/
+-rw-r--r--   0 imacat    (1000) users      (100)     1203 2023-04-10 15:59:48.000000 mia-accounting-1.5.0/src/accounting/account/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3868 2023-04-10 15:59:48.000000 mia-accounting-1.5.0/src/accounting/account/commands.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1512 2023-04-04 09:21:35.000000 mia-accounting-1.5.0/src/accounting/account/converters.py
+-rw-r--r--   0 imacat    (1000) users      (100)     7145 2023-04-04 09:21:33.000000 mia-accounting-1.5.0/src/accounting/account/forms.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2209 2023-04-04 09:21:35.000000 mia-accounting-1.5.0/src/accounting/account/queries.py
+-rw-r--r--   0 imacat    (1000) users      (100)     7416 2023-04-09 02:08:22.000000 mia-accounting-1.5.0/src/accounting/account/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.428269 mia-accounting-1.5.0/src/accounting/base_account/
+-rw-r--r--   0 imacat    (1000) users      (100)     1240 2023-04-10 15:59:48.000000 mia-accounting-1.5.0/src/accounting/base_account/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1800 2023-04-10 15:59:48.000000 mia-accounting-1.5.0/src/accounting/base_account/commands.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1592 2023-04-04 09:21:35.000000 mia-accounting-1.5.0/src/accounting/base_account/converters.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1769 2023-04-04 09:21:37.000000 mia-accounting-1.5.0/src/accounting/base_account/queries.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1812 2023-04-09 02:08:22.000000 mia-accounting-1.5.0/src/accounting/base_account/views.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2138 2023-04-10 15:59:48.000000 mia-accounting-1.5.0/src/accounting/commands.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.428269 mia-accounting-1.5.0/src/accounting/currency/
+-rw-r--r--   0 imacat    (1000) users      (100)     1312 2023-04-10 15:59:48.000000 mia-accounting-1.5.0/src/accounting/currency/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2212 2023-04-10 15:59:48.000000 mia-accounting-1.5.0/src/accounting/currency/commands.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1556 2023-04-04 09:21:35.000000 mia-accounting-1.5.0/src/accounting/currency/converters.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3172 2023-04-04 09:21:36.000000 mia-accounting-1.5.0/src/accounting/currency/forms.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1720 2023-04-04 09:21:34.000000 mia-accounting-1.5.0/src/accounting/currency/queries.py
+-rw-r--r--   0 imacat    (1000) users      (100)     6609 2023-04-09 02:08:22.000000 mia-accounting-1.5.0/src/accounting/currency/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.428269 mia-accounting-1.5.0/src/accounting/data/
+-rw-r--r--   0 imacat    (1000) users      (100)    36368 2023-03-14 01:04:26.000000 mia-accounting-1.5.0/src/accounting/data/base_accounts.csv
+-rw-r--r--   0 imacat    (1000) users      (100)      370 2023-03-14 01:04:26.000000 mia-accounting-1.5.0/src/accounting/data/currencies.csv
+-rw-r--r--   0 imacat    (1000) users      (100)     3144 2023-04-04 09:21:33.000000 mia-accounting-1.5.0/src/accounting/forms.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.428269 mia-accounting-1.5.0/src/accounting/journal_entry/
+-rw-r--r--   0 imacat    (1000) users      (100)     1376 2023-04-04 09:21:35.000000 mia-accounting-1.5.0/src/accounting/journal_entry/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3297 2023-04-23 01:52:21.000000 mia-accounting-1.5.0/src/accounting/journal_entry/converters.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.432269 mia-accounting-1.5.0/src/accounting/journal_entry/forms/
+-rw-r--r--   0 imacat    (1000) users      (100)      934 2023-04-04 09:21:37.000000 mia-accounting-1.5.0/src/accounting/journal_entry/forms/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)    11003 2023-04-23 05:21:41.000000 mia-accounting-1.5.0/src/accounting/journal_entry/forms/currency.py
+-rw-r--r--   0 imacat    (1000) users      (100)    24553 2023-04-04 09:21:37.000000 mia-accounting-1.5.0/src/accounting/journal_entry/forms/journal_entry.py
+-rw-r--r--   0 imacat    (1000) users      (100)    19808 2023-04-23 05:21:41.000000 mia-accounting-1.5.0/src/accounting/journal_entry/forms/line_item.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3408 2023-04-04 09:21:35.000000 mia-accounting-1.5.0/src/accounting/journal_entry/forms/reorder.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2535 2023-04-04 09:21:32.000000 mia-accounting-1.5.0/src/accounting/journal_entry/template_filters.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.432269 mia-accounting-1.5.0/src/accounting/journal_entry/utils/
+-rw-r--r--   0 imacat    (1000) users      (100)      729 2023-04-04 09:21:32.000000 mia-accounting-1.5.0/src/accounting/journal_entry/utils/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1802 2023-04-17 23:37:17.000000 mia-accounting-1.5.0/src/accounting/journal_entry/utils/account_option.py
+-rw-r--r--   0 imacat    (1000) users      (100)    12987 2023-04-17 23:42:37.000000 mia-accounting-1.5.0/src/accounting/journal_entry/utils/description_editor.py
+-rw-r--r--   0 imacat    (1000) users      (100)    12679 2023-04-04 09:21:35.000000 mia-accounting-1.5.0/src/accounting/journal_entry/utils/operators.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3722 2023-04-23 05:21:41.000000 mia-accounting-1.5.0/src/accounting/journal_entry/utils/original_line_items.py
+-rw-r--r--   0 imacat    (1000) users      (100)     9472 2023-04-09 02:08:22.000000 mia-accounting-1.5.0/src/accounting/journal_entry/views.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3809 2023-04-04 09:21:33.000000 mia-accounting-1.5.0/src/accounting/locale.py
+-rw-r--r--   0 imacat    (1000) users      (100)    32027 2023-04-23 05:21:54.000000 mia-accounting-1.5.0/src/accounting/models.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.432269 mia-accounting-1.5.0/src/accounting/option/
+-rw-r--r--   0 imacat    (1000) users      (100)      993 2023-04-04 09:21:35.000000 mia-accounting-1.5.0/src/accounting/option/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     9762 2023-04-08 00:27:23.000000 mia-accounting-1.5.0/src/accounting/option/forms.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2827 2023-04-04 09:21:32.000000 mia-accounting-1.5.0/src/accounting/option/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.432269 mia-accounting-1.5.0/src/accounting/report/
+-rw-r--r--   0 imacat    (1000) users      (100)     1362 2023-04-08 10:12:56.000000 mia-accounting-1.5.0/src/accounting/report/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3301 2023-04-08 10:12:56.000000 mia-accounting-1.5.0/src/accounting/report/converters.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.432269 mia-accounting-1.5.0/src/accounting/report/period/
+-rw-r--r--   0 imacat    (1000) users      (100)      793 2023-04-04 09:21:32.000000 mia-accounting-1.5.0/src/accounting/report/period/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3677 2023-04-04 09:21:34.000000 mia-accounting-1.5.0/src/accounting/report/period/chooser.py
+-rw-r--r--   0 imacat    (1000) users      (100)     5530 2023-04-04 09:21:35.000000 mia-accounting-1.5.0/src/accounting/report/period/description.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1045 2023-04-04 09:21:36.000000 mia-accounting-1.5.0/src/accounting/report/period/month_end.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4063 2023-04-04 09:21:31.000000 mia-accounting-1.5.0/src/accounting/report/period/parser.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4513 2023-04-04 09:21:32.000000 mia-accounting-1.5.0/src/accounting/report/period/period.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4707 2023-04-04 09:21:34.000000 mia-accounting-1.5.0/src/accounting/report/period/shortcuts.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3894 2023-04-04 09:21:34.000000 mia-accounting-1.5.0/src/accounting/report/period/specification.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.436269 mia-accounting-1.5.0/src/accounting/report/reports/
+-rw-r--r--   0 imacat    (1000) users      (100)      946 2023-04-04 09:21:36.000000 mia-accounting-1.5.0/src/accounting/report/reports/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)    17920 2023-04-06 01:50:58.000000 mia-accounting-1.5.0/src/accounting/report/reports/balance_sheet.py
+-rw-r--r--   0 imacat    (1000) users      (100)    18844 2023-04-23 05:21:41.000000 mia-accounting-1.5.0/src/accounting/report/reports/income_expenses.py
+-rw-r--r--   0 imacat    (1000) users      (100)    11733 2023-04-06 01:50:58.000000 mia-accounting-1.5.0/src/accounting/report/reports/income_statement.py
+-rw-r--r--   0 imacat    (1000) users      (100)     8128 2023-04-07 22:59:57.000000 mia-accounting-1.5.0/src/accounting/report/reports/journal.py
+-rw-r--r--   0 imacat    (1000) users      (100)    16567 2023-04-23 05:21:41.000000 mia-accounting-1.5.0/src/accounting/report/reports/ledger.py
+-rw-r--r--   0 imacat    (1000) users      (100)     8772 2023-04-23 05:21:41.000000 mia-accounting-1.5.0/src/accounting/report/reports/search.py
+-rw-r--r--   0 imacat    (1000) users      (100)     8853 2023-04-06 01:50:58.000000 mia-accounting-1.5.0/src/accounting/report/reports/trial_balance.py
+-rw-r--r--   0 imacat    (1000) users      (100)     8094 2023-04-18 01:09:36.000000 mia-accounting-1.5.0/src/accounting/report/reports/unapplied.py
+-rw-r--r--   0 imacat    (1000) users      (100)     5212 2023-04-18 01:09:36.000000 mia-accounting-1.5.0/src/accounting/report/reports/unapplied_accounts.py
+-rw-r--r--   0 imacat    (1000) users      (100)     8164 2023-04-18 01:14:44.000000 mia-accounting-1.5.0/src/accounting/report/reports/unmatched.py
+-rw-r--r--   0 imacat    (1000) users      (100)     5193 2023-04-18 01:09:36.000000 mia-accounting-1.5.0/src/accounting/report/reports/unmatched_accounts.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1205 2023-04-04 09:21:33.000000 mia-accounting-1.5.0/src/accounting/report/template_filters.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.436269 mia-accounting-1.5.0/src/accounting/report/utils/
+-rw-r--r--   0 imacat    (1000) users      (100)      711 2023-04-04 09:21:34.000000 mia-accounting-1.5.0/src/accounting/report/utils/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2996 2023-04-04 09:21:35.000000 mia-accounting-1.5.0/src/accounting/report/utils/base_page_params.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1143 2023-04-04 09:21:36.000000 mia-accounting-1.5.0/src/accounting/report/utils/base_report.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3340 2023-04-09 04:04:18.000000 mia-accounting-1.5.0/src/accounting/report/utils/csv_export.py
+-rw-r--r--   0 imacat    (1000) users      (100)     7369 2023-04-18 01:18:28.000000 mia-accounting-1.5.0/src/accounting/report/utils/offset_matcher.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1368 2023-04-04 09:21:37.000000 mia-accounting-1.5.0/src/accounting/report/utils/option_link.py
+-rw-r--r--   0 imacat    (1000) users      (100)     7865 2023-04-18 01:17:12.000000 mia-accounting-1.5.0/src/accounting/report/utils/report_chooser.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1371 2023-04-17 08:41:57.000000 mia-accounting-1.5.0/src/accounting/report/utils/report_type.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4385 2023-04-23 05:21:41.000000 mia-accounting-1.5.0/src/accounting/report/utils/unapplied.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2221 2023-04-23 05:21:41.000000 mia-accounting-1.5.0/src/accounting/report/utils/unmatched.py
+-rw-r--r--   0 imacat    (1000) users      (100)     5440 2023-04-18 00:59:05.000000 mia-accounting-1.5.0/src/accounting/report/utils/urls.py
+-rw-r--r--   0 imacat    (1000) users      (100)    14167 2023-04-18 01:14:44.000000 mia-accounting-1.5.0/src/accounting/report/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.420269 mia-accounting-1.5.0/src/accounting/static/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.436269 mia-accounting-1.5.0/src/accounting/static/css/
+-rw-r--r--   0 imacat    (1000) users      (100)    13431 2023-04-18 00:10:33.000000 mia-accounting-1.5.0/src/accounting/static/css/style.css
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.440269 mia-accounting-1.5.0/src/accounting/static/js/
+-rw-r--r--   0 imacat    (1000) users      (100)    10921 2023-04-04 10:05:35.000000 mia-accounting-1.5.0/src/accounting/static/js/account-form.js
+-rw-r--r--   0 imacat    (1000) users      (100)     1599 2023-04-04 10:05:35.000000 mia-accounting-1.5.0/src/accounting/static/js/account-order.js
+-rw-r--r--   0 imacat    (1000) users      (100)     4955 2023-04-04 10:05:35.000000 mia-accounting-1.5.0/src/accounting/static/js/currency-form.js
+-rw-r--r--   0 imacat    (1000) users      (100)    38865 2023-04-17 23:44:56.000000 mia-accounting-1.5.0/src/accounting/static/js/description-editor.js
+-rw-r--r--   0 imacat    (1000) users      (100)     3564 2023-04-04 10:05:35.000000 mia-accounting-1.5.0/src/accounting/static/js/drag-and-drop-reorder.js
+-rw-r--r--   0 imacat    (1000) users      (100)     9211 2023-04-17 23:32:14.000000 mia-accounting-1.5.0/src/accounting/static/js/journal-entry-account-selector.js
+-rw-r--r--   0 imacat    (1000) users      (100)    33086 2023-04-17 23:52:58.000000 mia-accounting-1.5.0/src/accounting/static/js/journal-entry-form.js
+-rw-r--r--   0 imacat    (1000) users      (100)    19574 2023-04-19 16:28:28.000000 mia-accounting-1.5.0/src/accounting/static/js/journal-entry-line-item-editor.js
+-rw-r--r--   0 imacat    (1000) users      (100)     1366 2023-04-04 10:05:35.000000 mia-accounting-1.5.0/src/accounting/static/js/journal-entry-order.js
+-rw-r--r--   0 imacat    (1000) users      (100)     1436 2023-04-04 10:05:35.000000 mia-accounting-1.5.0/src/accounting/static/js/material-fab-speed-dial.js
+-rw-r--r--   0 imacat    (1000) users      (100)    28660 2023-04-04 10:05:35.000000 mia-accounting-1.5.0/src/accounting/static/js/option-form.js
+-rw-r--r--   0 imacat    (1000) users      (100)    11670 2023-04-17 23:40:31.000000 mia-accounting-1.5.0/src/accounting/static/js/original-line-item-selector.js
+-rw-r--r--   0 imacat    (1000) users      (100)    10374 2023-04-04 10:05:35.000000 mia-accounting-1.5.0/src/accounting/static/js/period-chooser.js
+-rw-r--r--   0 imacat    (1000) users      (100)     2708 2023-04-04 09:21:31.000000 mia-accounting-1.5.0/src/accounting/template_filters.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1137 2023-04-23 01:43:59.000000 mia-accounting-1.5.0/src/accounting/template_globals.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.420269 mia-accounting-1.5.0/src/accounting/templates/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.440269 mia-accounting-1.5.0/src/accounting/templates/accounting/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.440269 mia-accounting-1.5.0/src/accounting/templates/accounting/account/
+-rw-r--r--   0 imacat    (1000) users      (100)     1034 2023-04-04 10:04:10.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/account/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4266 2023-04-04 10:04:11.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/account/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1081 2023-04-04 10:04:11.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/account/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.440269 mia-accounting-1.5.0/src/accounting/templates/accounting/account/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     5704 2023-04-04 10:04:10.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/account/include/form.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-04 10:04:11.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/account/list.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3052 2023-04-04 10:04:12.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/account/order.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.440269 mia-accounting-1.5.0/src/accounting/templates/accounting/base-account/
+-rw-r--r--   0 imacat    (1000) users      (100)     1581 2023-04-04 10:04:10.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/base-account/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2065 2023-04-04 10:04:10.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/base-account/list.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1035 2023-04-04 10:04:10.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/base.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.440269 mia-accounting-1.5.0/src/accounting/templates/accounting/currency/
+-rw-r--r--   0 imacat    (1000) users      (100)     1039 2023-04-04 10:04:12.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/currency/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3883 2023-04-04 10:04:10.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/currency/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1152 2023-04-04 10:04:11.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/currency/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.440269 mia-accounting-1.5.0/src/accounting/templates/accounting/currency/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     2850 2023-04-04 10:04:10.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/currency/include/form.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2576 2023-04-04 10:04:10.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/currency/list.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.440269 mia-accounting-1.5.0/src/accounting/templates/accounting/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     2706 2023-04-17 15:07:31.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/include/nav.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1986 2023-04-04 10:04:11.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/include/pagination.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.440269 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.440269 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/disbursement/
+-rw-r--r--   0 imacat    (1000) users      (100)     1149 2023-04-04 23:56:52.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/disbursement/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2028 2023-04-04 10:04:11.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/disbursement/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1213 2023-04-04 10:04:09.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/disbursement/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.440269 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/disbursement/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1195 2023-04-04 10:04:10.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/disbursement/include/form-currency.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2283 2023-04-04 10:04:12.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/disbursement/include/form.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.444269 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     3406 2023-04-17 23:32:14.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)    14492 2023-04-17 23:42:37.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3242 2023-04-17 23:11:57.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/include/detail-line-items.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4568 2023-04-04 23:56:52.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/include/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2726 2023-04-04 10:04:10.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/include/form-currency.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-04 10:04:11.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/include/form-debit-credit.html
+-rw-r--r--   0 imacat    (1000) users      (100)     6442 2023-04-17 23:54:15.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/include/form-line-item.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4370 2023-04-04 10:04:12.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/include/form.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4162 2023-04-04 10:04:11.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2093 2023-04-04 10:04:11.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/include/order-journal-entry.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3791 2023-04-18 00:10:33.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3083 2023-04-04 23:56:52.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/order.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.444269 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/receipt/
+-rw-r--r--   0 imacat    (1000) users      (100)     1134 2023-04-04 23:56:52.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/receipt/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2025 2023-04-04 10:04:12.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/receipt/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1203 2023-04-04 10:04:11.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/receipt/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.444269 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/receipt/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1194 2023-04-04 10:04:12.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/receipt/include/form-currency.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2278 2023-04-04 10:04:11.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/receipt/include/form.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.444269 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/transfer/
+-rw-r--r--   0 imacat    (1000) users      (100)     1127 2023-04-04 23:56:52.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/transfer/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2691 2023-04-04 10:04:09.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/transfer/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1200 2023-04-04 10:04:10.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/transfer/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.444269 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/transfer/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1649 2023-04-04 10:04:11.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2845 2023-04-04 10:04:12.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/transfer/include/form.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.444269 mia-accounting-1.5.0/src/accounting/templates/accounting/option/
+-rw-r--r--   0 imacat    (1000) users      (100)     2765 2023-04-08 10:12:54.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/option/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4699 2023-04-08 00:27:23.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/option/form.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.444269 mia-accounting-1.5.0/src/accounting/templates/accounting/option/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1851 2023-04-04 10:04:10.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/option/include/form-recurring-expense-income.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3214 2023-04-04 10:04:12.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/option/include/form-recurring-item.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3301 2023-04-04 10:04:12.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4276 2023-04-04 10:04:10.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.448269 mia-accounting-1.5.0/src/accounting/templates/accounting/report/
+-rw-r--r--   0 imacat    (1000) users      (100)     5435 2023-04-18 00:39:27.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/report/balance-sheet.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.448269 mia-accounting-1.5.0/src/accounting/templates/accounting/report/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1970 2023-04-04 10:04:12.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/report/include/add-journal-entry-material-fab.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1708 2023-04-04 10:04:12.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/report/include/balance-sheet-section.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1281 2023-04-04 10:04:10.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/report/include/income-expenses-row-desktop.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1760 2023-04-04 10:04:12.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/report/include/income-expenses-row-mobile.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1252 2023-04-04 10:04:11.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/report/include/ledger-row-desktop.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1429 2023-04-04 10:04:10.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/report/include/ledger-row-mobile.html
+-rw-r--r--   0 imacat    (1000) users      (100)     8857 2023-04-04 10:04:12.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/report/include/period-chooser.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1933 2023-04-04 23:56:52.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/report/include/search-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     5600 2023-04-18 00:10:33.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/report/include/toolbar-buttons.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4841 2023-04-18 00:34:44.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/report/income-expenses.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4618 2023-04-18 00:37:47.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/report/income-statement.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4202 2023-04-04 10:04:10.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/report/journal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4946 2023-04-18 00:33:38.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/report/ledger.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4044 2023-04-04 10:04:11.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/report/search.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3710 2023-04-18 00:36:16.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/report/trial-balance.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3037 2023-04-18 00:59:05.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/report/unapplied-accounts.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3843 2023-04-18 00:59:06.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/report/unapplied.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3034 2023-04-18 00:59:05.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/report/unmatched-accounts.html
+-rw-r--r--   0 imacat    (1000) users      (100)     6998 2023-04-18 00:59:05.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/report/unmatched.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.448269 mia-accounting-1.5.0/src/accounting/translations/
+-rw-r--r--   0 imacat    (1000) users      (100)    49437 2023-04-18 01:32:01.000000 mia-accounting-1.5.0/src/accounting/translations/accounting.pot
+-rw-r--r--   0 imacat    (1000) users      (100)       80 2023-01-27 03:33:36.000000 mia-accounting-1.5.0/src/accounting/translations/babel.cfg
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.420269 mia-accounting-1.5.0/src/accounting/translations/zh_Hans/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.448269 mia-accounting-1.5.0/src/accounting/translations/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 imacat    (1000) users      (100)    16202 2023-04-18 01:32:11.000000 mia-accounting-1.5.0/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.mo
+-rw-r--r--   0 imacat    (1000) users      (100)    54246 2023-04-18 01:32:11.000000 mia-accounting-1.5.0/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.po
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.420269 mia-accounting-1.5.0/src/accounting/translations/zh_Hant/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.448269 mia-accounting-1.5.0/src/accounting/translations/zh_Hant/LC_MESSAGES/
+-rw-r--r--   0 imacat    (1000) users      (100)    16202 2023-04-18 01:32:11.000000 mia-accounting-1.5.0/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.mo
+-rw-r--r--   0 imacat    (1000) users      (100)    54246 2023-04-18 01:32:11.000000 mia-accounting-1.5.0/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.po
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.452268 mia-accounting-1.5.0/src/accounting/utils/
+-rw-r--r--   0 imacat    (1000) users      (100)      778 2023-04-04 09:21:31.000000 mia-accounting-1.5.0/src/accounting/utils/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1081 2023-04-23 05:21:41.000000 mia-accounting-1.5.0/src/accounting/utils/cast.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3361 2023-04-04 09:21:34.000000 mia-accounting-1.5.0/src/accounting/utils/current_account.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1424 2023-04-04 09:21:35.000000 mia-accounting-1.5.0/src/accounting/utils/flash_errors.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1030 2023-04-04 09:21:32.000000 mia-accounting-1.5.0/src/accounting/utils/journal_entry_types.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2863 2023-04-04 09:21:35.000000 mia-accounting-1.5.0/src/accounting/utils/next_uri.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1198 2023-04-08 10:12:55.000000 mia-accounting-1.5.0/src/accounting/utils/offset_alias.py
+-rw-r--r--   0 imacat    (1000) users      (100)     6906 2023-04-08 10:12:55.000000 mia-accounting-1.5.0/src/accounting/utils/options.py
+-rw-r--r--   0 imacat    (1000) users      (100)    11734 2023-04-04 09:21:36.000000 mia-accounting-1.5.0/src/accounting/utils/pagination.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4260 2023-04-04 09:21:37.000000 mia-accounting-1.5.0/src/accounting/utils/permission.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1638 2023-04-04 09:21:34.000000 mia-accounting-1.5.0/src/accounting/utils/query.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1174 2023-04-04 09:21:34.000000 mia-accounting-1.5.0/src/accounting/utils/random_id.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1396 2023-04-04 09:21:37.000000 mia-accounting-1.5.0/src/accounting/utils/strip_text.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4970 2023-04-04 09:21:34.000000 mia-accounting-1.5.0/src/accounting/utils/user.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.452268 mia-accounting-1.5.0/src/mia_accounting.egg-info/
+-rw-r--r--   0 imacat    (1000) users      (100)     3412 2023-04-23 10:49:14.000000 mia-accounting-1.5.0/src/mia_accounting.egg-info/PKG-INFO
+-rw-r--r--   0 imacat    (1000) users      (100)    11434 2023-04-23 10:49:14.000000 mia-accounting-1.5.0/src/mia_accounting.egg-info/SOURCES.txt
+-rw-r--r--   0 imacat    (1000) users      (100)        1 2023-04-23 10:49:14.000000 mia-accounting-1.5.0/src/mia_accounting.egg-info/dependency_links.txt
+-rw-r--r--   0 imacat    (1000) users      (100)      107 2023-04-23 10:49:14.000000 mia-accounting-1.5.0/src/mia_accounting.egg-info/requires.txt
+-rw-r--r--   0 imacat    (1000) users      (100)       11 2023-04-23 10:49:14.000000 mia-accounting-1.5.0/src/mia_accounting.egg-info/top_level.txt
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.456268 mia-accounting-1.5.0/tests/
+-rwxr-xr-x   0 imacat    (1000) users      (100)     4341 2023-04-12 07:04:32.000000 mia-accounting-1.5.0/tests/babel-utils-test-site.py
+-rwxr-xr-x   0 imacat    (1000) users      (100)     4297 2023-04-12 07:04:32.000000 mia-accounting-1.5.0/tests/babel-utils.py
+-rw-r--r--   0 imacat    (1000) users      (100)    32736 2023-04-10 15:59:48.000000 mia-accounting-1.5.0/tests/test_account.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2409 2023-04-10 15:59:48.000000 mia-accounting-1.5.0/tests/test_base_account.py
+-rw-r--r--   0 imacat    (1000) users      (100)     6113 2023-04-10 15:59:48.000000 mia-accounting-1.5.0/tests/test_commands.py
+-rw-r--r--   0 imacat    (1000) users      (100)    23824 2023-04-10 15:59:48.000000 mia-accounting-1.5.0/tests/test_currency.py
+-rw-r--r--   0 imacat    (1000) users      (100)    15999 2023-04-13 01:09:51.000000 mia-accounting-1.5.0/tests/test_description_editor.py
+-rw-r--r--   0 imacat    (1000) users      (100)   103461 2023-04-13 01:09:51.000000 mia-accounting-1.5.0/tests/test_journal_entry.py
+-rw-r--r--   0 imacat    (1000) users      (100)    38887 2023-04-13 01:09:51.000000 mia-accounting-1.5.0/tests/test_offset.py
+-rw-r--r--   0 imacat    (1000) users      (100)    15935 2023-04-13 01:09:51.000000 mia-accounting-1.5.0/tests/test_option.py
+-rw-r--r--   0 imacat    (1000) users      (100)    17862 2023-04-18 01:19:22.000000 mia-accounting-1.5.0/tests/test_report.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.456268 mia-accounting-1.5.0/tests/test_site/
+-rw-r--r--   0 imacat    (1000) users      (100)     4505 2023-04-13 00:49:22.000000 mia-accounting-1.5.0/tests/test_site/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3898 2023-04-13 01:52:58.000000 mia-accounting-1.5.0/tests/test_site/auth.py
+-rw-r--r--   0 imacat    (1000) users      (100)    13223 2023-04-13 01:30:40.000000 mia-accounting-1.5.0/tests/test_site/lib.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3414 2023-04-04 09:28:44.000000 mia-accounting-1.5.0/tests/test_site/locale.py
+-rw-r--r--   0 imacat    (1000) users      (100)    13048 2023-04-13 01:52:58.000000 mia-accounting-1.5.0/tests/test_site/reset.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.456268 mia-accounting-1.5.0/tests/test_site/static/
+-rw-r--r--   0 imacat    (1000) users      (100)     1420 2023-04-03 07:56:03.000000 mia-accounting-1.5.0/tests/test_site/static/favicon.svg
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.456268 mia-accounting-1.5.0/tests/test_site/templates/
+-rw-r--r--   0 imacat    (1000) users      (100)     6435 2023-04-12 10:05:13.000000 mia-accounting-1.5.0/tests/test_site/templates/base.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1239 2023-04-11 14:27:31.000000 mia-accounting-1.5.0/tests/test_site/templates/home.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1532 2023-04-11 14:03:59.000000 mia-accounting-1.5.0/tests/test_site/templates/login.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1838 2023-04-12 10:05:13.000000 mia-accounting-1.5.0/tests/test_site/templates/reset.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.456268 mia-accounting-1.5.0/tests/test_site/translations/
+-rw-r--r--   0 imacat    (1000) users      (100)       80 2023-02-03 05:00:02.000000 mia-accounting-1.5.0/tests/test_site/translations/babel.cfg
+-rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-12 09:59:51.000000 mia-accounting-1.5.0/tests/test_site/translations/messages.pot
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.420269 mia-accounting-1.5.0/tests/test_site/translations/zh_Hans/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.456268 mia-accounting-1.5.0/tests/test_site/translations/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 imacat    (1000) users      (100)     2275 2023-04-12 10:00:18.000000 mia-accounting-1.5.0/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.mo
+-rw-r--r--   0 imacat    (1000) users      (100)     3505 2023-04-12 10:00:18.000000 mia-accounting-1.5.0/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.po
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.420269 mia-accounting-1.5.0/tests/test_site/translations/zh_Hant/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.456268 mia-accounting-1.5.0/tests/test_site/translations/zh_Hant/LC_MESSAGES/
+-rw-r--r--   0 imacat    (1000) users      (100)     2275 2023-04-12 10:00:18.000000 mia-accounting-1.5.0/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.mo
+-rw-r--r--   0 imacat    (1000) users      (100)     3505 2023-04-12 10:05:13.000000 mia-accounting-1.5.0/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.po
+-rw-r--r--   0 imacat    (1000) users      (100)    27794 2023-04-18 01:14:44.000000 mia-accounting-1.5.0/tests/test_unmatched_offset.py
+-rw-r--r--   0 imacat    (1000) users      (100)    13640 2023-04-04 09:21:31.000000 mia-accounting-1.5.0/tests/test_utils.py
+-rw-r--r--   0 imacat    (1000) users      (100)     5169 2023-04-13 01:09:51.000000 mia-accounting-1.5.0/tests/testlib.py
+-rw-r--r--   0 imacat    (1000) users      (100)    16670 2023-04-13 01:09:51.000000 mia-accounting-1.5.0/tests/testlib_journal_entry.py
```

### Comparing `mia-accounting-1.4.1/LICENSE` & `mia-accounting-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/MANIFEST.in` & `mia-accounting-1.5.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/docs/Makefile` & `mia-accounting-1.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/docs/make.bat` & `mia-accounting-1.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/docs/source/accounting.account.rst` & `mia-accounting-1.5.0/docs/source/accounting.account.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/docs/source/accounting.base_account.rst` & `mia-accounting-1.5.0/docs/source/accounting.base_account.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/docs/source/accounting.currency.rst` & `mia-accounting-1.5.0/docs/source/accounting.currency.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/docs/source/accounting.journal_entry.forms.rst` & `mia-accounting-1.5.0/docs/source/accounting.journal_entry.forms.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/docs/source/accounting.journal_entry.rst` & `mia-accounting-1.5.0/docs/source/accounting.journal_entry.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/docs/source/accounting.journal_entry.utils.rst` & `mia-accounting-1.5.0/docs/source/accounting.journal_entry.utils.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/docs/source/accounting.option.rst` & `mia-accounting-1.5.0/docs/source/accounting.option.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/docs/source/accounting.report.period.rst` & `mia-accounting-1.5.0/docs/source/accounting.report.period.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/docs/source/accounting.report.reports.rst` & `mia-accounting-1.5.0/docs/source/accounting.report.reports.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/docs/source/accounting.report.rst` & `mia-accounting-1.5.0/docs/source/accounting.report.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/docs/source/accounting.report.utils.rst` & `mia-accounting-1.5.0/docs/source/accounting.report.utils.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/docs/source/accounting.rst` & `mia-accounting-1.5.0/docs/source/accounting.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/docs/source/accounting.utils.rst` & `mia-accounting-1.5.0/docs/source/accounting.utils.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/docs/source/conf.py` & `mia-accounting-1.5.0/docs/source/conf.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 #
 # For the full list of built-in configuration values, see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 import os
 import sys
 
 sys.path.insert(0, os.path.abspath('../../src/'))
+import accounting
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'Mia! Accounting'
 copyright = '2023, imacat'
 author = 'imacat'
-release = '1.4.1'
+release = accounting.VERSION
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = ['sphinx.ext.autodoc']
 
 templates_path = ['_templates']
```

### Comparing `mia-accounting-1.4.1/docs/source/examples.rst` & `mia-accounting-1.5.0/docs/source/examples.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/docs/source/history.rst` & `mia-accounting-1.5.0/docs/source/history.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/docs/source/intro.rst` & `mia-accounting-1.5.0/docs/source/intro.rst`

 * *Files 4% similar despite different names*

```diff
@@ -99,28 +99,21 @@
         </div>
       </div>
     </nav>
 
 Check your Flask application and see how it works.
 
 
-Documentation
--------------
-
-Refer to the `documentation on Read the Docs`_.
-
-
 .. _Flask: https://flask.palletsprojects.com
 .. _double-entry bookkeeping: https://en.wikipedia.org/wiki/Double-entry_bookkeeping
 .. _live demonstration: https://accounting.imacat.idv.tw
 .. _test site: https://github.com/imacat/mia-accounting/tree/main/tests/test_site
 .. _source distribution: https://pypi.org/project/mia-accounting/#files
 .. _PyPI project page: https://pypi.org/project/mia-accounting
 .. _release page: https://github.com/imacat/mia-accounting/releases
 .. _Git repository: https://github.com/imacat/mia-accounting
 .. _CDN: https://en.wikipedia.org/wiki/Content_delivery_network
 .. _Bootstrap: https://getbootstrap.com
 .. _FontAwesome: https://fontawesome.com
 .. _Decimal.js: https://mikemcl.github.io/decimal.js
 .. _Tempus-Dominus: https://getdatepicker.com
 .. _Bootstrap navigation bar: https://getbootstrap.com/docs/5.3/components/navbar/
-.. _documentation on Read the Docs: https://mia-accounting.readthedocs.io
```

### Comparing `mia-accounting-1.4.1/pyproject.toml` & `mia-accounting-1.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 [project]
 name = "mia-accounting"
-version = "1.4.1"
+dynamic = ["version"]
 description = "A Flask accounting module."
 readme = "README.rst"
 requires-python = ">=3.11"
 authors = [
     {name = "imacat", email = "imacat@mail.imacat.idv.tw"},
 ]
 keywords = ["mia", "accounting", "flask"]
@@ -30,14 +30,15 @@
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
     "Framework :: Flask",
     "Topic :: Office/Business :: Financial :: Accounting",
 ]
 dependencies = [
     "flask",
+    "SQLAlchemy >= 2",
     "Flask-SQLAlchemy",
     "Flask-WTF",
     "Flask-Babel >= 3",
     "Flask-Babel-JS",
 ]
 
 [project.optional-dependencies]
@@ -45,21 +46,25 @@
     "unittest",
     "httpx",
     "OpenCC",
 ]
 
 [project.urls]
 "Documentation" = "https://mia-accounting.readthedocs.io"
+"Change Log" = "https://mia-accounting.readthedocs.io/en/latest/changelog.html"
 "Repository" = "https://github.com/imacat/mia-accounting"
 "Bug Tracker" = "https://github.com/imacat/mia-accounting/issues"
 "Demonstration" = "https://accounting.imacat.idv.tw"
 
 [build-system]
 requires = ["setuptools>=42"]
 build-backend = "setuptools.build_meta"
 
+[tool.setuptools.dynamic]
+version = {attr = "accounting.VERSION"}
+
 [tool.setuptools.exclude-package-data]
 "*" = [
     "babel.cfg",
     "*.pot",
     "*.po",
 ]
```

### Comparing `mia-accounting-1.4.1/src/accounting/__init__.py` & `mia-accounting-1.5.0/src/accounting/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 from pathlib import Path
 
 from flask import Flask, Blueprint
 from flask_sqlalchemy import SQLAlchemy
 
 from accounting.utils.user import UserUtilityInterface
 
+VERSION: str = "1.5.0"
+"""The package version."""
 db: SQLAlchemy = SQLAlchemy()
 """The database instance."""
 data_dir: Path = Path(__file__).parent / "data"
 """The data directory."""
 
 
 def init_app(app: Flask, user_utils: UserUtilityInterface,
```

### Comparing `mia-accounting-1.4.1/src/accounting/account/__init__.py` & `mia-accounting-1.5.0/src/accounting/account/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/account/commands.py` & `mia-accounting-1.5.0/src/accounting/account/commands.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/account/converters.py` & `mia-accounting-1.5.0/src/accounting/account/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/account/forms.py` & `mia-accounting-1.5.0/src/accounting/account/forms.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/account/queries.py` & `mia-accounting-1.5.0/src/accounting/account/queries.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/account/views.py` & `mia-accounting-1.5.0/src/accounting/account/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/base_account/__init__.py` & `mia-accounting-1.5.0/src/accounting/base_account/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/base_account/commands.py` & `mia-accounting-1.5.0/src/accounting/base_account/commands.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/base_account/converters.py` & `mia-accounting-1.5.0/src/accounting/base_account/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/base_account/queries.py` & `mia-accounting-1.5.0/src/accounting/base_account/queries.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/base_account/views.py` & `mia-accounting-1.5.0/src/accounting/base_account/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/commands.py` & `mia-accounting-1.5.0/src/accounting/commands.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/currency/__init__.py` & `mia-accounting-1.5.0/src/accounting/currency/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/currency/commands.py` & `mia-accounting-1.5.0/src/accounting/currency/commands.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/currency/converters.py` & `mia-accounting-1.5.0/src/accounting/currency/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/currency/forms.py` & `mia-accounting-1.5.0/src/accounting/currency/forms.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/currency/queries.py` & `mia-accounting-1.5.0/src/accounting/currency/queries.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/currency/views.py` & `mia-accounting-1.5.0/src/accounting/currency/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/data/base_accounts.csv` & `mia-accounting-1.5.0/src/accounting/data/base_accounts.csv`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/forms.py` & `mia-accounting-1.5.0/src/accounting/forms.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/journal_entry/__init__.py` & `mia-accounting-1.5.0/src/accounting/journal_entry/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/journal_entry/converters.py` & `mia-accounting-1.5.0/src/accounting/journal_entry/converters.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,16 @@
 
     def to_python(self, value: str) -> JournalEntry:
         """Converts a journal entry ID to a journal entry.
 
         :param value: The journal entry ID.
         :return: The corresponding journal entry.
         """
-        journal_entry: JournalEntry | None = db.session.get(JournalEntry, value)
+        journal_entry: JournalEntry | None \
+            = db.session.get(JournalEntry, value)
         if journal_entry is None:
             abort(404)
         return journal_entry
 
     def to_url(self, value: JournalEntry) -> str:
         """Converts a journal entry to its ID.
```

### Comparing `mia-accounting-1.4.1/src/accounting/journal_entry/forms/__init__.py` & `mia-accounting-1.5.0/src/accounting/journal_entry/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/journal_entry/forms/currency.py` & `mia-accounting-1.5.0/src/accounting/journal_entry/forms/currency.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,14 @@
     BooleanField, FormField
 from wtforms.validators import DataRequired
 
 from accounting import db
 from accounting.forms import CurrencyExists
 from accounting.locale import lazy_gettext
 from accounting.models import JournalEntryLineItem
-from accounting.utils.cast import be
 from accounting.utils.offset_alias import offset_alias
 from accounting.utils.strip_text import strip_text
 from .line_item import LineItemForm, CreditLineItemForm, DebitLineItemForm
 
 CURRENCY_REQUIRED: DataRequired = DataRequired(
     lazy_gettext("Please select the currency."))
 """The validator to check if the currency code is empty."""
@@ -71,16 +70,16 @@
     def __call__(self, form: FlaskForm, field: StringField) -> None:
         assert isinstance(form, CurrencyForm)
         if field.data is None:
             return
         offset: sa.Alias = offset_alias()
         original_line_items: list[JournalEntryLineItem]\
             = JournalEntryLineItem.query\
-            .join(offset, be(JournalEntryLineItem.id
-                             == offset.c.original_line_item_id),
+            .join(offset,
+                  JournalEntryLineItem.id == offset.c.original_line_item_id,
                   isouter=True)\
             .filter(JournalEntryLineItem.id
                     .in_({x.id.data for x in form.line_items
                           if x.id.data is not None}))\
             .group_by(JournalEntryLineItem.id,
                       JournalEntryLineItem.currency_code)\
             .having(sa.func.count(offset.c.id) > 0).all()
```

### Comparing `mia-accounting-1.4.1/src/accounting/journal_entry/forms/journal_entry.py` & `mia-accounting-1.5.0/src/accounting/journal_entry/forms/journal_entry.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/journal_entry/forms/line_item.py` & `mia-accounting-1.5.0/src/accounting/journal_entry/forms/line_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 
 from accounting import db
 from accounting.forms import ACCOUNT_REQUIRED, AccountExists, IsDebitAccount, \
     IsCreditAccount
 from accounting.locale import lazy_gettext
 from accounting.models import Account, JournalEntry, JournalEntryLineItem
 from accounting.template_filters import format_amount
-from accounting.utils.cast import be
 from accounting.utils.random_id import new_id
 from accounting.utils.strip_text import strip_text
 from accounting.utils.user import get_current_user_pk
 
 
 class OriginalLineItemExists:
     """The validator to check if the original line item exists."""
@@ -194,21 +193,21 @@
             return
         is_debit: bool = isinstance(form, DebitLineItemForm)
         existing_line_item_id: set[int] = set()
         if form.journal_entry_form.obj is not None:
             existing_line_item_id \
                 = {x.id for x in form.journal_entry_form.obj.line_items}
         offset_total_func: sa.Function = sa.func.sum(sa.case(
-            (be(JournalEntryLineItem.is_debit == is_debit),
+            (JournalEntryLineItem.is_debit == is_debit,
              JournalEntryLineItem.amount),
             else_=-JournalEntryLineItem.amount))
         offset_total_but_form: Decimal | None = db.session.scalar(
             sa.select(offset_total_func)
-            .filter(be(JournalEntryLineItem.original_line_item_id
-                       == original_line_item.id),
+            .filter(JournalEntryLineItem.original_line_item_id
+                    == original_line_item.id,
                     JournalEntryLineItem.id.not_in(existing_line_item_id)))
         if offset_total_but_form is None:
             offset_total_but_form = Decimal("0")
         offset_total_on_form: Decimal = sum(
             [x.amount.data for x in form.journal_entry_form.line_items
              if x.original_line_item_id.data == original_line_item.id
              and x.amount != field and x.amount.data is not None])
@@ -228,16 +227,15 @@
         if field.data is None or form.id.data is None:
             return
         is_debit: bool = isinstance(form, DebitLineItemForm)
         select_offset_total: sa.Select = sa.select(sa.func.sum(sa.case(
             (JournalEntryLineItem.is_debit != is_debit,
              JournalEntryLineItem.amount),
             else_=-JournalEntryLineItem.amount)))\
-            .filter(be(JournalEntryLineItem.original_line_item_id
-                       == form.id.data))
+            .filter(JournalEntryLineItem.original_line_item_id == form.id.data)
         offset_total: Decimal | None = db.session.scalar(select_offset_total)
         if offset_total is not None and field.data < offset_total:
             raise ValidationError(lazy_gettext(
                 "The amount must not be less than the offset total %(total)s.",
                 total=format_amount(offset_total)))
```

### Comparing `mia-accounting-1.4.1/src/accounting/journal_entry/forms/reorder.py` & `mia-accounting-1.5.0/src/accounting/journal_entry/forms/reorder.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/journal_entry/template_filters.py` & `mia-accounting-1.5.0/src/accounting/journal_entry/template_filters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/journal_entry/utils/__init__.py` & `mia-accounting-1.5.0/src/accounting/journal_entry/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/journal_entry/utils/account_option.py` & `mia-accounting-1.5.0/src/accounting/journal_entry/utils/account_option.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/journal_entry/utils/description_editor.py` & `mia-accounting-1.5.0/src/accounting/journal_entry/utils/description_editor.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/journal_entry/utils/operators.py` & `mia-accounting-1.5.0/src/accounting/journal_entry/utils/operators.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/journal_entry/utils/original_line_items.py` & `mia-accounting-1.5.0/src/accounting/journal_entry/utils/original_line_items.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 from decimal import Decimal
 
 import sqlalchemy as sa
 from sqlalchemy.orm import selectinload
 
 from accounting import db
 from accounting.models import Account, JournalEntry, JournalEntryLineItem
-from accounting.utils.cast import be
 from accounting.utils.offset_alias import offset_alias
 
 
 def get_selectable_original_line_items(
         line_item_id_on_form: set[int], is_payable: bool,
         is_receivable: bool) -> list[JournalEntryLineItem]:
     """Queries and returns the selectable original line items, with their net
@@ -41,31 +40,30 @@
         False otherwise.
     :return: The selectable original line items, with their net balances.
     """
     assert is_payable or is_receivable
     offset: sa.Alias = offset_alias()
     net_balance: sa.Label = (JournalEntryLineItem.amount + sa.func.sum(sa.case(
         (offset.c.id.in_(line_item_id_on_form), 0),
-        (be(offset.c.is_debit == JournalEntryLineItem.is_debit),
-         offset.c.amount),
+        (offset.c.is_debit == JournalEntryLineItem.is_debit, offset.c.amount),
         else_=-offset.c.amount))).label("net_balance")
     conditions: list[sa.BinaryExpression] = [Account.is_need_offset]
     sub_conditions: list[sa.BinaryExpression] = []
     if is_payable:
         sub_conditions.append(sa.and_(Account.base_code.startswith("2"),
                                       sa.not_(JournalEntryLineItem.is_debit)))
     if is_receivable:
         sub_conditions.append(sa.and_(Account.base_code.startswith("1"),
                                       JournalEntryLineItem.is_debit))
     conditions.append(sa.or_(*sub_conditions))
     select_net_balances: sa.Select \
         = sa.select(JournalEntryLineItem.id, net_balance)\
         .join(Account)\
-        .join(offset, be(JournalEntryLineItem.id
-                         == offset.c.original_line_item_id),
+        .join(offset,
+              JournalEntryLineItem.id == offset.c.original_line_item_id,
               isouter=True)\
         .filter(*conditions)\
         .group_by(JournalEntryLineItem.id)\
         .having(sa.or_(sa.func.count(offset.c.id) == 0, net_balance != 0))
     net_balances: dict[int, Decimal] \
         = {x.id: x.net_balance
            for x in db.session.execute(select_net_balances).all()}
```

### Comparing `mia-accounting-1.4.1/src/accounting/journal_entry/views.py` & `mia-accounting-1.5.0/src/accounting/journal_entry/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/locale.py` & `mia-accounting-1.5.0/src/accounting/locale.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/models.py` & `mia-accounting-1.5.0/src/accounting/models.py`

 * *Files 25% similar despite different names*

```diff
@@ -15,40 +15,42 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """The data models.
 
 """
 from __future__ import annotations
 
+import datetime as dt
 import re
 import typing as t
 from decimal import Decimal
 
 import sqlalchemy as sa
 from babel import Locale
 from flask_babel import get_locale, get_babel
 from sqlalchemy import text
+from sqlalchemy.orm import Mapped, mapped_column
 
 from accounting import db
 from accounting.locale import gettext
 from accounting.utils.user import user_cls, user_pk_column
 
 
 class BaseAccount(db.Model):
     """A base account."""
     __tablename__ = "accounting_base_accounts"
     """The table name."""
-    code = db.Column(db.String, nullable=False, primary_key=True)
+    code: Mapped[str] = mapped_column(primary_key=True)
     """The code."""
-    title_l10n = db.Column("title", db.String, nullable=False)
+    title_l10n: Mapped[str] = mapped_column("title")
     """The title."""
-    l10n = db.relationship("BaseAccountL10n", back_populates="account",
-                           lazy=False)
+    l10n: Mapped[list[BaseAccountL10n]] \
+        = db.relationship(back_populates="account", lazy=False)
     """The localized titles."""
-    accounts = db.relationship("Account", back_populates="base")
+    accounts: Mapped[list[Account]] = db.relationship(back_populates="base")
     """The descendant accounts under the base account."""
 
     def __str__(self) -> str:
         """Returns the string representation of the base account.
 
         :return: The string representation of the base account.
         """
@@ -77,73 +79,68 @@
         return [self.code, self.title_l10n] + [x.title for x in self.l10n]
 
 
 class BaseAccountL10n(db.Model):
     """A localized base account title."""
     __tablename__ = "accounting_base_accounts_l10n"
     """The table name."""
-    account_code = db.Column(db.String,
-                             db.ForeignKey(BaseAccount.code,
-                                           onupdate="CASCADE",
-                                           ondelete="CASCADE"),
-                             nullable=False, primary_key=True)
+    account_code: Mapped[str] \
+        = mapped_column(db.ForeignKey(BaseAccount.code, onupdate="CASCADE",
+                                      ondelete="CASCADE"),
+                        primary_key=True)
     """The code of the account."""
-    account = db.relationship(BaseAccount, back_populates="l10n")
+    account: Mapped[BaseAccount] = db.relationship(back_populates="l10n")
     """The account."""
-    locale = db.Column(db.String, nullable=False, primary_key=True)
+    locale: Mapped[str] = mapped_column(primary_key=True)
     """The locale."""
-    title = db.Column(db.String, nullable=False)
+    title: Mapped[str]
     """The localized title."""
 
 
 class Account(db.Model):
     """An account."""
     __tablename__ = "accounting_accounts"
     """The table name."""
-    id = db.Column(db.Integer, nullable=False, primary_key=True,
-                   autoincrement=False)
+    id: Mapped[int] = mapped_column(primary_key=True, autoincrement=False)
     """The account ID."""
-    base_code = db.Column(db.String,
-                          db.ForeignKey(BaseAccount.code, onupdate="CASCADE",
-                                        ondelete="CASCADE"),
-                          nullable=False)
+    base_code: Mapped[str] \
+        = mapped_column(db.ForeignKey(BaseAccount.code, onupdate="CASCADE",
+                                      ondelete="CASCADE"))
     """The code of the base account."""
-    base = db.relationship(BaseAccount, back_populates="accounts")
+    base: Mapped[BaseAccount] = db.relationship(back_populates="accounts")
     """The base account."""
-    no = db.Column(db.Integer, nullable=False, default=text("1"))
+    no: Mapped[int] = mapped_column(default=text("1"))
     """The account number under the base account."""
-    title_l10n = db.Column("title", db.String, nullable=False)
+    title_l10n: Mapped[str] = mapped_column("title")
     """The title."""
-    is_need_offset = db.Column(db.Boolean, nullable=False, default=False)
+    is_need_offset: Mapped[bool] = mapped_column(default=False)
     """Whether the journal entry line items of this account need offset."""
-    created_at = db.Column(db.DateTime(timezone=True), nullable=False,
-                           server_default=db.func.now())
+    created_at: Mapped[dt.datetime] \
+        = mapped_column(db.DateTime(timezone=True),
+                        server_default=db.func.now())
     """The time of creation."""
-    created_by_id = db.Column(db.Integer,
-                              db.ForeignKey(user_pk_column,
-                                            onupdate="CASCADE"),
-                              nullable=False)
+    created_by_id: Mapped[int] \
+        = mapped_column(db.ForeignKey(user_pk_column, onupdate="CASCADE"))
     """The ID of the creator."""
-    created_by = db.relationship(user_cls, foreign_keys=created_by_id)
+    created_by: Mapped[user_cls] = db.relationship(foreign_keys=created_by_id)
     """The creator."""
-    updated_at = db.Column(db.DateTime(timezone=True), nullable=False,
-                           server_default=db.func.now())
+    updated_at: Mapped[dt.datetime] \
+        = mapped_column(db.DateTime(timezone=True),
+                        server_default=db.func.now())
     """The time of last update."""
-    updated_by_id = db.Column(db.Integer,
-                              db.ForeignKey(user_pk_column,
-                                            onupdate="CASCADE"),
-                              nullable=False)
+    updated_by_id: Mapped[int] \
+        = mapped_column(db.ForeignKey(user_pk_column, onupdate="CASCADE"))
     """The ID of the updator."""
-    updated_by = db.relationship(user_cls, foreign_keys=updated_by_id)
+    updated_by: Mapped[user_cls] = db.relationship(foreign_keys=updated_by_id)
     """The updator."""
-    l10n = db.relationship("AccountL10n", back_populates="account",
-                           lazy=False)
+    l10n: Mapped[list[AccountL10n]] \
+        = db.relationship(back_populates="account", lazy=False)
     """The localized titles."""
-    line_items = db.relationship("JournalEntryLineItem",
-                                 back_populates="account")
+    line_items: Mapped[list[JournalEntryLineItem]] \
+        = db.relationship(back_populates="account")
     """The journal entry line items."""
 
     CASH_CODE: str = "1111-001"
     """The code of the cash account,"""
     ACCUMULATED_CHANGE_CODE: str = "3351-001"
     """The code of the accumulated-change account,"""
     NET_CHANGE_CODE: str = "3353-001"
@@ -348,60 +345,59 @@
         return cls.find_by_code(cls.ACCUMULATED_CHANGE_CODE)
 
 
 class AccountL10n(db.Model):
     """A localized account title."""
     __tablename__ = "accounting_accounts_l10n"
     """The table name."""
-    account_id = db.Column(db.Integer,
-                           db.ForeignKey(Account.id, onupdate="CASCADE",
-                                         ondelete="CASCADE"),
-                           nullable=False, primary_key=True)
+    account_id: Mapped[int] \
+        = mapped_column(db.ForeignKey(Account.id, onupdate="CASCADE",
+                                      ondelete="CASCADE"),
+                        primary_key=True)
     """The account ID."""
-    account = db.relationship(Account, back_populates="l10n")
+    account: Mapped[Account] = db.relationship(back_populates="l10n")
     """The account."""
-    locale = db.Column(db.String, nullable=False, primary_key=True)
+    locale: Mapped[str] = mapped_column(primary_key=True)
     """The locale."""
-    title = db.Column(db.String, nullable=False)
+    title: Mapped[str]
     """The localized title."""
 
 
 class Currency(db.Model):
     """A currency."""
     __tablename__ = "accounting_currencies"
     """The table name."""
-    code = db.Column(db.String, nullable=False, primary_key=True)
+    code: Mapped[str] = mapped_column(primary_key=True)
     """The code."""
-    name_l10n = db.Column("name", db.String, nullable=False)
+    name_l10n: Mapped[str] = mapped_column("name")
     """The name."""
-    created_at = db.Column(db.DateTime(timezone=True), nullable=False,
-                           server_default=db.func.now())
+    created_at: Mapped[dt.datetime] \
+        = mapped_column(db.DateTime(timezone=True),
+                        server_default=db.func.now())
     """The time of creation."""
-    created_by_id = db.Column(db.Integer,
-                              db.ForeignKey(user_pk_column,
-                                            onupdate="CASCADE"),
-                              nullable=False)
+    created_by_id: Mapped[int] \
+        = mapped_column(db.ForeignKey(user_pk_column, onupdate="CASCADE"))
     """The ID of the creator."""
-    created_by = db.relationship(user_cls, foreign_keys=created_by_id)
+    created_by: Mapped[user_cls] = db.relationship(foreign_keys=created_by_id)
     """The creator."""
-    updated_at = db.Column(db.DateTime(timezone=True), nullable=False,
-                           server_default=db.func.now())
+    updated_at: Mapped[dt.datetime] \
+        = mapped_column(db.DateTime(timezone=True),
+                        server_default=db.func.now())
     """The time of last update."""
-    updated_by_id = db.Column(db.Integer,
-                              db.ForeignKey(user_pk_column,
-                                            onupdate="CASCADE"),
-                              nullable=False)
+    updated_by_id: Mapped[int] \
+        = mapped_column(db.ForeignKey(user_pk_column, onupdate="CASCADE"))
     """The ID of the updator."""
-    updated_by = db.relationship(user_cls, foreign_keys=updated_by_id)
+    updated_by: Mapped[user_cls] \
+        = db.relationship(foreign_keys=updated_by_id)
     """The updator."""
-    l10n = db.relationship("CurrencyL10n", back_populates="currency",
-                           lazy=False)
+    l10n: Mapped[list[CurrencyL10n]] \
+        = db.relationship(back_populates="currency", lazy=False)
     """The localized names."""
-    line_items = db.relationship("JournalEntryLineItem",
-                                 back_populates="currency")
+    line_items: Mapped[list[JournalEntryLineItem]] \
+        = db.relationship(back_populates="currency")
     """The journal entry line items."""
 
     def __str__(self) -> str:
         """Returns the string representation of the currency.
 
         :return: The string representation of the currency.
         """
@@ -475,24 +471,24 @@
         cls.query.filter(cls.code == self.code).delete()
 
 
 class CurrencyL10n(db.Model):
     """A localized currency name."""
     __tablename__ = "accounting_currencies_l10n"
     """The table name."""
-    currency_code = db.Column(db.String,
-                              db.ForeignKey(Currency.code, onupdate="CASCADE",
-                                            ondelete="CASCADE"),
-                              nullable=False, primary_key=True)
+    currency_code: Mapped[str] \
+        = mapped_column(db.ForeignKey(Currency.code, onupdate="CASCADE",
+                                      ondelete="CASCADE"),
+                        primary_key=True)
     """The currency code."""
-    currency = db.relationship(Currency, back_populates="l10n")
+    currency: Mapped[Currency] = db.relationship(back_populates="l10n")
     """The currency."""
-    locale = db.Column(db.String, nullable=False, primary_key=True)
+    locale: Mapped[str] = mapped_column(primary_key=True)
     """The locale."""
-    name = db.Column(db.String, nullable=False)
+    name: Mapped[str]
     """The localized name."""
 
 
 class JournalEntryCurrency:
     """A currency in a journal entry."""
 
     def __init__(self, code: str, debit: list[JournalEntryLineItem],
@@ -535,45 +531,42 @@
         return sum([x.amount for x in self.credit])
 
 
 class JournalEntry(db.Model):
     """A journal entry."""
     __tablename__ = "accounting_journal_entries"
     """The table name."""
-    id = db.Column(db.Integer, nullable=False, primary_key=True,
-                   autoincrement=False)
+    id: Mapped[int] = mapped_column(primary_key=True, autoincrement=False)
     """The journal entry ID."""
-    date = db.Column(db.Date, nullable=False)
+    date: Mapped[dt.date]
     """The date."""
-    no = db.Column(db.Integer, nullable=False, default=text("1"))
+    no: Mapped[int] = mapped_column(default=text("1"))
     """The account number under the date."""
-    note = db.Column(db.String)
+    note: Mapped[str | None]
     """The note."""
-    created_at = db.Column(db.DateTime(timezone=True), nullable=False,
-                           server_default=db.func.now())
+    created_at: Mapped[dt.datetime] \
+        = mapped_column(db.DateTime(timezone=True),
+                        server_default=db.func.now())
     """The time of creation."""
-    created_by_id = db.Column(db.Integer,
-                              db.ForeignKey(user_pk_column,
-                                            onupdate="CASCADE"),
-                              nullable=False)
+    created_by_id: Mapped[int] \
+        = mapped_column(db.ForeignKey(user_pk_column, onupdate="CASCADE"))
     """The ID of the creator."""
-    created_by = db.relationship(user_cls, foreign_keys=created_by_id)
+    created_by: Mapped[user_cls] = db.relationship(foreign_keys=created_by_id)
     """The creator."""
-    updated_at = db.Column(db.DateTime(timezone=True), nullable=False,
-                           server_default=db.func.now())
+    updated_at: Mapped[dt.datetime] \
+        = mapped_column(db.DateTime(timezone=True),
+                        server_default=db.func.now())
     """The time of last update."""
-    updated_by_id = db.Column(db.Integer,
-                              db.ForeignKey(user_pk_column,
-                                            onupdate="CASCADE"),
-                              nullable=False)
+    updated_by_id: Mapped[int] \
+        = mapped_column(db.ForeignKey(user_pk_column, onupdate="CASCADE"))
     """The ID of the updator."""
-    updated_by = db.relationship(user_cls, foreign_keys=updated_by_id)
+    updated_by: Mapped[user_cls] = db.relationship(foreign_keys=updated_by_id)
     """The updator."""
-    line_items = db.relationship("JournalEntryLineItem",
-                                 back_populates="journal_entry")
+    line_items: Mapped[list[JournalEntryLineItem]] \
+        = db.relationship(back_populates="journal_entry")
     """The line items."""
 
     def __str__(self) -> str:
         """Returns the string representation of this journal entry.
 
         :return: The string representation of this journal entry.
         """
@@ -655,52 +648,47 @@
         db.session.delete(self)
 
 
 class JournalEntryLineItem(db.Model):
     """A line item in the journal entry."""
     __tablename__ = "accounting_journal_entry_line_items"
     """The table name."""
-    id = db.Column(db.Integer, nullable=False, primary_key=True,
-                   autoincrement=False)
+    id: Mapped[int] = mapped_column(primary_key=True, autoincrement=False)
     """The line item ID."""
-    journal_entry_id = db.Column(db.Integer,
-                                 db.ForeignKey(JournalEntry.id,
-                                               onupdate="CASCADE",
-                                               ondelete="CASCADE"),
-                                 nullable=False)
+    journal_entry_id: Mapped[int] \
+        = mapped_column(db.ForeignKey(JournalEntry.id, onupdate="CASCADE",
+                                      ondelete="CASCADE"))
     """The journal entry ID."""
-    journal_entry = db.relationship(JournalEntry, back_populates="line_items")
+    journal_entry: Mapped[JournalEntry] \
+        = db.relationship(back_populates="line_items")
     """The journal entry."""
-    is_debit = db.Column(db.Boolean, nullable=False)
+    is_debit: Mapped[bool]
     """True for a debit line item, or False for a credit line item."""
-    no = db.Column(db.Integer, nullable=False)
+    no: Mapped[int]
     """The line item number under the journal entry and debit or credit."""
-    original_line_item_id = db.Column(db.Integer,
-                                      db.ForeignKey(id, onupdate="CASCADE"),
-                                      nullable=True)
+    original_line_item_id: Mapped[int | None] \
+        = mapped_column(db.ForeignKey(id, onupdate="CASCADE"))
     """The ID of the original line item."""
-    original_line_item = db.relationship("JournalEntryLineItem",
-                                         remote_side=id, passive_deletes=True)
+    original_line_item: Mapped[JournalEntryLineItem | None] \
+        = db.relationship(remote_side=id, passive_deletes=True)
     """The original line item."""
-    currency_code = db.Column(db.String,
-                              db.ForeignKey(Currency.code, onupdate="CASCADE"),
-                              nullable=False)
+    currency_code: Mapped[str] \
+        = mapped_column(db.ForeignKey(Currency.code, onupdate="CASCADE"))
     """The currency code."""
-    currency = db.relationship(Currency, back_populates="line_items")
+    currency: Mapped[Currency] = db.relationship(back_populates="line_items")
     """The currency."""
-    account_id = db.Column(db.Integer,
-                           db.ForeignKey(Account.id,
-                                         onupdate="CASCADE"),
-                           nullable=False)
+    account_id: Mapped[int] \
+        = mapped_column(db.ForeignKey(Account.id, onupdate="CASCADE"))
     """The account ID."""
-    account = db.relationship(Account, back_populates="line_items", lazy=False)
+    account: Mapped[Account] \
+        = db.relationship(back_populates="line_items", lazy=False)
     """The account."""
-    description = db.Column(db.String, nullable=True)
+    description: Mapped[str | None]
     """The description."""
-    amount = db.Column(db.Numeric(14, 2), nullable=False)
+    amount: Mapped[Decimal] = mapped_column(db.Numeric(14, 2))
     """The amount."""
 
     def __str__(self) -> str:
         """Returns the string representation of the line item.
 
         :return: The string representation of the line item.
         """
@@ -887,31 +875,29 @@
                 format_amount(self.amount)]
 
 
 class Option(db.Model):
     """An option."""
     __tablename__ = "accounting_options"
     """The table name."""
-    name = db.Column(db.String, nullable=False, primary_key=True)
+    name: Mapped[str] = mapped_column(primary_key=True)
     """The name."""
-    value = db.Column(db.Text, nullable=False)
+    value: Mapped[str] = mapped_column(db.Text)
     """The option value."""
-    created_at = db.Column(db.DateTime(timezone=True), nullable=False,
-                           server_default=db.func.now())
+    created_at: Mapped[dt.datetime] \
+        = mapped_column(db.DateTime(timezone=True),
+                        server_default=db.func.now())
     """The time of creation."""
-    created_by_id = db.Column(db.Integer,
-                              db.ForeignKey(user_pk_column,
-                                            onupdate="CASCADE"),
-                              nullable=False)
+    created_by_id: Mapped[int] \
+        = mapped_column(db.ForeignKey(user_pk_column, onupdate="CASCADE"))
     """The ID of the creator."""
-    created_by = db.relationship(user_cls, foreign_keys=created_by_id)
+    created_by: Mapped[user_cls] = db.relationship(foreign_keys=created_by_id)
     """The creator."""
-    updated_at = db.Column(db.DateTime(timezone=True), nullable=False,
-                           server_default=db.func.now())
+    updated_at: Mapped[dt.datetime] \
+        = mapped_column(db.DateTime(timezone=True),
+                        server_default=db.func.now())
     """The time of last update."""
-    updated_by_id = db.Column(db.Integer,
-                              db.ForeignKey(user_pk_column,
-                                            onupdate="CASCADE"),
-                              nullable=False)
+    updated_by_id: Mapped[int] \
+        = mapped_column(db.ForeignKey(user_pk_column, onupdate="CASCADE"))
     """The ID of the updator."""
-    updated_by = db.relationship(user_cls, foreign_keys=updated_by_id)
+    updated_by: Mapped[user_cls] = db.relationship(foreign_keys=updated_by_id)
     """The updator."""
```

### Comparing `mia-accounting-1.4.1/src/accounting/option/__init__.py` & `mia-accounting-1.5.0/src/accounting/option/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/option/forms.py` & `mia-accounting-1.5.0/src/accounting/option/forms.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/option/views.py` & `mia-accounting-1.5.0/src/accounting/option/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/report/__init__.py` & `mia-accounting-1.5.0/src/accounting/report/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/report/converters.py` & `mia-accounting-1.5.0/src/accounting/report/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/report/period/__init__.py` & `mia-accounting-1.5.0/src/accounting/report/period/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/report/period/chooser.py` & `mia-accounting-1.5.0/src/accounting/report/period/chooser.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/report/period/description.py` & `mia-accounting-1.5.0/src/accounting/report/period/description.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/report/period/month_end.py` & `mia-accounting-1.5.0/src/accounting/report/period/month_end.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/report/period/parser.py` & `mia-accounting-1.5.0/src/accounting/report/period/parser.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/report/period/period.py` & `mia-accounting-1.5.0/src/accounting/report/period/period.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/report/period/shortcuts.py` & `mia-accounting-1.5.0/src/accounting/report/period/shortcuts.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/report/period/specification.py` & `mia-accounting-1.5.0/src/accounting/report/period/specification.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/report/reports/__init__.py` & `mia-accounting-1.5.0/src/accounting/report/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/report/reports/balance_sheet.py` & `mia-accounting-1.5.0/src/accounting/report/reports/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/report/reports/income_expenses.py` & `mia-accounting-1.5.0/src/accounting/report/reports/income_expenses.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 from accounting.report.utils.base_report import BaseReport
 from accounting.report.utils.csv_export import BaseCSVRow, csv_download, \
     period_spec
 from accounting.report.utils.option_link import OptionLink
 from accounting.report.utils.report_chooser import ReportChooser
 from accounting.report.utils.report_type import ReportType
 from accounting.report.utils.urls import income_expenses_url
-from accounting.utils.cast import be
 from accounting.utils.current_account import CurrentAccount
 from accounting.utils.pagination import Pagination
 
 
 class ReportLineItem:
     """A line item in the report."""
 
@@ -118,16 +117,15 @@
         if self.__period.start is None:
             return None
         balance_func: sa.Function = sa.func.sum(sa.case(
             (JournalEntryLineItem.is_debit, JournalEntryLineItem.amount),
             else_=-JournalEntryLineItem.amount))
         select: sa.Select = sa.Select(balance_func)\
             .join(JournalEntry).join(Account)\
-            .filter(be(JournalEntryLineItem.currency_code
-                       == self.__currency.code),
+            .filter(JournalEntryLineItem.currency_code == self.__currency.code,
                     self.__account_condition,
                     JournalEntry.date < self.__period.start)
         balance: int | None = db.session.scalar(select)
         if balance is None:
             return None
         line_item: ReportLineItem = ReportLineItem()
         line_item.is_brought_forward = True
@@ -343,16 +341,15 @@
         options: list[OptionLink] \
             = [OptionLink(str(current_al),
                           income_expenses_url(self.currency, current_al,
                                               self.period),
                           self.account.id == 0)]
         in_use: sa.Select = sa.Select(JournalEntryLineItem.account_id)\
             .join(Account)\
-            .filter(be(JournalEntryLineItem.currency_code
-                       == self.currency.code),
+            .filter(JournalEntryLineItem.currency_code == self.currency.code,
                     CurrentAccount.sql_condition())\
             .group_by(JournalEntryLineItem.account_id)
         options.extend([OptionLink(str(x),
                                    income_expenses_url(
                                        self.currency,
                                        CurrentAccount(x),
                                        self.period),
```

### Comparing `mia-accounting-1.4.1/src/accounting/report/reports/income_statement.py` & `mia-accounting-1.5.0/src/accounting/report/reports/income_statement.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/report/reports/journal.py` & `mia-accounting-1.5.0/src/accounting/report/reports/journal.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/report/reports/ledger.py` & `mia-accounting-1.5.0/src/accounting/report/reports/ledger.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 from accounting.report.utils.base_report import BaseReport
 from accounting.report.utils.csv_export import BaseCSVRow, csv_download, \
     period_spec
 from accounting.report.utils.option_link import OptionLink
 from accounting.report.utils.report_chooser import ReportChooser
 from accounting.report.utils.report_type import ReportType
 from accounting.report.utils.urls import ledger_url
-from accounting.utils.cast import be
 from accounting.utils.pagination import Pagination
 
 
 class ReportLineItem:
     """A line item in the report."""
 
     def __init__(self, line_item: JournalEntryLineItem | None = None):
@@ -114,18 +113,16 @@
             return None
         if self.__account.is_nominal:
             return None
         balance_func: sa.Function = sa.func.sum(sa.case(
             (JournalEntryLineItem.is_debit, JournalEntryLineItem.amount),
             else_=-JournalEntryLineItem.amount))
         select: sa.Select = sa.Select(balance_func).join(JournalEntry)\
-            .filter(be(JournalEntryLineItem.currency_code
-                       == self.__currency.code),
-                    be(JournalEntryLineItem.account_id
-                       == self.__account.id),
+            .filter(JournalEntryLineItem.currency_code == self.__currency.code,
+                    JournalEntryLineItem.account_id == self.__account.id,
                     JournalEntry.date < self.__period.start)
         balance: int | None = db.session.scalar(select)
         if balance is None:
             return None
         line_item: ReportLineItem = ReportLineItem()
         line_item.is_brought_forward = True
         line_item.date = self.__period.start
@@ -309,16 +306,15 @@
     @property
     def account_options(self) -> list[OptionLink]:
         """Returns the account options.
 
         :return: The account options.
         """
         in_use: sa.Select = sa.Select(JournalEntryLineItem.account_id)\
-            .filter(be(JournalEntryLineItem.currency_code
-                       == self.currency.code))\
+            .filter(JournalEntryLineItem.currency_code == self.currency.code)\
             .group_by(JournalEntryLineItem.account_id)
         return [OptionLink(str(x), ledger_url(self.currency, x, self.period),
                            x.id == self.account.id)
                 for x in Account.query.filter(Account.id.in_(in_use))
                 .order_by(Account.base_code, Account.no).all()]
```

### Comparing `mia-accounting-1.4.1/src/accounting/report/reports/search.py` & `mia-accounting-1.5.0/src/accounting/report/reports/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 from accounting.models import Currency, CurrencyL10n, Account, AccountL10n, \
     JournalEntry, JournalEntryLineItem
 from accounting.report.utils.base_page_params import BasePageParams
 from accounting.report.utils.base_report import BaseReport
 from accounting.report.utils.csv_export import csv_download
 from accounting.report.utils.report_chooser import ReportChooser
 from accounting.report.utils.report_type import ReportType
-from accounting.utils.cast import be
 from accounting.utils.pagination import Pagination
 from accounting.utils.query import parse_query_keywords
 from .journal import get_csv_rows
 
 
 class LineItemCollector:
     """The line item collector."""
@@ -124,17 +123,16 @@
         :return: The condition to filter the journal entry.
         """
         conditions: list[sa.BinaryExpression] \
             = [JournalEntry.note.icontains(k)]
         journal_entry_date: datetime
         try:
             journal_entry_date = datetime.strptime(k, "%Y")
-            conditions.append(
-                be(sa.extract("year", JournalEntry.date)
-                   == journal_entry_date.year))
+            conditions.append(sa.extract("year", JournalEntry.date)
+                              == journal_entry_date.year)
         except ValueError:
             pass
         try:
             journal_entry_date = datetime.strptime(k, "%Y/%m")
             conditions.append(sa.and_(
                 sa.extract("year", JournalEntry.date)
                 == journal_entry_date.year,
```

### Comparing `mia-accounting-1.4.1/src/accounting/report/reports/trial_balance.py` & `mia-accounting-1.5.0/src/accounting/report/reports/trial_balance.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/report/reports/unapplied.py` & `mia-accounting-1.5.0/src/accounting/report/reports/unapplied.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/report/reports/unapplied_accounts.py` & `mia-accounting-1.5.0/src/accounting/report/reports/unapplied_accounts.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/report/reports/unmatched.py` & `mia-accounting-1.5.0/src/accounting/report/reports/unmatched.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/report/reports/unmatched_accounts.py` & `mia-accounting-1.5.0/src/accounting/report/reports/unmatched_accounts.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/report/template_filters.py` & `mia-accounting-1.5.0/src/accounting/report/template_filters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/report/utils/__init__.py` & `mia-accounting-1.5.0/src/accounting/report/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/report/utils/base_page_params.py` & `mia-accounting-1.5.0/src/accounting/report/utils/base_page_params.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/report/utils/base_report.py` & `mia-accounting-1.5.0/src/accounting/report/utils/base_report.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/report/utils/csv_export.py` & `mia-accounting-1.5.0/src/accounting/report/utils/csv_export.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/report/utils/offset_matcher.py` & `mia-accounting-1.5.0/src/accounting/report/utils/offset_matcher.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/report/utils/option_link.py` & `mia-accounting-1.5.0/src/accounting/report/utils/option_link.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/report/utils/report_chooser.py` & `mia-accounting-1.5.0/src/accounting/report/utils/report_chooser.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/report/utils/report_type.py` & `mia-accounting-1.5.0/src/accounting/report/utils/report_type.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/report/utils/unapplied.py` & `mia-accounting-1.5.0/src/accounting/report/utils/unapplied.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,39 +20,38 @@
 from decimal import Decimal
 
 import sqlalchemy as sa
 
 from accounting import db
 from accounting.models import Currency, Account, JournalEntry, \
     JournalEntryLineItem
-from accounting.utils.cast import be
 from accounting.utils.offset_alias import offset_alias
 
 
 def get_accounts_with_unapplied(currency: Currency) -> list[Account]:
     """Returns the accounts with unapplied original line items.
 
     :param currency: The currency.
     :return: The accounts with unapplied original line items.
     """
     offset: sa.Alias = offset_alias()
     net_balance: sa.Label \
         = (JournalEntryLineItem.amount
            + sa.func.sum(sa.case(
-                (be(offset.c.is_debit == JournalEntryLineItem.is_debit),
+                (offset.c.is_debit == JournalEntryLineItem.is_debit,
                  offset.c.amount),
                 else_=-offset.c.amount))).label("net_balance")
     select_unapplied: sa.Select \
         = sa.select(JournalEntryLineItem.id)\
         .join(JournalEntry).join(Account)\
-        .join(offset, be(JournalEntryLineItem.id
-                         == offset.c.original_line_item_id),
+        .join(offset,
+              JournalEntryLineItem.id == offset.c.original_line_item_id,
               isouter=True)\
         .filter(Account.is_need_offset,
-                be(JournalEntryLineItem.currency_code == currency.code),
+                JournalEntryLineItem.currency_code == currency.code,
                 sa.or_(sa.and_(Account.base_code.startswith("2"),
                                sa.not_(JournalEntryLineItem.is_debit)),
                        sa.and_(Account.base_code.startswith("1"),
                                JournalEntryLineItem.is_debit)))\
         .group_by(JournalEntryLineItem.id)\
         .having(sa.or_(sa.func.count(offset.c.id) == 0, net_balance != 0))
 
@@ -80,25 +79,25 @@
     :param account: The account.
     :return: The net balances of the unapplied line items of the account.
     """
     offset: sa.Alias = offset_alias()
     net_balance: sa.Label \
         = (JournalEntryLineItem.amount
            + sa.func.sum(sa.case(
-                (be(offset.c.is_debit == JournalEntryLineItem.is_debit),
+                (offset.c.is_debit == JournalEntryLineItem.is_debit,
                  offset.c.amount),
                 else_=-offset.c.amount))).label("net_balance")
     select_net_balances: sa.Select \
         = sa.select(JournalEntryLineItem.id, net_balance) \
         .join(JournalEntry).join(Account) \
-        .join(offset, be(JournalEntryLineItem.id
-                         == offset.c.original_line_item_id),
+        .join(offset,
+              JournalEntryLineItem.id == offset.c.original_line_item_id,
               isouter=True) \
-        .filter(be(Account.id == account.id),
-                be(JournalEntryLineItem.currency_code == currency.code),
+        .filter(Account.id == account.id,
+                JournalEntryLineItem.currency_code == currency.code,
                 sa.or_(sa.and_(Account.base_code.startswith("2"),
                                sa.not_(JournalEntryLineItem.is_debit)),
                        sa.and_(Account.base_code.startswith("1"),
                                JournalEntryLineItem.is_debit))) \
         .group_by(JournalEntryLineItem.id) \
         .having(sa.or_(sa.func.count(offset.c.id) == 0, net_balance != 0))
     return {x.id: x.net_balance
```

### Comparing `mia-accounting-1.4.1/src/accounting/report/utils/unmatched.py` & `mia-accounting-1.5.0/src/accounting/report/utils/unmatched.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 
 """
 import sqlalchemy as sa
 
 from accounting import db
 from accounting.models import Currency, Account, JournalEntry, \
     JournalEntryLineItem
-from accounting.utils.cast import be
 
 
 def get_accounts_with_unmatched(currency: Currency) -> list[Account]:
     """Returns the accounts with unmatched offsets.
 
     :param currency: The currency.
     :return: The accounts with unmatched offsets, with the "count" property set
@@ -34,15 +33,15 @@
     """
     count_func: sa.Label \
         = sa.func.count(JournalEntryLineItem.id).label("count")
     select: sa.Select = sa.select(Account.id, count_func)\
         .select_from(Account)\
         .join(JournalEntryLineItem, isouter=True).join(JournalEntry)\
         .filter(Account.is_need_offset,
-                be(JournalEntryLineItem.currency_code == currency.code),
+                JournalEntryLineItem.currency_code == currency.code,
                 JournalEntryLineItem.original_line_item_id.is_(None),
                 sa.or_(sa.and_(Account.base_code.startswith("2"),
                                JournalEntryLineItem.is_debit),
                        sa.and_(Account.base_code.startswith("1"),
                                sa.not_(JournalEntryLineItem.is_debit))))\
         .group_by(Account.id)\
         .having(count_func > 0)
```

### Comparing `mia-accounting-1.4.1/src/accounting/report/utils/urls.py` & `mia-accounting-1.5.0/src/accounting/report/utils/urls.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/report/views.py` & `mia-accounting-1.5.0/src/accounting/report/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/static/css/style.css` & `mia-accounting-1.5.0/src/accounting/static/css/style.css`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/static/js/account-form.js` & `mia-accounting-1.5.0/src/accounting/static/js/account-form.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/static/js/account-order.js` & `mia-accounting-1.5.0/src/accounting/static/js/account-order.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/static/js/currency-form.js` & `mia-accounting-1.5.0/src/accounting/static/js/currency-form.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/static/js/description-editor.js` & `mia-accounting-1.5.0/src/accounting/static/js/description-editor.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/static/js/drag-and-drop-reorder.js` & `mia-accounting-1.5.0/src/accounting/static/js/drag-and-drop-reorder.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/static/js/journal-entry-account-selector.js` & `mia-accounting-1.5.0/src/accounting/static/js/journal-entry-account-selector.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/static/js/journal-entry-form.js` & `mia-accounting-1.5.0/src/accounting/static/js/journal-entry-form.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/static/js/journal-entry-line-item-editor.js` & `mia-accounting-1.5.0/src/accounting/static/js/journal-entry-line-item-editor.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/static/js/journal-entry-order.js` & `mia-accounting-1.5.0/src/accounting/static/js/journal-entry-order.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/static/js/material-fab-speed-dial.js` & `mia-accounting-1.5.0/src/accounting/static/js/material-fab-speed-dial.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/static/js/option-form.js` & `mia-accounting-1.5.0/src/accounting/static/js/option-form.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/static/js/original-line-item-selector.js` & `mia-accounting-1.5.0/src/accounting/static/js/original-line-item-selector.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/static/js/period-chooser.js` & `mia-accounting-1.5.0/src/accounting/static/js/period-chooser.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/template_filters.py` & `mia-accounting-1.5.0/src/accounting/template_filters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/template_globals.py` & `mia-accounting-1.5.0/src/accounting/template_globals.py`

 * *Files 21% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 """The template globals.
 
 """
 from accounting.models import Currency
 from accounting.utils.options import options
 
 
-def currency_options() -> str:
+def currency_options() -> list[Currency]:
     """Returns the currency options.
 
     :return: The currency options.
     """
     return Currency.query.order_by(Currency.code).all()
```

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/account/create.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/account/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/account/detail.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/account/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/account/edit.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/account/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/account/include/form.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/account/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/account/list.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/account/list.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/account/order.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/account/order.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/base-account/detail.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/base-account/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/base-account/list.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/base-account/list.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/base.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/base.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/currency/create.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/currency/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/currency/detail.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/currency/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/currency/edit.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/currency/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/currency/include/form.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/currency/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/currency/list.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/currency/list.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/include/nav.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/include/nav.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/include/pagination.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/include/pagination.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/disbursement/create.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/disbursement/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/disbursement/detail.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/disbursement/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/disbursement/edit.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/disbursement/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/disbursement/include/form-currency.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/disbursement/include/form-currency.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/disbursement/include/form.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/disbursement/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/include/detail-line-items.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/include/detail-line-items.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/include/detail.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/include/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/include/form-currency.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/include/form-currency.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/include/form-debit-credit.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/include/form-debit-credit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/include/form-line-item.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/include/form-line-item.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/include/form.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/include/order-journal-entry.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/include/order-journal-entry.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/order.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/order.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/receipt/create.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/receipt/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/receipt/detail.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/receipt/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/receipt/edit.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/receipt/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/receipt/include/form-currency.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/receipt/include/form-currency.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/receipt/include/form.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/receipt/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/transfer/create.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/transfer/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/transfer/detail.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/transfer/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/transfer/edit.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/transfer/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/journal-entry/transfer/include/form.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/transfer/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/option/detail.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/option/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/option/form.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/option/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/option/include/form-recurring-expense-income.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/option/include/form-recurring-expense-income.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/option/include/form-recurring-item.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/option/include/form-recurring-item.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/report/balance-sheet.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/report/balance-sheet.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/report/include/add-journal-entry-material-fab.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/report/include/add-journal-entry-material-fab.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/report/include/balance-sheet-section.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/report/include/balance-sheet-section.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/report/include/income-expenses-row-desktop.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/report/include/income-expenses-row-desktop.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/report/include/income-expenses-row-mobile.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/report/include/income-expenses-row-mobile.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/report/include/ledger-row-desktop.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/report/include/ledger-row-desktop.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/report/include/ledger-row-mobile.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/report/include/ledger-row-mobile.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/report/include/period-chooser.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/report/include/period-chooser.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/report/include/search-modal.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/report/include/search-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/report/include/toolbar-buttons.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/report/include/toolbar-buttons.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/report/income-expenses.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/report/income-expenses.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/report/income-statement.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/report/income-statement.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/report/journal.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/report/journal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/report/ledger.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/report/ledger.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/report/search.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/report/search.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/report/trial-balance.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/report/trial-balance.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/report/unapplied-accounts.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/report/unapplied-accounts.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/report/unapplied.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/report/unapplied.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/report/unmatched-accounts.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/report/unmatched-accounts.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/templates/accounting/report/unmatched.html` & `mia-accounting-1.5.0/src/accounting/templates/accounting/report/unmatched.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/translations/accounting.pot` & `mia-accounting-1.5.0/src/accounting/translations/accounting.pot`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.mo` & `mia-accounting-1.5.0/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.mo`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.po` & `mia-accounting-1.5.0/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.po`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.mo` & `mia-accounting-1.5.0/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.mo`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.po` & `mia-accounting-1.5.0/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.po`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/utils/__init__.py` & `mia-accounting-1.5.0/src/accounting/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/utils/cast.py` & `mia-accounting-1.5.0/src/accounting/utils/cast.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,24 +21,14 @@
 
 """
 import typing as t
 
 import sqlalchemy as sa
 
 
-def be(expression: t.Any) -> sa.BinaryExpression:
-    """Casts the SQLAlchemy binary expression to the binary expression type.
-
-    :param expression: The binary expression.
-    :return: The binary expression itself.
-    """
-    assert isinstance(expression, sa.BinaryExpression)
-    return expression
-
-
 def s(message: t.Any) -> str:
     """Casts the LazyString message to the string type.
 
     :param message: The message.
     :return: The binary expression itself.
     """
     return message
```

### Comparing `mia-accounting-1.4.1/src/accounting/utils/current_account.py` & `mia-accounting-1.5.0/src/accounting/utils/current_account.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/utils/flash_errors.py` & `mia-accounting-1.5.0/src/accounting/utils/flash_errors.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/utils/journal_entry_types.py` & `mia-accounting-1.5.0/src/accounting/utils/journal_entry_types.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/utils/next_uri.py` & `mia-accounting-1.5.0/src/accounting/utils/next_uri.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/utils/offset_alias.py` & `mia-accounting-1.5.0/src/accounting/utils/offset_alias.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/utils/options.py` & `mia-accounting-1.5.0/src/accounting/utils/options.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/utils/pagination.py` & `mia-accounting-1.5.0/src/accounting/utils/pagination.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/utils/permission.py` & `mia-accounting-1.5.0/src/accounting/utils/permission.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/utils/query.py` & `mia-accounting-1.5.0/src/accounting/utils/query.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/utils/random_id.py` & `mia-accounting-1.5.0/src/accounting/utils/random_id.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/utils/strip_text.py` & `mia-accounting-1.5.0/src/accounting/utils/strip_text.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/accounting/utils/user.py` & `mia-accounting-1.5.0/src/accounting/utils/user.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/src/mia_accounting.egg-info/SOURCES.txt` & `mia-accounting-1.5.0/src/mia_accounting.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 docs/source/accounting.option.rst
 docs/source/accounting.report.period.rst
 docs/source/accounting.report.reports.rst
 docs/source/accounting.report.rst
 docs/source/accounting.report.utils.rst
 docs/source/accounting.rst
 docs/source/accounting.utils.rst
+docs/source/changelog.rst
 docs/source/conf.py
 docs/source/examples.rst
 docs/source/history.rst
 docs/source/index.rst
 docs/source/intro.rst
 docs/source/modules.rst
 docs/source/_static/.keep
```

### Comparing `mia-accounting-1.4.1/tests/babel-utils-test-site.py` & `mia-accounting-1.5.0/tests/babel-utils-test-site.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/tests/babel-utils.py` & `mia-accounting-1.5.0/tests/babel-utils.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/tests/test_account.py` & `mia-accounting-1.5.0/tests/test_account.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/tests/test_base_account.py` & `mia-accounting-1.5.0/tests/test_base_account.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/tests/test_commands.py` & `mia-accounting-1.5.0/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/tests/test_currency.py` & `mia-accounting-1.5.0/tests/test_currency.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/tests/test_description_editor.py` & `mia-accounting-1.5.0/tests/test_description_editor.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/tests/test_journal_entry.py` & `mia-accounting-1.5.0/tests/test_journal_entry.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/tests/test_offset.py` & `mia-accounting-1.5.0/tests/test_offset.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/tests/test_option.py` & `mia-accounting-1.5.0/tests/test_option.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/tests/test_report.py` & `mia-accounting-1.5.0/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/tests/test_site/__init__.py` & `mia-accounting-1.5.0/tests/test_site/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/tests/test_site/auth.py` & `mia-accounting-1.5.0/tests/test_site/auth.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/tests/test_site/lib.py` & `mia-accounting-1.5.0/tests/test_site/lib.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/tests/test_site/locale.py` & `mia-accounting-1.5.0/tests/test_site/locale.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/tests/test_site/reset.py` & `mia-accounting-1.5.0/tests/test_site/reset.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/tests/test_site/static/favicon.svg` & `mia-accounting-1.5.0/tests/test_site/static/favicon.svg`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/tests/test_site/templates/base.html` & `mia-accounting-1.5.0/tests/test_site/templates/base.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/tests/test_site/templates/home.html` & `mia-accounting-1.5.0/tests/test_site/templates/home.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/tests/test_site/templates/login.html` & `mia-accounting-1.5.0/tests/test_site/templates/login.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/tests/test_site/templates/reset.html` & `mia-accounting-1.5.0/tests/test_site/templates/reset.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/tests/test_site/translations/messages.pot` & `mia-accounting-1.5.0/tests/test_site/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.mo` & `mia-accounting-1.5.0/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.po` & `mia-accounting-1.5.0/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.mo` & `mia-accounting-1.5.0/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.po` & `mia-accounting-1.5.0/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/tests/test_unmatched_offset.py` & `mia-accounting-1.5.0/tests/test_unmatched_offset.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/tests/test_utils.py` & `mia-accounting-1.5.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/tests/testlib.py` & `mia-accounting-1.5.0/tests/testlib.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.4.1/tests/testlib_journal_entry.py` & `mia-accounting-1.5.0/tests/testlib_journal_entry.py`

 * *Files identical despite different names*

