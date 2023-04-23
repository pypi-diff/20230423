# Comparing `tmp/cy_widgets-0.4.8.tar.gz` & `tmp/cy_widgets-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cy_widgets-0.4.8.tar", last modified: Fri Jan 22 12:43:25 2021, max compression
+gzip compressed data, was "dist/cy_widgets-0.4.9.tar", last modified: Sat Jan 23 03:47:19 2021, max compression
```

## Comparing `cy_widgets-0.4.8.tar` & `cy_widgets-0.4.9.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 hyl        (501) staff       (20)        0 2021-01-22 12:43:25.000000 cy_widgets-0.4.8/
--rw-r--r--   0 hyl        (501) staff       (20)     3534 2020-03-02 09:55:11.000000 cy_widgets-0.4.8/CONTRIBUTING.rst
--rw-r--r--   0 hyl        (501) staff       (20)       89 2020-03-02 09:53:02.000000 cy_widgets-0.4.8/HISTORY.rst
--rw-r--r--   0 hyl        (501) staff       (20)     1067 2020-03-02 09:53:02.000000 cy_widgets-0.4.8/LICENSE
--rw-r--r--   0 hyl        (501) staff       (20)      267 2020-03-02 10:01:27.000000 cy_widgets-0.4.8/MANIFEST.in
--rw-r--r--   0 hyl        (501) staff       (20)      912 2021-01-22 12:43:25.000000 cy_widgets-0.4.8/PKG-INFO
--rw-r--r--   0 hyl        (501) staff       (20)      146 2020-07-09 15:55:18.000000 cy_widgets-0.4.8/README.rst
-drwxr-xr-x   0 hyl        (501) staff       (20)        0 2021-01-22 12:43:25.000000 cy_widgets-0.4.8/cy_widgets/
--rw-r--r--   0 hyl        (501) staff       (20)      278 2021-01-22 12:43:24.000000 cy_widgets-0.4.8/cy_widgets/__init__.py
-drwxr-xr-x   0 hyl        (501) staff       (20)        0 2021-01-22 12:43:25.000000 cy_widgets-0.4.8/cy_widgets/backtest/
--rw-r--r--   0 hyl        (501) staff       (20)        0 2020-07-17 02:19:38.000000 cy_widgets-0.4.8/cy_widgets/backtest/__init__.py
--rw-r--r--   0 hyl        (501) staff       (20)      340 2020-07-17 02:19:38.000000 cy_widgets-0.4.8/cy_widgets/backtest/helper.py
--rw-r--r--   0 hyl        (501) staff       (20)     1768 2021-01-20 02:28:43.000000 cy_widgets-0.4.8/cy_widgets/backtest/strategy.py
-drwxr-xr-x   0 hyl        (501) staff       (20)        0 2021-01-22 12:43:25.000000 cy_widgets-0.4.8/cy_widgets/charts/
--rw-r--r--   0 hyl        (501) staff       (20)        0 2020-12-28 03:56:42.000000 cy_widgets-0.4.8/cy_widgets/charts/__init__.py
--rw-r--r--   0 hyl        (501) staff       (20)    18114 2021-01-22 11:57:43.000000 cy_widgets-0.4.8/cy_widgets/charts/pyecharts.py
--rw-r--r--   0 hyl        (501) staff       (20)      408 2020-03-02 09:53:02.000000 cy_widgets-0.4.8/cy_widgets/cli.py
-drwxr-xr-x   0 hyl        (501) staff       (20)        0 2021-01-22 12:43:25.000000 cy_widgets-0.4.8/cy_widgets/exchange/
--rw-r--r--   0 hyl        (501) staff       (20)        0 2020-03-04 09:46:48.000000 cy_widgets-0.4.8/cy_widgets/exchange/__init__.py
--rw-r--r--   0 hyl        (501) staff       (20)     4535 2020-08-17 01:46:48.000000 cy_widgets-0.4.8/cy_widgets/exchange/order.py
--rw-r--r--   0 hyl        (501) staff       (20)     7083 2021-01-17 16:57:39.000000 cy_widgets-0.4.8/cy_widgets/exchange/provider.py
--rw-r--r--   0 hyl        (501) staff       (20)      291 2020-03-18 06:26:24.000000 cy_widgets-0.4.8/cy_widgets/exchange/signal.py
-drwxr-xr-x   0 hyl        (501) staff       (20)        0 2021-01-22 12:43:25.000000 cy_widgets-0.4.8/cy_widgets/fetcher/
--rw-r--r--   0 hyl        (501) staff       (20)        0 2020-03-03 07:48:36.000000 cy_widgets-0.4.8/cy_widgets/fetcher/__init__.py
--rw-r--r--   0 hyl        (501) staff       (20)     4516 2021-01-17 13:44:32.000000 cy_widgets-0.4.8/cy_widgets/fetcher/exchange.py
-drwxr-xr-x   0 hyl        (501) staff       (20)        0 2021-01-22 12:43:25.000000 cy_widgets-0.4.8/cy_widgets/logger/
--rw-r--r--   0 hyl        (501) staff       (20)        0 2020-03-02 10:09:23.000000 cy_widgets-0.4.8/cy_widgets/logger/__init__.py
--rw-r--r--   0 hyl        (501) staff       (20)     1437 2020-08-22 18:05:18.000000 cy_widgets-0.4.8/cy_widgets/logger/base.py
--rw-r--r--   0 hyl        (501) staff       (20)     1566 2020-08-16 14:33:22.000000 cy_widgets-0.4.8/cy_widgets/logger/trading.py
-drwxr-xr-x   0 hyl        (501) staff       (20)        0 2021-01-22 12:43:25.000000 cy_widgets-0.4.8/cy_widgets/strategy/
--rw-r--r--   0 hyl        (501) staff       (20)        0 2020-03-18 10:20:05.000000 cy_widgets-0.4.8/cy_widgets/strategy/__init__.py
--rw-r--r--   0 hyl        (501) staff       (20)    13858 2021-01-19 06:55:53.000000 cy_widgets-0.4.8/cy_widgets/strategy/evaluation.py
-drwxr-xr-x   0 hyl        (501) staff       (20)        0 2021-01-22 12:43:25.000000 cy_widgets-0.4.8/cy_widgets/strategy/exchange/
--rw-r--r--   0 hyl        (501) staff       (20)      238 2021-01-20 07:00:16.000000 cy_widgets-0.4.8/cy_widgets/strategy/exchange/__init__.py
--rw-r--r--   0 hyl        (501) staff       (20)    21299 2021-01-09 08:05:09.000000 cy_widgets-0.4.8/cy_widgets/strategy/exchange/aberration_flash_bolling.py
--rw-r--r--   0 hyl        (501) staff       (20)     3730 2021-01-09 08:05:09.000000 cy_widgets-0.4.8/cy_widgets/strategy/exchange/aims.py
--rw-r--r--   0 hyl        (501) staff       (20)     2549 2021-01-09 08:05:09.000000 cy_widgets-0.4.8/cy_widgets/strategy/exchange/autobuy.py
--rw-r--r--   0 hyl        (501) staff       (20)     6563 2021-01-19 03:36:03.000000 cy_widgets-0.4.8/cy_widgets/strategy/exchange/base.py
--rw-r--r--   0 hyl        (501) staff       (20)     3921 2021-01-21 13:26:26.000000 cy_widgets-0.4.8/cy_widgets/strategy/exchange/bolling.py
--rw-r--r--   0 hyl        (501) staff       (20)     3088 2021-01-22 12:27:45.000000 cy_widgets-0.4.8/cy_widgets/strategy/exchange/ice_ma_shrinkage.py
--rw-r--r--   0 hyl        (501) staff       (20)     6650 2021-01-19 03:40:04.000000 cy_widgets-0.4.8/cy_widgets/strategy/exchange/mtm_adapt_bolling.py
--rw-r--r--   0 hyl        (501) staff       (20)     4886 2021-01-09 08:05:09.000000 cy_widgets-0.4.8/cy_widgets/strategy/exchange/rsi.py
--rw-r--r--   0 hyl        (501) staff       (20)     4090 2021-01-19 11:56:06.000000 cy_widgets-0.4.8/cy_widgets/strategy/exchange/sb_atr_bolling.py
--rw-r--r--   0 hyl        (501) staff       (20)     5146 2021-01-19 07:12:49.000000 cy_widgets-0.4.8/cy_widgets/strategy/exchange/sb_ma_gap_bolling.py
--rw-r--r--   0 hyl        (501) staff       (20)     2839 2021-01-20 06:59:03.000000 cy_widgets-0.4.8/cy_widgets/strategy/exchange/vix_bolling.py
-drwxr-xr-x   0 hyl        (501) staff       (20)        0 2021-01-22 12:43:25.000000 cy_widgets-0.4.8/cy_widgets/strategy/neutral/
--rw-r--r--   0 hyl        (501) staff       (20)       51 2021-01-17 16:57:39.000000 cy_widgets-0.4.8/cy_widgets/strategy/neutral/__init__.py
--rw-r--r--   0 hyl        (501) staff       (20)     4635 2021-01-18 15:47:04.000000 cy_widgets-0.4.8/cy_widgets/strategy/neutral/base.py
--rw-r--r--   0 hyl        (501) staff       (20)     4010 2021-01-18 15:47:04.000000 cy_widgets-0.4.8/cy_widgets/strategy/neutral/binance_neutral.py
--rw-r--r--   0 hyl        (501) staff       (20)      724 2020-12-28 03:56:42.000000 cy_widgets-0.4.8/cy_widgets/strategy/position.py
-drwxr-xr-x   0 hyl        (501) staff       (20)        0 2021-01-22 12:43:25.000000 cy_widgets-0.4.8/cy_widgets/trader/
--rw-r--r--   0 hyl        (501) staff       (20)        0 2020-03-03 07:48:49.000000 cy_widgets-0.4.8/cy_widgets/trader/__init__.py
--rw-r--r--   0 hyl        (501) staff       (20)    11649 2020-08-22 18:05:18.000000 cy_widgets-0.4.8/cy_widgets/trader/exchange_order_exec.py
--rw-r--r--   0 hyl        (501) staff       (20)     1950 2020-06-29 09:42:26.000000 cy_widgets-0.4.8/cy_widgets/trader/exchange_trader.py
-drwxr-xr-x   0 hyl        (501) staff       (20)        0 2021-01-22 12:43:25.000000 cy_widgets-0.4.8/cy_widgets.egg-info/
--rw-r--r--   0 hyl        (501) staff       (20)      912 2021-01-22 12:43:25.000000 cy_widgets-0.4.8/cy_widgets.egg-info/PKG-INFO
--rw-r--r--   0 hyl        (501) staff       (20)     1865 2021-01-22 12:43:25.000000 cy_widgets-0.4.8/cy_widgets.egg-info/SOURCES.txt
--rw-r--r--   0 hyl        (501) staff       (20)        1 2021-01-22 12:43:25.000000 cy_widgets-0.4.8/cy_widgets.egg-info/dependency_links.txt
--rw-r--r--   0 hyl        (501) staff       (20)       52 2021-01-22 12:43:25.000000 cy_widgets-0.4.8/cy_widgets.egg-info/entry_points.txt
--rw-r--r--   0 hyl        (501) staff       (20)        1 2020-03-30 09:47:18.000000 cy_widgets-0.4.8/cy_widgets.egg-info/not-zip-safe
--rw-r--r--   0 hyl        (501) staff       (20)       71 2021-01-22 12:43:25.000000 cy_widgets-0.4.8/cy_widgets.egg-info/requires.txt
--rw-r--r--   0 hyl        (501) staff       (20)       11 2021-01-22 12:43:25.000000 cy_widgets-0.4.8/cy_widgets.egg-info/top_level.txt
-drwxr-xr-x   0 hyl        (501) staff       (20)        0 2021-01-22 12:43:25.000000 cy_widgets-0.4.8/docs/
--rw-r--r--   0 hyl        (501) staff       (20)      611 2020-03-02 09:53:02.000000 cy_widgets-0.4.8/docs/Makefile
--rwxr-xr-x   0 hyl        (501) staff       (20)     4805 2020-03-02 09:53:02.000000 cy_widgets-0.4.8/docs/conf.py
--rw-r--r--   0 hyl        (501) staff       (20)       33 2020-03-02 09:53:02.000000 cy_widgets-0.4.8/docs/contributing.rst
--rw-r--r--   0 hyl        (501) staff       (20)       28 2020-03-02 09:53:02.000000 cy_widgets-0.4.8/docs/history.rst
--rw-r--r--   0 hyl        (501) staff       (20)      296 2020-03-02 09:53:02.000000 cy_widgets-0.4.8/docs/index.rst
--rw-r--r--   0 hyl        (501) staff       (20)     1130 2020-03-02 09:53:02.000000 cy_widgets-0.4.8/docs/installation.rst
--rw-r--r--   0 hyl        (501) staff       (20)      772 2020-03-02 09:53:02.000000 cy_widgets-0.4.8/docs/make.bat
--rw-r--r--   0 hyl        (501) staff       (20)       27 2020-03-02 09:53:02.000000 cy_widgets-0.4.8/docs/readme.rst
--rw-r--r--   0 hyl        (501) staff       (20)       75 2020-03-02 09:53:02.000000 cy_widgets-0.4.8/docs/usage.rst
--rw-r--r--   0 hyl        (501) staff       (20)       59 2020-12-28 03:56:42.000000 cy_widgets-0.4.8/requirements.txt
--rw-r--r--   0 hyl        (501) staff       (20)      452 2021-01-22 12:43:25.000000 cy_widgets-0.4.8/setup.cfg
--rw-r--r--   0 hyl        (501) staff       (20)     1498 2021-01-22 12:43:24.000000 cy_widgets-0.4.8/setup.py
-drwxr-xr-x   0 hyl        (501) staff       (20)        0 2021-01-22 12:43:25.000000 cy_widgets-0.4.8/tests/
--rw-r--r--   0 hyl        (501) staff       (20)       40 2020-03-02 09:53:02.000000 cy_widgets-0.4.8/tests/__init__.py
--rw-r--r--   0 hyl        (501) staff       (20)     9419 2021-01-20 06:45:52.000000 cy_widgets-0.4.8/tests/test.ipynb
--rw-r--r--   0 hyl        (501) staff       (20)      994 2020-03-02 09:53:02.000000 cy_widgets-0.4.8/tests/test_cy_widgets.py
+drwxr-xr-x   0 hyl        (501) staff       (20)        0 2021-01-23 03:47:19.000000 cy_widgets-0.4.9/
+-rw-r--r--   0 hyl        (501) staff       (20)     3534 2020-03-02 09:55:11.000000 cy_widgets-0.4.9/CONTRIBUTING.rst
+-rw-r--r--   0 hyl        (501) staff       (20)       89 2020-03-02 09:53:02.000000 cy_widgets-0.4.9/HISTORY.rst
+-rw-r--r--   0 hyl        (501) staff       (20)     1067 2020-03-02 09:53:02.000000 cy_widgets-0.4.9/LICENSE
+-rw-r--r--   0 hyl        (501) staff       (20)      267 2020-03-02 10:01:27.000000 cy_widgets-0.4.9/MANIFEST.in
+-rw-r--r--   0 hyl        (501) staff       (20)      912 2021-01-23 03:47:19.000000 cy_widgets-0.4.9/PKG-INFO
+-rw-r--r--   0 hyl        (501) staff       (20)      146 2020-07-09 15:55:18.000000 cy_widgets-0.4.9/README.rst
+drwxr-xr-x   0 hyl        (501) staff       (20)        0 2021-01-23 03:47:19.000000 cy_widgets-0.4.9/cy_widgets/
+-rw-r--r--   0 hyl        (501) staff       (20)      278 2021-01-23 03:47:17.000000 cy_widgets-0.4.9/cy_widgets/__init__.py
+drwxr-xr-x   0 hyl        (501) staff       (20)        0 2021-01-23 03:47:19.000000 cy_widgets-0.4.9/cy_widgets/backtest/
+-rw-r--r--   0 hyl        (501) staff       (20)        0 2020-07-17 02:19:38.000000 cy_widgets-0.4.9/cy_widgets/backtest/__init__.py
+-rw-r--r--   0 hyl        (501) staff       (20)      340 2020-07-17 02:19:38.000000 cy_widgets-0.4.9/cy_widgets/backtest/helper.py
+-rw-r--r--   0 hyl        (501) staff       (20)     1768 2021-01-20 02:28:43.000000 cy_widgets-0.4.9/cy_widgets/backtest/strategy.py
+drwxr-xr-x   0 hyl        (501) staff       (20)        0 2021-01-23 03:47:19.000000 cy_widgets-0.4.9/cy_widgets/charts/
+-rw-r--r--   0 hyl        (501) staff       (20)        0 2020-12-28 03:56:42.000000 cy_widgets-0.4.9/cy_widgets/charts/__init__.py
+-rw-r--r--   0 hyl        (501) staff       (20)    18114 2021-01-22 12:43:49.000000 cy_widgets-0.4.9/cy_widgets/charts/pyecharts.py
+-rw-r--r--   0 hyl        (501) staff       (20)      408 2020-03-02 09:53:02.000000 cy_widgets-0.4.9/cy_widgets/cli.py
+drwxr-xr-x   0 hyl        (501) staff       (20)        0 2021-01-23 03:47:19.000000 cy_widgets-0.4.9/cy_widgets/exchange/
+-rw-r--r--   0 hyl        (501) staff       (20)        0 2020-03-04 09:46:48.000000 cy_widgets-0.4.9/cy_widgets/exchange/__init__.py
+-rw-r--r--   0 hyl        (501) staff       (20)     4535 2020-08-17 01:46:48.000000 cy_widgets-0.4.9/cy_widgets/exchange/order.py
+-rw-r--r--   0 hyl        (501) staff       (20)     7083 2021-01-17 16:57:39.000000 cy_widgets-0.4.9/cy_widgets/exchange/provider.py
+-rw-r--r--   0 hyl        (501) staff       (20)      291 2020-03-18 06:26:24.000000 cy_widgets-0.4.9/cy_widgets/exchange/signal.py
+drwxr-xr-x   0 hyl        (501) staff       (20)        0 2021-01-23 03:47:19.000000 cy_widgets-0.4.9/cy_widgets/fetcher/
+-rw-r--r--   0 hyl        (501) staff       (20)        0 2020-03-03 07:48:36.000000 cy_widgets-0.4.9/cy_widgets/fetcher/__init__.py
+-rw-r--r--   0 hyl        (501) staff       (20)     4784 2021-01-23 03:33:49.000000 cy_widgets-0.4.9/cy_widgets/fetcher/exchange.py
+drwxr-xr-x   0 hyl        (501) staff       (20)        0 2021-01-23 03:47:19.000000 cy_widgets-0.4.9/cy_widgets/logger/
+-rw-r--r--   0 hyl        (501) staff       (20)        0 2020-03-02 10:09:23.000000 cy_widgets-0.4.9/cy_widgets/logger/__init__.py
+-rw-r--r--   0 hyl        (501) staff       (20)     1437 2020-08-22 18:05:18.000000 cy_widgets-0.4.9/cy_widgets/logger/base.py
+-rw-r--r--   0 hyl        (501) staff       (20)     1566 2020-08-16 14:33:22.000000 cy_widgets-0.4.9/cy_widgets/logger/trading.py
+drwxr-xr-x   0 hyl        (501) staff       (20)        0 2021-01-23 03:47:19.000000 cy_widgets-0.4.9/cy_widgets/strategy/
+-rw-r--r--   0 hyl        (501) staff       (20)        0 2020-03-18 10:20:05.000000 cy_widgets-0.4.9/cy_widgets/strategy/__init__.py
+-rw-r--r--   0 hyl        (501) staff       (20)    13858 2021-01-22 12:43:49.000000 cy_widgets-0.4.9/cy_widgets/strategy/evaluation.py
+drwxr-xr-x   0 hyl        (501) staff       (20)        0 2021-01-23 03:47:19.000000 cy_widgets-0.4.9/cy_widgets/strategy/exchange/
+-rw-r--r--   0 hyl        (501) staff       (20)      238 2021-01-22 12:43:49.000000 cy_widgets-0.4.9/cy_widgets/strategy/exchange/__init__.py
+-rw-r--r--   0 hyl        (501) staff       (20)    21299 2021-01-09 08:05:09.000000 cy_widgets-0.4.9/cy_widgets/strategy/exchange/aberration_flash_bolling.py
+-rw-r--r--   0 hyl        (501) staff       (20)     3730 2021-01-09 08:05:09.000000 cy_widgets-0.4.9/cy_widgets/strategy/exchange/aims.py
+-rw-r--r--   0 hyl        (501) staff       (20)     2549 2021-01-09 08:05:09.000000 cy_widgets-0.4.9/cy_widgets/strategy/exchange/autobuy.py
+-rw-r--r--   0 hyl        (501) staff       (20)     6563 2021-01-22 12:43:49.000000 cy_widgets-0.4.9/cy_widgets/strategy/exchange/base.py
+-rw-r--r--   0 hyl        (501) staff       (20)     3921 2021-01-21 13:26:26.000000 cy_widgets-0.4.9/cy_widgets/strategy/exchange/bolling.py
+-rw-r--r--   0 hyl        (501) staff       (20)     3092 2021-01-23 03:08:49.000000 cy_widgets-0.4.9/cy_widgets/strategy/exchange/ice_ma_shrinkage.py
+-rw-r--r--   0 hyl        (501) staff       (20)     6650 2021-01-19 03:40:04.000000 cy_widgets-0.4.9/cy_widgets/strategy/exchange/mtm_adapt_bolling.py
+-rw-r--r--   0 hyl        (501) staff       (20)     4886 2021-01-09 08:05:09.000000 cy_widgets-0.4.9/cy_widgets/strategy/exchange/rsi.py
+-rw-r--r--   0 hyl        (501) staff       (20)     4090 2021-01-22 12:43:49.000000 cy_widgets-0.4.9/cy_widgets/strategy/exchange/sb_atr_bolling.py
+-rw-r--r--   0 hyl        (501) staff       (20)     5146 2021-01-22 12:43:49.000000 cy_widgets-0.4.9/cy_widgets/strategy/exchange/sb_ma_gap_bolling.py
+-rw-r--r--   0 hyl        (501) staff       (20)     2839 2021-01-22 12:43:49.000000 cy_widgets-0.4.9/cy_widgets/strategy/exchange/vix_bolling.py
+drwxr-xr-x   0 hyl        (501) staff       (20)        0 2021-01-23 03:47:19.000000 cy_widgets-0.4.9/cy_widgets/strategy/neutral/
+-rw-r--r--   0 hyl        (501) staff       (20)       51 2021-01-17 16:57:39.000000 cy_widgets-0.4.9/cy_widgets/strategy/neutral/__init__.py
+-rw-r--r--   0 hyl        (501) staff       (20)     4635 2021-01-18 15:47:04.000000 cy_widgets-0.4.9/cy_widgets/strategy/neutral/base.py
+-rw-r--r--   0 hyl        (501) staff       (20)     4010 2021-01-18 15:47:04.000000 cy_widgets-0.4.9/cy_widgets/strategy/neutral/binance_neutral.py
+-rw-r--r--   0 hyl        (501) staff       (20)      724 2020-12-28 03:56:42.000000 cy_widgets-0.4.9/cy_widgets/strategy/position.py
+drwxr-xr-x   0 hyl        (501) staff       (20)        0 2021-01-23 03:47:19.000000 cy_widgets-0.4.9/cy_widgets/trader/
+-rw-r--r--   0 hyl        (501) staff       (20)        0 2020-03-03 07:48:49.000000 cy_widgets-0.4.9/cy_widgets/trader/__init__.py
+-rw-r--r--   0 hyl        (501) staff       (20)    11649 2020-08-22 18:05:18.000000 cy_widgets-0.4.9/cy_widgets/trader/exchange_order_exec.py
+-rw-r--r--   0 hyl        (501) staff       (20)     1950 2020-06-29 09:42:26.000000 cy_widgets-0.4.9/cy_widgets/trader/exchange_trader.py
+drwxr-xr-x   0 hyl        (501) staff       (20)        0 2021-01-23 03:47:19.000000 cy_widgets-0.4.9/cy_widgets.egg-info/
+-rw-r--r--   0 hyl        (501) staff       (20)      912 2021-01-23 03:47:19.000000 cy_widgets-0.4.9/cy_widgets.egg-info/PKG-INFO
+-rw-r--r--   0 hyl        (501) staff       (20)     1865 2021-01-23 03:47:19.000000 cy_widgets-0.4.9/cy_widgets.egg-info/SOURCES.txt
+-rw-r--r--   0 hyl        (501) staff       (20)        1 2021-01-23 03:47:19.000000 cy_widgets-0.4.9/cy_widgets.egg-info/dependency_links.txt
+-rw-r--r--   0 hyl        (501) staff       (20)       52 2021-01-23 03:47:19.000000 cy_widgets-0.4.9/cy_widgets.egg-info/entry_points.txt
+-rw-r--r--   0 hyl        (501) staff       (20)        1 2020-03-30 09:47:18.000000 cy_widgets-0.4.9/cy_widgets.egg-info/not-zip-safe
+-rw-r--r--   0 hyl        (501) staff       (20)       71 2021-01-23 03:47:19.000000 cy_widgets-0.4.9/cy_widgets.egg-info/requires.txt
+-rw-r--r--   0 hyl        (501) staff       (20)       11 2021-01-23 03:47:19.000000 cy_widgets-0.4.9/cy_widgets.egg-info/top_level.txt
+drwxr-xr-x   0 hyl        (501) staff       (20)        0 2021-01-23 03:47:19.000000 cy_widgets-0.4.9/docs/
+-rw-r--r--   0 hyl        (501) staff       (20)      611 2020-03-02 09:53:02.000000 cy_widgets-0.4.9/docs/Makefile
+-rwxr-xr-x   0 hyl        (501) staff       (20)     4805 2020-03-02 09:53:02.000000 cy_widgets-0.4.9/docs/conf.py
+-rw-r--r--   0 hyl        (501) staff       (20)       33 2020-03-02 09:53:02.000000 cy_widgets-0.4.9/docs/contributing.rst
+-rw-r--r--   0 hyl        (501) staff       (20)       28 2020-03-02 09:53:02.000000 cy_widgets-0.4.9/docs/history.rst
+-rw-r--r--   0 hyl        (501) staff       (20)      296 2020-03-02 09:53:02.000000 cy_widgets-0.4.9/docs/index.rst
+-rw-r--r--   0 hyl        (501) staff       (20)     1130 2020-03-02 09:53:02.000000 cy_widgets-0.4.9/docs/installation.rst
+-rw-r--r--   0 hyl        (501) staff       (20)      772 2020-03-02 09:53:02.000000 cy_widgets-0.4.9/docs/make.bat
+-rw-r--r--   0 hyl        (501) staff       (20)       27 2020-03-02 09:53:02.000000 cy_widgets-0.4.9/docs/readme.rst
+-rw-r--r--   0 hyl        (501) staff       (20)       75 2020-03-02 09:53:02.000000 cy_widgets-0.4.9/docs/usage.rst
+-rw-r--r--   0 hyl        (501) staff       (20)       59 2020-12-28 03:56:42.000000 cy_widgets-0.4.9/requirements.txt
+-rw-r--r--   0 hyl        (501) staff       (20)      452 2021-01-23 03:47:19.000000 cy_widgets-0.4.9/setup.cfg
+-rw-r--r--   0 hyl        (501) staff       (20)     1498 2021-01-23 03:47:17.000000 cy_widgets-0.4.9/setup.py
+drwxr-xr-x   0 hyl        (501) staff       (20)        0 2021-01-23 03:47:19.000000 cy_widgets-0.4.9/tests/
+-rw-r--r--   0 hyl        (501) staff       (20)       40 2020-03-02 09:53:02.000000 cy_widgets-0.4.9/tests/__init__.py
+-rw-r--r--   0 hyl        (501) staff       (20)     9419 2021-01-22 12:43:49.000000 cy_widgets-0.4.9/tests/test.ipynb
+-rw-r--r--   0 hyl        (501) staff       (20)      994 2020-03-02 09:53:02.000000 cy_widgets-0.4.9/tests/test_cy_widgets.py
```

### Comparing `cy_widgets-0.4.8/CONTRIBUTING.rst` & `cy_widgets-0.4.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cy_widgets-0.4.8/LICENSE` & `cy_widgets-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cy_widgets-0.4.8/PKG-INFO` & `cy_widgets-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: cy_widgets
-Version: 0.4.8
+Version: 0.4.9
 Summary: Widgets of quant app
 Home-page: https://github.com/cragod/CYWidgets
 Author: CY Gatro
 Author-email: cragodn@gmail.com
 License: MIT license
 Description: ==========
         CY Widgets
