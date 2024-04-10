# Comparing `tmp/sniffles-2.2.tar.gz` & `tmp/sniffles-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sniffles-2.2.tar", last modified: Thu Jul 27 18:10:34 2023, max compression
+gzip compressed data, was "sniffles-2.3.tar", last modified: Wed Apr 10 13:38:48 2024, max compression
```

## Comparing `sniffles-2.2.tar` & `sniffles-2.3.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxrwxr-x   0 lpaz      (1000) lpaz      (1000)        0 2023-07-27 18:10:34.749090 sniffles-2.2/
--rw-rw-r--   0 lpaz      (1000) lpaz      (1000)     1070 2023-03-26 18:37:33.000000 sniffles-2.2/LICENSE
--rw-rw-r--   0 lpaz      (1000) lpaz      (1000)     4486 2023-07-27 18:10:34.749090 sniffles-2.2/PKG-INFO
--rw-rw-r--   0 lpaz      (1000) lpaz      (1000)     3905 2023-07-27 17:54:14.000000 sniffles-2.2/README.md
--rw-rw-r--   0 lpaz      (1000) lpaz      (1000)      104 2023-03-26 18:37:33.000000 sniffles-2.2/pyproject.toml
--rw-rw-r--   0 lpaz      (1000) lpaz      (1000)      775 2023-07-27 18:10:34.753089 sniffles-2.2/setup.cfg
-drwxrwxr-x   0 lpaz      (1000) lpaz      (1000)        0 2023-07-27 18:10:34.749090 sniffles-2.2/src/
-drwxrwxr-x   0 lpaz      (1000) lpaz      (1000)        0 2023-07-27 18:10:34.749090 sniffles-2.2/src/sniffles/
--rw-rw-r--   0 lpaz      (1000) lpaz      (1000)      190 2023-03-26 18:37:33.000000 sniffles-2.2/src/sniffles/__init__.py
--rw-rw-r--   0 lpaz      (1000) lpaz      (1000)    14161 2023-07-06 18:59:06.000000 sniffles-2.2/src/sniffles/cluster.py
--rw-rw-r--   0 lpaz      (1000) lpaz      (1000)    23091 2023-07-06 16:32:31.000000 sniffles-2.2/src/sniffles/config.py
--rw-rw-r--   0 lpaz      (1000) lpaz      (1000)    15172 2023-07-06 16:58:35.000000 sniffles-2.2/src/sniffles/consensus.py
--rwxr-xr-x   0 lpaz      (1000) lpaz      (1000)    24947 2023-03-26 18:37:33.000000 sniffles-2.2/src/sniffles/leadprov.py
--rw-rw-r--   0 lpaz      (1000) lpaz      (1000)    15210 2023-03-26 18:37:33.000000 sniffles-2.2/src/sniffles/parallel.py
--rw-rw-r--   0 lpaz      (1000) lpaz      (1000)    17006 2023-03-26 18:37:33.000000 sniffles-2.2/src/sniffles/postprocessing.py
--rw-rw-r--   0 lpaz      (1000) lpaz      (1000)     5108 2023-03-26 18:37:33.000000 sniffles-2.2/src/sniffles/snf.py
--rwxr-xr-x   0 lpaz      (1000) lpaz      (1000)    26976 2023-07-06 17:01:28.000000 sniffles-2.2/src/sniffles/sniffles
--rwxr-xr-x   0 lpaz      (1000) lpaz      (1000)    19538 2023-03-26 18:37:33.000000 sniffles-2.2/src/sniffles/sv.py
--rw-rw-r--   0 lpaz      (1000) lpaz      (1000)     3283 2023-03-26 18:37:33.000000 sniffles-2.2/src/sniffles/util.py
--rwxr-xr-x   0 lpaz      (1000) lpaz      (1000)    15909 2023-03-26 18:37:33.000000 sniffles-2.2/src/sniffles/vcf.py
-drwxrwxr-x   0 lpaz      (1000) lpaz      (1000)        0 2023-07-27 18:10:34.749090 sniffles-2.2/src/sniffles.egg-info/
--rw-rw-r--   0 lpaz      (1000) lpaz      (1000)     4486 2023-07-27 18:10:34.000000 sniffles-2.2/src/sniffles.egg-info/PKG-INFO
--rw-rw-r--   0 lpaz      (1000) lpaz      (1000)      502 2023-07-27 18:10:34.000000 sniffles-2.2/src/sniffles.egg-info/SOURCES.txt
--rw-rw-r--   0 lpaz      (1000) lpaz      (1000)        1 2023-07-27 18:10:34.000000 sniffles-2.2/src/sniffles.egg-info/dependency_links.txt
--rw-rw-r--   0 lpaz      (1000) lpaz      (1000)       14 2023-07-27 18:10:34.000000 sniffles-2.2/src/sniffles.egg-info/requires.txt
--rw-rw-r--   0 lpaz      (1000) lpaz      (1000)        9 2023-07-27 18:10:34.000000 sniffles-2.2/src/sniffles.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:38:48.434989 sniffles-2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-10 13:38:44.000000 sniffles-2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5237 2024-04-10 13:38:48.434989 sniffles-2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4366 2024-04-10 13:38:44.000000 sniffles-2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-10 13:38:44.000000 sniffles-2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-10 13:38:48.434989 sniffles-2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-10 13:38:44.000000 sniffles-2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:38:48.426989 sniffles-2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:38:48.430989 sniffles-2.3/src/sniffles/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-10 13:38:44.000000 sniffles-2.3/src/sniffles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13915 2024-04-10 13:38:44.000000 sniffles-2.3/src/sniffles/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26870 2024-04-10 13:38:44.000000 sniffles-2.3/src/sniffles/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15746 2024-04-10 13:38:44.000000 sniffles-2.3/src/sniffles/consensus.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    25903 2024-04-10 13:38:44.000000 sniffles-2.3/src/sniffles/leadprov.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24149 2024-04-10 13:38:44.000000 sniffles-2.3/src/sniffles/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17736 2024-04-10 13:38:44.000000 sniffles-2.3/src/sniffles/postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-10 13:38:44.000000 sniffles-2.3/src/sniffles/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9839 2024-04-10 13:38:44.000000 sniffles-2.3/src/sniffles/snf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21199 2024-04-10 13:38:44.000000 sniffles-2.3/src/sniffles/sniffles
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24081 2024-04-10 13:38:44.000000 sniffles-2.3/src/sniffles/sv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-04-10 13:38:44.000000 sniffles-2.3/src/sniffles/util.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18412 2024-04-10 13:38:44.000000 sniffles-2.3/src/sniffles/vcf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:38:48.430989 sniffles-2.3/src/sniffles.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5237 2024-04-10 13:38:48.000000 sniffles-2.3/src/sniffles.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-10 13:38:48.000000 sniffles-2.3/src/sniffles.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 13:38:48.000000 sniffles-2.3/src/sniffles.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-10 13:38:48.000000 sniffles-2.3/src/sniffles.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-10 13:38:48.000000 sniffles-2.3/src/sniffles.egg-info/top_level.txt
```

### Comparing `sniffles-2.2/LICENSE` & `sniffles-2.3/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 MIT License
 
-Copyright (c) 2021 Moritz Smolka
+Copyright (c)
+    2021- Moritz Smolka
+    2023- Hermann Romanek
+
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `sniffles-2.2/PKG-INFO` & `sniffles-2.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: sniffles
-Version: 2.2
-Summary: A fast structural variation caller for long-read sequencing data
-Home-page: https://github.com/fritzsedlazeck/Sniffles
-Author: Moritz Smolka, Luis Paulin
-Author-email: moritz.g.smolka@gmail.com, lfpaulin@gmail.com
-Project-URL: Bug Tracker, https://github.com/fritzsedlazeck/Sniffles/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Sniffles2
 A fast structural variant caller for long-read sequencing, Sniffles2 accurately detect SVs on germline, somatic and population-level for PacBio and Oxford Nanopore read data.
 
 ## Quick Start: Germline SV calling using Sniffles2
 To call SVs from long read alignments (PacBio / ONT), you can use:
 
 `sniffles -i mapped_input.bam -v output.vcf`
@@ -28,35 +13,47 @@
 ## Installation
 You can install Sniffles2 using pip or conda using:
 
 `pip install sniffles`
 
 or
 
-`conda install sniffles=2.0 `
+`conda install sniffles=2.3`
 
 If you previously installed Sniffles1 using conda and want to upgrade to Sniffles2, you can use:
 
-`conda update sniffles=2.2`
+`conda update sniffles=2.3`
 
 ## Requirements
-* Python >= 3.8
-* pysam
+* Python >= 3.10
+* pysam >= 0.21.0
+
+### Optional requirements
+
+* edlib
+
+  If edlib is installed alignments are enabled by default during multi-sample SV/combine calling. This can be further tweaked (or disabled) with the `--combine-pctseq` argument. 
+
+* psutil
+
+  psutil can be used to facilitaty population calling with a large number of input files. 
 
 #### Tested on:
-* python==3.9.5
-* pysam==0.16.0.1
+* python==3.10.12
+* pysam==0.21.0
 
 ## Citation
 Please cite our paper at:
+Sniffles v2: 
+https://www.nature.com/articles/s41587-023-02024-y
 
+and 
+Sniffles v1:
 https://www.nature.com/articles/s41592-018-0001-7
 
-A new preprint for the new methods and improvements introduced with Sniffles2 is here: https://www.biorxiv.org/content/10.1101/2022.04.04.487055v1
-
 ## Use-Cases / Modes
 
 ### A. General (all Modes)
 * To output deletion (DEL SV) sequences, the reference genome (.fasta) must be specified using e.g. `--reference reference.fasta`.
 * Sniffles2 supports optionally specifying tandem repeat region annotations (.bed), which can improve calling in these regions `--tandem-repeats annotations.bed`. Sniffles2 compatible tandem repeat annotations for human references can be found in the [annotations/ folder](https://github.com/fritzsedlazeck/Sniffles/tree/master/annotations).
 * Sniffles2 is fully parallelized and uses 4 threads by default. This value can be adapted using e.g. `--threads 4` as option. Memory requirements will increase with the number of threads used.
 * To output read names in SNF and VCF files, the `--output-rnames` option is required.
@@ -86,7 +83,10 @@
 * .bam or .cram files containing long read alignments (i.e. from minimap2 or ngmlr) are supported as input
 * .vcf.gz (bgzipped+tabix indexed) output is supported
 * Simultaneous output of both .vcf and .snf file (for multi-sample calling) is supported
 
 ## Companion apps
 * We have developed a plotting tools for Sniffles2: [https://github.com/farhangus/sniffle2_plot](https://github.com/farhangus/sniffle2_plot)
 * We also provide VCF and scripts used for the manuscript [https://github.com/smolkmo/Sniffles2-Supplement](https://github.com/smolkmo/Sniffles2-Supplement) 
+
+## Supplementary tables
+[https://github.com/smolkmo/Sniffles2-Supplement/blob/main/Supplemetary%20tables.xlsx](https://github.com/smolkmo/Sniffles2-Supplement/blob/main/Supplemetary%20tables.xlsx)
```

### Comparing `sniffles-2.2/setup.cfg` & `sniffles-2.3/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = sniffles
-version = 2.2
-author = Moritz Smolka, Luis Paulin
-author_email = moritz.g.smolka@gmail.com, lfpaulin@gmail.com
+version = 2.3
+author = Moritz Smolka, Hermann Romanek
+author_email = moritz.g.smolka@gmail.com, sniffles@romanek.at
 description = A fast structural variation caller for long-read sequencing data
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/fritzsedlazeck/Sniffles
 project_urls = 
 	Bug Tracker = https://github.com/fritzsedlazeck/Sniffles/issues
 classifiers = 
@@ -14,20 +14,29 @@
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
 	= src
 packages = find:
-python_requires = >=3.8
+python_requires = >=3.10
 install_requires = 
-	pysam>=0.20.0
+	pysam>=0.21.0
 scripts = 
 	src/sniffles/sniffles
 
+[options.extras_require]
+align = 
+	edlib>=1.3.9
+mem = 
+	psutil>=5.9.4
+all = 
+	edlib>=1.3.9
+	psutil>=5.9.4
+
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `sniffles-2.2/src/sniffles/cluster.py` & `sniffles-2.3/src/sniffles/cluster.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,353 +1,343 @@
 #!/usr/bin/env python3
 #
 # Sniffles2
 # A fast structural variant caller for long-read sequencing data
 #
-# Created: 29.08.2021
-# Author:  Moritz Smolka
-# Contact: moritz.g.smolka@gmail.com
+# Created:     29.08.2021
+# Author:      Moritz Smolka
+# Maintainer:  Hermann Romanek
+# Contact:     sniffles@romanek.at
 #
 
 from dataclasses import dataclass
 import statistics
 import math
+from typing import Optional
 
 from sniffles import sv
 from sniffles import leadprov
 
+
 @dataclass
 class Cluster:
     id: str
     svtype: str
     contig: str
     start: int
     end: int
     seed: int
     leads: list
     repeat: bool
-    leads_long: list
-
-    def compute_metrics(self,max_n=100):
-        self.span=self.end-self.start
+    leads_long: Optional[list]
 
-        n=min(len(self.leads),max_n)
-        if n==0:
-            self.mean_svlen=0
-            self.stdev_start=0
+    @property
+    def span(self) -> Optional[int]:
+        if self.end is None or self.start is None:
+            return None
+
+        return self.end - self.start
+
+    def compute_metrics(self, max_n=100):
+        n = min(len(self.leads), max_n)
+        if n == 0:
+            self.mean_svlen = 0
+            self.stdev_start = 0
             return
 
-        # REVIEW: might need fix based on issue #407
-        step=int(len(self.leads)/n)
-        if n>1:
-            self.mean_svlen=sum(self.leads[i].svlen for i in range(0,len(self.leads),step))/float(n)
-            self.stdev_start=statistics.stdev(self.leads[i].ref_start for i in range(0,len(self.leads),step))
+        step = int(len(self.leads) / n)
+        if n > 1:
+            self.mean_svlen = sum(self.leads[i].svlen for i in range(0, len(self.leads), step)) / float(n)
+            self.stdev_start = statistics.stdev(self.leads[i].ref_start for i in range(0, len(self.leads), step))
         else:
-            self.mean_svlen=self.leads[0].svlen
-            self.stdev_start=0
+            self.mean_svlen = self.leads[0].svlen
+            self.stdev_start = 0
+
 
-def merge_inner(cluster,threshold):
-    read_seq={}
+def merge_inner(cluster, threshold):
+    read_seq = {}
     for ld in cluster.leads:
-        if not ld.read_qname in read_seq:
-            read_seq[ld.read_qname]=[]
+        if ld.read_qname not in read_seq:
+            read_seq[ld.read_qname] = []
         read_seq[ld.read_qname].append(ld)
 
-    cluster.leads=[]
+    cluster.leads = []
     for qname in read_seq:
         read_seq[qname].sort(key=lambda k: k.ref_start)
-        to_merge=read_seq[qname][0]
+        to_merge = read_seq[qname][0]
 
-        curr_lead=to_merge
+        curr_lead = to_merge
 
-        last_ref_end=to_merge.ref_end
-        last_qry_end=to_merge.qry_end
-        last_ref_start=to_merge.ref_start
-        last_qry_start=to_merge.qry_start
+        last_ref_end = to_merge.ref_end
+        last_qry_end = to_merge.qry_end
+        last_ref_start = to_merge.ref_start
+        last_qry_start = to_merge.qry_start
 
         for to_merge in read_seq[qname][1:]:
-            merge=(threshold==-1) or ((abs(to_merge.ref_start-last_ref_end) < threshold or abs(to_merge.ref_start-last_ref_start) < threshold) and (abs(to_merge.qry_start-last_qry_end) < threshold or abs(to_merge.qry_start-last_qry_start) < threshold))
+            merge = (threshold == -1) or ((abs(to_merge.ref_start - last_ref_end) < threshold or abs(to_merge.ref_start - last_ref_start) < threshold) and (
+                        abs(to_merge.qry_start - last_qry_end) < threshold or abs(to_merge.qry_start - last_qry_start) < threshold))
             if merge:
-                curr_lead.svlen+=to_merge.svlen
-                if to_merge.seq==None or curr_lead.seq==None:
-                    curr_lead.seq=None
+                curr_lead.svlen += to_merge.svlen
+                if to_merge.seq is None or curr_lead.seq is None:
+                    curr_lead.seq = None
                 else:
-                    curr_lead.seq+=to_merge.seq
+                    curr_lead.seq += to_merge.seq
             else:
                 cluster.leads.append(curr_lead)
-                curr_lead=to_merge
-            last_ref_end=to_merge.ref_end
-            last_qry_end=to_merge.qry_end
-            last_ref_start=to_merge.ref_start
-            last_qry_start=to_merge.qry_start
+                curr_lead = to_merge
+            last_ref_end = to_merge.ref_end
+            last_qry_end = to_merge.qry_end
+            last_ref_start = to_merge.ref_start
+            last_qry_start = to_merge.qry_start
 
         cluster.leads.append(curr_lead)
     return cluster
 
-def resplit(cluster,prop,binsize,merge_threshold_min,merge_threshold_frac):
-    bins_leads={}
+
+def resplit(cluster, prop, binsize, merge_threshold_min, merge_threshold_frac):
+    bins_leads = {}
     for lead in cluster.leads:
-        bin=int(abs(prop(lead))/binsize)*binsize
+        bin = int(abs(prop(lead)) / binsize) * binsize
         if not bin in bins_leads:
-            bins_leads[bin]=[lead]
+            bins_leads[bin] = [lead]
         else:
             bins_leads[bin].append(lead)
 
-    new_clusters=list(sorted(bins_leads.keys()))
-    i=1
+    new_clusters = list(sorted(bins_leads.keys()))
+    i = 1
     while len(new_clusters) > 1 and i < len(new_clusters):
-        last_cluster=new_clusters[i-1]
-        curr_cluster=new_clusters[i]
-        merge_threshold=max(merge_threshold_min,min(curr_cluster,last_cluster)*merge_threshold_frac)
-        merge=abs(curr_cluster - last_cluster) <= merge_threshold
+        last_cluster = new_clusters[i - 1]
+        curr_cluster = new_clusters[i]
+        merge_threshold = max(merge_threshold_min, min(curr_cluster, last_cluster) * merge_threshold_frac)
+        merge = abs(curr_cluster - last_cluster) <= merge_threshold
         if merge:
-            bins_leads[new_clusters[i]].extend(bins_leads[new_clusters[i-1]])
-            new_clusters.pop(i-1)
-            i=max(0,i-2)
+            bins_leads[new_clusters[i]].extend(bins_leads[new_clusters[i - 1]])
+            new_clusters.pop(i - 1)
+            i = max(0, i - 2)
         else:
-            i+=1
+            i += 1
 
     for cluster_index in new_clusters:
-        new_cluster=Cluster(id=cluster.id+f".{cluster_index}",
-                            svtype=cluster.svtype,
-                            contig=cluster.contig,
-                            start=cluster.start,
-                            end=cluster.end,
-                            seed=cluster.seed,
-                            leads=bins_leads[cluster_index],
-                            repeat=cluster.repeat,
-                            leads_long=cluster.leads_long)
+        new_cluster = Cluster(id=cluster.id + f".{cluster_index}",
+                              svtype=cluster.svtype,
+                              contig=cluster.contig,
+                              start=cluster.start,
+                              end=cluster.end,
+                              seed=cluster.seed,
+                              leads=bins_leads[cluster_index],
+                              repeat=cluster.repeat,
+                              leads_long=cluster.leads_long)
         yield new_cluster
 
-def resplit_bnd(cluster,merge_threshold):
-    contigs_leads={}
 
-    #Split by mate contig and mate ref start
+def resplit_bnd(cluster, merge_threshold):
+    contigs_leads = {}
+
+    # Split by mate contig and mate ref start
     for lead in cluster.leads:
         if not lead.bnd_info.mate_contig in contigs_leads:
-            contigs_leads[lead.bnd_info.mate_contig]={}
+            contigs_leads[lead.bnd_info.mate_contig] = {}
 
-        bin=int(lead.bnd_info.mate_ref_start/merge_threshold)*merge_threshold if merge_threshold>0 else 0
+        bin = int(lead.bnd_info.mate_ref_start / merge_threshold) * merge_threshold if merge_threshold > 0 else 0
         if not bin in contigs_leads[lead.bnd_info.mate_contig]:
-            contigs_leads[lead.bnd_info.mate_contig][bin]=[lead]
+            contigs_leads[lead.bnd_info.mate_contig][bin] = [lead]
         else:
             contigs_leads[lead.bnd_info.mate_contig][bin].append(lead)
 
     for contig in contigs_leads:
-        bins=sorted(contigs_leads[contig])
-        curr_leads=[]+contigs_leads[contig][bins[0]]
-        last_bin=bins[0]
+        bins = sorted(contigs_leads[contig])
+        curr_leads = [] + contigs_leads[contig][bins[0]]
+        last_bin = bins[0]
         for bin in bins[1:]:
             if bin - last_bin <= merge_threshold:
                 curr_leads.extend(contigs_leads[contig][bin])
             else:
                 if len(curr_leads):
-                    new_cluster=Cluster(id=cluster.id+f".CHR2.{contig}.POS2.{bin}",
-                                        svtype=cluster.svtype,
-                                        contig=cluster.contig,
-                                        start=cluster.start,
-                                        end=cluster.end,
-                                        seed=cluster.seed,
-                                        leads=[k for k in curr_leads],
-                                        repeat=cluster.repeat,
-                                        leads_long=None)
+                    new_cluster = Cluster(id=cluster.id + f".CHR2.{contig}.POS2.{bin}",
+                                          svtype=cluster.svtype,
+                                          contig=cluster.contig,
+                                          start=cluster.start,
+                                          end=cluster.end,
+                                          seed=cluster.seed,
+                                          leads=[k for k in curr_leads],
+                                          repeat=cluster.repeat,
+                                          leads_long=None)
                     yield new_cluster
-                curr_leads=[]+contigs_leads[contig][bin]
-            last_bin=bin
+                curr_leads = [] + contigs_leads[contig][bin]
+            last_bin = bin
         if len(curr_leads):
-            new_cluster=Cluster(id=cluster.id+f".CHR2.{contig}.POS2.{bin}",
-                                svtype=cluster.svtype,
-                                contig=cluster.contig,
-                                start=cluster.start,
-                                end=cluster.end,
-                                seed=cluster.seed,
-                                leads=[k for k in curr_leads],
-                                repeat=cluster.repeat,
-                                leads_long=None)
-            curr_leads=[]
+            new_cluster = Cluster(id=cluster.id + f".CHR2.{contig}.POS2.{bin}",
+                                  svtype=cluster.svtype,
+                                  contig=cluster.contig,
+                                  start=cluster.start,
+                                  end=cluster.end,
+                                  seed=cluster.seed,
+                                  leads=[k for k in curr_leads],
+                                  repeat=cluster.repeat,
+                                  leads_long=None)
+            curr_leads = []
             yield new_cluster
 
-def resolve(svtype,leadtab_provider,config,tr):
-    leadtab=leadtab_provider.leadtab[svtype]
-    seeds=sorted(leadtab_provider.leadtab[svtype])
 
-    if len(seeds)==0:
+def resolve(svtype, leadtab_provider, config, tr):
+    leadtab = leadtab_provider.leadtab[svtype]
+    seeds = sorted(leadtab_provider.leadtab[svtype])
+
+    if len(seeds) == 0:
         return []
 
-    #Initialize tandem repeat region handling
-    if tr != None:
-        tr_index=0
-        if len(tr)==0:
-            tr=None
+    # Initialize tandem repeat region handling
+    if tr is not None:
+        tr_index = 0
+        if len(tr) == 0:
+            tr = None
         else:
-            tr_start,tr_end=tr[tr_index]
+            tr_start, tr_end = tr[tr_index]
 
-    clusters=[]
-    for seed_index,seed in enumerate(seeds):
+    clusters = []
+    for seed_index, seed in enumerate(seeds):
         if config.dev_call_region != None:
-            if seed<config.dev_call_region["start"] or seed>config.dev_call_region["end"]:
+            if seed < config.dev_call_region["start"] or seed > config.dev_call_region["end"]:
                 continue
 
-        within_tr=False
-        if tr!=None and tr_index < len(tr):
-            while tr_end < seed and tr_index+1 < len(tr):
-                tr_index+=1
-                tr_start,tr_end=tr[tr_index]
-            if seed > tr_start and seed < tr_end:
-                within_tr=True
-
-        if svtype=="INS":
-            leads=[lead for lead in leadtab[seed] if lead.svlen!=None]
-            leads_long=[lead for lead in leadtab[seed] if lead.svlen==None]
+        within_tr = False
+        if tr is not None and tr_index < len(tr):
+            while tr_end < seed and tr_index + 1 < len(tr):
+                tr_index += 1
+                tr_start, tr_end = tr[tr_index]
+            if tr_start < seed < tr_end:
+                within_tr = True
+
+        if svtype == "INS":
+            leads = [lead for lead in leadtab[seed] if lead.svlen != None]
+            leads_long = [lead for lead in leadtab[seed] if lead.svlen == None]
         else:
-            leads=leadtab[seed]
-            leads_long=None
+            leads = leadtab[seed]
+            leads_long = None
 
-        cluster=Cluster(id=f"CL.{svtype}.{leadtab_provider.contig}.{leadtab_provider.start}.{seed_index}",
-                        svtype=svtype,
-                        contig=leadtab_provider.contig,
-                        start=seed,
-                        end=seed+config.cluster_binsize,
-                        seed=seed,
-                        leads=leads,
-                        repeat=within_tr or config.repeat,
-                        leads_long=leads_long)
+        cluster = Cluster(id=f"CL.{svtype}.{leadtab_provider.contig}.{leadtab_provider.start}.{seed_index}",
+                          svtype=svtype,
+                          contig=leadtab_provider.contig,
+                          start=seed,
+                          end=seed + config.cluster_binsize,
+                          seed=seed,
+                          leads=leads,
+                          repeat=within_tr or config.repeat,
+                          leads_long=leads_long)
 
         cluster.compute_metrics()
         clusters.append(cluster)
 
-
-    #Merge clusters
-    cluster_count_initial=len(clusters)
-    i=0
+    # Merge clusters
+    cluster_count_initial = len(clusters)
+    i = 0
     while i < len(clusters) - 1:
-        curr_cluster=clusters[i]
-        next_cluster=clusters[i+1]
+        curr_cluster = clusters[i]
+        next_cluster = clusters[i + 1]
 
-        #assert((next_cluster.end - curr_cluster.start) >= 0)
-        #assert((next_cluster.start - curr_cluster.end) >= 0)
+        # assert((next_cluster.end - curr_cluster.start) >= 0)
+        # assert((next_cluster.start - curr_cluster.end) >= 0)
 
-        #Fast Adaptive Scanning Clustering
+        # Fast Adaptive Scanning Clustering
         #  Inter-Cluster distance < (StdDev-Start-Within-A + StdDev-Stat-Within-B) * r   (r=1.0 default)
         #  Merged size (OR: Inter-cluster distance) < (MeanSVlen between both clusters) * h (h=0.5 default)
         #  Max. overall cluster size criterion?
 
-        inner_dist=(next_cluster.start - curr_cluster.end)
-        outer_dist=(next_cluster.end - curr_cluster.start)
+        inner_dist = (next_cluster.start - curr_cluster.end)
+        outer_dist = (next_cluster.end - curr_cluster.start)
         merge = inner_dist <= min(curr_cluster.stdev_start, next_cluster.stdev_start) * config.cluster_r
-        merge = merge or ( (config.repeat or curr_cluster.repeat or next_cluster.repeat) and outer_dist <= min(config.cluster_repeat_h_max, (abs(curr_cluster.mean_svlen)+abs(next_cluster.mean_svlen)) * config.cluster_repeat_h) )
-        merge = merge or (svtype=="BND" and inner_dist <= config.cluster_merge_bnd)
+        merge = merge or ((config.repeat or curr_cluster.repeat or next_cluster.repeat) and outer_dist <= min(config.cluster_repeat_h_max,
+                                                                                                              (abs(curr_cluster.mean_svlen) + abs(next_cluster.mean_svlen)) * config.cluster_repeat_h))
+        merge = merge or (svtype == "BND" and inner_dist <= config.cluster_merge_bnd)
 
         if merge:
-            clusters.pop(i+1)
-            curr_cluster.leads+=next_cluster.leads
-            if svtype=="INS":
-                curr_cluster.leads_long+=next_cluster.leads_long
-            curr_cluster.end=next_cluster.end
-            curr_cluster.repeat=curr_cluster.repeat or next_cluster.repeat
+            clusters.pop(i + 1)
+            curr_cluster.leads += next_cluster.leads
+            if svtype == "INS":
+                curr_cluster.leads_long += next_cluster.leads_long
+            curr_cluster.end = next_cluster.end
+            curr_cluster.repeat = curr_cluster.repeat or next_cluster.repeat
             curr_cluster.compute_metrics()
-            i=max(0,i-2)
-        i+=1
+            i = max(0, i - 2)
+        i += 1
 
     if config.dev_trace_read:
         for c in clusters:
             for ld in c.leads:
-                if ld.read_qname==config.dev_trace_read:
+                if ld.read_qname == config.dev_trace_read:
                     print(f"[DEV_TRACE_READ [2/4] [cluster.resolve] Read lead {ld} is in cluster {c.id}, containing a total of {len(c.leads)} leads")
 
     if config.dev_dump_clusters:
-        filename=f"{config.input}.clusters.{svtype}.{leadtab_provider.contig}.{leadtab_provider.start}.{leadtab_provider.end}.bed"
+        filename = f"{config.input}.clusters.{svtype}.{leadtab_provider.contig}.{leadtab_provider.start}.{leadtab_provider.end}.bed"
         print(f"Dumping clusters to {filename}")
-        with open(filename,"w") as h:
+        with open(filename, "w") as h:
             for c in clusters:
-                info=f"ID={c.id}, #LEADS={len(c.leads)}; "
+                info = f"ID={c.id}, #LEADS={len(c.leads)}; "
                 for ld in c.leads:
-                    info+=f"(ref_start={ld.ref_start},svlen={ld.svlen},source={ld.source}); "
+                    info += f"(ref_start={ld.ref_start},svlen={ld.svlen},source={ld.source}); "
                 h.write(f"{c.contig}\t{c.start}\t{c.end}\t\"{info}\"\n")
 
     for cluster in clusters:
-        if len(cluster.leads)==0:
+        if len(cluster.leads) == 0:
             continue
 
         if svtype == "BND":
             if config.dev_no_resplit:
                 yield cluster
             else:
-                for new_cluster in resplit_bnd(cluster,merge_threshold=config.cluster_merge_bnd):
+                for new_cluster in resplit_bnd(cluster, merge_threshold=config.cluster_merge_bnd):
                     yield new_cluster
         else:
-            if svtype=="INS" or svtype=="DEL":
+            if svtype == "INS" or svtype == "DEL":
                 if cluster.repeat:
-                    merge_inner_threshold=-1
+                    merge_inner_threshold = -1
                 else:
-                    merge_inner_threshold=config.cluster_merge_pos
+                    merge_inner_threshold = config.cluster_merge_pos
 
-                merge_inner(cluster,merge_inner_threshold)
+                merge_inner(cluster, merge_inner_threshold)
 
             if not config.dev_no_resplit_repeat and not config.dev_no_resplit:
                 for new_cluster in resplit(cluster,
                                            prop=lambda lead: lead.svlen,
                                            binsize=config.cluster_resplit_binsize,
                                            merge_threshold_min=config.minsvlen,
                                            merge_threshold_frac=config.cluster_merge_len):
                     yield new_cluster
             else:
                 yield cluster
 
-def resolve_block_groups(svtype,svcands,groups_initial,config):
+
+def resolve_block_groups(svtype, svcands, groups_initial, config):
     """For clustering groups of SVs for combining .snfs (multi-call)"""
 
-    #TODO: Remove sorting
-    groups=groups_initial
-    for svcand in sorted(svcands,key=lambda cand: cand.support,reverse=True):
-        best_group=None
-        best_dist=math.inf
+    # TODO: Remove sorting
+    groups = groups_initial
+    for svcand in sorted(svcands, key=lambda cand: cand.support, reverse=True):
+        best_group = None
+        best_dist = math.inf
 
-        if svtype=="BND":
-            mate_contig,mate_ref_start=svcand.bnd_info.mate_contig,svcand.bnd_info.mate_ref_start
+        if svtype == "BND":
+            mate_contig, mate_ref_start = svcand.bnd_info.mate_contig, svcand.bnd_info.mate_ref_start
             for group in groups:
-                #TODO: Favor bigger groups in placement
-                dist=abs(group.pos_mean - svcand.pos) + abs(group.bnd_mate_ref_start_mean - mate_ref_start)
-                if dist < best_dist and dist <= config.cluster_merge_bnd*2 and group.bnd_mate_contig==mate_contig:
-                    if not config.combine_separate_intra or not svcand.sample_internal_id in group.included_samples:
-                        best_group=group
-                        best_dist=dist
+                # TODO: Favor bigger groups in placement
+                dist = abs(group.pos_mean - svcand.pos) + abs(group.bnd_mate_ref_start_mean - mate_ref_start)
+                if dist < best_dist and dist <= config.cluster_merge_bnd * 2 and group.bnd_mate_contig == mate_contig:
+                    if not config.combine_separate_intra or svcand.sample_internal_id not in group.included_samples:
+                        best_group = group
+                        best_dist = dist
         else:
             for group in groups:
-                #TODO: Favor bigger groups in placement
-                dist=abs(group.pos_mean - svcand.pos) + abs(abs(group.len_mean) - abs(svcand.svlen))
-                minlen=float(min(abs(group.len_mean),abs(svcand.svlen)))
-                if minlen>0 and dist < best_dist and dist <= config.combine_match * math.sqrt(minlen) and dist <= config.combine_match_max:
-                    if not config.combine_separate_intra or not svcand.sample_internal_id in group.included_samples:
-                        best_group=group
-                        best_dist=dist
-
-        if best_group==None:
-            group=sv.SVGroup(candidates=[svcand],
-                             pos_mean=float(svcand.pos),
-                             len_mean=float(abs(svcand.svlen)),
-                             included_samples=set([svcand.sample_internal_id]),
-                             coverages_nonincluded=dict())
-            if svtype=="BND":
-                group.bnd_mate_contig=mate_contig
-                group.bnd_mate_ref_start_mean=mate_ref_start
-            groups.append(group)
+                # TODO: Favor bigger groups in placement
+                dist = abs(group.pos_mean - svcand.pos) + abs(abs(group.len_mean) - abs(svcand.svlen))  # check if group.pos_mean is updated or stays the same for the first SV starting the group
+                minlen = float(min(abs(group.len_mean), abs(svcand.svlen)))
+                if minlen > 0 and dist < best_dist and dist <= config.combine_match * math.sqrt(minlen) and dist <= config.combine_match_max:
+                    if (not config.combine_separate_intra or svcand.sample_internal_id not in group.included_samples) and group.align_call(svcand, config.combine_pctseq):
+                        best_group = group
+                        best_dist = dist
+
+        if best_group is None:
+            groups.append(
+                sv.SVGroup.from_candidate(svcand)
+            )
         else:
-            group_size=len(best_group.candidates)
-            best_group.pos_mean*=group_size
-            best_group.len_mean*=group_size
-            best_group.pos_mean+=svcand.pos
-            best_group.len_mean+=abs(svcand.svlen)
-            if svtype=="BND":
-                best_group.bnd_mate_ref_start_mean*=group_size
-                best_group.bnd_mate_ref_start_mean+=mate_ref_start
-
-            best_group.candidates.append(svcand)
-            group_size+=1
-            best_group.pos_mean/=group_size
-            best_group.len_mean/=group_size
-            best_group.included_samples.add(svcand.sample_internal_id)
-
-            if svtype=="BND":
-                best_group.bnd_mate_ref_start_mean/=group_size
-
+            best_group.add_candidate(svcand)
     return groups
```

