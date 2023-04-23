# Comparing `tmp/Shyna_speaks-0.0.6.tar.gz` & `tmp/Shyna_speaks-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Shyna_speaks-0.0.6.tar", last modified: Thu Mar 23 19:39:18 2023, max compression
+gzip compressed data, was "Shyna_speaks-0.0.7.tar", last modified: Sun Apr 23 12:22:45 2023, max compression
```

## Comparing `Shyna_speaks-0.0.6.tar` & `Shyna_speaks-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 shyna     (1000) shyna     (1000)        0 2023-03-23 19:39:18.155381 Shyna_speaks-0.0.6/
--rw-rw-r--   0 shyna     (1000) shyna     (1000)     1070 2023-03-12 09:12:39.000000 Shyna_speaks-0.0.6/LICENSE
--rw-rw-r--   0 shyna     (1000) shyna     (1000)      865 2023-03-23 19:39:18.155381 Shyna_speaks-0.0.6/PKG-INFO
--rw-rw-r--   0 shyna     (1000) shyna     (1000)      643 2023-03-12 09:12:39.000000 Shyna_speaks-0.0.6/README.md
-drwxrwxr-x   0 shyna     (1000) shyna     (1000)        0 2023-03-23 19:39:18.155381 Shyna_speaks-0.0.6/Shyna_speaks/
--rw-rw-r--   0 shyna     (1000) shyna     (1000)     3188 2023-03-12 09:12:39.000000 Shyna_speaks-0.0.6/Shyna_speaks/Shyna_speaks.py
--rw-rw-r--   0 shyna     (1000) shyna     (1000)        0 2023-03-12 09:12:39.000000 Shyna_speaks-0.0.6/Shyna_speaks/__init__.py
--rw-rw-r--   0 shyna     (1000) shyna     (1000)     3880 2023-03-23 19:38:36.000000 Shyna_speaks-0.0.6/Shyna_speaks/speak_automation.py
-drwxrwxr-x   0 shyna     (1000) shyna     (1000)        0 2023-03-23 19:39:18.155381 Shyna_speaks-0.0.6/Shyna_speaks.egg-info/
--rw-rw-r--   0 shyna     (1000) shyna     (1000)      865 2023-03-23 19:39:18.000000 Shyna_speaks-0.0.6/Shyna_speaks.egg-info/PKG-INFO
--rw-rw-r--   0 shyna     (1000) shyna     (1000)      307 2023-03-23 19:39:18.000000 Shyna_speaks-0.0.6/Shyna_speaks.egg-info/SOURCES.txt
--rw-rw-r--   0 shyna     (1000) shyna     (1000)        1 2023-03-23 19:39:18.000000 Shyna_speaks-0.0.6/Shyna_speaks.egg-info/dependency_links.txt
--rw-rw-r--   0 shyna     (1000) shyna     (1000)       54 2023-03-23 19:39:18.000000 Shyna_speaks-0.0.6/Shyna_speaks.egg-info/requires.txt
--rw-rw-r--   0 shyna     (1000) shyna     (1000)       13 2023-03-23 19:39:18.000000 Shyna_speaks-0.0.6/Shyna_speaks.egg-info/top_level.txt
--rw-rw-r--   0 shyna     (1000) shyna     (1000)      138 2023-03-12 09:12:39.000000 Shyna_speaks-0.0.6/pyproject.toml
--rw-rw-r--   0 shyna     (1000) shyna     (1000)       38 2023-03-23 19:39:18.155381 Shyna_speaks-0.0.6/setup.cfg
--rw-rw-r--   0 shyna     (1000) shyna     (1000)      605 2023-03-23 19:38:36.000000 Shyna_speaks-0.0.6/setup.py
+drwxrwxr-x   0 shyna     (1000) shyna     (1000)        0 2023-04-23 12:22:45.851091 Shyna_speaks-0.0.7/
+-rw-rw-r--   0 shyna     (1000) shyna     (1000)     1070 2023-03-12 09:12:39.000000 Shyna_speaks-0.0.7/LICENSE
+-rw-rw-r--   0 shyna     (1000) shyna     (1000)      865 2023-04-23 12:22:45.851091 Shyna_speaks-0.0.7/PKG-INFO
+-rw-rw-r--   0 shyna     (1000) shyna     (1000)      643 2023-03-12 09:12:39.000000 Shyna_speaks-0.0.7/README.md
+drwxrwxr-x   0 shyna     (1000) shyna     (1000)        0 2023-04-23 12:22:45.851091 Shyna_speaks-0.0.7/Shyna_speaks/
+-rw-rw-r--   0 shyna     (1000) shyna     (1000)     3188 2023-03-12 09:12:39.000000 Shyna_speaks-0.0.7/Shyna_speaks/Shyna_speaks.py
+-rw-rw-r--   0 shyna     (1000) shyna     (1000)        0 2023-03-12 09:12:39.000000 Shyna_speaks-0.0.7/Shyna_speaks/__init__.py
+-rw-rw-r--   0 shyna     (1000) shyna     (1000)     3884 2023-04-23 12:22:07.000000 Shyna_speaks-0.0.7/Shyna_speaks/speak_automation.py
+drwxrwxr-x   0 shyna     (1000) shyna     (1000)        0 2023-04-23 12:22:45.851091 Shyna_speaks-0.0.7/Shyna_speaks.egg-info/
+-rw-rw-r--   0 shyna     (1000) shyna     (1000)      865 2023-04-23 12:22:45.000000 Shyna_speaks-0.0.7/Shyna_speaks.egg-info/PKG-INFO
+-rw-rw-r--   0 shyna     (1000) shyna     (1000)      307 2023-04-23 12:22:45.000000 Shyna_speaks-0.0.7/Shyna_speaks.egg-info/SOURCES.txt
+-rw-rw-r--   0 shyna     (1000) shyna     (1000)        1 2023-04-23 12:22:45.000000 Shyna_speaks-0.0.7/Shyna_speaks.egg-info/dependency_links.txt
+-rw-rw-r--   0 shyna     (1000) shyna     (1000)       54 2023-04-23 12:22:45.000000 Shyna_speaks-0.0.7/Shyna_speaks.egg-info/requires.txt
+-rw-rw-r--   0 shyna     (1000) shyna     (1000)       13 2023-04-23 12:22:45.000000 Shyna_speaks-0.0.7/Shyna_speaks.egg-info/top_level.txt
+-rw-rw-r--   0 shyna     (1000) shyna     (1000)      138 2023-03-12 09:12:39.000000 Shyna_speaks-0.0.7/pyproject.toml
+-rw-rw-r--   0 shyna     (1000) shyna     (1000)       38 2023-04-23 12:22:45.851091 Shyna_speaks-0.0.7/setup.cfg
+-rw-rw-r--   0 shyna     (1000) shyna     (1000)      605 2023-04-23 12:22:07.000000 Shyna_speaks-0.0.7/setup.py
```

### Comparing `Shyna_speaks-0.0.6/LICENSE` & `Shyna_speaks-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `Shyna_speaks-0.0.6/PKG-INFO` & `Shyna_speaks-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Shyna_speaks
-Version: 0.0.6
+Version: 0.0.7
 Summary: Shyna Speak package, Phase one
 Author: Shivam Sharma
 Author-email: shivamsharma1913@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # shyna/Shyna_speaks
```

