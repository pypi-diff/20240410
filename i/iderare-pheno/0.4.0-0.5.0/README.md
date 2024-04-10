# Comparing `tmp/iderare-pheno-0.4.0.tar.gz` & `tmp/iderare-pheno-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iderare-pheno-0.4.0.tar", last modified: Sun Apr  7 10:23:31 2024, max compression
+gzip compressed data, was "iderare-pheno-0.5.0.tar", last modified: Wed Apr 10 10:18:15 2024, max compression
```

## Comparing `iderare-pheno-0.4.0.tar` & `iderare-pheno-0.5.0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:23:31.476653 iderare-pheno-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-07 10:22:43.000000 iderare-pheno-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7725 2024-04-07 10:23:31.476653 iderare-pheno-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4106 2024-04-07 10:22:43.000000 iderare-pheno-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:23:31.384652 iderare-pheno-0.4.0/iderare_pheno/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-07 10:22:43.000000 iderare-pheno-0.4.0/iderare_pheno/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11305 2024-04-07 10:22:43.000000 iderare-pheno-0.4.0/iderare_pheno/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:23:31.380652 iderare-pheno-0.4.0/iderare_pheno/phenotype/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:23:31.416653 iderare-pheno-0.4.0/iderare_pheno/phenotype/data/
--rw-r--r--   0 runner    (1001) docker     (127) 19051578 2024-04-07 10:22:43.000000 iderare-pheno-0.4.0/iderare_pheno/phenotype/data/genes_to_phenotype.txt
--rw-r--r--   0 runner    (1001) docker     (127)  9995624 2024-04-07 10:22:43.000000 iderare-pheno-0.4.0/iderare_pheno/phenotype/data/hp.obo
--rw-r--r--   0 runner    (1001) docker     (127) 31896677 2024-04-07 10:22:43.000000 iderare-pheno-0.4.0/iderare_pheno/phenotype/data/phenotype.hpoa
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:23:31.472653 iderare-pheno-0.4.0/iderare_pheno/phenotype/subset/
--rw-r--r--   0 runner    (1001) docker     (127)   196778 2024-04-07 10:22:43.000000 iderare-pheno-0.4.0/iderare_pheno/phenotype/subset/icd102omim_subset.tsv
--rw-r--r--   0 runner    (1001) docker     (127)   224561 2024-04-07 10:22:43.000000 iderare-pheno-0.4.0/iderare_pheno/phenotype/subset/loinc2hpo_standardized.tsv
--rw-r--r--   0 runner    (1001) docker     (127)  6033462 2024-04-07 10:22:43.000000 iderare-pheno-0.4.0/iderare_pheno/phenotype/subset/omim2hpo_subset.tsv
--rw-r--r--   0 runner    (1001) docker     (127)  7205315 2024-04-07 10:22:43.000000 iderare-pheno-0.4.0/iderare_pheno/phenotype/subset/orpha2hpo_subset.tsv
--rw-r--r--   0 runner    (1001) docker     (127)   218406 2024-04-07 10:22:43.000000 iderare-pheno-0.4.0/iderare_pheno/phenotype/subset/orpha2omim_subset.tsv
--rw-r--r--   0 runner    (1001) docker     (127)   232073 2024-04-07 10:22:43.000000 iderare-pheno-0.4.0/iderare_pheno/phenotype/subset/snomed2hpo_subset.tsv
--rw-r--r--   0 runner    (1001) docker     (127)  1298790 2024-04-07 10:22:43.000000 iderare-pheno-0.4.0/iderare_pheno/phenotype/subset/snomed2orpha_subset.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 10:22:43.000000 iderare-pheno-0.4.0/iderare_pheno/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     6585 2024-04-07 10:22:43.000000 iderare-pheno-0.4.0/iderare_pheno/simrec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:23:31.472653 iderare-pheno-0.4.0/iderare_pheno/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-07 10:22:43.000000 iderare-pheno-0.4.0/iderare_pheno/templates/template_iderare.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-07 10:22:43.000000 iderare-pheno-0.4.0/iderare_pheno/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-07 10:22:43.000000 iderare-pheno-0.4.0/iderare_pheno/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:23:31.472653 iderare-pheno-0.4.0/iderare_pheno.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7725 2024-04-07 10:23:31.000000 iderare-pheno-0.4.0/iderare_pheno.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-07 10:23:31.000000 iderare-pheno-0.4.0/iderare_pheno.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 10:23:31.000000 iderare-pheno-0.4.0/iderare_pheno.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-07 10:23:31.000000 iderare-pheno-0.4.0/iderare_pheno.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-07 10:23:31.000000 iderare-pheno-0.4.0/iderare_pheno.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-07 10:22:43.000000 iderare-pheno-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 10:23:31.476653 iderare-pheno-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:18:15.531985 iderare-pheno-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-10 10:17:53.000000 iderare-pheno-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9653 2024-04-10 10:18:15.531985 iderare-pheno-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6022 2024-04-10 10:17:53.000000 iderare-pheno-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:18:15.439985 iderare-pheno-0.5.0/iderare_pheno/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-10 10:17:53.000000 iderare-pheno-0.5.0/iderare_pheno/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11305 2024-04-10 10:17:53.000000 iderare-pheno-0.5.0/iderare_pheno/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:18:15.435985 iderare-pheno-0.5.0/iderare_pheno/phenotype/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:18:15.475985 iderare-pheno-0.5.0/iderare_pheno/phenotype/data/
+-rw-r--r--   0 runner    (1001) docker     (127) 19051578 2024-04-10 10:17:53.000000 iderare-pheno-0.5.0/iderare_pheno/phenotype/data/genes_to_phenotype.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  9995624 2024-04-10 10:17:53.000000 iderare-pheno-0.5.0/iderare_pheno/phenotype/data/hp.obo
+-rw-r--r--   0 runner    (1001) docker     (127) 31896677 2024-04-10 10:17:53.000000 iderare-pheno-0.5.0/iderare_pheno/phenotype/data/phenotype.hpoa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:18:15.527985 iderare-pheno-0.5.0/iderare_pheno/phenotype/subset/
+-rw-r--r--   0 runner    (1001) docker     (127)   196778 2024-04-10 10:17:53.000000 iderare-pheno-0.5.0/iderare_pheno/phenotype/subset/icd102omim_subset.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)   224561 2024-04-10 10:17:53.000000 iderare-pheno-0.5.0/iderare_pheno/phenotype/subset/loinc2hpo_standardized.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)  6033462 2024-04-10 10:17:53.000000 iderare-pheno-0.5.0/iderare_pheno/phenotype/subset/omim2hpo_subset.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)  7205315 2024-04-10 10:17:53.000000 iderare-pheno-0.5.0/iderare_pheno/phenotype/subset/orpha2hpo_subset.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)   218406 2024-04-10 10:17:53.000000 iderare-pheno-0.5.0/iderare_pheno/phenotype/subset/orpha2omim_subset.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)   232073 2024-04-10 10:17:53.000000 iderare-pheno-0.5.0/iderare_pheno/phenotype/subset/snomed2hpo_subset.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)  1298790 2024-04-10 10:17:53.000000 iderare-pheno-0.5.0/iderare_pheno/phenotype/subset/snomed2orpha_subset.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:17:53.000000 iderare-pheno-0.5.0/iderare_pheno/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-04-10 10:17:53.000000 iderare-pheno-0.5.0/iderare_pheno/simrec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-10 10:17:53.000000 iderare-pheno-0.5.0/iderare_pheno/streamlit_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:18:15.531985 iderare-pheno-0.5.0/iderare_pheno/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-10 10:17:53.000000 iderare-pheno-0.5.0/iderare_pheno/templates/template_iderare.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-10 10:17:53.000000 iderare-pheno-0.5.0/iderare_pheno/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-10 10:17:53.000000 iderare-pheno-0.5.0/iderare_pheno/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:18:15.531985 iderare-pheno-0.5.0/iderare_pheno.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9653 2024-04-10 10:18:15.000000 iderare-pheno-0.5.0/iderare_pheno.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-10 10:18:15.000000 iderare-pheno-0.5.0/iderare_pheno.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 10:18:15.000000 iderare-pheno-0.5.0/iderare_pheno.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-10 10:18:15.000000 iderare-pheno-0.5.0/iderare_pheno.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-10 10:18:15.000000 iderare-pheno-0.5.0/iderare_pheno.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-10 10:17:53.000000 iderare-pheno-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 10:18:15.531985 iderare-pheno-0.5.0/setup.cfg
```

### Comparing `iderare-pheno-0.4.0/LICENSE` & `iderare-pheno-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.4.0/PKG-INFO` & `iderare-pheno-0.5.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iderare-pheno
-Version: 0.4.0
+Version: 0.5.0
 Author-email: Ivan William Harsono <ivanwilliam.md@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Ivan William Harsono
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
@@ -32,15 +32,15 @@
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
 Project-URL: Homepage, https://github.com/ivanwilliammd/iderare-pheno
 Project-URL: Repository, https://github.com/ivanwilliammd/iderare-pheno
 Project-URL: Changelog, https://github.com/ivanwilliammd/iderare-pheno/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://iderare-pheno.readthedocs.io/
 Classifier: Intended Audience :: Science/Research
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas
@@ -70,19 +70,14 @@
 Requires-Dist: sphinx-copybutton==0.5.2; extra == "dev"
 Requires-Dist: sphinx-autobuild==2021.3.14; extra == "dev"
 Requires-Dist: sphinx-autodoc-typehints==1.23.3; extra == "dev"
 Requires-Dist: packaging; extra == "dev"
 
 # [IDeRare-Pheno](https://iderare-pheno.readthedocs.io/)
 
