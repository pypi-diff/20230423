# Comparing `tmp/NewsArticlesScraper-0.2.1.tar.gz` & `tmp/NewsArticlesScraper-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NewsArticlesScraper-0.2.1.tar", last modified: Thu Apr 20 12:41:00 2023, max compression
+gzip compressed data, was "NewsArticlesScraper-0.2.2.tar", last modified: Sun Apr 23 16:14:29 2023, max compression
```

## Comparing `NewsArticlesScraper-0.2.1.tar` & `NewsArticlesScraper-0.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 12:41:00.119482 NewsArticlesScraper-0.2.1/
-drwxrwxrwx   0        0        0        0 2023-04-20 12:41:00.095483 NewsArticlesScraper-0.2.1/NewsArticlesScraper/
--rw-rw-rw-   0        0        0    13762 2023-04-20 12:33:03.000000 NewsArticlesScraper-0.2.1/NewsArticlesScraper/Scrapers.py
--rw-rw-rw-   0        0        0       64 2023-02-14 20:15:57.000000 NewsArticlesScraper-0.2.1/NewsArticlesScraper/__init__.py
--rw-rw-rw-   0        0        0     1138 2023-04-20 12:35:55.000000 NewsArticlesScraper-0.2.1/NewsArticlesScraper/test.py
-drwxrwxrwx   0        0        0        0 2023-04-20 12:41:00.117980 NewsArticlesScraper-0.2.1/NewsArticlesScraper.egg-info/
--rw-rw-rw-   0        0        0      648 2023-04-20 12:41:00.000000 NewsArticlesScraper-0.2.1/NewsArticlesScraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      324 2023-04-20 12:41:00.000000 NewsArticlesScraper-0.2.1/NewsArticlesScraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 12:41:00.000000 NewsArticlesScraper-0.2.1/NewsArticlesScraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-04-20 12:41:00.000000 NewsArticlesScraper-0.2.1/NewsArticlesScraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-04-20 12:41:00.000000 NewsArticlesScraper-0.2.1/NewsArticlesScraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      648 2023-04-20 12:41:00.118982 NewsArticlesScraper-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-02-14 20:04:13.000000 NewsArticlesScraper-0.2.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-20 12:41:00.119482 NewsArticlesScraper-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      996 2023-04-20 12:40:52.000000 NewsArticlesScraper-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 16:14:29.823987 NewsArticlesScraper-0.2.2/
+drwxrwxrwx   0        0        0        0 2023-04-23 16:14:29.803987 NewsArticlesScraper-0.2.2/NewsArticlesScraper/
+-rw-rw-rw-   0        0        0    13787 2023-04-23 16:14:17.000000 NewsArticlesScraper-0.2.2/NewsArticlesScraper/Scrapers.py
+-rw-rw-rw-   0        0        0       64 2023-02-14 20:15:57.000000 NewsArticlesScraper-0.2.2/NewsArticlesScraper/__init__.py
+-rw-rw-rw-   0        0        0     1074 2023-04-23 16:12:20.000000 NewsArticlesScraper-0.2.2/NewsArticlesScraper/test.py
+drwxrwxrwx   0        0        0        0 2023-04-23 16:14:29.822486 NewsArticlesScraper-0.2.2/NewsArticlesScraper.egg-info/
+-rw-rw-rw-   0        0        0      648 2023-04-23 16:14:29.000000 NewsArticlesScraper-0.2.2/NewsArticlesScraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      324 2023-04-23 16:14:29.000000 NewsArticlesScraper-0.2.2/NewsArticlesScraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 16:14:29.000000 NewsArticlesScraper-0.2.2/NewsArticlesScraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-04-23 16:14:29.000000 NewsArticlesScraper-0.2.2/NewsArticlesScraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-04-23 16:14:29.000000 NewsArticlesScraper-0.2.2/NewsArticlesScraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      648 2023-04-23 16:14:29.823486 NewsArticlesScraper-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-02-14 20:04:13.000000 NewsArticlesScraper-0.2.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-23 16:14:29.823987 NewsArticlesScraper-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      996 2023-04-23 16:14:17.000000 NewsArticlesScraper-0.2.2/setup.py
```

### Comparing `NewsArticlesScraper-0.2.1/NewsArticlesScraper/Scrapers.py` & `NewsArticlesScraper-0.2.2/NewsArticlesScraper/Scrapers.py`

 * *Files 1% similar despite different names*

```diff
@@ -239,15 +239,15 @@
     name = 'TheGuardian'
     allowed_domains = ['theguardian.com', 'content.guardianapis.com']
     custom_settings = {
         'LOG_LEVEL': 'WARN',
         'USER_AGENT': 'Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.1 (KHTML, like Gecko) Chrome/22.0.1207.1 '
                       'Safari/537.1',
         'ROBOTSTXT_OBEY': False,
-        'DOWNLOAD_DELAY': 1,
+        'DOWNLOAD_DELAY': 6,
         # 'JOBDIR': './News/TheGuardianJobs',
         'REQUEST_FINGERPRINTER_IMPLEMENTATION': '2.7',
         'DOWNLOAD_TIMEOUT': 300,
         'DOWNLOADER_MIDDLEWARES': {
             'scrapy.downloadermiddlewares.useragent.UserAgentMiddleware': None,
             'scrapy_user_agents.middlewares.RandomUserAgentMiddleware': 400,
         },
@@ -279,15 +279,15 @@
             yield scrapy.Request(to_request_url, callback=self.parse_api)
 
     def parse_api(self, response):
         data = response.json()["response"]
         articles = data["results"]
         for article in articles:
             yield scrapy.Request(url=article["webUrl"], callback=self.parse_article,
-                                 meta={"time": article["webPublicationDate"]})
+                                 meta={"time": ciso8601.parse_datetime(article["webPublicationDate"])})
 
     def parse_article(self, response):
         yield self.parse_article_func(response, response.meta)
 
     @staticmethod
     def parse_article_func(response, meta):
         title = response.css(".dcr-y70mar ::text").get()
