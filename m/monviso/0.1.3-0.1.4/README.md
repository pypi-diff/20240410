# Comparing `tmp/monviso-0.1.3.tar.gz` & `tmp/monviso-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/monviso-0.1.3.tar", last modified: Mon Apr  8 14:11:32 2024, max compression
+gzip compressed data, was "dist/monviso-0.1.4.tar", last modified: Wed Apr 10 10:46:44 2024, max compression
```

## Comparing `monviso-0.1.3.tar` & `monviso-0.1.4.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 albani     (502) staff       (20)        0 2024-04-08 14:11:32.655487 monviso-0.1.3/
--rw-r--r--   0 albani     (502) staff       (20)     2161 2024-04-08 14:10:29.000000 monviso-0.1.3/Containerfile
--rw-r--r--   0 albani     (502) staff       (20)      648 2024-04-08 14:10:41.000000 monviso-0.1.3/HISTORY.md
--rw-r--r--   0 albani     (502) staff       (20)     1211 2024-02-28 10:12:03.000000 monviso-0.1.3/LICENSE
--rw-r--r--   0 albani     (502) staff       (20)       92 2024-02-28 10:12:03.000000 monviso-0.1.3/MANIFEST.in
--rw-r--r--   0 albani     (502) staff       (20)     2260 2024-04-08 14:11:32.654957 monviso-0.1.3/PKG-INFO
--rw-r--r--   0 albani     (502) staff       (20)     1302 2024-02-28 10:12:03.000000 monviso-0.1.3/README.md
-drwxr-xr-x   0 albani     (502) staff       (20)        0 2024-04-08 14:11:32.600659 monviso-0.1.3/monviso.egg-info/
--rw-r--r--   0 albani     (502) staff       (20)     2260 2024-04-08 14:11:32.000000 monviso-0.1.3/monviso.egg-info/PKG-INFO
--rw-r--r--   0 albani     (502) staff       (20)     1433 2024-04-08 14:11:32.000000 monviso-0.1.3/monviso.egg-info/SOURCES.txt
--rw-r--r--   0 albani     (502) staff       (20)        1 2024-04-08 14:11:32.000000 monviso-0.1.3/monviso.egg-info/dependency_links.txt
--rw-r--r--   0 albani     (502) staff       (20)       69 2024-04-08 14:11:32.000000 monviso-0.1.3/monviso.egg-info/entry_points.txt
--rw-r--r--   0 albani     (502) staff       (20)      125 2024-04-08 14:11:32.000000 monviso-0.1.3/monviso.egg-info/requires.txt
--rw-r--r--   0 albani     (502) staff       (20)       17 2024-04-08 14:11:32.000000 monviso-0.1.3/monviso.egg-info/top_level.txt
-drwxr-xr-x   0 albani     (502) staff       (20)        0 2024-04-08 14:11:32.618400 monviso-0.1.3/monviso_reloaded/
--rw-r--r--   0 albani     (502) staff       (20)     6906 2024-02-28 10:12:03.000000 monviso-0.1.3/monviso_reloaded/PDB_manager.py
--rw-r--r--   0 albani     (502) staff       (20)        6 2024-04-08 14:10:48.000000 monviso-0.1.3/monviso_reloaded/VERSION
--rw-r--r--   0 albani     (502) staff       (20)        0 2024-02-28 10:12:03.000000 monviso-0.1.3/monviso_reloaded/__init__.py
--rw-r--r--   0 albani     (502) staff       (20)      158 2024-02-28 10:12:03.000000 monviso-0.1.3/monviso_reloaded/__main__.py
-drwxr-xr-x   0 albani     (502) staff       (20)        0 2024-04-08 14:11:32.650987 monviso-0.1.3/monviso_reloaded/__pycache__/
--rw-r--r--   0 albani     (502) staff       (20)     5885 2024-03-01 15:37:30.000000 monviso-0.1.3/monviso_reloaded/__pycache__/PDB_manager.cpython-39.pyc
--rw-r--r--   0 albani     (502) staff       (20)      172 2024-03-01 15:27:07.000000 monviso-0.1.3/monviso_reloaded/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 albani     (502) staff       (20)      309 2024-03-01 15:27:07.000000 monviso-0.1.3/monviso_reloaded/__pycache__/__main__.cpython-39.pyc
--rw-r--r--   0 albani     (502) staff       (20)     4774 2024-03-29 12:14:49.000000 monviso-0.1.3/monviso_reloaded/__pycache__/base.cpython-39.pyc
--rw-r--r--   0 albani     (502) staff       (20)      873 2024-03-01 15:27:07.000000 monviso-0.1.3/monviso_reloaded/__pycache__/cli.cpython-39.pyc
--rw-r--r--   0 albani     (502) staff       (20)     1983 2024-03-01 15:37:30.000000 monviso-0.1.3/monviso_reloaded/__pycache__/cobalt_wrapper.cpython-39.pyc
--rw-r--r--   0 albani     (502) staff       (20)     4744 2024-03-11 14:35:13.000000 monviso-0.1.3/monviso_reloaded/__pycache__/database_parser.cpython-39.pyc
--rw-r--r--   0 albani     (502) staff       (20)     4744 2024-03-11 14:31:42.000000 monviso-0.1.3/monviso_reloaded/__pycache__/file_handler.cpython-39.pyc
--rw-r--r--   0 albani     (502) staff       (20)     8605 2024-03-29 13:43:08.000000 monviso-0.1.3/monviso_reloaded/__pycache__/gene.cpython-39.pyc
--rw-r--r--   0 albani     (502) staff       (20)     6792 2024-03-01 15:46:41.000000 monviso-0.1.3/monviso_reloaded/__pycache__/input_parser.cpython-39.pyc
--rw-r--r--   0 albani     (502) staff       (20)    16845 2024-03-29 09:02:50.000000 monviso-0.1.3/monviso_reloaded/__pycache__/isoform.cpython-39.pyc
--rw-r--r--   0 albani     (502) staff       (20)    11467 2024-04-08 09:23:33.000000 monviso-0.1.3/monviso_reloaded/__pycache__/modeller_manager.cpython-39.pyc
--rw-r--r--   0 albani     (502) staff       (20)     4678 2024-03-01 15:37:30.000000 monviso-0.1.3/monviso_reloaded/__pycache__/template.cpython-39.pyc
--rw-r--r--   0 albani     (502) staff       (20)     4378 2024-03-29 11:42:41.000000 monviso-0.1.3/monviso_reloaded/base.py
--rw-r--r--   0 albani     (502) staff       (20)      570 2024-02-28 10:12:03.000000 monviso-0.1.3/monviso_reloaded/cli.py
--rw-r--r--   0 albani     (502) staff       (20)     1739 2024-02-28 10:12:03.000000 monviso-0.1.3/monviso_reloaded/cobalt_wrapper.py
--rw-r--r--   0 albani     (502) staff       (20)     4013 2024-03-11 14:35:11.000000 monviso-0.1.3/monviso_reloaded/database_parser.py
--rw-r--r--   0 albani     (502) staff       (20)     4181 2024-03-11 14:31:34.000000 monviso-0.1.3/monviso_reloaded/file_handler.py
--rw-r--r--   0 albani     (502) staff       (20)    12827 2024-03-29 13:41:56.000000 monviso-0.1.3/monviso_reloaded/gene.py
--rw-r--r--   0 albani     (502) staff       (20)     8954 2024-03-01 15:46:37.000000 monviso-0.1.3/monviso_reloaded/input_parser.py
--rw-r--r--   0 albani     (502) staff       (20)    21299 2024-03-29 09:02:47.000000 monviso-0.1.3/monviso_reloaded/isoform.py
--rw-r--r--   0 albani     (502) staff       (20)    13275 2024-04-08 14:05:11.000000 monviso-0.1.3/monviso_reloaded/modeller_manager.py
--rw-r--r--   0 albani     (502) staff       (20)     5480 2024-02-28 10:12:03.000000 monviso-0.1.3/monviso_reloaded/template.py
--rw-r--r--   0 albani     (502) staff       (20)       38 2024-04-08 14:11:32.655658 monviso-0.1.3/setup.cfg
--rw-r--r--   0 albani     (502) staff       (20)     1567 2024-02-28 11:07:33.000000 monviso-0.1.3/setup.py
-drwxr-xr-x   0 albani     (502) staff       (20)        0 2024-04-08 14:11:32.653953 monviso-0.1.3/tests/
--rw-r--r--   0 albani     (502) staff       (20)        0 2024-02-28 10:12:03.000000 monviso-0.1.3/tests/__init__.py
--rw-r--r--   0 albani     (502) staff       (20)      398 2024-02-28 10:12:03.000000 monviso-0.1.3/tests/conftest.py
--rw-r--r--   0 albani     (502) staff       (20)       96 2024-02-28 10:12:03.000000 monviso-0.1.3/tests/test_base.py
+drwxr-xr-x   0 albani     (502) staff       (20)        0 2024-04-10 10:46:44.285040 monviso-0.1.4/
+-rw-r--r--   0 albani     (502) staff       (20)     2173 2024-04-08 14:12:18.000000 monviso-0.1.4/Containerfile
+-rw-r--r--   0 albani     (502) staff       (20)      648 2024-04-08 14:10:41.000000 monviso-0.1.4/HISTORY.md
+-rw-r--r--   0 albani     (502) staff       (20)     1211 2024-02-28 10:12:03.000000 monviso-0.1.4/LICENSE
+-rw-r--r--   0 albani     (502) staff       (20)       92 2024-02-28 10:12:03.000000 monviso-0.1.4/MANIFEST.in
+-rw-r--r--   0 albani     (502) staff       (20)     2260 2024-04-10 10:46:44.278069 monviso-0.1.4/PKG-INFO
+-rw-r--r--   0 albani     (502) staff       (20)     1302 2024-02-28 10:12:03.000000 monviso-0.1.4/README.md
+drwxr-xr-x   0 albani     (502) staff       (20)        0 2024-04-10 10:46:44.213468 monviso-0.1.4/monviso.egg-info/
+-rw-r--r--   0 albani     (502) staff       (20)     2260 2024-04-10 10:46:44.000000 monviso-0.1.4/monviso.egg-info/PKG-INFO
+-rw-r--r--   0 albani     (502) staff       (20)     1433 2024-04-10 10:46:44.000000 monviso-0.1.4/monviso.egg-info/SOURCES.txt
+-rw-r--r--   0 albani     (502) staff       (20)        1 2024-04-10 10:46:44.000000 monviso-0.1.4/monviso.egg-info/dependency_links.txt
+-rw-r--r--   0 albani     (502) staff       (20)       69 2024-04-10 10:46:44.000000 monviso-0.1.4/monviso.egg-info/entry_points.txt
+-rw-r--r--   0 albani     (502) staff       (20)      125 2024-04-10 10:46:44.000000 monviso-0.1.4/monviso.egg-info/requires.txt
+-rw-r--r--   0 albani     (502) staff       (20)       17 2024-04-10 10:46:44.000000 monviso-0.1.4/monviso.egg-info/top_level.txt
+drwxr-xr-x   0 albani     (502) staff       (20)        0 2024-04-10 10:46:44.232317 monviso-0.1.4/monviso_reloaded/
+-rw-r--r--   0 albani     (502) staff       (20)     6906 2024-02-28 10:12:03.000000 monviso-0.1.4/monviso_reloaded/PDB_manager.py
+-rw-r--r--   0 albani     (502) staff       (20)        6 2024-04-10 10:39:52.000000 monviso-0.1.4/monviso_reloaded/VERSION
+-rw-r--r--   0 albani     (502) staff       (20)        0 2024-02-28 10:12:03.000000 monviso-0.1.4/monviso_reloaded/__init__.py
+-rw-r--r--   0 albani     (502) staff       (20)      158 2024-02-28 10:12:03.000000 monviso-0.1.4/monviso_reloaded/__main__.py
+drwxr-xr-x   0 albani     (502) staff       (20)        0 2024-04-10 10:46:44.264957 monviso-0.1.4/monviso_reloaded/__pycache__/
+-rw-r--r--   0 albani     (502) staff       (20)     5885 2024-03-01 15:37:30.000000 monviso-0.1.4/monviso_reloaded/__pycache__/PDB_manager.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)      172 2024-03-01 15:27:07.000000 monviso-0.1.4/monviso_reloaded/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)      309 2024-03-01 15:27:07.000000 monviso-0.1.4/monviso_reloaded/__pycache__/__main__.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)     4774 2024-03-29 12:14:49.000000 monviso-0.1.4/monviso_reloaded/__pycache__/base.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)      873 2024-03-01 15:27:07.000000 monviso-0.1.4/monviso_reloaded/__pycache__/cli.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)     1983 2024-03-01 15:37:30.000000 monviso-0.1.4/monviso_reloaded/__pycache__/cobalt_wrapper.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)     4744 2024-03-11 14:35:13.000000 monviso-0.1.4/monviso_reloaded/__pycache__/database_parser.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)     4744 2024-03-11 14:31:42.000000 monviso-0.1.4/monviso_reloaded/__pycache__/file_handler.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)     8605 2024-03-29 13:43:08.000000 monviso-0.1.4/monviso_reloaded/__pycache__/gene.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)     6792 2024-03-01 15:46:41.000000 monviso-0.1.4/monviso_reloaded/__pycache__/input_parser.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)    16845 2024-03-29 09:02:50.000000 monviso-0.1.4/monviso_reloaded/__pycache__/isoform.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)    11396 2024-04-09 12:59:44.000000 monviso-0.1.4/monviso_reloaded/__pycache__/modeller_manager.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)     4678 2024-03-01 15:37:30.000000 monviso-0.1.4/monviso_reloaded/__pycache__/template.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)     4378 2024-03-29 11:42:41.000000 monviso-0.1.4/monviso_reloaded/base.py
+-rw-r--r--   0 albani     (502) staff       (20)      570 2024-02-28 10:12:03.000000 monviso-0.1.4/monviso_reloaded/cli.py
+-rw-r--r--   0 albani     (502) staff       (20)     1739 2024-02-28 10:12:03.000000 monviso-0.1.4/monviso_reloaded/cobalt_wrapper.py
+-rw-r--r--   0 albani     (502) staff       (20)     4013 2024-03-11 14:35:11.000000 monviso-0.1.4/monviso_reloaded/database_parser.py
+-rw-r--r--   0 albani     (502) staff       (20)     4181 2024-03-11 14:31:34.000000 monviso-0.1.4/monviso_reloaded/file_handler.py
+-rw-r--r--   0 albani     (502) staff       (20)    12827 2024-03-29 13:41:56.000000 monviso-0.1.4/monviso_reloaded/gene.py
+-rw-r--r--   0 albani     (502) staff       (20)     8954 2024-03-01 15:46:37.000000 monviso-0.1.4/monviso_reloaded/input_parser.py
+-rw-r--r--   0 albani     (502) staff       (20)    21299 2024-03-29 09:02:47.000000 monviso-0.1.4/monviso_reloaded/isoform.py
+-rw-r--r--   0 albani     (502) staff       (20)    13278 2024-04-09 12:59:41.000000 monviso-0.1.4/monviso_reloaded/modeller_manager.py
+-rw-r--r--   0 albani     (502) staff       (20)     5480 2024-02-28 10:12:03.000000 monviso-0.1.4/monviso_reloaded/template.py
+-rw-r--r--   0 albani     (502) staff       (20)       38 2024-04-10 10:46:44.287119 monviso-0.1.4/setup.cfg
+-rw-r--r--   0 albani     (502) staff       (20)     1567 2024-02-28 11:07:33.000000 monviso-0.1.4/setup.py
+drwxr-xr-x   0 albani     (502) staff       (20)        0 2024-04-10 10:46:44.271430 monviso-0.1.4/tests/
+-rw-r--r--   0 albani     (502) staff       (20)        0 2024-02-28 10:12:03.000000 monviso-0.1.4/tests/__init__.py
+-rw-r--r--   0 albani     (502) staff       (20)      398 2024-02-28 10:12:03.000000 monviso-0.1.4/tests/conftest.py
+-rw-r--r--   0 albani     (502) staff       (20)       96 2024-02-28 10:12:03.000000 monviso-0.1.4/tests/test_base.py
```

### Comparing `monviso-0.1.3/Containerfile` & `monviso-0.1.4/Containerfile`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 RUN echo "source activate myenv" > ~/.bashrc
 ENV PATH /miniconda/envs/myenv/bin:$PATH
 
 # Install Modeller
 RUN conda install -c salilab modeller -y
 
 # Define a build-time argument for the Modeller license
-ARG MODELLER_LICENSE=XXXXXX
+ARG MODELLER_LICENSE=MODELIRANJE
 
 
 # Replace the placeholder in the Modeller configuration file with the license key
 RUN sed -i "s/XXXX/${MODELLER_LICENSE}/" /miniconda/lib/modeller-*/modlib/modeller/config.py
 
 
 # Download and extract Cobalt
@@ -55,8 +55,8 @@
 # Download and decompress the UniProt/SwissProt databases into /Monviso
 RUN wget https://ftp.uniprot.org/pub/databases/uniprot/current_release/knowledgebase/complete/uniprot_sprot.fasta.gz && \
     wget https://ftp.uniprot.org/pub/databases/uniprot/current_release/knowledgebase/complete/uniprot_sprot_varsplic.fasta.gz && \
     gzip -d uniprot_sprot.fasta.gz && \
     gzip -d uniprot_sprot_varsplic.fasta.gz
 
 # Install Monviso using pip in the myenv environment
-RUN /bin/bash -c "source activate myenv && pip install monviso"
+RUN /bin/bash -c "source activate myenv && pip install monviso==0.1.3"
```

