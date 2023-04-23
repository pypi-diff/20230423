# Comparing `tmp/keypartx-0.1.8.tar.gz` & `tmp/keypartx-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keypartx-0.1.8.tar", last modified: Fri Nov 11 21:34:05 2022, max compression
+gzip compressed data, was "keypartx-0.1.9.tar", last modified: Sat Nov 12 07:53:08 2022, max compression
```

## Comparing `keypartx-0.1.8.tar` & `keypartx-0.1.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2022-11-11 21:34:05.155424 keypartx-0.1.8/
--rw-rw-rw-   0        0        0       78 2022-09-16 17:01:01.000000 keypartx-0.1.8/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1049 2022-09-16 17:01:25.000000 keypartx-0.1.8/LICENCE.txt
--rw-rw-rw-   0        0        0       26 2022-09-15 17:49:29.000000 keypartx-0.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0     2927 2022-11-11 21:34:05.155424 keypartx-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      325 2022-11-11 11:26:32.000000 keypartx-0.1.8/README.txt
-drwxrwxrwx   0        0        0        0 2022-11-11 21:34:05.139351 keypartx-0.1.8/keypartx/
--rw-rw-rw-   0        0        0    32787 2022-10-29 17:52:12.000000 keypartx-0.1.8/keypartx/KeypartX.py
--rw-rw-rw-   0        0        0    28199 2022-10-16 10:54:29.000000 keypartx-0.1.8/keypartx/KeypartX_12.10.2022.py
--rw-rw-rw-   0        0        0      135 2022-11-11 21:31:34.000000 keypartx-0.1.8/keypartx/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-11 21:34:05.155424 keypartx-0.1.8/keypartx/basemodes/
--rw-rw-rw-   0        0        0      119 2022-09-18 12:26:11.000000 keypartx-0.1.8/keypartx/basemodes/__init__.py
--rw-rw-rw-   0        0        0    29467 2022-11-11 10:44:50.000000 keypartx-0.1.8/keypartx/basemodes/avn_base.py
--rw-rw-rw-   0        0        0    13620 2022-11-05 18:42:21.000000 keypartx-0.1.8/keypartx/basemodes/net_base.py
--rw-rw-rw-   0        0        0    33775 2022-11-11 09:26:42.000000 keypartx-0.1.8/keypartx/basemodes/text_edges.py
-drwxrwxrwx   0        0        0        0 2022-11-11 21:34:05.155424 keypartx-0.1.8/keypartx.egg-info/
--rw-rw-rw-   0        0        0     2927 2022-11-11 21:34:04.000000 keypartx-0.1.8/keypartx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      416 2022-11-11 21:34:05.000000 keypartx-0.1.8/keypartx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-11 21:34:04.000000 keypartx-0.1.8/keypartx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      133 2022-11-11 21:34:04.000000 keypartx-0.1.8/keypartx.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-11-11 21:34:04.000000 keypartx-0.1.8/keypartx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-11-11 21:34:05.155424 keypartx-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1214 2022-11-11 21:33:12.000000 keypartx-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-11-12 07:53:08.948666 keypartx-0.1.9/
+-rw-rw-rw-   0        0        0       78 2022-09-16 17:01:01.000000 keypartx-0.1.9/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1049 2022-09-16 17:01:25.000000 keypartx-0.1.9/LICENCE.txt
+-rw-rw-rw-   0        0        0       26 2022-09-15 17:49:29.000000 keypartx-0.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     3000 2022-11-12 07:53:08.948666 keypartx-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      325 2022-11-11 11:26:32.000000 keypartx-0.1.9/README.txt
+drwxrwxrwx   0        0        0        0 2022-11-12 07:53:08.917414 keypartx-0.1.9/keypartx/
+-rw-rw-rw-   0        0        0    33629 2022-11-11 22:41:18.000000 keypartx-0.1.9/keypartx/KeypartX.py
+-rw-rw-rw-   0        0        0    28199 2022-10-16 10:54:29.000000 keypartx-0.1.9/keypartx/KeypartX_12.10.2022.py
+-rw-rw-rw-   0        0        0      135 2022-11-11 22:52:13.000000 keypartx-0.1.9/keypartx/__init__.py
+drwxrwxrwx   0        0        0        0 2022-11-12 07:53:08.933060 keypartx-0.1.9/keypartx/basemodes/
+-rw-rw-rw-   0        0        0      119 2022-09-18 12:26:11.000000 keypartx-0.1.9/keypartx/basemodes/__init__.py
+-rw-rw-rw-   0        0        0    29467 2022-11-11 10:44:50.000000 keypartx-0.1.9/keypartx/basemodes/avn_base.py
+-rw-rw-rw-   0        0        0    13620 2022-11-05 18:42:21.000000 keypartx-0.1.9/keypartx/basemodes/net_base.py
+-rw-rw-rw-   0        0        0    33775 2022-11-11 09:26:42.000000 keypartx-0.1.9/keypartx/basemodes/text_edges.py
+drwxrwxrwx   0        0        0        0 2022-11-12 07:53:08.933060 keypartx-0.1.9/keypartx.egg-info/
+-rw-rw-rw-   0        0        0     3000 2022-11-12 07:53:08.000000 keypartx-0.1.9/keypartx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      416 2022-11-12 07:53:08.000000 keypartx-0.1.9/keypartx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-11-12 07:53:08.000000 keypartx-0.1.9/keypartx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      133 2022-11-12 07:53:08.000000 keypartx-0.1.9/keypartx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2022-11-12 07:53:08.000000 keypartx-0.1.9/keypartx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-11-12 07:53:08.948666 keypartx-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1214 2022-11-11 23:23:21.000000 keypartx-0.1.9/setup.py
```

### Comparing `keypartx-0.1.8/LICENCE.txt` & `keypartx-0.1.9/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `keypartx-0.1.8/PKG-INFO` & `keypartx-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keypartx
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Graph-based Perception(Text) Representation
 Home-page: https://github.com/pengKiina/KeypartX
 Author: Peng Yang
 Author-email: pyseptimo@outlook.com
 License: MIT
 Keywords: text representation,text mining,nlp,topic modeling,emoji,image,perception
 Classifier: Development Status :: 5 - Production/Stable
@@ -32,15 +32,15 @@
  pip install keypartx  
  python -m spacy download en_core_web_lg
 ```
 
 
 ## Getting Started
 For an in-depth overview of the features of KeypartX
