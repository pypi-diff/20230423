# Comparing `tmp/enrRiceTrait-1.1.6.tar.gz` & `tmp/enrRiceTrait-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\enrRiceTrait-1.1.6.tar", last modified: Mon Mar 29 15:26:55 2021, max compression
+gzip compressed data, was "enrRiceTrait-1.2.0.tar", last modified: Sun Apr 23 12:15:32 2023, max compression
```

## Comparing `enrRiceTrait-1.1.6.tar` & `enrRiceTrait-1.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2021-03-29 15:26:55.000000 enrRiceTrait-1.1.6/
--rw-rw-rw-   0        0        0       53 2021-03-29 13:55:51.000000 enrRiceTrait-1.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0      618 2021-03-29 15:26:55.000000 enrRiceTrait-1.1.6/PKG-INFO
--rw-rw-rw-   0        0        0       92 2020-07-13 13:31:42.000000 enrRiceTrait-1.1.6/README.md
-drwxrwxrwx   0        0        0        0 2021-03-29 15:26:55.000000 enrRiceTrait-1.1.6/enrRiceTrait/
--rw-rw-rw-   0        0        0    19667 2021-03-29 15:26:37.000000 enrRiceTrait-1.1.6/enrRiceTrait/Enrichment.py
--rw-rw-rw-   0        0        0      478 2021-03-29 14:59:32.000000 enrRiceTrait-1.1.6/enrRiceTrait/PTE_config.py
--rw-rw-rw-   0        0        0      222 2021-03-29 02:12:50.000000 enrRiceTrait-1.1.6/enrRiceTrait/__init__.py
-drwxrwxrwx   0        0        0        0 2021-03-29 15:26:55.000000 enrRiceTrait-1.1.6/enrRiceTrait/data/
--rw-rw-rw-   0        0        0  9834834 2021-03-27 15:22:16.000000 enrRiceTrait-1.1.6/enrRiceTrait/data/Total_Association.txt
--rw-rw-rw-   0        0        0  1090456 2021-03-25 12:59:06.000000 enrRiceTrait-1.1.6/enrRiceTrait/data/to.wto.ro.funRiceGene.obo
-drwxrwxrwx   0        0        0        0 2021-03-29 15:26:55.000000 enrRiceTrait-1.1.6/enrRiceTrait.egg-info/
--rw-rw-rw-   0        0        0      618 2021-03-29 15:26:55.000000 enrRiceTrait-1.1.6/enrRiceTrait.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      337 2021-03-29 15:26:55.000000 enrRiceTrait-1.1.6/enrRiceTrait.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-03-29 15:26:55.000000 enrRiceTrait-1.1.6/enrRiceTrait.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2021-03-29 15:26:55.000000 enrRiceTrait-1.1.6/enrRiceTrait.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-03-29 15:26:55.000000 enrRiceTrait-1.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1085 2021-03-29 15:26:45.000000 enrRiceTrait-1.1.6/setup.py
+drwxr-xr-x   0 yao        (501) staff       (20)        0 2023-04-23 12:15:32.056778 enrRiceTrait-1.2.0/
+-rw-rw-r--   0 yao        (501) staff       (20)       53 2021-03-29 13:55:50.000000 enrRiceTrait-1.2.0/MANIFEST.in
+-rw-r--r--   0 yao        (501) staff       (20)      599 2023-04-23 12:15:32.056502 enrRiceTrait-1.2.0/PKG-INFO
+-rw-rw-r--   0 yao        (501) staff       (20)       92 2020-07-13 13:31:42.000000 enrRiceTrait-1.2.0/README.md
+drwxr-xr-x   0 yao        (501) staff       (20)        0 2023-04-23 12:15:32.031151 enrRiceTrait-1.2.0/enrRiceTrait/
+-rw-r--r--   0 yao        (501) staff       (20)    23316 2023-04-23 12:09:04.000000 enrRiceTrait-1.2.0/enrRiceTrait/Enrichment.py
+-rw-rw-r--   0 yao        (501) staff       (20)      478 2021-03-29 14:59:32.000000 enrRiceTrait-1.2.0/enrRiceTrait/PTE_config.py
+-rw-rw-r--   0 yao        (501) staff       (20)      222 2021-03-29 02:12:50.000000 enrRiceTrait-1.2.0/enrRiceTrait/__init__.py
+drwxr-xr-x   0 yao        (501) staff       (20)        0 2023-04-23 12:15:32.050664 enrRiceTrait-1.2.0/enrRiceTrait/data/
+-rw-rw-r--   0 yao        (501) staff       (20)  9834834 2021-03-27 15:22:16.000000 enrRiceTrait-1.2.0/enrRiceTrait/data/Total_Association.txt
+-rw-rw-r--   0 yao        (501) staff       (20)  1090456 2021-03-25 12:59:06.000000 enrRiceTrait-1.2.0/enrRiceTrait/data/to.wto.ro.funRiceGene.obo
+drwxr-xr-x   0 yao        (501) staff       (20)        0 2023-04-23 12:15:32.032229 enrRiceTrait-1.2.0/enrRiceTrait.egg-info/
+-rw-rw-r--   0 yao        (501) staff       (20)      599 2023-04-23 12:15:31.000000 enrRiceTrait-1.2.0/enrRiceTrait.egg-info/PKG-INFO
+-rw-rw-r--   0 yao        (501) staff       (20)      337 2023-04-23 12:15:32.000000 enrRiceTrait-1.2.0/enrRiceTrait.egg-info/SOURCES.txt
+-rw-rw-r--   0 yao        (501) staff       (20)        1 2023-04-23 12:15:31.000000 enrRiceTrait-1.2.0/enrRiceTrait.egg-info/dependency_links.txt
+-rw-rw-r--   0 yao        (501) staff       (20)       13 2023-04-23 12:15:31.000000 enrRiceTrait-1.2.0/enrRiceTrait.egg-info/top_level.txt
+-rw-r--r--   0 yao        (501) staff       (20)       38 2023-04-23 12:15:32.056877 enrRiceTrait-1.2.0/setup.cfg
+-rw-rw-r--   0 yao        (501) staff       (20)     1085 2023-04-23 12:05:02.000000 enrRiceTrait-1.2.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `enrRiceTrait-1.1.6/enrRiceTrait/Enrichment.py` & `enrRiceTrait-1.2.0/enrRiceTrait/Enrichment.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 # -*- coding:utf-8 -*-
 # ! usr/bin/env python3
 """
 Created on 09/07/2020 下午4:15
 @Author: xinzhi yao
 """
+# check if the package is complete.
 # python setup.py check
+# generate the package file.
 # python3 setup.py sdist bdist_wheel
+# only test
 # python3 -m twine upload --repository testpypi dist/*
-# python setup.py register sdist upload -r http://pypi.org
+# upload to your pypi
+# python3 setup.py register sdist upload -r http://pypi.org
 
 import os
 import re
-import wget
 import matplotlib
 import numpy as np
 import pandas as pd
 from plotnine import *
 import matplotlib.pyplot as plt
 from scipy.stats import hypergeom
 from collections import defaultdict
@@ -32,14 +35,18 @@
         self.terms_count = defaultdict(int)
 
         # Statistics of each concept
         self.terms_p_value = defaultdict(float)
         self.terms_p_adjust = defaultdict(float)
         self.terms_q_value = defaultdict(float)
 
+        # Bonferroni or Benjamini & Hochberg correlation
+        self.terms_p_bh = defaultdict(float)
+        self.terms_p_bf = defaultdict(float)
+
         self.Gene_Ratio = defaultdict(float)
         self.BG_Ratio = defaultdict(float)
 
 
 class Association:
     def __init__(self, gene_id: str, concept_id: str, source: str, evidence=''):
         self.gene_id = gene_id
@@ -78,15 +85,14 @@
 
                 self.gene_to_trait[gene_id].add(concept)
                 self.trait_to_gene[concept].add(gene_id)
 
                 self.pair_to_source[(gene_id, concept)].add(source)
                 self.pair_to_evidence[(gene_id, concept)].add(evidence)
 
-
 class trait_concept:
     def __init__(self, trait_id: str, trait_name: str, definition: str):
         self.id = trait_id
         self.trait_name = trait_name
         self.definition = definition
 
 
@@ -136,14 +142,17 @@
                     _id = l[1]
                 elif line.startswith('name:'):
                     if len(l) < 2:
                         continue
                     trait = l[1]
                 elif line.startswith('def:'):
                     definition = re.findall(r'\"(.*?)\"', line)[0]
+                elif line.startswith('xref:'):
+                    xref_id = l[ 1 ]
+                    self.id_to_trait[xref_id] = trait_concept(xref_id, trait, definition)
                 elif l == [''] and _id and '/' not in _id:
                     self.id_to_trait[_id] = trait_concept(_id, trait, definition)
 
     # todo: Distinguish different ontology
     # todo: add the evidence to the last col of background data.
     # todo-done: add source info in backgroud data.
     def load_background_data(self):
@@ -185,36 +194,51 @@
         """
         rv = hypergeom(N, k, m)
         x_arg = np.arange(x, k + 1)
         pmf_dogs = rv.pmf(x_arg)
         p = sum(pmf_dogs)
         return p
 
-    # fixme-done: check it.
-    def p_adjust(self, method='BH'):
+    def p_bh_and_bf_compute(self):
+        count_terms = len(self.enrich_result.terms_p_value.keys())
+
+        sorted_terms = sorted(self.enrich_result.terms_p_value, key=lambda x: self.enrich_result.terms_p_value[x])
+        #  k need add 1
+        for k, term in enumerate(sorted_terms):
+            # updated p-adjust computing for BH
+            self.enrich_result.terms_p_bh[term] = min((self.enrich_result.terms_p_value[term] * count_terms) / (k+1), 1)
+
+        for term in self.enrich_result.terms_p_value.keys():
+            # updated p-adjust computing for Bonferroui
+            self.enrich_result.terms_p_bf[term] = min(self.enrich_result.terms_p_value[term] / count_terms, 1)
+
+
+    def p_adjust_compute(self, method='BH'):
         count_terms = len(self.enrich_result.terms_p_value.keys())
 
         if method not in {'BH', 'Bonferroui'}:
             raise TypeError('Method must be "BH" or "Bonferroui"')
 
-
         if method == 'BH':
-
             sorted_terms = sorted(self.enrich_result.terms_p_value, key=lambda x: self.enrich_result.terms_p_value[x])
-            # fixme: k nedd add 1
+            #  k need add 1
             for k, term in enumerate(sorted_terms):
-                self.enrich_result.terms_p_adjust[term] = (self.p_threshold * (k+1)) / count_terms
+                # updated p-adjust computing for BH
+                # self.enrich_result.terms_p_adjust[term] = (self.p_threshold * (k+1)) / count_terms
+                self.enrich_result.terms_p_adjust[term] = min((self.enrich_result.terms_p_value[term] * count_terms) / (k+1), 1)
+
         elif method == 'Bonferroui':
             for term in self.enrich_result.terms_p_value.keys():
-                self.enrich_result.terms_p_adjust[term] = self.p_threshold / count_terms
+                # updated p-adjust computing for Bonferroui
+                # self.enrich_result.terms_p_adjust[term] = self.p_threshold / count_terms
+                self.enrich_result.terms_p_adjust[term] = min(self.enrich_result.terms_p_value[term] / count_terms, 1)
         else:
             raise TypeError("The p-value correction method must be 'BH' or 'Bonferroui'")
 
-    # fixme-done: check it.
-    def q_value(self):
+    def q_value_compute(self):
 
         count_terms = len(self.enrich_result.terms_p_value)
         sorted_terms = sorted(self.enrich_result.terms_p_value, key=lambda x: self.enrich_result.terms_p_value[x])
 
         for k, trait_id in enumerate(sorted_terms):
             self.enrich_result.terms_q_value[trait_id] = (self.enrich_result.terms_p_value[trait_id] * count_terms) / (k+1)
 
@@ -227,68 +251,83 @@
         :param p_threshold: threshold for p-value
         :return:
         """
 
         self.p_threshold = p_threshold
         self.enrich_result = enrichment_result()
 
-        if id_type == 'rap':
+        if id_type.lower() == 'rap':
             bg_data = self.rap_background
-        elif id_type == 'msu':
+        elif id_type.lower() == 'msu':
             bg_data = self.msu_background
-        elif id_type == 'gramene':
+        elif id_type.lower() == 'gramene':
             bg_data = self.gramene_background
         else:
             print('Gene id type must be "RAPDB", "MSU" or "Gramene".')
             raise TypeError
 
         N = len(bg_data.gene_set)
 
         # query_gene_count
         k = 0
+        matched_gene_set = set()
         for _id in query_gene_set:
             if _id in bg_data.gene_set:
                 k += 1
+                matched_gene_set.add(_id)
                 # number of trait related this gene.
                 for trait_id in bg_data.gene_to_trait[_id]:
                     self.enrich_result.terms_count[trait_id] += 1
             else:
                 self.enrich_result.miss_id_set.add(_id)
 
+        print(f'{len(matched_gene_set):,}/{len(query_gene_set):,} are found in the background data,'
+              f' include: {matched_gene_set}.')
+
+        print(f'{len(self.enrich_result.miss_id_set):,}/{len(query_gene_set):,} genes are missed in the background data,'
+              f' include: {self.enrich_result.miss_id_set}.')
+
         # enrichment
         for trait_id in self.enrich_result.terms_count.keys():
             trait_related_gene = bg_data.trait_to_gene[trait_id]
             m = len(bg_data.trait_to_gene[trait_id])
             x = len(trait_related_gene & query_gene_set)
 
-            # p = self.Hyper_Geometric_Test(N, m_dict[trait], m, self.enrich_result.terms_count[trait])
-            # print(N, m, k, x)
             p_value = self.Hyper_Geometric_Test(N, m, k, x)
             if p_value < self.p_threshold:
                 self.enrich_result.terms_p_value[trait_id] = p_value
                 # fixme: check here.
                 # print(trait_id, x, k)
                 self.enrich_result.Gene_Ratio[trait_id] =  x / k
                 self.enrich_result.BG_Ratio[trait_id] = k / N
 
         # todo: method need to give users options
-        self.p_adjust(p_adjust_method)
-        self.q_value()
-
+        self.p_adjust_compute(p_adjust_method)
+        self.q_value_compute()
+        self.p_bh_and_bf_compute()
 
         sorted_result = sorted(self.enrich_result.terms_p_value.keys(),
                                key=lambda x: self.enrich_result.terms_p_value[x])
 
-        print(f'{"Trait id":<10}\t{"Trait name":<50}\t{"p-value":<8}\t{"p-adjust":<8}'
-              f'\t{"q-value":<8}')
+        # change the print information of this package
+        print(f'{"Trait id":<10}\t{"Trait name":<50}\t{"p-value":<8}\t{"Bonferroni adjusted p-value":<8}'
+              f'\t{"BH adjusted p-value":<8}')
         for trait_id in sorted_result:
-            print(f'{trait_id:<10}\t{self.id_to_trait[trait_id].trait_name:<50}\t'
-                  f'{self.enrich_result.terms_p_value[trait_id]:<.2e}\t'
-                  f'{self.enrich_result.terms_p_adjust[trait_id]:<.2e}\t'
-                  f'{self.enrich_result.terms_q_value[trait_id]:<.2e}')
+            print(f'{trait_id:<10}\t{self.id_to_trait[ trait_id ].trait_name:<50}\t'
+                  f'{self.enrich_result.terms_p_value[ trait_id ]:<.2e}\t'
+                  f'{self.enrich_result.terms_p_bf[ trait_id ]:<.2e}\t'
+                  f'{self.enrich_result.terms_p_bh[ trait_id ]:<.2e}')
+
+        # print(f'{"Trait id":<10}\t{"Trait name":<50}\t{"p-value":<8}\t{"p-adjust":<8}'
+        #       f'\t{"q-value":<8}')
+        # for trait_id in sorted_result:
+        #     print(f'{trait_id:<10}\t{self.id_to_trait[trait_id].trait_name:<50}\t'
+        #           f'{self.enrich_result.terms_p_value[trait_id]:<.2e}\t'
+        #           f'{self.enrich_result.terms_p_adjust[trait_id]:<.2e}\t'
+        #           f'{self.enrich_result.terms_q_value[trait_id]:<.2e}')
 
         if save_result:
             if not save_path:
                 raise TypeError('You have to provide a path to save the result.')
             self.save_result(self.enrich_result, save_path, prefix)
 
         self.dataframe_init()
@@ -299,25 +338,31 @@
         sorted_trait_id = sorted(self.enrich_result.terms_p_value,
                                  key=lambda x: self.enrich_result.terms_p_value[ x ])
         trait_name = [self.id_to_trait[trait_id].trait_name for trait_id in sorted_trait_id]
         trait_definition = [self.id_to_trait[trait_id].definition for trait_id in sorted_trait_id]
         trait_GeneRatio = [self.enrich_result.Gene_Ratio[trait_id] for trait_id in sorted_trait_id]
         trait_BgRatio = [self.enrich_result.BG_Ratio[trait_id] for trait_id in sorted_trait_id]
         trait_p = [self.enrich_result.terms_p_value[trait_id] for trait_id in sorted_trait_id]
+        trait_p_bf = [self.enrich_result.terms_p_bf[trait_id] for trait_id in sorted_trait_id]
+        trait_p_bh = [self.enrich_result.terms_p_bh[trait_id] for trait_id in sorted_trait_id]
+
         trait_p_adjust = [self.enrich_result.terms_p_adjust[trait_id] for trait_id in sorted_trait_id]
         trait_q = [self.enrich_result.terms_q_value[trait_id] for trait_id in sorted_trait_id]
+
         trait_count = [self.enrich_result.terms_count[trait_id] for trait_id in sorted_trait_id]
 
         self.enrich_dataframe = pd.DataFrame({'ID': sorted_trait_id, 'Name': trait_name,
                                          'Description': trait_definition,
                                          'GeneRatio': trait_GeneRatio,
                                          'BgRatio': trait_BgRatio,
                                          'p-value': trait_p,
                                          'p-adjust': trait_p_adjust,
                                          'q-value': trait_q,
+                                         'p-bh': trait_p_bh,
+                                         'p-bf': trait_p_bf,
                                          'Count': trait_count
                                          })
 
         self.enrich_dataframe[ 'ID_Name' ] = self.enrich_dataframe[ 'ID' ] + ' ' + self.enrich_dataframe[ 'Name' ]
 
         self.enrich_dataframe[ 'p_value_str' ] = 'p-Value ' + self.enrich_dataframe[ 'p-value' ].map('{:.3e}'.format)
 
@@ -336,29 +381,37 @@
             os.mkdir(save_path)
 
         sorted_result = sorted(self.enrich_result.terms_p_value.keys(),
                                key=lambda x: self.enrich_result.terms_p_value[ x ])
 
         save_file = f'{save_path}/{prefix}.report.txt'
         with open(save_file, 'w') as wf:
+            # wf.write('ID\tName\tDescription\tGeneRatio\tBgRatio\tp-value\t'
+            #          'p-adjust\tq-value\tCount\n')
             wf.write('ID\tName\tDescription\tGeneRatio\tBgRatio\tp-value\t'
-                     'p-adjust\tq-value\tCount\n')
+                     'Bonferroni adjusted p-adjust\tBH adjusted p-value\tCount\n')
             for term_id in sorted_result:
                 trait_name = self.id_to_trait[term_id].trait_name
                 definition = self.id_to_trait[term_id].definition \
                                 if self.id_to_trait[term_id].definition else "Noun"
                 gene_ratio = enrich_result.Gene_Ratio[term_id]
                 bg_raito = enrich_result.BG_Ratio[term_id]
                 p_value = enrich_result.terms_p_value[term_id]
-                p_adjust = enrich_result.terms_p_adjust[term_id]
+                p_adjust_value = enrich_result.terms_p_adjust[term_id]
                 q_value = enrich_result.terms_q_value[term_id]
-                # todo: add term count for query gene set.
+
+                p_bf = enrich_result.terms_p_bf[term_id]
+                p_bh = enrich_result.terms_p_bh[term_id]
+
+                # add term count for query gene set.
                 trait_count = enrich_result.terms_count[term_id]
                 wf.write(f'{term_id}\t{trait_name}\t{definition}\t{gene_ratio}\t'
-                         f'{bg_raito}\t{p_value}\t{p_adjust}\t{q_value}\t{trait_count}\n')
+                         f'{bg_raito}\t{p_value}\t{p_bf}\t{p_bh}\t{trait_count}\n')
+                # wf.write(f'{term_id}\t{trait_name}\t{definition}\t{gene_ratio}\t'
+                #          f'{bg_raito}\t{p_value}\t{p_adjust_value}\t{q_value}\t{trait_count}\n')
         print(f'{save_file} save done.')
 
 
     # todo: add legend
     def draw_bar(self, save_path='../result',  prefix='EnrRiceTrait', save_plot=False):
         sorted_terms = sorted(self.enrich_result.terms_p_value,
                               key=lambda x: self.enrich_result.terms_p_value[x], reverse=True)
@@ -474,7 +527,22 @@
 
         if save_path:
             save_file = f'{save_path}/{prefix}.bubble2.png'
             p2.save(save_file, width=6, height=4, dpi=150)
 
         return p2
 
+# fixme: test main
+# if __name__ == '__main__':
+#     source_set = {'Oryzabase', 'TAS', 'ExactMatching'}
+#
+#     query_gene_set = {'Os01g0382000', 'Os01g0767900', 'Os01g0812100',
+#                       'Os02g0521300', 'Os03g0160100', 'Os03g0172000',
+#                       'Os05g0368300', 'Os09g0392100', 'Os11g0229500',
+#                       'Os11g0482000'}
+#
+#     Enricher = Gene_Ontology_enrichment(source_set)
+#
+#     # MSU must is lower case.
+#     # source code have been changed.
+#     Enricher.ontology_enricement(query_gene_set, 'msu')
+
```

### Comparing `enrRiceTrait-1.1.6/enrRiceTrait/data/Total_Association.txt` & `enrRiceTrait-1.2.0/enrRiceTrait/data/Total_Association.txt`

 * *Files identical despite different names*

### Comparing `enrRiceTrait-1.1.6/enrRiceTrait/data/to.wto.ro.funRiceGene.obo` & `enrRiceTrait-1.2.0/enrRiceTrait/data/to.wto.ro.funRiceGene.obo`

 * *Files identical despite different names*

### Comparing `enrRiceTrait-1.1.6/setup.py` & `enrRiceTrait-1.2.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setup(
   name='enrRiceTrait',
-  version='1.1.6',
+  version='1.2.0',
   author='xinzhi_yao',
   author_email='xinzhi_bioinfo@163.com',
   description="A python package for Rice Trait Enrichment.",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/YaoXinZhi/enrRiceTrait",
```

