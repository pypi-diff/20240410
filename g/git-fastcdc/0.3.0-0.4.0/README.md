# Comparing `tmp/git_fastcdc-0.3.0.tar.gz` & `tmp/git_fastcdc-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git_fastcdc-0.3.0.tar", max compression
+gzip compressed data, was "git_fastcdc-0.4.0.tar", max compression
```

## Comparing `git_fastcdc-0.3.0.tar` & `git_fastcdc-0.4.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    34523 2024-03-28 16:09:33.984653 git_fastcdc-0.3.0/LICENSE
--rw-r--r--   0        0        0     1927 2024-03-29 15:39:11.766309 git_fastcdc-0.3.0/README.md
--rw-r--r--   0        0        0    16321 2024-03-31 12:09:46.812605 git_fastcdc-0.3.0/git_fastcdc.py
--rw-r--r--   0        0        0      722 2024-03-31 12:13:03.981879 git_fastcdc-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2546 1970-01-01 00:00:00.000000 git_fastcdc-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-03-28 16:09:33.984653 git_fastcdc-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1927 2024-03-29 15:39:11.766309 git_fastcdc-0.4.0/README.md
+-rw-r--r--   0        0        0    16458 2024-03-31 12:41:39.115237 git_fastcdc-0.4.0/git_fastcdc.py
+-rw-r--r--   0        0        0      721 2024-04-10 10:42:15.108265 git_fastcdc-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2646 1970-01-01 00:00:00.000000 git_fastcdc-0.4.0/PKG-INFO
```

### Comparing `git_fastcdc-0.3.0/LICENSE` & `git_fastcdc-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `git_fastcdc-0.3.0/README.md` & `git_fastcdc-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `git_fastcdc-0.3.0/git_fastcdc.py` & `git_fastcdc-0.4.0/git_fastcdc.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,18 +8,14 @@
 from subprocess import DEVNULL, PIPE, CalledProcessError, Popen, run
 from tempfile import NamedTemporaryFile
 
 import click
 from fastcdc import fastcdc  # type: ignore
 from tqdm import tqdm
 
-read = sys.stdin.buffer.read
-buffer = sys.stdout.buffer
-write = buffer.write
-flush = buffer.flush
 cdcbranch = "git-fastcdc"
 cdcattr = "/.gitattributes text -binary -filter"
 cdcignore = "/.gitignore text -binary -filter"
 avg_min = 256 * 1024
 pkt_size = 65516
 
 # Helpers
@@ -55,14 +51,19 @@
     if _ondisk is None:
         _ondisk = git_config_ondisk().strip() == b"true"
     return _ondisk
 
 
 # git pkt-line
 
+read = sys.stdin.buffer.read
+buffer = sys.stdout.buffer
+write = buffer.write
+flush = buffer.flush
+
 
 def read_pkt_line():
     length_hex = read(4)
     if not length_hex:
         return b""
 
     length = int(length_hex, 16)
@@ -304,15 +305,18 @@
     data = b"".join(pkgs).decode("UTF-8")
     write_pkt_line_str("status=success\n")
     flush_pkt()
     proc = git_cat_batch()
     stdin = proc.stdin
     stdout = proc.stdout
     for line in data.splitlines():
-        line = line.strip()
+        if not fnmatch(line, "*.cdc"):
+            raise RuntimeError(
+                "Not a fastcdc file. Do you have a bad .gitattributes config?"
+            )
         hash = Path(line).stem
         if line:
             for chunk in git_cat_yield(hash, stdin, stdout, pkt_size):
                 write_pkt_line(chunk)
     flush_pkt()
     flush_pkt()
```

### Comparing `git_fastcdc-0.3.0/PKG-INFO` & `git_fastcdc-0.4.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: git-fastcdc
-Version: 0.3.0
+Version: 0.4.0
 Summary: FastCDC for large git files
 License: AGPL-3.0-or-later
 Author: Jean-Louis Fuchs
 Author-email: jean-louis.fuchs@adfinis.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: fastcdc (>=1.5.0,<2.0.0)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Description-Content-Type: text/markdown
```

