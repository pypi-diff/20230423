# Comparing `tmp/mell-2.0.0.tar.gz` & `tmp/mell-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mell-2.0.0.tar", last modified: Sat Apr 22 21:38:13 2023, max compression
+gzip compressed data, was "mell-2.0.1.tar", last modified: Sun Apr 23 00:43:24 2023, max compression
```

## Comparing `mell-2.0.0.tar` & `mell-2.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 21:38:13.204892 mell-2.0.0/
--rw-r--r--   0 root         (0) root         (0)      411 2023-04-22 21:38:13.204892 mell-2.0.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)        0 2023-04-22 21:10:54.000000 mell-2.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 21:38:13.204892 mell-2.0.0/mell/
--rw-rw-r--   0 root         (0) root         (0)       14 2023-04-22 21:31:52.000000 mell-2.0.0/mell/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)    16126 2023-04-22 21:37:38.000000 mell-2.0.0/mell/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 21:38:13.204892 mell-2.0.0/mell.egg-info/
--rw-rw-r--   0 root         (0) root         (0)      411 2023-04-22 21:38:13.000000 mell-2.0.0/mell.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      218 2023-04-22 21:38:13.000000 mell-2.0.0/mell.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2023-04-22 21:38:13.000000 mell-2.0.0/mell.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)       40 2023-04-22 21:38:13.000000 mell-2.0.0/mell.egg-info/entry_points.txt
--rw-rw-r--   0 root         (0) root         (0)       15 2023-04-22 21:38:13.000000 mell-2.0.0/mell.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)        5 2023-04-22 21:38:13.000000 mell-2.0.0/mell.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-22 21:38:13.204892 mell-2.0.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1024 2023-04-22 21:18:02.000000 mell-2.0.0/setup.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-04-23 00:43:24.591577 mell-2.0.1/
+-rw-rw-r--   0 diego     (1000) diego     (1000)    10046 2023-04-23 00:43:24.591577 mell-2.0.1/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)     9594 2023-04-23 00:43:10.000000 mell-2.0.1/README.md
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-04-23 00:43:24.591577 mell-2.0.1/mell/
+-rw-rw-r--   0 diego     (1000) diego     (1000)       14 2023-04-22 21:31:52.000000 mell-2.0.1/mell/__init__.py
+-rwxrwxr-x   0 diego     (1000) diego     (1000)    15036 2023-04-23 00:37:24.000000 mell-2.0.1/mell/main.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-04-23 00:43:24.591577 mell-2.0.1/mell.egg-info/
+-rw-rw-r--   0 diego     (1000) diego     (1000)    10046 2023-04-23 00:43:24.000000 mell-2.0.1/mell.egg-info/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)      218 2023-04-23 00:43:24.000000 mell-2.0.1/mell.egg-info/SOURCES.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)        1 2023-04-23 00:43:24.000000 mell-2.0.1/mell.egg-info/dependency_links.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)       40 2023-04-23 00:43:24.000000 mell-2.0.1/mell.egg-info/entry_points.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)       15 2023-04-23 00:43:24.000000 mell-2.0.1/mell.egg-info/requires.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)        5 2023-04-23 00:43:24.000000 mell-2.0.1/mell.egg-info/top_level.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)       38 2023-04-23 00:43:24.591577 mell-2.0.1/setup.cfg
+-rw-rw-r--   0 diego     (1000) diego     (1000)     1062 2023-04-23 00:38:25.000000 mell-2.0.1/setup.py
```

### Comparing `mell-2.0.0/mell/main.py` & `mell-2.0.1/mell/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,162 +27,105 @@
 
 def error(*args):
     if LOG_LEVEL <= 3:
         print("ERROR:", *args)
     sys.exit(1)
 
 
-def parse_args():
+def new_structure(value):
+    if os.path.exists(value):
+        error(f"Can't create a root structure, a folder with this name already exists: {value}")
+        
+    for foldernames in [("style", "asset"), ("style", "template"), ("style", "plugin"), ("style", "static"), ("meta",), ("generate",)]:
+        path = os.path.join(value, *foldernames)
+        info(f"  Creating folder {path}")
+        os.makedirs(path)
+    
+    sys.exit(0)
+
+def new_style_structure(value):
+    if os.path.exists(value):
+        error(f"Can't create a style structure, a folder with this name already exists: {value}")
+        
+    for foldernames in ["asset", "template", "plugin", "static"]:
+        path = os.path.join(value, foldernames)
+        info(f"  Creating folder {path}")
+        os.makedirs(path)
+    
+    sys.exit(0)
 
