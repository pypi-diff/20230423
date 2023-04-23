# Comparing `tmp/jal-2023.4.7.tar.gz` & `tmp/jal-2023.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jal-2023.4.7.tar", last modified: Fri Apr 21 18:29:44 2023, max compression
+gzip compressed data, was "jal-2023.4.8.tar", last modified: Sun Apr 23 12:20:32 2023, max compression
```

## Comparing `jal-2023.4.7.tar` & `jal-2023.4.8.tar`

### file list

```diff
@@ -1,218 +1,218 @@
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-21 18:29:44.020457 jal-2023.4.7/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      176 2022-01-13 06:08:45.000000 jal-2023.4.7/MANIFEST.in
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2726 2023-04-21 18:29:44.020457 jal-2023.4.7/PKG-INFO
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-21 18:29:43.977123 jal-2023.4.7/docs/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7580 2023-04-15 14:23:01.000000 jal-2023.4.7/docs/README.md
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-21 18:29:43.980456 jal-2023.4.7/jal/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       24 2023-04-21 18:26:09.000000 jal-2023.4.7/jal/__init__.py
--rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     3831 2023-04-15 14:13:28.000000 jal-2023.4.7/jal/constants.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-21 18:29:43.980456 jal-2023.4.7/jal/data_export/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2022-01-13 15:45:51.000000 jal-2023.4.7/jal/data_export/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    19856 2023-04-14 11:26:23.000000 jal-2023.4.7/jal/data_export/dlsg.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-21 18:29:43.983790 jal-2023.4.7/jal/data_export/tax_reports/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.7/jal/data_export/tax_reports/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      990 2023-02-07 18:26:24.000000 jal-2023.4.7/jal/data_export/tax_reports/portugal.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7089 2023-02-08 10:00:47.000000 jal-2023.4.7/jal/data_export/tax_reports/portugal.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1532 2023-02-07 18:26:24.000000 jal-2023.4.7/jal/data_export/tax_reports/russia.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    38366 2023-04-14 11:26:23.000000 jal-2023.4.7/jal/data_export/tax_reports/russia.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6433 2023-02-07 18:26:24.000000 jal-2023.4.7/jal/data_export/taxes.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5299 2023-02-07 18:26:24.000000 jal-2023.4.7/jal/data_export/taxes_flow.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-21 18:29:43.983790 jal-2023.4.7/jal/data_export/templates/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)        0 2022-01-30 08:37:57.000000 jal-2023.4.7/jal/data_export/templates/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1286 2023-02-07 18:26:24.000000 jal-2023.4.7/jal/data_export/templates/tax_prt_dividends.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2594 2023-02-07 18:26:24.000000 jal-2023.4.7/jal/data_export/templates/tax_prt_shares.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6163 2022-01-30 08:37:57.000000 jal-2023.4.7/jal/data_export/templates/tax_rus_bonds.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4792 2022-02-13 11:04:18.000000 jal-2023.4.7/jal/data_export/templates/tax_rus_corporate_actions.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4938 2022-04-30 20:05:13.000000 jal-2023.4.7/jal/data_export/templates/tax_rus_crypto.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4948 2022-04-30 20:05:13.000000 jal-2023.4.7/jal/data_export/templates/tax_rus_derivatives.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3249 2022-02-13 11:04:18.000000 jal-2023.4.7/jal/data_export/templates/tax_rus_dividends.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1450 2022-01-30 08:37:57.000000 jal-2023.4.7/jal/data_export/templates/tax_rus_fees.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1133 2022-06-19 17:39:33.000000 jal-2023.4.7/jal/data_export/templates/tax_rus_flow.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1654 2022-07-20 07:00:10.000000 jal-2023.4.7/jal/data_export/templates/tax_rus_interests.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5303 2022-01-30 08:37:57.000000 jal-2023.4.7/jal/data_export/templates/tax_rus_trades.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    10842 2023-02-08 13:35:53.000000 jal-2023.4.7/jal/data_export/xlsx.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-21 18:29:43.987123 jal-2023.4.7/jal/data_import/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.7/jal/data_import/__init__.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-21 18:29:43.987123 jal-2023.4.7/jal/data_import/broker_statements/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)        0 2022-01-22 16:32:16.000000 jal-2023.4.7/jal/data_import/broker_statements/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    65337 2023-04-21 18:16:02.000000 jal-2023.4.7/jal/data_import/broker_statements/ibkr.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    19903 2022-08-21 07:15:06.000000 jal-2023.4.7/jal/data_import/broker_statements/just2trade.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     9470 2022-08-21 07:15:06.000000 jal-2023.4.7/jal/data_import/broker_statements/kit.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5857 2023-02-14 12:14:19.000000 jal-2023.4.7/jal/data_import/broker_statements/open_portfolio.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    31013 2023-04-20 21:42:30.000000 jal-2023.4.7/jal/data_import/broker_statements/openbroker.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    15460 2022-12-07 21:59:21.000000 jal-2023.4.7/jal/data_import/broker_statements/psb.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    27485 2023-04-20 18:05:58.000000 jal-2023.4.7/jal/data_import/broker_statements/uralsib.py
--rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     3893 2023-03-05 19:06:08.000000 jal-2023.4.7/jal/data_import/category_recognizer.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      543 2021-08-05 15:24:10.000000 jal-2023.4.7/jal/data_import/import_schema.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    15598 2023-04-15 14:13:28.000000 jal-2023.4.7/jal/data_import/slips.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    13145 2023-04-14 18:14:21.000000 jal-2023.4.7/jal/data_import/slips_tax.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    35722 2023-04-21 16:25:20.000000 jal-2023.4.7/jal/data_import/statement.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    11314 2023-02-02 08:45:14.000000 jal-2023.4.7/jal/data_import/statement_xls.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6950 2023-04-14 11:26:23.000000 jal-2023.4.7/jal/data_import/statement_xml.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3224 2023-04-08 19:50:05.000000 jal-2023.4.7/jal/data_import/statements.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-21 18:29:43.993790 jal-2023.4.7/jal/db/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.7/jal/db/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    17607 2023-02-27 16:25:45.000000 jal-2023.4.7/jal/db/account.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    21487 2023-04-14 11:26:23.000000 jal-2023.4.7/jal/db/asset.py
--rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     6074 2022-12-06 18:30:39.000000 jal-2023.4.7/jal/db/backup_restore.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7360 2023-02-27 17:48:37.000000 jal-2023.4.7/jal/db/balances_model.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4103 2023-02-27 16:03:46.000000 jal-2023.4.7/jal/db/category.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5218 2023-02-07 18:26:24.000000 jal-2023.4.7/jal/db/closed_trade.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2399 2023-03-08 17:11:23.000000 jal-2023.4.7/jal/db/country.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    18652 2023-04-15 13:39:15.000000 jal-2023.4.7/jal/db/db.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3941 2023-04-12 09:44:25.000000 jal-2023.4.7/jal/db/helpers.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    15989 2023-04-14 11:27:05.000000 jal-2023.4.7/jal/db/holdings_model.py
--rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)    16683 2023-04-15 14:13:28.000000 jal-2023.4.7/jal/db/ledger.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    60565 2023-04-07 14:10:37.000000 jal-2023.4.7/jal/db/operations.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7461 2023-04-20 16:47:43.000000 jal-2023.4.7/jal/db/operations_model.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3379 2023-02-20 16:05:40.000000 jal-2023.4.7/jal/db/peer.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    15204 2023-04-15 13:54:08.000000 jal-2023.4.7/jal/db/reference_models.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1190 2023-01-06 21:49:49.000000 jal-2023.4.7/jal/db/settings.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      438 2023-02-16 17:12:29.000000 jal-2023.4.7/jal/db/tag.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6777 2023-04-14 18:14:21.000000 jal-2023.4.7/jal/db/tax_estimator.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1458 2023-02-23 19:54:06.000000 jal-2023.4.7/jal/db/view_model.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-21 18:29:43.997123 jal-2023.4.7/jal/img/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2922 2021-05-26 12:51:46.000000 jal-2023.4.7/jal/img/accept.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1443 2021-05-26 12:51:46.000000 jal-2023.4.7/jal/img/add.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2049 2021-05-26 12:51:46.000000 jal-2023.4.7/jal/img/add_child.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      435 2022-04-25 10:26:48.000000 jal-2023.4.7/jal/img/broom.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4004 2021-05-26 12:51:46.000000 jal-2023.4.7/jal/img/cancel.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      806 2023-03-08 16:58:09.000000 jal-2023.4.7/jal/img/chart.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      898 2021-05-26 12:51:46.000000 jal-2023.4.7/jal/img/copy.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2812 2021-05-26 12:51:46.000000 jal-2023.4.7/jal/img/delete.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      583 2021-03-20 12:52:05.000000 jal-2023.4.7/jal/img/ibkr.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2340 2022-04-29 07:05:21.000000 jal-2023.4.7/jal/img/j2t.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5563 2022-01-13 06:08:45.000000 jal-2023.4.7/jal/img/jal.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1516 2021-03-22 11:20:31.000000 jal-2023.4.7/jal/img/kit.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1163 2022-12-28 10:47:37.000000 jal-2023.4.7/jal/img/list.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      342 2022-04-25 10:26:48.000000 jal-2023.4.7/jal/img/meatballs.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      611 2021-05-26 12:51:46.000000 jal-2023.4.7/jal/img/new.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1175 2022-07-10 15:39:56.000000 jal-2023.4.7/jal/img/open_portfolio.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    15086 2021-08-05 15:24:10.000000 jal-2023.4.7/jal/img/openbroker.ico
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1150 2021-08-05 15:24:10.000000 jal-2023.4.7/jal/img/psb.ico
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1150 2021-03-20 12:52:05.000000 jal-2023.4.7/jal/img/quik.ico
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2651 2021-05-26 12:51:46.000000 jal-2023.4.7/jal/img/reconcile.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      822 2021-05-26 12:51:46.000000 jal-2023.4.7/jal/img/remove.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1874 2023-03-08 16:53:42.000000 jal-2023.4.7/jal/img/tax.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1406 2021-03-20 12:52:05.000000 jal-2023.4.7/jal/img/uralsib.ico
--rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     1938 2023-01-19 12:05:21.000000 jal-2023.4.7/jal/jal.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    91499 2023-04-07 14:10:37.000000 jal-2023.4.7/jal/jal_init.sql
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-21 18:29:43.997123 jal-2023.4.7/jal/languages/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      424 2020-12-21 16:23:10.000000 jal-2023.4.7/jal/languages/en.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    32025 2022-01-13 06:08:45.000000 jal-2023.4.7/jal/languages/en.qm
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      287 2022-04-25 10:26:48.000000 jal-2023.4.7/jal/languages/ru.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    87966 2023-04-20 18:09:17.000000 jal-2023.4.7/jal/languages/ru.qm
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-21 18:29:44.000456 jal-2023.4.7/jal/net/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2021-08-17 15:15:47.000000 jal-2023.4.7/jal/net/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    24656 2023-04-14 18:14:21.000000 jal-2023.4.7/jal/net/downloader.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2912 2023-01-27 21:53:46.000000 jal-2023.4.7/jal/net/helpers.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2040 2023-03-06 11:34:17.000000 jal-2023.4.7/jal/pypi_description.md
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-21 18:29:44.003790 jal-2023.4.7/jal/reports/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.7/jal/reports/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2967 2023-04-14 18:14:21.000000 jal-2023.4.7/jal/reports/category.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    14386 2023-04-14 18:14:21.000000 jal-2023.4.7/jal/reports/deals.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3936 2023-04-14 18:14:21.000000 jal-2023.4.7/jal/reports/holdings.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    17557 2023-04-16 16:12:41.000000 jal-2023.4.7/jal/reports/income_spending.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2855 2023-04-14 18:14:21.000000 jal-2023.4.7/jal/reports/peer.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     8772 2023-04-16 16:04:35.000000 jal-2023.4.7/jal/reports/profit_loss.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3287 2023-02-16 10:22:14.000000 jal-2023.4.7/jal/reports/reports.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2827 2023-04-14 18:14:21.000000 jal-2023.4.7/jal/reports/tag.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-21 18:29:44.003790 jal-2023.4.7/jal/ui/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.7/jal/ui/__init__.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-21 18:29:44.007123 jal-2023.4.7/jal/ui/reports/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)        0 2022-01-13 15:45:51.000000 jal-2023.4.7/jal/ui/reports/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5179 2023-04-20 18:08:23.000000 jal-2023.4.7/jal/ui/reports/ui_category_report.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4099 2023-04-20 18:08:23.000000 jal-2023.4.7/jal/ui/reports/ui_deals_report.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4159 2023-04-20 18:08:23.000000 jal-2023.4.7/jal/ui/reports/ui_holdings_report.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4954 2023-04-20 18:08:23.000000 jal-2023.4.7/jal/ui/reports/ui_income_spending_report.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5382 2023-04-20 18:08:23.000000 jal-2023.4.7/jal/ui/reports/ui_peer_report.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4687 2023-04-20 18:08:23.000000 jal-2023.4.7/jal/ui/reports/ui_profit_loss_report.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5353 2023-04-20 18:08:23.000000 jal-2023.4.7/jal/ui/reports/ui_tag_report.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4805 2023-04-20 18:08:23.000000 jal-2023.4.7/jal/ui/reports/ui_tax_estimation.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    12742 2023-04-20 18:08:23.000000 jal-2023.4.7/jal/ui/ui_asset_dlg.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4056 2023-04-20 18:08:23.000000 jal-2023.4.7/jal/ui/ui_flow_export_widget.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    14782 2023-04-20 18:08:23.000000 jal-2023.4.7/jal/ui/ui_login_fns_dlg.py
--rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     9324 2023-04-20 18:08:23.000000 jal-2023.4.7/jal/ui/ui_main_window.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    14510 2023-04-20 18:08:23.000000 jal-2023.4.7/jal/ui/ui_operations_widget.py
--rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     5707 2023-04-20 18:08:23.000000 jal-2023.4.7/jal/ui/ui_rebuild_window.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7302 2023-04-20 18:08:23.000000 jal-2023.4.7/jal/ui/ui_reference_data_dlg.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2903 2023-04-20 18:08:23.000000 jal-2023.4.7/jal/ui/ui_select_account_dlg.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3253 2023-04-20 18:08:23.000000 jal-2023.4.7/jal/ui/ui_select_reference_dlg.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    16301 2023-04-20 18:08:23.000000 jal-2023.4.7/jal/ui/ui_slip_import_dlg.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     9674 2023-04-20 18:08:23.000000 jal-2023.4.7/jal/ui/ui_tax_export_widget.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4023 2023-04-20 18:08:23.000000 jal-2023.4.7/jal/ui/ui_update_quotes_window.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-21 18:29:44.017123 jal-2023.4.7/jal/updates/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.7/jal/updates/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5122 2020-12-21 16:23:10.000000 jal-2023.4.7/jal/updates/jal_delta_10.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    12870 2021-08-18 12:53:40.000000 jal-2023.4.7/jal/updates/jal_delta_11.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    26116 2021-01-13 17:04:46.000000 jal-2023.4.7/jal/updates/jal_delta_12.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    16516 2021-01-30 16:01:43.000000 jal-2023.4.7/jal/updates/jal_delta_13.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    34961 2021-02-27 17:35:02.000000 jal-2023.4.7/jal/updates/jal_delta_14.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2250 2021-02-27 17:35:02.000000 jal-2023.4.7/jal/updates/jal_delta_15.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3630 2021-02-27 17:35:02.000000 jal-2023.4.7/jal/updates/jal_delta_16.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    20912 2021-02-27 17:35:02.000000 jal-2023.4.7/jal/updates/jal_delta_17.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      656 2021-03-07 11:58:53.000000 jal-2023.4.7/jal/updates/jal_delta_18.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      686 2021-03-08 13:39:11.000000 jal-2023.4.7/jal/updates/jal_delta_19.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    13578 2021-03-12 14:26:01.000000 jal-2023.4.7/jal/updates/jal_delta_20.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1428 2021-03-19 12:24:53.000000 jal-2023.4.7/jal/updates/jal_delta_21.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      949 2021-03-22 11:20:31.000000 jal-2023.4.7/jal/updates/jal_delta_22.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    17602 2021-04-08 12:12:36.000000 jal-2023.4.7/jal/updates/jal_delta_23.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      344 2021-04-11 10:57:46.000000 jal-2023.4.7/jal/updates/jal_delta_24.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     8270 2021-04-22 04:11:28.000000 jal-2023.4.7/jal/updates/jal_delta_25.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2492 2021-08-12 19:15:12.000000 jal-2023.4.7/jal/updates/jal_delta_26.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    26325 2022-01-13 05:57:31.000000 jal-2023.4.7/jal/updates/jal_delta_27.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    13276 2022-01-13 06:08:45.000000 jal-2023.4.7/jal/updates/jal_delta_28.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    35370 2022-01-13 15:45:51.000000 jal-2023.4.7/jal/updates/jal_delta_29.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     8671 2022-02-13 13:11:58.000000 jal-2023.4.7/jal/updates/jal_delta_30.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    11413 2022-02-13 11:04:18.000000 jal-2023.4.7/jal/updates/jal_delta_31.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    12545 2022-03-31 14:26:11.000000 jal-2023.4.7/jal/updates/jal_delta_32.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4229 2022-03-31 14:26:11.000000 jal-2023.4.7/jal/updates/jal_delta_33.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2287 2022-04-06 14:47:21.000000 jal-2023.4.7/jal/updates/jal_delta_34.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2858 2022-04-30 20:05:13.000000 jal-2023.4.7/jal/updates/jal_delta_35.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3427 2022-06-19 17:39:33.000000 jal-2023.4.7/jal/updates/jal_delta_36.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3755 2022-07-20 07:00:10.000000 jal-2023.4.7/jal/updates/jal_delta_37.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    21913 2022-08-21 07:15:06.000000 jal-2023.4.7/jal/updates/jal_delta_38.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      343 2023-01-04 13:14:35.000000 jal-2023.4.7/jal/updates/jal_delta_39.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3055 2023-01-27 21:53:46.000000 jal-2023.4.7/jal/updates/jal_delta_40.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    48157 2023-02-07 18:26:24.000000 jal-2023.4.7/jal/updates/jal_delta_41.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2085 2023-02-20 14:55:36.000000 jal-2023.4.7/jal/updates/jal_delta_42.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2528 2023-03-08 16:23:30.000000 jal-2023.4.7/jal/updates/jal_delta_43.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3020 2023-04-07 14:10:37.000000 jal-2023.4.7/jal/updates/jal_delta_44.sql
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-21 18:29:44.017123 jal-2023.4.7/jal/widgets/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.7/jal/widgets/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3912 2023-04-15 09:01:12.000000 jal-2023.4.7/jal/widgets/abstract_operation_details.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6846 2023-04-15 14:13:28.000000 jal-2023.4.7/jal/widgets/account_select.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    14491 2023-04-15 14:13:28.000000 jal-2023.4.7/jal/widgets/asset_dialog.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    11302 2023-04-15 14:13:28.000000 jal-2023.4.7/jal/widgets/corporate_action_widget.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-21 18:29:44.020457 jal-2023.4.7/jal/widgets/custom/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)        0 2022-12-24 19:32:40.000000 jal-2023.4.7/jal/widgets/custom/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4703 2023-04-20 16:58:35.000000 jal-2023.4.7/jal/widgets/custom/date_range_selector.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2015 2023-04-15 14:13:28.000000 jal-2023.4.7/jal/widgets/custom/db_lookup_combobox.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5874 2023-04-20 16:38:19.000000 jal-2023.4.7/jal/widgets/custom/log_viewer.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    13628 2023-04-15 14:13:28.000000 jal-2023.4.7/jal/widgets/delegates.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     9289 2023-04-15 14:13:28.000000 jal-2023.4.7/jal/widgets/dividend_widget.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    10438 2023-04-16 16:04:35.000000 jal-2023.4.7/jal/widgets/helpers.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    12488 2023-04-15 14:13:28.000000 jal-2023.4.7/jal/widgets/income_spending_widget.py
--rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)    13018 2023-04-14 18:14:21.000000 jal-2023.4.7/jal/widgets/main_window.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3386 2023-04-15 14:13:28.000000 jal-2023.4.7/jal/widgets/mdi.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2854 2022-12-26 13:26:40.000000 jal-2023.4.7/jal/widgets/operations_tabs.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7159 2023-04-14 18:14:21.000000 jal-2023.4.7/jal/widgets/operations_widget.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6013 2023-04-15 14:13:28.000000 jal-2023.4.7/jal/widgets/price_chart.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5667 2023-04-15 14:13:28.000000 jal-2023.4.7/jal/widgets/qr_scanner.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    11244 2023-04-14 18:14:21.000000 jal-2023.4.7/jal/widgets/reference_data.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    21856 2023-04-15 13:54:08.000000 jal-2023.4.7/jal/widgets/reference_dialogs.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4779 2023-04-15 14:13:28.000000 jal-2023.4.7/jal/widgets/reference_selector.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      632 2022-12-26 08:54:07.000000 jal-2023.4.7/jal/widgets/register_designer_plugins.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3499 2023-04-15 14:14:41.000000 jal-2023.4.7/jal/widgets/selection_dialog.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7862 2023-04-14 18:14:21.000000 jal-2023.4.7/jal/widgets/tax_widget.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6890 2023-04-15 14:13:28.000000 jal-2023.4.7/jal/widgets/trade_widget.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    10088 2023-04-15 14:13:28.000000 jal-2023.4.7/jal/widgets/transfer_widget.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-21 18:29:43.980456 jal-2023.4.7/jal.egg-info/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2726 2023-04-21 18:29:43.000000 jal-2023.4.7/jal.egg-info/PKG-INFO
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5592 2023-04-21 18:29:43.000000 jal-2023.4.7/jal.egg-info/SOURCES.txt
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)        1 2023-04-21 18:29:43.000000 jal-2023.4.7/jal.egg-info/dependency_links.txt
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       37 2023-04-21 18:29:43.000000 jal-2023.4.7/jal.egg-info/entry_points.txt
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       67 2023-04-21 18:29:43.000000 jal-2023.4.7/jal.egg-info/requires.txt
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       10 2023-04-21 18:29:43.000000 jal-2023.4.7/jal.egg-info/top_level.txt
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       38 2023-04-21 18:29:44.020457 jal-2023.4.7/setup.cfg
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1756 2023-04-14 18:14:21.000000 jal-2023.4.7/setup.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-23 12:20:32.026746 jal-2023.4.8/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      176 2022-01-13 06:08:45.000000 jal-2023.4.8/MANIFEST.in
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2726 2023-04-23 12:20:32.026746 jal-2023.4.8/PKG-INFO
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-23 12:20:31.833411 jal-2023.4.8/docs/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7580 2023-04-15 14:23:01.000000 jal-2023.4.8/docs/README.md
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-23 12:20:31.836744 jal-2023.4.8/jal/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       24 2023-04-23 12:17:50.000000 jal-2023.4.8/jal/__init__.py
+-rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     3831 2023-04-15 14:13:28.000000 jal-2023.4.8/jal/constants.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-23 12:20:31.843411 jal-2023.4.8/jal/data_export/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2022-01-13 15:45:51.000000 jal-2023.4.8/jal/data_export/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    19856 2023-04-14 11:26:23.000000 jal-2023.4.8/jal/data_export/dlsg.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-23 12:20:31.846744 jal-2023.4.8/jal/data_export/tax_reports/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.8/jal/data_export/tax_reports/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      990 2023-02-07 18:26:24.000000 jal-2023.4.8/jal/data_export/tax_reports/portugal.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7089 2023-02-08 10:00:47.000000 jal-2023.4.8/jal/data_export/tax_reports/portugal.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1532 2023-02-07 18:26:24.000000 jal-2023.4.8/jal/data_export/tax_reports/russia.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    38366 2023-04-14 11:26:23.000000 jal-2023.4.8/jal/data_export/tax_reports/russia.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6433 2023-02-07 18:26:24.000000 jal-2023.4.8/jal/data_export/taxes.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5299 2023-02-07 18:26:24.000000 jal-2023.4.8/jal/data_export/taxes_flow.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-23 12:20:31.860078 jal-2023.4.8/jal/data_export/templates/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)        0 2022-01-30 08:37:57.000000 jal-2023.4.8/jal/data_export/templates/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1286 2023-02-07 18:26:24.000000 jal-2023.4.8/jal/data_export/templates/tax_prt_dividends.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2594 2023-02-07 18:26:24.000000 jal-2023.4.8/jal/data_export/templates/tax_prt_shares.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6163 2022-01-30 08:37:57.000000 jal-2023.4.8/jal/data_export/templates/tax_rus_bonds.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4792 2022-02-13 11:04:18.000000 jal-2023.4.8/jal/data_export/templates/tax_rus_corporate_actions.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4938 2022-04-30 20:05:13.000000 jal-2023.4.8/jal/data_export/templates/tax_rus_crypto.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4948 2022-04-30 20:05:13.000000 jal-2023.4.8/jal/data_export/templates/tax_rus_derivatives.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3249 2022-02-13 11:04:18.000000 jal-2023.4.8/jal/data_export/templates/tax_rus_dividends.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1450 2022-01-30 08:37:57.000000 jal-2023.4.8/jal/data_export/templates/tax_rus_fees.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1133 2022-06-19 17:39:33.000000 jal-2023.4.8/jal/data_export/templates/tax_rus_flow.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1654 2022-07-20 07:00:10.000000 jal-2023.4.8/jal/data_export/templates/tax_rus_interests.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5303 2022-01-30 08:37:57.000000 jal-2023.4.8/jal/data_export/templates/tax_rus_trades.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    10842 2023-02-08 13:35:53.000000 jal-2023.4.8/jal/data_export/xlsx.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-23 12:20:31.870078 jal-2023.4.8/jal/data_import/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.8/jal/data_import/__init__.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-23 12:20:31.876744 jal-2023.4.8/jal/data_import/broker_statements/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)        0 2022-01-22 16:32:16.000000 jal-2023.4.8/jal/data_import/broker_statements/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    65337 2023-04-21 18:16:02.000000 jal-2023.4.8/jal/data_import/broker_statements/ibkr.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    19903 2022-08-21 07:15:06.000000 jal-2023.4.8/jal/data_import/broker_statements/just2trade.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     9470 2022-08-21 07:15:06.000000 jal-2023.4.8/jal/data_import/broker_statements/kit.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5857 2023-02-14 12:14:19.000000 jal-2023.4.8/jal/data_import/broker_statements/open_portfolio.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    31284 2023-04-22 15:56:59.000000 jal-2023.4.8/jal/data_import/broker_statements/openbroker.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    15460 2022-12-07 21:59:21.000000 jal-2023.4.8/jal/data_import/broker_statements/psb.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    27485 2023-04-20 18:05:58.000000 jal-2023.4.8/jal/data_import/broker_statements/uralsib.py
+-rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     3893 2023-03-05 19:06:08.000000 jal-2023.4.8/jal/data_import/category_recognizer.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      543 2021-08-05 15:24:10.000000 jal-2023.4.8/jal/data_import/import_schema.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    15598 2023-04-15 14:13:28.000000 jal-2023.4.8/jal/data_import/slips.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    13145 2023-04-14 18:14:21.000000 jal-2023.4.8/jal/data_import/slips_tax.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    35873 2023-04-22 16:02:25.000000 jal-2023.4.8/jal/data_import/statement.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    11314 2023-02-02 08:45:14.000000 jal-2023.4.8/jal/data_import/statement_xls.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6950 2023-04-14 11:26:23.000000 jal-2023.4.8/jal/data_import/statement_xml.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3224 2023-04-08 19:50:05.000000 jal-2023.4.8/jal/data_import/statements.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-23 12:20:31.896745 jal-2023.4.8/jal/db/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.8/jal/db/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    17607 2023-02-27 16:25:45.000000 jal-2023.4.8/jal/db/account.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    21487 2023-04-14 11:26:23.000000 jal-2023.4.8/jal/db/asset.py
+-rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     6074 2022-12-06 18:30:39.000000 jal-2023.4.8/jal/db/backup_restore.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7360 2023-02-27 17:48:37.000000 jal-2023.4.8/jal/db/balances_model.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4103 2023-02-27 16:03:46.000000 jal-2023.4.8/jal/db/category.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5218 2023-02-07 18:26:24.000000 jal-2023.4.8/jal/db/closed_trade.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2399 2023-03-08 17:11:23.000000 jal-2023.4.8/jal/db/country.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    18652 2023-04-15 13:39:15.000000 jal-2023.4.8/jal/db/db.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3941 2023-04-12 09:44:25.000000 jal-2023.4.8/jal/db/helpers.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    15989 2023-04-14 11:27:05.000000 jal-2023.4.8/jal/db/holdings_model.py
+-rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)    16683 2023-04-15 14:13:28.000000 jal-2023.4.8/jal/db/ledger.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    60565 2023-04-07 14:10:37.000000 jal-2023.4.8/jal/db/operations.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7461 2023-04-20 16:47:43.000000 jal-2023.4.8/jal/db/operations_model.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3379 2023-02-20 16:05:40.000000 jal-2023.4.8/jal/db/peer.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    15204 2023-04-15 13:54:08.000000 jal-2023.4.8/jal/db/reference_models.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1190 2023-01-06 21:49:49.000000 jal-2023.4.8/jal/db/settings.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      438 2023-02-16 17:12:29.000000 jal-2023.4.8/jal/db/tag.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6777 2023-04-14 18:14:21.000000 jal-2023.4.8/jal/db/tax_estimator.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1458 2023-02-23 19:54:06.000000 jal-2023.4.8/jal/db/view_model.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-23 12:20:31.920078 jal-2023.4.8/jal/img/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2922 2021-05-26 12:51:46.000000 jal-2023.4.8/jal/img/accept.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1443 2021-05-26 12:51:46.000000 jal-2023.4.8/jal/img/add.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2049 2021-05-26 12:51:46.000000 jal-2023.4.8/jal/img/add_child.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      435 2022-04-25 10:26:48.000000 jal-2023.4.8/jal/img/broom.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4004 2021-05-26 12:51:46.000000 jal-2023.4.8/jal/img/cancel.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      806 2023-03-08 16:58:09.000000 jal-2023.4.8/jal/img/chart.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      898 2021-05-26 12:51:46.000000 jal-2023.4.8/jal/img/copy.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2812 2021-05-26 12:51:46.000000 jal-2023.4.8/jal/img/delete.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      583 2021-03-20 12:52:05.000000 jal-2023.4.8/jal/img/ibkr.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2340 2022-04-29 07:05:21.000000 jal-2023.4.8/jal/img/j2t.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5563 2022-01-13 06:08:45.000000 jal-2023.4.8/jal/img/jal.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1516 2021-03-22 11:20:31.000000 jal-2023.4.8/jal/img/kit.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1163 2022-12-28 10:47:37.000000 jal-2023.4.8/jal/img/list.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      342 2022-04-25 10:26:48.000000 jal-2023.4.8/jal/img/meatballs.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      611 2021-05-26 12:51:46.000000 jal-2023.4.8/jal/img/new.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1175 2022-07-10 15:39:56.000000 jal-2023.4.8/jal/img/open_portfolio.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    15086 2021-08-05 15:24:10.000000 jal-2023.4.8/jal/img/openbroker.ico
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1150 2021-08-05 15:24:10.000000 jal-2023.4.8/jal/img/psb.ico
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1150 2021-03-20 12:52:05.000000 jal-2023.4.8/jal/img/quik.ico
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2651 2021-05-26 12:51:46.000000 jal-2023.4.8/jal/img/reconcile.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      822 2021-05-26 12:51:46.000000 jal-2023.4.8/jal/img/remove.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1874 2023-03-08 16:53:42.000000 jal-2023.4.8/jal/img/tax.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1406 2021-03-20 12:52:05.000000 jal-2023.4.8/jal/img/uralsib.ico
+-rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     1938 2023-01-19 12:05:21.000000 jal-2023.4.8/jal/jal.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    91499 2023-04-07 14:10:37.000000 jal-2023.4.8/jal/jal_init.sql
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-23 12:20:31.923411 jal-2023.4.8/jal/languages/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      424 2020-12-21 16:23:10.000000 jal-2023.4.8/jal/languages/en.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    32025 2022-01-13 06:08:45.000000 jal-2023.4.8/jal/languages/en.qm
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      287 2022-04-25 10:26:48.000000 jal-2023.4.8/jal/languages/ru.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    87966 2023-04-20 18:09:17.000000 jal-2023.4.8/jal/languages/ru.qm
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-23 12:20:31.926745 jal-2023.4.8/jal/net/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2021-08-17 15:15:47.000000 jal-2023.4.8/jal/net/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    25047 2023-04-22 15:07:28.000000 jal-2023.4.8/jal/net/downloader.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2912 2023-01-27 21:53:46.000000 jal-2023.4.8/jal/net/helpers.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2040 2023-03-06 11:34:17.000000 jal-2023.4.8/jal/pypi_description.md
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-23 12:20:31.936745 jal-2023.4.8/jal/reports/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.8/jal/reports/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2967 2023-04-14 18:14:21.000000 jal-2023.4.8/jal/reports/category.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    14386 2023-04-14 18:14:21.000000 jal-2023.4.8/jal/reports/deals.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3936 2023-04-14 18:14:21.000000 jal-2023.4.8/jal/reports/holdings.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    17557 2023-04-16 16:12:41.000000 jal-2023.4.8/jal/reports/income_spending.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2855 2023-04-14 18:14:21.000000 jal-2023.4.8/jal/reports/peer.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     8772 2023-04-16 16:04:35.000000 jal-2023.4.8/jal/reports/profit_loss.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3287 2023-02-16 10:22:14.000000 jal-2023.4.8/jal/reports/reports.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2827 2023-04-14 18:14:21.000000 jal-2023.4.8/jal/reports/tag.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-23 12:20:31.946745 jal-2023.4.8/jal/ui/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.8/jal/ui/__init__.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-23 12:20:31.956745 jal-2023.4.8/jal/ui/reports/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)        0 2022-01-13 15:45:51.000000 jal-2023.4.8/jal/ui/reports/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5179 2023-04-20 18:08:23.000000 jal-2023.4.8/jal/ui/reports/ui_category_report.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4099 2023-04-20 18:08:23.000000 jal-2023.4.8/jal/ui/reports/ui_deals_report.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4159 2023-04-20 18:08:23.000000 jal-2023.4.8/jal/ui/reports/ui_holdings_report.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4954 2023-04-20 18:08:23.000000 jal-2023.4.8/jal/ui/reports/ui_income_spending_report.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5382 2023-04-20 18:08:23.000000 jal-2023.4.8/jal/ui/reports/ui_peer_report.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4687 2023-04-20 18:08:23.000000 jal-2023.4.8/jal/ui/reports/ui_profit_loss_report.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5353 2023-04-20 18:08:23.000000 jal-2023.4.8/jal/ui/reports/ui_tag_report.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4805 2023-04-20 18:08:23.000000 jal-2023.4.8/jal/ui/reports/ui_tax_estimation.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    12742 2023-04-20 18:08:23.000000 jal-2023.4.8/jal/ui/ui_asset_dlg.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4056 2023-04-20 18:08:23.000000 jal-2023.4.8/jal/ui/ui_flow_export_widget.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    14782 2023-04-20 18:08:23.000000 jal-2023.4.8/jal/ui/ui_login_fns_dlg.py
+-rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     9324 2023-04-20 18:08:23.000000 jal-2023.4.8/jal/ui/ui_main_window.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    14510 2023-04-20 18:08:23.000000 jal-2023.4.8/jal/ui/ui_operations_widget.py
+-rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     5707 2023-04-20 18:08:23.000000 jal-2023.4.8/jal/ui/ui_rebuild_window.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7302 2023-04-20 18:08:23.000000 jal-2023.4.8/jal/ui/ui_reference_data_dlg.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2903 2023-04-20 18:08:23.000000 jal-2023.4.8/jal/ui/ui_select_account_dlg.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3253 2023-04-20 18:08:23.000000 jal-2023.4.8/jal/ui/ui_select_reference_dlg.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    16301 2023-04-20 18:08:23.000000 jal-2023.4.8/jal/ui/ui_slip_import_dlg.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     9674 2023-04-20 18:08:23.000000 jal-2023.4.8/jal/ui/ui_tax_export_widget.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4023 2023-04-20 18:08:23.000000 jal-2023.4.8/jal/ui/ui_update_quotes_window.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-23 12:20:31.996745 jal-2023.4.8/jal/updates/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.8/jal/updates/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5122 2020-12-21 16:23:10.000000 jal-2023.4.8/jal/updates/jal_delta_10.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    12870 2021-08-18 12:53:40.000000 jal-2023.4.8/jal/updates/jal_delta_11.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    26116 2021-01-13 17:04:46.000000 jal-2023.4.8/jal/updates/jal_delta_12.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    16516 2021-01-30 16:01:43.000000 jal-2023.4.8/jal/updates/jal_delta_13.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    34961 2021-02-27 17:35:02.000000 jal-2023.4.8/jal/updates/jal_delta_14.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2250 2021-02-27 17:35:02.000000 jal-2023.4.8/jal/updates/jal_delta_15.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3630 2021-02-27 17:35:02.000000 jal-2023.4.8/jal/updates/jal_delta_16.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    20912 2021-02-27 17:35:02.000000 jal-2023.4.8/jal/updates/jal_delta_17.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      656 2021-03-07 11:58:53.000000 jal-2023.4.8/jal/updates/jal_delta_18.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      686 2021-03-08 13:39:11.000000 jal-2023.4.8/jal/updates/jal_delta_19.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    13578 2021-03-12 14:26:01.000000 jal-2023.4.8/jal/updates/jal_delta_20.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1428 2021-03-19 12:24:53.000000 jal-2023.4.8/jal/updates/jal_delta_21.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      949 2021-03-22 11:20:31.000000 jal-2023.4.8/jal/updates/jal_delta_22.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    17602 2021-04-08 12:12:36.000000 jal-2023.4.8/jal/updates/jal_delta_23.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      344 2021-04-11 10:57:46.000000 jal-2023.4.8/jal/updates/jal_delta_24.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     8270 2021-04-22 04:11:28.000000 jal-2023.4.8/jal/updates/jal_delta_25.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2492 2021-08-12 19:15:12.000000 jal-2023.4.8/jal/updates/jal_delta_26.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    26325 2022-01-13 05:57:31.000000 jal-2023.4.8/jal/updates/jal_delta_27.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    13276 2022-01-13 06:08:45.000000 jal-2023.4.8/jal/updates/jal_delta_28.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    35370 2022-01-13 15:45:51.000000 jal-2023.4.8/jal/updates/jal_delta_29.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     8671 2022-02-13 13:11:58.000000 jal-2023.4.8/jal/updates/jal_delta_30.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    11413 2022-02-13 11:04:18.000000 jal-2023.4.8/jal/updates/jal_delta_31.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    12545 2022-03-31 14:26:11.000000 jal-2023.4.8/jal/updates/jal_delta_32.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4229 2022-03-31 14:26:11.000000 jal-2023.4.8/jal/updates/jal_delta_33.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2287 2022-04-06 14:47:21.000000 jal-2023.4.8/jal/updates/jal_delta_34.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2858 2022-04-30 20:05:13.000000 jal-2023.4.8/jal/updates/jal_delta_35.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3427 2022-06-19 17:39:33.000000 jal-2023.4.8/jal/updates/jal_delta_36.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3755 2022-07-20 07:00:10.000000 jal-2023.4.8/jal/updates/jal_delta_37.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    21913 2022-08-21 07:15:06.000000 jal-2023.4.8/jal/updates/jal_delta_38.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      343 2023-01-04 13:14:35.000000 jal-2023.4.8/jal/updates/jal_delta_39.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3055 2023-01-27 21:53:46.000000 jal-2023.4.8/jal/updates/jal_delta_40.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    48157 2023-02-07 18:26:24.000000 jal-2023.4.8/jal/updates/jal_delta_41.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2085 2023-02-20 14:55:36.000000 jal-2023.4.8/jal/updates/jal_delta_42.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2528 2023-03-08 16:23:30.000000 jal-2023.4.8/jal/updates/jal_delta_43.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3020 2023-04-07 14:10:37.000000 jal-2023.4.8/jal/updates/jal_delta_44.sql
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-23 12:20:32.020079 jal-2023.4.8/jal/widgets/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.8/jal/widgets/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3912 2023-04-15 09:01:12.000000 jal-2023.4.8/jal/widgets/abstract_operation_details.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6846 2023-04-15 14:13:28.000000 jal-2023.4.8/jal/widgets/account_select.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    14491 2023-04-15 14:13:28.000000 jal-2023.4.8/jal/widgets/asset_dialog.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    11302 2023-04-15 14:13:28.000000 jal-2023.4.8/jal/widgets/corporate_action_widget.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-23 12:20:32.026746 jal-2023.4.8/jal/widgets/custom/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)        0 2022-12-24 19:32:40.000000 jal-2023.4.8/jal/widgets/custom/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4703 2023-04-20 16:58:35.000000 jal-2023.4.8/jal/widgets/custom/date_range_selector.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2015 2023-04-15 14:13:28.000000 jal-2023.4.8/jal/widgets/custom/db_lookup_combobox.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5874 2023-04-20 16:38:19.000000 jal-2023.4.8/jal/widgets/custom/log_viewer.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    13628 2023-04-15 14:13:28.000000 jal-2023.4.8/jal/widgets/delegates.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     9289 2023-04-15 14:13:28.000000 jal-2023.4.8/jal/widgets/dividend_widget.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    10438 2023-04-16 16:04:35.000000 jal-2023.4.8/jal/widgets/helpers.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    12488 2023-04-15 14:13:28.000000 jal-2023.4.8/jal/widgets/income_spending_widget.py
+-rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)    13018 2023-04-14 18:14:21.000000 jal-2023.4.8/jal/widgets/main_window.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3386 2023-04-15 14:13:28.000000 jal-2023.4.8/jal/widgets/mdi.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2854 2022-12-26 13:26:40.000000 jal-2023.4.8/jal/widgets/operations_tabs.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7159 2023-04-14 18:14:21.000000 jal-2023.4.8/jal/widgets/operations_widget.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6013 2023-04-15 14:13:28.000000 jal-2023.4.8/jal/widgets/price_chart.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5667 2023-04-15 14:13:28.000000 jal-2023.4.8/jal/widgets/qr_scanner.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    11244 2023-04-14 18:14:21.000000 jal-2023.4.8/jal/widgets/reference_data.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    21856 2023-04-15 13:54:08.000000 jal-2023.4.8/jal/widgets/reference_dialogs.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4779 2023-04-15 14:13:28.000000 jal-2023.4.8/jal/widgets/reference_selector.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      632 2022-12-26 08:54:07.000000 jal-2023.4.8/jal/widgets/register_designer_plugins.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3499 2023-04-15 14:14:41.000000 jal-2023.4.8/jal/widgets/selection_dialog.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7862 2023-04-14 18:14:21.000000 jal-2023.4.8/jal/widgets/tax_widget.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6890 2023-04-15 14:13:28.000000 jal-2023.4.8/jal/widgets/trade_widget.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    10088 2023-04-15 14:13:28.000000 jal-2023.4.8/jal/widgets/transfer_widget.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-23 12:20:31.840077 jal-2023.4.8/jal.egg-info/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2726 2023-04-23 12:20:31.000000 jal-2023.4.8/jal.egg-info/PKG-INFO
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5592 2023-04-23 12:20:31.000000 jal-2023.4.8/jal.egg-info/SOURCES.txt
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)        1 2023-04-23 12:20:31.000000 jal-2023.4.8/jal.egg-info/dependency_links.txt
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       37 2023-04-23 12:20:31.000000 jal-2023.4.8/jal.egg-info/entry_points.txt
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       67 2023-04-23 12:20:31.000000 jal-2023.4.8/jal.egg-info/requires.txt
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       10 2023-04-23 12:20:31.000000 jal-2023.4.8/jal.egg-info/top_level.txt
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       38 2023-04-23 12:20:32.026746 jal-2023.4.8/setup.cfg
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1756 2023-04-14 18:14:21.000000 jal-2023.4.8/setup.py
```

### Comparing `jal-2023.4.7/PKG-INFO` & `jal-2023.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jal
-Version: 2023.4.7
+Version: 2023.4.8
 Summary: Just Another Ledger - project to track personal financial records
 Home-page: https://github.com/titov-vv/jal
 Author-email: jal@gmx.ru
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Topic :: Office/Business :: Financial :: Accounting
```

### Comparing `jal-2023.4.7/docs/README.md` & `jal-2023.4.8/docs/README.md`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/constants.py` & `jal-2023.4.8/jal/constants.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/data_export/dlsg.py` & `jal-2023.4.8/jal/data_export/dlsg.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/data_export/tax_reports/portugal.json` & `jal-2023.4.8/jal/data_export/tax_reports/portugal.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/data_export/tax_reports/portugal.py` & `jal-2023.4.8/jal/data_export/tax_reports/portugal.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/data_export/tax_reports/russia.json` & `jal-2023.4.8/jal/data_export/tax_reports/russia.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/data_export/tax_reports/russia.py` & `jal-2023.4.8/jal/data_export/tax_reports/russia.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/data_export/taxes.py` & `jal-2023.4.8/jal/data_export/taxes.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/data_export/taxes_flow.py` & `jal-2023.4.8/jal/data_export/taxes_flow.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/data_export/templates/tax_prt_dividends.json` & `jal-2023.4.8/jal/data_export/templates/tax_prt_dividends.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/data_export/templates/tax_prt_shares.json` & `jal-2023.4.8/jal/data_export/templates/tax_prt_shares.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/data_export/templates/tax_rus_bonds.json` & `jal-2023.4.8/jal/data_export/templates/tax_rus_bonds.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/data_export/templates/tax_rus_corporate_actions.json` & `jal-2023.4.8/jal/data_export/templates/tax_rus_corporate_actions.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/data_export/templates/tax_rus_crypto.json` & `jal-2023.4.8/jal/data_export/templates/tax_rus_crypto.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/data_export/templates/tax_rus_derivatives.json` & `jal-2023.4.8/jal/data_export/templates/tax_rus_derivatives.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/data_export/templates/tax_rus_dividends.json` & `jal-2023.4.8/jal/data_export/templates/tax_rus_dividends.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/data_export/templates/tax_rus_fees.json` & `jal-2023.4.8/jal/data_export/templates/tax_rus_fees.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/data_export/templates/tax_rus_flow.json` & `jal-2023.4.8/jal/data_export/templates/tax_rus_flow.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/data_export/templates/tax_rus_interests.json` & `jal-2023.4.8/jal/data_export/templates/tax_rus_interests.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/data_export/templates/tax_rus_trades.json` & `jal-2023.4.8/jal/data_export/templates/tax_rus_trades.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/data_export/xlsx.py` & `jal-2023.4.8/jal/data_export/xlsx.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/data_import/broker_statements/ibkr.py` & `jal-2023.4.8/jal/data_import/broker_statements/ibkr.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/data_import/broker_statements/just2trade.py` & `jal-2023.4.8/jal/data_import/broker_statements/just2trade.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/data_import/broker_statements/kit.py` & `jal-2023.4.8/jal/data_import/broker_statements/kit.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/data_import/broker_statements/open_portfolio.py` & `jal-2023.4.8/jal/data_import/broker_statements/open_portfolio.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/data_import/broker_statements/openbroker.py` & `jal-2023.4.8/jal/data_import/broker_statements/openbroker.py`

 * *Files 1% similar despite different names*

