# Comparing `tmp/lib-pybroker-1.1.3.tar.gz` & `tmp/lib-pybroker-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib-pybroker-1.1.3.tar", last modified: Tue Apr 11 08:38:33 2023, max compression
+gzip compressed data, was "lib-pybroker-1.1.4.tar", last modified: Sun Apr 23 21:17:14 2023, max compression
```

## Comparing `lib-pybroker-1.1.3.tar` & `lib-pybroker-1.1.4.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:38:33.521611 lib-pybroker-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    12318 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-04-11 08:38:33.521611 lib-pybroker-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-11 08:38:33.521611 lib-pybroker-1.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:38:33.509611 lib-pybroker-1.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:38:33.513611 lib-pybroker-1.1.3/src/lib_pybroker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-04-11 08:38:33.000000 lib-pybroker-1.1.3/src/lib_pybroker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-11 08:38:33.000000 lib-pybroker-1.1.3/src/lib_pybroker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:38:33.000000 lib-pybroker-1.1.3/src/lib_pybroker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-11 08:38:33.000000 lib-pybroker-1.1.3/src/lib_pybroker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-11 08:38:33.000000 lib-pybroker-1.1.3/src/lib_pybroker.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:38:33.517611 lib-pybroker-1.1.3/src/pybroker/
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/src/pybroker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7295 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/src/pybroker/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     9298 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/src/pybroker/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/src/pybroker/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    43490 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/src/pybroker/context.py
--rw-r--r--   0 runner    (1001) docker     (123)    19068 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/src/pybroker/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    34553 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/src/pybroker/eval.py
--rw-r--r--   0 runner    (1001) docker     (123)    15385 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/src/pybroker/indicator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15188 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/src/pybroker/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    15398 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/src/pybroker/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    38568 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/src/pybroker/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/src/pybroker/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    25106 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/src/pybroker/scope.py
--rw-r--r--   0 runner    (1001) docker     (123)    58263 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/src/pybroker/strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/src/pybroker/vect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:38:33.521611 lib-pybroker-1.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    21167 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    18142 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    18876 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/tests/test_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/tests/test_indicator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/tests/test_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    81106 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/tests/test_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)    16082 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/tests/test_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)    72675 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/tests/test_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/tests/test_vect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:17:14.525156 lib-pybroker-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    12318 2023-04-23 21:17:05.000000 lib-pybroker-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-23 21:17:05.000000 lib-pybroker-1.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5793 2023-04-23 21:17:14.525156 lib-pybroker-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-04-23 21:17:05.000000 lib-pybroker-1.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-23 21:17:05.000000 lib-pybroker-1.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-23 21:17:14.525156 lib-pybroker-1.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:17:14.517156 lib-pybroker-1.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:17:14.521156 lib-pybroker-1.1.4/src/lib_pybroker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5793 2023-04-23 21:17:14.000000 lib-pybroker-1.1.4/src/lib_pybroker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-23 21:17:14.000000 lib-pybroker-1.1.4/src/lib_pybroker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 21:17:14.000000 lib-pybroker-1.1.4/src/lib_pybroker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-23 21:17:14.000000 lib-pybroker-1.1.4/src/lib_pybroker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-23 21:17:14.000000 lib-pybroker-1.1.4/src/lib_pybroker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:17:14.521156 lib-pybroker-1.1.4/src/pybroker/
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-04-23 21:17:05.000000 lib-pybroker-1.1.4/src/pybroker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7295 2023-04-23 21:17:05.000000 lib-pybroker-1.1.4/src/pybroker/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9298 2023-04-23 21:17:05.000000 lib-pybroker-1.1.4/src/pybroker/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-04-23 21:17:05.000000 lib-pybroker-1.1.4/src/pybroker/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43490 2023-04-23 21:17:05.000000 lib-pybroker-1.1.4/src/pybroker/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19068 2023-04-23 21:17:05.000000 lib-pybroker-1.1.4/src/pybroker/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34553 2023-04-23 21:17:05.000000 lib-pybroker-1.1.4/src/pybroker/eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15385 2023-04-23 21:17:05.000000 lib-pybroker-1.1.4/src/pybroker/indicator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15188 2023-04-23 21:17:05.000000 lib-pybroker-1.1.4/src/pybroker/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15398 2023-04-23 21:17:05.000000 lib-pybroker-1.1.4/src/pybroker/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38568 2023-04-23 21:17:05.000000 lib-pybroker-1.1.4/src/pybroker/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 21:17:05.000000 lib-pybroker-1.1.4/src/pybroker/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25575 2023-04-23 21:17:05.000000 lib-pybroker-1.1.4/src/pybroker/scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58263 2023-04-23 21:17:05.000000 lib-pybroker-1.1.4/src/pybroker/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-04-23 21:17:05.000000 lib-pybroker-1.1.4/src/pybroker/vect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:17:14.525156 lib-pybroker-1.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-04-23 21:17:05.000000 lib-pybroker-1.1.4/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-04-23 21:17:05.000000 lib-pybroker-1.1.4/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21167 2023-04-23 21:17:05.000000 lib-pybroker-1.1.4/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18142 2023-04-23 21:17:05.000000 lib-pybroker-1.1.4/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18876 2023-04-23 21:17:05.000000 lib-pybroker-1.1.4/tests/test_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-04-23 21:17:05.000000 lib-pybroker-1.1.4/tests/test_indicator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-04-23 21:17:05.000000 lib-pybroker-1.1.4/tests/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-04-23 21:17:05.000000 lib-pybroker-1.1.4/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81106 2023-04-23 21:17:05.000000 lib-pybroker-1.1.4/tests/test_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16244 2023-04-23 21:17:05.000000 lib-pybroker-1.1.4/tests/test_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72675 2023-04-23 21:17:05.000000 lib-pybroker-1.1.4/tests/test_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-04-23 21:17:05.000000 lib-pybroker-1.1.4/tests/test_vect.py
```

### Comparing `lib-pybroker-1.1.3/LICENSE` & `lib-pybroker-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.3/PKG-INFO` & `lib-pybroker-1.1.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: lib-pybroker
-Version: 1.1.3
-Summary: Algorithmic trading with machine learning
-Home-page: http://www.pybroker.com
-Author: Edward West
-Author-email: edwest@pybroker.com
-License: Apache License 2.0 with Commons Clause
-Classifier: License :: Free for non-commercial use
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <h1>
     <img src="https://github.com/edtechre/pybroker/blob/master/docs/_static/pybroker-logo.png?raw=true" alt="PyBroker">
 </h1>
 
 ## Algorithmic Trading in Python with Machine Learning
 
 Are you looking to enhance your trading strategies with the power of Python and
