# Comparing `tmp/wafl-0.0.8-py3-none-any.whl.zip` & `tmp/wafl-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -2,15 +2,15 @@
 -rw-rw-r--  2.0 unx        0 b- defN 21-Dec-12 17:38 wafl/__init__.py
 -rw-rw-r--  2.0 unx      834 b- defN 22-Jan-06 12:13 wafl/__main__.py
 -rw-rw-r--  2.0 unx     1800 b- defN 22-Oct-31 11:33 wafl/config.py
 -rw-rw-r--  2.0 unx     1895 b- defN 22-Oct-07 12:12 wafl/deixis.py
 -rw-rw-r--  2.0 unx       88 b- defN 22-Jan-05 11:44 wafl/exceptions.py
 -rw-rw-r--  2.0 unx      261 b- defN 22-Jul-23 08:36 wafl/facts.py
 -rw-rw-r--  2.0 unx      175 b- defN 21-Dec-20 11:53 wafl/rules.py
--rw-rw-r--  2.0 unx     2703 b- defN 22-Oct-31 16:03 wafl/run.py
+-rw-rw-r--  2.0 unx     2708 b- defN 22-Nov-02 21:14 wafl/run.py
 -rw-rw-r--  2.0 unx     1675 b- defN 22-Jan-08 17:06 wafl/testcases.py
 -rw-rw-r--  2.0 unx      102 b- defN 22-Feb-05 17:26 wafl/text_utils.py
 -rw-rw-r--  2.0 unx        0 b- defN 21-Dec-20 15:10 wafl/conversation/__init__.py
 -rw-rw-r--  2.0 unx     3352 b- defN 22-Oct-31 16:20 wafl/conversation/conversation.py
 -rw-rw-r--  2.0 unx     3662 b- defN 22-Oct-16 14:32 wafl/conversation/utils.py
 -rw-rw-r--  2.0 unx     1431 b- defN 22-Oct-01 09:34 wafl/conversation/working_memory.py
 -rw-rw-r--  2.0 unx        0 b- defN 21-Dec-29 12:22 wafl/inference/__init__.py
@@ -57,12 +57,12 @@
 -rw-rw-r--  2.0 unx      752 b- defN 22-Sep-03 16:29 wafl/speaker/soundfile_speaker.py
 -rw-rw-r--  2.0 unx        0 b- defN 21-Dec-12 18:41 wafl/templates/__init__.py
 -rw-rw-r--  2.0 unx      264 b- defN 22-Oct-31 17:56 wafl/templates/config.json
 -rw-rw-r--  2.0 unx      104 b- defN 22-Jan-06 14:55 wafl/templates/functions.py
 -rw-rw-r--  2.0 unx      124 b- defN 22-Jan-09 11:54 wafl/templates/rules.wafl
 -rw-rw-r--  2.0 unx        0 b- defN 21-Dec-12 18:21 wafl/templates/server.py
 -rw-rw-r--  2.0 unx      122 b- defN 22-Jan-09 11:54 wafl/templates/testcases.txt
--rw-rw-r--  2.0 unx     1433 b- defN 22-Nov-02 21:12 wafl-0.0.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 22-Nov-02 21:12 wafl-0.0.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx        5 b- defN 22-Nov-02 21:12 wafl-0.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     5348 b- defN 22-Nov-02 21:12 wafl-0.0.8.dist-info/RECORD
-66 files, 4138637 bytes uncompressed, 1745223 bytes compressed:  57.8%
+-rw-rw-r--  2.0 unx     1433 b- defN 22-Nov-02 21:15 wafl-0.0.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 22-Nov-02 21:15 wafl-0.0.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        5 b- defN 22-Nov-02 21:15 wafl-0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     5348 b- defN 22-Nov-02 21:15 wafl-0.0.9.dist-info/RECORD
+66 files, 4138642 bytes uncompressed, 1745223 bytes compressed:  57.8%
```

## zipnote {}

```diff
@@ -180,20 +180,20 @@
 
 Filename: wafl/templates/server.py
 Comment: 
 
 Filename: wafl/templates/testcases.txt
 Comment: 
 
-Filename: wafl-0.0.8.dist-info/METADATA
+Filename: wafl-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: wafl-0.0.8.dist-info/WHEEL
+Filename: wafl-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: wafl-0.0.8.dist-info/top_level.txt
+Filename: wafl-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: wafl-0.0.8.dist-info/RECORD
+Filename: wafl-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## wafl/run.py

