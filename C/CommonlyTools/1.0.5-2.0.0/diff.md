# Comparing `tmp/CommonlyTools-1.0.5.tar.gz` & `tmp/CommonlyTools-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CommonlyTools-1.0.5.tar", last modified: Sun Apr 23 04:56:28 2023, max compression
+gzip compressed data, was "CommonlyTools-2.0.0.tar", last modified: Sun Apr 23 06:41:52 2023, max compression
```

## Comparing `CommonlyTools-1.0.5.tar` & `CommonlyTools-2.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-23 04:56:28.629826 CommonlyTools-1.0.5/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-23 04:56:28.629826 CommonlyTools-1.0.5/CommonlyTools.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1650 2023-04-23 04:56:28.000000 CommonlyTools-1.0.5/CommonlyTools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      278 2023-04-23 04:56:28.000000 CommonlyTools-1.0.5/CommonlyTools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-23 04:56:28.000000 CommonlyTools-1.0.5/CommonlyTools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       18 2023-04-23 04:56:28.000000 CommonlyTools-1.0.5/CommonlyTools.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       14 2023-04-23 04:56:28.000000 CommonlyTools-1.0.5/CommonlyTools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     1062 2023-04-23 04:55:31.000000 CommonlyTools-1.0.5/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)     1650 2023-04-23 04:56:28.629826 CommonlyTools-1.0.5/PKG-INFO
--rw-------   0 runner    (1000) runner    (1000)      910 2023-04-23 04:55:35.000000 CommonlyTools-1.0.5/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-23 04:56:28.629826 CommonlyTools-1.0.5/commonlytools/
--rw-------   0 runner    (1000) runner    (1000)       24 2023-04-23 04:55:26.000000 CommonlyTools-1.0.5/commonlytools/__init__.py
--rw-------   0 runner    (1000) runner    (1000)     2313 2023-04-23 04:55:26.000000 CommonlyTools-1.0.5/commonlytools/discohook.py
--rw-r--r--   0 runner    (1000) runner    (1000)      312 2023-04-23 02:53:39.000000 CommonlyTools-1.0.5/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-04-23 04:56:28.629826 CommonlyTools-1.0.5/setup.cfg
--rw-------   0 runner    (1000) runner    (1000)      740 2023-04-23 04:56:16.000000 CommonlyTools-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-23 06:41:52.390236 CommonlyTools-2.0.0/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-23 06:41:52.390236 CommonlyTools-2.0.0/CommonlyTools.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1650 2023-04-23 06:41:52.000000 CommonlyTools-2.0.0/CommonlyTools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      278 2023-04-23 06:41:52.000000 CommonlyTools-2.0.0/CommonlyTools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-23 06:41:52.000000 CommonlyTools-2.0.0/CommonlyTools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       18 2023-04-23 06:41:52.000000 CommonlyTools-2.0.0/CommonlyTools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       14 2023-04-23 06:41:52.000000 CommonlyTools-2.0.0/CommonlyTools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     1062 2023-04-23 04:55:31.000000 CommonlyTools-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)     1650 2023-04-23 06:41:52.390236 CommonlyTools-2.0.0/PKG-INFO
+-rw-------   0 runner    (1000) runner    (1000)      910 2023-04-23 06:38:57.000000 CommonlyTools-2.0.0/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-23 06:41:52.390236 CommonlyTools-2.0.0/commonlytools/
+-rw-------   0 runner    (1000) runner    (1000)       24 2023-04-23 04:55:26.000000 CommonlyTools-2.0.0/commonlytools/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)     2313 2023-04-23 04:55:26.000000 CommonlyTools-2.0.0/commonlytools/discohook.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      312 2023-04-23 02:53:39.000000 CommonlyTools-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-04-23 06:41:52.394236 CommonlyTools-2.0.0/setup.cfg
+-rw-------   0 runner    (1000) runner    (1000)      740 2023-04-23 06:40:28.000000 CommonlyTools-2.0.0/setup.py
```

### Comparing `CommonlyTools-1.0.5/CommonlyTools.egg-info/PKG-INFO` & `CommonlyTools-2.0.0/CommonlyTools.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: CommonlyTools
-Version: 1.0.5
+Version: 2.0.0
 Summary: You will use Python easily!
 Home-page: https://github.com/maxgamil110331/CommonlyTools
 Author: MaxPython110331
 Author-email: dengxiangcheng110331@gmail.com
 License: MIT
 Description: # CommonlyTools
         
         ----------
         
         How to use CommonlyTools?
         >```pip install CommonlyTools```
         ----------
         
