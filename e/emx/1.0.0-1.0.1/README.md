# Comparing `tmp/emx-1.0.0-py3-none-any.whl.zip` & `tmp/emx-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 7073 bytes, number of entries: 8
--rw-r--r--  2.0 unx    19116 b- defN 24-Apr-10 11:38 emx/__init__.py
+Zip file size: 7078 bytes, number of entries: 8
+-rw-r--r--  2.0 unx    19117 b- defN 24-Apr-10 11:54 emx/__init__.py
 -rw-r--r--  2.0 unx      239 b- defN 24-Apr-10 11:34 emx/__main__.py
 -rw-r--r--  2.0 unx     2320 b- defN 24-Apr-10 08:57 emx/http.py
--rw-r--r--  2.0 unx      310 b- defN 24-Apr-10 11:47 emx-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-10 11:47 emx-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       67 b- defN 24-Apr-10 11:47 emx-1.0.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        4 b- defN 24-Apr-10 11:47 emx-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      583 b- defN 24-Apr-10 11:47 emx-1.0.0.dist-info/RECORD
-8 files, 22731 bytes uncompressed, 6065 bytes compressed:  73.3%
+-rw-r--r--  2.0 unx      310 b- defN 24-Apr-10 12:02 emx-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-10 12:02 emx-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       67 b- defN 24-Apr-10 12:02 emx-1.0.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        4 b- defN 24-Apr-10 12:02 emx-1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      583 b- defN 24-Apr-10 12:02 emx-1.0.1.dist-info/RECORD
+8 files, 22732 bytes uncompressed, 6070 bytes compressed:  73.3%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: emx/__main__.py
 Comment: 
 
 Filename: emx/http.py
 Comment: 
 
-Filename: emx-1.0.0.dist-info/METADATA
+Filename: emx-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: emx-1.0.0.dist-info/WHEEL
+Filename: emx-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: emx-1.0.0.dist-info/entry_points.txt
+Filename: emx-1.0.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: emx-1.0.0.dist-info/top_level.txt
+Filename: emx-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: emx-1.0.0.dist-info/RECORD
+Filename: emx-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## emx/__init__.py

```diff
@@ -369,15 +369,15 @@
                 fp.write(data)
                 fp.seek(0)
                 os.system(f"bash \"{fp.name}\" {remargs_string}")
         elif file_type == "python":
             with tempfile.NamedTemporaryFile() as fp:
                 fp.write(data)
                 fp.seek(0)
-                os.system(f"python \"{fp.name}\" {remargs_string}")
+                os.system(f"python3 \"{fp.name}\" {remargs_string}")
 
     def config(self, args : argparse.Namespace):
         if args.name == "user":
             value = args.value
             if not value.encode("utf-8").isalnum():
                 print(f"An invalid username is entered. Only [a-zA-Z0-9] can be passed.")
                 return False
```

