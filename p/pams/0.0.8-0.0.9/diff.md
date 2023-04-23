# Comparing `tmp/pams-0.0.8.tar.gz` & `tmp/pams-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pams-0.0.8.tar", max compression
+gzip compressed data, was "pams-0.0.9.tar", max compression
```

## Comparing `pams-0.0.8.tar` & `pams-0.0.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1072 2022-12-19 04:34:50.307114 pams-0.0.8/LICENSE
--rw-r--r--   0        0        0     1913 2022-12-19 04:34:50.307114 pams-0.0.8/README.md
--rw-r--r--   0        0        0      520 2022-12-19 04:34:50.307114 pams-0.0.8/pams/__init__.py
--rw-r--r--   0        0        0      187 2022-12-19 04:34:50.307114 pams-0.0.8/pams/agents/__init__.py
--rw-r--r--   0        0        0     5561 2022-12-19 04:34:50.307114 pams-0.0.8/pams/agents/arbitrage_agent.py
--rw-r--r--   0        0        0     8376 2022-12-19 04:34:50.307114 pams-0.0.8/pams/agents/base.py
--rw-r--r--   0        0        0     9238 2022-12-19 04:34:50.307114 pams-0.0.8/pams/agents/fcn_agent.py
--rw-r--r--   0        0        0      332 2022-12-19 04:34:50.307114 pams-0.0.8/pams/agents/high_frequency_agent.py
--rw-r--r--   0        0        0     2323 2022-12-19 04:34:50.307114 pams-0.0.8/pams/agents/test_agent.py
--rw-r--r--   0        0        0      114 2022-12-19 04:34:50.307114 pams-0.0.8/pams/events/__init__.py
--rw-r--r--   0        0        0     8592 2022-12-19 04:34:50.307114 pams-0.0.8/pams/events/base.py
--rw-r--r--   0        0        0     3030 2022-12-19 04:34:50.307114 pams-0.0.8/pams/events/fundamental_price_shock.py
--rw-r--r--   0        0        0     7006 2022-12-19 04:34:50.307114 pams-0.0.8/pams/fundamentals.py
--rw-r--r--   0        0        0     2838 2022-12-19 04:34:50.307114 pams-0.0.8/pams/index_market.py
--rw-r--r--   0        0        0      447 2022-12-19 04:34:50.307114 pams-0.0.8/pams/logs/__init__.py
--rw-r--r--   0        0        0    10050 2022-12-19 04:34:50.307114 pams-0.0.8/pams/logs/base.py
--rw-r--r--   0        0        0      986 2022-12-19 04:34:50.307114 pams-0.0.8/pams/logs/market_step_loggers.py
--rw-r--r--   0        0        0    22730 2022-12-19 04:34:50.307114 pams-0.0.8/pams/market.py
--rw-r--r--   0        0        0     5458 2022-12-19 04:34:50.307114 pams-0.0.8/pams/order.py
--rw-r--r--   0        0        0     3554 2022-12-19 04:34:50.307114 pams-0.0.8/pams/order_book.py
--rw-r--r--   0        0        0       66 2022-12-19 04:34:50.307114 pams-0.0.8/pams/runners/__init__.py
--rw-r--r--   0        0        0     1753 2022-12-19 04:34:50.307114 pams-0.0.8/pams/runners/base.py
--rw-r--r--   0        0        0    23303 2022-12-19 04:34:50.307114 pams-0.0.8/pams/runners/sequential.py
--rw-r--r--   0        0        0     2730 2022-12-19 04:34:50.307114 pams-0.0.8/pams/session.py
--rw-r--r--   0        0        0    13130 2022-12-19 04:34:50.307114 pams-0.0.8/pams/simulator.py
--rw-r--r--   0        0        0      147 2022-12-19 04:34:50.311113 pams-0.0.8/pams/utils/__init__.py
--rw-r--r--   0        0        0      909 2022-12-19 04:34:50.311113 pams-0.0.8/pams/utils/class_finder.py
--rw-r--r--   0        0        0     1141 2022-12-19 04:34:50.311113 pams-0.0.8/pams/utils/json_extends.py
--rw-r--r--   0        0        0     3094 2022-12-19 04:34:50.311113 pams-0.0.8/pams/utils/json_random.py
--rw-r--r--   0        0        0       22 2022-12-19 04:34:50.311113 pams-0.0.8/pams/version.py
--rw-r--r--   0        0        0     1048 2022-12-19 04:34:50.311113 pams-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     3054 1970-01-01 00:00:00.000000 pams-0.0.8/setup.py
--rw-r--r--   0        0        0     2922 1970-01-01 00:00:00.000000 pams-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-01-07 11:10:00.324881 pams-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1903 2023-01-07 11:10:00.324881 pams-0.0.9/README.md
+-rw-r--r--   0        0        0      520 2023-01-07 11:10:00.328881 pams-0.0.9/pams/__init__.py
+-rw-r--r--   0        0        0      187 2023-01-07 11:10:00.328881 pams-0.0.9/pams/agents/__init__.py
+-rw-r--r--   0        0        0     5561 2023-01-07 11:10:00.328881 pams-0.0.9/pams/agents/arbitrage_agent.py
+-rw-r--r--   0        0        0     8376 2023-01-07 11:10:00.328881 pams-0.0.9/pams/agents/base.py
+-rw-r--r--   0        0        0     9238 2023-01-07 11:10:00.328881 pams-0.0.9/pams/agents/fcn_agent.py
+-rw-r--r--   0        0        0      332 2023-01-07 11:10:00.328881 pams-0.0.9/pams/agents/high_frequency_agent.py
+-rw-r--r--   0        0        0     2323 2023-01-07 11:10:00.328881 pams-0.0.9/pams/agents/test_agent.py
+-rw-r--r--   0        0        0      114 2023-01-07 11:10:00.328881 pams-0.0.9/pams/events/__init__.py
+-rw-r--r--   0        0        0     8592 2023-01-07 11:10:00.328881 pams-0.0.9/pams/events/base.py
+-rw-r--r--   0        0        0     3030 2023-01-07 11:10:00.328881 pams-0.0.9/pams/events/fundamental_price_shock.py
+-rw-r--r--   0        0        0     7006 2023-01-07 11:10:00.328881 pams-0.0.9/pams/fundamentals.py
+-rw-r--r--   0        0        0     2838 2023-01-07 11:10:00.328881 pams-0.0.9/pams/index_market.py
+-rw-r--r--   0        0        0      447 2023-01-07 11:10:00.328881 pams-0.0.9/pams/logs/__init__.py
+-rw-r--r--   0        0        0    13513 2023-01-07 11:10:00.328881 pams-0.0.9/pams/logs/base.py
+-rw-r--r--   0        0        0     1397 2023-01-07 11:10:00.328881 pams-0.0.9/pams/logs/market_step_loggers.py
+-rw-r--r--   0        0        0    23106 2023-01-07 11:10:00.328881 pams-0.0.9/pams/market.py
+-rw-r--r--   0        0        0     5458 2023-01-07 11:10:00.328881 pams-0.0.9/pams/order.py
+-rw-r--r--   0        0        0     3587 2023-01-07 11:10:00.328881 pams-0.0.9/pams/order_book.py
+-rw-r--r--   0        0        0       66 2023-01-07 11:10:00.328881 pams-0.0.9/pams/runners/__init__.py
+-rw-r--r--   0        0        0     3174 2023-01-07 11:10:00.328881 pams-0.0.9/pams/runners/base.py
+-rw-r--r--   0        0        0    23621 2023-01-07 11:10:00.328881 pams-0.0.9/pams/runners/sequential.py
+-rw-r--r--   0        0        0     2730 2023-01-07 11:10:00.328881 pams-0.0.9/pams/session.py
+-rw-r--r--   0        0        0    13751 2023-01-07 11:10:00.328881 pams-0.0.9/pams/simulator.py
+-rw-r--r--   0        0        0      147 2023-01-07 11:10:00.328881 pams-0.0.9/pams/utils/__init__.py
+-rw-r--r--   0        0        0      909 2023-01-07 11:10:00.328881 pams-0.0.9/pams/utils/class_finder.py
+-rw-r--r--   0        0        0     1141 2023-01-07 11:10:00.328881 pams-0.0.9/pams/utils/json_extends.py
+-rw-r--r--   0        0        0     3094 2023-01-07 11:10:00.328881 pams-0.0.9/pams/utils/json_random.py
+-rw-r--r--   0        0        0       22 2023-01-07 11:10:00.328881 pams-0.0.9/pams/version.py
+-rw-r--r--   0        0        0     1048 2023-01-07 11:10:00.328881 pams-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3044 1970-01-01 00:00:00.000000 pams-0.0.9/setup.py
+-rw-r--r--   0        0        0     2912 1970-01-01 00:00:00.000000 pams-0.0.9/PKG-INFO
```

### Comparing `pams-0.0.8/LICENSE` & `pams-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pams-0.0.8/README.md` & `pams-0.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,14 @@
     year={2022},
     url = {https://github.com/masanorihirano/pams}
 }
 ```
 
 ## Issues and Contribution
 About issues (bugs):
--   You can report issues [here](https://github.com/masanorihirano/slack_transfer/issues).
+-   You can report issues [here](https://github.com/masanorihirano/pams/issues).
 -   There are no guarantee to support or fix those issues.
 
 Contributions:
 -   You can send pull requests (PRs) to this repository.
 -   But, there are no guarantee to merge your PRs.
```