-        >CommonlyTools/discohook.py
+        >commonlytools/discohook.py
         >>Discord Webhook Sender
         >>>Step 1(If you do not need to use embed, you can skip this step.)
         >>>```py
-        >>>from CommonlyTools import discohook
+        >>>from commonlytools import discohook
         >>>
         >>>embed=discohook.Embed(color=dc.Colour(...), title="...", description="...") #If you need, you can enter the colour, title or descriotion
         >>>embed.author(name="...", url="...", icon_url="...") #author
         >>>embed.footer(text="...", icon_url="...") #footer
         >>>embed.image(image_url="...") #image
         >>>embed.thumbnail(thumbnail_url="...") #thumbnail
         >>>embed.add_field(name="...", value="...", inline=...) #add_field #This function can unlimited superposition.
```

### Comparing `CommonlyTools-1.0.5/LICENSE` & `CommonlyTools-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `CommonlyTools-1.0.5/PKG-INFO` & `CommonlyTools-2.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: CommonlyTools
-Version: 1.0.5
+Version: 2.0.0
 Summary: You will use Python easily!
 Home-page: https://github.com/maxgamil110331/CommonlyTools
 Author: MaxPython110331
 Author-email: dengxiangcheng110331@gmail.com
 License: MIT
 Description: # CommonlyTools
         
         ----------
         
         How to use CommonlyTools?
         >```pip install CommonlyTools```
         ----------
         
-        >CommonlyTools/discohook.py
+        >commonlytools/discohook.py
         >>Discord Webhook Sender
         >>>Step 1(If you do not need to use embed, you can skip this step.)
         >>>```py
-        >>>from CommonlyTools import discohook
+        >>>from commonlytools import discohook
         >>>
         >>>embed=discohook.Embed(color=dc.Colour(...), title="...", description="...") #If you need, you can enter the colour, title or descriotion
         >>>embed.author(name="...", url="...", icon_url="...") #author
         >>>embed.footer(text="...", icon_url="...") #footer
         >>>embed.image(image_url="...") #image
         >>>embed.thumbnail(thumbnail_url="...") #thumbnail
         >>>embed.add_field(name="...", value="...", inline=...) #add_field #This function can unlimited superposition.
```

### Comparing `CommonlyTools-1.0.5/README.md` & `CommonlyTools-2.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 ----------
 
 How to use CommonlyTools?
 >```pip install CommonlyTools```
 ----------
 
->CommonlyTools/discohook.py
+>commonlytools/discohook.py
 >>Discord Webhook Sender
 >>>Step 1(If you do not need to use embed, you can skip this step.)
 >>>```py
->>>from CommonlyTools import discohook
+>>>from commonlytools import discohook
 >>>
 >>>embed=discohook.Embed(color=dc.Colour(...), title="...", description="...") #If you need, you can enter the colour, title or descriotion
 >>>embed.author(name="...", url="...", icon_url="...") #author
 >>>embed.footer(text="...", icon_url="...") #footer
 >>>embed.image(image_url="...") #image
 >>>embed.thumbnail(thumbnail_url="...") #thumbnail
 >>>embed.add_field(name="...", value="...", inline=...) #add_field #This function can unlimited superposition.
```

### Comparing `CommonlyTools-1.0.5/commonlytools/discohook.py` & `CommonlyTools-2.0.0/commonlytools/discohook.py`

 * *Files identical despite different names*

### Comparing `CommonlyTools-1.0.5/setup.py` & `CommonlyTools-2.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="CommonlyTools",
-    version="1.0.5",
+    version="2.0.0",
     author="MaxPython110331",
     author_email="dengxiangcheng110331@gmail.com",
     description="You will use Python easily!",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://github.com/maxgamil110331/CommonlyTools",
```

