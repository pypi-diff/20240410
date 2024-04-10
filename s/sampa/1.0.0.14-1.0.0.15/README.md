# Comparing `tmp/sampa-1.0.0.14.tar.gz` & `tmp/sampa-1.0.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sampa-1.0.0.14.tar", last modified: Wed Apr 10 12:48:44 2024, max compression
+gzip compressed data, was "sampa-1.0.0.15.tar", last modified: Wed Apr 10 16:43:46 2024, max compression
```

## Comparing `sampa-1.0.0.14.tar` & `sampa-1.0.0.15.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 12:48:44.026332 sampa-1.0.0.14/
--rw-rw-rw-   0        0        0       13 2024-04-09 02:21:11.000000 sampa-1.0.0.14/LICENSE.txt
--rw-rw-rw-   0        0        0      288 2024-04-10 12:48:44.026332 sampa-1.0.0.14/PKG-INFO
--rw-rw-rw-   0        0        0       51 2024-04-09 02:20:56.000000 sampa-1.0.0.14/README.md
-drwxrwxrwx   0        0        0        0 2024-04-10 12:48:43.932617 sampa-1.0.0.14/sampa/
--rw-rw-rw-   0        0        0       52 2024-04-09 02:21:40.000000 sampa-1.0.0.14/sampa/__init__.py
--rw-rw-rw-   0        0        0     7897 2024-04-10 12:48:33.000000 sampa-1.0.0.14/sampa/__main__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:48:43.995080 sampa-1.0.0.14/sampa/src/
--rw-rw-rw-   0        0        0    67538 2024-04-09 14:15:03.000000 sampa-1.0.0.14/sampa/src/HeteroStructure_Generator-Augusto_Dlelis.py
--rw-rw-rw-   0        0        0    71626 2024-04-09 02:22:18.000000 sampa-1.0.0.14/sampa/src/HeteroStructure_Generator.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:48:44.010704 sampa-1.0.0.14/sampa/src/INPUTS/
--rw-rw-rw-   0        0        0      228 2024-04-05 14:40:05.000000 sampa-1.0.0.14/sampa/src/INPUTS/INCAR_bader
--rw-rw-rw-   0        0        0      269 2024-04-05 14:40:00.000000 sampa-1.0.0.14/sampa/src/INPUTS/INCAR_bader.SO
--rw-rw-rw-   0        0        0      223 2024-03-27 17:25:45.000000 sampa-1.0.0.14/sampa/src/INPUTS/INCAR_bands
--rw-rw-rw-   0        0        0      264 2024-03-24 14:34:17.000000 sampa-1.0.0.14/sampa/src/INPUTS/INCAR_bands.SO
--rw-rw-rw-   0        0        0      212 2024-04-04 18:32:53.000000 sampa-1.0.0.14/sampa/src/INPUTS/INCAR_dos
--rw-rw-rw-   0        0        0      253 2024-04-04 18:33:02.000000 sampa-1.0.0.14/sampa/src/INPUTS/INCAR_dos.SO
--rw-rw-rw-   0        0        0      201 2024-04-04 18:33:10.000000 sampa-1.0.0.14/sampa/src/INPUTS/INCAR_relax
--rw-rw-rw-   0        0        0      214 2024-04-04 18:33:17.000000 sampa-1.0.0.14/sampa/src/INPUTS/INCAR_scf
--rw-rw-rw-   0        0        0      255 2024-04-04 18:33:33.000000 sampa-1.0.0.14/sampa/src/INPUTS/INCAR_scf.SO
-drwxrwxrwx   0        0        0        0 2024-04-10 12:48:44.026332 sampa-1.0.0.14/sampa/src/INPUTS/inputs_VASProcar/
--rw-rw-rw-   0        0        0     4485 2024-03-20 16:04:46.000000 sampa-1.0.0.14/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.bands
--rw-rw-rw-   0        0        0     3123 2024-04-08 15:25:48.000000 sampa-1.0.0.14/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.chgcar
--rw-rw-rw-   0        0        0     2525 2024-03-20 16:04:58.000000 sampa-1.0.0.14/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.dos
--rw-rw-rw-   0        0        0     9603 2024-03-21 16:46:57.000000 sampa-1.0.0.14/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.location
--rw-rw-rw-   0        0        0     1187 2024-03-23 20:35:59.000000 sampa-1.0.0.14/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.locpot
--rw-rw-rw-   0        0        0     6378 2024-03-20 16:05:20.000000 sampa-1.0.0.14/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.orbitals
--rw-rw-rw-   0        0        0     7790 2024-03-20 16:06:00.000000 sampa-1.0.0.14/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.spin
--rw-rw-rw-   0        0        0     3968 2024-04-10 01:37:39.000000 sampa-1.0.0.14/sampa/src/SAMBA_HeteroStructure.input
--rw-rw-rw-   0        0        0     1610 2024-04-10 01:37:55.000000 sampa-1.0.0.14/sampa/src/SAMBA_WorkFlow.input
--rw-rw-rw-   0        0        0     1089 2024-04-10 12:48:10.000000 sampa-1.0.0.14/sampa/src/_info_pseudo.py
--rw-rw-rw-   0        0        0  4715152 2023-08-19 14:41:30.000000 sampa-1.0.0.14/sampa/src/bader
--rw-rw-rw-   0        0        0     4517 2024-04-09 02:22:42.000000 sampa-1.0.0.14/sampa/src/bader_poscar.py
--rw-rw-rw-   0        0        0     2522 2024-04-09 02:22:36.000000 sampa-1.0.0.14/sampa/src/bader_update.py
--rw-rw-rw-   0        0        0     7055 2024-04-09 02:22:30.000000 sampa-1.0.0.14/sampa/src/charge_transfer.py
--rw-rw-rw-   0        0        0     2139 2019-12-02 15:59:08.000000 sampa-1.0.0.14/sampa/src/chgsum.pl
--rw-rw-rw-   0        0        0      325 2024-04-09 02:22:24.000000 sampa-1.0.0.14/sampa/src/contcar_update.py
--rw-rw-rw-   0        0        0     9936 2024-04-09 12:38:41.000000 sampa-1.0.0.14/sampa/src/job.py
--rw-rw-rw-   0        0        0     6676 2024-04-09 12:37:10.000000 sampa-1.0.0.14/sampa/src/kpoints.py
--rw-rw-rw-   0        0        0    17429 2024-04-10 01:32:58.000000 sampa-1.0.0.14/sampa/src/make_files.py
--rw-rw-rw-   0        0        0     4024 2024-04-09 02:21:55.000000 sampa-1.0.0.14/sampa/src/output.py
--rw-rw-rw-   0        0        0     1048 2024-04-10 01:31:22.000000 sampa-1.0.0.14/sampa/src/potcar.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:48:43.948227 sampa-1.0.0.14/sampa.egg-info/
--rw-rw-rw-   0        0        0      288 2024-04-10 12:48:43.000000 sampa-1.0.0.14/sampa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1349 2024-04-10 12:48:43.000000 sampa-1.0.0.14/sampa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 12:48:43.000000 sampa-1.0.0.14/sampa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-04-10 12:48:43.000000 sampa-1.0.0.14/sampa.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       34 2024-04-10 12:48:43.000000 sampa-1.0.0.14/sampa.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-10 12:48:43.000000 sampa-1.0.0.14/sampa.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      167 2024-04-10 12:48:44.026332 sampa-1.0.0.14/setup.cfg
--rw-rw-rw-   0        0        0      719 2024-04-10 12:48:26.000000 sampa-1.0.0.14/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 16:43:46.971992 sampa-1.0.0.15/
+-rw-rw-rw-   0        0        0       13 2024-04-09 02:21:11.000000 sampa-1.0.0.15/LICENSE.txt
+-rw-rw-rw-   0        0        0      288 2024-04-10 16:43:46.971992 sampa-1.0.0.15/PKG-INFO
+-rw-rw-rw-   0        0        0       51 2024-04-09 02:20:56.000000 sampa-1.0.0.15/README.md
+drwxrwxrwx   0        0        0        0 2024-04-10 16:43:46.643857 sampa-1.0.0.15/sampa/
+-rw-rw-rw-   0        0        0       52 2024-04-09 02:21:40.000000 sampa-1.0.0.15/sampa/__init__.py
+-rw-rw-rw-   0        0        0     7897 2024-04-10 16:42:59.000000 sampa-1.0.0.15/sampa/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 16:43:46.846985 sampa-1.0.0.15/sampa/src/
+-rw-rw-rw-   0        0        0    67538 2024-04-09 14:15:03.000000 sampa-1.0.0.15/sampa/src/HeteroStructure_Generator-Augusto_Dlelis.py
+-rw-rw-rw-   0        0        0    71626 2024-04-09 02:22:18.000000 sampa-1.0.0.15/sampa/src/HeteroStructure_Generator.py
+drwxrwxrwx   0        0        0        0 2024-04-10 16:43:46.909481 sampa-1.0.0.15/sampa/src/INPUTS/
+-rw-rw-rw-   0        0        0      228 2024-04-05 14:40:05.000000 sampa-1.0.0.15/sampa/src/INPUTS/INCAR_bader
+-rw-rw-rw-   0        0        0      269 2024-04-05 14:40:00.000000 sampa-1.0.0.15/sampa/src/INPUTS/INCAR_bader.SO
+-rw-rw-rw-   0        0        0      223 2024-03-27 17:25:45.000000 sampa-1.0.0.15/sampa/src/INPUTS/INCAR_bands
+-rw-rw-rw-   0        0        0      264 2024-03-24 14:34:17.000000 sampa-1.0.0.15/sampa/src/INPUTS/INCAR_bands.SO
+-rw-rw-rw-   0        0        0      212 2024-04-04 18:32:53.000000 sampa-1.0.0.15/sampa/src/INPUTS/INCAR_dos
+-rw-rw-rw-   0        0        0      253 2024-04-04 18:33:02.000000 sampa-1.0.0.15/sampa/src/INPUTS/INCAR_dos.SO
+-rw-rw-rw-   0        0        0      201 2024-04-04 18:33:10.000000 sampa-1.0.0.15/sampa/src/INPUTS/INCAR_relax
+-rw-rw-rw-   0        0        0      214 2024-04-04 18:33:17.000000 sampa-1.0.0.15/sampa/src/INPUTS/INCAR_scf
+-rw-rw-rw-   0        0        0      255 2024-04-04 18:33:33.000000 sampa-1.0.0.15/sampa/src/INPUTS/INCAR_scf.SO
+drwxrwxrwx   0        0        0        0 2024-04-10 16:43:46.971992 sampa-1.0.0.15/sampa/src/INPUTS/inputs_VASProcar/
+-rw-rw-rw-   0        0        0     4485 2024-03-20 16:04:46.000000 sampa-1.0.0.15/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.bands
+-rw-rw-rw-   0        0        0     3123 2024-04-08 15:25:48.000000 sampa-1.0.0.15/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.chgcar
+-rw-rw-rw-   0        0        0     2525 2024-03-20 16:04:58.000000 sampa-1.0.0.15/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.dos
+-rw-rw-rw-   0        0        0     9603 2024-03-21 16:46:57.000000 sampa-1.0.0.15/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.location
+-rw-rw-rw-   0        0        0     1187 2024-03-23 20:35:59.000000 sampa-1.0.0.15/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.locpot
+-rw-rw-rw-   0        0        0     6378 2024-03-20 16:05:20.000000 sampa-1.0.0.15/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.orbitals
+-rw-rw-rw-   0        0        0     7790 2024-03-20 16:06:00.000000 sampa-1.0.0.15/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.spin
+-rw-rw-rw-   0        0        0     3968 2024-04-10 01:37:39.000000 sampa-1.0.0.15/sampa/src/SAMBA_HeteroStructure.input
+-rw-rw-rw-   0        0        0     1589 2024-04-10 16:42:36.000000 sampa-1.0.0.15/sampa/src/SAMBA_WorkFlow.input
+-rw-rw-rw-   0        0        0     1089 2024-04-10 12:48:10.000000 sampa-1.0.0.15/sampa/src/_info_pseudo.py
+-rw-rw-rw-   0        0        0  4715152 2023-08-19 14:41:30.000000 sampa-1.0.0.15/sampa/src/bader
+-rw-rw-rw-   0        0        0     4517 2024-04-09 02:22:42.000000 sampa-1.0.0.15/sampa/src/bader_poscar.py
+-rw-rw-rw-   0        0        0     2522 2024-04-09 02:22:36.000000 sampa-1.0.0.15/sampa/src/bader_update.py
+-rw-rw-rw-   0        0        0     7055 2024-04-09 02:22:30.000000 sampa-1.0.0.15/sampa/src/charge_transfer.py
+-rw-rw-rw-   0        0        0     2139 2019-12-02 15:59:08.000000 sampa-1.0.0.15/sampa/src/chgsum.pl
+-rw-rw-rw-   0        0        0      325 2024-04-09 02:22:24.000000 sampa-1.0.0.15/sampa/src/contcar_update.py
+-rw-rw-rw-   0        0        0     9936 2024-04-09 12:38:41.000000 sampa-1.0.0.15/sampa/src/job.py
+-rw-rw-rw-   0        0        0     6676 2024-04-09 12:37:10.000000 sampa-1.0.0.15/sampa/src/kpoints.py
+-rw-rw-rw-   0        0        0    17429 2024-04-10 01:32:58.000000 sampa-1.0.0.15/sampa/src/make_files.py
+-rw-rw-rw-   0        0        0     4024 2024-04-09 02:21:55.000000 sampa-1.0.0.15/sampa/src/output.py
+-rw-rw-rw-   0        0        0     1048 2024-04-10 01:31:22.000000 sampa-1.0.0.15/sampa/src/potcar.py
+drwxrwxrwx   0        0        0        0 2024-04-10 16:43:46.675108 sampa-1.0.0.15/sampa.egg-info/
+-rw-rw-rw-   0        0        0      288 2024-04-10 16:43:46.000000 sampa-1.0.0.15/sampa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1349 2024-04-10 16:43:46.000000 sampa-1.0.0.15/sampa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 16:43:46.000000 sampa-1.0.0.15/sampa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-04-10 16:43:46.000000 sampa-1.0.0.15/sampa.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       34 2024-04-10 16:43:46.000000 sampa-1.0.0.15/sampa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-10 16:43:46.000000 sampa-1.0.0.15/sampa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      167 2024-04-10 16:43:46.971992 sampa-1.0.0.15/setup.cfg
+-rw-rw-rw-   0        0        0      719 2024-04-10 16:42:49.000000 sampa-1.0.0.15/setup.py
```

### Comparing `sampa-1.0.0.14/sampa/__main__.py` & `sampa-1.0.0.15/sampa/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import subprocess
 import pyfiglet
 import shutil
 import time
 import os
 
 
