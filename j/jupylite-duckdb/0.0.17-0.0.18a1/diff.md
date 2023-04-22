# Comparing `tmp/jupylite_duckdb-0.0.17-py3-none-any.whl.zip` & `tmp/jupylite_duckdb-0.0.18a1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 7006 bytes, number of entries: 10
+Zip file size: 7302 bytes, number of entries: 10
 -rw-rw-rw-  2.0 fat      128 b- defN 23-Apr-21 01:44 jupylite_duckdb/__init__.py
--rw-rw-rw-  2.0 fat       22 b- defN 23-Apr-22 17:31 jupylite_duckdb/_version.py
--rw-rw-rw-  2.0 fat     9097 b- defN 23-Apr-22 17:30 jupylite_duckdb/jdw.py
--rw-rw-rw-  2.0 fat     1618 b- defN 23-Apr-22 17:28 jupylite_duckdb/jdw_magic.py
+-rw-rw-rw-  2.0 fat       23 b- defN 23-Apr-22 23:18 jupylite_duckdb/_version.py
+-rw-rw-rw-  2.0 fat     9216 b- defN 23-Apr-22 17:53 jupylite_duckdb/jdw.py
+-rw-rw-rw-  2.0 fat     2149 b- defN 23-Apr-22 23:17 jupylite_duckdb/jdw_magic.py
 -rw-rw-rw-  2.0 fat      979 b- defN 23-Apr-22 14:33 jupylite_duckdb/magic.py
--rw-rw-rw-  2.0 fat     1495 b- defN 23-Apr-22 17:32 jupylite_duckdb-0.0.17.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2314 b- defN 23-Apr-22 17:32 jupylite_duckdb-0.0.17.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-22 17:32 jupylite_duckdb-0.0.17.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       16 b- defN 23-Apr-22 17:32 jupylite_duckdb-0.0.17.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      840 b- defN 23-Apr-22 17:32 jupylite_duckdb-0.0.17.dist-info/RECORD
-10 files, 16601 bytes uncompressed, 5560 bytes compressed:  66.5%
+-rw-rw-rw-  2.0 fat     1495 b- defN 23-Apr-22 23:18 jupylite_duckdb-0.0.18a1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2467 b- defN 23-Apr-22 23:18 jupylite_duckdb-0.0.18a1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-22 23:18 jupylite_duckdb-0.0.18a1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       16 b- defN 23-Apr-22 23:18 jupylite_duckdb-0.0.18a1.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      850 b- defN 23-Apr-22 23:18 jupylite_duckdb-0.0.18a1.dist-info/RECORD
+10 files, 17415 bytes uncompressed, 5836 bytes compressed:  66.5%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: jupylite_duckdb/jdw_magic.py
 Comment: 
 
 Filename: jupylite_duckdb/magic.py
 Comment: 
 
-Filename: jupylite_duckdb-0.0.17.dist-info/LICENSE
+Filename: jupylite_duckdb-0.0.18a1.dist-info/LICENSE
 Comment: 
 
-Filename: jupylite_duckdb-0.0.17.dist-info/METADATA
+Filename: jupylite_duckdb-0.0.18a1.dist-info/METADATA
 Comment: 
 
-Filename: jupylite_duckdb-0.0.17.dist-info/WHEEL
+Filename: jupylite_duckdb-0.0.18a1.dist-info/WHEEL
 Comment: 
 
-Filename: jupylite_duckdb-0.0.17.dist-info/top_level.txt
+Filename: jupylite_duckdb-0.0.18a1.dist-info/top_level.txt
 Comment: 
 
-Filename: jupylite_duckdb-0.0.17.dist-info/RECORD
+Filename: jupylite_duckdb-0.0.18a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jupylite_duckdb/_version.py

```diff
@@ -1 +1 @@
-__version__="0.0.17"
+__version__="0.0.18a1"
```

## jupylite_duckdb/jdw.py

