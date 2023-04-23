# Comparing `tmp/utils_cv-baiyigali-0.0.8.tar.gz` & `tmp/utils_cv-baiyigali-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/utils_cv-baiyigali-0.0.8.tar", last modified: Sun Mar 27 15:02:00 2022, max compression
+gzip compressed data, was "dist/utils_cv-baiyigali-0.0.9.tar", last modified: Sat Apr  2 10:32:18 2022, max compression
```

## Comparing `utils_cv-baiyigali-0.0.8.tar` & `utils_cv-baiyigali-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-27 15:02:00.000000 utils_cv-baiyigali-0.0.8/
--rw-rw-r--   0 root         (0) root         (0)       93 2022-03-21 10:32:26.000000 utils_cv-baiyigali-0.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      857 2022-03-27 15:01:33.000000 utils_cv-baiyigali-0.0.8/setup.py
--rw-rw-r--   0 root         (0) root         (0)      170 2022-03-21 10:41:14.000000 utils_cv-baiyigali-0.0.8/README.md
--rw-rw-r--   0 root         (0) root         (0)      610 2022-03-27 15:02:00.000000 utils_cv-baiyigali-0.0.8/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1073 2022-03-21 10:42:04.000000 utils_cv-baiyigali-0.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)      725 2022-03-27 15:02:00.000000 utils_cv-baiyigali-0.0.8/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-27 15:02:00.000000 utils_cv-baiyigali-0.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-27 15:02:00.000000 utils_cv-baiyigali-0.0.8/src/utils_cv/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-27 15:02:00.000000 utils_cv-baiyigali-0.0.8/src/utils_cv/utils_benchmark/
--rw-r--r--   0 root         (0) root         (0)     3381 2022-03-27 14:43:39.000000 utils_cv-baiyigali-0.0.8/src/utils_cv/utils_benchmark/end2end.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-27 14:11:13.000000 utils_cv-baiyigali-0.0.8/src/utils_cv/utils_benchmark/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4189 2022-03-27 03:11:15.000000 utils_cv-baiyigali-0.0.8/src/utils_cv/utils_box.py
--rw-rw-r--   0 root         (0) root         (0)        0 2022-03-21 10:26:52.000000 utils_cv-baiyigali-0.0.8/src/utils_cv/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4304 2022-03-27 04:29:22.000000 utils_cv-baiyigali-0.0.8/src/utils_cv/utils_layout.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-27 15:02:00.000000 utils_cv-baiyigali-0.0.8/src/utils_cv_baiyigali.egg-info/
--rw-rw-r--   0 root         (0) root         (0)        1 2022-03-27 15:02:00.000000 utils_cv-baiyigali-0.0.8/src/utils_cv_baiyigali.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)      396 2022-03-27 15:02:00.000000 utils_cv-baiyigali-0.0.8/src/utils_cv_baiyigali.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        9 2022-03-27 15:02:00.000000 utils_cv-baiyigali-0.0.8/src/utils_cv_baiyigali.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      725 2022-03-27 15:02:00.000000 utils_cv-baiyigali-0.0.8/src/utils_cv_baiyigali.egg-info/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-02 10:32:17.000000 utils_cv-baiyigali-0.0.9/
+-rw-rw-r--   0 root         (0) root         (0)       93 2022-03-21 10:32:26.000000 utils_cv-baiyigali-0.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      858 2022-04-02 10:32:09.000000 utils_cv-baiyigali-0.0.9/setup.py
+-rw-rw-r--   0 root         (0) root         (0)      170 2022-03-21 10:41:14.000000 utils_cv-baiyigali-0.0.9/README.md
+-rw-rw-r--   0 root         (0) root         (0)      610 2022-04-02 10:32:17.000000 utils_cv-baiyigali-0.0.9/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1073 2022-03-21 10:42:04.000000 utils_cv-baiyigali-0.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      725 2022-04-02 10:32:17.000000 utils_cv-baiyigali-0.0.9/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-02 10:32:17.000000 utils_cv-baiyigali-0.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-02 10:32:17.000000 utils_cv-baiyigali-0.0.9/src/utils_cv/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-02 10:32:17.000000 utils_cv-baiyigali-0.0.9/src/utils_cv/utils_benchmark/
+-rw-r--r--   0 root         (0) root         (0)     6125 2022-04-02 10:29:00.000000 utils_cv-baiyigali-0.0.9/src/utils_cv/utils_benchmark/end2end.py
+-rw-r--r--   0 root         (0) root         (0)     1882 2022-04-02 10:29:00.000000 utils_cv-baiyigali-0.0.9/src/utils_cv/utils_benchmark/text_detection.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-03-27 14:11:13.000000 utils_cv-baiyigali-0.0.9/src/utils_cv/utils_benchmark/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4296 2022-04-02 10:29:00.000000 utils_cv-baiyigali-0.0.9/src/utils_cv/utils_box.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-03-21 10:26:52.000000 utils_cv-baiyigali-0.0.9/src/utils_cv/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4304 2022-03-27 15:05:31.000000 utils_cv-baiyigali-0.0.9/src/utils_cv/utils_layout.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-02 10:32:17.000000 utils_cv-baiyigali-0.0.9/src/utils_cv_baiyigali.egg-info/
+-rw-rw-r--   0 root         (0) root         (0)        1 2022-04-02 10:32:17.000000 utils_cv-baiyigali-0.0.9/src/utils_cv_baiyigali.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)      443 2022-04-02 10:32:17.000000 utils_cv-baiyigali-0.0.9/src/utils_cv_baiyigali.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        9 2022-04-02 10:32:17.000000 utils_cv-baiyigali-0.0.9/src/utils_cv_baiyigali.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      725 2022-04-02 10:32:17.000000 utils_cv-baiyigali-0.0.9/src/utils_cv_baiyigali.egg-info/PKG-INFO
```

### Comparing `utils_cv-baiyigali-0.0.8/setup.py` & `utils_cv-baiyigali-0.0.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="utils_cv-baiyigali",
-    version="0.0.8",
+    version="0.0.9",
     author="baiyigali",
     author_email="1304646911@qq.com",
     description="A small example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pypa/sampleproject",
     project_urls={
@@ -18,11 +18,11 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
-    test_suite='nose.collector',
-    tests_require=['nose'],
+    test_suite="nose.collector",
+    tests_require=["nose"],
     python_requires=">=3.6",
-)
+)
```

### Comparing `utils_cv-baiyigali-0.0.8/setup.cfg` & `utils_cv-baiyigali-0.0.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = utils_cv-baiyigali
-version = 0.0.8
+version = 0.0.9
 author = baiyigali
 author_email = 1304646911@qq.com
 description = CV utilites
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pypa/sampleproject
 project_urls =
