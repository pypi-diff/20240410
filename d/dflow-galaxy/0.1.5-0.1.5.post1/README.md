# Comparing `tmp/dflow_galaxy-0.1.5.tar.gz` & `tmp/dflow_galaxy-0.1.5.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dflow_galaxy-0.1.5.tar", max compression
+gzip compressed data, was "dflow_galaxy-0.1.5.post1.tar", max compression
```

## Comparing `dflow_galaxy-0.1.5.tar` & `dflow_galaxy-0.1.5.post1.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0    34523 2024-02-19 03:12:58.574253 dflow_galaxy-0.1.5/LICENSE
--rw-r--r--   0        0        0     1834 2024-04-09 15:45:18.275720 dflow_galaxy-0.1.5/README.md
--rw-r--r--   0        0        0        0 2024-01-30 01:22:58.649023 dflow_galaxy-0.1.5/dflow_galaxy/__init__.py
--rw-r--r--   0        0        0        0 2024-04-02 03:42:50.450085 dflow_galaxy-0.1.5/dflow_galaxy/app/__init__.py
--rw-r--r--   0        0        0     2499 2024-04-09 15:45:01.375722 dflow_galaxy-0.1.5/dflow_galaxy/app/common.py
--rw-r--r--   0        0        0        0 2024-04-02 03:42:50.450085 dflow_galaxy-0.1.5/dflow_galaxy/app/cp2k_lightning/__init__.py
--rw-r--r--   0        0        0     2047 2024-04-09 07:36:05.233859 dflow_galaxy-0.1.5/dflow_galaxy/app/cp2k_lightning/dflow.py
--rw-r--r--   0        0        0     6456 2024-04-07 14:10:40.795458 dflow_galaxy-0.1.5/dflow_galaxy/app/cp2k_lightning/main.py
--rw-r--r--   0        0        0        0 2024-04-07 12:32:16.436174 dflow_galaxy-0.1.5/dflow_galaxy/app/dynacat_md/__init__.py
--rw-r--r--   0        0        0     1910 2024-04-09 06:12:22.344468 dflow_galaxy-0.1.5/dflow_galaxy/app/dynacat_md/dflow.py
--rw-r--r--   0        0        0     4338 2024-04-09 15:45:01.375722 dflow_galaxy-0.1.5/dflow_galaxy/app/dynacat_md/main.py
--rw-r--r--   0        0        0        0 2024-04-02 03:42:50.450085 dflow_galaxy-0.1.5/dflow_galaxy/app/dynacat_tesla/__init__.py
--rw-r--r--   0        0        0    13473 2024-04-09 15:45:01.385722 dflow_galaxy-0.1.5/dflow_galaxy/app/dynacat_tesla/main.py
--rw-r--r--   0        0        0        0 2024-02-06 03:07:45.063120 dflow_galaxy-0.1.5/dflow_galaxy/core/__init__.py
--rw-r--r--   0        0        0    28431 2024-04-09 03:02:40.485846 dflow_galaxy-0.1.5/dflow_galaxy/core/dflow.py
--rw-r--r--   0        0        0     4683 2024-04-09 15:45:01.385722 dflow_galaxy-0.1.5/dflow_galaxy/core/dispatcher.py
--rw-r--r--   0        0        0      163 2024-02-06 03:07:45.063120 dflow_galaxy-0.1.5/dflow_galaxy/core/log.py
--rw-r--r--   0        0        0       97 2024-04-01 07:14:05.895738 dflow_galaxy-0.1.5/dflow_galaxy/core/pydantic.py
--rw-r--r--   0        0        0      541 2024-04-03 16:22:36.889294 dflow_galaxy-0.1.5/dflow_galaxy/core/types.py
--rw-r--r--   0        0        0     5603 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.5/dflow_galaxy/core/util.py
--rw-r--r--   0        0        0      335 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.5/dflow_galaxy/main.py
--rw-r--r--   0        0        0      146 2024-04-09 15:45:01.385722 dflow_galaxy-0.1.5/dflow_galaxy/res/__init__.py
--rw-r--r--   0        0        0   189331 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/ALL_BASIS_SETS
--rw-r--r--   0        0        0     2717 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/ALL_POTENTIALS
--rw-r--r--   0        0        0    15836 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/AcPP1_POTENTIALS
--rw-r--r--   0        0        0    57524 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_ADMM
--rw-r--r--   0        0        0   189911 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_ADMM_MOLOPT
--rw-r--r--   0        0        0   133011 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_ADMM_UZH
--rw-r--r--   0        0        0    66934 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_ADMM_ae
--rw-r--r--   0        0        0    17509 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_LRIGPW_AUXMOLOPT
--rw-r--r--   0        0        0   244853 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_MINBAS
--rw-r--r--   0        0        0    49588 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_MINIX
--rw-r--r--   0        0        0   127679 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT
--rw-r--r--   0        0        0    55644 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_AcPP1
--rw-r--r--   0        0        0    23527 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_LnPP1
--rw-r--r--   0        0        0    65485 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_LnPP2
--rw-r--r--   0        0        0   179850 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_UCL
--rw-r--r--   0        0        0  1574370 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_UZH
--rw-r--r--   0        0        0     6644 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_PERIODIC_GW
--rw-r--r--   0        0        0    37261 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_RI_cc-TZ
--rw-r--r--   0        0        0   195109 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_SET
--rw-r--r--   0        0        0     5526 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_ZIJLSTRA
--rw-r--r--   0        0        0   324291 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_ccGRB_UZH
--rw-r--r--   0        0        0   258169 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_def2_QZVP_RI_ALL
--rw-r--r--   0        0        0   191314 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_pob
--rw-r--r--   0        0        0   223481 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/ECP_POTENTIALS
--rw-r--r--   0        0        0    23668 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/ECP_POTENTIALS_pob-TZVP-rev2
--rw-r--r--   0        0        0  1713484 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/EMSL_BASIS_SETS
--rw-r--r--   0        0        0   119403 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/GTH_BASIS_SETS
--rw-r--r--   0        0        0   167483 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/GTH_POTENTIALS
--rw-r--r--   0        0        0   253677 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/GTH_SOC_POTENTIALS
--rw-r--r--   0        0        0    17275 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/HFX_BASIS
--rw-r--r--   0        0        0     2106 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/HF_POTENTIALS
--rw-r--r--   0        0        0     5486 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/LnPP1_POTENTIALS
--rw-r--r--   0        0        0     7829 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/LnPP2_POTENTIALS
--rw-r--r--   0        0        0      447 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/MM_POTENTIAL
--rw-r--r--   0        0        0     5498 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/NLCC_POTENTIALS
--rw-r--r--   0        0        0   177804 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/POTENTIAL
--rw-r--r--   0        0        0   385325 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/POTENTIAL_UZH
--rw-r--r--   0        0        0      125 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/README.md
--rw-r--r--   0        0        0    91811 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/nm12_parameters.xml
--rw-r--r--   0        0        0    32194 2024-04-02 03:42:50.640085 dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/xTB_parameters
--rw-r--r--   0        0        0     1171 2024-04-09 15:45:01.385722 dflow_galaxy-0.1.5/dflow_galaxy/res/dynacat/tesla_template.yml
--rw-r--r--   0        0        0        0 2024-02-07 08:30:41.445577 dflow_galaxy-0.1.5/dflow_galaxy/workflow/__init__.py
--rw-r--r--   0        0        0        0 2024-02-07 08:30:41.445577 dflow_galaxy-0.1.5/dflow_galaxy/workflow/tesla/__init__.py
--rw-r--r--   0        0        0     1702 2024-04-09 15:45:01.385722 dflow_galaxy-0.1.5/dflow_galaxy/workflow/tesla/config.py
--rw-r--r--   0        0        0        0 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.5/dflow_galaxy/workflow/tesla/domain/__init__.py
--rw-r--r--   0        0        0        0 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.5/dflow_galaxy/workflow/tesla/domain/abacus.py
--rw-r--r--   0        0        0     6298 2024-04-02 03:42:50.640085 dflow_galaxy-0.1.5/dflow_galaxy/workflow/tesla/domain/cp2k.py
--rw-r--r--   0        0        0     9775 2024-04-09 14:05:23.796450 dflow_galaxy-0.1.5/dflow_galaxy/workflow/tesla/domain/deepmd.py
--rw-r--r--   0        0        0     8016 2024-04-02 03:42:50.640085 dflow_galaxy-0.1.5/dflow_galaxy/workflow/tesla/domain/lammps.py
--rw-r--r--   0        0        0     1261 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.5/dflow_galaxy/workflow/tesla/domain/lib.py
--rw-r--r--   0        0        0     6334 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.5/dflow_galaxy/workflow/tesla/domain/model_devi.py
--rw-r--r--   0        0        0     8185 2024-04-09 15:45:01.385722 dflow_galaxy-0.1.5/dflow_galaxy/workflow/tesla/main.py
--rw-r--r--   0        0        0      541 2024-04-09 15:49:46.375684 dflow_galaxy-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2479 1970-01-01 00:00:00.000000 dflow_galaxy-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-02-19 03:12:58.574253 dflow_galaxy-0.1.5.post1/LICENSE
+-rw-r--r--   0        0        0     1834 2024-04-09 15:45:18.275720 dflow_galaxy-0.1.5.post1/README.md
+-rw-r--r--   0        0        0        0 2024-01-30 01:22:58.649023 dflow_galaxy-0.1.5.post1/dflow_galaxy/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-02 03:42:50.450085 dflow_galaxy-0.1.5.post1/dflow_galaxy/app/__init__.py
+-rw-r--r--   0        0        0     2499 2024-04-09 15:45:01.375722 dflow_galaxy-0.1.5.post1/dflow_galaxy/app/common.py
+-rw-r--r--   0        0        0        0 2024-04-02 03:42:50.450085 dflow_galaxy-0.1.5.post1/dflow_galaxy/app/cp2k_lightning/__init__.py
+-rw-r--r--   0        0        0     2047 2024-04-09 07:36:05.233859 dflow_galaxy-0.1.5.post1/dflow_galaxy/app/cp2k_lightning/dflow.py
+-rw-r--r--   0        0        0     6456 2024-04-07 14:10:40.795458 dflow_galaxy-0.1.5.post1/dflow_galaxy/app/cp2k_lightning/main.py
+-rw-r--r--   0        0        0        0 2024-04-07 12:32:16.436174 dflow_galaxy-0.1.5.post1/dflow_galaxy/app/dynacat_md/__init__.py
+-rw-r--r--   0        0        0     1910 2024-04-09 06:12:22.344468 dflow_galaxy-0.1.5.post1/dflow_galaxy/app/dynacat_md/dflow.py
+-rw-r--r--   0        0        0     4338 2024-04-10 01:12:26.524183 dflow_galaxy-0.1.5.post1/dflow_galaxy/app/dynacat_md/main.py
+-rw-r--r--   0        0        0        0 2024-04-02 03:42:50.450085 dflow_galaxy-0.1.5.post1/dflow_galaxy/app/dynacat_tesla/__init__.py
+-rw-r--r--   0        0        0    14450 2024-04-10 01:12:36.204179 dflow_galaxy-0.1.5.post1/dflow_galaxy/app/dynacat_tesla/main.py
+-rw-r--r--   0        0        0        0 2024-02-06 03:07:45.063120 dflow_galaxy-0.1.5.post1/dflow_galaxy/core/__init__.py
+-rw-r--r--   0        0        0    28431 2024-04-09 03:02:40.485846 dflow_galaxy-0.1.5.post1/dflow_galaxy/core/dflow.py
+-rw-r--r--   0        0        0     4683 2024-04-09 15:45:01.385722 dflow_galaxy-0.1.5.post1/dflow_galaxy/core/dispatcher.py
+-rw-r--r--   0        0        0      163 2024-02-06 03:07:45.063120 dflow_galaxy-0.1.5.post1/dflow_galaxy/core/log.py
+-rw-r--r--   0        0        0       97 2024-04-01 07:14:05.895738 dflow_galaxy-0.1.5.post1/dflow_galaxy/core/pydantic.py
+-rw-r--r--   0        0        0      541 2024-04-03 16:22:36.889294 dflow_galaxy-0.1.5.post1/dflow_galaxy/core/types.py
+-rw-r--r--   0        0        0     5603 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.5.post1/dflow_galaxy/core/util.py
+-rw-r--r--   0        0        0      335 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.5.post1/dflow_galaxy/main.py
+-rw-r--r--   0        0        0      146 2024-04-09 15:45:01.385722 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/__init__.py
+-rw-r--r--   0        0        0   189331 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/ALL_BASIS_SETS
+-rw-r--r--   0        0        0     2717 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/ALL_POTENTIALS
+-rw-r--r--   0        0        0    15836 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/AcPP1_POTENTIALS
+-rw-r--r--   0        0        0    57524 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_ADMM
+-rw-r--r--   0        0        0   189911 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_ADMM_MOLOPT
+-rw-r--r--   0        0        0   133011 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_ADMM_UZH
+-rw-r--r--   0        0        0    66934 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_ADMM_ae
+-rw-r--r--   0        0        0    17509 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_LRIGPW_AUXMOLOPT
+-rw-r--r--   0        0        0   244853 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_MINBAS
+-rw-r--r--   0        0        0    49588 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_MINIX
+-rw-r--r--   0        0        0   127679 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT
+-rw-r--r--   0        0        0    55644 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_AcPP1
+-rw-r--r--   0        0        0    23527 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_LnPP1
+-rw-r--r--   0        0        0    65485 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_LnPP2
+-rw-r--r--   0        0        0   179850 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_UCL
+-rw-r--r--   0        0        0  1574370 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_UZH
+-rw-r--r--   0        0        0     6644 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_PERIODIC_GW
+-rw-r--r--   0        0        0    37261 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_RI_cc-TZ
+-rw-r--r--   0        0        0   195109 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_SET
+-rw-r--r--   0        0        0     5526 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_ZIJLSTRA
+-rw-r--r--   0        0        0   324291 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_ccGRB_UZH
+-rw-r--r--   0        0        0   258169 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_def2_QZVP_RI_ALL
+-rw-r--r--   0        0        0   191314 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_pob
+-rw-r--r--   0        0        0   223481 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/ECP_POTENTIALS
+-rw-r--r--   0        0        0    23668 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/ECP_POTENTIALS_pob-TZVP-rev2
+-rw-r--r--   0        0        0  1713484 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/EMSL_BASIS_SETS
+-rw-r--r--   0        0        0   119403 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/GTH_BASIS_SETS
+-rw-r--r--   0        0        0   167483 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/GTH_POTENTIALS
+-rw-r--r--   0        0        0   253677 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/GTH_SOC_POTENTIALS
+-rw-r--r--   0        0        0    17275 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/HFX_BASIS
+-rw-r--r--   0        0        0     2106 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/HF_POTENTIALS
+-rw-r--r--   0        0        0     5486 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/LnPP1_POTENTIALS
+-rw-r--r--   0        0        0     7829 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/LnPP2_POTENTIALS
+-rw-r--r--   0        0        0      447 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/MM_POTENTIAL
+-rw-r--r--   0        0        0     5498 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/NLCC_POTENTIALS
+-rw-r--r--   0        0        0   177804 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/POTENTIAL
+-rw-r--r--   0        0        0   385325 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/POTENTIAL_UZH
+-rw-r--r--   0        0        0      125 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/README.md
+-rw-r--r--   0        0        0    91811 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/nm12_parameters.xml
+-rw-r--r--   0        0        0    32194 2024-04-02 03:42:50.640085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/xTB_parameters
+-rw-r--r--   0        0        0     1171 2024-04-09 15:45:01.385722 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/dynacat/tesla_template.yml
+-rw-r--r--   0        0        0        0 2024-02-07 08:30:41.445577 dflow_galaxy-0.1.5.post1/dflow_galaxy/workflow/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-07 08:30:41.445577 dflow_galaxy-0.1.5.post1/dflow_galaxy/workflow/tesla/__init__.py
+-rw-r--r--   0        0        0     1702 2024-04-09 15:45:01.385722 dflow_galaxy-0.1.5.post1/dflow_galaxy/workflow/tesla/config.py
+-rw-r--r--   0        0        0        0 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.5.post1/dflow_galaxy/workflow/tesla/domain/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.5.post1/dflow_galaxy/workflow/tesla/domain/abacus.py
+-rw-r--r--   0        0        0     6298 2024-04-02 03:42:50.640085 dflow_galaxy-0.1.5.post1/dflow_galaxy/workflow/tesla/domain/cp2k.py
+-rw-r--r--   0        0        0     9775 2024-04-09 14:05:23.796450 dflow_galaxy-0.1.5.post1/dflow_galaxy/workflow/tesla/domain/deepmd.py
+-rw-r--r--   0        0        0     8016 2024-04-02 03:42:50.640085 dflow_galaxy-0.1.5.post1/dflow_galaxy/workflow/tesla/domain/lammps.py
+-rw-r--r--   0        0        0     1261 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.5.post1/dflow_galaxy/workflow/tesla/domain/lib.py
+-rw-r--r--   0        0        0     6334 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.5.post1/dflow_galaxy/workflow/tesla/domain/model_devi.py
+-rw-r--r--   0        0        0     8185 2024-04-09 15:45:01.385722 dflow_galaxy-0.1.5.post1/dflow_galaxy/workflow/tesla/main.py
+-rw-r--r--   0        0        0      547 2024-04-10 01:34:21.744146 dflow_galaxy-0.1.5.post1/pyproject.toml
+-rw-r--r--   0        0        0     2485 1970-01-01 00:00:00.000000 dflow_galaxy-0.1.5.post1/PKG-INFO
```

### Comparing `dflow_galaxy-0.1.5/LICENSE` & `dflow_galaxy-0.1.5.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5/README.md` & `dflow_galaxy-0.1.5.post1/README.md`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5/dflow_galaxy/app/common.py` & `dflow_galaxy-0.1.5.post1/dflow_galaxy/app/common.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5/dflow_galaxy/app/cp2k_lightning/dflow.py` & `dflow_galaxy-0.1.5.post1/dflow_galaxy/app/cp2k_lightning/dflow.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5/dflow_galaxy/app/cp2k_lightning/main.py` & `dflow_galaxy-0.1.5.post1/dflow_galaxy/app/cp2k_lightning/main.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5/dflow_galaxy/app/dynacat_md/dflow.py` & `dflow_galaxy-0.1.5.post1/dflow_galaxy/app/dynacat_md/dflow.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5/dflow_galaxy/app/dynacat_md/main.py` & `dflow_galaxy-0.1.5.post1/dflow_galaxy/app/dynacat_md/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     )
 
     output_dir : OutputDirectory = Field(
         default='./output',
         description="Output directory of LAMMPS simulation")
 
     lammps_image: String = Field(
-        default='registry.dp.tech/dptech/dpmd:2.2.8-cuda11.8',
+        default='registry.dp.tech/dptech/dpmd:2.2.8-cuda12.0',
         description="Docker image for running LAMMPS simulation")
 
     lammps_device_model: String = Field(
         default='c8_m32_1 * NVIDIA V100',
         description="Device model for LAMMPS simulation")
 
     lammps_script: String = Field(
```

