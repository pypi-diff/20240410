# Comparing `tmp/emx-1.0.2-py3-none-any.whl.zip` & `tmp/emx-1.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 7074 bytes, number of entries: 8
--rw-r--r--  2.0 unx    19172 b- defN 24-Apr-10 12:05 emx/__init__.py
+Zip file size: 7050 bytes, number of entries: 8
+-rw-r--r--  2.0 unx    19044 b- defN 24-Apr-10 14:22 emx/__init__.py
 -rw-r--r--  2.0 unx      239 b- defN 24-Apr-10 11:34 emx/__main__.py
 -rw-r--r--  2.0 unx     2320 b- defN 24-Apr-10 08:57 emx/http.py
--rw-r--r--  2.0 unx      310 b- defN 24-Apr-10 12:07 emx-1.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-10 12:07 emx-1.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       67 b- defN 24-Apr-10 12:07 emx-1.0.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        4 b- defN 24-Apr-10 12:07 emx-1.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      583 b- defN 24-Apr-10 12:07 emx-1.0.2.dist-info/RECORD
-8 files, 22787 bytes uncompressed, 6066 bytes compressed:  73.4%
+-rw-r--r--  2.0 unx      310 b- defN 24-Apr-10 14:23 emx-1.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-10 14:23 emx-1.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       67 b- defN 24-Apr-10 14:23 emx-1.0.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        4 b- defN 24-Apr-10 14:23 emx-1.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      583 b- defN 24-Apr-10 14:23 emx-1.0.3.dist-info/RECORD
+8 files, 22659 bytes uncompressed, 6042 bytes compressed:  73.3%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: emx/__main__.py
 Comment: 
 
 Filename: emx/http.py
 Comment: 
 
-Filename: emx-1.0.2.dist-info/METADATA
+Filename: emx-1.0.3.dist-info/METADATA
 Comment: 
 
-Filename: emx-1.0.2.dist-info/WHEEL
+Filename: emx-1.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: emx-1.0.2.dist-info/entry_points.txt
+Filename: emx-1.0.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: emx-1.0.2.dist-info/top_level.txt
+Filename: emx-1.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: emx-1.0.2.dist-info/RECORD
+Filename: emx-1.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## emx/__init__.py

```diff
@@ -181,19 +181,18 @@
         
         files = resp["files"]
         print(f"Found {len(files)} files by {key}:")
         for i, file in enumerate(files):
             path = file["path"]
             size = int(file["size"])
             desc = file["descript"]
-            idd = file["id"]
             if desc:
-                print(f"{idd}. {path} [{format_size(size)}]: {desc}")
+                print(f"{i}. {path} [{format_size(size)}]: {desc}")
             else:
-                print(f"{idd}. {path} [{format_size(size)}]")
+                print(f"{i}. {path} [{format_size(size)}]")
 
     def cmds(self, args : argparse.Namespace):
         key = args.key
         show_count = args.count
         show_skip  = args.skip
 
         req_args = urlencode({
@@ -211,19 +210,18 @@
         
         files = resp["files"]
         print(f"Found {len(files)} files by {key}:")
         for i, file in enumerate(files):
             path = file["path"]
             size = int(file["size"])
             desc = file["descript"]
-            idd = file["id"]
             if desc:
-                print(f"{idd}. {path} [{format_size(size)}]: {desc}")
+                print(f"{i}. {path} [{format_size(size)}]: {desc}")
             else:
-                print(f"{idd}. {path} [{format_size(size)}]")
+                print(f"{i}. {path} [{format_size(size)}]")
 
     def info(self, args : argparse.Namespace):
         name = args.name
         isid = args.id
 
         try:
             n = int(name)
@@ -496,16 +494,15 @@
                 "zipped": str(zipped),
                 "file_type": file_type,
                 "user_name": self.cfg.get_cfg("UserName")
             }
             resp = http.upload_file(f"{self.cfg.SERVER}/upload", local, headers, f"Upload: {remote}")
 
         if resp is not None:
-            file_id = resp["file_id"]
-            print(f"Complete to upload and you can use [file id: {file_id}] or [file name: {remote}] to view this file")
+            print(f"Complete to upload and you can use [file name: {remote}] to view this file")
 
 class Application:
     def __init__(self):
         self.cfg     = Config()
         self.actions = Actions(self)
 
     def run_with_command(self, args=None)->bool:
```

## Comparing `emx-1.0.2.dist-info/RECORD` & `emx-1.0.3.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-emx/__init__.py,sha256=wEe2rrXmZlX-GZnYgWbQCF8mjX5nHTiWDoCvUVrhUIQ,19172
+emx/__init__.py,sha256=zK2O9LCpEDhllTzCMLdS_8lMqnqVRD3HvPZf6wtCoBg,19044
 emx/__main__.py,sha256=vZwS8IKVqP_M9MaJM8AsdM93XvflohMpoLrnXYcqnpk,239
 emx/http.py,sha256=3uk3kfKvKPb8mRaykRkb0_dpwvKZBSIUOVWnM3kFbpQ,2320
-emx-1.0.2.dist-info/METADATA,sha256=Al1FotIbHAa6imB42TE0LGPhg8sPifV0dzNArbPdqVE,310
-emx-1.0.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-emx-1.0.2.dist-info/entry_points.txt,sha256=Q4bfdmdN4hpNqKvXURVbkF8Q6KP0P9jykoccDI4GcI0,67
-emx-1.0.2.dist-info/top_level.txt,sha256=mAJdYxkuyZt_oZrtIM2mSBM2LadTIoXeo75v_-v-h5A,4
-emx-1.0.2.dist-info/RECORD,,
+emx-1.0.3.dist-info/METADATA,sha256=hHH-Sgu2jnUynAgqbuYDahR4CQaHfbHw7HjHTnUObAQ,310
+emx-1.0.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+emx-1.0.3.dist-info/entry_points.txt,sha256=Q4bfdmdN4hpNqKvXURVbkF8Q6KP0P9jykoccDI4GcI0,67
+emx-1.0.3.dist-info/top_level.txt,sha256=mAJdYxkuyZt_oZrtIM2mSBM2LadTIoXeo75v_-v-h5A,4
+emx-1.0.3.dist-info/RECORD,,
```

