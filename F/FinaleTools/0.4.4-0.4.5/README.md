# Comparing `tmp/FinaleTools-0.4.4.tar.gz` & `tmp/FinaleTools-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FinaleTools-0.4.4.tar", last modified: Fri Apr  5 05:05:04 2024, max compression
+gzip compressed data, was "FinaleTools-0.4.5.tar", last modified: Tue Apr  9 22:08:31 2024, max compression
```

## Comparing `FinaleTools-0.4.4.tar` & `FinaleTools-0.4.5.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-05 05:05:04.000000 FinaleTools-0.4.4/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     1067 2024-03-29 01:22:35.000000 FinaleTools-0.4.4/LICENSE
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     5911 2024-04-05 05:05:04.000000 FinaleTools-0.4.4/PKG-INFO
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     3739 2024-04-01 20:34:46.000000 FinaleTools-0.4.4/README.md
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     1058 2024-04-05 04:59:24.000000 FinaleTools-0.4.4/pyproject.toml
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)       38 2024-04-05 05:05:04.000000 FinaleTools-0.4.4/setup.cfg
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-05 05:05:03.000000 FinaleTools-0.4.4/src/
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-05 05:05:03.000000 FinaleTools-0.4.4/src/FinaleTools.egg-info/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     5911 2024-04-05 05:05:03.000000 FinaleTools-0.4.4/src/FinaleTools.egg-info/PKG-INFO
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     1083 2024-04-05 05:05:03.000000 FinaleTools-0.4.4/src/FinaleTools.egg-info/SOURCES.txt
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)        1 2024-04-05 05:05:03.000000 FinaleTools-0.4.4/src/FinaleTools.egg-info/dependency_links.txt
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)       57 2024-04-05 05:05:03.000000 FinaleTools-0.4.4/src/FinaleTools.egg-info/entry_points.txt
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)      145 2024-04-05 05:05:03.000000 FinaleTools-0.4.4/src/FinaleTools.egg-info/requires.txt
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)       12 2024-04-05 05:05:03.000000 FinaleTools-0.4.4/src/FinaleTools.egg-info/top_level.txt
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-05 05:05:03.000000 FinaleTools-0.4.4/src/finaletools/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)        0 2023-06-21 12:51:49.000000 FinaleTools-0.4.4/src/finaletools/__init__.py
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-05 05:05:03.000000 FinaleTools-0.4.4/src/finaletools/cli/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)       38 2024-03-29 01:22:38.000000 FinaleTools-0.4.4/src/finaletools/cli/__init__.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)    24678 2024-04-04 19:34:39.000000 FinaleTools-0.4.4/src/finaletools/cli/main_cli.py
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-05 05:05:03.000000 FinaleTools-0.4.4/src/finaletools/frag/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)      509 2024-03-29 01:22:38.000000 FinaleTools-0.4.4/src/finaletools/frag/__init__.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     9664 2024-03-29 01:22:38.000000 FinaleTools-0.4.4/src/finaletools/frag/adjust_wps.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     4402 2024-03-29 01:22:38.000000 FinaleTools-0.4.4/src/finaletools/frag/agg_wps.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     9329 2024-03-29 01:49:46.000000 FinaleTools-0.4.4/src/finaletools/frag/cleavage_profile.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     7546 2024-04-04 20:18:22.000000 FinaleTools-0.4.4/src/finaletools/frag/coverage.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)    14488 2024-04-01 20:23:25.000000 FinaleTools-0.4.4/src/finaletools/frag/delfi.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     3973 2024-03-29 01:22:38.000000 FinaleTools-0.4.4/src/finaletools/frag/delfi_gc_correct.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     2080 2024-04-01 20:23:25.000000 FinaleTools-0.4.4/src/finaletools/frag/delfi_merge_bins.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)    14184 2024-04-04 19:21:37.000000 FinaleTools-0.4.4/src/finaletools/frag/end_motifs.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)    14865 2024-03-29 02:06:16.000000 FinaleTools-0.4.4/src/finaletools/frag/frag_length.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     8466 2024-03-29 02:06:16.000000 FinaleTools-0.4.4/src/finaletools/frag/multi_wps.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     6797 2024-03-29 01:49:46.000000 FinaleTools-0.4.4/src/finaletools/frag/wps.py
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-05 05:05:03.000000 FinaleTools-0.4.4/src/finaletools/genome/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)       37 2024-03-29 01:22:39.000000 FinaleTools-0.4.4/src/finaletools/genome/__init__.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)    14339 2024-03-29 01:22:39.000000 FinaleTools-0.4.4/src/finaletools/genome/gaps.py
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-05 05:05:03.000000 FinaleTools-0.4.4/src/finaletools/methylation/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)        0 2024-03-29 01:22:39.000000 FinaleTools-0.4.4/src/finaletools/methylation/__init__.py
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-05 05:05:03.000000 FinaleTools-0.4.4/src/finaletools/qc/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)        0 2024-03-29 01:22:39.000000 FinaleTools-0.4.4/src/finaletools/qc/__init__.py
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-05 05:05:03.000000 FinaleTools-0.4.4/src/finaletools/too/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)        0 2024-03-29 01:22:39.000000 FinaleTools-0.4.4/src/finaletools/too/__init__.py
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-05 05:05:04.000000 FinaleTools-0.4.4/src/finaletools/utils/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)       90 2024-03-29 01:22:39.000000 FinaleTools-0.4.4/src/finaletools/utils/__init__.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     1649 2024-03-29 01:22:39.000000 FinaleTools-0.4.4/src/finaletools/utils/cli_hist.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     3917 2024-03-29 01:22:39.000000 FinaleTools-0.4.4/src/finaletools/utils/filter_bam.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)    18301 2024-04-04 20:13:31.000000 FinaleTools-0.4.4/src/finaletools/utils/utils.py
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-09 22:08:31.000000 FinaleTools-0.4.5/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     1067 2024-03-29 01:22:35.000000 FinaleTools-0.4.5/LICENSE
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     5911 2024-04-09 22:08:26.000000 FinaleTools-0.4.5/PKG-INFO
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     3739 2024-04-01 20:34:46.000000 FinaleTools-0.4.5/README.md
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     1058 2024-04-09 22:05:26.000000 FinaleTools-0.4.5/pyproject.toml
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)       38 2024-04-09 22:08:31.000000 FinaleTools-0.4.5/setup.cfg
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-09 22:07:29.000000 FinaleTools-0.4.5/src/
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-09 22:07:58.000000 FinaleTools-0.4.5/src/FinaleTools.egg-info/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     5911 2024-04-09 22:07:18.000000 FinaleTools-0.4.5/src/FinaleTools.egg-info/PKG-INFO
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     1083 2024-04-09 22:07:29.000000 FinaleTools-0.4.5/src/FinaleTools.egg-info/SOURCES.txt
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)        1 2024-04-09 22:07:29.000000 FinaleTools-0.4.5/src/FinaleTools.egg-info/dependency_links.txt
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)       57 2024-04-09 22:07:29.000000 FinaleTools-0.4.5/src/FinaleTools.egg-info/entry_points.txt
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)      145 2024-04-09 22:07:29.000000 FinaleTools-0.4.5/src/FinaleTools.egg-info/requires.txt
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)       12 2024-04-09 22:07:29.000000 FinaleTools-0.4.5/src/FinaleTools.egg-info/top_level.txt
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-09 22:07:58.000000 FinaleTools-0.4.5/src/finaletools/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)        0 2023-06-21 12:51:49.000000 FinaleTools-0.4.5/src/finaletools/__init__.py
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-09 22:07:58.000000 FinaleTools-0.4.5/src/finaletools/cli/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)       38 2024-03-29 01:22:38.000000 FinaleTools-0.4.5/src/finaletools/cli/__init__.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)    24767 2024-04-05 16:25:39.000000 FinaleTools-0.4.5/src/finaletools/cli/main_cli.py
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-09 22:08:13.000000 FinaleTools-0.4.5/src/finaletools/frag/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)      509 2024-03-29 01:22:38.000000 FinaleTools-0.4.5/src/finaletools/frag/__init__.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     9664 2024-03-29 01:22:38.000000 FinaleTools-0.4.5/src/finaletools/frag/adjust_wps.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     4402 2024-03-29 01:22:38.000000 FinaleTools-0.4.5/src/finaletools/frag/agg_wps.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     9329 2024-03-29 01:49:46.000000 FinaleTools-0.4.5/src/finaletools/frag/cleavage_profile.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     7549 2024-04-09 22:05:01.000000 FinaleTools-0.4.5/src/finaletools/frag/coverage.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)    14488 2024-04-01 20:23:25.000000 FinaleTools-0.4.5/src/finaletools/frag/delfi.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     3973 2024-03-29 01:22:38.000000 FinaleTools-0.4.5/src/finaletools/frag/delfi_gc_correct.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     2080 2024-04-01 20:23:25.000000 FinaleTools-0.4.5/src/finaletools/frag/delfi_merge_bins.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)    24836 2024-04-09 22:02:56.000000 FinaleTools-0.4.5/src/finaletools/frag/end_motifs.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)    14865 2024-03-29 02:06:16.000000 FinaleTools-0.4.5/src/finaletools/frag/frag_length.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     8466 2024-03-29 02:06:16.000000 FinaleTools-0.4.5/src/finaletools/frag/multi_wps.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     6797 2024-03-29 01:49:46.000000 FinaleTools-0.4.5/src/finaletools/frag/wps.py
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-09 22:08:13.000000 FinaleTools-0.4.5/src/finaletools/genome/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)       37 2024-03-29 01:22:39.000000 FinaleTools-0.4.5/src/finaletools/genome/__init__.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)    14339 2024-03-29 01:22:39.000000 FinaleTools-0.4.5/src/finaletools/genome/gaps.py
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-09 22:08:13.000000 FinaleTools-0.4.5/src/finaletools/methylation/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)        0 2024-03-29 01:22:39.000000 FinaleTools-0.4.5/src/finaletools/methylation/__init__.py
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-09 22:08:13.000000 FinaleTools-0.4.5/src/finaletools/qc/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)        0 2024-03-29 01:22:39.000000 FinaleTools-0.4.5/src/finaletools/qc/__init__.py
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-09 22:08:13.000000 FinaleTools-0.4.5/src/finaletools/too/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)        0 2024-03-29 01:22:39.000000 FinaleTools-0.4.5/src/finaletools/too/__init__.py
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-09 22:08:20.000000 FinaleTools-0.4.5/src/finaletools/utils/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)       90 2024-03-29 01:22:39.000000 FinaleTools-0.4.5/src/finaletools/utils/__init__.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     1649 2024-03-29 01:22:39.000000 FinaleTools-0.4.5/src/finaletools/utils/cli_hist.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     3917 2024-03-29 01:22:39.000000 FinaleTools-0.4.5/src/finaletools/utils/filter_bam.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)    18436 2024-04-05 05:11:54.000000 FinaleTools-0.4.5/src/finaletools/utils/utils.py
```

### Comparing `FinaleTools-0.4.4/LICENSE` & `FinaleTools-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `FinaleTools-0.4.4/PKG-INFO` & `FinaleTools-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FinaleTools
-Version: 0.4.4
+Version: 0.4.5
 Summary: A package and standalone program to process paired-end reads of cfDNA fragment WGS.
 Author-email: James Li <lijw21@wfu.edu>, Yaping Liu <yaping@northwestern.edu>
 License: MIT License
         
         Copyright (c) 2024 EpiFluidLab
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `FinaleTools-0.4.4/README.md` & `FinaleTools-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `FinaleTools-0.4.4/pyproject.toml` & `FinaleTools-0.4.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 include-package-data = true
 
 [project]
 name = "FinaleTools"
-version = "0.4.4"
+version = "0.4.5"
 authors = [
     {name="James Li", email="lijw21@wfu.edu"},
     {name="Yaping Liu", email="yaping@northwestern.edu"},
 ]
 description = "A package and standalone program to process paired-end reads of cfDNA fragment WGS."
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `FinaleTools-0.4.4/src/FinaleTools.egg-info/PKG-INFO` & `FinaleTools-0.4.5/src/FinaleTools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FinaleTools
-Version: 0.4.4
+Version: 0.4.5
 Summary: A package and standalone program to process paired-end reads of cfDNA fragment WGS.
 Author-email: James Li <lijw21@wfu.edu>, Yaping Liu <yaping@northwestern.edu>
 License: MIT License
         
         Copyright (c) 2024 EpiFluidLab
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `FinaleTools-0.4.4/src/FinaleTools.egg-info/SOURCES.txt` & `FinaleTools-0.4.5/src/FinaleTools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FinaleTools-0.4.4/src/finaletools/cli/main_cli.py` & `FinaleTools-0.4.5/src/finaletools/cli/main_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 from finaletools.genome.gaps import _cli_gap_bed
 
 # TODO: implement subcommands read from stdin
 # TODO: implement pipelining
 
 def main_cli_parser():
     parser = argparse.ArgumentParser(
-        description='Calculates fragmentation features given a CRAM/BAM/SAM '
-        'file',
+        description='Calculates fragmentation features given a CRAM, BAM, SAM,'
+        ' or Frag.gz file.',
         epilog='')
     subparsers = parser.add_subparsers(title='subcommands',
                                        dest='subcommand')
 
     # Common arguments
 
     # Subcommand 1: frag-coverage
@@ -147,16 +147,16 @@
         help='Verbose logging.'
     )
     parser_command2.set_defaults(func=_cli_frag_length)
 
     # Subcommand 3: frag_length_bins()
     parser_command3 = subparsers.add_parser(
         'frag-length-bins', prog='finaletools-frag-length-bins',
-        description='computes frag lengths of fragments and either prints'
-        'bins and counts to tsv or prints a histogram'
+        description='computes frag lengths of fragments and agregates in bins '
+        'by length. Either writes bins and counts to tsv or prints a histogram'
         )
     parser_command3.add_argument(
         'input_file',
         help='BAM or SAM file containing fragment data'
     )
     parser_command3.add_argument(
         '-c',
@@ -228,15 +228,16 @@
         help='Verbose logging.'
     )
     parser_command3.set_defaults(func=frag_length_bins)
 
     # Subcommand 3_1: frag_length_intervals
     parser_command3_1 = subparsers.add_parser(
         'frag-length-intervals',
-        description='Calculates frag lengths statistics for intervals'
+        description='Calculates frag lengths statistics over user-specified '
+        'genomic intervals.'
     )
     parser_command3_1.add_argument(
         'input_file',
         help='BAM or SAM file containing PE WGS of cfDNA'
     )
     parser_command3_1.add_argument(
         'interval_file',
@@ -285,15 +286,15 @@
 
     # Subcommand 4: wps (on interval bed file)
     parser_command4 = subparsers.add_parser(
         'wps',
         prog='finaletools-wps',
         description='Calculates Windowed Protection Score over a region '
         'around sites specified in a BED file from alignments in a '
-        'CRAM/BAM/SAM file'
+        'CRAM/BAM/SAM/Frag.gz file'
     )
     parser_command4.add_argument(
         'input_file',
         help='bam or sam file containing paired-end reads of cfDNA WGS'
     )
     parser_command4.add_argument(
         'site_bed',
```

