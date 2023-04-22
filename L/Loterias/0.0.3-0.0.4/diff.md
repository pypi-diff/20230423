# Comparing `tmp/Loterias-0.0.3.tar.gz` & `tmp/Loterias-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Loterias-0.0.3.tar", last modified: Thu Apr 20 12:15:46 2023, max compression
+gzip compressed data, was "Loterias-0.0.4.tar", last modified: Sat Apr 22 23:03:03 2023, max compression
```

## Comparing `Loterias-0.0.3.tar` & `Loterias-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 12:15:46.594887 Loterias-0.0.3/
--rw-rw-rw-   0        0        0     1097 2023-04-20 11:21:01.000000 Loterias-0.0.3/LICENCE
-drwxrwxrwx   0        0        0        0 2023-04-20 12:15:46.584382 Loterias-0.0.3/Loterias/
--rw-rw-rw-   0        0        0     2137 2023-04-18 11:46:15.000000 Loterias-0.0.3/Loterias/Apurar.py
--rw-rw-rw-   0        0        0     7121 2023-04-20 11:40:08.000000 Loterias-0.0.3/Loterias/Collection.py
--rw-rw-rw-   0        0        0     5178 2023-04-18 11:45:08.000000 Loterias-0.0.3/Loterias/Collections.py
--rw-rw-rw-   0        0        0     3331 2023-04-18 11:45:08.000000 Loterias-0.0.3/Loterias/Interpoler.py
--rw-rw-rw-   0        0        0    10489 2023-04-19 10:36:19.000000 Loterias-0.0.3/Loterias/Loto.py
--rw-rw-rw-   0        0        0      916 2023-04-18 11:45:08.000000 Loterias-0.0.3/Loterias/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 12:15:46.594887 Loterias-0.0.3/Loterias.egg-info/
--rw-rw-rw-   0        0        0     1645 2023-04-20 12:15:46.000000 Loterias-0.0.3/Loterias.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-04-20 12:15:46.000000 Loterias-0.0.3/Loterias.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 12:15:46.000000 Loterias-0.0.3/Loterias.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-04-20 12:15:46.000000 Loterias-0.0.3/Loterias.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-20 12:15:46.000000 Loterias-0.0.3/Loterias.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1645 2023-04-20 12:15:46.594887 Loterias-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1262 2023-04-20 12:09:33.000000 Loterias-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-04-20 12:15:46.594887 Loterias-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      514 2023-04-20 12:14:29.000000 Loterias-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 23:03:03.403266 Loterias-0.0.4/
+-rw-rw-rw-   0        0        0     1097 2023-04-20 11:21:01.000000 Loterias-0.0.4/LICENCE
+drwxrwxrwx   0        0        0        0 2023-04-22 23:03:03.387645 Loterias-0.0.4/Loterias/
+-rw-rw-rw-   0        0        0     2137 2023-04-18 11:46:15.000000 Loterias-0.0.4/Loterias/Apurar.py
+-rw-rw-rw-   0        0        0     7851 2023-04-22 22:57:55.000000 Loterias-0.0.4/Loterias/Collection.py
+-rw-rw-rw-   0        0        0     5178 2023-04-18 11:45:08.000000 Loterias-0.0.4/Loterias/Collections.py
+-rw-rw-rw-   0        0        0     3331 2023-04-18 11:45:08.000000 Loterias-0.0.4/Loterias/Interpoler.py
+-rw-rw-rw-   0        0        0    10489 2023-04-19 10:36:19.000000 Loterias-0.0.4/Loterias/Loto.py
+-rw-rw-rw-   0        0        0      916 2023-04-18 11:45:08.000000 Loterias-0.0.4/Loterias/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-22 23:03:03.403266 Loterias-0.0.4/Loterias.egg-info/
+-rw-rw-rw-   0        0        0     1645 2023-04-22 23:03:03.000000 Loterias-0.0.4/Loterias.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-04-22 23:03:03.000000 Loterias-0.0.4/Loterias.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 23:03:03.000000 Loterias-0.0.4/Loterias.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-04-22 23:03:03.000000 Loterias-0.0.4/Loterias.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-22 23:03:03.000000 Loterias-0.0.4/Loterias.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1645 2023-04-22 23:03:03.403266 Loterias-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1262 2023-04-20 12:09:33.000000 Loterias-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-22 23:03:03.403266 Loterias-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      514 2023-04-22 23:01:23.000000 Loterias-0.0.4/setup.py
```

### Comparing `Loterias-0.0.3/LICENCE` & `Loterias-0.0.4/LICENCE`

 * *Files identical despite different names*

### Comparing `Loterias-0.0.3/Loterias/Apurar.py` & `Loterias-0.0.4/Loterias/Apurar.py`

 * *Files identical despite different names*

### Comparing `Loterias-0.0.3/Loterias/Collection.py` & `Loterias-0.0.4/Loterias/Collection.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 
 import sys
 from threading import Thread