```

### Comparing `cy_widgets-0.4.8/cy_widgets/backtest/strategy.py` & `cy_widgets-0.4.9/cy_widgets/backtest/strategy.py`

 * *Files identical despite different names*

### Comparing `cy_widgets-0.4.8/cy_widgets/charts/pyecharts.py` & `cy_widgets-0.4.9/cy_widgets/charts/pyecharts.py`

 * *Files identical despite different names*

### Comparing `cy_widgets-0.4.8/cy_widgets/exchange/order.py` & `cy_widgets-0.4.9/cy_widgets/exchange/order.py`

 * *Files identical despite different names*

### Comparing `cy_widgets-0.4.8/cy_widgets/exchange/provider.py` & `cy_widgets-0.4.9/cy_widgets/exchange/provider.py`

 * *Files identical despite different names*

### Comparing `cy_widgets-0.4.8/cy_widgets/fetcher/exchange.py` & `cy_widgets-0.4.9/cy_widgets/fetcher/exchange.py`

 * *Files 7% similar despite different names*

```diff
@@ -87,16 +87,21 @@
             earliest_date = pd.datetime.now()
             if result_df is not None and result_df.shape[0] > 0:
                 earliest_date = result_df.iloc[0][COL_CANDLE_BEGIN_TIME]
 
             # fetch
             earliest_ts = int(time.mktime(earliest_date.timetuple()))
             fetch_ts = earliest_ts - fetch_lmt * time_frame.time_interval(res_unit='s')
