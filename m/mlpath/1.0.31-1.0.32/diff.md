# Comparing `tmp/mlpath-1.0.31.tar.gz` & `tmp/mlpath-1.0.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpath-1.0.31.tar", last modified: Thu Apr 20 16:27:24 2023, max compression
+gzip compressed data, was "mlpath-1.0.32.tar", last modified: Sat Apr 22 23:11:44 2023, max compression
```

## Comparing `mlpath-1.0.31.tar` & `mlpath-1.0.32.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-04-20 16:27:24.235901 mlpath-1.0.31/
--rw-r--r--   0 essam      (501) staff       (20)    18092 2023-04-20 16:25:39.000000 mlpath-1.0.31/LICENSE
--rw-r--r--   0 essam      (501) staff       (20)      192 2023-04-20 16:25:39.000000 mlpath-1.0.31/MANIFEST.in
--rw-r--r--   0 essam      (501) staff       (20)    17710 2023-04-20 16:27:24.235595 mlpath-1.0.31/PKG-INFO
--rw-r--r--   0 essam      (501) staff       (20)    16909 2023-04-20 16:25:39.000000 mlpath-1.0.31/README.md
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-04-20 16:27:24.232029 mlpath-1.0.31/mlpath/
--rw-r--r--   0 essam      (501) staff       (20)      122 2023-04-20 16:25:39.000000 mlpath-1.0.31/mlpath/__init__.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-04-20 16:27:24.233850 mlpath-1.0.31/mlpath/mldir_cli/
--rw-r--r--   0 essam      (501) staff       (20)        0 2023-04-20 16:25:39.000000 mlpath-1.0.31/mlpath/mldir_cli/__init__.py
--rw-r--r--   0 essam      (501) staff       (20)     2049 2023-04-20 16:25:39.000000 mlpath-1.0.31/mlpath/mldir_cli/cli.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-04-20 16:27:24.235077 mlpath-1.0.31/mlpath/mlquest/
--rw-r--r--   0 essam      (501) staff       (20)        0 2023-04-20 16:25:39.000000 mlpath-1.0.31/mlpath/mlquest/__init__.py
--rw-r--r--   0 essam      (501) staff       (20)    19811 2023-04-20 16:25:39.000000 mlpath-1.0.31/mlpath/mlquest/mlquest.py
--rw-r--r--   0 essam      (501) staff       (20)    10190 2023-04-20 16:25:39.000000 mlpath-1.0.31/mlpath/mlquest/utils.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-04-20 16:27:24.233492 mlpath-1.0.31/mlpath.egg-info/
--rw-r--r--   0 essam      (501) staff       (20)    17710 2023-04-20 16:27:23.000000 mlpath-1.0.31/mlpath.egg-info/PKG-INFO
--rw-r--r--   0 essam      (501) staff       (20)      369 2023-04-20 16:27:24.000000 mlpath-1.0.31/mlpath.egg-info/SOURCES.txt
--rw-r--r--   0 essam      (501) staff       (20)        1 2023-04-20 16:27:23.000000 mlpath-1.0.31/mlpath.egg-info/dependency_links.txt
--rw-r--r--   0 essam      (501) staff       (20)       85 2023-04-20 16:27:23.000000 mlpath-1.0.31/mlpath.egg-info/entry_points.txt
--rw-r--r--   0 essam      (501) staff       (20)       20 2023-04-20 16:27:24.000000 mlpath-1.0.31/mlpath.egg-info/requires.txt
--rw-r--r--   0 essam      (501) staff       (20)        7 2023-04-20 16:27:24.000000 mlpath-1.0.31/mlpath.egg-info/top_level.txt
--rw-r--r--   0 essam      (501) staff       (20)       38 2023-04-20 16:27:24.235991 mlpath-1.0.31/setup.cfg
--rw-r--r--   0 essam      (501) staff       (20)     2066 2023-04-20 16:27:01.000000 mlpath-1.0.31/setup.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-04-22 23:11:44.727516 mlpath-1.0.32/
+-rw-r--r--   0 essam      (501) staff       (20)    18092 2023-04-20 16:25:39.000000 mlpath-1.0.32/LICENSE
+-rw-r--r--   0 essam      (501) staff       (20)      192 2023-04-20 16:25:39.000000 mlpath-1.0.32/MANIFEST.in
+-rw-r--r--   0 essam      (501) staff       (20)    17710 2023-04-22 23:11:44.725484 mlpath-1.0.32/PKG-INFO
+-rw-r--r--   0 essam      (501) staff       (20)    16909 2023-04-20 16:25:39.000000 mlpath-1.0.32/README.md
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-04-22 23:11:44.721074 mlpath-1.0.32/mlpath/
+-rw-r--r--   0 essam      (501) staff       (20)      122 2023-04-20 16:25:39.000000 mlpath-1.0.32/mlpath/__init__.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-04-22 23:11:44.723457 mlpath-1.0.32/mlpath/mldir_cli/
+-rw-r--r--   0 essam      (501) staff       (20)        0 2023-04-20 16:25:39.000000 mlpath-1.0.32/mlpath/mldir_cli/__init__.py
+-rw-r--r--   0 essam      (501) staff       (20)     2049 2023-04-20 16:25:39.000000 mlpath-1.0.32/mlpath/mldir_cli/cli.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-04-22 23:11:44.724767 mlpath-1.0.32/mlpath/mlquest/
+-rw-r--r--   0 essam      (501) staff       (20)        0 2023-04-20 16:25:39.000000 mlpath-1.0.32/mlpath/mlquest/__init__.py
+-rw-r--r--   0 essam      (501) staff       (20)    19841 2023-04-22 23:11:06.000000 mlpath-1.0.32/mlpath/mlquest/mlquest.py
+-rw-r--r--   0 essam      (501) staff       (20)    10220 2023-04-22 23:11:18.000000 mlpath-1.0.32/mlpath/mlquest/utils.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-04-22 23:11:44.722962 mlpath-1.0.32/mlpath.egg-info/
+-rw-r--r--   0 essam      (501) staff       (20)    17710 2023-04-22 23:11:43.000000 mlpath-1.0.32/mlpath.egg-info/PKG-INFO
+-rw-r--r--   0 essam      (501) staff       (20)      369 2023-04-22 23:11:44.000000 mlpath-1.0.32/mlpath.egg-info/SOURCES.txt
+-rw-r--r--   0 essam      (501) staff       (20)        1 2023-04-22 23:11:43.000000 mlpath-1.0.32/mlpath.egg-info/dependency_links.txt
+-rw-r--r--   0 essam      (501) staff       (20)       85 2023-04-22 23:11:44.000000 mlpath-1.0.32/mlpath.egg-info/entry_points.txt
+-rw-r--r--   0 essam      (501) staff       (20)       20 2023-04-22 23:11:44.000000 mlpath-1.0.32/mlpath.egg-info/requires.txt
+-rw-r--r--   0 essam      (501) staff       (20)        7 2023-04-22 23:11:44.000000 mlpath-1.0.32/mlpath.egg-info/top_level.txt
+-rw-r--r--   0 essam      (501) staff       (20)       38 2023-04-22 23:11:44.727703 mlpath-1.0.32/setup.cfg
+-rw-r--r--   0 essam      (501) staff       (20)     2066 2023-04-22 23:11:33.000000 mlpath-1.0.32/setup.py
```

### Comparing `mlpath-1.0.31/LICENSE` & `mlpath-1.0.32/LICENSE`

 * *Files identical despite different names*

### Comparing `mlpath-1.0.31/PKG-INFO` & `mlpath-1.0.32/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpath
-Version: 1.0.31
+Version: 1.0.32
 Summary: A lightweight api for machine and deep learning experiment logging in the form of a python library. 
 Home-page: https://mlpath.readthedocs.io/
 Author: Essam W., Abdullah A.
 Author-email: essamwisam@outlook.com
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mlpath Version: 1.0.31 Summary: A lightweight api
+Metadata-Version: 2.1 Name: mlpath Version: 1.0.32 Summary: A lightweight api
 for machine and deep learning experiment logging in the form of a python
 library. Home-page: https://mlpath.readthedocs.io/ Author: Essam W., Abdullah
 A. Author-email: essamwisam@outlook.com License: GPLv3 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
