# Comparing `tmp/dg-itest-0.0.6.tar.gz` & `tmp/dg-itest-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dg-itest-0.0.6.tar", last modified: Sun Apr 23 03:05:02 2023, max compression
+gzip compressed data, was "dg-itest-0.0.7.tar", last modified: Sun Apr 23 03:32:08 2023, max compression
```

## Comparing `dg-itest-0.0.6.tar` & `dg-itest-0.0.7.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-23 03:05:02.715687 dg-itest-0.0.6/
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      286 2023-04-23 03:05:02.715571 dg-itest-0.0.6/PKG-INFO
--rw-r--r--   0 yaitzayoung   (501) staff       (20)     5861 2023-04-21 02:26:19.000000 dg-itest-0.0.6/README.md
-drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-23 03:05:02.710847 dg-itest-0.0.6/dg_itest/
--rw-r--r--   0 yaitzayoung   (501) staff       (20)     1738 2023-04-21 07:56:28.000000 dg-itest-0.0.6/dg_itest/__init__.py
-drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-23 03:05:02.711798 dg-itest-0.0.6/dg_itest/servers/
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      127 2023-04-21 01:59:08.000000 dg-itest-0.0.6/dg_itest/servers/__init__.py
-drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-23 03:05:02.712493 dg-itest-0.0.6/dg_itest/servers/dg_servers/
--rw-r--r--   0 yaitzayoung   (501) staff       (20)        0 2023-04-21 01:59:08.000000 dg-itest-0.0.6/dg_itest/servers/dg_servers/__init__.py
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      793 2023-04-21 01:59:08.000000 dg-itest-0.0.6/dg_itest/servers/dg_servers/dg_requsts.py
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      531 2023-04-21 01:59:08.000000 dg-itest-0.0.6/dg_itest/servers/dg_servers/dg_singleton.py
-drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-23 03:05:02.713103 dg-itest-0.0.6/dg_itest/servers/file_handler/
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      127 2023-04-21 01:59:08.000000 dg-itest-0.0.6/dg_itest/servers/file_handler/__init__.py
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      591 2023-04-21 01:59:08.000000 dg-itest-0.0.6/dg_itest/servers/file_handler/file_handler.py
--rw-r--r--   0 yaitzayoung   (501) staff       (20)     1470 2023-04-21 01:59:08.000000 dg-itest-0.0.6/dg_itest/servers/file_handler/xlsx_handler.py
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      343 2023-04-21 01:59:08.000000 dg-itest-0.0.6/dg_itest/servers/file_handler/yaml_handler.py
-drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-23 03:05:02.713549 dg-itest-0.0.6/dg_itest/servers/test_handler/
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      127 2023-04-21 01:59:08.000000 dg-itest-0.0.6/dg_itest/servers/test_handler/__init__.py
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      558 2023-04-21 01:59:08.000000 dg-itest-0.0.6/dg_itest/servers/test_handler/test_file.py
--rw-r--r--   0 yaitzayoung   (501) staff       (20)     3712 2023-04-23 01:37:13.000000 dg-itest-0.0.6/dg_itest/servers/test_handler/test_item.py
-drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-23 03:05:02.715000 dg-itest-0.0.6/dg_itest/utils/
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      127 2023-04-21 01:59:08.000000 dg-itest-0.0.6/dg_itest/utils/__init__.py
--rw-r--r--   0 yaitzayoung   (501) staff       (20)       53 2023-04-21 11:38:22.000000 dg-itest-0.0.6/dg_itest/utils/cache.py
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      661 2023-04-21 01:59:08.000000 dg-itest-0.0.6/dg_itest/utils/diff_helper.py
--rw-r--r--   0 yaitzayoung   (501) staff       (20)     1276 2023-04-21 01:59:08.000000 dg-itest-0.0.6/dg_itest/utils/env_generater.py
--rw-r--r--   0 yaitzayoung   (501) staff       (20)     1594 2023-04-23 02:56:10.000000 dg-itest-0.0.6/dg_itest/utils/replace.py
--rw-r--r--   0 yaitzayoung   (501) staff       (20)     1209 2023-04-21 01:59:08.000000 dg-itest-0.0.6/dg_itest/utils/string_helper.py
-drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-23 03:05:02.711702 dg-itest-0.0.6/dg_itest.egg-info/
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      286 2023-04-23 03:05:02.000000 dg-itest-0.0.6/dg_itest.egg-info/PKG-INFO
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      884 2023-04-23 03:05:02.000000 dg-itest-0.0.6/dg_itest.egg-info/SOURCES.txt
--rw-r--r--   0 yaitzayoung   (501) staff       (20)        1 2023-04-23 03:05:02.000000 dg-itest-0.0.6/dg_itest.egg-info/dependency_links.txt
--rw-r--r--   0 yaitzayoung   (501) staff       (20)        1 2023-04-23 03:05:02.000000 dg-itest-0.0.6/dg_itest.egg-info/not-zip-safe
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      362 2023-04-23 03:05:02.000000 dg-itest-0.0.6/dg_itest.egg-info/requires.txt
--rw-r--r--   0 yaitzayoung   (501) staff       (20)        9 2023-04-23 03:05:02.000000 dg-itest-0.0.6/dg_itest.egg-info/top_level.txt
--rw-r--r--   0 yaitzayoung   (501) staff       (20)       38 2023-04-23 03:05:02.715741 dg-itest-0.0.6/setup.cfg
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      879 2023-04-23 03:04:59.000000 dg-itest-0.0.6/setup.py
-drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-23 03:05:02.715190 dg-itest-0.0.6/test/
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      549 2023-04-23 02:09:23.000000 dg-itest-0.0.6/test/test_replace.py
+drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-23 03:32:08.831612 dg-itest-0.0.7/
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      286 2023-04-23 03:32:08.831512 dg-itest-0.0.7/PKG-INFO
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)     5861 2023-04-21 02:26:19.000000 dg-itest-0.0.7/README.md
+drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-23 03:32:08.827434 dg-itest-0.0.7/dg_itest/
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)     1738 2023-04-21 07:56:28.000000 dg-itest-0.0.7/dg_itest/__init__.py
+drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-23 03:32:08.828418 dg-itest-0.0.7/dg_itest/servers/
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      127 2023-04-21 01:59:08.000000 dg-itest-0.0.7/dg_itest/servers/__init__.py
+drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-23 03:32:08.828998 dg-itest-0.0.7/dg_itest/servers/dg_servers/
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)        0 2023-04-21 01:59:08.000000 dg-itest-0.0.7/dg_itest/servers/dg_servers/__init__.py
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      793 2023-04-21 01:59:08.000000 dg-itest-0.0.7/dg_itest/servers/dg_servers/dg_requsts.py
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      531 2023-04-21 01:59:08.000000 dg-itest-0.0.7/dg_itest/servers/dg_servers/dg_singleton.py
+drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-23 03:32:08.829528 dg-itest-0.0.7/dg_itest/servers/file_handler/
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      127 2023-04-21 01:59:08.000000 dg-itest-0.0.7/dg_itest/servers/file_handler/__init__.py
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      591 2023-04-21 01:59:08.000000 dg-itest-0.0.7/dg_itest/servers/file_handler/file_handler.py
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)     1470 2023-04-21 01:59:08.000000 dg-itest-0.0.7/dg_itest/servers/file_handler/xlsx_handler.py
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      343 2023-04-21 01:59:08.000000 dg-itest-0.0.7/dg_itest/servers/file_handler/yaml_handler.py
+drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-23 03:32:08.829887 dg-itest-0.0.7/dg_itest/servers/test_handler/
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      127 2023-04-21 01:59:08.000000 dg-itest-0.0.7/dg_itest/servers/test_handler/__init__.py
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      558 2023-04-21 01:59:08.000000 dg-itest-0.0.7/dg_itest/servers/test_handler/test_file.py
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)     3715 2023-04-23 03:30:34.000000 dg-itest-0.0.7/dg_itest/servers/test_handler/test_item.py
+drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-23 03:32:08.831062 dg-itest-0.0.7/dg_itest/utils/
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      127 2023-04-21 01:59:08.000000 dg-itest-0.0.7/dg_itest/utils/__init__.py
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)       53 2023-04-21 11:38:22.000000 dg-itest-0.0.7/dg_itest/utils/cache.py
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      661 2023-04-21 01:59:08.000000 dg-itest-0.0.7/dg_itest/utils/diff_helper.py
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)     1276 2023-04-21 01:59:08.000000 dg-itest-0.0.7/dg_itest/utils/env_generater.py
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)     1594 2023-04-23 02:56:10.000000 dg-itest-0.0.7/dg_itest/utils/replace.py
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)     1209 2023-04-21 01:59:08.000000 dg-itest-0.0.7/dg_itest/utils/string_helper.py
+drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-23 03:32:08.828310 dg-itest-0.0.7/dg_itest.egg-info/
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      286 2023-04-23 03:32:08.000000 dg-itest-0.0.7/dg_itest.egg-info/PKG-INFO
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      884 2023-04-23 03:32:08.000000 dg-itest-0.0.7/dg_itest.egg-info/SOURCES.txt
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)        1 2023-04-23 03:32:08.000000 dg-itest-0.0.7/dg_itest.egg-info/dependency_links.txt
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)        1 2023-04-23 03:32:08.000000 dg-itest-0.0.7/dg_itest.egg-info/not-zip-safe
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      362 2023-04-23 03:32:08.000000 dg-itest-0.0.7/dg_itest.egg-info/requires.txt
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)        9 2023-04-23 03:32:08.000000 dg-itest-0.0.7/dg_itest.egg-info/top_level.txt
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)       38 2023-04-23 03:32:08.831644 dg-itest-0.0.7/setup.cfg
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      879 2023-04-23 03:32:06.000000 dg-itest-0.0.7/setup.py
+drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-23 03:32:08.831219 dg-itest-0.0.7/test/
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      549 2023-04-23 02:09:23.000000 dg-itest-0.0.7/test/test_replace.py
```

### Comparing `dg-itest-0.0.6/README.md` & `dg-itest-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `dg-itest-0.0.6/dg_itest/__init__.py` & `dg-itest-0.0.7/dg_itest/__init__.py`

 * *Files identical despite different names*

