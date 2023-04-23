# Comparing `tmp/secapi-tl-1.1.7.tar.gz` & `tmp/secapi-tl-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secapi-tl-1.1.7.tar", last modified: Sun Apr 23 16:01:59 2023, max compression
+gzip compressed data, was "secapi-tl-1.1.8.tar", last modified: Sun Apr 23 19:25:10 2023, max compression
```

## Comparing `secapi-tl-1.1.7.tar` & `secapi-tl-1.1.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-23 16:01:59.165676 secapi-tl-1.1.7/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1063 2022-10-14 12:06:38.000000 secapi-tl-1.1.7/LICENSE
--rw-rw-r--   0 tom       (1000) tom       (1000)     5137 2023-04-23 16:01:59.165676 secapi-tl-1.1.7/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)     3698 2023-04-09 10:03:28.000000 secapi-tl-1.1.7/README.md
--rw-rw-r--   0 tom       (1000) tom       (1000)      391 2023-04-23 16:01:08.000000 secapi-tl-1.1.7/pyproject.toml
--rw-rw-r--   0 tom       (1000) tom       (1000)       38 2023-04-23 16:01:59.165676 secapi-tl-1.1.7/setup.cfg
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-23 16:01:59.161676 secapi-tl-1.1.7/src/
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-23 16:01:59.165676 secapi-tl-1.1.7/src/secapi_tl/
--rw-rw-r--   0 tom       (1000) tom       (1000)      299 2023-04-08 12:35:48.000000 secapi-tl-1.1.7/src/secapi_tl/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     6136 2023-04-15 21:09:49.000000 secapi-tl-1.1.7/src/secapi_tl/filing.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     4053 2023-04-15 16:38:29.000000 secapi-tl-1.1.7/src/secapi_tl/filing_query.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      989 2022-10-14 21:27:13.000000 secapi-tl-1.1.7/src/secapi_tl/key_mapper.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1175 2023-04-23 15:57:28.000000 secapi-tl-1.1.7/src/secapi_tl/request.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-23 16:01:59.165676 secapi-tl-1.1.7/src/secapi_tl.egg-info/
--rw-rw-r--   0 tom       (1000) tom       (1000)     5137 2023-04-23 16:01:59.000000 secapi-tl-1.1.7/src/secapi_tl.egg-info/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)      349 2023-04-23 16:01:59.000000 secapi-tl-1.1.7/src/secapi_tl.egg-info/SOURCES.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)        1 2023-04-23 16:01:59.000000 secapi-tl-1.1.7/src/secapi_tl.egg-info/dependency_links.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       42 2023-04-23 16:01:59.000000 secapi-tl-1.1.7/src/secapi_tl.egg-info/requires.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       10 2023-04-23 16:01:59.000000 secapi-tl-1.1.7/src/secapi_tl.egg-info/top_level.txt
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-23 19:25:10.049290 secapi-tl-1.1.8/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1063 2022-10-14 12:06:38.000000 secapi-tl-1.1.8/LICENSE
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4873 2023-04-23 19:25:10.049290 secapi-tl-1.1.8/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3434 2023-04-23 18:15:51.000000 secapi-tl-1.1.8/README.md
+-rw-rw-r--   0 tom       (1000) tom       (1000)      391 2023-04-23 18:15:51.000000 secapi-tl-1.1.8/pyproject.toml
+-rw-rw-r--   0 tom       (1000) tom       (1000)       38 2023-04-23 19:25:10.049290 secapi-tl-1.1.8/setup.cfg
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-23 19:25:10.049290 secapi-tl-1.1.8/src/
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-23 19:25:10.049290 secapi-tl-1.1.8/src/secapi_tl/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      307 2023-04-23 18:15:51.000000 secapi-tl-1.1.8/src/secapi_tl/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     6136 2023-04-15 21:09:49.000000 secapi-tl-1.1.8/src/secapi_tl/filing.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4041 2023-04-23 18:15:51.000000 secapi-tl-1.1.8/src/secapi_tl/filing_query.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      977 2023-04-23 16:14:09.000000 secapi-tl-1.1.8/src/secapi_tl/key_mapper.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      824 2023-04-23 19:21:29.000000 secapi-tl-1.1.8/src/secapi_tl/request.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-23 19:25:10.049290 secapi-tl-1.1.8/src/secapi_tl.egg-info/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4873 2023-04-23 19:25:10.000000 secapi-tl-1.1.8/src/secapi_tl.egg-info/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)      349 2023-04-23 19:25:10.000000 secapi-tl-1.1.8/src/secapi_tl.egg-info/SOURCES.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)        1 2023-04-23 19:25:10.000000 secapi-tl-1.1.8/src/secapi_tl.egg-info/dependency_links.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       42 2023-04-23 19:25:10.000000 secapi-tl-1.1.8/src/secapi_tl.egg-info/requires.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       10 2023-04-23 19:25:10.000000 secapi-tl-1.1.8/src/secapi_tl.egg-info/top_level.txt
```

### Comparing `secapi-tl-1.1.7/LICENSE` & `secapi-tl-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `secapi-tl-1.1.7/PKG-INFO` & `secapi-tl-1.1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secapi-tl
-Version: 1.1.7
+Version: 1.1.8
 License: MIT License
         
         Copyright (c) 2022 tlie03
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -84,28 +84,24 @@
 These metadata can then be used to create the links to the actual filings.
 The process of finding a way to build the links from the metadata can be quite difficult, 
 and requires a lot of experimentation.
 
 ### How to make requests to the sec server
 The sec has restricted the access to their servers .Thereby it is not allowed
 to do more than 10 requests per second. To ensure that the amount of requests stays
-within the boundaries set by the sec this package provides the `Request.sec_request`
+within the boundaries set by the sec this package provides the `sec_request`
 function which can be used to do requests to the sec servers. The
 function has a ratelimiter which ensures that the function can only be executed
 10 times per second. Due to the sleep and retry property of the function
 the user does not have to worry about the number of function calls he makes.
 Furthermore, all code segments in this package that make requests
 to the sec servers use the same function as well. Thereby the request limit
-can not be exceeded when alle requests are made with the `Request.sec_request`
+can not be exceeded when alle requests are made with the `sec_request`
 function. Because of that it is necessary that a user of this API uses
 this function for all requests to the sec servers otherwise problems can occur.
 
-The `Request.sec_request` function takes in three parameters which are:
-* url : the url that will be requested
-* header : the header of the request which by default only contains a User-Agent
-* retries : the number of retries which is 5 by default
 
 ### Utility functions
 * `get_cik` can be used to get the cik that belongs to a ticker symbol
 * `is_registered` can be used to proof if a company is registered at the sec
 
 Both functions take the ticker symbol of the company as an argument
```

