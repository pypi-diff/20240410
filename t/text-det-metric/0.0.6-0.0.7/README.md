# Comparing `tmp/text_det_metric-0.0.6-py3-none-any.whl.zip` & `tmp/text_det_metric-0.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 9691 bytes, number of entries: 8
--rw-r--r--  2.0 unx      151 b- defN 23-Aug-26 08:12 text_det_metric/__init__.py
--rw-r--r--  2.0 unx     7467 b- defN 23-Aug-26 08:12 text_det_metric/main.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Aug-26 08:12 text_det_metric-0.0.6.dist-info/LICENSE
--rw-r--r--  2.0 unx     4318 b- defN 23-Aug-26 08:12 text_det_metric-0.0.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Aug-26 08:12 text_det_metric-0.0.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       63 b- defN 23-Aug-26 08:12 text_det_metric-0.0.6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       16 b- defN 23-Aug-26 08:12 text_det_metric-0.0.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      693 b- defN 23-Aug-26 08:12 text_det_metric-0.0.6.dist-info/RECORD
-8 files, 24157 bytes uncompressed, 8467 bytes compressed:  65.0%
+Zip file size: 9695 bytes, number of entries: 8
+-rw-r--r--  2.0 unx      151 b- defN 24-Apr-10 02:07 text_det_metric/__init__.py
+-rw-r--r--  2.0 unx     7734 b- defN 24-Apr-10 02:07 text_det_metric/main.py
+-rw-r--r--  2.0 unx    11357 b- defN 24-Apr-10 02:07 text_det_metric-0.0.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4342 b- defN 24-Apr-10 02:07 text_det_metric-0.0.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-10 02:07 text_det_metric-0.0.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       63 b- defN 24-Apr-10 02:07 text_det_metric-0.0.7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       16 b- defN 24-Apr-10 02:07 text_det_metric-0.0.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      693 b- defN 24-Apr-10 02:07 text_det_metric-0.0.7.dist-info/RECORD
+8 files, 24448 bytes uncompressed, 8471 bytes compressed:  65.4%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: text_det_metric/__init__.py
 Comment: 
 
 Filename: text_det_metric/main.py
 Comment: 
 
-Filename: text_det_metric-0.0.6.dist-info/LICENSE
+Filename: text_det_metric-0.0.7.dist-info/LICENSE
 Comment: 
 
-Filename: text_det_metric-0.0.6.dist-info/METADATA
+Filename: text_det_metric-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: text_det_metric-0.0.6.dist-info/WHEEL
+Filename: text_det_metric-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: text_det_metric-0.0.6.dist-info/entry_points.txt
+Filename: text_det_metric-0.0.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: text_det_metric-0.0.6.dist-info/top_level.txt
+Filename: text_det_metric-0.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: text_det_metric-0.0.6.dist-info/RECORD
+Filename: text_det_metric-0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## text_det_metric/main.py

```diff
@@ -1,57 +1,64 @@
 # -*- encoding: utf-8 -*-
 # @Author: SWHL
 # @Contact: liekkaskono@163.com
 import argparse
 import ast
+import copy
 import json
-from pathlib import Path
 from typing import Dict, List, Tuple
 
 from shapely.geometry import Polygon
 
 
 class DetectionIoUEvaluator:
     def __init__(self, iou_constraint=0.5, area_precision_constraint=0.5):
         self.iou_constraint = iou_constraint
         self.area_precision_constraint = area_precision_constraint
 
     def __call__(self, pred_txt_path: str):
-        preds, img_list, elapses = self.read_pred_txt(pred_txt_path)
-        gts = self.read_gts(img_list)
+        preds, gts, elapses = self.read_pred_txt(pred_txt_path)
 
         results = []
         for gt, pred in zip(gts, preds):
             results.append(self.evaluate_image(gt, pred))
 
         avg_elapse = sum(elapses) / len(elapses)
         metrics = self.combine_results(results)
-        metrics['avg_elapse'] = avg_elapse
+        metrics["avg_elapse"] = avg_elapse
         return metrics
 
     def read_pred_txt(self, txt_path: str) -> Tuple[List, List]:
-        preds, image_list, elapses = [], [], []
+        pred_boxes, gt_boxes, elapses = [], [], []
         datas = self.read_txt(txt_path)
         for data in datas:
-            image_path, dt_boxes, elapse = data.split("\t")
-            image_list.append(image_path)
-            dt_boxes = ast.literal_eval(dt_boxes)
-            result = [{"points": p, "text": "", "ignore": False} for p in dt_boxes]
-            preds.append(result)
+            cur_pred_boxes, cur_gt_boxes, elapse = data.split("\t")
+            cur_pred_boxes = ast.literal_eval(cur_pred_boxes)
+            cur_pred_boxes = [
+                {"points": p, "text": "", "ignore": False} for p in cur_pred_boxes
+            ]
+            pred_boxes.append(cur_pred_boxes)
+
+            cur_gt_boxes = ast.literal_eval(cur_gt_boxes)
+            tmp_gt_boxes = copy.deepcopy(cur_gt_boxes)
+            for i, points in enumerate(tmp_gt_boxes):
+                if len(points) == 2:
+                    x0, y0 = points[0]
+                    x1, y1 = points[1]
+
+                    points = [[x0, y0], [x1, y0], [x1, y1], [x0, y1]]
+                cur_gt_boxes[i] = points
+
+            cur_gt_boxes = [
+                {"points": p, "text": "", "ignore": False} for p in cur_gt_boxes
+            ]
+            gt_boxes.append(cur_gt_boxes)
 
             elapses.append(float(elapse))
-        return preds, image_list, elapses
-
-    def read_gts(self, image_list: List) -> List[List[Dict]]:
-        gts = []
-        for image_path in image_list:
-            json_path = Path(image_path).with_suffix(".json")
-            gt = self.parse_single_gt(str(json_path))
-            gts.append(gt)
-        return gts
+        return pred_boxes, gt_boxes, elapses
 
     @staticmethod
     def parse_single_gt(json_path: str) -> List[Dict]:
         with open(json_path, "r", encoding="utf-8") as f:
             data = json.load(f)
 
         result = []
```

