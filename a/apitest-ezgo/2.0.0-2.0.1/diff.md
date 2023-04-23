# Comparing `tmp/apitest_ezgo-2.0.0-py2.py3-none-any.whl.zip` & `tmp/apitest_ezgo-2.0.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 13925 bytes, number of entries: 15
+Zip file size: 14004 bytes, number of entries: 15
 -rw-rw-rw-  2.0 fat     5287 b- defN 23-Apr-23 02:33 apitest_ezgo/Compare.py
--rw-rw-rw-  2.0 fat     9890 b- defN 23-Apr-21 10:09 apitest_ezgo/DbHelper.py
+-rw-rw-rw-  2.0 fat    10011 b- defN 23-Apr-23 07:34 apitest_ezgo/DbHelper.py
 -rw-rw-rw-  2.0 fat     4035 b- defN 23-Apr-10 07:13 apitest_ezgo/FastRequest.py
--rw-rw-rw-  2.0 fat      237 b- defN 23-Apr-23 02:24 apitest_ezgo/__about__.py
+-rw-rw-rw-  2.0 fat      237 b- defN 23-Apr-23 06:32 apitest_ezgo/__about__.py
 -rw-rw-rw-  2.0 fat       53 b- defN 23-Feb-09 11:57 apitest_ezgo/__init__.py
 -rw-rw-rw-  2.0 fat      901 b- defN 23-Apr-21 09:59 apitest_ezgo/compat.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jan-16 03:14 apitest_ezgo/Har2Template/__init__.py
 -rw-rw-rw-  2.0 fat     1844 b- defN 23-Apr-23 06:27 apitest_ezgo/Har2Template/cli.py
 -rw-rw-rw-  2.0 fat     6466 b- defN 23-Apr-21 09:44 apitest_ezgo/Har2Template/core.py
 -rw-rw-rw-  2.0 fat     3506 b- defN 23-Apr-21 09:44 apitest_ezgo/Har2Template/utils.py
--rw-rw-rw-  2.0 fat      366 b- defN 23-Apr-23 06:28 apitest_ezgo-2.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Apr-23 06:28 apitest_ezgo-2.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       69 b- defN 23-Apr-23 06:28 apitest_ezgo-2.0.0.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       13 b- defN 23-Apr-23 06:28 apitest_ezgo-2.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1262 b- defN 23-Apr-23 06:28 apitest_ezgo-2.0.0.dist-info/RECORD
-15 files, 34039 bytes uncompressed, 11815 bytes compressed:  65.3%
+-rw-rw-rw-  2.0 fat      501 b- defN 23-Apr-23 07:37 apitest_ezgo-2.0.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Apr-23 07:37 apitest_ezgo-2.0.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       69 b- defN 23-Apr-23 07:37 apitest_ezgo-2.0.1.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       13 b- defN 23-Apr-23 07:37 apitest_ezgo-2.0.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1263 b- defN 23-Apr-23 07:37 apitest_ezgo-2.0.1.dist-info/RECORD
+15 files, 34296 bytes uncompressed, 11894 bytes compressed:  65.3%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: apitest_ezgo/Har2Template/core.py
 Comment: 
 
 Filename: apitest_ezgo/Har2Template/utils.py
 Comment: 
 
-Filename: apitest_ezgo-2.0.0.dist-info/METADATA
+Filename: apitest_ezgo-2.0.1.dist-info/METADATA
 Comment: 
 
-Filename: apitest_ezgo-2.0.0.dist-info/WHEEL
+Filename: apitest_ezgo-2.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: apitest_ezgo-2.0.0.dist-info/entry_points.txt
+Filename: apitest_ezgo-2.0.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: apitest_ezgo-2.0.0.dist-info/top_level.txt
+Filename: apitest_ezgo-2.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: apitest_ezgo-2.0.0.dist-info/RECORD
+Filename: apitest_ezgo-2.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## apitest_ezgo/DbHelper.py