### Comparing `pams-0.0.8/pams/__init__.py` & `pams-0.0.9/pams/__init__.py`

 * *Files identical despite different names*

### Comparing `pams-0.0.8/pams/agents/arbitrage_agent.py` & `pams-0.0.9/pams/agents/arbitrage_agent.py`

 * *Files identical despite different names*

### Comparing `pams-0.0.8/pams/agents/base.py` & `pams-0.0.9/pams/agents/base.py`

 * *Files identical despite different names*

### Comparing `pams-0.0.8/pams/agents/fcn_agent.py` & `pams-0.0.9/pams/agents/fcn_agent.py`

 * *Files identical despite different names*

### Comparing `pams-0.0.8/pams/agents/test_agent.py` & `pams-0.0.9/pams/agents/test_agent.py`

 * *Files identical despite different names*

### Comparing `pams-0.0.8/pams/events/base.py` & `pams-0.0.9/pams/events/base.py`

 * *Files identical despite different names*

### Comparing `pams-0.0.8/pams/events/fundamental_price_shock.py` & `pams-0.0.9/pams/events/fundamental_price_shock.py`

 * *Files identical despite different names*

### Comparing `pams-0.0.8/pams/fundamentals.py` & `pams-0.0.9/pams/fundamentals.py`

 * *Files identical despite different names*