### Comparing `monviso-0.1.3/HISTORY.md` & `monviso-0.1.4/HISTORY.md`

 * *Files identical despite different names*

### Comparing `monviso-0.1.3/LICENSE` & `monviso-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `monviso-0.1.3/PKG-INFO` & `monviso-0.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monviso
-Version: 0.1.3
+Version: 0.1.4
 Summary: MoNvIso is a comprehensive software tool designed for the analysis and modeling of protein isoforms. It automates the process of identifying canonical and additional isoforms, assessing their modeling propensity, mapping mutations accurately, and building structural models of proteins.
 Home-page: https://github.com/alisamalb/monviso_reloaded
 Author: Ciskio
 License: UNKNOWN
 Description: # Monviso reloaded
         MoNvIso is a comprehensive software tool designed for the analysis and modeling of protein isoforms. It automates the process of identifying canonical and additional isoforms, assessing their modeling propensity, mapping mutations accurately, and building structural models of proteins. By leveraging data from the Uniprot database, MoNvIso facilitates a deeper understanding of protein function and variation.
```

### Comparing `monviso-0.1.3/README.md` & `monviso-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `monviso-0.1.3/monviso.egg-info/PKG-INFO` & `monviso-0.1.4/monviso.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monviso
-Version: 0.1.3
+Version: 0.1.4
 Summary: MoNvIso is a comprehensive software tool designed for the analysis and modeling of protein isoforms. It automates the process of identifying canonical and additional isoforms, assessing their modeling propensity, mapping mutations accurately, and building structural models of proteins.
 Home-page: https://github.com/alisamalb/monviso_reloaded
 Author: Ciskio
 License: UNKNOWN
 Description: # Monviso reloaded
         MoNvIso is a comprehensive software tool designed for the analysis and modeling of protein isoforms. It automates the process of identifying canonical and additional isoforms, assessing their modeling propensity, mapping mutations accurately, and building structural models of proteins. By leveraging data from the Uniprot database, MoNvIso facilitates a deeper understanding of protein function and variation.
```

### Comparing `monviso-0.1.3/monviso.egg-info/SOURCES.txt` & `monviso-0.1.4/monviso.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `monviso-0.1.3/monviso_reloaded/PDB_manager.py` & `monviso-0.1.4/monviso_reloaded/PDB_manager.py`

 * *Files identical despite different names*

### Comparing `monviso-0.1.3/monviso_reloaded/__pycache__/PDB_manager.cpython-39.pyc` & `monviso-0.1.4/monviso_reloaded/__pycache__/PDB_manager.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `monviso-0.1.3/monviso_reloaded/__pycache__/base.cpython-39.pyc` & `monviso-0.1.4/monviso_reloaded/__pycache__/base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `monviso-0.1.3/monviso_reloaded/__pycache__/cli.cpython-39.pyc` & `monviso-0.1.4/monviso_reloaded/__pycache__/cli.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `monviso-0.1.3/monviso_reloaded/__pycache__/cobalt_wrapper.cpython-39.pyc` & `monviso-0.1.4/monviso_reloaded/__pycache__/cobalt_wrapper.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `monviso-0.1.3/monviso_reloaded/__pycache__/database_parser.cpython-39.pyc` & `monviso-0.1.4/monviso_reloaded/__pycache__/database_parser.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `monviso-0.1.3/monviso_reloaded/__pycache__/file_handler.cpython-39.pyc` & `monviso-0.1.4/monviso_reloaded/__pycache__/file_handler.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `monviso-0.1.3/monviso_reloaded/__pycache__/gene.cpython-39.pyc` & `monviso-0.1.4/monviso_reloaded/__pycache__/gene.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `monviso-0.1.3/monviso_reloaded/__pycache__/input_parser.cpython-39.pyc` & `monviso-0.1.4/monviso_reloaded/__pycache__/input_parser.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `monviso-0.1.3/monviso_reloaded/__pycache__/isoform.cpython-39.pyc` & `monviso-0.1.4/monviso_reloaded/__pycache__/isoform.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `monviso-0.1.3/monviso_reloaded/__pycache__/modeller_manager.cpython-39.pyc` & `monviso-0.1.4/monviso_reloaded/__pycache__/modeller_manager.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr  8 09:23:12 2024 UTC, .py size: 13351 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 80b7 1366 2734 0000  a..........f'4..
+00000000: 610d 0d0a 0000 0000 bd3b 1566 de33 0000  a........;.f.3..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3a00 0000 6400  .....@...s:...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6403 6404 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 4700 6405 6406 8400 6406  m.Z...G.d.d...d.
 00000060: 8302 5a06 6401 5300 2907 e900 0000 004e  ..Z.d.S.)......N
 00000070: 2901 da04 5061 7468 e901 0000 0029 01da  )...Path.....)..
@@ -221,497 +221,493 @@
 00000dc0: 6b6e 6f77 6e73 203d 2028 7a13 292c 0a20  knowns = (z.),. 
 00000dd0: 2020 2073 6571 7565 6e63 6520 3d20 227a     sequence = "z
 00000de0: 5922 2c0a 2020 2020 6173 7365 7373 5f6d  Y",.    assess_m
 00000df0: 6574 686f 6473 3d28 6173 7365 7373 2e44  ethods=(assess.D
 00000e00: 4f50 452c 2061 7373 6573 732e 4741 3334  OPE, assess.GA34
 00000e10: 3129 290a 612e 7374 6172 7469 6e67 5f6d  1)).a.starting_m
 00000e20: 6f64 656c 3d20 310a 612e 656e 6469 6e67  odel= 1.a.ending
