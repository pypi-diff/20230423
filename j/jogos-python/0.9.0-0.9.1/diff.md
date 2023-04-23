# Comparing `tmp/jogos_python-0.9.0.tar.gz` & `tmp/jogos_python-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jogos_python-0.9.0.tar", last modified: Thu Jan 20 14:57:42 2022, max compression
+gzip compressed data, was "jogos_python-0.9.1.tar", last modified: Thu Jan 20 15:19:59 2022, max compression
```

## Comparing `jogos_python-0.9.0.tar` & `jogos_python-0.9.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 victormoreira  (1000) victormoreira  (1000)        0 2022-01-20 14:57:42.609141 jogos_python-0.9.0/
--rw-r--r--   0 victormoreira  (1000) victormoreira  (1000)       26 2021-08-08 11:39:03.000000 jogos_python-0.9.0/MANIFEST.in
--rw-r--r--   0 victormoreira  (1000) victormoreira  (1000)     3346 2022-01-20 14:57:42.609141 jogos_python-0.9.0/PKG-INFO
--rw-r--r--   0 victormoreira  (1000) victormoreira  (1000)     2438 2021-07-24 07:54:45.000000 jogos_python-0.9.0/README.md
-drwxr-xr-x   0 victormoreira  (1000) victormoreira  (1000)        0 2022-01-20 14:57:42.605141 jogos_python-0.9.0/jogos_python/
--rw-r--r--   0 victormoreira  (1000) victormoreira  (1000)    23871 2022-01-20 14:51:47.000000 jogos_python-0.9.0/jogos_python/__init__.py
--rw-r--r--   0 victormoreira  (1000) victormoreira  (1000)    15413 2021-08-24 20:28:21.000000 jogos_python-0.9.0/jogos_python/caixa.png
--rw-r--r--   0 victormoreira  (1000) victormoreira  (1000)    14924 2021-08-05 13:46:39.000000 jogos_python-0.9.0/jogos_python/fazenda.png
--rw-r--r--   0 victormoreira  (1000) victormoreira  (1000)    14810 2021-08-05 13:46:39.000000 jogos_python-0.9.0/jogos_python/galinha.png
--rw-r--r--   0 victormoreira  (1000) victormoreira  (1000)     1009 2021-08-05 13:46:39.000000 jogos_python-0.9.0/jogos_python/ovo.png
--rw-r--r--   0 victormoreira  (1000) victormoreira  (1000)    12686 2021-08-05 13:46:39.000000 jogos_python-0.9.0/jogos_python/pintinho.png
-drwxr-xr-x   0 victormoreira  (1000) victormoreira  (1000)        0 2022-01-20 14:57:42.609141 jogos_python-0.9.0/jogos_python.egg-info/
--rw-r--r--   0 victormoreira  (1000) victormoreira  (1000)     3346 2022-01-20 14:57:42.000000 jogos_python-0.9.0/jogos_python.egg-info/PKG-INFO
--rw-r--r--   0 victormoreira  (1000) victormoreira  (1000)      354 2022-01-20 14:57:42.000000 jogos_python-0.9.0/jogos_python.egg-info/SOURCES.txt
--rw-r--r--   0 victormoreira  (1000) victormoreira  (1000)        1 2022-01-20 14:57:42.000000 jogos_python-0.9.0/jogos_python.egg-info/dependency_links.txt
--rw-r--r--   0 victormoreira  (1000) victormoreira  (1000)        7 2022-01-20 14:57:42.000000 jogos_python-0.9.0/jogos_python.egg-info/requires.txt
--rw-r--r--   0 victormoreira  (1000) victormoreira  (1000)       13 2022-01-20 14:57:42.000000 jogos_python-0.9.0/jogos_python.egg-info/top_level.txt
--rw-r--r--   0 victormoreira  (1000) victormoreira  (1000)       38 2022-01-20 14:57:42.609141 jogos_python-0.9.0/setup.cfg
--rw-r--r--   0 victormoreira  (1000) victormoreira  (1000)      538 2022-01-20 14:57:03.000000 jogos_python-0.9.0/setup.py
+drwxr-xr-x   0 victormoreira  (1000) victormoreira  (1000)        0 2022-01-20 15:19:59.463855 jogos_python-0.9.1/
+-rw-r--r--   0 victormoreira  (1000) victormoreira  (1000)       26 2021-08-08 11:39:03.000000 jogos_python-0.9.1/MANIFEST.in
+-rw-r--r--   0 victormoreira  (1000) victormoreira  (1000)     3346 2022-01-20 15:19:59.463855 jogos_python-0.9.1/PKG-INFO
+-rw-r--r--   0 victormoreira  (1000) victormoreira  (1000)     2438 2021-07-24 07:54:45.000000 jogos_python-0.9.1/README.md
+drwxr-xr-x   0 victormoreira  (1000) victormoreira  (1000)        0 2022-01-20 15:19:59.463855 jogos_python-0.9.1/jogos_python/
+-rw-r--r--   0 victormoreira  (1000) victormoreira  (1000)    24031 2022-01-20 15:17:13.000000 jogos_python-0.9.1/jogos_python/__init__.py
+-rw-r--r--   0 victormoreira  (1000) victormoreira  (1000)    15413 2021-08-24 20:28:21.000000 jogos_python-0.9.1/jogos_python/caixa.png
+-rw-r--r--   0 victormoreira  (1000) victormoreira  (1000)    14924 2021-08-05 13:46:39.000000 jogos_python-0.9.1/jogos_python/fazenda.png
+-rw-r--r--   0 victormoreira  (1000) victormoreira  (1000)    14810 2021-08-05 13:46:39.000000 jogos_python-0.9.1/jogos_python/galinha.png
+-rw-r--r--   0 victormoreira  (1000) victormoreira  (1000)     1009 2021-08-05 13:46:39.000000 jogos_python-0.9.1/jogos_python/ovo.png
+-rw-r--r--   0 victormoreira  (1000) victormoreira  (1000)    12686 2021-08-05 13:46:39.000000 jogos_python-0.9.1/jogos_python/pintinho.png
+drwxr-xr-x   0 victormoreira  (1000) victormoreira  (1000)        0 2022-01-20 15:19:59.463855 jogos_python-0.9.1/jogos_python.egg-info/
+-rw-r--r--   0 victormoreira  (1000) victormoreira  (1000)     3346 2022-01-20 15:19:59.000000 jogos_python-0.9.1/jogos_python.egg-info/PKG-INFO
+-rw-r--r--   0 victormoreira  (1000) victormoreira  (1000)      354 2022-01-20 15:19:59.000000 jogos_python-0.9.1/jogos_python.egg-info/SOURCES.txt
+-rw-r--r--   0 victormoreira  (1000) victormoreira  (1000)        1 2022-01-20 15:19:59.000000 jogos_python-0.9.1/jogos_python.egg-info/dependency_links.txt
+-rw-r--r--   0 victormoreira  (1000) victormoreira  (1000)        7 2022-01-20 15:19:59.000000 jogos_python-0.9.1/jogos_python.egg-info/requires.txt
+-rw-r--r--   0 victormoreira  (1000) victormoreira  (1000)       13 2022-01-20 15:19:59.000000 jogos_python-0.9.1/jogos_python.egg-info/top_level.txt
+-rw-r--r--   0 victormoreira  (1000) victormoreira  (1000)       38 2022-01-20 15:19:59.463855 jogos_python-0.9.1/setup.cfg
+-rw-r--r--   0 victormoreira  (1000) victormoreira  (1000)      538 2022-01-20 15:19:43.000000 jogos_python-0.9.1/setup.py
```

### Comparing `jogos_python-0.9.0/PKG-INFO` & `jogos_python-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jogos_python
-Version: 0.9.0
+Version: 0.9.1
 Summary: Facilita a criação de jogos com Python
 Home-page: https://jogos-python.readthedocs.io
 Author: LIpE/UFRJ
 Author-email: lipe@poli.ufrj.br
 License: UNKNOWN
 Description: # jogos_python
