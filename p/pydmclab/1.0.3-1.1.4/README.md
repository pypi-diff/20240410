# Comparing `tmp/pydmclab-1.0.3.tar.gz` & `tmp/pydmclab-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydmclab-1.0.3.tar", last modified: Sat Sep 16 18:49:00 2023, max compression
+gzip compressed data, was "pydmclab-1.1.4.tar", last modified: Tue Apr  9 21:46:12 2024, max compression
```

## Comparing `pydmclab-1.0.3.tar` & `pydmclab-1.1.4.tar`

### file list

```diff
@@ -1,90 +1,102 @@
-drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2023-09-16 18:49:00.984056 pydmclab-1.0.3/
--rw-------   0 cbartel    (503) staff       (20)     1071 2023-04-03 21:26:17.000000 pydmclab-1.0.3/LICENSE.txt
--rw-------   0 cbartel    (503) staff       (20)      173 2023-04-03 21:38:56.000000 pydmclab-1.0.3/MANIFEST.in
--rw-r--r--   0 cbartel    (503) staff       (20)      686 2023-09-16 18:49:00.983551 pydmclab-1.0.3/PKG-INFO
--rw-------   0 cbartel    (503) staff       (20)      170 2023-04-05 14:50:32.000000 pydmclab-1.0.3/README.md
-drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2023-09-16 18:49:00.882992 pydmclab-1.0.3/pydmclab/
--rw-------   0 cbartel    (503) staff       (20)      282 2023-05-24 19:08:50.000000 pydmclab-1.0.3/pydmclab/__init__.py
-drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2023-09-16 18:49:00.917085 pydmclab-1.0.3/pydmclab/core/
--rw-------   0 cbartel    (503) staff       (20)      398 2023-04-03 21:26:17.000000 pydmclab-1.0.3/pydmclab/core/README.md
--rw-------   0 cbartel    (503) staff       (20)      176 2023-04-03 21:26:17.000000 pydmclab-1.0.3/pydmclab/core/__init__.py
--rw-------   0 cbartel    (503) staff       (20)     4582 2023-06-23 18:39:46.000000 pydmclab-1.0.3/pydmclab/core/comp.py
--rw-r--r--   0 cbartel    (503) staff       (20)    30379 2023-06-29 17:28:39.000000 pydmclab-1.0.3/pydmclab/core/energies.py
--rw-------   0 cbartel    (503) staff       (20)    52450 2023-07-06 18:38:40.000000 pydmclab-1.0.3/pydmclab/core/hulls.py
--rw-------   0 cbartel    (503) staff       (20)    12206 2023-06-23 20:18:22.000000 pydmclab-1.0.3/pydmclab/core/mag.py
--rw-------   0 cbartel    (503) staff       (20)    13935 2023-06-23 20:55:51.000000 pydmclab-1.0.3/pydmclab/core/query.py
--rw-r--r--   0 cbartel    (503) staff       (20)      470 2023-06-26 21:33:47.000000 pydmclab-1.0.3/pydmclab/core/reactions.py
--rw-r--r--   0 cbartel    (503) staff       (20)    18639 2023-09-11 19:12:09.000000 pydmclab-1.0.3/pydmclab/core/struc.py
-drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2023-09-16 18:49:00.927468 pydmclab-1.0.3/pydmclab/data/
--rw-r--r--   0 cbartel    (503) staff       (20)     6148 2023-04-03 21:26:17.000000 pydmclab-1.0.3/pydmclab/data/.DS_Store
--rw-------   0 cbartel    (503) staff       (20)      346 2023-04-03 21:26:17.000000 pydmclab-1.0.3/pydmclab/data/README.md
--rw-------   0 cbartel    (503) staff       (20)      331 2023-04-03 21:26:17.000000 pydmclab-1.0.3/pydmclab/data/__init__.py
--rw-------   0 cbartel    (503) staff       (20)      916 2023-04-03 21:26:17.000000 pydmclab-1.0.3/pydmclab/data/configs.py
-drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2023-09-16 18:49:00.949613 pydmclab-1.0.3/pydmclab/data/data/
--rw-r--r--   0 cbartel    (503) staff       (20)    15963 2023-04-03 21:26:17.000000 pydmclab-1.0.3/pydmclab/data/data/221220_dmc-mus.json
--rw-r--r--   0 cbartel    (503) staff       (20)     7720 2023-04-03 21:26:17.000000 pydmclab-1.0.3/pydmclab/data/data/230122_dmc-mus.json
--rw-------   0 cbartel    (503) staff       (20)     4723 2023-06-14 19:59:43.000000 pydmclab-1.0.3/pydmclab/data/data/230614_dmc-mus.json
--rw-r--r--   0 cbartel    (503) staff       (20)     1241 2023-04-17 14:02:36.000000 pydmclab-1.0.3/pydmclab/data/data/_batch_vasp_analysis_configs.yaml
--rw-------   0 cbartel    (503) staff       (20)      338 2023-06-30 21:45:22.000000 pydmclab-1.0.3/pydmclab/data/data/_launch_configs.yaml
--rw-------   0 cbartel    (503) staff       (20)     2069 2023-06-27 19:19:12.000000 pydmclab-1.0.3/pydmclab/data/data/_partition_configs.yaml
--rw-r--r--   0 cbartel    (503) staff       (20)      591 2023-06-28 13:54:53.000000 pydmclab-1.0.3/pydmclab/data/data/_slurm_configs.yaml
--rw-r--r--   0 cbartel    (503) staff       (20)     1795 2023-08-16 14:45:53.000000 pydmclab-1.0.3/pydmclab/data/data/_sub_configs.yaml
--rw-r--r--   0 cbartel    (503) staff       (20)     2124 2023-09-11 19:12:09.000000 pydmclab-1.0.3/pydmclab/data/data/_vasp_configs.yaml
--rw-------   0 cbartel    (503) staff       (20)     1570 2023-04-03 21:26:17.000000 pydmclab-1.0.3/pydmclab/data/data/atomic_masses.json
--rw-r--r--   0 cbartel    (503) staff       (20)     3140 2023-04-03 21:26:17.000000 pydmclab-1.0.3/pydmclab/data/data/bartel2019_npj_reference-energies.csv
--rw-r--r--   0 cbartel    (503) staff       (20)     2596 2023-04-03 21:26:17.000000 pydmclab-1.0.3/pydmclab/data/data/colors.json
--rw-------   0 cbartel    (503) staff       (20)    40326 2023-04-03 21:26:17.000000 pydmclab-1.0.3/pydmclab/data/data/elemental_gibbs_energies_T.json
--rw-r--r--   0 cbartel    (503) staff       (20)     1302 2023-05-31 16:34:05.000000 pydmclab-1.0.3/pydmclab/data/data/gas_thermo_data_nist.json
--rw-r--r--   0 cbartel    (503) staff       (20)      344 2023-08-25 19:02:07.000000 pydmclab-1.0.3/pydmclab/data/data/mp2020_compatibility_dmus.json
--rw-r--r--   0 cbartel    (503) staff       (20)     3788 2023-04-03 21:26:17.000000 pydmclab-1.0.3/pydmclab/data/data/mus_from_bartel2019_npj.json
--rw-r--r--   0 cbartel    (503) staff       (20)     4722 2023-06-14 19:59:59.000000 pydmclab-1.0.3/pydmclab/data/data/mus_from_dmc_no_corrections.json
--rw-------   0 cbartel    (503) staff       (20)     1710 2023-04-03 21:26:17.000000 pydmclab-1.0.3/pydmclab/data/data/mus_from_mp_no_corrections.json
--rw-------   0 cbartel    (503) staff       (20)    43287 2023-04-03 21:26:17.000000 pydmclab-1.0.3/pydmclab/data/data/ssub.dat
--rw-r--r--   0 cbartel    (503) staff       (20)    45994 2023-04-03 21:26:17.000000 pydmclab-1.0.3/pydmclab/data/data/ssub.json
--rw-------   0 cbartel    (503) staff       (20)      246 2023-04-03 21:26:17.000000 pydmclab-1.0.3/pydmclab/data/features.py
--rw-r--r--   0 cbartel    (503) staff       (20)     2252 2023-04-03 21:35:30.000000 pydmclab-1.0.3/pydmclab/data/plotting_configs.py
--rw-r--r--   0 cbartel    (503) staff       (20)     4186 2023-06-14 20:00:50.000000 pydmclab-1.0.3/pydmclab/data/thermochem.py
-drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2023-09-16 18:49:00.959609 pydmclab-1.0.3/pydmclab/demos/
--rw-------   0 cbartel    (503) staff       (20)     3762 2023-06-23 16:29:29.000000 pydmclab-1.0.3/pydmclab/demos/demo_comp.py
--rw-------   0 cbartel    (503) staff       (20)     7980 2023-06-29 18:58:01.000000 pydmclab-1.0.3/pydmclab/demos/demo_energies.py
--rw-------   0 cbartel    (503) staff       (20)    14056 2023-07-05 21:53:26.000000 pydmclab-1.0.3/pydmclab/demos/demo_hulls.py
--rw-r--r--   0 cbartel    (503) staff       (20)    10468 2023-08-16 15:08:44.000000 pydmclab-1.0.3/pydmclab/demos/demo_launcher_template.py
--rw-------   0 cbartel    (503) staff       (20)      685 2023-06-23 20:18:25.000000 pydmclab-1.0.3/pydmclab/demos/demo_mag.py
--rw-r--r--   0 cbartel    (503) staff       (20)     1665 2023-06-20 18:30:53.000000 pydmclab-1.0.3/pydmclab/demos/demo_plot_dos.py
--rw-------   0 cbartel    (503) staff       (20)     3167 2023-06-23 20:33:44.000000 pydmclab-1.0.3/pydmclab/demos/demo_query.py
--rw-------   0 cbartel    (503) staff       (20)     3848 2023-06-23 18:34:28.000000 pydmclab-1.0.3/pydmclab/demos/demo_struc.py
-drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2023-09-16 18:49:00.968893 pydmclab-1.0.3/pydmclab/dev/
--rw-r--r--   0 cbartel    (503) staff       (20)      153 2023-04-19 19:26:44.000000 pydmclab-1.0.3/pydmclab/dev/Untitled-2.py
--rw-------   0 cbartel    (503) staff       (20)       48 2023-04-03 21:26:17.000000 pydmclab-1.0.3/pydmclab/dev/__init__.py
--rw-r--r--   0 cbartel    (503) staff       (20)     9447 2023-08-14 13:57:01.000000 pydmclab-1.0.3/pydmclab/dev/defects.py
--rw-r--r--   0 cbartel    (503) staff       (20)     7439 2023-07-06 14:04:57.000000 pydmclab-1.0.3/pydmclab/dev/echem.py
--rw-------   0 cbartel    (503) staff       (20)     3091 2023-06-26 21:35:16.000000 pydmclab-1.0.3/pydmclab/dev/entries.py
--rw-------   0 cbartel    (503) staff       (20)      170 2023-04-03 21:26:17.000000 pydmclab-1.0.3/pydmclab/dev/grand.py
--rw-r--r--   0 cbartel    (503) staff       (20)      966 2023-06-26 20:47:07.000000 pydmclab-1.0.3/pydmclab/dev/mixing_pmg.py
--rw-r--r--   0 cbartel    (503) staff       (20)     2483 2023-06-23 20:34:26.000000 pydmclab-1.0.3/pydmclab/dev/query_new_mp_api.py
-drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2023-09-16 18:49:00.976136 pydmclab-1.0.3/pydmclab/hpc/
--rw-------   0 cbartel    (503) staff       (20)      707 2023-04-03 21:26:17.000000 pydmclab-1.0.3/pydmclab/hpc/README.md
--rw-------   0 cbartel    (503) staff       (20)      156 2023-04-03 21:26:17.000000 pydmclab-1.0.3/pydmclab/hpc/__init__.py
--rw-r--r--   0 cbartel    (503) staff       (20)    46832 2023-05-31 17:45:11.000000 pydmclab-1.0.3/pydmclab/hpc/analyze.py
--rw-r--r--   0 cbartel    (503) staff       (20)    47484 2023-09-11 19:12:09.000000 pydmclab-1.0.3/pydmclab/hpc/helpers.py
--rw-r--r--   0 cbartel    (503) staff       (20)    13167 2023-08-14 22:01:38.000000 pydmclab-1.0.3/pydmclab/hpc/launch.py
--rw-r--r--   0 cbartel    (503) staff       (20)    47727 2023-08-29 21:45:52.000000 pydmclab-1.0.3/pydmclab/hpc/submit.py
--rw-r--r--   0 cbartel    (503) staff       (20)    25915 2023-09-11 19:12:09.000000 pydmclab-1.0.3/pydmclab/hpc/vasp.py
-drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2023-09-16 18:49:00.980164 pydmclab-1.0.3/pydmclab/plotting/
--rw-r--r--   0 cbartel    (503) staff       (20)        7 2023-06-20 19:00:10.000000 pydmclab-1.0.3/pydmclab/plotting/__init__.py
--rw-r--r--   0 cbartel    (503) staff       (20)      604 2023-08-16 15:08:24.000000 pydmclab-1.0.3/pydmclab/plotting/bs.py
--rw-r--r--   0 cbartel    (503) staff       (20)    13934 2023-06-23 15:24:04.000000 pydmclab-1.0.3/pydmclab/plotting/dos.py
--rw-r--r--   0 cbartel    (503) staff       (20)    21966 2023-06-23 15:24:04.000000 pydmclab-1.0.3/pydmclab/plotting/pd.py
--rw-r--r--   0 cbartel    (503) staff       (20)     2430 2023-06-20 18:56:12.000000 pydmclab-1.0.3/pydmclab/plotting/utils.py
-drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2023-09-16 18:49:00.982835 pydmclab-1.0.3/pydmclab/utils/
--rw-------   0 cbartel    (503) staff       (20)      271 2023-04-03 21:26:17.000000 pydmclab-1.0.3/pydmclab/utils/README.md
--rw-r--r--   0 cbartel    (503) staff       (20)      205 2023-05-29 20:02:40.000000 pydmclab-1.0.3/pydmclab/utils/__init__.py
--rw-r--r--   0 cbartel    (503) staff       (20)     3421 2023-05-29 19:36:18.000000 pydmclab-1.0.3/pydmclab/utils/handy.py
-drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2023-09-16 18:49:00.901863 pydmclab-1.0.3/pydmclab.egg-info/
--rw-r--r--   0 cbartel    (503) staff       (20)      686 2023-09-16 18:49:00.000000 pydmclab-1.0.3/pydmclab.egg-info/PKG-INFO
--rw-r--r--   0 cbartel    (503) staff       (20)     2291 2023-09-16 18:49:00.000000 pydmclab-1.0.3/pydmclab.egg-info/SOURCES.txt
--rw-r--r--   0 cbartel    (503) staff       (20)        1 2023-09-16 18:49:00.000000 pydmclab-1.0.3/pydmclab.egg-info/dependency_links.txt
--rw-r--r--   0 cbartel    (503) staff       (20)       48 2023-09-16 18:49:00.000000 pydmclab-1.0.3/pydmclab.egg-info/requires.txt
--rw-r--r--   0 cbartel    (503) staff       (20)        9 2023-09-16 18:49:00.000000 pydmclab-1.0.3/pydmclab.egg-info/top_level.txt
--rw-r--r--   0 cbartel    (503) staff       (20)       38 2023-09-16 18:49:00.984112 pydmclab-1.0.3/setup.cfg
--rw-r--r--   0 cbartel    (503) staff       (20)     2580 2023-09-16 18:48:02.000000 pydmclab-1.0.3/setup.py
+drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2024-04-09 21:46:12.308858 pydmclab-1.1.4/
+-rw-------   0 cbartel    (503) staff       (20)     1071 2023-04-03 21:26:17.000000 pydmclab-1.1.4/LICENSE.txt
+-rw-------   0 cbartel    (503) staff       (20)      173 2023-04-03 21:38:56.000000 pydmclab-1.1.4/MANIFEST.in
+-rw-r--r--   0 cbartel    (503) staff       (20)      710 2024-04-09 21:46:12.308564 pydmclab-1.1.4/PKG-INFO
+-rw-------   0 cbartel    (503) staff       (20)      170 2023-04-05 14:50:32.000000 pydmclab-1.1.4/README.md
+drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2024-04-09 21:46:12.256947 pydmclab-1.1.4/pydmclab/
+drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2024-04-09 21:46:12.271169 pydmclab-1.1.4/pydmclab/core/
+-rw-------   0 cbartel    (503) staff       (20)      398 2023-04-03 21:26:17.000000 pydmclab-1.1.4/pydmclab/core/README.md
+-rw-------   0 cbartel    (503) staff       (20)      756 2024-01-24 14:41:43.000000 pydmclab-1.1.4/pydmclab/core/__init__.py
+-rw-r--r--   0 cbartel    (503) staff       (20)    41254 2024-04-07 23:00:14.000000 pydmclab-1.1.4/pydmclab/core/alloys.py
+-rw-------   0 cbartel    (503) staff       (20)     4582 2024-01-23 23:40:20.000000 pydmclab-1.1.4/pydmclab/core/comp.py
+-rw-r--r--   0 cbartel    (503) staff       (20)     4122 2024-03-01 13:46:18.000000 pydmclab-1.1.4/pydmclab/core/defects.py
+-rw-r--r--   0 cbartel    (503) staff       (20)    35106 2024-03-20 14:29:25.000000 pydmclab-1.1.4/pydmclab/core/energies.py
+-rw-------   0 cbartel    (503) staff       (20)    52185 2024-01-24 14:24:40.000000 pydmclab-1.1.4/pydmclab/core/hulls.py
+-rw-r--r--   0 cbartel    (503) staff       (20)    13295 2024-03-01 13:46:18.000000 pydmclab-1.1.4/pydmclab/core/mag.py
+-rw-r--r--   0 cbartel    (503) staff       (20)    25440 2024-03-19 14:49:24.000000 pydmclab-1.1.4/pydmclab/core/query.py
+-rw-r--r--   0 cbartel    (503) staff       (20)    19256 2024-03-12 22:10:25.000000 pydmclab-1.1.4/pydmclab/core/struc.py
+drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2024-04-09 21:46:12.274107 pydmclab-1.1.4/pydmclab/data/
+-rw-r--r--   0 cbartel    (503) staff       (20)     6148 2023-04-03 21:26:17.000000 pydmclab-1.1.4/pydmclab/data/.DS_Store
+-rw-------   0 cbartel    (503) staff       (20)      346 2023-04-03 21:26:17.000000 pydmclab-1.1.4/pydmclab/data/README.md
+-rw-------   0 cbartel    (503) staff       (20)      331 2023-04-03 21:26:17.000000 pydmclab-1.1.4/pydmclab/data/__init__.py
+-rw-------   0 cbartel    (503) staff       (20)      916 2023-04-03 21:26:17.000000 pydmclab-1.1.4/pydmclab/data/configs.py
+drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2024-04-09 21:46:12.287256 pydmclab-1.1.4/pydmclab/data/data/
+-rw-r--r--   0 cbartel    (503) staff       (20)    15963 2023-04-03 21:26:17.000000 pydmclab-1.1.4/pydmclab/data/data/221220_dmc-mus.json
+-rw-r--r--   0 cbartel    (503) staff       (20)     7720 2023-04-03 21:26:17.000000 pydmclab-1.1.4/pydmclab/data/data/230122_dmc-mus.json
+-rw-------   0 cbartel    (503) staff       (20)     4723 2023-06-14 19:59:43.000000 pydmclab-1.1.4/pydmclab/data/data/230614_dmc-mus.json
+-rw-r--r--   0 cbartel    (503) staff       (20)    11941 2023-10-03 22:05:55.000000 pydmclab-1.1.4/pydmclab/data/data/231002_dmc-mus.json
+-rw-r--r--   0 cbartel    (503) staff       (20)     1386 2024-03-14 22:04:48.000000 pydmclab-1.1.4/pydmclab/data/data/_batch_vasp_analysis_configs.yaml
+-rw-------   0 cbartel    (503) staff       (20)      338 2023-06-30 21:45:22.000000 pydmclab-1.1.4/pydmclab/data/data/_launch_configs.yaml
+-rw-------   0 cbartel    (503) staff       (20)     2069 2023-06-27 19:19:12.000000 pydmclab-1.1.4/pydmclab/data/data/_partition_configs.yaml
+-rw-r--r--   0 cbartel    (503) staff       (20)      591 2023-06-28 13:54:53.000000 pydmclab-1.1.4/pydmclab/data/data/_slurm_configs.yaml
+-rw-r--r--   0 cbartel    (503) staff       (20)     1776 2024-03-13 13:55:27.000000 pydmclab-1.1.4/pydmclab/data/data/_sub_configs.yaml
+-rw-r--r--   0 cbartel    (503) staff       (20)     2471 2024-04-09 21:44:29.000000 pydmclab-1.1.4/pydmclab/data/data/_vasp_configs.yaml
+-rw-r--r--   0 cbartel    (503) staff       (20)     1246 2024-01-19 15:26:12.000000 pydmclab-1.1.4/pydmclab/data/data/atomic_electronegativities.json
+-rw-------   0 cbartel    (503) staff       (20)     1570 2023-04-03 21:26:17.000000 pydmclab-1.1.4/pydmclab/data/data/atomic_masses.json
+-rw-r--r--   0 cbartel    (503) staff       (20)     3140 2023-04-03 21:26:17.000000 pydmclab-1.1.4/pydmclab/data/data/bartel2019_npj_reference-energies.csv
+-rw-r--r--   0 cbartel    (503) staff       (20)     2596 2023-04-03 21:26:17.000000 pydmclab-1.1.4/pydmclab/data/data/colors.json
+-rw-------   0 cbartel    (503) staff       (20)    40326 2023-04-03 21:26:17.000000 pydmclab-1.1.4/pydmclab/data/data/elemental_gibbs_energies_T.json
+-rw-r--r--   0 cbartel    (503) staff       (20)     1302 2023-05-31 16:34:05.000000 pydmclab-1.1.4/pydmclab/data/data/gas_thermo_data_nist.json
+-rw-r--r--   0 cbartel    (503) staff       (20)      344 2023-08-25 19:02:07.000000 pydmclab-1.1.4/pydmclab/data/data/mp2020_compatibility_dmus.json
+-rw-r--r--   0 cbartel    (503) staff       (20)     3788 2023-04-03 21:26:17.000000 pydmclab-1.1.4/pydmclab/data/data/mus_from_bartel2019_npj.json
+-rw-r--r--   0 cbartel    (503) staff       (20)    11941 2023-10-03 22:05:55.000000 pydmclab-1.1.4/pydmclab/data/data/mus_from_dmc_no_corrections.json
+-rw-------   0 cbartel    (503) staff       (20)     1710 2023-04-03 21:26:17.000000 pydmclab-1.1.4/pydmclab/data/data/mus_from_mp_no_corrections.json
+-rw-r--r--   0 cbartel    (503) staff       (20)     8009 2024-01-19 15:26:23.000000 pydmclab-1.1.4/pydmclab/data/data/shannon_revised_effective_ionic_radii.json
+-rw-------   0 cbartel    (503) staff       (20)    43287 2023-04-03 21:26:17.000000 pydmclab-1.1.4/pydmclab/data/data/ssub.dat
+-rw-r--r--   0 cbartel    (503) staff       (20)    45994 2023-04-03 21:26:17.000000 pydmclab-1.1.4/pydmclab/data/data/ssub.json
+-rw-------   0 cbartel    (503) staff       (20)      545 2024-01-19 15:27:05.000000 pydmclab-1.1.4/pydmclab/data/features.py
+-rw-r--r--   0 cbartel    (503) staff       (20)     2252 2023-04-03 21:35:30.000000 pydmclab-1.1.4/pydmclab/data/plotting_configs.py
+-rw-r--r--   0 cbartel    (503) staff       (20)     4194 2023-10-02 13:25:16.000000 pydmclab-1.1.4/pydmclab/data/thermochem.py
+drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2024-04-09 21:46:12.293006 pydmclab-1.1.4/pydmclab/dev/
+-rw-r--r--   0 cbartel    (503) staff       (20)      153 2023-04-19 19:26:44.000000 pydmclab-1.1.4/pydmclab/dev/Untitled-2.py
+-rw-------   0 cbartel    (503) staff       (20)       48 2023-04-03 21:26:17.000000 pydmclab-1.1.4/pydmclab/dev/__init__.py
+-rw-r--r--   0 cbartel    (503) staff       (20)     9447 2023-08-14 13:57:01.000000 pydmclab-1.1.4/pydmclab/dev/defects.py
+-rw-r--r--   0 cbartel    (503) staff       (20)     7439 2023-07-06 14:04:57.000000 pydmclab-1.1.4/pydmclab/dev/echem.py
+-rw-------   0 cbartel    (503) staff       (20)     3091 2023-06-26 21:35:16.000000 pydmclab-1.1.4/pydmclab/dev/entries.py
+-rw-------   0 cbartel    (503) staff       (20)      170 2023-04-03 21:26:17.000000 pydmclab-1.1.4/pydmclab/dev/grand.py
+-rw-r--r--   0 cbartel    (503) staff       (20)      966 2023-06-26 20:47:07.000000 pydmclab-1.1.4/pydmclab/dev/mixing_pmg.py
+-rw-r--r--   0 cbartel    (503) staff       (20)      430 2024-03-21 18:41:19.000000 pydmclab-1.1.4/pydmclab/dev/phonons.py
+-rw-r--r--   0 cbartel    (503) staff       (20)     2483 2023-06-23 20:34:26.000000 pydmclab-1.1.4/pydmclab/dev/query_new_mp_api.py
+drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2024-04-09 21:46:12.297293 pydmclab-1.1.4/pydmclab/hpc/
+-rw-r--r--   0 cbartel    (503) staff       (20)     6148 2023-09-19 13:18:08.000000 pydmclab-1.1.4/pydmclab/hpc/.DS_Store
+-rw-------   0 cbartel    (503) staff       (20)      707 2023-04-03 21:26:17.000000 pydmclab-1.1.4/pydmclab/hpc/README.md
+-rw-------   0 cbartel    (503) staff       (20)      156 2023-04-03 21:26:17.000000 pydmclab-1.1.4/pydmclab/hpc/__init__.py
+-rw-r--r--   0 cbartel    (503) staff       (20)    49149 2024-03-14 22:06:20.000000 pydmclab-1.1.4/pydmclab/hpc/analyze.py
+-rw-r--r--   0 cbartel    (503) staff       (20)    59642 2024-04-02 17:14:37.000000 pydmclab-1.1.4/pydmclab/hpc/helpers.py
+-rw-r--r--   0 cbartel    (503) staff       (20)    13167 2023-08-14 22:01:38.000000 pydmclab-1.1.4/pydmclab/hpc/launch.py
+-rw-r--r--   0 cbartel    (503) staff       (20)    64691 2024-04-05 16:02:05.000000 pydmclab-1.1.4/pydmclab/hpc/submit.py
+-rw-r--r--   0 cbartel    (503) staff       (20)    26578 2024-04-09 21:44:35.000000 pydmclab-1.1.4/pydmclab/hpc/vasp.py
+drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2024-04-09 21:46:12.299014 pydmclab-1.1.4/pydmclab/mlp/
+-rw-r--r--   0 cbartel    (503) staff       (20)     2583 2023-10-18 17:33:08.000000 pydmclab-1.1.4/pydmclab/mlp/chgnet_md.py
+-rw-r--r--   0 cbartel    (503) staff       (20)     5192 2023-11-28 14:04:13.000000 pydmclab-1.1.4/pydmclab/mlp/md.py
+-rw-r--r--   0 cbartel    (503) staff       (20)    14702 2024-04-07 14:35:04.000000 pydmclab-1.1.4/pydmclab/mlp/phonons.py
+-rw-r--r--   0 cbartel    (503) staff       (20)     5107 2023-10-13 17:44:55.000000 pydmclab-1.1.4/pydmclab/mlp/relax.py
+drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2024-04-09 21:46:12.302122 pydmclab-1.1.4/pydmclab/plotting/
+-rw-r--r--   0 cbartel    (503) staff       (20)        7 2023-06-20 19:00:10.000000 pydmclab-1.1.4/pydmclab/plotting/__init__.py
+-rw-r--r--   0 cbartel    (503) staff       (20)      604 2023-08-16 15:08:24.000000 pydmclab-1.1.4/pydmclab/plotting/bs.py
+-rw-r--r--   0 cbartel    (503) staff       (20)    13934 2023-06-23 15:24:04.000000 pydmclab-1.1.4/pydmclab/plotting/dos.py
+-rw-r--r--   0 cbartel    (503) staff       (20)    21966 2023-06-23 15:24:04.000000 pydmclab-1.1.4/pydmclab/plotting/pd.py
+-rw-r--r--   0 cbartel    (503) staff       (20)     2430 2023-06-20 18:56:12.000000 pydmclab-1.1.4/pydmclab/plotting/utils.py
+drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2024-04-09 21:46:12.303668 pydmclab-1.1.4/pydmclab/utils/
+-rw-------   0 cbartel    (503) staff       (20)      271 2023-04-03 21:26:17.000000 pydmclab-1.1.4/pydmclab/utils/README.md
+-rw-r--r--   0 cbartel    (503) staff       (20)      205 2023-05-29 20:02:40.000000 pydmclab-1.1.4/pydmclab/utils/__init__.py
+-rw-r--r--   0 cbartel    (503) staff       (20)     3413 2024-03-15 20:17:27.000000 pydmclab-1.1.4/pydmclab/utils/handy.py
+drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2024-04-09 21:46:12.266977 pydmclab-1.1.4/pydmclab.egg-info/
+-rw-r--r--   0 cbartel    (503) staff       (20)      710 2024-04-09 21:46:12.000000 pydmclab-1.1.4/pydmclab.egg-info/PKG-INFO
+-rw-r--r--   0 cbartel    (503) staff       (20)     2538 2024-04-09 21:46:12.000000 pydmclab-1.1.4/pydmclab.egg-info/SOURCES.txt
+-rw-r--r--   0 cbartel    (503) staff       (20)        1 2024-04-09 21:46:12.000000 pydmclab-1.1.4/pydmclab.egg-info/dependency_links.txt
+-rw-r--r--   0 cbartel    (503) staff       (20)      116 2024-04-09 21:46:12.000000 pydmclab-1.1.4/pydmclab.egg-info/requires.txt
+-rw-r--r--   0 cbartel    (503) staff       (20)        9 2024-04-09 21:46:12.000000 pydmclab-1.1.4/pydmclab.egg-info/top_level.txt
+-rw-r--r--   0 cbartel    (503) staff       (20)       38 2024-04-09 21:46:12.308926 pydmclab-1.1.4/setup.cfg
+-rw-r--r--   0 cbartel    (503) staff       (20)     2788 2024-04-09 21:45:46.000000 pydmclab-1.1.4/setup.py
+drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2024-04-09 21:46:12.308079 pydmclab-1.1.4/tests/
+-rw-------   0 cbartel    (503) staff       (20)     1532 2023-05-25 17:38:50.000000 pydmclab-1.1.4/tests/test_comp.py
+-rw-r--r--   0 cbartel    (503) staff       (20)    10090 2024-01-24 19:04:51.000000 pydmclab-1.1.4/tests/test_energies.py
+-rw-r--r--   0 cbartel    (503) staff       (20)     7855 2023-08-24 19:14:39.000000 pydmclab-1.1.4/tests/test_helpers.py
+-rw-r--r--   0 cbartel    (503) staff       (20)     5706 2024-01-24 17:57:04.000000 pydmclab-1.1.4/tests/test_hulls.py
+-rw-r--r--   0 cbartel    (503) staff       (20)     2375 2023-08-14 16:31:47.000000 pydmclab-1.1.4/tests/test_launch.py
+-rw-r--r--   0 cbartel    (503) staff       (20)     2181 2023-05-26 20:53:47.000000 pydmclab-1.1.4/tests/test_mag.py
+-rw-r--r--   0 cbartel    (503) staff       (20)      969 2024-01-24 17:57:29.000000 pydmclab-1.1.4/tests/test_query.py
+-rw-r--r--   0 cbartel    (503) staff       (20)     3187 2023-06-23 15:54:04.000000 pydmclab-1.1.4/tests/test_struc.py
+-rw-r--r--   0 cbartel    (503) staff       (20)     1911 2023-06-30 20:01:12.000000 pydmclab-1.1.4/tests/test_submit.py
+-rw-r--r--   0 cbartel    (503) staff       (20)     5986 2024-01-25 21:13:05.000000 pydmclab-1.1.4/tests/test_vasp.py
```

### Comparing `pydmclab-1.0.3/LICENSE.txt` & `pydmclab-1.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pydmclab-1.0.3/PKG-INFO` & `pydmclab-1.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: pydmclab
-Version: 1.0.3
+Version: 1.1.4
 Summary: Package to facilitate DFT calculations and analysis
 Home-page: https://github.umn.edu/bartel-group/pydmclab
 Author: Chris Bartel
 Author-email: cbartel@umn.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6.0
+Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 Provides-Extra: mlp
 Provides-Extra: defects
+Provides-Extra: phonons
 License-File: LICENSE.txt
 
 
 # pydmclab
 
 - common framework to rely upon for typical calculations and analysis done in the Bartel research group
```

### Comparing `pydmclab-1.0.3/pydmclab/core/comp.py` & `pydmclab-1.1.4/pydmclab/core/comp.py`

 * *Files identical despite different names*

### Comparing `pydmclab-1.0.3/pydmclab/core/energies.py` & `pydmclab-1.1.4/pydmclab/core/energies.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import numpy as np
 import math
 from itertools import combinations
+from pymatgen.analysis.reaction_calculator import Reaction
+from pymatgen.core.composition import Composition
+from pymatgen.entries.computed_entries import ComputedStructureEntry
+from pymatgen.analysis.phase_diagram import PhaseDiagram
+from pymatgen.entries.mixing_scheme import MaterialsProjectDFTMixingScheme
 
 from pydmclab.data.thermochem import (
     mp2020_compatibility_dmus,
     mus_at_0K,
     mus_at_T,
     mus_from_mp_no_corrections,
-    mus_from_bartel2019_npj,
+    #    mus_from_bartel2019_npj,
 )
 from pydmclab.data.features import atomic_masses
 from pydmclab.core.comp import CompTools
 from pydmclab.core.struc import StrucTools
 
