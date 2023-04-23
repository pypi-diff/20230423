# Comparing `tmp/common-xmjz-0.1.2.tar.gz` & `tmp/common-xmjz-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\common-xmjz-0.1.2.tar", last modified: Sun Apr 23 10:58:12 2023, max compression
+gzip compressed data, was "dist\common-xmjz-0.1.3.tar", last modified: Sun Apr 23 11:45:15 2023, max compression
```

## Comparing `common-xmjz-0.1.2.tar` & `common-xmjz-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 10:58:12.372532 common-xmjz-0.1.2/
--rw-rw-rw-   0        0        0      634 2023-04-23 10:58:12.372532 common-xmjz-0.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-23 10:58:12.371533 common-xmjz-0.1.2/common_xmjz.egg-info/
--rw-rw-rw-   0        0        0      634 2023-04-23 10:58:12.000000 common-xmjz-0.1.2/common_xmjz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      256 2023-04-23 10:58:12.000000 common-xmjz-0.1.2/common_xmjz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 10:58:12.000000 common-xmjz-0.1.2/common_xmjz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-04-23 10:58:12.000000 common-xmjz-0.1.2/common_xmjz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 10:58:12.372532 common-xmjz-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     3879 2023-04-23 10:54:42.000000 common-xmjz-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-23 10:58:12.371533 common-xmjz-0.1.2/xmjz/
--rw-rw-rw-   0        0        0        0 2023-04-23 10:43:32.000000 common-xmjz-0.1.2/xmjz/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 10:58:12.371533 common-xmjz-0.1.2/xmjz/common/
--rw-rw-rw-   0        0        0        0 2023-04-23 10:43:32.000000 common-xmjz-0.1.2/xmjz/common/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 10:58:12.372532 common-xmjz-0.1.2/xmjz/common/mysql/
--rw-rw-rw-   0        0        0        0 2023-04-23 10:07:49.000000 common-xmjz-0.1.2/xmjz/common/mysql/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 10:58:12.372532 common-xmjz-0.1.2/xmjz/common/mysql/helper/
--rw-rw-rw-   0        0        0     1946 2023-04-23 10:57:08.000000 common-xmjz-0.1.2/xmjz/common/mysql/helper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 11:45:15.184267 common-xmjz-0.1.3/
+-rw-rw-rw-   0        0        0      634 2023-04-23 11:45:15.184267 common-xmjz-0.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-23 11:45:15.183267 common-xmjz-0.1.3/common_xmjz.egg-info/
+-rw-rw-rw-   0        0        0      634 2023-04-23 11:45:15.000000 common-xmjz-0.1.3/common_xmjz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      256 2023-04-23 11:45:15.000000 common-xmjz-0.1.3/common_xmjz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 11:45:15.000000 common-xmjz-0.1.3/common_xmjz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-04-23 11:45:15.000000 common-xmjz-0.1.3/common_xmjz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 11:45:15.184267 common-xmjz-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     3879 2023-04-23 11:45:03.000000 common-xmjz-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 11:45:15.183267 common-xmjz-0.1.3/xmjz/
+-rw-rw-rw-   0        0        0        0 2023-04-23 10:43:32.000000 common-xmjz-0.1.3/xmjz/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 11:45:15.183267 common-xmjz-0.1.3/xmjz/common/
+-rw-rw-rw-   0        0        0        0 2023-04-23 10:43:32.000000 common-xmjz-0.1.3/xmjz/common/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 11:45:15.184267 common-xmjz-0.1.3/xmjz/common/mysql/
+-rw-rw-rw-   0        0        0        0 2023-04-23 10:07:49.000000 common-xmjz-0.1.3/xmjz/common/mysql/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 11:45:15.184267 common-xmjz-0.1.3/xmjz/common/mysql/helper/
+-rw-rw-rw-   0        0        0     2181 2023-04-23 11:43:39.000000 common-xmjz-0.1.3/xmjz/common/mysql/helper/__init__.py
```

### Comparing `common-xmjz-0.1.2/PKG-INFO` & `common-xmjz-0.1.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: common-xmjz
-Version: 0.1.2
+Version: 0.1.3
 Summary: common-xmjz
 Home-page: https://github.com/me/myproject
 Author: xmjz
 Author-email: xxx@example.com
 License: MIT
 Description: common-xmjz
 Platform: UNKNOWN
```

### Comparing `common-xmjz-0.1.2/common_xmjz.egg-info/PKG-INFO` & `common-xmjz-0.1.3/common_xmjz.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: common-xmjz
-Version: 0.1.2
+Version: 0.1.3
 Summary: common-xmjz
 Home-page: https://github.com/me/myproject
 Author: xmjz
 Author-email: xxx@example.com
 License: MIT
 Description: common-xmjz
 Platform: UNKNOWN
```

### Comparing `common-xmjz-0.1.2/setup.py` & `common-xmjz-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'common-xmjz'
 DESCRIPTION = 'common-xmjz'
 URL = 'https://github.com/me/myproject'
 EMAIL = 'xxx@example.com'
 AUTHOR = 'xmjz'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.2'
+VERSION = '0.1.3'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

### Comparing `common-xmjz-0.1.2/xmjz/common/mysql/helper/__init__.py` & `common-xmjz-0.1.3/xmjz/common/mysql/helper/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,64 +18,72 @@
         执行Sql语句
         :param sql:
         :param args:
         :return:(fields,rows )
         """
         c = self.conn.cursor()
         c.execute(sql, args)
+        c.close()
         thead = [e[0] for e in c.description]
         tbody = c.fetchall()
         return thead, tbody
 
-    def query_for_map(self, sql, args=None):
+    def query_dict(self, sql, args=None):
         """
-        执行Sql语句
+        执行Sql语句 返回字典
         :param sql:
         :param args:
-        :return:map
+        :return:(fields,rows )
         """
-        fields, rows = self.query(sql, args)
-        return self.map_list(fields, rows)
+        c = self.conn.cursor(pymysql.cursors.DictCursor)
+        c.execute(sql, args)
+        c.close()
+        datas = c.fetchall()
+        return datas
 
     def update(self, sql, args=None):
         """
         执行Sql语句
         :param sql:
         :param args:
         """
+        c = self.conn.cursor()
         try:
-            c = self.conn.cursor()
             i = c.execute(sql, args)
             self.conn.commit()
             return i
         except Exception as e:
             self.conn.rollback()
             # 事务回滚
             logger.error('事务处理失败', e)
             raise e
+        finally:
+            c.close()
 
-    def updatemany(self, sql, args):
+    def update_many(self, sql, args):
         """
         执行Sql语句
-        :param sql:
+        :param sql: 参数为tuple时用%s,为dict时用%(name)
         :param args:
         """
+        c = self.conn.cursor()
         try:
-            c = self.conn.cursor()
             i = c.executemany(sql, args)
-            conn.commit()
+            self.conn.commit()
             return i
         except Exception as e:
             self.conn.rollback()
             # 事务回滚
             logger.error('事务处理失败', e)
             raise e
+        finally:
+            c.close()
 
     @staticmethod
     def map_list(fields, rows):
         datarow = []
         for row in rows:
             temp = {}
             for i, e in enumerate(fields):
                 temp[e] = row[i]
             datarow.append(temp)
-        return datarow
+        return datarow
```

