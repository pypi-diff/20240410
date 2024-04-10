# Comparing `tmp/mdrocr-3.tar.gz` & `tmp/mdrocr-5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdrocr-3.tar", last modified: Wed Mar 20 16:58:52 2024, max compression
+gzip compressed data, was "mdrocr-5.tar", last modified: Wed Apr 10 14:40:44 2024, max compression
```

## Comparing `mdrocr-3.tar` & `mdrocr-5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2024-03-20 16:58:52.975922 mdrocr-3/
--rw-rw-r--   0 j         (1000) j         (1000)       30 2024-03-20 16:50:35.000000 mdrocr-3/.gitignore
--rw-rw-r--   0 j         (1000) j         (1000)      458 2024-03-20 16:58:52.975922 mdrocr-3/PKG-INFO
--rw-rw-r--   0 j         (1000) j         (1000)       89 2024-03-20 16:55:05.000000 mdrocr-3/README.md
--rwxrwxr-x   0 j         (1000) j         (1000)     1879 2024-03-20 16:43:14.000000 mdrocr-3/mdrocr
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2024-03-20 16:58:52.975922 mdrocr-3/mdrocr.egg-info/
--rw-rw-r--   0 j         (1000) j         (1000)      458 2024-03-20 16:58:52.000000 mdrocr-3/mdrocr.egg-info/PKG-INFO
--rw-rw-r--   0 j         (1000) j         (1000)      167 2024-03-20 16:58:52.000000 mdrocr-3/mdrocr.egg-info/SOURCES.txt
--rw-rw-r--   0 j         (1000) j         (1000)        1 2024-03-20 16:58:52.000000 mdrocr-3/mdrocr.egg-info/dependency_links.txt
--rw-rw-r--   0 j         (1000) j         (1000)        1 2024-03-20 16:58:52.000000 mdrocr-3/mdrocr.egg-info/top_level.txt
--rwxr-xr-x   0 j         (1000) j         (1000)      291 2024-03-20 16:56:34.000000 mdrocr-3/release.sh
--rw-rw-r--   0 j         (1000) j         (1000)       38 2024-03-20 16:58:52.975922 mdrocr-3/setup.cfg
--rw-rw-r--   0 j         (1000) j         (1000)      924 2024-03-20 16:58:52.000000 mdrocr-3/setup.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2024-04-10 14:40:44.745209 mdrocr-5/
+-rw-rw-r--   0 j         (1000) j         (1000)       30 2024-03-20 16:50:35.000000 mdrocr-5/.gitignore
+-rw-rw-r--   0 j         (1000) j         (1000)      458 2024-04-10 14:40:44.745209 mdrocr-5/PKG-INFO
+-rw-rw-r--   0 j         (1000) j         (1000)       89 2024-03-20 16:55:05.000000 mdrocr-5/README.md
+-rwxrwxr-x   0 j         (1000) j         (1000)     2483 2024-04-10 14:39:36.000000 mdrocr-5/mdrocr
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2024-04-10 14:40:44.745209 mdrocr-5/mdrocr.egg-info/
+-rw-rw-r--   0 j         (1000) j         (1000)      458 2024-04-10 14:40:43.000000 mdrocr-5/mdrocr.egg-info/PKG-INFO
+-rw-rw-r--   0 j         (1000) j         (1000)      167 2024-04-10 14:40:44.000000 mdrocr-5/mdrocr.egg-info/SOURCES.txt
+-rw-rw-r--   0 j         (1000) j         (1000)        1 2024-04-10 14:40:43.000000 mdrocr-5/mdrocr.egg-info/dependency_links.txt
+-rw-rw-r--   0 j         (1000) j         (1000)        1 2024-04-10 14:40:43.000000 mdrocr-5/mdrocr.egg-info/top_level.txt
+-rwxr-xr-x   0 j         (1000) j         (1000)      291 2024-03-20 16:56:34.000000 mdrocr-5/release.sh
+-rw-rw-r--   0 j         (1000) j         (1000)       38 2024-04-10 14:40:44.745209 mdrocr-5/setup.cfg
+-rw-rw-r--   0 j         (1000) j         (1000)      924 2024-04-10 14:40:42.000000 mdrocr-5/setup.py
```

### Comparing `mdrocr-3/mdrocr` & `mdrocr-5/mdrocr`

 * *Files 15% similar despite different names*

```diff
@@ -11,48 +11,74 @@
 import os
 import re
 import shutil
 import subprocess
 import sys
 import tempfile
 
