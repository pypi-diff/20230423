# Comparing `tmp/p-template-res-0.1.8.tar.gz` & `tmp/p-template-res-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p-template-res-0.1.8.tar", last modified: Wed Mar 22 08:44:42 2023, max compression
+gzip compressed data, was "p-template-res-0.1.9.tar", last modified: Wed Mar 22 09:07:15 2023, max compression
```

## Comparing `p-template-res-0.1.8.tar` & `p-template-res-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-03-22 08:44:42.109671 p-template-res-0.1.8/
--rw-rw-rw-   0        0        0     1074 2023-02-27 11:23:20.000000 p-template-res-0.1.8/LICENSE
--rw-rw-rw-   0        0        0      396 2023-03-22 08:44:42.109671 p-template-res-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0       17 2023-03-14 06:24:40.000000 p-template-res-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-03-22 08:44:42.105669 p-template-res-0.1.8/p_template_res.egg-info/
--rw-rw-rw-   0        0        0      396 2023-03-22 08:44:42.000000 p-template-res-0.1.8/p_template_res.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      356 2023-03-22 08:44:42.000000 p-template-res-0.1.8/p_template_res.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-22 08:44:42.000000 p-template-res-0.1.8/p_template_res.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-03-22 08:44:42.000000 p-template-res-0.1.8/p_template_res.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-03-22 08:44:42.000000 p-template-res-0.1.8/p_template_res.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-03-22 08:44:42.000000 p-template-res-0.1.8/p_template_res.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-22 08:44:42.110669 p-template-res-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      817 2023-03-22 08:44:11.000000 p-template-res-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-22 08:44:42.107669 p-template-res-0.1.8/template_res/
--rw-rw-rw-   0        0        0        0 2023-03-22 02:42:04.000000 p-template-res-0.1.8/template_res/__init__.py
--rw-rw-rw-   0        0        0      682 2023-03-21 10:00:39.000000 p-template-res-0.1.8/template_res/main.py
-drwxrwxrwx   0        0        0        0 2023-03-22 08:44:42.108668 p-template-res-0.1.8/template_res/res/
--rw-rw-rw-   0        0        0        0 2023-03-22 02:42:04.000000 p-template-res-0.1.8/template_res/res/__init__.py
--rw-rw-rw-   0        0        0     5333 2023-03-22 08:42:53.000000 p-template-res-0.1.8/template_res/template.py
+drwxrwxrwx   0        0        0        0 2023-03-22 09:07:15.383379 p-template-res-0.1.9/
+-rw-rw-rw-   0        0        0     1074 2023-02-27 11:23:20.000000 p-template-res-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0      396 2023-03-22 09:07:15.382380 p-template-res-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0       17 2023-03-14 06:24:40.000000 p-template-res-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-03-22 09:07:15.377381 p-template-res-0.1.9/p_template_res.egg-info/
+-rw-rw-rw-   0        0        0      396 2023-03-22 09:07:15.000000 p-template-res-0.1.9/p_template_res.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      356 2023-03-22 09:07:15.000000 p-template-res-0.1.9/p_template_res.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-22 09:07:15.000000 p-template-res-0.1.9/p_template_res.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-03-22 09:07:15.000000 p-template-res-0.1.9/p_template_res.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-03-22 09:07:15.000000 p-template-res-0.1.9/p_template_res.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-03-22 09:07:15.000000 p-template-res-0.1.9/p_template_res.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-03-22 09:07:15.383379 p-template-res-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      817 2023-03-22 09:07:10.000000 p-template-res-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-22 09:07:15.380380 p-template-res-0.1.9/template_res/
+-rw-rw-rw-   0        0        0        0 2023-03-22 02:42:04.000000 p-template-res-0.1.9/template_res/__init__.py
+-rw-rw-rw-   0        0        0      682 2023-03-21 10:00:39.000000 p-template-res-0.1.9/template_res/main.py
+drwxrwxrwx   0        0        0        0 2023-03-22 09:07:15.381380 p-template-res-0.1.9/template_res/res/
+-rw-rw-rw-   0        0        0        0 2023-03-22 02:42:04.000000 p-template-res-0.1.9/template_res/res/__init__.py
+-rw-rw-rw-   0        0        0     5341 2023-03-22 09:07:00.000000 p-template-res-0.1.9/template_res/template.py
```

### Comparing `p-template-res-0.1.8/LICENSE` & `p-template-res-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `p-template-res-0.1.8/setup.py` & `p-template-res-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="p-template-res",
-    version="0.1.8",
+    version="0.1.9",
     author="pengjun",
     author_email="mr_lonely@foxmail.com",
     description="temple tools",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `p-template-res-0.1.8/template_res/main.py` & `p-template-res-0.1.9/template_res/main.py`

 * *Files identical despite different names*

### Comparing `p-template-res-0.1.8/template_res/template.py` & `p-template-res-0.1.9/template_res/template.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,17 +24,17 @@
             os.remove(localFile)
         s = requests.session()
         s.keep_alive = False
         file = s.get(url, verify=False)
         with open(localFile, "wb") as c:
             c.write(file.content)
         s.close()
-
+        
 def updateNewTempalte(rootDir):
-    getOssResource(rootDir, "http://mecord-m.2tianxin.com/res/template_res_2023032216.zip", "abe8ace85a5aecdce1944a9bdbdfbc1f", "template_res.zip.py")
+    getOssResource(rootDir, "http://mecord-m.2tianxin.com/res/template_res_2023032217.zip", "5a128d3b8810bda7d7df2ae2bc2532f4", "template_res.zip.py")
     for root,dirs,files in os.walk(rootDir):
         for dir in dirs:
             shutil.rmtree(os.path.join(root, dir))
 
     for root,dirs,files in os.walk(rootDir):
         for file in files:
             name = file[0:file.index(".")]
```