```diff
@@ -173,35 +173,36 @@
         conn.close()
 
     # 查询所有， 应该是最常用的了
     def select_all(self, sql, param=None):
         cursor, conn, count = self.execute(sql, param)
         try:
             res = cursor.fetchall()
-            if self.cursor_factory:
-                return [dict(i) for i in res]
-            return res
+            print(res)
+            if self.cursor_factory and res:
+                res = [dict(i) for i in res]
+            return [] if res == 0 else res
         except Exception as e:
             print(e)
             self.close(cursor, conn)
-            return count
+            return [] if self.cursor_factory else count
 
     # 查询单条
     def select_one(self, sql, param=None):
         cursor, conn, count = self.execute(sql, param)
         try:
             res = cursor.fetchone()
             self.close(cursor, conn)
-            if self.cursor_factory:
+            if self.cursor_factory and res:
                 return [dict(i) for i in res]
             return res
         except Exception as e:
             print("error_msg:", e.args)
             self.close(cursor, conn)
-            return count
+            return [] if self.cursor_factory else count
 
     # 增加
     def insert_one(self, sql, param):
         cursor, conn, count = self.execute(sql, param)
         try:
             # _id = cursor.lastrowid()  # 获取当前插入数据的主键id，该id应该为自动生成为好
             conn.commit()
```

## apitest_ezgo/__about__.py

```diff
@@ -1,8 +1,8 @@
 __title__ = 'apitest_ezgo'
 __description__ = 'easy http interface test frame'
 __url__ = ''
-__version__ = '2.0.0'
+__version__ = '2.0.1'
 __author__ = 'Gawen'
 __author_email__ = '502286126@qq.com'
 __license__ = 'Apache-2.0'
 __copyright__ = 'Copyright 2022 Gawen'
```

## Comparing `apitest_ezgo-2.0.0.dist-info/RECORD` & `apitest_ezgo-2.0.1.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 apitest_ezgo/Compare.py,sha256=cXD4UFvHFTKnj_eMo9qD-AgsShPMorVQsw4mwhSDtuU,5287
-apitest_ezgo/DbHelper.py,sha256=taQBNEUMp5mvTkE41jdt8-S3J9Q2GFwys082PGgbBUw,9890
+apitest_ezgo/DbHelper.py,sha256=vSyy4clGU2hG1JtNiyE85M9iUY9F7jS81rBxppJ29nA,10011
 apitest_ezgo/FastRequest.py,sha256=dJURPhlq_7npDkEY2VrRy9s04aQ51qV5hIGZL-6-qYA,4035
-apitest_ezgo/__about__.py,sha256=PKAVRhWXXARKuOLtOLRjvcskQwsnURLZbn9ztyjncOM,237
+apitest_ezgo/__about__.py,sha256=F3aPnxqfgI_fw1DG8tK8Tn5htsBskh8tt4kZXJMYstM,237
 apitest_ezgo/__init__.py,sha256=uM6HTTSwSziyZus-ubqZ-VKNG3KKd4kBHOlj7lR2OhQ,53
 apitest_ezgo/compat.py,sha256=U6y6S0jiigCV76iOZZoU26EYuxaIhnvT1nZr3v-nSCA,901
 apitest_ezgo/Har2Template/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 apitest_ezgo/Har2Template/cli.py,sha256=zXDmePVyKb7mRE__8bZQRI74Fjw8VKMVWYHHgBU2uGo,1844
 apitest_ezgo/Har2Template/core.py,sha256=ib7X-miBSHbxFAhDq24bgXlJA4jK2y3YdS0nukk4OSg,6466
 apitest_ezgo/Har2Template/utils.py,sha256=6bdbmru4nCCXK4J9xYMh-00IcZFZj6zw1wFQjbMH5VM,3506
-apitest_ezgo-2.0.0.dist-info/METADATA,sha256=7LcxRPkANzzzh2A6mGOZ1UzEOaTojUc6Dlp9ECimDQI,366
-apitest_ezgo-2.0.0.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
-apitest_ezgo-2.0.0.dist-info/entry_points.txt,sha256=aiep-Pjj130COhWjsCumlAgLfs_UrCKNLiW0rCprSHM,69
-apitest_ezgo-2.0.0.dist-info/top_level.txt,sha256=XZrZdozvAJVSlCHruFoGsK7hTau52-om-M9nnxTqOXE,13
-apitest_ezgo-2.0.0.dist-info/RECORD,,
+apitest_ezgo-2.0.1.dist-info/METADATA,sha256=wL4P2DgIDuVxc_MESjX6b9UY0K0tBy1dv9Tw3PbRDiY,501
+apitest_ezgo-2.0.1.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
+apitest_ezgo-2.0.1.dist-info/entry_points.txt,sha256=aiep-Pjj130COhWjsCumlAgLfs_UrCKNLiW0rCprSHM,69
+apitest_ezgo-2.0.1.dist-info/top_level.txt,sha256=XZrZdozvAJVSlCHruFoGsK7hTau52-om-M9nnxTqOXE,13
+apitest_ezgo-2.0.1.dist-info/RECORD,,
```

