# Comparing `tmp/biorag-0.1.5.tar.gz` & `tmp/biorag-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biorag-0.1.5.tar", max compression
+gzip compressed data, was "biorag-0.1.6.tar", max compression
```

## Comparing `biorag-0.1.5.tar` & `biorag-0.1.6.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     7184 2024-03-24 07:20:34.106827 biorag-0.1.5/README.md
--rw-r--r--   0        0        0        0 2024-03-16 04:52:33.038054 biorag-0.1.5/biorag/__init__.py
--rw-r--r--   0        0        0    21229 2024-03-27 00:33:04.741799 biorag-0.1.5/biorag/biorag.py
--rw-r--r--   0        0        0     3594 2024-03-26 21:50:17.272832 biorag-0.1.5/biorag/enrichment.py
--rw-r--r--   0        0        0     6195 2024-03-26 13:48:20.855664 biorag-0.1.5/biorag/rag_embedding.py
--rw-r--r--   0        0        0     5377 2024-03-26 21:47:42.662500 biorag-0.1.5/biorag/rnaseq_analysis.py
--rw-r--r--   0        0        0     3778 2024-03-22 15:58:47.152255 biorag-0.1.5/biorag/transcriptome_embedding.py
--rw-r--r--   0        0        0     4590 2024-03-21 20:18:03.941548 biorag-0.1.5/biorag/utils.py
--rw-r--r--   0        0        0      619 2024-03-27 00:39:54.592533 biorag-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     8152 1970-01-01 00:00:00.000000 biorag-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     7179 2024-04-08 08:11:34.540052 biorag-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2024-03-16 04:52:33.038054 biorag-0.1.6/biorag/__init__.py
+-rw-r--r--   0        0        0    21834 2024-03-28 02:40:31.472799 biorag-0.1.6/biorag/biorag.py
+-rw-r--r--   0        0        0     4888 2024-04-08 08:09:03.303101 biorag-0.1.6/biorag/cli.py
+-rw-r--r--   0        0        0     3594 2024-03-26 21:50:17.272832 biorag-0.1.6/biorag/enrichment.py
+-rw-r--r--   0        0        0     6195 2024-03-26 13:48:20.855664 biorag-0.1.6/biorag/rag_embedding.py
+-rw-r--r--   0        0        0     5377 2024-03-26 21:47:42.662500 biorag-0.1.6/biorag/rnaseq_analysis.py
+-rw-r--r--   0        0        0     3778 2024-03-22 15:58:47.152255 biorag-0.1.6/biorag/transcriptome_embedding.py
+-rw-r--r--   0        0        0     4590 2024-03-21 20:18:03.941548 biorag-0.1.6/biorag/utils.py
+-rw-r--r--   0        0        0      669 2024-04-10 00:08:53.252948 biorag-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     8147 1970-01-01 00:00:00.000000 biorag-0.1.6/PKG-INFO
```

### Comparing `biorag-0.1.5/README.md` & `biorag-0.1.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# BioRAG [![codecov](https://codecov.io/gh/wlchin/bioRAG/graph/badge.svg?token=9GG94JA003)](https://codecov.io/gh/wlchin/bioRAG) ![workflow](https://github.com/wlchin/bioRAG/actions/workflows/python-package.yml/badge.svg)
+# BioRAG [![codecov](https://codecov.io/gh/wlchin/bioRAG/graph/badge.svg?token=9GG94JA003)](https://codecov.io/gh/wlchin/bioRAG) ![workflow](https://github.com/wlchin/bioRAG/actions/workflows/python-package.yml/badge.svg) ![version](https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11-blue) ![license](https://img.shields.io/badge/license-MIT-blue)
 
 This is the repository for BioRAG[^1]. BioRAG can identify relevant studies within the ARCHS4 database, using a text-based query or a gene set. 
 
 ![Image Description](https://github.com/wlchin/bioRAG/blob/master/assets/BioRAG.png)
 
 ## Table of Contents
 
@@ -147,16 +147,17 @@
     result = new_query_db.search(text_query = text_query, geneset = None, search = "semantic", expand = "semantic", perform_enrichment = True)
 
     # save enrichment results from the sample dataframe
     results.samples.to_csv("samples_with_ssgsea_results.csv")
 
 ```
 
+
 ## License
 
-Creative Commons Attribution 4.0 International. The Creative Commons Attribution license allows re-distribution and re-use of a licensed work on the condition that the creator is appropriately credited. 
+BioRAG is published under the MIT License.
 
 ## References
 
-[^1]: Chin WL, & Lassmann, T. (2024). Language models improve the discovery of public RNA-seq data. *bioRxiv*.
+[^1]: Chin WL, & Lassmann, T. (2024). BioRAG: using large language models to discover relevant transcriptome data. *bioRxiv*.
 [^2]: Lachmann A, Torre D, Keenan AB, Jagodnik KM, Lee HJ, Wang L, Silverstein MC, Ma'ayan A. Massive mining of publicly available RNA-seq data from human and mouse. Nat Commun. 2018 Apr 10;9(1):1366. doi: 10.1038/s41467-018-03751-6. PMID: 29636450; PMCID: PMC5893633.
-[^3]: [AnnData] (https://anndata.readthedocs.io/en/latest/)
+[^3]: [AnnData](https://anndata.readthedocs.io/en/latest/)
```

### Comparing `biorag-0.1.5/biorag/biorag.py` & `biorag-0.1.6/biorag/biorag.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,14 +45,15 @@
         self.logger.info("RAG embedding initialized.")
         self.transcriptome_enrichment = Transcriptome_enrichment(trans_obj)        
         self.logger.info("Transcriptome object initialized.")
         
         if h5file is not None:
             self.logger.info("Loading ARCHS4 database object...")
             self.RNASeqAnalysis = RNASeqAnalysis(h5file)
+            self.h5file = h5file    
             self.logger.info("ARCHS4 database object loaded.")
             
             self.logger.info("Creating series to sample mapping...")
             self.metafile = self.process_metadata(h5file)
             self.logger.info("DONE.")
         else:
             self.logger.info("ARCHS4 database object not loaded.")
@@ -71,14 +72,29 @@
             pandas.DataFrame: A DataFrame containing processed metadata with columns 'series_id' and 'samples'.
         """
         x = a4.meta.meta(h5_path, ".*", meta_fields=["series_id"])
         x["samples"] = x.index
         x = x[['series_id', 'samples']].drop_duplicates()
         return x
 
+    def retrieve_sample_metadata_from_h5(self, h5_path, sample_list):
+        """
+        Retrieves sample metadata from an HDF5 file.
+
+        Args:
+            h5_path (str): The path to the HDF5 file.
+            sample_list (list): A list of sample names.
+
+        Returns:
+            dict: A dictionary containing the sample metadata.
+
+        """
+        sample_meta = a4.meta.samples(h5_path, sample_list)
+        return sample_meta
+
     def get_top_samples(self, df, n=1000):
         """
         Returns a subset of samples from the given DataFrame based on their ranking.
 
         Parameters:
         - df (pandas.DataFrame): The DataFrame containing the samples.
         - n (int): The number of top samples to retrieve. Default is 1000.
@@ -385,20 +401,20 @@
                 enrichment_df = self.RNASeqAnalysis.perform_enrichment_on_samples_batched(samps.index, geneset)
                 res_df = pd.concat([enrichment_df, samps], axis = 1)
                 results_object.samples = res_df
                 self.logger.info("Completed enrichment on seed studies.")
         elif perform_enrichment is False and self.RNASeqAnalysis is not None:
             if results_object.expansion_studies is not None:
                 samps = self.metafile[self.metafile["series_id"].isin(results_object.expansion_studies["gse_id"])]
-                res_df = samps
+                res_df = self.retrieve_sample_metadata_from_h5(self.h5file, samps["samples"])
                 results_object.samples = res_df
                 self.logger.info("Retrieving samples from expansion step. Enrichment not performed.")
             else:
                 samps = self.metafile[self.metafile["series_id"].isin(results_object.seed_studies["gse_id"])]
-                res_df = samps
+                res_df = self.retrieve_sample_metadata_from_h5(self.h5file, samps["samples"])
                 results_object.samples = res_df
                 self.logger.info("Retrieving samples from search step. Enrichment not performed.")
         else:
             self.logger.info("Enrichment not performed.")
             results_object.samples = None
             
         #additional_series = additional_series.drop(["similarity_score"], axis=1).reset_index(drop=True).drop_duplicates()
```

### Comparing `biorag-0.1.5/biorag/enrichment.py` & `biorag-0.1.6/biorag/enrichment.py`

 * *Files identical despite different names*

### Comparing `biorag-0.1.5/biorag/rag_embedding.py` & `biorag-0.1.6/biorag/rag_embedding.py`

 * *Files identical despite different names*

### Comparing `biorag-0.1.5/biorag/rnaseq_analysis.py` & `biorag-0.1.6/biorag/rnaseq_analysis.py`

 * *Files identical despite different names*

### Comparing `biorag-0.1.5/biorag/transcriptome_embedding.py` & `biorag-0.1.6/biorag/transcriptome_embedding.py`

 * *Files identical despite different names*

### Comparing `biorag-0.1.5/biorag/utils.py` & `biorag-0.1.6/biorag/utils.py`

 * *Files identical despite different names*

### Comparing `biorag-0.1.5/pyproject.toml` & `biorag-0.1.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "biorag"
-version = "0.1.5"
+version = "0.1.6"
 description = "BioRAG: A tool for textual and gene set search against ARCHS4 data"
 authors = ["wchin <wee.chin@health.wa.gov.au>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pandas = "2.0.2"
@@ -20,11 +20,14 @@
 coverage = "^7.4.4"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
+[tool.poetry.scripts]
+biorag = "biorag.cli:main"
+
 [tool.coverage.run]
 omit = [
     "tests/*"
     ]
```

### Comparing `biorag-0.1.5/PKG-INFO` & `biorag-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biorag
-Version: 0.1.5
+Version: 0.1.6
 Summary: BioRAG: A tool for textual and gene set search against ARCHS4 data
 Author: wchin
 Author-email: wee.chin@health.wa.gov.au
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -19,15 +19,15 @@
 Requires-Dist: pytest-codecov (>=0.5.1,<0.6.0)
 Requires-Dist: pytest-cov (>=4.1.0,<5.0.0)
 Requires-Dist: scipy (>=1.12.0,<2.0.0)
 Requires-Dist: sentence-transformers (>=2.5.1,<3.0.0)
 Requires-Dist: statsmodels (>=0.14.1,<0.15.0)
 Description-Content-Type: text/markdown
 
-# BioRAG [![codecov](https://codecov.io/gh/wlchin/bioRAG/graph/badge.svg?token=9GG94JA003)](https://codecov.io/gh/wlchin/bioRAG) ![workflow](https://github.com/wlchin/bioRAG/actions/workflows/python-package.yml/badge.svg)
+# BioRAG [![codecov](https://codecov.io/gh/wlchin/bioRAG/graph/badge.svg?token=9GG94JA003)](https://codecov.io/gh/wlchin/bioRAG) ![workflow](https://github.com/wlchin/bioRAG/actions/workflows/python-package.yml/badge.svg) ![version](https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11-blue) ![license](https://img.shields.io/badge/license-MIT-blue)
 
 This is the repository for BioRAG[^1]. BioRAG can identify relevant studies within the ARCHS4 database, using a text-based query or a gene set. 
 
 ![Image Description](https://github.com/wlchin/bioRAG/blob/master/assets/BioRAG.png)
 
 ## Table of Contents
 
@@ -172,17 +172,18 @@
     result = new_query_db.search(text_query = text_query, geneset = None, search = "semantic", expand = "semantic", perform_enrichment = True)
 
     # save enrichment results from the sample dataframe
     results.samples.to_csv("samples_with_ssgsea_results.csv")
 
 ```
 
+
 ## License
 
-Creative Commons Attribution 4.0 International. The Creative Commons Attribution license allows re-distribution and re-use of a licensed work on the condition that the creator is appropriately credited. 
+BioRAG is published under the MIT License.
 
 ## References
 
-[^1]: Chin WL, & Lassmann, T. (2024). Language models improve the discovery of public RNA-seq data. *bioRxiv*.
+[^1]: Chin WL, & Lassmann, T. (2024). BioRAG: using large language models to discover relevant transcriptome data. *bioRxiv*.
 [^2]: Lachmann A, Torre D, Keenan AB, Jagodnik KM, Lee HJ, Wang L, Silverstein MC, Ma'ayan A. Massive mining of publicly available RNA-seq data from human and mouse. Nat Commun. 2018 Apr 10;9(1):1366. doi: 10.1038/s41467-018-03751-6. PMID: 29636450; PMCID: PMC5893633.
-[^3]: [AnnData] (https://anndata.readthedocs.io/en/latest/)
+[^3]: [AnnData](https://anndata.readthedocs.io/en/latest/)
```