### Comparing `dflow_galaxy-0.1.5/dflow_galaxy/app/dynacat_tesla/main.py` & `dflow_galaxy-0.1.5.post1/dflow_galaxy/app/dynacat_tesla/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 
 
 logger = get_logger(__name__)
 
 
 BH_DEEPMD_DEFAULT = {
-    'image_name': 'registry.dp.tech/dptech/dpmd:2.2.8-cuda11.8',
+    'image_name': 'registry.dp.tech/dptech/dpmd:2.2.8-cuda12.0',
     'scass_type': 'c8_m32_1 * NVIDIA V100',
 }
 BH_LAMMPS_DEFAULT = BH_DEEPMD_DEFAULT
 
 BH_CP2K_DEFAULT = {
     'image_name': 'registry.dp.tech/dptech/cp2k:11',
     'scass_type': 'c32_m64_cpu',
@@ -76,14 +76,19 @@
         default=4,
         description="Number of concurrent run")
 
     cmd: String = Field(
         default='dp',
         description="Command to run DeepMD, note that it depends on the docker image you used")
 
+    setup_script: String = Field(
+        default='',
+        format='multi-line',
+        description="Setup script for DeepMD simulation, note that it depends on the docker image you used")
+
 
 class LammpsSetting(BaseModel):
     system_file: InputFilePath = Field(
         description="Structure file in xyz format use for LAMMPS simulation")
 
     ensemble: EnsembleOptions = Field(
         default=EnsembleOptions.csvr,
@@ -132,14 +137,19 @@
         default=5,
         description="Number of concurrent run")
 
     cmd: String = Field(
         default='lmp',
         description="Command to run LAMMPS, note that it depends on the docker image you used")
 