-<!-- start tagline -->
-
-IDeRare or "Indonesia Exome Rare Disease Variant Discovery Pipeline" is simple and ready to use variant discovery pipeline to discover rare disease variants from exome sequencing data.
-<!-- end tagline -->
-
 <p align="center">
     <a href="https://github.com/ivanwilliammd/iderare-pheno/actions">
         <img alt="CI" src="https://github.com/ivanwilliammd/iderare-pheno/workflows/Main/badge.svg">
     </a>
     <a href="https://pypi.org/project/iderare_pheno/">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/iderare_pheno">
     </a>
@@ -93,19 +88,39 @@
         <img alt="License" src="https://img.shields.io/github/license/ivanwilliammd/iderare-pheno.svg?color=blue&cachedrop">
     </a>
     <a href="https://bioinformatics-ivanwilliamharsono.streamlit.app/IDeRare_Pheno">
         <img alt="Streamlit" src="https://static.streamlit.io/badges/streamlit_badge_black_white.svg">
     <br/>
 </p>
 
+IDeRare or "Indonesia Exome Rare Disease Variant Discovery Pipeline" is a simple and ready to use variant discovery pipeline to discover rare disease variants from exome sequencing data. 
+
+This repository is **the first part** of IDeRare workflow for **phenotype analysis**. For complete pipeline for _**phenotype-genotype analysis**_, kindly refer to [IDeRare Github repository](https://github.com/ivanwilliammd/IDeRare).
+
+## Authored by 
+Ivan William Harsono<sup>a</sup>, Yulia Ariani<sup>b</sup>, Beben Benyamin<sup>c,d,e</sup>, Fadilah Fadilah<sup>f,g</sup>, Dwi Ari Pujianto<sup>b</sup>, Cut Nurul Hafifah<sup>h</sup>
+
+<sup>a</sup>Doctoral Program in Biomedical Sciences, Faculty of Medicine, Universitas Indonesia, Jakarta, Indonesia.<br> 
+<sup>b</sup>Department of Medical Biology, Faculty of Medicine, Universitas Indonesia, Jakarta, Indonesia.<br> 
+<sup>c</sup>Australian Centre for Precision Health, University of South Australia, Adelaide, SA, 5000, Australia. <br>
+<sup>d</sup>UniSA Allied Health and Human Performance, University of South Australia, Adelaide, SA, 5000, Australia. <br>
+<sup>e</sup>South Australian Health and Medical Research Institute (SAHMRI), University of South Australia, Adelaide, SA, 5000, Australia. <br>
+<sup>f</sup>Department of Medical Chemistry, Faculty of Medicine, Universitas Indonesia, Jalan Salemba Raya number 4, Jakarta, 10430, Indonesia.<br>
+<sup>g</sup>Bioinformatics Core Facilities - IMERI, Faculty of Medicine, Universitas Indonesia, Jalan Salemba Raya number 6, Jakarta, 10430, Indonesia .<br>
+<sup>h</sup>Department of Child Health, Dr. Cipto Mangunkusumo Hospital, Faculty of Medicine, University of Indonesia, Jakarta, Indonesia. <br>
+
+
+**Note:** Currently IDeRare paper is being considered journal submission. The citation will be updated once the paper is published.
+
 ## Quick links
 
 - [Documentation](https://iderare-pheno.readthedocs.io/)
 - [PyPI Package](https://pypi.org/project/iderare-pheno/)
 - [License](https://github.com/ivanwilliammd/iderare-pheno/blob/main/LICENSE)
+- [Interactive Playbook Example](https://github.com/ivanwilliammd/iderare-pheno/blob/main/Playbook.ipynb)
 - Interactive Webapps Implementation of at [Streamlit](https://bioinformatics-ivanwilliamharsono.streamlitapp.com/IDeRare_Pheno)
 
 
 ## What does it do?
 
 This script is recommended if you would like to do conversion, linkage analysis, similarity scoring, and gene-disease recommendation based on the phenotype data provided at [clinical_data.txt](clinical_data.txt). Full feature : 
 1. Convert the phenotype data to HPO code (accept mixed SNOMED, LOINC, and HPO code)
@@ -153,21 +168,23 @@
 
 ```bash
 pip install -e .
 ```
 
 <!-- end install source -->
 
-## Usage
+## Importing the library
 
 ```python
 from iderare_pheno.converter import term2omim, term2orpha, term2hpo, batchconvert
 from iderare_pheno.simrec import hpo2omim_similarity, omim_recommendation, hpo2name
-from iderare_pheno.utils import linkage_dendrogram, list2tsv
+from iderare_pheno.utils import linkage_dendrogram, list2tsv, generate_yml
 ```
+As the complete readthedocs.io is still ongoing, please kindly refer to this [Interactive Playbook Example](https://github.com/ivanwilliammd/iderare-pheno/blob/main/Playbook.ipynb)
+
 
 ## Team
 
 <!-- start team -->
 
 **iderare-pheno** is developed and maintained by the author(s), To learn more about who specifically contributed to this codebase, see [our contributors](https://github.com/ivanwilliammd/iderare-pheno/graphs/contributors) page.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: iderare-pheno Version: 0.4.0 Author-email: Ivan
+Metadata-Version: 2.1 Name: iderare-pheno Version: 0.5.0 Author-email: Ivan
 William Harsono
 gmail.com> License: BSD 3-Clause License Copyright (c) 2024, Ivan William
 Harsono Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met: 1.
 Redistributions of source code must retain the above copyright notice, this
 list of conditions and the following disclaimer. 2. Redistributions in binary
 form must reproduce the above copyright notice, this list of conditions and the
@@ -20,42 +20,65 @@
 LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 ADVISED OF THE POSSIBILITY OF SUCH DAMAGE. Project-URL: Homepage, https://
 github.com/ivanwilliammd/iderare-pheno Project-URL: Repository, https://
 github.com/ivanwilliammd/iderare-pheno Project-URL: Changelog, https://
 github.com/ivanwilliammd/iderare-pheno/blob/main/CHANGELOG.md Project-URL:
 Documentation, https://iderare-pheno.readthedocs.io/ Classifier: Intended
-Audience :: Science/Research Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: BSD License Classifier: Programming
-Language :: Python :: 3 Classifier: Topic :: Scientific/Engineering :: Medical
-Science Apps. Requires-Python: >=3.8 Description-Content-Type: text/markdown
-License-File: LICENSE Requires-Dist: pandas Requires-Dist: numpy Requires-Dist:
-matplotlib Requires-Dist: scipy Requires-Dist: hpo3 Requires-Dist: scikit-learn
-Requires-Dist: pyyaml Provides-Extra: dev Requires-Dist: ruff; extra == "dev"
-Requires-Dist: mypy<1.10,>=1.0; extra == "dev" Requires-Dist: types-PyYAML;
-extra == "dev" Requires-Dist: black<25.0,>=23.0; extra == "dev" Requires-Dist:
-black[jupyter]; extra == "dev" Requires-Dist: isort<5.14,>=5.12; extra == "dev"
-Requires-Dist: pytest; extra == "dev" Requires-Dist: pytest-sphinx; extra ==
-"dev" Requires-Dist: pytest-cov; extra == "dev" Requires-Dist: twine>=1.11.0;
-extra == "dev" Requires-Dist: build; extra == "dev" Requires-Dist: setuptools;
-extra == "dev" Requires-Dist: wheel; extra == "dev" Requires-Dist:
-Sphinx<7.3.0,>=4.3.0; extra == "dev" Requires-Dist: furo==2024.1.29; extra ==
-"dev" Requires-Dist: myst-parser<2.1,>=1.0; extra == "dev" Requires-Dist:
-sphinx-copybutton==0.5.2; extra == "dev" Requires-Dist: sphinx-
-autobuild==2021.3.14; extra == "dev" Requires-Dist: sphinx-autodoc-
-typehints==1.23.3; extra == "dev" Requires-Dist: packaging; extra == "dev" #
-[IDeRare-Pheno](https://iderare-pheno.readthedocs.io/) IDeRare or "Indonesia
-Exome Rare Disease Variant Discovery Pipeline" is simple and ready to use
-variant discovery pipeline to discover rare disease variants from exome
-sequencing data.
+Audience :: Science/Research Classifier: Development Status :: 5 - Production/
+Stable Classifier: License :: OSI Approved :: BSD License Classifier:
+Programming Language :: Python :: 3 Classifier: Topic :: Scientific/Engineering
+:: Medical Science Apps. Requires-Python: >=3.8 Description-Content-Type: text/
+markdown License-File: LICENSE Requires-Dist: pandas Requires-Dist: numpy
+Requires-Dist: matplotlib Requires-Dist: scipy Requires-Dist: hpo3 Requires-
+Dist: scikit-learn Requires-Dist: pyyaml Provides-Extra: dev Requires-Dist:
+ruff; extra == "dev" Requires-Dist: mypy<1.10,>=1.0; extra == "dev" Requires-
+Dist: types-PyYAML; extra == "dev" Requires-Dist: black<25.0,>=23.0; extra ==
+"dev" Requires-Dist: black[jupyter]; extra == "dev" Requires-Dist:
+isort<5.14,>=5.12; extra == "dev" Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-sphinx; extra == "dev" Requires-Dist: pytest-cov; extra
+== "dev" Requires-Dist: twine>=1.11.0; extra == "dev" Requires-Dist: build;
+extra == "dev" Requires-Dist: setuptools; extra == "dev" Requires-Dist: wheel;
+extra == "dev" Requires-Dist: Sphinx<7.3.0,>=4.3.0; extra == "dev" Requires-
+Dist: furo==2024.1.29; extra == "dev" Requires-Dist: myst-parser<2.1,>=1.0;
+extra == "dev" Requires-Dist: sphinx-copybutton==0.5.2; extra == "dev"
+Requires-Dist: sphinx-autobuild==2021.3.14; extra == "dev" Requires-Dist:
+sphinx-autodoc-typehints==1.23.3; extra == "dev" Requires-Dist: packaging;
+extra == "dev" # [IDeRare-Pheno](https://iderare-pheno.readthedocs.io/)
              _[_C_I_]_[_P_y_P_I_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_L_i_c_e_n_s_e_]_[_S_t_r_e_a_m_l_i_t_]
-## Quick links - [Documentation](https://iderare-pheno.readthedocs.io/) - [PyPI
-Package](https://pypi.org/project/iderare-pheno/) - [License](https://
-github.com/ivanwilliammd/iderare-pheno/blob/main/LICENSE) - Interactive Webapps
-Implementation of at [Streamlit](https://bioinformatics-
+IDeRare or "Indonesia Exome Rare Disease Variant Discovery Pipeline" is a
+simple and ready to use variant discovery pipeline to discover rare disease
+variants from exome sequencing data. This repository is **the first part** of
+IDeRare workflow for **phenotype analysis**. For complete pipeline for
+_**phenotype-genotype analysis**_, kindly refer to [IDeRare Github repository]
+(https://github.com/ivanwilliammd/IDeRare). ## Authored by Ivan William
+Harsonoa, Yulia Arianib, Beben Benyaminc,d,e, Fadilah Fadilahf,g, Dwi Ari
+Pujiantob, Cut Nurul Hafifahh aDoctoral Program in Biomedical Sciences, Faculty
+of Medicine, Universitas Indonesia, Jakarta, Indonesia.
+bDepartment of Medical Biology, Faculty of Medicine, Universitas Indonesia,
+Jakarta, Indonesia.
+cAustralian Centre for Precision Health, University of South Australia,
+Adelaide, SA, 5000, Australia.
+dUniSA Allied Health and Human Performance, University of South Australia,
+Adelaide, SA, 5000, Australia.
+eSouth Australian Health and Medical Research Institute (SAHMRI), University of
+South Australia, Adelaide, SA, 5000, Australia.
+fDepartment of Medical Chemistry, Faculty of Medicine, Universitas Indonesia,
+Jalan Salemba Raya number 4, Jakarta, 10430, Indonesia.
+gBioinformatics Core Facilities - IMERI, Faculty of Medicine, Universitas
+Indonesia, Jalan Salemba Raya number 6, Jakarta, 10430, Indonesia .
+hDepartment of Child Health, Dr. Cipto Mangunkusumo Hospital, Faculty of
+Medicine, University of Indonesia, Jakarta, Indonesia.
+**Note:** Currently IDeRare paper is being considered journal submission. The
+citation will be updated once the paper is published. ## Quick links -
+[Documentation](https://iderare-pheno.readthedocs.io/) - [PyPI Package](https:/
+/pypi.org/project/iderare-pheno/) - [License](https://github.com/ivanwilliammd/
+iderare-pheno/blob/main/LICENSE) - [Interactive Playbook Example](https://
+github.com/ivanwilliammd/iderare-pheno/blob/main/Playbook.ipynb) - Interactive
+Webapps Implementation of at [Streamlit](https://bioinformatics-
 ivanwilliamharsono.streamlitapp.com/IDeRare_Pheno) ## What does it do? This
 script is recommended if you would like to do conversion, linkage analysis,
 similarity scoring, and gene-disease recommendation based on the phenotype data
 provided at [clinical_data.txt](clinical_data.txt). Full feature : 1. Convert
 the phenotype data to HPO code (accept mixed SNOMED, LOINC, and HPO code) 2.
 Similarity scoring of differential diagnosis 3. Linkage analysis of
 differential diagnosis (accept mixed SNOMED, ICD-10, ORPHA, OMIM code), include
@@ -70,16 +93,19 @@
 Information Example section](#clinical-information-example) ## Installation
 **iderare-pheno** requires Python 3.8 or later. ### Installing with `pip`
 **iderare-pheno** is available [on PyPI](https://pypi.org/project/iderare-
 pheno/). Just run ```bash pip install iderare-pheno ``` ### Installing from
 source To install **iderare-pheno** from source, first clone [the repository]
 (https://github.com/ivanwilliammd/iderare-pheno): ```bash git clone https://
 github.com/ivanwilliammd/iderare-pheno.git cd iderare_pheno ``` Then run
-```bash pip install -e . ``` ## Usage ```python from iderare_pheno.converter
-import term2omim, term2orpha, term2hpo, batchconvert from iderare_pheno.simrec
-import hpo2omim_similarity, omim_recommendation, hpo2name from
-iderare_pheno.utils import linkage_dendrogram, list2tsv ``` ## Team **iderare-
-pheno** is developed and maintained by the author(s), To learn more about who
-specifically contributed to this codebase, see [our contributors](https://
-github.com/ivanwilliammd/iderare-pheno/graphs/contributors) page. ## License
-**iderare-pheno** license is derived from [IDeRare](https://github.com/
-ivanwilliammd/iderare)
+```bash pip install -e . ``` ## Importing the library ```python from
+iderare_pheno.converter import term2omim, term2orpha, term2hpo, batchconvert
+from iderare_pheno.simrec import hpo2omim_similarity, omim_recommendation,
+hpo2name from iderare_pheno.utils import linkage_dendrogram, list2tsv,
+generate_yml ``` As the complete readthedocs.io is still ongoing, please kindly
+refer to this [Interactive Playbook Example](https://github.com/ivanwilliammd/
+iderare-pheno/blob/main/Playbook.ipynb) ## Team **iderare-pheno** is developed
+and maintained by the author(s), To learn more about who specifically
+contributed to this codebase, see [our contributors](https://github.com/
+ivanwilliammd/iderare-pheno/graphs/contributors) page. ## License **iderare-
+pheno** license is derived from [IDeRare](https://github.com/ivanwilliammd/
+iderare)
```

### Comparing `iderare-pheno-0.4.0/iderare_pheno/converter.py` & `iderare-pheno-0.5.0/iderare_pheno/converter.py`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.4.0/iderare_pheno/phenotype/data/genes_to_phenotype.txt` & `iderare-pheno-0.5.0/iderare_pheno/phenotype/data/genes_to_phenotype.txt`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.4.0/iderare_pheno/phenotype/data/hp.obo` & `iderare-pheno-0.5.0/iderare_pheno/phenotype/data/hp.obo`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.4.0/iderare_pheno/phenotype/data/phenotype.hpoa` & `iderare-pheno-0.5.0/iderare_pheno/phenotype/data/phenotype.hpoa`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.4.0/iderare_pheno/phenotype/subset/icd102omim_subset.tsv` & `iderare-pheno-0.5.0/iderare_pheno/phenotype/subset/icd102omim_subset.tsv`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.4.0/iderare_pheno/phenotype/subset/loinc2hpo_standardized.tsv` & `iderare-pheno-0.5.0/iderare_pheno/phenotype/subset/loinc2hpo_standardized.tsv`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.4.0/iderare_pheno/phenotype/subset/omim2hpo_subset.tsv` & `iderare-pheno-0.5.0/iderare_pheno/phenotype/subset/omim2hpo_subset.tsv`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.4.0/iderare_pheno/phenotype/subset/orpha2hpo_subset.tsv` & `iderare-pheno-0.5.0/iderare_pheno/phenotype/subset/orpha2hpo_subset.tsv`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.4.0/iderare_pheno/phenotype/subset/orpha2omim_subset.tsv` & `iderare-pheno-0.5.0/iderare_pheno/phenotype/subset/orpha2omim_subset.tsv`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.4.0/iderare_pheno/phenotype/subset/snomed2hpo_subset.tsv` & `iderare-pheno-0.5.0/iderare_pheno/phenotype/subset/snomed2hpo_subset.tsv`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.4.0/iderare_pheno/phenotype/subset/snomed2orpha_subset.tsv` & `iderare-pheno-0.5.0/iderare_pheno/phenotype/subset/snomed2orpha_subset.tsv`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.4.0/iderare_pheno/simrec.py` & `iderare-pheno-0.5.0/iderare_pheno/simrec.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,18 +24,23 @@
     hpo_object = HPOSet.from_queries(list(set(hpo_set)))
     return hpo_object
 
 
 # Get HPO Name from HPO Code
 def hpo2name(hpo_set):
     hpo_name = [Ontology.hpo(int(d.strip("HP:"))).name for d in hpo_set]
-
     return hpo_name
 
 
+# Get OMIM Name from HPO Code
+def omim2name(diagnosis_sets):
+    omim_name = [Omim.get(int(d.strip("OMIM:"))).name for d in diagnosis_sets]
+    return omim_name
+
+
 # Threshold similarity
 def similarity_linkage(omim_sets, hpo_sets, threshold=0.3, differential=10, linkage="both"):
 
     # Split into names, sets
     print("Splitting process done")
     omim_id = [d[0] for d in omim_sets]
     omim_names = [d[1] for d in omim_sets]
```

### Comparing `iderare-pheno-0.4.0/iderare_pheno/templates/template_iderare.yml` & `iderare-pheno-0.5.0/iderare_pheno/templates/template_iderare.yml`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.4.0/iderare_pheno/utils.py` & `iderare-pheno-0.5.0/iderare_pheno/utils.py`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.4.0/iderare_pheno.egg-info/PKG-INFO` & `iderare-pheno-0.5.0/iderare_pheno.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iderare-pheno
-Version: 0.4.0
+Version: 0.5.0
 Author-email: Ivan William Harsono <ivanwilliam.md@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Ivan William Harsono
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
@@ -32,15 +32,15 @@
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
 Project-URL: Homepage, https://github.com/ivanwilliammd/iderare-pheno
 Project-URL: Repository, https://github.com/ivanwilliammd/iderare-pheno
 Project-URL: Changelog, https://github.com/ivanwilliammd/iderare-pheno/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://iderare-pheno.readthedocs.io/
 Classifier: Intended Audience :: Science/Research
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas
@@ -70,19 +70,14 @@
 Requires-Dist: sphinx-copybutton==0.5.2; extra == "dev"
 Requires-Dist: sphinx-autobuild==2021.3.14; extra == "dev"
 Requires-Dist: sphinx-autodoc-typehints==1.23.3; extra == "dev"
 Requires-Dist: packaging; extra == "dev"
 
 # [IDeRare-Pheno](https://iderare-pheno.readthedocs.io/)
 
-<!-- start tagline -->
-
-IDeRare or "Indonesia Exome Rare Disease Variant Discovery Pipeline" is simple and ready to use variant discovery pipeline to discover rare disease variants from exome sequencing data.
-<!-- end tagline -->
-
 <p align="center">
     <a href="https://github.com/ivanwilliammd/iderare-pheno/actions">
         <img alt="CI" src="https://github.com/ivanwilliammd/iderare-pheno/workflows/Main/badge.svg">
     </a>
     <a href="https://pypi.org/project/iderare_pheno/">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/iderare_pheno">
     </a>
@@ -93,19 +88,39 @@
         <img alt="License" src="https://img.shields.io/github/license/ivanwilliammd/iderare-pheno.svg?color=blue&cachedrop">
     </a>
     <a href="https://bioinformatics-ivanwilliamharsono.streamlit.app/IDeRare_Pheno">
         <img alt="Streamlit" src="https://static.streamlit.io/badges/streamlit_badge_black_white.svg">
     <br/>
 </p>
 
+IDeRare or "Indonesia Exome Rare Disease Variant Discovery Pipeline" is a simple and ready to use variant discovery pipeline to discover rare disease variants from exome sequencing data. 
+
+This repository is **the first part** of IDeRare workflow for **phenotype analysis**. For complete pipeline for _**phenotype-genotype analysis**_, kindly refer to [IDeRare Github repository](https://github.com/ivanwilliammd/IDeRare).
+
+## Authored by 
+Ivan William Harsono<sup>a</sup>, Yulia Ariani<sup>b</sup>, Beben Benyamin<sup>c,d,e</sup>, Fadilah Fadilah<sup>f,g</sup>, Dwi Ari Pujianto<sup>b</sup>, Cut Nurul Hafifah<sup>h</sup>
+
+<sup>a</sup>Doctoral Program in Biomedical Sciences, Faculty of Medicine, Universitas Indonesia, Jakarta, Indonesia.<br> 
+<sup>b</sup>Department of Medical Biology, Faculty of Medicine, Universitas Indonesia, Jakarta, Indonesia.<br> 
+<sup>c</sup>Australian Centre for Precision Health, University of South Australia, Adelaide, SA, 5000, Australia. <br>
+<sup>d</sup>UniSA Allied Health and Human Performance, University of South Australia, Adelaide, SA, 5000, Australia. <br>
+<sup>e</sup>South Australian Health and Medical Research Institute (SAHMRI), University of South Australia, Adelaide, SA, 5000, Australia. <br>
+<sup>f</sup>Department of Medical Chemistry, Faculty of Medicine, Universitas Indonesia, Jalan Salemba Raya number 4, Jakarta, 10430, Indonesia.<br>
+<sup>g</sup>Bioinformatics Core Facilities - IMERI, Faculty of Medicine, Universitas Indonesia, Jalan Salemba Raya number 6, Jakarta, 10430, Indonesia .<br>
+<sup>h</sup>Department of Child Health, Dr. Cipto Mangunkusumo Hospital, Faculty of Medicine, University of Indonesia, Jakarta, Indonesia. <br>
+
+
+**Note:** Currently IDeRare paper is being considered journal submission. The citation will be updated once the paper is published.
+
 ## Quick links
 
 - [Documentation](https://iderare-pheno.readthedocs.io/)
 - [PyPI Package](https://pypi.org/project/iderare-pheno/)
 - [License](https://github.com/ivanwilliammd/iderare-pheno/blob/main/LICENSE)
+- [Interactive Playbook Example](https://github.com/ivanwilliammd/iderare-pheno/blob/main/Playbook.ipynb)
 - Interactive Webapps Implementation of at [Streamlit](https://bioinformatics-ivanwilliamharsono.streamlitapp.com/IDeRare_Pheno)
 
 
 ## What does it do?
 
 This script is recommended if you would like to do conversion, linkage analysis, similarity scoring, and gene-disease recommendation based on the phenotype data provided at [clinical_data.txt](clinical_data.txt). Full feature : 
 1. Convert the phenotype data to HPO code (accept mixed SNOMED, LOINC, and HPO code)
@@ -153,21 +168,23 @@
 
 ```bash
 pip install -e .
 ```
 
 <!-- end install source -->
 
-## Usage
+## Importing the library
 
 ```python
 from iderare_pheno.converter import term2omim, term2orpha, term2hpo, batchconvert
 from iderare_pheno.simrec import hpo2omim_similarity, omim_recommendation, hpo2name
-from iderare_pheno.utils import linkage_dendrogram, list2tsv
+from iderare_pheno.utils import linkage_dendrogram, list2tsv, generate_yml
 ```
+As the complete readthedocs.io is still ongoing, please kindly refer to this [Interactive Playbook Example](https://github.com/ivanwilliammd/iderare-pheno/blob/main/Playbook.ipynb)
+
 
 ## Team
 
 <!-- start team -->
 
 **iderare-pheno** is developed and maintained by the author(s), To learn more about who specifically contributed to this codebase, see [our contributors](https://github.com/ivanwilliammd/iderare-pheno/graphs/contributors) page.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: iderare-pheno Version: 0.4.0 Author-email: Ivan
+Metadata-Version: 2.1 Name: iderare-pheno Version: 0.5.0 Author-email: Ivan
 William Harsono
 gmail.com> License: BSD 3-Clause License Copyright (c) 2024, Ivan William
 Harsono Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met: 1.
 Redistributions of source code must retain the above copyright notice, this
 list of conditions and the following disclaimer. 2. Redistributions in binary
 form must reproduce the above copyright notice, this list of conditions and the
@@ -20,42 +20,65 @@
 LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 ADVISED OF THE POSSIBILITY OF SUCH DAMAGE. Project-URL: Homepage, https://
 github.com/ivanwilliammd/iderare-pheno Project-URL: Repository, https://
 github.com/ivanwilliammd/iderare-pheno Project-URL: Changelog, https://
 github.com/ivanwilliammd/iderare-pheno/blob/main/CHANGELOG.md Project-URL:
 Documentation, https://iderare-pheno.readthedocs.io/ Classifier: Intended
-Audience :: Science/Research Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: BSD License Classifier: Programming
-Language :: Python :: 3 Classifier: Topic :: Scientific/Engineering :: Medical
-Science Apps. Requires-Python: >=3.8 Description-Content-Type: text/markdown
-License-File: LICENSE Requires-Dist: pandas Requires-Dist: numpy Requires-Dist:
-matplotlib Requires-Dist: scipy Requires-Dist: hpo3 Requires-Dist: scikit-learn
-Requires-Dist: pyyaml Provides-Extra: dev Requires-Dist: ruff; extra == "dev"
-Requires-Dist: mypy<1.10,>=1.0; extra == "dev" Requires-Dist: types-PyYAML;
-extra == "dev" Requires-Dist: black<25.0,>=23.0; extra == "dev" Requires-Dist:
-black[jupyter]; extra == "dev" Requires-Dist: isort<5.14,>=5.12; extra == "dev"
-Requires-Dist: pytest; extra == "dev" Requires-Dist: pytest-sphinx; extra ==
-"dev" Requires-Dist: pytest-cov; extra == "dev" Requires-Dist: twine>=1.11.0;
-extra == "dev" Requires-Dist: build; extra == "dev" Requires-Dist: setuptools;
-extra == "dev" Requires-Dist: wheel; extra == "dev" Requires-Dist:
-Sphinx<7.3.0,>=4.3.0; extra == "dev" Requires-Dist: furo==2024.1.29; extra ==
-"dev" Requires-Dist: myst-parser<2.1,>=1.0; extra == "dev" Requires-Dist:
-sphinx-copybutton==0.5.2; extra == "dev" Requires-Dist: sphinx-
-autobuild==2021.3.14; extra == "dev" Requires-Dist: sphinx-autodoc-
-typehints==1.23.3; extra == "dev" Requires-Dist: packaging; extra == "dev" #
-[IDeRare-Pheno](https://iderare-pheno.readthedocs.io/) IDeRare or "Indonesia
-Exome Rare Disease Variant Discovery Pipeline" is simple and ready to use
-variant discovery pipeline to discover rare disease variants from exome
-sequencing data.
+Audience :: Science/Research Classifier: Development Status :: 5 - Production/
+Stable Classifier: License :: OSI Approved :: BSD License Classifier:
+Programming Language :: Python :: 3 Classifier: Topic :: Scientific/Engineering
+:: Medical Science Apps. Requires-Python: >=3.8 Description-Content-Type: text/
+markdown License-File: LICENSE Requires-Dist: pandas Requires-Dist: numpy
+Requires-Dist: matplotlib Requires-Dist: scipy Requires-Dist: hpo3 Requires-
+Dist: scikit-learn Requires-Dist: pyyaml Provides-Extra: dev Requires-Dist:
+ruff; extra == "dev" Requires-Dist: mypy<1.10,>=1.0; extra == "dev" Requires-
+Dist: types-PyYAML; extra == "dev" Requires-Dist: black<25.0,>=23.0; extra ==
+"dev" Requires-Dist: black[jupyter]; extra == "dev" Requires-Dist:
+isort<5.14,>=5.12; extra == "dev" Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-sphinx; extra == "dev" Requires-Dist: pytest-cov; extra
+== "dev" Requires-Dist: twine>=1.11.0; extra == "dev" Requires-Dist: build;
+extra == "dev" Requires-Dist: setuptools; extra == "dev" Requires-Dist: wheel;
+extra == "dev" Requires-Dist: Sphinx<7.3.0,>=4.3.0; extra == "dev" Requires-
+Dist: furo==2024.1.29; extra == "dev" Requires-Dist: myst-parser<2.1,>=1.0;
+extra == "dev" Requires-Dist: sphinx-copybutton==0.5.2; extra == "dev"
+Requires-Dist: sphinx-autobuild==2021.3.14; extra == "dev" Requires-Dist:
+sphinx-autodoc-typehints==1.23.3; extra == "dev" Requires-Dist: packaging;
+extra == "dev" # [IDeRare-Pheno](https://iderare-pheno.readthedocs.io/)
              _[_C_I_]_[_P_y_P_I_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_L_i_c_e_n_s_e_]_[_S_t_r_e_a_m_l_i_t_]
-## Quick links - [Documentation](https://iderare-pheno.readthedocs.io/) - [PyPI
-Package](https://pypi.org/project/iderare-pheno/) - [License](https://
-github.com/ivanwilliammd/iderare-pheno/blob/main/LICENSE) - Interactive Webapps
-Implementation of at [Streamlit](https://bioinformatics-
+IDeRare or "Indonesia Exome Rare Disease Variant Discovery Pipeline" is a
+simple and ready to use variant discovery pipeline to discover rare disease
+variants from exome sequencing data. This repository is **the first part** of
+IDeRare workflow for **phenotype analysis**. For complete pipeline for
+_**phenotype-genotype analysis**_, kindly refer to [IDeRare Github repository]
+(https://github.com/ivanwilliammd/IDeRare). ## Authored by Ivan William
+Harsonoa, Yulia Arianib, Beben Benyaminc,d,e, Fadilah Fadilahf,g, Dwi Ari
+Pujiantob, Cut Nurul Hafifahh aDoctoral Program in Biomedical Sciences, Faculty
+of Medicine, Universitas Indonesia, Jakarta, Indonesia.
+bDepartment of Medical Biology, Faculty of Medicine, Universitas Indonesia,
+Jakarta, Indonesia.
+cAustralian Centre for Precision Health, University of South Australia,
+Adelaide, SA, 5000, Australia.
+dUniSA Allied Health and Human Performance, University of South Australia,
+Adelaide, SA, 5000, Australia.
+eSouth Australian Health and Medical Research Institute (SAHMRI), University of
+South Australia, Adelaide, SA, 5000, Australia.
+fDepartment of Medical Chemistry, Faculty of Medicine, Universitas Indonesia,
+Jalan Salemba Raya number 4, Jakarta, 10430, Indonesia.
+gBioinformatics Core Facilities - IMERI, Faculty of Medicine, Universitas
+Indonesia, Jalan Salemba Raya number 6, Jakarta, 10430, Indonesia .
+hDepartment of Child Health, Dr. Cipto Mangunkusumo Hospital, Faculty of
+Medicine, University of Indonesia, Jakarta, Indonesia.
+**Note:** Currently IDeRare paper is being considered journal submission. The
+citation will be updated once the paper is published. ## Quick links -
+[Documentation](https://iderare-pheno.readthedocs.io/) - [PyPI Package](https:/
+/pypi.org/project/iderare-pheno/) - [License](https://github.com/ivanwilliammd/
+iderare-pheno/blob/main/LICENSE) - [Interactive Playbook Example](https://
+github.com/ivanwilliammd/iderare-pheno/blob/main/Playbook.ipynb) - Interactive
+Webapps Implementation of at [Streamlit](https://bioinformatics-
 ivanwilliamharsono.streamlitapp.com/IDeRare_Pheno) ## What does it do? This
 script is recommended if you would like to do conversion, linkage analysis,
 similarity scoring, and gene-disease recommendation based on the phenotype data
 provided at [clinical_data.txt](clinical_data.txt). Full feature : 1. Convert
 the phenotype data to HPO code (accept mixed SNOMED, LOINC, and HPO code) 2.
 Similarity scoring of differential diagnosis 3. Linkage analysis of
 differential diagnosis (accept mixed SNOMED, ICD-10, ORPHA, OMIM code), include
@@ -70,16 +93,19 @@
 Information Example section](#clinical-information-example) ## Installation
 **iderare-pheno** requires Python 3.8 or later. ### Installing with `pip`
 **iderare-pheno** is available [on PyPI](https://pypi.org/project/iderare-
 pheno/). Just run ```bash pip install iderare-pheno ``` ### Installing from
 source To install **iderare-pheno** from source, first clone [the repository]
 (https://github.com/ivanwilliammd/iderare-pheno): ```bash git clone https://
 github.com/ivanwilliammd/iderare-pheno.git cd iderare_pheno ``` Then run
-```bash pip install -e . ``` ## Usage ```python from iderare_pheno.converter
-import term2omim, term2orpha, term2hpo, batchconvert from iderare_pheno.simrec
-import hpo2omim_similarity, omim_recommendation, hpo2name from
-iderare_pheno.utils import linkage_dendrogram, list2tsv ``` ## Team **iderare-
-pheno** is developed and maintained by the author(s), To learn more about who
-specifically contributed to this codebase, see [our contributors](https://
-github.com/ivanwilliammd/iderare-pheno/graphs/contributors) page. ## License
-**iderare-pheno** license is derived from [IDeRare](https://github.com/
-ivanwilliammd/iderare)
+```bash pip install -e . ``` ## Importing the library ```python from
+iderare_pheno.converter import term2omim, term2orpha, term2hpo, batchconvert
+from iderare_pheno.simrec import hpo2omim_similarity, omim_recommendation,
+hpo2name from iderare_pheno.utils import linkage_dendrogram, list2tsv,
+generate_yml ``` As the complete readthedocs.io is still ongoing, please kindly
+refer to this [Interactive Playbook Example](https://github.com/ivanwilliammd/
+iderare-pheno/blob/main/Playbook.ipynb) ## Team **iderare-pheno** is developed
+and maintained by the author(s), To learn more about who specifically
+contributed to this codebase, see [our contributors](https://github.com/
+ivanwilliammd/iderare-pheno/graphs/contributors) page. ## License **iderare-
+pheno** license is derived from [IDeRare](https://github.com/ivanwilliammd/
+iderare)
```

### Comparing `iderare-pheno-0.4.0/iderare_pheno.egg-info/SOURCES.txt` & `iderare-pheno-0.5.0/iderare_pheno.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 pyproject.toml
 iderare_pheno/__init__.py
 iderare_pheno/converter.py
 iderare_pheno/py.typed
 iderare_pheno/simrec.py
+iderare_pheno/streamlit_utils.py
 iderare_pheno/utils.py
 iderare_pheno/version.py
 iderare_pheno.egg-info/PKG-INFO
 iderare_pheno.egg-info/SOURCES.txt
 iderare_pheno.egg-info/dependency_links.txt
 iderare_pheno.egg-info/requires.txt
 iderare_pheno.egg-info/top_level.txt
```

### Comparing `iderare-pheno-0.4.0/pyproject.toml` & `iderare-pheno-0.5.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 # See https://setuptools.pypa.io/en/latest/userguide/quickstart.html for more project configuration options.
 name = "iderare-pheno"
 dynamic = ["version"]
 readme = "README.md"
 classifiers = [
     "Intended Audience :: Science/Research",
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering :: Medical Science Apps.",
 ]
 authors = [
     {name = "Ivan William Harsono", email = "ivanwilliam.md@gmail.com"}
 ]
```

