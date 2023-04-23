# Comparing `tmp/vtda-1.5.0-py3-none-any.whl.zip` & `tmp/vtda-1.5.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 53546 bytes, number of entries: 26
--rw-rw-rw-  2.0 fat     2683 b- defN 22-Aug-19 06:59 vtda/__init__.py
+Zip file size: 53589 bytes, number of entries: 26
+-rw-rw-rw-  2.0 fat     2683 b- defN 23-Feb-11 15:15 vtda/__init__.py
 -rw-rw-rw-  2.0 fat     2020 b- defN 21-Dec-30 15:14 vtda/analysis/__init__.py
 -rw-rw-rw-  2.0 fat    29599 b- defN 22-Jul-04 09:45 vtda/analysis/base.py
 -rw-rw-rw-  2.0 fat    11168 b- defN 21-Jun-26 16:24 vtda/analysis/batch_calculate.py
 -rw-rw-rw-  2.0 fat    18504 b- defN 21-Nov-23 08:14 vtda/analysis/noise.py
 -rw-rw-rw-  2.0 fat    17769 b- defN 22-Jul-04 10:09 vtda/analysis/sperling.py
 -rw-rw-rw-  2.0 fat      876 b- defN 21-Nov-25 16:44 vtda/analysis/untitled1.py
 -rw-rw-rw-  2.0 fat    46938 b- defN 21-Dec-11 14:26 vtda/analysis/vehicle_dynamics.py
@@ -16,13 +16,13 @@
 -rw-rw-rw-  2.0 fat      313 b- defN 21-Jun-12 08:28 vtda/read_data/__init__.py
 -rw-rw-rw-  2.0 fat     9562 b- defN 22-Aug-14 11:25 vtda/read_data/read_dasp.py
 -rw-rw-rw-  2.0 fat     8813 b- defN 21-Nov-28 16:18 vtda/read_data/read_dxd.py
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Nov-14 13:16 vtda/test/__init__.py
 -rw-rw-rw-  2.0 fat     3043 b- defN 21-Jun-27 03:15 vtda/test/find_start_and_end.py
 -rw-rw-rw-  2.0 fat     2179 b- defN 21-Jun-14 14:47 vtda/test/test.py
 -rw-rw-rw-  2.0 fat      362 b- defN 21-Nov-11 12:14 vtda/util/__init__.py
--rw-rw-rw-  2.0 fat    10473 b- defN 21-Nov-23 07:11 vtda/util/util.py
--rw-rw-rw-  2.0 fat      285 b- defN 22-Aug-19 07:00 vtda-1.5.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 22-Aug-19 07:00 vtda-1.5.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 22-Aug-19 07:00 vtda-1.5.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     2073 b- defN 22-Aug-19 07:00 vtda-1.5.0.dist-info/RECORD
-26 files, 213961 bytes uncompressed, 50240 bytes compressed:  76.5%
+-rw-rw-rw-  2.0 fat    10650 b- defN 23-Feb-11 15:27 vtda/util/util.py
+-rw-rw-rw-  2.0 fat      285 b- defN 23-Apr-23 02:47 vtda-1.5.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 23-Apr-23 02:47 vtda-1.5.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 23-Apr-23 02:47 vtda-1.5.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     2073 b- defN 23-Apr-23 02:47 vtda-1.5.1.dist-info/RECORD
+26 files, 214138 bytes uncompressed, 50283 bytes compressed:  76.5%
```

## zipnote {}

```diff
@@ -60,20 +60,20 @@
 
 Filename: vtda/util/__init__.py
 Comment: 
 
 Filename: vtda/util/util.py
 Comment: 
 
-Filename: vtda-1.5.0.dist-info/METADATA
+Filename: vtda-1.5.1.dist-info/METADATA
 Comment: 
 
-Filename: vtda-1.5.0.dist-info/WHEEL
+Filename: vtda-1.5.1.dist-info/WHEEL
 Comment: 
 
-Filename: vtda-1.5.0.dist-info/top_level.txt
+Filename: vtda-1.5.1.dist-info/top_level.txt
 Comment: 
 
-Filename: vtda-1.5.0.dist-info/RECORD
+Filename: vtda-1.5.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vtda/__init__.py

```diff
@@ -1,13 +1,13 @@
 ﻿"""
 vtda
 Vibration Test Data Analysis
 """
 
-__version__ = '1.5.0'
+__version__ = '1.5.1'
 __author__ = 'zhangshenglong'
 
 '''
 read_data
 '''
 from vtda.read_data.read_dasp import (
                                                read_dasp_data_single,
```

## vtda/util/util.py

