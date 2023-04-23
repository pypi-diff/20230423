# Comparing `tmp/enrRiceTrait-1.2.0.tar.gz` & `tmp/enrRiceTrait-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enrRiceTrait-1.2.0.tar", last modified: Sun Apr 23 12:15:32 2023, max compression
+gzip compressed data, was "enrRiceTrait-1.2.1.tar", last modified: Sun Apr 23 14:57:49 2023, max compression
```

## Comparing `enrRiceTrait-1.2.0.tar` & `enrRiceTrait-1.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 yao        (501) staff       (20)        0 2023-04-23 12:15:32.056778 enrRiceTrait-1.2.0/
--rw-rw-r--   0 yao        (501) staff       (20)       53 2021-03-29 13:55:50.000000 enrRiceTrait-1.2.0/MANIFEST.in
--rw-r--r--   0 yao        (501) staff       (20)      599 2023-04-23 12:15:32.056502 enrRiceTrait-1.2.0/PKG-INFO
--rw-rw-r--   0 yao        (501) staff       (20)       92 2020-07-13 13:31:42.000000 enrRiceTrait-1.2.0/README.md
-drwxr-xr-x   0 yao        (501) staff       (20)        0 2023-04-23 12:15:32.031151 enrRiceTrait-1.2.0/enrRiceTrait/
--rw-r--r--   0 yao        (501) staff       (20)    23316 2023-04-23 12:09:04.000000 enrRiceTrait-1.2.0/enrRiceTrait/Enrichment.py
--rw-rw-r--   0 yao        (501) staff       (20)      478 2021-03-29 14:59:32.000000 enrRiceTrait-1.2.0/enrRiceTrait/PTE_config.py
--rw-rw-r--   0 yao        (501) staff       (20)      222 2021-03-29 02:12:50.000000 enrRiceTrait-1.2.0/enrRiceTrait/__init__.py
-drwxr-xr-x   0 yao        (501) staff       (20)        0 2023-04-23 12:15:32.050664 enrRiceTrait-1.2.0/enrRiceTrait/data/
--rw-rw-r--   0 yao        (501) staff       (20)  9834834 2021-03-27 15:22:16.000000 enrRiceTrait-1.2.0/enrRiceTrait/data/Total_Association.txt
--rw-rw-r--   0 yao        (501) staff       (20)  1090456 2021-03-25 12:59:06.000000 enrRiceTrait-1.2.0/enrRiceTrait/data/to.wto.ro.funRiceGene.obo
-drwxr-xr-x   0 yao        (501) staff       (20)        0 2023-04-23 12:15:32.032229 enrRiceTrait-1.2.0/enrRiceTrait.egg-info/
--rw-rw-r--   0 yao        (501) staff       (20)      599 2023-04-23 12:15:31.000000 enrRiceTrait-1.2.0/enrRiceTrait.egg-info/PKG-INFO
--rw-rw-r--   0 yao        (501) staff       (20)      337 2023-04-23 12:15:32.000000 enrRiceTrait-1.2.0/enrRiceTrait.egg-info/SOURCES.txt
--rw-rw-r--   0 yao        (501) staff       (20)        1 2023-04-23 12:15:31.000000 enrRiceTrait-1.2.0/enrRiceTrait.egg-info/dependency_links.txt
--rw-rw-r--   0 yao        (501) staff       (20)       13 2023-04-23 12:15:31.000000 enrRiceTrait-1.2.0/enrRiceTrait.egg-info/top_level.txt
--rw-r--r--   0 yao        (501) staff       (20)       38 2023-04-23 12:15:32.056877 enrRiceTrait-1.2.0/setup.cfg
--rw-rw-r--   0 yao        (501) staff       (20)     1085 2023-04-23 12:05:02.000000 enrRiceTrait-1.2.0/setup.py
+drwxr-xr-x   0 yao        (501) staff       (20)        0 2023-04-23 14:57:49.383813 enrRiceTrait-1.2.1/
+-rw-rw-r--   0 yao        (501) staff       (20)       53 2021-03-29 13:55:50.000000 enrRiceTrait-1.2.1/MANIFEST.in
+-rw-r--r--   0 yao        (501) staff       (20)      599 2023-04-23 14:57:49.383499 enrRiceTrait-1.2.1/PKG-INFO
+-rw-rw-r--   0 yao        (501) staff       (20)       92 2020-07-13 13:31:42.000000 enrRiceTrait-1.2.1/README.md
+drwxr-xr-x   0 yao        (501) staff       (20)        0 2023-04-23 14:57:49.351439 enrRiceTrait-1.2.1/enrRiceTrait/
+-rw-r--r--   0 yao        (501) staff       (20)    28228 2023-04-23 14:14:51.000000 enrRiceTrait-1.2.1/enrRiceTrait/Enrichment.py
+-rw-rw-r--   0 yao        (501) staff       (20)      478 2021-03-29 14:59:32.000000 enrRiceTrait-1.2.1/enrRiceTrait/PTE_config.py
+-rw-rw-r--   0 yao        (501) staff       (20)      222 2023-04-23 14:57:32.000000 enrRiceTrait-1.2.1/enrRiceTrait/__init__.py
+drwxr-xr-x   0 yao        (501) staff       (20)        0 2023-04-23 14:57:49.376342 enrRiceTrait-1.2.1/enrRiceTrait/data/
+-rw-rw-r--   0 yao        (501) staff       (20)  9834834 2021-03-27 15:22:16.000000 enrRiceTrait-1.2.1/enrRiceTrait/data/Total_Association.txt
+-rw-rw-r--   0 yao        (501) staff       (20)  1090456 2021-03-25 12:59:06.000000 enrRiceTrait-1.2.1/enrRiceTrait/data/to.wto.ro.funRiceGene.obo
+drwxr-xr-x   0 yao        (501) staff       (20)        0 2023-04-23 14:57:49.353908 enrRiceTrait-1.2.1/enrRiceTrait.egg-info/
+-rw-rw-r--   0 yao        (501) staff       (20)      599 2023-04-23 14:57:49.000000 enrRiceTrait-1.2.1/enrRiceTrait.egg-info/PKG-INFO
+-rw-rw-r--   0 yao        (501) staff       (20)      337 2023-04-23 14:57:49.000000 enrRiceTrait-1.2.1/enrRiceTrait.egg-info/SOURCES.txt
+-rw-rw-r--   0 yao        (501) staff       (20)        1 2023-04-23 14:57:49.000000 enrRiceTrait-1.2.1/enrRiceTrait.egg-info/dependency_links.txt
+-rw-rw-r--   0 yao        (501) staff       (20)       13 2023-04-23 14:57:49.000000 enrRiceTrait-1.2.1/enrRiceTrait.egg-info/top_level.txt
+-rw-r--r--   0 yao        (501) staff       (20)       38 2023-04-23 14:57:49.384014 enrRiceTrait-1.2.1/setup.cfg
+-rw-rw-r--   0 yao        (501) staff       (20)     1085 2023-04-23 14:57:32.000000 enrRiceTrait-1.2.1/setup.py
```

### Comparing `enrRiceTrait-1.2.0/PKG-INFO` & `enrRiceTrait-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enrRiceTrait
-Version: 1.2.0
+Version: 1.2.1
 Summary: A python package for Rice Trait Enrichment.
 Home-page: https://github.com/YaoXinZhi/enrRiceTrait
 Author: xinzhi_yao
 Author-email: xinzhi_bioinfo@163.com
 License: UNKNOWN
 Description: # Plant Trait Enrichment Package  
         This is a python package for plant trait enrichment.
