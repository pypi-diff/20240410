# Comparing `tmp/gemsembler-0.6.2.tar.gz` & `tmp/gemsembler-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gemsembler-0.6.2.tar", last modified: Thu Apr  4 12:16:51 2024, max compression
+gzip compressed data, was "gemsembler-0.6.3.tar", last modified: Wed Apr 10 08:59:58 2024, max compression
```

## Comparing `gemsembler-0.6.2.tar` & `gemsembler-0.6.3.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:16:51.787443 gemsembler-0.6.2/
--rw-rw-rw-   0 root         (0) root         (0)     1083 2024-04-04 12:16:40.000000 gemsembler-0.6.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       72 2024-04-04 12:16:40.000000 gemsembler-0.6.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4287 2024-04-04 12:16:51.786443 gemsembler-0.6.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1867 2024-04-04 12:16:40.000000 gemsembler-0.6.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1949 2024-04-04 12:16:40.000000 gemsembler-0.6.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-04 12:16:51.787443 gemsembler-0.6.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:16:51.777443 gemsembler-0.6.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:16:51.780443 gemsembler-0.6.2/src/gemsembler/
--rw-rw-rw-   0 root         (0) root         (0)     1785 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      896 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     7898 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/anticreation.py
--rw-rw-rw-   0 root         (0) root         (0)    19906 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/comparison.py
--rw-rw-rw-   0 root         (0) root         (0)    14845 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/conversion.py
--rw-rw-rw-   0 root         (0) root         (0)    52270 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/creation.py
--rw-rw-rw-   0 root         (0) root         (0)     4300 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/curation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:16:51.781443 gemsembler-0.6.2/src/gemsembler/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:16:51.783443 gemsembler-0.6.2/src/gemsembler/data/BU/
--rw-rw-rw-   0 root         (0) root         (0)   180894 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/data/BU/BU_agora.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)   303843 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/data/BU/BU_carveme_hom.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)   381510 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/data/BU/BU_gapseq.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)    83221 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/data/BU/BU_modelSEED.sbml.gz
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/data/BU/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:16:51.786443 gemsembler-0.6.2/src/gemsembler/data/LP/
--rw-rw-rw-   0 root         (0) root         (0)   153653 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/data/LP/LP_CA1.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)   157673 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/data/LP/LP_CA2.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)    82710 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/data/LP/LP_MS2.sbml.gz
--rw-rw-rw-   0 root         (0) root         (0)   885760 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/data/LP/LP_WCFS1.fasta.gz
--rw-rw-rw-   0 root         (0) root         (0)   151435 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/data/LP/LP_WCFS1_agora.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)   124883 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/data/LP/LP_iLP728_revision_data_met_C_c.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)   547669 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/data/LP/LP_protein_fasta.faa.gz
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/data/LP/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10388 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/dbs.py
--rw-rw-rw-   0 root         (0) root         (0)    19185 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/downstream.py
--rw-rw-rw-   0 root         (0) root         (0)    50045 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/drawing.py
--rw-rw-rw-   0 root         (0) root         (0)    24476 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/gathering.py
--rw-rw-rw-   0 root         (0) root         (0)      396 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/general.py
--rw-rw-rw-   0 root         (0) root         (0)    13452 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/genes.py
--rw-rw-rw-   0 root         (0) root         (0)    22859 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/pathsfinding.py
--rw-rw-rw-   0 root         (0) root         (0)     4557 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/periplasmic.py
--rw-rw-rw-   0 root         (0) root         (0)    10165 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/selection.py
--rw-rw-rw-   0 root         (0) root         (0)    31443 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/structural.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:16:51.786443 gemsembler-0.6.2/src/gemsembler.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4287 2024-04-04 12:16:51.000000 gemsembler-0.6.2/src/gemsembler.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1435 2024-04-04 12:16:51.000000 gemsembler-0.6.2/src/gemsembler.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 12:16:51.000000 gemsembler-0.6.2/src/gemsembler.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2024-04-04 12:16:51.000000 gemsembler-0.6.2/src/gemsembler.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      121 2024-04-04 12:16:51.000000 gemsembler-0.6.2/src/gemsembler.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-04-04 12:16:51.000000 gemsembler-0.6.2/src/gemsembler.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:16:51.786443 gemsembler-0.6.2/tests/
--rw-rw-rw-   0 root         (0) root         (0)    12691 2024-04-04 12:16:40.000000 gemsembler-0.6.2/tests/test_conversion.py
--rw-rw-rw-   0 root         (0) root         (0)     2191 2024-04-04 12:16:40.000000 gemsembler-0.6.2/tests/test_curation.py
--rw-rw-rw-   0 root         (0) root         (0)     4293 2024-04-04 12:16:40.000000 gemsembler-0.6.2/tests/test_dbs.py
--rw-rw-rw-   0 root         (0) root         (0)     4021 2024-04-04 12:16:40.000000 gemsembler-0.6.2/tests/test_gathering.py
--rw-rw-rw-   0 root         (0) root         (0)     2357 2024-04-04 12:16:40.000000 gemsembler-0.6.2/tests/test_selection.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 08:59:58.832836 gemsembler-0.6.3/
+-rw-rw-rw-   0 root         (0) root         (0)     1083 2024-04-10 08:59:46.000000 gemsembler-0.6.3/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       72 2024-04-10 08:59:46.000000 gemsembler-0.6.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4287 2024-04-10 08:59:58.832836 gemsembler-0.6.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1867 2024-04-10 08:59:46.000000 gemsembler-0.6.3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1949 2024-04-10 08:59:46.000000 gemsembler-0.6.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 08:59:58.832836 gemsembler-0.6.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 08:59:58.821836 gemsembler-0.6.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 08:59:58.825836 gemsembler-0.6.3/src/gemsembler/
+-rw-rw-rw-   0 root         (0) root         (0)     1785 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      896 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7898 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/anticreation.py
+-rw-rw-rw-   0 root         (0) root         (0)    19906 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/comparison.py
+-rw-rw-rw-   0 root         (0) root         (0)    14845 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/conversion.py
+-rw-rw-rw-   0 root         (0) root         (0)    52270 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/creation.py
+-rw-rw-rw-   0 root         (0) root         (0)     4300 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/curation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 08:59:58.826836 gemsembler-0.6.3/src/gemsembler/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 08:59:58.828836 gemsembler-0.6.3/src/gemsembler/data/BU/
+-rw-rw-rw-   0 root         (0) root         (0)   180894 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/data/BU/BU_agora.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)   303843 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/data/BU/BU_carveme_hom.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)   381510 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/data/BU/BU_gapseq.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)    83221 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/data/BU/BU_modelSEED.sbml.gz
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/data/BU/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 08:59:58.831836 gemsembler-0.6.3/src/gemsembler/data/LP/
+-rw-rw-rw-   0 root         (0) root         (0)   153653 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/data/LP/LP_CA1.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)   157673 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/data/LP/LP_CA2.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)    82710 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/data/LP/LP_MS2.sbml.gz
+-rw-rw-rw-   0 root         (0) root         (0)   885760 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/data/LP/LP_WCFS1.fasta.gz
+-rw-rw-rw-   0 root         (0) root         (0)   151435 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/data/LP/LP_WCFS1_agora.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)   124883 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/data/LP/LP_iLP728_revision_data_met_C_c.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)   547669 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/data/LP/LP_protein_fasta.faa.gz
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/data/LP/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10388 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/dbs.py
+-rw-rw-rw-   0 root         (0) root         (0)    19185 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/downstream.py
+-rw-rw-rw-   0 root         (0) root         (0)    50045 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/drawing.py
+-rw-rw-rw-   0 root         (0) root         (0)    24476 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/gathering.py
+-rw-rw-rw-   0 root         (0) root         (0)      396 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/general.py
+-rw-rw-rw-   0 root         (0) root         (0)    13452 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/genes.py
+-rw-rw-rw-   0 root         (0) root         (0)    22859 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/pathsfinding.py
+-rw-rw-rw-   0 root         (0) root         (0)     4557 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/periplasmic.py
+-rw-rw-rw-   0 root         (0) root         (0)    10165 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/selection.py
+-rw-rw-rw-   0 root         (0) root         (0)    31443 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/structural.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 08:59:58.832836 gemsembler-0.6.3/src/gemsembler.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4287 2024-04-10 08:59:58.000000 gemsembler-0.6.3/src/gemsembler.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1435 2024-04-10 08:59:58.000000 gemsembler-0.6.3/src/gemsembler.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 08:59:58.000000 gemsembler-0.6.3/src/gemsembler.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2024-04-10 08:59:58.000000 gemsembler-0.6.3/src/gemsembler.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      121 2024-04-10 08:59:58.000000 gemsembler-0.6.3/src/gemsembler.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-04-10 08:59:58.000000 gemsembler-0.6.3/src/gemsembler.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 08:59:58.832836 gemsembler-0.6.3/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    12691 2024-04-10 08:59:46.000000 gemsembler-0.6.3/tests/test_conversion.py
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2024-04-10 08:59:46.000000 gemsembler-0.6.3/tests/test_curation.py
+-rw-rw-rw-   0 root         (0) root         (0)     4293 2024-04-10 08:59:46.000000 gemsembler-0.6.3/tests/test_dbs.py
+-rw-rw-rw-   0 root         (0) root         (0)     4021 2024-04-10 08:59:46.000000 gemsembler-0.6.3/tests/test_gathering.py
+-rw-rw-rw-   0 root         (0) root         (0)     2357 2024-04-10 08:59:46.000000 gemsembler-0.6.3/tests/test_selection.py
```

### Comparing `gemsembler-0.6.2/LICENSE` & `gemsembler-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.2/PKG-INFO` & `gemsembler-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemsembler
-Version: 0.6.2
+Version: 0.6.3
 Summary: A tool for assembling and comparing several types of Genome-Scale Metabolic Models.
 Author-email: Elena Matveishina <elena.matveishina@embl.de>, Bartosz Bartmanski <bartosz.bartmanski@embl.de>
 License: MIT License
         
         Copyright (c) 2024 Zimmermann-Kogadeeva Group
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `gemsembler-0.6.2/README.md` & `gemsembler-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.2/pyproject.toml` & `gemsembler-0.6.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gemsembler"
-version = "0.6.2"
+version = "0.6.3"
 description = "A tool for assembling and comparing several types of Genome-Scale Metabolic Models."
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [
     { name = "Elena Matveishina", email = "elena.matveishina@embl.de" },
     { name = "Bartosz Bartmanski", email = "bartosz.bartmanski@embl.de" }
 ]
@@ -49,15 +49,15 @@
 include-package-data = true
 
 [tool.setuptools.packages.find]
 namespaces = true
 where = ["src"]
 
 [tool.bumpver]
-current_version = "0.6.2"
+current_version = "0.6.3"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `gemsembler-0.6.2/src/gemsembler/__init__.py` & `gemsembler-0.6.3/src/gemsembler/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from importlib.resources import files
 
 from .anticreation import get_model_of_interest
 from .creation import read_supermodel_from_pkl
 from .data import BU, LP
 from .gathering import GatheredModels, load_sbml_model
 