### Comparing `FinaleTools-0.4.4/src/finaletools/frag/adjust_wps.py` & `FinaleTools-0.4.5/src/finaletools/frag/adjust_wps.py`

 * *Files identical despite different names*

### Comparing `FinaleTools-0.4.4/src/finaletools/frag/agg_wps.py` & `FinaleTools-0.4.5/src/finaletools/frag/agg_wps.py`

 * *Files identical despite different names*

### Comparing `FinaleTools-0.4.4/src/finaletools/frag/cleavage_profile.py` & `FinaleTools-0.4.5/src/finaletools/frag/cleavage_profile.py`

 * *Files identical despite different names*

### Comparing `FinaleTools-0.4.4/src/finaletools/frag/coverage.py` & `FinaleTools-0.4.5/src/finaletools/frag/coverage.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,15 +224,15 @@
                             f'{coverage/total_coverage[4]*scale_factor}\n'
                         )
                 else:
                     for contig, start, stop, name, coverage in coverages:
                         output.write(
                             f'{contig}\t{start}\t{stop}\t'
                             f'{name}\t'
-                            f'{coverage/total_coverage*scale_factor}\n'
+                            f'{coverage/total_coverage[4]*scale_factor}\n'
                         )
 
             finally:
                 if output_is_file:
                     output.close()
     finally:
         pool.close()