### Comparing `dg-itest-0.0.6/dg_itest/servers/dg_servers/dg_requsts.py` & `dg-itest-0.0.7/dg_itest/servers/dg_servers/dg_requsts.py`

 * *Files identical despite different names*

### Comparing `dg-itest-0.0.6/dg_itest/servers/dg_servers/dg_singleton.py` & `dg-itest-0.0.7/dg_itest/servers/dg_servers/dg_singleton.py`

 * *Files identical despite different names*

### Comparing `dg-itest-0.0.6/dg_itest/servers/file_handler/file_handler.py` & `dg-itest-0.0.7/dg_itest/servers/file_handler/file_handler.py`

 * *Files identical despite different names*

### Comparing `dg-itest-0.0.6/dg_itest/servers/file_handler/xlsx_handler.py` & `dg-itest-0.0.7/dg_itest/servers/file_handler/xlsx_handler.py`

 * *Files identical despite different names*

### Comparing `dg-itest-0.0.6/dg_itest/servers/test_handler/test_file.py` & `dg-itest-0.0.7/dg_itest/servers/test_handler/test_file.py`

 * *Files identical despite different names*

### Comparing `dg-itest-0.0.6/dg_itest/servers/test_handler/test_item.py` & `dg-itest-0.0.7/dg_itest/servers/test_handler/test_item.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
                     expect_result = sorted(expect_result)
                 assert actual_result == expect_result, '\n' + DiffHelper.diff(str(actual_result), str(expect_result))
             if "sa" in item.keys():
                 sa_value = item.get("sa")
                 for sa_item_key in sa_value.keys():
                     sa_item_value =  jsonpath.jsonpath(response.json(), sa_value.get(sa_item_key))
                     assert type(sa_item_value) is list and len(sa_item_value) > 0, '\n' + '未获取到值'
