# Comparing `tmp/PyTDC-0.4.8.tar.gz` & `tmp/PyTDC-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyTDC-0.4.8.tar", last modified: Tue Apr  9 22:48:58 2024, max compression
+gzip compressed data, was "PyTDC-0.4.9.tar", last modified: Tue Apr  9 22:51:56 2024, max compression
```

## Comparing `PyTDC-0.4.8.tar` & `PyTDC-0.4.9.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 alejandrovelez-arce   (501) staff       (20)        0 2024-04-09 22:48:58.438099 PyTDC-0.4.8/
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1069 2024-03-01 19:46:57.000000 PyTDC-0.4.8/LICENSE
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      102 2024-03-01 19:46:57.000000 PyTDC-0.4.8/MANIFEST.in
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    19377 2024-04-09 22:48:58.437856 PyTDC-0.4.8/PKG-INFO
-drwxr-xr-x   0 alejandrovelez-arce   (501) staff       (20)        0 2024-04-09 22:48:58.437171 PyTDC-0.4.8/PyTDC.egg-info/
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    19377 2024-04-09 22:48:58.000000 PyTDC-0.4.8/PyTDC.egg-info/PKG-INFO
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     2733 2024-04-09 22:48:58.000000 PyTDC-0.4.8/PyTDC.egg-info/SOURCES.txt
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)        1 2024-04-09 22:48:58.000000 PyTDC-0.4.8/PyTDC.egg-info/dependency_links.txt
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)        1 2024-04-09 21:37:01.000000 PyTDC-0.4.8/PyTDC.egg-info/not-zip-safe
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      371 2024-04-09 22:48:58.000000 PyTDC-0.4.8/PyTDC.egg-info/requires.txt
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)        4 2024-04-09 22:48:58.000000 PyTDC-0.4.8/PyTDC.egg-info/top_level.txt
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    18401 2024-03-23 16:49:43.000000 PyTDC-0.4.8/README.md
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      372 2024-04-09 22:48:45.000000 PyTDC-0.4.8/requirements.txt
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)       79 2024-04-09 22:48:58.438688 PyTDC-0.4.8/setup.cfg
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1160 2024-03-25 19:24:21.000000 PyTDC-0.4.8/setup.py
-drwxr-xr-x   0 alejandrovelez-arce   (501) staff       (20)        0 2024-04-09 22:48:58.400803 PyTDC-0.4.8/tdc/
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      199 2024-03-17 21:08:33.000000 PyTDC-0.4.8/tdc/__init__.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     7852 2024-03-07 18:03:45.000000 PyTDC-0.4.8/tdc/base_dataset.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    22305 2024-03-07 18:03:45.000000 PyTDC-0.4.8/tdc/benchmark_deprecated.py
-drwxr-xr-x   0 alejandrovelez-arce   (501) staff       (20)        0 2024-04-09 22:48:58.403367 PyTDC-0.4.8/tdc/benchmark_group/
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      162 2024-03-01 19:46:57.000000 PyTDC-0.4.8/tdc/benchmark_group/__init__.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      449 2024-03-05 15:50:55.000000 PyTDC-0.4.8/tdc/benchmark_group/admet_group.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    10499 2024-03-07 18:03:45.000000 PyTDC-0.4.8/tdc/benchmark_group/base_group.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    16066 2024-03-07 18:03:45.000000 PyTDC-0.4.8/tdc/benchmark_group/docking_group.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      775 2024-03-07 18:03:45.000000 PyTDC-0.4.8/tdc/benchmark_group/drugcombo_group.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      453 2024-03-05 15:52:54.000000 PyTDC-0.4.8/tdc/benchmark_group/dti_dg_group.py
-drwxr-xr-x   0 alejandrovelez-arce   (501) staff       (20)        0 2024-04-09 22:48:58.404190 PyTDC-0.4.8/tdc/chem_utils/
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1021 2024-03-01 19:46:57.000000 PyTDC-0.4.8/tdc/chem_utils/__init__.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    14100 2024-03-07 18:03:45.000000 PyTDC-0.4.8/tdc/chem_utils/evaluator.py
-drwxr-xr-x   0 alejandrovelez-arce   (501) staff       (20)        0 2024-04-09 22:48:58.406361 PyTDC-0.4.8/tdc/chem_utils/featurize/
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)        0 2024-03-01 19:46:57.000000 PyTDC-0.4.8/tdc/chem_utils/featurize/__init__.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    28488 2024-03-05 15:54:24.000000 PyTDC-0.4.8/tdc/chem_utils/featurize/_smartsPatts.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    23821 2024-03-07 18:03:45.000000 PyTDC-0.4.8/tdc/chem_utils/featurize/_smiles2pubchem.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    22094 2024-03-07 18:03:45.000000 PyTDC-0.4.8/tdc/chem_utils/featurize/_xyz2mol.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    27277 2024-03-07 18:03:45.000000 PyTDC-0.4.8/tdc/chem_utils/featurize/molconvert.py
-drwxr-xr-x   0 alejandrovelez-arce   (501) staff       (20)        0 2024-04-09 22:48:58.408038 PyTDC-0.4.8/tdc/chem_utils/oracle/
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)        0 2024-03-01 19:46:57.000000 PyTDC-0.4.8/tdc/chem_utils/oracle/__init__.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1134 2024-03-07 18:03:45.000000 PyTDC-0.4.8/tdc/chem_utils/oracle/docking.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     6083 2024-03-07 18:03:45.000000 PyTDC-0.4.8/tdc/chem_utils/oracle/filter.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    61143 2024-03-07 18:03:45.000000 PyTDC-0.4.8/tdc/chem_utils/oracle/oracle.py
-drwxr-xr-x   0 alejandrovelez-arce   (501) staff       (20)        0 2024-04-09 22:48:58.410716 PyTDC-0.4.8/tdc/dataset_configs/
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      109 2024-03-23 16:49:30.000000 PyTDC-0.4.8/tdc/dataset_configs/__init__.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     2208 2024-03-23 16:49:30.000000 PyTDC-0.4.8/tdc/dataset_configs/config.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      706 2024-04-09 17:21:43.000000 PyTDC-0.4.8/tdc/dataset_configs/config_map.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1093 2024-03-23 16:49:30.000000 PyTDC-0.4.8/tdc/dataset_configs/pentelute_mdm2_ace2_12ca5_config.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      702 2024-04-09 17:21:43.000000 PyTDC-0.4.8/tdc/dataset_configs/scperturb_config.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    15896 2024-03-07 18:03:45.000000 PyTDC-0.4.8/tdc/evaluator.py
-drwxr-xr-x   0 alejandrovelez-arce   (501) staff       (20)        0 2024-04-09 22:48:58.412425 PyTDC-0.4.8/tdc/feature_generators/
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)        0 2024-03-25 19:24:21.000000 PyTDC-0.4.8/tdc/feature_generators/__init__.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1348 2024-04-09 17:21:43.000000 PyTDC-0.4.8/tdc/feature_generators/anndata_to_dataframe.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     4055 2024-03-23 16:49:30.000000 PyTDC-0.4.8/tdc/feature_generators/data_feature_generator.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     7504 2024-03-23 16:49:30.000000 PyTDC-0.4.8/tdc/feature_generators/protein_feature_generator.py
-drwxr-xr-x   0 alejandrovelez-arce   (501) staff       (20)        0 2024-04-09 22:48:58.416467 PyTDC-0.4.8/tdc/generation/
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      112 2024-03-01 19:46:57.000000 PyTDC-0.4.8/tdc/generation/__init__.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     3826 2024-03-07 18:03:45.000000 PyTDC-0.4.8/tdc/generation/bi_generation_dataset.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     9977 2024-03-07 18:03:45.000000 PyTDC-0.4.8/tdc/generation/generation_dataset.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      816 2024-03-07 18:03:45.000000 PyTDC-0.4.8/tdc/generation/ligandmolgen.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1060 2024-03-07 18:03:45.000000 PyTDC-0.4.8/tdc/generation/molgen.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1146 2024-03-07 18:03:45.000000 PyTDC-0.4.8/tdc/generation/reaction.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     2470 2024-03-07 18:03:45.000000 PyTDC-0.4.8/tdc/generation/retrosyn.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     5805 2024-03-07 18:03:45.000000 PyTDC-0.4.8/tdc/generation/sbdd.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    29018 2024-04-09 17:21:43.000000 PyTDC-0.4.8/tdc/metadata.py
-drwxr-xr-x   0 alejandrovelez-arce   (501) staff       (20)        0 2024-04-09 22:48:58.424796 PyTDC-0.4.8/tdc/multi_pred/
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      430 2024-03-23 16:49:30.000000 PyTDC-0.4.8/tdc/multi_pred/__init__.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      727 2024-04-09 17:21:43.000000 PyTDC-0.4.8/tdc/multi_pred/anndata_dataset.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1491 2024-03-07 18:03:45.000000 PyTDC-0.4.8/tdc/multi_pred/antibodyaff.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    13985 2024-04-04 13:31:38.000000 PyTDC-0.4.8/tdc/multi_pred/bi_pred_dataset.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1481 2024-03-07 18:03:45.000000 PyTDC-0.4.8/tdc/multi_pred/catalyst.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      444 2024-04-09 17:21:43.000000 PyTDC-0.4.8/tdc/multi_pred/cellxgene.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     2062 2024-03-07 18:03:45.000000 PyTDC-0.4.8/tdc/multi_pred/ddi.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     2031 2024-03-07 18:03:45.000000 PyTDC-0.4.8/tdc/multi_pred/drugres.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1291 2024-03-07 18:03:45.000000 PyTDC-0.4.8/tdc/multi_pred/drugsyn.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     2987 2024-03-07 18:03:45.000000 PyTDC-0.4.8/tdc/multi_pred/dti.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1534 2024-03-07 18:03:45.000000 PyTDC-0.4.8/tdc/multi_pred/gda.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1579 2024-03-07 18:03:45.000000 PyTDC-0.4.8/tdc/multi_pred/mti.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     4056 2024-03-07 18:03:45.000000 PyTDC-0.4.8/tdc/multi_pred/multi_pred_dataset.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1544 2024-03-07 18:03:45.000000 PyTDC-0.4.8/tdc/multi_pred/peptidemhc.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     2085 2024-03-07 18:03:45.000000 PyTDC-0.4.8/tdc/multi_pred/ppi.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1904 2024-04-09 17:21:43.000000 PyTDC-0.4.8/tdc/multi_pred/proteinpeptide.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1305 2024-03-07 18:03:45.000000 PyTDC-0.4.8/tdc/multi_pred/tcr_epi.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1163 2024-03-07 18:03:45.000000 PyTDC-0.4.8/tdc/multi_pred/test_multi_pred.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1616 2024-03-07 18:03:45.000000 PyTDC-0.4.8/tdc/multi_pred/trialoutcome.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    25828 2024-04-09 20:55:54.000000 PyTDC-0.4.8/tdc/oracles.py
-drwxr-xr-x   0 alejandrovelez-arce   (501) staff       (20)        0 2024-04-09 22:48:58.426055 PyTDC-0.4.8/tdc/resource/
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)       74 2024-03-17 21:08:33.000000 PyTDC-0.4.8/tdc/resource/__init__.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    18591 2024-03-25 19:24:21.000000 PyTDC-0.4.8/tdc/resource/cellxgene_census.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     2613 2024-03-17 21:08:33.000000 PyTDC-0.4.8/tdc/resource/primekg.py
-drwxr-xr-x   0 alejandrovelez-arce   (501) staff       (20)        0 2024-04-09 22:48:58.432079 PyTDC-0.4.8/tdc/single_pred/
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      287 2024-03-01 19:46:57.000000 PyTDC-0.4.8/tdc/single_pred/__init__.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     4229 2024-03-07 18:03:45.000000 PyTDC-0.4.8/tdc/single_pred/adme.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1560 2024-03-07 18:03:45.000000 PyTDC-0.4.8/tdc/single_pred/crispr_outcome.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     5751 2024-03-07 18:03:45.000000 PyTDC-0.4.8/tdc/single_pred/develop.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1554 2024-03-07 18:03:45.000000 PyTDC-0.4.8/tdc/single_pred/epitope.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1473 2024-03-07 18:03:45.000000 PyTDC-0.4.8/tdc/single_pred/hts.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1559 2024-03-07 18:03:45.000000 PyTDC-0.4.8/tdc/single_pred/paratope.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1587 2024-03-07 18:03:45.000000 PyTDC-0.4.8/tdc/single_pred/qm.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     6831 2024-03-07 18:03:45.000000 PyTDC-0.4.8/tdc/single_pred/single_pred_dataset.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1484 2024-03-07 18:03:45.000000 PyTDC-0.4.8/tdc/single_pred/test_single_pred.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1517 2024-03-07 18:03:45.000000 PyTDC-0.4.8/tdc/single_pred/tox.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1583 2024-03-07 18:03:45.000000 PyTDC-0.4.8/tdc/single_pred/yields.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     3594 2024-03-07 18:03:45.000000 PyTDC-0.4.8/tdc/tdc_hf.py
-drwxr-xr-x   0 alejandrovelez-arce   (501) staff       (20)        0 2024-04-09 22:48:58.436677 PyTDC-0.4.8/tdc/utils/
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1232 2024-03-23 16:49:30.000000 PyTDC-0.4.8/tdc/utils/__init__.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      916 2024-03-17 21:08:33.000000 PyTDC-0.4.8/tdc/utils/knowledge_graph.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     9227 2024-03-18 13:44:09.000000 PyTDC-0.4.8/tdc/utils/label.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    19101 2024-03-07 18:03:45.000000 PyTDC-0.4.8/tdc/utils/label_name_list.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    38462 2024-04-09 17:21:43.000000 PyTDC-0.4.8/tdc/utils/load.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     3438 2024-03-07 18:03:45.000000 PyTDC-0.4.8/tdc/utils/misc.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     3114 2024-03-07 18:03:45.000000 PyTDC-0.4.8/tdc/utils/query.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     3576 2024-03-07 18:03:45.000000 PyTDC-0.4.8/tdc/utils/retrieve.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    13042 2024-03-07 18:03:45.000000 PyTDC-0.4.8/tdc/utils/split.py
--rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      535 2024-04-09 22:47:27.000000 PyTDC-0.4.8/tdc/version.py
+drwxr-xr-x   0 alejandrovelez-arce   (501) staff       (20)        0 2024-04-09 22:51:56.077976 PyTDC-0.4.9/
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1069 2024-03-01 19:46:57.000000 PyTDC-0.4.9/LICENSE
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      102 2024-03-01 19:46:57.000000 PyTDC-0.4.9/MANIFEST.in
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    19374 2024-04-09 22:51:56.077718 PyTDC-0.4.9/PKG-INFO
+drwxr-xr-x   0 alejandrovelez-arce   (501) staff       (20)        0 2024-04-09 22:51:56.076759 PyTDC-0.4.9/PyTDC.egg-info/
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    19374 2024-04-09 22:51:55.000000 PyTDC-0.4.9/PyTDC.egg-info/PKG-INFO
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     2733 2024-04-09 22:51:55.000000 PyTDC-0.4.9/PyTDC.egg-info/SOURCES.txt
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)        1 2024-04-09 22:51:55.000000 PyTDC-0.4.9/PyTDC.egg-info/dependency_links.txt
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)        1 2024-04-09 21:37:01.000000 PyTDC-0.4.9/PyTDC.egg-info/not-zip-safe
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      368 2024-04-09 22:51:55.000000 PyTDC-0.4.9/PyTDC.egg-info/requires.txt
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)        4 2024-04-09 22:51:55.000000 PyTDC-0.4.9/PyTDC.egg-info/top_level.txt
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    18401 2024-03-23 16:49:43.000000 PyTDC-0.4.9/README.md
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      369 2024-04-09 22:51:25.000000 PyTDC-0.4.9/requirements.txt
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)       79 2024-04-09 22:51:56.078638 PyTDC-0.4.9/setup.cfg
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1160 2024-03-25 19:24:21.000000 PyTDC-0.4.9/setup.py
+drwxr-xr-x   0 alejandrovelez-arce   (501) staff       (20)        0 2024-04-09 22:51:56.018746 PyTDC-0.4.9/tdc/
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      199 2024-03-17 21:08:33.000000 PyTDC-0.4.9/tdc/__init__.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     7852 2024-03-07 18:03:45.000000 PyTDC-0.4.9/tdc/base_dataset.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    22305 2024-03-07 18:03:45.000000 PyTDC-0.4.9/tdc/benchmark_deprecated.py
+drwxr-xr-x   0 alejandrovelez-arce   (501) staff       (20)        0 2024-04-09 22:51:56.023067 PyTDC-0.4.9/tdc/benchmark_group/
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      162 2024-03-01 19:46:57.000000 PyTDC-0.4.9/tdc/benchmark_group/__init__.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      449 2024-03-05 15:50:55.000000 PyTDC-0.4.9/tdc/benchmark_group/admet_group.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    10499 2024-03-07 18:03:45.000000 PyTDC-0.4.9/tdc/benchmark_group/base_group.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    16066 2024-03-07 18:03:45.000000 PyTDC-0.4.9/tdc/benchmark_group/docking_group.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      775 2024-03-07 18:03:45.000000 PyTDC-0.4.9/tdc/benchmark_group/drugcombo_group.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      453 2024-03-05 15:52:54.000000 PyTDC-0.4.9/tdc/benchmark_group/dti_dg_group.py
+drwxr-xr-x   0 alejandrovelez-arce   (501) staff       (20)        0 2024-04-09 22:51:56.025050 PyTDC-0.4.9/tdc/chem_utils/
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1021 2024-03-01 19:46:57.000000 PyTDC-0.4.9/tdc/chem_utils/__init__.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    14100 2024-03-07 18:03:45.000000 PyTDC-0.4.9/tdc/chem_utils/evaluator.py
+drwxr-xr-x   0 alejandrovelez-arce   (501) staff       (20)        0 2024-04-09 22:51:56.029592 PyTDC-0.4.9/tdc/chem_utils/featurize/
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)        0 2024-03-01 19:46:57.000000 PyTDC-0.4.9/tdc/chem_utils/featurize/__init__.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    28488 2024-03-05 15:54:24.000000 PyTDC-0.4.9/tdc/chem_utils/featurize/_smartsPatts.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    23821 2024-03-07 18:03:45.000000 PyTDC-0.4.9/tdc/chem_utils/featurize/_smiles2pubchem.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    22094 2024-03-07 18:03:45.000000 PyTDC-0.4.9/tdc/chem_utils/featurize/_xyz2mol.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    27277 2024-03-07 18:03:45.000000 PyTDC-0.4.9/tdc/chem_utils/featurize/molconvert.py
+drwxr-xr-x   0 alejandrovelez-arce   (501) staff       (20)        0 2024-04-09 22:51:56.032647 PyTDC-0.4.9/tdc/chem_utils/oracle/
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)        0 2024-03-01 19:46:57.000000 PyTDC-0.4.9/tdc/chem_utils/oracle/__init__.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1134 2024-03-07 18:03:45.000000 PyTDC-0.4.9/tdc/chem_utils/oracle/docking.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     6083 2024-03-07 18:03:45.000000 PyTDC-0.4.9/tdc/chem_utils/oracle/filter.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    61143 2024-03-07 18:03:45.000000 PyTDC-0.4.9/tdc/chem_utils/oracle/oracle.py
+drwxr-xr-x   0 alejandrovelez-arce   (501) staff       (20)        0 2024-04-09 22:51:56.037127 PyTDC-0.4.9/tdc/dataset_configs/
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      109 2024-03-23 16:49:30.000000 PyTDC-0.4.9/tdc/dataset_configs/__init__.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     2208 2024-03-23 16:49:30.000000 PyTDC-0.4.9/tdc/dataset_configs/config.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      706 2024-04-09 17:21:43.000000 PyTDC-0.4.9/tdc/dataset_configs/config_map.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1093 2024-03-23 16:49:30.000000 PyTDC-0.4.9/tdc/dataset_configs/pentelute_mdm2_ace2_12ca5_config.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      702 2024-04-09 17:21:43.000000 PyTDC-0.4.9/tdc/dataset_configs/scperturb_config.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    15896 2024-03-07 18:03:45.000000 PyTDC-0.4.9/tdc/evaluator.py
+drwxr-xr-x   0 alejandrovelez-arce   (501) staff       (20)        0 2024-04-09 22:51:56.039464 PyTDC-0.4.9/tdc/feature_generators/
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)        0 2024-03-25 19:24:21.000000 PyTDC-0.4.9/tdc/feature_generators/__init__.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1348 2024-04-09 17:21:43.000000 PyTDC-0.4.9/tdc/feature_generators/anndata_to_dataframe.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     4055 2024-03-23 16:49:30.000000 PyTDC-0.4.9/tdc/feature_generators/data_feature_generator.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     7504 2024-03-23 16:49:30.000000 PyTDC-0.4.9/tdc/feature_generators/protein_feature_generator.py
+drwxr-xr-x   0 alejandrovelez-arce   (501) staff       (20)        0 2024-04-09 22:51:56.045068 PyTDC-0.4.9/tdc/generation/
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      112 2024-03-01 19:46:57.000000 PyTDC-0.4.9/tdc/generation/__init__.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     3826 2024-03-07 18:03:45.000000 PyTDC-0.4.9/tdc/generation/bi_generation_dataset.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     9977 2024-03-07 18:03:45.000000 PyTDC-0.4.9/tdc/generation/generation_dataset.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      816 2024-03-07 18:03:45.000000 PyTDC-0.4.9/tdc/generation/ligandmolgen.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1060 2024-03-07 18:03:45.000000 PyTDC-0.4.9/tdc/generation/molgen.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1146 2024-03-07 18:03:45.000000 PyTDC-0.4.9/tdc/generation/reaction.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     2470 2024-03-07 18:03:45.000000 PyTDC-0.4.9/tdc/generation/retrosyn.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     5805 2024-03-07 18:03:45.000000 PyTDC-0.4.9/tdc/generation/sbdd.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    29018 2024-04-09 17:21:43.000000 PyTDC-0.4.9/tdc/metadata.py
+drwxr-xr-x   0 alejandrovelez-arce   (501) staff       (20)        0 2024-04-09 22:51:56.057579 PyTDC-0.4.9/tdc/multi_pred/
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      430 2024-03-23 16:49:30.000000 PyTDC-0.4.9/tdc/multi_pred/__init__.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      727 2024-04-09 17:21:43.000000 PyTDC-0.4.9/tdc/multi_pred/anndata_dataset.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1491 2024-03-07 18:03:45.000000 PyTDC-0.4.9/tdc/multi_pred/antibodyaff.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    13985 2024-04-04 13:31:38.000000 PyTDC-0.4.9/tdc/multi_pred/bi_pred_dataset.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1481 2024-03-07 18:03:45.000000 PyTDC-0.4.9/tdc/multi_pred/catalyst.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      444 2024-04-09 17:21:43.000000 PyTDC-0.4.9/tdc/multi_pred/cellxgene.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     2062 2024-03-07 18:03:45.000000 PyTDC-0.4.9/tdc/multi_pred/ddi.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     2031 2024-03-07 18:03:45.000000 PyTDC-0.4.9/tdc/multi_pred/drugres.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1291 2024-03-07 18:03:45.000000 PyTDC-0.4.9/tdc/multi_pred/drugsyn.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     2987 2024-03-07 18:03:45.000000 PyTDC-0.4.9/tdc/multi_pred/dti.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1534 2024-03-07 18:03:45.000000 PyTDC-0.4.9/tdc/multi_pred/gda.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1579 2024-03-07 18:03:45.000000 PyTDC-0.4.9/tdc/multi_pred/mti.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     4056 2024-03-07 18:03:45.000000 PyTDC-0.4.9/tdc/multi_pred/multi_pred_dataset.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1544 2024-03-07 18:03:45.000000 PyTDC-0.4.9/tdc/multi_pred/peptidemhc.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     2085 2024-03-07 18:03:45.000000 PyTDC-0.4.9/tdc/multi_pred/ppi.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1904 2024-04-09 17:21:43.000000 PyTDC-0.4.9/tdc/multi_pred/proteinpeptide.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1305 2024-03-07 18:03:45.000000 PyTDC-0.4.9/tdc/multi_pred/tcr_epi.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1163 2024-03-07 18:03:45.000000 PyTDC-0.4.9/tdc/multi_pred/test_multi_pred.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1616 2024-03-07 18:03:45.000000 PyTDC-0.4.9/tdc/multi_pred/trialoutcome.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    25828 2024-04-09 20:55:54.000000 PyTDC-0.4.9/tdc/oracles.py
+drwxr-xr-x   0 alejandrovelez-arce   (501) staff       (20)        0 2024-04-09 22:51:56.059808 PyTDC-0.4.9/tdc/resource/
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)       74 2024-03-17 21:08:33.000000 PyTDC-0.4.9/tdc/resource/__init__.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    18591 2024-03-25 19:24:21.000000 PyTDC-0.4.9/tdc/resource/cellxgene_census.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     2613 2024-03-17 21:08:33.000000 PyTDC-0.4.9/tdc/resource/primekg.py
+drwxr-xr-x   0 alejandrovelez-arce   (501) staff       (20)        0 2024-04-09 22:51:56.067685 PyTDC-0.4.9/tdc/single_pred/
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      287 2024-03-01 19:46:57.000000 PyTDC-0.4.9/tdc/single_pred/__init__.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     4229 2024-03-07 18:03:45.000000 PyTDC-0.4.9/tdc/single_pred/adme.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1560 2024-03-07 18:03:45.000000 PyTDC-0.4.9/tdc/single_pred/crispr_outcome.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     5751 2024-03-07 18:03:45.000000 PyTDC-0.4.9/tdc/single_pred/develop.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1554 2024-03-07 18:03:45.000000 PyTDC-0.4.9/tdc/single_pred/epitope.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1473 2024-03-07 18:03:45.000000 PyTDC-0.4.9/tdc/single_pred/hts.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1559 2024-03-07 18:03:45.000000 PyTDC-0.4.9/tdc/single_pred/paratope.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1587 2024-03-07 18:03:45.000000 PyTDC-0.4.9/tdc/single_pred/qm.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     6831 2024-03-07 18:03:45.000000 PyTDC-0.4.9/tdc/single_pred/single_pred_dataset.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1484 2024-03-07 18:03:45.000000 PyTDC-0.4.9/tdc/single_pred/test_single_pred.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1517 2024-03-07 18:03:45.000000 PyTDC-0.4.9/tdc/single_pred/tox.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1583 2024-03-07 18:03:45.000000 PyTDC-0.4.9/tdc/single_pred/yields.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     3594 2024-03-07 18:03:45.000000 PyTDC-0.4.9/tdc/tdc_hf.py
+drwxr-xr-x   0 alejandrovelez-arce   (501) staff       (20)        0 2024-04-09 22:51:56.076020 PyTDC-0.4.9/tdc/utils/
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     1232 2024-03-23 16:49:30.000000 PyTDC-0.4.9/tdc/utils/__init__.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      916 2024-03-17 21:08:33.000000 PyTDC-0.4.9/tdc/utils/knowledge_graph.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     9227 2024-03-18 13:44:09.000000 PyTDC-0.4.9/tdc/utils/label.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    19101 2024-03-07 18:03:45.000000 PyTDC-0.4.9/tdc/utils/label_name_list.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    38462 2024-04-09 17:21:43.000000 PyTDC-0.4.9/tdc/utils/load.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     3438 2024-03-07 18:03:45.000000 PyTDC-0.4.9/tdc/utils/misc.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     3114 2024-03-07 18:03:45.000000 PyTDC-0.4.9/tdc/utils/query.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)     3576 2024-03-07 18:03:45.000000 PyTDC-0.4.9/tdc/utils/retrieve.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)    13042 2024-03-07 18:03:45.000000 PyTDC-0.4.9/tdc/utils/split.py
+-rw-r--r--   0 alejandrovelez-arce   (501) staff       (20)      535 2024-04-09 22:51:46.000000 PyTDC-0.4.9/tdc/version.py
```

### Comparing `PyTDC-0.4.8/LICENSE` & `PyTDC-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/PKG-INFO` & `PyTDC-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: PyTDC
-Version: 0.4.8
+Version: 0.4.9
 Summary: Therapeutics Data Commons
 Home-page: https://github.com/mims-harvard/TDC
 Author: TDC Team
 Author-email: alejandro_velez-arce@hms.harvard.edu
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: biopython==1.78
 Requires-Dist: dataclasses==0.6
 Requires-Dist: DeepPurpose==0.1.5
