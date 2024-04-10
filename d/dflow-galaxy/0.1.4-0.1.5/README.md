# Comparing `tmp/dflow_galaxy-0.1.4.tar.gz` & `tmp/dflow_galaxy-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dflow_galaxy-0.1.4.tar", max compression
+gzip compressed data, was "dflow_galaxy-0.1.5.tar", max compression
```

## Comparing `dflow_galaxy-0.1.4.tar` & `dflow_galaxy-0.1.5.tar`

### file list

```diff
@@ -1,75 +1,76 @@
--rw-r--r--   0        0        0    34523 2024-02-19 03:12:58.574253 dflow_galaxy-0.1.4/LICENSE
--rw-r--r--   0        0        0     1648 2024-04-07 12:32:34.406173 dflow_galaxy-0.1.4/README.md
--rw-r--r--   0        0        0        0 2024-01-30 01:22:58.649023 dflow_galaxy-0.1.4/dflow_galaxy/__init__.py
--rw-r--r--   0        0        0        0 2024-04-02 03:42:50.450085 dflow_galaxy-0.1.4/dflow_galaxy/app/__init__.py
--rw-r--r--   0        0        0     2193 2024-04-07 12:32:16.436174 dflow_galaxy-0.1.4/dflow_galaxy/app/common.py
--rw-r--r--   0        0        0        0 2024-04-02 03:42:50.450085 dflow_galaxy-0.1.4/dflow_galaxy/app/cp2k_lightning/__init__.py
--rw-r--r--   0        0        0     2047 2024-04-07 12:32:16.436174 dflow_galaxy-0.1.4/dflow_galaxy/app/cp2k_lightning/dflow.py
--rw-r--r--   0        0        0     6456 2024-04-07 12:32:16.436174 dflow_galaxy-0.1.4/dflow_galaxy/app/cp2k_lightning/main.py
--rw-r--r--   0        0        0        0 2024-04-07 12:32:16.436174 dflow_galaxy-0.1.4/dflow_galaxy/app/dynacat_md/__init__.py
--rw-r--r--   0        0        0     1910 2024-04-07 12:32:16.436174 dflow_galaxy-0.1.4/dflow_galaxy/app/dynacat_md/dflow.py
--rw-r--r--   0        0        0     4562 2024-04-07 12:32:16.436174 dflow_galaxy-0.1.4/dflow_galaxy/app/dynacat_md/main.py
--rw-r--r--   0        0        0        0 2024-04-02 03:42:50.450085 dflow_galaxy-0.1.4/dflow_galaxy/app/dynacat_tesla/__init__.py
--rw-r--r--   0        0        0      525 2024-04-07 06:31:41.633804 dflow_galaxy-0.1.4/dflow_galaxy/app/dynacat_tesla/main.py
--rw-r--r--   0        0        0        0 2024-02-06 03:07:45.063120 dflow_galaxy-0.1.4/dflow_galaxy/core/__init__.py
--rw-r--r--   0        0        0    28431 2024-04-07 12:32:16.436174 dflow_galaxy-0.1.4/dflow_galaxy/core/dflow.py
--rw-r--r--   0        0        0     4655 2024-04-02 03:42:50.450085 dflow_galaxy-0.1.4/dflow_galaxy/core/dispatcher.py
--rw-r--r--   0        0        0      163 2024-02-06 03:07:45.063120 dflow_galaxy-0.1.4/dflow_galaxy/core/log.py
--rw-r--r--   0        0        0       97 2024-04-01 07:14:05.895738 dflow_galaxy-0.1.4/dflow_galaxy/core/pydantic.py
--rw-r--r--   0        0        0      541 2024-04-03 16:22:36.889294 dflow_galaxy-0.1.4/dflow_galaxy/core/types.py
--rw-r--r--   0        0        0     5603 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.4/dflow_galaxy/core/util.py
--rw-r--r--   0        0        0      335 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.4/dflow_galaxy/main.py
--rw-r--r--   0        0        0       98 2024-04-02 03:42:50.450085 dflow_galaxy-0.1.4/dflow_galaxy/res/__init__.py
--rw-r--r--   0        0        0   189331 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/ALL_BASIS_SETS
--rw-r--r--   0        0        0     2717 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/ALL_POTENTIALS
--rw-r--r--   0        0        0    15836 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/AcPP1_POTENTIALS
--rw-r--r--   0        0        0    57524 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_ADMM
--rw-r--r--   0        0        0   189911 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_ADMM_MOLOPT
--rw-r--r--   0        0        0   133011 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_ADMM_UZH
--rw-r--r--   0        0        0    66934 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_ADMM_ae
--rw-r--r--   0        0        0    17509 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_LRIGPW_AUXMOLOPT
--rw-r--r--   0        0        0   244853 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_MINBAS
--rw-r--r--   0        0        0    49588 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_MINIX
--rw-r--r--   0        0        0   127679 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT
--rw-r--r--   0        0        0    55644 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_AcPP1
--rw-r--r--   0        0        0    23527 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_LnPP1
--rw-r--r--   0        0        0    65485 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_LnPP2
--rw-r--r--   0        0        0   179850 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_UCL
--rw-r--r--   0        0        0  1574370 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_UZH
--rw-r--r--   0        0        0     6644 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_PERIODIC_GW
--rw-r--r--   0        0        0    37261 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_RI_cc-TZ
--rw-r--r--   0        0        0   195109 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_SET
--rw-r--r--   0        0        0     5526 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_ZIJLSTRA
--rw-r--r--   0        0        0   324291 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_ccGRB_UZH
--rw-r--r--   0        0        0   258169 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_def2_QZVP_RI_ALL
--rw-r--r--   0        0        0   191314 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_pob
--rw-r--r--   0        0        0   223481 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/ECP_POTENTIALS
--rw-r--r--   0        0        0    23668 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/ECP_POTENTIALS_pob-TZVP-rev2
--rw-r--r--   0        0        0  1713484 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/EMSL_BASIS_SETS
--rw-r--r--   0        0        0   119403 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/GTH_BASIS_SETS
--rw-r--r--   0        0        0   167483 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/GTH_POTENTIALS
--rw-r--r--   0        0        0   253677 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/GTH_SOC_POTENTIALS
--rw-r--r--   0        0        0    17275 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/HFX_BASIS
--rw-r--r--   0        0        0     2106 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/HF_POTENTIALS
--rw-r--r--   0        0        0     5486 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/LnPP1_POTENTIALS
--rw-r--r--   0        0        0     7829 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/LnPP2_POTENTIALS
--rw-r--r--   0        0        0      447 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/MM_POTENTIAL
--rw-r--r--   0        0        0     5498 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/NLCC_POTENTIALS
--rw-r--r--   0        0        0   177804 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/POTENTIAL
--rw-r--r--   0        0        0   385325 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/POTENTIAL_UZH
--rw-r--r--   0        0        0      125 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/README.md
--rw-r--r--   0        0        0    91811 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/nm12_parameters.xml
--rw-r--r--   0        0        0    32194 2024-04-02 03:42:50.640085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/xTB_parameters
--rw-r--r--   0        0        0        0 2024-02-07 08:30:41.445577 dflow_galaxy-0.1.4/dflow_galaxy/workflow/__init__.py
--rw-r--r--   0        0        0        0 2024-02-07 08:30:41.445577 dflow_galaxy-0.1.4/dflow_galaxy/workflow/tesla/__init__.py
--rw-r--r--   0        0        0     1704 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.4/dflow_galaxy/workflow/tesla/config.py
--rw-r--r--   0        0        0        0 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.4/dflow_galaxy/workflow/tesla/domain/__init__.py
--rw-r--r--   0        0        0        0 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.4/dflow_galaxy/workflow/tesla/domain/abacus.py
--rw-r--r--   0        0        0     6298 2024-04-02 03:42:50.640085 dflow_galaxy-0.1.4/dflow_galaxy/workflow/tesla/domain/cp2k.py
--rw-r--r--   0        0        0     9775 2024-02-25 16:58:10.948762 dflow_galaxy-0.1.4/dflow_galaxy/workflow/tesla/domain/deepmd.py
--rw-r--r--   0        0        0     8016 2024-04-02 03:42:50.640085 dflow_galaxy-0.1.4/dflow_galaxy/workflow/tesla/domain/lammps.py
--rw-r--r--   0        0        0     1261 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.4/dflow_galaxy/workflow/tesla/domain/lib.py
--rw-r--r--   0        0        0     6334 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.4/dflow_galaxy/workflow/tesla/domain/model_devi.py
--rw-r--r--   0        0        0     7676 2024-04-07 12:32:16.436174 dflow_galaxy-0.1.4/dflow_galaxy/workflow/tesla/main.py
--rw-r--r--   0        0        0      541 2024-04-07 12:34:47.066159 dflow_galaxy-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2293 1970-01-01 00:00:00.000000 dflow_galaxy-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-02-19 03:12:58.574253 dflow_galaxy-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1834 2024-04-09 15:45:18.275720 dflow_galaxy-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2024-01-30 01:22:58.649023 dflow_galaxy-0.1.5/dflow_galaxy/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-02 03:42:50.450085 dflow_galaxy-0.1.5/dflow_galaxy/app/__init__.py
+-rw-r--r--   0        0        0     2499 2024-04-09 15:45:01.375722 dflow_galaxy-0.1.5/dflow_galaxy/app/common.py
+-rw-r--r--   0        0        0        0 2024-04-02 03:42:50.450085 dflow_galaxy-0.1.5/dflow_galaxy/app/cp2k_lightning/__init__.py
+-rw-r--r--   0        0        0     2047 2024-04-09 07:36:05.233859 dflow_galaxy-0.1.5/dflow_galaxy/app/cp2k_lightning/dflow.py
+-rw-r--r--   0        0        0     6456 2024-04-07 14:10:40.795458 dflow_galaxy-0.1.5/dflow_galaxy/app/cp2k_lightning/main.py
+-rw-r--r--   0        0        0        0 2024-04-07 12:32:16.436174 dflow_galaxy-0.1.5/dflow_galaxy/app/dynacat_md/__init__.py
+-rw-r--r--   0        0        0     1910 2024-04-09 06:12:22.344468 dflow_galaxy-0.1.5/dflow_galaxy/app/dynacat_md/dflow.py
+-rw-r--r--   0        0        0     4338 2024-04-09 15:45:01.375722 dflow_galaxy-0.1.5/dflow_galaxy/app/dynacat_md/main.py
+-rw-r--r--   0        0        0        0 2024-04-02 03:42:50.450085 dflow_galaxy-0.1.5/dflow_galaxy/app/dynacat_tesla/__init__.py
+-rw-r--r--   0        0        0    13473 2024-04-09 15:45:01.385722 dflow_galaxy-0.1.5/dflow_galaxy/app/dynacat_tesla/main.py
+-rw-r--r--   0        0        0        0 2024-02-06 03:07:45.063120 dflow_galaxy-0.1.5/dflow_galaxy/core/__init__.py
+-rw-r--r--   0        0        0    28431 2024-04-09 03:02:40.485846 dflow_galaxy-0.1.5/dflow_galaxy/core/dflow.py
+-rw-r--r--   0        0        0     4683 2024-04-09 15:45:01.385722 dflow_galaxy-0.1.5/dflow_galaxy/core/dispatcher.py
+-rw-r--r--   0        0        0      163 2024-02-06 03:07:45.063120 dflow_galaxy-0.1.5/dflow_galaxy/core/log.py
+-rw-r--r--   0        0        0       97 2024-04-01 07:14:05.895738 dflow_galaxy-0.1.5/dflow_galaxy/core/pydantic.py
+-rw-r--r--   0        0        0      541 2024-04-03 16:22:36.889294 dflow_galaxy-0.1.5/dflow_galaxy/core/types.py
+-rw-r--r--   0        0        0     5603 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.5/dflow_galaxy/core/util.py
+-rw-r--r--   0        0        0      335 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.5/dflow_galaxy/main.py
+-rw-r--r--   0        0        0      146 2024-04-09 15:45:01.385722 dflow_galaxy-0.1.5/dflow_galaxy/res/__init__.py
+-rw-r--r--   0        0        0   189331 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/ALL_BASIS_SETS
+-rw-r--r--   0        0        0     2717 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/ALL_POTENTIALS
+-rw-r--r--   0        0        0    15836 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/AcPP1_POTENTIALS
+-rw-r--r--   0        0        0    57524 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_ADMM
+-rw-r--r--   0        0        0   189911 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_ADMM_MOLOPT
+-rw-r--r--   0        0        0   133011 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_ADMM_UZH
+-rw-r--r--   0        0        0    66934 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_ADMM_ae
+-rw-r--r--   0        0        0    17509 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_LRIGPW_AUXMOLOPT
+-rw-r--r--   0        0        0   244853 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_MINBAS
+-rw-r--r--   0        0        0    49588 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_MINIX
+-rw-r--r--   0        0        0   127679 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT
+-rw-r--r--   0        0        0    55644 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_AcPP1
+-rw-r--r--   0        0        0    23527 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_LnPP1
+-rw-r--r--   0        0        0    65485 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_LnPP2
+-rw-r--r--   0        0        0   179850 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_UCL
+-rw-r--r--   0        0        0  1574370 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_UZH
+-rw-r--r--   0        0        0     6644 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_PERIODIC_GW
+-rw-r--r--   0        0        0    37261 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_RI_cc-TZ
+-rw-r--r--   0        0        0   195109 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_SET
+-rw-r--r--   0        0        0     5526 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_ZIJLSTRA
+-rw-r--r--   0        0        0   324291 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_ccGRB_UZH
+-rw-r--r--   0        0        0   258169 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_def2_QZVP_RI_ALL
+-rw-r--r--   0        0        0   191314 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_pob
+-rw-r--r--   0        0        0   223481 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/ECP_POTENTIALS
+-rw-r--r--   0        0        0    23668 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/ECP_POTENTIALS_pob-TZVP-rev2
+-rw-r--r--   0        0        0  1713484 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/EMSL_BASIS_SETS
+-rw-r--r--   0        0        0   119403 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/GTH_BASIS_SETS
+-rw-r--r--   0        0        0   167483 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/GTH_POTENTIALS
+-rw-r--r--   0        0        0   253677 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/GTH_SOC_POTENTIALS
+-rw-r--r--   0        0        0    17275 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/HFX_BASIS
+-rw-r--r--   0        0        0     2106 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/HF_POTENTIALS
+-rw-r--r--   0        0        0     5486 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/LnPP1_POTENTIALS
+-rw-r--r--   0        0        0     7829 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/LnPP2_POTENTIALS
+-rw-r--r--   0        0        0      447 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/MM_POTENTIAL
+-rw-r--r--   0        0        0     5498 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/NLCC_POTENTIALS
+-rw-r--r--   0        0        0   177804 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/POTENTIAL
+-rw-r--r--   0        0        0   385325 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/POTENTIAL_UZH
+-rw-r--r--   0        0        0      125 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/README.md
+-rw-r--r--   0        0        0    91811 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/nm12_parameters.xml
+-rw-r--r--   0        0        0    32194 2024-04-02 03:42:50.640085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/xTB_parameters
+-rw-r--r--   0        0        0     1171 2024-04-09 15:45:01.385722 dflow_galaxy-0.1.5/dflow_galaxy/res/dynacat/tesla_template.yml
+-rw-r--r--   0        0        0        0 2024-02-07 08:30:41.445577 dflow_galaxy-0.1.5/dflow_galaxy/workflow/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-07 08:30:41.445577 dflow_galaxy-0.1.5/dflow_galaxy/workflow/tesla/__init__.py
+-rw-r--r--   0        0        0     1702 2024-04-09 15:45:01.385722 dflow_galaxy-0.1.5/dflow_galaxy/workflow/tesla/config.py
+-rw-r--r--   0        0        0        0 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.5/dflow_galaxy/workflow/tesla/domain/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.5/dflow_galaxy/workflow/tesla/domain/abacus.py
+-rw-r--r--   0        0        0     6298 2024-04-02 03:42:50.640085 dflow_galaxy-0.1.5/dflow_galaxy/workflow/tesla/domain/cp2k.py
+-rw-r--r--   0        0        0     9775 2024-04-09 14:05:23.796450 dflow_galaxy-0.1.5/dflow_galaxy/workflow/tesla/domain/deepmd.py
+-rw-r--r--   0        0        0     8016 2024-04-02 03:42:50.640085 dflow_galaxy-0.1.5/dflow_galaxy/workflow/tesla/domain/lammps.py
+-rw-r--r--   0        0        0     1261 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.5/dflow_galaxy/workflow/tesla/domain/lib.py
+-rw-r--r--   0        0        0     6334 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.5/dflow_galaxy/workflow/tesla/domain/model_devi.py
+-rw-r--r--   0        0        0     8185 2024-04-09 15:45:01.385722 dflow_galaxy-0.1.5/dflow_galaxy/workflow/tesla/main.py
+-rw-r--r--   0        0        0      541 2024-04-09 15:49:46.375684 dflow_galaxy-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2479 1970-01-01 00:00:00.000000 dflow_galaxy-0.1.5/PKG-INFO
```

### Comparing `dflow_galaxy-0.1.4/LICENSE` & `dflow_galaxy-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.4/README.md` & `dflow_galaxy-0.1.5/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 # DFlow Galaxy
 
 [![PyPI version](https://badge.fury.io/py/dflow-galaxy.svg)](https://badge.fury.io/py/dflow-galaxy)
 [![Downloads](https://pepy.tech/badge/dflow-galaxy)](https://pepy.tech/project/dflow-galaxy)
+[![Docker](https://img.shields.io/docker/v/link89/dflow-galaxy?label=docker&logo=docker)](https://hub.docker.com/repository/docker/link89/dflow-galaxy/general)
+
 
 Collection of workflows and tools built on top of DFlow and [ai2-kit](https://github.com/chenggroup/ai2-kit).
 
 ## Features
 * DFlowBuilder: A type friendly wrapper for `DFlow` to build workflows in a more intuitive way.
 * Workflows:
   * TESLA: a **T**raining-**E**xploration-**S**creening-**L**abeling workflow designed by **AI4EC**. Get inspired by [DPGEN](https://github.com/deepmodeling/dpgen), [DPGEN2](https://github.com/deepmodeling/dpgen2), ported from [ai2-kit](https://github.com/chenggroup/ai2-kit).
 
+
 ## Get Started
 `dflow-galaxy` requires Python 3.9+ since it depends on `typing.Annotated`.
 
 To use `dflow-galaxy` as a library, you can install it via pip:
 
 ```bash
 pip install dflow-galaxy
@@ -25,20 +28,26 @@
 poetry install
 poetry shell
 ```
 
 ## Bohrium Launch App
 This repository also contains some launch apps for Bohrium. The entry of the Bohrium launch app is in the `launch_app` directory, and relative modules are in the `dflow_galaxy/app` directory.
 
-To build docker image for the launch app, you can use the following command:
+Currently, the following launch apps are available:
 
-```bash
-./build-docker.sh
-```
-### Launch Apps
 * CP2K Lightning: Run CP2K without building input files from scratch.
-* DynaCat TESLA: An automated workflow to generated DeepMD potential for DynaCat. (TODO)
+* DynaCat TESLA: An automated workflow to generated DeepMD potential for DynaCat.
 * DynaCat MD: Run MD simulations with DeepMD potential for DynaCat. 
 
 
+## Distribution
+### PyPI
+```bash
+poetry publish --build
+```
+### Docker
+```bash
+./build-docker.sh
+```
+
 ## Manuals
 * [TESLA Workflow](doc/tesla.md)
```

### Comparing `dflow_galaxy-0.1.4/dflow_galaxy/app/common.py` & `dflow_galaxy-0.1.5/dflow_galaxy/app/common.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from dp.launching.typing import BaseModel, Optional
+from dp.launching.typing import Int, String, Enum, Float, Boolean
 from dp.launching.typing import BohriumUsername, BohriumTicket, BohriumProjectId
 from dp.launching.typing import (
     DflowArgoAPIServer, DflowK8sAPIServer,
     DflowAccessToken, DflowStorageEndpoint,
     DflowStorageRepository, DflowLabels,
 )
 
@@ -59,7 +60,20 @@
     bohrium.config["bohrium_url"] = "https://bohrium.dp.tech"
     # override config? I have no idea
     dflow.s3_config["repo_key"] = "oss-bohrium"
     # side effect alert!!!
     # the following must be set at the end of all config
     dflow.s3_config['storage_client'] = bohrium.TiefblueClient()
     logger.info(f's3_config: {dflow.s3_config}')
+
+
+class EnsembleOptions(String, Enum):
+    nvt = 'nvt'
+    nvt_i = 'nvt-i'
+    nvt_a = 'nvt-a'
+    nvt_iso = 'nvt-iso'
+    nvt_aniso = 'nvt-aniso'
+    npt = 'npt'
+    npt_t = 'npt-t'
+    npt_tri = 'npt-tri'
+    nve = 'nve'
+    csvr = 'csvr'
```

### Comparing `dflow_galaxy-0.1.4/dflow_galaxy/app/cp2k_lightning/dflow.py` & `dflow_galaxy-0.1.5/dflow_galaxy/app/cp2k_lightning/dflow.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.4/dflow_galaxy/app/cp2k_lightning/main.py` & `dflow_galaxy-0.1.5/dflow_galaxy/app/cp2k_lightning/main.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.4/dflow_galaxy/app/dynacat_md/dflow.py` & `dflow_galaxy-0.1.5/dflow_galaxy/app/dynacat_md/dflow.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.4/dflow_galaxy/app/dynacat_md/main.py` & `dflow_galaxy-0.1.5/dflow_galaxy/app/dynacat_md/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dp.launching.typing import BaseModel, Field, OutputDirectory, InputFilePath, Optional, Dict
 from dp.launching.typing import Int, String, Enum, Float, Boolean
 from dp.launching.cli import to_runner, default_minimal_exception_handler
 
-from dflow_galaxy.app.common import DFlowOptions, setup_dflow_context
+from dflow_galaxy.app.common import DFlowOptions, setup_dflow_context, EnsembleOptions
 from dflow_galaxy.core.log import get_logger
 from ai2_kit.feat import catalysis as ai2cat
 from ai2_kit.core.util import dump_text, dump_json
 
 
 from pathlib import Path
 import shutil
@@ -14,27 +14,14 @@
 import os
 
 from .dflow import run_lammps_workflow
 
 logger = get_logger(__name__)
 
 
-class EnsembleOptions(String, Enum):
-    nvt = 'nvt'
-    nvt_i = 'nvt-i'
-    nvt_a = 'nvt-a'
-    nvt_iso = 'nvt-iso'
-    nvt_aniso = 'nvt-aniso'
-    npt = 'npt'
-    npt_t = 'npt-t'
-    npt_tri = 'npt-tri'
-    nve = 'nve'
-    csvr = 'csvr'
-
-
 class DynaCatMdArgs(DFlowOptions):
 
     dry_run: Boolean = Field(
         default = True,
         description="Generate configuration file without running the simulation")
 
     system_file: InputFilePath = Field(
```

### Comparing `dflow_galaxy-0.1.4/dflow_galaxy/core/dflow.py` & `dflow_galaxy-0.1.5/dflow_galaxy/core/dflow.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.4/dflow_galaxy/core/dispatcher.py` & `dflow_galaxy-0.1.5/dflow_galaxy/core/dispatcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from .pydantic import BaseModel
+from pydantic import Field
+
 
 from typing import Optional
 from urllib.parse import urlparse
 import os
 
 
 class BohriumInputData(BaseModel):
     image_name: str
+    scass_type: str = 'c2_m4_cpu'
     job_type: str = 'container'
     platform: str = 'ali'
-    scass_type: str = 'c2_m4_cpu'
     job_name: str = 'bohrium_job'
     disk_size: int = 20  # in GB
 
 
 class Resource(BaseModel):
     queue: Optional[str] = None
     image: Optional[str] = None
```

### Comparing `dflow_galaxy-0.1.4/dflow_galaxy/core/types.py` & `dflow_galaxy-0.1.5/dflow_galaxy/core/types.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.4/dflow_galaxy/core/util.py` & `dflow_galaxy-0.1.5/dflow_galaxy/core/util.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/ALL_BASIS_SETS` & `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/ALL_BASIS_SETS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/ALL_POTENTIALS` & `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/ALL_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/AcPP1_POTENTIALS` & `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/AcPP1_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_ADMM` & `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_ADMM`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_ADMM_MOLOPT` & `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_ADMM_MOLOPT`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_ADMM_UZH` & `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_ADMM_UZH`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_ADMM_ae` & `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_ADMM_ae`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_LRIGPW_AUXMOLOPT` & `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_LRIGPW_AUXMOLOPT`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_MINBAS` & `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_MINBAS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_MINIX` & `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_MINIX`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT` & `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_AcPP1` & `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_AcPP1`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_LnPP1` & `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_LnPP1`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_LnPP2` & `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_LnPP2`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_UCL` & `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_UCL`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_UZH` & `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_UZH`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_PERIODIC_GW` & `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_PERIODIC_GW`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_RI_cc-TZ` & `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_RI_cc-TZ`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_SET` & `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_SET`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_ZIJLSTRA` & `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_ZIJLSTRA`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_ccGRB_UZH` & `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_ccGRB_UZH`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_def2_QZVP_RI_ALL` & `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_def2_QZVP_RI_ALL`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_pob` & `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_pob`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/ECP_POTENTIALS` & `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/ECP_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/ECP_POTENTIALS_pob-TZVP-rev2` & `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/ECP_POTENTIALS_pob-TZVP-rev2`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/EMSL_BASIS_SETS` & `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/EMSL_BASIS_SETS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/GTH_BASIS_SETS` & `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/GTH_BASIS_SETS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/GTH_POTENTIALS` & `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/GTH_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/GTH_SOC_POTENTIALS` & `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/GTH_SOC_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/HFX_BASIS` & `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/HFX_BASIS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/HF_POTENTIALS` & `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/HF_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/LnPP1_POTENTIALS` & `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/LnPP1_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/LnPP2_POTENTIALS` & `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/LnPP2_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/NLCC_POTENTIALS` & `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/NLCC_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/POTENTIAL` & `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/POTENTIAL`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/POTENTIAL_UZH` & `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/POTENTIAL_UZH`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/nm12_parameters.xml` & `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/nm12_parameters.xml`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/xTB_parameters` & `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/xTB_parameters`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.4/dflow_galaxy/workflow/tesla/config.py` & `dflow_galaxy-0.1.5/dflow_galaxy/workflow/tesla/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,16 +55,14 @@
     label: LabelConfig
     train: TrainConfig
     explore: ExploreConfig
     screen: ScreenConfig
     update: Optional[UpdateConfig] = None
 
 
-
-
 class TeslaConfig(BaseModel):
     executors: Mapping[str, TeslaExecutorConfig]
     orchestration: Orchestration
     datasets: Mapping[str, Artifact]
     workflow: Any
 
     def init(self):
```

### Comparing `dflow_galaxy-0.1.4/dflow_galaxy/workflow/tesla/domain/cp2k.py` & `dflow_galaxy-0.1.5/dflow_galaxy/workflow/tesla/domain/cp2k.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.4/dflow_galaxy/workflow/tesla/domain/deepmd.py` & `dflow_galaxy-0.1.5/dflow_galaxy/workflow/tesla/domain/deepmd.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.4/dflow_galaxy/workflow/tesla/domain/lammps.py` & `dflow_galaxy-0.1.5/dflow_galaxy/workflow/tesla/domain/lammps.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.4/dflow_galaxy/workflow/tesla/domain/lib.py` & `dflow_galaxy-0.1.5/dflow_galaxy/workflow/tesla/domain/lib.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.4/dflow_galaxy/workflow/tesla/domain/model_devi.py` & `dflow_galaxy-0.1.5/dflow_galaxy/workflow/tesla/domain/model_devi.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.4/dflow_galaxy/workflow/tesla/main.py` & `dflow_galaxy-0.1.5/dflow_galaxy/workflow/tesla/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,54 +11,63 @@
 from .config import TeslaConfig, WorkflowConfig
 from .domain import deepmd, lammps, model_devi, cp2k
 from .domain.lib import StepSwitch, LabelApp, ExploreApp
 
 logger = get_logger(__name__)
 
 class RuntimeContext:
-    train_url: Optional[str]
+    train_url: Optional[str] = None
 
-    explore_url: Optional[str]
+    explore_url: Optional[str] = None
     explore_app: ExploreApp
 
-    screen_url: Optional[str]
+    screen_url: Optional[str] = None
 
-    label_url: Optional[str]
-    label_app: LabelApp
+    label_url: Optional[str] = None
+    label_app: Optional[LabelApp] = None
 
 
 def run_tesla(*config_files: str, s3_prefix: str, debug: bool = False, skip: bool = False, max_iters: int = 1):
+    builder = build_tesla_workflow(*config_files, s3_prefix=s3_prefix, debug=debug, skip=skip, max_iters=max_iters)
+    builder.run()
+
+
+def build_tesla_workflow(*config_files: str, s3_prefix: str, debug: bool = False, skip: bool = False, max_iters: int = 1):
     config_raw = load_yaml_files(*config_files)
     config = TeslaConfig(**config_raw)
     config.init()
 
     builder = DFlowBuilder(name='tesla', s3_prefix=s3_prefix, debug=debug,
                            default_archive=None)
     step_switch = StepSwitch(skip)
     runtime_ctx = RuntimeContext()
 
+    # ensure the existence of the placeholder files or else argo will raise 404 error
+    # this can not be tested in debug mode
+    builder.s3_dump('', 'init-dataset/.placeholder')
+    builder.s3_dump('', 'iter-dataset/.placeholder')
+
     raw_workflow_cfg = config.workflow
     for iter_num in range(max_iters):
         workflow_cfg = WorkflowConfig(**raw_workflow_cfg)
 
         type_map = workflow_cfg.general.type_map
         mass_map = workflow_cfg.general.mass_map
 
         iter_str = f'{iter_num:03d}'
 
         # Labeling
         cp2k_cfg = workflow_cfg.label.cp2k
-        if cp2k_cfg:
+
+        if cp2k_cfg and (iter_num > 0 or cp2k_cfg.init_systems):
             step_name = f'label-cp2k-iter-{iter_str}'
             runtime_ctx.label_app = 'cp2k'
             runtime_ctx.label_url = f's3://./label-cp2k/iter/{iter_str}'
-
             cp2k_executor = not_none(config.executors[not_none(config.orchestration.cp2k)])
-            if (iter_num > 0 or cp2k_cfg.init_systems) and \
-                    not step_switch.shall_skip(step_name):
+            if not step_switch.shall_skip(step_name):
                 if iter_num == 0:
                     assert cp2k_cfg.init_systems, 'init_systems should not be empty for first iteration'
                     assert runtime_ctx.screen_url is None, f'explore_url should be None for iter 0, actual: {runtime_ctx.screen_url}'
 
                 for sys_key in cp2k_cfg.init_systems:
                     sys = not_none(config.datasets[sys_key])
                     builder.s3_upload(sys.url, f'init-systems/{sys_key}', cache=True)
@@ -154,16 +163,18 @@
             raise ValueError('No screen app specified')
 
         if workflow_cfg.update:
             if iter_num == workflow_cfg.update.until_iter:
                 logger.info('Updating workflow config at iter %d', iter_num)
                 # the patch is applied to the original config, not the updated one
                 raw_workflow_cfg = deepcopy(config.workflow)
-                raw_workflow_cfg['workflow']['update'] = None  # clean the old update config
+                raw_workflow_cfg['update'] = None  # clean the old update config
                 raw_workflow_cfg = merge_dict(raw_workflow_cfg, workflow_cfg.update.patch)
 
-    builder.run()
+    return builder
+
+
 
 
 cmd_entry = CmdGroup({
     'run': run_tesla,
 }, doc='TESLA workflow')
```

### Comparing `dflow_galaxy-0.1.4/pyproject.toml` & `dflow_galaxy-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dflow-galaxy"
-version = "0.1.4"
+version = "0.1.5"
 description = ""
 authors = ["weihong.xu <xuweihong.cn@gmail.com>"]
 readme = "README.md"
 include = ["dflow_galaxy/res/*"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `dflow_galaxy-0.1.4/PKG-INFO` & `dflow_galaxy-0.1.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dflow-galaxy
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Author: weihong.xu
 Author-email: xuweihong.cn@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -17,22 +17,25 @@
 Requires-Dist: pydflow (==1.8.60)
 Description-Content-Type: text/markdown
 
 # DFlow Galaxy
 
 [![PyPI version](https://badge.fury.io/py/dflow-galaxy.svg)](https://badge.fury.io/py/dflow-galaxy)
 [![Downloads](https://pepy.tech/badge/dflow-galaxy)](https://pepy.tech/project/dflow-galaxy)
+[![Docker](https://img.shields.io/docker/v/link89/dflow-galaxy?label=docker&logo=docker)](https://hub.docker.com/repository/docker/link89/dflow-galaxy/general)
+
 
 Collection of workflows and tools built on top of DFlow and [ai2-kit](https://github.com/chenggroup/ai2-kit).
 
 ## Features
 * DFlowBuilder: A type friendly wrapper for `DFlow` to build workflows in a more intuitive way.
 * Workflows:
   * TESLA: a **T**raining-**E**xploration-**S**creening-**L**abeling workflow designed by **AI4EC**. Get inspired by [DPGEN](https://github.com/deepmodeling/dpgen), [DPGEN2](https://github.com/deepmodeling/dpgen2), ported from [ai2-kit](https://github.com/chenggroup/ai2-kit).
 
+
 ## Get Started
 `dflow-galaxy` requires Python 3.9+ since it depends on `typing.Annotated`.
 
 To use `dflow-galaxy` as a library, you can install it via pip:
 
 ```bash
 pip install dflow-galaxy
@@ -44,21 +47,27 @@
 poetry install
 poetry shell
 ```
 
 ## Bohrium Launch App
 This repository also contains some launch apps for Bohrium. The entry of the Bohrium launch app is in the `launch_app` directory, and relative modules are in the `dflow_galaxy/app` directory.
 
-To build docker image for the launch app, you can use the following command:
+Currently, the following launch apps are available:
 
-```bash
-./build-docker.sh
-```
-### Launch Apps
 * CP2K Lightning: Run CP2K without building input files from scratch.
-* DynaCat TESLA: An automated workflow to generated DeepMD potential for DynaCat. (TODO)
+* DynaCat TESLA: An automated workflow to generated DeepMD potential for DynaCat.
 * DynaCat MD: Run MD simulations with DeepMD potential for DynaCat. 
 
 
+## Distribution
+### PyPI
+```bash
+poetry publish --build
+```
+### Docker
+```bash
+./build-docker.sh
+```
+
 ## Manuals
 * [TESLA Workflow](doc/tesla.md)
```