### Comparing `sniffles-2.2/src/sniffles/consensus.py` & `sniffles-2.3/src/sniffles/consensus.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,390 +1,394 @@
 #!/usr/bin/env python3
 #
 # Sniffles2
 # A fast structural variant caller for long-read sequencing data
 #
-# Created: 09.09.2021
-# Author:  Moritz Smolka
-# Contact: moritz.g.smolka@gmail.com
+# Created:     09.09.2021
+# Author:      Moritz Smolka
+# Maintainer:  Hermann Romanek
+# Contact:     sniffles@romanek.at
 #
 
 from dataclasses import dataclass
 import collections
 
 from sniffles import util
 
+
 @dataclass
 class Group:
     """
     A sequence to which other sequences are pseudoaligned (mappings) through exact kmer matches (anchors)
     Can be reduced to a consensus sequence using the flatten() method
     """
     anchors: dict
     mappings: dict
     consensus_min: int
     consensus_max: int
     start_len: int
     origin: object
     support: list
 
-    def flatten(self,frameshift_origin=False,return_debug=False):
-        override_origin_min=3
-        override_origin_indel_ratio=0.6
-
-        consensus=""
-        origin_space_consensus=""
-        ins_consensus=""
-        del_consensus=""
-        mappings_consensus=""
-        skip_until=self.consensus_min-1
-        for ci in range(self.consensus_min,self.consensus_max+1,1):
-            if not ci in self.mappings:
-                origin_space_consensus+="-"
-                ins_consensus+="-"
-                del_consensus+="-"
-                mappings_consensus+="-"
+    def flatten(self, frameshift_origin=False, return_debug=False):
+        override_origin_min = 3
+        override_origin_indel_ratio = 0.6
+
+        consensus = ""
+        origin_space_consensus = ""
+        ins_consensus = ""
+        del_consensus = ""
+        mappings_consensus = ""
+        skip_until = self.consensus_min - 1
+        for ci in range(self.consensus_min, self.consensus_max + 1, 1):
+            if ci not in self.mappings:
+                origin_space_consensus += "-"
+                ins_consensus += "-"
+                del_consensus += "-"
+                mappings_consensus += "-"
                 continue
-            type_fragments={"M":[], "I":[], "D":[]}
-            type_fragments_counts={"M":0, "I":0, "D":0}
+            type_fragments = {"M": [], "I": [], "D": []}
+            type_fragments_counts = {"M": 0, "I": 0, "D": 0}
             for maptype, maplen, map_last_i, map_i, map_j, map_lead in self.mappings[ci]:
-                type_fragments[maptype].append((maplen,map_lead.seq[map_last_i:map_i]))
-                type_fragments_counts[maptype]+=1
+                type_fragments[maptype].append((maplen, map_lead.seq[map_last_i:map_i]))
+                type_fragments_counts[maptype] += 1
 
-            type_consensus=sorted(type_fragments, key=lambda t: len(type_fragments[t]))[-1]
-            assert(len(type_fragments[type_consensus])>0)
+            type_consensus = sorted(type_fragments, key=lambda t: len(type_fragments[t]))[-1]
+            assert (len(type_fragments[type_consensus]) > 0)
 
-            #Favor match over I/D when ratio is below 2
+            # Favor match over I/D when ratio is below 2
 
-            if type_consensus=="I" and type_fragments_counts["M"]>0 and type_fragments_counts["I"] / float(type_fragments_counts["M"]+type_fragments_counts["I"]) < override_origin_indel_ratio:
-                type_consensus="N"
+            if type_consensus == "I" and type_fragments_counts["M"] > 0 and type_fragments_counts["I"] / float(type_fragments_counts["M"] + type_fragments_counts["I"]) < override_origin_indel_ratio:
+                type_consensus = "N"
 
-            if type_consensus=="D" and type_fragments_counts["M"]>0 and type_fragments_counts["D"] / float(type_fragments_counts["M"]+type_fragments_counts["D"]) < override_origin_indel_ratio:
-                type_consensus="N"
+            if type_consensus == "D" and type_fragments_counts["M"] > 0 and type_fragments_counts["D"] / float(type_fragments_counts["M"] + type_fragments_counts["D"]) < override_origin_indel_ratio:
+                type_consensus = "N"
 
-            if type_consensus=="M":
-                #print(type_fragments_seq)
+            if type_consensus == "M":
+                # print(type_fragments_seq)
                 if len(type_fragments[type_consensus]) < 3:
-                    #Favor original sequence when only two mappings present
-                    maplen,seq=type_fragments[type_consensus][0]
-                    common_base,count=seq[0],1
+                    # Favor original sequence when only two mappings present
+                    maplen, seq = type_fragments[type_consensus][0]
+                    common_base, count = seq[0], 1
                 else:
-                    common_base,count=collections.Counter(seq[0] for maplen,seq in type_fragments[type_consensus]).most_common(1)[0]
+                    common_base, count = collections.Counter(seq[0] for maplen, seq in type_fragments[type_consensus]).most_common(1)[0]
 
                 if ci > skip_until:
-                    consensus+=common_base
-                    origin_space_consensus+=common_base
+                    consensus += common_base
+                    origin_space_consensus += common_base
                 else:
-                    origin_space_consensus+="-"
-                ins_consensus+="-"
-                del_consensus+="-"
-                mappings_consensus+=str(min(9,count))
-
-            elif type_consensus=="N":
-                #Favor original sequence when only two mappings present
-                maplen,seq=type_fragments["M"][0]
-                common_base,count=seq[0],1
+                    origin_space_consensus += "-"
+                ins_consensus += "-"
+                del_consensus += "-"
+                mappings_consensus += str(min(9, count))
+
+            elif type_consensus == "N":
+                # Favor original sequence when only two mappings present
+                maplen, seq = type_fragments["M"][0]
+                common_base, count = seq[0], 1
 
                 if ci > skip_until:
-                    consensus+=common_base
-                    origin_space_consensus+=common_base
+                    consensus += common_base
+                    origin_space_consensus += common_base
                 else:
-                    origin_space_consensus+="-"
-                ins_consensus+="-"
-                del_consensus+="-"
-                mappings_consensus+=str(min(9,count))
-
-            elif frameshift_origin and type_consensus=="I":
-                common_maplen,count=collections.Counter(maplen for maplen,seq in type_fragments[type_consensus]).most_common(1)[0]
-                common_seqlen,count=collections.Counter(len(seq) for maplen,seq in type_fragments[type_consensus] if maplen==common_maplen).most_common(1)[0]
-                origin_space_consensus+="^"
-                ins_consensus+=str(min(9,maplen))
-                del_consensus+="-"
-                mappings_consensus+=str(min(9,count))
+                    origin_space_consensus += "-"
+                ins_consensus += "-"
+                del_consensus += "-"
+                mappings_consensus += str(min(9, count))
+
+            elif frameshift_origin and type_consensus == "I":
+                common_maplen, count = collections.Counter(maplen for maplen, seq in type_fragments[type_consensus]).most_common(1)[0]
+                common_seqlen, count = collections.Counter(len(seq) for maplen, seq in type_fragments[type_consensus] if maplen == common_maplen).most_common(1)[0]
+                origin_space_consensus += "^"
+                ins_consensus += str(min(9, maplen))
+                del_consensus += "-"
+                mappings_consensus += str(min(9, count))
 
-                selected=[seq for maplen,seq in type_fragments[type_consensus] if common_maplen==maplen and len(seq)==common_seqlen]
+                selected = [seq for maplen, seq in type_fragments[type_consensus] if common_maplen == maplen and len(seq) == common_seqlen]
 
                 for i in range(common_seqlen):
-                    common_ins_base,_=collections.Counter(seq[i] for seq in selected).most_common(1)[0]
-                    consensus+=common_ins_base
+                    common_ins_base, _ = collections.Counter(seq[i] for seq in selected).most_common(1)[0]
+                    consensus += common_ins_base
 
-                skip_until=ci+common_seqlen+common_maplen-1
+                skip_until = ci + common_seqlen + common_maplen - 1
 
-            elif frameshift_origin and type_consensus=="D":
-                del_consensus=del_consensus[:-1]+str(min(9,maplen))
+            elif frameshift_origin and type_consensus == "D":
+                del_consensus = del_consensus[:-1] + str(min(9, maplen))
 
         if not return_debug:
             return consensus
         else:
-            return origin_space_consensus,ins_consensus,del_consensus,mappings_consensus,consensus
+            return origin_space_consensus, ins_consensus, del_consensus, mappings_consensus, consensus
+
 
-def make_group(lead,klen,skip,repetitive_kmers):
-    anchors={}
-    for i, kmer in iter_kmers(lead.seq,klen,skip):
+def make_group(lead, klen, skip, repetitive_kmers):
+    anchors = {}
+    for i, kmer in iter_kmers(lead.seq, klen, skip):
         if kmer in repetitive_kmers:
             continue
         if not kmer in anchors:
-            anchors[kmer]=[i]
+            anchors[kmer] = [i]
         else:
             anchors[kmer].append(i)
 
     return Group(anchors=anchors,
-                 mappings={i:[("M", 1, i, i+1, i, lead)] for i in range(len(lead.seq))},
+                 mappings={i: [("M", 1, i, i + 1, i, lead)] for i in range(len(lead.seq))},
                  consensus_min=0,
-                 consensus_max=len(lead.seq)-1,
+                 consensus_max=len(lead.seq) - 1,
                  start_len=len(lead.seq),
                  origin=lead,
                  support=[lead])
 
-def iter_kmers(seq,klen,skip):
-    for i in range(0,len(seq)-klen,skip):
-        yield (i,seq[i:i+klen])
+
+def iter_kmers(seq, klen, skip):
+    for i in range(0, len(seq) - klen, skip):
+        yield (i, seq[i:i + klen])
+
 
 def from_leads(leads, initial_lead, max_grp=3, klen=15, skip=1, skip_repetitive=1, extend=False):
-    #TODO: Handle DELs in flattening
-    #TODO: Allow mapping across putative INDELs at sequence ends, allowing correcting them
-    #TODO: Dynamically adapt kmer len threshold so short+long origs can be assembled at the same time, same for repetitive_limit
-    #TODO: Ensure that kmers before and after last mapping are added as (secondary) anchors (hints 4 indels)
-
-    repetitive_limit=len(leads)+2
-
-    #Generate repetitive kmer list
-    kmer_counts={}
-    #for lead in leads:
-    for i, kmer in iter_kmers(initial_lead.seq,klen=klen,skip=skip_repetitive):
-        if not kmer in kmer_counts:
-            kmer_counts[kmer]=1
+    # TODO: Handle DELs in flattening
+    # TODO: Allow mapping across putative INDELs at sequence ends, allowing correcting them
+    # TODO: Dynamically adapt kmer len threshold so short+long origs can be assembled at the same time, same for repetitive_limit
+    # TODO: Ensure that kmers before and after last mapping are added as (secondary) anchors (hints 4 indels)
+
+    repetitive_limit = len(leads) + 2
+
+    # Generate repetitive kmer list
+    kmer_counts = {}
+    # for lead in leads:
+    for i, kmer in iter_kmers(initial_lead.seq, klen=klen, skip=skip_repetitive):
+        if kmer not in kmer_counts:
+            kmer_counts[kmer] = 1
         else:
-            kmer_counts[kmer]+=1
-    repetitive_kmers=set(kmer for kmer,count in kmer_counts.items() if count>repetitive_limit)
+            kmer_counts[kmer] += 1
+    repetitive_kmers = set(kmer for kmer, count in kmer_counts.items() if count > repetitive_limit)
 
-    #Create initial group
-    leads=sorted(leads,key=lambda ld: len(ld.seq))
-    groups=[make_group(initial_lead,klen,skip,repetitive_kmers)]
+    # Create initial group
+    leads = sorted(leads, key=lambda ld: len(ld.seq))
+    groups = [make_group(initial_lead, klen, skip, repetitive_kmers)]
 
     for lead in leads:
-        if lead.seq==None:
+        if lead.seq is None:
             continue
 
-        assigned=False
+        assigned = False
 
-        #Try to place this lead's INS seq in the group
+        # Try to place this lead's INS seq in the group
         for group in groups[:max_grp]:
-            mapped=False
-            last_i,last_j,last_was_repeat=None,None,False
-            first_i,first_j=None,None
-
-            #Attempt to anchor kmers from seq to current group
-            for i, kmer in iter_kmers(lead.seq,klen=klen,skip=skip):
-                if not kmer in group.anchors: #and len(set(group.anchors[kmer]))==1:
+            mapped = False
+            last_i, last_j, last_was_repeat = None, None, False
+            first_i, first_j = None, None
+
+            # Attempt to anchor kmers from seq to current group
+            for i, kmer in iter_kmers(lead.seq, klen=klen, skip=skip):
+                if kmer not in group.anchors:  # and len(set(group.anchors[kmer]))==1:
                     continue
 
                 if len(set(group.anchors[kmer])) > 1:
-                    if last_j==None:
-                        #Do not allow the first kmer to have multiple potential positions
+                    if last_j is None:
+                        # Do not allow the first kmer to have multiple potential positions
                         continue
 
-                    #Kmer occurs at multiple points in group sequence. Attempt to choose anchor most suitable for linear mapping
-                    j=group.anchors[kmer][0]
+                    # Kmer occurs at multiple points in group sequence. Attempt to choose anchor most suitable for linear mapping
+                    j = group.anchors[kmer][0]
                     for anchor_j_curr in group.anchors[kmer][1:]:
-                        if abs(anchor_j_curr-(last_j+1)) < abs(j-(last_j+1)):
-                            j=anchor_j_curr
-                    last_was_repeat=True
+                        if abs(anchor_j_curr - (last_j + 1)) < abs(j - (last_j + 1)):
+                            j = anchor_j_curr
+                    last_was_repeat = True
                 else:
-                    #Kmer can be unambiguously placed on group sequence
-                    j=group.anchors[kmer][0]
+                    # Kmer can be unambiguously placed on group sequence
+                    j = group.anchors[kmer][0]
 
-                if first_i==None and first_j==None:
-                    first_i=i
-                    first_j=j
-
-                if last_i != None and last_j != None:
-                    #Determine mapping type by position of current and last kmer on the lead sequence and group sequence
-                    dist_lead=i-last_i
-                    dist_group=j-last_j
+                if first_i is None and first_j is None:
+                    first_i = i
+                    first_j = j
+
+                if last_i is not None and last_j is not None:
+                    # Determine mapping type by position of current and last kmer on the lead sequence and group sequence
+                    dist_lead = i - last_i
+                    dist_group = j - last_j
 
                     if not last_was_repeat and dist_lead > dist_group:
-                        maptype="D"
-                        maplen=dist_group-dist_lead
+                        maptype = "D"
+                        maplen = dist_group - dist_lead
                         if not last_j in group.mappings:
-                            group.mappings[last_j]=[]
+                            group.mappings[last_j] = []
                         group.mappings[last_j].append((maptype, maplen, last_i, i, j, lead))
 
                     elif not last_was_repeat and dist_lead < dist_group:
-                        maptype="I"
-                        maplen=dist_group-dist_lead
+                        maptype = "I"
+                        maplen = dist_group - dist_lead
                         if not last_j in group.mappings:
-                            group.mappings[last_j]=[]
+                            group.mappings[last_j] = []
                         group.mappings[last_j].append((maptype, maplen, last_i, i, j, lead))
 
                     else:
-                        maptype="M"
-                        maplen=last_i-i
-                        act_j=last_j
-                        for act_i in range(last_i,i):
-                            if not act_j in group.mappings:
-                                group.mappings[act_j]=[]
-                            group.mappings[act_j].append((maptype, maplen, act_i, act_i+1, last_j, lead))
-                            act_j+=1
-
-                mapped=True
-                last_i=i
-                last_j=j
-                last_was_repeat=False
+                        maptype = "M"
+                        maplen = last_i - i
+                        act_j = last_j
+                        for act_i in range(last_i, i):
+                            if act_j not in group.mappings:
+                                group.mappings[act_j] = []
+                            group.mappings[act_j].append((maptype, maplen, act_i, act_i + 1, last_j, lead))
+                            act_j += 1
+
+                mapped = True
+                last_i = i
+                last_j = j
+                last_was_repeat = False
 
             if mapped:
                 group.support.append(lead)
-                assigned=True
-                max_i=len(lead.seq)
+                assigned = True
+                max_i = len(lead.seq)
 
