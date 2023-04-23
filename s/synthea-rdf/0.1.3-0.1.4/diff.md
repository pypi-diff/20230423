# Comparing `tmp/synthea-rdf-0.1.3.tar.gz` & `tmp/synthea-rdf-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synthea-rdf-0.1.3.tar", last modified: Sun Mar 12 02:18:49 2023, max compression
+gzip compressed data, was "synthea-rdf-0.1.4.tar", last modified: Sun Apr 23 04:06:39 2023, max compression
```

## Comparing `synthea-rdf-0.1.3.tar` & `synthea-rdf-0.1.4.tar`

### file list

```diff
@@ -1,25 +1,40 @@
-drwxrwxr-x   0 k163     (65010) k163      (1049)        0 2023-03-12 02:18:49.080542 synthea-rdf-0.1.3/
--rw-rw-r--   0 k163     (65010) k163      (1049)    35130 2023-03-03 16:20:48.000000 synthea-rdf-0.1.3/LICENSE
--rw-rw-r--   0 k163     (65010) k163      (1049)       61 2023-03-07 03:05:34.000000 synthea-rdf-0.1.3/MANIFEST.in
--rw-rw-r--   0 k163     (65010) k163      (1049)     2370 2023-03-12 02:18:49.080542 synthea-rdf-0.1.3/PKG-INFO
--rw-rw-r--   0 k163     (65010) k163      (1049)     1889 2023-03-07 03:32:36.000000 synthea-rdf-0.1.3/README.md
--rw-rw-r--   0 k163     (65010) k163      (1049)       38 2023-03-12 02:18:49.080542 synthea-rdf-0.1.3/setup.cfg
--rw-rw-r--   0 k163     (65010) k163      (1049)      739 2023-03-12 02:17:33.000000 synthea-rdf-0.1.3/setup.py
-drwxrwxr-x   0 k163     (65010) k163      (1049)        0 2023-03-12 02:18:49.080542 synthea-rdf-0.1.3/synthea_ontology/
--rw-rw-r--   0 k163     (65010) k163      (1049)   565508 2023-03-04 03:42:16.000000 synthea-rdf-0.1.3/synthea_ontology/synthea_ontology.png
--rw-rw-r--   0 k163     (65010) k163      (1049)    71879 2023-03-04 02:50:57.000000 synthea-rdf-0.1.3/synthea_ontology/synthea_ontology.ttl
-drwxrwxr-x   0 k163     (65010) k163      (1049)        0 2023-03-12 02:18:49.080542 synthea-rdf-0.1.3/synthea_rdf/
--rw-rw-r--   0 k163     (65010) k163      (1049)        0 2022-09-28 13:50:44.000000 synthea-rdf-0.1.3/synthea_rdf/__init__.py
--rw-rw-r--   0 k163     (65010) k163      (1049)     8081 2023-03-04 16:40:51.000000 synthea-rdf-0.1.3/synthea_rdf/graph.py
--rw-rw-r--   0 k163     (65010) k163      (1049)     1515 2023-03-04 03:34:56.000000 synthea-rdf-0.1.3/synthea_rdf/literal.py
--rw-rw-r--   0 k163     (65010) k163      (1049)    40283 2023-03-12 02:13:22.000000 synthea-rdf-0.1.3/synthea_rdf/resource.py
--rw-rw-r--   0 k163     (65010) k163      (1049)      585 2023-03-02 22:39:24.000000 synthea-rdf-0.1.3/synthea_rdf/settings.py
--rw-rw-r--   0 k163     (65010) k163      (1049)     1442 2023-03-04 16:34:46.000000 synthea-rdf-0.1.3/synthea_rdf/uri.py
-drwxrwxr-x   0 k163     (65010) k163      (1049)        0 2023-03-12 02:18:49.080542 synthea-rdf-0.1.3/synthea_rdf.egg-info/
--rw-rw-r--   0 k163     (65010) k163      (1049)     2370 2023-03-12 02:18:49.000000 synthea-rdf-0.1.3/synthea_rdf.egg-info/PKG-INFO
--rw-rw-r--   0 k163     (65010) k163      (1049)      445 2023-03-12 02:18:49.000000 synthea-rdf-0.1.3/synthea_rdf.egg-info/SOURCES.txt
--rw-rw-r--   0 k163     (65010) k163      (1049)        1 2023-03-12 02:18:49.000000 synthea-rdf-0.1.3/synthea_rdf.egg-info/dependency_links.txt
--rw-rw-r--   0 k163     (65010) k163      (1049)       29 2023-03-12 02:18:49.000000 synthea-rdf-0.1.3/synthea_rdf.egg-info/requires.txt
--rw-rw-r--   0 k163     (65010) k163      (1049)       12 2023-03-12 02:18:49.000000 synthea-rdf-0.1.3/synthea_rdf.egg-info/top_level.txt
-drwxrwxr-x   0 k163     (65010) k163      (1049)        0 2023-03-12 02:18:49.080542 synthea-rdf-0.1.3/tests/
--rw-rw-r--   0 k163     (65010) k163      (1049)     3951 2023-03-12 02:08:32.000000 synthea-rdf-0.1.3/tests/test_convert.py
+drwxrwxr-x   0 k163     (65010) k163      (1049)        0 2023-04-23 04:06:39.130283 synthea-rdf-0.1.4/
+-rw-rw-r--   0 k163     (65010) k163      (1049)    35130 2023-03-24 16:59:14.000000 synthea-rdf-0.1.4/LICENSE
+-rw-rw-r--   0 k163     (65010) k163      (1049)      100 2023-04-23 04:03:43.000000 synthea-rdf-0.1.4/MANIFEST.in
+-rw-rw-r--   0 k163     (65010) k163      (1049)     1990 2023-04-23 04:06:39.130283 synthea-rdf-0.1.4/PKG-INFO
+-rw-rw-r--   0 k163     (65010) k163      (1049)     1510 2023-03-24 16:59:14.000000 synthea-rdf-0.1.4/README.md
+drwxrwxr-x   0 k163     (65010) k163      (1049)        0 2023-04-23 04:06:39.130283 synthea-rdf-0.1.4/abstract/
+-rw-rw-r--   0 k163     (65010) k163      (1049)       31 2023-04-07 02:02:05.000000 synthea-rdf-0.1.4/abstract/__init__.py
+-rw-rw-r--   0 k163     (65010) k163      (1049)     1543 2023-04-10 20:00:28.000000 synthea-rdf-0.1.4/abstract/literal.py
+-rw-rw-r--   0 k163     (65010) k163      (1049)      456 2023-04-10 19:53:47.000000 synthea-rdf-0.1.4/abstract/namespace.py
+-rw-rw-r--   0 k163     (65010) k163      (1049)      410 2023-04-06 06:27:31.000000 synthea-rdf-0.1.4/abstract/resource.py
+-rw-rw-r--   0 k163     (65010) k163      (1049)     2245 2023-04-10 20:40:37.000000 synthea-rdf-0.1.4/abstract/uri.py
+drwxrwxr-x   0 k163     (65010) k163      (1049)        0 2023-04-23 04:06:39.130283 synthea-rdf-0.1.4/dua/
+-rw-rw-r--   0 k163     (65010) k163      (1049)        0 2023-04-05 20:11:51.000000 synthea-rdf-0.1.4/dua/__init__.py
+-rw-rw-r--   0 k163     (65010) k163      (1049)      683 2023-04-06 19:49:21.000000 synthea-rdf-0.1.4/dua/constants.py
+-rw-rw-r--   0 k163     (65010) k163      (1049)     6044 2023-04-23 01:11:11.000000 synthea-rdf-0.1.4/dua/generator.py
+-rw-rw-r--   0 k163     (65010) k163      (1049)     4954 2023-04-11 05:20:57.000000 synthea-rdf-0.1.4/dua/resource.py
+drwxrwxr-x   0 k163     (65010) k163      (1049)        0 2023-04-23 04:06:39.130283 synthea-rdf-0.1.4/generator_gui/
+-rw-rw-r--   0 k163     (65010) k163      (1049)     3137 2023-04-23 04:00:58.000000 synthea-rdf-0.1.4/generator_gui/dua_generator.py
+-rw-rw-r--   0 k163     (65010) k163      (1049)       38 2023-04-23 04:06:39.130283 synthea-rdf-0.1.4/setup.cfg
+-rw-rw-r--   0 k163     (65010) k163      (1049)      789 2023-04-23 04:05:05.000000 synthea-rdf-0.1.4/setup.py
+drwxrwxr-x   0 k163     (65010) k163      (1049)        0 2023-04-23 04:06:39.130283 synthea-rdf-0.1.4/synthea_ontology/
+-rw-rw-r--   0 k163     (65010) k163      (1049)   565508 2023-03-24 16:59:14.000000 synthea-rdf-0.1.4/synthea_ontology/synthea_ontology.png
+-rw-rw-r--   0 k163     (65010) k163      (1049)    71879 2023-03-24 16:59:14.000000 synthea-rdf-0.1.4/synthea_ontology/synthea_ontology.ttl
+drwxrwxr-x   0 k163     (65010) k163      (1049)        0 2023-04-23 04:06:39.130283 synthea-rdf-0.1.4/synthea_rdf/
+-rw-rw-r--   0 k163     (65010) k163      (1049)        0 2023-04-05 20:12:52.000000 synthea-rdf-0.1.4/synthea_rdf/__init__.py
+-rw-rw-r--   0 k163     (65010) k163      (1049)    13774 2023-04-21 04:57:51.000000 synthea-rdf-0.1.4/synthea_rdf/graph.py
+-rw-rw-r--   0 k163     (65010) k163      (1049)    40887 2023-04-22 00:58:58.000000 synthea-rdf-0.1.4/synthea_rdf/resource.py
+-rw-rw-r--   0 k163     (65010) k163      (1049)      152 2023-04-10 19:53:56.000000 synthea-rdf-0.1.4/synthea_rdf/settings.py
+drwxrwxr-x   0 k163     (65010) k163      (1049)        0 2023-04-23 04:06:39.130283 synthea-rdf-0.1.4/synthea_rdf.egg-info/
+-rw-rw-r--   0 k163     (65010) k163      (1049)     1990 2023-04-23 04:06:39.000000 synthea-rdf-0.1.4/synthea_rdf.egg-info/PKG-INFO
+-rw-rw-r--   0 k163     (65010) k163      (1049)      670 2023-04-23 04:06:39.000000 synthea-rdf-0.1.4/synthea_rdf.egg-info/SOURCES.txt
+-rw-rw-r--   0 k163     (65010) k163      (1049)        1 2023-04-23 04:06:39.000000 synthea-rdf-0.1.4/synthea_rdf.egg-info/dependency_links.txt
+-rw-rw-r--   0 k163     (65010) k163      (1049)       35 2023-04-23 04:06:39.000000 synthea-rdf-0.1.4/synthea_rdf.egg-info/requires.txt
+-rw-rw-r--   0 k163     (65010) k163      (1049)       36 2023-04-23 04:06:39.000000 synthea-rdf-0.1.4/synthea_rdf.egg-info/top_level.txt
+drwxrwxr-x   0 k163     (65010) k163      (1049)        0 2023-04-23 04:06:39.130283 synthea-rdf-0.1.4/tests/
+-rw-rw-r--   0 k163     (65010) k163      (1049)     3985 2023-03-24 16:59:14.000000 synthea-rdf-0.1.4/tests/test_convert.py
+drwxrwxr-x   0 k163     (65010) k163      (1049)        0 2023-04-23 04:06:39.130283 synthea-rdf-0.1.4/trustscore/
+-rw-rw-r--   0 k163     (65010) k163      (1049)        0 2023-04-06 06:09:53.000000 synthea-rdf-0.1.4/trustscore/__init__.py
+-rw-rw-r--   0 k163     (65010) k163      (1049)     5535 2023-04-11 01:51:24.000000 synthea-rdf-0.1.4/trustscore/generator.py
+-rw-rw-r--   0 k163     (65010) k163      (1049)     2637 2023-04-22 05:22:38.000000 synthea-rdf-0.1.4/trustscore/resource.py
```

### Comparing `synthea-rdf-0.1.3/LICENSE` & `synthea-rdf-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `synthea-rdf-0.1.3/PKG-INFO` & `synthea-rdf-0.1.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synthea-rdf
-Version: 0.1.3
+Version: 0.1.4
 Summary: Semantic web representation for the Synthea.
 Author: Dae-young Kim
 Author-email: leroy.kim@umbc.edu
 License: GPLv3
 Project-URL: Source Code, https://github.com/leroykim/synthea-rdf
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -23,15 +23,15 @@
 ### Installation
 ```bash
 pip install synthea-rdf
 ```
 
 ### Single CSV
 ```python