```

### Comparing `FinaleTools-0.4.4/src/finaletools/frag/delfi.py` & `FinaleTools-0.4.5/src/finaletools/frag/delfi.py`

 * *Files identical despite different names*

### Comparing `FinaleTools-0.4.4/src/finaletools/frag/delfi_gc_correct.py` & `FinaleTools-0.4.5/src/finaletools/frag/delfi_gc_correct.py`

 * *Files identical despite different names*

### Comparing `FinaleTools-0.4.4/src/finaletools/frag/delfi_merge_bins.py` & `FinaleTools-0.4.5/src/finaletools/frag/delfi_merge_bins.py`

 * *Files identical despite different names*

### Comparing `FinaleTools-0.4.4/src/finaletools/frag/end_motifs.py` & `FinaleTools-0.4.5/src/finaletools/frag/end_motifs.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 from collections.abc import Iterator
-from typing import Union, Iterable
+from typing import Union, Iterable, Tuple
 from multiprocessing import Pool
 from time import time
 from sys import stderr, stdout, stdin
 import gzip
 try:
     from importlib.resources import files
 except ImportError:
@@ -13,15 +13,15 @@
 from collections import UserDict
 
 import tqdm
 import py2bit
 import numpy as np
 from numpy.typing import NDArray
 
-from finaletools.utils.utils import frag_generator
+from finaletools.utils.utils import frag_generator, _get_intervals
 import finaletools.frag as pkg_data
 
 # path to tsv containing f-profiles from Zhou et al (2023)
 FPROFILE_PATH: Path = (files(pkg_data) / 'data' / 'end_motif_f_profiles.tsv')
 
 # quality threshold used by Jiang et al (2020)
 MIN_QUALITY: int = 20