-                #Extend consensus group leftwards
-                if extend and first_i - (first_j-group.consensus_min) > 0: # and first_j < 1.5*klen:
-                    for i in range(first_i,-1,-1):
-                        curr_j=first_j-(first_i-i)
-                        if curr_j <= group.consensus_min: #+klen/1:
-                            assert(curr_j==group.consensus_min)
-                            kmer=lead.seq[i:i+klen]
-                            if not kmer in repetitive_kmers:
-                                group.anchors[kmer]=[curr_j]
-                            group.consensus_min-=1
-                            if not curr_j in group.mappings:
-                                group.mappings[curr_j]=[]
-                            group.mappings[curr_j].append(("M", 1, i, i+1, first_j, lead))
-
-                #Extend consensus group rightwards
-                if extend and last_j+(max_i-last_i) > group.consensus_max:
-                    for i in range(last_i,max_i,1):
-                        curr_j=last_j+(i-last_i)
-                        if curr_j+klen >= group.consensus_max: #-klen/1:
-                            assert(curr_j+klen==group.consensus_max)
-                            kmer=lead.seq[i:i+klen]
-                            if not kmer in repetitive_kmers:
-                                group.anchors[kmer]=[curr_j]
-                            group.consensus_max+=1
-                            if not curr_j in group.mappings:
-                                group.mappings[curr_j]=[]
-                            group.mappings[curr_j].append(("M", 1, i, i+1, last_j, lead))
+                # Extend consensus group leftwards
+                if extend and first_i - (first_j - group.consensus_min) > 0:  # and first_j < 1.5*klen:
+                    for i in range(first_i, -1, -1):
+                        curr_j = first_j - (first_i - i)
+                        if curr_j <= group.consensus_min:  # +klen/1:
+                            assert (curr_j == group.consensus_min)
+                            kmer = lead.seq[i:i + klen]
+                            if kmer not in repetitive_kmers:
+                                group.anchors[kmer] = [curr_j]
+                            group.consensus_min -= 1
+                            if curr_j not in group.mappings:
+                                group.mappings[curr_j] = []
+                            group.mappings[curr_j].append(("M", 1, i, i + 1, first_j, lead))
+
+                # Extend consensus group rightwards
+                if extend and last_j + (max_i - last_i) > group.consensus_max:
+                    for i in range(last_i, max_i, 1):
+                        curr_j = last_j + (i - last_i)
+                        if curr_j + klen >= group.consensus_max:  # -klen/1:
+                            assert (curr_j + klen == group.consensus_max)
+                            kmer = lead.seq[i:i + klen]
+                            if kmer not in repetitive_kmers:
+                                group.anchors[kmer] = [curr_j]
+                            group.consensus_max += 1
+                            if curr_j not in group.mappings:
+                                group.mappings[curr_j] = []
+                            group.mappings[curr_j].append(("M", 1, i, i + 1, last_j, lead))
                 break
 
         if not assigned:
-            groups.append(make_group(lead,klen,skip,repetitive_kmers))
-            #groups.sort(key=lambda g: len(g.mappings), reverse=True)
+            groups.append(make_group(lead, klen, skip, repetitive_kmers))
+            # groups.sort(key=lambda g: len(g.mappings), reverse=True)
 
     return groups
 
 
-def novel_from_reads(best_lead,other_leads,klen,skip,skip_repetitive,debug=False):
-    consensus_min=2
-    maxshift=klen
-    minspan=0.2
-    minalns=0.25
-    minident=0.5
-    minident_abs=5
-    minbestdiff=3
-
-    alignments=[]
-    anchors={}
-    taboo=set()
-    for i, kmer in iter_kmers(best_lead.seq,klen=klen,skip=skip_repetitive):
+def novel_from_reads(best_lead, other_leads, klen, skip, skip_repetitive, debug=False):
+    consensus_min = 2
+    maxshift = klen
+    minspan = 0.2
+    minalns = 0.25
+    minident = 0.5
+    minident_abs = 5
+    minbestdiff = 3
+
+    alignments = []
+    anchors = {}
+    taboo = set()
+    for i, kmer in iter_kmers(best_lead.seq, klen=klen, skip=skip_repetitive):
         if kmer in taboo:
             continue
         if kmer in anchors:
             del anchors[kmer]
             taboo.add(kmer)
             continue
-        anchors[kmer]=i
+        anchors[kmer] = i
 
-    for leadi,lead in enumerate(other_leads):
-        last_i=None
-        last_j=None
-        conseq=""
-        span=0
-        for j, kmer in iter_kmers(lead.seq,klen=klen,skip=skip):
-            if not kmer in anchors:
+    for leadi, lead in enumerate(other_leads):
+        last_i = None
+        last_j = None
+        conseq = ""
+        span = 0
+        for j, kmer in iter_kmers(lead.seq, klen=klen, skip=skip):
+            if kmer not in anchors:
                 continue
-            i=anchors[kmer]
-            if abs(i-j) > maxshift:
+            i = anchors[kmer]
+            if abs(i - j) > maxshift:
                 continue
-            if last_i != None and i <= last_i:
+            if last_i is not None and i <= last_i:
                 continue
 
-            if last_i == None:
-                if j>0:
-                    conseq="-"*i
+            if last_i is None:
+                if j > 0:
+                    conseq = "-" * i
             else:
-                fwd_i=i-last_i
-                fwd_j=j-last_j
-                if len(conseq)+fwd_j > len(best_lead.seq):
-                    fwd_j=len(best_lead.seq)-len(conseq)
+                fwd_i = i - last_i
+                fwd_j = j - last_j
+                if len(conseq) + fwd_j > len(best_lead.seq):
+                    fwd_j = len(best_lead.seq) - len(conseq)
 
                 if fwd_i == fwd_j and fwd_j > 0:
-                    span+=(j-last_j)
-                    m=0
-                    for l in range(1,(j-last_j)+1):
-                        if lead.seq[last_j+l] == best_lead.seq[last_i+l]:
-                            m+=1
-                    ident=m/float((j-last_j))
+                    span += (j - last_j)
+                    m = 0
+                    for l in range(1, (j - last_j) + 1):
+                        if lead.seq[last_j + l] == best_lead.seq[last_i + l]:
+                            m += 1
+                    ident = m / float((j - last_j))
                     if ident >= minident:
-                        conseq+=lead.seq[last_j:j][:fwd_j]
+                        conseq += lead.seq[last_j:j][:fwd_j]
                     else:
-                        conseq+="-"*(fwd_j)
+                        conseq += "-" * (fwd_j)
                 else:
-                    conseq+="-"*(fwd_j)
-            last_i=i
-            last_j=j
+                    conseq += "-" * (fwd_j)
+            last_i = i
+            last_j = j
 
         if len(conseq) < len(best_lead.seq):
-            conseq+="-"*(len(best_lead.seq)-len(conseq))
+            conseq += "-" * (len(best_lead.seq) - len(conseq))
 
-        conseq_new=[]
-        h=0
+        conseq_new = []
+        h = 0
         while h < len(best_lead.seq):
-            if conseq[h]=="-":
+            if conseq[h] == "-":
                 conseq_new.append("-")
-                h+=1
+                h += 1
             else:
-                buffer=[]
-                ident=0
-                while h < len(best_lead.seq) and conseq[h]!="-":
-                    ident+=(best_lead.seq[h]==conseq[h])
+                buffer = []
+                ident = 0
+                while h < len(best_lead.seq) and conseq[h] != "-":
+                    ident += (best_lead.seq[h] == conseq[h])
                     buffer.append(conseq[h])
-                    h+=1
-                if ident/float(len(buffer)) > minident and ident>minident_abs:
+                    h += 1
+                if ident / float(len(buffer)) > minident and ident > minident_abs:
                     conseq_new.append("".join(buffer))
                 else:
-                    conseq_new.append("-"*len(buffer))
-        conseq="".join(conseq_new)
+                    conseq_new.append("-" * len(buffer))
+        conseq = "".join(conseq_new)
 
-        # FIXME: can lead to ZeroDivisionError
-        if span/float(len(best_lead.seq)) > minspan:
+        if span / float(len(best_lead.seq)) > minspan:
             alignments.append(conseq)
 
-    maxal=1
+    maxal = 1
     for i in range(len(best_lead.seq)):
-        maxal=max(maxal,len([best_lead.seq[i]]+[a[i] for a in alignments if not a[i] in "^_"]))
-    maxal=float(maxal)
+        maxal = max(maxal, len([best_lead.seq[i]] + [a[i] for a in alignments if not a[i] in "^_"]))
+    maxal = float(maxal)
 
-    flattened=""
+    flattened = ""
     for i in range(len(best_lead.seq)):
-        al=[a[i] for a in alignments if not a[i]=="-"]
-        if len(al) < consensus_min or len(al)/maxal < minalns:
-            flattened+=best_lead.seq[i]
+        al = [a[i] for a in alignments if not a[i] == "-"]
+        if len(al) < consensus_min or len(al) / maxal < minalns:
+            flattened += best_lead.seq[i]
         else:
-            top=util.most_common([best_lead.seq[i]]+al)
-            if len(top)>1 and top[0][0]-top[1][0] >= minbestdiff:
-                flattened+=top[0][1]
+            top = util.most_common([best_lead.seq[i]] + al)
+            if len(top) > 1 and top[0][0] - top[1][0] >= minbestdiff:
+                flattened += top[0][1]
             else:
-                flattened+=best_lead.seq[i]
+                flattened += best_lead.seq[i]
 
-            #if top[0][0]/float(len(al)+1) < 0.75:
+            # if top[0][0]/float(len(al)+1) < 0.75:
             #    flattened+=best_lead.seq[i]
-            #else:
+            # else:
             #    flattened+=top[0][1]
 
-    #print("FLT",flattened)
-    #if debug:
+    # print("FLT",flattened)
+    # if debug:
     #    print("B",best_lead.seq)
     #    for o in other_leads:
     #        print("O",o.seq)
     #    print("F",flattened)
     #    print("=====")
     return flattened
```

### Comparing `sniffles-2.2/src/sniffles/leadprov.py` & `sniffles-2.3/src/sniffles/leadprov.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,439 +1,453 @@
 #!/usr/bin/env python3
 #
 # Sniffles2
 # A fast structural variant caller for long-read sequencing data
 #
-# Created: 28.05.2021
-# Author:  Moritz Smolka
-# Contact: moritz.g.smolka@gmail.com
+# Created:     28.05.2021
+# Author:      Moritz Smolka
+# Maintainer:  Hermann Romanek
+# Contact:     sniffles@romanek.at
 #
 from dataclasses import dataclass
 import re
 import itertools
+from typing import Optional
 
 import pysam
 
-#for: --dev-cache
+# for: --dev-cache
 import os
 import sys
 import pickle
-#end: for: --dev-cache
+# end: for: --dev-cache
 
 from sniffles import util
 from sniffles import sv
 
+
 @dataclass
 class Lead:
-    read_id: int=None
-    read_qname: str=None
-    contig: str=None
-    ref_start: int=None
-    ref_end: int=None
-    qry_start: int=None
-    qry_end: int=None
-    strand: str=None
-    mapq: int=None
-    nm: float=None
-    source: str=None
-    svtype: str=None
-    svlen: int=None
-    seq: str=None
-    svtypes_starts_lens: list=None
+    read_id: int = None
+    read_qname: str = None
+    contig: str = None
+    ref_start: int = None
+    ref_end: int = None
+    qry_start: int = None
+    qry_end: int = None
+    strand: str = None
+    mapq: int = None
+    nm: float = None
+    source: str = None
+    svtype: str = None
+    svlen: Optional[int] = None
+    seq: Optional[str] = None
+    svtypes_starts_lens: list = None
+
 
 def CIGAR_analyze(cigar):
-    buf=""
-    readspan=0
-    refspan=0
-    clip_start=None
-    clip=0
+    buf = ""
+    readspan = 0
+    refspan = 0
+    clip_start = None
+    clip = 0
     for c in cigar:
         if c.isnumeric():
-            buf+=c
+            buf += c
         else:
-            oplen=int(buf)
-            h=False
+            oplen = int(buf)
+            h = False
             if c in "MIX=":
-                readspan+=oplen
-                h=True
+                readspan += oplen
+                h = True
             if c in "MDX=N":
-                refspan+=oplen
-                h=True
+                refspan += oplen
+                h = True
             if not h:
                 if c in "SH":
-                    if clip_start==None and readspan+refspan>0:
-                        clip_start=clip
-                    clip+=oplen
+                    if clip_start == None and readspan + refspan > 0:
+                        clip_start = clip
+                    clip += oplen
                 else:
                     raise f"Unknown CIGAR operation: '{c}'"
-            buf=""
-    if clip_start==None:
-        clip_start=clip
-    return clip_start, clip-clip_start, refspan, readspan
+            buf = ""
+    if clip_start == None:
+        clip_start = clip
+    return clip_start, clip - clip_start, refspan, readspan
+
 
 def CIGAR_analyze_regex(cigar):
-    #TODO: Obsolete
-    opsums={"M":0,"I":0,"D":0,"=":0,"X":0,"N":0,"H":0,"S":0}
-    iter=re.split(r"(\d+)", cigar)
-    for i in range(1,len(iter)-1,2):
-        op=iter[i+1]
-        if op!="H" and op!="S":
-            readstart_fwd=opsums["H"]+opsums["S"]
-        opsums[iter[i+1]]+=int(iter[i])
-    readstart_rev=opsums["H"]+opsums["S"]-readstart_fwd
-    refspan=opsums["M"]+opsums["D"]+opsums["="]+opsums["X"]+opsums["N"]
-    readspan=opsums["M"]+opsums["I"]+opsums["="]+opsums["X"]
-    return readstart_fwd,readstart_rev,refspan,readspan
+    # TODO: Obsolete
+    opsums = {"M": 0, "I": 0, "D": 0, "=": 0, "X": 0, "N": 0, "H": 0, "S": 0}
+    iter = re.split(r"(\d+)", cigar)
+    for i in range(1, len(iter) - 1, 2):
+        op = iter[i + 1]
+        if op != "H" and op != "S":
+            readstart_fwd = opsums["H"] + opsums["S"]
+        opsums[iter[i + 1]] += int(iter[i])
+    readstart_rev = opsums["H"] + opsums["S"] - readstart_fwd
+    refspan = opsums["M"] + opsums["D"] + opsums["="] + opsums["X"] + opsums["N"]
+    readspan = opsums["M"] + opsums["I"] + opsums["="] + opsums["X"]
+    return readstart_fwd, readstart_rev, refspan, readspan
+
 
 def CIGAR_tolist(cigar):
-    #TODO: Obsolete (see CIGAR_tolist_analyze)
+    # TODO: Obsolete (see CIGAR_tolist_analyze)
     """
     CIGAR string : str -> List of CIGAR operation & length tuples : [(op1:char, op1_length:int),...]
     """
-    buf=""
-    ops=[]
+    buf = ""
+    ops = []
     for c in cigar:
         if c.isnumeric():
-            buf+=c
+            buf += c
         else:
-            ops.append((c,int(buf)))
-            buf=""
+            ops.append((c, int(buf)))
+            buf = ""
     return ops
 
+
 def CIGAR_listrefspan(ops):
-    #TODO: Obsolete (see CIGAR_analyze)
-    #TODO(Potential): Detect&utilize minimap2 condensed supplementary alignment cigar for speed
-    return sum(oplen for op,oplen in ops if op=="M" or op=="D" or op=="=" or op=="X" or op=="N")
+    # TODO: Obsolete (see CIGAR_analyze)
+    # TODO(Potential): Detect&utilize minimap2 condensed supplementary alignment cigar for speed
+    return sum(oplen for op, oplen in ops if op == "M" or op == "D" or op == "=" or op == "X" or op == "N")
+
 
 def CIGAR_listreadspan(ops):
-    #TODO: Obsolete (see CIGAR_analyze)
-    return sum(oplen for op,oplen in ops if op=="M" or op=="I" or op=="=" or op=="X")
+    # TODO: Obsolete (see CIGAR_analyze)
+    return sum(oplen for op, oplen in ops if op == "M" or op == "I" or op == "=" or op == "X")
+
 
 def CIGAR_listreadstart_fwd(ops):
-    #TODO: Obsolete (see CIGAR_analyze)
+    # TODO: Obsolete (see CIGAR_analyze)
     """
     Position in query read where CIGAR alignment starts (i.e. taking into account start clipping)
     """
-    op,oplen=ops[0]
-    op2,op2len=ops[1]
-    if op=="H" or op=="S":
-        assert(op2!="H" and op2!="S")
+    op, oplen = ops[0]
+    op2, op2len = ops[1]
+    if op == "H" or op == "S":
+        assert (op2 != "H" and op2 != "S")
         return oplen
     else:
         return 0
 
+
 def CIGAR_listreadstart_rev(ops):
-    #TODO: Obsolete (see CIGAR_analyze)
+    # TODO: Obsolete (see CIGAR_analyze)
     """
     Position in query read where CIGAR alignment starts (i.e. taking into account start clipping)
     """
-    op,oplen=ops[-1]
-    op2,op2len=ops[-2]
-    if op=="H" or op=="S":
-        assert(op2!="H" and op2!="S")
+    op, oplen = ops[-1]
+    op2, op2len = ops[-2]
+    if op == "H" or op == "S":
+        assert (op2 != "H" and op2 != "S")
         return oplen
     else:
         return 0
 
-OPTAB={pysam.CMATCH:     (1,1,0),
-       pysam.CEQUAL:     (1,1,0),
-       pysam.CDIFF:      (1,1,0),
-       pysam.CINS:       (1,0,1),
-       pysam.CDEL:       (0,1,1),
-       pysam.CREF_SKIP:  (0,1,0),
-       pysam.CSOFT_CLIP: (1,0,1),
-       pysam.CHARD_CLIP: (0,0,0),
-       pysam.CPAD:       (0,0,0)}
+
+OPTAB = {pysam.CMATCH: (1, 1, 0),
+         pysam.CEQUAL: (1, 1, 0),
+         pysam.CDIFF: (1, 1, 0),
+         pysam.CINS: (1, 0, 1),
+         pysam.CDEL: (0, 1, 1),
+         pysam.CREF_SKIP: (0, 1, 0),
+         pysam.CSOFT_CLIP: (1, 0, 1),
+         pysam.CHARD_CLIP: (0, 0, 0),
+         pysam.CPAD: (0, 0, 0)}
 #      pysam.CBACK:      (0,0,0)}
 
-OPLIST=[(0,0,0) for i in range(max(int(k) for k in OPTAB.keys())+1)]
-for k,v in OPTAB.items():
-    OPLIST[int(k)]=v
-
-def read_iterindels(read_id,read,contig,config,use_clips,read_nm):
-    minsvlen=config.minsvlen_screen
-    longinslen=config.long_ins_length/2.0
-    seq_cache_maxlen=config.dev_seq_cache_maxlen
-    qname=read.query_name
-    mapq=read.mapping_quality
-    strand="-" if read.is_reverse else "+"
-    CINS=pysam.CINS
-    CDEL=pysam.CDEL
-    CSOFT_CLIP=pysam.CSOFT_CLIP
+OPLIST = [(0, 0, 0) for i in range(max(int(k) for k in OPTAB.keys()) + 1)]
+for k, v in OPTAB.items():
+    OPLIST[int(k)] = v
+
+
+def read_iterindels(read_id, read, contig, config, use_clips, read_nm):
+    minsvlen = config.minsvlen_screen
+    longinslen = config.long_ins_length / 2.0
+    seq_cache_maxlen = config.dev_seq_cache_maxlen
+    qname = read.query_name
+    mapq = read.mapping_quality
+    strand = "-" if read.is_reverse else "+"
+    CINS = pysam.CINS
+    CDEL = pysam.CDEL
+    CSOFT_CLIP = pysam.CSOFT_CLIP
 
-    pos_read=0
-    pos_ref=read.reference_start
+    pos_read = 0
+    pos_ref = read.reference_start
 
-    for op,oplength in read.cigartuples:
-        add_read,add_ref,event=OPLIST[op]
+    for op, oplength in read.cigartuples:
+        add_read, add_ref, event = OPLIST[op]
         if event and oplength >= minsvlen:
-            if op==CINS:
+            if op == CINS:
                 yield Lead(read_id,
                            qname,
                            contig,
                            pos_ref,
                            pos_ref,
                            pos_read,
-                           pos_read+oplength,
+                           pos_read + oplength,
                            strand,
                            mapq,
                            read_nm,
                            "INLINE",
                            "INS",
                            oplength,
-                           seq=read.query_sequence[pos_read:pos_read+oplength] if oplength <= seq_cache_maxlen else None)
-            elif op==CDEL:
+                           seq=read.query_sequence[pos_read:pos_read + oplength] if oplength <= seq_cache_maxlen else None)
+            elif op == CDEL:
                 yield Lead(read_id,
                            qname,
                            contig,
-                           pos_ref+oplength,
+                           pos_ref + oplength,
                            pos_ref,
                            pos_read,
                            pos_read,
                            strand,
                            mapq,
                            read_nm,
                            "INLINE",
                            "DEL",
                            -oplength)
-            elif use_clips and op==CSOFT_CLIP and oplength >= longinslen:
+            elif use_clips and op == CSOFT_CLIP and oplength >= longinslen:
                 yield Lead(read_id,
                            qname,
                            contig,
                            pos_ref,
                            pos_ref,
                            pos_read,
-                           pos_read+oplength,
+                           pos_read + oplength,
                            strand,
                            mapq,
                            read_nm,
                            "INLINE",
                            "INS",
                            None,
                            seq=None)
-        pos_read+=add_read*oplength
-        pos_ref+=add_ref*oplength
+        pos_read += add_read * oplength
+        pos_ref += add_ref * oplength
+
 
-def get_cigar_indels(read_id,read,contig,config,use_clips,read_nm):
-    minsvlen=config.minsvlen_screen
-    longinslen=config.long_ins_length/2.0
-    seq_cache_maxlen=config.dev_seq_cache_maxlen
-    qname=read.query_name
-    mapq=read.mapping_quality
-    strand="-" if read.is_reverse else "+"
-    CINS=pysam.CINS
-    CDEL=pysam.CDEL
-    CSOFT_CLIP=pysam.CSOFT_CLIP
-
-    INS_SUM=0
-    DEL_SUM=0
-
-    pos_read=0
-    pos_ref=read.reference_start
-    for op,oplength in read.cigartuples:
-        add_read,add_ref,event=OPLIST[op]
+def get_cigar_indels(read_id, read, contig, config, use_clips, read_nm):
+    minsvlen = config.minsvlen_screen
+    longinslen = config.long_ins_length / 2.0
+    seq_cache_maxlen = config.dev_seq_cache_maxlen
+    qname = read.query_name
+    mapq = read.mapping_quality
+    strand = "-" if read.is_reverse else "+"
+    CINS = pysam.CINS
+    CDEL = pysam.CDEL
+    CSOFT_CLIP = pysam.CSOFT_CLIP
+
+    INS_SUM = 0
+    DEL_SUM = 0
+
+    pos_read = 0
+    pos_ref = read.reference_start
+    for op, oplength in read.cigartuples:
+        add_read, add_ref, event = OPLIST[op]
         if event:
-            if op==CINS:
-                INS_SUM+=oplength
-            elif op==CDEL:
-                DEL_SUM+=oplength
-        pos_read+=add_read*oplength
-        pos_ref+=add_ref*oplength
-
-    return INS_SUM,DEL_SUM
-
-def read_itersplits_bnd(read_id,read,contig,config,read_nm):
-    assert(read.is_supplementary)
-    #SA:refname,pos,strand,CIGAR,MAPQ,NM
-    all_leads=[]
-    supps=[part.split(",") for part in read.get_tag("SA").split(";") if len(part)>0]
+            if op == CINS:
+                INS_SUM += oplength
+            elif op == CDEL:
+                DEL_SUM += oplength
+        pos_read += add_read * oplength
+        pos_ref += add_ref * oplength
+
+    return INS_SUM, DEL_SUM
+
+
+def read_itersplits_bnd(read_id, read, contig, config, read_nm):
+    assert (read.is_supplementary)
+    # SA:refname,pos,strand,CIGAR,MAPQ,NM
+    all_leads = []
+    supps = [part.split(",") for part in read.get_tag("SA").split(";") if len(part) > 0]
 
-    if len(supps) > config.max_splits_base + config.max_splits_kb*(read.query_length/1000.0):
+    if len(supps) > config.max_splits_base + config.max_splits_kb * (read.query_length / 1000.0):
         return
 
     if read.is_reverse:
-        qry_start=read.query_length-read.query_alignment_end
+        qry_start = read.query_length - read.query_alignment_end
     else:
-        qry_start=read.query_alignment_start
+        qry_start = read.query_alignment_start
 
-    curr_lead=Lead(read_id,
-                   read.query_name,
-                   contig,
-                   read.reference_start,
-                   read.reference_start+read.reference_length,
-                   qry_start,
-                   qry_start+read.query_alignment_length,
-                   "-" if read.is_reverse else "+",
-                   read.mapping_quality,
-                   read_nm,
-                   "SPLIT_SUP",
-                   "?")
+    curr_lead = Lead(read_id,
+                     read.query_name,
+                     contig,
+                     read.reference_start,
+                     read.reference_start + read.reference_length,
+                     qry_start,
+                     qry_start + read.query_alignment_length,
+                     "-" if read.is_reverse else "+",
+                     read.mapping_quality,
+                     read_nm,
+                     "SPLIT_SUP",
+                     "?")
     all_leads.append(curr_lead)
 
-    prim_refname,prim_pos,prim_strand,prim_cigar,prim_mapq,prim_nm=supps[0]
+    prim_refname, prim_pos, prim_strand, prim_cigar, prim_mapq, prim_nm = supps[0]
     if prim_refname == contig:
-        #Primary alignment is on this chromosome, no need to parse the supplementary
+        # Primary alignment is on this chromosome, no need to parse the supplementary
         return
 
-    minpos_curr_chr=min(itertools.chain([read.reference_start],(int(pos) for refname,pos,strand,cigar,mapq,nm in supps if refname==contig)))
+    minpos_curr_chr = min(itertools.chain([read.reference_start], (int(pos) for refname, pos, strand, cigar, mapq, nm in supps if refname == contig)))
     if minpos_curr_chr < read.reference_start:
-        #Only process splits once per chr (there may be multiple supplementary alignments on the same chr)
+        # Only process splits once per chr (there may be multiple supplementary alignments on the same chr)
         return
 
-    for refname,pos,strand,cigar,mapq,nm in supps:
-        mapq=int(mapq)
-        nm=int(nm)
-        #if not config.dev_keep_lowqual_splits and mapq < config.mapq:
+    for refname, pos, strand, cigar, mapq, nm in supps:
+        mapq = int(mapq)
+        nm = int(nm)
+        # if not config.dev_keep_lowqual_splits and mapq < config.mapq:
         #    continue
 
-        is_rev=(strand=="-")
+        is_rev = (strand == "-")
 
         try:
-            readstart_fwd,readstart_rev,refspan,readspan=CIGAR_analyze(cigar)
+            readstart_fwd, readstart_rev, refspan, readspan = CIGAR_analyze(cigar)
         except Exception as e:
             util.error(f"Malformed CIGAR '{cigar}' with pos {pos} of read '{read.query_name}' ({e}). Skipping.")
             return
 
