# Comparing `tmp/panisa-0.1.6.tar.gz` & `tmp/panisa-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panisa-0.1.6.tar", last modified: Mon Mar 28 08:27:25 2022, max compression
+gzip compressed data, was "panisa-0.1.7.tar", last modified: Wed Apr 10 12:36:37 2024, max compression
```

## Comparing `panisa-0.1.6.tar` & `panisa-0.1.7.tar`

### file list

```diff
@@ -1,30 +1,28 @@
-drwxrwx---   0 bvalot3   (1003) 2b2s      (1006)        0 2022-03-28 08:27:25.536653 panisa-0.1.6/
--rwxrwx---   0 bvalot3   (1003) 2b2s      (1006)     7418 2022-03-28 08:01:46.000000 panisa-0.1.6/ISFinder_search.py
--rw-r--r--   0 bvalot3   (1003) 2b2s      (1006)    35141 2017-02-23 14:14:48.000000 panisa-0.1.6/LICENSE
--rw-r--r--   0 bvalot3   (1003) 2b2s      (1006)       93 2018-01-10 13:58:54.000000 panisa-0.1.6/MANIFEST.in
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)      689 2022-03-28 08:27:25.536653 panisa-0.1.6/PKG-INFO
--rw-r--r--   0 bvalot3   (1003) 2b2s      (1006)     3353 2019-11-29 14:05:34.000000 panisa-0.1.6/README.rst
-drwxrwx---   0 bvalot3   (1003) 2b2s      (1006)        0 2022-03-28 08:27:25.536653 panisa-0.1.6/lib/
--rw-r--r--   0 bvalot3   (1003) 2b2s      (1006)      186 2018-01-10 09:04:27.000000 panisa-0.1.6/lib/__init__.py
--rw-r--r--   0 bvalot3   (1003) 2b2s      (1006)     1531 2018-01-10 09:07:28.000000 panisa-0.1.6/lib/bamreader.py
--rw-r--r--   0 bvalot3   (1003) 2b2s      (1006)     2634 2018-01-10 09:07:18.000000 panisa-0.1.6/lib/clipread.py
--rw-r--r--   0 bvalot3   (1003) 2b2s      (1006)     6048 2018-01-10 09:07:59.000000 panisa-0.1.6/lib/couple.py
--rw-r--r--   0 bvalot3   (1003) 2b2s      (1006)     2185 2019-11-29 15:25:27.000000 panisa-0.1.6/lib/gff.py
--rw-r--r--   0 bvalot3   (1003) 2b2s      (1006)     4019 2018-05-09 11:18:07.000000 panisa-0.1.6/lib/invertedrepeat.py
--rw-r--r--   0 bvalot3   (1003) 2b2s      (1006)     3380 2018-01-10 09:35:51.000000 panisa-0.1.6/lib/position.py
--rw-r--r--   0 bvalot3   (1003) 2b2s      (1006)     1051 2018-01-10 09:51:38.000000 panisa-0.1.6/lib/temporalfile.py
--rw-r--r--   0 bvalot3   (1003) 2b2s      (1006)      269 2022-03-28 08:21:16.000000 panisa-0.1.6/lib/variables.py
--rw-r--r--   0 bvalot3   (1003) 2b2s      (1006)      925 2018-05-04 11:32:27.000000 panisa-0.1.6/lib/writer.py
--rwxr-xr-x   0 bvalot3   (1003) 2b2s      (1006)     2554 2022-03-28 08:01:46.000000 panisa-0.1.6/panISa.py
-drwxrwx---   0 bvalot3   (1003) 2b2s      (1006)        0 2022-03-28 08:27:25.536653 panisa-0.1.6/panisa.egg-info/
--rw-r--r--   0 bvalot3   (1003) 2b2s      (1006)      689 2022-03-28 08:27:25.000000 panisa-0.1.6/panisa.egg-info/PKG-INFO
--rw-r--r--   0 bvalot3   (1003) 2b2s      (1006)      425 2022-03-28 08:27:25.000000 panisa-0.1.6/panisa.egg-info/SOURCES.txt
--rw-r--r--   0 bvalot3   (1003) 2b2s      (1006)        1 2022-03-28 08:27:25.000000 panisa-0.1.6/panisa.egg-info/dependency_links.txt
--rw-r--r--   0 bvalot3   (1003) 2b2s      (1006)       26 2022-03-28 08:27:25.000000 panisa-0.1.6/panisa.egg-info/requires.txt
--rw-r--r--   0 bvalot3   (1003) 2b2s      (1006)        4 2022-03-28 08:27:25.000000 panisa-0.1.6/panisa.egg-info/top_level.txt
--rw-r--r--   0 bvalot3   (1003) 2b2s      (1006)       67 2022-03-28 08:27:25.536653 panisa-0.1.6/setup.cfg
--rw-r--r--   0 bvalot3   (1003) 2b2s      (1006)     6600 2022-03-28 08:26:36.000000 panisa-0.1.6/setup.py
-drwxrwx---   0 bvalot3   (1003) 2b2s      (1006)        0 2022-03-28 08:27:25.536653 panisa-0.1.6/test/
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)      204 2022-03-28 08:08:55.000000 panisa-0.1.6/test/out
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)      338 2022-03-28 08:07:18.000000 panisa-0.1.6/test/result
--rw-r--r--   0 bvalot3   (1003) 2b2s      (1006)    30536 2017-02-24 12:21:25.000000 panisa-0.1.6/test/test.bam
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:36:37.904356 panisa-0.1.7/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7418 2024-04-10 12:36:33.000000 panisa-0.1.7/ISFinder_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-04-10 12:36:33.000000 panisa-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-10 12:36:33.000000 panisa-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4247 2024-04-10 12:36:37.904356 panisa-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-04-10 12:36:33.000000 panisa-0.1.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:36:37.904356 panisa-0.1.7/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-10 12:36:33.000000 panisa-0.1.7/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-10 12:36:33.000000 panisa-0.1.7/lib/bamreader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-10 12:36:33.000000 panisa-0.1.7/lib/clipread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-04-10 12:36:33.000000 panisa-0.1.7/lib/couple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-04-10 12:36:33.000000 panisa-0.1.7/lib/gff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-04-10 12:36:33.000000 panisa-0.1.7/lib/invertedrepeat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-04-10 12:36:33.000000 panisa-0.1.7/lib/position.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-10 12:36:33.000000 panisa-0.1.7/lib/temporalfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-10 12:36:33.000000 panisa-0.1.7/lib/variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-10 12:36:33.000000 panisa-0.1.7/lib/writer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2554 2024-04-10 12:36:33.000000 panisa-0.1.7/panISa.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:36:37.904356 panisa-0.1.7/panisa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4247 2024-04-10 12:36:37.000000 panisa-0.1.7/panisa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-10 12:36:37.000000 panisa-0.1.7/panisa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 12:36:37.000000 panisa-0.1.7/panisa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-10 12:36:37.000000 panisa-0.1.7/panisa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-10 12:36:37.000000 panisa-0.1.7/panisa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-10 12:36:37.904356 panisa-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6646 2024-04-10 12:36:33.000000 panisa-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:36:37.904356 panisa-0.1.7/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    30536 2024-04-10 12:36:33.000000 panisa-0.1.7/test/test.bam
```

### Comparing `panisa-0.1.6/ISFinder_search.py` & `panisa-0.1.7/ISFinder_search.py`

 * *Files identical despite different names*

### Comparing `panisa-0.1.6/LICENSE` & `panisa-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `panisa-0.1.6/README.rst` & `panisa-0.1.7/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: panisa
+Version: 0.1.7
+Summary: panISa is a software to search insertion sequence (IS) on resequencing data (bam file)
+Home-page: https://github.com/bvalot/panISa
+Author: Benoit Valot
+Author-email: benoit.valot@univ-fcomte.fr
+Keywords: bioinformatic IS bacteria
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: pysam>=0.9
+Requires-Dist: requests>=2.12
+
 panISa
 ======
 
 panISa is a software identifying insertion sequence (IS) on resequencing
 data (bam file) in bacterial genomes.
 
 Idea
@@ -19,51 +38,60 @@
 .. image:: principe.png
    :alt: Principe of panISa
    :align: center
 
 Requirements and Installation
 -----------------------------
 
+Conda installation
+~~~~~~~~~~~~~~~~~~
+
+You can easy install panisa program and requirements using conda:
+
+.. code-block:: bash
+
+   conda install -c bioconda panisa
+
 Requirements
 ~~~~~~~~~~~~
 
 The program used the python library **pysam** (>=0.9) and **request** (>=2.12)
 
 You need to install `the emboss package <http://emboss.sourceforge.net>`_
 
 In debian, type:
 
