# Comparing `tmp/PyTDC-0.4.6.tar.gz` & `tmp/PyTDC-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyTDC-0.4.6.tar", last modified: Sat Mar 23 21:31:55 2024, max compression
+gzip compressed data, was "PyTDC-0.4.7.tar", last modified: Tue Apr  9 21:38:42 2024, max compression
```

## Comparing `PyTDC-0.4.6.tar` & `PyTDC-0.4.7.tar`

### file list

```diff
@@ -1,107 +1,112 @@
-drwxr-xr-x   0 alejandrovelez-arce   (501) staff       (20)        0 2024-03-23 21:31:55.101646 PyTDC-0.4.6/
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1069 2024-03-01 19:46:57.000000 PyTDC-0.4.6/LICENSE
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      102 2024-03-01 19:46:57.000000 PyTDC-0.4.6/MANIFEST.in
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    19276 2024-03-23 21:31:55.101363 PyTDC-0.4.6/PKG-INFO
-drwxr-xr-x   0 alejandrovelez-arce   (501) staff       (20)        0 2024-03-23 21:31:55.099871 PyTDC-0.4.6/PyTDC.egg-info/
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    19276 2024-03-23 21:31:54.000000 PyTDC-0.4.6/PyTDC.egg-info/PKG-INFO
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     2550 2024-03-23 21:31:54.000000 PyTDC-0.4.6/PyTDC.egg-info/SOURCES.txt
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)        1 2024-03-23 21:31:54.000000 PyTDC-0.4.6/PyTDC.egg-info/dependency_links.txt
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)        1 2024-03-23 19:33:04.000000 PyTDC-0.4.6/PyTDC.egg-info/not-zip-safe
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      315 2024-03-23 21:31:54.000000 PyTDC-0.4.6/PyTDC.egg-info/requires.txt
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)        4 2024-03-23 21:31:54.000000 PyTDC-0.4.6/PyTDC.egg-info/top_level.txt
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    18401 2024-03-23 16:49:43.000000 PyTDC-0.4.6/README.md
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      316 2024-03-23 19:58:07.000000 PyTDC-0.4.6/requirements.txt
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)       79 2024-03-23 21:31:55.102431 PyTDC-0.4.6/setup.cfg
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1160 2024-03-23 19:32:47.000000 PyTDC-0.4.6/setup.py
-drwxr-xr-x   0 alejandrovelez-arce   (501) staff       (20)        0 2024-03-23 21:31:55.049713 PyTDC-0.4.6/tdc/
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      199 2024-03-17 21:08:33.000000 PyTDC-0.4.6/tdc/__init__.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     7852 2024-03-07 18:03:45.000000 PyTDC-0.4.6/tdc/base_dataset.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    22305 2024-03-07 18:03:45.000000 PyTDC-0.4.6/tdc/benchmark_deprecated.py
-drwxr-xr-x   0 alejandrovelez-arce   (501) staff       (20)        0 2024-03-23 21:31:55.053569 PyTDC-0.4.6/tdc/benchmark_group/
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      162 2024-03-01 19:46:57.000000 PyTDC-0.4.6/tdc/benchmark_group/__init__.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      449 2024-03-05 15:50:55.000000 PyTDC-0.4.6/tdc/benchmark_group/admet_group.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    10499 2024-03-07 18:03:45.000000 PyTDC-0.4.6/tdc/benchmark_group/base_group.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    16066 2024-03-07 18:03:45.000000 PyTDC-0.4.6/tdc/benchmark_group/docking_group.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      775 2024-03-07 18:03:45.000000 PyTDC-0.4.6/tdc/benchmark_group/drugcombo_group.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      453 2024-03-05 15:52:54.000000 PyTDC-0.4.6/tdc/benchmark_group/dti_dg_group.py
-drwxr-xr-x   0 alejandrovelez-arce   (501) staff       (20)        0 2024-03-23 21:31:55.055294 PyTDC-0.4.6/tdc/chem_utils/
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1021 2024-03-01 19:46:57.000000 PyTDC-0.4.6/tdc/chem_utils/__init__.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    14100 2024-03-07 18:03:45.000000 PyTDC-0.4.6/tdc/chem_utils/evaluator.py
-drwxr-xr-x   0 alejandrovelez-arce   (501) staff       (20)        0 2024-03-23 21:31:55.057898 PyTDC-0.4.6/tdc/chem_utils/featurize/
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)        0 2024-03-01 19:46:57.000000 PyTDC-0.4.6/tdc/chem_utils/featurize/__init__.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    28488 2024-03-05 15:54:24.000000 PyTDC-0.4.6/tdc/chem_utils/featurize/_smartsPatts.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    23821 2024-03-07 18:03:45.000000 PyTDC-0.4.6/tdc/chem_utils/featurize/_smiles2pubchem.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    22094 2024-03-07 18:03:45.000000 PyTDC-0.4.6/tdc/chem_utils/featurize/_xyz2mol.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    27277 2024-03-07 18:03:45.000000 PyTDC-0.4.6/tdc/chem_utils/featurize/molconvert.py
-drwxr-xr-x   0 alejandrovelez-arce   (501) staff       (20)        0 2024-03-23 21:31:55.059621 PyTDC-0.4.6/tdc/chem_utils/oracle/
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)        0 2024-03-01 19:46:57.000000 PyTDC-0.4.6/tdc/chem_utils/oracle/__init__.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1134 2024-03-07 18:03:45.000000 PyTDC-0.4.6/tdc/chem_utils/oracle/docking.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     6083 2024-03-07 18:03:45.000000 PyTDC-0.4.6/tdc/chem_utils/oracle/filter.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    61143 2024-03-07 18:03:45.000000 PyTDC-0.4.6/tdc/chem_utils/oracle/oracle.py
-drwxr-xr-x   0 alejandrovelez-arce   (501) staff       (20)        0 2024-03-23 21:31:55.061500 PyTDC-0.4.6/tdc/dataset_configs/
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      109 2024-03-23 16:49:30.000000 PyTDC-0.4.6/tdc/dataset_configs/__init__.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     2208 2024-03-23 16:49:30.000000 PyTDC-0.4.6/tdc/dataset_configs/config.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1093 2024-03-23 16:49:30.000000 PyTDC-0.4.6/tdc/dataset_configs/pentelute_mdm2_ace2_12ca5_config.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    15896 2024-03-07 18:03:45.000000 PyTDC-0.4.6/tdc/evaluator.py
-drwxr-xr-x   0 alejandrovelez-arce   (501) staff       (20)        0 2024-03-23 21:31:55.063106 PyTDC-0.4.6/tdc/feature_generators/
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)        0 2024-03-23 20:10:21.000000 PyTDC-0.4.6/tdc/feature_generators/__init__.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     4055 2024-03-23 16:49:30.000000 PyTDC-0.4.6/tdc/feature_generators/data_feature_generator.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     7504 2024-03-23 16:49:30.000000 PyTDC-0.4.6/tdc/feature_generators/protein_feature_generator.py
-drwxr-xr-x   0 alejandrovelez-arce   (501) staff       (20)        0 2024-03-23 21:31:55.067687 PyTDC-0.4.6/tdc/generation/
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      112 2024-03-01 19:46:57.000000 PyTDC-0.4.6/tdc/generation/__init__.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     3826 2024-03-07 18:03:45.000000 PyTDC-0.4.6/tdc/generation/bi_generation_dataset.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     9977 2024-03-07 18:03:45.000000 PyTDC-0.4.6/tdc/generation/generation_dataset.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      816 2024-03-07 18:03:45.000000 PyTDC-0.4.6/tdc/generation/ligandmolgen.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1060 2024-03-07 18:03:45.000000 PyTDC-0.4.6/tdc/generation/molgen.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1146 2024-03-07 18:03:45.000000 PyTDC-0.4.6/tdc/generation/reaction.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     2470 2024-03-07 18:03:45.000000 PyTDC-0.4.6/tdc/generation/retrosyn.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     5805 2024-03-07 18:03:45.000000 PyTDC-0.4.6/tdc/generation/sbdd.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    28189 2024-03-23 16:49:30.000000 PyTDC-0.4.6/tdc/metadata.py
-drwxr-xr-x   0 alejandrovelez-arce   (501) staff       (20)        0 2024-03-23 21:31:55.081971 PyTDC-0.4.6/tdc/multi_pred/
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      430 2024-03-23 16:49:30.000000 PyTDC-0.4.6/tdc/multi_pred/__init__.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1491 2024-03-07 18:03:45.000000 PyTDC-0.4.6/tdc/multi_pred/antibodyaff.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    13985 2024-03-23 16:49:30.000000 PyTDC-0.4.6/tdc/multi_pred/bi_pred_dataset.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1481 2024-03-07 18:03:45.000000 PyTDC-0.4.6/tdc/multi_pred/catalyst.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     2062 2024-03-07 18:03:45.000000 PyTDC-0.4.6/tdc/multi_pred/ddi.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     2031 2024-03-07 18:03:45.000000 PyTDC-0.4.6/tdc/multi_pred/drugres.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1291 2024-03-07 18:03:45.000000 PyTDC-0.4.6/tdc/multi_pred/drugsyn.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     2987 2024-03-07 18:03:45.000000 PyTDC-0.4.6/tdc/multi_pred/dti.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1534 2024-03-07 18:03:45.000000 PyTDC-0.4.6/tdc/multi_pred/gda.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1579 2024-03-07 18:03:45.000000 PyTDC-0.4.6/tdc/multi_pred/mti.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     4056 2024-03-07 18:03:45.000000 PyTDC-0.4.6/tdc/multi_pred/multi_pred_dataset.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1544 2024-03-07 18:03:45.000000 PyTDC-0.4.6/tdc/multi_pred/peptidemhc.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     2085 2024-03-07 18:03:45.000000 PyTDC-0.4.6/tdc/multi_pred/ppi.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1819 2024-03-23 16:49:30.000000 PyTDC-0.4.6/tdc/multi_pred/proteinpeptide.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1305 2024-03-07 18:03:45.000000 PyTDC-0.4.6/tdc/multi_pred/tcr_epi.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1163 2024-03-07 18:03:45.000000 PyTDC-0.4.6/tdc/multi_pred/test_multi_pred.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1616 2024-03-07 18:03:45.000000 PyTDC-0.4.6/tdc/multi_pred/trialoutcome.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    25828 2024-03-07 18:03:45.000000 PyTDC-0.4.6/tdc/oracles.py
-drwxr-xr-x   0 alejandrovelez-arce   (501) staff       (20)        0 2024-03-23 21:31:55.083764 PyTDC-0.4.6/tdc/resource/
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)       74 2024-03-17 21:08:33.000000 PyTDC-0.4.6/tdc/resource/__init__.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    18591 2024-03-23 21:31:12.000000 PyTDC-0.4.6/tdc/resource/cellxgene_census.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     2613 2024-03-17 21:08:33.000000 PyTDC-0.4.6/tdc/resource/primekg.py
-drwxr-xr-x   0 alejandrovelez-arce   (501) staff       (20)        0 2024-03-23 21:31:55.092911 PyTDC-0.4.6/tdc/single_pred/
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      287 2024-03-01 19:46:57.000000 PyTDC-0.4.6/tdc/single_pred/__init__.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     4229 2024-03-07 18:03:45.000000 PyTDC-0.4.6/tdc/single_pred/adme.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1560 2024-03-07 18:03:45.000000 PyTDC-0.4.6/tdc/single_pred/crispr_outcome.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     5751 2024-03-07 18:03:45.000000 PyTDC-0.4.6/tdc/single_pred/develop.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1554 2024-03-07 18:03:45.000000 PyTDC-0.4.6/tdc/single_pred/epitope.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1473 2024-03-07 18:03:45.000000 PyTDC-0.4.6/tdc/single_pred/hts.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1559 2024-03-07 18:03:45.000000 PyTDC-0.4.6/tdc/single_pred/paratope.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1587 2024-03-07 18:03:45.000000 PyTDC-0.4.6/tdc/single_pred/qm.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     6831 2024-03-07 18:03:45.000000 PyTDC-0.4.6/tdc/single_pred/single_pred_dataset.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1484 2024-03-07 18:03:45.000000 PyTDC-0.4.6/tdc/single_pred/test_single_pred.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1517 2024-03-07 18:03:45.000000 PyTDC-0.4.6/tdc/single_pred/tox.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1583 2024-03-07 18:03:45.000000 PyTDC-0.4.6/tdc/single_pred/yields.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     3594 2024-03-07 18:03:45.000000 PyTDC-0.4.6/tdc/tdc_hf.py
-drwxr-xr-x   0 alejandrovelez-arce   (501) staff       (20)        0 2024-03-23 21:31:55.099243 PyTDC-0.4.6/tdc/utils/
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1232 2024-03-23 16:49:30.000000 PyTDC-0.4.6/tdc/utils/__init__.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      916 2024-03-17 21:08:33.000000 PyTDC-0.4.6/tdc/utils/knowledge_graph.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     9227 2024-03-18 13:44:09.000000 PyTDC-0.4.6/tdc/utils/label.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    19101 2024-03-07 18:03:45.000000 PyTDC-0.4.6/tdc/utils/label_name_list.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    37971 2024-03-23 16:49:30.000000 PyTDC-0.4.6/tdc/utils/load.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     3438 2024-03-07 18:03:45.000000 PyTDC-0.4.6/tdc/utils/misc.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     3114 2024-03-07 18:03:45.000000 PyTDC-0.4.6/tdc/utils/query.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     3576 2024-03-07 18:03:45.000000 PyTDC-0.4.6/tdc/utils/retrieve.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    13042 2024-03-07 18:03:45.000000 PyTDC-0.4.6/tdc/utils/split.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      535 2024-03-23 21:31:48.000000 PyTDC-0.4.6/tdc/version.py
+drwxr-xr-x   0 alejandrovelez-arce   (501) staff       (20)        0 2024-04-09 21:38:42.278674 PyTDC-0.4.7/
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1069 2024-03-01 19:46:57.000000 PyTDC-0.4.7/LICENSE
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      102 2024-03-01 19:46:57.000000 PyTDC-0.4.7/MANIFEST.in
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    19276 2024-04-09 21:38:42.278515 PyTDC-0.4.7/PKG-INFO
+drwxr-xr-x   0 alejandrovelez-arce   (501) staff       (20)        0 2024-04-09 21:38:42.277244 PyTDC-0.4.7/PyTDC.egg-info/
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    19276 2024-04-09 21:38:42.000000 PyTDC-0.4.7/PyTDC.egg-info/PKG-INFO
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     2733 2024-04-09 21:38:42.000000 PyTDC-0.4.7/PyTDC.egg-info/SOURCES.txt
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)        1 2024-04-09 21:38:42.000000 PyTDC-0.4.7/PyTDC.egg-info/dependency_links.txt
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)        1 2024-04-09 21:37:01.000000 PyTDC-0.4.7/PyTDC.egg-info/not-zip-safe
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      315 2024-04-09 21:38:42.000000 PyTDC-0.4.7/PyTDC.egg-info/requires.txt
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)        4 2024-04-09 21:38:42.000000 PyTDC-0.4.7/PyTDC.egg-info/top_level.txt
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    18401 2024-03-23 16:49:43.000000 PyTDC-0.4.7/README.md
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      316 2024-04-09 21:38:13.000000 PyTDC-0.4.7/requirements.txt
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)       79 2024-04-09 21:38:42.279175 PyTDC-0.4.7/setup.cfg
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1160 2024-03-25 19:24:21.000000 PyTDC-0.4.7/setup.py
+drwxr-xr-x   0 alejandrovelez-arce   (501) staff       (20)        0 2024-04-09 21:38:42.245178 PyTDC-0.4.7/tdc/
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      199 2024-03-17 21:08:33.000000 PyTDC-0.4.7/tdc/__init__.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     7852 2024-03-07 18:03:45.000000 PyTDC-0.4.7/tdc/base_dataset.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    22305 2024-03-07 18:03:45.000000 PyTDC-0.4.7/tdc/benchmark_deprecated.py
+drwxr-xr-x   0 alejandrovelez-arce   (501) staff       (20)        0 2024-04-09 21:38:42.247438 PyTDC-0.4.7/tdc/benchmark_group/
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      162 2024-03-01 19:46:57.000000 PyTDC-0.4.7/tdc/benchmark_group/__init__.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      449 2024-03-05 15:50:55.000000 PyTDC-0.4.7/tdc/benchmark_group/admet_group.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    10499 2024-03-07 18:03:45.000000 PyTDC-0.4.7/tdc/benchmark_group/base_group.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    16066 2024-03-07 18:03:45.000000 PyTDC-0.4.7/tdc/benchmark_group/docking_group.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      775 2024-03-07 18:03:45.000000 PyTDC-0.4.7/tdc/benchmark_group/drugcombo_group.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      453 2024-03-05 15:52:54.000000 PyTDC-0.4.7/tdc/benchmark_group/dti_dg_group.py
+drwxr-xr-x   0 alejandrovelez-arce   (501) staff       (20)        0 2024-04-09 21:38:42.248386 PyTDC-0.4.7/tdc/chem_utils/
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1021 2024-03-01 19:46:57.000000 PyTDC-0.4.7/tdc/chem_utils/__init__.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    14100 2024-03-07 18:03:45.000000 PyTDC-0.4.7/tdc/chem_utils/evaluator.py
+drwxr-xr-x   0 alejandrovelez-arce   (501) staff       (20)        0 2024-04-09 21:38:42.251009 PyTDC-0.4.7/tdc/chem_utils/featurize/
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)        0 2024-03-01 19:46:57.000000 PyTDC-0.4.7/tdc/chem_utils/featurize/__init__.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    28488 2024-03-05 15:54:24.000000 PyTDC-0.4.7/tdc/chem_utils/featurize/_smartsPatts.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    23821 2024-03-07 18:03:45.000000 PyTDC-0.4.7/tdc/chem_utils/featurize/_smiles2pubchem.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    22094 2024-03-07 18:03:45.000000 PyTDC-0.4.7/tdc/chem_utils/featurize/_xyz2mol.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    27277 2024-03-07 18:03:45.000000 PyTDC-0.4.7/tdc/chem_utils/featurize/molconvert.py
+drwxr-xr-x   0 alejandrovelez-arce   (501) staff       (20)        0 2024-04-09 21:38:42.252694 PyTDC-0.4.7/tdc/chem_utils/oracle/
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)        0 2024-03-01 19:46:57.000000 PyTDC-0.4.7/tdc/chem_utils/oracle/__init__.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1134 2024-03-07 18:03:45.000000 PyTDC-0.4.7/tdc/chem_utils/oracle/docking.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     6083 2024-03-07 18:03:45.000000 PyTDC-0.4.7/tdc/chem_utils/oracle/filter.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    61143 2024-03-07 18:03:45.000000 PyTDC-0.4.7/tdc/chem_utils/oracle/oracle.py
+drwxr-xr-x   0 alejandrovelez-arce   (501) staff       (20)        0 2024-04-09 21:38:42.255057 PyTDC-0.4.7/tdc/dataset_configs/
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      109 2024-03-23 16:49:30.000000 PyTDC-0.4.7/tdc/dataset_configs/__init__.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     2208 2024-03-23 16:49:30.000000 PyTDC-0.4.7/tdc/dataset_configs/config.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      706 2024-04-09 17:21:43.000000 PyTDC-0.4.7/tdc/dataset_configs/config_map.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1093 2024-03-23 16:49:30.000000 PyTDC-0.4.7/tdc/dataset_configs/pentelute_mdm2_ace2_12ca5_config.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      702 2024-04-09 17:21:43.000000 PyTDC-0.4.7/tdc/dataset_configs/scperturb_config.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    15896 2024-03-07 18:03:45.000000 PyTDC-0.4.7/tdc/evaluator.py
+drwxr-xr-x   0 alejandrovelez-arce   (501) staff       (20)        0 2024-04-09 21:38:42.256516 PyTDC-0.4.7/tdc/feature_generators/
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)        0 2024-03-25 19:24:21.000000 PyTDC-0.4.7/tdc/feature_generators/__init__.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1348 2024-04-09 17:21:43.000000 PyTDC-0.4.7/tdc/feature_generators/anndata_to_dataframe.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     4055 2024-03-23 16:49:30.000000 PyTDC-0.4.7/tdc/feature_generators/data_feature_generator.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     7504 2024-03-23 16:49:30.000000 PyTDC-0.4.7/tdc/feature_generators/protein_feature_generator.py
+drwxr-xr-x   0 alejandrovelez-arce   (501) staff       (20)        0 2024-04-09 21:38:42.259533 PyTDC-0.4.7/tdc/generation/
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      112 2024-03-01 19:46:57.000000 PyTDC-0.4.7/tdc/generation/__init__.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     3826 2024-03-07 18:03:45.000000 PyTDC-0.4.7/tdc/generation/bi_generation_dataset.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     9977 2024-03-07 18:03:45.000000 PyTDC-0.4.7/tdc/generation/generation_dataset.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      816 2024-03-07 18:03:45.000000 PyTDC-0.4.7/tdc/generation/ligandmolgen.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1060 2024-03-07 18:03:45.000000 PyTDC-0.4.7/tdc/generation/molgen.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1146 2024-03-07 18:03:45.000000 PyTDC-0.4.7/tdc/generation/reaction.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     2470 2024-03-07 18:03:45.000000 PyTDC-0.4.7/tdc/generation/retrosyn.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     5805 2024-03-07 18:03:45.000000 PyTDC-0.4.7/tdc/generation/sbdd.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    29018 2024-04-09 17:21:43.000000 PyTDC-0.4.7/tdc/metadata.py
+drwxr-xr-x   0 alejandrovelez-arce   (501) staff       (20)        0 2024-04-09 21:38:42.266786 PyTDC-0.4.7/tdc/multi_pred/
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      430 2024-03-23 16:49:30.000000 PyTDC-0.4.7/tdc/multi_pred/__init__.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      727 2024-04-09 17:21:43.000000 PyTDC-0.4.7/tdc/multi_pred/anndata_dataset.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1491 2024-03-07 18:03:45.000000 PyTDC-0.4.7/tdc/multi_pred/antibodyaff.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    13985 2024-04-04 13:31:38.000000 PyTDC-0.4.7/tdc/multi_pred/bi_pred_dataset.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1481 2024-03-07 18:03:45.000000 PyTDC-0.4.7/tdc/multi_pred/catalyst.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      444 2024-04-09 17:21:43.000000 PyTDC-0.4.7/tdc/multi_pred/cellxgene.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     2062 2024-03-07 18:03:45.000000 PyTDC-0.4.7/tdc/multi_pred/ddi.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     2031 2024-03-07 18:03:45.000000 PyTDC-0.4.7/tdc/multi_pred/drugres.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1291 2024-03-07 18:03:45.000000 PyTDC-0.4.7/tdc/multi_pred/drugsyn.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     2987 2024-03-07 18:03:45.000000 PyTDC-0.4.7/tdc/multi_pred/dti.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1534 2024-03-07 18:03:45.000000 PyTDC-0.4.7/tdc/multi_pred/gda.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1579 2024-03-07 18:03:45.000000 PyTDC-0.4.7/tdc/multi_pred/mti.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     4056 2024-03-07 18:03:45.000000 PyTDC-0.4.7/tdc/multi_pred/multi_pred_dataset.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1544 2024-03-07 18:03:45.000000 PyTDC-0.4.7/tdc/multi_pred/peptidemhc.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     2085 2024-03-07 18:03:45.000000 PyTDC-0.4.7/tdc/multi_pred/ppi.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1904 2024-04-09 17:21:43.000000 PyTDC-0.4.7/tdc/multi_pred/proteinpeptide.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1305 2024-03-07 18:03:45.000000 PyTDC-0.4.7/tdc/multi_pred/tcr_epi.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1163 2024-03-07 18:03:45.000000 PyTDC-0.4.7/tdc/multi_pred/test_multi_pred.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1616 2024-03-07 18:03:45.000000 PyTDC-0.4.7/tdc/multi_pred/trialoutcome.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    25828 2024-04-09 20:55:54.000000 PyTDC-0.4.7/tdc/oracles.py
+drwxr-xr-x   0 alejandrovelez-arce   (501) staff       (20)        0 2024-04-09 21:38:42.268171 PyTDC-0.4.7/tdc/resource/
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)       74 2024-03-17 21:08:33.000000 PyTDC-0.4.7/tdc/resource/__init__.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    18591 2024-03-25 19:24:21.000000 PyTDC-0.4.7/tdc/resource/cellxgene_census.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     2613 2024-03-17 21:08:33.000000 PyTDC-0.4.7/tdc/resource/primekg.py
+drwxr-xr-x   0 alejandrovelez-arce   (501) staff       (20)        0 2024-04-09 21:38:42.273069 PyTDC-0.4.7/tdc/single_pred/
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      287 2024-03-01 19:46:57.000000 PyTDC-0.4.7/tdc/single_pred/__init__.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     4229 2024-03-07 18:03:45.000000 PyTDC-0.4.7/tdc/single_pred/adme.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1560 2024-03-07 18:03:45.000000 PyTDC-0.4.7/tdc/single_pred/crispr_outcome.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     5751 2024-03-07 18:03:45.000000 PyTDC-0.4.7/tdc/single_pred/develop.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1554 2024-03-07 18:03:45.000000 PyTDC-0.4.7/tdc/single_pred/epitope.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1473 2024-03-07 18:03:45.000000 PyTDC-0.4.7/tdc/single_pred/hts.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1559 2024-03-07 18:03:45.000000 PyTDC-0.4.7/tdc/single_pred/paratope.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1587 2024-03-07 18:03:45.000000 PyTDC-0.4.7/tdc/single_pred/qm.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     6831 2024-03-07 18:03:45.000000 PyTDC-0.4.7/tdc/single_pred/single_pred_dataset.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1484 2024-03-07 18:03:45.000000 PyTDC-0.4.7/tdc/single_pred/test_single_pred.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1517 2024-03-07 18:03:45.000000 PyTDC-0.4.7/tdc/single_pred/tox.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1583 2024-03-07 18:03:45.000000 PyTDC-0.4.7/tdc/single_pred/yields.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     3594 2024-03-07 18:03:45.000000 PyTDC-0.4.7/tdc/tdc_hf.py
+drwxr-xr-x   0 alejandrovelez-arce   (501) staff       (20)        0 2024-04-09 21:38:42.276728 PyTDC-0.4.7/tdc/utils/
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1232 2024-03-23 16:49:30.000000 PyTDC-0.4.7/tdc/utils/__init__.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      916 2024-03-17 21:08:33.000000 PyTDC-0.4.7/tdc/utils/knowledge_graph.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     9227 2024-03-18 13:44:09.000000 PyTDC-0.4.7/tdc/utils/label.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    19101 2024-03-07 18:03:45.000000 PyTDC-0.4.7/tdc/utils/label_name_list.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    38462 2024-04-09 17:21:43.000000 PyTDC-0.4.7/tdc/utils/load.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     3438 2024-03-07 18:03:45.000000 PyTDC-0.4.7/tdc/utils/misc.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     3114 2024-03-07 18:03:45.000000 PyTDC-0.4.7/tdc/utils/query.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     3576 2024-03-07 18:03:45.000000 PyTDC-0.4.7/tdc/utils/retrieve.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    13042 2024-03-07 18:03:45.000000 PyTDC-0.4.7/tdc/utils/split.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      535 2024-04-09 21:38:34.000000 PyTDC-0.4.7/tdc/version.py
```

### Comparing `PyTDC-0.4.6/LICENSE` & `PyTDC-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/PKG-INFO` & `PyTDC-0.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTDC
-Version: 0.4.6
+Version: 0.4.7
 Summary: Therapeutics Data Commons
 Home-page: https://github.com/mims-harvard/TDC
 Author: TDC Team
 Author-email: alejandro_velez-arce@hms.harvard.edu
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -13,15 +13,15 @@
 Requires-Dist: fuzzywuzzy==0.18.0
 Requires-Dist: huggingface_hub==0.20.3
 Requires-Dist: mygene==3.2.2
 Requires-Dist: numpy==1.26.4
 Requires-Dist: openpyxl==3.0.10
 Requires-Dist: pandas==2.1.4
 Requires-Dist: requests==2.31.0