-        pos_zero=int(pos)-1
-        split_qry_start=readstart_rev if is_rev else readstart_fwd
+        pos_zero = int(pos) - 1
+        split_qry_start = readstart_rev if is_rev else readstart_fwd
 
         all_leads.append(Lead(read_id,
                               read.query_name,
                               refname,
                               pos_zero,
                               pos_zero + refspan,
                               split_qry_start,
-                              split_qry_start+readspan,
+                              split_qry_start + readspan,
                               strand,
                               mapq,
                               read_nm,
                               "SPLIT_SUP",
                               "?"))
 
-    sv.classify_splits(read,all_leads,config,contig)
+    sv.classify_splits(read, all_leads, config, contig)
 
     for lead in all_leads:
         for svtype, svstart, arg in lead.svtypes_starts_lens:
-            if svtype=="BND":
+            if svtype == "BND":
                 bnd = Lead(read_id=lead.read_id,
                            read_qname=lead.read_qname,
                            contig=lead.contig,
                            ref_start=svstart,
                            ref_end=svstart,
                            qry_start=lead.qry_start,
                            qry_end=lead.qry_end,
                            strand=lead.strand,
                            mapq=lead.mapq,
                            nm=lead.nm,
                            source=lead.source,
                            svtype=svtype,
                            svlen=config.bnd_cluster_length,
                            seq=None)
-                bnd.bnd_info=arg
-                #print(lead.contig,svstart,bnd.bnd_info)
+                bnd.bnd_info = arg
+                # print(lead.contig,svstart,bnd.bnd_info)
                 yield bnd
 
-def read_itersplits(read_id,read,contig,config,read_nm):
-    #SA:refname,pos,strand,CIGAR,MAPQ,NM
-    all_leads=[]
-    supps=[part.split(",") for part in read.get_tag("SA").split(";") if len(part)>0]
-    trace_read=config.dev_trace_read!=False and config.dev_trace_read==read.query_name
 
-    if len(supps) > config.max_splits_base + config.max_splits_kb*(read.query_length/1000.0):
+def read_itersplits(read_id, read, contig, config, read_nm):
+    # SA:refname,pos,strand,CIGAR,MAPQ,NM
+    all_leads = []
+    supps = [part.split(",") for part in read.get_tag("SA").split(";") if len(part) > 0]
+    trace_read = config.dev_trace_read != False and config.dev_trace_read == read.query_name
+
+    if len(supps) > config.max_splits_base + config.max_splits_kb * (read.query_length / 1000.0):
         return
 
     if trace_read:
         print(f"[DEV_TRACE_READ] [0c/4] [LeadProvider.read_itersplits] [{read.query_name}] passed max_splits check")
 
-    #QC on: 18Aug21, HG002.ont.chr22; O.K.
-    #cigarl=CIGAR_tolist(read.cigarstring)
-    #if read.is_reverse:
+    # QC on: 18Aug21, HG002.ont.chr22; O.K.
+    # cigarl=CIGAR_tolist(read.cigarstring)
+    # if read.is_reverse:
     #    cigarl.reverse()
 
-    #if read.is_reverse:
+    # if read.is_reverse:
     #    assert(read.query_length-read.query_alignment_end == CIGAR_listreadstart(cigarl))
-    #else:
+    # else:
     #    assert(read.query_alignment_start == CIGAR_listreadstart(cigarl))
 
-    #assert(CIGAR_listrefspan(cigarl)==read.reference_length)
-    #assert(CIGAR_listreadspan(cigarl)==read.query_alignment_length)
-    #End QC
+    # assert(CIGAR_listrefspan(cigarl)==read.reference_length)
+    # assert(CIGAR_listreadspan(cigarl)==read.query_alignment_length)
+    # End QC
 
     if read.is_reverse:
-        qry_start=read.query_length-read.query_alignment_end
+        qry_start = read.query_length - read.query_alignment_end
     else:
-        qry_start=read.query_alignment_start
+        qry_start = read.query_alignment_start
 
-    curr_lead=Lead(read_id,
-                   read.query_name,
-                   contig,
-                   read.reference_start,
-                   read.reference_start+read.reference_length,
-                   qry_start,
-                   qry_start+read.query_alignment_length,
-                   "-" if read.is_reverse else "+",
-                   read.mapping_quality,
-                   read_nm,
-                   "SPLIT_PRIM",
-                   "?")
+    curr_lead = Lead(read_id,
+                     read.query_name,
+                     contig,
+                     read.reference_start,
+                     read.reference_start + read.reference_length,
+                     qry_start,
+                     qry_start + read.query_alignment_length,
+                     "-" if read.is_reverse else "+",
+                     read.mapping_quality,
+                     read_nm,
+                     "SPLIT_PRIM",
+                     "?")
     all_leads.append(curr_lead)
 
-    #QC on: 18Aug21; O.K.
-    #assert(read.reference_length == CIGAR_listrefspan(CIGAR_tolist(read.cigarstring)))
-    #assert(read.query_alignment_start == CIGAR_listreadstart(CIGAR_tolist(read.cigarstring)))
-    #assert(read.query_alignment_length == CIGAR_listreadspan(CIGAR_tolist(read.cigarstring)))
-    #End QC
-
-    for refname,pos,strand,cigar,mapq,nm in supps:
-        mapq=int(mapq)
-        nm=int(nm)
-        #if not config.dev_keep_lowqual_splits and mapq < config.mapq:
+    # QC on: 18Aug21; O.K.
+    # assert(read.reference_length == CIGAR_listrefspan(CIGAR_tolist(read.cigarstring)))
+    # assert(read.query_alignment_start == CIGAR_listreadstart(CIGAR_tolist(read.cigarstring)))
+    # assert(read.query_alignment_length == CIGAR_listreadspan(CIGAR_tolist(read.cigarstring)))
+    # End QC
+
+    for refname, pos, strand, cigar, mapq, nm in supps:
+        mapq = int(mapq)
+        nm = int(nm)
+        # if not config.dev_keep_lowqual_splits and mapq < config.mapq:
         #    continue
 
-        is_rev=(strand=="-")
+        is_rev = (strand == "-")
 
         try:
-            readstart_fwd,readstart_rev,refspan,readspan=CIGAR_analyze(cigar)
+            readstart_fwd, readstart_rev, refspan, readspan = CIGAR_analyze(cigar)
         except Exception as e:
             util.error(f"Malformed CIGAR '{cigar}' with pos {pos} of read '{read.query_name}' ({e}). Skipping.")
             return
 
-        pos_zero=int(pos)-1
-        split_qry_start=readstart_rev if is_rev else readstart_fwd
+        pos_zero = int(pos) - 1
+        split_qry_start = readstart_rev if is_rev else readstart_fwd
 
         all_leads.append(Lead(read_id,
                               read.query_name,
                               refname,
                               pos_zero,
                               pos_zero + refspan,
                               split_qry_start,
-                              split_qry_start+readspan,
+                              split_qry_start + readspan,
                               strand,
                               mapq,
                               read_nm,
                               "SPLIT_SUP",
                               "?"))
 
-        #QC on: 08Sep21; O.K.
-        #cigarl=CIGAR_tolist(cigar)
-        #assert(CIGAR_listrefspan(cigarl)==refspan)
-        #assert(CIGAR_listreadspan(cigarl)==readspan)
-        #assert(CIGAR_listreadstart_fwd(cigarl)==readstart_fwd)
-        #assert(CIGAR_listreadstart_rev(cigarl)==readstart_rev)
-        #End QC
+        # QC on: 08Sep21; O.K.
+        # cigarl=CIGAR_tolist(cigar)
+        # assert(CIGAR_listrefspan(cigarl)==refspan)
+        # assert(CIGAR_listreadspan(cigarl)==readspan)
+        # assert(CIGAR_listreadstart_fwd(cigarl)==readstart_fwd)
+        # assert(CIGAR_listreadstart_rev(cigarl)==readstart_rev)
+        # End QC
 
     if trace_read:
         print(f"[DEV_TRACE_READ] [0c/4] [LeadProvider.read_itersplits] [{read.query_name}] all_leads: {all_leads}")
 
-    sv.classify_splits(read,all_leads,config,contig)
+    sv.classify_splits(read, all_leads, config, contig)
 
     if trace_read:
         print(f"[DEV_TRACE_READ] [0c/4] [LeadProvider.read_itersplits] [{read.query_name}] classify_splits(all_leads): {all_leads}")
 
-
     """
     if config.dev_trace_read != False:
         print(read.query_name)
         if read.query_name == config.dev_trace_read:
             for lead_i, lead in enumerate(all_leads):
                 for svtype, svstart, arg in lead.svtypes_starts_lens:
                     min_mapq=min(lead.mapq,all_leads[max(0,lead_i-1)].mapq)
@@ -441,229 +455,229 @@
                     if not config.dev_keep_lowqual_splits and min_mapq < config.mapq:
                         keep=False
                     print(f"[DEV_TRACE_READ] [REPORT_LEAD_SPLIT] Splits identified from read {read.read_id}")
     """
 
     for lead_i, lead in enumerate(all_leads):
         for svtype, svstart, arg in lead.svtypes_starts_lens:
-            min_mapq=min(lead.mapq,all_leads[max(0,lead_i-1)].mapq)
+            min_mapq = min(lead.mapq, all_leads[max(0, lead_i - 1)].mapq)
             if not config.dev_keep_lowqual_splits and min_mapq < config.mapq:
                 continue
 
-            if svtype=="BND":
+            if svtype == "BND":
                 bnd = Lead(read_id=lead.read_id,
                            read_qname=lead.read_qname,
                            contig=lead.contig,
                            ref_start=svstart,
                            ref_end=svstart,
                            qry_start=lead.qry_start,
                            qry_end=lead.qry_end,
                            strand=lead.strand,
                            mapq=lead.mapq,
                            nm=lead.nm,
                            source=lead.source,
                            svtype=svtype,
                            svlen=config.bnd_cluster_length,
                            seq=None)
-                bnd.bnd_info=arg
+                bnd.bnd_info = arg
                 yield bnd
 
-            elif svtype!="NOSV":
-                svlen=arg
+            elif svtype != "NOSV":
+                svlen = arg
 
                 yield Lead(read_id=lead.read_id,
                            read_qname=lead.read_qname,
                            contig=lead.contig,
                            ref_start=svstart,
-                           ref_end=svstart+svlen if svlen!=None and svtype!="INS" else svstart,
+                           ref_end=svstart + svlen if svlen != None and svtype != "INS" else svstart,
                            qry_start=lead.qry_start,
                            qry_end=lead.qry_end,
                            strand=lead.strand,
                            mapq=lead.mapq,
                            nm=lead.nm,
                            source=lead.source,
                            svtype=svtype,
                            svlen=svlen,
-                           seq=lead.seq if svtype=="INS" else None)
+                           seq=lead.seq if svtype == "INS" else None)
+
 
 class LeadProvider:
-    def __init__(self,config,read_id_offset):
-        self.config=config
+    def __init__(self, config, read_id_offset):
+        self.config = config
 
-        self.leadtab={}
-        self.leadcounts={}
+        self.leadtab = {}
+        self.leadcounts = {}
 
         for svtype in sv.TYPES:
-            self.leadtab[svtype]={}
-            self.leadcounts[svtype]=0
+            self.leadtab[svtype] = {}
+            self.leadcounts[svtype] = 0
 
-        self.covrtab_fwd={}
-        self.covrtab_rev={}
-        self.covrtab_min_bin=None
-        #self.covrtab_read_start={}
-        #self.covrtab_read_end={}
-
-        self.read_id=read_id_offset
-        self.read_count=0
-
-        self.contig=None
-        self.start=None
-        self.end=None
+        self.covrtab_fwd = {}
+        self.covrtab_rev = {}
+        self.covrtab_min_bin = None
+        # self.covrtab_read_start={}
+        # self.covrtab_read_end={}
+
+        self.read_id = read_id_offset
+        self.read_count = 0
+
+        self.contig = None
+        self.start = None
+        self.end = None
 
-    def record_lead(self,ld,pos_leadtab):
-        leadtab_svtype=self.leadtab[ld.svtype]
+    def record_lead(self, ld, pos_leadtab):
+        leadtab_svtype = self.leadtab[ld.svtype]
         if pos_leadtab in leadtab_svtype:
             leadtab_svtype[pos_leadtab].append(ld)
-            lead_count=len(leadtab_svtype[pos_leadtab])
+            lead_count = len(leadtab_svtype[pos_leadtab])
             if lead_count > self.config.consensus_max_reads_bin:
-                ld.seq=None
+                ld.seq = None
         else:
-            leadtab_svtype[pos_leadtab]=[ld]
-            lead_count=1
-        self.leadcounts[ld.svtype]+=1
+            leadtab_svtype[pos_leadtab] = [ld]
+            lead_count = 1
+        self.leadcounts[ld.svtype] += 1
 
-    def build_leadtab(self,contig,start,end,bam):
+    def build_leadtab(self, contig, start, end, bam):
         if self.config.dev_cache:
-            loaded_externals=self.dev_load_leadtab(contig,start,end)
-            if loaded_externals!=False:
+            loaded_externals = self.dev_load_leadtab(contig, start, end)
+            if loaded_externals != False:
                 return loaded_externals
 
-        assert(self.contig==None)
-        assert(self.start==None)
-        assert(self.end==None)
-        self.contig=contig
-        self.start=start
-        self.end=end
-        self.covrtab_min_bin=int(self.start/self.config.coverage_binsize)*self.config.coverage_binsize
-
-        externals=[]
-        ld_binsize=self.config.cluster_binsize
-
-        for ld in self.iter_region(bam,contig,start,end):
-            ld_contig,ld_ref_start=ld.contig,ld.ref_start
-
-            if contig==ld_contig and ld_ref_start >= start and ld_ref_start < end:
-                pos_leadtab=int(ld_ref_start/ld_binsize)*ld_binsize
-                self.record_lead(ld,pos_leadtab)
+        assert (self.contig == None)
+        assert (self.start == None)
+        assert (self.end == None)
+        self.contig = contig
+        self.start = start
+        self.end = end
+        self.covrtab_min_bin = int(self.start / self.config.coverage_binsize) * self.config.coverage_binsize
+
+        externals = []
+        ld_binsize = self.config.cluster_binsize
+
+        for ld in self.iter_region(bam, contig, start, end):
+            ld_contig, ld_ref_start = ld.contig, ld.ref_start
+
+            if contig == ld_contig and ld_ref_start >= start and ld_ref_start < end:
+                pos_leadtab = int(ld_ref_start / ld_binsize) * ld_binsize
+                self.record_lead(ld, pos_leadtab)
             else:
                 externals.append(ld)
 
         if self.config.dev_cache:
-            self.dev_store_leadtab(contig,start,end,externals)
+            self.dev_store_leadtab(contig, start, end, externals)
 
         return externals
 
-    def iter_region(self,bam,contig,start=None,end=None):
-        leads_all=[]
-        binsize=self.config.cluster_binsize
-        coverage_binsize=self.config.coverage_binsize
-        coverage_shift_bins=self.config.coverage_shift_bins
-        coverage_shift_min_aln_len=self.config.coverage_shift_bins_min_aln_length
-        long_ins_threshold=self.config.long_ins_length*0.5
-        qc_nm=self.config.qc_nm_measure
-        phase=self.config.phase
-        advanced_tags=qc_nm or phase
-        mapq_min=self.config.mapq
-        alen_min=self.config.min_alignment_length
-        nm_sum=0
-        nm_count=0
-        trace_read=self.config.dev_trace_read
-
-        for read in bam.fetch(contig,start,end,until_eof=False):
-            if trace_read!=False:
-                if trace_read==read.query_name:
+    def iter_region(self, bam, contig, start=None, end=None):
+        leads_all = []
+        binsize = self.config.cluster_binsize
+        coverage_binsize = self.config.coverage_binsize
+        coverage_shift_bins = self.config.coverage_shift_bins
+        coverage_shift_min_aln_len = self.config.coverage_shift_bins_min_aln_length
+        long_ins_threshold = self.config.long_ins_length * 0.5
+        qc_nm = self.config.qc_nm_measure
+        phase = self.config.phase
+        advanced_tags = qc_nm or phase
+        mapq_min = self.config.mapq
+        alen_min = self.config.min_alignment_length
+        nm_sum = 0
+        nm_count = 0
+        trace_read = self.config.dev_trace_read
+
+        for read in bam.fetch(contig, start, end, until_eof=False):
+            if trace_read != False:
+                if trace_read == read.query_name:
                     print(f"[DEV_TRACE_READ] [0b/4] [LeadProvider.iter_region] [{contig}:{start}-{end}] [{read.query_name}] has been fetched and is entering pre-filtering")
 
-            #if self.read_count % 1000000 == 0:
+            # if self.read_count % 1000000 == 0:
             #    gc.collect()
             if read.reference_start < start or read.reference_start >= end:
                 continue
 
-            self.read_id+=1
-            self.read_count+=1
+            self.read_id += 1
+            self.read_count += 1
 
-            alen=read.query_alignment_length
+            alen = read.query_alignment_length
             if read.mapping_quality < mapq_min or read.is_secondary or alen < alen_min:
                 continue
 
-            has_sa=read.has_tag("SA")
-            use_clips=self.config.detect_large_ins and not read.is_supplementary and not has_sa
+            has_sa = read.has_tag("SA")
+            use_clips = self.config.detect_large_ins and not read.is_supplementary and not has_sa
 
-            nm=-1
-            curr_read_id=self.read_id
+            nm = -1
+            curr_read_id = self.read_id
             if advanced_tags:
                 if qc_nm:
                     if read.has_tag("NM"):
-                        nm_raw=read.get_tag("NM")
-                        nm_ratio=read.get_tag("NM")/float(read.query_alignment_length+1)
-                        ins_sum,del_sum=get_cigar_indels(curr_read_id,read,contig,self.config,use_clips,read_nm=nm)
-                        nm_adj=(nm_raw-(ins_sum+del_sum))
-                        nm_adj_ratio=nm_adj/float(read.query_alignment_length+1)
-                        nm=nm_adj_ratio
-                        nm_sum+=nm
-                        nm_count+=1
+                        nm_raw = read.get_tag("NM")
+                        nm_ratio = read.get_tag("NM") / float(read.query_alignment_length + 1)
+                        ins_sum, del_sum = get_cigar_indels(curr_read_id, read, contig, self.config, use_clips, read_nm=nm)
+                        nm_adj = (nm_raw - (ins_sum + del_sum))
+                        nm_adj_ratio = nm_adj / float(read.query_alignment_length + 1)
+                        nm = nm_adj_ratio
+                        nm_sum += nm
+                        nm_count += 1
 
                 if phase:
-                    curr_read_id=(self.read_id,str(read.get_tag("HP")) if read.has_tag("HP") else "NULL",str(read.get_tag("PS")) if read.has_tag("PS") else "NULL")
+                    curr_read_id = (self.read_id, str(read.get_tag("HP")) if read.has_tag("HP") else "NULL", str(read.get_tag("PS")) if read.has_tag("PS") else "NULL")
 
-            if trace_read!=False:
-                if trace_read==read.query_name:
+            if trace_read != False:
+                if trace_read == read.query_name:
                     print(f"[DEV_TRACE_READ] [0b/4] [LeadProvider.iter_region] [{contig}:{start}-{end}] [{read.query_name}] passed pre-filtering (whole-read), begin to extract leads")
 
-            #Extract small indels
-            for lead in read_iterindels(curr_read_id,read,contig,self.config,use_clips,read_nm=nm):
-                if trace_read!=False:
-                    if trace_read==read.query_name:
+            # Extract small indels
+            for lead in read_iterindels(curr_read_id, read, contig, self.config, use_clips, read_nm=nm):
+                if trace_read != False:
+                    if trace_read == read.query_name:
                         print(f"[DEV_TRACE_READ] [1/4] [leadprov.read_iterindels] [{contig}:{start}-{end}] [{read.query_name}] new lead: {lead}")
                 yield lead
 
-            #Extract read splits
+            # Extract read splits
             if has_sa:
                 if read.is_supplementary:
-                    if trace_read!=False:
-                        if trace_read==read.query_name:
+                    if trace_read != False:
+                        if trace_read == read.query_name:
                             print(f"[DEV_TRACE_READ] [1/4] [leadprov.read_itersplits_bnd] [{contig}:{start}-{end}] [{read.query_name}] is entering read_itersplits_bnd")
-                    for lead in read_itersplits_bnd(curr_read_id,read,contig,self.config,read_nm=nm):
-                        if trace_read!=False:
-                            if trace_read==read.query_name:
+                    for lead in read_itersplits_bnd(curr_read_id, read, contig, self.config, read_nm=nm):
+                        if trace_read != False:
+                            if trace_read == read.query_name:
                                 print(f"[DEV_TRACE_READ] [1/4] [leadprov.read_itersplits_bnd] [{contig}:{start}-{end}] [{read.query_name}] new lead: {lead}")
                         yield lead
                 else:
-                    if trace_read!=False:
-                        if trace_read==read.query_name:
+                    if trace_read != False:
+                        if trace_read == read.query_name:
                             print(f"[DEV_TRACE_READ] [1/4] [leadprov.read_itersplits] [{contig}:{start}-{end}] [{read.query_name}] is entering read_itersplits")
-                    for lead in read_itersplits(curr_read_id,read,contig,self.config,read_nm=nm):
-                        if trace_read!=False:
-                            if trace_read==read.query_name:
+                    for lead in read_itersplits(curr_read_id, read, contig, self.config, read_nm=nm):
+                        if trace_read != False:
+                            if trace_read == read.query_name:
                                 print(f"[DEV_TRACE_READ] [1/4] [leadprov.read_itersplits] [{contig}:{start}-{end}] [{read.query_name}] new lead: {lead}")
                         yield lead
 
-            #Record in coverage table
-            read_end=read.reference_start+read.reference_length
-            assert(read_end==read.reference_end)
-            #assert(read_end>=read.reference_start)
+            # Record in coverage table
+            read_end = read.reference_start + read.reference_length
+            assert (read_end == read.reference_end)
+            # assert(read_end>=read.reference_start)
             if read.is_reverse:
-                target_tab=self.covrtab_rev
+                target_tab = self.covrtab_rev
             else:
-                target_tab=self.covrtab_fwd
-            covr_start_bin=(int(read.reference_start/coverage_binsize)+coverage_shift_bins*(alen>=coverage_shift_min_aln_len))*coverage_binsize
-            covr_end_bin=(int(read_end/coverage_binsize)-coverage_shift_bins*(alen>=coverage_shift_min_aln_len))*coverage_binsize
+                target_tab = self.covrtab_fwd
+            covr_start_bin = (int(read.reference_start / coverage_binsize) + coverage_shift_bins * (alen >= coverage_shift_min_aln_len)) * coverage_binsize
+            covr_end_bin = (int(read_end / coverage_binsize) - coverage_shift_bins * (alen >= coverage_shift_min_aln_len)) * coverage_binsize
 
             if covr_end_bin > covr_start_bin:
-                self.covrtab_min_bin=min(self.covrtab_min_bin,covr_start_bin)
-                target_tab[covr_start_bin]=target_tab[covr_start_bin]+1 if covr_start_bin in target_tab else 1
+                self.covrtab_min_bin = min(self.covrtab_min_bin, covr_start_bin)
+                target_tab[covr_start_bin] = target_tab[covr_start_bin] + 1 if covr_start_bin in target_tab else 1
 
                 if read_end <= self.end:
-                    target_tab[covr_end_bin]=target_tab[covr_end_bin]-1 if covr_end_bin in target_tab else -1
-
-        self.config.average_regional_nm=nm_sum/float(max(1,nm_count))
-        self.config.qc_nm_threshold=self.config.average_regional_nm
-        #print(f"Contig {contig} avg. regional NM={self.config.average_regional_nm}, threshold={self.config.qc_nm_threshold}")
-
+                    target_tab[covr_end_bin] = target_tab[covr_end_bin] - 1 if covr_end_bin in target_tab else -1
 
-    def dev_leadtab_filename(self,contig,start,end):
-        scriptloc=os.path.dirname(os.path.realpath(sys.argv[0]))
-        if self.config.dev_cache_dir==None:
-            cache_dir=f"{scriptloc}/cache"
+        self.config.average_regional_nm = nm_sum / float(max(1, nm_count))
+        self.config.qc_nm_threshold = self.config.average_regional_nm
+        # print(f"Contig {contig} avg. regional NM={self.config.average_regional_nm}, threshold={self.config.qc_nm_threshold}")
+
+    def dev_leadtab_filename(self, contig, start, end):
+        scriptloc = os.path.dirname(os.path.realpath(sys.argv[0]))
+        if self.config.dev_cache_dir is None:
+            cache_dir = f"{scriptloc}/cache"
         else:
-            cache_dir=self.config.dev_cache_dir
+            cache_dir = self.config.dev_cache_dir
         return f"{cache_dir}/{os.path.basename(self.config.input)}_{contig}_{start}_{end}.pickle"
```

### Comparing `sniffles-2.2/src/sniffles/postprocessing.py` & `sniffles-2.3/src/sniffles/postprocessing.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,426 +1,442 @@
 #!/usr/bin/env python3
 #
 # Sniffles2
 # A fast structural variant caller for long-read sequencing data
 #
-# Created: 27.08.2021
-# Author:  Moritz Smolka
-# Contact: moritz.g.smolka@gmail.com
+# Created:     27.08.2021
+# Author:      Moritz Smolka
+# Maintainer:  Hermann Romanek
+# Contact:     sniffles@romanek.at
 #
 
 from dataclasses import dataclass
 
 import collections
 
 from sniffles import sv
 from sniffles import util
 from sniffles import consensus
 
 import math
 
-def annotate_sv(svcall,config):
+
+def annotate_sv(svcall, config):
     if config.phase:
-        phase=phase_sv(svcall,config)
+        phase = phase_sv(svcall, config)
     else:
-        phase=None
+        phase = None
 
-    genotype_sv(svcall,config,phase)
+    genotype_sv(svcall, config, phase)
 
-    if svcall.svtype=="INS" and not config.symbolic:
-        merged_leads=[l for l in svcall.postprocess.cluster.leads if l.seq!=None]
+    if svcall.svtype == "INS" and not config.symbolic:
+        merged_leads = [l for l in svcall.postprocess.cluster.leads if l.seq is not None]
 
         if len(merged_leads):
