# Comparing `tmp/dg-itest-0.0.8.tar.gz` & `tmp/dg-itest-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dg-itest-0.0.8.tar", last modified: Sun Apr 23 03:40:20 2023, max compression
+gzip compressed data, was "dg-itest-0.0.9.tar", last modified: Sun Apr 23 04:49:11 2023, max compression
```

## Comparing `dg-itest-0.0.8.tar` & `dg-itest-0.0.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-23 03:40:20.520391 dg-itest-0.0.8/
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      286 2023-04-23 03:40:20.520274 dg-itest-0.0.8/PKG-INFO
--rw-r--r--   0 yaitzayoung   (501) staff       (20)     5861 2023-04-21 02:26:19.000000 dg-itest-0.0.8/README.md
-drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-23 03:40:20.515744 dg-itest-0.0.8/dg_itest/
--rw-r--r--   0 yaitzayoung   (501) staff       (20)     1738 2023-04-21 07:56:28.000000 dg-itest-0.0.8/dg_itest/__init__.py
-drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-23 03:40:20.516970 dg-itest-0.0.8/dg_itest/servers/
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      127 2023-04-21 01:59:08.000000 dg-itest-0.0.8/dg_itest/servers/__init__.py
-drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-23 03:40:20.517655 dg-itest-0.0.8/dg_itest/servers/dg_servers/
--rw-r--r--   0 yaitzayoung   (501) staff       (20)        0 2023-04-21 01:59:08.000000 dg-itest-0.0.8/dg_itest/servers/dg_servers/__init__.py
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      793 2023-04-21 01:59:08.000000 dg-itest-0.0.8/dg_itest/servers/dg_servers/dg_requsts.py
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      531 2023-04-21 01:59:08.000000 dg-itest-0.0.8/dg_itest/servers/dg_servers/dg_singleton.py
-drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-23 03:40:20.518277 dg-itest-0.0.8/dg_itest/servers/file_handler/
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      127 2023-04-21 01:59:08.000000 dg-itest-0.0.8/dg_itest/servers/file_handler/__init__.py
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      591 2023-04-21 01:59:08.000000 dg-itest-0.0.8/dg_itest/servers/file_handler/file_handler.py
--rw-r--r--   0 yaitzayoung   (501) staff       (20)     1470 2023-04-21 01:59:08.000000 dg-itest-0.0.8/dg_itest/servers/file_handler/xlsx_handler.py
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      343 2023-04-21 01:59:08.000000 dg-itest-0.0.8/dg_itest/servers/file_handler/yaml_handler.py
-drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-23 03:40:20.518693 dg-itest-0.0.8/dg_itest/servers/test_handler/
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      127 2023-04-21 01:59:08.000000 dg-itest-0.0.8/dg_itest/servers/test_handler/__init__.py
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      558 2023-04-21 01:59:08.000000 dg-itest-0.0.8/dg_itest/servers/test_handler/test_file.py
--rw-r--r--   0 yaitzayoung   (501) staff       (20)     3720 2023-04-23 03:40:10.000000 dg-itest-0.0.8/dg_itest/servers/test_handler/test_item.py
-drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-23 03:40:20.519736 dg-itest-0.0.8/dg_itest/utils/
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      127 2023-04-21 01:59:08.000000 dg-itest-0.0.8/dg_itest/utils/__init__.py
--rw-r--r--   0 yaitzayoung   (501) staff       (20)       39 2023-04-23 03:40:10.000000 dg-itest-0.0.8/dg_itest/utils/cache.py
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      661 2023-04-21 01:59:08.000000 dg-itest-0.0.8/dg_itest/utils/diff_helper.py
--rw-r--r--   0 yaitzayoung   (501) staff       (20)     1276 2023-04-21 01:59:08.000000 dg-itest-0.0.8/dg_itest/utils/env_generater.py
--rw-r--r--   0 yaitzayoung   (501) staff       (20)     1594 2023-04-23 02:56:10.000000 dg-itest-0.0.8/dg_itest/utils/replace.py
--rw-r--r--   0 yaitzayoung   (501) staff       (20)     1209 2023-04-21 01:59:08.000000 dg-itest-0.0.8/dg_itest/utils/string_helper.py
-drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-23 03:40:20.516773 dg-itest-0.0.8/dg_itest.egg-info/
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      286 2023-04-23 03:40:20.000000 dg-itest-0.0.8/dg_itest.egg-info/PKG-INFO
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      884 2023-04-23 03:40:20.000000 dg-itest-0.0.8/dg_itest.egg-info/SOURCES.txt
--rw-r--r--   0 yaitzayoung   (501) staff       (20)        1 2023-04-23 03:40:20.000000 dg-itest-0.0.8/dg_itest.egg-info/dependency_links.txt
--rw-r--r--   0 yaitzayoung   (501) staff       (20)        1 2023-04-23 03:40:20.000000 dg-itest-0.0.8/dg_itest.egg-info/not-zip-safe
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      362 2023-04-23 03:40:20.000000 dg-itest-0.0.8/dg_itest.egg-info/requires.txt
--rw-r--r--   0 yaitzayoung   (501) staff       (20)        9 2023-04-23 03:40:20.000000 dg-itest-0.0.8/dg_itest.egg-info/top_level.txt
--rw-r--r--   0 yaitzayoung   (501) staff       (20)       38 2023-04-23 03:40:20.520444 dg-itest-0.0.8/setup.cfg
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      879 2023-04-23 03:40:18.000000 dg-itest-0.0.8/setup.py
-drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-23 03:40:20.519874 dg-itest-0.0.8/test/
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      549 2023-04-23 02:09:23.000000 dg-itest-0.0.8/test/test_replace.py
+drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-23 04:49:11.587769 dg-itest-0.0.9/
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      286 2023-04-23 04:49:11.587673 dg-itest-0.0.9/PKG-INFO
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)     5861 2023-04-21 02:26:19.000000 dg-itest-0.0.9/README.md
+drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-23 04:49:11.583369 dg-itest-0.0.9/dg_itest/
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)     1738 2023-04-21 07:56:28.000000 dg-itest-0.0.9/dg_itest/__init__.py
+drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-23 04:49:11.584386 dg-itest-0.0.9/dg_itest/servers/
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      127 2023-04-21 01:59:08.000000 dg-itest-0.0.9/dg_itest/servers/__init__.py
+drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-23 04:49:11.584968 dg-itest-0.0.9/dg_itest/servers/dg_servers/
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)        0 2023-04-21 01:59:08.000000 dg-itest-0.0.9/dg_itest/servers/dg_servers/__init__.py
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      793 2023-04-21 01:59:08.000000 dg-itest-0.0.9/dg_itest/servers/dg_servers/dg_requsts.py
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      531 2023-04-21 01:59:08.000000 dg-itest-0.0.9/dg_itest/servers/dg_servers/dg_singleton.py
+drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-23 04:49:11.585506 dg-itest-0.0.9/dg_itest/servers/file_handler/
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      127 2023-04-21 01:59:08.000000 dg-itest-0.0.9/dg_itest/servers/file_handler/__init__.py
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      591 2023-04-21 01:59:08.000000 dg-itest-0.0.9/dg_itest/servers/file_handler/file_handler.py
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)     1470 2023-04-21 01:59:08.000000 dg-itest-0.0.9/dg_itest/servers/file_handler/xlsx_handler.py
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      343 2023-04-21 01:59:08.000000 dg-itest-0.0.9/dg_itest/servers/file_handler/yaml_handler.py
+drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-23 04:49:11.585859 dg-itest-0.0.9/dg_itest/servers/test_handler/
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      127 2023-04-21 01:59:08.000000 dg-itest-0.0.9/dg_itest/servers/test_handler/__init__.py
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      558 2023-04-21 01:59:08.000000 dg-itest-0.0.9/dg_itest/servers/test_handler/test_file.py
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)     3689 2023-04-23 04:48:15.000000 dg-itest-0.0.9/dg_itest/servers/test_handler/test_item.py
+drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-23 04:49:11.587103 dg-itest-0.0.9/dg_itest/utils/
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      127 2023-04-21 01:59:08.000000 dg-itest-0.0.9/dg_itest/utils/__init__.py
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)       53 2023-04-23 04:47:45.000000 dg-itest-0.0.9/dg_itest/utils/cache.py
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      661 2023-04-21 01:59:08.000000 dg-itest-0.0.9/dg_itest/utils/diff_helper.py
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)     1276 2023-04-21 01:59:08.000000 dg-itest-0.0.9/dg_itest/utils/env_generater.py
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)     1599 2023-04-23 04:43:41.000000 dg-itest-0.0.9/dg_itest/utils/replace.py
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)     1209 2023-04-21 01:59:08.000000 dg-itest-0.0.9/dg_itest/utils/string_helper.py
+drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-23 04:49:11.584288 dg-itest-0.0.9/dg_itest.egg-info/
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      286 2023-04-23 04:49:11.000000 dg-itest-0.0.9/dg_itest.egg-info/PKG-INFO
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      884 2023-04-23 04:49:11.000000 dg-itest-0.0.9/dg_itest.egg-info/SOURCES.txt
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)        1 2023-04-23 04:49:11.000000 dg-itest-0.0.9/dg_itest.egg-info/dependency_links.txt
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)        1 2023-04-23 04:49:11.000000 dg-itest-0.0.9/dg_itest.egg-info/not-zip-safe
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      362 2023-04-23 04:49:11.000000 dg-itest-0.0.9/dg_itest.egg-info/requires.txt
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)        9 2023-04-23 04:49:11.000000 dg-itest-0.0.9/dg_itest.egg-info/top_level.txt
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)       38 2023-04-23 04:49:11.587801 dg-itest-0.0.9/setup.cfg
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      879 2023-04-23 04:48:56.000000 dg-itest-0.0.9/setup.py
+drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-23 04:49:11.587275 dg-itest-0.0.9/test/
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      549 2023-04-23 02:09:23.000000 dg-itest-0.0.9/test/test_replace.py
```

### Comparing `dg-itest-0.0.8/README.md` & `dg-itest-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `dg-itest-0.0.8/dg_itest/__init__.py` & `dg-itest-0.0.9/dg_itest/__init__.py`

 * *Files identical despite different names*