```

### Comparing `enrRiceTrait-1.2.0/enrRiceTrait/Enrichment.py` & `enrRiceTrait-1.2.1/enrRiceTrait/Enrichment.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 # -*- coding:utf-8 -*-
 # ! usr/bin/env python3
 """
 Created on 09/07/2020 下午4:15
 @Author: xinzhi yao
 """
-# check if the package is complete.
+# 1. check if the package is complete.
 # python setup.py check
-# generate the package file.
+# 2. generate the package file.
 # python3 setup.py sdist bdist_wheel
 # only test
 # python3 -m twine upload --repository testpypi dist/*
-# upload to your pypi
+# upload to your pypi (obselate)
 # python3 setup.py register sdist upload -r http://pypi.org
+# 3. upload to your pypi
+# twine upload dist/*
+
 
 import os
 import re
 import matplotlib
 import numpy as np
 import pandas as pd
 from plotnine import *
@@ -282,38 +285,39 @@
 
         print(f'{len(matched_gene_set):,}/{len(query_gene_set):,} are found in the background data,'
               f' include: {matched_gene_set}.')
 
         print(f'{len(self.enrich_result.miss_id_set):,}/{len(query_gene_set):,} genes are missed in the background data,'
               f' include: {self.enrich_result.miss_id_set}.')
 