-            best_lead=merged_leads[0]
-            best_index=0
-            best_diff=abs(len(best_lead.seq) - svcall.svlen) + abs(best_lead.ref_start - svcall.pos)*1.5
-            for i,ld in enumerate(merged_leads):
-                if i==0:
+            best_lead = merged_leads[0]
+            best_index = 0
+            best_diff = abs(len(best_lead.seq) - svcall.svlen) + abs(best_lead.ref_start - svcall.pos) * 1.5
+            for i, ld in enumerate(merged_leads):
+                if i == 0:
                     continue
-                curr_diff=abs(len(ld.seq) - svcall.svlen) + abs(ld.ref_start - svcall.pos)*1.5
+                curr_diff = abs(len(ld.seq) - svcall.svlen) + abs(ld.ref_start - svcall.pos) * 1.5
                 if curr_diff < best_diff:
-                    best_lead=ld
-                    best_index=i
-                    best_diff=curr_diff
+                    best_lead = ld
+                    best_index = i
+                    best_diff = curr_diff
 
             merged_leads.pop(best_index)
-            #merged_leads_new=list()
+            # merged_leads_new=list()
 
-            #for lead in merged_leads:
+            # for lead in merged_leads:
             #    curr_lendiff=abs(len(ld.seq) - len(best_lead.seq)) + abs(ld.ref_start - best_lead.ref_start)
             #    #if curr_lendiff < 25:
             #    merged_leads_new.append(lead)
-            #merged_leads=merged_leads_new
-
+            # merged_leads=merged_leads_new
 
             if len(merged_leads) >= config.consensus_min_reads and not config.no_consensus:
-                klen=config.consensus_kmer_len
-                skip=config.consensus_kmer_skip_base+int(len(best_lead.seq)*config.consensus_kmer_skip_seqlen_mult)
-                skip_repetitive=skip
+                klen = config.consensus_kmer_len
+                skip = config.consensus_kmer_skip_base + int(len(best_lead.seq) * config.consensus_kmer_skip_seqlen_mult)
+                skip_repetitive = skip
 
-                svcall.alt=consensus.novel_from_reads(best_lead,merged_leads,klen=klen,skip=skip,skip_repetitive=skip_repetitive)
+                svcall.alt = consensus.novel_from_reads(best_lead, merged_leads, klen=klen, skip=skip, skip_repetitive=skip_repetitive)
             else:
-                svcall.alt=best_lead.seq
+                svcall.alt = best_lead.seq
+
+
+def add_request(svcall, field, pos, requests_for_coverage, config):
+    bin = int(pos / config.coverage_binsize) * config.coverage_binsize
+    if bin not in requests_for_coverage:
+        requests_for_coverage[bin] = []
+    requests_for_coverage[bin].append((svcall, field))
+
 
-def add_request(svcall,field,pos,requests_for_coverage,config):
-    bin=int(pos/config.coverage_binsize)*config.coverage_binsize
-    if not bin in requests_for_coverage:
-        requests_for_coverage[bin]=[]
-    requests_for_coverage[bin].append((svcall,field))
-
-def coverage(calls,lead_provider,config):
-    requests_for_coverage=coverage_build_requests(calls,lead_provider,config)
-    return coverage_fulfill(requests_for_coverage,calls,lead_provider,config)
+def coverage(calls, lead_provider, config):
+    requests_for_coverage = coverage_build_requests(calls, lead_provider, config)
+    return coverage_fulfill(requests_for_coverage, calls, lead_provider, config)
 
-def coverage_build_requests(calls,lead_provider,config):
-    requests_for_coverage={}
+
+def coverage_build_requests(calls, lead_provider, config):
+    requests_for_coverage = {}
     for svcall in calls:
-        start=svcall.pos
-        if svcall.svtype=="INS":
-            end=start+1
+        start = svcall.pos
+        if svcall.svtype == "INS":
+            end = start + 1
         else:
-            end=svcall.pos+abs(svcall.svlen)
-        add_request(svcall,"coverage_start",start-config.coverage_binsize,requests_for_coverage,config)
-        add_request(svcall,"coverage_center",int((start+end)/2),requests_for_coverage,config)
-        add_request(svcall,"coverage_end",end+config.coverage_binsize,requests_for_coverage,config)
-        add_request(svcall,"coverage_upstream",start-config.coverage_binsize*config.coverage_updown_bins,requests_for_coverage,config)
-        add_request(svcall,"coverage_downstream",end+config.coverage_binsize*config.coverage_updown_bins,requests_for_coverage,config)
+            end = svcall.pos + abs(svcall.svlen)
+        add_request(svcall, "coverage_start", start - config.coverage_binsize, requests_for_coverage, config)
+        add_request(svcall, "coverage_center", int((start + end) / 2), requests_for_coverage, config)
+        add_request(svcall, "coverage_end", end + config.coverage_binsize, requests_for_coverage, config)
+        add_request(svcall, "coverage_upstream", start - config.coverage_binsize * config.coverage_updown_bins, requests_for_coverage, config)
+        add_request(svcall, "coverage_downstream", end + config.coverage_binsize * config.coverage_updown_bins, requests_for_coverage, config)
     return requests_for_coverage
 
-def coverage_fulfill(requests_for_coverage,calls,lead_provider,config):
-    if len(requests_for_coverage)==0:
-        return -1,-1
-
-    start_bin=lead_provider.covrtab_min_bin
-    end_bin=int(lead_provider.end/config.coverage_binsize)*config.coverage_binsize
-    coverage_fwd=0
-    coverage_rev=0
-    coverage_fwd_total=0
-    coverage_rev_total=0
-    n=0
 
-    for bin in range(start_bin, end_bin+config.coverage_binsize,config.coverage_binsize):
-        n+=1
+def coverage_fulfill(requests_for_coverage, calls, lead_provider, config):
+    if len(requests_for_coverage) == 0:
+        return -1, -1
+
+    start_bin = lead_provider.covrtab_min_bin
+    end_bin = int(lead_provider.end / config.coverage_binsize) * config.coverage_binsize
+    coverage_fwd = 0
+    coverage_rev = 0
+    coverage_fwd_total = 0
+    coverage_rev_total = 0
+    n = 0
+
+    for bin in range(start_bin, end_bin + config.coverage_binsize, config.coverage_binsize):
+        n += 1
 
         if bin in lead_provider.covrtab_fwd:
-            coverage_fwd+=lead_provider.covrtab_fwd[bin]
+            coverage_fwd += lead_provider.covrtab_fwd[bin]
 
         if bin in lead_provider.covrtab_rev:
-            coverage_rev+=lead_provider.covrtab_rev[bin]
+            coverage_rev += lead_provider.covrtab_rev[bin]
 
         if bin in requests_for_coverage:
-            coverage_total_curr=coverage_fwd+coverage_rev
+            coverage_total_curr = coverage_fwd + coverage_rev
             for svcall, field in requests_for_coverage[bin]:
-                setattr(svcall,field,coverage_total_curr)
+                setattr(svcall, field, coverage_total_curr)
 
-        coverage_fwd_total+=coverage_fwd
-        coverage_rev_total+=coverage_rev
+        coverage_fwd_total += coverage_fwd
+        coverage_rev_total += coverage_rev
 
-    average_coverage_fwd=coverage_fwd_total/float(n) if n>0 else 0
-    average_coverage_rev=coverage_rev_total/float(n) if n>0 else 0
-    return average_coverage_fwd,average_coverage_rev
+    average_coverage_fwd = coverage_fwd_total / float(n) if n > 0 else 0
+    average_coverage_rev = coverage_rev_total / float(n) if n > 0 else 0
+    return average_coverage_fwd, average_coverage_rev
 
-def qc_sv_support(svcall,coverage_global,config):
+
+def qc_sv_support(svcall, coverage_global, config):
     if config.mosaic:
         return True
     if config.minsupport == "auto":
-        if not qc_support_auto(svcall,coverage_global,config):
-            svcall.filter="SUPPORT_MIN"
+        if not qc_support_auto(svcall, coverage_global, config):
+            svcall.filter = "SUPPORT_MIN"
             return False
     else:
-        if not qc_support_const(svcall,config):
-            svcall.filter="SUPPORT_MIN"
+        if not qc_support_const(svcall, config):
+            svcall.filter = "SUPPORT_MIN"
             return False
     return True
 
-def rescale_support(svcall,config):
-    if svcall.svtype!="INS" or svcall.svlen < config.long_ins_length:
+
+def rescale_support(svcall, config):
+    if svcall.svtype != "INS" or svcall.svlen < config.long_ins_length:
         return svcall.support
     else:
-        base=svcall.support + svcall.get_info("SUPPORT_LONG")
-        scale_factor=config.long_ins_rescale_mult*(float(svcall.svlen)/config.long_ins_length)
-        return round(base*(config.long_ins_rescale_base+scale_factor))
-
-def qc_support_auto(svcall,coverage_global,config):
-    support=rescale_support(svcall,config)
-    #if svcall.svtype=="INS":
+        base = svcall.support + svcall.get_info("SUPPORT_LONG")
+        scale_factor = config.long_ins_rescale_mult * (float(svcall.svlen) / config.long_ins_length)
+        return round(base * (config.long_ins_rescale_base + scale_factor))
+
+
+def qc_support_auto(svcall, coverage_global, config):
+    support = rescale_support(svcall, config)
+    # if svcall.svtype=="INS":
     #    coverage_list=[svcall.coverage_center]
-    #else:
-    coverage_list=[svcall.coverage_upstream,svcall.coverage_downstream]
-    coverage_list=[c for c in coverage_list if c!=None and c!=0]
-    if len(coverage_list)==0:
-        coverage_list=[svcall.coverage_start,svcall.coverage_center,svcall.coverage_end]
-        coverage_list=[c for c in coverage_list if c!=None and c!=0]
+    # else:
+    coverage_list = [svcall.coverage_upstream, svcall.coverage_downstream]
+    coverage_list = [c for c in coverage_list if c != None and c != 0]
+    if len(coverage_list) == 0:
+        coverage_list = [svcall.coverage_start, svcall.coverage_center, svcall.coverage_end]
+        coverage_list = [c for c in coverage_list if c != None and c != 0]
 
-    if len(coverage_list)==0:
-        coverage_regional=coverage_global
+    if len(coverage_list) == 0:
+        coverage_regional = coverage_global
     else:
-        coverage_regional=round(sum(coverage_list)/len(coverage_list))
-        if coverage_regional==0:
-            coverage_regional=coverage_global
-    coverage=(coverage_regional*config.minsupport_auto_regional_coverage_weight+coverage_global*(1.0-config.minsupport_auto_regional_coverage_weight))
-    min_support=round(config.minsupport_auto_base+config.minsupport_auto_mult*coverage)
+        coverage_regional = round(sum(coverage_list) / len(coverage_list))
+        if coverage_regional == 0:
+            coverage_regional = coverage_global
+    coverage = (coverage_regional * config.minsupport_auto_regional_coverage_weight + coverage_global * (1.0 - config.minsupport_auto_regional_coverage_weight))
+    min_support = round(config.minsupport_auto_base + config.minsupport_auto_mult * coverage)
     return support >= min_support
-    #return True
+    # return True
+
 
-def qc_support_const(svcall,config):
-    #svcall.set_info("MINSUPPORT",config.minsupport)
+def qc_support_const(svcall, config):
+    # svcall.set_info("MINSUPPORT",config.minsupport)
     return svcall.support >= config.minsupport
 
-def qc_sv(svcall,config):
-    af=svcall.get_info("AF")
-    af=af if af!=None else 0
+
+def qc_sv(svcall, config):
+    af = svcall.get_info("AF")
+    af = af if af != None else 0
     sv_is_mosaic = af <= config.mosaic_af_max
 
     if config.qc_stdev:
-        stdev_pos=svcall.get_info("STDEV_POS")
+        stdev_pos = svcall.get_info("STDEV_POS")
         if stdev_pos > config.qc_stdev_abs_max:
-            svcall.filter="STDEV_POS"
+            svcall.filter = "STDEV_POS"
             return False
-        if svcall.svtype!="BND" and stdev_pos / abs(svcall.svlen) > 2.0:
-            svcall.filter="STDEV_POS"
+        if svcall.svtype != "BND" and stdev_pos / abs(svcall.svlen) > 2.0:
+            svcall.filter = "STDEV_POS"
             return False
 
         stdev_len = svcall.get_info("STDEV_LEN")
         if stdev_len != None:
             if svcall.svtype != "BND" and stdev_len / abs(svcall.svlen) > 1.0:
-                svcall.filter="STDEV_LEN"
+                svcall.filter = "STDEV_LEN"
                 return False
             if stdev_len > config.qc_stdev_abs_max:
-                svcall.filter="STDEV_LEN"
+                svcall.filter = "STDEV_LEN"
                 return False
 
     if abs(svcall.svlen) < config.minsvlen:
-        svcall.filter="SVLEN_MIN"
+        svcall.filter = "SVLEN_MIN"
         return False
 
-    if svcall.svtype=="BND":
-        if config.qc_bnd_filter_strand and len(set(l.strand for l in svcall.postprocess.cluster.leads))<2:
-            svcall.filter="STRAND"
+    if svcall.svtype == "BND":
+        if config.qc_bnd_filter_strand and len(set(l.strand for l in svcall.postprocess.cluster.leads)) < 2:
+            svcall.filter = "STRAND"
             return False
     elif ((config.mosaic and sv_is_mosaic) and config.mosaic_qc_strand) or (not (config.mosaic and sv_is_mosaic) and config.qc_strand):
-        is_long_ins=(svcall.svtype=="INS" and svcall.svlen >= config.long_ins_length)
-        if not is_long_ins and len(set(l.strand for l in svcall.postprocess.cluster.leads))<2:
-            svcall.filter="STRAND"
+        is_long_ins = (svcall.svtype == "INS" and svcall.svlen >= config.long_ins_length)
+        if not is_long_ins and len(set(l.strand for l in svcall.postprocess.cluster.leads)) < 2:
+            svcall.filter = "STRAND"
             return False
 
     if config.mosaic and sv_is_mosaic:
-        if svcall.svtype=="INV" or svcall.svtype=="DUP" and svcall.svlen < config.mosaic_qc_invdup_min_length:
-            svcall.filter="SVLEN_MIN"
+        if svcall.svtype == "INV" or svcall.svtype == "DUP" and svcall.svlen < config.mosaic_qc_invdup_min_length:
+            svcall.filter = "SVLEN_MIN"
             return False
 
-    #if (svcall.coverage_upstream != None and svcall.coverage_upstream < config.qc_coverage) or (svcall.coverage_downstream != None and svcall.coverage_downstream < config.qc_coverage):
+    # if (svcall.coverage_upstream != None and svcall.coverage_upstream < config.qc_coverage) or (svcall.coverage_downstream != None and svcall.coverage_downstream < config.qc_coverage):
     if svcall.svtype != "DEL" and svcall.svtype != "INS" and (svcall.coverage_center != None and svcall.coverage_center < config.qc_coverage):
-        svcall.filter="COV_MIN"
+        svcall.filter = "COV_MIN"
         return False
 
     if svcall.svtype == "DEL" and config.long_del_length != -1 and abs(svcall.svlen) >= config.long_del_length and not config.mosaic:
-        if svcall.coverage_center != None and svcall.coverage_upstream != None and svcall.coverage_downstream != None and svcall.coverage_center > (svcall.coverage_upstream+svcall.coverage_downstream)/2.0 * config.long_del_coverage:
-            svcall.filter="COV_CHANGE"
+        if svcall.coverage_center != None and svcall.coverage_upstream != None and svcall.coverage_downstream != None and svcall.coverage_center > (svcall.coverage_upstream + svcall.coverage_downstream) / 2.0 * config.long_del_coverage:
+            svcall.filter = "COV_CHANGE"
             return False
-    elif svcall.svtype=="INS" and ( (svcall.coverage_upstream != None and svcall.coverage_upstream < config.qc_coverage) or (svcall.coverage_downstream != None and svcall.coverage_downstream < config.qc_coverage)):
-        svcall.filter="COV_CHANGE"
+    elif svcall.svtype == "INS" and ((svcall.coverage_upstream != None and svcall.coverage_upstream < config.qc_coverage) or (svcall.coverage_downstream != None and svcall.coverage_downstream < config.qc_coverage)):
+        svcall.filter = "COV_CHANGE"
         return False
     elif svcall.svtype == "DUP" and config.long_dup_length != -1 and abs(svcall.svlen) >= config.long_dup_length and not config.mosaic:
-        if svcall.coverage_center != None and svcall.coverage_upstream != None and svcall.coverage_downstream != None and svcall.coverage_center < (svcall.coverage_upstream+svcall.coverage_downstream)/2.0 * config.long_dup_coverage:
-            svcall.filter="COV_CHANGE"
+        if svcall.coverage_center != None and svcall.coverage_upstream != None and svcall.coverage_downstream != None and svcall.coverage_center < (svcall.coverage_upstream + svcall.coverage_downstream) / 2.0 * config.long_dup_coverage:
+            svcall.filter = "COV_CHANGE"
             return False
 
-    qc_coverage_max_change_frac=config.qc_coverage_max_change_frac
+    qc_coverage_max_change_frac = config.qc_coverage_max_change_frac
     if config.mosaic and sv_is_mosaic:
-        qc_coverage_max_change_frac=config.mosaic_qc_coverage_max_change_frac
+        qc_coverage_max_change_frac = config.mosaic_qc_coverage_max_change_frac
     if qc_coverage_max_change_frac != -1.0:
-        if svcall.coverage_upstream!=None and svcall.coverage_upstream!=0:
-            u=float(svcall.coverage_upstream)
+        if svcall.coverage_upstream != None and svcall.coverage_upstream != 0:
+            u = float(svcall.coverage_upstream)
         else:
-            u=1.0
+            u = 1.0
 
-        if svcall.coverage_start!=None and svcall.coverage_start!=0:
-            s=float(svcall.coverage_start)
+        if svcall.coverage_start != None and svcall.coverage_start != 0:
+            s = float(svcall.coverage_start)
         else:
-            s=1.0
+            s = 1.0
 
-        if svcall.coverage_center!=None and svcall.coverage_center!=0:
-            c=float(svcall.coverage_center)
+        if svcall.coverage_center != None and svcall.coverage_center != 0:
+            c = float(svcall.coverage_center)
         else:
-            c=1.0
+            c = 1.0
 
-        if svcall.coverage_end!=None and svcall.coverage_end!=0:
-            e=float(svcall.coverage_end)
+        if svcall.coverage_end != None and svcall.coverage_end != 0:
+            e = float(svcall.coverage_end)
         else:
-            e=1.0
+            e = 1.0
 
-        if svcall.coverage_downstream!=None and svcall.coverage_downstream!=0:
-            d=float(svcall.coverage_downstream)
+        if svcall.coverage_downstream != None and svcall.coverage_downstream != 0:
+            d = float(svcall.coverage_downstream)
         else:
-            d=1.0
+            d = 1.0
 
-        if abs(u-s)/max(u,s) > qc_coverage_max_change_frac:
-            svcall.filter="COV_CHANGE_FRAC"
+        if abs(u - s) / max(u, s) > qc_coverage_max_change_frac:
+            svcall.filter = "COV_CHANGE_FRAC"
             return False
 
-        if abs(s-c)/max(s,c) > qc_coverage_max_change_frac:
-            svcall.filter="COV_CHANGE_FRAC"
+        if abs(s - c) / max(s, c) > qc_coverage_max_change_frac:
+            svcall.filter = "COV_CHANGE_FRAC"
             return False
 
-        if abs(c-e)/max(c,e) > qc_coverage_max_change_frac:
-            svcall.filter="COV_CHANGE_FRAC"
+        if abs(c - e) / max(c, e) > qc_coverage_max_change_frac:
+            svcall.filter = "COV_CHANGE_FRAC"
             return False
 
-        if abs(e-d)/max(e,d) > qc_coverage_max_change_frac:
-            svcall.filter="COV_CHANGE_FRAC"
+        if abs(e - d) / max(e, d) > qc_coverage_max_change_frac:
+            svcall.filter = "COV_CHANGE_FRAC"
             return False
 
     return True
 
-def qc_sv_post_annotate(svcall,config):
-    af=svcall.get_info("AF")
-    af=af if af!=None else 0
+
+def qc_sv_post_annotate(svcall, config):
+    af = svcall.get_info("AF")
+    af = af if af != None else 0
     sv_is_mosaic = af <= config.mosaic_af_max
 
-    if (len(svcall.genotypes)==0 or (svcall.genotypes[0][0]!="." and svcall.genotypes[0][0]+svcall.genotypes[0][1]<2)) and (svcall.coverage_center != None and svcall.coverage_center < config.qc_coverage):
-        svcall.filter="COV_MIN"
+    if (len(svcall.genotypes) == 0 or (svcall.genotypes[0][0] != "." and svcall.genotypes[0][0] + svcall.genotypes[0][1] < 2)) and (svcall.coverage_center != None and svcall.coverage_center < config.qc_coverage):
+        svcall.filter = "COV_MIN"
         return False
 
-    qc_nm=config.qc_nm
-    qc_nm_threshold=config.qc_nm_threshold*config.qc_nm_mult
+    qc_nm = config.qc_nm
+    qc_nm_threshold = config.qc_nm_threshold * config.qc_nm_mult
     if config.mosaic and sv_is_mosaic:
-        qc_nm=config.mosaic_qc_nm
-        qc_nm_threshold=config.qc_nm_threshold*config.qc_nm_mult
-    if qc_nm and svcall.nm > qc_nm_threshold and (len(svcall.genotypes)==0 or svcall.genotypes[0][1]==0):
-        svcall.filter="ALN_NM"
+        qc_nm = config.mosaic_qc_nm
+        qc_nm_threshold = config.qc_nm_threshold * config.qc_nm_mult
+    if qc_nm and svcall.nm > qc_nm_threshold and (len(svcall.genotypes) == 0 or svcall.genotypes[0][1] == 0):
+        svcall.filter = "ALN_NM"
         return False
 
     if config.mosaic:
-        if sv_is_mosaic and ( af < config.mosaic_af_min or af > config.mosaic_af_max ):
-            svcall.filter="MOSAIC_AF"
+        if sv_is_mosaic and (af < config.mosaic_af_min or af > config.mosaic_af_max):
+            svcall.filter = "MOSAIC_AF"
             return False
         elif not sv_is_mosaic and not config.mosaic_include_germline:
-            svcall.filter="MOSAIC_AF"
+            svcall.filter = "MOSAIC_AF"
             return False
 
     return True
 
-def binomial_coef(n,k):
-    return math.factorial(n)/(math.factorial(k)*math.factorial(n-k))
 
-def binomial_probability(k,n,p):
+def binomial_coef(n, k):
+    return math.factorial(n) / (math.factorial(k) * math.factorial(n - k))
+
+
+def binomial_probability(k, n, p):
     try:
-        #Binomial coef cancels out for likelihood ratios
-        #return binomial_coef(n,k) * (p**k) * ((1.0-p)**(n-k))
-        return (p**k) * ((1.0-p)**(n-k))
+        # Binomial coef cancels out for likelihood ratios
+        # return binomial_coef(n,k) * (p**k) * ((1.0-p)**(n-k))
+        return (p ** k) * ((1.0 - p) ** (n - k))
     except OverflowError:
         return 1.0
 
-def likelihood_ratio(q1,q2):
-    if q1/q2>0:
+
+def likelihood_ratio(q1, q2):
+    if q1 / q2 > 0:
         try:
-            return math.log(q1/q2,10)
+            return math.log(q1 / q2, 10)
         except ValueError:
             return 0
     else:
         return 0
 
-def genotype_sv(svcall,config,phase):
-    normalization_target=250
-    hom_ref_p=config.genotype_error
-    het_p=(1.0/config.genotype_ploidy) # - config.genotype_error
-    hom_var_p=1.0 - config.genotype_error
-    coverage=0
-
-    #Count inline events only once per read, but split events as individual alignments, as in coverage calculation
-    leads=svcall.postprocess.cluster.leads
-    support=rescale_support(svcall,config)
 
-    if svcall.svtype=="INS":
-        coverage_list=[svcall.coverage_center]
+def genotype_sv(svcall, config, phase):
+    normalization_target = 250
+    hom_ref_p = config.genotype_error
+    het_p = (1.0 / config.genotype_ploidy)  # - config.genotype_error
+    hom_var_p = 1.0 - config.genotype_error
+    coverage = 0
+
+    # Count inline events only once per read, but split events as individual alignments, as in coverage calculation
+    leads = svcall.postprocess.cluster.leads
+    support = rescale_support(svcall, config)
+
+    if svcall.svtype == "INS":
+        coverage_list = [svcall.coverage_center]
     else:
-        if svcall.svtype=="DUP":
-            if False and svcall.coverage_start!=None and svcall.coverage_end!=None:
-                if svcall.coverage_start>svcall.coverage_end:
-                    coverage_list=[svcall.coverage_end]
+        if svcall.svtype == "DUP":
+            if False and svcall.coverage_start != None and svcall.coverage_end != None:
+                if svcall.coverage_start > svcall.coverage_end:
+                    coverage_list = [svcall.coverage_end]
                 else:
-                    coverage_list=[svcall.coverage_start]
+                    coverage_list = [svcall.coverage_start]
             else:
-                coverage_list=[svcall.coverage_start,svcall.coverage_end]
-            coverage+=round(support*0.75)
-        elif svcall.svtype=="INV":
-            coverage_list=[svcall.coverage_upstream,svcall.coverage_downstream]
-            coverage+=round(support*0.5)
+                coverage_list = [svcall.coverage_start, svcall.coverage_end]
+            coverage += round(support * 0.75)
+        elif svcall.svtype == "INV":
+            coverage_list = [svcall.coverage_upstream, svcall.coverage_downstream]
+            coverage += round(support * 0.5)
         else:
-            coverage_list=[svcall.coverage_start,svcall.coverage_center,svcall.coverage_end]
+            coverage_list = [svcall.coverage_start, svcall.coverage_center, svcall.coverage_end]
 
-    coverage_list=[c for c in coverage_list if c!=None and c!=0]
-    if len(coverage_list)==0:
+    coverage_list = [c for c in coverage_list if c != None and c != 0]
+    if len(coverage_list) == 0:
         return
-    coverage+=round(sum(coverage_list)/len(coverage_list))
+    coverage += round(sum(coverage_list) / len(coverage_list))
 
     if support > coverage:
-        coverage=support
+        coverage = support
 
-    af=support / float(coverage)
+    af = support / float(coverage)
 