-Requires-Dist: scikit-learn==1.3.0
+Requires-Dist: scikit-learn==1.2.2
 Requires-Dist: seaborn==0.12.2
 Requires-Dist: tqdm==4.65.0
 Requires-Dist: cellxgene-census==1.10.2
 Requires-Dist: gget==0.28.4
 Requires-Dist: pydantic==2.6.3
 Requires-Dist: gget==0.28.4
 Requires-Dist: rdkit==2023.9.5
```

### Comparing `PyTDC-0.4.6/PyTDC.egg-info/PKG-INFO` & `PyTDC-0.4.7/PyTDC.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTDC
-Version: 0.4.6
+Version: 0.4.7
 Summary: Therapeutics Data Commons
 Home-page: https://github.com/mims-harvard/TDC
 Author: TDC Team
 Author-email: alejandro_velez-arce@hms.harvard.edu
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -13,15 +13,15 @@
 Requires-Dist: fuzzywuzzy==0.18.0
 Requires-Dist: huggingface_hub==0.20.3
 Requires-Dist: mygene==3.2.2
 Requires-Dist: numpy==1.26.4
 Requires-Dist: openpyxl==3.0.10
 Requires-Dist: pandas==2.1.4
 Requires-Dist: requests==2.31.0
-Requires-Dist: scikit-learn==1.3.0
+Requires-Dist: scikit-learn==1.2.2
 Requires-Dist: seaborn==0.12.2
 Requires-Dist: tqdm==4.65.0
 Requires-Dist: cellxgene-census==1.10.2
 Requires-Dist: gget==0.28.4
 Requires-Dist: pydantic==2.6.3
 Requires-Dist: gget==0.28.4
 Requires-Dist: rdkit==2023.9.5
