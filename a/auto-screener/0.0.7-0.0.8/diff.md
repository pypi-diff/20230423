# Comparing `tmp/auto-screener-0.0.7.tar.gz` & `tmp/auto-screener-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-screener-0.0.7.tar", last modified: Sat Apr 22 22:10:29 2023, max compression
+gzip compressed data, was "auto-screener-0.0.8.tar", last modified: Sun Apr 23 18:01:01 2023, max compression
```

## Comparing `auto-screener-0.0.7.tar` & `auto-screener-0.0.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 22:10:29.686858 auto-screener-0.0.7/
--rw-rw-rw-   0        0        0      115 2023-04-22 22:10:29.000000 auto-screener-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     2066 2023-04-22 22:10:29.686858 auto-screener-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1255 2023-04-21 09:27:54.000000 auto-screener-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-22 22:10:29.681258 auto-screener-0.0.7/auto_screener/
--rw-rw-rw-   0        0        0      498 2023-04-21 09:31:59.000000 auto-screener-0.0.7/auto_screener/__init__.py
--rw-rw-rw-   0        0        0     6694 2023-03-18 20:51:39.000000 auto-screener-0.0.7/auto_screener/base.py
--rw-rw-rw-   0        0        0     5944 2023-04-22 07:38:43.000000 auto-screener-0.0.7/auto_screener/dataset.py
--rw-rw-rw-   0        0        0      526 2023-04-21 17:13:30.000000 auto-screener-0.0.7/auto_screener/document.py
--rw-rw-rw-   0        0        0      180 2023-04-21 16:51:56.000000 auto-screener-0.0.7/auto_screener/hints.py
--rw-rw-rw-   0        0        0     2665 2023-04-21 16:51:36.000000 auto-screener-0.0.7/auto_screener/interval.py
--rw-rw-rw-   0        0        0    10013 2023-04-21 17:11:58.000000 auto-screener-0.0.7/auto_screener/progress.py
--rw-rw-rw-   0        0        0    51960 2023-04-22 22:09:03.000000 auto-screener-0.0.7/auto_screener/screening.py
--rw-rw-rw-   0        0        0     9865 2023-04-21 17:03:15.000000 auto-screener-0.0.7/auto_screener/tickers.py
-drwxrwxrwx   0        0        0        0 2023-04-22 22:10:29.685810 auto-screener-0.0.7/auto_screener.egg-info/
--rw-rw-rw-   0        0        0     2066 2023-04-22 22:10:29.000000 auto-screener-0.0.7/auto_screener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      489 2023-04-22 22:10:29.000000 auto-screener-0.0.7/auto_screener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 22:10:29.000000 auto-screener-0.0.7/auto_screener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-04-22 22:10:29.000000 auto-screener-0.0.7/auto_screener.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-22 22:10:29.000000 auto-screener-0.0.7/auto_screener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 auto-screener-0.0.7/build.py
--rw-rw-rw-   0        0        0      645 2023-04-22 22:10:29.000000 auto-screener-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       38 2023-04-21 17:54:19.000000 auto-screener-0.0.7/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-22 22:10:29.686858 auto-screener-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1655 2023-04-22 22:10:27.000000 auto-screener-0.0.7/setup.py
--rw-rw-rw-   0        0        0     1186 2023-04-22 22:10:01.000000 auto-screener-0.0.7/test.py
+drwxrwxrwx   0        0        0        0 2023-04-23 18:01:01.582907 auto-screener-0.0.8/
+-rw-rw-rw-   0        0        0      115 2023-04-23 18:01:01.000000 auto-screener-0.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     2066 2023-04-23 18:01:01.582907 auto-screener-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1255 2023-04-21 09:27:54.000000 auto-screener-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 18:01:01.576783 auto-screener-0.0.8/auto_screener/
+-rw-rw-rw-   0        0        0      498 2023-04-21 09:31:59.000000 auto-screener-0.0.8/auto_screener/__init__.py
+-rw-rw-rw-   0        0        0     6694 2023-03-18 20:51:39.000000 auto-screener-0.0.8/auto_screener/base.py
+-rw-rw-rw-   0        0        0     5944 2023-04-22 07:38:43.000000 auto-screener-0.0.8/auto_screener/dataset.py
+-rw-rw-rw-   0        0        0      526 2023-04-21 17:13:30.000000 auto-screener-0.0.8/auto_screener/document.py
+-rw-rw-rw-   0        0        0      180 2023-04-21 16:51:56.000000 auto-screener-0.0.8/auto_screener/hints.py
+-rw-rw-rw-   0        0        0     2665 2023-04-21 16:51:36.000000 auto-screener-0.0.8/auto_screener/interval.py
+-rw-rw-rw-   0        0        0    10013 2023-04-21 17:11:58.000000 auto-screener-0.0.8/auto_screener/progress.py
+-rw-rw-rw-   0        0        0    53152 2023-04-23 17:57:09.000000 auto-screener-0.0.8/auto_screener/screening.py
+-rw-rw-rw-   0        0        0     9865 2023-04-21 17:03:15.000000 auto-screener-0.0.8/auto_screener/tickers.py
+drwxrwxrwx   0        0        0        0 2023-04-23 18:01:01.581907 auto-screener-0.0.8/auto_screener.egg-info/
+-rw-rw-rw-   0        0        0     2066 2023-04-23 18:01:01.000000 auto-screener-0.0.8/auto_screener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      489 2023-04-23 18:01:01.000000 auto-screener-0.0.8/auto_screener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 18:01:01.000000 auto-screener-0.0.8/auto_screener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 18:01:01.000000 auto-screener-0.0.8/auto_screener.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-23 18:01:01.000000 auto-screener-0.0.8/auto_screener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 auto-screener-0.0.8/build.py
+-rw-rw-rw-   0        0        0      645 2023-04-23 18:01:01.000000 auto-screener-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       38 2023-04-21 17:54:19.000000 auto-screener-0.0.8/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 18:01:01.583907 auto-screener-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1655 2023-04-23 18:00:58.000000 auto-screener-0.0.8/setup.py
+-rw-rw-rw-   0        0        0      850 2023-04-23 18:00:43.000000 auto-screener-0.0.8/test.py
```

### Comparing `auto-screener-0.0.7/PKG-INFO` & `auto-screener-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-screener
-Version: 0.0.7
+Version: 0.0.8
 Summary: A software for automatically screening crypto exchanges for crypto pairs trading prices and rates.
 Home-page: https://github.com/Shahaf-F-S/auto-screener
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `auto-screener-0.0.7/README.md` & `auto-screener-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `auto-screener-0.0.7/auto_screener/base.py` & `auto-screener-0.0.8/auto_screener/base.py`

 * *Files identical despite different names*

### Comparing `auto-screener-0.0.7/auto_screener/dataset.py` & `auto-screener-0.0.8/auto_screener/dataset.py`

 * *Files identical despite different names*

### Comparing `auto-screener-0.0.7/auto_screener/document.py` & `auto-screener-0.0.8/auto_screener/document.py`

 * *Files identical despite different names*

### Comparing `auto-screener-0.0.7/auto_screener/interval.py` & `auto-screener-0.0.8/auto_screener/interval.py`

 * *Files identical despite different names*

### Comparing `auto-screener-0.0.7/auto_screener/progress.py` & `auto-screener-0.0.8/auto_screener/progress.py`

 * *Files identical despite different names*

### Comparing `auto-screener-0.0.7/auto_screener/screening.py` & `auto-screener-0.0.8/auto_screener/screening.py`

 * *Files 3% similar despite different names*

```diff
@@ -1130,78 +1130,102 @@
 
     return WaitingState(
         screeners=screeners, delay=delay, count=count
     )
 # end wait_for_update
 
 def _collect_exchange_assets(
-        data: Dict[str, List[str]], source: str, exchange: ccxt.Exchange
+        data: Dict[str, List[str]],
+        source: str,
+        exchange: ccxt.Exchange,
+        quotes: Optional[Iterable[str]] = None
 ) -> None:
     """
     Collects the tickers from the exchanges.
 
     :param source: The name of the exchange.
     :param exchange: The exchange object.
     :param data: The data to collect the assets.
+    :param quotes: The quotes of the asset pairs.
 
     :return: The data of the exchanges.
     """
 
