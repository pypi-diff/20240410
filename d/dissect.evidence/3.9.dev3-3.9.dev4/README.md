# Comparing `tmp/dissect.evidence-3.9.dev3.tar.gz` & `tmp/dissect.evidence-3.9.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.evidence-3.9.dev3.tar", last modified: Thu Mar 28 17:21:51 2024, max compression
+gzip compressed data, was "dissect.evidence-3.9.dev4.tar", last modified: Wed Apr 10 11:03:52 2024, max compression
```

## Comparing `dissect.evidence-3.9.dev3.tar` & `dissect.evidence-3.9.dev4.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:51.369973 dissect.evidence-3.9.dev3/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-03-28 17:21:41.000000 dissect.evidence-3.9.dev3/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-28 17:21:41.000000 dissect.evidence-3.9.dev3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-28 17:21:41.000000 dissect.evidence-3.9.dev3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-03-28 17:21:51.369973 dissect.evidence-3.9.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-03-28 17:21:41.000000 dissect.evidence-3.9.dev3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:51.361973 dissect.evidence-3.9.dev3/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:51.365973 dissect.evidence-3.9.dev3/dissect/evidence/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-28 17:21:41.000000 dissect.evidence-3.9.dev3/dissect/evidence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6560 2024-03-28 17:21:41.000000 dissect.evidence-3.9.dev3/dissect/evidence/ad1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:51.365973 dissect.evidence-3.9.dev3/dissect/evidence/asdf/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-03-28 17:21:41.000000 dissect.evidence-3.9.dev3/dissect/evidence/asdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23802 2024-03-28 17:21:41.000000 dissect.evidence-3.9.dev3/dissect/evidence/asdf/asdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-03-28 17:21:41.000000 dissect.evidence-3.9.dev3/dissect/evidence/asdf/streams.py
--rw-r--r--   0 runner    (1001) docker     (127)    14757 2024-03-28 17:21:41.000000 dissect.evidence-3.9.dev3/dissect/evidence/ewf.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-03-28 17:21:41.000000 dissect.evidence-3.9.dev3/dissect/evidence/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:51.365973 dissect.evidence-3.9.dev3/dissect/evidence/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:41.000000 dissect.evidence-3.9.dev3/dissect/evidence/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:51.369973 dissect.evidence-3.9.dev3/dissect/evidence/tools/asdf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:41.000000 dissect.evidence-3.9.dev3/dissect/evidence/tools/asdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-03-28 17:21:41.000000 dissect.evidence-3.9.dev3/dissect/evidence/tools/asdf/dd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-03-28 17:21:41.000000 dissect.evidence-3.9.dev3/dissect/evidence/tools/asdf/meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-03-28 17:21:41.000000 dissect.evidence-3.9.dev3/dissect/evidence/tools/asdf/repair.py
--rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-03-28 17:21:41.000000 dissect.evidence-3.9.dev3/dissect/evidence/tools/asdf/verify.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:51.369973 dissect.evidence-3.9.dev3/dissect.evidence.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-03-28 17:21:51.000000 dissect.evidence-3.9.dev3/dissect.evidence.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-03-28 17:21:51.000000 dissect.evidence-3.9.dev3/dissect.evidence.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 17:21:51.000000 dissect.evidence-3.9.dev3/dissect.evidence.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-03-28 17:21:51.000000 dissect.evidence-3.9.dev3/dissect.evidence.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-28 17:21:51.000000 dissect.evidence-3.9.dev3/dissect.evidence.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-28 17:21:51.000000 dissect.evidence-3.9.dev3/dissect.evidence.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-03-28 17:21:46.000000 dissect.evidence-3.9.dev3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 17:21:51.369973 dissect.evidence-3.9.dev3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:51.369973 dissect.evidence-3.9.dev3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:41.000000 dissect.evidence-3.9.dev3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-03-28 17:21:41.000000 dissect.evidence-3.9.dev3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:51.369973 dissect.evidence-3.9.dev3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-03-28 17:21:41.000000 dissect.evidence-3.9.dev3/tests/data/ad1_long.ad1
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-03-28 17:21:41.000000 dissect.evidence-3.9.dev3/tests/data/ad1_test.ad1
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-03-28 17:21:41.000000 dissect.evidence-3.9.dev3/tests/data/ad1_test_compressed.ad1
--rw-r--r--   0 runner    (1001) docker     (127)     7630 2024-03-28 17:21:41.000000 dissect.evidence-3.9.dev3/tests/data/ewf.E01
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:51.369973 dissect.evidence-3.9.dev3/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-03-28 17:21:41.000000 dissect.evidence-3.9.dev3/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-03-28 17:21:41.000000 dissect.evidence-3.9.dev3/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-28 17:21:41.000000 dissect.evidence-3.9.dev3/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-03-28 17:21:41.000000 dissect.evidence-3.9.dev3/tests/test_ad1.py
--rw-r--r--   0 runner    (1001) docker     (127)     8289 2024-03-28 17:21:41.000000 dissect.evidence-3.9.dev3/tests/test_asdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-03-28 17:21:41.000000 dissect.evidence-3.9.dev3/tests/test_ewf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-03-28 17:21:41.000000 dissect.evidence-3.9.dev3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:03:52.930215 dissect.evidence-3.9.dev4/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-04-10 11:03:52.930215 dissect.evidence-3.9.dev4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:03:52.922215 dissect.evidence-3.9.dev4/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:03:52.926215 dissect.evidence-3.9.dev4/dissect/evidence/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/dissect/evidence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6560 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/dissect/evidence/ad1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:03:52.926215 dissect.evidence-3.9.dev4/dissect/evidence/asdf/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/dissect/evidence/asdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23846 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/dissect/evidence/asdf/asdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/dissect/evidence/asdf/streams.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14757 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/dissect/evidence/ewf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/dissect/evidence/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:03:52.926215 dissect.evidence-3.9.dev4/dissect/evidence/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/dissect/evidence/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:03:52.926215 dissect.evidence-3.9.dev4/dissect/evidence/tools/asdf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/dissect/evidence/tools/asdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/dissect/evidence/tools/asdf/dd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/dissect/evidence/tools/asdf/meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/dissect/evidence/tools/asdf/repair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/dissect/evidence/tools/asdf/verify.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:03:52.930215 dissect.evidence-3.9.dev4/dissect.evidence.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-04-10 11:03:52.000000 dissect.evidence-3.9.dev4/dissect.evidence.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-10 11:03:52.000000 dissect.evidence-3.9.dev4/dissect.evidence.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 11:03:52.000000 dissect.evidence-3.9.dev4/dissect.evidence.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-10 11:03:52.000000 dissect.evidence-3.9.dev4/dissect.evidence.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-10 11:03:52.000000 dissect.evidence-3.9.dev4/dissect.evidence.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-10 11:03:52.000000 dissect.evidence-3.9.dev4/dissect.evidence.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-10 11:03:47.000000 dissect.evidence-3.9.dev4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 11:03:52.930215 dissect.evidence-3.9.dev4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:03:52.926215 dissect.evidence-3.9.dev4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:03:52.926215 dissect.evidence-3.9.dev4/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/tests/data/ad1_long.ad1
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/tests/data/ad1_test.ad1
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/tests/data/ad1_test_compressed.ad1
+-rw-r--r--   0 runner    (1001) docker     (127)     7630 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/tests/data/ewf.E01
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:03:52.930215 dissect.evidence-3.9.dev4/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/tests/test_ad1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8289 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/tests/test_asdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/tests/test_ewf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/tox.ini
```

### Comparing `dissect.evidence-3.9.dev3/LICENSE` & `dissect.evidence-3.9.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.9.dev3/PKG-INFO` & `dissect.evidence-3.9.dev4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.evidence
-Version: 3.9.dev3
+Version: 3.9.dev4
 Summary: A Dissect module implementing a parsers for various forensic evidence file containers, currently: AD1, ASDF and EWF
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.evidence
 Project-URL: repository, https://github.com/fox-it/dissect.evidence
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.evidence-3.9.dev3/README.md` & `dissect.evidence-3.9.dev4/README.md`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.9.dev3/dissect/evidence/ad1.py` & `dissect.evidence-3.9.dev4/dissect/evidence/ad1.py`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.9.dev3/dissect/evidence/asdf/asdf.py` & `dissect.evidence-3.9.dev4/dissect/evidence/asdf/asdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import uuid
 from bisect import bisect_right
 from collections import defaultdict
 from typing import BinaryIO, Callable, Iterator, Optional
 
 from dissect import cstruct
 from dissect.util import ts