-from pymatgen.analysis.reaction_calculator import Reaction
-from pymatgen.core.composition import Composition
-
 
 class ChemPots(object):
     """
     return dictionary of chemical potentials {el : chemical potential (eV/at)} based on user inputs
     """
 
     def __init__(
@@ -714,15 +716,14 @@
             out[E_Fermi] = (
                 dE_rxn + charge_contribution[E_Fermi] + charge_correction
             ) / n_defects
         return out
 
 
 class ReactionEnergy(object):
-
     """
     *** This is a work in progress ***
 
     @TODO:
         - write demo
         - incorporate open systems
 
@@ -874,14 +875,140 @@
             # divide by # atoms if norm is per atom
             return dE_rxn / norm_counter
         else:
             # keep molar reaction energy if norm is per mole
             return dE_rxn
 
 
+class MPFormationEnergy(object):
+    """
+    This class allows you to compare your calculations to calculations that are in MP (next-gen version)
+
+    For instance, if you calculate some formation energies and you want to see if your material is stable vs MP,
+    this would be a good way to generate compatible formation energies for the hull analysis
+
+    To get all_entries:
+        Run some calculations on whatever materials you want
+            retrieve their ComputedStructureEntry objects using hpc.helpers.get_entries
+        Query MP for all chemical spaces spanned by those materials
+            eg using core.query.MPQuery.get_entries_for_chemsys or hpc.helpers.get_mp_entries
+        Combine the two lists of entries
+            eg using hpc.helpers.get_merged_entries
+
+    This class gets called by hpc.helpers.get_mp_compatible_Efs
+
+    """
+
+    def __init__(self, all_entries):
+        """
+        Args:
+            all_entries (list)
+                list of ComputedStructureEntry (or ...as_dict()) objects for all calculations you want to consider
+                    could include MP and your own calculations
+
+        Returns:
+            all_entries (list)
+                list of ComputedStructureEntry objects
+            scheme (MaterialsProjectDFTMixingScheme)
+                how to mix functionals (if necessary)
+            queried_entries (list)
+                entries you got from MP
+            my_entries (list)
+                entries that you calculated
+        """
+        if isinstance(all_entries[0], dict):
+            # convert to pymatgen ComputedStructureEntry objects
+            all_entries = [ComputedStructureEntry.from_dict(e) for e in all_entries]
+        for e in all_entries:
+            old_run_type = e.parameters["run_type"]
+            new_run_type = old_run_type.replace("PBE", "GGA")
+            e.parameters["run_type"] = new_run_type
+        self.all_entries = all_entries
+        self.scheme = MaterialsProjectDFTMixingScheme(check_potcar=False)
+        self.queried_entries = [e for e in all_entries if e.data["queried"]]
+        self.my_entries = [
+            e for e in all_entries if "queried" not in e.data or not e.data["queried"]
+        ]
+
+    @property
+    def my_corrected_entries(self):
+        """
+        Returns:
+            list of your entries after applying MP compatibility corrections
+        """
+        scheme = self.scheme
+        entries = self.my_entries
+        formulas = sorted(list(set([e.data["formula"] for e in entries])))
+        mp_entries = self.queried_entries
+        for e in mp_entries:
+            if CompTools(e.data["formula"]).clean not in formulas:
+                entries.append(e)
+        corrected_entries = scheme.process_entries(entries)
+        return corrected_entries
+
+    @property
+    def my_pd(self):
+        """
+        Returns:
+            PhaseDiagram built from your corrected entries
+        """
+        entries = self.my_corrected_entries
+        pd = PhaseDiagram(entries)
+        return pd
+
+    @property
+    def mp_pd(self):
+        """
+        Returns:
+            PhaseDiagram built from MP entries (these were queried from MP so they don't need correcting)
+        """
+        entries = self.queried_entries
+        pd = PhaseDiagram(entries)
+        return pd
+
+    @property
+    def Efs(self):
+        """
+        Returns:
+            {formula (str) :
+                ID (str) :
+                    formation energy (eV/atom)}
+            all formation energies in this dict should be compatible with one another
+            note: this will include all polymorphs
+            note: this will include MP data (ID = mp-id) and your data (ID = formula--ID--standard--mag--xc-calc)
+        """
+        my_pd = self.my_pd
+        my_entries = my_pd.all_entries
+
+        for e in my_entries:
+            Ef = my_pd.get_form_energy_per_atom(e)
+            e.data["Ef"] = Ef
+
+        mp_pd = self.mp_pd
+        mp_entries = mp_pd.all_entries
+
+        for e in mp_entries:
+            Ef = mp_pd.get_form_energy_per_atom(e)
+            e.data["Ef"] = Ef
+
+        entries = mp_entries + my_entries
+
+        formulas = sorted(list(set([e.data["formula"] for e in entries])))
+
+        d = {}
+        for formula in formulas:
+            d[formula] = {}
+            relevant_entries = [e for e in entries if e.data["formula"] == formula]
+            for e in relevant_entries:
+                Ef = e.data["Ef"]
+                ID = e.data["material_id"]
+                d[formula][ID] = Ef
+        return d
+
+
 def main():
     chempots = ChemPots(functional="r2scan", standard="dmc").chempots
 
     # chempots = {"Li": chempots["Li"], "Co": chempots["Co"], "O": chempots["O"]}
     E_pristine = -1.744
     E_defect = -1.461
     formula_pristine = "LiCoO2"
```

### Comparing `pydmclab-1.0.3/pydmclab/core/hulls.py` & `pydmclab-1.1.4/pydmclab/core/hulls.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,32 +1,24 @@
-from pydmclab.core.comp import CompTools
-from pydmclab.core.struc import StrucTools
-from pydmclab.utils.handy import read_json, write_json
-from pydmclab.data.thermochem import (
-    mus_at_0K,
-    mus_at_T,
-    mp2020_compatibility_dmus,
-    mus_from_mp_no_corrections,
-)
-from pydmclab.data.features import atomic_masses
-
-from pymatgen.analysis.phase_diagram import PDEntry, PhaseDiagram, CompoundPhaseDiagram
-from pymatgen.core.composition import Composition
-
-from pydmclab.core.energies import ReactionEnergy
-
 import os
 import numpy as np
+
 from scipy.spatial import ConvexHull
 from scipy.optimize import minimize
-from scipy.stats import mode
+
 import multiprocessing as multip
 
+from pymatgen.analysis.phase_diagram import PDEntry, CompoundPhaseDiagram
+from pymatgen.core.composition import Composition
+
+from pydmclab.core.comp import CompTools
+from pydmclab.utils.handy import read_json, write_json
+from pydmclab.core.energies import ReactionEnergy
+
 
-HERE = os.path.dirname(os.path.abspath(__file__))
+# HERE = os.path.dirname(os.path.abspath(__file__))
 
 """
 Contents:
 
     1) Classes allowing you to compute decomposition energies using the convex hull analysis
         Standard approach:
             - collect formation energies for all compounds in given chemical system(s)
```

### Comparing `pydmclab-1.0.3/pydmclab/core/mag.py` & `pydmclab-1.1.4/pydmclab/core/mag.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,34 @@
-from pydmclab.core.struc import StrucTools, SiteTools
-import itertools
+from itertools import product, islice
 import random
+
 from pymatgen.core.structure import Structure
 from pymatgen.transformations.site_transformations import (
     ReplaceSiteSpeciesTransformation,
 )
 from pymatgen.analysis.structure_matcher import StructureMatcher
+from pymatgen.analysis.magnetism.analyzer import MagneticStructureEnumerator
+
+from pydmclab.core.struc import StrucTools, SiteTools
+
+
+class PymatgenMagTools(object):
+    """
+    Need to get enumlib figured out to use this...
+
+    """
+
+    def __init__(self, structure):
+        st = StrucTools(structure)
+        self.st = st
+
+        self.structure = st.structure
+
+        mse = MagneticStructureEnumerator(self.structure)
+        self.mse = mse
 
 
 class MagTools(object):
     """
     For generating magnetic orderings for structures
     """
 
@@ -255,18 +274,40 @@
 
         # get sites w/ magnetic ions
         magnetic_sites = [
             i for i in range(len(s)) if s[i].species_string in magnetic_ions_in_struc
         ]
 
         print("%i magnetic sites" % len(magnetic_sites))
+
+        if len(magnetic_sites) % 2:
+            return []
+
+        spin_sum = 0.5 * len(magnetic_sites)
+
+        def filter_by_sum(c):
+            return sum(c) == spin_sum
+
+        combos = filter(
+            filter_by_sum,
+            product(range(len(spins)), repeat=len(magnetic_sites)),
+        )
+
+        print("filtered")
+
+        combos = list(islice(combos, int(1e6)))
+
+        print("isliced")
+        combos = list(combos)
         # enumerate all possible ways to yield afm ordering
-        combos = itertools.product(range(len(spins)), repeat=len(magnetic_sites))
+        #        combos = itertools.product(range(len(spins)), repeat=len(magnetic_sites))
+
+        #        print('enumerated %i combos' % len(list(combos)))
 
-        combos = [c for c in combos if sum(c) == 0.5 * len(magnetic_sites)]
+        #        combos = [c for c in combos if np.sum(c) == 0.5 * len(magnetic_sites)]
         print("%i afm combos" % len(combos))
 
         # randomly reduce list if too big for practical usage
         if len(combos) > max_combos:
             combos = random.Random(0).sample(combos, max_combos)
             print("reduced to: %i afm combos" % len(combos))
 
@@ -288,17 +329,19 @@
         # replace spin-up and spin-down sites with new species for symmetry matching
         fake_strucs = []
         for struc in strucs_with_magmoms:
             magmom = struc.site_properties["magmom"]
             spin_up = [i for i in magnetic_sites if magmom[i] == spins[1]]
             spin_down = [i for i in magnetic_sites if magmom[i] == spins[0]]
             indices_species_map = {
-                idx: struc[idx].species_string + "8+"
-                if idx in spin_up
-                else struc[idx].species_string + "8-"
+                idx: (
+                    struc[idx].species_string + "8+"
+                    if idx in spin_up
+                    else struc[idx].species_string + "8-"
+                )
                 for idx in spin_up + spin_down
             }
             rsst = ReplaceSiteSpeciesTransformation(indices_species_map)
             s_tmp = rsst.apply_transformation(struc)
             fake_strucs.append(s_tmp)
         fake_strucs_dict = dict(zip(list(range(len(fake_strucs))), fake_strucs))
 
@@ -333,12 +376,15 @@
             for i in range(len(afm_strucs)):
                 magmoms[i] = afm_strucs[i].site_properties["magmom"]
 
         return magmoms
 
 
 def main():
+    # fcif = "/Users/cbartel/Downloads/Cr2O3.cif"
+    # mt = PymatgenMagTools(fcif)
+    # return mt
     return
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pydmclab-1.0.3/pydmclab/core/struc.py` & `pydmclab-1.1.4/pydmclab/core/struc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from pydmclab.core.comp import CompTools
+import os
+import numpy as np
 
 from pymatgen.core.structure import Structure
 from pymatgen.transformations.standard_transformations import (
     OrderDisorderedStructureTransformation,
     AutoOxiStateDecorationTransformation,
     OxidationStateDecorationTransformation,
 )
 from pymatgen.analysis.structure_matcher import StructureMatcher
 from pymatgen.symmetry.analyzer import SpacegroupAnalyzer
 from pymatgen.core.surface import SlabGenerator
 
-import os
-import numpy as np
+from pydmclab.core.comp import CompTools
 
 
 class StrucTools(object):
     """
     Purpose: to manipulate crystal structures for DFT calculations
     """
 
@@ -403,14 +403,17 @@
         self,
         miller=(1, 0, 0),
         min_slab_size=10,
         min_vacuum_size=10,
         center_slab=True,
         in_unit_planes=False,
         reorient_lattice=True,
+        symmetrize=True,
+        tolerance=0.1,
+        ftolerance=0.1,
     ):
         """
         Args:
             TODO
 
         Returns:
             TODO
@@ -436,29 +439,50 @@
             min_slab_size=min_slab_size,
             min_vacuum_size=min_vacuum_size,
             center_slab=center_slab,
             in_unit_planes=in_unit_planes,
             reorient_lattice=reorient_lattice,
         )
 
-        slabs = slabgen.get_slabs(symmetrize=True)
+        slabs = slabgen.get_slabs(symmetrize=symmetrize, tol=tolerance, ftol=ftolerance)
 
         out = {}
         for i, slab in enumerate(slabs):
             key = (
                 "".join([str(v) for v in miller])
                 + "_"
                 + str(min_vacuum_size)
                 + "_"
                 + str(i)
             )
             out[key] = slab.as_dict()
 
         return out
 
+    def structure_to_cif(self, filename, data_dir=None):
+        """
+        Coverts a structure to a cif file and saves it to a directory, useful for VESTA viewing
+
+        Args:
+            filename (str): name of cif file
+            data_dir (str): path to directory to save cif file
+
+        Returns:
+            None
+        """
+        if not data_dir:
+            data_dir = os.getcwd()
+
+        if not os.path.exists(data_dir):
+            os.makedirs(data_dir)
+
+        self.structure.to(filename=os.path.join(data_dir, f"{filename}.cif"))
+
+        return None
+
 
 class SiteTools(object):
     """
     Purpose: make it a little easier to get site info from structures
 
     """
 
@@ -594,15 +618,7 @@
         d = self.site_dict
         ox = 0
         species = d["species"]
         for entry in species:
             if entry["oxidation_state"]:
                 ox += entry["oxidation_state"] * entry["occu"]
         return ox
-
-
-def main():
-    return
-
-
-if __name__ == "__main__":
-    main()
```

### Comparing `pydmclab-1.0.3/pydmclab/data/.DS_Store` & `pydmclab-1.1.4/pydmclab/data/.DS_Store`

 * *Files identical despite different names*

### Comparing `pydmclab-1.0.3/pydmclab/data/configs.py` & `pydmclab-1.1.4/pydmclab/data/configs.py`

 * *Files identical despite different names*

### Comparing `pydmclab-1.0.3/pydmclab/data/data/221220_dmc-mus.json` & `pydmclab-1.1.4/pydmclab/data/data/221220_dmc-mus.json`

 * *Files identical despite different names*

### Comparing `pydmclab-1.0.3/pydmclab/data/data/230122_dmc-mus.json` & `pydmclab-1.1.4/pydmclab/data/data/230122_dmc-mus.json`

 * *Files identical despite different names*

### Comparing `pydmclab-1.0.3/pydmclab/data/data/230614_dmc-mus.json` & `pydmclab-1.1.4/pydmclab/data/data/230614_dmc-mus.json`

 * *Files identical despite different names*

### Comparing `pydmclab-1.0.3/pydmclab/data/data/_batch_vasp_analysis_configs.yaml` & `pydmclab-1.1.4/pydmclab/data/data/_batch_vasp_analysis_configs.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 only_static: True # only retrieve data from the static calculations
 one_xc: # if None, retrieve all xcs, else retrieve only the one specified
 check_relax: True # make sure the relax calculation and the static have similar energies
 include_meta: True # include metadata like INCAR, KPOINTS, POTCAR settings
 include_calc_setup: True # include things related to the calculation setup -- standard, mag, final_xc, etc
 include_structure: False # include the relaxed crystal structure as a dict
+include_trajectory: False # include the compact trajectory from the vasprun.xml
 include_mag: False # include the relaxed magnetization info as as dict
 include_tdos: False # include the light version of the density of states
 include_pdos: False # include heavy dos
 include_charge: False # include partial chage info
 include_madelung: False # include Madelung energies
 include_tcohp: False # include light COHPCAR data
 include_pcohp: False # include heavy COHPCAR data
 include_tcoop: False # include light COOPCAR data
 include_pcoop: False # include heavy COOPCAR data
 include_tcobi: False # include light COBICAR data
 include_pcobi: False # include heavy COBICAR data
+include_entry: False # include pymatgen computed structure entry
 create_cif: True # create a .cif file for each CONTCAR
 verbose: True # print stuff as things get analyzed
 n_procs: 1 # how many cores to parallelize the analysis over
```

### Comparing `pydmclab-1.0.3/pydmclab/data/data/_partition_configs.yaml` & `pydmclab-1.1.4/pydmclab/data/data/_partition_configs.yaml`

 * *Files identical despite different names*

### Comparing `pydmclab-1.0.3/pydmclab/data/data/_slurm_configs.yaml` & `pydmclab-1.1.4/pydmclab/data/data/_slurm_configs.yaml`

 * *Files identical despite different names*

### Comparing `pydmclab-1.0.3/pydmclab/data/data/_sub_configs.yaml` & `pydmclab-1.1.4/pydmclab/data/data/_sub_configs.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 vasp: vasp_std # use vasp_gam for "loose" calcs (havent implemented yet)
-#vasp_dir: /home/cbartel/shared/bin/vasp/ # where vasp executable lives
+vasp_version: 6 # version of VASP
 mpi_command: mpirun # how to launch on multicore/multinode (may be mpirun depending on compilation)
 manager: '#SBATCH' # how to manage interactions with the queue (some machines dont use slurm)
 machine: msi # which supercomputer
 
 fqueue: q.o # this will be created in the folder where you execute python
 
 fresh_restart: False # True if you want to re-run all calculations; False if you want to pick up where you left off
@@ -11,14 +11,16 @@
 
 files_to_inherit: ['WAVECAR', 'CONTCAR'] # usually no need to change
 
 execute_flags: ['srun', 'python', 'lobster', 'bader', 'mpirun'] # what to look for in a submission script to see if it should be launched
 
 perturb_first_struc: 0.1 # if float, perturb internal coordinates of all ions for POSCAR of first structure by perturb_first_struc
 
+skip_loose: False
+
 # this defines what jobs should be chained together and in what order they should be executed
 # if you only wanted to run a static calculation for metagga, you might pass packing['metagga'] = ['metagga-static']
 packing: 
  gga: 
   - gga-loose
   - gga-relax
   - gga-static
```

### Comparing `pydmclab-1.0.3/pydmclab/data/data/_vasp_configs.yaml` & `pydmclab-1.1.4/pydmclab/data/data/_vasp_configs.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -14,14 +14,21 @@
 generate_bandstructure: False # if True, run a bandstructure calculation at the end
 bs_symprec: 0.1 # symprec for generating primitive cell for bs calculation
 bs_line_density: 20 # kpoint line density for bs calculation
 generate_parchg: False # if True, generate a partial charge
 eint_for_parchg: -1 # the lower energy (relative to E_Fermi) that you want to analyze
 generate_dielectric: False # if True, prepare the INCAR for the static calculation to generate the dielectric tensor
 
+generate_finite_displacements: False # if True, run finite displacements
+supercell_grid_for_finite_displacements: [2,2,2] # supercell grid for finite displacements
+
+generate_dfpt: False # if True, run dfpt
+supercell_grid_for_dfpt: [2,2,2] # supercell grid for dfpt
+
+generate_magtest: False # this will pass MAGMOMs from relax to a new static calc
 
 # some output files
 fvaspout: vasp.o # where vasp output goes in calc_dir for each vasp run
 fvasperrors: errors.o # where vasp errors go in calc_dir for each vasp run
 
 # may be desirable to pass various configs for each type of calculation
 # INCARs should be {INCAR_FLAG : value}
```

### Comparing `pydmclab-1.0.3/pydmclab/data/data/atomic_masses.json` & `pydmclab-1.1.4/pydmclab/data/data/atomic_masses.json`

 * *Files identical despite different names*

### Comparing `pydmclab-1.0.3/pydmclab/data/data/bartel2019_npj_reference-energies.csv` & `pydmclab-1.1.4/pydmclab/data/data/bartel2019_npj_reference-energies.csv`

 * *Files identical despite different names*

### Comparing `pydmclab-1.0.3/pydmclab/data/data/colors.json` & `pydmclab-1.1.4/pydmclab/data/data/colors.json`

 * *Files identical despite different names*

### Comparing `pydmclab-1.0.3/pydmclab/data/data/elemental_gibbs_energies_T.json` & `pydmclab-1.1.4/pydmclab/data/data/elemental_gibbs_energies_T.json`

 * *Files identical despite different names*

### Comparing `pydmclab-1.0.3/pydmclab/data/data/gas_thermo_data_nist.json` & `pydmclab-1.1.4/pydmclab/data/data/gas_thermo_data_nist.json`

 * *Files identical despite different names*

### Comparing `pydmclab-1.0.3/pydmclab/data/data/mus_from_bartel2019_npj.json` & `pydmclab-1.1.4/pydmclab/data/data/mus_from_bartel2019_npj.json`

 * *Files identical despite different names*

### Comparing `pydmclab-1.0.3/pydmclab/data/data/mus_from_mp_no_corrections.json` & `pydmclab-1.1.4/pydmclab/data/data/mus_from_mp_no_corrections.json`

 * *Files identical despite different names*

### Comparing `pydmclab-1.0.3/pydmclab/data/data/ssub.dat` & `pydmclab-1.1.4/pydmclab/data/data/ssub.dat`

 * *Files identical despite different names*

### Comparing `pydmclab-1.0.3/pydmclab/data/data/ssub.json` & `pydmclab-1.1.4/pydmclab/data/data/ssub.json`

 * *Files identical despite different names*

### Comparing `pydmclab-1.0.3/pydmclab/data/plotting_configs.py` & `pydmclab-1.1.4/pydmclab/data/plotting_configs.py`

 * *Files identical despite different names*

### Comparing `pydmclab-1.0.3/pydmclab/data/thermochem.py` & `pydmclab-1.1.4/pydmclab/data/thermochem.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,21 +13,21 @@
     """
     These were run by Bartel in January 20223
     """
     fjson = os.path.join(DATA_PATH, "mus_from_dmc_no_corrections.json")
     if os.path.exists(fjson):
         return read_json(fjson)
     mus = {}
-    d = read_json(os.path.join(DATA_PATH, "230614_dmc-mus.json"))
-    for xc in d:
-        if xc == "gga":
-            functional = "pbe"
-        elif xc == "metagga":
-            functional = "r2scan"
-        mus[functional] = d[xc]
+    mus = read_json(os.path.join(DATA_PATH, "231002_dmc-mus.json"))
+#    for xc in d:
+#        if xc == "gga":
+#            functional = "pbe"
+#        elif xc == "metagga":
+#            functional = "r2scan"
+#        mus[functional] = d[xc]
     return write_json(mus, fjson)
 
 
 def mus_at_T():
     """
     These come from Bartel 2018 Nat Comm
     """
```

### Comparing `pydmclab-1.0.3/pydmclab/dev/defects.py` & `pydmclab-1.1.4/pydmclab/dev/defects.py`

 * *Files identical despite different names*

### Comparing `pydmclab-1.0.3/pydmclab/dev/echem.py` & `pydmclab-1.1.4/pydmclab/dev/echem.py`

 * *Files identical despite different names*

### Comparing `pydmclab-1.0.3/pydmclab/dev/entries.py` & `pydmclab-1.1.4/pydmclab/dev/entries.py`

 * *Files identical despite different names*

### Comparing `pydmclab-1.0.3/pydmclab/dev/mixing_pmg.py` & `pydmclab-1.1.4/pydmclab/dev/mixing_pmg.py`

 * *Files identical despite different names*

### Comparing `pydmclab-1.0.3/pydmclab/dev/query_new_mp_api.py` & `pydmclab-1.1.4/pydmclab/dev/query_new_mp_api.py`

 * *Files identical despite different names*

### Comparing `pydmclab-1.0.3/pydmclab/hpc/README.md` & `pydmclab-1.1.4/pydmclab/hpc/README.md`

 * *Files identical despite different names*

### Comparing `pydmclab-1.0.3/pydmclab/hpc/analyze.py` & `pydmclab-1.1.4/pydmclab/hpc/analyze.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import os
 import numpy as np
 import multiprocessing as multip
 import json
 
-from pymatgen.io.vasp.outputs import Vasprun, Outcar, Eigenval
+from pymatgen.io.vasp.outputs import Vasprun, Outcar, Eigenval, Oszicar
 from pymatgen.core.structure import Structure
 from pymatgen.io.vasp.inputs import Kpoints, Incar
 from pymatgen.io.lobster.outputs import Doscar, Cohpcar, Charge, MadelungEnergies
 
 from pydmclab.core.struc import StrucTools, SiteTools
+from pydmclab.core.comp import CompTools
 from pydmclab.utils.handy import read_json, write_json, read_yaml, write_yaml
 from pydmclab.data.configs import load_batch_vasp_analysis_configs
 
 
 class VASPOutputs(object):
     def __init__(self, calc_dir):
         """