+            # OKEx
             if self.__ccxt_provider.exchange_type == ExchangeType.Okex:
-                params['type'] = 'Candles'
+                if limit > 1000 and coin_pair.trade_coin.upper() in ['BTC', 'ETH', 'LTC', 'ETC', 'XRP', 'EOS', 'BCH', 'BSV', 'TRX']:
+                    params['type'] = 'HistoryCandles'
+                    fetch_lmt = 300
+                else:
+                    params['type'] = 'Candles'
             elif self.__ccxt_provider.exchange_type == ExchangeType.BinanceSpotFetching or self.__ccxt_provider.exchange_type == ExchangeType.Binance:
                 params['endTime'] = earliest_ts * 1000
             df = self.__fetch_candle_data_by_ccxt_object(
                 coin_pair, time_frame, fetch_ts * 1000, fetch_lmt, params)
 
             # update to df
             if result_df is None:
```

### Comparing `cy_widgets-0.4.8/cy_widgets/logger/base.py` & `cy_widgets-0.4.9/cy_widgets/logger/base.py`

 * *Files identical despite different names*

### Comparing `cy_widgets-0.4.8/cy_widgets/logger/trading.py` & `cy_widgets-0.4.9/cy_widgets/logger/trading.py`

 * *Files identical despite different names*

### Comparing `cy_widgets-0.4.8/cy_widgets/strategy/evaluation.py` & `cy_widgets-0.4.9/cy_widgets/strategy/evaluation.py`

 * *Files identical despite different names*

### Comparing `cy_widgets-0.4.8/cy_widgets/strategy/exchange/aberration_flash_bolling.py` & `cy_widgets-0.4.9/cy_widgets/strategy/exchange/aberration_flash_bolling.py`

 * *Files identical despite different names*

### Comparing `cy_widgets-0.4.8/cy_widgets/strategy/exchange/aims.py` & `cy_widgets-0.4.9/cy_widgets/strategy/exchange/aims.py`

 * *Files identical despite different names*

### Comparing `cy_widgets-0.4.8/cy_widgets/strategy/exchange/autobuy.py` & `cy_widgets-0.4.9/cy_widgets/strategy/exchange/autobuy.py`

 * *Files identical despite different names*

### Comparing `cy_widgets-0.4.8/cy_widgets/strategy/exchange/base.py` & `cy_widgets-0.4.9/cy_widgets/strategy/exchange/base.py`

 * *Files identical despite different names*

### Comparing `cy_widgets-0.4.8/cy_widgets/strategy/exchange/bolling.py` & `cy_widgets-0.4.9/cy_widgets/strategy/exchange/bolling.py`

 * *Files identical despite different names*

### Comparing `cy_widgets-0.4.8/cy_widgets/strategy/exchange/ice_ma_shrinkage.py` & `cy_widgets-0.4.9/cy_widgets/strategy/exchange/ice_ma_shrinkage.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     @property
     def name(self):
         """策略名"""
         return "IceMAShrinkage"
 
     @property
     def candle_count_for_calculating(self):