```diff
@@ -264,26 +264,31 @@
     return res
         
     
 def fix_num(num='3,5,8-10'):
     '''
     将字符格式的序号转换为list格式的序号
     '''
-    
     res_ls1=num.split(',')
     res=[]
     for i in res_ls1:
         pass
         res_ls2=i.split('-')
         if len(res_ls2)>1 and len(res_ls2)<3:
-            ls=list(range(int(res_ls2[0]),int(res_ls2[1])+1))
-            ls=[str(x) for x in ls]
-            res+=ls
+            if res_ls2[0]=='Km':
+                res+=[i]
+            else:
+                ls=list(range(int(res_ls2[0]),int(res_ls2[1])+1))
+                ls=[str(x) for x in ls]
+                res+=ls                
         elif len(res_ls2)==1:
-            ls=[str(int(res_ls2[0]))]
+            try:
+                ls=[str(int(res_ls2[0]))]
+            except:
+                ls=[res_ls2[0]]
             res+=ls
         else:
             print('输入编号格式错误，请检查。')
     return res
         
 def find_start_end(y,
                    sample_rate=4096,
```

## Comparing `vtda-1.5.0.dist-info/RECORD` & `vtda-1.5.1.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-vtda/__init__.py,sha256=2i3jJZMYrZ77hqCfyBS-trEQwem57CjG-oBYeveI9ls,2683
+vtda/__init__.py,sha256=MzCG3dCH8VRKTE079cUkL1G2QrdTJkhXGl5jNZ7XGtw,2683
 vtda/analysis/__init__.py,sha256=zRVrAQv1k1Lq-aB4Wn04JyxmfjKLNA3bWQ75ExOSj3k,2020
 vtda/analysis/base.py,sha256=XSSvKP7ZChMKLc4hN8FWR2u-7Je1X0VcFN4o-8F2aPg,29599
 vtda/analysis/batch_calculate.py,sha256=BkCpaX1w6t9s9VGQy4QUWMJZbNrTJ7P9zYmrrQWgo-c,11168
 vtda/analysis/noise.py,sha256=5wIs3ZhWEHMEVTxqE7T3qgwHN2EvGsxfQCQajt9egXw,18504
 vtda/analysis/sperling.py,sha256=JwtBFQGyQ0OQPiJr34x7NYagfONVfFSA2JBsEj4rQ5M,17769
 vtda/analysis/untitled1.py,sha256=5-0Toujm65I0Eneie-8n-T2jOtbdWRNH18G7iI8ZGYI,876
 vtda/analysis/vehicle_dynamics.py,sha256=Xb8zl250jsbXi5t5XIGyRygogxBiEuum2TtokI6Nwjo,46938
@@ -15,12 +15,12 @@
 vtda/read_data/__init__.py,sha256=kWepW0h7WzFhQN90NpHY5kHPFM5QH8411cx284Outho,313
 vtda/read_data/read_dasp.py,sha256=nIpZ8UtzzxkvRE-rpl6dntNROLex8aZDKOyQPipDFcM,9562
 vtda/read_data/read_dxd.py,sha256=m3jX0YbbIElU3OSBq2ObXnl6cULHXbLp378knC8a-4w,8813
 vtda/test/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 vtda/test/find_start_and_end.py,sha256=4_KG4ny2rINEo-j9GdWVu1OWtdGCzZNXAZsnv1jCpFg,3043
 vtda/test/test.py,sha256=OsyeOy8n6qaILK81wlGsut4k45EXHlNfB48gSly8JAs,2179
 vtda/util/__init__.py,sha256=giJ_UE71YWyBIc9aKW934Otilcdsy_FayKvMOaYpuDg,362
-vtda/util/util.py,sha256=3GMEANff-AFR22-c1OtlAWN7SQ2dMrGiU0qQVhljol0,10473
-vtda-1.5.0.dist-info/METADATA,sha256=XS49WY_X50eAJbPY9XcOGVnrFwkrNnSs09hH8QfBv5c,285
-vtda-1.5.0.dist-info/WHEEL,sha256=D1Wh14kWDxPnrM-5t_6UCB-UuQNrEODtRa3vF4OsvQY,97
-vtda-1.5.0.dist-info/top_level.txt,sha256=DnhjMA74wO4kU53vr91eo3C0r-6Od0RMXgWT6JreCq4,5
-vtda-1.5.0.dist-info/RECORD,,
+vtda/util/util.py,sha256=PZJGYSFOIiSQnCB75z0LkU_AbYp7n-snzuaIUuUwdxI,10650
+vtda-1.5.1.dist-info/METADATA,sha256=A48QYZtAFsc6ejubadrYH_Bulfqk-c4stG01nV59tNo,285
+vtda-1.5.1.dist-info/WHEEL,sha256=D1Wh14kWDxPnrM-5t_6UCB-UuQNrEODtRa3vF4OsvQY,97
+vtda-1.5.1.dist-info/top_level.txt,sha256=DnhjMA74wO4kU53vr91eo3C0r-6Od0RMXgWT6JreCq4,5
+vtda-1.5.1.dist-info/RECORD,,
```

