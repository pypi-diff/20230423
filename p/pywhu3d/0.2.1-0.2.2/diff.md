# Comparing `tmp/pywhu3d-0.2.1-py3-none-any.whl.zip` & `tmp/pywhu3d-0.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 30685 bytes, number of entries: 18
+Zip file size: 30736 bytes, number of entries: 18
 -rw-r--r--  2.0 unx        0 b- defN 22-Oct-30 14:16 pywhu3d/__init__.py
--rw-r--r--  2.0 unx    12457 b- defN 22-Nov-06 03:47 pywhu3d/evaluation.py
--rw-r--r--  2.0 unx    23499 b- defN 23-Feb-28 08:32 pywhu3d/tool.py
+-rw-r--r--  2.0 unx    12682 b- defN 23-Apr-23 14:35 pywhu3d/evaluation.py
+-rw-r--r--  2.0 unx    23500 b- defN 23-Mar-04 06:47 pywhu3d/tool.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Oct-30 14:17 pywhu3d/configs/__init__.py
 -rw-r--r--  2.0 unx     5172 b- defN 22-Dec-03 05:50 pywhu3d/configs/als_config.py
 -rw-r--r--  2.0 unx     2285 b- defN 22-Oct-06 11:31 pywhu3d/configs/base_config.py
 -rw-r--r--  2.0 unx    11576 b- defN 22-Nov-05 11:35 pywhu3d/configs/mls_config.py
 -rw-r--r--  2.0 unx    13768 b- defN 22-Nov-19 08:32 pywhu3d/configs/mls_config_pole.py
 -rw-r--r--  2.0 unx     7411 b- defN 22-Nov-05 11:35 pywhu3d/configs/paris_config.py
 -rw-r--r--  2.0 unx     4395 b- defN 22-Nov-05 11:35 pywhu3d/configs/s3dis_config.py
 -rw-r--r--  2.0 unx     4283 b- defN 22-Oct-06 11:31 pywhu3d/configs/scannet_config.py
 -rw-r--r--  2.0 unx     4740 b- defN 22-Nov-05 11:35 pywhu3d/configs/toronto_config.py
 -rw-r--r--  2.0 unx      186 b- defN 22-Oct-06 11:31 pywhu3d/configs/wrap_configs.py
--rw-r--r--  2.0 unx     1076 b- defN 23-Feb-28 08:33 pywhu3d-0.2.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     1199 b- defN 23-Feb-28 08:33 pywhu3d-0.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-28 08:33 pywhu3d-0.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Feb-28 08:33 pywhu3d-0.2.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1486 b- defN 23-Feb-28 08:33 pywhu3d-0.2.1.dist-info/RECORD
-18 files, 93633 bytes uncompressed, 28251 bytes compressed:  69.8%
+-rw-r--r--  2.0 unx     1076 b- defN 23-Apr-23 14:37 pywhu3d-0.2.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1199 b- defN 23-Apr-23 14:37 pywhu3d-0.2.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-23 14:37 pywhu3d-0.2.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Apr-23 14:37 pywhu3d-0.2.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1486 b- defN 23-Apr-23 14:37 pywhu3d-0.2.2.dist-info/RECORD
+18 files, 93859 bytes uncompressed, 28302 bytes compressed:  69.8%
```

## zipnote {}

```diff
@@ -33,23 +33,23 @@
 
 Filename: pywhu3d/configs/toronto_config.py
 Comment: 
 
 Filename: pywhu3d/configs/wrap_configs.py
 Comment: 
 
-Filename: pywhu3d-0.2.1.dist-info/LICENSE
+Filename: pywhu3d-0.2.2.dist-info/LICENSE
 Comment: 
 
-Filename: pywhu3d-0.2.1.dist-info/METADATA
+Filename: pywhu3d-0.2.2.dist-info/METADATA
 Comment: 
 
-Filename: pywhu3d-0.2.1.dist-info/WHEEL
+Filename: pywhu3d-0.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: pywhu3d-0.2.1.dist-info/top_level.txt
+Filename: pywhu3d-0.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: pywhu3d-0.2.1.dist-info/RECORD
+Filename: pywhu3d-0.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pywhu3d/evaluation.py

```diff
@@ -12,14 +12,15 @@
 from rich.table import Column, Table
 from prettytable import PrettyTable as PT
 import xlwt
 from scipy import stats
 
 class Evaluator:
     def __init__(self, whu3d, pred):
+        assert len(pred) == 2, 'pred format wrong!'
         self.truth = []
         self.pred = []
         assert len(pred) == len(whu3d.scenes)
         for scene in whu3d.scenes:
             ins = whu3d.gt[scene]['semantics'].astype('int32')
             sem = whu3d.gt[scene]['instances'].astype('int32')
             self.truth.append(np.stack([ins, sem], axis=1))
@@ -30,15 +31,19 @@
         self.label2cat = whu3d.gt2cat
         self.compute_ins_list = whu3d.compute_ins_list
         self.workbook = None
         self.eval_list = None
         self.info = None
         self.eval_table = None
 
-
+    def set_gt(self, truth):
+        assert len(truth) == 2, 'gt format wrong!'
+        self.truth = []
+        for gt in truth:
+            self.truth.append(gt.astype('int32'))
 
     def compute_metrics(self):
         seg_label_to_cat = self.label2cat
         compute_ins_list = self.compute_ins_list
 
         pred_time = 0
         cluster_time = 0
@@ -304,15 +309,15 @@
     scenes = ['0404', '0940']
     whu3d = WHU3D(data_root=data_root, data_type='mls', format='h5', scenes=scenes)
     whu3d.interprete_labels()
     gts = []
     for scene in whu3d.scenes:
         ins = whu3d.gt[scene]['semantics']
         sem = whu3d.gt[scene]['instances']
-        gt = gts.append(np.stack([ins, sem], axis=1))
+        gts.append(np.stack([ins, sem], axis=1))
 
     eval = Evaluator(whu3d, gts)
     eval.compute_metrics()
     eval.export('/Users/hanxu/Downloads/')
     print(eval.eval_table)
     print(eval.info)
```