-you can check the [**Documents**](https://mr./) or you can follow along 
+you can check the [**Documents**](https://medium.com/@egalitrans/topic-modeling-is-dead-long-live-keypartx-a1998a94a0b0) or you can follow along 
 with one of the examples as follows:
 
 | Name  | Link  |
 |---|---|
 | KepartX Quick Start  | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1VdKIJtMMcYRnXsne87azY7B1FXp9FpD1?usp=sharing)  |
 | KepartX Sentence NLP | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1hjAU-_RP7GGzMm6rnpdJZR7LSY0KS81E?usp=sharing) |
 | KepartX VS Topic Modelling |  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/14XvylCMBZ2oUnjpZhnf_658paVdvAhp0?usp=sharing) |
```

### Comparing `keypartx-0.1.8/keypartx/KeypartX.py` & `keypartx-0.1.9/keypartx/KeypartX.py`

 * *Files 3% similar despite different names*

```diff
@@ -190,18 +190,19 @@
     print('processing time:', time.time()-time_start)
     print('length of reviews:',line_i)
     print('length of sentences:',sent_i)
     return all_adjV2N_edges,allNNedges,all_new_nodes,all_old_nodes,new_node_nouns,new_node_verbs,new_node_adjs,emojis1
 
 
 ## -- avn network -- ## 
-def keynet(all_edges1,heading='avN_N Network',core_K =1,plot_graph = True,save_add ="avnn.html",height='600px', width='100%',bgcolor='white',font_color="black", directed = True, notebook =True,cdn='remote'):
+def keynet(all_edges1,heading='avN_N Network',core_K =1,plot_graph = False,save_add ="network_avnn.html",height='600px', width='100%',bgcolor='white',font_color="black", directed = True, notebook =True,cdn='remote'):
     """ all_edges1: weighted edges 
         core_k: if node degree is less than k then edge droped
         cdn=['remote','local'] more in pyvis 
+        plot_graph = False for google colab 
     """
     # get Networkx 
     #import math
     Gd = nx.DiGraph() 
     #all_edges1 = all_adjV2N_edges_w + allNNEdges_dir_w
     Gd.add_weighted_edges_from(all_edges1)
     #print('length Gd nodes: ',len(Gd.nodes))
@@ -264,27 +265,31 @@
         
     print('length Gd nodes after error node removed:',len(Gd.nodes))
     print('all edges after k-core: ', len(all_edges))
     
     nt.show_buttons(filter_=['physics']) 
     if plot_graph:
         display(nt.show("network_avnn.html"))
+    else: # google colab 
+        nt.show("network_avnn.html")
+        display(HTML('network_avnn.html'))
         #display(HTML('network_avnn.html'))
     if save_add:      
         nt.save_graph(save_add)
     # all_edges after k-core of all_edges1
     return all_edges,Gd
 
 
 
 ## -- avn network colored by community 