```

### Comparing `PyTDC-0.4.6/PyTDC.egg-info/SOURCES.txt` & `PyTDC-0.4.7/PyTDC.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -33,30 +33,35 @@
 tdc/chem_utils/featurize/molconvert.py
 tdc/chem_utils/oracle/__init__.py
 tdc/chem_utils/oracle/docking.py
 tdc/chem_utils/oracle/filter.py
 tdc/chem_utils/oracle/oracle.py
 tdc/dataset_configs/__init__.py
 tdc/dataset_configs/config.py
+tdc/dataset_configs/config_map.py
 tdc/dataset_configs/pentelute_mdm2_ace2_12ca5_config.py
+tdc/dataset_configs/scperturb_config.py
 tdc/feature_generators/__init__.py
+tdc/feature_generators/anndata_to_dataframe.py
 tdc/feature_generators/data_feature_generator.py
 tdc/feature_generators/protein_feature_generator.py
 tdc/generation/__init__.py
 tdc/generation/bi_generation_dataset.py
 tdc/generation/generation_dataset.py
 tdc/generation/ligandmolgen.py
 tdc/generation/molgen.py
 tdc/generation/reaction.py
 tdc/generation/retrosyn.py
 tdc/generation/sbdd.py
 tdc/multi_pred/__init__.py