+    setup_script: String = Field(
+        default='',
+        format='multi-line',
+        description="Setup script for LAMMPS simulation, note that it depends on the docker image you used")
+
 
 class ModelDeviation(BaseModel):
     lo: Float = Field(
         default=0.2,
         description="Lower bound of the deviation")
 
     hi: Float = Field(
@@ -163,14 +173,23 @@
         default=5,
         description="Number of concurrent run")
 
     cmd: String = Field(
         default='mpirun -np 32 cp2k.popt',
         description="Script to run CP2K simulation, note that it depends on the docker image")
 
+    setup_script: String = Field(
+        default = '\n'.join([
+            '# guess cp2k data dir',
+            '[[ -z "${CP2K_DATA_DIR}" ]] && export CP2K_DATA_DIR="$(dirname "$(which cp2k)")/../../data" || true',
+            'source /opt/cp2k-toolchain/install/setup',
+        ]),
+        format='multi-line',
+        description="Setup script for CP2K simulation, note that it depends on the docker image you used")
+
 
 class DynacatTeslaArgs(DFlowOptions):
 
     dry_run: Boolean = Field(
         default = True,
         description="Generate configuration file without running the simulation")
 
@@ -251,16 +270,20 @@
     try:
         workflow.run()
     except:
         logger.exception('Failed to run workflow')
         return 1
     finally:
         # reclaim useful data
