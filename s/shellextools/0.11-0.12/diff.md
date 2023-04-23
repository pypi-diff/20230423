# Comparing `tmp/shellextools-0.11.tar.gz` & `tmp/shellextools-0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shellextools-0.11.tar", last modified: Sun Apr 23 15:56:17 2023, max compression
+gzip compressed data, was "shellextools-0.12.tar", last modified: Sun Apr 23 17:54:16 2023, max compression
```

## Comparing `shellextools-0.11.tar` & `shellextools-0.12.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 15:56:17.208249 shellextools-0.11/
--rw-rw-rw-   0        0        0     1148 2023-04-23 15:56:03.000000 shellextools-0.11/LICENSE.rst
--rw-rw-rw-   0        0        0      209 2023-04-23 15:56:03.000000 shellextools-0.11/MANIFEST.in
--rw-rw-rw-   0        0        0     3573 2023-04-23 15:56:17.208249 shellextools-0.11/PKG-INFO
--rw-rw-rw-   0        0        0     2923 2023-04-22 12:39:53.000000 shellextools-0.11/README.md
--rw-rw-rw-   0        0        0       85 2023-04-23 15:56:17.209247 shellextools-0.11/setup.cfg
--rw-rw-rw-   0        0        0     1861 2023-04-23 15:56:16.000000 shellextools-0.11/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-23 15:56:17.203235 shellextools-0.11/shellextools/
--rw-rw-rw-   0        0        0     1148 2023-04-15 00:23:59.000000 shellextools-0.11/shellextools/LICENSE
--rw-rw-rw-   0        0        0     2923 2023-04-22 12:39:53.000000 shellextools-0.11/shellextools/README.md
--rw-rw-rw-   0        0        0    47690 2023-04-23 15:38:04.000000 shellextools-0.11/shellextools/__init__.py
--rw-rw-rw-   0        0        0     2728 2023-04-23 15:51:51.000000 shellextools-0.11/shellextools/getmultifiles.py
--rw-rw-rw-   0        0        0     2555 2023-04-23 15:50:28.000000 shellextools-0.11/shellextools/loggax3.py
--rw-rw-rw-   0        0        0      248 2023-04-23 15:56:16.000000 shellextools-0.11/shellextools/requirements.txt
--rw-rw-rw-   0        0        0     9983 2023-04-23 15:56:16.000000 shellextools-0.11/shellextools/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-04-23 15:56:17.207252 shellextools-0.11/shellextools.egg-info/
--rw-rw-rw-   0        0        0     3573 2023-04-23 15:56:16.000000 shellextools-0.11/shellextools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      413 2023-04-23 15:56:17.000000 shellextools-0.11/shellextools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 15:56:16.000000 shellextools-0.11/shellextools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      236 2023-04-23 15:56:16.000000 shellextools-0.11/shellextools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-23 15:56:16.000000 shellextools-0.11/shellextools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 17:54:16.958320 shellextools-0.12/
+-rw-rw-rw-   0        0        0     1148 2023-04-23 17:53:54.000000 shellextools-0.12/LICENSE.rst
+-rw-rw-rw-   0        0        0      209 2023-04-23 17:53:50.000000 shellextools-0.12/MANIFEST.in
+-rw-rw-rw-   0        0        0     3573 2023-04-23 17:54:16.958320 shellextools-0.12/PKG-INFO
+-rw-rw-rw-   0        0        0     2923 2023-04-23 15:59:07.000000 shellextools-0.12/README.md
+-rw-rw-rw-   0        0        0       85 2023-04-23 17:54:16.959317 shellextools-0.12/setup.cfg
+-rw-rw-rw-   0        0        0     1861 2023-04-23 17:54:16.000000 shellextools-0.12/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 17:54:16.954330 shellextools-0.12/shellextools/
+-rw-rw-rw-   0        0        0     1148 2023-04-15 00:23:59.000000 shellextools-0.12/shellextools/LICENSE
+-rw-rw-rw-   0        0        0     2923 2023-04-23 15:59:07.000000 shellextools-0.12/shellextools/README.md
+-rw-rw-rw-   0        0        0    48251 2023-04-23 17:14:00.000000 shellextools-0.12/shellextools/__init__.py
+-rw-rw-rw-   0        0        0     2728 2023-04-23 15:59:07.000000 shellextools-0.12/shellextools/getmultifiles.py
+-rw-rw-rw-   0        0        0     2555 2023-04-23 15:59:07.000000 shellextools-0.12/shellextools/loggax3.py
+-rw-rw-rw-   0        0        0      248 2023-04-23 17:54:16.000000 shellextools-0.12/shellextools/requirements.txt
+-rw-rw-rw-   0        0        0     9983 2023-04-23 17:54:16.000000 shellextools-0.12/shellextools/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-04-23 17:54:16.957322 shellextools-0.12/shellextools.egg-info/
+-rw-rw-rw-   0        0        0     3573 2023-04-23 17:54:16.000000 shellextools-0.12/shellextools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2023-04-23 17:54:16.000000 shellextools-0.12/shellextools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 17:54:16.000000 shellextools-0.12/shellextools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      236 2023-04-23 17:54:16.000000 shellextools-0.12/shellextools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-23 17:54:16.000000 shellextools-0.12/shellextools.egg-info/top_level.txt
```

### Comparing `shellextools-0.11/LICENSE.rst` & `shellextools-0.12/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `shellextools-0.11/PKG-INFO` & `shellextools-0.12/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shellextools
-Version: 0.11
+Version: 0.12
 Summary: Adds Python functions/methods to the Windows context menu
 Home-page: https://github.com/hansalemaos/shellextools
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: Windows context menu,python,nutika
 Classifier: Development Status :: 4 - Beta
```