### Comparing `secapi-tl-1.1.7/README.md` & `secapi-tl-1.1.8/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -54,28 +54,24 @@
 These metadata can then be used to create the links to the actual filings.
 The process of finding a way to build the links from the metadata can be quite difficult, 
 and requires a lot of experimentation.
 
 ### How to make requests to the sec server
 The sec has restricted the access to their servers .Thereby it is not allowed
 to do more than 10 requests per second. To ensure that the amount of requests stays
-within the boundaries set by the sec this package provides the `Request.sec_request`
+within the boundaries set by the sec this package provides the `sec_request`
 function which can be used to do requests to the sec servers. The
 function has a ratelimiter which ensures that the function can only be executed
 10 times per second. Due to the sleep and retry property of the function
 the user does not have to worry about the number of function calls he makes.
 Furthermore, all code segments in this package that make requests
 to the sec servers use the same function as well. Thereby the request limit
-can not be exceeded when alle requests are made with the `Request.sec_request`
+can not be exceeded when alle requests are made with the `sec_request`
 function. Because of that it is necessary that a user of this API uses
 this function for all requests to the sec servers otherwise problems can occur.
 
-The `Request.sec_request` function takes in three parameters which are:
-* url : the url that will be requested
-* header : the header of the request which by default only contains a User-Agent
-* retries : the number of retries which is 5 by default
 
 ### Utility functions
 * `get_cik` can be used to get the cik that belongs to a ticker symbol
 * `is_registered` can be used to proof if a company is registered at the sec
 
 Both functions take the ticker symbol of the company as an argument
```

### Comparing `secapi-tl-1.1.7/src/secapi_tl/filing.py` & `secapi-tl-1.1.8/src/secapi_tl/filing.py`

 * *Files identical despite different names*

### Comparing `secapi-tl-1.1.7/src/secapi_tl/filing_query.py` & `secapi-tl-1.1.8/src/secapi_tl/filing_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import List
 from warnings import warn
 from openDateRange import DateRange
 
