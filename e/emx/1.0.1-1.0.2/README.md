# Comparing `tmp/emx-1.0.1-py3-none-any.whl.zip` & `tmp/emx-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 7078 bytes, number of entries: 8
--rw-r--r--  2.0 unx    19117 b- defN 24-Apr-10 11:54 emx/__init__.py
+Zip file size: 7074 bytes, number of entries: 8
+-rw-r--r--  2.0 unx    19172 b- defN 24-Apr-10 12:05 emx/__init__.py
 -rw-r--r--  2.0 unx      239 b- defN 24-Apr-10 11:34 emx/__main__.py
 -rw-r--r--  2.0 unx     2320 b- defN 24-Apr-10 08:57 emx/http.py
--rw-r--r--  2.0 unx      310 b- defN 24-Apr-10 12:02 emx-1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-10 12:02 emx-1.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       67 b- defN 24-Apr-10 12:02 emx-1.0.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        4 b- defN 24-Apr-10 12:02 emx-1.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      583 b- defN 24-Apr-10 12:02 emx-1.0.1.dist-info/RECORD
-8 files, 22732 bytes uncompressed, 6070 bytes compressed:  73.3%
+-rw-r--r--  2.0 unx      310 b- defN 24-Apr-10 12:07 emx-1.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-10 12:07 emx-1.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       67 b- defN 24-Apr-10 12:07 emx-1.0.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        4 b- defN 24-Apr-10 12:07 emx-1.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      583 b- defN 24-Apr-10 12:07 emx-1.0.2.dist-info/RECORD
+8 files, 22787 bytes uncompressed, 6066 bytes compressed:  73.4%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: emx/__main__.py
 Comment: 
 
 Filename: emx/http.py
 Comment: 
 
-Filename: emx-1.0.1.dist-info/METADATA
+Filename: emx-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: emx-1.0.1.dist-info/WHEEL
+Filename: emx-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: emx-1.0.1.dist-info/entry_points.txt
+Filename: emx-1.0.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: emx-1.0.1.dist-info/top_level.txt
+Filename: emx-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: emx-1.0.1.dist-info/RECORD
+Filename: emx-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## emx/__init__.py

```diff
@@ -197,15 +197,16 @@
         show_skip  = args.skip
 
         req_args = urlencode({
             "keyword": key, 
             "type": "name", 
             "show_count": show_count,
             "show_skip": show_skip,
-            "ftype": "cmds"
+            "ftype": "cmds",
+            "user_name": self.cfg.get_cfg("UserName")
         })
         
         resp = http.request_info(f"{self.cfg.SERVER}/search?{req_args}")
         if resp is None:
             return False
         
         files = resp["files"]
```

## Comparing `emx-1.0.1.dist-info/RECORD` & `emx-1.0.2.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-emx/__init__.py,sha256=qpjX3T-RR4TPtNudY87sNBhPSTHTAvmmBlb2Eh6Fsek,19117
+emx/__init__.py,sha256=wEe2rrXmZlX-GZnYgWbQCF8mjX5nHTiWDoCvUVrhUIQ,19172
 emx/__main__.py,sha256=vZwS8IKVqP_M9MaJM8AsdM93XvflohMpoLrnXYcqnpk,239
 emx/http.py,sha256=3uk3kfKvKPb8mRaykRkb0_dpwvKZBSIUOVWnM3kFbpQ,2320
-emx-1.0.1.dist-info/METADATA,sha256=X3SqLtrhvQbheClzFk32uAXGv21s1qaAzsP-mC8UpgA,310
-emx-1.0.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-emx-1.0.1.dist-info/entry_points.txt,sha256=Q4bfdmdN4hpNqKvXURVbkF8Q6KP0P9jykoccDI4GcI0,67
-emx-1.0.1.dist-info/top_level.txt,sha256=mAJdYxkuyZt_oZrtIM2mSBM2LadTIoXeo75v_-v-h5A,4
-emx-1.0.1.dist-info/RECORD,,
+emx-1.0.2.dist-info/METADATA,sha256=Al1FotIbHAa6imB42TE0LGPhg8sPifV0dzNArbPdqVE,310
+emx-1.0.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+emx-1.0.2.dist-info/entry_points.txt,sha256=Q4bfdmdN4hpNqKvXURVbkF8Q6KP0P9jykoccDI4GcI0,67
+emx-1.0.2.dist-info/top_level.txt,sha256=mAJdYxkuyZt_oZrtIM2mSBM2LadTIoXeo75v_-v-h5A,4
+emx-1.0.2.dist-info/RECORD,,
```

