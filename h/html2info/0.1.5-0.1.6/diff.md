# Comparing `tmp/html2info-0.1.5.tar.gz` & `tmp/html2info-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "html2info-0.1.5.tar", last modified: Sun Apr 23 00:43:56 2023, max compression
+gzip compressed data, was "html2info-0.1.6.tar", last modified: Sun Apr 23 00:59:59 2023, max compression
```

## Comparing `html2info-0.1.5.tar` & `html2info-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-04-23 00:43:56.810199 html2info-0.1.5/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     6013 2023-04-23 00:43:56.810199 html2info-0.1.5/PKG-INFO
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     5278 2023-04-20 20:54:37.000000 html2info-0.1.5/README.md
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-04-23 00:43:56.810199 html2info-0.1.5/html2info/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)        0 2023-04-19 18:56:39.000000 html2info-0.1.5/html2info/__init__.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     5002 2023-04-23 00:28:59.000000 html2info-0.1.5/html2info/linkedin.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      439 2023-04-23 00:43:09.000000 html2info-0.1.5/html2info/types.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      190 2023-04-19 19:16:29.000000 html2info-0.1.5/html2info/utils.py
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-04-23 00:43:56.810199 html2info-0.1.5/html2info.egg-info/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     6013 2023-04-23 00:43:56.000000 html2info-0.1.5/html2info.egg-info/PKG-INFO
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      279 2023-04-23 00:43:56.000000 html2info-0.1.5/html2info.egg-info/SOURCES.txt
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)        1 2023-04-23 00:43:56.000000 html2info-0.1.5/html2info.egg-info/dependency_links.txt
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       23 2023-04-23 00:43:56.000000 html2info-0.1.5/html2info.egg-info/requires.txt
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       10 2023-04-23 00:43:56.000000 html2info-0.1.5/html2info.egg-info/top_level.txt
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1475 2023-04-23 00:41:00.000000 html2info-0.1.5/pyproject.toml
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       38 2023-04-23 00:43:56.810199 html2info-0.1.5/setup.cfg
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1360 2023-04-23 00:43:25.000000 html2info-0.1.5/setup.py
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-04-23 00:59:59.955166 html2info-0.1.6/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     6013 2023-04-23 00:59:59.955166 html2info-0.1.6/PKG-INFO
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     5278 2023-04-20 20:54:37.000000 html2info-0.1.6/README.md
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-04-23 00:59:59.955166 html2info-0.1.6/html2info/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)        0 2023-04-19 18:56:39.000000 html2info-0.1.6/html2info/__init__.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     5034 2023-04-23 00:59:23.000000 html2info-0.1.6/html2info/linkedin.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      439 2023-04-23 00:43:09.000000 html2info-0.1.6/html2info/types.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      190 2023-04-19 19:16:29.000000 html2info-0.1.6/html2info/utils.py
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-04-23 00:59:59.955166 html2info-0.1.6/html2info.egg-info/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     6013 2023-04-23 00:59:59.000000 html2info-0.1.6/html2info.egg-info/PKG-INFO
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      279 2023-04-23 00:59:59.000000 html2info-0.1.6/html2info.egg-info/SOURCES.txt
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)        1 2023-04-23 00:59:59.000000 html2info-0.1.6/html2info.egg-info/dependency_links.txt
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       23 2023-04-23 00:59:59.000000 html2info-0.1.6/html2info.egg-info/requires.txt
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       10 2023-04-23 00:59:59.000000 html2info-0.1.6/html2info.egg-info/top_level.txt
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1475 2023-04-23 00:41:00.000000 html2info-0.1.6/pyproject.toml
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       38 2023-04-23 00:59:59.955166 html2info-0.1.6/setup.cfg
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1360 2023-04-23 00:58:54.000000 html2info-0.1.6/setup.py
```

### Comparing `html2info-0.1.5/PKG-INFO` & `html2info-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html2info
-Version: 0.1.5
+Version: 0.1.6
 Summary: A package to parse raw HTML and return structured information.
 Author: Vladimir Iglovikov
 Author-email: iglovikov@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `html2info-0.1.5/README.md` & `html2info-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `html2info-0.1.5/html2info/linkedin.py` & `html2info-0.1.6/html2info/linkedin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Optional
+
 from bs4 import BeautifulSoup
 
 from html2info.types import EducationType, ExperienceType
 
 
 class Person:
     def __init__(self, linkein_url: str, raw_html: str) -> None:
@@ -26,15 +28,15 @@
         profile_photo = self.soup.find("img", {"alt": self.name})
         self.profile_photo_link = profile_photo["src"] if profile_photo else None
 
         self.parse_about()
         self.parse_experience()
         self.parse_education()
 
-    def find_section_by_id(self, section_name: str) -> BeautifulSoup | None:
+    def find_section_by_id(self, section_name: str) -> Optional[BeautifulSoup]:
         div = self.soup.find("div", {"id": section_name})
         return None if div is None else div.find_parent("section")
 
     def parse_about(self):
         # Find the span containing the text
         # Find the parent container with specific class
         parent_container = self.soup.find(
```

### Comparing `html2info-0.1.5/html2info.egg-info/PKG-INFO` & `html2info-0.1.6/html2info.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html2info
-Version: 0.1.5
+Version: 0.1.6
 Summary: A package to parse raw HTML and return structured information.
 Author: Vladimir Iglovikov
 Author-email: iglovikov@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `html2info-0.1.5/pyproject.toml` & `html2info-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `html2info-0.1.5/setup.py` & `html2info-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="html2info",  # Replace with your package name
-    version="0.1.5",  # Replace with your package version
+    version="0.1.6",  # Replace with your package version
     author="Vladimir Iglovikov",  # Replace with your name
     author_email="iglovikov@gmail.com",  # Replace with your email
     description="A package to parse raw HTML and return structured information.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(exclude=["tests"]),
     classifiers=[
```