```diff
@@ -375,15 +375,17 @@
             'Удержан налог на купонный доход': None,  # Tax information is included into interest payment data
             'Поставлены на торги средства клиента': self.transfer_in,
             'Списаны средства клиента': self.transfer_out,
             'Выплата дохода': self.asset_payment,
             'Возврат излишне удержанного налога': self.tax_refund,
             'Проценты по предоставленным займам ЦБ': None,   # Loan payments are loaded in self.load_loans
             'Удержан налог на прочий доход': self.cash_tax,
-            'Плата за остаток на счете': self.cash_interest
+            'Плата за остаток на счете': self.cash_interest,
+            'Удержан налог с дарения по договору дарения': self.cash_tax,  # FIXME - better to combine with next operation
+            'Поступили средства клиента': self.cash_interest
         }
 
         for cash in cash_operations:
             operation = [operation for operation in operations if cash['description'].startswith(operation)]
             if len(operation) != 1:
                 raise Statement_ImportError(self.tr("Operation not supported: ") + cash['description'])
             for operation in operations:
@@ -469,15 +471,15 @@
         intrest_pattern = r"^Выплата дохода клиент (?P<account>\w+) \((?P<type>\w+) (?P<number>\d+) (?P<symbol>.*)\) налог.* (?P<tax>\d+\.\d+) рубл.*$"
         parts = re.match(intrest_pattern, description, re.IGNORECASE)
         if parts is None:
             raise Statement_ImportError(self.tr("Can't parse Interest description ") + f"'{description}'")
         interest = parts.groupdict()
         if len(interest) != intrest_pattern.count("(?P<"):  # check expected number of matches
             raise Statement_ImportError(self.tr("Interest description miss some data ") + f"'{description}'")
-        asset_id = self.asset_id({'symbol': interest['symbol']})
+        asset_id = self.asset_id({'symbol': interest['symbol'], 'search_online': 'MOEX'})
         if asset_id is None:
             raise Statement_ImportError(self.tr("Can't find asset for bond interest ")
                                         + f"'{interest['symbol']}'")
         tax = float(interest['tax'])   # it has '\d+\.\d+' regex pattern so here shouldn't be an exception
         note = f"{interest['type']} {interest['number']}"
         new_id = max([0] + [x['id'] for x in self._data[FOF.ASSET_PAYMENTS]]) + 1
         payment = {"id": new_id, "type": FOF.PAYMENT_INTEREST, "account": account_id, "timestamp": timestamp,
```

