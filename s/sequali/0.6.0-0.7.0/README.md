# Comparing `tmp/sequali-0.6.0.tar.gz` & `tmp/sequali-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sequali-0.6.0.tar", last modified: Fri Mar 29 13:58:16 2024, max compression
+gzip compressed data, was "sequali-0.7.0.tar", last modified: Wed Apr 10 11:54:11 2024, max compression
```

## Comparing `sequali-0.6.0.tar` & `sequali-0.7.0.tar`

### file list

```diff
@@ -1,56 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:58:16.889583 sequali-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-03-29 13:53:55.000000 sequali-0.6.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6614 2024-03-29 13:53:55.000000 sequali-0.6.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-29 13:53:55.000000 sequali-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-29 13:53:55.000000 sequali-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6005 2024-03-29 13:58:16.889583 sequali-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-03-29 13:53:55.000000 sequali-0.6.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-29 13:53:55.000000 sequali-0.6.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:58:16.881583 sequali-0.6.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:58:16.877583 sequali-0.6.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:58:16.881583 sequali-0.6.0/docs/_static/images/
--rw-r--r--   0 runner    (1001) docker     (127)    42483 2024-03-29 13:53:55.000000 sequali-0.6.0/docs/_static/images/fingerprint.fodg
--rw-r--r--   0 runner    (1001) docker     (127)    14977 2024-03-29 13:53:55.000000 sequali-0.6.0/docs/_static/images/fingerprint.svg
--rw-r--r--   0 runner    (1001) docker     (127)    48097 2024-03-29 13:53:55.000000 sequali-0.6.0/docs/_static/images/overrepresented_sampling.fodg
--rw-r--r--   0 runner    (1001) docker     (127)    26339 2024-03-29 13:53:55.000000 sequali-0.6.0/docs/_static/images/overrepresented_sampling.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-03-29 13:53:55.000000 sequali-0.6.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:58:16.881583 sequali-0.6.0/docs/includes/
--rw-r--r--   0 runner    (1001) docker     (127)     6614 2024-03-29 13:53:55.000000 sequali-0.6.0/docs/includes/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-03-29 13:53:55.000000 sequali-0.6.0/docs/includes/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-03-29 13:53:55.000000 sequali-0.6.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-03-29 13:53:55.000000 sequali-0.6.0/docs/module_options.rst
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-29 13:53:55.000000 sequali-0.6.0/docs/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-03-29 13:53:55.000000 sequali-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 13:58:16.889583 sequali-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-03-29 13:53:55.000000 sequali-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:58:16.877583 sequali-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:58:16.881583 sequali-0.6.0/src/sequali/
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-03-29 13:53:55.000000 sequali-0.6.0/src/sequali/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12866 2024-03-29 13:53:55.000000 sequali-0.6.0/src/sequali/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-03-29 13:53:55.000000 sequali-0.6.0/src/sequali/_qc.pyi
--rw-r--r--   0 runner    (1001) docker     (127)   163158 2024-03-29 13:53:55.000000 sequali-0.6.0/src/sequali/_qcmodule.c
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-29 13:58:16.000000 sequali-0.6.0/src/sequali/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:58:16.885583 sequali-0.6.0/src/sequali/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-03-29 13:53:55.000000 sequali-0.6.0/src/sequali/adapters/adapter_list.tsv
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-03-29 13:53:55.000000 sequali-0.6.0/src/sequali/adapters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:58:16.885583 sequali-0.6.0/src/sequali/contaminants/
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-03-29 13:53:55.000000 sequali-0.6.0/src/sequali/contaminants/README
--rw-r--r--   0 runner    (1001) docker     (127)  1701925 2024-03-29 13:53:55.000000 sequali-0.6.0/src/sequali/contaminants/UniVec.fasta
--rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-03-29 13:53:55.000000 sequali-0.6.0/src/sequali/contaminants/oxford_nanopore.fasta
--rw-r--r--   0 runner    (1001) docker     (127)    58889 2024-03-29 13:53:55.000000 sequali-0.6.0/src/sequali/contaminants/oxford_nanopore_barcodes.fasta
--rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-03-29 13:53:55.000000 sequali-0.6.0/src/sequali/murmur3.h
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-29 13:53:55.000000 sequali-0.6.0/src/sequali/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    67615 2024-03-29 13:53:55.000000 sequali-0.6.0/src/sequali/report_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-03-29 13:53:55.000000 sequali-0.6.0/src/sequali/score_to_error_rate.h
--rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-03-29 13:53:55.000000 sequali-0.6.0/src/sequali/sequence_identification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:58:16.885583 sequali-0.6.0/src/sequali/style/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-03-29 13:53:55.000000 sequali-0.6.0/src/sequali/style/sequali_report.css
--rw-r--r--   0 runner    (1001) docker     (127)     6988 2024-03-29 13:53:55.000000 sequali-0.6.0/src/sequali/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-03-29 13:53:55.000000 sequali-0.6.0/src/sequali/wanghash.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:58:16.885583 sequali-0.6.0/src/sequali.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6005 2024-03-29 13:58:16.000000 sequali-0.6.0/src/sequali.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-03-29 13:58:16.000000 sequali-0.6.0/src/sequali.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 13:58:16.000000 sequali-0.6.0/src/sequali.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-29 13:58:16.000000 sequali-0.6.0/src/sequali.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-29 13:58:16.000000 sequali-0.6.0/src/sequali.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-29 13:58:16.000000 sequali-0.6.0/src/sequali.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:54:11.166338 sequali-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-10 11:49:50.000000 sequali-0.7.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7184 2024-04-10 11:49:50.000000 sequali-0.7.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-10 11:49:50.000000 sequali-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-10 11:49:50.000000 sequali-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6005 2024-04-10 11:54:11.166338 sequali-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-04-10 11:49:50.000000 sequali-0.7.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-10 11:49:50.000000 sequali-0.7.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:54:11.158337 sequali-0.7.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:54:11.154338 sequali-0.7.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:54:11.158337 sequali-0.7.0/docs/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    42483 2024-04-10 11:49:50.000000 sequali-0.7.0/docs/_static/images/fingerprint.fodg
+-rw-r--r--   0 runner    (1001) docker     (127)    14977 2024-04-10 11:49:50.000000 sequali-0.7.0/docs/_static/images/fingerprint.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    48097 2024-04-10 11:49:50.000000 sequali-0.7.0/docs/_static/images/overrepresented_sampling.fodg
+-rw-r--r--   0 runner    (1001) docker     (127)    26339 2024-04-10 11:49:50.000000 sequali-0.7.0/docs/_static/images/overrepresented_sampling.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-10 11:49:50.000000 sequali-0.7.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:54:11.158337 sequali-0.7.0/docs/includes/
+-rw-r--r--   0 runner    (1001) docker     (127)     7184 2024-04-10 11:49:50.000000 sequali-0.7.0/docs/includes/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-04-10 11:49:50.000000 sequali-0.7.0/docs/includes/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-10 11:49:50.000000 sequali-0.7.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-04-10 11:49:50.000000 sequali-0.7.0/docs/module_options.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-10 11:49:50.000000 sequali-0.7.0/docs/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-10 11:49:50.000000 sequali-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 11:54:11.166338 sequali-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-10 11:49:50.000000 sequali-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:54:11.154338 sequali-0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:54:11.162338 sequali-0.7.0/src/sequali/
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-10 11:49:50.000000 sequali-0.7.0/src/sequali/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12810 2024-04-10 11:49:50.000000 sequali-0.7.0/src/sequali/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-04-10 11:49:50.000000 sequali-0.7.0/src/sequali/_qc.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)   155348 2024-04-10 11:49:50.000000 sequali-0.7.0/src/sequali/_qcmodule.c
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-10 11:54:11.000000 sequali-0.7.0/src/sequali/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:54:11.162338 sequali-0.7.0/src/sequali/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-04-10 11:49:50.000000 sequali-0.7.0/src/sequali/adapters/adapter_list.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-10 11:49:50.000000 sequali-0.7.0/src/sequali/adapters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:54:11.166338 sequali-0.7.0/src/sequali/contaminants/
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-10 11:49:50.000000 sequali-0.7.0/src/sequali/contaminants/README
+-rw-r--r--   0 runner    (1001) docker     (127)  1701925 2024-04-10 11:49:50.000000 sequali-0.7.0/src/sequali/contaminants/UniVec.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-04-10 11:49:50.000000 sequali-0.7.0/src/sequali/contaminants/oxford_nanopore.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)    58889 2024-04-10 11:49:50.000000 sequali-0.7.0/src/sequali/contaminants/oxford_nanopore_barcodes.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-10 11:49:50.000000 sequali-0.7.0/src/sequali/debug_vectors.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16796 2024-04-10 11:49:50.000000 sequali-0.7.0/src/sequali/function_dispatch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-04-10 11:49:50.000000 sequali-0.7.0/src/sequali/murmur3.h
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-10 11:49:50.000000 sequali-0.7.0/src/sequali/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:54:11.166338 sequali-0.7.0/src/sequali/pygal.js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:54:11.166338 sequali-0.7.0/src/sequali/pygal.js/2.0.x/
+-rw-r--r--   0 runner    (1001) docker     (127)    11879 2024-04-10 11:49:50.000000 sequali-0.7.0/src/sequali/pygal.js/2.0.x/pygal-tooltips.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-04-10 11:49:50.000000 sequali-0.7.0/src/sequali/pygal.js/2.0.x/pygal-tooltips.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-10 11:49:50.000000 sequali-0.7.0/src/sequali/pygal.js/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    70963 2024-04-10 11:49:50.000000 sequali-0.7.0/src/sequali/report_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-04-10 11:49:50.000000 sequali-0.7.0/src/sequali/score_to_error_rate.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-04-10 11:49:50.000000 sequali-0.7.0/src/sequali/sequence_identification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:54:11.166338 sequali-0.7.0/src/sequali/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-10 11:49:50.000000 sequali-0.7.0/src/sequali/static/sequali_report.css
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-10 11:49:50.000000 sequali-0.7.0/src/sequali/static/svg_to_download_link.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6988 2024-04-10 11:49:50.000000 sequali-0.7.0/src/sequali/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-10 11:49:50.000000 sequali-0.7.0/src/sequali/wanghash.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:54:11.166338 sequali-0.7.0/src/sequali.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6005 2024-04-10 11:54:11.000000 sequali-0.7.0/src/sequali.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-10 11:54:11.000000 sequali-0.7.0/src/sequali.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 11:54:11.000000 sequali-0.7.0/src/sequali.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-10 11:54:11.000000 sequali-0.7.0/src/sequali.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-10 11:54:11.000000 sequali-0.7.0/src/sequali.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-10 11:54:11.000000 sequali-0.7.0/src/sequali.egg-info/top_level.txt
```

### Comparing `sequali-0.6.0/CHANGELOG.rst` & `sequali-0.7.0/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,27 @@
 ==========
 
 .. Newest changes should be on top.
 
 .. This document is user facing. Please word the changes in such a way
 .. that users understand how the changes affect the new version.
 