## Comparing `text_det_metric-0.0.6.dist-info/LICENSE` & `text_det_metric-0.0.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `text_det_metric-0.0.6.dist-info/METADATA` & `text_det_metric-0.0.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text-det-metric
-Version: 0.0.6
+Version: 0.0.7
 Summary: Tool of computing the metric of text detection
 Home-page: https://github.com/SWHL/TextDetMetric
 Author: SWHL
 Author-email: liekkaskono@163.com
 License: Apache-2.0
 Keywords: ocr, text-det, hmean
 Platform: Any
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6,<3.12
 Description-Content-Type: text/markdown
 Requires-Dist: Shapely
+Requires-Dist: datasets
 
 ## Text Detect Metric
 <p align="left">
      <a href=""><img src="https://img.shields.io/badge/OS-Linux%2C%20Win%2C%20Mac-pink.svg"></a>
      <a href=""><img src="https://img.shields.io/badge/python->=3.6,<3.12-aff.svg"></a>
      <a href="https://pypi.org/project/text_det_metric/"><img alt="PyPI" src="https://img.shields.io/pypi/v/text_det_metric"></a>
      <a href="https://pepy.tech/project/text_det_metric"><img src="https://static.pepy.tech/personalized-badge/text_det_metric?period=total&units=abbreviation&left_color=grey&right_color=blue&left_text=Downloads "></a>
```

## Comparing `text_det_metric-0.0.6.dist-info/RECORD` & `text_det_metric-0.0.7.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 text_det_metric/__init__.py,sha256=K1TeK28y90XdOksdLCixf5d--5KXgzpsD1s6108yA1g,151
-text_det_metric/main.py,sha256=XVqYJjYvVoUiE0csh9_rrEoABLH0QVqbQ_hfRxBiNII,7467
-text_det_metric-0.0.6.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-text_det_metric-0.0.6.dist-info/METADATA,sha256=_Kb4JJkjdLJOFaeuQHLiyL0OIg3UagBNRBXU3R17a9Q,4318
-text_det_metric-0.0.6.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-text_det_metric-0.0.6.dist-info/entry_points.txt,sha256=gTbVodddXRR93pLeNRW5XXLwlzkYEB295t8Iy1e-N7Y,63
-text_det_metric-0.0.6.dist-info/top_level.txt,sha256=7olohGvTTeSsVHraNv5VoQm1nFkIT3GS3qWCl_Eamoc,16
-text_det_metric-0.0.6.dist-info/RECORD,,
+text_det_metric/main.py,sha256=gp-dmHTOuo8nz17pcI6OkNd3B9XjQNlwUSdlkYXojuQ,7734
+text_det_metric-0.0.7.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+text_det_metric-0.0.7.dist-info/METADATA,sha256=-lOoAO3o3nYlTVJCiD-Sgh2fLHqZ9vRhY-wQTLTE6cM,4342
+text_det_metric-0.0.7.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+text_det_metric-0.0.7.dist-info/entry_points.txt,sha256=gTbVodddXRR93pLeNRW5XXLwlzkYEB295t8Iy1e-N7Y,63
+text_det_metric-0.0.7.dist-info/top_level.txt,sha256=7olohGvTTeSsVHraNv5VoQm1nFkIT3GS3qWCl_Eamoc,16
+text_det_metric-0.0.7.dist-info/RECORD,,
```