-from from pathlib import Path
+from pathlib import Path
 from synthea_rdf.graph import GraphBuilder
 
 MODEL_PATH = "./synthea_ontology/synthea_ontology.ttl"
 CSV_DIR = "./csv"
 DEST_PATH = "./result"
 
 builder = GraphBuilder(CSV_DIR, MODEL_PATH)
@@ -68,20 +68,7 @@
 CSV_DIR = "./csv"
 DEST_PATH = "./result"
 
 builder = GraphBuilder(CSV_DIR, MODEL_PATH)
 graph = builder.build()
 graph.serialize(destination=Path(DEST_PATH) / "all.ttl")
 ```
-
-## :warning: Issues
-- [ ] Confusing naming convention for the following data properties:
-
-        - syn:start
-        - syn:startDate
-        - syn:startDateTime
-        - syn:date
-        - syn:dateTime
-
-- [ ] There are no `Allergy` and `ImagingStudy` data in the test dataset. Testing required with a larger dataset.
-    - [ ] Test `Allergy`
-    - [ ] Test `ImagingStudy`
```

### Comparing `synthea-rdf-0.1.3/README.md` & `synthea-rdf-0.1.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ### Installation
 ```bash
 pip install synthea-rdf
 ```
 
 ### Single CSV
 ```python
-from from pathlib import Path
+from pathlib import Path
 from synthea_rdf.graph import GraphBuilder
 
 MODEL_PATH = "./synthea_ontology/synthea_ontology.ttl"
 CSV_DIR = "./csv"
 DEST_PATH = "./result"
 
 builder = GraphBuilder(CSV_DIR, MODEL_PATH)
@@ -54,20 +54,7 @@
 CSV_DIR = "./csv"
 DEST_PATH = "./result"
 
 builder = GraphBuilder(CSV_DIR, MODEL_PATH)
 graph = builder.build()
 graph.serialize(destination=Path(DEST_PATH) / "all.ttl")
 ```
-
-## :warning: Issues
-- [ ] Confusing naming convention for the following data properties:
-
-        - syn:start
-        - syn:startDate
-        - syn:startDateTime
-        - syn:date
-        - syn:dateTime
-
-- [ ] There are no `Allergy` and `ImagingStudy` data in the test dataset. Testing required with a larger dataset.
-    - [ ] Test `Allergy`
-    - [ ] Test `ImagingStudy`
```

### Comparing `synthea-rdf-0.1.3/setup.py` & `synthea-rdf-0.1.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from setuptools import setup
 
 setup(
     name="synthea-rdf",
-    version="0.1.3",
+    version="0.1.4",
     description="Semantic web representation for the Synthea.",
     author="Dae-young Kim",
     author_email="leroy.kim@umbc.edu",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     project_urls={"Source Code": "https://github.com/leroykim/synthea-rdf"},
     license="GPLv3",
-    packages=["synthea_rdf"],
+    packages=["synthea_rdf", "dua", "trustscore", "abstract"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
     ],  # Optional
     install_requires=[
         "rdflib",
         "pandas",
         "alive_progress",
+        "panel",
     ],
 )