### Comparing `dg-itest-0.0.8/dg_itest/servers/dg_servers/dg_requsts.py` & `dg-itest-0.0.9/dg_itest/servers/dg_servers/dg_requsts.py`

 * *Files identical despite different names*

### Comparing `dg-itest-0.0.8/dg_itest/servers/dg_servers/dg_singleton.py` & `dg-itest-0.0.9/dg_itest/servers/dg_servers/dg_singleton.py`

 * *Files identical despite different names*

### Comparing `dg-itest-0.0.8/dg_itest/servers/file_handler/file_handler.py` & `dg-itest-0.0.9/dg_itest/servers/file_handler/file_handler.py`

 * *Files identical despite different names*

### Comparing `dg-itest-0.0.8/dg_itest/servers/file_handler/xlsx_handler.py` & `dg-itest-0.0.9/dg_itest/servers/file_handler/xlsx_handler.py`

 * *Files identical despite different names*

### Comparing `dg-itest-0.0.8/dg_itest/servers/test_handler/test_file.py` & `dg-itest-0.0.9/dg_itest/servers/test_handler/test_file.py`

 * *Files identical despite different names*

### Comparing `dg-itest-0.0.8/dg_itest/servers/test_handler/test_item.py` & `dg-itest-0.0.9/dg_itest/servers/test_handler/test_item.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,20 +21,19 @@
         self.name = name
         self.values = values
         self.request = self.values.get("request")
         self.validate = self.values.get("validate")
         self.expect = self.values.get('expect')
 
     def runtest(self):