@@ -34,20 +34,16 @@
     Parameters
     ----------
     kmer_frequencies : Iterable
         A Iterable of tuples, each containing a str representing a k-mer
         and a float representing its frequency
     k : int
         Size of k-mers
-    refseq_file: str
-        A 2bit file containing the reference sequence that cfDNA
-        fragments were aligned to
     quality_threshold: int, optional
         Minimum mapping quality used. Default is 30.
-
     """
 
     def __init__(
         self,
         kmer_frequencies: Iterable[tuple[str, float]],
         k: int,
         quality_threshold: int = MIN_QUALITY,
@@ -175,14 +171,190 @@
                 )
         finally:
             if is_file:
                 file.close()
         return cls(freq_list, k, quality_threshold)
 
 
+class EndMotifsIntervals():
+    """
+    Class that stores frequencies of end-motif k-mers over
+    user-specified intervals and contains methods to manipulate this
+    data.
+
+    Parameters
+    ----------
+    intervals : Iterable
+        A collection of tuples, each containing a tuple representing
+        a genomic interval (chrom, 0-based start, 1-based stop) and a
+        dict that maps kmers to frequencies in the interval.
+    k : int
+        Size of k-mers
+    quality_threshold: int, optional
+        Minimum mapping quality used. Default is 30.
+    """
+
+    def __init__(
+        self,
+        intervals: Iterable[tuple[tuple, dict]],
+        k: int,
+        quality_threshold: int = MIN_QUALITY,
+    ):
+        self.intervals = intervals
+        self.k = k
+        self.quality_threshold = quality_threshold
+        if not all(len(freqs) == 4**k for _, freqs in intervals):
+            raise ValueError(
+                'bins contains results for kmer with length not equal'
+                ' to k.'
+            )
+
+    def __iter__(self) -> Iterator:
+        return (interval for interval in self.intervals)
+
+    def __len__(self) -> int:
+        return self.intervals.__len__()
+
+    def __str__(self) -> str:
+        return f'EndMotifsIntervals over {len(self.intervals)} intervals.'
+
+    def freq(self, kmer: str) -> list[Tuple[str, int, int, float]]:
+        """
+        Returns a list of intervals and associated frquency for given
+        kmer. Results are in the form (chrom, 0-based start, 1-based
+        stop, frequency).
+        """
+        return dict(
+            [(*interval, freq[kmer]) for interval, freq in self.intervals]
+        )
+
+    def motif_diversity_score(self) -> list[tuple[tuple, float]]:
+        """
+        Calculates a motif diversity score (MDS) for each interval using
+        normalized Shannon entropy as described by Jiang et al (2020). This
+        function is generalized for any k instead of just 4-mers.
+        """
+        num_kmers = 4**self.k
+        mds = []
+        for interval, kmers in self.intervals:
+            freq = np.array(kmers.values())
+            interval_mds = np.sum(-freq*np.log(freq)/np.log(num_kmers))
+        mds.append((interval, interval_mds))
+
+        return mds
+    
+    def to_tsv(self, output_file: str, calc_freq: bool=True, sep: str='\t'):
+        """
+        Writes all intervals and associated frquencies to file.
+        
+        Parameters
+        ----------
+        output_file: str
+            File to write frequencies to.
+        calc_freq: bool, optional
+            Calculates frequency of motifs if true. Otherwise, writes counts
+            for each motif. Default is true.
+        sep: str, optional
+            Separator for table. Tab-separated by default.
+        """
+        if type(output_file) == str:
+            try:
+                # open file based on name
+                output_is_file = False
+                if output_file == '-':
+                    output = stdout
+                else:
+                    output_is_file = True
+                    output = open(output_file, 'w')
+
+                # write to file
+                kmers = _gen_kmers(self.k, 'ACGT')
+                # header
+                output.write(sep.join(['contig','start','stop','count',*kmers]))
+                output.write('\n')
+                # data
+                for interval, freqs in self.intervals:
+                    count = sum(freqs.values())
+                    output.write(
+                        sep.join([
+                            interval[0],
+                            str(interval[1]),
+                            str(interval[2]),
+                            str(count), 
+                            *([str(freq) for freq in freqs.values()]
+                             if not calc_freq
+                             else [f"{(freq/count):.6f}"
+                                   if count!=0
+                                   else "NaN" 
+                                for freq
+                                in freqs.values()])
+                        ])
+                    )
+                    output.write('\n')
+
+            finally:
+                if output_is_file:
+                    output.close()
+        else:
+            raise TypeError(f'output_file must be a string.')
+    
+    def to_bedgraph(
+            self,
+            kmer: str,
+            output_file: str,
+            calc_freq: bool=True,
+            sep: str='\t'
+        ):
+        """
+        Take frequency of specified kmer and writes to BED.
+        
+        Parameters
+        ----------
+        output_file: str
+            File to write frequencies to.
+        calc_freq: bool, optional
+            Calculates frequency of motifs if true. Otherwise, writes counts
+            for each motif. Default is true.
+        sep: str, optional
+            Separator for table. Tab-separated by default.
+        """
+        if type(output_file) == str:
+            try:
+                # open file based on name
+                output_is_file = False
+                if output_file == '-':
+                    output = stdout
+                else:
+                    output_is_file = True
+                    output = open(output_file, 'w')
+
+                # write to file
+                for interval, freqs in self.intervals:
+                    count = sum(freqs.values())
+                    output.write(
+                        sep.join([
+                            interval[0],
+                            str(interval[1]),
+                            str(interval[2]),
+                            (self.freq[kmer] if not calc_freq
+                             else f"{(freqs[kmer]/count):.6f}"
+                                if count!=0
+                                else "NaN"
+                            )
+                        ])
+                    )
+                    output.write('\n')
+
+            finally:
+                if output_is_file:
+                    output.close()
+        else:
+            raise TypeError(f'output_file must be a string.')
+
+
 def _gen_kmers(k: int, bases: str) -> list:
         """Function to recursively create a list of k-mers."""
         if k == 1:
             return [base for base in bases]
         else:
             kmers = []
             for k_minus_mer in _gen_kmers(k-1, bases):
@@ -206,41 +378,56 @@
     contig: str,
     start: int,
     stop: int,
     refseq_file: str,
     k: int = 4,
     fraction_low: int = 10,
     fraction_high: int = 600,
-    both_strands: bool = False,
-    output_file: Union(None, str) = None,
+    both_strands: bool = True,
+    output_file: Union[None, str] = None,
     quality_threshold: int = MIN_QUALITY,
-    verbose: Union(bool, int) = False,
+    verbose: Union[bool, int] = False,
 ) -> dict:
     """
     Function that reads fragments in the specified region from a BAM,
     SAM, or tabix indexed file and returns the 5' k-mer (default is