-Requires-Dist: descriptastorus==2.5.0.23
+Requires-Dist: descriptastorus==2.4.2
 Requires-Dist: dgl==2.1.0
 Requires-Dist: fuzzywuzzy==0.18.0
 Requires-Dist: huggingface_hub==0.20.3
 Requires-Dist: mygene==3.2.2
 Requires-Dist: numpy==1.26.4
 Requires-Dist: openpyxl==3.0.10
 Requires-Dist: pandas==2.1.4
```

### Comparing `PyTDC-0.4.8/PyTDC.egg-info/PKG-INFO` & `PyTDC-0.4.9/PyTDC.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: PyTDC
-Version: 0.4.8
+Version: 0.4.9
 Summary: Therapeutics Data Commons
 Home-page: https://github.com/mims-harvard/TDC
 Author: TDC Team
 Author-email: alejandro_velez-arce@hms.harvard.edu
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: biopython==1.78
 Requires-Dist: dataclasses==0.6
 Requires-Dist: DeepPurpose==0.1.5
-Requires-Dist: descriptastorus==2.5.0.23
+Requires-Dist: descriptastorus==2.4.2
 Requires-Dist: dgl==2.1.0
 Requires-Dist: fuzzywuzzy==0.18.0
 Requires-Dist: huggingface_hub==0.20.3
 Requires-Dist: mygene==3.2.2
 Requires-Dist: numpy==1.26.4
 Requires-Dist: openpyxl==3.0.10
 Requires-Dist: pandas==2.1.4
