# Comparing `tmp/aug-tool-0.0.1.tar.gz` & `tmp/aug-tool-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aug-tool-0.0.1.tar", last modified: Fri Apr 14 20:35:45 2023, max compression
+gzip compressed data, was "aug-tool-0.0.2.tar", last modified: Sun Apr 23 15:47:50 2023, max compression
```

## Comparing `aug-tool-0.0.1.tar` & `aug-tool-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 20:35:45.546422 aug-tool-0.0.1/
--rw-rw-rw-   0        0        0     1089 2023-04-14 20:14:24.000000 aug-tool-0.0.1/LICENCE
--rw-rw-rw-   0        0        0       20 2023-04-14 20:14:30.000000 aug-tool-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      555 2023-04-14 20:35:45.546422 aug-tool-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-14 18:46:06.000000 aug-tool-0.0.1/README.md
--rw-rw-rw-   0        0        0      108 2023-04-14 20:14:26.000000 aug-tool-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      696 2023-04-14 20:35:45.547427 aug-tool-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-14 20:35:45.504667 aug-tool-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-14 20:35:45.539041 aug-tool-0.0.1/src/aug-tool/
--rw-rw-rw-   0        0        0     6583 2023-04-14 20:14:28.000000 aug-tool-0.0.1/src/aug-tool/Augmentation.py
--rw-rw-rw-   0        0        0        0 2023-04-14 18:48:21.000000 aug-tool-0.0.1/src/aug-tool/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 20:35:45.545362 aug-tool-0.0.1/src/aug_tool.egg-info/
--rw-rw-rw-   0        0        0      555 2023-04-14 20:35:45.000000 aug-tool-0.0.1/src/aug_tool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-04-14 20:35:45.000000 aug-tool-0.0.1/src/aug_tool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 20:35:45.000000 aug-tool-0.0.1/src/aug_tool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-14 20:35:45.000000 aug-tool-0.0.1/src/aug_tool.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 15:47:50.519628 aug-tool-0.0.2/
+-rw-rw-rw-   0        0        0     1089 2023-04-14 20:14:24.000000 aug-tool-0.0.2/LICENCE
+-rw-rw-rw-   0        0        0       20 2023-04-14 20:14:30.000000 aug-tool-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2725 2023-04-23 15:47:50.519628 aug-tool-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2059 2023-04-15 13:31:22.000000 aug-tool-0.0.2/README.md
+-rw-rw-rw-   0        0        0      108 2023-04-14 20:14:26.000000 aug-tool-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      805 2023-04-23 15:47:50.521622 aug-tool-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-23 15:47:50.479320 aug-tool-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-23 15:47:50.511683 aug-tool-0.0.2/src/aug-tool/
+-rw-rw-rw-   0        0        0     6540 2023-04-23 15:20:48.000000 aug-tool-0.0.2/src/aug-tool/Augmentation.py
+-rw-rw-rw-   0        0        0        0 2023-04-14 18:48:21.000000 aug-tool-0.0.2/src/aug-tool/__init__.py
+-rw-rw-rw-   0        0        0     3832 2023-04-23 15:46:09.000000 aug-tool-0.0.2/src/aug-tool/aug_tool.py
+-rw-rw-rw-   0        0        0      617 2023-04-23 15:47:09.000000 aug-tool-0.0.2/src/aug-tool/deneme.py
+drwxrwxrwx   0        0        0        0 2023-04-23 15:47:50.518632 aug-tool-0.0.2/src/aug_tool.egg-info/
+-rw-rw-rw-   0        0        0     2725 2023-04-23 15:47:50.000000 aug-tool-0.0.2/src/aug_tool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      300 2023-04-23 15:47:50.000000 aug-tool-0.0.2/src/aug_tool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 15:47:50.000000 aug-tool-0.0.2/src/aug_tool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-23 15:47:50.000000 aug-tool-0.0.2/src/aug_tool.egg-info/top_level.txt
```

### Comparing `aug-tool-0.0.1/LICENCE` & `aug-tool-0.0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `aug-tool-0.0.1/setup.cfg` & `aug-tool-0.0.2/setup.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,51 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 7567 2d74 6f6f 6c0d 0a76 6572   = aug-tool..ver
-00000020: 7369 6f6e 203d 2030 2e30 2e31 0d0a 6175  sion = 0.0.1..au
+00000020: 7369 6f6e 203d 2030 2e30 2e32 0d0a 6175  sion = 0.0.2..au
 00000030: 7468 6f72 203d 2048 616b 616e 2041 6b74  thor = Hakan Akt
 00000040: 61c5 9f0d 0a61 7574 686f 725f 656d 6169  a....author_emai
 00000050: 6c20 3d20 6861 6b61 6e61 6b74 6173 3435  l = hakanaktas45
 00000060: 3431 4067 6d61 696c 2e63 6f6d 0d0a 6465  41@gmail.com..de
-00000070: 7363 7269 7074 696f 6e20 3d20 4120 736d  scription = A sm
-00000080: 616c 6c20 7061 636b 6167 6520 746f 2069  all package to i
-00000090: 6e63 7265 6173 6520 796f 7572 2064 6174  ncrease your dat
-000000a0: 6120 666f 7220 796f 7572 206d 6163 6869  a for your machi
-000000b0: 6e65 206c 6561 726e 696e 6720 7072 6f6a  ne learning proj
-000000c0: 6563 740d 0a6c 6f6e 675f 6465 7363 7269  ect..long_descri
-000000d0: 7074 696f 6e20 3d20 6669 6c65 3a20 5245  ption = file: RE
-000000e0: 4144 4d45 2e6d 640d 0a6c 6f6e 675f 6465  ADME.md..long_de
-000000f0: 7363 7269 7074 696f 6e5f 636f 6e74 656e  scription_conten
-00000100: 745f 7479 7065 203d 2074 6578 742f 6d61  t_type = text/ma
-00000110: 726b 646f 776e 0d0a 7572 6c20 3d20 6874  rkdown..url = ht
-00000120: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000130: 2f68 616b 616e 616b 7461 7331 2f61 7567  /hakanaktas1/aug
-00000140: 2d74 6f6f 6c0d 0a70 726f 6a65 6374 5f75  -tool..project_u
-00000150: 726c 7320 3d20 0d0a 0942 7567 2054 7261  rls = ...Bug Tra
-00000160: 636b 6572 203d 2068 7474 7073 3a2f 2f67  cker = https://g
-00000170: 6974 6875 622e 636f 6d2f 6861 6b61 6e61  ithub.com/hakana
-00000180: 6b74 6173 312f 6175 672d 746f 6f6c 0d0a  ktas1/aug-tool..
-00000190: 636c 6173 7369 6669 6572 7320 3d20 0d0a  classifiers = ..
-000001a0: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
-000001b0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-000001c0: 3a3a 2033 0d0a 094c 6963 656e 7365 203a  :: 3...License :
-000001d0: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
-000001e0: 3a20 4d49 5420 4c69 6365 6e73 650d 0a09  : MIT License...
-000001f0: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
-00000200: 203a 3a20 4f53 2049 6e64 6570 656e 6465   :: OS Independe
-00000210: 6e74 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d  nt....[options].
-00000220: 0a70 6163 6b61 6765 5f64 6972 203d 200d  .package_dir = .
-00000230: 0a09 3d20 7372 630d 0a70 6163 6b61 6765  ..= src..package
-00000240: 7320 3d20 6669 6e64 3a0d 0a70 7974 686f  s = find:..pytho
-00000250: 6e5f 7265 7175 6972 6573 203d 203e 3d33  n_requires = >=3
-00000260: 2e36 0d0a 0d0a 5b6f 7074 696f 6e73 2e70  .6....[options.p
-00000270: 6163 6b61 6765 732e 6669 6e64 5d0d 0a77  ackages.find]..w
-00000280: 6865 7265 203d 2073 7263 0d0a 0d0a 5b65  here = src....[e
-00000290: 6767 5f69 6e66 6f5d 0d0a 7461 675f 6275  gg_info]..tag_bu
-000002a0: 696c 6420 3d20 0d0a 7461 675f 6461 7465  ild = ..tag_date
-000002b0: 203d 2030 0d0a 0d0a                       = 0....
+00000070: 7363 7269 7074 696f 6e20 3d20 4f75 7220  scription = Our 
+00000080: 6c69 6272 6172 7920 6973 206e 6f77 2061  library is now a
+00000090: 7661 696c 6162 6c65 206f 6e20 5079 5049  vailable on PyPI
+000000a0: 2066 6f72 2065 6173 7920 696e 7374 616c   for easy instal
+000000b0: 6c61 7469 6f6e 2061 6e64 2069 6e74 6567  lation and integ
+000000c0: 7261 7469 6f6e 2e20 446f 6e20 7420 7365  ration. Don t se
+000000d0: 7474 6c65 2066 6f72 206c 696d 6974 6564  ttle for limited
+000000e0: 2074 7261 696e 696e 6720 6461 7461 202d   training data -
+000000f0: 2074 7279 206f 7572 206c 6962 7261 7279   try our library
+00000100: 2074 6f64 6179 2061 6e64 2074 616b 6520   today and take 
+00000110: 796f 7572 204d 4c20 7072 6f6a 6563 7473  your ML projects
+00000120: 2074 6f20 6e65 7720 6865 6967 6874 7321   to new heights!
+00000130: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
+00000140: 6f6e 203d 2066 696c 653a 2052 4541 444d  on = file: READM
+00000150: 452e 6d64 0d0a 6c6f 6e67 5f64 6573 6372  E.md..long_descr
+00000160: 6970 7469 6f6e 5f63 6f6e 7465 6e74 5f74  iption_content_t
+00000170: 7970 6520 3d20 7465 7874 2f6d 6172 6b64  ype = text/markd
+00000180: 6f77 6e0d 0a75 726c 203d 2068 7474 7073  own..url = https
+00000190: 3a2f 2f67 6974 6875 622e 636f 6d2f 6861  ://github.com/ha
+000001a0: 6b61 6e61 6b74 6173 312f 6175 672d 746f  kanaktas1/aug-to
+000001b0: 6f6c 0d0a 7072 6f6a 6563 745f 7572 6c73  ol..project_urls
+000001c0: 203d 200d 0a09 4275 6720 5472 6163 6b65   = ...Bug Tracke
+000001d0: 7220 3d20 6874 7470 733a 2f2f 6769 7468  r = https://gith
+000001e0: 7562 2e63 6f6d 2f68 616b 616e 616b 7461  ub.com/hakanakta
+000001f0: 7331 2f61 7567 2d74 6f6f 6c0d 0a63 6c61  s1/aug-tool..cla
+00000200: 7373 6966 6965 7273 203d 200d 0a09 5072  ssifiers = ...Pr
+00000210: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+00000220: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+00000230: 330d 0a09 4c69 6365 6e73 6520 3a3a 204f  3...License :: O
+00000240: 5349 2041 7070 726f 7665 6420 3a3a 204d  SI Approved :: M
+00000250: 4954 204c 6963 656e 7365 0d0a 094f 7065  IT License...Ope
+00000260: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
+00000270: 204f 5320 496e 6465 7065 6e64 656e 740d   OS Independent.
+00000280: 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a 7061  ...[options]..pa
+00000290: 636b 6167 655f 6469 7220 3d20 0d0a 093d  ckage_dir = ...=
+000002a0: 2073 7263 0d0a 7061 636b 6167 6573 203d   src..packages =
+000002b0: 2066 696e 643a 0d0a 7079 7468 6f6e 5f72   find:..python_r
+000002c0: 6571 7569 7265 7320 3d20 3e3d 332e 360d  equires = >=3.6.
+000002d0: 0a0d 0a5b 6f70 7469 6f6e 732e 7061 636b  ...[options.pack
+000002e0: 6167 6573 2e66 696e 645d 0d0a 7768 6572  ages.find]..wher
+000002f0: 6520 3d20 7372 630d 0a0d 0a5b 6567 675f  e = src....[egg_
+00000300: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
+00000310: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date = 
+00000320: 300d 0a0d 0a                             0....
```

### Comparing `aug-tool-0.0.1/src/aug-tool/Augmentation.py` & `aug-tool-0.0.2/src/aug-tool/Augmentation.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         self.xml_file.find_all('path')[0].string =  self.data_name + ".jpg"
 
     def apply_noise_effect(self):
         """
         It takes an image and pastes it on top of another image.
         """
 
-        effect1_img = "C:\Users\hakan.aktas\Desktop\deneme\effect\effect_" + str(random.randint(1, 2)) + ".png"
+        effect1_img = "effect_" + str(random.randint(1, 2)) + ".png"
         
         with resources.open_binary('aug-tool', effect1_img) as fp:
             effect_img = fp.read()
         effect_img = Image.open(io.BytesIO(effect_img))
 
         effect1_img = effect1_img.resize((self.width, self.height))
         self.image_aug.paste(effect1_img, (0, 0), mask=effect1_img)
```