@@ -67,16 +55,18 @@
       if ctx.bars < 20:
          return
       # Get the rolling 10 day high.
       high_10d = ctx.indicator('high_10d')
       # Buy on a new 10 day high.
       if not ctx.long_pos() and high_10d[-1] > high_10d[-2]:
          ctx.buy_shares = 100
-         # Hold the position for 2 days.
-         ctx.hold_bars = 2
+         # Hold the position for 5 days.
+         ctx.hold_bars = 5
+         # Set a stop loss of 2%.
+         ctx.stop_loss_pct = 2
 
    strategy = Strategy(YFinance(), start_date='1/1/2022', end_date='7/1/2022')
    strategy.add_execution(
       exec_fn, ['AAPL', 'MSFT'], indicators=highest('high_10d', 'close', period=10))
    result = strategy.backtest()
 ```
 
@@ -116,14 +106,15 @@
 - [Backtesting a Strategy](https://www.pybroker.com/en/latest/notebooks/2.%20Backtesting%20a%20Strategy.html)
 - [Evaluating with Bootstrap Metrics](https://www.pybroker.com/en/latest/notebooks/3.%20Evaluating%20with%20Bootstrap%20Metrics.html)
 - [Ranking and Position Sizing](https://www.pybroker.com/en/latest/notebooks/4.%20Ranking%20and%20Position%20Sizing.html)
 - [Writing Indicators](https://www.pybroker.com/en/latest/notebooks/5.%20Writing%20Indicators.html)
 - [Training a Model](https://www.pybroker.com/en/latest/notebooks/6.%20Training%20a%20Model.html)
 - [Creating a Custom Data Source](https://www.pybroker.com/en/latest/notebooks/7.%20Creating%20a%20Custom%20Data%20Source.html)
 - [Applying Stops](https://www.pybroker.com/en/latest/notebooks/8.%20Applying%20Stops.html)
+- [Rebalancing Positions](https://www.pybroker.com/en/latest/notebooks/9.%20Rebalancing%20Positions.html)
 - [FAQs](https://www.pybroker.com/en/latest/notebooks/FAQs.html)
 
 ## Online Documentation
 
 [The full reference documentation is hosted at **www.pybroker.com**.](https://www.pybroker.com)
 
 ## Contact
```