-.. raw:: html
+.. code-block:: bash
 
-   <pre>sudo apt-get install python-pysam python-requests emboss</pre>
+   sudo apt-get install python-pysam python-requests emboss
 
 Installation
 ~~~~~~~~~~~~
 
 Download the current tarball and unzip it.
 
 Verify the installation using the test file
 
-.. raw:: html
+.. code-block:: bash
 
-   <pre>python panISa.py test/test.bam</pre>
+   python panISa.py test/test.bam
 
 Alternatively, you can install from `PyPI repository <https://pypi.python.org/pypi>`_
 
-.. raw:: html
+.. code-block:: bash
 
-   <pre>pip install panisa</pre>
+   pip install panisa
 
    
 Command and Options
 -------------------
 
-.. raw:: html
+.. code-block:: bash
 
-   <pre>python panISa.py [options] bam</pre>
+   python panISa.py [options] bam
 
 Options
 ~~~~~~~
 
 -h     show this help message and exit
 -o     Return list of IS insertion by alignment [stdout]
 -q     Minimum alignment quality value to conserve a clipped read [20]
@@ -99,17 +127,17 @@
   reconstruction of the right boundary of the potential IS (IRR)
 
 Validation
 ----------
   
 PanISa results can be search for homology against ISFinder to find IS familly using the script ISFinder_search.py
 
