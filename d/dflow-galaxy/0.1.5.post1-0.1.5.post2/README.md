# Comparing `tmp/dflow_galaxy-0.1.5.post1.tar.gz` & `tmp/dflow_galaxy-0.1.5.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dflow_galaxy-0.1.5.post1.tar", max compression
+gzip compressed data, was "dflow_galaxy-0.1.5.post2.tar", max compression
```

## Comparing `dflow_galaxy-0.1.5.post1.tar` & `dflow_galaxy-0.1.5.post2.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0    34523 2024-02-19 03:12:58.574253 dflow_galaxy-0.1.5.post1/LICENSE
--rw-r--r--   0        0        0     1834 2024-04-09 15:45:18.275720 dflow_galaxy-0.1.5.post1/README.md
--rw-r--r--   0        0        0        0 2024-01-30 01:22:58.649023 dflow_galaxy-0.1.5.post1/dflow_galaxy/__init__.py
--rw-r--r--   0        0        0        0 2024-04-02 03:42:50.450085 dflow_galaxy-0.1.5.post1/dflow_galaxy/app/__init__.py
--rw-r--r--   0        0        0     2499 2024-04-09 15:45:01.375722 dflow_galaxy-0.1.5.post1/dflow_galaxy/app/common.py
--rw-r--r--   0        0        0        0 2024-04-02 03:42:50.450085 dflow_galaxy-0.1.5.post1/dflow_galaxy/app/cp2k_lightning/__init__.py
--rw-r--r--   0        0        0     2047 2024-04-09 07:36:05.233859 dflow_galaxy-0.1.5.post1/dflow_galaxy/app/cp2k_lightning/dflow.py
--rw-r--r--   0        0        0     6456 2024-04-07 14:10:40.795458 dflow_galaxy-0.1.5.post1/dflow_galaxy/app/cp2k_lightning/main.py
--rw-r--r--   0        0        0        0 2024-04-07 12:32:16.436174 dflow_galaxy-0.1.5.post1/dflow_galaxy/app/dynacat_md/__init__.py
--rw-r--r--   0        0        0     1910 2024-04-09 06:12:22.344468 dflow_galaxy-0.1.5.post1/dflow_galaxy/app/dynacat_md/dflow.py
--rw-r--r--   0        0        0     4338 2024-04-10 01:12:26.524183 dflow_galaxy-0.1.5.post1/dflow_galaxy/app/dynacat_md/main.py
--rw-r--r--   0        0        0        0 2024-04-02 03:42:50.450085 dflow_galaxy-0.1.5.post1/dflow_galaxy/app/dynacat_tesla/__init__.py
--rw-r--r--   0        0        0    14450 2024-04-10 01:12:36.204179 dflow_galaxy-0.1.5.post1/dflow_galaxy/app/dynacat_tesla/main.py
--rw-r--r--   0        0        0        0 2024-02-06 03:07:45.063120 dflow_galaxy-0.1.5.post1/dflow_galaxy/core/__init__.py
--rw-r--r--   0        0        0    28431 2024-04-09 03:02:40.485846 dflow_galaxy-0.1.5.post1/dflow_galaxy/core/dflow.py
--rw-r--r--   0        0        0     4683 2024-04-09 15:45:01.385722 dflow_galaxy-0.1.5.post1/dflow_galaxy/core/dispatcher.py
--rw-r--r--   0        0        0      163 2024-02-06 03:07:45.063120 dflow_galaxy-0.1.5.post1/dflow_galaxy/core/log.py
--rw-r--r--   0        0        0       97 2024-04-01 07:14:05.895738 dflow_galaxy-0.1.5.post1/dflow_galaxy/core/pydantic.py
--rw-r--r--   0        0        0      541 2024-04-03 16:22:36.889294 dflow_galaxy-0.1.5.post1/dflow_galaxy/core/types.py
--rw-r--r--   0        0        0     5603 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.5.post1/dflow_galaxy/core/util.py
--rw-r--r--   0        0        0      335 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.5.post1/dflow_galaxy/main.py
--rw-r--r--   0        0        0      146 2024-04-09 15:45:01.385722 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/__init__.py
--rw-r--r--   0        0        0   189331 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/ALL_BASIS_SETS
--rw-r--r--   0        0        0     2717 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/ALL_POTENTIALS
--rw-r--r--   0        0        0    15836 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/AcPP1_POTENTIALS
--rw-r--r--   0        0        0    57524 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_ADMM
--rw-r--r--   0        0        0   189911 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_ADMM_MOLOPT
--rw-r--r--   0        0        0   133011 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_ADMM_UZH
--rw-r--r--   0        0        0    66934 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_ADMM_ae
--rw-r--r--   0        0        0    17509 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_LRIGPW_AUXMOLOPT
--rw-r--r--   0        0        0   244853 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_MINBAS
--rw-r--r--   0        0        0    49588 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_MINIX
--rw-r--r--   0        0        0   127679 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT
--rw-r--r--   0        0        0    55644 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_AcPP1
--rw-r--r--   0        0        0    23527 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_LnPP1
--rw-r--r--   0        0        0    65485 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_LnPP2
--rw-r--r--   0        0        0   179850 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_UCL
--rw-r--r--   0        0        0  1574370 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_UZH
--rw-r--r--   0        0        0     6644 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_PERIODIC_GW
--rw-r--r--   0        0        0    37261 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_RI_cc-TZ
--rw-r--r--   0        0        0   195109 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_SET
--rw-r--r--   0        0        0     5526 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_ZIJLSTRA
--rw-r--r--   0        0        0   324291 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_ccGRB_UZH
--rw-r--r--   0        0        0   258169 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_def2_QZVP_RI_ALL
--rw-r--r--   0        0        0   191314 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_pob
--rw-r--r--   0        0        0   223481 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/ECP_POTENTIALS
--rw-r--r--   0        0        0    23668 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/ECP_POTENTIALS_pob-TZVP-rev2
--rw-r--r--   0        0        0  1713484 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/EMSL_BASIS_SETS
--rw-r--r--   0        0        0   119403 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/GTH_BASIS_SETS
--rw-r--r--   0        0        0   167483 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/GTH_POTENTIALS
--rw-r--r--   0        0        0   253677 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/GTH_SOC_POTENTIALS
--rw-r--r--   0        0        0    17275 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/HFX_BASIS
--rw-r--r--   0        0        0     2106 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/HF_POTENTIALS
--rw-r--r--   0        0        0     5486 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/LnPP1_POTENTIALS
--rw-r--r--   0        0        0     7829 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/LnPP2_POTENTIALS
--rw-r--r--   0        0        0      447 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/MM_POTENTIAL
--rw-r--r--   0        0        0     5498 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/NLCC_POTENTIALS
--rw-r--r--   0        0        0   177804 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/POTENTIAL
--rw-r--r--   0        0        0   385325 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/POTENTIAL_UZH
--rw-r--r--   0        0        0      125 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/README.md
--rw-r--r--   0        0        0    91811 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/nm12_parameters.xml
--rw-r--r--   0        0        0    32194 2024-04-02 03:42:50.640085 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/xTB_parameters
--rw-r--r--   0        0        0     1171 2024-04-09 15:45:01.385722 dflow_galaxy-0.1.5.post1/dflow_galaxy/res/dynacat/tesla_template.yml
--rw-r--r--   0        0        0        0 2024-02-07 08:30:41.445577 dflow_galaxy-0.1.5.post1/dflow_galaxy/workflow/__init__.py
--rw-r--r--   0        0        0        0 2024-02-07 08:30:41.445577 dflow_galaxy-0.1.5.post1/dflow_galaxy/workflow/tesla/__init__.py
--rw-r--r--   0        0        0     1702 2024-04-09 15:45:01.385722 dflow_galaxy-0.1.5.post1/dflow_galaxy/workflow/tesla/config.py
--rw-r--r--   0        0        0        0 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.5.post1/dflow_galaxy/workflow/tesla/domain/__init__.py
--rw-r--r--   0        0        0        0 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.5.post1/dflow_galaxy/workflow/tesla/domain/abacus.py
--rw-r--r--   0        0        0     6298 2024-04-02 03:42:50.640085 dflow_galaxy-0.1.5.post1/dflow_galaxy/workflow/tesla/domain/cp2k.py
--rw-r--r--   0        0        0     9775 2024-04-09 14:05:23.796450 dflow_galaxy-0.1.5.post1/dflow_galaxy/workflow/tesla/domain/deepmd.py
--rw-r--r--   0        0        0     8016 2024-04-02 03:42:50.640085 dflow_galaxy-0.1.5.post1/dflow_galaxy/workflow/tesla/domain/lammps.py
--rw-r--r--   0        0        0     1261 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.5.post1/dflow_galaxy/workflow/tesla/domain/lib.py
--rw-r--r--   0        0        0     6334 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.5.post1/dflow_galaxy/workflow/tesla/domain/model_devi.py
--rw-r--r--   0        0        0     8185 2024-04-09 15:45:01.385722 dflow_galaxy-0.1.5.post1/dflow_galaxy/workflow/tesla/main.py
--rw-r--r--   0        0        0      547 2024-04-10 01:34:21.744146 dflow_galaxy-0.1.5.post1/pyproject.toml
--rw-r--r--   0        0        0     2485 1970-01-01 00:00:00.000000 dflow_galaxy-0.1.5.post1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-02-19 03:12:58.574253 dflow_galaxy-0.1.5.post2/LICENSE
+-rw-r--r--   0        0        0     1834 2024-04-09 15:45:18.275720 dflow_galaxy-0.1.5.post2/README.md
+-rw-r--r--   0        0        0        0 2024-01-30 01:22:58.649023 dflow_galaxy-0.1.5.post2/dflow_galaxy/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-02 03:42:50.450085 dflow_galaxy-0.1.5.post2/dflow_galaxy/app/__init__.py
+-rw-r--r--   0        0        0     2499 2024-04-09 15:45:01.375722 dflow_galaxy-0.1.5.post2/dflow_galaxy/app/common.py
+-rw-r--r--   0        0        0        0 2024-04-02 03:42:50.450085 dflow_galaxy-0.1.5.post2/dflow_galaxy/app/cp2k_lightning/__init__.py
+-rw-r--r--   0        0        0     2047 2024-04-09 07:36:05.233859 dflow_galaxy-0.1.5.post2/dflow_galaxy/app/cp2k_lightning/dflow.py
+-rw-r--r--   0        0        0     6456 2024-04-07 14:10:40.795458 dflow_galaxy-0.1.5.post2/dflow_galaxy/app/cp2k_lightning/main.py
+-rw-r--r--   0        0        0        0 2024-04-07 12:32:16.436174 dflow_galaxy-0.1.5.post2/dflow_galaxy/app/dynacat_md/__init__.py
+-rw-r--r--   0        0        0     1910 2024-04-09 06:12:22.344468 dflow_galaxy-0.1.5.post2/dflow_galaxy/app/dynacat_md/dflow.py
+-rw-r--r--   0        0        0     4338 2024-04-10 01:12:26.524183 dflow_galaxy-0.1.5.post2/dflow_galaxy/app/dynacat_md/main.py
+-rw-r--r--   0        0        0        0 2024-04-02 03:42:50.450085 dflow_galaxy-0.1.5.post2/dflow_galaxy/app/dynacat_tesla/__init__.py
+-rw-r--r--   0        0        0    14589 2024-04-10 02:22:31.884074 dflow_galaxy-0.1.5.post2/dflow_galaxy/app/dynacat_tesla/main.py
+-rw-r--r--   0        0        0        0 2024-02-06 03:07:45.063120 dflow_galaxy-0.1.5.post2/dflow_galaxy/core/__init__.py
+-rw-r--r--   0        0        0    28431 2024-04-09 03:02:40.485846 dflow_galaxy-0.1.5.post2/dflow_galaxy/core/dflow.py
+-rw-r--r--   0        0        0     4683 2024-04-09 15:45:01.385722 dflow_galaxy-0.1.5.post2/dflow_galaxy/core/dispatcher.py
+-rw-r--r--   0        0        0      163 2024-02-06 03:07:45.063120 dflow_galaxy-0.1.5.post2/dflow_galaxy/core/log.py
+-rw-r--r--   0        0        0       97 2024-04-01 07:14:05.895738 dflow_galaxy-0.1.5.post2/dflow_galaxy/core/pydantic.py
+-rw-r--r--   0        0        0      541 2024-04-03 16:22:36.889294 dflow_galaxy-0.1.5.post2/dflow_galaxy/core/types.py
+-rw-r--r--   0        0        0     5603 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.5.post2/dflow_galaxy/core/util.py
+-rw-r--r--   0        0        0      335 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.5.post2/dflow_galaxy/main.py
+-rw-r--r--   0        0        0      146 2024-04-09 15:45:01.385722 dflow_galaxy-0.1.5.post2/dflow_galaxy/res/__init__.py
+-rw-r--r--   0        0        0   189331 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/ALL_BASIS_SETS
+-rw-r--r--   0        0        0     2717 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/ALL_POTENTIALS
+-rw-r--r--   0        0        0    15836 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/AcPP1_POTENTIALS
+-rw-r--r--   0        0        0    57524 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/BASIS_ADMM
+-rw-r--r--   0        0        0   189911 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/BASIS_ADMM_MOLOPT
+-rw-r--r--   0        0        0   133011 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/BASIS_ADMM_UZH
+-rw-r--r--   0        0        0    66934 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/BASIS_ADMM_ae
+-rw-r--r--   0        0        0    17509 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/BASIS_LRIGPW_AUXMOLOPT
+-rw-r--r--   0        0        0   244853 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/BASIS_MINBAS
+-rw-r--r--   0        0        0    49588 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/BASIS_MINIX
+-rw-r--r--   0        0        0   127679 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT
+-rw-r--r--   0        0        0    55644 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_AcPP1
+-rw-r--r--   0        0        0    23527 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_LnPP1
+-rw-r--r--   0        0        0    65485 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_LnPP2
+-rw-r--r--   0        0        0   179850 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_UCL
+-rw-r--r--   0        0        0  1574370 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_UZH
+-rw-r--r--   0        0        0     6644 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/BASIS_PERIODIC_GW
+-rw-r--r--   0        0        0    37261 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/BASIS_RI_cc-TZ
+-rw-r--r--   0        0        0   195109 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/BASIS_SET
+-rw-r--r--   0        0        0     5526 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/BASIS_ZIJLSTRA
+-rw-r--r--   0        0        0   324291 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/BASIS_ccGRB_UZH
+-rw-r--r--   0        0        0   258169 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/BASIS_def2_QZVP_RI_ALL
+-rw-r--r--   0        0        0   191314 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/BASIS_pob
+-rw-r--r--   0        0        0   223481 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/ECP_POTENTIALS
+-rw-r--r--   0        0        0    23668 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/ECP_POTENTIALS_pob-TZVP-rev2
+-rw-r--r--   0        0        0  1713484 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/EMSL_BASIS_SETS
+-rw-r--r--   0        0        0   119403 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/GTH_BASIS_SETS
+-rw-r--r--   0        0        0   167483 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/GTH_POTENTIALS
+-rw-r--r--   0        0        0   253677 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/GTH_SOC_POTENTIALS
+-rw-r--r--   0        0        0    17275 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/HFX_BASIS
+-rw-r--r--   0        0        0     2106 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/HF_POTENTIALS
+-rw-r--r--   0        0        0     5486 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/LnPP1_POTENTIALS
+-rw-r--r--   0        0        0     7829 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/LnPP2_POTENTIALS
+-rw-r--r--   0        0        0      447 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/MM_POTENTIAL
+-rw-r--r--   0        0        0     5498 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/NLCC_POTENTIALS
+-rw-r--r--   0        0        0   177804 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/POTENTIAL
+-rw-r--r--   0        0        0   385325 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/POTENTIAL_UZH
+-rw-r--r--   0        0        0      125 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/README.md
+-rw-r--r--   0        0        0    91811 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/nm12_parameters.xml
+-rw-r--r--   0        0        0    32194 2024-04-02 03:42:50.640085 dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/xTB_parameters
+-rw-r--r--   0        0        0     1171 2024-04-09 15:45:01.385722 dflow_galaxy-0.1.5.post2/dflow_galaxy/res/dynacat/tesla_template.yml
+-rw-r--r--   0        0        0        0 2024-02-07 08:30:41.445577 dflow_galaxy-0.1.5.post2/dflow_galaxy/workflow/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-07 08:30:41.445577 dflow_galaxy-0.1.5.post2/dflow_galaxy/workflow/tesla/__init__.py
+-rw-r--r--   0        0        0     1702 2024-04-09 15:45:01.385722 dflow_galaxy-0.1.5.post2/dflow_galaxy/workflow/tesla/config.py
+-rw-r--r--   0        0        0        0 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.5.post2/dflow_galaxy/workflow/tesla/domain/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.5.post2/dflow_galaxy/workflow/tesla/domain/abacus.py
+-rw-r--r--   0        0        0     6298 2024-04-02 03:42:50.640085 dflow_galaxy-0.1.5.post2/dflow_galaxy/workflow/tesla/domain/cp2k.py
+-rw-r--r--   0        0        0     9775 2024-04-09 14:05:23.796450 dflow_galaxy-0.1.5.post2/dflow_galaxy/workflow/tesla/domain/deepmd.py
+-rw-r--r--   0        0        0     8016 2024-04-02 03:42:50.640085 dflow_galaxy-0.1.5.post2/dflow_galaxy/workflow/tesla/domain/lammps.py
+-rw-r--r--   0        0        0     1261 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.5.post2/dflow_galaxy/workflow/tesla/domain/lib.py
+-rw-r--r--   0        0        0     6334 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.5.post2/dflow_galaxy/workflow/tesla/domain/model_devi.py
+-rw-r--r--   0        0        0     8185 2024-04-09 15:45:01.385722 dflow_galaxy-0.1.5.post2/dflow_galaxy/workflow/tesla/main.py
+-rw-r--r--   0        0        0      547 2024-04-10 02:22:55.284072 dflow_galaxy-0.1.5.post2/pyproject.toml
+-rw-r--r--   0        0        0     2485 1970-01-01 00:00:00.000000 dflow_galaxy-0.1.5.post2/PKG-INFO
```

### Comparing `dflow_galaxy-0.1.5.post1/LICENSE` & `dflow_galaxy-0.1.5.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post1/README.md` & `dflow_galaxy-0.1.5.post2/README.md`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post1/dflow_galaxy/app/common.py` & `dflow_galaxy-0.1.5.post2/dflow_galaxy/app/common.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post1/dflow_galaxy/app/cp2k_lightning/dflow.py` & `dflow_galaxy-0.1.5.post2/dflow_galaxy/app/cp2k_lightning/dflow.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post1/dflow_galaxy/app/cp2k_lightning/main.py` & `dflow_galaxy-0.1.5.post2/dflow_galaxy/app/cp2k_lightning/main.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post1/dflow_galaxy/app/dynacat_md/dflow.py` & `dflow_galaxy-0.1.5.post2/dflow_galaxy/app/dynacat_md/dflow.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post1/dflow_galaxy/app/dynacat_md/main.py` & `dflow_galaxy-0.1.5.post2/dflow_galaxy/app/dynacat_md/main.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post1/dflow_galaxy/app/dynacat_tesla/main.py` & `dflow_galaxy-0.1.5.post2/dflow_galaxy/app/dynacat_tesla/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -329,25 +329,26 @@
         },
     }
 
 
 def _get_workflow_config(args: DynacatTeslaArgs, dp_dataset_config: dict):
     # process system file
     explore_data_file = args.lammps.system_file.get_full_path()
+    explore_data_key = os.path.basename(explore_data_file)
     atoms = ase.io.read(explore_data_file, index=0)
     type_map, mass_map = ai2cat.get_type_map(atoms)  # type: ignore
 
     cp2k_input_template = load_text(args.cp2k.input_template.get_full_path())
     deepmd_template = load_json(args.deepmd.input_template.get_full_path())
     product_vars, broadcast_vars = _get_lammps_vars(args.lammps.explore_vars)
 
     return {
         'datasets': {
             **dp_dataset_config,
-            'explore-data': {
+            explore_data_key: {  # data key must be a normal file name or else ase cannot detect the format
                 'url': explore_data_file,
             },
         },
         'workflow': {
             'general': {
                 'type_map': type_map,
                 'mass_map': mass_map,
@@ -357,15 +358,15 @@
                     'init_dataset': list(dp_dataset_config.keys()),
                     'input_template': deepmd_template,
                     'compress_model': args.deepmd.compress_model,
                 }
             },
             'explore':{
                 'lammps': {
-                    'systems': ['explore-data'],
+                    'systems': [explore_data_key],
                     'nsteps': args.lammps.nsteps,
                     'ensemble': args.lammps.ensemble.value,
                     'timestep': args.lammps.timestep,
                     'sample_freq': args.lammps.sample_freq,
                     'no_pbc': args.lammps.no_pbc,
                     'plumed_config': args.lammps.plumed_config or None,
                     'product_vars': product_vars,
```