### Comparing `lib-pybroker-1.1.3/README.md` & `lib-pybroker-1.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: lib-pybroker
+Version: 1.1.4
+Summary: Algorithmic trading with machine learning
+Home-page: http://www.pybroker.com
+Author: Edward West
+Author-email: edwest@pybroker.com
+License: Apache License 2.0 with Commons Clause
+Classifier: License :: Free for non-commercial use
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <h1>
     <img src="https://github.com/edtechre/pybroker/blob/master/docs/_static/pybroker-logo.png?raw=true" alt="PyBroker">
 </h1>
 
 ## Algorithmic Trading in Python with Machine Learning
 
 Are you looking to enhance your trading strategies with the power of Python and
@@ -55,16 +67,18 @@
       if ctx.bars < 20:
          return
       # Get the rolling 10 day high.
       high_10d = ctx.indicator('high_10d')
       # Buy on a new 10 day high.
       if not ctx.long_pos() and high_10d[-1] > high_10d[-2]:
          ctx.buy_shares = 100
-         # Hold the position for 2 days.
-         ctx.hold_bars = 2
+         # Hold the position for 5 days.
+         ctx.hold_bars = 5
+         # Set a stop loss of 2%.
+         ctx.stop_loss_pct = 2
 
    strategy = Strategy(YFinance(), start_date='1/1/2022', end_date='7/1/2022')
    strategy.add_execution(
       exec_fn, ['AAPL', 'MSFT'], indicators=highest('high_10d', 'close', period=10))
    result = strategy.backtest()
 ```
 
@@ -104,14 +118,15 @@
 - [Backtesting a Strategy](https://www.pybroker.com/en/latest/notebooks/2.%20Backtesting%20a%20Strategy.html)
 - [Evaluating with Bootstrap Metrics](https://www.pybroker.com/en/latest/notebooks/3.%20Evaluating%20with%20Bootstrap%20Metrics.html)
 - [Ranking and Position Sizing](https://www.pybroker.com/en/latest/notebooks/4.%20Ranking%20and%20Position%20Sizing.html)
 - [Writing Indicators](https://www.pybroker.com/en/latest/notebooks/5.%20Writing%20Indicators.html)
 - [Training a Model](https://www.pybroker.com/en/latest/notebooks/6.%20Training%20a%20Model.html)
 - [Creating a Custom Data Source](https://www.pybroker.com/en/latest/notebooks/7.%20Creating%20a%20Custom%20Data%20Source.html)
 - [Applying Stops](https://www.pybroker.com/en/latest/notebooks/8.%20Applying%20Stops.html)
+- [Rebalancing Positions](https://www.pybroker.com/en/latest/notebooks/9.%20Rebalancing%20Positions.html)
 - [FAQs](https://www.pybroker.com/en/latest/notebooks/FAQs.html)
 
 ## Online Documentation
 
 [The full reference documentation is hosted at **www.pybroker.com**.](https://www.pybroker.com)
 
 ## Contact
```

### Comparing `lib-pybroker-1.1.3/setup.cfg` & `lib-pybroker-1.1.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lib-pybroker
-version = 1.1.3
+version = 1.1.4
 url = http://www.pybroker.com
 author = Edward West
 author_email = edwest@pybroker.com
 description = Algorithmic trading with machine learning
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = Apache License 2.0 with Commons Clause
```

### Comparing `lib-pybroker-1.1.3/src/lib_pybroker.egg-info/PKG-INFO` & `lib-pybroker-1.1.4/src/lib_pybroker.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-pybroker
-Version: 1.1.3
+Version: 1.1.4
 Summary: Algorithmic trading with machine learning
 Home-page: http://www.pybroker.com
 Author: Edward West
 Author-email: edwest@pybroker.com
 License: Apache License 2.0 with Commons Clause
 Classifier: License :: Free for non-commercial use
 Description-Content-Type: text/markdown