-from .request import Request
+from .request import sec_request
 from .key_mapper import get_cik
 from .filing import Filing
 
 # list of keys for all existing metadata points
 FILING_INFORMATION_KEYS = ['accessionNumber',
                            'filingDate',
                            'reportDate',
@@ -55,29 +55,29 @@
 
     # get the main submissions file
     cik = get_cik(ticker_symbol)
     length_diff = REQUIRED_CIK_LENGTH - len(cik)
     cik_formatted = ('0' * length_diff) + cik
     submissions_url = BASE_URL_SUBMISSIONS + CIK_STRING + cik_formatted + JSON_FILE
 
-    response = Request.sec_request(url=submissions_url)
+    response = sec_request(url=submissions_url)
     submissions_dict = response.json()
 
     filings = []
     # parse recent
     data = submissions_dict['filings']['recent']
     if search_daterange.intersects(date_from=data['filingDate'][-1], date_to=data['filingDate'][0]):
         filings += filter_filings(data, checker, information_keys, cik, ticker_symbol)
 
     # parse files
     files = submissions_dict['filings']['files']
     for file in files:
         if search_daterange.intersects(date_from=file['filingFrom'], date_to=file['filingTo']):
             url = BASE_URL_SUBMISSIONS + file['name']
-            response = Request.sec_request(url=url)
+            response = sec_request(url=url)
             data = response.json()
             filings += filter_filings(data, checker, information_keys, cik, ticker_symbol)
 
     return [Filing.from_dict(filing_dict=filing) for filing in filings]
 
 
 def filter_filings(raw_filings, checker, required_information, cik, ticker_symbol):
```

### Comparing `secapi-tl-1.1.7/src/secapi_tl/key_mapper.py` & `secapi-tl-1.1.8/src/secapi_tl/key_mapper.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-from .request import Request
+from .request import sec_request
 
 # a file maintained by the sec that holds all ticker symbols and their corresponding cik
 SEC_CIK_TICKERS_DATA = r"https://www.sec.gov/files/company_tickers.json"
 
 
 def get_cik(ticker_symbol: str) -> str:
     # returns the cik that belongs to the company with the given ticker symbol
     ticker = ticker_symbol.upper()
-    response = Request.sec_request(SEC_CIK_TICKERS_DATA)
+    response = sec_request(SEC_CIK_TICKERS_DATA)
     data = response.json()
 
     for entry in data.values():
         if entry['ticker'] == ticker:
             return str(entry['cik_str'])
     raise ValueError(f'ticker symbol {ticker} not found')
 
 
 def is_registered(ticker_symbol: str) -> bool:
     # proofs whether the company with the given ticker symbol is registered at the sec or not
     ticker = ticker_symbol.upper()
-    response = Request.sec_request(SEC_CIK_TICKERS_DATA)
+    response = sec_request(SEC_CIK_TICKERS_DATA)
     data = response.json()
 
     for entry in data.values():
         if entry['ticker'] == ticker:
             return True
     else:
         return False
```

### Comparing `secapi-tl-1.1.7/src/secapi_tl.egg-info/PKG-INFO` & `secapi-tl-1.1.8/src/secapi_tl.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secapi-tl
-Version: 1.1.7
+Version: 1.1.8
 License: MIT License
         
         Copyright (c) 2022 tlie03
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -84,28 +84,24 @@
 These metadata can then be used to create the links to the actual filings.
 The process of finding a way to build the links from the metadata can be quite difficult, 
 and requires a lot of experimentation.
 
 ### How to make requests to the sec server
 The sec has restricted the access to their servers .Thereby it is not allowed
 to do more than 10 requests per second. To ensure that the amount of requests stays
-within the boundaries set by the sec this package provides the `Request.sec_request`
+within the boundaries set by the sec this package provides the `sec_request`
 function which can be used to do requests to the sec servers. The
 function has a ratelimiter which ensures that the function can only be executed
 10 times per second. Due to the sleep and retry property of the function
 the user does not have to worry about the number of function calls he makes.
 Furthermore, all code segments in this package that make requests
 to the sec servers use the same function as well. Thereby the request limit
-can not be exceeded when alle requests are made with the `Request.sec_request`
+can not be exceeded when alle requests are made with the `sec_request`
 function. Because of that it is necessary that a user of this API uses
 this function for all requests to the sec servers otherwise problems can occur.
 
-The `Request.sec_request` function takes in three parameters which are:
-* url : the url that will be requested
-* header : the header of the request which by default only contains a User-Agent
-* retries : the number of retries which is 5 by default
 
 ### Utility functions
 * `get_cik` can be used to get the cik that belongs to a ticker symbol
 * `is_registered` can be used to proof if a company is registered at the sec
 
 Both functions take the ticker symbol of the company as an argument
```