-__version__ = "0.6.2"
+__version__ = "0.6.3"
 
 lp_example = [
     dict(
         model_id="curated_LP",
         path_to_model=files(LP) / "LP_iLP728_revision_data_met_C_c.xml.gz",
         model_type="carveme",
         path_to_genome=files(LP) / "LP_protein_fasta.faa.gz",
```

### Comparing `gemsembler-0.6.2/src/gemsembler/__main__.py` & `gemsembler-0.6.3/src/gemsembler/__main__.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.2/src/gemsembler/anticreation.py` & `gemsembler-0.6.3/src/gemsembler/anticreation.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.2/src/gemsembler/comparison.py` & `gemsembler-0.6.3/src/gemsembler/comparison.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.2/src/gemsembler/conversion.py` & `gemsembler-0.6.3/src/gemsembler/conversion.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.2/src/gemsembler/creation.py` & `gemsembler-0.6.3/src/gemsembler/creation.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.2/src/gemsembler/curation.py` & `gemsembler-0.6.3/src/gemsembler/curation.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.2/src/gemsembler/data/BU/BU_agora.xml.gz` & `gemsembler-0.6.3/src/gemsembler/data/BU/BU_agora.xml.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.2/src/gemsembler/data/BU/BU_carveme_hom.xml.gz` & `gemsembler-0.6.3/src/gemsembler/data/BU/BU_carveme_hom.xml.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.2/src/gemsembler/data/BU/BU_gapseq.xml.gz` & `gemsembler-0.6.3/src/gemsembler/data/BU/BU_gapseq.xml.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.2/src/gemsembler/data/BU/BU_modelSEED.sbml.gz` & `gemsembler-0.6.3/src/gemsembler/data/BU/BU_modelSEED.sbml.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.2/src/gemsembler/data/LP/LP_CA1.xml.gz` & `gemsembler-0.6.3/src/gemsembler/data/LP/LP_CA1.xml.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.2/src/gemsembler/data/LP/LP_CA2.xml.gz` & `gemsembler-0.6.3/src/gemsembler/data/LP/LP_CA2.xml.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.2/src/gemsembler/data/LP/LP_MS2.sbml.gz` & `gemsembler-0.6.3/src/gemsembler/data/LP/LP_MS2.sbml.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.2/src/gemsembler/data/LP/LP_WCFS1.fasta.gz` & `gemsembler-0.6.3/src/gemsembler/data/LP/LP_WCFS1.fasta.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.2/src/gemsembler/data/LP/LP_WCFS1_agora.xml.gz` & `gemsembler-0.6.3/src/gemsembler/data/LP/LP_WCFS1_agora.xml.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.2/src/gemsembler/data/LP/LP_iLP728_revision_data_met_C_c.xml.gz` & `gemsembler-0.6.3/src/gemsembler/data/LP/LP_iLP728_revision_data_met_C_c.xml.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.2/src/gemsembler/data/LP/LP_protein_fasta.faa.gz` & `gemsembler-0.6.3/src/gemsembler/data/LP/LP_protein_fasta.faa.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.2/src/gemsembler/dbs.py` & `gemsembler-0.6.3/src/gemsembler/dbs.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.2/src/gemsembler/downstream.py` & `gemsembler-0.6.3/src/gemsembler/downstream.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -78,19 +78,19 @@
     output_name: str,
     pathway_r=None,
     yes_range=1,
     no_range=1,
     genes=True,
     and_as_solid=False,
 ):
+    if pathway_r is None:
+        pathway_r = list(supermodel.reactions.assembly.keys())
     output = {"Reaction": pathway_r, "R_confidence": [], "Status": [], "R_models": []}
     if genes:
         output.update({"GPR_confidence": [], "GPR_core": [], "GPR_assembly": []})
-    if pathway_r is None:
-        pathway_r = list(supermodel.reactions.assembly.keys())
     for r_id in pathway_r:
         if r_id in supermodel.reactions.assembly.keys():
             r = supermodel.reactions.assembly[r_id]
             output["R_confidence"].append(f"Core{r.in_models['models_amount']}")
             if r.in_models["models_amount"] >= len(supermodel.sources) - yes_range:
                 output["Status"].append("yes")
             elif r.in_models["models_amount"] <= no_range:
```

### Comparing `gemsembler-0.6.2/src/gemsembler/drawing.py` & `gemsembler-0.6.3/src/gemsembler/drawing.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.2/src/gemsembler/gathering.py` & `gemsembler-0.6.3/src/gemsembler/gathering.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.2/src/gemsembler/genes.py` & `gemsembler-0.6.3/src/gemsembler/genes.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.2/src/gemsembler/pathsfinding.py` & `gemsembler-0.6.3/src/gemsembler/pathsfinding.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.2/src/gemsembler/periplasmic.py` & `gemsembler-0.6.3/src/gemsembler/periplasmic.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.2/src/gemsembler/selection.py` & `gemsembler-0.6.3/src/gemsembler/selection.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.2/src/gemsembler/structural.py` & `gemsembler-0.6.3/src/gemsembler/structural.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.2/src/gemsembler.egg-info/PKG-INFO` & `gemsembler-0.6.3/src/gemsembler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemsembler
-Version: 0.6.2
+Version: 0.6.3
 Summary: A tool for assembling and comparing several types of Genome-Scale Metabolic Models.
 Author-email: Elena Matveishina <elena.matveishina@embl.de>, Bartosz Bartmanski <bartosz.bartmanski@embl.de>
 License: MIT License
         
         Copyright (c) 2024 Zimmermann-Kogadeeva Group
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `gemsembler-0.6.2/src/gemsembler.egg-info/SOURCES.txt` & `gemsembler-0.6.3/src/gemsembler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.2/tests/test_conversion.py` & `gemsembler-0.6.3/tests/test_conversion.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.2/tests/test_curation.py` & `gemsembler-0.6.3/tests/test_curation.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.2/tests/test_dbs.py` & `gemsembler-0.6.3/tests/test_dbs.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.2/tests/test_gathering.py` & `gemsembler-0.6.3/tests/test_gathering.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.2/tests/test_selection.py` & `gemsembler-0.6.3/tests/test_selection.py`

 * *Files identical despite different names*