-    genotype_p=[((0,0),hom_ref_p),
-                ((0,1),het_p),
-                ((1,1),hom_var_p)]
-
-    max_lead=max(support,coverage)
-    if max_lead>normalization_target:
-        norm=normalization_target/float(max_lead)
-        normalized_support=round(support*norm)
-        normalized_coverage=round(coverage*norm)
+    genotype_p = [((0, 0), hom_ref_p),
+                  ((0, 1), het_p),
+                  ((1, 1), hom_var_p)]
+
+    max_lead = max(support, coverage)
+    if max_lead > normalization_target:
+        norm = normalization_target / float(max_lead)
+        normalized_support = round(support * norm)
+        normalized_coverage = round(coverage * norm)
     else:
-        normalized_support=support
-        normalized_coverage=coverage
+        normalized_support = support
+        normalized_coverage = coverage
 
-    genotype_likelihoods=[]
+    genotype_likelihoods = []
     for gt, p in genotype_p:
-        q=binomial_probability(normalized_support,normalized_coverage,p)
-        genotype_likelihoods.append((gt,q))
+        q = binomial_probability(normalized_support, normalized_coverage, p)
+        genotype_likelihoods.append((gt, q))
     genotype_likelihoods.sort(key=lambda k: k[1], reverse=True)
 
-    sum_likelihoods=sum(q for gt,q in genotype_likelihoods)
-    normalized_likelihoods=[ (gt,(q/sum_likelihoods)) for gt,q in genotype_likelihoods]
+    sum_likelihoods = sum(q for gt, q in genotype_likelihoods)
+    normalized_likelihoods = [(gt, (q / sum_likelihoods)) for gt, q in genotype_likelihoods]
 
-    gt1,q1=normalized_likelihoods[0]
-    gt2,q2=normalized_likelihoods[1]
-    qz=[q for gt,q in normalized_likelihoods if gt==(0,0)][0]
-    genotype_z_score = min(60,int((-10) * likelihood_ratio(qz,q1)))
-    genotype_quality = min(60,int((-10) * likelihood_ratio(q2,q1)))
+    gt1, q1 = normalized_likelihoods[0]
+    gt2, q2 = normalized_likelihoods[1]
+    qz = [q for gt, q in normalized_likelihoods if gt == (0, 0)][0]
+    genotype_z_score = min(60, int((-10) * likelihood_ratio(qz, q1)))
+    genotype_quality = min(60, int((-10) * likelihood_ratio(q2, q1)))
 
-    is_long_ins=(svcall.svtype=="INS" and svcall.svlen >= config.long_ins_length and config.detect_large_ins)
+    is_long_ins = (svcall.svtype == "INS" and svcall.svlen >= config.long_ins_length and config.detect_large_ins)
     if genotype_z_score < config.genotype_min_z_score and not config.mosaic and not is_long_ins:
-        if svcall.filter=="PASS":
-            svcall.filter="GT"
+        if svcall.filter == "PASS":
+            svcall.filter = "GT"
 
-    if is_long_ins and gt1==(0,0):
-        a,b=".","."
+    if is_long_ins and gt1 == (0, 0):
+        a, b = ".", "."
     else:
-        a,b=gt1
-    svcall.genotypes[0]=(a,b,genotype_quality,coverage-support,support,phase)
-    svcall.set_info("AF",af)
-
-def phase_sv(svcall,config):
-    reads_phases={lead.read_id[0]: (lead.read_id[1],lead.read_id[2]) for lead in svcall.postprocess.cluster.leads}
-    hp_list=util.most_common(hp for hp,ps in reads_phases.values())
-    ps_list=util.most_common(ps for hp,ps in reads_phases.values())
-
-    hp_support,hp=hp_list[0]
-    ps_support,ps=ps_list[0]
-    if hp==None:
-        hp="NULL"
-    if ps==None:
-        ps="NULL"
-
-    other_hp_support=sum(other_supp for other_supp, other_hp in hp_list if other_hp != hp and other_hp != "NULL")
-    other_ps_support=sum(other_supp for other_supp, other_ps in ps_list if other_ps != ps and other_ps != "NULL")
-
-    hp_filter="FAIL"
-    if hp != "NULL" and hp_support > 0 and float(other_hp_support)/(hp_support+other_hp_support) < config.phase_conflict_threshold:
-        hp_filter="PASS"
-
-    ps_filter="FAIL"
-    if ps != "NULL" and ps_support > 0 and float(other_ps_support)/(ps_support+other_ps_support) < config.phase_conflict_threshold:
-        ps_filter="PASS"
+        a, b = gt1
+    svcall.genotypes[0] = (a, b, genotype_quality, coverage - support, support, phase)
+    svcall.set_info("AF", af)
+
+
+def phase_sv(svcall, config):
+    reads_phases = {lead.read_id[0]: (lead.read_id[1], lead.read_id[2]) for lead in svcall.postprocess.cluster.leads}
+    hp_list = util.most_common(hp for hp, ps in reads_phases.values())
+    ps_list = util.most_common(ps for hp, ps in reads_phases.values())
+
+    hp_support, hp = hp_list[0]
+    ps_support, ps = ps_list[0]
+    if hp is None:
+        hp = "NULL"
+    if ps is None:
+        ps = "NULL"
+
+    other_hp_support = sum(other_supp for other_supp, other_hp in hp_list if other_hp != hp and other_hp != "NULL")
+    other_ps_support = sum(other_supp for other_supp, other_ps in ps_list if other_ps != ps and other_ps != "NULL")
+
+    hp_filter = "FAIL"
+    if hp != "NULL" and hp_support > 0 and float(other_hp_support) / (hp_support + other_hp_support) < config.phase_conflict_threshold:
+        hp_filter = "PASS"
+
+    ps_filter = "FAIL"
+    if ps != "NULL" and ps_support > 0 and float(other_ps_support) / (ps_support + other_ps_support) < config.phase_conflict_threshold:
+        ps_filter = "PASS"
 
-    svcall.set_info("PHASE",f"{hp},{ps},{hp_support},{ps_support},{hp_filter},{ps_filter}")
-    return (config.phase_identifiers.index(hp) if hp in config.phase_identifiers else None if hp_filter=="PASS" else None)
+    svcall.set_info("PHASE", f"{hp},{ps},{hp_support},{ps_support},{hp_filter},{ps_filter}")
+    return config.phase_identifiers.index(hp) if hp in config.phase_identifiers else None if hp_filter == "PASS" else None
```

### Comparing `sniffles-2.2/src/sniffles/sv.py` & `sniffles-2.3/src/sniffles/sv.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,499 +1,610 @@
 #!/usr/bin/env python3
 #
 # Sniffles2
 # A fast structural variant caller for long-read sequencing data
 #
-# Created: 15.08.2021
-# Author:  Moritz Smolka
-# Contact: moritz.g.smolka@gmail.com
+# Created:     15.08.2021
+# Author:      Moritz Smolka
+# Maintainer:  Hermann Romanek
+# Contact:     sniffles@romanek.at
 #
-
+import logging
 from dataclasses import dataclass
+from typing import Optional, Callable
+
+try:
+    from edlib import align
+except ImportError:
+    logging.getLogger('sniffles.dependencies').info('Dependency edlib not installed - alignments are disabled.')
+    align: Optional[Callable] = None
 
 from sniffles import util
 
-TYPES=["INS","DEL","DUP","INV","BND"]
+TYPES = ["INS", "DEL", "DUP", "INV", "BND"]
+
 
 @dataclass
 class SVCallBNDInfo:
     mate_contig: str
     mate_ref_start: int
     is_first: bool
-    is_reverse:bool
+    is_reverse: bool
+
 
 @dataclass
 class SVCallPostprocessingInfo:
     cluster: list
 
+
 @dataclass
 class SVCall:
     contig: str
     pos: int
     id: str
     ref: str
     alt: str
     qual: int
     filter: str
     info: dict
 
     svtype: str
     svlen: int
     end: int
-    genotypes: dict
+    genotypes: dict[int, tuple]
 
     precise: bool
     support: int
-    rnames: list
+    rnames: list[str]
 
     qc: bool
     nm: float
-    postprocess: SVCallPostprocessingInfo
+    postprocess: Optional[SVCallPostprocessingInfo]
 
     fwd: int = None
     rev: int = None
 
     coverage_upstream: int = None
     coverage_downstream: int = None
     coverage_start: int = None
     coverage_center: int = None
     coverage_end: int = None
 
-    def set_info(self,k,v):
-        self.info[k]=v
+    sample_internal_id: int = None
+    bnd_info: SVCallBNDInfo = None
+
+    raw_vcf_line: Optional[str] = None
+    raw_vcf_line_index: Optional[int] = None
+
+    _counter = 0
 
-    def get_info(self,k):
+    def set_info(self, k, v):
+        self.info[k] = v
+
+    def get_info(self, k):
         return self.info[k] if k in self.info else None
 
-    def has_info(self,k):
+    def has_info(self, k):
         return k in self.info
 
     def finalize(self):
-        self.postprocess=None
+        self.postprocess = None
+
 
 @dataclass
 class SVGroup:
-    candidates: list
+    """
+    For combining grouped SV calls from multiple .snf samples into one SV call
+    """
+    candidates: list[SVCall]
     pos_mean: float
     len_mean: float
     included_samples: set
     coverages_nonincluded: dict
 
-def calculate_bounds(svtype,ref_start_mode,svlen_mode):
-    if svtype=="INS":
-        svstart=ref_start_mode
-        svend=ref_start_mode
-    elif svtype=="DEL":
-        svstart=ref_start_mode+svlen_mode
-        svend=ref_start_mode
+    bnd_mate_ref_start_mean: float = None
+
+    # _pos_mean: float = None
+    # _len_mean: float = None
+
+    _counter = 0
+
+    def __new__(cls, *args, **kwargs):
+        cls._counter += 1
+        return super().__new__(cls)
+
+    def __del__(self):
+        SVGroup._counter -= 1
+
+    # @property
+    # def pos_mean(self) -> float:
+    #     if self._pos_mean is None:
+    #         self._pos_mean = util.mean(c.pos for c in self.candidates)
+    #     return self._pos_mean
+    #
+    # @property
+    # def len_mean(self) -> float:
+    #     if self._len_mean is None:
+    #         self._len_mean = util.mean(c.svlen for c in self.candidates)
+    #     return self._len_mean
+
+    @classmethod
+    def from_candidate(cls, candidate: SVCall) -> "SVGroup":
+        """
+        Start a new group from given candidate.
+        """
+        obj = cls(
+            candidates=[candidate],
+            pos_mean=float(candidate.pos),
+            len_mean=float(abs(candidate.svlen)),
+            included_samples={candidate.sample_internal_id},
+            coverages_nonincluded=dict()
+        )
+        if candidate.svtype == "BND":
+            obj.bnd_mate_contig = candidate.bnd_info.mate_contig
+            obj.bnd_mate_ref_start_mean = candidate.bnd_info.mate_ref_start
+        return obj
+
+    def align_call(self, candidate: SVCall, limit: float) -> bool:
+        """
+        Check if the candidate aligns with this group better than given limit.
+        """
+        if not limit or align is None:
+            return True
+
+        distance = align(self.candidates[0].alt, candidate.alt)['editDistance']
+
+        return ((self.len_mean-distance) / self.len_mean) > limit
+
+    def check_call(self):
+        """
+        Checks if this group is a fit for the given candidate, and adds the candidate if it is. Returns true
+        if the candidate was added to this group, false otherwise.
+        """
+
+    def add_candidate(self, candidate: SVCall):
+        """
+        Adds a candidate to this group, updating mean position, length
+        and optionally bnd ref start.
+        """
+        group_size = len(self.candidates)
+        self.pos_mean *= group_size
+        self.len_mean *= group_size
+        self.pos_mean += candidate.pos
+        self.len_mean += abs(candidate.svlen)
+        if candidate.svtype == "BND":
+            self.bnd_mate_ref_start_mean *= group_size
+            self.bnd_mate_ref_start_mean += candidate.bnd_info.mate_ref_start
+
+        self.candidates.append(candidate)
+        group_size += 1
+        self.pos_mean /= group_size
+        self.len_mean /= group_size
+        self.included_samples.add(candidate.sample_internal_id)
+
+        if candidate.svtype == "BND":
+            self.bnd_mate_ref_start_mean /= group_size
+
+    def call(self, config, task) -> Optional[SVCall]:
+        """
+        Call this group, returning either an SVCall or None.
+        """
+        first_cand = self.candidates[0]
+
+        # Filtering
+        samples_count = float(len(config.snf_input_info))
+        sample_internal_ids = set(sample["internal_id"] for sample in config.snf_input_info)
+        total_count = len(self.included_samples)
+        pass_count = sum(cand.qc for cand in self.candidates)
+        qc = (pass_count > 0 and pass_count / samples_count >= config.combine_high_confidence) or (
+                    total_count / samples_count >= config.combine_low_confidence and total_count >= config.combine_low_confidence_abs)
+
+        if not qc:
+            return None
+
+        if (not config.combine_output_filtered) and not any(cand.qc and cand.filter == "PASS" for cand in self.candidates):
+            return None
+
+        rnames = [] if config.output_rnames else None
+        genotypes = {}
+
+        for cand in self.candidates:
+            if rnames is not None and cand.rnames is not None:
+                rnames.extend(cand.rnames)
+
+            if 0 not in cand.genotypes:
+                cand.genotypes[0] = (".", ".", 0, 0, cand.support, None)
+            if cand.sample_internal_id in genotypes:
+                # Intra-sample merging
+                a, b, gt_qual, dr, dv, ps = cand.genotypes[0]
+                curr_a, curr_b, curr_gt_qual, curr_dr, curr_dv, curr_ps, curr_id = genotypes[cand.sample_internal_id]
+                new_id = curr_id + "," + config.id_prefix + cand.id
+                if (curr_a == ".") or (a != "." and (a, b) >= (curr_a, curr_b)):
+                    genotypes[cand.sample_internal_id] = (a, b, gt_qual, dr, dv, ps, new_id)
+                else:
+                    genotypes[cand.sample_internal_id] = (curr_a, curr_b, curr_gt_qual, curr_dr, curr_dv, curr_ps, new_id)
+            else:
+                a, b, gt_qual, dr, dv, ps = cand.genotypes[0]
+                genotypes[cand.sample_internal_id] = (a, b, gt_qual, dr, dv, ps, config.id_prefix + cand.id)
+
+        for sample_internal_id in sample_internal_ids:
+            if sample_internal_id in genotypes:
+                continue
+            coverage = self.coverages_nonincluded[sample_internal_id]
+            if coverage >= config.combine_null_min_coverage:
+                genotypes[sample_internal_id] = (0, 0, 0, coverage, 0, None, "NULL")
+            else:
+                genotypes[sample_internal_id] = (".", ".", 0, coverage, 0, None, "NULL")
+
+        if config.combine_consensus:
+            genotypes_consensus = {}
+            for a, b, gt_qual, dr, dv in genotypes.values():
+                if not (a, b) in genotypes_consensus:
+                    genotypes_consensus[(a, b)] = {"count": 0, "qual": list(), "dr": list(), "dv": list()}
+                genotypes_consensus[(a, b)]["count"] += 1
+                genotypes_consensus[(a, b)]["qual"].append(gt_qual)
+                genotypes_consensus[(a, b)]["dr"].append(dr)
+                genotypes_consensus[(a, b)]["dv"].append(dv)
+            most_common_count = genotypes_consensus[sorted(genotypes_consensus, key=lambda k: genotypes_consensus[k]["count"], reverse=True)[0]]["count"]
+            most_common_gt = [gt for gt in genotypes_consensus if genotypes_consensus[gt]["count"] == most_common_count]
+            cons_a, cons_b = max(most_common_gt)
+            consensus_info = genotypes_consensus[(cons_a, cons_b)]
+            genotypes = {0: (cons_a, cons_b, int(sum(consensus_info["qual"]) / consensus_info["count"]), sum(consensus_info["dr"]), sum(consensus_info["dv"]))}
+            if cons_a != 1 and cons_b != 1:
+                return None
+
+        if config.combine_pair_relabel:
+            max_gt = (0, 0)
+            for sample_id in genotypes:
+                a, b, qual, dr, dv, ps, new_id = genotypes[sample_id]
+                if qual > config.combine_pair_relabel_threshold and a != ".":
+                    max_gt = max(max_gt, (a, b))
+
+            if max_gt != (0, 0):
+                for sample_id in genotypes:
+                    a, b, qual, dr, dv, ps, new_id = genotypes[sample_id]
+                    if qual < config.combine_pair_relabel_threshold and a != ".":
+                        max_a, max_b = max_gt
+                        genotypes[sample_id] = (max_a, max_b, qual, dr, dv, ps, new_id)
+
+        svcall_pos = int(util.median(cand.pos for cand in self.candidates))
+        svcall_svlen = int(util.median(cand.svlen for cand in self.candidates))
+        svcall_alt = first_cand.alt
+        svcall_alt_mindist = abs(len(svcall_alt) - svcall_svlen)
+        if first_cand.svtype == "INS":
+            svcall_end = svcall_pos
+            for cand in self.candidates:
+                dist = abs(len(cand.alt) - svcall_svlen)
+                if dist < svcall_alt_mindist:
+                    svcall_alt_mindist = dist
+                    svcall_alt = cand.alt
+        else:
+            svcall_end = svcall_pos + abs(svcall_svlen)
+
+        svcall = SVCall(contig=first_cand.contig,
+                        pos=svcall_pos if config.dev_combine_medians else first_cand.pos,
+                        id=f"{first_cand.svtype}.{task.sv_id:X}M{task.id:X}",
+                        ref="N",
+                        alt=svcall_alt,
+                        qual=round(util.mean(int(cand.qual) for cand in self.candidates)),
+                        filter="PASS",
+                        info=dict(),
+                        svtype=first_cand.svtype,
+                        svlen=svcall_svlen if config.dev_combine_medians else first_cand.svlen,
+                        end=svcall_end if config.dev_combine_medians else first_cand.end,
+                        genotypes=genotypes,
+                        precise=sum(int(cand.precise) for cand in self.candidates) / float(len(self.candidates)) > 0.5,
+                        support=round(util.mean(cand.support for cand in self.candidates)),
+                        rnames=rnames,
+                        postprocess=None,
+                        qc=True,
+                        nm=-1,
+                        fwd=sum(cand.fwd for cand in self.candidates),
+                        rev=sum(cand.rev for cand in self.candidates),
+                        coverage_upstream=util.mean_or_none_round(cand.coverage_upstream for cand in self.candidates if cand.coverage_upstream is not None),
+                        coverage_start=util.mean_or_none_round(cand.coverage_start for cand in self.candidates if cand.coverage_start is not None),
+                        coverage_center=util.mean_or_none_round(cand.coverage_center for cand in self.candidates if cand.coverage_center is not None),
+                        coverage_end=util.mean_or_none_round(cand.coverage_end for cand in self.candidates if cand.coverage_end is not None),
+                        coverage_downstream=util.mean_or_none_round(cand.coverage_downstream for cand in self.candidates if cand.coverage_downstream is not None))
+
+        svcall.set_info("STDEV_POS", util.stdev(cand.pos for cand in self.candidates))
+        svcall.set_info("STDEV_LEN", util.stdev(cand.svlen for cand in self.candidates))
+
+        if abs(svcall.svlen) < config.minsvlen_screen:
+            return None
+
+        task.sv_id += 1
+
+        return svcall
+
+
+def calculate_bounds(svtype, ref_start_mode, svlen_mode):
+    if svtype == "INS":
+        svstart = ref_start_mode
+        svend = ref_start_mode
+    elif svtype == "DEL":
+        svstart = ref_start_mode + svlen_mode
+        svend = ref_start_mode
     else:
-        svstart=ref_start_mode
-        svend=svstart+abs(svlen_mode)
-    return svstart,svend
-
-def call_from(cluster,config,keep_qc_fails,task):
-    leads=cluster.leads
-
-    svtype=cluster.svtype
-    stdev_pos,stdev_len=None,None
-    qc=True
+        svstart = ref_start_mode
+        svend = svstart + abs(svlen_mode)
+    return svstart, svend
 
-    svlen=util.center(v.svlen for v in leads)
+
+def call_from(cluster, config, keep_qc_fails, task):
+    leads = cluster.leads
+
+    svtype = cluster.svtype
+    stdev_pos, stdev_len = None, None
+    qc = True
+
+    svlen = util.center(v.svlen for v in leads)
 
     if abs(svlen) < config.minsvlen_screen:
         return
 
-    #Count inline events only once per read, but split events as individual alignments, as in coverage calculation
-    #inline_qnames=set(k.read_qname for k in leads if k.source=="INLINE")
-    #support=len(inline_qnames)+sum(1 for k in leads if k.source!="INLINE")
-    if svtype=="INS" and svlen>=config.long_ins_length:
-        support_long_set=set(lead.read_qname for lead in cluster.leads_long)
-        support=len(set(k.read_qname for k in leads) | support_long_set)
-        support_long=len(support_long_set)
+    # Count inline events only once per read, but split events as individual alignments, as in coverage calculation
+    # inline_qnames=set(k.read_qname for k in leads if k.source=="INLINE")
+    # support=len(inline_qnames)+sum(1 for k in leads if k.source!="INLINE")
+    if svtype == "INS" and svlen >= config.long_ins_length:
+        support_long_set = set(lead.read_qname for lead in cluster.leads_long)
+        support = len(set(k.read_qname for k in leads) | support_long_set)
+        support_long = len(support_long_set)
     else:
-        support=len(set(k.read_qname for k in leads))
-        support_long=0
-    ref_start=util.center(v.ref_start for v in leads)
-    stdev_pos=util.stdev(util.trim((v.ref_start for v in leads)))
-    if svtype!="BND":
-        stdev_len=util.stdev(util.trim((v.svlen for v in leads)))
-        precise=(stdev_pos+stdev_len < config.precise)
+        support = len(set(k.read_qname for k in leads))
+        support_long = 0
+    ref_start = util.center(v.ref_start for v in leads)
+    stdev_pos = util.stdev(util.trim((v.ref_start for v in leads)))
+    if svtype != "BND":
+        stdev_len = util.stdev(util.trim((v.svlen for v in leads)))
+        precise = (stdev_pos + stdev_len < config.precise)
     else:
-        precise=(stdev_pos < config.precise)
-    svstart,svend=calculate_bounds(svtype,ref_start,svlen)
-    qual=int(util.mean(v.mapq for v in leads))
+        precise = (stdev_pos < config.precise)
+    svstart, svend = calculate_bounds(svtype, ref_start, svlen)
+    qual = int(util.mean(v.mapq for v in leads))
 
-    support_fwd=sum(lead.strand == "+" for lead in leads)
-    support_rev=len(leads) - support_fwd
+    support_fwd = sum(lead.strand == "+" for lead in leads)
+    support_rev = len(leads) - support_fwd
 
-    filter="PASS"
+    filter = "PASS"
 
     if config.qc_nm_measure:
-        nm_mean=util.mean(v.nm for v in leads)
+        nm_mean = util.mean(v.nm for v in leads)
     else:
-        nm_mean=-1
+        nm_mean = -1
 
     if not keep_qc_fails and not qc:
         return
 
-    svpi=SVCallPostprocessingInfo(cluster=cluster)
+    svpi = SVCallPostprocessingInfo(cluster=cluster)
 
-    if config.output_rnames or config.snf!=None:
-        rnames=list(set(k.read_qname for k in leads))
+    if config.output_rnames or config.snf is not None:
+        rnames = list(set(k.read_qname for k in leads))
     else:
-        rnames=None
+        rnames = None
 
-    svcall=SVCall(contig=cluster.contig,
-                  pos=svstart,
-                  id=f"{svtype}.{task.sv_id:X}S{task.id:X}",
-                  ref="N",
-                  alt=f"<{svtype}>",
-                  qual=qual,
-                  filter=filter,
-                  info=dict(),
-                  svtype=svtype,
-                  svlen=svlen,
-                  end=svend,
-                  genotypes=dict(),
-                  precise=precise,
-                  support=support,
-                  rnames=rnames,
-                  postprocess=svpi,
-                  qc=qc,
-                  nm=nm_mean,
-                  fwd=support_fwd,
-                  rev=support_rev)
-
-    if svtype=="BND":
-        resolve_bnd(svcall,cluster,config)
-    elif svtype=="INS":
-        svcall.set_info("SUPPORT_LONG",support_long)
-
-    if stdev_pos!=None:
-        svcall.set_info("STDEV_POS",stdev_pos)
-    if stdev_len!=None:
-        svcall.set_info("STDEV_LEN",stdev_len)
+    svcall = SVCall(contig=cluster.contig,
+                    pos=svstart,
+                    id=f"{svtype}.{task.sv_id:X}S{task.id:X}",
+                    ref="N",
+                    alt=f"<{svtype}>",
+                    qual=qual,
+                    filter=filter,
+                    info=dict(),
+                    svtype=svtype,
+                    svlen=svlen,
+                    end=svend,
+                    genotypes=dict(),
+                    precise=precise,
+                    support=support,
+                    rnames=rnames,
+                    postprocess=svpi,
+                    qc=qc,
+                    nm=nm_mean,
+                    fwd=support_fwd,
+                    rev=support_rev)
+
+    if svtype == "BND":
+        resolve_bnd(svcall, cluster, config)
+    elif svtype == "INS":
+        svcall.set_info("SUPPORT_LONG", support_long)
+
+    if stdev_pos is not None:
+        svcall.set_info("STDEV_POS", stdev_pos)
+    if stdev_len is not None:
+        svcall.set_info("STDEV_LEN", stdev_len)
 
-    #svcall.set_info("CLUSTER_ID",cluster.id)
+    # svcall.set_info("CLUSTER_ID",cluster.id)
 
-    task.sv_id+=1
+    task.sv_id += 1
 
     yield svcall
 
-def merge_inner_bounds(leads,config):
-    svlength_binsize=25
-    read_svlengths={}
-    read_starts={}
+
+def merge_inner_bounds(leads, config):
+    svlength_binsize = 25
+    read_svlengths = {}
+    read_starts = {}
     for ld in leads:
         if not ld.read_id in read_svlengths:
-            read_svlengths[ld.read_id]=0
-            read_starts[ld.read_id]=ld.ref_start
-        read_svlengths[ld.read_id]+=ld.svlen
-        read_starts[ld.read_id]=min(ld.ref_start,read_starts[ld.read_id])
-    svlen=util.center(v for k,v in read_svlengths.items())
-    pos=util.center(v for k,v in read_starts.items())
+            read_svlengths[ld.read_id] = 0
+            read_starts[ld.read_id] = ld.ref_start
+        read_svlengths[ld.read_id] += ld.svlen
+        read_starts[ld.read_id] = min(ld.ref_start, read_starts[ld.read_id])
+    svlen = util.center(v for k, v in read_svlengths.items())
+    pos = util.center(v for k, v in read_starts.items())
 
