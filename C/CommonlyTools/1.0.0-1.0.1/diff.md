# Comparing `tmp/CommonlyTools-1.0.0.tar.gz` & `tmp/CommonlyTools-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CommonlyTools-1.0.0.tar", last modified: Sun Apr 23 02:22:43 2023, max compression
+gzip compressed data, was "CommonlyTools-1.0.1.tar", last modified: Sun Apr 23 02:28:53 2023, max compression
```

## Comparing `CommonlyTools-1.0.0.tar` & `CommonlyTools-1.0.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-23 02:22:43.530530 CommonlyTools-1.0.0/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-23 02:22:43.526530 CommonlyTools-1.0.0/CommonlyTools.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1601 2023-04-23 02:22:43.000000 CommonlyTools-1.0.0/CommonlyTools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      183 2023-04-23 02:22:43.000000 CommonlyTools-1.0.0/CommonlyTools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-23 02:22:43.000000 CommonlyTools-1.0.0/CommonlyTools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       18 2023-04-23 02:22:43.000000 CommonlyTools-1.0.0/CommonlyTools.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-23 02:22:43.000000 CommonlyTools-1.0.0/CommonlyTools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     1601 2023-04-23 02:22:43.526530 CommonlyTools-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-04-23 02:22:43.530530 CommonlyTools-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-23 02:28:53.397718 CommonlyTools-1.0.1/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-23 02:28:53.397718 CommonlyTools-1.0.1/CommonlyTools.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1626 2023-04-23 02:28:53.000000 CommonlyTools-1.0.1/CommonlyTools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      183 2023-04-23 02:28:53.000000 CommonlyTools-1.0.1/CommonlyTools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-23 02:28:53.000000 CommonlyTools-1.0.1/CommonlyTools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       18 2023-04-23 02:28:53.000000 CommonlyTools-1.0.1/CommonlyTools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-23 02:28:53.000000 CommonlyTools-1.0.1/CommonlyTools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     1626 2023-04-23 02:28:53.397718 CommonlyTools-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-04-23 02:28:53.397718 CommonlyTools-1.0.1/setup.cfg
```

### Comparing `CommonlyTools-1.0.0/CommonlyTools.egg-info/PKG-INFO` & `CommonlyTools-1.0.1/CommonlyTools.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: CommonlyTools
-Version: 1.0.0
+Version: 1.0.1
 Summary: You will use Python easily!
 Home-page: https://github.com/maxgamil110331/CommonlyTools
 Author: MaxPython110331
 Author-email: dengxiangcheng110331@gmail.com
 License: MIT
-Description: # Easy-Python
+Description: # CommonlyTools
         
         ----------
         
-        How to use Easy-Python?
-        >```pip install EasyPY```
+        How to use CommonlyTools?
+        >```pip install CommonlyTools```
         ----------
         
-        >easypy/discohook.py
+        >CommonlyTools/discohook.py
         >>Discord Webhook Sender
         >>>Step 1(If you do not need to use embed, you can skip this step.)
         >>>```py
-        >>>from easypy import discohook
+        >>>from CommonlyTools import discohook
         >>>
         >>>embed=discohook.Embed(color=dc.Colour(...), title="...", description="...") #If you need, you can enter the colour, title or descriotion
         >>>embed.author(name="...", url="...", icon_url="...") #author
         >>>embed.footer(text="...", icon_url="...") #footer
         >>>embed.image(image_url="...") #image
         >>>embed.thumbnail(thumbnail_url="...") #thumbnail
         >>>embed.add_field(name="...", value="...", inline=...) #add_field #This function can unlimited superposition.
```

### Comparing `CommonlyTools-1.0.0/PKG-INFO` & `CommonlyTools-1.0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: CommonlyTools
-Version: 1.0.0
+Version: 1.0.1
 Summary: You will use Python easily!
 Home-page: https://github.com/maxgamil110331/CommonlyTools
 Author: MaxPython110331
 Author-email: dengxiangcheng110331@gmail.com
 License: MIT
-Description: # Easy-Python
+Description: # CommonlyTools
         
         ----------
         
-        How to use Easy-Python?
-        >```pip install EasyPY```
+        How to use CommonlyTools?
+        >```pip install CommonlyTools```
         ----------
         
-        >easypy/discohook.py
+        >CommonlyTools/discohook.py
         >>Discord Webhook Sender
         >>>Step 1(If you do not need to use embed, you can skip this step.)
         >>>```py
-        >>>from easypy import discohook
+        >>>from CommonlyTools import discohook
         >>>
         >>>embed=discohook.Embed(color=dc.Colour(...), title="...", description="...") #If you need, you can enter the colour, title or descriotion
         >>>embed.author(name="...", url="...", icon_url="...") #author
         >>>embed.footer(text="...", icon_url="...") #footer
         >>>embed.image(image_url="...") #image
         >>>embed.thumbnail(thumbnail_url="...") #thumbnail
         >>>embed.add_field(name="...", value="...", inline=...) #add_field #This function can unlimited superposition.
```