-def communet(partition,iGd,Gdc,all_edges,colorList_rgba1,plot_graph = True,save_add ="network_community.html",height='600px', width='100%',heading='Community Network', directed = True, notebook =True,cdn='remote'):
+def communet(partition,iGd,Gdc,all_edges,colorList_rgba1,plot_graph = False,save_add ="network_community.html",height='600px', width='100%',heading='Community Network', directed = True, notebook =True,cdn='remote'):
     #import matplotlib
     """ 
         cdn=['remote','local'] more in pyvis 
+        plot_graph = False for google colab 
     """
     #from itertools import cycle, islice
     colorList1  = list(islice(cycle(colorList_rgba1),len(partition)))
 
     ntc=Network(height=height, width=width,heading=heading,bgcolor='white',font_color="black", directed = directed, notebook =notebook ,cdn_resources=cdn)
     ntc.set_edge_smooth('cubicBezier')
     #error_noeds =[]
@@ -323,28 +328,31 @@
       
       edge0 = re.sub(r'[2][a-zA-Z]{2}',"2",edge[0])
       edge1 = re.sub(r'[2][a-zA-Z]{2}',"2",edge[1])
       ntc.add_edge(edge0,edge1, title = elabel,width = value)
       #ntc.add_edge(edge[0][:-2],edge[1][:-2], title = elabel,width = value)
     ntc.show_buttons(filter_=['physics']) 
     if plot_graph:
-         
         display(ntc.show('community_network.html'))
         #display(HTML('community_network.html'))
+    else: # google colab
+        ntc.show("community_network.html")
+        display(HTML('community_network.html'))      
     if save_add:
         ntc.save_graph(save_add)
         
 
 
 ## --plot color by nouns in AVNN community --#
 
-def communet_nnc(partition,iGd,Gdc,all_edges,colorList_rgba1,plot_graph = True,save_add = 'community_NNColors.html', height='600px', width='100%',heading='Community_NNColors',bgcolor='white',font_color="black", directed = True, notebook =True,cdn='remote'):
+def communet_nnc(partition,iGd,Gdc,all_edges,colorList_rgba1,plot_graph = False,save_add = 'community_NNColors.html', height='600px', width='100%',heading='Community_NNColors',bgcolor='white',font_color="black", directed = True, notebook =True,cdn='remote'):
     #import matplotlib,itertools
     """ 
         cdn=['remote','local'] more in pyvis 
+        plot_graph = False for google colab 
     """
     partition_all_names = [] 
     for index in partition:
         partition_all_names.append([iGd.vs[index]['name'] for index in index])
 
     #list2d_all =  [x for x in partition_all_names]
     #all_nodes_index =  list(itertools.chain(*list2d_all))
@@ -442,14 +450,17 @@
       ntc2.add_edge(edge0,edge1, title = elabel,width = value)
 
       #ntc2.add_edge(edge[0][:-2],edge[1][:-2], title = elabel,width = value)
     ntc2.show_buttons(filter_=['physics']) 
     if plot_graph:
         display(ntc2.show('communityNNcolor.html'))
         #display(HTML('communityNNcolor.html'))
+    else:# google colab
+        ntc2.show("communityNNcolor.html")
+        display(HTML('communityNNcolor.html'))      
     if save_add:
         ntc2.save_graph(save_add)
 
     com_dict = []
     for com, edges,nodes in  zip(com_aa,com_edges,com_nodes):
         for edge,node in zip(edges,nodes):
             dict1 = {'community_nn':com,'edges':edge,'node':node}
@@ -459,14 +470,15 @@
 
 
 
 ## -single community with gray connection -## 
 def gray_unit(nnColor_df,Gdc,all_edges,comLen = False,plot_graph = False, save_folder='gray_units/',height='600px', width='100%',heading='Gray Unit Community Network',bgcolor='white',font_color="black", directed = True, notebook =True,cdn='remote'):
     """ 
         cdn=['remote','local'] more in pyvis 
+        plot_graph = False for google colab 
     """    
     
     if comLen == False:
         com_len = len(set(nnColor_df.community_nn.to_list()))
     else:
         com_len = comLen
     
@@ -546,14 +558,17 @@
             ntc3.add_edge(edge0,edge1, title = elabel,width = value)
             #ntc3.add_edge(edge[0][:-2],edge[1][:-2], title = elabel,width = value)
       ntc3.show_buttons(filter_=['physics'])
       if plot_graph:
         if community_index == com_len-1: 
             display(ntc3.show(str(community_index) + '_gray_unit.html'))
             #display(HTML(str(community_index) + '_gray_unit.html'))
+      else:
+             ntc3.show(str(community_index) + '_gray_unit.html')
+             display(HTML(str(community_index) + '_gray_unit.html'))       
       if save_folder:
         ntc3.save_graph(save_folder+ '/{}.html'.format(community_index +1))
 
       # gray_color edges dataframe 
       gray_nodes = [x for x in comNodes if x not in comNodes_ori]
       gray_edges = []
       color_edges = []