-version = '1.0.0.14'
+version = '1.0.0.15'
 
 
 print(" ")
 print("=============================================================")
 print(f'SAMBA v{version} Copyright (C) 2024 ---------------------------')
 print("Closed source: Adalberto Fazzio's research group (Ilum|CNPEM)")
 print("Author: Augusto de Lelis Araujo -----------------------------")
```

### Comparing `sampa-1.0.0.14/sampa/src/HeteroStructure_Generator-Augusto_Dlelis.py` & `sampa-1.0.0.15/sampa/src/HeteroStructure_Generator-Augusto_Dlelis.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.14/sampa/src/HeteroStructure_Generator.py` & `sampa-1.0.0.15/sampa/src/HeteroStructure_Generator.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.14/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.bands` & `sampa-1.0.0.15/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.bands`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.14/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.chgcar` & `sampa-1.0.0.15/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.chgcar`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.14/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.dos` & `sampa-1.0.0.15/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.dos`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.14/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.location` & `sampa-1.0.0.15/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.location`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.14/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.locpot` & `sampa-1.0.0.15/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.locpot`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.14/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.orbitals` & `sampa-1.0.0.15/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.orbitals`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.14/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.spin` & `sampa-1.0.0.15/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.spin`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.14/sampa/src/SAMBA_HeteroStructure.input` & `sampa-1.0.0.15/sampa/src/SAMBA_HeteroStructure.input`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.14/sampa/src/SAMBA_WorkFlow.input` & `sampa-1.0.0.15/sampa/src/SAMBA_WorkFlow.input`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SAMBA Copyright (C) 2024 - Closed source
 
-#================================================
-tasks = ['relax', 'scf', 'bands', 'dos', 'bader']          # As tarefas são executadas em sequência, logo: 'relax' e 'scf' devem estar na 1º e 2º posições, respectivamentety.
-type  = ['sem_SO','com_SO']                                # Define se as tarefas serão realizadas sem e/ou com SO. 'relax' sempre é executados sem SO.
+#=======================================
+tasks = ['relax', 'scf', 'bands', 'dos']             # As tarefas são executadas em sequência, logo: 'relax' e 'scf' devem estar na 1º e 2º posições, respectivamentety.
+type  = ['sem_SO','com_SO']                          # Define se as tarefas serão realizadas sem e/ou com SO. 'relax' sempre é executados sem SO.
 # tasks = ['relax', 'scf', 'bands', 'dos', 'bader']
 # type  = ['sem_SO','com_SO']    
 #============================
 type_k_dens  = 1            # [1] KPOINTS (Monkhorst-Pack);  [2]  KPOINTS (Gamma);  [3] INCAR (KSPACING Monkhorst-Pack);  [4] INCAR (KSPACING Gamma)
 k_dens_relax = 12           # Cálculo de relaxação:            nº de pontos-k por Angs^-1
 k_dens_scf   = 12           # Cálculo auto-consistente (scf):  nº de pontos-k por Angs^-1
 k_dens_dos   = 12           # Cálculo da DOS:                  nº de pontos-k por Angs^-1
```