+tdc/multi_pred/anndata_dataset.py
 tdc/multi_pred/antibodyaff.py
 tdc/multi_pred/bi_pred_dataset.py
 tdc/multi_pred/catalyst.py
+tdc/multi_pred/cellxgene.py
 tdc/multi_pred/ddi.py
 tdc/multi_pred/drugres.py
 tdc/multi_pred/drugsyn.py
 tdc/multi_pred/dti.py
 tdc/multi_pred/gda.py
 tdc/multi_pred/mti.py
 tdc/multi_pred/multi_pred_dataset.py
```

### Comparing `PyTDC-0.4.6/README.md` & `PyTDC-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/setup.py` & `PyTDC-0.4.7/setup.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/base_dataset.py` & `PyTDC-0.4.7/tdc/base_dataset.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/benchmark_deprecated.py` & `PyTDC-0.4.7/tdc/benchmark_deprecated.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/benchmark_group/base_group.py` & `PyTDC-0.4.7/tdc/benchmark_group/base_group.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/benchmark_group/docking_group.py` & `PyTDC-0.4.7/tdc/benchmark_group/docking_group.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/benchmark_group/drugcombo_group.py` & `PyTDC-0.4.7/tdc/benchmark_group/drugcombo_group.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/chem_utils/__init__.py` & `PyTDC-0.4.7/tdc/chem_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/chem_utils/evaluator.py` & `PyTDC-0.4.7/tdc/chem_utils/evaluator.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/chem_utils/featurize/_smartsPatts.py` & `PyTDC-0.4.7/tdc/chem_utils/featurize/_smartsPatts.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/chem_utils/featurize/_smiles2pubchem.py` & `PyTDC-0.4.7/tdc/chem_utils/featurize/_smiles2pubchem.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/chem_utils/featurize/_xyz2mol.py` & `PyTDC-0.4.7/tdc/chem_utils/featurize/_xyz2mol.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/chem_utils/featurize/molconvert.py` & `PyTDC-0.4.7/tdc/chem_utils/featurize/molconvert.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/chem_utils/oracle/docking.py` & `PyTDC-0.4.7/tdc/chem_utils/oracle/docking.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/chem_utils/oracle/filter.py` & `PyTDC-0.4.7/tdc/chem_utils/oracle/filter.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/chem_utils/oracle/oracle.py` & `PyTDC-0.4.7/tdc/chem_utils/oracle/oracle.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/dataset_configs/config.py` & `PyTDC-0.4.7/tdc/dataset_configs/config.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/dataset_configs/pentelute_mdm2_ace2_12ca5_config.py` & `PyTDC-0.4.7/tdc/dataset_configs/pentelute_mdm2_ace2_12ca5_config.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/evaluator.py` & `PyTDC-0.4.7/tdc/evaluator.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/feature_generators/data_feature_generator.py` & `PyTDC-0.4.7/tdc/feature_generators/data_feature_generator.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/feature_generators/protein_feature_generator.py` & `PyTDC-0.4.7/tdc/feature_generators/protein_feature_generator.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/generation/bi_generation_dataset.py` & `PyTDC-0.4.7/tdc/generation/bi_generation_dataset.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/generation/generation_dataset.py` & `PyTDC-0.4.7/tdc/generation/generation_dataset.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/generation/ligandmolgen.py` & `PyTDC-0.4.7/tdc/generation/ligandmolgen.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/generation/molgen.py` & `PyTDC-0.4.7/tdc/generation/molgen.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/generation/reaction.py` & `PyTDC-0.4.7/tdc/generation/reaction.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/generation/retrosyn.py` & `PyTDC-0.4.7/tdc/generation/retrosyn.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/generation/sbdd.py` & `PyTDC-0.4.7/tdc/generation/sbdd.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/metadata.py` & `PyTDC-0.4.7/tdc/metadata.py`

 * *Files 4% similar despite different names*

```diff
@@ -158,15 +158,18 @@
 
 mti_dataset_names = ["mirtarbase"]
 
 gda_dataset_names = ["disgenet"]
 
 crisproutcome_dataset_names = ["leenay"]
 