-from pandas import DataFrame
+#from pandas import DataFrame
+import pandas as pd
 from .Loto import ExportLoteriaBase
 # from .Volante import Volantes
 from .Apurar import Apostas
 
 import warnings
 warnings.filterwarnings('ignore')
 
@@ -26,14 +27,55 @@
             self.start()
 
     def run(self) -> None:
         while not self.stop:
             if not self.stop and self.callProcess:
                 self.stop = self.callProcess(self)
 
+class srcCounter:
+    def __init__(self, dezenas=0):
+        self.__dezenas = dezenas
+        self.soma = []
+        self.cont = []
+
+        #Lista para integrar o dicionário final
+        self.finalSoma = []
+        self.finalCont = []
+
+        self.doMake()
+
+    def doMake(self):
+        self.soma = [0 for i in range(0, self.__dezenas)]
+        self.cont = [0 for i in range(0, self.__dezenas)]
+
+    def resetCont(self):
+        self.cont = [0 for i in range(0, self.__dezenas)]
+
+    def calculate(self, v):
+        self.soma[v] += 1
+        self.cont[v] += 1
+
+    @property
+    def getDict(self):
+        soma = {}
+        cont = {}
+
+        def __process(i):
+            soma.update({f'smDz{i}': self.soma[i]})
+            cont.update({f'ctDz{i}': self.cont[i]})
+
+        #for i in range(0, self.__dezenas):
+        #    soma.update({f'smDz{i}': self.soma[i]})
+        #    cont.update({f'ctDz{i}': self.cont[i]})
+        [__process(i) for i in range(0, self.__dezenas)]
+
+        r = {}
+        r.update(soma)
+        r.update(cont)
+        return r
 
 class Collection:
     def __init__(self, loteriaBase=ExportLoteriaBase, maxThreads=8, concursoStart=1, verbose=False, autoStart=False):
         self.buffer = []
 
         self.__repescar = []
         self.__th = []
@@ -197,65 +239,57 @@
 
         meStop = False
         while not meStop:
             meStop = doStop()
 
         self.__doMakeCount()
 
-        print('')
-
     def __doMakeCount(self):
+        self.__verbose = 'Calcular ocorrências'
         #Executa a contagem - precisa ser incluído no final de todos os processos, pois a busca é feita em thread
-        bloco = DataFrame(self.buffer).sort_values(by='concurso')
+        bloco = pd.DataFrame(self.buffer).sort_values(by='concurso')
+
+        counter = srcCounter(self.__lb().volante.dezenas)
 
-        contagem_soma = [0 for s in range(0, self.__lb().volante.dezenas)]
-        contagem_individual = [0 for s in range(0, self.__lb().volante.dezenas)]
+        gruposDZ = list(bloco['dezenas'])
+        concurso = list(bloco['concurso'])
 
-        dezenas = list(bloco['dezenas'])
+        dc = []
 
-        soma = []
-        contagem = []
+        #Verifica individualmente cada grupo de dezenas
+        for i in range(0, len(gruposDZ)):
+            dzn = gruposDZ[i]
+            #Reseta contagem individual de valores
+            counter.resetCont()
 