```

### Comparing `PyTDC-0.4.8/PyTDC.egg-info/SOURCES.txt` & `PyTDC-0.4.9/PyTDC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/README.md` & `PyTDC-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/setup.py` & `PyTDC-0.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/base_dataset.py` & `PyTDC-0.4.9/tdc/base_dataset.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/benchmark_deprecated.py` & `PyTDC-0.4.9/tdc/benchmark_deprecated.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/benchmark_group/base_group.py` & `PyTDC-0.4.9/tdc/benchmark_group/base_group.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/benchmark_group/docking_group.py` & `PyTDC-0.4.9/tdc/benchmark_group/docking_group.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/benchmark_group/drugcombo_group.py` & `PyTDC-0.4.9/tdc/benchmark_group/drugcombo_group.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/chem_utils/__init__.py` & `PyTDC-0.4.9/tdc/chem_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/chem_utils/evaluator.py` & `PyTDC-0.4.9/tdc/chem_utils/evaluator.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/chem_utils/featurize/_smartsPatts.py` & `PyTDC-0.4.9/tdc/chem_utils/featurize/_smartsPatts.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/chem_utils/featurize/_smiles2pubchem.py` & `PyTDC-0.4.9/tdc/chem_utils/featurize/_smiles2pubchem.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/chem_utils/featurize/_xyz2mol.py` & `PyTDC-0.4.9/tdc/chem_utils/featurize/_xyz2mol.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/chem_utils/featurize/molconvert.py` & `PyTDC-0.4.9/tdc/chem_utils/featurize/molconvert.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/chem_utils/oracle/docking.py` & `PyTDC-0.4.9/tdc/chem_utils/oracle/docking.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/chem_utils/oracle/filter.py` & `PyTDC-0.4.9/tdc/chem_utils/oracle/filter.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/chem_utils/oracle/oracle.py` & `PyTDC-0.4.9/tdc/chem_utils/oracle/oracle.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/dataset_configs/config.py` & `PyTDC-0.4.9/tdc/dataset_configs/config.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/dataset_configs/config_map.py` & `PyTDC-0.4.9/tdc/dataset_configs/config_map.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/dataset_configs/pentelute_mdm2_ace2_12ca5_config.py` & `PyTDC-0.4.9/tdc/dataset_configs/pentelute_mdm2_ace2_12ca5_config.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/dataset_configs/scperturb_config.py` & `PyTDC-0.4.9/tdc/dataset_configs/scperturb_config.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/evaluator.py` & `PyTDC-0.4.9/tdc/evaluator.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/feature_generators/anndata_to_dataframe.py` & `PyTDC-0.4.9/tdc/feature_generators/anndata_to_dataframe.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/feature_generators/data_feature_generator.py` & `PyTDC-0.4.9/tdc/feature_generators/data_feature_generator.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/feature_generators/protein_feature_generator.py` & `PyTDC-0.4.9/tdc/feature_generators/protein_feature_generator.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/generation/bi_generation_dataset.py` & `PyTDC-0.4.9/tdc/generation/bi_generation_dataset.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/generation/generation_dataset.py` & `PyTDC-0.4.9/tdc/generation/generation_dataset.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/generation/ligandmolgen.py` & `PyTDC-0.4.9/tdc/generation/ligandmolgen.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/generation/molgen.py` & `PyTDC-0.4.9/tdc/generation/molgen.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/generation/reaction.py` & `PyTDC-0.4.9/tdc/generation/reaction.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/generation/retrosyn.py` & `PyTDC-0.4.9/tdc/generation/retrosyn.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/generation/sbdd.py` & `PyTDC-0.4.9/tdc/generation/sbdd.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/metadata.py` & `PyTDC-0.4.9/tdc/metadata.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/multi_pred/anndata_dataset.py` & `PyTDC-0.4.9/tdc/multi_pred/anndata_dataset.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/multi_pred/antibodyaff.py` & `PyTDC-0.4.9/tdc/multi_pred/antibodyaff.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/multi_pred/bi_pred_dataset.py` & `PyTDC-0.4.9/tdc/multi_pred/bi_pred_dataset.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/multi_pred/catalyst.py` & `PyTDC-0.4.9/tdc/multi_pred/catalyst.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/multi_pred/ddi.py` & `PyTDC-0.4.9/tdc/multi_pred/ddi.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/multi_pred/drugres.py` & `PyTDC-0.4.9/tdc/multi_pred/drugres.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/multi_pred/drugsyn.py` & `PyTDC-0.4.9/tdc/multi_pred/drugsyn.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/multi_pred/dti.py` & `PyTDC-0.4.9/tdc/multi_pred/dti.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/multi_pred/gda.py` & `PyTDC-0.4.9/tdc/multi_pred/gda.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/multi_pred/mti.py` & `PyTDC-0.4.9/tdc/multi_pred/mti.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/multi_pred/multi_pred_dataset.py` & `PyTDC-0.4.9/tdc/multi_pred/multi_pred_dataset.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/multi_pred/peptidemhc.py` & `PyTDC-0.4.9/tdc/multi_pred/peptidemhc.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/multi_pred/ppi.py` & `PyTDC-0.4.9/tdc/multi_pred/ppi.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/multi_pred/proteinpeptide.py` & `PyTDC-0.4.9/tdc/multi_pred/proteinpeptide.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/multi_pred/tcr_epi.py` & `PyTDC-0.4.9/tdc/multi_pred/tcr_epi.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/multi_pred/test_multi_pred.py` & `PyTDC-0.4.9/tdc/multi_pred/test_multi_pred.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/multi_pred/trialoutcome.py` & `PyTDC-0.4.9/tdc/multi_pred/trialoutcome.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/oracles.py` & `PyTDC-0.4.9/tdc/oracles.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/resource/cellxgene_census.py` & `PyTDC-0.4.9/tdc/resource/cellxgene_census.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/resource/primekg.py` & `PyTDC-0.4.9/tdc/resource/primekg.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/single_pred/adme.py` & `PyTDC-0.4.9/tdc/single_pred/adme.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/single_pred/crispr_outcome.py` & `PyTDC-0.4.9/tdc/single_pred/crispr_outcome.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/single_pred/develop.py` & `PyTDC-0.4.9/tdc/single_pred/develop.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/single_pred/epitope.py` & `PyTDC-0.4.9/tdc/single_pred/epitope.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/single_pred/hts.py` & `PyTDC-0.4.9/tdc/single_pred/hts.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/single_pred/paratope.py` & `PyTDC-0.4.9/tdc/single_pred/paratope.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/single_pred/qm.py` & `PyTDC-0.4.9/tdc/single_pred/qm.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/single_pred/single_pred_dataset.py` & `PyTDC-0.4.9/tdc/single_pred/single_pred_dataset.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/single_pred/test_single_pred.py` & `PyTDC-0.4.9/tdc/single_pred/test_single_pred.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/single_pred/tox.py` & `PyTDC-0.4.9/tdc/single_pred/tox.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/single_pred/yields.py` & `PyTDC-0.4.9/tdc/single_pred/yields.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/tdc_hf.py` & `PyTDC-0.4.9/tdc/tdc_hf.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/utils/__init__.py` & `PyTDC-0.4.9/tdc/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/utils/knowledge_graph.py` & `PyTDC-0.4.9/tdc/utils/knowledge_graph.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/utils/label.py` & `PyTDC-0.4.9/tdc/utils/label.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/utils/label_name_list.py` & `PyTDC-0.4.9/tdc/utils/label_name_list.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/utils/load.py` & `PyTDC-0.4.9/tdc/utils/load.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/utils/misc.py` & `PyTDC-0.4.9/tdc/utils/misc.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/utils/query.py` & `PyTDC-0.4.9/tdc/utils/query.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/utils/retrieve.py` & `PyTDC-0.4.9/tdc/utils/retrieve.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.8/tdc/utils/split.py` & `PyTDC-0.4.9/tdc/utils/split.py`

 * *Files identical despite different names*