-00000e30: 5f6d 6f64 656c 2020 3d20 7af5 0a61 2e6d  _model  = z..a.m
+00000e30: 5f6d 6f64 656c 2020 3d20 7aa9 0a61 2e6d  _model  = z..a.m
 00000e40: 616b 6528 290a 6f6b 5f6d 6f64 656c 7320  ake().ok_models 
 00000e50: 3d20 6669 6c74 6572 286c 616d 6264 6120  = filter(lambda 
 00000e60: 783a 2078 5b27 6661 696c 7572 6527 5d20  x: x['failure'] 
 00000e70: 6973 204e 6f6e 652c 2061 2e6f 7574 7075  is None, a.outpu
 00000e80: 7473 290a 746f 7363 6f72 6520 3d20 2744  ts).toscore = 'D
 00000e90: 4f50 4520 7363 6f72 6527 0a0a 6d6f 6465  OPE score'..mode
 00000ea0: 6c73 3d20 6c69 7374 286f 6b5f 6d6f 6465  ls= list(ok_mode
-00000eb0: 6c73 2920 6966 2069 7369 6e73 7461 6e63  ls) if isinstanc
-00000ec0: 6528 6f6b 5f6d 6f64 656c 732c 2074 7970  e(ok_models, typ
-00000ed0: 6528 6669 6c74 6572 286c 616d 6264 613a  e(filter(lambda:
-00000ee0: 204e 6f6e 652c 205b 5d29 2929 2065 6c73   None, []))) els
-00000ef0: 6520 6f6b 5f6d 6f64 656c 730a 6d6f 6465  e ok_models.mode
-00000f00: 6c73 2e73 6f72 7428 6b65 793d 6c61 6d62  ls.sort(key=lamb
-00000f10: 6461 206b 3a20 6b5b 746f 7363 6f72 655d  da k: k[toscore]
-00000f20: 290a 0a6d 796f 7574 203d 206f 7065 6e28  )..myout = open(
-00000f30: 2261 3401 0000 222c 2022 7722 290a 666f  "a4...", "w").fo
-00000f40: 7220 6d20 696e 206d 6f64 656c 733a 0a20  r m in models:. 
-00000f50: 2020 2020 2020 206d 796f 7574 2e77 7269         myout.wri
-00000f60: 7465 2873 7472 286d 5b27 6e61 6d65 275d  te(str(m['name']
-00000f70: 2920 2b20 2220 2844 4f50 4520 5343 4f52  ) + " (DOPE SCOR
-00000f80: 453a 2025 2e33 6629 2220 2520 286d 5b74  E: %.3f)" % (m[t
-00000f90: 6f73 636f 7265 5d29 290a 656e 762e 6c69  oscore])).env.li
-00000fa0: 6273 2e74 6f70 6f6c 6f67 792e 7265 6164  bs.topology.read
-00000fb0: 2866 696c 653d 2724 284c 4942 292f 746f  (file='$(LIB)/to
-00000fc0: 705f 6865 6176 2e6c 6962 2729 0a65 6e76  p_heav.lib').env
-00000fd0: 2e6c 6962 732e 7061 7261 6d65 7465 7273  .libs.parameters
-00000fe0: 2e72 6561 6428 6669 6c65 3d27 2428 4c49  .read(file='$(LI
-00000ff0: 4229 2f70 6172 2e6c 6962 2729 0a6d 646c  B)/par.lib').mdl
-00001000: 203d 2063 6f6d 706c 6574 655f 7064 6228   = complete_pdb(
-00001010: 656e 762c 206d 5b27 6e61 6d65 275d 290a  env, m['name']).
-00001020: 7320 3d20 7365 6c65 6374 696f 6e28 6d64  s = selection(md
-00001030: 6c29 0a73 2e61 7373 6573 735f 646f 7065  l).s.assess_dope
-00001040: 286f 7574 7075 743d 2745 4e45 5247 595f  (output='ENERGY_
-00001050: 5052 4f46 494c 4520 4e4f 5f52 4550 4f52  PROFILE NO_REPOR
-00001060: 5427 2c20 6669 6c65 3d22 7a2f 222c 206e  T', file="z/", n
-00001070: 6f72 6d61 6c69 7a65 5f70 726f 6669 6c65  ormalize_profile
-00001080: 3d54 7275 652c 2073 6d6f 6f74 6869 6e67  =True, smoothing
-00001090: 5f77 696e 646f 773d 3135 2929 0e72 1300  _window=15)).r..
-000010a0: 0000 7206 0000 0072 0200 0000 720d 0000  ..r....r....r...
-000010b0: 00da 086f 7574 5f70 6174 68da 0974 656d  ...out_path..tem
-000010c0: 706c 6174 6573 da03 7374 72da 0572 616e  plates..str..ran
-000010d0: 6765 7210 0000 0072 1100 0000 721b 0000  ger....r....r...
-000010e0: 0072 1400 0000 7204 0000 00da 0a77 7269  .r....r......wri
-000010f0: 7465 5f66 696c 6529 0772 1500 0000 da0e  te_file).r......
-00001100: 616c 6967 6e6d 656e 745f 6e61 6d65 5a0b  alignment_nameZ.
-00001110: 6f75 7470 7574 5f6e 616d 65da 0b73 6372  output_name..scr
-00001120: 6970 745f 7061 7468 5a0e 7465 6d70 6c61  ipt_pathZ.templa
-00001130: 7465 5f6e 616d 6573 da07 636f 6e74 656e  te_names..conten
-00001140: 74da 0266 6872 1600 0000 7216 0000 0072  t..fhr....r....r
-00001150: 1700 0000 721e 0000 003e 0000 0073 5a00  ....r....>...sZ.
-00001160: 0000 0001 1401 1401 0201 0601 12fe 0404  ................
-00001170: 0602 06fe 0605 0207 16f9 0207 02f9 0208  ................
-00001180: 08f8 0208 02f8 0210 02f0 0211 02ef 0213  ................
-00001190: 06ed 0214 02ec 0216 06ea 0217 02e9 021a  ................
-000011a0: 08e6 021a 02e6 0223 02dd 0224 02dc 022c  .......#...$...,
-000011b0: 06d4 022d 02d3 02ff 0231 0801 7a1d 4d6f  ...-.....1..z.Mo
-000011c0: 6465 6c6c 6572 5f6d 616e 6167 6572 2e77  deller_manager.w
-000011d0: 7269 7465 5f73 6372 6970 7429 0272 2a00  rite_script).r*.
-000011e0: 0000 7220 0000 0063 0300 0000 0000 0000  ..r ...c........
-000011f0: 0000 0000 0500 0000 0400 0000 4300 0000  ............C...
-00001200: 73a8 0000 007c 0164 016b 0272 0c7c 0253  s....|.d.k.r.|.S
-00001210: 0074 007c 0164 0219 0083 0164 0218 007d  .t.|.d.....d...}
-00001220: 037c 0374 017c 0283 016b 0072 947c 037c  .|.t.|...k.r.|.|
-00001230: 0264 037c 0385 0219 00a0 0264 04a1 0118  .d.|.......d....
-00001240: 007d 047c 0464 0217 0074 007c 0164 0219  .}.|.d...t.|.d..
-00001250: 0083 016b 0272 8a7c 027c 0319 007c 0164  ...k.r.|.|...|.d
-00001260: 0519 006b 0272 8a7c 0264 037c 0385 0219  ...k.r.|.d.|....
-00001270: 007c 0164 0619 0017 007c 027c 0364 0217  .|.d.....|.|.d..
-00001280: 0064 0385 0219 0017 007d 027c 0253 007c  .d.......}.|.S.|
-00001290: 0364 0237 007d 0371 1c74 0364 077c 019b  .d.7.}.q.t.d.|..
-000012a0: 0064 089d 0383 0101 007c 0253 0029 097a  .d.......|.S.).z
-000012b0: ea54 616b 6520 6120 6d75 7461 7469 6f6e  .Take a mutation
-000012c0: 2069 6e20 7468 6520 666f 726d 6174 0a20   in the format. 
-000012d0: 2020 2020 2020 205b 3120 6c65 7474 6572         [1 letter
-000012e0: 2061 6d69 6e6f 2061 6369 642c 7265 7369   amino acid,resi
-000012f0: 6475 6520 6e75 6d62 6572 2c20 3120 6c65  due number, 1 le
-00001300: 7474 2e20 616d 696e 6f20 6163 6964 5d0a  tt. amino acid].
-00001310: 2020 2020 2020 2020 616e 6420 6170 706c          and appl
-00001320: 7920 6974 2074 6f20 7468 6520 616c 6967  y it to the alig
-00001330: 6e65 6420 7365 7175 656e 6365 2074 6f20  ned sequence to 
-00001340: 6d6f 6465 6c2c 0a20 2020 2020 2020 2074  model,.        t
-00001350: 616b 696e 6720 696e 746f 2061 6363 6f75  aking into accou
-00001360: 6e74 2061 6c6c 2074 6865 2022 2d22 2773  nt all the "-"'s
-00001370: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-00001380: 6e73 2065 6469 7465 6420 7365 7175 656e  ns edited sequen
-00001390: 6365 0a20 2020 2020 2020 2072 0c00 0000  ce.        r....
-000013a0: 7203 0000 004e fa01 2d72 0100 0000 e902  r....N..-r......
-000013b0: 0000 007a 1943 6f75 6c64 206e 6f74 2061  ...z.Could not a
-000013c0: 7070 6c79 206d 7574 6174 696f 6e20 fa01  pply mutation ..
-000013d0: 2129 0472 2700 0000 da03 6c65 6eda 0563  !).r'.....len..c
-000013e0: 6f75 6e74 721a 0000 0029 0572 1500 0000  ountr....).r....
-000013f0: 7206 0000 0072 2a00 0000 7236 0000 005a  r....r*...r6...Z
-00001400: 1461 6374 7561 6c5f 7265 7369 6475 655f  .actual_residue_
-00001410: 696e 6465 7872 1600 0000 7216 0000 0072  indexr....r....r
-00001420: 1700 0000 da0e 5f6d 7574 6174 655f 7265  ......_mutate_re
-00001430: 7369 6465 7d00 0000 7326 0000 0000 0908  side}...s&......
-00001440: 0104 0310 010c 0116 0212 ff02 020e fe02  ................
-00001450: 040a 0106 ff02 020e fe02 ff02 0504 010a  ................
-00001460: 0210 017a 1f4d 6f64 656c 6c65 725f 6d61  ...z.Modeller_ma
-00001470: 6e61 6765 722e 5f6d 7574 6174 655f 7265  nager._mutate_re
-00001480: 7369 6465 6302 0000 0000 0000 0000 0000  sidec...........
-00001490: 0005 0000 0005 0000 0043 0000 0073 4400  .........C...sD.
-000014a0: 0000 6700 7d02 6401 7d03 7c01 4400 5d32  ..g.}.d.}.|.D.]2
-000014b0: 7d04 7c04 6402 6b02 7228 7c02 a000 6402  }.|.d.k.r(|...d.
-000014c0: 7c04 6702 a101 0100 710c 7c02 a000 7c03  |.g.....q.|...|.
-000014d0: 7c04 6702 a101 0100 7c03 6401 3700 7d03  |.g.....|.d.7.}.
-000014e0: 710c 7c02 5300 2903 7a37 4672 6f6d 2061  q.|.S.).z7From a
-000014f0: 2073 6571 7565 6e63 652c 2072 6574 7572   sequence, retur
-00001500: 6e20 6120 3244 206c 6973 7420 7769 7468  n a 2D list with
-00001510: 205b 7265 736e 756d 2c72 6573 6975 6465   [resnum,resiude
-00001520: 5d72 0300 0000 7240 0000 0029 0172 2900  ]r....r@...).r).
-00001530: 0000 2905 7215 0000 0072 2a00 0000 5a0c  ..).r....r*...Z.
-00001540: 6e75 6d62 6572 6564 5f73 6571 7236 0000  numbered_seqr6..
-00001550: 00da 0463 6861 7272 1600 0000 7216 0000  ...charr....r...
-00001560: 0072 1700 0000 da17 5f61 6464 5f6e 756d  .r......_add_num
-00001570: 6265 725f 746f 5f73 6571 7565 6e63 659b  ber_to_sequence.
-00001580: 0000 0073 1000 0000 0002 0401 0401 0801  ...s............
-00001590: 0801 1002 0e01 0a01 7a28 4d6f 6465 6c6c  ........z(Modell
-000015a0: 6572 5f6d 616e 6167 6572 2e5f 6164 645f  er_manager._add_
-000015b0: 6e75 6d62 6572 5f74 6f5f 7365 7175 656e  number_to_sequen
-000015c0: 6365 4e29 02da 1473 6571 7565 6e63 655f  ceN)...sequence_
-000015d0: 7769 7468 5f72 6573 6e75 6d72 2000 0000  with_resnumr ...
-000015e0: 6302 0000 0000 0000 0000 0000 0004 0000  c...............
-000015f0: 0005 0000 0043 0000 0073 6200 0000 6401  .....C...sb...d.
-00001600: 6402 8400 7c01 4400 8301 7d02 7c00 6a00  d...|.D...}.|.j.
-00001610: a001 7c02 6403 1900 a101 0100 7402 6404  ..|.d.......t.d.
-00001620: 7403 7c02 8301 8302 4400 5d30 7d03 7c02  t.|.....D.]0}.|.
-00001630: 7c03 1900 7c02 7c03 6404 1800 1900 6404  |...|.|.d.....d.
-00001640: 1700 6b03 722c 7c00 6a00 a001 7c02 7c03  ..k.r,|.j...|.|.
-00001650: 1900 6404 1800 a101 0100 712c 6405 5300  ..d.......q,d.S.
-00001660: 2906 7aa7 4769 7665 6e20 6120 7365 7175  ).z.Given a sequ
-00001670: 656e 6365 2073 6176 6564 2061 7320 6120  ence saved as a 
-00001680: 6c69 7374 205b 7265 736e 756d 2c20 7265  list [resnum, re
-00001690: 7369 6475 655d 2c0a 2020 2020 2020 2020  sidue],.        
-000016a0: 7361 7665 2061 6c6c 2074 6865 2072 6573  save all the res
-000016b0: 6964 7565 206e 756d 6265 7273 2074 6861  idue numbers tha
-000016c0: 7420 7265 7072 6573 656e 7420 616e 2069  t represent an i
-000016d0: 6e74 6572 7275 7074 696f 6e0a 2020 2020  nterruption.    
-000016e0: 2020 2020 696e 2074 6865 2063 6f6e 7469      in the conti
-000016f0: 6e75 6974 7920 6f66 2074 6865 2070 726f  nuity of the pro
-00001700: 7465 696e 2063 6861 696e 2e63 0100 0000  tein chain.c....
-00001710: 0000 0000 0000 0000 0200 0000 0400 0000  ................
-00001720: 5300 0000 7320 0000 0067 007c 005d 187d  S...s ...g.|.].}
-00001730: 017c 0164 0019 0064 016b 0372 047c 0164  .|.d...d.k.r.|.d
-00001740: 0019 0091 0271 0453 0029 0272 0100 0000  .....q.S.).r....
-00001750: 7240 0000 0072 1600 0000 7222 0000 0072  r@...r....r"...r
-00001760: 1600 0000 7216 0000 0072 1700 0000 7225  ....r....r....r%
-00001770: 0000 00ad 0000 0072 2600 0000 7a37 4d6f  .......r&...z7Mo
-00001780: 6465 6c6c 6572 5f6d 616e 6167 6572 2e5f  deller_manager._
-00001790: 7361 7665 5f63 6861 696e 5f73 7461 7274  save_chain_start
-000017a0: 732e 3c6c 6f63 616c 733e 2e3c 6c69 7374  s.<locals>.<list
-000017b0: 636f 6d70 3e72 0100 0000 7203 0000 004e  comp>r....r....N
-000017c0: 2904 7211 0000 0072 2900 0000 723a 0000  ).r....r)...r:..
-000017d0: 0072 4300 0000 2904 7215 0000 0072 4800  .rC...).r....rH.
-000017e0: 0000 5a10 6669 6c74 6572 6564 5f6e 756d  ..Z.filtered_num
-000017f0: 6265 7273 7236 0000 0072 1600 0000 7216  bersr6...r....r.
-00001800: 0000 0072 1700 0000 da12 5f73 6176 655f  ...r......_save_
-00001810: 6368 6169 6e5f 7374 6172 7473 a700 0000  chain_starts....
-00001820: 730a 0000 0000 060e 0310 0212 0118 017a  s..............z
-00001830: 234d 6f64 656c 6c65 725f 6d61 6e61 6765  #Modeller_manage
-00001840: 722e 5f73 6176 655f 6368 6169 6e5f 7374  r._save_chain_st
-00001850: 6172 7473 2902 da09 7365 7175 656e 6365  arts)...sequence
-00001860: 7372 2000 0000 6302 0000 0000 0000 0000  sr ...c.........
-00001870: 0000 0009 0000 0006 0000 0003 0000 0073  ...............s
-00001880: ba01 0000 6401 6402 8400 7c01 4400 8301  ....d.d...|.D...
-00001890: 8902 6403 6402 8400 7c01 4400 8301 8900  ..d.d...|.D.....
-000018a0: 7c00 a000 8800 6404 1900 a101 7d02 7401  |.....d.....}.t.
-000018b0: 6405 6402 8400 8800 4400 8301 8301 8901  d.d.....D.......
-000018c0: 8801 7c00 6a02 6b05 9001 723e 8701 6601  ..|.j.k...r>..f.
-000018d0: 6406 6402 8408 8800 6407 6408 8502 1900  d.d.....d.d.....
-000018e0: 4400 8301 7d03 7403 7c03 8301 7404 8800  D...}.t.|...t...
-000018f0: 8301 6407 1800 6b02 9001 7234 8701 6601  ..d...k...r4..f.
-00001900: 6409 6402 8408 8800 6407 6408 8502 1900  d.d.....d.d.....
-00001910: 4400 8301 7d04 7c04 4400 5d9c 8903 8701  D...}.|.D.].....
-00001920: 8703 6602 640a 6402 8408 8800 6407 6408  ..f.d.d.....d.d.
-00001930: 8502 1900 4400 8301 7d05 7403 7c05 8301  ....D...}.t.|...
-00001940: 7404 8800 8301 6407 1800 6b02 7296 7c02  t.....d...k.r.|.
-00001950: 6408 8803 8502 1900 7c02 8803 8801 1700  d.......|.......
-00001960: 6408 8502 1900 1700 7d02 7405 8800 8301  d.......}.t.....
-00001970: 4400 5d3a 5c02 7d06 7d07 7c07 6408 8803  D.]:\.}.}.|.d...
-00001980: 8502 1900 640b 1700 7c07 8803 8801 1700  ....d...|.......
-00001990: 6408 8502 1900 1700 8800 7c06 3c00 7c00  d.........|.<.|.
-000019a0: 0400 6a06 6407 3700 0200 5f06 71ee 8801  ..j.d.7..._.q...
-000019b0: 6407 3700 8901 7196 8801 6407 3800 8901  d.7...q...d.8...
-000019c0: 713c 8700 8702 6602 640c 6402 8408 7407  q<....f.d.d...t.
-000019d0: 7404 8802 8301 8301 4400 8301 7d01 7c01  t.......D...}.|.
-000019e0: 6404 1900 6407 1900 6404 1900 640b 6b02  d...d...d...d.k.
-000019f0: 9001 727e 640d 6402 8400 7c01 4400 8301  ..r~d.d...|.D...
-00001a00: 7d01 7c01 6404 1900 6407 1900 640e 1900  }.|.d...d...d...
-00001a10: 640b 6b02 9001 72a2 640f 6402 8400 7c01  d.k...r.d.d...|.
-00001a20: 4400 8301 7d01 7c00 a008 7c02 a101 0100  D...}.|...|.....
-00001a30: 7c00 a009 7c02 a101 7d08 7c01 5300 2910  |...|...}.|.S.).
-00001a40: 619f 0100 0046 6f72 2061 6c69 676e 6d65  a....For alignme
-00001a50: 6e74 7320 696e 2077 6869 6368 2074 6865  nts in which the
-00001a60: 7265 2069 7320 6e6f 2063 6f76 6572 6167  re is no coverag
-00001a70: 6520 666f 7220 7365 6c66 2e6d 6f64 656c  e for self.model
-00001a80: 5f63 7574 6f66 662b 0a20 2020 2020 2020  _cutoff+.       
-00001a90: 2072 6573 6964 7565 732c 2074 6865 2073   residues, the s
-00001aa0: 6563 7469 6f6e 2077 6974 686f 7574 2063  ection without c
-00001ab0: 6f76 6572 6167 6520 6973 2072 6570 6c61  overage is repla
-00001ac0: 6365 6420 6279 0a20 2020 2020 2020 2063  ced by.        c
-00001ad0: 6861 696e 2062 7265 616b 732e 0a0a 2020  hain breaks...  
-00001ae0: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
-00001af0: 2020 2020 2020 2020 7365 7175 656e 6365          sequence
-00001b00: 7320 286c 6973 7429 3a20 4120 6c69 7374  s (list): A list
-00001b10: 206f 6620 5b6e 616d 652c 2073 6571 7565   of [name, seque
-00001b20: 6e63 655d 206c 6973 7473 2c0a 2020 2020  nce] lists,.    
-00001b30: 2020 2020 2020 2020 6f6e 6520 666f 7220          one for 
-00001b40: 6561 6368 2073 6571 7565 6e63 6520 746f  each sequence to
-00001b50: 2062 6520 7772 6974 7465 6e20 696e 2074   be written in t
-00001b60: 6865 206d 6f64 656c 6c65 720a 2020 2020  he modeller.    
-00001b70: 2020 2020 2020 2020 616c 6967 6e6d 656e          alignmen
-00001b80: 7420 696e 7075 7420 6669 6c65 2e0a 0a20  t input file... 
-00001b90: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
-00001ba0: 2020 2020 2020 2020 2020 2020 6c69 7374              list
-00001bb0: 3a20 5265 7475 726e 7320 7468 6520 7361  : Returns the sa
-00001bc0: 6d65 206c 6973 742c 2077 6974 6820 6368  me list, with ch
-00001bd0: 6169 6e20 6272 6561 6b73 2e0a 2020 2020  ain breaks..    
-00001be0: 2020 2020 6301 0000 0000 0000 0000 0000      c...........
-00001bf0: 0002 0000 0004 0000 0053 0000 0073 1400  .........S...s..
-00001c00: 0000 6700 7c00 5d0c 7d01 7c01 6400 1900  ..g.|.].}.|.d...
-00001c10: 9102 7104 5300 7221 0000 0072 1600 0000  ..q.S.r!...r....
-00001c20: a902 7223 0000 00da 066f 626a 6563 7472  ..r#.....objectr
-00001c30: 1600 0000 7216 0000 0072 1700 0000 7225  ....r....r....r%
-00001c40: 0000 00c5 0000 0072 2600 0000 7a36 4d6f  .......r&...z6Mo
-00001c50: 6465 6c6c 6572 5f6d 616e 6167 6572 2e5f  deller_manager._
-00001c60: 6164 645f 6368 6169 6e5f 6272 6561 6b73  add_chain_breaks
-00001c70: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
-00001c80: 6f6d 703e 6301 0000 0000 0000 0000 0000  omp>c...........
-00001c90: 0002 0000 0004 0000 0053 0000 0073 1400  .........S...s..
-00001ca0: 0000 6700 7c00 5d0c 7d01 7c01 6400 1900  ..g.|.].}.|.d...
-00001cb0: 9102 7104 5300 2901 7203 0000 0072 1600  ..q.S.).r....r..
-00001cc0: 0000 724b 0000 0072 1600 0000 7216 0000  ..rK...r....r...
-00001cd0: 0072 1700 0000 7225 0000 00c6 0000 0072  .r....r%.......r
-00001ce0: 2600 0000 7201 0000 0063 0100 0000 0000  &...r....c......
-00001cf0: 0000 0000 0000 0200 0000 0500 0000 5300  ..............S.
-00001d00: 0000 7316 0000 0067 007c 005d 0e7d 017c  ..s....g.|.].}.|
-00001d10: 01a0 0064 00a1 0191 0271 0453 00a9 0172  ...d.....q.S...r
-00001d20: 4000 0000 2901 7244 0000 00a9 0272 2300  @...).rD.....r#.
-00001d30: 0000 da03 7365 7172 1600 0000 7216 0000  ....seqr....r...
-00001d40: 0072 1700 0000 7225 0000 00cb 0000 0072  .r....r%.......r
-00001d50: 2600 0000 6301 0000 0000 0000 0000 0000  &...c...........
-00001d60: 0002 0000 0004 0000 0013 0000 0073 1800  .............s..
-00001d70: 0000 6700 7c00 5d10 7d01 6400 8800 1400  ..g.|.].}.d.....
-00001d80: 7c01 7600 9102 7104 5300 724d 0000 0072  |.v...q.S.rM...r
-00001d90: 1600 0000 724e 0000 00a9 01da 0f6d 6178  ....rN.......max
-00001da0: 5f6e 6f6e 5f63 6f76 6572 6564 7216 0000  _non_coveredr...
-00001db0: 0072 1700 0000 7225 0000 00d3 0000 0073  .r....r%.......s
-00001dc0: 0200 0000 0601 7203 0000 004e 6301 0000  ......r....Nc...
-00001dd0: 0000 0000 0000 0000 0002 0000 0006 0000  ................
-00001de0: 0013 0000 0073 1a00 0000 6700 7c00 5d12  .....s....g.|.].
-00001df0: 7d01 7c01 a000 6400 8800 1400 a101 9102  }.|...d.........
-00001e00: 7104 5300 724d 0000 0029 01da 0466 696e  q.S.rM...)...fin
-00001e10: 6472 4e00 0000 7250 0000 0072 1600 0000  drN...rP...r....
-00001e20: 7217 0000 0072 2500 0000 dc00 0000 7302  r....r%.......s.
-00001e30: 0000 0006 0163 0100 0000 0000 0000 0000  .....c..........
-00001e40: 0000 0200 0000 0600 0000 1300 0000 7324  ..............s$
-00001e50: 0000 0067 007c 005d 1c7d 017c 0188 0188  ...g.|.].}.|....
-00001e60: 0188 0017 0085 0219 0064 0088 0014 006b  .........d.....k
-00001e70: 0291 0271 0453 0072 4d00 0000 7216 0000  ...q.S.rM...r...
-00001e80: 0072 4e00 0000 2902 7251 0000 00da 0370  .rN...).rQ.....p
-00001e90: 6f73 7216 0000 0072 1700 0000 7225 0000  osr....r....r%..
-00001ea0: 00e0 0000 0073 0800 0000 0603 02fe 0e01  .....s..........
-00001eb0: 06ff fa01 2f63 0100 0000 0000 0000 0000  ..../c..........
-00001ec0: 0000 0200 0000 0500 0000 1300 0000 731c  ..............s.
-00001ed0: 0000 0067 007c 005d 147d 0188 017c 0119  ...g.|.].}...|..
-00001ee0: 0088 007c 0119 0067 0291 0271 0453 0072  ...|...g...q.S.r
-00001ef0: 1600 0000 7216 0000 0072 3500 0000 2902  ....r....r5...).
-00001f00: da0b 616c 6967 6e65 645f 7365 71da 056e  ..aligned_seq..n
-00001f10: 616d 6573 7216 0000 0072 1700 0000 7225  amesr....r....r%
-00001f20: 0000 00f4 0000 0072 2600 0000 6301 0000  .......r&...c...
-00001f30: 0000 0000 0000 0000 0002 0000 0006 0000  ................
-00001f40: 0053 0000 0073 2400 0000 6700 7c00 5d1c  .S...s$...g.|.].
-00001f50: 7d01 7c01 6400 1900 7c01 6401 1900 6401  }.|.d...|.d...d.
-00001f60: 6402 8502 1900 6702 9102 7104 5300 2903  d.....g...q.S.).
-00001f70: 7201 0000 0072 0300 0000 4e72 1600 0000  r....r....Nr....
-00001f80: a902 7223 0000 00da 0173 7216 0000 0072  ..r#.....sr....r
-00001f90: 1600 0000 7217 0000 0072 2500 0000 f800  ....r....r%.....
-00001fa0: 0000 7226 0000 00e9 ffff ffff 6301 0000  ..r&........c...
-00001fb0: 0000 0000 0000 0000 0002 0000 0006 0000  ................
-00001fc0: 0053 0000 0073 2400 0000 6700 7c00 5d1c  .S...s$...g.|.].
-00001fd0: 7d01 7c01 6400 1900 7c01 6401 1900 6402  }.|.d...|.d...d.
-00001fe0: 6403 8502 1900 6702 9102 7104 5300 2904  d.....g...q.S.).
-00001ff0: 7201 0000 0072 0300 0000 4e72 5900 0000  r....r....NrY...
-00002000: 7216 0000 0072 5700 0000 7216 0000 0072  r....rW...r....r
-00002010: 1600 0000 7217 0000 0072 2500 0000 fa00  ....r....r%.....
-00002020: 0000 7226 0000 0029 0a72 4700 0000 da03  ..r&...).rG.....
-00002030: 6d61 7872 0800 0000 da03 7375 6d72 4300  maxr......sumrC.
-00002040: 0000 da09 656e 756d 6572 6174 6572 1000  ....enumerater..
-00002050: 0000 723a 0000 0072 4900 0000 722b 0000  ..r:...rI...r+..
-00002060: 0029 0972 1500 0000 724a 0000 005a 0e6e  .).r....rJ...Z.n
-00002070: 756d 5f74 6172 6765 745f 7365 71da 0e63  um_target_seq..c
-00002080: 6865 636b 5f70 7265 7365 6e63 65da 0970  heck_presence..p
-00002090: 6f73 6974 696f 6e73 da0e 6368 6563 6b5f  ositions..check_
-000020a0: 706f 7369 7469 6f6e 7236 0000 0072 4f00  positionr6...rO.
-000020b0: 0000 722f 0000 0072 1600 0000 2904 7255  ..r/...r....).rU
-000020c0: 0000 0072 5100 0000 7256 0000 0072 5300  ...rQ...rV...rS.
-000020d0: 0000 7217 0000 00da 115f 6164 645f 6368  ..r......_add_ch
-000020e0: 6169 6e5f 6272 6561 6b73 b600 0000 7344  ain_breaks....sD
-000020f0: 0000 0000 0f0e 010e 030e 0212 040c 040a  ................
-00002100: 010a ff06 0316 060a 010a ff06 0308 010c  ................
-00002110: 030a fd06 0514 041c 0110 021e ff06 0210  ................
-00002120: 0202 0102 ff06 030a 021c 0316 010e 0116  ................
-00002130: 010e 020a 030a 027a 224d 6f64 656c 6c65  .......z"Modelle
-00002140: 725f 6d61 6e61 6765 722e 5f61 6464 5f63  r_manager._add_c
-00002150: 6861 696e 5f62 7265 616b 7363 0100 0000  hain_breaksc....
-00002160: 0000 0000 0000 0000 0a00 0000 0800 0000  ................
-00002170: 4300 0000 737e 0100 0064 0164 02a0 007c  C...s~...d.d...|
-00002180: 006a 01a1 0117 0064 0317 007d 0174 027c  .j.....d...}.t.|
-00002190: 006a 036a 047c 0183 027d 0267 007d 0374  .j.j.|...}.g.}.t
-000021a0: 0583 008f 487d 0474 027c 006a 036a 0464  ....H}.t.|.j.j.d
-000021b0: 0483 027d 057c 04a0 067c 05a1 017d 067c  ...}.|...|...}.|
-000021c0: 06a0 0764 05a1 0164 0664 0085 0219 007d  ...d...d.d.....}
-000021d0: 0764 0764 0884 007c 0744 0083 017d 0357  .d.d...|.D...}.W
-000021e0: 0064 0004 0004 0083 0301 006e 1031 0073  .d.........n.1.s
-000021f0: 7a30 0001 0001 0001 0059 0001 007c 00a0  z0.......Y...|..
-00002200: 087c 006a 017c 0364 0919 0064 0619 00a1  .|.j.|.d...d....
-00002210: 027c 0364 0919 0064 063c 007c 00a0 097c  .|.d...d.<.|...|
-00002220: 03a1 017d 0364 027d 087c 0864 0a7c 006a  ...}.d.}.|.d.|.j
-00002230: 036a 0a17 0064 0b17 0037 007d 087c 0864  .j...d...7.}.|.d
-00002240: 0c7c 006a 036a 0a17 0064 0d17 0037 007d  .|.j.j...d...7.}
-00002250: 087c 087c 0364 0919 0064 0619 0064 0e17  .|.|.d...d...d..
-00002260: 0037 007d 087c 0364 0664 0085 0219 0044  .7.}.|.d.d.....D
-00002270: 005d 447d 097c 0864 0a7c 0964 0919 0017  .]D}.|.d.|.d....
-00002280: 0064 0f17 0064 0b17 0037 007d 087c 0864  .d...d...7.}.|.d
-00002290: 107c 0964 0919 0017 0064 0f17 0064 0d17  .|.d.....d...d..
-000022a0: 0037 007d 087c 087c 0964 0619 0064 0e17  .7.}.|.|.d...d..
-000022b0: 0037 007d 0871 f87c 006a 0b90 0172 7a74  .7.}.q.|.j...rzt
-000022c0: 0583 008f 1c7d 047c 04a0 0c7c 027c 08a1  .....}.|...|.|..
-000022d0: 0201 0057 0064 0004 0004 0083 0301 006e  ...W.d.........n
-000022e0: 1231 0090 0173 7030 0001 0001 0001 0059  .1...sp0.......Y
-000022f0: 0001 0064 0053 0029 114e 5a0f 6d6f 6465  ...d.S.).NZ.mode
-00002300: 6c6c 6572 5f69 6e70 7574 5f72 0b00 0000  ller_input_r....
-00002310: 722c 0000 007a 1774 656d 706c 6174 6573  r,...z.templates
-00002320: 5f61 6c69 676e 6564 2e66 6173 7461 fa01  _aligned.fasta..
-00002330: 3e72 0300 0000 6301 0000 0000 0000 0000  >r....c.........
-00002340: 0000 0002 0000 0008 0000 0053 0000 0073  ...........S...s
-00002350: 3a00 0000 6700 7c00 5d32 7d01 7c01 a000  :...g.|.]2}.|...
-00002360: 6400 a101 6401 1900 a000 a100 6402 1900  d...d.......d...
-00002370: 6403 a001 7c01 a000 6400 a101 6404 6405  d...|...d...d.d.
-00002380: 8502 1900 a101 6702 9102 7104 5300 2906  ......g...q.S.).
-00002390: da01 0a72 0100 0000 7259 0000 0072 0b00  ...r....rY...r..
-000023a0: 0000 7203 0000 004e 2902 da05 7370 6c69  ..r....N)...spli
-000023b0: 7472 1300 0000 2902 7223 0000 00da 0178  tr....).r#.....x
-000023c0: 7216 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
-000023d0: 2500 0000 0d01 0000 7226 0000 007a 344d  %.......r&...z4M
-000023e0: 6f64 656c 6c65 725f 6d61 6e61 6765 722e  odeller_manager.
-000023f0: 7772 6974 655f 616c 6967 6e6d 656e 742e  write_alignment.
-00002400: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
-00002410: 6d70 3e72 0100 0000 7a04 3e50 313b 7262  mp>r....z.>P1;rb
-00002420: 0000 007a 0973 6571 7565 6e63 653a 7a0d  ...z.sequence:z.
-00002430: 3a2e 3a2e 3a2e 3a2e 3a3a 3a3a 0a7a 022a  :.:.:.:.::::.z.*
-00002440: 0a72 3000 0000 7a0b 7374 7275 6374 7572  .r0...z.structur
-00002450: 6558 3a29 0d72 1300 0000 7206 0000 0072  eX:).r....r....r
-00002460: 0200 0000 720d 0000 0072 3700 0000 7204  ....r....r7...r.
-00002470: 0000 00da 0972 6561 645f 6669 6c65 7263  .....read_filerc
-00002480: 0000 0072 4500 0000 7260 0000 0072 1b00  ...rE...r`...r..
-00002490: 0000 7212 0000 0072 3b00 0000 290a 7215  ..r....r;...).r.
-000024a0: 0000 0072 3c00 0000 da0b 6f75 7470 7574  ...r<.....output
-000024b0: 5f70 6174 6872 4a00 0000 723f 0000 00da  _pathrJ...r?....
-000024c0: 0966 696c 655f 7061 7468 5a15 616c 6967  .file_pathZ.alig
-000024d0: 6e65 645f 7365 7175 656e 6365 5f66 696c  ned_sequence_fil
-000024e0: 655a 1161 6c69 676e 6564 5f73 6571 7565  eZ.aligned_seque
-000024f0: 6e63 6573 723e 0000 00da 1174 656d 706c  ncesr>.....templ
-00002500: 6174 655f 7365 7175 656e 6365 7216 0000  ate_sequencer...
-00002510: 0072 1600 0000 7217 0000 0072 1d00 0000  .r....r....r....
-00002520: 0301 0000 733a 0000 0000 0214 010e 0204  ....s:..........
-00002530: 0108 010e 010a 0112 012c 031e 030a 0404  .........,......
-00002540: 0114 0114 0114 0310 0118 0102 0102 0106  ................
-00002550: ff02 0202 fe02 0302 fd02 ff04 0612 0508  ................
-00002560: 0108 017a 204d 6f64 656c 6c65 725f 6d61  ...z Modeller_ma
-00002570: 6e61 6765 722e 7772 6974 655f 616c 6967  nager.write_alig
-00002580: 6e6d 656e 7463 0100 0000 0000 0000 0000  nmentc..........
-00002590: 0000 0600 0000 0800 0000 4300 0000 7302  ..........C...s.
-000025a0: 0100 007c 006a 0064 016b 0272 4674 0164  ...|.j.d.k.rFt.d
-000025b0: 0264 03a0 027c 006a 03a1 0117 0064 0417  .d...|.j.....d..
-000025c0: 007c 006a 046a 0517 0064 0517 007c 006a  .|.j.j...d...|.j
-000025d0: 046a 0617 0064 0617 0083 0101 007c 00a0  .j...d.......|..
-000025e0: 07a1 0001 0064 0053 0074 087c 006a 046a  .....d.S.t.|.j.j
-000025f0: 097c 006a 046a 0564 0717 0064 03a0 027c  .|.j.j.d...d...|
-00002600: 006a 03a1 0117 0064 0817 0083 027d 0174  .j.....d.....}.t
-00002610: 0a83 008f 1a7d 027c 02a0 0b7c 01a1 0101  .....}.|...|....
-00002620: 0057 0064 0004 0004 0083 0301 006e 1031  .W.d.........n.1
-00002630: 0073 9230 0001 0001 0001 0059 0001 0074  .s.0.......Y...t
-00002640: 0ca0 0da1 007d 0374 0ca0 0e74 0f7c 0183  .....}.t...t.|..
-00002650: 01a1 0101 0064 0964 03a0 027c 006a 03a1  .....d.d...|.j..
-00002660: 0117 0064 0a17 007d 047c 006a 109b 0064  ...d...}.|.j...d
-00002670: 0574 0f7c 0483 019b 009d 037d 0574 116a  .t.|.......}.t.j
-00002680: 127c 0564 0b64 0b64 0b64 0c8d 0401 0074  .|.d.d.d.d.....t
-00002690: 0ca0 0e7c 03a1 0101 007c 00a0 07a1 0001  ...|.....|......
-000026a0: 0064 0053 0029 0d4e 467a 164d 6f64 656c  .d.S.).NFz.Model
-000026b0: 6c69 6e67 206f 6620 6d75 7461 7469 6f6e  ling of mutation
-000026c0: 2072 0b00 0000 7a12 2077 6173 2065 6578   r....z. was eex
-000026d0: 636c 7564 6564 206f 6e20 7219 0000 007a  cluded on r....z
-000026e0: 1920 6475 6520 746f 206d 6973 7369 6e67  . due to missing
-000026f0: 2063 6f76 6572 6167 652e 722f 0000 005a   coverage.r/...Z
-00002700: 065f 6d6f 6465 6c7a 102e 2e2f 7275 6e5f  ._modelz.../run_
-00002710: 6d6f 6465 6c6c 6572 5f72 2e00 0000 5429  modeller_r....T)
-00002720: 03da 0573 6865 6c6c da12 756e 6976 6572  ...shell..univer
-00002730: 7361 6c5f 6e65 776c 696e 6573 da05 6368  sal_newlines..ch
-00002740: 6563 6b29 1372 1200 0000 721a 0000 0072  eck).r....r....r
-00002750: 1300 0000 7206 0000 0072 0d00 0000 721b  ....r....r....r.
-00002760: 0000 0072 1c00 0000 da0d 6c6f 6164 5f6c  ...r......load_l
-00002770: 6f67 5f66 696c 6572 0200 0000 7237 0000  og_filer....r7..
-00002780: 0072 0400 0000 da10 6372 6561 7465 5f64  .r......create_d
-00002790: 6972 6563 746f 7279 da02 6f73 da06 6765  irectory..os..ge
-000027a0: 7463 7764 da05 6368 6469 7272 3900 0000  tcwd..chdirr9...
-000027b0: 7207 0000 00da 0a73 7562 7072 6f63 6573  r......subproces
-000027c0: 73da 0372 756e 2906 7215 0000 005a 0a6d  s..run).r....Z.m
-000027d0: 6f64 656c 5f70 6174 6872 3f00 0000 5a16  odel_pathr?...Z.
-000027e0: 686f 6d65 5f77 6f72 6b69 6e67 5f64 6972  home_working_dir
-000027f0: 6563 746f 7279 723d 0000 00da 0763 6f6d  ectoryr=.....com
-00002800: 6d61 6e64 7216 0000 0072 1600 0000 7217  mandr....r....r.
-00002810: 0000 0072 7200 0000 2e01 0000 733a 0000  ...rr.......s:..
-00002820: 0000 020a 0110 0102 ff02 0106 ff02 0102  ................
-00002830: ff02 0206 fe02 0202 fe06 0308 0104 0202  ................
-00002840: 0106 011a fe04 0408 0128 0108 010e 0114  .........(......
-00002850: 0114 0104 0108 ff06 030a 017a 144d 6f64  ...........z.Mod
-00002860: 656c 6c65 725f 6d61 6e61 6765 722e 7275  eller_manager.ru
-00002870: 6e63 0100 0000 0000 0000 0000 0000 0600  nc..............
-00002880: 0000 0800 0000 4300 0000 7394 0000 007c  ......C...s....|
-00002890: 006a 0072 8874 0183 008f 6a7d 0174 027c  .j.r.t....j}.t.|
-000028a0: 006a 036a 0464 0164 02a0 057c 006a 06a1  .j.j.d.d...|.j..
-000028b0: 0117 0064 0317 0083 027d 027c 01a0 077c  ...d.....}.|...|
-000028c0: 02a1 01a0 08a1 007d 037c 03a0 0964 04a1  .......}.|...d..
-000028d0: 017d 047c 047c 037c 0464 0585 0219 00a0  .}.|.|.|.d......
-000028e0: 0964 02a1 0117 007d 057c 037c 047c 0585  .d.....}.|.|.|..
-000028f0: 0219 007c 005f 0a57 0064 0504 0004 0083  ...|._.W.d......
-00002900: 0301 0071 9031 0073 7c30 0001 0001 0001  ...q.1.s|0......
-00002910: 0059 0001 006e 0864 0667 017c 005f 0a64  .Y...n.d.g.|._.d
-00002920: 0553 0029 0761 1801 0000 204f 7065 6e20  .S.).a.... Open 
-00002930: 7468 6520 6c6f 6720 6669 6c65 2061 6674  the log file aft
-00002940: 6572 2074 6865 2072 756e 206f 6620 6d6f  er the run of mo
-00002950: 6465 6c6c 6572 2e0a 2020 2020 2020 2020  deller..        
-00002960: 4c6f 6f6b 2066 6f72 2074 6865 2074 6162  Look for the tab
-00002970: 6c65 2077 6974 6820 7468 6520 444f 5045  le with the DOPE
-00002980: 2073 636f 7265 732e 0a20 2020 2020 2020   scores..       
-00002990: 2053 6176 6520 6974 2061 7320 6174 7472   Save it as attr
-000029a0: 6962 7574 6520 286c 6973 7429 2e0a 2020  ibute (list)..  
-000029b0: 2020 2020 2020 0a20 2020 2020 2020 2042        .        B
-000029c0: 7574 2069 6620 7468 6520 6d75 7461 7469  ut if the mutati
-000029d0: 6f6e 2069 7320 6e6f 7420 6d6f 6465 6c6c  on is not modell
-000029e0: 6162 6c65 2c20 6475 6520 746f 206d 6973  able, due to mis
-000029f0: 7369 6e67 2074 656d 706c 6174 650a 2020  sing template.  
-00002a00: 2020 2020 2020 636f 6e76 6572 6167 652c        converage,
-00002a10: 206a 7573 7420 7361 7665 2061 2077 6172   just save a war
-00002a20: 6e69 6e67 2073 7472 696e 6720 6173 2061  ning string as a
-00002a30: 7474 7269 6275 7465 2e0a 2020 2020 2020  ttribute..      
-00002a40: 2020 722d 0000 0072 0b00 0000 7a04 2e6c    r-...r....z..l
-00002a50: 6f67 7a46 4669 6c65 6e61 6d65 2020 2020  ogzFFilename    
-00002a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a70: 2020 2020 2020 6d6f 6c70 6466 2020 2020        molpdf    
-00002a80: 2044 4f50 4520 7363 6f72 6520 2020 2047   DOPE score    G
-00002a90: 4133 3431 2073 636f 7265 4e7a 4a21 2054  A341 scoreNzJ! T
-00002aa0: 6865 206d 7574 6174 696f 6e20 7761 7320  he mutation was 
-00002ab0: 6e6f 7420 6d6f 6465 6c6c 6564 2c20 6475  not modelled, du
-00002ac0: 6520 746f 206d 6973 7369 6e67 2074 656d  e to missing tem
-00002ad0: 706c 6174 6573 2066 6f72 2074 6861 7420  plates for that 
-00002ae0: 7265 6769 6f6e 2e29 0b72 1200 0000 7204  region.).r....r.
-00002af0: 0000 0072 0200 0000 720d 0000 0072 3700  ...r....r....r7.
-00002b00: 0000 7213 0000 0072 0600 0000 7265 0000  ..r....r....re..
-00002b10: 00da 0a73 706c 6974 6c69 6e65 73da 0569  ...splitlines..i
-00002b20: 6e64 6578 720f 0000 0029 0672 1500 0000  ndexr....).r....
-00002b30: 723f 0000 005a 086c 6f67 5f70 6174 685a  r?...Z.log_pathZ
-00002b40: 046c 6f67 735a 1174 6162 6c65 5f73 7461  .logsZ.table_sta
-00002b50: 7274 5f69 6e64 6578 5a0f 7461 626c 655f  rt_indexZ.table_
-00002b60: 656e 645f 696e 6465 7872 1600 0000 7216  end_indexr....r.
-00002b70: 0000 0072 1700 0000 726c 0000 0047 0100  ...r....rl...G..
-00002b80: 0073 1000 0000 0008 0601 0801 1e01 0e02  .s..............
-00002b90: 0a01 1602 2e02 7a1e 4d6f 6465 6c6c 6572  ......z.Modeller
-00002ba0: 5f6d 616e 6167 6572 2e6c 6f61 645f 6c6f  _manager.load_lo
-00002bb0: 675f 6669 6c65 2912 da08 5f5f 6e61 6d65  g_file)...__name
-00002bc0: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
-00002bd0: 5f5f 7175 616c 6e61 6d65 5f5f da04 6c69  __qualname__..li
-00002be0: 7374 7239 0000 0072 2700 0000 7218 0000  str9...r'...r...
-00002bf0: 0072 1f00 0000 da04 626f 6f6c 722b 0000  .r......boolr+..
-00002c00: 0072 1e00 0000 7245 0000 0072 4700 0000  .r....rE...rG...
-00002c10: 7249 0000 0072 6000 0000 721d 0000 0072  rI...r`...r....r
-00002c20: 7200 0000 726c 0000 0072 1600 0000 7216  r...rl...r....r.
-00002c30: 0000 0072 1600 0000 7217 0000 0072 0500  ...r....r....r..
-00002c40: 0000 0800 0000 731a 0000 0008 0106 0104  ......s.........
-00002c50: ff0c 1008 090e 1c08 3f10 1e10 0c10 0f10  ........?.......
-00002c60: 4d08 2b0e 1972 0500 0000 2907 726e 0000  M.+..r....).rn..
-00002c70: 0072 7100 0000 da07 7061 7468 6c69 6272  .rq.....pathlibr
-00002c80: 0200 0000 da0c 6669 6c65 5f68 616e 646c  ......file_handl
-00002c90: 6572 7204 0000 0072 0500 0000 7216 0000  err....r....r...
-00002ca0: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
-00002cb0: da08 3c6d 6f64 756c 653e 0100 0000 7308  ..<module>....s.
-00002cc0: 0000 0008 0108 010c 020c 03              ...........
+00000eb0: 6c73 290a 6d6f 6465 6c73 2e73 6f72 7428  ls).models.sort(
+00000ec0: 6c61 6d62 6461 206b 3a20 6b5b 746f 7363  lambda k: k[tosc
+00000ed0: 6f72 655d 290a 0a6d 796f 7574 203d 206f  ore])..myout = o
+00000ee0: 7065 6e28 2261 3401 0000 222c 2022 7722  pen("a4...", "w"
+00000ef0: 290a 666f 7220 6d20 696e 206d 6f64 656c  ).for m in model
+00000f00: 733a 0a20 2020 2020 2020 206d 796f 7574  s:.        myout
+00000f10: 2e77 7269 7465 2873 7472 286d 5b27 6e61  .write(str(m['na
+00000f20: 6d65 275d 2920 2b20 2220 2844 4f50 4520  me']) + " (DOPE 
+00000f30: 5343 4f52 453a 2025 2e33 6629 2220 2520  SCORE: %.3f)" % 
+00000f40: 286d 5b74 6f73 636f 7265 5d29 290a 656e  (m[toscore])).en
+00000f50: 762e 6c69 6273 2e74 6f70 6f6c 6f67 792e  v.libs.topology.
+00000f60: 7265 6164 2866 696c 653d 2724 284c 4942  read(file='$(LIB
+00000f70: 292f 746f 705f 6865 6176 2e6c 6962 2729  )/top_heav.lib')
+00000f80: 0a65 6e76 2e6c 6962 732e 7061 7261 6d65  .env.libs.parame
+00000f90: 7465 7273 2e72 6561 6428 6669 6c65 3d27  ters.read(file='
+00000fa0: 2428 4c49 4229 2f70 6172 2e6c 6962 2729  $(LIB)/par.lib')
+00000fb0: 0a6d 646c 203d 2063 6f6d 706c 6574 655f  .mdl = complete_
+00000fc0: 7064 6228 656e 762c 206d 5b27 6e61 6d65  pdb(env, m['name
+00000fd0: 275d 290a 7320 3d20 7365 6c65 6374 696f  ']).s = selectio
+00000fe0: 6e28 6d64 6c29 0a73 2e61 7373 6573 735f  n(mdl).s.assess_
+00000ff0: 646f 7065 286f 7574 7075 743d 2745 4e45  dope(output='ENE
+00001000: 5247 595f 5052 4f46 494c 4520 4e4f 5f52  RGY_PROFILE NO_R
+00001010: 4550 4f52 5427 2c20 6669 6c65 3d22 7a2f  EPORT', file="z/
+00001020: 222c 206e 6f72 6d61 6c69 7a65 5f70 726f  ", normalize_pro
+00001030: 6669 6c65 3d54 7275 652c 2073 6d6f 6f74  file=True, smoot
+00001040: 6869 6e67 5f77 696e 646f 773d 3135 2929  hing_window=15))
+00001050: 0e72 1300 0000 7206 0000 0072 0200 0000  .r....r....r....
+00001060: 720d 0000 00da 086f 7574 5f70 6174 68da  r......out_path.
+00001070: 0974 656d 706c 6174 6573 da03 7374 72da  .templates..str.
+00001080: 0572 616e 6765 7210 0000 0072 1100 0000  .ranger....r....
+00001090: 721b 0000 0072 1400 0000 7204 0000 00da  r....r....r.....
+000010a0: 0a77 7269 7465 5f66 696c 6529 0772 1500  .write_file).r..
+000010b0: 0000 da0e 616c 6967 6e6d 656e 745f 6e61  ....alignment_na
+000010c0: 6d65 5a0b 6f75 7470 7574 5f6e 616d 65da  meZ.output_name.
+000010d0: 0b73 6372 6970 745f 7061 7468 5a0e 7465  .script_pathZ.te
+000010e0: 6d70 6c61 7465 5f6e 616d 6573 da07 636f  mplate_names..co
+000010f0: 6e74 656e 74da 0266 6872 1600 0000 7216  ntent..fhr....r.
+00001100: 0000 0072 1700 0000 721e 0000 003e 0000  ...r....r....>..
+00001110: 0073 5a00 0000 0001 1401 1401 0201 0601  .sZ.............
+00001120: 12fe 0404 0602 06fe 0605 0207 16f9 0207  ................
+00001130: 02f9 0208 08f8 0208 02f8 0210 02f0 0211  ................
+00001140: 02ef 0213 06ed 0214 02ec 0216 06ea 0217  ................
+00001150: 02e9 021a 08e6 021a 02e6 0223 02dd 0224  ...........#...$
+00001160: 02dc 022c 06d4 022d 02d3 02ff 0231 0801  ...,...-.....1..
+00001170: 7a1d 4d6f 6465 6c6c 6572 5f6d 616e 6167  z.Modeller_manag
+00001180: 6572 2e77 7269 7465 5f73 6372 6970 7429  er.write_script)
+00001190: 0272 2a00 0000 7220 0000 0063 0300 0000  .r*...r ...c....
+000011a0: 0000 0000 0000 0000 0500 0000 0400 0000  ................
+000011b0: 4300 0000 73a8 0000 007c 0164 016b 0272  C...s....|.d.k.r
+000011c0: 0c7c 0253 0074 007c 0164 0219 0083 0164  .|.S.t.|.d.....d
+000011d0: 0218 007d 037c 0374 017c 0283 016b 0072  ...}.|.t.|...k.r
+000011e0: 947c 037c 0264 037c 0385 0219 00a0 0264  .|.|.d.|.......d
+000011f0: 04a1 0118 007d 047c 0464 0217 0074 007c  .....}.|.d...t.|
+00001200: 0164 0219 0083 016b 0272 8a7c 027c 0319  .d.....k.r.|.|..
+00001210: 007c 0164 0519 006b 0272 8a7c 0264 037c  .|.d...k.r.|.d.|
+00001220: 0385 0219 007c 0164 0619 0017 007c 027c  .....|.d.....|.|
+00001230: 0364 0217 0064 0385 0219 0017 007d 027c  .d...d.......}.|
+00001240: 0253 007c 0364 0237 007d 0371 1c74 0364  .S.|.d.7.}.q.t.d
+00001250: 077c 019b 0064 089d 0383 0101 007c 0253  .|...d.......|.S
+00001260: 0029 097a ea54 616b 6520 6120 6d75 7461  .).z.Take a muta
+00001270: 7469 6f6e 2069 6e20 7468 6520 666f 726d  tion in the form
+00001280: 6174 0a20 2020 2020 2020 205b 3120 6c65  at.        [1 le
+00001290: 7474 6572 2061 6d69 6e6f 2061 6369 642c  tter amino acid,
+000012a0: 7265 7369 6475 6520 6e75 6d62 6572 2c20  residue number, 
+000012b0: 3120 6c65 7474 2e20 616d 696e 6f20 6163  1 lett. amino ac
+000012c0: 6964 5d0a 2020 2020 2020 2020 616e 6420  id].        and 
+000012d0: 6170 706c 7920 6974 2074 6f20 7468 6520  apply it to the 
+000012e0: 616c 6967 6e65 6420 7365 7175 656e 6365  aligned sequence
+000012f0: 2074 6f20 6d6f 6465 6c2c 0a20 2020 2020   to model,.     
+00001300: 2020 2074 616b 696e 6720 696e 746f 2061     taking into a
+00001310: 6363 6f75 6e74 2061 6c6c 2074 6865 2022  ccount all the "
+00001320: 2d22 2773 2e0a 0a20 2020 2020 2020 2052  -"'s...        R
+00001330: 6574 7572 6e73 2065 6469 7465 6420 7365  eturns edited se
+00001340: 7175 656e 6365 0a20 2020 2020 2020 2072  quence.        r
+00001350: 0c00 0000 7203 0000 004e fa01 2d72 0100  ....r....N..-r..
+00001360: 0000 e902 0000 007a 1943 6f75 6c64 206e  .......z.Could n
+00001370: 6f74 2061 7070 6c79 206d 7574 6174 696f  ot apply mutatio
+00001380: 6e20 fa01 2129 0472 2700 0000 da03 6c65  n ..!).r'.....le
+00001390: 6eda 0563 6f75 6e74 721a 0000 0029 0572  n..countr....).r
+000013a0: 1500 0000 7206 0000 0072 2a00 0000 7236  ....r....r*...r6
+000013b0: 0000 005a 1461 6374 7561 6c5f 7265 7369  ...Z.actual_resi
+000013c0: 6475 655f 696e 6465 7872 1600 0000 7216  due_indexr....r.
+000013d0: 0000 0072 1700 0000 da0f 5f6d 7574 6174  ...r......_mutat
+000013e0: 655f 7265 7369 6475 657d 0000 0073 2600  e_residue}...s&.
+000013f0: 0000 0009 0801 0403 1001 0c01 1602 12ff  ................
+00001400: 0202 0efe 0204 0a01 06ff 0202 0efe 02ff  ................
+00001410: 0205 0401 0a02 1001 7a20 4d6f 6465 6c6c  ........z Modell
+00001420: 6572 5f6d 616e 6167 6572 2e5f 6d75 7461  er_manager._muta
+00001430: 7465 5f72 6573 6964 7565 6302 0000 0000  te_residuec.....
+00001440: 0000 0000 0000 0005 0000 0005 0000 0043  ...............C
+00001450: 0000 0073 4400 0000 6700 7d02 6401 7d03  ...sD...g.}.d.}.
+00001460: 7c01 4400 5d32 7d04 7c04 6402 6b02 7228  |.D.]2}.|.d.k.r(
+00001470: 7c02 a000 6402 7c04 6702 a101 0100 710c  |...d.|.g.....q.
+00001480: 7c02 a000 7c03 7c04 6702 a101 0100 7c03  |...|.|.g.....|.
+00001490: 6401 3700 7d03 710c 7c02 5300 2903 7a37  d.7.}.q.|.S.).z7
+000014a0: 4672 6f6d 2061 2073 6571 7565 6e63 652c  From a sequence,
+000014b0: 2072 6574 7572 6e20 6120 3244 206c 6973   return a 2D lis
+000014c0: 7420 7769 7468 205b 7265 736e 756d 2c72  t with [resnum,r
+000014d0: 6573 6964 7565 5d72 0300 0000 7240 0000  esidue]r....r@..
+000014e0: 0029 0172 2900 0000 2905 7215 0000 0072  .).r)...).r....r
+000014f0: 2a00 0000 5a0c 6e75 6d62 6572 6564 5f73  *...Z.numbered_s
+00001500: 6571 7236 0000 00da 0463 6861 7272 1600  eqr6.....charr..
+00001510: 0000 7216 0000 0072 1700 0000 da17 5f61  ..r....r......_a
+00001520: 6464 5f6e 756d 6265 725f 746f 5f73 6571  dd_number_to_seq
+00001530: 7565 6e63 659b 0000 0073 1000 0000 0002  uence....s......
+00001540: 0401 0401 0801 0801 1002 0e01 0a01 7a28  ..............z(
+00001550: 4d6f 6465 6c6c 6572 5f6d 616e 6167 6572  Modeller_manager
+00001560: 2e5f 6164 645f 6e75 6d62 6572 5f74 6f5f  ._add_number_to_
+00001570: 7365 7175 656e 6365 4e29 02da 1473 6571  sequenceN)...seq
+00001580: 7565 6e63 655f 7769 7468 5f72 6573 6e75  uence_with_resnu
+00001590: 6d72 2000 0000 6302 0000 0000 0000 0000  mr ...c.........
+000015a0: 0000 0004 0000 0005 0000 0043 0000 0073  ...........C...s
+000015b0: 6200 0000 6401 6402 8400 7c01 4400 8301  b...d.d...|.D...
+000015c0: 7d02 7c00 6a00 a001 7c02 6403 1900 a101  }.|.j...|.d.....
+000015d0: 0100 7402 6404 7403 7c02 8301 8302 4400  ..t.d.t.|.....D.
+000015e0: 5d30 7d03 7c02 7c03 1900 7c02 7c03 6404  ]0}.|.|...|.|.d.
+000015f0: 1800 1900 6404 1700 6b03 722c 7c00 6a00  ....d...k.r,|.j.
+00001600: a001 7c02 7c03 1900 6404 1700 a101 0100  ..|.|...d.......
+00001610: 712c 6405 5300 2906 7aa7 4769 7665 6e20  q,d.S.).z.Given 
+00001620: 6120 7365 7175 656e 6365 2073 6176 6564  a sequence saved
+00001630: 2061 7320 6120 6c69 7374 205b 7265 736e   as a list [resn
+00001640: 756d 2c20 7265 7369 6475 655d 2c0a 2020  um, residue],.  
+00001650: 2020 2020 2020 7361 7665 2061 6c6c 2074        save all t
+00001660: 6865 2072 6573 6964 7565 206e 756d 6265  he residue numbe
+00001670: 7273 2074 6861 7420 7265 7072 6573 656e  rs that represen
+00001680: 7420 616e 2069 6e74 6572 7275 7074 696f  t an interruptio
+00001690: 6e0a 2020 2020 2020 2020 696e 2074 6865  n.        in the
+000016a0: 2063 6f6e 7469 6e75 6974 7920 6f66 2074   continuity of t
+000016b0: 6865 2070 726f 7465 696e 2063 6861 696e  he protein chain
+000016c0: 2e63 0100 0000 0000 0000 0000 0000 0200  .c..............
+000016d0: 0000 0400 0000 5300 0000 7320 0000 0067  ......S...s ...g
+000016e0: 007c 005d 187d 017c 0164 0019 0064 016b  .|.].}.|.d...d.k
+000016f0: 0372 047c 0164 0019 0091 0271 0453 0029  .r.|.d.....q.S.)
+00001700: 0272 0100 0000 7240 0000 0072 1600 0000  .r....r@...r....
+00001710: 7222 0000 0072 1600 0000 7216 0000 0072  r"...r....r....r
+00001720: 1700 0000 7225 0000 00ad 0000 0072 2600  ....r%.......r&.
+00001730: 0000 7a37 4d6f 6465 6c6c 6572 5f6d 616e  ..z7Modeller_man
+00001740: 6167 6572 2e5f 7361 7665 5f63 6861 696e  ager._save_chain
+00001750: 5f73 7461 7274 732e 3c6c 6f63 616c 733e  _starts.<locals>
+00001760: 2e3c 6c69 7374 636f 6d70 3e72 0100 0000  .<listcomp>r....
+00001770: 7203 0000 004e 2904 7211 0000 0072 2900  r....N).r....r).
+00001780: 0000 723a 0000 0072 4300 0000 2904 7215  ..r:...rC...).r.
+00001790: 0000 0072 4800 0000 5a10 6669 6c74 6572  ...rH...Z.filter
+000017a0: 6564 5f6e 756d 6265 7273 7236 0000 0072  ed_numbersr6...r
+000017b0: 1600 0000 7216 0000 0072 1700 0000 da12  ....r....r......
+000017c0: 5f73 6176 655f 6368 6169 6e5f 7374 6172  _save_chain_star
+000017d0: 7473 a700 0000 730a 0000 0000 060e 0310  ts....s.........
+000017e0: 0212 0118 017a 234d 6f64 656c 6c65 725f  .....z#Modeller_
+000017f0: 6d61 6e61 6765 722e 5f73 6176 655f 6368  manager._save_ch
+00001800: 6169 6e5f 7374 6172 7473 2902 da09 7365  ain_starts)...se
+00001810: 7175 656e 6365 7372 2000 0000 6302 0000  quencesr ...c...
+00001820: 0000 0000 0000 0000 0009 0000 0006 0000  ................
+00001830: 0003 0000 0073 be01 0000 6401 6402 8400  .....s....d.d...
+00001840: 7c01 4400 8301 8902 6403 6402 8400 7c01  |.D.....d.d...|.
+00001850: 4400 8301 8900 7c00 a000 8800 6404 1900  D.....|.....d...
+00001860: a101 7d02 7401 6405 6402 8400 8800 4400  ..}.t.d.d.....D.
+00001870: 8301 8301 8901 8801 7c00 6a02 6b05 9001  ........|.j.k...
+00001880: 7242 8701 6601 6406 6402 8408 8800 6407  rB..f.d.d.....d.
+00001890: 6408 8502 1900 4400 8301 7d03 7403 7c03  d.....D...}.t.|.
+000018a0: 8301 7404 8800 8301 6407 1800 6b02 9001  ..t.....d...k...
+000018b0: 7238 8701 6601 6409 6402 8408 8800 6407  r8..f.d.d.....d.
+000018c0: 6408 8502 1900 4400 8301 7d04 7c04 4400  d.....D...}.|.D.
+000018d0: 5da0 8903 8701 8703 6602 640a 6402 8408  ].......f.d.d...
+000018e0: 8800 6407 6408 8502 1900 4400 8301 7d05  ..d.d.....D...}.
+000018f0: 7403 7c05 8301 7404 8800 8301 6407 1800  t.|...t.....d...
+00001900: 6b02 7296 7c02 6408 8803 8502 1900 7c02  k.r.|.d.......|.
+00001910: 8803 8801 1700 6407 1800 6408 8502 1900  ......d...d.....
+00001920: 1700 7d02 7405 8800 8301 4400 5d3a 5c02  ..}.t.....D.]:\.
+00001930: 7d06 7d07 7c07 6408 8803 8502 1900 640b  }.}.|.d.......d.
+00001940: 1700 7c07 8803 8801 1700 6408 8502 1900  ..|.......d.....
+00001950: 1700 8800 7c06 3c00 7c00 0400 6a06 6407  ....|.<.|...j.d.
+00001960: 3700 0200 5f06 71f2 8801 6407 3700 8901  7..._.q...d.7...
+00001970: 7196 8801 6407 3800 8901 713c 8700 8702  q...d.8...q<....
+00001980: 6602 640c 6402 8408 7407 7404 8802 8301  f.d.d...t.t.....
+00001990: 8301 4400 8301 7d01 7c01 6404 1900 6407  ..D...}.|.d...d.
+000019a0: 1900 6404 1900 640b 6b02 9001 7282 640d  ..d...d.k...r.d.
+000019b0: 6402 8400 7c01 4400 8301 7d01 7c01 6404  d...|.D...}.|.d.
+000019c0: 1900 6407 1900 640e 1900 640b 6b02 9001  ..d...d...d.k...
+000019d0: 72a6 640f 6402 8400 7c01 4400 8301 7d01  r.d.d...|.D...}.
+000019e0: 7c00 a008 7c02 a101 0100 7c00 a009 7c02  |...|.....|...|.
+000019f0: a101 7d08 7c01 5300 2910 619f 0100 0046  ..}.|.S.).a....F
+00001a00: 6f72 2061 6c69 676e 6d65 6e74 7320 696e  or alignments in
+00001a10: 2077 6869 6368 2074 6865 7265 2069 7320   which there is 
+00001a20: 6e6f 2063 6f76 6572 6167 6520 666f 7220  no coverage for 
+00001a30: 7365 6c66 2e6d 6f64 656c 5f63 7574 6f66  self.model_cutof
+00001a40: 662b 0a20 2020 2020 2020 2072 6573 6964  f+.        resid
+00001a50: 7565 732c 2074 6865 2073 6563 7469 6f6e  ues, the section
+00001a60: 2077 6974 686f 7574 2063 6f76 6572 6167   without coverag
+00001a70: 6520 6973 2072 6570 6c61 6365 6420 6279  e is replaced by
+00001a80: 0a20 2020 2020 2020 2063 6861 696e 2062  .        chain b
+00001a90: 7265 616b 732e 0a0a 2020 2020 2020 2020  reaks...        
+00001aa0: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
+00001ab0: 2020 7365 7175 656e 6365 7320 286c 6973    sequences (lis
+00001ac0: 7429 3a20 4120 6c69 7374 206f 6620 5b6e  t): A list of [n
+00001ad0: 616d 652c 2073 6571 7565 6e63 655d 206c  ame, sequence] l
+00001ae0: 6973 7473 2c0a 2020 2020 2020 2020 2020  ists,.          
+00001af0: 2020 6f6e 6520 666f 7220 6561 6368 2073    one for each s
+00001b00: 6571 7565 6e63 6520 746f 2062 6520 7772  equence to be wr
+00001b10: 6974 7465 6e20 696e 2074 6865 206d 6f64  itten in the mod
+00001b20: 656c 6c65 720a 2020 2020 2020 2020 2020  eller.          
+00001b30: 2020 616c 6967 6e6d 656e 7420 696e 7075    alignment inpu
+00001b40: 7420 6669 6c65 2e0a 0a20 2020 2020 2020  t file...       
+00001b50: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
+00001b60: 2020 2020 2020 6c69 7374 3a20 5265 7475        list: Retu
+00001b70: 726e 7320 7468 6520 7361 6d65 206c 6973  rns the same lis
+00001b80: 742c 2077 6974 6820 6368 6169 6e20 6272  t, with chain br
+00001b90: 6561 6b73 2e0a 2020 2020 2020 2020 6301  eaks..        c.
+00001ba0: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+00001bb0: 0000 0053 0000 0073 1400 0000 6700 7c00  ...S...s....g.|.
+00001bc0: 5d0c 7d01 7c01 6400 1900 9102 7104 5300  ].}.|.d.....q.S.
+00001bd0: 7221 0000 0072 1600 0000 a902 7223 0000  r!...r......r#..
+00001be0: 00da 066f 626a 6563 7472 1600 0000 7216  ...objectr....r.
+00001bf0: 0000 0072 1700 0000 7225 0000 00c5 0000  ...r....r%......
+00001c00: 0072 2600 0000 7a36 4d6f 6465 6c6c 6572  .r&...z6Modeller
+00001c10: 5f6d 616e 6167 6572 2e5f 6164 645f 6368  _manager._add_ch
+00001c20: 6169 6e5f 6272 6561 6b73 2e3c 6c6f 6361  ain_breaks.<loca
+00001c30: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 6301  ls>.<listcomp>c.
+00001c40: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+00001c50: 0000 0053 0000 0073 1400 0000 6700 7c00  ...S...s....g.|.
+00001c60: 5d0c 7d01 7c01 6400 1900 9102 7104 5300  ].}.|.d.....q.S.
+00001c70: 2901 7203 0000 0072 1600 0000 724b 0000  ).r....r....rK..
+00001c80: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
+00001c90: 7225 0000 00c6 0000 0072 2600 0000 7201  r%.......r&...r.
+00001ca0: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+00001cb0: 0200 0000 0500 0000 5300 0000 7316 0000  ........S...s...
+00001cc0: 0067 007c 005d 0e7d 017c 01a0 0064 00a1  .g.|.].}.|...d..
+00001cd0: 0191 0271 0453 00a9 0172 4000 0000 2901  ...q.S...r@...).
+00001ce0: 7244 0000 00a9 0272 2300 0000 da03 7365  rD.....r#.....se
+00001cf0: 7172 1600 0000 7216 0000 0072 1700 0000  qr....r....r....
+00001d00: 7225 0000 00cb 0000 0072 2600 0000 6301  r%.......r&...c.
+00001d10: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+00001d20: 0000 0013 0000 0073 1800 0000 6700 7c00  .......s....g.|.
+00001d30: 5d10 7d01 6400 8800 1400 7c01 7600 9102  ].}.d.....|.v...
+00001d40: 7104 5300 724d 0000 0072 1600 0000 724e  q.S.rM...r....rN
+00001d50: 0000 00a9 01da 0f6d 6178 5f6e 6f6e 5f63  .......max_non_c
+00001d60: 6f76 6572 6564 7216 0000 0072 1700 0000  overedr....r....
+00001d70: 7225 0000 00d3 0000 0073 0200 0000 0601  r%.......s......
+00001d80: 7203 0000 004e 6301 0000 0000 0000 0000  r....Nc.........
+00001d90: 0000 0002 0000 0006 0000 0013 0000 0073  ...............s
+00001da0: 1a00 0000 6700 7c00 5d12 7d01 7c01 a000  ....g.|.].}.|...
+00001db0: 6400 8800 1400 a101 9102 7104 5300 724d  d.........q.S.rM
+00001dc0: 0000 0029 01da 0466 696e 6472 4e00 0000  ...)...findrN...
+00001dd0: 7250 0000 0072 1600 0000 7217 0000 0072  rP...r....r....r
+00001de0: 2500 0000 dc00 0000 7302 0000 0006 0163  %.......s......c
+00001df0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00001e00: 0600 0000 1300 0000 7324 0000 0067 007c  ........s$...g.|
+00001e10: 005d 1c7d 017c 0188 0188 0188 0017 0085  .].}.|..........
+00001e20: 0219 0064 0088 0014 006b 0291 0271 0453  ...d.....k...q.S
+00001e30: 0072 4d00 0000 7216 0000 0072 4e00 0000  .rM...r....rN...
+00001e40: 2902 7251 0000 00da 0370 6f73 7216 0000  ).rQ.....posr...
+00001e50: 0072 1700 0000 7225 0000 00e0 0000 0073  .r....r%.......s
+00001e60: 0800 0000 0603 02fe 0e01 06ff fa01 2f63  ............../c
+00001e70: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00001e80: 0500 0000 1300 0000 731c 0000 0067 007c  ........s....g.|
+00001e90: 005d 147d 0188 017c 0119 0088 007c 0119  .].}...|.....|..
+00001ea0: 0067 0291 0271 0453 0072 1600 0000 7216  .g...q.S.r....r.
+00001eb0: 0000 0072 3500 0000 2902 da0b 616c 6967  ...r5...)...alig
+00001ec0: 6e65 645f 7365 71da 056e 616d 6573 7216  ned_seq..namesr.
+00001ed0: 0000 0072 1700 0000 7225 0000 00f4 0000  ...r....r%......
+00001ee0: 0072 2600 0000 6301 0000 0000 0000 0000  .r&...c.........
+00001ef0: 0000 0002 0000 0006 0000 0053 0000 0073  ...........S...s
+00001f00: 2400 0000 6700 7c00 5d1c 7d01 7c01 6400  $...g.|.].}.|.d.
+00001f10: 1900 7c01 6401 1900 6401 6402 8502 1900  ..|.d...d.d.....
+00001f20: 6702 9102 7104 5300 2903 7201 0000 0072  g...q.S.).r....r
+00001f30: 0300 0000 4e72 1600 0000 a902 7223 0000  ....Nr......r#..
+00001f40: 00da 0173 7216 0000 0072 1600 0000 7217  ...sr....r....r.
+00001f50: 0000 0072 2500 0000 f800 0000 7226 0000  ...r%.......r&..
+00001f60: 00e9 ffff ffff 6301 0000 0000 0000 0000  ......c.........
+00001f70: 0000 0002 0000 0006 0000 0053 0000 0073  ...........S...s
+00001f80: 2400 0000 6700 7c00 5d1c 7d01 7c01 6400  $...g.|.].}.|.d.
+00001f90: 1900 7c01 6401 1900 6402 6403 8502 1900  ..|.d...d.d.....
+00001fa0: 6702 9102 7104 5300 2904 7201 0000 0072  g...q.S.).r....r
+00001fb0: 0300 0000 4e72 5900 0000 7216 0000 0072  ....NrY...r....r
+00001fc0: 5700 0000 7216 0000 0072 1600 0000 7217  W...r....r....r.
+00001fd0: 0000 0072 2500 0000 fa00 0000 7226 0000  ...r%.......r&..
+00001fe0: 0029 0a72 4700 0000 da03 6d61 7872 0800  .).rG.....maxr..
+00001ff0: 0000 da03 7375 6d72 4300 0000 da09 656e  ....sumrC.....en
+00002000: 756d 6572 6174 6572 1000 0000 723a 0000  umerater....r:..
+00002010: 0072 4900 0000 722b 0000 0029 0972 1500  .rI...r+...).r..
+00002020: 0000 724a 0000 005a 0e6e 756d 5f74 6172  ..rJ...Z.num_tar
+00002030: 6765 745f 7365 71da 0e63 6865 636b 5f70  get_seq..check_p
+00002040: 7265 7365 6e63 65da 0970 6f73 6974 696f  resence..positio
+00002050: 6e73 da0e 6368 6563 6b5f 706f 7369 7469  ns..check_positi
+00002060: 6f6e 7236 0000 0072 4f00 0000 722f 0000  onr6...rO...r/..
+00002070: 0072 1600 0000 2904 7255 0000 0072 5100  .r....).rU...rQ.
+00002080: 0000 7256 0000 0072 5300 0000 7217 0000  ..rV...rS...r...
+00002090: 00da 115f 6164 645f 6368 6169 6e5f 6272  ..._add_chain_br
+000020a0: 6561 6b73 b600 0000 7344 0000 0000 0f0e  eaks....sD......
+000020b0: 010e 030e 0212 040c 040a 010a ff06 0316  ................
+000020c0: 060a 010a ff06 0308 010c 030a fd06 0514  ................
+000020d0: 0420 0110 021e ff06 0210 0202 0102 ff06  . ..............
+000020e0: 030a 021c 0316 010e 0116 010e 020a 030a  ................
+000020f0: 027a 224d 6f64 656c 6c65 725f 6d61 6e61  .z"Modeller_mana
+00002100: 6765 722e 5f61 6464 5f63 6861 696e 5f62  ger._add_chain_b
+00002110: 7265 616b 7363 0100 0000 0000 0000 0000  reaksc..........
+00002120: 0000 0a00 0000 0800 0000 4300 0000 737e  ..........C...s~
+00002130: 0100 0064 0164 02a0 007c 006a 01a1 0117  ...d.d...|.j....
+00002140: 0064 0317 007d 0174 027c 006a 036a 047c  .d...}.t.|.j.j.|
+00002150: 0183 027d 0267 007d 0374 0583 008f 487d  ...}.g.}.t....H}
+00002160: 0474 027c 006a 036a 0464 0483 027d 057c  .t.|.j.j.d...}.|
+00002170: 04a0 067c 05a1 017d 067c 06a0 0764 05a1  ...|...}.|...d..
+00002180: 0164 0664 0085 0219 007d 0764 0764 0884  .d.d.....}.d.d..
+00002190: 007c 0744 0083 017d 0357 0064 0004 0004  .|.D...}.W.d....
+000021a0: 0083 0301 006e 1031 0073 7a30 0001 0001  .....n.1.sz0....
+000021b0: 0001 0059 0001 007c 00a0 087c 006a 017c  ...Y...|...|.j.|
+000021c0: 0364 0919 0064 0619 00a1 027c 0364 0919  .d...d.....|.d..
+000021d0: 0064 063c 007c 00a0 097c 03a1 017d 0364  .d.<.|...|...}.d
+000021e0: 027d 087c 0864 0a7c 006a 036a 0a17 0064  .}.|.d.|.j.j...d
+000021f0: 0b17 0037 007d 087c 0864 0c7c 006a 036a  ...7.}.|.d.|.j.j
+00002200: 0a17 0064 0d17 0037 007d 087c 087c 0364  ...d...7.}.|.|.d
+00002210: 0919 0064 0619 0064 0e17 0037 007d 087c  ...d...d...7.}.|
+00002220: 0364 0664 0085 0219 0044 005d 447d 097c  .d.d.....D.]D}.|
+00002230: 0864 0a7c 0964 0919 0017 0064 0f17 0064  .d.|.d.....d...d
+00002240: 0b17 0037 007d 087c 0864 107c 0964 0919  ...7.}.|.d.|.d..
+00002250: 0017 0064 0f17 0064 0d17 0037 007d 087c  ...d...d...7.}.|
+00002260: 087c 0964 0619 0064 0e17 0037 007d 0871  .|.d...d...7.}.q
+00002270: f87c 006a 0b90 0172 7a74 0583 008f 1c7d  .|.j...rzt.....}
+00002280: 047c 04a0 0c7c 027c 08a1 0201 0057 0064  .|...|.|.....W.d
+00002290: 0004 0004 0083 0301 006e 1231 0090 0173  .........n.1...s
+000022a0: 7030 0001 0001 0001 0059 0001 0064 0053  p0.......Y...d.S
+000022b0: 0029 114e 5a0f 6d6f 6465 6c6c 6572 5f69  .).NZ.modeller_i
+000022c0: 6e70 7574 5f72 0b00 0000 722c 0000 007a  nput_r....r,...z
+000022d0: 1774 656d 706c 6174 6573 5f61 6c69 676e  .templates_align
+000022e0: 6564 2e66 6173 7461 fa01 3e72 0300 0000  ed.fasta..>r....
+000022f0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00002300: 0008 0000 0053 0000 0073 3a00 0000 6700  .....S...s:...g.
+00002310: 7c00 5d32 7d01 7c01 a000 6400 a101 6401  |.]2}.|...d...d.
+00002320: 1900 a000 a100 6402 1900 6403 a001 7c01  ......d...d...|.
+00002330: a000 6400 a101 6404 6405 8502 1900 a101  ..d...d.d.......
+00002340: 6702 9102 7104 5300 2906 da01 0a72 0100  g...q.S.)....r..
+00002350: 0000 7259 0000 0072 0b00 0000 7203 0000  ..rY...r....r...
+00002360: 004e 2902 da05 7370 6c69 7472 1300 0000  .N)...splitr....
+00002370: 2902 7223 0000 00da 0178 7216 0000 0072  ).r#.....xr....r
+00002380: 1600 0000 7217 0000 0072 2500 0000 0d01  ....r....r%.....
+00002390: 0000 7226 0000 007a 344d 6f64 656c 6c65  ..r&...z4Modelle
+000023a0: 725f 6d61 6e61 6765 722e 7772 6974 655f  r_manager.write_
+000023b0: 616c 6967 6e6d 656e 742e 3c6c 6f63 616c  alignment.<local
+000023c0: 733e 2e3c 6c69 7374 636f 6d70 3e72 0100  s>.<listcomp>r..
+000023d0: 0000 7a04 3e50 313b 7262 0000 007a 0973  ..z.>P1;rb...z.s
+000023e0: 6571 7565 6e63 653a 7a0d 3a2e 3a2e 3a2e  equence:z.:.:.:.
+000023f0: 3a2e 3a3a 3a3a 0a7a 022a 0a72 3000 0000  :.::::.z.*.r0...
+00002400: 7a0b 7374 7275 6374 7572 6558 3a29 0d72  z.structureX:).r
+00002410: 1300 0000 7206 0000 0072 0200 0000 720d  ....r....r....r.
+00002420: 0000 0072 3700 0000 7204 0000 00da 0972  ...r7...r......r
+00002430: 6561 645f 6669 6c65 7263 0000 0072 4500  ead_filerc...rE.
+00002440: 0000 7260 0000 0072 1b00 0000 7212 0000  ..r`...r....r...
+00002450: 0072 3b00 0000 290a 7215 0000 0072 3c00  .r;...).r....r<.
+00002460: 0000 da0b 6f75 7470 7574 5f70 6174 6872  ....output_pathr
+00002470: 4a00 0000 723f 0000 00da 0966 696c 655f  J...r?.....file_
+00002480: 7061 7468 5a15 616c 6967 6e65 645f 7365  pathZ.aligned_se
+00002490: 7175 656e 6365 5f66 696c 655a 1161 6c69  quence_fileZ.ali
+000024a0: 676e 6564 5f73 6571 7565 6e63 6573 723e  gned_sequencesr>
+000024b0: 0000 00da 1174 656d 706c 6174 655f 7365  .....template_se
+000024c0: 7175 656e 6365 7216 0000 0072 1600 0000  quencer....r....
+000024d0: 7217 0000 0072 1d00 0000 0301 0000 733a  r....r........s:
+000024e0: 0000 0000 0214 010e 0204 0108 010e 010a  ................
+000024f0: 0112 012c 031e 030a 0404 0114 0114 0114  ...,............
+00002500: 0310 0118 0102 0102 0106 ff02 0202 fe02  ................
+00002510: 0302 fd02 ff04 0612 0508 0108 017a 204d  .............z M
+00002520: 6f64 656c 6c65 725f 6d61 6e61 6765 722e  odeller_manager.
+00002530: 7772 6974 655f 616c 6967 6e6d 656e 7463  write_alignmentc
+00002540: 0100 0000 0000 0000 0000 0000 0600 0000  ................
+00002550: 0800 0000 4300 0000 7302 0100 007c 006a  ....C...s....|.j
+00002560: 0064 016b 0272 4674 0164 0264 03a0 027c  .d.k.rFt.d.d...|
+00002570: 006a 03a1 0117 0064 0417 007c 006a 046a  .j.....d...|.j.j
+00002580: 0517 0064 0517 007c 006a 046a 0617 0064  ...d...|.j.j...d
+00002590: 0617 0083 0101 007c 00a0 07a1 0001 0064  .......|.......d
+000025a0: 0053 0074 087c 006a 046a 097c 006a 046a  .S.t.|.j.j.|.j.j
+000025b0: 0564 0717 0064 03a0 027c 006a 03a1 0117  .d...d...|.j....
+000025c0: 0064 0817 0083 027d 0174 0a83 008f 1a7d  .d.....}.t.....}
+000025d0: 027c 02a0 0b7c 01a1 0101 0057 0064 0004  .|...|.....W.d..
+000025e0: 0004 0083 0301 006e 1031 0073 9230 0001  .......n.1.s.0..
+000025f0: 0001 0001 0059 0001 0074 0ca0 0da1 007d  .....Y...t.....}
+00002600: 0374 0ca0 0e74 0f7c 0183 01a1 0101 0064  .t...t.|.......d
+00002610: 0964 03a0 027c 006a 03a1 0117 0064 0a17  .d...|.j.....d..
+00002620: 007d 047c 006a 109b 0064 0574 0f7c 0483  .}.|.j...d.t.|..
+00002630: 019b 009d 037d 0574 116a 127c 0564 0b64  .....}.t.j.|.d.d
+00002640: 0b64 0b64 0c8d 0401 0074 0ca0 0e7c 03a1  .d.d.....t...|..
+00002650: 0101 007c 00a0 07a1 0001 0064 0053 0029  ...|.......d.S.)
+00002660: 0d4e 467a 164d 6f64 656c 6c69 6e67 206f  .NFz.Modelling o
+00002670: 6620 6d75 7461 7469 6f6e 2072 0b00 0000  f mutation r....
+00002680: 7a11 2077 6173 2065 7863 6c75 6465 6420  z. was excluded 
+00002690: 6f6e 2072 1900 0000 7a19 2064 7565 2074  on r....z. due t
+000026a0: 6f20 6d69 7373 696e 6720 636f 7665 7261  o missing covera
+000026b0: 6765 2e72 2f00 0000 5a06 5f6d 6f64 656c  ge.r/...Z._model
+000026c0: 7a10 2e2e 2f72 756e 5f6d 6f64 656c 6c65  z.../run_modelle
+000026d0: 725f 722e 0000 0054 2903 da05 7368 656c  r_r....T)...shel
+000026e0: 6cda 1275 6e69 7665 7273 616c 5f6e 6577  l..universal_new
+000026f0: 6c69 6e65 73da 0563 6865 636b 2913 7212  lines..check).r.
+00002700: 0000 0072 1a00 0000 7213 0000 0072 0600  ...r....r....r..
+00002710: 0000 720d 0000 0072 1b00 0000 721c 0000  ..r....r....r...
+00002720: 00da 0d6c 6f61 645f 6c6f 675f 6669 6c65  ...load_log_file
+00002730: 7202 0000 0072 3700 0000 7204 0000 00da  r....r7...r.....
+00002740: 1063 7265 6174 655f 6469 7265 6374 6f72  .create_director
+00002750: 79da 026f 73da 0667 6574 6377 64da 0563  y..os..getcwd..c
+00002760: 6864 6972 7239 0000 0072 0700 0000 da0a  hdirr9...r......
+00002770: 7375 6270 726f 6365 7373 da03 7275 6e29  subprocess..run)
+00002780: 0672 1500 0000 5a0a 6d6f 6465 6c5f 7061  .r....Z.model_pa
+00002790: 7468 723f 0000 005a 1668 6f6d 655f 776f  thr?...Z.home_wo
+000027a0: 726b 696e 675f 6469 7265 6374 6f72 7972  rking_directoryr
+000027b0: 3d00 0000 da07 636f 6d6d 616e 6472 1600  =.....commandr..
+000027c0: 0000 7216 0000 0072 1700 0000 7272 0000  ..r....r....rr..
+000027d0: 002e 0100 0073 3a00 0000 0002 0a01 1001  .....s:.........
+000027e0: 02ff 0201 06ff 0201 02ff 0202 06fe 0202  ................
+000027f0: 02fe 0603 0801 0402 0201 0601 1afe 0404  ................
+00002800: 0801 2801 0801 0e01 1401 1401 0401 08ff  ..(.............
+00002810: 0603 0a01 7a14 4d6f 6465 6c6c 6572 5f6d  ....z.Modeller_m
+00002820: 616e 6167 6572 2e72 756e 6301 0000 0000  anager.runc.....
+00002830: 0000 0000 0000 0006 0000 0008 0000 0043  ...............C
+00002840: 0000 0073 9400 0000 7c00 6a00 7288 7401  ...s....|.j.r.t.
+00002850: 8300 8f6a 7d01 7402 7c00 6a03 6a04 6401  ...j}.t.|.j.j.d.
+00002860: 6402 a005 7c00 6a06 a101 1700 6403 1700  d...|.j.....d...
+00002870: 8302 7d02 7c01 a007 7c02 a101 a008 a100  ..}.|...|.......
+00002880: 7d03 7c03 a009 6404 a101 7d04 7c04 7c03  }.|...d...}.|.|.
+00002890: 7c04 6405 8502 1900 a009 6402 a101 1700  |.d.......d.....
+000028a0: 7d05 7c03 7c04 7c05 8502 1900 7c00 5f0a  }.|.|.|.....|._.
+000028b0: 5700 6405 0400 0400 8303 0100 7190 3100  W.d.........q.1.
+000028c0: 737c 3000 0100 0100 0100 5900 0100 6e08  s|0.......Y...n.
+000028d0: 6406 6701 7c00 5f0a 6405 5300 2907 6118  d.g.|._.d.S.).a.
+000028e0: 0100 0020 4f70 656e 2074 6865 206c 6f67  ... Open the log
+000028f0: 2066 696c 6520 6166 7465 7220 7468 6520   file after the 
+00002900: 7275 6e20 6f66 206d 6f64 656c 6c65 722e  run of modeller.
+00002910: 0a20 2020 2020 2020 204c 6f6f 6b20 666f  .        Look fo
+00002920: 7220 7468 6520 7461 626c 6520 7769 7468  r the table with
+00002930: 2074 6865 2044 4f50 4520 7363 6f72 6573   the DOPE scores
+00002940: 2e0a 2020 2020 2020 2020 5361 7665 2069  ..        Save i
+00002950: 7420 6173 2061 7474 7269 6275 7465 2028  t as attribute (
+00002960: 6c69 7374 292e 0a20 2020 2020 2020 200a  list)..        .
+00002970: 2020 2020 2020 2020 4275 7420 6966 2074          But if t
+00002980: 6865 206d 7574 6174 696f 6e20 6973 206e  he mutation is n
+00002990: 6f74 206d 6f64 656c 6c61 626c 652c 2064  ot modellable, d
+000029a0: 7565 2074 6f20 6d69 7373 696e 6720 7465  ue to missing te
+000029b0: 6d70 6c61 7465 0a20 2020 2020 2020 2063  mplate.        c
+000029c0: 6f6e 7665 7261 6765 2c20 6a75 7374 2073  onverage, just s
+000029d0: 6176 6520 6120 7761 726e 696e 6720 7374  ave a warning st
+000029e0: 7269 6e67 2061 7320 6174 7472 6962 7574  ring as attribut
+000029f0: 652e 0a20 2020 2020 2020 2072 2d00 0000  e..        r-...
+00002a00: 720b 0000 007a 042e 6c6f 677a 4646 696c  r....z..logzFFil
+00002a10: 656e 616d 6520 2020 2020 2020 2020 2020  ename           
+00002a20: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00002a30: 6f6c 7064 6620 2020 2020 444f 5045 2073  olpdf     DOPE s
+00002a40: 636f 7265 2020 2020 4741 3334 3120 7363  core    GA341 sc
+00002a50: 6f72 654e 7a4a 2120 5468 6520 6d75 7461  oreNzJ! The muta
+00002a60: 7469 6f6e 2077 6173 206e 6f74 206d 6f64  tion was not mod
+00002a70: 656c 6c65 642c 2064 7565 2074 6f20 6d69  elled, due to mi
+00002a80: 7373 696e 6720 7465 6d70 6c61 7465 7320  ssing templates 
+00002a90: 666f 7220 7468 6174 2072 6567 696f 6e2e  for that region.
+00002aa0: 290b 7212 0000 0072 0400 0000 7202 0000  ).r....r....r...
+00002ab0: 0072 0d00 0000 7237 0000 0072 1300 0000  .r....r7...r....
+00002ac0: 7206 0000 0072 6500 0000 da0a 7370 6c69  r....re.....spli
+00002ad0: 746c 696e 6573 da05 696e 6465 7872 0f00  tlines..indexr..
+00002ae0: 0000 2906 7215 0000 0072 3f00 0000 5a08  ..).r....r?...Z.
+00002af0: 6c6f 675f 7061 7468 5a04 6c6f 6773 5a11  log_pathZ.logsZ.
+00002b00: 7461 626c 655f 7374 6172 745f 696e 6465  table_start_inde
+00002b10: 785a 0f74 6162 6c65 5f65 6e64 5f69 6e64  xZ.table_end_ind
+00002b20: 6578 7216 0000 0072 1600 0000 7217 0000  exr....r....r...
+00002b30: 0072 6c00 0000 4701 0000 7310 0000 0000  .rl...G...s.....
+00002b40: 0806 0108 011e 010e 020a 0116 022e 027a  ...............z
+00002b50: 1e4d 6f64 656c 6c65 725f 6d61 6e61 6765  .Modeller_manage
+00002b60: 722e 6c6f 6164 5f6c 6f67 5f66 696c 6529  r.load_log_file)
+00002b70: 12da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
+00002b80: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
+00002b90: 616d 655f 5fda 046c 6973 7472 3900 0000  ame__..listr9...
+00002ba0: 7227 0000 0072 1800 0000 721f 0000 00da  r'...r....r.....
+00002bb0: 0462 6f6f 6c72 2b00 0000 721e 0000 0072  .boolr+...r....r
+00002bc0: 4500 0000 7247 0000 0072 4900 0000 7260  E...rG...rI...r`
+00002bd0: 0000 0072 1d00 0000 7272 0000 0072 6c00  ...r....rr...rl.
+00002be0: 0000 7216 0000 0072 1600 0000 7216 0000  ..r....r....r...
+00002bf0: 0072 1700 0000 7205 0000 0008 0000 0073  .r....r........s
+00002c00: 1a00 0000 0801 0601 04ff 0c10 0809 0e1c  ................
+00002c10: 083f 101e 100c 100f 104d 082b 0e19 7205  .?.......M.+..r.
+00002c20: 0000 0029 0772 6e00 0000 7271 0000 00da  ...).rn...rq....
+00002c30: 0770 6174 686c 6962 7202 0000 00da 0c66  .pathlibr......f
+00002c40: 696c 655f 6861 6e64 6c65 7272 0400 0000  ile_handlerr....
+00002c50: 7205 0000 0072 1600 0000 7216 0000 0072  r....r....r....r
+00002c60: 1600 0000 7217 0000 00da 083c 6d6f 6475  ....r......<modu
+00002c70: 6c65 3e01 0000 0073 0800 0000 0801 0801  le>....s........
+00002c80: 0c02 0c03                                ....
```

### Comparing `monviso-0.1.3/monviso_reloaded/__pycache__/template.cpython-39.pyc` & `monviso-0.1.4/monviso_reloaded/__pycache__/template.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `monviso-0.1.3/monviso_reloaded/base.py` & `monviso-0.1.4/monviso_reloaded/base.py`

 * *Files identical despite different names*

