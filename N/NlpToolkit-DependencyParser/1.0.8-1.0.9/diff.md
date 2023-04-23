# Comparing `tmp/NlpToolkit-DependencyParser-1.0.8.tar.gz` & `tmp/NlpToolkit-DependencyParser-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/NlpToolkit-DependencyParser-1.0.8.tar", last modified: Wed Feb 19 18:05:51 2020, max compression
+gzip compressed data, was "dist/NlpToolkit-DependencyParser-1.0.9.tar", last modified: Mon Jun  8 16:49:47 2020, max compression
```

## Comparing `NlpToolkit-DependencyParser-1.0.8.tar` & `NlpToolkit-DependencyParser-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 olcay      (501) staff       (20)        0 2020-02-19 18:05:51.000000 NlpToolkit-DependencyParser-1.0.8/
-drwxr-xr-x   0 olcay      (501) staff       (20)        0 2020-02-19 18:05:51.000000 NlpToolkit-DependencyParser-1.0.8/DependencyParser/
--rw-r--r--   0 olcay      (501) staff       (20)      583 2020-02-19 18:05:09.000000 NlpToolkit-DependencyParser-1.0.8/DependencyParser/DependencyRelation.py
--rw-r--r--   0 olcay      (501) staff       (20)     4515 2020-02-19 18:05:09.000000 NlpToolkit-DependencyParser-1.0.8/DependencyParser/StanfordDependencyRelation.py
--rw-r--r--   0 olcay      (501) staff       (20)      998 2019-12-13 06:32:09.000000 NlpToolkit-DependencyParser-1.0.8/DependencyParser/StanfordDependencyType.py
--rw-r--r--   0 olcay      (501) staff       (20)     4054 2020-02-19 18:05:09.000000 NlpToolkit-DependencyParser-1.0.8/DependencyParser/TurkishDependencyRelation.py
--rw-r--r--   0 olcay      (501) staff       (20)     1012 2020-02-19 18:05:09.000000 NlpToolkit-DependencyParser-1.0.8/DependencyParser/TurkishDependencyTreeBankCorpus.py
--rw-r--r--   0 olcay      (501) staff       (20)     1331 2020-02-19 18:05:09.000000 NlpToolkit-DependencyParser-1.0.8/DependencyParser/TurkishDependencyTreeBankSentence.py
--rw-r--r--   0 olcay      (501) staff       (20)     3747 2020-02-19 18:05:09.000000 NlpToolkit-DependencyParser-1.0.8/DependencyParser/TurkishDependencyTreeBankWord.py
--rw-r--r--   0 olcay      (501) staff       (20)      647 2019-12-13 06:33:36.000000 NlpToolkit-DependencyParser-1.0.8/DependencyParser/TurkishDependencyType.py
--rw-r--r--   0 olcay      (501) staff       (20)     4154 2020-02-19 18:05:09.000000 NlpToolkit-DependencyParser-1.0.8/DependencyParser/UniversalDependencyRelation.py
--rw-r--r--   0 olcay      (501) staff       (20)      877 2020-01-19 16:11:58.000000 NlpToolkit-DependencyParser-1.0.8/DependencyParser/UniversalDependencyType.py
--rw-r--r--   0 olcay      (501) staff       (20)        0 2019-12-13 06:24:54.000000 NlpToolkit-DependencyParser-1.0.8/DependencyParser/__init__.py
-drwxr-xr-x   0 olcay      (501) staff       (20)        0 2020-02-19 18:05:51.000000 NlpToolkit-DependencyParser-1.0.8/NlpToolkit_DependencyParser.egg-info/
--rw-r--r--   0 olcay      (501) staff       (20)      288 2020-02-19 18:05:51.000000 NlpToolkit-DependencyParser-1.0.8/NlpToolkit_DependencyParser.egg-info/PKG-INFO
--rw-r--r--   0 olcay      (501) staff       (20)      756 2020-02-19 18:05:51.000000 NlpToolkit-DependencyParser-1.0.8/NlpToolkit_DependencyParser.egg-info/SOURCES.txt
--rw-r--r--   0 olcay      (501) staff       (20)        1 2020-02-19 18:05:51.000000 NlpToolkit-DependencyParser-1.0.8/NlpToolkit_DependencyParser.egg-info/dependency_links.txt
--rw-r--r--   0 olcay      (501) staff       (20)       33 2020-02-19 18:05:51.000000 NlpToolkit-DependencyParser-1.0.8/NlpToolkit_DependencyParser.egg-info/requires.txt
--rw-r--r--   0 olcay      (501) staff       (20)       17 2020-02-19 18:05:51.000000 NlpToolkit-DependencyParser-1.0.8/NlpToolkit_DependencyParser.egg-info/top_level.txt
--rw-r--r--   0 olcay      (501) staff       (20)      288 2020-02-19 18:05:51.000000 NlpToolkit-DependencyParser-1.0.8/PKG-INFO
--rw-r--r--   0 olcay      (501) staff       (20)       38 2020-02-19 18:05:51.000000 NlpToolkit-DependencyParser-1.0.8/setup.cfg
--rw-r--r--   0 olcay      (501) staff       (20)      392 2020-02-19 18:05:09.000000 NlpToolkit-DependencyParser-1.0.8/setup.py
+drwxr-xr-x   0 olcay      (501) staff       (20)        0 2020-06-08 16:49:47.000000 NlpToolkit-DependencyParser-1.0.9/
+drwxr-xr-x   0 olcay      (501) staff       (20)        0 2020-06-08 16:49:47.000000 NlpToolkit-DependencyParser-1.0.9/DependencyParser/
+-rw-r--r--   0 olcay      (501) staff       (20)      583 2020-02-19 18:05:09.000000 NlpToolkit-DependencyParser-1.0.9/DependencyParser/DependencyRelation.py
+-rw-r--r--   0 olcay      (501) staff       (20)     4515 2020-02-19 18:05:09.000000 NlpToolkit-DependencyParser-1.0.9/DependencyParser/StanfordDependencyRelation.py
+-rw-r--r--   0 olcay      (501) staff       (20)      998 2019-12-13 06:32:09.000000 NlpToolkit-DependencyParser-1.0.9/DependencyParser/StanfordDependencyType.py
+-rw-r--r--   0 olcay      (501) staff       (20)     4054 2020-02-19 18:05:09.000000 NlpToolkit-DependencyParser-1.0.9/DependencyParser/TurkishDependencyRelation.py
+-rw-r--r--   0 olcay      (501) staff       (20)     1012 2020-02-19 18:05:09.000000 NlpToolkit-DependencyParser-1.0.9/DependencyParser/TurkishDependencyTreeBankCorpus.py
+-rw-r--r--   0 olcay      (501) staff       (20)     1331 2020-02-19 18:05:09.000000 NlpToolkit-DependencyParser-1.0.9/DependencyParser/TurkishDependencyTreeBankSentence.py
+-rw-r--r--   0 olcay      (501) staff       (20)     3928 2020-06-08 16:48:01.000000 NlpToolkit-DependencyParser-1.0.9/DependencyParser/TurkishDependencyTreeBankWord.py
+-rw-r--r--   0 olcay      (501) staff       (20)      647 2019-12-13 06:33:36.000000 NlpToolkit-DependencyParser-1.0.9/DependencyParser/TurkishDependencyType.py
+-rw-r--r--   0 olcay      (501) staff       (20)     4154 2020-02-19 18:05:09.000000 NlpToolkit-DependencyParser-1.0.9/DependencyParser/UniversalDependencyRelation.py
+-rw-r--r--   0 olcay      (501) staff       (20)      877 2020-01-19 16:11:58.000000 NlpToolkit-DependencyParser-1.0.9/DependencyParser/UniversalDependencyType.py
+-rw-r--r--   0 olcay      (501) staff       (20)        0 2019-12-13 06:24:54.000000 NlpToolkit-DependencyParser-1.0.9/DependencyParser/__init__.py
+drwxr-xr-x   0 olcay      (501) staff       (20)        0 2020-06-08 16:49:47.000000 NlpToolkit-DependencyParser-1.0.9/NlpToolkit_DependencyParser.egg-info/
+-rw-r--r--   0 olcay      (501) staff       (20)      288 2020-06-08 16:49:47.000000 NlpToolkit-DependencyParser-1.0.9/NlpToolkit_DependencyParser.egg-info/PKG-INFO
+-rw-r--r--   0 olcay      (501) staff       (20)      766 2020-06-08 16:49:47.000000 NlpToolkit-DependencyParser-1.0.9/NlpToolkit_DependencyParser.egg-info/SOURCES.txt
+-rw-r--r--   0 olcay      (501) staff       (20)        1 2020-06-08 16:49:47.000000 NlpToolkit-DependencyParser-1.0.9/NlpToolkit_DependencyParser.egg-info/dependency_links.txt
+-rw-r--r--   0 olcay      (501) staff       (20)       33 2020-06-08 16:49:47.000000 NlpToolkit-DependencyParser-1.0.9/NlpToolkit_DependencyParser.egg-info/requires.txt
+-rw-r--r--   0 olcay      (501) staff       (20)       17 2020-06-08 16:49:47.000000 NlpToolkit-DependencyParser-1.0.9/NlpToolkit_DependencyParser.egg-info/top_level.txt
+-rw-r--r--   0 olcay      (501) staff       (20)      288 2020-06-08 16:49:47.000000 NlpToolkit-DependencyParser-1.0.9/PKG-INFO
+-rw-r--r--   0 olcay      (501) staff       (20)     1290 2020-06-01 20:53:42.000000 NlpToolkit-DependencyParser-1.0.9/README.md
+-rw-r--r--   0 olcay      (501) staff       (20)       38 2020-06-08 16:49:47.000000 NlpToolkit-DependencyParser-1.0.9/setup.cfg
+-rw-r--r--   0 olcay      (501) staff       (20)      392 2020-06-08 16:40:02.000000 NlpToolkit-DependencyParser-1.0.9/setup.py
```

### Comparing `NlpToolkit-DependencyParser-1.0.8/DependencyParser/DependencyRelation.py` & `NlpToolkit-DependencyParser-1.0.9/DependencyParser/DependencyRelation.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-DependencyParser-1.0.8/DependencyParser/StanfordDependencyRelation.py` & `NlpToolkit-DependencyParser-1.0.9/DependencyParser/StanfordDependencyRelation.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-DependencyParser-1.0.8/DependencyParser/StanfordDependencyType.py` & `NlpToolkit-DependencyParser-1.0.9/DependencyParser/StanfordDependencyType.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-DependencyParser-1.0.8/DependencyParser/TurkishDependencyRelation.py` & `NlpToolkit-DependencyParser-1.0.9/DependencyParser/TurkishDependencyRelation.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-DependencyParser-1.0.8/DependencyParser/TurkishDependencyTreeBankCorpus.py` & `NlpToolkit-DependencyParser-1.0.9/DependencyParser/TurkishDependencyTreeBankCorpus.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-DependencyParser-1.0.8/DependencyParser/TurkishDependencyTreeBankSentence.py` & `NlpToolkit-DependencyParser-1.0.9/DependencyParser/TurkishDependencyTreeBankSentence.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-DependencyParser-1.0.8/DependencyParser/TurkishDependencyTreeBankWord.py` & `NlpToolkit-DependencyParser-1.0.9/DependencyParser/TurkishDependencyTreeBankWord.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,15 +24,17 @@
             Xml parsed node containing information about a word.
         """
         toWord = 0
         toIG = 0
         self.__originalParses = []
         self.name = wordNode.text
         IG = wordNode.attrib["IG"]
+        IG = IG[:IG.index("+")] + "+" + IG[IG.index("+") + 1:].upper()
         self.__parse = MorphologicalParse(self.splitIntoInflectionalGroups(IG))
+        self.__relation = None
         relationName = wordNode.attrib["REL"]
         if relationName != "[,( )]":
             relationParts = re.compile("[\\[()\\],]").split(relationName)
             index = 0
             for part in relationParts:
                 if len(part) != 0:
                     index = index + 1
@@ -41,14 +43,15 @@
                     elif index == 2:
                         toIG = int(part)
                     elif index == 3:
                         self.__relation = TurkishDependencyRelation(toWord - 1, toIG - 1, part)
         for i in range(1, 10):
             if ("ORG_ID" + str(i)) in wordNode.attrib:
                 IG = wordNode.attrib["ORG_ID" + str(i)]
+                IG = IG[:IG.index("+")] + "+" + IG[IG.index("+") + 1:].upper()
                 self.__originalParses.append(MorphologicalParse(self.splitIntoInflectionalGroups(IG)))
 
     def splitIntoInflectionalGroups(self, IG: str) -> list:
         """
         Given the morphological parse of a word, this method splits it into inflectional groups.
 
         PARAMETERS
```

### Comparing `NlpToolkit-DependencyParser-1.0.8/DependencyParser/TurkishDependencyType.py` & `NlpToolkit-DependencyParser-1.0.9/DependencyParser/TurkishDependencyType.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-DependencyParser-1.0.8/DependencyParser/UniversalDependencyRelation.py` & `NlpToolkit-DependencyParser-1.0.9/DependencyParser/UniversalDependencyRelation.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-DependencyParser-1.0.8/DependencyParser/UniversalDependencyType.py` & `NlpToolkit-DependencyParser-1.0.9/DependencyParser/UniversalDependencyType.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-DependencyParser-1.0.8/NlpToolkit_DependencyParser.egg-info/SOURCES.txt` & `NlpToolkit-DependencyParser-1.0.9/NlpToolkit_DependencyParser.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+README.md
 setup.py
 DependencyParser/DependencyRelation.py
 DependencyParser/StanfordDependencyRelation.py
 DependencyParser/StanfordDependencyType.py
 DependencyParser/TurkishDependencyRelation.py
 DependencyParser/TurkishDependencyTreeBankCorpus.py
 DependencyParser/TurkishDependencyTreeBankSentence.py
```