-from dissect.util.stream import AlignedStream
+from dissect.util.stream import AlignedStream, RangeStream
 
 from dissect.evidence.asdf.streams import CompressedStream, Crc32Stream, HashedStream
 from dissect.evidence.exceptions import (
     InvalidBlock,
     InvalidSnapshot,
     UnsupportedVersion,
 )
@@ -307,16 +307,16 @@
             idx=idx,
             offset=absolute_offset,
             size=size,
         )
         block.write(self.fh)
         data_offset = self.fh.tell()  # Block data location
 
-        source.seek(offset)
-        shutil.copyfileobj(source, outfh, size)
+        source_stream = RangeStream(source, offset, size)
+        shutil.copyfileobj(source_stream, outfh)
         # This writes any remaining data or footer for each block writer
         outfh.finalize()
 
         data_size = self.fh.tell() - data_offset
 
         lookup_table.insert(table_idx, absolute_offset)
         entry_table.insert(table_idx, (flags, idx, absolute_offset, size, block_offset, data_size))
```

### Comparing `dissect.evidence-3.9.dev3/dissect/evidence/asdf/streams.py` & `dissect.evidence-3.9.dev4/dissect/evidence/asdf/streams.py`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.9.dev3/dissect/evidence/ewf.py` & `dissect.evidence-3.9.dev4/dissect/evidence/ewf.py`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.9.dev3/dissect/evidence/exceptions.py` & `dissect.evidence-3.9.dev4/dissect/evidence/exceptions.py`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.9.dev3/dissect/evidence/tools/asdf/dd.py` & `dissect.evidence-3.9.dev4/dissect/evidence/tools/asdf/dd.py`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.9.dev3/dissect/evidence/tools/asdf/meta.py` & `dissect.evidence-3.9.dev4/dissect/evidence/tools/asdf/meta.py`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.9.dev3/dissect/evidence/tools/asdf/repair.py` & `dissect.evidence-3.9.dev4/dissect/evidence/tools/asdf/repair.py`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.9.dev3/dissect/evidence/tools/asdf/verify.py` & `dissect.evidence-3.9.dev4/dissect/evidence/tools/asdf/verify.py`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.9.dev3/dissect.evidence.egg-info/PKG-INFO` & `dissect.evidence-3.9.dev4/dissect.evidence.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.evidence
-Version: 3.9.dev3
+Version: 3.9.dev4
 Summary: A Dissect module implementing a parsers for various forensic evidence file containers, currently: AD1, ASDF and EWF
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.evidence
 Project-URL: repository, https://github.com/fox-it/dissect.evidence
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.evidence-3.9.dev3/dissect.evidence.egg-info/SOURCES.txt` & `dissect.evidence-3.9.dev4/dissect.evidence.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.9.dev3/pyproject.toml` & `dissect.evidence-3.9.dev4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.9.dev3/tests/conftest.py` & `dissect.evidence-3.9.dev4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.9.dev3/tests/data/ad1_long.ad1` & `dissect.evidence-3.9.dev4/tests/data/ad1_long.ad1`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.9.dev3/tests/data/ad1_test.ad1` & `dissect.evidence-3.9.dev4/tests/data/ad1_test.ad1`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.9.dev3/tests/data/ad1_test_compressed.ad1` & `dissect.evidence-3.9.dev4/tests/data/ad1_test_compressed.ad1`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.9.dev3/tests/data/ewf.E01` & `dissect.evidence-3.9.dev4/tests/data/ewf.E01`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.9.dev3/tests/docs/Makefile` & `dissect.evidence-3.9.dev4/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.9.dev3/tests/docs/conf.py` & `dissect.evidence-3.9.dev4/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.9.dev3/tests/test_ad1.py` & `dissect.evidence-3.9.dev4/tests/test_ad1.py`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.9.dev3/tests/test_asdf.py` & `dissect.evidence-3.9.dev4/tests/test_asdf.py`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.9.dev3/tests/test_ewf.py` & `dissect.evidence-3.9.dev4/tests/test_ewf.py`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.9.dev3/tox.ini` & `dissect.evidence-3.9.dev4/tox.ini`

 * *Files identical despite different names*