+version 0.7.0
+-----------------
++ Image files can now be saved as SVG files.
++ The javascript file for the tooltip highlighting is now embedded in the
+  html file so no internet access is needed for the functionality.
++ A sidebar with a table of contents is added to the report for easier
+  navigation.
++ Graph fonts are made a little bigger. Graphs now respond to zooming in and
+  out on the web page.
++ Enable building on ARM platforms such as M1 macintosh and Aarch64.
++ Speedup the overrepresented sequences module by adding an AVX2 k-mer
+  construction algorithm.
+
 version 0.6.0
 -----------------
 + Add links to the documentation in the report.
 + Moved documentation to readthedocs and added extensive module documentation.
 + Change the ``-deduplication-estimate-bits`` to a more understandable
   ``--duplication-max-stored-fingerprints``.
 + Add a small table that lists how many reads are >=Q5, >=Q7 etc. in the
```

### Comparing `sequali-0.6.0/LICENSE` & `sequali-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sequali-0.6.0/PKG-INFO` & `sequali-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sequali
-Version: 0.6.0
+Version: 0.7.0
 Summary: Fast sequencing quality metrics
 Author-email: Ruben Vorderman <r.h.p.vorderman@lumc.nl>
 License: AGPL-v3.0
 Project-URL: Documentation, https://sequali.readthedocs.io
 Project-URL: Homepage, https://github.com/rhpvorderman/sequali
 Project-URL: Issue tracker, https://github.com/rhpvorderman/sequali/issues
 Keywords: FASTQ,sequencing quality,uBAM,QC,nanopore,illumina
```

### Comparing `sequali-0.6.0/README.rst` & `sequali-0.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `sequali-0.6.0/docs/_static/images/fingerprint.fodg` & `sequali-0.7.0/docs/_static/images/fingerprint.fodg`

 * *Files identical despite different names*

### Comparing `sequali-0.6.0/docs/_static/images/fingerprint.svg` & `sequali-0.7.0/docs/_static/images/fingerprint.svg`

 * *Files identical despite different names*

### Comparing `sequali-0.6.0/docs/_static/images/overrepresented_sampling.fodg` & `sequali-0.7.0/docs/_static/images/overrepresented_sampling.fodg`

 * *Files identical despite different names*

### Comparing `sequali-0.6.0/docs/_static/images/overrepresented_sampling.svg` & `sequali-0.7.0/docs/_static/images/overrepresented_sampling.svg`

 * *Files identical despite different names*

### Comparing `sequali-0.6.0/docs/conf.py` & `sequali-0.7.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sequali-0.6.0/docs/includes/CHANGELOG.rst` & `sequali-0.7.0/docs/includes/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,27 @@
 ==========
 
 .. Newest changes should be on top.
 
 .. This document is user facing. Please word the changes in such a way
 .. that users understand how the changes affect the new version.
 
+version 0.7.0
+-----------------
++ Image files can now be saved as SVG files.
++ The javascript file for the tooltip highlighting is now embedded in the
+  html file so no internet access is needed for the functionality.
++ A sidebar with a table of contents is added to the report for easier
+  navigation.
++ Graph fonts are made a little bigger. Graphs now respond to zooming in and
+  out on the web page.
++ Enable building on ARM platforms such as M1 macintosh and Aarch64.
++ Speedup the overrepresented sequences module by adding an AVX2 k-mer
+  construction algorithm.
+
 version 0.6.0
 -----------------
 + Add links to the documentation in the report.
 + Moved documentation to readthedocs and added extensive module documentation.
 + Change the ``-deduplication-estimate-bits`` to a more understandable
   ``--duplication-max-stored-fingerprints``.
 + Add a small table that lists how many reads are >=Q5, >=Q7 etc. in the
```

### Comparing `sequali-0.6.0/docs/includes/README.rst` & `sequali-0.7.0/docs/includes/README.rst`

 * *Files identical despite different names*

### Comparing `sequali-0.6.0/docs/index.rst` & `sequali-0.7.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `sequali-0.6.0/docs/module_options.rst` & `sequali-0.7.0/docs/module_options.rst`

 * *Files identical despite different names*

### Comparing `sequali-0.6.0/pyproject.toml` & `sequali-0.7.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -50,15 +50,17 @@
 
 [tool.setuptools.package-data]
 sequali = [
     '*.pyi',
     'py.typed',
     'contaminants/*',
     'adapters/*',
-    'style/*'
+    'static/*',
+    'pygal.js/README.md',
+    'pygal.js/2.0.x/*'
 ]
 [project.urls]
 "Documentation" = "https://sequali.readthedocs.io"
 "Homepage" = "https://github.com/rhpvorderman/sequali"
 "Issue tracker" = "https://github.com/rhpvorderman/sequali/issues"
 
 [tool.setuptools_scm]
```

### Comparing `sequali-0.6.0/setup.py` & `sequali-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `sequali-0.6.0/src/sequali/__init__.py` & `sequali-0.7.0/src/sequali/__init__.py`

 * *Files identical despite different names*

### Comparing `sequali-0.6.0/src/sequali/__main__.py` & `sequali-0.7.0/src/sequali/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -228,15 +228,15 @@
         args.json = os.path.join(args.outdir, args.json)
     if not os.path.isabs(args.html):
         args.html = os.path.join(args.outdir, args.html)
     with open(args.json, "wt") as json_file:
         json_dict = report_modules_to_dict(report_modules)
         # Indent=0 is ~40% smaller than indent=2 while still human-readable
         json.dump(json_dict, json_file, indent=0)
-    write_html_report(report_modules, args.html, filename)
+    write_html_report(report_modules, args.html)
 
 
 if __name__ == "__main__":  # pragma: no cover
     main()
 
 
 def sequali_report():
@@ -248,9 +248,8 @@
     output = args.html
     in_json = args.json
     if not output:
         # Remove json extension and add HTML
         output = ".".join(in_json.split(".")[:-1]) + ".html"
     with open(in_json) as j:
         json_data = json.load(j)
-    write_html_report(dict_to_report_modules(json_data), output,
-                      output.rstrip(".html"))
+    write_html_report(dict_to_report_modules(json_data), output)
```

### Comparing `sequali-0.6.0/src/sequali/_qc.pyi` & `sequali-0.7.0/src/sequali/_qc.pyi`

 * *Files identical despite different names*

### Comparing `sequali-0.6.0/src/sequali/_qcmodule.c` & `sequali-0.7.0/src/sequali/_qcmodule.c`

 * *Files 7% similar despite different names*

```diff
@@ -15,29 +15,27 @@
 You should have received a copy of the GNU Affero General Public License
 along with Sequali.  If not, see <https://www.gnu.org/licenses/
 */
 
 #define PY_SSIZE_T_CLEAN
 #include "Python.h"
 #include "structmember.h"
-#include "stdbool.h"
 
+#include "stdbool.h"
 #include "math.h"
+
+#include "function_dispatch.h"
 #include "score_to_error_rate.h"
 #include "murmur3.h"
 #include "wanghash.h"
 
 #ifdef __SSE2__
 #include "emmintrin.h"
 #endif
 
-#ifdef __SSSE3__
-#include "tmmintrin.h"
-#endif
-
 #if (PY_VERSION_HEX < 0x03090000)
     #define Py_SET_REFCNT(op, count) (Py_REFCNT(op) = count)
     #define Py_SET_SIZE(op, size) (Py_SIZE(op) = size)
     #define Py_SET_TYPE(op, type) (Py_TYPE(op) = type)
 #endif
 
 /* Pointers to types that will be imported in the module initialization section */
@@ -107,52 +105,65 @@
     return result;
 }
 
 
 #define ASCII_MASK_8BYTE 0x8080808080808080ULL
 #define ASCII_MASK_1BYTE 0x80
 
+static inline int string_is_ascii_fallback(const char *string, size_t length)
+{
+    size_t all_chars = 0;
+    for (size_t i=0; i<length; i++) {
+        all_chars |= string[i];
+    }
+    return !(all_chars & ASCII_MASK_1BYTE);
+}
+
 /**
  * @brief Check if a string of given length only contains ASCII characters.
  *
  * @param string A char pointer to the start of the string.
- * @param length The length of the string. This funtion does not check for 
+ * @param length The length of the string. This funtion does not check for
  *               terminating NULL bytes.
  * @returns 1 if the string is ASCII-only, 0 otherwise.
  */
 static int
