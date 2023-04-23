# Comparing `tmp/yashpy-0.5.tar.gz` & `tmp/yashpy-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yashpy-0.5.tar", last modified: Sun Apr 23 07:29:33 2023, max compression
+gzip compressed data, was "yashpy-0.6.tar", last modified: Sun Apr 23 07:53:28 2023, max compression
```

## Comparing `yashpy-0.5.tar` & `yashpy-0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 07:29:33.837032 yashpy-0.5/
--rw-rw-rw-   0        0        0      175 2023-04-23 07:29:33.810100 yashpy-0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1091 2023-04-22 07:53:52.000000 yashpy-0.5/licence.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 07:29:33.837032 yashpy-0.5/setup.cfg
--rw-rw-rw-   0        0        0      245 2023-04-23 07:28:46.000000 yashpy-0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-23 07:29:33.737572 yashpy-0.5/yashpy/
--rw-rw-rw-   0        0        0     1784 2023-04-23 07:27:13.000000 yashpy-0.5/yashpy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 07:29:33.805976 yashpy-0.5/yashpy.egg-info/
--rw-rw-rw-   0        0        0      175 2023-04-23 07:29:33.000000 yashpy-0.5/yashpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      159 2023-04-23 07:29:33.000000 yashpy-0.5/yashpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 07:29:33.000000 yashpy-0.5/yashpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-23 07:29:33.000000 yashpy-0.5/yashpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 07:53:28.226511 yashpy-0.6/
+-rw-rw-rw-   0        0        0      175 2023-04-23 07:53:28.222284 yashpy-0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1091 2023-04-22 07:53:52.000000 yashpy-0.6/licence.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 07:53:28.227163 yashpy-0.6/setup.cfg
+-rw-rw-rw-   0        0        0      245 2023-04-23 07:53:14.000000 yashpy-0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 07:53:28.163724 yashpy-0.6/yashpy/
+-rw-rw-rw-   0        0        0     2157 2023-04-23 07:53:17.000000 yashpy-0.6/yashpy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 07:53:28.217404 yashpy-0.6/yashpy.egg-info/
+-rw-rw-rw-   0        0        0      175 2023-04-23 07:53:27.000000 yashpy-0.6/yashpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      159 2023-04-23 07:53:27.000000 yashpy-0.6/yashpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 07:53:27.000000 yashpy-0.6/yashpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-23 07:53:27.000000 yashpy-0.6/yashpy.egg-info/top_level.txt
```

### Comparing `yashpy-0.5/licence.txt` & `yashpy-0.6/licence.txt`

 * *Files identical despite different names*

### Comparing `yashpy-0.5/yashpy/__init__.py` & `yashpy-0.6/yashpy/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -44,14 +44,16 @@
 def factorial(n):
     fact = 1
 
     for i in range(1,n+1):
      fact = fact * i
     print (fact)
     
+
+    
     
 def is_negative(num):
     if num > 0:
        print("it is a Positive number")
     elif num == 0:
        print(" it is a Zero")
     else:
@@ -98,8 +100,19 @@
 
 
 def radian(degrees):
     pi=22/7
     return degrees * pi / 180
 
 radians = radian(180)
-print(radian)
+print(radian)
+
+#ecludian distance
+#point1=(1,22)
+#point2=(12,2)
+def distance(point1, point2):
+    differences = [point1[x] - point2[x] for x in range(len(point1))]
+    differences_squared = [difference ** 2 for difference in differences]
+    sum_of_squares = sum(differences_squared)
+    return sum_of_squares ** 0.5
+
+print(naive_euclidian_distance(point_1, point_2))
```