-    epilogue = """
-    Recommended folder structure:
 
-        <root>:
-        |- generate: folder that will hold the generated data, do not edit this folder.
-        |
-        |- meta:     folder holding json files, each with a variation of the metadata.
-        |
-        |- template: folder holding the template files that will be rendered with the 
-        |            current metadata and saved to the generate folder, using the same path.
-        |
-        |- static:   folder holding the static files that will be copied as they are to the 
-        |            generate folder, using the same path.
-        |
-        |- plugin:   folder holding scripts with a main function receiving the parameters 
-        |            inflater and meta.Create scripts to generate multiple files from 
-        |            templates in the asset folder.
-        |
-        |- asset:    folder holding template and other files that are not directly copied to 
-                    generate. They may be used by plugins or other tools.
-
-
-    basic example:
-
-        # Content of ./template/main.py
-        print(|= meta["message"] =|)
-
-        # Content of ./meta/pt.json
-        { "message": "Olá Mundo" }
-
-        # Content of ./meta/en.json
-        { "message": "Hello World" }
-
-        # Execute it with the following command:
-        mel pt
-
-        # It will generate the following file in ./generate/main.py
-        print("Olá Mundo")
-                    
-        # Execute it with the following command:
-        mel en
-
-        # It will generate the following file in ./generate/main.py
-        print("Hello World")
-
-
-    plugin example:
-
-        # Content of ./asset/example.txt
-        Key: |= meta["key"] =|
-        Value: |= meta["value"]=|
-
-        # Content of ./plugin/example_plugin.py
-        def main(inflater, meta):
-            for i, item in enumerate(meta["examples"]):
-                inflater.inflateAsset("example.txt", item, to_file=f"examples/ex{i}.txt")
-
-        # Content of ./meta/en.txt
-        {
-            "examples": [
-                {
-                    "key": "nome",
-                    "value": "Diego"
-                },
-                {
-                    "key": "idade",
-                    "value": "33"
-                },
-                {
-                    "key": "sexo",
-                    "value": "Masculino"
-                },
-                {
-                    "key": "estado civil",
-                    "value": "Solteiro"
-                }
-            ]
-        }
-
-        # Run it with the following command:
-        mel en
-
-        # Four files will be generated in ./generate/examples. The first file is ex0.txt, 
-        # with the following content:
-        Key: nome
-        Value: Diego
-    """
+def parse_args():
+
 
     parser = argparse.ArgumentParser(
                         prog='mel',
                         description='Metaprogramming layer designed to generates anything from template files.',
-                        epilog=epilogue,
+                        epilog="Check my README.md to learn more tips on how to use this application: https://github.com/diegofps/mell/blob/main/README.md",
                         formatter_class=argparse.RawDescriptionHelpFormatter)
 
     parser.add_argument('metadata',
                         type=str,
                         metavar='METADATA',
                         help="name of file(s) located inside the meta folder. If multiple are provided, separated by comma, a merge will be performed.")
 