-        request_data = self.values['request']
-        params = self.replace(request_data)
-        params = request_data['params']
+        request_data = self.replace(self.values['request'])
+        params = request_data.get("params")
         if "files" in params.keys():
-                params.update({"files": self.get_files(params.get("files"))})
-        request_data.pop('params')
+            params.update({"files": self.get_files(params.get("files"))})
+        request_data.pop("params")
         request_data.update(params)
 
         try:
             api = DgSingleton().apis
             response = api.http_request(**request_data)
         except Exception as ex:
             print("request Error！\n" + str(ex))
@@ -54,24 +53,24 @@
                     expect_result = sorted(expect_result)
                 assert actual_result == expect_result, '\n' + DiffHelper.diff(str(actual_result), str(expect_result))
             if "sa" in item.keys():
                 sa_value = item.get("sa")
                 for sa_item_key in sa_value.keys():
                     sa_item_value =  jsonpath.jsonpath(response.json(), sa_value.get(sa_item_key))
                     assert type(sa_item_value) is list and len(sa_item_value) > 0, '\n' + '未获取到值'
-                    local_cache.update({f"${sa_item_key}$": sa_item_value[0]})
+                    local_cache.put(f"${sa_item_key}$", sa_item_value[0])
 
     def replace(self, source):
         pattern_str = r'\$.*?\$'
         source_str = json.dumps(source)
         pattern = re.compile(pattern_str, re.DOTALL)
         match_items = pattern.findall(source_str)
         update = {}
         for items in match_items:
-            update.update({items: local_cache[items]})
+            update.update({items: local_cache.get(items)})
         if len(update.keys()) > 0:
             result = Replace.replace(pattern_str, source, update)
             return result
         else:
             return source
 
     def get_files(self, files_array):
```

### Comparing `dg-itest-0.0.8/dg_itest/utils/diff_helper.py` & `dg-itest-0.0.9/dg_itest/utils/diff_helper.py`

 * *Files identical despite different names*

### Comparing `dg-itest-0.0.8/dg_itest/utils/env_generater.py` & `dg-itest-0.0.9/dg_itest/utils/env_generater.py`

 * *Files identical despite different names*

### Comparing `dg-itest-0.0.8/dg_itest/utils/replace.py` & `dg-itest-0.0.9/dg_itest/utils/replace.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 		elif isinstance(v, list):
 			if match_item in v:
 				match_index = v.index(match_item)
 				v[match_index] = update
 				source.update({k: v})
 		elif isinstance(v, str):
 			if v == match_item:
-				source.update({k: v})
+				source.update({k: update})
 			elif v.__contains__(match_item):
 				replace_v = v.replace(match_item, str(update))
 				source.update({k: replace_v})
 			else:
 				pass
 		else:
 			pass
```

### Comparing `dg-itest-0.0.8/dg_itest/utils/string_helper.py` & `dg-itest-0.0.9/dg_itest/utils/string_helper.py`

 * *Files identical despite different names*

### Comparing `dg-itest-0.0.8/dg_itest.egg-info/SOURCES.txt` & `dg-itest-0.0.9/dg_itest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dg-itest-0.0.8/setup.py` & `dg-itest-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     if not os.path.exists(requirements):  # install from tar
         requirements = 'dg_itest.egg-info/requires.txt'
     with open(requirements) as fp:
         install_requires = fp.read()
     return install_requires.split('\n')
 
 setup(name='dg-itest',
-      version='0.0.8',
+      version='0.0.9',
       description='接口自动化测试框架',
       url='https://github.com/yaitza/dg-itest',
       download_url='https://github.com/yaitza/dg-itest/releases',
       author='yaitza',
       author_email='yaitza@foxmail.com',
       packages=find_packages(),
       package_data={'': ['*.py']},
```

### Comparing `dg-itest-0.0.8/test/test_replace.py` & `dg-itest-0.0.9/test/test_replace.py`

 * *Files identical despite different names*

