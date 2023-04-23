# Comparing `tmp/tradeX-0.0.2.tar.gz` & `tmp/tradeX-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tradeX-0.0.2.tar", last modified: Sun Apr 23 14:38:30 2023, max compression
+gzip compressed data, was "tradeX-0.0.3.tar", last modified: Sun Apr 23 16:38:01 2023, max compression
```

## Comparing `tradeX-0.0.2.tar` & `tradeX-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,59 @@
-drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-04-23 14:38:30.956026 tradeX-0.0.2/
--rw-rw-r--   0 tu        (1000) tu        (1000)     1066 2023-04-04 16:17:18.000000 tradeX-0.0.2/LICENSE.txt
--rw-rw-r--   0 tu        (1000) tu        (1000)     2849 2023-04-23 14:38:30.956026 tradeX-0.0.2/PKG-INFO
--rw-rw-r--   0 tu        (1000) tu        (1000)     2449 2023-04-04 09:31:25.000000 tradeX-0.0.2/README.md
--rw-rw-r--   0 tu        (1000) tu        (1000)       86 2023-04-04 15:51:41.000000 tradeX-0.0.2/pyproject.toml
--rw-rw-r--   0 tu        (1000) tu        (1000)       38 2023-04-23 14:38:30.956026 tradeX-0.0.2/setup.cfg
--rw-rw-r--   0 tu        (1000) tu        (1000)     1028 2023-04-23 14:38:21.000000 tradeX-0.0.2/setup.py
-drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-04-23 14:38:30.956026 tradeX-0.0.2/tradeX/
--rw-rw-r--   0 tu        (1000) tu        (1000)        0 2023-02-15 14:48:23.000000 tradeX-0.0.2/tradeX/__init__.py
-drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-04-23 14:38:30.956026 tradeX-0.0.2/tradeX.egg-info/
--rw-rw-r--   0 tu        (1000) tu        (1000)     2849 2023-04-23 14:38:30.000000 tradeX-0.0.2/tradeX.egg-info/PKG-INFO
--rw-rw-r--   0 tu        (1000) tu        (1000)      184 2023-04-23 14:38:30.000000 tradeX-0.0.2/tradeX.egg-info/SOURCES.txt
--rw-rw-r--   0 tu        (1000) tu        (1000)        1 2023-04-23 14:38:30.000000 tradeX-0.0.2/tradeX.egg-info/dependency_links.txt
--rw-rw-r--   0 tu        (1000) tu        (1000)        7 2023-04-23 14:38:30.000000 tradeX-0.0.2/tradeX.egg-info/top_level.txt
+drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-04-23 16:38:01.238098 tradeX-0.0.3/
+-rw-rw-r--   0 tu        (1000) tu        (1000)     1066 2023-04-04 16:17:18.000000 tradeX-0.0.3/LICENSE.txt
+-rw-rw-r--   0 tu        (1000) tu        (1000)     2844 2023-04-23 16:38:01.238098 tradeX-0.0.3/PKG-INFO
+-rw-rw-r--   0 tu        (1000) tu        (1000)     2444 2023-04-23 15:00:53.000000 tradeX-0.0.3/README.md
+-rw-rw-r--   0 tu        (1000) tu        (1000)      105 2023-04-23 16:24:57.000000 tradeX-0.0.3/pyproject.toml
+-rw-rw-r--   0 tu        (1000) tu        (1000)      295 2023-04-23 16:34:29.000000 tradeX-0.0.3/requirements.txt
+-rw-rw-r--   0 tu        (1000) tu        (1000)       81 2023-04-23 16:38:01.238098 tradeX-0.0.3/setup.cfg
+-rw-rw-r--   0 tu        (1000) tu        (1000)      831 2023-04-23 16:37:36.000000 tradeX-0.0.3/setup.py
+drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-04-23 16:38:01.234097 tradeX-0.0.3/tradeX/
+-rw-rw-r--   0 tu        (1000) tu        (1000)        0 2023-02-15 14:48:23.000000 tradeX-0.0.3/tradeX/__init__.py
+drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-04-23 16:38:01.234097 tradeX-0.0.3/tradeX/bots/
+-rw-rw-r--   0 tu        (1000) tu        (1000)     3363 2023-04-04 09:31:25.000000 tradeX-0.0.3/tradeX/bots/AbnormalDetectionBot.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)     3781 2023-04-23 11:21:32.000000 tradeX-0.0.3/tradeX/bots/BinanceDataBot.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)     2196 2023-04-04 09:31:25.000000 tradeX-0.0.3/tradeX/bots/LiveAbnormalDetectionBot.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)     4997 2023-04-04 09:31:25.000000 tradeX-0.0.3/tradeX/bots/LogOnlyBot.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)     3086 2023-04-04 09:31:25.000000 tradeX-0.0.3/tradeX/bots/SimpleBot.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)       29 2023-04-23 11:25:44.000000 tradeX-0.0.3/tradeX/bots/__init__.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)    13012 2023-04-04 09:31:25.000000 tradeX-0.0.3/tradeX/bots/binance_bot.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)      306 2023-02-25 07:35:17.000000 tradeX-0.0.3/tradeX/bots/consts.py
+drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-04-23 16:38:01.234097 tradeX-0.0.3/tradeX/datasets/
+-rw-rw-r--   0 tu        (1000) tu        (1000)     1372 2023-04-04 09:31:25.000000 tradeX-0.0.3/tradeX/datasets/BinanceDataset.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)     2017 2023-04-19 02:37:40.000000 tradeX-0.0.3/tradeX/datasets/ClassifierDataset.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)     4412 2023-04-15 10:36:05.000000 tradeX-0.0.3/tradeX/datasets/DirectionDataset.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)     2004 2023-04-23 07:38:57.000000 tradeX-0.0.3/tradeX/datasets/RegressionDataset.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)       39 2023-04-04 09:14:34.000000 tradeX-0.0.3/tradeX/datasets/__init__.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)      398 2023-04-04 09:14:34.000000 tradeX-0.0.3/tradeX/datasets/consts.py
+drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-04-23 16:38:01.234097 tradeX-0.0.3/tradeX/models/
+-rw-rw-r--   0 tu        (1000) tu        (1000)     2378 2023-04-09 15:05:29.000000 tradeX-0.0.3/tradeX/models/BinaryClassifier.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)     2938 2023-04-16 10:46:47.000000 tradeX-0.0.3/tradeX/models/DirectionModel.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)      804 2023-04-23 11:27:32.000000 tradeX-0.0.3/tradeX/models/EModel.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)     2140 2023-04-23 03:44:48.000000 tradeX-0.0.3/tradeX/models/FC_LSTM.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)     5282 2023-04-23 09:35:52.000000 tradeX-0.0.3/tradeX/models/RegressionModel.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)     2513 2023-04-16 06:26:29.000000 tradeX-0.0.3/tradeX/models/SimpleMLPClassifier.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)        0 2022-10-09 07:59:07.000000 tradeX-0.0.3/tradeX/models/__init__.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)     1445 2022-10-26 07:36:35.000000 tradeX-0.0.3/tradeX/models/lstm.py
+drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-04-23 16:38:01.234097 tradeX-0.0.3/tradeX/scripts/
+-rw-rw-r--   0 tu        (1000) tu        (1000)        0 2022-10-09 07:51:30.000000 tradeX-0.0.3/tradeX/scripts/__init__.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)     1047 2023-04-04 09:31:25.000000 tradeX-0.0.3/tradeX/scripts/get_all_time_data.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)     1010 2023-04-04 09:14:34.000000 tradeX-0.0.3/tradeX/scripts/split_train_val.py
+drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-04-23 16:38:01.238098 tradeX-0.0.3/tradeX/utils/
+-rw-rw-r--   0 tu        (1000) tu        (1000)        0 2022-10-09 07:38:55.000000 tradeX-0.0.3/tradeX/utils/__init__.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)     1568 2023-04-06 10:14:26.000000 tradeX-0.0.3/tradeX/utils/args.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)     4190 2023-04-06 07:24:47.000000 tradeX-0.0.3/tradeX/utils/data.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)     4221 2023-04-16 08:33:39.000000 tradeX-0.0.3/tradeX/utils/data_getter.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)     1931 2023-04-06 10:30:23.000000 tradeX-0.0.3/tradeX/utils/evaluation.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)     7198 2023-04-23 10:57:00.000000 tradeX-0.0.3/tradeX/utils/feature_engineering.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)     3339 2023-04-12 15:43:54.000000 tradeX-0.0.3/tradeX/utils/losses.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)      566 2023-04-16 10:46:47.000000 tradeX-0.0.3/tradeX/utils/model.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)     1172 2023-03-10 07:58:47.000000 tradeX-0.0.3/tradeX/utils/optimizer.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)      866 2023-04-04 09:14:34.000000 tradeX-0.0.3/tradeX/utils/time.py
+drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-04-23 16:38:01.234097 tradeX-0.0.3/tradeX.egg-info/
+-rw-rw-r--   0 tu        (1000) tu        (1000)     2844 2023-04-23 16:38:01.000000 tradeX-0.0.3/tradeX.egg-info/PKG-INFO
+-rw-rw-r--   0 tu        (1000) tu        (1000)     1286 2023-04-23 16:38:01.000000 tradeX-0.0.3/tradeX.egg-info/SOURCES.txt
+-rw-rw-r--   0 tu        (1000) tu        (1000)        1 2023-04-23 16:38:01.000000 tradeX-0.0.3/tradeX.egg-info/dependency_links.txt
+-rw-rw-r--   0 tu        (1000) tu        (1000)      296 2023-04-23 16:38:01.000000 tradeX-0.0.3/tradeX.egg-info/requires.txt
+-rw-rw-r--   0 tu        (1000) tu        (1000)       13 2023-04-23 16:38:01.000000 tradeX-0.0.3/tradeX.egg-info/top_level.txt
+drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-04-23 16:38:01.238098 tradeX-0.0.3/webui/
+-rw-rw-r--   0 tu        (1000) tu        (1000)        0 2023-04-16 07:35:30.000000 tradeX-0.0.3/webui/__init__.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)     1790 2023-04-23 13:39:25.000000 tradeX-0.0.3/webui/stream_lit.py
```

### Comparing `tradeX-0.0.2/LICENSE.txt` & `tradeX-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tradeX-0.0.2/PKG-INFO` & `tradeX-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: tradeX
-Version: 0.0.2
+Version: 0.0.3
 Summary: Machine learning based crypto currency price prediction
 Author: TaQuangTu
 Author-email: taquangtu132@gmail.com
 License: LICENSE
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# Intel-Trace
+# TradeX
 
 This project provides tool to download Binance trading data in the past. Use the data to develop a mini AI model for coin prediction.
 Follow below step to reproduce:
 
 <ol>
   <li>Install Python and required packages</li>
```

### Comparing `tradeX-0.0.2/README.md` & `tradeX-0.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Intel-Trace
+# TradeX
 
 This project provides tool to download Binance trading data in the past. Use the data to develop a mini AI model for coin prediction.
 Follow below step to reproduce:
 
 <ol>
   <li>Install Python and required packages</li>
```

### Comparing `tradeX-0.0.2/tradeX.egg-info/PKG-INFO` & `tradeX-0.0.3/tradeX.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: tradeX
-Version: 0.0.2
+Version: 0.0.3
 Summary: Machine learning based crypto currency price prediction
 Author: TaQuangTu
 Author-email: taquangtu132@gmail.com
 License: LICENSE
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# Intel-Trace
+# TradeX
 
 This project provides tool to download Binance trading data in the past. Use the data to develop a mini AI model for coin prediction.
 Follow below step to reproduce:
 
 <ol>
   <li>Install Python and required packages</li>
```