```diff
@@ -8,14 +8,16 @@
 # - Register pandas dataframes with duckdb_wasm: maybe use get_table_names to determine
 # what needs to be registered, then register
 # - Update connect to take connect(file)
 # - 
 
 CONNECTION = None
 
+DEBUG = False
+
 async def future_to_df(result_promise):
     try:
         obj = await result_promise # <class 'pyodide.ffi.JsProxy'>
         a = obj.toArray()
         data = [dict(v) for v in a.object_values()] 
 
         df = DataFrame(data)
@@ -28,14 +30,16 @@
     """Executes query in a standalone connection"""
     if connection is None:
         connection = CONNECTION # if both are None, then a temp db & connection is used
     try:
         if connection is not None:
             result_fut = connection.query(sql)
         else:
+            if DEBUG:
+                print("Creating a new connection to a temporary database...")
             js_function = js.Function('obj', '''
                 async function executeSqlDuckdb() {
                         let c = undefined
                         if(obj.connection == undefined) {
                             const duckdb = await import('https://cdn.skypack.dev/@duckdb/duckdb-wasm');
                             const JSDELIVR_BUNDLES = duckdb.getJsDelivrBundles();
                             const bundle = await duckdb.selectBundle(JSDELIVR_BUNDLES);
```

## jupylite_duckdb/jdw_magic.py

```diff
@@ -1,34 +1,30 @@
-# Inspired by: https://github.com/jupyterlite/jupyterlite/issues/237
-
 from IPython.core.magic import register_line_magic, register_cell_magic
 from IPython.core import magic_arguments
 from IPython.display import display
 import ipywidgets as widgets
 import asyncio
 import jupylite_duckdb as jd
 import functools
 from IPython.core.getipython import get_ipython
 
-
-debug = False
-
+DEBUG = True
 async def display_result(result, output, outputvar = None):
     with output:
         try:
             if result is None:
                 display("Empty Result")
             else:
-                if debug:
+                if DEBUG:
                     display(f"Output type: {type(result)}")
                 display(result)
                 if outputvar is not None: 
                     get_ipython().user_ns[outputvar] = result  # type: ignore
         except Exception as e:
-            display(e)
+            print(e)
 
 #@register_line_magic
 @register_cell_magic
 @magic_arguments.magic_arguments()
 @magic_arguments.argument('-output', nargs=1, help="Output.", type=str)
 #@magic_arguments.argument('query', nargs="+", help="Query.", type=str)
 def dql(line = "", cell = ""):
@@ -41,8 +37,29 @@
     sql = cell
 
     s_out = widgets.Output(layout={'border': '1px solid black'})
     display(s_out)
 
     with s_out:
             r = asyncio.get_event_loop().run_until_complete(jd.query(sql=sql, return_future=False))
-            r.then(functools.partial(display_result, outputvar = outputvar, output=s_out))
+            r.then(functools.partial(display_result, outputvar = outputvar, output=s_out))
+
+
+def patch_magic():
+    # Monkey patching a transformation to stick an "await" ahead of this cell magic
+    
+    
+    shell = get_ipython()
+
+    if not hasattr(shell, "_orig_transform_cell"):
+        shell._orig_transform_cell = shell.transform_cell
+
+    def transform_cell(*args, **kwargs) -> bool:
+            #print(args)
+            #print(kwargs)
+            
+            result=shell._orig_transform_cell(*args, **kwargs)
+            if result.startswith("get_ipython().run_cell_magic('dql',"):
+                result="await" + result
+            return result
+    
+patch_magic()
```