```

### Comparing `utils_cv-baiyigali-0.0.8/LICENSE` & `utils_cv-baiyigali-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `utils_cv-baiyigali-0.0.8/PKG-INFO` & `utils_cv-baiyigali-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utils_cv-baiyigali
-Version: 0.0.8
+Version: 0.0.9
 Summary: A small example package
 Home-page: https://github.com/pypa/sampleproject
 Author: baiyigali
 Author-email: 1304646911@qq.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Description: # Example Package
```

### Comparing `utils_cv-baiyigali-0.0.8/src/utils_cv/utils_box.py` & `utils_cv-baiyigali-0.0.9/src/utils_cv/utils_box.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,56 +1,64 @@
 import numpy as np
 
+
 def get_area(box):
-    area = (box[2]-box[0]+1) * (box[3]-box[1]+1)
+    area = (box[2] - box[0] + 1) * (box[3] - box[1] + 1)
     return area
 
+
 def get_iou(box1, box2):
     box1 = np.array(box1)
     box2 = np.array(box2)
 
     area1 = get_area(box1)
     area2 = get_area(box2)
 
     x1 = max(box1[0], box2[0])
     y1 = max(box1[1], box2[1])
     x2 = min(box1[2], box2[2])
     y2 = min(box1[3], box2[3])
-    area_inter = get_area([x1, y1, x2, y2])
+    if x1 <= x2 and y1 <= y2:
+        area_inter = get_area([x1, y1, x2, y2])
+    else:
+        area_inter = 0
 
-    area_union = area1+area2-area_inter
+    area_union = area1 + area2 - area_inter
 
     return area_inter / area_union
 
-def get_match_num(boxes1, boxes2, iou_thresh=0.8):    
+
+def get_match_num(boxes1, boxes2, iou_thresh=0.8):
     boxes1 = np.array(boxes1, dtype=np.float32).reshape([-1, 4]).tolist()
     boxes2 = np.array(boxes2, dtype=np.float32).reshape([-1, 4]).tolist()
     boxes1 = sorted(boxes1, key=lambda x: get_area(x))
     boxes2 = sorted(boxes2, key=lambda x: get_area(x))
 
     match_n = 0
-    while len(boxes1)>0 and len(boxes2)>0:
+    while len(boxes1) > 0 and len(boxes2) > 0:
         box1 = boxes1.pop(0)
-        j=0
-        while len(boxes2)>j:
+        j = 0
+        while len(boxes2) > j:
             if get_iou(box1, boxes2[j]) > iou_thresh:
                 boxes2.pop(j)
-                match_n+=1
+                match_n += 1
                 break
-            j+=1
+            j += 1
 
     return match_n
 
+
 def get_prf(boxes_gt, boxes_pd, iou_thresh=0.5):
     match_n = get_match_num(boxes_gt, boxes_pd)
-    precision_ = match_n/len(boxes_pd)
-    recall_ = match_n/len(boxes_gt)
-    fmeasure_ = precision_ * recall_ * 2 / (precision_ + recall_ )
+    precision_ = match_n / len(boxes_pd)
+    recall_ = match_n / len(boxes_gt)
+    fmeasure_ = precision_ * recall_ * 2 / (precision_ + recall_)
     return precision_, recall_, fmeasure_
 
