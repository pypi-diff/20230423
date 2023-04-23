# Comparing `tmp/torch_book-0.0.6-py3-none-any.whl.zip` & `tmp/torch_book-0.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 54298 bytes, number of entries: 42
--rw-r--r--  2.0 unx       51 b- defN 23-Apr-23 15:15 torch_book/__init__.py
+Zip file size: 54300 bytes, number of entries: 42
+-rw-r--r--  2.0 unx       51 b- defN 23-Apr-23 15:17 torch_book/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Mar-13 15:28 torch_book/backend/__init__.py
 -rw-r--r--  2.0 unx      533 b- defN 23-Mar-13 15:28 torch_book/backend/gpu.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Mar-30 17:18 torch_book/datasets/__init__.py
 -rw-r--r--  2.0 unx     1408 b- defN 23-Mar-30 17:20 torch_book/datasets/imagenet.py
 -rw-r--r--  2.0 unx     3972 b- defN 23-Apr-08 17:38 torch_book/datasets/simple_vision.py
 -rw-r--r--  2.0 unx       48 b- defN 23-Mar-13 15:28 torch_book/plotx/__init__.py
 -rw-r--r--  2.0 unx     2742 b- defN 23-Mar-13 15:28 torch_book/plotx/bbox.py
@@ -33,12 +33,12 @@
 -rw-r--r--  2.0 unx        0 b- defN 23-Mar-13 15:28 torch_book/vision/__init__.py
 -rw-r--r--  2.0 unx     5844 b- defN 23-Mar-13 15:28 torch_book/vision/_classifier2.py
 -rw-r--r--  2.0 unx     4059 b- defN 23-Mar-13 15:28 torch_book/vision/_model.py
 -rw-r--r--  2.0 unx     5238 b- defN 23-Mar-13 15:28 torch_book/vision/classifier.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Mar-13 15:28 torch_book/vision/model.py
 -rw-r--r--  2.0 unx     3245 b- defN 23-Mar-13 15:28 torch_book/vision/optim.py
 -rw-r--r--  2.0 unx      729 b- defN 23-Mar-13 15:28 torch_book/vision/utils.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Mar-13 15:28 torch_book-0.0.6.dist-info/LICENSE
-?rw-r--r--  2.0 unx       81 b- defN 16-Jan-01 00:00 torch_book-0.0.6.dist-info/WHEEL
-?rw-r--r--  2.0 unx     4507 b- defN 16-Jan-01 00:00 torch_book-0.0.6.dist-info/METADATA
-?rw-r--r--  2.0 unx     3636 b- defN 16-Jan-01 00:00 torch_book-0.0.6.dist-info/RECORD
-42 files, 148364 bytes uncompressed, 48436 bytes compressed:  67.4%
+-rw-r--r--  2.0 unx    11357 b- defN 23-Mar-13 15:28 torch_book-0.0.7.dist-info/LICENSE
+?rw-r--r--  2.0 unx       81 b- defN 16-Jan-01 00:00 torch_book-0.0.7.dist-info/WHEEL
+?rw-r--r--  2.0 unx     4508 b- defN 16-Jan-01 00:00 torch_book-0.0.7.dist-info/METADATA
+?rw-r--r--  2.0 unx     3636 b- defN 16-Jan-01 00:00 torch_book-0.0.7.dist-info/RECORD
+42 files, 148365 bytes uncompressed, 48438 bytes compressed:  67.4%
```

## zipnote {}

```diff
@@ -108,20 +108,20 @@
 
 Filename: torch_book/vision/optim.py
 Comment: 
 
 Filename: torch_book/vision/utils.py
 Comment: 
 
-Filename: torch_book-0.0.6.dist-info/LICENSE
+Filename: torch_book-0.0.7.dist-info/LICENSE
 Comment: 
 