@@ -67,16 +67,18 @@
       if ctx.bars < 20:
          return
       # Get the rolling 10 day high.
       high_10d = ctx.indicator('high_10d')
       # Buy on a new 10 day high.
       if not ctx.long_pos() and high_10d[-1] > high_10d[-2]:
          ctx.buy_shares = 100
-         # Hold the position for 2 days.
-         ctx.hold_bars = 2
+         # Hold the position for 5 days.
+         ctx.hold_bars = 5
+         # Set a stop loss of 2%.
+         ctx.stop_loss_pct = 2
 
    strategy = Strategy(YFinance(), start_date='1/1/2022', end_date='7/1/2022')
    strategy.add_execution(
       exec_fn, ['AAPL', 'MSFT'], indicators=highest('high_10d', 'close', period=10))
    result = strategy.backtest()
 ```
 
@@ -116,14 +118,15 @@
 - [Backtesting a Strategy](https://www.pybroker.com/en/latest/notebooks/2.%20Backtesting%20a%20Strategy.html)
 - [Evaluating with Bootstrap Metrics](https://www.pybroker.com/en/latest/notebooks/3.%20Evaluating%20with%20Bootstrap%20Metrics.html)
 - [Ranking and Position Sizing](https://www.pybroker.com/en/latest/notebooks/4.%20Ranking%20and%20Position%20Sizing.html)
 - [Writing Indicators](https://www.pybroker.com/en/latest/notebooks/5.%20Writing%20Indicators.html)
 - [Training a Model](https://www.pybroker.com/en/latest/notebooks/6.%20Training%20a%20Model.html)
 - [Creating a Custom Data Source](https://www.pybroker.com/en/latest/notebooks/7.%20Creating%20a%20Custom%20Data%20Source.html)
 - [Applying Stops](https://www.pybroker.com/en/latest/notebooks/8.%20Applying%20Stops.html)
+- [Rebalancing Positions](https://www.pybroker.com/en/latest/notebooks/9.%20Rebalancing%20Positions.html)
 - [FAQs](https://www.pybroker.com/en/latest/notebooks/FAQs.html)
 
 ## Online Documentation
 
 [The full reference documentation is hosted at **www.pybroker.com**.](https://www.pybroker.com)
 
 ## Contact
```

### Comparing `lib-pybroker-1.1.3/src/lib_pybroker.egg-info/SOURCES.txt` & `lib-pybroker-1.1.4/src/lib_pybroker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.3/src/pybroker/__init__.py` & `lib-pybroker-1.1.4/src/pybroker/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,12 +36,13 @@
 from .eval import EvalMetrics, BootstrapResult
 from .indicator import Indicator, IndicatorSet, highest, indicator, lowest
 from .model import ModelLoader, ModelSource, ModelTrainer, model
 from .portfolio import Entry, Order, Position, Trade
 from .scope import (
     disable_logging,
     enable_logging,
+    param,
     register_columns,
     unregister_columns,
 )
 from .strategy import Strategy, TestResult
 from .vect import cross, highv, lowv, sumv
```

### Comparing `lib-pybroker-1.1.3/src/pybroker/cache.py` & `lib-pybroker-1.1.4/src/pybroker/cache.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.3/src/pybroker/common.py` & `lib-pybroker-1.1.4/src/pybroker/common.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.3/src/pybroker/config.py` & `lib-pybroker-1.1.4/src/pybroker/config.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.3/src/pybroker/context.py` & `lib-pybroker-1.1.4/src/pybroker/context.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.3/src/pybroker/data.py` & `lib-pybroker-1.1.4/src/pybroker/data.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.3/src/pybroker/eval.py` & `lib-pybroker-1.1.4/src/pybroker/eval.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.3/src/pybroker/indicator.py` & `lib-pybroker-1.1.4/src/pybroker/indicator.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.3/src/pybroker/log.py` & `lib-pybroker-1.1.4/src/pybroker/log.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.3/src/pybroker/model.py` & `lib-pybroker-1.1.4/src/pybroker/model.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.3/src/pybroker/portfolio.py` & `lib-pybroker-1.1.4/src/pybroker/portfolio.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.3/src/pybroker/scope.py` & `lib-pybroker-1.1.4/src/pybroker/scope.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 )
 from .log import Logger
 from collections import defaultdict
 from decimal import Decimal
 from diskcache import Cache
 from numpy.typing import NDArray
 from typing import (
+    Any,
     Callable,
     Collection,
     Iterable,
     Literal,
     Mapping,
     NamedTuple,
     Optional,
@@ -87,14 +88,15 @@
                 DataCol.CLOSE.value,
                 DataCol.VOLUME.value,
                 DataCol.VWAP.value,
             )
         )
         self.custom_data_cols = set()
         self._cols_frozen: bool = False