### Comparing `Shyna_speaks-0.0.6/README.md` & `Shyna_speaks-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `Shyna_speaks-0.0.6/Shyna_speaks/Shyna_speaks.py` & `Shyna_speaks-0.0.7/Shyna_speaks/Shyna_speaks.py`

 * *Files identical despite different names*

### Comparing `Shyna_speaks-0.0.6/Shyna_speaks/speak_automation.py` & `Shyna_speaks-0.0.7/Shyna_speaks/speak_automation.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,18 +78,18 @@
             self.s_data.default_database = os.environ.get('notify_db')
             self.s_data.query = "SELECT * from speak_sentence where status='False' order by count DESC"
             result = self.s_data.select_from_table()
             if str(result[0]).lower().__eq__('empty'):
                 pass
             else:
                 for item in result:
-                    self.priority = list(str(item[6]).strip("[]").split(","))
-                    self.shyna_speaks(msg=item[3])
                     self.s_data.default_database = os.environ.get('notify_db')
-                    self.s_data.query = "UPDATE speak_sentence set status='True' where count = '"+str(item[0])+"'"
+                    self.s_data.query = "UPDATE speak_sentence set status='True' where count = '" + str(item[0]) + "'"
                     self.s_data.create_insert_update_or_delete()
+                    self.priority = list(str(item[6]).strip("[]").split(","))
+                    self.shyna_speaks(msg=item[3])
         except Exception as e:
             print(e)
 
 
 if __name__ == '__main__':
     ShynaSpeak().get_sentence()
```

### Comparing `Shyna_speaks-0.0.6/Shyna_speaks.egg-info/PKG-INFO` & `Shyna_speaks-0.0.7/Shyna_speaks.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Shyna-speaks
-Version: 0.0.6
+Version: 0.0.7
 Summary: Shyna Speak package, Phase one
 Author: Shivam Sharma
 Author-email: shivamsharma1913@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # shyna/Shyna_speaks
```

### Comparing `Shyna_speaks-0.0.6/setup.py` & `Shyna_speaks-0.0.7/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup_args = dict(
     name='Shyna_speaks',
-    version='0.0.6',
+    version='0.0.7',
     packages=find_packages(),
     author="Shivam Sharma",
     author_email="shivamsharma1913@gmail.com",
     description="Shyna Speak package, Phase one",
     long_description=long_description,
     long_description_content_type="text/markdown",
 )
```

