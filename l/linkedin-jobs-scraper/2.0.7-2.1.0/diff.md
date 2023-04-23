# Comparing `tmp/linkedin-jobs-scraper-2.0.7.tar.gz` & `tmp/linkedin-jobs-scraper-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/linkedin-jobs-scraper-2.0.7.tar", last modified: Sat Mar 18 10:56:46 2023, max compression
+gzip compressed data, was "dist/linkedin-jobs-scraper-2.1.0.tar", last modified: Sun Apr 23 15:33:50 2023, max compression
```

## Comparing `linkedin-jobs-scraper-2.0.7.tar` & `linkedin-jobs-scraper-2.1.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 10:56:46.000000 linkedin-jobs-scraper-2.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    13306 2023-03-18 10:56:46.000000 linkedin-jobs-scraper-2.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10113 2023-03-18 10:53:28.000000 linkedin-jobs-scraper-2.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 10:56:46.000000 linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-18 10:53:28.000000 linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 10:56:46.000000 linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper/chrome_cdp/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-03-18 10:53:28.000000 linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper/chrome_cdp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-03-18 10:53:28.000000 linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper/chrome_cdp/cdp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-03-18 10:53:28.000000 linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper/chrome_cdp/cookie.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-03-18 10:53:28.000000 linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper/chrome_cdp/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-03-18 10:53:28.000000 linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper/chrome_cdp/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-03-18 10:53:28.000000 linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper/chrome_cdp/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-03-18 10:53:28.000000 linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper/chrome_cdp/target_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-18 10:53:28.000000 linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper/chrome_cdp/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-03-18 10:53:28.000000 linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 10:56:46.000000 linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper/events/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-18 10:53:28.000000 linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-03-18 10:53:28.000000 linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper/events/events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 10:56:46.000000 linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-18 10:53:28.000000 linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-03-18 10:53:28.000000 linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 10:56:46.000000 linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper/filters/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-18 10:53:28.000000 linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-03-18 10:53:28.000000 linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper/filters/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    18149 2023-03-18 10:53:28.000000 linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper/linkedin_scraper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 10:56:46.000000 linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper/query/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-18 10:53:28.000000 linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6319 2023-03-18 10:53:28.000000 linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper/query/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 10:56:46.000000 linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper/strategies/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-03-18 10:53:28.000000 linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13843 2023-03-18 10:53:28.000000 linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper/strategies/anonymous_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    22928 2023-03-18 10:53:28.000000 linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper/strategies/authenticated_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-03-18 10:53:28.000000 linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper/strategies/strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 10:56:46.000000 linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 10:53:28.000000 linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-03-18 10:53:28.000000 linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper/utils/chrome_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-18 10:53:28.000000 linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-03-18 10:53:28.000000 linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-18 10:53:28.000000 linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper/utils/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-03-18 10:53:28.000000 linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper/utils/url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-03-18 10:53:28.000000 linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper/utils/user_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 10:56:46.000000 linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13306 2023-03-18 10:56:46.000000 linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-03-18 10:56:46.000000 linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-18 10:56:46.000000 linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-18 10:56:46.000000 linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-18 10:56:46.000000 linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-18 10:56:46.000000 linkedin-jobs-scraper-2.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-03-18 10:53:28.000000 linkedin-jobs-scraper-2.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:33:50.000000 linkedin-jobs-scraper-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    13367 2023-04-23 15:33:50.000000 linkedin-jobs-scraper-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10166 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:33:50.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:33:50.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/chrome_cdp/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/chrome_cdp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/chrome_cdp/cdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/chrome_cdp/cookie.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/chrome_cdp/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/chrome_cdp/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/chrome_cdp/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/chrome_cdp/target_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/chrome_cdp/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:33:50.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/events/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/events/events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:33:50.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:33:50.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/filters/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18234 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/linkedin_scraper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:33:50.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/query/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/query/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:33:50.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13870 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/strategies/anonymous_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23067 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/strategies/authenticated_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/strategies/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:33:50.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/utils/chrome_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/utils/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/utils/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/utils/user_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:33:50.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13367 2023-04-23 15:33:49.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-04-23 15:33:50.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 15:33:49.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-23 15:33:49.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-23 15:33:49.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 15:33:50.000000 linkedin-jobs-scraper-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/setup.py
```

### Comparing `linkedin-jobs-scraper-2.0.7/PKG-INFO` & `linkedin-jobs-scraper-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkedin-jobs-scraper
-Version: 2.0.7
+Version: 2.1.0
 Summary: Scrape public available jobs on Linkedin using headless browser
 Home-page: https://github.com/spinlud/py-linkedin-jobs-scraper.git
 Author: Ludovico Fabbri
 Author-email: ludovico.fabbri@gmail.com
 License: UNKNOWN
 Description: # linkedin-jobs-scraper
         > Scrape public available jobs on Linkedin using headless browser. 