## pywhu3d/tool.py

```diff
@@ -225,15 +225,15 @@
                 else:
                     pprint('[orange1][Warning: loaded features number wrong!] passing %s' % scene)
                     continue
                 pprint('[bright_black]#return: %.1f, intensity: %.1f' % (return_num.max(), intensity.max()))
                 self.data[scene] = {}
                 self.labels[scene] = {}
                 self.data[scene]['number_returns'] = return_num.squeeze()
-                self.data[scene]['intensity'] = intensity.squeeze()
+                self.data[scene]['intensity'] = intensity.soqueeze()
             elif self.data_type == 'als':
                 x, y, z, sem, ins, r, g, b = np.split(points, points.shape[1], axis=1)
                 self.data[scene] = {}
                 self.labels[scene] = {}
             self.data[scene]['coords'] = np.concatenate([x, y, z], axis=-1)
             self.labels[scene]['semantics'] = sem.squeeze()
             self.labels[scene]['instances'] = ins.squeeze()
```

## Comparing `pywhu3d-0.2.1.dist-info/LICENSE` & `pywhu3d-0.2.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pywhu3d-0.2.1.dist-info/METADATA` & `pywhu3d-0.2.2.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywhu3d
-Version: 0.2.1
+Version: 0.2.2
 Summary: Example pywhu3d tool Package
 Home-page: https://github.com/astroy
 Author: Xu Han
 Author-email: hanxu@glad3d.com
 Keywords: whu3d,dataset,package
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

## Comparing `pywhu3d-0.2.1.dist-info/RECORD` & `pywhu3d-0.2.2.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 pywhu3d/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pywhu3d/evaluation.py,sha256=1lcw39gBHM643nVDxRPF8s6kLDWH2jpyPbF-WSu7Crg,12457
-pywhu3d/tool.py,sha256=FotKGxcL2U6ozIvuO-6-7XdO190jGR2r9C-Vti_K2tE,23499
+pywhu3d/evaluation.py,sha256=Etj9-4kPt0f4Dw9IzL4Ryn-YE9iyuYKUNGPl4IKB00Y,12682
+pywhu3d/tool.py,sha256=4htM7mkMr_APbKODpEXKGeBrFVM5pwaykPVIoNHHQdA,23500
 pywhu3d/configs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pywhu3d/configs/als_config.py,sha256=rA-T6OyyM085K8p7T_-iejYr3Xj7qEebI0YwleBiFXc,5172
 pywhu3d/configs/base_config.py,sha256=6UCAS9UCipC_h6quwik6KulWZkp2KxkTYbApRCrRiGQ,2285
 pywhu3d/configs/mls_config.py,sha256=StVuLEMN9gRyywnhMD7JpHBVCNN47PNf2swkRxegEOw,11576
 pywhu3d/configs/mls_config_pole.py,sha256=aTtouZrropJ_fbhUNcWjzdc-pTWV3fVeGE3IZ4_fldU,13768
 pywhu3d/configs/paris_config.py,sha256=JrBFXzUkLLMT20bRLlLIUqooXFWftu_qwa5avvG083Q,7411
 pywhu3d/configs/s3dis_config.py,sha256=bB8-j0um70lPLv03PeZvw-LkjKYLOc0bvzYVozsdFyw,4395
 pywhu3d/configs/scannet_config.py,sha256=dJjkjiP1l3VEWQ1Uluwd7lum_3LMvFt0l7TPz1NydgI,4283
 pywhu3d/configs/toronto_config.py,sha256=SxYgYKJ6bf7zaNlmszNdpwTy7126kCW9HsEwWT0xeXI,4740
 pywhu3d/configs/wrap_configs.py,sha256=9Lezbp6IStVpvS2BJiNm_qQ-9e9gyXT5TN-h_L4UbJg,186
-pywhu3d-0.2.1.dist-info/LICENSE,sha256=jAt62vPGMrWssYEKav2xAaDp8wjtKQScCguopKunN8Q,1076
-pywhu3d-0.2.1.dist-info/METADATA,sha256=YsuZJbgtC6V-M24JJRiClPjHImS_0Sh21E7tw92ax3s,1199
-pywhu3d-0.2.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-pywhu3d-0.2.1.dist-info/top_level.txt,sha256=XacQWDtHJRY_akQP8PPiX56iNHQ_epUiFTGekh1FP7g,8
-pywhu3d-0.2.1.dist-info/RECORD,,
+pywhu3d-0.2.2.dist-info/LICENSE,sha256=jAt62vPGMrWssYEKav2xAaDp8wjtKQScCguopKunN8Q,1076
+pywhu3d-0.2.2.dist-info/METADATA,sha256=oIU4lAYcBiLMr7ddKNsqHSQMKfbu5L5Eagb2AX3Ldhw,1199
+pywhu3d-0.2.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pywhu3d-0.2.2.dist-info/top_level.txt,sha256=XacQWDtHJRY_akQP8PPiX56iNHQ_epUiFTGekh1FP7g,8
+pywhu3d-0.2.2.dist-info/RECORD,,
```