-    svlengths_reads={}
+    svlengths_reads = {}
     for read_id, length in read_svlengths.items():
-        bin=int(length/svlength_binsize)*svlength_binsize
+        bin = int(length / svlength_binsize) * svlength_binsize
         if not bin in svlengths_reads:
-            svlengths_reads[bin]=[(read_id,length)]
+            svlengths_reads[bin] = [(read_id, length)]
         else:
-            svlengths_reads[bin].append((read_id,length))
+            svlengths_reads[bin].append((read_id, length))
 
-    return pos,svlen,util.stdev(util.trim((v for k,v in read_starts.items()))),util.stdev(util.trim((v for k,v in read_svlengths.items())))
+    return pos, svlen, util.stdev(util.trim((v for k, v in read_starts.items()))), util.stdev(util.trim((v for k, v in read_svlengths.items())))
 
-def resolve_bnd(svcall,cluster,config):
-    mate_contig=util.most_common_top([lead.bnd_info.mate_contig for lead in cluster.leads])
-    selected=[lead for lead in cluster.leads if lead.bnd_info.mate_contig==mate_contig]
-    mate_ref_start=util.center([lead.bnd_info.mate_ref_start for lead in selected])
-    is_first=util.most_common_top([lead.bnd_info.is_first for lead in selected])
-    is_reverse=util.most_common_top([lead.bnd_info.is_reverse for lead in selected])
-    svcall.alt=(("N" if is_first else "") +
-                ("]" if is_reverse else "[" ) +
-                f"{mate_contig}:{mate_ref_start}" +
-                ("]" if is_reverse else "[" ) +
-                ("N" if not is_first else ""))
-    svcall.support=len(set(k.read_qname for k in selected))
-    cluster.leads=selected
-    svcall.bnd_info=SVCallBNDInfo(mate_contig=mate_contig, mate_ref_start=mate_ref_start, is_first=is_first, is_reverse=is_reverse)
-    svcall.set_info("CHR2",mate_contig)
-
-def call_groups(svgroups,config,task):
-    for group in svgroups:
-        svcall=call_group(group,config,task)
-        if svcall!=None:
-            yield svcall
 
-def call_group(svgroup,config,task):
-    """For combining grouped SV calls from multiple .snf samples into one SV call"""
-    first_cand=svgroup.candidates[0]
-
-    #Filtering
-    samples_count=float(len(config.snf_input_info))
-    sample_internal_ids=set(sample["internal_id"] for sample in config.snf_input_info)
-    total_count=len(svgroup.included_samples)
-    pass_count=sum(cand.qc==True for cand in svgroup.candidates)
-    qc=(pass_count > 0 and pass_count/samples_count >= config.combine_high_confidence) or (total_count/samples_count >= config.combine_low_confidence and total_count >= config.combine_low_confidence_abs)
+def resolve_bnd(svcall, cluster, config):
+    mate_contig = util.most_common_top([lead.bnd_info.mate_contig for lead in cluster.leads])
+    selected = [lead for lead in cluster.leads if lead.bnd_info.mate_contig == mate_contig]
+    mate_ref_start = util.center([lead.bnd_info.mate_ref_start for lead in selected])
+    is_first = util.most_common_top([lead.bnd_info.is_first for lead in selected])
+    is_reverse = util.most_common_top([lead.bnd_info.is_reverse for lead in selected])
+    svcall.alt = (("N" if is_first else "") +
+                  ("]" if is_reverse else "[") +
+                  f"{mate_contig}:{mate_ref_start}" +
+                  ("]" if is_reverse else "[") +
+                  ("N" if not is_first else ""))
+    svcall.support = len(set(k.read_qname for k in selected))
+    cluster.leads = selected
+    svcall.bnd_info = SVCallBNDInfo(mate_contig=mate_contig, mate_ref_start=mate_ref_start, is_first=is_first, is_reverse=is_reverse)
+    svcall.set_info("CHR2", mate_contig)
 
-    if not qc:
-        return None
 
-    if (not config.combine_output_filtered) and not any(cand.qc and cand.filter=="PASS" for cand in svgroup.candidates):
-        return None
-
-    if config.output_rnames:
-        rnames=[]
-    else:
-        rnames=None
-
-    genotypes={}
-    genotyped_count=0
-    for cand in svgroup.candidates:
-        if config.output_rnames and cand.rnames!=None:
-            rnames.extend(cand.rnames)
-        if not 0 in cand.genotypes:
-            cand.genotypes[0]=(".",".",0,0,cand.support,None)
-        if cand.sample_internal_id in genotypes:
-            #Intra-sample merging
-            a,b,gt_qual,dr,dv,ps=cand.genotypes[0]
-            curr_a,curr_b,curr_gt_qual,curr_dr,curr_dv,curr_ps,curr_id=genotypes[cand.sample_internal_id]
-            new_id=curr_id+","+config.id_prefix+cand.id
-            if (curr_a==".") or (a != "." and (a,b) >= (curr_a,curr_b)):
-                genotypes[cand.sample_internal_id]=(a,b,gt_qual,dr,dv,ps,new_id)
-            else:
-                genotypes[cand.sample_internal_id]=(curr_a,curr_b,curr_gt_qual,curr_dr,curr_dv,curr_ps,new_id)
-        else:
-            a,b,gt_qual,dr,dv,ps=cand.genotypes[0]
-            genotypes[cand.sample_internal_id]=(a,b,gt_qual,dr,dv,ps,config.id_prefix+cand.id)
-        genotyped_count+=1
-
-    for sample_internal_id in sample_internal_ids:
-        if sample_internal_id in genotypes:
-            continue
-        coverage=svgroup.coverages_nonincluded[sample_internal_id]
-        if coverage >= config.combine_null_min_coverage:
-            genotypes[sample_internal_id]=(0,0,0,coverage,0,None,"NULL")
-        else:
-            genotypes[sample_internal_id]=(".",".",0,coverage,0,None,"NULL")
-
-    if config.combine_consensus:
-        genotypes_consensus={}
-        for a,b,gt_qual,dr,dv in genotypes.values():
-            if not (a,b) in genotypes_consensus:
-                genotypes_consensus[(a,b)]={"count":0,"qual":list(),"dr":list(),"dv":list()}
-            genotypes_consensus[(a,b)]["count"]+=1
-            genotypes_consensus[(a,b)]["qual"].append(gt_qual)
-            genotypes_consensus[(a,b)]["dr"].append(dr)
-            genotypes_consensus[(a,b)]["dv"].append(dv)
-        most_common_count=genotypes_consensus[sorted(genotypes_consensus,key=lambda k: genotypes_consensus[k]["count"],reverse=True)[0]]["count"]
-        most_common_gt=[gt for gt in genotypes_consensus if genotypes_consensus[gt]["count"]==most_common_count]
-        cons_a,cons_b=max(most_common_gt)
-        consensus_info=genotypes_consensus[(cons_a,cons_b)]
-        genotypes={0:(cons_a,cons_b,int(sum(consensus_info["qual"])/consensus_info["count"]),sum(consensus_info["dr"]),sum(consensus_info["dv"]))}
-        if cons_a!=1 and cons_b!=1:
-            return None
-
-    if config.combine_pair_relabel:
-        max_gt=(0,0)
-        for sample_id in genotypes:
-            a,b,qual,dr,dv,ps,new_id=genotypes[sample_id]
-            if qual > config.combine_pair_relabel_threshold and a!=".":
-                max_gt=max(max_gt,(a,b))
+def call_groups(svgroups: list[SVGroup], config, task):
+    for group in svgroups:
+        svcall = group.call(config, task)
+        if svcall is not None:
+            yield svcall
 
-        if max_gt!=(0,0):
-            for sample_id in genotypes:
-                a,b,qual,dr,dv,ps,new_id=genotypes[sample_id]
-                if qual < config.combine_pair_relabel_threshold and a!=".":
-                    max_a,max_b=max_gt
-                    genotypes[sample_id]=(max_a,max_b,qual,dr,dv,ps,new_id)
-
-    svcall_pos=int(util.median(cand.pos for cand in svgroup.candidates))
-    svcall_svlen=int(util.median(cand.svlen for cand in svgroup.candidates))
-    svcall_alt=first_cand.alt
-    svcall_alt_mindist=abs(len(svcall_alt)-svcall_svlen)
-    if first_cand.svtype=="INS":
-        svcall_end=svcall_pos
-        for cand in svgroup.candidates:
-            dist=abs(len(cand.alt)-svcall_svlen)
-            if dist < svcall_alt_mindist:
-                svcall_alt_mindist=dist
-                svcall_alt=cand.alt
-    else:
-        svcall_end=svcall_pos+abs(svcall_svlen)
 
-    svcall=SVCall(contig=first_cand.contig,
-                  pos=svcall_pos,
-                  id=f"{first_cand.svtype}.{task.sv_id:X}M{task.id:X}",
-                  ref="N",
-                  alt=svcall_alt,
-                  qual=round(util.mean(int(cand.qual) for cand in svgroup.candidates)),
-                  filter="PASS",
-                  info=dict(),
-                  svtype=first_cand.svtype,
-                  svlen=svcall_svlen,
-                  end=svcall_end,
-                  genotypes=genotypes,
-                  precise=sum(int(cand.precise) for cand in svgroup.candidates)/float(len(svgroup.candidates)) > 0.5,
-                  support=round(util.mean(cand.support for cand in svgroup.candidates)),
-                  rnames=rnames,
-                  postprocess=None,
-                  qc=True,
-                  nm=-1,
-                  fwd=sum(cand.fwd for cand in svgroup.candidates),
-                  rev=sum(cand.rev for cand in svgroup.candidates),
-                  coverage_upstream=util.mean_or_none_round(cand.coverage_upstream for cand in svgroup.candidates if cand.coverage_upstream!=None),
-                  coverage_start=util.mean_or_none_round(cand.coverage_start for cand in svgroup.candidates if cand.coverage_start!=None),
-                  coverage_center=util.mean_or_none_round(cand.coverage_center for cand in svgroup.candidates if cand.coverage_center!=None),
-                  coverage_end=util.mean_or_none_round(cand.coverage_end for cand in svgroup.candidates if cand.coverage_end!=None),
-                  coverage_downstream=util.mean_or_none_round(cand.coverage_downstream for cand in svgroup.candidates if cand.coverage_downstream!=None) )
-
-    svcall.set_info("STDEV_POS",util.stdev(cand.pos for cand in svgroup.candidates))
-    svcall.set_info("STDEV_LEN",util.stdev(cand.svlen for cand in svgroup.candidates))
-
-    if abs(svcall.svlen) < config.minsvlen_screen:
-        return None
-
-    task.sv_id+=1
-
-    return svcall
-
-def classify_splits(read,leads,config,main_contig):
-    minsvlen_screen=config.minsvlen_screen
-    maxsvlen_other=minsvlen_screen*config.dev_split_max_query_distance_mult
-    min_split_len_bnd=config.bnd_min_split_length
+def classify_splits(read, leads, config, main_contig):
+    minsvlen_screen = config.minsvlen_screen
+    maxsvlen_other = minsvlen_screen * config.dev_split_max_query_distance_mult
+    min_split_len_bnd = config.bnd_min_split_length
 
     leads.sort(key=lambda ld: ld.qry_start)
-    last=leads[0]
-    last.svtypes_starts_lens=[]
+    last = leads[0]
+    last.svtypes_starts_lens = []
 
-    if last.qry_start >= config.long_ins_length*0.5:
-        last.svtypes_starts_lens.append(("INS",last.ref_start,None))
+    if last.qry_start >= config.long_ins_length * 0.5:
+        last.svtypes_starts_lens.append(("INS", last.ref_start, None))
 
-    for i in range(1,len(leads)):
-        curr=leads[i]
-        curr.svtypes_starts_lens=[]
-        qry_dist_abs=abs(curr.qry_start - last.qry_end)
+    for i in range(1, len(leads)):
+        curr = leads[i]
+        curr.svtypes_starts_lens = []
+        qry_dist_abs = abs(curr.qry_start - last.qry_end)
 
         if curr.contig == last.contig:
-            rev=(curr.strand == "-")
-            fwd=not rev
+            rev = (curr.strand == "-")
+            fwd = not rev
             if curr.strand == last.strand:
                 #
-                #INS, DEL, DUP
+                # INS, DEL, DUP
                 #
                 if (fwd and (curr.qry_start - last.qry_end) >= minsvlen_screen
-                    and (curr.ref_start - last.ref_end) < maxsvlen_other
-                    and (curr.qry_start - last.qry_end) - (curr.ref_start - last.ref_end) >= minsvlen_screen):
-                    #INS, FWD
-                    svstart=curr.ref_start
-                    svlen=(curr.qry_start - last.qry_end)
+                        and (curr.ref_start - last.ref_end) < maxsvlen_other
+                        and (curr.qry_start - last.qry_end) - (curr.ref_start - last.ref_end) >= minsvlen_screen):
+                    # INS, FWD
+                    svstart = curr.ref_start
+                    svlen = (curr.qry_start - last.qry_end)
                     if svlen <= config.dev_seq_cache_maxlen:
-                        curr.seq=read.query_sequence[last.qry_end:curr.qry_start]
+                        curr.seq = read.query_sequence[last.qry_end:curr.qry_start]
                     else:
-                        curr.seq=None
-                    curr.svtypes_starts_lens.append(("INS",svstart,svlen))
+                        curr.seq = None
+                    curr.svtypes_starts_lens.append(("INS", svstart, svlen))
 
                 elif (rev and (curr.qry_start - last.qry_end) >= minsvlen_screen
                       and (last.ref_start - curr.ref_end) < maxsvlen_other
                       and (curr.qry_start - last.qry_end) - (last.ref_start - curr.ref_end) >= minsvlen_screen):
-                    #INS, REV
-                    svstart=last.ref_start
-                    svlen=(curr.qry_start - last.qry_end)
+                    # INS, REV
+                    svstart = last.ref_start
+                    svlen = (curr.qry_start - last.qry_end)
                     if svlen <= config.dev_seq_cache_maxlen:
-                        curr.seq=read.query_sequence[last.qry_end:curr.qry_start]
+                        curr.seq = read.query_sequence[last.qry_end:curr.qry_start]
                     else:
-                        curr.seq=None
-                    curr.svtypes_starts_lens.append(("INS",svstart,svlen))
+                        curr.seq = None
+                    curr.svtypes_starts_lens.append(("INS", svstart, svlen))
 
                 elif (fwd and (curr.ref_start - last.ref_end) >= minsvlen_screen
                       and qry_dist_abs < maxsvlen_other
                       and (curr.ref_start - last.ref_end) - (curr.qry_start - last.qry_end) >= minsvlen_screen):
-                        #DEL, FWD
-                        svstart=curr.ref_start
-                        svlen=(curr.ref_start - last.ref_end)
-                        curr.svtypes_starts_lens.append(("DEL",svstart,-svlen))
+                    # DEL, FWD
+                    svstart = curr.ref_start
+                    svlen = (curr.ref_start - last.ref_end)
+                    curr.svtypes_starts_lens.append(("DEL", svstart, -svlen))
 
                 elif (rev and (last.ref_start - curr.ref_end) >= minsvlen_screen
                       and qry_dist_abs < maxsvlen_other
                       and (last.ref_start - curr.ref_end) - (curr.qry_start - last.qry_end) >= minsvlen_screen):
-                        #DEL, REV
-                        svstart=last.ref_start
-                        svlen=(last.ref_start - curr.ref_end)
-                        curr.svtypes_starts_lens.append(("DEL",svstart,-svlen))
+                    # DEL, REV
+                    svstart = last.ref_start
+                    svlen = (last.ref_start - curr.ref_end)
+                    curr.svtypes_starts_lens.append(("DEL", svstart, -svlen))
 
                 elif fwd and curr.ref_start <= last.ref_end:
                     if qry_dist_abs < maxsvlen_other:
-                        #DUP, FWD
-                        svstart=curr.ref_start
-                        svlen=(last.ref_end - curr.ref_start)
+                        # DUP, FWD
+                        svstart = curr.ref_start
+                        svlen = (last.ref_end - curr.ref_start)
                         if svlen >= minsvlen_screen:
-                            curr.svtypes_starts_lens.append(("DUP",svstart,svlen))
+                            curr.svtypes_starts_lens.append(("DUP", svstart, svlen))
 
                 elif rev and last.ref_start <= curr.ref_end:
                     if qry_dist_abs < maxsvlen_other:
-                        #DUP, REV
-                        svstart=last.ref_start
-                        svlen=(curr.ref_end - last.ref_start)
+                        # DUP, REV
+                        svstart = last.ref_start
+                        svlen = (curr.ref_end - last.ref_start)
                         if svlen >= minsvlen_screen:
-                            curr.svtypes_starts_lens.append(("DUP",svstart,svlen))
+                            curr.svtypes_starts_lens.append(("DUP", svstart, svlen))
 
             elif qry_dist_abs < maxsvlen_other:
                 #
-                #INV
+                # INV
                 #
                 if fwd and curr.ref_start <= last.ref_start:
-                    #CASE B
-                    svstart=curr.ref_start
-                    svlen=last.ref_start-curr.ref_start
+                    # CASE B
+                    svstart = curr.ref_start
+                    svlen = last.ref_start - curr.ref_start
                     if svlen >= minsvlen_screen:
-                        curr.svtypes_starts_lens.append(("INV",svstart,svlen))
+                        curr.svtypes_starts_lens.append(("INV", svstart, svlen))
 
                 elif fwd and curr.ref_start > last.ref_start:
-                    #CASE C
-                    svstart=last.ref_start
-                    svlen=curr.ref_start-last.ref_start
+                    # CASE C
+                    svstart = last.ref_start
+                    svlen = curr.ref_start - last.ref_start
                     if svlen >= minsvlen_screen:
-                        curr.svtypes_starts_lens.append(("INV",svstart,svlen))
+                        curr.svtypes_starts_lens.append(("INV", svstart, svlen))
 
                 elif rev and curr.ref_end >= last.ref_end:
-                    #CASE A
-                    svstart=last.ref_end
-                    svlen=curr.ref_end-last.ref_end
+                    # CASE A
+                    svstart = last.ref_end
+                    svlen = curr.ref_end - last.ref_end
                     if svlen >= minsvlen_screen:
-                        curr.svtypes_starts_lens.append(("INV",svstart,svlen))
+                        curr.svtypes_starts_lens.append(("INV", svstart, svlen))
 
                 elif rev and curr.ref_end < last.ref_end:
-                    #CASE D
-                    svstart=curr.ref_end
-                    svlen=last.ref_end-curr.ref_end
+                    # CASE D
+                    svstart = curr.ref_end
+                    svlen = last.ref_end - curr.ref_end
                     if svlen >= minsvlen_screen:
-                        curr.svtypes_starts_lens.append(("INV",svstart,svlen))
+                        curr.svtypes_starts_lens.append(("INV", svstart, svlen))
 
         elif qry_dist_abs < maxsvlen_other:
             #
-            #BND
+            # BND
             #
             if curr.contig == main_contig:
-                a,b=curr,last
+                a, b = curr, last
             else:
-                a,b=last,curr
+                a, b = last, curr
 
-            if a.contig == main_contig and abs(last.qry_end-last.qry_start) >= min_split_len_bnd and abs(curr.qry_end-curr.qry_start) >= min_split_len_bnd:
-                is_first=a.qry_start < b.qry_start
+            if a.contig == main_contig and abs(last.qry_end - last.qry_start) >= min_split_len_bnd and abs(curr.qry_end - curr.qry_start) >= min_split_len_bnd:
+                is_first = a.qry_start < b.qry_start
                 if is_first:
-                    if a.strand=="+":
-                        svstart=a.ref_end
+                    if a.strand == "+":
+                        svstart = a.ref_end
                     else:
-                        svstart=a.ref_start
+                        svstart = a.ref_start
                 else:
-                    if a.strand=="+":
-                        svstart=a.ref_start
+                    if a.strand == "+":
+                        svstart = a.ref_start
                     else:
-                        svstart=a.ref_end
+                        svstart = a.ref_end
                 a.svtypes_starts_lens.append(("BND",
-                                            svstart,
-                                            SVCallBNDInfo(b.contig,
-                                                          b.ref_start,
-                                                          is_first,
-                                                          a.strand!=b.strand)))
-        last=curr
+                                              svstart,
+                                              SVCallBNDInfo(b.contig,
+                                                            b.ref_start,
+                                                            is_first,
+                                                            a.strand != b.strand)))
+        last = curr
```

### Comparing `sniffles-2.2/src/sniffles/util.py` & `sniffles-2.3/src/sniffles/util.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,128 +1,145 @@
 #!/usr/bin/env python3
 #
 # Sniffles2
 # A fast structural variant caller for long-read sequencing data
 #
-# Created: 27.08.2021
-# Author:  Moritz Smolka
-# Contact: moritz.g.smolka@gmail.com
+# Created:     27.08.2021
+# Author:      Moritz Smolka
+# Maintainer:  Hermann Romanek
+# Contact:     sniffles@romanek.at
 #
 
 import statistics
-import math
 import sys
 import time
 
+
 class Sniffles2Exit(Exception):
     pass
 
+
 def stdev(nums):
-    nums=list(nums)
+    nums = list(nums)
     return statistics.stdev(nums) if len(nums) > 1 else 0
 
+
 def median(nums):
     return int(statistics.median(nums))
 
+
 def median_or_mode(nums):
-    nums=list(nums)
-    top=most_common(nums)
-    if len(top)>1 and (top[0][0]-top[1][0]<2):
+    nums = list(nums)
+    top = most_common(nums)
+    if len(top) > 1 and (top[0][0] - top[1][0] < 2):
         return median_noavg(nums)
     else:
         return median_modes(nums)
 
+
 def median_noavg(nums):
-    nums=sorted(list(nums))
-    mid=int(len(nums)/2)
+    nums = sorted(list(nums))
+    mid = int(len(nums) / 2)
     return nums[mid]
 
+
 def median_modes(nums):
-    max_count=0
-    counts={}
+    max_count = 0
+    counts = {}
     for n in nums:
-        if not n in counts:
-            counts[n]=1
+        if n not in counts:
+            counts[n] = 1
         else:
-            counts[n]+=1
-        max_count=max(max_count,counts[n])
-    return median_noavg(k for k,n in counts.items() if max_count-n<3 )
+            counts[n] += 1
+        max_count = max(max_count, counts[n])
+    return median_noavg(k for k, n in counts.items() if max_count - n < 3)
+
 
 def mean(nums):
-    nums=list(nums)
-    return sum(nums)/len(nums)
+    nums = list(nums)
+    return sum(nums) / len(nums)
+
 
 def mean_or_none(nums):
-    nums=list(nums)
-    if len(nums)==0:
+    nums = list(nums)
+    if len(nums) == 0:
         return None
     else:
-        return sum(nums)/len(nums)
+        return sum(nums) / len(nums)
+
 
 def mean_or_none_round(nums):
-    r=mean_or_none(nums)
-    if r==None:
+    r = mean_or_none(nums)
+    if r is None:
         return r
     else:
         return round(r)
 
-def trim(nums,pct=25):
-    nums=sorted(list(nums))
-    trim_n=int(len(nums)/float(100.0)*pct)
+
+def trim(nums, pct=25):
+    nums = sorted(list(nums))
+    trim_n = int(len(nums) / float(100.0) * pct)
     if trim_n > 0:
         return nums[trim_n:-trim_n]
     else:
         return nums
 
+
 def most_common(nums):
-    counts={}
+    counts = {}
     for n in nums:
-        if not n in counts:
-            counts[n]=1
+        if n not in counts:
+            counts[n] = 1
         else:
-            counts[n]+=1
-    return sorted(((counts[n],n) for n in counts), reverse=True)
+            counts[n] += 1
+    return sorted(((counts[n], n) for n in counts), reverse=True)
+
 
 def most_common_top(nums):
-    result=most_common(nums)
-    return sorted(item for count,item in result if count==result[0][0])[0]
+    result = most_common(nums)
+    return sorted(item for count, item in result if count == result[0][0])[0]
+
 
 def error(msg):
-    sys.stderr.write("Sniffles2 Error: "+msg+"\n")
+    sys.stderr.write("Sniffles2 Error: " + msg + "\n")
     sys.stderr.flush()
 
+
 def fatal_error(msg):
-    error(msg+" (Fatal error, exiting.)")
+    error(msg + " (Fatal error, exiting.)")
     exit(1)
 
+
 def fatal_error_main(msg):
-    error(msg+" (Fatal error, exiting.)")
+    error(msg + " (Fatal error, exiting.)")
     raise Sniffles2Exit
 
-def load_tandem_repeats(filename,padding):
-    contigs_tr={}
-    unsorted=False
-    with open(filename,"r") as handle:
+
+def load_tandem_repeats(filename, padding):
+    contigs_tr = {}
+    unsorted = False
+    with open(filename, "r") as handle:
         for line in handle:
-            parts=line.split("\t")
+            parts = line.split("\t")
             if len(parts) >= 3:
-                contig,start,end=parts[:3]
-                start=int(start)
-                end=int(end)
-                if not contig in contigs_tr:
-                    contigs_tr[contig]=[]
-                if len(contigs_tr[contig])>0:
-                    last_start,last_end=contigs_tr[contig][-1]
+                contig, start, end = parts[:3]
+                start = int(start)
+                end = int(end)
+                if contig not in contigs_tr:
+                    contigs_tr[contig] = []
+                if len(contigs_tr[contig]) > 0:
+                    last_start, last_end = contigs_tr[contig][-1]
                     if start < last_start:
-                        unsorted=True
-                contigs_tr[contig].append((max(0,int(start)-padding),int(end)+padding))
+                        unsorted = True
+                contigs_tr[contig].append((max(0, int(start) - padding), int(end) + padding))
 
     if unsorted:
         print("Info: The tandem repeat annotations file was not sorted. Sorting it in-memory after loading... (please sort the .bed file once before to save time when running multiple samples)")
-        sort_start=time.time()
+        sort_start = time.time()
         for contig in contigs_tr:
             contigs_tr[contig].sort()
-        print(f"Info: Optional sorting of input tandem repeat annotations took {time.time()-sort_start:.2f}s.")
+        print(f"Info: Optional sorting of input tandem repeat annotations took {time.time() - sort_start:.2f}s.")
 
     return contigs_tr
 