### Comparing `monviso-0.1.3/monviso_reloaded/cli.py` & `monviso-0.1.4/monviso_reloaded/cli.py`

 * *Files identical despite different names*

### Comparing `monviso-0.1.3/monviso_reloaded/cobalt_wrapper.py` & `monviso-0.1.4/monviso_reloaded/cobalt_wrapper.py`

 * *Files identical despite different names*

### Comparing `monviso-0.1.3/monviso_reloaded/database_parser.py` & `monviso-0.1.4/monviso_reloaded/database_parser.py`

 * *Files identical despite different names*

### Comparing `monviso-0.1.3/monviso_reloaded/file_handler.py` & `monviso-0.1.4/monviso_reloaded/file_handler.py`

 * *Files identical despite different names*

### Comparing `monviso-0.1.3/monviso_reloaded/gene.py` & `monviso-0.1.4/monviso_reloaded/gene.py`

 * *Files identical despite different names*

### Comparing `monviso-0.1.3/monviso_reloaded/input_parser.py` & `monviso-0.1.4/monviso_reloaded/input_parser.py`

 * *Files identical despite different names*

### Comparing `monviso-0.1.3/monviso_reloaded/isoform.py` & `monviso-0.1.4/monviso_reloaded/isoform.py`

 * *Files identical despite different names*