+    quotes = quotes or []
     assets = []
 
     # noinspection PyBroadException
     try:
         for value in exchange.load_markets().values():
+            if quotes and (value['quote'] not in quotes):
+                continue
+            # end if
+
             assets.append(value['base'])
         # end for
 
         data[source] = list(set(assets))
 
     except Exception:
         data[source] = []
     # end try
 # end _collect_exchange_assets
 
 def _collect_exchange_tickers(
-        data: Dict[str, List[str]], source: str, exchange: ccxt.Exchange
+        data: Dict[str, List[str]],
+        source: str,
+        exchange: ccxt.Exchange,
+        quotes: Optional[Iterable[str]] = None
 ) -> None:
     """
     Collects the tickers from the exchanges.
 
     :param source: The name of the exchange.
     :param exchange: The exchange object.
     :param data: The data to collect the assets.
+    :param quotes: The quotes of the asset pairs.
 
     :return: The data of the exchanges.
     """
 
+    quotes = quotes or []
     tickers = []
 
     # noinspection PyBroadException
     try:
         for value in exchange.load_markets().values():
+            if quotes and (value['quote'] not in quotes):
+                continue
+            # end if
+
             tickers.append(parts_to_ticker(value['base'], value['quote']))
         # end for
 
         data[source] = list(set(tickers))
 
     except Exception:
         data[source] = []
     # end try
 # end _collect_exchange_tickers
 
-def collect_assets(exchanges: Optional[Iterable[str]] = None) -> Dict[str, List[str]]:
+def collect_assets(
+        exchanges: Optional[Iterable[str]] = None,
+        quotes: Optional[Iterable[str]] = None
+) -> Dict[str, List[str]]:
     """
     Collects the tickers from the exchanges.
 
     :param exchanges: The exchanges.
+    :param quotes: The quotes of the asset pairs.
 
     :return: The data of the exchanges.
     """
 