-.. raw:: html
+.. code-block:: bash
 
-   <pre>python ISFinder_search.py [options] panISa results</pre>
+   python ISFinder_search.py [options] panISa results
 
 Recommandation
 --------------
 
 panISa works well with the alignment from **bwa** software.
 
 Citation
```

### Comparing `panisa-0.1.6/lib/bamreader.py` & `panisa-0.1.7/lib/bamreader.py`

 * *Files identical despite different names*

### Comparing `panisa-0.1.6/lib/clipread.py` & `panisa-0.1.7/lib/clipread.py`

 * *Files identical despite different names*

### Comparing `panisa-0.1.6/lib/couple.py` & `panisa-0.1.7/lib/couple.py`

 * *Files identical despite different names*

### Comparing `panisa-0.1.6/lib/gff.py` & `panisa-0.1.7/lib/gff.py`

 * *Files identical despite different names*

### Comparing `panisa-0.1.6/lib/invertedrepeat.py` & `panisa-0.1.7/lib/invertedrepeat.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,17 +41,17 @@
         
 
 def searchir(prime5seq, prime3seq):
     """Searched ir from 5 to 3 prime consensus and return InvertRepeat class or None"""
     range_ir_pos = 15
 
     ##test if consensus sequence is not empty
-    if prime5seq == "" or prime3seq:
+    if prime5seq == "" or prime3seq == "":
         return None
-    
+
     outseq_data = __performedirsearchwitheinverted(prime5seq, prime3seq)
     len_cons = __lenofconsensus(prime5seq, prime3seq)
 
     for invert in __getnextirfromeinverted(outseq_data,len_cons):
         if invert is None:
             return None
         invertRepeat = None
```

### Comparing `panisa-0.1.6/lib/position.py` & `panisa-0.1.7/lib/position.py`

 * *Files identical despite different names*

### Comparing `panisa-0.1.6/lib/temporalfile.py` & `panisa-0.1.7/lib/temporalfile.py`

 * *Files identical despite different names*

### Comparing `panisa-0.1.6/lib/writer.py` & `panisa-0.1.7/lib/writer.py`

 * *Files identical despite different names*

### Comparing `panisa-0.1.6/panISa.py` & `panisa-0.1.7/panISa.py`

 * *Files identical despite different names*

### Comparing `panisa-0.1.6/setup.py` & `panisa-0.1.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,30 +37,31 @@
 
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.1.6',  # Required
+    version='0.1.7',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='panISa is a software to search insertion sequence (IS) on resequencing data (bam file)',  # Required
 
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
     # Often, this is the same as your README, so you can just read it in from
     # that file directly (as we have already done above)
     #
     # This field corresponds to the "Description" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#description-optional
-    # long_description=long_description,  # Optional
+    long_description=long_description,  # Optional
+    long_description_content_type='text/x-rst',
 
     # This should be a valid link to your project's main homepage.
     #
     # This field corresponds to the "Home-Page" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#home-page-optional
     url='https://github.com/bvalot/panISa',  # Optional
```

### Comparing `panisa-0.1.6/test/test.bam` & `panisa-0.1.7/test/test.bam`

 * *Files identical despite different names*