### Comparing `jal-2023.4.7/jal/data_import/broker_statements/psb.py` & `jal-2023.4.8/jal/data_import/broker_statements/psb.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/data_import/broker_statements/uralsib.py` & `jal-2023.4.8/jal/data_import/broker_statements/uralsib.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/data_import/category_recognizer.py` & `jal-2023.4.8/jal/data_import/category_recognizer.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/data_import/import_schema.json` & `jal-2023.4.8/jal/data_import/import_schema.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/data_import/slips.py` & `jal-2023.4.8/jal/data_import/slips.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/data_import/slips_tax.py` & `jal-2023.4.8/jal/data_import/slips_tax.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/data_import/statement.py` & `jal-2023.4.8/jal/data_import/statement.py`

 * *Files 2% similar despite different names*

```diff
@@ -607,14 +607,16 @@
                 asset = self._find_in_list(self._data[FOF.ASSETS], 'id', symbol['asset'])
                 if 'isin' in asset and 'isin' in asset_info and asset['isin'] != asset_info['isin']:
                     asset = None
         if asset is None and 'search_online' in asset_info:
             if asset_info['search_online'] == "MOEX":
                 search_data = {}
                 self._uppend_keys_from(search_data, asset_info, ['isin', 'reg_number'])
+                if 'symbol' in asset_info:
+                    search_data['name'] = asset_info['symbol']   # Search as by name as it is more flexible
                 symbol = QuoteDownloader.MOEX_find_secid(**search_data)
                 if not symbol and 'symbol' in asset_info:
                     symbol = asset_info['symbol']
                 currency = asset_info['currency'] if 'currency' in asset_info else None  # Keep currency
                 asset_info = QuoteDownloader.MOEX_info(symbol=symbol)
                 asset_info['type'] = FOF.convert_predefined_asset_type(asset_info['type'])
                 if currency is not None:
```