+        self._params: dict[str, Any] = {}
 
     def set_indicator(self, indicator):
         """Stores :class:`pybroker.indicator.Indicator` in static scope."""
         self._indicators[indicator.name] = indicator
 
     def has_indicator(self, name: str) -> bool:
         """Whether :class:`pybroker.indicator.Indicator` is stored in static
@@ -168,14 +170,21 @@
 
     def unfreeze_data_cols(self):
         """Allows additional data columns to be registered if
         :func:`pybroker.scope.StaticScope.freeze_data_cols` was called.
         """
         self._cols_frozen = False
 
+    def param(self, name: str, value: Optional[Any] = None) -> Optional[Any]:
+        """Get or set a global parameter."""
+        if value is None:
+            return self._params.get(name, None)
+        self._params[name] = value
+        return value
+
     @classmethod
     def instance(cls) -> "StaticScope":
         """Returns singleton instance."""
         if cls.__instance is None:
             cls.__instance = StaticScope()
         return cls.__instance
 
@@ -206,14 +215,19 @@
 
 
 def unregister_columns(names: Union[str, Iterable[str]], *args):
     """Unregisters ``names`` of user-defined data columns."""
     StaticScope.instance().unregister_custom_cols(names, *args)
 
 
+def param(name: str, value: Optional[Any] = None) -> Optional[Any]:
+    """Get or set a global parameter."""
+    return StaticScope.instance().param(name, value)
+
+
 class ColumnScope:
     """Caches and retrieves column data queried from :class:`pandas.DataFrame`.
 
     Args:
         df: :class:`pandas.DataFrame` containing the column data.
     """
```

### Comparing `lib-pybroker-1.1.3/src/pybroker/strategy.py` & `lib-pybroker-1.1.4/src/pybroker/strategy.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.3/src/pybroker/vect.py` & `lib-pybroker-1.1.4/src/pybroker/vect.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.3/tests/test_cache.py` & `lib-pybroker-1.1.4/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.3/tests/test_common.py` & `lib-pybroker-1.1.4/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.3/tests/test_context.py` & `lib-pybroker-1.1.4/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.3/tests/test_data.py` & `lib-pybroker-1.1.4/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.3/tests/test_eval.py` & `lib-pybroker-1.1.4/tests/test_eval.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.3/tests/test_indicator.py` & `lib-pybroker-1.1.4/tests/test_indicator.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.3/tests/test_log.py` & `lib-pybroker-1.1.4/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.3/tests/test_model.py` & `lib-pybroker-1.1.4/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.3/tests/test_portfolio.py` & `lib-pybroker-1.1.4/tests/test_portfolio.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.3/tests/test_scope.py` & `lib-pybroker-1.1.4/tests/test_scope.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from pybroker.model import model
 from pybroker.scope import (
     PriceScope,
     enable_logging,
     enable_progress_bar,
     disable_logging,
     disable_progress_bar,
+    param,
     register_columns,
     unregister_columns,
 )
 from unittest.mock import Mock
 
 
 @pytest.fixture(params=[10, None])
@@ -104,14 +105,23 @@
 
 
 def test_disable_progress_bar(mock_logger):
     disable_progress_bar()
     mock_logger.disable_progress_bar.assert_called_once()
 
 
+def test_param_when_empty():
+    assert param("bar") is None
+
+
+def test_param_when_set_and_get():
+    param("foo", 42)
+    assert param("foo") == 42
+
+
 class TestStaticScope:
     def test_set_and_get_indicator(self, scope, hhv_ind):
         scope.set_indicator(hhv_ind)
         assert scope.has_indicator(hhv_ind.name)
         assert scope.get_indicator(hhv_ind.name) == hhv_ind
 
     def test_get_indicator_when_not_found_then_error(self, scope):
```

### Comparing `lib-pybroker-1.1.3/tests/test_strategy.py` & `lib-pybroker-1.1.4/tests/test_strategy.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.3/tests/test_vect.py` & `lib-pybroker-1.1.4/tests/test_vect.py`

 * *Files identical despite different names*

