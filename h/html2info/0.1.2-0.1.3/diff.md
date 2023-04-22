# Comparing `tmp/html2info-0.1.2.tar.gz` & `tmp/html2info-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "html2info-0.1.2.tar", last modified: Thu Apr 20 20:58:01 2023, max compression
+gzip compressed data, was "html2info-0.1.3.tar", last modified: Sat Apr 22 23:02:15 2023, max compression
```

## Comparing `html2info-0.1.2.tar` & `html2info-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-04-20 20:58:01.828477 html2info-0.1.2/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     6013 2023-04-20 20:58:01.828477 html2info-0.1.2/PKG-INFO
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     5278 2023-04-20 20:54:37.000000 html2info-0.1.2/README.md
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-04-20 20:58:01.828477 html2info-0.1.2/html2info/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)        0 2023-04-19 18:56:39.000000 html2info-0.1.2/html2info/__init__.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     4720 2023-04-20 20:52:29.000000 html2info-0.1.2/html2info/linkedin.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      190 2023-04-19 19:16:29.000000 html2info-0.1.2/html2info/utils.py
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-04-20 20:58:01.828477 html2info-0.1.2/html2info.egg-info/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     6013 2023-04-20 20:58:01.000000 html2info-0.1.2/html2info.egg-info/PKG-INFO
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      260 2023-04-20 20:58:01.000000 html2info-0.1.2/html2info.egg-info/SOURCES.txt
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)        1 2023-04-20 20:58:01.000000 html2info-0.1.2/html2info.egg-info/dependency_links.txt
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       23 2023-04-20 20:58:01.000000 html2info-0.1.2/html2info.egg-info/requires.txt
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       10 2023-04-20 20:58:01.000000 html2info-0.1.2/html2info.egg-info/top_level.txt
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1478 2023-04-19 22:54:36.000000 html2info-0.1.2/pyproject.toml
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       38 2023-04-20 20:58:01.828477 html2info-0.1.2/setup.cfg
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1360 2023-04-20 20:54:01.000000 html2info-0.1.2/setup.py
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-04-22 23:02:15.034994 html2info-0.1.3/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     6013 2023-04-22 23:02:15.034994 html2info-0.1.3/PKG-INFO
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     5278 2023-04-20 20:54:37.000000 html2info-0.1.3/README.md
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-04-22 23:02:15.034994 html2info-0.1.3/html2info/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)        0 2023-04-19 18:56:39.000000 html2info-0.1.3/html2info/__init__.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     4802 2023-04-22 22:58:54.000000 html2info-0.1.3/html2info/linkedin.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      190 2023-04-19 19:16:29.000000 html2info-0.1.3/html2info/utils.py
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-04-22 23:02:15.034994 html2info-0.1.3/html2info.egg-info/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     6013 2023-04-22 23:02:15.000000 html2info-0.1.3/html2info.egg-info/PKG-INFO
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      260 2023-04-22 23:02:15.000000 html2info-0.1.3/html2info.egg-info/SOURCES.txt
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)        1 2023-04-22 23:02:15.000000 html2info-0.1.3/html2info.egg-info/dependency_links.txt
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       23 2023-04-22 23:02:15.000000 html2info-0.1.3/html2info.egg-info/requires.txt
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       10 2023-04-22 23:02:15.000000 html2info-0.1.3/html2info.egg-info/top_level.txt
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1478 2023-04-19 22:54:36.000000 html2info-0.1.3/pyproject.toml
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       38 2023-04-22 23:02:15.034994 html2info-0.1.3/setup.cfg
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1360 2023-04-22 23:00:55.000000 html2info-0.1.3/setup.py
```

### Comparing `html2info-0.1.2/PKG-INFO` & `html2info-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html2info
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package to parse raw HTML and return structured information.
 Author: Vladimir Iglovikov
 Author-email: iglovikov@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `html2info-0.1.2/README.md` & `html2info-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `html2info-0.1.2/html2info/linkedin.py` & `html2info-0.1.3/html2info/linkedin.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
         self.name = None
         self.title = None
         self.location = None
         self.profile_photo_link = None
         self.about = None
         self.experience = None
         self.education_list = None
+        self.about = None
 
     def parse(self):
         self.name = self.soup.find("h1").text.strip()
         self.title = self.soup.find("div", class_="text-body-medium").text.strip()
 
         self.location = self.soup.find("span", class_="text-body-small inline t-black--light break-words").text.strip()
 
@@ -34,14 +35,16 @@
         # Find the span containing the text
         # Find the parent container with specific class
         parent_container = self.soup.find(
             "div",
             class_="pv-shared-text-with-see-more full-width t-14 t-normal t-black display-flex align-items-center",
         )
 
+        if parent_container is None:
+            return
         # Find the span containing the text within the parent container
         text_span = parent_container.find("span", class_="visually-hidden")
 
         # Extract the text and remove extra spaces
         self.about = text_span.text.strip()
 
     def parse_experience(self):
```

### Comparing `html2info-0.1.2/html2info.egg-info/PKG-INFO` & `html2info-0.1.3/html2info.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html2info
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package to parse raw HTML and return structured information.
 Author: Vladimir Iglovikov
 Author-email: iglovikov@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `html2info-0.1.2/pyproject.toml` & `html2info-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `html2info-0.1.2/setup.py` & `html2info-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="html2info",  # Replace with your package name
-    version="0.1.2",  # Replace with your package version
+    version="0.1.3",  # Replace with your package version
     author="Vladimir Iglovikov",  # Replace with your name
     author_email="iglovikov@gmail.com",  # Replace with your email
     description="A package to parse raw HTML and return structured information.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(exclude=["tests"]),
     classifiers=[
```

