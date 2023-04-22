# Comparing `tmp/Conanmail-1.0.7-py3-none-any.whl.zip` & `tmp/Conanmail-1.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,14 @@
-Zip file size: 4755 bytes, number of entries: 9
+Zip file size: 14384 bytes, number of entries: 12
 -rw-rw-rw-  2.0 fat     1502 b- defN 23-Apr-21 19:13 conan/IMAP.json
 -rw-rw-rw-  2.0 fat      852 b- defN 23-Apr-22 21:44 conan/config.py
 -rw-rw-rw-  2.0 fat     1027 b- defN 23-Apr-22 20:29 conan/main.py
--rw-rw-rw-  2.0 fat     5469 b- defN 23-Apr-22 21:57 conan/utils.py
--rw-rw-rw-  2.0 fat      308 b- defN 23-Apr-22 21:57 Conanmail-1.0.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-22 21:57 Conanmail-1.0.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       42 b- defN 23-Apr-22 21:57 Conanmail-1.0.7.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        6 b- defN 23-Apr-22 21:57 Conanmail-1.0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      685 b- defN 23-Apr-22 21:57 Conanmail-1.0.7.dist-info/RECORD
-9 files, 9983 bytes uncompressed, 3579 bytes compressed:  64.1%
+-rw-rw-rw-  2.0 fat     5510 b- defN 23-Apr-22 22:01 conan/utils.py
+-rw-rw-rw-  2.0 fat     2903 b- defN 23-Apr-22 18:38 conan/web/index.html
+-rw-rw-rw-  2.0 fat    15313 b- defN 23-Apr-22 16:51 conan/web/render.svg
+-rw-rw-rw-  2.0 fat     3718 b- defN 23-Apr-22 19:50 conan/web/style.css
+-rw-rw-rw-  2.0 fat      308 b- defN 23-Apr-22 22:01 Conanmail-1.0.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-22 22:01 Conanmail-1.0.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       42 b- defN 23-Apr-22 22:01 Conanmail-1.0.8.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        6 b- defN 23-Apr-22 22:01 Conanmail-1.0.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      916 b- defN 23-Apr-22 22:01 Conanmail-1.0.8.dist-info/RECORD
+12 files, 32189 bytes uncompressed, 12862 bytes compressed:  60.0%
```

## zipnote {}

```diff
@@ -6,23 +6,32 @@
 
 Filename: conan/main.py
 Comment: 
 
 Filename: conan/utils.py
 Comment: 
 
-Filename: Conanmail-1.0.7.dist-info/METADATA
+Filename: conan/web/index.html
 Comment: 
 
-Filename: Conanmail-1.0.7.dist-info/WHEEL
+Filename: conan/web/render.svg
 Comment: 
 
-Filename: Conanmail-1.0.7.dist-info/entry_points.txt
+Filename: conan/web/style.css
 Comment: 
 
-Filename: Conanmail-1.0.7.dist-info/top_level.txt
+Filename: Conanmail-1.0.8.dist-info/METADATA
 Comment: 
 
-Filename: Conanmail-1.0.7.dist-info/RECORD
+Filename: Conanmail-1.0.8.dist-info/WHEEL
+Comment: 
+
+Filename: Conanmail-1.0.8.dist-info/entry_points.txt
+Comment: 
+
+Filename: Conanmail-1.0.8.dist-info/top_level.txt
+Comment: 
+
+Filename: Conanmail-1.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## conan/utils.py

```diff
@@ -37,15 +37,15 @@
         self.send_response(200)
         self.send_header("Content-type", "application/json")
         self.send_header("Content-Disposition", "attachment; filename=\"domains.json\"")
         self.end_headers()
         self.wfile.write(dump)
 
     def _serve_template(self):
-        env = Environment(loader=FileSystemLoader('web'))
+        env = Environment(loader=FileSystemLoader(os.path.join(os.path.dirname(__file__), 'web')))
         template = env.get_template(os.path.join(os.path.dirname(__file__), 'index.html'))
         content = template.render(domains=[dict(x) for x in self.domains], email=self.email_address).encode()
         
         self.send_response(200)
         self.send_header("Content-type", "text/html")
         self.end_headers()
         self.wfile.write(content)
```