```

### Comparing `synthea-rdf-0.1.3/synthea_ontology/synthea_ontology.png` & `synthea-rdf-0.1.4/synthea_ontology/synthea_ontology.png`

 * *Files identical despite different names*

### Comparing `synthea-rdf-0.1.3/synthea_ontology/synthea_ontology.ttl` & `synthea-rdf-0.1.4/synthea_ontology/synthea_ontology.ttl`

 * *Files identical despite different names*

### Comparing `synthea-rdf-0.1.3/synthea_rdf/literal.py` & `synthea-rdf-0.1.4/abstract/literal.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from rdflib import Literal
 from rdflib.namespace import RDF, XSD
 from datetime import datetime
-from .settings import SYN
+from abstract.namespace import SYN
 
 
+# Synthea Literals
 def dateLiteral(date):
     return Literal(datetime.strptime(date, "%Y-%m-%d"), datatype=XSD.dateTime)
 
 
 def dateTimeLiteral(date):
     return Literal(datetime.strptime(date, "%Y-%m-%dT%H:%M:%SZ"), datatype=XSD.dateTime)
```

### Comparing `synthea-rdf-0.1.3/synthea_rdf/resource.py` & `synthea-rdf-0.1.4/synthea_rdf/resource.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from abc import ABC, abstractmethod
 from rdflib.namespace import RDF
 from alive_progress import alive_bar
 import pandas as pd
