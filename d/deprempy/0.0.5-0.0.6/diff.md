# Comparing `tmp/deprempy-0.0.5.tar.gz` & `tmp/deprempy-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deprempy-0.0.5.tar", last modified: Wed Apr 19 14:40:53 2023, max compression
+gzip compressed data, was "deprempy-0.0.6.tar", last modified: Sun Apr 23 17:48:51 2023, max compression
```

## Comparing `deprempy-0.0.5.tar` & `deprempy-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 14:40:53.859206 deprempy-0.0.5/
--rw-rw-rw-   0        0        0    35149 2022-12-02 14:26:43.000000 deprempy-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     3169 2023-04-19 14:40:53.858202 deprempy-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2534 2023-04-19 13:15:00.000000 deprempy-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 14:40:53.844455 deprempy-0.0.5/deprempy/
--rw-rw-rw-   0        0        0     3110 2023-04-19 12:36:52.000000 deprempy-0.0.5/deprempy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 14:40:53.855902 deprempy-0.0.5/deprempy.egg-info/
--rw-rw-rw-   0        0        0     3169 2023-04-19 14:40:53.000000 deprempy-0.0.5/deprempy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      175 2023-04-19 14:40:53.000000 deprempy-0.0.5/deprempy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 14:40:53.000000 deprempy-0.0.5/deprempy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-19 14:40:53.000000 deprempy-0.0.5/deprempy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 14:40:53.860522 deprempy-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      805 2023-04-19 14:40:01.000000 deprempy-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 17:48:51.606341 deprempy-0.0.6/
+-rw-rw-rw-   0        0        0    35149 2022-12-02 14:26:43.000000 deprempy-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     3190 2023-04-23 17:48:51.605333 deprempy-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2555 2023-04-23 17:47:24.000000 deprempy-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 17:48:51.591774 deprempy-0.0.6/deprempy/
+-rw-rw-rw-   0        0        0     4596 2023-04-23 17:43:47.000000 deprempy-0.0.6/deprempy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 17:48:51.603318 deprempy-0.0.6/deprempy.egg-info/
+-rw-rw-rw-   0        0        0     3190 2023-04-23 17:48:51.000000 deprempy-0.0.6/deprempy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      175 2023-04-23 17:48:51.000000 deprempy-0.0.6/deprempy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 17:48:51.000000 deprempy-0.0.6/deprempy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-23 17:48:51.000000 deprempy-0.0.6/deprempy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 17:48:51.607344 deprempy-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      805 2023-04-23 17:48:44.000000 deprempy-0.0.6/setup.py
```

### Comparing `deprempy-0.0.5/LICENSE` & `deprempy-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `deprempy-0.0.5/PKG-INFO` & `deprempy-0.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deprempy
-Version: 0.0.5
+Version: 0.0.6
 Summary: Kandilli Rasathanesi aracılığı ile elde edilen deprem sinyallerini kullanarak depremleri gösteren bir Python kütüphanesidir.
 Home-page: https://gihtub.com/Meinos10/deprempy
 Author: Emre
 Author-email: E.tmen2023@gmail.com
 License: MIT
 Keywords: deprempy,deprempython,deprem,deprem-python,deprem-py
 Classifier: Programming Language :: Python :: 3
@@ -68,16 +68,16 @@
     {
         'tarih': '2023.04.19', 
         'saat': '14:28:29', 
         'enlem': '37.4822', 
         'boylam': '35.2963', 
         'derinlik': '7.7', 
         'buyukluk': '2.0', 
-        'yer': 'MADENLI-ALADAG', 
-        'tip': '(ADANA)'
+        'yer': 'MADENLI-ALADAG (ADANA)', 
+        'tip': 'Ilksel'
     }
 ]
 """
 
 deprem.son_24saat(2)
 
 """
@@ -95,16 +95,16 @@
     {
         'tarih': '2023.04.19', 
         'saat': '14:28:29', 
         'enlem': '37.4822', 
         'boylam': '35.2963', 
         'derinlik': '7.7', 
         'buyukluk': '2.0', 
-        'yer': 'MADENLI-ALADAG', 
-        'tip': '(ADANA)'
+        'yer': 'MADENLI-ALADAG (ADANA)', 
+        'tip': 'Ilksel'
     }
 ]
 """
 
 deprem.tum_depremler(2)
 
 """
@@ -122,16 +122,16 @@
     {
         'tarih': '2023.04.19', 
         'saat': '14:28:29', 
         'enlem': '37.4822', 
         'boylam': '35.2963', 
         'derinlik': '7.7', 
         'buyukluk': '2.0', 
-        'yer': 'MADENLI-ALADAG', 
-        'tip': '(ADANA)'
+        'yer': 'MADENLI-ALADAG (ADANA)', 
+        'tip': 'Ilksel'
     }
 ]
 """
 ```
 
 ## License
