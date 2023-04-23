# Comparing `tmp/huhangkai-1.0.8.tar.gz` & `tmp/huhangkai-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huhangkai-1.0.8.tar", last modified: Sun Apr 23 06:25:22 2023, max compression
+gzip compressed data, was "huhangkai-1.0.9.tar", last modified: Sun Apr 23 09:22:57 2023, max compression
```

## Comparing `huhangkai-1.0.8.tar` & `huhangkai-1.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 06:25:22.908200 huhangkai-1.0.8/
--rw-rw-rw-   0        0        0      228 2023-04-23 06:25:22.907202 huhangkai-1.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-23 06:25:22.896232 huhangkai-1.0.8/commen/
--rw-rw-rw-   0        0        0      929 2023-01-30 02:59:52.000000 huhangkai-1.0.8/commen/__init__.py
--rw-rw-rw-   0        0        0    32340 2023-02-22 03:30:12.000000 huhangkai-1.0.8/commen/init_project.py
--rw-rw-rw-   0        0        0     4508 2022-11-09 07:51:47.000000 huhangkai-1.0.8/commen/unit_dict.py
--rw-rw-rw-   0        0        0    19449 2023-04-23 06:24:44.000000 huhangkai-1.0.8/commen/unit_fun.py
--rw-rw-rw-   0        0        0     1242 2022-11-09 07:51:47.000000 huhangkai-1.0.8/commen/unit_logger.py
--rw-rw-rw-   0        0        0     6122 2023-02-15 10:10:32.000000 huhangkai-1.0.8/commen/unit_request.py
-drwxrwxrwx   0        0        0        0 2023-04-23 06:25:22.905210 huhangkai-1.0.8/huhangkai.egg-info/
--rw-rw-rw-   0        0        0      228 2023-04-23 06:25:22.000000 huhangkai-1.0.8/huhangkai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      298 2023-04-23 06:25:22.000000 huhangkai-1.0.8/huhangkai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 06:25:22.000000 huhangkai-1.0.8/huhangkai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-04-23 06:25:22.000000 huhangkai-1.0.8/huhangkai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-23 06:25:22.000000 huhangkai-1.0.8/huhangkai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 06:25:22.908200 huhangkai-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      495 2023-04-23 06:24:59.000000 huhangkai-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 09:22:57.717679 huhangkai-1.0.9/
+-rw-rw-rw-   0        0        0      228 2023-04-23 09:22:57.716681 huhangkai-1.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-23 09:22:57.701691 huhangkai-1.0.9/commen/
+-rw-rw-rw-   0        0        0      929 2023-01-30 02:59:52.000000 huhangkai-1.0.9/commen/__init__.py
+-rw-rw-rw-   0        0        0    32340 2023-02-22 03:30:12.000000 huhangkai-1.0.9/commen/init_project.py
+-rw-rw-rw-   0        0        0     4508 2022-11-09 07:51:47.000000 huhangkai-1.0.9/commen/unit_dict.py
+-rw-rw-rw-   0        0        0    20151 2023-04-23 09:21:46.000000 huhangkai-1.0.9/commen/unit_fun.py
+-rw-rw-rw-   0        0        0     1242 2022-11-09 07:51:47.000000 huhangkai-1.0.9/commen/unit_logger.py
+-rw-rw-rw-   0        0        0     6122 2023-02-15 10:10:32.000000 huhangkai-1.0.9/commen/unit_request.py
+drwxrwxrwx   0        0        0        0 2023-04-23 09:22:57.714684 huhangkai-1.0.9/huhangkai.egg-info/
+-rw-rw-rw-   0        0        0      228 2023-04-23 09:22:57.000000 huhangkai-1.0.9/huhangkai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      298 2023-04-23 09:22:57.000000 huhangkai-1.0.9/huhangkai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 09:22:57.000000 huhangkai-1.0.9/huhangkai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-04-23 09:22:57.000000 huhangkai-1.0.9/huhangkai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-23 09:22:57.000000 huhangkai-1.0.9/huhangkai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 09:22:57.717679 huhangkai-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      495 2023-04-23 09:22:51.000000 huhangkai-1.0.9/setup.py
```

### Comparing `huhangkai-1.0.8/commen/__init__.py` & `huhangkai-1.0.9/commen/__init__.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.0.8/commen/init_project.py` & `huhangkai-1.0.9/commen/init_project.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.0.8/commen/unit_dict.py` & `huhangkai-1.0.9/commen/unit_dict.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.0.8/commen/unit_fun.py` & `huhangkai-1.0.9/commen/unit_fun.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,14 +57,29 @@
         if vin9 == 10:
             vin9 = "X"
         list1 = list(vin)
         list1[8] = str(vin9)
         vin = ''.join(list1)
         return vin
 
+    @staticmethod
+    def random_carnum():
+        char0 = '京津沪渝冀豫云辽黑湘皖鲁新苏浙赣鄂桂甘晋蒙陕吉闽赣粤青藏川宁琼'
+        char1 = 'ABCDEFGHJKLMNPQRSTUVWXYZ'  # 车牌号中没有I和O，可自行百度
+        char2 = '1234567890ABCDEFGHJKLMNPQRSTUVWXYZ'
+        char3 = '1234567890'
+        while True:
+            code = random.choice(char0)
+            code += random.choice(char1)
+            code += "".join(random.choices(char2, k=4))
+            code += random.choice(char3)
+            test = re.match('^.\w.[A-Z]\d{4}$|^.\w.\d[A-Z]\d{3}$|^.\w.\d{2}[A-Z]\d{2}$|^.\w.\d{3}[A-Z]\d$|^.\w.\d{5}$', code)
+            if test:
+                return code
+
     # # mock方法，国家locale_list随机，也可根据数字获取第几个国家，超出时随机
     # def faker_random_country(self, locale=None):
     #     country = None
     #     if locale:
     #         try:
     #             if self.locale_list.get(locale):
     #                 country = locale
@@ -447,15 +462,15 @@
                               sheet_name="sheet1",
                               index=False,
                               engine="openpyxl"
                               )
 
 
 if __name__ == '__main__':
-    print(FunBase().random_vin())
+    print(FunBase().random_carnum())
     # f = FunBase().faker()
 
     # print(f.name())  # 随机姓名
     # print(f.ipv4())  # 随机IP4地址
     # print(f.uri())  # 随机URI地址
     # print(f.url())  # 随机URL地址
     # print(f.user_name())  # 随机⽤户名
```

### Comparing `huhangkai-1.0.8/commen/unit_logger.py` & `huhangkai-1.0.9/commen/unit_logger.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.0.8/commen/unit_request.py` & `huhangkai-1.0.9/commen/unit_request.py`

 * *Files identical despite different names*