-        workflow.s3_download('iter-dataset', args.output_dir)
-        workflow.s3_download('train-deepmd', args.output_dir)
+        dp_dataset_dir = os.path.join(args.output_dir, 'dp-dataset')
+        dp_models_dir = os.path.join(args.output_dir, 'dp-models')
+        os.makedirs(dp_dataset_dir, exist_ok=True)
+        os.makedirs(dp_models_dir, exist_ok=True)
+        workflow.s3_download('iter-dataset', dp_dataset_dir)
+        workflow.s3_download('train-deepmd', dp_models_dir)
     return 0
 
 
 def _get_executor_config(args: DynacatTeslaArgs):
     return {
         'executors': {
             'bohrium': {
@@ -273,33 +296,31 @@
                     },
                     'deepmd': {
                         'resource': {
                             'bohrium': args.deepmd_resource,
                         },
                         'dp_cmd': args.deepmd.cmd,
                         'concurrency': args.deepmd.concurrency,
-
+                        'setup_script': args.deepmd.setup_script,
                     },
                     'lammps': {
                         'resource': {
                             'bohrium': args.lammps_resource,
                         },
                         'lammps_cmd': args.lammps.cmd,
                         'concurrency': args.lammps.concurrency,
+                        'setup_script': args.lammps.setup_script,
                     },
                     'cp2k': {
                         'resource': {
                             'bohrium': args.cp2k_resource,
                         },
                         'cp2k_cmd': args.cp2k.cmd,
                         'concurrency': args.cp2k.concurrency,
-                        'setup_script': '\n'.join([
-                            # guess cp2k data dir
-                            '[[ -z "${CP2K_DATA_DIR}" ]] && export CP2K_DATA_DIR="$(dirname "$(which cp2k)")/../../data" || true',
-                        ])
+                        'setup_script':  args.cp2k.setup_script,
                     }
                 }
             }
         },
         'orchestration': {
             'deepmd': 'bohrium',
             'lammps': 'bohrium',
```

### Comparing `dflow_galaxy-0.1.5/dflow_galaxy/core/dflow.py` & `dflow_galaxy-0.1.5.post1/dflow_galaxy/core/dflow.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5/dflow_galaxy/core/dispatcher.py` & `dflow_galaxy-0.1.5.post1/dflow_galaxy/core/dispatcher.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5/dflow_galaxy/core/types.py` & `dflow_galaxy-0.1.5.post1/dflow_galaxy/core/types.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5/dflow_galaxy/core/util.py` & `dflow_galaxy-0.1.5.post1/dflow_galaxy/core/util.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/ALL_BASIS_SETS` & `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/ALL_BASIS_SETS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/ALL_POTENTIALS` & `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/ALL_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/AcPP1_POTENTIALS` & `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/AcPP1_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_ADMM` & `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_ADMM`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_ADMM_MOLOPT` & `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_ADMM_MOLOPT`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_ADMM_UZH` & `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_ADMM_UZH`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_ADMM_ae` & `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_ADMM_ae`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_LRIGPW_AUXMOLOPT` & `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_LRIGPW_AUXMOLOPT`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_MINBAS` & `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_MINBAS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_MINIX` & `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_MINIX`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT` & `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_AcPP1` & `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_AcPP1`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_LnPP1` & `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_LnPP1`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_LnPP2` & `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_LnPP2`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_UCL` & `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_UCL`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_UZH` & `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_UZH`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_PERIODIC_GW` & `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_PERIODIC_GW`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_RI_cc-TZ` & `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_RI_cc-TZ`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_SET` & `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_SET`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_ZIJLSTRA` & `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_ZIJLSTRA`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_ccGRB_UZH` & `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_ccGRB_UZH`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_def2_QZVP_RI_ALL` & `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_def2_QZVP_RI_ALL`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/BASIS_pob` & `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_pob`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/ECP_POTENTIALS` & `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/ECP_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/ECP_POTENTIALS_pob-TZVP-rev2` & `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/ECP_POTENTIALS_pob-TZVP-rev2`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/EMSL_BASIS_SETS` & `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/EMSL_BASIS_SETS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/GTH_BASIS_SETS` & `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/GTH_BASIS_SETS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/GTH_POTENTIALS` & `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/GTH_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/GTH_SOC_POTENTIALS` & `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/GTH_SOC_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/HFX_BASIS` & `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/HFX_BASIS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/HF_POTENTIALS` & `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/HF_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/LnPP1_POTENTIALS` & `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/LnPP1_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/LnPP2_POTENTIALS` & `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/LnPP2_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/NLCC_POTENTIALS` & `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/NLCC_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/POTENTIAL` & `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/POTENTIAL`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/POTENTIAL_UZH` & `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/POTENTIAL_UZH`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/nm12_parameters.xml` & `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/nm12_parameters.xml`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5/dflow_galaxy/res/cp2k_data/xTB_parameters` & `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/xTB_parameters`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5/dflow_galaxy/res/dynacat/tesla_template.yml` & `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/dynacat/tesla_template.yml`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5/dflow_galaxy/workflow/tesla/config.py` & `dflow_galaxy-0.1.5.post1/dflow_galaxy/workflow/tesla/config.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5/dflow_galaxy/workflow/tesla/domain/cp2k.py` & `dflow_galaxy-0.1.5.post1/dflow_galaxy/workflow/tesla/domain/cp2k.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5/dflow_galaxy/workflow/tesla/domain/deepmd.py` & `dflow_galaxy-0.1.5.post1/dflow_galaxy/workflow/tesla/domain/deepmd.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5/dflow_galaxy/workflow/tesla/domain/lammps.py` & `dflow_galaxy-0.1.5.post1/dflow_galaxy/workflow/tesla/domain/lammps.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5/dflow_galaxy/workflow/tesla/domain/lib.py` & `dflow_galaxy-0.1.5.post1/dflow_galaxy/workflow/tesla/domain/lib.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5/dflow_galaxy/workflow/tesla/domain/model_devi.py` & `dflow_galaxy-0.1.5.post1/dflow_galaxy/workflow/tesla/domain/model_devi.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5/dflow_galaxy/workflow/tesla/main.py` & `dflow_galaxy-0.1.5.post1/dflow_galaxy/workflow/tesla/main.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5/pyproject.toml` & `dflow_galaxy-0.1.5.post1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dflow-galaxy"
-version = "0.1.5"
+version = "0.1.5.post1"
 description = ""
 authors = ["weihong.xu <xuweihong.cn@gmail.com>"]
 readme = "README.md"
 include = ["dflow_galaxy/res/*"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `dflow_galaxy-0.1.5/PKG-INFO` & `dflow_galaxy-0.1.5.post1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dflow-galaxy
-Version: 0.1.5
+Version: 0.1.5.post1
 Summary: 
 Author: weihong.xu
 Author-email: xuweihong.cn@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