-        return max(self.long_ma, self.gap_ma) + 10
+        return max(self.long_ma, self.gap_ma) * 2 + 10
 
     def available_to_calculate(self, df):
         return df.shape[0] > self.candle_count_for_calculating and self.long_ma > self.short_ma
 
     def calculate_signals(self, df, drop_extra_columns=True):
         '''
         :param df:
```

### Comparing `cy_widgets-0.4.8/cy_widgets/strategy/exchange/mtm_adapt_bolling.py` & `cy_widgets-0.4.9/cy_widgets/strategy/exchange/mtm_adapt_bolling.py`

 * *Files identical despite different names*

### Comparing `cy_widgets-0.4.8/cy_widgets/strategy/exchange/rsi.py` & `cy_widgets-0.4.9/cy_widgets/strategy/exchange/rsi.py`

 * *Files identical despite different names*

### Comparing `cy_widgets-0.4.8/cy_widgets/strategy/exchange/sb_atr_bolling.py` & `cy_widgets-0.4.9/cy_widgets/strategy/exchange/sb_atr_bolling.py`

 * *Files identical despite different names*

### Comparing `cy_widgets-0.4.8/cy_widgets/strategy/exchange/sb_ma_gap_bolling.py` & `cy_widgets-0.4.9/cy_widgets/strategy/exchange/sb_ma_gap_bolling.py`

 * *Files identical despite different names*

### Comparing `cy_widgets-0.4.8/cy_widgets/strategy/exchange/vix_bolling.py` & `cy_widgets-0.4.9/cy_widgets/strategy/exchange/vix_bolling.py`

 * *Files identical despite different names*

### Comparing `cy_widgets-0.4.8/cy_widgets/strategy/neutral/base.py` & `cy_widgets-0.4.9/cy_widgets/strategy/neutral/base.py`

 * *Files identical despite different names*

### Comparing `cy_widgets-0.4.8/cy_widgets/strategy/neutral/binance_neutral.py` & `cy_widgets-0.4.9/cy_widgets/strategy/neutral/binance_neutral.py`

 * *Files identical despite different names*

### Comparing `cy_widgets-0.4.8/cy_widgets/strategy/position.py` & `cy_widgets-0.4.9/cy_widgets/strategy/position.py`

 * *Files identical despite different names*

### Comparing `cy_widgets-0.4.8/cy_widgets/trader/exchange_order_exec.py` & `cy_widgets-0.4.9/cy_widgets/trader/exchange_order_exec.py`

 * *Files identical despite different names*

### Comparing `cy_widgets-0.4.8/cy_widgets/trader/exchange_trader.py` & `cy_widgets-0.4.9/cy_widgets/trader/exchange_trader.py`

 * *Files identical despite different names*

### Comparing `cy_widgets-0.4.8/cy_widgets.egg-info/PKG-INFO` & `cy_widgets-0.4.9/cy_widgets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: cy-widgets
-Version: 0.4.8
+Version: 0.4.9
 Summary: Widgets of quant app
 Home-page: https://github.com/cragod/CYWidgets
 Author: CY Gatro
 Author-email: cragodn@gmail.com
 License: MIT license
 Description: ==========
         CY Widgets
```

### Comparing `cy_widgets-0.4.8/cy_widgets.egg-info/SOURCES.txt` & `cy_widgets-0.4.9/cy_widgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cy_widgets-0.4.8/docs/Makefile` & `cy_widgets-0.4.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cy_widgets-0.4.8/docs/conf.py` & `cy_widgets-0.4.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cy_widgets-0.4.8/docs/installation.rst` & `cy_widgets-0.4.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `cy_widgets-0.4.8/docs/make.bat` & `cy_widgets-0.4.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cy_widgets-0.4.8/setup.py` & `cy_widgets-0.4.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,10 +44,10 @@
     keywords='cy_widgets',
     name='cy_widgets',
     packages=find_packages(include=['cy_widgets', 'cy_widgets.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/cragod/CYWidgets',
-    version='0.4.8',
+    version='0.4.9',
     zip_safe=False,
 )
```

### Comparing `cy_widgets-0.4.8/tests/test.ipynb` & `cy_widgets-0.4.9/tests/test.ipynb`

 * *Files identical despite different names*

### Comparing `cy_widgets-0.4.8/tests/test_cy_widgets.py` & `cy_widgets-0.4.9/tests/test_cy_widgets.py`

 * *Files identical despite different names*