-Filename: torch_book-0.0.6.dist-info/WHEEL
+Filename: torch_book-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: torch_book-0.0.6.dist-info/METADATA
+Filename: torch_book-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: torch_book-0.0.6.dist-info/RECORD
+Filename: torch_book-0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## torch_book/__init__.py

```diff
@@ -1,3 +1,3 @@
 """Dive into Torch Book."""
 
-__version__ = "0.0.6"
+__version__ = "0.0.7"
```

## Comparing `torch_book-0.0.6.dist-info/LICENSE` & `torch_book-0.0.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `torch_book-0.0.6.dist-info/METADATA` & `torch_book-0.0.7.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: torch-book
-Version: 0.0.6
+Version: 0.0.7
 Summary: Dive into Torch Book.
 Author-email: xinetzone <735613050@qq.com>
 Maintainer-email: xinetzone <735613050@qq.com>
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Sphinx
 Classifier: Framework :: Sphinx :: Theme
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

## Comparing `torch_book-0.0.6.dist-info/RECORD` & `torch_book-0.0.7.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-torch_book/__init__.py,sha256=DAOqegGyM1u45K8Qy0hZU4rrcgmzE-psnZUlqaFghg8,51
+torch_book/__init__.py,sha256=MogB2c0YMdaECMQHRlrEYAWfSpbyPBWN1UjoxpFCb-M,51
 torch_book/backend/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 torch_book/backend/gpu.py,sha256=8KEtrj4u7qYM5lgOry0aQzTxiYRFXkmcSDqOyOFJVr8,533
 torch_book/datasets/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 torch_book/datasets/imagenet.py,sha256=5JCccJ4vPNdVvBh3iZ9gpnytROWbzBB_zVZxdGNdZq8,1408
 torch_book/datasets/simple_vision.py,sha256=wS18odR6UOU5vlcFrQg7uVNARpT_Xog7BJmD1sc5Hpg,3972
 torch_book/plotx/__init__.py,sha256=fRZZD2rIr3z59JtcXvLWqzPeztVgj7SvptqLLDDdNFk,48
 torch_book/plotx/bbox.py,sha256=lez7sHs9vwbx31JSOOGgGGmED47wDCdz8ahE8mGM-rw,2742
@@ -32,11 +32,11 @@
 torch_book/vision/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 torch_book/vision/_classifier2.py,sha256=4N2skg40uRWZ694lHSYZFU1Gkg_gCh0ceiOJ9dd07Vo,5844
 torch_book/vision/_model.py,sha256=WHBv9Vyu8rCtS8wbnRmSmZhp3RHpQihKUZBAfAJUwuE,4059
 torch_book/vision/classifier.py,sha256=CsfZ4UpK0qkHxAgT-hS6EAZY3ROp10lsqDK2hDIpFzU,5238
 torch_book/vision/model.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 torch_book/vision/optim.py,sha256=yd-6ntRK0q53l279rkHEVoX5mCrUQIo0nlPmJbkBHBg,3245
 torch_book/vision/utils.py,sha256=c43gKjgpYfLqJPUk4laVuEsTPPjRWyHpwhcQ_hyTrOk,729
-torch_book-0.0.6.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-torch_book-0.0.6.dist-info/WHEEL,sha256=rSgq_JpHF9fHR1lx53qwg_1-2LypZE_qmcuXbVUq948,81
-torch_book-0.0.6.dist-info/METADATA,sha256=WgYPAEAeqRE_9Y0ZR4qtO9z7XemC29Gth5GezCiCzSU,4507
-torch_book-0.0.6.dist-info/RECORD,,
+torch_book-0.0.7.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+torch_book-0.0.7.dist-info/WHEEL,sha256=rSgq_JpHF9fHR1lx53qwg_1-2LypZE_qmcuXbVUq948,81
+torch_book-0.0.7.dist-info/METADATA,sha256=QikqbCx0B4khMdnXZdd2NNKdF1oPRtgTubSRUTjXOC8,4508
+torch_book-0.0.7.dist-info/RECORD,,
```