```

### Comparing `mlpath-1.0.31/README.md` & `mlpath-1.0.32/README.md`

 * *Files identical despite different names*

### Comparing `mlpath-1.0.31/mlpath/mldir_cli/cli.py` & `mlpath-1.0.32/mlpath/mldir_cli/cli.py`

 * *Files identical despite different names*

### Comparing `mlpath-1.0.31/mlpath/mlquest/mlquest.py` & `mlpath-1.0.32/mlpath/mlquest/mlquest.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
       - The :samp:`table_dest` parameter is used to decide where the experiments table should be saved. If it's given as :samp:`../` then this means that the markdown file (experiments table) corresponding to this quest will be saved in the folder :samp:`../Quests/<ParentFolder>/<QuestName>/`.
        '''
        # get the name of the folder containing the current file
        mlquest.relative_path = table_dest
        mlquest.log_defs = log_defs
        mlquest.curr_dir = os.path.basename(os.getcwd())
        if not os.path.exists(f'{mlquest.relative_path}Quests/{mlquest.curr_dir}/{quest_name}'):
-          os.makedirs(mlquest.relative_path + 'Quests/' + mlquest.curr_dir + '/' + quest_name)
+          os.makedirs(mlquest.relative_path + 'Quests/' + mlquest.curr_dir + '/' + quest_name, exist_ok=True)
             
        if 'quests.mlq' in os.listdir(f'{mlquest.relative_path}Quests/{mlquest.curr_dir}/{quest_name}'):
             with open(mlquest.relative_path + f'Quests/{mlquest.curr_dir}/{quest_name}/quests.mlq', 'rb') as f:
                mlquest.quests = pickle.load(f)
        
        mlquest.quest_name = quest_name
        if mlquest.active == True: warnings.warn("Attempting to start a run while another one is active may cause data overwrite")
@@ -264,15 +264,15 @@
     @staticmethod
     def save_quest(quest_name):
        '''
        Uses pickle to save the quests object to a file.
        '''
        # see if there is a 'mlquests' folder, if not, create it
        if not os.path.exists(f'{mlquest.relative_path}Quests/{mlquest.curr_dir}'):
-          os.makedirs(mlquest.relative_path + 'Quests/'  + mlquest.curr_dir)
+          os.makedirs(mlquest.relative_path + 'Quests/'  + mlquest.curr_dir, exist_ok=True)
        
        with open(f'{mlquest.relative_path}Quests/{mlquest.curr_dir}/{quest_name}/quests.mlq', 'wb') as f:
             pickle.dump(mlquest.quests, f)
           
     @staticmethod
     def end_quest():
        '''