@@ -591,19 +606,19 @@
       colorNodes.append(set(colorNodeDs))
       grayEdges.append(set(gray_edges))
       grayNodes.append(set(grayNodeDs))
     colorGrayDF = pd.DataFrame({'commus': commus,'colorEdges':colorEdges,'colorNodes':colorNodes,'grayEdges':grayEdges,'grayNodes':grayNodes})
     return colorGrayDF
   
 
-def compare_net(allWedges, weight_K=1, specEdges1 = False,specEdges2 = False, specNodes1=False,specNodes2=False, color1= 'red', color2 = 'green', save_add = False,heading = 'Compared Network',core_K = 1 , plot_graph = True, height='600px',width='100%',bgcolor='white', font_color="black",directed = True,notebook =True,cdn='remote'):
+def compare_net(allWedges, weight_K=1, specEdges1 = False,specEdges2 = False, specNodes1=False,specNodes2=False, color1= 'red', color2 = 'green', save_add = False,heading = 'Compared Network',core_K = 1 , plot_graph = False, height='600px',width='100%',bgcolor='white', font_color="black",directed = True,notebook =True,cdn='remote'):
     """ 
     allWEdges  of list of weighted edges including SharedA, ShareB, SpecificA, SpecificB edges 
     if specedge or specnodes False, color1 , color2 do not work all show gray color
-    
+    plot_graph = False for google colab 
     """
     nt=Network(heading=heading, height=height, width=width,bgcolor=bgcolor,font_color=font_color, directed = directed, notebook =notebook,cdn_resources=cdn)
     nt.set_edge_smooth('cubicBezier')
     allWedges1 = []
     for wedge in allWedges:
         if wedge[2]>= weight_K:
             allWedges1.append(wedge)
@@ -703,14 +718,17 @@
         all_edges.append(edge)
 
     nt.show_buttons(filter_=['physics']) 
     if save_add:
         nt.save_graph(save_add) 
     if plot_graph:
         display(nt.show("compare_avnn.html"))
+    else: # google colab
+        nt.show("compare_avnn.html")
+        display(HTML('compare_avnn.html'))
 
     return all_nodes, specNodes1_new,specNodes2_new ,all_edges,  specEdges1new,specEdges2new
 
   
   
   
 if __name__ == "__main__":
```

### Comparing `keypartx-0.1.8/keypartx/KeypartX_12.10.2022.py` & `keypartx-0.1.9/keypartx/KeypartX_12.10.2022.py`

 * *Files identical despite different names*

### Comparing `keypartx-0.1.8/keypartx/basemodes/avn_base.py` & `keypartx-0.1.9/keypartx/basemodes/avn_base.py`

 * *Files identical despite different names*

### Comparing `keypartx-0.1.8/keypartx/basemodes/net_base.py` & `keypartx-0.1.9/keypartx/basemodes/net_base.py`

 * *Files identical despite different names*

### Comparing `keypartx-0.1.8/keypartx/basemodes/text_edges.py` & `keypartx-0.1.9/keypartx/basemodes/text_edges.py`

 * *Files identical despite different names*

### Comparing `keypartx-0.1.8/keypartx.egg-info/PKG-INFO` & `keypartx-0.1.9/keypartx.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keypartx
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Graph-based Perception(Text) Representation
 Home-page: https://github.com/pengKiina/KeypartX
 Author: Peng Yang
 Author-email: pyseptimo@outlook.com
 License: MIT
 Keywords: text representation,text mining,nlp,topic modeling,emoji,image,perception
 Classifier: Development Status :: 5 - Production/Stable
@@ -32,15 +32,15 @@
  pip install keypartx  
  python -m spacy download en_core_web_lg
 ```
 
 
 ## Getting Started
 For an in-depth overview of the features of KeypartX
-you can check the [**Documents**](https://mr./) or you can follow along 
+you can check the [**Documents**](https://medium.com/@egalitrans/topic-modeling-is-dead-long-live-keypartx-a1998a94a0b0) or you can follow along 
 with one of the examples as follows:
 
 | Name  | Link  |
 |---|---|
 | KepartX Quick Start  | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1VdKIJtMMcYRnXsne87azY7B1FXp9FpD1?usp=sharing)  |
 | KepartX Sentence NLP | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1hjAU-_RP7GGzMm6rnpdJZR7LSY0KS81E?usp=sharing) |
 | KepartX VS Topic Modelling |  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/14XvylCMBZ2oUnjpZhnf_658paVdvAhp0?usp=sharing) |
```

### Comparing `keypartx-0.1.8/setup.py` & `keypartx-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-version = '0.1.8'
+version = '0.1.9'
 
 
 base_packages = ['networkx','leidenalg','autocorrect','autocorrect','xlsxwriter','igraph','matplotlib','numpy','emoji']
 classifiers = [
   'Development Status :: 5 - Production/Stable',
   'Intended Audience :: Education',
   'Operating System :: Microsoft :: Windows :: Windows 10',
```