+    quotes = quotes or []
+
     data = {}
     markets = {}
 
     count = 0
 
     for source in (exchanges or ccxt.__dict__):
         if source in ccxt.exchanges:
@@ -1219,35 +1243,42 @@
             markets[source] = exchange
         # end if
     # end for
 
     for source, exchange in markets.items():
         threading.Thread(
             target=_collect_exchange_assets,
-            kwargs=dict(source=source, exchange=exchange, data=data)
+            kwargs=dict(
+                source=source, exchange=exchange,
+                data=data, quotes=quotes
+            )
         ).start()
     # end for
 
     while (len(markets) - count) > len(data):
         pass
     # end while
 
     return {key: value for key, value in data.items() if value}
 # end collect_tickers
 
-def collect_mutual_assets(exchanges: Optional[Iterable[str]] = None) -> Dict[str, List[str]]:
+def collect_mutual_assets(
+        exchanges: Optional[Iterable[str]] = None,
+        quotes: Optional[Iterable[str]] = None
+) -> Dict[str, List[str]]:
     """
     Collects the tickers from the exchanges.
 
     :param exchanges: The exchanges.
+    :param quotes: The quotes of the asset pairs.
 
     :return: The data of the exchanges.
     """
 
-    exchanges = collect_assets(exchanges)
+    exchanges = collect_assets(exchanges=exchanges, quotes=quotes)
 
     assets = {}
 
     for source in exchanges:
         for asset in exchanges[source]:
             assets[asset] = assets.setdefault(asset, 0) + 1
         # end for
@@ -1258,23 +1289,29 @@
             asset for asset in exchanges[source]
             if assets.get(asset, 0) > 1
         ]
         for source in exchanges
     }
 # end collect_mutual_assets
 
-def collect_tickers(exchanges: Optional[Iterable[str]] = None) -> Dict[str, List[str]]:
+def collect_tickers(
+        exchanges: Optional[Iterable[str]] = None,
+        quotes: Optional[Iterable[str]] = None
+) -> Dict[str, List[str]]:
     """
     Collects the tickers from the exchanges.
 
     :param exchanges: The exchanges.
+    :param quotes: The quotes of the asset pairs.
 
     :return: The data of the exchanges.
     """
 
+    quotes = quotes or []
+
     data = {}
     markets = {}
 
     count = 0
 
     for source in (exchanges or ccxt.__dict__):
         if source in ccxt.exchanges:
@@ -1292,35 +1329,42 @@
             markets[source] = exchange
         # end if
     # end for
 
     for source, exchange in markets.items():
         threading.Thread(
             target=_collect_exchange_tickers,
-            kwargs=dict(source=source, exchange=exchange, data=data)
+            kwargs=dict(
+                source=source, exchange=exchange,
+                data=data, quotes=quotes
+            )
         ).start()
     # end for
 
     while (len(markets) - count) > len(data):
         pass
     # end while
 
     return {key: value for key, value in data.items() if value}
 # end collect_tickers
 
-def collect_mutual_tickers(exchanges: Optional[Iterable[str]] = None) -> Dict[str, List[str]]:
+def collect_mutual_tickers(
+        exchanges: Optional[Iterable[str]] = None,
+        quotes: Optional[Iterable[str]] = None
+) -> Dict[str, List[str]]:
     """
     Collects the tickers from the exchanges.
 
     :param exchanges: The exchanges.
+    :param quotes: The quotes of the asset pairs.
 
     :return: The data of the exchanges.
     """
 
-    exchanges = collect_tickers(exchanges)
+    exchanges = collect_tickers(exchanges=exchanges, quotes=quotes)
 
     tickers = {}
 
     for source in exchanges:
         for ticker in exchanges[source]:
             tickers[ticker] = tickers.setdefault(ticker, 0) + 1
         # end for
```

### Comparing `auto-screener-0.0.7/auto_screener/tickers.py` & `auto-screener-0.0.8/auto_screener/tickers.py`

 * *Files identical despite different names*

### Comparing `auto-screener-0.0.7/auto_screener.egg-info/PKG-INFO` & `auto-screener-0.0.8/auto_screener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-screener
-Version: 0.0.7
+Version: 0.0.8
 Summary: A software for automatically screening crypto exchanges for crypto pairs trading prices and rates.
 Home-page: https://github.com/Shahaf-F-S/auto-screener
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `auto-screener-0.0.7/build.py` & `auto-screener-0.0.8/build.py`

 * *Files identical despite different names*

### Comparing `auto-screener-0.0.7/pyproject.toml` & `auto-screener-0.0.8/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'auto-screener'
-version = '0.0.7'
+version = '0.0.8'
 description = 'A software for automatically screening crypto exchanges for crypto pairs trading prices and rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `auto-screener-0.0.7/setup.py` & `auto-screener-0.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         include=[
             "test.py",
             "auto_screener/source"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='auto-screener',
-        version='0.0.7',
+        version='0.0.8',
         description=(
             "A software for automatically screening "
             "crypto exchanges for crypto pairs "
             "trading prices and rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