```diff
@@ -1,13 +1,13 @@
-from logger.local_file_logger import LocalFileLogger
 from wafl.config import Configuration
 from wafl.exceptions import CloseConversation
 from wafl.conversation.conversation import Conversation
 from wafl.interface.command_line_interface import CommandLineInterface
 from wafl.interface.voice_interface import VoiceInterface
+from wafl.logger.local_file_logger import LocalFileLogger
 from wafl.knowledge.knowledge import Knowledge
 from wafl.testcases import ConversationTestCases
 
 _logger = LocalFileLogger(__file__)
 
 
 def run_from_command_line():
```

## Comparing `wafl-0.0.8.dist-info/METADATA` & `wafl-0.0.9.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wafl
-Version: 0.0.8
+Version: 0.0.9
 Summary: A hybrid chatbot.
 Home-page: http://github.com/fractalego/wafl
 Author: Alberto Cetoli
 Author-email: alberto@fractalego.io
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `wafl-0.0.8.dist-info/RECORD` & `wafl-0.0.9.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 wafl/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 wafl/__main__.py,sha256=M8lT1vSuPqK2XPU1Vb3ECym3Zb20tYBhIpGEOCmXyAs,834
 wafl/config.py,sha256=7Jwto8JXGX4z0cPq87Avshj9vAJcq8eVBsY2Z-Q6vsE,1800
 wafl/deixis.py,sha256=ZmcrGWsWYoaYZJv3NyMJaaesxhmSzwSles_mEnYX-Cc,1895
 wafl/exceptions.py,sha256=rAFJfIzkDiSDNunI__wEllL2RvoJbwTnbiVLXQO5DW0,88
 wafl/facts.py,sha256=1QlPjB-X56FjNf0I_9QgxbRFXP2xqw-9_UWwZpo8CKM,261
 wafl/rules.py,sha256=uqqU9RI6hk9HW4MTU7oRN14b4ze_kwGizd19BfGbn9E,175
-wafl/run.py,sha256=OJ_QkJV1Qk4ev78j1fG6Cus5vxwf-iwWkGuRU45ogc8,2703
+wafl/run.py,sha256=PoO46wArTJfIQvr0eQcKV0GnggFi6T_k1xqnBc72aFk,2708
 wafl/testcases.py,sha256=wHKDox-VzJhvvjRNfGuYqj11wy-ZcAty2wHDYwvLGNs,1675
 wafl/text_utils.py,sha256=zzmGu7fWftv2vFqxFNv7RCDjr4-d_jVr79Hbwe98orQ,102
 wafl/conversation/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 wafl/conversation/conversation.py,sha256=ksJ8WIfEiJpzVKA1F74buqdW9e52RDGHRZZ-U8SMLJQ,3352
 wafl/conversation/utils.py,sha256=MygO6sbzFe7lXA8OYBylISEK75bMxSNKxgscWQpMMfU,3662
 wafl/conversation/working_memory.py,sha256=t_rrW3QdAit3loA2SbIfAxCHOo15jG9PKzFY_vZ_mCk,1431
 wafl/inference/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -56,11 +56,11 @@
 wafl/speaker/soundfile_speaker.py,sha256=rDoRnjCuVpiRljzUIAZxf2g_7aRy9cKJmQxcM6VQDAA,752
 wafl/templates/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 wafl/templates/config.json,sha256=v3CYw-2Okn92wpInKY_slAbYtbI4wKV6aCMGhVL37UA,264
 wafl/templates/functions.py,sha256=YD6q0R_iprH6_NlmdmX7JQPVVEei-u2p0iSf_BLjZzk,104
 wafl/templates/rules.wafl,sha256=OPacBQwihZW6sd96vdlcr1MCKTjmdra7HfKkScw4P8I,124
 wafl/templates/server.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 wafl/templates/testcases.txt,sha256=fhlNOp_RQffLWdEgs6fFagd03hx9QjyczJ4dWfk8hZ0,122
-wafl-0.0.8.dist-info/METADATA,sha256=jrHsWk1LMSSDbHsJQ0HH3iiUh6lJPtRCSTez0rfoVf8,1433
-wafl-0.0.8.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-wafl-0.0.8.dist-info/top_level.txt,sha256=NdV2vpxhV56ibAA9ksvtBmwWZS8mRLjqEdYPFIyr1p8,5
-wafl-0.0.8.dist-info/RECORD,,
+wafl-0.0.9.dist-info/METADATA,sha256=CkwFLMP5izGkPmZm1YaKEI5EKH3AL1HE_T3ezC3iQGA,1433
+wafl-0.0.9.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+wafl-0.0.9.dist-info/top_level.txt,sha256=NdV2vpxhV56ibAA9ksvtBmwWZS8mRLjqEdYPFIyr1p8,5
+wafl-0.0.9.dist-info/RECORD,,
```

