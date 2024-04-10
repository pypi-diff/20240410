# Comparing `tmp/NetworkXsimple-0.1.3-py3-none-any.whl.zip` & `tmp/NetworkXsimple-0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 9403 bytes, number of entries: 8
+Zip file size: 9383 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat       20 b- defN 24-Apr-09 17:46 package_xskj_NetworkXsimple/__init__.py
 -rw-rw-rw-  2.0 fat      352 b- defN 24-Apr-09 17:46 package_xskj_NetworkXsimple/__version__.py
 -rw-rw-rw-  2.0 fat     7767 b- defN 24-Apr-10 07:36 package_xskj_NetworkXsimple/core.py
--rw-rw-rw-  2.0 fat    11357 b- defN 24-Apr-10 07:41 NetworkXsimple-0.1.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3123 b- defN 24-Apr-10 07:41 NetworkXsimple-0.1.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-10 07:41 NetworkXsimple-0.1.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       28 b- defN 24-Apr-10 07:41 NetworkXsimple-0.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      706 b- defN 24-Apr-10 07:41 NetworkXsimple-0.1.3.dist-info/RECORD
-8 files, 23445 bytes uncompressed, 8153 bytes compressed:  65.2%
+-rw-rw-rw-  2.0 fat    11357 b- defN 24-Apr-10 08:41 NetworkXsimple-0.1.4.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3269 b- defN 24-Apr-10 08:41 NetworkXsimple-0.1.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-10 08:41 NetworkXsimple-0.1.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       28 b- defN 24-Apr-10 08:41 NetworkXsimple-0.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      706 b- defN 24-Apr-10 08:41 NetworkXsimple-0.1.4.dist-info/RECORD
+8 files, 23591 bytes uncompressed, 8133 bytes compressed:  65.5%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: package_xskj_NetworkXsimple/__version__.py
 Comment: 
 
 Filename: package_xskj_NetworkXsimple/core.py
 Comment: 
 
-Filename: NetworkXsimple-0.1.3.dist-info/LICENSE
+Filename: NetworkXsimple-0.1.4.dist-info/LICENSE
 Comment: 
 
-Filename: NetworkXsimple-0.1.3.dist-info/METADATA
+Filename: NetworkXsimple-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: NetworkXsimple-0.1.3.dist-info/WHEEL
+Filename: NetworkXsimple-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: NetworkXsimple-0.1.3.dist-info/top_level.txt
+Filename: NetworkXsimple-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: NetworkXsimple-0.1.3.dist-info/RECORD
+Filename: NetworkXsimple-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `NetworkXsimple-0.1.3.dist-info/LICENSE` & `NetworkXsimple-0.1.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `NetworkXsimple-0.1.3.dist-info/METADATA` & `NetworkXsimple-0.1.4.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NetworkXsimple
-Version: 0.1.3
+Version: 0.1.4
 Summary: This is a simple encapsulation for networkX, which further simplifies the process of networkX for drawing neural network diagrams, so that the author can only focus on the logical writing of neural networks, without spending time on the visual presentation of neural networks. At the same time, this module also inherits all the methods of network and does not affect the normal function calls of networkX.
 Home-page: https://github.com/gnu-xiaosong/networkXsimple.git
 Author: xskj
 Author-email: 1829134124@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -25,22 +25,32 @@
 `
 pip install NetworkXsimple
 `
 # guid
 
 ### api
 ```python
-graph.addNode(name="node name", desc="node A desc", pos=(int layer, int node No. in this layer) , nexts=[
+graph.addNode(
+    name="node name",
+    pos=(int layer, int node No)  ,
+    nexts=[
     {
-        "node": "B",
-        "label":"B"
-    },
-    previous=[]
-])
+        "node": "G",
+        "label":"edge label"
+    }],
+    previous=[
+        {
+            "node": "G",
+            "label": "edge label G"
+        }
+    ],
+    label="AAAAA",
+    label_color="pink")
 ```
+![img.png](img.png)
 * nexts : output degress   dict
 * previous : input degress  dict
 ``
  {
         "node": "next node name",
         "label":"edge desc"
     }
```

## Comparing `NetworkXsimple-0.1.3.dist-info/RECORD` & `NetworkXsimple-0.1.4.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 package_xskj_NetworkXsimple/__init__.py,sha256=K0kNy26Vm6A-1V5lST3ily6yVsNLUbiqk6AZDFm2nJI,20
 package_xskj_NetworkXsimple/__version__.py,sha256=MobQVtrO9Ze27biO6l6QreTAONnDTqbALI54Q1gpCI8,352
 package_xskj_NetworkXsimple/core.py,sha256=J2N_DpqIRecFJg4_kZ4XceJV7zf8bAW33qKsohLBHiU,7767
-NetworkXsimple-0.1.3.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-NetworkXsimple-0.1.3.dist-info/METADATA,sha256=fXmYfmb7pbj30RNPs7h2q7RwOXIC-KjuKPG_9MMQdUI,3123
-NetworkXsimple-0.1.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-NetworkXsimple-0.1.3.dist-info/top_level.txt,sha256=loTHGhQs_kDS22SI4mDhjw5gUdIZ3cat36pif79VyG8,28
-NetworkXsimple-0.1.3.dist-info/RECORD,,
+NetworkXsimple-0.1.4.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+NetworkXsimple-0.1.4.dist-info/METADATA,sha256=DTuvENZTTBgrngGpnGA-tlTX9u8Qoey0wcVBX9JMwS8,3269
+NetworkXsimple-0.1.4.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+NetworkXsimple-0.1.4.dist-info/top_level.txt,sha256=loTHGhQs_kDS22SI4mDhjw5gUdIZ3cat36pif79VyG8,28
+NetworkXsimple-0.1.4.dist-info/RECORD,,
```