-    parser.add_argument('-t', '--template',
+    parser.add_argument('--template',
                         type=str,
                         default=None,
                         dest='template',
-                        help="Folder to read the template files, the default value is <root>/template",
+                        help="Folder to read the template files, the default value is <style>/template",
                         action='store')
 
-    parser.add_argument('-s', '--static',
+    parser.add_argument('--static',
                         type=str,
                         default=None,
                         dest='static',
-                        help="Folder to read the static files, the default value is <root>/static",
+                        help="Folder to read the static files, the default value is <style>/static",
                         action='store')
 
-    parser.add_argument('-m', '--meta',
+    parser.add_argument('--plugin',
                         type=str,
                         default=None,
-                        dest='meta',
-                        help="Folder to read the metadata files, the default value is <root>/meta",
+                        dest='plugin',
+                        help="Folder to read the plugins, the default value is <style>/plugin",
                         action='store')
 
-    parser.add_argument('-g', '--generate',
+    parser.add_argument('--asset',
                         type=str,
                         default=None,
-                        dest=None,
-                        help="Folder to generate the code, the default value is <root>/generate",
+                        dest='asset',
+                        help="Folder holding the asset files, the default value is <style>/asset",
                         action='store')
 
-    parser.add_argument('-p', '--plugin',
+    parser.add_argument('--meta',
                         type=str,
                         default=None,
-                        dest='plugin',
-                        help="Folder to read the plugins, the default value is <root>/plugin",
+                        dest='meta',
+                        help="Folder to read the metadata files, the default value is <root>/meta",
                         action='store')
 
-    parser.add_argument('-a', '--asset',
+    parser.add_argument('--generate',
                         type=str,
                         default=None,
-                        dest='asset',
-                        help="Folder holding the asset files, the default value is <root>/asset",
+                        dest=None,
+                        help="Folder to generate the code, the default value is <root>/generate",
+                        action='store')
+
+    parser.add_argument('--style',
+                        type=str,
+                        default=None,
+                        dest='style',
+                        help="Style folder that contains asset, template, plugin, and static. Its default value is <root>/style",
                         action='store')
 
-    parser.add_argument('-r', '--root',
+    parser.add_argument('--root',
                         type=str,
                         default='.',
                         dest='root',
-                        help="Root folder that contains all other folders, the default value is '.'",
+                        help="Root folder that contains the folders style, meta, and generate. Its default value is '.'",
                         action='store')
 
     parser.add_argument('-v', '--verbose',
                         default=None,
                         dest='verbose',
                         help="Allow debug log messages to be displayed",
                         action='store_true')
@@ -238,37 +181,48 @@
     parser.add_argument('-d', '--do',
                         type=str,
                         default=None,
                         choices=['clean', 'static', 'template', 'plugin'],
                         dest='do',
                         help="Define one or more tasks to be executed. Will run all of them by default",
                         action='append')
-
+    
+    parser.add_argument('--new',
+                        help="Create a new root folder with the recommended structure",
+                        type=new_structure)
+    
+    parser.add_argument('--new-style',
+                        help="Create a new style folder with the recommended structure",
+                        type=new_style_structure)
+    
     args = parser.parse_args()
 
     if args.root is None:
         args.root = '.'
 
     if args.generate is None:
         args.generate = os.path.join(args.root, 'generate')
 
     if args.meta is None:
         args.meta = os.path.join(args.root, 'meta')
 
+    if args.style is None:
+        args.style = os.path.join(args.root, 'style')
+
     if args.static is None:
-        args.static = os.path.join(args.root, 'static')
+        args.static = os.path.join(args.style, 'static')
 
     if args.template is None:
-        args.template = os.path.join(args.root, 'template')
+        args.template = os.path.join(args.style, 'template')
 
     if args.plugin is None:
-        args.plugin = os.path.join(args.root, 'plugin')
+        args.plugin = os.path.join(args.style, 'plugin')
 
     if args.asset is None:
-        args.asset = os.path.join(args.root, 'asset')
+        args.asset = os.path.join(args.style, 'asset')
 
     if args.do is None:
         args.do = ['clean', 'static', 'template', 'plugin']
 
     global LOG_LEVEL
     
     if args.quiet and args.verbose:
@@ -489,26 +443,24 @@
             plugin_spec.loader.exec_module(plugin)
             plugin.main(inflater, meta)
 
 
 def main(*params):
     
     args = parse_args()
-    debug(json.dumps(args.__dict__, indent=2))
-
 
     info("Loading the metadata")
     meta = Meta(args)
-    debug(meta)
 
+    debug(meta)
+    debug(json.dumps(args.__dict__, indent=2))
 
     info("Loading the inflater")
     inflater = Inflater(args)
 
-
     info("Executing actions")
     for name in args.do:
         globals()['do_' + name](args, inflater, meta)
 
 
     info("Bye!")
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mell-2.0.0/setup.py` & `mell-2.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 
 #import mell.consts as c
 import setuptools
 
 name = "mell"
-version = "2.0.0"
+version = "2.0.1"
 author = "Diego Souza"
 author_email = "diegofpsouza+mell@gmail.com"
 url = "https://github.com/diegofps/pywup"
 
 description = "A Metaprogramming Logic Layer designed to generate anything from template files"
-long_description = None
-long_description_content_type = None # "text/markdown"
+
+long_description_content_type = "text/markdown"
+with open("README.md", "r") as fh:
+    long_description = fh.read()
 
 
 setuptools.setup(
     name=name,
     version=version,
     author=author,
     author_email=author_email,
```