```

### Comparing `jogos_python-0.9.0/README.md` & `jogos_python-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `jogos_python-0.9.0/jogos_python/__init__.py` & `jogos_python-0.9.1/jogos_python/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -751,16 +751,21 @@
     #texta se tempo é float ou int
     if( isinstance( tempo, (int, float) ) ):
         time.sleep(tempo)
         despausar()
         
 #usado quando uma ação precisa de um intervalo entre uma
 #execução e outra
+#o usuário deve escolher entre usar a função de período ou
+#frequência
 esperar = time.sleep
-frequencia = pygame.time.Clock().tick
+definir_frequencia = pygame.time.Clock().tick
+def definir_periodo( periodo ): 
+    pygame.time.Clock().tick( 1/periodo )
+
 
 #roda ação em paralelo
 def rodar_em_paralelo( funcao, argumentos = [] ):
     if( argumentos == [] ):
         threading.Thread( target= funcao ).start()
     else:
         threading.Thread( target= funcao, args = argumentos ).start()
```

### Comparing `jogos_python-0.9.0/jogos_python/caixa.png` & `jogos_python-0.9.1/jogos_python/caixa.png`

 * *Files identical despite different names*

### Comparing `jogos_python-0.9.0/jogos_python/fazenda.png` & `jogos_python-0.9.1/jogos_python/fazenda.png`

 * *Files identical despite different names*

### Comparing `jogos_python-0.9.0/jogos_python/galinha.png` & `jogos_python-0.9.1/jogos_python/galinha.png`

 * *Files identical despite different names*

### Comparing `jogos_python-0.9.0/jogos_python/ovo.png` & `jogos_python-0.9.1/jogos_python/ovo.png`

 * *Files identical despite different names*

### Comparing `jogos_python-0.9.0/jogos_python/pintinho.png` & `jogos_python-0.9.1/jogos_python/pintinho.png`

 * *Files identical despite different names*

### Comparing `jogos_python-0.9.0/jogos_python.egg-info/PKG-INFO` & `jogos_python-0.9.1/jogos_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jogos-python
-Version: 0.9.0
+Version: 0.9.1
 Summary: Facilita a criação de jogos com Python
 Home-page: https://jogos-python.readthedocs.io
 Author: LIpE/UFRJ
 Author-email: lipe@poli.ufrj.br
 License: UNKNOWN
 Description: # jogos_python
```

### Comparing `jogos_python-0.9.0/setup.py` & `jogos_python-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text()
 
 setup(
     name="jogos_python",
-    version="0.9.0",
+    version="0.9.1",
     description="Facilita a criação de jogos com Python",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://jogos-python.readthedocs.io",
     author="LIpE/UFRJ",
     author_email="lipe@poli.ufrj.br",
     packages=["jogos_python"],
```

