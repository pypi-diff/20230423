# Comparing `tmp/demoparser2-0.0.5-cp39-none-win_amd64.whl.zip` & `tmp/demoparser2-0.0.6-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 3184347 bytes, number of entries: 5
--rw-r--r--  4.6 unx     5493 b- defN 23-Apr-20 16:19 demoparser2-0.0.5.dist-info/METADATA
--rw-r--r--  4.6 unx       95 b- defN 23-Apr-20 16:19 demoparser2-0.0.5.dist-info/WHEEL
--rw-r--r--  4.6 unx      127 b- defN 23-Apr-20 16:19 demoparser2/__init__.py
--rwxr-xr-x  4.6 unx 12608000 b- defN 23-Apr-20 16:19 demoparser2/demoparser2.cp39-win_amd64.pyd
--rw-r--r--  4.6 unx      400 b- defN 23-Apr-20 16:19 demoparser2-0.0.5.dist-info/RECORD
-5 files, 12614115 bytes uncompressed, 3183609 bytes compressed:  74.8%
+Zip file size: 3187159 bytes, number of entries: 5
+-rw-r--r--  4.6 unx     5324 b- defN 23-Apr-23 19:32 demoparser2-0.0.6.dist-info/METADATA
+-rw-r--r--  4.6 unx       95 b- defN 23-Apr-23 19:32 demoparser2-0.0.6.dist-info/WHEEL
+-rw-r--r--  4.6 unx      127 b- defN 23-Apr-23 19:32 demoparser2/__init__.py
+-rwxr-xr-x  4.6 unx 12622848 b- defN 23-Apr-23 19:32 demoparser2/demoparser2.cp39-win_amd64.pyd
+-rw-r--r--  4.6 unx      400 b- defN 23-Apr-23 19:32 demoparser2-0.0.6.dist-info/RECORD
+5 files, 12628794 bytes uncompressed, 3186421 bytes compressed:  74.8%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: demoparser2-0.0.5.dist-info/METADATA
+Filename: demoparser2-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: demoparser2-0.0.5.dist-info/WHEEL
+Filename: demoparser2-0.0.6.dist-info/WHEEL
 Comment: 
 
 Filename: demoparser2/__init__.py
 Comment: 
 
 Filename: demoparser2/demoparser2.cp39-win_amd64.pyd
 Comment: 
 
-Filename: demoparser2-0.0.5.dist-info/RECORD
+Filename: demoparser2-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `demoparser2-0.0.5.dist-info/METADATA` & `demoparser2-0.0.6.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: demoparser2
-Version: 0.0.5
+Version: 0.0.6
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: polars
 Requires-Dist: pyarrow
@@ -25,26 +25,21 @@
 This will have to do for now 😂
 
 ### Utility functions
 ```python
 parser = DemoParser("path_to_demo.dem")
 
 # returns list like: ["player_death", "weapon_fire"...]
-name_list = parser.list_game_events()
-# returns dict like: {"m_iHealth": 41487, "m_iPing": 4871} where 
-# key is field name and val is how many times it was updated.
-freq_dict = parser.list_entity_values()
-
+event_name_list = parser.list_game_events()
 
 df = parser.parse_grenades()
 df = parser.parse_item_drops()
 df = parser.parse_skins()
 df = parser.parse_player_info()
 dict_output = parser.parse_convars()
-
 ```
 All of these take no arguments and return the same shape data. Probably easiest to understand by just trying these out.
 
 ### Game events
 ```python
 from demoparser2 import DemoParser
```