### Comparing `jal-2023.4.7/jal/data_import/statement_xls.py` & `jal-2023.4.8/jal/data_import/statement_xls.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/data_import/statement_xml.py` & `jal-2023.4.8/jal/data_import/statement_xml.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/data_import/statements.py` & `jal-2023.4.8/jal/data_import/statements.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/db/account.py` & `jal-2023.4.8/jal/db/account.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/db/asset.py` & `jal-2023.4.8/jal/db/asset.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/db/backup_restore.py` & `jal-2023.4.8/jal/db/backup_restore.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/db/balances_model.py` & `jal-2023.4.8/jal/db/balances_model.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/db/category.py` & `jal-2023.4.8/jal/db/category.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/db/closed_trade.py` & `jal-2023.4.8/jal/db/closed_trade.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/db/country.py` & `jal-2023.4.8/jal/db/country.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/db/db.py` & `jal-2023.4.8/jal/db/db.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/db/helpers.py` & `jal-2023.4.8/jal/db/helpers.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/db/holdings_model.py` & `jal-2023.4.8/jal/db/holdings_model.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/db/ledger.py` & `jal-2023.4.8/jal/db/ledger.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/db/operations.py` & `jal-2023.4.8/jal/db/operations.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/db/operations_model.py` & `jal-2023.4.8/jal/db/operations_model.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/db/peer.py` & `jal-2023.4.8/jal/db/peer.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/db/reference_models.py` & `jal-2023.4.8/jal/db/reference_models.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/db/settings.py` & `jal-2023.4.8/jal/db/settings.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/db/tax_estimator.py` & `jal-2023.4.8/jal/db/tax_estimator.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/db/view_model.py` & `jal-2023.4.8/jal/db/view_model.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/img/accept.png` & `jal-2023.4.8/jal/img/accept.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/img/add.png` & `jal-2023.4.8/jal/img/add.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/img/add_child.png` & `jal-2023.4.8/jal/img/add_child.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/img/cancel.png` & `jal-2023.4.8/jal/img/cancel.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/img/chart.png` & `jal-2023.4.8/jal/img/chart.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/img/copy.png` & `jal-2023.4.8/jal/img/copy.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/img/delete.png` & `jal-2023.4.8/jal/img/delete.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/img/ibkr.png` & `jal-2023.4.8/jal/img/ibkr.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/img/j2t.png` & `jal-2023.4.8/jal/img/j2t.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/img/jal.png` & `jal-2023.4.8/jal/img/jal.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/img/kit.png` & `jal-2023.4.8/jal/img/kit.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/img/list.png` & `jal-2023.4.8/jal/img/list.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/img/new.png` & `jal-2023.4.8/jal/img/new.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/img/open_portfolio.png` & `jal-2023.4.8/jal/img/open_portfolio.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/img/openbroker.ico` & `jal-2023.4.8/jal/img/openbroker.ico`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/img/psb.ico` & `jal-2023.4.8/jal/img/psb.ico`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/img/quik.ico` & `jal-2023.4.8/jal/img/quik.ico`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/img/reconcile.png` & `jal-2023.4.8/jal/img/reconcile.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/img/remove.png` & `jal-2023.4.8/jal/img/remove.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/img/tax.png` & `jal-2023.4.8/jal/img/tax.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/img/uralsib.ico` & `jal-2023.4.8/jal/img/uralsib.ico`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/jal.py` & `jal-2023.4.8/jal/jal.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/jal_init.sql` & `jal-2023.4.8/jal/jal_init.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/languages/en.qm` & `jal-2023.4.8/jal/languages/en.qm`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/languages/ru.qm` & `jal-2023.4.8/jal/languages/ru.qm`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/net/downloader.py` & `jal-2023.4.8/jal/net/downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -319,14 +319,20 @@
                     x[columns.index('regnumber')] == kwargs['reg_number'] or x[columns.index('regnumber')] is None]
         if not data and 'isin' in kwargs:
             url = f"https://iss.moex.com/iss/securities.json?q={kwargs['isin']}&iss.meta=off&limit=10"
             asset_data = json.loads(get_web_data(url))
             securities = asset_data['securities']
             columns = securities['columns']
             data = securities['data']  # take the whole list if we search by isin