```

### Comparing `NewsArticlesScraper-0.2.1/NewsArticlesScraper/test.py` & `NewsArticlesScraper-0.2.2/NewsArticlesScraper/test.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,24 +4,23 @@
 import datetime
 import pytz
 
 from NewsArticlesScraper.Scrapers import NYTSpider, CNBCSpider, TheGuardianSpider
 
 
 def print_(item):
-    if item["author_name"] == "" or item["title"] == "" or item["body"] == "":
-        print(item)
+    print(type(item["time"]))
 
 
 def main():
     crawler = CrawlerProcess()
     dispatcher.connect(print_, signal=signals.item_passed)
     from_stamp = datetime.datetime.fromtimestamp(1628208000).replace(tzinfo=pytz.timezone("GMT"))
     to_stamp = datetime.datetime.now(tz=pytz.timezone("GMT"))
-    crawler.crawl(CNBCSpider, from_stamp, to_stamp)
+    crawler.crawl(TheGuardianSpider, from_stamp, to_stamp)
     crawler.start()
 
 
 def main2():
     from scrapy.selector import Selector
     from scrapy.http import HtmlResponse
     import requests
@@ -32,8 +31,8 @@
     data = requests.get(url).text
 
     response = HtmlResponse(url=url, body=data, encoding="utf-8")
     print(parse_cnbc(response, {"time": "wdwd"}))
 
 
 if __name__ == "__main__":
-    main2()
+    main()
```

### Comparing `NewsArticlesScraper-0.2.1/NewsArticlesScraper.egg-info/PKG-INFO` & `NewsArticlesScraper-0.2.2/NewsArticlesScraper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NewsArticlesScraper
-Version: 0.2.1
+Version: 0.2.2
 Summary: Scraping news articles
 Author: PySlayer (Paul Antweiler)
 Author-email: antweiler.paul@gmail.com
 Keywords: python,news,scraping,news scraping,news articles
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `NewsArticlesScraper-0.2.1/PKG-INFO` & `NewsArticlesScraper-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NewsArticlesScraper
-Version: 0.2.1
+Version: 0.2.2
 Summary: Scraping news articles
 Author: PySlayer (Paul Antweiler)
 Author-email: antweiler.paul@gmail.com
 Keywords: python,news,scraping,news scraping,news articles
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `NewsArticlesScraper-0.2.1/setup.py` & `NewsArticlesScraper-0.2.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.2.1'
+VERSION = '0.2.2'
 DESCRIPTION = 'Scraping news articles'
 LONG_DESCRIPTION = 'A package that allows you to scrape news articles from various news sites via scrapy.'
 
 # Setting up
 setup(
     name="NewsArticlesScraper",
     version=VERSION,
```

