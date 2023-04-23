# Comparing `tmp/cotat-0.1.0.tar.gz` & `tmp/cotat-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cotat-0.1.0.tar", last modified: Thu Aug  4 01:43:25 2022, max compression
+gzip compressed data, was "cotat-0.2.0.tar", last modified: Sun Apr 23 17:52:26 2023, max compression
```

## Comparing `cotat-0.1.0.tar` & `cotat-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 Henry      (501) staff       (20)        0 2022-08-04 01:43:25.729465 cotat-0.1.0/
--rw-r--r--   0 Henry      (501) staff       (20)     1083 2022-04-20 01:33:47.000000 cotat-0.1.0/LICENSE
--rw-r--r--   0 Henry      (501) staff       (20)       59 2022-04-17 22:07:10.000000 cotat-0.1.0/MANIFEST.in
--rw-r--r--   0 Henry      (501) staff       (20)     2014 2022-08-04 01:43:25.729165 cotat-0.1.0/PKG-INFO
--rw-r--r--   0 Henry      (501) staff       (20)     1333 2022-08-04 01:37:17.000000 cotat-0.1.0/README.md
-drwxr-xr-x   0 Henry      (501) staff       (20)        0 2022-08-04 01:43:25.724659 cotat-0.1.0/cotat/
--rw-r--r--   0 Henry      (501) staff       (20)      108 2022-04-16 22:05:13.000000 cotat-0.1.0/cotat/__init__.py
--rw-r--r--   0 Henry      (501) staff       (20)    10705 2022-04-19 18:45:27.000000 cotat-0.1.0/cotat/cotat.py
-drwxr-xr-x   0 Henry      (501) staff       (20)        0 2022-08-04 01:43:25.727777 cotat-0.1.0/cotat/resources/
--rw-r--r--   0 Henry      (501) staff       (20)      222 2022-04-17 21:52:16.000000 cotat-0.1.0/cotat/resources/button.js
--rw-r--r--   0 Henry      (501) staff       (20)      840 2022-04-17 22:00:21.000000 cotat-0.1.0/cotat/resources/instructions.html
--rw-r--r--   0 Henry      (501) staff       (20)      546 2022-04-17 21:52:42.000000 cotat-0.1.0/cotat/resources/search.js
-drwxr-xr-x   0 Henry      (501) staff       (20)        0 2022-08-04 01:43:25.728551 cotat-0.1.0/cotat/tests/
--rw-------   0 Henry      (501) staff       (20)        0 2022-04-16 22:13:15.000000 cotat-0.1.0/cotat/tests/__init__.py
--rw-r--r--   0 Henry      (501) staff       (20)      725 2022-04-19 18:45:15.000000 cotat-0.1.0/cotat/tests/test_cotat.py
-drwxr-xr-x   0 Henry      (501) staff       (20)        0 2022-08-04 01:43:25.726387 cotat-0.1.0/cotat.egg-info/
--rw-r--r--   0 Henry      (501) staff       (20)     2014 2022-08-04 01:43:25.000000 cotat-0.1.0/cotat.egg-info/PKG-INFO
--rw-r--r--   0 Henry      (501) staff       (20)      351 2022-08-04 01:43:25.000000 cotat-0.1.0/cotat.egg-info/SOURCES.txt
--rw-r--r--   0 Henry      (501) staff       (20)        1 2022-08-04 01:43:25.000000 cotat-0.1.0/cotat.egg-info/dependency_links.txt
--rw-r--r--   0 Henry      (501) staff       (20)      107 2022-08-04 01:43:25.000000 cotat-0.1.0/cotat.egg-info/requires.txt
--rw-r--r--   0 Henry      (501) staff       (20)        6 2022-08-04 01:43:25.000000 cotat-0.1.0/cotat.egg-info/top_level.txt
--rw-r--r--   0 Henry      (501) staff       (20)       38 2022-08-04 01:43:25.729610 cotat-0.1.0/setup.cfg
--rw-r--r--   0 Henry      (501) staff       (20)     1212 2022-08-04 01:34:42.000000 cotat-0.1.0/setup.py
+drwxr-xr-x   0 hwr        (501) staff       (20)        0 2023-04-23 17:52:26.184843 cotat-0.2.0/
+-rw-r--r--   0 hwr        (501) staff       (20)     1083 2022-04-20 01:33:47.000000 cotat-0.2.0/LICENSE
+-rw-r--r--   0 hwr        (501) staff       (20)       59 2022-04-17 22:07:10.000000 cotat-0.2.0/MANIFEST.in
+-rw-r--r--   0 hwr        (501) staff       (20)     2122 2023-04-23 17:52:26.184604 cotat-0.2.0/PKG-INFO
+-rw-r--r--   0 hwr        (501) staff       (20)     1441 2022-08-04 01:44:50.000000 cotat-0.2.0/README.md
+drwxr-xr-x   0 hwr        (501) staff       (20)        0 2023-04-23 17:52:26.180403 cotat-0.2.0/cotat/
+-rw-r--r--   0 hwr        (501) staff       (20)      108 2022-04-16 22:05:13.000000 cotat-0.2.0/cotat/__init__.py
+-rw-r--r--   0 hwr        (501) staff       (20)    12245 2023-04-23 17:48:53.000000 cotat-0.2.0/cotat/cotat.py
+drwxr-xr-x   0 hwr        (501) staff       (20)        0 2023-04-23 17:52:26.183429 cotat-0.2.0/cotat/resources/
+-rw-r--r--   0 hwr        (501) staff       (20)      222 2022-04-17 21:52:16.000000 cotat-0.2.0/cotat/resources/button.js
+-rw-r--r--   0 hwr        (501) staff       (20)     1065 2022-08-04 20:29:25.000000 cotat-0.2.0/cotat/resources/instructions.html
+-rw-r--r--   0 hwr        (501) staff       (20)      546 2022-04-17 21:52:42.000000 cotat-0.2.0/cotat/resources/search.js
+drwxr-xr-x   0 hwr        (501) staff       (20)        0 2023-04-23 17:52:26.184194 cotat-0.2.0/cotat/tests/
+-rw-------   0 hwr        (501) staff       (20)        0 2022-04-16 22:13:15.000000 cotat-0.2.0/cotat/tests/__init__.py
+-rw-r--r--   0 hwr        (501) staff       (20)      725 2022-04-19 18:45:15.000000 cotat-0.2.0/cotat/tests/test_cotat.py
+drwxr-xr-x   0 hwr        (501) staff       (20)        0 2023-04-23 17:52:26.182068 cotat-0.2.0/cotat.egg-info/
+-rw-r--r--   0 hwr        (501) staff       (20)     2122 2023-04-23 17:52:26.000000 cotat-0.2.0/cotat.egg-info/PKG-INFO
+-rw-r--r--   0 hwr        (501) staff       (20)      351 2023-04-23 17:52:26.000000 cotat-0.2.0/cotat.egg-info/SOURCES.txt
+-rw-r--r--   0 hwr        (501) staff       (20)        1 2023-04-23 17:52:26.000000 cotat-0.2.0/cotat.egg-info/dependency_links.txt
+-rw-r--r--   0 hwr        (501) staff       (20)      105 2023-04-23 17:52:26.000000 cotat-0.2.0/cotat.egg-info/requires.txt
+-rw-r--r--   0 hwr        (501) staff       (20)        6 2023-04-23 17:52:26.000000 cotat-0.2.0/cotat.egg-info/top_level.txt
+-rw-r--r--   0 hwr        (501) staff       (20)       38 2023-04-23 17:52:26.184908 cotat-0.2.0/setup.cfg
+-rw-r--r--   0 hwr        (501) staff       (20)     1210 2023-04-23 17:39:16.000000 cotat-0.2.0/setup.py
```

### Comparing `cotat-0.1.0/LICENSE` & `cotat-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cotat-0.1.0/PKG-INFO` & `cotat-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cotat
-Version: 0.1.0
+Version: 0.2.0
 Home-page: https://github.com/cornell-covid-modeling/cotat
 Author: Cornell Covid Modeling Team
 Author-email: hwr26@cornell.edu
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -15,14 +15,15 @@
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # <img alt="cotat" src="docs/branding/cotat_color.png" height="90">
 
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/cotat.svg)](https://pypi.python.org/pypi/cotat/)
 [![CircleCI](https://circleci.com/gh/cornell-covid-modeling/cotat/tree/master.svg?style=shield&circle-token=97897740e926742355ec6f2809bb29815c07a1fb)](https://circleci.com/gh/cornell-covid-modeling/cotat/tree/master)
 [![Documentation Status](https://readthedocs.org/projects/cotat/badge/?version=latest)](https://cotat.henryrobbins.com/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/cornell-covid-modeling/cotat/branch/master/graph/badge.svg?token=59BOEOE7TB)](https://codecov.io/gh/cornell-covid-modeling/cotat)
 
 cotat is a visualization tool for the analysis of contact tracing data. Given
 a dataframe of people (along with their attributes) and a dataframe of
 known contacts among the individuals, cotat exports an interactive HTML
```

### Comparing `cotat-0.1.0/README.md` & `cotat-0.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # <img alt="cotat" src="docs/branding/cotat_color.png" height="90">
 
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/cotat.svg)](https://pypi.python.org/pypi/cotat/)
 [![CircleCI](https://circleci.com/gh/cornell-covid-modeling/cotat/tree/master.svg?style=shield&circle-token=97897740e926742355ec6f2809bb29815c07a1fb)](https://circleci.com/gh/cornell-covid-modeling/cotat/tree/master)
 [![Documentation Status](https://readthedocs.org/projects/cotat/badge/?version=latest)](https://cotat.henryrobbins.com/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/cornell-covid-modeling/cotat/branch/master/graph/badge.svg?token=59BOEOE7TB)](https://codecov.io/gh/cornell-covid-modeling/cotat)
 
 cotat is a visualization tool for the analysis of contact tracing data. Given
 a dataframe of people (along with their attributes) and a dataframe of
 known contacts among the individuals, cotat exports an interactive HTML
```

### Comparing `cotat-0.1.0/cotat/cotat.py` & `cotat-0.2.0/cotat/cotat.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from typing import List
 
 # bokeh imports
 from bokeh.plotting import figure, output_file, save
 from bokeh.layouts import row, gridplot
 from bokeh.plotting import from_networkx
 from bokeh.models import (HoverTool, ColumnDataSource, LabelSet, TextInput,
-                          Div, Button, CustomJS, Circle, MultiLine,
-                          Panel, Tabs)
+                          Div, Button, CustomJS, Circle, MultiLine, TabPanel,
+                          Tabs)
 
 # =============================
 # CONSTANTS
 # =============================
 
 GRAPH_PLOT_HEIGHT = 700
 GRAPH_PLOT_WIDTH = 1500
@@ -49,14 +49,49 @@
                    .decode().format(**globals())
 INSTRUCTIONS_HTML = pkgutil.get_data(__name__, "resources/instructions.html") \
                            .decode().format(**globals())
 
 # =============================
 
 
+def _prune(nodes_df: pd.DataFrame, edges_df: pd.DataFrame,
+           start: datetime.date, end: datetime.date) -> List[pd.DataFrame]:
+    """Return only the nodes and edges relevant to the given time range.
+
+    The nodes infected during
+
+    Args:
+        nodes_df (pd.DataFrame): The full set of nodes.
+        edges_df (pd.DataFrame): The full set of edges.
+        start (datetime.date): The start date of the time range.
+        end (datetime.date): The end data of the time range.
+
+    Returns:
+        List[pd.DataFrame]: The pruned dataframes of nodes and edges.
+    """
+    infected_df = nodes_df[~nodes_df.date.isna()]
+    infected_in_range = list(infected_df[(start <= infected_df.date) &
+                                         (infected_df.date <= end)].index)
+
+    nodes = infected_in_range
+    edges = []
+    for i,j in edges_df.apply(lambda x: (x.source, x.target), axis=1):
+        if i in infected_in_range and j not in nodes:
+            nodes.append(j)
+            edges.append((i,j))
+        elif j in infected_in_range and i not in nodes:
+            nodes.append(i)
+            edges.append((i,j))
+
+    pruned_nodes_df = nodes_df.loc[nodes]
+    pruned_edges_df = pd.DataFrame([{"source":i, "target":j} for i,j in edges])
+
+    return pruned_nodes_df, pruned_edges_df
+
+
 def _contact_graph(nodes: pd.DataFrame, edges: pd.DataFrame,
                    membership_cols: List[str] = []) -> nx.Graph:
     """Return a graph representing the contact tracing data.
 
     Edges are given an "edge_type" attribute which is "contact" for contact
     tracing data. For each membership column, edges are added between nodes
     that are members of the same group. The "edge_type" of these edges is the
@@ -77,18 +112,16 @@
 
     # edge attributes
     edges["dummy"] = 0
     edges["edge_type"] = "contact"
     G = nx.from_pandas_edgelist(edges, edge_attr=["dummy", "edge_type"])
 
     # node attributes
-    nodes = nodes.reset_index().rename(columns={'index': 'id'})
-    G.add_nodes_from(nodes["id"])
-    node_attr = nodes.set_index("id").to_dict("index")
-    nx.set_node_attributes(G, node_attr)
+    G.add_nodes_from(list(nodes.index))
+    nx.set_node_attributes(G, nodes.to_dict("index"))
 
     # add membership dummy edges
     for membership_col in membership_cols:
         groups = nodes[membership_col].value_counts().to_dict()
         for group, n in groups.items():
             if group != "" and n > 1:
                 members = list(nodes[nodes[membership_col] == group].index)
@@ -97,19 +130,19 @@
                         if i < j and not G.has_edge(members[i], members[j]):
                             G.add_edge(members[i], members[j], dummy=1,
                                        edge_type=membership_col)
 
     return G
 
 
-def _blank_plot(name, plot_height, plot_width):
+def _blank_plot(name, height, width):
     """Create a blank plot with default configurations set."""
     plot = figure(title=name,
-                  plot_width=plot_width,
-                  plot_height=plot_height,
+                  width=width,
+                  height=height,
                   tools="pan, wheel_zoom, box_zoom, reset")
     plot.toolbar.logo = None
     plot.xgrid.grid_line_color = None
     plot.ygrid.grid_line_color = None
     plot.xaxis.visible = False
     plot.yaxis.visible = False
     plot.background_fill_color = None
@@ -139,28 +172,27 @@
     pos_dict = nx.get_node_attributes(G, "pos")
     pos = [pos_dict[id] for id in ids]
     x, y = list(zip(*pos))
     case_labels = ColumnDataSource(data={"x": x, "y": y, "case": case})
     return LabelSet(x="x", y="y", text="case",
                     x_offset=LABEL_OFFSET, y_offset=LABEL_OFFSET,
                     text_font_size=LABEL_TEXT_SIZE,
-                    source=case_labels, render_mode="canvas")
+                    source=case_labels)
 
 
 def _hover_labels(G, graph_renderer, attributes):
     """Add hover labels to plot."""
     tooltips = [(attr, f"@{attr}") for attr in attributes]
     return HoverTool(tooltips=tooltips,
                      renderers=[graph_renderer.node_renderer])
 
 
 def _tab(title, tab_name, G, attributes):
     """Return a tab (Panel) showing graph G of nodes"""
-    p = _blank_plot(f"{title}: {tab_name}", GRAPH_PLOT_HEIGHT,
-                    GRAPH_PLOT_WIDTH)
+    p = _blank_plot(title, GRAPH_PLOT_HEIGHT, GRAPH_PLOT_WIDTH)
     graph_renderer = _graph_renderer(G)
     p.renderers.append(graph_renderer)
     p.add_layout(_case_labels(G))
     p.tools.append(_hover_labels(G, graph_renderer, attributes))
 
     # add custom JS to button and search bar
     node_source = graph_renderer.node_renderer.data_source
@@ -169,18 +201,20 @@
     text_input = TextInput(value="case_number", title="Search Case:")
     text_input.js_on_change("value", CustomJS(args={"source": node_source},
                                               code=SEARCH_JS))
 
     # aggregate plot
     plot = gridplot([[p],
                      [row(text_input, button, sizing_mode="stretch_both")],
-                     [Div(text=INSTRUCTIONS_HTML)]],
+                     [Div(text=INSTRUCTIONS_HTML,
+                          styles={"overflow-wrap": "break-word",
+                                  "width": f"{INSTRUCTIONS_PLOT_WIDTH}px"})]],
                     toolbar_options={'logo': None})
 
-    return Panel(child=plot, title=tab_name)
+    return TabPanel(child=plot, title=tab_name)
 
 
 def visualization(title: str, file_name: str, nodes: pd.DataFrame,
                   edges: pd.DataFrame, start: datetime.date,
                   end: datetime.date, membership_cols: List[str] = []):
     """Write an HTML visualization of the given contact tracing graph.
 
@@ -200,14 +234,16 @@
             leading up to this data as inactive (blue) on the visualization).
         end (datetime.date): End date (show cases after this data as inactive \
             (blue) on the visualization).
         membership_cols (List[str]): List of columns recognized as memberships.
     """
     attributes = nodes.columns
 
+    # prune and initialize contact graph
+    nodes, edges = _prune(nodes, edges, start, end)
     G = _contact_graph(nodes, edges, membership_cols)
 
     # set node color of positive cases
     nx.set_node_attributes(G, values=9, name='size')
 
     offset = 14  # days (2 weeks)
     alphas = list(np.linspace(0.5, 1, (end - start).days + offset + 1))
@@ -237,14 +273,20 @@
     for contact, dummy, name in edge_attributes:
         alpha = {k:{0:contact, 1:dummy}[v] for k,v in dummy_attribute}
         nx.set_edge_attributes(G, values=alpha, name=name)
 
     pos = nx.spring_layout(G, k=0.13, weight="weight", seed=1, iterations=150)
     nx.set_node_attributes(G, pos, "pos")
 
+    # Add date range to title
+    date_format = r'%-m/%-d/%Y'
+    start_str = start.strftime(date_format)
+    end_str = end.strftime(date_format)
+    title = f"{title} [{start_str} - {end_str}]"
+
     # all edges
     edge_alpha = {k:{0:EDGE_ALPHA_CONTACT, 1:EDGE_ALPHA_DUMMY}[v]
                   for k,v in dummy_attribute}
     nx.set_edge_attributes(G, values=edge_alpha, name="alpha")
     tab1 = _tab(title, "All", G, attributes)
 
     # only contact edges
```

### Comparing `cotat-0.1.0/cotat/resources/instructions.html` & `cotat-0.2.0/cotat/resources/instructions.html`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 <b>Instructions:</b><br>
-Red nodes are positive cases within the last 2 weeks; they are labeled with
-their case number. Furthermore, the opacity of the node decreases as the time
-since they tested positive increases, ranging from 1 (today) to 0.5 (2 weeks
-ago). All other nodes are blue. Solid edges indicate a contact trace.  Dashed
-edges indicate the two nodes are a member of the same group. Use the tabs to
-toggle on and off edges by type. Hover over a node for more information. Search
-for a case number by typing into the search box above and pressing enter. If
-the case is found, it will be enlarged. To reset the search, press the reset
-button. Use the toolbar in the top right to navigate the graph. A blue line
-indicates the tool is active. Contact Henry Robbins (<a
-href="mailto:hwr26@cornell.edu">hwr26</a>) with any questions.
+Every node represents someone who was (a) infected in the given date range, (b)
+identified a type (a) node as a contact, or (c) were identified by a type (a)
+node as a contact. Red nodes are positive cases in the date range or the two
+weeks leading up to the start date; they are labeled with their case number.
+Furthermore, the opacity of the node decreases as the time since they tested
+positive increases, ranging from 1 (today) to 0.5 (>2 weeks ago). All other
+nodes are blue. Solid edges indicate a contact trace.  Dashed edges indicate
+the two nodes are a affiliated with the same group. Use the tabs to toggle on
+and off edges by type. Hover over a node for more information.  Search for a
+case number by typing into the search box above and pressing enter. If the case
+is found, it will be enlarged. To reset the search, press the reset button. Use
+the toolbar in the top right to navigate the graph. A blue line indicates the
+tool is active. Contact Henry Robbins
+(<a href="mailto:hwr26@cornell.edu">hwr26</a>) with any questions.
```

#### html2text {}

```diff
@@ -1,11 +1,14 @@
 Instructions:
-Red nodes are positive cases within the last 2 weeks; they are labeled with
-their case number. Furthermore, the opacity of the node decreases as the time
-since they tested positive increases, ranging from 1 (today) to 0.5 (2 weeks
-ago). All other nodes are blue. Solid edges indicate a contact trace. Dashed
-edges indicate the two nodes are a member of the same group. Use the tabs to
-toggle on and off edges by type. Hover over a node for more information. Search
-for a case number by typing into the search box above and pressing enter. If
-the case is found, it will be enlarged. To reset the search, press the reset
-button. Use the toolbar in the top right to navigate the graph. A blue line
-indicates the tool is active. Contact Henry Robbins (hwr26) with any questions.
+Every node represents someone who was (a) infected in the given date range, (b)
+identified a type (a) node as a contact, or (c) were identified by a type (a)
+node as a contact. Red nodes are positive cases in the date range or the two
+weeks leading up to the start date; they are labeled with their case number.
+Furthermore, the opacity of the node decreases as the time since they tested
+positive increases, ranging from 1 (today) to 0.5 (>2 weeks ago). All other
+nodes are blue. Solid edges indicate a contact trace. Dashed edges indicate the
+two nodes are a affiliated with the same group. Use the tabs to toggle on and
+off edges by type. Hover over a node for more information. Search for a case
+number by typing into the search box above and pressing enter. If the case is
+found, it will be enlarged. To reset the search, press the reset button. Use
+the toolbar in the top right to navigate the graph. A blue line indicates the
+tool is active. Contact Henry Robbins (hwr26) with any questions.
```

### Comparing `cotat-0.1.0/cotat/resources/search.js` & `cotat-0.2.0/cotat/resources/search.js`

 * *Files identical despite different names*

### Comparing `cotat-0.1.0/cotat/tests/test_cotat.py` & `cotat-0.2.0/cotat/tests/test_cotat.py`

 * *Files identical despite different names*

### Comparing `cotat-0.1.0/cotat.egg-info/PKG-INFO` & `cotat-0.2.0/cotat.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cotat
-Version: 0.1.0
+Version: 0.2.0
 Home-page: https://github.com/cornell-covid-modeling/cotat
 Author: Cornell Covid Modeling Team
 Author-email: hwr26@cornell.edu
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -15,14 +15,15 @@
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # <img alt="cotat" src="docs/branding/cotat_color.png" height="90">
 
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/cotat.svg)](https://pypi.python.org/pypi/cotat/)
 [![CircleCI](https://circleci.com/gh/cornell-covid-modeling/cotat/tree/master.svg?style=shield&circle-token=97897740e926742355ec6f2809bb29815c07a1fb)](https://circleci.com/gh/cornell-covid-modeling/cotat/tree/master)
 [![Documentation Status](https://readthedocs.org/projects/cotat/badge/?version=latest)](https://cotat.henryrobbins.com/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/cornell-covid-modeling/cotat/branch/master/graph/badge.svg?token=59BOEOE7TB)](https://codecov.io/gh/cornell-covid-modeling/cotat)
 
 cotat is a visualization tool for the analysis of contact tracing data. Given
 a dataframe of people (along with their attributes) and a dataframe of
 known contacts among the individuals, cotat exports an interactive HTML
```

### Comparing `cotat-0.1.0/setup.py` & `cotat-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="cotat",
-    version="0.1.0",
+    version="0.2.0",
     author="Cornell Covid Modeling Team",
     author_email="hwr26@cornell.edu",
     description="",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cornell-covid-modeling/cotat",
     packages=find_packages(),
@@ -24,15 +24,15 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
         "numpy>=1.20",
         "pandas>=1.2",
         "networkx>=2.5",
-        "bokeh>=2.3"
+        "bokeh>=3"
     ],
     extras_require={
         "dev": ['pytest>=5',
                 'mock>=3',
                 'coverage>=4.5',
                 'tox>=3',
                 "flake8>=3.9"]
```