## Comparing `jupylite_duckdb-0.0.17.dist-info/LICENSE` & `jupylite_duckdb-0.0.18a1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `jupylite_duckdb-0.0.17.dist-info/METADATA` & `jupylite_duckdb-0.0.18a1.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupylite-duckdb
-Version: 0.0.17
+Version: 0.0.18a1
 Summary: Testing
 Home-page: https://github.com/iqmo-org/
 Author: iqmo
 Author-email: info@iqmo.com
 Keywords: jupyterlite duckdb wasm
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -44,7 +44,8 @@
 
 
 ## Some development notes
 - There's some (well known) CORS considerations when trying to load data from other sites. Examples here are all using public sites, there's some limits that to address with your own jupyterlite deployment 
 - If you're adding local .py files, use [importlib.invalidate_caches()](https://pyodide.org/en/stable/usage/faq.html#why-can-t-i-import-a-file-i-just-wrote-to-the-file-system). Even then, it was flaky to import.
 - Careful with caching... %pip install will pull from browser cache. I had to clear frequently within dev tools
 - To clear local storage, which is annoyingly persistent, https://superuser.com/questions/519628/clear-html5-local-storage-on-a-specific-page
+- %autoawait is part of why this works in notebooks, which is enabled by default: https://ipython.readthedocs.io/en/stable/interactive/autoawait.html
```

## Comparing `jupylite_duckdb-0.0.17.dist-info/RECORD` & `jupylite_duckdb-0.0.18a1.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 jupylite_duckdb/__init__.py,sha256=-Z_P6KBbWKDsMsnvKal14k3bbGljgWmFQPEvz7zrLVU,128
-jupylite_duckdb/_version.py,sha256=GEd_d0cJY-aeYoeZOG699Pnc0HUqdnua0qUTnNIzWpU,22
-jupylite_duckdb/jdw.py,sha256=P3zFLAew-KwZZhRm8ky7HFF7jaujDHJ8_BHd9X6KVKY,9097
-jupylite_duckdb/jdw_magic.py,sha256=3rFnfFdOwc_yUbkGkSeVDmaQw0JSa1koD3VyCqHo3XI,1618
+jupylite_duckdb/_version.py,sha256=bnGb1xseM2J6mXvI8BV0FJtYzRxYAhmJ11S9NxczMas,23
+jupylite_duckdb/jdw.py,sha256=LzIoBx4_3j3iUlp5lviHuISdCClNdHEKb9_O8X1-cpg,9216
+jupylite_duckdb/jdw_magic.py,sha256=EBbz8IhYUc4Wubrfjb5jQcxsHblPj-BdwerktkUWxBo,2149
 jupylite_duckdb/magic.py,sha256=okWgdHbcu0ul2BOYNdu9NHwRSoyAG_0m6RiGnw2Bj_k,979
-jupylite_duckdb-0.0.17.dist-info/LICENSE,sha256=WJMtiY9u9JD8FJ18a6_psLMXvrOIA7F-mYphCuyGFvw,1495
-jupylite_duckdb-0.0.17.dist-info/METADATA,sha256=KJOoPGLlUhs907vlD763KxGh0T5YtkS_3UiVm3QKHBw,2314
-jupylite_duckdb-0.0.17.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-jupylite_duckdb-0.0.17.dist-info/top_level.txt,sha256=y1GybQE7FyRTQPGLf2lE9dStC--h8ZozxhgXQRxz490,16
-jupylite_duckdb-0.0.17.dist-info/RECORD,,
+jupylite_duckdb-0.0.18a1.dist-info/LICENSE,sha256=WJMtiY9u9JD8FJ18a6_psLMXvrOIA7F-mYphCuyGFvw,1495
+jupylite_duckdb-0.0.18a1.dist-info/METADATA,sha256=O6zIm7mROG8kgkKpB2TDEDXdwQ1pvebr-P5A3oQWoIw,2467
+jupylite_duckdb-0.0.18a1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+jupylite_duckdb-0.0.18a1.dist-info/top_level.txt,sha256=y1GybQE7FyRTQPGLf2lE9dStC--h8ZozxhgXQRxz490,16
+jupylite_duckdb-0.0.18a1.dist-info/RECORD,,
```