```

### Comparing `mlpath-1.0.31/mlpath/mlquest/utils.py` & `mlpath-1.0.32/mlpath/mlquest/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,15 +159,15 @@
                value = json_obj[key][subkey][i] if json_obj[key][subkey][i] is not None else ''
                table += f'<td style="text-align: center; vertical-align: middle;"> <font color={color}>{value}</font></td>\n'
       table += '</tr>\n'
 
    # save the html file
    if save:
       if not os.path.exists(f'{relative_path}Quests/{curr_dir}/{quest_name}'):
-         os.makedirs(f'{relative_path}Quests/{curr_dir}/{quest_name}')
+         os.makedirs(f'{relative_path}Quests/{curr_dir}/{quest_name}', exist_ok=True)
       with open(relative_path + f'Quests/{curr_dir}/{quest_name}/{quest_name}.md', 'w') as f:
          f.write(table)
    
    # return the html table
    return table
    
       
@@ -175,15 +175,15 @@
 def runs_to_json(relative_path, curr_dir, runs, quest_name, log_defs, non_default_log):
    '''
    converts the runs of a quest to a json file
    :param quest_name: The name of the quest to be converted
    :type quest_name: string
    '''
    if not os.path.exists(f'{relative_path}Quests/{curr_dir}/{quest_name}/json'):
-      os.makedirs(f'{relative_path}Quests/{curr_dir}/{quest_name}/json')
+      os.makedirs(f'{relative_path}Quests/{curr_dir}/{quest_name}/json', exist_ok=True)
    
    big_dict = merge_dicts(runs)
    # remove ['info]['name'] from the dict
    del big_dict['info']['name']
    # now convert to json
    j = json.dumps(big_dict, indent=4)
    # save the json file
```

### Comparing `mlpath-1.0.31/mlpath.egg-info/PKG-INFO` & `mlpath-1.0.32/mlpath.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpath
-Version: 1.0.31
+Version: 1.0.32
 Summary: A lightweight api for machine and deep learning experiment logging in the form of a python library. 
 Home-page: https://mlpath.readthedocs.io/
 Author: Essam W., Abdullah A.
 Author-email: essamwisam@outlook.com
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mlpath Version: 1.0.31 Summary: A lightweight api
+Metadata-Version: 2.1 Name: mlpath Version: 1.0.32 Summary: A lightweight api
 for machine and deep learning experiment logging in the form of a python
 library. Home-page: https://mlpath.readthedocs.io/ Author: Essam W., Abdullah
 A. Author-email: essamwisam@outlook.com License: GPLv3 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
```

### Comparing `mlpath-1.0.31/setup.py` & `mlpath-1.0.32/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         requirements = f.read().splitlines()
     return requirements
 
 
 # This call to setup() does all the work
 setup(
     name="mlpath",
-    version="1.0.31",
+    version="1.0.32",
     description="A lightweight api for machine and deep learning experiment logging in the form of a python library. ",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://mlpath.readthedocs.io/",
     author="Essam W., Abdullah A.",
     author_email="essamwisam@outlook.com",
     license="GPLv3",
```

