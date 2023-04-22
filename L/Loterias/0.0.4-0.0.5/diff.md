# Comparing `tmp/Loterias-0.0.4.tar.gz` & `tmp/Loterias-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Loterias-0.0.4.tar", last modified: Sat Apr 22 23:03:03 2023, max compression
+gzip compressed data, was "Loterias-0.0.5.tar", last modified: Sat Apr 22 23:14:46 2023, max compression
```

## Comparing `Loterias-0.0.4.tar` & `Loterias-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 23:03:03.403266 Loterias-0.0.4/
--rw-rw-rw-   0        0        0     1097 2023-04-20 11:21:01.000000 Loterias-0.0.4/LICENCE
-drwxrwxrwx   0        0        0        0 2023-04-22 23:03:03.387645 Loterias-0.0.4/Loterias/
--rw-rw-rw-   0        0        0     2137 2023-04-18 11:46:15.000000 Loterias-0.0.4/Loterias/Apurar.py
--rw-rw-rw-   0        0        0     7851 2023-04-22 22:57:55.000000 Loterias-0.0.4/Loterias/Collection.py
--rw-rw-rw-   0        0        0     5178 2023-04-18 11:45:08.000000 Loterias-0.0.4/Loterias/Collections.py
--rw-rw-rw-   0        0        0     3331 2023-04-18 11:45:08.000000 Loterias-0.0.4/Loterias/Interpoler.py
--rw-rw-rw-   0        0        0    10489 2023-04-19 10:36:19.000000 Loterias-0.0.4/Loterias/Loto.py
--rw-rw-rw-   0        0        0      916 2023-04-18 11:45:08.000000 Loterias-0.0.4/Loterias/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-22 23:03:03.403266 Loterias-0.0.4/Loterias.egg-info/
--rw-rw-rw-   0        0        0     1645 2023-04-22 23:03:03.000000 Loterias-0.0.4/Loterias.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-04-22 23:03:03.000000 Loterias-0.0.4/Loterias.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 23:03:03.000000 Loterias-0.0.4/Loterias.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-04-22 23:03:03.000000 Loterias-0.0.4/Loterias.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-22 23:03:03.000000 Loterias-0.0.4/Loterias.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1645 2023-04-22 23:03:03.403266 Loterias-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1262 2023-04-20 12:09:33.000000 Loterias-0.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-04-22 23:03:03.403266 Loterias-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      514 2023-04-22 23:01:23.000000 Loterias-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 23:14:46.176694 Loterias-0.0.5/
+-rw-rw-rw-   0        0        0     1097 2023-04-20 11:21:01.000000 Loterias-0.0.5/LICENCE
+drwxrwxrwx   0        0        0        0 2023-04-22 23:14:46.145437 Loterias-0.0.5/Loterias/
+-rw-rw-rw-   0        0        0     2137 2023-04-18 11:46:15.000000 Loterias-0.0.5/Loterias/Apurar.py
+-rw-rw-rw-   0        0        0     8511 2023-04-22 23:13:42.000000 Loterias-0.0.5/Loterias/Collection.py
+-rw-rw-rw-   0        0        0     5178 2023-04-18 11:45:08.000000 Loterias-0.0.5/Loterias/Collections.py
+-rw-rw-rw-   0        0        0     3331 2023-04-18 11:45:08.000000 Loterias-0.0.5/Loterias/Interpoler.py
+-rw-rw-rw-   0        0        0    10489 2023-04-19 10:36:19.000000 Loterias-0.0.5/Loterias/Loto.py
+-rw-rw-rw-   0        0        0      916 2023-04-18 11:45:08.000000 Loterias-0.0.5/Loterias/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-22 23:14:46.161024 Loterias-0.0.5/Loterias.egg-info/
+-rw-rw-rw-   0        0        0     1870 2023-04-22 23:14:46.000000 Loterias-0.0.5/Loterias.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-04-22 23:14:46.000000 Loterias-0.0.5/Loterias.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 23:14:46.000000 Loterias-0.0.5/Loterias.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-04-22 23:14:46.000000 Loterias-0.0.5/Loterias.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-22 23:14:46.000000 Loterias-0.0.5/Loterias.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1870 2023-04-22 23:14:46.161024 Loterias-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1485 2023-04-22 23:11:47.000000 Loterias-0.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-22 23:14:46.176694 Loterias-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      514 2023-04-22 23:14:38.000000 Loterias-0.0.5/setup.py
```

### Comparing `Loterias-0.0.4/LICENCE` & `Loterias-0.0.5/LICENCE`

 * *Files identical despite different names*

### Comparing `Loterias-0.0.4/Loterias/Apurar.py` & `Loterias-0.0.5/Loterias/Apurar.py`

 * *Files identical despite different names*

### Comparing `Loterias-0.0.4/Loterias/Collection.py` & `Loterias-0.0.5/Loterias/Collection.py`

 * *Files 4% similar despite different names*

```diff
@@ -286,10 +286,38 @@
         self.__verbose = 'Iniciar pesquisa'
         self.wait()
 
     @property
     def values(self) -> pd.DataFrame:
         if len(self.buffer) == 0:
             self.startAndWait()
+            print('')
         return self.buffer
         #df = DataFrame(self.buffer)
         #return df.sort_values(by='concurso')