### Comparing `pams-0.0.8/pams/index_market.py` & `pams-0.0.9/pams/index_market.py`

 * *Files identical despite different names*

### Comparing `pams-0.0.8/pams/logs/market_step_loggers.py` & `pams-0.0.9/pams/logs/market_step_loggers.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,24 +2,44 @@
 from typing import List
 
 from .base import Logger
 from .base import MarketStepEndLog
 
 
 class MarketStepPrintLogger(Logger):
+    """Logger of the market step class."""
+
     def process_market_step_end_log(self, log: MarketStepEndLog) -> None:
+        """print the market log.
+
+        Args:
+            log (:class:`pams.logs.MarketStepEndLog`): matket log.
+
+        Returns:
+            None
+        """
         print(
             f"{log.session.session_id} {log.market.get_time()} {log.market.market_id} {log.market.name} {log.market.get_market_price()} {log.market.get_fundamental_price()}"
         )
 
 
 class MarketStepSaver(Logger):
+    """Saver of the market step class."""
+
     market_step_logs: List[Dict] = []
 
     def process_market_step_end_log(self, log: MarketStepEndLog) -> None:
+        """stack the market log.
+
+        Args:
+            log (:class:`pams.logs.MarketStepEndLog`): market log.
+
+        Returns:
+            None
+        """
         self.market_step_logs.append(
             {
                 "session_id": log.session.session_id,
                 "market_time": log.market.get_time(),
                 "market_id": log.market.market_id,
                 "market_name": log.market.name,
                 "market_price": log.market.get_market_price(),
```

### Comparing `pams-0.0.8/pams/market.py` & `pams-0.0.9/pams/market.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import math
 import random
+import warnings
 from typing import Any
 from typing import Dict
 from typing import Iterable
 from typing import List
 from typing import Optional
 from typing import Tuple
 from typing import TypeVar
@@ -437,14 +438,22 @@
         if order.market_id != self.market_id:
             raise ValueError("order is not for this market")
         (self.buy_order_book if order.is_buy else self.sell_order_book).add(order=order)
         if order.placed_at is None:
             raise AssertionError
         if order.order_id is not None:
             raise ValueError("the order is already submitted")
+        if order.price is not None and order.price % self.tick_size != 0:
+            warnings.warn(
+                "order price does not accord to the tick size. price will be modified"
+            )
+            order.price = (
+                self.convert_to_tick_level(price=order.price, is_buy=order.is_buy)
+                * self.tick_size
+            )
         order.order_id = self._next_order_id
         self._next_order_id += 1
         self._update_market_price()
         if order.is_buy:
             self._n_buy_orders[self.time] += 1
         else:
             self._n_sell_orders[self.time] += 1
```

### Comparing `pams-0.0.8/pams/order.py` & `pams-0.0.9/pams/order.py`

 * *Files identical despite different names*

### Comparing `pams-0.0.8/pams/order_book.py` & `pams-0.0.9/pams/order_book.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,15 +80,16 @@
         return len(self.priority_queue.queue)
 
     def get_price_volume(self) -> Dict[Optional[float], int]:
         keys: List[Optional[float]] = list(
             set(map(lambda x: x.price, self.priority_queue.queue))
         )
         has_market_order: bool = None in keys
-        keys.remove(None)
+        if has_market_order:
+            keys.remove(None)
         keys.sort(reverse=self.is_buy)
         if has_market_order:
             keys.insert(0, None)
         result: Dict[Optional[float], int] = dict(
             [
                 (
                     key,
```

### Comparing `pams-0.0.8/pams/runners/sequential.py` & `pams-0.0.9/pams/runners/sequential.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,15 @@
                 fundamental_price = float(market_settings["marketPrice"])
             else:
                 raise ValueError(
                     f"fundamentalPrice or marketPrice is required for {name}"
                 )
             fundamental_drift: float = 0.0
             if "fundamentalDrift" in market_settings:
-                fundamental_price = float(market_settings["fundamentalDrift"])
+                fundamental_drift = float(market_settings["fundamentalDrift"])
             fundamental_volatility: float = 0.0
             if "fundamentalVolatility" in market_settings:
                 fundamental_volatility = float(market_settings["fundamentalVolatility"])
 
             for i in range(id_from, id_to + 1):
                 market = market_class(
                     market_id=i_market,
@@ -376,15 +376,19 @@
                     agent = self.simulator.id2agent[order.order.agent_id]
                     agent.canceled_order(log=log_)
                     self.simulator._trigger_event_after_cancel(cancel_log=order)
                 else:
                     raise NotImplementedError
                 if session.with_order_execution:
                     logs: List[ExecutionLog] = market._execution()
+                    self.simulator._update_agents_for_execution(execution_logs=logs)
                     for execution_log in logs:
+                        agent = self.simulator.id2agent[execution_log.buy_agent_id]
+                        agent.executed_order(log=execution_log)
+                        agent = self.simulator.id2agent[execution_log.sell_agent_id]
                         agent.executed_order(log=execution_log)
                         self.simulator._trigger_event_after_execution(
                             execution_log=execution_log
                         )
 
             if session.high_frequency_submission_rate < self._prng.random():
                 continue
```

### Comparing `pams-0.0.8/pams/session.py` & `pams-0.0.9/pams/session.py`

 * *Files identical despite different names*

### Comparing `pams-0.0.8/pams/simulator.py` & `pams-0.0.9/pams/simulator.py`

 * *Files 10% similar despite different names*

```diff
@@ -162,14 +162,28 @@
 
     def _update_times_on_markets(self, markets: List[Market]) -> None:
         for market in filter(lambda x: not isinstance(x, IndexMarket), markets):
             self._update_time_on_market(market=market)
         for market in filter(lambda x: isinstance(x, IndexMarket), markets):
             self._update_time_on_market(market=market)
 
+    def _update_agents_for_execution(
+        self, execution_logs: List["ExecutionLog"]  # type: ignore
+    ) -> None:
+        for log in execution_logs:
+            buy_agent: Agent = self.id2agent[log.buy_agent_id]
+            sell_agent: Agent = self.id2agent[log.sell_agent_id]
+            price: float = log.price
+            volume: int = log.volume
+            market_id: int = log.market_id
+            buy_agent.cash_amount -= price * volume
+            sell_agent.cash_amount += price * volume
+            buy_agent.asset_volumes[market_id] += volume
+            sell_agent.asset_volumes[market_id] -= volume
+
     def _check_event_class_and_instance(
         self,
         check_object: object,
         class_requirement: Optional[Type] = None,
         instance_requirement: Optional[object] = None,
     ) -> bool:
         if class_requirement is not None:
```

### Comparing `pams-0.0.8/pams/utils/class_finder.py` & `pams-0.0.9/pams/utils/class_finder.py`

 * *Files identical despite different names*

### Comparing `pams-0.0.8/pams/utils/json_extends.py` & `pams-0.0.9/pams/utils/json_extends.py`

 * *Files identical despite different names*

### Comparing `pams-0.0.8/pams/utils/json_random.py` & `pams-0.0.9/pams/utils/json_random.py`

 * *Files identical despite different names*

### Comparing `pams-0.0.8/pyproject.toml` & `pams-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pams"
-version = "0.0.8"
+version = "0.0.9"
 description = "PAMS: Platform for Artificial Market Simulations"
 authors = ["Masanori HIRANO <masa.hirano.1996@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `pams-0.0.8/setup.py` & `pams-0.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 {':python_version >= "3.7" and python_version < "3.8"': ['numpy>=1.21.0,<2.0.0',
                                                          'scipy>=1.7.0,<2.0.0'],
  ':python_version >= "3.8" and python_version < "4.0"': ['numpy>=1.23.4,<2.0.0',
                                                          'scipy>=1.9.2,<2.0.0']}
 
 setup_kwargs = {
     'name': 'pams',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'PAMS: Platform for Artificial Market Simulations',
-    'long_description': '# pams\nPAMS: Platform for Artificial Market Simulations\n\n[![python](https://img.shields.io/pypi/pyversions/pams.svg)](https://pypi.org/project/pams)\n[![pypi](https://img.shields.io/pypi/v/pams.svg)](https://pypi.org/project/pams)\n[![CI](https://github.com/masanorihirano/pams/actions/workflows/ci-python.yml/badge.svg)](https://github.com/masanorihirano/pams/actions/workflows/ci-python.yml)\n[![downloads](https://img.shields.io/pypi/dm/pams)](https://pypi.org/project/pams)\n[![code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Codacy Badge](https://app.codacy.com/project/badge/Grade/18ed1eecc4f34a99bb6fd9a7160f78ca)](https://www.codacy.com/gh/masanorihirano/pams/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=masanorihirano/pams&amp;utm_campaign=Badge_Grade)\n[![codecov](https://codecov.io/gh/masanorihirano/pams/branch/main/graph/badge.svg?token=tFccElw7Wd)](https://codecov.io/gh/masanorihirano/pams)\n\n## Documentations & User Guides\n\nDocumentations are available on [readthedoc](https://pams.hirano.dev/)\n\n## Install\nThis package is available on pypi as [`pams`](https://pypi.org/project/pams/)\n```bash\n$ pip install pams\n$ python\n>> import pams\n```\n\n## Citation\nCurrently, no publication related to this repository. Therefore, please cite this repository directly if you want.\n```bibtex\n@misc{Hirano2022-pams\n    title={{PAMS: Platform for Artificial Market Simulations}},\n    autors={Masanori HIRANO, Ryosuke TAKATA},\n    year={2022},\n    url = {https://github.com/masanorihirano/pams}\n}\n```\n\n## Issues and Contribution\nAbout issues (bugs):\n-   You can report issues [here](https://github.com/masanorihirano/slack_transfer/issues).\n-   There are no guarantee to support or fix those issues.\n\nContributions:\n-   You can send pull requests (PRs) to this repository.\n-   But, there are no guarantee to merge your PRs.\n\n',
+    'long_description': '# pams\nPAMS: Platform for Artificial Market Simulations\n\n[![python](https://img.shields.io/pypi/pyversions/pams.svg)](https://pypi.org/project/pams)\n[![pypi](https://img.shields.io/pypi/v/pams.svg)](https://pypi.org/project/pams)\n[![CI](https://github.com/masanorihirano/pams/actions/workflows/ci-python.yml/badge.svg)](https://github.com/masanorihirano/pams/actions/workflows/ci-python.yml)\n[![downloads](https://img.shields.io/pypi/dm/pams)](https://pypi.org/project/pams)\n[![code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Codacy Badge](https://app.codacy.com/project/badge/Grade/18ed1eecc4f34a99bb6fd9a7160f78ca)](https://www.codacy.com/gh/masanorihirano/pams/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=masanorihirano/pams&amp;utm_campaign=Badge_Grade)\n[![codecov](https://codecov.io/gh/masanorihirano/pams/branch/main/graph/badge.svg?token=tFccElw7Wd)](https://codecov.io/gh/masanorihirano/pams)\n\n## Documentations & User Guides\n\nDocumentations are available on [readthedoc](https://pams.hirano.dev/)\n\n## Install\nThis package is available on pypi as [`pams`](https://pypi.org/project/pams/)\n```bash\n$ pip install pams\n$ python\n>> import pams\n```\n\n## Citation\nCurrently, no publication related to this repository. Therefore, please cite this repository directly if you want.\n```bibtex\n@misc{Hirano2022-pams\n    title={{PAMS: Platform for Artificial Market Simulations}},\n    autors={Masanori HIRANO, Ryosuke TAKATA},\n    year={2022},\n    url = {https://github.com/masanorihirano/pams}\n}\n```\n\n## Issues and Contribution\nAbout issues (bugs):\n-   You can report issues [here](https://github.com/masanorihirano/pams/issues).\n-   There are no guarantee to support or fix those issues.\n\nContributions:\n-   You can send pull requests (PRs) to this repository.\n-   But, there are no guarantee to merge your PRs.\n\n',
     'author': 'Masanori HIRANO',
     'author_email': 'masa.hirano.1996@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pams-0.0.8/PKG-INFO` & `pams-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pams
-Version: 0.0.8
+Version: 0.0.9
 Summary: PAMS: Platform for Artificial Market Simulations
 License: MIT
 Author: Masanori HIRANO
 Author-email: masa.hirano.1996@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -52,15 +52,15 @@
     year={2022},
     url = {https://github.com/masanorihirano/pams}
 }
 ```
 
 ## Issues and Contribution
 About issues (bugs):
--   You can report issues [here](https://github.com/masanorihirano/slack_transfer/issues).
+-   You can report issues [here](https://github.com/masanorihirano/pams/issues).
 -   There are no guarantee to support or fix those issues.
 
 Contributions:
 -   You can send pull requests (PRs) to this repository.
 -   But, there are no guarantee to merge your PRs.
```

