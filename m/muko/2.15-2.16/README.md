# Comparing `tmp/muko-2.15-py3-none-any.whl.zip` & `tmp/muko-2.16-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,11 @@
-Zip file size: 1587684 bytes, number of entries: 7
--rw-r--r--  2.0 fat       20 b- defN 80-Jan-01 00:00 muko/__init__.py
--rw-r--r--  2.0 fat   355840 b- defN 80-Jan-01 00:00 muko/cmuko.cp38-win_amd64.pyd
--rw-r--r--  2.0 fat  2082964 b- defN 80-Jan-01 00:00 muko/font/default.otf
--rw-r--r--  2.0 fat     1074 b- defN 80-Jan-01 00:00 muko-2.15.dist-info/LICENSE
--rw-r--r--  2.0 fat     1058 b- defN 80-Jan-01 00:00 muko-2.15.dist-info/METADATA
--rw-r--r--  2.0 fat       88 b- defN 80-Jan-01 00:00 muko-2.15.dist-info/WHEEL
-?rw-r--r--  2.0 fat      518 b- defN 16-Jan-01 00:00 muko-2.15.dist-info/RECORD
-7 files, 2441562 bytes uncompressed, 1586786 bytes compressed:  35.0%
+Zip file size: 1628746 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat       20 b- defN 24-Mar-13 17:30 muko/__init__.py
+-rw-rw-rw-  2.0 fat   462336 b- defN 24-Apr-10 01:53 muko/cmuko.cp38-win_amd64.pyd
+-rw-rw-rw-  2.0 fat  2082964 b- defN 24-Feb-08 07:11 muko/font/default.otf
+-rw-rw-rw-  2.0 fat     1074 b- defN 24-Apr-10 01:53 muko-2.16.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1179 b- defN 24-Apr-10 01:53 muko-2.16.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-10 01:53 muko-2.16.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       20 b- defN 24-Apr-10 01:53 muko-2.16.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        5 b- defN 24-Apr-10 01:53 muko-2.16.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      696 b- defN 24-Apr-10 01:53 muko-2.16.dist-info/RECORD
+9 files, 2548386 bytes uncompressed, 1627558 bytes compressed:  36.1%
```

## zipnote {}

```diff
@@ -3,20 +3,26 @@
 
 Filename: muko/cmuko.cp38-win_amd64.pyd
 Comment: 
 
 Filename: muko/font/default.otf
 Comment: 
 
-Filename: muko-2.15.dist-info/LICENSE
+Filename: muko-2.16.dist-info/LICENSE
 Comment: 
 
-Filename: muko-2.15.dist-info/METADATA
+Filename: muko-2.16.dist-info/METADATA
 Comment: 
 
-Filename: muko-2.15.dist-info/WHEEL
+Filename: muko-2.16.dist-info/WHEEL
 Comment: 
 
-Filename: muko-2.15.dist-info/RECORD
+Filename: muko-2.16.dist-info/entry_points.txt
+Comment: 
+
+Filename: muko-2.16.dist-info/top_level.txt
+Comment: 
+
+Filename: muko-2.16.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `muko-2.15.dist-info/LICENSE` & `muko-2.16.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `muko-2.15.dist-info/METADATA` & `muko-2.16.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,43 @@
-Metadata-Version: 2.1
-Name: muko
-Version: 2.15
-Summary: 加速实现AIGC、自动办公的中文编程工具
-Home-page: https://www.mikooo.cn
-License: MIT
-Author: Milk
-Author-email: 719496375@qq.com
-Requires-Python: ==3.8.*
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Requires-Dist: diskcache (>=5.6.3)
-Requires-Dist: moviepy (>=1.0.3)
-Requires-Dist: numpy (>=1.24.4)
-Requires-Dist: opencv-python (>=4.9.0.80)
-Requires-Dist: pillow (==9.5.0)
-Requires-Dist: requests (>=2.31.0)
-Requires-Dist: retrying (>=1.3.3)
-Description-Content-Type: text/markdown
-
-# Muko：加速实现AIGC、自动办公的中文编程工具
-
-## 安装方式
-    pip install muko
-
-## 使用方法
-在你的代码文件开头添加以下这句，就可以获得Muko的所有能力
-
-    from muko import *
-
-## 输出文本到控制台（入门）
-    输出('凡事发生皆有利于我')
-
-## AI朗读
-自动将文本生成wav音频文件
-
-    朗读('凡事发生皆有利于我')
-
+Metadata-Version: 2.1
+Name: muko
+Version: 2.16
+Summary: 加速实现AIGC、自动办公的中文编程工具
+Home-page: https://www.mikooo.cn
+Author: Milk
+Author-email: 719496375@qq.com
+License: The MIT License
+Platform: win64
+Classifier: Programming Language :: Python :: 3.8
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Microsoft :: Windows
+Requires-Python: ==3.8
+Description-Content-Type: text/markdown
+Requires-Dist: requests >=2.31.0
+Requires-Dist: moviepy >=1.0.3
+Requires-Dist: pillow ==9.5.0
+Requires-Dist: diskcache >=5.6.3
+Requires-Dist: retrying >=1.3.3
+Requires-Dist: numpy >=1.24.4
+Requires-Dist: opencv-python >=4.9.0.80
+Requires-Dist: diplib >=3.4.3
+Requires-Dist: rembg >=2.0.56
+
+# Muko：加速实现AIGC、自动办公的中文编程工具
+
+## 安装方式
+    pip install muko
+
+## 使用方法
+在你的代码文件开头添加以下这句，就可以获得Muko的所有能力
+
+    from muko import *
+
+## 输出文本到控制台（入门）
+    输出('凡事发生皆有利于我')
+
+## AI朗读
+自动将文本生成wav音频文件
+
+    朗读('凡事发生皆有利于我')
+
+
```