-string_is_ascii(const char * string, size_t length) {
-    // By performing bitwise OR on all characters in 8-byte chunks (16-byte 
-    // with SSE2) we can
-    // determine ASCII status in a non-branching (except the loops) fashion.
-    uint64_t all_chars = 0;
-    const char *cursor = string;
-    const char *string_end_ptr = string + length;
-    const char *string_8b_end_ptr = string_end_ptr - sizeof(uint64_t); 
-    int non_ascii_in_vec = 0;
-    #ifdef __SSE2__
-    const char *string_16b_end_ptr = string_end_ptr - sizeof(__m128i);
-    __m128i vec_all_chars = _mm_setzero_si128();
-    while (cursor < string_16b_end_ptr) {
-        __m128i loaded_chars = _mm_loadu_si128((__m128i *)cursor);
-        vec_all_chars = _mm_or_si128(loaded_chars, vec_all_chars);
-        cursor += sizeof(__m128i);
-    }
-    non_ascii_in_vec = _mm_movemask_epi8(vec_all_chars);
-    #endif
-
-    while (cursor < string_8b_end_ptr) {
-        all_chars |= *(uint64_t *)cursor;
-        cursor += sizeof(uint64_t);
-    }
-    while (cursor < string_end_ptr) {
-        all_chars |= *cursor;
-        cursor += 1;
+string_is_ascii(const char *string, size_t length)
+{
+    if (length < sizeof(size_t)) {
+        return string_is_ascii_fallback(string, length);
     }
-    return !(non_ascii_in_vec + (all_chars & ASCII_MASK_8BYTE));
+    size_t number_of_chunks = length / sizeof(size_t);
+    size_t *chunks = (size_t *)string;
+    size_t number_of_unrolls = number_of_chunks / 4;
+    size_t remaining_chunks = number_of_chunks - (number_of_unrolls * 4);
+    size_t *chunk_ptr = chunks;
+    size_t all_chars0 = 0;
+    size_t all_chars1 = 0;
+    size_t all_chars2 = 0;
+    size_t all_chars3 = 0;
+    for (size_t i=0; i < number_of_unrolls; i++) {
+        /* Performing indepedent OR calculations allows the compiler to use
+           vectors. It also allows out of order execution. */
+        all_chars0 |= chunk_ptr[0];
+        all_chars1 |= chunk_ptr[1];
+        all_chars2 |= chunk_ptr[2];
+        all_chars3 |= chunk_ptr[3];
+        chunk_ptr += 4;
+    }
+    size_t all_chars = all_chars0 | all_chars1 | all_chars2 | all_chars3;
+    for (size_t i=0; i<remaining_chunks; i++) {
+        all_chars |= chunk_ptr[i];
+    }
+    /* Load the last few bytes left in a single integer for fast operations.
+       There is some overlap here with the work done before, but for a simple
+       ascii check this does not matter. */
+    size_t last_chunk = *(size_t *)(string + length - sizeof(size_t));
+    all_chars |= last_chunk;
+    return !(all_chars & ASCII_MASK_8BYTE);
 }
 
 /***
  * Seconds since epoch for years of 1970 and higher is defined in the POSIX 
  * specification.:
  * https://pubs.opengroup.org/onlinepubs/9699919799/basedefs/V1_chap04.html#tag_04_16
  * With a little help from Eric S. Raymond's solution in this stackoverflow
@@ -1050,129 +1061,14 @@
     uint16_t flag;
     uint32_t l_seq;
     int32_t next_ref_id;
     int32_t next_pos;
     int32_t tlen;
 };
 
-static void 
-decode_bam_sequence(uint8_t *dest, const uint8_t *encoded_sequence, size_t length) 
-{
-    /* Reuse a trick from sam_internal.h in htslib. Have a table to lookup 
-       two characters simultaneously.*/
-    static const char code2base[512] =
-        "===A=C=M=G=R=S=V=T=W=Y=H=K=D=B=N"
-        "A=AAACAMAGARASAVATAWAYAHAKADABAN"
-        "C=CACCCMCGCRCSCVCTCWCYCHCKCDCBCN"
-        "M=MAMCMMMGMRMSMVMTMWMYMHMKMDMBMN"
-        "G=GAGCGMGGGRGSGVGTGWGYGHGKGDGBGN"
-        "R=RARCRMRGRRRSRVRTRWRYRHRKRDRBRN"
-        "S=SASCSMSGSRSSSVSTSWSYSHSKSDSBSN"
-        "V=VAVCVMVGVRVSVVVTVWVYVHVKVDVBVN"
-        "T=TATCTMTGTRTSTVTTTWTYTHTKTDTBTN"
-        "W=WAWCWMWGWRWSWVWTWWWYWHWKWDWBWN"
-        "Y=YAYCYMYGYRYSYVYTYWYYYHYKYDYBYN"
-        "H=HAHCHMHGHRHSHVHTHWHYHHHKHDHBHN"
-        "K=KAKCKMKGKRKSKVKTKWKYKHKKKDKBKN"
-        "D=DADCDMDGDRDSDVDTDWDYDHDKDDDBDN"
-        "B=BABCBMBGBRBSBVBTBWBYBHBKBDBBBN"
-        "N=NANCNMNGNRNSNVNTNWNYNHNKNDNBNN";
-    static const uint8_t *nuc_lookup = (uint8_t *)"=ACMGRSVTWYHKDBN";
-    const uint8_t *dest_end_ptr = dest + length;
-    uint8_t *dest_cursor = dest;
-    const uint8_t *encoded_cursor = encoded_sequence;
-    #ifdef __SSSE3__
-    const uint8_t *dest_vec_end_ptr = dest_end_ptr - (2 * sizeof(__m128i));
-    __m128i first_upper_shuffle = _mm_setr_epi8(
-        0, 0xff, 1, 0xff, 2, 0xff, 3, 0xff, 4, 0xff, 5, 0xff, 6, 0xff, 7, 0xff);
-    __m128i first_lower_shuffle = _mm_setr_epi8(
-        0xff, 0, 0xff, 1, 0xff, 2, 0xff, 3, 0xff, 4, 0xff, 5, 0xff, 6, 0xff, 7);
-    __m128i second_upper_shuffle = _mm_setr_epi8(
-        8, 0xff, 9, 0xff, 10, 0xff, 11, 0xff, 12, 0xff, 13, 0xff, 14, 0xff, 15, 0xff);
-    __m128i second_lower_shuffle = _mm_setr_epi8(
-        0xff, 8, 0xff, 9, 0xff, 10, 0xff, 11, 0xff, 12, 0xff, 13, 0xff, 14, 0xff, 15);
-    __m128i nuc_lookup_vec = _mm_lddqu_si128((__m128i *)nuc_lookup);
-    /* Work on 16 encoded characters at the time resulting in 32 decoded characters 
-       Examples are given for 8 encoded characters A until H to keep it readable.
-        Encoded stored as |AB|CD|EF|GH|
-        Shuffle into |AB|00|CD|00|EF|00|GH|00| and 
-                     |00|AB|00|CD|00|EF|00|GH| 
-        Shift upper to the right resulting into
-                     |0A|B0|0C|D0|0E|F0|0G|H0| and 
-                     |00|AB|00|CD|00|EF|00|GH|
-        Merge with or resulting into (X stands for garbage)
-                     |0A|XB|0C|XD|0E|XF|0G|XH|
-        Bitwise and with 0b1111 leads to:
-                     |0A|0B|0C|0D|0E|0F|0G|0H|
-        We can use the resulting 4-bit integers as indexes for the shuffle of 
-        the nucleotide lookup. */
-    while (dest_cursor < dest_vec_end_ptr) {
-        __m128i encoded = _mm_lddqu_si128((__m128i *)encoded_cursor);
-
-        __m128i first_upper = _mm_shuffle_epi8(encoded, first_upper_shuffle);
-        __m128i first_lower = _mm_shuffle_epi8(encoded, first_lower_shuffle);
-        __m128i shifted_first_upper = _mm_srli_epi64(first_upper, 4);
-        __m128i first_merged = _mm_or_si128(shifted_first_upper, first_lower);
-        __m128i first_indexes = _mm_and_si128(first_merged, _mm_set1_epi8(0b1111));
-        __m128i first_nucleotides = _mm_shuffle_epi8(nuc_lookup_vec, first_indexes);
-        _mm_storeu_si128((__m128i *)dest_cursor, first_nucleotides);
-
-        __m128i second_upper = _mm_shuffle_epi8(encoded, second_upper_shuffle);
-        __m128i second_lower = _mm_shuffle_epi8(encoded, second_lower_shuffle);
-        __m128i shifted_second_upper = _mm_srli_epi64(second_upper, 4);
-        __m128i second_merged = _mm_or_si128(shifted_second_upper, second_lower);
-        __m128i second_indexes = _mm_and_si128(second_merged, _mm_set1_epi8(0b1111));
-        __m128i second_nucleotides = _mm_shuffle_epi8(nuc_lookup_vec, second_indexes);
-        _mm_storeu_si128((__m128i *)(dest_cursor + 16), second_nucleotides);
-
-        encoded_cursor += sizeof(__m128i);
-        dest_cursor += 2 * sizeof(__m128i);
-    }
-    #endif
-    /* Do two at the time until it gets to the last even address. */
-    const uint8_t *dest_end_ptr_twoatatime = dest + (length & (~1ULL));
-    while (dest_cursor < dest_end_ptr_twoatatime) {
-        /* According to htslib, size_t cast helps the optimizer. 
-           Code confirmed to indeed run faster. */
-        memcpy(dest_cursor, code2base + ((size_t)*encoded_cursor * 2), 2);
-        dest_cursor += 2;
-        encoded_cursor += 1;
-    }
-    assert((dest_end_ptr - dest_cursor) < 2);
-    if (dest_cursor != dest_end_ptr) {
-        /* There is a single encoded nuc left */
-        uint8_t encoded_nucs = *encoded_cursor;
-        uint8_t upper_nuc_index = encoded_nucs >> 4;
-        dest_cursor[0] = nuc_lookup[upper_nuc_index];
-    }
-}
-
-static void 
-decode_bam_qualities(uint8_t *dest, const uint8_t *encoded_qualities, size_t length) 
-{
-    const uint8_t *end_ptr = encoded_qualities + length;
-    const uint8_t *cursor = encoded_qualities;
-    uint8_t *dest_cursor = dest; 
-    #ifdef __SSE2__
-    const uint8_t *vec_end_ptr = end_ptr - sizeof(__m128i);
-    while (cursor < vec_end_ptr) {
-        __m128i quals = _mm_loadu_si128((__m128i *)cursor);
-        __m128i phreds = _mm_add_epi8(quals, _mm_set1_epi8(33));
-        _mm_storeu_si128((__m128i *)dest_cursor, phreds);
-        cursor += sizeof(__m128i);
-        dest_cursor += sizeof(__m128i);
-    }
-    #endif
-    while (cursor < end_ptr) {
-        *dest_cursor = *cursor + 33; 
-        cursor += 1;
-        dest_cursor += 1;    
-    }
-}
-
 static int
 bam_tags_to_fastq_meta(const uint8_t *tags, size_t tags_length, struct FastqMeta *meta)
 {
     meta->channel = -1;
     meta->duration = 0.0;
     meta->start_time = 0;
     while (tags_length > 0) {
@@ -1644,16 +1540,16 @@
         register __m128i a_counts = _mm_setzero_si128();
         register __m128i c_counts = _mm_setzero_si128();
         register __m128i g_counts = _mm_setzero_si128();
         register __m128i t_counts = _mm_setzero_si128();
         register __m128i all1 = _mm_set1_epi8(1);
         for (size_t i=0; i<iterations; i++) {
             __m128i nucleotides = _mm_loadu_si128((__m128i *)sequence_ptr);
-            // This will make all the nucleotides uppercase.
-            nucleotides = _mm_and_si128(nucleotides, _mm_set1_epi8(223)); 
+            // 32 is the lowercase bit. Turning it off makes everything uppercase.
+            nucleotides = _mm_andnot_si128(_mm_set1_epi8(32), nucleotides);
             __m128i a_nucs = _mm_cmpeq_epi8(nucleotides, _mm_set1_epi8('A'));
             __m128i a_positions = _mm_and_si128(a_nucs, all1);
             a_counts = _mm_add_epi8(a_counts, a_positions);
             __m128i c_nucs = _mm_cmpeq_epi8(nucleotides, _mm_set1_epi8('C'));
             __m128i c_positions = _mm_and_si128(c_nucs, all1);
             c_counts = _mm_add_epi8(c_counts, c_positions);
             __m128i g_nucs = _mm_cmpeq_epi8(nucleotides, _mm_set1_epi8('G'));
@@ -3018,97 +2914,20 @@
     .tp_methods = PerTileQuality_methods,
 };
 
 /**********************
  * TWOBIT CONVERSIONS *
  **********************/
 
-/* To be used in the sequence duplication part */
-
-static const uint8_t NUCLEOTIDE_TO_TWOBIT[128] = {
-// Control characters
-    4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4,
-    4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4,
-// Interpunction numbers etc
-    4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4,
-    4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4,
-//     A, B, C, D, E, F, G, H, I, J, K, L, M, N, O,
-    4, 0, 4, 1, 4, 4, 4, 2, 4, 4, 4, 4, 4, 4, 8, 4,
-//  P, Q, R, S, T, U, V, W, X, Y, Z,  
-    4, 4, 4, 4, 3, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4,
-//     a, b, c, d, e, f, g, h, i, j, k, l, m, n, o,
-    4, 0, 4, 1, 4, 4, 4, 2, 4, 4, 4, 4, 4, 4, 8, 4,
-//  p, q, r, s, t, u, v, w, x, y, z, 
-    4, 4, 4, 4, 3, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 
-};
-
-#define TWOBIT_UNKNOWN_CHAR -1
-#define TWOBIT_N_CHAR -2 
-#define TWOBIT_SUCCESS 0
-
-static uint64_t reverse_complement_kmer(uint64_t kmer, uint64_t k) {
-    // Invert all the bits, with 0,1,2,3 == A,C,G,T this automatically is the
-    // complement. 
-    uint64_t comp = ~kmer; 
-    // Progressively swap all the twobits inplace.
-    uint64_t revcomp = (comp << 32) | (comp >> 32);
-    revcomp = ((revcomp & 0xFFFF0000FFFF0000ULL) >> 16) | 
-              ((revcomp & 0x0000FFFF0000FFFFULL) << 16);
-    revcomp = ((revcomp & 0xFF00FF00FF00FF00ULL) >> 8) | 
-              ((revcomp & 0x00FF00FF00FF00FFULL) << 8);
-    revcomp = ((revcomp & 0xF0F0F0F0F0F0F0F0ULL) >> 4) | 
-              ((revcomp & 0x0F0F0F0F0F0F0F0FULL) << 4);
-    revcomp = ((revcomp & 0xCCCCCCCCCCCCCCCCULL) >> 2) | 
-              ((revcomp & 0x3333333333333333ULL) << 2);
-    // If k < 32, the empty twobit slots will have ended up at the least 
-    // significant bits. Use a shift to move them to the highest bits again.
-    return revcomp >> (64 - (k *2));
-}
-
-static int64_t sequence_to_canonical_kmer(uint8_t *sequence, uint64_t k) {
-    uint64_t kmer = 0;
-    size_t all_nucs = 0;
-    Py_ssize_t i=0;
-    Py_ssize_t vector_end = k - 4;
-    for (i=0; i<vector_end; i+=4) {
-        size_t nuc0 = NUCLEOTIDE_TO_TWOBIT[sequence[i]];
-        size_t nuc1 = NUCLEOTIDE_TO_TWOBIT[sequence[i+1]];
-        size_t nuc2 = NUCLEOTIDE_TO_TWOBIT[sequence[i+2]];
-        size_t nuc3 = NUCLEOTIDE_TO_TWOBIT[sequence[i+3]];
-        all_nucs |= (nuc0 | nuc1 | nuc2 | nuc3);
-        uint64_t kchunk = ((nuc0 << 6) | (nuc1 << 4) | (nuc2 << 2) | (nuc3));
-        kmer <<= 8;
-        kmer |= kchunk;
-    }
-    for (i=i; i<(Py_ssize_t)k; i++) {
-        size_t nuc = NUCLEOTIDE_TO_TWOBIT[sequence[i]];
-        all_nucs |= nuc;
-        kmer <<= 2;
-        kmer |= nuc;
-    }
-    if (all_nucs > 3) {
-        if (all_nucs & 4) {
-            return TWOBIT_UNKNOWN_CHAR;
-        }
-        if (all_nucs & 8) {
-            return TWOBIT_N_CHAR;
-        }
-    }
-    uint64_t revcomp_kmer = reverse_complement_kmer(kmer, k);
-    // If k is uneven there can be no ambiguity
-    if (revcomp_kmer > kmer) {
-        return kmer;
-    }
-    return revcomp_kmer;
-}
+/* Most functions moved to function_dispatch.h */
 
 static void kmer_to_sequence(uint64_t kmer, size_t k, uint8_t *sequence) {
     static uint8_t nucs[4] = {'A', 'C', 'G', 'T'};
     for (size_t i=k; i>0; i-=1) {
-        size_t nuc = kmer & 0b11;
+        size_t nuc = kmer & 3; // 3 == 0b11
         sequence[i - 1] = nucs[nuc];
         kmer >>= 2;
     }
 }
 
 /*************************
  * SEQUENCE DUPLICATION *
@@ -3304,20 +3123,22 @@
             continue;
         }
         fragments += 1;
         uint64_t hash = wanghash64(kmer);
         Sequence_duplication_insert_hash(self, hash);
     }
     if (warn_unknown) {
+        PyObject *culprit = PyUnicode_DecodeASCII((char *)sequence, sequence_length, NULL);
         PyErr_WarnFormat(
             PyExc_UserWarning, 
             1,
             "Sequence contains a chacter that is not A, C, G, T or N: %R", 
-            PyUnicode_DecodeASCII((char *)sequence, sequence_length, NULL)
+            culprit
         );
+        Py_DECREF(culprit);
     }
     self->total_fragments += fragments;
     return 0;
 } 
 
 PyDoc_STRVAR(SequenceDuplication_add_read__doc__,
 "add_read($self, read, /)\n"
```

### Comparing `sequali-0.6.0/src/sequali/adapters/adapter_list.tsv` & `sequali-0.7.0/src/sequali/adapters/adapter_list.tsv`

 * *Files identical despite different names*

### Comparing `sequali-0.6.0/src/sequali/adapters.py` & `sequali-0.7.0/src/sequali/adapters.py`

 * *Files identical despite different names*

### Comparing `sequali-0.6.0/src/sequali/contaminants/README` & `sequali-0.7.0/src/sequali/contaminants/README`

 * *Files identical despite different names*

### Comparing `sequali-0.6.0/src/sequali/contaminants/UniVec.fasta` & `sequali-0.7.0/src/sequali/contaminants/UniVec.fasta`

 * *Files identical despite different names*

### Comparing `sequali-0.6.0/src/sequali/contaminants/oxford_nanopore.fasta` & `sequali-0.7.0/src/sequali/contaminants/oxford_nanopore.fasta`

 * *Files identical despite different names*

### Comparing `sequali-0.6.0/src/sequali/contaminants/oxford_nanopore_barcodes.fasta` & `sequali-0.7.0/src/sequali/contaminants/oxford_nanopore_barcodes.fasta`

 * *Files identical despite different names*

### Comparing `sequali-0.6.0/src/sequali/murmur3.h` & `sequali-0.7.0/src/sequali/murmur3.h`

 * *Files identical despite different names*

### Comparing `sequali-0.6.0/src/sequali/report_modules.py` & `sequali-0.7.0/src/sequali/report_modules.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,20 +13,22 @@
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with Sequali.  If not, see <https://www.gnu.org/licenses/
 
 import array
 import collections
 import dataclasses
+import html
 import io
 import math
 import os
 import sys
 import time
 import typing
+import xml.etree.ElementTree
 from abc import ABC, abstractmethod
 from collections import defaultdict
 from pathlib import Path
 from typing import (Any, Dict, Iterable, Iterator, List, Optional, Sequence,
                     Set, Tuple, Type)
 
 import pygal  # type: ignore
@@ -38,16 +40,22 @@
 from ._qc import NUMBER_OF_NUCS, NUMBER_OF_PHREDS, PHRED_MAX
 from ._version import __version__
 from .adapters import Adapter
 from .sequence_identification import DEFAULT_CONTAMINANTS_FILES, DEFAULT_K, \
     create_sequence_index, identify_sequence, reverse_complement
 from .util import fasta_parser
 
-SEQUALI_REPORT_CSS = Path(__file__).parent / "style" / "sequali_report.css"
+SEQUALI_REPORT_CSS = Path(__file__).parent / "static" / "sequali_report.css"
 SEQUALI_REPORT_CSS_CONTENT = SEQUALI_REPORT_CSS.read_text(encoding="utf-8")
+SEQUALI_REPORT_JS = (Path(__file__).parent / "pygal.js" / "2.0.x" /
+                     "pygal-tooltips.min.js")
+SEQUALI_DOWNLOAD_SVG_JS = (Path(__file__).parent / "static" /
+                           "svg_to_download_link.js")
+SEQUALI_DOWNLOAD_SVG_JS_CONTENT = SEQUALI_DOWNLOAD_SVG_JS.read_text()
+SEQUALI_REPORT_JS_CONTENT = SEQUALI_REPORT_JS.read_text()
 
 PHRED_INDEX_TO_ERROR_RATE = [
     sum(10 ** (-p / 10) for p in range(start * 4, start * 4 + 4)) / 4
     for start in range(NUMBER_OF_PHREDS)
 ]
 PHRED_INDEX_TO_PHRED = [-10 * math.log10(PHRED_INDEX_TO_ERROR_RATE[i])
                         for i in range(NUMBER_OF_PHREDS)]
@@ -74,32 +82,99 @@
     '#15508d',  # 40-43
     '#053061',  # >=44
 ]
 
 COLOR_GREEN = "#33cc33"
 COLOR_RED = "#ff0000"
 
+COMMON_GRAPH_STYLE_OPTIONS = dict(
+    font_family="sans-serif",
+    label_font_size=14,
+    major_label_font_size=14,
+    value_label_font_size=14,
+    title_font_size=18,
+    legend_font_size=16,
+)
+
 QUALITY_DISTRIBUTION_STYLE = pygal.style.Style(colors=QUALITY_COLORS,
-                                               font_family="sans-serif")
+                                               **COMMON_GRAPH_STYLE_OPTIONS)
 ONE_SERIE_STYLE = pygal.style.DefaultStyle(colors=("#33cc33",),  # Green
-                                           font_family="sans-serif")
-MULTIPLE_SERIES_STYLE = pygal.style.DefaultStyle(font_family="sans-serif")
+                                           **COMMON_GRAPH_STYLE_OPTIONS)
+MULTIPLE_SERIES_STYLE = pygal.style.DefaultStyle(**COMMON_GRAPH_STYLE_OPTIONS)
 
 DEFAULT_FRACTION_THRESHOLD = 0.0001
 DEFAULT_MIN_THRESHOLD = 100
 DEFAULT_MAX_THRESHOLD = sys.maxsize
 
 COMMON_GRAPH_OPTIONS = dict(
     truncate_label=-1,
-    width=1200,
+    width=1250,
+    height=700,
     disable_xml_declaration=True,
     js=[],  # Script is globally downloaded once
 )
 
 
+def html_header(header: str, level: int):
+    html_id = header.lower().replace(" ", "-")
+    return f"""
+        <h{level} id="{html_id}">
+            <a class="headerlink" href="#{html_id}">{header}</a>
+        </h{level}>
+    """
+
+
+def create_toc(content: str):
+    toc = io.StringIO()
+    toc.write('<ul class="toc_list">')
+    root = xml.etree.ElementTree.fromstring(content)
+    current_level = 1
+    for element in root.iter():  # type: xml.etree.ElementTree.Element
+        tag = element.tag
+        if tag.startswith("h") and len(tag) == 2 and tag[1].isdecimal():
+            header_level = int(tag[1])
+            reference_element = element.find("a")
+            if reference_element is None:
+                raise RuntimeError("Header format error. Can't create toc.")
+            header = reference_element.text
+            id = element.get("id")
+            if header_level != current_level:
+                if header_level > current_level:
+                    for i in range(header_level - current_level):
+                        toc.write('<ul class="toc_list">')
+                else:
+                    for i in range(current_level - header_level):
+                        toc.write("</ul>")
+                current_level = header_level
+            toc.write(f'<li><a class="toclink" href="#{id}">{header}</a></li>')
+    if current_level > 0:
+        for i in range(current_level):
+            toc.write("</ul>")
+    return toc.getvalue()
+
+
+def figurize_plot(plot: pygal.Graph):
+    svg_unicode = plot.render(is_unicode=True)
+    svg_tree: xml.etree.ElementTree.Element = (
+        xml.etree.ElementTree.fromstring(svg_unicode))
+    svg_id = svg_tree.get("id")
+    title: str = plot.config.title
+    filename = title.lower().replace(" ", "_") + ".svg"
+    return f"""
+        <figure>
+            {svg_unicode}
+            <figcaption>
+                <script>
+                document.write(svgToDownloadLink("{svg_id}", "{filename}"));
+                </script>
+            </figcaption>
+        </figure>
+    """
+
+
 def equidistant_ranges(length: int, parts: int) -> Iterator[Tuple[int, int]]:
     size = length // parts
     remainder = length % parts
     small_parts = parts - remainder
     start = 0
     for i in range(parts):
         part_size = size if i < small_parts else size + 1
@@ -177,15 +252,15 @@
 
 def label_settings(x_labels: Sequence[str]) -> Dict[str, Any]:
     # Labels are ranges such as 1-5, 101-142 etc. This clutters the x axis
     # labeling so only use the first number. The values will be labelled
     # separately.
     simple_x_labels = [label.split("-")[0] for label in x_labels]
     if simple_x_labels and len(simple_x_labels[-1]) > 4:
-        rotation = 30
+        rotation = 45
     else:
         rotation = 0
     return dict(
         x_labels=simple_x_labels,
         x_labels_major_every=round(len(x_labels) / 30),
         x_label_rotation=rotation,
         show_minor_x_labels=False
@@ -232,14 +307,15 @@
         timestamp = time.time()
         time_struct = time.localtime(timestamp)
         report_generated = time.strftime("%Y-%m-%d %H:%M:%S%z", time_struct)
         return cls(__version__, report_generated, filename, filesize)
 
     def to_html(self) -> str:
         return f"""
+        {html_header("Metadata", 1)}
         <table>
             <tr><td>Filename</td><td><code>{self.filename}</code></td></tr>
             <tr><td>Filesize</td><td>{self.filesize / (1024 ** 3):.2f} GiB</td></tr>
             <tr><td>Sequali version</td><td>{self.sequali_version}</td></tr>
             <tr><td>Report generated on</td><td>{self.report_generated}</td></tr>
         </table>
         """
@@ -255,15 +331,15 @@
     total_bases: int
     q20_bases: int
     total_gc_bases: int
     total_n_bases: int
 
     def to_html(self) -> str:
         return f"""
-            <h2>Summary</h2>
+            {html_header("Summary", 1)}
             <table>
             <tr><td>Mean length</td><td style="text-align:right;">
                 {self.mean_length:,.2f}</td><td></td></tr>
             <tr><td>Length range (min-max)</td><td style="text-align:right;">
                 {self.minimum_length:,}</td>
                 <td style="text-align:right;">{self.maximum_length:,}</td></tr>
             <tr>
@@ -312,25 +388,25 @@
     q25: int
     q50: int
     q75: int
     q90: int
     q95: int
     q99: int
 
-    def plot(self) -> str:
+    def plot(self) -> pygal.Graph:
         plot = pygal.Bar(
             title="Sequence length distribution",
             x_title="sequence length",
             y_title="number of reads",
             style=ONE_SERIE_STYLE,
             **label_settings(self.length_ranges),
             **COMMON_GRAPH_OPTIONS,
         )
         plot.add("Length", label_values(self.counts, self.length_ranges))
-        return plot.render(is_unicode=True)
+        return plot
 
     def distribution_table(self):
         if len({self.q1, self.q5, self.q10, self.q25, self.q50,
                 self.q75, self.q90, self.q95, self.q99}) == 1:
             return ""
         return f"""
             <table>
@@ -344,17 +420,17 @@
                 <tr><td>N95</td><td style="text-align:right;">{self.q95:,}</td></tr>
                 <tr><td>N99</td><td style="text-align:right;">{self.q99:,}</td></tr>
             </table>
         """
 
     def to_html(self):
         return f"""
-            <h2>Sequence length distribution</h2>
+            {html_header("Sequence length distribution", 1)}
             <p>{self.distribution_table()}</p>
-            <figure>{self.plot()}</figure>
+            {figurize_plot(self.plot())}
         """
 
     @classmethod
     def from_base_count_tables(cls,
                                base_count_tables: array.ArrayType,
                                total_sequences: int,
                                data_ranges: Sequence[Tuple[int, int]]):
@@ -404,25 +480,25 @@
 
 
 @dataclasses.dataclass
 class PerPositionMeanQualityAndSpread(ReportModule):
     x_labels: List[str]
     percentiles: List[Tuple[str, List[float]]]
 
-    def plot(self) -> str:
+    def plot(self) -> pygal.Graph:
         plot = pygal.Line(
             title="Per position quality percentiles",
             show_dots=False,
             x_title="position",
             y_title="phred score",
             y_labels=list(range(0, 51, 10)),
             range=(0.0, 50.0),
             style=pygal.style.DefaultStyle(
                 colors=["#000000"] * 12,
-                font_family="sans-serif",
+                **COMMON_GRAPH_STYLE_OPTIONS,
             ),
             **label_settings(self.x_labels),
             **COMMON_GRAPH_OPTIONS,
         )
         percentiles = dict(self.percentiles)
         plot.add("top 1%", label_values(percentiles["top 1%"], self.x_labels),
                  stroke_style={"dasharray": '1,2'})
@@ -430,25 +506,25 @@
                  stroke_style={"dasharray": '3,3'})
         plot.add("mean", label_values(percentiles["mean"], self.x_labels),
                  show_dots=True, dots_size=1)
         plot.add("bottom 5%", label_values(percentiles["bottom 5%"], self.x_labels),
                  stroke_style={"dasharray": '3,3'})
         plot.add("bottom 1%", label_values(percentiles["bottom 1%"], self.x_labels),
                  stroke_style={"dasharray": '1,2'})
-        return plot.render(is_unicode=True)
+        return plot
 
     def to_html(self):
         return f"""
-            <h2>Per position quality percentiles</h2>
+            {html_header("Per position quality percentiles", 1)}
             <p class="explanation">Shows the mean for all bases and the means
             of the lowest and
             highest percentiles to indicate the spread. Since the graph is
             based on the sampled categories, rather than exact phreds, it is
             an approximation.</p>
-            <figure>{self.plot()}</figure>
+            {figurize_plot(self.plot())}
         """
 
     @classmethod
     def from_phred_table_and_labels(cls, phred_tables: array.ArrayType, x_labels):
         percentiles = [1, 5, 10, 25, 50, 75, 90, 95, 99]
         percentile_fractions = [i / 100 for i in percentiles]
         total_tables = len(phred_tables) // NUMBER_OF_PHREDS
@@ -539,15 +615,15 @@
             for offset, phred_count in enumerate(table):
                 if phred_count == 0:
                     continue
                 nuc_fraction = phred_count / total_nucs
                 quality_distribution[offset][cat_index] = nuc_fraction
         return cls(x_labels, quality_distribution)
 
-    def plot(self) -> str:
+    def plot(self) -> pygal.Graph:
         plot = pygal.StackedBar(
             title="Per base quality distribution",
             style=QUALITY_DISTRIBUTION_STYLE,
             dots_size=1,
             y_labels=[i / 10 for i in range(11)],
             x_title="position",
             y_title="fraction",
@@ -555,29 +631,29 @@
             **label_settings(self.x_labels),
             **COMMON_GRAPH_OPTIONS,
         )
         for name, serie in zip(QUALITY_SERIES_NAMES, self.series):
             serie_filled = sum(serie) > 0.0
             plot.add(name, label_values(serie, self.x_labels),
                      show_dots=serie_filled)
-        return plot.render(is_unicode=True)
+        return plot
 
     def to_html(self):
         return f"""
-            <h2>Per position quality score distribution</h2>
-            <figure>{self.plot()}</figure>
+            {html_header("Per position quality score distribution", 1)}
+            {figurize_plot(self.plot())}
         """
 
 
 @dataclasses.dataclass
 class PerSequenceAverageQualityScores(ReportModule):
     average_quality_counts: Sequence[int]
     x_labels: Tuple[str, ...] = tuple(str(x) for x in range(PHRED_MAX + 1))
 
-    def plot(self) -> str:
+    def plot(self) -> pygal.Graph:
         maximum_score = 0
         for i, count in enumerate(self.average_quality_counts):
             if count > 0:
                 maximum_score = i
         maximum_score = max(maximum_score + 2, 40)
         plot = pygal.Bar(
             title="Per sequence quality scores",
@@ -593,33 +669,33 @@
         if total == 0:
             percentage_scores = [0.0 for _ in self.average_quality_counts]
         else:
             percentage_scores = [100 * score / total
                                  for score in self.average_quality_counts]
 
         plot.add("", percentage_scores[:maximum_score])
-        return plot.render(is_unicode=True)
+        return plot
 
     def to_html(self) -> str:
         return f"""
-            <h2>Per sequence average quality scores</h2>
+            {html_header("Per sequence average quality scores", 1)}
             <p>{self.quality_scores_table()}</p>
-            <figure>{self.plot()}</figure>
+            {figurize_plot(self.plot())}
         """
 
     def quality_scores_table(self) -> str:
         table = io.StringIO()
         total = max(sum(self.average_quality_counts), 1)
         fractions = [count / total for count in self.average_quality_counts]
         table.write("<table>")
         for i in (5, 7, 10, 12, 15, 20, 30):
             table.write(
                 f"""
                 <tr>
-                    <td>&gt=Q{i}</td>
+                    <td>{html.escape(">=Q")}{i}</td>
                     <td style="text-align:right;">
                         {sum(self.average_quality_counts[i:]):,}
                     </td>
                     <td style="text-align:right;">
                         {sum(fractions[i:]):.2%}
                     </td>
                 </tr>
@@ -637,24 +713,24 @@
 class PerPositionBaseContent(ReportModule):
     x_labels: Sequence[str]
     A: Sequence[float]
     C: Sequence[float]
     G: Sequence[float]
     T: Sequence[float]
 
-    def plot(self):
+    def plot(self) -> pygal.Graph:
         style_class = pygal.style.Style
         green = COLOR_GREEN
         dark_green = "#228B22"  # ForestGreen
         blue = "#00BFFF"  # DeepSkyBlue
         dark_blue = "#1E90FF"  # DodgerBlue
         black = "#000000"
         style = style_class(
             colors=(green, dark_green, blue, dark_blue, black),
-            font_family="sans-serif"
+            **COMMON_GRAPH_STYLE_OPTIONS
         )
         plot = pygal.StackedLine(
             title="Base content",
             style=style,
             dots_size=1,
             y_labels=[i / 10 for i in range(11)],
             x_title="position",
@@ -663,20 +739,20 @@
             **label_settings(self.x_labels),
             **COMMON_GRAPH_OPTIONS,
         )
         plot.add("G", label_values(self.G, self.x_labels))
         plot.add("C", label_values(self.C, self.x_labels))
         plot.add("A", label_values(self.A, self.x_labels))
         plot.add("T", label_values(self.T, self.x_labels))
-        return plot.render(is_unicode=True)
+        return plot
 
     def to_html(self) -> str:
         return f"""
-             <h2>Per position base content</h2>
-             <figure>{self.plot()}</figure>
+             {html_header("Per position base content", 1)}
+             {figurize_plot(self.plot())}
         """
 
     @classmethod
     def from_base_count_tables_and_labels(cls,
                                           base_count_tables: array.ArrayType,
                                           labels: Sequence[str]):
         total_tables = len(base_count_tables) // NUMBER_OF_NUCS
@@ -721,86 +797,86 @@
                 continue
             n_fractions[index] = table[N] / total_bases
         return cls(
             labels,
             n_fractions
         )
 
-    def plot(self):
+    def plot(self) -> pygal.Graph:
         plot = pygal.Bar(
             title="Per position N content",
             dots_size=1,
             y_labels=[i / 10 for i in range(11)],
             x_title="position",
             y_title="fraction",
             fill=True,
             style=ONE_SERIE_STYLE,
             **label_settings(self.x_labels),
             **COMMON_GRAPH_OPTIONS,
         )
         plot.add("N", label_values(self.n_content, self.x_labels))
-        return plot.render(is_unicode=True)
+        return plot
 
     def to_html(self) -> str:
         return f"""
-            <h2>Per position N content</h2>
-            <figure>{self.plot()}</figure>
+            {html_header("Per position N content", 1)}
+            {figurize_plot(self.plot())}
         """
 
 
 @dataclasses.dataclass
 class PerSequenceGCContent(ReportModule):
     gc_content_counts: Sequence[int]
     smoothened_gc_content_counts: Sequence[int]
     x_labels: Sequence[str] = tuple(str(x) for x in range(101))
     smoothened_x_labels: Sequence[str] = tuple(str(x) for x in range(0, 101, 2))
 
-    def plot(self):
+    def plot(self) -> pygal.Graph:
         plot = pygal.Bar(
             title="Per sequence GC content",
             x_labels=self.x_labels,
             x_labels_major_every=3,
             show_minor_x_labels=False,
             x_title="GC %",
             y_title="number of reads",
             style=ONE_SERIE_STYLE,
             **COMMON_GRAPH_OPTIONS,
         )
         plot.add("", self.gc_content_counts)
-        return plot.render(is_unicode=True)
+        return plot
 
     def smoothened_plot(self):
         plot = pygal.Line(
             title="Per sequence GC content (smoothened)",
             x_labels=self.smoothened_x_labels,
             x_labels_major_every=3,
             show_minor_x_labels=False,
             x_title="GC %",
             y_title="number of reads",
             interpolate="cubic",
             style=ONE_SERIE_STYLE,
             **COMMON_GRAPH_OPTIONS,
         )
         plot.add("", self.smoothened_gc_content_counts)
-        return plot.render(is_unicode=True)
+        return plot
 
     def to_html(self) -> str:
         return f"""
-            <h2>Per sequence GC content</h2>
+            {html_header("Per sequence GC content", 1)}
             <p class="explanation">
             For short reads with fixed size (i.e. Illumina) the plot will
             look very spiky due to the GC content calculation: GC bases / all
             bases. For read lengths of 151, both 75 and 76 GC bases lead to a
             percentage of 50% (rounded) and 72 and 73 GC bases leads to 48%
             (rounded). Only 74 GC bases leads to 49%. As a result the
             even categories will be twice as high, which creates a spike. The
             smoothened plot is provided to give a clearer picture in this case.
             </p>
-            <figure>{self.plot()}</figure>
-            <figure>{self.smoothened_plot()}</figure>
+            {figurize_plot(self.plot())}
+            {figurize_plot(self.smoothened_plot())}
         """
 
     @classmethod
     def from_qc_metrics(cls, metrics: QCMetrics):
         gc_content = list(metrics.gc_content())
         smoothened_gc_content = []
         gc_content_iter = iter(gc_content)
@@ -812,15 +888,15 @@
 
 
 @dataclasses.dataclass
 class AdapterContent(ReportModule):
     x_labels: Sequence[str]
     adapter_content: Sequence[Tuple[str, Sequence[float]]]
 
-    def plot(self):
+    def plot(self) -> pygal.Graph:
         plot = pygal.Line(
             title="Adapter content (%)",
             range=(0.0, 100.0),
             x_title="position",
             y_title="%",
             legend_at_bottom=True,
             legend_at_bottom_columns=1,
@@ -831,34 +907,34 @@
         )
         adapter_content = [(label, content) for label, content in
                            self.adapter_content if content and max(content) >= 0.1]
         adapter_content.sort(key=lambda x: max(x[1]),
                              reverse=True)
         for label, content in adapter_content:
             plot.add(label, label_values(content, self.x_labels))
-        return plot.render(is_unicode=True)
+        return plot
 
     def to_html(self):
         return f"""
-            <h2>Adapter content</h2>
+            {html_header("Adapter content", 1)}
             <p class="explanation">Only adapters that are present more than 0.1%
             are shown. Given the 12&#8239;bp
             length of the sequences used to estimate the content, values below this
             threshold are problably false positives. The legend is sorted from
             most frequent to least frequent.</p>
             <p class="explanation">For nanopore the the adapter mix (AMX) and
             ligation kit have overlapping adapter sequences and are therefore
             indistinguishable. Please consult the
             <a href="https://help.nanoporetech.com/en/articles/6632917-what-are-the-adapter-sequences-used-in-the-kits">
             nanopore documentation</a> for more information which adapters are
             used by your kit.</p>
             <p class="explanation">For illumina short reads, the last part of
             the graph will be flat as the 12&#8239;bp probes cannot be found in
-            the last 11 base pairs.
-            <figure>{self.plot()}</figure>
+            the last 11 base pairs.</p>
+            {figurize_plot(self.plot())}
         """  # noqa: E501
 
     @classmethod
     def from_adapter_counter_adapters_and_ranges(
             cls, adapter_counter: AdapterCounter, adapters: Sequence[Adapter],
             data_ranges: Sequence[Tuple[int, int]]):
 
@@ -942,21 +1018,21 @@
             x_labels=stringify_ranges(data_ranges),
             normalized_per_tile_averages=normalized_averages,
             tiles_2x_errors=tiles_2x_errors,
             tiles_10x_errors=tiles_10x_errors,
             skipped_reason=ptq.skipped_reason,
         )
 
-    def plot(self):
+    def plot(self) -> pygal.Graph:
         style_colors = MULTIPLE_SERIES_STYLE.colors
         red = "#FF0000"
         yellow = "#FFD700"  # actually 'Gold' which is darker and more visible.
         style = pygal.style.Style(
             colors=(yellow, red) + style_colors,
-            font_family="sans-serif",
+            **COMMON_GRAPH_STYLE_OPTIONS,
         )
         scatter_plot = pygal.Line(
             title="Deviation from geometric mean in phred units.",
             x_title="position",
             stroke=False,
             style=style,
             y_title="Normalized phred",
@@ -983,18 +1059,18 @@
                 continue
             cleaned_phreds = [{'value': phred, 'label': label}
                               if (phred > 3 or phred < -3) else None
                               for phred, label in
                               zip(tile_phreds, self.x_labels)]
             scatter_plot.add(str(tile), cleaned_phreds)
 
-        return scatter_plot.render(is_unicode=True)
+        return scatter_plot
 
     def to_html(self) -> str:
-        header = "<h2>Per tile quality</h2>"
+        header = html_header("Per tile quality", 1)
         if self.skipped_reason:
             return header + (f"Per tile quality skipped. Reason: "
                              f"{self.skipped_reason}.")
         return header + f"""
             <p class="explanation">
             This graph shows the deviation of each tile on each position from
             the geometric mean of all tiles at that position. The scale is
@@ -1002,43 +1078,43 @@
             average.
             -3 is ~2 times more errors than the average. Only points that
             deviate more than 2 phred units from the average are shown. </p>
             <p>Tiles with more than 2 times the average error:
                 {", ".join(self.tiles_2x_errors)}</p>
             <p>Tiles with more than 10 times the average error:
                 {", ".join(self.tiles_10x_errors)}</p>
-            <figure>{self.plot()}</figure>
+            {figurize_plot(self.plot())}
         """
 
 
 @dataclasses.dataclass
 class DuplicationCounts(ReportModule):
     tracked_unique_sequences: int
     duplication_counts: Sequence[Tuple[int, int]]
     remaining_fraction: float
     estimated_duplication_fractions: Dict[str, float]
     fingerprint_front_sequence_length: int
     fingerprint_back_sequence_length: int
     fingerprint_front_sequence_offset: int
     fingerprint_back_sequence_offset: int
 
-    def plot(self):
+    def plot(self) -> pygal.Graph:
         plot = pygal.Bar(
             title="Duplication levels (%)",
             x_labels=list(self.estimated_duplication_fractions.keys()),
             x_title="Duplication counts",
             y_title="Percentage of total",
-            x_label_rotation=30,
+            x_label_rotation=45,
             style=ONE_SERIE_STYLE,
             **COMMON_GRAPH_OPTIONS
         )
         plot.add("",
                  [100 * fraction for fraction in
                   self.estimated_duplication_fractions.values()])
-        return plot.render(is_unicode=True)
+        return plot
 
     def to_html(self):
         first_part = f"""
         <p class="explanation">
         Fingerprints are taken by taking a sample from the beginning and the
         end at an offset. The samples are combined and hashed while using the
         length as a seed. A subsample of these fingerprints is stored to
@@ -1081,17 +1157,17 @@
                 <td>Estimated remaining sequences if deduplicated</td>
                 <td style="text-align:right;">{self.remaining_fraction:.2%}</td>
             </tr>
             </table>
         </p>
         """
         return f"""
-            <h2>Duplication percentages</h2>
+            {html_header("Duplication percentages", 1)}
             {first_part}
-            <figure>{self.plot()}</figure>
+            {figurize_plot(self.plot())}
         """
 
     @staticmethod
     def estimated_counts_to_fractions(
             estimated_counts: Iterable[Tuple[int, int]]):
         named_slices = {
             "1": slice(1, 2),
@@ -1194,15 +1270,15 @@
                    sample_every=d["sample_every"],
                    sequence_length=d["sequence_length"],
                    total_fragments=d["total_fragments"],
                    total_sequences=d["total_sequences"],
                    sampled_sequences=d["sampled_sequences"])  # type: ignore
 
     def to_html(self) -> str:
-        header = "<h2>Overrepresented sequences</h2>"
+        header = html_header("Overrepresented sequences", 1)
         if len(self.overrepresented_sequences) == 0:
             return header + "No overrepresented sequences."
         content = io.StringIO()
         content.write(header)
         content.write(
             f"""
             <p class="explanation">A subsample of the sequences is analysed
@@ -1266,15 +1342,15 @@
                 f"""<tr><td style="text-align:right;">{item.count}</td>
                     <td style="text-align:right;">{item.fraction:.2%}</td>
                     <td style="text-align:center;font-family:monospace;">
                         {item.sequence}</td>
                     <td style="text-align:center;font-family:monospace;">
                         {item.revcomp_sequence}</td>
                     <td>({item.most_matches}/{item.max_matches})</td>
-                    <td>{item.best_match}</td></tr>""")
+                    <td>{html.escape(item.best_match)}</td></tr>""")
         content.write("</table>")
         return content.getvalue()
 
     @classmethod
     def from_sequence_duplication(
             cls,
             seqdup: SequenceDuplication,
@@ -1424,39 +1500,39 @@
             x_title="time(HH:MM)",
             y_title="base count",
             style=ONE_SERIE_STYLE,
             **label_settings(self.x_labels),
             **COMMON_GRAPH_OPTIONS
         )
         plot.add("", label_values(self.time_bases, self.x_labels))
-        return plot.render(is_unicode=True)
+        return plot
 
     def time_reads_plot(self):
         plot = pygal.Bar(
             title="Number of reads over time",
             x_title="time(HH:MM)",
             y_title="number of reads",
             style=ONE_SERIE_STYLE,
             **label_settings(self.x_labels),
             **COMMON_GRAPH_OPTIONS
         )
         plot.add("", label_values(self.time_reads, self.x_labels))
-        return plot.render(is_unicode=True)
+        return plot
 
     def time_active_channels_plot(self):
         plot = pygal.Bar(
             title="Active channels over time",
             x_title="time(HH:MM)",
             y_title="active channels",
             style=ONE_SERIE_STYLE,
             **label_settings(self.x_labels),
             **COMMON_GRAPH_OPTIONS
         )
         plot.add("", label_values(self.time_active_channels, self.x_labels))
-        return plot.render(is_unicode=True)
+        return plot
 
     def time_quality_distribution_plot(self):
         plot = pygal.StackedBar(
             title="Quality distribution over time",
             style=QUALITY_DISTRIBUTION_STYLE,
             dots_size=1,
             y_labels=[i / 10 for i in range(11)],
@@ -1466,15 +1542,15 @@
             **label_settings(self.x_labels),
             **COMMON_GRAPH_OPTIONS,
         )
         for name, serie in zip(QUALITY_SERIES_NAMES, self.qual_percentages_over_time):
             serie_filled = sum(serie) > 0.0
             plot.add(name, label_values(serie, self.x_labels),
                      show_dots=serie_filled)
-        return plot.render(is_unicode=True)
+        return plot
 
     def channel_plot(self):
         plot = pygal.XY(
             title="Channel base yield and quality",
             dots_size=1,
             x_title="base yield (megabases)",
             y_title="quality (phred score)",
@@ -1484,21 +1560,21 @@
         )
         serie = []
         for channel, base_yield in self.per_channel_bases.items():
             quality = self.per_channel_quality[channel]
             serie.append(dict(value=(base_yield/1_000_000, quality),
                               label=str(channel)))
         plot.add(None, serie)
-        return plot.render(is_unicode=True)
+        return plot
 
     def translocation_section(self):
         transl_speeds = self.translocation_speed
         if sum(transl_speeds) == 0:
-            return """
-            <h2>translocation speeds</h2>
+            return f"""
+            {html_header("translocation speeds", 1)}
             Duration information not available.
             """
         too_slow = transl_speeds[:35] + [0] * 55
         too_fast = [0] * 45 + transl_speeds[45:]
         normal = [0] * 35 + transl_speeds[35:45] + [0] * 35
         total = sum(transl_speeds)
         within_bounds_frac = sum(normal) / total
@@ -1508,50 +1584,50 @@
         plot = pygal.Bar(
             title="Translocation speed distribution",
             x_title="Translocation_speed",
             y_title="active channels",
             style=pygal.style.DefaultStyle(
                 # Use blue and red colors to accommodate colorblind people.
                 colors=(QUALITY_COLORS[-3], QUALITY_COLORS[1], QUALITY_COLORS[1]),
-                font_family="sans-serif",
+                **COMMON_GRAPH_STYLE_OPTIONS,
             ),
             x_labels=[str(i) for i in range(0, 800, 10)] + [">800"],
             x_labels_major_every=10,
             show_minor_x_labels=False,
             **COMMON_GRAPH_OPTIONS
         )
         plot.add("within bounds", normal)
         plot.add("too slow", too_slow)
         plot.add("too fast", too_fast)
         return f"""
-        <h2>translocation speeds</h2>
+        {html_header("translocation speeds", 1)}
         <p>Percentage of reads within accepted bounds: {within_bounds_frac:.2%}</p>
         <p>Percentage of reads that are too slow: {too_slow_frac:.2%}</p>
         <p>Percentage of reads that are too fast: {too_fast_frac:.2%}</p>
-        <figure>{plot.render(is_unicode=True)}</figure>
+        {figurize_plot(plot)}
         """
 
     def to_html(self) -> str:
         if self.skipped_reason:
             return f"""
-            <h2>Nanopore time series</h2>
+            {html_header("Nanopore time series", 1)}
             Skipped: {self.skipped_reason}
             """
         return f"""
-        <h2>Nanopore time series</h2>
-        <h3>Base counts over time</h3>
-        <figure>{self.time_bases_plot()}</figure>
-        <h3>Read counts over time</h3>
-        <figure>{self.time_reads_plot()}</figure>
-        <h3>Active channels over time</h3>
-        <figure>{self.time_active_channels_plot()}</figure>
-        <h3>Quality distribution over time</h3>
-        <figure>{self.time_quality_distribution_plot()}</figure>
-        <h2>Per channel base yield versus quality<h2>
-        <figure>{self.channel_plot()}</figure>
+        {html_header("Nanopore time series", 1)}
+        {html_header("Base counts over time", 2)}
+        {figurize_plot(self.time_bases_plot())}
+        {html_header("Read counts over time", 2)}
+        {figurize_plot(self.time_reads_plot())}
+        {html_header("Active channels over time", 2)}
+        {figurize_plot(self.time_active_channels_plot())}
+        {html_header("Quality distribution over time", 2)}
+        {figurize_plot(self.time_quality_distribution_plot())}
+        {html_header("Per channel base yield versus quality", 2)}
+        {figurize_plot(self.channel_plot())}
         {self.translocation_section()}
         """
 
 
 NAME_TO_CLASS: Dict[str, Type[ReportModule]] = {
     "meta": Meta,
     "summary": Summary,
@@ -1583,41 +1659,68 @@
 def dict_to_report_modules(d: Dict[str, Dict[str, Any]]) -> List[ReportModule]:
     return [NAME_TO_CLASS[name].from_dict(
                 NAME_TO_CLASS[name], class_dict)  # type: ignore
             for name, class_dict in d.items()]
 
 
 def write_html_report(report_modules: Iterable[ReportModule],
-                      html: str,
-                      filename: str):
-    default_config = pygal.Config()
-    pygal_script_uri = default_config.js[0].lstrip('/')
+                      html: str):
+    for mod in report_modules:
+        if isinstance(mod, Meta):
+            filename = mod.filename
+            break
+    else:
+        raise RuntimeError("No filename found in metadata")
+    content_division = io.StringIO()
+    content_division.write('<div class="content">')
+    for module in report_modules:
+        content_division.write(module.to_html())
+    content_division.write("</div>")
+    content = content_division.getvalue()
+    toc = create_toc(content)
+
     with open(html, "wt", encoding="utf-8") as html_file:
         html_file.write(f"""
             <!DOCTYPE html>
             <html lang="en">
             <head>
-                <script src="https://{pygal_script_uri}"></script>
+                <script>
+                    {SEQUALI_REPORT_JS_CONTENT}
+                </script>
+                <script>
+                    {SEQUALI_DOWNLOAD_SVG_JS_CONTENT}
+                </script>
                 <style>
                     {SEQUALI_REPORT_CSS_CONTENT}
                 </style>
                 <meta charset="utf-8">
                 <title>{os.path.basename(filename)}: Sequali Report</title>
             </head>
-            <header><p>
-                Report created by Sequali. Please visit the
-                <a href="https://github.com/rhpvorderman/sequali">homepage</a>
-                for bug reports and feature requests.
-            </p></header>
-            <h1>Sequali report</h1>
+            <body>
+        """)
+
+        html_file.write(f"""
+        <div class="toc">
+        {html_header("Sequali report", 1)}
+        <h2>Table of contents</h2>
+        {toc}
+        """)
+        html_file.write("""
+        <h2>Links</h2>
+        <ul>
+            <li><a href="https://sequali.readthedocs.io">Documentation</a></li>
+            <li><a href="https://github.com/rhpvorderman/sequali"
+                >Github repository</a></li>
+            <li><a href="https://github.com/rhpvorderman/sequali/issues"
+                >Bug tracker</a></li>
+        </ul>
         """)
-        # size: {os.stat(filename).st_size / (1024 ** 3):.2f}GiB<br>
-        for module in report_modules:
-            html_file.write(module.to_html())
-        html_file.write("</html>")
+        html_file.write('</div>')
+        html_file.write(content)
+        html_file.write("</body></html>")
 
 
 def qc_metrics_modules(metrics: QCMetrics,
                        data_ranges: Sequence[Tuple[int, int]]
                        ) -> List[ReportModule]:
     base_count_tables = metrics.base_count_table()
     phred_count_table = metrics.phred_count_table()
```

### Comparing `sequali-0.6.0/src/sequali/score_to_error_rate.h` & `sequali-0.7.0/src/sequali/score_to_error_rate.h`

 * *Files identical despite different names*

### Comparing `sequali-0.6.0/src/sequali/sequence_identification.py` & `sequali-0.7.0/src/sequali/sequence_identification.py`

 * *Files identical despite different names*

### Comparing `sequali-0.6.0/src/sequali/util.py` & `sequali-0.7.0/src/sequali/util.py`

 * *Files identical despite different names*

### Comparing `sequali-0.6.0/src/sequali/wanghash.h` & `sequali-0.7.0/src/sequali/wanghash.h`

 * *Files identical despite different names*

### Comparing `sequali-0.6.0/src/sequali.egg-info/PKG-INFO` & `sequali-0.7.0/src/sequali.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sequali
-Version: 0.6.0
+Version: 0.7.0
 Summary: Fast sequencing quality metrics
 Author-email: Ruben Vorderman <r.h.p.vorderman@lumc.nl>
 License: AGPL-v3.0
 Project-URL: Documentation, https://sequali.readthedocs.io
 Project-URL: Homepage, https://github.com/rhpvorderman/sequali
 Project-URL: Issue tracker, https://github.com/rhpvorderman/sequali/issues
 Keywords: FASTQ,sequencing quality,uBAM,QC,nanopore,illumina
```

### Comparing `sequali-0.6.0/src/sequali.egg-info/SOURCES.txt` & `sequali-0.7.0/src/sequali.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 docs/includes/README.rst
 src/sequali/__init__.py
 src/sequali/__main__.py
 src/sequali/_qc.pyi
 src/sequali/_qcmodule.c
 src/sequali/_version.py
 src/sequali/adapters.py
+src/sequali/debug_vectors.h
+src/sequali/function_dispatch.h
 src/sequali/murmur3.h
 src/sequali/py.typed
 src/sequali/report_modules.py
 src/sequali/score_to_error_rate.h
 src/sequali/sequence_identification.py
 src/sequali/util.py
 src/sequali/wanghash.h
@@ -36,8 +38,12 @@
 src/sequali.egg-info/requires.txt
 src/sequali.egg-info/top_level.txt
 src/sequali/adapters/adapter_list.tsv
 src/sequali/contaminants/README
 src/sequali/contaminants/UniVec.fasta
 src/sequali/contaminants/oxford_nanopore.fasta
 src/sequali/contaminants/oxford_nanopore_barcodes.fasta
-src/sequali/style/sequali_report.css
+src/sequali/pygal.js/README.md
+src/sequali/pygal.js/2.0.x/pygal-tooltips.js
+src/sequali/pygal.js/2.0.x/pygal-tooltips.min.js
+src/sequali/static/sequali_report.css
+src/sequali/static/svg_to_download_link.js
```