+            #Calcula todos os valores de uma vez só [soma e contagem]
+            [counter.calculate(dz) for dz in dzn]
 
-        #Diferença entre o sorteio atual e o anterior
-        diferenciacao = []
+            cto = {'concurso': concurso[i]}
+            cto.update(counter.getDict)
 
-        firstDiferenciacao = True
+            dc.append(cto)
 
-        for dzn in dezenas:
-            contagem_individual = [0 for s in range(0, self.__lb().volante.dezenas)]
-            for dz in dzn:
-                contagem_soma[dz] += 1
-                contagem_individual[dz] += 1
-            soma.append(list(contagem_soma))
-            contagem.append(contagem_individual)
+        blocCount = pd.DataFrame(dc)
 
-            #Primeira vez que a diferenciacao está sendo feita,
-            #Nãm tem registro anterior para substrair contagem
-            """
-            if firstDiferenciacao:
-                diferenciacao.append(list(contagem))
-            else:
-                diferencial = [0 for s in range(0, self.__lb().volante.dezenas)]
-                for i in range(0, len(contagem)):
-                    diferencial[i]
-            """
+        self.buffer = pd.merge(bloco, blocCount, on='concurso')
 
-        bloco['soma'] = soma
-        bloco['contagem'] = contagem
+        pass
+        #bloco['soma'] = soma
+        #bloco['contagem'] = contagem
 
-        self.buffer = bloco
+        #self.buffer = bloco
 
 
     def startAndWait(self):
         self.__verbose = 'Preparar threads'
         self.start()
         self.__verbose = 'Iniciar pesquisa'
         self.wait()
 
     @property
-    def values(self) -> DataFrame:
+    def values(self) -> pd.DataFrame:
         if len(self.buffer) == 0:
             self.startAndWait()
         return self.buffer
         #df = DataFrame(self.buffer)
         #return df.sort_values(by='concurso')
```

### Comparing `Loterias-0.0.3/Loterias/Collections.py` & `Loterias-0.0.4/Loterias/Collections.py`

 * *Files identical despite different names*

### Comparing `Loterias-0.0.3/Loterias/Interpoler.py` & `Loterias-0.0.4/Loterias/Interpoler.py`

 * *Files identical despite different names*

### Comparing `Loterias-0.0.3/Loterias/Loto.py` & `Loterias-0.0.4/Loterias/Loto.py`

 * *Files identical despite different names*

### Comparing `Loterias-0.0.3/Loterias/__init__.py` & `Loterias-0.0.4/Loterias/__init__.py`

 * *Files identical despite different names*

### Comparing `Loterias-0.0.3/Loterias.egg-info/PKG-INFO` & `Loterias-0.0.4/Loterias.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Loterias
-Version: 0.0.3
+Version: 0.0.4
 Summary: Wrapper não oficial para pesquisa de dados lotéricos em thread
 Home-page: UNKNOWN
 Author: PKG
 Author-email: drjpp.drjpp@gmail.com
 License: MIT License
 Keywords: loterias CEF
 Platform: UNKNOWN
```

### Comparing `Loterias-0.0.3/PKG-INFO` & `Loterias-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Loterias
-Version: 0.0.3
+Version: 0.0.4
 Summary: Wrapper não oficial para pesquisa de dados lotéricos em thread
 Home-page: UNKNOWN
 Author: PKG
 Author-email: drjpp.drjpp@gmail.com
 License: MIT License
 Keywords: loterias CEF
 Platform: UNKNOWN
```

### Comparing `Loterias-0.0.3/README.md` & `Loterias-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `Loterias-0.0.3/setup.py` & `Loterias-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
 setup(name='Loterias',
-    version='0.0.3',
+    version='0.0.4',
     license='MIT License',
     author='PKG',
     long_description=readme,
     long_description_content_type="text/markdown",
     author_email='drjpp.drjpp@gmail.com',
     keywords='loterias CEF',
     description=u'Wrapper não oficial para pesquisa de dados lotéricos em thread',
```