-drugres_dataset_names = ["gdsc1", "gdsc2"]
+drugres_dataset_names = [
+    "gdsc1",
+    "gdsc2",
+]
 
 drugsyn_dataset_names = ["oncopolypharmacology", "drugcomb"]
 
 antibodyaff_dataset_names = ["protein_sabdab"]
 
 yield_dataset_names = ["uspto_yields", "buchwald-hartwig"]
 
@@ -174,14 +177,22 @@
 
 tcr_epi_dataset_names = ["weber"]
 
 trial_outcome_dataset_names = ['phase1', 'phase2', 'phase3']
 
 proteinpeptide_dataset_names = ['pentelute_mdm2_ace2_12ca5']
 
+cellxgene_dataset_names = [
+    "scperturb_drug_AissaBenevolenskaya2021",
+    "scperturb_drug_SrivatsanTrapnell2020_sciplex2",
+    "scperturb_drug_SrivatsanTrapnell2020_sciplex3",
+    "scperturb_drug_SrivatsanTrapnell2020_sciplex4",
+    "scperturb_drug_ZhaoSims2021",
+]
+
 ####################################
 # generation
 
 retrosyn_dataset_names = ["uspto50k", "uspto"]
 
 forwardsyn_dataset_names = ["uspto"]
 
@@ -539,26 +550,17 @@
         "Develop",
         "QM",
         "Paratope",
         "Yields",
         "CRISPROutcome",
     ],
     "multi_pred": [
-        "DTI",
-        "PPI",
-        "DDI",
-        "PeptideMHC",
-        "DrugRes",
-        "AntibodyAff",
-        "DrugSyn",
-        "MTI",
-        "GDA",
-        "Catalyst",
-        "TCR_Epitope_Binding",
-        "TrialOutcome",
+        "DTI", "PPI", "DDI", "PeptideMHC", "DrugRes", "AntibodyAff", "DrugSyn",
+        "MTI", "GDA", "Catalyst", "TCR_Epitope_Binding", "TrialOutcome",
+        "CellXGene"
     ],
     "generation": ["RetroSyn", "Reaction", "MolGen"],
 }
 
 
 def get_task2category():
     task2category = {}
