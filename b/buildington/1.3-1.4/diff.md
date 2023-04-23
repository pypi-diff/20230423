# Comparing `tmp/buildington-1.3.tar.gz` & `tmp/buildington-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildington-1.3.tar", last modified: Sat Apr 22 13:22:55 2023, max compression
+gzip compressed data, was "buildington-1.4.tar", last modified: Sun Apr 23 09:06:39 2023, max compression
```

## Comparing `buildington-1.3.tar` & `buildington-1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 13:22:55.245676 buildington-1.3/
--rw-rw-rw-   0        0        0      482 2023-04-22 13:22:55.245676 buildington-1.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-22 13:22:55.198811 buildington-1.3/buildington/
--rw-rw-rw-   0        0        0     3573 2023-04-22 13:22:36.000000 buildington-1.3/buildington/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-22 13:22:55.245676 buildington-1.3/buildington.egg-info/
--rw-rw-rw-   0        0        0      482 2023-04-22 13:22:54.000000 buildington-1.3/buildington.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      206 2023-04-22 13:22:55.000000 buildington-1.3/buildington.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 13:22:54.000000 buildington-1.3/buildington.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-22 13:22:54.000000 buildington-1.3/buildington.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-22 13:22:54.000000 buildington-1.3/buildington.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-22 13:22:55.245676 buildington-1.3/setup.cfg
--rw-rw-rw-   0        0        0      556 2023-04-22 13:22:50.000000 buildington-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 09:06:39.918872 buildington-1.4/
+-rw-rw-rw-   0        0        0      482 2023-04-23 09:06:39.915873 buildington-1.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-23 09:06:39.854870 buildington-1.4/buildington/
+-rw-rw-rw-   0        0        0     3594 2023-04-23 09:05:44.000000 buildington-1.4/buildington/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 09:06:39.910871 buildington-1.4/buildington.egg-info/
+-rw-rw-rw-   0        0        0      482 2023-04-23 09:06:39.000000 buildington-1.4/buildington.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      206 2023-04-23 09:06:39.000000 buildington-1.4/buildington.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 09:06:39.000000 buildington-1.4/buildington.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-23 09:06:39.000000 buildington-1.4/buildington.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-23 09:06:39.000000 buildington-1.4/buildington.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 09:06:39.918872 buildington-1.4/setup.cfg
+-rw-rw-rw-   0        0        0      556 2023-04-23 09:06:22.000000 buildington-1.4/setup.py
```

### Comparing `buildington-1.3/buildington/__init__.py` & `buildington-1.4/buildington/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,16 @@
 		return wrap
 	return decor
 
 def addFile(file):
 	PAGES = list(globals()["PAGES"])
 	def returnResp():
 		import flask
-		return flask.send_from_directory(".", file)
+		import os
+		return flask.send_from_directory(os.getcwd(), file)
 	PAGES.append(("/" + file, returnResp, {"met": GETONLY}))
 	globals()["PAGES"] = tuple(PAGES)
 	del locals()["PAGES"]
 
 def start(host, port):
 	import flask, threading
 	app = flask.Flask(__name__) # The module name will fit :)
@@ -79,15 +80,15 @@
 		count = 0
 		while count != len(globals()["PAGES"]):
 			endpnt = globals()["PAGES"][count]
 			if endpnt[0] == path:
 				foundEndpnt = True
 				break
 			count += 1
-		if not foundEndpnt:
+		if foundEndpnt == False:
 			return flask.abort(404) # Page not found!!1
 		endpntMets = []
 		count = 0
 		for met in endpnt[2]["met"]:
 			endpntMets.append("GET" if met == GETMET else ("POST" if met == POSTMET else None))
 			count += 1
 		if flask.request.method.upper() not in endpntMets:
@@ -96,15 +97,15 @@
 		bdRes = endpnt[1]()
 		def escapeHTML(txt):
 			res = ""
 			for char in txt:
 				res += "&#" + str(ord(char)) + ";"
 			return res
 		count = 0
-		if isinstance(bdRes, flask.Response):
+		if not isinstance(bdRes, tuple):
 			return bdRes
 		bdRes = list(bdRes)
 		for elem in bdRes:
 			if isinstance(elem, str):
 				elem = escapeHTML(elem)
 			elem = str(elem)
 			bdRes[count] = elem
```

### Comparing `buildington-1.3/setup.py` & `buildington-1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
 	name="buildington",
-	version="1.3",
+	version="1.4",
 	author="RixTheTyrunt",
 	author_email="rixthetyrunt@gmail.com",
 	description="Building websites like React, and hosting 'em like Flask!",
 	packages=["buildington"],
 	classifiers=[
 		"Environment :: Console",
 		"Framework :: Flask",
```