@@ -150,14 +151,29 @@
         try:
             oc = Outcar(os.path.join(self.calc_dir, "OUTCAR"))
             return oc
         except:
             return None
 
     @property
+    def oszicar(self):
+        """
+        Returns Oszicar object from OSZICAR in calc_dir
+        """
+        foszicar = os.path.join(self.calc_dir, "OSZICAR")
+        if not os.path.exists(foszicar):
+            return None
+
+        try:
+            oz = Oszicar(os.path.join(self.calc_dir, "OSZICAR"))
+            return oz
+        except:
+            return None
+
+    @property
     def eigenval(self):
         """
         Returns Eigenval object from EIGENVAL in calc_dir
         """
         feigenval = os.path.join(self.calc_dir, "EIGENVAL")
         if not os.path.exists(feigenval):
             return None
@@ -412,14 +428,32 @@
         out = {}
         for site in sites_to_els:
             el = sites_to_els[site]
             orbs = els_to_orbs[el]
             out[site] = orbs
         return out
 
+    @property
+    def compact_trajectory(self):
+        """
+        Returns:
+            list of tuples summarizing the trajectory : (step, energy, structure (pymatgen.Structure))
+        """
+        if self.is_converged:
+            vr = self.outputs.vasprun
+            nsites = self.nsites
+
+            if vr and nsites:
+                energies = [step["e_wo_entrp"] / nsites for step in vr.ionic_steps]
+                structures = [step["structure"].as_dict() for step in vr.ionic_steps]
+                return list(zip(range(len(energies)), energies, structures))
+            return None
+        else:
+            return None
+
     def pdos(self, fjson=None, remake=False):
         """
         @TODO: add demo/test
 
         Returns complex dict of projected DOS data
             - uses DOSCAR.lobster as of now (must run LOBSTER first)
 
@@ -647,16 +681,22 @@
                 sorted_sites = (sites[1], sites[0])
             el_tag = "-".join(sorted(els))
             site_tag = "-".join([str(site) for site in sorted_sites])
             bond_length = cohp[bond_idx]["length"]
             if el_tag not in out:
                 out[el_tag] = {}
             out[el_tag][site_tag] = {
-                "cohp": {"1": list(np.zeros(len(energies))), "-1": list(np.zeros(len(energies)))},
-                "icohp": {"-1": list(np.zeros(len(energies))), "1": list(np.zeros(len(energies)))},
+                "cohp": {
+                    "1": list(np.zeros(len(energies))),
+                    "-1": list(np.zeros(len(energies))),
+                },
+                "icohp": {
+                    "-1": list(np.zeros(len(energies))),
+                    "1": list(np.zeros(len(energies))),
+                },
                 "length": bond_length,
             }
             out[el_tag][site_tag]["cohp"]["total"] = np.zeros(len(energies))
             out[el_tag][site_tag]["icohp"]["total"] = np.zeros(len(energies))
             for spin in cohp[bond_idx]["COHP"]:
                 if spin.name == "up":
                     spin_tag = "1"
@@ -747,27 +787,22 @@
             if el_tag == "E":
                 continue
             out[el_tag] = {}
             tmp_cohp = np.zeros(len(out["E"]))
             tmp_icohp = np.zeros(len(out["E"]))
             for site_tag in pcohp[el_tag]:
                 for spin in pcohp[el_tag][site_tag]["cohp"]:
-
                     cohp_to_add = np.array(pcohp[el_tag][site_tag]["cohp"][spin])
-#                    print(cohp_to_add)
+                    #                    print(cohp_to_add)
                     if len(cohp_to_add) == len(tmp_cohp):
-                        tmp_cohp = np.add(cohp_to_add
-                                          , tmp_cohp
-                        )
-                    
+                        tmp_cohp = np.add(cohp_to_add, tmp_cohp)
+
                     icohp_to_add = np.array(pcohp[el_tag][site_tag]["icohp"][spin])
                     if len(icohp_to_add) == len(tmp_icohp):
-                        tmp_icohp = np.add(
-                            icohp_to_add, tmp_icohp
-                        )
+                        tmp_icohp = np.add(icohp_to_add, tmp_icohp)
 
             out[el_tag]["cohp"] = tmp_cohp
             out[el_tag]["icohp"] = tmp_icohp
 
         for el_tag in out:
             if el_tag == "E":
                 continue
@@ -1046,31 +1081,60 @@
             "ID": ID,
             "standard": standard,
             "mag": mag,
             "xc": xc_calc.split("-")[0],
             "calc": xc_calc.split("-")[1],
         }
 
+    @property
+    def computed_structure_entry(self):
+        """
+        Returns:
+            ComputedStructureEntry
+        """
+        calc_setup = self.calc_setup
+        vr = self.outputs.vasprun
+        if not vr:
+            return None
+        entry = vr.get_computed_entry()
+        for key in calc_setup:
+            entry.data[key] = calc_setup[key]
+        entry.data["material_id"] = "--".join(
+            [
+                entry.data["formula_tag"],
+                entry.data["ID"],
+                entry.data["standard"],
+                entry.data["mag"],
+                entry.data["xc"],
+                entry.data["calc"],
+            ]
+        )
+        entry.data["formula"] = CompTools(entry.composition.reduced_formula).clean
+        entry.data["queried"] = False
+        return entry.as_dict()
+
     def summary(
         self,
         include_meta=False,
         include_calc_setup=False,
         include_structure=False,
+        include_trajectory=False,
         include_mag=False,
         include_tdos=False,
         include_pdos=False,
         include_gap=True,
         include_charge=True,
         include_madelung=True,
         include_tcohp=False,
         include_pcohp=False,
         include_tcoop=False,
         include_pcoop=False,
         include_tcobi=False,
         include_pcobi=False,
+        include_entry=False,
     ):
         """
         Returns all desired data for post-processing DFT calculations
 
         Args:
             include_meta (bool, optional): _description_. Defaults to False.
             include_calc_setup (bool, optional): _description_. Defaults to False.