+        if len(matched_gene_set) == 0:
+            raise ValueError('No gene match in enrRiceTrait background data.')
+
         # enrichment
         for trait_id in self.enrich_result.terms_count.keys():
             trait_related_gene = bg_data.trait_to_gene[trait_id]
             m = len(bg_data.trait_to_gene[trait_id])
             x = len(trait_related_gene & query_gene_set)
 
             p_value = self.Hyper_Geometric_Test(N, m, k, x)
             if p_value < self.p_threshold:
                 self.enrich_result.terms_p_value[trait_id] = p_value
-                # fixme: check here.
-                # print(trait_id, x, k)
                 self.enrich_result.Gene_Ratio[trait_id] =  x / k
                 self.enrich_result.BG_Ratio[trait_id] = k / N
 
-        # todo: method need to give users options
+        # method need to give users options
         self.p_adjust_compute(p_adjust_method)
         self.q_value_compute()
         self.p_bh_and_bf_compute()
 
         sorted_result = sorted(self.enrich_result.terms_p_value.keys(),
                                key=lambda x: self.enrich_result.terms_p_value[x])
 
         # change the print information of this package
-        print(f'{"Trait id":<10}\t{"Trait name":<50}\t{"p-value":<8}\t{"Bonferroni adjusted p-value":<8}'
+        print(f'{"Trait id":<10}\t{"Trait name":<50}\t{"p-value":<8}\t{"Bonferroni adjusted p-value":<20}'
               f'\t{"BH adjusted p-value":<8}')
         for trait_id in sorted_result:
             print(f'{trait_id:<10}\t{self.id_to_trait[ trait_id ].trait_name:<50}\t'
                   f'{self.enrich_result.terms_p_value[ trait_id ]:<.2e}\t'
                   f'{self.enrich_result.terms_p_bf[ trait_id ]:<.2e}\t'
                   f'{self.enrich_result.terms_p_bh[ trait_id ]:<.2e}')
 
@@ -527,22 +531,146 @@
 
         if save_path:
             save_file = f'{save_path}/{prefix}.bubble2.png'
             p2.save(save_file, width=6, height=4, dpi=150)
 
         return p2
 
-# fixme: test main
-# if __name__ == '__main__':
-#     source_set = {'Oryzabase', 'TAS', 'ExactMatching'}
-#
-#     query_gene_set = {'Os01g0382000', 'Os01g0767900', 'Os01g0812100',
-#                       'Os02g0521300', 'Os03g0160100', 'Os03g0172000',
-#                       'Os05g0368300', 'Os09g0392100', 'Os11g0229500',
-#                       'Os11g0482000'}
-#
-#     Enricher = Gene_Ontology_enrichment(source_set)
-#
-#     # MSU must is lower case.
-#     # source code have been changed.
-#     Enricher.ontology_enricement(query_gene_set, 'msu')
+    # latest bar plot 2023-04-23
+    def bar_stat(self, save_path='.', prefix='enrRiceTrait.bar', save_plot=False):
+        # plot data from large p-value to small p-value
+        sorted_result = sorted(self.enrich_result.terms_p_value.keys(),
+                               key=lambda x: self.enrich_result.terms_p_value[ x ],
+                               reverse=True)
+
+        data = []
+        for term_id in sorted_result:
+            trait_name = self.id_to_trait[ term_id ].trait_name
+            trait_count = self.enrich_result.terms_count[ term_id ]
+            p_value = self.enrich_result.terms_p_value[ term_id ]
+
+            data.append([trait_name, trait_count, p_value])
+
+        print(f'data')
+        print(data)
+
+        font_size = 24
+        # 设置颜色映射
+        cmap = plt.cm.get_cmap('RdYlBu_r')
+
+        # 转换基因数和p值为浮点数
+        gene_nums = [ float(d[ 1 ]) for d in data ]
+        p_values = [ -np.log10(float(d[ 2 ])) for d in data ]
+
+        # 根据p值设置颜色
+        colors = [ cmap(p) for p in np.interp(p_values, (np.min(p_values), np.max(p_values)), (0, 1)) ]
+
+        plt.rcParams[ 'font.family' ] = 'Times New Roman'
+
+        # 绘制水平条形图
+        fig, ax = plt.subplots(figsize=(16, 14))
+        bars = ax.barh(range(len(data)), gene_nums, color=colors)
+        ax.grid(True, linestyle='--', linewidth=0.5, color='gray')
+
+        # 设置Y轴标签和刻度
+        ax.set_yticks(range(len(data)))
+        ax.set_yticklabels([ d[ 0 ].capitalize() for d in data ], fontsize=font_size)
+
+        ax.set_xticklabels([ i for i in range(len(gene_nums)) ], fontsize=font_size)
+
+        # 设置X轴标签和刻度
+        ax.set_xlabel('Gene Count', fontsize=font_size)
+        # ax.set_ylabel('GO Enrichment Name')
+        # ax.set_title('GO Enrichment Bar Plot')
+        # 添加颜色条
+        sm = plt.cm.ScalarMappable(cmap=cmap, norm=plt.Normalize(vmin=np.min(p_values), vmax=np.max(p_values)))
+        sm._A = [ ]
+        cbar = fig.colorbar(sm, ax=ax)
+        # 设置 colorbar 的标签字体
+        cbar.ax.yaxis.label.set_fontfamily('Times New Roman')
+        # cbar.ax.yaxis.label.set_fontsize(16)
+
+        cbar.ax.tick_params(axis='both', which='major', labelsize=font_size)
+
+        plt.subplots_adjust(left=0.37)
+
+        plt.show()
+        if save_plot:
+            save_file = f'{save_path}/{prefix}.bar.png'
+            plt.savefig(save_file, dpi=300, bbox_inches='tight')
+            print(f'{save_file} saved.')
+
+    # latest version of bubble plot 2023-04-23
+    def bubble_stat(self, save_path='.', prefix='enrRiceTrait.bubble', save_plot=False):
+        sorted_result = sorted(self.enrich_result.terms_p_value.keys(),
+                               key=lambda x: self.enrich_result.terms_p_value[ x ],
+                               reverse=True)
+
+        df = defaultdict(list)
+        for term_id in sorted_result:
+            trait_name = self.id_to_trait[ term_id ].trait_name
+            trait_count = self.enrich_result.terms_count[ term_id ]
+            p_value = self.enrich_result.terms_p_value[ term_id ]
+
+            gene_ratio = self.enrich_result.Gene_Ratio[ term_id ]
+
+            df['gene ratio'].append(gene_ratio)
+            df['name'].append(trait_name)
+            df['count'].append(trait_count)
+            df['p-value'].append(p_value)
+
+        print('df')
+        print(df)
+
+        font_size = 24
+
+        # 创建子图
+        plt.rcParams[ 'font.family' ] = 'Times New Roman'
+
+        # fig, ax = plt.subplots()
+        fig, ax = plt.subplots(figsize=(16, 14))
+
+        ax.grid(True, linestyle='--', linewidth=0.5, color='gray')
+
+        # 设置散点图
+        scatter = ax.scatter(df[ 'gene ratio' ], list(map(lambda x: x.capitalize(), df[ 'name' ])), s=df[ 'count' ],
+                             c=df[ 'p-value' ], alpha=0.5, cmap='viridis')
+
+        # 添加颜色条
+        cbar = plt.colorbar(scatter)
+        cbar.ax.tick_params(labelsize=font_size)
+
+        # 设置气泡大小
+        scatter.set_sizes(200 * df[ 'count' ])
+
+        # 设置坐标轴标签和标题
+        ax.set_xlabel('Gene Ratio', fontsize=18)
+        # ax.set_ylabel('GO Enrichment Name')
+        # ax.set_title('GO Enrichment Bubble Plot')
+
+        plt.subplots_adjust(left=0.45)
+
+        ax.tick_params(axis='both', which='major', labelsize=font_size, direction='inout')
+
+        # 添加图例
+        # legend1 = ax.legend(*scatter.legend_elements(prop="sizes"), loc="upper right", title="Count", ncol=1, fontsize=10, handletextpad=0.4)
+        legend1 = ax.legend(*scatter.legend_elements(prop="sizes"), loc="lower right", title="Count", ncol=1,
+                            fontsize=28, handletextpad=0.4)
+
+        legend1.get_title().set_fontsize(font_size)  # 设置图例标题字体大小
+
+        legend1.get_texts()[ 0 ].set_text("1")
+        legend1.get_texts()[ 1 ].set_text("2")
+        legend1.get_texts()[ 2 ].set_text("3")
+        legend1.get_texts()[ 3 ].set_text("5")
+        legend1.get_texts()[ 4 ].set_text("7")
+        for text in legend1.get_texts():
+            text.set_fontsize(font_size)
+
+        # 显示图形
+        plt.show()
+        if save_plot:
+            save_file = f'{save_path}/{prefix}.bubble.png'
+            plt.savefig(save_file, dpi=300, bbox_inches='tight')
+            print(f'{save_file} saved.')
+
```

### Comparing `enrRiceTrait-1.2.0/enrRiceTrait/data/Total_Association.txt` & `enrRiceTrait-1.2.1/enrRiceTrait/data/Total_Association.txt`

 * *Files identical despite different names*

### Comparing `enrRiceTrait-1.2.0/enrRiceTrait/data/to.wto.ro.funRiceGene.obo` & `enrRiceTrait-1.2.1/enrRiceTrait/data/to.wto.ro.funRiceGene.obo`

 * *Files identical despite different names*

### Comparing `enrRiceTrait-1.2.0/enrRiceTrait.egg-info/PKG-INFO` & `enrRiceTrait-1.2.1/enrRiceTrait.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enrRiceTrait
-Version: 1.2.0
+Version: 1.2.1
 Summary: A python package for Rice Trait Enrichment.
 Home-page: https://github.com/YaoXinZhi/enrRiceTrait
 Author: xinzhi_yao
 Author-email: xinzhi_bioinfo@163.com
 License: UNKNOWN
 Description: # Plant Trait Enrichment Package  
         This is a python package for plant trait enrichment.
```

### Comparing `enrRiceTrait-1.2.0/setup.py` & `enrRiceTrait-1.2.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setup(
   name='enrRiceTrait',
-  version='1.2.0',
+  version='1.2.1',
   author='xinzhi_yao',
   author_email='xinzhi_bioinfo@163.com',
   description="A python package for Rice Trait Enrichment.",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/YaoXinZhi/enrRiceTrait",
```