+
 # def get_match_num(gt, pred, iou_thresh=0.8):
 #     gt = np.array(gt, dtype=np.float32).reshape([-1, 4])
 #     pred = np.array(pred, dtype=np.float32).reshape([-1, 4])
 #     gt_idxs = list(range(len(gt)))
 #     pd_idxs = list(range(len(pred)))
 #     iou_matrix = get_iou_matrix(gt, pred)
 
@@ -62,48 +70,53 @@
 #             if iou_matrix[i, pd_idxs[j]]>iou_thresh:
 #                 pd_idxs.pop(j)
 #                 num_tp+=1
 #                 break
 #             j+=1
 #     return num_tp
 
+
 def get_iou_matrix(boxes1, boxes2):
     boxes1 = np.array(boxes1, dtype=np.float32).reshape([-1, 4])
     boxes2 = np.array(boxes2, dtype=np.float32).reshape([-1, 4])
-    if len(boxes1) == 0 or len(boxes2)==0:
-        return np.zeros([len(boxes1),len(boxes2)])
-    boxes1_area = (boxes1[:, 2]-boxes1[:, 0]) * (boxes1[:, 3]-boxes1[:, 1])
-    boxes2_area = (boxes2[:, 2]-boxes2[:, 0]) * (boxes2[:, 3]-boxes2[:, 1])
+    if len(boxes1) == 0 or len(boxes2) == 0:
+        return np.zeros([len(boxes1), len(boxes2)])
+    boxes1_area = (boxes1[:, 2] - boxes1[:, 0]) * (boxes1[:, 3] - boxes1[:, 1])
+    boxes2_area = (boxes2[:, 2] - boxes2[:, 0]) * (boxes2[:, 3] - boxes2[:, 1])
     inter_x1 = np.maximum(boxes1[:, 0].reshape([-1, 1]), boxes2[:, 0])
     inter_x2 = np.minimum(boxes1[:, 2].reshape([-1, 1]), boxes2[:, 2])
     inter_y1 = np.maximum(boxes1[:, 1].reshape([-1, 1]), boxes2[:, 1])
     inter_y2 = np.minimum(boxes1[:, 3].reshape([-1, 1]), boxes2[:, 3])
-    inter_w = (inter_x2 - inter_x1)
+    inter_w = inter_x2 - inter_x1
     inter_w = np.clip(inter_w, 0, inter_w.max())
-    inter_h = (inter_y2 - inter_y1)
+    inter_h = inter_y2 - inter_y1
     inter_h = np.clip(inter_h, 0, inter_h.max())
     inter_area = inter_w * inter_h
     union_area = (boxes1_area.reshape([-1, 1]) + boxes2_area) - inter_area
     iou_matrix = inter_area / union_area
     return iou_matrix
 
+
 def box2poly(box):
     x1, y1, x2, y2 = box
     poly = [x1, y1, x2, y1, x2, y2, x1, y2]
     return poly
 
+
 def poly2box(poly):
     poly = np.reshape(poly, [-1, 2])
     box = np.concatenate([np.min(poly, axis=0), np.max(poly, axis=0)])
     return box
 
+
 def boxes2bbox(boxes):
     boxes = np.array(boxes).reshape([-1, 2])
     return poly2box(boxes)
 
+
 def nms(dets, scores, thresh):
     dets = np.array(dets).reshape([-1, 4])
     scores = np.array(scores).reshape([-1])
     x1 = dets[:, 0]
     y1 = dets[:, 1]
     x2 = dets[:, 2]
     y2 = dets[:, 3]
```

### Comparing `utils_cv-baiyigali-0.0.8/src/utils_cv/utils_layout.py` & `utils_cv-baiyigali-0.0.9/src/utils_cv/utils_layout.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 import numpy as np
 from .utils_box import boxes2bbox
 
+
 class TextLineCfg:
     MAX_HORIZONTAL_GAP_REL = 3
     HORIZONTAL_OVERLAP_MARGIN_REL = 1
     MIN_V_OVERLAPS = 0.4
     MIN_SIZE_SIM = 0.4
 
 
@@ -110,9 +111,9 @@
         return: line_boxes_index, line_boxes, line_bbox
         line_boxes_index: [idxs, idxs]
         line_boxes:[boxes, boxes]
         line_boxes_bbox: [box, box]
         """
         line_boxes_index = self.get_line_boxes_index()
         line_boxes = list(self.text_proposals[sg] for sg in line_boxes_index)
-        line_boxes_bbox =  list(boxes2bbox(box) for box in line_boxes)
+        line_boxes_bbox = list(boxes2bbox(box) for box in line_boxes)
         return line_boxes_index, line_boxes, line_boxes_bbox
```

### Comparing `utils_cv-baiyigali-0.0.8/src/utils_cv_baiyigali.egg-info/PKG-INFO` & `utils_cv-baiyigali-0.0.9/src/utils_cv_baiyigali.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utils-cv-baiyigali
-Version: 0.0.8
+Version: 0.0.9
 Summary: A small example package
 Home-page: https://github.com/pypa/sampleproject
 Author: baiyigali
 Author-email: 1304646911@qq.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Description: # Example Package
```