+
 def sorted_list(l):
     convert = lambda text: float(text) if text.isdigit() else text
-    alphanum = lambda key: [convert(c) for c in re.split('([-+]?[0-9]*\.?[0-9]*)', key)]
+    alphanum = lambda key: [
+        convert(c) for c in re.split(r"([-+]?[0-9]*\.?[0-9]*)", key)
+    ]
     l.sort(key=alphanum)
     return l
 
-parser = argparse.ArgumentParser(description='OCR folders of images')
-parser.add_argument('--lang', dest='lang', default="eng",
-                    help='language to use (default eng)')
-parser.add_argument('--dpi', dest='dpi', default="300",
-                    help='dpi of scan (default 300)')
-parser.add_argument('folder')
+
+def which(program):
+    for folder in os.environ["PATH"].split(":"):
+        p = os.path.join(folder, program)
+        if os.access(p, os.X_OK) and os.path.isfile(p):
+            return p
+    return None
+
+
+parser = argparse.ArgumentParser(description="OCR folders of images")
+parser.add_argument(
+    "--lang", dest="lang", default="eng", help="language to use (default eng)"
+)
+parser.add_argument(
+    "--dpi", dest="dpi", default="300", help="dpi of scan (default 300)"
+)
+parser.add_argument("folder")
 
 args = parser.parse_args()
 
 language = args.lang
 dpi = args.dpi
 base = os.path.normpath(os.path.abspath(args.folder))
 
+sips_installed = which("sips")
+
 for root, folders, files in os.walk(base):
     if not folders and files:
-        pdf = root + '.pdf'
+        pdf = root + ".pdf"
         if os.path.exists(pdf):
             print("\n--\nskip", root, "pdf exists", pdf)
             continue
-        images = sorted_list([f for f in files if f.split('.')[-1] in ('jpg', 'jp2', 'jpeg')])
+        images = sorted_list(
+            [f for f in files if f.split(".")[-1] in ("jpg", "jp2", "jpeg")]
+        )
         print("\n---\nprocessing %s\n%s pages\n" % (root, len(images)))
         tmp = tempfile.mkdtemp()
         pages = []
         for image in images:
             image = os.path.join(root, image)
             tmp_pdf = os.path.join(tmp, os.path.basename(os.path.splitext(image)[0]))
-            cmd = ["tesseract", "-l", language, '--dpi', dpi, image, tmp_pdf, "pdf"]
-            print(image[len(root) + 1:])
+            if image.endswith(".jp2"):
+                tmp_jpg = tmp_pdf + ".jpg"
+                if sips_installed:
+                    cmd = ["sips", "-s", "format", "jpeg", image, "--out", tmp_jpg]
+                else:
+                    cmd = ["convert", image, tmp_jpg]
+                subprocess.check_output(cmd)
+                image = tmp_jpg
+            cmd = ["tesseract", "-l", language, "--dpi", dpi, image, tmp_pdf, "pdf"]
+            print(image[len(root) + 1 :])
             subprocess.check_output(cmd)
             pages.append(tmp_pdf + ".pdf")
         cmd = ["pdfunite"] + pages + [pdf]
         subprocess.check_output(cmd)
         print("\ncreated %s" % pdf)
         shutil.rmtree(tmp)
 print("")
```

### Comparing `mdrocr-3/setup.py` & `mdrocr-5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 from setuptools import setup
 
 
 def get_version():
-    return 3 #import subprocess
+    return 5 #import subprocess
     cmd = ['git', 'rev-list', 'HEAD', '--count']
     p = subprocess.Popen(cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
     stdout, stderr = p.communicate()
     rev = int(stdout)
     return u'%s' % rev
```