+
+    @property
+    def getDezenas(self):
+        dzs = self.__lb().volante.sorteio
+        cols = ['concurso']
+        for i in range(1, dzs+1):
+            cols.append(f'Dz{i}')
+
+        return self.values[cols]
+
+    @property
+    def getSomas(self):
+        dzs = self.__lb().volante.dezenas
+        cols = ['concurso']
+        for i in range(0, dzs):
+            cols.append(f'smDz{i}')
+
+        return self.values[cols]
+
+    @property
+    def getContagem(self):
+        dzs = self.__lb().volante.dezenas
+        cols = ['concurso']
+        for i in range(0, dzs):
+            cols.append(f'ctDz{i}')
+
+        return self.values[cols]
```

### Comparing `Loterias-0.0.4/Loterias/Collections.py` & `Loterias-0.0.5/Loterias/Collections.py`

 * *Files identical despite different names*

### Comparing `Loterias-0.0.4/Loterias/Interpoler.py` & `Loterias-0.0.5/Loterias/Interpoler.py`

 * *Files identical despite different names*

### Comparing `Loterias-0.0.4/Loterias/Loto.py` & `Loterias-0.0.5/Loterias/Loto.py`

 * *Files identical despite different names*

### Comparing `Loterias-0.0.4/Loterias/__init__.py` & `Loterias-0.0.5/Loterias/__init__.py`

 * *Files identical despite different names*

### Comparing `Loterias-0.0.4/Loterias.egg-info/PKG-INFO` & `Loterias-0.0.5/Loterias.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Loterias
-Version: 0.0.4
+Version: 0.0.5
 Summary: Wrapper não oficial para pesquisa de dados lotéricos em thread
 Home-page: UNKNOWN
 Author: PKG
 Author-email: drjpp.drjpp@gmail.com
 License: MIT License
 Keywords: loterias CEF
 Platform: UNKNOWN
@@ -32,9 +32,14 @@
 
 Elementos/Rotinas de CollectionByType
     maxThreads      Ajusta o nÃºmero mÃ¡ximo de threads [para mÃºltipla pesquisa]
     sorteioInicial  Ajusta o nÃºmero do sorteio inicial
     sorteioFinal    Limita o nÃºmero do sorteio final [default Ã© o Ãºltimo sorteio
     verbose         Apresenta ou nÃ£o algumas informaÃ§Ãµes durante a pesquisa
     value           Inicia a busca, se necessÃ¡rio, de dados e apresenta o resultado em pandas.DataFrame
-    
+
+v 0.0.5
+    Adicionados mÃ©todos
+    getDezenas      Extrai a lista de dezemas
+    getSomas        Extrai a lista de somas, considerado cada sorteio
+    getContagem     Extrai a contagem individual relativo a cada sorteio
```

### Comparing `Loterias-0.0.4/PKG-INFO` & `Loterias-0.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Loterias
-Version: 0.0.4
+Version: 0.0.5
 Summary: Wrapper não oficial para pesquisa de dados lotéricos em thread
 Home-page: UNKNOWN
 Author: PKG
 Author-email: drjpp.drjpp@gmail.com
 License: MIT License
 Keywords: loterias CEF
 Platform: UNKNOWN
@@ -32,9 +32,14 @@
 
 Elementos/Rotinas de CollectionByType
     maxThreads      Ajusta o nÃºmero mÃ¡ximo de threads [para mÃºltipla pesquisa]
     sorteioInicial  Ajusta o nÃºmero do sorteio inicial
     sorteioFinal    Limita o nÃºmero do sorteio final [default Ã© o Ãºltimo sorteio
     verbose         Apresenta ou nÃ£o algumas informaÃ§Ãµes durante a pesquisa
     value           Inicia a busca, se necessÃ¡rio, de dados e apresenta o resultado em pandas.DataFrame
-    
+
+v 0.0.5
+    Adicionados mÃ©todos
+    getDezenas      Extrai a lista de dezemas
+    getSomas        Extrai a lista de somas, considerado cada sorteio
+    getContagem     Extrai a contagem individual relativo a cada sorteio
```

### Comparing `Loterias-0.0.4/README.md` & `Loterias-0.0.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -19,8 +19,13 @@
 
 Elementos/Rotinas de CollectionByType
     maxThreads      Ajusta o número máximo de threads [para múltipla pesquisa]
     sorteioInicial  Ajusta o número do sorteio inicial
     sorteioFinal    Limita o número do sorteio final [default é o último sorteio
     verbose         Apresenta ou não algumas informações durante a pesquisa
     value           Inicia a busca, se necessário, de dados e apresenta o resultado em pandas.DataFrame
-    
+
+v 0.0.5
+    Adicionados métodos
+    getDezenas      Extrai a lista de dezemas
+    getSomas        Extrai a lista de somas, considerado cada sorteio
+    getContagem     Extrai a contagem individual relativo a cada sorteio
```

### Comparing `Loterias-0.0.4/setup.py` & `Loterias-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
 setup(name='Loterias',
-    version='0.0.4',
+    version='0.0.5',
     license='MIT License',
     author='PKG',
     long_description=readme,
     long_description_content_type="text/markdown",
     author_email='drjpp.drjpp@gmail.com',
     keywords='loterias CEF',
     description=u'Wrapper não oficial para pesquisa de dados lotéricos em thread',
```

