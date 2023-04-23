# Comparing `tmp/BukeColabProject-0.4.0.tar.gz` & `tmp/BukeColabProject-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\BukeColabProject-0.4.0.tar", last modified: Sun Apr  2 08:47:14 2023, max compression
+gzip compressed data, was "dist\BukeColabProject-0.4.2.tar", last modified: Sun Apr 23 08:47:01 2023, max compression
```

## Comparing `BukeColabProject-0.4.0.tar` & `BukeColabProject-0.4.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-02 08:47:14.000000 BukeColabProject-0.4.0/
-drwxrwxrwx   0        0        0        0 2023-04-02 08:47:14.000000 BukeColabProject-0.4.0/BukeColabProject/
--rw-rw-rw-   0        0        0     8961 2023-04-02 08:47:11.000000 BukeColabProject-0.4.0/BukeColabProject/Buke_S002_buy_list.py
--rw-rw-rw-   0        0        0    17411 2023-04-02 08:39:38.000000 BukeColabProject-0.4.0/BukeColabProject/Buke_S002_sell_list.py
--rw-rw-rw-   0        0        0    21693 2023-03-19 08:57:24.000000 BukeColabProject-0.4.0/BukeColabProject/function.py
--rw-rw-rw-   0        0        0     8943 2023-03-19 08:20:07.000000 BukeColabProject-0.4.0/BukeColabProject/generate_day_price.py
--rw-rw-rw-   0        0        0     4165 2023-03-19 08:06:52.000000 BukeColabProject-0.4.0/BukeColabProject/generate_index_day_price.py
--rw-rw-rw-   0        0        0     2307 2023-03-19 08:27:27.000000 BukeColabProject-0.4.0/BukeColabProject/generate_stock_list.py
--rw-rw-rw-   0        0        0     2481 2023-03-19 07:22:24.000000 BukeColabProject-0.4.0/BukeColabProject/generate_trading_days.py
--rw-rw-rw-   0        0        0    63703 2023-03-19 08:57:24.000000 BukeColabProject-0.4.0/BukeColabProject/indicator.py
--rw-rw-rw-   0        0        0      561 2021-08-12 12:11:28.000000 BukeColabProject-0.4.0/BukeColabProject/parameter.py
--rw-rw-rw-   0        0        0     3678 2023-03-19 08:57:24.000000 BukeColabProject-0.4.0/BukeColabProject/tools.py
--rw-rw-rw-   0        0        0        0 2023-03-19 07:24:19.000000 BukeColabProject-0.4.0/BukeColabProject/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-02 08:47:14.000000 BukeColabProject-0.4.0/BukeColabProject.egg-info/
--rw-rw-rw-   0        0        0        1 2023-04-02 08:47:14.000000 BukeColabProject-0.4.0/BukeColabProject.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      472 2023-04-02 08:47:14.000000 BukeColabProject-0.4.0/BukeColabProject.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      567 2023-04-02 08:47:14.000000 BukeColabProject-0.4.0/BukeColabProject.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       17 2023-04-02 08:47:14.000000 BukeColabProject-0.4.0/BukeColabProject.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      472 2023-04-02 08:47:14.000000 BukeColabProject-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0        9 2023-03-19 07:23:35.000000 BukeColabProject-0.4.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-02 08:47:14.000000 BukeColabProject-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0      700 2023-04-02 08:47:11.000000 BukeColabProject-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 08:47:01.000000 BukeColabProject-0.4.2/
+drwxrwxrwx   0        0        0        0 2023-04-23 08:47:01.000000 BukeColabProject-0.4.2/BukeColabProject/
+-rw-rw-rw-   0        0        0     8961 2023-04-02 08:47:11.000000 BukeColabProject-0.4.2/BukeColabProject/Buke_S002_buy_list.py
+-rw-rw-rw-   0        0        0    17411 2023-04-02 08:39:38.000000 BukeColabProject-0.4.2/BukeColabProject/Buke_S002_sell_list.py
+-rw-rw-rw-   0        0        0    21693 2023-03-19 08:57:24.000000 BukeColabProject-0.4.2/BukeColabProject/function.py
+-rw-rw-rw-   0        0        0     8943 2023-03-19 08:20:07.000000 BukeColabProject-0.4.2/BukeColabProject/generate_day_price.py
+-rw-rw-rw-   0        0        0     4165 2023-03-19 08:06:52.000000 BukeColabProject-0.4.2/BukeColabProject/generate_index_day_price.py
+-rw-rw-rw-   0        0        0     2307 2023-03-19 08:27:27.000000 BukeColabProject-0.4.2/BukeColabProject/generate_stock_list.py
+-rw-rw-rw-   0        0        0     2481 2023-03-19 07:22:24.000000 BukeColabProject-0.4.2/BukeColabProject/generate_trading_days.py
+-rw-rw-rw-   0        0        0    63703 2023-03-19 08:57:24.000000 BukeColabProject-0.4.2/BukeColabProject/indicator.py
+-rw-rw-rw-   0        0        0      561 2021-08-12 12:11:28.000000 BukeColabProject-0.4.2/BukeColabProject/parameter.py
+-rw-rw-rw-   0        0        0     4116 2023-04-23 08:45:14.000000 BukeColabProject-0.4.2/BukeColabProject/tools.py
+-rw-rw-rw-   0        0        0        0 2023-03-19 07:24:19.000000 BukeColabProject-0.4.2/BukeColabProject/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 08:47:01.000000 BukeColabProject-0.4.2/BukeColabProject.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-04-23 08:47:00.000000 BukeColabProject-0.4.2/BukeColabProject.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      472 2023-04-23 08:47:00.000000 BukeColabProject-0.4.2/BukeColabProject.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      567 2023-04-23 08:47:00.000000 BukeColabProject-0.4.2/BukeColabProject.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       17 2023-04-23 08:47:00.000000 BukeColabProject-0.4.2/BukeColabProject.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      472 2023-04-23 08:47:01.000000 BukeColabProject-0.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0        9 2023-03-19 07:23:35.000000 BukeColabProject-0.4.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-23 08:47:01.000000 BukeColabProject-0.4.2/setup.cfg
+-rw-rw-rw-   0        0        0      700 2023-04-23 08:46:17.000000 BukeColabProject-0.4.2/setup.py
```

### Comparing `BukeColabProject-0.4.0/BukeColabProject/Buke_S002_buy_list.py` & `BukeColabProject-0.4.2/BukeColabProject/Buke_S002_buy_list.py`

 * *Files identical despite different names*

### Comparing `BukeColabProject-0.4.0/BukeColabProject/Buke_S002_sell_list.py` & `BukeColabProject-0.4.2/BukeColabProject/Buke_S002_sell_list.py`

 * *Files identical despite different names*

### Comparing `BukeColabProject-0.4.0/BukeColabProject/function.py` & `BukeColabProject-0.4.2/BukeColabProject/function.py`

 * *Files identical despite different names*

### Comparing `BukeColabProject-0.4.0/BukeColabProject/generate_day_price.py` & `BukeColabProject-0.4.2/BukeColabProject/generate_day_price.py`

 * *Files identical despite different names*

### Comparing `BukeColabProject-0.4.0/BukeColabProject/generate_index_day_price.py` & `BukeColabProject-0.4.2/BukeColabProject/generate_index_day_price.py`

 * *Files identical despite different names*

### Comparing `BukeColabProject-0.4.0/BukeColabProject/generate_stock_list.py` & `BukeColabProject-0.4.2/BukeColabProject/generate_stock_list.py`

 * *Files identical despite different names*

### Comparing `BukeColabProject-0.4.0/BukeColabProject/generate_trading_days.py` & `BukeColabProject-0.4.2/BukeColabProject/generate_trading_days.py`

 * *Files identical despite different names*

### Comparing `BukeColabProject-0.4.0/BukeColabProject/indicator.py` & `BukeColabProject-0.4.2/BukeColabProject/indicator.py`

 * *Files identical despite different names*

### Comparing `BukeColabProject-0.4.0/BukeColabProject/parameter.py` & `BukeColabProject-0.4.2/BukeColabProject/parameter.py`

 * *Files identical despite different names*

### Comparing `BukeColabProject-0.4.0/BukeColabProject/tools.py` & `BukeColabProject-0.4.2/BukeColabProject/tools.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 def get_hoga(price: int, market: Market) -> int:
     """
     주가에 따른 1호가 가격을 구하는 함수
     :param price: 주가
     :param market: kospi / kosdaq
     :return: 1호가 가격
     """