-                    local_cache[f"${sa_item_key}$"] = sa_item_value[0]
+                    local_cache.put(f"${sa_item_key}$", sa_item_value[0])
 
     def replace(self, source):
         pattern_str = r'\$.*?\$'
         source_str = json.dumps(source)
         pattern = re.compile(pattern_str, re.DOTALL)
         match_items = pattern.findall(source_str)
         update = {}
```

### Comparing `dg-itest-0.0.6/dg_itest/utils/diff_helper.py` & `dg-itest-0.0.7/dg_itest/utils/diff_helper.py`

 * *Files identical despite different names*

### Comparing `dg-itest-0.0.6/dg_itest/utils/env_generater.py` & `dg-itest-0.0.7/dg_itest/utils/env_generater.py`

 * *Files identical despite different names*

### Comparing `dg-itest-0.0.6/dg_itest/utils/replace.py` & `dg-itest-0.0.7/dg_itest/utils/replace.py`

 * *Files identical despite different names*

### Comparing `dg-itest-0.0.6/dg_itest/utils/string_helper.py` & `dg-itest-0.0.7/dg_itest/utils/string_helper.py`

 * *Files identical despite different names*

### Comparing `dg-itest-0.0.6/dg_itest.egg-info/SOURCES.txt` & `dg-itest-0.0.7/dg_itest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dg-itest-0.0.6/setup.py` & `dg-itest-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     if not os.path.exists(requirements):  # install from tar
         requirements = 'dg_itest.egg-info/requires.txt'
     with open(requirements) as fp:
         install_requires = fp.read()
     return install_requires.split('\n')
 
 setup(name='dg-itest',
-      version='0.0.6',
+      version='0.0.7',
       description='接口自动化测试框架',
       url='https://github.com/yaitza/dg-itest',
       download_url='https://github.com/yaitza/dg-itest/releases',
       author='yaitza',
       author_email='yaitza@foxmail.com',
       packages=find_packages(),
       package_data={'': ['*.py']},
```

### Comparing `dg-itest-0.0.6/test/test_replace.py` & `dg-itest-0.0.7/test/test_replace.py`

 * *Files identical despite different names*