+        if not data and 'name' in kwargs:
+            url = f"https://iss.moex.com/iss/securities.json?q={kwargs['name']}&iss.meta=off&limit=10"
+            asset_data = json.loads(get_web_data(url))
+            securities = asset_data['securities']
+            columns = securities['columns']
+            data = [x for x in securities['data'] if x[columns.index('name')] == kwargs['name']]
         if data:
             if len(data) > 1:
                 # remove not traded assets if there are any outdated doubles present
                 data = [x for x in data if x[columns.index('is_traded')] == 1]
             if len(data) > 1:  # and then check again
                 logging.info(QApplication.translate("MOEX", "Multiple MOEX assets found for: ") + f"{kwargs}")
                 return secid
```

### Comparing `jal-2023.4.7/jal/net/helpers.py` & `jal-2023.4.8/jal/net/helpers.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/pypi_description.md` & `jal-2023.4.8/jal/pypi_description.md`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/reports/category.py` & `jal-2023.4.8/jal/reports/category.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/reports/deals.py` & `jal-2023.4.8/jal/reports/deals.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/reports/holdings.py` & `jal-2023.4.8/jal/reports/holdings.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/reports/income_spending.py` & `jal-2023.4.8/jal/reports/income_spending.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/reports/peer.py` & `jal-2023.4.8/jal/reports/peer.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/reports/profit_loss.py` & `jal-2023.4.8/jal/reports/profit_loss.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/reports/reports.py` & `jal-2023.4.8/jal/reports/reports.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/reports/tag.py` & `jal-2023.4.8/jal/reports/tag.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/ui/reports/ui_category_report.py` & `jal-2023.4.8/jal/ui/reports/ui_category_report.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/ui/reports/ui_deals_report.py` & `jal-2023.4.8/jal/ui/reports/ui_deals_report.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/ui/reports/ui_holdings_report.py` & `jal-2023.4.8/jal/ui/reports/ui_holdings_report.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/ui/reports/ui_income_spending_report.py` & `jal-2023.4.8/jal/ui/reports/ui_income_spending_report.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/ui/reports/ui_peer_report.py` & `jal-2023.4.8/jal/ui/reports/ui_peer_report.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/ui/reports/ui_profit_loss_report.py` & `jal-2023.4.8/jal/ui/reports/ui_profit_loss_report.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/ui/reports/ui_tag_report.py` & `jal-2023.4.8/jal/ui/reports/ui_tag_report.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/ui/reports/ui_tax_estimation.py` & `jal-2023.4.8/jal/ui/reports/ui_tax_estimation.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/ui/ui_asset_dlg.py` & `jal-2023.4.8/jal/ui/ui_asset_dlg.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/ui/ui_flow_export_widget.py` & `jal-2023.4.8/jal/ui/ui_flow_export_widget.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/ui/ui_login_fns_dlg.py` & `jal-2023.4.8/jal/ui/ui_login_fns_dlg.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/ui/ui_main_window.py` & `jal-2023.4.8/jal/ui/ui_main_window.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/ui/ui_operations_widget.py` & `jal-2023.4.8/jal/ui/ui_operations_widget.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/ui/ui_rebuild_window.py` & `jal-2023.4.8/jal/ui/ui_rebuild_window.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/ui/ui_reference_data_dlg.py` & `jal-2023.4.8/jal/ui/ui_reference_data_dlg.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/ui/ui_select_account_dlg.py` & `jal-2023.4.8/jal/ui/ui_select_account_dlg.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/ui/ui_select_reference_dlg.py` & `jal-2023.4.8/jal/ui/ui_select_reference_dlg.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/ui/ui_slip_import_dlg.py` & `jal-2023.4.8/jal/ui/ui_slip_import_dlg.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/ui/ui_tax_export_widget.py` & `jal-2023.4.8/jal/ui/ui_tax_export_widget.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/ui/ui_update_quotes_window.py` & `jal-2023.4.8/jal/ui/ui_update_quotes_window.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/updates/jal_delta_10.sql` & `jal-2023.4.8/jal/updates/jal_delta_10.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/updates/jal_delta_11.sql` & `jal-2023.4.8/jal/updates/jal_delta_11.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/updates/jal_delta_12.sql` & `jal-2023.4.8/jal/updates/jal_delta_12.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/updates/jal_delta_13.sql` & `jal-2023.4.8/jal/updates/jal_delta_13.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/updates/jal_delta_14.sql` & `jal-2023.4.8/jal/updates/jal_delta_14.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/updates/jal_delta_15.sql` & `jal-2023.4.8/jal/updates/jal_delta_15.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/updates/jal_delta_16.sql` & `jal-2023.4.8/jal/updates/jal_delta_16.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/updates/jal_delta_17.sql` & `jal-2023.4.8/jal/updates/jal_delta_17.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/updates/jal_delta_18.sql` & `jal-2023.4.8/jal/updates/jal_delta_18.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/updates/jal_delta_19.sql` & `jal-2023.4.8/jal/updates/jal_delta_19.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/updates/jal_delta_20.sql` & `jal-2023.4.8/jal/updates/jal_delta_20.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/updates/jal_delta_21.sql` & `jal-2023.4.8/jal/updates/jal_delta_21.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/updates/jal_delta_22.sql` & `jal-2023.4.8/jal/updates/jal_delta_22.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/updates/jal_delta_23.sql` & `jal-2023.4.8/jal/updates/jal_delta_23.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/updates/jal_delta_25.sql` & `jal-2023.4.8/jal/updates/jal_delta_25.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/updates/jal_delta_26.sql` & `jal-2023.4.8/jal/updates/jal_delta_26.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/updates/jal_delta_27.sql` & `jal-2023.4.8/jal/updates/jal_delta_27.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/updates/jal_delta_28.sql` & `jal-2023.4.8/jal/updates/jal_delta_28.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/updates/jal_delta_29.sql` & `jal-2023.4.8/jal/updates/jal_delta_29.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/updates/jal_delta_30.sql` & `jal-2023.4.8/jal/updates/jal_delta_30.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/updates/jal_delta_31.sql` & `jal-2023.4.8/jal/updates/jal_delta_31.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/updates/jal_delta_32.sql` & `jal-2023.4.8/jal/updates/jal_delta_32.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/updates/jal_delta_33.sql` & `jal-2023.4.8/jal/updates/jal_delta_33.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/updates/jal_delta_34.sql` & `jal-2023.4.8/jal/updates/jal_delta_34.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/updates/jal_delta_35.sql` & `jal-2023.4.8/jal/updates/jal_delta_35.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/updates/jal_delta_36.sql` & `jal-2023.4.8/jal/updates/jal_delta_36.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/updates/jal_delta_37.sql` & `jal-2023.4.8/jal/updates/jal_delta_37.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/updates/jal_delta_38.sql` & `jal-2023.4.8/jal/updates/jal_delta_38.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/updates/jal_delta_40.sql` & `jal-2023.4.8/jal/updates/jal_delta_40.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/updates/jal_delta_41.sql` & `jal-2023.4.8/jal/updates/jal_delta_41.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/updates/jal_delta_42.sql` & `jal-2023.4.8/jal/updates/jal_delta_42.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/updates/jal_delta_43.sql` & `jal-2023.4.8/jal/updates/jal_delta_43.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/updates/jal_delta_44.sql` & `jal-2023.4.8/jal/updates/jal_delta_44.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/widgets/abstract_operation_details.py` & `jal-2023.4.8/jal/widgets/abstract_operation_details.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/widgets/account_select.py` & `jal-2023.4.8/jal/widgets/account_select.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/widgets/asset_dialog.py` & `jal-2023.4.8/jal/widgets/asset_dialog.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/widgets/corporate_action_widget.py` & `jal-2023.4.8/jal/widgets/corporate_action_widget.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/widgets/custom/date_range_selector.py` & `jal-2023.4.8/jal/widgets/custom/date_range_selector.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/widgets/custom/db_lookup_combobox.py` & `jal-2023.4.8/jal/widgets/custom/db_lookup_combobox.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/widgets/custom/log_viewer.py` & `jal-2023.4.8/jal/widgets/custom/log_viewer.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/widgets/delegates.py` & `jal-2023.4.8/jal/widgets/delegates.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/widgets/dividend_widget.py` & `jal-2023.4.8/jal/widgets/dividend_widget.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/widgets/helpers.py` & `jal-2023.4.8/jal/widgets/helpers.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/widgets/income_spending_widget.py` & `jal-2023.4.8/jal/widgets/income_spending_widget.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/widgets/main_window.py` & `jal-2023.4.8/jal/widgets/main_window.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/widgets/mdi.py` & `jal-2023.4.8/jal/widgets/mdi.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/widgets/operations_tabs.py` & `jal-2023.4.8/jal/widgets/operations_tabs.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/widgets/operations_widget.py` & `jal-2023.4.8/jal/widgets/operations_widget.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/widgets/price_chart.py` & `jal-2023.4.8/jal/widgets/price_chart.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/widgets/qr_scanner.py` & `jal-2023.4.8/jal/widgets/qr_scanner.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/widgets/reference_data.py` & `jal-2023.4.8/jal/widgets/reference_data.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/widgets/reference_dialogs.py` & `jal-2023.4.8/jal/widgets/reference_dialogs.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/widgets/reference_selector.py` & `jal-2023.4.8/jal/widgets/reference_selector.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/widgets/register_designer_plugins.py` & `jal-2023.4.8/jal/widgets/register_designer_plugins.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/widgets/selection_dialog.py` & `jal-2023.4.8/jal/widgets/selection_dialog.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/widgets/tax_widget.py` & `jal-2023.4.8/jal/widgets/tax_widget.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/widgets/trade_widget.py` & `jal-2023.4.8/jal/widgets/trade_widget.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal/widgets/transfer_widget.py` & `jal-2023.4.8/jal/widgets/transfer_widget.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/jal.egg-info/PKG-INFO` & `jal-2023.4.8/jal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jal
-Version: 2023.4.7
+Version: 2023.4.8
 Summary: Just Another Ledger - project to track personal financial records
 Home-page: https://github.com/titov-vv/jal
 Author-email: jal@gmx.ru
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Topic :: Office/Business :: Financial :: Accounting
```

### Comparing `jal-2023.4.7/jal.egg-info/SOURCES.txt` & `jal-2023.4.8/jal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jal-2023.4.7/setup.py` & `jal-2023.4.8/setup.py`

 * *Files identical despite different names*