@@ -110,14 +110,15 @@
             ),
             Query(
                 query='Engineer',
                 options=QueryOptions(
                     locations=['United States', 'Europe'],
                     apply_link=True,  # Try to extract apply link (easy applies are skipped). If set to True, scraping is slower because an additional page mus be navigated. Default to False.
                     skip_promoted_jobs=True,  # Skip promoted jobs. Default to False.
+                    page_offset=2,  # How many pages to skip
                     limit=5,
                     filters=QueryFilters(
                         company_jobs_url='https://www.linkedin.com/jobs/search/?f_C=1441%2C17876832%2C791962%2C2374003%2C18950635%2C16140%2C10440912&geoId=92000000',  # Filter by companies.                
                         relevance=RelevanceFilters.RECENT,
                         time=TimeFilters.MONTH,
                         type=[TypeFilters.FULL_TIME, TypeFilters.INTERNSHIP],
                         on_site_or_remote=[OnSiteOrRemoteFilters.REMOTE],
```

### Comparing `linkedin-jobs-scraper-2.0.7/README.md` & `linkedin-jobs-scraper-2.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -102,14 +102,15 @@
     ),
     Query(
         query='Engineer',
         options=QueryOptions(
             locations=['United States', 'Europe'],
             apply_link=True,  # Try to extract apply link (easy applies are skipped). If set to True, scraping is slower because an additional page mus be navigated. Default to False.
             skip_promoted_jobs=True,  # Skip promoted jobs. Default to False.
+            page_offset=2,  # How many pages to skip
             limit=5,
             filters=QueryFilters(
                 company_jobs_url='https://www.linkedin.com/jobs/search/?f_C=1441%2C17876832%2C791962%2C2374003%2C18950635%2C16140%2C10440912&geoId=92000000',  # Filter by companies.                
                 relevance=RelevanceFilters.RECENT,
                 time=TimeFilters.MONTH,
                 type=[TypeFilters.FULL_TIME, TypeFilters.INTERNSHIP],
                 on_site_or_remote=[OnSiteOrRemoteFilters.REMOTE],
```

### Comparing `linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper/chrome_cdp/cdp.py` & `linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/chrome_cdp/cdp.py`

 * *Files identical despite different names*

### Comparing `linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper/chrome_cdp/cookie.py` & `linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/chrome_cdp/cookie.py`

 * *Files identical despite different names*

### Comparing `linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper/chrome_cdp/request.py` & `linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/chrome_cdp/request.py`

 * *Files identical despite different names*

### Comparing `linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper/chrome_cdp/response.py` & `linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/chrome_cdp/response.py`

 * *Files identical despite different names*

### Comparing `linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper/chrome_cdp/target_info.py` & `linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/chrome_cdp/target_info.py`

 * *Files identical despite different names*

### Comparing `linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper/config.py` & `linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/config.py`

 * *Files identical despite different names*

### Comparing `linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper/events/events.py` & `linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/events/events.py`

 * *Files identical despite different names*

### Comparing `linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper/filters/filters.py` & `linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/filters/filters.py`

 * *Files identical despite different names*

### Comparing `linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper/linkedin_scraper.py` & `linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/linkedin_scraper.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,14 +152,15 @@
 
         info('Starting new query', str(query))
 
         if query.options.optimize:
             warn('Query option optimize=True: this could cause issues in jobs loading or pagination')
 
         try:
+            page_offset = query.options.page_offset
             # Locations loop
             for location in query.options.locations:
                 tag = f'[{query.query}][{location}]'
                 search_url = LinkedinScraper.__build_search_url(query, location)
 
                 driver = build_driver(
                     executable_path=self.chrome_executable_path,
@@ -292,14 +293,15 @@
                 # Run strategy
                 self._strategy.run(
                     driver,
                     cdp,
                     search_url,
                     query,
                     location,
+                    page_offset,
                     # query.options.apply_link
                 )
 
                 try:
                     debug(tag, 'Stopping Chrome DevTools')
                     cdp.stop()
                 except:
```

### Comparing `linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper/query/query.py` & `linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/query/query.py`

 * *Files 6% similar despite different names*

```diff
@@ -83,27 +83,29 @@
 class QueryOptions(__Base):
     def __init__(self,
                  limit: int = None,
                  locations: List[str] = None,
                  filters: QueryFilters = None,
                  optimize: bool = None,  # Could cause instability in dynamic jobs loading
                  apply_link: bool = None,
-                 skip_promoted_jobs: bool = None):
+                 skip_promoted_jobs: bool = None,
+                 page_offset: int = 0):
 
         super().__init__()
 
         if isinstance(locations, str):
             locations = [locations]
 
         self.limit = limit
         self.locations = locations
         self.filters = filters
         self.optimize = optimize
         self.apply_link = apply_link
         self.skip_promoted_jobs = skip_promoted_jobs
+        self.page_offset = page_offset
 
     def validate(self):
         if self.limit is not None:
             if not isinstance(self.limit, int) or self.limit < 0:
                 raise ValueError('Parameter limit must be a positive integer')
 
         if self.locations is not None:
@@ -115,14 +117,18 @@
 
         if self.apply_link is not None and not isinstance(self.apply_link, bool):
             raise ValueError('Parameter apply_link must be a boolean')
 
         if self.skip_promoted_jobs is not None and not isinstance(self.skip_promoted_jobs, bool):
             raise ValueError('Parameter skip_promoted_jobs must be a boolean')
 
+        if self.page_offset is not None:
+            if not isinstance(self.page_offset, int) or self.page_offset < 0:
+                raise ValueError('Parameter page_offset must be a positive integer')
+
         if self.filters is not None:
             self.filters.validate()
 
 
 class Query(__Base):
     def __init__(self, query: str = '', options: QueryOptions = QueryOptions()):
         super().__init__()
```

### Comparing `linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper/strategies/anonymous_strategy.py` & `linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/strategies/anonymous_strategy.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,24 +181,25 @@
 
     def run(
         self,
         driver: webdriver,
         cdp: CDP,
         search_url: str,
         query: Query,
-        location: str
+        location: str,
+        page_offset: int,
     ) -> None:
         """
         Run scraper
         :param driver: webdriver
         :param cdp: CDP
         :param search_url: str
         :param query: Query
         :param location: str
-        :param apply_link: bool
+        :param page_offset: int
         :return: None
         """
 
         tag = f'[{query.query}][{location}]'
         processed = 0
 
         info(tag, f'Opening {search_url}')
```

### Comparing `linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper/strategies/authenticated_strategy.py` & `linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/strategies/authenticated_strategy.py`

 * *Files 1% similar despite different names*

```diff
@@ -263,32 +263,33 @@
 
     def run(
         self,
         driver: webdriver,
         cdp: CDP,
         search_url: str,
         query: Query,
-        location: str
+        location: str,
+        page_offset: int,
     ) -> None:
         """
         Run strategy
         :param driver: webdriver
         :param cdp: CDP
         :param search_url: str
         :param query: Query
         :param location: str
-        :param apply_link: bool
+        :param page_offset: int
         :return: None
         """
 
         tag = f'[{query.query}][{location}]'
 
         metrics = EventMetrics()
 
-        pagination_index = 0
+        pagination_index = page_offset
         pagination_size = 25
 
         # Open main page first to verify/set the session
         debug(tag, f'Opening {HOME_URL}')
         driver.get(HOME_URL)
         sleep(self.scraper.slow_mo)
 
@@ -303,14 +304,15 @@
                 })
             except BaseException as e:
                 error(tag, e)
                 error(tag, traceback.format_exc())
                 return
 
         # Open search url
+        search_url = override_query_params(search_url, {'start': pagination_index * pagination_size})
         info(tag, f'Opening {search_url}')
         driver.get(search_url)
         sleep(self.scraper.slow_mo)
 
         # Verify session
         if not AuthenticatedStrategy.__is_authenticated_session(driver):
             message = 'The provided session cookie is invalid. ' \
```

### Comparing `linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper/utils/chrome_driver.py` & `linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/utils/chrome_driver.py`

 * *Files identical despite different names*

### Comparing `linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper/utils/logger.py` & `linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/utils/logger.py`

 * *Files identical despite different names*

### Comparing `linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper/utils/url.py` & `linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/utils/url.py`

 * *Files identical despite different names*

### Comparing `linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper/utils/user_agent.py` & `linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/utils/user_agent.py`

 * *Files identical despite different names*

### Comparing `linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper.egg-info/PKG-INFO` & `linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkedin-jobs-scraper
-Version: 2.0.7
+Version: 2.1.0
 Summary: Scrape public available jobs on Linkedin using headless browser
 Home-page: https://github.com/spinlud/py-linkedin-jobs-scraper.git
 Author: Ludovico Fabbri
 Author-email: ludovico.fabbri@gmail.com
 License: UNKNOWN
 Description: # linkedin-jobs-scraper
         > Scrape public available jobs on Linkedin using headless browser. 
@@ -110,14 +110,15 @@
             ),
             Query(
                 query='Engineer',
                 options=QueryOptions(
                     locations=['United States', 'Europe'],
                     apply_link=True,  # Try to extract apply link (easy applies are skipped). If set to True, scraping is slower because an additional page mus be navigated. Default to False.
                     skip_promoted_jobs=True,  # Skip promoted jobs. Default to False.
+                    page_offset=2,  # How many pages to skip
                     limit=5,
                     filters=QueryFilters(
                         company_jobs_url='https://www.linkedin.com/jobs/search/?f_C=1441%2C17876832%2C791962%2C2374003%2C18950635%2C16140%2C10440912&geoId=92000000',  # Filter by companies.                
                         relevance=RelevanceFilters.RECENT,
                         time=TimeFilters.MONTH,
                         type=[TypeFilters.FULL_TIME, TypeFilters.INTERNSHIP],
                         on_site_or_remote=[OnSiteOrRemoteFilters.REMOTE],
```

### Comparing `linkedin-jobs-scraper-2.0.7/linkedin_jobs_scraper.egg-info/SOURCES.txt` & `linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `linkedin-jobs-scraper-2.0.7/setup.py` & `linkedin-jobs-scraper-2.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='linkedin-jobs-scraper',
-    version='2.0.7',
+    version='2.1.0',
     author='Ludovico Fabbri',
     author_email='ludovico.fabbri@gmail.com',
     description='Scrape public available jobs on Linkedin using headless browser',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/spinlud/py-linkedin-jobs-scraper.git',
     packages=[
```