### Comparing `monviso-0.1.3/monviso_reloaded/modeller_manager.py` & `monviso-0.1.4/monviso_reloaded/modeller_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,15 +118,15 @@
             + self.isoform.gene_name
             + """\", normalize_profile=True, smoothing_window=15)"""
         )
 
         with FileHandler() as fh:
             fh.write_file(script_path, content)
 
-    def _mutate_reside(self, mutation, sequence:str) -> bool:
+    def _mutate_residue(self, mutation, sequence:str) -> bool:
         """Take a mutation in the format
         [1 letter amino acid,residue number, 1 lett. amino acid]
         and apply it to the aligned sequence to model,
         taking into account all the "-"'s.
 
         Returns edited sequence
         """
@@ -149,15 +149,15 @@
                 return sequence
             i += 1
 
         print(f"Could not apply mutation {mutation}!")
         return sequence
 
     def _add_number_to_sequence(self,sequence:str)->list:
-        """From a sequence, return a 2D list with [resnum,resiude]"""
+        """From a sequence, return a 2D list with [resnum,residue]"""
         numbered_seq=[]
         i=1
         for char in sequence:
             if (char=="-"):
                 numbered_seq.append(["-",char])
             else:
                 numbered_seq.append([i,char])
@@ -173,15 +173,15 @@
         filtered_numbers=[r[0] for r in sequence_with_resnum if r[0]!="-"]
 
    
         self.chain_starts.append(filtered_numbers[0])
 
         for i in range(1,len(filtered_numbers)):
             if filtered_numbers[i]!=filtered_numbers[i-1]+1:
-                self.chain_starts.append(filtered_numbers[i]-1)
+                self.chain_starts.append(filtered_numbers[i]+1)
     
     def _add_chain_breaks(self, sequences: list) -> list:
         """For alignments in which there is no coverage for self.model_cutoff+
         residues, the section without coverage is replaced by
         chain breaks.
 
         Args:
@@ -226,15 +226,15 @@
                         == "-" * max_non_covered
                         for seq in aligned_seq[1:]
                     ]
                     if sum(check_position) == (len(aligned_seq) - 1):
                         # If that is the case, replace that section in
                         # all sequences (+ target sequences) with a chain
                         # break ("/").
-                        num_target_seq=num_target_seq[:pos]+num_target_seq[pos + max_non_covered :]
+                        num_target_seq=num_target_seq[:pos]+num_target_seq[pos + max_non_covered -1:]
                         for i, seq in enumerate(aligned_seq):
                             aligned_seq[i] = (
                                 seq[:pos] + "/" + seq[pos + max_non_covered :])
                             self.num_chains+=1
 
                         max_non_covered += (
                             1  # This repeats the check for the current value
@@ -265,15 +265,15 @@
         with FileHandler() as fh:
             file_path=Path(self.isoform.out_path,"templates_aligned.fasta")
             aligned_sequence_file=fh.read_file(file_path)
             aligned_sequences=aligned_sequence_file.split(">")[1:]
             sequences=[[x.split("\n")[0].split()[-1],"".join(x.split('\n')[1:])] for x in aligned_sequences]
 
         #Add mutation if needed
-        sequences[0][1]=self._mutate_reside(self.mutation,sequences[0][1])
+        sequences[0][1]=self._mutate_residue(self.mutation,sequences[0][1])
         
         # Add chain breaks in place of long seqs with no coverage
         sequences = self._add_chain_breaks(sequences)
 
 
         # Start writing the content string to be printed in the file
         content = ""
@@ -299,15 +299,15 @@
             with FileHandler() as fh:
                 fh.write_file(output_path, content)
 
     def run(self) -> None:
         
         if self.mutation_is_modellable==False:
             print("Modelling of mutation "+"".join(self.mutation)+
-                  " was eexcluded on "+self.isoform.gene_name+" "+
+                  " was excluded on "+self.isoform.gene_name+" "+
                   self.isoform.isoform_name+" due to missing coverage.")
             self.load_log_file()
             return None
         
         model_path = Path(
             self.isoform.out_path,
             self.isoform.gene_name + "_" + "".join(self.mutation) + "_model",
```

### Comparing `monviso-0.1.3/monviso_reloaded/template.py` & `monviso-0.1.4/monviso_reloaded/template.py`

 * *Files identical despite different names*

### Comparing `monviso-0.1.3/setup.py` & `monviso-0.1.4/setup.py`

 * *Files identical despite different names*