-from .settings import SYN  # , TST
-from .literal import (
+from abstract import Resource
+from abstract.namespace import SYN
+from abstract.literal import (
     dateLiteral,
     dateTimeLiteral,
     dicomUidLiteral,
     dicomDcmLiteral,
     dicomSopLiteral,
     fdaUdiLiteral,
     floatLiteral,
@@ -15,15 +15,15 @@
     integerLiteral,
     loincLiteral,
     plainLiteral,
     snomedCtLiteral,
     umlsRxnormLiteral,
     urnUuidLiteral,
 )
-from .uri import (
+from abstract.uri import (
     allergyUri,
     carePlanUri,
     claimUri,
     claimTransactionUri,
     conditionUri,
     deviceUri,
     encounterUri,
@@ -39,34 +39,14 @@
     providerUri,
     supplyUri,
 )
 
 # from .trust import generate_user_trust, generate_org_trust, generate_veracity
 
 
-class Resource(ABC):
-    @abstractmethod
-    def __init__(self, df):
-        self.__resource_df = df
-
-    @property
-    @abstractmethod
-    def resource_df(self):
-        pass
-
-    @resource_df.setter
-    @abstractmethod
-    def resource_df(self, value):
-        pass
-
-    @abstractmethod
-    def convert(self, graph):
-        pass
-
-
 """
 Issue:
     - [ ] Confusing naming convention for the following data properties:
         - syn:start
         - syn:startDate
         - syn:startDateTime
         - syn:date
@@ -98,15 +78,16 @@
             for index, row in self.__resource_df.iterrows():
                 # Create name of the allergy class individual
                 allergy = allergyUri(index)
                 patient = patientUri(row["PATIENT"])
                 encounter = encounterUri(row["ENCOUNTER"])
 
                 # Data Properties
-                graph.add((allergy, SYN.start, dateLiteral(row["START"])))
+                graph.add((allergy, RDF.type, SYN.Allergy))
+                graph.add((allergy, SYN.startDate, dateLiteral(row["START"])))
                 graph.add((allergy, SYN.patientId, urnUuidLiteral(row["PATIENT"])))
                 graph.add((allergy, SYN.encounterId, urnUuidLiteral(row["ENCOUNTER"])))
                 graph.add((allergy, SYN.system, plainLiteral(row["SYSTEM"])))
                 graph.add((allergy, SYN.description, plainLiteral(row["DESCRIPTION"])))
 
                 # Object Properties
                 graph.add((allergy, SYN.isAbout, patient))
@@ -135,21 +116,30 @@
             for index, row in self.__resource_df.iterrows():
                 # Create name of the careplan class individual
                 careplan = carePlanUri(row["Id"])
                 patient = patientUri(row["PATIENT"])
                 encounter = encounterUri(row["ENCOUNTER"])
 
                 # Data Properties
+                graph.add((careplan, RDF.type, SYN.CarePlan))
                 graph.add((careplan, SYN.start, dateLiteral(row["START"])))
                 graph.add((careplan, SYN.patientId, urnUuidLiteral(row["PATIENT"])))
                 graph.add((careplan, SYN.encounterId, urnUuidLiteral(row["ENCOUNTER"])))
                 graph.add((careplan, SYN.code, snomedCtLiteral(row["CODE"])))
                 graph.add((careplan, SYN.description, plainLiteral(row["DESCRIPTION"])))
-                graph.add((careplan, SYN.reasonCode, snomedCtLiteral(row["REASONCODE"])))
-                graph.add((careplan, SYN.reasonDescription, plainLiteral(row["REASONDESCRIPTION"])))
+                graph.add(
+                    (careplan, SYN.reasonCode, snomedCtLiteral(row["REASONCODE"]))
+                )
+                graph.add(
+                    (
+                        careplan,
+                        SYN.reasonDescription,
+                        plainLiteral(row["REASONDESCRIPTION"]),
+                    )
+                )
 
                 # Object Properties
                 graph.add((careplan, SYN.isAbout, patient))
                 graph.add((patient, SYN.hasCarePlan, careplan))
                 graph.add((careplan, SYN.isOrderedDuring, encounter))
                 graph.add((encounter, SYN.hasOrdered, careplan))
 
@@ -178,20 +168,35 @@
             for index, row in self.__resource_df.iterrows():
                 # Create name of the claim class individual
                 claim = claimUri(row["Id"])
                 patient = patientUri(row["PATIENTID"])
                 provider = providerUri(row["PROVIDERID"])
 
                 # Data Properties
+                graph.add((claim, RDF.type, SYN.Claim))
                 graph.add((claim, SYN.id, urnUuidLiteral(row["Id"])))
                 graph.add((claim, SYN.patientId, urnUuidLiteral(row["PATIENTID"])))
                 graph.add((claim, SYN.providerId, urnUuidLiteral(row["PROVIDERID"])))
-                graph.add((claim, SYN.departmentId, urnUuidLiteral(row["DEPARTMENTID"])))
-                graph.add((claim, SYN.patientDepartmentId, urnUuidLiteral(row["PATIENTDEPARTMENTID"])))
-                graph.add((claim, SYN.currentIllnessDate, dateTimeLiteral(row["CURRENTILLNESSDATE"])))
+                graph.add(
+                    (claim, SYN.departmentId, urnUuidLiteral(row["DEPARTMENTID"]))
+                )
+                graph.add(
+                    (
+                        claim,
+                        SYN.patientDepartmentId,
+                        urnUuidLiteral(row["PATIENTDEPARTMENTID"]),
+                    )
+                )
+                graph.add(
+                    (
+                        claim,
+                        SYN.currentIllnessDate,
+                        dateTimeLiteral(row["CURRENTILLNESSDATE"]),
+                    )
+                )
                 graph.add((claim, SYN.serviceDate, dateTimeLiteral(row["SERVICEDATE"])))
 
                 # Object Properties
                 graph.add((claim, SYN.isAssociatedWith, patient))
                 graph.add((patient, SYN.hasClaim, claim))
                 graph.add((claim, SYN.isFiledBy, provider))
                 graph.add((provider, SYN.hasFiled, claim))
@@ -209,32 +214,59 @@
 
     @resource_df.setter
     def resource_df(self, value):
         self.__resource_df = value
 
     def convert(self, graph):
         rows = self.__resource_df.shape[0]
-        with alive_bar(rows, force_tty=True, title="ClaimTransaction Conversion") as bar:
+        with alive_bar(
+            rows, force_tty=True, title="ClaimTransaction Conversion"
+        ) as bar:
             for index, row in self.__resource_df.iterrows():
                 # Create name of the claimtransaction class individual
                 claimtransaction = claimTransactionUri(row["ID"])
                 claim = claimUri(row["CLAIMID"])
                 patient = patientUri(row["PATIENTID"])
                 provider = providerUri(row["PROVIDERID"])
                 organization = organizationUri(row["PLACEOFSERVICE"])
 
                 # Data Properties
+                graph.add((claimtransaction, RDF.type, SYN.ClaimTransaction))
                 graph.add((claimtransaction, SYN.id, urnUuidLiteral(row["ID"])))
-                graph.add((claimtransaction, SYN.claimId, urnUuidLiteral(row["CLAIMID"])))
-                graph.add((claimtransaction, SYN.chargeId, urnUuidLiteral(row["CHARGEID"])))
-                graph.add((claimtransaction, SYN.patientId, urnUuidLiteral(row["PATIENTID"])))
+                graph.add(
+                    (claimtransaction, SYN.claimId, urnUuidLiteral(row["CLAIMID"]))
+                )
+                graph.add(
+                    (claimtransaction, SYN.chargeId, urnUuidLiteral(row["CHARGEID"]))
+                )
+                graph.add(
+                    (claimtransaction, SYN.patientId, urnUuidLiteral(row["PATIENTID"]))
+                )
                 graph.add((claimtransaction, SYN.type, plainLiteral(row["TYPE"])))
-                graph.add((claimtransaction, SYN.placeOfService, urnUuidLiteral(row["PLACEOFSERVICE"])))
-                graph.add((claimtransaction, SYN.procedureCode, snomedCtLiteral(row["PROCEDURECODE"])))
-                graph.add((claimtransaction, SYN.providerId, urnUuidLiteral(row["PROVIDERID"])))
+                graph.add(
+                    (
+                        claimtransaction,
+                        SYN.placeOfService,
+                        urnUuidLiteral(row["PLACEOFSERVICE"]),
+                    )
+                )
+                graph.add(
+                    (
+                        claimtransaction,
+                        SYN.procedureCode,
+                        snomedCtLiteral(row["PROCEDURECODE"]),
+                    )
+                )
+                graph.add(
+                    (
+                        claimtransaction,
+                        SYN.providerId,
+                        urnUuidLiteral(row["PROVIDERID"]),
+                    )
+                )
 
                 # Object Properties
                 graph.add((claimtransaction, SYN.isTransactionFor, claim))
                 graph.add((claim, SYN.hasTransaction, claimtransaction))
                 graph.add((claimtransaction, SYN.isAssociatedWith, patient))
                 graph.add((patient, SYN.hasClaimTransaction, claimtransaction))
                 graph.add((claimtransaction, SYN.isAssociatedWith, provider))
@@ -263,19 +295,24 @@
             for index, row in self.__resource_df.iterrows():
                 # Create name of the condition class individual
                 condition = conditionUri(index)
                 patient = patientUri(row["PATIENT"])
                 encounter = encounterUri(row["ENCOUNTER"])
 
                 # Data Properties
+                graph.add((condition, RDF.type, SYN.Condition))
                 graph.add((condition, SYN.startDate, dateLiteral(row["START"])))
                 graph.add((condition, SYN.patientId, urnUuidLiteral(row["PATIENT"])))
-                graph.add((condition, SYN.encounterId, urnUuidLiteral(row["ENCOUNTER"])))
+                graph.add(
+                    (condition, SYN.encounterId, urnUuidLiteral(row["ENCOUNTER"]))
+                )
                 graph.add((condition, SYN.code, snomedCtLiteral(row["CODE"])))
-                graph.add((condition, SYN.description, plainLiteral(row["DESCRIPTION"])))
+                graph.add(
+                    (condition, SYN.description, plainLiteral(row["DESCRIPTION"]))
+                )
 
                 # Object Properties
                 graph.add((condition, SYN.isAbout, patient))
                 graph.add((patient, SYN.hasHistoryOf, condition))
                 graph.add((condition, SYN.isDiagnosedDuring, encounter))
                 graph.add((encounter, SYN.hasDiagnosed, condition))
 
@@ -300,14 +337,15 @@
             for index, row in self.__resource_df.iterrows():
                 # Create name of the device class individual
                 device = deviceUri(index)
                 patient = patientUri(row["PATIENT"])
                 encounter = encounterUri(row["ENCOUNTER"])
 
                 # Data Properties
+                graph.add((device, RDF.type, SYN.Device))
                 graph.add((device, SYN.startDateTime, dateTimeLiteral(row["START"])))
                 graph.add((device, SYN.patientId, urnUuidLiteral(row["PATIENT"])))
                 graph.add((device, SYN.encounterId, urnUuidLiteral(row["ENCOUNTER"])))
                 graph.add((device, SYN.code, snomedCtLiteral(row["CODE"])))
                 graph.add((device, SYN.description, plainLiteral(row["DESCRIPTION"])))
                 graph.add((device, SYN.udi, fdaUdiLiteral(row["UDI"])))
 
@@ -329,31 +367,14 @@
         return self.__resource_df
 
     @resource_df.setter
     def resource_df(self, value):
         self.__resource_df = value
 
     def convert(self, graph):
-        """
-        Object properties covered by other resource conversion:
-            - syn:hasOrdered
-                - [x] syn:CarePlan
-                - [x] syn:Device
-                - [x] syn:Procedure
-                - [x] syn:Supply
-                - [x] syn:ImagingStudy
-                - [ ] syn:Observation
-            - syn:hasDiagnosed
-                - [x] syn:Condition
-                - [x] syn:Allergy
-            - syn:hasPrescribed
-                - [x] syn:Immunization
-                - [x] syn:Medication
-
-        """
         rows = self.__resource_df.shape[0]
         # veracity = generate_veracity(rows)
         with alive_bar(rows, force_tty=True, title="Encounter Conversion") as bar:
             for index, row in self.__resource_df.iterrows():
                 # Create name of the encounter class individual
                 encounter = encounterUri(row["Id"])
                 organization = organizationUri(row["ORGANIZATION"])
@@ -362,53 +383,61 @@
                 payer = payerUri(row["PAYER"])
 
                 # Data Properties
                 graph.add((encounter, RDF.type, SYN.Encounter))
                 graph.add((encounter, SYN.id, urnUuidLiteral(row["Id"])))
                 graph.add((encounter, SYN.startDateTime, dateTimeLiteral(row["START"])))
                 graph.add((encounter, SYN.patientId, urnUuidLiteral(row["PATIENT"])))
-                graph.add((encounter, SYN.organizationId, urnUuidLiteral(row["ORGANIZATION"])))
+                graph.add(
+                    (encounter, SYN.organizationId, urnUuidLiteral(row["ORGANIZATION"]))
+                )
                 graph.add((encounter, SYN.providerId, urnUuidLiteral(row["PROVIDER"])))
                 graph.add((encounter, SYN.payerId, urnUuidLiteral(row["PAYER"])))
-                graph.add((encounter, SYN.encounterClass, plainLiteral(row["ENCOUNTERCLASS"])))
+                graph.add(
+                    (encounter, SYN.encounterClass, plainLiteral(row["ENCOUNTERCLASS"]))
+                )
                 graph.add((encounter, SYN.code, snomedCtLiteral(row["CODE"])))
-                graph.add((encounter, SYN.description, plainLiteral(row["DESCRIPTION"])))
-                graph.add((encounter, SYN.baseEncounterCost, floatLiteral(row["BASE_ENCOUNTER_COST"])))
-                graph.add((encounter, SYN.totalClaimCost, floatLiteral(row["TOTAL_CLAIM_COST"])))
-                graph.add((encounter, SYN.payerCoverage, floatLiteral(row["PAYER_COVERAGE"])))
+                graph.add(
+                    (encounter, SYN.description, plainLiteral(row["DESCRIPTION"]))
+                )
+                graph.add(
+                    (
+                        encounter,
+                        SYN.baseEncounterCost,
+                        floatLiteral(row["BASE_ENCOUNTER_COST"]),
+                    )
+                )
+                graph.add(
+                    (
+                        encounter,
+                        SYN.totalClaimCost,
+                        floatLiteral(row["TOTAL_CLAIM_COST"]),
+                    )
+                )
+                graph.add(
+                    (encounter, SYN.payerCoverage, floatLiteral(row["PAYER_COVERAGE"]))
+                )
 
                 # Object Properties
                 graph.add((encounter, SYN.hasPatient, patient))
                 graph.add((encounter, SYN.isPerformedAt, organization))
                 graph.add((encounter, SYN.isPerformedBy, provider))
                 graph.add((provider, SYN.hasPerformed, encounter))
                 graph.add((encounter, SYN.isCoveredBy, payer))
 
-                # Veracity
-                # graph.add(
-                #     (
-                #         encounter,
-                #         TST.credibility,
-                #         float_literal(veracity.iloc[index]["credibility"]),
-                #     )
-                # )
-                # graph.add(
-                #     (
-                #         encounter,
-                #         TST.objectivity,
-                #         float_literal(veracity.iloc[index]["objectivity"]),
-                #     )
-                # )
-                # graph.add(
-                #     (
-                #         encounter,
-                #         TST.trustfulness,
-                #         float_literal(veracity.iloc[index]["trustfulness"]),
-                #     )
-                # )
+                graph.add(
+                    (encounter, SYN.reasonCode, snomedCtLiteral(row["REASONCODE"]))
+                )
+                graph.add(
+                    (
+                        encounter,
+                        SYN.reasonDescription,
+                        plainLiteral(row["REASONDESCRIPTION"]),
+                    )
+                )
 
                 bar()
 
 
 class ImagingStudy(Resource):
     def __init__(self, df):
         self.__resource_df = df
@@ -432,27 +461,74 @@
             for index, row in self.__resource_df.iterrows():
                 # Create name of the imagingstudy class individual
                 imagingstudy = imagingStudyUri(index)
                 patient = patientUri(row["PATIENT"])
                 encounter = encounterUri(row["ENCOUNTER"])
 
                 # Data Properties
+                graph.add((imagingstudy, RDF.type, SYN.ImagingStudy))
                 graph.add((imagingstudy, SYN.id, urnUuidLiteral(row["Id"])))
                 graph.add((imagingstudy, SYN.dateTime, dateTimeLiteral(row["DATE"])))
                 graph.add((imagingstudy, SYN.patientId, urnUuidLiteral(row["PATIENT"])))
-                graph.add((imagingstudy, SYN.encounterId, urnUuidLiteral(row["ENCOUNTER"])))
-                graph.add((imagingstudy, SYN.seriesUid, dicomUidLiteral(row["SERIES_UID"])))
-                graph.add((imagingstudy, SYN.bodySiteCode, snomedCtLiteral(row["BODYSITE_CODE"])))
-                graph.add((imagingstudy, SYN.bodySiteDescription, plainLiteral(row["BODYSITE_DESCRIPTION"])))
-                graph.add((imagingstudy, SYN.modalityCode, dicomDcmLiteral(row["MODALITY_CODE"])))
-                graph.add((imagingstudy, SYN.modalityDescription, plainLiteral(row["MODALITY_DESCRIPTION"])))
-                graph.add((imagingstudy, SYN.instanceUid, dicomUidLiteral(row["INSTANCE_UID"])))
+                graph.add(
+                    (imagingstudy, SYN.encounterId, urnUuidLiteral(row["ENCOUNTER"]))
+                )
+                graph.add(
+                    (imagingstudy, SYN.seriesUid, dicomUidLiteral(row["SERIES_UID"]))
+                )
+                graph.add(
+                    (
+                        imagingstudy,
+                        SYN.bodySiteCode,
+                        snomedCtLiteral(row["BODYSITE_CODE"]),
+                    )
+                )
+                graph.add(
+                    (
+                        imagingstudy,
+                        SYN.bodySiteDescription,
+                        plainLiteral(row["BODYSITE_DESCRIPTION"]),
+                    )
+                )
+                graph.add(
+                    (
+                        imagingstudy,
+                        SYN.modalityCode,
+                        dicomDcmLiteral(row["MODALITY_CODE"]),
+                    )
+                )
+                graph.add(
+                    (
+                        imagingstudy,
+                        SYN.modalityDescription,
+                        plainLiteral(row["MODALITY_DESCRIPTION"]),
+                    )
+                )
+                graph.add(
+                    (
+                        imagingstudy,
+                        SYN.instanceUid,
+                        dicomUidLiteral(row["INSTANCE_UID"]),
+                    )
+                )
                 graph.add((imagingstudy, SYN.sopCode, dicomSopLiteral(row["SOP_CODE"])))
-                graph.add((imagingstudy, SYN.sopDescription, plainLiteral(row["SOP_DESCRIPTION"])))
-                graph.add((imagingstudy, SYN.procedureCode, snomedCtLiteral(row["PROCEDURE_CODE"])))
+                graph.add(
+                    (
+                        imagingstudy,
+                        SYN.sopDescription,
+                        plainLiteral(row["SOP_DESCRIPTION"]),
+                    )
+                )
+                graph.add(
+                    (
+                        imagingstudy,
+                        SYN.procedureCode,
+                        snomedCtLiteral(row["PROCEDURE_CODE"]),
+                    )
+                )
 
                 # Object Properties
                 graph.add((imagingstudy, SYN.isAbout, patient))
                 graph.add((patient, SYN.hasHistoryOf, imagingstudy))
                 graph.add((imagingstudy, SYN.isOrderedDuring, encounter))
                 graph.add((encounter, SYN.hasOrdered, imagingstudy))
 
@@ -477,19 +553,24 @@
             for index, row in self.__resource_df.iterrows():
                 # Create name of the immunization class individual
                 immunization = immunizationUri(index)
                 patient = patientUri(row["PATIENT"])
                 encounter = encounterUri(row["ENCOUNTER"])
 
                 # Data Properties
+                graph.add((immunization, RDF.type, SYN.Immunization))
                 graph.add((immunization, SYN.dateTime, dateTimeLiteral(row["DATE"])))
                 graph.add((immunization, SYN.patientId, urnUuidLiteral(row["PATIENT"])))
-                graph.add((immunization, SYN.encounterId, urnUuidLiteral(row["ENCOUNTER"])))
+                graph.add(
+                    (immunization, SYN.encounterId, urnUuidLiteral(row["ENCOUNTER"]))
+                )
                 graph.add((immunization, SYN.code, hl7CvxLiteral(row["CODE"])))
-                graph.add((immunization, SYN.description, plainLiteral(row["DESCRIPTION"])))
+                graph.add(
+                    (immunization, SYN.description, plainLiteral(row["DESCRIPTION"]))
+                )
                 graph.add((immunization, SYN.cost, floatLiteral(row["BASE_COST"])))
 
                 # Object Properties
                 graph.add((immunization, SYN.isPrescribedFor, patient))
                 graph.add((patient, SYN.hasHistoryOf, immunization))
                 graph.add((immunization, SYN.isPrescribedDuring, encounter))
                 graph.add((encounter, SYN.hasPrescribed, immunization))
@@ -516,22 +597,31 @@
                 # Create name of the medication class individual
                 medication = medicationUri(index)
                 patient = patientUri(row["PATIENT"])
                 encounter = encounterUri(row["ENCOUNTER"])
                 payer = payerUri(row["PAYER"])
 
                 # Data Properties
-                graph.add((medication, SYN.startDateTime, dateTimeLiteral(row["START"])))
+                graph.add((medication, RDF.type, SYN.Medication))
+                graph.add(
+                    (medication, SYN.startDateTime, dateTimeLiteral(row["START"]))
+                )
                 graph.add((medication, SYN.patientId, urnUuidLiteral(row["PATIENT"])))
                 graph.add((medication, SYN.payerId, urnUuidLiteral(row["PAYER"])))
-                graph.add((medication, SYN.encounterId, urnUuidLiteral(row["ENCOUNTER"])))
+                graph.add(
+                    (medication, SYN.encounterId, urnUuidLiteral(row["ENCOUNTER"]))
+                )
                 graph.add((medication, SYN.code, umlsRxnormLiteral(row["CODE"])))
-                graph.add((medication, SYN.description, plainLiteral(row["DESCRIPTION"])))
+                graph.add(
+                    (medication, SYN.description, plainLiteral(row["DESCRIPTION"]))
+                )
                 graph.add((medication, SYN.baseCost, floatLiteral(row["BASE_COST"])))
-                graph.add((medication, SYN.payerCoverage, floatLiteral(row["PAYER_COVERAGE"])))
+                graph.add(
+                    (medication, SYN.payerCoverage, floatLiteral(row["PAYER_COVERAGE"]))
+                )
                 graph.add((medication, SYN.dispense, floatLiteral(row["DISPENSES"])))
                 graph.add((medication, SYN.totalCost, floatLiteral(row["TOTALCOST"])))
 
                 # Object Properties
                 graph.add((medication, SYN.isPrescribedFor, patient))
                 graph.add((patient, SYN.hasHistoryOf, medication))
                 graph.add((medication, SYN.isPrescribedDuring, encounter))
@@ -539,20 +629,14 @@
                 graph.add((payer, SYN.hasCovered, medication))
                 graph.add((medication, SYN.isCoveredBy, payer))
 
                 bar()
 
 
 class Observation(Resource):
-    """
-    Object properties covered by other resource conversion:
-        - [ ] syn:Patient syn:hasHistoryOf syn:Observation
-        - [ ] syn:Encounter syn:hasOrdered syn:Observation
-    """
-
     def __init__(self, df):
         self.__resource_df = df
 
     @property
     def resource_df(self):
         return self.__resource_df
 
@@ -569,48 +653,35 @@
                 observation = observationUri(index)
 
                 # Data Properties
                 graph.add((observation, RDF.type, SYN.Observation))
                 graph.add((observation, SYN.dateTime, dateTimeLiteral(row["DATE"])))
                 graph.add((observation, SYN.patientId, urnUuidLiteral(row["PATIENT"])))
                 if pd.notnull(row["ENCOUNTER"]):
-                    graph.add((observation, SYN.encounterId, urnUuidLiteral(row["ENCOUNTER"])))
+                    graph.add(
+                        (observation, SYN.encounterId, urnUuidLiteral(row["ENCOUNTER"]))
+                    )
                 graph.add((observation, SYN.code, loincLiteral(row["CODE"])))
-                graph.add((observation, SYN.description, plainLiteral(row["DESCRIPTION"])))
+                graph.add(
+                    (observation, SYN.description, plainLiteral(row["DESCRIPTION"]))
+                )
                 graph.add((observation, SYN.value, plainLiteral(row["VALUE"])))
                 graph.add((observation, SYN.type, plainLiteral(row["TYPE"])))
 
                 # Object Properties
                 if pd.notnull(row["ENCOUNTER"]):
-                    graph.add((observation, SYN.isOrderedDuring, encounterUri(row["ENCOUNTER"])))
+                    graph.add(
+                        (
+                            observation,
+                            SYN.isOrderedDuring,
+                            encounterUri(row["ENCOUNTER"]),
+                        )
+                    )
                 graph.add((observation, SYN.isAbout, patientUri(row["PATIENT"])))
 
-                # Veracity
-                # graph.add(
-                #     (
-                #         observation,
-                #         TST.credibility,
-                #         float_literal(veracity.iloc[index]["credibility"]),
-                #     )
-                # )
-                # graph.add(
-                #     (
-                #         observation,
-                #         TST.objectivity,
-                #         float_literal(veracity.iloc[index]["objectivity"]),
-                #     )
-                # )
-                # graph.add(
-                #     (
-                #         observation,
-                #         TST.trustfulness,
-                #         float_literal(veracity.iloc[index]["trustfulness"]),
-                #     )
-                # )
-
                 bar()
 
 
 class Organization(Resource):
     # This class use TRUST_IRI for now.
     def __init__(self, df):
         self.__resource_df = df
@@ -640,26 +711,17 @@
                 # Data Properties
                 graph.add((organization, RDF.type, SYN.Organization))
                 graph.add((organization, SYN.id, urnUuidLiteral(row["Id"])))
                 graph.add((organization, SYN.name, plainLiteral(row["NAME"])))
                 graph.add((organization, SYN.address, plainLiteral(row["ADDRESS"])))
                 graph.add((organization, SYN.city, plainLiteral(row["CITY"])))
                 graph.add((organization, SYN.revenue, floatLiteral(row["REVENUE"])))
-                graph.add((organization, SYN.utilization, integerLiteral(row["UTILIZATION"])))
-
-                # Object Properties
-
-                # Reputation
-                # graph.add(
-                #     (
-                #         organization,
-                #         TST.reputation,
-                #         float_literal(reputation.iloc[index]["reputation"]),
-                #     )
-                # )
+                graph.add(
+                    (organization, SYN.utilization, integerLiteral(row["UTILIZATION"]))
+                )
 
                 bar()
 
 
 class Patient(Resource):
     def __init__(self, df):
         self.__resource_df = df
@@ -669,73 +731,53 @@
         return self.__resource_df
 
     @resource_df.setter
     def resource_df(self, value):
         self.__resource_df = value
 
     def convert(self, graph):
-        """
-        Object properties covered by other resource conversion:
-            - [x] syn:Patient syn:hasAllergy syn:Allergy
-            - syn:Patient syn:hasHistoryOf
-                - [ ] syn:Observation
-                - [x] syn:Condition
-                - [x] syn:Procedure
-                - [x] syn:Medication
-                - [x] syn:Immunization
-                - [x] syn:ImagingStudy
-                - [x] syn:Supply
-            - [x] syn:Patient syn:isMeasuredBy syn:Device
-            - [x] syn:Patient syn:hasCarePlan syn:CarePlan
-            - [ ] syn:Patient syn:hasEncounter syn:Encounter
-            - [x] syn:Patient syn:hasClaim syn:Claim
-            - [x] syn:Patient syn:hasClaimTransaction syn:ClaimTransaction
-            - [x] syn:Patient syn:hasPayerTransitionHistory syn:PayerTransition
-        """
         rows = self.__resource_df.shape[0]
         # user_trust = generate_user_trust(rows)
         with alive_bar(rows, force_tty=True, title="Patient Conversion") as bar:
             for index, row in self.__resource_df.iterrows():
                 # Create name of the patient class individual
                 patient = patientUri(row["Id"])
 
                 # Data Properties
-                # graph.add((patient, RDF.type, SYN.Patient))  # type
+                graph.add((patient, RDF.type, SYN.Patient))  # type
                 graph.add((patient, SYN.id, urnUuidLiteral(row["Id"])))  # id
-                graph.add((patient, SYN.birthdate, dateLiteral(row["BIRTHDATE"])))  # birthdate
+                graph.add(
+                    (patient, SYN.birthdate, dateLiteral(row["BIRTHDATE"]))
+                )  # birthdate
                 graph.add((patient, SYN.ssn, plainLiteral(row["SSN"])))  # ssn
                 graph.add((patient, SYN.first, plainLiteral(row["FIRST"])))
                 graph.add((patient, SYN.last, plainLiteral(row["LAST"])))
                 graph.add((patient, SYN.race, plainLiteral(row["RACE"])))
                 graph.add((patient, SYN.ethnicity, plainLiteral(row["ETHNICITY"])))
                 graph.add((patient, SYN.gender, plainLiteral(row["GENDER"])))
                 graph.add((patient, SYN.birthplace, plainLiteral(row["BIRTHPLACE"])))
                 graph.add((patient, SYN.address, plainLiteral(row["ADDRESS"])))
                 graph.add((patient, SYN.city, plainLiteral(row["CITY"])))
                 graph.add((patient, SYN.state, plainLiteral(row["STATE"])))
-                graph.add((patient, SYN.healthcareExpense, plainLiteral(row["HEALTHCARE_EXPENSES"])))
-                graph.add((patient, SYN.healthcareCoverage, plainLiteral(row["HEALTHCARE_COVERAGE"])))
+                graph.add(
+                    (
+                        patient,
+                        SYN.healthcareExpense,
+                        plainLiteral(row["HEALTHCARE_EXPENSES"]),
+                    )
+                )
+                graph.add(
+                    (
+                        patient,
+                        SYN.healthcareCoverage,
+                        plainLiteral(row["HEALTHCARE_COVERAGE"]),
+                    )
+                )
                 graph.add((patient, SYN.income, integerLiteral(row["INCOME"])))
 
-                # User Trust
-                # graph.add(
-                #     (
-                #         patient,
-                #         TST.behavior,
-                #         float_literal(user_trust.iloc[index]["behavioral_trust"]),
-                #     )
-                # )
-                # graph.add(
-                #     (
-                #         patient,
-                #         TST.identity,
-                #         float_literal(user_trust.iloc[index]["identity_trust"]),
-                #     )
-                # )
-
                 bar()
 
 
 class Payer(Resource):
     def __init__(self, df):
         self.__resource_df = df
 
@@ -758,49 +800,91 @@
         # user_trust = generate_user_trust(rows)
         with alive_bar(rows, force_tty=True, title="Payer Conversion") as bar:
             for index, row in self.__resource_df.iterrows():
                 # Create name of the payer class individual
                 payer = payerUri(row["Id"])
 
                 # Data Properties
-                # graph.add((payer, RDF.type, SYN.Payer))  # type
+                graph.add((payer, RDF.type, SYN.Payer))  # type
                 graph.add((payer, SYN.id, urnUuidLiteral(row["Id"])))  # id
                 graph.add((payer, SYN.name, plainLiteral(row["NAME"])))
-                graph.add((payer, SYN.amountCovered, floatLiteral(row["AMOUNT_COVERED"])))
-                graph.add((payer, SYN.amountUncovered, floatLiteral(row["AMOUNT_UNCOVERED"])))
+                graph.add(
+                    (payer, SYN.amountCovered, floatLiteral(row["AMOUNT_COVERED"]))
+                )
+                graph.add(
+                    (payer, SYN.amountUncovered, floatLiteral(row["AMOUNT_UNCOVERED"]))
+                )
                 graph.add((payer, SYN.revenue, floatLiteral(row["REVENUE"])))
-                graph.add((payer, SYN.coveredEncounters, integerLiteral(row["COVERED_ENCOUNTERS"])))
-                graph.add((payer, SYN.uncoveredEncounters, integerLiteral(row["UNCOVERED_ENCOUNTERS"])))
-                graph.add((payer, SYN.coveredMedications, integerLiteral(row["COVERED_MEDICATIONS"])))
-                graph.add((payer, SYN.uncoveredMedications, integerLiteral(row["UNCOVERED_MEDICATIONS"])))
-                graph.add((payer, SYN.coveredProcedures, integerLiteral(row["COVERED_PROCEDURES"])))
-                graph.add((payer, SYN.uncoveredProcedures, integerLiteral(row["UNCOVERED_PROCEDURES"])))
-                graph.add((payer, SYN.coveredImmunizations, integerLiteral(row["COVERED_IMMUNIZATIONS"])))
-                graph.add((payer, SYN.uncoveredImmunizations, integerLiteral(row["UNCOVERED_IMMUNIZATIONS"])))
-                graph.add((payer, SYN.uniqueCustomers, integerLiteral(row["UNIQUE_CUSTOMERS"])))
+                graph.add(
+                    (
+                        payer,
+                        SYN.coveredEncounters,
+                        integerLiteral(row["COVERED_ENCOUNTERS"]),
+                    )
+                )
+                graph.add(
+                    (
+                        payer,
+                        SYN.uncoveredEncounters,
+                        integerLiteral(row["UNCOVERED_ENCOUNTERS"]),
+                    )
+                )
+                graph.add(
+                    (
+                        payer,
+                        SYN.coveredMedications,
+                        integerLiteral(row["COVERED_MEDICATIONS"]),
+                    )
+                )
+                graph.add(
+                    (
+                        payer,
+                        SYN.uncoveredMedications,
+                        integerLiteral(row["UNCOVERED_MEDICATIONS"]),
+                    )
+                )
+                graph.add(
+                    (
+                        payer,
+                        SYN.coveredProcedures,
+                        integerLiteral(row["COVERED_PROCEDURES"]),
+                    )
+                )
+                graph.add(
+                    (
+                        payer,
+                        SYN.uncoveredProcedures,
+                        integerLiteral(row["UNCOVERED_PROCEDURES"]),
+                    )
+                )
+                graph.add(
+                    (
+                        payer,
+                        SYN.coveredImmunizations,
+                        integerLiteral(row["COVERED_IMMUNIZATIONS"]),
+                    )
+                )
+                graph.add(
+                    (
+                        payer,
+                        SYN.uncoveredImmunizations,
+                        integerLiteral(row["UNCOVERED_IMMUNIZATIONS"]),
+                    )
+                )
+                graph.add(
+                    (
+                        payer,
+                        SYN.uniqueCustomers,
+                        integerLiteral(row["UNIQUE_CUSTOMERS"]),
+                    )
+                )
                 graph.add((payer, SYN.qolsAvg, floatLiteral(row["QOLS_AVG"])))
-                graph.add((payer, SYN.memberMonths, integerLiteral(row["MEMBER_MONTHS"])))
-
-                # Object Properties
-
-                # User Trust
-                # graph.add(
-                #     (
-                #         payer,
-                #         TST.behavior,
-                #         float_literal(user_trust.iloc[index]["behavioral_trust"]),
-                #     )
-                # )
-                # graph.add(
-                #     (
-                #         payer,
-                #         TST.identity,
-                #         float_literal(user_trust.iloc[index]["identity_trust"]),
-                #     )
-                # )
+                graph.add(
+                    (payer, SYN.memberMonths, integerLiteral(row["MEMBER_MONTHS"]))
+                )
 
                 bar()
 
 
 class PayerTransition(Resource):
     def __init__(self, df):
         self.__resource_df = df
@@ -811,25 +895,38 @@
 
     @resource_df.setter
     def resource_df(self, value):
         self.__resource_df = value
 
     def convert(self, graph):
         rows = self.__resource_df.shape[0]
-        with alive_bar(rows, force_tty=True, title="Payer Transition Conversion") as bar:
+        with alive_bar(
+            rows, force_tty=True, title="Payer Transition Conversion"
+        ) as bar:
             for index, row in self.__resource_df.iterrows():
                 # Create name of the payertransition class individual
                 payertransition = payertransitionUri(index)
                 patient = patientUri(row["PATIENT"])
                 payer = payerUri(row["PAYER"])
 
                 # Data Properties
-                graph.add((payertransition, SYN.patientId, urnUuidLiteral(row["PATIENT"])))
-                graph.add((payertransition, SYN.startYear, dateLiteral(row["START_YEAR"][:10])))
-                graph.add((payertransition, SYN.endYear, dateLiteral(row["END_YEAR"][:10])))
+                graph.add((payertransition, RDF.type, SYN.PayerTransition))  # type
+                graph.add(
+                    (payertransition, SYN.patientId, urnUuidLiteral(row["PATIENT"]))
+                )
+                graph.add(
+                    (
+                        payertransition,
+                        SYN.startYear,
+                        dateLiteral(row["START_YEAR"][:10]),
+                    )
+                )
+                graph.add(
+                    (payertransition, SYN.endYear, dateLiteral(row["END_YEAR"][:10]))
+                )
                 graph.add((payertransition, SYN.payerId, urnUuidLiteral(row["PAYER"])))
 
                 # Object Properties
                 graph.add((payertransition, SYN.hasPatientRecord, patient))
                 graph.add((patient, SYN.hasPayerTransitionHistory, payertransition))
                 graph.add((payertransition, SYN.hasPayerRecord, payer))
                 graph.add((payer, SYN.hasPayerTransitionHistory, payertransition))
@@ -855,19 +952,24 @@
             for index, row in self.__resource_df.iterrows():
                 # Create name of the procedure class individual
                 procedure = procedureUri(index)
                 patient = patientUri(row["PATIENT"])
                 encounter = encounterUri(row["ENCOUNTER"])
 
                 # Data Properties
+                graph.add((procedure, RDF.type, SYN.Procedure))  # type
                 graph.add((procedure, SYN.startDateTime, dateTimeLiteral(row["START"])))
                 graph.add((procedure, SYN.patientId, urnUuidLiteral(row["PATIENT"])))
-                graph.add((procedure, SYN.encounterId, urnUuidLiteral(row["ENCOUNTER"])))
+                graph.add(
+                    (procedure, SYN.encounterId, urnUuidLiteral(row["ENCOUNTER"]))
+                )
                 graph.add((procedure, SYN.code, snomedCtLiteral(row["CODE"])))
-                graph.add((procedure, SYN.description, plainLiteral(row["DESCRIPTION"])))
+                graph.add(
+                    (procedure, SYN.description, plainLiteral(row["DESCRIPTION"]))
+                )
                 graph.add((procedure, SYN.baseCost, floatLiteral(row["BASE_COST"])))
 
                 # Object Properties
                 graph.add((procedure, SYN.isOrderedFor, patient))
                 graph.add((patient, SYN.hasHistoryOf, procedure))
                 graph.add((procedure, SYN.isOrderedDuring, encounter))
                 graph.add((encounter, SYN.hasOrdered, procedure))
@@ -884,59 +986,49 @@
         return self.__resource_df
 
     @resource_df.setter
     def resource_df(self, value):
         self.__resource_df = value
 
     def convert(self, graph):
-        """
-        Object properties covered by other resource conversion:
-            - [x] syn:Provider syn:hasPerformed syn:Encounter
-            - [x] syn:Provider syn:hasClaimTransaction syn:ClaimTransaction
-            - [x] syn:Provider syn:hasFiled syn:Claim
-        """
         rows = self.__resource_df.shape[0]
         # user_trust = generate_user_trust(rows)
         with alive_bar(rows, force_tty=True, title="Provider Conversion") as bar:
             for index, row in self.__resource_df.iterrows():
                 # Create name of the provider class individual
                 provider = providerUri(row["Id"])
-                organization = organizationUri(row["ORGANIZATION"])  # for object property
+                organization = organizationUri(
+                    row["ORGANIZATION"]
+                )  # for object property
 
                 # Data Properties
                 graph.add((provider, RDF.type, SYN.Provider))
                 graph.add((provider, SYN.id, urnUuidLiteral(row["Id"])))
-                graph.add((provider, SYN.organizationId, urnUuidLiteral(row["ORGANIZATION"])))
+                graph.add(
+                    (provider, SYN.organizationId, urnUuidLiteral(row["ORGANIZATION"]))
+                )
                 graph.add((provider, SYN.name, plainLiteral(row["NAME"])))
                 graph.add((provider, SYN.gender, plainLiteral(row["GENDER"])))
                 graph.add((provider, SYN.speciality, plainLiteral(row["SPECIALITY"])))
                 graph.add((provider, SYN.address, plainLiteral(row["ADDRESS"])))
                 graph.add((provider, SYN.city, plainLiteral(row["CITY"])))
-                graph.add((provider, SYN.utilization, integerLiteral(row["UTILIZATION"])))
+                graph.add(
+                    (provider, SYN.utilization, integerLiteral(row["UTILIZATION"]))
+                )
 
                 # Object Properties
-                graph.add((provider, SYN.isAffiliatedWith, organizationUri(row["ORGANIZATION"])))
+                graph.add(
+                    (
+                        provider,
+                        SYN.isAffiliatedWith,
+                        organizationUri(row["ORGANIZATION"]),
+                    )
+                )
                 graph.add((organization, SYN.hasEmployed, provider))
 
-                # User Trust
-                # graph.add(
-                #     (
-                #         provider,
-                #         TST.behavior,
-                #         float_literal(user_trust.iloc[index]["behavioral_trust"]),
-                #     )
-                # )
-                # graph.add(
-                #     (
-                #         provider,
-                #         TST.identity,
-                #         float_literal(user_trust.iloc[index]["identity_trust"]),
-                #     )
-                # )
-
                 bar()
 
 
 class Supply(Resource):
     def __init__(self, df):
         self.__resource_df = df
 
@@ -954,14 +1046,15 @@
             for index, row in self.__resource_df.iterrows():
                 # Create name of the supply class individual
                 supply = supplyUri(index)
                 patient = patientUri(row["PATIENT"])
                 encounter = encounterUri(row["ENCOUNTER"])
 
                 # Data Properties
+                graph.add((supply, RDF.type, SYN.Supply))  # type
                 graph.add((supply, SYN.date, dateLiteral(row["DATE"][:10])))
                 graph.add((supply, SYN.patientId, urnUuidLiteral(row["PATIENT"])))
                 graph.add((supply, SYN.encounterId, urnUuidLiteral(row["ENCOUNTER"])))
                 graph.add((supply, SYN.code, snomedCtLiteral(row["CODE"])))
                 graph.add((supply, SYN.description, plainLiteral(row["DESCRIPTION"])))
                 graph.add((supply, SYN.quantity, integerLiteral(row["QUANTITY"])))
```

### Comparing `synthea-rdf-0.1.3/synthea_rdf.egg-info/PKG-INFO` & `synthea-rdf-0.1.4/synthea_rdf.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synthea-rdf
-Version: 0.1.3
+Version: 0.1.4
 Summary: Semantic web representation for the Synthea.
 Author: Dae-young Kim
 Author-email: leroy.kim@umbc.edu
 License: GPLv3
 Project-URL: Source Code, https://github.com/leroykim/synthea-rdf
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -23,15 +23,15 @@
 ### Installation
 ```bash
 pip install synthea-rdf
 ```
 
 ### Single CSV
 ```python
-from from pathlib import Path
+from pathlib import Path
 from synthea_rdf.graph import GraphBuilder
 
 MODEL_PATH = "./synthea_ontology/synthea_ontology.ttl"
 CSV_DIR = "./csv"
 DEST_PATH = "./result"
 
 builder = GraphBuilder(CSV_DIR, MODEL_PATH)
@@ -68,20 +68,7 @@
 CSV_DIR = "./csv"
 DEST_PATH = "./result"
 
 builder = GraphBuilder(CSV_DIR, MODEL_PATH)
 graph = builder.build()
 graph.serialize(destination=Path(DEST_PATH) / "all.ttl")
 ```
-
-## :warning: Issues
-- [ ] Confusing naming convention for the following data properties:
-
-        - syn:start
-        - syn:startDate
-        - syn:startDateTime
-        - syn:date
-        - syn:dateTime
-
-- [ ] There are no `Allergy` and `ImagingStudy` data in the test dataset. Testing required with a larger dataset.
-    - [ ] Test `Allergy`
-    - [ ] Test `ImagingStudy`
```

### Comparing `synthea-rdf-0.1.3/tests/test_convert.py` & `synthea-rdf-0.1.4/tests/test_convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path
 from synthea_rdf.graph import GraphBuilder
 
 MODEL_PATH = "./synthea_ontology/synthea_ontology.ttl"
-CSV_DIR = "./csv"
+CSV_DIR = "./csv/Maryland_covid19_patient_10_bin_1"
 DEST_PATH = "./test_result"
 
 
 def test_convert_allergy():
     builder = GraphBuilder(CSV_DIR, MODEL_PATH)
     builder.convertAllergy()
     assert builder.serialize(destination=Path(DEST_PATH) / "allergy.ttl") == builder.graph
```