@@ -593,14 +595,15 @@
     "Catalyst": catalyst_dataset_names,
     "CRISPROutcome": crisproutcome_dataset_names,
     "test_single_pred": test_single_pred_dataset_names,
     "test_multi_pred": test_multi_pred_dataset_names,
     "TCREpitopeBinding": tcr_epi_dataset_names,
     "TrialOutcome": trial_outcome_dataset_names,
     "ProteinPeptide": proteinpeptide_dataset_names,
+    "CellXGene": cellxgene_dataset_names,
 }
 
 benchmark_names = {
     "admet_group": admet_benchmark,
     "drugcombo_group": drugsyn_benchmark,
     "docking_group": docking_benchmark,
     "dti_dg_group": dti_dg_benchmark,
@@ -732,14 +735,19 @@
     "primekg_drug_feature": "tab",
     "primekg_disease_feature": "tab",
     "drug_comb_meta_data": "pkl",
     "phase1": "tab",
     "phase2": "tab",
     "phase3": "tab",
     "pentelute_mdm2_ace2_12ca5": "xlsx",
+    "scperturb_drug_AissaBenevolenskaya2021": "h5ad",
+    "scperturb_drug_SrivatsanTrapnell2020_sciplex2": "h5ad",
+    "scperturb_drug_SrivatsanTrapnell2020_sciplex3": "h5ad",
+    "scperturb_drug_SrivatsanTrapnell2020_sciplex4": "h5ad",
+    "scperturb_drug_ZhaoSims2021": "h5ad",
 }
 
 name2id = {
     "bbb_adenot": 4259565,
     "bbb_martins": 4259566,
     "b3db_classification": 7878566,
     "b3db_regression": 7878567,
@@ -847,14 +855,19 @@
     "primekg_drug_feature": 6180619,
     "primekg_disease_feature": 6180618,
     "drug_comb_meta_data": 7104245,
     "phase1": 7331305,
     "phase2": 7331306,
     "phase3": 7331307,
     "pentelute_mdm2_ace2_12ca5": 9649623,
+    "scperturb_drug_AissaBenevolenskaya2021": 9845396,
+    "scperturb_drug_SrivatsanTrapnell2020_sciplex2": 9845394,
+    "scperturb_drug_SrivatsanTrapnell2020_sciplex3": 9845397,
+    "scperturb_drug_SrivatsanTrapnell2020_sciplex4": 9845395,
+    "scperturb_drug_ZhaoSims2021": 9845393,
 }
 
 oracle2type = {
     "drd2": "pkl",
     "jnk3": "pkl",
     "gsk3b": "pkl",
     "fpscores": "pkl",
```

### Comparing `PyTDC-0.4.6/tdc/multi_pred/antibodyaff.py` & `PyTDC-0.4.7/tdc/multi_pred/antibodyaff.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/multi_pred/bi_pred_dataset.py` & `PyTDC-0.4.7/tdc/multi_pred/bi_pred_dataset.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/multi_pred/catalyst.py` & `PyTDC-0.4.7/tdc/multi_pred/catalyst.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/multi_pred/ddi.py` & `PyTDC-0.4.7/tdc/multi_pred/ddi.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/multi_pred/drugres.py` & `PyTDC-0.4.7/tdc/multi_pred/drugres.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/multi_pred/drugsyn.py` & `PyTDC-0.4.7/tdc/multi_pred/drugsyn.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/multi_pred/dti.py` & `PyTDC-0.4.7/tdc/multi_pred/dti.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/multi_pred/gda.py` & `PyTDC-0.4.7/tdc/multi_pred/gda.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/multi_pred/mti.py` & `PyTDC-0.4.7/tdc/multi_pred/mti.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/multi_pred/multi_pred_dataset.py` & `PyTDC-0.4.7/tdc/multi_pred/multi_pred_dataset.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/multi_pred/peptidemhc.py` & `PyTDC-0.4.7/tdc/multi_pred/peptidemhc.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/multi_pred/ppi.py` & `PyTDC-0.4.7/tdc/multi_pred/ppi.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/multi_pred/proteinpeptide.py` & `PyTDC-0.4.7/tdc/multi_pred/proteinpeptide.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 warnings.filterwarnings("ignore")
 import sys
 
 from ..utils import print_sys
 from ..dataset_configs.pentelute_mdm2_ace2_12ca5_config import PenteluteProteinPeptideConfig
 from . import bi_pred_dataset
 from ..metadata import dataset_names
+from ..dataset_configs.config_map import ConfigMap
 
 
 class ProteinPeptide(bi_pred_dataset.DataLoader):
     """Data loader class to load datasets in Protein-Peptide Binding Prediction task.
     More info: TODO 
 
     Task Description: Regression.
@@ -32,21 +33,23 @@
 
 
     """
 
     def __init__(self, name, path="./data", label_name=None, print_stats=False):
         """Create Protein-Peptide Prediction dataloader object"""
         label_name = label_name if label_name is not None else "KD (nm)"  # TODO: this column should be parsed into float and upper/lower
+        cfm = ConfigMap()
+        config = cfm.get(name)
         super().__init__(
             name,
             path,
             label_name,
             print_stats,
             dataset_names=dataset_names["ProteinPeptide"],
-            data_config=PenteluteProteinPeptideConfig(),
+            data_config=config(),
         )
         self.entity1_name = "Sequence"  # peptide sequence
         self.entity2_name = "Protein Target"  # protein target label
         self.two_types = True
 
         if print_stats:
             self.print_stats()
```

### Comparing `PyTDC-0.4.6/tdc/multi_pred/tcr_epi.py` & `PyTDC-0.4.7/tdc/multi_pred/tcr_epi.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/multi_pred/test_multi_pred.py` & `PyTDC-0.4.7/tdc/multi_pred/test_multi_pred.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/multi_pred/trialoutcome.py` & `PyTDC-0.4.7/tdc/multi_pred/trialoutcome.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/oracles.py` & `PyTDC-0.4.7/tdc/oracles.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/resource/cellxgene_census.py` & `PyTDC-0.4.7/tdc/resource/cellxgene_census.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/resource/primekg.py` & `PyTDC-0.4.7/tdc/resource/primekg.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/single_pred/adme.py` & `PyTDC-0.4.7/tdc/single_pred/adme.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/single_pred/crispr_outcome.py` & `PyTDC-0.4.7/tdc/single_pred/crispr_outcome.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/single_pred/develop.py` & `PyTDC-0.4.7/tdc/single_pred/develop.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/single_pred/epitope.py` & `PyTDC-0.4.7/tdc/single_pred/epitope.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/single_pred/hts.py` & `PyTDC-0.4.7/tdc/single_pred/hts.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/single_pred/paratope.py` & `PyTDC-0.4.7/tdc/single_pred/paratope.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/single_pred/qm.py` & `PyTDC-0.4.7/tdc/single_pred/qm.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/single_pred/single_pred_dataset.py` & `PyTDC-0.4.7/tdc/single_pred/single_pred_dataset.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/single_pred/test_single_pred.py` & `PyTDC-0.4.7/tdc/single_pred/test_single_pred.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/single_pred/tox.py` & `PyTDC-0.4.7/tdc/single_pred/tox.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/single_pred/yields.py` & `PyTDC-0.4.7/tdc/single_pred/yields.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/tdc_hf.py` & `PyTDC-0.4.7/tdc/tdc_hf.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/utils/__init__.py` & `PyTDC-0.4.7/tdc/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/utils/knowledge_graph.py` & `PyTDC-0.4.7/tdc/utils/knowledge_graph.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/utils/label.py` & `PyTDC-0.4.7/tdc/utils/label.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/utils/label_name_list.py` & `PyTDC-0.4.7/tdc/utils/label_name_list.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/utils/load.py` & `PyTDC-0.4.7/tdc/utils/load.py`

 * *Files 0% similar despite different names*

```diff
@@ -298,14 +298,23 @@
         elif name2type[name] == "xlsx":
             df = pd.read_excel(os.path.join(path, name + "." + name2type[name]))
         elif name2type[name] == "pkl":
             df = pd.read_pickle(os.path.join(path,
                                              name + "." + name2type[name]))
         elif name2type[name] == "zip":
             df = pd.read_pickle(os.path.join(path, name + "/" + name + ".pkl"))
+        elif name2type[name] == "h5ad":
+            import anndata
+            adata = anndata.read_h5ad(
+                os.path.join(path, name + "." + name2type[name]))
+            # df = pd.DataFrame(adata.X.toarray(), columns=adata.var_names, index=adata.obs_names)
+            # TODO: multi-index would help include var information in columns
+            # multi_index = pd.MultiIndex.from_frame(adata.var.reset_index())
+            # df.columns = multi_index
+            return adata
         else:
             raise ValueError(
                 "The file type must be one of tab/csv/xlsx/pickle/zip.")
         try:
             df = df.drop_duplicates()
         except:
             pass
```

### Comparing `PyTDC-0.4.6/tdc/utils/misc.py` & `PyTDC-0.4.7/tdc/utils/misc.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/utils/query.py` & `PyTDC-0.4.7/tdc/utils/query.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/utils/retrieve.py` & `PyTDC-0.4.7/tdc/utils/retrieve.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/utils/split.py` & `PyTDC-0.4.7/tdc/utils/split.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.6/tdc/version.py` & `PyTDC-0.4.7/tdc/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,8 +15,8 @@
 # X.YbN # Beta release
 # X.YrcN # Release Candidate
 # X.Y # Final release
 #
 # Dev branch marker is: 'X.Y.dev' or 'X.Y.devN' where N is an integer.
 # 'X.Y.dev0' is the canonical version of 'X.Y.dev'
 #
-__version__ = "0.4.6"  # pragma: no cover
+__version__ = "0.4.7"  # pragma: no cover
```

