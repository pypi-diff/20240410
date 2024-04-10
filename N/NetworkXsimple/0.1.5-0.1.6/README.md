# Comparing `tmp/NetworkXsimple-0.1.5-py3-none-any.whl.zip` & `tmp/NetworkXsimple-0.1.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 9381 bytes, number of entries: 8
+Zip file size: 9483 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat       20 b- defN 24-Apr-09 17:46 package_xskj_NetworkXsimple/__init__.py
 -rw-rw-rw-  2.0 fat      352 b- defN 24-Apr-09 17:46 package_xskj_NetworkXsimple/__version__.py
--rw-rw-rw-  2.0 fat     7767 b- defN 24-Apr-10 07:36 package_xskj_NetworkXsimple/core.py
--rw-rw-rw-  2.0 fat    11357 b- defN 24-Apr-10 08:54 NetworkXsimple-0.1.5.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3269 b- defN 24-Apr-10 08:54 NetworkXsimple-0.1.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-10 08:54 NetworkXsimple-0.1.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       28 b- defN 24-Apr-10 08:54 NetworkXsimple-0.1.5.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      706 b- defN 24-Apr-10 08:54 NetworkXsimple-0.1.5.dist-info/RECORD
-8 files, 23591 bytes uncompressed, 8131 bytes compressed:  65.5%
+-rw-rw-rw-  2.0 fat     8181 b- defN 24-Apr-10 09:02 package_xskj_NetworkXsimple/core.py
+-rw-rw-rw-  2.0 fat    11357 b- defN 24-Apr-10 09:03 NetworkXsimple-0.1.6.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3269 b- defN 24-Apr-10 09:03 NetworkXsimple-0.1.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-10 09:03 NetworkXsimple-0.1.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       28 b- defN 24-Apr-10 09:03 NetworkXsimple-0.1.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      706 b- defN 24-Apr-10 09:03 NetworkXsimple-0.1.6.dist-info/RECORD
+8 files, 24005 bytes uncompressed, 8233 bytes compressed:  65.7%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: package_xskj_NetworkXsimple/__version__.py
 Comment: 
 
 Filename: package_xskj_NetworkXsimple/core.py
 Comment: 
 
-Filename: NetworkXsimple-0.1.5.dist-info/LICENSE
+Filename: NetworkXsimple-0.1.6.dist-info/LICENSE
 Comment: 
 
-Filename: NetworkXsimple-0.1.5.dist-info/METADATA
+Filename: NetworkXsimple-0.1.6.dist-info/METADATA
 Comment: 
 
-Filename: NetworkXsimple-0.1.5.dist-info/WHEEL
+Filename: NetworkXsimple-0.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: NetworkXsimple-0.1.5.dist-info/top_level.txt
+Filename: NetworkXsimple-0.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: NetworkXsimple-0.1.5.dist-info/RECORD
+Filename: NetworkXsimple-0.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## package_xskj_NetworkXsimple/core.py

```diff
@@ -32,40 +32,44 @@
 
         """
         degrees = []
         for item in previous:
             degrees.append({
                 "type": 0,  # 入度
                 "node": item["node"],
-                "label": item["label"],
-                "color": "green",
-                "weight": 1
+                "label": item["label"]   if item.has_key("label") else "",
+                "color": item["color"]   if item.has_key("color") else "black",
+                "weight": item["weight"] if item.has_key("weight") else 1
             })
 
         for item in nexts:
             degrees.append({
                 "type": 1,  # 出度
                 "node": item["node"],
-                "label": item["label"],
-                "color": "green",
-                "weight": 1
+                "label":  item["label"]   if item.has_key("label")   else "",
+                "color":  item["color"]   if item.has_key("color")   else "black",
+                "weight": item["weight"]  if item.has_key("weight") else 1
             })
 
         node = {
             "id": len(self.nodes_arr) + 1,
             "name": name,
             "label": label,
             "labelColor": label_color,
             "position": self.setPostion(pos),
             "degree": degrees
         }
 
+        # 判断是否重复设置了相同的node
+        if name  in self.pos:
+            print(f"node={name} alread exist!")
+            return None
+
         self.pos[name] = self.setPostion(pos)
         self.nodes_arr.append(node)
-
         # 增加层数： 判断是否存在layer数组中
         if pos[0] not in self.layers:
             self.layers.append(pos[0])
 
         # 数据类型转化
         self.netGraphToNetworkX()
```

## Comparing `NetworkXsimple-0.1.5.dist-info/LICENSE` & `NetworkXsimple-0.1.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `NetworkXsimple-0.1.5.dist-info/METADATA` & `NetworkXsimple-0.1.6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NetworkXsimple
-Version: 0.1.5
+Version: 0.1.6
 Summary: This is a simple encapsulation for networkX, which further simplifies the process of networkX for drawing neural network diagrams, so that the author can only focus on the logical writing of neural networks, without spending time on the visual presentation of neural networks. At the same time, this module also inherits all the methods of network and does not affect the normal function calls of networkX.
 Home-page: https://github.com/gnu-xiaosong/networkXsimple.git
 Author: xskj
 Author-email: 1829134124@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `NetworkXsimple-0.1.5.dist-info/RECORD` & `NetworkXsimple-0.1.6.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 package_xskj_NetworkXsimple/__init__.py,sha256=K0kNy26Vm6A-1V5lST3ily6yVsNLUbiqk6AZDFm2nJI,20
 package_xskj_NetworkXsimple/__version__.py,sha256=MobQVtrO9Ze27biO6l6QreTAONnDTqbALI54Q1gpCI8,352
-package_xskj_NetworkXsimple/core.py,sha256=J2N_DpqIRecFJg4_kZ4XceJV7zf8bAW33qKsohLBHiU,7767
-NetworkXsimple-0.1.5.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-NetworkXsimple-0.1.5.dist-info/METADATA,sha256=wsA0cy_VzvbtgRec7gXIVPNDhDPo-ISxZ7-qAlqK_-U,3269
-NetworkXsimple-0.1.5.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-NetworkXsimple-0.1.5.dist-info/top_level.txt,sha256=loTHGhQs_kDS22SI4mDhjw5gUdIZ3cat36pif79VyG8,28
-NetworkXsimple-0.1.5.dist-info/RECORD,,
+package_xskj_NetworkXsimple/core.py,sha256=7cpJTJshtEGGAfLXeBB4skgKG9tAaunVBzIfudzs3z8,8181
+NetworkXsimple-0.1.6.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+NetworkXsimple-0.1.6.dist-info/METADATA,sha256=dooyU22TUaH7P-ttl5xD7Gz6oDUTj3N5ZaDFXVE48o0,3269
+NetworkXsimple-0.1.6.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+NetworkXsimple-0.1.6.dist-info/top_level.txt,sha256=loTHGhQs_kDS22SI4mDhjw5gUdIZ3cat36pif79VyG8,28
+NetworkXsimple-0.1.6.dist-info/RECORD,,
```