-    4-mer) end motif counts as a structured array. This function
+    4-mer) end motif counts as a dictionary. This function
     reproduces the methodology of Zhou et al (2023).
 
     Parameters
     ----------
     input_file : str
+        Path of SAM, BAM, CRAM, or Frag.gz containing pair-end reads.
     contig : str
+        Name of contig or chromosome for region.
     start : int
+        0-based start coordinate.
     stop : int
+        1-based end coordinate.
     refseq_file : str
+        2bit file with reference sequence `input_file` was aligned to.
     k : int, optional
+        Length of end motif kmer. Default is 4.
+    fraction_low: int, optional
+        Minimum fragment length.
+    fraction_high: int, optional
+        Maximum fragment length.
+    both_strands: bool, optional
+        Choose whether to use forward 5' ends only or use 5' ends for
+        both ends of PE reads.
     output_file : None or str, optional
     quality_threshold : int, optional
     verbose : bool or int, optional
 
     Return
     ------
     end_motif_freq : dict
     """
+    # NOTE: consider renaming to interval_end_motif
+
     if verbose:
         start_time = time()
 
     # iterable of fragments
     frag_ends = frag_generator(
         input_file,
         contig,
@@ -305,15 +492,16 @@
                     try:
                         reverse_kmer = refseq.sequence(
                             contig, int(frag[2]-k), int(frag[2])
                         )
                         assert len(reverse_kmer) == k
 
                         if 'N' not in reverse_kmer:
-                            end_motif_counts[_reverse_complement(reverse_kmer)] += 1
+                            rc_reverse_kmer = _reverse_complement(reverse_kmer)
+                            end_motif_counts[rc_reverse_kmer] += 1
                     except RuntimeError:
                         if verbose > 1:
                             stderr.write(
                                 f'Attempt to read interval at {contig}:'
                                 f'{int(frag[2]-k)}-{int(frag[2])} failed.'
                                 'Skipping.')
                         continue
@@ -326,50 +514,62 @@
         stderr.write(
             f'region_end_motifs took {stop_time-start_time} seconds to run\n'
         )
 
     return end_motif_counts
 
 
-def _region_end_motifs_star(args) -> NDArray:
+def _region_end_motifs_star(args) -> dict:
     results_dict = region_end_motifs(*args)
     return np.array(list(results_dict.values()), dtype='<f8')
 
 
+def _region_end_motifs_dict_star(args) -> dict:
+    results_dict = region_end_motifs(*args)
+    return results_dict
+
+
 def end_motifs(
     input_file: str,
     refseq_file: str,
     k: int = 4,
     fraction_low: int = 10,
     fraction_high: int = 600,
     both_strands: bool = False,
-    output_file: Union(None, str) = None,
+    output_file: Union[None, str] = None,
     quality_threshold: int = 30,
     workers: int = 1,
-    verbose: Union(bool, int) = False,
+    verbose: Union[bool, int] = False,
 ) -> EndMotifFreqs:
     """
     Function that reads fragments from a BAM, SAM, or tabix indexed
     file and returns the 5' k-mer (default is 4-mer) end motif
     frequencies as a dictionary. Optionally writes data to a tsv. This
     function reproduces the methodology of Zhou et al (2023).
 
     Parameters
     ----------
     input_file : str
