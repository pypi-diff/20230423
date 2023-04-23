# Comparing `tmp/MetaMatching-0.2.3.tar.gz` & `tmp/MetaMatching-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MetaMatching-0.2.3.tar", last modified: Fri Apr 21 12:29:10 2023, max compression
+gzip compressed data, was "MetaMatching-1.0.1.tar", last modified: Sun Apr 23 07:09:04 2023, max compression
```

## Comparing `MetaMatching-0.2.3.tar` & `MetaMatching-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 leqi      (1000) leqi      (1000)        0 2023-04-21 12:29:10.248707 MetaMatching-0.2.3/
--rw-rw-r--   0 leqi      (1000) leqi      (1000)     1068 2023-04-21 07:13:05.000000 MetaMatching-0.2.3/LICENSE.txt
-drwxrwxr-x   0 leqi      (1000) leqi      (1000)        0 2023-04-21 12:29:10.248707 MetaMatching-0.2.3/MetaMatching/
--rw-rw-r--   0 leqi      (1000) leqi      (1000)       69 2023-04-21 11:41:56.000000 MetaMatching-0.2.3/MetaMatching/__init__.py
--rw-rw-r--   0 leqi      (1000) leqi      (1000)     6737 2023-04-21 12:28:28.000000 MetaMatching-0.2.3/MetaMatching/model.py
--rw-rw-r--   0 leqi      (1000) leqi      (1000)    12243 2023-04-21 11:41:35.000000 MetaMatching-0.2.3/MetaMatching/utils.py
-drwxrwxr-x   0 leqi      (1000) leqi      (1000)        0 2023-04-21 12:29:10.248707 MetaMatching-0.2.3/MetaMatching.egg-info/
--rw-rw-r--   0 leqi      (1000) leqi      (1000)      265 2023-04-21 12:29:10.000000 MetaMatching-0.2.3/MetaMatching.egg-info/PKG-INFO
--rw-rw-r--   0 leqi      (1000) leqi      (1000)      314 2023-04-21 12:29:10.000000 MetaMatching-0.2.3/MetaMatching.egg-info/SOURCES.txt
--rw-rw-r--   0 leqi      (1000) leqi      (1000)        1 2023-04-21 12:29:10.000000 MetaMatching-0.2.3/MetaMatching.egg-info/dependency_links.txt
--rw-rw-r--   0 leqi      (1000) leqi      (1000)        1 2023-04-21 12:29:10.000000 MetaMatching-0.2.3/MetaMatching.egg-info/not-zip-safe
--rw-rw-r--   0 leqi      (1000) leqi      (1000)       84 2023-04-21 12:29:10.000000 MetaMatching-0.2.3/MetaMatching.egg-info/requires.txt
--rw-rw-r--   0 leqi      (1000) leqi      (1000)       13 2023-04-21 12:29:10.000000 MetaMatching-0.2.3/MetaMatching.egg-info/top_level.txt
--rw-rw-r--   0 leqi      (1000) leqi      (1000)      265 2023-04-21 12:29:10.248707 MetaMatching-0.2.3/PKG-INFO
--rw-rw-r--   0 leqi      (1000) leqi      (1000)      115 2023-04-21 07:11:30.000000 MetaMatching-0.2.3/README.rst
--rw-rw-r--   0 leqi      (1000) leqi      (1000)       38 2023-04-21 12:29:10.248707 MetaMatching-0.2.3/setup.cfg
--rw-rw-r--   0 leqi      (1000) leqi      (1000)      699 2023-04-21 12:29:01.000000 MetaMatching-0.2.3/setup.py
+drwxrwxr-x   0 leqi      (1000) leqi      (1000)        0 2023-04-23 07:09:04.336961 MetaMatching-1.0.1/
+-rw-rw-r--   0 leqi      (1000) leqi      (1000)     1068 2023-04-21 07:13:05.000000 MetaMatching-1.0.1/LICENSE.txt
+drwxrwxr-x   0 leqi      (1000) leqi      (1000)        0 2023-04-23 07:09:04.336961 MetaMatching-1.0.1/MetaMatching/
+-rw-rw-r--   0 leqi      (1000) leqi      (1000)       69 2023-04-21 11:41:56.000000 MetaMatching-1.0.1/MetaMatching/__init__.py
+-rw-rw-r--   0 leqi      (1000) leqi      (1000)     6737 2023-04-21 12:28:28.000000 MetaMatching-1.0.1/MetaMatching/model.py
+-rw-rw-r--   0 leqi      (1000) leqi      (1000)    12303 2023-04-23 07:01:08.000000 MetaMatching-1.0.1/MetaMatching/utils.py
+drwxrwxr-x   0 leqi      (1000) leqi      (1000)        0 2023-04-23 07:09:04.336961 MetaMatching-1.0.1/MetaMatching.egg-info/
+-rw-rw-r--   0 leqi      (1000) leqi      (1000)      265 2023-04-23 07:09:04.000000 MetaMatching-1.0.1/MetaMatching.egg-info/PKG-INFO
+-rw-rw-r--   0 leqi      (1000) leqi      (1000)      314 2023-04-23 07:09:04.000000 MetaMatching-1.0.1/MetaMatching.egg-info/SOURCES.txt
+-rw-rw-r--   0 leqi      (1000) leqi      (1000)        1 2023-04-23 07:09:04.000000 MetaMatching-1.0.1/MetaMatching.egg-info/dependency_links.txt
+-rw-rw-r--   0 leqi      (1000) leqi      (1000)        1 2023-04-23 07:09:04.000000 MetaMatching-1.0.1/MetaMatching.egg-info/not-zip-safe
+-rw-rw-r--   0 leqi      (1000) leqi      (1000)       84 2023-04-23 07:09:04.000000 MetaMatching-1.0.1/MetaMatching.egg-info/requires.txt
+-rw-rw-r--   0 leqi      (1000) leqi      (1000)       13 2023-04-23 07:09:04.000000 MetaMatching-1.0.1/MetaMatching.egg-info/top_level.txt
+-rw-rw-r--   0 leqi      (1000) leqi      (1000)      265 2023-04-23 07:09:04.336961 MetaMatching-1.0.1/PKG-INFO
+-rw-rw-r--   0 leqi      (1000) leqi      (1000)      115 2023-04-21 07:11:30.000000 MetaMatching-1.0.1/README.rst
+-rw-rw-r--   0 leqi      (1000) leqi      (1000)       38 2023-04-23 07:09:04.336961 MetaMatching-1.0.1/setup.cfg
+-rw-rw-r--   0 leqi      (1000) leqi      (1000)      699 2023-04-23 07:08:38.000000 MetaMatching-1.0.1/setup.py
```

### Comparing `MetaMatching-0.2.3/LICENSE.txt` & `MetaMatching-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MetaMatching-0.2.3/MetaMatching/model.py` & `MetaMatching-1.0.1/MetaMatching/model.py`

 * *Files identical despite different names*

### Comparing `MetaMatching-0.2.3/MetaMatching/utils.py` & `MetaMatching-1.0.1/MetaMatching/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,22 +111,22 @@
         dat = neg
         
     new_dat = remove_rows(dat, dat.iloc[:,idx_feature:], thres = zero_threshold)
 
     # select only the compounds that are in the graph
      
     if pos is not None and neg is not None:
-        dic_pos = find_keggid(new_dat.loc[new_dat.index.str.contains('pos')], kegg_sub, pos_adductlist)
-        dic_neg = find_keggid(new_dat.loc[new_dat.index.str.contains('neg')], kegg_sub, neg_adductlist)
+        dic_pos = find_keggid(new_dat.loc[new_dat.index.str.contains('pos')], kegg_sub, pos_adductlist, match_tol_ppm)
+        dic_neg = find_keggid(new_dat.loc[new_dat.index.str.contains('neg')], kegg_sub, neg_adductlist, match_tol_ppm)
 
         dic = {**dic_pos, **dic_neg}
     elif pos is not None:
-        dic = find_keggid(new_dat.loc[new_dat.index.str.contains('pos')], kegg_sub, pos_adductlist)
+        dic = find_keggid(new_dat.loc[new_dat.index.str.contains('pos')], kegg_sub, pos_adductlist, match_tol_ppm)
     elif neg is not None:
-        dic = find_keggid(new_dat.loc[new_dat.index.str.contains('neg')], kegg_sub, neg_adductlist)
+        dic = find_keggid(new_dat.loc[new_dat.index.str.contains('neg')], kegg_sub, neg_adductlist, match_tol_ppm)
 
     data_annos, matchings, adj_matrices, metabolites = get_data(dic, new_dat, g)
     
     if log_transform:
         data_annos.iloc[:,idx_feature:] = np.log(data_annos.iloc[:,idx_feature:]+1)
         
     if scale:
```

### Comparing `MetaMatching-0.2.3/setup.py` & `MetaMatching-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # @Author : Leqi Tian
 # @File : setup.py
 
 from setuptools import setup
 from setuptools import find_packages
 
 
-VERSION = '0.2.3'
+VERSION = '1.0.1'
 
 setup(
     name='MetaMatching',  # package name
     version=VERSION,  # package version
     description='An integrated deep learning framework for the interpretation of untargeted metabolomics data',  
     packages=find_packages(),
     author='Leqi Tian',
```