@@ -1094,14 +1158,16 @@
                 data["meta"] = {}
             data["meta"]["setup"] = self.calc_setup
         if include_structure:
             # data["structure"] = self.decorated_structure(
             #    charge_source="bader", structure=None
             # )
             data["structure"] = self.relaxed_structure
+        if include_trajectory:
+            data["trajectory"] = self.compact_trajectory
         if include_mag:
             data["magnetization"] = self.magnetization
         if include_tdos:
             pdos = self.pdos()
             tdos = self.tdos(pdos=pdos)
             data["tdos"] = tdos
         if include_pdos:
@@ -1126,14 +1192,16 @@
             data["tcoop"] = self.tcohp(are_coops=True)
         if include_pcoop:
             data["pcoop"] = self.pcohp(are_coops=True)
         if include_tcobi:
             data["tcobi"] = self.tcohp(are_cobis=True)
         if include_pcobi:
             data["pcobi"] = self.pcohp(are_cobis=True)
+        if include_entry:
+            data["entry"] = self.computed_structure_entry
         return data
 
 
 class AnalyzeBatch(object):
     def __init__(
         self,
         launch_dirs,
@@ -1231,44 +1299,48 @@
         """
 
         configs = self.configs.copy()
         verbose = configs["verbose"]
         include_meta = configs["include_meta"]
         include_calc_setup = configs["include_calc_setup"]
         include_structure = configs["include_structure"]
+        include_trajectory = configs["include_trajectory"]
         include_mag = configs["include_mag"]
         include_tdos = configs["include_tdos"]
         include_pdos = configs["include_pdos"]
         include_tcohp = configs["include_tcohp"]
         include_pcohp = configs["include_pcohp"]
         include_tcoop = configs["include_tcoop"]
         include_pcoop = configs["include_pcoop"]
         include_tcobi = configs["include_tcobi"]
         include_pcobi = configs["include_pcobi"]
+        include_entry = configs["include_entry"]
         check_relax = configs["check_relax"]
         create_cif = configs["create_cif"]
 
         if verbose:
             print("analyzing %s" % calc_dir)
         analyzer = AnalyzeVASP(calc_dir)
 
         # collect the data we asked for
         summary = analyzer.summary(
             include_meta=include_meta,
             include_calc_setup=include_calc_setup,
             include_structure=include_structure,
+            include_trajectory=include_trajectory,
             include_mag=include_mag,
             include_tdos=include_tdos,
             include_pdos=include_pdos,
             include_tcohp=include_tcohp,
             include_pcohp=include_pcohp,
             include_tcoop=include_tcoop,
             include_pcoop=include_pcoop,
             include_tcobi=include_tcobi,
             include_pcobi=include_pcobi,
+            include_entry=include_entry,
         )
 
         # store the relax energy if we asked to
         if check_relax:
             relax_energy = AnalyzeVASP(calc_dir.replace("static", "relax")).E_per_at
             summary["meta"]["E_relax"] = relax_energy
             if not relax_energy:
```

### Comparing `pydmclab-1.0.3/pydmclab/hpc/helpers.py` & `pydmclab-1.1.4/pydmclab/hpc/helpers.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 import multiprocessing as multip
 import os
 from pydmclab.hpc.launch import LaunchTools
 from pydmclab.hpc.submit import SubmitTools
 from pydmclab.hpc.analyze import AnalyzeVASP, AnalyzeBatch
-from pydmclab.core.query import MPQuery
+from pydmclab.core.comp import CompTools
+from pydmclab.core.query import MPQuery, MPLegacyQuery
 from pydmclab.core.struc import StrucTools
 from pydmclab.core.mag import MagTools
-from pydmclab.core.energies import ChemPots, FormationEnthalpy
+from pydmclab.core.energies import ChemPots, FormationEnthalpy, MPFormationEnergy
 from pydmclab.utils.handy import read_json, write_json
 from pydmclab.data.configs import load_partition_configs
 
+# from pymatgen.entries.computed_entries import ComputedStructureEntry
+
 
 def get_vasp_configs(
     run_lobster=False,
     run_bandstructure=False,
     run_parchg=False,
     run_dielectric=False,
-    detailed_dos=True,
+    run_phonons=False,
+    phonon_mode="dfpt",
+    run_magtest=False,
+    detailed_dos=False,
     modify_loose_incar=False,
     modify_relax_incar=False,
     modify_static_incar=False,
     modify_loose_kpoints=False,
     modify_relax_kpoints=False,
     modify_static_kpoints=False,
     modify_loose_potcar=False,
@@ -45,14 +51,19 @@
         run_parchg (bool):
             True to run a parchg calculation after your static calculations
                 sets vasp_configs['generate_parchg'] = True
 
         run_dielectric (bool):
             True to get the dielectric tensor on your static calculation
 
+        run_phonons (False or list):
+            False = don't do phonons
+            list (3 elements) = supercell expansion for finite displacements (eg [2, 3, 4])
+            True = use default supercell expansion = [2, 2, 2]
+
         detailed_dos (bool or int):
             if you're running LOBSTER, this will determine how many (E, DOS/COHP) points you get
                 if False, COHPSteps = 400
                 if True, COHPSteps = 4000
                 if int, COHPSteps = detailed_dos
             if run_lobster is False, this is ignored
 
@@ -91,31 +102,33 @@
 
     Returns:
         dictionary of VASP_CONFIGS
             {config_key : config_value}
 
             to get passed as user_configs to VASPSetUp (through SubmitTools)
     """
-    # DOS-related
     vasp_configs = {
         "lobster_static": run_lobster,
         "generate_bandstructure": run_bandstructure,
         "generate_parchg": run_parchg,
         "generate_dielectric": run_dielectric,
+        "generate_magtest": run_magtest,
     }
 
+    if isinstance(run_phonons, list):
+        vasp_configs["supercell_grid_for_%s" % phonon_mode] = run_phonons
+        generate_finite_displacements = True
+    else:
+        generate_finite_displacements = run_phonons
+
+    vasp_configs["generate_%s" % phonon_mode] = generate_finite_displacements
+
     if vasp_configs["generate_bandstructure"]:
         vasp_configs["lobster_static"] = True
 
-    if detailed_dos:
-        if type(detailed_dos) == bool:
-            vasp_configs["COHPSteps"] = 4000
-        else:
-            vasp_configs["COHPSteps"] = detailed_dos
-
     # INCARs
     if modify_loose_incar:
         vasp_configs["loose_incar"] = modify_loose_incar
     if modify_relax_incar:
         vasp_configs["relax_incar"] = modify_relax_incar
     if modify_static_incar:
         vasp_configs["static_incar"] = modify_static_incar
@@ -132,14 +145,28 @@
     if modify_loose_potcar:
         vasp_configs["loose_potcar"] = modify_loose_potcar
     if modify_relax_potcar:
         vasp_configs["relax_potcar"] = modify_relax_potcar
     if modify_static_potcar:
         vasp_configs["static_potcar"] = modify_static_potcar
 
+    if detailed_dos:
+        if isinstance(detailed_dos, bool):
+            vasp_configs["COHPSteps"] = 4000
+        else:
+            vasp_configs["COHPSteps"] = detailed_dos
+
+        if ("static_incar" in vasp_configs) and isinstance(
+            vasp_configs["static_incar"], dict
+        ):
+            vasp_configs["static_incar"]["NEDOS"] = vasp_configs["COHPSteps"]
+
+        else:
+            vasp_configs["static_incar"] = {"NEDOS": vasp_configs["COHPSteps"]}
+
     return vasp_configs
 
 
 def get_slurm_configs(
     total_nodes=1,
     cores_per_node=8,
     walltime_in_hours=95,
@@ -234,14 +261,16 @@
 def get_sub_configs(
     machine="msi",
     submit_calculations_in_parallel=False,
     delete_all_calculations_and_start_over=False,
     rerun_lobster=False,
     mpi_command="mpirun",
     special_packing=False,
+    vasp_version=6,
+    skip_loose=False,
 ):
     """
 
     configs related to preparing submission scripts and submitting VASP calculations
 
         see defaults in pydmclab.data.data._sub_configs.yaml
         see pydmclab.hpc.submit.SubmitTools for more info
@@ -296,14 +325,19 @@
     if special_packing:
         sub_configs["packing"] = {}
         for xc in special_packing:
             sub_configs["packing"][xc] = special_packing[xc]
 
     sub_configs["machine"] = machine
 
+    sub_configs["vasp_version"] = vasp_version
+
+    if skip_loose:
+        sub_configs["skip_loose"] = True
+
     return sub_configs
 
 
 def get_launch_configs(
     standards=["dmc"],
     xcs=["metagga"],
     use_mp_thermo_data=False,
@@ -354,17 +388,16 @@
         for xc in xcs:
             if (standard in skip_xcs_for_standards) and (
                 xc in skip_xcs_for_standards[standard]
             ):
                 continue
             to_launch[standard].append(xc)
 
-    for standard in to_launch:
-        if not to_launch[standard]:
-            del to_launch[standard]
+    standards_to_keep = [standard for standard in to_launch if to_launch[standard]]
+    to_launch = {standard: to_launch[standard] for standard in standards_to_keep}
 
     if use_mp_thermo_data:
         # make sure we run GGA+U for MP consistency
         to_launch["mp"] = ["ggau"]
 
     launch_configs["to_launch"] = to_launch
 
@@ -372,14 +405,15 @@
 
     return launch_configs
 
 
 def get_analysis_configs(
     analyze_calculations_in_parallel=False,
     analyze_structure=True,
+    analyze_trajectory=False,
     analyze_mag=False,
     analyze_charge=False,
     analyze_dos=False,
     analyze_bonding=False,
     exclude=[],
 ):
     """
@@ -391,14 +425,17 @@
             - False: use 1 processor
             - True: use all available processors
             - int: use that many processors
 
         analyze_structure (bool, optional):
             True to include structure in your results
 
+        analyze_trajectory (bool, optional):
+            True to include trajectory in your results
+
         analyze_mag (bool, optional):
             True to include magnetization in your results
 
         analyze_charge (bool, optional):
             True to include bader charge + lobster charges + madelung in your results
 
         analyze_dos (bool, optional):
@@ -429,14 +466,17 @@
 
     analysis_configs["n_procs"] = n_procs
 
     includes = []
     if analyze_structure:
         includes.append("structure")
 
+    if analyze_trajectory:
+        includes.append("trajectory")
+
     if analyze_mag:
         includes.append("mag")
 
     if analyze_charge:
         includes.extend(["charge", "madelung"])
 
     if analyze_dos:
@@ -452,14 +492,112 @@
         for ex in exclude:
             analysis_configs["include_" + ex] = False
 
     return analysis_configs
 
 
 def get_query(
+    api_key,
+    search_for,
+    properties=None,
+    max_Ehull=0.1,
+    max_sites_per_structure=100,
+    max_polymorph_energy=0.1,
+    only_gs=False,
+    include_structure=True,
+    max_strucs_per_cmpd=5,
+    include_sub_phase_diagrams=False,
+    data_dir=os.getcwd().replace("scripts", "data"),
+    savename="query.json",
+    remake=False,
+):
+    """
+    Args:
+        api_key (str)
+            your API key (should be 32 characters)
+        search_for (str or list)
+            can either be:
+                - a chemical system (str) of elements joined by "-"
+                - a chemical formula (str)
+                - an MP ID (str)
+            can either be a list of:
+                - chemical systems (str) of elements joined by "-"
+                - chemical formulas (str)
+                - MP IDs (str)
+
+        properties (list or None)
+            list of properties to query
+                - if None, then use typical_properties
+                - if 'all', then use all properties
+                - if a string, then add that property to typical_properties
+                - if a list, then add those properties to typical_properties
+
+        band_gap (tuple)
+            band gap range to query
+
+        max_Ehull (float)
+            upper bound on energy above hull to query
+
+        max_sites_per_structure (int)
+            upper bound on number of sites to query
+
+        max_polymorph_energy (float)
+            upper bound on polymorph energy to query
+
+        only_gs (bool)
+            if True, remove non-ground state polymorphs for each unique composition
+
+        include_structure (bool)
+            if True, include the structure (as a dictionary) for each entry
+
+        max_strucs_per_cmpd (int)
+            if not None, only retain the lowest energy structures for each composition until you reach max_strucs_per_cmpd
+
+        include_sub_phase_diagrams (bool)
+            if True, include all sub-phase diagrams for a given composition
+                e.g., if comp = "Sr-Zr-S", then also include "Sr-S" and "Zr-S" in the query
+        data_dir (str)
+            directory to save fjson
+        savename (str)
+            filename for fjson in data_dir
+        remake (bool)
+            write (True) or just read (False) fjson
+    Returns:
+        {ID (str) : {'structure' : Pymatgen Structure as dict,
+                    < any other data you want to keep track of >}}
+    """
+
+    if len(api_key) < 32:
+        raise ValueError("API key should be 32 characters")
+
+    fjson = os.path.join(data_dir, savename)
+    if os.path.exists(fjson) and not remake:
+        return read_json(fjson)
+
+    # initialize MPQuery with your API key
+    mpq = MPQuery(api_key=api_key)
+
+    # get the data from MP
+    data = mpq.get_data(
+        search_for=search_for,
+        properties=properties,
+        max_Ehull=max_Ehull,
+        max_sites_per_structure=max_sites_per_structure,
+        max_polymorph_energy=max_polymorph_energy,
+        only_gs=only_gs,
+        include_structure=include_structure,
+        max_strucs_per_cmpd=max_strucs_per_cmpd,
+        include_sub_phase_diagrams=include_sub_phase_diagrams,
+    )
+
+    write_json(data, fjson)
+    return read_json(fjson)
+
+
+def get_legacy_query(
     comp,
     api_key,
     properties=None,
     criteria=None,
     only_gs=True,
     include_structure=True,
     supercell_structure=False,
@@ -527,15 +665,15 @@
     """
 
     fjson = os.path.join(data_dir, savename)
     if os.path.exists(fjson) and not remake:
         return read_json(fjson)
 
     # initialize MPQuery with your API key
-    mpq = MPQuery(api_key=api_key)
+    mpq = MPLegacyQuery(api_key=api_key)
 
     # get the data from MP
     data = mpq.get_data_for_comp(
         comp=comp,
         properties=properties,
         criteria=criteria,
         only_gs=only_gs,
@@ -797,45 +935,68 @@
 
     """
     launch_dir = submit_args["launch_dir"]
     launch_dirs = submit_args["launch_dirs"]
     user_configs = submit_args["user_configs"]
     refresh_configs = submit_args["refresh_configs"]
     ready_to_launch = submit_args["ready_to_launch"]
+    running_in_parallel = submit_args["parallel"]
+
+    curr_user_configs = user_configs.copy()
 
     if "ID_specific_vasp_configs" in launch_dirs[launch_dir]:
         if launch_dirs[launch_dir]["ID_specific_vasp_configs"]:
-            user_configs.update(launch_dirs[launch_dir]["ID_specific_vasp_configs"])
+            curr_user_configs.update(
+                launch_dirs[launch_dir]["ID_specific_vasp_configs"]
+            )
 
     # what are our terminal xcs for that launch_dir
     final_xcs = launch_dirs[launch_dir]["xcs"]
 
     # what magmoms apply to that launch_dir
     magmom = launch_dirs[launch_dir]["magmom"]
 
-    try:
+    if running_in_parallel:
+        try:
+            sub = SubmitTools(
+                launch_dir=launch_dir,
+                final_xcs=final_xcs,
+                magmom=magmom,
+                user_configs=curr_user_configs,
+                refresh_configs=refresh_configs,
+            )
+
+            # prepare VASP directories and write submission script
+            sub.write_sub
+
+            # submit submission script to the queue
+            if ready_to_launch:
+                sub.launch_sub
+
+            success = True
+        except TypeError:
+            print("\nERROR: %s\n   will submit without multiprocessing" % launch_dir)
+            success = False
+    else:
         sub = SubmitTools(
             launch_dir=launch_dir,
             final_xcs=final_xcs,
             magmom=magmom,
-            user_configs=user_configs,
+            user_configs=curr_user_configs,
             refresh_configs=refresh_configs,
         )
 
         # prepare VASP directories and write submission script
         sub.write_sub
 
         # submit submission script to the queue
         if ready_to_launch:
             sub.launch_sub
 
         success = True
-    except TypeError:
-        print("\nERROR: %s\n   will submit without multiprocessing" % launch_dir)
-        success = False
 
     return {"launch_dir": launch_dir, "success": success}
 
 
 def submit_calcs(
     launch_dirs,
     user_configs={},
@@ -865,14 +1026,15 @@
     """
 
     submit_args = {
         "launch_dirs": launch_dirs,
         "user_configs": user_configs,
         "refresh_configs": refresh_configs,
         "ready_to_launch": ready_to_launch,
+        "parallel": False if n_procs == 1 else True,
     }
 
     if n_procs == 1:
         print("\n\n submitting calculations in serial\n\n")
         for launch_dir in launch_dirs:
             curr_submit_args = submit_args.copy()
             curr_submit_args["launch_dir"] = launch_dir
@@ -1051,14 +1213,15 @@
     for standard in gs:
         for xc in gs[standard]:
             keys = [
                 k
                 for k in results
                 if results[k]["meta"]["setup"]["standard"] == standard
                 if results[k]["meta"]["setup"]["xc"] == xc
+                if results[k]["results"]["formula"]
             ]
 
             unique_formulas = sorted(
                 list(set([results[key]["results"]["formula"] for key in keys]))
             )
             for formula in unique_formulas:
                 gs[standard][xc][formula] = {}
@@ -1405,14 +1568,225 @@
         if "pcobi" in dos_to_store:
             thermo_results[standard][xc][formula][ID]["pcobi"] = pcohp
 
     write_json(thermo_results, fjson)
     return read_json(fjson)
 
 
+def get_entries(
+    results,
+    data_dir=os.getcwd().replace("scripts", "data"),
+    savename="entries.json",
+    remake=False,
+):
+    """
+    Args:
+        results (dict)
+            from get_results
+                {formula--ID--standard--mag--xc-calc (str) : {scraped results from VASP calculation}}
+
+        data_dir (str)
+            path to data directory
+
+        savename (str)
+            name of json file to save results to
+
+        remake (bool)
+            if True, remake the json file
+
+    Returns:
+        dictionary with ComputedStructureEntry objects for each of your completed calculations
+            {'entries' : [list of ComputedStructureEntry.as_dict() objects]}
+
+        note: each of these entries has the "key" from the results dictionary stored as entry['data']['material_id']
+    """
+    fjson = os.path.join(data_dir, savename)
+    if os.path.exists(fjson) and not remake:
+        return read_json(fjson)
+    d = {"entries": [results[k]["entry"] for k in results if results[k]["entry"]]}
+    write_json(d, fjson)
+    return read_json(fjson)
+
+
+def get_mp_entries(
+    chemsyses,
+    api_key,
+    thermo_types=None,
+    data_dir=os.getcwd().replace("scripts", "data"),
+    savename="mp_entries.json",
+    remake=False,
+):
+    """
+    Args:
+        chemsyses (list)
+            list of chemical systems to get entries for (e.g., ['Li-Fe-O', 'Mg-Cr-O'])
+                will include "sub phase diagrams" in query
+                e.g., for 'Li-Fe-O', will include 'Li-Fe-O', 'Li-Fe', 'Li-O', 'Fe-O', 'Li', 'Fe', 'O'
+
+        api_key (str)
+            your Materials Project API key
+
+        thermo_types (list)
+            list of thermo types to get entries for
+                this could be ['GGA_GGA+U'], ['R2SCAN'], ['GGA_GGA+U', 'R2SCAN']
+            if None, will get all data regardless of thermo_type (note: this should be equivalent to thermo_types=['GGA_GGA+U', 'R2SCAN'])
+
+        data_dir (str)
+            path to data directory
+
+        savename (str)
+            name of json file to save results to
+
+        remake (bool)
+            if True, remake the json file
+
+    Returns:
+        dictionary of ComputedStructureEntry objects from the Materials Project
+            {chemsys (str) :
+                [list of ComputedStructureEntry.as_dict() objects]}
+            note: the mp-id is stored as entry['data']['material_id']
+            note: the xc is stored in entry['parameters']['run_type']
+
+    """
+    fjson = os.path.join(data_dir, savename)
+    if os.path.exists(fjson) and not remake:
+        return read_json(fjson)
+
+    mpq = MPQuery(api_key=api_key)
+    out = {}
+    for chemsys in chemsyses:
+        if thermo_types:
+            data = mpq.get_entries_for_chemsys(chemsys, thermo_types=thermo_types)
+        else:
+            data = mpq.get_entries_for_chemsys(chemsys)
+        out[chemsys] = list(data.values())
+    write_json(out, fjson)
+    return read_json(fjson)
+
+
+def get_merged_entries(
+    my_entries,
+    mp_entries,
+    restrict_my_xc_to=None,
+    data_dir=os.getcwd().replace("scripts", "data"),
+    savename="merged_entries_for_mp_Ef.json",
+    remake=False,
+):
+    """
+    Args:
+        my_entries (dict)
+            from get_entries
+                {'entries' : [list of ComputedStructureEntry.as_dict() objects]}
+
+        mp_entries (dict)
+            from get_mp_entries
+                {chemsys (str) : [list of ComputedStructureEntry.as_dict() objects]}
+
+        restrict_my_xc_to (str)
+            if not None, only include my entries with this xc
+                e.g., 'GGA', 'GGA+U', 'r2SCAN'
+
+        data_dir (str)
+            path to data directory
+
+        savename (str)
+            name of json file to save results to
+
+        remake (bool)
+            if True, remake the json file
+
+    Returns:
+        dictionary of ComputedStructureEntry objects from the Materials Project and your calculations
+            {chemsys (str) :
+                [list of ComputedStructureEntry.as_dict() objects]}
+            note: this will exclude any of your calculations where standard != 'mp' because the purpose of this is to compare to MP
+                if you're not comparing to MP, then you can just get your own entries from get_entries
+    """
+    fjson = os.path.join(data_dir, savename)
+    if os.path.exists(fjson) and not remake:
+        return read_json(fjson)
+
+    if restrict_my_xc_to == "GGA":
+        my_allowed_xcs = ["gga"]
+    elif restrict_my_xc_to == "GGA+U":
+        my_allowed_xcs = ["ggau"]
+    elif restrict_my_xc_to == "r2SCAN":
+        my_allowed_xcs = ["r2scan"]
+    elif restrict_my_xc_to == "GGA_GGA+U":
+        my_allowed_xcs = ["gga", "ggau"]
+    else:
+        my_allowed_xcs = None
+
+    entries = {}
+    for chemsys in mp_entries:
+        entries[chemsys] = []
+        mp_entries_for_chemsys = mp_entries[chemsys]
+        for e in mp_entries_for_chemsys:
+            entries[chemsys].append(e)
+
+    relevant_chemsyses = list(entries.keys())
+
+    my_entries = my_entries["entries"]
+    for e in my_entries:
+        if e["data"]["standard"] != "mp":
+            continue
+        if my_allowed_xcs and (e["data"]["xc"] not in my_allowed_xcs):
+            continue
+        formula = e["data"]["formula"]
+        for chemsys in relevant_chemsyses:
+            if set(CompTools(formula).els).issubset(set(chemsys.split("-"))):
+                entries[chemsys].append(e)
+
+    write_json(entries, fjson)
+    return read_json(fjson)
+
+
+def get_mp_compatible_Efs(
+    merged_entries,
+    data_dir=os.getcwd().replace("scripts", "data"),
+    savename="mp_compatible_Efs.json",
+    remake=False,
+):
+    """
+    Args:
+        merged_entries (dict)
+            from get_merged_entries
+                {chemsys (str) : [list of ComputedStructureEntry.as_dict() objects]}
+
+        data_dir (str)
+            path to data directory
+
+        savename (str)
+            name of json file to save results to
+
+        remake (bool)
+            if True, remake the json file
+
+    Returns:
+        dictionary of compatible formation energies for each chemsys
+            {chemsys (str) :
+                {formula (str) :
+                    ID (str) : formation energy (eV/atom)}
+            note: this will include all polymorphs
+            note: this will include MP data (ID = mp-id) and your data (ID = formula--ID--standard--mag--xc-calc)
+    """
+    fjson = os.path.join(data_dir, savename)
+    if os.path.exists(fjson) and not remake:
+        return read_json(fjson)
+
+    out = {}
+    for chemsys in merged_entries:
+        mpfe = MPFormationEnergy(merged_entries[chemsys])
+        Efs = mpfe.Efs
+        out[chemsys] = Efs
+
+    write_json(out, fjson)
+    return read_json(fjson)
+
+
 def crawl_and_purge(
     head_dir,
     files_to_purge=[
         "WAVECAR",
         "CHGCAR",
         "CHG",
         "PROCAR",
```

### Comparing `pydmclab-1.0.3/pydmclab/hpc/launch.py` & `pydmclab-1.1.4/pydmclab/hpc/launch.py`

 * *Files identical despite different names*

### Comparing `pydmclab-1.0.3/pydmclab/hpc/submit.py` & `pydmclab-1.1.4/pydmclab/hpc/submit.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from pydmclab.core.struc import StrucTools
 from pydmclab.hpc.vasp import VASPSetUp
 from pydmclab.hpc.analyze import AnalyzeVASP
 from pydmclab.utils.handy import read_yaml, write_yaml
 from pydmclab.data.configs import (
     load_vasp_configs,
     load_slurm_configs,
     load_sub_configs,
@@ -14,14 +15,18 @@
 
 import multiprocessing as multip
 import os
 from shutil import copyfile, rmtree
 import subprocess
 import warnings
 
+from subprocess import call
+
+from pymatgen.io.vasp.sets import get_structure_from_prev_run
+
 HERE = os.path.dirname(os.path.abspath(__file__))
 
 
 class SubmitTools(object):
     """
     This class is focused on figuring out how to prepare chains of calculations
         the idea being that the output from this class is some file that you can
@@ -298,18 +303,26 @@
 
     @property
     def vasp_dir(self):
         """
         Returns directory containing vasp executable
         """
         machine = self.sub_configs["machine"]
+        version = self.sub_configs["vasp_version"]
         if machine == "msi":
-            return "%s/vasp" % self.bin_dir
+            preamble = "%s/vasp" % self.bin_dir
+            if version == 5:
+                return "%s/vasp.5.4.4.pl2" % preamble
+            elif version == 6:
+                return "%s/vasp.6.4.1" % preamble
         elif machine == "bridges2":
-            return "/opt/packages/VASP/VASP6/6.3+VTST"
+            if version == 6:
+                return "/opt/packages/VASP/VASP6/6.3+VTST"
+            else:
+                raise NotImplementedError("VASP < 6 not on Bridges?")
         else:
             raise NotImplementedError('dont have VASP path for machine "%s"' % machine)
 
     @property
     def vasp_command(self):
         """
         Returns command used to execute vasp
@@ -442,14 +455,23 @@
 
         # determine the terminal ends of each chain of VASP calcs to be submitted
         final_xcs = self.final_xcs
 
         # determine how VASP jobs get chained together
         packing = sub_configs["packing"]
 
+        if sub_configs["skip_loose"]:
+            new_packing = {}
+            for xc in packing:
+                new_packing[xc] = []
+                for calc in packing[xc]:
+                    if "loose" not in calc:
+                        new_packing[xc].append(calc)
+            packing = new_packing.copy()
+
         print("\n\n~~~~~ starting to work on %s ~~~~~\n\n" % launch_dir)
 
         fpos_src = os.path.join(launch_dir, "POSCAR")
 
         # loop through all calculations within each chain and collect statuses
         # statuses = {final_xc : {xc_calc : status}}
         statuses = {}
@@ -507,15 +529,15 @@
                             if not parent_energy:
                                 print(
                                     "     %s (parent) not converged, need to continue this calc"
                                     % parent_xc_calc
                                 )
                             else:
                                 # if there is a large difference b/t the relax and static energy, something fishy happened, so let's start the static calc over
-                                if abs(parent_energy - static_energy) > 0.2:
+                                if abs(parent_energy - static_energy) > 0.05:
                                     print(
                                         "     %s (parent) and %s (child) energies differ by more than 0.2 eV/atom"
                                         % (parent_xc_calc, xc_calc)
                                     )
                                     large_E_diff_between_relax_and_static = True
                         else:
                             parent_convergence = True
@@ -531,15 +553,16 @@
                         # for statics, also check if we want to force postprocess
                         # this means re-compute the static so we can re-run lobster, bader, etc
                         if (
                             convergence
                             and parent_convergence
                             and not fresh_restart
                             and not large_E_diff_between_relax_and_static
-                            and not sub_configs["force_postprocess"]
+                            # note: muting force_postprocess here b/c we want the calc to still be "done", right?
+                            # and not sub_configs["force_postprocess"]
                         ):
                             print("     %s is already converged; skipping" % xc_calc)
                             status = "done"
                             statuses[final_xc][xc_calc] = status
                             continue
                     else:
                         if convergence and parent_convergence and not fresh_restart:
@@ -594,32 +617,39 @@
 
                 # (6) initialize VASPSetUp with current VASP configs for this calculation
                 vsu = VASPSetUp(
                     calc_dir=calc_dir,
                     user_configs=user_vasp_configs_before_error_handling,
                 )
 
+                user_vasp_configs = user_vasp_configs_before_error_handling.copy()
+
                 # (7) check for errors in continuing jobs
                 incar_changes = {}
                 if status in ["continue", "new"]:
                     calc_is_clean = vsu.is_clean
                     if not calc_is_clean:
                         # change INCAR based on errors and include in calc_configs
                         incar_changes = vsu.incar_changes_from_errors
 
                 # if there are INCAR updates, add them to calc_configs
                 if incar_changes:
                     incar_key = "%s_incar" % calc_to_run
-                    if incar_key not in calc_configs:
-                        calc_configs[incar_key] = {}
                     for setting in incar_changes:
-                        calc_configs[incar_key][setting] = incar_changes[setting]
+                        user_vasp_configs[incar_key][setting] = incar_changes[setting]
+
+                # print("\n\n\n\n\n\n")
+                # print(calc_dir)
+                # print("THESE ARE MY USER_VASP_CONFIGS")
+                # print(user_vasp_configs)
+                # print("\n\n\n\n\n\n")
+                # print(calc_dir)
 
                 # update our vasp_configs with any modifications to the INCAR that we made to fix errors
-                user_vasp_configs = {**vasp_configs, **calc_configs}
+                # user_vasp_configs = {**vasp_configs, **calc_configs}
                 print("--------- may be some warnings (POTCAR ones OK) ----------")
 
                 # (8) prepare calc_dir to launch
                 vsu = VASPSetUp(calc_dir=calc_dir, user_configs=user_vasp_configs)
 
                 vsu.prepare_calc
 
@@ -670,19 +700,28 @@
         vasp_command = self.vasp_command
         slurm_options = self.slurm_options.copy()
         queue_manager = self.queue_manager
 
         # determine how jobs will be chained together
         packing = sub_configs["packing"]
 
+        if sub_configs["skip_loose"]:
+            new_packing = {}
+            for xc in packing:
+                new_packing[xc] = []
+                for calc in packing[xc]:
+                    if "loose" not in calc:
+                        new_packing[xc].append(calc)
+            packing = new_packing.copy()
+
         # get our statuses from when we prepared VASP input files for each directory
         # statuses = {final_xc : {xc_calc : status}}
         # e.g., statuses['metagga']['gga-relax'] = 'done'
         statuses = self.prepare_directories
-        for final_xc in statuses:
+        for final_xc, v in statuses.items():
             # initialize a submission script for this chain
             # this is what we'll launch with sbatch sub_...sh
             fsub = os.path.join(launch_dir, "sub_%s.sh" % final_xc)
 
             # initialize a status log file for this chain
             # this is where we'll print status updates (helpful for debugging)
             fstatus = os.path.join(launch_dir, "status_%s.o" % final_xc)
@@ -694,15 +733,15 @@
             # make sure job is not in queue already
             print("\nchecking if %s is in q" % job_name)
             if self.is_job_in_queue(job_name):
                 continue
             slurm_options["job-name"] = job_name
 
             # if job isnt in queue already, start writing our submission script
-            with open(fsub, "w") as f:
+            with open(fsub, "w", encoding="utf-8") as f:
                 # slurm requires this header
                 f.write("#!/bin/bash -l\n")
 
                 # write the SLURM stuff (partition, nodes, time, etc) at the top
                 for key in slurm_options:
                     slurm_option = slurm_options[key]
                     if slurm_option:
@@ -713,15 +752,30 @@
 
                 # this is for running MPI jobs that may require large memory
                 f.write("ulimit -s unlimited\n")
 
                 # load certain modules if needed for MPI command
                 if sub_configs["mpi_command"] == "mpirun":
                     if sub_configs["machine"] == "msi":
-                        f.write("module load impi/2018/release_multithread\n")
+                        if sub_configs["vasp_version"] == 5:
+                            f.write("module load impi/2018/release_multithread\n")
+                        elif sub_configs["vasp_version"] == 6:
+                            unload = [
+                                "mkl",
+                                "intel/2018.release",
+                                "intel/2018/release",
+                                "impi/2018/release_singlethread",
+                                "mkl/2018.release",
+                                "impi/intel",
+                            ]
+                            load = ["mkl/2021/release", "intel/cluster/2021"]
+                            for module in unload:
+                                f.write("module unload %s\n" % module)
+                            for module in load:
+                                f.write("module load %s\n" % module)
                     elif sub_configs["machine"] == "bridges2":
                         f.write("module load intelmpi\nexport OMP_NUM_THREADS=1\n")
 
                 # now write what is needed for the chain of VASP calcs + postprocessing
                 print("\n:::: writing sub now - %s ::::" % fsub)
 
                 # use this counter to figure if there are parents for a given calc and who those parents are
@@ -795,14 +849,78 @@
                                 f.write(
                                     "echo working on %s-parchg >> %s\n"
                                     % (xc_calc, fstatus)
                                 )
                                 f.write("cd %s\n" % parchg_dir)
                                 f.write("%s\n" % vasp_command)
 
+                            if vasp_configs["generate_finite_displacements"]:
+                                phonon_dir = generate_finite_displacements(
+                                    converged_static_dir=calc_dir,
+                                    supercell_grid=vasp_configs[
+                                        "supercell_grid_for_finite_displacements"
+                                    ],
+                                )
+                                print('phonon_dir = "%s"' % phonon_dir)
+                            else:
+                                phonon_dir = None
+
+                            if phonon_dir:
+
+                                disp_statuses = setup_finite_displacement_calcs(
+                                    phonon_dir
+                                )
+                                print(">>> here are disp statuses: ", disp_statuses)
+                                for disp in disp_statuses:
+                                    disp_dir = disp_statuses[disp]["calc_dir"]
+                                    convergence = disp_statuses[disp]["convergence"]
+                                    if convergence:
+                                        continue
+
+                                    f.write(
+                                        "echo working on %s-phonon-%s >> %s\n"
+                                        % (xc_calc, disp, fstatus)
+                                    )
+                                    f.write("cd %s\n" % disp_dir)
+                                    f.write("%s\n" % vasp_command)
+
+                            if vasp_configs["generate_dfpt"]:
+                                phonon_dir = setup_dfpt(
+                                    converged_static_dir=calc_dir,
+                                    supercell_grid=vasp_configs[
+                                        "supercell_grid_for_dfpt"
+                                    ],
+                                )
+                            else:
+                                phonon_dir = None
+
+                            if phonon_dir:
+                                f.write(
+                                    "echo working on %s-dfpt >> %s\n"
+                                    % (xc_calc, fstatus)
+                                )
+                                f.write("cd %s\n" % phonon_dir)
+                                f.write("%s\n" % vasp_command)
+                                f.write("phonopy --fc vasprun.xml\n")
+
+                            if vasp_configs["generate_magtest"]:
+                                magtest_dir = setup_static_magtest(
+                                    converged_static_dir=calc_dir
+                                )
+                            else:
+                                magtest_dir = None
+
+                            if magtest_dir:
+                                f.write(
+                                    "echo working on %s-static_magtest >> %s\n"
+                                    % (xc_calc, fstatus)
+                                )
+                                f.write("cd %s\n" % magtest_dir)
+                                f.write("%s\n" % vasp_command)
+
                         f.write("echo %s is done >> %s\n" % (xc_calc, fstatus))
                     else:
                         if status == "continue":
                             # copy the CONTCAR to the POSCAR
                             f.write(
                                 "cp %s %s\n"
                                 % (
@@ -848,15 +966,15 @@
                                 if file_to_inherit == "CONTCAR":
                                     fdst = os.path.join(calc_dir, "POSCAR")
                                 else:
                                     fdst = os.path.join(calc_dir, file_to_inherit)
                                 if file_to_inherit == "CONTCAR":
                                     # make sure CONTCAR is not empty
                                     if os.path.exists(fsrc):
-                                        with open(fsrc, "r") as f_tmp:
+                                        with open(fsrc, "r", encoding="utf-8") as f_tmp:
                                             contents = f_tmp.readlines()
                                         if len(contents) < 0:
                                             continue
                                 f.write("cp %s %s\n" % (fsrc, fdst))
 
                         # navigate to calculation directory and run vasp
                         f.write("cd %s\n" % calc_dir)
@@ -993,21 +1111,31 @@
 
     # create a primitive cell and write to bs POSCAR (needed so we don't have a bunch of overlapping bands)
     lobsterin.write_POSCAR_with_standard_primitive(
         POSCAR_input=fposcar_src, POSCAR_output=fposcar_dst, symprec=symprec
     )
 
     # create a line-mode KPOINTS file and write to bs KPOINTS
-    lobsterin.write_KPOINTS(
-        POSCAR_input=fposcar_dst,
-        KPOINTS_output=fkpoints_dst,
-        line_mode=True,
-        symprec=symprec,
-        kpoints_line_density=kpoints_line_density,
-    )
+    try:
+        lobsterin.write_KPOINTS(
+            POSCAR_input=fposcar_dst,
+            KPOINTS_output=fkpoints_dst,
+            line_mode=True,
+            symprec=symprec,
+            kpoints_line_density=kpoints_line_density,
+        )
+    except ValueError:
+        print("trying higher symprec")
+        lobsterin.write_KPOINTS(
+            POSCAR_input=fposcar_dst,
+            KPOINTS_output=fkpoints_dst,
+            line_mode=True,
+            symprec=symprec * 2,
+            kpoints_line_density=kpoints_line_density,
+        )
 
     # copy our POTCAR from the static calc
     copyfile(fpotcar_src, fpotcar_dst)
 
     # write a lobsterin file, including fatband analysis
     lobsterin = Lobsterin.standard_calculations_from_vasp_files(
         POSCAR_input=fposcar_dst,
@@ -1092,13 +1220,328 @@
                 if line.split("=")[0].strip() in new_incar_params:
                     continue
                 f_dst.write(line)
 
     return parchg_dir
 
 
+def setup_dfpt(converged_static_dir, supercell_grid=[2, 2, 2], rerun=False):
+    """
+    function to create input files (INCAR, KPOINTS, POTCAR, POSCAR, WAVECAR, CHGCAR) for partial charge calculation
+        after static calculations
+
+    Args:
+        converged_static_dir (str)
+            path to converged static calculation
+
+        supercell_grid (list)
+            the supercell grid to create from original POSCAR
+
+        rerun (bool)
+            if True, rerun bandstructure calculation even if it's already converged
+
+    Returns:
+        directory to band structure calculation (str) or None if not ready to run this
+
+    """
+    # make sure static is converged
+    av = AnalyzeVASP(converged_static_dir)
+    if not av.is_converged:
+        print("static calculation not converged; not setting up dfpt calc yet")
+        return None
+
+    # get the paths to relevant input files from the static calculation
+    files_from_static = ["POSCAR", "KPOINTS", "POTCAR"]
+
+    # make a directory for the bandstructure calculation
+    dfpt_dir = converged_static_dir.replace("-static", "-dfpt")
+    if not os.path.exists(dfpt_dir):
+        os.mkdir(dfpt_dir)
+
+    # make sure dfpt calc didn't already run
+    av = AnalyzeVASP(dfpt_dir)
+    if av.is_converged and not rerun:
+        print("dfpt already converged")
+        return None
+
+    for file_to_copy in files_from_static:
+        f_src = os.path.join(converged_static_dir, file_to_copy)
+        f_dst = os.path.join(dfpt_dir, file_to_copy)
+        copyfile(f_src, f_dst)
+
+    copyfile(
+        os.path.join(dfpt_dir, "POSCAR"), os.path.join(dfpt_dir, "POSCAR-unitcell")
+    )
+    st_unit = StrucTools(os.path.join(dfpt_dir, "POSCAR-unitcell"))
+    supercell = st_unit.make_supercell(supercell_grid)
+    supercell.to(fmt="POSCAR", filename=os.path.join(dfpt_dir, "POSCAR"))
+
+    fstatic_incar = os.path.join(converged_static_dir, "INCAR")
+    fdfpt_incar = os.path.join(dfpt_dir, "INCAR")
+
+    new_incar_params = {
+        "IBRION": 7,
+        "NSW": 1,
+        "IALGO": 38,
+        "EDIFF": 1e-6,
+        "ADDGRID": True,
+        "ALGO": "Normal",
+        "ISYM": 2,
+    }
+
+    incar_params_to_exclude = ["NPAR", "NCORE"]
+
+    with open(fstatic_incar) as f_src:
+        with open(fdfpt_incar, "w") as f_dst:
+            for line in f_src:
+                if line.split("=")[0].strip() in new_incar_params:
+                    continue
+                if line.split("=")[0].strip() in incar_params_to_exclude:
+                    continue
+                if "MAGMOM" in line:
+                    magmom = line.split("=")[1].strip()
+                    magmoms = magmom.split(" ")
+                    new_magmoms = []
+                    for mag in magmoms:
+                        if mag:
+                            old_number = int(mag.split("*")[0])
+                            new_number = (
+                                old_number
+                                * supercell_grid[0]
+                                * supercell_grid[1]
+                                * supercell_grid[2]
+                            )
+                            old_mag = mag.split("*")[1]
+                            new_mag = old_mag
+                            new_magmoms.append("%s*%s" % (new_number, new_mag))
+                    f_dst.write("MAGMOM = %s\n" % " ".join(new_magmoms))
+                else:
+                    f_dst.write(line)
+            for key in new_incar_params:
+                f_dst.write("%s = %s\n" % (key, new_incar_params[key]))
+
+    fdfpt_kpoints = os.path.join(dfpt_dir, "KPOINTS")
+    with open(fdfpt_kpoints, "w") as f_dst:
+        f_dst.write("Regular\n")
+        f_dst.write("0 0 0\n")
+        f_dst.write("Gamma\n")
+        f_dst.write("1 1 1\n")
+
+    return dfpt_dir
+
+
+def generate_finite_displacements(
+    converged_static_dir, supercell_grid=[2, 2, 2], remake=False
+):
+    """
+    Args:
+        converged_static_dir (str)
+            path to converged static calculation
+
+        supercell_grid (list)
+            the supercell grid to create from original POSCAR
+
+    Returns:
+        phonon_dir
+            disp-*/
+            POSCAR-*
+    """
+    # make sure static is converged
+    av = AnalyzeVASP(converged_static_dir)
+    if not av.is_converged:
+        print("static calculation not converged; not setting up phonon calcs yet")
+        return None
+
+    # create a directory called phonons within the static directory
+    phonon_dir = os.path.join(converged_static_dir, "phonons")
+    if not os.path.exists(phonon_dir):
+        os.mkdir(phonon_dir)
+
+    # use my current directory as a reference point
+    curr_dir = os.getcwd()
+
+    # see if POSCARs are already created
+    created_poscars = os.listdir(phonon_dir)
+    created_poscars = [f for f in created_poscars if "POSCAR-" in f]
+
+    # go into the phonon directory and generate the displacement POSCARs
+    if remake or not created_poscars:
+        copyfile(
+            os.path.join(converged_static_dir, "CONTCAR"),
+            os.path.join(phonon_dir, "POSCAR"),
+        )
+        os.chdir(phonon_dir)
+        subprocess.call(
+            [
+                "phonopy",
+                "-d",
+                "--dim=%s %s %s"
+                % (
+                    str(supercell_grid[0]),
+                    str(supercell_grid[1]),
+                    str(supercell_grid[2]),
+                ),
+            ]
+        )
+        os.chdir(curr_dir)
+
+    # get the paths to relevant input files from the static calculation
+    files_from_static = ["KPOINTS", "POTCAR", "INCAR"]
+
+    # some special INCAR settings for the static calculations of each displacement
+    new_incar_params = {
+        "IBRION": 2,
+        "ISIF": 3,
+        "ENCUT": 700,
+        "EDIFF": 1e-7,
+        "LAECHG": False,
+        "LREAL": False,
+        "ALGO": "Normal",
+        "NSW": 0,
+        "LCHARG": False,
+    }
+
+    # copy KPOINTS, INCAR, POTCAR from the static calculation into phonon_dir
+    for file_to_copy in files_from_static:
+        f_src = os.path.join(converged_static_dir, file_to_copy)
+        f_dst = os.path.join(phonon_dir, file_to_copy)
+        copyfile(f_src, f_dst)
+
+    # modify the INCAR in the disp-* dir
+    with open(os.path.join(converged_static_dir, "INCAR")) as f_src:
+        with open(os.path.join(phonon_dir, "INCAR"), "w") as f_dst:
+            for key in new_incar_params:
+                f_dst.write("%s = %s\n" % (key, new_incar_params[key]))
+            for line in f_src:
+                if line.split("=")[0].strip() in new_incar_params:
+                    continue
+                if "MAGMOM" in line:
+                    magmom = line.split("=")[1].strip()
+                    magmoms = magmom.split(" ")
+                    new_magmoms = []
+                    for mag in magmoms:
+                        if mag:
+                            old_number = int(mag.split("*")[0])
+                            new_number = (
+                                old_number
+                                * supercell_grid[0]
+                                * supercell_grid[1]
+                                * supercell_grid[2]
+                            )
+                            old_mag = mag.split("*")[1]
+                            new_mag = old_mag
+                            new_magmoms.append("%s*%s" % (new_number, new_mag))
+                    f_dst.write("MAGMOM = %s\n" % " ".join(new_magmoms))
+                    continue
+                f_dst.write(line)
+
+    return phonon_dir
+
+
+def setup_finite_displacement_calcs(phonon_dir, remake=False, rerun=False):
+
+    # grab the created POSCARs
+    created_poscars = os.listdir(phonon_dir)
+    created_poscars = [f for f in created_poscars if "POSCAR-" in f]
+
+    # get the paths to relevant input files from the static calculation
+    files_from_static = ["KPOINTS", "POTCAR", "INCAR"]
+
+    # for each displacement,
+    # create a disp-00* directory,
+    # grab the POSCAR-00*,
+    # copy the static calculation files,
+    # modify the INCAR
+
+    statuses = {}
+
+    for poscar in created_poscars:
+        number = poscar.split("-")[-1]
+
+        # create disp-00* dir
+        disp_dir = os.path.join(phonon_dir, "disp-%s" % number)
+        if not os.path.exists(disp_dir):
+            os.mkdir(disp_dir)
+
+        statuses[number] = {"convergence": False, "calc_dir": disp_dir}
+
+        # copy the displaced POSCAR-00* into the disp-00* dir
+        poscar_src = os.path.join(phonon_dir, poscar)
+        poscar_dst = os.path.join(disp_dir, "POSCAR")
+        if not os.path.exists(poscar_dst) or remake:
+            copyfile(poscar_src, poscar_dst)
+
+        # check convergence
+        av = AnalyzeVASP(disp_dir)
+        if av.is_converged and not rerun:
+            statuses[number]["convergence"] = True
+            continue
+
+        # copy KPOINTS, INCAR, POTCAR from the phonon dir into disp_dir
+        for file_to_copy in files_from_static:
+            f_src = os.path.join(phonon_dir, file_to_copy)
+            f_dst = os.path.join(disp_dir, file_to_copy)
+            if not os.path.exists(f_dst) or remake:
+                copyfile(f_src, f_dst)
+
+    return statuses
+
+
+def setup_static_magtest(converged_static_dir, rerun=False):
+    # make sure relax is converged
+    av = AnalyzeVASP(converged_static_dir)
+    if not av.is_converged:
+        print("static calculation not converged; not setting up static mag test")
+        return None
+
+    relax_dir = converged_static_dir.replace("-static", "-relax")
+    av_relax = AnalyzeVASP(relax_dir)
+    if not av_relax.is_converged:
+        print("relax calculation not converged; not setting up static mag test")
+        return None
+
+    # get the paths to relevant input files from the static calculation
+    files_from_relax = ["POSCAR", "KPOINTS", "POTCAR", "INCAR", "WAVECAR", "CHGCAR"]
+
+    # make a directory for the magtest calculation
+    magtest_dir = converged_static_dir.replace("-static", "-static_magtest")
+    if not os.path.exists(magtest_dir):
+        os.mkdir(magtest_dir)
+
+    # make sure bandstructure calc didn't already run
+    av = AnalyzeVASP(magtest_dir)
+    if av.is_converged and not rerun:
+        print("magtest already converged")
+        return None
+
+    mag_decorated_relax_structure = get_structure_from_prev_run(
+        av_relax.outputs.vasprun, av_relax.outputs.outcar
+    )
+
+    magmom = mag_decorated_relax_structure.site_properties["magmom"]
+    magmom_string = " ".join([str(m) for m in magmom])
+
+    new_incar_params = {"MAGMOM": magmom_string}
+
+    for file_to_copy in files_from_relax:
+        f_src = os.path.join(converged_static_dir, file_to_copy)
+        f_dst = os.path.join(magtest_dir, file_to_copy)
+        copyfile(f_src, f_dst)
+
+    with open(os.path.join(converged_static_dir, "INCAR"), "r") as f_src:
+        with open(os.path.join(magtest_dir, "INCAR"), "w") as f_dst:
+            for key in new_incar_params:
+                f_dst.write("%s = %s\n" % (key, new_incar_params[key]))
+            for line in f_src:
+                if line.split("=")[0].strip() in new_incar_params:
+                    continue
+                f_dst.write(line)
+
+    return magtest_dir
+
+
 def main():
     return
 
 
 if __name__ == "__main__":
-    sub = main()
+    main()
```

### Comparing `pydmclab-1.0.3/pydmclab/hpc/vasp.py` & `pydmclab-1.1.4/pydmclab/hpc/vasp.py`

 * *Files 2% similar despite different names*

```diff
@@ -323,39 +323,42 @@
         if "NSW" not in modify_incar:
             if configs["calc_to_run"] == "static":
                 modify_incar["NSW"] = 0
             else:
                 modify_incar["NSW"] = 199
 
         # make sure spin is off for nm calculations
-        if configs["mag"] == "nm":
+        if (configs["mag"] == "nm") and ("ISPIN" not in modify_incar):
             modify_incar["ISPIN"] = 1
         else:
             # make sure magnetization is written to OUTCAR for magnetic calcs
             modify_incar["LORBIT"] = 11
 
         # if we are doing LOBSTER, need special parameters
         # note: some of this gets handled later for us
         if configs["lobster_static"] and (configs["calc_to_run"] == "static"):
             if configs["standard"] != "mp":
                 # want to write charge densities
                 # new NBANDS so don't want to start from WAVECAR
-                lobster_incar_settings = {"NEDOS": 800, "ISTART": 0, "LAECHG": True}
+                lobster_incar_settings = {"ISTART": 0, "LAECHG": True}
                 for key in lobster_incar_settings:
                     if key not in configs["lobster_incar"]:
-                        modify_incar[key] = lobster_incar_settings[key]
+                        if key not in modify_incar:
+                            modify_incar[key] = lobster_incar_settings[key]
 
                 for key in configs["lobster_incar"]:
-                    modify_incar[key] = configs["lobster_incar"][key]
+                    if key not in modify_incar:
+                        modify_incar[key] = configs["lobster_incar"][key]
 
-                if not configs["lobster_kpoints"]:
-                    # need KPOINTS file for LOBSTER (as opposed to KSPACING)
-                    modify_kpoints = {"length": 25}
-                else:
-                    modify_kpoints = configs["lobster_kpoints"]
+                if not modify_kpoints:
+                    if not configs["lobster_kpoints"]:
+                        # need KPOINTS file for LOBSTER (as opposed to KSPACING)
+                        modify_kpoints = {"length": 25}
+                    else:
+                        modify_kpoints = configs["lobster_kpoints"]
 
         if configs["lobster_static"]:
             if configs["xc_to_run"] == "metagga":
                 # gga-static will get ISYM = -1, so need to pass that to metagga relax otherwise WAVECAR from GGA doesnt help metagga
                 modify_incar["ISYM"] = -1
 
         if configs["generate_dielectric"]:
@@ -368,14 +371,18 @@
                 else:
                     warnings.warn(
                         "\nyou cannot run METAGGA and generate a dielectric. the METAGGA calculation will run but without a dielectric\n"
                     )
 
         print("modify_incar = %s" % modify_incar)
 
+        if configs["standard"] == "dmc":
+            if "W" not in modify_potcar:
+                modify_potcar["W"] = "W"
+
         # initialize new VASPSet with all our settings
         vasp_input = vaspset(
             structure,
             user_incar_settings=modify_incar,
             user_kpoints_settings=modify_kpoints,
             user_potcar_settings=modify_potcar,
             user_potcar_functional=potcar_functional,
@@ -479,14 +486,16 @@
             "posmap": ["POSMAP internal error: symmetry equivalent atom not found"],
             "point_group": ["Error: point group operation missing"],
             "ibzkpt": ["internal error in subroutine IBZKPT"],
             "bad_sym": [
                 "ERROR: while reading WAVECAR, plane wave coefficients changed"
             ],
             "num_prob": ["num prob"],
+            "sym_too_tight": ["try changing SYMPREC"],
+            "coef": ["while reading plane", "while reading WAVECAR"],
         }
 
     @property
     def unconverged_log(self):
         """
         checks to see if both ionic and electronic convergence have been reached
             if calculation had NELM # electronic steps, electronic convergence may not be met
@@ -644,14 +653,20 @@
         if "amin" in errors:
             incar_changes["AMIN"] = 0.01
         if "pricel" in errors:
             incar_changes["SYMPREC"] = 1e-8
             incar_changes["ISYM"] = 0
         if "num_prob" in errors:
             incar_changes["ISMEAR"] = -1
+        if "sym_too_tight" in errors:
+            incar_changes["ISYM"] = -1
+            incar_changes["SYMPREC"] = 1e-3
+        if "coef" in errors:
+            if os.path.exists(wavecar):
+                os.remove(wavecar)
         return incar_changes
 
 
 def main():
     return
```

### Comparing `pydmclab-1.0.3/pydmclab/plotting/bs.py` & `pydmclab-1.1.4/pydmclab/plotting/bs.py`

 * *Files identical despite different names*

### Comparing `pydmclab-1.0.3/pydmclab/plotting/dos.py` & `pydmclab-1.1.4/pydmclab/plotting/dos.py`

 * *Files identical despite different names*

### Comparing `pydmclab-1.0.3/pydmclab/plotting/pd.py` & `pydmclab-1.1.4/pydmclab/plotting/pd.py`

 * *Files identical despite different names*

### Comparing `pydmclab-1.0.3/pydmclab/plotting/utils.py` & `pydmclab-1.1.4/pydmclab/plotting/utils.py`

 * *Files identical despite different names*

### Comparing `pydmclab-1.0.3/pydmclab/utils/handy.py` & `pydmclab-1.1.4/pydmclab/utils/handy.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 
 
 def make_project_tree():
     project_dir = os.getcwd()
     tree = {
         "dev": ["scripts", "data", "figures"],
         "results": ["scripts", "data", "figures"],
-        "prep": ["notes", "background"],
+        "background": ["notes"],
         "products": ["drafts", "slides", "other"],
     }
     for first_layer in tree:
         next_layers = tree[first_layer]
         for n in next_layers:
             that_layer = os.path.join(project_dir, first_layer, n)
             if not os.path.exists(that_layer):
```

### Comparing `pydmclab-1.0.3/pydmclab.egg-info/PKG-INFO` & `pydmclab-1.1.4/pydmclab.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: pydmclab
-Version: 1.0.3
+Version: 1.1.4
 Summary: Package to facilitate DFT calculations and analysis
 Home-page: https://github.umn.edu/bartel-group/pydmclab
 Author: Chris Bartel
 Author-email: cbartel@umn.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6.0
+Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 Provides-Extra: mlp
 Provides-Extra: defects
+Provides-Extra: phonons
 License-File: LICENSE.txt
 
 
 # pydmclab
 
 - common framework to rely upon for typical calculations and analysis done in the Bartel research group
```

### Comparing `pydmclab-1.0.3/setup.py` & `pydmclab-1.1.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,33 @@
 import io
 import os
 import sys
 from shutil import rmtree
+import numpy as np
 
-from setuptools import find_packages, setup, Command
+from setuptools import find_packages, setup, Command, find_namespace_packages
 
 NAME = "pydmclab"
 DESCRIPTION = "Package to facilitate DFT calculations and analysis"
 URL = "https://github.umn.edu/bartel-group/pydmclab"
 EMAIL = "cbartel@umn.edu"
 AUTHOR = "Chris Bartel"
-REQUIRES_PYTHON = ">=3.6.0"
-VERSION = "1.0.3"
+REQUIRES_PYTHON = ">=3.9.0"
+VERSION = "1.1.4"
 
-REQUIRED = ["numpy", "pymatgen"]
-EXTRAS = {"mlp": ["chgnet"], "defects": ["dscribe"]}
+REQUIRED = [
+    "numpy>=1.25.0",
+    "mp-api>=0.39",
+    "pymatgen>=2023.0.0",
+]
+EXTRAS = {
+    "mlp": ["chgnet"],
+    "defects": ["pymatgen-analysis-defects"],
+    "phonons": ["phonopy"],
+}
 here = os.path.abspath(os.path.dirname(__file__))
 try:
     with io.open(os.path.join(here, "README.md"), encoding="utf-8") as f:
         long_description = "\n" + f.read()
 except FileNotFoundError:
     long_description = DESCRIPTION
 
@@ -72,22 +81,23 @@
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type="text/markdown",
     author=AUTHOR,
     author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
     url=URL,
-    packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
-    package_data={"pydmclab": ["pydmclab/data/data/*"]},
+    packages=find_namespace_packages(include=["pydmclab.*", "pydmclab.**.*"]),
+    package_data={"pydmclab.data.data": ["*.json", "*.yaml", "*.csv", "*.dat"]},
     install_requires=REQUIRED,
     extras_require=EXTRAS,
     include_package_data=True,
     license="MIT",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     cmdclass={
         "upload": UploadCommand,
     },
+    include_dirs=[np.get_include()],
 )
```

