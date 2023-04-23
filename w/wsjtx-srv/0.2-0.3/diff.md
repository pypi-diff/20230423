# Comparing `tmp/wsjtx_srv-0.2.tar.gz` & `tmp/wsjtx_srv-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wsjtx_srv-0.2.tar", last modified: Sat May 14 10:28:46 2022, max compression
+gzip compressed data, was "wsjtx_srv-0.3.tar", last modified: Sun Apr 23 07:22:06 2023, max compression
```

## Comparing `wsjtx_srv-0.2.tar` & `wsjtx_srv-0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2022-05-14 10:28:46.572507 wsjtx_srv-0.2/
--rw-r--r--   0 ralf      (1000) priv      (1011)     2319 2022-05-14 10:28:46.576507 wsjtx_srv-0.2/PKG-INFO
--rw-r--r--   0 ralf      (1000) priv      (1011)     7980 2022-05-14 10:28:06.396516 wsjtx_srv-0.2/README.html
--rw-r--r--   0 ralf      (1000) priv      (1011)     1355 2022-05-14 10:26:35.336538 wsjtx_srv-0.2/README.rst
-drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2022-05-14 10:28:46.572507 wsjtx_srv-0.2/bin/
--rwxr-xr-x   0 ralf      (1000) priv      (1011)      979 2021-10-26 11:43:05.045461 wsjtx_srv-0.2/bin/wbf
--rwxr-xr-x   0 ralf      (1000) priv      (1011)       56 2021-09-13 11:37:43.842778 wsjtx_srv-0.2/bin/wsjtx-srv
--rw-r--r--   0 ralf      (1000) priv      (1011)     3089 2022-05-14 10:25:48.328549 wsjtx_srv-0.2/setup.py
-drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2022-05-14 10:28:46.572507 wsjtx_srv-0.2/wsjtx_srv/
--rw-r--r--   0 ralf      (1000) priv      (1011)       14 2022-05-14 10:28:06.396516 wsjtx_srv-0.2/wsjtx_srv/Version.py
--rw-r--r--   0 ralf      (1000) priv      (1011)       21 2021-09-13 11:36:52.530794 wsjtx_srv-0.2/wsjtx_srv/__init__.py
--rwxr-xr-x   0 ralf      (1000) priv      (1011)    45250 2021-10-26 13:20:53.875702 wsjtx_srv-0.2/wsjtx_srv/wsjtx.py
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-04-23 07:22:06.562580 wsjtx_srv-0.3/
+-rw-r--r--   0 ralf      (1000) priv      (1011)     2519 2023-04-23 07:22:06.566580 wsjtx_srv-0.3/PKG-INFO
+-rw-r--r--   0 ralf      (1000) priv      (1011)     8175 2023-04-23 07:21:47.154585 wsjtx_srv-0.3/README.html
+-rw-r--r--   0 ralf      (1000) priv      (1011)     1507 2023-04-23 07:21:15.394593 wsjtx_srv-0.3/README.rst
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-04-23 07:22:06.558580 wsjtx_srv-0.3/bin/
+-rwxr-xr-x   0 ralf      (1000) priv      (1011)      979 2021-10-26 11:43:05.045461 wsjtx_srv-0.3/bin/wbf
+-rwxr-xr-x   0 ralf      (1000) priv      (1011)       56 2021-09-13 11:37:43.842778 wsjtx_srv-0.3/bin/wsjtx-srv
+-rw-r--r--   0 ralf      (1000) priv      (1011)     3089 2022-05-14 10:25:48.328549 wsjtx_srv-0.3/setup.py
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-04-23 07:22:06.562580 wsjtx_srv-0.3/wsjtx_srv/
+-rw-r--r--   0 ralf      (1000) priv      (1011)       14 2023-04-23 07:21:47.154585 wsjtx_srv-0.3/wsjtx_srv/Version.py
+-rw-r--r--   0 ralf      (1000) priv      (1011)       21 2021-09-13 11:36:52.530794 wsjtx_srv-0.3/wsjtx_srv/__init__.py
+-rwxr-xr-x   0 ralf      (1000) priv      (1011)    45636 2023-04-23 07:17:49.078639 wsjtx_srv-0.3/wsjtx_srv/wsjtx.py
```

### Comparing `wsjtx_srv-0.2/PKG-INFO` & `wsjtx_srv-0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: wsjtx_srv
-Version: 0.2
+Version: 0.3
 Summary: Library implementation of WSJTX companion program
 Home-page: https://github.com/schlatterbeck/wsjtx-srv
 Author: Ralf Schlatterbeck
 Author-email: rsc@runtux.com
 License: BSD License
 Description: wsjtx-srv: Library for WSJT-X server implementation
         ===================================================