+
+    """ 
     if market == Market.kospi:
         if price >= 500000:
             hoga = 1000
         elif price >= 100000:
             hoga = 500
         elif price >= 50000:
             hoga = 100
@@ -38,22 +40,39 @@
             hoga = 50
         elif price >= 5000:
             hoga = 10
         elif price >= 1000:
             hoga = 5
         else:
             hoga = 1
+    """
+
+    if market == Market.kospi or market == Market.kosdaq:
+        if price >= 500000:
+            hoga = 1000
+        elif price >= 200000:
+            hoga = 500
+        elif price >= 50000:
+            hoga = 100
+        elif price >= 20000:
+            hoga = 50
+        elif price >= 5000:
+            hoga = 10
+        elif price >= 2000:
+            hoga = 5
+        else:
+            hoga = 1
+
     elif market == Market.etf:
         hoga = 5
     else:
         raise ValueError("market should be kospi or kosdaq")
 
     return hoga
 
-
 def get_bid_price(price: int or float, market: Market) -> int:
     """
     살 가격을 구하는 함수
     :param price: 현재가
     :param market: 시장
     :return: 매수 가격
     """
```

### Comparing `BukeColabProject-0.4.0/BukeColabProject.egg-info/SOURCES.txt` & `BukeColabProject-0.4.2/BukeColabProject.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `BukeColabProject-0.4.0/setup.py` & `BukeColabProject-0.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="BukeColabProject", # Replace with your own username
-    version="0.4.0",
+    version="0.4.2",
     author="Example Author",
     author_email="yesben214@gamil.com",
     description="A small example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pypa/sampleproject",
     packages=setuptools.find_packages(),
```