-center=median_modes
+
+center = median_modes
```

### Comparing `sniffles-2.2/src/sniffles/vcf.py` & `sniffles-2.3/src/sniffles/vcf.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,84 +1,93 @@
 #!/usr/bin/env python3
 #
 # Sniffles2
 # A fast structural variant caller for long-read sequencing data
 #
-# Created: 15.08.2021
-# Author:  Moritz Smolka
-# Contact: moritz.g.smolka@gmail.com
+# Created:     15.08.2021
+# Author:      Moritz Smolka
+# Maintainer:  Hermann Romanek
+# Contact:     sniffles@romanek.at
 #
+import logging
 
 import pysam
 import os
 
 from sniffles import sv
 from sniffles import util
 
-def format_info(k,v):
-    if isinstance(v,float):
+
+log = logging.getLogger(__name__)
+
+
+def format_info(k, v):
+    if isinstance(v, float):
         return f"{k}={v:.3f}"
-    elif isinstance(v,list):
+    elif isinstance(v, list):
         return f"{k}={','.join(v)}"
     else:
         return f"{k}={v}"
 
+
 def format_genotype(gt):
-    if len(gt)==6:
-        a,b,qual,dr,dv,ps=gt
-        if ps!=None and (a,b)==(0,1):
-            gt_sep="|"
-            if ps==1:
-                a,b=b,a
+    if len(gt) == 6:
+        a, b, qual, dr, dv, ps = gt
+        if ps is not None and (a, b) == (0, 1):
+            gt_sep = "|"
+            if ps == 1:
+                a, b = b, a
         else:
-            gt_sep="/"
+            gt_sep = "/"
         return f"{a}{gt_sep}{b}:{qual}:{dr}:{dv}"
     else:
-        a,b,qual,dr,dv,ps,id=gt
-        if ps!=None and (a,b)==(0,1):
-            gt_sep="|"
-            if ps==1:
-                a,b=b,a
+        a, b, qual, dr, dv, ps, id = gt
+        if ps is not None and (a, b) == (0, 1):
+            gt_sep = "|"
+            if ps == 1:
+                a, b = b, a
         else:
-            gt_sep="/"
+            gt_sep = "/"
         return f"{a}{gt_sep}{b}:{qual}:{dr}:{dv}:{id}"
 
+
 class VCF:
-    def __init__(self,config,handle):
-        self.config=config
-        self.handle=handle
-        self.call_count=0
-        self.info_order=["SVTYPE","SVLEN","END","SUPPORT","RNAMES","COVERAGE","STRAND"]
+    def __init__(self, config, handle):
+        self.config = config
+        self.handle = handle
+        self.call_count = 0
+        self.info_order = ["SVTYPE", "SVLEN", "END", "SUPPORT", "RNAMES", "COVERAGE", "STRAND"]
         if config.qc_nm_measure:
             self.info_order.append("NM")
 
-        self.default_genotype=config.genotype_none
+        self.default_genotype = config.genotype_none
 
-        if config.mode=="combine":
-            self.genotype_format=config.genotype_format+":ID"
-            self.default_genotype+=tuple(["NULL"])
+        if config.mode == "combine":
+            self.genotype_format = config.genotype_format + ":ID"
+            self.default_genotype += tuple(["NULL"])
         else:
-            self.genotype_format=config.genotype_format
+            self.genotype_format = config.genotype_format
 
-        self.reference_handle=None
+        self.reference_handle = None
 
     def open_reference(self):
-        if self.config.reference == None:
+        if self.config.reference is None:
             return
-        if not os.path.exists(self.config.reference+".fai") and not os.path.exists(self.config.reference+".gzi"):
+
+        if not os.path.exists(self.config.reference + ".fai") and not os.path.exists(self.config.reference + ".gzi"):
             print(f"Info: Fasta index for {self.config.reference} not found. Generating with pysam.faidx (this may take a while)")
             pysam.faidx(self.config.reference)
-        self.reference_handle=pysam.FastaFile(self.config.reference)
+        self.reference_handle = pysam.FastaFile(self.config.reference)
 
-    def write_header(self,contigs_lengths):
+    def write_header(self, contigs_lengths):
         self.write_header_line("fileformat=VCFv4.2")
         self.write_header_line(f"source={self.config.version}_{self.config.build}")
-        self.write_header_line('command="'+self.config.command+'"')
-        self.write_header_line('fileDate="'+self.config.start_date+'"')
-        for contig,contig_len in contigs_lengths:
+        self.write_header_line('command="' + self.config.command + '"')
+        self.write_header_line('fileDate="' + self.config.start_date + '"')
+        for contig, contig_len in contigs_lengths:
             self.write_header_line(f"contig=<ID={contig},length={contig_len}>")
 
         self.write_header_line('ALT=<ID=INS,Description="Insertion">')
         self.write_header_line('ALT=<ID=DEL,Description="Deletion">')
         self.write_header_line('ALT=<ID=DUP,Description="Duplication">')
         self.write_header_line('ALT=<ID=INV,Description="Inversion">')
         self.write_header_line('ALT=<ID=BND,Description="Breakend; Translocation">')
@@ -119,205 +128,245 @@
         self.write_header_line('INFO=<ID=SUPP_VEC,Number=1,Type=String,Description="List of read support for all samples">')
         self.write_header_line('INFO=<ID=CONSENSUS_SUPPORT,Number=1,Type=Integer,Description="Number of reads that support the generated insertion (INS) consensus sequence">')
         self.write_header_line('INFO=<ID=RNAMES,Number=.,Type=String,Description="Names of supporting reads (if enabled with --output-rnames)">')
         self.write_header_line('INFO=<ID=AF,Number=1,Type=Float,Description="Allele Frequency">')
         self.write_header_line('INFO=<ID=NM,Number=.,Type=Float,Description="Mean number of query alignment length adjusted mismatches of supporting reads">')
         self.write_header_line('INFO=<ID=PHASE,Number=.,Type=String,Description="Phasing information derived from supporting reads, represented as list of: HAPLOTYPE,PHASESET,HAPLOTYPE_SUPPORT,PHASESET_SUPPORT,HAPLOTYPE_FILTER,PHASESET_FILTER">')
 
-        samples_header="\t".join(sample_id for internal_id,sample_id in self.config.sample_ids_vcf)
+        samples_header = "\t".join(sample_id for internal_id, sample_id in self.config.sample_ids_vcf)
         self.write_raw(f"#CHROM\tPOS\tID\tREF\tALT\tQUAL\tFILTER\tINFO\tFORMAT\t{samples_header}")
 
-    def write_raw(self,text,endl="\n"):
+    def write_raw(self, text, endl="\n"):
         if self.config.vcf_output_bgz:
             self.handle.write(text.encode())
             self.handle.write(endl.encode())
         else:
             self.handle.write(text)
             self.handle.write(endl)
 
-    def write_header_line(self,text):
-        self.write_raw("##"+text)
+    def write_header_line(self, text):
+        self.write_raw("##" + text)
 
-    def write_call(self,call):
-        #pysam coordinates are 0-based, VCF 1-based - therefore +1 is added to call.pos
-        end=call.end + 1
-        pos=call.pos + 1
-
-        #Determine genotypes columns
-        ac=0 #Allele count
-        supvec=[]
-        sample_genotypes=[]
+    def write_call(self, call):
+        # pysam coordinates are 0-based, VCF 1-based
+        # but VCF also requires the index of the base before the SV to be reported,
+        # so we are fine without offsetting
+        end = call.end
+        pos = call.pos if call.pos > 0 else 1
+
+        # Determine genotypes columns
+        ac = 0  # Allele count
+        supvec = []
+        sample_genotypes = []
         for internal_id, sample_id in self.config.sample_ids_vcf:
-            if internal_id in call.genotypes and call.genotypes[internal_id]!=None:
-                gt_curr=call.genotypes[internal_id]
+            if internal_id in call.genotypes and call.genotypes[internal_id] is not None:
+                gt_curr = call.genotypes[internal_id]
                 sample_genotypes.append(format_genotype(gt_curr))
-                if gt_curr[0]!="." and gt_curr[4]>0: #Not non-genotype and has supporting reads
-                    ac+=sum(call.genotypes[internal_id][:2])
-                    supp="1"
+                if gt_curr[0] != "." and gt_curr[4] > 0:  # Not non-genotype and has supporting reads
+                    ac += sum(call.genotypes[internal_id][:2])
+                    supp = "1"
                 else:
-                    supp="0"
+                    supp = "0"
             else:
                 sample_genotypes.append(format_genotype(self.default_genotype))
-                supp="0"
+                supp = "0"
             supvec.append(supp)
 
         if len(self.config.sample_ids_vcf) > 1:
-            call.set_info("AC",ac)
-            call.set_info("SUPP_VEC","".join(supvec))
-            if ac==0:
-                call.filter="GT"
-
-        #Output core SV attributes
-        infos={"SVTYPE": call.svtype,
-               "SVLEN": call.svlen,
-               "END": end,
-               "SUPPORT": call.support,
-               "RNAMES": call.rnames if self.config.output_rnames else None,
-               "COVERAGE": f"{call.coverage_upstream},{call.coverage_start},{call.coverage_center},{call.coverage_end},{call.coverage_downstream}",
-               "STRAND": ("+" if call.fwd>0 else "") + ("-" if call.rev>0 else ""),
-               "NM": call.nm}
-
-        if call.svtype=="BND":
-            infos["SVLEN"]=None
-            infos["END"]=None
-
-        infos_ordered=["PRECISE" if call.precise else "IMPRECISE"]
-        af=call.get_info("AF")
-        af=af if af!=None else 0
+            call.set_info("AC", ac)
+            call.set_info("SUPP_VEC", "".join(supvec))
+            if ac == 0:
+                call.filter = "GT"
+
+        # Output core SV attributes
+        infos = {
+            "SVTYPE": call.svtype,
+            "SVLEN": call.svlen,
+            "END": end,
+            "SUPPORT": call.support,
+            "RNAMES": call.rnames if self.config.output_rnames else None,
+            "COVERAGE": f"{call.coverage_upstream},{call.coverage_start},{call.coverage_center},{call.coverage_end},{call.coverage_downstream}",
+            "STRAND": ("+" if call.fwd > 0 else "") + ("-" if call.rev > 0 else ""),
+            "NM": call.nm
+        }
+
+        if call.svtype == "BND":
+            infos["SVLEN"] = None
+            infos["END"] = None
+
+        infos_ordered = ["PRECISE" if call.precise else "IMPRECISE"]
+        af = call.get_info("AF")
+        af = af if af is not None else 0
         sv_is_mosaic = af <= self.config.mosaic_af_max
         if sv_is_mosaic and self.config.mosaic:
             infos_ordered.append("MOSAIC")
-        infos_ordered.extend(format_info(k,infos[k]) for k in self.info_order if infos[k]!=None)
-        info_str=";".join(infos_ordered)
+        infos_ordered.extend(format_info(k, infos[k]) for k in self.info_order if infos[k] != None)
+        info_str = ";".join(infos_ordered)
 
-        #Output call specific additional information
+        # Output call specific additional information
         for k in sorted(call.info):
-            if call.info[k]==None:
+            if call.info[k] is None:
                 continue
-            info_str+=";" + format_info(k,call.info[k])
+            info_str += ";" + format_info(k, call.info[k])
 
-        #if call.id==None:
+        # if call.id==None:
         #    call.id=f"Sniffles2.{call.svtype}.{self.call_count+1:06}"
 
-        #Resolve DEL sequence
-        if not self.config.symbolic and call.svtype=="DEL" and self.reference_handle != None and abs(call.svlen) <= self.config.max_del_seq_len:
+        # Resolve DEL sequence
+        if not self.config.symbolic and call.svtype == "DEL" and self.reference_handle is not None and abs(call.svlen) <= self.config.max_del_seq_len:
             try:
-                call.ref=self.reference_handle.fetch(call.contig,call.pos,call.pos-call.svlen)
-                call.alt="N"
+                call.ref = self.reference_handle.fetch(call.contig, call.pos - 1, call.pos - call.svlen)  # VCF requires inclusion of the last reference base before the SV
+                call.alt = call.ref[0]
             except KeyError:
-                call.ref="N"
-                call.alt=f"<{call.svtype}>"
+                call.ref = "N"
+                call.alt = f"<{call.svtype}>"
             except ValueError:
-                call.ref="N"
-                call.alt=f"<{call.svtype}>"
+                call.ref = "N"
+                call.alt = f"<{call.svtype}>"
 
         if self.config.symbolic:
-            call.ref="N"
-            call.alt=f"<{call.svtype}>"
+            call.ref = "N"
+            call.alt = f"<{call.svtype}>"
+        else:
+            if self.reference_handle is not None and call.ref == 'N':
+                # Fetch the base before the SV
+                try:
+                    call.ref = self.reference_handle.fetch(call.contig, start := max(0, call.pos - 1), start + 1)
+                except (KeyError, ValueError):
+                    ...
+
+                if call.svtype == "INS":
+                    call.alt = call.ref + call.alt
+                elif call.svtype == 'BND':
+                    call.alt = (call.ref + call.alt[1:]) if call.alt.startswith('N') else call.alt[:-1] + call.ref
 
-        call.qual=max(0,min(60,call.qual))
+        call.qual = max(0, min(60, call.qual))
 
-        self.write_raw("\t".join(str(v) for v in [call.contig,pos,self.config.id_prefix+call.id,call.ref,call.alt,call.qual,call.filter,info_str,self.genotype_format]+sample_genotypes))
-        self.call_count+=1
+        self.write_raw("\t".join(str(v) for v in [call.contig, pos, self.config.id_prefix + call.id, call.ref, call.alt, call.qual, call.filter, info_str, self.genotype_format] + sample_genotypes))
+        self.call_count += 1
 
     def read_svs_iter(self):
-        self.header_str=""
-        line_index=0
+        self.header_str = ""
+        line_index = 0
         for line in self.handle:
             try:
-                if isinstance(line,bytes):
-                    line=line.decode("utf-8")
-                line_index+=1
-                line_strip=line.strip()
-                if line_strip=="" or line_strip[0]=="#":
-                    if line_strip[0]=="#":
-                        self.header_str+=line_strip+"\n"
+                if isinstance(line, bytes):
+                    line = line.decode("utf-8")
+                line_index += 1
+                line_strip = line.strip()
+                if line_strip == "" or line_strip[0] == "#":
+                    if line_strip[0] == "#":
+                        self.header_str += line_strip + "\n"
                     continue
-                CHROM,POS,ID,REF,ALT,QUAL,FILTER,INFO=line.split("\t")[:8]
-                info_dict={}
+                CHROM, POS, ID, REF, ALT, QUAL, FILTER, INFO = line.split("\t")[:8]
+                info_dict = {}
                 for info_item in INFO.split(";"):
                     if "=" in info_item:
-                        key,value=info_item.split("=")
+                        key, value = info_item.split("=")
                     else:
-                        key,value=info_item,True
-                    info_dict[key]=value
-                call=sv.SVCall(contig=CHROM,
-                               pos=int(POS)-1,
-                               id=line_index,
-                               ref=REF,
-                               alt=ALT,
-                               qual=QUAL,
-                               filter=FILTER,
-                               info=info_dict,
-                               svtype=None,
-                               svlen=None,
-                               end=None,
-                               rnames=None,
-                               qc=True,
-                               postprocess=None,
-                               genotypes=None,
-                               precise=None,
-                               support=0,
-                               fwd=0,
-                               rev=0,
-                               nm=-1)
-                if len(call.alt)>len(call.ref):
-                    call.svtype="INS"
-                    call.svlen=len(call.alt)
-                    call.end=call.pos
+                        key, value = info_item, True
+                    info_dict[key] = value
+                call = sv.SVCall(contig=CHROM,
+                                 pos=int(POS) - 1,
+                                 id=line_index,
+                                 ref=REF,
+                                 alt=ALT,
+                                 qual=QUAL,
+                                 filter=FILTER,
+                                 info=info_dict,
+                                 svtype=None,
+                                 svlen=None,
+                                 end=None,
+                                 rnames=None,
+                                 qc=True,
+                                 postprocess=None,
+                                 genotypes=None,
+                                 precise=None,
+                                 support=0,
+                                 fwd=0,
+                                 rev=0,
+                                 nm=-1)
+                if len(call.alt) > len(call.ref):
+                    call.svtype = "INS"
+                    call.svlen = len(call.alt)
+                    call.end = call.pos
                 else:
-                    call.svtype="DEL"
-                    call.svlen=-len(call.ref)
-                    call.end=call.pos+call.svlen
+                    call.svtype = "DEL"
+                    call.svlen = -len(call.ref)
+                    call.end = call.pos + call.svlen
 
                 if "SVTYPE" in info_dict:
-                    call.svtype=info_dict["SVTYPE"]
-                    if call.svtype=="TRA":
-                        call.svtype="BND"
+                    call.svtype = info_dict["SVTYPE"]
+                    if call.svtype == "TRA":
+                        call.svtype = "BND"
 
                 if "SVLEN" in info_dict:
-                    call.svlen=int(info_dict["SVLEN"])
+                    call.svlen = int(info_dict["SVLEN"])
                 if "END" in info_dict:
-                    call.end=int(info_dict["END"])
+                    call.end = int(info_dict["END"])
 
-                if call.svtype=="BND":
-                    bnd_parts=call.alt.replace("]","[").split("[")
-                    if len(bnd_parts)>2:
-                        mate_contig,mate_ref_start=bnd_parts[1].split(":")
-                        call.bnd_info=sv.SVCallBNDInfo(mate_contig=mate_contig, mate_ref_start=int(mate_ref_start), is_first=(call.alt[0]=="N"), is_reverse=("]" in call.alt))
+                if call.svtype == "BND":
+                    bnd_parts = call.alt.replace("]", "[").split("[")
+                    if len(bnd_parts) > 2:
+                        mate_contig, mate_ref_start = bnd_parts[1].split(":")
+                        call.bnd_info = sv.SVCallBNDInfo(mate_contig=mate_contig, mate_ref_start=int(mate_ref_start), is_first=(call.alt[0] == "N"), is_reverse=("]" in call.alt))
                     else:
                         raise ValueError("BND ALT not formatted according to VCF 4.2 specifications")
 
-                call.raw_vcf_line=line_strip
-                call.raw_vcf_line_index=line_index
+                call.raw_vcf_line = line_strip
+                call.raw_vcf_line_index = line_index
                 yield call
             except Exception as e:
                 util.fatal_error(f"Error parsing input VCF: Line {line_index}: {e}")
 
-    def rewrite_genotype(self,svcall):
-        parts_no_gt=svcall.raw_vcf_line.split("\t")[:8]
-        gt_format=self.config.genotype_format
+    def rewrite_genotype(self, svcall):
+        parts_no_gt = svcall.raw_vcf_line.split("\t")[:8]
+        gt_format = self.config.genotype_format
         if svcall.genotype_match_sv != None:
-            if len(svcall.genotype_match_sv.genotypes)>0:
-                gt=svcall.genotype_match_sv.genotypes[0]
+            if len(svcall.genotype_match_sv.genotypes) > 0:
+                gt = svcall.genotype_match_sv.genotypes[0]
             else:
-                gt=svcall.genotypes[0]
+                gt = svcall.genotypes[0]
         else:
-            gt=svcall.genotypes[0] #0/0 or ./. depending on whether input SV had coverage in sample
-        #parts=parts_no_gt + [gt_format,vcf.format_genotype(gt)]
-        #gt_vcf=svcall.raw_vcf_line.split("\t")[9].split(":")[0]
-        #parts= parts_no_gt + [gt_vcf] + [gt_format,vcf.format_genotype(gt)]
-        parts=parts_no_gt + [gt_format,format_genotype(gt)]
-        #parts[7]="NA"
-        #parts[3]=f"REF_{len(parts[3])}"
-        #parts[4]=f"ALT_{len(parts[4])}"
+            gt = svcall.genotypes[0]  # 0/0 or ./. depending on whether input SV had coverage in sample
+        # parts=parts_no_gt + [gt_format,vcf.format_genotype(gt)]
+        # gt_vcf=svcall.raw_vcf_line.split("\t")[9].split(":")[0]
+        # parts= parts_no_gt + [gt_vcf] + [gt_format,vcf.format_genotype(gt)]
+        parts = parts_no_gt + [gt_format, format_genotype(gt)]
+        # parts[7]="NA"
+        # parts[3]=f"REF_{len(parts[3])}"
+        # parts[4]=f"ALT_{len(parts[4])}"
         self.write_raw("\t".join(parts))
 
     def rewrite_header_genotype(self,orig_header):
         header_lines=orig_header.split("\n")
         header_lines.insert(1,'##genotypeFileDate="'+self.config.start_date+'"')
         header_lines.insert(1,'##genotypeCommand="'+self.config.command+'"')
         header_lines.insert(1,f"##genotypeSource={self.config.version}_{self.config.build}")
+
+        # Fix missing genotype headers errors when reading input vcf in genotype mode.
+        # This error will happen when input vcf does not have GT,GQ,DR,DV headers.
+        # Some tools such as turvari will throw errors when processing the output vcf.
+        has_gt_headers = {
+            "GT":False,
+            "GQ":False,
+            "DR":False,
+            "DV":False,
+        }
+        for header_line in header_lines:
+            for gt in has_gt_headers.keys():
+                if "##FORMAT=<ID="+gt+"," in header_line:
+                    has_gt_headers[gt] = True
+        
+        if not has_gt_headers["GT"]:
+            header_lines.insert(len(header_lines)-2,'##FORMAT=<ID=GT,Number=1,Type=String,Description="Genotype">')
+        if not has_gt_headers["GQ"]:
+            header_lines.insert(len(header_lines)-2,'##FORMAT=<ID=GQ,Number=1,Type=Integer,Description="Genotype quality">')
+        if not has_gt_headers["DR"]:
+            header_lines.insert(len(header_lines)-2,'##FORMAT=<ID=DR,Number=1,Type=Integer,Description="Number of reference reads">')
+        if not has_gt_headers["DV"]:
+            header_lines.insert(len(header_lines)-2,'##FORMAT=<ID=DV,Number=1,Type=Integer,Description="Number of variant reads">')
+
         self.write_raw("\n".join(header_lines),endl="")
 
     def close(self):
         self.handle.close()
```

### Comparing `sniffles-2.2/src/sniffles.egg-info/PKG-INFO` & `sniffles-2.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,30 @@
 Metadata-Version: 2.1
 Name: sniffles
-Version: 2.2
+Version: 2.3
 Summary: A fast structural variation caller for long-read sequencing data
 Home-page: https://github.com/fritzsedlazeck/Sniffles
-Author: Moritz Smolka, Luis Paulin
-Author-email: moritz.g.smolka@gmail.com, lfpaulin@gmail.com
+Author: Moritz Smolka, Hermann Romanek
+Author-email: moritz.g.smolka@gmail.com, sniffles@romanek.at
+License: MIT
 Project-URL: Bug Tracker, https://github.com/fritzsedlazeck/Sniffles/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pysam>=0.21.0
+Provides-Extra: align
+Requires-Dist: edlib>=1.3.9; extra == "align"
+Provides-Extra: mem
+Requires-Dist: psutil>=5.9.4; extra == "mem"
+Provides-Extra: all
+Requires-Dist: edlib>=1.3.9; extra == "all"
+Requires-Dist: psutil>=5.9.4; extra == "all"
 
 # Sniffles2
 A fast structural variant caller for long-read sequencing, Sniffles2 accurately detect SVs on germline, somatic and population-level for PacBio and Oxford Nanopore read data.
 
 ## Quick Start: Germline SV calling using Sniffles2
 To call SVs from long read alignments (PacBio / ONT), you can use:
 
@@ -28,35 +37,47 @@
 ## Installation
 You can install Sniffles2 using pip or conda using:
 
 `pip install sniffles`
 
 or
 
-`conda install sniffles=2.0 `
+`conda install sniffles=2.3`
 
 If you previously installed Sniffles1 using conda and want to upgrade to Sniffles2, you can use:
 
-`conda update sniffles=2.2`
+`conda update sniffles=2.3`
 
 ## Requirements
-* Python >= 3.8
-* pysam
+* Python >= 3.10
+* pysam >= 0.21.0
+
+### Optional requirements
+
+* edlib
+
+  If edlib is installed alignments are enabled by default during multi-sample SV/combine calling. This can be further tweaked (or disabled) with the `--combine-pctseq` argument. 
+
+* psutil
+
+  psutil can be used to facilitaty population calling with a large number of input files. 
 
 #### Tested on:
-* python==3.9.5
-* pysam==0.16.0.1
+* python==3.10.12
+* pysam==0.21.0
 
 ## Citation
 Please cite our paper at:
+Sniffles v2: 
+https://www.nature.com/articles/s41587-023-02024-y
 
+and 
+Sniffles v1:
 https://www.nature.com/articles/s41592-018-0001-7
 
-A new preprint for the new methods and improvements introduced with Sniffles2 is here: https://www.biorxiv.org/content/10.1101/2022.04.04.487055v1
-
 ## Use-Cases / Modes
 
 ### A. General (all Modes)
 * To output deletion (DEL SV) sequences, the reference genome (.fasta) must be specified using e.g. `--reference reference.fasta`.
 * Sniffles2 supports optionally specifying tandem repeat region annotations (.bed), which can improve calling in these regions `--tandem-repeats annotations.bed`. Sniffles2 compatible tandem repeat annotations for human references can be found in the [annotations/ folder](https://github.com/fritzsedlazeck/Sniffles/tree/master/annotations).
 * Sniffles2 is fully parallelized and uses 4 threads by default. This value can be adapted using e.g. `--threads 4` as option. Memory requirements will increase with the number of threads used.
 * To output read names in SNF and VCF files, the `--output-rnames` option is required.
@@ -86,7 +107,10 @@
 * .bam or .cram files containing long read alignments (i.e. from minimap2 or ngmlr) are supported as input
 * .vcf.gz (bgzipped+tabix indexed) output is supported
 * Simultaneous output of both .vcf and .snf file (for multi-sample calling) is supported
 
 ## Companion apps
 * We have developed a plotting tools for Sniffles2: [https://github.com/farhangus/sniffle2_plot](https://github.com/farhangus/sniffle2_plot)
 * We also provide VCF and scripts used for the manuscript [https://github.com/smolkmo/Sniffles2-Supplement](https://github.com/smolkmo/Sniffles2-Supplement) 
+
+## Supplementary tables
+[https://github.com/smolkmo/Sniffles2-Supplement/blob/main/Supplemetary%20tables.xlsx](https://github.com/smolkmo/Sniffles2-Supplement/blob/main/Supplemetary%20tables.xlsx)
```