### Comparing `sampa-1.0.0.14/sampa/src/_info_pseudo.py` & `sampa-1.0.0.15/sampa/src/_info_pseudo.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.14/sampa/src/bader` & `sampa-1.0.0.15/sampa/src/bader`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.14/sampa/src/bader_poscar.py` & `sampa-1.0.0.15/sampa/src/bader_poscar.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.14/sampa/src/bader_update.py` & `sampa-1.0.0.15/sampa/src/bader_update.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.14/sampa/src/charge_transfer.py` & `sampa-1.0.0.15/sampa/src/charge_transfer.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.14/sampa/src/chgsum.pl` & `sampa-1.0.0.15/sampa/src/chgsum.pl`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.14/sampa/src/job.py` & `sampa-1.0.0.15/sampa/src/job.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.14/sampa/src/kpoints.py` & `sampa-1.0.0.15/sampa/src/kpoints.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.14/sampa/src/make_files.py` & `sampa-1.0.0.15/sampa/src/make_files.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.14/sampa/src/output.py` & `sampa-1.0.0.15/sampa/src/output.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.14/sampa/src/potcar.py` & `sampa-1.0.0.15/sampa/src/potcar.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.14/sampa.egg-info/SOURCES.txt` & `sampa-1.0.0.15/sampa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.14/setup.py` & `sampa-1.0.0.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 import json
 from pathlib import Path
 from typing import Optional
 
 setup(
     name = "sampa",
-    version = "1.0.0.14",
+    version = "1.0.0.15",
     entry_points={'console_scripts': ['sampa = sampa:main']},
     description = "...",
     author = "Augusto de Lelis Araujo", 
     author_email = "augusto-lelis@outlook.com",
     license = "Closed source",
     install_requires=['numpy',
                       'requests',
```