### Comparing `shellextools-0.11/README.md` & `shellextools-0.12/README.md`

 * *Files identical despite different names*

### Comparing `shellextools-0.11/setup.py` & `shellextools-0.12/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
 #     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.11'''
+VERSION = '''0.12'''
 DESCRIPTION = '''Adds Python functions/methods to the Windows context menu'''
 
 # Setting up
 setup(
     name="shellextools",
     version=VERSION,
     license='MIT',
```

### Comparing `shellextools-0.11/shellextools/LICENSE` & `shellextools-0.12/shellextools/LICENSE`

 * *Files identical despite different names*

### Comparing `shellextools-0.11/shellextools/README.md` & `shellextools-0.12/shellextools/README.md`

 * *Files identical despite different names*

### Comparing `shellextools-0.11/shellextools/__init__.py` & `shellextools-0.12/shellextools/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,14 +114,29 @@
     "\x1c",
     "\x1d",
     "\x1e",
     "\x1f",
 )
 
 
+def get_my_icon(iconfile="iconapp.ico"):
+    icon = os.path.dirname(sys.argv[0])
+    icon = os.path.normpath(os.path.join(icon,iconfile))
+    if os.path.exists(icon):
+        return icon
+    icon = os.path.dirname(__file__)
+    icon = os.path.normpath(os.path.join(icon,iconfile))
+    if os.path.exists(icon):
+        return icon
+    icon = os.sep.join(os.path.dirname(__file__).split(os.sep)[:-1])
+    icon = os.path.normpath(os.path.join(icon,iconfile))
+    if os.path.exists(icon):
+        return icon
+    return None
+
 class FlexiblePartialOwnName:
     r"""
     FlexiblePartial(
             remove_file,
             "()",
             True,
             fullpath_on_device=x.aa_fullpath,
@@ -1308,15 +1323,15 @@
         cm,
         shell=True,
     )
     if loopnumber == 0:
         shutil.copy(myfile, newpath)
     uninstalldata = f"\ndel {newpathescaped}\ndel {newpathuninstall}\n"
     if loopnumber == 0:
-        writemode = "w"
+        writemode = "a"
     else:
         writemode = "a"
     with open(newpathuninstall, mode=writemode, encoding="utf-8") as f:
         f.write('\n')
         f.write(
             rf"""%systemroot%\system32\Reg.exe delete "HKCR\{Drive_or_Directory}\shell\{mainmenuitem}\shell" /f"""
         )
@@ -1425,32 +1440,32 @@
         rf"""%systemroot%\system32\Reg.exe delete "HKCR\SystemFileAssociations\.FTYPE\shell\{mainmenuitem}" /f""",
 
 
     ]
     uninstalldatalist = []
     for fi in filetypes:
         for c in commandsrawdelete:
-            command2add = c.replace(rf"\.FTYPE{os.sep}", rf"\.{fi}{os.sep}")
+            command2add = c.replace(rf"\.FTYPE{os.sep}", rf"\.{fi.strip('. ')}{os.sep}")
             uninstalldatalist.append(command2add)
 
     commands = []
     for fi in filetypes:
         for c in commandsraw:
-            command2add = c.replace(rf"\.FTYPE{os.sep}", rf"\.{fi}{os.sep}")
+            command2add = c.replace(rf"\.FTYPE{os.sep}", rf"\.{fi.strip('. ')}{os.sep}")
             commands.append(command2add)
 
     for c in commands:
         subprocess.run(c, shell=True)
 
     shutil.copy(myfile, newpath)
     fileswritten.append(newpath)
     uninstalldata = "\n".join(uninstalldatalist)
     finaldelete = f"\ndel {newpathescaped}\ndel {newpathuninstall}\n"
     if loopnumber == 0:
-        writemode = "w"
+        writemode = "a"
     else:
         writemode = "a"
     with open(newpathuninstall, mode=writemode, encoding="utf-8") as f:
         f.write(uninstalldata)
     fileswritten.append(newpathuninstall)
     #show_after_install(silentinstall, newpath, newpathuninstall)
```

### Comparing `shellextools-0.11/shellextools/getmultifiles.py` & `shellextools-0.12/shellextools/getmultifiles.py`

 * *Files identical despite different names*

### Comparing `shellextools-0.11/shellextools/loggax3.py` & `shellextools-0.12/shellextools/loggax3.py`

 * *Files identical despite different names*

### Comparing `shellextools-0.11/shellextools/thirdparty.json` & `shellextools-0.12/shellextools/thirdparty.json`

 * *Files identical despite different names*

### Comparing `shellextools-0.11/shellextools.egg-info/PKG-INFO` & `shellextools-0.12/shellextools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shellextools
-Version: 0.11
+Version: 0.12
 Summary: Adds Python functions/methods to the Windows context menu
 Home-page: https://github.com/hansalemaos/shellextools
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: Windows context menu,python,nutika
 Classifier: Development Status :: 4 - Beta
```