+        SAM, BAM, CRAM, or Frag.gz file with paired-end reads.
     refseq_file : str
+        2bit file with sequence of reference genome input_file is
+        aligned to.
     k : int, optional
+        Length of end motif kmer. Default is 4.
     output_file : None or str, optional
+        File path to write results to. Either tsv or csv.
     quality_threshold : int, optional
+        Minimum MAPQ to filter.
     workers : int, optional
+        Number of worker processes.
     verbose : bool or int, optional
 
     Return
     ------
-    end_motif_freq : list
+    end_motif_freq : EndMotifFreqs
     """
     if verbose:
         start_time = time()
 
     bases='ACGT'
     kmer_list = _gen_kmers(k, bases)
 
@@ -442,14 +642,139 @@
     )
 
     if output_file is not None:
         if output_file.endswith('.csv'):
             results.to_tsv(output_file, sep=',')
         else:
             results.to_tsv(output_file)
+
+    if verbose:
+        stop_time = time()
+        tqdm.tqdm.write(
+            f'end_motifs took {stop_time-start_time} seconds to run\n'
+        )
+
+    return results
+
+
+def interval_end_motifs(
+    input_file: str,
+    refseq_file: str,
+    intervals: Union[str, list[Tuple[str,int,int]]],
+    k: int = 4,
+    fraction_low: int = 10,
+    fraction_high: int = 600,
+    both_strands: bool = True,
+    output_file: Union[None, str] = None,
+    quality_threshold: int = 30,
+    workers: int = 1,
+    verbose: Union[bool, int] = False,
+) -> EndMotifFreqs:
+    """
+    Function that reads fragments from a BAM, SAM, or tabix indexed
+    file and user-specified intervals and returns the 5' k-mer
+    (default is 4-mer) end motif. Optionally writes data to a tsv.
+
+    Parameters
+    ----------
+    input_file : str
+        Path of SAM, BAM, CRAM, or Frag.gz containing pair-end reads.
+    refseq_file : str
+        Path of 2bit file for reference genome that reads are aligned to.
+    intervals : str or tuple
+        Path of BED file containing intervals or list of tuples
+        (chrom, start, stop).
+    k : int, optional
+        Length of end motif kmer. Default is 4.
+    output_file : None or str, optional
+        File path to write results to. Either tsv or csv.
+    quality_threshold : int, optional
+        Minimum MAPQ to filter.
+    workers : int, optional
+        Number of worker processes.
+    verbose : bool or int, optional
+
+    Return
+    ------
+    end_motif_freq : EndMotifIntervals
+    """
+    if verbose:
+        start_time = time()
+
+    bases='ACGT'
+    kmer_list = _gen_kmers(k, bases)
+
+    # read chromosomes from py2bit
+    try:
+        refseq = py2bit.open(refseq_file, 'r')
+        chroms: dict = refseq.chroms()
+    finally:
+        refseq.close()
+
+    # generate list of inputs
+    if type(intervals) is str:
+        with open(intervals, 'r') as interval_file:
+            intervals_tuples = [
+                (chrom, int(start), int(stop))
+                for chrom, start, stop, *_
+                in [line.split() for line in interval_file.readlines()]
+                ]
+    elif type(intervals) is tuple:
+        intervals_tuples = intervals
+    else:
+        raise TypeError("Intervals should be string or tuple.")
+    
+    mp_intervals = []   # args to be fed into pool processes
+    for chrom, start, stop in intervals_tuples:
+        mp_intervals.append((
+            input_file,
+            chrom,
+            start,
+            stop,
+            refseq_file,
+            k,
+            fraction_low,
+            fraction_high,
+            both_strands,
+            None,
+            quality_threshold,
+            verbose - 2 if verbose > 2 else 0
+        )
+    )
+
+    # use process pool to aggregate kmers
+    try:
+        # open pool
+        pool = Pool(workers)
+
+        # uses tqdm loading bar if verbose == True
+        counts_iter = pool.imap(
+            _region_end_motifs_dict_star,
+            tqdm.tqdm(
+                mp_intervals,
+                'Reading intervals',
+                position=0) if verbose else mp_intervals,
+            chunksize=min(int(len(intervals)/workers/2+1), 1000)
+        )
+
+    finally:
+        pool.close()
+    results = EndMotifsIntervals(
+        [(interval, counts)
+         for interval, counts
+         in zip(intervals_tuples, counts_iter)],
+         k,
+         quality_threshold,
+    )
+
+    if output_file is not None:
+        if output_file.endswith('.csv'):
+            results.to_tsv(output_file, sep=',')
+        else:
+            results.to_tsv(output_file)
 
     if verbose:
         stop_time = time()
         tqdm.tqdm.write(
             f'end_motifs took {stop_time-start_time} seconds to run\n'
         )
```

### Comparing `FinaleTools-0.4.4/src/finaletools/frag/frag_length.py` & `FinaleTools-0.4.5/src/finaletools/frag/frag_length.py`

 * *Files identical despite different names*

### Comparing `FinaleTools-0.4.4/src/finaletools/frag/multi_wps.py` & `FinaleTools-0.4.5/src/finaletools/frag/multi_wps.py`

 * *Files identical despite different names*

### Comparing `FinaleTools-0.4.4/src/finaletools/frag/wps.py` & `FinaleTools-0.4.5/src/finaletools/frag/wps.py`

 * *Files identical despite different names*

### Comparing `FinaleTools-0.4.4/src/finaletools/genome/gaps.py` & `FinaleTools-0.4.5/src/finaletools/genome/gaps.py`

 * *Files identical despite different names*

### Comparing `FinaleTools-0.4.4/src/finaletools/utils/cli_hist.py` & `FinaleTools-0.4.5/src/finaletools/utils/cli_hist.py`

 * *Files identical despite different names*

### Comparing `FinaleTools-0.4.4/src/finaletools/utils/filter_bam.py` & `FinaleTools-0.4.5/src/finaletools/utils/filter_bam.py`

 * *Files identical despite different names*

### Comparing `FinaleTools-0.4.4/src/finaletools/utils/utils.py` & `FinaleTools-0.4.5/src/finaletools/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -426,16 +426,21 @@
 
 def _get_intervals(
     input_file: Union[str, pysam.AlignmentFile],
     interval_file: str,
     intersect_policy: str,
     quality_threshold: int,
     verbose: Union[bool, int]
-) -> list[Tuple[str,str,int,int,str,str,int,int]]:
-    """Helper function to read intervals from bed file."""
+) -> list[Tuple[str, str, int, int, str, str, int]]:
+    """
+    Helper function to read intervals from bed file.
+    Returns list of tuples:
+    (input_file, chrom, start, stop, name, intersect_policy,
+    quality_threshold, verbosity)
+    """
     intervals = []  # list of inputs for single_coverage
 
     with open(interval_file) as bed:
         for line in bed:
             if ~line.startswith('#'):
                 if line != '':
                     contig, start, stop, *name = line.split()
```

