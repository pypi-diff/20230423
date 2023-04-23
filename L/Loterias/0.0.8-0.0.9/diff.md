# Comparing `tmp/Loterias-0.0.8.tar.gz` & `tmp/Loterias-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Loterias-0.0.8.tar", last modified: Sun Apr 23 00:36:03 2023, max compression
+gzip compressed data, was "Loterias-0.0.9.tar", last modified: Sun Apr 23 00:50:06 2023, max compression
```

## Comparing `Loterias-0.0.8.tar` & `Loterias-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 00:36:03.802862 Loterias-0.0.8/
--rw-rw-rw-   0        0        0     1097 2023-04-20 11:21:01.000000 Loterias-0.0.8/LICENCE
-drwxrwxrwx   0        0        0        0 2023-04-23 00:36:03.787230 Loterias-0.0.8/Loterias/
--rw-rw-rw-   0        0        0     2137 2023-04-18 11:46:15.000000 Loterias-0.0.8/Loterias/Apurar.py
--rw-rw-rw-   0        0        0     8679 2023-04-23 00:34:32.000000 Loterias-0.0.8/Loterias/Collection.py
--rw-rw-rw-   0        0        0     5178 2023-04-18 11:45:08.000000 Loterias-0.0.8/Loterias/Collections.py
--rw-rw-rw-   0        0        0     3331 2023-04-18 11:45:08.000000 Loterias-0.0.8/Loterias/Interpoler.py
--rw-rw-rw-   0        0        0    10489 2023-04-19 10:36:19.000000 Loterias-0.0.8/Loterias/Loto.py
--rw-rw-rw-   0        0        0      916 2023-04-18 11:45:08.000000 Loterias-0.0.8/Loterias/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 00:36:03.787230 Loterias-0.0.8/Loterias.egg-info/
--rw-rw-rw-   0        0        0     1870 2023-04-23 00:36:03.000000 Loterias-0.0.8/Loterias.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-04-23 00:36:03.000000 Loterias-0.0.8/Loterias.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 00:36:03.000000 Loterias-0.0.8/Loterias.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-04-23 00:36:03.000000 Loterias-0.0.8/Loterias.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-23 00:36:03.000000 Loterias-0.0.8/Loterias.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1870 2023-04-23 00:36:03.787230 Loterias-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1485 2023-04-22 23:11:47.000000 Loterias-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-04-23 00:36:03.802862 Loterias-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      514 2023-04-23 00:34:32.000000 Loterias-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 00:50:06.899286 Loterias-0.0.9/
+-rw-rw-rw-   0        0        0     1097 2023-04-20 11:21:01.000000 Loterias-0.0.9/LICENCE
+drwxrwxrwx   0        0        0        0 2023-04-23 00:50:06.883666 Loterias-0.0.9/Loterias/
+-rw-rw-rw-   0        0        0     2137 2023-04-18 11:46:15.000000 Loterias-0.0.9/Loterias/Apurar.py
+-rw-rw-rw-   0        0        0     9063 2023-04-23 00:50:00.000000 Loterias-0.0.9/Loterias/Collection.py
+-rw-rw-rw-   0        0        0     5178 2023-04-18 11:45:08.000000 Loterias-0.0.9/Loterias/Collections.py
+-rw-rw-rw-   0        0        0     3331 2023-04-18 11:45:08.000000 Loterias-0.0.9/Loterias/Interpoler.py
+-rw-rw-rw-   0        0        0    10489 2023-04-19 10:36:19.000000 Loterias-0.0.9/Loterias/Loto.py
+-rw-rw-rw-   0        0        0      916 2023-04-18 11:45:08.000000 Loterias-0.0.9/Loterias/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 00:50:06.899286 Loterias-0.0.9/Loterias.egg-info/
+-rw-rw-rw-   0        0        0     1870 2023-04-23 00:50:06.000000 Loterias-0.0.9/Loterias.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-04-23 00:50:06.000000 Loterias-0.0.9/Loterias.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 00:50:06.000000 Loterias-0.0.9/Loterias.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-04-23 00:50:06.000000 Loterias-0.0.9/Loterias.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-23 00:50:06.000000 Loterias-0.0.9/Loterias.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1870 2023-04-23 00:50:06.899286 Loterias-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1485 2023-04-22 23:11:47.000000 Loterias-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-23 00:50:06.899286 Loterias-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      514 2023-04-23 00:50:00.000000 Loterias-0.0.9/setup.py
```

### Comparing `Loterias-0.0.8/LICENCE` & `Loterias-0.0.9/LICENCE`

 * *Files identical despite different names*

### Comparing `Loterias-0.0.8/Loterias/Apurar.py` & `Loterias-0.0.9/Loterias/Apurar.py`

 * *Files identical despite different names*

### Comparing `Loterias-0.0.8/Loterias/Collection.py` & `Loterias-0.0.9/Loterias/Collection.py`

 * *Files 7% similar despite different names*

```diff
@@ -156,14 +156,24 @@
 
     @maxThreads.setter
     def maxThreads(self, v):
         if (self.__thMax != v) and (v > 1):
             self.__thMax = v
             self.__dumpThreads()
 