@@ -32,14 +32,20 @@
         before status.
         
         .. _WSJT-X: https://physics.princeton.edu/pulsar/k1jt/wsjtx.html
         
         Changes
         -------
         
+        Version 0.3: Small fixes
+        
+        - Compatibility with older protocol versions, thanks to Sampo Savolainen
+          for the patch
+        - Fix band lookup if no QSO on band
+        
         Version 0.2: Fix setup.py install_requires
         
         Version 0.1: Initial implementation
         
         - Implement serialization and deserialization of WSJT-X_ telegrams and a
           simple server
         - First Release
```

### Comparing `wsjtx_srv-0.2/README.html` & `wsjtx_srv-0.3/README.html`

 * *Files 2% similar despite different names*

```diff
@@ -301,14 +301,20 @@
 <p>The implementation of <tt class="docutils literal"><span class="pre">wsjtx-srv</span></tt> should give a rough idea of how to use
 this in your own projects.</p>
 <p>There is a companion-program <tt class="docutils literal">wbf</tt> standing for <em>worked before</em> that
 takes a number of callsigns on the command-line and tells you the worked
 before status.</p>
 <div class="section" id="changes">
 <h1>Changes</h1>
+<p>Version 0.3: Small fixes</p>
+<ul class="simple">
+<li>Compatibility with older protocol versions, thanks to Sampo Savolainen
+for the patch</li>
+<li>Fix band lookup if no QSO on band</li>
+</ul>
 <p>Version 0.2: Fix setup.py install_requires</p>
 <p>Version 0.1: Initial implementation</p>
 <ul class="simple">
 <li>Implement serialization and deserialization of <a class="reference external" href="https://physics.princeton.edu/pulsar/k1jt/wsjtx.html">WSJT-X</a> telegrams and a
 simple server</li>
 <li>First Release</li>
 </ul>
```

### Comparing `wsjtx_srv-0.2/README.rst` & `wsjtx_srv-0.3/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -24,14 +24,20 @@
 before status.
 
 .. _WSJT-X: https://physics.princeton.edu/pulsar/k1jt/wsjtx.html
 
 Changes
 -------
 
+Version 0.3: Small fixes
+
+- Compatibility with older protocol versions, thanks to Sampo Savolainen
+  for the patch
+- Fix band lookup if no QSO on band
+
 Version 0.2: Fix setup.py install_requires
 
 Version 0.1: Initial implementation
 
 - Implement serialization and deserialization of WSJT-X_ telegrams and a
   simple server
 - First Release
```

### Comparing `wsjtx_srv-0.2/bin/wbf` & `wsjtx_srv-0.3/bin/wbf`

 * *Files identical despite different names*

### Comparing `wsjtx_srv-0.2/setup.py` & `wsjtx_srv-0.3/setup.py`

 * *Files identical despite different names*

### Comparing `wsjtx_srv-0.2/wsjtx_srv/wsjtx.py` & `wsjtx_srv-0.3/wsjtx_srv/wsjtx.py`

 * *Files 0% similar despite different names*

```diff
@@ -328,14 +328,20 @@
     # end def from_bytes
 
     @classmethod
     def deserialize (cls, bytes) :
         b  = bytes
         kw = {}
         for name, (format, length) in cls.format :
+            # Due to compatibility reasons new message fields are added to
+            # the end of the messsage. The buffer is empty when the message
+            # is older format and a field is missing.
+            if (len(b) == 0):
+                kw[name] = None
+                continue
             if isinstance (format, type ('')) :
                 kw [name] = unpack (format, b [:length]) [0]
                 b = b [length:]
             else :
                 value = format.deserialize (b, length)
                 b = b [value.serialization_size:]
                 kw [name] = value.value
@@ -1113,14 +1119,16 @@
         if r :
             return 'wbf'
         dxccs = self.fuzzy_match_dxcc_code (call)
         if not dxccs :
             return 'new_dxcc'
         r2 = 1
         for dxcc in dxccs :
+            if band not in self.dxcc_info:
+                self.dxcc_info [band] = WBF (band)
             r2 = r2 and self.dxcc_info [band].lookup (dxcc)
         # Matched for *all* dxccs; not new dxcc on this (and any) band
         if r2 :
             for dxcc in dxccs :
                 if dxcc in self.args.highlight_dxcc :
                     return 'highlight'
             return self.lookup_new_call (call)
```