```

### Comparing `deprempy-0.0.5/README.md` & `deprempy-0.0.6/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -51,16 +51,16 @@
     {
         'tarih': '2023.04.19', 
         'saat': '14:28:29', 
         'enlem': '37.4822', 
         'boylam': '35.2963', 
         'derinlik': '7.7', 
         'buyukluk': '2.0', 
-        'yer': 'MADENLI-ALADAG', 
-        'tip': '(ADANA)'
+        'yer': 'MADENLI-ALADAG (ADANA)', 
+        'tip': 'Ilksel'
     }
 ]
 """
 
 deprem.son_24saat(2)
 
 """
@@ -78,16 +78,16 @@
     {
         'tarih': '2023.04.19', 
         'saat': '14:28:29', 
         'enlem': '37.4822', 
         'boylam': '35.2963', 
         'derinlik': '7.7', 
         'buyukluk': '2.0', 
-        'yer': 'MADENLI-ALADAG', 
-        'tip': '(ADANA)'
+        'yer': 'MADENLI-ALADAG (ADANA)', 
+        'tip': 'Ilksel'
     }
 ]
 """
 
 deprem.tum_depremler(2)
 
 """
@@ -105,16 +105,16 @@
     {
         'tarih': '2023.04.19', 
         'saat': '14:28:29', 
         'enlem': '37.4822', 
         'boylam': '35.2963', 
         'derinlik': '7.7', 
         'buyukluk': '2.0', 
-        'yer': 'MADENLI-ALADAG', 
-        'tip': '(ADANA)'
+        'yer': 'MADENLI-ALADAG (ADANA)', 
+        'tip': 'Ilksel'
     }
 ]
 """
 ```
 
 ## License
```

### Comparing `deprempy-0.0.5/deprempy/__init__.py` & `deprempy-0.0.6/deprempy/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,69 +15,103 @@
     def __init__(self) -> None:
         self.r = g(url).text
         self.soup = bs(self.r, "html.parser")
         self.allstrs = self.soup.find("pre").text
         self.strs = self.allstrs.split("---------- --------  --------  -------   ----------    ------------    --------------                                  --------------")[1].strip().split("\n")
 
     def son_deprem(self):
+        yer = ""
+        tip = ""
+        if self.strs[0].split()[9].replace("Ý", "I") == "Ilkesel":
+            yer = self.strs[0].split()[8]
+            tip = self.strs[0].split()[9].replace("Ý", "I")
+        else:
+            yer = self.strs[0].split()[8] + " " + self.strs[0].split()[9]
+            tip = self.strs[0].split()[10].replace("Ý", "I")
+        
         sd = {
             "tarih": self.strs[0].split()[0],
             "saat": self.strs[0].split()[1],
             "enlem": self.strs[0].split()[2],
             "boylam": self.strs[0].split()[3],
             "derinlik": self.strs[0].split()[4],
             "buyukluk": self.strs[0].split()[6],
-            "yer": self.strs[0].split()[8],
-            "tip": self.strs[0].split()[9].replace("Ý", "I")
+            "yer": yer,
+            "tip": tip
         }
         return sd
     
     def tum_depremler(self, limit: int=100):
         td = []
         for i in self.strs:
             if not self.strs.index(i)+1 > limit:
+                yer = ""
+                tip = ""
+                if self.strs[0].split()[9].replace("Ý", "I") == "Ilkesel":
+                    yer = self.strs[0].split()[8]
+                    tip = self.strs[0].split()[9].replace("Ý", "I")
+                else:
+                    yer = self.strs[0].split()[8] + " " + self.strs[0].split()[9]
+                    tip = self.strs[0].split()[10].replace("Ý", "I")
                 td.append({
                     "tarih": i.split()[0],
                     "saat": i.split()[1],
                     "enlem": i.split()[2],
                     "boylam": i.split()[3],
                     "derinlik": i.split()[4],
                     "buyukluk": i.split()[6],
-                    "yer": i.split()[8],
-                    "tip": i.split()[9].replace("Ý", "I")
+                    "yer": yer,
+                    "tip": tip
                 })
         return td
     
     def son_24saat(self, limit: int=100):
         s24 = []
         for i in self.strs:
             if not self.strs.index(i)+1 > limit:
+                yer = ""
+                tip = ""
+                if self.strs[0].split()[9].replace("Ý", "I") == "Ilkesel":
+                    yer = self.strs[0].split()[8]
+                    tip = self.strs[0].split()[9].replace("Ý", "I")
+                else:
+                    yer = self.strs[0].split()[8] + " " + self.strs[0].split()[9]
+                    tip = self.strs[0].split()[10].replace("Ý", "I")
+
                 if i.split()[0] == self.son_deprem()["tarih"]:
                     s24.append({
                         "tarih": i.split()[0],
                         "saat": i.split()[1],
                         "enlem": i.split()[2],
                         "boylam": i.split()[3],
                         "derinlik": i.split()[4],
                         "buyukluk": i.split()[6],
-                        "yer": i.split()[8],
-                        "tip": i.split()[9].replace("Ý", "I")
+                        "yer": yer,
+                        "tip": tip
                     })
         return s24
     
     def son_1saat(self, limit: int=100):
         s1 = []
         for i in self.strs:
             if not self.strs.index(i)+1 > limit:
+                yer = ""
+                tip = ""
+                if self.strs[0].split()[9].replace("Ý", "I") == "Ilkesel":
+                    yer = self.strs[0].split()[8]
+                    tip = self.strs[0].split()[9].replace("Ý", "I")
+                else:
+                    yer = self.strs[0].split()[8] + " " + self.strs[0].split()[9]
+                    tip = self.strs[0].split()[10].replace("Ý", "I")
                 if i.split()[0] == self.son_deprem()["tarih"] and i.split()[1].split(":")[0] == self.son_deprem()["saat"].split(":")[0]:
                     s1.append({
                         "tarih": i.split()[0],
                         "saat": i.split()[1],
                         "enlem": i.split()[2],
                         "boylam": i.split()[3],
                         "derinlik": i.split()[4],
                         "buyukluk": i.split()[6],
-                        "yer": i.split()[8],
-                        "tip": i.split()[9].replace("Ý", "I")
+                        "yer": yer,
+                        "tip": tip
                     })
         return s1
```

### Comparing `deprempy-0.0.5/deprempy.egg-info/PKG-INFO` & `deprempy-0.0.6/deprempy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deprempy
-Version: 0.0.5
+Version: 0.0.6
 Summary: Kandilli Rasathanesi aracılığı ile elde edilen deprem sinyallerini kullanarak depremleri gösteren bir Python kütüphanesidir.
 Home-page: https://gihtub.com/Meinos10/deprempy
 Author: Emre
 Author-email: E.tmen2023@gmail.com
 License: MIT
 Keywords: deprempy,deprempython,deprem,deprem-python,deprem-py
 Classifier: Programming Language :: Python :: 3
@@ -68,16 +68,16 @@
     {
         'tarih': '2023.04.19', 
         'saat': '14:28:29', 
         'enlem': '37.4822', 
         'boylam': '35.2963', 
         'derinlik': '7.7', 
         'buyukluk': '2.0', 
-        'yer': 'MADENLI-ALADAG', 
-        'tip': '(ADANA)'
+        'yer': 'MADENLI-ALADAG (ADANA)', 
+        'tip': 'Ilksel'
     }
 ]
 """
 
 deprem.son_24saat(2)
 
 """
@@ -95,16 +95,16 @@
     {
         'tarih': '2023.04.19', 
         'saat': '14:28:29', 
         'enlem': '37.4822', 
         'boylam': '35.2963', 
         'derinlik': '7.7', 
         'buyukluk': '2.0', 
-        'yer': 'MADENLI-ALADAG', 
-        'tip': '(ADANA)'
+        'yer': 'MADENLI-ALADAG (ADANA)', 
+        'tip': 'Ilksel'
     }
 ]
 """
 
 deprem.tum_depremler(2)
 
 """
@@ -122,16 +122,16 @@
     {
         'tarih': '2023.04.19', 
         'saat': '14:28:29', 
         'enlem': '37.4822', 
         'boylam': '35.2963', 
         'derinlik': '7.7', 
         'buyukluk': '2.0', 
-        'yer': 'MADENLI-ALADAG', 
-        'tip': '(ADANA)'
+        'yer': 'MADENLI-ALADAG (ADANA)', 
+        'tip': 'Ilksel'
     }
 ]
 """
 ```
 
 ## License
```

### Comparing `deprempy-0.0.5/setup.py` & `deprempy-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="deprempy",
-    version="0.0.5",
+    version="0.0.6",
     description="Kandilli Rasathanesi aracılığı ile elde edilen deprem sinyallerini kullanarak depremleri gösteren bir Python kütüphanesidir.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://gihtub.com/Meinos10/deprempy",
     author="Emre",
     author_email="E.tmen2023@gmail.com",
     license="MIT",
```