+
+    @property
+    def showSetup(self):
+        print('Jogo             ', self.__lb().jogo)
+        print('Dezenas          ', self.__lb().volante.dezenas)
+        print('Sorteios         ', self.__lb().volante.sorteio)
+        print('Sorteio inicial  ', self.sorteioInicial)
+        print('Sorteio final    ', self.sorteioFinal)
+        print('Threads          ', self.maxThreads)
+
     def __dumpThreads(self):
 
         # Encerra todas as Threads anteriores, se houver
         for th in self.__th:
             th.stop = True
 
         # Reseta a lista de threads
```

### Comparing `Loterias-0.0.8/Loterias/Collections.py` & `Loterias-0.0.9/Loterias/Collections.py`

 * *Files identical despite different names*

### Comparing `Loterias-0.0.8/Loterias/Interpoler.py` & `Loterias-0.0.9/Loterias/Interpoler.py`

 * *Files identical despite different names*

### Comparing `Loterias-0.0.8/Loterias/Loto.py` & `Loterias-0.0.9/Loterias/Loto.py`

 * *Files identical despite different names*

### Comparing `Loterias-0.0.8/Loterias/__init__.py` & `Loterias-0.0.9/Loterias/__init__.py`

 * *Files identical despite different names*

### Comparing `Loterias-0.0.8/Loterias.egg-info/PKG-INFO` & `Loterias-0.0.9/Loterias.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Loterias
-Version: 0.0.8
+Version: 0.0.9
 Summary: Wrapper não oficial para pesquisa de dados lotéricos em thread
 Home-page: UNKNOWN
 Author: PKG
 Author-email: drjpp.drjpp@gmail.com
 License: MIT License
 Keywords: loterias CEF
 Platform: UNKNOWN
```

### Comparing `Loterias-0.0.8/PKG-INFO` & `Loterias-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Loterias
-Version: 0.0.8
+Version: 0.0.9
 Summary: Wrapper não oficial para pesquisa de dados lotéricos em thread
 Home-page: UNKNOWN
 Author: PKG
 Author-email: drjpp.drjpp@gmail.com
 License: MIT License
 Keywords: loterias CEF
 Platform: UNKNOWN
```

### Comparing `Loterias-0.0.8/README.md` & `Loterias-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `Loterias-0.0.8/setup.py` & `Loterias-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
 setup(name='Loterias',
-    version='0.0.8',
+    version='0.0.9',
     license='MIT License',
     author='PKG',
     long_description=readme,
     long_description_content_type="text/markdown",
     author_email='drjpp.drjpp@gmail.com',
     keywords='loterias CEF',
     description=u'Wrapper não oficial para pesquisa de dados lotéricos em thread',
```