### Comparing `dflow_galaxy-0.1.5.post1/dflow_galaxy/core/dflow.py` & `dflow_galaxy-0.1.5.post2/dflow_galaxy/core/dflow.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post1/dflow_galaxy/core/dispatcher.py` & `dflow_galaxy-0.1.5.post2/dflow_galaxy/core/dispatcher.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post1/dflow_galaxy/core/types.py` & `dflow_galaxy-0.1.5.post2/dflow_galaxy/core/types.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post1/dflow_galaxy/core/util.py` & `dflow_galaxy-0.1.5.post2/dflow_galaxy/core/util.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/ALL_BASIS_SETS` & `dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/ALL_BASIS_SETS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/ALL_POTENTIALS` & `dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/ALL_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/AcPP1_POTENTIALS` & `dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/AcPP1_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_ADMM` & `dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/BASIS_ADMM`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_ADMM_MOLOPT` & `dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/BASIS_ADMM_MOLOPT`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_ADMM_UZH` & `dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/BASIS_ADMM_UZH`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_ADMM_ae` & `dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/BASIS_ADMM_ae`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_LRIGPW_AUXMOLOPT` & `dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/BASIS_LRIGPW_AUXMOLOPT`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_MINBAS` & `dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/BASIS_MINBAS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_MINIX` & `dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/BASIS_MINIX`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT` & `dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_AcPP1` & `dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_AcPP1`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_LnPP1` & `dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_LnPP1`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_LnPP2` & `dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_LnPP2`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_UCL` & `dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_UCL`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_UZH` & `dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_UZH`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_PERIODIC_GW` & `dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/BASIS_PERIODIC_GW`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_RI_cc-TZ` & `dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/BASIS_RI_cc-TZ`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_SET` & `dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/BASIS_SET`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_ZIJLSTRA` & `dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/BASIS_ZIJLSTRA`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_ccGRB_UZH` & `dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/BASIS_ccGRB_UZH`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_def2_QZVP_RI_ALL` & `dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/BASIS_def2_QZVP_RI_ALL`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/BASIS_pob` & `dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/BASIS_pob`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/ECP_POTENTIALS` & `dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/ECP_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/ECP_POTENTIALS_pob-TZVP-rev2` & `dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/ECP_POTENTIALS_pob-TZVP-rev2`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/EMSL_BASIS_SETS` & `dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/EMSL_BASIS_SETS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/GTH_BASIS_SETS` & `dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/GTH_BASIS_SETS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/GTH_POTENTIALS` & `dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/GTH_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/GTH_SOC_POTENTIALS` & `dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/GTH_SOC_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/HFX_BASIS` & `dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/HFX_BASIS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/HF_POTENTIALS` & `dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/HF_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/LnPP1_POTENTIALS` & `dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/LnPP1_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/LnPP2_POTENTIALS` & `dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/LnPP2_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/NLCC_POTENTIALS` & `dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/NLCC_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/POTENTIAL` & `dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/POTENTIAL`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/POTENTIAL_UZH` & `dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/POTENTIAL_UZH`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/nm12_parameters.xml` & `dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/nm12_parameters.xml`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/cp2k_data/xTB_parameters` & `dflow_galaxy-0.1.5.post2/dflow_galaxy/res/cp2k_data/xTB_parameters`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post1/dflow_galaxy/res/dynacat/tesla_template.yml` & `dflow_galaxy-0.1.5.post2/dflow_galaxy/res/dynacat/tesla_template.yml`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post1/dflow_galaxy/workflow/tesla/config.py` & `dflow_galaxy-0.1.5.post2/dflow_galaxy/workflow/tesla/config.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post1/dflow_galaxy/workflow/tesla/domain/cp2k.py` & `dflow_galaxy-0.1.5.post2/dflow_galaxy/workflow/tesla/domain/cp2k.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post1/dflow_galaxy/workflow/tesla/domain/deepmd.py` & `dflow_galaxy-0.1.5.post2/dflow_galaxy/workflow/tesla/domain/deepmd.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post1/dflow_galaxy/workflow/tesla/domain/lammps.py` & `dflow_galaxy-0.1.5.post2/dflow_galaxy/workflow/tesla/domain/lammps.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post1/dflow_galaxy/workflow/tesla/domain/lib.py` & `dflow_galaxy-0.1.5.post2/dflow_galaxy/workflow/tesla/domain/lib.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post1/dflow_galaxy/workflow/tesla/domain/model_devi.py` & `dflow_galaxy-0.1.5.post2/dflow_galaxy/workflow/tesla/domain/model_devi.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post1/dflow_galaxy/workflow/tesla/main.py` & `dflow_galaxy-0.1.5.post2/dflow_galaxy/workflow/tesla/main.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post1/pyproject.toml` & `dflow_galaxy-0.1.5.post2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dflow-galaxy"
-version = "0.1.5.post1"
+version = "0.1.5.post2"
 description = ""
 authors = ["weihong.xu <xuweihong.cn@gmail.com>"]
 readme = "README.md"
 include = ["dflow_galaxy/res/*"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `dflow_galaxy-0.1.5.post1/PKG-INFO` & `dflow_galaxy-0.1.5.post2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dflow-galaxy
-Version: 0.1.5.post1
+Version: 0.1.5.post2
 Summary: 
 Author: weihong.xu
 Author-email: xuweihong.cn@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

