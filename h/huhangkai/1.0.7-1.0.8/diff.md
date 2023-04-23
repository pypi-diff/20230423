# Comparing `tmp/huhangkai-1.0.7.tar.gz` & `tmp/huhangkai-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huhangkai-1.0.7.tar", last modified: Tue Apr 11 07:16:16 2023, max compression
+gzip compressed data, was "huhangkai-1.0.8.tar", last modified: Sun Apr 23 06:25:22 2023, max compression
```

## Comparing `huhangkai-1.0.7.tar` & `huhangkai-1.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 07:16:16.486534 huhangkai-1.0.7/
--rw-rw-rw-   0        0        0      228 2023-04-11 07:16:16.485537 huhangkai-1.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-11 07:16:16.468580 huhangkai-1.0.7/commen/
--rw-rw-rw-   0        0        0      929 2023-01-30 02:59:52.000000 huhangkai-1.0.7/commen/__init__.py
--rw-rw-rw-   0        0        0    32340 2023-02-22 03:30:12.000000 huhangkai-1.0.7/commen/init_project.py
--rw-rw-rw-   0        0        0     4508 2022-11-09 07:51:47.000000 huhangkai-1.0.7/commen/unit_dict.py
--rw-rw-rw-   0        0        0    18531 2023-04-07 08:26:33.000000 huhangkai-1.0.7/commen/unit_fun.py
--rw-rw-rw-   0        0        0     1242 2022-11-09 07:51:47.000000 huhangkai-1.0.7/commen/unit_logger.py
--rw-rw-rw-   0        0        0     6122 2023-02-15 10:10:32.000000 huhangkai-1.0.7/commen/unit_request.py
-drwxrwxrwx   0        0        0        0 2023-04-11 07:16:16.482543 huhangkai-1.0.7/huhangkai.egg-info/
--rw-rw-rw-   0        0        0      228 2023-04-11 07:16:16.000000 huhangkai-1.0.7/huhangkai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      298 2023-04-11 07:16:16.000000 huhangkai-1.0.7/huhangkai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 07:16:16.000000 huhangkai-1.0.7/huhangkai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-04-11 07:16:16.000000 huhangkai-1.0.7/huhangkai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-11 07:16:16.000000 huhangkai-1.0.7/huhangkai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 07:16:16.486534 huhangkai-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0      495 2023-04-11 07:15:57.000000 huhangkai-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:25:22.908200 huhangkai-1.0.8/
+-rw-rw-rw-   0        0        0      228 2023-04-23 06:25:22.907202 huhangkai-1.0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-23 06:25:22.896232 huhangkai-1.0.8/commen/
+-rw-rw-rw-   0        0        0      929 2023-01-30 02:59:52.000000 huhangkai-1.0.8/commen/__init__.py
+-rw-rw-rw-   0        0        0    32340 2023-02-22 03:30:12.000000 huhangkai-1.0.8/commen/init_project.py
+-rw-rw-rw-   0        0        0     4508 2022-11-09 07:51:47.000000 huhangkai-1.0.8/commen/unit_dict.py
+-rw-rw-rw-   0        0        0    19449 2023-04-23 06:24:44.000000 huhangkai-1.0.8/commen/unit_fun.py
+-rw-rw-rw-   0        0        0     1242 2022-11-09 07:51:47.000000 huhangkai-1.0.8/commen/unit_logger.py
+-rw-rw-rw-   0        0        0     6122 2023-02-15 10:10:32.000000 huhangkai-1.0.8/commen/unit_request.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:25:22.905210 huhangkai-1.0.8/huhangkai.egg-info/
+-rw-rw-rw-   0        0        0      228 2023-04-23 06:25:22.000000 huhangkai-1.0.8/huhangkai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      298 2023-04-23 06:25:22.000000 huhangkai-1.0.8/huhangkai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 06:25:22.000000 huhangkai-1.0.8/huhangkai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-04-23 06:25:22.000000 huhangkai-1.0.8/huhangkai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-23 06:25:22.000000 huhangkai-1.0.8/huhangkai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 06:25:22.908200 huhangkai-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      495 2023-04-23 06:24:59.000000 huhangkai-1.0.8/setup.py
```

### Comparing `huhangkai-1.0.7/commen/__init__.py` & `huhangkai-1.0.8/commen/__init__.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.0.7/commen/init_project.py` & `huhangkai-1.0.8/commen/init_project.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.0.7/commen/unit_dict.py` & `huhangkai-1.0.8/commen/unit_dict.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.0.7/commen/unit_fun.py` & `huhangkai-1.0.8/commen/unit_fun.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,14 +33,38 @@
         else:
             time.sleep(1)
             
 
     def _faker_name(self):
         return self._faker.name() + str(self._faker.numerify())
 
+    @staticmethod
+    def random_vin():
+        # 内容的权值
+        content_map = {
+            'A': 1, 'B': 2, 'C': 3, 'D': 4, 'E': 5,
+            'F': 6, 'G': 7, 'H': 8, 'I': 0, 'J': 1, 'K': 2, 'L': 3,
+            'M': 4, 'N': 5, 'O': 0, 'P': 7, 'Q': 8, 'R': 9, 'S': 2, 'T': 3,
+            'U': 4, 'V': 5, 'W': 6, 'X': 7, 'Y': 8, 'Z': 9, "0": 0, "1": 1,
+            "2": 2, "3": 3, "4": 4, "5": 5, "6": 6, "7": 7, "8": 8, "9": 9
+        }
+        # 位置的全值
+        location_map = [8, 7, 6, 5, 4, 3, 2, 10, 0, 9, 8, 7, 6, 5, 4, 3, 2]
+        vin = ''.join(random.sample('0123456789ABCDEFGHJKLMPRSTUVWXYZ', 17))
+        num = 0
+        for i in range(len(vin)):
+            num = num + content_map[vin[i]] * location_map[i]
+        vin9 = num % 11
+        if vin9 == 10:
+            vin9 = "X"
+        list1 = list(vin)
+        list1[8] = str(vin9)
+        vin = ''.join(list1)
+        return vin
+
     # # mock方法，国家locale_list随机，也可根据数字获取第几个国家，超出时随机
     # def faker_random_country(self, locale=None):
     #     country = None
     #     if locale:
     #         try:
     #             if self.locale_list.get(locale):
     #                 country = locale
@@ -423,16 +447,17 @@
                               sheet_name="sheet1",
                               index=False,
                               engine="openpyxl"
                               )
 
 
 if __name__ == '__main__':
-    f = FunBase().faker()
-    # print(f.run_mysql("", ))
+    print(FunBase().random_vin())
+    # f = FunBase().faker()
+
     # print(f.name())  # 随机姓名
     # print(f.ipv4())  # 随机IP4地址
     # print(f.uri())  # 随机URI地址
     # print(f.url())  # 随机URL地址
     # print(f.user_name())  # 随机⽤户名
     # print(f.paragraph())  # 随机⽣成⼀个段落
     # print(f.text())  # 随机⽣成⼀篇⽂章
```

### Comparing `huhangkai-1.0.7/commen/unit_logger.py` & `huhangkai-1.0.8/commen/unit_logger.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.0.7/commen/unit_request.py` & `huhangkai-1.0.8/commen/unit_request.py`

 * *Files identical despite different names*

